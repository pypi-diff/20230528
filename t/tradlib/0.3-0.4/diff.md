# Comparing `tmp/tradlib-0.3.tar.gz` & `tmp/tradlib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradlib-0.3.tar", last modified: Tue Feb  8 17:08:55 2022, max compression
+gzip compressed data, was "tradlib-0.4.tar", last modified: Sun May 28 11:47:08 2023, max compression
```

## Comparing `tradlib-0.3.tar` & `tradlib-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-02-08 17:08:55.868110 tradlib-0.3/
--rw-rw-rw-   0        0        0     1150 2022-02-08 16:51:59.000000 tradlib-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5329 2022-02-08 17:08:55.868110 tradlib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4717 2022-02-08 16:51:32.000000 tradlib-0.3/README.md
--rw-rw-rw-   0        0        0      108 2022-01-30 17:43:26.000000 tradlib-0.3/pyproject.toml
--rw-rw-rw-   0        0        0      702 2022-02-08 17:08:55.875363 tradlib-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-02-08 17:08:55.825268 tradlib-0.3/tradlib/
-drwxrwxrwx   0        0        0        0 2022-02-08 17:08:55.847166 tradlib-0.3/tradlib/tradlib/
--rw-rw-rw-   0        0        0      306 2022-02-08 16:52:38.000000 tradlib-0.3/tradlib/tradlib/__init__.py
--rw-rw-rw-   0        0        0     3846 2022-02-08 16:52:58.000000 tradlib-0.3/tradlib/tradlib/tradlib.py
-drwxrwxrwx   0        0        0        0 2022-02-08 17:08:55.867113 tradlib-0.3/tradlib/tradlib.egg-info/
--rw-rw-rw-   0        0        0     5329 2022-02-08 17:08:55.000000 tradlib-0.3/tradlib/tradlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-02-08 17:08:55.000000 tradlib-0.3/tradlib/tradlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-08 17:08:55.000000 tradlib-0.3/tradlib/tradlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-02-08 17:08:55.000000 tradlib-0.3/tradlib/tradlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 11:47:08.239326 tradlib-0.4/
+-rw-rw-rw-   0        0        0     1147 2022-02-09 21:03:22.000000 tradlib-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5290 2023-05-28 11:47:08.239326 tradlib-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4717 2022-02-08 16:51:32.000000 tradlib-0.4/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-30 17:43:26.000000 tradlib-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      702 2023-05-28 11:47:08.242833 tradlib-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 11:47:08.222319 tradlib-0.4/tradlib/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:47:08.226325 tradlib-0.4/tradlib/tradlib/
+-rw-rw-rw-   0        0        0      306 2022-02-08 16:52:38.000000 tradlib-0.4/tradlib/tradlib/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-05-28 11:44:14.000000 tradlib-0.4/tradlib/tradlib/tradlib.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:47:08.238362 tradlib-0.4/tradlib/tradlib.egg-info/
+-rw-rw-rw-   0        0        0     5290 2023-05-28 11:47:08.000000 tradlib-0.4/tradlib/tradlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-28 11:47:08.000000 tradlib-0.4/tradlib/tradlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:47:08.000000 tradlib-0.4/tradlib/tradlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 11:47:08.000000 tradlib-0.4/tradlib/tradlib.egg-info/top_level.txt
```

### Comparing `tradlib-0.3/LICENSE.txt` & `tradlib-0.4/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2022-2022] [Translator] by [Disk_MTH] at [https://github.com/Disk-MTH/Tradlib]
+Copyright (c) [2022-2022] [Tradlib] by [Disk_MTH] at [https://github.com/Disk-MTH/Tradlib]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tradlib-0.3/PKG-INFO` & `tradlib-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tradlib
-Version: 0.3
+Version: 0.4
 Summary: A python library designed to allow an easy translation system for other projects
 Home-page: https://github.com/Disk-MTH/Tradlib
 Author: Disk_MTH
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Disk-MTH/Tradlib/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -124,8 +122,7 @@
 ## License
 
 All the files in this repository are completely free of rights (see the  [license](https://github.com/Disk-MTH/Tradlib/blob/master/diskmth/LICENSE.txt)) so you can grab the code and do whatever you want with them (just respect the  [license](https://github.com/Disk-MTH/Tradlib/blob/master/diskmth/LICENSE.txt)).
 
 Thanks for reading and good development!
 
 Disk_MTH
-
```

### Comparing `tradlib-0.3/README.md` & `tradlib-0.4/README.md`

 * *Files identical despite different names*

### Comparing `tradlib-0.3/setup.cfg` & `tradlib-0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7261 646c 6962 0d0a 7665 7273   = tradlib..vers
-00000020: 696f 6e20 3d20 302e 330d 0a61 7574 686f  ion = 0.3..autho
+00000020: 696f 6e20 3d20 302e 340d 0a61 7574 686f  ion = 0.4..autho
 00000030: 7220 3d20 4469 736b 5f4d 5448 0d0a 6465  r = Disk_MTH..de
 00000040: 7363 7269 7074 696f 6e20 3d20 4120 7079  scription = A py
 00000050: 7468 6f6e 206c 6962 7261 7279 2064 6573  thon library des
 00000060: 6967 6e65 6420 746f 2061 6c6c 6f77 2061  igned to allow a
 00000070: 6e20 6561 7379 2074 7261 6e73 6c61 7469  n easy translati
 00000080: 6f6e 2073 7973 7465 6d20 666f 7220 6f74  on system for ot
 00000090: 6865 7220 7072 6f6a 6563 7473 0d0a 6c6f  her projects..lo
```

### Comparing `tradlib-0.3/tradlib/tradlib/tradlib.py` & `tradlib-0.4/tradlib/tradlib/tradlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     This function loads your translation files. If you don't have executed "set_translations_files_path",
     translations files in the current work directory will be load.
     """
     global translations
 
     for file in os.listdir(translations_path):
         if str(file.lower()).endswith(selected_extension):
-            with open(translations_path + file, "r", encoding="utf-8") as lang:
+            with open(translations_path + "\\" + file, "r", encoding="utf-8") as lang:
                 try:
                     translations.append(json.load(lang))
                 except json.decoder.JSONDecodeError:
                     pass
 
 
 def get_available_languages():
```

### Comparing `tradlib-0.3/tradlib/tradlib.egg-info/PKG-INFO` & `tradlib-0.4/tradlib/tradlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tradlib
-Version: 0.3
+Version: 0.4
 Summary: A python library designed to allow an easy translation system for other projects
 Home-page: https://github.com/Disk-MTH/Tradlib
 Author: Disk_MTH
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Disk-MTH/Tradlib/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -124,8 +122,7 @@
 ## License
 
 All the files in this repository are completely free of rights (see the  [license](https://github.com/Disk-MTH/Tradlib/blob/master/diskmth/LICENSE.txt)) so you can grab the code and do whatever you want with them (just respect the  [license](https://github.com/Disk-MTH/Tradlib/blob/master/diskmth/LICENSE.txt)).
 
 Thanks for reading and good development!
 
 Disk_MTH
-
```

