# Comparing `tmp/simpleobsws-1.3.1.tar.gz` & `tmp/simpleobsws-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleobsws-1.3.1.tar", last modified: Wed Jan 12 16:55:02 2022, max compression
+gzip compressed data, was "simpleobsws-1.4.0.tar", last modified: Sun May 28 07:07:06 2023, max compression
```

## Comparing `simpleobsws-1.3.1.tar` & `simpleobsws-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        0 2022-01-12 16:55:02.759563 simpleobsws-1.3.1/
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)     1627 2022-01-12 16:55:02.759563 simpleobsws-1.3.1/PKG-INFO
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      832 2021-09-26 11:53:19.000000 simpleobsws-1.3.1/README.md
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       79 2022-01-12 16:55:02.759563 simpleobsws-1.3.1/setup.cfg
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      884 2022-01-12 16:14:31.000000 simpleobsws-1.3.1/setup.py
-drwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        0 2022-01-12 16:55:02.743935 simpleobsws-1.3.1/simpleobsws.egg-info/
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)     1627 2022-01-12 16:55:02.000000 simpleobsws-1.3.1/simpleobsws.egg-info/PKG-INFO
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      217 2022-01-12 16:55:02.000000 simpleobsws-1.3.1/simpleobsws.egg-info/SOURCES.txt
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        1 2022-01-12 16:55:02.000000 simpleobsws-1.3.1/simpleobsws.egg-info/dependency_links.txt
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       11 2022-01-12 16:55:02.000000 simpleobsws-1.3.1/simpleobsws.egg-info/requires.txt
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       12 2022-01-12 16:55:02.000000 simpleobsws-1.3.1/simpleobsws.egg-info/top_level.txt
--rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)    13799 2022-01-12 16:14:31.000000 simpleobsws-1.3.1/simpleobsws.py
+drwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        0 2023-05-28 07:07:06.028566 simpleobsws-1.4.0/
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)     1072 2023-05-28 06:40:49.000000 simpleobsws-1.4.0/LICENSE
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)     1466 2023-05-28 07:07:06.030567 simpleobsws-1.4.0/PKG-INFO
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      881 2023-05-28 06:40:49.000000 simpleobsws-1.4.0/README.md
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       79 2023-05-28 07:07:06.035566 simpleobsws-1.4.0/setup.cfg
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      877 2023-05-28 07:06:28.000000 simpleobsws-1.4.0/setup.py
+drwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        0 2023-05-28 07:07:06.010566 simpleobsws-1.4.0/simpleobsws.egg-info/
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)     1466 2023-05-28 07:07:05.000000 simpleobsws-1.4.0/simpleobsws.egg-info/PKG-INFO
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)      225 2023-05-28 07:07:05.000000 simpleobsws-1.4.0/simpleobsws.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)        1 2023-05-28 07:07:05.000000 simpleobsws-1.4.0/simpleobsws.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       19 2023-05-28 07:07:05.000000 simpleobsws-1.4.0/simpleobsws.egg-info/requires.txt
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)       12 2023-05-28 07:07:05.000000 simpleobsws-1.4.0/simpleobsws.egg-info/top_level.txt
+-rwxrwxrwx   0 tt2468    (1000) tt2468    (1000)    13929 2023-05-28 06:52:45.000000 simpleobsws-1.4.0/simpleobsws.py
```

### Comparing `simpleobsws-1.3.1/PKG-INFO` & `simpleobsws-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: simpleobsws
-Version: 1.3.1
+Version: 1.4.0
 Summary: A simple obs-websocket library in async Python for people who just want JSON output.
 Home-page: https://github.com/IRLToolkit/simpleobsws
 Author: tt2468
 Author-email: tt2468@gmail.com
-License: UNKNOWN
-Description: # simpleobsws
-        A simple obs-websocket library in Python for people who just want JSON output.
-        
-        ## Please Note
-        simpleobsws >= v1.0.0 is **only** for versions of obs-websocket that are 5.0.0 or higher. If you are using obs-websocket pre-5.0.0, use a pre v1.0.0 version of simpleobsws.
-        
-        Click [here](https://github.com/IRLToolkit/simpleobsws/tree/simpleobsws-4.x) to go to the pre-5.0.0 branch.
-        
-        ## Installing:
-        `pip install simpleobsws` [PyPi Link](https://pypi.org/project/simpleobsws/)
-        
-        ## Docs:
-        - Library docs: [the sort-of docs](/usage.md)
-        - obs-websocket docs: https://github.com/Palakis/obs-websocket/blob/4.x-current/docs/generated/protocol.md
-        
-        ## Samples:
-        Samples are located in the samples folder [here.](/samples)
-        
-        ## IRLTookit Links
-        
-        - https://twitter.com/IRLToolkit
-        - https://irltoolkit.com/discord
-        - https://irltoolkit.com
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Plugins
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# simpleobsws
+A simple obs-websocket library in Python for people who just want JSON output.
+
+## Please Note
+simpleobsws >= v1.0.0 is **only** for versions of obs-websocket that are 5.0.0 or higher. If you are using obs-websocket pre-5.0.0, use a pre v1.0.0 version of simpleobsws.
+
+Click [here](https://github.com/IRLToolkit/simpleobsws/tree/simpleobsws-4.x) to go to the pre-5.0.0 branch.
+
+## Installing:
+`pip install simpleobsws` [PyPi Link](https://pypi.org/project/simpleobsws/)
+
+## Docs:
+- Library docs: [the sort-of docs](/usage.md)
+- obs-websocket docs: https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md
+
+## Samples:
+Samples are located in the samples folder [here.](/samples)
+
+## IRLTookit Links
+
+- Please go to the [obs-websocket Discord](https://discord.gg/WBaSQ3A) for support.
+- https://twitter.com/IRLToolkit
+- https://irltoolkit.com
```

### Comparing `simpleobsws-1.3.1/README.md` & `simpleobsws-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 Click [here](https://github.com/IRLToolkit/simpleobsws/tree/simpleobsws-4.x) to go to the pre-5.0.0 branch.
 
 ## Installing:
 `pip install simpleobsws` [PyPi Link](https://pypi.org/project/simpleobsws/)
 
 ## Docs:
 - Library docs: [the sort-of docs](/usage.md)
-- obs-websocket docs: https://github.com/Palakis/obs-websocket/blob/4.x-current/docs/generated/protocol.md
+- obs-websocket docs: https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md
 
 ## Samples:
 Samples are located in the samples folder [here.](/samples)
 
 ## IRLTookit Links
 
+- Please go to the [obs-websocket Discord](https://discord.gg/WBaSQ3A) for support.
 - https://twitter.com/IRLToolkit
-- https://irltoolkit.com/discord
 - https://irltoolkit.com
```

### Comparing `simpleobsws-1.3.1/setup.py` & `simpleobsws-1.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = open('requirements.txt', 'rt').readlines()
+requirements = [
+    'websockets',
+    'msgpack'
+]
 
 setuptools.setup(
     name="simpleobsws",
-    version="1.3.1",
+    version="1.4.0",
     author="tt2468",
     author_email="tt2468@gmail.com",
     description="A simple obs-websocket library in async Python for people who just want JSON output.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IRLToolkit/simpleobsws",
     py_modules=['simpleobsws'],
```

### Comparing `simpleobsws-1.3.1/simpleobsws.egg-info/PKG-INFO` & `simpleobsws-1.4.0/simpleobsws.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: simpleobsws
-Version: 1.3.1
+Version: 1.4.0
 Summary: A simple obs-websocket library in async Python for people who just want JSON output.
 Home-page: https://github.com/IRLToolkit/simpleobsws
 Author: tt2468
 Author-email: tt2468@gmail.com
-License: UNKNOWN
-Description: # simpleobsws
-        A simple obs-websocket library in Python for people who just want JSON output.
-        
-        ## Please Note
-        simpleobsws >= v1.0.0 is **only** for versions of obs-websocket that are 5.0.0 or higher. If you are using obs-websocket pre-5.0.0, use a pre v1.0.0 version of simpleobsws.
-        
-        Click [here](https://github.com/IRLToolkit/simpleobsws/tree/simpleobsws-4.x) to go to the pre-5.0.0 branch.
-        
-        ## Installing:
-        `pip install simpleobsws` [PyPi Link](https://pypi.org/project/simpleobsws/)
-        
-        ## Docs:
-        - Library docs: [the sort-of docs](/usage.md)
-        - obs-websocket docs: https://github.com/Palakis/obs-websocket/blob/4.x-current/docs/generated/protocol.md
-        
-        ## Samples:
-        Samples are located in the samples folder [here.](/samples)
-        
-        ## IRLTookit Links
-        
-        - https://twitter.com/IRLToolkit
-        - https://irltoolkit.com/discord
-        - https://irltoolkit.com
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Plugins
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# simpleobsws
+A simple obs-websocket library in Python for people who just want JSON output.
+
+## Please Note
+simpleobsws >= v1.0.0 is **only** for versions of obs-websocket that are 5.0.0 or higher. If you are using obs-websocket pre-5.0.0, use a pre v1.0.0 version of simpleobsws.
+
+Click [here](https://github.com/IRLToolkit/simpleobsws/tree/simpleobsws-4.x) to go to the pre-5.0.0 branch.
+
+## Installing:
+`pip install simpleobsws` [PyPi Link](https://pypi.org/project/simpleobsws/)
+
+## Docs:
+- Library docs: [the sort-of docs](/usage.md)
+- obs-websocket docs: https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md
+
+## Samples:
+Samples are located in the samples folder [here.](/samples)
+
+## IRLTookit Links
+
+- Please go to the [obs-websocket Discord](https://discord.gg/WBaSQ3A) for support.
+- https://twitter.com/IRLToolkit
+- https://irltoolkit.com
```

### Comparing `simpleobsws-1.3.1/simpleobsws.py` & `simpleobsws-1.4.0/simpleobsws.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 wsLogger.setLevel(logging.INFO)
 log = logging.getLogger(__name__)
 import asyncio
 import websockets
 import base64
 import hashlib
 import json
+import msgpack
 import uuid
 import time
 import inspect
 import enum
 from dataclasses import dataclass, field
 from inspect import signature
 
@@ -72,16 +73,16 @@
         url: str = "ws://localhost:4444",
         password: str = '',
         identification_parameters: IdentificationParameters = IdentificationParameters()
     ):
         self.url = url
         self.password = password
         self.identification_parameters = identification_parameters
-        self.loop = asyncio.get_event_loop()
 
+        self.http_headers = {}
         self.ws = None
         self.waiters = {}
         self.identified = False
         self.recv_task = None
         self.hello_message = None
         self.event_callbacks = []
         self.cond = asyncio.Condition()
@@ -91,16 +92,16 @@
         if self.ws != None and self.ws.open:
             log.debug('WebSocket session is already open. Returning early.')
             return False
         self.answers = {}
         self.recv_task = None
         self.identified = False
         self.hello_message = None
-        self.ws = await websockets.connect(self.url, max_size=2**24)
-        self.recv_task = self.loop.create_task(self._ws_recv_task())
+        self.ws = await websockets.connect(self.url, subprotocols = ['obswebsocket.msgpack'], extra_headers = self.http_headers, max_size=2**24)
+        self.recv_task = asyncio.create_task(self._ws_recv_task())
         return True
 
     async def wait_until_identified(self, timeout: int = 10):
         if not self.ws.open:
             log.debug('WebSocket session is not open. Returning early.')
             return False
         try:
@@ -136,15 +137,15 @@
         }
         if request.requestData != None:
             request_payload['d']['requestData'] = request.requestData
         log.debug('Sending Request message:\n{}'.format(json.dumps(request_payload, indent=2)))
         waiter = _ResponseWaiter()
         try:
             self.waiters[request_id] = waiter
-            await self.ws.send(json.dumps(request_payload))
+            await self.ws.send(msgpack.packb(request_payload))
             await asyncio.wait_for(waiter.event.wait(), timeout=timeout)
         except asyncio.TimeoutError:
             raise MessageTimeout('The request with type {} timed out after {} seconds.'.format(request.requestType, timeout))
         finally:
             del self.waiters[request_id]
         return self._build_request_response(waiter.response_data)
 
@@ -158,15 +159,15 @@
                 'requestType': request.requestType,
                 'requestId': 'emit_{}'.format(request_id)
             }
         }
         if request.requestData != None:
             request_payload['d']['requestData'] = request.requestData
         log.debug('Sending Request message:\n{}'.format(json.dumps(request_payload, indent=2)))
-        await self.ws.send(json.dumps(request_payload))
+        await self.ws.send(msgpack.packb(request_payload))
 
     async def call_batch(self, requests: list, timeout: int = 15, halt_on_failure: bool = None, execution_type: RequestBatchExecutionType = None, variables: dict = None):
         if not self.identified:
             raise NotIdentifiedError('Calls to requests cannot be made without being identified with obs-websocket.')
         request_batch_id = str(uuid.uuid1())
         request_batch_payload = {
             'op': 8,
@@ -192,15 +193,15 @@
             if request.requestData:
                 request_payload['requestData'] = request.requestData
             request_batch_payload['d']['requests'].append(request_payload)
         log.debug('Sending Request batch message:\n{}'.format(json.dumps(request_batch_payload, indent=2)))
         waiter = _ResponseWaiter()
         try:
             self.waiters[request_batch_id] = waiter
-            await self.ws.send(json.dumps(request_batch_payload))
+            await self.ws.send(msgpack.packb(request_batch_payload))
             await asyncio.wait_for(waiter.event.wait(), timeout=timeout)
         except asyncio.TimeoutError:
             raise MessageTimeout('The request batch timed out after {} seconds.'.format(timeout))
         finally:
             del self.waiters[request_batch_id]
         ret = []
         for result in waiter.response_data['results']:
@@ -228,15 +229,15 @@
             request_payload = {
                 'requestType': request.requestType
             }
             if request.requestData:
                 request_payload['requestData'] = request.requestData
             request_batch_payload['d']['requests'].append(request_payload)
         log.debug('Sending Request batch message:\n{}'.format(json.dumps(request_batch_payload, indent=2)))
-        await self.ws.send(json.dumps(request_batch_payload))
+        await self.ws.send(msgpack.packb(request_batch_payload))
 
     def register_event_callback(self, callback, event: str = None):
         if not inspect.iscoroutinefunction(callback):
             raise EventRegistrationError('Registered functions must be async')
         else:
             self.event_callbacks.append((callback, event))
 
@@ -268,24 +269,24 @@
             authentication_string = base64.b64encode(hashlib.sha256(secret + (self.hello_message['authentication']['challenge'].encode('utf-8'))).digest()).decode('utf-8')
             identify_message['d']['authentication'] = authentication_string
         if self.identification_parameters.ignoreNonFatalRequestChecks != None:
             identify_message['d']['ignoreNonFatalRequestChecks'] = self.identification_parameters.ignoreNonFatalRequestChecks
         if self.identification_parameters.eventSubscriptions != None:
             identify_message['d']['eventSubscriptions'] = self.identification_parameters.eventSubscriptions
         log.debug('Sending Identify message:\n{}'.format(json.dumps(identify_message, indent=2)))
-        await self.ws.send(json.dumps(identify_message))
+        await self.ws.send(msgpack.packb(identify_message))
 
     async def _ws_recv_task(self):
         while self.ws.open:
             message = ''
             try:
                 message = await self.ws.recv()
-                if not message:
+                if not message or type(message) != bytes:
                     continue
-                incoming_payload = json.loads(message)
+                incoming_payload = msgpack.unpackb(message)
 
                 log.debug('Received message:\n{}'.format(json.dumps(incoming_payload, indent=2)))
 
                 op_code = incoming_payload['op']
                 data_payload = incoming_payload['d']
                 if op_code == 7 or op_code == 9: # RequestResponse or RequestBatchResponse
                     paylod_request_id = data_payload['requestId']
@@ -298,29 +299,29 @@
                     except KeyError:
                         log.warning('Discarding request response {} because there is no waiter for it.'.format(paylod_request_id))
                 elif op_code == 5: # Event
                     for callback, trigger in self.event_callbacks:
                         if trigger == None:
                             params = len(signature(callback).parameters)
                             if params == 1:
-                                self.loop.create_task(callback(data_payload))
+                                asyncio.create_task(callback(data_payload))
                             elif params == 2:
-                                self.loop.create_task(callback(data_payload['eventType'], data_payload.get('eventData')))
+                                asyncio.create_task(callback(data_payload['eventType'], data_payload.get('eventData')))
                             elif params == 3:
-                                self.loop.create_task(callback(data_payload['eventType'], data_payload.get('eventIntent'), data_payload.get('eventData')))
+                                asyncio.create_task(callback(data_payload['eventType'], data_payload.get('eventIntent'), data_payload.get('eventData')))
                         elif trigger == data_payload['eventType']:
-                            self.loop.create_task(callback(data_payload.get('eventData')))
+                            asyncio.create_task(callback(data_payload.get('eventData')))
                 elif op_code == 0: # Hello
                     self.hello_message = data_payload
                     await self._send_identify(self.password, self.identification_parameters)
                 elif op_code == 2: # Identified
                     self.identified = True
                     async with self.cond:
                         self.cond.notify_all()
                 else:
                     log.warning('Unknown OpCode: {}'.format(op_code))
             except (websockets.exceptions.ConnectionClosed, websockets.exceptions.ConnectionClosedError, websockets.exceptions.ConnectionClosedOK):
                 log.debug('The WebSocket connection was closed. Code: {} | Reason: {}'.format(self.ws.close_code, self.ws.close_reason))
                 break
-            except json.JSONDecodeError:
+            except (ValueError, msgpack.UnpackException):
                 continue
         self.identified = False
```

