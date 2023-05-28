# Comparing `tmp/dbnd-airflow-export-1.0.8.1.tar.gz` & `tmp/dbnd-airflow-export-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-airflow-export-1.0.8.1.tar", last modified: Tue Nov 22 15:16:20 2022, max compression
+gzip compressed data, was "dbnd-airflow-export-1.0.9.1.tar", last modified: Tue Nov 22 16:26:42 2022, max compression
```

## Comparing `dbnd-airflow-export-1.0.8.1.tar` & `dbnd-airflow-export-1.0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:19.961202 dbnd-airflow-export-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-airflow-export-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-airflow-export-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1412 2022-11-22 15:16:19.961202 dbnd-airflow-export-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:19.962202 dbnd-airflow-export-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      735 2022-11-22 15:16:09.000000 dbnd-airflow-export-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:19.957202 dbnd-airflow-export-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:19.959202 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 15:16:09.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:19.961202 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1412 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-22 15:16:19.000000 dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:42.615296 dbnd-airflow-export-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-airflow-export-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-airflow-export-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1412 2022-11-22 16:26:42.616296 dbnd-airflow-export-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:42.617296 dbnd-airflow-export-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      735 2022-11-22 16:26:26.000000 dbnd-airflow-export-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:42.611295 dbnd-airflow-export-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:42.613296 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 16:26:26.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:42.615296 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1412 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-11-22 16:26:42.000000 dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/top_level.txt
```

### Comparing `dbnd-airflow-export-1.0.8.1/LICENSE` & `dbnd-airflow-export-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-export-1.0.8.1/PKG-INFO` & `dbnd-airflow-export-1.0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow-export
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

### Comparing `dbnd-airflow-export-1.0.8.1/setup.cfg` & `dbnd-airflow-export-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-airflow-export-1.0.8.1/setup.py` & `dbnd-airflow-export-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-export-1.0.8.1/src/dbnd_airflow_export.egg-info/PKG-INFO` & `dbnd-airflow-export-1.0.9.1/src/dbnd_airflow_export.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow-export
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

