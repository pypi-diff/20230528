# Comparing `tmp/aquatemp-0.0.1.tar.gz` & `tmp/aquatemp-0.0.2.tar.gz`

## Comparing `aquatemp-0.0.1.tar` & `aquatemp-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 aquatemp-0.0.1/build.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aquatemp-0.0.1/src/aquatemp/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 aquatemp-0.0.1/src/aquatemp/aquatemp.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 aquatemp-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aquatemp-0.0.1/LICENSE
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 aquatemp-0.0.1/README.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aquatemp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aquatemp-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 aquatemp-0.0.2/build.sh
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 aquatemp-0.0.2/publish.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aquatemp-0.0.2/aquatemp/__init__.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aquatemp-0.0.2/aquatemp/aquatemp.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 aquatemp-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aquatemp-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aquatemp-0.0.2/README.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aquatemp-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 aquatemp-0.0.2/PKG-INFO
```

### Comparing `aquatemp-0.0.1/src/aquatemp/aquatemp.py` & `aquatemp-0.0.2/aquatemp/aquatemp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from dataclasses import dataclass
 from typing import Optional
 import requests
 import hashlib
 from datetime import datetime, timedelta
 
+def apa():
+    print("apa")
+
 @dataclass
 class AquaTempData:
     powered_on: bool
     inlet_temp: float
     outlet_temp: float
     target_temp: float
     min_target_temp: float
```

### Comparing `aquatemp-0.0.1/.gitignore` & `aquatemp-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aquatemp-0.0.1/LICENSE` & `aquatemp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aquatemp-0.0.1/pyproject.toml` & `aquatemp-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aquatemp"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kristoffer Löfberg", email="kristofer.lofberg@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

