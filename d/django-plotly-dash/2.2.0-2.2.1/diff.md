# Comparing `tmp/django-plotly-dash-2.2.0.tar.gz` & `tmp/django-plotly-dash-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plotly-dash-2.2.0.tar", last modified: Wed May  3 05:50:15 2023, max compression
+gzip compressed data, was "django-plotly-dash-2.2.1.tar", last modified: Sun May 28 17:40:22 2023, max compression
```

## Comparing `django-plotly-dash-2.2.0.tar` & `django-plotly-dash-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.786577 django-plotly-dash-2.2.0/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1107 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)       53 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/MANIFEST.in
--rw-rw-r--   0 mark      (1000) mark      (1000)     6750 2023-05-03 05:50:15.786577 django-plotly-dash-2.2.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     5896 2023-05-03 04:25:45.000000 django-plotly-dash-2.2.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.774577 django-plotly-dash-2.2.0/django_plotly_dash/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1426 2022-10-29 04:56:24.000000 django-plotly-dash-2.2.0/django_plotly_dash/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4034 2022-07-02 21:00:46.000000 django-plotly-dash-2.2.0/django_plotly_dash/_callback.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5166 2022-11-10 23:41:50.000000 django-plotly-dash-2.2.0/django_plotly_dash/_patches.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2176 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/access.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1398 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/admin.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1190 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/app_name.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1360 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/apps.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6076 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/consumers.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    30898 2022-11-11 04:55:36.000000 django-plotly-dash-2.2.0/django_plotly_dash/dash_wrapper.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7772 2022-10-29 03:43:04.000000 django-plotly-dash-2.2.0/django_plotly_dash/finders.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5213 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/middleware.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.778576 django-plotly-dash-2.2.0/django_plotly_dash/migrations/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1549 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/migrations/0001_initial.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3105 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/migrations/0002_add_examples.py
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/migrations/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9950 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/models.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2266 2023-05-03 04:59:10.000000 django-plotly-dash-2.2.0/django_plotly_dash/routing.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.774577 django-plotly-dash-2.2.0/django_plotly_dash/templates/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.774577 django-plotly-dash-2.2.0/django_plotly_dash/templates/admin/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.774577 django-plotly-dash-2.2.0/django_plotly_dash/templates/admin/django_plotly_dash/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.778576 django-plotly-dash-2.2.0/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/
--rw-rw-r--   0 mark      (1000) mark      (1000)      564 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/change_list.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.786577 django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/
--rw-rw-r--   0 mark      (1000) mark      (1000)      147 2022-10-29 04:56:24.000000 django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/plotly_app.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      170 2022-10-29 04:56:24.000000 django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/plotly_app_bootstrap.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      112 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/plotly_direct.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      909 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/plotly_messaging.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.786577 django-plotly-dash-2.2.0/django_plotly_dash/templatetags/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-05-08 05:22:26.000000 django-plotly-dash-2.2.0/django_plotly_dash/templatetags/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6140 2022-10-29 04:56:24.000000 django-plotly-dash-2.2.0/django_plotly_dash/templatetags/plotly_dash.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    30927 2022-07-02 21:00:46.000000 django-plotly-dash-2.2.0/django_plotly_dash/tests.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7646 2022-07-02 21:00:46.000000 django-plotly-dash-2.2.0/django_plotly_dash/tests_dash_contract.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4170 2022-07-02 21:00:46.000000 django-plotly-dash-2.2.0/django_plotly_dash/urls.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4743 2022-10-29 04:56:24.000000 django-plotly-dash-2.2.0/django_plotly_dash/util.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1243 2023-05-03 04:20:35.000000 django-plotly-dash-2.2.0/django_plotly_dash/version.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7194 2022-07-02 21:00:46.000000 django-plotly-dash-2.2.0/django_plotly_dash/views.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 05:50:15.778576 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     6750 2023-05-03 05:50:15.000000 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     1416 2023-05-03 05:50:15.000000 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-03 05:50:15.000000 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      113 2023-05-03 05:50:15.000000 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       19 2023-05-03 05:50:15.000000 django-plotly-dash-2.2.0/django_plotly_dash.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-03 05:50:15.786577 django-plotly-dash-2.2.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)     1627 2023-05-03 04:21:56.000000 django-plotly-dash-2.2.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.376659 django-plotly-dash-2.2.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1107 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)       53 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/MANIFEST.in
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6750 2023-05-28 17:40:22.376659 django-plotly-dash-2.2.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5896 2023-05-28 17:32:00.000000 django-plotly-dash-2.2.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.372660 django-plotly-dash-2.2.1/django_plotly_dash/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1426 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4034 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/_callback.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5166 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/_patches.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2176 2019-11-16 00:41:24.000000 django-plotly-dash-2.2.1/django_plotly_dash/access.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1398 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/admin.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1190 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/app_name.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1414 2023-05-28 17:32:00.000000 django-plotly-dash-2.2.1/django_plotly_dash/apps.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6076 2021-02-06 14:37:20.000000 django-plotly-dash-2.2.1/django_plotly_dash/consumers.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    30898 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/dash_wrapper.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7772 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/finders.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5213 2019-12-20 18:43:29.000000 django-plotly-dash-2.2.1/django_plotly_dash/middleware.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.372660 django-plotly-dash-2.2.1/django_plotly_dash/migrations/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1549 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/migrations/0001_initial.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3105 2021-02-06 14:37:20.000000 django-plotly-dash-2.2.1/django_plotly_dash/migrations/0002_add_examples.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/migrations/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     9950 2021-02-06 14:37:20.000000 django-plotly-dash-2.2.1/django_plotly_dash/models.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2266 2023-05-28 17:32:00.000000 django-plotly-dash-2.2.1/django_plotly_dash/routing.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.364660 django-plotly-dash-2.2.1/django_plotly_dash/templates/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.364660 django-plotly-dash-2.2.1/django_plotly_dash/templates/admin/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.364660 django-plotly-dash-2.2.1/django_plotly_dash/templates/admin/django_plotly_dash/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.372660 django-plotly-dash-2.2.1/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      564 2019-12-04 14:04:55.000000 django-plotly-dash-2.2.1/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/change_list.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.376659 django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      147 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/plotly_app.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      170 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/plotly_app_bootstrap.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      112 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/plotly_direct.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      909 2019-12-20 18:43:29.000000 django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/plotly_messaging.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.376659 django-plotly-dash-2.2.1/django_plotly_dash/templatetags/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2018-12-17 07:04:19.000000 django-plotly-dash-2.2.1/django_plotly_dash/templatetags/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6140 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/templatetags/plotly_dash.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    30927 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/tests.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7646 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/tests_dash_contract.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4170 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/urls.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4743 2023-04-26 12:19:15.000000 django-plotly-dash-2.2.1/django_plotly_dash/util.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1243 2023-05-28 17:33:27.000000 django-plotly-dash-2.2.1/django_plotly_dash/version.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7194 2022-06-06 02:03:57.000000 django-plotly-dash-2.2.1/django_plotly_dash/views.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-28 17:40:22.372660 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6750 2023-05-28 17:40:22.000000 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1416 2023-05-28 17:40:22.000000 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-28 17:40:22.000000 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      119 2023-05-28 17:40:22.000000 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       19 2023-05-28 17:40:22.000000 django-plotly-dash-2.2.1/django_plotly_dash.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-28 17:40:22.376659 django-plotly-dash-2.2.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1633 2023-05-28 17:33:11.000000 django-plotly-dash-2.2.1/setup.py
```

### Comparing `django-plotly-dash-2.2.0/LICENSE` & `django-plotly-dash-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/PKG-INFO` & `django-plotly-dash-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plotly-dash
-Version: 2.2.0
+Version: 2.2.1
 Summary: Django use of plotly dash apps through template tags
 Home-page: https://github.com/GibbsConsulting/django-plotly-dash
 Author: Mark Gibbs
 Author-email: django_plotly_dash@gibbsconsulting.ca
 License: MIT
 Project-URL: Source, https://github.com/GibbsConsulting/django-plotly-dash
 Project-URL: Tracker, https://github.com/GibbsConsulting/django-plotly-dash/issues
```

### Comparing `django-plotly-dash-2.2.0/README.md` & `django-plotly-dash-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/__init__.py` & `django-plotly-dash-2.2.1/django_plotly_dash/__init__.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/_callback.py` & `django-plotly-dash-2.2.1/django_plotly_dash/_callback.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/_patches.py` & `django-plotly-dash-2.2.1/django_plotly_dash/_patches.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/access.py` & `django-plotly-dash-2.2.1/django_plotly_dash/access.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/admin.py` & `django-plotly-dash-2.2.1/django_plotly_dash/admin.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/app_name.py` & `django-plotly-dash-2.2.1/django_plotly_dash/app_name.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/apps.py` & `django-plotly-dash-2.2.1/django_plotly_dash/apps.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 from django.apps import AppConfig
 
 
 class DjangoPlotlyDashConfig(AppConfig):
     'Verbose name and other settings for the django-plotly-dash application'
     name = 'django_plotly_dash'
     verbose_name = "Django Plotly Dash"
+    default_auto_field = 'django.db.models.AutoField'
```

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/consumers.py` & `django-plotly-dash-2.2.1/django_plotly_dash/consumers.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/dash_wrapper.py` & `django-plotly-dash-2.2.1/django_plotly_dash/dash_wrapper.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/finders.py` & `django-plotly-dash-2.2.1/django_plotly_dash/finders.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/middleware.py` & `django-plotly-dash-2.2.1/django_plotly_dash/middleware.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/migrations/0001_initial.py` & `django-plotly-dash-2.2.1/django_plotly_dash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/migrations/0002_add_examples.py` & `django-plotly-dash-2.2.1/django_plotly_dash/migrations/0002_add_examples.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/models.py` & `django-plotly-dash-2.2.1/django_plotly_dash/models.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/routing.py` & `django-plotly-dash-2.2.1/django_plotly_dash/routing.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/change_list.html` & `django-plotly-dash-2.2.1/django_plotly_dash/templates/admin/django_plotly_dash/statelessapp/change_list.html`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/templates/django_plotly_dash/plotly_messaging.html` & `django-plotly-dash-2.2.1/django_plotly_dash/templates/django_plotly_dash/plotly_messaging.html`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/templatetags/plotly_dash.py` & `django-plotly-dash-2.2.1/django_plotly_dash/templatetags/plotly_dash.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/tests.py` & `django-plotly-dash-2.2.1/django_plotly_dash/tests.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/tests_dash_contract.py` & `django-plotly-dash-2.2.1/django_plotly_dash/tests_dash_contract.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/urls.py` & `django-plotly-dash-2.2.1/django_plotly_dash/urls.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/util.py` & `django-plotly-dash-2.2.1/django_plotly_dash/util.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/version.py` & `django-plotly-dash-2.2.1/django_plotly_dash/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
```

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash/views.py` & `django-plotly-dash-2.2.1/django_plotly_dash/views.py`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash.egg-info/PKG-INFO` & `django-plotly-dash-2.2.1/django_plotly_dash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plotly-dash
-Version: 2.2.0
+Version: 2.2.1
 Summary: Django use of plotly dash apps through template tags
 Home-page: https://github.com/GibbsConsulting/django-plotly-dash
 Author: Mark Gibbs
 Author-email: django_plotly_dash@gibbsconsulting.ca
 License: MIT
 Project-URL: Source, https://github.com/GibbsConsulting/django-plotly-dash
 Project-URL: Tracker, https://github.com/GibbsConsulting/django-plotly-dash/issues
```

### Comparing `django-plotly-dash-2.2.0/django_plotly_dash.egg-info/SOURCES.txt` & `django-plotly-dash-2.2.1/django_plotly_dash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plotly-dash-2.2.0/setup.py` & `django-plotly-dash-2.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     keywords='django plotly plotly-dash dash dashboard',
     project_urls = {
     'Source': "https://github.com/GibbsConsulting/django-plotly-dash",
     'Tracker': "https://github.com/GibbsConsulting/django-plotly-dash/issues",
     'Documentation': 'http://django-plotly-dash.readthedocs.io/',
     },
     install_requires = ['plotly',
-                        'dash>=2.0',
+                        'dash>=2.0,<2.10',
                         'dpd-components',
 
                         'dash-bootstrap-components',
 
                         'channels>=2.0',
                         'Django>=3.2,<5.0.0',
                         'Flask>=1.0.2',
```

