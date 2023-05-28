# Comparing `tmp/greenstalk-2.0.1.tar.gz` & `tmp/greenstalk-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenstalk-2.0.1.tar", last modified: Sat May 27 15:20:16 2023, max compression
+gzip compressed data, was "greenstalk-2.0.2.tar", last modified: Sun May 28 11:12:13 2023, max compression
```

## Comparing `greenstalk-2.0.1.tar` & `greenstalk-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/
--rw-r--r--   0 justin    (1000) users      (984)     1057 2023-05-26 15:48:09.000000 greenstalk-2.0.1/LICENSE
--rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-27 15:20:16.169826 greenstalk-2.0.1/PKG-INFO
--rw-r--r--   0 justin    (1000) users      (984)     1018 2023-05-27 15:09:53.000000 greenstalk-2.0.1/README.rst
-drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/greenstalk.egg-info/
--rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/PKG-INFO
--rw-r--r--   0 justin    (1000) users      (984)      206 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/SOURCES.txt
--rw-r--r--   0 justin    (1000) users      (984)        1 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/dependency_links.txt
--rw-r--r--   0 justin    (1000) users      (984)       11 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/top_level.txt
--rw-r--r--   0 justin    (1000) users      (984)       90 2023-05-26 19:54:29.000000 greenstalk-2.0.1/pyproject.toml
--rw-r--r--   0 justin    (1000) users      (984)      810 2023-05-27 15:20:16.169826 greenstalk-2.0.1/setup.cfg
-drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/src/
-drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/src/greenstalk/
--rw-r--r--   0 justin    (1000) users      (984)    15489 2023-05-27 15:09:53.000000 greenstalk-2.0.1/src/greenstalk/__init__.py
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-28 11:12:13.932722 greenstalk-2.0.2/
+-rw-r--r--   0 justin    (1000) users      (984)     1057 2023-05-26 15:48:09.000000 greenstalk-2.0.2/LICENSE
+-rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-28 11:12:13.932722 greenstalk-2.0.2/PKG-INFO
+-rw-r--r--   0 justin    (1000) users      (984)     1018 2023-05-27 15:09:53.000000 greenstalk-2.0.2/README.rst
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-28 11:12:13.932722 greenstalk-2.0.2/greenstalk.egg-info/
+-rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-28 11:12:13.000000 greenstalk-2.0.2/greenstalk.egg-info/PKG-INFO
+-rw-r--r--   0 justin    (1000) users      (984)      206 2023-05-28 11:12:13.000000 greenstalk-2.0.2/greenstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 justin    (1000) users      (984)        1 2023-05-28 11:12:13.000000 greenstalk-2.0.2/greenstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 justin    (1000) users      (984)       11 2023-05-28 11:12:13.000000 greenstalk-2.0.2/greenstalk.egg-info/top_level.txt
+-rw-r--r--   0 justin    (1000) users      (984)       81 2023-05-28 11:04:57.000000 greenstalk-2.0.2/pyproject.toml
+-rw-r--r--   0 justin    (1000) users      (984)      810 2023-05-28 11:12:13.932722 greenstalk-2.0.2/setup.cfg
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-28 11:12:13.932722 greenstalk-2.0.2/src/
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-28 11:12:13.932722 greenstalk-2.0.2/src/greenstalk/
+-rw-r--r--   0 justin    (1000) users      (984)    15489 2023-05-28 11:06:19.000000 greenstalk-2.0.2/src/greenstalk/__init__.py
```

### Comparing `greenstalk-2.0.1/LICENSE` & `greenstalk-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `greenstalk-2.0.1/PKG-INFO` & `greenstalk-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenstalk
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python 3 client for the beanstalkd work queue
 Home-page: https://github.com/justinmayhew/greenstalk
 Author: Justin Mayhew
 Author-email: mayhew@live.ca
 License: MIT
 Project-URL: Documentation, https://greenstalk.readthedocs.io/
 Project-URL: Source, https://github.com/justinmayhew/greenstalk
```

### Comparing `greenstalk-2.0.1/README.rst` & `greenstalk-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `greenstalk-2.0.1/greenstalk.egg-info/PKG-INFO` & `greenstalk-2.0.2/greenstalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenstalk
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python 3 client for the beanstalkd work queue
 Home-page: https://github.com/justinmayhew/greenstalk
 Author: Justin Mayhew
 Author-email: mayhew@live.ca
 License: MIT
 Project-URL: Documentation, https://greenstalk.readthedocs.io/
 Project-URL: Source, https://github.com/justinmayhew/greenstalk
```

### Comparing `greenstalk-2.0.1/setup.cfg` & `greenstalk-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `greenstalk-2.0.1/src/greenstalk/__init__.py` & `greenstalk-2.0.2/src/greenstalk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import socket
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 Address = Union[Tuple[str, int], str]
 Body = Union[bytes, str]
 Stats = Dict[str, Union[str, int]]
 
 DEFAULT_TUBE = "default"
 DEFAULT_PRIORITY = 2**16
```

