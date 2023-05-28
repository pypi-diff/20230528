# Comparing `tmp/mapna-mind-sdk-0.4.5.tar.gz` & `tmp/mapna-mind-sdk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapna-mind-sdk-0.4.5.tar", last modified: Sat Nov  5 11:49:42 2022, max compression
+gzip compressed data, was "dist/mapna-mind-sdk-0.4.6.tar", last modified: Sun May 28 06:41:43 2023, max compression
```

## Comparing `mapna-mind-sdk-0.4.5.tar` & `mapna-mind-sdk-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-05 11:49:42.853029 mapna-mind-sdk-0.4.5/
--rw-rw-r--   0 root         (0) root         (0)       76 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.5/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-05 11:49:42.837029 mapna-mind-sdk-0.4.5/.idea/
--rw-rw-r--   0 root         (0) root         (0)       41 2020-12-29 06:29:43.000000 mapna-mind-sdk-0.4.5/.idea/.gitignore
--rw-r--r--   0 root         (0) root         (0)      565 2022-11-05 11:49:42.853029 mapna-mind-sdk-0.4.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       55 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-05 11:49:42.837029 mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      565 2022-11-05 11:49:41.000000 mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      655 2022-11-05 11:49:41.000000 mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-11-05 11:49:41.000000 mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2022-11-05 11:49:41.000000 mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-05 11:49:42.849029 mapna-mind-sdk-0.4.5/mapnamindsdk/
--rw-rw-r--   0 root         (0) root         (0)      951 2022-11-01 12:38:34.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Constants.py
--rw-r--r--   0 root         (0) root         (0)     1549 2022-10-24 07:49:05.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Mapper.py
--rw-r--r--   0 root         (0) root         (0)    21561 2022-11-05 11:39:52.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Mind.py
--rw-r--r--   0 root         (0) root         (0)     9652 2022-11-05 11:03:18.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Offline.py
--rw-rw-r--   0 root         (0) root         (0)     1877 2022-04-24 08:41:16.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Online.py
--rw-rw-r--   0 root         (0) root         (0)     2304 2021-02-21 12:09:15.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/Rest.py
--rw-rw-r--   0 root         (0) root         (0)     1070 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/WS.py
--rw-rw-r--   0 root         (0) root         (0)      179 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-05 11:49:42.853029 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/
--rw-rw-r--   0 root         (0) root         (0)      507 2022-04-12 07:23:44.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/Constants.cpython-36.pyc
--rw-rw-r--   0 root         (0) root         (0)     2409 2020-10-12 18:27:46.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/Online.cpython-36.pyc
--rw-rw-r--   0 root         (0) root         (0)     2406 2021-05-17 06:33:06.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/Rest.cpython-36.pyc
--rw-rw-r--   0 root         (0) root         (0)     1451 2020-04-25 08:42:24.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/WS.cpython-36.pyc
--rw-rw-r--   0 root         (0) root         (0)      145 2020-04-25 08:42:14.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 root         (0) root         (0)      845 2021-02-22 09:26:28.000000 mapna-mind-sdk-0.4.5/mapnamindsdk/login_required.py
--rw-rw-r--   0 root         (0) root         (0)       38 2022-11-05 11:49:42.853029 mapna-mind-sdk-0.4.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      751 2022-11-01 12:38:04.000000 mapna-mind-sdk-0.4.5/setup.py
+drwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)        0 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)       76 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.6/.gitignore
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)       38 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/setup.cfg
+drwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)        0 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/
+-rwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)    12442 2021-12-05 09:54:00.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/sdk_test.py
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)       13 2023-05-28 06:41:41.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      691 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)        1 2023-05-28 06:41:41.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      538 2023-05-28 06:41:41.000000 mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      538 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/PKG-INFO
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)       55 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.6/README.md
+drwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)        0 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      179 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__init__.py
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      845 2021-02-22 09:26:28.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/login_required.py
+-rw-r--r--   0 afsaneh   (1000) afsaneh   (1000)     1549 2022-10-24 07:49:05.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Mapper.py
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     1070 2020-04-25 07:27:18.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/WS.py
+-rw-r--r--   0 afsaneh   (1000) afsaneh   (1000)    21682 2023-05-28 06:39:20.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Mind.py
+-rw-r--r--   0 afsaneh   (1000) afsaneh   (1000)     9662 2023-05-28 06:30:45.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Offline.py
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      951 2022-11-01 12:38:34.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Constants.py
+drwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)        0 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     1451 2020-04-25 08:42:24.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/WS.cpython-36.pyc
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      145 2020-04-25 08:42:14.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      490 2023-05-21 06:21:14.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/Constants.cpython-36.pyc
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     2409 2020-10-12 18:27:46.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/Online.cpython-36.pyc
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     2406 2021-05-17 06:33:06.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/Rest.cpython-36.pyc
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     1877 2022-04-24 08:41:16.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Online.py
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)     2304 2021-02-21 12:09:15.000000 mapna-mind-sdk-0.4.6/mapnamindsdk/Rest.py
+drwxrwxr-x   0 afsaneh   (1000) afsaneh   (1000)        0 2023-05-28 06:41:42.000000 mapna-mind-sdk-0.4.6/.idea/
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)       41 2020-12-29 06:29:43.000000 mapna-mind-sdk-0.4.6/.idea/.gitignore
+-rw-rw-r--   0 afsaneh   (1000) afsaneh   (1000)      751 2023-05-28 06:41:35.000000 mapna-mind-sdk-0.4.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mapna-mind-sdk-0.4.5/PKG-INFO` & `mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: mapna-mind-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Mapna MIND Software Development Kit
 Home-page: https://www.mapnaec.com
 Author: Soheil Mehralian, Homa Hasannezhad, Afsaneh Sadeghnezhad
 Author-email: mehralian1@gmail.com
 License: UNKNOWN
-Description: # Mapna MIND SDK
-        
-        Mapna MIND Software Development Kit. 
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# Mapna MIND SDK
+
+Mapna MIND Software Development Kit. 
+
```

### Comparing `mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/PKG-INFO` & `mapna-mind-sdk-0.4.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: mapna-mind-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Mapna MIND Software Development Kit
 Home-page: https://www.mapnaec.com
 Author: Soheil Mehralian, Homa Hasannezhad, Afsaneh Sadeghnezhad
 Author-email: mehralian1@gmail.com
 License: UNKNOWN
-Description: # Mapna MIND SDK
-        
-        Mapna MIND Software Development Kit. 
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# Mapna MIND SDK
+
+Mapna MIND Software Development Kit. 
+
```

### Comparing `mapna-mind-sdk-0.4.5/mapna_mind_sdk.egg-info/SOURCES.txt` & `mapna-mind-sdk-0.4.6/mapna_mind_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 .idea/.gitignore
 mapna_mind_sdk.egg-info/PKG-INFO
 mapna_mind_sdk.egg-info/SOURCES.txt
 mapna_mind_sdk.egg-info/dependency_links.txt
+mapna_mind_sdk.egg-info/sdk_test.py
 mapna_mind_sdk.egg-info/top_level.txt
 mapnamindsdk/Constants.py
 mapnamindsdk/Mapper.py
 mapnamindsdk/Mind.py
 mapnamindsdk/Offline.py
 mapnamindsdk/Online.py
 mapnamindsdk/Rest.py
```

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Constants.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Constants.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Mapper.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Mapper.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Mind.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Mind.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,23 +326,23 @@
         #     # Get signalId for given signalName from the Mapper
         # except KeyError as err:
         #     print("ERROR: Signal Name {} not found!\n".format(err))
 
     @staticmethod
     def _validate(start_date, end_text, myinterval):
         try:
-            interval = {"SECOND": 7, 'MINUTE': 90, 'DAY': 366}
+            interval = {"SECOND": 7, 'MINUTE': 90, 'DAY': 366, "HOUR":366}
             start_date = datetime.datetime.strptime(start_date, '%Y/%m/%d-%H:%M:%S')
             end_text = datetime.datetime.strptime(end_text, '%Y/%m/%d-%H:%M:%S')
             delta = end_text - start_date
             if int(delta.days) > interval[myinterval]:
                 raise Exception("Your timespan is out of range. In the minute interval that is 90 days and "
-                                 "In the second interval that is 7 days")
+                                 "In the second interval that is 7 days and In the hour,day interval that is one year")
         except ValueError:
-            raise ValueError("Incorrect data format, should be YYYY/MM/DD-HH:mm:SS")
+            raise ValueError("Incorrect data format, should be YYYY/MM/DD-HH:mm:SS and interval must be one of these : SECOND, MINUTE, DAY, HOUR ")
 
     @staticmethod
     def _sec_validate(date_text):
         try:
             datetime.datetime.strptime(date_text, '%Y-%m-%d %H:%M:%S')
         except ValueError:
             raise ValueError("Incorrect data format, should be YYYY/MM/DD-HH:mm:SS")
```

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Offline.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Offline.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def getValue(plantName, signalNames, startDate, endDate, aggregation, interval, pageNumber=1,
                  pageSize=100000000):
         jsonResult = None
 
         try:
             Offline._validate_signalName(signalNames)
             Offline._plant_validate(plantName)
-            Offline._validate(startDate, endDate, interval)
+            Offline._validate(startDate, endDate, interval.upper())
             # Offline._validate(endDate)
             signalNames.sort()
             print(len(signalNames))
 
             plant = switch_plant(plantName)
             f = mapper.getInstance(plant)
 
@@ -202,15 +202,15 @@
                 path = 'transient'
             else:
                 print("ERROR: Table Name not found!\n")
                 return None
             post_req = Rest(f'http://{Constants.VIB_SERVICE_IP}:{Constants.VIB_SERVICE_PORT}',
                             path=f'/{path}', params=body)
             jsonResult = post_req.post()
-            print(jsonResult)
+            # print(jsonResult)
         except KeyError as err:
             print("ERROR: Signal Name {} not found!\n".format(err))
         if (isinstance(jsonResult, list) and len(jsonResult)):
             # print(len(jsonResult))
             df_result = Mind._convertJsonVibToDataFrame(jsonResult, tableName)
             # return jsonResult
             if (df_result is not None):
```

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Online.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Online.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/Rest.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/Rest.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/WS.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/WS.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/Online.cpython-36.pyc` & `mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/Online.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/Rest.cpython-36.pyc` & `mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/Rest.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/__pycache__/WS.cpython-36.pyc` & `mapna-mind-sdk-0.4.6/mapnamindsdk/__pycache__/WS.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/mapnamindsdk/login_required.py` & `mapna-mind-sdk-0.4.6/mapnamindsdk/login_required.py`

 * *Files identical despite different names*

### Comparing `mapna-mind-sdk-0.4.5/setup.py` & `mapna-mind-sdk-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
         long_description = fh.read()
         setuptools.setup(
         name="mapna-mind-sdk",
-        version="0.4.5",
+        version="0.4.6",
         author="Soheil Mehralian, Homa Hasannezhad, Afsaneh Sadeghnezhad",
         author_email="mehralian1@gmail.com",
         description="Mapna MIND Software Development Kit",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://www.mapnaec.com",
         packages=setuptools.find_packages(),
```

