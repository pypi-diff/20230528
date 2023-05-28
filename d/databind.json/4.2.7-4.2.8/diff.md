# Comparing `tmp/databind.json-4.2.7-py3-none-any.whl.zip` & `tmp/databind.json-4.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12833 bytes, number of entries: 8
+Zip file size: 12831 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     2358 b- defN 80-Jan-01 00:00 databind/json/__init__.py
 -rw-r--r--  2.0 unx    33037 b- defN 80-Jan-01 00:00 databind/json/converters.py
 -rw-r--r--  2.0 unx     2706 b- defN 80-Jan-01 00:00 databind/json/module.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 databind/json/py.typed
 -rw-r--r--  2.0 unx     1773 b- defN 80-Jan-01 00:00 databind/json/settings.py
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 databind.json-4.2.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4368 b- defN 16-Jan-01 00:00 databind.json-4.2.7.dist-info/METADATA
-?rw-r--r--  2.0 unx      629 b- defN 16-Jan-01 00:00 databind.json-4.2.7.dist-info/RECORD
-8 files, 44954 bytes uncompressed, 11741 bytes compressed:  73.9%
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 databind.json-4.2.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4368 b- defN 16-Jan-01 00:00 databind.json-4.2.8.dist-info/METADATA
+?rw-r--r--  2.0 unx      629 b- defN 16-Jan-01 00:00 databind.json-4.2.8.dist-info/RECORD
+8 files, 44954 bytes uncompressed, 11739 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -9,17 +9,17 @@
 
 Filename: databind/json/py.typed
 Comment: 
 
 Filename: databind/json/settings.py
 Comment: 
 
-Filename: databind.json-4.2.7.dist-info/WHEEL
+Filename: databind.json-4.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: databind.json-4.2.7.dist-info/METADATA
+Filename: databind.json-4.2.8.dist-info/METADATA
 Comment: 
 
-Filename: databind.json-4.2.7.dist-info/RECORD
+Filename: databind.json-4.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databind/json/__init__.py

```diff
@@ -5,15 +5,15 @@
 
 from databind.core.utils import T
 
 if t.TYPE_CHECKING:
     from databind.core.mapper import ObjectMapper
     from databind.core.settings import Setting, Settings
 
-__version__ = "4.2.7"
+__version__ = "4.2.8"
 
 JsonType = t.Union[
     None,
     bool,
     int,
     float,
     str,
```

## Comparing `databind.json-4.2.7.dist-info/METADATA` & `databind.json-4.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: databind.json
-Version: 4.2.7
+Version: 4.2.8
 Summary: De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.2.7,<5.0.0)
+Requires-Dist: databind.core (>=4.2.8,<5.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: typeapi (>=1.4.2,<2.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
```

## Comparing `databind.json-4.2.7.dist-info/RECORD` & `databind.json-4.2.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-databind/json/__init__.py,sha256=Uyy4VryCkUXetqgFKN2cdpTR44yrtL9hg2_uTxLdF9A,2358
+databind/json/__init__.py,sha256=MaKam_nBlUfwZ_LNo5zuLvWa71NTmVWseJTEKm5bBhY,2358
 databind/json/converters.py,sha256=FixNdlIfyWQEKFhY17LMVi72D_BBPnjavoHS-2aIxJU,33037
 databind/json/module.py,sha256=CiFQBB1osjS6VIpnKQo84JwncfypfXKGmbuOToZAeMI,2706
 databind/json/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databind/json/settings.py,sha256=zTcKnUgq4SlEK7CjbMt5Iyh_z1FnVOaAocM_165sFYY,1773
-databind.json-4.2.7.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-databind.json-4.2.7.dist-info/METADATA,sha256=Svm299dVflT7vnWye73AOZk0AmnH6liywtcmyr7MxSA,4368
-databind.json-4.2.7.dist-info/RECORD,,
+databind.json-4.2.8.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+databind.json-4.2.8.dist-info/METADATA,sha256=KNySRZn5sL4AQMV7moHWb4x6jKd09YfNvrd-uehj2E8,4368
+databind.json-4.2.8.dist-info/RECORD,,
```

