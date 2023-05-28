# Comparing `tmp/ziper-0.1.4.tar.gz` & `tmp/ziper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziper-0.1.4.tar", max compression
+gzip compressed data, was "ziper-0.1.5.tar", max compression
```

## Comparing `ziper-0.1.4.tar` & `ziper-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.4/LICENSE
--rw-r--r--   0        0        0      365 2023-05-27 22:20:47.417939 ziper-0.1.4/README.md
--rw-r--r--   0        0        0      506 2023-05-27 22:20:47.418011 ziper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.4/ziper/__init__.py
--rw-r--r--   0        0        0     3955 2023-05-27 22:30:24.195834 ziper-0.1.4/ziper/iter.py
--rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.4/ziper/py.typed
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 ziper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.5/LICENSE
+-rw-r--r--   0        0        0      365 2023-05-27 22:20:47.417939 ziper-0.1.5/README.md
+-rw-r--r--   0        0        0      506 2023-05-27 23:35:14.962889 ziper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.5/ziper/__init__.py
+-rw-r--r--   0        0        0     4364 2023-05-28 00:12:40.072403 ziper-0.1.5/ziper/iter.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.5/ziper/py.typed
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 ziper-0.1.5/PKG-INFO
```

### Comparing `ziper-0.1.4/LICENSE` & `ziper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ziper-0.1.4/ziper/iter.py` & `ziper-0.1.5/ziper/iter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 import itertools
 import more_itertools as mitertools
 
 from typing import (
+    Callable,
+    Generic,
     Iterable,
     Iterator,
-    Generic,
     Optional,
     TypeVar,
     Tuple,
-    Callable,
 )
 
 
 T = TypeVar('T')
 U = TypeVar('U')
 V = TypeVar('V')
 
@@ -145,13 +145,21 @@
 
     def find_position(self, predicate: Fn[T, bool]) -> Optional[Tuple[int, T]]:
         for index, x in self.enumerate():
             if predicate(x):
                 return index, x
         return None
 
+    def find_positions(self, predicate: Fn[T, bool]) -> Iter[Tuple[int, T]]:
+        return self.enumerate().filter(lambda pair: predicate(pair[1]))
+
     def positions(self, predicate: Fn[T, bool]) -> Iter[int]:
-        return (
-            self.enumerate()
-            .filter(lambda pair: predicate(pair[1]))
-            .map(lambda pair: pair[0])
-        )
+        return self.find_positions(predicate).map(lambda pair: pair[0])
+
+    def cartesian_product(self, other: Iterable[U]) -> Iter[Tuple[T, U]]:
+        return Iter(itertools.product(self, other))
+
+    def permutations(self, k: int) -> Iter[Tuple[T, ...]]:
+        return Iter(itertools.permutations(self, k))
+
+    def powerset(self) -> Iter[Tuple[T, ...]]:
+        return Iter(mitertools.powerset(self))
```

### Comparing `ziper-0.1.4/PKG-INFO` & `ziper-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Rust-like iterator for Python
 Home-page: https://github.com/cospectrum/ziper
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

