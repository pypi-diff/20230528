# Comparing `tmp/superkabuki-0.0.43.tar.gz` & `tmp/superkabuki-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superkabuki-0.0.43.tar", last modified: Sun May 28 05:03:14 2023, max compression
+gzip compressed data, was "superkabuki-0.0.45.tar", last modified: Sun May 28 18:18:03 2023, max compression
```

## Comparing `superkabuki-0.0.43.tar` & `superkabuki-0.0.45.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.248524 superkabuki-0.0.43/
--rw-r--r--   0 a         (1000) a         (1000)     1295 2023-05-28 05:02:44.000000 superkabuki-0.0.43/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)     6641 2023-05-28 05:03:14.244523 superkabuki-0.0.43/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     6030 2023-05-28 05:02:44.000000 superkabuki-0.0.43/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.244523 superkabuki-0.0.43/bin/
--rw-r--r--   0 a         (1000) a         (1000)      127 2023-05-28 05:02:44.000000 superkabuki-0.0.43/bin/superkabuki
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-28 05:03:14.248524 superkabuki-0.0.43/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1003 2023-05-28 05:02:44.000000 superkabuki-0.0.43/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.244523 superkabuki-0.0.43/superkabuki.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     6641 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      231 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       44 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       12 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    12922 2023-05-28 05:02:44.000000 superkabuki-0.0.43/superkabuki.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.897341 superkabuki-0.0.45/
+-rw-r--r--   0 a         (1000) a         (1000)     1295 2023-05-28 05:02:44.000000 superkabuki-0.0.45/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 18:18:03.897341 superkabuki-0.0.45/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     5920 2023-05-28 18:17:59.000000 superkabuki-0.0.45/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.893342 superkabuki-0.0.45/bin/
+-rw-r--r--   0 a         (1000) a         (1000)      127 2023-05-28 05:02:44.000000 superkabuki-0.0.45/bin/superkabuki
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-28 18:18:03.897341 superkabuki-0.0.45/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1003 2023-05-28 05:02:44.000000 superkabuki-0.0.45/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.897341 superkabuki-0.0.45/superkabuki.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      231 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       44 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       12 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    13080 2023-05-28 18:17:22.000000 superkabuki-0.0.45/superkabuki.py
```

### Comparing `superkabuki-0.0.43/LICENSE` & `superkabuki-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.43/PKG-INFO` & `superkabuki-0.0.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.43
+Version: 0.0.45
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,16 +13,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.41 is now Released.
-![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
+# SuperKabuki v.0.0.45 is now Released.
+
+
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.43/README.md` & `superkabuki-0.0.45/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.41 is now Released.
-![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
+# SuperKabuki v.0.0.45 is now Released.
+
+
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.43/setup.py` & `superkabuki-0.0.45/setup.py`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.43/superkabuki.egg-info/PKG-INFO` & `superkabuki-0.0.45/superkabuki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.43
+Version: 0.0.45
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,16 +13,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.41 is now Released.
-![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
+# SuperKabuki v.0.0.45 is now Released.
+
+
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.43/superkabuki.py` & `superkabuki-0.0.45/superkabuki.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from threefive.crc import crc32
 from threefive.bitn import NBin
 from new_reader import reader
 from iframes import IFramer
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "43"
+MAINTAINENCE = "45"
 
 
 def version():
     """
     version prints version as a string
 
     Odd number versions are releases.
@@ -120,22 +120,29 @@
             help="Show version",
         )
 
         args = parser.parse_args()
         self._apply_args(args)
 
     def _apply_args(self, args):
+        self._args_version(args)
         if args.scte35_pid and args.input:
             self.outfile = args.output
             self.infile = args.input
             self.sidecar_file = args.sidecar
             self._tsdata = reader(args.input)
             self.pid2int(args.scte35_pid)
             self.time_signals = args.time_signals
 
+    @staticmethod
+    def _args_version(args):
+        if args.version:
+            print(version())
+            sys.exit()
+
     def pid2int(self, pid):
         try:
             self.scte35_pid = int(args.scte35_pid)
         except:
             try:
                 self.scte35_pid = int(args.scte35_pid, 16)
             except:
```

