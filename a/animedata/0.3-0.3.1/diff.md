# Comparing `tmp/animedata-0.3.tar.gz` & `tmp/animedata-0.3.1.tar.gz`

## Comparing `animedata-0.3.tar` & `animedata-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3/ad_test.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 animedata-0.3/animedata.py
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3/animedata_source.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3/LICENSE
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 animedata-0.3/pyproject.toml
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 animedata-0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.1/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 animedata-0.3.1/ad_test.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 animedata-0.3.1/animedata.py
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 animedata-0.3.1/animedata_source.json
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 animedata-0.3.1/path.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 animedata-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.1/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 animedata-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 animedata-0.3.1/PKG-INFO
```

### Comparing `animedata-0.3/ad_test.py` & `animedata-0.3.1/ad_test.py`

 * *Files identical despite different names*

### Comparing `animedata-0.3/animedata.py` & `animedata-0.3.1/animedata.py`

 * *Files identical despite different names*

### Comparing `animedata-0.3/animedata_source.json` & `animedata-0.3.1/animedata_source.json`

 * *Files identical despite different names*

### Comparing `animedata-0.3/LICENSE` & `animedata-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animedata-0.3/README.md` & `animedata-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `animedata-0.3/pyproject.toml` & `animedata-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 00000050: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
 00000060: 5d0d 0a65 7863 6c75 6465 203d 205b 0d0a  ]..exclude = [..
 00000070: 2020 222f 6469 7374 222c 0d0a 2020 222f    "/dist",..  "/
 00000080: 2e67 6974 222c 0d0a 2020 222e 6769 7469  .git",..  ".giti
 00000090: 676e 6f72 6522 0d0a 2020 5d0d 0a0d 0a5b  gnore"..  ]....[
 000000a0: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 000000b0: 2022 616e 696d 6564 6174 6122 0d0a 7665   "animedata"..ve
-000000c0: 7273 696f 6e20 3d20 2230 2e33 220d 0a61  rsion = "0.3"..a
-000000d0: 7574 686f 7273 203d 205b 0d0a 207b 6e61  uthors = [.. {na
-000000e0: 6d65 3d22 7377 6172 7468 7572 227d 0d0a  me="swarthur"}..
-000000f0: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
-00000100: 2022 4f70 656e 2d73 6f75 7263 6520 6c69   "Open-source li
-00000110: 6272 6172 7920 636f 6e74 6169 6e69 6e67  brary containing
-00000120: 2064 6174 6162 6173 6520 6162 6f75 7420   database about 
-00000130: 616e 696d 6573 2f73 6572 6965 7320 616e  animes/series an
-00000140: 6420 696e 636c 7564 696e 6720 6120 6275  d including a bu
-00000150: 696c 742d 696e 2075 7469 6c69 7479 2e22  ilt-in utility."
-00000160: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-00000170: 4d45 2e6d 6422 0d0a 7265 7175 6972 6573  ME.md"..requires
-00000180: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
-00000190: 3122 0d0a 6c69 6365 6e73 6520 3d20 224d  1"..license = "M
-000001a0: 4954 220d 0a63 6c61 7373 6966 6965 7273  IT"..classifiers
-000001b0: 203d 205b 0d0a 2020 2020 2250 726f 6772   = [..    "Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
-000001e0: 0d0a 2020 2020 224c 6963 656e 7365 203a  ..    "License :
-000001f0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000200: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
-00000210: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000220: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000230: 6570 656e 6465 6e74 222c 0d0a 5d0d 0a0d  ependent",..]...
-00000240: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000250: 0a22 4769 7468 7562 2220 3d20 2268 7474  ."Github" = "htt
-00000260: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000270: 7377 6172 7468 7572 2f61 6e69 6d65 6461  swarthur/animeda
-00000280: 7461 220d 0a22 4275 6722 203d 2022 6874  ta".."Bug" = "ht
-00000290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002a0: 2f73 7761 7274 6875 722f 616e 696d 6564  /swarthur/animed
-000002b0: 6174 612f 6973 7375 6573 220d 0a         ata/issues"..
+000000c0: 7273 696f 6e20 3d20 2230 2e33 2e31 220d  rsion = "0.3.1".
+000000d0: 0a61 7574 686f 7273 203d 205b 0d0a 207b  .authors = [.. {
+000000e0: 6e61 6d65 3d22 7377 6172 7468 7572 227d  name="swarthur"}
+000000f0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
+00000100: 203d 2022 4f70 656e 2d73 6f75 7263 6520   = "Open-source 
+00000110: 6c69 6272 6172 7920 636f 6e74 6169 6e69  library containi
+00000120: 6e67 2064 6174 6162 6173 6520 6162 6f75  ng database abou
+00000130: 7420 616e 696d 6573 2f73 6572 6965 7320  t animes/series 
+00000140: 616e 6420 696e 636c 7564 696e 6720 6120  and including a 
+00000150: 6275 696c 742d 696e 2075 7469 6c69 7479  built-in utility
+00000160: 2e22 0d0a 7265 6164 6d65 203d 2022 5245  ."..readme = "RE
+00000170: 4144 4d45 2e6d 6422 0d0a 7265 7175 6972  ADME.md"..requir
+00000180: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
+00000190: 2e31 3122 0d0a 6c69 6365 6e73 6520 3d20  .11"..license = 
+000001a0: 224d 4954 220d 0a63 6c61 7373 6966 6965  "MIT"..classifie
+000001b0: 7273 203d 205b 0d0a 2020 2020 2250 726f  rs = [..    "Pro
+000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001e0: 222c 0d0a 2020 2020 224c 6963 656e 7365  ",..    "License
+000001f0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000200: 203a 3a20 4d49 5420 4c69 6365 6e73 6522   :: MIT License"
+00000210: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
+00000220: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000230: 6e64 6570 656e 6465 6e74 222c 0d0a 5d0d  ndependent",..].
+00000240: 0a0d 0a5b 7072 6f6a 6563 742e 7572 6c73  ...[project.urls
+00000250: 5d0d 0a22 4769 7468 7562 2220 3d20 2268  ].."Github" = "h
+00000260: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000270: 6d2f 7377 6172 7468 7572 2f61 6e69 6d65  m/swarthur/anime
+00000280: 6461 7461 220d 0a22 4275 6722 203d 2022  data".."Bug" = "
+00000290: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002a0: 6f6d 2f73 7761 7274 6875 722f 616e 696d  om/swarthur/anim
+000002b0: 6564 6174 612f 6973 7375 6573 220d 0a    edata/issues"..
```

### Comparing `animedata-0.3/PKG-INFO` & `animedata-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animedata
-Version: 0.3
+Version: 0.3.1
 Summary: Open-source library containing database about animes/series and including a built-in utility.
 Project-URL: Github, https://github.com/swarthur/animedata
 Project-URL: Bug, https://github.com/swarthur/animedata/issues
 Author: swarthur
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

