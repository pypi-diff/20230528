# Comparing `tmp/erutils-1.3.2.tar.gz` & `tmp/erutils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erutils-1.3.2.tar", last modified: Sun Apr 16 07:20:45 2023, max compression
+gzip compressed data, was "erutils-1.4.0.tar", last modified: Sun May 28 12:49:01 2023, max compression
```

## Comparing `erutils-1.3.2.tar` & `erutils-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.074921 erutils-1.3.2/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-16 07:20:45.074921 erutils-1.3.2/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2287 2023-04-16 07:20:29.000000 erutils-1.3.2/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.070922 erutils-1.3.2/erutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      601 2023-04-15 14:09:00.000000 erutils-1.3.2/erutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      160 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/__main__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       67 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    32172 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/lightning.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3379 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/loggers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    47142 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/nn.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12973 2023-04-15 14:07:54.000000 erutils-1.3.2/erutils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.074921 erutils-1.3.2/erutils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      316 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      120 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      576 2023-04-15 14:06:10.000000 erutils-1.3.2/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-04-16 07:20:45.074921 erutils-1.3.2/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1272 2023-04-16 07:20:29.000000 erutils-1.3.2/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-28 12:49:01.788319 erutils-1.4.0/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-05-28 12:49:01.788319 erutils-1.4.0/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2287 2023-05-28 12:43:29.000000 erutils-1.4.0/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-28 12:49:01.788319 erutils-1.4.0/erutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      601 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      160 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/__main__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       67 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8238 2023-05-28 12:48:36.000000 erutils-1.4.0/erutils/flax_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    32172 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/lightning.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3379 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/loggers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    47142 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/nn.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12973 2023-05-28 12:43:29.000000 erutils-1.4.0/erutils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-28 12:49:01.788319 erutils-1.4.0/erutils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-05-28 12:49:01.000000 erutils-1.4.0/erutils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      338 2023-05-28 12:49:01.000000 erutils-1.4.0/erutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-05-28 12:49:01.000000 erutils-1.4.0/erutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      113 2023-05-28 12:49:01.000000 erutils-1.4.0/erutils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-05-28 12:49:01.000000 erutils-1.4.0/erutils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      583 2023-05-28 12:48:36.000000 erutils-1.4.0/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-05-28 12:49:01.788319 erutils-1.4.0/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1265 2023-05-28 12:48:36.000000 erutils-1.4.0/setup.py
```

### Comparing `erutils-1.3.2/PKG-INFO` & `erutils-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erutils
-Version: 1.3.2
+Version: 1.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erutils-1.3.2/README.md` & `erutils-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils/__init__.py` & `erutils-1.4.0/erutils/__init__.py`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils/lightning.py` & `erutils-1.4.0/erutils/lightning.py`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils/loggers.py` & `erutils-1.4.0/erutils/loggers.py`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils/nn.py` & `erutils-1.4.0/erutils/nn.py`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils/utils.py` & `erutils-1.4.0/erutils/utils.py`

 * *Files identical despite different names*

### Comparing `erutils-1.3.2/erutils.egg-info/PKG-INFO` & `erutils-1.4.0/erutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erutils
-Version: 1.3.2
+Version: 1.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erutils-1.3.2/pyproject.toml` & `erutils-1.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
-requires = ["setuptools>=46.4.0", "wheel>=0.34.2", "torch>=1.13.0"]
+requires = ["setuptools>=46.4.0", "wheel>=0.34.2", "torch"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 88
 target-version = ["py36", "py37", "py38", "py39", "py310"]
 
 [tool.isort]
 line_length = 88
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
-known_third_party = ["torch"]
+known_third_party = ["torch", 'jax', 'flax']
 
 [tool.flake8]
 max-line-length = 88
 [tool.poetry]
 # other poetry parameters...
 readme = "README.md"
 [tool.mypy]
```

### Comparing `erutils-1.3.2/setup.py` & `erutils-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="erutils",
-    version='1.3.2',
+    version='1.4.0',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
         'numpy',
         'torchvision>=1.13.0',
         'numba',
         'nltk',
         'pandas',
         'json5',
         'PyYAML',
-        'torchtext>=0.9.0',
+        'torchtext',
         'torchaudio>=0.9.0',
         'onnxruntime',
         'thop',
         'matplotlib'
     ],
     python_requires=">=3.6, <3.11",
     license='Apache License 2.0',
```

