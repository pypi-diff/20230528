# Comparing `tmp/mathbib-0.1.0.tar.gz` & `tmp/mathbib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.1.0.tar", last modified: Sun May 28 15:13:05 2023, max compression
+gzip compressed data, was "mathbib-0.1.1.tar", last modified: Sun May 28 15:22:39 2023, max compression
```

## Comparing `mathbib-0.1.0.tar` & `mathbib-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.557053 mathbib-0.1.0/
--rw-r--r--   0 alexrutar   (501) staff       (20)       51 2023-05-25 15:29:52.000000 mathbib-0.1.0/MANIFEST.in
--rw-r--r--   0 alexrutar   (501) staff       (20)     5808 2023-05-28 15:13:05.557325 mathbib-0.1.0/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     5347 2023-05-28 15:00:10.000000 mathbib-0.1.0/README.md
--rw-r--r--   0 alexrutar   (501) staff       (20)      318 2023-05-10 21:34:37.000000 mathbib-0.1.0/pyproject.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)     1023 2023-05-28 15:13:05.558134 mathbib-0.1.0/setup.cfg
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.540100 mathbib-0.1.0/src/
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.546525 mathbib-0.1.0/src/mathbib/
--rw-r--r--   0 alexrutar   (501) staff       (20)      217 2023-05-10 21:29:36.000000 mathbib-0.1.0/src/mathbib/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 21:47:55.000000 mathbib-0.1.0/src/mathbib/__main__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1402 2023-05-28 11:08:27.000000 mathbib-0.1.0/src/mathbib/bibtex.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2724 2023-05-28 10:46:08.000000 mathbib-0.1.0/src/mathbib/citegen.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9508 2023-05-28 15:04:27.000000 mathbib-0.1.0/src/mathbib/command.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2632 2023-05-28 15:08:09.000000 mathbib-0.1.0/src/mathbib/partition.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9459 2023-05-28 15:11:22.000000 mathbib-0.1.0/src/mathbib/record.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.553439 mathbib-0.1.0/src/mathbib/remote/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5481 2023-05-28 13:40:33.000000 mathbib-0.1.0/src/mathbib/remote/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     3088 2023-05-28 12:38:27.000000 mathbib-0.1.0/src/mathbib/remote/arxiv.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      923 2023-05-27 20:04:18.000000 mathbib-0.1.0/src/mathbib/remote/doi.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      855 2023-05-28 09:33:03.000000 mathbib-0.1.0/src/mathbib/remote/error.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1475 2023-05-27 20:04:18.000000 mathbib-0.1.0/src/mathbib/remote/isbn.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1194 2023-05-27 18:35:57.000000 mathbib-0.1.0/src/mathbib/remote/ol.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     4257 2023-05-28 15:10:12.000000 mathbib-0.1.0/src/mathbib/remote/utils.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      597 2023-05-25 12:11:18.000000 mathbib-0.1.0/src/mathbib/remote/zbl.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1816 2023-05-28 12:19:04.000000 mathbib-0.1.0/src/mathbib/remote/zbmath.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5552 2023-05-28 12:31:57.000000 mathbib-0.1.0/src/mathbib/request.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.554034 mathbib-0.1.0/src/mathbib/resources/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2023-05-25 15:24:07.000000 mathbib-0.1.0/src/mathbib/resources/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)   270192 2023-05-25 15:19:42.000000 mathbib-0.1.0/src/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0 alexrutar   (501) staff       (20)     2613 2023-05-28 12:14:16.000000 mathbib-0.1.0/src/mathbib/session.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      705 2023-05-25 11:53:39.000000 mathbib-0.1.0/src/mathbib/term.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.548794 mathbib-0.1.0/src/mathbib.egg-info/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5808 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)      835 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/SOURCES.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/dependency_links.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       45 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/entry_points.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)      131 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/requires.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        8 2023-05-28 15:13:05.000000 mathbib-0.1.0/src/mathbib.egg-info/top_level.txt
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:13:05.556241 mathbib-0.1.0/test/
--rw-r--r--   0 alexrutar   (501) staff       (20)      719 2023-05-27 20:04:18.000000 mathbib-0.1.0/test/test_partition.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.768019 mathbib-0.1.1/
+-rw-r--r--   0 alexrutar   (501) staff       (20)       51 2023-05-25 15:29:52.000000 mathbib-0.1.1/MANIFEST.in
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5814 2023-05-28 15:22:39.768324 mathbib-0.1.1/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5353 2023-05-28 15:17:21.000000 mathbib-0.1.1/README.md
+-rw-r--r--   0 alexrutar   (501) staff       (20)      318 2023-05-10 21:34:37.000000 mathbib-0.1.1/pyproject.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1023 2023-05-28 15:22:39.769498 mathbib-0.1.1/setup.cfg
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.749239 mathbib-0.1.1/src/
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.755195 mathbib-0.1.1/src/mathbib/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      217 2023-05-28 15:22:00.000000 mathbib-0.1.1/src/mathbib/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 21:47:55.000000 mathbib-0.1.1/src/mathbib/__main__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1402 2023-05-28 11:08:27.000000 mathbib-0.1.1/src/mathbib/bibtex.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2724 2023-05-28 10:46:08.000000 mathbib-0.1.1/src/mathbib/citegen.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     9508 2023-05-28 15:04:27.000000 mathbib-0.1.1/src/mathbib/command.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2632 2023-05-28 15:08:09.000000 mathbib-0.1.1/src/mathbib/partition.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     9459 2023-05-28 15:11:22.000000 mathbib-0.1.1/src/mathbib/record.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.762960 mathbib-0.1.1/src/mathbib/remote/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5481 2023-05-28 13:40:33.000000 mathbib-0.1.1/src/mathbib/remote/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     3088 2023-05-28 12:38:27.000000 mathbib-0.1.1/src/mathbib/remote/arxiv.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      923 2023-05-27 20:04:18.000000 mathbib-0.1.1/src/mathbib/remote/doi.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      855 2023-05-28 09:33:03.000000 mathbib-0.1.1/src/mathbib/remote/error.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1475 2023-05-27 20:04:18.000000 mathbib-0.1.1/src/mathbib/remote/isbn.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1194 2023-05-27 18:35:57.000000 mathbib-0.1.1/src/mathbib/remote/ol.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4257 2023-05-28 15:10:12.000000 mathbib-0.1.1/src/mathbib/remote/utils.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      597 2023-05-25 12:11:18.000000 mathbib-0.1.1/src/mathbib/remote/zbl.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1816 2023-05-28 12:19:04.000000 mathbib-0.1.1/src/mathbib/remote/zbmath.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5552 2023-05-28 12:31:57.000000 mathbib-0.1.1/src/mathbib/request.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.763962 mathbib-0.1.1/src/mathbib/resources/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2023-05-25 15:24:07.000000 mathbib-0.1.1/src/mathbib/resources/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)   270192 2023-05-25 15:19:42.000000 mathbib-0.1.1/src/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2613 2023-05-28 12:14:16.000000 mathbib-0.1.1/src/mathbib/session.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      705 2023-05-25 11:53:39.000000 mathbib-0.1.1/src/mathbib/term.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.758198 mathbib-0.1.1/src/mathbib.egg-info/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5814 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)      835 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/SOURCES.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/dependency_links.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       45 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/entry_points.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)      131 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/requires.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        8 2023-05-28 15:22:39.000000 mathbib-0.1.1/src/mathbib.egg-info/top_level.txt
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:22:39.766911 mathbib-0.1.1/test/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      719 2023-05-27 20:04:18.000000 mathbib-0.1.1/test/test_partition.py
```

### Comparing `mathbib-0.1.0/PKG-INFO` & `mathbib-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 
 # MathBib
 MathBib is a mathematics BibLaTeX bibliography manager.
-Jump to:
-- [Installation and basic usage](#installation-and-basic-usage)
-- [Finer details](#some-finer-details)
+
+**WARNING: MathBib is currently in alpha state. The API and other implementation details may change substantially!**
 
 ## Installation and basic usage
 First, ensure that `mbib` is installed with
 ```sh
 pip install mathbib
 ```
 This installs the `mbib` command-line interface.
```

### Comparing `mathbib-0.1.0/README.md` & `mathbib-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # MathBib
 MathBib is a mathematics BibLaTeX bibliography manager.
-Jump to:
-- [Installation and basic usage](#installation-and-basic-usage)
-- [Finer details](#some-finer-details)
+
+**WARNING: MathBib is currently in alpha state. The API and other implementation details may change substantially!**
 
 ## Installation and basic usage
 First, ensure that `mbib` is installed with
 ```sh
 pip install mathbib
 ```
 This installs the `mbib` command-line interface.
```

### Comparing `mathbib-0.1.0/setup.cfg` & `mathbib-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/bibtex.py` & `mathbib-0.1.1/src/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/citegen.py` & `mathbib-0.1.1/src/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/command.py` & `mathbib-0.1.1/src/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/partition.py` & `mathbib-0.1.1/src/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/record.py` & `mathbib-0.1.1/src/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/__init__.py` & `mathbib-0.1.1/src/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/arxiv.py` & `mathbib-0.1.1/src/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/doi.py` & `mathbib-0.1.1/src/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/error.py` & `mathbib-0.1.1/src/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/isbn.py` & `mathbib-0.1.1/src/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/ol.py` & `mathbib-0.1.1/src/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/utils.py` & `mathbib-0.1.1/src/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/zbl.py` & `mathbib-0.1.1/src/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/remote/zbmath.py` & `mathbib-0.1.1/src/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/request.py` & `mathbib-0.1.1/src/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/resources/journal_abbrevs.json` & `mathbib-0.1.1/src/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/session.py` & `mathbib-0.1.1/src/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib/term.py` & `mathbib-0.1.1/src/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/src/mathbib.egg-info/PKG-INFO` & `mathbib-0.1.1/src/mathbib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 
 # MathBib
 MathBib is a mathematics BibLaTeX bibliography manager.
-Jump to:
-- [Installation and basic usage](#installation-and-basic-usage)
-- [Finer details](#some-finer-details)
+
+**WARNING: MathBib is currently in alpha state. The API and other implementation details may change substantially!**
 
 ## Installation and basic usage
 First, ensure that `mbib` is installed with
 ```sh
 pip install mathbib
 ```
 This installs the `mbib` command-line interface.
```

### Comparing `mathbib-0.1.0/src/mathbib.egg-info/SOURCES.txt` & `mathbib-0.1.1/src/mathbib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.0/test/test_partition.py` & `mathbib-0.1.1/test/test_partition.py`

 * *Files identical despite different names*

