# Comparing `tmp/docker-recipe-0.1.3.tar.gz` & `tmp/docker-recipe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-recipe-0.1.3.tar", last modified: Sun May 28 14:18:41 2023, max compression
+gzip compressed data, was "docker-recipe-0.1.4.tar", last modified: Sun May 28 14:22:34 2023, max compression
```

## Comparing `docker-recipe-0.1.3.tar` & `docker-recipe-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:18:41.497732 docker-recipe-0.1.3/
--rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.3/LICENSE.md
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:18:41.497559 docker-recipe-0.1.3/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.3/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:18:41.497348 docker-recipe-0.1.3/docker_recipe.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      253 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-28 14:18:41.000000 docker-recipe-0.1.3/docker_recipe.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-28 14:18:41.497769 docker-recipe-0.1.3/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-28 14:18:06.000000 docker-recipe-0.1.3/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:22:34.461649 docker-recipe-0.1.4/
+-rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.4/LICENSE.md
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:22:34.461513 docker-recipe-0.1.4/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.4/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:22:34.460252 docker-recipe-0.1.4/docker_recipe/
+-rw-r--r--   0 steve      (501) staff       (20)       23 2023-05-28 14:22:01.000000 docker-recipe-0.1.4/docker_recipe/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1014 2023-05-28 14:21:47.000000 docker-recipe-0.1.4/docker_recipe/main.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:22:34.461336 docker-recipe-0.1.4/docker_recipe.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      301 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-05-28 14:22:34.000000 docker-recipe-0.1.4/docker_recipe.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-28 14:22:34.461690 docker-recipe-0.1.4/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-28 14:21:47.000000 docker-recipe-0.1.4/setup.py
```

### Comparing `docker-recipe-0.1.3/LICENSE.md` & `docker-recipe-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docker-recipe-0.1.3/PKG-INFO` & `docker-recipe-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.3
+Version: 0.1.4
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.3/docker_recipe.egg-info/PKG-INFO` & `docker-recipe-0.1.4/docker_recipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.3
+Version: 0.1.4
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.3/setup.py` & `docker-recipe-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="docker-recipe",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         'pydantic~=1.10.8',
         'PyYaml~=6.0',
         'Jinja2~=3.1.2',
     ],
     author="Stephan Meijer",
```

