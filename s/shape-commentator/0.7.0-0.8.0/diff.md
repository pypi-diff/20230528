# Comparing `tmp/shape_commentator-0.7.0.tar.gz` & `tmp/shape_commentator-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shape_commentator-0.7.0.tar", last modified: Wed Dec 11 13:20:13 2019, max compression
+gzip compressed data, was "shape_commentator-0.8.0.tar", last modified: Sun May 28 12:47:43 2023, max compression
```

## Comparing `shape_commentator-0.7.0.tar` & `shape_commentator-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4061 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/shape_commentator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      337 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/print_clear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8359 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      962 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/ipython_ext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1472 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      481 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/print_comment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1242 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/shape_commentator/jupyter_ext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4061 2019-12-11 13:20:13.000000 shape_commentator-0.7.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      857 2019-12-11 13:20:07.000000 shape_commentator-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-28 12:47:43.519380 shape_commentator-0.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2023-05-28 12:47:43.519380 shape_commentator-0.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3304 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-28 12:47:43.519380 shape_commentator-0.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-28 12:47:43.519380 shape_commentator-0.8.0/shape_commentator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1083 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/ipython_ext.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/jupyter_ext.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8359 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/print_clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-05-28 12:47:38.000000 shape_commentator-0.8.0/shape_commentator/print_comment.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-28 12:47:43.519380 shape_commentator-0.8.0/shape_commentator.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2023-05-28 12:47:43.000000 shape_commentator-0.8.0/shape_commentator.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-05-28 12:47:43.000000 shape_commentator-0.8.0/shape_commentator.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-28 12:47:43.000000 shape_commentator-0.8.0/shape_commentator.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-05-28 12:47:43.000000 shape_commentator-0.8.0/shape_commentator.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `shape_commentator-0.7.0/README.md` & `shape_commentator-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # Shape Commentator
 [![CircleCI](https://circleci.com/gh/shiba6v/shape_commentator.svg?style=svg)](https://circleci.com/gh/shiba6v/shape_commentator)
 
 ## About  
-You can easily add numpy.ndarray.shape, torch.Size, other shape and type information at runtime to your script as comments.
+You can easily add numpy.ndarray.shape, torch.Size, other shape and type information at runtime to your script code as comments.  
+NumPyやPyTorchなどの配列のshape属性や，変数の型の実行時の情報を，スクリプトにコメントとして貼り付けるツールです．
 
-NumPyやPyTorchなどの配列のshape属性や，変数の型の実行時の情報を，ソースコードにコメントとして貼り付けるツールです．
+## Install
+```
+pip install -U shape_commentator
+```
+-U means upgrading.
 
-![Sample](https://user-images.githubusercontent.com/13820488/70534467-76321d80-1b9e-11ea-9ff1-e2d9c4140382.png)
+## Usage
+This tool has two types of usage.  
+このツールには2つの使い方があります．
 
-## Usage  
-### Execute as a Module
-#### Create Commented Script to File
-1. Run this script as a module with argument of script name.  Command line arguments to the target script are available.
+### Usage 1. Execute this as a Module
+![Sample_Module](https://user-images.githubusercontent.com/13820488/70629620-9f6daf00-1c6d-11ea-95d1-e4b8adc31a4d.png)
 
-Pythonのモジュールとしてshape_commentatorを実行してください．引数は，スクリプト名の後にスクリプトに渡したい引数を続けてください．
+#### Create Commented Script
+1. Run this script as a module with argument of script name.  Command line arguments to the target script are available.  
+Pythonのモジュールとしてshape_commentatorを実行してください．引数は，スクリプト名の後にスクリプトに渡したい引数を続けることもできます．
 
 ```bash
 python -m shape_commentator src.py
 ```
 
 ```bash
 python -m shape_commentator src.py arg1 arg2 arg3
 ```
 
 2. You get the commented script. For example, you execute shape_commentator to `src.py`, you get `src.py.commented.py`.  
-
 `src.py`というスクリプトに対して実行すると，`src.py.commented.py`が生成されます．
 
 `src.py`
 ```python
 import numpy as np
 a = np.array([1,2,3,4,5,6])
 b = np.array([0,1,2,3,4,5])
@@ -59,18 +65,19 @@
 c = 1 + 1j  #_ complex
 s = "string1"  #_ str
 class A():
     pass
 a = A()  #_ A
 ```
 
-### IPython / Jupyter Notebook (Magic Command)
-To use IPython magic command,
+### Usage 2. IPython / Jupyter Notebook (Magic Command)
+![Sample_IPython](https://user-images.githubusercontent.com/13820488/70638063-91268f80-1c7b-11ea-94c3-d00d32133636.png)
 
-IPythonでのマジックコマンドの使い方
+To use IPython / Jupyter Notebook magic command,  
+IPythonやJupyter Notebookでのマジックコマンドの使い方
 ```python
 import shape_commentator
 ```
 
 #### Create Commented Script
 コメントを付ける
 ```python
@@ -92,19 +99,21 @@
 
 output
 ```
 a = np.array([1,2,3,4,5,6])
 ```
 
 ## Tested Python Version  
-Test scripts are written in these version of Python.
+Test scripts are written in these version of Python.  
 以下のバージョンがテストされています．
-- 3.8.0
-- 3.7.5
-- 3.6.9
-- 3.5.9
-- 3.4.10
+- 3.11.3
+- 3.10.11
+- 3.9.16
+- 3.8.16
+- 3.7.16
+- 3.6.15
+- 3.5.10
 - 2.7.17
 
 ## Blog
-作った経緯などを書いた解説ブログはこちらにあります．
+作った経緯などを書いた解説ブログはこちらにあります．  
 [NumPyやPyTorchで使える超便利ツールを作った](http://shiba6v.hatenablog.com/entry/shape_commentator_release)
```

### Comparing `shape_commentator-0.7.0/shape_commentator/main.py` & `shape_commentator-0.8.0/shape_commentator/main.py`

 * *Files identical despite different names*

### Comparing `shape_commentator-0.7.0/shape_commentator/ipython_ext.py` & `shape_commentator-0.8.0/shape_commentator/ipython_ext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from IPython.core import page
 from IPython.core.magic import Magics, magics_class, cell_magic
 from .main import make_comment, clear_comment, SHAPE_COMMENTATOR_ENV
 import sys
 
+def find_frame():
+    for i in range(20):
+        f = sys._getframe(i)
+        if "In" in f.f_globals:
+            return f
+
 @magics_class
 class ShapeMagics(Magics):
     @cell_magic
     def shape(self, parameter_s='', cell=None):
         opts,argsl = self.parse_options(parameter_s,"d",mode="string")
         if "d" in opts:
             # erase
@@ -16,13 +22,13 @@
             output = "\n".join(output)
             page.page(output)
         else:
             # comment
             output = []
             output_func = lambda x: output.append(x)
             env = SHAPE_COMMENTATOR_ENV()
-            env.globals = sys._getframe(4).f_globals
+            env.globals = find_frame().f_globals
             try:
                 make_comment(cell, env, output_func)
             finally:
                 output = "\n".join(output)
                 page.page(output)
```

### Comparing `shape_commentator-0.7.0/shape_commentator/formatter.py` & `shape_commentator-0.8.0/shape_commentator/formatter.py`

 * *Files identical despite different names*

### Comparing `shape_commentator-0.7.0/shape_commentator/jupyter_ext.py` & `shape_commentator-0.8.0/shape_commentator/jupyter_ext.py`

 * *Files identical despite different names*

### Comparing `shape_commentator-0.7.0/LICENSE` & `shape_commentator-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shape_commentator-0.7.0/setup.py` & `shape_commentator-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import os
 import subprocess
 import io
 
-VERSION = "0.7.0"
+VERSION = "0.8.0"
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="shape_commentator",
```

