# Comparing `tmp/dbnd-snowflake-1.0.8.1.tar.gz` & `tmp/dbnd-snowflake-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-snowflake-1.0.8.1.tar", last modified: Tue Nov 22 15:16:26 2022, max compression
+gzip compressed data, was "dbnd-snowflake-1.0.9.1.tar", last modified: Tue Nov 22 16:26:52 2022, max compression
```

## Comparing `dbnd-snowflake-1.0.8.1.tar` & `dbnd-snowflake-1.0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.934915 dbnd-snowflake-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1667 2022-11-22 15:16:26.934915 dbnd-snowflake-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:26.935915 dbnd-snowflake-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.930914 dbnd-snowflake-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.932914 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.934915 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/sdk/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2022-11-22 15:16:09.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/sdk/snowflake_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.933915 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1667 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-11-22 15:16:26.000000 dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.904352 dbnd-snowflake-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-11-22 16:26:52.904352 dbnd-snowflake-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:52.906352 dbnd-snowflake-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      602 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.895351 dbnd-snowflake-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.901351 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.903351 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9834 2022-11-22 16:26:26.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/sdk/snowflake_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.903351 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-11-22 16:26:52.000000 dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/top_level.txt
```

### Comparing `dbnd-snowflake-1.0.8.1/LICENSE` & `dbnd-snowflake-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-snowflake-1.0.8.1/PKG-INFO` & `dbnd-snowflake-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-snowflake
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

### Comparing `dbnd-snowflake-1.0.8.1/setup.cfg` & `dbnd-snowflake-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-snowflake-1.0.8.1/setup.py` & `dbnd-snowflake-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-snowflake-1.0.8.1/src/dbnd_snowflake/sdk/snowflake_tracker.py` & `dbnd-snowflake-1.0.9.1/src/dbnd_snowflake/sdk/snowflake_tracker.py`

 * *Files identical despite different names*

### Comparing `dbnd-snowflake-1.0.8.1/src/dbnd_snowflake.egg-info/PKG-INFO` & `dbnd-snowflake-1.0.9.1/src/dbnd_snowflake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-snowflake
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

