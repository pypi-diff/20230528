# Comparing `tmp/tablebase-1.6.1.tar.gz` & `tmp/tablebase-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-hdzlg_x6\tablebase-1.6.1.tar", last modified: Mon Dec 26 01:43:14 2022, max compression
+gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-wl7xyb_b\tablebase-1.6.2.tar", last modified: Sun May 28 00:59:45 2023, max compression
```

## Comparing `tablebase-1.6.1.tar` & `tablebase-1.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-26 01:43:14.136399 tablebase-1.6.1/
--rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.1/LICENSE.txt
--rw-rw-rw-   0        0        0      399 2022-12-26 01:43:14.137400 tablebase-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      721 2022-07-20 22:00:14.000000 tablebase-1.6.1/README.md
--rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      494 2022-12-26 01:43:14.138398 tablebase-1.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-26 01:43:14.122388 tablebase-1.6.1/tablebase/
--rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.1/tablebase/__init__.py
--rw-rw-rw-   0        0        0    10778 2022-12-26 01:34:24.000000 tablebase-1.6.1/tablebase/tablebase.py
-drwxrwxrwx   0        0        0        0 2022-12-26 01:43:14.135398 tablebase-1.6.1/tablebase.egg-info/
--rw-rw-rw-   0        0        0      399 2022-12-26 01:43:14.000000 tablebase-1.6.1/tablebase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2022-12-26 01:43:14.000000 tablebase-1.6.1/tablebase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-26 01:43:14.000000 tablebase-1.6.1/tablebase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-12-26 01:43:14.000000 tablebase-1.6.1/tablebase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.701393 tablebase-1.6.2/
+-rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      399 2023-05-28 00:59:45.701393 tablebase-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2022-07-20 22:00:14.000000 tablebase-1.6.2/README.md
+-rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      494 2023-05-28 00:59:45.704300 tablebase-1.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.654534 tablebase-1.6.2/tablebase/
+-rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.2/tablebase/__init__.py
+-rw-rw-rw-   0        0        0    10790 2023-05-28 00:54:54.000000 tablebase-1.6.2/tablebase/tablebase.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.698375 tablebase-1.6.2/tablebase.egg-info/
+-rw-rw-rw-   0        0        0      399 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/top_level.txt
```

### Comparing `tablebase-1.6.1/LICENSE` & `tablebase-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.1/LICENSE.txt` & `tablebase-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.1/README.md` & `tablebase-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.1/tablebase/tablebase.py` & `tablebase-1.6.2/tablebase/tablebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         """
         Used to save your table for that file.
 
         :param path: Path to that file.
         :param divider: The divider between columns.
         :return:
         """
-        with open(path, 'w') as csv_file:
+        with open(path, 'w', newline="") as csv_file:
             csv_writer = csv.writer(csv_file, delimiter=divider)
             csv_writer.writerows(self.table_content)
 
 
 class CsvTable(Table):
     """
     Used to import a CSV file.
```

