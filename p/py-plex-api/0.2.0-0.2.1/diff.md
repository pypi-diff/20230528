# Comparing `tmp/py_plex_api-0.2.0.tar.gz` & `tmp/py_plex_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py_plex_api-0.2.0.tar", last modified: Fri Jul 16 13:46:19 2021, max compression
+gzip compressed data, was "py_plex_api-0.2.1.tar", last modified: Sun May 28 18:25:37 2023, max compression
```

## Comparing `py_plex_api-0.2.0.tar` & `py_plex_api-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-07-16 13:46:19.868748 py_plex_api-0.2.0/
--rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/AUTHORS.rst
--rw-r--r--   0 paul       (501) staff       (20)     3596 2021-06-27 18:28:21.000000 py_plex_api-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/HISTORY.rst
--rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)     1610 2021-07-16 13:46:19.868958 py_plex_api-0.2.0/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      766 2021-06-27 18:48:13.000000 py_plex_api-0.2.0/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-07-16 13:46:19.853948 py_plex_api-0.2.0/docs/
--rw-r--r--   0 paul       (501) staff       (20)      609 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/Makefile
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/authors.rst
--rwxr-xr-x   0 paul       (501) staff       (20)     4760 2021-06-27 18:41:39.000000 py_plex_api-0.2.0/docs/conf.py
--rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/contributing.rst
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/history.rst
--rw-r--r--   0 paul       (501) staff       (20)      305 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/index.rst
--rw-r--r--   0 paul       (501) staff       (20)     1162 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/installation.rst
--rw-r--r--   0 paul       (501) staff       (20)      770 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/make.bat
--rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/readme.rst
--rw-r--r--   0 paul       (501) staff       (20)       71 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/docs/usage.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-07-16 13:46:19.856280 py_plex_api-0.2.0/py_plex_api/
--rw-r--r--   0 paul       (501) staff       (20)      164 2021-07-16 13:44:36.000000 py_plex_api-0.2.0/py_plex_api/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     9275 2021-07-16 13:40:42.000000 py_plex_api-0.2.0/py_plex_api/py_plex_api.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-07-16 13:46:19.865105 py_plex_api-0.2.0/py_plex_api.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     1610 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      593 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)       54 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 18:32:25.000000 py_plex_api-0.2.0/py_plex_api.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       31 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       12 2021-07-16 13:46:19.000000 py_plex_api-0.2.0/py_plex_api.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)      383 2021-07-16 13:46:19.870058 py_plex_api-0.2.0/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     1662 2021-07-16 13:44:36.000000 py_plex_api-0.2.0/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-07-16 13:46:19.868013 py_plex_api-0.2.0/tests/
--rw-r--r--   0 paul       (501) staff       (20)       38 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      392 2021-06-27 17:56:44.000000 py_plex_api-0.2.0/tests/test_plex_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:25:37.641456 py_plex_api-0.2.1/
+-rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/AUTHORS.rst
+-rw-r--r--   0 paul       (501) staff       (20)     3596 2021-06-27 18:28:21.000000 py_plex_api-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/HISTORY.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     1590 2023-05-28 18:25:37.641526 py_plex_api-0.2.1/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      766 2021-06-27 18:48:13.000000 py_plex_api-0.2.1/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:25:37.639548 py_plex_api-0.2.1/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      609 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/Makefile
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 paul       (501) staff       (20)     4760 2021-06-27 18:41:39.000000 py_plex_api-0.2.1/docs/conf.py
+-rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/contributing.rst
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/history.rst
+-rw-r--r--   0 paul       (501) staff       (20)      305 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/index.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1162 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/installation.rst
+-rw-r--r--   0 paul       (501) staff       (20)      770 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/make.bat
+-rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/readme.rst
+-rw-r--r--   0 paul       (501) staff       (20)       71 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/docs/usage.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:25:37.639834 py_plex_api-0.2.1/py_plex_api/
+-rw-r--r--   0 paul       (501) staff       (20)      164 2023-05-28 18:25:24.000000 py_plex_api-0.2.1/py_plex_api/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     9259 2023-05-28 18:24:59.000000 py_plex_api-0.2.1/py_plex_api/py_plex_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:25:37.641007 py_plex_api-0.2.1/py_plex_api.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     1590 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      593 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)       53 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 18:32:25.000000 py_plex_api-0.2.1/py_plex_api.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       31 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       12 2023-05-28 18:25:37.000000 py_plex_api-0.2.1/py_plex_api.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-28 18:25:37.642169 py_plex_api-0.2.1/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     1662 2023-05-28 18:25:24.000000 py_plex_api-0.2.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:25:37.641322 py_plex_api-0.2.1/tests/
+-rw-r--r--   0 paul       (501) staff       (20)       38 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      392 2021-06-27 17:56:44.000000 py_plex_api-0.2.1/tests/test_plex_api.py
```

### Comparing `py_plex_api-0.2.0/CONTRIBUTING.rst` & `py_plex_api-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/LICENSE` & `py_plex_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/PKG-INFO` & `py_plex_api-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: py_plex_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: API wrapper for interacting with a Plex Server
 Home-page: https://github.com/paul-armstrong-dev/py_plex_api
 Author: Paul Armstrong
 Author-email: paul.armstrong211@gmail.com
 License: MIT license
 Keywords: py_plex_api
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -61,9 +60,7 @@
 History
 =======
 
 0.1.0 (2021-06-27)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `py_plex_api-0.2.0/README.rst` & `py_plex_api-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/docs/Makefile` & `py_plex_api-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/docs/conf.py` & `py_plex_api-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/docs/installation.rst` & `py_plex_api-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/docs/make.bat` & `py_plex_api-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/py_plex_api/py_plex_api.py` & `py_plex_api-0.2.1/py_plex_api/py_plex_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,25 +233,25 @@
         logger.info("Getting movie info")
         return self.get_plex_section_content("Movies")
 
     def get_show_info(self):
         logger.info("Getting show info")
         return self.get_plex_section_content("TV Shows")
 
-    def get_all_plex_info(self) -> (List):
+    def get_all_plex_info(self) -> (Dict):
         """
         
         :return:
         """
         
         # Sections
         
         logger.info("Getting library sections")
 
-        all_data = []
+        all_data = {}
 
-        all_data.append({"movies": self.get_movie_info()})
-        all_data.append({"shows": self.get_show_info()})
+        all_data["movies"] = self.get_movie_info()
+        all_data["shows"] = self.get_show_info()
 
         return all_data
```

### Comparing `py_plex_api-0.2.0/py_plex_api.egg-info/PKG-INFO` & `py_plex_api-0.2.1/py_plex_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: py-plex-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: API wrapper for interacting with a Plex Server
 Home-page: https://github.com/paul-armstrong-dev/py_plex_api
 Author: Paul Armstrong
 Author-email: paul.armstrong211@gmail.com
 License: MIT license
 Keywords: py_plex_api
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -61,9 +60,7 @@
 History
 =======
 
 0.1.0 (2021-06-27)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `py_plex_api-0.2.0/py_plex_api.egg-info/SOURCES.txt` & `py_plex_api-0.2.1/py_plex_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_plex_api-0.2.0/setup.py` & `py_plex_api-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     include_package_data=True,
     keywords='py_plex_api',
     name='py_plex_api',
     packages=find_packages(include=['py_plex_api', 'py_plex_api.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/paul-armstrong-dev/py_plex_api',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

