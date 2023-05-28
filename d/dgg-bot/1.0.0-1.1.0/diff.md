# Comparing `tmp/dgg-bot-1.0.0.tar.gz` & `tmp/dgg-bot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgg-bot-1.0.0.tar", last modified: Fri May 26 14:20:52 2023, max compression
+gzip compressed data, was "dgg-bot-1.1.0.tar", last modified: Sun May 28 00:28:32 2023, max compression
```

## Comparing `dgg-bot-1.0.0.tar` & `dgg-bot-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.726970 dgg-bot-1.0.0/
--rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3886 2023-05-26 14:20:52.725970 dgg-bot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2023-05-26 14:19:48.000000 dgg-bot-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.690970 dgg-bot-1.0.0/dgg_bot.egg-info/
--rw-rw-rw-   0        0        0     3886 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.716971 dgg-bot-1.0.0/dggbot/
--rw-rw-rw-   0        0        0      329 2023-05-26 14:15:08.000000 dgg-bot-1.0.0/dggbot/__init__.py
--rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-1.0.0/dggbot/_logging.py
--rw-rw-rw-   0        0        0     4141 2023-04-03 11:05:30.000000 dgg-bot-1.0.0/dggbot/bot.py
--rw-rw-rw-   0        0        0     7756 2023-05-26 13:57:58.000000 dgg-bot-1.0.0/dggbot/chat.py
--rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-1.0.0/dggbot/errors.py
--rw-rw-rw-   0        0        0      622 2023-05-26 13:06:27.000000 dgg-bot-1.0.0/dggbot/event.py
--rw-rw-rw-   0        0        0      863 2023-05-26 13:12:01.000000 dgg-bot-1.0.0/dggbot/flairs.py
--rw-rw-rw-   0        0        0      339 2023-03-13 02:12:12.000000 dgg-bot-1.0.0/dggbot/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.721970 dgg-bot-1.0.0/dggbot/live/
--rw-rw-rw-   0        0        0     1770 2023-04-28 01:20:01.000000 dgg-bot-1.0.0/dggbot/live/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-05-22 18:25:49.000000 dgg-bot-1.0.0/dggbot/live/message.py
--rw-rw-rw-   0        0        0     3892 2023-05-26 14:03:51.000000 dgg-bot-1.0.0/dggbot/message.py
--rw-rw-rw-   0        0        0      151 2023-05-26 11:13:39.000000 dgg-bot-1.0.0/dggbot/user.py
--rw-rw-rw-   0        0        0     2578 2023-05-26 10:38:55.000000 dgg-bot-1.0.0/dggbot/wsbase.py
--rw-rw-rw-   0        0        0     1221 2023-05-26 14:19:48.000000 dgg-bot-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       41 2023-05-26 14:11:03.000000 dgg-bot-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 14:20:52.726970 dgg-bot-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.724969 dgg-bot-1.0.0/tests/
--rw-rw-rw-   0        0        0      357 2023-05-26 13:31:13.000000 dgg-bot-1.0.0/tests/testtest.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/
+-rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3886 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2023-05-26 14:19:48.000000 dgg-bot-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.663973 dgg-bot-1.1.0/dgg_bot.egg-info/
+-rw-rw-rw-   0        0        0     3886 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.691721 dgg-bot-1.1.0/dggbot/
+-rw-rw-rw-   0        0        0      479 2023-05-28 00:19:50.000000 dgg-bot-1.1.0/dggbot/__init__.py
+-rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-1.1.0/dggbot/_logging.py
+-rw-rw-rw-   0        0        0     4141 2023-04-03 11:05:30.000000 dgg-bot-1.1.0/dggbot/bot.py
+-rw-rw-rw-   0        0        0     8692 2023-05-28 00:23:03.000000 dgg-bot-1.1.0/dggbot/chat.py
+-rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-1.1.0/dggbot/errors.py
+-rw-rw-rw-   0        0        0      736 2023-05-27 22:47:33.000000 dgg-bot-1.1.0/dggbot/event.py
+-rw-rw-rw-   0        0        0      863 2023-05-26 13:12:01.000000 dgg-bot-1.1.0/dggbot/flairs.py
+-rw-rw-rw-   0        0        0      339 2023-03-13 02:12:12.000000 dgg-bot-1.1.0/dggbot/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.695720 dgg-bot-1.1.0/dggbot/live/
+-rw-rw-rw-   0        0        0     1770 2023-04-28 01:20:01.000000 dgg-bot-1.1.0/dggbot/live/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-05-22 18:25:49.000000 dgg-bot-1.1.0/dggbot/live/message.py
+-rw-rw-rw-   0        0        0     5476 2023-05-28 00:17:58.000000 dgg-bot-1.1.0/dggbot/message.py
+-rw-rw-rw-   0        0        0      210 2023-05-27 23:15:52.000000 dgg-bot-1.1.0/dggbot/user.py
+-rw-rw-rw-   0        0        0     2578 2023-05-26 10:38:55.000000 dgg-bot-1.1.0/dggbot/wsbase.py
+-rw-rw-rw-   0        0        0     1238 2023-05-26 21:35:47.000000 dgg-bot-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       41 2023-05-26 14:11:03.000000 dgg-bot-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.697720 dgg-bot-1.1.0/tests/
+-rw-rw-rw-   0        0        0      586 2023-05-28 00:09:42.000000 dgg-bot-1.1.0/tests/test_chat.py
```

### Comparing `dgg-bot-1.0.0/LICENSE` & `dgg-bot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/PKG-INFO` & `dgg-bot-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgg-bot-1.0.0/README.rst` & `dgg-bot-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/dgg_bot.egg-info/PKG-INFO` & `dgg-bot-1.1.0/dgg_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgg-bot-1.0.0/dggbot/bot.py` & `dgg-bot-1.1.0/dggbot/bot.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/dggbot/chat.py` & `dgg-bot-1.1.0/dggbot/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime, timezone
 import json
 import requests
 from typing import Union
 
 from ._logging import _logger
 from .event import EventType
 from .flairs import Flair, flair_converter, convert_flairs
@@ -10,14 +9,20 @@
 from .message import (
     Message,
     MuteMessage,
     PinnedMessage,
     PollMessage,
     PrivateMessage,
     VoteMessage,
+    SubscriptionMessage,
+    MassGiftMessage,
+    GiftSubMessage,
+    DonationMessage,
+    BroadcastMessage,
+    convert_datetime,
 )
 from .user import User
 from .wsbase import WSBase
 from .errors import (
     AccountTooYoung,
     Banned,
     DuplicateMessage,
@@ -133,27 +138,38 @@
     def _on_message(self, ws, message: str):
         event_type, data = message.split(maxsplit=1)
         data = json.loads(data)
         if event_type == EventType.ME:
             _logger.debug(f"{event_type} {data}")
             if data is not None:
                 self.user = User(
-                    data["ID"],
+                    data["id"],
                     data["nick"],
+                    convert_datetime(data.get("createdDate")),
                     convert_flairs(self._flairs, data.get("features")),
                 )
             else:
                 self.user = None
             return
         elif event_type == EventType.MUTE:
             msg = MuteMessage(self, event_type, data)
         elif event_type == EventType.PRIVMSG:
             msg = PrivateMessage(self, event_type, data)
         elif event_type == EventType.PRIVMSGSENT:
             return
+        elif event_type == EventType.SUBSCRIPTION:
+            msg = SubscriptionMessage(self, event_type, data)
+        elif event_type == EventType.MASSGIFT:
+            msg = MassGiftMessage(self, event_type, data)
+        elif event_type == EventType.GIFTSUB:
+            msg = GiftSubMessage(self, event_type, data)
+        elif event_type == EventType.DONATION:
+            msg = DonationMessage(self, event_type, data)
+        elif event_type == EventType.BROADCAST:
+            msg = BroadcastMessage(self, event_type, data)
         elif event_type == EventType.ERROR:
             if (desc := data["description"]) in self._err_dict:
                 raise self._err_dict[desc]
             else:
                 _logger.error(event_type, data)
                 raise Exception(desc)
         elif event_type == EventType.NAMES:
@@ -168,15 +184,14 @@
             msg = VoteMessage(self, event_type, data)
         else:
             msg = Message(self, event_type, data)
         if event_type == EventType.QUIT:
             self._users.pop(msg.nick_lower, None)
         elif event_type == EventType.JOIN:
             self._users[msg.nick_lower] = msg.user
-        print(msg)
 
         self.on_event(event_type.lower(), msg)
         if event_type in (EventType.MESSAGE, EventType.PRIVMSG) and self.is_mentioned(
             msg
         ):
             self.on_event("mention", msg)
         self._post_message(msg)
@@ -203,23 +218,29 @@
         )
 
     @threaded
     def on_names(self, connection_count: int, users: list):
         """Do stuff when the NAMES message is received upon connecting to chat."""
         self._users = {
             user["nick"].lower(): User(
-                user.get("ID"),
+                user.get("id"),
                 user.get("nick"),
+                convert_datetime(user.get("createdDate")),
                 convert_flairs(self._flairs, user.get("features")),
             )
             for user in users
         }
         self.on_event("names", connection_count, self._users)
 
     @threaded
+    def send_raw(self, event_type: str, payload: dict):
+        """Send the specified event_type and payload."""
+        self.ws.send(f"{event_type} {json.dumps(payload)}")
+
+    @threaded
     def send(self, msg: str):
         """Send a message to chat."""
         assert len(msg) <= 512, "512 character limit broken"
         payload = {"data": msg}
         self.ws.send(f"MSG {json.dumps(payload)}")
 
     @threaded
```

### Comparing `dgg-bot-1.0.0/dggbot/event.py` & `dgg-bot-1.1.0/dggbot/event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from functools import cache
 
 
 class EventType:
     BAN = "BAN"
     BROADCAST = "BROADCAST"
+    DONATION = "DONATION"
     ERROR = "ERR"
+    GIFTSUB = "GIFTSUB"
     JOIN = "JOIN"
+    MASSGIFT = "MASSGIFT"
     ME = "ME"
     MESSAGE = "MSG"
     MUTE = "MUTE"
     NAMES = "NAMES"
     PIN = "PIN"
     POLLSTART = "POLLSTART"
     POLLSTOP = "POLLSTOP"
     PRIVMSG = "PRIVMSG"
     PRIVMSGSENT = "PRIVMSGSENT"
     QUIT = "QUIT"
     REFRESH = "REFRESH"
     SUBONLY = "SUBONLY"
+    SUBSCRIPTION = "SUBSCRIPTION"
     UNBAN = "UNBAN"
     UNMUTE = "UNMUTE"
     VOTECAST = "VOTECAST"
 
     @classmethod
     @cache
     def types(cls) -> tuple[str]:
```

### Comparing `dgg-bot-1.0.0/dggbot/flairs.py` & `dgg-bot-1.1.0/dggbot/flairs.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/dggbot/live/__init__.py` & `dgg-bot-1.1.0/dggbot/live/__init__.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/dggbot/live/message.py` & `dgg-bot-1.1.0/dggbot/live/message.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/dggbot/message.py` & `dgg-bot-1.1.0/dggbot/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 from typing import Union, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .chat import DGGChat
 
 
 def convert_datetime(dt_string: str) -> datetime:
-    # DGG returns a string with 9 microsecond digits, while datetime only goes up to 6. So the last 3 are cut off.
-    dt = datetime.strptime(f"{dt_string[:-4]}Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+    if (n := len(dt_string)) == 20:  # seconds given
+        dt = datetime.strptime(dt_string, "%Y-%m-%dT%H:%M:%SZ")
+    elif n <= 27:  # microseconds given
+        dt = datetime.strptime(dt_string, "%Y-%m-%dT%H:%M:%S.%fZ")
+    else:  # if more than 6 digits for microseconds is given, do not include them. Datetime only allows up to 6
+        dt = datetime.strptime(dt_string[:26] + "Z", "%Y-%m-%dT%H:%M:%S.%fZ")
     return dt
 
 
 def convert_timestamp(ts: int) -> datetime:
     """ts: timestamp (in microseconds)"""
     return datetime.fromtimestamp(ts // 1000, tz=timezone.utc)
 
@@ -29,16 +33,17 @@
         self.nick: str = data.get("nick")
         self._data = data
 
     def get(self, key: str):
         return self._data.get(key)
 
     @property
-    def nick_lower(self) -> str:
-        return self.nick.lower()
+    def nick_lower(self) -> Union[str, None]:
+        if self.nick:
+            return self.nick.lower()
 
     def __post_init__(self):
         _logger.debug(self)
 
     def __repr__(self):
         return (
             f"""{self.__class__.__name__}"""
@@ -47,24 +52,21 @@
 
 
 class Message(_MessageBase):
     def __init__(self, chat: DGGChat, type_: str, data: dict):
         super().__init__(chat, type_, data)
         self.id: int = data.get("ID")
         self.features: list[Flair] = convert_flairs(chat._flairs, data.get("features"))
-        self.last_message: str = data.get("Lastmessage")
-        self.last_message_time: datetime = convert_datetime(data.get("Lastmessagetime"))
-        self.delay_scale: int = data.get("Delayscale")
-        self.connections: int = data.get("Connections")
+        self.created_date = convert_datetime(data.get("createdDate"))
         self.timestamp = convert_timestamp(data.get("timestamp"))
         self.data: str = data.get("data")
 
     @property
     def user(self) -> User:
-        return User(self.id, self.nick, self.features)
+        return User(self.id, self.nick, self.created_date, self.features)
 
     def reply(self, content):
         self.chat.send(content)
 
 
 class MuteMessage(Message):
     def __init__(self, chat: DGGChat, type_: str, data: dict):
@@ -89,14 +91,55 @@
 
 class PinnedMessage(Message):
     def __init__(self, chat: DGGChat, type_: str, data: dict):
         super().__init__(chat, type_, data)
         self.uuid: str = data.get("uuid")
 
 
+class BroadcastMessage(_MessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.data: str = data.get("data")
+
+
+class _SubMessageBase(_MessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.timestamp = convert_timestamp(data.get("timestamp"))
+        self.data: str = data.get("data")
+        self.tier: int = data.get("tier")
+        self.tier_label: str = data.get("tierLabel")
+
+
+class SubscriptionMessage(_SubMessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.streak: int = data.get("streak")
+
+
+class MassGiftMessage(_SubMessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.quantity: int = data.get("quantity")
+
+
+class GiftSubMessage(_SubMessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.giftee: int = data.get("giftee")
+
+
+class DonationMessage(_MessageBase):
+    def __init__(self, chat: DGGChat, type_: str, data: dict):
+        super().__init__(chat, type_, data)
+        self.timestamp = convert_timestamp(data.get("timestamp"))
+        self.data: str = data.get("data")
+        self.amount: int = data.get("amount")  # in US cents
+
+
 class PollMessage(_MessageBase):
     def __init__(self, chat: DGGChat, type_: str, data: dict):
         super().__init__(chat, type_, data)
         self.can_vote: bool = data.get("canvote")
         self.my_vote: int = data.get("myvote")
         self.weighted: bool = data.get("weighted")
         self.start: datetime = convert_datetime(data.get("start"))
```

### Comparing `dgg-bot-1.0.0/dggbot/wsbase.py` & `dgg-bot-1.1.0/dggbot/wsbase.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.0.0/pyproject.toml` & `dgg-bot-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 dynamic = ["dependencies", "version"]
 
 [project.urls]
 "Homepage" = "https://github.com/Fritz-02/dgg-bot/"
 "Bug Tracker" = "https://github.com/Fritz-02/dgg-bot/issues"
 
 [project.optional-dependencies]
-dev = ["black", "flake8"]
+dev = ["black", "flake8", "python-dotenv"]
 
 [tool.black]
 line-length = 88
 target-version = ['py39']
 
 [tool.isort]
 profile = "black"
```

