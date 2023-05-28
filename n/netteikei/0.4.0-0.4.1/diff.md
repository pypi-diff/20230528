# Comparing `tmp/netteikei-0.4.0.tar.gz` & `tmp/netteikei-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netteikei-0.4.0.tar", last modified: Sun May 28 06:35:22 2023, max compression
+gzip compressed data, was "netteikei-0.4.1.tar", last modified: Sun May 28 19:03:49 2023, max compression
```

## Comparing `netteikei-0.4.0.tar` & `netteikei-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:22.386169 netteikei-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 06:35:05.000000 netteikei-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 06:35:22.386169 netteikei-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 06:35:05.000000 netteikei-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:22.386169 netteikei-0.4.0/netteikei/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:22.386169 netteikei-0.4.0/netteikei/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/contrib/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/contrib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-28 06:35:05.000000 netteikei-0.4.0/netteikei/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 06:35:22.386169 netteikei-0.4.0/netteikei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 06:35:22.000000 netteikei-0.4.0/netteikei.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 06:35:05.000000 netteikei-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-28 06:35:22.390169 netteikei-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 19:03:33.000000 netteikei-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 19:03:49.687676 netteikei-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 19:03:33.000000 netteikei-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 19:03:33.000000 netteikei-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-28 19:03:49.691676 netteikei-0.4.1/setup.cfg
```

### Comparing `netteikei-0.4.0/LICENSE` & `netteikei-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netteikei-0.4.0/PKG-INFO` & `netteikei-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.4.0
+Version: 0.4.1
 Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

### Comparing `netteikei-0.4.0/netteikei/contrib/download.py` & `netteikei-0.4.1/netteikei/contrib/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import NamedTuple, Self, Unpack
 
 import aiofiles
 from aiohttp import ClientResponse, ClientSession
 import tqdm
 
 from .. import Client, Request
-from ..typedefs import SessionOpts, StrOrURL
+from ..typedefs import SessionKwargs, StrOrURL
 from .utils import isfile, parse_name, parse_length, get_start_byte
 
 
 __all__ = ["download"]
 
 download_dir: ContextVar[Path] = ContextVar("dir")
 
@@ -68,15 +68,15 @@
 
 
 async def download(
     dir: Path,
     /,
     *urls: StrOrURL,
     limit: int = 3,
-    **opts: Unpack[SessionOpts]
+    **kwargs: Unpack[SessionKwargs]
 ) -> None:
     """Asynchronously download files.
 
     Parameters
     ----------
     dir
         Directory where downloads will be stored.
@@ -87,14 +87,14 @@
 
     Raises
     ------
     DownloadAlreadyExists
         Raised when the file has already been downloaded.
     """
     token = download_dir.set(dir)
-    async with ClientSession(**opts) as session:
+    async with ClientSession(**kwargs) as session:
         info = await asyncio.gather(
             *(DownloadInfo.find(session, url) for url in urls)
         )
         client = Client(handlers=(handle_req, handle_res), max_workers=limit)
         await client.run(session, info)
     download_dir.reset(token)
```

### Comparing `netteikei-0.4.0/netteikei/contrib/utils.py` & `netteikei-0.4.1/netteikei/contrib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from collections.abc import Awaitable, Callable
 import functools
 import os
 from pathlib import Path
 from typing import ParamSpec, TypeVar
 
 from aiohttp import ClientResponse
+from aiohttp.typedefs import LooseHeaders
 import pyrfc6266
 
-from ..typedefs import Headers
-
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 
 def wrap(fn: Callable[_P, _R]) -> Callable[_P, Awaitable[_R]]:
     @functools.wraps(fn)
@@ -31,16 +30,16 @@
         return res.url.name
     else:
         if (name := pyrfc6266.parse_filename(s)) is None:
             return default
         return name
 
 
-def parse_length(headers: Headers) -> int | None:
+def parse_length(headers: LooseHeaders) -> int | None:
     if (s := headers.get("Content-Length")) is not None:
         return int(s)
 
 
-async def get_start_byte(headers: Headers, file: Path) -> int:
+async def get_start_byte(headers: LooseHeaders, file: Path) -> int:
     if headers.get("Accept-Ranges") == "bytes" and await isfile(file):
         return await getsize(file)
     return 0
```

### Comparing `netteikei-0.4.0/netteikei/core.py` & `netteikei-0.4.1/netteikei/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         max_workers: int = 5
     ) -> None:
         self._semaphore = asyncio.Semaphore(max_workers)
         self._req_handler, self._res_handler = handlers
     
     async def _request(self, session: ClientSession, obj: T) -> U:
         async with self._semaphore:
-            method, url, opts = await self._req_handler(obj)
-            async with session.request(method, url, **opts) as res:
+            method, url, kwargs = await self._req_handler(obj)
+            async with session.request(method, url, **kwargs) as res:
                 return await self._res_handler(obj, res)
 
     @overload
     async def run(
         self,
         session: ClientSession,
         objs: Iterable[T],
```

### Comparing `netteikei-0.4.0/netteikei.egg-info/PKG-INFO` & `netteikei-0.4.1/netteikei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.4.0
+Version: 0.4.1
 Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

### Comparing `netteikei-0.4.0/setup.cfg` & `netteikei-0.4.1/setup.cfg`

 * *Files identical despite different names*

