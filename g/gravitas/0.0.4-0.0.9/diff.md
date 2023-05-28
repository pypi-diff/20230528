# Comparing `tmp/gravitas-0.0.4.tar.gz` & `tmp/gravitas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.0.4.tar", max compression
+gzip compressed data, was "gravitas-0.0.9.tar", max compression
```

## Comparing `gravitas-0.0.4.tar` & `gravitas-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0        4 2023-05-27 04:07:39.325347 gravitas-0.0.4/README.md
--rw-r--r--   0        0        0     1396 2023-05-27 04:38:13.803710 gravitas-0.0.4/build.py
--rw-r--r--   0        0        0  5121578 2023-05-27 01:15:07.470942 gravitas-0.0.4/gravitas/EGM96
--rw-r--r--   0        0        0  6559245 2023-05-27 01:18:34.665548 gravitas-0.0.4/gravitas/GRGM360
--rw-r--r--   0        0        0   731918 2023-05-27 03:41:09.634209 gravitas-0.0.4/gravitas/MRO120F
--rw-r--r--   0        0        0      255 2023-05-27 02:23:57.048359 gravitas-0.0.4/gravitas/__init__.py
--rwxr-xr-x   0        0        0    34292 2023-05-27 03:57:02.894875 gravitas-0.0.4/gravitas/grav.so
--rw-r--r--   0        0        0     6152 2023-05-27 03:46:44.136925 gravitas-0.0.4/gravitas/gravlib.c
--rw-r--r--   0        0        0     1288 2023-05-27 03:44:34.140209 gravitas-0.0.4/gravitas/lib.py
--rw-r--r--   0        0        0      603 2023-05-27 04:44:21.672843 gravitas-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 gravitas-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-05-27 04:07:39.325347 gravitas-0.0.9/README.md
+-rw-r--r--   0        0        0     1834 2023-05-27 05:00:41.836776 gravitas-0.0.9/build.py
+-rw-r--r--   0        0        0  5121578 2023-05-27 01:15:07.470942 gravitas-0.0.9/gravitas/EGM96
+-rw-r--r--   0        0        0  6559245 2023-05-27 01:18:34.665548 gravitas-0.0.9/gravitas/GRGM360
+-rw-r--r--   0        0        0   731918 2023-05-27 03:41:09.634209 gravitas-0.0.9/gravitas/MRO120F
+-rw-r--r--   0        0        0      255 2023-05-27 02:23:57.048359 gravitas-0.0.9/gravitas/__init__.py
+-rw-r--r--   0        0        0      838 2023-05-27 02:24:05.204776 gravitas-0.0.9/gravitas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2597 2023-05-27 03:49:02.392833 gravitas-0.0.9/gravitas/__pycache__/lib.cpython-311.pyc
+-rwxr-xr-x   0        0        0    34292 2023-05-27 03:57:02.894875 gravitas-0.0.9/gravitas/grav.so
+-rw-r--r--   0        0        0     6152 2023-05-27 03:46:44.136925 gravitas-0.0.9/gravitas/gravlib.c
+-rw-r--r--   0        0        0     1288 2023-05-27 03:44:34.140209 gravitas-0.0.9/gravitas/lib.py
+-rw-r--r--   0        0        0      680 2023-05-27 05:00:52.809625 gravitas-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 gravitas-0.0.9/setup.py
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 gravitas-0.0.9/PKG-INFO
```

### Comparing `gravitas-0.0.4/build.py` & `gravitas-0.0.9/build.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from distutils.command.build_ext import build_ext
 from distutils.core import Distribution
 from distutils.core import Extension
 from distutils.errors import CCompilerError
 from distutils.errors import DistutilsExecError
 from distutils.errors import DistutilsPlatformError
 
+import os
+import shutil
+
 
 extensions = [
     Extension("grav", ["gravitas/gravlib.c"]),
 ]
 
 
 class ExtBuilder(build_ext):
@@ -37,12 +40,23 @@
     """
     distribution = Distribution({"name": "gravitas", "ext_modules": extensions})
     distribution.package_dir = "gravitas"
 
     cmd = ExtBuilder(distribution)
     cmd.ensure_finalized()
     cmd.run()
+    # Copy built extensions back to the project
+    # for output in cmd.get_outputs():
+        # relative_extension = os.path.relpath(output, cmd.build_lib)
+        # if not os.path.exists(output):
+        #     continue
+
+        # shutil.copyfile(output, relative_extension)
+        # mode = os.stat(relative_extension).st_mode
+        # mode |= (mode & 0o444) >> 2
+        # os.chmod(relative_extension, mode)
+
     return setup_kwargs
 
 
 if __name__ == "__main__":
     build({})
```

### Comparing `gravitas-0.0.4/gravitas/EGM96` & `gravitas-0.0.9/gravitas/EGM96`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/gravitas/GRGM360` & `gravitas-0.0.9/gravitas/GRGM360`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/gravitas/MRO120F` & `gravitas-0.0.9/gravitas/MRO120F`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/gravitas/grav.so` & `gravitas-0.0.9/gravitas/grav.so`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/gravitas/gravlib.c` & `gravitas-0.0.9/gravitas/gravlib.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/gravitas/lib.py` & `gravitas-0.0.9/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.4/PKG-INFO` & `gravitas-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.0.4
+Version: 0.0.9
 Summary: High-fidelity gravity fields for satellite propagation
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
```

