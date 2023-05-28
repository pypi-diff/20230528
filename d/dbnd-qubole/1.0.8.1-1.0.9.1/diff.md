# Comparing `tmp/dbnd-qubole-1.0.8.1.tar.gz` & `tmp/dbnd-qubole-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-qubole-1.0.8.1.tar", last modified: Tue Nov 22 15:16:27 2022, max compression
+gzip compressed data, was "dbnd-qubole-1.0.9.1.tar", last modified: Tue Nov 22 16:26:53 2022, max compression
```

## Comparing `dbnd-qubole-1.0.8.1.tar` & `dbnd-qubole-1.0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:27.500973 dbnd-qubole-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1426 2022-11-22 15:16:27.500973 dbnd-qubole-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:27.501973 dbnd-qubole-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:27.497972 dbnd-qubole-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:27.498972 dbnd-qubole-1.0.8.1/src/dbnd_qubole/
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7347 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole/qubole.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2022-11-22 15:16:09.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole/qubole_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:27.500973 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1426 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 15:16:27.000000 dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:53.689432 dbnd-qubole-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1426 2022-11-22 16:26:53.689432 dbnd-qubole-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:53.690433 dbnd-qubole-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      562 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:53.685432 dbnd-qubole-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:53.687432 dbnd-qubole-1.0.9.1/src/dbnd_qubole/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7347 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole/qubole.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2022-11-22 16:26:26.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole/qubole_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:53.689432 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1426 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 16:26:53.000000 dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/top_level.txt
```

### Comparing `dbnd-qubole-1.0.8.1/LICENSE` & `dbnd-qubole-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-qubole-1.0.8.1/PKG-INFO` & `dbnd-qubole-1.0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-qubole
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

### Comparing `dbnd-qubole-1.0.8.1/setup.cfg` & `dbnd-qubole-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-qubole-1.0.8.1/setup.py` & `dbnd-qubole-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-qubole-1.0.8.1/src/dbnd_qubole/errors.py` & `dbnd-qubole-1.0.9.1/src/dbnd_qubole/errors.py`

 * *Files identical despite different names*

### Comparing `dbnd-qubole-1.0.8.1/src/dbnd_qubole/qubole.py` & `dbnd-qubole-1.0.9.1/src/dbnd_qubole/qubole.py`

 * *Files identical despite different names*

### Comparing `dbnd-qubole-1.0.8.1/src/dbnd_qubole/qubole_config.py` & `dbnd-qubole-1.0.9.1/src/dbnd_qubole/qubole_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-qubole-1.0.8.1/src/dbnd_qubole.egg-info/PKG-INFO` & `dbnd-qubole-1.0.9.1/src/dbnd_qubole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-qubole
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

