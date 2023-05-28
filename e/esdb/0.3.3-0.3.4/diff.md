# Comparing `tmp/esdb-0.3.3.tar.gz` & `tmp/esdb-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdb-0.3.3.tar", max compression
+gzip compressed data, was "esdb-0.3.4.tar", max compression
```

## Comparing `esdb-0.3.3.tar` & `esdb-0.3.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1069 2023-04-01 11:47:24.583724 esdb-0.3.3/LICENSE
--rw-r--r--   0        0        0     9078 2023-05-28 14:29:30.174032 esdb-0.3.3/README.md
--rw-r--r--   0        0        0       57 2023-04-01 11:47:24.584376 esdb-0.3.3/esdb/__init__.py
--rw-r--r--   0        0        0     9850 2023-04-01 11:47:24.584514 esdb-0.3.3/esdb/client.py
--rw-r--r--   0        0        0     1218 2023-04-01 11:47:24.584615 esdb-0.3.3/esdb/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:47.850336 esdb-0.3.3/esdb/generated/__init__.py
--rw-r--r--   0        0        0    12093 2023-04-24 20:24:47.850642 esdb-0.3.3/esdb/generated/cluster_pb2.py
--rw-r--r--   0        0        0    32744 2023-04-24 20:24:47.851219 esdb-0.3.3/esdb/generated/cluster_pb2.pyi
--rw-r--r--   0        0        0    16685 2023-04-24 20:24:47.851610 esdb-0.3.3/esdb/generated/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1737 2023-04-24 20:24:47.851838 esdb-0.3.3/esdb/generated/code_pb2.py
--rw-r--r--   0        0        0    13544 2023-04-24 20:24:47.852125 esdb-0.3.3/esdb/generated/code_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 20:24:47.852333 esdb-0.3.3/esdb/generated/code_pb2_grpc.py
--rw-r--r--   0        0        0     2587 2023-04-24 20:24:47.852507 esdb-0.3.3/esdb/generated/gossip_pb2.py
--rw-r--r--   0        0        0     5145 2023-04-24 20:24:47.852754 esdb-0.3.3/esdb/generated/gossip_pb2.pyi
--rw-r--r--   0        0        0     2405 2023-04-24 20:24:47.852978 esdb-0.3.3/esdb/generated/gossip_pb2_grpc.py
--rw-r--r--   0        0        0     1835 2023-04-24 20:24:47.853155 esdb-0.3.3/esdb/generated/monitoring_pb2.py
--rw-r--r--   0        0        0     2163 2023-04-24 20:24:47.853335 esdb-0.3.3/esdb/generated/monitoring_pb2.pyi
--rw-r--r--   0        0        0     2450 2023-04-24 20:24:47.853504 esdb-0.3.3/esdb/generated/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     3278 2023-04-24 20:24:47.853664 esdb-0.3.3/esdb/generated/operations_pb2.py
--rw-r--r--   0        0        0     4731 2023-04-24 20:24:47.853863 esdb-0.3.3/esdb/generated/operations_pb2.pyi
--rw-r--r--   0        0        0    11771 2023-04-24 20:24:47.854174 esdb-0.3.3/esdb/generated/operations_pb2_grpc.py
--rw-r--r--   0        0        0    20587 2023-04-24 20:24:47.854426 esdb-0.3.3/esdb/generated/persistent_pb2.py
--rw-r--r--   0        0        0    58720 2023-04-24 20:24:47.855085 esdb-0.3.3/esdb/generated/persistent_pb2.pyi
--rw-r--r--   0        0        0    13623 2023-04-24 20:24:47.855401 esdb-0.3.3/esdb/generated/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     8971 2023-04-24 20:24:47.855629 esdb-0.3.3/esdb/generated/projections_pb2.py
--rw-r--r--   0        0        0    22084 2023-04-24 20:24:47.856039 esdb-0.3.3/esdb/generated/projections_pb2.pyi
--rw-r--r--   0        0        0    16190 2023-04-24 20:24:47.856372 esdb-0.3.3/esdb/generated/projections_pb2_grpc.py
--rw-r--r--   0        0        0     1789 2023-04-24 20:24:47.856582 esdb-0.3.3/esdb/generated/serverfeatures_pb2.py
--rw-r--r--   0        0        0     2095 2023-04-24 20:24:47.856773 esdb-0.3.3/esdb/generated/serverfeatures_pb2.pyi
--rw-r--r--   0        0        0     2648 2023-04-24 20:24:47.856998 esdb-0.3.3/esdb/generated/serverfeatures_pb2_grpc.py
--rw-r--r--   0        0        0     3511 2023-04-24 20:24:47.857185 esdb-0.3.3/esdb/generated/shared_pb2.py
--rw-r--r--   0        0        0     8801 2023-04-24 20:24:47.857432 esdb-0.3.3/esdb/generated/shared_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 20:24:47.857589 esdb-0.3.3/esdb/generated/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1522 2023-04-24 20:24:47.857758 esdb-0.3.3/esdb/generated/status_pb2.py
--rw-r--r--   0        0        0     2710 2023-04-24 20:24:47.857929 esdb-0.3.3/esdb/generated/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 20:24:47.858066 esdb-0.3.3/esdb/generated/status_pb2_grpc.py
--rw-r--r--   0        0        0    18369 2023-04-24 20:24:47.858313 esdb-0.3.3/esdb/generated/streams_pb2.py
--rw-r--r--   0        0        0    55248 2023-04-24 20:24:47.859017 esdb-0.3.3/esdb/generated/streams_pb2.pyi
--rw-r--r--   0        0        0     8442 2023-04-24 20:24:47.859299 esdb-0.3.3/esdb/generated/streams_pb2_grpc.py
--rw-r--r--   0        0        0     6362 2023-04-24 20:24:47.859494 esdb-0.3.3/esdb/generated/users_pb2.py
--rw-r--r--   0        0        0    14660 2023-04-24 20:24:47.859805 esdb-0.3.3/esdb/generated/users_pb2.pyi
--rw-r--r--   0        0        0    12765 2023-04-24 20:24:47.860113 esdb-0.3.3/esdb/generated/users_pb2_grpc.py
--rw-r--r--   0        0        0     1700 2023-04-01 11:47:24.589225 esdb-0.3.3/esdb/gossip.py
--rw-r--r--   0        0        0        0 2023-05-28 14:43:51.488972 esdb-0.3.3/esdb/py.typed
--rw-r--r--   0        0        0     1407 2023-04-01 11:47:24.589325 esdb-0.3.3/esdb/shared.py
--rw-r--r--   0        0        0      142 2023-04-01 11:47:24.589468 esdb-0.3.3/esdb/streams/__init__.py
--rw-r--r--   0        0        0    10227 2023-04-01 11:54:15.669952 esdb-0.3.3/esdb/streams/streams.py
--rw-r--r--   0        0        0     4466 2023-04-01 11:47:24.589700 esdb-0.3.3/esdb/streams/types.py
--rw-r--r--   0        0        0      232 2023-04-01 11:47:24.589856 esdb-0.3.3/esdb/subscriptions/__init__.py
--rw-r--r--   0        0        0     8611 2023-04-01 11:47:24.589972 esdb-0.3.3/esdb/subscriptions/subscriptions.py
--rw-r--r--   0        0        0     7583 2023-04-01 11:47:24.590085 esdb-0.3.3/esdb/subscriptions/types.py
--rw-r--r--   0        0        0     1509 2023-05-28 14:44:02.431940 esdb-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9826 1970-01-01 00:00:00.000000 esdb-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-01 11:47:24.583724 esdb-0.3.4/LICENSE
+-rw-r--r--   0        0        0     9078 2023-05-28 14:29:30.174032 esdb-0.3.4/README.md
+-rw-r--r--   0        0        0       57 2023-04-01 11:47:24.584376 esdb-0.3.4/esdb/__init__.py
+-rw-r--r--   0        0        0     9833 2023-05-28 15:22:09.222358 esdb-0.3.4/esdb/client.py
+-rw-r--r--   0        0        0     1218 2023-04-01 11:47:24.584615 esdb-0.3.4/esdb/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-28 15:17:17.560178 esdb-0.3.4/esdb/generated/__init__.py
+-rw-r--r--   0        0        0    12093 2023-05-28 15:17:17.560446 esdb-0.3.4/esdb/generated/cluster_pb2.py
+-rw-r--r--   0        0        0    32744 2023-05-28 15:17:17.560993 esdb-0.3.4/esdb/generated/cluster_pb2.pyi
+-rw-r--r--   0        0        0    16685 2023-05-28 15:17:17.561330 esdb-0.3.4/esdb/generated/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1737 2023-05-28 15:17:17.561550 esdb-0.3.4/esdb/generated/code_pb2.py
+-rw-r--r--   0        0        0    13544 2023-05-28 15:17:17.561832 esdb-0.3.4/esdb/generated/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 15:17:17.562017 esdb-0.3.4/esdb/generated/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2587 2023-05-28 15:17:17.562173 esdb-0.3.4/esdb/generated/gossip_pb2.py
+-rw-r--r--   0        0        0     5145 2023-05-28 15:17:17.562358 esdb-0.3.4/esdb/generated/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2405 2023-05-28 15:17:17.562533 esdb-0.3.4/esdb/generated/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0     1835 2023-05-28 15:17:17.562709 esdb-0.3.4/esdb/generated/monitoring_pb2.py
+-rw-r--r--   0        0        0     2163 2023-05-28 15:17:17.562907 esdb-0.3.4/esdb/generated/monitoring_pb2.pyi
+-rw-r--r--   0        0        0     2450 2023-05-28 15:17:17.563074 esdb-0.3.4/esdb/generated/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     3278 2023-05-28 15:17:17.563235 esdb-0.3.4/esdb/generated/operations_pb2.py
+-rw-r--r--   0        0        0     4731 2023-05-28 15:17:17.563446 esdb-0.3.4/esdb/generated/operations_pb2.pyi
+-rw-r--r--   0        0        0    11771 2023-05-28 15:17:17.563750 esdb-0.3.4/esdb/generated/operations_pb2_grpc.py
+-rw-r--r--   0        0        0    20587 2023-05-28 15:17:17.564000 esdb-0.3.4/esdb/generated/persistent_pb2.py
+-rw-r--r--   0        0        0    58720 2023-05-28 15:17:17.564666 esdb-0.3.4/esdb/generated/persistent_pb2.pyi
+-rw-r--r--   0        0        0    13623 2023-05-28 15:17:17.564998 esdb-0.3.4/esdb/generated/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     8971 2023-05-28 15:17:17.565235 esdb-0.3.4/esdb/generated/projections_pb2.py
+-rw-r--r--   0        0        0    22084 2023-05-28 15:17:17.565624 esdb-0.3.4/esdb/generated/projections_pb2.pyi
+-rw-r--r--   0        0        0    16190 2023-05-28 15:17:17.565940 esdb-0.3.4/esdb/generated/projections_pb2_grpc.py
+-rw-r--r--   0        0        0     1789 2023-05-28 15:17:17.566123 esdb-0.3.4/esdb/generated/serverfeatures_pb2.py
+-rw-r--r--   0        0        0     2095 2023-05-28 15:17:17.566285 esdb-0.3.4/esdb/generated/serverfeatures_pb2.pyi
+-rw-r--r--   0        0        0     2648 2023-05-28 15:17:17.566481 esdb-0.3.4/esdb/generated/serverfeatures_pb2_grpc.py
+-rw-r--r--   0        0        0     3511 2023-05-28 15:17:17.566645 esdb-0.3.4/esdb/generated/shared_pb2.py
+-rw-r--r--   0        0        0     8801 2023-05-28 15:17:17.566914 esdb-0.3.4/esdb/generated/shared_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 15:17:17.567070 esdb-0.3.4/esdb/generated/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1522 2023-05-28 15:17:17.567222 esdb-0.3.4/esdb/generated/status_pb2.py
+-rw-r--r--   0        0        0     2710 2023-05-28 15:17:17.567382 esdb-0.3.4/esdb/generated/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-28 15:17:17.567520 esdb-0.3.4/esdb/generated/status_pb2_grpc.py
+-rw-r--r--   0        0        0    18369 2023-05-28 15:17:17.567742 esdb-0.3.4/esdb/generated/streams_pb2.py
+-rw-r--r--   0        0        0    55248 2023-05-28 15:17:17.568399 esdb-0.3.4/esdb/generated/streams_pb2.pyi
+-rw-r--r--   0        0        0     8442 2023-05-28 15:17:17.568649 esdb-0.3.4/esdb/generated/streams_pb2_grpc.py
+-rw-r--r--   0        0        0     6362 2023-05-28 15:17:17.568863 esdb-0.3.4/esdb/generated/users_pb2.py
+-rw-r--r--   0        0        0    14660 2023-05-28 15:17:17.569178 esdb-0.3.4/esdb/generated/users_pb2.pyi
+-rw-r--r--   0        0        0    12765 2023-05-28 15:17:17.569487 esdb-0.3.4/esdb/generated/users_pb2_grpc.py
+-rw-r--r--   0        0        0     1700 2023-04-01 11:47:24.589225 esdb-0.3.4/esdb/gossip.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:43:51.488972 esdb-0.3.4/esdb/py.typed
+-rw-r--r--   0        0        0     1407 2023-04-01 11:47:24.589325 esdb-0.3.4/esdb/shared.py
+-rw-r--r--   0        0        0      142 2023-04-01 11:47:24.589468 esdb-0.3.4/esdb/streams/__init__.py
+-rw-r--r--   0        0        0    10227 2023-04-01 11:54:15.669952 esdb-0.3.4/esdb/streams/streams.py
+-rw-r--r--   0        0        0     4466 2023-04-01 11:47:24.589700 esdb-0.3.4/esdb/streams/types.py
+-rw-r--r--   0        0        0      232 2023-04-01 11:47:24.589856 esdb-0.3.4/esdb/subscriptions/__init__.py
+-rw-r--r--   0        0        0     8611 2023-04-01 11:47:24.589972 esdb-0.3.4/esdb/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0     7583 2023-04-01 11:47:24.590085 esdb-0.3.4/esdb/subscriptions/types.py
+-rw-r--r--   0        0        0     1543 2023-05-28 15:22:14.133920 esdb-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9808 1970-01-01 00:00:00.000000 esdb-0.3.4/PKG-INFO
```

### Comparing `esdb-0.3.3/LICENSE` & `esdb-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/README.md` & `esdb-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/client.py` & `esdb-0.3.4/esdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import base64
 import contextlib
 import enum
 import itertools
 import logging
 import random
 import urllib.parse
+from collections.abc import AsyncIterator
 from dataclasses import dataclass
 from functools import cmp_to_key
-from typing import AsyncContextManager, Optional
+from typing import Optional
 
 import grpc
 
 from esdb.exceptions import DiscoveryError
 from esdb.generated.gossip_pb2_grpc import GossipStub
 from esdb.generated.persistent_pb2_grpc import PersistentSubscriptionsStub
 from esdb.generated.streams_pb2_grpc import StreamsStub
@@ -226,16 +227,16 @@
             if self.call_credentials
             else self.channel_credentials
         )
         return grpc.aio.secure_channel(  # type: ignore
             f"{endpoint.address}:{endpoint.port}", credentials, self.options
         )
 
-    @contextlib.asynccontextmanager  # type: ignore
-    async def connect(self) -> AsyncContextManager[Connection]:  # type: ignore
+    @contextlib.asynccontextmanager
+    async def connect(self) -> AsyncIterator[Connection]:
         if self.config.dns_discover:
             endpoint = await self.discover_endpoint()
         else:
             assert self.config.address
             endpoint = self.config.address
 
         async with self._create_channel(endpoint) as channel:
```

### Comparing `esdb-0.3.3/esdb/exceptions.py` & `esdb-0.3.4/esdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/cluster_pb2.py` & `esdb-0.3.4/esdb/generated/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/cluster_pb2.pyi` & `esdb-0.3.4/esdb/generated/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/cluster_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/code_pb2.py` & `esdb-0.3.4/esdb/generated/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/code_pb2.pyi` & `esdb-0.3.4/esdb/generated/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/gossip_pb2.py` & `esdb-0.3.4/esdb/generated/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/gossip_pb2.pyi` & `esdb-0.3.4/esdb/generated/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/gossip_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/monitoring_pb2.py` & `esdb-0.3.4/esdb/generated/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/monitoring_pb2.pyi` & `esdb-0.3.4/esdb/generated/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/monitoring_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/operations_pb2.py` & `esdb-0.3.4/esdb/generated/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/operations_pb2.pyi` & `esdb-0.3.4/esdb/generated/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/operations_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/persistent_pb2.py` & `esdb-0.3.4/esdb/generated/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/persistent_pb2.pyi` & `esdb-0.3.4/esdb/generated/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/persistent_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/projections_pb2.py` & `esdb-0.3.4/esdb/generated/projections_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/projections_pb2.pyi` & `esdb-0.3.4/esdb/generated/projections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/projections_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/projections_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/serverfeatures_pb2.py` & `esdb-0.3.4/esdb/generated/serverfeatures_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/serverfeatures_pb2.pyi` & `esdb-0.3.4/esdb/generated/serverfeatures_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/serverfeatures_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/serverfeatures_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/shared_pb2.py` & `esdb-0.3.4/esdb/generated/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/shared_pb2.pyi` & `esdb-0.3.4/esdb/generated/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/status_pb2.py` & `esdb-0.3.4/esdb/generated/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/status_pb2.pyi` & `esdb-0.3.4/esdb/generated/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/streams_pb2.py` & `esdb-0.3.4/esdb/generated/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/streams_pb2.pyi` & `esdb-0.3.4/esdb/generated/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/streams_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/users_pb2.py` & `esdb-0.3.4/esdb/generated/users_pb2.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/users_pb2.pyi` & `esdb-0.3.4/esdb/generated/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/generated/users_pb2_grpc.py` & `esdb-0.3.4/esdb/generated/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/gossip.py` & `esdb-0.3.4/esdb/gossip.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/shared.py` & `esdb-0.3.4/esdb/shared.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/streams/streams.py` & `esdb-0.3.4/esdb/streams/streams.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/streams/types.py` & `esdb-0.3.4/esdb/streams/types.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/subscriptions/subscriptions.py` & `esdb-0.3.4/esdb/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/esdb/subscriptions/types.py` & `esdb-0.3.4/esdb/subscriptions/types.py`

 * *Files identical despite different names*

### Comparing `esdb-0.3.3/pyproject.toml` & `esdb-0.3.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdb"
-version = "0.3.3"
+version = "0.3.4"
 description = "gRPC client for EventStore DB"
 authors = ["Andrii Kohut <kogut.andriy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andriykohut/esdb-py"
 repository = "https://github.com/andriykohut/esdb-py"
 keywords = ["eventstore", "esdb", "event sourcing", "cqrs", "event-sourcing", "grpcio", "grpc"]
@@ -13,28 +13,28 @@
     { include = "esdb" },
 ]
 
 exclude = ["EventStore", "certs", "es_config", "protos"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-grpcio = "^1.53.0"
-protobuf = "^4.22.1"
+grpcio = ">=1.4.0"
+protobuf = ">=4.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.982,<1.4"
+mypy = "^1.3.0"
 mypy-protobuf = "^3.4.0"
-black = ">=22.10,<24.0"
-pytest = "^7.2.2"
+black = "^23.3.0"
+pytest = "^7.3.1"
 isort = "^5.12.0"
-pytest-asyncio = ">=0.19,<0.22"
-flake8 = ">=5.0.4,<7.0.0"
-grpcio-tools = "^1.53.0"
-grpc-stubs = "^1.24.12.1"
-pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.0"
+grpcio-tools = "^1.54.2"
+grpc-stubs = "^1.53.0.2"
+pytest-cov = "^4.1.0"
+ruff = "^0.0.270"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 exclude = ["esdb/generated"]
@@ -62,7 +62,11 @@
     "pragma: no cover",
     "def __repr__",
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "@(abc.)?abstractmethod",
 ]
+
+[tool.ruff]
+line-length = 119
+exclude = ["esdb/generated/*"]
```

### Comparing `esdb-0.3.3/PKG-INFO` & `esdb-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: esdb
-Version: 0.3.3
+Version: 0.3.4
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
-Requires-Dist: grpcio (>=1.53.0,<2.0.0)
-Requires-Dist: protobuf (>=4.22.1,<5.0.0)
+Requires-Dist: grpcio (>=1.4.0)
+Requires-Dist: protobuf (>=4.0)
 Project-URL: Repository, https://github.com/andriykohut/esdb-py
 Description-Content-Type: text/markdown
 
 # esdb-py
 
 [![PyPI version](https://badge.fury.io/py/esdb.svg)](https://pypi.org/project/esdb/)
 [![codecov](https://codecov.io/gh/andriykohut/esdb-py/branch/main/graph/badge.svg?token=YVDPTDBPFB)](https://codecov.io/gh/andriykohut/esdb-py)
```

