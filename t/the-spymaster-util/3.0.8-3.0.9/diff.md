# Comparing `tmp/the_spymaster_util-3.0.8.tar.gz` & `tmp/the_spymaster_util-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_spymaster_util-3.0.8.tar", max compression
+gzip compressed data, was "the_spymaster_util-3.0.9.tar", max compression
```

## Comparing `the_spymaster_util-3.0.8.tar` & `the_spymaster_util-3.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      425 2022-06-10 11:30:12.549286 the_spymaster_util-3.0.8/README.md
--rw-r--r--   0        0        0     1516 2023-05-27 23:27:56.523058 the_spymaster_util-3.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-15 13:25:57.275196 the_spymaster_util-3.0.8/the_spymaster_util/__init__.py
--rw-r--r--   0        0        0     4617 2023-01-27 13:56:20.797826 the_spymaster_util-3.0.8/the_spymaster_util/async_task_manager.py
--rw-r--r--   0        0        0     2324 2023-02-10 18:06:29.069924 the_spymaster_util-3.0.8/the_spymaster_util/config.py
--rw-r--r--   0        0        0     1250 2023-01-27 14:07:17.722389 the_spymaster_util-3.0.8/the_spymaster_util/context_thread.py
--rw-r--r--   0        0        0        0 2023-01-26 23:16:49.007374 the_spymaster_util-3.0.8/the_spymaster_util/http/__init__.py
--rw-r--r--   0        0        0     6983 2023-02-10 18:21:42.356758 the_spymaster_util-3.0.8/the_spymaster_util/http/base_client.py
--rw-r--r--   0        0        0      406 2023-02-10 18:20:33.626233 the_spymaster_util-3.0.8/the_spymaster_util/http/defs.py
--rw-r--r--   0        0        0     3521 2023-02-10 19:25:44.706999 the_spymaster_util-3.0.8/the_spymaster_util/http/errors.py
--rw-r--r--   0        0        0     7087 2023-02-23 17:57:01.036300 the_spymaster_util-3.0.8/the_spymaster_util/logger.py
--rw-r--r--   0        0        0      482 2022-06-12 20:38:01.845963 the_spymaster_util-3.0.8/the_spymaster_util/measure_time.py
--rw-r--r--   0        0        0      310 2023-02-10 17:50:20.410580 the_spymaster_util-3.0.8/the_spymaster_util/strings.py
--rw-r--r--   0        0        0     3914 2023-01-27 14:18:34.256651 the_spymaster_util-3.0.8/the_spymaster_util/ttl_dict.py
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 the_spymaster_util-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0      425 2022-06-10 11:30:12.549286 the_spymaster_util-3.0.9/README.md
+-rw-r--r--   0        0        0     1516 2023-05-27 23:30:19.436541 the_spymaster_util-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-15 13:25:57.275196 the_spymaster_util-3.0.9/the_spymaster_util/__init__.py
+-rw-r--r--   0        0        0     4617 2023-01-27 13:56:20.797826 the_spymaster_util-3.0.9/the_spymaster_util/async_task_manager.py
+-rw-r--r--   0        0        0     2324 2023-02-10 18:06:29.069924 the_spymaster_util-3.0.9/the_spymaster_util/config.py
+-rw-r--r--   0        0        0     1250 2023-01-27 14:07:17.722389 the_spymaster_util-3.0.9/the_spymaster_util/context_thread.py
+-rw-r--r--   0        0        0        0 2023-01-26 23:16:49.007374 the_spymaster_util-3.0.9/the_spymaster_util/http/__init__.py
+-rw-r--r--   0        0        0     6983 2023-02-10 18:21:42.356758 the_spymaster_util-3.0.9/the_spymaster_util/http/base_client.py
+-rw-r--r--   0        0        0      406 2023-02-10 18:20:33.626233 the_spymaster_util-3.0.9/the_spymaster_util/http/defs.py
+-rw-r--r--   0        0        0     3521 2023-02-10 19:25:44.706999 the_spymaster_util-3.0.9/the_spymaster_util/http/errors.py
+-rw-r--r--   0        0        0     7087 2023-02-23 17:57:01.036300 the_spymaster_util-3.0.9/the_spymaster_util/logger.py
+-rw-r--r--   0        0        0      482 2022-06-12 20:38:01.845963 the_spymaster_util-3.0.9/the_spymaster_util/measure_time.py
+-rw-r--r--   0        0        0      310 2023-02-10 17:50:20.410580 the_spymaster_util-3.0.9/the_spymaster_util/strings.py
+-rw-r--r--   0        0        0     3914 2023-01-27 14:18:34.256651 the_spymaster_util-3.0.9/the_spymaster_util/ttl_dict.py
+-rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 the_spymaster_util-3.0.9/PKG-INFO
```

### Comparing `the_spymaster_util-3.0.8/pyproject.toml` & `the_spymaster_util-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Poetry
 
 [tool.poetry]
 name = "the-spymaster-util"
-version = "3.0.8"
+version = "3.0.9"
 description = "Common utilities and infra for The Spymaster game."
 authors = ["Asaf Kali <akali93@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "the_spymaster_util" }]
 repository = "https://github.com/asaf-kali/the-spymaster-util"
 
 [tool.poetry.dependencies]
```

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/async_task_manager.py` & `the_spymaster_util-3.0.9/the_spymaster_util/async_task_manager.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/config.py` & `the_spymaster_util-3.0.9/the_spymaster_util/config.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/context_thread.py` & `the_spymaster_util-3.0.9/the_spymaster_util/context_thread.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/http/base_client.py` & `the_spymaster_util-3.0.9/the_spymaster_util/http/base_client.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/http/errors.py` & `the_spymaster_util-3.0.9/the_spymaster_util/http/errors.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/logger.py` & `the_spymaster_util-3.0.9/the_spymaster_util/logger.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/the_spymaster_util/ttl_dict.py` & `the_spymaster_util-3.0.9/the_spymaster_util/ttl_dict.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_util-3.0.8/PKG-INFO` & `the_spymaster_util-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: the-spymaster-util
-Version: 3.0.8
+Version: 3.0.9
 Summary: Common utilities and infra for The Spymaster game.
 Home-page: https://github.com/asaf-kali/the-spymaster-util
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

