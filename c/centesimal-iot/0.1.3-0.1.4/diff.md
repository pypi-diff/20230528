# Comparing `tmp/centesimal_iot-0.1.3-py2.py3-none-any.whl.zip` & `tmp/centesimal_iot-0.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24181 bytes, number of entries: 24
+Zip file size: 24190 bytes, number of entries: 24
 -rw-rw-r--  2.0 unx      127 b- defN 23-May-26 11:14 iot/__init__.py
 -rw-rw-r--  2.0 unx      387 b- defN 23-Apr-17 09:42 iot/cli.py
 -rw-rw-r--  2.0 unx     4957 b- defN 23-Apr-17 11:32 iot/helpers.py
 -rw-rw-r--  2.0 unx       51 b- defN 23-Apr-17 09:52 iot/iot.py
 -rw-rw-r--  2.0 unx      795 b- defN 23-May-25 16:27 iot/cli/__init__.py
 -rw-rw-r--  2.0 unx     5068 b- defN 23-Apr-26 09:33 iot/cli/describe.py
 -rw-rw-r--  2.0 unx     4549 b- defN 23-May-28 10:44 iot/cli/inventory.py
@@ -13,14 +13,14 @@
 -rw-rw-r--  2.0 unx     3247 b- defN 23-May-23 15:23 iot/cli/target.py
 -rw-rw-r--  2.0 unx     3246 b- defN 23-Apr-26 17:36 iot/cli/test.py
 -rw-rw-r--  2.0 unx     1795 b- defN 23-Apr-26 09:30 iot/cli/users.py
 -rw-rw-r--  2.0 unx     3258 b- defN 23-May-23 15:23 iot/cli/watch.py
 -rw-rw-r--  2.0 unx    15853 b- defN 23-May-20 17:56 iot/cli/wingdbstub.py
 -rw-rw-r--  2.0 unx     1918 b- defN 23-Apr-26 09:35 iot/cli/workspaces.py
 -rw-rw-r--  2.0 unx     2766 b- defN 23-May-26 09:41 iot/tools/__init__.py
--rw-rw-r--  2.0 unx      162 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/AUTHORS.rst
--rw-rw-r--  2.0 unx     1071 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       37 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1841 b- defN 23-May-28 10:58 centesimal_iot-0.1.3.dist-info/RECORD
-24 files, 59078 bytes uncompressed, 21257 bytes compressed:  64.0%
+-rw-rw-r--  2.0 unx      162 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/AUTHORS.rst
+-rw-rw-r--  2.0 unx     1222 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       37 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1841 b- defN 23-May-28 11:05 centesimal_iot-0.1.4.dist-info/RECORD
+24 files, 59229 bytes uncompressed, 21266 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -48,26 +48,26 @@
 
 Filename: iot/cli/workspaces.py
 Comment: 
 
 Filename: iot/tools/__init__.py
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/AUTHORS.rst
+Filename: centesimal_iot-0.1.4.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/METADATA
+Filename: centesimal_iot-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/WHEEL
+Filename: centesimal_iot-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/entry_points.txt
+Filename: centesimal_iot-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/top_level.txt
+Filename: centesimal_iot-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: centesimal_iot-0.1.3.dist-info/RECORD
+Filename: centesimal_iot-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `centesimal_iot-0.1.3.dist-info/METADATA` & `centesimal_iot-0.1.4.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: centesimal-iot
-Version: 0.1.3
+Version: 0.1.4
 Summary: IoT infrastructure
 Home-page: https://github.com/asterio.gonzalez/iot
 Author: Asterio Gonzalez
 Author-email: apastor@cibernos.com
 Keywords: iot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
 License-File: AUTHORS.rst
 Requires-Dist: Click (>=7.0)
 Requires-Dist: pycelium
 
 ===
 iot
 ===
```

## Comparing `centesimal_iot-0.1.3.dist-info/RECORD` & `centesimal_iot-0.1.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 iot/cli/target.py,sha256=bRXllA2pvqKORTFe_Yohmh87JkekpHTCg-qMW_RiC-A,3247
 iot/cli/test.py,sha256=C0lqt8IQEGo2cOoHR43G1jcAlkoOillZ2Q0WYfV7H1A,3246
 iot/cli/users.py,sha256=sair249wY-fG4E6ayZIpxDcI6IxVY2UcItOnc85zlwE,1795
 iot/cli/watch.py,sha256=-ZUVZEaHvuL0zbKHnzGPVjBaOzcyj6-naP4GOx0kjjQ,3258
 iot/cli/wingdbstub.py,sha256=lV72joWEBWLtQM-SaDZchxe72UGZkhaa1dT0h192vpI,15853
 iot/cli/workspaces.py,sha256=6XRO-aYZy_aFXHoIbumlpHTmEFPyylMBIaR1RbI57Ns,1918
 iot/tools/__init__.py,sha256=AVGIL_fR5ChEV9r692EWA0eNHZFeeO3tydt85jnGBu4,2766
-centesimal_iot-0.1.3.dist-info/AUTHORS.rst,sha256=DJWRsAX9L2yG7FsyDzWBb8G9Oeb0cvjnUxyPZR_5elM,162
-centesimal_iot-0.1.3.dist-info/METADATA,sha256=0VgvmGsx1DmoR9My-FuA1jDhXNVLdopIGCNJT9JsP9o,1071
-centesimal_iot-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-centesimal_iot-0.1.3.dist-info/entry_points.txt,sha256=shS0YwmHrq5G3uFwO3YHoSeUmRstZj4KcaJW-bn5CB4,37
-centesimal_iot-0.1.3.dist-info/top_level.txt,sha256=GrFBYwTe_zimcbxQb9lowAJUNeDArWJA0esDNiSx9Kw,4
-centesimal_iot-0.1.3.dist-info/RECORD,,
+centesimal_iot-0.1.4.dist-info/AUTHORS.rst,sha256=DJWRsAX9L2yG7FsyDzWBb8G9Oeb0cvjnUxyPZR_5elM,162
+centesimal_iot-0.1.4.dist-info/METADATA,sha256=_y6jlCwyBnnJfzuRYPOD8j8IiK5rJk0QnEfa6uhY-yk,1222
+centesimal_iot-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+centesimal_iot-0.1.4.dist-info/entry_points.txt,sha256=shS0YwmHrq5G3uFwO3YHoSeUmRstZj4KcaJW-bn5CB4,37
+centesimal_iot-0.1.4.dist-info/top_level.txt,sha256=GrFBYwTe_zimcbxQb9lowAJUNeDArWJA0esDNiSx9Kw,4
+centesimal_iot-0.1.4.dist-info/RECORD,,
```

