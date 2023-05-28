# Comparing `tmp/animedata-0.3.5.tar.gz` & `tmp/animedata-0.3.6.tar.gz`

## Comparing `animedata-0.3.5.tar` & `animedata-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3.5/ad_test.py
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 animedata-0.3.5/animedata.py
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3.5/animedata_source.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.5/LICENSE
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.5/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 animedata-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 animedata-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3.6/ad_test.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 animedata-0.3.6/animedata.py
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3.6/animedata_source.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.6/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 animedata-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 animedata-0.3.6/PKG-INFO
```

### Comparing `animedata-0.3.5/ad_test.py` & `animedata-0.3.6/ad_test.py`

 * *Files identical despite different names*

### Comparing `animedata-0.3.5/animedata.py` & `animedata-0.3.6/animedata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 """Module to manage AnimeData library."""
 
 import json
 import urllib.request
 import urllib.error
-import tomllib
 import warnings
+import importlib.metadata
 import os.path
 from copy import deepcopy
 
+ad_version = importlib.metadata.version("animedata")
 dir_path = os.path.dirname(__file__)
 ad_table = {
     "repository_url":
     "https://raw.githubusercontent.com/swarthur/animedata/",
     "source_file_name": "./animedata_source.json",
     "local_file_name": "./animedata_local.json",
     "anime_name": "anime_name",
     "seasons": "seasons",
     "episode_duration": "episode_duration",
     "episode_release_date": "episode_release_date",
     "episode_name": "episode_name"}
 
-"""with open(os.path.join(dir_path, ".\\pyproject.toml"), mode="rb") as pypr:
-    ad_version = tomllib.load(pypr)["project"]["version"]
-print("AnimeData script version : ", ad_version)"""
-
-def print_path():
-    file_path = os.path.dirname(__file__)
-    for element in os.walk(file_path):
-        print(element)
-    print(os.path.join(file_path,".\\pyproject.toml"))
-    with open(os.path.join(file_path,".\\pyproject.toml"),"rb") as toml_file:
-        version = tomllib.load(toml_file)["project"]["version"]
-        print(version)
-
 
 def get_ad_lib(branch: str = "main"):
     """Download and replace local AnimeData library from Github.
 
     Args:
         branch (str, optional): select the target branch.
             Defaults to "main".
```

### Comparing `animedata-0.3.5/animedata_source.json` & `animedata-0.3.6/animedata_source.json`

 * *Files identical despite different names*

### Comparing `animedata-0.3.5/LICENSE` & `animedata-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `animedata-0.3.5/README.md` & `animedata-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `animedata-0.3.5/pyproject.toml` & `animedata-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
 00000060: 5d0d 0a65 7863 6c75 6465 203d 205b 0d0a  ]..exclude = [..
 00000070: 2020 222f 6469 7374 222c 0d0a 2020 222f    "/dist",..  "/
 00000080: 2e67 6974 222c 0d0a 2020 222e 6769 7469  .git",..  ".giti
 00000090: 676e 6f72 6522 0d0a 2020 5d0d 0a0d 0a5b  gnore"..  ]....[
 000000a0: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 000000b0: 2022 616e 696d 6564 6174 6122 0d0a 7665   "animedata"..ve
-000000c0: 7273 696f 6e20 3d20 2230 2e33 2e35 220d  rsion = "0.3.5".
+000000c0: 7273 696f 6e20 3d20 2230 2e33 2e36 220d  rsion = "0.3.6".
 000000d0: 0a61 7574 686f 7273 203d 205b 0d0a 207b  .authors = [.. {
 000000e0: 6e61 6d65 3d22 7377 6172 7468 7572 227d  name="swarthur"}
 000000f0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 00000100: 203d 2022 4f70 656e 2d73 6f75 7263 6520   = "Open-source 
 00000110: 6c69 6272 6172 7920 636f 6e74 6169 6e69  library containi
 00000120: 6e67 2064 6174 6162 6173 6520 6162 6f75  ng database abou
 00000130: 7420 616e 696d 6573 2f73 6572 6965 7320  t animes/series
```

### Comparing `animedata-0.3.5/PKG-INFO` & `animedata-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animedata
-Version: 0.3.5
+Version: 0.3.6
 Summary: Open-source library containing database about animes/series and including a built-in utility.
 Project-URL: Github, https://github.com/swarthur/animedata
 Project-URL: Bug, https://github.com/swarthur/animedata/issues
 Author: swarthur
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

