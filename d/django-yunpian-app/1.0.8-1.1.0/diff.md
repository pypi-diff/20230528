# Comparing `tmp/django-yunpian-app-1.0.8.tar.gz` & `tmp/django-yunpian-app-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-yunpian-app-1.0.8.tar", last modified: Thu Jul  8 15:40:44 2021, max compression
+gzip compressed data, was "django-yunpian-app-1.1.0.tar", last modified: Sun May 28 02:55:18 2023, max compression
```

## Comparing `django-yunpian-app-1.0.8.tar` & `django-yunpian-app-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 wangx     (1000) wangx     (1001)        0 2021-07-08 15:40:19.475029 django-yunpian-app-1.0.8/
--rw-r--r--   0 wangx     (1000) wangx     (1001)    35149 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/LICENSE
--rw-r--r--   0 wangx     (1000) wangx     (1001)     1158 2021-07-08 15:40:44.094958 django-yunpian-app-1.0.8/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1001)      709 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/README.md
-drwxr-xr-x   0 wangx     (1000) wangx     (1001)        0 2021-07-08 15:40:19.471695 django-yunpian-app-1.0.8/django_yunpian/
--rw-r--r--   0 wangx     (1000) wangx     (1001)       28 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/__init__.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      539 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/admin.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      102 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/apps.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      387 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/exceptions.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1001)        0 2021-07-08 15:40:19.475029 django-yunpian-app-1.0.8/django_yunpian/migrations/
--rw-r--r--   0 wangx     (1000) wangx     (1001)     2562 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/migrations/0001_initial.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      760 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/migrations/0002_auto_20190823_1746.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      567 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/migrations/0003_auto_20190823_1900.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)      863 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/migrations/0004_auto_20190823_1939.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)        0 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/migrations/__init__.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)     3358 2021-07-08 15:39:18.000000 django-yunpian-app-1.0.8/django_yunpian/models.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)       60 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/tests.py
--rw-r--r--   0 wangx     (1000) wangx     (1001)       63 2020-04-05 12:28:12.000000 django-yunpian-app-1.0.8/django_yunpian/views.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1001)        0 2021-07-08 15:40:44.094958 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/
--rw-r--r--   0 wangx     (1000) wangx     (1001)     1158 2021-07-08 15:40:44.000000 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1001)      650 2021-07-08 15:40:44.000000 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/SOURCES.txt
--rw-r--r--   0 wangx     (1000) wangx     (1001)        1 2021-07-08 15:40:44.000000 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/dependency_links.txt
--rw-r--r--   0 wangx     (1000) wangx     (1001)       19 2021-07-08 15:40:44.000000 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/requires.txt
--rw-r--r--   0 wangx     (1000) wangx     (1001)       15 2021-07-08 15:40:44.000000 django-yunpian-app-1.0.8/django_yunpian_app.egg-info/top_level.txt
--rw-r--r--   0 wangx     (1000) wangx     (1001)       38 2021-07-08 15:40:44.094958 django-yunpian-app-1.0.8/setup.cfg
--rw-r--r--   0 wangx     (1000) wangx     (1001)      764 2020-04-05 12:41:35.000000 django-yunpian-app-1.0.8/setup.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-05-28 02:55:18.773750 django-yunpian-app-1.1.0/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)    35149 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/LICENSE
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1121 2023-05-28 02:55:18.772755 django-yunpian-app-1.1.0/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      709 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/README.md
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-05-28 02:55:18.745814 django-yunpian-app-1.1.0/django_yunpian/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       28 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/__init__.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      539 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/admin.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      102 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/apps.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      387 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/exceptions.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-05-28 02:55:18.755787 django-yunpian-app-1.1.0/django_yunpian/migrations/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     2562 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/0001_initial.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      760 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/0002_auto_20190823_1746.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      567 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/0003_auto_20190823_1900.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      863 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/0004_auto_20190823_1939.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1057 2023-05-28 02:05:49.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/0005_template_min_interval_alter_account_id_and_more.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        0 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/migrations/__init__.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     4060 2023-05-28 02:05:27.000000 django-yunpian-app-1.1.0/django_yunpian/models.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       60 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/tests.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       63 2023-05-28 01:46:09.000000 django-yunpian-app-1.1.0/django_yunpian/views.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-05-28 02:55:18.770747 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1121 2023-05-28 02:55:18.000000 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      732 2023-05-28 02:55:18.000000 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/SOURCES.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2023-05-28 02:55:18.000000 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/dependency_links.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       38 2023-05-28 02:55:18.000000 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/requires.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       15 2023-05-28 02:55:18.000000 django-yunpian-app-1.1.0/django_yunpian_app.egg-info/top_level.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       38 2023-05-28 02:55:18.773750 django-yunpian-app-1.1.0/setup.cfg
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      795 2023-05-28 02:54:19.000000 django-yunpian-app-1.1.0/setup.py
```

### Comparing `django-yunpian-app-1.0.8/LICENSE` & `django-yunpian-app-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/PKG-INFO` & `django-yunpian-app-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-yunpian-app
-Version: 1.0.8
+Version: 1.1.0
 Summary: 用于云片网的django app
 Home-page: https://github.com/ramwin/django-yunpian-app
 Author: Xiang Wang
 Author-email: ramwin@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-yunpian-app
@@ -56,9 +54,7 @@
 ```
 from django_yunpian.models import Message
 Message.objects.create(
     template = template,
     ...
 )
 ```
-
-
```

### Comparing `django-yunpian-app-1.0.8/README.md` & `django-yunpian-app-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian/admin.py` & `django-yunpian-app-1.1.0/django_yunpian/admin.py`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian/migrations/0001_initial.py` & `django-yunpian-app-1.1.0/django_yunpian/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian/migrations/0002_auto_20190823_1746.py` & `django-yunpian-app-1.1.0/django_yunpian/migrations/0002_auto_20190823_1746.py`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian/migrations/0003_auto_20190823_1900.py` & `django-yunpian-app-1.1.0/django_yunpian/migrations/0003_auto_20190823_1900.py`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian/migrations/0004_auto_20190823_1939.py` & `django-yunpian-app-1.1.0/django_yunpian/migrations/0004_auto_20190823_1939.py`

 * *Files identical despite different names*

### Comparing `django-yunpian-app-1.0.8/django_yunpian_app.egg-info/PKG-INFO` & `django-yunpian-app-1.1.0/django_yunpian_app.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-yunpian-app
-Version: 1.0.8
+Version: 1.1.0
 Summary: 用于云片网的django app
 Home-page: https://github.com/ramwin/django-yunpian-app
 Author: Xiang Wang
 Author-email: ramwin@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-yunpian-app
@@ -56,9 +54,7 @@
 ```
 from django_yunpian.models import Message
 Message.objects.create(
     template = template,
     ...
 )
 ```
-
-
```

### Comparing `django-yunpian-app-1.0.8/django_yunpian_app.egg-info/SOURCES.txt` & `django-yunpian-app-1.1.0/django_yunpian_app.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 django_yunpian/models.py
 django_yunpian/tests.py
 django_yunpian/views.py
 django_yunpian/migrations/0001_initial.py
 django_yunpian/migrations/0002_auto_20190823_1746.py
 django_yunpian/migrations/0003_auto_20190823_1900.py
 django_yunpian/migrations/0004_auto_20190823_1939.py
+django_yunpian/migrations/0005_template_min_interval_alter_account_id_and_more.py
 django_yunpian/migrations/__init__.py
 django_yunpian_app.egg-info/PKG-INFO
 django_yunpian_app.egg-info/SOURCES.txt
 django_yunpian_app.egg-info/dependency_links.txt
 django_yunpian_app.egg-info/requires.txt
 django_yunpian_app.egg-info/top_level.txt
```

### Comparing `django-yunpian-app-1.0.8/setup.py` & `django-yunpian-app-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-yunpian-app",
-    version="1.0.8",
+    version="1.1.0",
     author="Xiang Wang",
     author_email="ramwin@qq.com",
     description="用于云片网的django app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ramwin/django-yunpian-app",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "yunpian-python-sdk"
+        "djangorestframework",
     ],
 )
```

