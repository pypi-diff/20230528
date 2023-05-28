# Comparing `tmp/yellowbox-0.8.2.tar.gz` & `tmp/yellowbox-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox-0.8.2.tar", max compression
+gzip compressed data, was "yellowbox-0.8.3.tar", max compression
```

## Comparing `yellowbox-0.8.2.tar` & `yellowbox-0.8.3.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1081 2023-02-21 11:14:23.280330 yellowbox-0.8.2/LICENSE
--rw-r--r--   0        0        0     1265 2023-02-21 11:14:23.280330 yellowbox-0.8.2/README.md
--rw-r--r--   0        0        0     2586 2023-02-21 11:14:23.284330 yellowbox-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      691 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/__init__.py
--rw-r--r--   0        0        0      236 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/_pytest.py
--rw-r--r--   0        0        0       22 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/_version.py
--rw-r--r--   0        0        0      550 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/clients.py
--rw-r--r--   0        0        0    10220 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/containers.py
--rw-r--r--   0        0        0        0 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/__init__.py
--rw-r--r--   0        0        0     2247 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/aerospike.py
--rw-r--r--   0        0        0     4643 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/azure_storage.py
--rw-r--r--   0        0        0     5998 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/fake_gcs.py
--rw-r--r--   0        0        0    10058 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/http_server.py
--rw-r--r--   0        0        0     4792 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/kafka.py
--rw-r--r--   0        0        0    10361 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/logstash.py
--rw-r--r--   0        0        0     2262 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/mssql.py
--rw-r--r--   0        0        0     3598 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/postgresql.py
--rw-r--r--   0        0        0     4426 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/rabbit_mq.py
--rw-r--r--   0        0        0     3255 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/redis.py
--rw-r--r--   0        0        0     7631 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/sql_base.py
--rw-r--r--   0        0        0     5535 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/vault.py
--rw-r--r--   0        0        0      784 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/webserver/__init__.py
--rw-r--r--   0        0        0     4010 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/webserver/class_endpoint.py
--rw-r--r--   0        0        0    13779 2023-02-21 11:14:23.284330 yellowbox-0.8.2/yellowbox/extras/webserver/endpoints.py
--rw-r--r--   0        0        0    15962 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/webserver/http_request_capture.py
--rw-r--r--   0        0        0     7876 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/webserver/request_capture.py
--rw-r--r--   0        0        0     3857 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/webserver/util.py
--rw-r--r--   0        0        0    12332 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/webserver/webserver.py
--rw-r--r--   0        0        0    20155 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/webserver/ws_request_capture.py
--rw-r--r--   0        0        0    14333 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/extras/websocket.py
--rw-r--r--   0        0        0     3408 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/image_build.py
--rw-r--r--   0        0        0     3104 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/networks.py
--rw-r--r--   0        0        0        0 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/py.typed
--rw-r--r--   0        0        0     3564 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/retry.py
--rw-r--r--   0        0        0      578 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/service.py
--rw-r--r--   0        0        0     7164 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/subclasses.py
--rw-r--r--   0        0        0     2919 2023-02-21 11:14:23.288330 yellowbox-0.8.2/yellowbox/utils.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 yellowbox-0.8.2/setup.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-28 09:57:20.995778 yellowbox-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1265 2023-05-28 09:57:20.995778 yellowbox-0.8.3/README.md
+-rw-r--r--   0        0        0     2586 2023-05-28 09:57:20.999778 yellowbox-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      691 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/_pytest.py
+-rw-r--r--   0        0        0       22 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/_version.py
+-rw-r--r--   0        0        0      550 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/clients.py
+-rw-r--r--   0        0        0    10220 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/containers.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/__init__.py
+-rw-r--r--   0        0        0     2247 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/aerospike.py
+-rw-r--r--   0        0        0     4643 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/azure_storage.py
+-rw-r--r--   0        0        0     5998 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/fake_gcs.py
+-rw-r--r--   0        0        0    10058 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/http_server.py
+-rw-r--r--   0        0        0     4792 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/kafka.py
+-rw-r--r--   0        0        0    10361 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/logstash.py
+-rw-r--r--   0        0        0     2262 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/mssql.py
+-rw-r--r--   0        0        0     3598 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/postgresql.py
+-rw-r--r--   0        0        0     4426 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/rabbit_mq.py
+-rw-r--r--   0        0        0     3255 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/redis.py
+-rw-r--r--   0        0        0     7631 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/sql_base.py
+-rw-r--r--   0        0        0     5535 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/vault.py
+-rw-r--r--   0        0        0      784 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/__init__.py
+-rw-r--r--   0        0        0     4010 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/class_endpoint.py
+-rw-r--r--   0        0        0    13779 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/endpoints.py
+-rw-r--r--   0        0        0    15962 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/http_request_capture.py
+-rw-r--r--   0        0        0     7876 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/request_capture.py
+-rw-r--r--   0        0        0     3857 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/util.py
+-rw-r--r--   0        0        0    12332 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/webserver.py
+-rw-r--r--   0        0        0    20155 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/ws_request_capture.py
+-rw-r--r--   0        0        0    14333 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/websocket.py
+-rw-r--r--   0        0        0     3408 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/image_build.py
+-rw-r--r--   0        0        0     3104 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/networks.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/py.typed
+-rw-r--r--   0        0        0     3564 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/retry.py
+-rw-r--r--   0        0        0      578 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/service.py
+-rw-r--r--   0        0        0     7164 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/subclasses.py
+-rw-r--r--   0        0        0     1986 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/utils.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.3/PKG-INFO
```

### Comparing `yellowbox-0.8.2/LICENSE` & `yellowbox-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/README.md` & `yellowbox-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/pyproject.toml` & `yellowbox-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yellowbox"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = ["biocatch ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/biocatchltd/yellowbox"
 
 [tool.poetry.dependencies]
```

### Comparing `yellowbox-0.8.2/yellowbox/__init__.py` & `yellowbox-0.8.3/yellowbox/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/clients.py` & `yellowbox-0.8.3/yellowbox/clients.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/containers.py` & `yellowbox-0.8.3/yellowbox/containers.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/aerospike.py` & `yellowbox-0.8.3/yellowbox/extras/aerospike.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/azure_storage.py` & `yellowbox-0.8.3/yellowbox/extras/azure_storage.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/fake_gcs.py` & `yellowbox-0.8.3/yellowbox/extras/fake_gcs.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/http_server.py` & `yellowbox-0.8.3/yellowbox/extras/http_server.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/kafka.py` & `yellowbox-0.8.3/yellowbox/extras/kafka.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/logstash.py` & `yellowbox-0.8.3/yellowbox/extras/logstash.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/mssql.py` & `yellowbox-0.8.3/yellowbox/extras/mssql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/postgresql.py` & `yellowbox-0.8.3/yellowbox/extras/postgresql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/rabbit_mq.py` & `yellowbox-0.8.3/yellowbox/extras/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/redis.py` & `yellowbox-0.8.3/yellowbox/extras/redis.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/sql_base.py` & `yellowbox-0.8.3/yellowbox/extras/sql_base.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/vault.py` & `yellowbox-0.8.3/yellowbox/extras/vault.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/__init__.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/class_endpoint.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/class_endpoint.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/endpoints.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/endpoints.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/http_request_capture.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/http_request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/request_capture.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/util.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/util.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/webserver.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/webserver.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/webserver/ws_request_capture.py` & `yellowbox-0.8.3/yellowbox/extras/webserver/ws_request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/extras/websocket.py` & `yellowbox-0.8.3/yellowbox/extras/websocket.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/image_build.py` & `yellowbox-0.8.3/yellowbox/image_build.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/networks.py` & `yellowbox-0.8.3/yellowbox/networks.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/retry.py` & `yellowbox-0.8.3/yellowbox/retry.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/service.py` & `yellowbox-0.8.3/yellowbox/service.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/subclasses.py` & `yellowbox-0.8.3/yellowbox/subclasses.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.2/yellowbox/utils.py` & `yellowbox-0.8.3/yellowbox/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import platform
-import sys
 from contextlib import AbstractContextManager, closing, contextmanager, nullcontext
 from socket import AF_INET, SO_REUSEADDR, SOCK_STREAM, SOL_SOCKET, socket
 from typing import Callable, Optional, TypeVar
 
 from yaspin import yaspin
 
 _T = TypeVar('_T')
@@ -46,48 +45,28 @@
 # if we expose a port in docker, this is where we expect to find it hosted
 # this is almost always just localhost
 # you can set the value here to some value with the YELLOWBOX_DOCKER_EXPOSE_HOST env-var
 # DO NOT manually change this const, instead call update_docker_expose_host
 DOCKER_EXPOSE_HOST = ""
 
 
-def update_docker_expose_host(value: Optional[str], print_file):
+def update_docker_expose_host(value: Optional[str]):
     """
     update the global docker expose host, attempting to infer from the environment
 
     Args:
         value: if provided, will use this value instead of inferring a host
-        print_file: the stream to print messages to on inference
 
     Notes:
         This function is called once when yellowbox is imported with a value of the env var
         YELLOWBOX_DOCKER_EXPOSE_HOST
 
     """
     global DOCKER_EXPOSE_HOST
 
-    def _helper():
-        if value is not None:
-            return value
-
-        if ('microsoft' in uname) and ('wsl2' in uname):
-            # wsl2 exposes ports on the microsoft machine, so we need to target it instead
-            with open('/etc/resolv.conf') as resolv:
-                for line in resolv:
-                    if line.startswith("nameserver "):
-                        ret = line[len("nameserver "):].strip()
-                        print(
-                            f"resolved DOCKER_EXPOSE_HOST to be {ret}",
-                            file=print_file,
-                        )
-                        return ret
-                else:
-                    print(
-                        "could not resolve DOCKER_EXPOSE_HOST from resolution file, using default",
-                        file=print_file,
-                    )
-        return "127.0.0.1"
+    if value is None:
+        value = "127.0.0.1"
 
-    DOCKER_EXPOSE_HOST = _helper()
+    DOCKER_EXPOSE_HOST = value
 
 
-update_docker_expose_host(os.getenv("YELLOWBOX_DOCKER_EXPOSE_HOST"), sys.stderr)
+update_docker_expose_host(os.getenv("YELLOWBOX_DOCKER_EXPOSE_HOST"))
```

### Comparing `yellowbox-0.8.2/PKG-INFO` & `yellowbox-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowbox
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 Home-page: https://github.com/biocatchltd/yellowbox
 License: MIT
 Author: biocatch ltd
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

