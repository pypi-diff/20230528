# Comparing `tmp/pyenphase-0.0.3.tar.gz` & `tmp/pyenphase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.0.3.tar", max compression
+gzip compressed data, was "pyenphase-0.1.0.tar", max compression
```

## Comparing `pyenphase-0.0.3.tar` & `pyenphase-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-05-23 15:34:59.410828 pyenphase-0.0.3/LICENSE
--rw-r--r--   0        0        0     3476 2023-05-23 15:34:59.410828 pyenphase-0.0.3/README.md
--rw-r--r--   0        0        0     2226 2023-05-23 15:35:00.174826 pyenphase-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-23 15:35:00.138826 pyenphase-0.0.3/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/auth.py
--rw-r--r--   0        0        0     2404 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      446 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1321 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-28 00:12:42.225858 pyenphase-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-05-28 00:12:42.225858 pyenphase-0.1.0/README.md
+-rw-r--r--   0        0        0     2226 2023-05-28 00:12:42.989860 pyenphase-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-28 00:12:42.949860 pyenphase-0.1.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     4055 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      612 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0     3000 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0      446 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1618 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.1.0/PKG-INFO
```

### Comparing `pyenphase-0.0.3/LICENSE` & `pyenphase-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.3/README.md` & `pyenphase-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.3/pyproject.toml` & `pyenphase-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.0.3"
+version = "0.1.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.0.3/src/pyenphase/envoy.py` & `pyenphase-0.1.0/src/pyenphase/envoy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import contextlib
+import logging
 import ssl
-from typing import Union
 
 import httpx
 from awesomeversion import AwesomeVersion
 
-from .auth import EnvoyLegacyAuth, EnvoyTokenAuth
+from .auth import EnvoyAuth, EnvoyTokenAuth
 from .firmware import EnvoyFirmware
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
     ssl verify turned off and old SSL versions enabled.
 
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
@@ -30,40 +32,52 @@
 
 _NO_VERIFY_SSL_CONTEXT = create_no_verify_ssl_context()
 
 
 class Envoy:
     """Class for querying and determining the Envoy firmware version."""
 
-    def __init__(self, host: str, auth: Union[EnvoyLegacyAuth, EnvoyTokenAuth]) -> None:
+    def __init__(self, host: str) -> None:
         """Initialize the Envoy class."""
         # We use our own httpx client session so we can disable SSL verification (Envoys use self-signed SSL certs)
         self._client = httpx.AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT)  # nosec
-        self.auth = auth
+        self.auth: EnvoyAuth | None = None
         self._host = host
-        self._firmware = EnvoyFirmware(self._host)
+        self._firmware = EnvoyFirmware(self._client, self._host)
 
-        if AwesomeVersion(self._firmware.firmware_version) < AwesomeVersion("3.9.0"):
+    async def setup(self) -> None:
+        """Obtain the firmware version for later Envoy authentication."""
+        await self._firmware.setup()
+
+    async def authenticate(
+        self, username: str | None = None, password: str | None = None
+    ) -> None:
+        """Authenticate to the Envoy based on firmware version."""
+        if self._firmware.version < AwesomeVersion("3.9.0"):
             # Legacy Envoy firmware
             pass
 
-        if (
-            AwesomeVersion("3.9.0")
-            <= AwesomeVersion(self._firmware.firmware_version)
-            < AwesomeVersion("7.0.0")
-        ):
+        if AwesomeVersion("3.9.0") <= self._firmware.version < AwesomeVersion("7.0.0"):
             # Envoy firmware using old envoy/installer authentication
             pass
 
-        if AwesomeVersion(self._firmware.firmware_version) >= AwesomeVersion("7.0.0"):
+        if self._firmware.version >= AwesomeVersion("7.0.0"):
             # Envoy firmware using new token authentication
-            pass
+            _LOGGER.debug("Authenticating to Envoy using token authentication")
+            if (
+                self.auth is None
+                and username is not None
+                and password is not None
+                and self._firmware.serial is not None
+            ):
+                self.auth = EnvoyTokenAuth(username, password, self._firmware.serial)
+                await self.auth.setup()
 
     @property
     def host(self) -> str:
         """Return the Envoy host."""
         return self._host
 
     @property
     def firmware(self) -> str:
         """Return the Envoy firmware version."""
-        return self._firmware.firmware_version
+        return self._firmware.version
```

### Comparing `pyenphase-0.0.3/src/pyenphase/ssl.py` & `pyenphase-0.1.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.3/PKG-INFO` & `pyenphase-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.0.3
+Version: 0.1.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.0.3 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.1.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

