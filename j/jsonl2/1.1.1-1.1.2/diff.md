# Comparing `tmp/jsonl2-1.1.1.tar.gz` & `tmp/jsonl2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonl2-1.1.1.tar", last modified: Sun May 28 03:42:37 2023, max compression
+gzip compressed data, was "jsonl2-1.1.2.tar", last modified: Sun May 28 07:14:45 2023, max compression
```

## Comparing `jsonl2-1.1.1.tar` & `jsonl2-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-05-28 03:42:37.518227 jsonl2-1.1.1/
--rw-r--r--   0 pedro      (501) staff       (20)     1035 2023-05-28 03:31:06.000000 jsonl2-1.1.1/LICENSE
--rw-r--r--   0 pedro      (501) staff       (20)     1432 2023-05-28 03:42:37.518131 jsonl2-1.1.1/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)     1071 2023-05-28 03:31:06.000000 jsonl2-1.1.1/README.md
--rw-r--r--   0 pedro      (501) staff       (20)      484 2023-05-28 03:41:52.000000 jsonl2-1.1.1/pyproject.toml
--rw-r--r--   0 pedro      (501) staff       (20)       38 2023-05-28 03:42:37.518262 jsonl2-1.1.1/setup.cfg
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-05-28 03:42:37.516902 jsonl2-1.1.1/src/
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-05-28 03:42:37.517415 jsonl2-1.1.1/src/jsonl/
--rw-r--r--   0 pedro      (501) staff       (20)       22 2023-05-28 03:31:06.000000 jsonl2-1.1.1/src/jsonl/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     4934 2023-05-28 03:31:06.000000 jsonl2-1.1.1/src/jsonl/jsonl.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2023-05-28 03:42:37.517940 jsonl2-1.1.1/src/jsonl2.egg-info/
--rw-r--r--   0 pedro      (501) staff       (20)     1432 2023-05-28 03:42:37.000000 jsonl2-1.1.1/src/jsonl2.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)      242 2023-05-28 03:42:37.000000 jsonl2-1.1.1/src/jsonl2.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (501) staff       (20)        1 2023-05-28 03:42:37.000000 jsonl2-1.1.1/src/jsonl2.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (501) staff       (20)       16 2023-05-28 03:42:37.000000 jsonl2-1.1.1/src/jsonl2.egg-info/requires.txt
--rw-r--r--   0 pedro      (501) staff       (20)        6 2023-05-28 03:42:37.000000 jsonl2-1.1.1/src/jsonl2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:14:45.534072 jsonl2-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-28 07:14:31.000000 jsonl2-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 07:14:45.534072 jsonl2-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 07:14:31.000000 jsonl2-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-28 07:14:31.000000 jsonl2-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 07:14:45.534072 jsonl2-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:14:45.530072 jsonl2-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:14:45.534072 jsonl2-1.1.2/src/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 07:14:31.000000 jsonl2-1.1.2/src/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-28 07:14:31.000000 jsonl2-1.1.2/src/jsonl/jsonl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 07:14:45.534072 jsonl2-1.1.2/src/jsonl2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-28 07:14:45.000000 jsonl2-1.1.2/src/jsonl2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 07:14:45.000000 jsonl2-1.1.2/src/jsonl2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 07:14:45.000000 jsonl2-1.1.2/src/jsonl2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 07:14:45.000000 jsonl2-1.1.2/src/jsonl2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 07:14:45.000000 jsonl2-1.1.2/src/jsonl2.egg-info/top_level.txt
```

### Comparing `jsonl2-1.1.1/LICENSE` & `jsonl2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.1/PKG-INFO` & `jsonl2-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Json line library
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `jsonl2-1.1.1/README.md` & `jsonl2-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.1/src/jsonl/jsonl.py` & `jsonl2-1.1.2/src/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `jsonl2-1.1.1/src/jsonl2.egg-info/PKG-INFO` & `jsonl2-1.1.2/src/jsonl2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Json line library
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

