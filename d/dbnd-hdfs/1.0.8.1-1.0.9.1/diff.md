# Comparing `tmp/dbnd-hdfs-1.0.8.1.tar.gz` & `tmp/dbnd-hdfs-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-hdfs-1.0.8.1.tar", last modified: Tue Nov 22 15:16:21 2022, max compression
+gzip compressed data, was "dbnd-hdfs-1.0.9.1.tar", last modified: Tue Nov 22 16:26:45 2022, max compression
```

## Comparing `dbnd-hdfs-1.0.8.1.tar` & `dbnd-hdfs-1.0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.798390 dbnd-hdfs-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1449 2022-11-22 15:16:21.799390 dbnd-hdfs-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:21.800390 dbnd-hdfs-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      623 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.795390 dbnd-hdfs-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.796390 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.798390 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/hdfs.py
--rw-rw-rw-   0 root         (0) root         (0)     7814 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/hdfs_hdfscli.py
--rw-rw-rw-   0 root         (0) root         (0)     8360 2022-11-22 15:16:09.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/hdfs_pyox.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.798390 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1449 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       97 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-22 15:16:21.000000 dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:45.326574 dbnd-hdfs-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1449 2022-11-22 16:26:45.326574 dbnd-hdfs-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:45.327574 dbnd-hdfs-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      623 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:45.321573 dbnd-hdfs-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:45.323573 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:45.325574 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/hdfs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7814 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/hdfs_hdfscli.py
+-rw-rw-rw-   0 root         (0) root         (0)     8360 2022-11-22 16:26:26.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/hdfs_pyox.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:45.324574 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1449 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       97 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-11-22 16:26:45.000000 dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/top_level.txt
```

### Comparing `dbnd-hdfs-1.0.8.1/LICENSE` & `dbnd-hdfs-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-hdfs-1.0.8.1/PKG-INFO` & `dbnd-hdfs-1.0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-hdfs
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

### Comparing `dbnd-hdfs-1.0.8.1/setup.cfg` & `dbnd-hdfs-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-hdfs-1.0.8.1/setup.py` & `dbnd-hdfs-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/hdfs_hdfscli.py` & `dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/hdfs_hdfscli.py`

 * *Files identical despite different names*

### Comparing `dbnd-hdfs-1.0.8.1/src/dbnd_hdfs/fs/hdfs_pyox.py` & `dbnd-hdfs-1.0.9.1/src/dbnd_hdfs/fs/hdfs_pyox.py`

 * *Files identical despite different names*

### Comparing `dbnd-hdfs-1.0.8.1/src/dbnd_hdfs.egg-info/PKG-INFO` & `dbnd-hdfs-1.0.9.1/src/dbnd_hdfs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-hdfs
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

