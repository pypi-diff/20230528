# Comparing `tmp/ak_pynn-0.1.2.tar.gz` & `tmp/ak_pynn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_pynn-0.1.2.tar", last modified: Sun May 28 16:24:07 2023, max compression
+gzip compressed data, was "ak_pynn-0.1.3.tar", last modified: Sun May 28 17:00:00 2023, max compression
```

## Comparing `ak_pynn-0.1.2.tar` & `ak_pynn-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 16:24:07.110749 ak_pynn-0.1.2/
--rw-rw-rw-   0        0        0     1381 2023-05-28 16:24:07.110749 ak_pynn-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 16:24:07.057846 ak_pynn-0.1.2/ak_pynn/
--rw-rw-rw-   0        0        0      181 2023-05-28 16:23:18.000000 ak_pynn-0.1.2/ak_pynn/__init__.py
--rw-rw-rw-   0        0        0    36258 2023-05-28 15:56:47.000000 ak_pynn-0.1.2/ak_pynn/mlp.py
--rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.2/ak_pynn/nnv.py
--rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.2/ak_pynn/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 16:24:07.107554 ak_pynn-0.1.2/ak_pynn.egg-info/
--rw-rw-rw-   0        0        0     1381 2023-05-28 16:24:06.000000 ak_pynn-0.1.2/ak_pynn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-28 16:24:06.000000 ak_pynn-0.1.2/ak_pynn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 16:24:06.000000 ak_pynn-0.1.2/ak_pynn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-28 16:24:06.000000 ak_pynn-0.1.2/ak_pynn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 16:24:06.000000 ak_pynn-0.1.2/ak_pynn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 16:24:07.115763 ak_pynn-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2211 2023-05-28 16:23:09.000000 ak_pynn-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:00:00.331305 ak_pynn-0.1.3/
+-rw-rw-rw-   0        0        0     1381 2023-05-28 17:00:00.329125 ak_pynn-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 17:00:00.266349 ak_pynn-0.1.3/ak_pynn/
+-rw-rw-rw-   0        0        0      181 2023-05-28 16:57:36.000000 ak_pynn-0.1.3/ak_pynn/__init__.py
+-rw-rw-rw-   0        0        0    36237 2023-05-28 16:58:18.000000 ak_pynn-0.1.3/ak_pynn/mlp.py
+-rw-rw-rw-   0        0        0     7040 2023-05-28 14:22:38.000000 ak_pynn-0.1.3/ak_pynn/nnv.py
+-rw-rw-rw-   0        0        0     8780 2023-05-28 08:27:19.000000 ak_pynn-0.1.3/ak_pynn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:00:00.322899 ak_pynn-0.1.3/ak_pynn.egg-info/
+-rw-rw-rw-   0        0        0     1381 2023-05-28 16:59:59.000000 ak_pynn-0.1.3/ak_pynn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-28 17:00:00.000000 ak_pynn-0.1.3/ak_pynn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 16:59:59.000000 ak_pynn-0.1.3/ak_pynn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-28 16:59:59.000000 ak_pynn-0.1.3/ak_pynn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 16:59:59.000000 ak_pynn-0.1.3/ak_pynn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 17:00:00.332308 ak_pynn-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2180 2023-05-28 16:59:15.000000 ak_pynn-0.1.3/setup.py
```

### Comparing `ak_pynn-0.1.2/PKG-INFO` & `ak_pynn-0.1.3/ak_pynn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ak_pynn
-Version: 0.1.2
+Name: ak-pynn
+Version: 0.1.3
 Summary: A simplistic and efficient pure-python neural network library
 Author: Ankit kohli
 Author-email: <contact.ankitkohli@gmail.com>
 License: MIT
 Keywords: neural network,pure python,ankit_nn,machine learning,ML,deep learning,deepL,MLP,perceptron,ankit kohli,ak_pynn
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `ak_pynn-0.1.2/ak_pynn/mlp.py` & `ak_pynn-0.1.3/ak_pynn/mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     - Ankit Kohli (Student at Delhi University)
     - ankitkohli181@gmail.com (mail)
 
 Have fun!
 
 '''
 import numpy as np
-import pandas as pd
 import random
 import time
 import math
 from ak_pynn.utils import *
 from tqdm import tqdm
 from ak_pynn.nnv import NNV
 import matplotlib.pyplot as plt
```

### Comparing `ak_pynn-0.1.2/ak_pynn/nnv.py` & `ak_pynn-0.1.3/ak_pynn/nnv.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.2/ak_pynn/utils.py` & `ak_pynn-0.1.3/ak_pynn/utils.py`

 * *Files identical despite different names*

### Comparing `ak_pynn-0.1.2/ak_pynn.egg-info/PKG-INFO` & `ak_pynn-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ak-pynn
-Version: 0.1.2
+Name: ak_pynn
+Version: 0.1.3
 Summary: A simplistic and efficient pure-python neural network library
 Author: Ankit kohli
 Author-email: <contact.ankitkohli@gmail.com>
 License: MIT
 Keywords: neural network,pure python,ankit_nn,machine learning,ML,deep learning,deepL,MLP,perceptron,ankit kohli,ak_pynn
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `ak_pynn-0.1.2/setup.py` & `ak_pynn-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'A simplistic and efficient pure-python neural network library'
 LONG_DESCRIPTION = 'A package that allows to build multilayer neural network with ease.'
 
 setup(
     name = "ak_pynn",
     version=VERSION,
     author="Ankit kohli",
     author_email="<contact.ankitkohli@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     license = "MIT",
     packages=find_packages(exclude=['datasets']),
     keywords = ["neural network", "pure python", "ankit_nn", "machine learning", "ML", "deep learning", "deepL", "MLP", "perceptron","ankit kohli","ak_pynn"],
-    install_requires=['numba>=0.54.1',
-                      'numpy==1.19.2', 
-                      'autograd',
+    install_requires=['numpy', 
                       'tqdm',
                       'opt_einsum',
                       'nnv',
                       'matplotlib',
                       'numexpr',
-                      'opencv-python' ,
-                      'seaborn'                   
+                      'seaborn',
+                      'math',
+                      'random',
+                      'time'                 
                       ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
```

