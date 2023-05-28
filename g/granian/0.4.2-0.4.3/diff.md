# Comparing `tmp/granian-0.4.2.tar.gz` & `tmp/granian-0.4.3.tar.gz`

## Comparing `granian-0.4.2.tar` & `granian-0.4.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.2/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-05-16 12:04:16.000000 granian-0.4.2/LICENSE
--rw-r--r--   0     1001      123     4024 2023-05-16 12:04:16.000000 granian-0.4.2/README.md
--rw-r--r--   0     1001      123       54 2023-05-16 12:04:16.000000 granian-0.4.2/build.rs
--rw-r--r--   0     1001      123       28 2023-05-16 12:04:16.000000 granian-0.4.2/granian/__init__.py
--rw-r--r--   0     1001      123       22 2023-05-16 12:04:16.000000 granian-0.4.2/granian/__version__.py
--rw-r--r--   0     1001      123     1868 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_granian.pyi
--rw-r--r--   0     1001      123     1677 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_internal.py
--rw-r--r--   0     1001      123     2862 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_loops.py
--rw-r--r--   0     1001      123       93 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_types.py
--rw-r--r--   0     1001      123     4682 2023-05-16 12:04:16.000000 granian-0.4.2/granian/asgi.py
--rw-r--r--   0     1001      123     3590 2023-05-16 12:04:16.000000 granian-0.4.2/granian/cli.py
--rw-r--r--   0     1001      123      357 2023-05-16 12:04:16.000000 granian-0.4.2/granian/constants.py
--rw-r--r--   0     1001      123     1328 2023-05-16 12:04:16.000000 granian-0.4.2/granian/log.py
--rw-r--r--   0     1001      123      153 2023-05-16 12:04:16.000000 granian-0.4.2/granian/net.py
--rw-r--r--   0     1001      123        0 2023-05-16 12:04:16.000000 granian-0.4.2/granian/py.typed
--rw-r--r--   0     1001      123      462 2023-05-16 12:04:16.000000 granian-0.4.2/granian/rsgi.py
--rw-r--r--   0     1001      123    10646 2023-05-16 12:04:16.000000 granian-0.4.2/granian/server.py
--rw-r--r--   0     1001      123     2068 2023-05-16 12:04:16.000000 granian-0.4.2/granian/wsgi.py
--rw-r--r--   0     1001      123     1624 2023-05-16 12:04:16.000000 granian-0.4.2/pyproject.toml
--rw-r--r--   0     1001      123     6984 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/callbacks.rs
--rw-r--r--   0     1001      123     1611 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/errors.rs
--rw-r--r--   0     1001      123     4765 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/http.rs
--rw-r--r--   0     1001      123    15092 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/io.rs
--rw-r--r--   0     1001      123      329 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/serve.rs
--rw-r--r--   0     1001      123     2708 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/types.rs
--rw-r--r--   0     1001      123     9591 2023-05-16 12:04:16.000000 granian-0.4.2/src/callbacks.rs
--rw-r--r--   0     1001      123      415 2023-05-16 12:04:16.000000 granian-0.4.2/src/http.rs
--rw-r--r--   0     1001      123      550 2023-05-16 12:04:16.000000 granian-0.4.2/src/lib.rs
--rw-r--r--   0     1001      123     6256 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      123      565 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/errors.rs
--rw-r--r--   0     1001      123     5186 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/http.rs
--rw-r--r--   0     1001      123    10350 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/io.rs
--rw-r--r--   0     1001      123      609 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/serve.rs
--rw-r--r--   0     1001      123     5619 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/types.rs
--rw-r--r--   0     1001      123     8066 2023-05-16 12:04:16.000000 granian-0.4.2/src/runtime.rs
--rw-r--r--   0     1001      123     4301 2023-05-16 12:04:16.000000 granian-0.4.2/src/tcp.rs
--rw-r--r--   0     1001      123     2431 2023-05-16 12:04:16.000000 granian-0.4.2/src/tls.rs
--rw-r--r--   0     1001      123      837 2023-05-16 12:04:16.000000 granian-0.4.2/src/utils.rs
--rw-r--r--   0     1001      123    16456 2023-05-16 12:04:16.000000 granian-0.4.2/src/workers.rs
--rw-r--r--   0     1001      123     3435 2023-05-16 12:04:16.000000 granian-0.4.2/src/ws.rs
--rw-r--r--   0     1001      123     1027 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      123      308 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/errors.rs
--rw-r--r--   0     1001      123     1638 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/http.rs
--rw-r--r--   0     1001      123      312 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/mod.rs
--rw-r--r--   0     1001      123     2206 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/serve.rs
--rw-r--r--   0     1001      123     4151 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/types.rs
--rw-r--r--   0     1001      123     3078 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/asgi.py
--rw-r--r--   0     1001      123     2490 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/rsgi.py
--rw-r--r--   0     1001      123      861 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/wsgi.py
--rw-r--r--   0     1001      123     1759 2023-05-16 12:04:16.000000 granian-0.4.2/tests/conftest.py
--rw-r--r--   0     1001      123     1139 2023-05-16 12:04:16.000000 granian-0.4.2/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      123     1704 2023-05-16 12:04:16.000000 granian-0.4.2/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      123     1830 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_asgi.py
--rw-r--r--   0     1001      123     1851 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_https.py
--rw-r--r--   0     1001      123     1450 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_rsgi.py
--rw-r--r--   0     1001      123     2487 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_ws.py
--rw-r--r--   0     1001      123     1438 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_wsgi.py
--rw-r--r--   0     1001      123    33385 2023-05-16 12:04:16.000000 granian-0.4.2/Cargo.lock
--rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      123     1486 2023-05-28 13:22:53.000000 granian-0.4.3/LICENSE
+-rw-r--r--   0     1001      123     4024 2023-05-28 13:22:53.000000 granian-0.4.3/README.md
+-rw-r--r--   0     1001      123       54 2023-05-28 13:22:53.000000 granian-0.4.3/build.rs
+-rw-r--r--   0     1001      123       28 2023-05-28 13:22:53.000000 granian-0.4.3/granian/__init__.py
+-rw-r--r--   0     1001      123       22 2023-05-28 13:22:53.000000 granian-0.4.3/granian/__version__.py
+-rw-r--r--   0     1001      123      261 2023-05-28 13:22:53.000000 granian-0.4.3/granian/_futures.py
+-rw-r--r--   0     1001      123     1868 2023-05-28 13:22:53.000000 granian-0.4.3/granian/_granian.pyi
+-rw-r--r--   0     1001      123     1677 2023-05-28 13:22:53.000000 granian-0.4.3/granian/_internal.py
+-rw-r--r--   0     1001      123     2862 2023-05-28 13:22:53.000000 granian-0.4.3/granian/_loops.py
+-rw-r--r--   0     1001      123       93 2023-05-28 13:22:53.000000 granian-0.4.3/granian/_types.py
+-rw-r--r--   0     1001      123     4682 2023-05-28 13:22:53.000000 granian-0.4.3/granian/asgi.py
+-rw-r--r--   0     1001      123     3772 2023-05-28 13:22:53.000000 granian-0.4.3/granian/cli.py
+-rw-r--r--   0     1001      123      357 2023-05-28 13:22:53.000000 granian-0.4.3/granian/constants.py
+-rw-r--r--   0     1001      123     1328 2023-05-28 13:22:53.000000 granian-0.4.3/granian/log.py
+-rw-r--r--   0     1001      123      153 2023-05-28 13:22:53.000000 granian-0.4.3/granian/net.py
+-rw-r--r--   0     1001      123        0 2023-05-28 13:22:53.000000 granian-0.4.3/granian/py.typed
+-rw-r--r--   0     1001      123      462 2023-05-28 13:22:53.000000 granian-0.4.3/granian/rsgi.py
+-rw-r--r--   0     1001      123    10976 2023-05-28 13:22:53.000000 granian-0.4.3/granian/server.py
+-rw-r--r--   0     1001      123     2068 2023-05-28 13:22:53.000000 granian-0.4.3/granian/wsgi.py
+-rw-r--r--   0     1001      123     1624 2023-05-28 13:22:53.000000 granian-0.4.3/pyproject.toml
+-rw-r--r--   0     1001      123    11007 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      123     1611 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/errors.rs
+-rw-r--r--   0     1001      123     5171 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/http.rs
+-rw-r--r--   0     1001      123    15092 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/io.rs
+-rw-r--r--   0     1001      123      329 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/mod.rs
+-rw-r--r--   0     1001      123     4636 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/serve.rs
+-rw-r--r--   0     1001      123     2708 2023-05-28 13:22:53.000000 granian-0.4.3/src/asgi/types.rs
+-rw-r--r--   0     1001      123    10305 2023-05-28 13:22:53.000000 granian-0.4.3/src/callbacks.rs
+-rw-r--r--   0     1001      123      415 2023-05-28 13:22:53.000000 granian-0.4.3/src/http.rs
+-rw-r--r--   0     1001      123      550 2023-05-28 13:22:53.000000 granian-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      123     6256 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      123      565 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/errors.rs
+-rw-r--r--   0     1001      123     5186 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/http.rs
+-rw-r--r--   0     1001      123    10350 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/io.rs
+-rw-r--r--   0     1001      123      609 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/mod.rs
+-rw-r--r--   0     1001      123     3017 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/serve.rs
+-rw-r--r--   0     1001      123     5619 2023-05-28 13:22:53.000000 granian-0.4.3/src/rsgi/types.rs
+-rw-r--r--   0     1001      123     8066 2023-05-28 13:22:53.000000 granian-0.4.3/src/runtime.rs
+-rw-r--r--   0     1001      123     4301 2023-05-28 13:22:53.000000 granian-0.4.3/src/tcp.rs
+-rw-r--r--   0     1001      123     2431 2023-05-28 13:22:53.000000 granian-0.4.3/src/tls.rs
+-rw-r--r--   0     1001      123      837 2023-05-28 13:22:53.000000 granian-0.4.3/src/utils.rs
+-rw-r--r--   0     1001      123    16535 2023-05-28 13:22:53.000000 granian-0.4.3/src/workers.rs
+-rw-r--r--   0     1001      123     3435 2023-05-28 13:22:53.000000 granian-0.4.3/src/ws.rs
+-rw-r--r--   0     1001      123     1027 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      123      308 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/errors.rs
+-rw-r--r--   0     1001      123     1638 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/http.rs
+-rw-r--r--   0     1001      123      312 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/mod.rs
+-rw-r--r--   0     1001      123     2228 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/serve.rs
+-rw-r--r--   0     1001      123     4151 2023-05-28 13:22:53.000000 granian-0.4.3/src/wsgi/types.rs
+-rw-r--r--   0     1001      123     3078 2023-05-28 13:22:53.000000 granian-0.4.3/tests/apps/asgi.py
+-rw-r--r--   0     1001      123     2490 2023-05-28 13:22:53.000000 granian-0.4.3/tests/apps/rsgi.py
+-rw-r--r--   0     1001      123      861 2023-05-28 13:22:53.000000 granian-0.4.3/tests/apps/wsgi.py
+-rw-r--r--   0     1001      123     1759 2023-05-28 13:22:53.000000 granian-0.4.3/tests/conftest.py
+-rw-r--r--   0     1001      123     1139 2023-05-28 13:22:53.000000 granian-0.4.3/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      123     1704 2023-05-28 13:22:53.000000 granian-0.4.3/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      123     1830 2023-05-28 13:22:53.000000 granian-0.4.3/tests/test_asgi.py
+-rw-r--r--   0     1001      123     1851 2023-05-28 13:22:53.000000 granian-0.4.3/tests/test_https.py
+-rw-r--r--   0     1001      123     1450 2023-05-28 13:22:53.000000 granian-0.4.3/tests/test_rsgi.py
+-rw-r--r--   0     1001      123     2487 2023-05-28 13:22:53.000000 granian-0.4.3/tests/test_ws.py
+-rw-r--r--   0     1001      123     1438 2023-05-28 13:22:53.000000 granian-0.4.3/tests/test_wsgi.py
+-rw-r--r--   0     1001      123    33385 2023-05-28 13:22:53.000000 granian-0.4.3/Cargo.lock
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.3/PKG-INFO
```

### Comparing `granian-0.4.2/Cargo.toml` & `granian-0.4.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
```

### Comparing `granian-0.4.2/LICENSE` & `granian-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/README.md` & `granian-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/_granian.pyi` & `granian-0.4.3/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/_internal.py` & `granian-0.4.3/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/_loops.py` & `granian-0.4.3/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/asgi.py` & `granian-0.4.3/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/cli.py` & `granian-0.4.3/granian/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     workers: int = typer.Option(1, min=1, help="Number of worker processes."),
     threads: int = typer.Option(1, min=1, help="Number of threads."),
     threading_mode: ThreadModes = typer.Option(
         ThreadModes.workers.value,
         help="Threading mode to use."
     ),
     loop: Loops = typer.Option(Loops.auto.value, help="Event loop implementation"),
+    loop_opt: bool = typer.Option(
+        True,
+        "--opt/--no-opt",
+        help="Enable loop optimizations",
+        show_default="enabled"
+    ),
     backlog: int = typer.Option(
         1024,
         min=128,
         help="Maximum number of connections to hold in backlog."
     ),
     log_level: LogLevels = typer.Option(
         LogLevels.info.value,
@@ -112,14 +118,15 @@
         port=port,
         interface=interface,
         workers=workers,
         threads=threads,
         pthreads=threads,
         threading_mode=threading_mode,
         loop=loop,
+        loop_opt=loop_opt,
         http=http,
         websockets=websockets,
         backlog=backlog,
         log_level=log_level,
         log_dictconfig=log_dictconfig,
         ssl_cert=ssl_certificate,
         ssl_key=ssl_keyfile,
```

### Comparing `granian-0.4.2/granian/log.py` & `granian-0.4.3/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/granian/server.py` & `granian-0.4.3/granian/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional
 
 import watchfiles
 
+from ._futures import future_watcher_wrapper
 from ._granian import ASGIWorker, RSGIWorker, WSGIWorker
 from ._internal import load_target
 from .asgi import LifespanProtocol, _callback_wrapper as _asgi_call_wrap
 from .constants import Interfaces, HTTPModes, Loops, ThreadModes
 from .log import LogLevels, configure_logging, logger
 from .net import SocketHolder
 from .wsgi import _callback_wrapper as _wsgi_call_wrap
@@ -32,14 +33,15 @@
         port: int = 8000,
         interface: Interfaces = Interfaces.RSGI,
         workers: int = 1,
         threads: int = 1,
         pthreads: int = 1,
         threading_mode: ThreadModes = ThreadModes.workers,
         loop: Loops = Loops.auto,
+        loop_opt: bool = True,
         http: HTTPModes = HTTPModes.auto,
         websockets: bool = True,
         backlog: int = 1024,
         http1_buffer_size: int = 65535,
         log_level: LogLevels = LogLevels.info,
         log_dictconfig: Optional[Dict[str, Any]] = None,
         ssl_cert: Optional[Path] = None,
@@ -52,14 +54,15 @@
         self.bind_port = port
         self.interface = interface
         self.workers = max(1, workers)
         self.threads = max(1, threads)
         self.pthreads = max(1, pthreads)
         self.threading_mode = threading_mode
         self.loop = loop
+        self.loop_opt = loop_opt
         self.http = http
         self.websockets = websockets
         self.backlog = max(128, backlog)
         self.http1_buffer_size = http1_buffer_size
         self.log_level = log_level
         self.log_config = log_dictconfig
         self.url_path_prefix = url_path_prefix
@@ -96,14 +99,15 @@
         loop_impl,
         threads,
         pthreads,
         threading_mode,
         http_mode,
         http1_buffer_size,
         websockets,
+        loop_opt,
         log_level,
         log_config,
         ssl_ctx,
         scope_opts
     ):
         from granian._loops import loops, set_loop_signals
 
@@ -115,30 +119,35 @@
 
         loop.run_until_complete(lifespan_handler.startup())
         if lifespan_handler.interrupt:
             return
 
         shutdown_event = set_loop_signals(loop, [signal.SIGTERM, signal.SIGINT])
 
+        wcallback = _asgi_call_wrap(callback, scope_opts)
+        if not loop_opt:
+            wcallback = future_watcher_wrapper(wcallback)
+
         worker = ASGIWorker(
             worker_id,
             sfd,
             threads,
             pthreads,
             http_mode,
             http1_buffer_size,
             websockets,
+            loop_opt,
             *ssl_ctx
         )
         serve = getattr(worker, {
             ThreadModes.runtime: "serve_rth",
             ThreadModes.workers: "serve_wth"
         }[threading_mode])
         serve(
-            _asgi_call_wrap(callback, scope_opts),
+            wcallback,
             loop,
             contextvars.copy_context(),
             shutdown_event.wait()
         )
         loop.run_until_complete(lifespan_handler.shutdown())
 
 
@@ -150,14 +159,15 @@
         loop_impl,
         threads,
         pthreads,
         threading_mode,
         http_mode,
         http1_buffer_size,
         websockets,
+        loop_opt,
         log_level,
         log_config,
         ssl_ctx,
         scope_opts
     ):
         from granian._loops import loops, set_loop_signals
 
@@ -206,14 +216,15 @@
         loop_impl,
         threads,
         pthreads,
         threading_mode,
         http_mode,
         http1_buffer_size,
         websockets,
+        loop_opt,
         log_level,
         log_config,
         ssl_ctx,
         scope_opts
     ):
         from granian._loops import loops, set_loop_signals
 
@@ -272,14 +283,15 @@
                 self.loop,
                 self.threads,
                 self.pthreads,
                 self.threading_mode,
                 self.http,
                 self.http1_buffer_size,
                 self.websockets,
+                self.loop_opt,
                 self.log_level,
                 self.log_config,
                 self.ssl_ctx,
                 {
                     "url_path_prefix": self.url_path_prefix
                 }
             )
```

### Comparing `granian-0.4.2/granian/wsgi.py` & `granian-0.4.3/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/pyproject.toml` & `granian-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/asgi/callbacks.rs` & `granian-0.4.3/src/rsgi/callbacks.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use hyper::{Body, Request, Response};
 use pyo3::prelude::*;
 use pyo3_asyncio::TaskLocals;
 use tokio::sync::oneshot;
 
 use crate::{
     callbacks::{
         CallbackWrapper,
@@ -12,16 +11,16 @@
         callback_impl_loop_wake,
         callback_impl_loop_err
     },
     runtime::RuntimeRef,
     ws::{HyperWebsocket, UpgradeData}
 };
 use super::{
-    io::{ASGIHTTPProtocol as HTTPProtocol, ASGIWebsocketProtocol as WebsocketProtocol},
-    types::ASGIScope as Scope
+    io::{RSGIHTTPProtocol as HTTPProtocol, RSGIWebsocketProtocol as WebsocketProtocol},
+    types::{RSGIScope as Scope, PyResponse, PyResponseBytes}
 };
 
 
 #[pyclass]
 pub(crate) struct CallbackRunnerHTTP {
     proto: Py<HTTPProtocol>,
     context: TaskLocals,
@@ -65,23 +64,23 @@
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<HTTPProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
         let pyctx = context.context(py);
-        Ok(Self { proto, context, pycontext: pyctx.call_method0("copy")?.into(), cb })
+        Ok(Self { proto, context, pycontext: pyctx.call_method0(pyo3::intern!(py, "copy"))?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
-                let mut res = Response::new("Internal server error".into());
-                *res.status_mut() = hyper::StatusCode::INTERNAL_SERVER_ERROR;
-                let _ = tx.send(res);
+                let _ = tx.send(
+                    PyResponse::Bytes(PyResponseBytes::empty(500, Vec::new()))
+                );
             }
         }
     }
 
     fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
@@ -146,15 +145,15 @@
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<WebsocketProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
         let pyctx = context.context(py);
-        Ok(Self { proto, context, pycontext: pyctx.call_method0("copy")?.into(), cb })
+        Ok(Self { proto, context, pycontext: pyctx.call_method0(pyo3::intern!(py, "copy"))?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
@@ -177,61 +176,38 @@
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
 
-// NOTE: we cannot use single `impl` function as structs with pyclass won't handle
-//       dyn fields easily.
-// pub(crate) async fn call(
-//     cb: CallbackWrapper,
-//     protocol: impl ASGIProtocol + IntoPy<PyObject>,
-//     scope: Scope
-// ) -> Result<(), ASGIFlowError> {
-//     let (tx, rx) = oneshot::channel();
-//     let callback = cb.callback.clone();
-//     Python::with_gil(|py| {
-//         callback.call1(py, (CallbackWatcher::new(py, cb, tx), scope, protocol))
-//     })?;
-
-//     match rx.await {
-//         Ok(true) => Ok(()),
-//         Ok(false) => {
-//             log::warn!("Application callable raised an exception");
-//             error_flow!()
-//         },
-//         _ => error_flow!()
-//     }
-// }
-
 pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: Request<Body>,
+    req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> oneshot::Receiver<Response<Body>> {
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, tx, req);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
     });
 
     rx
 }
 
 pub(crate) fn call_rtt_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: Request<Body>,
+    req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> oneshot::Receiver<Response<Body>> {
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, tx, req);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
         });
     });
 
@@ -240,15 +216,15 @@
 
 pub(crate) fn call_rtb_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<bool> {
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
     });
 
@@ -257,15 +233,15 @@
 
 pub(crate) fn call_rtt_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<bool> {
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
         });
```

### Comparing `granian-0.4.2/src/asgi/errors.rs` & `granian-0.4.3/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/asgi/http.rs` & `granian-0.4.3/src/asgi/http.rs`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,24 @@
 use crate::{
     callbacks::CallbackWrapper,
     http::{HV_SERVER, response_500},
     runtime::RuntimeRef,
     ws::{UpgradeData, is_upgrade_request as is_ws_upgrade, upgrade_intent as ws_upgrade}
 };
 use super::{
-    callbacks::{call_rtb_http, call_rtb_ws, call_rtt_http, call_rtt_ws},
+    callbacks::{
+        call_rtb_http,
+        call_rtb_http_pyw,
+        call_rtb_ws,
+        call_rtb_ws_pyw,
+        call_rtt_http,
+        call_rtt_http_pyw,
+        call_rtt_ws,
+        call_rtt_ws_pyw
+    },
     types::ASGIScope as Scope
 };
 
 
 macro_rules! default_scope {
     ($server_addr:expr, $client_addr:expr, $req:expr, $scheme:expr) => {
         Scope::new(
@@ -132,9 +141,13 @@
             handle_http_response!($handler_req, rt, callback, req, scope)
         }
     };
 }
 
 handle_request!(handle_rtt, call_rtt_http);
 handle_request!(handle_rtb, call_rtb_http);
+handle_request!(handle_rtt_pyw, call_rtt_http_pyw);
+handle_request!(handle_rtb_pyw, call_rtb_http_pyw);
 handle_request_with_ws!(handle_rtt_ws, call_rtt_http, call_rtt_ws);
 handle_request_with_ws!(handle_rtb_ws, call_rtb_http, call_rtb_ws);
+handle_request_with_ws!(handle_rtt_ws_pyw, call_rtt_http_pyw, call_rtt_ws_pyw);
+handle_request_with_ws!(handle_rtb_ws_pyw, call_rtb_http_pyw, call_rtb_ws_pyw);
```

### Comparing `granian-0.4.2/src/asgi/io.rs` & `granian-0.4.3/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/asgi/serve.rs` & `granian-0.4.3/src/rsgi/serve.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,31 @@
         serve_rth_ssl,
         serve_wth_ssl
     }
 };
 use super::http::{handle_rtb, handle_rtt, handle_rtb_ws, handle_rtt_ws};
 
 #[pyclass(module="granian._granian")]
-pub struct ASGIWorker {
+pub struct RSGIWorker {
     config: WorkerConfig
 }
 
-impl ASGIWorker {
+impl RSGIWorker {
     serve_rth!(_serve_rth, handle_rtb);
     serve_rth!(_serve_rth_ws, handle_rtb_ws);
     serve_wth!(_serve_wth, handle_rtt);
     serve_wth!(_serve_wth_ws, handle_rtt_ws);
     serve_rth_ssl!(_serve_rth_ssl, handle_rtb);
     serve_rth_ssl!(_serve_rth_ssl_ws, handle_rtb_ws);
     serve_wth_ssl!(_serve_wth_ssl, handle_rtt);
     serve_wth_ssl!(_serve_wth_ssl_ws, handle_rtt_ws);
 }
 
 #[pymethods]
-impl ASGIWorker {
+impl RSGIWorker {
     #[new]
     #[pyo3(
         signature = (
             worker_id,
             socket_fd,
             threads=1,
             pthreads=1,
@@ -61,14 +61,15 @@
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
                 http_mode,
                 http1_buffer_max,
                 websockets_enabled,
+                true,
                 ssl_enabled,
                 ssl_cert,
                 ssl_key
             )
         })
     }
```

### Comparing `granian-0.4.2/src/asgi/types.rs` & `granian-0.4.3/src/asgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/callbacks.rs` & `granian-0.4.3/src/callbacks.rs`

 * *Files 3% similar despite different names*

```diff
@@ -220,14 +220,34 @@
                 (target,),
                 Some(kwctx)
             )
         }
     };
 }
 
+macro_rules! callback_impl_run_pytask {
+    () => {
+        pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
+            let event_loop = self.context.event_loop(py);
+            let context = self.context.context(py);
+            let target = self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_task"))?;
+            let kwctx = pyo3::types::PyDict::new(py);
+            kwctx.set_item(
+                pyo3::intern!(py, "context"),
+                context
+            )?;
+            event_loop.call_method(
+                pyo3::intern!(py, "call_soon_threadsafe"),
+                (target,),
+                Some(kwctx)
+            )
+        }
+    };
+}
+
 macro_rules! callback_impl_loop_run {
     () => {
         pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
             let context = self.pycontext.clone().into_ref(py);
             context.call_method1(
                 pyo3::intern!(py, "run"),
                 (self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_step"))?,)
@@ -318,11 +338,12 @@
             self.err(py);
             cberr
         }
     };
 }
 
 pub(crate) use callback_impl_run;
+pub(crate) use callback_impl_run_pytask;
 pub(crate) use callback_impl_loop_run;
 pub(crate) use callback_impl_loop_step;
 pub(crate) use callback_impl_loop_wake;
 pub(crate) use callback_impl_loop_err;
```

### Comparing `granian-0.4.2/src/lib.rs` & `granian-0.4.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/rsgi/errors.rs` & `granian-0.4.3/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/rsgi/http.rs` & `granian-0.4.3/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/rsgi/io.rs` & `granian-0.4.3/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/rsgi/mod.rs` & `granian-0.4.3/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/rsgi/serve.rs` & `granian-0.4.3/src/asgi/serve.rs`

 * *Files 24% similar despite different names*

```diff
@@ -5,100 +5,137 @@
         WorkerConfig,
         serve_rth,
         serve_wth,
         serve_rth_ssl,
         serve_wth_ssl
     }
 };
-use super::http::{handle_rtb, handle_rtt, handle_rtb_ws, handle_rtt_ws};
+use super::http::{
+    handle_rtb,
+    handle_rtb_pyw,
+    handle_rtt,
+    handle_rtt_pyw,
+    handle_rtb_ws,
+    handle_rtb_ws_pyw,
+    handle_rtt_ws,
+    handle_rtt_ws_pyw
+};
+
 
 #[pyclass(module="granian._granian")]
-pub struct RSGIWorker {
+pub struct ASGIWorker {
     config: WorkerConfig
 }
 
-impl RSGIWorker {
+impl ASGIWorker {
     serve_rth!(_serve_rth, handle_rtb);
+    serve_rth!(_serve_rth_pyw, handle_rtb_pyw);
     serve_rth!(_serve_rth_ws, handle_rtb_ws);
+    serve_rth!(_serve_rth_ws_pyw, handle_rtb_ws_pyw);
     serve_wth!(_serve_wth, handle_rtt);
+    serve_wth!(_serve_wth_pyw, handle_rtt_pyw);
     serve_wth!(_serve_wth_ws, handle_rtt_ws);
+    serve_wth!(_serve_wth_ws_pyw, handle_rtt_ws_pyw);
     serve_rth_ssl!(_serve_rth_ssl, handle_rtb);
+    serve_rth_ssl!(_serve_rth_ssl_pyw, handle_rtb_pyw);
     serve_rth_ssl!(_serve_rth_ssl_ws, handle_rtb_ws);
+    serve_rth_ssl!(_serve_rth_ssl_ws_pyw, handle_rtb_ws_pyw);
     serve_wth_ssl!(_serve_wth_ssl, handle_rtt);
+    serve_wth_ssl!(_serve_wth_ssl_pyw, handle_rtt_pyw);
     serve_wth_ssl!(_serve_wth_ssl_ws, handle_rtt_ws);
+    serve_wth_ssl!(_serve_wth_ssl_ws_pyw, handle_rtt_ws_pyw);
 }
 
 #[pymethods]
-impl RSGIWorker {
+impl ASGIWorker {
     #[new]
     #[pyo3(
         signature = (
             worker_id,
             socket_fd,
             threads=1,
             pthreads=1,
             http_mode="1",
             http1_buffer_max=65535,
             websockets_enabled=false,
+            opt_enabled=true,
             ssl_enabled=false,
             ssl_cert=None,
             ssl_key=None
         )
     )]
     fn new(
         worker_id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
         http_mode: &str,
         http1_buffer_max: usize,
         websockets_enabled: bool,
+        opt_enabled: bool,
         ssl_enabled: bool,
         ssl_cert: Option<&str>,
         ssl_key: Option<&str>
     ) -> PyResult<Self> {
         Ok(Self {
             config: WorkerConfig::new(
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
                 http_mode,
                 http1_buffer_max,
                 websockets_enabled,
+                opt_enabled,
                 ssl_enabled,
                 ssl_cert,
                 ssl_key
             )
         })
     }
 
     fn serve_rth(
         &self,
         callback: PyObject,
         event_loop: &PyAny,
         context: &PyAny,
         signal_rx: PyObject
     ) {
-        match (self.config.websockets_enabled, self.config.ssl_enabled) {
-            (false, false) => self._serve_rth(callback, event_loop, context, signal_rx),
-            (true, false) => self._serve_rth_ws(callback, event_loop, context, signal_rx),
-            (false, true) => self._serve_rth_ssl(callback, event_loop, context, signal_rx),
-            (true, true) => self._serve_rth_ssl_ws(callback, event_loop, context, signal_rx)
+        match (
+            self.config.websockets_enabled,
+            self.config.ssl_enabled,
+            self.config.opt_enabled
+        ) {
+            (false, false, true) => self._serve_rth(callback, event_loop, context, signal_rx),
+            (false, false, false) => self._serve_rth_pyw(callback, event_loop, context, signal_rx),
+            (true, false, true) => self._serve_rth_ws(callback, event_loop, context, signal_rx),
+            (true, false, false) => self._serve_rth_ws_pyw(callback, event_loop, context, signal_rx),
+            (false, true, true) => self._serve_rth_ssl(callback, event_loop, context, signal_rx),
+            (false, true, false) => self._serve_rth_ssl_pyw(callback, event_loop, context, signal_rx),
+            (true, true, true) => self._serve_rth_ssl_ws(callback, event_loop, context, signal_rx),
+            (true, true, false) => self._serve_rth_ssl_ws_pyw(callback, event_loop, context, signal_rx)
         }
     }
 
     fn serve_wth(
         &self,
         callback: PyObject,
         event_loop: &PyAny,
         context: &PyAny,
         signal_rx: PyObject
     ) {
-        match (self.config.websockets_enabled, self.config.ssl_enabled) {
-            (false, false) => self._serve_wth(callback, event_loop, context, signal_rx),
-            (true, false) => self._serve_wth_ws(callback, event_loop, context, signal_rx),
-            (false, true) => self._serve_wth_ssl(callback, event_loop, context, signal_rx),
-            (true, true) => self._serve_wth_ssl_ws(callback, event_loop, context, signal_rx)
+        match (
+            self.config.websockets_enabled,
+            self.config.ssl_enabled,
+            self.config.opt_enabled
+        ) {
+            (false, false, true) => self._serve_wth(callback, event_loop, context, signal_rx),
+            (false, false, false) => self._serve_wth_pyw(callback, event_loop, context, signal_rx),
+            (true, false, true) => self._serve_wth_ws(callback, event_loop, context, signal_rx),
+            (true, false, false) => self._serve_wth_ws_pyw(callback, event_loop, context, signal_rx),
+            (false, true, true) => self._serve_wth_ssl(callback, event_loop, context, signal_rx),
+            (false, true, false) => self._serve_wth_ssl_pyw(callback, event_loop, context, signal_rx),
+            (true, true, true) => self._serve_wth_ssl_ws(callback, event_loop, context, signal_rx),
+            (true, true, false) => self._serve_wth_ssl_ws_pyw(callback, event_loop, context, signal_rx)
         }
     }
 }
```

### Comparing `granian-0.4.2/src/rsgi/types.rs` & `granian-0.4.3/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/runtime.rs` & `granian-0.4.3/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/tcp.rs` & `granian-0.4.3/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/tls.rs` & `granian-0.4.3/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/utils.rs` & `granian-0.4.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/workers.rs` & `granian-0.4.3/src/workers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,40 +15,43 @@
     pub id: i32,
     socket_fd: i32,
     pub threads: usize,
     pub pthreads: usize,
     pub http_mode: String,
     pub http1_buffer_max: usize,
     pub websockets_enabled: bool,
+    pub opt_enabled: bool,
     pub ssl_enabled: bool,
     ssl_cert: Option<String>,
     ssl_key: Option<String>
 }
 
 impl WorkerConfig {
     pub fn new(
         id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
         http_mode: &str,
         http1_buffer_max: usize,
         websockets_enabled: bool,
+        opt_enabled: bool,
         ssl_enabled: bool,
         ssl_cert: Option<&str>,
         ssl_key: Option<&str>
     ) -> Self {
         Self {
             id,
             socket_fd,
             threads,
             pthreads,
             http_mode: http_mode.into(),
             http1_buffer_max,
             websockets_enabled,
+            opt_enabled,
             ssl_enabled,
             ssl_cert: ssl_cert.map_or(None, |v| Some(v.into())),
             ssl_key: ssl_key.map_or(None, |v| Some(v.into()))
         }
     }
 
     #[cfg(unix)]
```

### Comparing `granian-0.4.2/src/ws.rs` & `granian-0.4.3/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/wsgi/callbacks.rs` & `granian-0.4.3/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/wsgi/http.rs` & `granian-0.4.3/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/src/wsgi/serve.rs` & `granian-0.4.3/src/wsgi/serve.rs`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
                 http_mode,
                 http1_buffer_max,
                 false,
+                true,
                 ssl_enabled,
                 ssl_cert,
                 ssl_key
             )
         })
     }
```

### Comparing `granian-0.4.2/src/wsgi/types.rs` & `granian-0.4.3/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/apps/asgi.py` & `granian-0.4.3/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/apps/rsgi.py` & `granian-0.4.3/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/apps/wsgi.py` & `granian-0.4.3/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/conftest.py` & `granian-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/fixtures/tls/cert.pem` & `granian-0.4.3/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/fixtures/tls/key.pem` & `granian-0.4.3/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/test_asgi.py` & `granian-0.4.3/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/test_https.py` & `granian-0.4.3/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/test_rsgi.py` & `granian-0.4.3/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/test_ws.py` & `granian-0.4.3/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/tests/test_wsgi.py` & `granian-0.4.3/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.2/Cargo.lock` & `granian-0.4.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "granian"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "bytes",
  "futures",
  "hyper",
  "log",
  "mimalloc",
  "once_cell",
```

### Comparing `granian-0.4.2/PKG-INFO` & `granian-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granian
-Version: 0.4.2
+Version: 0.4.3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -31,16 +31,16 @@
 Home-Page: https://github.com/emmett-framework/granian
 Author: Giovanni Barillari <g@baro.dev>
 Author-email: Giovanni Barillari <g@baro.dev>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Funding, https://github.com/sponsors/gi0baro
-Project-URL: Homepage, https://github.com/emmett-framework/granian
 Project-URL: Source, https://github.com/emmett-framework/granian
+Project-URL: Homepage, https://github.com/emmett-framework/granian
 
 # Granian
 
 A Rust HTTP server for Python applications.
 
 ## Rationale
```

