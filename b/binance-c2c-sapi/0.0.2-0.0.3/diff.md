# Comparing `tmp/binance-c2c-sapi-0.0.2.tar.gz` & `tmp/binance-c2c-sapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sapi-0.0.2.tar", last modified: Sun May 28 21:04:49 2023, max compression
+gzip compressed data, was "binance-c2c-sapi-0.0.3.tar", last modified: Sun May 28 21:07:17 2023, max compression
```

## Comparing `binance-c2c-sapi-0.0.2.tar` & `binance-c2c-sapi-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.439718 binance-c2c-sapi-0.0.2/
--rw-rw-rw-   0        0        0      603 2023-05-28 21:04:49.436737 binance-c2c-sapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.411515 binance-c2c-sapi-0.0.2/binance-c2c-sapi/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.2/binance-c2c-sapi/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.2/binance-c2c-sapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.433713 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:04:49.439718 binance-c2c-sapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1136 2023-05-28 21:04:46.000000 binance-c2c-sapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.989075 binance-c2c-sapi-0.0.3/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:07:17.988075 binance-c2c-sapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.965345 binance-c2c-sapi-0.0.3/binance-c2c-sapi/
+-rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.3/binance-c2c-sapi/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.3/binance-c2c-sapi/api.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:07:17.986076 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 21:07:17.000000 binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:07:17.989075 binance-c2c-sapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-05-28 21:07:15.000000 binance-c2c-sapi-0.0.3/setup.py
```

### Comparing `binance-c2c-sapi-0.0.2/PKG-INFO` & `binance-c2c-sapi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sapi-0.0.2/README.md` & `binance-c2c-sapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.2/binance-c2c-sapi/api.py` & `binance-c2c-sapi-0.0.3/binance-c2c-sapi/api.py`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/PKG-INFO` & `binance-c2c-sapi-0.0.3/binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-c2c-sapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binance-c2c-sapi-0.0.2/setup.py` & `binance-c2c-sapi-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="binance-c2c-sapi",
     version=VERSION,
     author="Richard",
     author_email="<rich_swainson@hotmail.co.uk>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'hashlib', 'hmac', 'json'],
+    install_requires=['requests', 'hashlib', 'hmac'],
     keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

