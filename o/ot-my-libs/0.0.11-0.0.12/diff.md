# Comparing `tmp/ot_my_libs-0.0.11.tar.gz` & `tmp/ot_my_libs-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ot_my_libs-0.0.11.tar", last modified: Mon May 22 00:31:49 2023, max compression
+gzip compressed data, was "ot_my_libs-0.0.12.tar", last modified: Sun May 28 20:06:32 2023, max compression
```

## Comparing `ot_my_libs-0.0.11.tar` & `ot_my_libs-0.0.12.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-22 00:31:49.380083 ot_my_libs-0.0.11/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1068 2023-05-12 13:21:05.000000 ot_my_libs-0.0.11/LICENSE.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4358 2023-05-22 00:31:49.380083 ot_my_libs-0.0.11/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3739 2023-05-22 00:31:01.000000 ot_my_libs-0.0.11/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      653 2023-05-22 00:30:45.000000 ot_my_libs-0.0.11/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-05-22 00:31:49.380083 ot_my_libs-0.0.11/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-22 00:31:49.376083 ot_my_libs-0.0.11/src/
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-22 00:31:49.380083 ot_my_libs-0.0.11/src/ot_my_libs/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1369 2023-05-21 11:47:37.000000 ot_my_libs-0.0.11/src/ot_my_libs/ArgsParse.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     8182 2023-05-13 23:15:03.000000 ot_my_libs-0.0.11/src/ot_my_libs/FileActions.py
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3534 2020-12-13 15:12:40.000000 ot_my_libs-0.0.11/src/ot_my_libs/MyCalculate.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2452 2021-11-25 22:30:22.000000 ot_my_libs-0.0.11/src/ot_my_libs/TimeHelper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4222 2021-08-18 16:59:52.000000 ot_my_libs-0.0.11/src/ot_my_libs/XMLHelper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       83 2023-05-20 16:54:46.000000 ot_my_libs-0.0.11/src/ot_my_libs/__init__.py
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4036 2023-05-19 11:11:30.000000 ot_my_libs-0.0.11/src/ot_my_libs/db_helper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1508 2023-05-12 16:10:01.000000 ot_my_libs-0.0.11/src/ot_my_libs/example.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3673 2021-03-23 17:12:02.000000 ot_my_libs-0.0.11/src/ot_my_libs/myFastPlot.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2619 2023-05-21 11:44:07.000000 ot_my_libs-0.0.11/src/ot_my_libs/myLoger.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1710 2023-05-12 15:48:52.000000 ot_my_libs-0.0.11/src/ot_my_libs/myMqttClient.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     9935 2023-05-13 22:54:38.000000 ot_my_libs-0.0.11/src/ot_my_libs/mysql_helper.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-22 00:31:49.380083 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4358 2023-05-22 00:31:49.000000 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      568 2023-05-22 00:31:49.000000 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-05-22 00:31:49.000000 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-05-22 00:31:49.000000 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/requires.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-05-22 00:31:49.000000 ot_my_libs-0.0.11/src/ot_my_libs.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1068 2023-05-12 13:21:05.000000 ot_my_libs-0.0.12/LICENSE.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4320 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3687 2023-05-28 19:58:34.000000 ot_my_libs-0.0.12/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      667 2023-05-28 20:00:47.000000 ot_my_libs-0.0.12/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.928776 ot_my_libs-0.0.12/src/
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.932776 ot_my_libs-0.0.12/src/ot_my_libs/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1369 2023-05-21 11:47:37.000000 ot_my_libs-0.0.12/src/ot_my_libs/ArgsParse.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     8182 2023-05-13 23:15:03.000000 ot_my_libs-0.0.12/src/ot_my_libs/FileActions.py
+-rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3534 2020-12-13 15:12:40.000000 ot_my_libs-0.0.12/src/ot_my_libs/MyCalculate.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     5876 2023-05-28 19:53:25.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:50.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug1_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       91 2023-05-28 16:33:34.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug2_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:38.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug3_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2452 2021-11-25 22:30:22.000000 ot_my_libs-0.0.12/src/ot_my_libs/TimeHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4222 2021-08-18 16:59:52.000000 ot_my_libs-0.0.12/src/ot_my_libs/XMLHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       84 2023-05-28 20:05:46.000000 ot_my_libs-0.0.12/src/ot_my_libs/__init__.py
+-rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4036 2023-05-19 11:11:30.000000 ot_my_libs-0.0.12/src/ot_my_libs/db_helper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1508 2023-05-12 16:10:01.000000 ot_my_libs-0.0.12/src/ot_my_libs/example.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3673 2021-03-23 17:12:02.000000 ot_my_libs-0.0.12/src/ot_my_libs/myFastPlot.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2619 2023-05-21 11:44:07.000000 ot_my_libs-0.0.12/src/ot_my_libs/myLoger.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1710 2023-05-12 15:48:52.000000 ot_my_libs-0.0.12/src/ot_my_libs/myMqttClient.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     9935 2023-05-13 22:54:38.000000 ot_my_libs-0.0.12/src/ot_my_libs/mysql_helper.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4320 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      724 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/requires.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/top_level.txt
```

### Comparing `ot_my_libs-0.0.11/LICENSE.txt` & `ot_my_libs-0.0.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/PKG-INFO` & `ot_my_libs-0.0.12/src/ot_my_libs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,173 @@
 Metadata-Version: 2.1
-Name: ot_my_libs
-Version: 0.0.11
-Summary: oiyshTerminal my basic libs: myLoger | FileActions | MyCalculate | db_helper | mysql_helper | ...
+Name: ot-my-libs
+Version: 0.0.12
+Summary: oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ...
 Author-email: Bartlomiej Ceglik <yoyoek@wp.pl>
 Project-URL: Homepage, https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs
 Project-URL: Bug Tracker, https://github.com/yOyOeK1/oiyshTerminal/labels/ot_my_libs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# oiyshTerminal (pypips) -  ot_my_libs
+# oiyshTerminal (otpips) -  ot_my_libs
 
   Set of function to speed up things like:
 
-  * ArgsParse - to parse argument pass to app returns json
-  * MyCalculate - trigonometry and other maths
-  * db_helper - sqlite3 helper
-  * myFastPlot - fast plot data with kivy
-  * TimeHelper - to do operation on time 
-  * myLoger - logging unifide 
-  * XMLHelper
-  * FileActions - file/dirs/path operations helper
-  * myMqttClient
-  * mysql_helper - mysql helper
-  * example - use case of:
-    * benchmarking - from TimeHelper
-    * sqlite3 - from db_helper
-    
+* ArgsParse - to parse argument pass to app returns json
+
+* MyCalculate - trigonometry and other maths
+
+* db_helper - sqlite3 helper
+
+* myFastPlot - fast plot data with kivy
+
+* TimeHelper - to do operation on time
+
+* myLoger - logging unifide
+
+* XMLHelper
+
+* FileActions - file/dirs/path operations helper
+
+* myMqttClient
+
+* mysql_helper - mysql helper
+
+* PlugsHelper - to help with plugins loading and exploration
+
+* example - use case of:
+
+  * benchmarking - from TimeHelper
+
+  * sqlite3 - from db_helper
+
   **important** - some of subs will want more dependencies then default so look for logs if there is any pip missing ( myFastPlot )
-  
+
+
 ## check example
 
   In directory of library in my case is `/usr/lib/python3.8/site-packages`
-    
-  ```bash
-  python3 ot_my_libs/example.py
-  ```
+
+```bash
+python3 ot_my_libs/example.py
+```
+
   *this will run example use of bencharking uning `ot_my_libs.TimeHelper` and `sqlite3` using `ot_my_libs.db_helper` from the example to get you going :)*
-	
+
   **or**
-	
+
   [xdocs - more in depth](https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs/README_xdoc.md)
 
+### example
 
-### example 
-  
   **TimeHelper** use case as benchmarking tool
 
-  ```python3
-  from ot_my_libs.TimeHelper import TimeHelper as thd
-  import time
-
-  def benchmarkTimer():
-      th = thd()
-      bKey = th.benStart()
-      print("making test run ...")
-      time.sleep(1)
-      th.benDone(
-          bKey,
-          f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]", 
-          printIt=True 
-          )
-  ```
-  
+```python3
+from ot_my_libs.TimeHelper import TimeHelper as thd
+import time
+
+def benchmarkTimer():
+    th = thd()
+    bKey = th.benStart()
+    print("making test run ...")
+    time.sleep(1)
+    th.benDone(
+        bKey,
+        f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]",
+        printIt=True
+        )
+```
+
   **db_helper** use case as fast sqlite3 init_table and CRUDish
-  
-  ```python3
-  from ot_my_libs.db_helper import db_helper as dbh
-  
-  class mdb ( dbh ):
-      ## set your structure of db / table
-      def set_struct(self):
-          self.struct = {
-              'tableA' : { # your table name
-                        'lat':     "float", # field 1 - name: lat type: float
-                        'lon':     "float", # field 2 - name: lat type: float
-                        }
-              }
-              
-    db = mdb('/tmp/mdbTest1.db')
-
-    # yes no initing strate to insert or ...
-    print("inserting ....")
-    insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
-
-    print("select tableA ...")
-    resA = db.select('tableA')
-    print( resA )
-
-    db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
-    print("select id,lat,lon from tableA where id=2 .....")
-    # yes `id` column autoincremental is added automaticly 
-    resB = db.select('tableA','id,lat,lon', 'id=2')
-    print( resB )
-
-    print("delete all ...")
-    db.query('delete from tableA where 1')
-    print("after delete ... select tableA")
-    resC = db.select('tableA')
-    print( resC )
 
-  ```
+```python3
+from ot_my_libs.db_helper import db_helper as dbh
+
+class mdb ( dbh ):
+    ## set your structure of db / table
+    def set_struct(self):
+        self.struct = {
+            'tableA' : { # your table name
+                      'lat':     "float", # field 1 - name: lat type: float
+                      'lon':     "float", # field 2 - name: lat type: float
+                      }
+            }
+
+  db = mdb('/tmp/mdbTest1.db')
+
+  # yes no initing strate to insert or ...
+  print("inserting ....")
+  insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
+
+  print("select tableA ...")
+  resA = db.select('tableA')
+  print( resA )
+
+  db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
+  print("select id,lat,lon from tableA where id=2 .....")
+  # yes `id` column autoincremental is added automaticly
+  resB = db.select('tableA','id,lat,lon', 'id=2')
+  print( resB )
+
+  print("delete all ...")
+  db.query('delete from tableA where 1')
+  print("after delete ... select tableA")
+  resC = db.select('tableA')
+  print( resC )
+```
 
 ## development of package - base line
 
   In directory of project to deploy `tree ot_my_libs`
 
-  ```shell
-  ot_my_libs
-  ├── __init__.py
-  ├── ArgsParse.py
-  ├── example.py
-  ├── db_helper.py
-  ├── FileActions.py
-  ├── MyCalculate.py
-  ├── myFastPlot.py
-  ├── myLoger.py
-  ├── myMqttClient.py
-  ├── mysql_helper.py
-  ├── TimeHelper.py
-  └── XMLHelper.py
-  ```
+```shell
+ot_my_libs
+├── __init__.py
+├── ArgsParse.py
+├── example.py
+├── db_helper.py
+├── FileActions.py
+├── MyCalculate.py
+├── myFastPlot.py
+├── myLoger.py
+├── myMqttClient.py
+├── mysql_helper.py
+├── TimeHelper.py
+├── PlugsHelper.py
+├── PlugsHelperTest_plugXXX_a.py
+└── XMLHelper.py
+```
 
 ### uninstalling it
 
-  ```shell
-  pip3 uninstall ot_my_libs
-  ```
-
-### TODO 
-  
-  - [ ] more examples
-  - [ ] more def xdoc descriptions
+```shell
+pip3 uninstall ot_my_libs
+```
+
+### TODO
+
+- [ ] more examples
+- [ ] more def xdoc descriptions
 
 ### change log
 
- * 0.0.11
-   - fix some README errors parsing and ... 
+* 0.0.12
+
+  - PlugsHelper
+
+* 0.0.11
 
- * 0.0.10
-   - ArgsParse to parse argument comming at start of app
-   - myLoger have more colors to select and new `defColor` argument
-   - add `change log` in README :)
-    
-    
+  - fix some README errors parsing and ...
+
+* 0.0.10
+
+  - ArgsParse to parse argument comming at start of app
+  - myLoger have more colors to select and new `defColor` argument
+  - add `change log` in README :)
 
 ---
 
 If you see that this makes sense [ send me a ☕ ](https://ko-fi.com/B0B0DFYGS) | [Master repository](https://github.com/yOyOeK1/oiyshTerminal) | [About SvOiysh](https://www.youtube.com/@svoiysh)
-
```

### Comparing `ot_my_libs-0.0.11/README.md` & `ot_my_libs-0.0.12/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,159 @@
-# oiyshTerminal (pypips) -  ot_my_libs
+# oiyshTerminal (otpips) -  ot_my_libs
 
   Set of function to speed up things like:
 
-  * ArgsParse - to parse argument pass to app returns json
-  * MyCalculate - trigonometry and other maths
-  * db_helper - sqlite3 helper
-  * myFastPlot - fast plot data with kivy
-  * TimeHelper - to do operation on time 
-  * myLoger - logging unifide 
-  * XMLHelper
-  * FileActions - file/dirs/path operations helper
-  * myMqttClient
-  * mysql_helper - mysql helper
-  * example - use case of:
-    * benchmarking - from TimeHelper
-    * sqlite3 - from db_helper
-    
+* ArgsParse - to parse argument pass to app returns json
+
+* MyCalculate - trigonometry and other maths
+
+* db_helper - sqlite3 helper
+
+* myFastPlot - fast plot data with kivy
+
+* TimeHelper - to do operation on time
+
+* myLoger - logging unifide
+
+* XMLHelper
+
+* FileActions - file/dirs/path operations helper
+
+* myMqttClient
+
+* mysql_helper - mysql helper
+
+* PlugsHelper - to help with plugins loading and exploration
+
+* example - use case of:
+
+  * benchmarking - from TimeHelper
+
+  * sqlite3 - from db_helper
+
   **important** - some of subs will want more dependencies then default so look for logs if there is any pip missing ( myFastPlot )
-  
+
+
 ## check example
 
   In directory of library in my case is `/usr/lib/python3.8/site-packages`
-    
-  ```bash
-  python3 ot_my_libs/example.py
-  ```
+
+```bash
+python3 ot_my_libs/example.py
+```
+
   *this will run example use of bencharking uning `ot_my_libs.TimeHelper` and `sqlite3` using `ot_my_libs.db_helper` from the example to get you going :)*
-	
+
   **or**
-	
+
   [xdocs - more in depth](https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs/README_xdoc.md)
 
+### example
 
-### example 
-  
   **TimeHelper** use case as benchmarking tool
 
-  ```python3
-  from ot_my_libs.TimeHelper import TimeHelper as thd
-  import time
-
-  def benchmarkTimer():
-      th = thd()
-      bKey = th.benStart()
-      print("making test run ...")
-      time.sleep(1)
-      th.benDone(
-          bKey,
-          f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]", 
-          printIt=True 
-          )
-  ```
-  
+```python3
+from ot_my_libs.TimeHelper import TimeHelper as thd
+import time
+
+def benchmarkTimer():
+    th = thd()
+    bKey = th.benStart()
+    print("making test run ...")
+    time.sleep(1)
+    th.benDone(
+        bKey,
+        f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]",
+        printIt=True
+        )
+```
+
   **db_helper** use case as fast sqlite3 init_table and CRUDish
-  
-  ```python3
-  from ot_my_libs.db_helper import db_helper as dbh
-  
-  class mdb ( dbh ):
-      ## set your structure of db / table
-      def set_struct(self):
-          self.struct = {
-              'tableA' : { # your table name
-                        'lat':     "float", # field 1 - name: lat type: float
-                        'lon':     "float", # field 2 - name: lat type: float
-                        }
-              }
-              
-    db = mdb('/tmp/mdbTest1.db')
-
-    # yes no initing strate to insert or ...
-    print("inserting ....")
-    insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
-
-    print("select tableA ...")
-    resA = db.select('tableA')
-    print( resA )
-
-    db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
-    print("select id,lat,lon from tableA where id=2 .....")
-    # yes `id` column autoincremental is added automaticly 
-    resB = db.select('tableA','id,lat,lon', 'id=2')
-    print( resB )
-
-    print("delete all ...")
-    db.query('delete from tableA where 1')
-    print("after delete ... select tableA")
-    resC = db.select('tableA')
-    print( resC )
 
-  ```
+```python3
+from ot_my_libs.db_helper import db_helper as dbh
+
+class mdb ( dbh ):
+    ## set your structure of db / table
+    def set_struct(self):
+        self.struct = {
+            'tableA' : { # your table name
+                      'lat':     "float", # field 1 - name: lat type: float
+                      'lon':     "float", # field 2 - name: lat type: float
+                      }
+            }
+
+  db = mdb('/tmp/mdbTest1.db')
+
+  # yes no initing strate to insert or ...
+  print("inserting ....")
+  insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
+
+  print("select tableA ...")
+  resA = db.select('tableA')
+  print( resA )
+
+  db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
+  print("select id,lat,lon from tableA where id=2 .....")
+  # yes `id` column autoincremental is added automaticly
+  resB = db.select('tableA','id,lat,lon', 'id=2')
+  print( resB )
+
+  print("delete all ...")
+  db.query('delete from tableA where 1')
+  print("after delete ... select tableA")
+  resC = db.select('tableA')
+  print( resC )
+```
 
 ## development of package - base line
 
   In directory of project to deploy `tree ot_my_libs`
 
-  ```shell
-  ot_my_libs
-  ├── __init__.py
-  ├── ArgsParse.py
-  ├── example.py
-  ├── db_helper.py
-  ├── FileActions.py
-  ├── MyCalculate.py
-  ├── myFastPlot.py
-  ├── myLoger.py
-  ├── myMqttClient.py
-  ├── mysql_helper.py
-  ├── TimeHelper.py
-  └── XMLHelper.py
-  ```
+```shell
+ot_my_libs
+├── __init__.py
+├── ArgsParse.py
+├── example.py
+├── db_helper.py
+├── FileActions.py
+├── MyCalculate.py
+├── myFastPlot.py
+├── myLoger.py
+├── myMqttClient.py
+├── mysql_helper.py
+├── TimeHelper.py
+├── PlugsHelper.py
+├── PlugsHelperTest_plugXXX_a.py
+└── XMLHelper.py
+```
 
 ### uninstalling it
 
-  ```shell
-  pip3 uninstall ot_my_libs
-  ```
-
-### TODO 
-  
-  - [ ] more examples
-  - [ ] more def xdoc descriptions
+```shell
+pip3 uninstall ot_my_libs
+```
+
+### TODO
+
+- [ ] more examples
+- [ ] more def xdoc descriptions
 
 ### change log
 
- * 0.0.11
-   - fix some README errors parsing and ... 
+* 0.0.12
+
+  - PlugsHelper
+
+* 0.0.11
 
- * 0.0.10
-   - ArgsParse to parse argument comming at start of app
-   - myLoger have more colors to select and new `defColor` argument
-   - add `change log` in README :)
-    
-    
+  - fix some README errors parsing and ...
+
+* 0.0.10
+
+  - ArgsParse to parse argument comming at start of app
+  - myLoger have more colors to select and new `defColor` argument
+  - add `change log` in README :)
 
 ---
 
 If you see that this makes sense [ send me a ☕ ](https://ko-fi.com/B0B0DFYGS) | [Master repository](https://github.com/yOyOeK1/oiyshTerminal) | [About SvOiysh](https://www.youtube.com/@svoiysh)
-
```

### Comparing `ot_my_libs-0.0.11/pyproject.toml` & `ot_my_libs-0.0.12/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "ot_my_libs"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Bartlomiej Ceglik", email="yoyoek@wp.pl" },
 ]
-description = "oiyshTerminal my basic libs: myLoger | FileActions | MyCalculate | db_helper | mysql_helper | ..."
+description = "oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ..."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'pymysql',
   'paho-mqtt==1.5.0'
 ]
 classifiers = [
```

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/ArgsParse.py` & `ot_my_libs-0.0.12/src/ot_my_libs/ArgsParse.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/FileActions.py` & `ot_my_libs-0.0.12/src/ot_my_libs/FileActions.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/MyCalculate.py` & `ot_my_libs-0.0.12/src/ot_my_libs/MyCalculate.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/TimeHelper.py` & `ot_my_libs-0.0.12/src/ot_my_libs/TimeHelper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/XMLHelper.py` & `ot_my_libs-0.0.12/src/ot_my_libs/XMLHelper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/db_helper.py` & `ot_my_libs-0.0.12/src/ot_my_libs/db_helper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/example.py` & `ot_my_libs-0.0.12/src/ot_my_libs/example.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/myFastPlot.py` & `ot_my_libs-0.0.12/src/ot_my_libs/myFastPlot.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/myLoger.py` & `ot_my_libs-0.0.12/src/ot_my_libs/myLoger.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/myMqttClient.py` & `ot_my_libs-0.0.12/src/ot_my_libs/myMqttClient.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs/mysql_helper.py` & `ot_my_libs-0.0.12/src/ot_my_libs/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.11/src/ot_my_libs.egg-info/PKG-INFO` & `ot_my_libs-0.0.12/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,173 @@
 Metadata-Version: 2.1
-Name: ot-my-libs
-Version: 0.0.11
-Summary: oiyshTerminal my basic libs: myLoger | FileActions | MyCalculate | db_helper | mysql_helper | ...
+Name: ot_my_libs
+Version: 0.0.12
+Summary: oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ...
 Author-email: Bartlomiej Ceglik <yoyoek@wp.pl>
 Project-URL: Homepage, https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs
 Project-URL: Bug Tracker, https://github.com/yOyOeK1/oiyshTerminal/labels/ot_my_libs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# oiyshTerminal (pypips) -  ot_my_libs
+# oiyshTerminal (otpips) -  ot_my_libs
 
   Set of function to speed up things like:
 
-  * ArgsParse - to parse argument pass to app returns json
-  * MyCalculate - trigonometry and other maths
-  * db_helper - sqlite3 helper
-  * myFastPlot - fast plot data with kivy
-  * TimeHelper - to do operation on time 
-  * myLoger - logging unifide 
-  * XMLHelper
-  * FileActions - file/dirs/path operations helper
-  * myMqttClient
-  * mysql_helper - mysql helper
-  * example - use case of:
-    * benchmarking - from TimeHelper
-    * sqlite3 - from db_helper
-    
+* ArgsParse - to parse argument pass to app returns json
+
+* MyCalculate - trigonometry and other maths
+
+* db_helper - sqlite3 helper
+
+* myFastPlot - fast plot data with kivy
+
+* TimeHelper - to do operation on time
+
+* myLoger - logging unifide
+
+* XMLHelper
+
+* FileActions - file/dirs/path operations helper
+
+* myMqttClient
+
+* mysql_helper - mysql helper
+
+* PlugsHelper - to help with plugins loading and exploration
+
+* example - use case of:
+
+  * benchmarking - from TimeHelper
+
+  * sqlite3 - from db_helper
+
   **important** - some of subs will want more dependencies then default so look for logs if there is any pip missing ( myFastPlot )
-  
+
+
 ## check example
 
   In directory of library in my case is `/usr/lib/python3.8/site-packages`
-    
-  ```bash
-  python3 ot_my_libs/example.py
-  ```
+
+```bash
+python3 ot_my_libs/example.py
+```
+
   *this will run example use of bencharking uning `ot_my_libs.TimeHelper` and `sqlite3` using `ot_my_libs.db_helper` from the example to get you going :)*
-	
+
   **or**
-	
+
   [xdocs - more in depth](https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs/README_xdoc.md)
 
+### example
 
-### example 
-  
   **TimeHelper** use case as benchmarking tool
 
-  ```python3
-  from ot_my_libs.TimeHelper import TimeHelper as thd
-  import time
-
-  def benchmarkTimer():
-      th = thd()
-      bKey = th.benStart()
-      print("making test run ...")
-      time.sleep(1)
-      th.benDone(
-          bKey,
-          f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]", 
-          printIt=True 
-          )
-  ```
-  
+```python3
+from ot_my_libs.TimeHelper import TimeHelper as thd
+import time
+
+def benchmarkTimer():
+    th = thd()
+    bKey = th.benStart()
+    print("making test run ...")
+    time.sleep(1)
+    th.benDone(
+        bKey,
+        f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]",
+        printIt=True
+        )
+```
+
   **db_helper** use case as fast sqlite3 init_table and CRUDish
-  
-  ```python3
-  from ot_my_libs.db_helper import db_helper as dbh
-  
-  class mdb ( dbh ):
-      ## set your structure of db / table
-      def set_struct(self):
-          self.struct = {
-              'tableA' : { # your table name
-                        'lat':     "float", # field 1 - name: lat type: float
-                        'lon':     "float", # field 2 - name: lat type: float
-                        }
-              }
-              
-    db = mdb('/tmp/mdbTest1.db')
-
-    # yes no initing strate to insert or ...
-    print("inserting ....")
-    insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
-
-    print("select tableA ...")
-    resA = db.select('tableA')
-    print( resA )
-
-    db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
-    print("select id,lat,lon from tableA where id=2 .....")
-    # yes `id` column autoincremental is added automaticly 
-    resB = db.select('tableA','id,lat,lon', 'id=2')
-    print( resB )
-
-    print("delete all ...")
-    db.query('delete from tableA where 1')
-    print("after delete ... select tableA")
-    resC = db.select('tableA')
-    print( resC )
 
-  ```
+```python3
+from ot_my_libs.db_helper import db_helper as dbh
+
+class mdb ( dbh ):
+    ## set your structure of db / table
+    def set_struct(self):
+        self.struct = {
+            'tableA' : { # your table name
+                      'lat':     "float", # field 1 - name: lat type: float
+                      'lon':     "float", # field 2 - name: lat type: float
+                      }
+            }
+
+  db = mdb('/tmp/mdbTest1.db')
+
+  # yes no initing strate to insert or ...
+  print("inserting ....")
+  insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.11} )
+
+  print("select tableA ...")
+  resA = db.select('tableA')
+  print( resA )
+
+  db.insert( 'tableA', {"lat":2.1,"lon":1.1} )
+  print("select id,lat,lon from tableA where id=2 .....")
+  # yes `id` column autoincremental is added automaticly
+  resB = db.select('tableA','id,lat,lon', 'id=2')
+  print( resB )
+
+  print("delete all ...")
+  db.query('delete from tableA where 1')
+  print("after delete ... select tableA")
+  resC = db.select('tableA')
+  print( resC )
+```
 
 ## development of package - base line
 
   In directory of project to deploy `tree ot_my_libs`
 
-  ```shell
-  ot_my_libs
-  ├── __init__.py
-  ├── ArgsParse.py
-  ├── example.py
-  ├── db_helper.py
-  ├── FileActions.py
-  ├── MyCalculate.py
-  ├── myFastPlot.py
-  ├── myLoger.py
-  ├── myMqttClient.py
-  ├── mysql_helper.py
-  ├── TimeHelper.py
-  └── XMLHelper.py
-  ```
+```shell
+ot_my_libs
+├── __init__.py
+├── ArgsParse.py
+├── example.py
+├── db_helper.py
+├── FileActions.py
+├── MyCalculate.py
+├── myFastPlot.py
+├── myLoger.py
+├── myMqttClient.py
+├── mysql_helper.py
+├── TimeHelper.py
+├── PlugsHelper.py
+├── PlugsHelperTest_plugXXX_a.py
+└── XMLHelper.py
+```
 
 ### uninstalling it
 
-  ```shell
-  pip3 uninstall ot_my_libs
-  ```
-
-### TODO 
-  
-  - [ ] more examples
-  - [ ] more def xdoc descriptions
+```shell
+pip3 uninstall ot_my_libs
+```
+
+### TODO
+
+- [ ] more examples
+- [ ] more def xdoc descriptions
 
 ### change log
 
- * 0.0.11
-   - fix some README errors parsing and ... 
+* 0.0.12
+
+  - PlugsHelper
+
+* 0.0.11
 
- * 0.0.10
-   - ArgsParse to parse argument comming at start of app
-   - myLoger have more colors to select and new `defColor` argument
-   - add `change log` in README :)
-    
-    
+  - fix some README errors parsing and ...
+
+* 0.0.10
+
+  - ArgsParse to parse argument comming at start of app
+  - myLoger have more colors to select and new `defColor` argument
+  - add `change log` in README :)
 
 ---
 
 If you see that this makes sense [ send me a ☕ ](https://ko-fi.com/B0B0DFYGS) | [Master repository](https://github.com/yOyOeK1/oiyshTerminal) | [About SvOiysh](https://www.youtube.com/@svoiysh)
-
```

