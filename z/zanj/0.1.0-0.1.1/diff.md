# Comparing `tmp/zanj-0.1.0.tar.gz` & `tmp/zanj-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanj-0.1.0.tar", max compression
+gzip compressed data, was "zanj-0.1.1.tar", max compression
```

## Comparing `zanj-0.1.0.tar` & `zanj-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.0/LICENSE
--rw-r--r--   0        0        0      937 2023-05-28 06:42:14.371167 zanj-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4213 2023-05-28 05:11:39.608638 zanj-0.1.0/README.md
--rw-r--r--   0        0        0      146 2023-05-28 05:56:06.808527 zanj-0.1.0/zanj/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.0/zanj/externals.py
--rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.0/zanj/loading.py
--rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.0/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.0/zanj/serializing.py
--rw-r--r--   0        0        0     9696 2023-05-28 05:22:18.549492 zanj-0.1.0/zanj/torchutil.py
--rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.0/zanj/zanj.py
--rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 zanj-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.1/LICENSE
+-rw-r--r--   0        0        0      937 2023-05-28 07:22:02.319290 zanj-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4213 2023-05-28 05:11:39.608638 zanj-0.1.1/README.md
+-rw-r--r--   0        0        0      146 2023-05-28 07:19:30.975404 zanj-0.1.1/zanj/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.1/zanj/externals.py
+-rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.1/zanj/loading.py
+-rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.1/zanj/readme.md
+-rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.1/zanj/serializing.py
+-rw-r--r--   0        0        0     9696 2023-05-28 05:22:18.549492 zanj-0.1.1/zanj/torchutil.py
+-rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.1/zanj/zanj.py
+-rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 zanj-0.1.1/PKG-INFO
```

### Comparing `zanj-0.1.0/LICENSE` & `zanj-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/pyproject.toml` & `zanj-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "zanj"
-version = "0.1.0"
+version = "0.1.1"
 description = "save and load complex objects to disk without pickling"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 repository = "https://github.com/mivanit/ZANJ"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-muutils = "^0.4.0"
-torch = "^1.12.1"
+muutils = "^0.4.1"
+torch = "^1.13.1"
 numpy = "^1.22.4"
 jaxtyping = "^0.2.12"
 pandas = "^1.5.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `zanj-0.1.0/README.md` & `zanj-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/externals.py` & `zanj-0.1.1/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/loading.py` & `zanj-0.1.1/zanj/loading.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/readme.md` & `zanj-0.1.1/zanj/readme.md`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/serializing.py` & `zanj-0.1.1/zanj/serializing.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/torchutil.py` & `zanj-0.1.1/zanj/torchutil.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/zanj/zanj.py` & `zanj-0.1.1/zanj/zanj.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.0/PKG-INFO` & `zanj-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: zanj
-Version: 0.1.0
+Version: 0.1.1
 Summary: save and load complex objects to disk without pickling
 Home-page: https://github.com/mivanit/ZANJ
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jaxtyping (>=0.2.12,<0.3.0)
-Requires-Dist: muutils (>=0.4.0,<0.5.0)
+Requires-Dist: muutils (>=0.4.1,<0.5.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: torch (>=1.12.1,<2.0.0)
+Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/ZANJ
 Description-Content-Type: text/markdown
 
 # ZANJ
 
 
 # Overview
```

