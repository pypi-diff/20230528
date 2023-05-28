# Comparing `tmp/dbnd-tensorflow-1.0.8.1.tar.gz` & `tmp/dbnd-tensorflow-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-tensorflow-1.0.8.1.tar", last modified: Tue Nov 22 15:16:25 2022, max compression
+gzip compressed data, was "dbnd-tensorflow-1.0.9.1.tar", last modified: Tue Nov 22 16:26:50 2022, max compression
```

## Comparing `dbnd-tensorflow-1.0.8.1.tar` & `dbnd-tensorflow-1.0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.173735 dbnd-tensorflow-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:25.173735 dbnd-tensorflow-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:25.174735 dbnd-tensorflow-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.170735 dbnd-tensorflow-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.172735 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.173735 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/marshalling/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/marshalling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/marshalling/tensorflow_marshaller.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-11-22 15:16:09.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/marshalling/tensorflow_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.173735 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      557 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-22 15:16:25.000000 dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:50.240077 dbnd-tensorflow-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:50.240077 dbnd-tensorflow-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:50.242078 dbnd-tensorflow-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:50.236077 dbnd-tensorflow-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:50.238077 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:50.240077 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/marshalling/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/marshalling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/marshalling/tensorflow_marshaller.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2022-11-22 16:26:26.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/marshalling/tensorflow_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:50.239077 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      557 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-11-22 16:26:50.000000 dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/top_level.txt
```

### Comparing `dbnd-tensorflow-1.0.8.1/LICENSE` & `dbnd-tensorflow-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-tensorflow-1.0.8.1/PKG-INFO` & `dbnd-tensorflow-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-tensorflow
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-tensorflow-1.0.8.1/setup.cfg` & `dbnd-tensorflow-1.0.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.8.1
+version = 1.0.9.1
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-tensorflow-1.0.8.1/setup.py` & `dbnd-tensorflow-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/_plugin.py` & `dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow/marshalling/tensorflow_marshaller.py` & `dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow/marshalling/tensorflow_marshaller.py`

 * *Files identical despite different names*

### Comparing `dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/PKG-INFO` & `dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-tensorflow
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-tensorflow-1.0.8.1/src/dbnd_tensorflow.egg-info/SOURCES.txt` & `dbnd-tensorflow-1.0.9.1/src/dbnd_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

