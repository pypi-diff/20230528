# Comparing `tmp/pygmssl-0.0.3.tar.gz` & `tmp/pygmssl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmssl-0.0.3.tar", last modified: Sun May 28 00:26:43 2023, max compression
+gzip compressed data, was "pygmssl-0.0.4.tar", last modified: Sun May 28 05:57:43 2023, max compression
```

## Comparing `pygmssl-0.0.3.tar` & `pygmssl-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/
--rw-r--r--   0 todd      (1000) todd      (1000)     1087 2023-05-26 14:16:26.000000 pygmssl-0.0.3/LICENSE
--rw-r--r--   0 todd      (1000) todd      (1000)     1056 2023-05-28 00:26:43.838622 pygmssl-0.0.3/PKG-INFO
--rw-r--r--   0 todd      (1000) todd      (1000)      497 2023-05-26 14:32:22.000000 pygmssl-0.0.3/README.md
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/pygmssl/
--rw-r--r--   0 todd      (1000) todd      (1000)      228 2023-05-28 00:23:39.000000 pygmssl-0.0.3/pygmssl/__init__.py
--rw-r--r--   0 todd      (1000) todd      (1000)      368 2023-05-27 00:25:43.000000 pygmssl-0.0.3/pygmssl/_gm.py
--rw-r--r--   0 todd      (1000) todd      (1000)     3007 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm2.py
--rw-r--r--   0 todd      (1000) todd      (1000)     2251 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm3.py
--rw-r--r--   0 todd      (1000) todd      (1000)     3060 2023-05-27 13:35:21.000000 pygmssl-0.0.3/pygmssl/sm4.py
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/pygmssl.egg-info/
--rw-r--r--   0 todd      (1000) todd      (1000)     1056 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/PKG-INFO
--rw-r--r--   0 todd      (1000) todd      (1000)      290 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/SOURCES.txt
--rw-r--r--   0 todd      (1000) todd      (1000)        1 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/dependency_links.txt
--rw-r--r--   0 todd      (1000) todd      (1000)        8 2023-05-28 00:26:43.000000 pygmssl-0.0.3/pygmssl.egg-info/top_level.txt
--rw-r--r--   0 todd      (1000) todd      (1000)      710 2023-05-28 00:26:13.000000 pygmssl-0.0.3/pyproject.toml
--rw-r--r--   0 todd      (1000) todd      (1000)       38 2023-05-28 00:26:43.838622 pygmssl-0.0.3/setup.cfg
-drwxr-xr-x   0 todd      (1000) todd      (1000)        0 2023-05-28 00:26:43.838622 pygmssl-0.0.3/tests/
--rw-r--r--   0 todd      (1000) todd      (1000)     1894 2023-05-27 10:56:56.000000 pygmssl-0.0.3/tests/test_sm2.py
--rw-r--r--   0 todd      (1000) todd      (1000)     2268 2023-05-27 02:56:08.000000 pygmssl-0.0.3/tests/test_sm3.py
--rw-r--r--   0 todd      (1000) todd      (1000)     1211 2023-05-27 13:26:10.000000 pygmssl-0.0.3/tests/test_sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.410868 pygmssl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 05:57:32.000000 pygmssl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 05:57:43.410868 pygmssl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-28 05:57:32.000000 pygmssl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/pygmssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/_gm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/pygmssl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 05:57:43.410868 pygmssl-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm4.py
```

### Comparing `pygmssl-0.0.3/LICENSE` & `pygmssl-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Zhang Jie
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Zhang Jie
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pygmssl-0.0.3/PKG-INFO` & `pygmssl-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
 Keywords: 国密,SM2,SM3,SM4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmssl-0.0.3/pygmssl/sm2.py` & `pygmssl-0.0.4/pygmssl/sm3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,80 @@
-from ctypes import *
-
-from ._gm import _gm
-from .sm3 import _SM3CTX
-
-SM2_DEFAULT_ID = b'1234567812345678'
-SM2_MIN_SIGNATURE_SIZE = 8
-SM2_MAX_SIGNATURE_SIZE = 72
-
-
-class _SM2_POINT(Structure):
-    _fields_ = [
-        ('x', c_uint8 * 32),
-        ('y', c_uint8 * 32),
-    ]
-
-
-class _SM2_KEY(Structure):
-    _fields_ = [
-        ('pub', _SM2_POINT),
-        ('pri', c_uint8 * 32),
-    ]
-
-
-class _SM2_SIGN_CTX(Structure):
-    _fields_ = [
-        ('sm3_ctx', _SM3CTX),
-        ('key', _SM2_KEY)
-    ]
-
-
-class SM2:
-    def __init__(self, pub_key: bytes | None = None, pri_key: bytes | None = None):
-        self._sm2_key = _SM2_KEY()
-        if pub_key and len(pub_key) == 65 and pub_key[0] == 4:
-            # if 65 bytes, 0x04 + pub.x + pub.y
-            pub_key = pub_key[1:]
-        if pub_key:
-            if len(pub_key) != 64:
-                raise ValueError('the length of sm2 public key should be 64 bytes')
-            self._sm2_key.pub.x[:32] = pub_key[:32]
-            self._sm2_key.pub.y[:32] = pub_key[32:64]
-        if pri_key:
-            if len(pri_key) != 32:
-                raise ValueError('the length of sm2 private key should be 32 bytes')
-            self._sm2_key.pri[:32] = pri_key
-
-    @classmethod
-    def generate_new_pair(cls) -> 'SM2':
-        obj = cls()
-        _gm.sm2_key_generate(byref(obj._sm2_key))
-        return obj
-
-    @property
-    def pub_key(self) -> bytes:
-        return bytes(self._sm2_key.pub)
-
-    @property
-    def pri_key(self) -> bytes:
-        return bytes(self._sm2_key.pri)
-
-    def compute_z(self, id: bytes = SM2_DEFAULT_ID) -> bytes:
-        z = (c_uint8 * 32)()
-        _gm.sm2_compute_z(byref(z), byref(self._sm2_key.pub), c_char_p(id), len(id))
-        return bytes(z)
-
-    def sign(self, data: bytes, id: bytes = SM2_DEFAULT_ID) -> bytes:
-        _sign_ctx = _SM2_SIGN_CTX()
-        _gm.sm2_sign_init(byref(_sign_ctx), byref(self._sm2_key), c_char_p(id), len(id))
-        buff = (c_uint8 * 4096)()
-        for i in range(0, len(data), 4096):
-            chunk = data[i:i + 4096]
-            buff[:len(chunk)] = chunk
-            _gm.sm2_sign_update(byref(_sign_ctx), byref(buff), len(chunk))
-        sigdst = (c_uint8 * SM2_MAX_SIGNATURE_SIZE)()
-        sigdst_len = c_size_t()
-        _gm.sm2_sign_finish(byref(_sign_ctx), byref(sigdst), byref(sigdst_len))
-        return bytes(sigdst[:sigdst_len.value])
-
-    def verify(self, data: bytes, sig: bytes, id: bytes = SM2_DEFAULT_ID) -> bool:
-        _verify_ctx = _SM2_SIGN_CTX()
-        _gm.sm2_verify_init(byref(_verify_ctx), byref(self._sm2_key), c_char_p(id), len(id))
-        buff = (c_uint8 * 4096)()
-        for i in range(0, len(data), 4096):
-            chunk = data[i:i + 4096]
-            buff[:len(chunk)] = chunk
-            _gm.sm2_verify_update(byref(_verify_ctx), byref(buff), len(chunk))
-        ret = _gm.sm2_verify_finish(byref(_verify_ctx), c_char_p(sig), len(sig))
-        return ret == 1
+from ctypes import byref, c_uint8, c_size_t, c_uint32, c_uint64, Structure, c_char_p
+from typing import Optional
+
+from ._gm import _gm
+
+SM3_DIGEST_SIZE = 32
+SM3_BLOCK_SIZE = 64
+SM3_STATE_WORDS = 8
+SM3_HMAC_SIZE = SM3_DIGEST_SIZE
+
+
+class _SM3CTX(Structure):
+    _fields_ = [
+        ('digest', c_uint32 * SM3_STATE_WORDS),
+        ('nblocks', c_uint64),
+        ('block', c_uint8 * SM3_BLOCK_SIZE),
+        ('num', c_size_t),
+    ]
+
+
+class SM3:
+    def __init__(self, data: Optional[bytes] = None):
+        self._sm3_ctx = _SM3CTX()
+        _gm.sm3_init(byref(self._sm3_ctx))
+        if data is not None:
+            self.update(data)
+
+    def update(self, data: bytes):
+        buff = (c_uint8 * 4096)()
+        for i in range(0, len(data), 4096):
+            chunk = data[i:i + 4096]
+            buff[:len(chunk)] = chunk
+            _gm.sm3_update(byref(self._sm3_ctx), byref(buff), len(chunk))
+
+    def digest(self) -> bytes:
+        dst = (c_uint8 * 32)()
+        _gm.sm3_finish(byref(self._sm3_ctx), byref(dst))
+        return bytes(dst)
+
+    def hexdigest(self) -> str:
+        return self.digest().hex()
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

### Comparing `pygmssl-0.0.3/pygmssl/sm4.py` & `pygmssl-0.0.4/pygmssl/sm4.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from ctypes import *
-
-from ._gm import _gm
-
-SM4_KEY_SIZE = 16
-SM4_BLOCK_SIZE = 16
-SM4_NUM_ROUNDS = 32
-
-
-class _SM4_KEY(Structure):
-    _fields_ = [
-        ('rk', c_uint32 * SM4_NUM_ROUNDS)
-    ]
-
-
-class _SM4_CBC_CTX(Structure):
-    _fields_ = [
-        ('sm4_key', _SM4_KEY),
-        ('iv', c_uint8 * SM4_BLOCK_SIZE),
-        ('block', c_uint8 * SM4_BLOCK_SIZE),
-        ('block_nbytes', c_size_t),
-    ]
-
-    def init(self, key: bytes, iv: bytes, encrypt: bool):
-        assert len(key) == 16
-        assert len(iv) == 16
-        if encrypt:
-            _gm.sm4_cbc_encrypt_init(byref(self), c_char_p(key), c_char_p(iv))
-        else:
-            _gm.sm4_cbc_decrypt_init(byref(self), c_char_p(key), c_char_p(iv))
-        self._result: list[bytes] = []
-
-    def encrypt_update(self, data: bytes):
-        outbuf = (c_uint8 * 4196)()
-        out_length = c_size_t(0)
-        inbuf = (c_uint8 * 4096)()
-        for i in range(0, len(data), 4096):
-            chunk = data[i:i + 4096]
-            inbuf[:len(chunk)] = chunk
-            _gm.sm4_cbc_encrypt_update(byref(self), byref(inbuf), len(chunk), byref(outbuf), byref(out_length))
-            self._result.append(bytes(outbuf[:out_length.value]))
-
-    def decrypt_update(self, encrypted_data: bytes):
-        outbuf = (c_uint8 * 4196)()
-        out_length = c_size_t(0)
-        inbuf = (c_uint8 * 4096)()
-        for i in range(0, len(encrypted_data), 4096):
-            chunk = encrypted_data[i:i + 4096]
-            inbuf[:len(chunk)] = chunk
-            _gm.sm4_cbc_decrypt_update(byref(self), byref(inbuf), len(chunk), byref(outbuf), byref(out_length))
-            self._result.append(bytes(outbuf[:out_length.value]))
-
-    def encrypt_get(self) -> bytes:
-        outbuf = (c_uint8 * 4196)()
-        out_length = c_size_t(0)
-        _gm.sm4_cbc_encrypt_finish(byref(self), byref(outbuf), byref(out_length))
-        self._result.append(bytes(outbuf[:out_length.value]))
-        return b''.join(self._result)
-
-    def decrypt_get(self) -> bytes:
-        outbuf = (c_uint8 * 4196)()
-        out_length = c_size_t(0)
-        _gm.sm4_cbc_decrypt_finish(byref(self), byref(outbuf), byref(out_length))
-        self._result.append(bytes(outbuf[:out_length.value]))
-        return b''.join(self._result)
-
-
-MOD_CTX_DICT = {
-    'CBC': _SM4_CBC_CTX
-}
-
-
-class SM4:
-    def __init__(self, key: bytes, *, mode: str, iv: bytes):
-        if mode.upper() not in MOD_CTX_DICT:
-            raise ValueError(u'Only support sm4 mod: %s' % MOD_CTX_DICT.keys())
-        self._ctx = MOD_CTX_DICT[mode.upper()]()
-        self.key = key
-        self.iv = iv
-
-    def encrypt(self, data: bytes) -> bytes:
-        self._ctx.init(self.key, self.iv, encrypt=True)
-        self._ctx.encrypt_update(data)
-        return self._ctx.encrypt_get()
-
-    def decrypt(self, encrypted_data: bytes) -> bytes:
-        self._ctx.init(self.key, self.iv, encrypt=False)
-        self._ctx.decrypt_update(encrypted_data)
-        return self._ctx.decrypt_get()
+from ctypes import byref, c_uint8, c_size_t, c_uint32, Structure, c_char_p
+
+from ._gm import _gm
+
+SM4_KEY_SIZE = 16
+SM4_BLOCK_SIZE = 16
+SM4_NUM_ROUNDS = 32
+
+
+class _SM4_KEY(Structure):
+    _fields_ = [
+        ('rk', c_uint32 * SM4_NUM_ROUNDS)
+    ]
+
+
+class _SM4_CBC_CTX(Structure):
+    _fields_ = [
+        ('sm4_key', _SM4_KEY),
+        ('iv', c_uint8 * SM4_BLOCK_SIZE),
+        ('block', c_uint8 * SM4_BLOCK_SIZE),
+        ('block_nbytes', c_size_t),
+    ]
+
+    def init(self, key: bytes, iv: bytes, encrypt: bool):
+        assert len(key) == 16
+        assert len(iv) == 16
+        if encrypt:
+            _gm.sm4_cbc_encrypt_init(byref(self), c_char_p(key), c_char_p(iv))
+        else:
+            _gm.sm4_cbc_decrypt_init(byref(self), c_char_p(key), c_char_p(iv))
+        self._result: list[bytes] = []
+
+    def encrypt_update(self, data: bytes):
+        outbuf = (c_uint8 * 4196)()
+        out_length = c_size_t(0)
+        inbuf = (c_uint8 * 4096)()
+        for i in range(0, len(data), 4096):
+            chunk = data[i:i + 4096]
+            inbuf[:len(chunk)] = chunk
+            _gm.sm4_cbc_encrypt_update(byref(self), byref(inbuf), len(chunk), byref(outbuf), byref(out_length))
+            self._result.append(bytes(outbuf[:out_length.value]))
+
+    def decrypt_update(self, encrypted_data: bytes):
+        outbuf = (c_uint8 * 4196)()
+        out_length = c_size_t(0)
+        inbuf = (c_uint8 * 4096)()
+        for i in range(0, len(encrypted_data), 4096):
+            chunk = encrypted_data[i:i + 4096]
+            inbuf[:len(chunk)] = chunk
+            _gm.sm4_cbc_decrypt_update(byref(self), byref(inbuf), len(chunk), byref(outbuf), byref(out_length))
+            self._result.append(bytes(outbuf[:out_length.value]))
+
+    def encrypt_get(self) -> bytes:
+        outbuf = (c_uint8 * 4196)()
+        out_length = c_size_t(0)
+        _gm.sm4_cbc_encrypt_finish(byref(self), byref(outbuf), byref(out_length))
+        self._result.append(bytes(outbuf[:out_length.value]))
+        return b''.join(self._result)
+
+    def decrypt_get(self) -> bytes:
+        outbuf = (c_uint8 * 4196)()
+        out_length = c_size_t(0)
+        _gm.sm4_cbc_decrypt_finish(byref(self), byref(outbuf), byref(out_length))
+        self._result.append(bytes(outbuf[:out_length.value]))
+        return b''.join(self._result)
+
+
+MOD_CTX_DICT = {
+    'CBC': _SM4_CBC_CTX
+}
+
+
+class SM4:
+    def __init__(self, key: bytes, *, mode: str, iv: bytes):
+        if mode.upper() not in MOD_CTX_DICT:
+            raise ValueError(u'Only support sm4 mod: %s' % MOD_CTX_DICT.keys())
+        self._ctx = MOD_CTX_DICT[mode.upper()]()
+        self.key = key
+        self.iv = iv
+
+    def encrypt(self, data: bytes) -> bytes:
+        self._ctx.init(self.key, self.iv, encrypt=True)
+        self._ctx.encrypt_update(data)
+        return self._ctx.encrypt_get()
+
+    def decrypt(self, encrypted_data: bytes) -> bytes:
+        self._ctx.init(self.key, self.iv, encrypt=False)
+        self._ctx.decrypt_update(encrypted_data)
+        return self._ctx.decrypt_get()
```

### Comparing `pygmssl-0.0.3/pygmssl.egg-info/PKG-INFO` & `pygmssl-0.0.4/pygmssl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmssl
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python ctypes GmSSL implementation
 Author-email: Zhang Jie <zhangj_10ujs@foxmail.com>
 Project-URL: Homepage, https://github.com/jz10ujs/pygmssl
 Project-URL: Bug Tracker, https://github.com/jz10ujs/pygmssl/issues
 Keywords: 国密,SM2,SM3,SM4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmssl-0.0.3/pyproject.toml` & `pygmssl-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.3/tests/test_sm2.py` & `pygmssl-0.0.4/tests/test_sm2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from unittest import TestCase
-
-from pygmssl.sm2 import SM2
-
-test_pub_key = b'\xe8G\x0be\xc3P\x12\x10\xa9+\xe6n%\x9dc\xe9\xed\xaeBEf\xab\xd0\x12t\x01RQ\xb8\xceJ\xb0\x9b;\x17\xbb.\xf7i\x00\x18Nq~\xa3\xf4n\xf8\xd7\xdd%m-@\xa3\xc3tv\xe4\xe2\xf7\x81\x83\xe0'
-test_pri_key = b'\x87\x95\x84V\xcej\x8cq\xd1\x10\x94\xa7\xb7\x8d\xc1\x9a\x98\xcf\xe7\x84\x90\x9d\x8d\xd2\xff\xb4\xaeo2\xb8j\x1b'
-
-
-class TestSM2(TestCase):
-    def setUp(self) -> None:
-        self.k = SM2(test_pub_key, test_pri_key)
-
-    def test_001_base(self):
-        k = SM2(test_pub_key, test_pri_key)
-        self.assertEqual(k.pub_key, test_pub_key)
-        self.assertEqual(k.pri_key, test_pri_key)
-
-    def test_002_pub_key(self):
-        k2 = SM2(b'\x04' + test_pub_key, test_pri_key)
-        self.assertEqual(k2.pub_key, test_pub_key)
-        self.assertEqual(k2.pri_key, test_pri_key)
-
-    def test_003_wrong_key(self):
-        with self.assertRaises(ValueError):
-            SM2(test_pub_key + b'\x03')
-
-        with self.assertRaises(ValueError):
-            SM2(pri_key=test_pri_key + b'\x03')
-
-    def test_004_generate_key(self):
-        k = SM2.generate_new_pair()
-        self.assertEqual(len(k.pub_key), 64)
-        self.assertEqual(len(k.pri_key), 32)
-        self.assertNotEqual(k.pub_key, b'\x00'*64)
-        self.assertNotEqual(k.pri_key, b'\x00'*32)
-
-    def test_005_sm2_sign(self):
-        data = b'hello, world'
-        sig = self.k.sign(data)
-        self.assertFalse(self.k.verify(data + b'\x00', sig))
-        self.assertTrue(self.k.verify(data, sig))
-
-    def test_006_sm2_sign_with_id(self):
-        data = b'hello, world'
-        sig = self.k.sign(data, id=b'123')
-        self.assertFalse(self.k.verify(data, sig))
-        self.assertTrue(self.k.verify(data, sig=sig, id=b'123'))
-        self.assertFalse(self.k.verify(b'\x00' + data, sig=sig, id=b'123'))
+from unittest import TestCase
+
+from pygmssl.sm2 import SM2
+
+test_pub_key = b'\xe8G\x0be\xc3P\x12\x10\xa9+\xe6n%\x9dc\xe9\xed\xaeBEf' \
+               b'\xab\xd0\x12t\x01RQ\xb8\xceJ\xb0\x9b;\x17\xbb.\xf7i\x00' \
+               b'\x18Nq~\xa3\xf4n\xf8\xd7\xdd%m-@\xa3\xc3tv\xe4\xe2\xf7\x81\x83\xe0'
+test_pri_key = b'\x87\x95\x84V\xcej\x8cq\xd1\x10\x94\xa7\xb7\x8d\xc1\x9a' \
+               b'\x98\xcf\xe7\x84\x90\x9d\x8d\xd2\xff\xb4\xaeo2\xb8j\x1b'
+
+
+class TestSM2(TestCase):
+    def setUp(self) -> None:
+        self.k = SM2(test_pub_key, test_pri_key)
+
+    def test_001_base(self):
+        k = SM2(test_pub_key, test_pri_key)
+        self.assertEqual(k.pub_key, test_pub_key)
+        self.assertEqual(k.pri_key, test_pri_key)
+
+    def test_002_pub_key(self):
+        k2 = SM2(b'\x04' + test_pub_key, test_pri_key)
+        self.assertEqual(k2.pub_key, test_pub_key)
+        self.assertEqual(k2.pri_key, test_pri_key)
+
+    def test_003_wrong_key(self):
+        with self.assertRaises(ValueError):
+            SM2(test_pub_key + b'\x03')
+
+        with self.assertRaises(ValueError):
+            SM2(pri_key=test_pri_key + b'\x03')
+
+    def test_004_generate_key(self):
+        k = SM2.generate_new_pair()
+        self.assertEqual(len(k.pub_key), 64)
+        self.assertEqual(len(k.pri_key), 32)
+        self.assertNotEqual(k.pub_key, b'\x00' * 64)
+        self.assertNotEqual(k.pri_key, b'\x00' * 32)
+
+    def test_005_sm2_sign(self):
+        data = b'hello, world'
+        sig = self.k.sign(data)
+        self.assertFalse(self.k.verify(data + b'\x00', sig))
+        self.assertTrue(self.k.verify(data, sig))
+
+    def test_006_sm2_sign_with_id(self):
+        data = b'hello, world'
+        sig = self.k.sign(data, id=b'123')
+        self.assertFalse(self.k.verify(data, sig))
+        self.assertTrue(self.k.verify(data, sig=sig, id=b'123'))
+        self.assertFalse(self.k.verify(b'\x00' + data, sig=sig, id=b'123'))
```

### Comparing `pygmssl-0.0.3/tests/test_sm3.py` & `pygmssl-0.0.4/tests/test_sm3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-from unittest import TestCase
-from pygmssl.sm3 import SM3, SM3HMAC
-
-test_pub_key = b'\xe8G\x0be\xc3P\x12\x10\xa9+\xe6n%\x9dc\xe9\xed\xaeBEf\xab\xd0\x12t\x01RQ\xb8\xceJ\xb0\x9b;\x17\xbb.\xf7i\x00\x18Nq~\xa3\xf4n\xf8\xd7\xdd%m-@\xa3\xc3tv\xe4\xe2\xf7\x81\x83\xe0'
-test_pri_key = b'\x87\x95\x84V\xcej\x8cq\xd1\x10\x94\xa7\xb7\x8d\xc1\x9a\x98\xcf\xe7\x84\x90\x9d\x8d\xd2\xff\xb4\xaeo2\xb8j\x1b'
-
-class TestSM3(TestCase):
-    def test_001_sm3_init(self):
-        s = SM3(b'hello, world')
-        self.assertEqual(s.hexdigest(), '02df30dff15f2ccb72bffdcb44e68d4d09974036dc7a6927e556fbef421c7f34')
-
-    def test_002_sm3_update(self):
-        s = SM3()
-        s.update(b'hello,')
-        s.update(b' world')
-        self.assertEqual(s.hexdigest(), '02df30dff15f2ccb72bffdcb44e68d4d09974036dc7a6927e556fbef421c7f34')
-
-    def test_003_sm3_unicode(self):
-        s = SM3(b'hello, ')
-        s.update('中国'.encode('utf-8'))
-        self.assertEqual(s.hexdigest(), '8800ffdad7b39f09312d61877e33e5814f76b5b2a97cba9f2caeb6117296d9d3')
-
-    def test_004_sm3_hash_with_sm2_default_id(self):
-        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key)
-        self.assertEqual(s.hexdigest(), 'ec6781ebf9fc156ac95dbf4df20688f998a121aea34ee71b727fc8b9195d4b42')
-
-    def test_004_sm3_hash_with_sm2_and_id(self):
-        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key, id=b'zhangjie')
-        self.assertEqual(s.hexdigest(), '4c3d2d21c9414db7837c9c495b30415dd39ee8ff127a47a560c8586df40cbdf5')
-
-    def test_004_sm3_hash_update_with_sm2_and_id(self):
-        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key, id=b'zhangjie')
-        s.update('中国'.encode('utf-8'))
-        self.assertEqual(s.hexdigest(), '14e6d70f7b60a849ad9bfea5d0790e2b2c8765e87b2859142f087c67e8bc4e5d')
-
-
-class TestSM3HMAC(TestCase):
-    def test_001_sm3_hmac(self):
-        s = SM3HMAC(key=b'123', data=b'hello, world')
-        self.assertEqual(s.hexdigest(), '4410e0fef1ae0a641c7c4f1a7f6c7cef5b992f80607d5275f669d8942a77cc08')
-
-    def test_002_sm3_hmac_update(self):
-        s = SM3HMAC(b'123')
-        s.update(b'hello,')
-        s.update(b' world')
-        self.assertEqual(s.hexdigest(), '4410e0fef1ae0a641c7c4f1a7f6c7cef5b992f80607d5275f669d8942a77cc08')
+from unittest import TestCase
+
+from pygmssl.sm3 import SM3, SM3HMAC
+
+test_pub_key = b'\xe8G\x0be\xc3P\x12\x10\xa9+\xe6n%\x9dc\xe9\xed\xaeBEf' \
+               b'\xab\xd0\x12t\x01RQ\xb8\xceJ\xb0\x9b;\x17\xbb.\xf7i\x00' \
+               b'\x18Nq~\xa3\xf4n\xf8\xd7\xdd%m-@\xa3\xc3tv\xe4\xe2\xf7\x81\x83\xe0'
+test_pri_key = b'\x87\x95\x84V\xcej\x8cq\xd1\x10\x94\xa7\xb7\x8d\xc1\x9a' \
+               b'\x98\xcf\xe7\x84\x90\x9d\x8d\xd2\xff\xb4\xaeo2\xb8j\x1b'
+
+
+class TestSM3(TestCase):
+    def test_001_sm3_init(self):
+        s = SM3(b'hello, world')
+        self.assertEqual(s.hexdigest(), '02df30dff15f2ccb72bffdcb44e68d4d09974036dc7a6927e556fbef421c7f34')
+
+    def test_002_sm3_update(self):
+        s = SM3()
+        s.update(b'hello,')
+        s.update(b' world')
+        self.assertEqual(s.hexdigest(), '02df30dff15f2ccb72bffdcb44e68d4d09974036dc7a6927e556fbef421c7f34')
+
+    def test_003_sm3_unicode(self):
+        s = SM3(b'hello, ')
+        s.update('中国'.encode('utf-8'))
+        self.assertEqual(s.hexdigest(), '8800ffdad7b39f09312d61877e33e5814f76b5b2a97cba9f2caeb6117296d9d3')
+
+    def test_004_sm3_hash_with_sm2_default_id(self):
+        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key)
+        self.assertEqual(s.hexdigest(), 'ec6781ebf9fc156ac95dbf4df20688f998a121aea34ee71b727fc8b9195d4b42')
+
+    def test_004_sm3_hash_with_sm2_and_id(self):
+        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key, id=b'zhangjie')
+        self.assertEqual(s.hexdigest(), '4c3d2d21c9414db7837c9c495b30415dd39ee8ff127a47a560c8586df40cbdf5')
+
+    def test_004_sm3_hash_update_with_sm2_and_id(self):
+        s = SM3.hash_with_sm2(b'abc', pub_key=test_pub_key, id=b'zhangjie')
+        s.update('中国'.encode('utf-8'))
+        self.assertEqual(s.hexdigest(), '14e6d70f7b60a849ad9bfea5d0790e2b2c8765e87b2859142f087c67e8bc4e5d')
+
+
+class TestSM3HMAC(TestCase):
+    def test_001_sm3_hmac(self):
+        s = SM3HMAC(key=b'123', data=b'hello, world')
+        self.assertEqual(s.hexdigest(), '4410e0fef1ae0a641c7c4f1a7f6c7cef5b992f80607d5275f669d8942a77cc08')
+
+    def test_002_sm3_hmac_update(self):
+        s = SM3HMAC(b'123')
+        s.update(b'hello,')
+        s.update(b' world')
+        self.assertEqual(s.hexdigest(), '4410e0fef1ae0a641c7c4f1a7f6c7cef5b992f80607d5275f669d8942a77cc08')
```

### Comparing `pygmssl-0.0.3/tests/test_sm4.py` & `pygmssl-0.0.4/tests/test_sm4.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from unittest import TestCase
-
-from pygmssl.sm4 import SM4
-import os
-
-class TestSM2(TestCase):
-    def setUp(self) -> None:
-        self._16_key = b"\x97\xfc\xa3\xd7\t;\xf3\xd1'\x9c\x8c\x03\x92\x1c\xf5\xd2"
-        self._16_iv = b'p\xce\xb9\x8d\t$x\x9c\x0f]\xea\x92\xae\xa1\x96\x9d'
-        self._48_key = b'q\xb4j\xdem\x84|J\xf2\x92u\x14\x8f\x95\x85\x1e\x8fT\x01A\x19<\xe1\x82t\xf4\x921\x0b\xbb\x9f\xabY8\xf4\xb2\xf2^\x10|\xbf\xf90\xeb\x19\x12,\xd4'
-
-    def test_000_valid_mod(self):
-        with self.assertRaises(ValueError):
-            SM4(self._16_key, mode='JBC', iv=b'123')
-
-    def test_001_cbc_encrypt(self):
-        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        e_data = k.encrypt(b'hello, world')
-        self.assertEqual(b'W\x855 su+\x95\xd9@\x0fGL\xacKk', e_data)
-        self.assertEqual(b'hello, world', k2.decrypt(e_data))
-
-    def test_002_cbc_bulk_encrypt(self):
-        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        bulk_data = os.urandom(512) * 2099
-        self.assertEqual(bulk_data, k2.decrypt(k.encrypt(bulk_data)))
+import os
+from unittest import TestCase
+
+from pygmssl.sm4 import SM4
+
+
+class TestSM2(TestCase):
+    def setUp(self) -> None:
+        self._16_key = b"\x97\xfc\xa3\xd7\t;\xf3\xd1'\x9c\x8c\x03\x92\x1c\xf5\xd2"
+        self._16_iv = b'p\xce\xb9\x8d\t$x\x9c\x0f]\xea\x92\xae\xa1\x96\x9d'
+        self._48_key = b'q\xb4j\xdem\x84|J\xf2\x92u\x14\x8f\x95\x85\x1e\x8fT\x01A' \
+                       b'\x19<\xe1\x82t\xf4\x921\x0b\xbb\x9f\xabY8\xf4\xb2\xf2^\x10|\xbf\xf90\xeb\x19\x12,\xd4'
+
+    def test_000_valid_mod(self):
+        with self.assertRaises(ValueError):
+            SM4(self._16_key, mode='JBC', iv=b'123')
+
+    def test_001_cbc_encrypt(self):
+        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        e_data = k.encrypt(b'hello, world')
+        self.assertEqual(b'W\x855 su+\x95\xd9@\x0fGL\xacKk', e_data)
+        self.assertEqual(b'hello, world', k2.decrypt(e_data))
+
+    def test_002_cbc_bulk_encrypt(self):
+        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        bulk_data = os.urandom(512) * 2099
+        self.assertEqual(bulk_data, k2.decrypt(k.encrypt(bulk_data)))
```

