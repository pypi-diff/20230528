# Comparing `tmp/faceid-lib-2.0.2.tar.gz` & `tmp/faceid-lib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid-lib-2.0.2.tar", max compression
+gzip compressed data, was "faceid-lib-3.0.0.tar", max compression
```

## Comparing `faceid-lib-2.0.2.tar` & `faceid-lib-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,34 @@
--rw-r--r--   0        0        0     2640 2023-05-28 15:35:29.796981 faceid-lib-2.0.2/README.md
--rw-r--r--   0        0        0     2235 2023-05-26 08:43:24.659565 faceid-lib-2.0.2/build.py
--rw-r--r--   0        0        0      590 2023-05-26 07:24:21.410634 faceid-lib-2.0.2/faceid_lib/CHANGELOG.md
--rw-r--r--   0        0        0      240 2023-05-26 08:41:56.166622 faceid-lib-2.0.2/faceid_lib/Makefile
--rwxr-xr-x   0        0        0    39408 2023-05-28 15:42:19.000000 faceid-lib-2.0.2/faceid_lib/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    47040 2023-05-28 15:42:20.000000 faceid-lib-2.0.2/faceid_lib/__main__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    39024 2023-05-28 15:42:37.000000 faceid-lib-2.0.2/faceid_lib/events/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    96640 2023-05-28 15:42:34.000000 faceid-lib-2.0.2/faceid_lib/events/event_producer.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    96400 2023-05-28 15:42:37.000000 faceid-lib-2.0.2/faceid_lib/events/event_receiver.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    39024 2023-05-28 15:42:20.000000 faceid-lib-2.0.2/faceid_lib/logger/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    65280 2023-05-28 15:42:21.000000 faceid-lib-2.0.2/faceid_lib/logger/logger_helper.cpython-38-darwin.so
--rwxr-xr-x   0        0        0   128696 2023-05-28 15:42:27.000000 faceid-lib-2.0.2/faceid_lib/ratelimiter/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0   122464 2023-05-28 15:42:24.000000 faceid-lib-2.0.2/faceid_lib/ratelimiter/depends.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    39160 2023-05-28 15:42:27.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    39104 2023-05-28 15:42:28.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    68360 2023-05-28 15:42:29.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/power.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    39048 2023-05-28 15:42:32.000000 faceid-lib-2.0.2/faceid_lib/workflow/__init__.cpython-38-darwin.so
--rwxr-xr-x   0        0        0    66688 2023-05-28 15:42:31.000000 faceid-lib-2.0.2/faceid_lib/workflow/workflow_helper.cpython-38-darwin.so
--rw-r--r--   0        0        0     1629 2023-05-28 15:41:41.440546 faceid-lib-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3696 2023-05-28 15:43:09.081791 faceid-lib-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2640 2023-05-28 15:57:17.547252 faceid-lib-3.0.0/README.md
+-rw-r--r--   0        0        0     2235 2023-05-28 15:57:16.403237 faceid-lib-3.0.0/build.py
+-rw-r--r--   0        0        0      590 2023-05-28 15:57:27.259372 faceid-lib-3.0.0/faceid_lib/CHANGELOG.md
+-rw-r--r--   0        0        0      240 2023-05-28 15:57:27.403374 faceid-lib-3.0.0/faceid_lib/Makefile
+-rwxr-xr-x   0        0        0    39408 2023-05-28 15:57:27.347373 faceid-lib-3.0.0/faceid_lib/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75744 2023-05-28 16:21:30.000000 faceid-lib-3.0.0/faceid_lib/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    47040 2023-05-28 15:57:27.915380 faceid-lib-3.0.0/faceid_lib/__main__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   173704 2023-05-28 16:21:30.000000 faceid-lib-3.0.0/faceid_lib/__main__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    39024 2023-05-28 15:57:28.395386 faceid-lib-3.0.0/faceid_lib/events/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75312 2023-05-28 16:21:31.000000 faceid-lib-3.0.0/faceid_lib/events/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    96640 2023-05-28 15:57:28.603389 faceid-lib-3.0.0/faceid_lib/events/event_producer.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   641600 2023-05-28 16:21:32.000000 faceid-lib-3.0.0/faceid_lib/events/event_producer.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    96400 2023-05-28 15:57:28.531388 faceid-lib-3.0.0/faceid_lib/events/event_receiver.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   707176 2023-05-28 16:21:34.000000 faceid-lib-3.0.0/faceid_lib/events/event_receiver.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    39024 2023-05-28 15:57:26.747366 faceid-lib-3.0.0/faceid_lib/logger/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75312 2023-05-28 16:21:35.000000 faceid-lib-3.0.0/faceid_lib/logger/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    65280 2023-05-28 15:57:26.711365 faceid-lib-3.0.0/faceid_lib/logger/logger_helper.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   236504 2023-05-28 16:21:36.000000 faceid-lib-3.0.0/faceid_lib/logger/logger_helper.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0   128696 2023-05-28 15:57:27.039369 faceid-lib-3.0.0/faceid_lib/ratelimiter/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   744048 2023-05-28 16:21:38.000000 faceid-lib-3.0.0/faceid_lib/ratelimiter/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0   122464 2023-05-28 15:57:26.947368 faceid-lib-3.0.0/faceid_lib/ratelimiter/depends.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   702080 2023-05-28 16:21:40.000000 faceid-lib-3.0.0/faceid_lib/ratelimiter/depends.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    39160 2023-05-28 15:57:27.827379 faceid-lib-3.0.0/faceid_lib/vector_similarity/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75440 2023-05-28 16:21:34.000000 faceid-lib-3.0.0/faceid_lib/vector_similarity/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    39104 2023-05-28 15:57:27.603376 faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75392 2023-05-28 16:21:34.000000 faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    68360 2023-05-28 15:57:27.559376 faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/power.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   257968 2023-05-28 16:21:35.000000 faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/power.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    39048 2023-05-28 15:57:28.015382 faceid-lib-3.0.0/faceid_lib/workflow/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    75344 2023-05-28 16:21:37.000000 faceid-lib-3.0.0/faceid_lib/workflow/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    66688 2023-05-28 15:57:28.151383 faceid-lib-3.0.0/faceid_lib/workflow/workflow_helper.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   252760 2023-05-28 16:21:36.000000 faceid-lib-3.0.0/faceid_lib/workflow/workflow_helper.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1780 2023-05-28 16:26:34.909247 faceid-lib-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3846 2023-05-28 16:26:57.456164 faceid-lib-3.0.0/PKG-INFO
```

### Comparing `faceid-lib-2.0.2/README.md` & `faceid-lib-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.2/build.py` & `faceid-lib-3.0.0/build.py`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.2/faceid_lib/CHANGELOG.md` & `faceid-lib-3.0.0/faceid_lib/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.2/faceid_lib/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -312,15 +312,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/__init__.o (1790)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473765B
+    Value: 0x64737693
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2161,15 +2161,15 @@
 00008700: f405 0000 0e0d 0000 1044 0000 0000 0000  .........D......
 00008710: 2006 0000 0e0d 0000 1844 0000 0000 0000   ........D......
 00008720: 5106 0000 0e0d 0000 2044 0000 0000 0000  Q....... D......
 00008730: 6506 0000 0e0d 0000 2844 0000 0000 0000  e.......(D......
 00008740: 7906 0000 0e0d 0000 3044 0000 0000 0000  y.......0D......
 00008750: 8d06 0000 6400 0000 0000 0000 0000 0000  ....d...........
 00008760: f306 0000 6400 0000 0000 0000 0000 0000  ....d...........
-00008770: fe06 0000 6603 0100 5b76 7364 0000 0000  ....f...[vsd....
+00008770: fe06 0000 6603 0100 9376 7364 0000 0000  ....f....vsd....
 00008780: 0100 0000 2e01 0000 902c 0000 0000 0000  .........,......
 00008790: 9007 0000 2401 0000 902c 0000 0000 0000  ....$....,......
 000087a0: a307 0000 8400 0000 0000 0000 0000 0000  ................
 000087b0: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 000087c0: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 000087d0: 0100 0000 2e01 0000 b02c 0000 0000 0000  .........,......
 000087e0: c607 0000 2401 0000 b02c 0000 0000 0000  ....$....,......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/__main__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/__main__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -708,15 +708,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/__main__.o (3694)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473765C
+    Value: 0x64737694
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2259,15 +2259,15 @@
 00008d20: 404b 0000 0000 0000 900d 0000 0e0d 0000  @K..............
 00008d30: 484b 0000 0000 0000 c10d 0000 0e0d 0000  HK..............
 00008d40: 504b 0000 0000 0000 d50d 0000 0e0d 0000  PK..............
 00008d50: 584b 0000 0000 0000 e90d 0000 0e0d 0000  XK..............
 00008d60: 604b 0000 0000 0000 fd0d 0000 6400 0000  `K..........d...
 00008d70: 0000 0000 0000 0000 630e 0000 6400 0000  ........c...d...
 00008d80: 0000 0000 0000 0000 6e0e 0000 6603 0100  ........n...f...
-00008d90: 5c76 7364 0000 0000 0100 0000 2e01 0000  \vsd............
+00008d90: 9476 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 00008da0: 200d 0000 0000 0000 000f 0000 2401 0000   ...........$...
 00008db0: 200d 0000 0000 0000 110f 0000 8400 0000   ...............
 00008dc0: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008dd0: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 00008de0: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 00008df0: 400d 0000 0000 0000 340f 0000 2401 0000  @.......4...$...
 00008e00: 400d 0000 0000 0000 480f 0000 8400 0000  @.......H.......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/events/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/events/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -267,15 +267,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/events/__init__.o (1699)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473766D
+    Value: 0x647376A5
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2154,15 +2154,15 @@
 00008690: c042 0000 0000 0000 be05 0000 0e0c 0000  .B..............
 000086a0: c842 0000 0000 0000 ef05 0000 0e0c 0000  .B..............
 000086b0: d042 0000 0000 0000 0306 0000 0e0c 0000  .B..............
 000086c0: d842 0000 0000 0000 1706 0000 0e0c 0000  .B..............
 000086d0: e042 0000 0000 0000 2b06 0000 6400 0000  .B......+...d...
 000086e0: 0000 0000 0000 0000 9806 0000 6400 0000  ............d...
 000086f0: 0000 0000 0000 0000 a306 0000 6603 0100  ............f...
-00008700: 6d76 7364 0000 0000 0100 0000 2e01 0000  mvsd............
+00008700: a576 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 00008710: 902c 0000 0000 0000 3c07 0000 2401 0000  .,......<...$...
 00008720: 902c 0000 0000 0000 4b07 0000 8400 0000  .,......K.......
 00008730: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008740: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 00008750: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 00008760: b02c 0000 0000 0000 7507 0000 2401 0000  .,......u...$...
 00008770: b02c 0000 0000 0000 8907 0000 8400 0000  .,..............
```

### Comparing `faceid-lib-2.0.2/faceid_lib/events/event_producer.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/events/event_producer.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -2148,15 +2148,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/events/event_producer.o (9062)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473766A
+    Value: 0x647376A2
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -4499,15 +4499,15 @@
 00011920: 88d9 0000 0000 0000 7b22 0000 0e0d 0000  ........{"......
 00011930: 90d9 0000 0000 0000 ac22 0000 0e0d 0000  ........."......
 00011940: 98d9 0000 0000 0000 c022 0000 0e0d 0000  ........."......
 00011950: a0d9 0000 0000 0000 d422 0000 0e0d 0000  ........."......
 00011960: a8d9 0000 0000 0000 e822 0000 6400 0000  ........."..d...
 00011970: 0000 0000 0000 0000 5523 0000 6400 0000  ........U#..d...
 00011980: 0000 0000 0000 0000 6623 0000 6603 0100  ........f#..f...
-00011990: 6a76 7364 0000 0000 0100 0000 2e01 0000  jvsd............
+00011990: a276 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 000119a0: d031 0000 0000 0000 0524 0000 2401 0000  .1.......$..$...
 000119b0: d031 0000 0000 0000 1c24 0000 8400 0000  .1.......$......
 000119c0: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 000119d0: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 000119e0: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 000119f0: f031 0000 0000 0000 4c24 0000 2401 0000  .1......L$..$...
 00011a00: f031 0000 0000 0000 6024 0000 8400 0000  .1......`$......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/events/event_receiver.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/events/event_receiver.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -2139,15 +2139,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/events/event_receiver.o (8911)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473766D
+    Value: 0x647376A5
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -4502,15 +4502,15 @@
 00011950: b821 0000 0e0d 0000 c0d9 0000 0000 0000  .!..............
 00011960: e421 0000 0e0d 0000 c8d9 0000 0000 0000  .!..............
 00011970: 1522 0000 0e0d 0000 d0d9 0000 0000 0000  ."..............
 00011980: 2922 0000 0e0d 0000 d8d9 0000 0000 0000  )"..............
 00011990: 3d22 0000 0e0d 0000 e0d9 0000 0000 0000  ="..............
 000119a0: 5122 0000 6400 0000 0000 0000 0000 0000  Q"..d...........
 000119b0: be22 0000 6400 0000 0000 0000 0000 0000  ."..d...........
-000119c0: cf22 0000 6603 0100 6d76 7364 0000 0000  ."..f...mvsd....
+000119c0: cf22 0000 6603 0100 a576 7364 0000 0000  ."..f....vsd....
 000119d0: 0100 0000 2e01 0000 2031 0000 0000 0000  ........ 1......
 000119e0: 6e23 0000 2401 0000 2031 0000 0000 0000  n#..$... 1......
 000119f0: 8523 0000 8400 0000 0000 0000 0000 0000  .#..............
 00011a00: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 00011a10: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 00011a20: 0100 0000 2e01 0000 4031 0000 0000 0000  ........@1......
 00011a30: b523 0000 2401 0000 4031 0000 0000 0000  .#..$...@1......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/logger/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/logger/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -267,15 +267,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/logger/__init__.o (1699)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473765C
+    Value: 0x64737695
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2154,15 +2154,15 @@
 00008690: c042 0000 0000 0000 be05 0000 0e0c 0000  .B..............
 000086a0: c842 0000 0000 0000 ef05 0000 0e0c 0000  .B..............
 000086b0: d042 0000 0000 0000 0306 0000 0e0c 0000  .B..............
 000086c0: d842 0000 0000 0000 1706 0000 0e0c 0000  .B..............
 000086d0: e042 0000 0000 0000 2b06 0000 6400 0000  .B......+...d...
 000086e0: 0000 0000 0000 0000 9806 0000 6400 0000  ............d...
 000086f0: 0000 0000 0000 0000 a306 0000 6603 0100  ............f...
-00008700: 5c76 7364 0000 0000 0100 0000 2e01 0000  \vsd............
+00008700: 9576 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 00008710: 902c 0000 0000 0000 3c07 0000 2401 0000  .,......<...$...
 00008720: 902c 0000 0000 0000 4b07 0000 8400 0000  .,......K.......
 00008730: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008740: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 00008750: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 00008760: b02c 0000 0000 0000 7507 0000 2401 0000  .,......u...$...
 00008770: b02c 0000 0000 0000 8907 0000 8400 0000  .,..............
```

### Comparing `faceid-lib-2.0.2/faceid_lib/logger/logger_helper.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/logger/logger_helper.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -888,15 +888,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/logger/logger_helper.o (4278)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x6473765D
+    Value: 0x64737696
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -3305,15 +3305,15 @@
 0000ce80: d08c 0000 0000 0000 cc0f 0000 0e0d 0000  ................
 0000ce90: d88c 0000 0000 0000 fd0f 0000 0e0d 0000  ................
 0000cea0: e08c 0000 0000 0000 1110 0000 0e0d 0000  ................
 0000ceb0: e88c 0000 0000 0000 2510 0000 0e0d 0000  ........%.......
 0000cec0: f08c 0000 0000 0000 3910 0000 6400 0000  ........9...d...
 0000ced0: 0000 0000 0000 0000 a610 0000 6400 0000  ............d...
 0000cee0: 0000 0000 0000 0000 b610 0000 6603 0100  ............f...
-0000cef0: 5d76 7364 0000 0000 0100 0000 2e01 0000  ]vsd............
+0000cef0: 9676 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 0000cf00: f041 0000 0000 0000 5411 0000 2401 0000  .A......T...$...
 0000cf10: f041 0000 0000 0000 6a11 0000 8400 0000  .A......j.......
 0000cf20: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 0000cf30: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 0000cf40: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 0000cf50: 1042 0000 0000 0000 9911 0000 2401 0000  .B..........$...
 0000cf60: 1042 0000 0000 0000 ad11 0000 8400 0000  .B..............
```

### Comparing `faceid-lib-2.0.2/faceid_lib/ratelimiter/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/ratelimiter/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -2922,15 +2922,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/ratelimiter/__init__.o (13603)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737662
+    Value: 0x6473769C
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -5685,15 +5685,15 @@
 00016340: 0d34 0000 0e0d 0000 b829 0100 0000 0000  .4.......)......
 00016350: 3934 0000 0e0d 0000 c029 0100 0000 0000  94.......)......
 00016360: 6a34 0000 0e0d 0000 c829 0100 0000 0000  j4.......)......
 00016370: 7e34 0000 0e0d 0000 d029 0100 0000 0000  ~4.......)......
 00016380: 9234 0000 0e0d 0000 d829 0100 0000 0000  .4.......)......
 00016390: a634 0000 6400 0000 0000 0000 0000 0000  .4..d...........
 000163a0: 1835 0000 6400 0000 0000 0000 0000 0000  .5..d...........
-000163b0: 2335 0000 6603 0100 6276 7364 0000 0000  #5..f...bvsd....
+000163b0: 2335 0000 6603 0100 9c76 7364 0000 0000  #5..f....vsd....
 000163c0: 0100 0000 2e01 0000 003e 0000 0000 0000  .........>......
 000163d0: c135 0000 2401 0000 003e 0000 0000 0000  .5..$....>......
 000163e0: d535 0000 8400 0000 0000 0000 0000 0000  .5..............
 000163f0: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 00016400: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 00016410: 0100 0000 2e01 0000 203e 0000 0000 0000  ........ >......
 00016420: 0436 0000 2401 0000 203e 0000 0000 0000  .6..$... >......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/ratelimiter/depends.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/ratelimiter/depends.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -2553,15 +2553,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/ratelimiter/depends.o (11420)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737660
+    Value: 0x64737698
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -5650,15 +5650,15 @@
 00016110: 2821 0100 0000 0000 b32b 0000 0e0d 0000  (!.......+......
 00016120: 3021 0100 0000 0000 e42b 0000 0e0d 0000  0!.......+......
 00016130: 3821 0100 0000 0000 f82b 0000 0e0d 0000  8!.......+......
 00016140: 4021 0100 0000 0000 0c2c 0000 0e0d 0000  @!.......,......
 00016150: 4821 0100 0000 0000 202c 0000 6400 0000  H!...... ,..d...
 00016160: 0000 0000 0000 0000 922c 0000 6400 0000  .........,..d...
 00016170: 0000 0000 0000 0000 9c2c 0000 6603 0100  .........,..f...
-00016180: 6076 7364 0000 0000 0100 0000 2e01 0000  `vsd............
+00016180: 9876 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 00016190: 1037 0000 0000 0000 392d 0000 2401 0000  .7......9-..$...
 000161a0: 1037 0000 0000 0000 492d 0000 8400 0000  .7......I-......
 000161b0: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 000161c0: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 000161d0: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 000161e0: 3037 0000 0000 0000 772d 0000 2401 0000  07......w-..$...
 000161f0: 3037 0000 0000 0000 8b2d 0000 8400 0000  07.......-......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/vector_similarity/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/vector_similarity/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -267,15 +267,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/vector_similarity/__init__.o (1751)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737663
+    Value: 0x6473769C
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2155,15 +2155,15 @@
 000086a0: bb05 0000 0e0c 0000 c042 0000 0000 0000  .........B......
 000086b0: e705 0000 0e0c 0000 c842 0000 0000 0000  .........B......
 000086c0: 1806 0000 0e0c 0000 d042 0000 0000 0000  .........B......
 000086d0: 2c06 0000 0e0c 0000 d842 0000 0000 0000  ,........B......
 000086e0: 4006 0000 0e0c 0000 e042 0000 0000 0000  @........B......
 000086f0: 5406 0000 6400 0000 0000 0000 0000 0000  T...d...........
 00008700: cc06 0000 6400 0000 0000 0000 0000 0000  ....d...........
-00008710: d706 0000 6603 0100 6376 7364 0000 0000  ....f...cvsd....
+00008710: d706 0000 6603 0100 9c76 7364 0000 0000  ....f....vsd....
 00008720: 0100 0000 2e01 0000 402c 0000 0000 0000  ........@,......
 00008730: 7b07 0000 2401 0000 402c 0000 0000 0000  {...$...@,......
 00008740: 9507 0000 8400 0000 0000 0000 0000 0000  ................
 00008750: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 00008760: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 00008770: 0100 0000 2e01 0000 602c 0000 0000 0000  ........`,......
 00008780: ca07 0000 2401 0000 602c 0000 0000 0000  ....$...`,......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -267,15 +267,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/vector_similarity/v1/__init__.o (1727)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737664
+    Value: 0x6473769D
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2154,15 +2154,15 @@
 00008690: a005 0000 0e0c 0000 c042 0000 0000 0000  .........B......
 000086a0: cc05 0000 0e0c 0000 c842 0000 0000 0000  .........B......
 000086b0: fd05 0000 0e0c 0000 d042 0000 0000 0000  .........B......
 000086c0: 1106 0000 0e0c 0000 d842 0000 0000 0000  .........B......
 000086d0: 2506 0000 0e0c 0000 e042 0000 0000 0000  %........B......
 000086e0: 3906 0000 6400 0000 0000 0000 0000 0000  9...d...........
 000086f0: b406 0000 6400 0000 0000 0000 0000 0000  ....d...........
-00008700: bf06 0000 6603 0100 6476 7364 0000 0000  ....f...dvsd....
+00008700: bf06 0000 6603 0100 9d76 7364 0000 0000  ....f....vsd....
 00008710: 0100 0000 2e01 0000 502c 0000 0000 0000  ........P,......
 00008720: 6607 0000 2401 0000 502c 0000 0000 0000  f...$...P,......
 00008730: 7107 0000 8400 0000 0000 0000 0000 0000  q...............
 00008740: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 00008750: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 00008760: 0100 0000 2e01 0000 702c 0000 0000 0000  ........p,......
 00008770: a907 0000 2401 0000 702c 0000 0000 0000  ....$...p,......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/power.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/vector_similarity/v1/power.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -1140,15 +1140,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/vector_similarity/v1/power.o (5307)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737665
+    Value: 0x6473769E
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -3332,15 +3332,15 @@
 0000d030: 9f13 0000 0e0d 0000 d08f 0000 0000 0000  ................
 0000d040: cb13 0000 0e0d 0000 d88f 0000 0000 0000  ................
 0000d050: fc13 0000 0e0d 0000 e08f 0000 0000 0000  ................
 0000d060: 1014 0000 0e0d 0000 e88f 0000 0000 0000  ................
 0000d070: 2414 0000 0e0d 0000 f08f 0000 0000 0000  $...............
 0000d080: 3814 0000 6400 0000 0000 0000 0000 0000  8...d...........
 0000d090: b314 0000 6400 0000 0000 0000 0000 0000  ....d...........
-0000d0a0: bb14 0000 6603 0100 6576 7364 0000 0000  ....f...evsd....
+0000d0a0: bb14 0000 6603 0100 9e76 7364 0000 0000  ....f....vsd....
 0000d0b0: 0100 0000 2e01 0000 d038 0000 0000 0000  .........8......
 0000d0c0: 5f15 0000 2401 0000 d038 0000 0000 0000  _...$....8......
 0000d0d0: 6d15 0000 8400 0000 0000 0000 0000 0000  m...............
 0000d0e0: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 0000d0f0: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 0000d100: 0100 0000 2e01 0000 f038 0000 0000 0000  .........8......
 0000d110: a215 0000 2401 0000 f038 0000 0000 0000  ....$....8......
```

### Comparing `faceid-lib-2.0.2/faceid_lib/workflow/__init__.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/workflow/__init__.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -267,15 +267,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/workflow/__init__.o (1709)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737668
+    Value: 0x647376A0
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2154,15 +2154,15 @@
 00008690: c042 0000 0000 0000 c605 0000 0e0c 0000  .B..............
 000086a0: c842 0000 0000 0000 f705 0000 0e0c 0000  .B..............
 000086b0: d042 0000 0000 0000 0b06 0000 0e0c 0000  .B..............
 000086c0: d842 0000 0000 0000 1f06 0000 0e0c 0000  .B..............
 000086d0: e042 0000 0000 0000 3306 0000 6400 0000  .B......3...d...
 000086e0: 0000 0000 0000 0000 a206 0000 6400 0000  ............d...
 000086f0: 0000 0000 0000 0000 ad06 0000 6603 0100  ............f...
-00008700: 6876 7364 0000 0000 0100 0000 2e01 0000  hvsd............
+00008700: a076 7364 0000 0000 0100 0000 2e01 0000  .vsd............
 00008710: 802c 0000 0000 0000 4807 0000 2401 0000  .,......H...$...
 00008720: 802c 0000 0000 0000 5907 0000 8400 0000  .,......Y.......
 00008730: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008740: 2000 0000 0000 0000 0100 0000 4e01 0000   ...........N...
 00008750: 2000 0000 0000 0000 0100 0000 2e01 0000   ...............
 00008760: a02c 0000 0000 0000 8507 0000 2401 0000  .,..........$...
 00008770: a02c 0000 0000 0000 9907 0000 8400 0000  .,..............
```

### Comparing `faceid-lib-2.0.2/faceid_lib/workflow/workflow_helper.cpython-38-darwin.so` & `faceid-lib-3.0.0/faceid_lib/workflow/workflow_helper.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -951,15 +951,15 @@
   Symbol {
     Name: /Volumes/HDD500-DANI/PICASO-FACEID/picaso-faceid-engine/v1/faceid-lib-cython/build/temp.macosx-10.9-x86_64-3.8/cython_build/faceid_lib/workflow/workflow_helper.o (4584)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64737667
+    Value: 0x6473769F
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -3333,15 +3333,15 @@
 0000d040: ce10 0000 0e0d 0000 108e 0000 0000 0000  ................
 0000d050: fa10 0000 0e0d 0000 188e 0000 0000 0000  ................
 0000d060: 2b11 0000 0e0d 0000 208e 0000 0000 0000  +....... .......
 0000d070: 3f11 0000 0e0d 0000 288e 0000 0000 0000  ?.......(.......
 0000d080: 5311 0000 0e0d 0000 308e 0000 0000 0000  S.......0.......
 0000d090: 6711 0000 6400 0000 0000 0000 0000 0000  g...d...........
 0000d0a0: d611 0000 6400 0000 0000 0000 0000 0000  ....d...........
-0000d0b0: e811 0000 6603 0100 6776 7364 0000 0000  ....f...gvsd....
+0000d0b0: e811 0000 6603 0100 9f76 7364 0000 0000  ....f....vsd....
 0000d0c0: 0100 0000 2e01 0000 103f 0000 0000 0000  .........?......
 0000d0d0: 8a12 0000 2401 0000 103f 0000 0000 0000  ....$....?......
 0000d0e0: a212 0000 8400 0000 0000 0000 0000 0000  ................
 0000d0f0: 0100 0000 2400 0000 2000 0000 0000 0000  ....$... .......
 0000d100: 0100 0000 4e01 0000 2000 0000 0000 0000  ....N... .......
 0000d110: 0100 0000 2e01 0000 303f 0000 0000 0000  ........0?......
 0000d120: d512 0000 2401 0000 303f 0000 0000 0000  ....$...0?......
```

### Comparing `faceid-lib-2.0.2/pyproject.toml` & `faceid-lib-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "faceid-lib"
-version = "2.0.2"
+version = "3.0.0"
 description = "Simple and flexible AI/ML workflow engine by Picaso - FaceID"
 authors = ["Dani Gunawan <danigunawan.elektroug@gmail.com>"]
 
 license = "Apache License"
 readme = "README.md"
-homepage = "#"
-repository = "#"
+homepage = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
+repository = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
 keywords = ["machine learning", "Deep Learning", "Message Broker", "Distributed System", "pipeline", "rabbitmq", "ratelimiter"]
 classifiers = [
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.7",
 ]
@@ -58,8 +58,8 @@
 requires = ["poetry-core>=1.0.0", "setuptools~=50.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 # The allows us to build C extensions (using Cython). Unstable feature
 # https://github.com/python-poetry/poetry/issues/2740#issuecomment-666551481
 script = "build.py"
-generate-setup-file = false
+generate-setup-file = false
```

### Comparing `faceid-lib-2.0.2/PKG-INFO` & `faceid-lib-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: faceid-lib
-Version: 2.0.2
+Version: 3.0.0
 Summary: Simple and flexible AI/ML workflow engine by Picaso - FaceID
-Home-page: #
+Home-page: https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib
 License: Apache License
 Keywords: machine learning,Deep Learning,Message Broker,Distributed System,pipeline,rabbitmq,ratelimiter
 Author: Dani Gunawan
 Author-email: danigunawan.elektroug@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: aioredis (==1.3.1)
 Requires-Dist: appengine-python-standard (>=1.1.1,<2.0.0)
 Requires-Dist: fastapi
 Requires-Dist: pika (>=1.2.0,<2.0.0)
 Requires-Dist: requests
-Project-URL: Repository, #
+Project-URL: Repository, https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib
 Description-Content-Type: text/markdown
 
 # picaso-engine ML faceid workflow
 
 ## Overview
 
 This is a helper library for picaso-engine ML faceid workflow product. The idea of this library is to wrap all reusable code to simplify and improve workflow implementation.
```

