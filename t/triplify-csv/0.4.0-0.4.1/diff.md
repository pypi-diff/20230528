# Comparing `tmp/triplify_csv-0.4.0.tar.gz` & `tmp/triplify_csv-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.4.0.tar", max compression
+gzip compressed data, was "triplify_csv-0.4.1.tar", max compression
```

## Comparing `triplify_csv-0.4.0.tar` & `triplify_csv-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.4.0/LICENSE
--rw-r--r--   0        0        0     7905 2023-05-11 07:35:24.158330 triplify_csv-0.4.0/README.md
--rw-r--r--   0        0        0      568 2023-05-11 07:37:35.982325 triplify_csv-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.4.0/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    18065 2023-05-10 17:33:25.481276 triplify_csv-0.4.0/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     8702 1970-01-01 00:00:00.000000 triplify_csv-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-05-28 12:11:08.656135 triplify_csv-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7905 2023-05-28 12:11:08.658135 triplify_csv-0.4.1/README.md
+-rw-r--r--   0        0        0      585 2023-05-28 12:19:10.176120 triplify_csv-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-28 12:11:08.739135 triplify_csv-0.4.1/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    18065 2023-05-28 12:11:08.745135 triplify_csv-0.4.1/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 triplify_csv-0.4.1/PKG-INFO
```

### Comparing `triplify_csv-0.4.0/LICENSE` & `triplify_csv-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.4.0/README.md` & `triplify_csv-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.4.0/triplify_csv/triplify_csv.py` & `triplify_csv-0.4.1/triplify_csv/triplify_csv.py`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.4.0/PKG-INFO` & `triplify_csv-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: triplify-csv
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool to generate triples from CSV files according to a configuration file.
 Home-page: https://github.com/AAtley/triplify_csv
 License: BSD-3-Clause
 Author: Adrian Atley
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Requires-Dist: rdflib (==6.3.2)
 Project-URL: Repository, https://github.com/AAtley/triplify_csv
 Description-Content-Type: text/markdown
 
 triplify\_csv
 =============
 
 Features
```

