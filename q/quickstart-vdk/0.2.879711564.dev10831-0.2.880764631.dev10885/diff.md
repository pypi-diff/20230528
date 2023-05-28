# Comparing `tmp/quickstart-vdk-0.2.879711564.dev10831.tar.gz` & `tmp/quickstart-vdk-0.2.880764631.dev10885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.879711564.dev10831.tar", last modified: Fri May 26 04:24:31 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.880764631.dev10885.tar", last modified: Sat May 27 04:23:32 2023, max compression
```

## Comparing `quickstart-vdk-0.2.879711564.dev10831.tar` & `quickstart-vdk-0.2.880764631.dev10885.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 04:24:31.305800 quickstart-vdk-0.2.879711564.dev10831/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-26 04:24:31.305800 quickstart-vdk-0.2.879711564.dev10831/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-26 04:21:46.000000 quickstart-vdk-0.2.879711564.dev10831/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 04:24:31.305800 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-26 04:24:31.000000 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-26 04:24:31.000000 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 04:24:31.000000 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-26 04:24:31.000000 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-26 04:24:31.000000 quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 04:24:31.305800 quickstart-vdk-0.2.879711564.dev10831/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-26 04:24:20.000000 quickstart-vdk-0.2.879711564.dev10831/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 04:24:31.305800 quickstart-vdk-0.2.879711564.dev10831/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-26 04:21:46.000000 quickstart-vdk-0.2.879711564.dev10831/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 04:23:32.655409 quickstart-vdk-0.2.880764631.dev10885/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-27 04:23:32.655409 quickstart-vdk-0.2.880764631.dev10885/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-27 04:20:45.000000 quickstart-vdk-0.2.880764631.dev10885/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 04:23:32.655409 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-27 04:23:32.000000 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-27 04:23:32.000000 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 04:23:32.000000 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-27 04:23:32.000000 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-27 04:23:32.000000 quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 04:23:32.655409 quickstart-vdk-0.2.880764631.dev10885/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-27 04:23:22.000000 quickstart-vdk-0.2.880764631.dev10885/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 04:23:32.655409 quickstart-vdk-0.2.880764631.dev10885/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-27 04:20:45.000000 quickstart-vdk-0.2.880764631.dev10885/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.879711564.dev10831/PKG-INFO` & `quickstart-vdk-0.2.880764631.dev10885/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.879711564.dev10831
+Version: 0.2.880764631.dev10885
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.879711564.dev10831/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.880764631.dev10885/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.879711564.dev10831
+Version: 0.2.880764631.dev10885
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.879711564.dev10831/setup.py` & `quickstart-vdk-0.2.880764631.dev10885/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.879711564.dev10831"
+__version__ = "0.2.880764631.dev10885"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

