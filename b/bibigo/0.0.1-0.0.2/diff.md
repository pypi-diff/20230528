# Comparing `tmp/bibigo-0.0.1.tar.gz` & `tmp/bibigo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.1.tar", last modified: Sun May 28 06:54:58 2023, max compression
+gzip compressed data, was "bibigo-0.0.2.tar", last modified: Sun May 28 07:55:08 2023, max compression
```

## Comparing `bibigo-0.0.1.tar` & `bibigo-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 06:54:58.006263 bibigo-0.0.1/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.1/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 06:54:58.006263 bibigo-0.0.1/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3906 2023-05-28 04:22:26.000000 bibigo-0.0.1/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.1/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      474 2023-05-28 06:54:58.006263 bibigo-0.0.1/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 06:54:58.002262 bibigo-0.0.1/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 06:54:58.002262 bibigo-0.0.1/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.1/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 06:54:58.006263 bibigo-0.0.1/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.1/src/bibigo/init/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2916 2023-05-28 06:27:56.000000 bibigo-0.0.1/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.1/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.1/src/bibigo/scripts.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      710 2023-05-28 06:20:23.000000 bibigo-0.0.1/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 06:54:58.006263 bibigo-0.0.1/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 06:54:57.000000 bibigo-0.0.1/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      396 2023-05-28 06:54:58.000000 bibigo-0.0.1/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 06:54:57.000000 bibigo-0.0.1/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 06:54:57.000000 bibigo-0.0.1/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 06:54:57.000000 bibigo-0.0.1/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 06:54:57.000000 bibigo-0.0.1/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.2/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 07:55:08.515187 bibigo-0.0.2/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.2/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.2/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      474 2023-05-28 07:55:08.515187 bibigo-0.0.2/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.2/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/src/bibigo/files/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.2/src/bibigo/files/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.2/src/bibigo/init/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2916 2023-05-28 06:27:56.000000 bibigo-0.0.2/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.2/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.2/src/bibigo/scripts.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      710 2023-05-28 06:20:23.000000 bibigo-0.0.2/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:55:08.515187 bibigo-0.0.2/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      425 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 07:55:08.000000 bibigo-0.0.2/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.1/LICENSE` & `bibigo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.1/src/bibigo/init/package.py` & `bibigo-0.0.2/src/bibigo/init/package.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.1/src/bibigo/init/settings.py` & `bibigo-0.0.2/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.1/src/bibigo/scripts.py` & `bibigo-0.0.2/src/bibigo/scripts.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.1/src/bibigo/utils.py` & `bibigo-0.0.2/src/bibigo/utils.py`

 * *Files identical despite different names*

