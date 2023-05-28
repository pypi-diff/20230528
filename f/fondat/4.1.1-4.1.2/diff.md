# Comparing `tmp/fondat-4.1.1.tar.gz` & `tmp/fondat-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.1.tar", max compression
+gzip compressed data, was "fondat-4.1.2.tar", max compression
```

## Comparing `fondat-4.1.1.tar` & `fondat-4.1.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.1/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.1/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.1/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2022-10-04 05:00:48.782297 fondat-4.1.1/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.1/fondat/cache.py
--rw-r--r--   0        0        0    47643 2023-02-01 23:37:21.447708 fondat-4.1.1/fondat/codec.py
--rw-r--r--   0        0        0     5810 2022-05-30 18:20:00.397322 fondat-4.1.1/fondat/context.py
--rw-r--r--   0        0        0    10819 2023-02-01 23:44:51.812872 fondat-4.1.1/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.1/fondat/data.py
--rw-r--r--   0        0        0     2444 2022-09-25 17:46:57.851193 fondat-4.1.1/fondat/error.py
--rw-r--r--   0        0        0     6660 2023-01-03 22:30:55.181857 fondat-4.1.1/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.1/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.1/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.1/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.1/fondat/monitor.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.1/fondat/openapi.py
--rw-r--r--   0        0        0     2592 2022-10-17 23:26:39.100935 fondat-4.1.1/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.1/fondat/patch.py
--rw-r--r--   0        0        0    11500 2023-01-03 22:31:58.798780 fondat-4.1.1/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.1/fondat/security.py
--rw-r--r--   0        0        0    27754 2022-10-26 17:21:16.900572 fondat-4.1.1/fondat/sql.py
--rw-r--r--   0        0        0    10988 2023-02-01 23:37:21.447708 fondat-4.1.1/fondat/sqlite.py
--rw-r--r--   0        0        0     5127 2022-10-18 15:34:06.934521 fondat-4.1.1/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.1/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.1/fondat/types.py
--rw-r--r--   0        0        0    10948 2022-09-30 06:16:57.338274 fondat-4.1.1/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-02-02 00:10:39.137350 fondat-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 fondat-4.1.1/setup.py
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.2/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.2/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.2/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.2/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.2/fondat/cache.py
+-rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.2/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.2/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.2/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.2/fondat/data.py
+-rw-r--r--   0        0        0     2444 2022-09-25 17:46:57.851193 fondat-4.1.2/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.2/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.2/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.2/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.2/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.2/fondat/monitor.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.2/fondat/openapi.py
+-rw-r--r--   0        0        0     2592 2022-10-17 23:26:39.100935 fondat-4.1.2/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.2/fondat/patch.py
+-rw-r--r--   0        0        0    11502 2023-05-27 21:02:45.275230 fondat-4.1.2/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.2/fondat/security.py
+-rw-r--r--   0        0        0    27754 2022-10-26 17:21:16.900572 fondat-4.1.2/fondat/sql.py
+-rw-r--r--   0        0        0    10988 2023-02-01 23:37:21.447708 fondat-4.1.2/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.2/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.2/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.2/fondat/types.py
+-rw-r--r--   0        0        0    10948 2022-09-30 06:16:57.338274 fondat-4.1.2/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-05-27 21:05:30.232080 fondat-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.2/PKG-INFO
```

### Comparing `fondat-4.1.1/LICENSE` & `fondat-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/README.md` & `fondat-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/annotation.py` & `fondat-4.1.2/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/asgi.py` & `fondat-4.1.2/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/cache.py` & `fondat-4.1.2/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/codec.py` & `fondat-4.1.2/fondat/codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,45 +133,44 @@
 
 
 PT = TypeVar("PT")  # Python type hint
 TT = TypeVar("TT")  # target type hint
 
 
 class Codec(Generic[PT, TT]):
-    """
-    Base class for all things encode and decode.
-    """
+    """Base class for all things encode and decode."""
+
+    _cache: Mapping | None = None
 
     def __init__(self, python_type: Any):
         self.python_type = python_type
 
     @staticmethod
     def handles(python_type: Any) -> bool:
         """Return True if the codec handles the specified Python type."""
         raise NotImplementedError
 
     @classmethod
     def get(cls, python_type: Any) -> "Codec[PT, TT]":
         """
         Return a codec that handles the specified Python type.
 
-        If the subclass contains a `_cache` attribute, and does not
-
+        If a subclass defines a `_cache` class attribute with a mapping, this method will use
+        it to cache the return value for future calls.
         """
         if cls is Codec:
             raise NotImplementedError
         with suppress(AttributeError, KeyError):
             return cls._cache[python_type]
         for codec_class in cls.__subclasses__():
             if codec_class.handles(python_type):
                 codec = codec_class(python_type)
                 with suppress(AttributeError):
-                    cache = getattr(codec, "_cache", False)
-                    if isinstance(cache, Mapping):
-                        cache[python_type] = codec
+                    if isinstance(codec._cache, Mapping):
+                        codec._cache[python_type] = codec
                 return codec
         raise TypeError(f"no codec for {python_type}")
 
     def encode(self, value: PT) -> TT:
         """Encode value from F type to T type."""
         raise NotImplementedError
 
@@ -179,15 +178,15 @@
         """Decode value from T type to F type."""
         raise NotImplementedError
 
 
 class StringCodec(Codec[PT, StringType]):
     """Encodes Python types to/from Unicode string representations."""
 
-    _cache = {}
+    _cache = {}  # cache all string codecs
 
     def encode(self, value: PT) -> StringType:
         """Encode value from Python type to string type."""
         raise NotImplementedError
 
     def decode(self, value: StringType) -> PT:
         """Decode value from string type to Python type."""
@@ -197,15 +196,15 @@
 class BinaryCodec(Codec[PT, BinaryType]):
     """Encodes Python types to/from binary representations.
 
     Attribute:
     • content_type: string containing the media type of the binary representation
     """
 
-    _cache = {}
+    _cache = {}  # cache all binary codecs
 
     content_type = APPLICATION_OCTET_STREAM
 
     def encode(self, value: PT) -> BinaryType:
         """Encode value from Python type to binary type."""
         raise NotImplementedError
 
@@ -213,15 +212,15 @@
         """Decode value from binary type to Python type."""
         raise NotImplementedError
 
 
 class JSONCodec(Codec[PT, JSONType]):
     """Encodes Python types to/from the JSON representations."""
 
-    _cache = {}
+    _cache = {}  # cache all JSON codecs
 
     def encode(self, value: PT) -> JSONType:
         """Encode value from Python type to binary type."""
         raise NotImplementedError
 
     def decode(self, value: JSONType) -> PT:
         """Decode value from binary type to Python type."""
```

### Comparing `fondat-4.1.1/fondat/context.py` & `fondat-4.1.2/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/csv.py` & `fondat-4.1.2/fondat/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
 # type aliases
 Row = Iterable[str]
 
 
 def _round(value: Number, precision: int | None) -> str:
     if precision is None:  # floating point
-        value = str(value)
-        if "." in value:
-            value = value.rstrip("0").rstrip(".")
-        return value
+        svalue = str(value)
+        if "." in svalue:
+            svalue = svalue.rstrip("0").rstrip(".")
+        return svalue
     if precision == 0:
         return str(round(value))
     return f"{{:.{precision}f}}".format(value)
 
 
 class CurrencyCodec(Codec[N | NoneType, str]):
     """
@@ -137,16 +137,17 @@
     are encoded in a row. If the columns parameter is omitted, then columns will be all
     TypedDict keys, in the order they are defined in the TypedDict.
 
     The keys mapping specifies the mapping between columns and dictionary keys. If no key
     for a given column is specified, then the column will map the to dictionary key of the
     same name.
 
-    The codecs mapping specifies which codecs are used to encode columns. If no codec for a
-    given column is specified, then the default string codec for its associated type is used.
+    The codecs mapping specifies which codecs are used to encode/decode columns. If no codec
+    for a given column is specified, then the default string codec for its associated type is
+    used.
     """
 
     def __init__(
         self,
         typeddict: Any,
         columns: Iterable[str] | None = None,
         keys: Mapping[str, str] | None = None,
@@ -226,16 +227,16 @@
     in a row. If the columns parameter is omitted, then columns will be all dataclass
     fields, in the order they are defined in the dataclass.
 
     The fields mapping specifies the mapping between column names and dictionary keys. If no
     mapping for a given column is specified, then the column will map to the field name of
     the same name.
 
-    The codecs mapping specifies which codecs are used to encode columns. If no mapping for a
-    given column is provided, then the default codec for its associated field is used.
+    The codecs mapping specifies which codecs are used to encode/decode columns. If no mapping
+    for a given column is provided, then the default codec for its associated field is used.
     """
 
     def __init__(
         self,
         dataclass: Any,
         columns: Iterable[str] = None,
         fields: Mapping[str, str] = None,
```

### Comparing `fondat-4.1.1/fondat/data.py` & `fondat-4.1.2/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/error.py` & `fondat-4.1.2/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/file.py` & `fondat-4.1.2/fondat/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """File I/O module."""
 
 import fondat.error
 import logging
 import mimetypes
 
-from contextlib import suppress
 from fondat.codec import BinaryCodec, DecodeError, StringCodec
 from fondat.http import AsBody
 from fondat.resource import operation, resource
-from fondat.stream import Reader, Stream
+from fondat.stream import IOBaseStream, Reader, Stream
 from pathlib import Path
 from typing import Annotated, BinaryIO, Generic, TypeVar
 from urllib.parse import quote, unquote
 
 
 _logger = logging.getLogger(__name__)
 
@@ -48,34 +47,30 @@
     • content_type: content type of the file, or None if unknown
 
     If content_type is not specified, this class will attempt to guess the content type
     from the filename extension.
     """
 
     def __init__(self, path: Path, content_type: str | None = None):
-        self.file = path.open("rb")
-        self.file.seek(0, 2)
+        file = path.open("rb")
+        file.seek(0, 2)
         if content_type is None:
             content_type = _content_type(path.name)
-        content_length = self.file.tell()
-        self.file.seek(0, 0)
+        content_length = file.tell()
+        file.seek(0, 0)
         super().__init__(content_type, content_length)
+        self.iostream = IOBaseStream(
+            iobase=file, content_type=content_type, content_length=content_length
+        )
 
     async def __anext__(self) -> bytes:
-        if self.file:
-            chunk = self.file.read1(1048576)  # 1 MiB
-            if len(chunk):
-                return chunk
-            await self.close()
-        raise StopAsyncIteration
+        return await anext(self.iostream)
 
     async def close(self) -> None:
-        with suppress(Exception):
-            self.file.close()
-        self.file = None
+        return await self.iostream.close()
 
 
 @resource
 class DirectoryResource(Generic[K, V]):
     """
     Resource that represents files in a directory.
```

### Comparing `fondat-4.1.1/fondat/http.py` & `fondat-4.1.2/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/lazy.py` & `fondat-4.1.2/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/memory.py` & `fondat-4.1.2/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/monitor.py` & `fondat-4.1.2/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/openapi.py` & `fondat-4.1.2/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/pagination.py` & `fondat-4.1.2/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/patch.py` & `fondat-4.1.2/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/resource.py` & `fondat-4.1.2/fondat/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,17 +289,19 @@
     managed through hasattr, getattr, setattr, delattr functions and del statement.
     """
 
 
 def container_resource(resources: Mapping[str, Any], tag: str | None = None):
     """
     Create a resource to contain subordinate resources.
+
     Parameters:
     • resources: mapping of resource names to resource objects
     • tag: tag to group the resource
+
     Suborindates are accessed as attributes by name.
     """
 
     @resource(tag=tag)
     class DeprecatedContainerResource:
         def __getattr__(self, name):
             try:
```

### Comparing `fondat-4.1.1/fondat/security.py` & `fondat-4.1.2/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/sql.py` & `fondat-4.1.2/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/sqlite.py` & `fondat-4.1.2/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/stream.py` & `fondat-4.1.2/fondat/stream.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module for binary content streaming."""
 
 from asyncio import LimitOverrunError
 from collections.abc import AsyncIterator
+from contextlib import suppress
 from fondat.validation import MinLen, MinValue, validate_arguments
+from io import IOBase
 from typing import Annotated
 
 
 class Stream(AsyncIterator[bytes | bytearray]):
     """
     Base class to provide binary content through an asynchronous stream. The stream provides
     binary data through asynchronously iterable chunks of bytes or bytearray.
@@ -70,14 +72,58 @@
         self._content = None
         return result
 
     async def close(self) -> None:
         self._content = None
 
 
+class IOBaseStream(Stream):
+    """
+    Represents an IOBase file-like object as an asynchronous byte stream.
+
+    Parameters:
+    • iobase: the file-like object to stream
+    • content_type: the media type of the stream
+    • content_length: the length of the content, or None if unknown
+    • chunk_size: chunk size to read in each iteration
+    """
+
+    def __init__(
+        self,
+        iobase: IOBase,
+        content_type: str = "application/octet-stream",
+        content_length: int | None = None,
+        chunk_size: int = 1048576,  # 1 MiB
+    ):
+        super().__init__(content_type, content_length)
+        self.iobase = iobase
+        self.chunk_size = chunk_size
+        self._read = getattr(iobase, "read1", "read")
+
+    async def __anext__(self) -> bytes:
+        if not self.iobase:
+            raise StopAsyncIteration
+        try:
+            chunk = self._read(self.chunk_size)
+        except BlockingIOError:  # BufferedIOBase empty response
+            return b""
+        if chunk is None:  # RawIOBase empty
+            return b""
+        if len(chunk) == 0:  # EOF
+            await self.close()
+            raise StopAsyncIteration
+        return chunk
+
+    async def close(self) -> None:
+        if self.iobase:
+            with suppress(Exception):
+                self.iobase.close()
+        self.iobase = None
+
+
 class Reader:
     """
     Buffered stream reader.
 
     If the reader is used as an asynchronous context manager (`async with`), then upon
     exiting the context the stream will be closed.
 
@@ -110,15 +156,15 @@
 
     @validate_arguments
     async def read(self, size: Annotated[int, MinValue(1)] | None = None) -> bytes:
         """
         Read bytes from the stream.
 
         Parameter:
-        • size: number of bytes to read  [to end of stream]
+        • size: number of bytes to read  [read up to end of stream]
 
         This method blocks until all requested bytes are read or the end of the stream is
         encountered.
 
         The end of stream is signified by zero bytes returned.
         """
         while not self._eof and (size is None or len(self._buffer) < size):
```

### Comparing `fondat-4.1.1/fondat/string.py` & `fondat-4.1.2/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/types.py` & `fondat-4.1.2/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/fondat/validation.py` & `fondat-4.1.2/fondat/validation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.1/pyproject.toml` & `fondat-4.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.1"
+version = "4.1.2"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
@@ -23,26 +23,26 @@
 ]
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiosqlite = "^0.18"
+aiosqlite = "^0.19"
 iso8601 = "^1.1"
 multidict = "^6.0"
-wrapt = "^1.14"
+wrapt = "^1.15"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
+black = "^23.3"
 isort = "^5.12"
-pre-commit = "^3.0"
-pytest = "^7.2"
-pytest-asyncio = "^0.20"
-pytest-cov = "^4.0"
+pre-commit = "^3.3"
+pytest = "^7.3"
+pytest-asyncio = "^0.21"
+pytest-cov = "^4.1"
 
 [tool.isort]
 profile = "black"
 lexicographical = true
 lines_after_imports = 2
 lines_between_types = 1
 line_length = 96
```

### Comparing `fondat-4.1.1/PKG-INFO` & `fondat-4.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.1
+Version: 4.1.2
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: aiosqlite (>=0.18,<0.19)
+Requires-Dist: aiosqlite (>=0.19,<0.20)
 Requires-Dist: iso8601 (>=1.1,<2.0)
 Requires-Dist: multidict (>=6.0,<7.0)
-Requires-Dist: wrapt (>=1.14,<2.0)
+Requires-Dist: wrapt (>=1.15,<2.0)
 Project-URL: Documentation, https://github.com/fondat/fondat/tree/main/docs
 Description-Content-Type: text/markdown
 
 # fondat
 
 [![PyPI](https://img.shields.io/pypi/v/fondat)](https://pypi.org/project/fondat/)
 [![Python](https://img.shields.io/pypi/pyversions/fondat)](https://python.org/)
```

