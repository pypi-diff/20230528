# Comparing `tmp/pyzoom-0.1.9.tar.gz` & `tmp/pyzoom-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzoom-0.1.9.tar", max compression
+gzip compressed data, was "pyzoom-1.0.0.tar", max compression
```

## Comparing `pyzoom-0.1.9.tar` & `pyzoom-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     3318 2021-07-19 07:14:03.725320 pyzoom-0.1.9/README.md
--rw-r--r--   0        0        0      580 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       50 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyzoom/__init__.py
--rw-r--r--   0        0        0     4719 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyzoom/_base.py
--rw-r--r--   0        0        0     5167 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyzoom/_client.py
--rw-r--r--   0        0        0      438 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyzoom/err.py
--rw-r--r--   0        0        0     4347 2021-07-19 07:14:03.725320 pyzoom-0.1.9/pyzoom/schemas.py
--rw-r--r--   0        0        0     4226 2021-07-19 07:14:12.206870 pyzoom-0.1.9/setup.py
--rw-r--r--   0        0        0     4106 2021-07-19 07:14:12.207244 pyzoom-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     4279 2023-05-28 14:31:58.813129 pyzoom-1.0.0/README.md
+-rw-r--r--   0        0        0      567 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyzoom/__init__.py
+-rw-r--r--   0        0        0     4534 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyzoom/_base.py
+-rw-r--r--   0        0        0     7287 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyzoom/_client.py
+-rw-r--r--   0        0        0      438 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyzoom/err.py
+-rw-r--r--   0        0        0     4856 2023-05-28 14:31:58.813129 pyzoom-1.0.0/pyzoom/schemas.py
+-rw-r--r--   0        0        0     5129 1970-01-01 00:00:00.000000 pyzoom-1.0.0/PKG-INFO
```

### Comparing `pyzoom-0.1.9/README.md` & `pyzoom-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,80 @@
 ![Zoom Logo](https://d24cgw3uvb9a9h.cloudfront.net/static/93946/image/new/ZoomLogo.png)
 
+**WARNING: Version 1.0.0 introduces breaking change. The library now only supports OAUTH tokens, since Zoom is deprecating the JWT support as of June 1, 2023**
+
+Also the project now uses [break versioning](https://github.com/ptaoussanis/encore/blob/master/BREAK-VERSIONING.md), meaning that upgrading from 1.0.x to 1.0.y will always be safe, upgrade to 1.x.x might break something small, and upgrade to 2.x.x will break almost everything. That was a versioning spec in one sentence, by the way.
+
 # Python wrapper for Zoom API
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyzoom)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/pyzoom)](https://pypi.org/project/pyzoom/)
 ![PyPI - License](https://img.shields.io/pypi/l/pyzoom)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/pyzoom)
 [![](https://img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/licht1stein)
 
-This library is work in progress, and that includes documentation. Not all of the implemented methods are documented here,
-so please explore the `ZoomClient` class.
+
+**This library requires contributors and maintainers since Python stopped being my primary language a couple of years ago.**
+I do use it in some of my older projects, so I have to update it from time to time.
 
 Links:
 * [Api Reference](https://marketplace.zoom.us/docs/api-reference)
 * [Using Zoom API](https://marketplace.zoom.us/docs/api-reference/using-zoom-apis)
 
 ## Installation
 
 Using pip:
 
 `pip install -U pyzoom`
 
-Using [poetry](https://https://python-poetry.org/):
+Using [poetry](https://python-poetry.org/):
 
 `poetry add pyzoom`
 
 ## Usage
 
 ### Basic instantiation:
 
 ```python
 from pyzoom import ZoomClient
 
-client = ZoomClient('YOUR_ZOOM_API_KEY', 'YOUR_ZOOM_API_SECRET')
+client = ZoomClient('YOUR_ZOOM_ACCESS_TOKEN')
+```
+
+Optionally you can specify a different base URL either upon instantiation or any time later:
+
+```python
+client = ZoomClient ('YOU_ZOOM_ACCCESS_TOKEN', base_url="https://api.zoomgov.us/v2")
 ```
 
 ### Instantiation from environment variables
 
-You can also create an instance of client when storing your key and secret in environment variables `ZOOM_API_KEY` 
-and `ZOOM_API_SECRET`.
+You can also create an instance of client when access key in environment variables `ZOOM_ACCESS_TOIKEN`. *Since the access token expires after one hour, this method is not a good idea any more.*
 
 ```python
 from pyzoom import ZoomClient
 
 client = ZoomClient.from_environment()
 ```
 
 
 ### Meetings
 
-#### Create meeting and add registrant
+#### Create meeting, update meeting and add registrant
 ```python
 from pyzoom import ZoomClient
 from datetime import datetime as dt
 
 client = ZoomClient.from_environment()
 
 # Creating a meeting
 meeting = client.meetings.create_meeting('Auto created 1', start_time=dt.now().isoformat(), duration_min=60, password='not-secure')
 
+# Update a meeting
+meeting = client.meetings.update_meeting('Auto updated 1', meeting_id = meeting.id ,start_time=dt.now().isoformat(), duration_min=60,password='not-secure')
 
 # Adding registrants
 client.meetings.add_meeting_registrant(meeting.id, first_name='John', last_name='Doe', email='john.doe@example.com')
 ```
 You can use `client.meetings.add_and_confirm_registrant` to also confirm auto added
 registrants to a closed meeting.
 
@@ -72,15 +84,15 @@
 
 ```python
 from pyzoom import ZoomClient
 
 client = ZoomClient.from_environment()
 
 # Get self
-response = client.raw.get('/me')
+response = client.raw.get('/users/me')
 
 # Get all pages of meeting participants
 result_dict = client.raw.get_all_pages('/past_meetings/{meetingUUID}/participants')
 ```
 
 ### Packaging notice
 This project uses the excellent [poetry](https://python-poetry.org) for packaging. Please read about it and let's all start using
```

#### html2text {}

```diff
@@ -1,39 +1,52 @@
 ![Zoom Logo](https://d24cgw3uvb9a9h.cloudfront.net/static/93946/image/new/
-ZoomLogo.png) # Python wrapper for Zoom API ![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/pyzoom) [![Code style: black](https://
-img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) [![PyPI](https://img.shields.io/pypi/v/pyzoom)](https://pypi.org/
-project/pyzoom/) ![PyPI - License](https://img.shields.io/pypi/l/pyzoom) ![PyPI
-- Downloads](https://img.shields.io/pypi/dw/pyzoom) [![](https://
-img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/
-licht1stein) This library is work in progress, and that includes documentation.
-Not all of the implemented methods are documented here, so please explore the
-`ZoomClient` class. Links: * [Api Reference](https://marketplace.zoom.us/docs/
-api-reference) * [Using Zoom API](https://marketplace.zoom.us/docs/api-
-reference/using-zoom-apis) ## Installation Using pip: `pip install -U pyzoom`
-Using [poetry](https://https://python-poetry.org/): `poetry add pyzoom` ##
-Usage ### Basic instantiation: ```python from pyzoom import ZoomClient client =
-ZoomClient('YOUR_ZOOM_API_KEY', 'YOUR_ZOOM_API_SECRET') ``` ### Instantiation
-from environment variables You can also create an instance of client when
-storing your key and secret in environment variables `ZOOM_API_KEY` and
-`ZOOM_API_SECRET`. ```python from pyzoom import ZoomClient client =
-ZoomClient.from_environment() ``` ### Meetings #### Create meeting and add
-registrant ```python from pyzoom import ZoomClient from datetime import
-datetime as dt client = ZoomClient.from_environment() # Creating a meeting
-meeting = client.meetings.create_meeting('Auto created 1', start_time=dt.now
-().isoformat(), duration_min=60, password='not-secure') # Adding registrants
+ZoomLogo.png) **WARNING: Version 1.0.0 introduces breaking change. The library
+now only supports OAUTH tokens, since Zoom is deprecating the JWT support as of
+June 1, 2023** Also the project now uses [break versioning](https://github.com/
+ptaoussanis/encore/blob/master/BREAK-VERSIONING.md), meaning that upgrading
+from 1.0.x to 1.0.y will always be safe, upgrade to 1.x.x might break something
+small, and upgrade to 2.x.x will break almost everything. That was a versioning
+spec in one sentence, by the way. # Python wrapper for Zoom API ![PyPI - Python
+Version](https://img.shields.io/pypi/pyversions/pyzoom) [![Code style: black]
+(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) [![PyPI](https://img.shields.io/pypi/v/pyzoom)](https://
+pypi.org/project/pyzoom/) ![PyPI - License](https://img.shields.io/pypi/l/
+pyzoom) ![PyPI - Downloads](https://img.shields.io/pypi/dw/pyzoom) [![](https:/
+/img.shields.io/badge/Support-Buy_coffee!-Orange)](https://
+www.buymeacoffee.com/licht1stein) **This library requires contributors and
+maintainers since Python stopped being my primary language a couple of years
+ago.** I do use it in some of my older projects, so I have to update it from
+time to time. Links: * [Api Reference](https://marketplace.zoom.us/docs/api-
+reference) * [Using Zoom API](https://marketplace.zoom.us/docs/api-reference/
+using-zoom-apis) ## Installation Using pip: `pip install -U pyzoom` Using
+[poetry](https://python-poetry.org/): `poetry add pyzoom` ## Usage ### Basic
+instantiation: ```python from pyzoom import ZoomClient client = ZoomClient
+('YOUR_ZOOM_ACCESS_TOKEN') ``` Optionally you can specify a different base URL
+either upon instantiation or any time later: ```python client = ZoomClient
+('YOU_ZOOM_ACCCESS_TOKEN', base_url="https://api.zoomgov.us/v2") ``` ###
+Instantiation from environment variables You can also create an instance of
+client when access key in environment variables `ZOOM_ACCESS_TOIKEN`. *Since
+the access token expires after one hour, this method is not a good idea any
+more.* ```python from pyzoom import ZoomClient client =
+ZoomClient.from_environment() ``` ### Meetings #### Create meeting, update
+meeting and add registrant ```python from pyzoom import ZoomClient from
+datetime import datetime as dt client = ZoomClient.from_environment() #
+Creating a meeting meeting = client.meetings.create_meeting('Auto created 1',
+start_time=dt.now().isoformat(), duration_min=60, password='not-secure') #
+Update a meeting meeting = client.meetings.update_meeting('Auto updated 1',
+meeting_id = meeting.id ,start_time=dt.now().isoformat(),
+duration_min=60,password='not-secure') # Adding registrants
 client.meetings.add_meeting_registrant(meeting.id, first_name='John',
 last_name='Doe', email='john.doe@example.com') ``` You can use
 `client.meetings.add_and_confirm_registrant` to also confirm auto added
 registrants to a closed meeting. ### Raw API methods You can also use the
 library for making raw requests to the API: ```python from pyzoom import
 ZoomClient client = ZoomClient.from_environment() # Get self response =
-client.raw.get('/me') # Get all pages of meeting participants result_dict =
-client.raw.get_all_pages('/past_meetings/{meetingUUID}/participants') ``` ###
+client.raw.get('/users/me') # Get all pages of meeting participants result_dict
+= client.raw.get_all_pages('/past_meetings/{meetingUUID}/participants') ``` ###
 Packaging notice This project uses the excellent [poetry](https://python-
 poetry.org) for packaging. Please read about it and let's all start using
 `pyproject.toml` files as a standard. Read more: * [PEP 518 -- Specifying
 Minimum Build System Requirements for Python Projects](https://www.python.org/
 dev/peps/pep-0518/) * [What the heck is pyproject.toml?](https://snarky.ca/
 what-the-heck-is-pyproject-toml/) * [Clarifying PEP 518 (a.k.a.
 pyproject.toml)](https://snarky.ca/clarifying-pep-518/) ### Support [Buy_Me_A
```

### Comparing `pyzoom-0.1.9/pyproject.toml` & `pyzoom-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "pyzoom"
-version = "0.1.9"
+version = "1.0.0"
 description = "Python wrapper for Zoom Video API"
 authors = ["MB <mb@blaster.ai>"]
 license = "MIT"
 readme='README.md'
 homepage='https://github.com/licht1stein/pyzoom'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.23.0"
 attrs = "*"
-pyjwt = ">=2.0,<3.0.0"
-typing-extensions = "^3.7.4"
+typing-extensions = ">=3.7.4,<5.0.0"
 pydantic = "^1.5.1"
-cachetools = "^4.1.0"
+cachetools = ">=4.1,<6.0"
 shortuuid = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2"
-black = "^21.4b2"
-python-dotenv = "^0.17.0"
+pytest = "^7.1"
+black = "^22.6"
+python-dotenv = "^0.21.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pyzoom-0.1.9/pyzoom/_base.py` & `pyzoom-1.0.0/pyzoom/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,65 @@
+from json import JSONDecodeError
 import logging
 import time
 from typing import Dict
 
 import jwt
 import requests
 import attr
 from typing_extensions import Literal
 
 from pyzoom import err
 
 
 @attr.s
 class APIClientBase:
-    api_key: str = attr.ib(repr=False)
-    api_secret: str = attr.ib(repr=False)
+    access_token: str = attr.ib(repr=False)
+    refresh_token: str = attr.ib(repr=False)
+    base_url: str = attr.ib(repr=False, default="https://api.zoom.us/v2")
 
     name = "zoom_api_client"
     user_id: str = "me"
-    base_url: str = "https://api.zoom.us/v2"
-
-    def bearer_token(self) -> str:
-        return self.generate_jwt(self.api_key, self.api_secret)
 
     def make_request(
         self,
         endpoint: str,
         method: Literal["GET", "POST", "PATCH", "DELETE", "PUT"],
         query: Dict = None,
         body: Dict = None,
         raise_on_error=True,
     ) -> requests.Response:
         allowed_methods = "GET POST PATCH DELETE PUT".split()
         if method not in allowed_methods:
             raise ValueError(
                 f'Invalid method: {method}. Must be one of {", ".join(allowed_methods)}'
             )
-        headers = {"Authorization": f"Bearer {self.bearer_token()}"}
+        headers = {"Authorization": f"Bearer {self.access_token}"}
         url = self.base_url + endpoint
         logging.debug(f"Making {method} request to {endpoint}")
         session = requests.Session()
 
         r = session.request(method, url, headers=headers, params=query, json=body)
 
         if 200 <= r.status_code < 300:
             return r
 
         try:
-            message = r.json()["_error"]["message"]
-        except KeyError:
-            message = r.json()
+            body = r.json()
+            try:
+                message = body["_error"]["message"]
+            except KeyError:
+                message = body
+        except JSONDecodeError:
+            body = r.text
+            message = body
 
         logging.error(f"Unsuccessful request to {r.url}: [{r.status_code}] {message}")
 
-        logging.debug(f"Full response: {r.json()}")
+        logging.debug(f"Full response: {body}")
         logging.debug(f"Headers: {r.headers}")
         logging.debug(f"Params: {query}")
         logging.debug(f"Body: {body}")
         if not raise_on_error:
             logging.warning(
                 f"raise_on_error is False, ignoring API error and returning response"
             )
@@ -147,16 +150,7 @@
         return self.make_request(
             endpoint,
             method="DELETE",
             query=query,
             body=body,
             raise_on_error=raise_on_error,
         )
-
-    @staticmethod
-    def generate_jwt(key, secret):
-        header = {"alg": "HS256", "typ": "JWT"}
-
-        payload = {"iss": key, "exp": int(time.time() + 3600)}
-
-        token = jwt.encode(payload, secret, algorithm="HS256", headers=header)
-        return token.decode("utf-8")
```

### Comparing `pyzoom-0.1.9/pyzoom/schemas.py` & `pyzoom-1.0.0/pyzoom/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,7 +167,32 @@
         return [i for i in self.participants if i.id == id_]
 
     def find_by_email(self, email: str) -> List[MeetingParticipant]:
         return [i for i in self.participants if i.user_email == email]
 
     def find_by_name(self, name):
         return [i for i in self.participants if i.name == name]
+
+class ZoomUser(MyZoomBase):
+    id: str
+    first_name: str
+    last_name: str
+    email: str
+    type: int
+    pmi: int
+    timezone: Optional[str]
+    verified: int
+    dept: Optional[str]
+    created_at: str
+    pic_url: Optional[str]
+    group_ids: Optional[List[str]]
+    language: Optional[str]
+    phone_number: Optional[str]
+    status: str
+    role_id: str
+
+class ZoomUserList(MyZoomBase):
+    page_count: int
+    page_number: int
+    page_size: int
+    total_records: int
+    users: List[ZoomUser]
```

### Comparing `pyzoom-0.1.9/PKG-INFO` & `pyzoom-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7a6f  : 2.1.Name: pyzo
-00000020: 6f6d 0a56 6572 7369 6f6e 3a20 302e 312e  om.Version: 0.1.
-00000030: 390a 5375 6d6d 6172 793a 2050 7974 686f  9.Summary: Pytho
+00000020: 6f6d 0a56 6572 7369 6f6e 3a20 312e 302e  om.Version: 1.0.
+00000030: 300a 5375 6d6d 6172 793a 2050 7974 686f  0.Summary: Pytho
 00000040: 6e20 7772 6170 7065 7220 666f 7220 5a6f  n wrapper for Zo
 00000050: 6f6d 2056 6964 656f 2041 5049 0a48 6f6d  om Video API.Hom
 00000060: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000070: 6769 7468 7562 2e63 6f6d 2f6c 6963 6874  github.com/licht
 00000080: 3173 7465 696e 2f70 797a 6f6f 6d0a 4c69  1stein/pyzoom.Li
 00000090: 6365 6e73 653a 204d 4954 0a41 7574 686f  cense: MIT.Autho
 000000a0: 723a 204d 420a 4175 7468 6f72 2d65 6d61  r: MB.Author-ema
@@ -23,235 +23,299 @@
 00000160: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000170: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
 00000180: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000190: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 000001a0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
 000001b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
 000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001d0: 3a3a 2033 2e39 0a52 6571 7569 7265 732d  :: 3.9.Requires-
-000001e0: 4469 7374 3a20 6174 7472 730a 5265 7175  Dist: attrs.Requ
-000001f0: 6972 6573 2d44 6973 743a 2063 6163 6865  ires-Dist: cache
-00000200: 746f 6f6c 7320 283e 3d34 2e31 2e30 2c3c  tools (>=4.1.0,<
-00000210: 352e 302e 3029 0a52 6571 7569 7265 732d  5.0.0).Requires-
-00000220: 4469 7374 3a20 7079 6461 6e74 6963 2028  Dist: pydantic (
-00000230: 3e3d 312e 352e 312c 3c32 2e30 2e30 290a  >=1.5.1,<2.0.0).
-00000240: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000250: 796a 7774 2028 3e3d 322e 302c 3c33 2e30  yjwt (>=2.0,<3.0
-00000260: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000270: 743a 2072 6571 7565 7374 7320 283e 3d32  t: requests (>=2
-00000280: 2e32 332e 302c 3c33 2e30 2e30 290a 5265  .23.0,<3.0.0).Re
-00000290: 7175 6972 6573 2d44 6973 743a 2073 686f  quires-Dist: sho
-000002a0: 7274 7575 6964 2028 3e3d 312e 302e 312c  rtuuid (>=1.0.1,
-000002b0: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
-000002c0: 2d44 6973 743a 2074 7970 696e 672d 6578  -Dist: typing-ex
-000002d0: 7465 6e73 696f 6e73 2028 3e3d 332e 372e  tensions (>=3.7.
-000002e0: 342c 3c34 2e30 2e30 290a 4465 7363 7269  4,<4.0.0).Descri
-000002f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000300: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000310: 6e0a 0a21 5b5a 6f6f 6d20 4c6f 676f 5d28  n..![Zoom Logo](
-00000320: 6874 7470 733a 2f2f 6432 3463 6777 3375  https://d24cgw3u
-00000330: 7662 3961 3968 2e63 6c6f 7564 6672 6f6e  vb9a9h.cloudfron
-00000340: 742e 6e65 742f 7374 6174 6963 2f39 3339  t.net/static/939
-00000350: 3436 2f69 6d61 6765 2f6e 6577 2f5a 6f6f  46/image/new/Zoo
-00000360: 6d4c 6f67 6f2e 706e 6729 0a0a 2320 5079  mLogo.png)..# Py
-00000370: 7468 6f6e 2077 7261 7070 6572 2066 6f72  thon wrapper for
-00000380: 205a 6f6f 6d20 4150 490a 215b 5079 5049   Zoom API.![PyPI
-00000390: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
-000003a0: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-000003b0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-000003c0: 7976 6572 7369 6f6e 732f 7079 7a6f 6f6d  yversions/pyzoom
-000003d0: 290a 5b21 5b43 6f64 6520 7374 796c 653a  ).[![Code style:
-000003e0: 2062 6c61 636b 5d28 6874 7470 733a 2f2f   black](https://
-000003f0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000400: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-00000410: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
-00000420: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000430: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
-00000440: 6b29 0a5b 215b 5079 5049 5d28 6874 7470  k).[![PyPI](http
-00000450: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000460: 696f 2f70 7970 692f 762f 7079 7a6f 6f6d  io/pypi/v/pyzoom
-00000470: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000480: 6f72 672f 7072 6f6a 6563 742f 7079 7a6f  org/project/pyzo
-00000490: 6f6d 2f29 0a21 5b50 7950 4920 2d20 4c69  om/).![PyPI - Li
-000004a0: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-000004b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000004c0: 7069 2f6c 2f70 797a 6f6f 6d29 0a21 5b50  pi/l/pyzoom).![P
-000004d0: 7950 4920 2d20 446f 776e 6c6f 6164 735d  yPI - Downloads]
-000004e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000004f0: 656c 6473 2e69 6f2f 7079 7069 2f64 772f  elds.io/pypi/dw/
-00000500: 7079 7a6f 6f6d 290a 5b21 5b5d 2868 7474  pyzoom).[![](htt
-00000510: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000520: 2e69 6f2f 6261 6467 652f 5375 7070 6f72  .io/badge/Suppor
-00000530: 742d 4275 795f 636f 6666 6565 212d 4f72  t-Buy_coffee!-Or
-00000540: 616e 6765 295d 2868 7474 7073 3a2f 2f77  ange)](https://w
-00000550: 7777 2e62 7579 6d65 6163 6f66 6665 652e  ww.buymeacoffee.
-00000560: 636f 6d2f 6c69 6368 7431 7374 6569 6e29  com/licht1stein)
-00000570: 0a0a 5468 6973 206c 6962 7261 7279 2069  ..This library i
-00000580: 7320 776f 726b 2069 6e20 7072 6f67 7265  s work in progre
-00000590: 7373 2c20 616e 6420 7468 6174 2069 6e63  ss, and that inc
-000005a0: 6c75 6465 7320 646f 6375 6d65 6e74 6174  ludes documentat
-000005b0: 696f 6e2e 204e 6f74 2061 6c6c 206f 6620  ion. Not all of 
-000005c0: 7468 6520 696d 706c 656d 656e 7465 6420  the implemented 
-000005d0: 6d65 7468 6f64 7320 6172 6520 646f 6375  methods are docu
-000005e0: 6d65 6e74 6564 2068 6572 652c 0a73 6f20  mented here,.so 
-000005f0: 706c 6561 7365 2065 7870 6c6f 7265 2074  please explore t
-00000600: 6865 2060 5a6f 6f6d 436c 6965 6e74 6020  he `ZoomClient` 
-00000610: 636c 6173 732e 0a0a 4c69 6e6b 733a 0a2a  class...Links:.*
-00000620: 205b 4170 6920 5265 6665 7265 6e63 655d   [Api Reference]
-00000630: 2868 7474 7073 3a2f 2f6d 6172 6b65 7470  (https://marketp
-00000640: 6c61 6365 2e7a 6f6f 6d2e 7573 2f64 6f63  lace.zoom.us/doc
-00000650: 732f 6170 692d 7265 6665 7265 6e63 6529  s/api-reference)
-00000660: 0a2a 205b 5573 696e 6720 5a6f 6f6d 2041  .* [Using Zoom A
-00000670: 5049 5d28 6874 7470 733a 2f2f 6d61 726b  PI](https://mark
-00000680: 6574 706c 6163 652e 7a6f 6f6d 2e75 732f  etplace.zoom.us/
-00000690: 646f 6373 2f61 7069 2d72 6566 6572 656e  docs/api-referen
-000006a0: 6365 2f75 7369 6e67 2d7a 6f6f 6d2d 6170  ce/using-zoom-ap
-000006b0: 6973 290a 0a23 2320 496e 7374 616c 6c61  is)..## Installa
-000006c0: 7469 6f6e 0a0a 5573 696e 6720 7069 703a  tion..Using pip:
-000006d0: 0a0a 6070 6970 2069 6e73 7461 6c6c 202d  ..`pip install -
-000006e0: 5520 7079 7a6f 6f6d 600a 0a55 7369 6e67  U pyzoom`..Using
-000006f0: 205b 706f 6574 7279 5d28 6874 7470 733a   [poetry](https:
-00000700: 2f2f 6874 7470 733a 2f2f 7079 7468 6f6e  //https://python
-00000710: 2d70 6f65 7472 792e 6f72 672f 293a 0a0a  -poetry.org/):..
-00000720: 6070 6f65 7472 7920 6164 6420 7079 7a6f  `poetry add pyzo
-00000730: 6f6d 600a 0a23 2320 5573 6167 650a 0a23  om`..## Usage..#
-00000740: 2323 2042 6173 6963 2069 6e73 7461 6e74  ## Basic instant
-00000750: 6961 7469 6f6e 3a0a 0a60 6060 7079 7468  iation:..```pyth
-00000760: 6f6e 0a66 726f 6d20 7079 7a6f 6f6d 2069  on.from pyzoom i
-00000770: 6d70 6f72 7420 5a6f 6f6d 436c 6965 6e74  mport ZoomClient
-00000780: 0a0a 636c 6965 6e74 203d 205a 6f6f 6d43  ..client = ZoomC
-00000790: 6c69 656e 7428 2759 4f55 525f 5a4f 4f4d  lient('YOUR_ZOOM
-000007a0: 5f41 5049 5f4b 4559 272c 2027 594f 5552  _API_KEY', 'YOUR
-000007b0: 5f5a 4f4f 4d5f 4150 495f 5345 4352 4554  _ZOOM_API_SECRET
-000007c0: 2729 0a60 6060 0a0a 2323 2320 496e 7374  ').```..### Inst
-000007d0: 616e 7469 6174 696f 6e20 6672 6f6d 2065  antiation from e
-000007e0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000007f0: 626c 6573 0a0a 596f 7520 6361 6e20 616c  bles..You can al
-00000800: 736f 2063 7265 6174 6520 616e 2069 6e73  so create an ins
-00000810: 7461 6e63 6520 6f66 2063 6c69 656e 7420  tance of client 
-00000820: 7768 656e 2073 746f 7269 6e67 2079 6f75  when storing you
-00000830: 7220 6b65 7920 616e 6420 7365 6372 6574  r key and secret
-00000840: 2069 6e20 656e 7669 726f 6e6d 656e 7420   in environment 
-00000850: 7661 7269 6162 6c65 7320 605a 4f4f 4d5f  variables `ZOOM_
-00000860: 4150 495f 4b45 5960 200a 616e 6420 605a  API_KEY` .and `Z
-00000870: 4f4f 4d5f 4150 495f 5345 4352 4554 602e  OOM_API_SECRET`.
-00000880: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00000890: 2070 797a 6f6f 6d20 696d 706f 7274 205a   pyzoom import Z
-000008a0: 6f6f 6d43 6c69 656e 740a 0a63 6c69 656e  oomClient..clien
-000008b0: 7420 3d20 5a6f 6f6d 436c 6965 6e74 2e66  t = ZoomClient.f
-000008c0: 726f 6d5f 656e 7669 726f 6e6d 656e 7428  rom_environment(
-000008d0: 290a 6060 600a 0a0a 2323 2320 4d65 6574  ).```...### Meet
-000008e0: 696e 6773 0a0a 2323 2323 2043 7265 6174  ings..#### Creat
-000008f0: 6520 6d65 6574 696e 6720 616e 6420 6164  e meeting and ad
-00000900: 6420 7265 6769 7374 7261 6e74 0a60 6060  d registrant.```
-00000910: 7079 7468 6f6e 0a66 726f 6d20 7079 7a6f  python.from pyzo
-00000920: 6f6d 2069 6d70 6f72 7420 5a6f 6f6d 436c  om import ZoomCl
-00000930: 6965 6e74 0a66 726f 6d20 6461 7465 7469  ient.from dateti
-00000940: 6d65 2069 6d70 6f72 7420 6461 7465 7469  me import dateti
-00000950: 6d65 2061 7320 6474 0a0a 636c 6965 6e74  me as dt..client
-00000960: 203d 205a 6f6f 6d43 6c69 656e 742e 6672   = ZoomClient.fr
-00000970: 6f6d 5f65 6e76 6972 6f6e 6d65 6e74 2829  om_environment()
-00000980: 0a0a 2320 4372 6561 7469 6e67 2061 206d  ..# Creating a m
-00000990: 6565 7469 6e67 0a6d 6565 7469 6e67 203d  eeting.meeting =
-000009a0: 2063 6c69 656e 742e 6d65 6574 696e 6773   client.meetings
-000009b0: 2e63 7265 6174 655f 6d65 6574 696e 6728  .create_meeting(
-000009c0: 2741 7574 6f20 6372 6561 7465 6420 3127  'Auto created 1'
-000009d0: 2c20 7374 6172 745f 7469 6d65 3d64 742e  , start_time=dt.
-000009e0: 6e6f 7728 292e 6973 6f66 6f72 6d61 7428  now().isoformat(
-000009f0: 292c 2064 7572 6174 696f 6e5f 6d69 6e3d  ), duration_min=
-00000a00: 3630 2c20 7061 7373 776f 7264 3d27 6e6f  60, password='no
-00000a10: 742d 7365 6375 7265 2729 0a0a 0a23 2041  t-secure')...# A
-00000a20: 6464 696e 6720 7265 6769 7374 7261 6e74  dding registrant
-00000a30: 730a 636c 6965 6e74 2e6d 6565 7469 6e67  s.client.meeting
-00000a40: 732e 6164 645f 6d65 6574 696e 675f 7265  s.add_meeting_re
-00000a50: 6769 7374 7261 6e74 286d 6565 7469 6e67  gistrant(meeting
-00000a60: 2e69 642c 2066 6972 7374 5f6e 616d 653d  .id, first_name=
-00000a70: 274a 6f68 6e27 2c20 6c61 7374 5f6e 616d  'John', last_nam
-00000a80: 653d 2744 6f65 272c 2065 6d61 696c 3d27  e='Doe', email='
-00000a90: 6a6f 686e 2e64 6f65 4065 7861 6d70 6c65  john.doe@example
-00000aa0: 2e63 6f6d 2729 0a60 6060 0a59 6f75 2063  .com').```.You c
-00000ab0: 616e 2075 7365 2060 636c 6965 6e74 2e6d  an use `client.m
-00000ac0: 6565 7469 6e67 732e 6164 645f 616e 645f  eetings.add_and_
-00000ad0: 636f 6e66 6972 6d5f 7265 6769 7374 7261  confirm_registra
-00000ae0: 6e74 6020 746f 2061 6c73 6f20 636f 6e66  nt` to also conf
-00000af0: 6972 6d20 6175 746f 2061 6464 6564 0a72  irm auto added.r
-00000b00: 6567 6973 7472 616e 7473 2074 6f20 6120  egistrants to a 
-00000b10: 636c 6f73 6564 206d 6565 7469 6e67 2e0a  closed meeting..
-00000b20: 0a23 2323 2052 6177 2041 5049 206d 6574  .### Raw API met
-00000b30: 686f 6473 0a0a 596f 7520 6361 6e20 616c  hods..You can al
-00000b40: 736f 2075 7365 2074 6865 206c 6962 7261  so use the libra
-00000b50: 7279 2066 6f72 206d 616b 696e 6720 7261  ry for making ra
-00000b60: 7720 7265 7175 6573 7473 2074 6f20 7468  w requests to th
-00000b70: 6520 4150 493a 0a0a 6060 6070 7974 686f  e API:..```pytho
-00000b80: 6e0a 6672 6f6d 2070 797a 6f6f 6d20 696d  n.from pyzoom im
-00000b90: 706f 7274 205a 6f6f 6d43 6c69 656e 740a  port ZoomClient.
-00000ba0: 0a63 6c69 656e 7420 3d20 5a6f 6f6d 436c  .client = ZoomCl
-00000bb0: 6965 6e74 2e66 726f 6d5f 656e 7669 726f  ient.from_enviro
-00000bc0: 6e6d 656e 7428 290a 0a23 2047 6574 2073  nment()..# Get s
-00000bd0: 656c 660a 7265 7370 6f6e 7365 203d 2063  elf.response = c
-00000be0: 6c69 656e 742e 7261 772e 6765 7428 272f  lient.raw.get('/
-00000bf0: 6d65 2729 0a0a 2320 4765 7420 616c 6c20  me')..# Get all 
-00000c00: 7061 6765 7320 6f66 206d 6565 7469 6e67  pages of meeting
-00000c10: 2070 6172 7469 6369 7061 6e74 730a 7265   participants.re
-00000c20: 7375 6c74 5f64 6963 7420 3d20 636c 6965  sult_dict = clie
-00000c30: 6e74 2e72 6177 2e67 6574 5f61 6c6c 5f70  nt.raw.get_all_p
-00000c40: 6167 6573 2827 2f70 6173 745f 6d65 6574  ages('/past_meet
-00000c50: 696e 6773 2f7b 6d65 6574 696e 6755 5549  ings/{meetingUUI
-00000c60: 447d 2f70 6172 7469 6369 7061 6e74 7327  D}/participants'
-00000c70: 290a 6060 600a 0a23 2323 2050 6163 6b61  ).```..### Packa
-00000c80: 6769 6e67 206e 6f74 6963 650a 5468 6973  ging notice.This
-00000c90: 2070 726f 6a65 6374 2075 7365 7320 7468   project uses th
-00000ca0: 6520 6578 6365 6c6c 656e 7420 5b70 6f65  e excellent [poe
-00000cb0: 7472 795d 2868 7474 7073 3a2f 2f70 7974  try](https://pyt
-00000cc0: 686f 6e2d 706f 6574 7279 2e6f 7267 2920  hon-poetry.org) 
-00000cd0: 666f 7220 7061 636b 6167 696e 672e 2050  for packaging. P
-00000ce0: 6c65 6173 6520 7265 6164 2061 626f 7574  lease read about
-00000cf0: 2069 7420 616e 6420 6c65 7427 7320 616c   it and let's al
-00000d00: 6c20 7374 6172 7420 7573 696e 670a 6070  l start using.`p
-00000d10: 7970 726f 6a65 6374 2e74 6f6d 6c60 2066  yproject.toml` f
-00000d20: 696c 6573 2061 7320 6120 7374 616e 6461  iles as a standa
-00000d30: 7264 2e20 5265 6164 206d 6f72 653a 0a0a  rd. Read more:..
-00000d40: 2a20 5b50 4550 2035 3138 202d 2d20 5370  * [PEP 518 -- Sp
-00000d50: 6563 6966 7969 6e67 204d 696e 696d 756d  ecifying Minimum
-00000d60: 2042 7569 6c64 2053 7973 7465 6d20 5265   Build System Re
-00000d70: 7175 6972 656d 656e 7473 2066 6f72 2050  quirements for P
-00000d80: 7974 686f 6e20 5072 6f6a 6563 7473 5d28  ython Projects](
-00000d90: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
-00000da0: 6f6e 2e6f 7267 2f64 6576 2f70 6570 732f  on.org/dev/peps/
-00000db0: 7065 702d 3035 3138 2f29 0a0a 2a20 5b57  pep-0518/)..* [W
-00000dc0: 6861 7420 7468 6520 6865 636b 2069 7320  hat the heck is 
-00000dd0: 7079 7072 6f6a 6563 742e 746f 6d6c 3f5d  pyproject.toml?]
-00000de0: 2868 7474 7073 3a2f 2f73 6e61 726b 792e  (https://snarky.
-00000df0: 6361 2f77 6861 742d 7468 652d 6865 636b  ca/what-the-heck
-00000e00: 2d69 732d 7079 7072 6f6a 6563 742d 746f  -is-pyproject-to
-00000e10: 6d6c 2f29 0a0a 2a20 5b43 6c61 7269 6679  ml/)..* [Clarify
-00000e20: 696e 6720 5045 5020 3531 3820 2861 2e6b  ing PEP 518 (a.k
-00000e30: 2e61 2e20 7079 7072 6f6a 6563 742e 746f  .a. pyproject.to
-00000e40: 6d6c 295d 2868 7474 7073 3a2f 2f73 6e61  ml)](https://sna
-00000e50: 726b 792e 6361 2f63 6c61 7269 6679 696e  rky.ca/clarifyin
-00000e60: 672d 7065 702d 3531 382f 290a 0a0a 2323  g-pep-518/)...##
-00000e70: 2320 5375 7070 6f72 740a 0a3c 6120 6872  # Support..<a hr
-00000e80: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-00000e90: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
-00000ea0: 2f6c 6963 6874 3173 7465 696e 2220 7461  /licht1stein" ta
-00000eb0: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c69  rget="_blank"><i
-00000ec0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000ed0: 6364 6e2e 6275 796d 6561 636f 6666 6565  cdn.buymeacoffee
-00000ee0: 2e63 6f6d 2f62 7574 746f 6e73 2f64 6566  .com/buttons/def
-00000ef0: 6175 6c74 2d6f 7261 6e67 652e 706e 6722  ault-orange.png"
-00000f00: 2061 6c74 3d22 4275 7920 4d65 2041 2043   alt="Buy Me A C
-00000f10: 6f66 6665 6522 2073 7479 6c65 3d22 6865  offee" style="he
-00000f20: 6967 6874 3a20 3330 7078 2021 696d 706f  ight: 30px !impo
-00000f30: 7274 616e 743b 7769 6474 683a 2031 3330  rtant;width: 130
-00000f40: 7078 2021 696d 706f 7274 616e 743b 2220  px !important;" 
-00000f50: 3e3c 2f61 3e0a 0a23 2323 2044 6973 636c  ></a>..### Discl
-00000f60: 6169 6d65 720a 5468 6973 206c 6962 7261  aimer.This libra
-00000f70: 7279 2069 7320 6e6f 7420 7265 6c61 7465  ry is not relate
-00000f80: 6420 746f 205a 6f6f 6d20 5669 6465 6f20  d to Zoom Video 
-00000f90: 436f 6d6d 756e 6963 6174 696f 6e73 2c20  Communications, 
-00000fa0: 496e 632e 2049 7427 7320 616e 206f 7065  Inc. It's an ope
-00000fb0: 6e2d 736f 7572 6365 2070 726f 6a65 6374  n-source project
-00000fc0: 2074 6861 7420 0a61 696d 7320 746f 2073   that .aims to s
-00000fd0: 696d 706c 6966 7920 776f 726b 696e 6720  implify working 
-00000fe0: 7769 7468 2074 6869 7320 7375 6464 656e  with this sudden
-00000ff0: 6c79 2076 6572 7920 706f 7075 6c61 7220  ly very popular 
-00001000: 7365 7276 6963 652e 0a0a                 service...
+000001d0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+000001e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000200: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+00000210: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000230: 7468 6f6e 203a 3a20 332e 3131 0a52 6571  thon :: 3.11.Req
+00000240: 7569 7265 732d 4469 7374 3a20 6174 7472  uires-Dist: attr
+00000250: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
+00000260: 2063 6163 6865 746f 6f6c 7320 283e 3d34   cachetools (>=4
+00000270: 2e31 2c3c 362e 3029 0a52 6571 7569 7265  .1,<6.0).Require
+00000280: 732d 4469 7374 3a20 7079 6461 6e74 6963  s-Dist: pydantic
+00000290: 2028 3e3d 312e 352e 312c 3c32 2e30 2e30   (>=1.5.1,<2.0.0
+000002a0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+000002b0: 2072 6571 7565 7374 7320 283e 3d32 2e32   requests (>=2.2
+000002c0: 332e 302c 3c33 2e30 2e30 290a 5265 7175  3.0,<3.0.0).Requ
+000002d0: 6972 6573 2d44 6973 743a 2073 686f 7274  ires-Dist: short
+000002e0: 7575 6964 2028 3e3d 312e 302e 312c 3c32  uuid (>=1.0.1,<2
+000002f0: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000300: 6973 743a 2074 7970 696e 672d 6578 7465  ist: typing-exte
+00000310: 6e73 696f 6e73 2028 3e3d 332e 372e 342c  nsions (>=3.7.4,
+00000320: 3c35 2e30 2e30 290a 4465 7363 7269 7074  <5.0.0).Descript
+00000330: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000340: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000350: 0a21 5b5a 6f6f 6d20 4c6f 676f 5d28 6874  .![Zoom Logo](ht
+00000360: 7470 733a 2f2f 6432 3463 6777 3375 7662  tps://d24cgw3uvb
+00000370: 3961 3968 2e63 6c6f 7564 6672 6f6e 742e  9a9h.cloudfront.
+00000380: 6e65 742f 7374 6174 6963 2f39 3339 3436  net/static/93946
+00000390: 2f69 6d61 6765 2f6e 6577 2f5a 6f6f 6d4c  /image/new/ZoomL
+000003a0: 6f67 6f2e 706e 6729 0a0a 2a2a 5741 524e  ogo.png)..**WARN
+000003b0: 494e 473a 2056 6572 7369 6f6e 2031 2e30  ING: Version 1.0
+000003c0: 2e30 2069 6e74 726f 6475 6365 7320 6272  .0 introduces br
+000003d0: 6561 6b69 6e67 2063 6861 6e67 652e 2054  eaking change. T
+000003e0: 6865 206c 6962 7261 7279 206e 6f77 206f  he library now o
+000003f0: 6e6c 7920 7375 7070 6f72 7473 204f 4155  nly supports OAU
+00000400: 5448 2074 6f6b 656e 732c 2073 696e 6365  TH tokens, since
+00000410: 205a 6f6f 6d20 6973 2064 6570 7265 6361   Zoom is depreca
+00000420: 7469 6e67 2074 6865 204a 5754 2073 7570  ting the JWT sup
+00000430: 706f 7274 2061 7320 6f66 204a 756e 6520  port as of June 
+00000440: 312c 2032 3032 332a 2a0a 0a41 6c73 6f20  1, 2023**..Also 
+00000450: 7468 6520 7072 6f6a 6563 7420 6e6f 7720  the project now 
+00000460: 7573 6573 205b 6272 6561 6b20 7665 7273  uses [break vers
+00000470: 696f 6e69 6e67 5d28 6874 7470 733a 2f2f  ioning](https://
+00000480: 6769 7468 7562 2e63 6f6d 2f70 7461 6f75  github.com/ptaou
+00000490: 7373 616e 6973 2f65 6e63 6f72 652f 626c  ssanis/encore/bl
+000004a0: 6f62 2f6d 6173 7465 722f 4252 4541 4b2d  ob/master/BREAK-
+000004b0: 5645 5253 494f 4e49 4e47 2e6d 6429 2c20  VERSIONING.md), 
+000004c0: 6d65 616e 696e 6720 7468 6174 2075 7067  meaning that upg
+000004d0: 7261 6469 6e67 2066 726f 6d20 312e 302e  rading from 1.0.
+000004e0: 7820 746f 2031 2e30 2e79 2077 696c 6c20  x to 1.0.y will 
+000004f0: 616c 7761 7973 2062 6520 7361 6665 2c20  always be safe, 
+00000500: 7570 6772 6164 6520 746f 2031 2e78 2e78  upgrade to 1.x.x
+00000510: 206d 6967 6874 2062 7265 616b 2073 6f6d   might break som
+00000520: 6574 6869 6e67 2073 6d61 6c6c 2c20 616e  ething small, an
+00000530: 6420 7570 6772 6164 6520 746f 2032 2e78  d upgrade to 2.x
+00000540: 2e78 2077 696c 6c20 6272 6561 6b20 616c  .x will break al
+00000550: 6d6f 7374 2065 7665 7279 7468 696e 672e  most everything.
+00000560: 2054 6861 7420 7761 7320 6120 7665 7273   That was a vers
+00000570: 696f 6e69 6e67 2073 7065 6320 696e 206f  ioning spec in o
+00000580: 6e65 2073 656e 7465 6e63 652c 2062 7920  ne sentence, by 
+00000590: 7468 6520 7761 792e 0a0a 2320 5079 7468  the way...# Pyth
+000005a0: 6f6e 2077 7261 7070 6572 2066 6f72 205a  on wrapper for Z
+000005b0: 6f6f 6d20 4150 490a 215b 5079 5049 202d  oom API.![PyPI -
+000005c0: 2050 7974 686f 6e20 5665 7273 696f 6e5d   Python Version]
+000005d0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000005e0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000005f0: 6572 7369 6f6e 732f 7079 7a6f 6f6d 290a  ersions/pyzoom).
+00000600: 5b21 5b43 6f64 6520 7374 796c 653a 2062  [![Code style: b
+00000610: 6c61 636b 5d28 6874 7470 733a 2f2f 696d  lack](https://im
+00000620: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000630: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+00000640: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
+00000650: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000660: 622e 636f 6d2f 7073 662f 626c 6163 6b29  b.com/psf/black)
+00000670: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
+00000680: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000690: 2f70 7970 692f 762f 7079 7a6f 6f6d 295d  /pypi/v/pyzoom)]
+000006a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000006b0: 672f 7072 6f6a 6563 742f 7079 7a6f 6f6d  g/project/pyzoom
+000006c0: 2f29 0a21 5b50 7950 4920 2d20 4c69 6365  /).![PyPI - Lice
+000006d0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+000006e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000006f0: 2f6c 2f70 797a 6f6f 6d29 0a21 5b50 7950  /l/pyzoom).![PyP
+00000700: 4920 2d20 446f 776e 6c6f 6164 735d 2868  I - Downloads](h
+00000710: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000720: 6473 2e69 6f2f 7079 7069 2f64 772f 7079  ds.io/pypi/dw/py
+00000730: 7a6f 6f6d 290a 5b21 5b5d 2868 7474 7073  zoom).[![](https
+00000740: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000750: 6f2f 6261 6467 652f 5375 7070 6f72 742d  o/badge/Support-
+00000760: 4275 795f 636f 6666 6565 212d 4f72 616e  Buy_coffee!-Oran
+00000770: 6765 295d 2868 7474 7073 3a2f 2f77 7777  ge)](https://www
+00000780: 2e62 7579 6d65 6163 6f66 6665 652e 636f  .buymeacoffee.co
+00000790: 6d2f 6c69 6368 7431 7374 6569 6e29 0a0a  m/licht1stein)..
+000007a0: 0a2a 2a54 6869 7320 6c69 6272 6172 7920  .**This library 
+000007b0: 7265 7175 6972 6573 2063 6f6e 7472 6962  requires contrib
+000007c0: 7574 6f72 7320 616e 6420 6d61 696e 7461  utors and mainta
+000007d0: 696e 6572 7320 7369 6e63 6520 5079 7468  iners since Pyth
+000007e0: 6f6e 2073 746f 7070 6564 2062 6569 6e67  on stopped being
+000007f0: 206d 7920 7072 696d 6172 7920 6c61 6e67   my primary lang
+00000800: 7561 6765 2061 2063 6f75 706c 6520 6f66  uage a couple of
+00000810: 2079 6561 7273 2061 676f 2e2a 2a0a 4920   years ago.**.I 
+00000820: 646f 2075 7365 2069 7420 696e 2073 6f6d  do use it in som
+00000830: 6520 6f66 206d 7920 6f6c 6465 7220 7072  e of my older pr
+00000840: 6f6a 6563 7473 2c20 736f 2049 2068 6176  ojects, so I hav
+00000850: 6520 746f 2075 7064 6174 6520 6974 2066  e to update it f
+00000860: 726f 6d20 7469 6d65 2074 6f20 7469 6d65  rom time to time
+00000870: 2e0a 0a4c 696e 6b73 3a0a 2a20 5b41 7069  ...Links:.* [Api
+00000880: 2052 6566 6572 656e 6365 5d28 6874 7470   Reference](http
+00000890: 733a 2f2f 6d61 726b 6574 706c 6163 652e  s://marketplace.
+000008a0: 7a6f 6f6d 2e75 732f 646f 6373 2f61 7069  zoom.us/docs/api
+000008b0: 2d72 6566 6572 656e 6365 290a 2a20 5b55  -reference).* [U
+000008c0: 7369 6e67 205a 6f6f 6d20 4150 495d 2868  sing Zoom API](h
+000008d0: 7474 7073 3a2f 2f6d 6172 6b65 7470 6c61  ttps://marketpla
+000008e0: 6365 2e7a 6f6f 6d2e 7573 2f64 6f63 732f  ce.zoom.us/docs/
+000008f0: 6170 692d 7265 6665 7265 6e63 652f 7573  api-reference/us
+00000900: 696e 672d 7a6f 6f6d 2d61 7069 7329 0a0a  ing-zoom-apis)..
+00000910: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+00000920: 0a55 7369 6e67 2070 6970 3a0a 0a60 7069  .Using pip:..`pi
+00000930: 7020 696e 7374 616c 6c20 2d55 2070 797a  p install -U pyz
+00000940: 6f6f 6d60 0a0a 5573 696e 6720 5b70 6f65  oom`..Using [poe
+00000950: 7472 795d 2868 7474 7073 3a2f 2f70 7974  try](https://pyt
+00000960: 686f 6e2d 706f 6574 7279 2e6f 7267 2f29  hon-poetry.org/)
+00000970: 3a0a 0a60 706f 6574 7279 2061 6464 2070  :..`poetry add p
+00000980: 797a 6f6f 6d60 0a0a 2323 2055 7361 6765  yzoom`..## Usage
+00000990: 0a0a 2323 2320 4261 7369 6320 696e 7374  ..### Basic inst
+000009a0: 616e 7469 6174 696f 6e3a 0a0a 6060 6070  antiation:..```p
+000009b0: 7974 686f 6e0a 6672 6f6d 2070 797a 6f6f  ython.from pyzoo
+000009c0: 6d20 696d 706f 7274 205a 6f6f 6d43 6c69  m import ZoomCli
+000009d0: 656e 740a 0a63 6c69 656e 7420 3d20 5a6f  ent..client = Zo
+000009e0: 6f6d 436c 6965 6e74 2827 594f 5552 5f5a  omClient('YOUR_Z
+000009f0: 4f4f 4d5f 4143 4345 5353 5f54 4f4b 454e  OOM_ACCESS_TOKEN
+00000a00: 2729 0a60 6060 0a0a 4f70 7469 6f6e 616c  ').```..Optional
+00000a10: 6c79 2079 6f75 2063 616e 2073 7065 6369  ly you can speci
+00000a20: 6679 2061 2064 6966 6665 7265 6e74 2062  fy a different b
+00000a30: 6173 6520 5552 4c20 6569 7468 6572 2075  ase URL either u
+00000a40: 706f 6e20 696e 7374 616e 7469 6174 696f  pon instantiatio
+00000a50: 6e20 6f72 2061 6e79 2074 696d 6520 6c61  n or any time la
+00000a60: 7465 723a 0a0a 6060 6070 7974 686f 6e0a  ter:..```python.
+00000a70: 636c 6965 6e74 203d 205a 6f6f 6d43 6c69  client = ZoomCli
+00000a80: 656e 7420 2827 594f 555f 5a4f 4f4d 5f41  ent ('YOU_ZOOM_A
+00000a90: 4343 4345 5353 5f54 4f4b 454e 272c 2062  CCCESS_TOKEN', b
+00000aa0: 6173 655f 7572 6c3d 2268 7474 7073 3a2f  ase_url="https:/
+00000ab0: 2f61 7069 2e7a 6f6f 6d67 6f76 2e75 732f  /api.zoomgov.us/
+00000ac0: 7632 2229 0a60 6060 0a0a 2323 2320 496e  v2").```..### In
+00000ad0: 7374 616e 7469 6174 696f 6e20 6672 6f6d  stantiation from
+00000ae0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00000af0: 6961 626c 6573 0a0a 596f 7520 6361 6e20  iables..You can 
+00000b00: 616c 736f 2063 7265 6174 6520 616e 2069  also create an i
+00000b10: 6e73 7461 6e63 6520 6f66 2063 6c69 656e  nstance of clien
+00000b20: 7420 7768 656e 2061 6363 6573 7320 6b65  t when access ke
+00000b30: 7920 696e 2065 6e76 6972 6f6e 6d65 6e74  y in environment
+00000b40: 2076 6172 6961 626c 6573 2060 5a4f 4f4d   variables `ZOOM
+00000b50: 5f41 4343 4553 535f 544f 494b 454e 602e  _ACCESS_TOIKEN`.
+00000b60: 202a 5369 6e63 6520 7468 6520 6163 6365   *Since the acce
+00000b70: 7373 2074 6f6b 656e 2065 7870 6972 6573  ss token expires
+00000b80: 2061 6674 6572 206f 6e65 2068 6f75 722c   after one hour,
+00000b90: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
+00000ba0: 6e6f 7420 6120 676f 6f64 2069 6465 6120  not a good idea 
+00000bb0: 616e 7920 6d6f 7265 2e2a 0a0a 6060 6070  any more.*..```p
+00000bc0: 7974 686f 6e0a 6672 6f6d 2070 797a 6f6f  ython.from pyzoo
+00000bd0: 6d20 696d 706f 7274 205a 6f6f 6d43 6c69  m import ZoomCli
+00000be0: 656e 740a 0a63 6c69 656e 7420 3d20 5a6f  ent..client = Zo
+00000bf0: 6f6d 436c 6965 6e74 2e66 726f 6d5f 656e  omClient.from_en
+00000c00: 7669 726f 6e6d 656e 7428 290a 6060 600a  vironment().```.
+00000c10: 0a0a 2323 2320 4d65 6574 696e 6773 0a0a  ..### Meetings..
+00000c20: 2323 2323 2043 7265 6174 6520 6d65 6574  #### Create meet
+00000c30: 696e 672c 2075 7064 6174 6520 6d65 6574  ing, update meet
+00000c40: 696e 6720 616e 6420 6164 6420 7265 6769  ing and add regi
+00000c50: 7374 7261 6e74 0a60 6060 7079 7468 6f6e  strant.```python
+00000c60: 0a66 726f 6d20 7079 7a6f 6f6d 2069 6d70  .from pyzoom imp
+00000c70: 6f72 7420 5a6f 6f6d 436c 6965 6e74 0a66  ort ZoomClient.f
+00000c80: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
+00000c90: 6f72 7420 6461 7465 7469 6d65 2061 7320  ort datetime as 
+00000ca0: 6474 0a0a 636c 6965 6e74 203d 205a 6f6f  dt..client = Zoo
+00000cb0: 6d43 6c69 656e 742e 6672 6f6d 5f65 6e76  mClient.from_env
+00000cc0: 6972 6f6e 6d65 6e74 2829 0a0a 2320 4372  ironment()..# Cr
+00000cd0: 6561 7469 6e67 2061 206d 6565 7469 6e67  eating a meeting
+00000ce0: 0a6d 6565 7469 6e67 203d 2063 6c69 656e  .meeting = clien
+00000cf0: 742e 6d65 6574 696e 6773 2e63 7265 6174  t.meetings.creat
+00000d00: 655f 6d65 6574 696e 6728 2741 7574 6f20  e_meeting('Auto 
+00000d10: 6372 6561 7465 6420 3127 2c20 7374 6172  created 1', star
+00000d20: 745f 7469 6d65 3d64 742e 6e6f 7728 292e  t_time=dt.now().
+00000d30: 6973 6f66 6f72 6d61 7428 292c 2064 7572  isoformat(), dur
+00000d40: 6174 696f 6e5f 6d69 6e3d 3630 2c20 7061  ation_min=60, pa
+00000d50: 7373 776f 7264 3d27 6e6f 742d 7365 6375  ssword='not-secu
+00000d60: 7265 2729 0a0a 2320 5570 6461 7465 2061  re')..# Update a
+00000d70: 206d 6565 7469 6e67 0a6d 6565 7469 6e67   meeting.meeting
+00000d80: 203d 2063 6c69 656e 742e 6d65 6574 696e   = client.meetin
+00000d90: 6773 2e75 7064 6174 655f 6d65 6574 696e  gs.update_meetin
+00000da0: 6728 2741 7574 6f20 7570 6461 7465 6420  g('Auto updated 
+00000db0: 3127 2c20 6d65 6574 696e 675f 6964 203d  1', meeting_id =
+00000dc0: 206d 6565 7469 6e67 2e69 6420 2c73 7461   meeting.id ,sta
+00000dd0: 7274 5f74 696d 653d 6474 2e6e 6f77 2829  rt_time=dt.now()
+00000de0: 2e69 736f 666f 726d 6174 2829 2c20 6475  .isoformat(), du
+00000df0: 7261 7469 6f6e 5f6d 696e 3d36 302c 7061  ration_min=60,pa
+00000e00: 7373 776f 7264 3d27 6e6f 742d 7365 6375  ssword='not-secu
+00000e10: 7265 2729 0a0a 2320 4164 6469 6e67 2072  re')..# Adding r
+00000e20: 6567 6973 7472 616e 7473 0a63 6c69 656e  egistrants.clien
+00000e30: 742e 6d65 6574 696e 6773 2e61 6464 5f6d  t.meetings.add_m
+00000e40: 6565 7469 6e67 5f72 6567 6973 7472 616e  eeting_registran
+00000e50: 7428 6d65 6574 696e 672e 6964 2c20 6669  t(meeting.id, fi
+00000e60: 7273 745f 6e61 6d65 3d27 4a6f 686e 272c  rst_name='John',
+00000e70: 206c 6173 745f 6e61 6d65 3d27 446f 6527   last_name='Doe'
+00000e80: 2c20 656d 6169 6c3d 276a 6f68 6e2e 646f  , email='john.do
+00000e90: 6540 6578 616d 706c 652e 636f 6d27 290a  e@example.com').
+00000ea0: 6060 600a 596f 7520 6361 6e20 7573 6520  ```.You can use 
+00000eb0: 6063 6c69 656e 742e 6d65 6574 696e 6773  `client.meetings
+00000ec0: 2e61 6464 5f61 6e64 5f63 6f6e 6669 726d  .add_and_confirm
+00000ed0: 5f72 6567 6973 7472 616e 7460 2074 6f20  _registrant` to 
+00000ee0: 616c 736f 2063 6f6e 6669 726d 2061 7574  also confirm aut
+00000ef0: 6f20 6164 6465 640a 7265 6769 7374 7261  o added.registra
+00000f00: 6e74 7320 746f 2061 2063 6c6f 7365 6420  nts to a closed 
+00000f10: 6d65 6574 696e 672e 0a0a 2323 2320 5261  meeting...### Ra
+00000f20: 7720 4150 4920 6d65 7468 6f64 730a 0a59  w API methods..Y
+00000f30: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00000f40: 7468 6520 6c69 6272 6172 7920 666f 7220  the library for 
+00000f50: 6d61 6b69 6e67 2072 6177 2072 6571 7565  making raw reque
+00000f60: 7374 7320 746f 2074 6865 2041 5049 3a0a  sts to the API:.
+00000f70: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00000f80: 7079 7a6f 6f6d 2069 6d70 6f72 7420 5a6f  pyzoom import Zo
+00000f90: 6f6d 436c 6965 6e74 0a0a 636c 6965 6e74  omClient..client
+00000fa0: 203d 205a 6f6f 6d43 6c69 656e 742e 6672   = ZoomClient.fr
+00000fb0: 6f6d 5f65 6e76 6972 6f6e 6d65 6e74 2829  om_environment()
+00000fc0: 0a0a 2320 4765 7420 7365 6c66 0a72 6573  ..# Get self.res
+00000fd0: 706f 6e73 6520 3d20 636c 6965 6e74 2e72  ponse = client.r
+00000fe0: 6177 2e67 6574 2827 2f75 7365 7273 2f6d  aw.get('/users/m
+00000ff0: 6527 290a 0a23 2047 6574 2061 6c6c 2070  e')..# Get all p
+00001000: 6167 6573 206f 6620 6d65 6574 696e 6720  ages of meeting 
+00001010: 7061 7274 6963 6970 616e 7473 0a72 6573  participants.res
+00001020: 756c 745f 6469 6374 203d 2063 6c69 656e  ult_dict = clien
+00001030: 742e 7261 772e 6765 745f 616c 6c5f 7061  t.raw.get_all_pa
+00001040: 6765 7328 272f 7061 7374 5f6d 6565 7469  ges('/past_meeti
+00001050: 6e67 732f 7b6d 6565 7469 6e67 5555 4944  ngs/{meetingUUID
+00001060: 7d2f 7061 7274 6963 6970 616e 7473 2729  }/participants')
+00001070: 0a60 6060 0a0a 2323 2320 5061 636b 6167  .```..### Packag
+00001080: 696e 6720 6e6f 7469 6365 0a54 6869 7320  ing notice.This 
+00001090: 7072 6f6a 6563 7420 7573 6573 2074 6865  project uses the
+000010a0: 2065 7863 656c 6c65 6e74 205b 706f 6574   excellent [poet
+000010b0: 7279 5d28 6874 7470 733a 2f2f 7079 7468  ry](https://pyth
+000010c0: 6f6e 2d70 6f65 7472 792e 6f72 6729 2066  on-poetry.org) f
+000010d0: 6f72 2070 6163 6b61 6769 6e67 2e20 506c  or packaging. Pl
+000010e0: 6561 7365 2072 6561 6420 6162 6f75 7420  ease read about 
+000010f0: 6974 2061 6e64 206c 6574 2773 2061 6c6c  it and let's all
+00001100: 2073 7461 7274 2075 7369 6e67 0a60 7079   start using.`py
+00001110: 7072 6f6a 6563 742e 746f 6d6c 6020 6669  project.toml` fi
+00001120: 6c65 7320 6173 2061 2073 7461 6e64 6172  les as a standar
+00001130: 642e 2052 6561 6420 6d6f 7265 3a0a 0a2a  d. Read more:..*
+00001140: 205b 5045 5020 3531 3820 2d2d 2053 7065   [PEP 518 -- Spe
+00001150: 6369 6679 696e 6720 4d69 6e69 6d75 6d20  cifying Minimum 
+00001160: 4275 696c 6420 5379 7374 656d 2052 6571  Build System Req
+00001170: 7569 7265 6d65 6e74 7320 666f 7220 5079  uirements for Py
+00001180: 7468 6f6e 2050 726f 6a65 6374 735d 2868  thon Projects](h
+00001190: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
+000011a0: 6e2e 6f72 672f 6465 762f 7065 7073 2f70  n.org/dev/peps/p
+000011b0: 6570 2d30 3531 382f 290a 0a2a 205b 5768  ep-0518/)..* [Wh
+000011c0: 6174 2074 6865 2068 6563 6b20 6973 2070  at the heck is p
+000011d0: 7970 726f 6a65 6374 2e74 6f6d 6c3f 5d28  yproject.toml?](
+000011e0: 6874 7470 733a 2f2f 736e 6172 6b79 2e63  https://snarky.c
+000011f0: 612f 7768 6174 2d74 6865 2d68 6563 6b2d  a/what-the-heck-
+00001200: 6973 2d70 7970 726f 6a65 6374 2d74 6f6d  is-pyproject-tom
+00001210: 6c2f 290a 0a2a 205b 436c 6172 6966 7969  l/)..* [Clarifyi
+00001220: 6e67 2050 4550 2035 3138 2028 612e 6b2e  ng PEP 518 (a.k.
+00001230: 612e 2070 7970 726f 6a65 6374 2e74 6f6d  a. pyproject.tom
+00001240: 6c29 5d28 6874 7470 733a 2f2f 736e 6172  l)](https://snar
+00001250: 6b79 2e63 612f 636c 6172 6966 7969 6e67  ky.ca/clarifying
+00001260: 2d70 6570 2d35 3138 2f29 0a0a 0a23 2323  -pep-518/)...###
+00001270: 2053 7570 706f 7274 0a0a 3c61 2068 7265   Support..<a hre
+00001280: 663d 2268 7474 7073 3a2f 2f77 7777 2e62  f="https://www.b
+00001290: 7579 6d65 6163 6f66 6665 652e 636f 6d2f  uymeacoffee.com/
+000012a0: 6c69 6368 7431 7374 6569 6e22 2074 6172  licht1stein" tar
+000012b0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+000012c0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+000012d0: 646e 2e62 7579 6d65 6163 6f66 6665 652e  dn.buymeacoffee.
+000012e0: 636f 6d2f 6275 7474 6f6e 732f 6465 6661  com/buttons/defa
+000012f0: 756c 742d 6f72 616e 6765 2e70 6e67 2220  ult-orange.png" 
+00001300: 616c 743d 2242 7579 204d 6520 4120 436f  alt="Buy Me A Co
+00001310: 6666 6565 2220 7374 796c 653d 2268 6569  ffee" style="hei
+00001320: 6768 743a 2033 3070 7820 2169 6d70 6f72  ght: 30px !impor
+00001330: 7461 6e74 3b77 6964 7468 3a20 3133 3070  tant;width: 130p
+00001340: 7820 2169 6d70 6f72 7461 6e74 3b22 203e  x !important;" >
+00001350: 3c2f 613e 0a0a 2323 2320 4469 7363 6c61  </a>..### Discla
+00001360: 696d 6572 0a54 6869 7320 6c69 6272 6172  imer.This librar
+00001370: 7920 6973 206e 6f74 2072 656c 6174 6564  y is not related
+00001380: 2074 6f20 5a6f 6f6d 2056 6964 656f 2043   to Zoom Video C
+00001390: 6f6d 6d75 6e69 6361 7469 6f6e 732c 2049  ommunications, I
+000013a0: 6e63 2e20 4974 2773 2061 6e20 6f70 656e  nc. It's an open
+000013b0: 2d73 6f75 7263 6520 7072 6f6a 6563 7420  -source project 
+000013c0: 7468 6174 200a 6169 6d73 2074 6f20 7369  that .aims to si
+000013d0: 6d70 6c69 6679 2077 6f72 6b69 6e67 2077  mplify working w
+000013e0: 6974 6820 7468 6973 2073 7564 6465 6e6c  ith this suddenl
+000013f0: 7920 7665 7279 2070 6f70 756c 6172 2073  y very popular s
+00001400: 6572 7669 6365 2e0a 0a                   ervice...
```

