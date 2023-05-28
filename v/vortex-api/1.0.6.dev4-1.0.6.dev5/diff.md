# Comparing `tmp/vortex_api-1.0.6.dev4.tar.gz` & `tmp/vortex_api-1.0.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-1nme3hvo/vortex_api-1.0.6.dev4.tar", last modified: Fri May 26 09:54:38 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-8665d3oj/vortex_api-1.0.6.dev5.tar", last modified: Fri May 26 12:36:35 2023, max compression
```

## Comparing `vortex_api-1.0.6.dev4.tar` & `vortex_api-1.0.6.dev5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.574833 vortex_api-1.0.6.dev4/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev4/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 09:54:38.574921 vortex_api-1.0.6.dev4/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2345 2023-05-26 09:51:08.000000 vortex_api-1.0.6.dev4/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 09:54:38.575193 vortex_api-1.0.6.dev4/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1569 2023-05-26 09:54:09.000000 vortex_api-1.0.6.dev4/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.573412 vortex_api-1.0.6.dev4/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev4/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 09:54:17.000000 vortex_api-1.0.6.dev4/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev4/vortex_api/api.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    22011 2023-05-26 09:41:32.000000 vortex_api-1.0.6.dev4/vortex_api/vortex_feed.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.574696 vortex_api-1.0.6.dev4/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      136 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 12:36:35.918047 vortex_api-1.0.6.dev5/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev5/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 12:36:35.918147 vortex_api-1.0.6.dev5/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2345 2023-05-26 09:51:08.000000 vortex_api-1.0.6.dev5/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 12:36:35.918471 vortex_api-1.0.6.dev5/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1569 2023-05-26 09:54:09.000000 vortex_api-1.0.6.dev5/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 12:36:35.916783 vortex_api-1.0.6.dev5/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev5/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 12:36:17.000000 vortex_api-1.0.6.dev5/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev5/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22135 2023-05-26 12:36:10.000000 vortex_api-1.0.6.dev5/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 12:36:35.917900 vortex_api-1.0.6.dev5/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 12:36:35.000000 vortex_api-1.0.6.dev5/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 12:36:35.000000 vortex_api-1.0.6.dev5/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 12:36:35.000000 vortex_api-1.0.6.dev5/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      136 2023-05-26 12:36:35.000000 vortex_api-1.0.6.dev5/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 12:36:35.000000 vortex_api-1.0.6.dev5/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.6.dev4/LICENSE` & `vortex_api-1.0.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev4/PKG-INFO` & `vortex_api-1.0.6.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.6.dev4
+Version: 1.0.6.dev5
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `vortex_api-1.0.6.dev4/README.md` & `vortex_api-1.0.6.dev5/README.md`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev4/setup.py` & `vortex_api-1.0.6.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev4/vortex_api/__init__.py` & `vortex_api-1.0.6.dev5/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev4/vortex_api/api.py` & `vortex_api-1.0.6.dev5/vortex_api/api.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev4/vortex_api/vortex_feed.py` & `vortex_api-1.0.6.dev5/vortex_api/vortex_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,33 +497,34 @@
                     "open_price": open_price,
                     "high_price": high_price,
                     "low_price": low_price,
                     "close_price": close_price,
                     "volume": volume
                 })
             elif len(packet) == 263:
-                format_string = "<7siiidiidqqidddddiidiidiidiidiidiidiidiidiidiiii"
+                format_string = "<7sididdddiiidqqidiidiidiidiidiidiidiidiidiidiiii"
                 unpacked_data = struct.unpack(format_string, packet)
                 exchange = unpacked_data[0].decode("utf-8").rstrip('\x00')
                 data.append({
                     "exchange" : exchange, 
                     "token": unpacked_data[1],
-                    "last_trade_time": unpacked_data[2],
-                    "last_update_time": unpacked_data[3],
-                    "last_trade_price": unpacked_data[4],
-                    "last_trade_quantity": unpacked_data[5],
-                    "volume": unpacked_data[6],
-                    "average_trade_price": unpacked_data[7],
-                    "total_buy_quantity": unpacked_data[8],
-                    "total_sell_quantity": unpacked_data[9],
-                    "open_interest": unpacked_data[10],
-                    "open_price": unpacked_data[11],
-                    "high_price": unpacked_data[12],
-                    "low_price": unpacked_data[13],
-                    "close_price": unpacked_data[14],
+                    "last_trade_price": unpacked_data[2],
+                    "last_trade_time": unpacked_data[3],
+                    "open_price": unpacked_data[4],
+                    "high_price": unpacked_data[5],
+                    "low_price": unpacked_data[6],
+                    "close_price": unpacked_data[7],
+                    "volume": unpacked_data[8],
+                    "last_update_time": unpacked_data[9],
+                    "last_trade_quantity": unpacked_data[10],
+                    "average_trade_price": unpacked_data[11],
+                    "total_buy_quantity": unpacked_data[12],
+                    "total_sell_quantity": unpacked_data[13],
+                    "open_interest": unpacked_data[14],
+                    
                     "depth": {
                         "buy": [{
                             "price": unpacked_data[15],
                             "quantity": unpacked_data[16],
                             "orders": unpacked_data[17],
                         },{
                             "price": unpacked_data[18],
@@ -559,15 +560,17 @@
                             "quantity": unpacked_data[40],
                             "orders": unpacked_data[41],
                         },{
                             "price": unpacked_data[42],
                             "quantity": unpacked_data[43],
                             "orders": unpacked_data[44],
                         }]
-                    }
+                    }, 
+                    "dpr_high": unpacked_data[45],
+                    "dpr_low": unpacked_data[46],
                 })
         return data
 
     def _unpack_int(self, bin, start, end, byte_format="H"):
         """Unpack binary data as unsgined interger."""
         return struct.unpack("<" + byte_format, bin[start:end])[0]
```

### Comparing `vortex_api-1.0.6.dev4/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.6.dev5/vortex_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.6.dev4
+Version: 1.0.6.dev5
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

