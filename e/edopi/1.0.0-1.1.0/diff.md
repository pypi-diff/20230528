# Comparing `tmp/edopi-1.0.0.tar.gz` & `tmp/edopi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edopi-1.0.0.tar", last modified: Fri Jul 16 00:36:34 2021, max compression
+gzip compressed data, was "edopi-1.1.0.tar", last modified: Sun May 28 18:59:55 2023, max compression
```

## Comparing `edopi-1.0.0.tar` & `edopi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-07-16 00:36:34.056632 edopi-1.0.0/
--rw-rw-rw-   0        0        0     1259 2021-07-16 00:36:34.055633 edopi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      619 2021-05-26 20:37:32.000000 edopi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2021-07-16 00:36:33.959688 edopi-1.0.0/edopi/
--rw-rw-rw-   0        0        0       91 2021-07-07 22:39:13.000000 edopi-1.0.0/edopi/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-16 00:36:34.052634 edopi-1.0.0/edopi/domain/
--rw-rw-rw-   0        0        0      219 2021-07-07 22:47:31.000000 edopi-1.0.0/edopi/domain/__init__.py
--rw-rw-rw-   0        0        0     5862 2021-07-07 22:46:53.000000 edopi-1.0.0/edopi/domain/balzano_diagram.py
--rw-rw-rw-   0        0        0     3140 2021-07-07 22:42:24.000000 edopi-1.0.0/edopi/domain/chroma.py
--rw-rw-rw-   0        0        0     3161 2021-07-07 22:46:41.000000 edopi-1.0.0/edopi/domain/gcycle.py
--rw-rw-rw-   0        0        0     8354 2021-07-07 22:46:29.000000 edopi-1.0.0/edopi/domain/scale.py
--rw-rw-rw-   0        0        0     3254 2021-07-07 22:47:02.000000 edopi-1.0.0/edopi/domain/tonal_system.py
--rw-rw-rw-   0        0        0      428 2021-04-10 18:46:37.000000 edopi-1.0.0/edopi/domain/utils.py
-drwxrwxrwx   0        0        0        0 2021-07-16 00:36:34.012658 edopi-1.0.0/edopi.egg-info/
--rw-rw-rw-   0        0        0     1259 2021-07-16 00:36:32.000000 edopi-1.0.0/edopi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2021-07-16 00:36:32.000000 edopi-1.0.0/edopi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-16 00:36:32.000000 edopi-1.0.0/edopi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-07-16 00:36:32.000000 edopi-1.0.0/edopi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-07-16 00:36:32.000000 edopi-1.0.0/edopi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-16 00:36:34.056632 edopi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      647 2021-07-16 00:34:55.000000 edopi-1.0.0/setup.py
+drwxr-xr-x   0 luansimoes  (1000) luansimoes  (1000)        0 2023-05-28 18:59:55.463804 edopi-1.1.0/
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     1060 2023-05-28 18:29:39.000000 edopi-1.1.0/LICENSE.txt
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      974 2023-05-28 18:59:55.463804 edopi-1.1.0/PKG-INFO
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      589 2023-05-28 18:29:39.000000 edopi-1.1.0/README.md
+drwxr-xr-x   0 luansimoes  (1000) luansimoes  (1000)        0 2023-05-28 18:59:55.457137 edopi-1.1.0/edopi/
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)       91 2023-05-28 18:29:39.000000 edopi-1.1.0/edopi/__init__.py
+drwxr-xr-x   0 luansimoes  (1000) luansimoes  (1000)        0 2023-05-28 18:59:55.460471 edopi-1.1.0/edopi/domain/
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      214 2023-05-28 18:29:39.000000 edopi-1.1.0/edopi/domain/__init__.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     5707 2023-05-28 18:29:39.000000 edopi-1.1.0/edopi/domain/balzano_diagram.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     3229 2023-05-28 18:32:38.000000 edopi-1.1.0/edopi/domain/chroma.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     3082 2023-05-28 18:29:39.000000 edopi-1.1.0/edopi/domain/gcycle.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)    10143 2023-05-28 18:54:17.000000 edopi-1.1.0/edopi/domain/scale.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     3333 2023-05-28 18:32:38.000000 edopi-1.1.0/edopi/domain/tonal_system.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      413 2023-05-28 18:29:39.000000 edopi-1.1.0/edopi/domain/utils.py
+drwxr-xr-x   0 luansimoes  (1000) luansimoes  (1000)        0 2023-05-28 18:59:55.460471 edopi-1.1.0/edopi.egg-info/
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      974 2023-05-28 18:59:55.000000 edopi-1.1.0/edopi.egg-info/PKG-INFO
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      488 2023-05-28 18:59:55.000000 edopi-1.1.0/edopi.egg-info/SOURCES.txt
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)        1 2023-05-28 18:59:55.000000 edopi-1.1.0/edopi.egg-info/dependency_links.txt
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)       17 2023-05-28 18:59:55.000000 edopi-1.1.0/edopi.egg-info/requires.txt
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)        6 2023-05-28 18:59:55.000000 edopi-1.1.0/edopi.egg-info/top_level.txt
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)       38 2023-05-28 18:59:55.463804 edopi-1.1.0/setup.cfg
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      649 2023-05-28 18:57:15.000000 edopi-1.1.0/setup.py
+drwxr-xr-x   0 luansimoes  (1000) luansimoes  (1000)        0 2023-05-28 18:59:55.463804 edopi-1.1.0/tests/
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     1213 2023-05-28 18:29:39.000000 edopi-1.1.0/tests/test_balzano_diagram.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     2367 2023-05-28 18:29:39.000000 edopi-1.1.0/tests/test_chroma.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)      494 2023-05-28 18:29:39.000000 edopi-1.1.0/tests/test_g_cycle.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     2454 2023-05-28 18:55:50.000000 edopi-1.1.0/tests/test_scale.py
+-rw-r--r--   0 luansimoes  (1000) luansimoes  (1000)     1320 2023-05-28 18:29:39.000000 edopi-1.1.0/tests/test_tonal_system.py
```

### Comparing `edopi-1.0.0/PKG-INFO` & `edopi-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1
-Name: edopi
-Version: 1.0.0
-Summary: Python package to deal with Group-Theoretic microtonal music structures
-Home-page: https://github.com/luansimoes/edopi
-Author: Flavia Elias e Luan Simões
-Author-email: luansimoes@id.uff.br
-License: MIT License
-Description: # EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
-        
-        ### Installation
-        ```
-        pip install edopi
-        ```
-        
-        ### Get started
-        How to generate the main structures and visualizations:
-        
-        ```Python
-        from edopi import TonalSystem
-        
-        # Instantiate a 12-EDO with generator 7
-        edo_12 = TonalSystem(12, 7)
-        
-        # Show the Chromatic representation
-        edo_12.show()
-        
-        # Show the cycle of Fifths
-        edo_12.show_gCycle()
-        
-        # Get the diatonic scale and show it
-        diatonic = edo_12.diatonic_scale()
-        diatonic.show()
-        
-        # Get Balzano Diagram and show it
-        b_diagram = edo_12.balzano_diagram(3, 4)
-        b_diagram.show()
-        ```
-        
-Keywords: microtonal edo music group-theoretic
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: edopi
+Version: 1.1.0
+Summary: Python package to deal with Group-Theoretic microtonal music structures
+Home-page: https://github.com/luansimoes/edopi
+Author: Flavia Elias e Luan Simões
+Author-email: luansimoes@cos.ufrj.br
+License: MIT License
+Keywords: microtonal edo music group-theoretic
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
+
+### Installation
+```
+pip install edopi
+```
+
+### Get started
+How to generate the main structures and visualizations:
+
+```Python
+from edopi import TonalSystem
+
+# Instantiate a 12-EDO with generator 7
+edo_12 = TonalSystem(12, 7)
+
+# Show the Chromatic representation
+edo_12.show()
+
+# Show the cycle of Fifths
+edo_12.show_gCycle()
+
+# Get the diatonic scale and show it
+diatonic = edo_12.diatonic_scale()
+diatonic.show()
+
+# Get Balzano Diagram and show it
+b_diagram = edo_12.balzano_diagram(3, 4)
+b_diagram.show()
+```
```

### Comparing `edopi-1.0.0/README.md` & `edopi-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
-
-### Installation
-```
-pip install edopi
-```
-
-### Get started
-How to generate the main structures and visualizations:
-
-```Python
-from edopi import TonalSystem
-
-# Instantiate a 12-EDO with generator 7
-edo_12 = TonalSystem(12, 7)
-
-# Show the Chromatic representation
-edo_12.show()
-
-# Show the cycle of Fifths
-edo_12.show_gCycle()
-
-# Get the diatonic scale and show it
-diatonic = edo_12.diatonic_scale()
-diatonic.show()
-
-# Get Balzano Diagram and show it
-b_diagram = edo_12.balzano_diagram(3, 4)
-b_diagram.show()
-```
+# EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
+
+### Installation
+```
+pip install edopi
+```
+
+### Get started
+How to generate the main structures and visualizations:
+
+```Python
+from edopi import TonalSystem
+
+# Instantiate a 12-EDO with generator 7
+edo_12 = TonalSystem(12, 7)
+
+# Show the Chromatic representation
+edo_12.show()
+
+# Show the cycle of Fifths
+edo_12.show_gCycle()
+
+# Get the diatonic scale and show it
+diatonic = edo_12.diatonic_scale()
+diatonic.show()
+
+# Get Balzano Diagram and show it
+b_diagram = edo_12.balzano_diagram(3, 4)
+b_diagram.show()
+```
```

### Comparing `edopi-1.0.0/edopi/domain/chroma.py` & `edopi-1.1.0/edopi/domain/chroma.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-import math
-
-class Chroma:
-    """
-    Instantiate a Tonal System Element.
-    Elements must have a chroma defined in a System. 
-    The System's cardinality acts as a module when operating microtonal chromas.
-    
-    :param pitch: A value that will be transformed into a chroma.
-    :type pitch: int
-
-    :param module: The cardinality of the System.
-    :type module: int
-    """
-
-    def __init__(self, pitch: int, module: int):
-        self.pitch_class = pitch % module
-        self.module = module
-
-        self.cents = self.pitch_class * (1200/self.module)
-        self.midi = (self.cents/100)
-    
-    @property
-    def is_generator(self):
-        return math.gcd(self.pitch_class, self.module)==1
-
-    def __add__(self, o):
-        assert isinstance(o, Chroma), f"Cannot add Chroma to {type(o)}"
-        assert self.module == o.module, "Cannot add elements of different modules"
-        return Chroma(self.pitch_class + o.pitch_class, self.module)
-
-    def __sub__(self, o):
-        assert isinstance(o, Chroma), f"Cannot subtract Chroma to {type(o)}"
-        assert self.module == o.module, "Cannot subtract elements of different modules"
-        return Chroma(self.pitch_class - o.pitch_class, self.module)
-
-    def __mul__(self, o):
-        assert isinstance(o, Chroma), f"Cannot multiply Chroma to {type(o)}"
-        assert self.module == o.module, "Cannot multiply elements of different modules"
-        return Chroma(self.pitch_class * o.pitch_class, self.module)
-    
-    def __truediv__(self, o):
-        assert isinstance(o, Chroma), f"Cannot divide Chroma to {type(o)}"
-        assert self.module == o.module, "Cannot divide elements of different modules"
-        assert o.is_generator, "Cannot divide by a zero-divisor element"
-        return self * o.inverse()
-
-    def __eq__(self, o):
-        return isinstance(o, Chroma) and self.pitch_class == o.pitch_class and self.module == o.module
-
-    def __gt__(self, o):
-        return isinstance(o, Chroma) and (self.pitch_class > o.pitch_class) and self.module == o.module
-
-    def __lt__(self, o):
-        return isinstance(o, Chroma) and self.pitch_class < o.pitch_class and self.module == o.module
-
-    def __le__(self, o):
-        return isinstance(o, Chroma) and self.pitch_class <= o.pitch_class and self.module == o.module
-
-    def __ge__(self, o):
-        return isinstance(o, Chroma) and self.pitch_class >= o.pitch_class and self.module == o.module
-
-    def inverse(self):
-        if math.gcd(self.pitch_class, self.module) != 1:
-            return None
-        else:
-            for i in range(self.module):
-                if (i * self.pitch_class) % self.module == 1:
-                    return Chroma(i, self.module)
-
-    def symmetrical(self):
-        return Chroma(-self.pitch_class, self.module)
-
-    def subgroup(self):
-        i = 1
-        pitch_class = self.pitch_class
-        while pitch_class!=0:
-            i+=1
-            pitch_class = (pitch_class+self.pitch_class)%self.module
-        return i
-    
-    def __str__(self):
-        return str(self.pitch_class)
+import math
+
+class Chroma:
+    """
+    Instantiate a Tonal System Element.
+    Elements must have a chroma defined in a System. 
+    The System's cardinality acts as a module when operating microtonal chromas.
+    
+    :param pitch: A value that will be transformed into a chroma.
+    :type pitch: int
+
+    :param module: The cardinality of the System.
+    :type module: int
+    """
+
+    def __init__(self, pitch: int, module: int):
+        self.pitch_class = pitch % module
+        self.module = module
+
+        self.cents = self.pitch_class * (1200/self.module)
+        self.midi = (self.cents/100)
+    
+    @property
+    def is_generator(self):
+        return math.gcd(self.pitch_class, self.module)==1
+
+    def __add__(self, o):
+        assert isinstance(o, (Chroma, int)), f"Cannot add Chroma to {type(o)}"
+        if isinstance(o, int): return Chroma(self.pitch_class+o, self.module)
+
+        assert self.module == o.module, "Cannot add elements of different modules"
+        return Chroma(self.pitch_class + o.pitch_class, self.module)
+
+    def __sub__(self, o):
+        assert isinstance(o, (Chroma, int)), f"Cannot subtract Chroma to {type(o)}"
+        if isinstance(o, int): return Chroma(self.pitch_class-o, self.module)
+
+        assert self.module == o.module, "Cannot subtract elements of different modules"
+        return Chroma(self.pitch_class - o.pitch_class, self.module)
+
+    def __mul__(self, o):
+        assert isinstance(o, Chroma), f"Cannot multiply Chroma to {type(o)}"
+        assert self.module == o.module, "Cannot multiply elements of different modules"
+        return Chroma(self.pitch_class * o.pitch_class, self.module)
+    
+    def __truediv__(self, o):
+        assert isinstance(o, Chroma), f"Cannot divide Chroma to {type(o)}"
+        assert self.module == o.module, "Cannot divide elements of different modules"
+        assert o.is_generator, "Cannot divide by a zero-divisor element"
+        return self * o.inverse()
+
+    def __eq__(self, o):
+        return isinstance(o, Chroma) and self.pitch_class == o.pitch_class and self.module == o.module
+
+    def __gt__(self, o):
+        return isinstance(o, Chroma) and (self.pitch_class > o.pitch_class) and self.module == o.module
+
+    def __lt__(self, o):
+        return isinstance(o, Chroma) and self.pitch_class < o.pitch_class and self.module == o.module
+
+    def __le__(self, o):
+        return isinstance(o, Chroma) and self.pitch_class <= o.pitch_class and self.module == o.module
+
+    def __ge__(self, o):
+        return isinstance(o, Chroma) and self.pitch_class >= o.pitch_class and self.module == o.module
+
+    def inverse(self):
+        if math.gcd(self.pitch_class, self.module) != 1:
+            return None
+        else:
+            for i in range(self.module):
+                if (i * self.pitch_class) % self.module == 1:
+                    return Chroma(i, self.module)
+
+    def symmetrical(self):
+        return Chroma(-self.pitch_class, self.module)
+
+    def subgroup(self):
+        i = 1
+        pitch_class = self.pitch_class
+        while pitch_class!=0:
+            i+=1
+            pitch_class = (pitch_class+self.pitch_class)%self.module
+        return i
+    
+    def __str__(self):
+        return str(self.pitch_class)
```

### Comparing `edopi-1.0.0/edopi/domain/gcycle.py` & `edopi-1.1.0/edopi/domain/gcycle.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from .chroma import Chroma
-from .scale import DiatonicScale
-from typing import Union
-import copy
-import numpy as np
-import matplotlib.pyplot as plt
-
-class GCycle:
-    """
-    Instantiate a G-Cycle of the Tonal System.
-    A G-Cycle is a generalized Cycle of Fifths - which is isomorph to the Group.
-    In most cases, there's no need to interact directly with this class.
-    
-    :param generator: The generator of the Cycle.
-    :type g: Chroma
-    """
-
-    def __init__(self, generator: Chroma):
-        assert generator.is_generator, 'GCycle must be initialized with a element that is a generator of the given system'
-        self.generator = generator
-        self.system_size = self.generator.module
-        self.elements = self.generate_cycle()
-        #self.scale_sizes = sorted([self.generator.inverse().pitch_class, self.generator.inverse().symmetrical().pitch_class])
-
-    def generate_cycle(self):
-        elements = [Chroma(0, self.system_size)]
-        for _ in range(self.system_size - 1):
-            elements.append(elements[-1] + self.generator)
-        return elements
-
-    #TODO: Gerar escala diatônica e pentatônica, dependendo das características
-    #TODO: Gerar no modo dórico generalizado
-    def diatonic_scale(self, tonic: int):
-        length = self.generator.inverse().pitch_class
-
-        start_element = Chroma(-self.generator.pitch_class, self.system_size)
-        
-        sc_elements = [start_element]
-        for _ in range(length-1):
-            sc_elements.append(sc_elements[-1]+self.generator)
-        sc_elements.sort()
-        sc_elements.append(sc_elements[0])
-
-        struct = tuple((sc_elements[i]-sc_elements[i-1]).pitch_class for i in range(1, len(sc_elements)))
-
-        return DiatonicScale(self.system_size, struct, self.generator, tonic=tonic, name="Diatonic Scale")
-
-    # TODO: return integer if elem is an integer
-    def next(self, elem: Union[Chroma, int], steps: int):
-        real_elem = Chroma(elem, self.system_size) if isinstance(elem, int) else elem
-        next_index = (self.elements.index(real_elem) + steps) % len(self.elements)
-        return copy.deepcopy(self.elements[next_index])
-
-    def show(self):
-        r = 10
-        angle = 2 * np.pi / self.system_size
-        x = [self.elements[0].pitch_class]
-        y = [r]
-
-        figure, axes = plt.subplots()
-        cycle = plt.Circle((0, 0), r, fill=False)
-        axes.add_artist(cycle)
-
-        for i in range(1, self.system_size + 1):
-            x.append(r * np.sin(i * angle))
-            y.append(r * np.cos(i * angle))
-
-        #plt.plot(x, y, markersize=20)
-        plt.plot(x, y, 'wo', markersize=20)
-        for i in range(self.system_size):
-            plt.text(x[i], y[i],self.elements[i], ha='center', va='center')
-        plt.axis('equal')
-        plt.axis('off')
-        plt.show()
-
-    def __str__(self):
-        resp_str = f'\n*************Cycle:***************\n'
-        resp_str += f'Elements: {[str(e) for e in self.elements]}\n'
-        #resp_str += f'Scale Sizes: {self.scale_sizes[0]} {self.scale_sizes[1]}'
+from .chroma import Chroma
+from .scale import DiatonicScale
+from typing import Union
+import copy
+import numpy as np
+import matplotlib.pyplot as plt
+
+class GCycle:
+    """
+    Instantiate a G-Cycle of the Tonal System.
+    A G-Cycle is a generalized Cycle of Fifths - which is isomorph to the Group.
+    In most cases, there's no need to interact directly with this class.
+    
+    :param generator: The generator of the Cycle.
+    :type g: Chroma
+    """
+
+    def __init__(self, generator: Chroma):
+        assert generator.is_generator, 'GCycle must be initialized with a element that is a generator of the given system'
+        self.generator = generator
+        self.system_size = self.generator.module
+        self.elements = self.generate_cycle()
+        #self.scale_sizes = sorted([self.generator.inverse().pitch_class, self.generator.inverse().symmetrical().pitch_class])
+
+    def generate_cycle(self):
+        elements = [Chroma(0, self.system_size)]
+        for _ in range(self.system_size - 1):
+            elements.append(elements[-1] + self.generator)
+        return elements
+
+    #TODO: Gerar escala diatônica e pentatônica, dependendo das características
+    #TODO: Gerar no modo dórico generalizado
+    def diatonic_scale(self, tonic: int):
+        length = self.generator.inverse().pitch_class
+
+        start_element = Chroma(-self.generator.pitch_class, self.system_size)
+        
+        sc_elements = [start_element]
+        for _ in range(length-1):
+            sc_elements.append(sc_elements[-1]+self.generator)
+        sc_elements.sort()
+        sc_elements.append(sc_elements[0])
+
+        struct = tuple((sc_elements[i]-sc_elements[i-1]).pitch_class for i in range(1, len(sc_elements)))
+
+        return DiatonicScale(self.system_size, struct, self.generator, tonic=tonic, name="Diatonic Scale")
+
+    # TODO: return integer if elem is an integer
+    def next(self, elem: Union[Chroma, int], steps: int):
+        real_elem = Chroma(elem, self.system_size) if isinstance(elem, int) else elem
+        next_index = (self.elements.index(real_elem) + steps) % len(self.elements)
+        return copy.deepcopy(self.elements[next_index])
+
+    def show(self):
+        r = 10
+        angle = 2 * np.pi / self.system_size
+        x = [self.elements[0].pitch_class]
+        y = [r]
+
+        figure, axes = plt.subplots()
+        cycle = plt.Circle((0, 0), r, fill=False)
+        axes.add_artist(cycle)
+
+        for i in range(1, self.system_size + 1):
+            x.append(r * np.sin(i * angle))
+            y.append(r * np.cos(i * angle))
+
+        #plt.plot(x, y, markersize=20)
+        plt.plot(x, y, 'wo', markersize=20)
+        for i in range(self.system_size):
+            plt.text(x[i], y[i],self.elements[i], ha='center', va='center')
+        plt.axis('equal')
+        plt.axis('off')
+        plt.show()
+
+    def __str__(self):
+        resp_str = f'\n*************Cycle:***************\n'
+        resp_str += f'Elements: {[str(e) for e in self.elements]}\n'
+        #resp_str += f'Scale Sizes: {self.scale_sizes[0]} {self.scale_sizes[1]}'
         return resp_str
```

### Comparing `edopi-1.0.0/edopi/domain/tonal_system.py` & `edopi-1.1.0/edopi/domain/tonal_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,92 @@
-from .gcycle import GCycle
-from .chroma import Chroma
-from .scale import Scale
-from .balzano_diagram import BalzanoDiagram
-from typing import Union
-import math
-
-class TonalSystem:
-    """
-    Instantiate a Tonal System.
-    A Tonal System is a group of n elements and it has a generator chosen as a generalized fifth. 
-    All the other structures are defined within a Tonal System.
-    
-    :param n: The number of elements.
-    :type n: int
-
-    :param g: The generalized fifth of the System.
-    :type g: int
-    """
-
-    def __init__(self, n: int, g=1):
-        assert n>1, "Tonal System must have more than one element"
-        self.cardinality = n
-        self._generator = Chroma(g, n)
-        self.cycle = GCycle(self._generator)
-
-    @property
-    def generators(self):
-        n = self.cardinality
-        return [x for x in range(n) if math.gcd(x, n)==1]
-
-    @property
-    def generator(self):
-        return self._generator.pitch_class
-    
-    @generator.setter
-    def generator(self, value):
-        self.set_generator(value)
-
-    def set_generator(self, g: Union[Chroma, int]):
-        if isinstance(g, int):
-            assert math.gcd(g, self.cardinality)==1, "Element must be a generator"
-            self._generator = Chroma(g, self.cardinality)
-        elif isinstance(g, Chroma):
-            assert g.is_generator, "Element must be a generator"
-            self._generator = g
-        self.cycle = GCycle(self._generator)
-
-    def scale(self, elements=[], struct=[], name='Generic Scale'):
-        assert (len(elements)==0) ^ (len(struct)==0), "argument must be either elements or struct"
-        if len(elements)!=0:
-            elements.sort()
-            if all(isinstance(e, Chroma) for e in elements):
-                circle_elements = elements + [elements[0]]
-            elif all(isinstance(e, int) for e in elements):
-                circle_elements = [Chroma(e, self.cardinality) for e in elements] + [Chroma(elements[0], self.cardinality)]
-
-            struct = tuple((circle_elements[i]-circle_elements[i-1]).pitch_class for i in range(1, len(circle_elements)))
-
-        return Scale(self.cardinality, struct, name=name)
-
-    def diatonic_scale(self):
-        return self.cycle.diatonic_scale(0)
-    
-    def chromatic_scale(self):
-        struct = tuple([1 for _ in range(self.cardinality)])
-        return Scale(self.cardinality, struct, name=f'{self.cardinality}EDO Chromatic Scale')
-
-    # TODO: Figure out another way to do this
-    def midi_pitch(self, pitch_class: int, oct=0):
-        oct+=2
-        if oct==2:
-            oct += int(pitch_class//self.cardinality) - 2
-        return Chroma(pitch_class, self.cardinality).midi + (12*oct)
-
-    def balzano_diagram(self, minor: int, major: int):
-        n = self.cardinality
-        assert Chroma(minor+major, n)==self._generator, "thirds must sum up to generator"
-        return BalzanoDiagram(n, Chroma(minor, n), Chroma(major, n))
-
-    def show_gCycle(self):
-        self.cycle.show()
-    
-    def show(self):
-        GCycle(Chroma(1, self.cardinality)).show()
-
-    def __str__(self):
-        return f'{self.cardinality}-Fold Tonal System with generator {self._generator}'
+from .gcycle import GCycle
+from .chroma import Chroma
+from .scale import Scale
+from .balzano_diagram import BalzanoDiagram
+from typing import Union
+import math
+
+class TonalSystem:
+    """
+    Instantiate a Tonal System.
+    A Tonal System is a group of n elements and it has a generator chosen as a generalized fifth. 
+    All the other structures are defined within a Tonal System.
+    
+    :param n: The number of elements.
+    :type n: int
+
+    :param g: The generalized fifth of the System.
+    :type g: int
+    """
+
+    def __init__(self, n: int, g=1):
+        assert n>1, "Tonal System must have more than one element"
+        self.cardinality = n
+        self._generator = Chroma(g, n)
+        self.cycle = GCycle(self._generator)
+        self.diatonic = self.diatonic_scale()
+
+    @property
+    def generators(self):
+        n = self.cardinality
+        return [x for x in range(n) if math.gcd(x, n)==1]
+
+    @property
+    def generator(self):
+        return self._generator.pitch_class
+    
+    @generator.setter
+    def generator(self, value):
+        self.set_generator(value)
+
+    def set_generator(self, g: Union[Chroma, int]):
+        if isinstance(g, int):
+            assert math.gcd(g, self.cardinality)==1, "Element must be a generator"
+            self._generator = Chroma(g, self.cardinality)
+        elif isinstance(g, Chroma):
+            assert g.is_generator, "Element must be a generator"
+            self._generator = g
+        self.cycle = GCycle(self._generator)
+        self.diatonic = self.diatonic_scale()
+
+    def scale(self, elements=[], struct=[], name='Generic Scale'):
+        assert (len(elements)==0) ^ (len(struct)==0), "argument must be either elements or struct"
+        if len(elements)!=0:
+            elements.sort()
+            if all(isinstance(e, Chroma) for e in elements):
+                circle_elements = elements + [elements[0]]
+            elif all(isinstance(e, int) for e in elements):
+                circle_elements = [Chroma(e, self.cardinality) for e in elements] + [Chroma(elements[0], self.cardinality)]
+
+            struct = tuple((circle_elements[i]-circle_elements[i-1]).pitch_class for i in range(1, len(circle_elements)))
+
+        return Scale(self.cardinality, struct, name=name)
+
+    def diatonic_scale(self):
+        return self.cycle.diatonic_scale(0)
+    
+    def chromatic_scale(self):
+        struct = tuple([1 for _ in range(self.cardinality)])
+        return Scale(self.cardinality, struct, name=f'{self.cardinality}EDO Chromatic Scale')
+
+    # TODO: Figure out another way to do this
+    def midi_pitch(self, pitch_class: int, oct=0):
+        oct+=2
+        if oct==2:
+            oct += int(pitch_class//self.cardinality) - 2
+        return Chroma(pitch_class, self.cardinality).midi + (12*oct)
+
+    def balzano_diagram(self, minor: int, major: int):
+        n = self.cardinality
+        assert Chroma(minor+major, n)==self._generator, "thirds must sum up to generator"
+        return BalzanoDiagram(n, Chroma(minor, n), Chroma(major, n))
+    
+    #---------------------COMPOSITION METHODS------------------------
+
+    def show_gCycle(self):
+        self.cycle.show()
+    
+    def show(self):
+        GCycle(Chroma(1, self.cardinality)).show()
+
+    def __str__(self):
+        return f'{self.cardinality}-Fold Tonal System with generator {self._generator}'
```

### Comparing `edopi-1.0.0/edopi.egg-info/PKG-INFO` & `edopi-1.1.0/edopi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1
-Name: edopi
-Version: 1.0.0
-Summary: Python package to deal with Group-Theoretic microtonal music structures
-Home-page: https://github.com/luansimoes/edopi
-Author: Flavia Elias e Luan Simões
-Author-email: luansimoes@id.uff.br
-License: MIT License
-Description: # EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
-        
-        ### Installation
-        ```
-        pip install edopi
-        ```
-        
-        ### Get started
-        How to generate the main structures and visualizations:
-        
-        ```Python
-        from edopi import TonalSystem
-        
-        # Instantiate a 12-EDO with generator 7
-        edo_12 = TonalSystem(12, 7)
-        
-        # Show the Chromatic representation
-        edo_12.show()
-        
-        # Show the cycle of Fifths
-        edo_12.show_gCycle()
-        
-        # Get the diatonic scale and show it
-        diatonic = edo_12.diatonic_scale()
-        diatonic.show()
-        
-        # Get Balzano Diagram and show it
-        b_diagram = edo_12.balzano_diagram(3, 4)
-        b_diagram.show()
-        ```
-        
-Keywords: microtonal edo music group-theoretic
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: edopi
+Version: 1.1.0
+Summary: Python package to deal with Group-Theoretic microtonal music structures
+Home-page: https://github.com/luansimoes/edopi
+Author: Flavia Elias e Luan Simões
+Author-email: luansimoes@cos.ufrj.br
+License: MIT License
+Keywords: microtonal edo music group-theoretic
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# EDO&pi;: A Python Library for Group-Theoretic Microtonal Music Structures
+
+### Installation
+```
+pip install edopi
+```
+
+### Get started
+How to generate the main structures and visualizations:
+
+```Python
+from edopi import TonalSystem
+
+# Instantiate a 12-EDO with generator 7
+edo_12 = TonalSystem(12, 7)
+
+# Show the Chromatic representation
+edo_12.show()
+
+# Show the cycle of Fifths
+edo_12.show_gCycle()
+
+# Get the diatonic scale and show it
+diatonic = edo_12.diatonic_scale()
+diatonic.show()
+
+# Get Balzano Diagram and show it
+b_diagram = edo_12.balzano_diagram(3, 4)
+b_diagram.show()
+```
```

### Comparing `edopi-1.0.0/setup.py` & `edopi-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(name='edopi',
-    version='1.0.0',
+    version='1.1.0',
     url='https://github.com/luansimoes/edopi',
     license='MIT License',
     author='Flavia Elias e Luan Simões',
     long_description=readme,
     long_description_content_type="text/markdown",
-    author_email='luansimoes@id.uff.br',
+    author_email='luansimoes@cos.ufrj.br',
     keywords='microtonal edo music group-theoretic',
     description='Python package to deal with Group-Theoretic microtonal music structures',
     packages=find_packages(include=['edopi', 'edopi.*']),
     install_requires=['numpy','matplotlib'],)
```

