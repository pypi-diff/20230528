# Comparing `tmp/pygmssl-0.0.2.tar.gz` & `tmp/pygmssl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmssl-0.0.2.tar", last modified: Sat May 27 01:19:16 2023, max compression
+gzip compressed data, was "pygmssl-0.0.3.tar", last modified: Sun May 28 00:26:43 2023, max compression
```

## Comparing `pygmssl-0.0.2.tar` & `pygmssl-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-27 01:19:15.998562 pygmssl-0.0.2/
--rw-r--r--   0 todd      (1000) todd      (1000)     1087 2023-05-26 14:16:26.000000 pygmssl-0.0.2/LICENSE
--rw-r--r--   0 todd      (1000) todd      (1000)      979 2023-05-27 01:19:15.998562 pygmssl-0.0.2/PKG-INFO
--rw-r--r--   0 todd      (1000) todd      (1000)      497 2023-05-26 14:32:22.000000 pygmssl-0.0.2/README.md
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-27 01:19:15.998562 pygmssl-0.0.2/pygmssl/
--rw-r--r--   0 todd      (1000) todd      (1000)      192 2023-05-27 00:25:43.000000 pygmssl-0.0.2/pygmssl/__init__.py
--rw-r--r--   0 todd      (1000) todd      (1000)      368 2023-05-27 00:25:43.000000 pygmssl-0.0.2/pygmssl/_gm.py
--rw-r--r--   0 todd      (1000) todd      (1000)     1084 2023-05-27 00:40:34.000000 pygmssl-0.0.2/pygmssl/sm3.py
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-27 01:19:15.998562 pygmssl-0.0.2/pygmssl.egg-info/
--rw-r--r--   0 todd      (1000) todd      (1000)      979 2023-05-27 01:19:15.000000 pygmssl-0.0.2/pygmssl.egg-info/PKG-INFO
--rw-r--r--   0 todd      (1000) todd      (1000)      224 2023-05-27 01:19:15.000000 pygmssl-0.0.2/pygmssl.egg-info/SOURCES.txt
--rw-r--r--   0 todd      (1000) todd      (1000)        1 2023-05-27 01:19:15.000000 pygmssl-0.0.2/pygmssl.egg-info/dependency_links.txt
--rw-r--r--   0 todd      (1000) todd      (1000)        8 2023-05-27 01:19:15.000000 pygmssl-0.0.2/pygmssl.egg-info/top_level.txt
--rw-r--r--   0 todd      (1000) todd      (1000)      508 2023-05-27 01:19:03.000000 pygmssl-0.0.2/pyproject.toml
--rw-r--r--   0 todd      (1000) todd      (1000)       38 2023-05-27 01:19:15.998562 pygmssl-0.0.2/setup.cfg
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-27 01:19:15.998562 pygmssl-0.0.2/tests/
--rw-r--r--   0 todd      (1000) todd      (1000)      710 2023-05-27 01:11:18.000000 pygmssl-0.0.2/tests/test_sm3.py
+drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/
+-rw-r--r--   0 todd      (1000) todd      (1000)     1087 2023-05-26 14:16:26.000000 pygmssl-0.0.3/LICENSE
+-rw-r--r--   0 todd      (1000) todd      (1000)     1056 2023-05-28 00:26:43.838622 pygmssl-0.0.3/PKG-INFO
+-rw-r--r--   0 todd      (1000) todd      (1000)      497 2023-05-26 14:32:22.000000 pygmssl-0.0.3/README.md
+drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/pygmssl/
+-rw-r--r--   0 todd      (1000) todd      (1000)      228 2023-05-28 00:23:39.000000 pygmssl-0.0.3/pygmssl/__init__.py
+-rw-r--r--   0 todd      (1000) todd      (1000)      368 2023-05-27 00:25:43.000000 pygmssl-0.0.3/pygmssl/_gm.py
+-rw-r--r--   0 todd      (1000) todd      (1000)     3007 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm2.py
+-rw-r--r--   0 todd      (1000) todd      (1000)     2251 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm3.py
+-rw-r--r--   0 todd      (1000) todd      (1000)     3060 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm4.py
+drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/pygmssl.egg-info/
+-rw-r--r--   0 todd      (1000) todd      (1000)     1056 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/PKG-INFO
+-rw-r--r--   0 todd      (1000) todd      (1000)      290 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/SOURCES.txt
+-rw-r--r--   0 todd      (1000) todd      (1000)        1 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/dependency_links.txt
+-rw-r--r--   0 todd      (1000) todd      (1000)        8 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/top_level.txt
+-rw-r--r--   0 todd      (1000) todd      (1000)      710 2023-05-28 00:26:13.000000 pygmssl-0.0.3/pyproject.toml
+-rw-r--r--   0 todd      (1000) todd      (1000)       38 2023-05-28 00:26:43.838622 pygmssl-0.0.3/setup.cfg
+drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/tests/
+-rw-r--r--   0 todd      (1000) todd      (1000)     1894 2023-05-27 10:56:56.000000 pygmssl-0.0.3/tests/test_sm2.py
+-rw-r--r--   0 todd      (1000) todd      (1000)     2268 2023-05-27 02:56:08.000000 pygmssl-0.0.3/tests/test_sm3.py
+-rw-r--r--   0 todd      (1000) todd      (1000)     1211 2023-05-27 13:26:10.000000 pygmssl-0.0.3/tests/test_sm4.py
```

### Comparing `pygmssl-0.0.2/LICENSE` & `pygmssl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.2/PKG-INFO` & `pygmssl-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
+Keywords: 国密,SM2,SM3,SM4
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmssl-0.0.2/pygmssl/sm3.py` & `pygmssl-0.0.3/pygmssl/sm3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from ctypes import *
 from typing import Optional
+
 from ._gm import _gm
 
 SM3_DIGEST_SIZE = 32
 SM3_BLOCK_SIZE = 64
 SM3_STATE_WORDS = 8
 SM3_HMAC_SIZE = SM3_DIGEST_SIZE
 
 
-class SM3CTX(Structure):
+class _SM3CTX(Structure):
     _fields_ = [
         ('digest', c_uint32 * SM3_STATE_WORDS),
         ('nblocks', c_uint64),
         ('block', c_uint8 * SM3_BLOCK_SIZE),
         ('num', c_size_t),
     ]
 
 
 class SM3:
     def __init__(self, data: Optional[bytes] = None):
-        self._sm3_ctx = SM3CTX()
+        self._sm3_ctx = _SM3CTX()
         _gm.sm3_init(byref(self._sm3_ctx))
         if data is not None:
             self.update(data)
 
     def update(self, data: bytes):
         buff = (c_uint8 * 4096)()
         for i in range(0, len(data), 4096):
@@ -34,7 +35,46 @@
     def digest(self) -> bytes:
         dst = (c_uint8 * 32)()
         _gm.sm3_finish(byref(self._sm3_ctx), byref(dst))
         return bytes(dst)
 
     def hexdigest(self) -> str:
         return self.digest().hex()
+
+    @classmethod
+    def hash_with_sm2(cls, data: bytes, pub_key: bytes, id: bytes = None) -> 'SM3':
+        from .sm2 import SM2
+        sm2 = SM2(pub_key=pub_key)
+        z = sm2.compute_z(id=id) if id else sm2.compute_z()
+        s3 = SM3(z)
+        s3.update(data)
+        return s3
+
+
+class _SM3HMACCTX(Structure):
+    _fields_ = [
+        ('sm3ctx', _SM3CTX),
+        ('key', c_uint8 * SM3_BLOCK_SIZE),
+    ]
+
+
+class SM3HMAC:
+    def __init__(self, key: bytes, data: bytes | None = None):
+        self._ctx = _SM3HMACCTX()
+        _gm.sm3_hmac_init(byref(self._ctx), c_char_p(key), len(key))
+        if data:
+            self.update(data)
+
+    def update(self, data: bytes):
+        buff = (c_uint8 * 4096)()
+        for i in range(0, len(data), 4096):
+            chunk = data[i:i + 4096]
+            buff[:len(chunk)] = chunk
+            _gm.sm3_hmac_update(byref(self._ctx), byref(buff), len(chunk))
+
+    def digest(self) -> bytes:
+        dst = (c_uint8 * 32)()
+        _gm.sm3_hmac_finish(byref(self._ctx), byref(dst))
+        return bytes(dst)
+
+    def hexdigest(self) -> str:
+        return self.digest().hex()
```

### Comparing `pygmssl-0.0.2/pygmssl.egg-info/PKG-INFO` & `pygmssl-0.0.3/pygmssl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
+Keywords: 国密,SM2,SM3,SM4
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

