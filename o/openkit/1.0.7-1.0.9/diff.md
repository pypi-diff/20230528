# Comparing `tmp/openkit-1.0.7.tar.gz` & `tmp/openkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openkit-1.0.7.tar", last modified: Fri Nov  4 02:32:03 2022, max compression
+gzip compressed data, was "openkit-1.0.9.tar", last modified: Wed Nov  9 00:04:32 2022, max compression
```

## Comparing `openkit-1.0.7.tar` & `openkit-1.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       75 2022-05-21 01:33:41.411652 openkit-1.0.7/.gitignore
--rw-r--r--   0        0        0     1099 2022-05-21 00:47:41.295158 openkit-1.0.7/LICENSE
--rw-r--r--   0        0        0     1039 2022-06-01 20:50:34.577833 openkit-1.0.7/README.md
--rw-r--r--   0        0        0      107 2022-11-04 02:30:51.041878 openkit-1.0.7/openkit/__init__.py
--rw-r--r--   0        0        0       29 2022-05-21 04:23:09.995309 openkit-1.0.7/openkit/api/__init__.py
--rw-r--r--   0        0        0     1297 2022-05-23 00:28:18.853495 openkit-1.0.7/openkit/api/action.py
--rw-r--r--   0        0        0      909 2022-05-23 18:06:05.885713 openkit-1.0.7/openkit/api/composite.py
--rw-r--r--   0        0        0      740 2022-05-21 04:35:30.011795 openkit-1.0.7/openkit/api/constants.py
--rw-r--r--   0        0        0     6579 2022-11-04 02:31:25.598404 openkit-1.0.7/openkit/api/openkit.py
--rw-r--r--   0        0        0      230 2022-05-22 23:48:35.700302 openkit-1.0.7/openkit/api/openkit_object.py
--rw-r--r--   0        0        0      288 2022-05-22 23:44:49.543514 openkit-1.0.7/openkit/api/root_action.py
--rw-r--r--   0        0        0     1027 2022-05-22 23:45:03.082355 openkit-1.0.7/openkit/api/session.py
--rw-r--r--   0        0        0      678 2022-05-23 00:04:57.322004 openkit-1.0.7/openkit/api/web_request_tracer.py
--rw-r--r--   0        0        0        0 2022-05-24 01:07:58.229033 openkit-1.0.7/openkit/core/__init__.py
--rw-r--r--   0        0        0     6024 2022-05-24 01:52:41.816862 openkit-1.0.7/openkit/core/beacon_sender.py
--rw-r--r--   0        0        0       78 2022-05-23 13:52:41.240176 openkit-1.0.7/openkit/core/caching/__init__.py
--rw-r--r--   0        0        0     7875 2022-05-23 17:57:45.990341 openkit-1.0.7/openkit/core/caching/beacon_cache.py
--rw-r--r--   0        0        0      523 2022-05-21 00:29:22.433836 openkit-1.0.7/openkit/core/caching/beacon_key.py
--rw-r--r--   0        0        0     4976 2022-05-24 01:52:13.921403 openkit-1.0.7/openkit/core/caching/evictor.py
--rw-r--r--   0        0        0      338 2022-05-21 01:01:05.469940 openkit-1.0.7/openkit/core/communication/__init__.py
--rw-r--r--   0        0        0      730 2022-05-21 03:10:49.360285 openkit-1.0.7/openkit/core/communication/beacon_abstract.py
--rw-r--r--   0        0        0     2067 2022-05-23 14:36:41.565746 openkit-1.0.7/openkit/core/communication/beacon_capture_off.py
--rw-r--r--   0        0        0     3867 2022-05-23 15:09:58.138503 openkit-1.0.7/openkit/core/communication/beacon_capture_on.py
--rw-r--r--   0        0        0     1562 2022-05-23 14:37:27.062548 openkit-1.0.7/openkit/core/communication/beacon_flush.py
--rw-r--r--   0        0        0     2506 2022-05-23 14:36:08.501632 openkit-1.0.7/openkit/core/communication/beacon_init.py
--rw-r--r--   0        0        0      505 2022-05-23 14:30:30.164039 openkit-1.0.7/openkit/core/communication/beacon_terminal.py
--rw-r--r--   0        0        0      479 2022-05-22 22:22:41.639259 openkit-1.0.7/openkit/core/communication/countdown_latch.py
--rw-r--r--   0        0        0      721 2022-05-21 01:08:02.309177 openkit-1.0.7/openkit/core/communication/state_utils.py
--rw-r--r--   0        0        0      110 2022-05-21 01:01:05.607403 openkit-1.0.7/openkit/core/configuration/__init__.py
--rw-r--r--   0        0        0     2380 2022-05-22 22:42:25.461143 openkit-1.0.7/openkit/core/configuration/beacon_configuration.py
--rw-r--r--   0        0        0      227 2022-05-21 15:42:21.711277 openkit-1.0.7/openkit/core/configuration/http_client_configuration.py
--rw-r--r--   0        0        0      623 2022-05-21 01:31:06.268859 openkit-1.0.7/openkit/core/configuration/openkit_configuration.py
--rw-r--r--   0        0        0     2304 2022-05-22 21:40:08.172030 openkit-1.0.7/openkit/core/configuration/privacy_configuration.py
--rw-r--r--   0        0        0     2953 2022-05-22 22:53:43.319768 openkit-1.0.7/openkit/core/configuration/server_configuration.py
--rw-r--r--   0        0        0        0 2022-05-24 01:05:13.937317 openkit-1.0.7/openkit/core/objects/__init__.py
--rw-r--r--   0        0        0     5111 2022-05-23 18:03:46.293977 openkit-1.0.7/openkit/core/objects/base_action.py
--rw-r--r--   0        0        0      296 2022-05-21 14:57:53.990929 openkit-1.0.7/openkit/core/objects/leaf_action.py
--rw-r--r--   0        0        0     1240 2022-05-23 00:28:18.847039 openkit-1.0.7/openkit/core/objects/null_action.py
--rw-r--r--   0        0        0     1414 2022-05-24 00:56:37.700976 openkit-1.0.7/openkit/core/objects/null_root_action.py
--rw-r--r--   0        0        0      983 2022-05-22 23:48:26.970897 openkit-1.0.7/openkit/core/objects/null_session.py
--rw-r--r--   0        0        0      642 2022-05-23 00:05:11.557004 openkit-1.0.7/openkit/core/objects/null_web_request_tracer.py
--rw-r--r--   0        0        0     1353 2022-05-21 14:56:16.764765 openkit-1.0.7/openkit/core/objects/root_action.py
--rw-r--r--   0        0        0     6152 2022-05-24 01:12:05.413544 openkit-1.0.7/openkit/core/objects/session.py
--rw-r--r--   0        0        0     1806 2022-05-21 16:04:07.452055 openkit-1.0.7/openkit/core/objects/session_creator.py
--rw-r--r--   0        0        0     9208 2022-05-24 01:11:41.995655 openkit-1.0.7/openkit/core/objects/session_proxy.py
--rw-r--r--   0        0        0     3097 2022-05-23 18:03:33.967216 openkit-1.0.7/openkit/core/objects/web_request_tracer.py
--rw-r--r--   0        0        0     5521 2022-05-24 01:53:48.974543 openkit-1.0.7/openkit/core/session_watchdog.py
--rw-r--r--   0        0        0        0 2022-05-21 01:01:05.680995 openkit-1.0.7/openkit/protocol/__init__.py
--rw-r--r--   0        0        0    20308 2022-05-23 17:58:59.118407 openkit-1.0.7/openkit/protocol/beacon.py
--rw-r--r--   0        0        0      264 2022-05-21 01:01:05.698322 openkit-1.0.7/openkit/protocol/event_type.py
--rw-r--r--   0        0        0     3995 2022-11-04 02:31:57.605059 openkit-1.0.7/openkit/protocol/http_client.py
--rw-r--r--   0        0        0       92 2022-05-21 01:01:05.707064 openkit-1.0.7/openkit/protocol/response_attributes.py
--rw-r--r--   0        0        0     3872 2022-05-21 03:12:38.246284 openkit-1.0.7/openkit/protocol/status_response.py
--rw-r--r--   0        0        0        0 2022-05-21 15:22:23.762869 openkit-1.0.7/openkit/providers/__init__.py
--rw-r--r--   0        0        0      531 2022-05-21 15:26:05.733426 openkit-1.0.7/openkit/providers/session_id.py
--rw-r--r--   0        0        0        0 2022-05-21 01:01:05.771199 openkit-1.0.7/openkit/vendor/__init__.py
--rw-r--r--   0        0        0      671 2022-05-21 01:01:05.811057 openkit-1.0.7/openkit/vendor/mureq/LICENSE
--rw-r--r--   0        0        0        0 2022-05-21 01:01:05.814474 openkit-1.0.7/openkit/vendor/mureq/__init__.py
--rw-r--r--   0        0        0    14476 2022-05-21 01:01:05.820820 openkit-1.0.7/openkit/vendor/mureq/mureq.py
--rw-r--r--   0        0        0      409 2022-05-23 18:26:21.507189 openkit-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-21 00:29:22.441302 openkit-1.0.7/test/__init__.py
--rw-r--r--   0        0        0      840 2022-05-23 14:04:14.266845 openkit-1.0.7/test/test_beacon_cache.py
--rw-r--r--   0        0        0     1991 2022-05-23 14:03:47.779011 openkit-1.0.7/test/test_beacon_cache_evictor.py
--rw-r--r--   0        0        0     2637 2022-05-24 01:09:53.611543 openkit-1.0.7/test/test_session_watchdog.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 openkit-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       75 2022-05-21 01:33:41.411652 openkit-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1099 2022-05-21 00:47:41.295158 openkit-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1039 2022-06-01 20:50:34.577833 openkit-1.0.9/README.md
+-rw-r--r--   0        0        0      107 2022-11-09 00:04:28.340911 openkit-1.0.9/openkit/__init__.py
+-rw-r--r--   0        0        0       29 2022-05-21 04:23:09.995309 openkit-1.0.9/openkit/api/__init__.py
+-rw-r--r--   0        0        0     1297 2022-05-23 00:28:18.853495 openkit-1.0.9/openkit/api/action.py
+-rw-r--r--   0        0        0      909 2022-05-23 18:06:05.885713 openkit-1.0.9/openkit/api/composite.py
+-rw-r--r--   0        0        0      740 2022-05-21 04:35:30.011795 openkit-1.0.9/openkit/api/constants.py
+-rw-r--r--   0        0        0     6553 2022-11-04 02:52:28.882761 openkit-1.0.9/openkit/api/openkit.py
+-rw-r--r--   0        0        0      230 2022-05-22 23:48:35.700302 openkit-1.0.9/openkit/api/openkit_object.py
+-rw-r--r--   0        0        0      288 2022-05-22 23:44:49.543514 openkit-1.0.9/openkit/api/root_action.py
+-rw-r--r--   0        0        0     1027 2022-05-22 23:45:03.082355 openkit-1.0.9/openkit/api/session.py
+-rw-r--r--   0        0        0      678 2022-05-23 00:04:57.322004 openkit-1.0.9/openkit/api/web_request_tracer.py
+-rw-r--r--   0        0        0        0 2022-05-24 01:07:58.229033 openkit-1.0.9/openkit/core/__init__.py
+-rw-r--r--   0        0        0     6305 2022-11-04 02:52:28.882761 openkit-1.0.9/openkit/core/beacon_sender.py
+-rw-r--r--   0        0        0       78 2022-05-23 13:52:41.240176 openkit-1.0.9/openkit/core/caching/__init__.py
+-rw-r--r--   0        0        0     7875 2022-05-23 17:57:45.990341 openkit-1.0.9/openkit/core/caching/beacon_cache.py
+-rw-r--r--   0        0        0      523 2022-05-21 00:29:22.433836 openkit-1.0.9/openkit/core/caching/beacon_key.py
+-rw-r--r--   0        0        0     4976 2022-05-24 01:52:13.921403 openkit-1.0.9/openkit/core/caching/evictor.py
+-rw-r--r--   0        0        0      338 2022-05-21 01:01:05.469940 openkit-1.0.9/openkit/core/communication/__init__.py
+-rw-r--r--   0        0        0      730 2022-05-21 03:10:49.360285 openkit-1.0.9/openkit/core/communication/beacon_abstract.py
+-rw-r--r--   0        0        0     2067 2022-05-23 14:36:41.565746 openkit-1.0.9/openkit/core/communication/beacon_capture_off.py
+-rw-r--r--   0        0        0     3867 2022-05-23 15:09:58.138503 openkit-1.0.9/openkit/core/communication/beacon_capture_on.py
+-rw-r--r--   0        0        0     1562 2022-05-23 14:37:27.062548 openkit-1.0.9/openkit/core/communication/beacon_flush.py
+-rw-r--r--   0        0        0     2506 2022-05-23 14:36:08.501632 openkit-1.0.9/openkit/core/communication/beacon_init.py
+-rw-r--r--   0        0        0      505 2022-05-23 14:30:30.164039 openkit-1.0.9/openkit/core/communication/beacon_terminal.py
+-rw-r--r--   0        0        0      570 2022-11-09 00:01:05.774248 openkit-1.0.9/openkit/core/communication/countdown_latch.py
+-rw-r--r--   0        0        0      721 2022-05-21 01:08:02.309177 openkit-1.0.9/openkit/core/communication/state_utils.py
+-rw-r--r--   0        0        0      110 2022-05-21 01:01:05.607403 openkit-1.0.9/openkit/core/configuration/__init__.py
+-rw-r--r--   0        0        0     2380 2022-05-22 22:42:25.461143 openkit-1.0.9/openkit/core/configuration/beacon_configuration.py
+-rw-r--r--   0        0        0      227 2022-05-21 15:42:21.711277 openkit-1.0.9/openkit/core/configuration/http_client_configuration.py
+-rw-r--r--   0        0        0      623 2022-05-21 01:31:06.268859 openkit-1.0.9/openkit/core/configuration/openkit_configuration.py
+-rw-r--r--   0        0        0     2304 2022-05-22 21:40:08.172030 openkit-1.0.9/openkit/core/configuration/privacy_configuration.py
+-rw-r--r--   0        0        0     2953 2022-05-22 22:53:43.319768 openkit-1.0.9/openkit/core/configuration/server_configuration.py
+-rw-r--r--   0        0        0        0 2022-05-24 01:05:13.937317 openkit-1.0.9/openkit/core/objects/__init__.py
+-rw-r--r--   0        0        0     5111 2022-05-23 18:03:46.293977 openkit-1.0.9/openkit/core/objects/base_action.py
+-rw-r--r--   0        0        0      296 2022-05-21 14:57:53.990929 openkit-1.0.9/openkit/core/objects/leaf_action.py
+-rw-r--r--   0        0        0     1240 2022-05-23 00:28:18.847039 openkit-1.0.9/openkit/core/objects/null_action.py
+-rw-r--r--   0        0        0     1414 2022-05-24 00:56:37.700976 openkit-1.0.9/openkit/core/objects/null_root_action.py
+-rw-r--r--   0        0        0      983 2022-05-22 23:48:26.970897 openkit-1.0.9/openkit/core/objects/null_session.py
+-rw-r--r--   0        0        0      642 2022-05-23 00:05:11.557004 openkit-1.0.9/openkit/core/objects/null_web_request_tracer.py
+-rw-r--r--   0        0        0     1353 2022-05-21 14:56:16.764765 openkit-1.0.9/openkit/core/objects/root_action.py
+-rw-r--r--   0        0        0     6152 2022-05-24 01:12:05.413544 openkit-1.0.9/openkit/core/objects/session.py
+-rw-r--r--   0        0        0     1806 2022-05-21 16:04:07.452055 openkit-1.0.9/openkit/core/objects/session_creator.py
+-rw-r--r--   0        0        0     9208 2022-05-24 01:11:41.995655 openkit-1.0.9/openkit/core/objects/session_proxy.py
+-rw-r--r--   0        0        0     3097 2022-05-23 18:03:33.967216 openkit-1.0.9/openkit/core/objects/web_request_tracer.py
+-rw-r--r--   0        0        0     5521 2022-05-24 01:53:48.974543 openkit-1.0.9/openkit/core/session_watchdog.py
+-rw-r--r--   0        0        0        0 2022-05-21 01:01:05.680995 openkit-1.0.9/openkit/protocol/__init__.py
+-rw-r--r--   0        0        0    20308 2022-05-23 17:58:59.118407 openkit-1.0.9/openkit/protocol/beacon.py
+-rw-r--r--   0        0        0      264 2022-05-21 01:01:05.698322 openkit-1.0.9/openkit/protocol/event_type.py
+-rw-r--r--   0        0        0     3995 2022-11-04 02:31:57.605059 openkit-1.0.9/openkit/protocol/http_client.py
+-rw-r--r--   0        0        0       92 2022-05-21 01:01:05.707064 openkit-1.0.9/openkit/protocol/response_attributes.py
+-rw-r--r--   0        0        0     3872 2022-05-21 03:12:38.246284 openkit-1.0.9/openkit/protocol/status_response.py
+-rw-r--r--   0        0        0        0 2022-05-21 15:22:23.762869 openkit-1.0.9/openkit/providers/__init__.py
+-rw-r--r--   0        0        0      531 2022-05-21 15:26:05.733426 openkit-1.0.9/openkit/providers/session_id.py
+-rw-r--r--   0        0        0        0 2022-05-21 01:01:05.771199 openkit-1.0.9/openkit/vendor/__init__.py
+-rw-r--r--   0        0        0      671 2022-05-21 01:01:05.811057 openkit-1.0.9/openkit/vendor/mureq/LICENSE
+-rw-r--r--   0        0        0        0 2022-05-21 01:01:05.814474 openkit-1.0.9/openkit/vendor/mureq/__init__.py
+-rw-r--r--   0        0        0    14476 2022-05-21 01:01:05.820820 openkit-1.0.9/openkit/vendor/mureq/mureq.py
+-rw-r--r--   0        0        0      409 2022-05-23 18:26:21.507189 openkit-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-21 00:29:22.441302 openkit-1.0.9/test/__init__.py
+-rw-r--r--   0        0        0      840 2022-05-23 14:04:14.266845 openkit-1.0.9/test/test_beacon_cache.py
+-rw-r--r--   0        0        0     1991 2022-05-23 14:03:47.779011 openkit-1.0.9/test/test_beacon_cache_evictor.py
+-rw-r--r--   0        0        0     2637 2022-05-24 01:09:53.611543 openkit-1.0.9/test/test_session_watchdog.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 openkit-1.0.9/PKG-INFO
```

### Comparing `openkit-1.0.7/LICENSE` & `openkit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/README.md` & `openkit-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/api/action.py` & `openkit-1.0.9/openkit/api/action.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/api/composite.py` & `openkit-1.0.9/openkit/api/composite.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/api/constants.py` & `openkit-1.0.9/openkit/api/constants.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/api/openkit.py` & `openkit-1.0.9/openkit/api/openkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,29 @@
         self._session_watchdog = SessionWatchdog(self._logger, SessionWatchdogContext())
 
         self._lock = RLock()
         self._openkit_configuration = OpenkitConfiguration(self)
 
         # Call shutdown on exit signals
         signal.signal(signal.SIGINT, self._signal_handler)
-        self.initialize()
+        self._initialize()
 
-    def initialize(self):
+    def _initialize(self):
         self._beacon_cache_evictor.start()
         self._beacon_sender.initialize()
         self._session_watchdog.initialize()
 
     def _signal_handler(self, signal_number: int, frame):
         self.shutdown()
 
     def wait_for_init_completion(self, timeout_ms: Optional[int] = None) -> bool:
-        raise NotImplementedError("Wait for init completion is not implemented")
+        return self._beacon_sender.wait_for_init_completion(timeout_ms)
 
     def initialized(self) -> bool:
-        raise NotImplementedError("Initialized is not implemented")
+        return self._beacon_sender.initialized()
 
     def create_session(self,
                        ip_address: Optional[str] = None,
                        timestamp: Optional[int] = None,
                        device_id: Optional[int] = None) -> Session:
         self._logger.debug(f"create_session({ip_address}, {timestamp})")
         with self._lock:
```

### Comparing `openkit-1.0.7/openkit/api/session.py` & `openkit-1.0.9/openkit/api/session.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/api/web_request_tracer.py` & `openkit-1.0.9/openkit/api/web_request_tracer.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/beacon_sender.py` & `openkit-1.0.9/openkit/core/beacon_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,17 @@
             if session.state.is_configured_and_open:
                 sessions.append(session)
         return sessions
 
     def remove_session(self, finished_session):
         return self.sessions.remove(finished_session)
 
+    def wait_for_init_completion(self, timeout_ms):
+        self.countdown_latch.wait(timeout_ms)
+
 
 class BeaconSenderThread(Thread):
     def __init__(self, logger: logging.Logger, context: BeaconSendingContext):
         Thread.__init__(self, name="BeaconSenderThread", daemon=True)
         self.logger = logger
         self.shutdown_flag = Event()
         self.context = context
@@ -179,7 +182,13 @@
     def add_session(self, session):
         self.logger.debug(f"Adding session {session}")
         self.context.add_session(session)
 
     @property
     def last_server_configuration(self):
         return self.context.last_server_configuration
+
+    def wait_for_init_completion(self, timeout_ms):
+        self.context.wait_for_init_completion(timeout_ms)
+
+    def initialized(self):
+        return self.context.init_succeeded
```

### Comparing `openkit-1.0.7/openkit/core/caching/beacon_cache.py` & `openkit-1.0.9/openkit/core/caching/beacon_cache.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/caching/beacon_key.py` & `openkit-1.0.9/openkit/core/caching/beacon_key.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/caching/evictor.py` & `openkit-1.0.9/openkit/core/caching/evictor.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/beacon_abstract.py` & `openkit-1.0.9/openkit/core/communication/beacon_abstract.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/beacon_capture_off.py` & `openkit-1.0.9/openkit/core/communication/beacon_capture_off.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/beacon_capture_on.py` & `openkit-1.0.9/openkit/core/communication/beacon_capture_on.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/beacon_flush.py` & `openkit-1.0.9/openkit/core/communication/beacon_flush.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/beacon_init.py` & `openkit-1.0.9/openkit/core/communication/beacon_init.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/communication/state_utils.py` & `openkit-1.0.9/openkit/core/communication/state_utils.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/configuration/beacon_configuration.py` & `openkit-1.0.9/openkit/core/configuration/beacon_configuration.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/configuration/openkit_configuration.py` & `openkit-1.0.9/openkit/core/configuration/openkit_configuration.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/configuration/privacy_configuration.py` & `openkit-1.0.9/openkit/core/configuration/privacy_configuration.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/configuration/server_configuration.py` & `openkit-1.0.9/openkit/core/configuration/server_configuration.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/base_action.py` & `openkit-1.0.9/openkit/core/objects/base_action.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/null_action.py` & `openkit-1.0.9/openkit/core/objects/null_action.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/null_root_action.py` & `openkit-1.0.9/openkit/core/objects/null_root_action.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/null_session.py` & `openkit-1.0.9/openkit/core/objects/null_session.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/null_web_request_tracer.py` & `openkit-1.0.9/openkit/core/objects/null_web_request_tracer.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/root_action.py` & `openkit-1.0.9/openkit/core/objects/root_action.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/session.py` & `openkit-1.0.9/openkit/core/objects/session.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/session_creator.py` & `openkit-1.0.9/openkit/core/objects/session_creator.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/session_proxy.py` & `openkit-1.0.9/openkit/core/objects/session_proxy.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/objects/web_request_tracer.py` & `openkit-1.0.9/openkit/core/objects/web_request_tracer.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/core/session_watchdog.py` & `openkit-1.0.9/openkit/core/session_watchdog.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/protocol/beacon.py` & `openkit-1.0.9/openkit/protocol/beacon.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/protocol/http_client.py` & `openkit-1.0.9/openkit/protocol/http_client.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/protocol/status_response.py` & `openkit-1.0.9/openkit/protocol/status_response.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/providers/session_id.py` & `openkit-1.0.9/openkit/providers/session_id.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/vendor/mureq/LICENSE` & `openkit-1.0.9/openkit/vendor/mureq/LICENSE`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/openkit/vendor/mureq/mureq.py` & `openkit-1.0.9/openkit/vendor/mureq/mureq.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/test/test_beacon_cache.py` & `openkit-1.0.9/test/test_beacon_cache.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/test/test_beacon_cache_evictor.py` & `openkit-1.0.9/test/test_beacon_cache_evictor.py`

 * *Files identical despite different names*

### Comparing `openkit-1.0.7/test/test_session_watchdog.py` & `openkit-1.0.9/test/test_session_watchdog.py`

 * *Files identical despite different names*

