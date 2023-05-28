# Comparing `tmp/pyAGI-1.0.1.tar.gz` & `tmp/pyAGI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAGI-1.0.1.tar", last modified: Sun May 28 13:38:15 2023, max compression
+gzip compressed data, was "pyAGI-1.0.2.tar", last modified: Sun May 28 13:48:22 2023, max compression
```

## Comparing `pyAGI-1.0.1.tar` & `pyAGI-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.129948 pyAGI-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:38:04.000000 pyAGI-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:38:15.129948 pyAGI-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-28 13:38:04.000000 pyAGI-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.125947 pyAGI-1.0.1/pyAGI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/pyAGIChainGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/pyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.129948 pyAGI-1.0.1/pyAGI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:38:15.129948 pyAGI-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-28 13:38:04.000000 pyAGI-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.502799 pyAGI-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:48:13.000000 pyAGI-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:48:22.498799 pyAGI-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-28 13:48:13.000000 pyAGI-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.498799 pyAGI-1.0.2/pyAGI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/pyAGIChainGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/pyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.498799 pyAGI-1.0.2/pyAGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:48:22.502799 pyAGI-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-28 13:48:13.000000 pyAGI-1.0.2/setup.py
```

### Comparing `pyAGI-1.0.1/LICENSE` & `pyAGI-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.1/PKG-INFO` & `pyAGI-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAGI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Autonomous agent for building the python app using OpenAI with AGI concept
 Home-page: https://github.com/sattyamjjain/pyAGI
 Author: Sattyam Jain
 Author-email: sattyamjain96@gmail.com
 Project-URL: Bug Reports, https://github.com/sattyamjjain/pyAGI
 Project-URL: Source, https://github.com/sattyamjjain/pyAGI
 Keywords: agi,pyagi,autonomous agent,code agi,python agi
```

### Comparing `pyAGI-1.0.1/README.md` & `pyAGI-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.1/pyAGI/prompts.py` & `pyAGI-1.0.2/pyAGI/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple
 
-from utils import setup_logger, log_header
+from pyAGI.utils import setup_logger, log_header
 
 logger = setup_logger(__name__)
 
 CHAIN_GENERATOR_PROMPT = """
             You are code generation AI proficient in Python.\n
             Your task is to build a '{objective}' console-based Python app.\n 
             {maincontent}.\n
```

### Comparing `pyAGI-1.0.1/pyAGI/pyAGIChainGenerator.py` & `pyAGI-1.0.2/pyAGI/pyAGIChainGenerator.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.1/pyAGI/pyagi.py` & `pyAGI-1.0.2/pyAGI/pyagi.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.1/pyAGI/utils.py` & `pyAGI-1.0.2/pyAGI/utils.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.1/pyAGI.egg-info/PKG-INFO` & `pyAGI-1.0.2/pyAGI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAGI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Autonomous agent for building the python app using OpenAI with AGI concept
 Home-page: https://github.com/sattyamjjain/pyAGI
 Author: Sattyam Jain
 Author-email: sattyamjain96@gmail.com
 Project-URL: Bug Reports, https://github.com/sattyamjjain/pyAGI
 Project-URL: Source, https://github.com/sattyamjjain/pyAGI
 Keywords: agi,pyagi,autonomous agent,code agi,python agi
```

### Comparing `pyAGI-1.0.1/setup.py` & `pyAGI-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyAGI",
-    version="1.0.1",
+    version="1.0.2",
     author="Sattyam Jain",
     author_email="sattyamjain96@gmail.com",
     description="Autonomous agent for building the python app using OpenAI with AGI concept",
     url="https://github.com/sattyamjjain/pyAGI",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

