# Comparing `tmp/django_batteries-0.0.1.tar.gz` & `tmp/django_batteries-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_batteries-0.0.1.tar", max compression
+gzip compressed data, was "django_batteries-0.0.2.tar", max compression
```

## Comparing `django_batteries-0.0.1.tar` & `django_batteries-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      770 2023-03-09 14:40:08.654809 django_batteries-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-07 15:00:49.862571 django_batteries-0.0.1/django_batteries/__init__.py
--rw-r--r--   0        0        0     3604 2023-03-09 14:32:56.643615 django_batteries-0.0.1/django_batteries/fields.py
--rw-r--r--   0        0        0     1792 2023-03-09 14:30:14.723884 django_batteries-0.0.1/django_batteries/models.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:07.778656 django_batteries-0.0.1/django_batteries/tests.py
--rw-r--r--   0        0        0     1223 2023-03-09 14:36:35.328377 django_batteries-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 django_batteries-0.0.1/setup.py
--rw-r--r--   0        0        0     1218 1970-01-01 00:00:00.000000 django_batteries-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1458 2023-05-28 15:25:15.518585 django_batteries-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-07 15:00:49.862571 django_batteries-0.0.2/django_batteries/__init__.py
+-rw-r--r--   0        0        0     3582 2023-05-28 15:01:54.342689 django_batteries-0.0.2/django_batteries/fields.py
+-rw-r--r--   0        0        0      737 2023-05-28 15:20:58.590927 django_batteries-0.0.2/django_batteries/mixins.py
+-rw-r--r--   0        0        0     2587 2023-05-28 15:09:04.235056 django_batteries-0.0.2/django_batteries/models.py
+-rw-r--r--   0        0        0      624 2023-05-28 15:24:15.216601 django_batteries-0.0.2/django_batteries/paginators.py
+-rw-r--r--   0        0        0        0 2023-05-28 15:07:36.572145 django_batteries-0.0.2/django_batteries/tests.py
+-rw-r--r--   0        0        0      658 2023-05-28 15:21:33.668904 django_batteries-0.0.2/django_batteries/utils.py
+-rw-r--r--   0        0        0     1277 2023-05-28 15:29:07.337997 django_batteries-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 django_batteries-0.0.2/setup.py
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 django_batteries-0.0.2/PKG-INFO
```

### Comparing `django_batteries-0.0.1/django_batteries/fields.py` & `django_batteries-0.0.2/django_batteries/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from django.utils.timezone import now
 from django.db import models
+from django.utils.timezone import now
 
 
 class AutoCreatedField(models.DateTimeField):
     """
     A DateTimeField that automatically populates itself at
     object creation.
     By default, sets editable=False, default=datetime.now.
@@ -52,24 +52,24 @@
     changes.
     """
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("default", now)
         monitor = kwargs.pop("monitor", None)
         if not monitor:
-            raise TypeError('%s requires a "monitor" argument' % self.__class__.__name__)
+            raise TypeError(f'{self.__class__.__name__} requires a "monitor" argument')
         self.monitor = monitor
         when = kwargs.pop("when", None)
         if when is not None:
             when = set(when)
         self.when = when
         super().__init__(*args, **kwargs)
 
     def contribute_to_class(self, cls, name):
-        self.monitor_attname = "_monitor_%s" % name
+        self.monitor_attname = f"_monitor_{name}"
         models.signals.post_init.connect(self._save_initial, sender=cls)
         super().contribute_to_class(cls, name)
 
     def get_monitored_value(self, instance):
         return getattr(instance, self.monitor)
 
     def _save_initial(self, sender, instance, **kwargs):
@@ -78,18 +78,17 @@
             return
         setattr(instance, self.monitor_attname, self.get_monitored_value(instance))
 
     def pre_save(self, model_instance, add):
         value = now()
         previous = getattr(model_instance, self.monitor_attname, None)
         current = self.get_monitored_value(model_instance)
-        if previous != current:
-            if self.when is None or current in self.when:
-                setattr(model_instance, self.attname, value)
-                self._save_initial(model_instance.__class__, model_instance)
+        if previous != current and (self.when is None or current in self.when):
+            setattr(model_instance, self.attname, value)
+            self._save_initial(model_instance.__class__, model_instance)
         return super().pre_save(model_instance, add)
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         kwargs["monitor"] = self.monitor
         if self.when is not None:
             kwargs["when"] = self.when
```

### Comparing `django_batteries-0.0.1/pyproject.toml` & `django_batteries-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 authors = ["Oleksandr Korol <zibertua@gmail.com>"]
 description = "Set of most common utils for django/drf projects"
 license = "MIT"
-name = "django_batteries"
+name = "django-batteries"
 packages = [{include = "django_batteries"}]
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 
 [tool.poetry.dependencies]
 django = "^4.1.7"
+djangorestframework = "^3.14.0"
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ruff = "^0.0.254"
+pre-commit = "^3.3.2"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 # Ruff settings
 [tool.ruff]
```

### Comparing `django_batteries-0.0.1/setup.py` & `django_batteries-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['django_batteries']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django>=4.1.7,<5.0.0']
+['django>=4.1.7,<5.0.0', 'djangorestframework>=3.14.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'django-batteries',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Set of most common utils for django/drf projects',
-    'long_description': "# Django-batteries\n\nThis package contains useful utilities for django/drf project\n\n## Models\n\nContains set of abstract models to enforce DRY principle for most common use cases\n\n### TimeStampedModel\n\n- `created`\n- `modified`\n\n### TimeFramedModel\n\n- `start`\n- `end`\n\n  For time bound entities\n\n### DescriptionModel\n\n- `description`\n\n### TitleModel\n\n- `title`\n\n### TitleDescriptionModel\n\n- `title`\n- `description`\n\n## Fields\n\n### Monitor field\n\nA DateTimeField that monitors another field on the same model and sets itself to the current date/time whenever the monitored field\nchanges.\nuse it like this in your models:\nclass MyMode(models.Model):\n\n    title = models.Charfield(max_length=50)\n    title_changed = MonitorField(_('title changed'), monitor='title')\n\n## Tests\n",
+    'long_description': "# Django-batteries\n\nThis package contains useful utilities for django/drf project\n\n## Models\n\nContains set of abstract models to enforce DRY principle for most common use cases\n\n### `django_batteries.models.TimeStampedModel`\n\n- `created`\n- `modified`\n\n### `django_batteries.models.TimeFramedModel`\n\n- `start`\n- `end`\n\n  For time bound entities\n\n### `django_batteries.models.DescriptionModel`\n\n- `description`\n\n### `django_batteries.models.TitleModel`\n\n- `title`\n\n### `django_batteries.models.TitleDescriptionModel`\n\n- `title`\n- `description`\n\n## Fields\n\n### Monitor field\n\nA DateTimeField that monitors another field on the same model and sets itself to the current date/time whenever the monitored field\nchanges.\nuse it like this in your models:\nclass MyMode(models.Model):\n\n    title = models.Charfield(max_length=50)\n    title_changed = MonitorField(_('title changed'), monitor='title')\n\n## Mixins\n\n### `django_batteries.mixins.ListSerializerMixin`\n\nAllow you to specify `list_serializer_class` that will be used only in list action\n\n## Paginators\n\n### django_batteries.paginators.ResultSetPagination\n\nPaginator with `page_size` as query parameter for setting page size\n\n### django_batteries.paginators.SingleResultPaginator\n\nCustom paginator class that returns not paginated(detail result) if qs result have only 1 item\n\n## Utils\n\n### django_batteries.utils.qs_admin_or_author\n\nReturn all objects if user is staff, otherwise return objects owned by user\n",
     'author': 'Oleksandr Korol',
     'author_email': 'zibertua@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

