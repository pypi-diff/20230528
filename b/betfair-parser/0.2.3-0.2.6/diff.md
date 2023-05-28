# Comparing `tmp/betfair_parser-0.2.3.tar.gz` & `tmp/betfair_parser-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.2.3.tar", max compression
+gzip compressed data, was "betfair_parser-0.2.6.tar", max compression
```

## Comparing `betfair_parser-0.2.3.tar` & `betfair_parser-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0        0 2023-05-24 06:39:57.992048 betfair_parser-0.2.3/betfair_parser/__init__.py
--rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.3/betfair_parser/core.py
--rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.3/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-05-22 03:56:48.978534 betfair_parser-0.2.3/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-05-22 03:56:48.978762 betfair_parser-0.2.3/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3127 2023-05-27 00:39:32.172273 betfair_parser-0.2.3/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-05-27 00:39:32.172518 betfair_parser-0.2.3/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-05-22 03:56:48.979357 betfair_parser-0.2.3/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    20833 2023-05-22 03:56:48.979639 betfair_parser-0.2.3/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9556 2023-05-27 00:39:32.172747 betfair_parser-0.2.3/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-05-22 03:56:48.979989 betfair_parser-0.2.3/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8762 2023-05-27 00:39:32.172968 betfair_parser-0.2.3/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    29242 2023-05-27 00:39:32.173280 betfair_parser-0.2.3/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0     5811 2023-05-27 00:39:32.173519 betfair_parser-0.2.3/betfair_parser/spec/common.py
--rw-r--r--   0        0        0      923 2023-05-27 00:39:32.173730 betfair_parser-0.2.3/betfair_parser/spec/constants.py
--rw-r--r--   0        0        0     7970 2023-05-22 03:56:48.980964 betfair_parser-0.2.3/betfair_parser/spec/error.py
--rw-r--r--   0        0        0     1775 2023-05-27 00:39:32.173931 betfair_parser-0.2.3/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     4181 2023-05-27 00:39:32.174126 betfair_parser-0.2.3/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     2975 2023-05-27 00:39:32.174337 betfair_parser-0.2.3/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.3/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     6233 2023-05-27 00:39:32.174546 betfair_parser-0.2.3/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-05-27 00:39:32.174723 betfair_parser-0.2.3/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2422 2023-05-27 00:39:32.174911 betfair_parser-0.2.3/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.3/betfair_parser/strenums.py
--rw-r--r--   0        0        0      645 2023-05-27 07:33:29.403575 betfair_parser-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/__init__.py
+-rw-r--r--   0        0        0      919 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/core.py
+-rw-r--r--   0        0        0        0 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3127 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    20833 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9556 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8762 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    29242 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0     5811 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/common.py
+-rw-r--r--   0        0        0      923 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/constants.py
+-rw-r--r--   0        0        0     7970 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/error.py
+-rw-r--r--   0        0        0     1775 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     4181 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     2975 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      324 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     6233 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2422 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2148 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      737 2023-05-28 02:35:37.971668 betfair_parser-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 betfair_parser-0.2.6/PKG-INFO
```

### Comparing `betfair_parser-0.2.3/betfair_parser/core.py` & `betfair_parser-0.2.6/betfair_parser/core.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.2.6/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.2.6/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.2.6/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.2.6/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.2.6/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.2.6/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.2.6/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/common.py` & `betfair_parser-0.2.6/betfair_parser/spec/common.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/constants.py` & `betfair_parser-0.2.6/betfair_parser/spec/constants.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/error.py` & `betfair_parser-0.2.6/betfair_parser/spec/error.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.2.6/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/navigation.py` & `betfair_parser-0.2.6/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/race_status.py` & `betfair_parser-0.2.6/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.2.6/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.2.6/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.2.6/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.3/betfair_parser/strenums.py` & `betfair_parser-0.2.6/betfair_parser/strenums.py`

 * *Files identical despite different names*

