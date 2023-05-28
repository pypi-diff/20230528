# Comparing `tmp/xcodex-0.0.1-py3-none-any.whl.zip` & `tmp/xcodex-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12740 bytes, number of entries: 19
+Zip file size: 12727 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-03 11:34 Util/__init__.py
 -rw-rw-rw-  2.0 fat      641 b- defN 23-May-27 11:38 Util/check.py
 -rw-rw-rw-  2.0 fat      353 b- defN 23-May-27 14:23 Util/create_dodsrc.py
 -rw-rw-rw-  2.0 fat      415 b- defN 23-May-27 14:23 Util/create_netrc.py
 -rw-rw-rw-  2.0 fat      671 b- defN 23-May-27 15:46 Util/date.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-May-27 15:12 Util/download.py
 -rw-rw-rw-  2.0 fat      506 b- defN 23-May-27 12:34 Util/download_data.py
 -rw-rw-rw-  2.0 fat     1567 b- defN 23-May-27 12:20 Util/download_file_progress.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-May-27 12:20 Util/generate_links.py
 -rw-rw-rw-  2.0 fat     1248 b- defN 23-May-27 13:50 Util/make_Dataframe.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-May-27 14:05 Util/missing.py
 -rw-rw-rw-  2.0 fat      931 b- defN 23-May-27 11:49 Util/var_imp.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-03 11:34 xcodex/__init__.py
 -rw-rw-rw-  2.0 fat     6613 b- defN 23-May-27 17:54 xcodex/main.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-May-27 19:11 xcodex-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6062 b- defN 23-May-27 19:11 xcodex-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 19:11 xcodex-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-27 19:11 xcodex-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1421 b- defN 23-May-27 19:11 xcodex-0.0.1.dist-info/RECORD
-19 files, 24660 bytes uncompressed, 10456 bytes compressed:  57.6%
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-May-28 12:36 xcodex-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6034 b- defN 23-May-28 12:36 xcodex-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 12:36 xcodex-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-28 12:36 xcodex-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1421 b- defN 23-May-28 12:36 xcodex-0.0.2.dist-info/RECORD
+19 files, 24632 bytes uncompressed, 10443 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: xcodex/__init__.py
 Comment: 
 
 Filename: xcodex/main.py
 Comment: 
 
-Filename: xcodex-0.0.1.dist-info/LICENSE
+Filename: xcodex-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: xcodex-0.0.1.dist-info/METADATA
+Filename: xcodex-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xcodex-0.0.1.dist-info/WHEEL
+Filename: xcodex-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xcodex-0.0.1.dist-info/top_level.txt
+Filename: xcodex-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xcodex-0.0.1.dist-info/RECORD
+Filename: xcodex-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `xcodex-0.0.1.dist-info/LICENSE` & `xcodex-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xcodex-0.0.1.dist-info/METADATA` & `xcodex-0.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: xcodex
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package will extract daily data from netCDF4 files downloaded at GES DISC database"
 Author: henriquefl24@git
 Author-email: Henrique Fontellas Laurito <henrique.f.laurito@unesp.br>
 Project-URL: Homepage, https://github.com/henriquefl24/xcodex
 Project-URL: Bug Tracker, https://github.com/henriquefl24/xcodex/issues
 Keywords: python,NASA,GES DISC,XCO2,daily,OCO-2,jupyter notebook,xcodex
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: netCDF4
 Requires-Dist: jupyter
 Requires-Dist: requests
 Requires-Dist: setuptools
 
-<img height="200" src="logo_gas.jpg" width="550" alt="logo"/> <br>
+![logo](D:\Git\xcodex\logo_gas.jpg) <br>
 
 # **Welcome to XCODEX - XCO2 Daily EXtractor**
 
 Hi there! My name is Henrique.
 
 The creation of this Python package was intended to create a simple solution for extracting daily data from XCO2 retrieved from the GES DISC platform.
```

## Comparing `xcodex-0.0.1.dist-info/RECORD` & `xcodex-0.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 Util/download_file_progress.py,sha256=azEK6sBJwTa6U4_1DKN_Bw3eB-7kPDUEzAvxgTIfhJ0,1567
 Util/generate_links.py,sha256=xxLaSq9-seZ-TXCEnJ290s15dNJoqv7FTw6Q1fR-0qA,644
 Util/make_Dataframe.py,sha256=PRP1Ly0A_iK7jop2vihbAeWfy4aeryQCmCLw_qHhLC4,1248
 Util/missing.py,sha256=35VDt5dENvtlXvlfZPFl9s6jUISTQtybSyBa4BTyx-o,1047
 Util/var_imp.py,sha256=ITs7vsWm1wrcxoDqnpkwUflwtTgsKng_dmkSCLA4ZZ4,931
 xcodex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xcodex/main.py,sha256=RA3uBj1U3JHi0hKMoRe7LgLYb_CFZfkxpQVG3DxGLXo,6613
-xcodex-0.0.1.dist-info/LICENSE,sha256=wiLVM6zHzr69ULNwUrxRAlTZBf8j_xtUvKrLPgP98K8,1097
-xcodex-0.0.1.dist-info/METADATA,sha256=Zc-20MDXbtD3fXoJW29EIXM2ZOkyhSiP_PVz6e_xJ5c,6062
-xcodex-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-xcodex-0.0.1.dist-info/top_level.txt,sha256=t8cwNIdQesVwGdWqlkzTh-AdzTVvQb3YI3F3Ab6pjNs,12
-xcodex-0.0.1.dist-info/RECORD,,
+xcodex-0.0.2.dist-info/LICENSE,sha256=wiLVM6zHzr69ULNwUrxRAlTZBf8j_xtUvKrLPgP98K8,1097
+xcodex-0.0.2.dist-info/METADATA,sha256=dRoWpfFebBaxC09l2FOZS0lzQ0udxi4DC01dXF66Ei4,6034
+xcodex-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+xcodex-0.0.2.dist-info/top_level.txt,sha256=t8cwNIdQesVwGdWqlkzTh-AdzTVvQb3YI3F3Ab6pjNs,12
+xcodex-0.0.2.dist-info/RECORD,,
```

