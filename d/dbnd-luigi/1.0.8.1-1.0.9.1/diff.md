# Comparing `tmp/dbnd-luigi-1.0.8.1.tar.gz` & `tmp/dbnd-luigi-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-luigi-1.0.8.1.tar", last modified: Tue Nov 22 15:16:23 2022, max compression
+gzip compressed data, was "dbnd-luigi-1.0.9.1.tar", last modified: Tue Nov 22 16:26:47 2022, max compression
```

## Comparing `dbnd-luigi-1.0.8.1.tar` & `dbnd-luigi-1.0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.566570 dbnd-luigi-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:23.566570 dbnd-luigi-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:23.567571 dbnd-luigi-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.562570 dbnd-luigi-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.564570 dbnd-luigi-1.0.8.1/src/dbnd_luigi/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_params.py
--rw-rw-rw-   0 root         (0) root         (0)     1137 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     5980 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_run_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_target.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3744 2022-11-22 15:16:09.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_tracking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:23.566570 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 15:16:23.000000 dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.792827 dbnd-luigi-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:47.792827 dbnd-luigi-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:47.794827 dbnd-luigi-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      614 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.786826 dbnd-luigi-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.790826 dbnd-luigi-1.0.9.1/src/dbnd_luigi/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     5980 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_run_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_target.py
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2022-11-22 16:26:26.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_tracking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:47.792827 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       44 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 16:26:47.000000 dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/top_level.txt
```

### Comparing `dbnd-luigi-1.0.8.1/LICENSE` & `dbnd-luigi-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/PKG-INFO` & `dbnd-luigi-1.0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-luigi
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

### Comparing `dbnd-luigi-1.0.8.1/setup.cfg` & `dbnd-luigi-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-luigi-1.0.8.1/setup.py` & `dbnd-luigi-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_handlers.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_handlers.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_parameters.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_params.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_params.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_postgres.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_postgres.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_run_manager.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_run_manager.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_target.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_target.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_task.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi/luigi_tracking.py` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi/luigi_tracking.py`

 * *Files identical despite different names*

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/PKG-INFO` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-luigi
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

### Comparing `dbnd-luigi-1.0.8.1/src/dbnd_luigi.egg-info/SOURCES.txt` & `dbnd-luigi-1.0.9.1/src/dbnd_luigi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

