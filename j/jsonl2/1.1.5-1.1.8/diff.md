# Comparing `tmp/jsonl2-1.1.5.tar.gz` & `tmp/jsonl2-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonl2-1.1.5.tar", last modified: Sun May 28 07:49:11 2023, max compression
+gzip compressed data, was "jsonl2-1.1.8.tar", last modified: Sun May 28 08:30:32 2023, max compression
```

## Comparing `jsonl2-1.1.5.tar` & `jsonl2-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:49:11.952375 jsonl2-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-28 07:49:00.000000 jsonl2-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 07:49:11.952375 jsonl2-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 07:49:00.000000 jsonl2-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-28 07:49:00.000000 jsonl2-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 07:49:11.952375 jsonl2-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:49:11.948375 jsonl2-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:49:11.948375 jsonl2-1.1.5/src/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 07:49:00.000000 jsonl2-1.1.5/src/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-28 07:49:00.000000 jsonl2-1.1.5/src/jsonl/jsonl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:49:11.952375 jsonl2-1.1.5/src/jsonl2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 07:49:11.000000 jsonl2-1.1.5/src/jsonl2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 07:49:11.000000 jsonl2-1.1.5/src/jsonl2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 07:49:11.000000 jsonl2-1.1.5/src/jsonl2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 07:49:11.000000 jsonl2-1.1.5/src/jsonl2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 07:49:11.000000 jsonl2-1.1.5/src/jsonl2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:30:32.991236 jsonl2-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-28 08:30:24.000000 jsonl2-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 08:30:32.991236 jsonl2-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 08:30:24.000000 jsonl2-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-28 08:30:24.000000 jsonl2-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 08:30:32.991236 jsonl2-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:30:32.991236 jsonl2-1.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:30:32.991236 jsonl2-1.1.8/src/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 08:30:24.000000 jsonl2-1.1.8/src/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-28 08:30:24.000000 jsonl2-1.1.8/src/jsonl/jsonl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:30:32.991236 jsonl2-1.1.8/src/jsonl2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 08:30:32.000000 jsonl2-1.1.8/src/jsonl2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 08:30:32.000000 jsonl2-1.1.8/src/jsonl2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 08:30:32.000000 jsonl2-1.1.8/src/jsonl2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 08:30:32.000000 jsonl2-1.1.8/src/jsonl2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 08:30:32.000000 jsonl2-1.1.8/src/jsonl2.egg-info/top_level.txt
```

### Comparing `jsonl2-1.1.5/LICENSE` & `jsonl2-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.5/PKG-INFO` & `jsonl2-1.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2
-Version: 1.1.5
+Version: 1.1.8
 Summary: Json line library
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `jsonl2-1.1.5/README.md` & `jsonl2-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.5/src/jsonl/jsonl.py` & `jsonl2-1.1.8/src/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.5/src/jsonl2.egg-info/PKG-INFO` & `jsonl2-1.1.8/src/jsonl2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2
-Version: 1.1.5
+Version: 1.1.8
 Summary: Json line library
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

