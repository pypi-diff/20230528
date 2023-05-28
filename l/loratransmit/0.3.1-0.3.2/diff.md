# Comparing `tmp/loratransmit-0.3.1.tar.gz` & `tmp/loratransmit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loratransmit-0.3.1.tar", last modified: Sun May 28 18:58:38 2023, max compression
+gzip compressed data, was "loratransmit-0.3.2.tar", last modified: Sun May 28 19:01:41 2023, max compression
```

## Comparing `loratransmit-0.3.1.tar` & `loratransmit-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 18:58:38.117458 loratransmit-0.3.1/
--rw-rw-r--   0 flux      (1000) flux      (1000)     1066 2023-05-11 17:54:13.000000 loratransmit-0.3.1/LICENSE
--rw-rw-r--   0 flux      (1000) flux      (1000)     1789 2023-05-28 18:58:38.117458 loratransmit-0.3.1/PKG-INFO
--rw-rw-r--   0 flux      (1000) flux      (1000)     1342 2023-05-28 18:58:08.000000 loratransmit-0.3.1/README.md
-drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 18:58:38.113458 loratransmit-0.3.1/loratransmit/
--rw-rw-r--   0 flux      (1000) flux      (1000)    22951 2023-05-11 17:58:05.000000 loratransmit-0.3.1/loratransmit/RNode.py
--rw-rw-r--   0 flux      (1000) flux      (1000)      228 2023-05-28 18:46:23.000000 loratransmit-0.3.1/loratransmit/__init__.py
--rw-rw-r--   0 flux      (1000) flux      (1000)     2078 2023-05-28 18:47:37.000000 loratransmit-0.3.1/loratransmit/loratransmit.py
-drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 18:58:38.117458 loratransmit-0.3.1/loratransmit.egg-info/
--rw-rw-r--   0 flux      (1000) flux      (1000)     1789 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/PKG-INFO
--rw-rw-r--   0 flux      (1000) flux      (1000)      320 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/SOURCES.txt
--rw-rw-r--   0 flux      (1000) flux      (1000)        1 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/dependency_links.txt
--rw-rw-r--   0 flux      (1000) flux      (1000)       51 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/entry_points.txt
--rw-rw-r--   0 flux      (1000) flux      (1000)        9 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/requires.txt
--rw-rw-r--   0 flux      (1000) flux      (1000)       13 2023-05-28 18:58:38.000000 loratransmit-0.3.1/loratransmit.egg-info/top_level.txt
--rw-rw-r--   0 flux      (1000) flux      (1000)       38 2023-05-28 18:58:38.117458 loratransmit-0.3.1/setup.cfg
--rw-rw-r--   0 flux      (1000) flux      (1000)      785 2023-05-28 18:48:15.000000 loratransmit-0.3.1/setup.py
+drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 19:01:41.069218 loratransmit-0.3.2/
+-rw-rw-r--   0 flux      (1000) flux      (1000)     1066 2023-05-11 17:54:13.000000 loratransmit-0.3.2/LICENSE
+-rw-rw-r--   0 flux      (1000) flux      (1000)     1757 2023-05-28 19:01:41.069218 loratransmit-0.3.2/PKG-INFO
+-rw-rw-r--   0 flux      (1000) flux      (1000)     1310 2023-05-28 19:00:54.000000 loratransmit-0.3.2/README.md
+drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 19:01:41.065218 loratransmit-0.3.2/loratransmit/
+-rw-rw-r--   0 flux      (1000) flux      (1000)    22951 2023-05-11 17:58:05.000000 loratransmit-0.3.2/loratransmit/RNode.py
+-rw-rw-r--   0 flux      (1000) flux      (1000)      228 2023-05-28 18:46:23.000000 loratransmit-0.3.2/loratransmit/__init__.py
+-rw-rw-r--   0 flux      (1000) flux      (1000)     2078 2023-05-28 18:47:37.000000 loratransmit-0.3.2/loratransmit/loratransmit.py
+drwxrwxr-x   0 flux      (1000) flux      (1000)        0 2023-05-28 19:01:41.069218 loratransmit-0.3.2/loratransmit.egg-info/
+-rw-rw-r--   0 flux      (1000) flux      (1000)     1757 2023-05-28 19:01:40.000000 loratransmit-0.3.2/loratransmit.egg-info/PKG-INFO
+-rw-rw-r--   0 flux      (1000) flux      (1000)      320 2023-05-28 19:01:41.000000 loratransmit-0.3.2/loratransmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 flux      (1000) flux      (1000)        1 2023-05-28 19:01:40.000000 loratransmit-0.3.2/loratransmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 flux      (1000) flux      (1000)       51 2023-05-28 19:01:40.000000 loratransmit-0.3.2/loratransmit.egg-info/entry_points.txt
+-rw-rw-r--   0 flux      (1000) flux      (1000)        9 2023-05-28 19:01:40.000000 loratransmit-0.3.2/loratransmit.egg-info/requires.txt
+-rw-rw-r--   0 flux      (1000) flux      (1000)       13 2023-05-28 19:01:40.000000 loratransmit-0.3.2/loratransmit.egg-info/top_level.txt
+-rw-rw-r--   0 flux      (1000) flux      (1000)       38 2023-05-28 19:01:41.069218 loratransmit-0.3.2/setup.cfg
+-rw-rw-r--   0 flux      (1000) flux      (1000)      785 2023-05-28 19:01:36.000000 loratransmit-0.3.2/setup.py
```

### Comparing `loratransmit-0.3.1/LICENSE` & `loratransmit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loratransmit-0.3.1/PKG-INFO` & `loratransmit-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loratransmit
-Version: 0.3.1
+Version: 0.3.2
 Summary: LoRa packet transmitter for RNode hardware
 Home-page: https://github.com/randogoth/loratransmit
 Author: randogoth
 Author-email: randogoth@posteo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 ```
 
 ## Example
 
 Payload passed as argument
 
 ```
-$ /bin/python3 loratransmit.py --freq 917500000 /dev/ttyACM0 "Hello World"
+$ loratransmit --freq 917500000 /dev/ttyACM0 "Hello World"
 ```
 
 Payload passed through pipe
 
 ```
-$ echo "Hello World" | /bin/python3 loratransmit.py --freq 917500000 /dev/ttyACM0
+$ echo "Hello World" | loratransmit --freq 917500000 /dev/ttyACM0
 ```
```

### Comparing `loratransmit-0.3.1/README.md` & `loratransmit-0.3.2/loratransmit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: loratransmit
+Version: 0.3.2
+Summary: LoRa packet transmitter for RNode hardware
+Home-page: https://github.com/randogoth/loratransmit
+Author: randogoth
+Author-email: randogoth@posteo.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LoRaTransmit
 
 Simple commandline raw LoRa packet transmitter for [RNode](https://unsigned.io/articles/2023_01_16_The_New_RNode_Ecosystem_Is_Here.html) hardware.
 
 It's meant to be complementary to the packet sniffer [LoRaMon](https://github.com/markqvist/LoRaMon) and uses the latest [Python Module](https://github.com/markqvist/RNode_Firmware/tree/master/Python%20Module) that comes with the [RNode Firmware](https://github.com/markqvist/RNode_Firmware).
 
 ## Install
@@ -35,15 +49,15 @@
 ```
 
 ## Example
 
 Payload passed as argument
 
 ```
-$ /bin/python3 loratransmit.py --freq 917500000 /dev/ttyACM0 "Hello World"
+$ loratransmit --freq 917500000 /dev/ttyACM0 "Hello World"
 ```
 
 Payload passed through pipe
 
 ```
-$ echo "Hello World" | /bin/python3 loratransmit.py --freq 917500000 /dev/ttyACM0
-```
+$ echo "Hello World" | loratransmit --freq 917500000 /dev/ttyACM0
+```
```

### Comparing `loratransmit-0.3.1/loratransmit/RNode.py` & `loratransmit-0.3.2/loratransmit/RNode.py`

 * *Files identical despite different names*

### Comparing `loratransmit-0.3.1/loratransmit/loratransmit.py` & `loratransmit-0.3.2/loratransmit/loratransmit.py`

 * *Files identical despite different names*

### Comparing `loratransmit-0.3.1/setup.py` & `loratransmit-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="loratransmit",
-    version="0.3.1",
+    version="0.3.2",
     author="randogoth",
     author_email="randogoth@posteo.org",
     description="LoRa packet transmitter for RNode hardware",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/randogoth/loratransmit",
     packages=setuptools.find_packages(),
```

