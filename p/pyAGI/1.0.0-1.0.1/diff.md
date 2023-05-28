# Comparing `tmp/pyAGI-1.0.0.tar.gz` & `tmp/pyAGI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAGI-1.0.0.tar", last modified: Sun May 28 13:22:30 2023, max compression
+gzip compressed data, was "pyAGI-1.0.1.tar", last modified: Sun May 28 13:38:15 2023, max compression
```

## Comparing `pyAGI-1.0.0.tar` & `pyAGI-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-05-28 13:22:30.561172 pyAGI-1.0.0/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1069 2023-05-28 13:16:45.000000 pyAGI-1.0.0/LICENSE
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      655 2023-05-28 13:22:30.557172 pyAGI-1.0.0/PKG-INFO
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1567 2023-05-28 13:15:12.000000 pyAGI-1.0.0/README.md
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-05-28 13:22:30.557172 pyAGI-1.0.0/pyAGI/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-05-28 13:07:03.000000 pyAGI-1.0.0/pyAGI/__init__.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     3795 2023-05-28 11:48:25.000000 pyAGI-1.0.0/pyAGI/prompts.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1841 2023-05-28 13:02:39.000000 pyAGI-1.0.0/pyAGI/pyAGIChainGenerator.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     4340 2023-05-28 13:02:56.000000 pyAGI-1.0.0/pyAGI/pyagi.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1162 2023-05-28 11:44:03.000000 pyAGI-1.0.0/pyAGI/utils.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-05-28 13:22:30.557172 pyAGI-1.0.0/pyAGI.egg-info/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      655 2023-05-28 13:22:30.000000 pyAGI-1.0.0/pyAGI.egg-info/PKG-INFO
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      264 2023-05-28 13:22:30.000000 pyAGI-1.0.0/pyAGI.egg-info/SOURCES.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        1 2023-05-28 13:22:30.000000 pyAGI-1.0.0/pyAGI.egg-info/dependency_links.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)       58 2023-05-28 13:22:30.000000 pyAGI-1.0.0/pyAGI.egg-info/requires.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        6 2023-05-28 13:22:30.000000 pyAGI-1.0.0/pyAGI.egg-info/top_level.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)       38 2023-05-28 13:22:30.561172 pyAGI-1.0.0/setup.cfg
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      915 2023-05-28 13:07:05.000000 pyAGI-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.129948 pyAGI-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:38:04.000000 pyAGI-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:38:15.129948 pyAGI-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-28 13:38:04.000000 pyAGI-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.125947 pyAGI-1.0.1/pyAGI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/pyAGIChainGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/pyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-28 13:38:04.000000 pyAGI-1.0.1/pyAGI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:38:15.129948 pyAGI-1.0.1/pyAGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 13:38:15.000000 pyAGI-1.0.1/pyAGI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:38:15.129948 pyAGI-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-28 13:38:04.000000 pyAGI-1.0.1/setup.py
```

### Comparing `pyAGI-1.0.0/LICENSE` & `pyAGI-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/PKG-INFO` & `pyAGI-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAGI
-Version: 1.0.0
+Version: 1.0.1
 Summary: Autonomous agent for building the python app using OpenAI with AGI concept
 Home-page: https://github.com/sattyamjjain/pyAGI
 Author: Sattyam Jain
 Author-email: sattyamjain96@gmail.com
 Project-URL: Bug Reports, https://github.com/sattyamjjain/pyAGI
 Project-URL: Source, https://github.com/sattyamjjain/pyAGI
 Keywords: agi,pyagi,autonomous agent,code agi,python agi
```

### Comparing `pyAGI-1.0.0/README.md` & `pyAGI-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/pyAGI/prompts.py` & `pyAGI-1.0.1/pyAGI/prompts.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/pyAGI/pyAGIChainGenerator.py` & `pyAGI-1.0.1/pyAGI/pyAGIChainGenerator.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/pyAGI/pyagi.py` & `pyAGI-1.0.1/pyAGI/pyagi.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/pyAGI/utils.py` & `pyAGI-1.0.1/pyAGI/utils.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.0/pyAGI.egg-info/PKG-INFO` & `pyAGI-1.0.1/pyAGI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAGI
-Version: 1.0.0
+Version: 1.0.1
 Summary: Autonomous agent for building the python app using OpenAI with AGI concept
 Home-page: https://github.com/sattyamjjain/pyAGI
 Author: Sattyam Jain
 Author-email: sattyamjain96@gmail.com
 Project-URL: Bug Reports, https://github.com/sattyamjjain/pyAGI
 Project-URL: Source, https://github.com/sattyamjjain/pyAGI
 Keywords: agi,pyagi,autonomous agent,code agi,python agi
```

### Comparing `pyAGI-1.0.0/setup.py` & `pyAGI-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyAGI",
-    version="1.0.0",
+    version="1.0.1",
     author="Sattyam Jain",
     author_email="sattyamjain96@gmail.com",
     description="Autonomous agent for building the python app using OpenAI with AGI concept",
     url="https://github.com/sattyamjjain/pyAGI",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

