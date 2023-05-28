# Comparing `tmp/multi_stock_api-0.1.1.tar.gz` & `tmp/multi_stock_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_stock_api-0.1.1.tar", last modified: Sun May 28 13:08:18 2023, max compression
+gzip compressed data, was "multi_stock_api-0.1.2.tar", last modified: Sun May 28 13:14:09 2023, max compression
```

## Comparing `multi_stock_api-0.1.1.tar` & `multi_stock_api-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:08:18.948049 multi_stock_api-0.1.1/
--rw-rw-r--   0 emir      (1001) emir      (1001)     1064 2023-05-28 08:50:15.000000 multi_stock_api-0.1.1/LICENSE
--rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:08:18.948049 multi_stock_api-0.1.1/PKG-INFO
--rw-rw-r--   0 emir      (1001) emir      (1001)       96 2023-05-28 12:28:24.000000 multi_stock_api-0.1.1/README.md
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:08:18.944049 multi_stock_api-0.1.1/multi_stock_api/
--rw-rw-r--   0 emir      (1001) emir      (1001)       26 2023-05-28 12:17:47.000000 multi_stock_api-0.1.1/multi_stock_api/__init__.py
--rw-rw-r--   0 emir      (1001) emir      (1001)     1322 2023-05-28 12:18:46.000000 multi_stock_api-0.1.1/multi_stock_api/app.py
--rw-rw-r--   0 emir      (1001) emir      (1001)     1534 2023-05-28 12:18:38.000000 multi_stock_api-0.1.1/multi_stock_api/configurations.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      915 2023-05-28 12:18:32.000000 multi_stock_api-0.1.1/multi_stock_api/external_api_access.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      326 2023-05-28 12:01:51.000000 multi_stock_api-0.1.1/multi_stock_api/helpers.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      831 2023-05-28 12:18:52.000000 multi_stock_api-0.1.1/multi_stock_api/mappers.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      654 2023-05-28 12:03:50.000000 multi_stock_api-0.1.1/multi_stock_api/models.py
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:08:18.948049 multi_stock_api-0.1.1/multi_stock_api.egg-info/
--rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:08:18.000000 multi_stock_api-0.1.1/multi_stock_api.egg-info/PKG-INFO
--rw-rw-r--   0 emir      (1001) emir      (1001)      424 2023-05-28 13:08:18.000000 multi_stock_api-0.1.1/multi_stock_api.egg-info/SOURCES.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)        1 2023-05-28 13:08:18.000000 multi_stock_api-0.1.1/multi_stock_api.egg-info/dependency_links.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)      490 2023-05-28 13:08:18.000000 multi_stock_api-0.1.1/multi_stock_api.egg-info/requires.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)       16 2023-05-28 13:08:18.000000 multi_stock_api-0.1.1/multi_stock_api.egg-info/top_level.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)       38 2023-05-28 13:08:18.948049 multi_stock_api-0.1.1/setup.cfg
--rw-rw-r--   0 emir      (1001) emir      (1001)      745 2023-05-28 12:59:16.000000 multi_stock_api-0.1.1/setup.py
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1064 2023-05-28 08:50:15.000000 multi_stock_api-0.1.2/LICENSE
+-rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/PKG-INFO
+-rw-rw-r--   0 emir      (1001) emir      (1001)       96 2023-05-28 12:28:24.000000 multi_stock_api-0.1.2/README.md
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.958508 multi_stock_api-0.1.2/multi_stock_api/
+-rw-rw-r--   0 emir      (1001) emir      (1001)       26 2023-05-28 12:17:47.000000 multi_stock_api-0.1.2/multi_stock_api/__init__.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1322 2023-05-28 12:18:46.000000 multi_stock_api-0.1.2/multi_stock_api/app.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1534 2023-05-28 12:18:38.000000 multi_stock_api-0.1.2/multi_stock_api/configurations.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      915 2023-05-28 12:18:32.000000 multi_stock_api-0.1.2/multi_stock_api/external_api_access.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      326 2023-05-28 12:01:51.000000 multi_stock_api-0.1.2/multi_stock_api/helpers.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      831 2023-05-28 12:18:52.000000 multi_stock_api-0.1.2/multi_stock_api/mappers.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      654 2023-05-28 12:03:50.000000 multi_stock_api-0.1.2/multi_stock_api/models.py
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/multi_stock_api.egg-info/
+-rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/PKG-INFO
+-rw-rw-r--   0 emir      (1001) emir      (1001)      424 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)        1 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)      490 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/requires.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)       16 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/top_level.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)       38 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/setup.cfg
+-rw-rw-r--   0 emir      (1001) emir      (1001)      745 2023-05-28 13:08:47.000000 multi_stock_api-0.1.2/setup.py
```

### Comparing `multi_stock_api-0.1.1/LICENSE` & `multi_stock_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/multi_stock_api/app.py` & `multi_stock_api-0.1.2/multi_stock_api/app.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/multi_stock_api/configurations.py` & `multi_stock_api-0.1.2/multi_stock_api/configurations.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/multi_stock_api/external_api_access.py` & `multi_stock_api-0.1.2/multi_stock_api/external_api_access.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/multi_stock_api/mappers.py` & `multi_stock_api-0.1.2/multi_stock_api/mappers.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/multi_stock_api/models.py` & `multi_stock_api-0.1.2/multi_stock_api/models.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.1/setup.py` & `multi_stock_api-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='multi_stock_api',
-    version='0.1.1',
+    version='0.1.2',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Emir Moćević',
     author_email='emirmocevic88@gmail.com',
     license='MIT',
     packages=['multi_stock_api'],
     include_package_data=True,
```

