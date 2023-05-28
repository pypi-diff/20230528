# Comparing `tmp/django-bulk-tracker-0.0.5.tar.gz` & `tmp/django-bulk-tracker-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulk-tracker-0.0.5.tar", last modified: Tue Mar  7 17:21:28 2023, max compression
+gzip compressed data, was "django-bulk-tracker-0.0.6.tar", last modified: Sun May 28 12:32:30 2023, max compression
```

## Comparing `django-bulk-tracker-0.0.5.tar` & `django-bulk-tracker-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-07 17:21:28.567025 django-bulk-tracker-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/bulk_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/helper_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/bulk_tracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-07 17:21:28.000000 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-07 17:21:28.000000 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 17:21:28.000000 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-07 17:21:28.000000 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-07 17:21:28.000000 django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-07 17:21:28.567025 django-bulk-tracker-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:28.563025 django-bulk-tracker-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/test_create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/test_delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-03-07 17:21:18.000000 django-bulk-tracker-0.0.5/tests/test_update_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.561239 django-bulk-tracker-0.0.6/bulk_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/helper_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_update_signal.py
```

### Comparing `django-bulk-tracker-0.0.5/PKG-INFO` & `django-bulk-tracker-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
```

### Comparing `django-bulk-tracker-0.0.5/README.md` & `django-bulk-tracker-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/bulk_tracker/helper_objects.py` & `django-bulk-tracker-0.0.6/bulk_tracker/helper_objects.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/bulk_tracker/managers.py` & `django-bulk-tracker-0.0.6/bulk_tracker/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,9 @@
             return super().delete()
         objs = (obj for obj in self)
         result = super().delete()
         send_post_delete_signal(objs, self.model, tracking_info_)
         return result
 
 
-class BulkTrackerManager(Manager):
+class BulkTrackerManager(Manager.from_queryset(BulkTrackerQuerySet)):
     pass
```

### Comparing `django-bulk-tracker-0.0.5/bulk_tracker/models.py` & `django-bulk-tracker-0.0.6/bulk_tracker/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 from django.db import models
 from model_utils import FieldTracker
 
 from bulk_tracker.helper_objects import TrackingInfo
+from bulk_tracker.managers import BulkTrackerManager
 from bulk_tracker.signals import (
     send_post_create_signal,
     send_post_delete_signal,
     send_post_update_signal,
 )
 
 
 class BulkTrackerModel(models.Model):
+    objects = BulkTrackerManager()
     tracker: FieldTracker
 
     class Meta:
         abstract = True
 
     def _save_table(self, *args, **kwargs):
         updated = super()._save_table(*args, **kwargs)
```

### Comparing `django-bulk-tracker-0.0.5/bulk_tracker/signals.py` & `django-bulk-tracker-0.0.6/bulk_tracker/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 ):
     do_stuff()
 """
 post_update_signal = Signal()  # custom signal for bulk and single update
 
 
 """
-# @receiver(post_create_signal, sender=MyModel)
-# def i_am_a_receiver_function(
-#     sender,
-#     objects: list[ModifiedObject[MyModel]],
-#     tracking_info_: TrackingInfo | None = None,
-#     **kwargs,
-# ):
-#     do_stuff()
+@receiver(post_create_signal, sender=MyModel)
+def i_am_a_receiver_function(
+    sender,
+    objects: list[ModifiedObject[MyModel]],
+    tracking_info_: TrackingInfo | None = None,
+    **kwargs,
+):
+    do_stuff()
 """
 post_create_signal = Signal()  # custom signal for bulk and single create
 
 """
-# @receiver(post_delete_signal, sender=MyModel)
-# def i_am_a_receiver_function(
-#     sender,
-#     objects: list[ModifiedObject[MyModel]],
-#     tracking_info_: TrackingInfo | None = None,
-#     **kwargs,
-# ):
-#     do_stuff()
+@receiver(post_delete_signal, sender=MyModel)
+def i_am_a_receiver_function(
+    sender,
+    objects: list[ModifiedObject[MyModel]],
+    tracking_info_: TrackingInfo | None = None,
+    **kwargs,
+):
+    do_stuff()
 """
 post_delete_signal = Signal()  # custom signal for bulk and single delete
 
 
 def send_post_create_signal(
     objs: Iterable[BulkTrackerModel], model: type[BulkTrackerModel], tracking_info_: TrackingInfo | None = None
 ):
```

### Comparing `django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/PKG-INFO` & `django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
```

### Comparing `django-bulk-tracker-0.0.5/django_bulk_tracker.egg-info/SOURCES.txt` & `django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/usage.rst
 tests/__init__.py
-tests/managers.py
 tests/models.py
 tests/settings.py
 tests/test_create_signal.py
 tests/test_delete_signal.py
 tests/test_update_signal.py
```

### Comparing `django-bulk-tracker-0.0.5/docs/Makefile` & `django-bulk-tracker-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/docs/make.bat` & `django-bulk-tracker-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/docs/source/conf.py` & `django-bulk-tracker-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/docs/source/index.rst` & `django-bulk-tracker-0.0.6/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 django-bulk-tracker documentation
 =================================
 django-bulk-tracker is a reusable app for Django that allow you to have signals (``post_update_signal`` and ``post_create_signal``)
 that will be sent with your bulk operations.
 i.e. ``bulk_update()``, ``bulk_create()``, ``queryset.update()``.
 
-django-bulk-tracker allows you to pass tracking date related to your save/create operation.
+django-bulk-tracker allows you to pass tracking data related to your save/create operation.
 a feature that is missing from django builtin ``post_save`` signal.
 
 You can use ``post_update_signal`` and ``post_create_signal`` and ``tracking_info`` to stop relying
 on ``post_save`` method that force you to use ``.save()`` method.
 which is a bottleneck for a lot of django projects.
 
 django-bulk-tracker will send
```

### Comparing `django-bulk-tracker-0.0.5/docs/source/installation.rst` & `django-bulk-tracker-0.0.6/docs/source/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Installation
 ============
 
-Installing django-bulk-tracker is simple and straightforward. First of all, you need a copy of Auditlog on your system. The easiest
+Installing django-bulk-tracker is simple and straightforward. First of all, you need a copy of ``django-bulk-tracker`` on your system. The easiest
 way to do this is by using the Python Package Index (PyPI). Simply run the following command:
 
 ``pip install django-bulk-tracker``
 
-Instead of installing Auditlog via PyPI, you can also clone the Git repository or download the source code via GitHub.
+Instead of installing ``django-bulk-tracker`` via PyPI, you can also clone the Git repository or download the source code via GitHub.
 The repository can be found at https://github.com/hassaanalansary/django-bulk-tracker/.
 
 **Requirements**
 
 - Python 3.9 or higher
 - Django 3.2 or higher
 
-Auditlog is currently tested with Python 3.9+ and Django 3.2 and 4.0+.
+``django-bulk-tracker`` is currently tested with Python 3.9+ and Django 3.2 and 4.0+.
 
 Adding django-bulk-tracker to your Django application
 -----------------------------------------------------
 
 To use django-bulk-tracker in your application, just add ``'bulk-tracker'`` to your project's ``INSTALLED_APPS`` ``settings.py``
```

### Comparing `django-bulk-tracker-0.0.5/docs/source/usage.rst` & `django-bulk-tracker-0.0.6/docs/source/usage.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,44 @@
 
 and single operations:
 
 - ``create()``
 - ``save() # update and create``
 - ``delete()``
 
-all you need to do is to define your queryset and inherit from::
+all you need to do is to define your Model and inherit from::
+
+    from bulk_tracker.models import BulkTrackerModel
+
+    class Author(BulkTrackerModel):
+    first_name = models.CharField(max_length=200)
+    last_name = models.CharField(max_length=200)
+
+OR if you have a custom queryset inherit from or Don't want to support single-operation::
 
     from bulk_tracker.managers import BulkTrackerQuerySet
 
     class MyModelQuerySet(BulkTrackerQuerySet):
-        pass
+        def do_something_custom(self):
+            pass
 
 
 now you can listen to the signals ``post_update_signal``, ``post_create_signal``, ``post_delete_signal``::
 
     @receiver(post_update_signal, sender=MyModel)
     def i_am_a_receiver_function(
         sender,
         objects: list[ModifiedObject[MyModel]],
         tracking_info_: TrackingInfo | None = None,
         **kwargs,
     ):
         do_stuff()
 
 .. hint:: 
-    all signal has the same signature for consistency, 
+    all signals have the same signature for consistency,
     and also in case you want to assign one function to listen to multiple signals
 
 
 ``ModifiedObject`` is a very simple object, it contains 2 attributes: 
 1- ``instance`` this is your model instance after it has been updated, or created
 2- ``changed_values`` is dict[str, Any] which contains the changed fields only in case of ``post_update_signal``,
 in case of ``post_create_signal`` and ``post_delete_signal``, ``changed_values`` will be an empty dict ``{}``
@@ -109,22 +118,22 @@
 
         objects = MyModelManager()
         tracker = FieldTracker()
 
 ::
 
     # managers.py
-    from bulk_tracker.managers import BulkTrackerQuerySet
+    from bulk_tracker.managers import BulkTrackerQuerySet # optional
 
 
     class MyModelQuerySet(BulkTrackerQuerySet):
         pass
 
 
-    class MyModelManager(BulkTrackerManager.from_queryset(MyModelQuerySet)):
+    class MyModelManager(BulkTrackerManager.from_queryset(MyModelQuerySet)): # optional
         pass
 
 ::
 
     # signal_handlers.py
     from bulk_tracker.signals import post_update_signal
     from bulk_tracker.helper_objects import ModifiedObject, TrackingInfo
```

### Comparing `django-bulk-tracker-0.0.5/setup.cfg` & `django-bulk-tracker-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/tests/test_create_signal.py` & `django-bulk-tracker-0.0.6/tests/test_create_signal.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/tests/test_delete_signal.py` & `django-bulk-tracker-0.0.6/tests/test_delete_signal.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.5/tests/test_update_signal.py` & `django-bulk-tracker-0.0.6/tests/test_update_signal.py`

 * *Files identical despite different names*

