# Comparing `tmp/animetime-0.1.6.tar.gz` & `tmp/animetime-0.2.tar.gz`

## Comparing `animetime-0.1.6.tar` & `animetime-0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 animetime-0.1.6/animetime.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 animetime-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animetime-0.1.6/LICENSE
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 animetime-0.1.6/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 animetime-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 animetime-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 animetime-0.2/animetime.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 animetime-0.2/at_test.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 animetime-0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animetime-0.2/LICENSE
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 animetime-0.2/README.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 animetime-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 animetime-0.2/PKG-INFO
```

### Comparing `animetime-0.1.6/LICENSE` & `animetime-0.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 cassphir
+Copyright (c) 2022 swarthur
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `animetime-0.1.6/pyproject.toml` & `animetime-0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 00000050: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
 00000060: 5d0d 0a65 7863 6c75 6465 203d 205b 0d0a  ]..exclude = [..
 00000070: 2020 222f 6469 7374 222c 0d0a 2020 222f    "/dist",..  "/
 00000080: 2e67 6974 222c 0d0a 2020 222e 6769 7469  .git",..  ".giti
 00000090: 676e 6f72 6522 0d0a 2020 5d0d 0a0d 0a5b  gnore"..  ]....[
 000000a0: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 000000b0: 2022 616e 696d 6574 696d 6522 0d0a 7665   "animetime"..ve
-000000c0: 7273 696f 6e20 3d20 2230 2e31 2e36 220d  rsion = "0.1.6".
-000000d0: 0a61 7574 686f 7273 203d 205b 0d0a 207b  .authors = [.. {
-000000e0: 6e61 6d65 3d22 6361 7373 7068 6972 222c  name="cassphir",
-000000f0: 2065 6d61 696c 3d22 227d 0d0a 5d0d 0a64   email=""}..]..d
-00000100: 6573 6372 6970 7469 6f6e 203d 2022 556e  escription = "Un
-00000110: 206d 6f64 756c 6520 706f 7572 2067 c3a9   module pour g..
-00000120: 7265 7220 7365 7320 616e 696d c3a9 7320  rer ses anim..s 
-00000130: 6661 6369 6c65 6d65 6e74 220d 0a72 6561  facilement"..rea
-00000140: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
-00000150: 220d 0a72 6571 7569 7265 732d 7079 7468  "..requires-pyth
-00000160: 6f6e 203d 2022 3e3d 332e 3722 0d0a 6c69  on = ">=3.7"..li
-00000170: 6365 6e73 6520 3d20 224d 4954 220d 0a63  cense = "MIT"..c
-00000180: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
-00000190: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
-000001a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001b0: 686f 6e20 3a3a 2033 222c 0d0a 2020 2020  hon :: 3",..    
-000001c0: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
-000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001e0: 4c69 6365 6e73 6522 2c0d 0a20 2020 2022  License",..    "
-000001f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000200: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000210: 6e74 222c 0d0a 5d0d 0a64 6570 656e 6465  nt",..]..depende
-00000220: 6e63 6965 7320 3d20 5b22 616e 696d 6564  ncies = ["animed
-00000230: 6174 6122 2c22 746f 6d6c 6922 5d0d 0a0d  ata","tomli"]...
-00000240: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000250: 0a22 4769 7468 7562 2220 3d20 2268 7474  ."Github" = "htt
-00000260: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000270: 6361 7373 7068 6972 2f61 6e69 6d65 7469  cassphir/animeti
-00000280: 6d65 220d 0a22 4275 6722 203d 2022 6874  me".."Bug" = "ht
-00000290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002a0: 2f63 6173 7370 6869 722f 616e 696d 6574  /cassphir/animet
-000002b0: 696d 652f 6973 7375 6573 220d 0a         ime/issues"..
+000000c0: 7273 696f 6e20 3d20 2230 2e32 220d 0a61  rsion = "0.2"..a
+000000d0: 7574 686f 7273 203d 205b 0d0a 207b 6e61  uthors = [.. {na
+000000e0: 6d65 3d22 7377 6172 7468 7572 227d 0d0a  me="swarthur"}..
+000000f0: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
+00000100: 2022 4120 6d6f 6475 6c65 2074 6f20 6d61   "A module to ma
+00000110: 6e61 6765 2061 6e64 2074 7261 636b 2079  nage and track y
+00000120: 6f75 7220 6661 766f 7572 6974 6573 2061  our favourites a
+00000130: 6e69 6d65 7320 616e 6420 7365 7269 6573  nimes and series
+00000140: 220d 0a72 6561 646d 6520 3d20 2252 4541  "..readme = "REA
+00000150: 444d 452e 6d64 220d 0a72 6571 7569 7265  DME.md"..require
+00000160: 732d 7079 7468 6f6e 203d 2022 3e3d 332e  s-python = ">=3.
+00000170: 3131 220d 0a6c 6963 656e 7365 203d 2022  11"..license = "
+00000180: 4d49 5422 0d0a 636c 6173 7369 6669 6572  MIT"..classifier
+00000190: 7320 3d20 5b0d 0a20 2020 2022 5072 6f67  s = [..    "Prog
+000001a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+000001c0: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
+000001d0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001e0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
+000001f0: 0d0a 2020 2020 224f 7065 7261 7469 6e67  ..    "Operating
+00000200: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000210: 6465 7065 6e64 656e 7422 2c0d 0a5d 0d0a  dependent",..]..
+00000220: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
+00000230: 2261 6e69 6d65 6461 7461 225d 0d0a 0d0a  "animedata"]....
+00000240: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
+00000250: 2247 6974 6875 6222 203d 2022 6874 7470  "Github" = "http
+00000260: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000270: 7761 7274 6875 722f 616e 696d 6574 696d  warthur/animetim
+00000280: 6522 0d0a 2242 7567 2220 3d20 2268 7474  e".."Bug" = "htt
+00000290: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000002a0: 7377 6172 7468 7572 2f61 6e69 6d65 7469  swarthur/animeti
+000002b0: 6d65 2f69 7373 7565 7322 0d0a            me/issues"..
```

