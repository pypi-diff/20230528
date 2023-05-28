# Comparing `tmp/whatsapp-python-2.9.3.tar.gz` & `tmp/whatsapp-python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-python-2.9.3.tar", last modified: Sat May 27 10:35:58 2023, max compression
+gzip compressed data, was "whatsapp-python-3.0.0.tar", last modified: Sun May 28 11:59:37 2023, max compression
```

## Comparing `whatsapp-python-2.9.3.tar` & `whatsapp-python-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/whatsapp/
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-27 10:35:57.000000 whatsapp-python-2.9.3/whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:35:58.667622 whatsapp-python-2.9.3/whatsapp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 10:35:58.000000 whatsapp-python-2.9.3/whatsapp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:59:37.445787 whatsapp-python-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 11:59:36.000000 whatsapp-python-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-28 11:59:37.441787 whatsapp-python-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-28 11:59:36.000000 whatsapp-python-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:59:37.445787 whatsapp-python-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-28 11:59:36.000000 whatsapp-python-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:59:37.441787 whatsapp-python-3.0.0/whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-28 11:59:36.000000 whatsapp-python-3.0.0/whatsapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:59:36.000000 whatsapp-python-3.0.0/whatsapp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:59:37.441787 whatsapp-python-3.0.0/whatsapp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-28 11:59:37.000000 whatsapp-python-3.0.0/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-28 11:59:37.000000 whatsapp-python-3.0.0/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:59:37.000000 whatsapp-python-3.0.0/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 11:59:37.000000 whatsapp-python-3.0.0/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 11:59:37.000000 whatsapp-python-3.0.0/whatsapp_python.egg-info/top_level.txt
```

### Comparing `whatsapp-python-2.9.3/LICENSE` & `whatsapp-python-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-python-2.9.3/PKG-INFO` & `whatsapp-python-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.9.3
-Summary: Opensource Python wrapper to WhatsApp Cloud API
+Version: 3.0.0
+Summary: Open source Python wrapper for the WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
+Download-URL: https://github.com/filipporomani/whatsapp/releases/latest
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
@@ -29,31 +31,33 @@
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
 ## Supported features
 
-1. Sending messages
-2. Marking messages as read
-3. Sending Media (images, audio, video and documents)
-4. Sending location
-5. Sending interactive buttons
-6. Sending template messages
-7. Parsing messages and media received
-8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+1. Listening to events (messages, media, etc.)
+2. Sending messages
+3. Marking messages as read
+4. Sending Media (images, audio, video and documents)
+5. Sending location
+6. Sending interactive buttons
+7. Sending template messages
+8. Parsing messages and media received
 
 ## App events
 
-App events are now available! 
+Asynchronous app events are now available!
 
 The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
 
 Please test this feature out and leave feedbacks/report issues on GitHub!
 
+**NOTE:** this feature is still in beta, so it may not work as expected. The FastAPI endpoint was not completely tested. Please report any issue you find or open a PR to fix it!
+
 ## Installation
 
 To install the library you can either use pip:
 
 ``pip install whatsapp-python``
 
 or git:
@@ -80,15 +84,15 @@
 Any version <=1.1.2 is fully compatible with the original `heyoo` library and doesn't include any breaking change.
 You can ignore this warning if it's your first time using the library.
 
 
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
-Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
+Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2).
 
 
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [**GitHub repository**](https://github.com/filipporomani/whatsapp/issues)
```

### Comparing `whatsapp-python-2.9.3/README.md` & `whatsapp-python-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,33 @@
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
 ## Supported features
 
-1. Sending messages
-2. Marking messages as read
-3. Sending Media (images, audio, video and documents)
-4. Sending location
-5. Sending interactive buttons
-6. Sending template messages
-7. Parsing messages and media received
-8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+1. Listening to events (messages, media, etc.)
+2. Sending messages
+3. Marking messages as read
+4. Sending Media (images, audio, video and documents)
+5. Sending location
+6. Sending interactive buttons
+7. Sending template messages
+8. Parsing messages and media received
 
 ## App events
 
-App events are now available! 
+Asynchronous app events are now available!
 
 The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
 
 Please test this feature out and leave feedbacks/report issues on GitHub!
 
+**NOTE:** this feature is still in beta, so it may not work as expected. The FastAPI endpoint was not completely tested. Please report any issue you find or open a PR to fix it!
+
 ## Installation
 
 To install the library you can either use pip:
 
 ``pip install whatsapp-python``
 
 or git:
@@ -58,15 +60,15 @@
 Any version <=1.1.2 is fully compatible with the original `heyoo` library and doesn't include any breaking change.
 You can ignore this warning if it's your first time using the library.
 
 
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
-Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
+Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2).
 
 
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [**GitHub repository**](https://github.com/filipporomani/whatsapp/issues)
```

### Comparing `whatsapp-python-2.9.3/setup.py` & `whatsapp-python-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from os import path
 from setuptools import setup
-
+from pre_dist import update_version
+update_version()
+from constants import VERSION
 # read the contents of your description file
 # the version in this file should be updated ONLY on a new PYPI release
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="whatsapp-python",
-    version="2.9.3",
-    description="Opensource Python wrapper to WhatsApp Cloud API",
+    version=VERSION,
+    description="Open source Python wrapper for the WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
+    download_url="https://github.com/filipporomani/whatsapp/releases/latest",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
     packages=["whatsapp"],
-    install_requires=["requests", "requests-toolbelt", "typing"],
+    install_requires=["requests", "requests-toolbelt", "typing", "fastapi"],
     keywords=[
         "whatsapp",
         "whatsapp-libary",
         "WhatsApp Cloud API Wrapper",
         "PyWhatsApp",
         "WhatsApp API in Python",
     ],
@@ -34,9 +37,10 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `whatsapp-python-2.9.3/whatsapp/__init__.py` & `whatsapp-python-3.0.0/whatsapp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,108 +2,112 @@
 Unofficial Python wrapper for the WhatsApp Cloud API.
 """
 from __future__ import annotations
 
 import requests
 from json import dumps
 import logging
-from flask import Flask, request, Response
+from fastapi import FastAPI, Request
+from constants import VERSION
 
 
 # Setup logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 class WhatsApp(object):
-    def __init__(self, token: str = "", phone_number_id: str = "", logger: bool = True):
+    def __init__(self, token: str = "", phone_number_id: str = "", logger: bool = True, update_check: bool = True):
         """
         Initialize the WhatsApp Object
 
         Args:
             token[str]: Token for the WhatsApp cloud API obtained from the Facebook developer portal
             phone_number_id[str]: Phone number id for the WhatsApp cloud API obtained from the developer portal
             logger[bool]: Whether to enable logging or not (default: True)
         """
 
-        # version here MUST be changed manually after every change to deferentiate between PYPI and GitHub versions
         # Check if the version is up to date
 
-        self.VERSION = "2.9.3"
-
-        latest = str(requests.get(
-            "https://pypi.org/pypi/whatsapp-python/json").json()["info"]["version"])
-        if self.VERSION != latest:
-            version_int = int(self.VERSION.replace(".", ""))
-            latest_int = int(latest.replace(".", ""))
-            # this is to avoid the case where the version is 1.0.10 and the latest is 1.0.2 (possible if user is using the github version)
-            if version_int < latest_int:
-                logging.critical(
-                    f"Whatsapp-python is out of date. Please update to the latest version {latest}. READ THE CHANGELOG BEFORE UPDATING. NEW VERSIONS MAY BREAK YOUR CODE IF NOT PROPERLY UPDATED.")
-            if version_int > latest_int:
-                logging.critical(
-                    f"You are using a development version of whatsapp-python. Please report any issue on GitHub.")
+        self.VERSION = VERSION
+        if update_check is True:
+            latest = str(requests.get(
+                "https://pypi.org/pypi/whatsapp-python/json").json()["info"]["version"])
+            if self.VERSION != latest:
+                version_int = int(self.VERSION.replace(".", ""))
+                latest_int = int(latest.replace(".", ""))
+                # this is to avoid the case where the version is 1.0.10 and the latest is 1.0.2 (possible if user is using the github version)
+                if version_int < latest_int:
+                    logging.critical(
+                        f"Whatsapp-python is out of date. Please update to the latest version {latest}. READ THE CHANGELOG BEFORE UPDATING. NEW VERSIONS MAY BREAK YOUR CODE IF NOT PROPERLY UPDATED.")
+                if version_int > latest_int:
+                    latest_beta = int(str(requests.get(
+                        "https://raw.githubusercontent.com/filipporomani/whatsapp/main/.version").text).replace(".", ""))
+                    if latest_beta > version_int:
+                        logging.critical(
+                            "A new beta version is available. Please update to the latest version. READ THE CHANGELOG BEFORE UPDATING. NEW VERSIONS MAY BREAK YOUR CODE IF NOT PROPERLY UPDATED.")
+                    logging.critical(
+                        f"You are using a development version of whatsapp-python. Please report any issue on GitHub.")
 
         if token == "" or phone_number_id == "":
             logging.error("Token or phone number id not provided")
             raise ValueError(
                 "Token or phone number ID not provided but is required")
         self.token = token
         self.phone_number_id = phone_number_id
-        self.base_url = "https://graph.facebook.com/v15.0"
+        self.base_url = "https://graph.facebook.com/v16.0"
         self.url = f"{self.base_url}/{phone_number_id}/messages"
 
-        def base():
+        async def base():
             pass
         self.message_handler = base
         self.other_handler = base
         self.verification_handler = base
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.token}"
         }
         if logger is False:
             logging.disable(logging.INFO)
             logging.disable(logging.ERROR)
 
-        self.app = Flask(__name__)
+        self.app = FastAPI()
 
         # Verification handler has 1 argument: challenge (str | bool): str if verification is successful, False if not
 
         @self.app.get("/")
-        def verify_token():
-            if request.args.get("hub.verify_token") == self.token:
+        async def verify_endpoint(r: Request):
+            if r.query_params.get("hub.verify_token") == self.token:
                 logging.info("Verified webhook")
-                challenge = request.args.get("hub.challenge")
+                challenge = r.query_params.get("hub.challenge")
                 self.verification_handler(challenge)
                 self.other_handler(challenge)
                 return str(challenge)
             logging.error("Webhook Verification failed")
-            self.verification_handler(False)
-            self.other_handler(False)
-            return "Invalid verification token"
+            await self.verification_handler(False)
+            await self.other_handler(False)
+            return {"success": False}
 
         @self.app.post("/")
-        def hook():
+        async def hook(r: Request):
             # Handle Webhook Subscriptions
-            data = request.get_json()
+            data = await r.json()
             if data is None:
-                return Response(status=200)
+                return {"success": False}
             logging.info("Received webhook data: %s", data)
             changed_field = self.instance.changed_field(data)
             if changed_field == "messages":
                 new_message = self.instance.is_message(data)
                 if new_message:
                     msg = Message(instance=self.instance, data=data)
-                    self.message_handler(msg)
-                    self.other_handler(msg)
-            return "OK", 200
+                    await self.message_handler(msg)
+                    await self.other_handler(msg)
+            return {"success": True}
 
     # all the files starting with _ are imported here, and should not be imported directly.
 
-
     from ext._property import authorized
     from ext._send_others import send_custom_json, send_contacts
     from ext._message import send_template
     from ext._send_media import send_image, send_video, send_audio, send_location, send_sticker, send_document
     from ext._media import upload_media, query_media_url, download_media, delete_media
     from ext._buttons import send_button, create_button, send_reply_button
     from ext._static import is_message, get_mobile, get_author, get_name, get_message, get_message_id, get_message_type, get_message_timestamp, get_audio, get_delivery, get_document, get_image, get_interactive_response, get_location, get_video, changed_field
```

### Comparing `whatsapp-python-2.9.3/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-3.0.0/whatsapp_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.9.3
-Summary: Opensource Python wrapper to WhatsApp Cloud API
+Version: 3.0.0
+Summary: Open source Python wrapper for the WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
+Download-URL: https://github.com/filipporomani/whatsapp/releases/latest
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
@@ -29,31 +31,33 @@
 
 Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
 
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
 ## Supported features
 
-1. Sending messages
-2. Marking messages as read
-3. Sending Media (images, audio, video and documents)
-4. Sending location
-5. Sending interactive buttons
-6. Sending template messages
-7. Parsing messages and media received
-8. Receiving and parsing messages - [hook object](https://github.com/filipporomani/whatsapp/wiki/Hook()-object)
+1. Listening to events (messages, media, etc.)
+2. Sending messages
+3. Marking messages as read
+4. Sending Media (images, audio, video and documents)
+5. Sending location
+6. Sending interactive buttons
+7. Sending template messages
+8. Parsing messages and media received
 
 ## App events
 
-App events are now available! 
+Asynchronous app events are now available!
 
 The docs are available in the [wiki](https://github.com/filipporomani/whatsapp/wiki/App-events)
 
 Please test this feature out and leave feedbacks/report issues on GitHub!
 
+**NOTE:** this feature is still in beta, so it may not work as expected. The FastAPI endpoint was not completely tested. Please report any issue you find or open a PR to fix it!
+
 ## Installation
 
 To install the library you can either use pip:
 
 ``pip install whatsapp-python``
 
 or git:
@@ -80,15 +84,15 @@
 Any version <=1.1.2 is fully compatible with the original `heyoo` library and doesn't include any breaking change.
 You can ignore this warning if it's your first time using the library.
 
 
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
-Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
+Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2).
 
 
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [**GitHub repository**](https://github.com/filipporomani/whatsapp/issues)
```

