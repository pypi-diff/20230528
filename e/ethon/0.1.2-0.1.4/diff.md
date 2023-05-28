# Comparing `tmp/ethon-0.1.2.tar.gz` & `tmp/ethon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethon-0.1.2.tar", last modified: Thu Mar  9 16:18:25 2023, max compression
+gzip compressed data, was "ethon-0.1.4.tar", last modified: Sun May 28 06:45:11 2023, max compression
```

## Comparing `ethon-0.1.2.tar` & `ethon-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:18:25.730457 ethon-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-09 16:18:17.000000 ethon-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-09 16:18:25.730457 ethon-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-09 16:18:17.000000 ethon-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:18:25.730457 ethon-0.1.2/ethon/
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/FasterTg.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/mystarts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/pyfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/telefunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/teleutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-09 16:18:17.000000 ethon-0.1.2/ethon/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:18:25.730457 ethon-0.1.2/ethon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-09 16:18:25.000000 ethon-0.1.2/ethon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-09 16:18:25.000000 ethon-0.1.2/ethon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:18:25.000000 ethon-0.1.2/ethon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 16:18:25.000000 ethon-0.1.2/ethon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-09 16:18:25.000000 ethon-0.1.2/ethon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-09 16:18:25.730457 ethon-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-09 16:18:17.000000 ethon-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:45:11.145105 ethon-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 06:44:54.000000 ethon-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-28 06:45:11.145105 ethon-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-28 06:44:54.000000 ethon-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:45:11.145105 ethon-0.1.4/ethon/
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/FasterTg.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/mystarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/pyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/telefunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/teleutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-28 06:44:54.000000 ethon-0.1.4/ethon/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:45:11.145105 ethon-0.1.4/ethon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-28 06:45:11.000000 ethon-0.1.4/ethon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-28 06:45:11.000000 ethon-0.1.4/ethon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 06:45:11.000000 ethon-0.1.4/ethon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-28 06:45:11.000000 ethon-0.1.4/ethon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 06:45:11.000000 ethon-0.1.4/ethon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 06:45:11.145105 ethon-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-28 06:44:54.000000 ethon-0.1.4/setup.py
```

### Comparing `ethon-0.1.2/LICENSE.txt` & `ethon-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/PKG-INFO` & `ethon-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethon
-Version: 0.1.2
+Version: 0.1.4
 Summary: Package containing basic functions to build telegram bots.
 Home-page: https://github.com/vasusen-code/ethon
 Author: vasusen-code
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ethon-0.1.2/README.rst` & `ethon-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/FasterTg.py` & `ethon-0.1.4/ethon/FasterTg.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/mystarts.py` & `ethon-0.1.4/ethon/mystarts.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/pyutils.py` & `ethon-0.1.4/ethon/pyutils.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/telefunc.py` & `ethon-0.1.4/ethon/telefunc.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/teleutils.py` & `ethon-0.1.4/ethon/teleutils.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon/uploader.py` & `ethon-0.1.4/ethon/uploader.py`

 * *Files identical despite different names*

### Comparing `ethon-0.1.2/ethon.egg-info/PKG-INFO` & `ethon-0.1.4/ethon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethon
-Version: 0.1.2
+Version: 0.1.4
 Summary: Package containing basic functions to build telegram bots.
 Home-page: https://github.com/vasusen-code/ethon
 Author: vasusen-code
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ethon-0.1.2/setup.py` & `ethon-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import os
 import setuptools
 
-ver = 'v0.1.2'
+ver = 'v0.1.4'
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 desc = "Package containing basic functions to build telegram bots."
 GPL = "GNU AFFERO GENERAL PUBLIC LICENSE (v3)"
 git = "https://github.com/vasusen-code/ethon"
```

