# Comparing `tmp/bahire-hasab-0.2.1.tar.gz` & `tmp/bahire_hasab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.1.tar", last modified: Sun May 28 10:35:05 2023, max compression
+gzip compressed data, was "bahire_hasab-0.2.2.tar", last modified: Sun May 28 10:44:44 2023, max compression
```

## Comparing `bahire-hasab-0.2.1.tar` & `bahire_hasab-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/bahire-hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/src/bahire-hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:44:44.319312 bahire_hasab-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:44:31.000000 bahire_hasab-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:44:44.319312 bahire_hasab-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:44:31.000000 bahire_hasab-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:44:31.000000 bahire_hasab-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:44:44.319312 bahire_hasab-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:44:31.000000 bahire_hasab-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:44:44.315312 bahire_hasab-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:44:44.319312 bahire_hasab-0.2.2/src/bahire-hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-28 10:44:31.000000 bahire_hasab-0.2.2/src/bahire-hasab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:44:44.319312 bahire_hasab-0.2.2/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:44:44.000000 bahire_hasab-0.2.2/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:44:44.000000 bahire_hasab-0.2.2/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:44:44.000000 bahire_hasab-0.2.2/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:44:44.000000 bahire_hasab-0.2.2/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.1/LICENSE` & `bahire_hasab-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.1/PKG-INFO` & `bahire_hasab-0.2.2/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.2 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.1/README.md` & `bahire_hasab-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.1/src/bahire-hasab/__init__.py` & `bahire_hasab-0.2.2/src/bahire-hasab/__init__.py`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.1/src/bahire_hasab.egg-info/PKG-INFO` & `bahire_hasab-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bahire-hasab
-Version: 0.2.1
+Name: bahire_hasab
+Version: 0.2.2
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: bahire_hasab Version: 0.2.2 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

