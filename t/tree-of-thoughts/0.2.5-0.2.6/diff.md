# Comparing `tmp/tree-of-thoughts-0.2.5.tar.gz` & `tmp/tree-of-thoughts-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.5.tar", last modified: Sun May 28 03:44:13 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.6.tar", last modified: Sun May 28 03:58:43 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.5.tar` & `tree-of-thoughts-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:44:13.059126 tree-of-thoughts-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:44:13.059126 tree-of-thoughts-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15193 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 03:44:13.059126 tree-of-thoughts-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:44:13.055126 tree-of-thoughts-0.2.5/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-28 03:43:59.000000 tree-of-thoughts-0.2.5/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:44:13.059126 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:44:13.000000 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-28 03:44:13.000000 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 03:44:13.000000 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 03:44:13.000000 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 03:44:13.000000 tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.994712 tree-of-thoughts-0.2.6/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.5/LICENSE` & `tree-of-thoughts-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.5/PKG-INFO` & `tree-of-thoughts-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.5/README.md` & `tree-of-thoughts-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,23 @@
 Navigate to the repository folder: ```cd tree-of-thoughts```
 
 ```pip install openai```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
-from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts, HuggingLanguageModel
+import os
+from tree_of_thoughts.openaiModels import OpenAILanguageModel
+from tree_of_thoughts.treeofthoughts import TreeofThoughts
+from tree_of_thoughts.huggingModel import HuggingLanguageModel
 
 use_v2 = False
 
 
-model = OptimizedOpenAILanguageModel(api_key=api_key) # api_model="gpt4" # for higher performance base model is not smart
+model = OptimizedOpenAILanguageModel(api_key='') # api_model="gpt4" # for higher performance base model is not smart
 
 
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
```

### Comparing `tree-of-thoughts-0.2.5/setup.py` & `tree-of-thoughts-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.5',
+  version = '0.2.6',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.2.5/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.2.6/tree_of_thoughts/guidanceModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.5/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.2.6/tree_of_thoughts/huggingModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.5/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.2.6/tree_of_thoughts/openaiModels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import openai
 import time
-from .abstractLanguageModel import AbstractLanguageModel
+from  tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
 import concurrent.futures
 
 class OpenAILanguageModel(AbstractLanguageModel):
     def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=True):
         if api_key == "" or api_key == None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
```

### Comparing `tree-of-thoughts-0.2.5/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.2.6/tree_of_thoughts/treeofthoughts.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.5/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

