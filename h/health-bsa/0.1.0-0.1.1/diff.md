# Comparing `tmp/health_bsa-0.1.0.tar.gz` & `tmp/health_bsa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health_bsa-0.1.0.tar", max compression
+gzip compressed data, was "health_bsa-0.1.1.tar", max compression
```

## Comparing `health_bsa-0.1.0.tar` & `health_bsa-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      480 2023-05-28 10:22:37.086888 health_bsa-0.1.0/README.md
--rw-r--r--   0        0        0       41 2023-05-28 10:00:46.955191 health_bsa-0.1.0/health_bsa/__init__.py
--rw-r--r--   0        0        0      519 2023-05-28 09:53:13.358488 health_bsa-0.1.0/health_bsa/bsa.py
--rw-r--r--   0        0        0      611 2023-05-28 10:26:09.135682 health_bsa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 health_bsa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      480 2023-05-28 10:22:37.086888 health_bsa-0.1.1/README.md
+-rw-r--r--   0        0        0       41 2023-05-28 11:55:18.850774 health_bsa-0.1.1/health_bsa/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-28 11:53:47.296141 health_bsa-0.1.1/health_bsa/bsa.py
+-rw-r--r--   0        0        0      570 2023-05-28 11:55:14.992124 health_bsa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 health_bsa-0.1.1/PKG-INFO
```

### Comparing `health_bsa-0.1.0/pyproject.toml` & `health_bsa-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "health-bsa"
-version = "0.1.0"
+version = "0.1.1"
 description = "This is a small tool to compute Body Surface Area of a human body based on height and weight"
 authors = ["LamNguyen <lamnvcnsh@gmail.com>"]
 readme = "README.md"
 license = "MIT"
-homepage= "https://github.com/lamnvcnsh/health-bsa/tree/main/health-bsa"
-repository = "https://github.com/lamnvcnsh/health-bsa/tree/main/health-bsa"
+homepage= "https://github.com/lamnvcnsh/health-bsa/"
+repository = "https://github.com/lamnvcnsh/health-bsa"
 keywords = ["Body Surface Area", "Health index"]
 
 packages = [{include = "health_bsa"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `health_bsa-0.1.0/PKG-INFO` & `health_bsa-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: health-bsa
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a small tool to compute Body Surface Area of a human body based on height and weight
-Home-page: https://github.com/lamnvcnsh/health-bsa/tree/main/health-bsa
+Home-page: https://github.com/lamnvcnsh/health-bsa/
 License: MIT
 Keywords: Body Surface Area,Health index
 Author: LamNguyen
 Author-email: lamnvcnsh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/lamnvcnsh/health-bsa/tree/main/health-bsa
+Project-URL: Repository, https://github.com/lamnvcnsh/health-bsa
 Description-Content-Type: text/markdown
 
 # Health-BSA
 A small tool to compute the human body surface area from body weight (kg) and height (cm)
 
 
 ### Getting started
```

