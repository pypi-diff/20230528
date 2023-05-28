# Comparing `tmp/digital_unit-1.5b0.tar.gz` & `tmp/digital_unit-1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.5b0.tar", last modified: Thu May 25 14:15:13 2023, max compression
+gzip compressed data, was "digital_unit-1.6b0.tar", last modified: Sun May 28 08:18:06 2023, max compression
```

## Comparing `digital_unit-1.5b0.tar` & `digital_unit-1.6b0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.849369 digital_unit-1.5b0/
--rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.848379 digital_unit-1.5b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.831365 digital_unit-1.5b0/digital_unit/
--rw-rw-rw-   0        0        0      827 2023-05-24 12:55:31.000000 digital_unit-1.5b0/digital_unit/Area.py
--rw-rw-rw-   0        0        0      797 2023-05-24 12:55:26.000000 digital_unit-1.5b0/digital_unit/Lenth.py
--rw-rw-rw-   0        0        0      169 2023-05-25 14:12:42.000000 digital_unit-1.5b0/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-05-24 14:05:13.000000 digital_unit-1.5b0/digital_unit/root.py
--rw-rw-rw-   0        0        0      330 2023-05-25 13:54:40.000000 digital_unit-1.5b0/digital_unit/sample.py
--rw-rw-rw-   0        0        0      294 2023-05-25 14:15:08.000000 digital_unit-1.5b0/digital_unit/volume.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.845265 digital_unit-1.5b0/digital_unit.egg-info/
--rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:15:13.850380 digital_unit-1.5b0/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-05-25 14:08:23.000000 digital_unit-1.5b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.072172 digital_unit-1.6b0/
+-rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:06.072172 digital_unit-1.6b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1383 2023-05-28 08:12:19.000000 digital_unit-1.6b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.054184 digital_unit-1.6b0/digital_unit/
+-rw-rw-rw-   0        0        0     1166 2023-05-28 08:07:32.000000 digital_unit-1.6b0/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      925 2023-05-28 08:08:29.000000 digital_unit-1.6b0/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      570 2023-05-28 08:17:58.000000 digital_unit-1.6b0/digital_unit/Temperature.py
+-rw-rw-rw-   0        0        0     1159 2023-05-28 08:06:54.000000 digital_unit-1.6b0/digital_unit/Volume.py
+-rw-rw-rw-   0        0        0      209 2023-05-28 07:44:32.000000 digital_unit-1.6b0/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-05-28 08:05:25.000000 digital_unit-1.6b0/digital_unit/root.py
+-rw-rw-rw-   0        0        0      330 2023-05-28 08:11:42.000000 digital_unit-1.6b0/digital_unit/sample.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.068171 digital_unit-1.6b0/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-28 08:18:06.074171 digital_unit-1.6b0/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-28 08:09:55.000000 digital_unit-1.6b0/setup.py
```

### Comparing `digital_unit-1.5b0/digital_unit/Area.py` & `digital_unit-1.6b0/digital_unit/Lenth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from .root import DigitalUnit
-class Area(DigitalUnit):
+
+class Lenth(DigitalUnit):
     def __init__(self) -> None:
-        self.type = 'Area'
+        self.type = 'Lenth'
 
-class SquareMeter(Area):
+class Metre(Lenth):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 1.0 
+        self.measure = 1.0
+        self.measure_add = 0.0
     def __str__(self) -> str:
-        return 'm²'
+        return 'm'
 
-class SquareKiloMeter(Area):
+class KiloMetre(Lenth):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 1000_000.0
+        self.measure = 1000.0
+        self.measure_add = 0.0
     def __str__(self) -> str:
-        return 'km²'
+        return 'km'
 
-class Hectare(Area):
+class CentiMeter(Lenth):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 10_000.0
+        self.measure = 0.01
+        self.measure_add = 0.0
     def __str__(self) -> str:
-        return 'hm²'
+        return 'cm'
 
-class SquareCentiMeter(Area):
+class MilliMeter(Lenth):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 1.0
+        self.measure = 0.001
+        self.measure_add = 0.0
     def __str__(self) -> str:
-        return 'cm²'
-
-
-    
+        return 'mm'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `digital_unit-1.5b0/digital_unit/Lenth.py` & `digital_unit-1.6b0/digital_unit/Temperature.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 from .root import DigitalUnit
-
-class Lenth(DigitalUnit):
-    def __init__(self) -> None:
-        self.type = 'Lenth'
-
-class Metre(Lenth):
-    def __init__(self) -> None:
-        super().__init__()
-        self.measure = 1.0
-    def __str__(self) -> str:
-        return 'm'
-
-class KiloMetre(Lenth):
+class Temperature(DigitalUnit):
     def __init__(self) -> None:
-        super().__init__()
-        self.measure = 1000.0
-    def __str__(self) -> str:
-        return 'km'
+        self.type = 'Temperature'
 
-class CentiMeter(Lenth):
+class CelsiusDegree(Temperature):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 0.01
+        self.measure = 1.8 
+        self.measure_add = 0.0
     def __str__(self) -> str:
-        return 'cm'
-
-class MilliMeter(Lenth):
+        return '℃'
+    
+class FahrenheitTegree(Temperature):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 0.001
+        self.measure = 1.0 
+        self.measure_add = 32.0
     def __str__(self) -> str:
-        return 'mm'
+        return '℉'
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `digital_unit-1.5b0/digital_unit/root.py` & `digital_unit-1.6b0/digital_unit/root.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 class DigitalUnit:
     def __init__(self) -> None:
         self.type = "NONE"
 
 
 class Number:
-    def __init__(self, number : float, unit:DigitalUnit) -> None:
+    def __init__(self, number:float, unit:DigitalUnit) -> None:
         self.digital_part = number
         if unit.__class__.__base__.__base__ == DigitalUnit:
             self.unit = unit
         else:
             print(unit.__class__.__base__.__base__)
             raise TypeError('You should set the unit parameter to numerical units.')
 
-    def change_unit(self, new_unit):
+    def change_unit(self, new_unit:DigitalUnit) -> None:
         if new_unit.__class__.__base__.__base__ == DigitalUnit:
             if new_unit.type == self.unit.type:
-                self.digital_part = self.digital_part * self.unit.measure / new_unit.measure
+                self.digital_part = self.digital_part * self.unit.measure / new_unit.measure + (new_unit.measure_add-self.unit.measure_add)
                 self.unit = new_unit
             else:
                 raise TypeError('Different unit types')
         else:
             raise TypeError('You should set the unit parameter to numerical units.')
     
     def __str__(self) -> str:
```

### Comparing `digital_unit-1.5b0/setup.py` & `digital_unit-1.6b0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from distutils.core import setup
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.5b0',      # Start with a small number and increase it with every change you make
+  version = '1.6b0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
+  long_description = long_description,
+  long_description_content_type="text/markdown",
 
   classifiers=[ 
     'Programming Language :: Python :: 3.6',
+
   ],
 )
```

