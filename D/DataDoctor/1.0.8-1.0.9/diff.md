# Comparing `tmp/DataDoctor-1.0.8.tar.gz` & `tmp/DataDoctor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataDoctor-1.0.8.tar", last modified: Thu May 25 22:53:04 2023, max compression
+gzip compressed data, was "DataDoctor-1.0.9.tar", last modified: Thu May 25 22:56:21 2023, max compression
```

## Comparing `DataDoctor-1.0.8.tar` & `DataDoctor-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:53:04.434785 DataDoctor-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-25 22:53:04.434785 DataDoctor-1.0.8/DataDoctor.egg-info/
--rw-rw-rw-   0        0        0     4869 2023-05-25 22:53:04.000000 DataDoctor-1.0.8/DataDoctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-25 22:53:04.000000 DataDoctor-1.0.8/DataDoctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:53:04.000000 DataDoctor-1.0.8/DataDoctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-25 22:53:04.000000 DataDoctor-1.0.8/DataDoctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 22:53:04.000000 DataDoctor-1.0.8/DataDoctor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0     4869 2023-05-25 22:53:04.434785 DataDoctor-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3989 2023-05-25 22:51:40.000000 DataDoctor-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 22:53:04.434785 DataDoctor-1.0.8/data_doctor/
--rw-rw-rw-   0        0        0       34 2023-05-25 15:39:28.000000 DataDoctor-1.0.8/data_doctor/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.8/data_doctor/cleaner.py
--rw-rw-rw-   0        0        0     7326 2023-05-25 22:09:02.000000 DataDoctor-1.0.8/data_doctor/normalizer.py
--rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.8/data_doctor/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-25 22:53:04.434785 DataDoctor-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-05-25 22:46:56.000000 DataDoctor-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:56:21.632465 DataDoctor-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-25 22:56:21.624455 DataDoctor-1.0.9/DataDoctor.egg-info/
+-rw-rw-rw-   0        0        0     4830 2023-05-25 22:56:21.000000 DataDoctor-1.0.9/DataDoctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-25 22:56:21.000000 DataDoctor-1.0.9/DataDoctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:56:21.000000 DataDoctor-1.0.9/DataDoctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 22:56:21.000000 DataDoctor-1.0.9/DataDoctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 22:56:21.000000 DataDoctor-1.0.9/DataDoctor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0     4830 2023-05-25 22:56:21.632465 DataDoctor-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3950 2023-05-25 22:54:45.000000 DataDoctor-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 22:56:21.632465 DataDoctor-1.0.9/data_doctor/
+-rw-rw-rw-   0        0        0       34 2023-05-25 15:39:28.000000 DataDoctor-1.0.9/data_doctor/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.9/data_doctor/cleaner.py
+-rw-rw-rw-   0        0        0     7326 2023-05-25 22:09:02.000000 DataDoctor-1.0.9/data_doctor/normalizer.py
+-rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.9/data_doctor/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 22:56:21.632465 DataDoctor-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-05-25 22:54:54.000000 DataDoctor-1.0.9/setup.py
```

### Comparing `DataDoctor-1.0.8/DataDoctor.egg-info/PKG-INFO` & `DataDoctor-1.0.9/DataDoctor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -101,15 +101,14 @@
 - Invalid values treatment
 - Inconsistent or conflicting values treatment
 - Encoding errors treatment
 - Inconsistent date and time formats treatment
 - Inconsistent variable names treatment
 - Inconsistent capitalization or punctuation treatment
 - Spelling or typographical errors treatment
-- Data normalization issues treatment
 
 ## Algorithm
 
 The DataDoctor package uses a combination of techniques to clean and preprocess data. These techniques include iterative imputation, simple imputation, isolation forest, fuzzy matching, and others. Each technique serves a specific purpose in the data cleaning and preprocessing process.
 
 Iterative imputation is a method for handling missing data by modeling each missing value as a function of other variables in the data. Simple imputation is another method for handling missing data by replacing missing values with a single estimated value.
```

### Comparing `DataDoctor-1.0.8/LICENSE.md` & `DataDoctor-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.8/PKG-INFO` & `DataDoctor-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -101,15 +101,14 @@
 - Invalid values treatment
 - Inconsistent or conflicting values treatment
 - Encoding errors treatment
 - Inconsistent date and time formats treatment
 - Inconsistent variable names treatment
 - Inconsistent capitalization or punctuation treatment
 - Spelling or typographical errors treatment
-- Data normalization issues treatment
 
 ## Algorithm
 
 The DataDoctor package uses a combination of techniques to clean and preprocess data. These techniques include iterative imputation, simple imputation, isolation forest, fuzzy matching, and others. Each technique serves a specific purpose in the data cleaning and preprocessing process.
 
 Iterative imputation is a method for handling missing data by modeling each missing value as a function of other variables in the data. Simple imputation is another method for handling missing data by replacing missing values with a single estimated value.
```

### Comparing `DataDoctor-1.0.8/README.md` & `DataDoctor-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 - Invalid values treatment
 - Inconsistent or conflicting values treatment
 - Encoding errors treatment
 - Inconsistent date and time formats treatment
 - Inconsistent variable names treatment
 - Inconsistent capitalization or punctuation treatment
 - Spelling or typographical errors treatment
-- Data normalization issues treatment
 
 ## Algorithm
 
 The DataDoctor package uses a combination of techniques to clean and preprocess data. These techniques include iterative imputation, simple imputation, isolation forest, fuzzy matching, and others. Each technique serves a specific purpose in the data cleaning and preprocessing process.
 
 Iterative imputation is a method for handling missing data by modeling each missing value as a function of other variables in the data. Simple imputation is another method for handling missing data by replacing missing values with a single estimated value.
```

### Comparing `DataDoctor-1.0.8/data_doctor/cleaner.py` & `DataDoctor-1.0.9/data_doctor/cleaner.py`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.8/data_doctor/normalizer.py` & `DataDoctor-1.0.9/data_doctor/normalizer.py`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.8/setup.py` & `DataDoctor-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='DataDoctor',
-    version='1.0.8',
+    version='1.0.9',
     author='Aryan Bajaj',
     author_email='aryanbajaj104@email.com',
     description="A Python package for data cleaning and preprocessing.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

