# Comparing `tmp/berens-neat-0.1.0.tar.gz` & `tmp/berens-neat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berens-neat-0.1.0.tar", last modified: Sun May 28 11:12:42 2023, max compression
+gzip compressed data, was "berens-neat-0.1.1.tar", last modified: Sun May 28 11:38:29 2023, max compression
```

## Comparing `berens-neat-0.1.0.tar` & `berens-neat-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:12:42.161546 berens-neat-0.1.0/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1058 2023-05-28 09:09:34.000000 berens-neat-0.1.0/LICENSE
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:12:42.161546 berens-neat-0.1.0/PKG-INFO
--rw-r--r--   0 charlie   (1000) charlie   (1000)      772 2023-05-27 21:27:50.000000 berens-neat-0.1.0/README.md
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:12:42.151546 berens-neat-0.1.0/berens_neat.egg-info/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:12:42.000000 berens-neat-0.1.0/berens_neat.egg-info/PKG-INFO
--rw-r--r--   0 charlie   (1000) charlie   (1000)      337 2023-05-28 11:12:42.000000 berens-neat-0.1.0/berens_neat.egg-info/SOURCES.txt
--rw-r--r--   0 charlie   (1000) charlie   (1000)        1 2023-05-28 11:12:42.000000 berens-neat-0.1.0/berens_neat.egg-info/dependency_links.txt
--rw-r--r--   0 charlie   (1000) charlie   (1000)       10 2023-05-28 11:12:42.000000 berens-neat-0.1.0/berens_neat.egg-info/top_level.txt
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:12:42.161546 berens-neat-0.1.0/neat/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     5184 2023-05-28 08:59:46.000000 berens-neat-0.1.0/neat/__init__.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      131 2023-05-28 10:50:26.000000 berens-neat-0.1.0/neat/activations.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2910 2023-05-28 09:01:35.000000 berens-neat-0.1.0/neat/config.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)    17561 2023-05-28 08:57:11.000000 berens-neat-0.1.0/neat/organism.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2458 2023-05-28 08:57:20.000000 berens-neat-0.1.0/neat/population.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     4526 2023-05-28 11:07:11.000000 berens-neat-0.1.0/neat/reporter.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     7986 2023-05-28 08:57:46.000000 berens-neat-0.1.0/neat/reproduction.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2156 2023-05-28 08:57:51.000000 berens-neat-0.1.0/neat/species.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      123 2023-05-23 05:56:11.000000 berens-neat-0.1.0/neat/utils.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      669 2023-05-28 11:11:47.000000 berens-neat-0.1.0/pyproject.toml
--rw-r--r--   0 charlie   (1000) charlie   (1000)       38 2023-05-28 11:12:42.161546 berens-neat-0.1.0/setup.cfg
--rw-r--r--   0 charlie   (1000) charlie   (1000)      136 2023-05-28 10:40:58.000000 berens-neat-0.1.0/setup.py
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1058 2023-05-28 11:15:24.000000 berens-neat-0.1.1/LICENSE
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:38:29.221498 berens-neat-0.1.1/PKG-INFO
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      772 2023-05-27 21:27:50.000000 berens-neat-0.1.1/README.md
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/berens_neat.egg-info/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/PKG-INFO
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      337 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie   (1000) charlie   (1000)        1 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie   (1000) charlie   (1000)       10 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/top_level.txt
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/neat/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     5184 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/__init__.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      131 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/activations.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2915 2023-05-28 11:37:51.000000 berens-neat-0.1.1/neat/config.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)    17561 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/organism.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2458 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/population.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     4526 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/reporter.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     7986 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/reproduction.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2156 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/species.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      123 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/utils.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      669 2023-05-28 11:38:11.000000 berens-neat-0.1.1/pyproject.toml
+-rw-r--r--   0 charlie   (1000) charlie   (1000)       38 2023-05-28 11:38:29.221498 berens-neat-0.1.1/setup.cfg
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      136 2023-05-28 11:15:24.000000 berens-neat-0.1.1/setup.py
```

### Comparing `berens-neat-0.1.0/LICENSE` & `berens-neat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/PKG-INFO` & `berens-neat-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berens-neat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple implementation of NEAT in Python
 Author-email: Charlie Berens <charliejb3@gmail.com>
 Project-URL: Homepage, https://github.com/charlieberens/neat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `berens-neat-0.1.0/README.md` & `berens-neat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/berens_neat.egg-info/PKG-INFO` & `berens-neat-0.1.1/berens_neat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berens-neat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple implementation of NEAT in Python
 Author-email: Charlie Berens <charliejb3@gmail.com>
 Project-URL: Homepage, https://github.com/charlieberens/neat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `berens-neat-0.1.0/neat/__init__.py` & `berens-neat-0.1.1/neat/__init__.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/neat/config.py` & `berens-neat-0.1.1/neat/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     "progress_directory": "progress",
     "organism_directory": "organisms",
 }
 
 config = defaults.copy()
 
 
-def get_config(file):
+def get_config(file=None):
     """
     Load a config from a file
     """
     file_config = {}
     if file:
         with open(file, "r") as f:
             file_config = json.load(f)
```

### Comparing `berens-neat-0.1.0/neat/organism.py` & `berens-neat-0.1.1/neat/organism.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/neat/population.py` & `berens-neat-0.1.1/neat/population.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/neat/reporter.py` & `berens-neat-0.1.1/neat/reporter.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/neat/reproduction.py` & `berens-neat-0.1.1/neat/reproduction.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/neat/species.py` & `berens-neat-0.1.1/neat/species.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.0/pyproject.toml` & `berens-neat-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "berens-neat"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Charlie Berens", email="charliejb3@gmail.com" },
 ]
 description = "A simple implementation of NEAT in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

