# Comparing `tmp/tinyerr-0.0.1a0.tar.gz` & `tmp/tinyerr-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyerr-0.0.1a0.tar", last modified: Mon May 15 09:39:55 2023, max compression
+gzip compressed data, was "tinyerr-0.0.1a1.tar", last modified: Sun May 28 08:02:09 2023, max compression
```

## Comparing `tinyerr-0.0.1a0.tar` & `tinyerr-0.0.1a1.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-15 09:39:55.610749 tinyerr-0.0.1a0/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-05-15 09:32:44.000000 tinyerr-0.0.1a0/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1951 2023-05-15 09:39:55.610563 tinyerr-0.0.1a0/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      447 2023-05-15 09:29:07.000000 tinyerr-0.0.1a0/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      538 2023-05-15 08:55:20.000000 tinyerr-0.0.1a0/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       13 2023-05-15 03:56:01.000000 tinyerr-0.0.1a0/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-05-15 09:39:55.610796 tinyerr-0.0.1a0/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-15 09:39:55.607148 tinyerr-0.0.1a0/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-15 09:39:55.609391 tinyerr-0.0.1a0/src/tinyerr/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       43 2023-05-15 06:51:07.000000 tinyerr-0.0.1a0/src/tinyerr/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      343 2023-05-15 06:16:08.000000 tinyerr-0.0.1a0/src/tinyerr/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3013 2023-05-15 06:14:04.000000 tinyerr-0.0.1a0/src/tinyerr/anchor.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2221 2023-05-15 09:30:15.000000 tinyerr-0.0.1a0/src/tinyerr/errors.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      888 2023-05-15 06:55:46.000000 tinyerr-0.0.1a0/src/tinyerr/exechook.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1328 2023-05-15 06:51:07.000000 tinyerr-0.0.1a0/src/tinyerr/frames.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-15 09:39:55.610258 tinyerr-0.0.1a0/src/tinyerr.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1951 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      399 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       45 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       13 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        8 2023-05-15 09:39:55.000000 tinyerr-0.0.1a0/src/tinyerr.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.361466 tinyerr-0.0.1a1/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-05-15 09:32:44.000000 tinyerr-0.0.1a1/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-05-28 08:02:09.361327 tinyerr-0.0.1a1/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1183 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      441 2023-05-28 08:01:43.000000 tinyerr-0.0.1a1/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-05-28 08:02:09.361512 tinyerr-0.0.1a1/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.359089 tinyerr-0.0.1a1/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.360463 tinyerr-0.0.1a1/src/tinyerr/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       43 2023-05-15 06:51:07.000000 tinyerr-0.0.1a1/src/tinyerr/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      468 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/src/tinyerr/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3013 2023-05-28 07:57:36.000000 tinyerr-0.0.1a1/src/tinyerr/anchor.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     7680 2023-05-28 07:59:15.000000 tinyerr-0.0.1a1/src/tinyerr/errors.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1342 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/src/tinyerr/exechook.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2807 2023-05-17 06:55:24.000000 tinyerr-0.0.1a1/src/tinyerr/frames.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.361156 tinyerr-0.0.1a1/src/tinyerr.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      348 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       45 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        8 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/top_level.txt
```

### Comparing `tinyerr-0.0.1a0/LICENSE` & `tinyerr-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyerr-0.0.1a0/src/tinyerr/anchor.py` & `tinyerr-0.0.1a1/src/tinyerr/anchor.py`

 * *Files identical despite different names*

