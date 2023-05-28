# Comparing `tmp/ak_pynn-0.1.7.tar.gz` & `tmp/ak_pynn-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_pynn-0.1.7.tar", last modified: Sun May 28 17:18:55 2023, max compression
+gzip compressed data, was "ak_pynn-0.1.8.tar", last modified: Sun May 28 19:44:20 2023, max compression
```

## Comparing `ak_pynn-0.1.7.tar` & `ak_pynn-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:18:55.057622 ak_pynn-0.1.7/
--rw-rw-rw-   0        0        0     1381 2023-05-28 17:18:55.036135 ak_pynn-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 17:18:54.941298 ak_pynn-0.1.7/ak_pynn/
--rw-rw-rw-   0        0        0      181 2023-05-28 17:18:27.000000 ak_pynn-0.1.7/ak_pynn/__init__.py
--rw-rw-rw-   0        0        0    36237 2023-05-28 16:58:18.000000 ak_pynn-0.1.7/ak_pynn/mlp.py
--rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.7/ak_pynn/nnv.py
--rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.7/ak_pynn/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:18:55.026334 ak_pynn-0.1.7/ak_pynn.egg-info/
--rw-rw-rw-   0        0        0     1381 2023-05-28 17:18:54.000000 ak_pynn-0.1.7/ak_pynn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-28 17:18:54.000000 ak_pynn-0.1.7/ak_pynn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:18:54.000000 ak_pynn-0.1.7/ak_pynn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-28 17:18:54.000000 ak_pynn-0.1.7/ak_pynn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 17:18:54.000000 ak_pynn-0.1.7/ak_pynn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 17:18:55.073321 ak_pynn-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2039 2023-05-28 17:18:37.000000 ak_pynn-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:44:20.346219 ak_pynn-0.1.8/
+-rw-rw-rw-   0        0        0     1086 2023-05-28 18:15:32.000000 ak_pynn-0.1.8/LICENCE.md
+-rw-rw-rw-   0        0        0     6388 2023-05-28 19:44:20.341946 ak_pynn-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4828 2023-05-28 19:42:32.000000 ak_pynn-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 19:44:20.067249 ak_pynn-0.1.8/ak_pynn/
+-rw-rw-rw-   0        0        0      181 2023-05-28 19:42:54.000000 ak_pynn-0.1.8/ak_pynn/__init__.py
+-rw-rw-rw-   0        0        0    36237 2023-05-28 16:58:18.000000 ak_pynn-0.1.8/ak_pynn/mlp.py
+-rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.8/ak_pynn/nnv.py
+-rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.8/ak_pynn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:44:20.333946 ak_pynn-0.1.8/ak_pynn.egg-info/
+-rw-rw-rw-   0        0        0     6388 2023-05-28 19:44:19.000000 ak_pynn-0.1.8/ak_pynn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-28 19:44:19.000000 ak_pynn-0.1.8/ak_pynn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:44:19.000000 ak_pynn-0.1.8/ak_pynn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-28 19:44:19.000000 ak_pynn-0.1.8/ak_pynn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 19:44:19.000000 ak_pynn-0.1.8/ak_pynn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:44:20.346219 ak_pynn-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2100 2023-05-28 19:44:04.000000 ak_pynn-0.1.8/setup.py
```

### Comparing `ak_pynn-0.1.7/ak_pynn/mlp.py` & `ak_pynn-0.1.8/ak_pynn/mlp.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.7/ak_pynn/nnv.py` & `ak_pynn-0.1.8/ak_pynn/nnv.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.7/ak_pynn/utils.py` & `ak_pynn-0.1.8/ak_pynn/utils.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.7/setup.py` & `ak_pynn-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.1.7'
-DESCRIPTION = 'A simplistic and efficient pure-python neural network library'
-LONG_DESCRIPTION = 'A package that allows to build multilayer neural network with ease.'
+def read(fname):
+    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+
+VERSION = '0.1.8'
+DESCRIPTION = 'A simplistic and efficient pure-python neural network library that allows to build multilayer neural network with ease.'
 
 setup(
     name = "ak_pynn",
     version=VERSION,
     author="Ankit kohli",
     author_email="<contact.ankitkohli@gmail.com>",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
     license = "MIT",
     packages=find_packages(exclude=['datasets']),
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
     keywords = ["neural network", "pure python", "ankit_nn", "machine learning", "ML", "deep learning", "deepL", "MLP", "perceptron","ankit kohli","ak_pynn"],
     install_requires=['numpy', 
                       'tqdm',
                       'opt_einsum',
                       'matplotlib',
                       'numexpr',
                       'seaborn',
```

