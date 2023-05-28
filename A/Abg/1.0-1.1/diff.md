# Comparing `tmp/Abg-1.0.tar.gz` & `tmp/Abg-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.0.tar", last modified: Sun May 28 14:51:52 2023, max compression
+gzip compressed data, was "Abg-1.1.tar", last modified: Sun May 28 18:12:46 2023, max compression
```

## Comparing `Abg-1.0.tar` & `Abg-1.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.990280 Abg-1.0/Abg/
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-28 14:26:43.000000 Abg-1.0/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/conversation/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-28 14:26:43.000000 Abg-1.0/Abg/conversation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5532 2023-05-28 14:26:43.000000 Abg-1.0/Abg/conversation/conversation.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-05-28 14:26:43.000000 Abg-1.0/Abg/conversation/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/lock.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-28 14:26:43.000000 Abg-1.0/Abg/helpers/pyro_progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-28 14:26:43.000000 Abg-1.0/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-05-28 14:26:43.000000 Abg-1.0/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-05-28 14:26:43.000000 Abg-1.0/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-05-28 14:26:43.000000 Abg-1.0/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.994279 Abg-1.0/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-05-28 14:26:43.000000 Abg-1.0/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:51:52.990280 Abg-1.0/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4415 2023-05-28 14:51:52.000000 Abg-1.0/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-28 14:51:52.000000 Abg-1.0/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 14:51:52.000000 Abg-1.0/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-28 14:51:52.000000 Abg-1.0/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4415 2023-05-28 14:51:52.994279 Abg-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2660 2023-05-28 14:26:43.000000 Abg-1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 14:51:52.994279 Abg-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3112 2023-05-28 14:51:14.000000 Abg-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-28 18:05:19.000000 Abg-1.1/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/conversation/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/lock.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/pyro_progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      721 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-28 18:05:19.000000 Abg-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-05-28 18:12:46.280024 Abg-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-05-28 18:05:19.000000 Abg-1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 18:12:46.280024 Abg-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3052 2023-05-28 18:12:24.000000 Abg-1.1/setup.py
```

### Comparing `Abg-1.0/Abg/conversation/conversation.py` & `Abg-1.1/Abg/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/conversation/errors.py` & `Abg-1.1/Abg/conversation/errors.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/helpers/__init__.py` & `Abg-1.1/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/helpers/helpers.py` & `Abg-1.1/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/helpers/http_helper.py` & `Abg-1.1/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/helpers/parser.py` & `Abg-1.1/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/helpers/pyro_progress.py` & `Abg-1.1/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/inline/inline_keyboard.py` & `Abg-1.1/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/inline/inline_pagination_keyboard.py` & `Abg-1.1/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/inline/reply_keyboard.py` & `Abg-1.1/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/patch/bound/message.py` & `Abg-1.1/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/patch/methods/edit_message_text.py` & `Abg-1.1/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/patch/methods/send_as_file.py` & `Abg-1.1/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg/patch/methods/send_message.py` & `Abg-1.1/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.0/Abg.egg-info/PKG-INFO` & `Abg-1.1/Abg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.0
+Version: 1.1
 Summary: add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
-License: LGPLv3+
+License: MIT
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
-Keywords: telegram chat messenger mtproto api client library python conversation
+Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,37 +30,61 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ᴀʙɢ-ᴘʏʀᴏ :->
 
 > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 > 
 • Conversation in pyrogram
 
 ```python
-  from Abg import Askclient
+  from Abg.conversation import Askclient
   from pyrogram import Client, filters
   
   app = Client("my_account")
   read = Askclient(app)
 
   @app.on_message(filters.command("start"))
   async def start(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
+>
+• Keyboards
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### Result
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
 
 ### ɪɴsᴛᴀʟʟɪɴɢ :->
 
 ```bash
 pip3 install Abg
 ```
```

#### html2text {}

```diff
@@ -1,38 +1,44 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.0 Summary: add-on for pyrogram Home-
+Metadata-Version: 2.1 Name: Abg Version: 1.1 Summary: add-on for pyrogram Home-
 page: https://github.com/Abishnoi69 Download-URL: https://github.com/
 Abishnoi69/Abg/releases/latest Author: Abishnoi1M Author-email:
-Abishnoi69@Abg.org License: LGPLv3+ Project-URL: Tracker, https://github.com/
+Abishnoi69@Abg.org License: MIT Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Keywords: telegram chat messenger mtproto api
-client library python conversation Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 (LGPLv3) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation Classifier: Programming Language :: Python
-:: Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
-Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
-Type: text/markdown # á´ÊÉ¢-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] >
-â¢ Conversation in pyrogram ```python from Abg import Askclient from pyrogram
-import Client, filters app = Client("my_account") read = Askclient(app)
-@app.on_message(filters.command("start")) async def start(c: app, m: Message):
-answer = await read.ask(m, text) if answer.text: print(answer.text) await
-answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ###
-ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
+github.com/Abishnoi69/Abg/wiki Keywords: telegram bot chat messenger mtproto
+api client library python conversation keyboard userbot patch Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Natural Language :: English Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
+Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: Libraries :: Application Frameworks Requires-Python:
+~=3.7 Description-Content-Type: text/markdown License-File: LICENSE # á´ÊÉ¢-
+á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
+[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
+from Abg.conversation import Askclient from pyrogram import Client, filters app
+= Client("my_account") read = Askclient(app) @app.on_message(filters.command
+("start")) async def start(c: app, m: Message): answer = await read.ask(m,
+text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
+á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
+import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
+keyboard.add( InlineButton('1', 'inline_keyboard:1'), InlineButton('2',
+'inline_keyboard:2'), InlineButton('3', 'inline_keyboard:3'), InlineButton('4',
+'inline_keyboard:4'), InlineButton('5', 'inline_keyboard:5'), InlineButton('6',
+'inline_keyboard:6'), InlineButton('7', 'inline_keyboard:7') ) ``` #### Result
+[add_inline_button]
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ :-> ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
```

### Comparing `Abg-1.0/Abg.egg-info/SOURCES.txt` & `Abg-1.1/Abg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 Abg/__init__.py
 Abg.egg-info/PKG-INFO
 Abg.egg-info/SOURCES.txt
 Abg.egg-info/dependency_links.txt
 Abg.egg-info/top_level.txt
```

### Comparing `Abg-1.0/PKG-INFO` & `Abg-1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.0
+Version: 1.1
 Summary: add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
-License: LGPLv3+
+License: MIT
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
-Keywords: telegram chat messenger mtproto api client library python conversation
+Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,37 +30,61 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ᴀʙɢ-ᴘʏʀᴏ :->
 
 > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 > 
 • Conversation in pyrogram
 
 ```python
-  from Abg import Askclient
+  from Abg.conversation import Askclient
   from pyrogram import Client, filters
   
   app = Client("my_account")
   read = Askclient(app)
 
   @app.on_message(filters.command("start"))
   async def start(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
+>
+• Keyboards
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### Result
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
 
 ### ɪɴsᴛᴀʟʟɪɴɢ :->
 
 ```bash
 pip3 install Abg
 ```
```

#### html2text {}

```diff
@@ -1,38 +1,44 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.0 Summary: add-on for pyrogram Home-
+Metadata-Version: 2.1 Name: Abg Version: 1.1 Summary: add-on for pyrogram Home-
 page: https://github.com/Abishnoi69 Download-URL: https://github.com/
 Abishnoi69/Abg/releases/latest Author: Abishnoi1M Author-email:
-Abishnoi69@Abg.org License: LGPLv3+ Project-URL: Tracker, https://github.com/
+Abishnoi69@Abg.org License: MIT Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Keywords: telegram chat messenger mtproto api
-client library python conversation Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 (LGPLv3) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation Classifier: Programming Language :: Python
-:: Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
-Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
-Type: text/markdown # á´ÊÉ¢-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] >
-â¢ Conversation in pyrogram ```python from Abg import Askclient from pyrogram
-import Client, filters app = Client("my_account") read = Askclient(app)
-@app.on_message(filters.command("start")) async def start(c: app, m: Message):
-answer = await read.ask(m, text) if answer.text: print(answer.text) await
-answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ###
-ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
+github.com/Abishnoi69/Abg/wiki Keywords: telegram bot chat messenger mtproto
+api client library python conversation keyboard userbot patch Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Natural Language :: English Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
+Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: Libraries :: Application Frameworks Requires-Python:
+~=3.7 Description-Content-Type: text/markdown License-File: LICENSE # á´ÊÉ¢-
+á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
+[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
+from Abg.conversation import Askclient from pyrogram import Client, filters app
+= Client("my_account") read = Askclient(app) @app.on_message(filters.command
+("start")) async def start(c: app, m: Message): answer = await read.ask(m,
+text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
+á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
+import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
+keyboard.add( InlineButton('1', 'inline_keyboard:1'), InlineButton('2',
+'inline_keyboard:2'), InlineButton('3', 'inline_keyboard:3'), InlineButton('4',
+'inline_keyboard:4'), InlineButton('5', 'inline_keyboard:5'), InlineButton('6',
+'inline_keyboard:6'), InlineButton('7', 'inline_keyboard:7') ) ``` #### Result
+[add_inline_button]
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ :-> ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
```

### Comparing `Abg-1.0/README.md` & `Abg-1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 # ᴀʙɢ-ᴘʏʀᴏ :->
 
 > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
 > 
 • Conversation in pyrogram
 
 ```python
-  from Abg import Askclient
+  from Abg.conversation import Askclient
   from pyrogram import Client, filters
   
   app = Client("my_account")
   read = Askclient(app)
 
   @app.on_message(filters.command("start"))
   async def start(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
+>
+• Keyboards
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### Result
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
 
 ### ɪɴsᴛᴀʟʟɪɴɢ :->
 
 ```bash
 pip3 install Abg
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,22 @@
 # á´ÊÉ¢-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê
 @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in
-pyrogram ```python from Abg import Askclient from pyrogram import Client,
-filters app = Client("my_account") read = Askclient(app) @app.on_message
-(filters.command("start")) async def start(c: app, m: Message): answer = await
-read.ask(m, text) if answer.text: print(answer.text) await answer.reply("Éª
-É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash
-pip3 install Abg ```
+pyrogram ```python from Abg.conversation import Askclient from pyrogram import
+Client, filters app = Client("my_account") read = Askclient(app)
+@app.on_message(filters.command("start")) async def start(c: app, m: Message):
+answer = await read.ask(m, text) if answer.text: print(answer.text) await
+answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards
+```python from Abg.inline import InlineKeyboard, InlineButton keyboard =
+InlineKeyboard(row_width=3) keyboard.add( InlineButton('1', 'inline_keyboard:
+1'), InlineButton('2', 'inline_keyboard:2'), InlineButton('3',
+'inline_keyboard:3'), InlineButton('4', 'inline_keyboard:4'), InlineButton('5',
+'inline_keyboard:5'), InlineButton('6', 'inline_keyboard:6'), InlineButton('7',
+'inline_keyboard:7') ) ``` #### Result
+[add_inline_button]
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ :-> ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
```

### Comparing `Abg-1.0/setup.py` & `Abg-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,28 +33,27 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.0",
+    version="1.1",
     description="add-on for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
-    author_email="Abishnoi69@Abg.org",
-    license="LGPLv3+",
+    author_email="Abishnoi69@Abg.org", 
+    license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
-        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
@@ -65,15 +64,15 @@
         "Topic :: Internet",
         "Topic :: Communications",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
-    keywords="telegram chat messenger mtproto api client library python conversation",
+    keywords="telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch",
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Abg/issues",
         "Community": "https://t.me/Abg",
         "Source": "https://github.com/Abishnoi69/Abg",
         "Documentation": "https://github.com/Abishnoi69/Abg/wiki",
     },
     python_requires="~=3.7",
```

