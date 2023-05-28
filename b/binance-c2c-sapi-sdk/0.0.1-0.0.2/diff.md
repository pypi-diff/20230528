# Comparing `tmp/binance-c2c-sapi-sdk-0.0.1.tar.gz` & `tmp/binance-c2c-sapi-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sapi-sdk-0.0.1.tar", last modified: Sun May 28 21:26:54 2023, max compression
+gzip compressed data, was "binance-c2c-sapi-sdk-0.0.2.tar", last modified: Sun May 28 21:29:35 2023, max compression
```

## Comparing `binance-c2c-sapi-sdk-0.0.1.tar` & `binance-c2c-sapi-sdk-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:26:54.078888 binance-c2c-sapi-sdk-0.0.1/
--rw-rw-rw-   0        0        0      607 2023-05-28 21:26:54.077889 binance-c2c-sapi-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:26:54.039354 binance-c2c-sapi-sdk-0.0.1/binance-c2c-sapi-sdk/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-sdk-0.0.1/binance-c2c-sapi-sdk/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-sdk-0.0.1/binance-c2c-sapi-sdk/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:26:54.075830 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/
--rw-rw-rw-   0        0        0      607 2023-05-28 21:26:53.000000 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-28 21:26:53.000000 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:26:53.000000 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-28 21:26:53.000000 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-28 21:26:53.000000 binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:26:54.079890 binance-c2c-sapi-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-05-28 21:26:49.000000 binance-c2c-sapi-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:35.574504 binance-c2c-sapi-sdk-0.0.2/
+-rw-rw-rw-   0        0        0      607 2023-05-28 21:29:35.573507 binance-c2c-sapi-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:35.543508 binance-c2c-sapi-sdk-0.0.2/binance-c2c-sapi-sdk/
+-rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-sdk-0.0.2/binance-c2c-sapi-sdk/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-sdk-0.0.2/binance-c2c-sapi-sdk/api.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:29:35.571509 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/
+-rw-rw-rw-   0        0        0      607 2023-05-28 21:29:35.000000 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-28 21:29:35.000000 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:29:35.000000 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 21:29:35.000000 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-28 21:29:35.000000 binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:29:35.574504 binance-c2c-sapi-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-05-28 21:29:23.000000 binance-c2c-sapi-sdk-0.0.2/setup.py
```

### Comparing `binance-c2c-sapi-sdk-0.0.1/PKG-INFO` & `binance-c2c-sapi-sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi-sdk
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

### Comparing `binance-c2c-sapi-sdk-0.0.1/README.md` & `binance-c2c-sapi-sdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-sdk-0.0.1/binance-c2c-sapi-sdk/api.py` & `binance-c2c-sapi-sdk-0.0.2/binance-c2c-sapi-sdk/api.py`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-sdk-0.0.1/binance_c2c_sapi_sdk.egg-info/PKG-INFO` & `binance-c2c-sapi-sdk-0.0.2/binance_c2c_sapi_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi-sdk
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

### Comparing `binance-c2c-sapi-sdk-0.0.1/setup.py` & `binance-c2c-sapi-sdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

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
     name="binance-c2c-sapi-sdk",
     version=VERSION,
     author="Richard",
     author_email="<rich_swainson@hotmail.co.uk>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'hmac'],
+    install_requires=['requests'],
     keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

