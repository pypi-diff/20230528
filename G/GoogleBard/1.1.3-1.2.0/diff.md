# Comparing `tmp/GoogleBard-1.1.3.tar.gz` & `tmp/GoogleBard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.1.3.tar", last modified: Fri May 26 13:06:24 2023, max compression
+gzip compressed data, was "GoogleBard-1.2.0.tar", last modified: Sun May 28 12:52:56 2023, max compression
```

## Comparing `GoogleBard-1.1.3.tar` & `GoogleBard-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:06:24.071500 GoogleBard-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.1.3/LICENSE` & `GoogleBard-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.3/PKG-INFO` & `GoogleBard-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.3
+Version: 1.2.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.1.3/README.md` & `GoogleBard-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.3/setup.py` & `GoogleBard-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.1.3",
+    version="1.2.0",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.1.3/src/Bard.py` & `GoogleBard-1.2.0/src/Bard.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import argparse
 import json
 import os
 import random
 import re
-import sys
 import string
+import sys
+import time
+
 import requests
-from prompt_toolkit import prompt, PromptSession
+from prompt_toolkit import prompt
+from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.console import Console
 from rich.markdown import Markdown
 
@@ -92,31 +95,72 @@
         self.session_id = session_id
         self.session = session or requests.Session()
         self.session.headers = headers
         self.session.cookies.set("__Secure-1PSID", session_id)
         self.SNlM0e = self.__get_snlm0e()
         self.timeout = timeout
 
+    def save_conversation(self, file_path: str, conversation_name: str):
+        conversations = self.load_conversations(file_path)
+        conversation_details = {
+            {
+                "conversation_name": conversation_name,
+                "_reqid": self._reqid,
+                "conversation_id": self.conversation_id,
+                "response_id": self.response_id,
+                "choice_id": self.choice_id,
+                "SNlM0e": self.SNlM0e,
+            },
+        }
+        conversations.append(conversation_details)
+
+        with open(file_path, "w", encoding="utf-8") as f:
+            json.dump(conversations, f, indent=4)
+
+    def load_conversations(self, file_path: str) -> list[dict]:
+        # Check if file exists
+        if not os.path.isfile(file_path):
+            return []
+        with open(file_path, encoding="utf-8") as f:
+            return json.load(f)
+
+    def load_conversation(self, file_path: str, conversation_name: str) -> bool:
+        """
+        Loads a conversation from history file. Returns whether the conversation was found.
+        """
+        conversations = self.load_conversations(file_path)
+        for conversation in conversations:
+            if conversation["conversation_name"] == conversation_name:
+                self._reqid = conversation["_reqid"]
+                self.conversation_id = conversation["conversation_id"]
+                self.response_id = conversation["response_id"]
+                self.choice_id = conversation["choice_id"]
+                self.SNlM0e = conversation["SNlM0e"]
+                return True
+        return False
+
     def __get_snlm0e(self):
         # Find "SNlM0e":"<ID>"
         if not self.session_id or self.session_id[-1] != ".":
             raise Exception(
-                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value."
+                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value.",
             )
         resp = self.session.get(
-            "https://bard.google.com/", timeout=10, proxies=self.proxy
+            "https://bard.google.com/",
+            timeout=10,
+            proxies=self.proxy,
         )
         if resp.status_code != 200:
             raise Exception(
-                f"Response code not 200. Response Status is {resp.status_code}"
+                f"Response code not 200. Response Status is {resp.status_code}",
             )
         SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
         if not SNlM0e:
             raise Exception(
-                "SNlM0e value not found in response. Check __Secure-1PSID value."
+                "SNlM0e value not found in response. Check __Secure-1PSID value.",
             )
         return SNlM0e.group(1)
 
     def ask(self, message: str) -> dict:
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
```

### Comparing `GoogleBard-1.1.3/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.2.0/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.3
+Version: 1.2.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

