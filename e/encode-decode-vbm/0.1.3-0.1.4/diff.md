# Comparing `tmp/encode_decode_vbm-0.1.3.tar.gz` & `tmp/encode_decode_vbm-0.1.4.tar.gz`

## Comparing `encode_decode_vbm-0.1.3.tar` & `encode_decode_vbm-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/decode.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/encode.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/b32.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/b64.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/salter.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/sha256.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/sha_funcs.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/vigenere.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/LICENSE
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/decode.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/encode.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/b32.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/b64.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/salter.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/sha256.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/sha_funcs.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/vigenere.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/LICENSE
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 encode_decode_vbm-0.1.4/PKG-INFO
```

### Comparing `encode_decode_vbm-0.1.3/.DS_Store` & `encode_decode_vbm-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/.DS_Store` & `encode_decode_vbm-0.1.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/decode.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/decode.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/encode.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/encode.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from .funcs.vigenere import cypher
 from .funcs.salter import get_salt
 
 
 def encode(mess: str, method: str = "sha", key: str = "crypt", salty: bool = False) -> str:
     """
     Encodes or hashes a message.
-    Takes in the message, the method, key and whether you want the hash or encoding to be salted all as strings.
+    Takes in the message, the method, key and whether you want the hash or encoding to be salted all as strings except for the salt, it has to be True.
     Methods available: SHA256 (sha or sha256), BASE32 (b32 or base32), BASE64 (b64 or base64), VIGENERE (vig or vigenere).
-    The salty parameter can be anything and it will add salt.
     """
     if salty == True:
         salt = get_salt()
     else:
         salt = ""
     mess += salt
     if method == "sha" or method == "sha256":
```

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/b32.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/b32.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/b64.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/b64.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/sha256.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/sha256.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/sha_funcs.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/sha_funcs.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/src/encode_decode_vbm/funcs/vigenere.py` & `encode_decode_vbm-0.1.4/src/encode_decode_vbm/funcs/vigenere.py`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/LICENSE` & `encode_decode_vbm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_decode_vbm-0.1.3/pyproject.toml` & `encode_decode_vbm-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "encode_decode_vbm"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Vidak-Becs Mate", email = "matevidakbecs@gmail.com" }]
 description = "encoding and decoding library for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `encode_decode_vbm-0.1.3/PKG-INFO` & `encode_decode_vbm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode_decode_vbm
-Version: 0.1.3
+Version: 0.1.4
 Summary: encoding and decoding library for python
 Project-URL: Homepage, https://github.com/mate12392/encode_decode_py
 Author-email: Vidak-Becs Mate <matevidakbecs@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

