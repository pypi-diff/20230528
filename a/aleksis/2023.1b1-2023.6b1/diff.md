# Comparing `tmp/aleksis-2023.1b1.tar.gz` & `tmp/aleksis-2023.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis-2023.1b1.tar", max compression
+gzip compressed data, was "aleksis-2023.6b1.tar", max compression
```

## Comparing `aleksis-2023.1b1.tar` & `aleksis-2023.6b1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     6489 2023-03-09 21:51:30.938247 aleksis-2023.1b1/README.rst
--rw-r--r--   0        0        0        0 2023-03-09 21:51:30.938247 aleksis-2023.1b1/aleksis_meta/__init__.py
--rw-r--r--   0        0        0     1318 2023-03-09 21:51:30.938247 aleksis-2023.1b1/pyproject.toml
--rw-r--r--   0        0        0     7664 1970-01-01 00:00:00.000000 aleksis-2023.1b1/setup.py
--rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 aleksis-2023.1b1/PKG-INFO
+-rw-r--r--   0        0        0     6489 2023-05-28 12:04:44.365658 aleksis-2023.6b1/README.rst
+-rw-r--r--   0        0        0        0 2023-05-28 12:04:44.365658 aleksis-2023.6b1/aleksis_meta/__init__.py
+-rw-r--r--   0        0        0     1296 2023-05-28 12:22:47.072994 aleksis-2023.6b1/pyproject.toml
+-rw-r--r--   0        0        0     8025 1970-01-01 00:00:00.000000 aleksis-2023.6b1/PKG-INFO
```

### Comparing `aleksis-2023.1b1/README.rst` & `aleksis-2023.6b1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis-2023.1b1/pyproject.toml` & `aleksis-2023.6b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS"
-version = "2023.1b1"
+version = "2023.6b1"
 packages = [ { include = "aleksis_meta" } ]
 include = ["LICNECE.rst"]
 readme = "README.rst"
 
 description = "Free School Information System Distribution"
 authors = ["Dominik George <dominik.george@teckids.org>"]
 maintainers = ["Jonathan Weth <wethjo@katharineum.de>", "Dominik George <dominik.george@teckids.org>"]
@@ -19,22 +19,22 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Topic :: Education",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = { version = "~3.0b2", extras = ["ldap", "s3", "sentry"]}
-aleksis-app-alsijil = "~3.0b0"
-aleksis-app-chronos = "~3.0b0"
-aleksis-app-csvimport = "~3.0b0"
-aleksis-app-dashboardfeeds = "~3.0b0"
-aleksis-app-hjelp = "~3.0b0"
-aleksis-app-ldap = "~3.0b0"
-aleksis-app-resint = "~3.0b1"
-aleksis-app-untis = "~3.0b0"
-aleksis-app-matrix = "~2.0b0"
-aleksis-app-stoelindeling = "~2.0b0"
+aleksis-core = { version = "~3.0", extras = ["ldap", "s3", "sentry"]}
+aleksis-app-alsijil = "~3.0"
+aleksis-app-chronos = "~3.0"
+aleksis-app-csvimport = "~3.0"
+aleksis-app-dashboardfeeds = "~3.0"
+aleksis-app-hjelp = "~3.0"
+aleksis-app-ldap = "~3.0"
+aleksis-app-resint = "~3.0"
+aleksis-app-untis = "~3.0"
+aleksis-app-matrix = "~2.0"
+aleksis-app-stoelindeling = "~2.0"
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `aleksis-2023.1b1/PKG-INFO` & `aleksis-2023.6b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis
-Version: 2023.1b1
+Version: 2023.6b1
 Summary: Free School Information System Distribution
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -17,25 +17,25 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-app-alsijil (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-chronos (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-csvimport (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-dashboardfeeds (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-hjelp (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-ldap (>=3.0b0,<3.1)
-Requires-Dist: aleksis-app-matrix (>=2.0b0,<2.1)
-Requires-Dist: aleksis-app-resint (>=3.0b1,<3.1)
-Requires-Dist: aleksis-app-stoelindeling (>=2.0b0,<2.1)
-Requires-Dist: aleksis-app-untis (>=3.0b0,<3.1)
-Requires-Dist: aleksis-core[ldap,s3,sentry] (>=3.0b2,<3.1)
+Requires-Dist: aleksis-app-alsijil (>=3.0,<3.1)
+Requires-Dist: aleksis-app-chronos (>=3.0,<3.1)
+Requires-Dist: aleksis-app-csvimport (>=3.0,<3.1)
+Requires-Dist: aleksis-app-dashboardfeeds (>=3.0,<3.1)
+Requires-Dist: aleksis-app-hjelp (>=3.0,<3.1)
+Requires-Dist: aleksis-app-ldap (>=3.0,<3.1)
+Requires-Dist: aleksis-app-matrix (>=2.0,<2.1)
+Requires-Dist: aleksis-app-resint (>=3.0,<3.1)
+Requires-Dist: aleksis-app-stoelindeling (>=2.0,<2.1)
+Requires-Dist: aleksis-app-untis (>=3.0,<3.1)
+Requires-Dist: aleksis-core[ldap,s3,sentry] (>=3.0,<3.1)
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS
 Description-Content-Type: text/x-rst
 
 AlekSIS® — All-libre extensible kit for school information systems
 ==================================================================
 
 What AlekSIS® is
```

