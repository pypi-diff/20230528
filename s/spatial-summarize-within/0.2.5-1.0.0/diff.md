# Comparing `tmp/spatial_summarize_within-0.2.5.tar.gz` & `tmp/spatial_summarize_within-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.2.5.tar", last modified: Mon May 15 04:12:15 2023, max compression
+gzip compressed data, was "spatial_summarize_within-1.0.0.tar", last modified: Sun May 28 20:46:27 2023, max compression
```

## Comparing `spatial_summarize_within-0.2.5.tar` & `spatial_summarize_within-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.191775 spatial_summarize_within-0.2.5/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.5/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-15 04:12:15.191663 spatial_summarize_within-0.2.5/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.5/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-15 04:12:15.191808 spatial_summarize_within-0.2.5/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-15 04:12:06.000000 spatial_summarize_within-0.2.5/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.190878 spatial_summarize_within-0.2.5/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2645 2023-05-15 03:55:52.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.191515 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-28 20:46:27.938464 spatial_summarize_within-1.0.0/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.0/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-28 20:46:27.938354 spatial_summarize_within-1.0.0/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-1.0.0/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-28 20:46:27.938499 spatial_summarize_within-1.0.0/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-28 20:42:41.000000 spatial_summarize_within-1.0.0/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-28 20:46:27.937630 spatial_summarize_within-1.0.0/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.0/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-1.0.0/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2645 2023-05-15 03:55:52.000000 spatial_summarize_within-1.0.0/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-1.0.0/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-1.0.0/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-28 20:46:27.938193 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-28 20:46:27.000000 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-28 20:46:27.000000 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-28 20:46:27.000000 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-28 20:46:27.000000 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-28 20:46:27.000000 spatial_summarize_within-1.0.0/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.2.5/LICENSE` & `spatial_summarize_within-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.5/README.md` & `spatial_summarize_within-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.5/spatial_summarize_within/max_within.py` & `spatial_summarize_within-1.0.0/spatial_summarize_within/max_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.5/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-1.0.0/spatial_summarize_within/mean_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.5/spatial_summarize_within/min_within.py` & `spatial_summarize_within-1.0.0/spatial_summarize_within/min_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.5/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-1.0.0/spatial_summarize_within/sum_within.py`

 * *Files identical despite different names*

