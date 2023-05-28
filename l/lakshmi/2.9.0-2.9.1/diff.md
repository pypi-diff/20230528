# Comparing `tmp/lakshmi-2.9.0.tar.gz` & `tmp/lakshmi-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakshmi-2.9.0.tar", last modified: Tue Jan 31 03:10:00 2023, max compression
+gzip compressed data, was "lakshmi-2.9.1.tar", last modified: Sat Feb 11 03:06:35 2023, max compression
```

## Comparing `lakshmi-2.9.0.tar` & `lakshmi-2.9.1.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-01-31 03:10:00.168512 lakshmi-2.9.0/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2021-11-11 08:03:29.000000 lakshmi-2.9.0/LICENSE
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       23 2021-11-11 08:03:29.000000 lakshmi-2.9.0/MANIFEST.in
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    11606 2023-01-31 03:10:00.168512 lakshmi-2.9.0/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10800 2023-01-31 03:09:23.000000 lakshmi-2.9.0/README.md
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-01-31 03:10:00.168512 lakshmi-2.9.0/lakshmi/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       68 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/__init__.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    25907 2022-09-29 03:30:58.000000 lakshmi-2.9.0/lakshmi/analyze.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    27862 2023-01-31 03:09:23.000000 lakshmi-2.9.0/lakshmi/assets.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10390 2022-06-22 04:24:57.000000 lakshmi-2.9.0/lakshmi/cache.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       61 2023-01-31 03:09:38.000000 lakshmi-2.9.0/lakshmi/constants.py
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-01-31 03:10:00.168512 lakshmi-2.9.0/lakshmi/data/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      372 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/Account.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      533 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/AssetClass.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      246 2022-01-26 04:42:26.000000 lakshmi-2.9.0/lakshmi/data/Checkpoint.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      493 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/EEBonds.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      490 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/IBonds.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      367 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/ManualAsset.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      544 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/TickerAsset.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      678 2021-11-11 08:03:29.000000 lakshmi-2.9.0/lakshmi/data/VanguardFund.yaml
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    35679 2023-01-31 03:09:23.000000 lakshmi-2.9.0/lakshmi/lak.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    39373 2023-01-31 03:09:23.000000 lakshmi-2.9.0/lakshmi/lakshmi.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    18204 2022-09-29 03:30:58.000000 lakshmi-2.9.0/lakshmi/performance.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     4226 2022-04-24 16:28:38.000000 lakshmi-2.9.0/lakshmi/table.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1058 2022-10-02 05:49:45.000000 lakshmi-2.9.0/lakshmi/utils.py
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-01-31 03:10:00.168512 lakshmi-2.9.0/lakshmi.egg-info/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    11606 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      638 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/SOURCES.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/dependency_links.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       40 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/entry_points.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      102 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/requires.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        8 2023-01-31 03:10:00.000000 lakshmi-2.9.0/lakshmi.egg-info/top_level.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-01-31 03:10:00.168512 lakshmi-2.9.0/setup.cfg
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1462 2023-01-31 03:09:23.000000 lakshmi-2.9.0/setup.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-02-11 03:06:35.921782 lakshmi-2.9.1/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2021-11-11 08:03:29.000000 lakshmi-2.9.1/LICENSE
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       23 2021-11-11 08:03:29.000000 lakshmi-2.9.1/MANIFEST.in
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    11606 2023-02-11 03:06:35.921782 lakshmi-2.9.1/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10800 2023-01-31 03:09:23.000000 lakshmi-2.9.1/README.md
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-02-11 03:06:35.918449 lakshmi-2.9.1/lakshmi/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       68 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/__init__.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    25907 2022-09-29 03:30:58.000000 lakshmi-2.9.1/lakshmi/analyze.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    27925 2023-02-11 03:04:38.000000 lakshmi-2.9.1/lakshmi/assets.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10390 2022-06-22 04:24:57.000000 lakshmi-2.9.1/lakshmi/cache.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       61 2023-02-11 03:04:38.000000 lakshmi-2.9.1/lakshmi/constants.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-02-11 03:06:35.918449 lakshmi-2.9.1/lakshmi/data/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      372 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/Account.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      533 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/AssetClass.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      246 2022-01-26 04:42:26.000000 lakshmi-2.9.1/lakshmi/data/Checkpoint.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      493 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/EEBonds.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      490 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/IBonds.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      367 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/ManualAsset.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      544 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/TickerAsset.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      678 2021-11-11 08:03:29.000000 lakshmi-2.9.1/lakshmi/data/VanguardFund.yaml
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    35679 2023-02-11 03:06:23.000000 lakshmi-2.9.1/lakshmi/lak.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    39373 2023-01-31 03:09:23.000000 lakshmi-2.9.1/lakshmi/lakshmi.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    18204 2022-09-29 03:30:58.000000 lakshmi-2.9.1/lakshmi/performance.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     4226 2022-04-24 16:28:38.000000 lakshmi-2.9.1/lakshmi/table.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1058 2022-10-02 05:49:45.000000 lakshmi-2.9.1/lakshmi/utils.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-02-11 03:06:35.918449 lakshmi-2.9.1/lakshmi.egg-info/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    11606 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      826 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       40 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/entry_points.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      103 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/requires.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        8 2023-02-11 03:06:35.000000 lakshmi-2.9.1/lakshmi.egg-info/top_level.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-02-11 03:06:35.921782 lakshmi-2.9.1/setup.cfg
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1463 2023-02-11 03:04:38.000000 lakshmi-2.9.1/setup.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-02-11 03:06:35.921782 lakshmi-2.9.1/tests/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    27970 2022-07-23 16:20:27.000000 lakshmi-2.9.1/tests/test_analyze.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    13555 2023-02-11 03:04:38.000000 lakshmi-2.9.1/tests/test_assets.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10773 2022-06-22 04:24:57.000000 lakshmi-2.9.1/tests/test_cache.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     2189 2022-01-26 04:42:26.000000 lakshmi-2.9.1/tests/test_data.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    22866 2023-01-31 03:09:23.000000 lakshmi-2.9.1/tests/test_lak.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    35049 2023-01-31 03:09:23.000000 lakshmi-2.9.1/tests/test_lakshmi.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)    10287 2022-04-24 16:28:38.000000 lakshmi-2.9.1/tests/test_performance.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     2781 2022-04-24 16:28:38.000000 lakshmi-2.9.1/tests/test_table.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      940 2022-01-26 04:42:26.000000 lakshmi-2.9.1/tests/test_utils.py
```

### Comparing `lakshmi-2.9.0/LICENSE` & `lakshmi-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/PKG-INFO` & `lakshmi-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakshmi
-Version: 2.9.0
+Version: 2.9.1
 Summary: Investing library and command-line interface inspired by the Bogleheads philosophy
 Home-page: https://github.com/sarvjeets/lakshmi
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lakshmi-2.9.0/README.md` & `lakshmi-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/analyze.py` & `lakshmi-2.9.1/lakshmi/analyze.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/assets.py` & `lakshmi-2.9.1/lakshmi/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,15 +531,16 @@
 
         The return price is cached for a day.
 
         Returns: Price (float).
 
         Raises: NotFoundError if the ticker is not found.
         """
-        price = self.yticker.fast_info.get('last_price', None)
+        price = self.yticker.fast_info.get('lastPrice', None) or \
+            self.yticker.fast_info.get('last_price', None)
         if price is None:
             raise NotFoundError(
                 f'Cannot retrieve ticker ("{self._ticker}") '
                 'from Yahoo Finance')
         return price
 
     def prefetch_add(self):
```

### Comparing `lakshmi-2.9.0/lakshmi/cache.py` & `lakshmi-2.9.1/lakshmi/cache.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/data/AssetClass.yaml` & `lakshmi-2.9.1/lakshmi/data/AssetClass.yaml`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/data/TickerAsset.yaml` & `lakshmi-2.9.1/lakshmi/data/TickerAsset.yaml`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/data/VanguardFund.yaml` & `lakshmi-2.9.1/lakshmi/data/VanguardFund.yaml`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/lak.py` & `lakshmi-2.9.1/lakshmi/lak.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/lakshmi.py` & `lakshmi-2.9.1/lakshmi/lakshmi.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/performance.py` & `lakshmi-2.9.1/lakshmi/performance.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/table.py` & `lakshmi-2.9.1/lakshmi/table.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi/utils.py` & `lakshmi-2.9.1/lakshmi/utils.py`

 * *Files identical despite different names*

### Comparing `lakshmi-2.9.0/lakshmi.egg-info/PKG-INFO` & `lakshmi-2.9.1/lakshmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakshmi
-Version: 2.9.0
+Version: 2.9.1
 Summary: Investing library and command-line interface inspired by the Bogleheads philosophy
 Home-page: https://github.com/sarvjeets/lakshmi
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lakshmi-2.9.0/setup.py` & `lakshmi-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     install_requires=[
         'click~=8.0',
         'numpy~=1.22',
         'pyxirr~=0.6',
         'PyYAML>=5.4,<7.0',
         'requests~=2.25',
         'tabulate~=0.8',
-        'yfinance>=0.2.9,<0.3',
+        'yfinance>=0.2.11,<0.3',
     ],
     entry_points={
         'console_scripts': [
             'lak = lakshmi.lak:lak',
         ],
     },
     test_suite='tests',
```

