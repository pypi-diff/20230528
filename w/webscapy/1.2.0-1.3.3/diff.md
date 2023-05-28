# Comparing `tmp/webscapy-1.2.0.tar.gz` & `tmp/webscapy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.2.0.tar", last modified: Sun May 28 10:01:56 2023, max compression
+gzip compressed data, was "webscapy-1.3.3.tar", last modified: Sun May 28 11:12:40 2023, max compression
```

## Comparing `webscapy-1.2.0.tar` & `webscapy-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.237221 webscapy-1.2.0/
--rw-rw-rw-   0        0        0      131 2023-05-28 10:01:56.235216 webscapy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3697 2023-05-28 09:56:04.000000 webscapy-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 10:01:56.239243 webscapy-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      225 2023-05-28 10:01:46.000000 webscapy-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.191211 webscapy-1.2.0/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.2.0/webscapy/__init__.py
--rw-rw-rw-   0        0        0     4177 2023-05-28 10:00:29.000000 webscapy-1.2.0/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.229213 webscapy-1.2.0/webscapy.egg-info/
--rw-rw-rw-   0        0        0      131 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.482298 webscapy-1.3.3/
+-rw-rw-rw-   0        0        0     4741 2023-05-28 11:12:40.480309 webscapy-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4446 2023-05-28 11:11:47.000000 webscapy-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:12:40.483303 webscapy-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-28 11:12:27.000000 webscapy-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.415587 webscapy-1.3.3/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.3.3/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     4177 2023-05-28 10:00:29.000000 webscapy-1.3.3/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.473299 webscapy-1.3.3/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     4741 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.2.0/webscapy/webscapy.py` & `webscapy-1.3.3/webscapy/webscapy.py`

 * *Files identical despite different names*

