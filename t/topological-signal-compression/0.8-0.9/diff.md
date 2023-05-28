# Comparing `tmp/topological-signal-compression-0.8.tar.gz` & `tmp/topological-signal-compression-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topological-signal-compression-0.8.tar", last modified: Wed May 25 14:02:20 2022, max compression
+gzip compressed data, was "topological-signal-compression-0.9.tar", last modified: Wed May 25 14:29:10 2022, max compression
```

## Comparing `topological-signal-compression-0.8.tar` & `topological-signal-compression-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:02:20.514033 topological-signal-compression-0.8/
--rw-rw-rw-   0 root         (0) root         (0)    34472 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4549 2022-05-25 14:02:20.513033 topological-signal-compression-0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4058 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      888 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-25 14:02:20.514033 topological-signal-compression-0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:02:20.510033 topological-signal-compression-0.8/topological_signal_compression.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4549 2022-05-25 14:02:19.000000 topological-signal-compression-0.8/topological_signal_compression.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2022-05-25 14:02:20.000000 topological-signal-compression-0.8/topological_signal_compression.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 14:02:19.000000 topological-signal-compression-0.8/topological_signal_compression.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      177 2022-05-25 14:02:20.000000 topological-signal-compression-0.8/topological_signal_compression.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-05-25 14:02:20.000000 topological-signal-compression-0.8/topological_signal_compression.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:02:20.511033 topological-signal-compression-0.8/tsc/
--rw-rw-rw-   0 root         (0) root         (0)    12140 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:02:20.513033 topological-signal-compression-0.8/tsc/utils/
--rw-rw-rw-   0 root         (0) root         (0)      320 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   160749 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/chopin.mp3
--rw-rw-rw-   0 root         (0) root         (0)     7034 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/compression.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/compression_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/data.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/helper_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     5815 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/reconstruction.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2022-05-25 14:01:58.000000 topological-signal-compression-0.8/tsc/utils/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:29:10.725602 topological-signal-compression-0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    34472 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4549 2022-05-25 14:29:10.724602 topological-signal-compression-0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      888 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-05-25 14:29:10.725602 topological-signal-compression-0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:29:10.713601 topological-signal-compression-0.9/topological_signal_compression.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4549 2022-05-25 14:29:10.000000 topological-signal-compression-0.9/topological_signal_compression.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2022-05-25 14:29:10.000000 topological-signal-compression-0.9/topological_signal_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 14:29:10.000000 topological-signal-compression-0.9/topological_signal_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2022-05-25 14:29:10.000000 topological-signal-compression-0.9/topological_signal_compression.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2022-05-25 14:29:10.000000 topological-signal-compression-0.9/topological_signal_compression.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:29:10.713601 topological-signal-compression-0.9/tsc/
+-rw-rw-rw-   0 root         (0) root         (0)    12140 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 14:29:10.724602 topological-signal-compression-0.9/tsc/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   160749 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/chopin.mp3
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/compression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/compression_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/helper_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5815 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/reconstruction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2022-05-25 14:28:50.000000 topological-signal-compression-0.9/tsc/utils/viz.py
```

### Comparing `topological-signal-compression-0.8/LICENSE` & `topological-signal-compression-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/PKG-INFO` & `topological-signal-compression-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topological-signal-compression
-Version: 0.8
+Version: 0.9
 Summary: Topological Signal Compression
 Author-email: Gary Koplik <gary.koplik@geomdata.com>
 License: GNU AGPL
 Project-URL: Documentation, https://geomdata.gitlab.io/topological-signal-compression/index.html
 Project-URL: Source, https://gitlab.com/geomdata/topological-signal-compression
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `topological-signal-compression-0.8/README.md` & `topological-signal-compression-0.9/README.md`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/pyproject.toml` & `topological-signal-compression-0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "topological-signal-compression"
-version = "0.08"
+version = "0.09"
 authors = [{name="Gary Koplik", email="gary.koplik@geomdata.com"}]
 description = "Topological Signal Compression"
 readme = "README.md"
 license = {text = "GNU AGPL"}
 urls = {Documentation="https://geomdata.gitlab.io/topological-signal-compression/index.html", Source="https://gitlab.com/geomdata/topological-signal-compression" }
 
 dependencies = [
```

### Comparing `topological-signal-compression-0.8/topological_signal_compression.egg-info/PKG-INFO` & `topological-signal-compression-0.9/topological_signal_compression.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topological-signal-compression
-Version: 0.8
+Version: 0.9
 Summary: Topological Signal Compression
 Author-email: Gary Koplik <gary.koplik@geomdata.com>
 License: GNU AGPL
 Project-URL: Documentation, https://geomdata.gitlab.io/topological-signal-compression/index.html
 Project-URL: Source, https://gitlab.com/geomdata/topological-signal-compression
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `topological-signal-compression-0.8/topological_signal_compression.egg-info/SOURCES.txt` & `topological-signal-compression-0.9/topological_signal_compression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/__init__.py` & `topological-signal-compression-0.9/tsc/__init__.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/chopin.mp3` & `topological-signal-compression-0.9/tsc/utils/chopin.mp3`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/compression.py` & `topological-signal-compression-0.9/tsc/utils/compression.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/compression_pipelines.py` & `topological-signal-compression-0.9/tsc/utils/compression_pipelines.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/data.py` & `topological-signal-compression-0.9/tsc/utils/data.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/helper_functions.py` & `topological-signal-compression-0.9/tsc/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/reconstruction.py` & `topological-signal-compression-0.9/tsc/utils/reconstruction.py`

 * *Files identical despite different names*

### Comparing `topological-signal-compression-0.8/tsc/utils/viz.py` & `topological-signal-compression-0.9/tsc/utils/viz.py`

 * *Files identical despite different names*

