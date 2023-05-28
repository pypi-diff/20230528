# Comparing `tmp/binance-c2c-sapi-0.0.3.tar.gz` & `tmp/binance-c2c-sapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sapi-0.0.3.tar", last modified: Sun May 28 21:07:17 2023, max compression
+gzip compressed data, was "binance-c2c-sapi-0.0.4.tar", last modified: Sun May 28 21:14:20 2023, max compression
```

## Comparing `binance-c2c-sapi-0.0.3.tar` & `binance-c2c-sapi-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.989075 binance-c2c-sapi-0.0.3/
--rw-rw-rw-   0        0        0      603 2023-05-28 21:07:17.988075 binance-c2c-sapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.965345 binance-c2c-sapi-0.0.3/binance-c2c-sapi/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.3/binance-c2c-sapi/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.3/binance-c2c-sapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.986076 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:07:17.989075 binance-c2c-sapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-05-28 21:07:15.000000 binance-c2c-sapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:14:20.345113 binance-c2c-sapi-0.0.4/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:14:20.344113 binance-c2c-sapi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:14:20.318538 binance-c2c-sapi-0.0.4/binance-c2c-sapi/
+-rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.4/binance-c2c-sapi/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.4/binance-c2c-sapi/api.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:14:20.343113 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:14:20.000000 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-28 21:14:20.000000 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:14:20.000000 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-28 21:14:20.000000 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 21:14:20.000000 binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:14:20.346113 binance-c2c-sapi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-05-28 21:14:05.000000 binance-c2c-sapi-0.0.4/setup.py
```

### Comparing `binance-c2c-sapi-0.0.3/PKG-INFO` & `binance-c2c-sapi-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sapi-0.0.3/README.md` & `binance-c2c-sapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.3/binance-c2c-sapi/api.py` & `binance-c2c-sapi-0.0.4/binance-c2c-sapi/api.py`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/PKG-INFO` & `binance-c2c-sapi-0.0.4/binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sapi-0.0.3/setup.py` & `binance-c2c-sapi-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="binance-c2c-sapi",
     version=VERSION,
```

