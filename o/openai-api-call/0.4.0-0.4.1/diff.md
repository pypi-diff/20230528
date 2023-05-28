# Comparing `tmp/openai_api_call-0.4.0.tar.gz` & `tmp/openai_api_call-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.4.0.tar", last modified: Tue May 16 08:37:08 2023, max compression
+gzip compressed data, was "openai_api_call-0.4.1.tar", last modified: Sun May 28 02:54:32 2023, max compression
```

## Comparing `openai_api_call-0.4.0.tar` & `openai_api_call-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 08:37:08.000000 openai_api_call-0.4.0/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-28 02:54:32.000000 openai_api_call-0.4.1/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 02:54:31.000000 openai_api_call-0.4.1/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 02:54:32.063508 openai_api_call-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-28 02:54:21.000000 openai_api_call-0.4.1/setup.py
```

### Comparing `openai_api_call-0.4.0/LICENSE` & `openai_api_call-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.0/PKG-INFO` & `openai_api_call-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.4.0
+Version: 0.4.1
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -160,14 +160,15 @@
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
+        - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.4.0/README.md` & `openai_api_call-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -151,8 +151,9 @@
 ## License
 
 This package is licensed under the MIT license. See the LICENSE file for more details.
 
 ## update log
 
 - Since version `0.2.0`, `Chat` type is used to handle data
-- Since version `0.3.0`, you can use different API Key to send requests.
+- Since version `0.3.0`, you can use different API Key to send requests.
+- Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
```

### Comparing `openai_api_call-0.4.0/openai_api_call/chattool.py` & `openai_api_call-0.4.1/openai_api_call/chattool.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             path (str): path to the file
             mode (str, optional): mode to open the file. Defaults to 'a'.
             end (str, optional): end of each line. Defaults to '\n'.
         """
         assert mode in ['a', 'w'], "mode should be 'a' or 'w'"
         data = self.chat_log
         with open(path, mode, encoding='utf-8') as f:
-            f.write(json.dumps(data) + end)
+            f.write(json.dumps(data, ensure_ascii=False) + end)
         return True
         
     def print_log(self, sep: Union[str, None]=None):
         """Print the chat log"""
         if sep is None:
             sep = '\n' + '-'*15 + '\n'
         for d in self._chat_log:
```

### Comparing `openai_api_call-0.4.0/openai_api_call/proxy.py` & `openai_api_call-0.4.1/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.0/openai_api_call/request.py` & `openai_api_call-0.4.1/openai_api_call/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         warnings.warn("The `url` parameter is deprecated. Please use `base_url` instead.", DeprecationWarning)
         chat_url = url
     else:
         chat_url = os.path.join(base_url, "v1/chat/completions")
     
     chat_url = normalize_url(chat_url)
     # get response
-    response = requests.post(chat_url, headers=headers, data=json.dumps(payload))
+    response = requests.post(chat_url, headers=headers, data=json.dumps(payload, ensure_ascii=False))
     if response.status_code != 200:
         raise Exception(response.text)
     return response.json()
 
 def usage_status(api_key:str, duration:int=99):
     """Get usage status
```

### Comparing `openai_api_call-0.4.0/openai_api_call/response.py` & `openai_api_call-0.4.1/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.0/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.4.1/openai_api_call.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.4.0
+Version: 0.4.1
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -160,14 +160,15 @@
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
+        - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.4.0/setup.py` & `openai_api_call-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

