# Comparing `tmp/django_dynamic_storage-0.1.2.tar.gz` & `tmp/django_dynamic_storage-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_storage-0.1.2.tar", max compression
+gzip compressed data, was "django_dynamic_storage-0.1.3.tar", max compression
```

## Comparing `django_dynamic_storage-0.1.2.tar` & `django_dynamic_storage-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.2/dynamic_storage/__init__.py
--rw-r--r--   0        0        0     5566 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/models.py
--rw-r--r--   0        0        0      125 2023-05-24 14:13:36.738915 django_dynamic_storage-0.1.2/dynamic_storage/signals.py
--rw-r--r--   0        0        0     1457 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/storage.py
--rw-r--r--   0        0        0     1099 2023-05-28 06:12:33.888183 django_dynamic_storage-0.1.2/dynamic_storage/test/storage.py
--rw-r--r--   0        0        0      908 2023-05-28 07:17:22.939947 django_dynamic_storage-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      750 2023-05-28 07:17:11.462564 django_dynamic_storage-0.1.2/README.md
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      717 2023-05-28 14:44:04.879858 django_dynamic_storage-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 14:44:04.879858 django_dynamic_storage-0.1.3/dynamic_storage/__init__.py
+-rw-r--r--   0        0        0     5418 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/models.py
+-rw-r--r--   0        0        0      120 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/signals.py
+-rw-r--r--   0        0        0     1410 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/storage.py
+-rw-r--r--   0        0        0     1064 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/test/storage.py
+-rw-r--r--   0        0        0      745 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.3/PKG-INFO
```

### Comparing `django_dynamic_storage-0.1.2/dynamic_storage/models.py` & `django_dynamic_storage-0.1.3/dynamic_storage/models.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-from typing import Any, Dict
-
-import django
-from django.db import models
-from django.db.models.fields.files import (
-    FieldFile,
-    FileDescriptor,
-    ImageField,
-    ImageFieldFile,
-    ImageFileDescriptor,
-)
-
-from .signals import pre_dynamic_file_save
-from .storage import DynamicStorage, prob
-
-
-if django.VERSION >= (3, 1):
-    from django.db.models import JSONField
-else:
-    from django.contrib.postgres.fields import JSONField
-
-# {"name": str, "storage": prob}
-jsonfield = Dict[str, Any]
-
-
-class DynamicFieldFile(FieldFile):
-    def __init__(self, instance, field, name, storage: DynamicStorage = None):
-        super(DynamicFieldFile, self).__init__(instance, field, name)
-        self._current_storage = (
-            storage  # keep track of the storage the file is actually at
-        )
-        self.storage = storage or self.storage
-
-        # To be able to save the file to the appropriate storage
-        # if providing the save() method with storage argument is not possible
-        self.destination_storage = None
-
-    def dictionary(self) -> jsonfield:
-        """Value to be stored in JSONField"""
-        return {"name": str(self), "storage": self.storage.uninit()}
-
-    def save(self, name, content, /, storage: DynamicStorage = None, save=True):
-        """
-        This is the dynamic storage save
-        """
-        self.destination_storage = storage or self.destination_storage
-        # Ensure we are not trying to move obj between storages (yet)
-        assert (
-            self._current_storage == self.destination_storage
-            if self._current_storage
-            else True
-        )
-
-        pre_dynamic_file_save.send(
-            sender=self.instance.__class__,
-            instance=self.instance,
-            field_file=self,
-            to_storage=self.destination_storage,
-        )
-
-        storage = self.destination_storage or self._current_storage or self.storage
-
-        name = self.field.generate_filename(self.instance, name)
-        self.name = storage.save(name, content, max_length=self.field.max_length)
-        self.storage = self._current_storage = self.destination_storage = storage
-
-        # This is the replacement for 'setattr(self.instance, self.field.attname, self.name)'
-        # because instance is not wrote to db yet, reinstantiating will break setting the right storage
-        getattr(self.instance, self.field.attname).name = self.name
-
-        self._committed = True
-
-        # Save the object because it has changed, unless save is False
-        if save:
-            self.instance.save()
-
-    def __getstate__(self):
-        # Don't know how to get the state related to storage
-        raise NotImplementedError
-
-    def __setstate__(self, state):
-        # __getstate__ is not implemented
-        raise NotImplementedError
-
-
-class DynamicFileDescriptor(FileDescriptor):
-    def __get__(self, instance, cls=None):
-        file = super(DynamicFileDescriptor, self).__get__(instance, cls=cls)
-        # If this value is a dictionary (instance.file = {"name": "path/to/file", **kw}) or {}
-        # then we simply wrap it with the appropriate attribute class according
-        # to the file field. [This is DynamicFieldFile for DynamicFileField and
-        # ImageFieldFile for ImageFields; it's also conceivable that user
-        # subclasses might also want to subclass the attribute class]. This
-        # object understands how to convert a jsonfield to a file, and also how to
-        # handle dict().
-        if isinstance(file, dict):
-            storage_prob: prob = file.get("storage")
-            storage = (
-                DynamicStorage.init(storage_prob) if storage_prob else storage_prob
-            )
-            attr = self.field.attr_class(
-                instance, self.field, file.get("name"), storage
-            )
-            instance.__dict__[self.field.attname] = attr
-
-        return instance.__dict__[self.field.attname]
-
-
-class DynamicFileField(JSONField, models.FileField):
-    """FileField with json db representation that contain info for dynamic behavior"""
-
-    attr_class = DynamicFieldFile
-
-    descriptor_class = DynamicFileDescriptor
-
-    def get_db_prep_value(self, value, connection, prepared=False):
-        if value is None:
-            return value
-        if not isinstance(value, dict):
-            value = value.dictionary()
-        return super(DynamicFileField, self).get_db_prep_value(
-            value, connection, prepared
-        )
-
-    def formfield(self, **kwargs):
-        return models.FileField.formfield(self, **kwargs)
-
-    def validate(self, value, model_instance):
-        super(DynamicFileField, self).validate(value.dictionary(), model_instance)
-
-
-class DynamicImageFieldFile(ImageFieldFile, DynamicFieldFile):
-    def save(self, *args, **kwargs):
-        super(DynamicImageFieldFile, self).save(*args, **kwargs)
-        # Since reinstantiating the FieldFile after calling save() is not the case anymore
-        # (due to delete 'setattr(self.instance, self.field.attname, self.name)')
-        self.field.update_dimension_fields(self.instance, force=True)
-
-
-class DynamicImageFileDescriptor(ImageFileDescriptor, DynamicFileDescriptor):
-    pass
-
-
-class DynamicImageField(ImageField, DynamicFileField):
-    """ImageField with json db representation that contain info for dynamic behavior"""
-
-    attr_class = DynamicImageFieldFile
-    descriptor_class = DynamicImageFileDescriptor
+from typing import Any, Dict
+
+import django
+from django.db import models
+from django.db.models.fields.files import (
+    FieldFile,
+    FileDescriptor,
+    ImageField,
+    ImageFieldFile,
+    ImageFileDescriptor,
+)
+
+from .signals import pre_dynamic_file_save
+from .storage import DynamicStorage, prob
+
+
+if django.VERSION >= (3, 1):
+    from django.db.models import JSONField
+else:
+    from django.contrib.postgres.fields import JSONField
+
+# {"name": str, "storage": prob}
+jsonfield = Dict[str, Any]
+
+
+class DynamicFieldFile(FieldFile):
+    def __init__(self, instance, field, name, storage: DynamicStorage = None):
+        super(DynamicFieldFile, self).__init__(instance, field, name)
+        self._current_storage = (
+            storage  # keep track of the storage the file is actually at
+        )
+        self.storage = storage or self.storage
+
+        # To be able to save the file to the appropriate storage
+        # if providing the save() method with storage argument is not possible
+        self.destination_storage = None
+
+    def dictionary(self) -> jsonfield:
+        """Value to be stored in JSONField"""
+        return {"name": str(self), "storage": self.storage.uninit()}
+
+    def save(self, name, content, /, storage: DynamicStorage = None, save=True):
+        """
+        This is the dynamic storage save
+        """
+        self.destination_storage = storage or self.destination_storage
+        # Ensure we are not trying to move obj between storages (yet)
+        assert (
+            self._current_storage == self.destination_storage
+            if self._current_storage
+            else True
+        )
+
+        pre_dynamic_file_save.send(
+            sender=self.instance.__class__,
+            instance=self.instance,
+            field_file=self,
+            to_storage=self.destination_storage,
+        )
+
+        storage = self.destination_storage or self._current_storage or self.storage
+
+        name = self.field.generate_filename(self.instance, name)
+        self.name = storage.save(name, content, max_length=self.field.max_length)
+        self.storage = self._current_storage = self.destination_storage = storage
+
+        # This is the replacement for 'setattr(self.instance, self.field.attname, self.name)'
+        # because instance is not wrote to db yet, reinstantiating will break setting the right storage
+        getattr(self.instance, self.field.attname).name = self.name
+
+        self._committed = True
+
+        # Save the object because it has changed, unless save is False
+        if save:
+            self.instance.save()
+
+    def __getstate__(self):
+        # Don't know how to get the state related to storage
+        raise NotImplementedError
+
+    def __setstate__(self, state):
+        # __getstate__ is not implemented
+        raise NotImplementedError
+
+
+class DynamicFileDescriptor(FileDescriptor):
+    def __get__(self, instance, cls=None):
+        file = super(DynamicFileDescriptor, self).__get__(instance, cls=cls)
+        # If this value is a dictionary (instance.file = {"name": "path/to/file", **kw}) or {}
+        # then we simply wrap it with the appropriate attribute class according
+        # to the file field. [This is DynamicFieldFile for DynamicFileField and
+        # ImageFieldFile for ImageFields; it's also conceivable that user
+        # subclasses might also want to subclass the attribute class]. This
+        # object understands how to convert a jsonfield to a file, and also how to
+        # handle dict().
+        if isinstance(file, dict):
+            storage_prob: prob = file.get("storage")
+            storage = (
+                DynamicStorage.init(storage_prob) if storage_prob else storage_prob
+            )
+            attr = self.field.attr_class(
+                instance, self.field, file.get("name"), storage
+            )
+            instance.__dict__[self.field.attname] = attr
+
+        return instance.__dict__[self.field.attname]
+
+
+class DynamicFileField(JSONField, models.FileField):
+    """FileField with json db representation that contain info for dynamic behavior"""
+
+    attr_class = DynamicFieldFile
+
+    descriptor_class = DynamicFileDescriptor
+
+    def get_db_prep_value(self, value, connection, prepared=False):
+        if value is None:
+            return value
+        if not isinstance(value, dict):
+            value = value.dictionary()
+        return super(DynamicFileField, self).get_db_prep_value(
+            value, connection, prepared
+        )
+
+    def formfield(self, **kwargs):
+        return models.FileField.formfield(self, **kwargs)
+
+    def validate(self, value, model_instance):
+        super(DynamicFileField, self).validate(value.dictionary(), model_instance)
+
+
+class DynamicImageFieldFile(ImageFieldFile, DynamicFieldFile):
+    def save(self, *args, **kwargs):
+        super(DynamicImageFieldFile, self).save(*args, **kwargs)
+        # Since reinstantiating the FieldFile after calling save() is not the case anymore
+        # (due to delete 'setattr(self.instance, self.field.attname, self.name)')
+        self.field.update_dimension_fields(self.instance, force=True)
+
+
+class DynamicImageFileDescriptor(ImageFileDescriptor, DynamicFileDescriptor):
+    pass
+
+
+class DynamicImageField(ImageField, DynamicFileField):
+    """ImageField with json db representation that contain info for dynamic behavior"""
+
+    attr_class = DynamicImageFieldFile
+    descriptor_class = DynamicImageFileDescriptor
```

### Comparing `django_dynamic_storage-0.1.2/dynamic_storage/storage.py` & `django_dynamic_storage-0.1.3/dynamic_storage/storage.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from __future__ import annotations
-
-import importlib
-from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict
-
-from django.core.files.storage import Storage
-
-
-# {"import_path": str, "constructor": dict}
-prob = Dict[str, Any]
-
-
-class DynamicStorageMixin(ABC):
-    @abstractmethod
-    def init_params(self) -> dict:
-        """parameters for calling __init__ on storage class"""
-        ...
-
-    def __eq__(self, other) -> bool:
-        """
-        how to differentiate two instances of the same storage class
-        Override this for your use case,
-        for example add the comparison based on bucket names
-        """
-        return self.__class__ == other.__class__
-
-    def uninit(self) -> prob:
-        """get the required properties for future initialization"""
-        return {
-            "import_path": f"{self.__class__.__module__}.{self.__class__.__qualname__}",
-            "constructor": self.init_params(),
-        }
-
-    @classmethod
-    def init(cls, probs: prob) -> DynamicStorageMixin:
-        """initialize storage"""
-        module_name = ".".join(probs["import_path"].split(".")[:-1])
-        class_name = probs["import_path"].split(".")[-1]
-        StorageClass: Callable = getattr(
-            importlib.import_module(module_name), class_name
-        )
-        return StorageClass(**probs["constructor"])
-
-
-class DynamicStorage(DynamicStorageMixin, Storage):
-    ...
+from __future__ import annotations
+
+import importlib
+from abc import ABC, abstractmethod
+from typing import Any, Callable, Dict
+
+from django.core.files.storage import Storage
+
+
+# {"import_path": str, "constructor": dict}
+prob = Dict[str, Any]
+
+
+class DynamicStorageMixin(ABC):
+    @abstractmethod
+    def init_params(self) -> dict:
+        """parameters for calling __init__ on storage class"""
+        ...
+
+    def __eq__(self, other) -> bool:
+        """
+        how to differentiate two instances of the same storage class
+        Override this for your use case,
+        for example add the comparison based on bucket names
+        """
+        return self.__class__ == other.__class__
+
+    def uninit(self) -> prob:
+        """get the required properties for future initialization"""
+        return {
+            "import_path": f"{self.__class__.__module__}.{self.__class__.__qualname__}",
+            "constructor": self.init_params(),
+        }
+
+    @classmethod
+    def init(cls, probs: prob) -> DynamicStorageMixin:
+        """initialize storage"""
+        module_name = ".".join(probs["import_path"].split(".")[:-1])
+        class_name = probs["import_path"].split(".")[-1]
+        StorageClass: Callable = getattr(
+            importlib.import_module(module_name), class_name
+        )
+        return StorageClass(**probs["constructor"])
+
+
+class DynamicStorage(DynamicStorageMixin, Storage):
+    ...
```

### Comparing `django_dynamic_storage-0.1.2/pyproject.toml` & `django_dynamic_storage-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-[tool.poetry]
-name = "django-dynamic-storage"
-version = "0.1.2"
-description = "Use and choose storages at runtime based on your logic"
-authors = ["Amir Khalife <eng.amir.bu@gmail.com>"]
-license = "Apache-2.0"
-readme = "README.md"
-packages = [{include = "dynamic_storage"}]
-
-[tool.poetry.dependencies]
-python = ">=3.7,<3.12"
-Django = ">=2.2,<5"
-
-[tool.poetry.group.test.dependencies]
-django-environ = "^0.10.0"
-pillow = "^9.5.0"
-pytest = "^7.3.1"
-pytest-django = "^4.5.2"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-django_find_project = false
-pythonpath = ". tests"
-DJANGO_SETTINGS_MODULE = "tests.settings"
-
-[tool.isort]
-known_first_party="django,pytest"
-known_apps="dynamic_storage"
-lines_after_imports=2
-profile = "black"
-py_version=39
-sections="FUTURE,STDLIB,FIRSTPARTY,THIRDPARTY,APPS,LOCALFOLDER"
+[tool.poetry]
+name = "django-dynamic-storage"
+version = "0.1.3"
+description = "Use and choose storages at runtime based on your logic"
+authors = ["Amir Khalife <eng.amir.bu@gmail.com>"]
+license = "Apache-2.0"
+readme = "README.md"
+packages = [{include = "dynamic_storage"}]
+
+[tool.poetry.dependencies]
+python = ">=3.7,<3.12"
+Django = ">=2.2,<5"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+django_find_project = false
+pythonpath = ". tests"
+DJANGO_SETTINGS_MODULE = "tests.settings"
+
+[tool.isort]
+known_first_party="django,pytest"
+known_apps="dynamic_storage"
+lines_after_imports=2
+profile = "black"
+py_version=39
+sections="FUTURE,STDLIB,FIRSTPARTY,THIRDPARTY,APPS,LOCALFOLDER"
```

### Comparing `django_dynamic_storage-0.1.2/README.md` & `django_dynamic_storage-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-![tox CI](https://github.com/engAmirEng/django-dynamic-storage/actions/workflows/tox.yml/badge.svg)
-![Python Versions](https://img.shields.io/pypi/pyversions/poetry)
-[![Django Versions](https://img.shields.io/pypi/djversions/django-silk.svg)](https://pypi.python.org/pypi/django-dynamic-storage)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/engAmirEng/django-dynamic-storage/main.svg)](https://results.pre-commit.ci/latest/github/engAmirEng/django-dynamic-storage/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![tox CI](https://github.com/engAmirEng/django-dynamic-storage/actions/workflows/tox.yml/badge.svg)
+![Python Versions](https://img.shields.io/pypi/pyversions/poetry)
+![Python Versionfs](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/engAmirEng/django-dynamic-storage/main.svg)](https://results.pre-commit.ci/latest/github/engAmirEng/django-dynamic-storage/main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

### Comparing `django_dynamic_storage-0.1.2/PKG-INFO` & `django_dynamic_storage-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-storage
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use and choose storages at runtime based on your logic
 License: Apache-2.0
 Author: Amir Khalife
 Author-email: eng.amir.bu@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,12 +14,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=2.2,<5)
 Description-Content-Type: text/markdown
 
 ![tox CI](https://github.com/engAmirEng/django-dynamic-storage/actions/workflows/tox.yml/badge.svg)
 ![Python Versions](https://img.shields.io/pypi/pyversions/poetry)
-[![Django Versions](https://img.shields.io/pypi/djversions/django-silk.svg)](https://pypi.python.org/pypi/django-dynamic-storage)
+![Python Versionfs](https://img.shields.io/badge/django-2.2_|_3.0_|_3.1_|_3.2_|_4.0_|_4.1_|_4.2-green)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/engAmirEng/django-dynamic-storage/main.svg)](https://results.pre-commit.ci/latest/github/engAmirEng/django-dynamic-storage/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

