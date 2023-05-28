# Comparing `tmp/django-toolshed-0.5.5.tar.gz` & `tmp/django_toolshed-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-toolshed-0.5.5.tar", max compression
+gzip compressed data, was "django_toolshed-0.5.6.tar", max compression
```

## Comparing `django-toolshed-0.5.5.tar` & `django_toolshed-0.5.6.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1069 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/LICENSE
--rw-r--r--   0        0        0       22 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/__init__.py
--rw-r--r--   0        0        0      292 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/apps.py
--rwxr-xr-x   0        0        0     1381 2021-12-18 17:09:19.982754 django-toolshed-0.5.5/django_toolshed/celery_auto_app.py
--rw-r--r--   0        0        0      254 2022-06-01 16:38:09.319991 django-toolshed-0.5.5/django_toolshed/celery_urls.py
--rw-r--r--   0        0        0     2072 2022-06-01 16:45:48.464357 django-toolshed-0.5.5/django_toolshed/celery_views.py
--rw-r--r--   0        0        0      969 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/management/commands/create_management_command.py
--rw-r--r--   0        0        0      264 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/management/commands/list_apps.py
--rw-r--r--   0        0        0      637 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/management/commands/list_commands.py
--rw-r--r--   0        0        0      337 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/management/commands/list_users.py
--rw-r--r--   0        0        0     1809 2021-11-09 23:02:33.020072 django-toolshed-0.5.5/django_toolshed/mixins.py
--rw-r--r--   0        0        0       37 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/signals.py
--rw-r--r--   0        0        0        0 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/static/django_toolshed/css/.gitkeep
--rw-r--r--   0        0        0        0 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/static/django_toolshed/images/.gitkeep
--rw-r--r--   0        0        0        0 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/static/django_toolshed/js/.gitkeep
--rw-r--r--   0        0        0        0 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/templates/django_toolshed/.gitkeep
--rw-r--r--   0        0        0       47 2021-11-08 13:28:39.012311 django-toolshed-0.5.5/django_toolshed/urls.py
--rw-r--r--   0        0        0     1104 2022-06-01 16:45:54.384362 django-toolshed-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1138 2022-06-01 16:46:04.098821 django-toolshed-0.5.5/setup.py
--rw-r--r--   0        0        0      637 2022-06-01 16:46:04.098999 django-toolshed-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/apps.py
+-rwxr-xr-x   0        0        0     1381 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/celery_auto_app.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/celery_urls.py
+-rw-r--r--   0        0        0     3156 2023-05-28 11:56:50.471025 django_toolshed-0.5.6/django_toolshed/celery_views.py
+-rw-r--r--   0        0        0      969 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/create_management_command.py
+-rw-r--r--   0        0        0      264 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_apps.py
+-rw-r--r--   0        0        0      637 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_commands.py
+-rw-r--r--   0        0        0      321 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/management/commands/list_users.py
+-rw-r--r--   0        0        0     1797 2023-05-28 11:56:50.471025 django_toolshed-0.5.6/django_toolshed/mixins.py
+-rw-r--r--   0        0        0       37 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/signals.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/css/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/images/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/static/django_toolshed/js/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/templates/django_toolshed/.gitkeep
+-rw-r--r--   0        0        0       47 2023-05-26 16:33:22.599223 django_toolshed-0.5.6/django_toolshed/urls.py
+-rw-r--r--   0        0        0     1148 2023-05-28 11:56:51.851087 django_toolshed-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 django_toolshed-0.5.6/PKG-INFO
```

### Comparing `django-toolshed-0.5.5/LICENSE` & `django_toolshed-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-toolshed-0.5.5/django_toolshed/celery_auto_app.py` & `django_toolshed-0.5.6/django_toolshed/celery_auto_app.py`

 * *Files identical despite different names*

### Comparing `django-toolshed-0.5.5/django_toolshed/celery_views.py` & `django_toolshed-0.5.6/django_toolshed/celery_views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,84 @@
+# pylint: disable=abstract-method
 import logging
 
 from celery import current_app
 from celery.result import AsyncResult
+from celery.states import ALL_STATES
+from drf_spectacular.types import OpenApiTypes
+from drf_spectacular.utils import OpenApiParameter, extend_schema
 from rest_framework import serializers
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound, ParseError
 from rest_framework.response import Response
 from rest_framework.viewsets import ViewSet
 
 
-# pylint: disable=abstract-method
-class TaskSerializer(serializers.Serializer):
+class CreateTaskSerializer(serializers.Serializer):
     task_name = serializers.CharField()
     args = serializers.ListField(required=False)
     kwargs = serializers.DictField(required=False)
 
 
-# pylint: disable=no-self-use
+class ReadTaskSerializer(serializers.Serializer):
+    task_id = serializers.CharField()
+    status = serializers.ChoiceField(choices=ALL_STATES)
+
+
 class CeleryTaskViewSet(ViewSet):
-    serializer_class = TaskSerializer
+    serializer_class = None
 
-    def retrieve(self, request, pk=None):
-        result = AsyncResult(pk)
-        return Response(dict(task_id=result.task_id, status=result.status))
+    @extend_schema(
+        operation_id="read_task_status",
+        parameters=[
+            OpenApiParameter(
+                name="id", type=OpenApiTypes.UUID, location=OpenApiParameter.PATH
+            )
+        ],
+        responses={200: ReadTaskSerializer},
+    )
+    def retrieve(self, request, pk=None, **kwargs):
+        async_result = AsyncResult(pk)
+        serializer = ReadTaskSerializer(
+            data=dict(
+                task_id=async_result.task_id,
+                status=async_result.status,
+            )
+        )
+        serializer.is_valid(raise_exception=True)
+        return Response(serializer.data)
 
+    @extend_schema(
+        operation_id="create_task",
+        request=CreateTaskSerializer,
+        responses={201: ReadTaskSerializer},
+    )
     def create(self, request):
-        serializer = TaskSerializer(data=request.data)
+        serializer = CreateTaskSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         task_name = serializer.data["task_name"]
+
         worker_tasks = registered_tasks()
-        task_arguments = serializer.data
-        task_arguments.pop("task_name")
         if task_name not in worker_tasks:
             raise NotFound(f"{task_name=} not found in registered {worker_tasks=}")
-        sent_task = current_app.send_task(task_name, **task_arguments)
-        logging.info(f"Triggered celery {task_name=} with {task_arguments=}")
-        return Response(
-            data={**serializer.data, "task_id": sent_task.task_id}, status=201
+
+        async_result = current_app.send_task(
+            name=task_name,
+            args=serializer.data.get("args"),
+            kwargs=serializer.data.get("kwargs"),
         )
+        logging.info(f"Triggered celery {task_name=} via HTTP request")
+        serializer = ReadTaskSerializer(
+            data=dict(
+                task_id=async_result.task_id,
+                status=async_result.status,
+            )
+        )
+        serializer.is_valid(raise_exception=True)
+        return Response(serializer.data, status=201)
 
     @action(detail=False, methods=["GET"])
     def types(self, request):
         worker_tasks = registered_tasks()
         return Response({"task_types": worker_tasks})
```

### Comparing `django-toolshed-0.5.5/django_toolshed/management/commands/create_management_command.py` & `django_toolshed-0.5.6/django_toolshed/management/commands/create_management_command.py`

 * *Files identical despite different names*

### Comparing `django-toolshed-0.5.5/django_toolshed/management/commands/list_commands.py` & `django_toolshed-0.5.6/django_toolshed/management/commands/list_commands.py`

 * *Files identical despite different names*

### Comparing `django-toolshed-0.5.5/django_toolshed/mixins.py` & `django_toolshed-0.5.6/django_toolshed/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mypy: ignore-errors
 from django.contrib import admin
 from django.urls import reverse
 from django.utils.html import format_html
 
 
-class UserURLMixin:  # pylint: disable=too-few-public-methods,no-self-use
+class UserURLMixin:  # pylint: disable=too-few-public-methods
     def user_url(self, obj):
         if not obj.user:
             return "-"
         url = reverse("admin:users_user_change", args=[obj.user.id])
         return format_html(
             '<a href="{}">{}</a>', url, obj.user.email or obj.user.username
         )
```

### Comparing `django-toolshed-0.5.5/pyproject.toml` & `django_toolshed-0.5.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 [tool.poetry]
 name = "django-toolshed"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 celery-auto-app = "django_toolshed.celery_auto_app:command"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ipython_genutils = "^0.2.0"
 django-click = "^2.2.0"
 iterfzf = "^0.5.0"
 djangorestframework = "^3.13.1"
 celery = "^5.2.1"
+drf-spectacular = "^0.26.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "6.2.2"
 pytest-clarity = "0.2.0a1"
 pytest-cov = "2.10.0"
 pytest-django = "4.1.0"
 coverage = "5.5"
 django-coverage-plugin = "1.8.0"
-black = "20.8b1"
 mypy = "0.782"
 mypy-extensions = "0.4.3"
 pylint = "^2.9.3"
 pylint-django = "^2.4.4"
 ptipython = "1.0.1"
 ptpython = "3.0.16"
 django-extensions = "^3.1.1"
-setuptools = "^54.1.2"
 pudb = "^2021.1"
 beautifulsoup4 = "^4.10.0"
 pytest-celery = "^0.0.0"
-docker-compose = "^1.29.2"
 redis = "^4.0.2"
 Django = "^4.0.2"
 lxml = "^4.9.0"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+docker-compose = "^1.29.2"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 skip_numeric_underscore_normalization = true
 exclude = ".*(venv|virtualenv|migrations|.db|.poetry|.poetry-cache)"
```

### Comparing `django-toolshed-0.5.5/PKG-INFO` & `django_toolshed-0.5.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: django-toolshed
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 License: MIT
 Author: Dani Hodovic
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.1,<6.0.0)
 Requires-Dist: django-click (>=2.2.0,<3.0.0)
 Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
+Requires-Dist: drf-spectacular (>=0.26.2,<0.27.0)
 Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0)
 Requires-Dist: iterfzf (>=0.5.0,<0.6.0)
```

