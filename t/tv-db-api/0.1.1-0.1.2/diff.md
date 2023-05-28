# Comparing `tmp/tv_db_api-0.1.1.tar.gz` & `tmp/tv_db_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tv_db_api-0.1.1.tar", last modified: Sun Jun 27 19:46:34 2021, max compression
+gzip compressed data, was "tv_db_api-0.1.2.tar", last modified: Sun May 28 18:17:07 2023, max compression
```

## Comparing `tv_db_api-0.1.1.tar` & `tv_db_api-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/
--rw-r--r--   0 paul       (501) staff       (20)     2087 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)     3578 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/CONTRIBUTING.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tests/
--rw-r--r--   0 paul       (501) staff       (20)       39 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      397 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/tests/test_tv_db_api.py
--rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/MANIFEST.in
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/docs/
--rw-r--r--   0 paul       (501) staff       (20)      306 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/index.rst
--rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/contributing.rst
--rw-r--r--   0 paul       (501) staff       (20)      610 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/Makefile
--rwxr-xr-x   0 paul       (501) staff       (20)     4810 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/conf.py
--rw-r--r--   0 paul       (501) staff       (20)       73 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/usage.rst
--rw-r--r--   0 paul       (501) staff       (20)      771 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/make.bat
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/history.rst
--rw-r--r--   0 paul       (501) staff       (20)     1170 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/installation.rst
--rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/authors.rst
--rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/docs/readme.rst
--rw-r--r--   0 paul       (501) staff       (20)     1541 2021-06-27 19:45:58.000000 tv_db_api-0.1.1/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2087 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 19:08:49.000000 tv_db_api-0.1.1/tv_db_api.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)      558 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)       31 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       10 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/HISTORY.rst
--rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/AUTHORS.rst
--rw-r--r--   0 paul       (501) staff       (20)      381 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)      907 2021-06-27 19:07:33.000000 tv_db_api-0.1.1/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2021-06-27 19:46:34.000000 tv_db_api-0.1.1/tv_db_api/
--rw-r--r--   0 paul       (501) staff       (20)     6079 2021-06-27 19:35:30.000000 tv_db_api-0.1.1/tv_db_api/tv_db_api.py
--rw-r--r--   0 paul       (501) staff       (20)      263 2021-06-27 19:21:29.000000 tv_db_api-0.1.1/tv_db_api/config.py
--rw-r--r--   0 paul       (501) staff       (20)      138 2021-06-27 19:45:58.000000 tv_db_api-0.1.1/tv_db_api/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.583618 tv_db_api-0.1.2/
+-rw-r--r--   0 paul       (501) staff       (20)      167 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/AUTHORS.rst
+-rw-r--r--   0 paul       (501) staff       (20)     3578 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 paul       (501) staff       (20)       89 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/HISTORY.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1073 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)      262 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:17:07.583720 tv_db_api-0.1.2/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      907 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.581804 tv_db_api-0.1.2/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      610 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/Makefile
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 paul       (501) staff       (20)     4810 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/conf.py
+-rw-r--r--   0 paul       (501) staff       (20)       33 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/contributing.rst
+-rw-r--r--   0 paul       (501) staff       (20)       28 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/history.rst
+-rw-r--r--   0 paul       (501) staff       (20)      306 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/index.rst
+-rw-r--r--   0 paul       (501) staff       (20)     1170 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/installation.rst
+-rw-r--r--   0 paul       (501) staff       (20)      771 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/make.bat
+-rw-r--r--   0 paul       (501) staff       (20)       27 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/readme.rst
+-rw-r--r--   0 paul       (501) staff       (20)       73 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/docs/usage.rst
+-rw-r--r--   0 paul       (501) staff       (20)      381 2023-05-28 18:17:07.584011 tv_db_api-0.1.2/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     1541 2023-05-28 18:16:55.000000 tv_db_api-0.1.2/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.582058 tv_db_api-0.1.2/tests/
+-rw-r--r--   0 paul       (501) staff       (20)       39 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      397 2021-06-27 19:07:33.000000 tv_db_api-0.1.2/tests/test_tv_db_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.582523 tv_db_api-0.1.2/tv_db_api/
+-rw-r--r--   0 paul       (501) staff       (20)      138 2023-05-28 18:16:55.000000 tv_db_api-0.1.2/tv_db_api/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      263 2021-06-27 19:21:29.000000 tv_db_api-0.1.2/tv_db_api/default_field_config.py
+-rw-r--r--   0 paul       (501) staff       (20)     6107 2023-05-28 18:16:17.000000 tv_db_api-0.1.2/tv_db_api/tv_db_api.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-28 18:17:07.583494 tv_db_api-0.1.2/tv_db_api.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     1728 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      572 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2021-06-27 19:08:49.000000 tv_db_api-0.1.2/tv_db_api.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       31 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       10 2023-05-28 18:17:07.000000 tv_db_api-0.1.2/tv_db_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tv_db_api-0.1.1/PKG-INFO` & `tv_db_api-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,68 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tv_db_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for interacting with the tv db api
 Home-page: https://github.com/paul-armstrong-dev/tv_db_api
 Author: Paul Armstrong
 Author-email: paul.armstrong211@gmail.com
 License: MIT license
-Description: =========
-        tv-db-api
-        =========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/tv_db_api.svg
-                :target: https://pypi.python.org/pypi/tv_db_api
-        
-        .. image:: https://img.shields.io/travis/paul-armstrong-dev/tv_db_api.svg
-                :target: https://travis-ci.com/paul-armstrong-dev/tv_db_api
-        
-        .. image:: https://readthedocs.org/projects/tv-db-api/badge/?version=latest
-                :target: https://tv-db-api.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Python wrapper for interacting with the tv db api
-        
-        
-        * Free software: MIT license
-        * Documentation: https://tv-db-api.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-06-27)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: tv_db_api
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=========
+tv-db-api
+=========
+
+
+.. image:: https://img.shields.io/pypi/v/tv_db_api.svg
+        :target: https://pypi.python.org/pypi/tv_db_api
+
+.. image:: https://img.shields.io/travis/paul-armstrong-dev/tv_db_api.svg
+        :target: https://travis-ci.com/paul-armstrong-dev/tv_db_api
+
+.. image:: https://readthedocs.org/projects/tv-db-api/badge/?version=latest
+        :target: https://tv-db-api.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Python wrapper for interacting with the tv db api
+
+
+* Free software: MIT license
+* Documentation: https://tv-db-api.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-06-27)
+------------------
+
+* First release on PyPI.
```

### Comparing `tv_db_api-0.1.1/LICENSE` & `tv_db_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/CONTRIBUTING.rst` & `tv_db_api-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/docs/Makefile` & `tv_db_api-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/docs/conf.py` & `tv_db_api-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/docs/make.bat` & `tv_db_api-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/docs/installation.rst` & `tv_db_api-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/setup.py` & `tv_db_api-0.1.2/setup.py`

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
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `tv_db_api-0.1.1/tv_db_api.egg-info/SOURCES.txt` & `tv_db_api-0.1.2/tv_db_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
 tests/test_tv_db_api.py
 tv_db_api/__init__.py
-tv_db_api/config.py
+tv_db_api/default_field_config.py
 tv_db_api/tv_db_api.py
 tv_db_api.egg-info/PKG-INFO
 tv_db_api.egg-info/SOURCES.txt
 tv_db_api.egg-info/dependency_links.txt
 tv_db_api.egg-info/not-zip-safe
 tv_db_api.egg-info/requires.txt
 tv_db_api.egg-info/top_level.txt
```

### Comparing `tv_db_api-0.1.1/README.rst` & `tv_db_api-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `tv_db_api-0.1.1/tv_db_api/tv_db_api.py` & `tv_db_api-0.1.2/tv_db_api/tv_db_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         :param show_fields:
         :type show_fields:
         """
         self.class_name = type(self).__name__
         logger.info(f"{self.class_name} initialised")
 
         if episode_fields is None:
-            from config import default_episode_fields
+            from default_field_config import default_episode_fields
             self.episode_fields = default_episode_fields
         else:
             self.episode_fields = episode_fields
 
         if show_fields is None:
-            from config import default_show_fields
+            from default_field_config import default_show_fields
             self.show_fields = default_show_fields
         else:
             self.show_fields = show_fields
 
         if shows_to_ignore is None:
             self.shows_to_ignore = []
         else:
```

