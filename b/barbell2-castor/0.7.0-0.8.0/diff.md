# Comparing `tmp/barbell2_castor-0.7.0.tar.gz` & `tmp/barbell2_castor-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbell2_castor-0.7.0.tar", last modified: Mon May 15 09:11:02 2023, max compression
+gzip compressed data, was "dist/barbell2_castor-0.8.0.tar", last modified: Sun May 28 08:45:14 2023, max compression
```

## Comparing `barbell2_castor-0.7.0.tar` & `barbell2_castor-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.199912 barbell2_castor-0.7.0/
--rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:11:02.199652 barbell2_castor-0.7.0/PKG-INFO
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.196915 barbell2_castor-0.7.0/barbell2_castor/
--rw-r--r--   0 Ralph      (501) staff       (20)      264 2023-05-15 09:10:56.000000 barbell2_castor-0.7.0/barbell2_castor/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     9836 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/api.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6634 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/castor2sqlite.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1511 2023-05-15 08:39:48.000000 barbell2_castor-0.7.0/barbell2_castor/query.py
--rw-r--r--   0 Ralph      (501) staff       (20)      628 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/utils.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.199112 barbell2_castor-0.7.0/barbell2_castor.egg-info/
--rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/PKG-INFO
--rw-r--r--   0 Ralph      (501) staff       (20)      416 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/SOURCES.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/dependency_links.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/entry_points.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:09:05.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/not-zip-safe
--rw-r--r--   0 Ralph      (501) staff       (20)       34 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/requires.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       16 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/top_level.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-05-15 09:11:02.200005 barbell2_castor-0.7.0/setup.cfg
--rw-r--r--   0 Ralph      (501) staff       (20)     1372 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-28 08:45:14.575280 barbell2_castor-0.8.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-05-28 08:45:14.574952 barbell2_castor-0.8.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-28 08:45:14.572807 barbell2_castor-0.8.0/barbell2_castor/
+-rw-r--r--   0 ralph      (501) staff       (20)      264 2023-05-28 08:44:59.000000 barbell2_castor-0.8.0/barbell2_castor/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     9836 2023-04-15 21:52:42.000000 barbell2_castor-0.8.0/barbell2_castor/api.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6717 2023-05-28 08:44:12.000000 barbell2_castor-0.8.0/barbell2_castor/castor2sqlite.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1511 2023-05-28 08:18:05.000000 barbell2_castor-0.8.0/barbell2_castor/query.py
+-rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.8.0/barbell2_castor/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-05-28 08:45:14.574516 barbell2_castor-0.8.0/barbell2_castor.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      416 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       34 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       16 2023-05-28 08:45:14.000000 barbell2_castor-0.8.0/barbell2_castor.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-05-28 08:45:14.575376 barbell2_castor-0.8.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.8.0/setup.py
```

### Comparing `barbell2_castor-0.7.0/PKG-INFO` & `barbell2_castor-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: barbell2_castor
-Version: 0.7.0
+Version: 0.8.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
+Description: UNKNOWN
 Keywords: barbell2_castor
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
-
-UNKNOWN
-
```

### Comparing `barbell2_castor-0.7.0/barbell2_castor/api.py` & `barbell2_castor-0.8.0/barbell2_castor/api.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.7.0/barbell2_castor/castor2sqlite.py` & `barbell2_castor-0.8.0/barbell2_castor/castor2sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
+import json
 import logging
-import pandas as pd
 
 # Recompiled version of sqlite3 with larger nr. of supported columns
 from pysqlite3 import dbapi2 as sqlite3
 from datetime import datetime
 from barbell2_castor.api import CastorApiClient
 
 
@@ -167,14 +167,16 @@
         self.output_db_file = output_db_file
         self.add_timestamp = add_timestamp        
         self.log_level = log_level
         logging.root.setLevel(self.log_level)
 
     def execute(self):
         data = self.castor2dict.execute()
+        with open(self.output_db_file + '.json', 'w') as f:
+            json.dump(data, f)
         dict2sqlite = DictToSqlite3(data, self.output_db_file, self.add_timestamp, self.log_level)
         return dict2sqlite.execute()
 
 
 if __name__ == '__main__':
     def main():
         extractor = CastorToSqlite3(
```

### Comparing `barbell2_castor-0.7.0/barbell2_castor/query.py` & `barbell2_castor-0.8.0/barbell2_castor/query.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.7.0/barbell2_castor/utils.py` & `barbell2_castor-0.8.0/barbell2_castor/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.7.0/barbell2_castor.egg-info/PKG-INFO` & `barbell2_castor-0.8.0/barbell2_castor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: barbell2-castor
-Version: 0.7.0
+Version: 0.8.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
+Description: UNKNOWN
 Keywords: barbell2_castor
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
-
-UNKNOWN
-
```

### Comparing `barbell2_castor-0.7.0/setup.py` & `barbell2_castor-0.8.0/setup.py`

 * *Files identical despite different names*

