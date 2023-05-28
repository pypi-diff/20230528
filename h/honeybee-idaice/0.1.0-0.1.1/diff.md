# Comparing `tmp/honeybee-idaice-0.1.0.tar.gz` & `tmp/honeybee-idaice-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.1.0.tar", last modified: Sun May 28 18:41:15 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.1.1.tar", last modified: Sun May 28 18:57:15 2023, max compression
```

## Comparing `honeybee-idaice-0.1.0.tar` & `honeybee-idaice-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 18:41:15.000000 honeybee-idaice-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-28 18:39:39.000000 honeybee-idaice-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/setup.py
```

### Comparing `honeybee-idaice-0.1.0/LICENSE` & `honeybee-idaice-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/PKG-INFO` & `honeybee-idaice-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.0
+Version: 0.1.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.0/README.md` & `honeybee-idaice-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/archive.py` & `honeybee-idaice-0.1.1/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.1.1/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.1.1/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.1.1/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/writer.py` & `honeybee-idaice-0.1.1/honeybee_idaice/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.1.1/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.1.1/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.0
+Version: 0.1.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.0/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.1.1/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.0/setup.py` & `honeybee-idaice-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     author_email="info@ladybug.tools",
     description="Honeybee extension for translating HBJSON files to IDA-ICE IDM.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ladybug-tools/honeybee-idaice",
     packages=setuptools.find_packages(exclude=["tests*"]),
     install_requires=requirements,
+    include_package_data=True,
     entry_points={
         "console_scripts": ["honeybee-idaice = honeybee_idaice.cli:ida"]
     },
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: GNU Affero General Public License v3",
```

