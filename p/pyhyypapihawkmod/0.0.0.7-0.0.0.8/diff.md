# Comparing `tmp/pyhyypapihawkmod-0.0.0.7.tar.gz` & `tmp/pyhyypapihawkmod-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.7.tar", last modified: Thu May 25 18:50:11 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-0.0.0.8.tar", last modified: Fri May 26 15:57:11 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.7.tar` & `pyhyypapihawkmod-0.0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.521609 pyhyypapihawkmod-0.0.0.7/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-05-25 18:50:11.520596 pyhyypapihawkmod-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-05-24 19:47:40.000000 pyhyypapihawkmod-0.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.508441 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     6750 2023-05-25 18:41:13.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    26159 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:50:11.518574 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 18:50:11.000000 pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 18:50:11.521609 pyhyypapihawkmod-0.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-05-25 18:39:15.000000 pyhyypapihawkmod-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.232308 pyhyypapihawkmod-0.0.0.8/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-05-26 15:57:11.231272 pyhyypapihawkmod-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1372 2023-05-26 15:54:57.000000 pyhyypapihawkmod-0.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.221170 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     6753 2023-05-26 15:53:17.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    26159 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-23 06:11:42.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:57:11.229246 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-26 15:57:11.000000 pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:57:11.233319 pyhyypapihawkmod-0.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-05-26 15:55:00.000000 pyhyypapihawkmod-0.0.0.8/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.7/LICENSE.md` & `pyhyypapihawkmod-0.0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/PKG-INFO` & `pyhyypapihawkmod-0.0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.7/README.md` & `pyhyypapihawkmod-0.0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
 
+
+
+0.0.0.8
+
+Minor fix to capture lost notifications
+
+0.0.0.7
+
+Added feature: Binary sensor which shows which zone caused alarm trigger.
+
+
 # pyHyypApi
 API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
 
 How to use:
 
   1. Install:
```

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/alarm_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,19 +59,19 @@
         _current_timestamp = round(datetime.now().timestamp())
             
         for x in _notifications:
             
             _notification_timestamp = round(x['timestamp']/1000)
             if _current_timestamp - _notification_timestamp > 120:
                 continue
-            if _notification_timestamp <= _last_notification_check_timestamp:
+            if _notification_timestamp <= (_last_notification_check_timestamp-30):
                 continue
             _response.append(x)
         
-        _last_notification_check_timestamp = _current_timestamp-1
+        _last_notification_check_timestamp = _current_timestamp
  
         return _response
 
 
     def _triggered_zones(self, site_id: int) -> Any:
            
        #### I still need to limit the zones per site#### <<<>>>><<<>>>< so that multiple sites are possible.
```

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.7/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-0.0.0.8/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.7/setup.py` & `pyhyypapihawkmod-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="0.0.0.7",
+    version="0.0.0.8",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

