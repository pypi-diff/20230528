# Comparing `tmp/bibigo-0.0.7.tar.gz` & `tmp/bibigo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.7.tar", last modified: Sun May 28 10:17:14 2023, max compression
+gzip compressed data, was "bibigo-0.0.8.tar", last modified: Sun May 28 11:30:01 2023, max compression
```

## Comparing `bibigo-0.0.7.tar` & `bibigo-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.249784 bibigo-0.0.7/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.7/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 10:17:14.249784 bibigo-0.0.7/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.7/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.7/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 10:17:14.249784 bibigo-0.0.7/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.7/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.7/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.7/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.7/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.7/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.7/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2527 2023-05-28 10:15:03.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2023-05-28 10:16:04.000000 bibigo-0.0.7/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.7/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.7/src/bibigo/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/static/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.7/src/bibigo/static/.dockerignore.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.7/src/bibigo/static/.gitignore.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.249784 bibigo-0.0.7/src/bibigo/static/.vscode/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.7/src/bibigo/static/.vscode/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.7/src/bibigo/static/.vscode/settings.json.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.7/src/bibigo/static/Dockerfile.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.7/src/bibigo/static/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.7/src/bibigo/static/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.7/src/bibigo/static/setup.cfg.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.7/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1038 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.8/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 11:30:01.851439 bibigo-0.0.8/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.8/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.8/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 11:30:01.851439 bibigo-0.0.8/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.8/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.8/src/bibigo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1528 2023-05-28 11:11:35.000000 bibigo-0.0.8/src/bibigo/__pycache__/scripts.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.8/src/bibigo/__pycache__/test.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.8/src/bibigo/__pycache__/utils.cpython-39.pyc
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.8/src/bibigo/init/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/init/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2527 2023-05-28 10:15:03.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/package.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.8/src/bibigo/init/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2616 2023-05-28 11:26:47.000000 bibigo-0.0.8/src/bibigo/init/docker_compose.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3476 2023-05-28 11:16:01.000000 bibigo-0.0.8/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.8/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1116 2023-05-28 11:11:31.000000 bibigo-0.0.8/src/bibigo/scripts.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/static/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.8/src/bibigo/static/.dockerignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.8/src/bibigo/static/.gitignore.default
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.851439 bibigo-0.0.8/src/bibigo/static/.vscode/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.8/src/bibigo/static/.vscode/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.8/src/bibigo/static/.vscode/settings.json.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.8/src/bibigo/static/Dockerfile.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.8/src/bibigo/static/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1318 2023-05-28 11:29:11.000000 bibigo-0.0.8/src/bibigo/static/docker-compose.yml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.8/src/bibigo/static/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.8/src/bibigo/static/setup.cfg.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.8/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 11:30:01.847439 bibigo-0.0.8/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1117 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 11:30:01.000000 bibigo-0.0.8/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.7/LICENSE` & `bibigo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/README.md` & `bibigo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/setup.cfg` & `bibigo-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/__pycache__/scripts.cpython-39.pyc` & `bibigo-0.0.8/src/bibigo/__pycache__/scripts.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 06:53:09 2023 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,96 @@
-00000000: 610d 0d0a 0000 0000 55fa 7264 cb03 0000  a.......U.rd....
+00000000: 610d 0d0a 0000 0000 e336 7364 5c04 0000  a........6sd\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6503 a004 a100 6403 6404  d.l.Z.e.....d.d.
 00000050: 8400 8301 5a05 6505 a004 a100 6405 6406  ....Z.e.....d.d.
 00000060: 8400 8301 5a06 6506 a007 a100 6503 a008  ....Z.e.....e...
 00000070: 6407 a101 6408 6409 8400 8301 8301 5a09  d...d.d.......Z.
 00000080: 6506 a007 a100 6503 a008 6407 a101 640a  e.....e...d...d.
-00000090: 640b 8400 8301 8301 5a0a 6505 a004 a100  d.......Z.e.....
-000000a0: 640c 640d 8400 8301 5a0b 650b a007 a100  d.d.....Z.e.....
-000000b0: 6503 a008 640e a101 6503 6a0c 640f 6410  e...d...e.j.d.d.
-000000c0: 6411 8d02 6412 6413 8400 8301 8301 8301  d...d.d.........
-000000d0: 5a0d 6402 5300 2914 e900 0000 0029 02da  Z.d.S.)......)..
-000000e0: 0e70 7269 6e74 5f66 756e 6374 696f 6eda  .print_function.
-000000f0: 1075 6e69 636f 6465 5f6c 6974 6572 616c  .unicode_literal
-00000100: 734e 6300 0000 0000 0000 0000 0000 0000  sNc.............
-00000110: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000120: 6400 5300 a901 4ea9 0072 0500 0000 7205  d.S...N..r....r.
-00000130: 0000 0072 0500 0000 fa32 2f68 6f6d 652f  ...r.....2/home/
-00000140: 6575 6765 6e65 2f70 726f 6a65 6374 732f  eugene/projects/
-00000150: 6269 6269 676f 2f73 7263 2f62 6962 6967  bibigo/src/bibig
-00000160: 6f2f 7363 7269 7074 732e 7079 da06 6269  o/scripts.py..bi
-00000170: 6269 676f 0900 0000 7302 0000 0000 0272  bigo....s......r
-00000180: 0700 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000190: 0000 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-000001a0: 0000 6400 5300 7204 0000 0072 0500 0000  ..d.S.r....r....
-000001b0: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-000001c0: 0600 0000 da04 696e 6974 1100 0000 7302  ......init....s.
-000001d0: 0000 0000 0272 0800 0000 da04 726f 6f74  .....r......root
-000001e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000001f0: 0004 0000 0043 0000 0073 1c00 0000 6401  .....C...s....d.
-00000200: 6402 6c00 6d01 7d01 0100 7c01 7c00 6403  d.l.m.}...|.|.d.
-00000210: 6404 8d02 0100 6400 5300 2905 4ee9 0100  d.....d.S.).N...
-00000220: 0000 a901 da0d 696e 6974 5f73 6574 7469  ......init_setti
-00000230: 6e67 7354 2901 da07 7665 7262 6f73 6529  ngsT)...verbose)
-00000240: 02da 0d69 6e69 742e 7365 7474 696e 6773  ...init.settings
-00000250: 720c 0000 0029 0272 0900 0000 720c 0000  r....).r....r...
-00000260: 0072 0500 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000270: da08 7365 7474 696e 6773 1600 0000 7304  ..settings....s.
-00000280: 0000 0000 030c 0272 0f00 0000 6301 0000  .......r....c...
-00000290: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000002a0: 0043 0000 0073 2c00 0000 6401 6402 6c00  .C...s,...d.d.l.
-000002b0: 6d01 7d01 0100 6401 6403 6c02 6d03 7d02  m.}...d.d.l.m.}.
-000002c0: 0100 7c02 7c00 8301 0100 7c01 7c00 8301  ..|.|.....|.|...
-000002d0: 0100 6400 5300 2904 4e72 0a00 0000 2901  ..d.S.).Nr....).
-000002e0: da0c 696e 6974 5f70 6163 6b61 6765 720b  ..init_packager.
-000002f0: 0000 0029 045a 0c69 6e69 742e 7061 636b  ...).Z.init.pack
-00000300: 6167 6572 1000 0000 720e 0000 0072 0c00  ager....r....r..
-00000310: 0000 2903 7209 0000 0072 1000 0000 720c  ..).r....r....r.
-00000320: 0000 0072 0500 0000 7205 0000 0072 0600  ...r....r....r..
-00000330: 0000 da07 7061 636b 6167 651e 0000 0073  ....package....s
-00000340: 0800 0000 0003 0c01 0c02 0801 7211 0000  ............r...
-00000350: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000360: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-00000370: 0053 0072 0400 0000 7205 0000 0072 0500  .S.r....r....r..
-00000380: 0000 7205 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00000390: 00da 0564 6562 7567 2b00 0000 7302 0000  ...debug+...s...
-000003a0: 0000 0272 1200 0000 da08 6669 6c65 6e61  ...r......filena
-000003b0: 6d65 7a09 2d2d 7665 7273 696f 6eda 0764  mez.--version..d
-000003c0: 6566 6175 6c74 2901 7214 0000 0063 0200  efault).r....c..
-000003d0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-000003e0: 0000 4300 0000 7324 0000 0064 0164 026c  ..C...s$...d.d.l
-000003f0: 006d 017d 0201 007c 027c 007c 0164 038d  .m.}...|.|.|.d..
-00000400: 027d 0374 027c 0383 0101 0064 0053 0029  .}.t.|.....d.S.)
-00000410: 044e 720a 0000 0029 01da 0472 6561 6429  .Nr....)...read)
-00000420: 02da 0266 6eda 0776 6572 7369 6f6e 2903  ...fn..version).
-00000430: 5a05 7574 696c 7372 1500 0000 da05 7072  Z.utilsr......pr
-00000440: 696e 7429 0472 1300 0000 7217 0000 0072  int).r....r....r
-00000450: 1500 0000 5a07 636f 6e74 656e 7472 0500  ....Z.contentr..
-00000460: 0000 7205 0000 0072 0600 0000 da04 6669  ..r....r......fi
-00000470: 6c65 3000 0000 7306 0000 0000 040c 020c  le0...s.........
-00000480: 0172 1900 0000 290e 5a0a 5f5f 6675 7475  .r....).Z.__futu
-00000490: 7265 5f5f 7202 0000 0072 0300 0000 5a05  re__r....r....Z.
-000004a0: 636c 6963 6bda 0567 726f 7570 7207 0000  click..groupr...
-000004b0: 0072 0800 0000 5a07 636f 6d6d 616e 645a  .r....Z.commandZ
-000004c0: 0861 7267 756d 656e 7472 0f00 0000 7211  .argumentr....r.
-000004d0: 0000 0072 1200 0000 5a06 6f70 7469 6f6e  ...r....Z.option
-000004e0: 7219 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-000004f0: 0500 0000 7206 0000 00da 083c 6d6f 6475  ....r......<modu
-00000500: 6c65 3e01 0000 0073 2200 0000 1002 0806  le>....s".......
-00000510: 0601 0a07 0601 0a04 0601 0801 0c06 0601  ................
-00000520: 0801 0c0b 0601 0a04 0601 0801 0c01       ..............
+00000090: 640b 8400 8301 8301 5a0a 6506 a007 a100  d.......Z.e.....
+000000a0: 6503 a008 6407 a101 640c 640d 8400 8301  e...d...d.d.....
+000000b0: 8301 5a0b 6505 a004 a100 640e 640f 8400  ..Z.e.....d.d...
+000000c0: 8301 5a0c 650c a007 a100 6503 a008 6410  ..Z.e.....e...d.
+000000d0: a101 6503 6a0d 6411 6412 6413 8d02 6414  ..e.j.d.d.d...d.
+000000e0: 6415 8400 8301 8301 8301 5a0e 6402 5300  d.........Z.d.S.
+000000f0: 2916 e900 0000 0029 02da 0e70 7269 6e74  )......)...print
+00000100: 5f66 756e 6374 696f 6eda 1075 6e69 636f  _function..unico
+00000110: 6465 5f6c 6974 6572 616c 734e 6300 0000  de_literalsNc...
+00000120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000130: 0043 0000 0073 0400 0000 6400 5300 a901  .C...s....d.S...
+00000140: 4ea9 0072 0500 0000 7205 0000 0072 0500  N..r....r....r..
+00000150: 0000 fa32 2f68 6f6d 652f 6575 6765 6e65  ...2/home/eugene
+00000160: 2f70 726f 6a65 6374 732f 6269 6269 676f  /projects/bibigo
+00000170: 2f73 7263 2f62 6962 6967 6f2f 7363 7269  /src/bibigo/scri
+00000180: 7074 732e 7079 da06 6269 6269 676f 0900  pts.py..bibigo..
+00000190: 0000 7302 0000 0000 0272 0700 0000 6300  ..s......r....c.
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000001b0: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
+000001c0: 7204 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
+000001d0: 0500 0000 7205 0000 0072 0600 0000 da04  ....r....r......
+000001e0: 696e 6974 1100 0000 7302 0000 0000 0272  init....s......r
+000001f0: 0800 0000 da04 726f 6f74 6301 0000 0000  ......rootc.....
+00000200: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000210: 0000 0073 1c00 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
+00000220: 7d01 0100 7c01 7c00 6403 6404 8d02 0100  }...|.|.d.d.....
+00000230: 6400 5300 2905 4ee9 0100 0000 a901 da0d  d.S.).N.........
+00000240: 696e 6974 5f73 6574 7469 6e67 7354 2901  init_settingsT).
+00000250: da07 7665 7262 6f73 6529 02da 0d69 6e69  ..verbose)...ini
+00000260: 742e 7365 7474 696e 6773 720c 0000 0029  t.settingsr....)
+00000270: 0272 0900 0000 720c 0000 0072 0500 0000  .r....r....r....
+00000280: 7205 0000 0072 0600 0000 da08 7365 7474  r....r......sett
+00000290: 696e 6773 1600 0000 7304 0000 0000 030c  ings....s.......
+000002a0: 0272 0f00 0000 6301 0000 0000 0000 0000  .r....c.........
+000002b0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
+000002c0: 2c00 0000 6401 6402 6c00 6d01 7d01 0100  ,...d.d.l.m.}...
+000002d0: 6401 6403 6c02 6d03 7d02 0100 7c02 7c00  d.d.l.m.}...|.|.
+000002e0: 8301 0100 7c01 7c00 8301 0100 6400 5300  ....|.|.....d.S.
+000002f0: 2904 4e72 0a00 0000 2901 da0c 696e 6974  ).Nr....)...init
+00000300: 5f70 6163 6b61 6765 720b 0000 0029 045a  _packager....).Z
+00000310: 0c69 6e69 742e 7061 636b 6167 6572 1000  .init.packager..
+00000320: 0000 720e 0000 0072 0c00 0000 2903 7209  ..r....r....).r.
+00000330: 0000 0072 1000 0000 720c 0000 0072 0500  ...r....r....r..
+00000340: 0000 7205 0000 0072 0600 0000 da07 7061  ..r....r......pa
+00000350: 636b 6167 651e 0000 0073 0800 0000 0003  ckage....s......
+00000360: 0c01 0c02 0801 7211 0000 0063 0100 0000  ......r....c....
+00000370: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000380: 4300 0000 7318 0000 0064 0164 026c 006d  C...s....d.d.l.m
+00000390: 017d 0101 007c 017c 0083 0101 0064 0053  .}...|.|.....d.S
+000003a0: 0029 034e 720a 0000 0029 01da 0a69 6e69  .).Nr....)...ini
+000003b0: 745f 7374 6163 6b29 025a 1369 6e69 742e  t_stack).Z.init.
+000003c0: 646f 636b 6572 5f63 6f6d 706f 7365 7212  docker_composer.
+000003d0: 0000 0029 0272 0900 0000 7212 0000 0072  ...).r....r....r
+000003e0: 0500 0000 7205 0000 0072 0600 0000 da0e  ....r....r......
+000003f0: 646f 636b 6572 5f63 6f6d 706f 7365 2700  docker_compose'.
+00000400: 0000 7304 0000 0000 030c 0272 1300 0000  ..s........r....
+00000410: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000420: 0001 0000 0043 0000 0073 0400 0000 6400  .....C...s....d.
+00000430: 5300 7204 0000 0072 0500 0000 7205 0000  S.r....r....r...
+00000440: 0072 0500 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000450: da05 6465 6275 6732 0000 0073 0200 0000  ..debug2...s....
+00000460: 0002 7214 0000 00da 0866 696c 656e 616d  ..r......filenam
+00000470: 657a 092d 2d76 6572 7369 6f6e da07 6465  ez.--version..de
+00000480: 6661 756c 7429 0172 1600 0000 6302 0000  fault).r....c...
+00000490: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+000004a0: 0043 0000 0073 2400 0000 6401 6402 6c00  .C...s$...d.d.l.
+000004b0: 6d01 7d02 0100 7c02 7c00 7c01 6403 8d02  m.}...|.|.|.d...
+000004c0: 7d03 7402 7c03 8301 0100 6400 5300 2904  }.t.|.....d.S.).
+000004d0: 4e72 0a00 0000 2901 da04 7265 6164 2902  Nr....)...read).
+000004e0: da02 666e da07 7665 7273 696f 6e29 035a  ..fn..version).Z
+000004f0: 0575 7469 6c73 7217 0000 00da 0570 7269  .utilsr......pri
+00000500: 6e74 2904 7215 0000 0072 1900 0000 7217  nt).r....r....r.
+00000510: 0000 005a 0763 6f6e 7465 6e74 7205 0000  ...Z.contentr...
+00000520: 0072 0500 0000 7206 0000 00da 0466 696c  .r....r......fil
+00000530: 6537 0000 0073 0600 0000 0004 0c02 0c01  e7...s..........
+00000540: 721b 0000 0029 0f5a 0a5f 5f66 7574 7572  r....).Z.__futur
+00000550: 655f 5f72 0200 0000 7203 0000 005a 0563  e__r....r....Z.c
+00000560: 6c69 636b da05 6772 6f75 7072 0700 0000  lick..groupr....
+00000570: 7208 0000 005a 0763 6f6d 6d61 6e64 5a08  r....Z.commandZ.
+00000580: 6172 6775 6d65 6e74 720f 0000 0072 1100  argumentr....r..
+00000590: 0000 7213 0000 0072 1400 0000 5a06 6f70  ..r....r....Z.op
+000005a0: 7469 6f6e 721b 0000 0072 0500 0000 7205  tionr....r....r.
+000005b0: 0000 0072 0500 0000 7206 0000 00da 083c  ...r....r......<
+000005c0: 6d6f 6475 6c65 3e01 0000 0073 2800 0000  module>....s(...
+000005d0: 1002 0806 0601 0a07 0601 0a04 0601 0801  ................
+000005e0: 0c06 0601 0801 0c07 0601 0801 0c09 0601  ................
+000005f0: 0a04 0601 0801 0c01                      ........
```

### Comparing `bibigo-0.0.7/src/bibigo/__pycache__/utils.cpython-39.pyc` & `bibigo-0.0.8/src/bibigo/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/init/__pycache__/package.cpython-39.pyc` & `bibigo-0.0.8/src/bibigo/init/__pycache__/package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/init/__pycache__/settings.cpython-39.pyc` & `bibigo-0.0.8/src/bibigo/init/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/init/package.py` & `bibigo-0.0.8/src/bibigo/init/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         },
         {
             "type": "input",
             "name": "dependency_links",
             "default": private_pypi,
             "message": "Your Private PyPI",
         },
-        {"type": "confirm", "name": "confirm", "message": "Confirm Initializer"},
+        {"type": "confirm", "name": "confirm", "message": "Confirm"},
     ]
 
     # user input
     conf = prompt(setup_conf)
     confirm = conf.pop("confirm")
     if not confirm:
         print("[EXIT] Nothing Happened!")
```

### Comparing `bibigo-0.0.7/src/bibigo/init/settings.py` & `bibigo-0.0.8/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/scripts.py` & `bibigo-0.0.8/src/bibigo/scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 @click.argument("root")
 def package(root):
     from .init.package import init_package
     from .init.settings import init_settings
 
     init_settings(root)
     init_package(root)
+    
+@init.command()
+@click.argument("root")
+def docker_compose(root):
+    from .init.docker_compose import init_stack
+    
+    init_stack(root)
 
 
 ################
 # debug
 ################
 @bibigo.group()
 def debug():
```

### Comparing `bibigo-0.0.7/src/bibigo/static/.dockerignore.default` & `bibigo-0.0.8/src/bibigo/static/.dockerignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/static/.gitignore.default` & `bibigo-0.0.8/src/bibigo/static/.gitignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/static/setup.cfg.default` & `bibigo-0.0.8/src/bibigo/static/setup.cfg.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo/utils.py` & `bibigo-0.0.8/src/bibigo/utils.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.7/src/bibigo.egg-info/SOURCES.txt` & `bibigo-0.0.8/src/bibigo.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 src/bibigo.egg-info/requires.txt
 src/bibigo.egg-info/top_level.txt
 src/bibigo/__pycache__/__init__.cpython-39.pyc
 src/bibigo/__pycache__/scripts.cpython-39.pyc
 src/bibigo/__pycache__/test.cpython-39.pyc
 src/bibigo/__pycache__/utils.cpython-39.pyc
 src/bibigo/init/__init__.py
+src/bibigo/init/docker_compose.py
 src/bibigo/init/package.py
 src/bibigo/init/settings.py
 src/bibigo/init/__pycache__/__init__.cpython-39.pyc
 src/bibigo/init/__pycache__/package.cpython-39.pyc
 src/bibigo/init/__pycache__/settings.cpython-39.pyc
 src/bibigo/static/.dockerignore.default
 src/bibigo/static/.gitignore.default
 src/bibigo/static/Dockerfile.default
 src/bibigo/static/__init__.py
+src/bibigo/static/docker-compose.yml.default
 src/bibigo/static/pyproject.toml.default
 src/bibigo/static/setup.cfg.default
 src/bibigo/static/.vscode/__init__.py
 src/bibigo/static/.vscode/settings.json.default
```

