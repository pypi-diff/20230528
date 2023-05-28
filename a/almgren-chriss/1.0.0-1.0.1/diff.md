# Comparing `tmp/almgren_chriss-1.0.0.tar.gz` & `tmp/almgren_chriss-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almgren_chriss-1.0.0.tar", max compression
+gzip compressed data, was "almgren_chriss-1.0.1.tar", max compression
```

## Comparing `almgren_chriss-1.0.0.tar` & `almgren_chriss-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-05-28 08:00:42.739493 almgren_chriss-1.0.0/LICENSE
--rw-r--r--   0        0        0     2102 2023-05-28 08:00:42.739493 almgren_chriss-1.0.0/README.rst
--rw-r--r--   0        0        0     1152 2023-05-28 08:00:42.739493 almgren_chriss-1.0.0/almgren_chriss/__init__.py
--rw-r--r--   0        0        0     3058 2023-05-28 08:00:42.739493 almgren_chriss-1.0.0/almgren_chriss/cost.py
--rw-r--r--   0        0        0     2754 2023-05-28 08:00:42.743493 almgren_chriss-1.0.0/almgren_chriss/decay_rate.py
--rw-r--r--   0        0        0     2528 2023-05-28 08:00:42.743493 almgren_chriss-1.0.0/almgren_chriss/trade.py
--rw-r--r--   0        0        0      820 2023-05-28 08:01:04.519557 almgren_chriss-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 almgren_chriss-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2102 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/README.rst
+-rw-r--r--   0        0        0     1152 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/__init__.py
+-rw-r--r--   0        0        0     3058 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/cost.py
+-rw-r--r--   0        0        0     2754 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/decay_rate.py
+-rw-r--r--   0        0        0     2528 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/trade.py
+-rw-r--r--   0        0        0      836 2023-05-28 21:04:35.590162 almgren_chriss-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 almgren_chriss-1.0.1/PKG-INFO
```

### Comparing `almgren_chriss-1.0.0/LICENSE` & `almgren_chriss-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/README.rst` & `almgren_chriss-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/almgren_chriss/__init__.py` & `almgren_chriss-1.0.1/almgren_chriss/__init__.py`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/almgren_chriss/cost.py` & `almgren_chriss-1.0.1/almgren_chriss/cost.py`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/almgren_chriss/decay_rate.py` & `almgren_chriss-1.0.1/almgren_chriss/decay_rate.py`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/almgren_chriss/trade.py` & `almgren_chriss-1.0.1/almgren_chriss/trade.py`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.0/pyproject.toml` & `almgren_chriss-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "almgren_chriss"
-version = "1.0.0"
+version = "1.0.1"
 description = "functions for implementing the Almgren-Chriss model for optimal execution of portfolio transactions."
 authors = ["Bernardo Paulsen <paulsen.bernardo@gmail.com>"]
 license = "GNU General Public License"
 readme = "README.rst"
 packages = [{ include = "almgren_chriss" }]
 keywords = ["optimal exeuction", "quantitative finance", "Almgren Chriss"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+numpy = '^1.0'
 
 [tool.poetry.urls]
-"GitHub" = "https://github.com/bernardopaulsen/almngre-chriss"
+"GitHub" = "https://github.com/bernardopaulsen/almngren-chriss"
 "Documentation" = "https://bernardopaulsen.github.io/almgren-chriss/"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = 'git'
 format = '{base}'
```

### Comparing `almgren_chriss-1.0.0/PKG-INFO` & `almgren_chriss-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: almgren-chriss
-Version: 1.0.0
+Version: 1.0.1
 Summary: functions for implementing the Almgren-Chriss model for optimal execution of portfolio transactions.
 License: GNU General Public License
 Keywords: optimal exeuction,quantitative finance,Almgren Chriss
 Author: Bernardo Paulsen
 Author-email: paulsen.bernardo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.0,<2.0)
 Project-URL: Documentation, https://bernardopaulsen.github.io/almgren-chriss/
-Project-URL: GitHub, https://github.com/bernardopaulsen/almngre-chriss
+Project-URL: GitHub, https://github.com/bernardopaulsen/almngren-chriss
 Description-Content-Type: text/x-rst
 
 almgren-chriss
 ==============
 
 This package provides functions for implementing the Almgren-Chriss model for optimal execution of portfolio transactions.
```

