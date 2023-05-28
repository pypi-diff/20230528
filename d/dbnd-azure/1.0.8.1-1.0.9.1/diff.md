# Comparing `tmp/dbnd-azure-1.0.8.1.tar.gz` & `tmp/dbnd-azure-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-azure-1.0.8.1.tar", last modified: Tue Nov 22 15:16:18 2022, max compression
+gzip compressed data, was "dbnd-azure-1.0.9.1.tar", last modified: Tue Nov 22 16:26:40 2022, max compression
```

## Comparing `dbnd-azure-1.0.8.1.tar` & `dbnd-azure-1.0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.166019 dbnd-azure-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 15:16:18.166019 dbnd-azure-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:18.167019 dbnd-azure-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.163018 dbnd-azure-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.165019 dbnd-azure-1.0.8.1/src/dbnd_azure/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/azure_sync_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.166019 dbnd-azure-1.0.8.1/src/dbnd_azure/fs/
--rw-rw-rw-   0 root         (0) root         (0)      439 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/fs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11086 2022-11-22 15:16:09.000000 dbnd-azure-1.0.8.1/src/dbnd_azure/fs/azure_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:18.166019 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       85 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 15:16:18.000000 dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.156044 dbnd-azure-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 16:26:40.156044 dbnd-azure-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:40.157044 dbnd-azure-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.150043 dbnd-azure-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.154044 dbnd-azure-1.0.9.1/src/dbnd_azure/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/azure_sync_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.155044 dbnd-azure-1.0.9.1/src/dbnd_azure/fs/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/fs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11086 2022-11-22 16:26:26.000000 dbnd-azure-1.0.9.1/src/dbnd_azure/fs/azure_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:40.155044 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       85 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 16:26:40.000000 dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/top_level.txt
```

### Comparing `dbnd-azure-1.0.8.1/LICENSE` & `dbnd-azure-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/PKG-INFO` & `dbnd-azure-1.0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-azure
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

### Comparing `dbnd-azure-1.0.8.1/setup.cfg` & `dbnd-azure-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-azure-1.0.8.1/setup.py` & `dbnd-azure-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure/_plugin.py` & `dbnd-azure-1.0.9.1/src/dbnd_azure/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure/azure_sync_ctrl.py` & `dbnd-azure-1.0.9.1/src/dbnd_azure/azure_sync_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure/credentials.py` & `dbnd-azure-1.0.9.1/src/dbnd_azure/credentials.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure/env.py` & `dbnd-azure-1.0.9.1/src/dbnd_azure/env.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure/fs/azure_blob.py` & `dbnd-azure-1.0.9.1/src/dbnd_azure/fs/azure_blob.py`

 * *Files identical despite different names*

### Comparing `dbnd-azure-1.0.8.1/src/dbnd_azure.egg-info/PKG-INFO` & `dbnd-azure-1.0.9.1/src/dbnd_azure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-azure
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

