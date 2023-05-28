# Comparing `tmp/tfc-1.0.3.tar.gz` & `tmp/tfc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfc-1.0.3.tar", last modified: Mon Feb 13 01:30:35 2023, max compression
+gzip compressed data, was "tfc-1.0.4.tar", last modified: Sun May 28 15:29:28 2023, max compression
```

## Comparing `tfc-1.0.3.tar` & `tfc-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.170803 tfc-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-13 01:30:28.000000 tfc-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-13 01:30:28.000000 tfc-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-02-13 01:30:35.170803 tfc-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-02-13 01:30:28.000000 tfc-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-13 01:30:28.000000 tfc-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 01:30:35.170803 tfc-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-02-13 01:30:28.000000 tfc-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.166803 tfc-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.166803 tfc-1.0.3/src/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/mtfc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utfc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.170803 tfc-1.0.3/src/tfc/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.170803 tfc-1.0.3/src/tfc/utils/BF/
--rw-r--r--   0 runner    (1001) docker     (123)    44710 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/BF.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/BF.h
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/BF.i
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/BF.py
--rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/BF_Py.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/BF/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/CeSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/Html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/Latex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/MakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/MayaviMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/PlotlyMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    56898 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/TFCUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-13 01:30:28.000000 tfc-1.0.3/src/tfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:30:35.166803 tfc-1.0.3/src/tfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-02-13 01:30:35.000000 tfc-1.0.3/src/tfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-13 01:30:35.000000 tfc-1.0.3/src/tfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 01:30:35.000000 tfc-1.0.3/src/tfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-13 01:30:35.000000 tfc-1.0.3/src/tfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 01:30:35.000000 tfc-1.0.3/src/tfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.593680 tfc-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 15:29:14.000000 tfc-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 15:29:14.000000 tfc-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-28 15:29:28.593680 tfc-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-28 15:29:14.000000 tfc-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-28 15:29:14.000000 tfc-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:29:28.593680 tfc-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-28 15:29:14.000000 tfc-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/mtfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utfc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.593680 tfc-1.0.4/src/tfc/utils/BF/
+-rw-r--r--   0 runner    (1001) docker     (123)    44710 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.i
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF_Py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/CeSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/MakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/MayaviMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/PlotlyMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58246 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/TFCUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/top_level.txt
```

### Comparing `tfc-1.0.3/LICENSE` & `tfc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/PKG-INFO` & `tfc-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -71,25 +71,25 @@
 ```
 Note that you may need to first install the system package dependencies listed in the [**Building from source**](#building-from-source) section if they are not already installed.
 
 ## Reference Documentation:
 For tutorials on how to use this package as well as information about the tfc API, see the [reference documentation](https://tfc-documentation.readthedocs.io/en/latest/).
 
 ## Mathematical Documentation:
-Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the TFC textbook is available for purchase [here](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4).
+Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the [TFC textbook](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4) is available for purchase.
 
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.3},
-    year = {2022},
+    version = {1.0.4},
+    year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303}, 
     DOI={10.3390/math8081303},
```

### Comparing `tfc-1.0.3/README.md` & `tfc-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,25 +53,25 @@
 ```
 Note that you may need to first install the system package dependencies listed in the [**Building from source**](#building-from-source) section if they are not already installed.
 
 ## Reference Documentation:
 For tutorials on how to use this package as well as information about the tfc API, see the [reference documentation](https://tfc-documentation.readthedocs.io/en/latest/).
 
 ## Mathematical Documentation:
-Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the TFC textbook is available for purchase [here](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4).
+Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the [TFC textbook](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4) is available for purchase.
 
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.3},
-    year = {2022},
+    version = {1.0.4},
+    year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303}, 
     DOI={10.3390/math8081303},
```

### Comparing `tfc-1.0.3/pyproject.toml` & `tfc-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/setup.py` & `tfc-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/mtfc.py` & `tfc-1.0.4/src/tfc/mtfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utfc.py` & `tfc-1.0.4/src/tfc/utfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/BF.cxx` & `tfc-1.0.4/src/tfc/utils/BF/BF.cxx`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/BF.h` & `tfc-1.0.4/src/tfc/utils/BF/BF.h`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/BF.i` & `tfc-1.0.4/src/tfc/utils/BF/BF.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/BF.py` & `tfc-1.0.4/src/tfc/utils/BF/BF.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/BF_Py.py` & `tfc-1.0.4/src/tfc/utils/BF/BF_Py.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/BF/numpy.i` & `tfc-1.0.4/src/tfc/utils/BF/numpy.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/CeSolver.py` & `tfc-1.0.4/src/tfc/utils/CeSolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sympy as sp
 from sympy import Expr
 from sympy.core.function import AppliedUndef
 from sympy.printing.pycode import PythonCodePrinter
-from .types import ConstraintOperators, Exprs, Union, Any, Literal
+from sympy.simplify.simplify import nc_simplify
+from .types import ConstraintOperators, Exprs, Union, Any, Literal, ConstraintOperator
 from .TFCUtils import TFCPrint
 from sympy import latex
 
 
 class CeSolver:
     """
     Constrained expression solver.
@@ -64,14 +65,16 @@
 
     def __init__(self, C: ConstraintOperators, kappa: Exprs, s: Exprs, g: Union[AppliedUndef, Any]):
         self._C = C
         self._K = kappa
         self._s = s
         self._g = g
         self._ce_stale: bool = True
+        self._S_stale: bool = True
+        self._alpha_stale: bool = True
         self._phi_stale: bool = True
         self._rho_stale: bool = True
 
     @property
     def print_type(self) -> Literal["tfc", "pretty", "latex", "str"]:
         return self._print_type
 
@@ -131,18 +134,16 @@
 
         Returns
         -------
         Any
             Switching functions.
         """
         if self._phi_stale:
-            S = sp.Matrix([[c(s) for s in self._s] for c in self._C])
-            alpha = S.inv()
             s_vec = sp.Matrix([s for s in self._s])
-            self._phi = s_vec.transpose() * alpha
+            self._phi = s_vec.transpose() * self.alpha
             self._phi_stale = False
         return self._phi
 
     @phi.setter
     def phi(self, phi: Any):
         """
         Set the switching functions.
@@ -152,25 +153,81 @@
         phi : Any
             The switching functions.
         """
         self._phi = phi
         self._phi_stale = False
 
     @property
+    def alpha(self) -> sp.Matrix:
+        """
+        Alpha matrix (inverse of the support matrix)
+
+        Returns
+        sp.Matrix
+            alpha matrix. The elements are on the field over which
+            the constrained expression is defined.
+        """
+        if self._alpha_stale:
+            self._alpha = self.S.inv()
+            self._alpha_stale = False
+        return self._alpha
+
+    @property
+    def S(self) -> sp.Matrix:
+        """
+        Support matrix.
+
+        Returns
+        sp.Matrix
+            Support matrix. The elements are on the field over which
+            the constrained expression is defined.
+        """
+
+        def _applyC(c, s) -> Any:
+            """
+            Apply the constraint operator to the switching function.
+
+            Parameters
+            ----------
+            c : ConstraintOperator
+                Constraint operator.
+            s : Expr
+                Switching function.
+
+            Returns
+            -------
+            Any
+                c(s), which is a number on the field over which the
+                constrained expression is defined.
+            """
+
+            dark = c(s)
+            if isinstance(dark, sp.Matrix) or isinstance(dark, sp.MatMul):
+                dark = nc_simplify(dark)[0]
+            return dark
+
+        if self._S_stale:
+            self._S = sp.Matrix([[_applyC(c, s) for s in self._s] for c in self._C])
+            self._S_stale = False
+        return self._S
+
+    @property
     def rho(self) -> Any:
         """
         Projection functionals.
 
         Returns
         -------
         Any
             Projection functionals.
         """
         if self._rho_stale:
-            self._rho = sp.Matrix([kappa - self._C[k](self._g) for k, kappa in enumerate(self._K)])
+            self._rho = sp.Matrix(
+                [sp.Add(kappa, -self._C[k](self._g)) for k, kappa in enumerate(self._K)]
+            )
         return self._rho
 
     @property
     def s(self) -> Exprs:
         """
         Switching functions.
 
@@ -191,14 +248,16 @@
         s : Exprs
             This is a tuple or list of the support functions. These should be given
             in terms of sympy symbols and constants. For example, if we wanted to
             use the constant function x = 1 as a support function, then we would
             use sympy.re(1) in this iterable.
         """
         self._s = s
+        self._S_stale = True
+        self._alpha_stale = True
         self._phi_stale = True
         self._ce_stale = True
 
     @property
     def kappa(self):
         """
         Kappa values.
@@ -248,14 +307,16 @@
             iterable should be a Python function that takes in a sympy function,
             such as `g(x)`, and outputs that function evaluated in the same way
             as the function in the constraint. For example, if the constraint was
             u(3) = 0, then the assocaited constraint operator would be:
             `lambda u: = u.subs(x,3)`.
         """
         self._C = C
+        self._S_stale = True
+        self._alpha_stale = True
         self._phi_stale = True
         self._rho_stale = True
         self._ce_stale = True
 
     @property
     def g(self) -> Union[AppliedUndef, Any]:
         """
@@ -283,15 +344,15 @@
         self._ce_stale = True
         self._rho_stale = True
 
     def _solveCe(self) -> None:
         """
         Solves the constrained expression and stores it in self.ce
         """
-        self._ce = self.g + (self.phi * self.rho)[0]
+        self._ce = sp.Add(self.g, (self.phi * self.rho)[0])
 
     def checkCe(self) -> bool:
         """
         Checks the constrained expression stored in the class against the stored constraints.
 
         Return
         ------
```

### Comparing `tfc-1.0.3/src/tfc/utils/Html.py` & `tfc-1.0.4/src/tfc/utils/Html.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/Latex.py` & `tfc-1.0.4/src/tfc/utils/Latex.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/MakePlot.py` & `tfc-1.0.4/src/tfc/utils/MakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/MayaviMakePlot.py` & `tfc-1.0.4/src/tfc/utils/MayaviMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/PlotlyMakePlot.py` & `tfc-1.0.4/src/tfc/utils/PlotlyMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.3/src/tfc/utils/TFCUtils.py` & `tfc-1.0.4/src/tfc/utils/TFCUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1685,7 +1685,49 @@
 
     Returns
     -------
     step_x : np.ndarray
         step(x)
     """
     return np.heaviside(x, 0)
+
+
+def criuCheckpoint(dir: str = "criu_checkpoint", user_mode: bool = False):
+    """
+    Use CRIU to create a checkpoint of your program.
+    WARNING: You must ensure no external sockets are used, i.e., via matplotlib.
+    WARNING: GPU memory cannot be mapped for all GPUs.
+    WARNING: user_mode is a work in progress and is not full featured yet.
+
+    Parameters
+    ----------
+    dir : str
+        Directory where the CRIU checkpoint will be created.
+    user_mode : bool
+        Whether to use user mode or not. (Default value = False)
+    """
+
+    import os
+    from pathlib import Path
+
+    path = Path(dir)
+    pid = os.getpid()
+
+    # Create path if it does not exist
+    if not os.path.exists(path):
+        os.mkdir(path)
+
+    # Run the command and print how to restart
+    if user_mode:
+        os.system(
+            f"(criu dump --unpriviledged -t {pid} -D {str(path.absolute())} --shell-job --leave-running &) &"
+        )
+        print(
+            f'Creating a checkpoint. To restart run: "sudo criu restore -D {str(path.absolute())} --shell-job'
+        )
+    else:
+        os.system(
+            f"(sudo criu dump -t {pid} -D {str(path.absolute())} --shell-job --leave-running &) &"
+        )
+        print(
+            f'Creating a checkpoint. To restart run: "sudo criu restore -D {str(path.absolute())} --shell-job'
+        )
```

### Comparing `tfc-1.0.3/src/tfc/utils/types.py` & `tfc-1.0.4/src/tfc/utils/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 from typing import Union, Any, Callable
 import numpy as np
 import numpy.typing as npt
-import jax.numpy as jnp
-from jaxtyping import Array
+from jax import Array
 from sympy.core.function import AppliedUndef
 from sympy import Expr
 
 if sys.version_info >= (3, 8):
     from typing import Literal, Protocol, TypedDict
 else:
     from typing_extensions import Literal, Protocol, TypedDict
```

### Comparing `tfc-1.0.3/src/tfc.egg-info/PKG-INFO` & `tfc-1.0.4/src/tfc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -71,25 +71,25 @@
 ```
 Note that you may need to first install the system package dependencies listed in the [**Building from source**](#building-from-source) section if they are not already installed.
 
 ## Reference Documentation:
 For tutorials on how to use this package as well as information about the tfc API, see the [reference documentation](https://tfc-documentation.readthedocs.io/en/latest/).
 
 ## Mathematical Documentation:
-Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the TFC textbook is available for purchase [here](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4).
+Any users interested in the process for developing constrained expressions, the mathematical theory behind TFC, and the application of TFC to differential equations should start with this [journal article](https://www.mdpi.com/2227-7390/8/8/1303); note that the article is open access, so you can download it for free. The curious user can continue their study of the mathematical theory by visiting the [TFC article repository](https://www.researchgate.net/project/Theory-of-Functional-Connections) on ResearchGate for a complete list of TFC publications with free downloadable PDFs. Furthermore, links to free downloadable versions of Hunter's and Carl's dissertations can be found in the READMEs of their respective folders in the `examples` directory. Finally, the [TFC textbook](https://www.lulu.com/en/us/shop/daniele-mortari-and-hunter-johnston-and-carl-leake/the-theory-of-functional-connections/hardcover/product-ve2ren.html?page=1&pageSize=4) is available for purchase.
 
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.3},
-    year = {2022},
+    version = {1.0.4},
+    year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303}, 
     DOI={10.3390/math8081303},
```

### Comparing `tfc-1.0.3/src/tfc.egg-info/SOURCES.txt` & `tfc-1.0.4/src/tfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

