# Comparing `tmp/rdfind2-0.0.0.tar.gz` & `tmp/rdfind2-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.0.tar", last modified: Sun May 28 00:14:38 2023, max compression
+gzip compressed data, was "rdfind2-0.0.1.tar", last modified: Sun May 28 00:22:31 2023, max compression
```

## Comparing `rdfind2-0.0.0.tar` & `rdfind2-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:14:38.943853 rdfind2-0.0.0/
--rw-rw-rw-   0        0        0      846 2023-05-28 00:14:38.943853 rdfind2-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-28 00:08:10.000000 rdfind2-0.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 00:14:38.942853 rdfind2-0.0.0/rdfind2.egg-info/
--rw-rw-rw-   0        0        0      846 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:14:38.000000 rdfind2-0.0.0/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7269 2023-05-28 00:04:30.000000 rdfind2-0.0.0/rdfind2.py
--rw-rw-rw-   0        0        0      533 2023-05-28 00:09:55.000000 rdfind2-0.0.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 00:14:38.944854 rdfind2-0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 00:22:31.639752 rdfind2-0.0.1/
+-rw-rw-rw-   0        0        0      900 2023-05-28 00:22:31.638752 rdfind2-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-28 00:22:22.000000 rdfind2-0.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-28 00:22:31.637750 rdfind2-0.0.1/rdfind2.egg-info/
+-rw-rw-rw-   0        0        0      900 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7269 2023-05-28 00:04:30.000000 rdfind2-0.0.1/rdfind2.py
+-rw-rw-rw-   0        0        0      533 2023-05-28 00:09:55.000000 rdfind2-0.0.1/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 00:22:31.639752 rdfind2-0.0.1/setup.cfg
```

### Comparing `rdfind2-0.0.0/PKG-INFO` & `rdfind2-0.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.0
+Version: 0.0.1
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pdf
 Provides-Extra: rest
 
 # rdfind2
 
 [![](https://img.shields.io/pypi/v/rdfind2.svg)](https://pypi.python.org/pypi/rdfind2)
```

### Comparing `rdfind2-0.0.0/rdfind2.egg-info/PKG-INFO` & `rdfind2-0.0.1/rdfind2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.0
+Version: 0.0.1
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pdf
 Provides-Extra: rest
 
 # rdfind2
 
 [![](https://img.shields.io/pypi/v/rdfind2.svg)](https://pypi.python.org/pypi/rdfind2)
```

### Comparing `rdfind2-0.0.0/rdfind2.py` & `rdfind2-0.0.1/rdfind2.py`

 * *Files identical despite different names*

### Comparing `rdfind2-0.0.0/readme.md` & `rdfind2-0.0.1/readme.md`

 * *Files identical despite different names*

