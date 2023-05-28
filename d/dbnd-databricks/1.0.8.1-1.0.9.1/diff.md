# Comparing `tmp/dbnd-databricks-1.0.8.1.tar.gz` & `tmp/dbnd-databricks-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-databricks-1.0.8.1.tar", last modified: Tue Nov 22 15:16:20 2022, max compression
+gzip compressed data, was "dbnd-databricks-1.0.9.1.tar", last modified: Tue Nov 22 16:26:43 2022, max compression
```

## Comparing `dbnd-databricks-1.0.8.1.tar` & `dbnd-databricks-1.0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:20.552262 dbnd-databricks-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:20.552262 dbnd-databricks-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:20.553263 dbnd-databricks-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:20.549262 dbnd-databricks-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:20.551262 dbnd-databricks-1.0.8.1/src/dbnd_databricks/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     9433 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks/databricks.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks/databricks_config.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2022-11-22 15:16:09.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:20.552262 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-22 15:16:20.000000 dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:43.563393 dbnd-databricks-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:43.563393 dbnd-databricks-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:43.564393 dbnd-databricks-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:43.559393 dbnd-databricks-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:43.561393 dbnd-databricks-1.0.9.1/src/dbnd_databricks/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      251 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9433 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks/databricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks/databricks_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2022-11-22 16:26:26.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:43.563393 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-11-22 16:26:43.000000 dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/top_level.txt
```

### Comparing `dbnd-databricks-1.0.8.1/LICENSE` & `dbnd-databricks-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-databricks-1.0.8.1/PKG-INFO` & `dbnd-databricks-1.0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-databricks
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

### Comparing `dbnd-databricks-1.0.8.1/setup.cfg` & `dbnd-databricks-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-databricks-1.0.8.1/setup.py` & `dbnd-databricks-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-databricks-1.0.8.1/src/dbnd_databricks/databricks.py` & `dbnd-databricks-1.0.9.1/src/dbnd_databricks/databricks.py`

 * *Files identical despite different names*

### Comparing `dbnd-databricks-1.0.8.1/src/dbnd_databricks/databricks_config.py` & `dbnd-databricks-1.0.9.1/src/dbnd_databricks/databricks_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-databricks-1.0.8.1/src/dbnd_databricks/errors.py` & `dbnd-databricks-1.0.9.1/src/dbnd_databricks/errors.py`

 * *Files identical despite different names*

### Comparing `dbnd-databricks-1.0.8.1/src/dbnd_databricks.egg-info/PKG-INFO` & `dbnd-databricks-1.0.9.1/src/dbnd_databricks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-databricks
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

