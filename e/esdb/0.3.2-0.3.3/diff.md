# Comparing `tmp/esdb-0.3.2.tar.gz` & `tmp/esdb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdb-0.3.2.tar", max compression
+gzip compressed data, was "esdb-0.3.3.tar", max compression
```

## Comparing `esdb-0.3.2.tar` & `esdb-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1069 2023-04-01 11:47:24.583724 esdb-0.3.2/LICENSE
--rw-r--r--   0        0        0     9078 2023-04-01 11:47:24.583965 esdb-0.3.2/README.md
--rw-r--r--   0        0        0       57 2023-04-01 11:47:24.584376 esdb-0.3.2/esdb/__init__.py
--rw-r--r--   0        0        0     9850 2023-04-01 11:47:24.584514 esdb-0.3.2/esdb/client.py
--rw-r--r--   0        0        0     1218 2023-04-01 11:47:24.584615 esdb-0.3.2/esdb/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-01 11:47:24.584708 esdb-0.3.2/esdb/generated/__init__.py
--rw-r--r--   0        0        0    12093 2023-04-01 11:47:24.584861 esdb-0.3.2/esdb/generated/cluster_pb2.py
--rw-r--r--   0        0        0    32744 2023-04-01 11:47:24.585027 esdb-0.3.2/esdb/generated/cluster_pb2.pyi
--rw-r--r--   0        0        0    16685 2023-04-01 11:47:24.585162 esdb-0.3.2/esdb/generated/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1737 2023-04-01 11:47:24.585303 esdb-0.3.2/esdb/generated/code_pb2.py
--rw-r--r--   0        0        0    13544 2023-04-01 11:47:24.585446 esdb-0.3.2/esdb/generated/code_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-01 11:47:24.585554 esdb-0.3.2/esdb/generated/code_pb2_grpc.py
--rw-r--r--   0        0        0     2587 2023-04-01 11:47:24.585680 esdb-0.3.2/esdb/generated/gossip_pb2.py
--rw-r--r--   0        0        0     5145 2023-04-01 11:47:24.585770 esdb-0.3.2/esdb/generated/gossip_pb2.pyi
--rw-r--r--   0        0        0     2405 2023-04-01 11:47:24.585865 esdb-0.3.2/esdb/generated/gossip_pb2_grpc.py
--rw-r--r--   0        0        0     1835 2023-04-01 11:47:24.586038 esdb-0.3.2/esdb/generated/monitoring_pb2.py
--rw-r--r--   0        0        0     2163 2023-04-01 11:47:24.586157 esdb-0.3.2/esdb/generated/monitoring_pb2.pyi
--rw-r--r--   0        0        0     2450 2023-04-01 11:47:24.586255 esdb-0.3.2/esdb/generated/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     3278 2023-04-01 11:47:24.586350 esdb-0.3.2/esdb/generated/operations_pb2.py
--rw-r--r--   0        0        0     4731 2023-04-01 11:47:24.586445 esdb-0.3.2/esdb/generated/operations_pb2.pyi
--rw-r--r--   0        0        0    11771 2023-04-01 11:47:24.586551 esdb-0.3.2/esdb/generated/operations_pb2_grpc.py
--rw-r--r--   0        0        0    20587 2023-04-01 11:47:24.586638 esdb-0.3.2/esdb/generated/persistent_pb2.py
--rw-r--r--   0        0        0    58720 2023-04-01 11:47:24.586903 esdb-0.3.2/esdb/generated/persistent_pb2.pyi
--rw-r--r--   0        0        0    13623 2023-04-01 11:47:24.587024 esdb-0.3.2/esdb/generated/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     8971 2023-04-01 11:47:24.587149 esdb-0.3.2/esdb/generated/projections_pb2.py
--rw-r--r--   0        0        0    22084 2023-04-01 11:47:24.587299 esdb-0.3.2/esdb/generated/projections_pb2.pyi
--rw-r--r--   0        0        0    16190 2023-04-01 11:47:24.587407 esdb-0.3.2/esdb/generated/projections_pb2_grpc.py
--rw-r--r--   0        0        0     1789 2023-04-01 11:47:24.587548 esdb-0.3.2/esdb/generated/serverfeatures_pb2.py
--rw-r--r--   0        0        0     2095 2023-04-01 11:47:24.587638 esdb-0.3.2/esdb/generated/serverfeatures_pb2.pyi
--rw-r--r--   0        0        0     2648 2023-04-01 11:47:24.587730 esdb-0.3.2/esdb/generated/serverfeatures_pb2_grpc.py
--rw-r--r--   0        0        0     3511 2023-04-01 11:47:24.587835 esdb-0.3.2/esdb/generated/shared_pb2.py
--rw-r--r--   0        0        0     8801 2023-04-01 11:47:24.587942 esdb-0.3.2/esdb/generated/shared_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-01 11:47:24.588031 esdb-0.3.2/esdb/generated/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1522 2023-04-01 11:47:24.588120 esdb-0.3.2/esdb/generated/status_pb2.py
--rw-r--r--   0        0        0     2710 2023-04-01 11:47:24.588238 esdb-0.3.2/esdb/generated/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-01 11:47:24.588337 esdb-0.3.2/esdb/generated/status_pb2_grpc.py
--rw-r--r--   0        0        0    18369 2023-04-01 11:47:24.588446 esdb-0.3.2/esdb/generated/streams_pb2.py
--rw-r--r--   0        0        0    55248 2023-04-01 11:47:24.588689 esdb-0.3.2/esdb/generated/streams_pb2.pyi
--rw-r--r--   0        0        0     8442 2023-04-01 11:47:24.588802 esdb-0.3.2/esdb/generated/streams_pb2_grpc.py
--rw-r--r--   0        0        0     6362 2023-04-01 11:47:24.588895 esdb-0.3.2/esdb/generated/users_pb2.py
--rw-r--r--   0        0        0    14660 2023-04-01 11:47:24.589004 esdb-0.3.2/esdb/generated/users_pb2.pyi
--rw-r--r--   0        0        0    12765 2023-04-01 11:47:24.589118 esdb-0.3.2/esdb/generated/users_pb2_grpc.py
--rw-r--r--   0        0        0     1700 2023-04-01 11:47:24.589225 esdb-0.3.2/esdb/gossip.py
--rw-r--r--   0        0        0     1407 2023-04-01 11:47:24.589325 esdb-0.3.2/esdb/shared.py
--rw-r--r--   0        0        0      142 2023-04-01 11:47:24.589468 esdb-0.3.2/esdb/streams/__init__.py
--rw-r--r--   0        0        0    10227 2023-04-01 11:54:15.669952 esdb-0.3.2/esdb/streams/streams.py
--rw-r--r--   0        0        0     4466 2023-04-01 11:47:24.589700 esdb-0.3.2/esdb/streams/types.py
--rw-r--r--   0        0        0      232 2023-04-01 11:47:24.589856 esdb-0.3.2/esdb/subscriptions/__init__.py
--rw-r--r--   0        0        0     8611 2023-04-01 11:47:24.589972 esdb-0.3.2/esdb/subscriptions/subscriptions.py
--rw-r--r--   0        0        0     7583 2023-04-01 11:47:24.590085 esdb-0.3.2/esdb/subscriptions/types.py
--rw-r--r--   0        0        0     1507 2023-04-02 09:43:01.038761 esdb-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9826 1970-01-01 00:00:00.000000 esdb-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-01 11:47:24.583724 esdb-0.3.3/LICENSE
+-rw-r--r--   0        0        0     9078 2023-05-28 14:29:30.174032 esdb-0.3.3/README.md
+-rw-r--r--   0        0        0       57 2023-04-01 11:47:24.584376 esdb-0.3.3/esdb/__init__.py
+-rw-r--r--   0        0        0     9850 2023-04-01 11:47:24.584514 esdb-0.3.3/esdb/client.py
+-rw-r--r--   0        0        0     1218 2023-04-01 11:47:24.584615 esdb-0.3.3/esdb/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:24:47.850336 esdb-0.3.3/esdb/generated/__init__.py
+-rw-r--r--   0        0        0    12093 2023-04-24 20:24:47.850642 esdb-0.3.3/esdb/generated/cluster_pb2.py
+-rw-r--r--   0        0        0    32744 2023-04-24 20:24:47.851219 esdb-0.3.3/esdb/generated/cluster_pb2.pyi
+-rw-r--r--   0        0        0    16685 2023-04-24 20:24:47.851610 esdb-0.3.3/esdb/generated/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1737 2023-04-24 20:24:47.851838 esdb-0.3.3/esdb/generated/code_pb2.py
+-rw-r--r--   0        0        0    13544 2023-04-24 20:24:47.852125 esdb-0.3.3/esdb/generated/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 20:24:47.852333 esdb-0.3.3/esdb/generated/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2587 2023-04-24 20:24:47.852507 esdb-0.3.3/esdb/generated/gossip_pb2.py
+-rw-r--r--   0        0        0     5145 2023-04-24 20:24:47.852754 esdb-0.3.3/esdb/generated/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2405 2023-04-24 20:24:47.852978 esdb-0.3.3/esdb/generated/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0     1835 2023-04-24 20:24:47.853155 esdb-0.3.3/esdb/generated/monitoring_pb2.py
+-rw-r--r--   0        0        0     2163 2023-04-24 20:24:47.853335 esdb-0.3.3/esdb/generated/monitoring_pb2.pyi
+-rw-r--r--   0        0        0     2450 2023-04-24 20:24:47.853504 esdb-0.3.3/esdb/generated/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     3278 2023-04-24 20:24:47.853664 esdb-0.3.3/esdb/generated/operations_pb2.py
+-rw-r--r--   0        0        0     4731 2023-04-24 20:24:47.853863 esdb-0.3.3/esdb/generated/operations_pb2.pyi
+-rw-r--r--   0        0        0    11771 2023-04-24 20:24:47.854174 esdb-0.3.3/esdb/generated/operations_pb2_grpc.py
+-rw-r--r--   0        0        0    20587 2023-04-24 20:24:47.854426 esdb-0.3.3/esdb/generated/persistent_pb2.py
+-rw-r--r--   0        0        0    58720 2023-04-24 20:24:47.855085 esdb-0.3.3/esdb/generated/persistent_pb2.pyi
+-rw-r--r--   0        0        0    13623 2023-04-24 20:24:47.855401 esdb-0.3.3/esdb/generated/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     8971 2023-04-24 20:24:47.855629 esdb-0.3.3/esdb/generated/projections_pb2.py
+-rw-r--r--   0        0        0    22084 2023-04-24 20:24:47.856039 esdb-0.3.3/esdb/generated/projections_pb2.pyi
+-rw-r--r--   0        0        0    16190 2023-04-24 20:24:47.856372 esdb-0.3.3/esdb/generated/projections_pb2_grpc.py
+-rw-r--r--   0        0        0     1789 2023-04-24 20:24:47.856582 esdb-0.3.3/esdb/generated/serverfeatures_pb2.py
+-rw-r--r--   0        0        0     2095 2023-04-24 20:24:47.856773 esdb-0.3.3/esdb/generated/serverfeatures_pb2.pyi
+-rw-r--r--   0        0        0     2648 2023-04-24 20:24:47.856998 esdb-0.3.3/esdb/generated/serverfeatures_pb2_grpc.py
+-rw-r--r--   0        0        0     3511 2023-04-24 20:24:47.857185 esdb-0.3.3/esdb/generated/shared_pb2.py
+-rw-r--r--   0        0        0     8801 2023-04-24 20:24:47.857432 esdb-0.3.3/esdb/generated/shared_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 20:24:47.857589 esdb-0.3.3/esdb/generated/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1522 2023-04-24 20:24:47.857758 esdb-0.3.3/esdb/generated/status_pb2.py
+-rw-r--r--   0        0        0     2710 2023-04-24 20:24:47.857929 esdb-0.3.3/esdb/generated/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 20:24:47.858066 esdb-0.3.3/esdb/generated/status_pb2_grpc.py
+-rw-r--r--   0        0        0    18369 2023-04-24 20:24:47.858313 esdb-0.3.3/esdb/generated/streams_pb2.py
+-rw-r--r--   0        0        0    55248 2023-04-24 20:24:47.859017 esdb-0.3.3/esdb/generated/streams_pb2.pyi
+-rw-r--r--   0        0        0     8442 2023-04-24 20:24:47.859299 esdb-0.3.3/esdb/generated/streams_pb2_grpc.py
+-rw-r--r--   0        0        0     6362 2023-04-24 20:24:47.859494 esdb-0.3.3/esdb/generated/users_pb2.py
+-rw-r--r--   0        0        0    14660 2023-04-24 20:24:47.859805 esdb-0.3.3/esdb/generated/users_pb2.pyi
+-rw-r--r--   0        0        0    12765 2023-04-24 20:24:47.860113 esdb-0.3.3/esdb/generated/users_pb2_grpc.py
+-rw-r--r--   0        0        0     1700 2023-04-01 11:47:24.589225 esdb-0.3.3/esdb/gossip.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:43:51.488972 esdb-0.3.3/esdb/py.typed
+-rw-r--r--   0        0        0     1407 2023-04-01 11:47:24.589325 esdb-0.3.3/esdb/shared.py
+-rw-r--r--   0        0        0      142 2023-04-01 11:47:24.589468 esdb-0.3.3/esdb/streams/__init__.py
+-rw-r--r--   0        0        0    10227 2023-04-01 11:54:15.669952 esdb-0.3.3/esdb/streams/streams.py
+-rw-r--r--   0        0        0     4466 2023-04-01 11:47:24.589700 esdb-0.3.3/esdb/streams/types.py
+-rw-r--r--   0        0        0      232 2023-04-01 11:47:24.589856 esdb-0.3.3/esdb/subscriptions/__init__.py
+-rw-r--r--   0        0        0     8611 2023-04-01 11:47:24.589972 esdb-0.3.3/esdb/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0     7583 2023-04-01 11:47:24.590085 esdb-0.3.3/esdb/subscriptions/types.py
+-rw-r--r--   0        0        0     1509 2023-05-28 14:44:02.431940 esdb-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9826 1970-01-01 00:00:00.000000 esdb-0.3.3/PKG-INFO
```

### Comparing `esdb-0.3.2/LICENSE` & `esdb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/README.md` & `esdb-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/client.py` & `esdb-0.3.3/esdb/client.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/exceptions.py` & `esdb-0.3.3/esdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/cluster_pb2.py` & `esdb-0.3.3/esdb/generated/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/cluster_pb2.pyi` & `esdb-0.3.3/esdb/generated/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/cluster_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/code_pb2.py` & `esdb-0.3.3/esdb/generated/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/code_pb2.pyi` & `esdb-0.3.3/esdb/generated/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/gossip_pb2.py` & `esdb-0.3.3/esdb/generated/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/gossip_pb2.pyi` & `esdb-0.3.3/esdb/generated/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/gossip_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/monitoring_pb2.py` & `esdb-0.3.3/esdb/generated/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/monitoring_pb2.pyi` & `esdb-0.3.3/esdb/generated/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/monitoring_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/operations_pb2.py` & `esdb-0.3.3/esdb/generated/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/operations_pb2.pyi` & `esdb-0.3.3/esdb/generated/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/operations_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/persistent_pb2.py` & `esdb-0.3.3/esdb/generated/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/persistent_pb2.pyi` & `esdb-0.3.3/esdb/generated/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/persistent_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/projections_pb2.py` & `esdb-0.3.3/esdb/generated/projections_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/projections_pb2.pyi` & `esdb-0.3.3/esdb/generated/projections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/projections_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/projections_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/serverfeatures_pb2.py` & `esdb-0.3.3/esdb/generated/serverfeatures_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/serverfeatures_pb2.pyi` & `esdb-0.3.3/esdb/generated/serverfeatures_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/serverfeatures_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/serverfeatures_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/shared_pb2.py` & `esdb-0.3.3/esdb/generated/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/shared_pb2.pyi` & `esdb-0.3.3/esdb/generated/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/status_pb2.py` & `esdb-0.3.3/esdb/generated/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/status_pb2.pyi` & `esdb-0.3.3/esdb/generated/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/streams_pb2.py` & `esdb-0.3.3/esdb/generated/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/streams_pb2.pyi` & `esdb-0.3.3/esdb/generated/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/streams_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/users_pb2.py` & `esdb-0.3.3/esdb/generated/users_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/users_pb2.pyi` & `esdb-0.3.3/esdb/generated/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/generated/users_pb2_grpc.py` & `esdb-0.3.3/esdb/generated/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/gossip.py` & `esdb-0.3.3/esdb/gossip.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/shared.py` & `esdb-0.3.3/esdb/shared.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/streams/streams.py` & `esdb-0.3.3/esdb/streams/streams.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/streams/types.py` & `esdb-0.3.3/esdb/streams/types.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/subscriptions/subscriptions.py` & `esdb-0.3.3/esdb/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/esdb/subscriptions/types.py` & `esdb-0.3.3/esdb/subscriptions/types.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.2/pyproject.toml` & `esdb-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdb"
-version = "0.3.2"
+version = "0.3.3"
 description = "gRPC client for EventStore DB"
 authors = ["Andrii Kohut <kogut.andriy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andriykohut/esdb-py"
 repository = "https://github.com/andriykohut/esdb-py"
 keywords = ["eventstore", "esdb", "event sourcing", "cqrs", "event-sourcing", "grpcio", "grpc"]
@@ -13,27 +13,27 @@
     { include = "esdb" },
 ]
 
 exclude = ["EventStore", "certs", "es_config", "protos"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-grpcio = "^1.50.0"
-protobuf = "^4.21.8"
+grpcio = "^1.53.0"
+protobuf = "^4.22.1"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.982,<1.2"
+mypy = ">=0.982,<1.4"
 mypy-protobuf = "^3.4.0"
 black = ">=22.10,<24.0"
-pytest = "^7.2.0"
-isort = "^5.10.1"
+pytest = "^7.2.2"
+isort = "^5.12.0"
 pytest-asyncio = ">=0.19,<0.22"
 flake8 = ">=5.0.4,<7.0.0"
-grpcio-tools = "^1.50.0"
-grpc-stubs = "^1.24.11"
+grpcio-tools = "^1.53.0"
+grpc-stubs = "^1.24.12.1"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `esdb-0.3.2/PKG-INFO` & `esdb-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: esdb
-Version: 0.3.2
+Version: 0.3.3
 Summary: gRPC client for EventStore DB
 Home-page: https://github.com/andriykohut/esdb-py
 License: MIT
 Keywords: eventstore,esdb,event sourcing,cqrs,event-sourcing,grpcio,grpc
 Author: Andrii Kohut
 Author-email: kogut.andriy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grpcio (>=1.50.0,<2.0.0)
-Requires-Dist: protobuf (>=4.21.8,<5.0.0)
+Requires-Dist: grpcio (>=1.53.0,<2.0.0)
+Requires-Dist: protobuf (>=4.22.1,<5.0.0)
 Project-URL: Repository, https://github.com/andriykohut/esdb-py
 Description-Content-Type: text/markdown
 
 # esdb-py
 
 [![PyPI version](https://badge.fury.io/py/esdb.svg)](https://pypi.org/project/esdb/)
 [![codecov](https://codecov.io/gh/andriykohut/esdb-py/branch/main/graph/badge.svg?token=YVDPTDBPFB)](https://codecov.io/gh/andriykohut/esdb-py)
```

