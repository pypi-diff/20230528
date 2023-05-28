# Comparing `tmp/nx_migrate-0.3.0.tar.gz` & `tmp/nx_migrate-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx_migrate-0.3.0.tar", max compression
+gzip compressed data, was "nx_migrate-0.3.1.tar", max compression
```

## Comparing `nx_migrate-0.3.0.tar` & `nx_migrate-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-05-28 04:39:22.212999 nx_migrate-0.3.0/LICENSE
--rw-r--r--   0        0        0      212 2023-05-28 05:06:37.009689 nx_migrate-0.3.0/README.md
--rw-r--r--   0        0        0       19 2023-05-28 04:39:22.234992 nx_migrate-0.3.0/nx_migrate/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-28 04:51:01.867027 nx_migrate-0.3.0/nx_migrate/nx_migrate.py
--rw-r--r--   0        0        0      481 2023-05-28 05:04:39.125237 nx_migrate-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 nx_migrate-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-28 04:39:22.212999 nx_migrate-0.3.1/LICENSE
+-rw-r--r--   0        0        0      307 2023-05-28 05:13:00.176483 nx_migrate-0.3.1/README.md
+-rw-r--r--   0        0        0       19 2023-05-28 04:39:22.234992 nx_migrate-0.3.1/nx_migrate/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-28 04:51:01.867027 nx_migrate-0.3.1/nx_migrate/nx_migrate.py
+-rw-r--r--   0        0        0      481 2023-05-28 05:13:04.598936 nx_migrate-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 nx_migrate-0.3.1/PKG-INFO
```

### Comparing `nx_migrate-0.3.0/LICENSE` & `nx_migrate-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nx_migrate-0.3.0/nx_migrate/nx_migrate.py` & `nx_migrate-0.3.1/nx_migrate/nx_migrate.py`

 * *Files identical despite different names*

### Comparing `nx_migrate-0.3.0/PKG-INFO` & `nx_migrate-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx-migrate
-Version: 0.3.0
+Version: 0.3.1
 Summary: call nx migrate anywhere
 Home-page: https://github.com/time4Wiley/nx.migrate
 License: MIT
 Author: Wei Sun
 Author-email: sunwei415@126.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/time4Wiley/nx.migrate
 Description-Content-Type: text/markdown
 
-# nx_migrate Package
+# nx-migrate Package
 
 ## installation
 ```
 pip install nx-migrate
 ```
 
+## Notice
+the `nx` command must be available in your `system's PATH` for this script to work.
+
 ## Usage
 - Example on Windows
 ```
 nx-migrate -u "C:\my-monorepo"
 ```
 
 - Example on Linux/macOS
```

