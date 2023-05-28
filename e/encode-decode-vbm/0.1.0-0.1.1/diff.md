# Comparing `tmp/encode_decode_vbm-0.1.0.tar.gz` & `tmp/encode_decode_vbm-0.1.1.tar.gz`

## Comparing `encode_decode_vbm-0.1.0.tar` & `encode_decode_vbm-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/decode.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/encode.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/b32.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/b64.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/salter.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/sha256.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/sha_funcs.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/vigenere.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/LICENSE
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/decode.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/encode.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b32.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b64.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/salter.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha256.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha_funcs.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/vigenere.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/LICENSE
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/PKG-INFO
```

### Comparing `encode_decode_vbm-0.1.0/.DS_Store` & `encode_decode_vbm-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/.DS_Store` & `encode_decode_vbm-0.1.1/src/.DS_Store`

 * *Files 15% similar despite different names*

```diff
@@ -26,37 +26,37 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0003 0000 000d  ................
+00000200: 0000 0000 0000 0000 0000 0003 0000 0011  ................
 00000210: 0065 006e 0063 006f 0064 0065 005f 0064  .e.n.c.o.d.e._.d
-00000220: 0065 0063 006f 0064 0065 496c 6f63 626c  .e.c.o.d.eIlocbl
-00000230: 6f62 0000 0010 0000 0041 0000 002e ffff  ob.......A......
-00000240: ffff ffff 0000 0000 000d 0065 006e 0063  ...........e.n.c
-00000250: 006f 0064 0065 005f 0064 0065 0063 006f  .o.d.e._.d.e.c.o
-00000260: 0064 0065 6277 7370 626c 6f62 0000 00bb  .d.ebwspblob....
-00000270: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-00000280: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00000290: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-000002a0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-000002b0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-000002c0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-000002d0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-000002e0: 101b 7b7b 3139 3931 2c20 2d35 367d 2c20  ..{{1991, -56}, 
-000002f0: 7b31 3638 302c 2031 3032 357d 7d09 0815  {1680, 1025}}...
-00000300: 232f 3b52 5f6b 6c6d 6e6f 8d00 0000 0000  #/;R_klmno......
-00000310: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 8e00 0000 0d00  ................
-00000330: 6500 6e00 6300 6f00 6400 6500 5f00 6400  e.n.c.o.d.e._.d.
-00000340: 6500 6300 6f00 6400 6576 5372 6e6c 6f6e  e.c.o.d.evSrnlon
-00000350: 6700 0000 0100 0000 0000 0000 0000 0000  g...............
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0065 0063 006f 0064 0065 005f 0076 0062  .e.c.o.d.e._.v.b
+00000230: 006d 496c 6f63 626c 6f62 0000 0010 0000  .mIlocblob......
+00000240: 0041 0000 002e ffff ffff ffff 0000 0000  .A..............
+00000250: 0011 0065 006e 0063 006f 0064 0065 005f  ...e.n.c.o.d.e._
+00000260: 0064 0065 0063 006f 0064 0065 005f 0076  .d.e.c.o.d.e._.v
+00000270: 0062 006d 6277 7370 626c 6f62 0000 00ba  .b.mbwspblob....
+00000280: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+00000290: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+000002a0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+000002b0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+000002c0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+000002d0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000002e0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+000002f0: 101a 7b7b 3139 3932 2c20 3135 7d2c 207b  ..{{1992, 15}, {
+00000300: 3136 3830 2c20 3130 3235 7d7d 0908 1523  1680, 1025}}...#
+00000310: 2f3b 525f 6b6c 6d6e 6f8c 0000 0000 0000  /;R_klmno.......
+00000320: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 008d 0000 0011 0065  ...............e
+00000340: 006e 0063 006f 0064 0065 005f 0064 0065  .n.c.o.d.e._.d.e
+00000350: 0063 006f 0064 0065 005f 0076 0062 006d  .c.o.d.e._.v.b.m
+00000360: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/decode.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/decode.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/b32.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b32.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/b64.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b64.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/sha256.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha256.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/sha_funcs.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha_funcs.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/src/encode_decode_vbm/funcs/vigenere.py` & `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/vigenere.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/LICENSE` & `encode_decode_vbm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.0/pyproject.toml` & `encode_decode_vbm-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "encode_decode_vbm"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Vidak-Becs Mate", email = "matevidakbecs@gmail.com" }]
 description = "encoding and decoding library for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `encode_decode_vbm-0.1.0/PKG-INFO` & `encode_decode_vbm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode_decode_vbm
-Version: 0.1.0
+Version: 0.1.1
 Summary: encoding and decoding library for python
 Project-URL: Homepage, https://github.com/mate12392/encode_decode_py
 Author-email: Vidak-Becs Mate <matevidakbecs@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

