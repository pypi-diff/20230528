# Comparing `tmp/the-spymaster-util-3.0.6.tar.gz` & `tmp/the_spymaster_util-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-spymaster-util-3.0.6.tar", last modified: Thu Feb 23 17:57:33 2023, max compression
+gzip compressed data, was "the_spymaster_util-3.0.7.tar", max compression
```

## Comparing `the-spymaster-util-3.0.6.tar` & `the_spymaster_util-3.0.7.tar`

### file list

```diff
@@ -1,37 +1,15 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/
--rw-rw-r--   0 akali     (1000) akali     (1000)      720 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      425 2022-06-10 11:30:12.000000 the-spymaster-util-3.0.6/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.028686 the-spymaster-util-3.0.6/playground/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-04-21 11:24:48.000000 the-spymaster-util-3.0.6/playground/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      724 2023-01-26 23:27:54.000000 the-spymaster-util-3.0.6/playground/multithread_logging.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      595 2023-01-27 14:06:26.000000 the-spymaster-util-3.0.6/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      466 2023-02-23 17:57:25.000000 the-spymaster-util-3.0.6/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.028686 the-spymaster-util-3.0.6/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-07-02 17:00:22.000000 the-spymaster-util-3.0.6/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      217 2023-01-26 23:27:29.000000 the-spymaster-util-3.0.6/tests/conftest.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     5308 2023-02-10 18:23:00.000000 the-spymaster-util-3.0.6/tests/test_base_http_client.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      947 2023-02-10 18:05:16.000000 the-spymaster-util-3.0.6/tests/test_config.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      289 2022-06-12 20:38:56.000000 the-spymaster-util-3.0.6/tests/test_measure_time.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2413 2023-01-27 13:56:20.000000 the-spymaster-util-3.0.6/tests/test_task_manager.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3448 2023-01-27 16:05:42.000000 the-spymaster-util-3.0.6/tests/test_ttl_dict.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/the_spymaster_util/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-07-15 13:25:57.000000 the-spymaster-util-3.0.6/the_spymaster_util/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4617 2023-01-27 13:56:20.000000 the-spymaster-util-3.0.6/the_spymaster_util/async_task_manager.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2324 2023-02-10 18:06:29.000000 the-spymaster-util-3.0.6/the_spymaster_util/config.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1250 2023-01-27 14:07:17.000000 the-spymaster-util-3.0.6/the_spymaster_util/context_thread.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/the_spymaster_util/http/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-01-26 23:16:49.000000 the-spymaster-util-3.0.6/the_spymaster_util/http/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6983 2023-02-10 18:21:42.000000 the-spymaster-util-3.0.6/the_spymaster_util/http/base_client.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      406 2023-02-10 18:20:33.000000 the-spymaster-util-3.0.6/the_spymaster_util/http/defs.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3521 2023-02-10 19:25:44.000000 the-spymaster-util-3.0.6/the_spymaster_util/http/errors.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7087 2023-02-23 17:57:01.000000 the-spymaster-util-3.0.6/the_spymaster_util/logger.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      482 2022-06-12 20:38:01.000000 the-spymaster-util-3.0.6/the_spymaster_util/measure_time.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      310 2023-02-10 17:50:20.000000 the-spymaster-util-3.0.6/the_spymaster_util/strings.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3914 2023-01-27 14:18:34.000000 the-spymaster-util-3.0.6/the_spymaster_util/ttl_dict.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-23 17:57:33.032686 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      720 2023-02-23 17:57:33.000000 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      878 2023-02-23 17:57:33.000000 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-02-23 17:57:33.000000 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       68 2023-02-23 17:57:33.000000 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       36 2023-02-23 17:57:33.000000 the-spymaster-util-3.0.6/the_spymaster_util.egg-info/top_level.txt
+-rw-r--r--   0        0        0      425 2022-06-10 11:30:12.549286 the_spymaster_util-3.0.7/README.md
+-rw-r--r--   0        0        0     1535 2023-05-27 23:25:46.545706 the_spymaster_util-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-15 13:25:57.275196 the_spymaster_util-3.0.7/the_spymaster_util/__init__.py
+-rw-r--r--   0        0        0     4617 2023-01-27 13:56:20.797826 the_spymaster_util-3.0.7/the_spymaster_util/async_task_manager.py
+-rw-r--r--   0        0        0     2324 2023-02-10 18:06:29.069924 the_spymaster_util-3.0.7/the_spymaster_util/config.py
+-rw-r--r--   0        0        0     1250 2023-01-27 14:07:17.722389 the_spymaster_util-3.0.7/the_spymaster_util/context_thread.py
+-rw-r--r--   0        0        0        0 2023-01-26 23:16:49.007374 the_spymaster_util-3.0.7/the_spymaster_util/http/__init__.py
+-rw-r--r--   0        0        0     6983 2023-02-10 18:21:42.356758 the_spymaster_util-3.0.7/the_spymaster_util/http/base_client.py
+-rw-r--r--   0        0        0      406 2023-02-10 18:20:33.626233 the_spymaster_util-3.0.7/the_spymaster_util/http/defs.py
+-rw-r--r--   0        0        0     3521 2023-02-10 19:25:44.706999 the_spymaster_util-3.0.7/the_spymaster_util/http/errors.py
+-rw-r--r--   0        0        0     7087 2023-02-23 17:57:01.036300 the_spymaster_util-3.0.7/the_spymaster_util/logger.py
+-rw-r--r--   0        0        0      482 2022-06-12 20:38:01.845963 the_spymaster_util-3.0.7/the_spymaster_util/measure_time.py
+-rw-r--r--   0        0        0      310 2023-02-10 17:50:20.410580 the_spymaster_util-3.0.7/the_spymaster_util/strings.py
+-rw-r--r--   0        0        0     3914 2023-01-27 14:18:34.256651 the_spymaster_util-3.0.7/the_spymaster_util/ttl_dict.py
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 the_spymaster_util-3.0.7/PKG-INFO
```

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/async_task_manager.py` & `the_spymaster_util-3.0.7/the_spymaster_util/async_task_manager.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/config.py` & `the_spymaster_util-3.0.7/the_spymaster_util/config.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/context_thread.py` & `the_spymaster_util-3.0.7/the_spymaster_util/context_thread.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/http/base_client.py` & `the_spymaster_util-3.0.7/the_spymaster_util/http/base_client.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/http/errors.py` & `the_spymaster_util-3.0.7/the_spymaster_util/http/errors.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/logger.py` & `the_spymaster_util-3.0.7/the_spymaster_util/logger.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-util-3.0.6/the_spymaster_util/ttl_dict.py` & `the_spymaster_util-3.0.7/the_spymaster_util/ttl_dict.py`

 * *Files identical despite different names*

