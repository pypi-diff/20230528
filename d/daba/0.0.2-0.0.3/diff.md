# Comparing `tmp/daba-0.0.2.tar.gz` & `tmp/daba-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daba-0.0.2.tar", last modified: Sun May 28 15:25:49 2023, max compression
+gzip compressed data, was "daba-0.0.3.tar", last modified: Sun May 28 15:56:16 2023, max compression
```

## Comparing `daba-0.0.2.tar` & `daba-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834774 daba-0.0.2/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.2/LICENSE
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:25:49.834644 daba-0.0.2/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     2821 2023-05-28 15:17:32.000000 daba-0.0.2/README.md
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.833570 daba-0.0.2/daba/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3257 2023-05-28 07:33:46.000000 daba-0.0.2/daba/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.2/daba/__init__.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834007 daba-0.0.2/daba.egg-info/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      238 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/SOURCES.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/dependency_links.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 15:25:49.000000 daba-0.0.2/daba.egg-info/top_level.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 15:25:49.834824 daba-0.0.2/setup.cfg
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      735 2023-05-28 15:22:05.000000 daba-0.0.2/setup.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834120 daba-0.0.2/tests/
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:25:49.834471 daba-0.0.2/tests/Database/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.2/tests/Database/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.2/tests/Database/__init__.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.2/tests/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:56:16.605763 daba-0.0.3/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.3/LICENSE
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:56:16.605657 daba-0.0.3/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     2821 2023-05-28 15:17:32.000000 daba-0.0.3/README.md
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:56:16.604602 daba-0.0.3/daba/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3611 2023-05-28 15:54:28.000000 daba-0.0.3/daba/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.3/daba/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:56:16.605033 daba-0.0.3/daba.egg-info/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 15:56:16.000000 daba-0.0.3/daba.egg-info/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      238 2023-05-28 15:56:16.000000 daba-0.0.3/daba.egg-info/SOURCES.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 15:56:16.000000 daba-0.0.3/daba.egg-info/dependency_links.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 15:56:16.000000 daba-0.0.3/daba.egg-info/top_level.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 15:56:16.605799 daba-0.0.3/setup.cfg
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      735 2023-05-28 15:55:02.000000 daba-0.0.3/setup.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:56:16.605147 daba-0.0.3/tests/
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 15:56:16.605504 daba-0.0.3/tests/Database/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.3/tests/Database/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.3/tests/Database/__init__.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.3/tests/__init__.py
```

### Comparing `daba-0.0.2/LICENSE` & `daba-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daba-0.0.2/PKG-INFO` & `daba-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daba
-Version: 0.0.2
+Version: 0.0.3
 Summary: daba by Klivolks.
 Home-page: https://github.com/klivolks/Database
 Author: Vishnu Prakash
 Author-email: vishnu@klivolks.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `daba-0.0.2/README.md` & `daba-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `daba-0.0.2/daba/Mongo.py` & `daba-0.0.3/daba/Mongo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 Mongo database is handled here
 Improved db class.
 """
 
 import pymongo
 import os
 from dotenv import load_dotenv
+import logging
 
 
 class collection:
     # Setting database
     def __init__(self, collection):
         self.collection = self.init_db(collection)
+        self.logger = logging.getLogger(__name__)
+        handler = logging.FileHandler('daba-error.log')
+        handler.setLevel(logging.ERROR)
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        handler.setFormatter(formatter)
+        self.logger.addHandler(handler)
 
     def init_db(self, collection):
         load_dotenv()
         mongo_url = os.environ.get('MONGO_URL')
         mongo_db = os.environ.get('MONGO_DB')
         client = pymongo.MongoClient(mongo_url)
         database = client[mongo_db]
@@ -82,12 +89,13 @@
         if condition is None:
             condition = {}
         return self.exec_operation(self.collection.count_documents, condition)
 
     def exec_operation(self, operation, *args):
         try:
             response = operation(*args)
-            self.close_db()
             return response
         except Exception as e:
-            print(f"An error occurred: {e}")
+            self.logger.error(f"An error occurred: {e}")
+            raise
+        finally:
             self.close_db()
```

### Comparing `daba-0.0.2/daba.egg-info/PKG-INFO` & `daba-0.0.3/daba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daba
-Version: 0.0.2
+Version: 0.0.3
 Summary: daba by Klivolks.
 Home-page: https://github.com/klivolks/Database
 Author: Vishnu Prakash
 Author-email: vishnu@klivolks.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `daba-0.0.2/setup.py` & `daba-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='daba',
-    version='0.0.2',
+    version='0.0.3',
     description='daba by Klivolks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Vishnu Prakash',
     author_email='vishnu@klivolks.com',
     url='https://github.com/klivolks/Database',
     packages=find_packages(),
```

### Comparing `daba-0.0.2/tests/Database/Mongo.py` & `daba-0.0.3/tests/Database/Mongo.py`

 * *Files identical despite different names*

