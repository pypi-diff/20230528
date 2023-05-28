# Comparing `tmp/daba-0.0.1.tar.gz` & `tmp/daba-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daba-0.0.1.tar", last modified: Sun May 28 08:07:59 2023, max compression
+gzip compressed data, was "daba-0.0.2.tar", last modified: Sun May 28 15:25:49 2023, max compression
```

## Comparing `daba-0.0.1.tar` & `daba-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 08:07:59.321909 daba-0.0.1/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.1/LICENSE
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      470 2023-05-28 08:07:59.321799 daba-0.0.1/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      143 2023-05-28 07:30:03.000000 daba-0.0.1/README.md
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 08:07:59.320757 daba-0.0.1/daba/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3257 2023-05-28 07:33:46.000000 daba-0.0.1/daba/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.1/daba/__init__.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 08:07:59.321210 daba-0.0.1/daba.egg-info/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      470 2023-05-28 08:07:59.000000 daba-0.0.1/daba.egg-info/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      253 2023-05-28 08:07:59.000000 daba-0.0.1/daba.egg-info/SOURCES.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 08:07:59.000000 daba-0.0.1/daba.egg-info/dependency_links.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 08:07:59.000000 daba-0.0.1/daba.egg-info/top_level.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      553 2023-05-28 08:06:34.000000 daba-0.0.1/pyproject.toml
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 08:07:59.321948 daba-0.0.1/setup.cfg
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      562 2023-05-28 08:06:34.000000 daba-0.0.1/setup.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 08:07:59.321332 daba-0.0.1/tests/
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 08:07:59.321656 daba-0.0.1/tests/Database/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.1/tests/Database/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.1/tests/Database/__init__.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.1/tests/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834774 daba-0.0.2/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.2/LICENSE
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:25:49.834644 daba-0.0.2/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     2821 2023-05-28 15:17:32.000000 daba-0.0.2/README.md
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.833570 daba-0.0.2/daba/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3257 2023-05-28 07:33:46.000000 daba-0.0.2/daba/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.2/daba/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834007 daba-0.0.2/daba.egg-info/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      238 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/SOURCES.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/dependency_links.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/top_level.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 15:25:49.834824 daba-0.0.2/setup.cfg
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      735 2023-05-28 15:22:05.000000 daba-0.0.2/setup.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834120 daba-0.0.2/tests/
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834471 daba-0.0.2/tests/Database/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.2/tests/Database/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.2/tests/Database/__init__.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.2/tests/__init__.py
```

### Comparing `daba-0.0.1/LICENSE` & `daba-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daba-0.0.1/daba/Mongo.py` & `daba-0.0.2/daba/Mongo.py`

 * *Files identical despite different names*

### Comparing `daba-0.0.1/tests/Database/Mongo.py` & `daba-0.0.2/tests/Database/Mongo.py`

 * *Files identical despite different names*

