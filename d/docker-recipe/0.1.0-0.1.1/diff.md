# Comparing `tmp/docker-recipe-0.1.0.tar.gz` & `tmp/docker-recipe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-recipe-0.1.0.tar", last modified: Sat May 27 23:08:09 2023, max compression
+gzip compressed data, was "docker-recipe-0.1.1.tar", last modified: Sat May 27 23:18:06 2023, max compression
```

## Comparing `docker-recipe-0.1.0.tar` & `docker-recipe-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:08:09.304617 docker-recipe-0.1.0/
--rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.0/LICENSE.md
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:08:09.304448 docker-recipe-0.1.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.0/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:08:09.304060 docker-recipe-0.1.0/docker_recipe.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:08:09.000000 docker-recipe-0.1.0/docker_recipe.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      213 2023-05-27 23:08:09.000000 docker-recipe-0.1.0/docker_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:08:09.000000 docker-recipe-0.1.0/docker_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-27 23:08:09.000000 docker-recipe-0.1.0/docker_recipe.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:08:09.000000 docker-recipe-0.1.0/docker_recipe.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-27 23:08:09.304740 docker-recipe-0.1.0/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      714 2023-05-27 23:05:54.000000 docker-recipe-0.1.0/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:18:06.953633 docker-recipe-0.1.1/
+-rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-0.1.1/LICENSE.md
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:18:06.953506 docker-recipe-0.1.1/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-0.1.1/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-27 23:18:06.953325 docker-recipe-0.1.1/docker_recipe.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      253 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-27 23:18:06.000000 docker-recipe-0.1.1/docker_recipe.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-27 23:18:06.953673 docker-recipe-0.1.1/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-27 23:17:27.000000 docker-recipe-0.1.1/setup.py
```

### Comparing `docker-recipe-0.1.0/LICENSE.md` & `docker-recipe-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docker-recipe-0.1.0/PKG-INFO` & `docker-recipe-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.0/docker_recipe.egg-info/PKG-INFO` & `docker-recipe-0.1.1/docker_recipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-0.1.0/setup.py` & `docker-recipe-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="docker-recipe",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         'pydantic~=1.10.8',
         'PyYaml~=6.0',
         'Jinja2~=3.1.2',
     ],
     author="Stephan Meijer",
@@ -16,8 +16,13 @@
     long_description_content_type='text/markdown',
     url="https://github.com/stephanmeijer/docker-recipe",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
     ],
+    entry_points={
+        'console_scripts': [
+            'docker-recipe=docker_recipe:main',  # map the docker-recipe command to a function
+        ],
+    },
 )
```

