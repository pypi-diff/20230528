# Comparing `tmp/edaplore-0.2.1.tar.gz` & `tmp/edaplore-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edaplore-0.2.1.tar", last modified: Sun May 28 19:22:27 2023, max compression
+gzip compressed data, was "edaplore-0.2.2.tar", last modified: Sun May 28 19:36:20 2023, max compression
```

## Comparing `edaplore-0.2.1.tar` & `edaplore-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 maximzabelin   (501) staff       (20)        0 2023-05-28 19:22:27.387423 edaplore-0.2.1/
--rw-r--r--   0 maximzabelin   (501) staff       (20)      215 2023-05-28 19:22:27.387057 edaplore-0.2.1/PKG-INFO
-drwxr-xr-x   0 maximzabelin   (501) staff       (20)        0 2023-05-28 19:22:27.386758 edaplore-0.2.1/edaplore.egg-info/
--rw-r--r--   0 maximzabelin   (501) staff       (20)      215 2023-05-28 19:22:27.000000 edaplore-0.2.1/edaplore.egg-info/PKG-INFO
--rw-r--r--   0 maximzabelin   (501) staff       (20)      167 2023-05-28 19:22:27.000000 edaplore-0.2.1/edaplore.egg-info/SOURCES.txt
--rw-r--r--   0 maximzabelin   (501) staff       (20)        1 2023-05-28 19:22:27.000000 edaplore-0.2.1/edaplore.egg-info/dependency_links.txt
--rw-r--r--   0 maximzabelin   (501) staff       (20)      128 2023-05-28 19:22:27.000000 edaplore-0.2.1/edaplore.egg-info/requires.txt
--rw-r--r--   0 maximzabelin   (501) staff       (20)        1 2023-05-28 19:22:27.000000 edaplore-0.2.1/edaplore.egg-info/top_level.txt
--rw-r--r--   0 maximzabelin   (501) staff       (20)       38 2023-05-28 19:22:27.387490 edaplore-0.2.1/setup.cfg
--rw-r--r--   0 maximzabelin   (501) staff       (20)      594 2023-05-28 19:20:02.000000 edaplore-0.2.1/setup.py
+drwxr-xr-x   0 maximzabelin   (501) staff       (20)        0 2023-05-28 19:36:20.962334 edaplore-0.2.2/
+-rw-r--r--   0 maximzabelin   (501) staff       (20)      215 2023-05-28 19:36:20.962102 edaplore-0.2.2/PKG-INFO
+drwxr-xr-x   0 maximzabelin   (501) staff       (20)        0 2023-05-28 19:36:20.961787 edaplore-0.2.2/edaplore.egg-info/
+-rw-r--r--   0 maximzabelin   (501) staff       (20)      215 2023-05-28 19:36:20.000000 edaplore-0.2.2/edaplore.egg-info/PKG-INFO
+-rw-r--r--   0 maximzabelin   (501) staff       (20)      167 2023-05-28 19:36:20.000000 edaplore-0.2.2/edaplore.egg-info/SOURCES.txt
+-rw-r--r--   0 maximzabelin   (501) staff       (20)        1 2023-05-28 19:36:20.000000 edaplore-0.2.2/edaplore.egg-info/dependency_links.txt
+-rw-r--r--   0 maximzabelin   (501) staff       (20)      128 2023-05-28 19:36:20.000000 edaplore-0.2.2/edaplore.egg-info/requires.txt
+-rw-r--r--   0 maximzabelin   (501) staff       (20)        1 2023-05-28 19:36:20.000000 edaplore-0.2.2/edaplore.egg-info/top_level.txt
+-rw-r--r--   0 maximzabelin   (501) staff       (20)       38 2023-05-28 19:36:20.962399 edaplore-0.2.2/setup.cfg
+-rw-r--r--   0 maximzabelin   (501) staff       (20)      594 2023-05-28 19:36:03.000000 edaplore-0.2.2/setup.py
```

### Comparing `edaplore-0.2.1/setup.py` & `edaplore-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='edaplore',
-    version='0.2.1',
+    version='0.2.2',
     author='Maksim Zabelin',
     author_email='mzabelin8@mail.ru',
     description='EDA helper',
     long_description='',
     license='MIT',
     url='https://github.com/mzabelin8/explore_hse',
     packages=find_packages(),
```

