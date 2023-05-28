# Comparing `tmp/django_dynamic_storage-0.1.1.tar.gz` & `tmp/django_dynamic_storage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_storage-0.1.1.tar", max compression
+gzip compressed data, was "django_dynamic_storage-0.1.2.tar", max compression
```

## Comparing `django_dynamic_storage-0.1.1.tar` & `django_dynamic_storage-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.1/dynamic_storage/__init__.py
--rw-r--r--   0        0        0     5417 2023-05-24 14:39:21.785616 django_dynamic_storage-0.1.1/dynamic_storage/models.py
--rw-r--r--   0        0        0      125 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.1/dynamic_storage/signals.py
--rw-r--r--   0        0        0     1167 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.1/dynamic_storage/storage.py
--rw-r--r--   0        0        0      416 2023-05-24 15:19:49.710288 django_dynamic_storage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.2/dynamic_storage/__init__.py
+-rw-r--r--   0        0        0     5566 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/models.py
+-rw-r--r--   0        0        0      125 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.2/dynamic_storage/signals.py
+-rw-r--r--   0        0        0     1457 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/storage.py
+-rw-r--r--   0        0        0     1099 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/test/storage.py
+-rw-r--r--   0        0        0      908 2023-05-28 07:17:22.939947 django_dynamic_storage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      750 2023-05-28 07:17:11.462564 django_dynamic_storage-0.1.2/README.md
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.2/PKG-INFO
```

### Comparing `django_dynamic_storage-0.1.1/dynamic_storage/models.py` & `django_dynamic_storage-0.1.2/dynamic_storage/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import Any, Dict
 
+import django
 from django.db import models
 from django.db.models.fields.files import (
     FieldFile,
     FileDescriptor,
     ImageField,
     ImageFieldFile,
     ImageFileDescriptor,
 )
 
 from .signals import pre_dynamic_file_save
 from .storage import DynamicStorage, prob
 
 
+if django.VERSION >= (3, 1):
+    from django.db.models import JSONField
+else:
+    from django.contrib.postgres.fields import JSONField
+
 # {"name": str, "storage": prob}
 jsonfield = Dict[str, Any]
 
 
 class DynamicFieldFile(FieldFile):
     def __init__(self, instance, field, name, storage: DynamicStorage = None):
         super(DynamicFieldFile, self).__init__(instance, field, name)
@@ -96,15 +102,15 @@
                 instance, self.field, file.get("name"), storage
             )
             instance.__dict__[self.field.attname] = attr
 
         return instance.__dict__[self.field.attname]
 
 
-class DynamicFileField(models.JSONField, models.FileField):
+class DynamicFileField(JSONField, models.FileField):
     """FileField with json db representation that contain info for dynamic behavior"""
 
     attr_class = DynamicFieldFile
 
     descriptor_class = DynamicFileDescriptor
 
     def get_db_prep_value(self, value, connection, prepared=False):
```

### Comparing `django_dynamic_storage-0.1.1/dynamic_storage/storage.py` & `django_dynamic_storage-0.1.2/dynamic_storage/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 class DynamicStorageMixin(ABC):
     @abstractmethod
     def init_params(self) -> dict:
         """parameters for calling __init__ on storage class"""
         ...
 
+    def __eq__(self, other) -> bool:
+        """
+        how to differentiate two instances of the same storage class
+        Override this for your use case,
+        for example add the comparison based on bucket names
+        """
+        return self.__class__ == other.__class__
+
     def uninit(self) -> prob:
         """get the required properties for future initialization"""
         return {
             "import_path": f"{self.__class__.__module__}.{self.__class__.__qualname__}",
             "constructor": self.init_params(),
         }
```

