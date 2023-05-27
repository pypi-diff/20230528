# Comparing `tmp/easybuild-4.7.1.tar.gz` & `tmp/easybuild-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybuild-4.7.1.tar", last modified: Mon Mar 20 10:26:31 2023, max compression
+gzip compressed data, was "easybuild-4.7.2.tar", last modified: Sat May 27 22:42:54 2023, max compression
```

## Comparing `easybuild-4.7.1.tar` & `easybuild-4.7.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-03-20 10:26:31.231342 easybuild-4.7.1/
--rw-r--r--   0 kehoste    (501) staff       (20)    18092 2022-10-21 08:06:35.751435 easybuild-4.7.1/LICENSE
--rw-r--r--   0 kehoste    (501) staff       (20)     6905 2023-03-20 10:26:31.231402 easybuild-4.7.1/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)     4538 2023-03-20 09:56:24.940586 easybuild-4.7.1/README.rst
--rw-r--r--   0 kehoste    (501) staff       (20)       31 2022-10-21 08:06:35.795029 easybuild-4.7.1/setup.cfg
--rw-r--r--   0 kehoste    (501) staff       (20)     3502 2023-03-20 10:26:22.824225 easybuild-4.7.1/setup.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-05-27 22:42:54.360526 easybuild-4.7.2/
+-rw-r--r--   0 kehoste    (501) staff       (20)    18092 2022-10-21 08:06:35.751435 easybuild-4.7.2/LICENSE
+-rw-r--r--   0 kehoste    (501) staff       (20)     6905 2023-05-27 22:42:54.360596 easybuild-4.7.2/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)     4538 2023-03-20 09:56:24.940586 easybuild-4.7.2/README.rst
+-rw-r--r--   0 kehoste    (501) staff       (20)       31 2022-10-21 08:06:35.795029 easybuild-4.7.2/setup.cfg
+-rw-r--r--   0 kehoste    (501) staff       (20)     3502 2023-05-27 20:13:43.295451 easybuild-4.7.2/setup.py
```

### Comparing `easybuild-4.7.1/LICENSE` & `easybuild-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easybuild-4.7.1/PKG-INFO` & `easybuild-4.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: easybuild
-Version: 4.7.1
+Version: 4.7.2
 Summary: EasyBuild is a software build and installation framework that allows you to manage (scientific) software on High Performance Computing (HPC) systems in an efficient way.
 Home-page: https://easybuild.io
 Author: EasyBuild community
 Author-email: easybuild@lists.ugent.be
 License: GPLv2
 Description: .. image:: https://github.com/easybuilders/easybuild/raw/develop/logo/png/easybuild_logo_2022_horizontal_dark_bg_transparent.png
            :align: center
@@ -136,10 +136,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
-Requires: easybuild_framework(==4.7.1)
-Requires: easybuild_easyblocks(==4.7.1)
-Requires: easybuild_easyconfigs(==4.7.1)
+Requires: easybuild_framework(==4.7.2)
+Requires: easybuild_easyblocks(==4.7.2)
+Requires: easybuild_easyconfigs(==4.7.2)
```

### Comparing `easybuild-4.7.1/README.rst` & `easybuild-4.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `easybuild-4.7.1/setup.py` & `easybuild-4.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 import os
 from distutils import log
 from distutils.core import setup
 
 # note: release candidates should be versioned as a pre-release, e.g. "1.1rc1"
 # 1.1-rc1 would indicate a post-release, i.e., and update of 1.1, so beware
-VERSION = '4.7.1'
+VERSION = '4.7.2'
 
 
 # Utility function to read README file
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
```

