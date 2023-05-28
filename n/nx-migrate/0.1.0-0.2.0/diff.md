# Comparing `tmp/nx_migrate-0.1.0.tar.gz` & `tmp/nx_migrate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx_migrate-0.1.0.tar", max compression
+gzip compressed data, was "nx_migrate-0.2.0.tar", max compression
```

## Comparing `nx_migrate-0.1.0.tar` & `nx_migrate-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-05-28 04:39:22.212999 nx_migrate-0.1.0/LICENSE
--rw-r--r--   0        0        0      168 2023-05-28 04:39:22.235175 nx_migrate-0.1.0/README.md
--rw-r--r--   0        0        0       19 2023-05-28 04:39:22.234992 nx_migrate-0.1.0/nx_migrate/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-28 04:51:01.867027 nx_migrate-0.1.0/nx_migrate/nx_migrate.py
--rw-r--r--   0        0        0      425 2023-05-28 04:48:12.431947 nx_migrate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 nx_migrate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-28 04:39:22.212999 nx_migrate-0.2.0/LICENSE
+-rw-r--r--   0        0        0      168 2023-05-28 04:39:22.235175 nx_migrate-0.2.0/README.md
+-rw-r--r--   0        0        0       19 2023-05-28 04:39:22.234992 nx_migrate-0.2.0/nx_migrate/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-28 04:51:01.867027 nx_migrate-0.2.0/nx_migrate/nx_migrate.py
+-rw-r--r--   0        0        0      481 2023-05-28 05:00:49.874893 nx_migrate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 nx_migrate-0.2.0/PKG-INFO
```

### Comparing `nx_migrate-0.1.0/LICENSE` & `nx_migrate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nx_migrate-0.1.0/nx_migrate/nx_migrate.py` & `nx_migrate-0.2.0/nx_migrate/nx_migrate.py`

 * *Files identical despite different names*

### Comparing `nx_migrate-0.1.0/PKG-INFO` & `nx_migrate-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nx-migrate
-Version: 0.1.0
+Version: 0.2.0
 Summary: call nx migrate anywhere
+Home-page: https://github.com/time4Wiley/nx.migrate
 License: MIT
 Author: Wei Sun
 Author-email: sunwei415@126.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Project-URL: Repository, https://github.com/time4Wiley/nx.migrate
 Description-Content-Type: text/markdown
 
 # nx_migrate Package
 
 This is a generated package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
```

