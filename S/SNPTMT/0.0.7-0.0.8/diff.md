# Comparing `tmp/SNPTMT-0.0.7.tar.gz` & `tmp/SNPTMT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.7.tar", last modified: Sat May 27 21:30:35 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.8.tar", last modified: Sun May 28 16:07:25 2023, max compression
```

## Comparing `SNPTMT-0.0.7.tar` & `SNPTMT-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.475846 SNPTMT-0.0.7/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.7/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 21:30:35.475955 SNPTMT-0.0.7/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.7/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.474664 SNPTMT-0.0.7/SNPTMT/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.7/SNPTMT/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8733 2023-05-27 21:29:46.000000 SNPTMT-0.0.7/SNPTMT/snptmt.py
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.475415 SNPTMT-0.0.7/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/top_level.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 21:30:35.476260 SNPTMT-0.0.7/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 21:29:56.000000 SNPTMT-0.0.7/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.103114 SNPTMT-0.0.8/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.8/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:07:25.103188 SNPTMT-0.0.8/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.8/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.102083 SNPTMT-0.0.8/SNPTMT/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.8/SNPTMT/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8728 2023-05-28 16:06:27.000000 SNPTMT-0.0.8/SNPTMT/snptmt.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-28 16:07:25.102740 SNPTMT-0.0.8/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-28 16:07:25.000000 SNPTMT-0.0.8/SNPTMT.egg-info/top_level.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-28 16:07:25.103464 SNPTMT-0.0.8/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-28 16:06:44.000000 SNPTMT-0.0.8/setup.py
```

### Comparing `SNPTMT-0.0.7/LICENSE` & `SNPTMT-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.7/PKG-INFO` & `SNPTMT-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.7/SNPTMT/snptmt.py` & `SNPTMT-0.0.8/SNPTMT/snptmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     n_clusters = len(cluster_dict)
     for i in range(1, n_clusters + 1):
         cluster_messages = [df.iloc[j + start_message]['message'] for j in cluster_dict[i]]
         #print(f"Cluster {i}: {cluster_messages}")
     return cluster_dict
 
 
-def add_points(df, start_message, end_message, cluster_dict, nlp):
+def add_points(df, start_message, end_message, cluster_dict):
     nlp = spacy.load("ru_core_news_sm")
     #take part of prev clusters
     half_cluster_dict = {}
     for key, value in cluster_dict.items():
         half_len = math.ceil(len(value)/2)
         half_cluster_dict[key] = random.sample(value, half_len)
     #this if we want to compare half_clusters
```

### Comparing `SNPTMT-0.0.7/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.8/SNPTMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.7/setup.py` & `SNPTMT-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.7'
+version = '0.0.8'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

