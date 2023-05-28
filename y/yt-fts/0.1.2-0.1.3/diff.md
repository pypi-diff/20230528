# Comparing `tmp/yt-fts-0.1.2.tar.gz` & `tmp/yt-fts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.2.tar", last modified: Sun May 28 07:05:41 2023, max compression
+gzip compressed data, was "yt-fts-0.1.3.tar", last modified: Sun May 28 07:15:42 2023, max compression
```

## Comparing `yt-fts-0.1.2.tar` & `yt-fts-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.975672 yt-fts-0.1.2/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-27 17:44:26.000000 yt-fts-0.1.2/LICENSE
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:05:41.975318 yt-fts-0.1.2/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-27 17:58:18.000000 yt-fts-0.1.2/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 07:05:41.975814 yt-fts-0.1.2/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 06:59:51.000000 yt-fts-0.1.2/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.971634 yt-fts-0.1.2/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 06:29:11.000000 yt-fts-0.1.2/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 06:34:41.000000 yt-fts-0.1.2/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-27 17:35:08.000000 yt-fts-0.1.2/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 06:49:46.000000 yt-fts-0.1.2/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:05:41.974653 yt-fts-0.1.2/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 07:05:41.000000 yt-fts-0.1.2/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.741631 yt-fts-0.1.3/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-27 17:44:26.000000 yt-fts-0.1.3/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:15:42.740894 yt-fts-0.1.3/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-27 17:58:18.000000 yt-fts-0.1.3/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 07:15:42.741805 yt-fts-0.1.3/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 07:15:36.000000 yt-fts-0.1.3/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.735995 yt-fts-0.1.3/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 06:29:11.000000 yt-fts-0.1.3/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 06:34:41.000000 yt-fts-0.1.3/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-27 17:35:08.000000 yt-fts-0.1.3/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 06:49:46.000000 yt-fts-0.1.3/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 07:15:42.739908 yt-fts-0.1.3/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 07:15:42.000000 yt-fts-0.1.3/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.2/LICENSE` & `yt-fts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.2/README.md` & `yt-fts-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.2/setup.py` & `yt-fts-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     dependencies = f.read().splitlines()
 
 entry_points = {
     'console_scripts': [
-        'yt_fts=yt_fts.yt_fts:cli',
+        'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.2',
+    version='0.1.3',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
     entry_points=entry_points,
     python_requires='>=3.11',
```

### Comparing `yt-fts-0.1.2/yt_fts/db_scripts.py` & `yt-fts-0.1.3/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.2/yt_fts/yt_fts.py` & `yt-fts-0.1.3/yt_fts/yt_fts.py`

 * *Files identical despite different names*

