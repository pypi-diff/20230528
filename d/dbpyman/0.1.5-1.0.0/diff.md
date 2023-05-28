# Comparing `tmp/dbpyman-0.1.5.tar.gz` & `tmp/dbpyman-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.5.tar", last modified: Sat May 27 15:39:46 2023, max compression
+gzip compressed data, was "dbpyman-1.0.0.tar", last modified: Sun May 28 21:29:45 2023, max compression
```

## Comparing `dbpyman-0.1.5.tar` & `dbpyman-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:39:46.673662 dbpyman-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-05-09 18:13:07.000000 dbpyman-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3934 2023-05-27 15:39:46.672665 dbpyman-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3345 2023-05-26 19:49:20.000000 dbpyman-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:39:46.657705 dbpyman-0.1.5/dbpyman.egg-info/
--rw-rw-rw-   0        0        0     3934 2023-05-27 15:39:46.000000 dbpyman-0.1.5/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-27 15:39:46.000000 dbpyman-0.1.5/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:39:46.000000 dbpyman-0.1.5/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 15:39:46.000000 dbpyman-0.1.5/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 15:39:46.660697 dbpyman-0.1.5/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-09 18:05:53.000000 dbpyman-0.1.5/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:39:46.665684 dbpyman-0.1.5/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.5/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1542 2023-05-27 15:38:30.000000 dbpyman-0.1.5/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     3757 2023-05-27 15:38:11.000000 dbpyman-0.1.5/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1462 2023-05-27 15:38:40.000000 dbpyman-0.1.5/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 17:07:59.000000 dbpyman-0.1.5/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:39:46.671667 dbpyman-0.1.5/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.5/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3837 2023-05-27 15:38:20.000000 dbpyman-0.1.5/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     2777 2023-05-27 15:38:49.000000 dbpyman-0.1.5/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-26 19:49:20.000000 dbpyman-0.1.5/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      577 2023-05-27 15:39:26.000000 dbpyman-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:39:46.673662 dbpyman-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:45.916180 dbpyman-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 18:13:07.000000 dbpyman-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3934 2023-05-28 21:29:45.915183 dbpyman-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-26 19:49:20.000000 dbpyman-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:45.897050 dbpyman-1.0.0/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3934 2023-05-28 21:29:45.000000 dbpyman-1.0.0/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-28 21:29:45.000000 dbpyman-1.0.0/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:29:45.000000 dbpyman-1.0.0/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 21:29:45.000000 dbpyman-1.0.0/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:45.901221 dbpyman-1.0.0/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-09 18:05:53.000000 dbpyman-1.0.0/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:45.907205 dbpyman-1.0.0/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-1.0.0/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1542 2023-05-27 15:38:30.000000 dbpyman-1.0.0/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     3757 2023-05-27 15:38:11.000000 dbpyman-1.0.0/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1462 2023-05-27 15:38:40.000000 dbpyman-1.0.0/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 17:07:59.000000 dbpyman-1.0.0/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:45.913189 dbpyman-1.0.0/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-1.0.0/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3837 2023-05-27 15:38:20.000000 dbpyman-1.0.0/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     2777 2023-05-27 15:38:49.000000 dbpyman-1.0.0/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-26 19:49:20.000000 dbpyman-1.0.0/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      577 2023-05-28 21:28:55.000000 dbpyman-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:29:45.916180 dbpyman-1.0.0/setup.cfg
```

### Comparing `dbpyman-0.1.5/LICENSE` & `dbpyman-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/PKG-INFO` & `dbpyman-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.5
+Version: 1.0.0
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.5/README.md` & `dbpyman-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/dbpyman.egg-info/PKG-INFO` & `dbpyman-1.0.0/dbpyman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.5
+Version: 1.0.0
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.5/dbpyman.egg-info/SOURCES.txt` & `dbpyman-1.0.0/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/classes/column.py` & `dbpyman-1.0.0/py_discord_db_management/classes/column.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/classes/database.py` & `dbpyman-1.0.0/py_discord_db_management/classes/database.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/classes/table.py` & `dbpyman-1.0.0/py_discord_db_management/classes/table.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/dbpyman.py` & `dbpyman-1.0.0/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-1.0.0/py_discord_db_management/views/table_add_data_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/views/table_categories_view.py` & `dbpyman-1.0.0/py_discord_db_management/views/table_categories_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/py_discord_db_management/views/table_overview_view.py` & `dbpyman-1.0.0/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.5/pyproject.toml` & `dbpyman-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbpyman"
-version = "0.1.5"
+version = "1.0.0"
 authors = [
   { name="JanikCodes", email="janiksielaff@gmx.de" },
 ]
 description = "A package used to modify & view your MySQL database data dynamically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

