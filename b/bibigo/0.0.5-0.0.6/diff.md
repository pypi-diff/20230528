# Comparing `tmp/bibigo-0.0.5.tar.gz` & `tmp/bibigo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibigo-0.0.5.tar", last modified: Sun May 28 08:13:23 2023, max compression
+gzip compressed data, was "bibigo-0.0.6.tar", last modified: Sun May 28 08:33:43 2023, max compression
```

## Comparing `bibigo-0.0.5.tar` & `bibigo-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.5/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:13:23.767126 bibigo-0.0.5/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.5/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.5/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      550 2023-05-28 08:13:23.767126 bibigo-0.0.5/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.763126 bibigo-0.0.5/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.5/src/bibigo/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.5/src/bibigo/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.5/src/bibigo/__pycache__/scripts.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.5/src/bibigo/__pycache__/test.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      985 2023-05-28 06:20:30.000000 bibigo-0.0.5/src/bibigo/__pycache__/utils.cpython-39.pyc
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/files/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.5/src/bibigo/files/.dockerignore.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.5/src/bibigo/files/.gitignore.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/files/.vscode/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.5/src/bibigo/files/.vscode/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.5/src/bibigo/files/.vscode/settings.json.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.5/src/bibigo/files/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.5/src/bibigo/files/pyproject.toml.default
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      508 2023-05-28 05:57:29.000000 bibigo-0.0.5/src/bibigo/files/setup.cfg.default
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/init/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.5/src/bibigo/init/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo/init/__pycache__/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.5/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2212 2023-05-28 06:34:44.000000 bibigo-0.0.5/src/bibigo/init/__pycache__/package.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.5/src/bibigo/init/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2916 2023-05-28 06:27:56.000000 bibigo-0.0.5/src/bibigo/init/package.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.5/src/bibigo/init/settings.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.5/src/bibigo/scripts.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      710 2023-05-28 06:20:23.000000 bibigo-0.0.5/src/bibigo/utils.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:13:23.767126 bibigo-0.0.5/src/bibigo.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      994 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 08:13:23.000000 bibigo-0.0.5/src/bibigo.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 04:22:26.000000 bibigo-0.0.6/LICENSE
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:33:43.205176 bibigo-0.0.6/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2463 2023-05-28 07:01:48.000000 bibigo-0.0.6/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 04:22:26.000000 bibigo-0.0.6/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      564 2023-05-28 08:33:43.205176 bibigo-0.0.6/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 04:22:26.000000 bibigo-0.0.6/src/bibigo/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      142 2023-05-28 04:26:51.000000 bibigo-0.0.6/src/bibigo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1326 2023-05-28 07:01:01.000000 bibigo-0.0.6/src/bibigo/__pycache__/scripts.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      253 2023-05-28 05:12:29.000000 bibigo-0.0.6/src/bibigo/__pycache__/test.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1009 2023-05-28 08:23:08.000000 bibigo-0.0.6/src/bibigo/__pycache__/utils.cpython-39.pyc
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/init/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 05:34:29.000000 bibigo-0.0.6/src/bibigo/init/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/init/__pycache__/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      147 2023-05-28 05:44:17.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2464 2023-05-28 08:32:34.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/package.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1057 2023-05-28 07:01:01.000000 bibigo-0.0.6/src/bibigo/init/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3342 2023-05-28 08:32:20.000000 bibigo-0.0.6/src/bibigo/init/package.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1163 2023-05-28 06:52:40.000000 bibigo-0.0.6/src/bibigo/init/settings.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      971 2023-05-28 06:53:09.000000 bibigo-0.0.6/src/bibigo/scripts.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/static/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1293 2023-05-28 05:03:37.000000 bibigo-0.0.6/src/bibigo/static/.dockerignore.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1798 2023-05-28 05:23:42.000000 bibigo-0.0.6/src/bibigo/static/.gitignore.default
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.205176 bibigo-0.0.6/src/bibigo/static/.vscode/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:01:16.000000 bibigo-0.0.6/src/bibigo/static/.vscode/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      455 2023-05-28 07:19:46.000000 bibigo-0.0.6/src/bibigo/static/.vscode/settings.json.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 07:53:07.000000 bibigo-0.0.6/src/bibigo/static/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 05:31:07.000000 bibigo-0.0.6/src/bibigo/static/pyproject.toml.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      616 2023-05-28 08:20:22.000000 bibigo-0.0.6/src/bibigo/static/setup.cfg.default
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      735 2023-05-28 08:17:40.000000 bibigo-0.0.6/src/bibigo/utils.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 08:33:43.201176 bibigo-0.0.6/src/bibigo.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      167 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1001 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       51 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 08:33:43.000000 bibigo-0.0.6/src/bibigo.egg-info/top_level.txt
```

### Comparing `bibigo-0.0.5/LICENSE` & `bibigo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/README.md` & `bibigo-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/setup.cfg` & `bibigo-0.0.6/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 bibigo = 
-	files/**/*
-	files/**/.*
-	files/.vscode/*
+	static/**/*
+	static/**/.*
+	static/.**/*
+	static/.**/.*
 
 [options.entry_points]
 console_scripts = 
 	bibigo = bibigo.scripts:bibigo
 
 [egg_info]
 tag_build =
```

### Comparing `bibigo-0.0.5/src/bibigo/__pycache__/scripts.cpython-39.pyc` & `bibigo-0.0.6/src/bibigo/__pycache__/scripts.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/__pycache__/utils.cpython-39.pyc` & `bibigo-0.0.6/src/bibigo/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 06:20:23 2023 UTC, .py size: 710 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-00000000: 610d 0d0a 0000 0000 a7f2 7264 c602 0000  a.........rd....
+00000000: 610d 0d0a 0000 0000 240e 7364 df02 0000  a.......$.sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6401 6c05 5a05 6502 6506 6504 6602 1900  d.l.Z.e.e.e.f...
-00000060: 6404 9c01 6405 6406 8404 5a07 640f 6504  d...d.d...Z.d.e.
-00000070: 6506 6408 9c02 6409 640a 8405 5a08 6410  e.d...d.d...Z.d.
-00000080: 6504 640c 9c01 640d 640e 8405 5a09 6401  e.d...d.d...Z.d.
-00000090: 5300 2911 e900 0000 004e 2901 da05 556e  S.)......N)...Un
-000000a0: 696f 6ea9 01da 0450 6174 68a9 01da 0266  ion....Path....f
-000000b0: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
-000000c0: 0000 0200 0000 4300 0000 7308 0000 0074  ......C...s....t
-000000d0: 007c 0083 0153 0029 014e 7203 0000 0072  .|...S.).Nr....r
-000000e0: 0500 0000 a900 7207 0000 00fa 302f 686f  ......r.....0/ho
-000000f0: 6d65 2f65 7567 656e 652f 7072 6f6a 6563  me/eugene/projec
-00000100: 7473 2f62 6962 6967 6f2f 7372 632f 6269  ts/bibigo/src/bi
-00000110: 6269 676f 2f75 7469 6c73 2e70 79da 0b65  bigo/utils.py..e
-00000120: 6e73 7572 655f 7061 7468 0800 0000 7302  nsure_path....s.
-00000130: 0000 0000 0172 0900 0000 da07 6465 6661  .....r......defa
-00000140: 756c 7429 02da 0266 6eda 0776 6572 7369  ult)...fn..versi
-00000150: 6f6e 6302 0000 0000 0000 0000 0000 0004  onc.............
-00000160: 0000 0005 0000 0043 0000 0073 2e00 0000  .......C...s....
-00000170: 7400 6401 8301 7c00 9b00 6402 7c01 9b00  t.d...|...d.|...
-00000180: 9d03 1b00 7d02 7401 a002 7403 7c02 a004  ....}.t...t.|...
-00000190: a100 a102 a005 a100 7d03 7c03 5300 2903  ........}.|.S.).
-000001a0: 4eda 0566 696c 6573 da01 2e29 0672 0400  N..files...).r..
-000001b0: 0000 da07 706b 6775 7469 6cda 0867 6574  ....pkgutil..get
-000001c0: 5f64 6174 61da 085f 5f6e 616d 655f 5fda  _data..__name__.
-000001d0: 0861 735f 706f 7369 78da 0664 6563 6f64  .as_posix..decod
-000001e0: 6529 0472 0b00 0000 720c 0000 0072 0600  e).r....r....r..
-000001f0: 0000 da07 636f 6e74 656e 7472 0700 0000  ....contentr....
-00000200: 7207 0000 0072 0800 0000 da04 7265 6164  r....r......read
-00000210: 0d00 0000 7306 0000 0000 0116 0114 0172  ....s..........r
-00000220: 1500 0000 da01 7729 01da 0664 7374 5f66  ......w)...dst_f
-00000230: 7063 0300 0000 0000 0000 0000 0000 0400  pc..............
-00000240: 0000 0800 0000 4300 0000 736c 0000 0074  ......C...sl...t
-00000250: 007c 0083 017d 007c 006a 016a 0264 0164  .|...}.|.j.j.d.d
-00000260: 0164 028d 0201 0074 037c 007c 0283 028f  .d.....t.|.|....
-00000270: 367d 037c 006a 04a0 05a1 0064 0376 0072  6}.|.j.....d.v.r
-00000280: 4074 06a0 077c 017c 03a1 0201 006e 0a7c  @t...|.|.....n.|
-00000290: 03a0 087c 01a1 0101 0057 0064 0004 0004  ...|.....W.d....
-000002a0: 0083 0301 006e 1031 0073 5e30 0001 0001  .....n.1.s^0....
-000002b0: 0001 0059 0001 0064 0053 0029 044e 5429  ...Y...d.S.).NT)
-000002c0: 02da 0770 6172 656e 7473 da08 6578 6973  ...parents..exis
-000002d0: 745f 6f6b 2901 da04 6a73 6f6e 2909 7209  t_ok)...json).r.
-000002e0: 0000 00da 0670 6172 656e 74da 056d 6b64  .....parent..mkd
-000002f0: 6972 da04 6f70 656e da06 7375 6666 6978  ir..open..suffix
-00000300: da05 6c6f 7765 7272 1a00 0000 da04 6475  ..lowerr......du
-00000310: 6d70 da05 7772 6974 6529 0472 1700 0000  mp..write).r....
-00000320: 7214 0000 00da 046d 6f64 65da 0266 7772  r......mode..fwr
-00000330: 0700 0000 7207 0000 0072 0800 0000 7221  ....r....r....r!
-00000340: 0000 0014 0000 0073 0c00 0000 0001 0803  .......s........
-00000350: 1003 0c01 0e01 0e02 7221 0000 0029 0172  ........r!...).r
-00000360: 0a00 0000 2901 7216 0000 0029 0a72 1a00  ....).r....).r..
-00000370: 0000 da06 7479 7069 6e67 7202 0000 00da  ....typingr.....
-00000380: 0770 6174 686c 6962 7204 0000 0072 0f00  .pathlibr....r..
-00000390: 0000 da03 7374 7272 0900 0000 7215 0000  ....strr....r...
-000003a0: 0072 2100 0000 7207 0000 0072 0700 0000  .r!...r....r....
-000003b0: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
-000003c0: 756c 653e 0100 0000 730c 0000 0008 010c  ule>....s.......
-000003d0: 010c 0108 0416 0512 07                   .........
+00000050: 6401 6c05 5a05 6404 5a06 6502 6507 6504  d.l.Z.d.Z.e.e.e.
+00000060: 6602 1900 6405 9c01 6406 6407 8404 5a08  f...d...d.d...Z.
+00000070: 6410 6504 6507 6409 9c02 640a 640b 8405  d.e.e.d...d.d...
+00000080: 5a09 6411 6504 640d 9c01 640e 640f 8405  Z.d.e.d...d.d...
+00000090: 5a0a 6401 5300 2912 e900 0000 004e 2901  Z.d.S.)......N).
+000000a0: da05 556e 696f 6ea9 01da 0450 6174 685a  ..Union....PathZ
+000000b0: 0673 7461 7469 63a9 01da 0266 7063 0100  .static....fpc..
+000000c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000000d0: 0000 4300 0000 7308 0000 0074 007c 0083  ..C...s....t.|..
+000000e0: 0153 0029 014e 7203 0000 0072 0500 0000  .S.).Nr....r....
+000000f0: a900 7207 0000 00fa 302f 686f 6d65 2f65  ..r.....0/home/e
+00000100: 7567 656e 652f 7072 6f6a 6563 7473 2f62  ugene/projects/b
+00000110: 6962 6967 6f2f 7372 632f 6269 6269 676f  ibigo/src/bibigo
+00000120: 2f75 7469 6c73 2e70 79da 0b65 6e73 7572  /utils.py..ensur
+00000130: 655f 7061 7468 0900 0000 7302 0000 0000  e_path....s.....
+00000140: 0172 0900 0000 da07 6465 6661 756c 7429  .r......default)
+00000150: 02da 0266 6eda 0776 6572 7369 6f6e 6302  ...fn..versionc.
+00000160: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000170: 0000 0043 0000 0073 2e00 0000 7400 7401  ...C...s....t.t.
+00000180: 8301 7c00 9b00 6401 7c01 9b00 9d03 1b00  ..|...d.|.......
+00000190: 7d02 7402 a003 7404 7c02 a005 a100 a102  }.t...t.|.......
+000001a0: a006 a100 7d03 7c03 5300 2902 4eda 012e  ....}.|.S.).N...
+000001b0: 2907 7204 0000 00da 0a53 5441 5449 435f  ).r......STATIC_
+000001c0: 4449 52da 0770 6b67 7574 696c da08 6765  DIR..pkgutil..ge
+000001d0: 745f 6461 7461 da08 5f5f 6e61 6d65 5f5f  t_data..__name__
+000001e0: da08 6173 5f70 6f73 6978 da06 6465 636f  ..as_posix..deco
+000001f0: 6465 2904 720b 0000 0072 0c00 0000 7206  de).r....r....r.
+00000200: 0000 00da 0763 6f6e 7465 6e74 7207 0000  .....contentr...
+00000210: 0072 0700 0000 7208 0000 00da 0472 6561  .r....r......rea
+00000220: 640e 0000 0073 0600 0000 0001 1601 1401  d....s..........
+00000230: 7215 0000 00da 0177 2901 da06 6473 745f  r......w)...dst_
+00000240: 6670 6303 0000 0000 0000 0000 0000 0004  fpc.............
+00000250: 0000 0008 0000 0043 0000 0073 6c00 0000  .......C...sl...
+00000260: 7400 7c00 8301 7d00 7c00 6a01 6a02 6401  t.|...}.|.j.j.d.
+00000270: 6401 6402 8d02 0100 7403 7c00 7c02 8302  d.d.....t.|.|...
+00000280: 8f36 7d03 7c00 6a04 a005 a100 6403 7600  .6}.|.j.....d.v.
+00000290: 7240 7406 a007 7c01 7c03 a102 0100 6e0a  r@t...|.|.....n.
+000002a0: 7c03 a008 7c01 a101 0100 5700 6400 0400  |...|.....W.d...
+000002b0: 0400 8303 0100 6e10 3100 735e 3000 0100  ......n.1.s^0...
+000002c0: 0100 0100 5900 0100 6400 5300 2904 4e54  ....Y...d.S.).NT
+000002d0: 2902 da07 7061 7265 6e74 73da 0865 7869  )...parents..exi
+000002e0: 7374 5f6f 6b29 01da 046a 736f 6e29 0972  st_ok)...json).r
+000002f0: 0900 0000 da06 7061 7265 6e74 da05 6d6b  ......parent..mk
+00000300: 6469 72da 046f 7065 6eda 0673 7566 6669  dir..open..suffi
+00000310: 78da 056c 6f77 6572 721a 0000 00da 0464  x..lowerr......d
+00000320: 756d 70da 0577 7269 7465 2904 7217 0000  ump..write).r...
+00000330: 0072 1400 0000 da04 6d6f 6465 da02 6677  .r......mode..fw
+00000340: 7207 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000350: 2100 0000 1500 0000 730c 0000 0000 0108  !.......s.......
+00000360: 0310 030c 010e 010e 0272 2100 0000 2901  .........r!...).
+00000370: 720a 0000 0029 0172 1600 0000 290b 721a  r....).r....).r.
+00000380: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
+00000390: da07 7061 7468 6c69 6272 0400 0000 720f  ..pathlibr....r.
+000003a0: 0000 0072 0e00 0000 da03 7374 7272 0900  ...r......strr..
+000003b0: 0000 7215 0000 0072 2100 0000 7207 0000  ..r....r!...r...
+000003c0: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
+000003d0: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+000003e0: 0000 0008 010c 010c 0108 0204 0316 0512  ................
+000003f0: 07                                       .
```

### Comparing `bibigo-0.0.5/src/bibigo/files/.dockerignore.default` & `bibigo-0.0.6/src/bibigo/static/.dockerignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/files/.gitignore.default` & `bibigo-0.0.6/src/bibigo/static/.gitignore.default`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/init/__pycache__/package.cpython-39.pyc` & `bibigo-0.0.6/src/bibigo/init/__pycache__/package.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 28 06:27:56 2023 UTC, .py size: 2916 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,154 @@
-00000000: 610d 0d0a 0000 0000 6cf4 7264 640b 0000  a.......l.rdd...
+00000000: 610d 0d0a 0000 0000 9411 7364 0e0d 0000  a.........sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 6d09 5a09 0100 6504 6407 6408  m.Z.m.Z...e.d.d.
-00000070: 8d01 5a0a 6409 640a 8400 5a0b 6401 5300  ..Z.d.d...Z.d.S.
-00000080: 290b e900 0000 004e 2901 da04 5061 7468  )......N)...Path
-00000090: 2901 da07 436f 6e73 6f6c 6529 01da 0550  )...Console)...P
-000000a0: 616e 656c e902 0000 0029 02da 0472 6561  anel.....)...rea
-000000b0: 64da 0577 7269 7465 e958 0000 0029 01da  d..write.X...)..
-000000c0: 0577 6964 7468 6301 0000 0000 0000 0000  .widthc.........
-000000d0: 0000 000c 0000 000e 0000 0043 0000 0073  ...........C...s
-000000e0: 8401 0000 6401 6402 6c00 6d01 7d01 0100  ....d.d.l.m.}...
-000000f0: 7402 7c00 8301 7d02 7c02 a003 a100 6a04  t.|...}.|.....j.
-00000100: 7d03 7405 a006 6403 a101 702a 6404 7d04  }.t...d...p*d.}.
-00000110: 6405 6406 7c03 6407 6408 9c04 6405 6409  d.d.|.d.d...d.d.
-00000120: 640a 640b 9c03 6405 640c 640d 640b 9c03  d.d...d.d.d.d...
-00000130: 6405 640e 640f 640b 9c03 6405 6410 6411  d.d.d.d...d.d.d.
-00000140: 6412 6408 9c04 6405 6413 6414 640b 9c03  d.d...d.d.d.d...
-00000150: 6405 6415 6416 6417 6408 9c04 6405 6418  d.d.d.d.d...d.d.
-00000160: 6419 641a 6408 9c04 6405 641b 641c 641d  d.d.d...d.d.d.d.
-00000170: 641e 8400 641f 9c04 6405 6420 7c04 6421  d...d...d.d |.d!
-00000180: 6408 9c04 6422 6422 6423 640b 9c03 670b  d...d"d"d#d...g.
-00000190: 7d05 7c01 7c05 8301 7d06 7c06 a007 6422  }.|.|...}.|...d"
-000001a0: a101 7d07 7c07 73d0 7408 6424 8301 0100  ..}.|.s.t.d$....
-000001b0: 6400 5300 7c06 641b 1900 6400 7501 9001  d.S.|.d...d.u...
-000001c0: 7218 6404 7c06 641b 1900 7601 72fc 6404  r.d.|.d...v.r.d.
-000001d0: 6701 7c06 641b 1900 a201 7c06 641b 3c00  g.|.d.....|.d.<.
-000001e0: 6425 7d08 6426 7c08 9b00 9d02 a009 7c06  d%}.d&|.......|.
-000001f0: 641b 1900 a101 7c06 641b 3c00 6427 7d09  d.....|.d.<.d'}.
-00000200: 740a 7c02 7c09 1b00 740b 7c09 8301 6428  t.|.|...t.|...d(
-00000210: 8d02 0100 6429 7d0a 740a 7c02 7c0a 1b00  ....d)}.t.|.|...
-00000220: 740b 7c0a 8301 6a0c 6600 6900 7c06 a401  t.|...j.f.i.|...
-00000230: 8e01 6428 8d02 0100 6426 a009 642a 7c03  ..d(....d&..d*|.
-00000240: 9b00 642b 9d03 642c 642d 6703 a101 7d0b  ..d+..d,d-g...}.
-00000250: 7408 8300 0100 740d a008 740e 7c0b 8301  t.....t...t.|...
-00000260: a101 0100 6400 5300 292e 4e72 0100 0000  ....d.S.).Nr....
-00000270: 2901 da06 7072 6f6d 7074 5a0d 5049 505f  )...promptZ.PIP_
-00000280: 494e 4445 585f 5552 4cda 00da 0569 6e70  INDEX_URL....inp
-00000290: 7574 da07 7072 6f6a 6563 747a 0c50 726f  ut..projectz.Pro
-000002a0: 6a65 6374 204e 616d 6529 04da 0474 7970  ject Name)...typ
-000002b0: 65da 046e 616d 65da 0764 6566 6175 6c74  e..name..default
-000002c0: da07 6d65 7373 6167 65da 0661 7574 686f  ..message..autho
-000002d0: 72da 0641 7574 686f 7229 0372 0e00 0000  r..Author).r....
-000002e0: 720f 0000 0072 1100 0000 da0c 6175 7468  r....r......auth
-000002f0: 6f72 5f65 6d61 696c 7a0c 4175 7468 6f72  or_emailz.Author
-00000300: 2045 6d61 696c da0b 6465 7363 7269 7074   Email..descript
-00000310: 696f 6eda 0b44 6573 6372 6970 7469 6f6e  ion..Description
-00000320: da10 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000330: 6f6e 7a0f 6669 6c65 3a20 5245 4144 4d45  onz.file: README
-00000340: 2e6d 647a 104c 6f6e 6720 4465 7363 7269  .mdz.Long Descri
-00000350: 7074 696f 6eda 086b 6579 776f 7264 73da  ption..keywords.
-00000360: 084b 6579 776f 7264 73da 076c 6963 656e  .Keywords..licen
-00000370: 7365 7a0b 4d49 5420 4c69 6365 6e73 65da  sez.MIT License.
-00000380: 074c 6963 656e 7365 da0f 7079 7468 6f6e  .License..python
-00000390: 5f72 6571 7569 7265 737a 063e 3d20 332e  _requiresz.>= 3.
-000003a0: 387a 0f50 7974 686f 6e20 5265 7175 6972  8z.Python Requir
-000003b0: 6573 da10 696e 7374 616c 6c5f 7265 7175  es..install_requ
-000003c0: 6972 6573 7a26 496e 7374 616c 6c20 5265  iresz&Install Re
-000003d0: 7175 6972 6573 2028 652e 672e 2c20 7061  quires (e.g., pa
-000003e0: 6e64 6173 2c20 6e75 6d70 7929 6301 0000  ndas, numpy)c...
-000003f0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000400: 0053 0000 0073 1400 0000 6401 6402 8400  .S...s....d.d...
-00000410: 7c00 a000 6403 a101 4400 8301 5300 2904  |...d...D...S.).
-00000420: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00000430: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00000440: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
-00000450: 0453 00a9 0029 01da 0573 7472 6970 2902  .S...)...strip).
-00000460: da02 2e30 da01 5f72 1e00 0000 721e 0000  ...0.._r....r...
-00000470: 00fa 372f 686f 6d65 2f65 7567 656e 652f  ..7/home/eugene/
-00000480: 7072 6f6a 6563 7473 2f62 6962 6967 6f2f  projects/bibigo/
-00000490: 7372 632f 6269 6269 676f 2f69 6e69 742f  src/bibigo/init/
-000004a0: 7061 636b 6167 652e 7079 da0a 3c6c 6973  package.py..<lis
-000004b0: 7463 6f6d 703e 2700 0000 f300 0000 007a  tcomp>'........z
-000004c0: 3269 6e69 745f 7061 636b 6167 652e 3c6c  2init_package.<l
-000004d0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e2e  ocals>.<lambda>.
-000004e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000004f0: 6d70 3efa 012c 2901 da05 7370 6c69 7429  mp>..,)...split)
-00000500: 01da 0178 721e 0000 0072 1e00 0000 7222  ...xr....r....r"
-00000510: 0000 00da 083c 6c61 6d62 6461 3e27 0000  .....<lambda>'..
-00000520: 0072 2400 0000 7a1e 696e 6974 5f70 6163  .r$...z.init_pac
-00000530: 6b61 6765 2e3c 6c6f 6361 6c73 3e2e 3c6c  kage.<locals>.<l
-00000540: 616d 6264 613e 2904 720e 0000 0072 0f00  ambda>).r....r..
-00000550: 0000 7211 0000 00da 0666 696c 7465 72da  ..r......filter.
-00000560: 1064 6570 656e 6465 6e63 795f 6c69 6e6b  .dependency_link
-00000570: 737a 1159 6f75 7220 5072 6976 6174 6520  sz.Your Private 
-00000580: 5079 5049 da07 636f 6e66 6972 6d7a 1343  PyPI..confirmz.C
-00000590: 6f6e 6669 726d 2049 6e69 7469 616c 697a  onfirm Initializ
-000005a0: 6572 7a18 5b45 5849 545d 204e 6f74 6869  erz.[EXIT] Nothi
-000005b0: 6e67 2048 6170 7065 6e65 6421 7a04 2020  ng Happened!z.  
-000005c0: 2020 da01 0a7a 0e70 7970 726f 6a65 6374    ...z.pyproject
-000005d0: 2e74 6f6d 6c29 02da 0664 7374 5f66 70da  .toml)...dst_fp.
-000005e0: 0763 6f6e 7465 6e74 7a09 7365 7475 702e  .contentz.setup.
-000005f0: 6366 677a 165b 626f 6c64 5d50 7974 686f  cfgz.[bold]Pytho
-00000600: 6e20 7072 6f6a 6563 7420 277a 1227 2069  n project 'z.' i
-00000610: 7320 7265 6164 792e 5b2f 626f 6c64 5d7a  s ready.[/bold]z
-00000620: 4820 2d20 4275 696c 6420 5061 636b 6167  H - Build Packag
-00000630: 653a 2027 7079 7468 6f6e 202d 6d20 6275  e: 'python -m bu
-00000640: 696c 6427 2c20 7079 7468 6f6e 2070 6163  ild', python pac
-00000650: 6b61 6765 2027 6275 696c 6427 2069 7320  kage 'build' is 
-00000660: 7265 7175 6972 6564 2e7a 4c20 2d20 5570  required.zL - Up
-00000670: 6c6f 6164 2074 6f20 5079 5049 3a20 2774  load to PyPI: 't
-00000680: 7769 6e65 2075 706c 6f61 6420 6469 7374  wine upload dist
-00000690: 2f2a 272c 2070 7974 686f 6e20 7061 636b  /*', python pack
-000006a0: 6167 6520 2774 7769 6e65 2069 7320 7265  age 'twine is re
-000006b0: 7175 6972 6564 2e29 0fda 0a50 7949 6e71  quired.)...PyInq
-000006c0: 7569 7265 7272 0a00 0000 7202 0000 00da  uirerr....r.....
-000006d0: 0861 6273 6f6c 7574 6572 0f00 0000 da02  .absoluter......
-000006e0: 6f73 da06 6765 7465 6e76 da03 706f 70da  os..getenv..pop.
-000006f0: 0570 7269 6e74 da04 6a6f 696e 7207 0000  .print..joinr...
-00000700: 0072 0600 0000 da06 666f 726d 6174 da07  .r......format..
-00000710: 636f 6e73 6f6c 6572 0400 0000 290c da04  consoler....)...
-00000720: 726f 6f74 720a 0000 00da 0266 7072 0d00  rootr......fpr..
-00000730: 0000 da0c 7072 6976 6174 655f 7079 7069  ....private_pypi
-00000740: 5a0a 7365 7475 705f 636f 6e66 da04 636f  Z.setup_conf..co
-00000750: 6e66 722b 0000 00da 0354 4142 5a13 5059  nfr+.....TABZ.PY
-00000760: 5052 4f4a 4543 545f 544f 4d4c 5f46 494c  PROJECT_TOML_FIL
-00000770: 455a 0e53 4554 5550 5f43 4647 5f46 494c  EZ.SETUP_CFG_FIL
-00000780: 45da 0773 756d 6d61 7279 721e 0000 0072  E..summaryr....r
-00000790: 1e00 0000 7222 0000 00da 0c69 6e69 745f  ....r".....init_
-000007a0: 7061 636b 6167 650f 0000 0073 6800 0000  package....sh...
-000007b0: 0001 0c03 0801 0a03 0e04 0c01 0a01 0a01  ................
-000007c0: 0a01 0c01 0a01 0c01 0c02 0201 0201 0201  ................
-000007d0: 06fc 0407 0201 0201 0201 02fc 0406 0aeb  ................
-000007e0: 0419 0801 0a01 0401 0801 0403 0e01 0c01  ................
-000007f0: 1201 0401 1804 0401 0201 0601 06fe 0606  ................
-00000800: 0401 0201 0601 12fe 0606 0402 0a01 0201  ................
-00000810: 02fd 02ff 0407 0601 723e 0000 0029 0c72  ........r>...).r
-00000820: 3100 0000 da07 7061 7468 6c69 6272 0200  1.....pathlibr..
-00000830: 0000 da0c 7269 6368 2e63 6f6e 736f 6c65  ....rich.console
-00000840: 7203 0000 005a 0a72 6963 682e 7061 6e65  r....Z.rich.pane
-00000850: 6c72 0400 0000 da05 7574 696c 7372 0600  lr......utilsr..
-00000860: 0000 7207 0000 0072 3700 0000 723e 0000  ..r....r7...r>..
-00000870: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00000880: 7222 0000 00da 083c 6d6f 6475 6c65 3e01  r".....<module>.
-00000890: 0000 0073 0c00 0000 0801 0c02 0c01 0c02  ...s............
-000008a0: 1002 0a06                                ....
+00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6504  m.Z.m.Z.m.Z...e.
+00000070: 6407 6408 8d01 5a0b 6409 640a 8400 5a0c  d.d...Z.d.d...Z.
+00000080: 6401 5300 290b e900 0000 004e 2901 da04  d.S.)......N)...
+00000090: 5061 7468 2901 da07 436f 6e73 6f6c 6529  Path)...Console)
+000000a0: 01da 0550 616e 656c e902 0000 0029 03da  ...Panel.....)..
+000000b0: 0472 6561 64da 0577 7269 7465 da0a 5354  .read..write..ST
+000000c0: 4154 4943 5f44 4952 e958 0000 0029 01da  ATIC_DIR.X...)..
+000000d0: 0577 6964 7468 6301 0000 0000 0000 0000  .widthc.........
+000000e0: 0000 000d 0000 000e 0000 0043 0000 0073  ...........C...s
+000000f0: 1802 0000 6401 6402 6c00 6d01 7d01 0100  ....d.d.l.m.}...
+00000100: 7402 7c00 8301 7d02 7c02 a003 a100 6a04  t.|...}.|.....j.
+00000110: 7d03 7405 a006 6403 a101 702a 6404 7d04  }.t...d...p*d.}.
+00000120: 6405 6406 7c03 6407 6408 9c04 6405 6409  d.d.|.d.d...d.d.
+00000130: 640a 640b 9c03 6405 640c 640d 640b 9c03  d.d...d.d.d.d...
+00000140: 6405 640e 640f 640b 9c03 6405 6410 6411  d.d.d.d...d.d.d.
+00000150: 6412 6408 9c04 6405 6413 6414 640b 9c03  d.d...d.d.d.d...
+00000160: 6405 6415 6416 6417 6408 9c04 6405 6418  d.d.d.d.d...d.d.
+00000170: 6419 641a 6408 9c04 6405 641b 641c 641d  d.d.d...d.d.d.d.
+00000180: 641e 8400 641f 9c04 6405 6420 7c04 6421  d...d...d.d |.d!
+00000190: 6408 9c04 6422 6422 6423 640b 9c03 670b  d...d"d"d#d...g.
+000001a0: 7d05 7c01 7c05 8301 7d06 7c06 a007 6422  }.|.|...}.|...d"
+000001b0: a101 7d07 7c07 73d0 7408 6424 8301 0100  ..}.|.s.t.d$....
+000001c0: 6400 5300 7c06 641b 1900 6400 7501 9001  d.S.|.d...d.u...
+000001d0: 7218 6404 7c06 641b 1900 7601 72fc 6404  r.d.|.d...v.r.d.
+000001e0: 6701 7c06 641b 1900 a201 7c06 641b 3c00  g.|.d.....|.d.<.
+000001f0: 6425 7d08 6426 7c08 9b00 9d02 a009 7c06  d%}.d&|.......|.
+00000200: 641b 1900 a101 7c06 641b 3c00 6427 7d09  d.....|.d.<.d'}.
+00000210: 740a 7c02 7c09 1b00 740b 7c09 8301 6428  t.|.|...t.|...d(
+00000220: 8d02 0100 6429 7d0a 740a 7c02 7c0a 1b00  ....d)}.t.|.|...
+00000230: 740b 7c0a 8301 6a0c 6600 6900 7c06 a401  t.|...j.f.i.|...
+00000240: 8e01 6428 8d02 0100 7c02 642a 1b00 6a0d  ..d(....|.d*..j.
+00000250: 642b 642c 8d01 0100 7c02 642a 1b00 7c06  d+d,....|.d*..|.
+00000260: 6406 1900 1b00 6a0d 642b 642c 8d01 0100  d.....j.d+d,....
+00000270: 7c02 642a 1b00 7c06 6406 1900 1b00 642d  |.d*..|.d.....d-
+00000280: 1b00 7d0b 7c0b a00e a100 9001 73a2 7c0b  ..}.|.......s.|.
+00000290: a00f a100 0100 7c02 642a 1b00 7c06 6406  ......|.d*..|.d.
+000002a0: 1900 1b00 7410 1b00 6a0d 642b 642c 8d01  ....t...j.d+d,..
+000002b0: 0100 7c02 642a 1b00 7c06 6406 1900 1b00  ..|.d*..|.d.....
+000002c0: 7410 1b00 642d 1b00 7d0b 7c0b a00e a100  t...d-..}.|.....
+000002d0: 9001 73e8 7c0b a00f a100 0100 6426 a009  ..s.|.......d&..
+000002e0: 642e 7c03 9b00 642f 9d03 6430 6431 6703  d.|...d/..d0d1g.
+000002f0: a101 7d0c 7408 8300 0100 7411 a008 7412  ..}.t.....t...t.
+00000300: 7c0c 8301 a101 0100 6400 5300 2932 4e72  |.......d.S.)2Nr
+00000310: 0100 0000 2901 da06 7072 6f6d 7074 5a0d  ....)...promptZ.
+00000320: 5049 505f 494e 4445 585f 5552 4cda 00da  PIP_INDEX_URL...
+00000330: 0569 6e70 7574 da07 7072 6f6a 6563 747a  .input..projectz
+00000340: 0c50 726f 6a65 6374 204e 616d 6529 04da  .Project Name)..
+00000350: 0474 7970 65da 046e 616d 65da 0764 6566  .type..name..def
+00000360: 6175 6c74 da07 6d65 7373 6167 655a 0661  ault..messageZ.a
+00000370: 7574 686f 725a 0641 7574 686f 7229 0372  uthorZ.Author).r
+00000380: 0f00 0000 7210 0000 0072 1200 0000 5a0c  ....r....r....Z.
+00000390: 6175 7468 6f72 5f65 6d61 696c 7a0c 4175  author_emailz.Au
+000003a0: 7468 6f72 2045 6d61 696c da0b 6465 7363  thor Email..desc
+000003b0: 7269 7074 696f 6e5a 0b44 6573 6372 6970  riptionZ.Descrip
+000003c0: 7469 6f6e 5a10 6c6f 6e67 5f64 6573 6372  tionZ.long_descr
+000003d0: 6970 7469 6f6e 7a0f 6669 6c65 3a20 5245  iptionz.file: RE
+000003e0: 4144 4d45 2e6d 647a 104c 6f6e 6720 4465  ADME.mdz.Long De
+000003f0: 7363 7269 7074 696f 6eda 086b 6579 776f  scription..keywo
+00000400: 7264 735a 084b 6579 776f 7264 73da 076c  rdsZ.Keywords..l
+00000410: 6963 656e 7365 7a0b 4d49 5420 4c69 6365  icensez.MIT Lice
+00000420: 6e73 655a 074c 6963 656e 7365 5a0f 7079  nseZ.LicenseZ.py
+00000430: 7468 6f6e 5f72 6571 7569 7265 737a 063e  thon_requiresz.>
+00000440: 3d20 332e 387a 0f50 7974 686f 6e20 5265  = 3.8z.Python Re
+00000450: 7175 6972 6573 5a10 696e 7374 616c 6c5f  quiresZ.install_
+00000460: 7265 7175 6972 6573 7a26 496e 7374 616c  requiresz&Instal
+00000470: 6c20 5265 7175 6972 6573 2028 652e 672e  l Requires (e.g.
+00000480: 2c20 7061 6e64 6173 2c20 6e75 6d70 7929  , pandas, numpy)
+00000490: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000004a0: 0004 0000 0053 0000 0073 1400 0000 6401  .....S...s....d.
+000004b0: 6402 8400 7c00 a000 6403 a101 4400 8301  d...|...d...D...
+000004c0: 5300 2904 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+000004d0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+000004e0: 0000 0067 007c 005d 0c7d 017c 01a0 00a1  ...g.|.].}.|....
+000004f0: 0091 0271 0453 00a9 0029 01da 0573 7472  ...q.S...)...str
+00000500: 6970 2902 da02 2e30 da01 5f72 1600 0000  ip)....0.._r....
+00000510: 7216 0000 00fa 372f 686f 6d65 2f65 7567  r.....7/home/eug
+00000520: 656e 652f 7072 6f6a 6563 7473 2f62 6962  ene/projects/bib
+00000530: 6967 6f2f 7372 632f 6269 6269 676f 2f69  igo/src/bibigo/i
+00000540: 6e69 742f 7061 636b 6167 652e 7079 da0a  nit/package.py..
+00000550: 3c6c 6973 7463 6f6d 703e 2700 0000 f300  <listcomp>'.....
+00000560: 0000 007a 3269 6e69 745f 7061 636b 6167  ...z2init_packag
+00000570: 652e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  e.<locals>.<lamb
+00000580: 6461 3e2e 3c6c 6f63 616c 733e 2e3c 6c69  da>.<locals>.<li
+00000590: 7374 636f 6d70 3efa 012c 2901 da05 7370  stcomp>..,)...sp
+000005a0: 6c69 7429 01da 0178 7216 0000 0072 1600  lit)...xr....r..
+000005b0: 0000 721a 0000 00da 083c 6c61 6d62 6461  ..r......<lambda
+000005c0: 3e27 0000 0072 1c00 0000 7a1e 696e 6974  >'...r....z.init
+000005d0: 5f70 6163 6b61 6765 2e3c 6c6f 6361 6c73  _package.<locals
+000005e0: 3e2e 3c6c 616d 6264 613e 2904 720f 0000  >.<lambda>).r...
+000005f0: 0072 1000 0000 7212 0000 00da 0666 696c  .r....r......fil
+00000600: 7465 725a 1064 6570 656e 6465 6e63 795f  terZ.dependency_
+00000610: 6c69 6e6b 737a 1159 6f75 7220 5072 6976  linksz.Your Priv
+00000620: 6174 6520 5079 5049 da07 636f 6e66 6972  ate PyPI..confir
+00000630: 6d7a 1343 6f6e 6669 726d 2049 6e69 7469  mz.Confirm Initi
+00000640: 616c 697a 6572 7a18 5b45 5849 545d 204e  alizerz.[EXIT] N
+00000650: 6f74 6869 6e67 2048 6170 7065 6e65 6421  othing Happened!
+00000660: 7a04 2020 2020 da01 0a7a 0e70 7970 726f  z.    ...z.pypro
+00000670: 6a65 6374 2e74 6f6d 6c29 025a 0664 7374  ject.toml).Z.dst
+00000680: 5f66 70da 0763 6f6e 7465 6e74 7a09 7365  _fp..contentz.se
+00000690: 7475 702e 6366 67da 0373 7263 5429 01da  tup.cfg..srcT)..
+000006a0: 0865 7869 7374 5f6f 6b7a 0b5f 5f69 6e69  .exist_okz.__ini
+000006b0: 745f 5f2e 7079 7a16 5b62 6f6c 645d 5079  t__.pyz.[bold]Py
+000006c0: 7468 6f6e 2070 726f 6a65 6374 2027 7a12  thon project 'z.
+000006d0: 2720 6973 2072 6561 6479 2e5b 2f62 6f6c  ' is ready.[/bol
+000006e0: 645d 7a48 202d 2042 7569 6c64 2050 6163  d]zH - Build Pac
+000006f0: 6b61 6765 3a20 2770 7974 686f 6e20 2d6d  kage: 'python -m
+00000700: 2062 7569 6c64 272c 2070 7974 686f 6e20   build', python 
+00000710: 7061 636b 6167 6520 2762 7569 6c64 2720  package 'build' 
+00000720: 6973 2072 6571 7569 7265 642e 7a4c 202d  is required.zL -
+00000730: 2055 706c 6f61 6420 746f 2050 7950 493a   Upload to PyPI:
+00000740: 2027 7477 696e 6520 7570 6c6f 6164 2064   'twine upload d
+00000750: 6973 742f 2a27 2c20 7079 7468 6f6e 2070  ist/*', python p
+00000760: 6163 6b61 6765 2027 7477 696e 6520 6973  ackage 'twine is
+00000770: 2072 6571 7569 7265 642e 2913 5a0a 5079   required.).Z.Py
+00000780: 496e 7175 6972 6572 720b 0000 0072 0200  Inquirerr....r..
+00000790: 0000 5a08 6162 736f 6c75 7465 7210 0000  ..Z.absoluter...
+000007a0: 00da 026f 73da 0667 6574 656e 76da 0370  ...os..getenv..p
+000007b0: 6f70 da05 7072 696e 74da 046a 6f69 6e72  op..print..joinr
+000007c0: 0700 0000 7206 0000 00da 0666 6f72 6d61  ....r......forma
+000007d0: 74da 056d 6b64 6972 da06 6578 6973 7473  t..mkdir..exists
+000007e0: 5a05 746f 7563 6872 0800 0000 da07 636f  Z.touchr......co
+000007f0: 6e73 6f6c 6572 0400 0000 290d da04 726f  nsoler....)...ro
+00000800: 6f74 720b 0000 00da 0266 7072 0e00 0000  otr......fpr....
+00000810: 5a0c 7072 6976 6174 655f 7079 7069 5a0a  Z.private_pypiZ.
+00000820: 7365 7475 705f 636f 6e66 5a04 636f 6e66  setup_confZ.conf
+00000830: 7222 0000 005a 0354 4142 5a13 5059 5052  r"...Z.TABZ.PYPR
+00000840: 4f4a 4543 545f 544f 4d4c 5f46 494c 455a  OJECT_TOML_FILEZ
+00000850: 0e53 4554 5550 5f43 4647 5f46 494c 455a  .SETUP_CFG_FILEZ
+00000860: 055f 696e 6974 5a07 7375 6d6d 6172 7972  ._initZ.summaryr
+00000870: 1600 0000 7216 0000 0072 1a00 0000 da0c  ....r....r......
+00000880: 696e 6974 5f70 6163 6b61 6765 0f00 0000  init_package....
+00000890: 737a 0000 0000 010c 0308 010a 030e 040c  sz..............
+000008a0: 010a 010a 010a 010c 010a 010c 010c 0202  ................
+000008b0: 0102 0102 0106 fc04 0702 0102 0102 0102  ................
+000008c0: fc04 060a eb04 1908 010a 0104 0108 0104  ................
+000008d0: 030e 010c 0112 0104 0118 0404 0102 0106  ................
+000008e0: 0106 fe06 0604 0102 0106 0112 fe06 0610  ................
+000008f0: 0118 0114 010a 0108 011c 0118 010a 0108  ................
+00000900: 0304 020a 0102 0102 fd02 ff04 0706 0172  ...............r
+00000910: 3200 0000 290d 7227 0000 00da 0770 6174  2...).r'.....pat
+00000920: 686c 6962 7202 0000 005a 0c72 6963 682e  hlibr....Z.rich.
+00000930: 636f 6e73 6f6c 6572 0300 0000 5a0a 7269  consoler....Z.ri
+00000940: 6368 2e70 616e 656c 7204 0000 00da 0575  ch.panelr......u
+00000950: 7469 6c73 7206 0000 0072 0700 0000 7208  tilsr....r....r.
+00000960: 0000 0072 2f00 0000 7232 0000 0072 1600  ...r/...r2...r..
+00000970: 0000 7216 0000 0072 1600 0000 721a 0000  ..r....r....r...
+00000980: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000990: 0c00 0000 0801 0c02 0c01 0c02 1402 0a06  ................
```

### Comparing `bibigo-0.0.5/src/bibigo/init/__pycache__/settings.cpython-39.pyc` & `bibigo-0.0.6/src/bibigo/init/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/init/package.py` & `bibigo-0.0.6/src/bibigo/init/package.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from rich.console import Console
 from rich.panel import Panel
 
-from ..utils import read, write
+from ..utils import read, write, STATIC_DIR
 
 console = Console(width=88)
 
 
 ################################################################
 # init package
 ################################################################
@@ -72,14 +72,25 @@
     # setup.cfg
     SETUP_CFG_FILE = "setup.cfg"
     write(
         dst_fp=fp / SETUP_CFG_FILE,
         content=read(SETUP_CFG_FILE).format(**conf),
     )
 
+    # make src directory
+    (fp / "src").mkdir(exist_ok=True)
+    (fp / "src" / conf["project"]).mkdir(exist_ok=True)
+    _init = fp / "src" / conf["project"] / "__init__.py"
+    if not _init.exists():
+        _init.touch()
+    (fp / "src" / conf["project"] / STATIC_DIR).mkdir(exist_ok=True)
+    _init = fp / "src" / conf["project"] / STATIC_DIR / "__init__.py"
+    if not _init.exists():
+        _init.touch()
+
     # [LOGGING]
     summary = "\n".join(
         [
             f"[bold]Python project '{project}' is ready.[/bold]",
             " - Build Package: 'python -m build', python package 'build' is required.",
             " - Upload to PyPI: 'twine upload dist/*', python package 'twine is required.",
         ]
```

### Comparing `bibigo-0.0.5/src/bibigo/init/settings.py` & `bibigo-0.0.6/src/bibigo/init/settings.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/scripts.py` & `bibigo-0.0.6/src/bibigo/scripts.py`

 * *Files identical despite different names*

### Comparing `bibigo-0.0.5/src/bibigo/utils.py` & `bibigo-0.0.6/src/bibigo/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 from typing import Union
 from pathlib import Path
 import pkgutil
 
+STATIC_DIR = "static"
 
 # ensure path
 def ensure_path(fp: Union[str, Path]):
     return Path(fp)
 
 
 # read file
 def read(fn: Path, version: str = "default"):
-    fp = Path("files") / f"{fn}.{version}"
+    fp = Path(STATIC_DIR) / f"{fn}.{version}"
     content = pkgutil.get_data(__name__, fp.as_posix()).decode()
     return content
 
 
 # make dir if not exist and write file
 def write(dst_fp: Path, content, mode="w"):
     dst_fp = ensure_path(dst_fp)
```

