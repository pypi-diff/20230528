# Comparing `tmp/pers-0.1.2.tar.gz` & `tmp/pers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pers-0.1.2.tar", last modified: Mon May 15 19:49:46 2023, max compression
+gzip compressed data, was "pers-0.1.3.tar", last modified: Sun May 28 10:08:49 2023, max compression
```

## Comparing `pers-0.1.2.tar` & `pers-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.703617 pers-0.1.2/
--rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.2/LICENSE
--rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-15 19:49:46.703617 pers-0.1.2/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)     2983 2023-05-15 19:47:59.000000 pers-0.1.2/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.701617 pers-0.1.2/pers/
--rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.2/pers/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     3580 2023-05-15 19:41:34.000000 pers-0.1.2/pers/pers.py
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-15 19:49:33.000000 pers-0.1.2/pers/version.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.702617 pers-0.1.2/pers.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      217 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/requires.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-15 19:49:46.703617 pers-0.1.2/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.2/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/
+-rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.3/LICENSE
+-rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-28 10:08:49.774864 pers-0.1.3/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)     2983 2023-05-15 19:47:59.000000 pers-0.1.3/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.773864 pers-0.1.3/pers/
+-rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.3/pers/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     5758 2023-05-28 10:04:18.000000 pers-0.1.3/pers/pers.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-28 08:15:19.000000 pers-0.1.3/pers/version.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/pers.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      232 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/requires.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-28 10:08:49.774864 pers-0.1.3/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.3/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/tests/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3254 2023-05-28 09:19:46.000000 pers-0.1.3/tests/tests.py
```

### Comparing `pers-0.1.2/LICENSE` & `pers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pers-0.1.2/PKG-INFO` & `pers-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.2
+Version: 0.1.3
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `pers-0.1.2/README.md` & `pers-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pers-0.1.2/pers.egg-info/PKG-INFO` & `pers-0.1.3/pers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.2
+Version: 0.1.3
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `pers-0.1.2/setup.py` & `pers-0.1.3/setup.py`

 * *Files identical despite different names*

