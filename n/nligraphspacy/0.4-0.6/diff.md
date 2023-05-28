# Comparing `tmp/NLIGraphSpacy-0.4.tar.gz` & `tmp/nligraphspacy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NLIGraphSpacy-0.4.tar", last modified: Thu May 25 17:01:41 2023, max compression
+gzip compressed data, was "nligraphspacy-0.6.tar", last modified: Sun May 28 04:42:37 2023, max compression
```

## Comparing `NLIGraphSpacy-0.4.tar` & `nligraphspacy-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:41.034476 NLIGraphSpacy-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 17:01:27.000000 NLIGraphSpacy-0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:01:41.030476 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 17:01:40.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 17:01:41.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:01:40.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:01:40.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 17:01:40.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 17:01:40.000000 NLIGraphSpacy-0.4/NLIGraphSpacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 17:01:41.034476 NLIGraphSpacy-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 17:01:27.000000 NLIGraphSpacy-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:01:41.034476 NLIGraphSpacy-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 17:01:27.000000 NLIGraphSpacy-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:42:37.618638 nligraphspacy-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 04:42:23.000000 nligraphspacy-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 04:42:37.618638 nligraphspacy-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 04:42:23.000000 nligraphspacy-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:42:37.618638 nligraphspacy-0.6/nligraphspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 04:42:37.000000 nligraphspacy-0.6/nligraphspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 04:42:37.618638 nligraphspacy-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-28 04:42:23.000000 nligraphspacy-0.6/setup.py
```

### Comparing `NLIGraphSpacy-0.4/LICENSE` & `nligraphspacy-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NLIGraphSpacy-0.4/setup.py` & `nligraphspacy-0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,33 @@
     long_description = fh.read()
 
 requirements = [
   'spacy'
 ]
 
 setuptools.setup(
-    name="NLIGraphSpacy",
-    version="0.4",
+    name="nligraphspacy",
+    version="0.6",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Knowledge graph using Spacy NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url = 'https://github.com/Vishnunkumar/NLIGraphSpacy/',
+    url = 'https://github.com/Vishnunkumar/nligraphspacy/',
     packages=[
-        'NLIGraphSpacy',
+        'nligraphspacy',
     ],
-    package_dir={'NLIGraphSpacy': 'nligraphspacy'},
+    package_dir={'nligraphspacy': 'nligraphspacy'},
     package_data={
-        'NLIGraphSpacy': ['nligraphspacy/*']
+        'nligraphspacy': ['nligraphspacy/*']
     },
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
-    keywords='nligraphspacy',
+    keywords='spacy nli keywords entities',
     classifiers=(
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
```

