# Comparing `tmp/bibigo-0.0.6.tar.gz` & `tmp/bibigo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.6.tar", last modified: Sun May 28 08:33:43 2023, max compression
+gzip compressed data, was "bibigo-0.0.7.tar", last modified: Sun May 28 10:17:14 2023, max compression
```

## Comparing `bibigo-0.0.6.tar` & `bibigo-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.6/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:33:43.205176 bibigo-0.0.6/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.6/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.6/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 08:33:43.205176 bibigo-0.0.6/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.6/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.6/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.6/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.6/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 08:23:08.000000 bibigo-0.0.6/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.6/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2023-05-28 08:32:34.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3342 2023-05-28 08:32:20.000000 bibigo-0.0.6/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.6/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.6/src/bibigo/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/static/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.6/src/bibigo/static/.dockerignore.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.6/src/bibigo/static/.gitignore.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/static/.vscode/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.6/src/bibigo/static/.vscode/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.6/src/bibigo/static/.vscode/settings.json.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.6/src/bibigo/static/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.6/src/bibigo/static/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.6/src/bibigo/static/setup.cfg.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      735 2023-05-28 08:17:40.000000 bibigo-0.0.6/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1001 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.249784 bibigo-0.0.7/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.7/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 10:17:14.249784 bibigo-0.0.7/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.7/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.7/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 10:17:14.249784 bibigo-0.0.7/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.7/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.7/src/bibigo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.7/src/bibigo/__pycache__/scripts.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.7/src/bibigo/__pycache__/test.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 10:15:03.000000 bibigo-0.0.7/src/bibigo/__pycache__/utils.cpython-39.pyc
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.7/src/bibigo/init/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/init/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2527 2023-05-28 10:15:03.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/package.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.7/src/bibigo/init/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3488 2023-05-28 10:16:04.000000 bibigo-0.0.7/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.7/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.7/src/bibigo/scripts.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo/static/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.7/src/bibigo/static/.dockerignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.7/src/bibigo/static/.gitignore.default
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.249784 bibigo-0.0.7/src/bibigo/static/.vscode/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.7/src/bibigo/static/.vscode/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.7/src/bibigo/static/.vscode/settings.json.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      244 2023-05-28 10:12:41.000000 bibigo-0.0.7/src/bibigo/static/Dockerfile.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.7/src/bibigo/static/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.7/src/bibigo/static/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.7/src/bibigo/static/setup.cfg.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      736 2023-05-28 10:14:42.000000 bibigo-0.0.7/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 10:17:14.245784 bibigo-0.0.7/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1038 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 10:17:14.000000 bibigo-0.0.7/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.6/LICENSE` & `bibigo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/README.md` & `bibigo-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/setup.cfg` & `bibigo-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/__pycache__/scripts.cpython-39.pyc` & `bibigo-0.0.7/src/bibigo/__pycache__/scripts.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/__pycache__/utils.cpython-39.pyc` & `bibigo-0.0.7/src/bibigo/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 08:17:40 2023 UTC, .py size: 735 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 240e 7364 df02 0000  a.......$.sd....
+00000000: 610d 0d0a 0000 0000 9229 7364 e002 0000  a........)sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c05 5a05 6404 5a06 6502 6507 6504  d.l.Z.d.Z.e.e.e.
 00000060: 6602 1900 6405 9c01 6406 6407 8404 5a08  f...d...d.d...Z.
 00000070: 6410 6504 6507 6409 9c02 640a 640b 8405  d.e.e.d...d.d...
@@ -13,30 +13,30 @@
 000000c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
 000000d0: 0000 4300 0000 7308 0000 0074 007c 0083  ..C...s....t.|..
 000000e0: 0153 0029 014e 7203 0000 0072 0500 0000  .S.).Nr....r....
 000000f0: a900 7207 0000 00fa 302f 686f 6d65 2f65  ..r.....0/home/e
 00000100: 7567 656e 652f 7072 6f6a 6563 7473 2f62  ugene/projects/b
 00000110: 6962 6967 6f2f 7372 632f 6269 6269 676f  ibigo/src/bibigo
 00000120: 2f75 7469 6c73 2e70 79da 0b65 6e73 7572  /utils.py..ensur
-00000130: 655f 7061 7468 0900 0000 7302 0000 0000  e_path....s.....
+00000130: 655f 7061 7468 0a00 0000 7302 0000 0000  e_path....s.....
 00000140: 0172 0900 0000 da07 6465 6661 756c 7429  .r......default)
 00000150: 02da 0266 6eda 0776 6572 7369 6f6e 6302  ...fn..versionc.
 00000160: 0000 0000 0000 0000 0000 0004 0000 0005  ................
 00000170: 0000 0043 0000 0073 2e00 0000 7400 7401  ...C...s....t.t.
 00000180: 8301 7c00 9b00 6401 7c01 9b00 9d03 1b00  ..|...d.|.......
 00000190: 7d02 7402 a003 7404 7c02 a005 a100 a102  }.t...t.|.......
 000001a0: a006 a100 7d03 7c03 5300 2902 4eda 012e  ....}.|.S.).N...
 000001b0: 2907 7204 0000 00da 0a53 5441 5449 435f  ).r......STATIC_
 000001c0: 4449 52da 0770 6b67 7574 696c da08 6765  DIR..pkgutil..ge
 000001d0: 745f 6461 7461 da08 5f5f 6e61 6d65 5f5f  t_data..__name__
 000001e0: da08 6173 5f70 6f73 6978 da06 6465 636f  ..as_posix..deco
 000001f0: 6465 2904 720b 0000 0072 0c00 0000 7206  de).r....r....r.
 00000200: 0000 00da 0763 6f6e 7465 6e74 7207 0000  .....contentr...
 00000210: 0072 0700 0000 7208 0000 00da 0472 6561  .r....r......rea
-00000220: 640e 0000 0073 0600 0000 0001 1601 1401  d....s..........
+00000220: 640f 0000 0073 0600 0000 0001 1601 1401  d....s..........
 00000230: 7215 0000 00da 0177 2901 da06 6473 745f  r......w)...dst_
 00000240: 6670 6303 0000 0000 0000 0000 0000 0004  fpc.............
 00000250: 0000 0008 0000 0043 0000 0073 6c00 0000  .......C...sl...
 00000260: 7400 7c00 8301 7d00 7c00 6a01 6a02 6401  t.|...}.|.j.j.d.
 00000270: 6401 6402 8d02 0100 7403 7c00 7c02 8302  d.d.....t.|.|...
 00000280: 8f36 7d03 7c00 6a04 a005 a100 6403 7600  .6}.|.j.....d.v.
 00000290: 7240 7406 a007 7c01 7c03 a102 0100 6e0a  r@t...|.|.....n.
@@ -47,18 +47,18 @@
 000002e0: 7374 5f6f 6b29 01da 046a 736f 6e29 0972  st_ok)...json).r
 000002f0: 0900 0000 da06 7061 7265 6e74 da05 6d6b  ......parent..mk
 00000300: 6469 72da 046f 7065 6eda 0673 7566 6669  dir..open..suffi
 00000310: 78da 056c 6f77 6572 721a 0000 00da 0464  x..lowerr......d
 00000320: 756d 70da 0577 7269 7465 2904 7217 0000  ump..write).r...
 00000330: 0072 1400 0000 da04 6d6f 6465 da02 6677  .r......mode..fw
 00000340: 7207 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000350: 2100 0000 1500 0000 730c 0000 0000 0108  !.......s.......
+00000350: 2100 0000 1600 0000 730c 0000 0000 0108  !.......s.......
 00000360: 0310 030c 010e 010e 0272 2100 0000 2901  .........r!...).
 00000370: 720a 0000 0029 0172 1600 0000 290b 721a  r....).r....).r.
 00000380: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
 00000390: da07 7061 7468 6c69 6272 0400 0000 720f  ..pathlibr....r.
 000003a0: 0000 0072 0e00 0000 da03 7374 7272 0900  ...r......strr..
 000003b0: 0000 7215 0000 0072 2100 0000 7207 0000  ..r....r!...r...
 000003c0: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
 000003d0: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
-000003e0: 0000 0008 010c 010c 0108 0204 0316 0512  ................
+000003e0: 0000 0008 010c 010c 0108 0204 0416 0512  ................
 000003f0: 07                                       .
```

### Comparing `bibigo-0.0.6/src/bibigo/init/__pycache__/package.cpython-39.pyc` & `bibigo-0.0.7/src/bibigo/init/__pycache__/package.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 08:32:20 2023 UTC, .py size: 3342 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 610d 0d0a 0000 0000 9411 7364 0e0d 0000  a.........sd....
+00000000: 610d 0d0a 0000 0000 9229 7364 a00d 0000  a........)sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6504  m.Z.m.Z.m.Z...e.
 00000070: 6407 6408 8d01 5a0b 6409 640a 8400 5a0c  d.d...Z.d.d...Z.
 00000080: 6401 5300 290b e900 0000 004e 2901 da04  d.S.)......N)...
 00000090: 5061 7468 2901 da07 436f 6e73 6f6c 6529  Path)...Console)
 000000a0: 01da 0550 616e 656c e902 0000 0029 03da  ...Panel.....)..
 000000b0: 0472 6561 64da 0577 7269 7465 da0a 5354  .read..write..ST
 000000c0: 4154 4943 5f44 4952 e958 0000 0029 01da  ATIC_DIR.X...)..
 000000d0: 0577 6964 7468 6301 0000 0000 0000 0000  .widthc.........
-000000e0: 0000 000d 0000 000e 0000 0043 0000 0073  ...........C...s
-000000f0: 1802 0000 6401 6402 6c00 6d01 7d01 0100  ....d.d.l.m.}...
+000000e0: 0000 000e 0000 000e 0000 0043 0000 0073  ...........C...s
+000000f0: 3002 0000 6401 6402 6c00 6d01 7d01 0100  0...d.d.l.m.}...
 00000100: 7402 7c00 8301 7d02 7c02 a003 a100 6a04  t.|...}.|.....j.
 00000110: 7d03 7405 a006 6403 a101 702a 6404 7d04  }.t...d...p*d.}.
 00000120: 6405 6406 7c03 6407 6408 9c04 6405 6409  d.d.|.d.d...d.d.
 00000130: 640a 640b 9c03 6405 640c 640d 640b 9c03  d.d...d.d.d.d...
 00000140: 6405 640e 640f 640b 9c03 6405 6410 6411  d.d.d.d...d.d.d.
 00000150: 6412 6408 9c04 6405 6413 6414 640b 9c03  d.d...d.d.d.d...
 00000160: 6405 6415 6416 6417 6408 9c04 6405 6418  d.d.d.d.d...d.d.
@@ -30,125 +30,129 @@
 000001d0: 7218 6404 7c06 641b 1900 7601 72fc 6404  r.d.|.d...v.r.d.
 000001e0: 6701 7c06 641b 1900 a201 7c06 641b 3c00  g.|.d.....|.d.<.
 000001f0: 6425 7d08 6426 7c08 9b00 9d02 a009 7c06  d%}.d&|.......|.
 00000200: 641b 1900 a101 7c06 641b 3c00 6427 7d09  d.....|.d.<.d'}.
 00000210: 740a 7c02 7c09 1b00 740b 7c09 8301 6428  t.|.|...t.|...d(
 00000220: 8d02 0100 6429 7d0a 740a 7c02 7c0a 1b00  ....d)}.t.|.|...
 00000230: 740b 7c0a 8301 6a0c 6600 6900 7c06 a401  t.|...j.f.i.|...
-00000240: 8e01 6428 8d02 0100 7c02 642a 1b00 6a0d  ..d(....|.d*..j.
-00000250: 642b 642c 8d01 0100 7c02 642a 1b00 7c06  d+d,....|.d*..|.
-00000260: 6406 1900 1b00 6a0d 642b 642c 8d01 0100  d.....j.d+d,....
-00000270: 7c02 642a 1b00 7c06 6406 1900 1b00 642d  |.d*..|.d.....d-
-00000280: 1b00 7d0b 7c0b a00e a100 9001 73a2 7c0b  ..}.|.......s.|.
-00000290: a00f a100 0100 7c02 642a 1b00 7c06 6406  ......|.d*..|.d.
-000002a0: 1900 1b00 7410 1b00 6a0d 642b 642c 8d01  ....t...j.d+d,..
-000002b0: 0100 7c02 642a 1b00 7c06 6406 1900 1b00  ..|.d*..|.d.....
-000002c0: 7410 1b00 642d 1b00 7d0b 7c0b a00e a100  t...d-..}.|.....
-000002d0: 9001 73e8 7c0b a00f a100 0100 6426 a009  ..s.|.......d&..
-000002e0: 642e 7c03 9b00 642f 9d03 6430 6431 6703  d.|...d/..d0d1g.
-000002f0: a101 7d0c 7408 8300 0100 7411 a008 7412  ..}.t.....t...t.
-00000300: 7c0c 8301 a101 0100 6400 5300 2932 4e72  |.......d.S.)2Nr
-00000310: 0100 0000 2901 da06 7072 6f6d 7074 5a0d  ....)...promptZ.
-00000320: 5049 505f 494e 4445 585f 5552 4cda 00da  PIP_INDEX_URL...
-00000330: 0569 6e70 7574 da07 7072 6f6a 6563 747a  .input..projectz
-00000340: 0c50 726f 6a65 6374 204e 616d 6529 04da  .Project Name)..
-00000350: 0474 7970 65da 046e 616d 65da 0764 6566  .type..name..def
-00000360: 6175 6c74 da07 6d65 7373 6167 655a 0661  ault..messageZ.a
-00000370: 7574 686f 725a 0641 7574 686f 7229 0372  uthorZ.Author).r
-00000380: 0f00 0000 7210 0000 0072 1200 0000 5a0c  ....r....r....Z.
-00000390: 6175 7468 6f72 5f65 6d61 696c 7a0c 4175  author_emailz.Au
-000003a0: 7468 6f72 2045 6d61 696c da0b 6465 7363  thor Email..desc
-000003b0: 7269 7074 696f 6e5a 0b44 6573 6372 6970  riptionZ.Descrip
-000003c0: 7469 6f6e 5a10 6c6f 6e67 5f64 6573 6372  tionZ.long_descr
-000003d0: 6970 7469 6f6e 7a0f 6669 6c65 3a20 5245  iptionz.file: RE
-000003e0: 4144 4d45 2e6d 647a 104c 6f6e 6720 4465  ADME.mdz.Long De
-000003f0: 7363 7269 7074 696f 6eda 086b 6579 776f  scription..keywo
-00000400: 7264 735a 084b 6579 776f 7264 73da 076c  rdsZ.Keywords..l
-00000410: 6963 656e 7365 7a0b 4d49 5420 4c69 6365  icensez.MIT Lice
-00000420: 6e73 655a 074c 6963 656e 7365 5a0f 7079  nseZ.LicenseZ.py
-00000430: 7468 6f6e 5f72 6571 7569 7265 737a 063e  thon_requiresz.>
-00000440: 3d20 332e 387a 0f50 7974 686f 6e20 5265  = 3.8z.Python Re
-00000450: 7175 6972 6573 5a10 696e 7374 616c 6c5f  quiresZ.install_
-00000460: 7265 7175 6972 6573 7a26 496e 7374 616c  requiresz&Instal
-00000470: 6c20 5265 7175 6972 6573 2028 652e 672e  l Requires (e.g.
-00000480: 2c20 7061 6e64 6173 2c20 6e75 6d70 7929  , pandas, numpy)
-00000490: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000004a0: 0004 0000 0053 0000 0073 1400 0000 6401  .....S...s....d.
-000004b0: 6402 8400 7c00 a000 6403 a101 4400 8301  d...|...d...D...
-000004c0: 5300 2904 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000004d0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-000004e0: 0000 0067 007c 005d 0c7d 017c 01a0 00a1  ...g.|.].}.|....
-000004f0: 0091 0271 0453 00a9 0029 01da 0573 7472  ...q.S...)...str
-00000500: 6970 2902 da02 2e30 da01 5f72 1600 0000  ip)....0.._r....
-00000510: 7216 0000 00fa 372f 686f 6d65 2f65 7567  r.....7/home/eug
-00000520: 656e 652f 7072 6f6a 6563 7473 2f62 6962  ene/projects/bib
-00000530: 6967 6f2f 7372 632f 6269 6269 676f 2f69  igo/src/bibigo/i
-00000540: 6e69 742f 7061 636b 6167 652e 7079 da0a  nit/package.py..
-00000550: 3c6c 6973 7463 6f6d 703e 2700 0000 f300  <listcomp>'.....
-00000560: 0000 007a 3269 6e69 745f 7061 636b 6167  ...z2init_packag
-00000570: 652e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  e.<locals>.<lamb
-00000580: 6461 3e2e 3c6c 6f63 616c 733e 2e3c 6c69  da>.<locals>.<li
-00000590: 7374 636f 6d70 3efa 012c 2901 da05 7370  stcomp>..,)...sp
-000005a0: 6c69 7429 01da 0178 7216 0000 0072 1600  lit)...xr....r..
-000005b0: 0000 721a 0000 00da 083c 6c61 6d62 6461  ..r......<lambda
-000005c0: 3e27 0000 0072 1c00 0000 7a1e 696e 6974  >'...r....z.init
-000005d0: 5f70 6163 6b61 6765 2e3c 6c6f 6361 6c73  _package.<locals
-000005e0: 3e2e 3c6c 616d 6264 613e 2904 720f 0000  >.<lambda>).r...
-000005f0: 0072 1000 0000 7212 0000 00da 0666 696c  .r....r......fil
-00000600: 7465 725a 1064 6570 656e 6465 6e63 795f  terZ.dependency_
-00000610: 6c69 6e6b 737a 1159 6f75 7220 5072 6976  linksz.Your Priv
-00000620: 6174 6520 5079 5049 da07 636f 6e66 6972  ate PyPI..confir
-00000630: 6d7a 1343 6f6e 6669 726d 2049 6e69 7469  mz.Confirm Initi
-00000640: 616c 697a 6572 7a18 5b45 5849 545d 204e  alizerz.[EXIT] N
-00000650: 6f74 6869 6e67 2048 6170 7065 6e65 6421  othing Happened!
-00000660: 7a04 2020 2020 da01 0a7a 0e70 7970 726f  z.    ...z.pypro
-00000670: 6a65 6374 2e74 6f6d 6c29 025a 0664 7374  ject.toml).Z.dst
-00000680: 5f66 70da 0763 6f6e 7465 6e74 7a09 7365  _fp..contentz.se
-00000690: 7475 702e 6366 67da 0373 7263 5429 01da  tup.cfg..srcT)..
-000006a0: 0865 7869 7374 5f6f 6b7a 0b5f 5f69 6e69  .exist_okz.__ini
-000006b0: 745f 5f2e 7079 7a16 5b62 6f6c 645d 5079  t__.pyz.[bold]Py
-000006c0: 7468 6f6e 2070 726f 6a65 6374 2027 7a12  thon project 'z.
-000006d0: 2720 6973 2072 6561 6479 2e5b 2f62 6f6c  ' is ready.[/bol
-000006e0: 645d 7a48 202d 2042 7569 6c64 2050 6163  d]zH - Build Pac
-000006f0: 6b61 6765 3a20 2770 7974 686f 6e20 2d6d  kage: 'python -m
-00000700: 2062 7569 6c64 272c 2070 7974 686f 6e20   build', python 
-00000710: 7061 636b 6167 6520 2762 7569 6c64 2720  package 'build' 
-00000720: 6973 2072 6571 7569 7265 642e 7a4c 202d  is required.zL -
-00000730: 2055 706c 6f61 6420 746f 2050 7950 493a   Upload to PyPI:
-00000740: 2027 7477 696e 6520 7570 6c6f 6164 2064   'twine upload d
-00000750: 6973 742f 2a27 2c20 7079 7468 6f6e 2070  ist/*', python p
-00000760: 6163 6b61 6765 2027 7477 696e 6520 6973  ackage 'twine is
-00000770: 2072 6571 7569 7265 642e 2913 5a0a 5079   required.).Z.Py
-00000780: 496e 7175 6972 6572 720b 0000 0072 0200  Inquirerr....r..
-00000790: 0000 5a08 6162 736f 6c75 7465 7210 0000  ..Z.absoluter...
-000007a0: 00da 026f 73da 0667 6574 656e 76da 0370  ...os..getenv..p
-000007b0: 6f70 da05 7072 696e 74da 046a 6f69 6e72  op..print..joinr
-000007c0: 0700 0000 7206 0000 00da 0666 6f72 6d61  ....r......forma
-000007d0: 74da 056d 6b64 6972 da06 6578 6973 7473  t..mkdir..exists
-000007e0: 5a05 746f 7563 6872 0800 0000 da07 636f  Z.touchr......co
-000007f0: 6e73 6f6c 6572 0400 0000 290d da04 726f  nsoler....)...ro
-00000800: 6f74 720b 0000 00da 0266 7072 0e00 0000  otr......fpr....
-00000810: 5a0c 7072 6976 6174 655f 7079 7069 5a0a  Z.private_pypiZ.
-00000820: 7365 7475 705f 636f 6e66 5a04 636f 6e66  setup_confZ.conf
-00000830: 7222 0000 005a 0354 4142 5a13 5059 5052  r"...Z.TABZ.PYPR
-00000840: 4f4a 4543 545f 544f 4d4c 5f46 494c 455a  OJECT_TOML_FILEZ
-00000850: 0e53 4554 5550 5f43 4647 5f46 494c 455a  .SETUP_CFG_FILEZ
-00000860: 055f 696e 6974 5a07 7375 6d6d 6172 7972  ._initZ.summaryr
-00000870: 1600 0000 7216 0000 0072 1a00 0000 da0c  ....r....r......
-00000880: 696e 6974 5f70 6163 6b61 6765 0f00 0000  init_package....
-00000890: 737a 0000 0000 010c 0308 010a 030e 040c  sz..............
-000008a0: 010a 010a 010a 010c 010a 010c 010c 0202  ................
-000008b0: 0102 0102 0106 fc04 0702 0102 0102 0102  ................
-000008c0: fc04 060a eb04 1908 010a 0104 0108 0104  ................
-000008d0: 030e 010c 0112 0104 0118 0404 0102 0106  ................
-000008e0: 0106 fe06 0604 0102 0106 0112 fe06 0610  ................
-000008f0: 0118 0114 010a 0108 011c 0118 010a 0108  ................
-00000900: 0304 020a 0102 0102 fd02 ff04 0706 0172  ...............r
-00000910: 3200 0000 290d 7227 0000 00da 0770 6174  2...).r'.....pat
-00000920: 686c 6962 7202 0000 005a 0c72 6963 682e  hlibr....Z.rich.
-00000930: 636f 6e73 6f6c 6572 0300 0000 5a0a 7269  consoler....Z.ri
-00000940: 6368 2e70 616e 656c 7204 0000 00da 0575  ch.panelr......u
-00000950: 7469 6c73 7206 0000 0072 0700 0000 7208  tilsr....r....r.
-00000960: 0000 0072 2f00 0000 7232 0000 0072 1600  ...r/...r2...r..
-00000970: 0000 7216 0000 0072 1600 0000 721a 0000  ..r....r....r...
-00000980: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000990: 0c00 0000 0801 0c02 0c01 0c02 1402 0a06  ................
+00000240: 8e01 6428 8d02 0100 642a 7d0b 740a 7c02  ..d(....d*}.t.|.
+00000250: 7c0b 1b00 740b 7c0b 8301 6428 8d02 0100  |...t.|...d(....
+00000260: 7c02 642b 1b00 6a0d 642c 642d 8d01 0100  |.d+..j.d,d-....
+00000270: 7c02 642b 1b00 7c06 6406 1900 1b00 6a0d  |.d+..|.d.....j.
+00000280: 642c 642d 8d01 0100 7c02 642b 1b00 7c06  d,d-....|.d+..|.
+00000290: 6406 1900 1b00 642e 1b00 7d0c 7c0c a00e  d.....d...}.|...
+000002a0: a100 9001 73ba 7c0c a00f a100 0100 7c02  ....s.|.......|.
+000002b0: 642b 1b00 7c06 6406 1900 1b00 7410 1b00  d+..|.d.....t...
+000002c0: 6a0d 642c 642d 8d01 0100 7c02 642b 1b00  j.d,d-....|.d+..
+000002d0: 7c06 6406 1900 1b00 7410 1b00 642e 1b00  |.d.....t...d...
+000002e0: 7d0c 7c0c a00e a100 9002 7300 7c0c a00f  }.|.......s.|...
+000002f0: a100 0100 6426 a009 642f 7c03 9b00 6430  ....d&..d/|...d0
+00000300: 9d03 6431 6432 6703 a101 7d0d 7408 8300  ..d1d2g...}.t...
+00000310: 0100 7411 a008 7412 7c0d 8301 a101 0100  ..t...t.|.......
+00000320: 6400 5300 2933 4e72 0100 0000 2901 da06  d.S.)3Nr....)...
+00000330: 7072 6f6d 7074 5a0d 5049 505f 494e 4445  promptZ.PIP_INDE
+00000340: 585f 5552 4cda 00da 0569 6e70 7574 da07  X_URL....input..
+00000350: 7072 6f6a 6563 747a 0c50 726f 6a65 6374  projectz.Project
+00000360: 204e 616d 6529 04da 0474 7970 65da 046e   Name)...type..n
+00000370: 616d 65da 0764 6566 6175 6c74 da07 6d65  ame..default..me
+00000380: 7373 6167 655a 0661 7574 686f 725a 0641  ssageZ.authorZ.A
+00000390: 7574 686f 7229 0372 0f00 0000 7210 0000  uthor).r....r...
+000003a0: 0072 1200 0000 5a0c 6175 7468 6f72 5f65  .r....Z.author_e
+000003b0: 6d61 696c 7a0c 4175 7468 6f72 2045 6d61  mailz.Author Ema
+000003c0: 696c da0b 6465 7363 7269 7074 696f 6e5a  il..descriptionZ
+000003d0: 0b44 6573 6372 6970 7469 6f6e 5a10 6c6f  .DescriptionZ.lo
+000003e0: 6e67 5f64 6573 6372 6970 7469 6f6e 7a0f  ng_descriptionz.
+000003f0: 6669 6c65 3a20 5245 4144 4d45 2e6d 647a  file: README.mdz
+00000400: 104c 6f6e 6720 4465 7363 7269 7074 696f  .Long Descriptio
+00000410: 6eda 086b 6579 776f 7264 735a 084b 6579  n..keywordsZ.Key
+00000420: 776f 7264 73da 076c 6963 656e 7365 7a0b  words..licensez.
+00000430: 4d49 5420 4c69 6365 6e73 655a 074c 6963  MIT LicenseZ.Lic
+00000440: 656e 7365 5a0f 7079 7468 6f6e 5f72 6571  enseZ.python_req
+00000450: 7569 7265 737a 063e 3d20 332e 397a 0f50  uiresz.>= 3.9z.P
+00000460: 7974 686f 6e20 5265 7175 6972 6573 5a10  ython RequiresZ.
+00000470: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000480: 7a26 496e 7374 616c 6c20 5265 7175 6972  z&Install Requir
+00000490: 6573 2028 652e 672e 2c20 7061 6e64 6173  es (e.g., pandas
+000004a0: 2c20 6e75 6d70 7929 6301 0000 0000 0000  , numpy)c.......
+000004b0: 0000 0000 0001 0000 0004 0000 0053 0000  .............S..
+000004c0: 0073 1400 0000 6401 6402 8400 7c00 a000  .s....d.d...|...
+000004d0: 6403 a101 4400 8301 5300 2904 4e63 0100  d...D...S.).Nc..
+000004e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000004f0: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00000500: 0c7d 017c 01a0 00a1 0091 0271 0453 00a9  .}.|.......q.S..
+00000510: 0029 01da 0573 7472 6970 2902 da02 2e30  .)...strip)....0
+00000520: da01 5f72 1600 0000 7216 0000 00fa 372f  .._r....r.....7/
+00000530: 686f 6d65 2f65 7567 656e 652f 7072 6f6a  home/eugene/proj
+00000540: 6563 7473 2f62 6962 6967 6f2f 7372 632f  ects/bibigo/src/
+00000550: 6269 6269 676f 2f69 6e69 742f 7061 636b  bibigo/init/pack
+00000560: 6167 652e 7079 da0a 3c6c 6973 7463 6f6d  age.py..<listcom
+00000570: 703e 2700 0000 f300 0000 007a 3269 6e69  p>'........z2ini
+00000580: 745f 7061 636b 6167 652e 3c6c 6f63 616c  t_package.<local
+00000590: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
+000005a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3efa  als>.<listcomp>.
+000005b0: 012c 2901 da05 7370 6c69 7429 01da 0178  .,)...split)...x
+000005c0: 7216 0000 0072 1600 0000 721a 0000 00da  r....r....r.....
+000005d0: 083c 6c61 6d62 6461 3e27 0000 0072 1c00  .<lambda>'...r..
+000005e0: 0000 7a1e 696e 6974 5f70 6163 6b61 6765  ..z.init_package
+000005f0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000600: 613e 2904 720f 0000 0072 1000 0000 7212  a>).r....r....r.
+00000610: 0000 00da 0666 696c 7465 725a 1064 6570  .....filterZ.dep
+00000620: 656e 6465 6e63 795f 6c69 6e6b 737a 1159  endency_linksz.Y
+00000630: 6f75 7220 5072 6976 6174 6520 5079 5049  our Private PyPI
+00000640: da07 636f 6e66 6972 6d7a 1343 6f6e 6669  ..confirmz.Confi
+00000650: 726d 2049 6e69 7469 616c 697a 6572 7a18  rm Initializerz.
+00000660: 5b45 5849 545d 204e 6f74 6869 6e67 2048  [EXIT] Nothing H
+00000670: 6170 7065 6e65 6421 7a04 2020 2020 da01  appened!z.    ..
+00000680: 0a7a 0e70 7970 726f 6a65 6374 2e74 6f6d  .z.pyproject.tom
+00000690: 6c29 025a 0664 7374 5f66 70da 0763 6f6e  l).Z.dst_fp..con
+000006a0: 7465 6e74 7a09 7365 7475 702e 6366 675a  tentz.setup.cfgZ
+000006b0: 0a44 6f63 6b65 7266 696c 65da 0373 7263  .Dockerfile..src
+000006c0: 5429 01da 0865 7869 7374 5f6f 6b7a 0b5f  T)...exist_okz._
+000006d0: 5f69 6e69 745f 5f2e 7079 7a16 5b62 6f6c  _init__.pyz.[bol
+000006e0: 645d 5079 7468 6f6e 2070 726f 6a65 6374  d]Python project
+000006f0: 2027 7a12 2720 6973 2072 6561 6479 2e5b   'z.' is ready.[
+00000700: 2f62 6f6c 645d 7a48 202d 2042 7569 6c64  /bold]zH - Build
+00000710: 2050 6163 6b61 6765 3a20 2770 7974 686f   Package: 'pytho
+00000720: 6e20 2d6d 2062 7569 6c64 272c 2070 7974  n -m build', pyt
+00000730: 686f 6e20 7061 636b 6167 6520 2762 7569  hon package 'bui
+00000740: 6c64 2720 6973 2072 6571 7569 7265 642e  ld' is required.
+00000750: 7a4c 202d 2055 706c 6f61 6420 746f 2050  zL - Upload to P
+00000760: 7950 493a 2027 7477 696e 6520 7570 6c6f  yPI: 'twine uplo
+00000770: 6164 2064 6973 742f 2a27 2c20 7079 7468  ad dist/*', pyth
+00000780: 6f6e 2070 6163 6b61 6765 2027 7477 696e  on package 'twin
+00000790: 6520 6973 2072 6571 7569 7265 642e 2913  e is required.).
+000007a0: 5a0a 5079 496e 7175 6972 6572 720b 0000  Z.PyInquirerr...
+000007b0: 0072 0200 0000 5a08 6162 736f 6c75 7465  .r....Z.absolute
+000007c0: 7210 0000 00da 026f 73da 0667 6574 656e  r......os..geten
+000007d0: 76da 0370 6f70 da05 7072 696e 74da 046a  v..pop..print..j
+000007e0: 6f69 6e72 0700 0000 7206 0000 00da 0666  oinr....r......f
+000007f0: 6f72 6d61 74da 056d 6b64 6972 da06 6578  ormat..mkdir..ex
+00000800: 6973 7473 5a05 746f 7563 6872 0800 0000  istsZ.touchr....
+00000810: da07 636f 6e73 6f6c 6572 0400 0000 290e  ..consoler....).
+00000820: da04 726f 6f74 720b 0000 00da 0266 7072  ..rootr......fpr
+00000830: 0e00 0000 5a0c 7072 6976 6174 655f 7079  ....Z.private_py
+00000840: 7069 5a0a 7365 7475 705f 636f 6e66 5a04  piZ.setup_confZ.
+00000850: 636f 6e66 7222 0000 005a 0354 4142 5a13  confr"...Z.TABZ.
+00000860: 5059 5052 4f4a 4543 545f 544f 4d4c 5f46  PYPROJECT_TOML_F
+00000870: 494c 455a 0e53 4554 5550 5f43 4647 5f46  ILEZ.SETUP_CFG_F
+00000880: 494c 455a 0f44 4f43 4b45 5246 494c 455f  ILEZ.DOCKERFILE_
+00000890: 4649 4c45 5a05 5f69 6e69 745a 0773 756d  FILEZ._initZ.sum
+000008a0: 6d61 7279 7216 0000 0072 1600 0000 721a  maryr....r....r.
+000008b0: 0000 00da 0c69 6e69 745f 7061 636b 6167  .....init_packag
+000008c0: 650f 0000 0073 8400 0000 0001 0c03 0801  e....s..........
+000008d0: 0a03 0e04 0c01 0a01 0a01 0a01 0c01 0a01  ................
+000008e0: 0c01 0c02 0201 0201 0201 06fc 0407 0201  ................
+000008f0: 0201 0201 02fc 0406 0aeb 0419 0801 0a01  ................
+00000900: 0401 0801 0403 0e01 0c01 1201 0401 1804  ................
+00000910: 0401 0201 0601 06fe 0606 0401 0201 0601  ................
+00000920: 12fe 0606 0401 0201 0601 06fe 0606 1001  ................
+00000930: 1801 1401 0a01 0801 1c01 1801 0a01 0803  ................
+00000940: 0402 0a01 0201 02fd 02ff 0407 0601 7232  ..............r2
+00000950: 0000 0029 0d72 2700 0000 da07 7061 7468  ...).r'.....path
+00000960: 6c69 6272 0200 0000 5a0c 7269 6368 2e63  libr....Z.rich.c
+00000970: 6f6e 736f 6c65 7203 0000 005a 0a72 6963  onsoler....Z.ric
+00000980: 682e 7061 6e65 6c72 0400 0000 da05 7574  h.panelr......ut
+00000990: 696c 7372 0600 0000 7207 0000 0072 0800  ilsr....r....r..
+000009a0: 0000 722f 0000 0072 3200 0000 7216 0000  ..r/...r2...r...
+000009b0: 0072 1600 0000 7216 0000 0072 1a00 0000  .r....r....r....
+000009c0: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
+000009d0: 0000 0008 010c 020c 010c 0214 020a 06    ...............
```

### Comparing `bibigo-0.0.6/src/bibigo/init/__pycache__/settings.cpython-39.pyc` & `bibigo-0.0.7/src/bibigo/init/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/init/package.py` & `bibigo-0.0.7/src/bibigo/init/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         {"type": "input", "name": "project", "default": project, "message": "Project Name"},
         {"type": "input", "name": "author", "message": "Author"},
         {"type": "input", "name": "author_email", "message": "Author Email"},
         {"type": "input", "name": "description", "message": "Description"},
         {"type": "input", "name": "long_description", "default": "file: README.md", "message": "Long Description"},
         {"type": "input", "name": "keywords", "message": "Keywords"},
         {"type": "input", "name": "license", "default": "MIT License", "message": "License"},
-        {"type": "input", "name": "python_requires", "default": ">= 3.8", "message": "Python Requires"},
+        {"type": "input", "name": "python_requires", "default": ">= 3.9", "message": "Python Requires"},
         {
             "type": "input",
             "name": "install_requires",
             "message": "Install Requires (e.g., pandas, numpy)",
             "filter": lambda x: [_.strip() for _ in x.split(",")],
         },
         {
@@ -72,14 +72,21 @@
     # setup.cfg
     SETUP_CFG_FILE = "setup.cfg"
     write(
         dst_fp=fp / SETUP_CFG_FILE,
         content=read(SETUP_CFG_FILE).format(**conf),
     )
 
+    # Dockerfile
+    DOCKERFILE_FILE = "Dockerfile"
+    write(
+        dst_fp=fp / DOCKERFILE_FILE,
+        content=read(DOCKERFILE_FILE),
+    )
+
     # make src directory
     (fp / "src").mkdir(exist_ok=True)
     (fp / "src" / conf["project"]).mkdir(exist_ok=True)
     _init = fp / "src" / conf["project"] / "__init__.py"
     if not _init.exists():
         _init.touch()
     (fp / "src" / conf["project"] / STATIC_DIR).mkdir(exist_ok=True)
```

### Comparing `bibigo-0.0.6/src/bibigo/init/settings.py` & `bibigo-0.0.7/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/scripts.py` & `bibigo-0.0.7/src/bibigo/scripts.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/static/.dockerignore.default` & `bibigo-0.0.7/src/bibigo/static/.dockerignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/static/.gitignore.default` & `bibigo-0.0.7/src/bibigo/static/.gitignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/static/setup.cfg.default` & `bibigo-0.0.7/src/bibigo/static/setup.cfg.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.6/src/bibigo/utils.py` & `bibigo-0.0.7/src/bibigo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from typing import Union
 from pathlib import Path
 import pkgutil
 
 STATIC_DIR = "static"
 
+
 # ensure path
 def ensure_path(fp: Union[str, Path]):
     return Path(fp)
 
 
 # read file
 def read(fn: Path, version: str = "default"):
```

### Comparing `bibigo-0.0.6/src/bibigo.egg-info/SOURCES.txt` & `bibigo-0.0.7/src/bibigo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 src/bibigo/init/package.py
 src/bibigo/init/settings.py
 src/bibigo/init/__pycache__/__init__.cpython-39.pyc
 src/bibigo/init/__pycache__/package.cpython-39.pyc
 src/bibigo/init/__pycache__/settings.cpython-39.pyc
 src/bibigo/static/.dockerignore.default
 src/bibigo/static/.gitignore.default
+src/bibigo/static/Dockerfile.default
 src/bibigo/static/__init__.py
 src/bibigo/static/pyproject.toml.default
 src/bibigo/static/setup.cfg.default
 src/bibigo/static/.vscode/__init__.py
 src/bibigo/static/.vscode/settings.json.default
```

