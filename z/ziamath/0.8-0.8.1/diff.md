# Comparing `tmp/ziamath-0.8.tar.gz` & `tmp/ziamath-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziamath-0.8.tar", last modified: Sun May 28 15:10:12 2023, max compression
+gzip compressed data, was "ziamath-0.8.1.tar", last modified: Sun May 28 20:57:35 2023, max compression
```

## Comparing `ziamath-0.8.tar` & `ziamath-0.8.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.955836 ziamath-0.8/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2023-04-22 17:44:45.000000 ziamath-0.8/LICENSE.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1728 2023-05-28 15:10:12.955836 ziamath-0.8/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      573 2023-05-17 03:54:18.000000 ziamath-0.8/README.md
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-04-22 17:44:41.000000 ziamath-0.8/pyproject.toml
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1298 2023-05-28 15:10:12.956836 ziamath-0.8/setup.cfg
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.949836 ziamath-0.8/ziamath/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      430 2023-05-28 15:09:47.000000 ziamath-0.8/ziamath/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2096 2023-05-22 01:13:13.000000 ziamath-0.8/ziamath/__main__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1829 2023-05-21 16:05:41.000000 ziamath-0.8/ziamath/config.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10494 2023-05-20 17:39:12.000000 ziamath-0.8/ziamath/drawable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    40482 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/escape_codes.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      998 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/escapes.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.952836 ziamath-0.8/ziamath/fonts/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1517704 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/fonts/STIXTwoMath-Regular.ttf
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/fonts/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      793 2023-05-16 02:20:45.000000 ziamath-0.8/ziamath/mathfont.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26767 2023-05-20 22:51:50.000000 ziamath-0.8/ziamath/mathtable.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.955836 ziamath-0.8/ziamath/nodes/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      453 2023-05-21 22:28:30.000000 ziamath-0.8/ziamath/nodes/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4453 2023-05-19 01:50:35.000000 ziamath-0.8/ziamath/nodes/menclose.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5347 2023-05-28 01:58:50.000000 ziamath-0.8/ziamath/nodes/mfenced.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4252 2023-05-20 22:02:32.000000 ziamath-0.8/ziamath/nodes/mfrac.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7591 2023-05-28 02:13:47.000000 ziamath-0.8/ziamath/nodes/mnode.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3343 2023-05-27 03:44:25.000000 ziamath-0.8/ziamath/nodes/mnumber.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3634 2023-05-28 01:59:40.000000 ziamath-0.8/ziamath/nodes/moperator.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4330 2023-05-20 03:46:23.000000 ziamath-0.8/ziamath/nodes/mroot.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6311 2023-05-21 17:26:37.000000 ziamath-0.8/ziamath/nodes/mrow.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2440 2023-05-20 21:57:21.000000 ziamath-0.8/ziamath/nodes/mspace.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11336 2023-05-27 03:42:46.000000 ziamath-0.8/ziamath/nodes/msubsup.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3579 2023-05-20 21:59:03.000000 ziamath-0.8/ziamath/nodes/mtable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10389 2023-05-20 18:34:20.000000 ziamath-0.8/ziamath/nodes/munderover.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1993 2023-05-18 01:26:19.000000 ziamath-0.8/ziamath/nodes/nodetools.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    36431 2023-05-28 02:10:18.000000 ziamath-0.8/ziamath/operators.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    80668 2023-05-20 22:40:49.000000 ziamath-0.8/ziamath/operators_mml4.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/py.typed
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9828 2023-05-27 01:18:44.000000 ziamath-0.8/ziamath/styles.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    22219 2023-05-27 01:09:49.000000 ziamath-0.8/ziamath/zmath.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.950836 ziamath-0.8/ziamath.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1728 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      903 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-19 21:05:39.000000 ziamath-0.8/ziamath.egg-info/not-zip-safe
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       28 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/requires.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/top_level.txt
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.737459 ziamath-0.8.1/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2023-04-22 17:44:45.000000 ziamath-0.8.1/LICENSE.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1730 2023-05-28 20:57:35.737459 ziamath-0.8.1/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      573 2023-05-17 03:54:18.000000 ziamath-0.8.1/README.md
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-04-22 17:44:41.000000 ziamath-0.8.1/pyproject.toml
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1298 2023-05-28 20:57:35.739460 ziamath-0.8.1/setup.cfg
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.709445 ziamath-0.8.1/ziamath/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      432 2023-05-28 20:56:36.000000 ziamath-0.8.1/ziamath/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2096 2023-05-22 01:13:13.000000 ziamath-0.8.1/ziamath/__main__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1899 2023-05-28 20:46:33.000000 ziamath-0.8.1/ziamath/config.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10494 2023-05-20 17:39:12.000000 ziamath-0.8.1/ziamath/drawable.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    40482 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/escape_codes.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      998 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/escapes.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.716448 ziamath-0.8.1/ziamath/fonts/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1517704 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/fonts/STIXTwoMath-Regular.ttf
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/fonts/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      793 2023-05-16 02:20:45.000000 ziamath-0.8.1/ziamath/mathfont.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26767 2023-05-20 22:51:50.000000 ziamath-0.8.1/ziamath/mathtable.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.737459 ziamath-0.8.1/ziamath/nodes/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      453 2023-05-21 22:28:30.000000 ziamath-0.8.1/ziamath/nodes/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4453 2023-05-19 01:50:35.000000 ziamath-0.8.1/ziamath/nodes/menclose.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5347 2023-05-28 01:58:50.000000 ziamath-0.8.1/ziamath/nodes/mfenced.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4252 2023-05-20 22:02:32.000000 ziamath-0.8.1/ziamath/nodes/mfrac.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7591 2023-05-28 02:13:47.000000 ziamath-0.8.1/ziamath/nodes/mnode.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3343 2023-05-27 03:44:25.000000 ziamath-0.8.1/ziamath/nodes/mnumber.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3634 2023-05-28 01:59:40.000000 ziamath-0.8.1/ziamath/nodes/moperator.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4330 2023-05-20 03:46:23.000000 ziamath-0.8.1/ziamath/nodes/mroot.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6311 2023-05-21 17:26:37.000000 ziamath-0.8.1/ziamath/nodes/mrow.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2440 2023-05-20 21:57:21.000000 ziamath-0.8.1/ziamath/nodes/mspace.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11336 2023-05-27 03:42:46.000000 ziamath-0.8.1/ziamath/nodes/msubsup.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3579 2023-05-20 21:59:03.000000 ziamath-0.8.1/ziamath/nodes/mtable.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10389 2023-05-20 18:34:20.000000 ziamath-0.8.1/ziamath/nodes/munderover.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1993 2023-05-18 01:26:19.000000 ziamath-0.8.1/ziamath/nodes/nodetools.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    36431 2023-05-28 02:10:18.000000 ziamath-0.8.1/ziamath/operators.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    80668 2023-05-20 22:40:49.000000 ziamath-0.8.1/ziamath/operators_mml4.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8.1/ziamath/py.typed
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9856 2023-05-28 20:47:36.000000 ziamath-0.8.1/ziamath/styles.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    22219 2023-05-27 01:09:49.000000 ziamath-0.8.1/ziamath/zmath.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 20:57:35.714447 ziamath-0.8.1/ziamath.egg-info/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1730 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      903 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/SOURCES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/dependency_links.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-19 21:05:39.000000 ziamath-0.8.1/ziamath.egg-info/not-zip-safe
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       28 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/requires.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2023-05-28 20:57:35.000000 ziamath-0.8.1/ziamath.egg-info/top_level.txt
```

### Comparing `ziamath-0.8/LICENSE.txt` & `ziamath-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/PKG-INFO` & `ziamath-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.8
+Version: 0.8.1
 Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
 Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziamath.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziamath
```

### Comparing `ziamath-0.8/README.md` & `ziamath-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/setup.cfg` & `ziamath-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/__main__.py` & `ziamath-0.8.1/ziamath/__main__.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/config.py` & `ziamath-0.8.1/ziamath/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ''' Global configuration options '''
 from typing import Optional
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from ziafont import config as zfconfig
 
 
 @dataclass
 class DebugConfig:
     baseline: bool = False
@@ -48,19 +48,19 @@
         debug: Debug mode, draws bounding boxes around <mrows>
         svg2: Use SVG2.0. Disable for better browser compatibility,
             at the expense of SVG size
         precision: SVG decimal precision for coordinates
         decimal_separator: Use `.` or `,` as decimal separator. (only
             affects Latex math)
     '''
-    math: MathStyle = MathStyle()
-    text: TextStyle = TextStyle()
+    math: MathStyle = field(default_factory=MathStyle)
+    text: TextStyle = field(default_factory=TextStyle)
     minsizefraction: float = .3
     decimal_separator = '.'
-    debug: DebugConfig = DebugConfig()
+    debug: DebugConfig = field(default_factory=DebugConfig)
 
     @property
     def svg2(self) -> bool:
         return zfconfig.svg2
 
     @svg2.setter
     def svg2(self, value: bool) -> None:
```

### Comparing `ziamath-0.8/ziamath/drawable.py` & `ziamath-0.8.1/ziamath/drawable.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/escape_codes.py` & `ziamath-0.8.1/ziamath/escape_codes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/escapes.py` & `ziamath-0.8.1/ziamath/escapes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/fonts/STIXTwoMath-Regular.ttf` & `ziamath-0.8.1/ziamath/fonts/STIXTwoMath-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/mathfont.py` & `ziamath-0.8.1/ziamath/mathfont.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/mathtable.py` & `ziamath-0.8.1/ziamath/mathtable.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/menclose.py` & `ziamath-0.8.1/ziamath/nodes/menclose.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mfenced.py` & `ziamath-0.8.1/ziamath/nodes/mfenced.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mfrac.py` & `ziamath-0.8.1/ziamath/nodes/mfrac.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mnode.py` & `ziamath-0.8.1/ziamath/nodes/mnode.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mnumber.py` & `ziamath-0.8.1/ziamath/nodes/mnumber.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/moperator.py` & `ziamath-0.8.1/ziamath/nodes/moperator.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mroot.py` & `ziamath-0.8.1/ziamath/nodes/mroot.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mrow.py` & `ziamath-0.8.1/ziamath/nodes/mrow.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mspace.py` & `ziamath-0.8.1/ziamath/nodes/mspace.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/msubsup.py` & `ziamath-0.8.1/ziamath/nodes/msubsup.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/mtable.py` & `ziamath-0.8.1/ziamath/nodes/mtable.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/munderover.py` & `ziamath-0.8.1/ziamath/nodes/munderover.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/nodes/nodetools.py` & `ziamath-0.8.1/ziamath/nodes/nodetools.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/operators.py` & `ziamath-0.8.1/ziamath/operators.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/operators_mml4.py` & `ziamath-0.8.1/ziamath/operators_mml4.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath/styles.py` & `ziamath-0.8.1/ziamath/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ''' Apply italic, bold, and other font styles by shifting the unstyled ASCII
     characters [A-Z, a-z, and 0-9] to their higher unicode alternatives. Note
     this does not check whether the new character glyph exists in the font.
 '''
 from __future__ import annotations
 from typing import Any, MutableMapping
 from collections import ChainMap, namedtuple
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass, field, asdict
 from xml.etree import ElementTree as ET
 
 from .config import config
 
 
 VARIANTS = ['serif', 'sans', 'script', 'double', 'mono', 'fraktur']
 Styletype = namedtuple('Styletype', 'bold italic')
@@ -23,15 +23,15 @@
     bold: bool = False
     normal: bool = False
 
 
 @dataclass
 class MathStyle:
     ''' Math Style parameters '''
-    mathvariant: MathVariant = MathVariant()
+    mathvariant: MathVariant = field(default_factory=MathVariant)
     displaystyle: bool = True
     mathcolor: str = 'black'
     mathbackground: str = 'none'
     mathsize: str = ''
     scriptlevel: int = 0
```

### Comparing `ziamath-0.8/ziamath/zmath.py` & `ziamath-0.8.1/ziamath/zmath.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.8/ziamath.egg-info/PKG-INFO` & `ziamath-0.8.1/ziamath.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.8
+Version: 0.8.1
 Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
 Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
 Author-email: code@collindelker.com
 License: MIT
 Project-URL: Documentation, https://ziamath.readthedocs.io
 Project-URL: Source Code, https://github.com/cdelker/ziamath
```

### Comparing `ziamath-0.8/ziamath.egg-info/SOURCES.txt` & `ziamath-0.8.1/ziamath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

