# Comparing `tmp/bloxflipeasily-0.0.1.tar.gz` & `tmp/bloxflipeasily-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloxflipeasily-0.0.1.tar", last modified: Mon May 22 23:56:10 2023, max compression
+gzip compressed data, was "bloxflipeasily-0.0.2.tar", last modified: Sun May 28 21:17:35 2023, max compression
```

## Comparing `bloxflipeasily-0.0.1.tar` & `bloxflipeasily-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 23:56:10.743217 bloxflipeasily-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2023-05-22 23:56:10.743217 bloxflipeasily-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 23:56:10.739217 bloxflipeasily-0.0.1/bloxflip_api/
--rw-r--r--   0 runner    (1000) runner    (1000)    21100 2023-05-22 06:18:18.000000 bloxflipeasily-0.0.1/bloxflip_api/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      655 2023-05-22 23:55:57.000000 bloxflipeasily-0.0.1/bloxflip_api/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 23:56:10.739217 bloxflipeasily-0.0.1/bloxflipeasily.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2023-05-22 23:56:10.000000 bloxflipeasily-0.0.1/bloxflipeasily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-05-22 23:56:10.000000 bloxflipeasily-0.0.1/bloxflipeasily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-22 23:56:10.000000 bloxflipeasily-0.0.1/bloxflipeasily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-05-22 23:56:10.000000 bloxflipeasily-0.0.1/bloxflipeasily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      422 2023-05-22 06:07:28.000000 bloxflipeasily-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-22 23:56:10.743217 bloxflipeasily-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-28 21:17:35.336612 bloxflipeasily-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2023-05-28 21:17:35.336612 bloxflipeasily-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-28 21:17:35.336612 bloxflipeasily-0.0.2/bloxflip_api/
+-rw-r--r--   0 runner    (1000) runner    (1000)    31053 2023-05-28 21:15:33.000000 bloxflipeasily-0.0.2/bloxflip_api/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      655 2023-05-28 21:15:33.000000 bloxflipeasily-0.0.2/bloxflip_api/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-28 21:17:35.336612 bloxflipeasily-0.0.2/bloxflipeasily.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2023-05-28 21:17:35.000000 bloxflipeasily-0.0.2/bloxflipeasily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-05-28 21:17:35.000000 bloxflipeasily-0.0.2/bloxflipeasily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-28 21:17:35.000000 bloxflipeasily-0.0.2/bloxflipeasily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-05-28 21:17:35.000000 bloxflipeasily-0.0.2/bloxflipeasily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      422 2023-05-22 06:07:28.000000 bloxflipeasily-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-28 21:17:35.336612 bloxflipeasily-0.0.2/setup.cfg
```

### Comparing `bloxflipeasily-0.0.1/bloxflip_api/setup.py` & `bloxflipeasily-0.0.2/bloxflip_api/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="bloxflipeasily", # Put your username here!
-    version="0.0.1", # The version of your package!
+    version="0.0.2", # The version of your package!
     author="Pytronomy", # Your name here!
     description="Made by Pytronomy on youtube", # A short description here!
     packages=setuptools.find_packages(), # A list of all packages for Python to distribute!
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

