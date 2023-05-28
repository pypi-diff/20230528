# Comparing `tmp/chatapi-translate-0.6.tar.gz` & `tmp/chatapi-translate-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatapi-translate-0.6.tar", last modified: Mon May 15 04:09:41 2023, max compression
+gzip compressed data, was "chatapi-translate-0.7.tar", last modified: Sun May 28 09:19:53 2023, max compression
```

## Comparing `chatapi-translate-0.6.tar` & `chatapi-translate-0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 04:09:41.220732 chatapi-translate-0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.6/chatapi_translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7957 2023-05-15 04:06:56.000000 chatapi-translate-0.6/chatapi_translate/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate/translator/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.6/chatapi_translate/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.6/chatapi_translate/translator/ali.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.6/chatapi_translate/translator/baidu.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.6/chatapi_translate/translator/caiyun.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.6/chatapi_translate/translator/chatgpt.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.6/chatapi_translate/translator/deepl.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.6/chatapi_translate/translator/google.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.6/chatapi_translate/translator/tencent.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.6/chatapi_translate/translator/utils.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.6/chatapi_translate/translator/volcengine.py
--rw-r--r--   0 root         (0) root         (0)     6962 2023-05-15 04:02:32.000000 chatapi-translate-0.6/chatapi_translate/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 04:09:41.220732 chatapi-translate-0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1305 2023-05-15 03:45:22.000000 chatapi-translate-0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 09:19:53.332135 chatapi-translate-0.7/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-28 09:19:53.332135 chatapi-translate-0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 09:19:53.328135 chatapi-translate-0.7/chatapi_translate/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.7/chatapi_translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2023-05-28 05:23:14.000000 chatapi-translate-0.7/chatapi_translate/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 09:19:53.332135 chatapi-translate-0.7/chatapi_translate/translator/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.7/chatapi_translate/translator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.7/chatapi_translate/translator/ali.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.7/chatapi_translate/translator/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.7/chatapi_translate/translator/caiyun.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.7/chatapi_translate/translator/chatgpt.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.7/chatapi_translate/translator/deepl.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.7/chatapi_translate/translator/google.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.7/chatapi_translate/translator/tencent.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.7/chatapi_translate/translator/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.7/chatapi_translate/translator/volcengine.py
+-rw-r--r--   0 root         (0) root         (0)     6962 2023-05-15 04:02:32.000000 chatapi-translate-0.7/chatapi_translate/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 09:19:53.332135 chatapi-translate-0.7/chatapi_translate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-28 09:19:53.000000 chatapi-translate-0.7/chatapi_translate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 09:19:53.332135 chatapi-translate-0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-28 05:22:47.000000 chatapi-translate-0.7/setup.py
```

### Comparing `chatapi-translate-0.6/LICENSE` & `chatapi-translate-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/PKG-INFO` & `chatapi-translate-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.6
+Version: 0.7
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.6/chatapi_translate/api.py` & `chatapi-translate-0.7/chatapi_translate/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         try:
             if 'messages' in body:
                 body["messages"] = filter_messages_and_trigger(body["messages"])
             if 'stream' in body and body["stream"]:
                 client_stream = client.stream("POST", url, headers=headers, json=body, timeout=360)
                 return EventSourceResponse(response_stream(client_stream), ping=10000)
             else:
-                response = await client.post(url, headers=headers, json=body)
+                response = await client.post(url, headers=headers, json=body, timeout=120)
                 return Response(
                     response.content,
                     status_code=response.status_code,
                     headers=dict(response.headers),
                     media_type=response.headers.get("Content-Type"),
                 )
         except Exception as e:
@@ -170,8 +170,12 @@
     parser.add_argument('--config', type=str, default='config.jsonc',
                         help='configuration file path, content format reference: https://github.com/aitsc/chatapi-translate/blob/master/config_example.jsonc')
     args = parser.parse_args()
     if not os.path.exists(args.config):
         print('需要用 --config 命令行参数指定存在的配置文件路径!\n样例模版请参考: https://github.com/aitsc/chatapi-translate/blob/master/config_example.jsonc')
         return
     get_global_config(args.config)
-    uvicorn.run(app, host=args.host, port=args.port)
+    
+    log_config = uvicorn.config.LOGGING_CONFIG
+    log_config["formatters"]["access"]["fmt"] = "%(asctime)s - %(levelname)s - %(message)s"
+    log_config["formatters"]["default"]["fmt"] = "%(asctime)s - %(levelname)s - %(message)s"
+    uvicorn.run(app, host=args.host, port=args.port, log_config=log_config)
```

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/__init__.py` & `chatapi-translate-0.7/chatapi_translate/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/ali.py` & `chatapi-translate-0.7/chatapi_translate/translator/ali.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/baidu.py` & `chatapi-translate-0.7/chatapi_translate/translator/baidu.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/caiyun.py` & `chatapi-translate-0.7/chatapi_translate/translator/caiyun.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/chatgpt.py` & `chatapi-translate-0.7/chatapi_translate/translator/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/deepl.py` & `chatapi-translate-0.7/chatapi_translate/translator/deepl.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/google.py` & `chatapi-translate-0.7/chatapi_translate/translator/google.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/tencent.py` & `chatapi-translate-0.7/chatapi_translate/translator/tencent.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/utils.py` & `chatapi-translate-0.7/chatapi_translate/translator/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/translator/volcengine.py` & `chatapi-translate-0.7/chatapi_translate/translator/volcengine.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate/utils.py` & `chatapi-translate-0.7/chatapi_translate/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/chatapi_translate.egg-info/PKG-INFO` & `chatapi-translate-0.7/chatapi_translate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.6
+Version: 0.7
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.6/chatapi_translate.egg-info/SOURCES.txt` & `chatapi-translate-0.7/chatapi_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.6/setup.py` & `chatapi-translate-0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'code: https://github.com/aitsc/chatapi-translate'
 
 setup(
     name='chatapi-translate',
-    version='0.6',
+    version='0.7',
     description="ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='MIT',
     url='https://github.com/aitsc/chatapi-translate',
     keywords='tools',
```

