# Comparing `tmp/django-precise-bbcode-1.2.8.tar.gz` & `tmp/django-precise-bbcode-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-precise-bbcode-1.2.8.tar", last modified: Tue Apr  4 23:00:38 2017, max compression
+gzip compressed data, was "dist/django-precise-bbcode-1.2.9.tar", last modified: Sat Dec 16 18:27:55 2017, max compression
```

## Comparing `django-precise-bbcode-1.2.8.tar` & `django-precise-bbcode-1.2.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/
--rw-r--r--   0 morgano   (1000) morgano   (1000)     1649 2017-04-04 22:59:21.000000 django-precise-bbcode-1.2.8/setup.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     1493 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/LICENSE
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/
--rw-r--r--   0 morgano   (1000) morgano   (1000)     1354 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/SOURCES.txt
--rw-r--r--   0 morgano   (1000) morgano   (1000)       26 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/requires.txt
--rw-r--r--   0 morgano   (1000) morgano   (1000)        1 2017-03-26 16:53:16.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/not-zip-safe
--rw-r--r--   0 morgano   (1000) morgano   (1000)       15 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/top_level.txt
--rw-r--r--   0 morgano   (1000) morgano   (1000)     5832 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/PKG-INFO
--rw-r--r--   0 morgano   (1000) morgano   (1000)        1 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/dependency_links.txt
--rw-r--r--   0 morgano   (1000) morgano   (1000)     3996 2017-04-04 23:00:01.000000 django-precise-bbcode-1.2.8/README.rst
--rw-r--r--   0 morgano   (1000) morgano   (1000)      118 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/MANIFEST.in
--rw-r--r--   0 morgano   (1000) morgano   (1000)      335 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/setup.cfg
--rw-r--r--   0 morgano   (1000) morgano   (1000)     5832 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/PKG-INFO
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/
--rw-r--r--   0 morgano   (1000) morgano   (1000)     2436 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/placeholder_pool.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      580 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/jinja2tags.py
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/defaults/
--rw-r--r--   0 morgano   (1000) morgano   (1000)        0 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/defaults/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     2084 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/defaults/placeholder.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     3233 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/defaults/tag.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     4192 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     3769 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/placeholder.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)    18050 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/parser.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      280 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/exceptions.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      874 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/regexes.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)    10179 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/bbcode/tag.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     9313 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/models.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     2555 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/tag_pool.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      155 2017-04-04 22:59:43.000000 django-precise-bbcode-1.2.8/precise_bbcode/__init__.py
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/locale/
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/LC_MESSAGES/
--rw-r--r--   0 morgano   (1000) morgano   (1000)     5006 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 morgano   (1000) morgano   (1000)     5915 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/conf/
--rw-r--r--   0 morgano   (1000) morgano   (1000)        0 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/conf/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      990 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/conf/settings.py
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/migrations/
--rw-r--r--   0 morgano   (1000) morgano   (1000)        0 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/migrations/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     4147 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/migrations/0001_initial.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      258 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/shortcuts.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     1944 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/admin.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     5969 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/fields.py
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/templatetags/
--rw-r--r--   0 morgano   (1000) morgano   (1000)        0 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/templatetags/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     2608 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/templatetags/bbcode_tags.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      207 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/apps.py
-drwxr-xr-x   0 morgano   (1000) morgano   (1000)        0 2017-04-04 23:00:38.000000 django-precise-bbcode-1.2.8/precise_bbcode/core/
--rw-r--r--   0 morgano   (1000) morgano   (1000)      503 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/core/compat.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)        0 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/core/__init__.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)     1106 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/core/loading.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      387 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/core/utils.py
--rw-r--r--   0 morgano   (1000) morgano   (1000)      567 2017-03-26 15:45:03.000000 django-precise-bbcode-1.2.8/precise_bbcode/test.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/
+-rw-r--r--   0 morgano    (501) staff       (20)     5867 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/PKG-INFO
+-rw-r--r--   0 morgano    (501) staff       (20)     1493 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/LICENSE
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/
+-rw-r--r--   0 morgano    (501) staff       (20)     5867 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/PKG-INFO
+-rw-r--r--   0 morgano    (501) staff       (20)        1 2017-10-09 14:53:51.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/not-zip-safe
+-rw-r--r--   0 morgano    (501) staff       (20)     1354 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/SOURCES.txt
+-rw-r--r--   0 morgano    (501) staff       (20)       27 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/requires.txt
+-rw-r--r--   0 morgano    (501) staff       (20)       15 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/top_level.txt
+-rw-r--r--   0 morgano    (501) staff       (20)        1 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/dependency_links.txt
+-rw-r--r--   0 morgano    (501) staff       (20)      118 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/MANIFEST.in
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/templatetags/
+-rw-r--r--   0 morgano    (501) staff       (20)        0 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/templatetags/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)     2608 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/templatetags/bbcode_tags.py
+-rw-r--r--   0 morgano    (501) staff       (20)     2555 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/tag_pool.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/migrations/
+-rw-r--r--   0 morgano    (501) staff       (20)        0 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/precise_bbcode/migrations/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)     4147 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/precise_bbcode/migrations/0001_initial.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/locale/
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 morgano    (501) staff       (20)     5006 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 morgano    (501) staff       (20)     5915 2017-04-30 23:13:15.000000 django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/core/
+-rw-r--r--   0 morgano    (501) staff       (20)     1107 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/core/loading.py
+-rw-r--r--   0 morgano    (501) staff       (20)      504 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/core/compat.py
+-rw-r--r--   0 morgano    (501) staff       (20)        0 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/core/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)      388 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/core/utils.py
+-rw-r--r--   0 morgano    (501) staff       (20)     9314 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/models.py
+-rw-r--r--   0 morgano    (501) staff       (20)     5971 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/fields.py
+-rw-r--r--   0 morgano    (501) staff       (20)      258 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/shortcuts.py
+-rw-r--r--   0 morgano    (501) staff       (20)      156 2017-12-16 18:27:12.000000 django-precise-bbcode-1.2.9/precise_bbcode/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)      567 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/test.py
+-rw-r--r--   0 morgano    (501) staff       (20)      207 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/apps.py
+-rw-r--r--   0 morgano    (501) staff       (20)      580 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/jinja2tags.py
+-rw-r--r--   0 morgano    (501) staff       (20)     1944 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/admin.py
+-rw-r--r--   0 morgano    (501) staff       (20)     2436 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/placeholder_pool.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/conf/
+-rw-r--r--   0 morgano    (501) staff       (20)        0 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/conf/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)      990 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/conf/settings.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/
+-rw-r--r--   0 morgano    (501) staff       (20)     3770 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/placeholder.py
+-rw-r--r--   0 morgano    (501) staff       (20)     4192 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)    18050 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/parser.py
+drwxr-xr-x   0 morgano    (501) staff       (20)        0 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/defaults/
+-rw-r--r--   0 morgano    (501) staff       (20)     2310 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/defaults/placeholder.py
+-rw-r--r--   0 morgano    (501) staff       (20)        0 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/defaults/__init__.py
+-rw-r--r--   0 morgano    (501) staff       (20)     3725 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/defaults/tag.py
+-rw-r--r--   0 morgano    (501) staff       (20)      875 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/regexes.py
+-rw-r--r--   0 morgano    (501) staff       (20)      280 2017-10-09 15:21:00.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/exceptions.py
+-rw-r--r--   0 morgano    (501) staff       (20)    10180 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/precise_bbcode/bbcode/tag.py
+-rw-r--r--   0 morgano    (501) staff       (20)     1651 2017-12-16 18:26:59.000000 django-precise-bbcode-1.2.9/setup.py
+-rw-r--r--   0 morgano    (501) staff       (20)      398 2017-12-16 18:27:55.000000 django-precise-bbcode-1.2.9/setup.cfg
+-rw-r--r--   0 morgano    (501) staff       (20)     3997 2017-12-16 18:27:38.000000 django-precise-bbcode-1.2.9/README.rst
```

### Comparing `django-precise-bbcode-1.2.8/setup.py` & `django-precise-bbcode-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import codecs
 from os.path import abspath
 from os.path import dirname
 from os.path import join
+
 from setuptools import find_packages
 from setuptools import setup
 
 import precise_bbcode
 
 
 def read_relative_file(filename):
@@ -28,15 +29,15 @@
     include_package_data=True,
     url='https://github.com/ellmetha/django-precise-bbcode',
     license='BSD',
     description='A django BBCode integration..',
     long_description=read_relative_file('README.rst'),
     zip_safe=False,
     install_requires=[
-        'django>=1.8',
+        'django>=1.11',
         'pillow>=2.2.1',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
```

### Comparing `django-precise-bbcode-1.2.8/LICENSE` & `django-precise-bbcode-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/SOURCES.txt` & `django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/django_precise_bbcode.egg-info/PKG-INFO` & `django-precise-bbcode-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: django-precise-bbcode
-Version: 1.2.8
+Version: 1.2.9
 Summary: A django BBCode integration..
 Home-page: https://github.com/ellmetha/django-precise-bbcode
 Author: Morgan Aubert
 Author-email: morgan.aubert@zoho.com
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: =====================
         django-precise-bbcode
         =====================
         
         *Django-precise-bbcode* is a Django application providing a way to create textual contents based on BBCodes.
         
           BBCode is a special implementation of HTML. BBCode itself is similar in style to HTML, tags are enclosed in square brackets [ and ] rather than < and > and it offers greater control over what and how something is displayed.
@@ -28,16 +29,16 @@
         
         Online browsable documentation is available at https://django-precise-bbcode.readthedocs.org.
         
         
         Requirements
         ------------
         
-        * Python 2.7+ or 3.3+
-        * Django 1.8+
+        * Python 2.7+ or 3.4+
+        * Django 1.11+
         * PIL or Pillow (required for smiley tags)
         
         Installation
         ------------
         
         Just run:
```

### Comparing `django-precise-bbcode-1.2.8/README.rst` & `django-precise-bbcode-1.2.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 Online browsable documentation is available at https://django-precise-bbcode.readthedocs.org.
 
 
 Requirements
 ------------
 
-* Python 2.7+ or 3.3+
-* Django 1.8+
+* Python 2.7+ or 3.4+
+* Django 1.11+
 * PIL or Pillow (required for smiley tags)
 
 Installation
 ------------
 
 Just run:
```

### Comparing `django-precise-bbcode-1.2.8/PKG-INFO` & `django-precise-bbcode-1.2.9/django_precise_bbcode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: django-precise-bbcode
-Version: 1.2.8
+Version: 1.2.9
 Summary: A django BBCode integration..
 Home-page: https://github.com/ellmetha/django-precise-bbcode
 Author: Morgan Aubert
 Author-email: morgan.aubert@zoho.com
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: =====================
         django-precise-bbcode
         =====================
         
         *Django-precise-bbcode* is a Django application providing a way to create textual contents based on BBCodes.
         
           BBCode is a special implementation of HTML. BBCode itself is similar in style to HTML, tags are enclosed in square brackets [ and ] rather than < and > and it offers greater control over what and how something is displayed.
@@ -28,16 +29,16 @@
         
         Online browsable documentation is available at https://django-precise-bbcode.readthedocs.org.
         
         
         Requirements
         ------------
         
-        * Python 2.7+ or 3.3+
-        * Django 1.8+
+        * Python 2.7+ or 3.4+
+        * Django 1.11+
         * PIL or Pillow (required for smiley tags)
         
         Installation
         ------------
         
         Just run:
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/placeholder_pool.py` & `django-precise-bbcode-1.2.9/precise_bbcode/placeholder_pool.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/jinja2tags.py` & `django-precise-bbcode-1.2.9/precise_bbcode/jinja2tags.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/defaults/tag.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/defaults/tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import re
 
+from django.core.exceptions import ValidationError
+from django.core.validators import URLValidator
+
 from precise_bbcode.bbcode.tag import BBCodeTag
 from precise_bbcode.conf import settings as bbcode_settings
 from precise_bbcode.core.utils import replace
 
 
 class StrongBBCodeTag(BBCodeTag):
     name = 'b'
@@ -100,20 +104,32 @@
 
     _domain_re = re.compile(r'^(?=.{4,255}$)([a-zA-Z0-9][a-zA-Z0-9-]{,61}[a-zA-Z0-9]\.)+[a-zA-Z0-9]{2,5}$')  # noqa
 
     class Options:
         replace_links = False
 
     def render(self, value, option=None, parent=None):
-        href = replace(option, bbcode_settings.BBCODE_ESCAPE_HTML) if option else value
+        href = option if option else value
+        href = replace(href, bbcode_settings.BBCODE_ESCAPE_HTML)
+        value = replace(value, bbcode_settings.BBCODE_ESCAPE_HTML)
         if '://' not in href and self._domain_re.match(href):
             href = 'http://' + href
-        content = value if option else href
-        # Render
-        return '<a href="{}">{}</a>'.format(href, content or href)
+        v = URLValidator()
+
+        # Validates and renders the considered URL.
+        try:
+            v(href)
+        except ValidationError:
+            rendered = '[url={}]{}[/url]'.format(href, value) if option else \
+                '[url]{}[/url]'.format(value)
+        else:
+            content = value if option else href
+            rendered = '<a href="{}">{}</a>'.format(href, content or href)
+
+        return rendered
 
 
 class ImgBBCodeTag(BBCodeTag):
     name = 'img'
     definition_string = '[img]{URL}[/img]'
     format_string = '<img src="{URL}" alt="" />'
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/__init__.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/__init__.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/placeholder.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/placeholder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import re
 
 from precise_bbcode.bbcode.exceptions import InvalidBBCodePlaholder
 from precise_bbcode.core.compat import with_metaclass
 
 
 class BBCodePlaceholderBase(type):
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/parser.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/parser.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/regexes.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/regexes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import re
 
 
 # Common regexes
 url_re = re.compile(r'(?im)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\([^\s()<>]+\))+(?:\([^\s()<>]+\)|[^\s`!()\[\]{};:\'".,<>?]))')  # noqa
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/bbcode/tag.py` & `django-precise-bbcode-1.2.9/precise_bbcode/bbcode/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import inspect
 import re
 
 from precise_bbcode.bbcode.exceptions import InvalidBBCodePlaholder
 from precise_bbcode.bbcode.exceptions import InvalidBBCodeTag
 from precise_bbcode.bbcode.regexes import bbcodde_standalone_re
 from precise_bbcode.bbcode.regexes import bbcodde_standard_re
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/models.py` & `django-precise-bbcode-1.2.9/precise_bbcode/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import re
 
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.encoding import force_str
 from django.utils.encoding import python_2_unicode_compatible
 from django.utils.translation import ugettext_lazy as _
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/tag_pool.py` & `django-precise-bbcode-1.2.9/precise_bbcode/tag_pool.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/LC_MESSAGES/django.mo` & `django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/locale/fr/LC_MESSAGES/django.po` & `django-precise-bbcode-1.2.9/precise_bbcode/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/conf/settings.py` & `django-precise-bbcode-1.2.9/precise_bbcode/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/migrations/0001_initial.py` & `django-precise-bbcode-1.2.9/precise_bbcode/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/admin.py` & `django-precise-bbcode-1.2.9/precise_bbcode/admin.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/fields.py` & `django-precise-bbcode-1.2.9/precise_bbcode/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import re
 
 from django.core.validators import RegexValidator
 from django.db import models
 from django.db.models import signals
 from django.utils.encoding import python_2_unicode_compatible
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
 from .bbcode import get_parser
 
+
 __all__ = (
     'BBCodeContent',
     'BBCodeTextField',
     'SmileyCodeField',
 )
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/templatetags/bbcode_tags.py` & `django-precise-bbcode-1.2.9/precise_bbcode/templatetags/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/core/loading.py` & `django-precise-bbcode-1.2.9/precise_bbcode/core/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals
+
 import imp
 import importlib
 import inspect
 
 from django.apps import apps
```

### Comparing `django-precise-bbcode-1.2.8/precise_bbcode/test.py` & `django-precise-bbcode-1.2.9/precise_bbcode/test.py`

 * *Files identical despite different names*

