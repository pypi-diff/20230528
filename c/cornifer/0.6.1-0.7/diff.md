# Comparing `tmp/cornifer-0.6.1.tar.gz` & `tmp/cornifer-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornifer-0.6.1.tar", last modified: Wed May 24 19:00:42 2023, max compression
+gzip compressed data, was "cornifer-0.7.tar", last modified: Sun May 28 18:16:47 2023, max compression
```

## Comparing `cornifer-0.6.1.tar` & `cornifer-0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:42.296423 cornifer-0.6.1/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.6.1/LICENSE
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      646 2023-05-24 19:00:42.285469 cornifer-0.6.1/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.6.1/README.md
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:39.173633 cornifer-0.6.1/lib/
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:39.943503 cornifer-0.6.1/lib/Cornifer.egg-info/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      646 2023-05-24 19:00:38.000000 cornifer-0.6.1/lib/Cornifer.egg-info/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-05-24 19:00:39.000000 cornifer-0.6.1/lib/Cornifer.egg-info/SOURCES.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-05-24 19:00:38.000000 cornifer-0.6.1/lib/Cornifer.egg-info/dependency_links.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.6.1/lib/Cornifer.egg-info/not-zip-safe
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-05-24 19:00:38.000000 cornifer-0.6.1/lib/Cornifer.egg-info/requires.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-05-24 19:00:38.000000 cornifer-0.6.1/lib/Cornifer.egg-info/top_level.txt
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:41.125642 cornifer-0.6.1/lib/cornifer/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      897 2022-09-20 19:30:38.000000 cornifer-0.6.1/lib/cornifer/__init__.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:41.740939 cornifer-0.6.1/lib/cornifer/_utilities/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     9959 2023-05-22 16:00:40.000000 cornifer-0.6.1/lib/cornifer/_utilities/__init__.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5805 2023-05-15 19:09:23.000000 cornifer-0.6.1/lib/cornifer/_utilities/lmdb.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8811 2023-05-24 18:08:21.000000 cornifer-0.6.1/lib/cornifer/blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1096 2022-08-25 21:25:33.000000 cornifer-0.6.1/lib/cornifer/errors.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.6.1/lib/cornifer/example.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.6.1/lib/cornifer/filemetadata.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13493 2023-05-19 18:04:55.000000 cornifer-0.6.1/lib/cornifer/info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1987 2023-05-10 16:57:49.000000 cornifer-0.6.1/lib/cornifer/regfilestructure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   127207 2023-05-24 18:09:26.000000 cornifer-0.6.1/lib/cornifer/registers.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.6.1/lib/cornifer/regloader.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      741 2023-05-24 18:54:23.000000 cornifer-0.6.1/lib/cornifer/version.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-05-24 19:00:42.301784 cornifer-0.6.1/setup.cfg
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.6.1/setup.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-24 19:00:42.165784 cornifer-0.6.1/tests/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     9632 2023-05-12 15:41:02.000000 cornifer-0.6.1/tests/test_blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.6.1/tests/test_info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2165 2023-05-10 17:07:48.000000 cornifer-0.6.1/tests/test_register_file_structure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   134643 2023-05-21 16:51:21.000000 cornifer-0.6.1/tests/test_registers.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:47.085758 cornifer-0.7/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.7/LICENSE
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-28 18:16:47.082754 cornifer-0.7/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.7/README.md
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.343713 cornifer-0.7/lib/
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.525860 cornifer-0.7/lib/Cornifer.egg-info/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.7/lib/Cornifer.egg-info/not-zip-safe
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/requires.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-05-28 18:16:46.000000 cornifer-0.7/lib/Cornifer.egg-info/top_level.txt
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.769624 cornifer-0.7/lib/cornifer/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      897 2022-09-20 19:30:38.000000 cornifer-0.7/lib/cornifer/__init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:46.944561 cornifer-0.7/lib/cornifer/_utilities/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10208 2023-05-26 19:18:06.000000 cornifer-0.7/lib/cornifer/_utilities/__init__.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5859 2023-05-25 21:14:31.000000 cornifer-0.7/lib/cornifer/_utilities/lmdb.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8811 2023-05-24 18:08:21.000000 cornifer-0.7/lib/cornifer/blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1096 2022-08-25 21:25:33.000000 cornifer-0.7/lib/cornifer/errors.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.7/lib/cornifer/example.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.7/lib/cornifer/filemetadata.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13578 2023-05-26 14:59:06.000000 cornifer-0.7/lib/cornifer/info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1987 2023-05-10 16:57:49.000000 cornifer-0.7/lib/cornifer/regfilestructure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   128928 2023-05-28 18:02:34.000000 cornifer-0.7/lib/cornifer/registers.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.7/lib/cornifer/regloader.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      730 2023-05-28 18:09:24.000000 cornifer-0.7/lib/cornifer/version.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-05-28 18:16:47.086755 cornifer-0.7/setup.cfg
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.7/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-28 18:16:47.054962 cornifer-0.7/tests/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     9632 2023-05-12 15:41:02.000000 cornifer-0.7/tests/test_blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.7/tests/test_info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2216 2023-05-26 15:26:43.000000 cornifer-0.7/tests/test_register_file_structure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   134663 2023-05-28 15:19:05.000000 cornifer-0.7/tests/test_registers.py
```

### Comparing `cornifer-0.6.1/LICENSE` & `cornifer-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/PKG-INFO` & `cornifer-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.6.1
+Version: 0.7
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.6.1/README.md` & `cornifer-0.7/README.md`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/Cornifer.egg-info/PKG-INFO` & `cornifer-0.7/lib/Cornifer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.6.1
+Version: 0.7
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.6.1/lib/Cornifer.egg-info/SOURCES.txt` & `cornifer-0.7/lib/Cornifer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/__init__.py` & `cornifer-0.7/lib/cornifer/__init__.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/_utilities/__init__.py` & `cornifer-0.7/lib/cornifer/_utilities/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,25 @@
 
 def is_signed_int(num):
     return isinstance(num, (int, np.int8, np.int16, np.int32, np.int64))
 
 def is_int(num):
     return isinstance(num, (int, np.int8, np.int16, np.int32, np.int64, np.uint8, np.uint16, np.uint32, np.uint64))
 
+def bytify_num(num, num_zeros = None):
+
+    if num_zeros is None:
+        return str(num).encode("ASCII")
+
+    else:
+        return f"{num:0{num_zeros}d}".encode("ASCII")
+
+def intify_bytes(bytes_):
+    return int(bytes_.decode("ASCII"))
+
 def check_type(obj, name, expected_type):
 
     if not isinstance(obj, expected_type):
         raise TypeError(f"`{name}` must be of type `{expected_type.__name__}`, not `{type(obj).__name__}`.")
 
 def check_type_None_default(obj, name, expected_type, default):
```

### Comparing `cornifer-0.6.1/lib/cornifer/_utilities/lmdb.py` & `cornifer-0.7/lib/cornifer/_utilities/lmdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,30 +81,32 @@
     def delete(self, key):
 
         if key not in self.undo.keys():
             self.undo[key] = self.txn.get(key, default = None)
 
         self.txn.delete(key)
 
-def lmdb_is_closed(db):
-
-    try:
-        with db.begin() as _:
-            pass
-
-    except BaseException as e:
-
-        if isinstance(e, lmdb.Error) and "Attempt to operate on closed/deleted/dropped object." in str(e):
-            return True
-
-        else:
-            raise e
-
-    else:
-        return False
+# def lmdb_is_closed(db):
+#
+#     try:
+#         print("lmdb_is_closed before", db.info()['num_readers'])
+#         with db.begin() as _:
+#             pass
+#         print("lmdb_is_closed after", db.info()['num_readers'])
+#
+#     except BaseException as e:
+#
+#         if isinstance(e, lmdb.Error) and "Attempt to operate on closed/deleted/dropped object." in str(e):
+#             return True
+#
+#         else:
+#             raise e
+#
+#     else:
+#         return False
 
 def open_lmdb(filepath, mapSize, readonly):
 
     if not isinstance(filepath, Path):
         raise TypeError("`filepath` must be of type `pathlib.Path`.")
 
     if not is_int(mapSize):
@@ -180,17 +182,14 @@
     return isinstance(txn, (lmdb.Transaction, ReversibleTransaction))
 
 @contextmanager
 def _resolve_db_or_txn(db_or_txn):
 
     if isinstance(db_or_txn, lmdb.Environment):
 
-        if lmdb_is_closed(db_or_txn):
-            raise lmdb.Error("Environment should not be closed.")
-
         txn = db_or_txn.begin()
         abort = True
 
     elif is_transaction(db_or_txn):
 
         txn = db_or_txn
         abort = False
```

### Comparing `cornifer-0.6.1/lib/cornifer/blocks.py` & `cornifer-0.7/lib/cornifer/blocks.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/errors.py` & `cornifer-0.7/lib/cornifer/errors.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/example.py` & `cornifer-0.7/lib/cornifer/example.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/filemetadata.py` & `cornifer-0.7/lib/cornifer/filemetadata.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/info.py` & `cornifer-0.7/lib/cornifer/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,17 @@
     def set_encoder(self, encoder):
 
         if not isinstance(encoder, json.JSONEncoder):
             raise TypeError("`encoder` must be of type `json.JSONEncoder`.")
 
         self._encoder = encoder
 
+    def clean_encoder(self):
+        self._encoder = type(self)._default_encoder
+
     def __iter__(self):
 
         for key, val in self.__dict__.items():
 
             if key not in type(self)._reserved_kws:
                 yield key, val
```

### Comparing `cornifer-0.6.1/lib/cornifer/regfilestructure.py` & `cornifer-0.7/lib/cornifer/regfilestructure.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/registers.py` & `cornifer-0.7/lib/cornifer/registers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 from .errors import DataNotFoundError, RegisterAlreadyOpenError, RegisterError, CompressionError, \
     DecompressionError, NOT_ABSOLUTE_ERROR_MESSAGE, RegisterRecoveryError
 from .info import ApriInfo, AposInfo, _InfoJsonEncoder, _InfoJsonDecoder, _Info
 from .blocks import Block, MemmapBlock, ReleaseBlock
 from .filemetadata import FileMetadata
 from ._utilities import random_unique_filename, is_int, resolve_path, BYTES_PER_MB, is_deletable, check_type, \
-    check_return_int_None_default, check_Path, check_return_int
-from ._utilities.lmdb import lmdb_has_key, lmdb_prefix_iter, open_lmdb, lmdb_is_closed, lmdb_count_keys, \
+    check_return_int_None_default, check_Path, check_return_int, bytify_num, intify_bytes
+from ._utilities.lmdb import lmdb_has_key, lmdb_prefix_iter, open_lmdb, lmdb_count_keys, \
     ReversibleTransaction, is_transaction, lmdb_prefix_list
 from .regfilestructure import VERSION_FILEPATH, LOCAL_DIR_CHARS, \
     COMPRESSED_FILE_SUFFIX, MSG_FILEPATH, CLS_FILEPATH, check_reg_structure, DATABASE_FILEPATH, \
     REG_FILENAME, MAP_SIZE_FILEPATH
 from .version import CURRENT_VERSION, COMPATIBLE_VERSIONS
 
 _NO_DEBUG = 0
@@ -50,15 +50,15 @@
 _KEY_SEP                   = b"\x00\x00"
 _START_N_HEAD_KEY          = b"head"
 _START_N_TAIL_LENGTH_KEY   = b"tail_length"
 _CLS_KEY                   = b"cls"
 _MSG_KEY                   = b"msg"
 _SUB_KEY_PREFIX            = b"sub"
 _BLK_KEY_PREFIX            = b"blk"
-_APRI_ID_KEY_PREFIX        = b"info"
+_APRI_ID_KEY_PREFIX        = b"apri"
 _ID_APRI_KEY_PREFIX        = b"id"
 _CURR_ID_KEY               = b"curr_id"
 _APOS_KEY_PREFIX           = b"apos"
 _COMPRESSED_KEY_PREFIX     = b"compr"
 _LENGTH_LENGTH_KEY         = b"lenlen"
 
 _KEY_SEP_LEN               = len(_KEY_SEP)
@@ -120,14 +120,16 @@
 #           CONSTANTS           #
 
 _START_N_TAIL_LENGTH_DEFAULT   = 12
 _LENGTH_LENGTH_DEFAULT         = 7
 _MAX_LENGTH_DEFAULT            = 10 ** _LENGTH_LENGTH_DEFAULT - 1
 _START_N_HEAD_DEFAULT          = 0
 _INITIAL_REGISTER_SIZE_DEFAULT = 5 * BYTES_PER_MB
+_MAX_NUM_APRI_LENGTH           = 6
+_MAX_NUM_APRI                  = 10**_MAX_NUM_APRI_LENGTH
 
 class Register(ABC):
 
     #################################
     #     PUBLIC INITIALIZATION     #
 
     def __init__(self, saves_dir, msg, initial_reg_size = None):
@@ -144,15 +146,15 @@
         check_Path(saves_dir, "saves_dir")
         check_type(msg, "msg", str)
         initial_reg_size = check_return_int_None_default(
             initial_reg_size, "initial_reg_size", _INITIAL_REGISTER_SIZE_DEFAULT
         )
 
         if initial_reg_size <= 0:
-            raise ValueError("`initialRegSize` must be positive.")
+            raise ValueError("`initial_reg_size` must be positive.")
 
         self.saves_dir = resolve_path(Path(saves_dir))
 
         if not self.saves_dir.is_dir():
             raise FileNotFoundError(
                 f"You must create the file `{str(self.saves_dir)}` before calling " +
                 f"`{self.__class__.__name__}(\"{str(self.saves_dir)}\", \"{msg}\")`."
@@ -166,14 +168,15 @@
         self._subreg_bytes = None
 
         self._db = None
         self._db_filepath = None
         self._db_map_size = initial_reg_size
         self._db_map_size_filepath = None
         self._readonly = None
+        self._opened = False
 
         self._version = CURRENT_VERSION
         self._version_filepath = None
 
         self._cls_filepath = None
 
         self._startn_head = _START_N_HEAD_DEFAULT
@@ -231,25 +234,25 @@
                     "only its concrete subclasses."
                 )
 
             con = Register._constructors.get(cls_name, None)
 
             if con is None:
                 raise TypeError(
-                    f"`Register` is not aware of a subclass called `{cls_name}`. Please be sure that `{cls_name}` properly "
-                    f"subclasses `Register` and that `{cls_name}` is in the namespace by importing it."
+                    f"`Register` is not aware of a subclass called `{cls_name}`. Please be sure that `{cls_name}` "
+                    f"properly subclasses `Register` and that `{cls_name}` is in the namespace by importing it."
                 )
 
             with (local_dir / MSG_FILEPATH).open("r") as fh:
                 msg = fh.read()
 
             with (local_dir / MAP_SIZE_FILEPATH).open("r") as fh:
-                mapSize = int(fh.readline().strip())
+                map_size = int(fh.readline().strip())
 
-            reg = con(local_dir.parent, msg, mapSize)
+            reg = con(local_dir.parent, msg, map_size)
             reg._set_local_dir(local_dir)
 
             with (local_dir / VERSION_FILEPATH).open("r") as fh:
                 reg._version = fh.readline().strip()
 
             return reg
 
@@ -412,14 +415,15 @@
             raise ValueError("`tail_len` must be positive.")
 
         if head == self._startn_head and tail_len == self._startn_tail_length:
             return
 
         new_mod = 10 ** tail_len
 
+        # check that every block startn has the correct head (don't change anything yet)
         with lmdb_prefix_iter(self._db, _BLK_KEY_PREFIX) as it:
 
             for key, _ in it:
 
                 apri, startn, length = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
 
                 if startn // new_mod != head:
@@ -439,26 +443,24 @@
 
             with self._db.begin(write = True) as rw_txn:
 
                 with self._db.begin() as ro_txn:
 
                     with lmdb_prefix_iter(ro_txn, _BLK_KEY_PREFIX) as it:
 
-                        rw_txn.put(_START_N_HEAD_KEY, str(head).encode("ASCII"))
-                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, str(tail_len).encode("ASCII"))
+                        rw_txn.put(_START_N_HEAD_KEY, bytify_num(head))
+                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, bytify_num(tail_len))
 
                         for key, val in it:
 
                             _, startn, _ = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
-                            apri_json, _, length_bytes = Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
-
-                            new_startn_bytes = str(startn % new_mod).encode("ASCII")
-
+                            apri_id, _, length_bytes = self._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
+                            new_startn_bytes = bytify_num(startn % new_mod, tail_len)
                             new_key = Register._join_disk_block_data(
-                                _BLK_KEY_PREFIX, apri_json, new_startn_bytes, length_bytes
+                                _BLK_KEY_PREFIX, apri_id, new_startn_bytes, length_bytes
                             )
 
                             if key != new_key:
 
                                 rw_txn.put(new_key, val)
                                 rw_txn.delete(key)
 
@@ -511,14 +513,15 @@
                         txn.put(_CURR_ID_KEY, b"0")
 
                 except lmdb.MapFullError as e:
                     raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                 Register._add_instance(local_dir, self)
                 yiel = self
+                yiel._opened = True
 
             except BaseException as e:
 
                 if local_dir.is_dir():
                     shutil.rmtree(local_dir)
 
                 raise e
@@ -628,29 +631,31 @@
 
         else:
             ret = self
 
         if not ret._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_open_created"))
 
-        if ret._db is not None and not ret._db_is_closed():
+        if ret._db is not None and ret._opened:
             raise RegisterAlreadyOpenError()
 
         ret._readonly = readonly
 
         ret._db = open_lmdb(ret._db_filepath, ret._db_map_size, readonly)
 
         with ret._db.begin() as txn:
             ret._length_length = int(txn.get(_LENGTH_LENGTH_KEY))
 
         ret._max_length = 10 ** ret._length_length - 1
-
+        ret._opened = True
         return ret
 
     def _close_created(self):
+
+        self._opened = False
         self._db.close()
 
     @contextmanager
     def _recursive_open(self, readonly):
 
         if not self._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_recursive_open"))
@@ -670,20 +675,23 @@
                     "Attempted to open a `Register` in read-write mode that is already open in read-only mode."
                 )
 
             try:
                 yield yiel
 
             finally:
+                
                 if need_close:
+                    
                     yiel._close_created()
+                    yiel._opened = False
 
     def _check_open_raise(self, method_name):
 
-        if self._db is None or self._db_is_closed():
+        if not self._opened:
             raise RegisterError(
                 f"This `Register` database has not been opened. You must open this register via `with reg.open() as " +
                 f"reg:` before calling the method `{method_name}`."
             )
 
     def _check_readwrite_raise(self, method_name):
         """Call `self._check_open_raise` before this method."""
@@ -741,52 +749,33 @@
         self._version_filepath = local_dir / VERSION_FILEPATH
         self._msg_filepath = local_dir / MSG_FILEPATH
         self._cls_filepath = local_dir / CLS_FILEPATH
         self._db_map_size_filepath = local_dir / MAP_SIZE_FILEPATH
 
     def _has_compatible_version(self):
         return self._version in COMPATIBLE_VERSIONS
-
-    def _db_is_closed(self):
-
-        if not self._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_db_is_closed"))
-
-        else:
-            return lmdb_is_closed(self._db)
+    #
+    # def _db_is_closed(self):
+    #
+    #     if not self._created:
+    #         raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_db_is_closed"))
+    #
+    #     else:
+    #         return lmdb_is_closed(self._db)
 
     #################################
     #      PUBLIC APRI METHODS      #
 
     def apris(self, diskonly = False, recursively = False):
 
         self._check_open_raise("apris")
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
-        ret = []
-
-        if not diskonly:
-            ret.extend(self._ram_blks.keys())
-
-        with self._db.begin() as txn:
-
-            with lmdb_prefix_iter(txn, _ID_APRI_KEY_PREFIX) as it:
-
-                for _, val in it:
-                    ret.append(relational_decode_info(self, ApriInfo, val, txn))
-
-        if recursively:
-
-            for subreg in self._iter_subregs():
-
-                with subreg._recursive_open(True) as subreg:
-                    ret.append(subreg.apris())
-
-        return sorted(list(set(ret)))
+        return list(self._apris_helper(diskonly, recursively, True))
 
     def change_apri(self, old_apri, new_apri, diskonly = False, recursively = False):
         """Replace an old `ApriInfo`, and all references to it, with a new `ApriInfo`.
 
         If ANY `Block`, `ApriInfo`, or `AposInfo` references `old_apri`, its entries in this `Register` will be
         updated to reflect the replacement of `old_apri` with `new_apri`. (See example below.) After the replacement
         `old_apri` -> `new_apri` is made, the set of `ApriInfo` that changed under that replacement must be disjoint
@@ -941,14 +930,41 @@
 
             else:
                 raise e
 
     #################################
     #      PROTEC APRI METHODS      #
 
+    def _apris_helper(self, diskonly, recursively, root_call):
+
+        ret = []
+
+        if not diskonly:
+            ret.extend(self._ram_blks.keys())
+
+        with self._db.begin() as txn:
+
+            with lmdb_prefix_iter(txn, _ID_APRI_KEY_PREFIX) as it:
+
+                for _, val in it:
+                    ret.append(relational_decode_info(self, ApriInfo, val, txn))
+
+        if recursively:
+
+            for subreg in self._iter_subregs():
+
+                with subreg._recursive_open(True) as subreg:
+                    ret.extend(subreg._apris_helper(diskonly, recursively, False))
+
+        if root_call:
+            yield from sorted(set(ret))
+
+        else:
+            yield from ret
+
     def _check_known_apri(self, apri, txn = None):
 
         commit = txn is None
 
         if commit:
             txn = self._db.begin()
 
@@ -1067,22 +1083,25 @@
 
         if 8 + 6 + len(apri_id_key) > 4096:
             warnings.warn(f"Long `ApriInfo` result in disk memory inefficiency. Long `ApriInfo`: {str(apri)}.")
 
     @staticmethod
     def _get_new_apri_id(txn, reserved):
 
-        for next_id_num in count(int(txn.get(_CURR_ID_KEY))):
+        for next_id_num in range(int(txn.get(_CURR_ID_KEY)), _MAX_NUM_APRI):
 
-            next_id = str(next_id_num).encode("ASCII")
+            next_id = bytify_num(next_id_num, _MAX_NUM_APRI_LENGTH)
 
             if next_id not in reserved:
                 break
 
-        txn.put(_CURR_ID_KEY, str(next_id_num + 1).encode("ASCII"))
+        else:
+            raise RegisterError(f"Too many apris added to this `Register`, the limit is {_MAX_NUM_APRI}.")
+
+        txn.put(_CURR_ID_KEY, bytify_num(next_id_num + 1, _MAX_NUM_APRI_LENGTH))
         return next_id
 
     def _rmv_apri_txn(self, apri, force, txn):
 
         apris = []
         aposs = []
         blk_datas = []
@@ -2129,24 +2148,24 @@
             return FileMetadata.from_path(blk_filename)
 
         else:
             return None
 
     def is_compressed(self, apri, startn = None, length = None):
 
-        self._check_open_raise("is_compressed")
-        check_type(apri, "apri", ApriInfo)
-        startn = check_return_int_None_default(startn, "startn", None)
-        length = check_return_int_None_default(length, "length", None)
-
-        if startn is not None and startn < 0:
-            raise ValueError("`startn` must be non-negative.")
-
-        if length is not None and length < 0:
-            raise ValueError("`length` must be non-negative.")
+        # self._check_open_raise("is_compressed")
+        # check_type(apri, "apri", ApriInfo)
+        # startn = check_return_int_None_default(startn, "startn", None)
+        # length = check_return_int_None_default(length, "length", None)
+        # 
+        # if startn is not None and startn < 0:
+        #     raise ValueError("`startn` must be non-negative.")
+        # 
+        # if length is not None and length < 0:
+        #     raise ValueError("`length` must be non-negative.")
 
         startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
         with self._db.begin() as txn:
             return txn.get(
                 self._get_disk_blk_key(_COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False, txn)
             ) != _IS_NOT_COMPRESSED_VAL
@@ -2286,18 +2305,16 @@
         :return: (type `bytes`)
         """
 
         if apri is None and apri_json is None:
             raise ValueError
 
         id_ = self._get_id_by_apri(apri, apri_json, missing_ok, txn, None)
-        tail = startn % self._startn_tail_mod
-        tail = f"{tail:0{self._startn_tail_length}d}".encode("ASCII")
-        op_length = self._max_length - length
-        op_length = f"{op_length:0{self._length_length}d}".encode("ASCII")
+        tail = bytify_num(startn % self._startn_tail_mod, self._startn_tail_length)
+        op_length = bytify_num(self._max_length - length, self._length_length)
 
         return (
                 prefix   +
                 id_      + _KEY_SEP +
                 tail     + _KEY_SEP +
                 op_length
         )
@@ -2318,41 +2335,40 @@
         """Iterate over key-value pairs for block entries.
 
         :param prefix: (type `bytes`)
         :param apri: (type `ApriInfo`)
         :param apri_json: (type `bytes`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
-        :raise DataNotFoundError: If `info` is not a disk `ApriInfo`.
+        :raise DataNotFoundError: If `apri` is not a disk `ApriInfo`.
         :return: (type `bytes`) key
         :return: (type `bytes`) value
         """
 
-        try:
-            prefix += self._get_id_by_apri(apri, apri_json, False, txn, None)
+        prefix += self._get_id_by_apri(apri, apri_json, False, txn, None) + _KEY_SEP
 
-        except DataNotFoundError:
-            pass
+        with lmdb_prefix_iter(txn if txn is not None else self._db, prefix) as it:
+            yield from it
 
-        else:
+    def _split_disk_block_key(self, prefix_len, key):
 
-            prefix += _KEY_SEP
+        stop1 = prefix_len + _MAX_NUM_APRI_LENGTH
+        stop2 = stop1 + _KEY_SEP_LEN + self._startn_tail_length
 
-            with lmdb_prefix_iter(txn if txn is not None else self._db, prefix) as it:
-                yield from it
-
-    @staticmethod
-    def _split_disk_block_key(prefix_len, key):
-        return tuple(key[prefix_len:].split(_KEY_SEP))
+        return (
+            key[prefix_len           : stop1], # apri id
+            key[stop1 + _KEY_SEP_LEN : stop2], # startn
+            key[stop2 + _KEY_SEP_LEN : ] # op_length
+        )
 
     @staticmethod
-    def _join_disk_block_data(prefix, apri_json, startn_bytes, len_bytes):
+    def _join_disk_block_data(prefix, apri_id, startn_bytes, len_bytes):
         return (
                 prefix +
-                apri_json + _KEY_SEP +
+                apri_id + _KEY_SEP +
                 startn_bytes + _KEY_SEP +
                 len_bytes
         )
 
     def _convert_disk_block_key(self, prefix_len, key, apri = None, txn = None):
         """
         :param prefix_len: (type `int`) Positive.
@@ -2362,15 +2378,15 @@
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
         :return: (type `ApriInfo`)
         :return (type `int`) startn
         :return (type `int`) length, non-negative
         """
 
-        apri_id, startn_bytes, op_length_bytes = Register._split_disk_block_key(prefix_len, key)
+        apri_id, startn_bytes, op_length_bytes = self._split_disk_block_key(prefix_len, key)
 
         commit = apri is None and txn is None
 
         if commit:
             txn = self._db.begin()
 
         try:
@@ -2381,19 +2397,22 @@
                 apri = relational_decode_info(self, ApriInfo, apri_json, txn)
 
         finally:
 
             if commit:
                 txn.commit()
 
-        return (
-            apri,
-            int(startn_bytes.decode("ASCII")) + self._startn_head * self._startn_tail_mod,
-            self._max_length - int(op_length_bytes.decode("ASCII"))
-        )
+        try:
+            return (
+                apri,
+                intify_bytes(startn_bytes) + self._startn_head * self._startn_tail_mod,
+                self._max_length - intify_bytes(op_length_bytes)
+            )
+        except ValueError:
+            raise
 
     def _check_blk_compressed_keys_raise(self, blk_key, compressed_key, apri, apri_json, startn, length, txn = None):
 
         if compressed_key is None and blk_key is None:
             compressed_key = self._get_disk_blk_key(_COMPRESSED_KEY_PREFIX, apri, apri_json, startn, length, False, txn)
 
         if blk_key is not None and compressed_key is None:
@@ -2844,55 +2863,15 @@
     def intervals(self, apri, combine = False, diskonly = False, recursively = False):
 
         self._check_open_raise("intervals")
         check_type(apri, "apri", ApriInfo)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
-        if not combine:
-
-            try:
-                self._check_known_apri(apri)
-
-            except DataNotFoundError:
-
-                if not recursively:
-                    raise
-
-            else:
-
-                if not diskonly and apri in self._ram_blks.keys():
-
-                    for blk in self._ram_blks[apri]:
-                        yield blk.startn(), len(blk)
-
-                for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None):
-                    yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri)[1:]
-
-            if recursively:
-
-                for subreg in self._iter_subregs():
-
-                    with subreg._recursive_open(True) as subreg:
-                        yield from subreg.intervals(apri, combine = False, diskonly = diskonly, recursively = True)
-
-        else:
-
-            ret = []
-            intervals_sorted = self.intervals(apri, combine = False, diskonly = diskonly, recursively = recursively)
-
-            for startn, length in intervals_sorted:
-
-                if len(ret) == 0:
-                    ret.append((startn, length))
-
-                elif startn <= ret[-1][0] + ret[-1][1]:
-                    ret[-1] = (ret[-1][0], max(startn + length - ret[-1][0], ret[-1][1]))
-
-            yield from ret
+        yield from self._intervals_helper(apri, combine, diskonly, recursively, True)
 
     def total_len(self, apri, diskonly = False, recursively = False):
 
         self._check_open_raise("total_len")
         check_type(apri, "apri", ApriInfo)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
@@ -3059,14 +3038,74 @@
 
                 for key, _ in it:
                     return self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
 
                 else:
                     raise DataNotFoundError(_blk_not_found_err_msg(True, apri))
 
+    def _intervals_helper(self, apri, combine, diskonly, recursively, root_call):
+
+        if not combine:
+
+            with self._db.begin() as txn:
+
+                try:
+                    self._check_known_apri(apri, txn)
+
+                except DataNotFoundError:
+
+                    if not recursively:
+                        raise
+
+                else:
+
+                    if not diskonly and apri in self._ram_blks.keys():
+
+                        for blk in self._ram_blks[apri]:
+                            yield blk.startn(), len(blk)
+
+                    try:
+
+                        for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None, txn):
+                            yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, txn)[1:]
+
+                    except DataNotFoundError:
+                        pass
+
+            if recursively:
+
+                for subreg in self._iter_subregs():
+
+                    with subreg._recursive_open(True) as subreg:
+                        yield from subreg._intervals_helper(apri, combine, diskonly, recursively, False)
+
+        if combine and root_call:
+
+            if (diskonly or len(self._ram_blks) == 0) and not recursively:
+                intervals_sorted = list(self._intervals_helper(apri, False, diskonly, recursively, False))
+
+            else:
+                intervals_sorted = sorted(
+                    self._intervals_helper(apri, False, diskonly, recursively, False),
+                    key = lambda t: (t[0], -t[1])
+                )
+
+            ret = []
+
+            for startn, length in intervals_sorted:
+
+                if len(ret) == 0:
+                    ret.append((startn, length))
+
+                elif startn <= ret[-1][0] + ret[-1][1]:
+                    ret[-1] = (ret[-1][0], max(startn + length - ret[-1][0], ret[-1][1]))
+
+            yield from ret
+
+
 class PickleRegister(Register):
 
     @classmethod
     def with_suffix(cls, filename):
         return filename.with_suffix(".pkl")
 
     @classmethod
@@ -3698,14 +3737,16 @@
             separators = (',', ':')
         )
         info.set_encoder(encoder)
         return info.to_json().encode("ASCII")
 
     finally:
 
+        info.clean_encoder() # necessary so that the garbage collector cleans Transactions properly
+
         if commit:
             txn.commit()
 
 def relational_decode_info(reg, cls, json, txn = None):
 
     check_type(reg, "reg", Register)
     check_type(json, "json", bytes)
```

### Comparing `cornifer-0.6.1/lib/cornifer/regloader.py` & `cornifer-0.7/lib/cornifer/regloader.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/lib/cornifer/version.py` & `cornifer-0.7/lib/cornifer/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
-CURRENT_VERSION          = "0.6.1"
-COMPATIBLE_VERSIONS      = ["0.6", "0.6.1"]
+CURRENT_VERSION          = "0.7"
+COMPATIBLE_VERSIONS      = ["0.7"]
```

### Comparing `cornifer-0.6.1/setup.py` & `cornifer-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/tests/test_blocks.py` & `cornifer-0.7/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/tests/test_info.py` & `cornifer-0.7/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.6.1/tests/test_register_file_structure.py` & `cornifer-0.7/tests/test_register_file_structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import shutil
 from pathlib import Path
 from unittest import TestCase
 
+from cornifer._utilities import random_unique_filename
 from cornifer.regfilestructure import check_reg_structure, REG_FILENAME, VERSION_FILEPATH, \
     MSG_FILEPATH, CLS_FILEPATH, DATABASE_FILEPATH, MAP_SIZE_FILEPATH
 
-SAVES_DIR = Path(__file__).parent.resolve() / "temp"
+SAVES_DIR = random_unique_filename(Path.home())
 
 class Test_Register_File_Structure(TestCase):
 
     def setUp(self):
         if SAVES_DIR.is_dir():
             shutil.rmtree(SAVES_DIR)
         SAVES_DIR.mkdir(exist_ok=False)
```

### Comparing `cornifer-0.6.1/tests/test_registers.py` & `cornifer-0.7/tests/test_registers.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,38 +206,38 @@
     #     )
     #
     #     self.assertEqual(
     #         Register._constructors["Testy_Register2"],
     #         Testy_Register2
     #     )
 
-    def test__split_disk_block_key(self):
-
-        keys = [
-            _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP + b"00000" + _KEY_SEP + b"10",
-            _BLK_KEY_PREFIX +                            _KEY_SEP + b"00000" + _KEY_SEP + b"10",
-            _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP +            _KEY_SEP + b"10",
-            _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP + b"00000" + _KEY_SEP        ,
-        ]
-        splits = [
-            (b"{\"hello\" = \"hey\"}", b"00000", b"10"),
-            (b"",                      b"00000", b"10"),
-            (b"{\"hello\" = \"hey\"}", b"",      b"10"),
-            (b"{\"hello\" = \"hey\"}", b"00000", b""  ),
-        ]
-        for key, split in zip(keys, splits):
-            self.assertEqual(
-                split,
-                Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
-            )
-        for key in keys:
-            self.assertEqual(
-                key,
-                Register._join_disk_block_data(*((_BLK_KEY_PREFIX,) + Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)))
-            )
+    # def test__split_disk_block_key(self):
+    #
+    #     keys = [
+    #         _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP + b"00000" + _KEY_SEP + b"10",
+    #         _BLK_KEY_PREFIX +                            _KEY_SEP + b"00000" + _KEY_SEP + b"10",
+    #         _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP +            _KEY_SEP + b"10",
+    #         _BLK_KEY_PREFIX + b"{\"hello\" = \"hey\"}" + _KEY_SEP + b"00000" + _KEY_SEP        ,
+    #     ]
+    #     splits = [
+    #         (b"{\"hello\" = \"hey\"}", b"00000", b"10"),
+    #         (b"",                      b"00000", b"10"),
+    #         (b"{\"hello\" = \"hey\"}", b"",      b"10"),
+    #         (b"{\"hello\" = \"hey\"}", b"00000", b""  ),
+    #     ]
+    #     for key, split in zip(keys, splits):
+    #         self.assertEqual(
+    #             split,
+    #             Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
+    #         )
+    #     for key in keys:
+    #         self.assertEqual(
+    #             key,
+    #             Register._join_disk_block_data(*((_BLK_KEY_PREFIX,) + Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)))
+    #         )
 
     def test__join_disk_block_data(self):
 
         splits = [
             (_BLK_KEY_PREFIX, b"hello", b"there", b"friend"),
             (_BLK_KEY_PREFIX, b"",      b"there", b"friend"),
             (_BLK_KEY_PREFIX, b"hello", b"",      b"friend"),
@@ -250,19 +250,19 @@
             _BLK_KEY_PREFIX + b"hello" + _KEY_SEP + b"there" + _KEY_SEP
         ]
         for split,key in zip(splits, keys):
             self.assertEqual(
                key,
                Register._join_disk_block_data(*split)
             )
-        for split in splits:
-            self.assertEqual(
-                split[1:],
-                Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, Register._join_disk_block_data(*split))
-            )
+        # for split in splits:
+        #     self.assertEqual(
+        #         split[1:],
+        #         Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, Register._join_disk_block_data(*split))
+        #     )
 
     def test___str__(self):
 
         self.assertEqual(
             str(Testy_Register(SAVES_DIR, "hello")),
             "hello"
         )
@@ -427,26 +427,26 @@
         )
 
     def test_open_uncreated(self):
 
         reg = Testy_Register(SAVES_DIR, "hey")
 
         with reg.open() as reg:
-            self.assertFalse(reg._db_is_closed())
+            self.assertTrue(reg._opened)
 
         self.assertTrue(reg._created)
 
         keyvals = {
             _START_N_HEAD_KEY : b"0",
             _START_N_TAIL_LENGTH_KEY : str(_START_N_TAIL_LENGTH_DEFAULT).encode("ASCII"),
             _LENGTH_LENGTH_KEY : str(_LENGTH_LENGTH_DEFAULT).encode("ASCII"),
             _CURR_ID_KEY : b"0",
         }
 
-        self.assertTrue(reg._db_is_closed())
+        self.assertFalse(reg._opened)
 
         db = None
 
         try:
 
             db = open_lmdb(reg._db_filepath, 1, False)
 
@@ -946,15 +946,15 @@
             )
 
     def test__open_created(self):
 
         reg = Testy_Register(SAVES_DIR, "testy")
         with reg.open() as reg: pass
         with reg.open() as reg:
-            self.assertFalse(reg._db_is_closed())
+            self.assertTrue(reg._opened)
             with self.assertRaises(RegisterAlreadyOpenError):
                 with reg.open() as reg: pass
 
         reg1 = Testy_Register(SAVES_DIR, "testy")
         with reg1.open() as reg1: pass
 
         reg2 = Testy_Register(SAVES_DIR, "testy")
@@ -1386,20 +1386,20 @@
             try:
                 with reg5._recursive_open(False):pass
 
             except RegisterError:
                 self.fail()
 
             else:
-                self.assertFalse(
-                    reg5._db_is_closed()
+                self.assertTrue(
+                    reg5._opened
                 )
 
-        self.assertTrue(
-            reg5._db_is_closed()
+        self.assertFalse(
+            reg5._opened
         )
 
         reg6 = Testy_Register(SAVES_DIR, "supp")
 
         with reg6.open() as reg6: pass
 
         with reg6.open(readonly= True) as reg6:
```

