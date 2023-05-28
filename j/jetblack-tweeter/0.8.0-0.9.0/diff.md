# Comparing `tmp/jetblack-tweeter-0.8.0.tar.gz` & `tmp/jetblack-tweeter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetblack-tweeter-0.8.0.tar", max compression
+gzip compressed data, was "jetblack-tweeter-0.9.0.tar", max compression
```

## Comparing `jetblack-tweeter-0.8.0.tar` & `jetblack-tweeter-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     2211 2022-02-02 11:16:57.586117 jetblack-tweeter-0.8.0/README.md
--rw-r--r--   0        0        0      127 2022-03-19 08:04:48.483929 jetblack-tweeter-0.8.0/jetblack_tweeter/__init__.py
--rw-r--r--   0        0        0      199 2022-02-02 11:16:57.599695 jetblack-tweeter-0.8.0/jetblack_tweeter/api/__init__.py
--rw-r--r--   0        0        0     2978 2022-03-19 08:02:31.191251 jetblack-tweeter-0.8.0/jetblack_tweeter/api/account.py
--rw-r--r--   0        0        0     5426 2022-03-19 08:03:29.497590 jetblack-tweeter-0.8.0/jetblack_tweeter/api/search.py
--rw-r--r--   0        0        0    29784 2022-03-19 07:55:48.269348 jetblack-tweeter-0.8.0/jetblack_tweeter/api/statuses.py
--rw-r--r--   0        0        0     3404 2022-02-02 11:16:57.600126 jetblack-tweeter-0.8.0/jetblack_tweeter/api/stream.py
--rw-r--r--   0        0        0     3201 2022-03-19 07:57:51.470017 jetblack-tweeter-0.8.0/jetblack_tweeter/auth_client.py
--rw-r--r--   0        0        0        0 2022-02-02 11:16:57.600265 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/__init__.py
--rw-r--r--   0        0        0      113 2022-02-02 11:16:57.600371 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/aiohttp/__init__.py
--rw-r--r--   0        0        0     2637 2022-03-19 07:58:51.346424 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/aiohttp/session.py
--rw-r--r--   0        0        0       80 2022-02-02 11:16:57.600595 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/bareclient/__init__.py
--rw-r--r--   0        0        0     3590 2022-03-19 07:58:14.617596 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/bareclient/session.py
--rw-r--r--   0        0        0      522 2022-02-02 11:16:57.600745 jetblack-tweeter-0.8.0/jetblack_tweeter/clients/bareclient/utils.py
--rw-r--r--   0        0        0      111 2022-02-02 11:16:57.600808 jetblack-tweeter-0.8.0/jetblack_tweeter/constants.py
--rw-r--r--   0        0        0     2030 2022-02-02 11:16:57.600901 jetblack-tweeter-0.8.0/jetblack_tweeter/errors.py
--rw-r--r--   0        0        0       10 2022-02-02 11:16:57.600962 jetblack-tweeter-0.8.0/jetblack_tweeter/py.typed
--rw-r--r--   0        0        0     2273 2022-02-02 11:16:57.601044 jetblack-tweeter-0.8.0/jetblack_tweeter/tweeter.py
--rw-r--r--   0        0        0     6355 2022-03-19 07:57:06.674322 jetblack-tweeter-0.8.0/jetblack_tweeter/types.py
--rw-r--r--   0        0        0     2288 2022-02-02 11:16:57.601192 jetblack-tweeter-0.8.0/jetblack_tweeter/utils.py
--rw-r--r--   0        0        0      835 2022-03-19 08:05:25.921786 jetblack-tweeter-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3247 2022-03-19 08:07:47.064812 jetblack-tweeter-0.8.0/setup.py
--rw-r--r--   0        0        0     3064 2022-03-19 08:07:47.065039 jetblack-tweeter-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2211 2022-02-02 07:10:12.523138 jetblack-tweeter-0.9.0/README.md
+-rw-r--r--   0        0        0      127 2023-05-28 08:48:27.772514 jetblack-tweeter-0.9.0/jetblack_tweeter/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-28 09:29:18.738926 jetblack-tweeter-0.9.0/jetblack_tweeter/api/__init__.py
+-rw-r--r--   0        0        0     2978 2023-05-28 08:48:27.772790 jetblack-tweeter-0.9.0/jetblack_tweeter/api/account.py
+-rw-r--r--   0        0        0     5426 2023-05-28 08:48:27.773007 jetblack-tweeter-0.9.0/jetblack_tweeter/api/search.py
+-rw-r--r--   0        0        0    29784 2023-05-28 08:48:27.773309 jetblack-tweeter-0.9.0/jetblack_tweeter/api/statuses.py
+-rw-r--r--   0        0        0     3404 2022-02-02 07:10:12.537759 jetblack-tweeter-0.9.0/jetblack_tweeter/api/stream.py
+-rw-r--r--   0        0        0     7592 2023-05-28 09:28:16.668599 jetblack-tweeter-0.9.0/jetblack_tweeter/api/tweets.py
+-rw-r--r--   0        0        0    25766 2023-05-28 09:06:27.362739 jetblack-tweeter-0.9.0/jetblack_tweeter/api/users.py
+-rw-r--r--   0        0        0     4348 2023-05-28 08:52:57.823445 jetblack-tweeter-0.9.0/jetblack_tweeter/auth_client.py
+-rw-r--r--   0        0        0        0 2022-02-02 07:10:12.537903 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/__init__.py
+-rw-r--r--   0        0        0      113 2022-02-02 07:10:12.538004 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/aiohttp/__init__.py
+-rw-r--r--   0        0        0     3871 2023-05-28 08:54:06.988788 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/aiohttp/session.py
+-rw-r--r--   0        0        0       80 2022-02-02 07:10:12.538184 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/bareclient/__init__.py
+-rw-r--r--   0        0        0     6730 2023-05-28 08:54:46.745577 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/bareclient/session.py
+-rw-r--r--   0        0        0      522 2022-02-02 07:47:17.694098 jetblack-tweeter-0.9.0/jetblack_tweeter/clients/bareclient/utils.py
+-rw-r--r--   0        0        0      151 2023-05-28 06:44:15.959121 jetblack-tweeter-0.9.0/jetblack_tweeter/constants.py
+-rw-r--r--   0        0        0     2030 2022-02-02 07:10:12.538477 jetblack-tweeter-0.9.0/jetblack_tweeter/errors.py
+-rw-r--r--   0        0        0       10 2022-02-02 07:10:12.538537 jetblack-tweeter-0.9.0/jetblack_tweeter/py.typed
+-rw-r--r--   0        0        0     2494 2023-05-28 09:30:09.484548 jetblack-tweeter-0.9.0/jetblack_tweeter/tweeter.py
+-rw-r--r--   0        0        0    10027 2023-05-28 09:05:38.966183 jetblack-tweeter-0.9.0/jetblack_tweeter/types.py
+-rw-r--r--   0        0        0     2316 2023-05-28 06:55:19.008098 jetblack-tweeter-0.9.0/jetblack_tweeter/utils.py
+-rw-r--r--   0        0        0      835 2023-05-28 09:33:08.196780 jetblack-tweeter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3247 2023-05-28 09:34:36.511984 jetblack-tweeter-0.9.0/setup.py
+-rw-r--r--   0        0        0     3064 2023-05-28 09:34:36.512231 jetblack-tweeter-0.9.0/PKG-INFO
```

### Comparing `jetblack-tweeter-0.8.0/README.md` & `jetblack-tweeter-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/api/account.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/api/account.py`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/api/search.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/api/search.py`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/api/statuses.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/api/statuses.py`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/api/stream.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/api/stream.py`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/auth_client.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/auth_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """An HTTP client which uses oauth1 for authentication"""
 
+import json
 from typing import Any, AsyncIterator, List, Mapping, Optional, Union
 from urllib.parse import urlencode
 
 from oauthlib.oauth1 import Client as OAuth1Client
 
 from .types import AbstractHttpClient, AbstractTweeterSession
 from .utils import clean_optional_dict, clean_dict
@@ -78,15 +79,44 @@
     async def post(
             self,
             url: str,
             params: Optional[Mapping[str, Any]] = None,
             timeout: Optional[float] = None
     ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
         data = clean_optional_dict(params)
+        body = None if data is None else json.dumps(data)
         url, headers, _ = self._oauth_client.sign(
             url + (f'?{urlencode(data)}' if data else ''),
             http_method='POST'
         )
-        return await self._client.post(url, headers, None, timeout)
+        return await self._client.post(url, headers, body, timeout)
+
+    async def put(
+            self,
+            url: str,
+            params: Optional[Mapping[str, Any]] = None,
+            timeout: Optional[float] = None
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        data = clean_optional_dict(params)
+        body = None if data is None else json.dumps(data)
+        url, headers, _ = self._oauth_client.sign(
+            url + (f'?{urlencode(data)}' if data else ''),
+            http_method='PUT'
+        )
+        return await self._client.put(url, headers, body, timeout)
+
+    async def delete(
+            self,
+            url: str,
+            params: Optional[Mapping[str, Any]] = None,
+            timeout: Optional[float] = None
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        data = clean_optional_dict(params)
+        body = None if data is None else json.dumps(data)
+        url, headers, _ = self._oauth_client.sign(
+            url + (f'?{urlencode(data)}' if data else ''),
+            http_method='DELETE'
+        )
+        return await self._client.delete(url, headers, body, timeout)
 
     async def close(self) -> None:
         await self._client.close()
```

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/clients/aiohttp/session.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/clients/aiohttp/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from typing import Any, AsyncIterator, List, Mapping, Optional, Union
 
 from aiohttp import ClientSession, Fingerprint, ClientTimeout
 
 from ...errors import ApiError
 from ...types import AbstractTweeterSession
 
+
 def _make_timeout(timeout: Optional[float]) -> Optional[ClientTimeout]:
     if timeout is None:
         return None
     else:
         return ClientTimeout(total=timeout)
 
+
 class AiohttpTweeterSession(AbstractTweeterSession):
     """A tweeter session using aiohttp."""
 
     def __init__(
             self,
             *,
             ssl: Optional[Union[SSLContext, bool, Fingerprint]] = None
@@ -77,11 +79,49 @@
                 url,
                 headers=headers,
                 data=data,
                 ssl=self._ssl,
                 timeout=client_timeout
         ) as response:
             response.raise_for_status()
+            return await response.json()
+
+    async def put(
+            self,
+            url: str,
+            headers: Mapping[str, str],
+            body: Optional[str],
+            timeout: Optional[float]
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        client_timeout = _make_timeout(timeout)
+        data = body.encode() if body else None
+        async with self._client.put(
+                url,
+                headers=headers,
+                data=data,
+                ssl=self._ssl,
+                timeout=client_timeout
+        ) as response:
+            response.raise_for_status()
+            return await response.json()
+
+    async def delete(
+            self,
+            url: str,
+            headers: Mapping[str, str],
+            body: Optional[str],
+            timeout: Optional[float]
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        client_timeout = _make_timeout(timeout)
+        data = body.encode() if body else None
+        async with self._client.delete(
+                url,
+                headers=headers,
+                data=data,
+                ssl=self._ssl,
+                timeout=client_timeout
+        ) as response:
+            response.raise_for_status()
             return await response.json()
 
     async def close(self) -> None:
         await self._client.close()
```

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/clients/bareclient/utils.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/clients/bareclient/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities for sessions"""
 
 from typing import List, Mapping, Tuple
 
-from baretypes import Header
+Header = Tuple[bytes, bytes]
 
 
 def to_lines(buf) -> Tuple[List[bytes], bytes]:
     lines: List[bytes] = []
     sep = b'\r\n'
     while sep:
         line, sep, rest = buf.partition(sep)
```

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/errors.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/errors.py`

 * *Files identical despite different names*

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/tweeter.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/tweeter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from types import TracebackType
 from typing import Optional, Type, TypeVar
 
 from .auth_client import AuthenticatedHttpClient
-from .api import Account, Search, Stream, Statuses
+from .api import Account, Search, Stream, Statuses, Tweets, Users
 from .types import AbstractTweeterSession
 
 TException = TypeVar('TException', bound=BaseException)
 
 
 class Tweeter:
     """The Twitter client.
@@ -37,26 +37,30 @@
                 token secret. Defaults to None.
 
         Attributes:
             account (Account): Access to the account end point.
             search (Search): Access to the search end point.
             statuses (Statuses): Access to the statuses end point.
             stream (Stream): Access to the stream end point.
+            tweets (Tweets): Access to the tweets end point.
+            users (Statuses): Access to the users end point.
         """
         self._client = AuthenticatedHttpClient(
             session,
             consumer_key=app_key,
             consumer_secret=app_key_secret,
             access_token=access_token,
             access_token_secret=access_token_secret
         )
         self.account = Account(self._client)
         self.search = Search(self._client)
         self.statuses = Statuses(self._client)
         self.stream = Stream(self._client)
+        self.tweets = Tweets(self._client)
+        self.users = Users(self._client)
 
     async def __aenter__(self) -> Tweeter:
         return self
 
     async def __aexit__(
             self,
             exec_type: Optional[Type[TException]],
```

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/types.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 from typing import (
     Any,
     AsyncIterator,
     List,
+    Literal,
     Mapping,
     Optional,
     TypedDict,
     Tuple,
     Union
 )
 
@@ -82,14 +83,56 @@
 
         Returns:
             Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
                 response (if any).
         """
 
     @abstractmethod
+    async def put(
+            self,
+            url: str,
+            headers: Mapping[str, str],
+            body: Optional[str],
+            timeout: Optional[float]
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        """Put data to Twitter
+
+        Args:
+            url (str): The url
+            headers (Mapping[str, str]): The HTTP headers
+            body (Optional[str]): The body (if any)
+            timeout (Optional[float]): An optional timeout.
+
+        Returns:
+            Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
+                response (if any).
+        """
+
+    @abstractmethod
+    async def delete(
+            self,
+            url: str,
+            headers: Mapping[str, str],
+            body: Optional[str],
+            timeout: Optional[float]
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        """Delete data in Twitter
+
+        Args:
+            url (str): The url
+            headers (Mapping[str, str]): The HTTP headers
+            body (Optional[str]): The body (if any),
+            timeout (Optional[float]): An optional timeout.
+
+        Returns:
+            Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
+                response (if any).
+        """
+
+    @abstractmethod
     async def close(self) -> None:
         """Close the connection.
         """
 
 
 class AbstractHttpClient(metaclass=ABCMeta):
     """The abstract class for HTTP clients.
@@ -142,15 +185,53 @@
             params: Optional[Mapping[str, Any]] = None,
             timeout: Optional[float] = None
     ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
         """Post data to Twitter.
 
         Args:
             url (str): The url
-            params (Optional[Mapping[str, Any]], optional): The parameters if
+            params (Optional[Mapping[str, Any]], optional): The params if
+                any. Defaults to None.
+
+        Returns:
+            Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
+                response if any
+        """
+
+    @ abstractmethod
+    async def put(
+            self,
+            url: str,
+            params: Optional[Mapping[str, Any]] = None,
+            timeout: Optional[float] = None
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        """Put data to Twitter.
+
+        Args:
+            url (str): The url
+            params (Optional[Mapping[str, Any]], optional): The params if
+                any. Defaults to None.
+
+        Returns:
+            Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
+                response if any
+        """
+
+    @ abstractmethod
+    async def delete(
+            self,
+            url: str,
+            params: Optional[Mapping[str, Any]] = None,
+            timeout: Optional[float] = None
+    ) -> Optional[Union[List[Any], Mapping[str, Any]]]:
+        """Delete data from Twitter.
+
+        Args:
+            url (str): The url
+            params (Optional[Mapping[str, Any]], optional): The params if
                 any. Defaults to None.
             timeout (Optional[float], optional): The timeout if any. Defaults
                 to None.
 
         Returns:
             Optional[Union[List[Any], Mapping[str, Any]]]: The unpacked JSON
                 response if any
@@ -239,7 +320,81 @@
     in_reply_to_status_id: Optional[int]
     in_reply_to_status_id_str: Optional[str]
     in_reply_to_user_id: Optional[int]
     in_reply_to_user_id_str: Optional[str]
     in_reply_to_screen_name: Optional[str]
     user: UserObject
     coordinates: CoordinatesObject
+
+
+MediaFields = Literal[
+    "duration_ms",
+    "height",
+    'media_key',
+    "preview_image_url",
+    "type",
+    "url",
+    "width",
+    "public_metrics",
+    "non_public_metrics",
+    "organic_metrics",
+    "promoted_metrics",
+    "alt_text",
+    "variants"
+]
+PollFields = Literal[
+    "duration_minutes",
+    "end_datetime",
+    "id",
+    "options",
+    "voting_status"
+]
+TweetFields = Literal[
+    "attachments",
+    "author_id",
+    "context_annotations",
+    "conversation_id",
+    "created_at",
+    "edit_controls",
+    "entities",
+    "geo",
+    "id",
+    "in_reply_to_user_id",
+    "lang",
+    "non_public_metrics",
+    "public_metrics",
+    "organic_metrics",
+    "promoted_metrics",
+    "possibly_sensitive",
+    "referenced_tweets",
+    "reply_settings",
+    "source",
+    "text",
+    "withheld"
+]
+UserFields = Literal[
+    "created_at",
+    "description",
+    "entities",
+    "id",
+    "location",
+    "name",
+    "pinned_tweet_id",
+    "profile_image_url",
+    "protected",
+    "public_metrics",
+    "url",
+    "username",
+    "verified",
+    "verified_type",
+    "withheld"
+]
+PlaceFields = Literal[
+    "contained_within",
+    "country",
+    "country_code",
+    "full_name",
+    "geo",
+    "id",
+    "name",
+    "place_type"
+]
```

### Comparing `jetblack-tweeter-0.8.0/jetblack_tweeter/utils.py` & `jetblack-tweeter-0.9.0/jetblack_tweeter/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Utilities"""
 
-from typing import Any, List, Mapping, Optional
+from typing import Any, Mapping, Optional, Sequence
 
 from .types import BoundingBox, Location
 
 
-def str_list_to_str(values: List[str]) -> str:
+def str_list_to_str(values: Sequence[str]) -> str:
     return ','.join(values)
 
 
 def optional_str_list_to_str(
-        values: Optional[List[str]],
+        values: Optional[Sequence[str]],
         default: Optional[str] = None
 ) -> Optional[str]:
     return str_list_to_str(values) if values else default
 
 
-def int_list_to_str(values: List[int]) -> str:
+def int_list_to_str(values: Sequence[int]) -> str:
     return ','.join(
         str(value)
         for value in values
     )
 
 
 def optional_int_list_to_str(
-        values: Optional[List[int]],
+        values: Optional[Sequence[int]],
         default: Optional[str] = None
 ) -> Optional[str]:
     return int_list_to_str(values) if values else default
 
 
 def clean_dict(data: Mapping[str, Any]) -> Mapping[str, Any]:
     return {
@@ -75,16 +75,16 @@
 def optional_bounding_box_to_str(
         value: Optional[BoundingBox],
         default: Optional[str] = None
 ) -> Optional[str]:
     return bounding_box_to_str(value) if value is not None else default
 
 
-def bounding_box_list_to_str(value: List[BoundingBox]) -> str:
+def bounding_box_list_to_str(value: Sequence[BoundingBox]) -> str:
     return ",".join(bounding_box_to_str(x) for x in value)
 
 
 def optional_bounding_box_list_to_str(
-        value: Optional[List[BoundingBox]],
+        value: Optional[Sequence[BoundingBox]],
         default: Optional[str] = None
 ) -> Optional[str]:
     return bounding_box_list_to_str(value) if value is not None else default
```

### Comparing `jetblack-tweeter-0.8.0/pyproject.toml` & `jetblack-tweeter-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "jetblack-tweeter"
-version = "0.8.0"
+version = "0.9.0"
 description = "An asyncio twitter client"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "jetblack_tweeter" }
 ]
 repository = "https://github.com/rob-blackbourn/jetblack-tweeter"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 oauthlib = "^3.1"
-bareclient = { version = "^4.6", optional = true }
-aiohttp = { version = "^3.7", optional = true }
+bareclient = { version = "^5.0", optional = true }
+aiohttp = { version = "^3.8", optional = true }
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.910"
 pylint = "^2.7"
 autopep8 = "^1.5.4"
 pytest = "^6.1.1"
 mkdocs = "^1.0.4"
```

### Comparing `jetblack-tweeter-0.8.0/setup.py` & `jetblack-tweeter-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['oauthlib>=3.1,<4.0']
 
 extras_require = \
-{'aiohttp': ['aiohttp>=3.7,<4.0'], 'bareclient': ['bareclient>=4.6,<5.0']}
+{'aiohttp': ['aiohttp>=3.8,<4.0'], 'bareclient': ['bareclient>=5.0,<6.0']}
 
 setup_kwargs = {
     'name': 'jetblack-tweeter',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'An asyncio twitter client',
     'long_description': '# jetblack-tweeter\n\nA Python 3.8 asyncio twitter client.\n\nThis Twitter client is designed to support arbitrary HTTP clients. There is\ncurrently support for\n[bareClient](https://rob-blackbourn.github.io/bareClient/api/bareclient/)\nand [aiohttp](https://docs.aiohttp.org/en/stable/index.html).\n\n## Status\n\nThis is work in progress, but functional.\n\nThere is currently limited support for streaming, statuses and accounts. Only the 1.1 api is currently implemented.\n\n## Installation\n\nInstall with `pip`, specifying the HTTP backend you wish to use.\n\nFor bareClient:\n\n```bash\npip install jetblack-tweeter[bareclient]\n```\n\nFor aiohttp:\n\n```bash\npip install jetblack-tweeter[aiohttp]\n```\n\n## Usage\n\nHere is an example:\n\n```python\nimport asyncio\nimport os\n\nfrom jetblack_tweeter import Tweeter\nfrom jetblack_tweeter.clients.bareclient import BareTweeterSession\n\n# Get the secrets from environment variables.\nAPP_KEY = os.environ["APP_KEY"]\nAPP_KEY_SECRET = os.environ["APP_KEY_SECRET"]\nACCESS_TOKEN = os.environ["ACCESS_TOKEN"]\nACCESS_TOKEN_SECRET = os.environ["ACCESS_TOKEN_SECRET"]\n\n\nasync def main():\n    tweeter = Tweeter(\n        BareTweeterSession(),\n        APP_KEY,\n        APP_KEY_SECRET,\n        # Optional for user authentication.\n        access_token=ACCESS_TOKEN,\n        access_token_secret=ACCESS_TOKEN_SECRET\n    )\n\n    user_timeline = await tweeter.statuses.user_timeline()\n    print(user_timeline)\n\n    account_settings = await tweeter.account.settings()\n    print(account_settings)\n\n    account_verify_credentials = await tweeter.account.verify_credentials()\n    print(account_verify_credentials)\n\n    # Watch the random sampling of tweets chosen by twitter\n    async for tweet in tweeter.stream.sample():\n        print(tweet)\n\n    # Stream tweets which have the tag "#python" from New York\n    # and San Francisco.\n    async for tweet in tweeter.stream.filter(\n            track=[\'#python\'],\n            locations=[\n                ((-122.75, 36.8), (-121.75, 37.8)),\n                ((-74, 40), (-73, 41))\n            ]\n    ):\n        print(tweet)\n\n    result = await tweeter.statuses.update(\'Hello from jetblack-tweeter\')\n    print(result)\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rob-blackbourn/jetblack-tweeter',
```

### Comparing `jetblack-tweeter-0.8.0/PKG-INFO` & `jetblack-tweeter-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: jetblack-tweeter
-Version: 0.8.0
+Version: 0.9.0
 Summary: An asyncio twitter client
 Home-page: https://github.com/rob-blackbourn/jetblack-tweeter
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: aiohttp
 Provides-Extra: bareclient
-Requires-Dist: aiohttp (>=3.7,<4.0); extra == "aiohttp"
-Requires-Dist: bareclient (>=4.6,<5.0); extra == "bareclient"
+Requires-Dist: aiohttp (>=3.8,<4.0); extra == "aiohttp"
+Requires-Dist: bareclient (>=5.0,<6.0); extra == "bareclient"
 Requires-Dist: oauthlib (>=3.1,<4.0)
 Project-URL: Repository, https://github.com/rob-blackbourn/jetblack-tweeter
 Description-Content-Type: text/markdown
 
 # jetblack-tweeter
 
 A Python 3.8 asyncio twitter client.
```

