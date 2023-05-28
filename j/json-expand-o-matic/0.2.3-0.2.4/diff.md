# Comparing `tmp/json_expand_o_matic-0.2.3.tar.gz` & `tmp/json_expand_o_matic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_expand_o_matic-0.2.3.tar", last modified: Thu May 25 02:45:09 2023, max compression
+gzip compressed data, was "json_expand_o_matic-0.2.4.tar", last modified: Sun May 28 21:39:37 2023, max compression
```

## Comparing `json_expand_o_matic-0.2.3.tar` & `json_expand_o_matic-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:43:35.000000 json_expand_o_matic-0.2.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:43:21.000000 json_expand_o_matic-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.613489 json_expand_o_matic-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/src/json_expand_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/contractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expand_o_matic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_zipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/leaf_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/test_leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-28 21:38:11.000000 json_expand_o_matic-0.2.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 21:38:06.000000 json_expand_o_matic-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:37.114923 json_expand_o_matic-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/src/json_expand_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/contractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/expand_o_matic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/expansion_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/expansion_zipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic/leaf_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-28 21:39:37.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-28 21:39:37.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:39:37.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-28 21:39:37.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 21:39:37.000000 json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:37.118923 json_expand_o_matic-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/tests/test_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 21:37:58.000000 json_expand_o_matic-0.2.4/version.txt
```

### Comparing `json_expand_o_matic-0.2.3/LICENSE.txt` & `json_expand_o_matic-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/PKG-INFO` & `json_expand_o_matic-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_expand_o_matic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.3/README.md` & `json_expand_o_matic-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/dev-requirements.txt` & `json_expand_o_matic-0.2.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/setup.py` & `json_expand_o_matic-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='json_expand_o_matic',
 
-    version='0.2.3',
+    version='0.2.4',
 
     description='Expand a dict into a collection of subdirectories and json files or '
                 'contract (un-expand) the output of expand() into a dict.',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/__init__.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     See also: .jsonrefkeeper
 
 """
 
 from .expand_o_matic import JsonExpandOMatic
 
-VERSION = "v0.2.3"
+VERSION = "v0.2.4"
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/cli.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/cli.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/contractor.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/contractor.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expand_o_matic.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/expand_o_matic.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expander.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/expander.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,22 @@
         self.data = data
         self.leaf_nodes = leaf_nodes
 
         self.options = options if options is not None else dict()
 
         # options will not include pool or zip options when called recursively.
         self.pool_options = {
-            key: self.options.pop(key) for key in {key for key in self.options.keys() if key.startswith("pool_")}
+            # See ExpansionPool
+            key: self.options.pop(key)
+            for key in {key for key in self.options.keys() if key.startswith("pool_")}
         }
         self.zip_options = {
-            key: self.options.pop(key) for key in {key for key in self.options.keys() if key.startswith("zip_")}
+            # See ExpansionZipper
+            key: self.options.pop(key)
+            for key in {key for key in self.options.keys() if key.startswith("zip_")}
         }
 
         assert (
             (not self.pool_options and not self.zip_options) or self.pool_options or self.zip_options
         ), f"Cannot mix {sorted(self.pool_options.keys())} and {sorted(self.zip_options.keys())}"
 
         self.ref_key = self.options.get("ref_key", "$ref")
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_pool.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/expansion_pool.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from ctypes import POINTER, Structure, c_ubyte, cast, create_string_buffer, string_at
 from enum import Enum
 from typing import Optional, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
-class Modes(Enum):
+class InitArgsType(Enum):
     ArrayOfTuples = "ArrayOfTuples"
     SharedMemoryArray = "SharedMemoryArray"
 
 
-__mode__ = Modes.SharedMemoryArray
-__unpack__ = None
+__initargsmode__ = InitArgsType.SharedMemoryArray
+__unpackfunc__ = None
 __work__ = None
 
 
 class WorkTuple(Structure):
     _fields_ = [
         ("directory", POINTER(c_ubyte)),
         ("filename", POINTER(c_ubyte)),
@@ -37,34 +37,34 @@
         yield self.filename
         yield self.data
         yield self.checksum_filename
         yield self.checksum
 
 
 def _initialize(mode, data):
-    global __mode__
+    global __initargsmode__
     global __work__
-    global __unpack__
+    global __unpackfunc__
 
-    __mode__ = mode
+    __initargsmode__ = mode
     __work__ = data
 
-    if __mode__ == Modes.SharedMemoryArray:
-        __unpack__ = lambda request: [  # noqa: E731
+    if __initargsmode__ == InitArgsType.SharedMemoryArray:
+        __unpackfunc__ = lambda request: [  # noqa: E731
             string_at(element).decode("utf-8") for element in __work__[request]
         ]
-    elif __mode__ == Modes.ArrayOfTuples:
-        __unpack__ = lambda request: __work__[request]  # noqa: E731
+    elif __initargsmode__ == InitArgsType.ArrayOfTuples:
+        __unpackfunc__ = lambda request: __work__[request]  # noqa: E731
 
 
 def _write_file(request):
-    global __unpack__
+    global __unpackfunc__
 
     begin = time.time()
-    directory, filename, data, checksum_filename, checksum = __unpack__(request)
+    directory, filename, data, checksum_filename, checksum = __unpackfunc__(request)
 
     def do():
         with open(f"{directory}/{filename}", "w") as f:
             f.write(data)
         if checksum_filename and checksum:
             with open(f"{directory}/{checksum_filename}", "w") as f:
                 f.write(checksum)
@@ -85,77 +85,80 @@
     def __init__(
         self,
         *,
         logger: logging.Logger,
         pool_ratio: Optional[float] = None,
         pool_size: Optional[int] = None,
         pool_disable: Optional[bool] = False,
-        pool_mode: Union[str, Modes] = Modes.SharedMemoryArray,
+        pool_mode: Union[str, InitArgsType] = InitArgsType.SharedMemoryArray,
     ):
         assert logger, "logger is required"
         self.logger = logger
         self.work: list = list()
 
-        self.mode = Modes(pool_mode)
+        self.init_style = InitArgsType(pool_mode)
 
         self._set_pool_size(pool_ratio, pool_size, pool_disable)
 
         if self.pool_size > 1:
-            logger.info(f"PoolSize: [{self.pool_size}]. Mode [{self.mode.value}].")
+            logger.info(f"PoolSize: [{self.pool_size}]. Mode [{self.init_style.value}].")
         else:
             logger.info(f"PoolSize: [{self.pool_size}].")
 
     def setup(self) -> Tuple["ExpansionPool", list]:
         return self, self.work
 
     def finalize(self):
         begin = time.time()
 
         if self.pool_size == 1:
-            _initialize(Modes.ArrayOfTuples, self.work)
+            _initialize(InitArgsType.ArrayOfTuples, self.work)
             results = [_write_file(i) for i in range(0, len(self.work))]
 
         else:
             results = self._pooled_processing()
 
         self.elapsed = time.time() - begin
 
         self.work_time = sum(results)
         self.overhead = self.elapsed - self.work_time
 
-    def _pooled_processing(self, chunksize, data):
-        if self.mode == Modes.SharedMemoryArray:
+    def _pooled_processing(self):
+        if self.init_style == InitArgsType.SharedMemoryArray:
             data = self._prepare_shared_memory_array()
-        elif self.mode == Modes.ArrayOfTuples:
+        elif self.init_style == InitArgsType.ArrayOfTuples:
             data = self.work
 
         chunksize = 1 + int(len(self.work) / self.pool_size)
 
-        with mp.Pool(processes=self.pool_size, initializer=_initialize, initargs=(self.mode, data)) as pool:
+        with mp.Pool(processes=self.pool_size, initializer=_initialize, initargs=(self.init_style, data)) as pool:
             futures = pool.map(_write_file, range(0, len(self.work)), chunksize=chunksize)
             results = [f for f in futures]
             return results
 
     def _prepare_shared_memory_array(self):
         value_list = [
             WorkTuple(
-                *[cast(create_string_buffer(component.encode("utf-8")), POINTER(c_ubyte)) for component in work_unit]
+                *[
+                    cast(create_string_buffer((component or "").encode("utf-8")), POINTER(c_ubyte))
+                    for component in work_unit
+                ]
             )
             for work_unit in self.work
         ]
         data = mp.Array(WorkTuple, value_list, lock=False)
         return data
 
     def _set_pool_size(self, pool_ratio, pool_size, pool_disable):
         if pool_disable:
             self.pool_size = 1
         elif pool_size:
             self.pool_size = abs(pool_size)
         elif pool_size == 0 and not pool_ratio:
             self.pool_size = os.cpu_count()
         elif pool_ratio:
-            assert pool_size is None, "Programmer error."
-            self.pool_size = abs(int(os.cpu_count() * self.pool_ratio))
+            assert (
+                pool_size is None
+            ), f"Programmer error: pool_ratio [{pool_ratio}] cannot be used with pool_size [{pool_size}]."
+            self.pool_size = abs(int(os.cpu_count() * pool_ratio))
         else:
-            assert pool_size is None, "Programmer error."
-            assert pool_ratio is None, "Programmer error."
             self.pool_size = 1
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_zipper.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/expansion_zipper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 import io
 import logging
 import os
 import zipfile
-from typing import Optional, Tuple
+from enum import Enum
+from typing import Optional, Tuple, Union
+
+
+class OutputChoice(Enum):
+    KeepZip = "KeepZip"
+    UnZipped = "UnZipped"
+    Zipped = "Zipped"
 
 
 class ExpansionZipper:
     def __init__(
         self,
         *,
         logger: logging.Logger,
-        output_path: Optional[str] = None,
-        zip_root: Optional[str] = None,
-        zip_file: Optional[str] = None,
+        output_path: Optional[str] = None,  # . Where the output will be written.
+        zip_root: Optional[str] = None,  # .... Where all the files are within the zip.
+        zip_file: Optional[str] = None,  # .... Name of the zip file to create in `output_path`.
+        zip_output: Union[str, OutputChoice] = OutputChoice.UnZipped,  # Keep zipped, unzip or both.
     ):
         assert logger, "logger is required"
         self.logger = logger
         self.work: list = list()
 
+        self.output_mode = OutputChoice(zip_output)
+
         if output_path:
-            if not zip_file:
+            if zip_file and zip_root:
+                ...
+            elif not zip_file and not zip_root:
                 zip_file = os.path.basename(output_path)
-                output_path = os.path.dirname(output_path) or "."
+                zip_root = os.path.basename(output_path)
+                output_path = os.path.dirname(output_path)
+            elif zip_file:
+                zip_root = os.path.basename(output_path)
+                output_path = os.path.dirname(output_path)
+            elif zip_root:
+                zip_file = os.path.basename(output_path)
+
         else:
             output_path = "."
 
         self.output_path = output_path
         self.zip_file = __name__ if not zip_file or zip_file == "." else zip_file
         self.zip_root = zip_root or "."
 
@@ -35,15 +54,28 @@
     def setup(self) -> Tuple["ExpansionZipper", list]:
         return self, self.work
 
     def finalize(self):
         zip_buffer = io.BytesIO()
         with zipfile.ZipFile(zip_buffer, mode="a", compression=zipfile.ZIP_DEFLATED, compresslevel=9) as zip_file:
             for directory, filename, data, checksum_filename, checksum in self.work:
+                assert data is not None
                 zip_file.writestr(f"{directory}/{filename}", data)
-                zip_file.writestr(
-                    f"{directory}/{checksum_filename}", checksum, compress_type=zipfile.ZIP_STORED, compresslevel=0
-                )
+                if checksum is not None:
+                    zip_file.writestr(
+                        f"{directory}/{checksum_filename}", checksum, compress_type=zipfile.ZIP_STORED, compresslevel=0
+                    )
 
         os.makedirs(self.output_path, exist_ok=True)
         with open(f"{self.output_path}/{self.zip_file}", "wb") as f:
             f.write(zip_buffer.getvalue())
+
+        if self.output_mode == OutputChoice.Zipped:
+            return
+
+        zip_file = zipfile.ZipFile(f"{self.output_path}/{self.zip_file}")
+        zip_file.extractall(self.output_path)
+
+        if self.output_mode == OutputChoice.KeepZip:
+            return
+
+        os.remove(f"{self.output_path}/{self.zip_file}")
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic/leaf_node.py` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic/leaf_node.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/PKG-INFO` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-expand-o-matic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/SOURCES.txt` & `json_expand_o_matic-0.2.4/src/json_expand_o_matic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.3/tests/test_leaves.py` & `json_expand_o_matic-0.2.4/tests/test_leaves.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,45 +28,44 @@
     def test_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
     @pytest.fixture
     def original_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
-    def test_actors1(self, tmpdir, test_data, original_data, threaded):
+    def test_actors1(self, tmpdir, test_data, original_data):
         """Verify that we can create a json file for each actor and not recurse any further."""
 
-        self._actors_test(tmpdir, test_data, original_data, "/root/actors/.*", threaded)
+        self._actors_test(tmpdir, test_data, original_data, "/root/actors/.*")
 
-    def test_actors2(self, tmpdir, test_data, original_data, threaded):
+    def test_actors2(self, tmpdir, test_data, original_data):
         """Same as test_actors1 but with a more precise regex."""
 
-        self._actors_test(tmpdir, test_data, original_data, "/root/actors/[^/]+", threaded)
+        self._actors_test(tmpdir, test_data, original_data, "/root/actors/[^/]+")
 
-    def test_charlie1(self, tmpdir, test_data, original_data, threaded):
+    def test_charlie1(self, tmpdir, test_data, original_data):
         """Verify that we can single out an actor."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/charlie_chaplin", threaded)
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/charlie_chaplin")
 
-    def test_charlie2(self, tmpdir, test_data, original_data, threaded):
+    def test_charlie2(self, tmpdir, test_data, original_data):
         """Like test_charlie1 but with a loose wildcard."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz].*", threaded)
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz].*")
 
-    def test_charlie3(self, tmpdir, test_data, original_data, threaded):
+    def test_charlie3(self, tmpdir, test_data, original_data):
         """Like test_charlie1 but with tighter regex."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz][^/]+", threaded)
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz][^/]+")
 
-    def test_threaded_nested1(self, tmpdir, test_data, original_data, threaded):
+    def test_threaded_nested1(self, tmpdir, test_data, original_data):
         """Test a simple leaf_nodes scenario."""
 
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "/[^/]+/filmography"]}],
-            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
@@ -86,15 +85,15 @@
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill.json")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill/children.json")
         assert os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies")
 
-    def test_nested1_equivalency(self, tmpdir, test_data, original_data, threaded):
+    def test_nested1_equivalency(self, tmpdir, test_data, original_data):
         """
         In a nested leaf-node expression the dict key is treated as it
         would be in the non-nested case.
 
         The nested functionality takes the file written by that expression
         and feeds it back through JsonExpandOMatic with the dict's value
         as the new leaf_nodes parameter value.
@@ -106,30 +105,28 @@
         import glob
 
         JsonExpandOMatic(path=f"{tmpdir}/n").expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "/[^/]+/filmography"]}],
-            threaded=threaded,
         )
         nested_files = [x.replace(f"{tmpdir}/n", "") for x in glob.glob(f"{tmpdir}/n", recursive=True)]
 
         JsonExpandOMatic(path=f"{tmpdir}/f").expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=["/root/actors/.*/movies/.*", "/root/actors/.*/filmography"],
-            threaded=threaded,
         )
         flattened_files = [x.replace(f"{tmpdir}/f", "") for x in glob.glob(f"{tmpdir}/f", recursive=True)]
 
         assert nested_files == flattened_files
 
-    def test_nested2(self, tmpdir, test_data, original_data, threaded):
+    def test_nested2(self, tmpdir, test_data, original_data):
         """Test a targeted leaf_node exmple.
 
         The expressions listed in the dict value are relative to the
         element matched by the dict key expression.
         Our previous examlpes used a regex to ignore that but we can do
         interesting things with it if we want.
 
@@ -137,15 +134,14 @@
         and Charlie Chaplin's spouses.
         """
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/dwayne_johnson/movies", "/charlie_chaplin/spouses"]}],
-            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
@@ -157,15 +153,15 @@
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/movies.json")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/movies")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses")
         assert os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/movies.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/movies")
 
-    def xtest_enhanced_nested1(self, tmpdir, test_data, original_data, threaded):
+    def xtest_enhanced_nested1(self, tmpdir, test_data, original_data):
         """Enhanced nested #1...
 
         But what if we want a single json file per actor to include
         everything about that actor _except_ movies and a separate
         movies.json for each actor with all of that actor's movie data?
 
         You might initially have thought that we would do:
@@ -206,15 +202,14 @@
         """
 
         JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "<A:/.*"]}],
-            threaded=threaded,
         )
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
         # Unlike the non-nested case with regex "/root/actors/.*", the nested case
@@ -238,21 +233,20 @@
 
         with open(f"{tmpdir}/root/actors/charlie_chaplin.json") as f:
             data = json.load(f)
             assert data.get("spouses", None)
             assert data.get["spouses"].get("lita_grey", None)
             assert data.get["spouses"]["lita_grey"].get("children", None)
 
-    def _actors_test(self, tmpdir, test_data, original_data, regex, threaded):
+    def _actors_test(self, tmpdir, test_data, original_data, regex):
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[regex],
-            threaded=threaded,
         )
 
         # preserve=True allows mangling of test_data by expand()
         assert test_data != original_data
 
         # expand() returns a new representation of `data`
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
@@ -264,21 +258,20 @@
         # Our leaf-node regex (/root/actors/.*) tells expand to create a
         # per-actor file but not the per-actor directory or anything below that.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
         self._assert_actor_dirs(tmpdir, f=_not)
         self._assert_movies(tmpdir, f=_not)
 
-    def _charlie_test(self, tmpdir, test_data, original_data, regex, threaded):
+    def _charlie_test(self, tmpdir, test_data, original_data, regex):
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[regex],
-            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
         # No recursion for Charlie Chaplin
```

