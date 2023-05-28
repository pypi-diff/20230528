# Comparing `tmp/ak_pynn-0.1.4.tar.gz` & `tmp/ak_pynn-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_pynn-0.1.4.tar", last modified: Sun May 28 17:09:09 2023, max compression
+gzip compressed data, was "ak_pynn-0.1.5.tar", last modified: Sun May 28 17:11:43 2023, max compression
```

## Comparing `ak_pynn-0.1.4.tar` & `ak_pynn-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:09:09.571132 ak_pynn-0.1.4/
--rw-rw-rw-   0        0        0     1381 2023-05-28 17:09:09.569132 ak_pynn-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 17:09:09.503544 ak_pynn-0.1.4/ak_pynn/
--rw-rw-rw-   0        0        0      181 2023-05-28 17:08:56.000000 ak_pynn-0.1.4/ak_pynn/__init__.py
--rw-rw-rw-   0        0        0    36237 2023-05-28 16:58:18.000000 ak_pynn-0.1.4/ak_pynn/mlp.py
--rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.4/ak_pynn/nnv.py
--rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.4/ak_pynn/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:09:09.566875 ak_pynn-0.1.4/ak_pynn.egg-info/
--rw-rw-rw-   0        0        0     1381 2023-05-28 17:09:09.000000 ak_pynn-0.1.4/ak_pynn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-28 17:09:09.000000 ak_pynn-0.1.4/ak_pynn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:09:09.000000 ak_pynn-0.1.4/ak_pynn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-28 17:09:09.000000 ak_pynn-0.1.4/ak_pynn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 17:09:09.000000 ak_pynn-0.1.4/ak_pynn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 17:09:09.572133 ak_pynn-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2180 2023-05-28 17:08:50.000000 ak_pynn-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:11:43.239622 ak_pynn-0.1.5/
+-rw-rw-rw-   0        0        0     1381 2023-05-28 17:11:43.234274 ak_pynn-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 17:11:43.164215 ak_pynn-0.1.5/ak_pynn/
+-rw-rw-rw-   0        0        0      181 2023-05-28 17:11:27.000000 ak_pynn-0.1.5/ak_pynn/__init__.py
+-rw-rw-rw-   0        0        0    36237 2023-05-28 16:58:18.000000 ak_pynn-0.1.5/ak_pynn/mlp.py
+-rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.5/ak_pynn/nnv.py
+-rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.5/ak_pynn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:11:43.231980 ak_pynn-0.1.5/ak_pynn.egg-info/
+-rw-rw-rw-   0        0        0     1381 2023-05-28 17:11:42.000000 ak_pynn-0.1.5/ak_pynn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-28 17:11:43.000000 ak_pynn-0.1.5/ak_pynn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:11:42.000000 ak_pynn-0.1.5/ak_pynn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-28 17:11:42.000000 ak_pynn-0.1.5/ak_pynn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 17:11:42.000000 ak_pynn-0.1.5/ak_pynn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 17:11:43.239622 ak_pynn-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2149 2023-05-28 17:11:23.000000 ak_pynn-0.1.5/setup.py
```

### Comparing `ak_pynn-0.1.4/PKG-INFO` & `ak_pynn-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak_pynn
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simplistic and efficient pure-python neural network library
 Author: Ankit kohli
 Author-email: <contact.ankitkohli@gmail.com>
 License: MIT
 Keywords: neural network,pure python,ankit_nn,machine learning,ML,deep learning,deepL,MLP,perceptron,ankit kohli,ak_pynn
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `ak_pynn-0.1.4/ak_pynn/mlp.py` & `ak_pynn-0.1.5/ak_pynn/mlp.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.4/ak_pynn/nnv.py` & `ak_pynn-0.1.5/ak_pynn/nnv.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.4/ak_pynn/utils.py` & `ak_pynn-0.1.5/ak_pynn/utils.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.4/ak_pynn.egg-info/PKG-INFO` & `ak_pynn-0.1.5/ak_pynn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak-pynn
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simplistic and efficient pure-python neural network library
 Author: Ankit kohli
 Author-email: <contact.ankitkohli@gmail.com>
 License: MIT
 Keywords: neural network,pure python,ankit_nn,machine learning,ML,deep learning,deepL,MLP,perceptron,ankit kohli,ak_pynn
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `ak_pynn-0.1.4/setup.py` & `ak_pynn-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'A simplistic and efficient pure-python neural network library'
 LONG_DESCRIPTION = 'A package that allows to build multilayer neural network with ease.'
 
 setup(
     name = "ak_pynn",
     version=VERSION,
     author="Ankit kohli",
@@ -19,15 +19,14 @@
     install_requires=['numpy', 
                       'tqdm',
                       'opt_einsum',
                       'nnv',
                       'matplotlib',
                       'numexpr',
                       'seaborn',
-                      'math',
                       'random',
                       'time'                 
                       ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Intended Audience :: Science/Research",
```

