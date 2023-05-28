# Comparing `tmp/pyAGI-1.0.2.tar.gz` & `tmp/pyAGI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAGI-1.0.2.tar", last modified: Sun May 28 13:48:22 2023, max compression
+gzip compressed data, was "pyAGI-1.0.3.tar", last modified: Sun May 28 13:55:22 2023, max compression
```

## Comparing `pyAGI-1.0.2.tar` & `pyAGI-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.502799 pyAGI-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:48:13.000000 pyAGI-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:48:22.498799 pyAGI-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-28 13:48:13.000000 pyAGI-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.498799 pyAGI-1.0.2/pyAGI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/pyAGIChainGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/pyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-28 13:48:13.000000 pyAGI-1.0.2/pyAGI/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:48:22.498799 pyAGI-1.0.2/pyAGI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 13:48:22.000000 pyAGI-1.0.2/pyAGI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:48:22.502799 pyAGI-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-28 13:48:13.000000 pyAGI-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:22.223009 pyAGI-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:55:11.000000 pyAGI-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-28 13:55:22.223009 pyAGI-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-28 13:55:11.000000 pyAGI-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:22.223009 pyAGI-1.0.3/pyAGI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:11.000000 pyAGI-1.0.3/pyAGI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-28 13:55:11.000000 pyAGI-1.0.3/pyAGI/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 13:55:11.000000 pyAGI-1.0.3/pyAGI/pyAGIChainGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 13:55:11.000000 pyAGI-1.0.3/pyAGI/pyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-28 13:55:11.000000 pyAGI-1.0.3/pyAGI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:22.223009 pyAGI-1.0.3/pyAGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-28 13:55:22.000000 pyAGI-1.0.3/pyAGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 13:55:22.000000 pyAGI-1.0.3/pyAGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:55:22.000000 pyAGI-1.0.3/pyAGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 13:55:22.000000 pyAGI-1.0.3/pyAGI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 13:55:22.000000 pyAGI-1.0.3/pyAGI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:55:22.223009 pyAGI-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-28 13:55:11.000000 pyAGI-1.0.3/setup.py
```

### Comparing `pyAGI-1.0.2/LICENSE` & `pyAGI-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.2/README.md` & `pyAGI-1.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,21 +10,33 @@
 2. User experience flows
 3. Code flow descriptions
 4. Coding steps
 5. Application code
 
 ## Installation
 
-To install pyAGI, use pip:
+To install pyAGI (https://pypi.org/project/pyAGI/), use pip:
 
 `pip install pyAGI`
 
 ## Usage
 After installing, you can use pyAGI to generate content for your application as follows:
 
+```
+from pyAGI.pyagi import PyAGI
+
+Create a PyAGI instance with a selected OpenAI model
+py_agi = PyAGI.create_llm_chain(selected_model="text-davinci-003")
+
+# Run the PyAGI instance with the objective
+py_agi({"objective": "Your Objective", "selected_model": "text-davinci-003"})
+```
+
+# Usage without installing the pip package
+
 `python main.py "Objective of your app" "OpenAI Model"`
 
 For example:
 
 `python main.py "Build a weather app" "text-davinci-003"`
 
 ## Available Models
```

### Comparing `pyAGI-1.0.2/pyAGI/prompts.py` & `pyAGI-1.0.3/pyAGI/prompts.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.2/pyAGI/pyAGIChainGenerator.py` & `pyAGI-1.0.3/pyAGI/pyAGIChainGenerator.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.2/pyAGI/pyagi.py` & `pyAGI-1.0.3/pyAGI/pyagi.py`

 * *Files identical despite different names*

### Comparing `pyAGI-1.0.2/pyAGI/utils.py` & `pyAGI-1.0.3/pyAGI/utils.py`

 * *Files identical despite different names*

