# Comparing `tmp/animedata-0.3.3.tar.gz` & `tmp/animedata-0.3.4.tar.gz`

## Comparing `animedata-0.3.3.tar` & `animedata-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.3/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3.3/ad_test.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 animedata-0.3.3/animedata.py
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3.3/animedata_source.json
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 animedata-0.3.3/path.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.3/LICENSE
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.3/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 animedata-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 animedata-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3.4/ad_test.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 animedata-0.3.4/animedata.py
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3.4/animedata_source.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.4/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 animedata-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 animedata-0.3.4/PKG-INFO
```

### Comparing `animedata-0.3.3/ad_test.py` & `animedata-0.3.4/ad_test.py`

 * *Files identical despite different names*

### Comparing `animedata-0.3.3/animedata.py` & `animedata-0.3.4/animedata.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,21 @@
     "episode_release_date": "episode_release_date",
     "episode_name": "episode_name"}
 
 """with open(os.path.join(dir_path, ".\\pyproject.toml"), mode="rb") as pypr:
     ad_version = tomllib.load(pypr)["project"]["version"]
 print("AnimeData script version : ", ad_version)"""
 
+def print_path():
+    file_path = os.path.dirname(__file__)
+    print(os.path.join(file_path,".\\pyproject.toml"))
+    with open(os.path.join(file_path,".\\pyproject.toml"),"rb") as toml_file:
+        version = tomllib.load(toml_file)["project"]["version"]
+        print(version)
+
 
 def get_ad_lib(branch: str = "main"):
     """Download and replace local AnimeData library from Github.
 
     Args:
         branch (str, optional): select the target branch.
             Defaults to "main".
```

### Comparing `animedata-0.3.3/animedata_source.json` & `animedata-0.3.4/animedata_source.json`

 * *Files identical despite different names*

### Comparing `animedata-0.3.3/LICENSE` & `animedata-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `animedata-0.3.3/README.md` & `animedata-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `animedata-0.3.3/pyproject.toml` & `animedata-0.3.4/pyproject.toml`

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
-000000c0: 7273 696f 6e20 3d20 2230 2e33 2e33 220d  rsion = "0.3.3".
+000000c0: 7273 696f 6e20 3d20 2230 2e33 2e34 220d  rsion = "0.3.4".
 000000d0: 0a61 7574 686f 7273 203d 205b 0d0a 207b  .authors = [.. {
 000000e0: 6e61 6d65 3d22 7377 6172 7468 7572 227d  name="swarthur"}
 000000f0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 00000100: 203d 2022 4f70 656e 2d73 6f75 7263 6520   = "Open-source 
 00000110: 6c69 6272 6172 7920 636f 6e74 6169 6e69  library containi
 00000120: 6e67 2064 6174 6162 6173 6520 6162 6f75  ng database abou
 00000130: 7420 616e 696d 6573 2f73 6572 6965 7320  t animes/series
```

### Comparing `animedata-0.3.3/PKG-INFO` & `animedata-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animedata
-Version: 0.3.3
+Version: 0.3.4
 Summary: Open-source library containing database about animes/series and including a built-in utility.
 Project-URL: Github, https://github.com/swarthur/animedata
 Project-URL: Bug, https://github.com/swarthur/animedata/issues
 Author: swarthur
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

