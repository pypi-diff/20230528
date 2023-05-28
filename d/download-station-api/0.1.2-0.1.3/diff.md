# Comparing `tmp/download_station_api-0.1.2.tar.gz` & `tmp/download_station_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/paul/Dev/GitHub/download-station-api/dist/tmp4eulon54/download_station_api-0.1.2.tar", last modified: Sun Jun 27 17:49:49 2021, max compression
+gzip compressed data, was "download_station_api-0.1.3.tar", last modified: Sun May 28 14:27:29 2023, max compression
```

## Comparing `download_station_api-0.1.2.tar` & `download_station_api-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.922746 download_station_api-0.1.2/
--rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 16:43:11.000000 download_station_api-0.1.2/AUTHORS.rst
--rw-r--r--   0 paul       (501) staff       (20)     3710 2021-06-26 17:38:47.000000 download_station_api-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 paul       (501) staff       (20)       94 2021-06-27 16:24:13.000000 download_station_api-0.1.2/HISTORY.rst
--rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-26 17:38:47.000000 download_station_api-0.1.2/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-26 17:38:47.000000 download_station_api-0.1.2/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)     2170 2021-06-27 17:49:49.922881 download_station_api-0.1.2/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1260 2021-06-27 17:38:49.000000 download_station_api-0.1.2/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.907061 download_station_api-0.1.2/docs/
--rw-r--r--   0 paul       (501) staff       (20)      621 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/Makefile
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.873562 download_station_api-0.1.2/docs/_build/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.873770 download_station_api-0.1.2/docs/_build/html/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.910546 download_station_api-0.1.2/docs/_build/html/_static/
--rw-r--r--   0 paul       (501) staff       (20)      286 2021-06-27 14:02:43.000000 download_station_api-0.1.2/docs/_build/html/_static/file.png
--rw-r--r--   0 paul       (501) staff       (20)       90 2021-06-27 14:02:43.000000 download_station_api-0.1.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 paul       (501) staff       (20)       90 2021-06-27 14:02:43.000000 download_station_api-0.1.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 paul       (501) staff       (20)      695 2021-06-27 14:15:38.000000 download_station_api-0.1.2/docs/_build/html/_static/py.png
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/authors.rst
--rw-r--r--   0 paul       (501) staff       (20)      154 2021-06-27 15:47:44.000000 download_station_api-0.1.2/docs/class_documentation.rst
--rwxr-xr-x   0 paul       (501) staff       (20)     4888 2021-06-27 16:45:19.000000 download_station_api-0.1.2/docs/conf.py
--rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/contributing.rst
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/history.rst
--rw-r--r--   0 paul       (501) staff       (20)      340 2021-06-27 16:22:48.000000 download_station_api-0.1.2/docs/index.rst
--rw-r--r--   0 paul       (501) staff       (20)     1258 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/installation.rst
--rw-r--r--   0 paul       (501) staff       (20)      782 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/make.bat
--rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/readme.rst
--rw-r--r--   0 paul       (501) staff       (20)       95 2021-06-26 17:38:47.000000 download_station_api-0.1.2/docs/usage.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.912381 download_station_api-0.1.2/download_station_api/
--rw-r--r--   0 paul       (501) staff       (20)      206 2021-06-27 17:48:53.000000 download_station_api-0.1.2/download_station_api/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)    14007 2021-06-27 16:22:09.000000 download_station_api-0.1.2/download_station_api/download_station_api.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.920614 download_station_api-0.1.2/download_station_api/utils/
--rw-r--r--   0 paul       (501) staff       (20)      111 2021-06-27 14:59:29.000000 download_station_api-0.1.2/download_station_api/utils/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      872 2021-06-27 15:00:09.000000 download_station_api-0.1.2/download_station_api/utils/api_endpoint_details.py
--rw-r--r--   0 paul       (501) staff       (20)       35 2021-06-27 15:00:09.000000 download_station_api-0.1.2/download_station_api/utils/auth_error.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.918048 download_station_api-0.1.2/download_station_api.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2170 2021-06-27 17:49:49.000000 download_station_api-0.1.2/download_station_api.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      943 2021-06-27 17:49:49.000000 download_station_api-0.1.2/download_station_api.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 17:49:49.000000 download_station_api-0.1.2/download_station_api.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-26 17:48:18.000000 download_station_api-0.1.2/download_station_api.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       31 2021-06-27 17:49:49.000000 download_station_api-0.1.2/download_station_api.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       21 2021-06-27 17:49:49.000000 download_station_api-0.1.2/download_station_api.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)      392 2021-06-27 17:49:49.924005 download_station_api-0.1.2/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     2051 2021-06-27 17:48:53.000000 download_station_api-0.1.2/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 17:49:49.922194 download_station_api-0.1.2/tests/
--rw-r--r--   0 paul       (501) staff       (20)       50 2021-06-26 17:38:47.000000 download_station_api-0.1.2/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      452 2021-06-26 17:38:47.000000 download_station_api-0.1.2/tests/test_download_station_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.111053 download_station_api-0.1.3/
+-rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 16:43:11.000000 download_station_api-0.1.3/AUTHORS.rst
+-rw-r--r--   0 paul       (501) staff       (20)     3710 2021-06-26 17:38:47.000000 download_station_api-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 paul       (501) staff       (20)       94 2021-06-27 16:24:13.000000 download_station_api-0.1.3/HISTORY.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-26 17:38:47.000000 download_station_api-0.1.3/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-26 17:38:47.000000 download_station_api-0.1.3/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     2150 2023-05-28 14:27:29.111117 download_station_api-0.1.3/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1260 2021-06-27 17:38:49.000000 download_station_api-0.1.3/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.108194 download_station_api-0.1.3/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      621 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/Makefile
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.105317 download_station_api-0.1.3/docs/_build/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.105372 download_station_api-0.1.3/docs/_build/html/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.109172 download_station_api-0.1.3/docs/_build/html/_static/
+-rw-r--r--   0 paul       (501) staff       (20)      286 2021-06-27 14:02:43.000000 download_station_api-0.1.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 paul       (501) staff       (20)       90 2021-06-27 14:02:43.000000 download_station_api-0.1.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 paul       (501) staff       (20)       90 2021-06-27 14:02:43.000000 download_station_api-0.1.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 paul       (501) staff       (20)      695 2021-06-27 14:15:38.000000 download_station_api-0.1.3/docs/_build/html/_static/py.png
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/authors.rst
+-rw-r--r--   0 paul       (501) staff       (20)      154 2021-06-27 15:47:44.000000 download_station_api-0.1.3/docs/class_documentation.rst
+-rwxr-xr-x   0 paul       (501) staff       (20)     4888 2021-06-27 16:45:19.000000 download_station_api-0.1.3/docs/conf.py
+-rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/contributing.rst
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/history.rst
+-rw-r--r--   0 paul       (501) staff       (20)      340 2021-06-27 16:22:48.000000 download_station_api-0.1.3/docs/index.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1258 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/installation.rst
+-rw-r--r--   0 paul       (501) staff       (20)      782 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/make.bat
+-rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/readme.rst
+-rw-r--r--   0 paul       (501) staff       (20)       95 2021-06-26 17:38:47.000000 download_station_api-0.1.3/docs/usage.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.109473 download_station_api-0.1.3/download_station_api/
+-rw-r--r--   0 paul       (501) staff       (20)      206 2023-05-28 14:20:40.000000 download_station_api-0.1.3/download_station_api/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)    14096 2023-05-28 14:20:40.000000 download_station_api-0.1.3/download_station_api/download_station_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.110675 download_station_api-0.1.3/download_station_api/utils/
+-rw-r--r--   0 paul       (501) staff       (20)      111 2021-06-27 14:59:29.000000 download_station_api-0.1.3/download_station_api/utils/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      872 2023-05-28 14:20:40.000000 download_station_api-0.1.3/download_station_api/utils/api_endpoint_details.py
+-rw-r--r--   0 paul       (501) staff       (20)       35 2021-06-27 15:00:09.000000 download_station_api-0.1.3/download_station_api/utils/auth_error.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.110285 download_station_api-0.1.3/download_station_api.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     2150 2023-05-28 14:27:29.000000 download_station_api-0.1.3/download_station_api.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      943 2023-05-28 14:27:29.000000 download_station_api-0.1.3/download_station_api.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-28 14:27:29.000000 download_station_api-0.1.3/download_station_api.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-26 17:48:18.000000 download_station_api-0.1.3/download_station_api.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       31 2023-05-28 14:27:29.000000 download_station_api-0.1.3/download_station_api.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       21 2023-05-28 14:27:29.000000 download_station_api-0.1.3/download_station_api.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)      392 2023-05-28 14:27:29.111381 download_station_api-0.1.3/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     2051 2023-05-28 14:20:40.000000 download_station_api-0.1.3/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 14:27:29.110931 download_station_api-0.1.3/tests/
+-rw-r--r--   0 paul       (501) staff       (20)       50 2021-06-26 17:38:47.000000 download_station_api-0.1.3/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      452 2021-06-26 17:38:47.000000 download_station_api-0.1.3/tests/test_download_station_api.py
```

### Comparing `download_station_api-0.1.2/CONTRIBUTING.rst` & `download_station_api-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/LICENSE` & `download_station_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/PKG-INFO` & `download_station_api-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: download_station_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small python wrapper for interacting with the Synology Download Station
 Home-page: https://github.com/paul-armstrong-dev/download_station_api
 Author: Paul Armstrong
 Author-email: paul_armstrong211@gmail.com
 License: MIT license
 Keywords: download_station_api,synology
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -61,9 +60,7 @@
 =======
 History
 =======
 
 0.1.1 (2021-06-26)
 ------------------
 * First release & update PyPI.
-
-
```

### Comparing `download_station_api-0.1.2/README.rst` & `download_station_api-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/docs/Makefile` & `download_station_api-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/docs/_build/html/_static/py.png` & `download_station_api-0.1.3/docs/_build/html/_static/py.png`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/docs/conf.py` & `download_station_api-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/docs/installation.rst` & `download_station_api-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/docs/make.bat` & `download_station_api-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/download_station_api/download_station_api.py` & `download_station_api-0.1.3/download_station_api/download_station_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.nas_ip = nas_ip
         self.api_endpoint = api_endpoint
         self.api_port = api_port
         self.nas_address = f"http://{self.nas_ip}:{api_port}/{api_endpoint}"
         self.session_id = self.authenticate(session='DownloadStation',
                                             auth_format='cookie',
                                             method='login',
-                                            version=2)
+                                            version=3)
 
     def _get_api_data(self, api_endpoint: str, params: Dict, return_json: bool = True):
         """
 
         :param api_endpoint: self-explanatory
         :param params: Request params be passed through to API
         :param return_json: Specify whether to return json/dict or the entire requests.response
@@ -66,14 +66,17 @@
         response = requests.get(api_url, params=params)
 
         if return_json:
             return response.json()
         else:
             return response
 
+    def __enter__(self):
+        logger.info(f"{self.class_name} entered successfully")
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is not None:
             logger.error(
                 'Problem in {class_name}'.format(class_name=self.class_name))
             logger.error(exc_type)
             logger.error(exc_val)
             exit(1)
```

### Comparing `download_station_api-0.1.2/download_station_api/utils/api_endpoint_details.py` & `download_station_api-0.1.3/download_station_api/utils/api_endpoint_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 nas_api_endpoint_details = {
     'API_Info'    : {'maxVersion'  : 1, 'minVersion': 1, 'path': 'query.cgi',
                      'api_endpoint': 'SYNO.API.Info'},
-    'API_Auth'    : {'maxVersion'  : 6, 'minVersion': 1, 'path': 'auth.cgi',
+    'API_Auth'    : {'maxVersion'  : 7, 'minVersion': 1, 'path': 'auth.cgi',
                      'api_endpoint': 'SYNO.API.Auth'},
     'DS_Info'     : {'maxVersion'  : 2, 'minVersion': 1,
                      'path'        : 'DownloadStation/info.cgi',
                      'api_endpoint': 'SYNO.DownloadStation.Info'},
     'DS_BT_Search': {'maxVersion'  : 1, 'minVersion': 1,
                      'path'        : 'DownloadStation/btsearch.cgi',
                      'api_endpoint': 'SYNO.DownloadStation.BTSearch'},
```

### Comparing `download_station_api-0.1.2/download_station_api.egg-info/PKG-INFO` & `download_station_api-0.1.3/download_station_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: download-station-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small python wrapper for interacting with the Synology Download Station
 Home-page: https://github.com/paul-armstrong-dev/download_station_api
 Author: Paul Armstrong
 Author-email: paul_armstrong211@gmail.com
 License: MIT license
 Keywords: download_station_api,synology
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -61,9 +60,7 @@
 =======
 History
 =======
 
 0.1.1 (2021-06-26)
 ------------------
 * First release & update PyPI.
-
-
```

### Comparing `download_station_api-0.1.2/download_station_api.egg-info/SOURCES.txt` & `download_station_api-0.1.3/download_station_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `download_station_api-0.1.2/setup.py` & `download_station_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     include_package_data=True,
     keywords='download_station_api, synology',
     name='download_station_api',
     packages=find_packages(include=['download_station_api', 'download_station_api.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/paul-armstrong-dev/download_station_api',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

