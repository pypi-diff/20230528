# Comparing `tmp/NeuralNetworkData-0.0.1.tar.gz` & `tmp/NeuralNetworkData-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralNetworkData-0.0.1.tar", last modified: Sun May 28 17:47:43 2023, max compression
+gzip compressed data, was "NeuralNetworkData-0.0.2.tar", last modified: Sun May 28 18:04:01 2023, max compression
```

## Comparing `NeuralNetworkData-0.0.1.tar` & `NeuralNetworkData-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:47:43.556286 NeuralNetworkData-0.0.1/
--rw-rw-rw-   0        0        0       55 2023-05-28 17:36:41.000000 NeuralNetworkData-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-28 17:40:03.000000 NeuralNetworkData-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-28 17:38:57.000000 NeuralNetworkData-0.0.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-28 17:47:43.533045 NeuralNetworkData-0.0.1/NeuralNetworkData/
--rw-rw-rw-   0        0        0    31694 2023-05-28 17:34:53.000000 NeuralNetworkData-0.0.1/NeuralNetworkData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:47:43.554183 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/
--rw-rw-rw-   0        0        0      654 2023-05-28 17:47:43.000000 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-28 17:47:43.000000 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:47:43.000000 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-28 17:47:43.000000 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-28 17:47:43.000000 NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2023-05-28 17:47:43.555200 NeuralNetworkData-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-05-28 17:35:57.000000 NeuralNetworkData-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 17:47:43.556286 NeuralNetworkData-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-28 17:47:40.000000 NeuralNetworkData-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:04:01.274060 NeuralNetworkData-0.0.2/
+-rw-rw-rw-   0        0        0       55 2023-05-28 17:36:41.000000 NeuralNetworkData-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-28 17:40:03.000000 NeuralNetworkData-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 17:38:57.000000 NeuralNetworkData-0.0.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-28 18:04:01.262040 NeuralNetworkData-0.0.2/NeuralNetworkData/
+-rw-rw-rw-   0        0        0    14582 2023-05-28 18:03:16.000000 NeuralNetworkData-0.0.2/NeuralNetworkData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:04:01.272061 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/
+-rw-rw-rw-   0        0        0      654 2023-05-28 18:04:01.000000 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-28 18:04:01.000000 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 18:04:01.000000 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-28 18:04:01.000000 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-28 18:04:01.000000 NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2023-05-28 18:04:01.273059 NeuralNetworkData-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-05-28 17:35:57.000000 NeuralNetworkData-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 18:04:01.274060 NeuralNetworkData-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-05-28 18:03:25.000000 NeuralNetworkData-0.0.2/setup.py
```

### Comparing `NeuralNetworkData-0.0.1/LICENSE.txt` & `NeuralNetworkData-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralNetworkData-0.0.1/NeuralNetworkData.egg-info/PKG-INFO` & `NeuralNetworkData-0.0.2/NeuralNetworkData.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralNetworkData
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Network Data
 Home-page: UNKNOWN
 Author: PythonCoder2002
 Author-email: <adityabijapurkar@gmail.com>
 License: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
 Platform: UNKNOWN
```

### Comparing `NeuralNetworkData-0.0.1/PKG-INFO` & `NeuralNetworkData-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralNetworkData
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Network Data
 Home-page: UNKNOWN
 Author: PythonCoder2002
 Author-email: <adityabijapurkar@gmail.com>
 License: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
 Platform: UNKNOWN
```

### Comparing `NeuralNetworkData-0.0.1/setup.py` & `NeuralNetworkData-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="NeuralNetworkData",
-    version="0.0.1",
+    version="0.0.2",
     author="PythonCoder2002",
     author_email="<adityabijapurkar@gmail.com>",
     description="Neural Network Data",
     long_description=open('README.txt').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scikit-learn', 'tensorflow'],
```

