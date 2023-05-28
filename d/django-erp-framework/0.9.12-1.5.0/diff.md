# Comparing `tmp/django-erp-framework-0.9.12.tar.gz` & `tmp/django-erp-framework-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-erp-framework-0.9.12.tar", last modified: Mon May  8 15:25:48 2023, max compression
+gzip compressed data, was "django-erp-framework-1.5.0.tar", last modified: Sun May 28 14:45:13 2023, max compression
```

## Comparing `django-erp-framework-0.9.12.tar` & `django-erp-framework-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/
--rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.12/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.12/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.12/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/django_erp_framework.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4996 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1724 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      204 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-08 15:25:48.000000 django-erp-framework-0.9.12/django_erp_framework.egg-info/top_level.txt
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/erp_framework/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       99 2023-05-08 15:25:37.000000 django-erp-framework-0.9.12/erp_framework/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.962422 django-erp-framework-0.9.12/erp_framework/activity/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/activity/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/0003_alter_myactivity_options.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/activity/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/admin/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    51303 2023-05-08 14:12:13.000000 django-erp-framework-0.9.12/erp_framework/admin/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7542 2023-05-08 14:10:04.000000 django-erp-framework-0.9.12/erp_framework/admin/base.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/admin/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/base/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2933 2023-05-08 14:23:36.000000 django-erp-framework-0.9.12/erp_framework/base/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/base/widgets.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/checks.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/contrib/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/contrib/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/contrib/jazzmin_integration/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/contrib/jazzmin_integration/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/printing.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      665 2023-05-08 14:33:00.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_ra_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/_suit_menu.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2683 2023-05-08 14:17:14.000000 django-erp-framework-0.9.12/erp_framework/reporting/templatetags/erp_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.12/erp_framework/reporting/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/erp_framework/utils/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/navigation.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/permissions.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.12/erp_framework/utils/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1781 2023-05-08 15:25:48.966422 django-erp-framework-0.9.12/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.12/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-1.5.0/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-1.5.0/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3335 2023-05-26 08:27:01.000000 django-erp-framework-1.5.0/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.695144 django-erp-framework-1.5.0/django_erp_framework.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1721 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      204 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/top_level.txt
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-05-28 14:24:57.000000 django-erp-framework-1.5.0/erp_framework/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/activity/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8413 2023-05-28 13:28:51.000000 django-erp-framework-1.5.0/erp_framework/activity/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/activity/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0002_auto_20200711_1253.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0003_alter_myactivity_options.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-10 22:04:15.000000 django-erp-framework-1.5.0/erp_framework/admin/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    47051 2023-05-28 14:00:46.000000 django-erp-framework-1.5.0/erp_framework/admin/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/admin/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7520 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/admin/base.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      474 2023-05-08 22:07:29.000000 django-erp-framework-1.5.0/erp_framework/admin/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      611 2023-05-08 22:03:29.000000 django-erp-framework-1.5.0/erp_framework/admin/helpers.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-14 13:33:44.000000 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      126 2023-05-14 13:33:44.000000 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      277 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/base/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/base/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2342 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/base/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7619 2023-05-28 14:00:04.000000 django-erp-framework-1.5.0/erp_framework/base/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    12628 2023-05-28 14:00:04.000000 django-erp-framework-1.5.0/erp_framework/base/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      813 2023-05-28 14:15:31.000000 django-erp-framework-1.5.0/erp_framework/checks.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/contrib/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/contrib/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3517 2023-05-14 14:42:52.000000 django-erp-framework-1.5.0/erp_framework/doc_types.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-08 18:31:35.000000 django-erp-framework-1.5.0/erp_framework/reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1051 2023-05-26 08:16:22.000000 django-erp-framework-1.5.0/erp_framework/reporting/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1698 2023-05-26 08:17:43.000000 django-erp-framework-1.5.0/erp_framework/reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/forms.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/reporting/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4526 2023-05-28 12:38:42.000000 django-erp-framework-1.5.0/erp_framework/reporting/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-25 21:59:15.000000 django-erp-framework-1.5.0/erp_framework/reporting/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1890 2023-05-26 08:17:43.000000 django-erp-framework-1.5.0/erp_framework/reporting/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/printing.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7009 2023-05-26 08:16:22.000000 django-erp-framework-1.5.0/erp_framework/reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2782 2023-05-23 14:48:31.000000 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/erp_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    13893 2023-05-28 14:37:56.000000 django-erp-framework-1.5.0/erp_framework/reporting/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      456 2023-05-28 13:28:51.000000 django-erp-framework-1.5.0/erp_framework/sites.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/erp_framework/utils/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/utils/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/utils/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1781 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-1.5.0/setup.py
```

### Comparing `django-erp-framework-0.9.12/LICENSE` & `django-erp-framework-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.12/PKG-INFO` & `django-erp-framework-1.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.12
+Version: 1.5.0
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
@@ -37,20 +37,17 @@
 
 .. image:: https://img.shields.io/pypi/v/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
 .. image:: https://img.shields.io/pypi/pyversions/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
-.. image:: https://img.shields.io/readthedocs/ra-framework
+.. image:: https://img.shields.io/readthedocs/django-erp-framework
     :target: https://django-erp-framework.readthedocs.io/
 
-.. image:: https://api.travis-ci.org/ra-systems/RA.svg?branch=master
-    :target: https://travis-ci.org/ra-systems/django-erp-framework
-
 .. image:: https://img.shields.io/codecov/c/github/ra-systems/django-erp-framework
     :target: https://codecov.io/gh/ra-systems/django-erp-framework
 
 
 
 
 
@@ -60,78 +57,73 @@
 A light-weight, effective, Django based framework to create various business applications, resource planing and management systems.
 
 Offers a ready made platform where you can start to create data entry pages and attach various reports to them.
 
 Features
 --------
 
-- Admin theme jazzmin support
-- A widget system to display various reports on a page.
-- Extendable and customizable
-- Python 3.6 / 3.7 / 3.8/ Django 2.2, 3.0 Compatible
-- Slick reporting integration for time series reports anf other
+* A Reporting Engine that can generate grouped reports and/or time series and/or crosstab from any model in your apps.
+* Charting capabilities to represent the data in the reports.
+* Widget system to create dashboards and display bits of the reports results and/or its charts on any page you want.
+* Customizable and easily extensible.
+* Django Jazzmin admin theme integration ready to use.
+* Python 3.8 / 3.9 / 3.10 , Django 3.2 +
 
 
 
 Installation
 ------------
 
 .. code-block:: console
 
     $ pip install django-erp-framework
+        OR
+    $ pip install -e git+https://github.com/RamezIssac/django-erp-framework.git#egg=django-erp-framework@develop
 
 
-Quick start
------------
-
-1. Create a virtual environment and install Django Ra ERP from Pypi
-
-    .. code-block:: console
-
-        $ virtualenv ra-erp
-        $ source ra-erp/bin/activate
-        $ pip install django-erp-framework
-
-2. Once installed, Ra provides a command to generate a new project, which would contains all the dependencies needed.
+Check out the `getting started <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_  on Read The Docs.
 
-    .. code-block:: console
 
-        $ ra-admin start my_project_name
+Demo
+----
 
-    You can always integrate Ra to your existing project, it's fairly simple. Here is the guide `Integrating into an existing django project <https://django-erp-framework.readthedocs.io/en/latest/usage/integrating_into_django.html>`_
+You can checkout a demo application `here <https://my-shop.django-erp-framework.com>`_.
 
-3. Let's run the preparation commands and get started !
-
-    .. code-block:: console
-
-        $ ./manage.py migrate
-        $ ./manage.py createsuperuser
-        $ ./manage.py runserver
+Code is available on `Github <https://github.com/RamezIssac/my-shop>`_.
 
+.. image:: https://github.com/RamezIssac/django-erp-framework/blob/develop/docs/source/_static/widgets.png?raw=true
+    :alt: Homepage
+    :align: center
 
 
 Documentation
 -------------
 
 Available on `Read The Docs <https://django-erp-framework.readthedocs.io/en/latest/>`_
 
-Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/usage/tutorial_1.html>`_
+Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_
+
+
+Reporting Engine
+----------------
+
+The reporting engine of this framework is released as a separate package `django-slick-reporting <https://pypi.org/project/django-slick-reporting/>`_.
 
 
 Testing and contribution
 ------------------------
 
 To run the test suite, first, create and activate a virtual environment. Then
 clone the repo, install the test requirements and run the tests::
 
     # 1. Clone and install requirements
     $ git clone git+git@github.com:ra-systems/django-erp-framework.git
     $ cd tests
-    $ python -m pip install -e ..
-    $ python -m pip install -r requirements/py3.txt
+    $ pip install -e ..
+    $ pip install -r requirements.txt
 
     # 2. Set the test database connection details in the environment
     $ export DATABASE_NAME=<database name>
     $ export DATABASE_USER=<database user>
     $ export DATABASE_PASSWORD=<database password if any>
 
     # 3. Run the tests
```

### Comparing `django-erp-framework-0.9.12/README.rst` & `django-erp-framework-1.5.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 .. image:: https://img.shields.io/pypi/v/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
 .. image:: https://img.shields.io/pypi/pyversions/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
-.. image:: https://img.shields.io/readthedocs/ra-framework
+.. image:: https://img.shields.io/readthedocs/django-erp-framework
     :target: https://django-erp-framework.readthedocs.io/
 
-.. image:: https://api.travis-ci.org/ra-systems/RA.svg?branch=master
-    :target: https://travis-ci.org/ra-systems/django-erp-framework
-
 .. image:: https://img.shields.io/codecov/c/github/ra-systems/django-erp-framework
     :target: https://codecov.io/gh/ra-systems/django-erp-framework
 
 
 
 
 
@@ -23,78 +20,73 @@
 A light-weight, effective, Django based framework to create various business applications, resource planing and management systems.
 
 Offers a ready made platform where you can start to create data entry pages and attach various reports to them.
 
 Features
 --------
 
-- Admin theme jazzmin support
-- A widget system to display various reports on a page.
-- Extendable and customizable
-- Python 3.6 / 3.7 / 3.8/ Django 2.2, 3.0 Compatible
-- Slick reporting integration for time series reports anf other
+* A Reporting Engine that can generate grouped reports and/or time series and/or crosstab from any model in your apps.
+* Charting capabilities to represent the data in the reports.
+* Widget system to create dashboards and display bits of the reports results and/or its charts on any page you want.
+* Customizable and easily extensible.
+* Django Jazzmin admin theme integration ready to use.
+* Python 3.8 / 3.9 / 3.10 , Django 3.2 +
 
 
 
 Installation
 ------------
 
 .. code-block:: console
 
     $ pip install django-erp-framework
+        OR
+    $ pip install -e git+https://github.com/RamezIssac/django-erp-framework.git#egg=django-erp-framework@develop
 
 
-Quick start
------------
-
-1. Create a virtual environment and install Django Ra ERP from Pypi
-
-    .. code-block:: console
-
-        $ virtualenv ra-erp
-        $ source ra-erp/bin/activate
-        $ pip install django-erp-framework
-
-2. Once installed, Ra provides a command to generate a new project, which would contains all the dependencies needed.
+Check out the `getting started <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_  on Read The Docs.
 
-    .. code-block:: console
 
-        $ ra-admin start my_project_name
+Demo
+----
 
-    You can always integrate Ra to your existing project, it's fairly simple. Here is the guide `Integrating into an existing django project <https://django-erp-framework.readthedocs.io/en/latest/usage/integrating_into_django.html>`_
+You can checkout a demo application `here <https://my-shop.django-erp-framework.com>`_.
 
-3. Let's run the preparation commands and get started !
-
-    .. code-block:: console
-
-        $ ./manage.py migrate
-        $ ./manage.py createsuperuser
-        $ ./manage.py runserver
+Code is available on `Github <https://github.com/RamezIssac/my-shop>`_.
 
+.. image:: https://github.com/RamezIssac/django-erp-framework/blob/develop/docs/source/_static/widgets.png?raw=true
+    :alt: Homepage
+    :align: center
 
 
 Documentation
 -------------
 
 Available on `Read The Docs <https://django-erp-framework.readthedocs.io/en/latest/>`_
 
-Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/usage/tutorial_1.html>`_
+Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_
+
+
+Reporting Engine
+----------------
+
+The reporting engine of this framework is released as a separate package `django-slick-reporting <https://pypi.org/project/django-slick-reporting/>`_.
 
 
 Testing and contribution
 ------------------------
 
 To run the test suite, first, create and activate a virtual environment. Then
 clone the repo, install the test requirements and run the tests::
 
     # 1. Clone and install requirements
     $ git clone git+git@github.com:ra-systems/django-erp-framework.git
     $ cd tests
-    $ python -m pip install -e ..
-    $ python -m pip install -r requirements/py3.txt
+    $ pip install -e ..
+    $ pip install -r requirements.txt
 
     # 2. Set the test database connection details in the environment
     $ export DATABASE_NAME=<database name>
     $ export DATABASE_USER=<database user>
     $ export DATABASE_PASSWORD=<database password if any>
 
     # 3. Run the tests
```

### Comparing `django-erp-framework-0.9.12/django_erp_framework.egg-info/PKG-INFO` & `django-erp-framework-1.5.0/django_erp_framework.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.12
+Version: 1.5.0
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
@@ -37,20 +37,17 @@
 
 .. image:: https://img.shields.io/pypi/v/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
 .. image:: https://img.shields.io/pypi/pyversions/django-erp-framework.svg
     :target: https://pypi.org/project/django-erp-framework
 
-.. image:: https://img.shields.io/readthedocs/ra-framework
+.. image:: https://img.shields.io/readthedocs/django-erp-framework
     :target: https://django-erp-framework.readthedocs.io/
 
-.. image:: https://api.travis-ci.org/ra-systems/RA.svg?branch=master
-    :target: https://travis-ci.org/ra-systems/django-erp-framework
-
 .. image:: https://img.shields.io/codecov/c/github/ra-systems/django-erp-framework
     :target: https://codecov.io/gh/ra-systems/django-erp-framework
 
 
 
 
 
@@ -60,78 +57,73 @@
 A light-weight, effective, Django based framework to create various business applications, resource planing and management systems.
 
 Offers a ready made platform where you can start to create data entry pages and attach various reports to them.
 
 Features
 --------
 
-- Admin theme jazzmin support
-- A widget system to display various reports on a page.
-- Extendable and customizable
-- Python 3.6 / 3.7 / 3.8/ Django 2.2, 3.0 Compatible
-- Slick reporting integration for time series reports anf other
+* A Reporting Engine that can generate grouped reports and/or time series and/or crosstab from any model in your apps.
+* Charting capabilities to represent the data in the reports.
+* Widget system to create dashboards and display bits of the reports results and/or its charts on any page you want.
+* Customizable and easily extensible.
+* Django Jazzmin admin theme integration ready to use.
+* Python 3.8 / 3.9 / 3.10 , Django 3.2 +
 
 
 
 Installation
 ------------
 
 .. code-block:: console
 
     $ pip install django-erp-framework
+        OR
+    $ pip install -e git+https://github.com/RamezIssac/django-erp-framework.git#egg=django-erp-framework@develop
 
 
-Quick start
------------
-
-1. Create a virtual environment and install Django Ra ERP from Pypi
-
-    .. code-block:: console
-
-        $ virtualenv ra-erp
-        $ source ra-erp/bin/activate
-        $ pip install django-erp-framework
-
-2. Once installed, Ra provides a command to generate a new project, which would contains all the dependencies needed.
+Check out the `getting started <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_  on Read The Docs.
 
-    .. code-block:: console
 
-        $ ra-admin start my_project_name
+Demo
+----
 
-    You can always integrate Ra to your existing project, it's fairly simple. Here is the guide `Integrating into an existing django project <https://django-erp-framework.readthedocs.io/en/latest/usage/integrating_into_django.html>`_
+You can checkout a demo application `here <https://my-shop.django-erp-framework.com>`_.
 
-3. Let's run the preparation commands and get started !
-
-    .. code-block:: console
-
-        $ ./manage.py migrate
-        $ ./manage.py createsuperuser
-        $ ./manage.py runserver
+Code is available on `Github <https://github.com/RamezIssac/my-shop>`_.
 
+.. image:: https://github.com/RamezIssac/django-erp-framework/blob/develop/docs/source/_static/widgets.png?raw=true
+    :alt: Homepage
+    :align: center
 
 
 Documentation
 -------------
 
 Available on `Read The Docs <https://django-erp-framework.readthedocs.io/en/latest/>`_
 
-Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/usage/tutorial_1.html>`_
+Please Proceed to the tutorial `Create a sales application Part 1 <https://django-erp-framework.readthedocs.io/en/latest/getting_started/index.html>`_
+
+
+Reporting Engine
+----------------
+
+The reporting engine of this framework is released as a separate package `django-slick-reporting <https://pypi.org/project/django-slick-reporting/>`_.
 
 
 Testing and contribution
 ------------------------
 
 To run the test suite, first, create and activate a virtual environment. Then
 clone the repo, install the test requirements and run the tests::
 
     # 1. Clone and install requirements
     $ git clone git+git@github.com:ra-systems/django-erp-framework.git
     $ cd tests
-    $ python -m pip install -e ..
-    $ python -m pip install -r requirements/py3.txt
+    $ pip install -e ..
+    $ pip install -r requirements.txt
 
     # 2. Set the test database connection details in the environment
     $ export DATABASE_NAME=<database name>
     $ export DATABASE_USER=<database user>
     $ export DATABASE_PASSWORD=<database password if any>
 
     # 3. Run the tests
```

### Comparing `django-erp-framework-0.9.12/django_erp_framework.egg-info/SOURCES.txt` & `django-erp-framework-1.5.0/django_erp_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,44 +7,44 @@
 django_erp_framework.egg-info/SOURCES.txt
 django_erp_framework.egg-info/dependency_links.txt
 django_erp_framework.egg-info/requires.txt
 django_erp_framework.egg-info/top_level.txt
 erp_framework/__init__.py
 erp_framework/apps.py
 erp_framework/checks.py
+erp_framework/doc_types.py
+erp_framework/sites.py
 erp_framework/activity/__init__.py
 erp_framework/activity/admin.py
 erp_framework/activity/apps.py
 erp_framework/activity/models.py
 erp_framework/activity/migrations/0001_initial.py
 erp_framework/activity/migrations/0002_auto_20200711_1253.py
 erp_framework/activity/migrations/0003_alter_myactivity_options.py
 erp_framework/activity/migrations/__init__.py
 erp_framework/admin/__init__.py
 erp_framework/admin/admin.py
 erp_framework/admin/apps.py
 erp_framework/admin/base.py
 erp_framework/admin/forms.py
 erp_framework/admin/helpers.py
+erp_framework/admin/jazzmin_integration/__init__.py
+erp_framework/admin/jazzmin_integration/apps.py
 erp_framework/base/__init__.py
 erp_framework/base/app_settings.py
 erp_framework/base/helpers.py
 erp_framework/base/models.py
-erp_framework/base/registry.py
-erp_framework/base/widgets.py
 erp_framework/contrib/__init__.py
-erp_framework/contrib/jazzmin_integration/__init__.py
 erp_framework/reporting/__init__.py
+erp_framework/reporting/admin.py
 erp_framework/reporting/apps.py
 erp_framework/reporting/forms.py
 erp_framework/reporting/models.py
 erp_framework/reporting/printing.py
 erp_framework/reporting/registry.py
 erp_framework/reporting/views.py
+erp_framework/reporting/migrations/0001_initial.py
+erp_framework/reporting/migrations/__init__.py
 erp_framework/reporting/templatetags/__init__.py
-erp_framework/reporting/templatetags/_ra_tags.py
-erp_framework/reporting/templatetags/_suit_menu.py
 erp_framework/reporting/templatetags/erp_reporting_tags.py
 erp_framework/utils/__init__.py
-erp_framework/utils/navigation.py
-erp_framework/utils/permissions.py
 erp_framework/utils/views.py
```

### Comparing `django-erp-framework-0.9.12/erp_framework/activity/admin.py` & `django-erp-framework-1.5.0/erp_framework/activity/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from django.template.defaultfilters import dictsort, capfirst, truncatewords
 from django.urls import reverse, NoReverseMatch
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from erp_framework.activity.models import MyActivity
-from erp_framework.admin.admin import erp_admin_site, RaThemeMixin
+from erp_framework.admin.admin import RaThemeMixin
+from erp_framework.sites import erp_admin_site
 from erp_framework.base import app_settings
 from erp_framework.base.helpers import RaPermissionWidgetExclude
 
 action_names = {
     ADDITION: 'Addition',
     CHANGE: 'Change',
     DELETION: 'Deletion',
@@ -163,15 +164,15 @@
 
     get_change_message.short_description = _('Comment')
 
     def object_link(self, obj):
         ct = obj.content_type
         repr_ = escape(obj.object_repr)
         try:
-            href = reverse('%s:%s_%s_change' % (app_settings.RA_ADMIN_SITE_NAME, ct.app_label, ct.model),
+            href = reverse('%s:%s_%s_change' % (app_settings.ERP_FRAMEWORK_SITE_NAME, ct.app_label, ct.model),
                            args=[obj.object_id])
             link = u'<a href="%s">%s</a>' % (href, repr_)
         except NoReverseMatch:
             link = repr_
         return mark_safe(link) if obj.action_flag != DELETION else repr_
 
     object_link.allow_tags = True
@@ -205,24 +206,24 @@
 
     get_contenttype.short_description = _('Content Type')
     get_contenttype.admin_order_field = 'content_type__model'
 
     def review(self, obj):
         if obj.action_flag == 2:
             try:
-                url = reverse('%s:%s_%s_history' % (app_settings.RA_ADMIN_SITE_NAME, obj.content_type.app_label,
+                url = reverse('%s:%s_%s_history' % (app_settings.ERP_FRAMEWORK_SITE_NAME, obj.content_type.app_label,
                                                     obj.content_type.model), args=(obj.object_id,))
             except NoReverseMatch:
                 url = ''
             link = """<a href="%s" class="legitRipple" data-popup="tooltip" title="%s">
                 <i class="fas fa-history text-indigo-800"></i>
                 <span class="legitRipple-ripple"></span></a>""" % (url, _('History'))
             return mark_safe(link)
         elif obj.action_flag == 3:
-            url = reverse('%s:%s_%s_recover' % (app_settings.RA_ADMIN_SITE_NAME, obj.content_type.app_label,
+            url = reverse('%s:%s_%s_recover' % (app_settings.ERP_FRAMEWORK_SITE_NAME, obj.content_type.app_label,
                                                 obj.content_type.model), args=(obj.object_id,))
             link = """<a href="%s" class="legitRipple" data-popup="tooltip" title="%s">
                     <i class="fas fa-undo text-indigo-800"></i>
                     <span class="legitRipple-ripple"></span></a>""" % (url, _('Recover'))
             return mark_safe(link)
 
         return ''
```

### Comparing `django-erp-framework-0.9.12/erp_framework/activity/migrations/0001_initial.py` & `django-erp-framework-1.5.0/erp_framework/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.12/erp_framework/admin/admin.py` & `django-erp-framework-1.5.0/erp_framework/admin/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,189 +1,84 @@
 from __future__ import unicode_literals
 
 import logging
-from functools import update_wrapper
 
 from crequest.middleware import CrequestMiddleware
 from django.contrib import admin
 from django.contrib.admin import helpers
 from django.contrib.admin.exceptions import DisallowedModelAdminToField
 from django.contrib.admin.options import (
     IS_POPUP_VAR,
     TO_FIELD_VAR,
     get_content_type_for_model,
 )
 from django.contrib.admin.templatetags.admin_urls import add_preserved_filters
 from django.contrib.admin.utils import quote, unquote, flatten_fieldsets
-from django.contrib.admin.widgets import AdminTextareaWidget
+from django.contrib.admin.widgets import AdminTextareaWidget, RelatedFieldWidgetWrapper
 from django.contrib.auth import get_permission_codename
-from django.contrib.auth.admin import UserAdmin, GroupAdmin
-from django.contrib.auth.models import User, Group
 from django.contrib.contenttypes.admin import GenericTabularInline
 from django.core.exceptions import PermissionDenied, ImproperlyConfigured
 from django.db import models
 from django.db.models import DecimalField, ForeignKey, TextField
 from django.db.models.base import ModelBase
 from django.dispatch import Signal
 from django.forms import all_valid
 from django.forms.widgets import TextInput, NumberInput
 from django.http import HttpResponseRedirect, Http404
 from django.template.defaultfilters import capfirst
 from django.template.response import TemplateResponse
 from django.urls import reverse, path
 from django.utils.decorators import method_decorator
-from django.utils.html import escape
-from django.utils.module_loading import import_string
 from django.utils.safestring import mark_safe
 from django.utils.timezone import now
-from django.utils.translation import gettext_lazy as _, gettext
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.csrf import csrf_protect
 from reversion.admin import VersionAdmin
-from tabular_permissions.admin import (
-    UserTabularPermissionsMixin,
-    GroupTabularPermissionsMixin,
-)
 
 from erp_framework.base.helpers import flatten_list
-from erp_framework.admin.forms import RaUserChangeForm
 from erp_framework.reporting.printing import HTMLPrintingClass
-from erp_framework.utils.views import (
-    get_typed_reports_for_templates,
-    get_typed_reports_map,
-    apply_order_to_typed_reports,
-)
-from .base import RaAdminSiteBase
+from .base import ERPFrameworkAdminSiteBase
 from ..base import app_settings
-from ..base.widgets import RaRelatedFieldWidgetWrapper
 
 csrf_protect_m = method_decorator(csrf_protect)
 
 default_fields = (("name", "slug"), "notes")
 
 default_exclude = ("owner", "creation_date", "lastmod", "lastmod_user")
 
 default_list_display = ("name", "slug", "notes")
 
 logger = logging.getLogger(__name__)
 
-from django.contrib.admin.views.main import ChangeList
-
 # todo bring back
 # changeform_saved = Signal(providing_args=["instance", "created", 'using'])
 changeform_saved = Signal()
 
 
-def get_reports_map(model_name, user, request, order_list=None):
-    """
-    Gets ReportViews associated with a specific model ie. namespace
-    :param model_name: or namespace defined in ReportView namespace
-    :param user: User to check for permissions
-    :param order_list: list to order the reports in comparision to
-
-    :return: a dictionary with two values `slugs` and `reports`
-        slugs: map to a list of report slugs
-        reports: map to a list of ReportView classes
-    """
-
-    # todo refine with erp_framework.views.ReportList View
-    order_list = list(order_list or [])
-    reports = get_typed_reports_for_templates(model_name, user, request)
-    reports = apply_order_to_typed_reports(reports, order_list)
-    return get_typed_reports_map(typed_reports=reports)
-
-
-class RaChangeList(ChangeList):
-    def __init__(
-        self,
-        request,
-        model,
-        list_display,
-        list_display_links,
-        list_filter,
-        date_hierarchy,
-        search_fields,
-        list_select_related,
-        list_per_page,
-        list_max_show_all,
-        list_editable,
-        model_admin,
-        sortable_by,
-    ):
-        super(RaChangeList, self).__init__(
-            request,
-            model,
-            list_display,
-            list_display_links,
-            list_filter,
-            date_hierarchy,
-            search_fields,
-            list_select_related,
-            list_per_page,
-            list_max_show_all,
-            list_editable,
-            model_admin,
-            sortable_by,
-        )
-        self.request = request  # Add request to the class
-        if self.is_popup:
-            name = gettext("Select %s")
-        else:
-            name = gettext("%s")
-        self.name = name % str(self.opts.verbose_name_plural)
-
-        self.no_records_message = model_admin.no_records_message
-
-    # def url_for_result(self, result):
-    #     """
-    #     Override parent to handle correct url mapping
-    #     :param result:
-    #     :return:
-    #     """
-    #     if self.model_admin.has_view_permission(self.request):
-    #         pk = getattr(result, self.pk_attname)
-    #         return reverse('%s:%s_%s_view' % (app_settings.RA_ADMIN_SITE_NAME, self.opts.app_label,
-    #                                           self.opts.model_name),
-    #                        args=(quote(pk),),
-    #                        current_app=self.model_admin.admin_site.name)
-    #     elif self.model_admin.has_change_permission(self.request):
-    #         pk = getattr(result, self.pk_attname)
-    #         return reverse('%s:%s_%s_change' % (app_settings.RA_ADMIN_SITE_NAME, self.opts.app_label,
-    #                                             self.opts.model_name),
-    #                        args=(quote(pk),),
-    #                        current_app=self.model_admin.admin_site.name)
-    #     elif self.model_admin.has_add_permission(self.request):
-    #         return reverse('%s:%s_%s_add' % (app_settings.RA_ADMIN_SITE_NAME, self.opts.app_label,
-    #                                          self.opts.model_name),
-    #                        current_app=self.model_admin.admin_site.name)
-    #     return False
-
-
-class RaAdminSite(RaAdminSiteBase):
+class ERPFrameworkAdminSite(ERPFrameworkAdminSiteBase):
     pass
 
 
-site_class = import_string(app_settings.RA_ADMIN_SITE_CLASS)
-erp_admin_site = site_class(name=app_settings.RA_ADMIN_SITE_NAME)
-
-
 class RaThemeMixin:
-    change_form_template = f"{app_settings.RA_THEME}/change_form.html"
-    change_list_template = f"{app_settings.RA_THEME}/change_list.html"
-    delete_confirmation_template = f"{app_settings.RA_THEME}/delete_confirmation.html"
+    change_form_template = f"{app_settings.ERP_FRAMEWORK_THEME}/change_form.html"
+    change_list_template = f"{app_settings.ERP_FRAMEWORK_THEME}/change_list.html"
+    delete_confirmation_template = (
+        f"{app_settings.ERP_FRAMEWORK_THEME}/delete_confirmation.html"
+    )
     delete_selected_confirmation_template = (
-        f"{app_settings.RA_THEME}/delete_selected_confirmation.html"
+        f"{app_settings.ERP_FRAMEWORK_THEME}/delete_selected_confirmation.html"
     )
-    add_form_template = f"{app_settings.RA_THEME}/change_form.html"
+    add_form_template = f"{app_settings.ERP_FRAMEWORK_THEME}/change_form.html"
 
     recover_form_template = f"erp_framework/reversion/recover_form.html"
     revision_form_template = f"erp_framework/reversion/revision_form.html"
     object_history_template = f"erp_framework/reversion/object_history.html"
     recover_list_template = f"erp_framework/reversion/recover_list.html"
 
-    view_template = None  # Defaults to f'{app_settings.RA_THEME}/view.html'
+    view_template = None  # Defaults to f'{app_settings.ERP_FRAMEWORK_THEME}/view.html'
 
 
 class AdminViewMixin(admin.ModelAdmin):
     enable_view_view = True
     view_fields = ()
     view_template = "erp_framework/view.html"
 
@@ -193,27 +88,27 @@
             % ("admin", self.model._meta.app_label, self.model._meta.model_name),
             args=(quote(obj.pk),),
             current_app=self.admin_site.name,
         )
 
         # todo change the str obj
         view_link = (
-            '<a href="%s" data-popup="tooltip" name="%s %s" data-placement="bottom"> '
-            '<i class="fas fa-chart-line"></i> </a>'
-            % (url, capfirst(_("Statistics for")), str(obj))
+                '<a href="%s" data-popup="tooltip" name="%s %s" data-placement="bottom"> '
+                '<i class="fas fa-chart-line"></i> </a>'
+                % (url, capfirst(_("Statistics for")), str(obj))
         )
         return mark_safe(view_link)
 
     get_stats_icon.short_description = _("Stats")
 
     def get_view_fields(self, request, obj=None):
         return (
-            self.view_fields
-            or [x for x in flatten_list(self.fields)]
-            or self.get_fields(request, obj)
+                self.view_fields
+                or [x for x in flatten_list(self.fields)]
+                or self.get_fields(request, obj)
         )
 
     def get_view_title(self, request, obj=None):
         return _("View %s") % str(obj)
         # return self.get_title(request, obj)
 
     def get_urls(self):
@@ -221,15 +116,15 @@
         info = self.model._meta.app_label, self.model._meta.model_name
 
         my_urls = [
             path(
                 "<path:object_id>/view/",
                 self.admin_site.admin_view(self.view_view),
                 name="%s_%s_view" % info,
-            ),
+            )
         ]
         return my_urls + urls
 
     def has_view_permission(self, request, obj=None):
         if not self.enable_view_view:
             return False
         opts = self.opts
@@ -314,15 +209,15 @@
         return TemplateResponse(
             request,
             self.view_template
             or [
                 "erp_framework/%s/%s/view.html" % (opts.app_label, opts.model_name),
                 "erp_framework/%s/view.html" % opts.app_label,
                 "erp_framework/view.html",
-                f"{app_settings.RA_THEME}/view.html",
+                f"{app_settings.ERP_FRAMEWORK_THEME}/view.html",
             ],
             context,
         )
 
 
 class EntityAdmin(RaThemeMixin, AdminViewMixin, VersionAdmin):
     # ModelAdmin Attributes
@@ -370,37 +265,37 @@
         pk_attname = self.model._meta.pk.attname
         pk = getattr(obj, pk_attname)
         main_url = False
         if self.has_change_permission(request, obj):
             url = reverse(
                 "%s:%s_%s_change"
                 % (
-                    app_settings.RA_ADMIN_SITE_NAME,
+                    app_settings.ERP_FRAMEWORK_SITE_NAME,
                     self.model._meta.app_label,
                     self.model._meta.model_name,
                 ),
                 args=(quote(pk),),
                 current_app=self.admin_site.name,
             )
             if not main_url:
                 main_url = url
             view_link = (
-                '<a href="%s" data-popup="tooltip" name="%s" data-placement="bottom">'
-                ' <i class="fas fa-edit"></i> </a>' % (url, capfirst(_("change")))
+                    '<a href="%s" data-popup="tooltip" name="%s" data-placement="bottom">'
+                    ' <i class="fas fa-edit"></i> </a>' % (url, capfirst(_("change")))
             )
             links.append(view_link)
             links = "<span class='go-to-change-form'>%s</span>" % "".join(links) + ""
             obj_link_title = "<a href='%s'>%s</a>" % (main_url, obj.name)
             return mark_safe("%s %s" % (obj_link_title, links))
 
         return obj.name
 
     def get_history_link(self, obj):
         info = self.model._meta.app_label, self.model._meta.model_name
-        url = reverse("erp_admin::%s_%s_history" % info, args=(obj.pk,))
+        url = reverse("erp_framework:%s_%s_history" % info, args=(obj.pk,))
 
         return mark_safe(
             """<a href="%s" class="legitRipple" data-popup="tooltip" name="%s">
                         <i class="fas fa-history text-indigo-800"></i>
                         <span class="legitRipple-ripple"></span></a>"""
             % (url, _("History"))
         )
@@ -487,48 +382,38 @@
     #         'to_field_var': TO_FIELD_VAR,
     #         'is_popup_var': IS_POPUP_VAR,
     #         'app_label': app_label,
     #     })
     #
     #     request.current_app = self.admin_site.name
     #     return TemplateResponse(request, self.view_template or [
-    #         "ra/%s/%s/view.html" % (opts.app_label, opts.model_name),
-    #         "ra/%s/view.html" % opts.app_label,
-    #         'ra/view.html',
-    #         f"{app_settings.RA_THEME}/view.html",
+    #         "erp_framework/%s/%s/view.html" % (opts.app_label, opts.model_name),
+    #         "erp_framework/%s/view.html" % opts.app_label,
+    #         'erp_framework/view.html',
+    #         f"{app_settings.ERP_FRAMEWORK_THEME}/view.html",
     #     ], context)
 
     @csrf_protect_m
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
         extra_context["description"] = self.description
         return super(EntityAdmin, self).changelist_view(request, extra_context)
 
-    # todo check and maybe bring back
-    # def get_changelist(self, request, **kwargs):
-    #     return RaChangeList
-
     def save_model(self, request, obj, form, change):
         obj.lastmod_user = request.user
         obj.lastmod_date = now()
         if not change:
             obj.owner = request.user
             obj.creation_date = now()
         super(EntityAdmin, self).save_model(request, obj, form, change)
 
     def get_urls(self):
         # Override ModelAdmin
         from django.urls import re_path as url
 
-        def wrap(view):
-            def wrapper(*args, **kwargs):
-                return self.admin_site.admin_view(view)(*args, **kwargs)
-
-            return update_wrapper(wrapper, view)
-
         info = self.model._meta.app_label, self.model._meta.model_name
         admin_site = self.admin_site
         reversion_urls = [
             url(
                 "^recover/$",
                 admin_site.admin_view(self.recoverlist_view),
                 name="%s_%s_recoverlist" % info,
@@ -549,27 +434,27 @@
 
         my_urls = [
             # path('autocomplete/', wrap(self.autocomplete_view), name='%s_%s_autocomplete' % info),
             url(
                 r"^slug/(?P<slug>[\w-]+)/$",
                 self.admin_site.admin_view(self.get_by_slug),
                 name="%s_%s_get-by-slug" % info,
-            ),
+            )
         ]
         return my_urls + reversion_urls + urlpatterns
 
     def get_by_slug(self, request, **kwargs):
         query = self.model.objects.filter(**kwargs)
         result = query.exists()
         if result:
             query = query[0]
             admin_url = reverse(
                 "%s:%s_%s_change"
                 % (
-                    app_settings.RA_ADMIN_SITE_NAME,
+                    app_settings.ERP_FRAMEWORK_SITE_NAME,
                     self.model._meta.app_label,
                     self.model._meta.model_name,
                 ),
                 args=(query.id,),
             )
             return HttpResponseRedirect(admin_url)
         else:
@@ -592,27 +477,24 @@
                         can_change_related=related_modeladmin.has_change_permission(
                             request
                         ),
                         can_delete_related=related_modeladmin.has_delete_permission(
                             request
                         ),
                     )
-                    formfield.widget = RaRelatedFieldWidgetWrapper(
+                    formfield.widget = RelatedFieldWidgetWrapper(
                         formfield.widget,
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
             return app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
                 self, db_field, formfield, request, **kwargs
             )
 
-        # if db_field.name == 'date' and db_field.__class__ == DateTimeField:
-        #     field = forms.SplitDateTimeField(widget=AdminSplitDateTimeNoBr, label=_('Date'))
-        # else:
         field = super(EntityAdmin, self).formfield_for_dbfield(
             db_field, request, **kwargs
         )
         if db_field.name == "slug" and self.enable_next_serial:
             field.initial = self.get_next_serial()
         elif db_field.name == "date":
             field.initial = now()
@@ -706,17 +588,17 @@
                 new_object = self.save_form(request, form, change=not add)
             else:
                 new_object = form.instance
             formsets, inline_instances = self._create_formsets(
                 request, new_object, change=not add
             )
             if (
-                all_valid(formsets)
-                and form_validated
-                and self.whole_changeform_validation(request, form, formsets, not add)
+                    all_valid(formsets)
+                    and form_validated
+                    and self.whole_changeform_validation(request, form, formsets, not add)
             ):
                 self.pre_save(form, formsets, change=not add)
                 self.save_model(request, new_object, form, not add)
                 self.save_related(request, form, formsets, not add)
                 self.post_save(request, new_object, form, formsets, not add)
                 changeform_saved.send(self.model, instance=new_object, created=add)
 
@@ -747,18 +629,20 @@
         if not add and not self.has_change_permission(request, obj):
             readonly_fields = flatten_fieldsets(self.get_fieldsets(request, obj))
         else:
             readonly_fields = self.get_readonly_fields(request, obj)
         adminForm = helpers.AdminForm(
             form,
             list(self.get_fieldsets(request, obj)),
-            # Clear prepopulated fields on a view-only form to avoid a crash.
-            self.get_prepopulated_fields(request, obj)
-            if add or self.has_change_permission(request, obj)
-            else {},
+            (
+                # Clear prepopulated fields on a view-only form to avoid a crash.
+                self.get_prepopulated_fields(request, obj)
+                if add or self.has_change_permission(request, obj)
+                else {}
+            ),
             readonly_fields,
             model_admin=self,
         )
         media = self.media + adminForm.media
 
         inline_formsets = self.get_inline_formsets(
             request, formsets, inline_instances, obj
@@ -785,32 +669,35 @@
             "errors": helpers.AdminErrorList(form, formsets),
             "preserved_filters": self.get_preserved_filters(request),
         }
 
         # Hide the "Save" and "Save and continue" buttons if "Save as New" was
         # previously chosen to prevent the interface from getting confusing.
         if (
-            request.method == "POST"
-            and not form_validated
-            and "_saveasnew" in request.POST
+                request.method == "POST"
+                and not form_validated
+                and "_saveasnew" in request.POST
         ):
             context["show_save"] = False
             context["show_save_and_continue"] = False
             # Use the change template instead of the add template.
             add = False
 
         context.update(extra_context or {})
 
         return self.render_change_form(
             request, context, add=add, change=not add, obj=obj, form_url=form_url
         )
 
     def get_actions(self, request):
         actions = super(EntityAdmin, self).get_actions(request)
-        if not (app_settings.RA_ENABLE_ADMIN_DELETE_ALL and request.user.is_superuser):
+        if not (
+                app_settings.ERP_FRAMEWORK_ENABLE_ADMIN_DELETE_ALL
+                and request.user.is_superuser
+        ):
             if "delete_selected" in actions:
                 del actions["delete_selected"]
         return actions
 
     def get_list_display(self, request):
         list_display = super(EntityAdmin, self).get_list_display(request)
 
@@ -824,19 +711,15 @@
     enable_view_view = False
     list_per_page = 50
     view_on_site = False
     list_display = ("slug", "date", "value", "get_history_link")
     list_display_links = ("slug", "date")
     fields = (("slug", "date"),)
     exclude = ("type",)
-    formfield_overrides = {
-        # DateTimeField: {'widget': AdminSplitDateTimeNoBr},
-        # DecimalField: {'widget': NumberInput},
-        # ForeignKey: {'widget': RaBootstrapForeignKeyWidget},
-    }
+    formfield_overrides = {}
     date_hierarchy = "date"
     type = None
 
     # Copy values from parent model to child inline models,
     # If `all-fk` then automatically it will copy all foreign keys included in the fields of the add/change Form
     # other options are None , or a list of field names
     copy_to_inlines = "all-fk"
@@ -891,15 +774,15 @@
                 # print(copy_item, form.instance.__getattribute__(copy_item))
             if formset_form.instance.pk is not None:
                 formset_form.instance.save()
         formset.save()
 
 
 class TransactionItemAdmin(admin.TabularInline):
-    template = f"{app_settings.RA_THEME}/edit_inline/tabular.html"
+    template = f"{app_settings.ERP_FRAMEWORK_THEME}/edit_inline/tabular.html"
     extra = 2
     exclude = (
         "slug",
         "date",
         "type",
         "lastmod",
         "lastmod_user",
@@ -939,15 +822,16 @@
             return self.permission_override_model
 
         elif type(self.permission_override_model) is ModelBase:
             return self.permission_override_model._meta.model_name
 
         else:
             raise ImproperlyConfigured(
-                "self.permission_override_model can be True, False , str or ModelBase .Got %s instead "
+                "self.permission_override_model can be True, False , str or ModelBase"
+                " .Got %s instead "
                 % type(self.permission_override_model)
             )
 
     def has_add_permission(self, request, obj=None):
         if self.opts.auto_created:
             # We're checking the rights to an auto-created intermediate model,
             # which doesn't have its own individual permissions. The user needs
@@ -1010,15 +894,15 @@
                         can_change_related=related_modeladmin.has_change_permission(
                             request
                         ),
                         can_delete_related=related_modeladmin.has_delete_permission(
                             request
                         ),
                     )
-                    formfield.widget = RaRelatedFieldWidgetWrapper(
+                    formfield.widget = RelatedFieldWidgetWrapper(
                         formfield.widget,
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
         form_field = super(TransactionItemAdmin, self).formfield_for_dbfield(
             db_field, request, **kwargs
@@ -1067,15 +951,15 @@
                         can_change_related=related_modeladmin.has_change_permission(
                             request
                         ),
                         can_delete_related=related_modeladmin.has_delete_permission(
                             request
                         ),
                     )
-                    formfield.widget = RaRelatedFieldWidgetWrapper(
+                    formfield.widget = RelatedFieldWidgetWrapper(
                         formfield.widget,
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
         form_field = super(RaGenericTabularInline, self).formfield_for_dbfield(
             db_field, request, **kwargs
@@ -1224,24 +1108,20 @@
                 )
             else:
                 initial_data = self.get_formset_initial(
                     inline, inline_queryset, request, obj, change
                 )
                 # Not here is a necessity, in case you find unuseful revise again
                 if (
-                    inline.__class__ in self.prepopulated_inlines
-                    or not self.prepopulated_inlines
+                        inline.__class__ in self.prepopulated_inlines
+                        or not self.prepopulated_inlines
                 ):
                     FormSet.extra = len(initial_data)
                 if initial_data:
-                    formset_params.update(
-                        {
-                            "initial": initial_data,
-                        }
-                    )
+                    formset_params.update({"initial": initial_data})
             formsets.append(FormSet(**formset_params))
             inline_instances.append(inline)
         return formsets, inline_instances
 
 
 class RaPrePopulatedAdmin(PrepopulatedAdmin, EntityAdmin):
     pass
@@ -1264,67 +1144,67 @@
             for copy_item in self.copy_to_inlines:
                 formset_form.instance.__setattr__(
                     copy_item, form.instance.__getattribute__(copy_item)
                 )
 
         formset.save()
 
-
-class RaUserAdmin(RaThemeMixin, UserTabularPermissionsMixin, UserAdmin):
-    enable_view_view = False
-    date_hierarchy = None
-    fields = None
-    list_display_links = ["username"]
-    change_user_password_template = (
-        f"{app_settings.RA_THEME}/auth/user/change_password.html"
-    )
-    list_display = ("username", "is_superuser", "last_login", "is_active")
-
-    save_on_top = True
-
-    fieldsets = (
-        (None, {"fields": ("username", "password")}),
-        (_("Personal info"), {"fields": (("first_name", "last_name", "email"),)}),
-        (
-            _("Permissions"),
-            {"fields": (("is_active", "is_superuser"), "groups", "user_permissions")},
-        ),
-        # (_('Important dates'), {'fields': (('last_login', 'date_joined'),)}),
-    )
-    list_filter = ("is_superuser", "is_active", "groups")
-    form = RaUserChangeForm
-
-    def get_actions(self, request):
-        actions = super(RaUserAdmin, self).get_actions(request)
-        if "delete_selected" in actions:
-            del actions["delete_selected"]
-        return actions
-
-    def has_delete_permission(self, request, obj=None):
-        return False
-
-    def save_model(self, request, obj, form, change):
-        obj.is_staff = True
-        super(RaUserAdmin, self).save_model(request, obj, form, change)
-
-    def get_inline_instances(self, request, obj=None):
-        if obj is None:
-            return []
-        return super(RaUserAdmin, self).get_inline_instances(request, obj)
-
-    def changelist_view(self, request, extra_context=None):
-        extra_context = {"has_detached_sidebar": True}
-        return super(RaUserAdmin, self).changelist_view(request, extra_context)
-
-
-class RaGroupAdmin(RaThemeMixin, GroupTabularPermissionsMixin, GroupAdmin):
-    enable_view_view = False
-    date_hierarchy = None
-    fields = None
-    list_display_links = ["name"]
-    list_display = ["name"]
-
-    save_on_top = True
-
-
-erp_admin_site.register(Group, RaGroupAdmin)
-erp_admin_site.register(User, RaUserAdmin)
+# class RaUserAdmin(RaThemeMixin, UserTabularPermissionsMixin, UserAdmin):
+#     enable_view_view = False
+#     date_hierarchy = None
+#     fields = None
+#     list_display_links = ["username"]
+#     change_user_password_template = (
+#         f"{app_settings.ERP_FRAMEWORK_THEME}/auth/user/change_password.html"
+#     )
+#     list_display = ("username", "is_superuser", "last_login", "is_active")
+#
+#     save_on_top = True
+#
+#     fieldsets = (
+#         (None, {"fields": ("username", "password")}),
+#         (_("Personal info"), {"fields": (("first_name", "last_name", "email"),)}),
+#         (
+#             _("Permissions"),
+#             {"fields": (("is_active", "is_superuser"), "groups", "user_permissions")},
+#         ),
+#         # (_('Important dates'), {'fields': (('last_login', 'date_joined'),)}),
+#     )
+#     list_filter = ("is_superuser", "is_active", "groups")
+#     form = CustomUserChangeForm
+#
+#     def get_actions(self, request):
+#         actions = super(RaUserAdmin, self).get_actions(request)
+#         if "delete_selected" in actions:
+#             del actions["delete_selected"]
+#         return actions
+#
+#     def has_delete_permission(self, request, obj=None):
+#         return False
+#
+#     def save_model(self, request, obj, form, change):
+#         obj.is_staff = True
+#         super(RaUserAdmin, self).save_model(request, obj, form, change)
+#
+#     def get_inline_instances(self, request, obj=None):
+#         if obj is None:
+#             return []
+#         return super(RaUserAdmin, self).get_inline_instances(request, obj)
+#
+#     def changelist_view(self, request, extra_context=None):
+#         extra_context = {"has_detached_sidebar": True}
+#         return super(RaUserAdmin, self).changelist_view(request, extra_context)
+#
+#
+# class RaGroupAdmin(RaThemeMixin, GroupTabularPermissionsMixin, GroupAdmin):
+#     enable_view_view = False
+#     date_hierarchy = None
+#     fields = None
+#     list_display_links = ["name"]
+#     list_display = ["name"]
+#
+#     save_on_top = True
+#
+#
+#
+# erp_admin_site.register(Group, RaGroupAdmin)
+# erp_admin_site.register(User, RaUserAdmin)
```

### Comparing `django-erp-framework-0.9.12/erp_framework/admin/base.py` & `django-erp-framework-1.5.0/erp_framework/admin/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from django.template.response import TemplateResponse
 from django.urls import re_path as url, include
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
 from erp_framework.admin.helpers import get_each_context
 from erp_framework.base import app_settings
-from erp_framework.base.helpers import get_from_list
 
 # from erp_framework.top_search.views import TopSearchView
 
 logger = logging.getLogger(__name__)
 CACHE_DURATION = 0
 
 MSG_ADDED_SUCCESSFULLY = _('The %(name)s "%(obj)s" was added successfully.')
@@ -45,37 +44,34 @@
 def get_report_view(request, base_model, report_slug):
     from erp_framework.reporting.registry import report_registry
 
     klass = report_registry.get(base_model, report_slug)
     return klass.as_view()(request)
 
 
-class RaAdminSiteBase(AdminSite):
+class ERPFrameworkAdminSiteBase(AdminSite):
     site_title = app_settings.ERP_ADMIN_SITE_TITLE
     site_header = app_settings.ERP_ADMIN_SITE_HEADER
     index_title = app_settings.ERP_ADMIN_INDEX_TITLE
 
     index_template = app_settings.ERP_ADMIN_INDEX_TEMPLATE
-    app_index_template = app_settings.RA_ADMIN_APP_INDEX_TEMPLATE
-    login_template = app_settings.RA_ADMIN_LOGIN_TEMPLATE
-
-    # logout_template = app_settings.RA_ADMIN_LOGGED_OUT_TEMPLATE
+    app_index_template = app_settings.ERP_FRAMEWORK_APP_INDEX_TEMPLATE
+    login_template = app_settings.ERP_FRAMEWORK_LOGIN_TEMPLATE
+    logout_template = app_settings.ERP_FRAMEWORK_LOGGED_OUT_TEMPLATE
 
     def get_urls(self):
         # from erp_framework.utils.views import access_denied
         def wrap(view, cacheable=False):
             def wrapper(*args, **kwargs):
                 return self.admin_view(view, cacheable)(*args, **kwargs)
 
             return update_wrapper(wrapper, view)
 
-        urls = super(RaAdminSiteBase, self).get_urls()
-        help_center = [
-            url(r"^i18n/", include("django.conf.urls.i18n")),
-        ]
+        urls = super(ERPFrameworkAdminSiteBase, self).get_urls()
+        help_center = [url(r"^i18n/", include("django.conf.urls.i18n"))]
 
         settings_update = [
             url(r"^manifest/$", self.manifest_view, name="manifest"),
             url(r"^sw.js$", self.service_worker_view, name="service-worker"),
         ]
 
         urlpatterns = [
@@ -105,15 +101,15 @@
 
     def manifest_view(self, request):
         json = {
             "short_name": "ERP Framework System",
             "name": "ERP Framework System",
             "icons": [
                 {
-                    "src": "/static/ra/images/ra_systems.png",
+                    "src": "/static/erp_framework/images/ra_systems.png",
                     "type": "image/png",
                     "sizes": "147x147",
                 },
                 # {
                 #     "src": "launcher-icon-2x.png",
                 #     "type": "image/png",
                 #     "sizes": "96x96"
@@ -128,15 +124,15 @@
             "display": "standalone",
             "theme_color": "#000066",
             "background_color": "#fff",
         }
         return JsonResponse(json, status=200)
 
     def __init__(self, name="admin"):
-        super(RaAdminSiteBase, self).__init__(name)
+        super(ERPFrameworkAdminSiteBase, self).__init__(name)
 
         self._registry_names = {}  # holds model name -> ModelAdmin instances
         #                  l-> Model
         self._registered_models_CT = []
 
     def _fill_registry_names(self):
         """
@@ -151,21 +147,21 @@
                 "admin": self._registry[model],
                 "model": model,
             }
 
     def app_index(self, request, app_label, extra_context=None):
         app_name = apps.get_app_config(app_label).verbose_name
         context = self.each_context(request)
-        app_list = context["app_list"]
-        current_app_list = get_from_list(False, app_list, "app_label", app_label)
+        # app_list = context["app_list"]
+        # current_app_list = get_from_list(False, app_list, "app_label", app_label)
         context.update(
             dict(
                 title=_("%(app)s administration") % {"app": app_name},
                 # current_app_list=[app_dict],
-                current_app_list=[current_app_list],
+                # current_app_list=[current_app_list],
                 app_label=app_label,
                 app_name=app_name,
             )
         )
         context.update(extra_context or {})
         request.current_app = self.name
 
@@ -177,30 +173,27 @@
         )
 
     def index(self, request, extra_context=None):
         extra_context = extra_context or {}
         extra_context["opts"] = {"app_name": "home"}
         extra_context["is_index"] = True
         extra_context["sidebar_status"] = "expanded"
-        context = dict(
-            self.each_context(request),
-            name=self.index_title,
-        )
+        context = dict(self.each_context(request), name=self.index_title)
         context.update(extra_context or {})
 
         request.current_app = self.name
         context["title"] = app_settings.ERP_ADMIN_INDEX_TITLE
 
         return TemplateResponse(
             request, self.index_template or "admin/index.html", context
         )
 
     def each_context(self, request):
-        context = super(RaAdminSiteBase, self).each_context(request)
-        context["RA_ADMIN_SITE_NAME"] = app_settings.RA_ADMIN_SITE_NAME
+        context = super(ERPFrameworkAdminSiteBase, self).each_context(request)
+        context["ERP_FRAMEWORK_SITE_NAME"] = app_settings.ERP_FRAMEWORK_SITE_NAME
         context.update(get_each_context(request, self))
         return context
 
     def get_admin_by_model_name(self, model_name):
         """
         Get the model admin of a model by its name
         :param model_name:
@@ -209,8 +202,8 @@
         if not self._registry_names:
             self._fill_registry_names()
         return self._registry_names.get(model_name, None)
 
     def login(self, request, extra_context=None):
         extra_context = extra_context or {}
         # extra_context["SHOW_LANGUAGE_SELECTOR"] = True
-        return super(RaAdminSiteBase, self).login(request, extra_context)
+        return super(ERPFrameworkAdminSiteBase, self).login(request, extra_context)
```

### Comparing `django-erp-framework-0.9.12/erp_framework/admin/helpers.py` & `django-erp-framework-1.5.0/erp_framework/admin/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import unicode_literals
 
-from django.core.cache import cache
-from django.conf import settings
 from django.utils.translation import get_language
 
-from erp_framework.base.helpers import admin_get_app_list
+
+# from erp_framework.base.helpers import admin_get_app_list
 
 
 def get_each_context(request, admin_site):
     context = {}
     current_language = get_language() or ""
     cache_key = "app_list_%s_%s" % (request.user.pk, current_language)
-    cache_val = cache.get(cache_key)
-    if not cache_val or settings.DEBUG:
-        cache_val = admin_get_app_list(request, admin_site)
-        cache.set(cache_key, cache_val)
-    context["app_list"] = cache_val
+    # cache_val = cache.get(cache_key)
+    # if not cache_val or settings.DEBUG:
+    #     cache_val = admin_get_app_list(request, admin_site)
+    #     cache.set(cache_key, cache_val)
+    # context["app_list"] = cache_val
     context["admin_site"] = admin_site
     return context
```

### Comparing `django-erp-framework-0.9.12/erp_framework/base/helpers.py` & `django-erp-framework-1.5.0/erp_framework/base/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-from __future__ import unicode_literals
-
 import logging
-from collections import OrderedDict
 from collections.abc import Iterable
 
 from django.apps import apps
 from django.db.models import Max
-from django.template.defaultfilters import capfirst
-from django.urls import reverse, NoReverseMatch
 
 logger = logging.getLogger(__name__)
 
 get_model = apps.get_model
 
 
 def get_obj_from_list(lst, key, val):
@@ -52,116 +47,114 @@
         ):
             return True
         if model._meta.auto_created:
             return True
         return False
 
 
-def order_apps(app_list):
-    """Called in admin/base_site.html template override and applies custom ordering of
-    apps/models defined by settings.ADMIN_REORDER
-    """
-    from . import app_settings
-
-    # sort key function - use index of item in order if exists, otherwise item
-    sort = (
-        lambda order, item: (order.index(item), "")
-        if item in order
-        else (len(order), item)
-    )
-
-    # sort the app list
-    order = OrderedDict(app_settings.ADMIN_REORDER)
-    app_list.sort(
-        key=lambda app: sort(order.keys(), app["app_url"].strip("/").split("/")[-1])
-    )
-    for i, app in enumerate(app_list):
-        # sort the model list for each app
-        app_name = app["app_url"].strip("/").split("/")[-1]
-        model_order = [m.lower() for m in order.get(app_name, [])]
-        app_list[i]["models"].sort(
-            key=lambda model: sort(
-                model_order, model.get("admin_url", "").strip("/").split("/")[-1]
-            )
-        )
-    return app_list
-
-
-def admin_get_app_list(request, admin_site):
-    """
-    :param request: Copied from AdminSite.index() djagno v1.8
-    :param admin_site:
-    :return:
-    """
-    from erp_framework.base.app_settings import RA_MENU_HIDE_MODELS, RA_ADMIN_SITE_NAME
-
-    app_dict = {}
-    for model, model_admin in admin_site._registry.items():
-        app_label = model._meta.app_label
-        has_module_perms = model_admin.has_module_permission(request)
-
-        is_model_hidden = (
-            "%s_%s" % (app_label, model.__name__.lower()) in RA_MENU_HIDE_MODELS
-        )
-
-        if has_module_perms and not is_model_hidden:
-            perms = model_admin.get_model_perms(request)
-
-            # Check whether user has any perm for this module.
-            # If so, add the module to the model_list.
-            if True in perms.values():
-                info = (RA_ADMIN_SITE_NAME, app_label, model._meta.model_name)
-                model_dict = {
-                    "name": capfirst(model._meta.verbose_name_plural),
-                    "object_name": model._meta.object_name,
-                    "perms": perms,
-                    "model_class": model,
-                }
-                if (
-                    perms.get("view", False)
-                    or perms.get("change", False)
-                    or perms.get("add", False)
-                ):
-                    try:
-                        model_dict["admin_url"] = reverse(
-                            "%s:%s_%s_changelist" % info, current_app=admin_site.name
-                        )
-                    except NoReverseMatch:
-                        pass
-                if perms.get("add", False):
-                    try:
-                        model_dict["add_url"] = reverse(
-                            "%s:%s_%s_add" % info, current_app=admin_site.name
-                        )
-                    except NoReverseMatch:
-                        pass
-                if app_label in app_dict:
-                    app_dict[app_label]["models"].append(model_dict)
-                else:
-                    app_dict[app_label] = {
-                        "name": apps.get_app_config(app_label).verbose_name,
-                        "app_label": app_label,
-                        "app_url": reverse(
-                            "%s:app_list" % RA_ADMIN_SITE_NAME,
-                            kwargs={"app_label": app_label},
-                            current_app=admin_site.name,
-                        ),
-                        "has_module_perms": has_module_perms,
-                        "models": [model_dict],
-                    }
-
-    # Sort the apps alphabetically.
-    app_list = list(app_dict.values())
-    app_list.sort(key=lambda x: x["name"].lower())
-
-    # Sort the models alphabetically within each app.
-    for app in app_list:
-        app["models"].sort(key=lambda x: x["name"])
-
-    return order_apps(app_list)
+# def order_apps(app_list):
+#     """Called in admin/base_site.html template override and applies custom ordering of
+#     apps/models defined by settings.ADMIN_REORDER
+#     """
+#     from . import app_settings
+#
+#     # sort key function - use index of item in order if exists, otherwise item
+#     sort = lambda order, item: (
+#         (order.index(item), "") if item in order else (len(order), item)
+#     )
+#
+#     # sort the app list
+#     order = OrderedDict(app_settings.ADMIN_REORDER)
+#     app_list.sort(
+#         key=lambda app: sort(order.keys(), app["app_url"].strip("/").split("/")[-1])
+#     )
+#     for i, app in enumerate(app_list):
+#         # sort the model list for each app
+#         app_name = app["app_url"].strip("/").split("/")[-1]
+#         model_order = [m.lower() for m in order.get(app_name, [])]
+#         app_list[i]["models"].sort(
+#             key=lambda model: sort(
+#                 model_order, model.get("admin_url", "").strip("/").split("/")[-1]
+#             )
+#         )
+#     return app_list
+#
+
+# def admin_get_app_list(request, admin_site):
+#     """
+#     :param request: Copied from AdminSite.index() djagno v1.8
+#     :param admin_site:
+#     :return:
+#     """
+#     from erp_framework.base.app_settings import RA_MENU_HIDE_MODELS, ERP_FRAMEWORK_SITE_NAME
+#
+#     app_dict = {}
+#     for model, model_admin in admin_site._registry.items():
+#         app_label = model._meta.app_label
+#         has_module_perms = model_admin.has_module_permission(request)
+#
+#         is_model_hidden = (
+#             "%s_%s" % (app_label, model.__name__.lower()) in RA_MENU_HIDE_MODELS
+#         )
+#
+#         if has_module_perms and not is_model_hidden:
+#             perms = model_admin.get_model_perms(request)
+#
+#             # Check whether user has any perm for this module.
+#             # If so, add the module to the model_list.
+#             if True in perms.values():
+#                 info = (ERP_FRAMEWORK_SITE_NAME, app_label, model._meta.model_name)
+#                 model_dict = {
+#                     "name": capfirst(model._meta.verbose_name_plural),
+#                     "object_name": model._meta.object_name,
+#                     "perms": perms,
+#                     "model_class": model,
+#                 }
+#                 if (
+#                     perms.get("view", False)
+#                     or perms.get("change", False)
+#                     or perms.get("add", False)
+#                 ):
+#                     try:
+#                         model_dict["admin_url"] = reverse(
+#                             "%s:%s_%s_changelist" % info, current_app=admin_site.name
+#                         )
+#                     except NoReverseMatch:
+#                         pass
+#                 if perms.get("add", False):
+#                     try:
+#                         model_dict["add_url"] = reverse(
+#                             "%s:%s_%s_add" % info, current_app=admin_site.name
+#                         )
+#                     except NoReverseMatch:
+#                         pass
+#                 if app_label in app_dict:
+#                     app_dict[app_label]["models"].append(model_dict)
+#                 else:
+#                     app_dict[app_label] = {
+#                         "name": apps.get_app_config(app_label).verbose_name,
+#                         "app_label": app_label,
+#                         "app_url": reverse(
+#                             "%s:app_list" % ERP_FRAMEWORK_SITE_NAME,
+#                             kwargs={"app_label": app_label},
+#                             current_app=admin_site.name,
+#                         ),
+#                         "has_module_perms": has_module_perms,
+#                         "models": [model_dict],
+#                     }
+#
+#     # Sort the apps alphabetically.
+#     app_list = list(app_dict.values())
+#     app_list.sort(key=lambda x: x["name"].lower())
+#
+#     # Sort the models alphabetically within each app.
+#     for app in app_list:
+#         app["models"].sort(key=lambda x: x["name"])
+#
+#     return order_apps(app_list)
 
 
 def dictsort(value, arg, desc=False):
     """
     Takes a list of dicts, returns that list sorted by the property given in
     the argument.
     """
```

### Comparing `django-erp-framework-0.9.12/erp_framework/base/models.py` & `django-erp-framework-1.5.0/erp_framework/base/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import datetime
 import logging
 
-from crequest.middleware import CrequestMiddleware
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.urls import reverse, NoReverseMatch
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 
-from . import app_settings, registry
+from . import app_settings
 
 logger = logging.getLogger(__name__)
 User = get_user_model()
 
 
 class DiffingMixin(object):
     def __init__(self, *args, **kwargs):
@@ -78,15 +77,15 @@
         abstract = True
 
 
 class ERPMixin:
     @classmethod
     def get_class_name(cls):
         """
-        return the class name, usable when a ra model is mimicking (ie:proxying)
+        return the class name, usable when a erp_framework model is mimicking (ie:proxying)
         another model.
         This method is used is get_doc_type_* functions,
         This method is made to avoid to repeat registered type to make adjustments
         """
         return cls.__name__
 
     @classmethod
@@ -105,15 +104,15 @@
         :return:
         """
         return cls._meta.verbose_name_plural
 
 
 class EntityModel(ERPMixin, RAModel):
     """
-    The Main base for Ra `static` models
+    The Main base for ERP framework `static` models
     Example: Client , Expense etc..
     """
 
     slug = models.SlugField(
         _("Identifier slug"),
         help_text=_("For fast recall"),
         max_length=50,
@@ -137,22 +136,26 @@
         return self.name
 
     def get_absolute_url(self):
         model_name = self._meta.model_name.lower()
         try:
             url = reverse(
                 "%s:%s_%s_view"
-                % (app_settings.RA_ADMIN_SITE_NAME, self._meta.app_label, model_name),
+                % (
+                    app_settings.ERP_FRAMEWORK_SITE_NAME,
+                    self._meta.app_label,
+                    model_name,
+                ),
                 args=(self.pk,),
             )
         except NoReverseMatch:
             url = reverse(
                 "%s:%s_%s_change"
                 % (
-                    app_settings.RA_ADMIN_SITE_NAME,
+                    app_settings.ERP_FRAMEWORK_SITE_NAME,
                     self._meta.app_label,
                     self.get_class_name().lower(),
                 ),
                 args=(self.pk,),
             )
         return url
 
@@ -168,44 +171,42 @@
         return get_next_serial(self.__class__)  # repr(time.time()).replace('.', '')
 
     def save(self, *args, **kwargs):
         if self.pk is None:
             if not self.slug:
                 self.slug = self.get_next_slug(self.name)
                 # print(self.slug)
-            if not self.owner_id:
-                try:
-                    self.owner = self.lastmod_user
-                except:
-                    self.owner_id = self.lastmod_user_id
-                    logger.info(
-                        "lastmod_user_id is used instead of lastmod_user object"
-                    )
+            if not self.owner_id and self.lastmod_user_id:
+                self.owner_id = self.lastmod_user_id
+
+            if not self.lastmod_user_id and self.owner_id:
+                self.lastmod_user_id = self.owner_id
 
         self.lastmod = now()
 
         super(EntityModel, self).save(*args, **kwargs)
 
     @classmethod
     def _get_doc_type_plus_list(cls):
         """
 
         Returns List of Identified doctype that a plus effect on the entity
         """
-        return ["fb"] + registry.get_model_doc_type_map(cls.get_class_name()).get(
-            "plus_list", []
-        )
+        return []
+        # return ["fb"] + registry.get_model_doc_type_map(cls.get_class_name()).get(
+        #     "plus_list", []
+        # )
 
     @classmethod
     def _get_doc_type_minus_list(cls):
         """Returns List of Identified doctype that a minus effect on the entity"""
-
-        return registry.get_model_doc_type_map(cls.get_class_name()).get(
-            "minus_list", []
-        )
+        return []
+        # return registry.get_model_doc_type_map(cls.get_class_name()).get(
+        #     "minus_list", []
+        # )
 
     @classmethod
     def get_doc_type_neuter_list(cls):
         """Returns List of Identified doctype that have a neuttral effect on the entity"""
 
         return []
 
@@ -226,70 +227,26 @@
     # def get_doc_types(cls):
     #     """
     #     Return a list of the doc_types supported by the current model , Must implemented when needed by children
     #     @return:
     #     """
     #     return cls._get_doc_type_plus_list() + cls._get_doc_type_minus_list() + cls.get_doc_type_neuter_list()
 
-    def get_pk_name(self):
-        """
-        This is used to get the full name of the primary key,
-        a bit hackish but is important for reports.
-        :return:
-        """
-        if self.pk_name:
-            return self.pk_name
-        else:
-            # return self._meta.pk.column #not now
-            return "%s_id" % self.__class__.__name__.lower()
-
-    def get_title(self):
-        """
-        A helper function to get a custom name of the instance if needed
-        :return:
-        """
-        return self.name
-
     @classmethod
     def get_report_list_url(cls):
         """
         Return the url for the report list for this model
         :return: a string url
         """
-
+        # todo consider deleting
         return reverse(
-            "%s:report_list" % app_settings.RA_ADMIN_SITE_NAME,
+            "%s:report_list" % app_settings.ERP_FRAMEWORK_SITE_NAME,
             args=(cls.get_class_name().lower(),),
         )
 
-    @classmethod
-    def get_redirect_url_prefix(cls):
-        """
-        Get the url for the change list of this model
-        :return: a string url
-        """
-        return reverse(
-            "%s:%s_%s_changelist"
-            % (
-                app_settings.RA_ADMIN_SITE_NAME,
-                cls._meta.app_label,
-                cls.get_class_name().lower(),
-            )
-        )
-
-
-# class BasePersonInfo(BaseInfo):
-#     address = models.CharField(_('address'), max_length=260, null=True, blank=True)
-#     telephone = models.CharField(_('telephone'), max_length=130, null=True, blank=True)
-#     email = models.EmailField(_('email'), null=True, blank=True)
-#
-#     class Meta:
-#         abstract = True
-#         # swappable = swapper.swappable_setting('ra', 'BasePersonInfo')
-
 
 class TransactionModel(EntityModel):
     name = None
 
     slug = models.SlugField(
         _("Slug"), max_length=50, db_index=True, validators=[], blank=True
     )
@@ -300,32 +257,30 @@
 
     owner = models.ForeignKey(
         User,
         related_name="%(app_label)s_%(class)s_related",
         verbose_name=_("Created By"),
         on_delete=models.CASCADE,
     )
-    creation_date = models.DateTimeField(_("Creation timestamp"), default=now)
-    lastmod = models.DateTimeField(_("Last modification"), db_index=True)
+    creation_date = models.DateTimeField(_("Created"), default=now)
+    lastmod = models.DateTimeField(_("Last modified"), db_index=True)
     lastmod_user = models.ForeignKey(
         User,
         related_name="%(app_label)s_%(class)s_lastmod_related",
         verbose_name=_("Last modification by"),
         on_delete=models.CASCADE,
     )
 
     @classmethod
     def get_doc_type(cls):
         """
         Return the type
         :return:
         """
         return cls.__name__.lower()
-        # raise NotImplementedError(
-        #     f'Class {cls} dont have a get_doc_type override. Each Transaction should define a *type*')
 
     def __str__(self):
         return "%s-%s" % (self._meta.verbose_name, self.slug)
 
     def __repr__(self):
         return "<%s pk:%s slug:%s type:%s>" % (
             self.__class__.__name__,
@@ -347,50 +302,18 @@
         :param using:
         :param update_fields:
         :return:
         """
 
         from erp_framework.base.helpers import get_next_serial
 
-        request = CrequestMiddleware.get_request()
         self.type = self.get_doc_type()
         if not self.slug:
             self.slug = get_next_serial(self.__class__)
-
-        # self.slug = slugify(self.slug)
-        if not self.pk:
-            if not self.lastmod_user_id:
-                self.lastmod_user_id = request.user.pk
-            if not self.owner_id:
-                self.owner_id = request.user.pk
-            self.date = self.date if self.date else now()
-        self.lastmod = now()
-
-        super(EntityModel, self).save(*args, **kwargs)
-
-    #
-    # @classmethod
-    # def get_doc_type_verbose_name(cls, type):
-    #     """
-    #     Return the type verbose name , Must be implemented when needed by children
-    #     @param type: the type field value
-    #     @return: the description of the type
-    #     Example: In: get_doc_type_verbose_name('1')
-    #             Out: Purchase
-    #     """
-    #     # Example :
-    #     # if type == '1': return _('purchase')
-    #     raise NotImplemented()
-
-    # def get_absolute_url(self):
-    #     doc_types = registry.get_doc_type_settings()
-    #     if self.type in doc_types:
-    #         return '%sslug/%s/' % (doc_types[self.type]['redirect_url_prefix'], self.slug)
-    #     else:
-    #         return self.type
+        super().save(*args, **kwargs)
 
     @property
     def name(self):
         return self.date.strftime("%Y/%m/%d %H:%M")
 
 
 class TransactionItemModel(TransactionModel):
@@ -447,32 +370,25 @@
 
     @classmethod
     def get_doc_type_plus_list(cls):
         """
 
         Returns List of Identified doctype that a plus effect on the entity
         """
-        return []  # ['0','3' , 'client-cash-in','supplier-cash-in']
+        return []
 
     @classmethod
     def get_doc_type_minus_list(cls):
         """Returns List of Identified doctype that a minus effect on the entity"""
 
-        return []  # ['1', '2', 'client-cash-out', 'supplier-cash-out']
-
-    # @classmethod
-    # def get_doc_types(cls):
-    #     """
-    #     Return a list of the doc_types supported by the current model , Must implemented when needed by children
-    #     @return:
-    #     """
-    #     return cls.get_doc_type_plus_list() + cls.get_doc_type_minus_list()
+        return []
 
     class Meta:
         abstract = True
+        default_permissions = ()
 
 
 class QuanValueReport(BaseReportModel):
     quantity = models.DecimalField(
         _("quantity"), max_digits=19, decimal_places=2, default=0
     )
     price = models.DecimalField(_("price"), max_digits=19, decimal_places=2, default=0)
@@ -482,59 +398,17 @@
 
     @classmethod
     def get_doc_type_plus_list(cls):
         """
 
         Returns List of Identified doctype that a plus effect on the entity
         """
-        return []  # ['0','3' , 'client-cash-in','supplier-cash-in']
+        return []
 
     @classmethod
     def get_doc_type_minus_list(cls):
         """Returns List of Identified doctype that a minus effect on the entity"""
 
-        return []  # ['1', '2', 'client-cash-out', 'supplier-cash-out']
-
-    # @classmethod
-    # def get_doc_types(cls):
-    #     """
-    #     Return a list of the doc_types supported by the current model , Must implemented when needed by children
-    #     @return:
-    #     """
-    #     return cls.get_doc_type_plus_list() + cls.get_doc_type_minus_list()
+        return []
 
     class Meta:
         abstract = True
-
-
-class ProxyMovementManager(models.Manager):
-    def get_queryset(self):
-        return (
-            super(ProxyMovementManager, self)
-            .get_queryset()
-            .filter(type=self.model.get_doc_type())
-        )
-
-
-class ProxyMovement(object):
-    objects = ProxyMovementManager()
-
-    @classmethod
-    def get_doc_type(cls):
-        """
-        Get the doc-type of the row.
-        This method is called internally during save to ensure that the record in the
-        proxy model always have the right type
-        :return: string (type)
-        """
-        return ""
-
-    def __init__(self, *args, **kwargs):
-        super(ProxyMovement, self).__init__(*args, **kwargs)
-        self._doc_type = ""
-
-    def save(self, *args, **kwargs):
-        self.type = self.__class__.get_doc_type()
-        super(ProxyMovement, self).save(*args, **kwargs)
-
-    class Meta:
-        proxy = True
```

### Comparing `django-erp-framework-0.9.12/erp_framework/reporting/forms.py` & `django-erp-framework-1.5.0/erp_framework/reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.12/erp_framework/reporting/printing.py` & `django-erp-framework-1.5.0/erp_framework/reporting/printing.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.12/erp_framework/reporting/templatetags/erp_reporting_tags.py` & `django-erp-framework-1.5.0/erp_framework/reporting/templatetags/erp_reporting_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 
 from erp_framework.base import app_settings
 
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
-def render_reports_menu(context):
+def render_reports_menu(context, template_name="erp_framework/reports_menu.html"):
     request = context["request"]
     is_in_reports = False
     active_base_model = ""
     if request.path.startswith("/reports/"):
         is_in_reports = True
         active_base_model = [x for x in request.path.split("/") if x][1]
 
     from erp_framework.reporting.registry import report_registry
 
     base_models = report_registry.get_base_models_with_reports()
     if base_models:
-        t = get_template(f"erp_framework/reports_menu.html")
         output = render_to_string(
-            "erp_framework/reports_menu.html",
+            template_name,
             {
                 "base_models_reports_tuple": base_models,
                 "is_report": context.get("is_report", False),
                 "base_model": context.get("base_model", False),
                 "report_slug": context.get("report_slug", False),
                 "current_base_model_name": context.get(
                     "current_base_model_name", False
@@ -71,12 +70,14 @@
     if not report:
         raise ValueError(
             "report argument is empty. Are you sure you're using the correct report name"
         )
 
     # No chart argument default to True if no charts in reports
     kwargs.setdefault("no_chart", not bool(report.chart_settings))
+    kwargs.setdefault("data_display_chart_selector", kwargs["no_chart"])
+    kwargs.setdefault("title", report.get_report_title())
 
     template = get_template(
         template_name or "erp_framework/report_widget_template.html"
     )
     return template.render(context=kwargs)
```

### Comparing `django-erp-framework-0.9.12/erp_framework/utils/views.py` & `django-erp-framework-1.5.0/erp_framework/utils/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.12/setup.cfg` & `django-erp-framework-1.5.0/setup.cfg`

 * *Files identical despite different names*

