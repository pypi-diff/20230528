# Comparing `tmp/terminut-0.0.0.869.tar.gz` & `tmp/terminut-0.0.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.869.tar", last modified: Tue May  9 01:53:25 2023, max compression
+gzip compressed data, was "terminut-0.0.0.901.tar", last modified: Sun May 28 17:03:42 2023, max compression
```

## Comparing `terminut-0.0.0.869.tar` & `terminut-0.0.0.901.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 01:53:25.273802 terminut-0.0.0.869/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.869/LICENSE
--rw-rw-rw-   0        0        0     2628 2023-05-09 01:53:25.273802 terminut-0.0.0.869/PKG-INFO
--rw-rw-rw-   0        0        0     1448 2023-05-09 01:18:24.000000 terminut-0.0.0.869/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.869/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 01:53:25.275311 terminut-0.0.0.869/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-09 01:20:52.000000 terminut-0.0.0.869/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:53:25.261224 terminut-0.0.0.869/terminut/
--rw-rw-rw-   0        0        0      379 2023-05-09 01:49:32.000000 terminut-0.0.0.869/terminut/__init__.py
--rw-rw-rw-   0        0        0     3058 2023-05-09 01:42:41.000000 terminut-0.0.0.869/terminut/console.py
--rw-rw-rw-   0        0        0     6083 2023-05-09 01:44:37.000000 terminut-0.0.0.869/terminut/customs.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:53:25.273802 terminut-0.0.0.869/terminut.egg-info/
--rw-rw-rw-   0        0        0     2628 2023-05-09 01:53:25.000000 terminut-0.0.0.869/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-09 01:53:25.000000 terminut-0.0.0.869/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 01:53:25.000000 terminut-0.0.0.869/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-09 01:53:25.000000 terminut-0.0.0.869/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 01:53:25.000000 terminut-0.0.0.869/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.816017 terminut-0.0.0.901/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.901/LICENSE
+-rw-rw-rw-   0        0        0     2632 2023-05-28 17:03:42.816017 terminut-0.0.0.901/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2023-05-09 02:05:42.000000 terminut-0.0.0.901/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.901/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 17:03:42.816017 terminut-0.0.0.901/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-05-28 16:59:59.000000 terminut-0.0.0.901/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.800706 terminut-0.0.0.901/terminut/
+-rw-rw-rw-   0        0        0      722 2023-05-28 17:03:17.000000 terminut-0.0.0.901/terminut/__init__.py
+-rw-rw-rw-   0        0        0     3058 2023-05-28 17:02:51.000000 terminut-0.0.0.901/terminut/console.py
+-rw-rw-rw-   0        0        0     6083 2023-05-19 01:42:55.000000 terminut-0.0.0.901/terminut/customs.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.815018 terminut-0.0.0.901/terminut.egg-info/
+-rw-rw-rw-   0        0        0     2632 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.869/LICENSE` & `terminut-0.0.0.901/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.869/PKG-INFO` & `terminut-0.0.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.869
+Version: 0.0.0.901
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
@@ -28,16 +28,16 @@
 License-File: LICENSE
 
 # Terminut.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-              > Custom Console Going To Be Used For My Projects
-                  And Available To Anyone Else Who Wants To Use <
+                > Custom Console Going To Be Used For My Projects
+                    And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
 ! package NOT FULLY available for non-personal use !
```

### Comparing `terminut-0.0.0.869/README.md` & `terminut-0.0.0.901/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Terminut.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-              > Custom Console Going To Be Used For My Projects
-                  And Available To Anyone Else Who Wants To Use <
+                > Custom Console Going To Be Used For My Projects
+                    And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
 ! package NOT FULLY available for non-personal use !
```

### Comparing `terminut-0.0.0.869/setup.py` & `terminut-0.0.0.901/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.869"
+vers = "0.0.0.901"
     
 setup(name="terminut",
       version=vers,
       description="Terminut // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `terminut-0.0.0.869/terminut/console.py` & `terminut-0.0.0.901/terminut/console.py`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.869/terminut/customs.py` & `terminut-0.0.0.901/terminut/customs.py`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.869/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.901/terminut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.869
+Version: 0.0.0.901
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
@@ -28,16 +28,16 @@
 License-File: LICENSE
 
 # Terminut.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-              > Custom Console Going To Be Used For My Projects
-                  And Available To Anyone Else Who Wants To Use <
+                > Custom Console Going To Be Used For My Projects
+                    And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
 ! package NOT FULLY available for non-personal use !
```

