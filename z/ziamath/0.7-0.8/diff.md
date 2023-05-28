# Comparing `tmp/ziamath-0.7.tar.gz` & `tmp/ziamath-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziamath-0.7.tar", last modified: Sun Nov  6 00:38:44 2022, max compression
+gzip compressed data, was "ziamath-0.8.tar", last modified: Sun May 28 15:10:12 2023, max compression
```

## Comparing `ziamath-0.7.tar` & `ziamath-0.8.tar`

### file list

```diff
@@ -1,30 +1,45 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:38:44.755606 ziamath-0.7/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2022-10-08 18:59:59.000000 ziamath-0.7/LICENSE.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1487 2022-11-06 00:38:44.755606 ziamath-0.7/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      352 2022-11-05 23:24:06.000000 ziamath-0.7/README.md
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       38 2022-11-06 00:38:44.755606 ziamath-0.7/setup.cfg
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1559 2022-11-06 00:20:56.000000 ziamath-0.7/setup.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:38:44.752606 ziamath-0.7/ziamath/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      151 2022-11-05 23:32:36.000000 ziamath-0.7/ziamath/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2620 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/__main__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      995 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/config.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10017 2022-10-16 17:33:23.000000 ziamath-0.7/ziamath/drawable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    40482 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/escape_codes.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      998 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/escapes.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:38:44.755606 ziamath-0.7/ziamath/fonts/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1517704 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/fonts/STIXTwoMath-Regular.ttf
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/fonts/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      651 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/mathfont.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    22532 2022-10-30 14:26:47.000000 ziamath-0.7/ziamath/mathtable.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    51466 2022-10-27 02:21:15.000000 ziamath-0.7/ziamath/nodes.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    35582 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/operators.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2022-10-08 18:59:59.000000 ziamath-0.7/ziamath/py.typed
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2942 2022-10-16 17:48:19.000000 ziamath-0.7/ziamath/styles.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    17875 2022-10-16 17:38:33.000000 ziamath-0.7/ziamath/zmath.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:38:44.753606 ziamath-0.7/ziamath.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1487 2022-11-06 00:38:44.000000 ziamath-0.7/ziamath.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      530 2022-11-06 00:38:44.000000 ziamath-0.7/ziamath.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2022-11-06 00:38:44.000000 ziamath-0.7/ziamath.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2022-10-08 19:00:58.000000 ziamath-0.7/ziamath.egg-info/not-zip-safe
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       35 2022-11-06 00:38:44.000000 ziamath-0.7/ziamath.egg-info/requires.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2022-11-06 00:38:44.000000 ziamath-0.7/ziamath.egg-info/top_level.txt
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.955836 ziamath-0.8/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2023-04-22 17:44:45.000000 ziamath-0.8/LICENSE.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1728 2023-05-28 15:10:12.955836 ziamath-0.8/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      573 2023-05-17 03:54:18.000000 ziamath-0.8/README.md
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-04-22 17:44:41.000000 ziamath-0.8/pyproject.toml
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1298 2023-05-28 15:10:12.956836 ziamath-0.8/setup.cfg
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.949836 ziamath-0.8/ziamath/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      430 2023-05-28 15:09:47.000000 ziamath-0.8/ziamath/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2096 2023-05-22 01:13:13.000000 ziamath-0.8/ziamath/__main__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1829 2023-05-21 16:05:41.000000 ziamath-0.8/ziamath/config.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10494 2023-05-20 17:39:12.000000 ziamath-0.8/ziamath/drawable.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    40482 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/escape_codes.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      998 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/escapes.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.952836 ziamath-0.8/ziamath/fonts/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1517704 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/fonts/STIXTwoMath-Regular.ttf
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/fonts/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      793 2023-05-16 02:20:45.000000 ziamath-0.8/ziamath/mathfont.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26767 2023-05-20 22:51:50.000000 ziamath-0.8/ziamath/mathtable.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.955836 ziamath-0.8/ziamath/nodes/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      453 2023-05-21 22:28:30.000000 ziamath-0.8/ziamath/nodes/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4453 2023-05-19 01:50:35.000000 ziamath-0.8/ziamath/nodes/menclose.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5347 2023-05-28 01:58:50.000000 ziamath-0.8/ziamath/nodes/mfenced.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4252 2023-05-20 22:02:32.000000 ziamath-0.8/ziamath/nodes/mfrac.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7591 2023-05-28 02:13:47.000000 ziamath-0.8/ziamath/nodes/mnode.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3343 2023-05-27 03:44:25.000000 ziamath-0.8/ziamath/nodes/mnumber.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3634 2023-05-28 01:59:40.000000 ziamath-0.8/ziamath/nodes/moperator.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4330 2023-05-20 03:46:23.000000 ziamath-0.8/ziamath/nodes/mroot.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6311 2023-05-21 17:26:37.000000 ziamath-0.8/ziamath/nodes/mrow.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2440 2023-05-20 21:57:21.000000 ziamath-0.8/ziamath/nodes/mspace.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11336 2023-05-27 03:42:46.000000 ziamath-0.8/ziamath/nodes/msubsup.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3579 2023-05-20 21:59:03.000000 ziamath-0.8/ziamath/nodes/mtable.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10389 2023-05-20 18:34:20.000000 ziamath-0.8/ziamath/nodes/munderover.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1993 2023-05-18 01:26:19.000000 ziamath-0.8/ziamath/nodes/nodetools.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    36431 2023-05-28 02:10:18.000000 ziamath-0.8/ziamath/operators.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    80668 2023-05-20 22:40:49.000000 ziamath-0.8/ziamath/operators_mml4.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:19:13.000000 ziamath-0.8/ziamath/py.typed
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9828 2023-05-27 01:18:44.000000 ziamath-0.8/ziamath/styles.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    22219 2023-05-27 01:09:49.000000 ziamath-0.8/ziamath/zmath.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-28 15:10:12.950836 ziamath-0.8/ziamath.egg-info/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1728 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      903 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/SOURCES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/dependency_links.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-19 21:05:39.000000 ziamath-0.8/ziamath.egg-info/not-zip-safe
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       28 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/requires.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2023-05-28 15:10:12.000000 ziamath-0.8/ziamath.egg-info/top_level.txt
```

### Comparing `ziamath-0.7/LICENSE.txt` & `ziamath-0.8/LICENSE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2022 Collin J. Delker
+Copyright (c) 2021-2023 Collin J. Delker
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ziamath-0.7/PKG-INFO` & `ziamath-0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.7
-Summary: Render MathML and LaTeX Math to SVG without Latex installation
-Home-page: https://ziamath.readthedocs.io/
+Version: 0.8
+Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
+Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
-Author-email: ziaplot@collindelker.com
-Project-URL: Source, https://bitbucket.org/cdelker/ziamath
+Author-email: code@collindelker.com
+License: MIT
+Project-URL: Documentation, https://ziamath.readthedocs.io
+Project-URL: Source Code, https://github.com/cdelker/ziamath
 Keywords: MathML,LaTeX,math,font,truetype,opentype,svg
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: latex
 License-File: LICENSE.txt
 
 # ziamath
 
-Render MathML or LaTeX Math expressions as SVG. Does not require a Latex installation.
+Render MathML or LaTeX Math expressions as SVG using pure Python. Does not require a Latex installation, nor a network connection.
 
 Ziamath comes with the STIXTwoMath-Regular font installed for use by default.
 Other Math-enabled Open Type fonts (TTF or OTF files) may also be used.
 
-![Example](example.png)
+![Example](https://github.com/cdelker/ziamath/blob/05e25b1789acc8ee816971d384aa851ffb197f7a/example.png)
 
+Documentation is available at [readthedocs](https://ziamath.readthedocs.io).
 
-Documentation is available at [readthedocs](https://ziamath.readthedocs.io)
+Also try the [online demo](https://cdelker.github.io/pyscript/ziamath.html) based on Pyscript.
```

### Comparing `ziamath-0.7/ziamath/drawable.py` & `ziamath-0.8/ziamath/drawable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 from __future__ import annotations
-from typing import Optional, Union, MutableMapping
-
+from typing import Optional
 import math
 import xml.etree.ElementTree as ET
 
-from .config import config
-from ziafont import Font
 from ziafont.fonttypes import BBox
 from ziafont.glyph import SimpleGlyph, fmt
+from .config import config
+from .styles import MathStyle
+
 
 class Drawable:
     ''' Base class for drawable nodes '''
+    mtag = 'drawable'
+    nodes: list[Drawable] = []
+
+    def __init__(self):
+        self.bbox = BBox(0, 0, 0, 0)
 
     def firstglyph(self) -> Optional[SimpleGlyph]:
         ''' Get the first glyph in this node '''
         return None
-        
+
     def lastglyph(self) -> Optional[SimpleGlyph]:
         ''' Get the last glyph in this node '''
         return None
 
     def lastchar(self) -> Optional[str]:
         ''' Get the last character in this node '''
         return None
 
+    def xadvance(self) -> float:
+        ''' X-advance for the glyph. Usually bbox.xmax '''
+        return self.bbox.xmax
+
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
+        ''' Draw the element. Must be subclassed. '''
         raise NotImplementedError
 
-        
+
 class Glyph(Drawable):
-    ''' A single glyph '''
-    def __init__(self, glyph: SimpleGlyph, char: str, size: float, emscale: float,
-                 style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+    ''' A single glyph
+
+        Args:
+            glyph: The glyph to draw
+            char: unicode character represented by the glyph
+            size: point size
+            style: font MathStyle
+    '''
+    def __init__(self, glyph: SimpleGlyph, char: str, size: float,
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.glyph = glyph
         self.char = char
         self.size = size
-        self.emscale = emscale
         self.phantom = kwargs.get('phantom', False)
-        self.style = style if style is not None else {}
-        self._setup()
-
-    def _setup(self, **kwargs) -> None:
-        ''' Place the glyphs with 0, 0 positions '''
+        self.style = style if style else MathStyle()
+        self._funits_to_pts = self.size / self.glyph.font.info.layout.unitsperem
         self.bbox = BBox(
-            self.glyph.path.bbox.xmin * self.emscale,
-            self.glyph.path.bbox.xmax * self.emscale,
-            self.glyph.path.bbox.ymin * self.emscale,
-            self.glyph.path.bbox.ymax * self.emscale)
+            self.funit_to_points(self.glyph.path.bbox.xmin),
+            self.funit_to_points(self.glyph.path.bbox.xmax),
+            self.funit_to_points(self.glyph.path.bbox.ymin),
+            self.funit_to_points(self.glyph.path.bbox.ymax))
+        
+    def funit_to_points(self, value: float) -> float:
+        ''' Convert font units to SVG points '''
+        return value * self._funits_to_pts
 
     def firstglyph(self) -> Optional[SimpleGlyph]:
         ''' Get the first glyph in this node '''
         return self.glyph
 
     def lastglyph(self) -> Optional[SimpleGlyph]:
         ''' Get the last glyph in this node '''
         return self.glyph
 
     def lastchar(self) -> Optional[str]:
         ''' Get the last character in this node '''
         return self.char
 
+    def xadvance(self) -> float:
+        ''' X-advance for the glyph. Usually bbox.xmax '''
+        return self.funit_to_points(self.glyph.advance())
+
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
                 y: Vertical position in SVG coordinates
                 svg: SVG drawing as XML
@@ -72,28 +94,30 @@
         symids = [sym.attrib.get('id') for sym in symbols]
         if self.glyph.id not in symids and config.svg2:
             svg.append(self.glyph.svgsymbol())
         if not self.phantom:
             path = self.glyph.place(x, y, self.size)
             if path is not None:
                 svg.append(path)
-            if 'mathcolor' in self.style:
-                svg[-1].set('fill', self.style['mathcolor'])  # type: ignore
-        x += self.glyph.advance() * self.emscale
+            if self.style.mathcolor and len(svg) > 0:
+                svg[-1].set('fill', str(self.style.mathcolor))
+        x += self.funit_to_points(self.glyph.advance())
         return x, y
 
 
 class HLine(Drawable):
     ''' Horizontal Line. '''
-    def __init__(self, length: float, lw: float, style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+    def __init__(self, length: float, lw: float,
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.length = length
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
-        self.bbox = BBox(0, lw/2, self.length, self.lw)
-        self.style = style if style is not None else {}
+        self.bbox = BBox(0, self.length, -self.lw/2, self.lw/2)
+        self.style = style if style else MathStyle()
 
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
                 y: Vertical position in SVG coordinates
@@ -103,27 +127,29 @@
             # Use rectangle so it can change color with 'fill' attribute
             # and not mess up glyphs with 'stroke' attribute
             bar = ET.SubElement(svg, 'rect')
             bar.attrib['x'] = fmt(x)
             bar.attrib['y'] = fmt(y)
             bar.attrib['width'] = fmt(self.length)
             bar.attrib['height'] = fmt(self.lw)
-            if 'mathcolor' in self.style:
-                bar.attrib['fill'] = self.style['mathcolor']  # type: ignore
+            if self.style.mathcolor:
+                bar.attrib['fill'] = str(self.style.mathcolor)
         return x+self.length, y
 
-    
+
 class VLine(Drawable):
     ''' Vertical Line. '''
-    def __init__(self, height: float, lw: float, style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+    def __init__(self, height: float, lw: float,
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.height = height
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.lw, 0, self.height)
-        self.style = style if style is not None else {}
+        self.style = style if style else MathStyle()
 
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
                 y: Vertical position in SVG coordinates
@@ -133,31 +159,32 @@
             # Use rectangle so it can change color with 'fill' attribute
             # and not mess up glyphs with 'stroke' attribute
             bar = ET.SubElement(svg, 'rect')
             bar.attrib['x'] = fmt(x-self.lw/2)
             bar.attrib['y'] = fmt(y)
             bar.attrib['width'] = fmt(self.lw)
             bar.attrib['height'] = fmt(self.height)
-            if 'mathcolor' in self.style:
-                bar.attrib['fill'] = self.style['mathcolor']  # type: ignore
+            if self.style.mathcolor:
+                bar.attrib['fill'] = str(self.style.mathcolor)
         return x, y
-    
-    
+
+
 class Box(Drawable):
     ''' Box '''
     def __init__(self, width: float, height: float, lw: float,
-                 cornerradius: float=None,
-                 style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+                 cornerradius: float = None,
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.width = width
         self.height = height
         self.cornerradius = cornerradius
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
-        self.style = style if style is not None else {}
+        self.style = style if style else MathStyle()
 
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
                 y: Vertical position in SVG coordinates
@@ -166,35 +193,36 @@
         if not self.phantom:
             bar = ET.SubElement(svg, 'rect')
             bar.set('x', fmt(x))
             bar.set('y', fmt(y-self.height))
             bar.set('width', fmt(self.width))
             bar.set('height', fmt(self.height))
             bar.set('stroke-width', fmt(self.lw))
-            bar.set('stroke', self.style.get('mathcolor', 'black'))  # type: ignore
-            bar.set('fill', self.style.get('mathbackground', 'none'))  # type: ignore
+            bar.set('stroke', self.style.mathcolor)
+            bar.set('fill', self.style.mathbackground)
             if self.cornerradius:
                 bar.set('rx', fmt(self.cornerradius))
-                
+
         return x+self.width, y
 
 
 class Diagonal(Drawable):
     ''' Diagonal Line - corners of Box '''
     def __init__(self, width: float, height: float, lw: float,
-                 arrow: bool=False,
-                 style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+                 arrow: bool = False,
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.width = width
         self.height = height
         self.lw = lw
         self.arrow = arrow
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
-        self.style = style if style is not None else {}
-        
+        self.style = style if style else MathStyle()
+
         self.arroww = self.width
         self.arrowh = self.height
         if self.arrow:
             # Bbox needs to be a bit bigger to accomodate arrowhead
             theta = math.atan2(-self.height, self.width)
             self.arroww = (10+self.lw*2) * math.cos(theta)
             self.arrowh = (10+self.lw*2) * math.sin(theta)
@@ -219,31 +247,32 @@
                 marker.set('refY', '3.5')
                 marker.set('orient', 'auto')
                 poly = ET.SubElement(marker, 'polygon')
                 poly.set('points', '0 0 10 3.5 0 7')
 
             bar.set('d', f'M {fmt(x)} {fmt(y-self.height)} L {fmt(x+self.width)} {fmt(y)}')
             bar.set('stroke-width', fmt(self.lw))
-            bar.set('stroke', self.style.get('mathcolor', 'black'))  # type: ignore
+            bar.set('stroke', self.style.mathcolor)
             if self.arrow:
                 bar.set('marker-end', 'url(#arrowhead)')
-                
+
         return x+self.width, y
 
-    
+
 class Ellipse(Drawable):
     ''' Ellipse '''
     def __init__(self, width: float, height: float, lw: float,
-                 style: MutableMapping[str, Union[str, bool]]=None, **kwargs):
+                 style: MathStyle = None, **kwargs):
+        super().__init__()
         self.width = width
         self.height = height
         self.lw = lw
         self.phantom = kwargs.get('phantom', False)
         self.bbox = BBox(0, self.width, 0, self.height)
-        self.style = style if style is not None else {}
+        self.style = style if style else MathStyle()
 
     def draw(self, x: float, y: float, svg: ET.Element) -> tuple[float, float]:
         ''' Draw the node on the SVG
 
             Args:
                 x: Horizontal position in SVG coordinates
                 y: Vertical position in SVG coordinates
@@ -252,10 +281,10 @@
         if not self.phantom:
             bar = ET.SubElement(svg, 'ellipse')
             bar.set('cx', fmt(x+self.width/2))
             bar.set('cy', fmt(y-self.height/2))
             bar.set('rx', fmt(self.width/2))
             bar.set('ry', fmt(self.height/2))
             bar.set('stroke-width', fmt(self.lw))
-            bar.set('stroke', self.style.get('mathcolor', 'black'))  # type: ignore
-            bar.set('fill', self.style.get('mathbackground', 'none'))  # type: ignore
+            bar.set('stroke', self.style.mathcolor)
+            bar.set('fill', self.style.mathbackground)
         return x+self.width, y
```

### Comparing `ziamath-0.7/ziamath/escape_codes.py` & `ziamath-0.8/ziamath/escape_codes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.7/ziamath/escapes.py` & `ziamath-0.8/ziamath/escapes.py`

 * *Files identical despite different names*

### Comparing `ziamath-0.7/ziamath/fonts/STIXTwoMath-Regular.ttf` & `ziamath-0.8/ziamath/fonts/STIXTwoMath-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ziamath-0.7/ziamath/mathtable.py` & `ziamath-0.8/ziamath/mathtable.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,27 @@
     Reference: https://docs.microsoft.com/en-us/typography/opentype/spec/math
 '''
 
 from __future__ import annotations
 from typing import Union, Sequence, Optional, TYPE_CHECKING
 from collections import namedtuple
 from dataclasses import dataclass
+import xml.etree.ElementTree as ET
 
 from ziafont.gpos import Coverage
 from ziafont.fontread import FontReader
-from ziafont import glyph
-from ziafont.fonttypes import Xform, BBox, GlyphComp
+from ziafont.glyph import SimpleGlyph, CompoundGlyph
+from ziafont.fonttypes import BBox
 
 if TYPE_CHECKING:
     from .mathfont import MathFont
 
 
-GlyphType = Union[glyph.SimpleGlyph, glyph.CompoundGlyph]    
-    
+GlyphType = Union[SimpleGlyph, CompoundGlyph]
+
 MathKernInfoRecord = namedtuple(
     'MathKernInfoRecord', ['topright', 'topleft', 'bottomright', 'bottomleft'])
 GlyphPartRecord = namedtuple(
     'GlyphPartRecord', ['glyphId', 'startConnectorLength', 'endConnectorLength',
                         'fullAdvance', 'partFlags'])
 
 
@@ -189,31 +190,35 @@
         # Italics table
         self.fontfile.seek(self.ofst + ofst + italics)
         covofst = self.fontfile.readuint16()
         cnt = self.fontfile.readuint16()
         italicscorrections = []
         for i in range(cnt):
             italicscorrections.append(read_valuerecord(self.fontfile))
-        italicscoverage = Coverage(self.ofst+ofst+italics+covofst, self.fontfile, nulltable=(italics==0))
+        italicscoverage = Coverage(self.ofst+ofst+italics+covofst,
+                                   self.fontfile, nulltable=(italics==0))
 
         # Top Accent Attachment Table
         self.fontfile.seek(self.ofst + ofst + topaccent)
         covofst = self.fontfile.readuint16()
         cnt = self.fontfile.readuint16()
         accents = []
         for i in range(cnt):
             accents.append(read_valuerecord(self.fontfile))
-        accentcoverage = Coverage(self.ofst+ofst+topaccent+covofst, self.fontfile, nulltable=(topaccent==0))
+        accentcoverage = Coverage(
+            self.ofst+ofst+topaccent+covofst, self.fontfile, nulltable=(topaccent==0))
 
         # Extended Shape Coverage
-        extshapes = Coverage(self.ofst+ofst+extendshape, self.fontfile, nulltable=(extendshape==0))
+        extshapes = Coverage(
+            self.ofst+ofst+extendshape, self.fontfile, nulltable=(extendshape==0))
 
         # Kern Info
         if kernofst:
-            kerninfo = MathKernInfoTable(self.ofst+ofst+kernofst, self.fontfile, nulltable=(kernofst==0))
+            kerninfo = MathKernInfoTable(
+                self.ofst+ofst+kernofst, self.fontfile, nulltable=(kernofst==0))
         else:
             kerninfo = None
 
         self.italicsCorrection = MathSubTable(italicscorrections, italicscoverage)
         self.topAccentAttachment = MathSubTable(accents, accentcoverage)
         self._extendedShapeCoverage = extshapes
         self.kernInfo = kerninfo
@@ -226,24 +231,28 @@
         horzcovofst = self.fontfile.readuint16()
         vertcount = self.fontfile.readuint16()
         horzcount = self.fontfile.readuint16()
 
         vertConstruction = []
         for i in range(vertcount):
             vofst = self.fontfile.readuint16()
-            vertConstruction.append(MathConstructionTable(self.ofst+ofst+vofst, self.font, vert=True))
+            vertConstruction.append(
+                MathConstructionTable(self.ofst+ofst+vofst, self.font, vert=True))
         horzConstruction = []
         for i in range(horzcount):
             hofst = self.fontfile.readuint16()
-            horzConstruction.append(MathConstructionTable(self.ofst+ofst+hofst, self.font, vert=False))
+            horzConstruction.append(
+                MathConstructionTable(self.ofst+ofst+hofst, self.font, vert=False))
 
         vertcoverage = Coverage(self.ofst + ofst + vertcovofst, self.fontfile)
         horzcoverage = Coverage(self.ofst + ofst + horzcovofst, self.fontfile)
-        self._variantsvert = MathVariants(vertcoverage, vertConstruction, minoverlap, self.font, vert=True)
-        self._variantshorz = MathVariants(horzcoverage, horzConstruction, minoverlap, self.font, vert=False)
+        self._variantsvert = MathVariants(
+            vertcoverage, vertConstruction, minoverlap, self.font, vert=True)
+        self._variantshorz = MathVariants(
+            horzcoverage, horzConstruction, minoverlap, self.font, vert=False)
 
     def kernsuper(self, glyph1: GlyphType, glyph2: GlyphType) -> tuple[int, int]:
         ''' Calculate superscript kerning between the two glyphs
 
             Args:
                 glyph1: Last glyph in base
                 glyph2: First glyph in superscript
@@ -252,93 +261,113 @@
                 kern: Kerning shift to apply in x direction
                 shift: Upward shift of superscript with respect to baseline
         '''
         if self.kernInfo is None:
             return 0, max(self.consts.superscriptShiftUp,
                           self.consts.superscriptBottomMin)
 
-        g1 = self.kernInfo.glyph(glyph1.index)
-        g2 = self.kernInfo.glyph(glyph2.index)
+        glyph1_kern = self.kernInfo.glyph(glyph1.index)
+        glyph2_kern2 = self.kernInfo.glyph(glyph2.index)
 
         # Extended shape, need to raise superscript up, but only if we're using
         # a variant
         if self._extendedShapeCoverage.covidx(glyph1.index) is not None:
             shiftup = glyph1.path.bbox.ymax - self.consts.superscriptShiftUp/2
         else:
             shiftup = self.consts.superscriptShiftUp
 
-        h1 = shiftup + glyph2.path.bbox.ymin * self.consts.scriptPercentScaleDown/100
-        h2 = glyph1.path.bbox.ymax - shiftup
-        k1 = k2 = 0
-        if g1:
-            k1 += g1.topright.getkern(h1)
-            k2 += g1.topright.getkern(h2)
-        if g2:
-            k1 += g2.bottomleft.getkern(h1)
-            k2 += g2.bottomleft.getkern(h2)
-        return min(k1, k2), shiftup
+        height1 = shiftup + glyph2.path.bbox.ymin * self.consts.scriptPercentScaleDown/100
+        height2 = glyph1.path.bbox.ymax - shiftup
+        kern1 = kern2 = 0
+        if glyph1_kern:
+            kern1 += glyph1_kern.topright.getkern(height1)
+            kern2 += glyph1_kern.topright.getkern(height2)
+        if glyph2_kern2:
+            kern1 += glyph2_kern2.bottomleft.getkern(height1)
+            kern2 += glyph2_kern2.bottomleft.getkern(height2)
+        return min(kern1, kern2), shiftup
 
     def kernsub(self, glyph1: GlyphType, glyph2: GlyphType) -> tuple[int, int]:
         ''' Calculate subscript kerning
 
             Args:
                 glyph1: Last glyph in base
                 glyph2: First glyph in subscript
 
             Returns:
                 kern: Kerning shift to apply in x direction
                 shift: Downward shift of subscript with respect to baseline
         '''
         if self.kernInfo is None:
             return 0, max(self.consts.subscriptTopMax,
-                           self.consts.subscriptShiftDown)
+                          self.consts.subscriptShiftDown)
 
-        g1 = self.kernInfo.glyph(glyph1.index)
-        g2 = self.kernInfo.glyph(glyph2.index)
+        glyph1_kern = self.kernInfo.glyph(glyph1.index)
+        glyph2_kern = self.kernInfo.glyph(glyph2.index)
 
         # Correction heights
         shiftdn = self.consts.subscriptShiftDown - glyph1.path.bbox.ymin
-        h1 = -shiftdn + glyph2.path.bbox.ymax * self.consts.scriptPercentScaleDown/100
-        h2 = glyph1.path.bbox.ymin + shiftdn
-        k1 = k2 = 0
-        if g1:
-            k1 += g1.bottomright.getkern(h1)
-            k2 += g1.bottomright.getkern(h2)
-        if g2:
-            k1 += g2.topleft.getkern(h1)
-            k2 += g2.topleft.getkern(h2)
-        return min(k1, k2), shiftdn
+        height1 = -shiftdn + glyph2.path.bbox.ymax * self.consts.scriptPercentScaleDown/100
+        height2 = glyph1.path.bbox.ymin + shiftdn
+        kern1 = kern2 = 0
+        if glyph1_kern:
+            kern1 += glyph1_kern.bottomright.getkern(height1)
+            kern2 += glyph1_kern.bottomright.getkern(height2)
+        if glyph2_kern:
+            kern1 += glyph2_kern.topleft.getkern(height1)
+            kern2 += glyph2_kern.topleft.getkern(height2)
+        return min(kern1, kern2), shiftdn
 
-    def variant(self, glyphid: int, height: float, vert: bool=True) -> GlyphType:
+    def variant(self, glyphid: int, height: float, vert: bool = True) -> GlyphType:
         ''' Get a height variant for the glyph
 
             glyphid: Glyph index
             height: Desired height of glyph in font units
             vert: Vertical variant or horizontal variant
         '''
         if vert:
             variant = self._variantsvert.getvariant(glyphid, height)
         else:
             variant = self._variantshorz.getvariant(glyphid, height)
         return variant
 
+    def variant_minmax(self, glyphid: int, ymin: float, ymax: float,
+                       vert: bool = True) -> GlyphType:
+        ''' Get a height variant for the glyph that covers or exceeds the range (ymin, ymax)
+
+            Args:
+                glyphid: Glyph index
+                ymin: Minimum y value to contain
+                ymax: Maximum y value to contain
+                vert: Vertical variant or horizontal variant
+        '''
+        if vert:
+            variant = self._variantsvert.getvariant_minmax(glyphid, ymin=ymin, ymax=ymax)
+        else:
+            variant = self._variantshorz.getvariant_minmax(glyphid, ymin=ymin, ymax=ymax)
+        return variant
+
     def isextended(self, glyphid: int) -> bool:
         ''' Determine if glyph is an extended shape (has stretchy variants) '''
         return self._extendedShapeCoverage.covidx(glyphid) is not None
 
+    def topattachment(self, glyphid: int) -> Optional[float]:
+        ''' Get x-position to align an accent over the given base glyph ''' 
+        return self.topAccentAttachment.getvalue(glyphid)
+
 
 class MathConstructionTable:
     ''' Math Construction Table, listing size variants for a glyph
 
         Args:
             ofst: Byte offset to table in font file
             font: Font
             vert: Vertical or horizontal variant
     '''
-    def __init__(self, ofst: int, font: 'MathFont', vert: bool=True):
+    def __init__(self, ofst: int, font: 'MathFont', vert: bool = True):
         fileptr = font.fontfile.tell()
         font.fontfile.seek(ofst)
         assemblyofst = font.fontfile.readuint16()
         varcount = font.fontfile.readuint16()
         self.variants = {}
         for i in range(varcount):
             varglyph = font.fontfile.readuint16()
@@ -349,110 +378,154 @@
         if assemblyofst:
             self.assembly = MathAssembly(ofst+assemblyofst, font, vert=vert)
         else:
             self.assembly = None
         font.fontfile.seek(fileptr)
 
 
+class AssembledGlyph(SimpleGlyph):
+    ''' Assembled glyph from Math Assembly Table
+
+        Args:
+            index: glyph index
+            glyphs: list of glyphs included in the assembly
+            offsets: offset (either vertical or horizontal) for each
+                glyph in the assembly
+            vert: Vertical or horizontal assembly
+            font: Font instance
+    '''
+    def __init__(self,
+                 index: int,
+                 glyphs: Sequence[GlyphType],
+                 offsets: Sequence[float],
+                 vert: bool,
+                 font: 'MathFont'):
+        self.index = index
+        self.glyphs = glyphs
+        self.offsets = offsets
+        self.vert = vert
+
+        if self.vert:
+            xmin = min([g.path.bbox.xmin for g in glyphs])
+            xmax = max([g.path.bbox.xmax for g in glyphs])
+            ymin = int(glyphs[0].path.bbox.ymin + offsets[0])
+            ymax = int(glyphs[-1].path.bbox.ymax + offsets[-1])
+        else:
+            xmin = int(glyphs[0].path.bbox.xmin)
+            xmax = int(glyphs[-1].path.bbox.xmax + offsets[-1])
+            ymin = min([g.path.bbox.ymin for g in glyphs])
+            ymax = max([g.path.bbox.ymax for g in glyphs])
+        bbox = BBox(xmin, xmax, ymin, ymax)
+        super().__init__(index, [], bbox, font)
+
+    def advance(self, nextchr=None) -> float:
+        ''' X-advance '''
+        return self.bbox.xmax
+
+    def svgpath(self, x0: float = 0, y0: float = 0,
+                scale_factor: float = 1) -> Optional[ET.Element]:
+        ''' Get svg <path> element for glyph, normalized to 12-point font '''
+        element = ET.Element('g')
+
+        for glyph, ofst in zip(self.glyphs, self.offsets):
+            path = ''
+            for operator in glyph.operators:
+                if self.vert:
+                    operator = operator.xform(1, 0, 0, 1, 0, ofst, 1, 1)
+                else:
+                    operator = operator.xform(1, 0, 0, 1, ofst, 0, 1, 1)
+                segment = operator.path(x0, y0, scale=self.funits_to_points(1, scale_factor))
+                if segment[0] == 'M' and path != '':
+                    path += 'Z '  # Close intermediate segments
+                path += segment
+            if path == '':
+                continue  # Don't add empty path
+            path += 'Z '
+            element.append(ET.Element('path', attrib={'d': path}))
+        return element
+
+
 class MathAssembly:
     ''' Math assembly table, for combining several glyphs to extend the size
         beyond the font built-in glyphs (for example, making a really big
         curly brace)
 
         Args:
             ofst: Byte offset into font file
             font: Font
             vert: Vertical or horizontal variant
     '''
-    def __init__(self, ofst: int, font: 'MathFont', vert: bool=True):
+    def __init__(self, ofst: int, font: 'MathFont', vert: bool = True):
         self.vert = vert
         self.font = font
         font.fontfile.seek(ofst)
         self.italicscorrection = read_valuerecord(font.fontfile)
         partcnt = font.fontfile.readuint16()
         self.parts = []
         for i in range(partcnt):
             self.parts.append(GlyphPartRecord(
                 font.fontfile.readuint16(),
                 font.fontfile.readuint16(),
                 font.fontfile.readuint16(),
                 font.fontfile.readuint16(),
                 font.fontfile.readuint16()))
 
-    def assemble(self, reqsize: float, minoverlap: float) -> glyph.CompoundGlyph:
+    def assemble(self, reqsize: float, minoverlap: float) -> AssembledGlyph:
         ''' Build glyph assembly, combining parts to create any required size
 
             Args:
                 reqsize: Desired glyph size
                 minoverlap: Minimum overlap from variants table
         '''
         size = 0.
-        N = 0
+        num_extenders = 0
 
         # Determine number of extender parts needed.
         while size < reqsize:
             # Min overlap give largest size with this many extenders
 
             testparts = []
             for part in self.parts:
                 if part.partFlags:
-                    testparts.extend([part]*N)
+                    testparts.extend([part]*num_extenders)
                 else:
                     testparts.append(part)
 
             y = 0.
             for i, part in enumerate(testparts):
                 if i > 0:
                     y -= minoverlap
                 y += part.fullAdvance
             size = y
-            N += 1
+            num_extenders += 1
 
         # Decrease overlap since full extenders make it too tall
         dy = (size - reqsize) / (len(testparts)-1)
 
         # Build transforms for compound glyph
-        xforms = []
+        offsets = []
         if self.vert:
             y = -reqsize/2 + self.font.math.consts.axisHeight
-            ymin = y
         else:
             y = 0.
         for i, part in enumerate(testparts):
             if i > 0:
                 y -= minoverlap + dy
             if self.vert:
-                xforms.append(Xform(1, 0, 0, 1, 0, y, False))
+                offsets.append(y - self.font.glyph_fromid(part.glyphId).bbox.ymin)
             else:
-                xforms.append(Xform(1, 0, 0, 1, y, 0, False))
+                offsets.append(y)
             y += part.fullAdvance
-        size = y
 
         # Put together the CompoundGlyph
         glyphs = [self.font.glyph_fromid(part.glyphId) for part in testparts]
-        
+
         # Make a unique ID, negative so it can't clash with other glyphs
         glyfid = -(testparts[0].glyphId + int(reqsize) << 16)
-
-        if self.vert:
-            xmin = min([g.path.bbox.xmin for g in glyphs])
-            xmax = max([g.path.bbox.xmax for g in glyphs])
-            ymin = min([ymin+g.path.bbox.ymin for g in glyphs])
-            ymax = size
-        else:
-            xmin = min([g.path.bbox.xmin for g in glyphs])
-            xmax = size
-            ymin = min([g.path.bbox.ymin for g in glyphs])
-            ymax = max([g.path.bbox.ymax for g in glyphs])
-
-        bbox = BBox(xmin, xmax, ymin, ymax)
-        gc = GlyphComp(glyphs, xforms, bbox)
-        glf = glyph.CompoundGlyph(glyfid, gc, self.font)
-        glf.advance = lambda x=bbox.xmax: x  # type: ignore
-        return glf
+        return AssembledGlyph(glyfid, glyphs, offsets, vert=self.vert, font=self.font)
 
 
 class MathVariants:
     ''' Math Variants Table. Provides different glyphs for different size symbols,
         such as curly braces and square roots.
     '''
     def __init__(self, coverage: Coverage, construction: Sequence[MathConstructionTable],
@@ -461,36 +534,62 @@
         self.construction = construction
         self.minoverlap = minoverlap
         self.font = font
         self.vert = vert
 
     def getvariant(self, glyphid: int, size: float) -> GlyphType:
         ''' Get the proper size variant for the glyphid '''
+        glf: GlyphType
         covidx = self.coverage.covidx(glyphid)
         if covidx is None:
             # Not covered by a variant
             return self.font.glyph_fromid(glyphid)
 
         construction = self.construction[covidx]
         variants = construction.variants
-        glf: GlyphType
         try:
             variantid = variants[min(k for k in variants if k >= size)]
 
         except ValueError:
             # size is bigger than all variants. Use assembly table.
             if construction.assembly:
                 glf = construction.assembly.assemble(size, self.minoverlap)
             else:
                 glf = self.font.glyph_fromid(variants[max(variants.keys())])
         else:
             glf = self.font.glyph_fromid(variantid)
 
         return glf
 
+    def getvariant_minmax(self, glyphid: int, ymin: float, ymax: float) -> GlyphType:
+        ''' Get the smallest variant that encloses ymin and ymax '''
+        glf: GlyphType
+        covidx = self.coverage.covidx(glyphid)
+        if covidx is None:
+            # Not covered by a variant
+            return self.font.glyph_fromid(glyphid)
+
+        construction = self.construction[covidx]
+        variants = construction.variants
+
+        gids = list(variants.values())
+        ymins = [self.font.glyph_fromid(gid).bbox.ymin for gid in gids]
+        ymaxs = [self.font.glyph_fromid(gid).bbox.ymax for gid in gids]
+        for gid, ymn, ymx in zip(gids, ymins, ymaxs):
+            if ymn <= ymin and ymx >= ymax:
+                glf = self.font.glyph_fromid(gid)
+                break
+        else:
+            height = ymax-ymin
+            if height > ymaxs[-1] - ymins[-1] and construction.assembly:
+                glf = construction.assembly.assemble(height, self.minoverlap)
+            else:
+                glf = self.font.glyph_fromid(gids[-1])
+        return glf
+
 
 class MathKernTable:
     ''' Math Kerning Table, for adjusting sub/superscripts
 
         Args:
             ofst: Byte offset into font file
             fontfile: font file
@@ -518,15 +617,16 @@
         else:
             i += 1
         return self.kernvalues[i]
 
 
 class ZeroKern:
     ''' A kerning table with 0 kerning '''
-    def getkern(self, height):
+    def getkern(self, height: float) -> int:
+        ''' Get kerning for this height '''
         return 0
 
 
 class MathKernInfoTable:
     ''' Math Kerning Info Table, listing of MathKernTables
 
         Args:
```

### Comparing `ziamath-0.7/ziamath/operators.py` & `ziamath-0.8/ziamath/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
     Defines how much space to put around operators such as in "x + y".
     Depends on where the operator falls in the mrow (prefix, infix, or postfix)
 
     See Appendix F of MathML2 Documentation:
     https://www.w3.org/TR/MathML2/appendixf.html
 '''
+from __future__ import annotations
+
 
 operators = {
     ('(', 'prefix'):  {'fence': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
     (')', 'postfix'): {'fence': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
     ('[', 'prefix'):  {'fence': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
     (']', 'postfix'): {'fence': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
     ('{', 'prefix'):  {'fence': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},
@@ -50,16 +52,17 @@
     ('∋', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &SuchThat;
     ('⫤', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DoubleLeftTee;
     ('⊨', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DoubleRightTee;
     ('⊤', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &DownTee;
     ('⊣', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &LeftTee;
     ('⊢', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &RightTee;
     ('⥰', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},  # &RoundImplies;
-    ('|', 'infix'): {'stretchy': 'true',  'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},
-    ('||', 'infix'): {'lspace': 'mediummathspace', 'rspace': 'mediummathspace'},
+    ('|', 'infix'): {'stretchy': 'true',  'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
+    ('‖', 'infix'): {'stretchy': 'true',  'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
+    ('||', 'infix'): {'lspace': '0em', 'rspace': '0em'},
     ('⩔', 'infix'): {'stretchy': 'true',  'lspace': 'mediummathspace', 'rspace': 'mediummathspace'},  # &Or;
     ('&&', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},
     ('⩓', 'infix'): {'stretchy': 'true',  'lspace': 'mediummathspace', 'rspace': 'mediummathspace'},  # &And;
     ('&', 'infix'): {'lspace': 'thickmathspace', 'rspace': 'thickmathspace'},
     ('!', 'prefix'): {'lspace': '0em', 'rspace': 'thickmathspace'},
     ('⫬', 'prefix'): {'lspace': '0em', 'rspace': 'thickmathspace'},  # &Not;
     ('∃', 'prefix'): {'lspace': '0em', 'rspace': 'thickmathspace'},  # &Exists;
@@ -252,21 +255,22 @@
     ('', 'infix'): {'lspace': '0em', 'rspace': '0em'},  # &InvisibleTimes;
     ('·', 'infix'): {'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &CenterDot;
     ('⊗', 'infix'): {'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &CircleTimes;
     ('⋁', 'infix'): {'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &Vee;
     ('⋀', 'infix'): {'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &Wedge;
     ('⋄', 'infix'): {'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &Diamond;
     ('∖', 'infix'): {'stretchy': 'true',  'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},  # &Backslash;
-    ('/','infix'): {'stretchy': 'true',  'lspace': 'thinmathspace', 'rspace': 'thinmathspace'},
+    ('/','infix'): {'lspace': '0em', 'rspace': '0em'},
     ('−', 'prefix'): {'lspace': '0em', 'rspace': 'veryverythinmathspace'},
     ('+', 'prefix'): {'lspace': '0em', 'rspace': 'veryverythinmathspace'},
     ('∓', 'prefix'): {'lspace': '0em', 'rspace': 'veryverythinmathspace'},
     ('±', 'prefix'): {'lspace': '0em', 'rspace': 'veryverythinmathspace'},
     ('.', 'infix'): {'lspace': '0em', 'rspace': '0em'},
     ('⨯', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},  # &Cross;
+    ('×', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
     ('÷', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
     ('**', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
     ('⊙', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},
     ('∘', 'infix'): {'lspace': 'verythinmathspace', 'rspace': 'verythinmathspace'},  # &SmallCircle;
     ('□', 'prefix'): {'lspace': '0em', 'rspace': 'verythinmathspace'},  # &Square;
     ('∇', 'prefix'): {'lspace': '0em', 'rspace': 'verythinmathspace'},  # &Del;
     ('∂', 'prefix'): {'lspace': '0em', 'rspace': 'verythinmathspace'},  # &PartialD;
@@ -345,8 +349,27 @@
     ('_', 'postfix'): {'accent': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},  # &UnderBar;
     ('⏟', 'postfix'): {'accent': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},  # &UnderBrace;
     ('⎵', 'postfix'): {'accent': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},  # &UnderBracket;
     ('⏝', 'postfix'): {'accent': 'true', 'stretchy': 'true',  'lspace': '0em', 'rspace': '0em'},  # &UnderParenthesis;
 }
 
 
-integrals = ['∫', '∬', '∭', '∲', '∮', '∳', '∯', '∰', ]
+integrals = ['∫', '∬', '∭', '∲', '∮', '∳', '∯', '∰', ]
+fences = [op[0] for op, params in operators.items() if params.get('fence') == 'true'] + ['|', '∣', '❘', '‖']
+names = set(op[0] for op in operators.keys())
+
+
+def get_params(name: str, form: str) -> dict[str, str]:
+    ''' Get parameters for the given operator name and form '''
+    if form == 'none':
+        # form of 'none' is given to single element mrows like {,}
+        return {}
+
+    params = operators.get((name, form), {})
+    if not params:
+        params = operators.get((name, 'infix'), {})
+    if not params:
+        params = operators.get((name, 'postfix'), {})
+    if not params:
+        params = operators.get((name, 'prefix'), {})
+
+    return params.copy()
```

### Comparing `ziamath-0.7/ziamath.egg-info/PKG-INFO` & `ziamath-0.8/ziamath.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: ziamath
-Version: 0.7
-Summary: Render MathML and LaTeX Math to SVG without Latex installation
-Home-page: https://ziamath.readthedocs.io/
+Version: 0.8
+Summary: Render MathML and LaTeX Math to SVG in pure Python without Latex installation
+Home-page: https://ziamath.readthedocs.io
 Author: Collin J. Delker
-Author-email: ziaplot@collindelker.com
-Project-URL: Source, https://bitbucket.org/cdelker/ziamath
+Author-email: code@collindelker.com
+License: MIT
+Project-URL: Documentation, https://ziamath.readthedocs.io
+Project-URL: Source Code, https://github.com/cdelker/ziamath
 Keywords: MathML,LaTeX,math,font,truetype,opentype,svg
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: latex
 License-File: LICENSE.txt
 
 # ziamath
 
-Render MathML or LaTeX Math expressions as SVG. Does not require a Latex installation.
+Render MathML or LaTeX Math expressions as SVG using pure Python. Does not require a Latex installation, nor a network connection.
 
 Ziamath comes with the STIXTwoMath-Regular font installed for use by default.
 Other Math-enabled Open Type fonts (TTF or OTF files) may also be used.
 
-![Example](example.png)
+![Example](https://github.com/cdelker/ziamath/blob/05e25b1789acc8ee816971d384aa851ffb197f7a/example.png)
 
+Documentation is available at [readthedocs](https://ziamath.readthedocs.io).
 
-Documentation is available at [readthedocs](https://ziamath.readthedocs.io)
+Also try the [online demo](https://cdelker.github.io/pyscript/ziamath.html) based on Pyscript.
```

