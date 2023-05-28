# Comparing `tmp/robotframework_jsonquery-1.0.0.tar.gz` & `tmp/robotframework_jsonquery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_jsonquery-1.0.0.tar", max compression
+gzip compressed data, was "robotframework_jsonquery-1.0.1.tar", max compression
```

## Comparing `robotframework_jsonquery-1.0.0.tar` & `robotframework_jsonquery-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1665 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/JsonQuery.py
--rw-r--r--   0        0        0       33 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/__init__.py
--rw-r--r--   0        0        0      213 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/errors.py
--rw-r--r--   0        0        0      242 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/module_importer.py
--rw-r--r--   0        0        0      713 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/queries.py
--rw-r--r--   0        0        0     1063 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/LICENSE
--rw-r--r--   0        0        0      895 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/README.md
--rw-r--r--   0        0        0      507 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1665 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/JsonQuery.py
+-rw-r--r--   0        0        0       33 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/errors.py
+-rw-r--r--   0        0        0      242 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/module_importer.py
+-rw-r--r--   0        0        0      713 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/JsonQuery/queries.py
+-rw-r--r--   0        0        0     1063 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/LICENSE
+-rw-r--r--   0        0        0      895 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/README.md
+-rw-r--r--   0        0        0      507 2023-05-28 09:33:54.916293 robotframework_jsonquery-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.1/PKG-INFO
```

### Comparing `robotframework_jsonquery-1.0.0/JsonQuery/JsonQuery.py` & `robotframework_jsonquery-1.0.1/JsonQuery/JsonQuery.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.0/JsonQuery/queries.py` & `robotframework_jsonquery-1.0.1/JsonQuery/queries.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.0/LICENSE` & `robotframework_jsonquery-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.0/README.md` & `robotframework_jsonquery-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-1.0.0/PKG-INFO` & `robotframework_jsonquery-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: robotframework-jsonquery
-Version: 1.0.0
+Version: 1.0.1
 Summary: Robot Framework library for parsing json files
 License: MIT
 Author: tom bsc
 Author-email: etombsc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jmespath (<2)
 Requires-Dist: jsonpath_ng (<2)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: robotframework
 Description-Content-Type: text/markdown
 
 # robotframework-jsonquery [![tests](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml/badge.svg?branch=master)](https://github.com/otemek/robotframework-jsonquery/actions/workflows/robotlib.yml)
 Simple wrapper for libraries used to query json files with different query language implementations
 - jsonpath-ng.ext (extended version with e.g. filters)
 - jsonpath-ng
```

