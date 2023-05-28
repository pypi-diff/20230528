# Comparing `tmp/tv_db_api-0.1.2.tar.gz` & `tmp/tv_db_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tv_db_api-0.1.2.tar", last modified: Sun May 28 18:17:07 2023, max compression
+gzip compressed data, was "tv_db_api-0.1.3.tar", last modified: Sun May 28 18:53:01 2023, max compression
```

## Comparing `tv_db_api-0.1.2.tar` & `tv_db_api-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.583618 tv_db_api-0.1.2/
--rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/AUTHORS.rst
--rw-r--r--   0 paul       (501) staff       (20)     3578 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/HISTORY.rst
--rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:17:07.583720 tv_db_api-0.1.2/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      907 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.581804 tv_db_api-0.1.2/docs/
--rw-r--r--   0 paul       (501) staff       (20)      610 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/Makefile
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/authors.rst
--rwxr-xr-x   0 paul       (501) staff       (20)     4810 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/conf.py
--rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/contributing.rst
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/history.rst
--rw-r--r--   0 paul       (501) staff       (20)      306 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/index.rst
--rw-r--r--   0 paul       (501) staff       (20)     1170 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/installation.rst
--rw-r--r--   0 paul       (501) staff       (20)      771 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/make.bat
--rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/readme.rst
--rw-r--r--   0 paul       (501) staff       (20)       73 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/usage.rst
--rw-r--r--   0 paul       (501) staff       (20)      381 2023-05-28 18:17:07.584011 tv_db_api-0.1.2/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     1541 2023-05-28 18:16:55.000000 tv_db_api-0.1.2/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.582058 tv_db_api-0.1.2/tests/
--rw-r--r--   0 paul       (501) staff       (20)       39 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      397 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/tests/test_tv_db_api.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.582523 tv_db_api-0.1.2/tv_db_api/
--rw-r--r--   0 paul       (501) staff       (20)      138 2023-05-28 18:16:55.000000 tv_db_api-0.1.2/tv_db_api/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      263 2021-06-27 19:21:29.000000 tv_db_api-0.1.2/tv_db_api/default_field_config.py
--rw-r--r--   0 paul       (501) staff       (20)     6107 2023-05-28 18:16:17.000000 tv_db_api-0.1.2/tv_db_api/tv_db_api.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.583494 tv_db_api-0.1.2/tv_db_api.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      572 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 19:08:49.000000 tv_db_api-0.1.2/tv_db_api.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       31 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       10 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:53:01.085391 tv_db_api-0.1.3/
+-rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/AUTHORS.rst
+-rw-r--r--   0 paul       (501) staff       (20)     3578 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/HISTORY.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:53:01.085467 tv_db_api-0.1.3/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      907 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:53:01.083397 tv_db_api-0.1.3/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      610 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/Makefile
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 paul       (501) staff       (20)     4810 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/conf.py
+-rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/contributing.rst
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/history.rst
+-rw-r--r--   0 paul       (501) staff       (20)      306 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/index.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1170 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/installation.rst
+-rw-r--r--   0 paul       (501) staff       (20)      771 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/make.bat
+-rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/readme.rst
+-rw-r--r--   0 paul       (501) staff       (20)       73 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/docs/usage.rst
+-rw-r--r--   0 paul       (501) staff       (20)      381 2023-05-28 18:53:01.085748 tv_db_api-0.1.3/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     1541 2023-05-28 18:52:36.000000 tv_db_api-0.1.3/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:53:01.083749 tv_db_api-0.1.3/tests/
+-rw-r--r--   0 paul       (501) staff       (20)       39 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      397 2021-06-27 19:07:33.000000 tv_db_api-0.1.3/tests/test_tv_db_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:53:01.084251 tv_db_api-0.1.3/tv_db_api/
+-rw-r--r--   0 paul       (501) staff       (20)      138 2023-05-28 18:52:36.000000 tv_db_api-0.1.3/tv_db_api/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      263 2021-06-27 19:21:29.000000 tv_db_api-0.1.3/tv_db_api/default_field_config.py
+-rw-r--r--   0 paul       (501) staff       (20)     6109 2023-05-28 18:52:13.000000 tv_db_api-0.1.3/tv_db_api/tv_db_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:53:01.085249 tv_db_api-0.1.3/tv_db_api.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:53:01.000000 tv_db_api-0.1.3/tv_db_api.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      572 2023-05-28 18:53:01.000000 tv_db_api-0.1.3/tv_db_api.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-28 18:53:01.000000 tv_db_api-0.1.3/tv_db_api.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 19:08:49.000000 tv_db_api-0.1.3/tv_db_api.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       31 2023-05-28 18:53:01.000000 tv_db_api-0.1.3/tv_db_api.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       10 2023-05-28 18:53:01.000000 tv_db_api-0.1.3/tv_db_api.egg-info/top_level.txt
```

### Comparing `tv_db_api-0.1.2/CONTRIBUTING.rst` & `tv_db_api-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/LICENSE` & `tv_db_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/PKG-INFO` & `tv_db_api-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tv_db_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for interacting with the tv db api
 Home-page: https://github.com/paul-armstrong-dev/tv_db_api
 Author: Paul Armstrong
 Author-email: paul.armstrong211@gmail.com
 License: MIT license
 Keywords: tv_db_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tv_db_api-0.1.2/README.rst` & `tv_db_api-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/docs/Makefile` & `tv_db_api-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/docs/conf.py` & `tv_db_api-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/docs/installation.rst` & `tv_db_api-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/docs/make.bat` & `tv_db_api-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.2/setup.py` & `tv_db_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords='tv_db_api',
     name='tv_db_api',
     packages=find_packages(include=['tv_db_api', 'tv_db_api.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/paul-armstrong-dev/tv_db_api',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `tv_db_api-0.1.2/tv_db_api/tv_db_api.py` & `tv_db_api-0.1.3/tv_db_api/tv_db_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         :param show_fields:
         :type show_fields:
         """
         self.class_name = type(self).__name__
         logger.info(f"{self.class_name} initialised")
 
         if episode_fields is None:
-            from default_field_config import default_episode_fields
+            from .default_field_config import default_episode_fields
             self.episode_fields = default_episode_fields
         else:
             self.episode_fields = episode_fields
 
         if show_fields is None:
-            from default_field_config import default_show_fields
+            from .default_field_config import default_show_fields
             self.show_fields = default_show_fields
         else:
             self.show_fields = show_fields
 
         if shows_to_ignore is None:
             self.shows_to_ignore = []
         else:
```

### Comparing `tv_db_api-0.1.2/tv_db_api.egg-info/PKG-INFO` & `tv_db_api-0.1.3/tv_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tv-db-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for interacting with the tv db api
 Home-page: https://github.com/paul-armstrong-dev/tv_db_api
 Author: Paul Armstrong
 Author-email: paul.armstrong211@gmail.com
 License: MIT license
 Keywords: tv_db_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tv_db_api-0.1.2/tv_db_api.egg-info/SOURCES.txt` & `tv_db_api-0.1.3/tv_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

