# Comparing `tmp/YetAnotherModule-0.0.2.tar.gz` & `tmp/YetAnotherModule-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YetAnotherModule-0.0.2.tar", last modified: Wed May 24 23:33:37 2023, max compression
+gzip compressed data, was "YetAnotherModule-0.0.2.1.tar", last modified: Sun May 28 18:34:32 2023, max compression
```

## Comparing `YetAnotherModule-0.0.2.tar` & `YetAnotherModule-0.0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/YAPM/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/Matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:34:32.453564 YetAnotherModule-0.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-28 18:34:32.453564 YetAnotherModule-0.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:34:32.453564 YetAnotherModule-0.0.2.1/YAPM/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/YAPM/Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/YAPM/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/YAPM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:34:32.453564 YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-28 18:34:32.000000 YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-28 18:34:32.000000 YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:34:32.000000 YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 18:34:32.000000 YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:34:32.453564 YetAnotherModule-0.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-28 18:34:20.000000 YetAnotherModule-0.0.2.1/setup.py
```

### Comparing `YetAnotherModule-0.0.2/LICENSE` & `YetAnotherModule-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.2/PKG-INFO` & `YetAnotherModule-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `YetAnotherModule-0.0.2/README.md` & `YetAnotherModule-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.2/YAPM/Matrix.py` & `YetAnotherModule-0.0.2.1/YAPM/Matrix.py`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.2/YAPM/Other.py` & `YetAnotherModule-0.0.2.1/YAPM/Other.py`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.2/YetAnotherModule.egg-info/PKG-INFO` & `YetAnotherModule-0.0.2.1/YetAnotherModule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `YetAnotherModule-0.0.2/setup.py` & `YetAnotherModule-0.0.2.1/setup.py`

 * *Files identical despite different names*

