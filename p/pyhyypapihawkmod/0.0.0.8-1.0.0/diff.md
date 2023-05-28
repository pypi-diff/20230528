# Comparing `tmp/pyhyypapihawkmod-0.0.0.8.tar.gz` & `tmp/pyhyypapihawkmod-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.8.tar", last modified: Fri May 26 15:57:11 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.0.0.tar", last modified: Sun May 28 15:24:31 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.8.tar` & `pyhyypapihawkmod-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.232308 pyhyypapihawkmod-0.0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-05-26 15:57:11.231272 pyhyypapihawkmod-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1372 2023-05-26 15:54:57.000000 pyhyypapihawkmod-0.0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.221170 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     6753 2023-05-26 15:53:17.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    26159 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.229246 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:57:11.233319 pyhyypapihawkmod-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-05-26 15:55:00.000000 pyhyypapihawkmod-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:24:31.417829 pyhyypapihawkmod-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-05-28 15:24:31.417829 pyhyypapihawkmod-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1277 2023-05-28 15:17:42.000000 pyhyypapihawkmod-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:24:31.406678 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     4808 2023-05-28 15:16:28.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    26159 2023-05-28 13:40:27.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:24:31.415809 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-28 15:24:31.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-28 15:24:31.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 15:24:31.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-28 15:24:31.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 15:24:31.000000 pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 15:24:31.417829 pyhyypapihawkmod-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-05-28 15:17:45.000000 pyhyypapihawkmod-1.0.0/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.8/LICENSE.md` & `pyhyypapihawkmod-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/PKG-INFO` & `pyhyypapihawkmod-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.8
+Version: 1.0.0
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.8/README.md` & `pyhyypapihawkmod-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
 
-
-
-0.0.0.8
-
-Minor fix to capture lost notifications
-
-0.0.0.7
-
-Added feature: Binary sensor which shows which zone caused alarm trigger.
-
-
 # pyHyypApi
 API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
 
+
 How to use:
 
   1. Install:
 
 ```pip install pyhyypapihawkmod```
 
   2.1. Login (ADT Secure Home):
 
 
 ```
 import pyhyypapihawkmod
 import json
-client = pyhyypapihawkmod.HyypClient(email="",password="")
+client = pyhyypapihawkmod.hyypclient(email="",password="")
 client.login()
 ```
 
 **OR**
 
   2.2. Login (IDT Hyyp):
 
 ```
 import pyhyypapihawkmod
 import json
-client = pyhyypapihawkmod.HyypClient(email="",password="",pkg=pyhyypapihawkmod.HyypPkg.IDS_HYYP_GENERIC.value)
+client = pyhyypapihawkmod.hyypclient(email="",password="",pkg=pyhyypapihawkmod.HyypPkg.IDS_HYYP_GENERIC.value)
 client.login()
 
 ```
 
 
 3. Get site/partition/user/zone info:
 
@@ -51,7 +41,12 @@
 ```
 
 TO Do:
 
 - CLI usage. (GCF client is there, just needs some more automation.)
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
+
+
+Changelog 1.0.0
+
+Bumped main release to 1.0.0
```

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.8
+Version: 1.0.0
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.0.0/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.8/setup.py` & `pyhyypapihawkmod-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="0.0.0.8",
+    version="1.0.0",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

