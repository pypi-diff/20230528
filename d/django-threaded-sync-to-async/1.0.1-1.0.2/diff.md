# Comparing `tmp/django_threaded_sync_to_async-1.0.1.tar.gz` & `tmp/django_threaded_sync_to_async-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_threaded_sync_to_async-1.0.1.tar", last modified: Sun May 28 07:47:43 2023, max compression
+gzip compressed data, was "django_threaded_sync_to_async-1.0.2.tar", last modified: Sun May 28 19:02:24 2023, max compression
```

## Comparing `django_threaded_sync_to_async-1.0.1.tar` & `django_threaded_sync_to_async-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 07:47:43.426292 django_threaded_sync_to_async-1.0.1/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1063 2023-05-26 19:21:14.000000 django_threaded_sync_to_async-1.0.1/LICENSE.md
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2848 2023-05-28 07:47:43.426292 django_threaded_sync_to_async-1.0.1/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1243 2023-05-28 07:46:05.000000 django_threaded_sync_to_async-1.0.1/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 07:47:43.422292 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4561 2023-05-28 07:24:38.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async/__init__.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 07:47:43.426292 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2848 2023-05-28 07:47:43.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      350 2023-05-28 07:47:43.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-28 07:47:43.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-05-28 07:47:43.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       30 2023-05-28 07:47:43.000000 django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       31 2023-05-27 15:17:43.000000 django_threaded_sync_to_async-1.0.1/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-28 07:47:43.426292 django_threaded_sync_to_async-1.0.1/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2348 2023-05-28 07:46:59.000000 django_threaded_sync_to_async-1.0.1/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1063 2023-05-26 19:21:14.000000 django_threaded_sync_to_async-1.0.2/LICENSE.md
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1250 2023-05-28 09:23:45.000000 django_threaded_sync_to_async-1.0.2/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2380 2023-05-28 18:27:08.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2294 2023-05-28 15:11:49.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/patch.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      389 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       30 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       31 2023-05-27 15:17:43.000000 django_threaded_sync_to_async-1.0.2/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2121 2023-05-28 19:01:38.000000 django_threaded_sync_to_async-1.0.2/setup.py
```

### Comparing `django_threaded_sync_to_async-1.0.1/LICENSE.md` & `django_threaded_sync_to_async-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_threaded_sync_to_async-1.0.1/PKG-INFO` & `django_threaded_sync_to_async-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: django_threaded_sync_to_async
-Version: 1.0.1
-Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently
+Version: 1.0.2
+Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently
 Home-page: https://github.com/excitoon/django_threaded_sync_to_async
 Author: Vladimir Chebotarev
 Author-email: vladimir.chebotarev@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/excitoon/django_threaded_sync_to_async/blob/master/README.md
 Project-URL: Source, https://github.com/excitoon/django_threaded_sync_to_async
 Project-URL: Tracker, https://github.com/excitoon/django_threaded_sync_to_async/issues
 Keywords: django,asyncio,asgiref,sync_to_async
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Text Processing :: Filters
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ## `django_threaded_sync_to_async`
 
-Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently.
+Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently.
 
 ```
 pip3 install django_threaded_sync_to_async
 ```
 
 ### `Executor`
 
@@ -54,15 +50,15 @@
 
 Maintains global dictionary of executors (`concurrent.futures.ThreadPoolExecutor`) accessed by name and allows to limit utilization of executor for a single context.
 
 ```python3
 import django_threaded_sync_to_async
 
 @django_threaded_sync_to_async.SharedExecutor("common", max_workers=3, max_tasks=2)
-def operations():
+async def operations():
     a = asgiref.sync.sync_to_async(long_call)(1)
     b = asgiref.sync.sync_to_async(long_call)(2)
     c = asgiref.sync.sync_to_async(long_call)(3)
     d = asgiref.sync.sync_to_async(long_call)(4)
     await asyncio.gather(a, b, c, d)
 ```
```

### Comparing `django_threaded_sync_to_async-1.0.1/README.md` & `django_threaded_sync_to_async-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## `django_threaded_sync_to_async`
 
-Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently.
+Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently.
 
 ```
 pip3 install django_threaded_sync_to_async
 ```
 
 ### `Executor`
 
@@ -23,14 +23,14 @@
 
 Maintains global dictionary of executors (`concurrent.futures.ThreadPoolExecutor`) accessed by name and allows to limit utilization of executor for a single context.
 
 ```python3
 import django_threaded_sync_to_async
 
 @django_threaded_sync_to_async.SharedExecutor("common", max_workers=3, max_tasks=2)
-def operations():
+async def operations():
     a = asgiref.sync.sync_to_async(long_call)(1)
     b = asgiref.sync.sync_to_async(long_call)(2)
     c = asgiref.sync.sync_to_async(long_call)(3)
     d = asgiref.sync.sync_to_async(long_call)(4)
     await asyncio.gather(a, b, c, d)
 ```
```

### Comparing `django_threaded_sync_to_async-1.0.1/django_threaded_sync_to_async.egg-info/PKG-INFO` & `django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: django-threaded-sync-to-async
-Version: 1.0.1
-Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently
+Version: 1.0.2
+Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently
 Home-page: https://github.com/excitoon/django_threaded_sync_to_async
 Author: Vladimir Chebotarev
 Author-email: vladimir.chebotarev@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/excitoon/django_threaded_sync_to_async/blob/master/README.md
 Project-URL: Source, https://github.com/excitoon/django_threaded_sync_to_async
 Project-URL: Tracker, https://github.com/excitoon/django_threaded_sync_to_async/issues
 Keywords: django,asyncio,asgiref,sync_to_async
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Text Processing :: Filters
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ## `django_threaded_sync_to_async`
 
-Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently.
+Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently.
 
 ```
 pip3 install django_threaded_sync_to_async
 ```
 
 ### `Executor`
 
@@ -54,15 +50,15 @@
 
 Maintains global dictionary of executors (`concurrent.futures.ThreadPoolExecutor`) accessed by name and allows to limit utilization of executor for a single context.
 
 ```python3
 import django_threaded_sync_to_async
 
 @django_threaded_sync_to_async.SharedExecutor("common", max_workers=3, max_tasks=2)
-def operations():
+async def operations():
     a = asgiref.sync.sync_to_async(long_call)(1)
     b = asgiref.sync.sync_to_async(long_call)(2)
     c = asgiref.sync.sync_to_async(long_call)(3)
     d = asgiref.sync.sync_to_async(long_call)(4)
     await asyncio.gather(a, b, c, d)
 ```
```

### Comparing `django_threaded_sync_to_async-1.0.1/setup.py` & `django_threaded_sync_to_async-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,27 @@
 import setuptools
 
 
 with open(f"{os.path.dirname(os.path.abspath(__file__))}/requirements.txt") as requirements:
     with open(f"{os.path.dirname(os.path.abspath(__file__))}/README.md") as readme:
         setuptools.setup(
             name="django_threaded_sync_to_async",
-            version="1.0.1",
-            description="Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=None, executor=...)`, effectively allowing Django to make calls to database concurrently",
+            version="1.0.2",
+            description="Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently",
             long_description=readme.read(),
             long_description_content_type="text/markdown",
             author="Vladimir Chebotarev",
             author_email="vladimir.chebotarev@gmail.com",
             license="MIT",
             classifiers=[
                 "Development Status :: 5 - Production/Stable",
                 "Intended Audience :: Developers",
                 "License :: OSI Approved :: MIT License",
                 "Operating System :: OS Independent",
                 "Programming Language :: Python :: 3 :: Only",
-                "Programming Language :: Python :: 3.6",
-                "Programming Language :: Python :: 3.7",
-                "Programming Language :: Python :: 3.8",
-                "Programming Language :: Python :: 3.9",
                 "Programming Language :: Python :: 3.10",
                 "Programming Language :: Python :: 3.11",
                 "Programming Language :: Python :: 3.12",
                 "Topic :: Software Development :: Libraries :: Python Modules",
                 "Topic :: Software Development :: Version Control :: Git",
                 "Topic :: Text Processing :: Filters",
             ], # FIXME
```

