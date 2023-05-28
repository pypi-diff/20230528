# Comparing `tmp/revChatGPT-5.3.0.tar.gz` & `tmp/revChatGPT-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.3.0.tar", last modified: Sun May 28 11:41:32 2023, max compression
+gzip compressed data, was "revChatGPT-5.3.1.tar", last modified: Sun May 28 11:46:07 2023, max compression
```

## Comparing `revChatGPT-5.3.0.tar` & `revChatGPT-5.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.178158 revChatGPT-5.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.178158 revChatGPT-5.3.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    53601 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    53960 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/tests/test_recipient.py
```

### Comparing `revChatGPT-5.3.0/LICENSE` & `revChatGPT-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/PKG-INFO` & `revChatGPT-5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.0
+Version: 5.3.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-5.3.0/README.md` & `revChatGPT-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/setup.py` & `revChatGPT-5.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.3.0",
+    version="5.3.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
@@ -32,15 +32,15 @@
         "OpenAIAuth>=1.0.2",
         "requests[socks]",
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
-        "curl_cffi"
+        "curl_cffi",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `revChatGPT-5.3.0/src/revChatGPT/V1.py` & `revChatGPT-5.3.1/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 
 import base64
 import binascii
 import contextlib
 import datetime
 import json
 import logging
+import tempfile
 import time
 import uuid
-import tempfile
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
-
 import httpx
 from curl_cffi import requests
 from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
 from .recipient import PythonRecipient
@@ -77,15 +76,17 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/" # "https://chat.openai.com/backend-api/"
+BASE_URL = (
+    environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
+)  # "https://chat.openai.com/backend-api/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
@@ -164,17 +165,22 @@
         self.lazy_loading = lazy_loading
         self.recipients = RecipientManager()
         self.disable_history = config.get("disable_history", False)
 
         self.__check_credentials()
         # Check if chat.openai.com is reachable
         if not base_url:
-            response = self.session.get("https://chat.openai.com/backend-api/accounts/check", impersonate='safari15_5')
+            response = self.session.get(
+                "https://chat.openai.com/backend-api/accounts/check",
+                impersonate="safari15_5",
+            )
             if response.status_code != 200:
-                print(f"Using bypass.churchless.tech backend due to status code {response.status_code}")
+                print(
+                    f"Using bypass.churchless.tech backend due to status code {response.status_code}"
+                )
                 self.base_url = BASE_URL
             else:
                 print("Using chat.openai.com backend")
                 self.base_url = "https://chat.openai.com/backend-api/"
         else:
             self.base_url = base_url
 
@@ -211,15 +217,15 @@
         """
         self.session.headers.clear()
         self.session.headers.update(
             {
                 "Accept": "text/event-stream",
                 "Authorization": f"Bearer {access_token}",
                 "Content-Type": "application/json",
-                "User-Agent": "OpenAI-API-Client/0.1.0",
+                "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
             },
         )
 
         self.config["access_token"] = access_token
 
         email = self.config.get("email", None)
         if email is not None:
@@ -351,16 +357,16 @@
         conversation_stream = self.handle_conversation_stream(step=1)
 
         with open(conversation_stream.name, "wb") as response_file:
             response = self.session.post(
                 url=f"{self.base_url}conversation",
                 data=json.dumps(data),
                 timeout=timeout,
-                impersonate='safari15_5',
-                content_callback=response_file.write, # a hack around curl_cffi not supporting stream=True
+                impersonate="safari15_5",
+                content_callback=response_file.write,  # a hack around curl_cffi not supporting stream=True
             )
         self.__check_response(response)
 
         finish_details = None
 
         response_lst = self.handle_conversation_stream(file=conversation_stream, step=2)
 
@@ -699,30 +705,30 @@
     ) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = self.session.get(url, impersonate='safari15_5')
+        response = self.session.get(url, impersonate="safari15_5")
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         data = json.loads(response.text)
         return data["items"]
 
     @logger(is_timed=True)
     def get_msg_history(self, convo_id: str, encoding: str | None = None) -> list:
         """
         Get message history
         :param id: UUID of conversation
         :param encoding: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.get(url, impersonate='safari15_5')
+        response = self.session.get(url, impersonate="safari15_5")
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
@@ -730,47 +736,53 @@
         Generate title for conversation
         """
         response = self.session.post(
             f"{self.base_url}conversation/gen_title/{convo_id}",
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
             ),
-            impersonate='safari15_5'
+            impersonate="safari15_5",
         )
         self.__check_response(response)
         return response.json().get("title", "Error generating title")
 
     @logger(is_timed=True)
     def change_title(self, convo_id: str, title: str) -> None:
         """
         Change title of conversation
         :param id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.patch(url, data=json.dumps({"title": title}), impersonate='safari15_5')
+        response = self.session.patch(
+            url, data=json.dumps({"title": title}), impersonate="safari15_5"
+        )
         self.__check_response(response)
 
     @logger(is_timed=True)
     def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
+        response = self.session.patch(
+            url, data='{"is_visible": false}', impersonate="safari15_5"
+        )
         self.__check_response(response)
 
     @logger(is_timed=True)
     def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
+        response = self.session.patch(
+            url, data='{"is_visible": false}', impersonate="safari15_5"
+        )
         self.__check_response(response)
 
     @logger(is_timed=False)
     def __map_conversations(self) -> None:
         conversations = self.get_conversations()
         histories = [self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
@@ -796,37 +808,40 @@
         for _ in range(num):
             self.conversation_id = self.conversation_id_prev_queue.pop()
             self.parent_id = self.parent_id_prev_queue.pop()
 
     @logger(is_timed=True)
     def get_plugins(self, offset: int = 0, limit: int = 250, status: str = "approved"):
         url = f"{self.base_url}aip/p?offset={offset}&limit={limit}&statuses={status}"
-        response = self.session.get(url, impersonate='safari15_5')
+        response = self.session.get(url, impersonate="safari15_5")
         self.__check_response(response)
         # Parse as JSON
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def install_plugin(self, plugin_id: str):
         url = f"{self.base_url}aip/p/{plugin_id}/user-settings"
         payload = {"is_installed": True}
-        response = self.session.patch(url, data=json.dumps(payload), impersonate='safari15_5')
+        response = self.session.patch(
+            url, data=json.dumps(payload), impersonate="safari15_5"
+        )
         self.__check_response(response)
 
     @logger(is_timed=False)
-    def handle_conversation_stream(self, file = None, step: int = 1):
-        if step == 1: 
+    def handle_conversation_stream(self, file=None, step: int = 1):
+        if step == 1:
             return tempfile.NamedTemporaryFile(delete=False)
         elif step == 2 and file:
-            with open(file.name, "r") as response_file:
+            with open(file.name) as response_file:
                 response_lst = response_file.read().splitlines()
             file.close()
             Path(file.name).unlink()
             return response_lst
 
+
 class AsyncChatbot(Chatbot):
     """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
         conversation_id: str | None = None,
@@ -867,20 +882,22 @@
 
         async with self.session as s:
             with open(conversation_stream.name, "wb") as response_file:
                 response = await s.post(
                     url=f"{self.base_url}conversation",
                     data=json.dumps(data),
                     timeout=timeout,
-                    impersonate='safari15_5',
+                    impersonate="safari15_5",
                     content_callback=response_file.write,
-                    )
+                )
             await self.__check_response(response)
 
-            response_lst = self.handle_conversation_stream(file=conversation_stream, step=2)
+            response_lst = self.handle_conversation_stream(
+                file=conversation_stream, step=2
+            )
 
             for line in response_lst:
                 if line.lower() == "internal server error":
                     log.error(f"Internal Server Error: {line}")
                     error = t.Error(
                         source="ask",
                         message="Internal Server Error",
@@ -1144,30 +1161,30 @@
     async def get_conversations(self, offset: int = 0, limit: int = 20) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = await self.session.get(url, impersonate='safari15_5')
+        response = await self.session.get(url, impersonate="safari15_5")
         await self.__check_response(response)
         data = json.loads(response.text)
         return data["items"]
 
     async def get_msg_history(
         self,
         convo_id: str,
         encoding: str | None = "utf-8",
     ) -> dict:
         """
         Get message history
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.get(url, impersonate='safari15_5')
+        response = await self.session.get(url, impersonate="safari15_5")
         if encoding is not None:
             response.encoding = encoding
             await self.__check_response(response)
             return json.loads(response.text)
         return None
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
@@ -1175,43 +1192,50 @@
         Generate title for conversation
         """
         url = f"{self.base_url}conversation/gen_title/{convo_id}"
         response = await self.session.post(
             url,
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
-            ), impersonate='safari15_5'
+            ),
+            impersonate="safari15_5",
         )
         await self.__check_response(response)
 
     async def change_title(self, convo_id: str, title: str) -> None:
         """
         Change title of conversation
         :param convo_id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(url, data=f'{{"title": "{title}"}}', impersonate='safari15_5')
+        response = await self.session.patch(
+            url, data=f'{{"title": "{title}"}}', impersonate="safari15_5"
+        )
         await self.__check_response(response)
 
     async def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param convo_id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
+        response = await self.session.patch(
+            url, data='{"is_visible": false}', impersonate="safari15_5"
+        )
         await self.__check_response(response)
 
     async def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = await self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
+        response = await self.session.patch(
+            url, data='{"is_visible": false}', impersonate="safari15_5"
+        )
         await self.__check_response(response)
 
     async def __map_conversations(self) -> None:
         conversations = await self.get_conversations()
         histories = [await self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
             self.conversation_mapping[x["id"]] = y["current_node"]
```

### Comparing `revChatGPT-5.3.0/src/revChatGPT/V3.py` & `revChatGPT-5.3.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/__init__.py` & `revChatGPT-5.3.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/__main__.py` & `revChatGPT-5.3.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.3.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/recipient.py` & `revChatGPT-5.3.1/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/typings.py` & `revChatGPT-5.3.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT/utils.py` & `revChatGPT-5.3.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.3.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.0
+Version: 5.3.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-5.3.0/tests/test_recipient.py` & `revChatGPT-5.3.1/tests/test_recipient.py`

 * *Files identical despite different names*

