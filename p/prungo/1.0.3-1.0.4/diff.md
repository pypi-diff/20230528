# Comparing `tmp/prungo-1.0.3.tar.gz` & `tmp/prungo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prungo-1.0.3.tar", max compression
+gzip compressed data, was "prungo-1.0.4.tar", max compression
```

## Comparing `prungo-1.0.3.tar` & `prungo-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1497 2023-05-27 15:06:53.831319 prungo-1.0.3/LICENSE
--rw-r--r--   0        0        0       58 2023-05-27 15:06:53.831319 prungo-1.0.3/README.md
--rw-r--r--   0        0        0       77 2023-05-27 15:06:53.831319 prungo-1.0.3/prungo/__init__.py
--rw-r--r--   0        0        0      599 2023-05-27 15:06:53.831319 prungo-1.0.3/prungo/decorators.py
--rw-r--r--   0        0        0      521 2023-05-27 15:06:53.831319 prungo-1.0.3/prungo/models.py
--rw-r--r--   0        0        0      693 2023-05-27 15:07:25.729466 prungo-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 prungo-1.0.3/setup.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 prungo-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-28 12:05:01.469931 prungo-1.0.4/LICENSE
+-rw-r--r--   0        0        0       58 2023-05-28 12:05:01.469931 prungo-1.0.4/README.md
+-rw-r--r--   0        0        0       93 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/decorators.py
+-rw-r--r--   0        0        0      521 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/models.py
+-rw-r--r--   0        0        0      693 2023-05-28 12:05:33.921893 prungo-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 prungo-1.0.4/setup.py
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 prungo-1.0.4/PKG-INFO
```

### Comparing `prungo-1.0.3/LICENSE` & `prungo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prungo-1.0.3/prungo/models.py` & `prungo-1.0.4/prungo/models.py`

 * *Files identical despite different names*

### Comparing `prungo-1.0.3/pyproject.toml` & `prungo-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prungo"
-version = "1.0.3"
+version = "1.0.4"
 description = "A package for basic utility functions/classes"
 authors = ["c-prungo"]
 packages = [{include = "prungo"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/c-prungo/prungo-util"
 repository = "https://github.com/c-prungo/prungo-util"
```

### Comparing `prungo-1.0.3/setup.py` & `prungo-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.8,<2.0.0']
 
 setup_kwargs = {
     'name': 'prungo',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'A package for basic utility functions/classes',
     'long_description': '# prungo-util\nutility package for importing into projects\n',
     'author': 'c-prungo',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/c-prungo/prungo-util',
```

### Comparing `prungo-1.0.3/PKG-INFO` & `prungo-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prungo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for basic utility functions/classes
 Home-page: https://github.com/c-prungo/prungo-util
 License: MIT
 Author: c-prungo
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

