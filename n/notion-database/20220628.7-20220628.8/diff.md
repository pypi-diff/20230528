# Comparing `tmp/notion-database-20220628.7.tar.gz` & `tmp/notion-database-20220628.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-database-20220628.7.tar", last modified: Fri Apr 21 14:11:10 2023, max compression
+gzip compressed data, was "notion-database-20220628.8.tar", last modified: Fri Apr 21 14:20:26 2023, max compression
```

## Comparing `notion-database-20220628.7.tar` & `notion-database-20220628.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.011622 notion-database-20220628.7/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    35148 2023-02-10 08:27:15.000000 notion-database-20220628.7/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:11:10.011260 notion-database-20220628.7/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1427 2023-02-10 08:27:15.000000 notion-database-20220628.7/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)       38 2023-04-21 14:11:10.011767 notion-database-20220628.7/setup.cfg
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1038 2023-04-21 13:57:04.000000 notion-database-20220628.7/setup.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:09.997581 notion-database-20220628.7/src/
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.007270 notion-database-20220628.7/src/notion_database/
--rw-r--r--   0 minwook-shin   (501) staff       (20)       30 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11957 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/children.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      497 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/color.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      641 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/cover.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     5340 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/database.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      979 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/icon.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3134 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/page.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     5722 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/properties.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      459 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/query.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1266 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/request.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2816 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/search.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.009696 notion-database-20220628.7/src/notion_database.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      619 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       42 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       22 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/top_level.txt
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.010432 notion-database-20220628.7/src/utils/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/utils/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      469 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/utils/deprecate.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:20:26.966633 notion-database-20220628.8/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    35148 2023-02-10 08:27:15.000000 notion-database-20220628.8/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:20:26.966255 notion-database-20220628.8/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1427 2023-02-10 08:27:15.000000 notion-database-20220628.8/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       38 2023-04-21 14:20:26.966810 notion-database-20220628.8/setup.cfg
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1038 2023-04-21 14:19:48.000000 notion-database-20220628.8/setup.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:20:26.952147 notion-database-20220628.8/src/
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:20:26.962454 notion-database-20220628.8/src/notion_database/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       30 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11957 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/children.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      497 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/color.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      641 2023-04-21 13:57:04.000000 notion-database-20220628.8/src/notion_database/cover.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     5332 2023-04-21 14:19:48.000000 notion-database-20220628.8/src/notion_database/database.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      979 2023-04-21 13:57:04.000000 notion-database-20220628.8/src/notion_database/icon.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3126 2023-04-21 14:19:48.000000 notion-database-20220628.8/src/notion_database/page.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     5722 2023-04-21 13:57:04.000000 notion-database-20220628.8/src/notion_database/properties.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      459 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/query.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1266 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/request.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2816 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/notion_database/search.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:20:26.964800 notion-database-20220628.8/src/notion_database.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:20:26.000000 notion-database-20220628.8/src/notion_database.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      619 2023-04-21 14:20:26.000000 notion-database-20220628.8/src/notion_database.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-04-21 14:20:26.000000 notion-database-20220628.8/src/notion_database.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       42 2023-04-21 14:20:26.000000 notion-database-20220628.8/src/notion_database.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       22 2023-04-21 14:20:26.000000 notion-database-20220628.8/src/notion_database.egg-info/top_level.txt
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:20:26.965522 notion-database-20220628.8/src/utils/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/utils/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      469 2023-02-10 08:27:15.000000 notion-database-20220628.8/src/utils/deprecate.py
```

### Comparing `notion-database-20220628.7/LICENSE` & `notion-database-20220628.8/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/PKG-INFO` & `notion-database-20220628.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-database
-Version: 20220628.7
+Version: 20220628.8
 Summary:  Notion API Database Python Implementation
 Home-page: https://github.com/minwook-shin/notion-database
 Author: minwook-shin
 Author-email: minwook0106@gmail.com
 Project-URL: Bug Tracker, https://github.com/minwook-shin/notion-database/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notion-database-20220628.7/README.md` & `notion-database-20220628.8/README.md`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/setup.py` & `notion-database-20220628.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from src.notion_database import NOTION_VERSION
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="notion-database",
-    version=NOTION_VERSION.replace("-", "") + ".7",
+    version=NOTION_VERSION.replace("-", "") + ".8",
     author="minwook-shin",
     author_email="minwook0106@gmail.com",
     description=" Notion API Database Python Implementation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/minwook-shin/notion-database",
     project_urls={
```

### Comparing `notion-database-20220628.7/src/notion_database/children.py` & `notion-database-20220628.8/src/notion_database/children.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database/cover.py` & `notion-database-20220628.8/src/notion_database/cover.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database/database.py` & `notion-database-20220628.8/src/notion_database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from utils import deprecate
 
 from notion_database.properties import Properties
 from notion_database.request import Request
 
-from src.notion_database.cover import Cover
-from src.notion_database.icon import Icon
+from notion_database.cover import Cover
+from notion_database.icon import Icon
 
 
 class Database:
     def __init__(self, integrations_token):
         """
         init
```

### Comparing `notion-database-20220628.7/src/notion_database/icon.py` & `notion-database-20220628.8/src/notion_database/icon.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database/page.py` & `notion-database-20220628.8/src/notion_database/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from notion_database.children import Children
 from notion_database.properties import Properties
 from notion_database.request import Request
 
-from src.notion_database.cover import Cover
-from src.notion_database.icon import Icon
+from notion_database.cover import Cover
+from notion_database.icon import Icon
 
 LOGGER = logging.getLogger("Notion-Database")
 
 
 class Page:
     def __init__(self, integrations_token):
         """
```

### Comparing `notion-database-20220628.7/src/notion_database/properties.py` & `notion-database-20220628.8/src/notion_database/properties.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database/request.py` & `notion-database-20220628.8/src/notion_database/request.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database/search.py` & `notion-database-20220628.8/src/notion_database/search.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.7/src/notion_database.egg-info/PKG-INFO` & `notion-database-20220628.8/src/notion_database.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-database
-Version: 20220628.7
+Version: 20220628.8
 Summary:  Notion API Database Python Implementation
 Home-page: https://github.com/minwook-shin/notion-database
 Author: minwook-shin
 Author-email: minwook0106@gmail.com
 Project-URL: Bug Tracker, https://github.com/minwook-shin/notion-database/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notion-database-20220628.7/src/notion_database.egg-info/SOURCES.txt` & `notion-database-20220628.8/src/notion_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

