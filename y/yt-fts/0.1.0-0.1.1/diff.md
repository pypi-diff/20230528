# Comparing `tmp/yt-fts-0.1.0.tar.gz` & `tmp/yt-fts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.0.tar", last modified: Sun May 28 04:01:25 2023, max compression
+gzip compressed data, was "yt-fts-0.1.1.tar", last modified: Sun May 28 04:24:52 2023, max compression
```

## Comparing `yt-fts-0.1.0.tar` & `yt-fts-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:01:25.885560 yt-fts-0.1.0/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 03:53:46.000000 yt-fts-0.1.0/LICENSE
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:01:25.884914 yt-fts-0.1.0/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-28 03:53:46.000000 yt-fts-0.1.0/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 04:01:25.885823 yt-fts-0.1.0/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 03:58:15.000000 yt-fts-0.1.0/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:01:25.880117 yt-fts-0.1.0/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 03:54:10.000000 yt-fts-0.1.0/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-28 03:53:46.000000 yt-fts-0.1.0/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10132 2023-05-28 03:53:46.000000 yt-fts-0.1.0/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:01:25.884104 yt-fts-0.1.0/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      265 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 04:01:25.000000 yt-fts-0.1.0/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.060311 yt-fts-0.1.1/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 03:53:46.000000 yt-fts-0.1.1/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:24:52.059799 yt-fts-0.1.1/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3645 2023-05-28 03:53:46.000000 yt-fts-0.1.1/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 04:24:52.060508 yt-fts-0.1.1/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      811 2023-05-28 04:24:22.000000 yt-fts-0.1.1/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.055588 yt-fts-0.1.1/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 03:54:10.000000 yt-fts-0.1.1/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-28 03:53:46.000000 yt-fts-0.1.1/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10139 2023-05-28 04:21:44.000000 yt-fts-0.1.1/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 04:24:52.059075 yt-fts-0.1.1/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)      502 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      265 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 04:24:52.000000 yt-fts-0.1.1/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.0/LICENSE` & `yt-fts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.0/README.md` & `yt-fts-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.0/setup.py` & `yt-fts-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'console_scripts': [
         'yt_fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.0',
+    version='0.1.1',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
     entry_points=entry_points,
     python_requires='>=3.11',
```

### Comparing `yt-fts-0.1.0/yt_fts/db_scripts.py` & `yt-fts-0.1.1/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.0/yt_fts/yt_fts.py` & `yt-fts-0.1.1/yt_fts/yt_fts.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from concurrent.futures import ThreadPoolExecutor
 
 from bs4 import BeautifulSoup
 import json
 
 
-from db_scripts import * 
+from yt_fts.db_scripts import * 
 
 @click.group()
 def cli():
     make_db()
 
 @click.command(help="Lists channels")
 def list():
```

