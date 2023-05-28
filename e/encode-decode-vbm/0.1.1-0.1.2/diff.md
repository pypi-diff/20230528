# Comparing `tmp/encode_decode_vbm-0.1.1.tar.gz` & `tmp/encode_decode_vbm-0.1.2.tar.gz`

## Comparing `encode_decode_vbm-0.1.1.tar` & `encode_decode_vbm-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/decode.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/encode.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b32.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b64.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/salter.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha256.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha_funcs.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/vigenere.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/LICENSE
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/decode.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/encode.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/b32.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/b64.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/salter.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/sha256.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/sha_funcs.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/vigenere.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/LICENSE
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.2/PKG-INFO
```

### Comparing `encode_decode_vbm-0.1.1/.DS_Store` & `encode_decode_vbm-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/.DS_Store` & `encode_decode_vbm-0.1.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/decode.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/decode.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/encode.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/encode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from .funcs.sha256 import sha256
 from .funcs.b32 import base32e
 from .funcs.b64 import base64e
 from .funcs.vigenere import cypher
 from .funcs.salter import get_salt
 
 
-def encode(mess: str, method: str = "sha", key: str = "crypt", salty: bool = True) -> str:
+def encode(mess: str, method: str = "sha", key: str = "crypt", salty: bool = False) -> str:
     """
     Encodes or hashes a message.
     Takes in the message, the method, key and whether you want the hash or encoding to be salted all as strings.
     Methods available: SHA256 (sha or sha256), BASE32 (b32 or base32), BASE64 (b64 or base64), VIGENERE (vig or vigenere).
     The salty parameter can be anything and it will add salt.
     """
-    if salty == True:
-        salt = get_salt()
-    else:
+    if salty == False:
         salt = ""
+    else:
+        salt = get_salt()
     mess += salt
     if method == "sha" or method == "sha256":
         return f"sha256${salt}${sha256(mess)}"
     elif method == "base32" or method == "b32":
         return f"base32${salt}${base32e(mess)}"
     elif method == "base64" or method == "b64":
         return f"base64${salt}${base64e(mess)}"
```

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b32.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/b32.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/b64.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/b64.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha256.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/sha256.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/sha_funcs.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/sha_funcs.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/src/encode_decode_vbm/funcs/vigenere.py` & `encode_decode_vbm-0.1.2/src/encode_decode_vbm/funcs/vigenere.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/LICENSE` & `encode_decode_vbm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.1/pyproject.toml` & `encode_decode_vbm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "encode_decode_vbm"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Vidak-Becs Mate", email = "matevidakbecs@gmail.com" }]
 description = "encoding and decoding library for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `encode_decode_vbm-0.1.1/PKG-INFO` & `encode_decode_vbm-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode_decode_vbm
-Version: 0.1.1
+Version: 0.1.2
 Summary: encoding and decoding library for python
 Project-URL: Homepage, https://github.com/mate12392/encode_decode_py
 Author-email: Vidak-Becs Mate <matevidakbecs@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

