# Comparing `tmp/dbnd-airflow-auto-tracking-1.0.8.1.tar.gz` & `tmp/dbnd-airflow-auto-tracking-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-airflow-auto-tracking-1.0.8.1.tar", last modified: Tue Nov 22 15:16:18 2022, max compression
+gzip compressed data, was "dbnd-airflow-auto-tracking-1.0.9.1.tar", last modified: Tue Nov 22 16:26:40 2022, max compression
```

## Comparing `dbnd-airflow-auto-tracking-1.0.8.1.tar` & `dbnd-airflow-auto-tracking-1.0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.801083 dbnd-airflow-auto-tracking-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1917 2022-11-22 15:16:18.801083 dbnd-airflow-auto-tracking-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:18.802084 dbnd-airflow-auto-tracking-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      806 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.798083 dbnd-airflow-auto-tracking-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.799083 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2022-11-22 15:16:09.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking/dbnd_airflow_auto_tracking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.800083 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1917 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       66 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-11-22 15:16:18.000000 dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.963127 dbnd-airflow-auto-tracking-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1917 2022-11-22 16:26:40.963127 dbnd-airflow-auto-tracking-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:40.964127 dbnd-airflow-auto-tracking-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      806 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.959126 dbnd-airflow-auto-tracking-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.961126 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2022-11-22 16:26:26.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking/dbnd_airflow_auto_tracking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.963127 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1917 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       66 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2022-11-22 16:26:40.000000 dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/top_level.txt
```

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/LICENSE` & `dbnd-airflow-auto-tracking-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/PKG-INFO` & `dbnd-airflow-auto-tracking-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow-auto-tracking
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

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/setup.cfg` & `dbnd-airflow-auto-tracking-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/setup.py` & `dbnd-airflow-auto-tracking-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking/dbnd_airflow_auto_tracking.py` & `dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking/dbnd_airflow_auto_tracking.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/PKG-INFO` & `dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow-auto-tracking
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

### Comparing `dbnd-airflow-auto-tracking-1.0.8.1/src/dbnd_airflow_auto_tracking.egg-info/SOURCES.txt` & `dbnd-airflow-auto-tracking-1.0.9.1/src/dbnd_airflow_auto_tracking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

