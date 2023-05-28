# Comparing `tmp/robotframework_jsonquery-0.0.1a0.tar.gz` & `tmp/robotframework_jsonquery-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_jsonquery-0.0.1a0.tar", max compression
+gzip compressed data, was "robotframework_jsonquery-1.0.0.tar", max compression
```

## Comparing `robotframework_jsonquery-0.0.1a0.tar` & `robotframework_jsonquery-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1665 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/JsonQuery/JsonQuery.py
--rw-r--r--   0        0        0       33 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/JsonQuery/__init__.py
--rw-r--r--   0        0        0      213 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/JsonQuery/errors.py
--rw-r--r--   0        0        0      242 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/JsonQuery/module_importer.py
--rw-r--r--   0        0        0      713 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/JsonQuery/queries.py
--rw-r--r--   0        0        0     1063 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      895 2023-05-27 10:14:31.102949 robotframework_jsonquery-0.0.1a0/README.md
--rw-r--r--   0        0        0      509 2023-05-28 08:57:30.335413 robotframework_jsonquery-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 robotframework_jsonquery-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1665 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/JsonQuery.py
+-rw-r--r--   0        0        0       33 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/errors.py
+-rw-r--r--   0        0        0      242 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/module_importer.py
+-rw-r--r--   0        0        0      713 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/JsonQuery/queries.py
+-rw-r--r--   0        0        0     1063 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/LICENSE
+-rw-r--r--   0        0        0      895 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/README.md
+-rw-r--r--   0        0        0      507 2023-05-28 09:18:54.704627 robotframework_jsonquery-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 robotframework_jsonquery-1.0.0/PKG-INFO
```

### Comparing `robotframework_jsonquery-0.0.1a0/JsonQuery/JsonQuery.py` & `robotframework_jsonquery-1.0.0/JsonQuery/JsonQuery.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-0.0.1a0/JsonQuery/queries.py` & `robotframework_jsonquery-1.0.0/JsonQuery/queries.py`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-0.0.1a0/LICENSE` & `robotframework_jsonquery-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-0.0.1a0/README.md` & `robotframework_jsonquery-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_jsonquery-0.0.1a0/PKG-INFO` & `robotframework_jsonquery-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-jsonquery
-Version: 0.0.1a0
+Version: 1.0.0
 Summary: Robot Framework library for parsing json files
 License: MIT
 Author: tom bsc
 Author-email: etombsc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

