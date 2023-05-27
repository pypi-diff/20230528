# Comparing `tmp/ziper-0.1.3.tar.gz` & `tmp/ziper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziper-0.1.3.tar", max compression
+gzip compressed data, was "ziper-0.1.4.tar", max compression
```

## Comparing `ziper-0.1.3.tar` & `ziper-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.3/LICENSE
--rw-r--r--   0        0        0      453 2023-05-25 18:54:12.835621 ziper-0.1.3/README.md
--rw-r--r--   0        0        0      506 2023-05-25 18:17:41.197798 ziper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.3/ziper/__init__.py
--rw-r--r--   0        0        0     3540 2023-05-25 18:39:02.895670 ziper-0.1.3/ziper/iter.py
--rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.3/ziper/py.typed
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 ziper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.4/LICENSE
+-rw-r--r--   0        0        0      365 2023-05-27 22:20:47.417939 ziper-0.1.4/README.md
+-rw-r--r--   0        0        0      506 2023-05-27 22:20:47.418011 ziper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.4/ziper/__init__.py
+-rw-r--r--   0        0        0     3955 2023-05-27 22:30:24.195834 ziper-0.1.4/ziper/iter.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.4/ziper/py.typed
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 ziper-0.1.4/PKG-INFO
```

### Comparing `ziper-0.1.3/LICENSE` & `ziper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ziper-0.1.3/ziper/iter.py` & `ziper-0.1.4/ziper/iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,7 +138,20 @@
             return x
 
         return self.map(inspector)
 
     def chunks(self, size: int) -> Iter[Iter[T]]:
         it = mitertools.ichunked(self, size)
         return Iter(it).map(lambda chunk: Iter(chunk))
+
+    def find_position(self, predicate: Fn[T, bool]) -> Optional[Tuple[int, T]]:
+        for index, x in self.enumerate():
+            if predicate(x):
+                return index, x
+        return None
+
+    def positions(self, predicate: Fn[T, bool]) -> Iter[int]:
+        return (
+            self.enumerate()
+            .filter(lambda pair: predicate(pair[1]))
+            .map(lambda pair: pair[0])
+        )
```

### Comparing `ziper-0.1.3/PKG-INFO` & `ziper-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Rust-like iterator for Python
 Home-page: https://github.com/cospectrum/ziper
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,24 +21,18 @@
 # ziper
 
 Rust-like iterator for Python
 
 
 ## Install
 
-From PyPI:
 ```sh
 pip install ziper
 ```
 
-From git:
-```sh
-pip install git+https://github.com/cospectrum/ziper.git
-```
-
 ## Usage
 
 ```py
 from ziper import Iter
 
 xs = ['1', '2', 'a', '3', '4', 'b', 'c']
 ys = [6, 7, 8, 9]
```

