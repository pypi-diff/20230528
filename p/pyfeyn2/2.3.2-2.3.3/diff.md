# Comparing `tmp/pyfeyn2-2.3.2.tar.gz` & `tmp/pyfeyn2-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.3.2.tar", max compression
+gzip compressed data, was "pyfeyn2-2.3.3.tar", max compression
```

## Comparing `pyfeyn2-2.3.2.tar` & `pyfeyn2-2.3.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-04-16 12:04:03.047864 pyfeyn2-2.3.2/LICENSE
--rw-r--r--   0        0        0     3115 2023-04-16 12:04:03.051864 pyfeyn2-2.3.2/README.md
--rw-r--r--   0        0        0      154 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      650 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/diagram.py
--rw-r--r--   0        0        0      774 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2073 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0     3332 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2733 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      273 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0     2748 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3638 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5977 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1616 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6640 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     7108 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13245 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41394 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12623 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     9184 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     9026 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      863 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2364 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1701 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     2113 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      527 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3846 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-04-16 12:04:03.135863 pyfeyn2-2.3.2/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1976 2023-04-16 12:04:03.139863 pyfeyn2-2.3.2/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2511 2023-04-16 12:04:05.275844 pyfeyn2-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 pyfeyn2-2.3.2/setup.py
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pyfeyn2-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-27 22:06:11.091484 pyfeyn2-2.3.3/LICENSE
+-rw-r--r--   0        0        0     3115 2023-05-27 22:06:11.091484 pyfeyn2-2.3.3/README.md
+-rw-r--r--   0        0        0      154 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2838 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      647 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/diagram.py
+-rw-r--r--   0        0        0      768 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     2068 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0     3335 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2734 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      279 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2748 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3596 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5926 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1617 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     6922 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7036 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12740 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9146 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     8914 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2114 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3850 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2621 2023-05-27 22:06:13.151519 pyfeyn2-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.3/setup.py
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.3/PKG-INFO
```

### Comparing `pyfeyn2-2.3.2/LICENSE` & `pyfeyn2-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/README.md` & `pyfeyn2-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/auto/bend.py` & `pyfeyn2-2.3.3/pyfeyn2/auto/bend.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def _auto_bend_1(i, fd):
     p = fd.propagators[i]
     p.bend = True
     ref = []
     # collect all references to the same vertex
     for c in fd.propagators:
         if c.target == p.target:
-            ref += [fd.get_vertex(c.source)]
+            ref += [fd.get_point(c.source)]
         if c.source == p.target:
-            ref += [fd.get_vertex(c.target)]
+            ref += [fd.get_point(c.target)]
     sumrefx = 0
     sumrefy = 0
-    me = fd.get_vertex(p.target)
+    me = fd.get_point(p.target)
     for r in ref:
         sumrefx += r.x - me.x
         sumrefy += r.y - me.y
 
     dire = "up"
     if sumrefy > 0:
         dire = "down"
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/auto/diagram.py` & `pyfeyn2-2.3.3/pyfeyn2/auto/diagram.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     """
     d = fd
     SCALE = scale
     d.legs[0].with_xy(-SCALE, SCALE)
     d.legs[1].with_xy(-SCALE, -SCALE)
     d.legs[2].with_xy(SCALE, SCALE)
     d.legs[3].with_xy(SCALE, -SCALE)
-    d = feynman_adjust_points(d, size=15, override_vertices=False)
+    d = feynman_adjust_points(d, size=15, clear_vertices=False)
     auto_bend(d)
     auto_label(d.propagators)
     auto_label(d.legs)
     return d
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/auto/position.py` & `pyfeyn2-2.3.3/pyfeyn2/auto/position.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     """Scale the positions of the vertices and legs."""
     for v in fd.vertices:
         v.x *= scale
         v.y *= scale
     return fd
 
 
-def feynman_adjust_points(feyndiag, size=5, override_vertices=True):
+def feynman_adjust_points(feyndiag, size=5, clear_vertices=False):
     """Adjust the points of the vertices and legs using Dot language algorithms."""
     fd = feyndiag
-    if override_vertices:
+    if clear_vertices:
         for v in fd.vertices:
             v.x = None
             v.y = None
     norm = size
     dot = feynman_to_dot(fd, resubstituteslash=False)
     positions = dot_to_positions(dot)
     mmax = 0
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.3.3/pyfeyn2/feynmandiagram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """Moved to :py:mod:`feynml`"""
 from importlib.metadata import version
 
 from feynml.connector import Connector as Connector_
 from feynml.feynmandiagram import FeynmanDiagram as FeynmanDiagram_
 from feynml.feynml import FeynML as FeynML_
-from feynml.feynml import Head as Head_
-from feynml.feynml import Meta as Meta_
-from feynml.feynml import Tool as Tool_
+from feynml.head import Head as Head_
+
+# from feynml.feynml import Tool as Tool_
 from feynml.leg import Leg as Leg_
+from feynml.meta import Meta as Meta_
 from feynml.momentum import Momentum as Momentum_
 from feynml.pdgid import PDG as PDG_
 from feynml.point import Point as Point_
 from feynml.propagator import Propagator as Propagator_
 from feynml.styled import Styled as Styled_
 from feynml.vertex import Vertex as Vertex_
 from smpl_doc import doc
 
 
 class Head(Head_):
     class Meta(Head_.Meta):
         pass
 
-    @doc.deprecated("2.2.6", "Directly use feynml.feynml.Head")
+    @doc.deprecated("2.2.6", "Directly use feynml.head.Head")
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Meta(Meta_):
     class Meta(Meta_.Meta):
         pass
 
-    @doc.deprecated("2.2.6", "Directly use feynml.feynml.Meta")
+    @doc.deprecated("2.2.6", "Directly use feynml.meta.Meta")
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class Tool(Tool_):
-    class Meta(Tool_.Meta):
-        pass
-
-    @doc.deprecated("2.2.6", "Directly use feynml.feynml.Tool")
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+# class Tool(Tool_):
+#    class Meta(Tool_.Meta):
+#        pass
+#
+#    @doc.deprecated("2.2.6", "Directly use feynml.feynml.Tool")
+#    def __init__(self, *args, **kwargs):
+#        super().__init__(*args, **kwargs)
 
 
 class Connector(Connector_):
     @doc.deprecated("2.2.6", "Directly use feynml.connector.Connector")
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/interface/dot.py` & `pyfeyn2-2.3.3/pyfeyn2/interface/dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def _fake_styler(fd, p):
     return 'style="draw=none"'
 
 
 def get_rankdir(fdstyle):
     rankdir = None
     if fdstyle.getProperty("direction") is None:
-        warn("direction is unkown, using default of 'right'")
+        warn("direction is unknown, using default of 'right'")
         rankdir = "LR"
     else:
         rdir = fdstyle.getProperty("direction").value
         if rdir == "right":
             rankdir = "LR"
         elif rdir == "left":
             rankdir = "RL"
@@ -28,23 +28,23 @@
             raise Exception(f"Unknown direction: {rdir}")
     return rankdir
 
 
 def get_layout(fdstyle):
     layout = None
     if fdstyle.getProperty("layout") is None:
-        warn("layout is unknwon, using default of 'dot'")
+        warn("layout is unknown, using default of 'dot'")
         layout = "dot"
     else:
         layout = fdstyle.getProperty("layout").value
     return layout
 
 
 def feynman_to_dot(fd, resubstituteslash=True, styler=_fake_styler):
-    # TODO better use pydot? still alive? or grpahviz?
+    # TODO better use pydot? still alive? or graphviz?
     fdstyle = fd.get_style(fd)
     rankdir = get_rankdir(fdstyle)
     layout = get_layout(fdstyle)
 
     thestyle = ""
     src = "graph G {\n"
     src += f"rankdir={rankdir};\n"
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/mkfeyndiag.py` & `pyfeyn2-2.3.3/pyfeyn2/mkfeyndiag.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/all.py` & `pyfeyn2-2.3.3/pyfeyn2/render/all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import shutil
 import tempfile
 import traceback
 from typing import List
 
-from feynml.types import get_shapes, get_types
+from feynml.shape import get_shapes
+from feynml.type import get_types
 from matplotlib import pyplot as plt
 from pylatex import Figure, NoEscape, SubFigure
 
 from pyfeyn2.render.latex.dot import DotRender
 from pyfeyn2.render.latex.feynmp import FeynmpRender
 from pyfeyn2.render.latex.latex import LatexRender
 from pyfeyn2.render.latex.tikzfeynman import TikzFeynmanRender
@@ -97,23 +98,19 @@
 
         if subfigure:
             super().render(file, show, resolution, width, height)
         shutil.rmtree(self.dirpath)
 
     @classmethod
     def valid_styles(style: str) -> List[str]:
-        return sorted(
-            list(set([i for r in renders.values() for i in r.valid_styles()]))
-        )
+        return sorted(list({i for r in renders.values() for i in r.valid_styles()}))
 
     @classmethod
     def valid_attributes(attr: str) -> List[str]:
-        return sorted(
-            list(set([i for r in renders.values() for i in r.valid_attributes()]))
-        )
+        return sorted(list({i for r in renders.values() for i in r.valid_attributes()}))
 
     @classmethod
     def valid_types(typ: str) -> List[str]:
         return sorted(get_types())
         # return [i for r in renders.values() for i in r.valid_types()]
 
     @classmethod
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.3.3/pyfeyn2/render/latex/dot.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,26 +88,26 @@
         self.src_dot = self.src_dot.replace(REPLACE_THIS_WITH_A_BACKSLASH, "\\")
 
     def get_src_dot(self):
         return self.src_dot
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
-        return super(DotRender, cls).valid_attributes() + [
+        return super().valid_attributes() + [
             "x",
             "y",
             "label",
             "style",
         ]
 
     @classmethod
     def valid_types(cls) -> List[str]:
-        return super(DotRender, cls).valid_types() + list(map_feyn_to_tikz.keys())
+        return super().valid_types() + list(map_feyn_to_tikz.keys())
 
     @classmethod
     def valid_styles(cls) -> bool:
-        return super(DotRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "direction",
             "layout",
             "length",
         ]
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.3.3/pyfeyn2/render/latex/feynmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,20 +182,20 @@
 
     def set_feynman_diagram(self, fd):
         super().set_feynman_diagram(fd)
         self.set_src_diag(NoEscape(feynman_to_feynmp(fd)))
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
-        return super(FeynmpRender, cls).valid_attributes() + ["label", "style"]
+        return super().valid_attributes() + ["label", "style"]
 
     @classmethod
     def valid_types(cls) -> List[str]:
-        return super(FeynmpRender, cls).valid_types() + list(type_map.keys())
+        return super().valid_types() + list(type_map.keys())
 
     @classmethod
     def valid_styles(cls) -> bool:
-        return super(FeynmpRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "direction",
             "tension",
         ]
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.3.3/pyfeyn2/render/latex/latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         height=None,
         clean_up=True,
     ):
         delete = False
         if file is None:
             delete = True
             file = "tmp"
-        file = re.sub("\.pdf$", "", file.strip())
+        file = re.sub(r"\.pdf$", "", file.strip())
         self.generate_pdf(
             file,
             clean_tex=clean_up,
             compiler="lualatex",
             compiler_args=["-shell-escape"],
         )
         wi = WImage(
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.3.3/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.3.3/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import List
 from warnings import warn
 
 from pylatex import Command
 from pylatex.utils import NoEscape
 
 from pyfeyn2.feynmandiagram import Connector, FeynmanDiagram, Leg, Vertex
@@ -108,26 +109,36 @@
     end = ret[:-1]
 
     if suffix is not None:
         suffix = "{" + suffix + "}"
     else:
         suffix = ""
 
+    if v.x is None or v.y is None:
+        warnings.warn("Vertex position not set")
+        return (
+            f"\t\\vertex ({v.id}) [{end}] {suffix};\n"
+            + f"\t\\vertex ({v.id}clone) [] {suffix};\n"
+        )
+
     return (
         f"\t\\vertex ({v.id}) [{end}] at ({v.x},{v.y}) {suffix};\n"
         + f"\t\\vertex ({v.id}clone) [] at ({v.x},{v.y});\n"
     )
 
 
 def stylize_leg_node(l: Leg):
     style = ""
     if l.external is not None:
         style += "label=" + l.external + ","
     sty = style[:-1]
 
+    if l.x is None or l.y is None:
+        warnings.warn("Leg position not set")
+        return f"\t\\vertex ({l.id}) [{sty}];\n"
     return f"\t\\vertex ({l.id}) [{sty}] at ({l.x},{l.y});\n"
 
 
 def get_line(source_id, target_id, style):
     # Fix self-loop
     if source_id == target_id:
         return f"\t\t({source_id}) -- [{style}] ({target_id}clone),\n"
@@ -189,15 +200,15 @@
 
     def set_feynman_diagram(self, fd):
         super().set_feynman_diagram(fd)
         self.set_src_diag(NoEscape(feynman_to_tikz_feynman(fd)))
 
     @classmethod
     def valid_styles(cls) -> bool:
-        return super(TikzFeynmanRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "symbol",
             "color",
             "opacity",
             "bend-direction",
             "bend-in",
             "bend-out",
@@ -205,21 +216,21 @@
             "bend-min-distance",
             "momentum-arrow",
             "momentum-arrow-sense",
         ]
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
-        return super(TikzFeynmanRender, cls).valid_attributes() + [
+        return super().valid_attributes() + [
             "x",
             "y",
             "label",
             "style",
         ]
 
     @classmethod
     def valid_types(cls) -> List[str]:
-        return super(TikzFeynmanRender, cls).valid_types() + list(type_map.keys())
+        return super().valid_types() + list(type_map.keys())
 
     @classmethod
     def valid_shapes(cls) -> List[str]:
-        return super(TikzFeynmanRender, cls).valid_types() + list(shape_map.keys())
+        return super().valid_types() + list(shape_map.keys())
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.3.3/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,34 +188,34 @@
             plt.savefig(file)
         if clean_up:
             plt.close()
         return diagram
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
-        return super(FeynmanRender, cls).valid_attributes() + [
+        return super().valid_attributes() + [
             "x",
             "y",
             "label",
             "style",
         ]
 
     @classmethod
     def valid_types(cls) -> List[str]:
-        return super(FeynmanRender, cls).valid_types() + list(namedlines.keys())
+        return super().valid_types() + list(namedlines.keys())
 
     @classmethod
     def valid_styles(cls) -> List[str]:
-        return super(FeynmanRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "color",
             "arrow-sense",
             "arrow-length",
             "arrow-width",
             "xamp",
             "yamp",
             "nloops",
         ]
 
     @classmethod
     def valid_shapes(cls) -> List[str]:
-        return super(FeynmanRender, cls).valid_types() + list(marker_map.keys())
+        return super().valid_types() + list(marker_map.keys())
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/lines.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,16 @@
 
     def getXY(self):
         "Return the x and y coordinates of this point as a 2-tuple."
         return self.getX(), self.getY()
 
     def setXY(self, xpos, ypos):
         "Set the x and y coordinates of this point."
+        if xpos is None or ypos is None:
+            raise Exception("Point coordinates cannot be None")
         self.setX(float(xpos))
         self.setY(float(ypos))
         return self
 
     def x(self):
         "Alias for getX()."
         return self.getX()
@@ -186,15 +188,15 @@
         if x is not None and y is not None:
             xx = x
             yy = y
         elif center is not None:
             xx = center.getX()
             yy = center.getY()
         else:
-            raise Exception("No center specified for blob.")
+            raise Exception("No (x,y) or no center specified for blob.")
 
         Point.__init__(self, xx, yy, blob, labels)
         self.setMark(copy(mark))
         self.layeroffset = 1000
         self.fillstyles = copy(fill)  # lists are mutable --
         self.strokestyles = copy(stroke)  # hence make a copy!
         ## Add this to the current diagram automatically
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/pyxrender.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,33 +35,34 @@
         for v in self.fd.vertices:
             dp = DecoratedPoint(v.x, v.y)
             dp = self.apply_layout(self.fd.get_style(v).cssText.replace("\n", " "), dp)
             if v.label is not None:
                 dp.setFillstyles(PointLabel(dp, v.label, displace=3, angle=90))
             pyxfd.add(dp)
         for l in self.fd.legs:
+            lp = Point(l.x, l.y)
             lstyle = self.fd.get_style(l)
-            tar = self.fd.get_vertex(l.target)
+            tar = self.fd.get_point(l.target)
             if lstyle.getProperty("line") is not None:
                 lname = lstyle.getProperty("line").value
             else:
                 lname = l.type  # fallback to type
             if l.is_incoming():
-                nl = NamedLine[lname](Point(l.x, l.y), Point(tar.x, tar.y))
+                nl = NamedLine[lname](lp, Point(tar.x, tar.y))
             elif l.is_outgoing():
-                nl = NamedLine[lname](Point(tar.x, tar.y), Point(l.x, l.y))
+                nl = NamedLine[lname](Point(tar.x, tar.y), lp)
             if lstyle.getProperty("bend") is not None:
                 nl = nl.bend(lstyle.getProperty("bend").value)
             nl = self.apply_layout(self.fd.get_style(l).cssText.replace("\n", " "), nl)
             nl = nl.addLabel(l.label)
 
         for p in self.fd.propagators:
             pstyle = self.fd.get_style(p)
-            src = self.fd.get_vertex(p.source)
-            tar = self.fd.get_vertex(p.target)
+            src = self.fd.get_point(p.source)
+            tar = self.fd.get_point(p.target)
             if pstyle.getProperty("line") is not None:
                 lname = pstyle.getProperty("line").value
             else:
                 lname = p.type
             nl = NamedLine[lname](Point(src.x, src.y), Point(tar.x, tar.y))
             if pstyle.getProperty("bend") is not None:
                 nl = nl.bend(pstyle.getProperty("bend").value)
@@ -216,29 +217,29 @@
                 obj.set3D(False)
             elif styledict["is3d"].lstrip().lower() in twords:
                 obj.set3D(True)
         return obj
 
     @classmethod
     def valid_types(cls):
-        return super(PyxRender, cls).valid_types() + list(NamedLine.keys())
+        return super().valid_types() + list(NamedLine.keys())
 
     @classmethod
     def valid_attributes(cls):
-        return super(PyxRender, cls).valid_attributes() + [
+        return super().valid_attributes() + [
             "style",
             "type",
             "label",
             "x",
             "y",
         ]
 
     @classmethod
     def valid_styles(cls):
-        return super(PyxRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "bend",
             "arrow-pos",
             "arrow-sense",
             "arrow-size",
             "arrow-angle",
             "arrow-constrict",
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.3.3/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/render.py` & `pyfeyn2-2.3.3/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/ascii.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,25 +234,25 @@
         scalex = (width - 1) / (maxx - minx)
         scaley = -(height - 1) / (maxy - miny)
         kickx = -minx
         kicky = -maxy
         fmt = {"scalex": scalex, "kickx": kickx, "scaley": scaley, "kicky": kicky}
 
         for p in self.fd.propagators:
-            src = self.fd.get_vertex(p.source)
-            tar = self.fd.get_vertex(p.target)
+            src = self.fd.get_point(p.source)
+            tar = self.fd.get_point(p.target)
             self.draw_connector(pane, p, src, tar, fmt)
 
         for l in self.fd.legs:
             if l.is_incoming():
                 src = Point(l.x, l.y)
-                tar = self.fd.get_vertex(l.target)
+                tar = self.fd.get_point(l.target)
                 self.draw_connector(pane, l, src, tar, fmt)
             elif l.is_outgoing():
-                src = self.fd.get_vertex(l.target)
+                src = self.fd.get_point(l.target)
                 tar = Point(l.x, l.y)
                 self.draw_connector(pane, l, src, tar, fmt)
         for v in self.fd.vertices:
             tmp_fmt = {}
             ssss = self.fd.get_style(v)
             if ssss.getProperty("symbol") is not None:
                 if ssss.getProperty("color") is not None:
@@ -290,34 +290,30 @@
         return self.src_txt
 
     def set_src_txt(self, src_txt):
         self.src_txt = src_txt
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
-        return super(ASCIIRender, cls).valid_attributes() + [
+        return super().valid_attributes() + [
             "x",
             "y",
             "label",
             "style",
         ]
 
     @classmethod
     def valid_styles(cls) -> List[str]:
-        return super(ASCIIRender, cls).valid_styles() + [
+        return super().valid_styles() + [
             "line",
             "symbol",
             "color",
             "label-color",
         ]
 
     @classmethod
     def valid_types(cls) -> List[str]:
-        return super(ASCIIRender, cls).valid_types() + list(
-            ASCIIRender.namedlines.keys()
-        )
+        return super().valid_types() + list(ASCIIRender.namedlines.keys())
 
     @classmethod
     def valid_shapes(cls) -> List[str]:
-        return super(ASCIIRender, cls).valid_types() + list(
-            ASCIIRender.namedshapes.keys()
-        )
+        return super().valid_types() + list(ASCIIRender.namedshapes.keys())
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/label.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/line.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/plainpdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """
         Return text with color via LaTeX commands.
         """
         self.preamble.append(
             Command(
                 "lstset",
                 NoEscape(
-                    "moredelim=[is][\color{"
+                    r"moredelim=[is][\color{"
                     + color
                     + "}]{@"
                     + color
                     + "!}{!"
                     + color
                     + "@}"
                 ),
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/point.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/point.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/style.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,24 +55,24 @@
         self.right = LineStyle(style=right)
         self.up = LineStyle(style=up)
         self.down = LineStyle(style=down)
 
     def next(self, dirx, diry):
         angle = super().next(dirx, diry)
         # right
-        if angle < math.pi / 4 or angle > 7 * math.pi / 4:
+        if angle <= math.pi / 4 or angle > 7 * math.pi / 4:
             return self.left.get(self.index)
         # left
-        elif angle > 3 * math.pi / 4 and angle < 5 * math.pi / 4:
+        elif angle >= 3 * math.pi / 4 and angle < 5 * math.pi / 4:
             return self.right.get(self.index)
         # up
-        elif angle > math.pi / 4 and angle < 3 * math.pi / 4:
+        elif angle >= math.pi / 4 and angle < 3 * math.pi / 4:
             return self.up.get(self.index)
         # down
-        elif angle > 5 * math.pi / 4 and angle < 7 * math.pi / 4:
+        elif angle >= 5 * math.pi / 4 and angle < 7 * math.pi / 4:
             return self.down.get(self.index)
         else:
             raise Exception("Angle not in range")
 
 
 class Compass(Style):
     def __init__(
```

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.3.3/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.2/pyproject.toml` & `pyfeyn2-2.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.3.2"
+version = "2.3.3"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -25,16 +25,16 @@
 ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 cssselect ="*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
-feynml = {version = ">=0.1.6", extras = ["interface"]}
-#feynml= {path= "../feynml", develop = true }
+feynml = {version = ">=0.1.6", extras = ["interfaces"]}
+#feynml= {path= "../feynml", develop = true, extras = ["interfaces"]}
 
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
 
@@ -47,23 +47,28 @@
 sphinx_autobuild = "*"
 sphinx_math_dollar = "*"
 myst-parser  = "*"
 toml = "*"
 colorama = "*"
 termcolor = "*"
 
-[tool.poetry.group.dev]
+[tool.poetry.group.test]
 optional = true
 
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
+[tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.3"
+
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = ">=2.20,<4.0"
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
 poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `pyfeyn2-2.3.2/setup.py` & `pyfeyn2-2.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['Wand',
  'cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'dot2tex',
  'feynman>=2.0,<3.0',
- 'feynml[interface]>=0.1.6',
+ 'feynml[interfaces]>=0.1.6',
  'graphviz',
  'ipyparallel',
  'matplotlib>=1.4.0,<4.0.0',
  'numpy>=1.6,<1.24',
  'particle',
  'pydot',
  'pygments',
@@ -39,15 +39,15 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.3.2',
+    'version': '2.3.3',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.3.2/PKG-INFO` & `pyfeyn2-2.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.3.2
+Version: 2.3.3
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 Requires-Dist: Wand
 Requires-Dist: cssselect
 Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: dot2tex
 Requires-Dist: feynman (>=2.0,<3.0)
-Requires-Dist: feynml[interface] (>=0.1.6)
+Requires-Dist: feynml[interfaces] (>=0.1.6)
 Requires-Dist: graphviz
 Requires-Dist: ipyparallel
 Requires-Dist: matplotlib (>=1.4.0,<4.0.0)
 Requires-Dist: numpy (>=1.6,<1.24)
 Requires-Dist: particle
 Requires-Dist: pydot
 Requires-Dist: pygments
```

