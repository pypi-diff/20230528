# Comparing `tmp/IMDBTraktSyncer-1.3.2.tar.gz` & `tmp/IMDBTraktSyncer-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.2.tar", last modified: Fri May 26 22:09:11 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.3.tar", last modified: Sun May 28 12:24:59 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.2.tar` & `IMDBTraktSyncer-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.047336 IMDBTraktSyncer-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.015326 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    22309 2023-05-25 05:33:53.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-05-26 22:03:46.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-25 05:26:36.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.044336 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     8573 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     8573 2023-05-26 22:09:11.046325 IMDBTraktSyncer-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     7856 2023-05-25 05:31:18.000000 IMDBTraktSyncer-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 22:09:11.047336 IMDBTraktSyncer-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-05-26 22:04:29.000000 IMDBTraktSyncer-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:24:59.523856 IMDBTraktSyncer-1.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-28 12:24:59.491582 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    22309 2023-05-25 05:33:53.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     3706 2023-05-28 12:21:24.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:24:59.520851 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11969 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 12:24:59.000000 IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0    11969 2023-05-28 12:24:59.522842 IMDBTraktSyncer-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11226 2023-05-28 12:23:51.000000 IMDBTraktSyncer-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:24:59.524842 IMDBTraktSyncer-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-05-28 12:23:42.000000 IMDBTraktSyncer-1.3.3/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.3/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/LICENSE` & `IMDBTraktSyncer-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.2/setup.py` & `IMDBTraktSyncer-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.2'
+VERSION = '1.3.3'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

