# Comparing `tmp/dbnd-mlflow-1.0.8.1.tar.gz` & `tmp/dbnd-mlflow-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-mlflow-1.0.8.1.tar", last modified: Tue Nov 22 15:16:23 2022, max compression
+gzip compressed data, was "dbnd-mlflow-1.0.9.1.tar", last modified: Tue Nov 22 16:26:47 2022, max compression
```

## Comparing `dbnd-mlflow-1.0.8.1.tar` & `dbnd-mlflow-1.0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.044517 dbnd-mlflow-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4290 2022-11-22 15:16:23.044517 dbnd-mlflow-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2871 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:23.045517 dbnd-mlflow-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.041517 dbnd-mlflow-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.043517 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2361 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/databand_store.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/mlflow_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/tracking_store.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2022-11-22 15:16:09.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.044517 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4290 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      275 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 15:16:23.000000 dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.039749 dbnd-mlflow-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4290 2022-11-22 16:26:47.039749 dbnd-mlflow-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:47.040749 dbnd-mlflow-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.034749 dbnd-mlflow-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.037749 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/databand_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/mlflow_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/tracking_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2022-11-22 16:26:26.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.039749 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4290 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      275 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 16:26:46.000000 dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/top_level.txt
```

### Comparing `dbnd-mlflow-1.0.8.1/LICENSE` & `dbnd-mlflow-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/PKG-INFO` & `dbnd-mlflow-1.0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-mlflow
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

### Comparing `dbnd-mlflow-1.0.8.1/README.md` & `dbnd-mlflow-1.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/setup.cfg` & `dbnd-mlflow-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-mlflow-1.0.8.1/setup.py` & `dbnd-mlflow-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/_plugin.py` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/databand_store.py` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/databand_store.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/mlflow_config.py` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/mlflow_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/tracking_store.py` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/tracking_store.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow/url_utils.py` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow/url_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-mlflow-1.0.8.1/src/dbnd_mlflow.egg-info/PKG-INFO` & `dbnd-mlflow-1.0.9.1/src/dbnd_mlflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-mlflow
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

