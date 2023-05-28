# Comparing `tmp/dbnd-gcp-1.0.8.1.tar.gz` & `tmp/dbnd-gcp-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-gcp-1.0.8.1.tar", last modified: Tue Nov 22 15:16:22 2022, max compression
+gzip compressed data, was "dbnd-gcp-1.0.9.1.tar", last modified: Tue Nov 22 16:26:46 2022, max compression
```

## Comparing `dbnd-gcp-1.0.8.1.tar` & `dbnd-gcp-1.0.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.385450 dbnd-gcp-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 15:16:22.385450 dbnd-gcp-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:22.386450 dbnd-gcp-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      801 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.379449 dbnd-gcp-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.381449 dbnd-gcp-1.0.8.1/src/dbnd_gcp/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.383450 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2566 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/apache_beam_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/apache_beam_task.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/local_apache_beam.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/big_query.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.384450 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/dataflow.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/dataflow_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.384450 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/dataproc.py
--rw-rw-rw-   0 root         (0) root         (0)     4697 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/dataproc_config.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.384450 dbnd-gcp-1.0.8.1/src/dbnd_gcp/fs/
--rw-rw-rw-   0 root         (0) root         (0)      254 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/fs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18612 2022-11-22 15:16:09.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp/fs/gcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:22.382449 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      895 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      218 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-22 15:16:22.000000 dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.186662 dbnd-gcp-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 16:26:46.187662 dbnd-gcp-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:46.188662 dbnd-gcp-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      801 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.180661 dbnd-gcp-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.182661 dbnd-gcp-1.0.9.1/src/dbnd_gcp/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.185662 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/apache_beam_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/apache_beam_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/local_apache_beam.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/big_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.185662 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/dataflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/dataflow_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.186662 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/dataproc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/dataproc_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.186662 dbnd-gcp-1.0.9.1/src/dbnd_gcp/fs/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/fs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18612 2022-11-22 16:26:26.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp/fs/gcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:46.184662 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      895 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      218 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-22 16:26:46.000000 dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/top_level.txt
```

### Comparing `dbnd-gcp-1.0.8.1/LICENSE` & `dbnd-gcp-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/PKG-INFO` & `dbnd-gcp-1.0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-gcp
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

### Comparing `dbnd-gcp-1.0.8.1/setup.cfg` & `dbnd-gcp-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-gcp-1.0.8.1/setup.py` & `dbnd-gcp-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/_plugin.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/apache_beam_ctrl.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/apache_beam_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/apache_beam/apache_beam_task.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/apache_beam/apache_beam_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/credentials.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/dataflow.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/dataflow.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataflow/dataflow_config.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataflow/dataflow_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/dataproc.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/dataproc.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/dataproc/dataproc_config.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/dataproc/dataproc_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp/fs/gcs.py` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp/fs/gcs.py`

 * *Files identical despite different names*

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/PKG-INFO` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-gcp
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

### Comparing `dbnd-gcp-1.0.8.1/src/dbnd_gcp.egg-info/SOURCES.txt` & `dbnd-gcp-1.0.9.1/src/dbnd_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

