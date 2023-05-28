# Comparing `tmp/pyGachi-1.1.tar.gz` & `tmp/pyGachi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGachi-1.1.tar", last modified: Sun May 28 11:23:04 2023, max compression
+gzip compressed data, was "pyGachi-1.2.tar", last modified: Sun May 28 11:27:30 2023, max compression
```

## Comparing `pyGachi-1.1.tar` & `pyGachi-1.2.tar`

### file list

```diff
@@ -1,50 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.967080 pyGachi-1.1/
--rw-rw-rw-   0        0        0     1027 2023-05-28 11:23:04.967080 pyGachi-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.946103 pyGachi-1.1/pyGachi/
--rw-rw-rw-   0        0        0      450 2023-05-28 11:19:48.000000 pyGachi-1.1/pyGachi/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/bd1.py
--rw-rw-rw-   0        0        0     3347 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/bd2.py
--rw-rw-rw-   0        0        0     1310 2023-05-27 12:40:52.000000 pyGachi-1.1/pyGachi/gosBel_3.py
--rw-rw-rw-   0        0        0     3058 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/oop1.py
--rw-rw-rw-   0        0        0     2639 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/oop2.py
--rw-rw-rw-   0        0        0      968 2023-05-27 12:41:35.000000 pyGachi-1.1/pyGachi/prog1.py
--rw-rw-rw-   0        0        0      237 2023-05-27 12:41:34.000000 pyGachi-1.1/pyGachi/prog10.py
--rw-rw-rw-   0        0        0      107 2023-05-27 12:41:38.000000 pyGachi-1.1/pyGachi/prog11.py
--rw-rw-rw-   0        0        0     1039 2023-05-27 12:40:54.000000 pyGachi-1.1/pyGachi/prog12.py
--rw-rw-rw-   0        0        0       84 2023-05-27 12:41:41.000000 pyGachi-1.1/pyGachi/prog13.py
--rw-rw-rw-   0        0        0      695 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog14.py
--rw-rw-rw-   0        0        0      247 2023-05-27 12:41:40.000000 pyGachi-1.1/pyGachi/prog15.py
--rw-rw-rw-   0        0        0      877 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog16.py
--rw-rw-rw-   0        0        0     1103 2023-05-27 12:41:39.000000 pyGachi-1.1/pyGachi/prog17.py
--rw-rw-rw-   0        0        0      488 2023-05-27 12:40:53.000000 pyGachi-1.1/pyGachi/prog18.py
--rw-rw-rw-   0        0        0      301 2023-05-27 12:41:38.000000 pyGachi-1.1/pyGachi/prog19.py
--rw-rw-rw-   0        0        0      139 2023-05-27 12:41:35.000000 pyGachi-1.1/pyGachi/prog2.py
--rw-rw-rw-   0        0        0      337 2023-05-27 12:40:52.000000 pyGachi-1.1/pyGachi/prog20.py
--rw-rw-rw-   0        0        0      272 2023-05-27 12:41:37.000000 pyGachi-1.1/pyGachi/prog3.py
--rw-rw-rw-   0        0        0      393 2023-05-27 12:41:36.000000 pyGachi-1.1/pyGachi/prog4.py
--rw-rw-rw-   0        0        0      168 2023-05-27 12:41:30.000000 pyGachi-1.1/pyGachi/prog5.py
--rw-rw-rw-   0        0        0     1787 2023-05-27 12:41:31.000000 pyGachi-1.1/pyGachi/prog6.py
--rw-rw-rw-   0        0        0     2607 2023-05-27 12:41:32.000000 pyGachi-1.1/pyGachi/prog7.py
--rw-rw-rw-   0        0        0     2449 2023-05-27 12:41:33.000000 pyGachi-1.1/pyGachi/prog8.py
--rw-rw-rw-   0        0        0      503 2023-05-27 12:41:33.000000 pyGachi-1.1/pyGachi/prog9.py
--rw-rw-rw-   0        0        0      809 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/siaod1.py
--rw-rw-rw-   0        0        0     3002 2023-05-22 15:01:09.000000 pyGachi-1.1/pyGachi/siaod2.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:23:04.966081 pyGachi-1.1/pyGachi.egg-info/
--rw-rw-rw-   0        0        0  1081344 2023-05-27 18:56:25.000000 pyGachi-1.1/pyGachi.egg-info/FAQ.docx
--rw-rw-rw-   0        0        0     1027 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      960 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0   471040 2023-05-27 18:53:56.000000 pyGachi-1.1/pyGachi.egg-info/Z_1.accdb
--rw-rw-rw-   0        0        0   507904 2023-05-27 18:58:53.000000 pyGachi-1.1/pyGachi.egg-info/Z_2.accdb
--rw-rw-rw-   0        0        0   425984 2023-05-27 19:06:43.000000 pyGachi-1.1/pyGachi.egg-info/Z_3.accdb
--rw-rw-rw-   0        0        0   430080 2023-05-27 19:16:48.000000 pyGachi-1.1/pyGachi.egg-info/Z_4.accdb
--rw-rw-rw-   0        0        0   462848 2023-05-27 19:26:18.000000 pyGachi-1.1/pyGachi.egg-info/Z_5.accdb
--rw-rw-rw-   0        0        0   421888 2023-05-27 19:38:25.000000 pyGachi-1.1/pyGachi.egg-info/Z_6.accdb
--rw-rw-rw-   0        0        0   450560 2023-05-27 19:49:08.000000 pyGachi-1.1/pyGachi.egg-info/Z_7.accdb
--rw-rw-rw-   0        0        0   438272 2023-05-27 19:59:15.000000 pyGachi-1.1/pyGachi.egg-info/Z_8.accdb
--rw-rw-rw-   0        0        0   450560 2023-05-27 20:07:17.000000 pyGachi-1.1/pyGachi.egg-info/Z_9.accdb
--rw-rw-rw-   0        0        0        1 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0   181760 2023-05-28 11:21:19.000000 pyGachi-1.1/pyGachi.egg-info/license.docx
--rw-rw-rw-   0        0        0       17 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 11:23:04.000000 pyGachi-1.1/pyGachi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 11:23:04.968079 pyGachi-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1311 2023-05-28 11:19:51.000000 pyGachi-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:27:30.900207 pyGachi-1.2/
+-rw-rw-rw-   0        0        0     1027 2023-05-28 11:27:30.900207 pyGachi-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 11:27:30.871208 pyGachi-1.2/pyGachi/
+-rw-rw-rw-   0        0        0      450 2023-05-28 11:27:07.000000 pyGachi-1.2/pyGachi/__init__.py
+-rw-rw-rw-   0        0        0     3654 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/bd1.py
+-rw-rw-rw-   0        0        0     3347 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/bd2.py
+-rw-rw-rw-   0        0        0     1310 2023-05-27 12:40:52.000000 pyGachi-1.2/pyGachi/gosBel_3.py
+-rw-rw-rw-   0        0        0     3058 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/oop1.py
+-rw-rw-rw-   0        0        0     2639 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/oop2.py
+-rw-rw-rw-   0        0        0      968 2023-05-27 12:41:35.000000 pyGachi-1.2/pyGachi/prog1.py
+-rw-rw-rw-   0        0        0      237 2023-05-27 12:41:34.000000 pyGachi-1.2/pyGachi/prog10.py
+-rw-rw-rw-   0        0        0      107 2023-05-27 12:41:38.000000 pyGachi-1.2/pyGachi/prog11.py
+-rw-rw-rw-   0        0        0     1039 2023-05-27 12:40:54.000000 pyGachi-1.2/pyGachi/prog12.py
+-rw-rw-rw-   0        0        0       84 2023-05-27 12:41:41.000000 pyGachi-1.2/pyGachi/prog13.py
+-rw-rw-rw-   0        0        0      695 2023-05-27 12:40:53.000000 pyGachi-1.2/pyGachi/prog14.py
+-rw-rw-rw-   0        0        0      247 2023-05-27 12:41:40.000000 pyGachi-1.2/pyGachi/prog15.py
+-rw-rw-rw-   0        0        0      877 2023-05-27 12:40:53.000000 pyGachi-1.2/pyGachi/prog16.py
+-rw-rw-rw-   0        0        0     1103 2023-05-27 12:41:39.000000 pyGachi-1.2/pyGachi/prog17.py
+-rw-rw-rw-   0        0        0      488 2023-05-27 12:40:53.000000 pyGachi-1.2/pyGachi/prog18.py
+-rw-rw-rw-   0        0        0      301 2023-05-27 12:41:38.000000 pyGachi-1.2/pyGachi/prog19.py
+-rw-rw-rw-   0        0        0      139 2023-05-27 12:41:35.000000 pyGachi-1.2/pyGachi/prog2.py
+-rw-rw-rw-   0        0        0      337 2023-05-27 12:40:52.000000 pyGachi-1.2/pyGachi/prog20.py
+-rw-rw-rw-   0        0        0      272 2023-05-27 12:41:37.000000 pyGachi-1.2/pyGachi/prog3.py
+-rw-rw-rw-   0        0        0      393 2023-05-27 12:41:36.000000 pyGachi-1.2/pyGachi/prog4.py
+-rw-rw-rw-   0        0        0      168 2023-05-27 12:41:30.000000 pyGachi-1.2/pyGachi/prog5.py
+-rw-rw-rw-   0        0        0     1787 2023-05-27 12:41:31.000000 pyGachi-1.2/pyGachi/prog6.py
+-rw-rw-rw-   0        0        0     2607 2023-05-27 12:41:32.000000 pyGachi-1.2/pyGachi/prog7.py
+-rw-rw-rw-   0        0        0     2449 2023-05-27 12:41:33.000000 pyGachi-1.2/pyGachi/prog8.py
+-rw-rw-rw-   0        0        0      503 2023-05-27 12:41:33.000000 pyGachi-1.2/pyGachi/prog9.py
+-rw-rw-rw-   0        0        0      809 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/siaod1.py
+-rw-rw-rw-   0        0        0     3002 2023-05-22 15:01:09.000000 pyGachi-1.2/pyGachi/siaod2.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:27:30.881207 pyGachi-1.2/pyGachi.egg-info/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:27:30.899207 pyGachi-1.2/pyGachi.egg-info/Files/
+-rw-rw-rw-   0        0        0  1081344 2023-05-27 18:56:25.000000 pyGachi-1.2/pyGachi.egg-info/Files/FAQ.docx
+-rw-rw-rw-   0        0        0    36317 2023-05-27 12:34:54.000000 pyGachi-1.2/pyGachi.egg-info/Files/SoundBox.unitypackage
+-rw-rw-rw-   0        0        0   471040 2023-05-27 18:53:56.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_1.accdb
+-rw-rw-rw-   0        0        0   507904 2023-05-27 18:58:53.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_2.accdb
+-rw-rw-rw-   0        0        0   425984 2023-05-27 19:06:43.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_3.accdb
+-rw-rw-rw-   0        0        0   430080 2023-05-27 19:16:48.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_4.accdb
+-rw-rw-rw-   0        0        0   462848 2023-05-27 19:26:18.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_5.accdb
+-rw-rw-rw-   0        0        0   421888 2023-05-27 19:38:25.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_6.accdb
+-rw-rw-rw-   0        0        0   450560 2023-05-27 19:49:08.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_7.accdb
+-rw-rw-rw-   0        0        0   438272 2023-05-27 19:59:15.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_8.accdb
+-rw-rw-rw-   0        0        0   450560 2023-05-27 20:07:17.000000 pyGachi-1.2/pyGachi.egg-info/Files/Z_9.accdb
+-rw-rw-rw-   0        0        0      372 2023-05-27 12:40:14.000000 pyGachi-1.2/pyGachi.egg-info/Files/book1.txt
+-rw-rw-rw-   0        0        0    73085 2023-05-24 12:18:33.000000 pyGachi-1.2/pyGachi.egg-info/Files/collisions.unitypackage
+-rw-rw-rw-   0        0        0       72 2023-05-27 12:40:14.000000 pyGachi-1.2/pyGachi.egg-info/Files/grades.txt
+-rw-rw-rw-   0        0        0   181760 2023-05-28 11:21:19.000000 pyGachi-1.2/pyGachi.egg-info/Files/license.docx
+-rw-rw-rw-   0        0        0     1027 2023-05-28 11:27:30.000000 pyGachi-1.2/pyGachi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1185 2023-05-28 11:27:30.000000 pyGachi-1.2/pyGachi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:27:30.000000 pyGachi-1.2/pyGachi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 11:27:30.000000 pyGachi-1.2/pyGachi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 11:27:30.000000 pyGachi-1.2/pyGachi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:27:30.900207 pyGachi-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1311 2023-05-28 11:27:04.000000 pyGachi-1.2/setup.py
```

### Comparing `pyGachi-1.1/PKG-INFO` & `pyGachi-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.1
+Version: 1.2
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.1.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.2.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.1/pyGachi/bd1.py` & `pyGachi-1.2/pyGachi/bd1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/bd2.py` & `pyGachi-1.2/pyGachi/bd2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/gosBel_3.py` & `pyGachi-1.2/pyGachi/gosBel_3.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/oop1.py` & `pyGachi-1.2/pyGachi/oop1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/oop2.py` & `pyGachi-1.2/pyGachi/oop2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog1.py` & `pyGachi-1.2/pyGachi/prog1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog12.py` & `pyGachi-1.2/pyGachi/prog12.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog14.py` & `pyGachi-1.2/pyGachi/prog14.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog16.py` & `pyGachi-1.2/pyGachi/prog16.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog17.py` & `pyGachi-1.2/pyGachi/prog17.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog6.py` & `pyGachi-1.2/pyGachi/prog6.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog7.py` & `pyGachi-1.2/pyGachi/prog7.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/prog8.py` & `pyGachi-1.2/pyGachi/prog8.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/siaod1.py` & `pyGachi-1.2/pyGachi/siaod1.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi/siaod2.py` & `pyGachi-1.2/pyGachi/siaod2.py`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/FAQ.docx` & `pyGachi-1.2/pyGachi.egg-info/Files/FAQ.docx`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/PKG-INFO` & `pyGachi-1.2/pyGachi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyGachi
-Version: 1.1
+Version: 1.2
 Summary: Brat ne trogai, eto tibe ne nado
 Home-page: https://github.com/DANILYH/pyGachi
-Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.1.zip
+Download-URL: https://github.com/DANILYH/pyGachi/archive/v1.2.zip
 Author: GachiParty
 Author-email: fetom30268@cutefier.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyGachi-1.1/pyGachi.egg-info/SOURCES.txt` & `pyGachi-1.2/pyGachi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 pyGachi/prog5.py
 pyGachi/prog6.py
 pyGachi/prog7.py
 pyGachi/prog8.py
 pyGachi/prog9.py
 pyGachi/siaod1.py
 pyGachi/siaod2.py
-pyGachi.egg-info/FAQ.docx
 pyGachi.egg-info/PKG-INFO
 pyGachi.egg-info/SOURCES.txt
-pyGachi.egg-info/Z_1.accdb
-pyGachi.egg-info/Z_2.accdb
-pyGachi.egg-info/Z_3.accdb
-pyGachi.egg-info/Z_4.accdb
-pyGachi.egg-info/Z_5.accdb
-pyGachi.egg-info/Z_6.accdb
-pyGachi.egg-info/Z_7.accdb
-pyGachi.egg-info/Z_8.accdb
-pyGachi.egg-info/Z_9.accdb
 pyGachi.egg-info/dependency_links.txt
-pyGachi.egg-info/license.docx
 pyGachi.egg-info/requires.txt
-pyGachi.egg-info/top_level.txt
+pyGachi.egg-info/top_level.txt
+pyGachi.egg-info/Files/FAQ.docx
+pyGachi.egg-info/Files/SoundBox.unitypackage
+pyGachi.egg-info/Files/Z_1.accdb
+pyGachi.egg-info/Files/Z_2.accdb
+pyGachi.egg-info/Files/Z_3.accdb
+pyGachi.egg-info/Files/Z_4.accdb
+pyGachi.egg-info/Files/Z_5.accdb
+pyGachi.egg-info/Files/Z_6.accdb
+pyGachi.egg-info/Files/Z_7.accdb
+pyGachi.egg-info/Files/Z_8.accdb
+pyGachi.egg-info/Files/Z_9.accdb
+pyGachi.egg-info/Files/book1.txt
+pyGachi.egg-info/Files/collisions.unitypackage
+pyGachi.egg-info/Files/grades.txt
+pyGachi.egg-info/Files/license.docx
```

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_1.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_1.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_2.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_2.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_3.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_3.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_4.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_4.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_5.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_5.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_6.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_6.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_7.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_7.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_8.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_8.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/Z_9.accdb` & `pyGachi-1.2/pyGachi.egg-info/Files/Z_9.accdb`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/pyGachi.egg-info/license.docx` & `pyGachi-1.2/pyGachi.egg-info/Files/license.docx`

 * *Files identical despite different names*

### Comparing `pyGachi-1.1/setup.py` & `pyGachi-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup
 
-version = '1.1'
+version = '1.2'
 
 setup(
     name='pyGachi',
     author='GachiParty',
 
     version=version,
     author_email='fetom30268@cutefier.com',
```

