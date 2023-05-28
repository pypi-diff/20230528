# Comparing `tmp/multicallable-5.0.1.tar.gz` & `tmp/multicallable-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmp88kvdulz/multicallable-5.0.1.tar", last modified: Sat May  6 14:24:34 2023, max compression
+gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmpvy7livpa/multicallable-5.1.0.tar", last modified: Sun May 28 16:00:25 2023, max compression
```

## Comparing `multicallable-5.0.1.tar` & `multicallable-5.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-5.0.1/LICENCE
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-06 14:24:34.000000 multicallable-5.0.1/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3582 2023-02-28 12:46:08.000000 multicallable-5.0.1/README.md
--rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-5.0.1/pyproject.toml
--rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2023-05-06 14:24:34.000000 multicallable-5.0.1/setup.cfg
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      424 2023-05-06 14:22:17.000000 multicallable-5.0.1/src/multicallable/__init__.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable/multicall/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      117 2023-04-04 13:25:46.000000 multicallable-5.0.1/src/multicallable/multicall/__init__.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     7362 2023-05-06 14:21:30.000000 multicallable-5.0.1/src/multicallable/multicall/constants.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4886 2023-04-04 14:00:44.000000 multicallable-5.0.1/src/multicallable/multicall/multicall.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3990 2023-04-04 13:53:09.000000 multicallable-5.0.1/src/multicallable/multicallable.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)      393 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/SOURCES.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/dependency_links.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/top_level.txt
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-28 16:00:25.000000 multicallable-5.1.0/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-5.1.0/LICENCE
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-28 16:00:25.000000 multicallable-5.1.0/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     3582 2023-02-28 12:46:08.000000 multicallable-5.1.0/README.md
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-5.1.0/pyproject.toml
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2023-05-28 16:00:25.000000 multicallable-5.1.0/setup.cfg
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      424 2023-05-28 15:58:33.000000 multicallable-5.1.0/src/multicallable/__init__.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable/multicall/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      117 2023-04-04 13:25:46.000000 multicallable-5.1.0/src/multicallable/multicall/__init__.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     7362 2023-05-06 14:21:30.000000 multicallable-5.1.0/src/multicallable/multicall/constants.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     5059 2023-05-28 15:58:01.000000 multicallable-5.1.0/src/multicallable/multicall/multicall.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4289 2023-05-28 15:58:01.000000 multicallable-5.1.0/src/multicallable/multicallable.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable.egg-info/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable.egg-info/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      393 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable.egg-info/SOURCES.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable.egg-info/dependency_links.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2023-05-28 16:00:25.000000 multicallable-5.1.0/src/multicallable.egg-info/top_level.txt
```

### Comparing `multicallable-5.0.1/LICENCE` & `multicallable-5.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.1/PKG-INFO` & `multicallable-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 5.0.1
+Version: 5.1.0
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multicallable-5.0.1/README.md` & `multicallable-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.1/setup.cfg` & `multicallable-5.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multicallable
-version = 5.0.1
+version = 5.1.0
 author = Hassan Abbasi, Mojtaba Farokhi
 author_email = hassan.abbp@gmail.com
 description = Easy way to work with Multicall package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deusfinance/multicallable
 project_urls =
```

### Comparing `multicallable-5.0.1/src/multicallable/multicall/constants.py` & `multicallable-5.1.0/src/multicallable/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.1/src/multicallable/multicall/multicall.py` & `multicallable-5.1.0/src/multicallable/multicall/multicall.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,31 +112,35 @@
 
         self.contract = w3.eth.contract(address=address, abi=abi)
 
     def call(
             self,
             calls: List[Call],
             require_success: bool = True,
+            block_identifier: str | int = 'latest',
     ) -> list:
         """
         Executes multicall for specified list of smart contracts functions.
 
         Parameters:
             calls: list(tuple)
                 list of Call objets
 
             require_success: bool
                 if true, all calls must return true, otherwise the multicall fails.
 
+            block_identifier: str | int
+                block identifier for web3 call
+
         Returns:
             list of outputs
         """
 
         block_number, block_hash, return_data = self.contract.functions.tryBlockAndAggregate(
-            require_success, [(call.target, call.call_data) for call in calls]).call()
+            require_success, [(call.target, call.call_data) for call in calls]).call(block_identifier=block_identifier)
 
         outputs = []
         for call, result in zip(calls, return_data):
             success, data = result
             if not success or not data:
                 try:
                     error_message = ''.join(chr(c) for c in data[-32:] if c)
```

### Comparing `multicallable-5.0.1/src/multicallable/multicallable.py` & `multicallable-5.1.0/src/multicallable/multicallable.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,38 +29,41 @@
 class Multicallable:
     class Function:
         class FCall:
             def __init__(self, function: 'Multicallable.Function', params: list):
                 self.function = function
                 self.params = params
 
-            def call(self, n: int = 1, require_success: bool = True, progress_bar: bool = False):
+            def call(self, n: int = 1, require_success: bool = True, progress_bar: bool = False,
+                     block_identifier: str | int = 'latest'):
                 mc = self.function.parent._multicall
                 calls = [Call(self.function.parent._target, self.function.name, args) for args in self.params]
                 result = []
                 for i, bucket in enumerate(_split(calls, n)):
                     if progress_bar:
                         percentage = i / n * 100
                         print(f'\r    {bar(percentage)} {i}/{n} buckets    ', end='')
                     if not bucket:
                         continue
-                    block_number, block_hash, outputs = mc.call(bucket, require_success=require_success)
+                    block_number, block_hash, outputs = mc.call(bucket, require_success=require_success,
+                                                                block_identifier=block_identifier)
                     result.extend(outputs)
                 if progress_bar:
                     print(f'\r    {bar(100)} {n}/{n} buckets    ')
                 return result
 
-            def detailed_call(self, n: int = 1, require_success: bool = True):
+            def detailed_call(self, n: int = 1, require_success: bool = True, block_identifier: str | int = 'latest'):
                 mc = self.function.parent._multicall
                 calls = [Call(self.function.parent._target, self.function.name, args) for args in self.params]
                 result = []
                 for bucket in _split(calls, n):
                     if not bucket:
                         continue
-                    block_number, block_hash, outputs = mc.call(bucket, require_success=require_success)
+                    block_number, block_hash, outputs = mc.call(bucket, require_success=require_success,
+                                                                block_identifier=block_identifier)
                     if not result or result[-1]['block_number'] != block_number:
                         result.append(dict(block_number=block_number, result=[]))
                     result[-1]['result'].extend(outputs)
                 return result
 
         def __init__(self, name: str, parent: 'Multicallable'):
             self.name = name
```

### Comparing `multicallable-5.0.1/src/multicallable.egg-info/PKG-INFO` & `multicallable-5.1.0/src/multicallable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 5.0.1
+Version: 5.1.0
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

