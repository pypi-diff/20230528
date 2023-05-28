# Comparing `tmp/rigorous_recorder-1.4.1.tar.gz` & `tmp/rigorous_recorder-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.4.1.tar", last modified: Thu May 25 20:56:13 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.4.2.tar", last modified: Sun May 28 15:55:05 2023, max compression
```

## Comparing `rigorous_recorder-1.4.1.tar` & `rigorous_recorder-1.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.321543 rigorous_recorder-1.4.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-25 20:56:13.321283 rigorous_recorder-1.4.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.320345 rigorous_recorder-1.4.1/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    35674 2023-05-25 20:48:40.000000 rigorous_recorder-1.4.1/rigorous_recorder/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:56:13.321134 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-25 20:56:12.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      202 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-05-25 20:56:13.000000 rigorous_recorder-1.4.1/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 20:56:13.321619 rigorous_recorder-1.4.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.492176 rigorous_recorder-1.4.2/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-28 15:55:05.492026 rigorous_recorder-1.4.2/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.490858 rigorous_recorder-1.4.2/rigorous_recorder/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    35674 2023-05-25 20:48:40.000000 rigorous_recorder-1.4.2/rigorous_recorder/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.491852 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      202 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-28 15:55:05.492220 rigorous_recorder-1.4.2/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.2/setup.py
```

### Comparing `rigorous_recorder-1.4.1/PKG-INFO` & `rigorous_recorder-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous_recorder
-Version: 1.4.1
+Version: 1.4.2
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.4.1/rigorous_recorder/__init__.py` & `rigorous_recorder-1.4.2/rigorous_recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `rigorous_recorder-1.4.1/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.4.2/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous-recorder
-Version: 1.4.1
+Version: 1.4.2
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.4.1/setup.py` & `rigorous_recorder-1.4.2/setup.py`

 * *Files identical despite different names*

