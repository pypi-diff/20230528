# Comparing `tmp/simple_matrix_api-0.0.2.tar.gz` & `tmp/simple_matrix_api-0.0.3.tar.gz`

## Comparing `simple_matrix_api-0.0.2.tar` & `simple_matrix_api-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/src/simple_matrix_api/__about__.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/src/simple_matrix_api/__init__.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/src/simple_matrix_api/client.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/.gitignore
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/README.md
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/src/simple_matrix_api/__about__.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/src/simple_matrix_api/__init__.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/src/simple_matrix_api/client.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/.gitignore
+-rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/README.md
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 simple_matrix_api-0.0.3/PKG-INFO
```

### Comparing `simple_matrix_api-0.0.2/src/simple_matrix_api/__init__.py` & `simple_matrix_api-0.0.3/src/simple_matrix_api/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_matrix_api-0.0.2/src/simple_matrix_api/client.py` & `simple_matrix_api-0.0.3/src/simple_matrix_api/client.py`

 * *Files identical despite different names*

### Comparing `simple_matrix_api-0.0.2/LICENSE.txt` & `simple_matrix_api-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_matrix_api-0.0.2/README.md` & `simple_matrix_api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_matrix_api-0.0.2/pyproject.toml` & `simple_matrix_api-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "requests"
+]
 
 [project.urls]
 Documentation = "https://github.com/StrajnarFilip/simple-matrix-api"
 Issues = "https://github.com/StrajnarFilip/simple-matrix-api"
 Source = "https://github.com/StrajnarFilip/simple-matrix-api"
 
 [tool.hatch.version]
```

### Comparing `simple_matrix_api-0.0.2/PKG-INFO` & `simple_matrix_api-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-matrix-api
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/StrajnarFilip/simple-matrix-api
 Project-URL: Issues, https://github.com/StrajnarFilip/simple-matrix-api
 Project-URL: Source, https://github.com/StrajnarFilip/simple-matrix-api
 Author-email: Filip Strajnar <filip.strajnar@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # simple-matrix-api
 
 [![PyPI - Version](https://img.shields.io/pypi/v/simple-matrix-api.svg)](https://pypi.org/project/simple-matrix-api)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simple-matrix-api.svg)](https://pypi.org/project/simple-matrix-api)
```

