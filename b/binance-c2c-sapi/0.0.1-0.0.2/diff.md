# Comparing `tmp/binance-c2c-sapi-0.0.1.tar.gz` & `tmp/binance-c2c-sapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sapi-0.0.1.tar", last modified: Sun May 28 18:52:04 2023, max compression
+gzip compressed data, was "binance-c2c-sapi-0.0.2.tar", last modified: Sun May 28 21:04:49 2023, max compression
```

## Comparing `binance-c2c-sapi-0.0.1.tar` & `binance-c2c-sapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:04.614485 binance-c2c-sapi-0.0.1/
--rw-rw-rw-   0        0        0      509 2023-05-28 18:52:04.608561 binance-c2c-sapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:04.550636 binance-c2c-sapi-0.0.1/binance-c2c-sapi/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.1/binance-c2c-sapi/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.1/binance-c2c-sapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:04.608561 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-28 18:52:04.000000 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-28 18:52:04.000000 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:52:04.000000 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-28 18:52:04.000000 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 18:52:04.000000 binance-c2c-sapi-0.0.1/binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 18:52:04.614485 binance-c2c-sapi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-05-28 18:48:11.000000 binance-c2c-sapi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.439718 binance-c2c-sapi-0.0.2/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:04:49.436737 binance-c2c-sapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.411515 binance-c2c-sapi-0.0.2/binance-c2c-sapi/
+-rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-0.0.2/binance-c2c-sapi/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-0.0.2/binance-c2c-sapi/api.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:04:49.433713 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 21:04:49.000000 binance-c2c-sapi-0.0.2/binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:04:49.439718 binance-c2c-sapi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2023-05-28 21:04:46.000000 binance-c2c-sapi-0.0.2/setup.py
```

### Comparing `binance-c2c-sapi-0.0.1/README.md` & `binance-c2c-sapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.1/binance-c2c-sapi/api.py` & `binance-c2c-sapi-0.0.2/binance-c2c-sapi/api.py`

 * *Files identical despite different names*

### Comparing `binance-c2c-sapi-0.0.1/setup.py` & `binance-c2c-sapi-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
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
     name="binance-c2c-sapi",
     version=VERSION,
@@ -23,10 +23,12 @@
     packages=find_packages(),
     install_requires=['requests', 'hashlib', 'hmac', 'json'],
     keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ]
 )
```

