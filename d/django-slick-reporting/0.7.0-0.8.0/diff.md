# Comparing `tmp/django-slick-reporting-0.7.0.tar.gz` & `tmp/django-slick-reporting-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-slick-reporting-0.7.0.tar", last modified: Mon May 15 07:50:41 2023, max compression
+gzip compressed data, was "django-slick-reporting-0.8.0.tar", last modified: Sun May 28 11:13:17 2023, max compression
```

## Comparing `django-slick-reporting-0.7.0.tar` & `django-slick-reporting-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.7.0/LICENSE.md
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.7.0/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9104 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7417 2022-08-26 21:11:35.000000 django-slick-reporting-0.7.0/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9104 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1178 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/dependency_links.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/requires.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-05-15 07:50:41.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.7.0/django_slick_reporting.egg-info/top_level.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-slick-reporting-0.7.0/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-05-15 07:50:39.000000 django-slick-reporting-0.7.0/slick_reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1688 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      207 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/decorators.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16339 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/fields.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8188 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/form_factory.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    38050 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/generator.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/main.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.chartsjs.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.highchart.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1937 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/base.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9363 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/simple_report.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/table.html
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-15 07:50:41.485818 django-slick-reporting-0.7.0/slick_reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.7.0/slick_reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2022-07-07 07:19:02.000000 django-slick-reporting-0.7.0/slick_reporting/templatetags/slick_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    14333 2023-05-15 07:49:20.000000 django-slick-reporting-0.7.0/slick_reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.8.0/LICENSE.md
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.8.0/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9291 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7604 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.148920 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9291 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1200 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/dependency_links.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/requires.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/top_level.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-slick-reporting-0.8.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1688 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      207 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/decorators.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    16896 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/fields.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8247 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/form_factory.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    38156 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/generator.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.144920 django-slick-reporting-0.8.0/slick_reporting/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/main.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.144920 django-slick-reporting-0.8.0/slick_reporting/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1937 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/base.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9397 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/simple_report.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/table.html
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.8.0/slick_reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2022-07-07 07:19:02.000000 django-slick-reporting-0.8.0/slick_reporting/templatetags/slick_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    14341 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/views.py
```

### Comparing `django-slick-reporting-0.7.0/LICENSE.md` & `django-slick-reporting-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/PKG-INFO` & `django-slick-reporting-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.7.0
+Version: 0.8.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -55,22 +55,23 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
+This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
 
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
 - Create your Custom Calculation easily, which will be integrated with the above reports types
 - Optimized for speed.
-- Batteries included! Chart.js , DataTable.net & a Bootstrap form.
+- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.7.0/README.rst` & `django-slick-reporting-0.8.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
+This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
 
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
 - Create your Custom Calculation easily, which will be integrated with the above reports types
 - Optimized for speed.
-- Batteries included! Chart.js , DataTable.net & a Bootstrap form.
+- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.7.0/django_slick_reporting.egg-info/PKG-INFO` & `django-slick-reporting-0.8.0/django_slick_reporting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.7.0
+Version: 0.8.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -55,22 +55,23 @@
 
 
 Django Slick Reporting
 ======================
 
 A one stop reports engine with batteries included.
 
+This is project is an extract of the reporting engine of `Django ERP Framework <https://github.com/RamezIssac/django-erp-framework>`_
 
 Features
 --------
 
 - Effortlessly create Simple, Grouped, Time series and Crosstab reports in a handful of code lines.
 - Create your Custom Calculation easily, which will be integrated with the above reports types
 - Optimized for speed.
-- Batteries included! Chart.js , DataTable.net & a Bootstrap form.
+- Batteries included! Highcharts & Chart.js charting capabilities , DataTable.net & easily customizable Bootstrap form.
 
 Installation
 ------------
 
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install django-slick-reporting.
 
 .. code-block:: console
```

### Comparing `django-slick-reporting-0.7.0/django_slick_reporting.egg-info/SOURCES.txt` & `django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 slick_reporting/decorators.py
 slick_reporting/fields.py
 slick_reporting/form_factory.py
 slick_reporting/generator.py
 slick_reporting/helpers.py
 slick_reporting/registry.py
 slick_reporting/views.py
+slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
+slick_reporting/static/slick_reporting/erp_framework.highchart.js
 slick_reporting/static/slick_reporting/main.js
-slick_reporting/static/slick_reporting/ra.chartsjs.js
-slick_reporting/static/slick_reporting/ra.highchart.js
 slick_reporting/templates/slick_reporting/base.html
 slick_reporting/templates/slick_reporting/simple_report.html
 slick_reporting/templates/slick_reporting/table.html
 slick_reporting/templatetags/__init__.py
 slick_reporting/templatetags/slick_reporting_tags.py
```

### Comparing `django-slick-reporting-0.7.0/setup.cfg` & `django-slick-reporting-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/app_settings.py` & `django-slick-reporting-0.8.0/slick_reporting/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/decorators.py` & `django-slick-reporting-0.8.0/slick_reporting/decorators.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/fields.py` & `django-slick-reporting-0.8.0/slick_reporting/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -341,15 +341,15 @@
         """
         Construct a verbose name for the crosstab field
         :param model: the model name
         :param id: the id of the current crosstab object
         :return: a verbose string
         """
         if id == "----":
-            return _("The reminder")
+            return _("The remainder")
         return f"{cls.verbose_name} {model} {id}"
 
     @classmethod
     def get_time_series_field_verbose_name(cls, date_period, index, dates, pattern):
         """
         Get the name of the verbose name of a computaion field that's in a time_series.
         should be a mix of the date period if the column an it's verbose name.
@@ -372,15 +372,15 @@
             return f"{cls.verbose_name} {year}"
 
         return f"{cls.verbose_name} {date_period[0].strftime(dt_format)} - {date_period[1].strftime(dt_format)}"
 
 
 class FirstBalanceField(SlickReportField):
     name = "__fb__"
-    verbose_name = _("first balance")
+    verbose_name = _("opening balance")
 
     def prepare(self, q_filters=None, extra_filters=None, **kwargs):
         extra_filters = extra_filters or {}
 
         from_date_value = extra_filters.get(f"{self.date_field}__gte")
         extra_filters.pop(f"{self.date_field}__gte", None)
         extra_filters[f"{self.date_field}__lt"] = from_date_value
@@ -397,15 +397,15 @@
 
 
 field_registry.register(TotalReportField)
 
 
 class BalanceReportField(SlickReportField):
     name = "__balance__"
-    verbose_name = _("Cumulative Total")
+    verbose_name = _("Closing Total")
     requires = ["__fb__"]
 
     def final_calculation(self, debit, credit, dep_dict):
         fb = dep_dict.get("__fb__")
         debit = debit or 0
         credit = credit or 0
         fb = fb or 0
@@ -435,53 +435,73 @@
     def final_calculation(self, debit, credit, dep_dict):
         return credit
 
 
 field_registry.register(CreditReportField)
 
 
+@field_registry.register
 class DebitReportField(SlickReportField):
     name = "__debit__"
     verbose_name = _("Debit")
 
     def final_calculation(self, debit, credit, dep_dict):
         return debit
 
 
-field_registry.register(DebitReportField)
+@field_registry.register
+class CreditQuantityReportField(SlickReportField):
+    name = "__credit_quantity__"
+    verbose_name = _("Credit QTY")
+    calculation_field = "quantity"
+    is_summable = False
+
+    def final_calculation(self, debit, credit, dep_dict):
+        return credit
+
+
+@field_registry.register
+class DebitQuantityReportField(SlickReportField):
+    name = "__debit_quantity__"
+    calculation_field = "quantity"
+    verbose_name = _("Debit QTY")
+    is_summable = False
+
+    def final_calculation(self, debit, credit, dep_dict):
+        return debit
 
 
 class TotalQTYReportField(SlickReportField):
     name = "__total_quantity__"
     verbose_name = _("Total QTY")
     calculation_field = "quantity"
     is_summable = False
 
 
 field_registry.register(TotalQTYReportField)
 
 
 class FirstBalanceQTYReportField(FirstBalanceField):
-    name = "__fb_quan__"
-    verbose_name = _("starting QTY")
+    name = "__fb_quantity__"
+    verbose_name = _("Opening QTY")
     calculation_field = "quantity"
     is_summable = False
 
 
 field_registry.register(FirstBalanceQTYReportField)
 
 
 class BalanceQTYReportField(SlickReportField):
     name = "__balance_quantity__"
-    verbose_name = _("Cumulative QTY")
+    verbose_name = _("Closing QTY")
     calculation_field = "quantity"
-    requires = ["__fb_quan__"]
+    requires = ["__fb_quantity__"]
     is_summable = False
 
     def final_calculation(self, debit, credit, dep_dict):
         # Use `get` so it fails loud if its not there
-        fb = dep_dict.get("__fb_quan__")
+        fb = dep_dict.get("__fb_quantity__")
         fb = fb or 0
         return fb + debit - credit
 
 
 field_registry.register(BalanceQTYReportField)
```

### Comparing `django-slick-reporting-0.7.0/slick_reporting/form_factory.py` & `django-slick-reporting-0.8.0/slick_reporting/form_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return f.formfield(**kwargs)
 
 
 def get_crispy_helper(
     foreign_keys_map=None,
     crosstab_model=None,
     crosstab_key_name=None,
-    crosstab_display_compute_reminder=False,
+    crosstab_display_compute_remainder=False,
     add_date_range=True,
 ):
     from crispy_forms.helper import FormHelper
     from crispy_forms.layout import Column, Layout, Div, Row, Field
 
     helper = FormHelper()
     helper.form_class = "form-horizontal"
@@ -48,16 +48,16 @@
                 css_class="raReportDateRange",
             ),
         )
     filters_container = Div(css_class="mt-20", style="margin-top:20px")
     # first add the crosstab model and its display reimder then the rest of the fields
     if crosstab_model:
         filters_container.append(Field(crosstab_key_name))
-        if crosstab_display_compute_reminder:
-            filters_container.append(Field("crosstab_compute_reminder"))
+        if crosstab_display_compute_remainder:
+            filters_container.append(Field("crosstab_compute_remainder"))
 
     for k in foreign_keys_map:
         if k != crosstab_key_name:
             filters_container.append(Field(k))
     helper.layout.fields.append(filters_container)
 
     return helper
@@ -93,14 +93,15 @@
                     if val:
                         val = [x for x in val.values_list("pk", flat=True)]
                         _values["%s__in" % key] = val
             return None, _values
 
     @cached_property
     def crosstab_key_name(self):
+        # todo get the model more accurately
         """
         return the actual foreignkey field name by simply adding an '_id' at the end.
         This is hook is to customize this naieve approach.
         :return: key: a string that should be in self.cleaned_data
         """
         return f"{self.crosstab_model}_id"
 
@@ -110,24 +111,24 @@
         :return:
         """
         if self.crosstab_model:
             qs = self.cleaned_data.get(self.crosstab_key_name)
             return [x for x in qs.values_list("pk", flat=True)]
         return []
 
-    def get_crosstab_compute_reminder(self):
-        return self.cleaned_data.get("crosstab_compute_reminder", True)
+    def get_crosstab_compute_remainder(self):
+        return self.cleaned_data.get("crosstab_compute_remainder", True)
 
     def get_crispy_helper(self, foreign_keys_map=None, crosstab_model=None, **kwargs):
         return get_crispy_helper(
             self.foreign_keys,
             crosstab_model=getattr(self, "crosstab_model", None),
             crosstab_key_name=getattr(self, "crosstab_key_name", None),
-            crosstab_display_compute_reminder=getattr(
-                self, "crosstab_display_compute_reminder", False
+            crosstab_display_compute_remainder=getattr(
+                self, "crosstab_display_compute_remainder", False
             ),
             **kwargs,
         )
 
 
 def _default_foreign_key_widget(f_field):
     return {
@@ -135,15 +136,15 @@
         "required": False,
     }
 
 
 def report_form_factory(
     model,
     crosstab_model=None,
-    display_compute_reminder=True,
+    display_compute_remainder=True,
     fkeys_filter_func=None,
     foreign_key_widget_func=None,
     excluded_fields=None,
     initial=None,
     required=None,
     show_time_series_selector=False,
     time_series_selector_choices=None,
@@ -154,15 +155,15 @@
     """
     Create a Report Form based on the report_model passed by
     1. adding a start_date and end_date fields
     2. extract all ForeignKeys on the report_model
 
     :param model: the report_model
     :param crosstab_model: crosstab model if any
-    :param display_compute_reminder:  relevant only if crosstab_model is specified. Control if we show the check to
+    :param display_compute_remainder:  relevant only if crosstab_model is specified. Control if we show the check to
     display the rest.
     :param fkeys_filter_func:  a receives an OrderedDict of Foreign Keys names and their model field instances found on the model, return the OrderedDict that would be used
     :param foreign_key_widget_func: receives a Field class return the used widget like this {'form_class': forms.ModelMultipleChoiceField, 'required': False, }
     :param excluded_fields: a list of fields to be excluded from the report form
     :param initial a dict for fields initial
     :param required a list of fields that should be marked as required
     :return:
@@ -214,28 +215,28 @@
     for name, f_field in fkeys_map.items():
         fkeys_list.append(name)
         field_attrs = foreign_key_widget_func(f_field)
         if name in required:
             field_attrs["required"] = True
         fields[name] = f_field.formfield(**field_attrs)
 
-    if crosstab_model and display_compute_reminder:
-        fields["crosstab_compute_reminder"] = forms.BooleanField(
-            required=False, label=_("Display the crosstab reminder"), initial=True
+    if crosstab_model and display_compute_remainder:
+        fields["crosstab_compute_remainder"] = forms.BooleanField(
+            required=False, label=_("Display the crosstab remainder"), initial=True
         )
 
     bases = (
         BaseReportForm,
         forms.BaseForm,
     )
     new_form = type(
         "ReportForm",
         bases,
         {
             "base_fields": fields,
             "_fkeys": fkeys_list,
             "foreign_keys": fkeys_map,
             "crosstab_model": crosstab_model,
-            "crosstab_display_compute_reminder": display_compute_reminder,
+            "crosstab_display_compute_remainder": display_compute_remainder,
         },
     )
     return new_form
```

### Comparing `django-slick-reporting-0.7.0/slick_reporting/generator.py` & `django-slick-reporting-0.8.0/slick_reporting/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     """
     crosstab_columns = None
     """The computation fields which will be computed for each crosstab-ed ids """
 
     crosstab_ids = None
     """A list is the ids to create a crosstab report on"""
 
-    crosstab_compute_reminder = True
+    crosstab_compute_remainder = True
     """Include an an extra crosstab_columns for the outer group ( ie: all expects those `crosstab_ids`) """
 
     show_empty_records = True
     """
     If group_by is set, this option control if the report result will include all objects regardless of appearing in the report_model/qs.
     If set False, only those objects which are found in the report_model/qs
     Example: Say you group by client
@@ -157,15 +157,15 @@
         columns=None,
         time_series_pattern=None,
         time_series_columns=None,
         time_series_custom_dates=None,
         crosstab_model=None,
         crosstab_columns=None,
         crosstab_ids=None,
-        crosstab_compute_reminder=None,
+        crosstab_compute_remainder=None,
         swap_sign=False,
         show_empty_records=None,
         print_flag=False,
         doc_type_plus_list=None,
         doc_type_minus_list=None,
         limit_records=False,
         format_row_func=None,
@@ -183,15 +183,15 @@
         :param group_by:
         :param columns:
         :param time_series_pattern:
         :param time_series_columns:
         :param crosstab_model:
         :param crosstab_columns:
         :param crosstab_ids:
-        :param crosstab_compute_reminder:
+        :param crosstab_compute_remainder:
         :param swap_sign:
         :param show_empty_records:
         :param base_model:
         :param print_flag:
         :param doc_type_plus_list:
         :param doc_type_minus_list:
         :param limit_records:
@@ -222,18 +222,18 @@
 
         self.q_filters = q_filters or []
         self.kwargs_filters = kwargs_filters or {}
 
         self.crosstab_model = self.crosstab_model or crosstab_model
         self.crosstab_columns = crosstab_columns or self.crosstab_columns or []
         self.crosstab_ids = self.crosstab_ids or crosstab_ids or []
-        self.crosstab_compute_reminder = (
-            self.crosstab_compute_reminder
-            if crosstab_compute_reminder is None
-            else crosstab_compute_reminder
+        self.crosstab_compute_remainder = (
+            self.crosstab_compute_remainder
+            if crosstab_compute_remainder is None
+            else crosstab_compute_remainder
         )
 
         self.format_row = format_row_func or self._default_format_row
 
         main_queryset = main_queryset or self.report_model.objects
         main_queryset = main_queryset.order_by()
 
@@ -298,15 +298,15 @@
         self.swap_sign = self.swap_sign or swap_sign
         self.limit_records = self.limit_records or limit_records
 
         # passed to the report fields
         # self.date_field = date_field or self.date_field
 
         # in case of a group by, do we show a grouped by model data regardless of their appearance in the results
-        # a client who didnt make a transaction during the date period.
+        # a client who didn't make a transaction during the date period.
         self.show_empty_records = False  # show_empty_records if show_empty_records else self.show_empty_records
         # Looks like this options is harder then what i thought as it interfere with the usual filtering of the report
 
         # Preparing actions
         self._parse()
         if self.group_by:
             if self.show_empty_records:
@@ -370,19 +370,19 @@
             query = query.filter(**filters)
         if fields:
             return query.values(*fields)
         return query.values()
 
     def _construct_crosstab_filter(self, col_data):
         """
-        In charge of adding the needed crosstab filter, specific to the case of is_reminder or not
+        In charge of adding the needed crosstab filter, specific to the case of is_remainder or not
         :param col_data:
         :return:
         """
-        if col_data["is_reminder"]:
+        if col_data["is_remainder"]:
             filters = [~Q(**{f"{col_data['model']}_id__in": self.crosstab_ids})]
         else:
             filters = [Q(**{f"{col_data['model']}_id": col_data["id"]})]
         return filters
 
     def _prepare_report_dependencies(self):
         from .fields import SlickReportField
@@ -801,15 +801,15 @@
     def get_crosstab_parsed_columns(self):
         """
         Return a list of the columns analyzed , with reference to computation field and everything
         :return:
         """
         report_columns = self.crosstab_columns or []
         ids = list(self.crosstab_ids)
-        if self.crosstab_compute_reminder:
+        if self.crosstab_compute_remainder:
             ids.append("----")
         output_cols = []
         ids_length = len(ids) - 1
         for counter, id in enumerate(ids):
             for col in report_columns:
                 magic_field_class = None
                 if type(col) is str:
@@ -823,15 +823,17 @@
                         "original_name": magic_field_class.name,
                         "verbose_name": self.get_crosstab_field_verbose_name(
                             magic_field_class, self.crosstab_model, id
                         ),
                         "ref": magic_field_class,
                         "id": id,
                         "model": self.crosstab_model,
-                        "is_reminder": counter == ids_length,
+                        "is_remainder": counter == ids_length
+                        if self.crosstab_compute_remainder
+                        else False,
                         "source": "magic_field" if magic_field_class else "",
                         "is_summable": magic_field_class.is_summable,
                     }
                 )
 
         return output_cols
```

### Comparing `django-slick-reporting-0.7.0/slick_reporting/helpers.py` & `django-slick-reporting-0.8.0/slick_reporting/helpers.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/registry.py` & `django-slick-reporting-0.8.0/slick_reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/main.js` & `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/main.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.chartsjs.js` & `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/static/slick_reporting/ra.highchart.js` & `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/base.html` & `django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     <!-- Bootstrap CSS -->
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
           integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
 
     <link rel="stylesheet" type="text/css"
           href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"/>
-    <title>Python Slick Reporting</title>
+    <title>Django Slick Reporting</title>
 </head>
 <body>
 <div class="container">
     <div class="py-5 ">
         {% block content %}
 
         {% endblock %}
```

### Comparing `django-slick-reporting-0.7.0/slick_reporting/templates/slick_reporting/simple_report.html` & `django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/simple_report.html`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 
     </div>
 
 {% endblock %}
 {% block extrajs %}
     {{ block.super }}
     <script src="{% static 'slick_reporting/main.js' %}"></script>
-    <script src="{% static 'slick_reporting/ra.chartsjs.js' %}"></script>
-    <script src="{% static 'slick_reporting/ra.highchart.js' %}"></script>
+    <script src="{% static 'slick_reporting/erp_framework.chartsjs.js' %}"></script>
+    <script src="{% static 'slick_reporting/erp_framework.highchart.js' %}"></script>
 
     <link href="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/css/select2.min.css" rel="stylesheet"/>
-<script src="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/js/select2.min.js"
-        integrity="sha384-JnbsSLBmv2/R0fUmF2XYIcAEMPHEAO51Gitn9IjL4l89uFTIgtLF1+jqIqqd9FSk"
-        crossorigin="anonymous"></script>
+    <script src="https://cdn.jsdelivr.net/npm/select2@4.0.13/dist/js/select2.min.js"
+            integrity="sha384-JnbsSLBmv2/R0fUmF2XYIcAEMPHEAO51Gitn9IjL4l89uFTIgtLF1+jqIqqd9FSk"
+            crossorigin="anonymous"></script>
 
 
     <script>
         $(document).ready(function () {
 
 
             $('select').select2();
```

### Comparing `django-slick-reporting-0.7.0/slick_reporting/templatetags/slick_reporting_tags.py` & `django-slick-reporting-0.8.0/slick_reporting/templatetags/slick_reporting_tags.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.7.0/slick_reporting/views.py` & `django-slick-reporting-0.8.0/slick_reporting/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     queryset = None
 
     chart_settings = None
 
     crosstab_model = None
     crosstab_ids = None
     crosstab_columns = None
-    crosstab_compute_reminder = True
+    crosstab_compute_remainder = True
     excluded_fields = None
     report_title_context_key = "title"
 
     time_series_selector = False
     time_series_selector_choices = None
     time_series_selector_default = None
     time_series_selector_allow_empty = False
@@ -180,15 +180,15 @@
         """
         Automatically instantiate a form based on details provided
         :return:
         """
         return self.form_class or report_form_factory(
             self.get_report_model(),
             crosstab_model=self.crosstab_model,
-            display_compute_reminder=self.crosstab_compute_reminder,
+            display_compute_remainder=self.crosstab_compute_remainder,
             excluded_fields=self.excluded_fields,
             initial=self.get_form_initial(),
             show_time_series_selector=self.time_series_selector,
             time_series_selector_choices=self.time_series_selector_choices,
             time_series_selector_default=self.time_series_selector_default,
             time_series_selector_allow_empty=self.time_series_selector_allow_empty,
         )
@@ -219,18 +219,18 @@
         return kwargs
 
     def get_report_generator(self, queryset, for_print):
         q_filters, kw_filters = self.form.get_filters()
         if self.crosstab_model:
             self.crosstab_ids = self.form.get_crosstab_ids()
 
-        crosstab_compute_reminder = (
-            self.form.get_crosstab_compute_reminder()
+        crosstab_compute_remainder = (
+            self.form.get_crosstab_compute_remainder()
             if self.request.GET or self.request.POST
-            else self.crosstab_compute_reminder
+            else self.crosstab_compute_remainder
         )
 
         time_series_pattern = self.time_series_pattern
         if self.time_series_selector:
             time_series_pattern = self.form.cleaned_data["time_series_pattern"]
 
         return self.report_generator_class(
@@ -247,15 +247,15 @@
             columns=self.columns,
             group_by=self.group_by,
             time_series_pattern=time_series_pattern,
             time_series_columns=self.time_series_columns,
             crosstab_model=self.crosstab_model,
             crosstab_ids=self.crosstab_ids,
             crosstab_columns=self.crosstab_columns,
-            crosstab_compute_reminder=crosstab_compute_reminder,
+            crosstab_compute_remainder=crosstab_compute_remainder,
             format_row_func=self.format_row,
             container_class=self,
         )
 
     def format_row(self, row_obj):
         """
         A hook to format each row . This method gets called on each row in the results. <ust return the object
```

