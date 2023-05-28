# Comparing `tmp/simple_minimizer-1.0.3.tar.gz` & `tmp/simple_minimizer-1.1.0.tar.gz`

## Comparing `simple_minimizer-1.0.3.tar` & `simple_minimizer-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/make_project.sh
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/test.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/src/simple_minimizer/__init__.py
--rwxr-xr-x   0        0        0    12209 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/src/simple_minimizer/minimizer.py
--rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/src/simple_minimizer/vertex.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/LICENSE
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 simple_minimizer-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/make_project.sh
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/__init__.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/logistic_constraints.py
+-rwxr-xr-x   0        0        0    13572 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/minimizer.py
+-rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/vertex.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/PKG-INFO
```

### Comparing `simple_minimizer-1.0.3/src/simple_minimizer/minimizer.py` & `simple_minimizer-1.1.0/src/simple_minimizer/minimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Copyright (C) 2018 TJ Radcliffe
+# Copyright (C) 2018, 2023 TJ Radcliffe
 # Licenced under GPL 3.0
 
 from .vertex import CopyVertex, EmptyVertex, SimpleVertex
 
 import copy
 from math import sqrt
 import random
 
+mapConvergenceReasons = {-1: "Exceeded iteration limit", 1: "Closest points indistinguishable", 
+                                                2: "Met fractional tolerance", 3:"Minimum scale achieved"}
+
 """ Simple minimizer class applies a simple sequential axial minimization.
 It does a simple bracketing followed by a parabolic interpolation to 
 the minimum along each axis in sequence, repeating with reduced scale
 until the scale is small.  This is a crude but extremely effective way 
 of decoupling parameters during registration.  If you have an objective
 function that goes negative, add a constant to it that is sufficient to
 get the minimum around +1.
@@ -26,24 +29,30 @@
         # The thing we are minimizing
         self.pObjective = None
 
         # All the points we have sampled
         self.lstHistory = [EmptyVertex(nDimension)]
 
         # The scale along each axis (used to determine sampling sphere)
-        self.lstScales = [1.0 for nI in range(0, nDimension)]
+        self.lstScales = [1.0 for nI in range(nDimension)]
+
+        # Set the order or lock out dimensions
+        self.lstOrder = [nI for nI in range(nDimension)]
 
         # The points that did not improve things
         self.lstBadPoints = []
 
         # The fractional radial scale (sampling sphere is this fraction of scale along each axis)
         self.fRadialScale = 1.0
 
         # The radial scale at which to stop minimizing
         self.fMinimumScale = 0.001
+        
+        # Fractional tolerance to quit
+        self.fFractionalTolerance = 0.001
 
         # The maximum number of iterations of the outermost loop before giving up
         self.nMaxIterations = 1000
 
         # The best value of the objective 
         self.fBest = 1e8
 
@@ -65,19 +74,39 @@
     # Objective is what we are minimizing
     def setObjective(self, pObjective):
         self.pObjective = pObjective
 
     # Set the scale for a given axis.  This determines the initial range of search
     def setScale(self, nAxis, fScale):
         self.lstScales[nAxis] = fScale
+
+    # Disable minimization on a given dimension
+    def disableAxis(self, nAxis):
+        self.lstMask[nAxis] = -1
+
+    # Enable minimization on a given dimension (will place it in axis order)
+    def enableAxis(self, nAxis):
+        self.lstMask[nAxis] = nAxis
+        
+    # Determines when we are close enough to minumum (default is 0.001)
+    def setFractionalTolerance(self, fFractionalTolerance):
+        self.fFractionalTolerance = fFractionalTolerance
         
     # Set the scales (initial range of search) for all axes
     def setScales(self, lstScales):
         self.lstScales = lstScales
 
+    # Set the order of minimization. -1 means omit. Use carefully!
+    def setOrder(self, lstOrder):
+        self.lstOrder = lstOrder
+
+    # Reset the order of minimization to the default (in axis order)
+    def resetOrder(self, lstOrder):
+        self.lstOrder = [nI for nI in range(self.nDimension)]
+
     # Set the starting position on a given axis
     def setStart(self, nAxis, fStart):
         self.lstHistory[0].setVertex(nAxis, fStart)
 
     # Set the starting position on all axes
     def setStarts(self, lstStart):
         self.lstHistory[0].lstVertex = lstStart
@@ -106,14 +135,18 @@
     def getValue(self):
         return self.lstHistory[-1].getValue()
 
     # Get the best vertex
     def getMinimum(self):
         return self.lstHistory[-1].getVertex()
 
+    # Get reason for convergence
+    def getConvergenceReason(self, nReason):
+        return mapConvergenceReasons[nReason]
+
     # Axial minimization
     def minimize(self, lstStart = None):
         """
         Minimize by minimizations along successive axes.  This is the same
         techinque used in the original pseudo-correlation work, and it has the
         advantage of decoupling the rotation from the translation as much as
         possible.
@@ -130,28 +163,29 @@
         self.traceOpen()        # open output stream if requested
         self.traceOut()         # dump starting point if we have a trace file
         self.fRadialScale = 1.0
         nReason = 0    # reason for quiting
         while True:
             self.fSecondBest = self.fBest;    # record old best value
 
-            for nAxis in range(0, self.nDimension):
-                self.fBest = self.minimizeOne(nAxis);    # minimize along the given axis
+            for nAxis in self.lstOrder:
+                if nAxis >= 0 and nAxis < self.nDimension:
+                    self.fBest = self.minimizeOne(nAxis);    # minimize along the given axis
 
             self.fRadialScale *= 0.3183098861; # ~1/pi (any ~irrational will do)
             nCount += 1
             if self.nMaxIterations < nCount:   # bail out if we are stuck
                 nReason = -1
                 break;
                 
             # for floating-point minimiation 0.001 is a reasonable tolerance
             if (self.fBest+self.fSecondBest) == 0:
                 nReason = 1
                 break
-            elif (abs(self.fBest-self.fSecondBest)/(self.fBest+self.fSecondBest) <= 0.001):
+            elif (abs(self.fBest-self.fSecondBest)/(self.fBest+self.fSecondBest) <= self.fFractionalTolerance):
                 nReason = 2
                 break
             elif (self.fRadialScale <= self.fMinimumScale):
                 nReason = 3
                 break
 
         return (nCount, self.lstHistory[-1], nReason);
```

### Comparing `simple_minimizer-1.0.3/src/simple_minimizer/vertex.py` & `simple_minimizer-1.1.0/src/simple_minimizer/vertex.py`

 * *Files identical despite different names*

### Comparing `simple_minimizer-1.0.3/.gitignore` & `simple_minimizer-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_minimizer-1.0.3/LICENSE` & `simple_minimizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_minimizer-1.0.3/README.md` & `simple_minimizer-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 Simple usage example:
 
 ```
 from math import sqrt
 
 from simple_minimizer import *
-from simple_vertex import *
 
 nDimension = 3
 
 # objective function is a callable
 class Test(object):
     def __init__(self):
         # place we are looking for
@@ -61,15 +60,15 @@
 minimizer = SimpleMinimizer(nDimension)
 test = Test()
 minimizer.setObjective(test)
 
 # nReason = -1 => failed to converge, 1 => best/second-best equal, 2 => ratio < 0.001, 3 => minimum scale
 (nCount, vertex, nReason) = minimizer.minimize()
 lstVertex = vertex.getVertex() # extract the list of floats from the vertex object
-fValue = vertext.getValue() # the value of the objective function at the minimum
+fValue = vertex.getValue() # the value of the objective function at the minimum
 fError = sqrt(sum([(nI-lstVertex[nI])**2 for nI in range(0,nDimension)])/nDimension)
 print(fError < 0.001)
 print(nCount < 10)
 print(lstVertex)
     
 ```
```

### Comparing `simple_minimizer-1.0.3/pyproject.toml` & `simple_minimizer-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple-minimizer"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="TJ Radcliffe", email="tj@tjradcliffe.com" },
 ]
 description = "A brutally simple, extremely robust minimizer"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `simple_minimizer-1.0.3/PKG-INFO` & `simple_minimizer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-minimizer
-Version: 1.0.3
+Version: 1.1.0
 Summary: A brutally simple, extremely robust minimizer
 Project-URL: Homepage, https://github.com/tjradcliffe/simple-minimizer
 Project-URL: Bug Tracker, https://github.com/tjradcliffe/simple-minimizer/issues
 Author-email: TJ Radcliffe <tj@tjradcliffe.com>
 License: Copyright (c) 2022 Thomas J. Radcliffe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,14 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Simple Minimizer
@@ -66,15 +67,14 @@
 
 Simple usage example:
 
 ```
 from math import sqrt
 
 from simple_minimizer import *
-from simple_vertex import *
 
 nDimension = 3
 
 # objective function is a callable
 class Test(object):
     def __init__(self):
         # place we are looking for
@@ -93,15 +93,15 @@
 minimizer = SimpleMinimizer(nDimension)
 test = Test()
 minimizer.setObjective(test)
 
 # nReason = -1 => failed to converge, 1 => best/second-best equal, 2 => ratio < 0.001, 3 => minimum scale
 (nCount, vertex, nReason) = minimizer.minimize()
 lstVertex = vertex.getVertex() # extract the list of floats from the vertex object
-fValue = vertext.getValue() # the value of the objective function at the minimum
+fValue = vertex.getValue() # the value of the objective function at the minimum
 fError = sqrt(sum([(nI-lstVertex[nI])**2 for nI in range(0,nDimension)])/nDimension)
 print(fError < 0.001)
 print(nCount < 10)
 print(lstVertex)
     
 ```
```

