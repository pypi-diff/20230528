# Comparing `tmp/binance-c2c-sdk-0.0.1.tar.gz` & `tmp/binance-c2c-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sdk-0.0.1.tar", last modified: Sun May 28 21:18:23 2023, max compression
+gzip compressed data, was "binance-c2c-sdk-0.0.2.tar", last modified: Sun May 28 21:24:53 2023, max compression
```

## Comparing `binance-c2c-sdk-0.0.1.tar` & `binance-c2c-sdk-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:18:23.538265 binance-c2c-sdk-0.0.1/
--rw-rw-rw-   0        0        0      602 2023-05-28 21:18:23.538265 binance-c2c-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:18:23.505922 binance-c2c-sdk-0.0.1/binance-c2c-sdk/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sdk-0.0.1/binance-c2c-sdk/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sdk-0.0.1/binance-c2c-sdk/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:18:23.535263 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/
--rw-rw-rw-   0        0        0      602 2023-05-28 21:18:23.000000 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-28 21:18:23.000000 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:18:23.000000 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-28 21:18:23.000000 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 21:18:23.000000 binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:18:23.539260 binance-c2c-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-05-28 21:17:50.000000 binance-c2c-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:24:53.286894 binance-c2c-sdk-0.0.2/
+-rw-rw-rw-   0        0        0      602 2023-05-28 21:24:53.283915 binance-c2c-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:24:53.260892 binance-c2c-sdk-0.0.2/binance-c2c-sdk/
+-rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sdk-0.0.2/binance-c2c-sdk/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sdk-0.0.2/binance-c2c-sdk/api.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:24:53.280892 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-05-28 21:24:53.000000 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-28 21:24:53.000000 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:24:53.000000 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-28 21:24:53.000000 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 21:24:53.000000 binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:24:53.286894 binance-c2c-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2023-05-28 21:24:42.000000 binance-c2c-sdk-0.0.2/setup.py
```

### Comparing `binance-c2c-sdk-0.0.1/PKG-INFO` & `binance-c2c-sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sdk-0.0.1/README.md` & `binance-c2c-sdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `binance-c2c-sdk-0.0.1/binance-c2c-sdk/api.py` & `binance-c2c-sdk-0.0.2/binance-c2c-sdk/api.py`

 * *Files identical despite different names*

### Comparing `binance-c2c-sdk-0.0.1/binance_c2c_sdk.egg-info/PKG-INFO` & `binance-c2c-sdk-0.0.2/binance_c2c_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sdk-0.0.1/setup.py` & `binance-c2c-sdk-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="binance-c2c-sdk",
     version=VERSION,
     author="Richard",
     author_email="<rich_swainson@hotmail.co.uk>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'hashlib', 'hmac'],
+    install_requires=['requests', 'hmac'],
     keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

