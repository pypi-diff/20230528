# Comparing `tmp/bibigo-0.0.3.tar.gz` & `tmp/bibigo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.3.tar", last modified: Sun May 28 08:07:15 2023, max compression
+gzip compressed data, was "bibigo-0.0.4.tar", last modified: Sun May 28 08:10:22 2023, max compression
```

## Comparing `bibigo-0.0.3.tar` & `bibigo-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.3/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:07:15.284503 bibigo-0.0.3/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.3/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.3/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      520 2023-05-28 08:07:15.284503 bibigo-0.0.3/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.280503 bibigo-0.0.3/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.3/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.3/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.3/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.3/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      985 2023-05-28 06:20:30.000000 bibigo-0.0.3/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo/files/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.3/src/bibigo/files/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.3/src/bibigo/files/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      508 2023-05-28 05:57:29.000000 bibigo-0.0.3/src/bibigo/files/setup.cfg.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.3/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.3/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2212 2023-05-28 06:34:44.000000 bibigo-0.0.3/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.3/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2916 2023-05-28 06:27:56.000000 bibigo-0.0.3/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.3/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.3/src/bibigo/scripts.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      710 2023-05-28 06:20:23.000000 bibigo-0.0.3/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:07:15.284503 bibigo-0.0.3/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      835 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 08:07:15.000000 bibigo-0.0.3/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.4/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:10:22.415804 bibigo-0.0.4/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.4/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.4/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      533 2023-05-28 08:10:22.415804 bibigo-0.0.4/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.4/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.4/src/bibigo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.4/src/bibigo/__pycache__/scripts.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.4/src/bibigo/__pycache__/test.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      985 2023-05-28 06:20:30.000000 bibigo-0.0.4/src/bibigo/__pycache__/utils.cpython-39.pyc
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo/files/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.4/src/bibigo/files/.dockerignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.4/src/bibigo/files/.gitignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.4/src/bibigo/files/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.4/src/bibigo/files/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      508 2023-05-28 05:57:29.000000 bibigo-0.0.4/src/bibigo/files/setup.cfg.default
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.4/src/bibigo/init/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo/init/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.4/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2212 2023-05-28 06:34:44.000000 bibigo-0.0.4/src/bibigo/init/__pycache__/package.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.4/src/bibigo/init/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2916 2023-05-28 06:27:56.000000 bibigo-0.0.4/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.4/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.4/src/bibigo/scripts.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      710 2023-05-28 06:20:23.000000 bibigo-0.0.4/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:10:22.415804 bibigo-0.0.4/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      910 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 08:10:22.000000 bibigo-0.0.4/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.3/LICENSE` & `bibigo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/README.md` & `bibigo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/setup.cfg` & `bibigo-0.0.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 bibigo = 
 	files/**/*
+	files/**/.*
 
 [options.entry_points]
 console_scripts = 
 	bibigo = bibigo.scripts:bibigo
 
 [egg_info]
 tag_build =
```

### Comparing `bibigo-0.0.3/src/bibigo/__pycache__/scripts.cpython-39.pyc` & `bibigo-0.0.4/src/bibigo/__pycache__/scripts.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/__pycache__/utils.cpython-39.pyc` & `bibigo-0.0.4/src/bibigo/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/init/__pycache__/package.cpython-39.pyc` & `bibigo-0.0.4/src/bibigo/init/__pycache__/package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/init/__pycache__/settings.cpython-39.pyc` & `bibigo-0.0.4/src/bibigo/init/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/init/package.py` & `bibigo-0.0.4/src/bibigo/init/package.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/init/settings.py` & `bibigo-0.0.4/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/scripts.py` & `bibigo-0.0.4/src/bibigo/scripts.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo/utils.py` & `bibigo-0.0.4/src/bibigo/utils.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.3/src/bibigo.egg-info/SOURCES.txt` & `bibigo-0.0.4/src/bibigo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 src/bibigo.egg-info/entry_points.txt
 src/bibigo.egg-info/requires.txt
 src/bibigo.egg-info/top_level.txt
 src/bibigo/__pycache__/__init__.cpython-39.pyc
 src/bibigo/__pycache__/scripts.cpython-39.pyc
 src/bibigo/__pycache__/test.cpython-39.pyc
 src/bibigo/__pycache__/utils.cpython-39.pyc
+src/bibigo/files/.dockerignore.default
+src/bibigo/files/.gitignore.default
 src/bibigo/files/__init__.py
 src/bibigo/files/pyproject.toml.default
 src/bibigo/files/setup.cfg.default
 src/bibigo/init/__init__.py
 src/bibigo/init/package.py
 src/bibigo/init/settings.py
 src/bibigo/init/__pycache__/__init__.cpython-39.pyc
```

