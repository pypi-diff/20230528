# Comparing `tmp/nutree-0.4.0.tar.gz` & `tmp/nutree-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutree-0.4.0.tar", last modified: Wed Feb 22 20:05:41 2023, max compression
+gzip compressed data, was "nutree-0.5.0.tar", last modified: Sun May 28 05:58:00 2023, max compression
```

## Comparing `nutree-0.4.0.tar` & `nutree-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-02-22 20:05:41.137525 nutree-0.4.0/
--rw-r--r--   0 martin     (501) staff       (20)      268 2023-02-22 20:04:17.000000 nutree-0.4.0/CHANGELOG.md
--rw-r--r--   0 martin     (501) staff       (20)     1069 2022-04-14 19:35:21.000000 nutree-0.4.0/LICENSE.txt
--rw-r--r--   0 martin     (501) staff       (20)     4103 2023-02-22 20:05:41.137601 nutree-0.4.0/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     2713 2022-08-13 06:00:11.000000 nutree-0.4.0/README.md
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-02-22 20:05:41.135615 nutree-0.4.0/nutree/
--rw-r--r--   0 martin     (501) staff       (20)     1107 2023-02-22 20:05:40.000000 nutree-0.4.0/nutree/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     6435 2023-02-22 16:24:55.000000 nutree-0.4.0/nutree/common.py
--rw-r--r--   0 martin     (501) staff       (20)     5914 2023-01-17 18:12:34.000000 nutree-0.4.0/nutree/diff.py
--rw-r--r--   0 martin     (501) staff       (20)     5280 2023-01-19 18:53:36.000000 nutree-0.4.0/nutree/dot.py
--rw-r--r--   0 martin     (501) staff       (20)     2776 2022-07-30 22:10:10.000000 nutree-0.4.0/nutree/fs.py
--rw-r--r--   0 martin     (501) staff       (20)    46071 2023-02-22 16:06:51.000000 nutree-0.4.0/nutree/node.py
--rw-r--r--   0 martin     (501) staff       (20)     4559 2022-08-12 19:25:13.000000 nutree-0.4.0/nutree/rdf.py
--rw-r--r--   0 martin     (501) staff       (20)    20583 2023-02-22 16:05:48.000000 nutree-0.4.0/nutree/tree.py
--rw-r--r--   0 martin     (501) staff       (20)    22919 2023-02-22 16:07:17.000000 nutree-0.4.0/nutree/typed_tree.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-02-22 20:05:41.136456 nutree-0.4.0/nutree.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     4103 2023-02-22 20:05:41.000000 nutree-0.4.0/nutree.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      561 2023-02-22 20:05:41.000000 nutree-0.4.0/nutree.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-02-22 20:05:41.000000 nutree-0.4.0/nutree.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)       49 2023-02-22 20:05:41.000000 nutree-0.4.0/nutree.egg-info/entry_points.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-04-15 09:27:55.000000 nutree-0.4.0/nutree.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)        7 2023-02-22 20:05:41.000000 nutree-0.4.0/nutree.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)      543 2022-04-14 19:35:21.000000 nutree-0.4.0/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)     2161 2023-02-22 20:05:41.138051 nutree-0.4.0/setup.cfg
--rw-r--r--   0 martin     (501) staff       (20)      167 2022-07-30 22:10:10.000000 nutree-0.4.0/setup.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-02-22 20:05:41.137407 nutree-0.4.0/tests/
--rw-r--r--   0 martin     (501) staff       (20)     5830 2022-08-13 06:00:11.000000 nutree-0.4.0/tests/test_bench.py
--rw-r--r--   0 martin     (501) staff       (20)     2100 2022-04-14 19:35:21.000000 nutree-0.4.0/tests/test_clones.py
--rw-r--r--   0 martin     (501) staff       (20)    26813 2023-02-22 16:25:12.000000 nutree-0.4.0/tests/test_core.py
--rw-r--r--   0 martin     (501) staff       (20)     2453 2023-02-19 13:58:10.000000 nutree-0.4.0/tests/test_diff.py
--rw-r--r--   0 martin     (501) staff       (20)     2058 2022-04-14 19:35:21.000000 nutree-0.4.0/tests/test_objects.py
--rw-r--r--   0 martin     (501) staff       (20)     8336 2023-02-19 13:58:06.000000 nutree-0.4.0/tests/test_serialize.py
--rw-r--r--   0 martin     (501) staff       (20)    10481 2022-12-30 12:08:09.000000 nutree-0.4.0/tests/test_typed_tree.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.289837 nutree-0.5.0/
+-rw-r--r--   0 martin     (501) staff       (20)      434 2023-05-27 14:52:54.000000 nutree-0.5.0/CHANGELOG.md
+-rw-r--r--   0 martin     (501) staff       (20)     1069 2022-04-14 19:35:21.000000 nutree-0.5.0/LICENSE.txt
+-rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-28 05:58:00.289909 nutree-0.5.0/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     2697 2023-05-20 19:09:46.000000 nutree-0.5.0/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.287783 nutree-0.5.0/nutree/
+-rw-r--r--   0 martin     (501) staff       (20)     1083 2023-05-28 05:57:59.000000 nutree-0.5.0/nutree/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     6612 2023-05-27 12:18:02.000000 nutree-0.5.0/nutree/common.py
+-rw-r--r--   0 martin     (501) staff       (20)     5910 2023-05-14 15:31:30.000000 nutree-0.5.0/nutree/diff.py
+-rw-r--r--   0 martin     (501) staff       (20)     5287 2023-05-14 15:30:35.000000 nutree-0.5.0/nutree/dot.py
+-rw-r--r--   0 martin     (501) staff       (20)     2752 2023-03-08 20:01:17.000000 nutree-0.5.0/nutree/fs.py
+-rw-r--r--   0 martin     (501) staff       (20)    47535 2023-05-27 14:41:28.000000 nutree-0.5.0/nutree/node.py
+-rw-r--r--   0 martin     (501) staff       (20)     4552 2023-05-14 15:37:56.000000 nutree-0.5.0/nutree/rdf.py
+-rw-r--r--   0 martin     (501) staff       (20)    21252 2023-05-27 19:31:30.000000 nutree-0.5.0/nutree/tree.py
+-rw-r--r--   0 martin     (501) staff       (20)    23420 2023-05-28 05:54:03.000000 nutree-0.5.0/nutree/typed_tree.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.288730 nutree-0.5.0/nutree.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      590 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)       49 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/entry_points.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-04-15 09:27:55.000000 nutree-0.5.0/nutree.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       31 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)        7 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)      954 2023-05-20 19:10:43.000000 nutree-0.5.0/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)     1875 2023-05-28 05:58:00.290294 nutree-0.5.0/setup.cfg
+-rw-r--r--   0 martin     (501) staff       (20)      143 2023-03-08 20:01:17.000000 nutree-0.5.0/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.289691 nutree-0.5.0/tests/
+-rw-r--r--   0 martin     (501) staff       (20)     5838 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_bench.py
+-rw-r--r--   0 martin     (501) staff       (20)     2076 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_clones.py
+-rw-r--r--   0 martin     (501) staff       (20)    26832 2023-05-28 05:48:14.000000 nutree-0.5.0/tests/test_core.py
+-rw-r--r--   0 martin     (501) staff       (20)     2429 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_diff.py
+-rw-r--r--   0 martin     (501) staff       (20)     2034 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_objects.py
+-rw-r--r--   0 martin     (501) staff       (20)     8820 2023-05-27 11:49:59.000000 nutree-0.5.0/tests/test_serialize.py
+-rw-r--r--   0 martin     (501) staff       (20)    14762 2023-05-27 14:44:45.000000 nutree-0.5.0/tests/test_typed_tree.py
```

### Comparing `nutree-0.4.0/LICENSE.txt` & `nutree-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nutree-0.4.0/PKG-INFO` & `nutree-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutree
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for tree data structures with an intuitive, yet powerful, API.
 Home-page: https://github.com/mar10/nutree/
 Author: Martin Wendt
 Author-email: nutree@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: nutree@wwwendt.de
 License: MIT
@@ -17,37 +17,35 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+Provides-Extra: graph
 License-File: LICENSE.txt
 
 # ![logo](https://raw.githubusercontent.com/mar10/nutree/main/docs/nutree_48x48.png) nutree
 
-[![Build Status](https://travis-ci.com/mar10/nutree.svg?branch=main)](https://app.travis-ci.com/github/mar10/nutree)
+[![Tests](https://github.com/mar10/nutree/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/nutree/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/nutree.svg)](https://pypi.python.org/pypi/nutree/)
 [![License](https://img.shields.io/pypi/l/nutree.svg)](https://github.com/mar10/nutree/blob/main/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/nutree/badge/?version=latest)](http://nutree.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/nutree/badge.svg?branch=main)](https://coveralls.io/github/mar10/nutree?branch=main)
+[![codecov](https://codecov.io/github/mar10/nutree/branch/main/graph/badge.svg?token=9xmAFm8Icl)](https://codecov.io/github/mar10/nutree)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: nutree](https://img.shields.io/badge/StackOverflow-nutree-blue.svg)](https://stackoverflow.com/questions/tagged/nutree)
 
-> Elegant trees for primates&trade;
-
-_Nutree_ is a Python library for tree data structures with an intuitive,
+> _Nutree_ is a Python library for tree data structures with an intuitive,
 yet powerful, API.
 
 **Nutree Facts**
 
 Handle multiple references of single objects ('clones') <br>
 Search by name pattern, id, or object reference <br>
 Unobtrusive handling of arbitrary objects <br>
```

### Comparing `nutree-0.4.0/README.md` & `nutree-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # ![logo](https://raw.githubusercontent.com/mar10/nutree/main/docs/nutree_48x48.png) nutree
 
-[![Build Status](https://travis-ci.com/mar10/nutree.svg?branch=main)](https://app.travis-ci.com/github/mar10/nutree)
+[![Tests](https://github.com/mar10/nutree/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/nutree/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/nutree.svg)](https://pypi.python.org/pypi/nutree/)
 [![License](https://img.shields.io/pypi/l/nutree.svg)](https://github.com/mar10/nutree/blob/main/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/nutree/badge/?version=latest)](http://nutree.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/nutree/badge.svg?branch=main)](https://coveralls.io/github/mar10/nutree?branch=main)
+[![codecov](https://codecov.io/github/mar10/nutree/branch/main/graph/badge.svg?token=9xmAFm8Icl)](https://codecov.io/github/mar10/nutree)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: nutree](https://img.shields.io/badge/StackOverflow-nutree-blue.svg)](https://stackoverflow.com/questions/tagged/nutree)
 
-> Elegant trees for primates&trade;
-
-_Nutree_ is a Python library for tree data structures with an intuitive,
+> _Nutree_ is a Python library for tree data structures with an intuitive,
 yet powerful, API.
 
 **Nutree Facts**
 
 Handle multiple references of single objects ('clones') <br>
 Search by name pattern, id, or object reference <br>
 Unobtrusive handling of arbitrary objects <br>
```

### Comparing `nutree-0.4.0/nutree/__init__.py` & `nutree-0.5.0/nutree/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Current version number.
 
 See https://www.python.org/dev/peps/pep-0440
 
 Examples
     Pre-releases (alpha, beta, release candidate):
@@ -12,15 +11,15 @@
     Developmental release (to mark 3.0.0 as 'used'. Don't publish this):
         '3.0.0.dev1'
 NOTE:
     When pywin32 is installed, number must be a.b.c for MSI builds?
     "3.0.0a4" seems not to work in this case!
 """
 # flake8: noqa
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from .common import (
     AmbiguousMatchError,
     IterMethod,
     SelectBranch,
     SkipBranch,
     StopTraversal,
```

### Comparing `nutree-0.4.0/nutree/common.py` & `nutree-0.5.0/nutree/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Functions and declarations used by the :mod:`nutree.tree` and :mod:`nutree.node`
 modules.
 """
+from __future__ import annotations
+
 import warnings
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Union
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .tree import Node
 
+#: Used as ID for the system root node
+ROOT_ID: str = "__root__"
+
+#: File format version used by `tree.save()` as `meta.$version`
+FILE_FORMAT_VERSION: str = "1.0"
 
 ItemIdType = Union[str, int]
 
 
 class TreeError(RuntimeError):
     """Base class for all `nutree` errors."""
 
@@ -58,15 +64,16 @@
     """
 
     def __init__(self, *, and_self=None):
         self.and_self = and_self
 
 
 class SelectBranch(IterationControl):
-    """Raised or returned by traversal callbacks unconditionally accept all descendants."""
+    """Raised or returned by traversal callbacks unconditionally accept all
+    descendants."""
 
 
 class StopTraversal(IterationControl):
     """Raised or returned by traversal callbacks to stop iteration.
 
     Optionally, a return value may be passed.
     Note that if a callback returns ``False``, this will be converted to an
@@ -109,15 +116,15 @@
     "round32": ("   ", "│  ", "╰─ ", "├─ "),
     "round42": ("    ", " │  ", " ╰─ ", " ├─ "),
     "round43": ("    ", "│   ", "╰── ", "├── "),
     "round43r": ("    ", " │  ", " ╰──", " ├──"),
 }
 
 
-def call_mapper(fn, node: "Node", data: dict) -> Any:
+def call_mapper(fn, node: Node, data: dict) -> Any:
     """Call the function and normalize result and exceptions.
 
     Handles `MapperCallbackType`:
     Call `fn(node, data)` if defined and return the result.
     If `fn` is undefined or returns `None`, return `data`.
     """
     if fn is None:
```

### Comparing `nutree-0.4.0/nutree/diff.py` & `nutree-0.5.0/nutree/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt and contributors; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt and contributors; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Implement diff/merge algorithms.
 """
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .tree import Tree, Node
 
 from enum import Enum
 
@@ -26,15 +27,15 @@
 def _find_child(arr, child):
     for i, c in enumerate(arr):
         if c == child:
             return (i, c)
     return (-1, None)
 
 
-def _copy_children(source: "Node", dest: "Node", add_set: set, meta: tuple) -> None:
+def _copy_children(source: Node, dest: Node, add_set: set, meta: tuple) -> None:
     assert source.has_children() and not dest.has_children()
     for n in source.children:
         n_dest = dest.append_child(n)
         add_set.add(n_dest._node_id)
         if meta:
             n_dest.set_meta(*meta)
         if n._children:
@@ -76,22 +77,22 @@
 
         flags = "[" + "], [".join(flags) + "]"
         s += f" - {flags}"
 
     return s
 
 
-def diff_tree(t0: "Tree", t1: "Tree", *, ordered=False, reduce=False) -> "Tree":
+def diff_tree(t0: Tree, t1: Tree, *, ordered=False, reduce=False) -> Tree:
     from nutree import Tree
 
     t2 = Tree(f"diff({t0.name!r}, {t1.name!r})")
     added_nodes = set()
     removed_nodes = set()
 
-    def compare(p0: "Node", p1: "Node", p2: "Node"):
+    def compare(p0: Node, p1: Node, p2: Node):
         p0_data_ids = set()
         # `p0.children` always returns an (empty) array
         for i0, c0 in enumerate(p0.children):
             p0_data_ids.add(c0._data_id)
             i1, c1 = _find_child(p1._children, c0)
 
             c2 = p2.add(c0)
```

### Comparing `nutree-0.4.0/nutree/dot.py` & `nutree-0.5.0/nutree/dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
-Functions and declarations to support `Graphviz <https://graphviz.org/doc/info/lang.html>`_.
+Functions and declarations to support 
+`Graphviz <https://graphviz.org/doc/info/lang.html>`_.
 """
+from __future__ import annotations
+
 from pathlib import Path, PurePath
 from typing import IO, TYPE_CHECKING, Generator, Union
 
 from .common import MapperCallbackType, call_mapper
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .node import Node
@@ -16,15 +18,15 @@
 try:
     import pydot
 except ImportError:
     pydot = None
 
 
 def node_to_dot(
-    node: "Node",
+    node: Node,
     *,
     add_self=False,
     unique_nodes=True,
     graph_attrs=None,
     node_attrs=None,
     edge_attrs=None,
     node_mapper=None,
@@ -38,15 +40,15 @@
         add_self (bool):
         unique_nodes (bool):
     """
     indent = "  "
     name = node.tree.name
     used_keys = set()
 
-    def _key(n: "Node"):
+    def _key(n: Node):
         return n._data_id if unique_nodes else n._node_id
 
     def _attr_str(attr_def: dict, mapper=None, node=None):
         if mapper:
             if attr_def is None:
                 attr_def = {}
             call_mapper(mapper, node, attr_def)
@@ -102,15 +104,15 @@
         attr_str = _attr_str(attr_def, edge_mapper, n)
         yield f"{indent}{_key(n._parent)} -> {_key(n)}{attr_str}"
 
     yield "}"
 
 
 def tree_to_dotfile(
-    tree: "Tree",
+    tree: Tree,
     target: Union[IO[str], str, PurePath],
     *,
     format=None,
     add_root=True,
     unique_nodes=True,
     graph_attrs=None,
     node_attrs=None,
```

### Comparing `nutree-0.4.0/nutree/fs.py` & `nutree-0.5.0/nutree/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Methods and classes to support file system related functionality.
 """
 from operator import attrgetter, itemgetter
 from pathlib import Path
```

### Comparing `nutree-0.4.0/nutree/node.py` & `nutree-0.5.0/nutree/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Declare the :class:`~nutree.node.Node` class.
 """
+from __future__ import annotations
+
 import re
 from operator import attrgetter
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Union
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .tree import Tree
 
@@ -60,24 +61,24 @@
     # DEFAULT_NAME_REPR = "{node.data!r}"
     # # DEFAULT_NAME_REPR = "{node.data}"
 
     def __init__(
         self,
         data,
         *,
-        parent: "Node",
+        parent: Node,
         data_id: Optional[ItemIdType] = None,
         node_id: Optional[int] = None,
         meta: Dict = None,
     ):
         self._data = data
         self._parent: Node = parent
 
         tree = parent._tree
-        self._tree: "Tree" = tree
+        self._tree: Tree = tree
         self._children: List[Node] = None
 
         if data_id is None:
             self._data_id: ItemIdType = tree._calc_data_id(data)
         else:
             self._data_id: ItemIdType = data_id
 
@@ -128,38 +129,40 @@
 
     @property
     def path(self) -> str:
         """All ancestor names including self, starting with and separated by '/'."""
         return self.get_path(repr="{node.name}")
 
     @property
-    def tree(self) -> "Tree":
+    def tree(self) -> Tree:
         """Return container :class:`~nutree.tree.Tree` instance."""
         return self._tree
 
     @property
-    def parent(self) -> "Node":
+    def parent(self) -> Node:
         """Return parent node or None for toplevel nodes."""
         p = self._parent
         return p if p._parent else None
 
     @property
-    def children(self) -> List["Node"]:
+    def children(self) -> List[Node]:
         """Return list of direct child nodes (list may be empty)."""
         c = self._children
         return [] if c is None else c
 
     @property
     def data(self) -> Any:
-        """Return the wrapped data instance (use :meth:`~nutree.tree.Tree.set_data()` to modify)."""
+        """Return the wrapped data instance (use :meth:`~nutree.tree.Tree.set_data()`
+        to modify)."""
         return self._data
 
     @property
     def data_id(self) -> ItemIdType:
-        """Return the wrapped data instance's id (use :meth:`~nutree.tree.Tree.set_data()` to modify)."""
+        """Return the wrapped data instance's id
+        (use :meth:`~nutree.tree.Tree.set_data()` to modify)."""
         return self._data_id
 
     @property
     def node_id(self) -> int:
         """Return the node's unique key."""
         return self._node_id
 
@@ -284,55 +287,55 @@
                 for n in cur_nodes:
                     n._data = data
             else:
                 self._data = new_data
 
         return
 
-    def get_children(self) -> List["Node"]:
+    def get_children(self) -> List[Node]:
         """Return list of direct child nodes (list may be empty)."""
         return self.children
 
-    def first_child(self) -> Union["Node", None]:
+    def first_child(self) -> Union[Node, None]:
         """First direct childnode or None if no children exist."""
         return self._children[0] if self._children else None
 
-    def last_child(self) -> Union["Node", None]:
+    def last_child(self) -> Union[Node, None]:
         """Last direct childnode or None if no children exist."""
         return self._children[-1] if self._children else None
 
-    def get_siblings(self, *, add_self=False) -> List["Node"]:
+    def get_siblings(self, *, add_self=False) -> List[Node]:
         """Return a list of all sibling entries of self (excluding self) if any."""
         if add_self:
             return self._parent._children
         return [n for n in self._parent._children if n is not self]
 
-    def first_sibling(self) -> "Node":
+    def first_sibling(self) -> Node:
         """Return first sibling (may be self)."""
         return self._parent._children[0]
 
-    def prev_sibling(self) -> Union["Node", None]:
+    def prev_sibling(self) -> Union[Node, None]:
         """Predecessor or None, if node is first sibling."""
         if self.is_first_sibling():
             return None
         idx = self._parent._children.index(self)
         return self._parent._children[idx - 1]
 
-    def next_sibling(self) -> Union["Node", None]:
+    def next_sibling(self) -> Union[Node, None]:
         """Return successor or None, if node is last sibling."""
         if self.is_last_sibling():
             return None
         idx = self._parent._children.index(self)
         return self._parent._children[idx + 1]
 
-    def last_sibling(self) -> "Node":
+    def last_sibling(self) -> Node:
         """Return last node, that share own parent (may be `self`)."""
         return self._parent._children[-1]
 
-    def get_clones(self, *, add_self=False) -> List["Node"]:
+    def get_clones(self, *, add_self=False) -> List[Node]:
         """Return a list of all nodes that reference the same data if any."""
         clones = self._tree._nodes_by_data_id[self._data_id]
         if add_self:
             return clones.copy()
         return [n for n in clones if n is not self]
 
     def depth(self) -> int:
@@ -376,15 +379,16 @@
     def get_index(self) -> int:
         """Return index in sibling list."""
         return self._parent._children.index(self)
 
     # --------------------------------------------------------------------------
 
     def is_system_root(self) -> bool:
-        """Return true if this node is the invisible system root :class:`~nutree.tree._SystemRootNode`."""
+        """Return true if this node is the invisible system root
+        :class:`~nutree.tree._SystemRootNode`."""
         return self._parent is None
 
     def is_top(self) -> bool:
         """Return true if this node has no parent."""
         return self._parent._parent is None
 
     def is_leaf(self) -> bool:
@@ -392,57 +396,59 @@
         return not self._children
 
     def is_clone(self) -> bool:
         """Return true if this node's data is referenced at least one more time."""
         return bool(len(self._tree._nodes_by_data_id.get(self._data_id)) > 1)
 
     def is_first_sibling(self) -> bool:
-        """Return true if this node is the first sibling, i.e. the first child of its parent."""
+        """Return true if this node is the first sibling, i.e. the first child
+        of its parent."""
         return self is self._parent._children[0]
 
     def is_last_sibling(self) -> bool:
-        """Return true if this node is the last sibling, i.e. the last child of its parent."""
+        """Return true if this node is the last sibling, i.e. the last child
+        of its parent."""
         return self is self._parent._children[-1]
 
     def has_children(self) -> bool:
         """Return true if this node has one or more children."""
         return bool(self._children)
 
-    def get_top(self) -> "Node":
+    def get_top(self) -> Node:
         """Return toplevel ancestor (may be self)."""
         root = self
         while root._parent._parent:
             root = root._parent
         return root
 
-    def is_descendant_of(self, other: "Node") -> bool:
+    def is_descendant_of(self, other: Node) -> bool:
         """Return true if this node is direct or indirect child of `other`."""
         parent = self._parent
         while parent is not None and parent._parent is not None:
             if parent is other:
                 return True
             parent = parent._parent
         return False
 
-    def is_ancestor_of(self, other: "Node") -> bool:
+    def is_ancestor_of(self, other: Node) -> bool:
         """Return true if this node is a parent, grandparent, ... of `other`."""
         return other.is_descendant_of(self)
 
-    def get_common_ancestor(self, other: "Node") -> Union["Node", None]:
+    def get_common_ancestor(self, other: Node) -> Union[Node, None]:
         """Return the nearest node that contains `self` and `other` (may be None)."""
         if self._tree is other._tree:
             other_parent_set = {
                 n._node_id for n in other.get_parent_list(add_self=True)
             }
             for parent in self.get_parent_list(add_self=True, bottom_up=True):
                 if parent._node_id in other_parent_set:
                     return parent
         return None
 
-    def get_parent_list(self, *, add_self=False, bottom_up=False) -> List["Node"]:
+    def get_parent_list(self, *, add_self=False, bottom_up=False) -> List[Node]:
         """Return ordered list of all parent nodes."""
         res = []
         parent = self if add_self else self._parent
         while parent is not None and parent._parent is not None:
             res.append(parent)
             parent = parent._parent
         if not bottom_up:
@@ -454,21 +460,21 @@
         res = (repr.format(node=p) for p in self.get_parent_list(add_self=add_self))
         return separator + separator.join(res)
 
     # --------------------------------------------------------------------------
 
     def add_child(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
-        before: Union["Node", bool, int, None] = None,
+        before: Union[Node, bool, int, None] = None,
         deep: bool = None,
         data_id=None,
         node_id=None,
-    ) -> "Node":
+    ) -> Node:
         """Append or insert a new subnode or branch as child.
 
         If `child` is an existing :class:`~nutree.node.Node` instance, a copy
         of this node will be created, that references the same `child.data`
         object. |br|
         If `deep` is true, the children are copied recursively.
 
@@ -494,15 +500,16 @@
         Args:
             child (Node|Tree|Any):
                 Either an existing Node or a data object.
             before (bool|int|Node|None):
                 Optional position.
             deep (bool):
                 Copy descendants if any.
-                This argument defaults to false  when `child` is a :class:`~nutree.node.Node`.
+                This argument defaults to false  when `child` is a
+                :class:`~nutree.node.Node`.
                 It defaults to true  when `child` is a :class:`~nutree.tree.Tree`.
             data_id (str|int|None):
                 Allow to override the new node's `data_id`.
                 This argument is only allowed for single nodes, but not for
                 deep copies.
                 Default `None` will to calculate from ``hash(node.data)``.
             node_id (str|int|None):
@@ -536,15 +543,19 @@
                         f"Same parent not allowed: {source_node}"
                     )
             else:
                 pass
                 # raise NotImplementedError("Cross-tree adding")
             if data_id and data_id != source_node._data_id:
                 raise UniqueConstraintError(f"data_id conflict: {source_node}")
-            node = factory(
+
+            # If creating an inherited node, use the parent class as constructor
+            child_class = child.__class__
+
+            node = child_class(
                 source_node.data, parent=self, data_id=data_id, node_id=node_id
             )
         else:
             node = factory(child, parent=self, data_id=data_id, node_id=node_id)
 
         children = self._children
         if children is None:
@@ -571,15 +582,15 @@
         return node
 
     #: Alias for :meth:`add_child`
     add = add_child
 
     def append_child(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
     ):
         """Append a new subnode.
 
@@ -587,15 +598,15 @@
         """
         return self.add_child(
             child, before=None, deep=deep, data_id=data_id, node_id=node_id
         )
 
     def prepend_child(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
     ):
         """Prepend a new subnode.
 
@@ -607,52 +618,56 @@
             deep=deep,
             data_id=data_id,
             node_id=node_id,
         )
 
     def prepend_sibling(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
-    ) -> "Node":
+    ) -> Node:
         """Add a new node before `self`.
 
         This method calls :meth:`add_child` on ``self.parent``.
         """
         return self._parent.add_child(
             child, before=self, deep=deep, data_id=data_id, node_id=node_id
         )
 
     def append_sibling(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
-    ) -> "Node":
+    ) -> Node:
         """Add a new node after `self`.
 
         This method calls :meth:`add_child` on ``self.parent``.
         """
         next_node = self.next_sibling()
         return self._parent.add_child(
             child, before=next_node, deep=deep, data_id=data_id, node_id=node_id
         )
 
     def move_to(
         self,
-        new_parent: Union["Node", "Tree"],
+        new_parent: Union[Node, Tree],
         *,
-        before: Union["Node", bool, int, None] = None,
+        before: Union[Node, bool, int, None] = None,
     ):
-        """Move this node before or after `otherNode`."""
+        """Move this node to another parent.
+
+        By default, the node is appended to existing children.
+        See :meth:`add_child` for a description of `before`.
+        """
         if new_parent is None:
             new_parent = self._tree._root
         # elif isinstance(new_parent, Tree):
         #     new_parent = new_parent._root
         elif hasattr(new_parent, "_root"):  # it's a Tree
             new_parent = new_parent._root
 
@@ -707,49 +722,58 @@
         """Remove all children of this node, making it a leaf node."""
         _unregister = self._tree._unregister
         for n in self._iter_post():
             _unregister(n)
         self._children = None
         return
 
-    def copy(self, *, add_self=True, predicate: PredicateCallbackType = None) -> "Tree":
+    def copy(self, *, add_self=True, predicate: PredicateCallbackType = None) -> Tree:
         """Return a new :class:`~nutree.tree.Tree` instance from this branch.
 
-        See also :meth:`_add_from` and :ref:`iteration callbacks`.
+        See also :ref:`iteration callbacks`.
         """
         new_tree = self._tree.__class__()
         if add_self:
             root = new_tree.add(self)
         else:
             root = new_tree._root
         root._add_from(self, predicate=predicate)
         return new_tree
 
     def copy_to(
         self,
-        target: Union["Node", "Tree"],
+        target: Union[Node, Tree],
         *,
         add_self=True,
-        before: Union["Node", bool, int, None] = None,
+        before: Union[Node, bool, int, None] = None,
         deep: bool = False,
-    ) -> None:
-        """Return a new :class:`~nutree.tree.Tree` instance from this branch.
+    ) -> Node:
+        """Copy this node to another parent and return the new node.
+
+        If `add_self` is set, a copy of this node becomes a child of `target`.
+        Otherwise copies of all children of this node are created below `target`.
 
-        See also :meth:`_add_from` and :ref:`iteration callbacks`.
+        By default new nodes are appended to existing children. The `before`
+        argument defines an alternative positioning.
+        It is only available when `add_self` is true.
+        See :meth:`add_child` for a description of `before`.
+
+        If `deep` is set, all descendants are copied recursively.
         """
         if add_self:
-            target.add_child(self, before=before, deep=deep)
-        else:
-            assert before is None
-            for child in self.children:
-                target.add_child(child, before=None, deep=deep)
-        return
+            return target.add_child(self, before=before, deep=deep)
+        assert before is None
+        res = None
+        for child in self.children:
+            n = target.add_child(child, before=None, deep=deep)
+            res = res or n  # Return the first new node
+        return res
 
     def _add_from(
-        self, other: "Node", *, predicate: PredicateCallbackType = None
+        self, other: Node, *, predicate: PredicateCallbackType = None
     ) -> None:
         """Append copies of all source descendants to self.
 
         See also :ref:`iteration callbacks`.
         """
         if predicate:
             return self._add_filtered(other, predicate)
@@ -758,15 +782,15 @@
         for child in other.children:
             new_child = self.add_child(child.data, data_id=child._data_id)
             if child.children:
                 # if child.has_children():
                 new_child._add_from(child, predicate=None)
         return
 
-    def _add_filtered(self, other: "Node", predicate: PredicateCallbackType) -> None:
+    def _add_filtered(self, other: Node, predicate: PredicateCallbackType) -> None:
         """Append a filtered copy of `other` and its descendants as children.
 
         See also :ref:`iteration callbacks`.
         """
         # Stack of parent node objects 2-tuples (is_existing, node), used to
         # create optional parents on demand.
         # If existing, `node` references this tree. Otherwise, `node` references
@@ -817,15 +841,15 @@
 
         try:
             _visit(other)
         except StopTraversal:
             pass
         return
 
-    def filtered(self, predicate: PredicateCallbackType) -> "Tree":
+    def filtered(self, predicate: PredicateCallbackType) -> Tree:
         """Return a filtered copy of this node and descendants as tree.
 
         See also :ref:`iteration callbacks`.
         """
         return self.copy(add_self=True, predicate=predicate)
 
     def filter(self, predicate: PredicateCallbackType) -> None:
@@ -1017,15 +1041,15 @@
                 if c._children:
                     next_level.extend(c._children)
             children = next_level
         return
 
     def iterator(
         self, method=IterMethod.PRE_ORDER, *, add_self=False
-    ) -> Generator["Node", None, None]:
+    ) -> Generator[Node, None, None]:
         """Generator that walks the hierarchy."""
         try:
             handler = getattr(self, f"_iter_{method.value}")
         except AttributeError:
             raise NotImplementedError(f"Unsupported traversal method {method!r}.")
 
         if add_self and method != IterMethod.POST_ORDER:
@@ -1040,20 +1064,20 @@
     __iter__ = iterator
 
     def _search(self, match, *, max_results=None, add_self=False):
         if callable(match):
             cb_match = match
         elif type(match) is str:
             pattern = re.compile(pattern=match)
-            cb_match = lambda node: pattern.fullmatch(node.name)
+            cb_match = lambda node: pattern.fullmatch(node.name)  # noqa: E731
         elif isinstance(match, (list, tuple)):
             pattern = re.compile(pattern=match[0], flags=match[1])
-            cb_match = lambda node: pattern.fullmatch(node.name)
+            cb_match = lambda node: pattern.fullmatch(node.name)  # noqa: E731
         else:
-            cb_match = lambda node: node._data is match
+            cb_match = lambda node: node._data is match  # noqa: E731
 
         count = 0
         for node in self.iterator(add_self=add_self):
             if not cb_match(node):
                 continue
             count += 1
             yield node
@@ -1208,83 +1232,98 @@
         return join.join(iter_lines)
 
     def to_dict(self, *, mapper: MapperCallbackType = None) -> Dict:
         """Return a nested dict of this node and its children."""
         res = {
             "data": str(self.data),
         }
-        # Add custom data_id if any
-        # data_id = hash(self._data)
-        data_id = self._tree._calc_data_id(self._data)
-        if data_id != self._data_id:
-            res["data_id"] = data_id
+        # Add custom data_id if not calculated to the hash by default.
+        if self._data_id != hash(self._data):
+            res["data_id"] = self._data_id
         res = call_mapper(mapper, self, res)
         # if mapper:
         #     res = mapper(self, res)
         if self._children:
             res["children"] = cl = []
             for n in self._children:
                 cl.append(n.to_dict(mapper=mapper))
         return res
 
+    @classmethod
+    def _make_list_entry(cls, node: Node) -> dict:
+        node_data = node._data
+        is_custom_id = node._data_id != hash(node_data)
+
+        # If data is more complex than a simple string, or if we use a custom
+        # data_id, we store data as a dict instead of a str:
+        if type(node_data) is str:
+            if not is_custom_id:
+                # Special case: node.data is a plain string without custom ID
+                return node_data
+            data = {
+                "str": node_data,
+            }
+        else:
+            # data is stored as-is, i.e. plain string instead of dict
+            data = {
+                # "id": data_id,
+            }
+        # Add custom data_id if not calculated as hash by default.
+        if node._data_id != hash(node_data):
+            data["data_id"] = node._data_id
+        return data
+
     def to_list_iter(
         self, *, mapper: MapperCallbackType = None
     ) -> Generator[Dict, None, None]:
         """Yield children as parent-referencing list.
 
         ```py
         [(parent_key, data)]
         ```
         """
         calc_id = self._tree._calc_data_id
         #: For nodes with multiple occurrences: index of the first one
-        clone_idx_map = {}
+        #: For typed nodes, we must also check if the `kind` matches, before
+        #: simply store a reference.
+        clone_idx_and_kind_map = {}
         parent_id_map = {self._node_id: 0}
 
         for id_gen, node in enumerate(self, 1):
             # Compact mode: use integer sequence as keys
             # Store idx with original id for later parent-ref. We only have to
             # do this for nodes that have children though:
             node_id = node._node_id
             if node._children:
                 parent_id_map[node_id] = id_gen
 
             parent_id = node._parent._node_id
             parent_idx = parent_id_map[parent_id]
 
-            data = node._data
-            data_id = calc_id(data)
-            # data_id = hash(data)
+            node_data = node._data
+            data_id = calc_id(node_data)
 
             # If node is a 2nd occurence of a clone, only store the index of the
             # first occurence and do not call the mapper
-            clone_idx = clone_idx_map.get(data_id)
+            node_kind = getattr(node, "kind", None)
+            clone_idx, clone_kind = clone_idx_and_kind_map.get(data_id, (None, None))
             if clone_idx:
-                yield (parent_idx, clone_idx)
-                continue
+                if node_kind == clone_kind:
+                    yield (parent_idx, clone_idx)
+                    continue
             elif node.is_clone():
-                clone_idx_map[data_id] = id_gen
+                # First instance of a clone node: take a note
+                clone_idx_and_kind_map[data_id] = (id_gen, node_kind)
+
+            # If node.data is more complex than a simple string, or if we use a
+            # custom data_id, we store data as a dict instead of a str:
+            data = self._make_list_entry(node)
 
-            # If data is more complex than a simple string, or if we use a custom
-            # data_id, we store data as a dict instead of a str:
-            if type(data) is str:
-                if data_id != node._data_id:
-                    data = {
-                        "str": data,
-                        "id": data_id,
-                    }
-                # else: data is stored as-is, i.e. plain string instead of dict
-            else:
-                data = {
-                    # "id": data_id,
-                }
             # Let caller serialize custom data objects
             data = call_mapper(mapper, node, data)
-            # if mapper:
-            #     data = mapper(node, data)
 
             yield (parent_idx, data)
         return
 
     def to_dot(
         self,
         *,
```

### Comparing `nutree-0.4.0/nutree/rdf.py` & `nutree-0.5.0/nutree/rdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Functions and declarations to implement `rdflib <https://github.com/RDFLib/rdflib>`_.
 """
+from __future__ import annotations
+
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 from nutree.common import IterationControl
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .node import Node
 
     # from .tree import Tree
     from .typed_tree import TypedNode, TypedTree
 
 # Export some common rdflib attributes, so they can be accessed as
-# `from nutree.rdf import Literal` for example.
-# witout having to `import rdflib`, ehich may be not available:
+# `from nutree.rdf import Literal` without having to `import rdflib`
+# (which may not be available):
 try:
     import rdflib
     from rdflib import Graph, IdentifiedNode, Literal, URIRef
     from rdflib.namespace import RDF, XSD, DefinedNamespace, Namespace
 except ImportError:
     rdflib = None
     Graph = IdentifiedNode = Literal = URIRef = None
@@ -60,15 +61,15 @@
     graph.bind("rdf", RDF)
     return graph
 
 
 def _add_child_node(
     graph: Graph,
     parent_graph_node: Optional[IdentifiedNode],
-    tree_node: "TypedNode",
+    tree_node: TypedNode,
     index: int,
     node_mapper: RDFMapperCallbackType,
 ) -> Union[IdentifiedNode, IterationControl, bool]:
     """"""
     graph_node = Literal(tree_node.data_id)
 
     # Mapper can call `graph.add()`
@@ -101,15 +102,15 @@
 
     return graph_node
 
 
 def _add_child_nodes(
     graph: Graph,
     graph_node: IdentifiedNode,
-    tree_node: "TypedNode",
+    tree_node: TypedNode,
     node_mapper: RDFMapperCallbackType = None,
 ) -> None:
     """"""
     for index, child_tree_node in enumerate(tree_node._children or ()):
         cgn = _add_child_node(
             graph,
             parent_graph_node=graph_node,
@@ -120,15 +121,15 @@
         if child_tree_node.has_children:
             _add_child_nodes(graph, cgn, child_tree_node, node_mapper)
 
     return
 
 
 def node_to_rdf(
-    tree_node: "TypedNode",
+    tree_node: TypedNode,
     *,
     add_self: bool = True,
     node_mapper: RDFMapperCallbackType = None,
 ) -> Graph:
     """Generate DOT formatted output line-by-line."""
     graph = _make_graph()
 
@@ -150,15 +151,15 @@
         node_mapper=node_mapper,
     )
 
     return graph
 
 
 def tree_to_rdf(
-    tree: "TypedTree",
+    tree: TypedTree,
     *,
     node_mapper: RDFMapperCallbackType = None,
 ) -> Graph:
     graph = _make_graph()
 
     root_graph_node = URIRef(NUTREE_NS.system_root)
     graph.add((root_graph_node, NUTREE_NS.name, Literal(tree.name)))
```

### Comparing `nutree-0.4.0/nutree/tree.py` & `nutree-0.5.0/nutree/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Declare the :class:`~nutree.tree.Tree` class.
 """
+from __future__ import annotations
+
 import json
 import random
 import threading
 from pathlib import PurePath
 from typing import IO, Any, Dict, Generator, List, Union
 
 from nutree.diff import diff_tree
 
 from .common import (
+    FILE_FORMAT_VERSION,
+    ROOT_ID,
     AmbiguousMatchError,
     ItemIdType,
     IterMethod,
     MapperCallbackType,
     PredicateCallbackType,
     TraversalCallbackType,
     call_mapper,
@@ -71,15 +74,15 @@
     def __exit__(self, type, value, traceback):
         self._lock.release()
         return
 
     def __eq__(self, other) -> bool:
         raise NotImplementedError("Use `is` or `tree.compare()` instead.")
 
-    def __getitem__(self, data: object) -> "Node":
+    def __getitem__(self, data: object) -> Node:
         """Implement ``tree[data]`` syntax to lookup a node.
 
         `data` may be a plain string, data object, data_id, or node_id.
 
         Note: This is a flexible and concise way to access tree nodes. However,
         :meth:`find_all` or :meth:`find_first` may be faster.
 
@@ -112,15 +115,16 @@
         return res[0]
 
     # def __iadd__(self, other) -> None:
     #     """Support `tree += node(s)` syntax"""
     #     self._root += other
 
     def __len__(self):
-        """Make ``len(tree)`` return the number of nodes (also makes empty trees falsy)."""
+        """Make ``len(tree)`` return the number of nodes
+        (also makes empty trees falsy)."""
         return self.count
 
     def _calc_data_id(self, data) -> ItemIdType:
         """Called internally to calculate `data_id` for a `data` object.
 
         This value is used to lookup nodes by data, identify clones, and for
         (de)serialization. It defaults to ``hash(data)`` but may be overloaded
@@ -131,15 +135,15 @@
         within an individual Python process, they are not predictable between
         repeated invocations of Python.
         """
         if self._calc_data_id_hook:
             return self._calc_data_id_hook(self, data)
         return hash(data)
 
-    def _register(self, node: "Node"):
+    def _register(self, node: Node):
         assert node._tree is self
         # node._tree = self
         assert node._node_id and node._node_id not in self._node_by_id, f"{node}"
         self._node_by_id[node._node_id] = node
         try:
             self._nodes_by_data_id[node._data_id].append(node)
         except KeyError:
@@ -169,16 +173,17 @@
             node._data_id = None
             node._node_id = None
             node._children = None
             node._meta = None
         return
 
     @property
-    def children(self) -> List["Node"]:
-        """Return list of direct child nodes, i.e. toplevel nodes (list may be empty)."""
+    def children(self) -> List[Node]:
+        """Return list of direct child nodes, i.e. toplevel nodes
+        (list may be empty)."""
         return self._root.children
 
     @property
     def count(self):
         """Return the total number of nodes."""
         return len(self._node_by_id)
 
@@ -258,21 +263,21 @@
 
     def print(self, *, repr=None, style=None, title=None, join="\n"):
         """Convenience method that simply runs print(self. :meth:`format()`)."""
         print(self.format(repr=repr, style=style, title=title, join=join))
 
     def add_child(
         self,
-        child: Union["Node", "Tree", Any],
+        child: Union[Node, Tree, Any],
         *,
-        before: Union["Node", bool, int, None] = None,
+        before: Union[Node, bool, int, None] = None,
         deep: bool = None,
         data_id=None,
         node_id=None,
-    ) -> "Node":
+    ) -> Node:
         """Add a toplevel node.
 
         See Node's :meth:`~nutree.node.Node.add_child` method for details.
         """
         return self._root.add_child(
             child,
             before=before,
@@ -282,15 +287,15 @@
         )
 
     #: Alias for :meth:`add_child`
     add = add_child
 
     def copy(
         self, *, name: str = None, predicate: PredicateCallbackType = None
-    ) -> "Tree":
+    ) -> Tree:
         """Return a copy of this tree.
 
         New :class:`Tree` and :class:`Node` instances are created.
         The new nodes reference the original data objects.
 
         `predicate` may be passed to filter the result, which is equivalent to
         calling :meth:`~nutree.tree.Tree.filtered`
@@ -301,43 +306,43 @@
         if name is None:
             name = f"Copy of {self}"
         new_tree = Tree(name)
         with self:
             new_tree._root._add_from(self._root, predicate=predicate)
         return new_tree
 
-    def copy_to(self, target: Union[Node, "Tree"], *, deep=True) -> Node:
+    def copy_to(self, target: Union[Node, Tree], *, deep=True) -> None:
         """Copy this tree's nodes to another target.
 
         See Node's :meth:`~nutree.node.Node.copy_to` method for details.
         """
         with self:
-            return self._root.copy_to(target, add_self=False, before=None, deep=deep)
+            self._root.copy_to(target, add_self=False, before=None, deep=deep)
 
     def filter(self, predicate: PredicateCallbackType) -> None:
         """In-place removal of unmatching nodes.
 
         See also :ref:`iteration callbacks`.
         """
         self._root.filter(predicate=predicate)
 
-    def filtered(self, predicate: PredicateCallbackType) -> "Tree":
+    def filtered(self, predicate: PredicateCallbackType) -> Tree:
         """Return a filtered copy of this tree.
 
         See also :ref:`iteration callbacks`.
         """
         return self.copy(predicate=predicate)
 
     def clear(self) -> None:
         """Remove all nodes from this tree."""
         self._root.remove_children()
 
     def find_all(
         self, data=None, *, match=None, data_id=None, max_results: int = None
-    ) -> List["Node"]:
+    ) -> List[Node]:
         """Return a list of matching nodes (list may be empty).
 
         See also Node's :meth:`~nutree.node.Node.find_all` method and
         :ref:`iteration callbacks`.
         """
         if data is not None:
             assert data_id is None
@@ -353,15 +358,15 @@
         elif match is not None:
             return self._root.find_all(match=match, max_results=max_results)
 
         raise NotImplementedError
 
     def find_first(
         self, data=None, *, match=None, data_id=None, node_id=None
-    ) -> Union["Node", None]:
+    ) -> Union[Node, None]:
         """Return the one matching node or `None`.
 
         Note that 'first' sometimes means 'one arbitrary' matching node, which
         is not neccessarily the first of a specific iteration method.
         See also Node's :meth:`~nutree.node.Node.find_first` method and
         :ref:`iteration callbacks`.
         """
@@ -398,15 +403,15 @@
         res = []
         with self:
             for n in self._root._children:
                 res.append(n.to_dict(mapper=mapper))
         return res
 
     @classmethod
-    def from_dict(cls, obj: List[Dict], *, mapper=None) -> "Tree":
+    def from_dict(cls, obj: List[Dict], *, mapper=None) -> Tree:
         """Return a new :class:`Tree` instance from a list of dicts.
 
         See also :meth:`~nutree.tree.Tree.to_dict` and
         Node's :meth:`~nutree.node.Node.find_first` methods, and
         :ref:`iteration callbacks`.
         """
         new_tree = Tree()
@@ -415,58 +420,76 @@
 
     def to_list_iter(
         self, *, mapper: MapperCallbackType = None
     ) -> Generator[Dict, None, None]:
         """Yield a parent-referencing list of child nodes."""
         return self._root.to_list_iter(mapper=mapper)
 
-    def save(self, fp: IO[str], *, mapper: MapperCallbackType = None) -> None:
+    def save(
+        self, fp: IO[str], *, mapper: MapperCallbackType = None, meta: dict = None
+    ) -> None:
         """Store tree in a compact JSON file stream.
 
         See also :meth:`to_list_iter` and :meth:`load` methods.
         """
+        header = {
+            "$version": FILE_FORMAT_VERSION,
+            # "$nutree_version": __version__,
+        }
+        if meta:
+            header.update(meta)
         with self:
-            iter = self.to_list_iter(mapper=mapper)
-            # Materialize so we can lock the snapshot.
-            # Also because json.dump() does not supprt streaming
+            # Materialize node list, so we can lock the snapshot.
+            # Also because json.dump() does not support streaming anyway.
             # TODO: Use s.th. like https://github.com/daggaz/json-stream ?
-            json.dump(list(iter), fp)
+            res = {
+                "meta": header,
+                "nodes": list(self.to_list_iter(mapper=mapper)),
+            }
+        json.dump(res, fp)
         return
 
     @classmethod
-    def _from_list(cls, obj: List[Dict], *, mapper=None) -> "Tree":
-        tree = Tree()
+    def _from_list(cls, obj: List[Dict], *, mapper=None) -> Tree:
+        tree = cls()  # Tree or TypedTree
         node_idx_map = {0: tree._root}
         for idx, (parent_idx, data) in enumerate(obj, 1):
             parent = node_idx_map[parent_idx]
             # print(idx, parent_idx, data, parent)
             if type(data) is str:
                 n = parent.add(data)
             elif type(data) is int:
                 first_clone = node_idx_map[data]
                 n = parent.add(first_clone)
             elif mapper:
                 data = call_mapper(mapper, parent, data)
-                # data = mapper(parent, data)
                 n = parent.add(data)
             else:
-                raise RuntimeError("Need mapper")  # pragma: no cover
+                raise RuntimeError(f"Need mapper for {data}")  # pragma: no cover
 
             node_idx_map[idx] = n
 
         return tree
 
     @classmethod
-    def load(cls, fp: IO[str], *, mapper=None) -> "Tree":
+    def load(cls, fp: IO[str], *, mapper=None, file_meta: dict = None) -> Tree:
         """Create a new :class:`Tree` instance from a JSON file stream.
 
+        If ``file_meta`` is a dict, it receives the content if the file's
+        ``meta`` header.
+
         See also :meth:`save`.
         """
         obj = json.load(fp)
-        return cls._from_list(obj, mapper=mapper)
+        if not isinstance(obj, dict) or "meta" not in obj or "nodes" not in obj:
+            raise RuntimeError("Invalid file format")
+        if isinstance(file_meta, dict):
+            file_meta.update(obj["meta"])
+        nodes = obj["nodes"]
+        return cls._from_list(nodes, mapper=mapper)
 
     def to_dot(
         self,
         *,
         add_root=True,
         unique_nodes=True,
         graph_attrs=None,
@@ -527,15 +550,15 @@
     def to_rdf_graph(self):
         """Return an instance of ``rdflib.Graph``.
 
         See :ref:`Graphs` for details.
         """
         return tree_to_rdf(self)
 
-    def diff(self, other: "Tree", *, ordered=False, reduce=False) -> "Tree":
+    def diff(self, other: Tree, *, ordered=False, reduce=False) -> Tree:
         """Compare this tree against `other` and return a merged, annotated copy.
 
         The resulting tree contains a union of all nodes from this and the
         other tree.
         Additional metadata is added to the resulting nodes to classify changes
         from the perspective of this tree. For example a node that only exists
         in `other`, will have ``node.get_meta("dc") == DiffClassification.ADDED``
@@ -586,14 +609,13 @@
 # ------------------------------------------------------------------------------
 # - _SystemRootNode
 # ------------------------------------------------------------------------------
 class _SystemRootNode(Node):
     """Invisible system root node."""
 
     def __init__(self, tree: Tree):
-
         self._tree: Tree = tree
         self._parent = None
-        self._node_id = self._data_id = "__root__"
+        self._node_id = self._data_id = ROOT_ID
         self._data = tree.name
         self._children = []
         self._meta = None
```

### Comparing `nutree-0.4.0/nutree/typed_tree.py` & `nutree-0.5.0/nutree/typed_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Declare the :class:`~nutree.tree.TypedTree` class.
 """
-from typing import Any, Dict, Generator, List, Union
+from __future__ import annotations
+
+from typing import IO, Any, Dict, Generator, List, Union
 
 from nutree.common import (
+    ROOT_ID,
     IterMethod,
     MapperCallbackType,
     PredicateCallbackType,
     UniqueConstraintError,
+    call_mapper,
 )
 
 from .node import Node
 from .tree import Tree
 
 
 class ANY_KIND:
@@ -43,15 +46,15 @@
     # DEFAULT_NAME_REPR = "{node.data!r}"
 
     def __init__(
         self,
         kind: str,
         data,
         *,
-        parent: "TypedNode",
+        parent: TypedNode,
         data_id=None,
         node_id=None,
         meta: Dict = None,
     ):
         super().__init__(
             data, parent=parent, data_id=data_id, node_id=node_id, meta=meta
         )
@@ -72,54 +75,54 @@
     #     return f"{self.data}"
 
     @property
     def kind(self) -> str:
         return self._kind
 
     @property
-    def parent(self) -> "TypedNode":
+    def parent(self) -> TypedNode:
         """Return parent node or None for toplevel nodes."""
         p = self._parent
         return p if p._parent else None
 
     @property
-    def children(self) -> List["TypedNode"]:
+    def children(self) -> List[TypedNode]:
         """Return list of direct child nodes (list may be empty)."""
         c = self._children
         return [] if c is None else c
 
-    def get_children(self, kind: Union[str, ANY_KIND]) -> List["TypedNode"]:
+    def get_children(self, kind: Union[str, ANY_KIND]) -> List[TypedNode]:
         """Return list of direct child nodes of a given type (list may be empty)."""
         all_children = self._children
         if not all_children:
             return []
         elif kind is ANY_KIND:
             return all_children
         return list(filter(lambda n: n._kind == kind, all_children))
 
     # def set_data(
     #     self, kind: str, data, *, data_id=None, with_clones: bool = None
     # ) -> None:
     #     """Change node's `data` and/or `data_id` and update bookkeeping."""
     #     super().set_data(data, data_id=data_id, with_clones=with_clones)
 
-    def first_child(self, kind: Union[str, ANY_KIND]) -> Union["TypedNode", None]:
+    def first_child(self, kind: Union[str, ANY_KIND]) -> Union[TypedNode, None]:
         """First direct childnode or None if no children exist."""
         all_children = self._children
         if not all_children:
             return None
         elif kind is ANY_KIND:
             return all_children[0]
 
         for n in all_children:
             if n._kind == kind:
                 return n
         return None
 
-    def last_child(self, kind: Union[str, ANY_KIND]) -> Union["TypedNode", None]:
+    def last_child(self, kind: Union[str, ANY_KIND]) -> Union[TypedNode, None]:
         """Last direct childnode or None if no children exist."""
         all_children = self._children
         if not all_children:
             return None
         elif kind is ANY_KIND:
             return all_children[-1]
 
@@ -131,67 +134,67 @@
 
     def has_children(self, kind: Union[str, ANY_KIND]) -> bool:
         """Return true if this node has one or more children."""
         if kind is ANY_KIND:
             return bool(self._children)
         return len(self.get_children(kind)) > 1
 
-    def get_siblings(self, *, add_self=False, any_kind=False) -> List["TypedNode"]:
+    def get_siblings(self, *, add_self=False, any_kind=False) -> List[TypedNode]:
         """Return a list of all sibling entries of self (excluding self) if any."""
         if any_kind:
             return super().get_siblings(add_self=add_self)
         children = self._parent._children
         rel = self.kind
         return [n for n in children if (add_self or n is not self) and n.kind == rel]
 
-    def first_sibling(self, *, any_kind=False) -> "TypedNode":
+    def first_sibling(self, *, any_kind=False) -> TypedNode:
         """Return first sibling `of the same kind` (may be self)."""
         pc = self._parent._children
         if any_kind:
             return pc[0]
         for n in pc:
             if n._kind == self._kind:
                 return n
         raise AssertionError("Internal error")
 
-    def last_sibling(self, *, any_kind=False) -> "TypedNode":
+    def last_sibling(self, *, any_kind=False) -> TypedNode:
         """Return last sibling `of the same kind` (may be self)."""
         pc = self._parent._children
         if any_kind:
             return pc[-1]
         for n in reversed(pc):
             if n._kind == self._kind:
                 return n
         raise AssertionError("Internal error")
 
-    def prev_sibling(self, *, any_kind=False) -> Union["TypedNode", None]:
+    def prev_sibling(self, *, any_kind=False) -> Union[TypedNode, None]:
         """Return predecessor `of the same kind` or None if node is first sibling."""
         pc = self._parent._children
         own_idx = pc.index(self)
         if own_idx > 0:
             for idx in range(own_idx - 1, -1, -1):
                 n = pc[idx]
                 if any_kind or n._kind == self._kind:
                     return n
         return None
 
-    def next_sibling(self, *, any_kind=False) -> Union["TypedNode", None]:
+    def next_sibling(self, *, any_kind=False) -> Union[TypedNode, None]:
         """Return successor `of the same kind` or None if node is last sibling."""
         pc = self._parent._children
         pc_len = len(pc)
         own_idx = pc.index(self)
 
         if own_idx < pc_len - 2:
             for idx in range(own_idx + 1, pc_len):
                 n = pc[idx]
                 if any_kind or n._kind == self._kind:
                     return n
         return None
 
-    # def get_clones(self, *, add_self=False) -> List["TypedNode"]:
+    # def get_clones(self, *, add_self=False) -> List[TypedNode]:
     #     """Return a list of all nodes that reference the same data if any."""
     #     clones = self._tree._nodes_by_data_id[self._data_id]
     #     if add_self:
     #         return clones.copy()
     #     return [n for n in clones if n is not self]
 
     def get_index(self, *, any_kind=False) -> int:
@@ -199,36 +202,37 @@
         if any_kind:
             kc = self._parent._children
         else:
             kc = self.parent.get_children(self.kind)
         return kc.index(self)
 
     def is_first_sibling(self, *, any_kind=False) -> bool:
-        """Return true if this node is the first sibling, i.e. the first child of its parent."""
+        """Return true if this node is the first sibling, i.e. the first child
+        of its parent."""
         if any_kind:
             return self is self._parent._children[0]
         return self is self.first_sibling(any_kind=False)
 
     def is_last_sibling(self, *, any_kind=False) -> bool:
         """Return true if this node is the last sibling, i.e. the last child
         **of this kind** of its parent."""
         if any_kind:
             return self is self._parent._children[-1]
         return self is self.last_sibling(any_kind=False)
 
     def add_child(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         kind: str = None,
-        before: Union["TypedNode", bool, int, None] = None,
+        before: Union[TypedNode, bool, int, None] = None,
         deep: bool = None,
         data_id=None,
         node_id=None,
-    ) -> "TypedNode":
+    ) -> TypedNode:
         """See ..."""
         # assert not isinstance(child, TypedNode) or child.kind == self.kind
         # TODO: kind is optional if child is a TypedNode
         # TODO: Check if target and child types match
         # TODO: share more code from overloaded method
         if kind is None:
             kind = DEFAULT_CHILD_TYPE
@@ -259,18 +263,21 @@
             if source_node._tree is self._tree:
                 if source_node._parent is self._parent:
                     raise UniqueConstraintError(
                         f"Same parent not allowed: {source_node}"
                     )
             else:
                 pass
-                # raise NotImplementedError("Cross-tree adding")
             if data_id and data_id != source_node._data_id:
                 raise UniqueConstraintError(f"data_id conflict: {source_node}")
-            node = factory(
+
+            # If creating an inherited node, use the parent class as constructor
+            child_class = child.__class__
+
+            node = child_class(
                 kind,
                 source_node.data,
                 parent=self,
                 data_id=data_id,
                 node_id=node_id,
             )
         else:
@@ -301,15 +308,15 @@
         return node
 
     #: Alias for :meth:`add_child`
     add = add_child
 
     def append_child(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         kind: str = None,
         deep=None,
         data_id=None,
         node_id=None,
     ):
         """Append a new subnode.
@@ -323,15 +330,15 @@
             deep=deep,
             data_id=data_id,
             node_id=node_id,
         )
 
     def prepend_child(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         kind: str = None,
         deep=None,
         data_id=None,
         node_id=None,
     ):
         """Prepend a new subnode.
@@ -345,52 +352,52 @@
             deep=deep,
             data_id=data_id,
             node_id=node_id,
         )
 
     def prepend_sibling(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
-    ) -> "TypedNode":
+    ) -> TypedNode:
         """Add a new node **of same kind** before `self`.
 
         This method calls :meth:`add_child` on ``self.parent``.
         """
         return self._parent.add_child(
             child, before=self, deep=deep, data_id=data_id, node_id=node_id
         )
 
     def append_sibling(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         deep=None,
         data_id=None,
         node_id=None,
-    ) -> "TypedNode":
+    ) -> TypedNode:
         """Add a new node **of same kind** after `self`.
 
         This method calls :meth:`add_child` on ``self.parent``.
         """
         next_node = self.next_sibling
         return self._parent.add_child(
             child, before=next_node, deep=deep, data_id=data_id, node_id=node_id
         )
 
     def move_to(
         self,
-        new_parent: Union["TypedNode", "TypedTree"],
+        new_parent: Union[TypedNode, TypedTree],
         *,
-        before: Union["TypedNode", bool, int, None] = None,
+        before: Union[TypedNode, bool, int, None] = None,
     ):
-        """Move this node before or after `otherNode` ."""
+        """Move this node before or after `new_parent`."""
         raise NotImplementedError
 
     # def remove(self, *, keep_children=False, with_clones=False) -> None:
     #     """Remove this node.
 
     #     If `keep_children` is true, all children will be moved one level up,
     #     so they become siblings, before this node is removed.
@@ -400,31 +407,31 @@
     #     """
     #     raise NotImplementedError
 
     # def remove_children(self, kind: Union[str, ANY_KIND]):
     #     """Remove all children of this node, making it a leaf node."""
     #     raise NotImplementedError
 
-    def copy(self, *, add_self=True, predicate=None) -> "TypedTree":
+    def copy(self, *, add_self=True, predicate=None) -> TypedTree:
         """Return a new :class:`~nutree.typed_tree.TypedTree` instance from this branch.
 
         See also :meth:`_add_from` and :ref:`iteration callbacks`.
         """
         return super().copy(add_self=add_self, predicate=predicate)
 
-    def filtered(self, predicate: PredicateCallbackType) -> "TypedTree":
+    def filtered(self, predicate: PredicateCallbackType) -> TypedTree:
         """Return a filtered copy of this node and descendants as tree.
 
         See also :ref:`iteration callbacks`.
         """
         return super().filtered(predicate=predicate)
 
     def iterator(
         self, method=IterMethod.PRE_ORDER, *, add_self=False
-    ) -> Generator["TypedNode", None, None]:
+    ) -> Generator[TypedNode, None, None]:
         """Generator that walks the hierarchy."""
         return super().iterator(method=method, add_self=add_self)
 
     #: Implement ``for subnode in node: ...`` syntax to iterate descendant nodes.
     __iter__ = iterator
 
     # def sort_children(self, *, key=None, reverse=False, deep=False):
@@ -468,15 +475,16 @@
 
     # def _render_lines(self, *, repr=None, style=None, add_self=True):
     #     if type(style) not in (list, tuple):
     #         try:
     #             style = CONNECTORS[style or self.tree.default_connector_style]
     #         except KeyError:
     #             raise ValueError(
-    #                 f"Invalid style '{style}'. Expected: {'|'.join(CONNECTORS.keys())}"
+    #                 f"Invalid style '{style}'. "
+    #                 f"Expected: {'|'.join(CONNECTORS.keys())}"
     #             )
 
     #     if repr is None:
     #         repr = DEFAULT_NAME_REPR
 
     #     # Find out if we need to strip some of the leftmost prefixes.
     #     # If this was called for a normal node, we strip all parent levels
@@ -516,72 +524,31 @@
     #     #     res = mapper(self, res)
     #     if self._children:
     #         res["children"] = cl = []
     #         for n in self._children:
     #             cl.append(n.to_dict(mapper=mapper))
     #     return res
 
-    # def to_list_iter(
-    #     self, *, mapper: MapperCallbackType = None
-    # ) -> Generator[Dict, None, None]:
-    #     """Yield children as parent-referencing list.
-
-    #     ```py
-    #     [(parent_key, data)]
-    #     ```
-    #     """
-    #     calc_id = self._tree._calc_data_id
-    #     #: For nodes with multiple occurrences: index of the first one
-    #     clone_idx_map = {}
-    #     parent_id_map = {self._node_id: 0}
-
-    #     for id_gen, node in enumerate(self, 1):
-    #         # Compact mode: use integer sequence as keys
-    #         # Store idx with original id for later parent-ref. We only have to
-    #         # do this of nodes that have children though:
-    #         node_id = node._node_id
-    #         if node._children:
-    #             parent_id_map[node_id] = id_gen
-
-    #         parent_id = node._parent._node_id
-    #         parent_idx = parent_id_map[parent_id]
-
-    #         data = node._data
-    #         data_id = calc_id(data)
-    #         # data_id = hash(data)
-
-    #         # If node is a 2nd occurence of a clone, only store the index of the
-    #         # first occurence and do not call the mapper
-    #         clone_idx = clone_idx_map.get(data_id)
-    #         if clone_idx:
-    #             yield (parent_idx, clone_idx)
-    #             continue
-    #         elif node.is_clone():
-    #             clone_idx_map[data_id] = id_gen
-
-    #         # If data is more complex than a simple string, or if we use a custom
-    #         # data_id, we store data as a dict instead of a str:
-    #         if type(data) is str:
-    #             if data_id != node._data_id:
-    #                 data = {
-    #                     "str": data,
-    #                     "id": data_id,
-    #                 }
-    #             # else: data is stored as-is, i.e. plain string instead of dict
-    #         else:
-    #             data = {
-    #                 # "id": data_id,
-    #             }
-    #         # Let caller serialize custom data objects
-    #         data = call_mapper(mapper, node, data)
-    #         # if mapper:
-    #         #     data = mapper(node, data)
+    @classmethod
+    def _make_list_entry(cls, node: TypedNode) -> dict:
+        node_data = node._data
+        # is_custom_id = node._data_id != hash(node_data)
+
+        if type(node_data) is str:
+            # Node._make_list_entry() would return a plain str, but we always
+            # need a dict
+            data = {
+                "str": node_data,
+            }
+        else:
+            data = Node._make_list_entry(node)
 
-    #         yield (parent_idx, data)
-    #     return
+        if node.kind != ANY_KIND:
+            data["kind"] = node.kind
+        return data
 
     def to_dot(
         self,
         *,
         add_self=False,
         unique_nodes=True,
         graph_attrs: dict = None,
@@ -625,27 +592,27 @@
 
     def __init__(self, name: str = None, *, factory=None, calc_data_id=None):
         if factory is None:
             factory = TypedNode
         super().__init__(name, factory=factory, calc_data_id=calc_data_id)
         self._root = _SystemRootTypedNode(self)
 
-    def __getitem__(self, data: object) -> "TypedNode":
+    def __getitem__(self, data: object) -> TypedNode:
         return super().__getitem__(data)
 
     def add_child(
         self,
-        child: Union["TypedNode", "TypedTree", Any],
+        child: Union[TypedNode, TypedTree, Any],
         *,
         kind: str = None,
-        before: Union["TypedNode", bool, int, None] = None,
+        before: Union[TypedNode, bool, int, None] = None,
         deep: bool = None,
         data_id=None,
         node_id=None,
-    ) -> "TypedNode":
+    ) -> TypedNode:
         """Add a toplevel node.
 
         See Node's :meth:`~nutree.node.Node.add_child` method for details.
         """
         return self._root.add_child(
             child,
             kind=kind,
@@ -654,33 +621,80 @@
             data_id=data_id,
             node_id=node_id,
         )
 
     #: Alias for :meth:`add_child`
     add = add_child  # Must re-bind here
 
+    def first_child(self, kind: Union[str, ANY_KIND]) -> Union[TypedNode, None]:
+        """Return the first toplevel node."""
+        return self._root.first_child(kind=kind)
+
+    def last_child(self, kind: Union[str, ANY_KIND]) -> Union[TypedNode, None]:
+        """Return the last toplevel node."""
+        return self._root.last_child(kind=kind)
+
     def iter_by_type(
         self, kind: Union[str, ANY_KIND]
     ) -> Generator[TypedNode, None, None]:
         if kind == ANY_KIND:
             return self.iterator()
         for n in self.iterator():
             if n._kind == kind:
                 yield n
         return
 
+    @classmethod
+    def _from_list(cls, obj: List[Dict], *, mapper=None) -> TypedTree:
+        tree = cls()
+        node_idx_map = {0: tree._root}
+        for idx, (parent_idx, data) in enumerate(obj, 1):
+            parent = node_idx_map[parent_idx]
+            # print(idx, parent_idx, data, parent)
+            if type(data) is str:
+                # this can only happen if the source was generate by a plain Tree
+                n = parent.add(data, kind=DEFAULT_CHILD_TYPE)
+            elif type(data) is int:
+                first_clone = node_idx_map[data]
+                n = parent.add(
+                    first_clone, kind=first_clone.kind, data_id=first_clone.data_id
+                )
+            elif mapper:
+                kind = data.get("kind", DEFAULT_CHILD_TYPE)
+                data_id = data.get("data_id")
+                data_obj = call_mapper(mapper, parent, data)
+                n = parent.add(data_obj, kind=kind, data_id=data_id)
+            elif isinstance(data, dict) and "str" in data:
+                # this can happen if the source was generate by without a
+                # serialization mapper, for a TypedTree that has str nodes
+                n = parent.add(data["str"], kind=data.get("kind"))
+            else:
+                raise RuntimeError(f"Need mapper for {data}")  # pragma: no cover
+
+            node_idx_map[idx] = n
+
+        return tree
+
+    @classmethod
+    def load(cls, fp: IO[str], *, mapper=None, file_meta: dict = None) -> TypedTree:
+        """Create a new :class:`TypedTree` instance from a JSON file stream.
+
+        See also Tree's :meth:`~nutree.tree.Tree.save()` and
+        :meth:`~nutree.tree.Tree.load()` methods.
+        """
+        return super().load(fp, mapper=mapper, file_meta=file_meta)
+
 
 # ------------------------------------------------------------------------------
 # - _SystemRootTypedNode
 # ------------------------------------------------------------------------------
 class _SystemRootTypedNode(TypedNode):
     """Invisible system root node."""
 
     def __init__(self, tree: TypedTree):
-
         self._tree: TypedTree = tree
         self._parent = None
-        self._node_id = self._data_id = "__root__"
+        self._node_id = self._data_id = ROOT_ID
         self._data = tree.name
         self._children = []
         self._meta = None
         self._kind = None
```

### Comparing `nutree-0.4.0/nutree.egg-info/PKG-INFO` & `nutree-0.5.0/nutree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutree
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for tree data structures with an intuitive, yet powerful, API.
 Home-page: https://github.com/mar10/nutree/
 Author: Martin Wendt
 Author-email: nutree@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: nutree@wwwendt.de
 License: MIT
@@ -17,37 +17,35 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+Provides-Extra: graph
 License-File: LICENSE.txt
 
 # ![logo](https://raw.githubusercontent.com/mar10/nutree/main/docs/nutree_48x48.png) nutree
 
-[![Build Status](https://travis-ci.com/mar10/nutree.svg?branch=main)](https://app.travis-ci.com/github/mar10/nutree)
+[![Tests](https://github.com/mar10/nutree/actions/workflows/tests.yml/badge.svg)](https://github.com/mar10/nutree/actions/workflows/tests.yml)
 [![Latest Version](https://img.shields.io/pypi/v/nutree.svg)](https://pypi.python.org/pypi/nutree/)
 [![License](https://img.shields.io/pypi/l/nutree.svg)](https://github.com/mar10/nutree/blob/main/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/nutree/badge/?version=latest)](http://nutree.readthedocs.io/)
-[![Coverage Status](https://coveralls.io/repos/github/mar10/nutree/badge.svg?branch=main)](https://coveralls.io/github/mar10/nutree?branch=main)
+[![codecov](https://codecov.io/github/mar10/nutree/branch/main/graph/badge.svg?token=9xmAFm8Icl)](https://codecov.io/github/mar10/nutree)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Released with: Yabs](https://img.shields.io/badge/released%20with-yabs-yellowgreen)](https://github.com/mar10/yabs)
 [![StackOverflow: nutree](https://img.shields.io/badge/StackOverflow-nutree-blue.svg)](https://stackoverflow.com/questions/tagged/nutree)
 
-> Elegant trees for primates&trade;
-
-_Nutree_ is a Python library for tree data structures with an intuitive,
+> _Nutree_ is a Python library for tree data structures with an intuitive,
 yet powerful, API.
 
 **Nutree Facts**
 
 Handle multiple references of single objects ('clones') <br>
 Search by name pattern, id, or object reference <br>
 Unobtrusive handling of arbitrary objects <br>
```

### Comparing `nutree-0.4.0/nutree.egg-info/SOURCES.txt` & `nutree-0.5.0/nutree.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ./nutree/tree.py
 ./nutree/typed_tree.py
 nutree.egg-info/PKG-INFO
 nutree.egg-info/SOURCES.txt
 nutree.egg-info/dependency_links.txt
 nutree.egg-info/entry_points.txt
 nutree.egg-info/not-zip-safe
+nutree.egg-info/requires.txt
 nutree.egg-info/top_level.txt
 tests/test_bench.py
 tests/test_clones.py
 tests/test_core.py
 tests/test_diff.py
 tests/test_objects.py
 tests/test_serialize.py
```

### Comparing `nutree-0.4.0/setup.cfg` & `nutree-0.5.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 package_dir = 
 	= .
 packages = find:
 zip_safe = False
 install_requires = 
 
+[options.extras_require]
+graph = pydot; rdflib; graphviz
+
 [options.packages.find]
 where = .
 include_package_data = True
 exclude = 
 	tests
 
 [options.data_files]
@@ -67,31 +69,11 @@
 	raise NotImplementedError
 	if __name__ == .__main__.:
 	if TYPE_CHECKING:
 
 [coverage:html]
 directory = build/coverage
 
-[flake8]
-enable-extensions = G
-exclude = 
-	__pycache__,
-	.cache,
-	.eggs,
-	.git,
-	.tox,
-	.vscode,
-	build,
-	dist,
-	docs
-max-line-length = 99
-ignore = E203, E501, E731, W503, P101
-docstring-convention = all  # google?
-inline-quotes = double
-multiline-quotes = """
-docstring-quotes = """
-avoid-escape = True
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nutree-0.4.0/tests/test_bench.py` & `nutree-0.5.0/tests/test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import sys
 
 import pytest
 
@@ -175,28 +174,30 @@
         # tree.print()
 
         node_count = len(tree)
         tree_size = asizeof(tree)
         node_size = tree_size / node_count
 
         results.append(
-            f"Tree 10x9: {node_count:,} nodes, {tree_size:,} bytes, node-size: {node_size:.1f} bytes"
+            f"Tree 10x9: {node_count:,} nodes, {tree_size:,} bytes, "
+            f"node-size: {node_size:.1f} bytes"
         )
 
         print(asized(tree.first_child(), detail=1).format())
 
         tree = fixture.generate_tree([100, 100, 99])
         assert len(tree) == 1000100
 
         node_count = len(tree)
         tree_size = asizeof(tree)
         node_size = tree_size / node_count
 
         results.append(
-            f"Tree 100x100x99: {node_count:,} nodes, {tree_size:,} bytes, node-size: {node_size:.1f} bytes"
+            f"Tree 100x100x99: {node_count:,} nodes, {tree_size:,} bytes, "
+            f"node-size: {node_size:.1f} bytes"
         )
         with capsys.disabled():
             print("\n  - ".join(results))
 
     # def test_tree_mem(self, capsys):
     #     """ """
     #     from pympler import tracker
```

### Comparing `nutree-0.4.0/tests/test_clones.py` & `nutree-0.5.0/tests/test_clones.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import pytest
 
 from nutree import AmbiguousMatchError, Node, Tree
```

### Comparing `nutree-0.4.0/tests/test_core.py` & `nutree-0.5.0/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import os
 import re
 from pathlib import Path
 
@@ -143,14 +142,15 @@
         assert records.is_first_sibling()
         assert records.next_sibling().is_last_sibling()
         assert records.last_child().is_leaf()
 
         assert records.count_descendants() == 2
         assert records.count_descendants(leaves_only=True) == 2
 
+        assert tree.children[0] is records
         assert tree.first_child() is records
         assert tree.last_child().name == "Books"
 
         assert records.parent is None
         assert records.first_child().parent is records
         assert records.first_child().name == "Let It Be"
         assert records.first_child().next_sibling().name == "Get Yer Ya-Ya's Out!"
```

### Comparing `nutree-0.4.0/tests/test_diff.py` & `nutree-0.5.0/tests/test_diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 from nutree import diff_node_formatter
 
 from . import fixture
```

### Comparing `nutree-0.4.0/tests/test_objects.py` & `nutree-0.5.0/tests/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import pytest
 
 from nutree import Tree
```

### Comparing `nutree-0.4.0/tests/test_serialize.py` & `nutree-0.5.0/tests/test_serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
-# (c) 2021-2022 Martin Wendt; see https://github.com/mar10/nutree
+# (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 """
 import json
 import tempfile
 
 from nutree import Node, Tree
+from nutree.common import FILE_FORMAT_VERSION
 from nutree.diff import DiffClassification, diff_node_formatter
 
 from . import fixture
 
 
 class TestSerialize:
     def setup_method(self):
@@ -45,19 +45,24 @@
         b = tree["B"]
         a11 = tree["a11"]
         clone = b.prepend_child(a11)
         assert clone.is_clone()
 
         with tempfile.TemporaryFile("r+t") as fp:
             # Serialize
-            tree.save(fp)
+            tree.save(fp, meta={"foo": "bar"})
             # Deserialize
             fp.seek(0)
-            tree_2 = Tree.load(fp)
+            meta_2 = {}
+            tree_2 = Tree.load(fp, file_meta=meta_2)
 
+        assert isinstance(tree_2, Tree)
+        assert all(isinstance(n, Node) for n in tree_2)
+        assert meta_2["$version"] == FILE_FORMAT_VERSION
+        assert meta_2["foo"] == "bar"
         assert fixture.trees_equal(tree, tree_2)
 
         # print(tree.format(repr="{node}"))
         # print(tree_2.format(repr="{node}"))
 
         assert tree.count == tree_2.count
         assert tree.first_child() is not tree_2.first_child()
@@ -143,14 +148,21 @@
         charleen_2 = tree_2.find(match=".*Charleen.*")
         assert charleen_2.is_clone(), "Restored clone"
         # assert len(tree_2.find_all("Charleen")) == 2
 
         assert tree._self_check()
         assert tree_2._self_check()
 
+    # def test_logger(self):
+    #     tree= fixture.create_tree()
+    #     logging.basicConfig()
+    #     logger = logging.getLogger()
+    #     logger.error(tree.format())
+    #     logger.error("DONE")
+
 
 class TestDot:
     def test_serialize_dot(self):
         """Save/load as  object tree with clones."""
 
         tree = fixture.create_tree(style="simple", clones=True, name="Root")
```

