# Comparing `tmp/pyGachi-1.0a4.tar.gz` & `tmp/pyGachi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGachi-1.0a4.tar", last modified: Mon May 22 14:58:58 2023, max compression
+gzip compressed data, was "pyGachi-1.1.tar", last modified: Sun May 28 11:23:04 2023, max compression
```

## Comparing `pyGachi-1.0a4.tar` & `pyGachi-1.1.tar`

### file list

```diff
@@ -1,24 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:58:58.531552 pyGachi-1.0a4/
--rw-rw-rw-   0        0        0     1031 2023-05-22 14:58:58.531552 pyGachi-1.0a4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 14:58:58.518552 pyGachi-1.0a4/pyGachi/
--rw-rw-rw-   0        0        0      452 2023-05-22 14:58:50.000000 pyGachi-1.0a4/pyGachi/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-05-22 14:02:51.000000 pyGachi-1.0a4/pyGachi/bd1.py
--rw-rw-rw-   0        0        0     3347 2023-05-22 14:02:53.000000 pyGachi-1.0a4/pyGachi/bd2.py
--rw-rw-rw-   0        0        0     3058 2023-05-22 14:02:53.000000 pyGachi-1.0a4/pyGachi/oop1.py
--rw-rw-rw-   0        0        0     2639 2023-05-22 14:02:54.000000 pyGachi-1.0a4/pyGachi/oop2.py
--rw-rw-rw-   0        0        0      723 2023-05-22 14:02:55.000000 pyGachi-1.0a4/pyGachi/prog1.py
--rw-rw-rw-   0        0        0     1042 2023-05-22 14:02:55.000000 pyGachi-1.0a4/pyGachi/prog2.py
--rw-rw-rw-   0        0        0      333 2023-05-22 14:02:58.000000 pyGachi-1.0a4/pyGachi/prog3.py
--rw-rw-rw-   0        0        0      490 2023-05-22 14:02:59.000000 pyGachi-1.0a4/pyGachi/prog4.py
--rw-rw-rw-   0        0        0     2257 2023-05-22 14:03:00.000000 pyGachi-1.0a4/pyGachi/prog5.py
--rw-rw-rw-   0        0        0      809 2023-05-22 14:03:00.000000 pyGachi-1.0a4/pyGachi/siaod1.py
--rw-rw-rw-   0        0        0     3002 2023-05-22 14:03:01.000000 pyGachi-1.0a4/pyGachi/siaod2.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:58:58.530552 pyGachi-1.0a4/pyGachi.egg-info/
--rw-rw-rw-   0        0        0   139264 2023-05-22 14:44:53.000000 pyGachi-1.0a4/pyGachi.egg-info/FAQ.docx
--rw-rw-rw-   0        0        0     1031 2023-05-22 14:58:58.000000 pyGachi-1.0a4/pyGachi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-05-22 14:58:58.000000 pyGachi-1.0a4/pyGachi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:58:58.000000 pyGachi-1.0a4/pyGachi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 14:58:58.000000 pyGachi-1.0a4/pyGachi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 14:58:58.000000 pyGachi-1.0a4/pyGachi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:58:58.532552 pyGachi-1.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-05-22 14:58:53.000000 pyGachi-1.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.967080 pyGachi-1.1/
+-rw-rw-rw-   0        0        0     1027 2023-05-28 11:23:04.967080 pyGachi-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.946103 pyGachi-1.1/pyGachi/
+-rw-rw-rw-   0        0        0      450 2023-05-28 11:19:48.000000 pyGachi-1.1/pyGachi/__init__.py
+-rw-rw-rw-   0        0        0     3654 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/bd1.py
+-rw-rw-rw-   0        0        0     3347 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/bd2.py
+-rw-rw-rw-   0        0        0     1310 2023-05-27 12:40:52.000000 pyGachi-1.1/pyGachi/gosBel_3.py
+-rw-rw-rw-   0        0        0     3058 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/oop1.py
+-rw-rw-rw-   0        0        0     2639 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/oop2.py
+-rw-rw-rw-   0        0        0      968 2023-05-27 12:41:35.000000 pyGachi-1.1/pyGachi/prog1.py
+-rw-rw-rw-   0        0        0      237 2023-05-27 12:41:34.000000 pyGachi-1.1/pyGachi/prog10.py
+-rw-rw-rw-   0        0        0      107 2023-05-27 12:41:38.000000 pyGachi-1.1/pyGachi/prog11.py
+-rw-rw-rw-   0        0        0     1039 2023-05-27 12:40:54.000000 pyGachi-1.1/pyGachi/prog12.py
+-rw-rw-rw-   0        0        0       84 2023-05-27 12:41:41.000000 pyGachi-1.1/pyGachi/prog13.py
+-rw-rw-rw-   0        0        0      695 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog14.py
+-rw-rw-rw-   0        0        0      247 2023-05-27 12:41:40.000000 pyGachi-1.1/pyGachi/prog15.py
+-rw-rw-rw-   0        0        0      877 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog16.py
+-rw-rw-rw-   0        0        0     1103 2023-05-27 12:41:39.000000 pyGachi-1.1/pyGachi/prog17.py
+-rw-rw-rw-   0        0        0      488 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog18.py
+-rw-rw-rw-   0        0        0      301 2023-05-27 12:41:38.000000 pyGachi-1.1/pyGachi/prog19.py
+-rw-rw-rw-   0        0        0      139 2023-05-27 12:41:35.000000 pyGachi-1.1/pyGachi/prog2.py
+-rw-rw-rw-   0        0        0      337 2023-05-27 12:40:52.000000 pyGachi-1.1/pyGachi/prog20.py
+-rw-rw-rw-   0        0        0      272 2023-05-27 12:41:37.000000 pyGachi-1.1/pyGachi/prog3.py
+-rw-rw-rw-   0        0        0      393 2023-05-27 12:41:36.000000 pyGachi-1.1/pyGachi/prog4.py
+-rw-rw-rw-   0        0        0      168 2023-05-27 12:41:30.000000 pyGachi-1.1/pyGachi/prog5.py
+-rw-rw-rw-   0        0        0     1787 2023-05-27 12:41:31.000000 pyGachi-1.1/pyGachi/prog6.py
+-rw-rw-rw-   0        0        0     2607 2023-05-27 12:41:32.000000 pyGachi-1.1/pyGachi/prog7.py
+-rw-rw-rw-   0        0        0     2449 2023-05-27 12:41:33.000000 pyGachi-1.1/pyGachi/prog8.py
+-rw-rw-rw-   0        0        0      503 2023-05-27 12:41:33.000000 pyGachi-1.1/pyGachi/prog9.py
+-rw-rw-rw-   0        0        0      809 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/siaod1.py
+-rw-rw-rw-   0        0        0     3002 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/siaod2.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.966081 pyGachi-1.1/pyGachi.egg-info/
+-rw-rw-rw-   0        0        0  1081344 2023-05-27 18:56:25.000000 pyGachi-1.1/pyGachi.egg-info/FAQ.docx
+-rw-rw-rw-   0        0        0     1027 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0   471040 2023-05-27 18:53:56.000000 pyGachi-1.1/pyGachi.egg-info/Z_1.accdb
+-rw-rw-rw-   0        0        0   507904 2023-05-27 18:58:53.000000 pyGachi-1.1/pyGachi.egg-info/Z_2.accdb
+-rw-rw-rw-   0        0        0   425984 2023-05-27 19:06:43.000000 pyGachi-1.1/pyGachi.egg-info/Z_3.accdb
+-rw-rw-rw-   0        0        0   430080 2023-05-27 19:16:48.000000 pyGachi-1.1/pyGachi.egg-info/Z_4.accdb
+-rw-rw-rw-   0        0        0   462848 2023-05-27 19:26:18.000000 pyGachi-1.1/pyGachi.egg-info/Z_5.accdb
+-rw-rw-rw-   0        0        0   421888 2023-05-27 19:38:25.000000 pyGachi-1.1/pyGachi.egg-info/Z_6.accdb
+-rw-rw-rw-   0        0        0   450560 2023-05-27 19:49:08.000000 pyGachi-1.1/pyGachi.egg-info/Z_7.accdb
+-rw-rw-rw-   0        0        0   438272 2023-05-27 19:59:15.000000 pyGachi-1.1/pyGachi.egg-info/Z_8.accdb
+-rw-rw-rw-   0        0        0   450560 2023-05-27 20:07:17.000000 pyGachi-1.1/pyGachi.egg-info/Z_9.accdb
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0   181760 2023-05-28 11:21:19.000000 pyGachi-1.1/pyGachi.egg-info/license.docx
+-rw-rw-rw-   0        0        0       17 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:23:04.968079 pyGachi-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1311 2023-05-28 11:19:51.000000 pyGachi-1.1/setup.py
```

### Comparing `pyGachi-1.0a4/PKG-INFO` & `pyGachi-1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.0a4
+Version: 1.1
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a4.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.1.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.0a4/pyGachi/bd1.py` & `pyGachi-1.1/pyGachi/bd1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi/bd2.py` & `pyGachi-1.1/pyGachi/bd2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi/oop1.py` & `pyGachi-1.1/pyGachi/oop1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi/oop2.py` & `pyGachi-1.1/pyGachi/oop2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi/siaod1.py` & `pyGachi-1.1/pyGachi/siaod1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi/siaod2.py` & `pyGachi-1.1/pyGachi/siaod2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.0a4/pyGachi.egg-info/PKG-INFO` & `pyGachi-1.1/pyGachi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.0a4
+Version: 1.1
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.0a4.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.1.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.0a4/setup.py` & `pyGachi-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup
 
-version = '1.0a4'
+version = '1.1'
 
 setup(
     name='pyGachi',
     author='GachiParty',
 
     version=version,
     author_email='fetom30268@cutefier.com',
```

