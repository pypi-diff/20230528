# Comparing `tmp/revChatGPT-5.2.0.tar.gz` & `tmp/revChatGPT-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.2.0.tar", last modified: Sat May 27 02:23:18 2023, max compression
+gzip compressed data, was "revChatGPT-5.3.0.tar", last modified: Sun May 28 11:41:32 2023, max compression
```

## Comparing `revChatGPT-5.2.0.tar` & `revChatGPT-5.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.678747 revChatGPT-5.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    50788 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.178158 revChatGPT-5.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.178158 revChatGPT-5.3.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    53601 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 11:41:32.000000 revChatGPT-5.3.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:41:32.182158 revChatGPT-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-28 11:40:55.000000 revChatGPT-5.3.0/tests/test_recipient.py
```

### Comparing `revChatGPT-5.2.0/LICENSE` & `revChatGPT-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/PKG-INFO` & `revChatGPT-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.2.0
+Version: 5.3.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -89,15 +89,16 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "disable_history": true,
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-5.2.0/README.md` & `revChatGPT-5.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "disable_history": true,
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-5.2.0/setup.py` & `revChatGPT-5.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.2.0",
+    version="5.3.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
@@ -32,14 +32,15 @@
         "OpenAIAuth>=1.0.2",
         "requests[socks]",
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
+        "curl_cffi"
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `revChatGPT-5.2.0/src/revChatGPT/V1.py` & `revChatGPT-5.3.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 import binascii
 import contextlib
 import datetime
 import json
 import logging
 import time
 import uuid
+import tempfile
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
+
 import httpx
-import requests
-from httpx import AsyncClient
+from curl_cffi import requests
 from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
 from .recipient import PythonRecipient
 from .recipient import Recipient
 from .recipient import RecipientManager
@@ -76,15 +77,15 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/" # "https://chat.openai.com/backend-api/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
@@ -94,15 +95,14 @@
 
     @logger(is_timed=True)
     def __init__(
         self,
         config: dict[str, str],
         conversation_id: str | None = None,
         parent_id: str | None = None,
-        session_client=None,
         lazy_loading: bool = True,
         base_url: str | None = None,
     ) -> None:
         """Initialize a chatbot
 
         Args:
             config (dict[str, str]): Login and proxy info. Example:
@@ -111,15 +111,14 @@
                     "proxy": "<proxy_url_string>",
                     "model": "<model_name>",
                     "plugin": "<plugin_id>",
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
-            session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
             Exception: _description_
         """
         user_home = getenv("HOME")
         if user_home is None:
             user_home = Path().cwd()
@@ -129,15 +128,16 @@
             if not Path(user_home, ".config").exists():
                 Path(user_home, ".config").mkdir()
             if not Path(user_home, ".config", "revChatGPT").exists():
                 Path(user_home, ".config", "revChatGPT").mkdir()
             self.cache_path = Path(user_home, ".config", "revChatGPT", "cache.json")
 
         self.config = config
-        self.session = session_client() if session_client else requests.Session()
+        self.session = requests.Session()
+
         if "email" in config and "password" in config:
             try:
                 cached_access_token = self.__get_cached_access_token(
                     self.config.get("email", None),
                 )
             except t.Error as error:
                 if error.code == 5:
@@ -150,33 +150,37 @@
             if not isinstance(config["proxy"], str):
                 error = TypeError("Proxy must be a string!")
                 raise error
             proxies = {
                 "http": config["proxy"],
                 "https": config["proxy"],
             }
-            if isinstance(self.session, AsyncClient):
-                proxies = {
-                    "http://": config["proxy"],
-                    "https://": config["proxy"],
-                }
-                self.session = AsyncClient(proxies=proxies)  # type: ignore
-            else:
-                self.session.proxies.update(proxies)
+            self.session.proxies.update(proxies)
 
         self.conversation_id = conversation_id or config.get("conversation_id", None)
         self.parent_id = parent_id or config.get("parent_id", None)
         self.conversation_mapping = {}
         self.conversation_id_prev_queue = []
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
-        self.base_url = base_url or BASE_URL
         self.recipients = RecipientManager()
+        self.disable_history = config.get("disable_history", False)
 
         self.__check_credentials()
+        # Check if chat.openai.com is reachable
+        if not base_url:
+            response = self.session.get("https://chat.openai.com/backend-api/accounts/check", impersonate='safari15_5')
+            if response.status_code != 200:
+                print(f"Using bypass.churchless.tech backend due to status code {response.status_code}")
+                self.base_url = BASE_URL
+            else:
+                print("Using chat.openai.com backend")
+                self.base_url = "https://chat.openai.com/backend-api/"
+        else:
+            self.base_url = base_url
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
@@ -339,26 +343,32 @@
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         model, message = None, ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
-        response = self.session.post(
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
-            timeout=timeout,
-            stream=True,
-        )
+
+        conversation_stream = self.handle_conversation_stream(step=1)
+
+        with open(conversation_stream.name, "wb") as response_file:
+            response = self.session.post(
+                url=f"{self.base_url}conversation",
+                data=json.dumps(data),
+                timeout=timeout,
+                impersonate='safari15_5',
+                content_callback=response_file.write, # a hack around curl_cffi not supporting stream=True
+            )
         self.__check_response(response)
 
         finish_details = None
-        for line in response.iter_lines():
-            # remove b' and ' at the beginning and end and ignore case
-            line = str(line)[2:-1]
+
+        response_lst = self.handle_conversation_stream(file=conversation_stream, step=2)
+
+        for line in response_lst:
             if line.lower() == "internal server error":
                 log.error(f"Internal Server Error: {line}")
                 error = t.Error(
                     source="ask",
                     message="Internal Server Error",
                     code=t.ErrorType.SERVER_ERROR,
                 )
@@ -366,17 +376,20 @@
             if not line or line is None:
                 continue
             if "data: " in line:
                 line = line[6:]
             if line == "[DONE]":
                 break
 
+            """
+            # this seems to just cut off parts of some messages
             line = line.replace('\\"', '"')
             line = line.replace("\\'", "'")
             line = line.replace("\\\\", "\\")
+            """
 
             try:
                 line = json.loads(line)
             except json.decoder.JSONDecodeError:
                 continue
             if not self.__check_fields(line):
                 raise ValueError(f"Field missing. Details: {str(line)}")
@@ -497,14 +510,15 @@
 
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model or self.config.get("model") or "text-davinci-002-render-sha",
+            "history_and_training_disabled": self.disable_history,
         }
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
 
         yield from self.__send_request(
             data,
@@ -635,14 +649,15 @@
             "model": model
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
+            "history_and_training_disabled": self.disable_history,
         }
 
         yield from self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         )
@@ -684,30 +699,30 @@
     ) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = self.session.get(url)
+        response = self.session.get(url, impersonate='safari15_5')
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
-        response = self.session.get(url)
+        response = self.session.get(url, impersonate='safari15_5')
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
@@ -715,46 +730,47 @@
         Generate title for conversation
         """
         response = self.session.post(
             f"{self.base_url}conversation/gen_title/{convo_id}",
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
             ),
+            impersonate='safari15_5'
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
-        response = self.session.patch(url, data=json.dumps({"title": title}))
+        response = self.session.patch(url, data=json.dumps({"title": title}), impersonate='safari15_5')
         self.__check_response(response)
 
     @logger(is_timed=True)
     def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.patch(url, data='{"is_visible": false}')
+        response = self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
         self.__check_response(response)
 
     @logger(is_timed=True)
     def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = self.session.patch(url, data='{"is_visible": false}')
+        response = self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
         self.__check_response(response)
 
     @logger(is_timed=False)
     def __map_conversations(self) -> None:
         conversations = self.get_conversations()
         histories = [self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
@@ -780,26 +796,36 @@
         for _ in range(num):
             self.conversation_id = self.conversation_id_prev_queue.pop()
             self.parent_id = self.parent_id_prev_queue.pop()
 
     @logger(is_timed=True)
     def get_plugins(self, offset: int = 0, limit: int = 250, status: str = "approved"):
         url = f"{self.base_url}aip/p?offset={offset}&limit={limit}&statuses={status}"
-        response = self.session.get(url)
+        response = self.session.get(url, impersonate='safari15_5')
         self.__check_response(response)
         # Parse as JSON
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def install_plugin(self, plugin_id: str):
         url = f"{self.base_url}aip/p/{plugin_id}/user-settings"
         payload = {"is_installed": True}
-        response = self.session.patch(url, data=json.dumps(payload))
+        response = self.session.patch(url, data=json.dumps(payload), impersonate='safari15_5')
         self.__check_response(response)
 
+    @logger(is_timed=False)
+    def handle_conversation_stream(self, file = None, step: int = 1):
+        if step == 1: 
+            return tempfile.NamedTemporaryFile(delete=False)
+        elif step == 2 and file:
+            with open(file.name, "r") as response_file:
+                response_lst = response_file.read().splitlines()
+            file.close()
+            Path(file.name).unlink()
+            return response_lst
 
 class AsyncChatbot(Chatbot):
     """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
@@ -810,53 +836,83 @@
         """
         Same as Chatbot class, but with async methods.
         """
         super().__init__(
             config=config,
             conversation_id=conversation_id,
             parent_id=parent_id,
-            session_client=AsyncClient,
             base_url=base_url,
         )
 
+        # overwrite inherited normal session with async
+        headers_transfer = self.session.headers
+        self.session = requests.AsyncSession()
+        self.session.headers = headers_transfer
+
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
     ) -> AsyncGenerator[dict, None]:
         cid, pid = data["conversation_id"], data["parent_message_id"]
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         message = ""
 
         finish_details = None
         response = None
-        async with self.session.stream(
-            method="POST",
-            url=f"{self.base_url}conversation",
-            data=json.dumps(data),
-            timeout=timeout,
-        ) as response:
+
+        conversation_stream = self.handle_conversation_stream(step=1)
+
+        async with self.session as s:
+            with open(conversation_stream.name, "wb") as response_file:
+                response = await s.post(
+                    url=f"{self.base_url}conversation",
+                    data=json.dumps(data),
+                    timeout=timeout,
+                    impersonate='safari15_5',
+                    content_callback=response_file.write,
+                    )
             await self.__check_response(response)
-            async for line in response.aiter_lines():
+
+            response_lst = self.handle_conversation_stream(file=conversation_stream, step=2)
+
+            for line in response_lst:
+                if line.lower() == "internal server error":
+                    log.error(f"Internal Server Error: {line}")
+                    error = t.Error(
+                        source="ask",
+                        message="Internal Server Error",
+                        code=t.ErrorType.SERVER_ERROR,
+                    )
+                    raise error
                 if not line or line is None:
                     continue
                 if "data: " in line:
                     line = line[6:]
                 if "[DONE]" in line:
                     break
 
+                """
+                # this seems to just cut off parts of some messages
+                line = line.replace('\\"', '"')
+                line = line.replace("\\'", "'")
+                line = line.replace("\\\\", "\\")
+                """
+
                 try:
                     line = json.loads(line)
                 except json.decoder.JSONDecodeError:
                     continue
                 if not self.__check_fields(line):
                     raise ValueError(f"Field missing. Details: {str(line)}")
+                if line.get("message").get("author").get("role") != "assistant":
+                    continue
 
                 message: str = line["message"]["content"]["parts"][0]
                 cid = line["conversation_id"]
                 pid = line["message"]["id"]
                 metadata = line["message"].get("metadata", {})
                 model = metadata.get("model_slug", None)
                 finish_details = metadata.get("finish_details", {"type": None})["type"]
@@ -948,14 +1004,15 @@
             "model": model
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
+            "history_and_training_disabled": self.disable_history,
         }
 
         async for msg in self.__send_request(
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
@@ -1070,14 +1127,15 @@
             "model": model
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
+            "history_and_training_disabled": self.disable_history,
         }
 
         async for msg in self.__send_request(
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
@@ -1086,30 +1144,30 @@
     async def get_conversations(self, offset: int = 0, limit: int = 20) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = await self.session.get(url)
+        response = await self.session.get(url, impersonate='safari15_5')
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
-        response = await self.session.get(url)
+        response = await self.session.get(url, impersonate='safari15_5')
         if encoding is not None:
             response.encoding = encoding
             await self.__check_response(response)
             return json.loads(response.text)
         return None
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
@@ -1117,43 +1175,43 @@
         Generate title for conversation
         """
         url = f"{self.base_url}conversation/gen_title/{convo_id}"
         response = await self.session.post(
             url,
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
-            ),
+            ), impersonate='safari15_5'
         )
         await self.__check_response(response)
 
     async def change_title(self, convo_id: str, title: str) -> None:
         """
         Change title of conversation
         :param convo_id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(url, data=f'{{"title": "{title}"}}')
+        response = await self.session.patch(url, data=f'{{"title": "{title}"}}', impersonate='safari15_5')
         await self.__check_response(response)
 
     async def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param convo_id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(url, data='{"is_visible": false}')
+        response = await self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
         await self.__check_response(response)
 
     async def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = await self.session.patch(url, data='{"is_visible": false}')
+        response = await self.session.patch(url, data='{"is_visible": false}', impersonate='safari15_5')
         await self.__check_response(response)
 
     async def __map_conversations(self) -> None:
         conversations = await self.get_conversations()
         histories = [await self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
             self.conversation_mapping[x["id"]] = y["current_node"]
@@ -1286,16 +1344,15 @@
                     + ("enabled" if plugin in plugins else "disabled"),
                 )
                 print()
             except IndexError:
                 log.exception("Please include plugin name in command")
                 print("Please include plugin name in command")
         elif command == "!exit":
-            if isinstance(chatbot.session, httpx.AsyncClient):
-                chatbot.session.aclose()
+            chatbot.session.close()
             exit()
         else:
             return False
         return True
 
     session = create_session()
     completer = create_completer(
```

### Comparing `revChatGPT-5.2.0/src/revChatGPT/V3.py` & `revChatGPT-5.3.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/__init__.py` & `revChatGPT-5.3.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/__main__.py` & `revChatGPT-5.3.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.3.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/recipient.py` & `revChatGPT-5.3.0/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/typings.py` & `revChatGPT-5.3.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT/utils.py` & `revChatGPT-5.3.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.2.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.3.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.2.0
+Version: 5.3.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -89,15 +89,16 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "disable_history": true,
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-5.2.0/tests/test_recipient.py` & `revChatGPT-5.3.0/tests/test_recipient.py`

 * *Files identical despite different names*

