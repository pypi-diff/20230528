# Comparing `tmp/dbnd-redshift-1.0.8.1.tar.gz` & `tmp/dbnd-redshift-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-redshift-1.0.8.1.tar", last modified: Tue Nov 22 15:16:24 2022, max compression
+gzip compressed data, was "dbnd-redshift-1.0.9.1.tar", last modified: Tue Nov 22 16:26:49 2022, max compression
```

## Comparing `dbnd-redshift-1.0.8.1.tar` & `dbnd-redshift-1.0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.639680 dbnd-redshift-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1688 2022-11-22 15:16:24.639680 dbnd-redshift-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:24.640680 dbnd-redshift-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.635680 dbnd-redshift-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.636680 dbnd-redshift-1.0.8.1/src/dbnd_redshift/
--rw-rw-rw-   0 root         (0) root         (0)      192 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/dbnd_redshift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.639680 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_connection_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_connection_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    11968 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13337 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_values.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2022-11-22 15:16:09.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/wrappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.637680 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1688 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      659 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       49 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 15:16:24.000000 dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:49.463998 dbnd-redshift-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1688 2022-11-22 16:26:49.463998 dbnd-redshift-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:49.465998 dbnd-redshift-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:49.458997 dbnd-redshift-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:49.459998 dbnd-redshift-1.0.9.1/src/dbnd_redshift/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/dbnd_redshift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:49.463998 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_connection_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_connection_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13337 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2022-11-22 16:26:26.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:49.461998 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1688 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 16:26:49.000000 dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/top_level.txt
```

### Comparing `dbnd-redshift-1.0.8.1/LICENSE` & `dbnd-redshift-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/PKG-INFO` & `dbnd-redshift-1.0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-redshift
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

### Comparing `dbnd-redshift-1.0.8.1/setup.cfg` & `dbnd-redshift-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/dbnd_redshift.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/dbnd_redshift.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_connection_collection.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_connection_collection.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_connection_extractor.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_connection_extractor.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_tracker.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_tracker.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_utils.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/redshift_values.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/redshift_values.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift/sdk/wrappers.py` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift/sdk/wrappers.py`

 * *Files identical despite different names*

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/PKG-INFO` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-redshift
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

### Comparing `dbnd-redshift-1.0.8.1/src/dbnd_redshift.egg-info/SOURCES.txt` & `dbnd-redshift-1.0.9.1/src/dbnd_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

