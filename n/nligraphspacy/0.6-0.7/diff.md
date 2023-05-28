# Comparing `tmp/nligraphspacy-0.6.tar.gz` & `tmp/nligraphspacy-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nligraphspacy-0.6.tar", last modified: Sun May 28 04:42:37 2023, max compression
+gzip compressed data, was "nligraphspacy-0.7.tar", last modified: Sun May 28 10:55:27 2023, max compression
```

## Comparing `nligraphspacy-0.6.tar` & `nligraphspacy-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:42:37.618638 nligraphspacy-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 04:42:23.000000 nligraphspacy-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 04:42:37.618638 nligraphspacy-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 04:42:23.000000 nligraphspacy-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:42:37.618638 nligraphspacy-0.6/nligraphspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 04:42:37.618638 nligraphspacy-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-28 04:42:23.000000 nligraphspacy-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:55:27.822482 nligraphspacy-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 10:55:16.000000 nligraphspacy-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 10:55:27.822482 nligraphspacy-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 10:55:16.000000 nligraphspacy-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:55:27.822482 nligraphspacy-0.7/nligraphspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 10:55:27.000000 nligraphspacy-0.7/nligraphspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:55:27.822482 nligraphspacy-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-28 10:55:16.000000 nligraphspacy-0.7/setup.py
```

### Comparing `nligraphspacy-0.6/LICENSE` & `nligraphspacy-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nligraphspacy-0.6/PKG-INFO` & `nligraphspacy-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 0.6
+Version: 0.7
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nligraphspacy-0.6/nligraphspacy.egg-info/PKG-INFO` & `nligraphspacy-0.7/nligraphspacy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 0.6
+Version: 0.7
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nligraphspacy-0.6/setup.py` & `nligraphspacy-0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 requirements = [
   'spacy'
 ]
 
 setuptools.setup(
     name="nligraphspacy",
-    version="0.6",
+    version="0.7",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Knowledge graph using Spacy NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/nligraphspacy/',
     packages=[
         'nligraphspacy',
     ],
-    package_dir={'nligraphspacy': 'nligraphspacy'},
+    package_dir={'nligraphspacy': 'nligraphspacy/'},
     package_data={
         'nligraphspacy': ['nligraphspacy/*']
     },
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
     keywords='spacy nli keywords entities',
```

