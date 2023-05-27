# Comparing `tmp/insidepostgresql-0.0.1.tar.gz` & `tmp/insidepostgresql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidepostgresql-0.0.1.tar", last modified: Sat May 27 21:55:01 2023, max compression
+gzip compressed data, was "insidepostgresql-0.0.2.tar", last modified: Sat May 27 21:57:16 2023, max compression
```

## Comparing `insidepostgresql-0.0.1.tar` & `insidepostgresql-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:55:01.131857 insidepostgresql-0.0.1/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-05-27 20:03:17.000000 insidepostgresql-0.0.1/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:55:01.131857 insidepostgresql-0.0.1/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     1661 2023-05-27 21:51:18.000000 insidepostgresql-0.0.1/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)      695 2023-05-27 21:55:01.131857 insidepostgresql-0.0.1/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      936 2023-05-27 21:52:00.000000 insidepostgresql-0.0.1/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:55:01.127857 insidepostgresql-0.0.1/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:55:01.131857 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:55:01.000000 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      311 2023-05-27 21:55:01.000000 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-27 21:55:01.000000 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       27 2023-05-27 21:55:01.000000 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       11 2023-05-27 21:55:01.000000 insidepostgresql-0.0.1/src/insidepostgresql.egg-info/top_level.txt
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:55:01.131857 insidepostgresql-0.0.1/src/postgresql/
--rw-rw-r--   0 demir     (1000) demir     (1000)       25 2023-05-27 20:03:59.000000 insidepostgresql-0.0.1/src/postgresql/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     5363 2023-05-27 21:47:24.000000 insidepostgresql-0.0.1/src/postgresql/postgresql.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-05-27 20:03:17.000000 insidepostgresql-0.0.2/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1661 2023-05-27 21:51:18.000000 insidepostgresql-0.0.2/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)      695 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)      943 2023-05-27 21:57:07.000000 insidepostgresql-0.0.2/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.013189 insidepostgresql-0.0.2/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      311 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       11 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/src/postgresql/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       25 2023-05-27 20:03:59.000000 insidepostgresql-0.0.2/src/postgresql/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5363 2023-05-27 21:47:24.000000 insidepostgresql-0.0.2/src/postgresql/postgresql.py
```

### Comparing `insidepostgresql-0.0.1/LICENSE` & `insidepostgresql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `insidepostgresql-0.0.1/PKG-INFO` & `insidepostgresql-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidepostgresql
-Version: 0.0.1
+Version: 0.0.2
 Summary: Check and analyze a PostgreSQL cluster.
 Home-page: https://github.com/adiosamig/insidepgs
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidepgs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `insidepostgresql-0.0.1/README.md` & `insidepostgresql-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `insidepostgresql-0.0.1/setup.cfg` & `insidepostgresql-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = insidecocuhbase
-version = 0.0.1
+version = 0.0.2
 author = Huseyin Demir
 author_email = huseyin.d3r@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/adiosamig/insidepgs
 project_urls =
```

### Comparing `insidepostgresql-0.0.1/setup.py` & `insidepostgresql-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidepostgresql",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a PostgreSQL cluster.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidepgs",
     install_requires=[
-        'psycopg2',
+        'psycopg2-binary',
         'tabulate',
         'datetime'
     ],
     project_urls = {
         "Bug Tracker": "https://github.com/adiosamig/insidepgs/issues",
     },
     classifiers = [
```

### Comparing `insidepostgresql-0.0.1/src/insidepostgresql.egg-info/PKG-INFO` & `insidepostgresql-0.0.2/src/insidepostgresql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidepostgresql
-Version: 0.0.1
+Version: 0.0.2
 Summary: Check and analyze a PostgreSQL cluster.
 Home-page: https://github.com/adiosamig/insidepgs
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidepgs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `insidepostgresql-0.0.1/src/postgresql/postgresql.py` & `insidepostgresql-0.0.2/src/postgresql/postgresql.py`

 * *Files identical despite different names*

