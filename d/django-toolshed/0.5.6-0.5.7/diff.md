# Comparing `tmp/django_toolshed-0.5.6.tar.gz` & `tmp/django_toolshed-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_toolshed-0.5.6.tar", max compression
+gzip compressed data, was "django_toolshed-0.5.7.tar", max compression
```

## Comparing `django_toolshed-0.5.6.tar` & `django_toolshed-0.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/LICENSE
--rw-r--r--   0        0        0       22 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/__init__.py
--rw-r--r--   0        0        0      292 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/apps.py
--rwxr-xr-x   0        0        0     1381 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/celery_auto_app.py
--rw-r--r--   0        0        0      254 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/celery_urls.py
--rw-r--r--   0        0        0     3156 2023-05-28 11:56:50.471025 django_toolshed-0.5.6/django_toolshed/celery_views.py
--rw-r--r--   0        0        0      969 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/create_management_command.py
--rw-r--r--   0        0        0      264 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_apps.py
--rw-r--r--   0        0        0      637 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_commands.py
--rw-r--r--   0        0        0      321 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_users.py
--rw-r--r--   0        0        0     1797 2023-05-28 11:56:50.471025 django_toolshed-0.5.6/django_toolshed/mixins.py
--rw-r--r--   0        0        0       37 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/signals.py
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/css/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/images/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/js/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/templates/django_toolshed/.gitkeep
--rw-r--r--   0        0        0       47 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/urls.py
--rw-r--r--   0        0        0     1148 2023-05-28 11:56:51.851087 django_toolshed-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 django_toolshed-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/apps.py
+-rwxr-xr-x   0        0        0     1381 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/celery_auto_app.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/celery_urls.py
+-rw-r--r--   0        0        0     3156 2023-05-28 11:56:50.471025 django_toolshed-0.5.7/django_toolshed/celery_views.py
+-rw-r--r--   0        0        0      969 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/management/commands/create_management_command.py
+-rw-r--r--   0        0        0      264 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/management/commands/list_apps.py
+-rw-r--r--   0        0        0      637 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/management/commands/list_commands.py
+-rw-r--r--   0        0        0      321 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/management/commands/list_users.py
+-rw-r--r--   0        0        0     1797 2023-05-28 11:56:50.471025 django_toolshed-0.5.7/django_toolshed/mixins.py
+-rw-r--r--   0        0        0       37 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/signals.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/static/django_toolshed/css/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/static/django_toolshed/images/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/static/django_toolshed/js/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/templates/django_toolshed/.gitkeep
+-rw-r--r--   0        0        0       47 2023-05-26 16:33:22.599223 django_toolshed-0.5.7/django_toolshed/urls.py
+-rw-r--r--   0        0        0     1106 2023-05-28 12:35:40.211093 django_toolshed-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 django_toolshed-0.5.7/PKG-INFO
```

### Comparing `django_toolshed-0.5.6/LICENSE` & `django_toolshed-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/django_toolshed/celery_auto_app.py` & `django_toolshed-0.5.7/django_toolshed/celery_auto_app.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/django_toolshed/celery_views.py` & `django_toolshed-0.5.7/django_toolshed/celery_views.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/django_toolshed/management/commands/create_management_command.py` & `django_toolshed-0.5.7/django_toolshed/management/commands/create_management_command.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/django_toolshed/management/commands/list_commands.py` & `django_toolshed-0.5.7/django_toolshed/management/commands/list_commands.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/django_toolshed/mixins.py` & `django_toolshed-0.5.7/django_toolshed/mixins.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.6/pyproject.toml` & `django_toolshed-0.5.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "django-toolshed"
-version = "0.5.6"
+version = "0.5.7"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 celery-auto-app = "django_toolshed.celery_auto_app:command"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-ipython_genutils = "^0.2.0"
-django-click = "^2.2.0"
+django-click = "2.x"
 iterfzf = "^0.5.0"
-djangorestframework = "^3.13.1"
-celery = "^5.2.1"
-drf-spectacular = "^0.26.2"
+djangorestframework = "3.x"
+celery = "5.x"
+drf-spectacular = "0.x"
 
 [tool.poetry.dev-dependencies]
 pytest = "6.2.2"
 pytest-clarity = "0.2.0a1"
 pytest-cov = "2.10.0"
 pytest-django = "4.1.0"
 coverage = "5.5"
```

### Comparing `django_toolshed-0.5.6/PKG-INFO` & `django_toolshed-0.5.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-toolshed
-Version: 0.5.6
+Version: 0.5.7
 Summary: 
 License: MIT
 Author: Dani Hodovic
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: celery (>=5.2.1,<6.0.0)
-Requires-Dist: django-click (>=2.2.0,<3.0.0)
-Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
-Requires-Dist: drf-spectacular (>=0.26.2,<0.27.0)
-Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0)
+Requires-Dist: celery (==5.*)
+Requires-Dist: django-click (==2.*)
+Requires-Dist: djangorestframework (==3.*)
+Requires-Dist: drf-spectacular (==0.*)
 Requires-Dist: iterfzf (>=0.5.0,<0.6.0)
```

