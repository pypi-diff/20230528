# Comparing `tmp/webscapy-1.0.0.tar.gz` & `tmp/webscapy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.0.0.tar", last modified: Sun May 28 06:41:00 2023, max compression
+gzip compressed data, was "webscapy-1.1.0.tar", last modified: Sun May 28 08:53:03 2023, max compression
```

## Comparing `webscapy-1.0.0.tar` & `webscapy-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 06:41:00.769096 webscapy-1.0.0/
--rw-rw-rw-   0        0        0      131 2023-05-28 06:41:00.768098 webscapy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-28 06:41:00.770104 webscapy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      225 2023-05-28 06:40:49.000000 webscapy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 06:41:00.726540 webscapy-1.0.0/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.0.0/webscapy/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-05-28 06:36:16.000000 webscapy-1.0.0/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 06:41:00.765104 webscapy-1.0.0/webscapy.egg-info/
--rw-rw-rw-   0        0        0      131 2023-05-28 06:41:00.000000 webscapy-1.0.0/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-28 06:41:00.000000 webscapy-1.0.0/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 06:41:00.000000 webscapy-1.0.0/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 06:37:52.000000 webscapy-1.0.0/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-28 06:41:00.000000 webscapy-1.0.0/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.784985 webscapy-1.1.0/
+-rw-rw-rw-   0        0        0      131 2023-05-28 08:53:03.780985 webscapy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       97 2023-05-28 06:36:34.000000 webscapy-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 08:53:03.785988 webscapy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      225 2023-05-28 08:53:00.000000 webscapy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.737621 webscapy-1.1.0/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.1.0/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     4008 2023-05-28 08:48:45.000000 webscapy-1.1.0/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.775012 webscapy-1.1.0/webscapy.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 08:52:41.000000 webscapy-1.1.0/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/top_level.txt
```

