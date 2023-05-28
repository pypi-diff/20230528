# Comparing `tmp/docker-recipe-0.1.1.tar.gz` & `tmp/docker-recipe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-recipe-0.1.1.tar", last modified: Sat May 27 23:18:06 2023, max compression
+gzip compressed data, was "docker-recipe-0.1.2.tar", last modified: Sun May 28 14:13:23 2023, max compression
```

## Comparing `docker-recipe-0.1.1.tar` & `docker-recipe-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:18:06.953633 docker-recipe-0.1.1/
--rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.1/LICENSE.md
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:18:06.953506 docker-recipe-0.1.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.1/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:18:06.953325 docker-recipe-0.1.1/docker_recipe.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      253 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-27 23:18:06.953673 docker-recipe-0.1.1/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-27 23:17:27.000000 docker-recipe-0.1.1/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:13:23.270835 docker-recipe-0.1.2/
+-rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.2/LICENSE.md
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:13:23.270694 docker-recipe-0.1.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.2/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-28 14:13:23.270510 docker-recipe-0.1.2/docker_recipe.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      253 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-28 14:13:23.000000 docker-recipe-0.1.2/docker_recipe.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-28 14:13:23.270875 docker-recipe-0.1.2/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-28 14:12:36.000000 docker-recipe-0.1.2/setup.py
```

### Comparing `docker-recipe-0.1.1/LICENSE.md` & `docker-recipe-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docker-recipe-0.1.1/PKG-INFO` & `docker-recipe-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.1/docker_recipe.egg-info/PKG-INFO` & `docker-recipe-0.1.2/docker_recipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.1/setup.py` & `docker-recipe-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="docker-recipe",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         'pydantic~=1.10.8',
         'PyYaml~=6.0',
         'Jinja2~=3.1.2',
     ],
     author="Stephan Meijer",
```

