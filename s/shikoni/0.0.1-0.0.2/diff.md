# Comparing `tmp/shikoni-0.0.1.tar.gz` & `tmp/shikoni-0.0.2.tar.gz`

## Comparing `shikoni-0.0.1.tar` & `shikoni-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,72 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 shikoni-0.0.1/Pipfile
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 shikoni-0.0.1/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 shikoni-0.0.1/packages_used.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shikoni-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 shikoni-0.0.1/setup.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/shikoni.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    20327 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 shikoni-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 shikoni-0.0.1/examples/add_server_connection.py
--rw-r--r--   0        0        0     9412 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/ShikoniClasses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/shikoni_main.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/MessageType.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/ShikoniMessageAddConnector.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/ShikoniMessageConnectorName.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/ShikoniMessageConnectorSocket.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/ShikoniMessageRemoveConnector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/base_messages/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/data/MessageTypeClasses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/data/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/data/massage_type_classes.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/ideas/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/ideas/message.txt
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/interfaces/ShikoniMessage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/interfaces/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/message_types/ShikoniMessageString.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/message_types/__init__.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/ClientConnector.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/PackageController.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/ServerConnector.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/ShikoniInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/__init__.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 shikoni-0.0.1/shikoni/tools/host_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.1/temp/.gitkeep
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/find_minimum_package_version.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/packages.json
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/packages_error.json
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/start_test_server.py
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/test_base.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 shikoni-0.0.1/test/test_result.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 shikoni-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 shikoni-0.0.1/LICENSE
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 shikoni-0.0.1/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 shikoni-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 shikoni-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 shikoni-0.0.2/Pipfile
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 shikoni-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 shikoni-0.0.2/main.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 shikoni-0.0.2/message.json
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 shikoni-0.0.2/packages_used.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shikoni-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 shikoni-0.0.2/setup.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/shikoni.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    23365 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 shikoni-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/message_overview.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/MessageType.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageAddConnector.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageAddConnectorGroup.md
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageAddConnectorToGroup.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageConnectorName.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageConnectorSocket.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageRemoveConnector.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageRemoveConnectorFromGroup.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/base_messages/ShikoniMessageRemoveConnectorGroup.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/message_types/ShikoniMessageClear.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/message_types/ShikoniMessageRun.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 shikoni-0.0.2/doc/message_types/ShikoniMessageString.md
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 shikoni-0.0.2/examples/add_server_connection.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 shikoni-0.0.2/notes/upload_package.txt
+-rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/ShikoniClasses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/__init__.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/shikoni_main.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/MessageType.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageAddConnector.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageAddConnectorGroup.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageAddConnectorToGroup.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageConnectorName.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageConnectorSocket.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageRemoveConnector.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageRemoveConnectorFromGroup.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/ShikoniMessageRemoveConnectorGroup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/base_messages/__init__.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/data/MessageTypeClasses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/data/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/data/massage_type_classes.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/ideas/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/ideas/message.txt
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/interfaces/ShikoniMessage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/interfaces/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/message_types/ShikoniMessageClear.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/message_types/ShikoniMessageRun.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/message_types/ShikoniMessageString.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/message_types/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/ClientConnector.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/PackageController.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/ServerConnector.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/ShikoniInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/__init__.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 shikoni-0.0.2/shikoni/tools/host_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shikoni-0.0.2/temp/.gitkeep
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/find_minimum_package_version.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/message.json
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/start_test_server.py
+-rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/test_base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/server_group/control_result.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 shikoni-0.0.2/test/server_group/start_test_server_server_group.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 shikoni-0.0.2/tool_connect/stt_tts.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 shikoni-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 shikoni-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 shikoni-0.0.2/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 shikoni-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 shikoni-0.0.2/PKG-INFO
```

### Comparing `shikoni-0.0.1/main.py` & `shikoni-0.0.2/examples/add_server_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 import sys
 import time
 
 from shikoni.ShikoniClasses import ShikoniClasses
-
-from shikoni.tools.ShikoniInfo import start_shikoni_api
-from shikoni.tools.host_info import request_free_ports
-
 from shikoni.message_types.ShikoniMessageString import ShikoniMessageString
 from shikoni.base_messages.ShikoniMessageAddConnector import ShikoniMessageAddConnector
 from shikoni.base_messages.ShikoniMessageConnectorSocket import ShikoniMessageConnectorSocket
 from shikoni.base_messages.ShikoniMessageRemoveConnector import ShikoniMessageRemoveConnector
 from shikoni.base_messages.ShikoniMessageConnectorName import ShikoniMessageConnectorName
 
 
-def on_message(msg):
+def on_message(msg, shikoni):
     for key, item in msg.items():
         if isinstance(item, ShikoniMessageString):
             print(key, item.message)
         else:
             print(key, item)
 
 
-def start_base_shikoni_server(shikoni: ShikoniClasses, server_port: int, join_server: bool = True):
-    api_server = start_shikoni_api(server_port + 1)
+def start_base_shikoni_server(shikoni: ShikoniClasses, server_port: int):
     shikoni.start_base_server_connection(
-        connection_data=ShikoniMessageConnectorSocket().set_variables(url="0.0.0.0",
-                                                                      port=server_port,
-                                                                      is_server=True,
-                                                                      connection_name="001"),
-        start_loop=join_server
-    )
+        ShikoniMessageConnectorSocket().set_variables(url="0.0.0.0",
+                                                      port=server_port,
+                                                      is_server=True,
+                                                      connection_name="001"))
     time.sleep(20.0)
     shikoni.close_base_server()
-    api_server.terminate()
 
 
 def start_connection_message_test(shikoni: ShikoniClasses, server_address: str, server_port: int):
     # connect to base server
     connector_base_client = shikoni.start_client_connection(
         ShikoniMessageConnectorSocket().set_variables(server_address, server_port, False, "001")
     )
-    free_port = request_free_ports(url=server_address, port=server_port + 1, num_ports=2)
+
     # start new server connections with base server
     connector_message = ShikoniMessageAddConnector(message=[
-        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[0], True, "010"),
-        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[1], True, "011"),
-        # ShikoniMessageConnectorSocket().set_variables(server_address, 19999, False, ""),
+        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", 19980, True, "010"),
+        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", 19981, True, "011"),
+        #ShikoniMessageConnectorSocket().set_variables(server_address, 19999, False, ""),
     ])
     connector_base_client.send_message(connector_message)
     time.sleep(2.0)
 
     # connect to the first new servers
     connector_client_01 = shikoni.start_client_connection(
-        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[0], False, "002")
+        ShikoniMessageConnectorSocket().set_variables(server_address, 19980, False, "002")
     )
     connector_client_01.send_message(ShikoniMessageString("Testing new server: 1"))
     time.sleep(1.0)
     connector_client_01.close_connection()
 
     # connect to the second new servers
     connector_client_02 = shikoni.start_client_connection(
-        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[1], False, "003")
+        ShikoniMessageConnectorSocket().set_variables(server_address, 19981, False, "003")
     )
     connector_client_02.send_message(ShikoniMessageString("Testing new server: 2"))
     time.sleep(1.0)
     connector_client_02.close_connection()
 
     time.sleep(2.0)
 
@@ -76,18 +68,18 @@
 
     connector_base_client.close_connection()
     time.sleep(5.0)
     print()
 
 
 if __name__ == '__main__':
-    shikoni = ShikoniClasses(message_type_decode_file="shikoni/data/massage_type_classes.json",
+    shikoni = ShikoniClasses(message_type_decode_file="data/massage_type_classes.json",
                              default_server_call_function=on_message)
-    # TODO make it save - API key?
-    # TODO find minimum package versions
+    # 1 PORT (server)
+    # 2 client or None
 
     args = sys.argv
     is_client = False
     server_port = 0
     if len(args) > 1:
         server_port = int(args[1])
     if len(args) > 2:
```

### Comparing `shikoni-0.0.1/.idea/workspace.xml` & `shikoni-0.0.2/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `shikoni-0.0.1/.idea/workspace.xml` & `shikoni-0.0.2/.idea/workspace.xml`

```diff
@@ -1,29 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="43705930-4989-4b36-8ce7-19085c29fd42" name="Changes" comment="added test script;
-update setup file;
-added requirements version testing script;
-prepare for upload package;">
-      <change beforePath="$PROJECT_DIR$/.gitignore" beforeDir="false" afterPath="$PROJECT_DIR$/.gitignore" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/Pipfile.lock" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/__inti__.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/examples/add_server_connection.py" beforeDir="false" afterPath="$PROJECT_DIR$/examples/add_server_connection.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/main.py" beforeDir="false" afterPath="$PROJECT_DIR$/main.py" afterDir="false"/>
+    <list default="true" id="43705930-4989-4b36-8ce7-19085c29fd42" name="Changes" comment="edit doc for messages -&gt; syntax was not right;
+update doc -&gt; better readable;
+prepare for version 0.0.2;">
+      <change afterPath="$PROJECT_DIR$/notes/upload_package.txt" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/requirements.txt" beforeDir="false" afterPath="$PROJECT_DIR$/requirements.txt" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/shikoni/data/ShikoniClasses.py" beforeDir="false" afterPath="$PROJECT_DIR$/shikoni/ShikoniClasses.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/shikoni/shikoni_main.py" beforeDir="false" afterPath="$PROJECT_DIR$/shikoni/shikoni_main.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/test/start_test_server.py" beforeDir="false" afterPath="$PROJECT_DIR$/test/start_test_server.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/test/test_base.py" beforeDir="false" afterPath="$PROJECT_DIR$/test/test_base.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -32,15 +21,15 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
-        <entry key="$PROJECT_DIR$" value="main"/>
+        <entry key="$PROJECT_DIR$" value="0.0.1"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
@@ -50,35 +39,35 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "TODO_SCOPE": "All Places",
-    "last_opened_file_path": "D:/progremieren/Phyton/shikoni/src/shikoni",
+    "last_opened_file_path": "D:/progremieren/Phyton/shikoni/doc/message_types",
     "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
-      <recent name="D:\progremieren\Phyton\shikoni\src\shikoni"/>
-      <recent name="D:\progremieren\Phyton\shikoni\examples"/>
-      <recent name="D:\progremieren\Phyton\shikoni\base_messages"/>
-      <recent name="D:\progremieren\Phyton\shikoni\message_types"/>
-      <recent name="D:\progremieren\Phyton\shikoni"/>
+      <recent name="D:\progremieren\Phyton\shikoni\doc\message_types"/>
+      <recent name="D:\progremieren\Phyton\shikoni\doc"/>
+      <recent name="D:\progremieren\Phyton\shikoni\shikoni\message_types"/>
+      <recent name="D:\progremieren\Phyton\shikoni\tool_connect"/>
+      <recent name="D:\progremieren\Phyton\shikoni\shikoni\base_messages"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
+      <recent name="D:\progremieren\Phyton\shikoni\doc\base_messages"/>
+      <recent name="D:\progremieren\Phyton\shikoni\shikoni\message_types"/>
+      <recent name="D:\progremieren\Phyton\shikoni\test\server_group"/>
       <recent name="D:\progremieren\Phyton\shikoni\shikoni"/>
       <recent name="D:\progremieren\Phyton\shikoni\src\shikoni"/>
-      <recent name="D:\progremieren\Phyton\shikoni\src"/>
-      <recent name="D:\progremieren\Phyton\shikoni\test"/>
-      <recent name="D:\progremieren\Phyton\shikoni"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.Python tests in test_base.py">
+  <component name="RunManager" selected="Python.stt_tts">
     <configuration name="ShikoniInfo" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -113,136 +102,121 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="main" type="PythonConfigurationType" factoryName="Python">
+    <configuration name="main_client" type="PythonConfigurationType" factoryName="Python">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
-      <option name="SDK_HOME" value="D:\progremieren\Phyton\shikoni\venv\Scripts\python.exe"/>
-      <option name="SDK_NAME" value="Python 3.10 (shikoni)"/>
+      <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="SCRIPT_NAME" value="$PROJECT_DIR$/main.py"/>
-      <option name="PARAMETERS" value=""/>
+      <option name="PARAMETERS" value="19999 client"/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="main_client" type="PythonConfigurationType" factoryName="Python">
+    <configuration name="main_server" type="PythonConfigurationType" factoryName="Python" singleton="false">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="SCRIPT_NAME" value="$PROJECT_DIR$/main.py"/>
-      <option name="PARAMETERS" value="19999 client"/>
+      <option name="PARAMETERS" value="19999"/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="main_server" type="PythonConfigurationType" factoryName="Python" singleton="false">
+    <configuration name="stt_tts" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tool_connect"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/main.py"/>
-      <option name="PARAMETERS" value="19999"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tool_connect/stt_tts.py"/>
+      <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test.test_base.TestClass" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_base.TestClass" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/test"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test.test_base.TestClass&quot;"/>
+      <option name="_new_target" value="&quot;test_base.TestClass&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test.test_base.TestClass" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="shikoni"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/shikoni/test"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test.test_base.TestClass&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests in test_base.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_base.TestClass.test_client_open_server_group_connection" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="shikoni"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/test"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/test/test_base.py&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <option name="_new_target" value="&quot;test_base.TestClass.test_client_open_server_group_connection&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.main_server"/>
       <item itemvalue="Python.main_client"/>
-      <item itemvalue="Python.main"/>
+      <item itemvalue="Python.stt_tts"/>
       <item itemvalue="Python.find_minimum_package_version"/>
       <item itemvalue="Python.ShikoniInfo"/>
-      <item itemvalue="Python tests.Python tests for test.test_base.TestClass"/>
-      <item itemvalue="Python tests.Python tests in test_base.py"/>
+      <item itemvalue="Python tests.Python tests for test_base.TestClass.test_client_open_server_group_connection"/>
+      <item itemvalue="Python tests.Python tests for test_base.TestClass"/>
     </list>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.Python tests in test_base.py"/>
-        <item itemvalue="Python.find_minimum_package_version"/>
-        <item itemvalue="Python tests.Python tests for test.test_base.TestClass"/>
-        <item itemvalue="Python tests.Python tests for test.test_base.TestClass"/>
+        <item itemvalue="Python.stt_tts"/>
+        <item itemvalue="Python tests.Python tests for test_base.TestClass.test_client_open_server_group_connection"/>
+        <item itemvalue="Python tests.Python tests for test_base.TestClass"/>
         <item itemvalue="Python.ShikoniInfo"/>
+        <item itemvalue="Python.find_minimum_package_version"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="43705930-4989-4b36-8ce7-19085c29fd42" name="Changes" comment=""/>
@@ -339,15 +313,71 @@
 prepare for upload package;">
       <created>1683482008265</created>
       <option name="number" value="00012"/>
       <option name="presentableId" value="LOCAL-00012"/>
       <option name="project" value="LOCAL"/>
       <updated>1683482008265</updated>
     </task>
-    <option name="localTasksCounter" value="13"/>
+    <task id="LOCAL-00013" summary="fixed package upload">
+      <created>1683486603076</created>
+      <option name="number" value="00013"/>
+      <option name="presentableId" value="LOCAL-00013"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683486603076</updated>
+    </task>
+    <task id="LOCAL-00014" summary="added files to .gitignore">
+      <created>1683486662611</created>
+      <option name="number" value="00014"/>
+      <option name="presentableId" value="LOCAL-00014"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683486662611</updated>
+    </task>
+    <task id="LOCAL-00015" summary="added doc;
+update readme to include doc;">
+      <created>1684006340728</created>
+      <option name="number" value="00015"/>
+      <option name="presentableId" value="LOCAL-00015"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1684006340728</updated>
+    </task>
+    <task id="LOCAL-00016" summary="added connection group -&gt; need testing">
+      <created>1684018778715</created>
+      <option name="number" value="00016"/>
+      <option name="presentableId" value="LOCAL-00016"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1684018778715</updated>
+    </task>
+    <task id="LOCAL-00017" summary="added connection group messages;
+added connection group start/stop functions;
+found bug in finding free port;">
+      <created>1684091894901</created>
+      <option name="number" value="00017"/>
+      <option name="presentableId" value="LOCAL-00017"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1684091894901</updated>
+    </task>
+    <task id="LOCAL-00018" summary="bugfix connection group;
+added shikoni message &quot;run&quot;;
+added first tool chain -&gt; STT &gt; TTS;">
+      <created>1685232629299</created>
+      <option name="number" value="00018"/>
+      <option name="presentableId" value="LOCAL-00018"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685232629299</updated>
+    </task>
+    <task id="LOCAL-00019" summary="edit doc for messages -&gt; syntax was not right;
+update doc -&gt; better readable;
+prepare for version 0.0.2;">
+      <created>1685251115242</created>
+      <option name="number" value="00019"/>
+      <option name="presentableId" value="LOCAL-00019"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685251115242</updated>
+    </task>
+    <option name="localTasksCounter" value="20"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -374,18 +404,31 @@
     <MESSAGE value="added start script"/>
     <MESSAGE value="fixed setup.py;"/>
     <MESSAGE value="added requirements.txt"/>
     <MESSAGE value="added test script;
 update setup file;
 added requirements version testing script;
 prepare for upload package;"/>
-    <option name="LAST_COMMIT_MESSAGE" value="added test script;
-update setup file;
-added requirements version testing script;
-prepare for upload package;"/>
+    <MESSAGE value="fixed package upload"/>
+    <MESSAGE value="added files to .gitignore"/>
+    <MESSAGE value="added doc;
+update readme to include doc;"/>
+    <MESSAGE value="added connection group -&gt; need testing"/>
+    <MESSAGE value="added connection group messages;
+added connection group start/stop functions;
+found bug in finding free port;"/>
+    <MESSAGE value="bugfix connection group;
+added shikoni message &quot;run&quot;;
+added first tool chain -&gt; STT &gt; TTS;"/>
+    <MESSAGE value="edit doc for messages -&gt; syntax was not right;
+update doc -&gt; better readable;
+prepare for version 0.0.2;"/>
+    <option name="LAST_COMMIT_MESSAGE" value="edit doc for messages -&gt; syntax was not right;
+update doc -&gt; better readable;
+prepare for version 0.0.2;"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/shikoni/tools/MessageConverter.py</url>
           <line>53</line>
@@ -402,14 +445,54 @@
           <option name="timeStamp" value="86"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/temp/for_testing.py</url>
           <line>51</line>
           <option name="timeStamp" value="87"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/main.py</url>
+          <line>165</line>
+          <option name="timeStamp" value="112"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/main.py</url>
+          <line>164</line>
+          <option name="timeStamp" value="114"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/shikoni/ShikoniClasses.py</url>
+          <line>328</line>
+          <option name="timeStamp" value="121"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/main.py</url>
+          <line>45</line>
+          <option name="timeStamp" value="122"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/shikoni/ShikoniClasses.py</url>
+          <line>323</line>
+          <option name="timeStamp" value="123"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/shikoni/ShikoniClasses.py</url>
+          <line>331</line>
+          <option name="timeStamp" value="126"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tool_connect/stt_tts.py</url>
+          <line>83</line>
+          <option name="timeStamp" value="127"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/shikoni/tools/ServerConnector.py</url>
+          <line>43</line>
+          <option name="timeStamp" value="132"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
     <watches-manager>
       <configuration name="PythonConfigurationType">
         <watch expression="self.shikoni"/>
       </configuration>
     </watches-manager>
```

### Comparing `shikoni-0.0.1/shikoni/ShikoniClasses.py` & `shikoni-0.0.2/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,198 +1,200 @@
 import json
+import pathlib
+import sys
 import time
-from typing import BinaryIO
-from multiprocessing import Process
-from typing import Dict
-
-from shikoni.data.MessageTypeClasses import get_message_type_classes
-
-from shikoni.tools.PackageController import PackageController
-from shikoni.base_messages.MessageType import MessageType
-from shikoni.tools.ClientConnector import ClientConnector
-from shikoni.tools.ServerConnector import ServerConnector
 
+from shikoni.ShikoniClasses import ShikoniClasses
+
+from shikoni.tools.ShikoniInfo import start_shikoni_api
+from shikoni.tools.host_info import request_free_ports
+from shikoni.tools.host_info import find_free_ports
+
+from shikoni.message_types.ShikoniMessageString import ShikoniMessageString
 from shikoni.base_messages.ShikoniMessageAddConnector import ShikoniMessageAddConnector
+from shikoni.base_messages.ShikoniMessageConnectorSocket import ShikoniMessageConnectorSocket
 from shikoni.base_messages.ShikoniMessageRemoveConnector import ShikoniMessageRemoveConnector
+from shikoni.base_messages.ShikoniMessageConnectorName import ShikoniMessageConnectorName
+
+from shikoni.base_messages.ShikoniMessageAddConnectorGroup import ShikoniMessageAddConnectorGroup
+from shikoni.base_messages.ShikoniMessageRemoveConnectorGroup import ShikoniMessageRemoveConnectorGroup
 
+from shikoni.base_messages.ShikoniMessageAddConnectorToGroup import ShikoniMessageAddConnectorToGroup
 
-class ShikoniClasses:
-    connections_server: Dict[str, Process] = {}
-    base_connection_server = None
-    connections_clients: Dict[str, ClientConnector] = {}
-    do_running = True
-
-    def __init__(self, default_server_call_function=None,
-                 base_server_call_function=None,
-                 message_type_decode_file: str = None):
-        self.message_type_decode_file = message_type_decode_file
-        self.message_type_dictionary = get_message_type_classes(message_type_decode_file)
-
-        self.package_controller = PackageController()
-        self.default_server_call_function = default_server_call_function
-        self.connector_server = ServerConnector(
-            shikoni=self,
-            external_on_base_messag=self.base_server_call_function,
-            external_on_message=self.default_server_call_function)
-        #self.message_query_class = Queue()
-
-    ########### CAll FUNCTIONS #################
-
-    def base_server_call_function(self, message_class):
-        if isinstance(message_class, ShikoniMessageAddConnector):
-            self.message_connection_start(message_class)
-        elif isinstance(message_class, ShikoniMessageRemoveConnector):
-            self.message_connection_close(message_class)
-
-    ########### MESSAGE CALL FUNCTIONS #################
-
-    def message_connection_start(self, shikoni_message_add_connector: ShikoniMessageAddConnector):
-        client_connections = []
-        server_connections = []
-        for connection_item in shikoni_message_add_connector.message:
-            if connection_item.is_server:
-                server_connections.append(connection_item)
-            else:
-                client_connections.append(connection_item)
-
-        self.start_server_connections(server_connections)
-        self.start_client_connections(client_connections)
-
-    def message_connection_close(self, shikoni_message_add_connector: ShikoniMessageRemoveConnector):
-        client_connections = []
-        server_connections = []
-        for connection_item in shikoni_message_add_connector.message:
-            if connection_item.is_server:
-                server_connections.append(connection_item.connection_name)
-            else:
-                client_connections.append(connection_item.connection_name)
-
-        self.close_server_connections(server_connections)
-        self.close_client_connections(client_connections)
-
-    ########### MESSAGE ENCODE FUNCTIONS #################
-
-    def encode_message_from_file(self, file_io: BinaryIO):
-        message_type = MessageType()
-        message_type.decode_io(file_io)
-        message_class_info = self.message_type_dictionary[str(message_type.type_id)]
-
-        message_class = self.package_controller.get_module_class(
-            package_import_path=message_class_info["module"],
-            class_name=message_class_info["class"])
-        message_class.decode_io(file_io)
-        return message_class
-
-    def encode_message(self, message_bytes: bytearray):
-        message_type = MessageType()
-        message_type.decode_bytes(message_bytes)
-        message_class_info = self.message_type_dictionary[str(message_type.type_id)]
-
-        message_class = self.package_controller.get_module_class(
-            package_import_path=message_class_info["module"],
-            class_name=message_class_info["class"])
-        message_class.shikoni = self
-        message_class.decode_bytes(message_bytes)
-        return message_class
-
-    ########### BASE SERVER FUNCTIONS #################
-
-    def start_base_server_connection(self, connection_data, start_loop: bool = True):
-        if connection_data.connection_name in self.connections_server:
-            return
-
-        server_process = self.connector_server.start_server_connection_as_subprocess(connection_data.url,
-                                                                                     connection_data.port,
-                                                                                     connection_data.connection_name,
-                                                                                     is_base_server=True)
-        # self.connector_server.prepare_server_dict(connection_data.connection_name)
-        self.base_connection_server = server_process
-        if start_loop:
-            self.connector_server.server_loop()
-        return self.connector_server
-
-    def close_base_server(self):
-        self.base_connection_server.terminate()
-        self.base_connection_server = None
-
-    ########### SERVER FUNCTIONS #################
-
-    def start_server_connections(self, connection_data_list: list):
-        return_list = []
-        for connection_data in connection_data_list:
-            if connection_data.connection_name in self.connections_server:
-                continue
-            server_process = self.connector_server.start_server_connection_as_subprocess(connection_data.url,
-                                                                                         connection_data.port,
-                                                                                         connection_data.connection_name)
-            self.connector_server.prepare_server_dict(connection_data.connection_name)
-            self.connections_server[connection_data.connection_name] = server_process
-            return_list.append(connection_data.connection_name)
-        return return_list
-
-    def close_server_connections(self, server_connections):
-        for connection_names in server_connections:
-            if connection_names in self.connections_server:
-                self.connections_server.pop(connection_names).terminate()
-                self.connector_server.remove_server_connection(connection_names)
-
-    def close_all_server_connections(self):
-        for connection_names, connector_server in self.connections_server.items():
-            self.connections_server.pop(connection_names).terminate()
-            self.connector_server.remove_server_connection(connection_names)
-        self.connections_server.clear()
-
-
-    ########### CLIENT FUNCTIONS #################
-
-    def start_client_connection(self, shikoni_message_connector_socket):
-        if shikoni_message_connector_socket.connection_name not in self.connections_clients:
-            client_connector = ClientConnector(
-                connect_url=shikoni_message_connector_socket.url,
-                connect_port=shikoni_message_connector_socket.port,
-                shikoni=self,
-                connection_name=shikoni_message_connector_socket.connection_name)
-            client_connector.start_connection()
-            self.connections_clients[shikoni_message_connector_socket.connection_name] = client_connector
-            return client_connector
-
-    def start_client_connections(self, shikoni_message_connector_socket_list: list):
-        added_clients = {}
-        for shikoni_message_connector_socket in shikoni_message_connector_socket_list:
-            if shikoni_message_connector_socket.connection_name in self.connections_clients:
-                continue
-            client_connector = ClientConnector(
-                connect_url=shikoni_message_connector_socket.url,
-                connect_port=shikoni_message_connector_socket.port,
-                shikoni=self,
-                connection_name=shikoni_message_connector_socket.connection_name)
-            client_connector.start_connection()
-            self.connections_clients[shikoni_message_connector_socket.connection_name] = client_connector
-            added_clients[shikoni_message_connector_socket.connection_name] = client_connector
-        return added_clients
-
-    def close_all_client_connections(self):
-        for connection_names, connector_client in self.connections_clients.items():
-            connector_client.close_connection()
-
-    def close_client_connections(self, client_connections):
-        for connection_name in client_connections:
-            if connection_name in self.connections_clients:
-                self.connections_clients.pop(connection_name).close_connection()
-
-
-
-    ########### DIV #################
-
-
-    def wait_until_closed(self):
-        while self.do_running:
-            time.sleep(1.0)
-        self.close_all_client_connections()
-        self.close_all_server_connections()
-
-    def send_to_all_clients(self, message):
-        for connection_names, connector_client in self.connections_clients.items():
-            connector_client.send_message(message)
 
-    def get_message_class(self, type_id: int):
-        self.package_controller.import_module([self.message_type_dictionary[str(type_id)]])
+def on_message(msg, shikoni):
+    group_name = msg["group_name"]
+    messages = msg["messages"]
+    output_file = pathlib.Path("temp").joinpath("message.json")
+    print(msg)
+    output_json = {"group_name": group_name}
+    messages_json = {}
+    for key, message in messages.items():
+        messages_json[key] = message.message
+    output_json["messages"] = messages_json
+
+    ################
+
+    with open(output_file) as f:
+        output_string = f.read()
+    if len(output_string) > 2:
+        output_string = "{0}, {1}]".format(output_string[:-1], json.dumps(messages_json))
+    else:
+        output_string = "{0}{1}]".format(output_string[:-1], json.dumps(messages_json))
+    print(output_string)
+    with open(output_file, "w") as f:
+        f.write(output_string)
+    if group_name == "102":
+        shikoni.send_to_all_clients(message=ShikoniMessageString("Testing"), group_name=group_name)
+
+
+
+
+def on_message_client_test(msg):
+    print(msg)
+
+
+def start_base_shikoni_server(shikoni: ShikoniClasses, server_port: int, join_server: bool = True):
+    api_server = start_shikoni_api(server_port + 1)
+    shikoni.start_base_server_connection(
+        connection_data=ShikoniMessageConnectorSocket().set_variables(url="0.0.0.0",
+                                                                      port=server_port,
+                                                                      is_server=True,
+                                                                      connection_name="001"),
+        start_loop=join_server
+    )
+    time.sleep(20.0)
+    shikoni.close_base_server()
+    api_server.terminate()
+
+
+def start_connection_message_test(shikoni: ShikoniClasses, server_address: str, server_port: int):
+    # connect to base server
+    connector_base_client = shikoni.start_client_connection(
+        ShikoniMessageConnectorSocket().set_variables(server_address, server_port, False, "001")
+    )
+    free_port = request_free_ports(url=server_address, port=server_port + 1, num_ports=2)
+    # start new server connections with base server
+    connector_message = ShikoniMessageAddConnector(message=[
+        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[0], True, "010"),
+        ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[1], True, "011"),
+        # ShikoniMessageConnectorSocket().set_variables(server_address, 19999, False, ""),
+    ])
+    connector_base_client.send_message(connector_message)
+    time.sleep(2.0)
+
+    # connect to the first new servers
+    connector_client_01 = shikoni.start_client_connection(
+        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[0], False, "002")
+    )
+    connector_client_01.send_message(ShikoniMessageString("Testing new server: 1"))
+    time.sleep(1.0)
+    connector_client_01.close_connection()
+
+    # connect to the second new servers
+    connector_client_02 = shikoni.start_client_connection(
+        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[1], False, "003")
+    )
+    connector_client_02.send_message(ShikoniMessageString("Testing new server: 2"))
+    time.sleep(1.0)
+    connector_client_02.close_connection()
+
+    time.sleep(2.0)
+
+    connector_message = ShikoniMessageRemoveConnector(message=[
+        ShikoniMessageConnectorName().set_variables(True, "010"),
+        ShikoniMessageConnectorName().set_variables(True, "011"),
+    ])
+    connector_base_client.send_message(connector_message)
+
+    connector_base_client.close_connection()
+    time.sleep(5.0)
+    print()
+
+
+def start_group_connection_message_test(shikoni: ShikoniClasses, server_address: str, server_port: int):
+    group_name_01 = "101"
+    group_name_02 = "102"
+
+    # connect to base server
+    connector_base_client = shikoni.start_client_connection(
+        ShikoniMessageConnectorSocket().set_variables(server_address, server_port, False, "001")
+    )
+
+    free_port = request_free_ports(url=server_address, port=server_port + 1, num_ports=4)
+    print(free_port)
+
+    # start first server connection group
+    connector_message = ShikoniMessageAddConnectorGroup().set_variables(
+        group_name=group_name_01,
+        connector_socket_list=[
+            ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[0], True, "010"),
+            ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[1], True, "011"),
+            # ShikoniMessageConnectorSocket().set_variables(server_address, free_port[2], False, ""),
+        ])
+    connector_base_client.send_message(connector_message)
+    print("open group connection 1")
+    time.sleep(2.0)
+
+    # start second server connection group
+    connector_message = ShikoniMessageAddConnectorGroup().set_variables(
+        group_name=group_name_02,
+        connector_socket_list=[
+            ShikoniMessageConnectorSocket().set_variables(server_address, free_port[0], False, "0"),
+            ShikoniMessageConnectorSocket().set_variables(server_address, free_port[1], False, "1"),
+            ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[2], True, "012")
+        ])
+    connector_base_client.send_message(connector_message)
+    print("open group connection 2")
+    time.sleep(2.0)
+
+    # add client to first server connection group
+    # connector_message = ShikoniMessageAddConnectorToGroup().set_variables(
+    #    group_name=group_name_01,
+    #    connector_socket_list=[
+    #        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[2], False, ""),
+    #    ])
+    # connector_base_client.send_message(connector_message)
+    # time.sleep(2.0)
+
+    ##############################################################
+
+    # connect to the first new servers
+    connector_client_01 = shikoni.start_client_connection(
+        ShikoniMessageConnectorSocket().set_variables(server_address, free_port[2], False, "002")
+    )
+    connector_client_01.send_message(ShikoniMessageString("start"))
+    time.sleep(1.0)
+    connector_client_01.close_connection()
+
+    ##############################################################
+
+    connector_base_client.close_connection()
+    time.sleep(5.0)
+    print()
+
+
+if __name__ == '__main__':
+    shikoni = ShikoniClasses(message_type_decode_file="shikoni/data/massage_type_classes.json",
+                             default_server_call_function=on_message)
+    # TODO make it save - API key?
+    # TODO find minimum package versions - DONE ???
+    # TODO add connection group test
+    args = sys.argv
+    is_client = False
+    server_port = 0
+    if len(args) > 1:
+        server_port = int(args[1])
+    if len(args) > 2:
+        if args[2] == "client":
+            is_client = True
+    output_file = pathlib.Path("temp").joinpath("message.json")
+
+    if server_port > 0:
+        if is_client:
+            # start_connection_message_test(shikoni, "127.0.0.1", server_port)
+            start_group_connection_message_test(shikoni, "127.0.0.1", server_port)
+        else:
+
+            with open(output_file, "w") as f:
+                f.write("[")
+            start_base_shikoni_server(shikoni, server_port)
```

### Comparing `shikoni-0.0.1/shikoni/shikoni_main.py` & `shikoni-0.0.2/shikoni/shikoni_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from shikoni.ShikoniClasses import ShikoniClasses
 
 from shikoni.tools.ShikoniInfo import start_shikoni_api
 from shikoni.message_types.ShikoniMessageString import ShikoniMessageString
 from shikoni.base_messages.ShikoniMessageConnectorSocket import ShikoniMessageConnectorSocket
 
 
-def on_message(msg):
+def on_message(msg, shikoni):
     # add stuff here
 
     # example
     for key, item in msg.items():
         if isinstance(item, ShikoniMessageString):
             print(key, item.message)
         else:
```

### Comparing `shikoni-0.0.1/shikoni/base_messages/MessageType.py` & `shikoni-0.0.2/shikoni/base_messages/MessageType.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/shikoni/base_messages/ShikoniMessageAddConnector.py` & `shikoni-0.0.2/shikoni/base_messages/ShikoniMessageAddConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         message_length = super().decode_io(file_io)
 
         message_list_length_length = int.from_bytes(file_io.read(1), "big")
         message_list_length = int.from_bytes(file_io.read(message_list_length_length), "big")
 
         message = []
         for _ in range(message_list_length):
-            message.append(self.shikoni.encode_message_from_file(file_io))
+            message.append(self.shikoni.decode_message_from_file(file_io))
         self.message = message
 
     def decode_bytes(self, message_bytes: bytearray):
         message_length = super().decode_bytes(message_bytes)
 
         message_list_length = self.decode_bytes_length(message_bytes)
         message = []
         for _ in range(message_list_length):
-            message.append(self.shikoni.encode_message(message_bytes))
+            message.append(self.shikoni.decode_message(message_bytes))
         self.message = message
 
     def encode(self, message_bytes=b""):
         return super().encode(self.encode_message())
```

### Comparing `shikoni-0.0.1/shikoni/base_messages/ShikoniMessageConnectorName.py` & `shikoni-0.0.2/shikoni/base_messages/ShikoniMessageConnectorName.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/shikoni/base_messages/ShikoniMessageConnectorSocket.py` & `shikoni-0.0.2/shikoni/base_messages/ShikoniMessageConnectorSocket.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,20 +10,27 @@
     def __init__(self, message=None, message_type: MessageType = None, shikoni=None):
         super().__init__(message, message_type, shikoni)
         self.message_type.type_id = 2  # Connector Socket
         self.is_server = True
         self.port: int = 0
         self.url: str = ""
         self.connection_name: str = ""
+        self.connection_path: str = ""
 
-    def set_variables(self, url: str, port: int, is_server: bool, connection_name: str):
+    def set_variables(self,
+                      url: str,
+                      port: int,
+                      is_server: bool,
+                      connection_name: str,
+                      connection_path: str = ""):
         self.is_server = is_server
         self.port: int = port
         self.url: str = url
         self.connection_name: str = connection_name
+        self.connection_path: str = connection_path
         return self
 
     ############### MESSAGE ENCODE FUNCTION ################
 
     def encode_message(self):
         return_bytes = b""
 
@@ -40,16 +47,20 @@
         port_bytes = port_bytes.lstrip(bytes([0]))
         return_bytes += self.encode_bytes_length(len(port_bytes)) + port_bytes
 
         url_bytes = self.url.encode("utf-8")
         return_bytes += self.encode_bytes_length(len(url_bytes)) + url_bytes
 
         connection_name_bytes = self.connection_name.encode("utf-8")
+        return_bytes += self.encode_bytes_length(len(connection_name_bytes)) + connection_name_bytes
 
-        return return_bytes + self.encode_bytes_length(len(connection_name_bytes)) + connection_name_bytes
+        connection_path_bytes = self.connection_path.encode("utf-8")
+        return_bytes += self.encode_bytes_length(len(connection_path_bytes)) + connection_path_bytes
+
+        return return_bytes
 
     ############### ShikoniMessage FUNCTION ################
 
     def decode_io(self, file_io: BinaryIO):
         message_length = super().decode_io(file_io)
 
         is_server_length = self.decode_bytes_length_io(file_io)
@@ -59,18 +70,22 @@
         port = int.from_bytes(file_io.read(port_length), "big")
 
         url_length = self.decode_bytes_length_io(file_io)
         url = file_io.read(url_length).decode()
 
         connection_name_length = self.decode_bytes_length_io(file_io)
         connection_name = file_io.read(connection_name_length).decode()
+
+        connection_path_length = self.decode_bytes_length_io(file_io)
+        connection_path = file_io.read(connection_path_length).decode()
         self.is_server = is_server == 1
         self.port = port
         self.url = url
         self.connection_name = connection_name
+        self.connection_path = connection_path
 
     def decode_bytes(self, message_bytes: bytearray):
         message_length = super().decode_bytes(message_bytes)
 
         is_server_length = self.decode_bytes_length(message_bytes)
         is_server = int.from_bytes(message_bytes[:is_server_length], "big")
         del message_bytes[:is_server_length]
@@ -83,14 +98,19 @@
         url = message_bytes[:url_length].decode()
         del message_bytes[:url_length]
 
         connection_name_length = self.decode_bytes_length(message_bytes)
         connection_name = message_bytes[:connection_name_length].decode()
         del message_bytes[:connection_name_length]
 
+        connection_path_length = self.decode_bytes_length(message_bytes)
+        connection_path = message_bytes[:connection_path_length].decode()
+        del message_bytes[:connection_path_length]
+
         self.is_server = is_server == 1
         self.port = port
         self.url = url
         self.connection_name = connection_name
+        self.connection_path = connection_path
 
     def encode(self, message_bytes=b""):
         return super().encode(self.encode_message())
```

### Comparing `shikoni-0.0.1/shikoni/base_messages/ShikoniMessageRemoveConnector.py` & `shikoni-0.0.2/shikoni/base_messages/ShikoniMessageRemoveConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         message_length = super().decode_io(file_io)
 
         message_list_length_length = int.from_bytes(file_io.read(1), "big")
         message_list_length = int.from_bytes(file_io.read(message_list_length_length), "big")
 
         message = []
         for _ in range(message_list_length):
-            message.append(self.shikoni.encode_message_from_file(file_io))
+            message.append(self.shikoni.decode_message_from_file(file_io))
         self.message = message
 
     def decode_bytes(self, message_bytes: bytearray):
         message_length = super().decode_bytes(message_bytes)
 
         message_list_length = self.decode_bytes_length(message_bytes)
         message = []
         for _ in range(message_list_length):
-            message.append(self.shikoni.encode_message(message_bytes))
+            message.append(self.shikoni.decode_message(message_bytes))
         self.message = message
 
     def encode(self, message_bytes=b""):
         return super().encode(self.encode_message())
```

### Comparing `shikoni-0.0.1/shikoni/data/massage_type_classes.json` & `shikoni-0.0.2/shikoni/data/massage_type_classes.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'100'": "OrderedDict([('module', 'shikoni.message_types.ShikoniMessageRun'), ('class', "*

 * *          "'ShikoniMessageRun')])",*

 * * "'103'": "OrderedDict([('module', 'shikoni.message_types.ShikoniMessageInteger'), ('class', "*

 * *          "'ShikoniMessageInteger')])",*

 * * "'5'": "OrderedDict([('module', 'shikoni.base_messages.ShikoniMessageAddConnectorGroup'), "*

 * *        "('class', 'ShikoniMessageAddConnectorGroup')])",*

 * * "'6'": "OrderedDict([('module', 'shikoni.base_messages.ShikoniMessageRemoveConnectorGroup'), "*

 * *    […]*

```diff
@@ -1,26 +1,50 @@
 {
     "1": {
         "class": "ShikoniMessageAddConnector",
         "module": "shikoni.base_messages.ShikoniMessageAddConnector"
     },
+    "100": {
+        "class": "ShikoniMessageRun",
+        "module": "shikoni.message_types.ShikoniMessageRun"
+    },
     "101": {
         "class": "ShikoniMessageString",
         "module": "shikoni.message_types.ShikoniMessageString"
     },
     "102": {
         "class": "ShikoniMessageInteger",
         "module": "shikoni.message_types.ShikoniMessageInteger"
     },
+    "103": {
+        "class": "ShikoniMessageInteger",
+        "module": "shikoni.message_types.ShikoniMessageInteger"
+    },
     "2": {
         "class": "ShikoniMessageConnectorSocket",
         "module": "shikoni.base_messages.ShikoniMessageConnectorSocket"
     },
     "3": {
         "class": "ShikoniMessageRemoveConnector",
         "module": "shikoni.base_messages.ShikoniMessageRemoveConnector"
     },
     "4": {
         "class": "ShikoniMessageConnectorName",
         "module": "shikoni.base_messages.ShikoniMessageConnectorName"
+    },
+    "5": {
+        "class": "ShikoniMessageAddConnectorGroup",
+        "module": "shikoni.base_messages.ShikoniMessageAddConnectorGroup"
+    },
+    "6": {
+        "class": "ShikoniMessageRemoveConnectorGroup",
+        "module": "shikoni.base_messages.ShikoniMessageRemoveConnectorGroup"
+    },
+    "7": {
+        "class": "ShikoniMessageAddConnectorToGroup",
+        "module": "shikoni.base_messages.ShikoniMessageAddConnectorToGroup"
+    },
+    "8": {
+        "class": "ShikoniMessageRemoveConnectorFromGroup",
+        "module": "shikoni.base_messages.ShikoniMessageRemoveConnectorFromGroup"
     }
 }
```

### Comparing `shikoni-0.0.1/shikoni/interfaces/ShikoniMessage.py` & `shikoni-0.0.2/shikoni/interfaces/ShikoniMessage.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/shikoni/message_types/ShikoniMessageString.py` & `shikoni-0.0.2/shikoni/message_types/ShikoniMessageString.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/shikoni/tools/PackageController.py` & `shikoni-0.0.2/shikoni/tools/PackageController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-
 import pip
-import __inti__ as base_direction
 import pathlib
 import importlib
 
 
 class PackageController:
 
     def __init__(self):
         self.molude_loaded = {}
 
     def base_package_file(self):
-        return pathlib.Path(base_direction.__file__).parent.joinpath("requieremts_base.txt")
+        return pathlib.Path().joinpath("requirements.txt")
 
     def read_package_list(self, base_requirements_file):
         return_list = []
         with open(base_requirements_file) as f:
             file_lines = f.readlines()
             for file_line in file_lines:
                 file_line = file_line.strip()
```

### Comparing `shikoni-0.0.1/shikoni/tools/ShikoniInfo.py` & `shikoni-0.0.2/shikoni/tools/ShikoniInfo.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/shikoni/tools/host_info.py` & `shikoni-0.0.2/shikoni/tools/host_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import socket
 import requests
 import json
 
-def find_free_ports(start_port=None, end_port=None, num_ports=None):
+def find_free_ports(num_ports=None):
     """Finds free ports within the given range and returns them as a list."""
     ports = []
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.bind(('localhost', 0))
-        base_port = s.getsockname()[1]
-    if start_port is None:
-        start_port = base_port
-    if end_port is None:
-        end_port = 65535
-    for port in range(start_port, end_port + 1):
+    if num_ports is None:
+        num_ports = 1
+    for port in range(num_ports):
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             try:
-                s.bind(('localhost', port))
-                ports.append(port)
+                s.bind(('localhost', 0))
+                ports.append(s.getsockname()[1])
+                s.close()
             except OSError:
                 pass
-            if num_ports is not None and len(ports) >= num_ports:
-                break
-    return ports[:num_ports] if num_ports else ports[:1]
+    return ports  # TODO port can't be used sometimes
 
 def request_free_ports(url: str, port: int, num_ports: int = 1):
     if not url.startswith("http://"):
         url = "http://{0}".format(url)
     r = requests.get(url="{0}:{1}/freeports".format(url, port), params={"num_ports": str(num_ports)})
     return json.loads(r.text)
```

### Comparing `shikoni-0.0.1/test/find_minimum_package_version.py` & `shikoni-0.0.2/test/find_minimum_package_version.py`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/test/start_test_server.py` & `shikoni-0.0.2/test/start_test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from shikoni.tools.ShikoniInfo import start_shikoni_api
 
 from shikoni.ShikoniClasses import ShikoniClasses
 from shikoni.base_messages.ShikoniMessageConnectorSocket import ShikoniMessageConnectorSocket
 
-def on_message(msg):
+def on_message(msg, shikoni):
     for key, item in msg.items():
         print(key, item)
 
 def start_base_shikoni_server(server_port: int, api_port: int):
     api_server = start_shikoni_api(api_port)
     shikoni = ShikoniClasses(default_server_call_function=on_message)
```

### Comparing `shikoni-0.0.1/test/test_base.py` & `shikoni-0.0.2/test/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pathlib
 from unittest import main, TestCase
 import time
 import subprocess
 import os
 import json
 
 from shikoni.tools.ShikoniInfo import start_shikoni_api
@@ -10,14 +11,15 @@
 
 from shikoni.ShikoniClasses import ShikoniClasses
 from shikoni.message_types.ShikoniMessageString import ShikoniMessageString
 from shikoni.base_messages.ShikoniMessageAddConnector import ShikoniMessageAddConnector
 from shikoni.base_messages.ShikoniMessageConnectorSocket import ShikoniMessageConnectorSocket
 from shikoni.base_messages.ShikoniMessageRemoveConnector import ShikoniMessageRemoveConnector
 from shikoni.base_messages.ShikoniMessageConnectorName import ShikoniMessageConnectorName
+from shikoni.base_messages.ShikoniMessageAddConnectorGroup import ShikoniMessageAddConnectorGroup
 
 output_file = "test_result.txt"
 
 if os.path.exists(output_file):
     os.remove(output_file)
 
 
@@ -156,18 +158,96 @@
             ShikoniMessageConnectorName().set_variables(True, "011"),
         ])
         connector_base_client.send_message(connector_message)
 
         connector_base_client.close_connection()
         time.sleep(2.0)
         p.kill()
+        p.terminate()
+        time.sleep(2.0)
+
+    def test_client_open_server_group_connection(self):
+        # preparing
+        test_server_ports = find_free_ports(num_ports=2)
+        server_port = test_server_ports[0]
+        api_server_port = test_server_ports[1]
+        group_name_01 = "101"
+        group_name_02 = "102"
+        control_file = pathlib.Path("server_group").joinpath("control_result.json")
+        result_file = pathlib.Path("message.json")
+
+        print(test_server_ports)
+        server_address = "127.0.0.1"
+        cmd = "python server_group/start_test_server_server_group.py {0} {1}".format(server_port, api_server_port)
+        p = subprocess.Popen(cmd, stdout=subprocess.PIPE, shell=True)
+        time.sleep(2.0)
+
+        # testing
+        shikoni = ShikoniClasses(default_server_call_function=on_message) # connect to base server
+
+        # connect to base server
+        connector_base_client = shikoni.start_client_connection(
+            ShikoniMessageConnectorSocket().set_variables(server_address, server_port, False, "001")
+        )
+
+        free_port = request_free_ports(url=server_address, port=server_port + 1, num_ports=4)
+        print(free_port)
+
+        # start first server connection group
+        connector_message = ShikoniMessageAddConnectorGroup().set_variables(
+            group_name=group_name_01,
+            connector_socket_list=[
+                ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[0], True, "010"),
+                ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[1], True, "011"),
+                # ShikoniMessageConnectorSocket().set_variables(server_address, free_port[2], False, ""),
+            ])
+        connector_base_client.send_message(connector_message)
+        print("open group connection 1")
         time.sleep(1.0)
 
+        # start second server connection group
+        connector_message = ShikoniMessageAddConnectorGroup().set_variables(
+            group_name=group_name_02,
+            connector_socket_list=[
+                ShikoniMessageConnectorSocket().set_variables(server_address, free_port[0], False, "001"),
+                ShikoniMessageConnectorSocket().set_variables(server_address, free_port[1], False, "002"),
+                ShikoniMessageConnectorSocket().set_variables("0.0.0.0", free_port[2], True, "012")
+            ])
+        connector_base_client.send_message(connector_message)
+        print("open group connection 2")
+        time.sleep(1.0)
+
+        # connect to the first new servers
+        connector_client_01 = shikoni.start_client_connection(
+            ShikoniMessageConnectorSocket().set_variables(server_address, free_port[2], False, "002")
+        )
+        connector_client_01.send_message(ShikoniMessageString("start"))
+        time.sleep(2.0)
+        connector_client_01.close_connection()
+
+        connector_base_client.close_connection()
+        time.sleep(2.0)
+        p.kill()
+        p.terminate()
+        time.sleep(2.0)
+
+        with open(control_file) as f:
+            control_json = f.read()
+        with open(result_file) as f:
+            result_json = f.read()
+
+        if control_json != result_json:
+            print(result_json)
+            raise Exception("result is wrong!!!")
+
+
+
+
 
-def on_message(msg):
+def on_message(msg, shikoni):
     for key, item in msg.items():
         if isinstance(item, ShikoniMessageString):
             print(key, item.message)
         else:
             print(key, item)
 
 if __name__ == "__main__":
```

### Comparing `shikoni-0.0.1/LICENSE` & `shikoni-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shikoni-0.0.1/pyproject.toml` & `shikoni-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "websockets>=11.0", "flask>=2.0.0", "requests>=2.19.0", "pip"]
 build-backend = "hatchling.build"
 
 [project]
 name = "shikoni"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="VG Dragon", email="vg_dragon@hotmail.com" },
 ]
 description = "Message system for connecting tools on a single or multiple Computer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `shikoni-0.0.1/PKG-INFO` & `shikoni-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-Metadata-Version: 2.1
-Name: shikoni
-Version: 0.0.1
-Summary: Message system for connecting tools on a single or multiple Computer.
-Project-URL: Github, https://github.com/VGDragon/shikoni
-Author-email: VG Dragon <vg_dragon@hotmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# shikoni
-This tool is for connection AI tools to combine them.
-
-Github: [https://github.com/VGDragon/shikoni](https://github.com/VGDragon/shikoni)
-
-## Idea
-It could take a lot of computer power for tools and AI to run. It makes sense to seperate some tools or use a entrypoint.
-The idea behind this project is to create an tool to make it easy to connect tools between computers.
-
-Example:
-
-You want to take an audio file (or microfon input) and want an AI to answer you with TTS.
-
-Audio input, AI, TTS, Audio output
-
-
-You make for each point an shikoni instance and conect them together if you need them. You take an shikoni instance and tell each point to connect to the next one.
-
-```
-Audio output: start server
-TTS: start server, connect client to "Audio output"
-AI: start server, connect client to "TTS"
-Audio input: connect client to "AI"
-
-Audio input -> AI -> TTS -> Audio output
-```
-If you want to switch the AI, you only need make an instance for that AI and keep the rest. You just have to remove the old connection and create the new one.
-
-```
-Audio input: disconnect client from "AI"
-AI: stop server, disconnect client from "TTS"
-
-AI_2: start server, connect client to "TTS"
-Audio input: connect client to "AI_2"
-
-Audio input -> AI_2 -> TTS -> Audio output
-```
-
-# Workflow
-I try to make everything as easy to use as posible but stull have important functionality. 
-The messages are send in bytes to keep it open for all kind of messages to be send. 
-To be able to know the message type, shikoni uses type_id with a combination of json to find the right Message class.
-
-It should be possible to add new message types later on.
-
-# Current status
-I am still working on the base scripts. 
-- ✅ Server Connection
-- ✅ Clinet Connection
-- ✅ start script
-- ✅ search for free ports (API)
-- ❌ forbit access for unauthorised users
-- ❌ setup script
-- ❌ make module and test it
-- ❌ test run with tools
+### Still Need testing
+Some important parts will change until everything is ready for release.
+
+# shikoni
+
+This tool is for connection AI tools to combine them.
+
+Github: [https://github.com/VGDragon/shikoni](https://github.com/VGDragon/shikoni)
+
+## Idea
+It could take a lot of computer power for tools and AI to run. It makes sense to seperate some tools or use a entrypoint.
+The idea behind this project is to create an tool to make it easy to connect tools between computers.
+
+Example:
+
+You want to take an audio file (or microfon input) and want an AI to answer you with TTS.
+
+Audio input, AI, TTS, Audio output
+
+
+You make for each point an shikoni instance and conect them together if you need them. You take an shikoni instance and tell each point to connect to the next one.
+
+```
+Audio output: start server
+TTS: start server, connect client to "Audio output"
+AI: start server, connect client to "TTS"
+Audio input: connect client to "AI"
+
+Audio input -> AI -> TTS -> Audio output
+```
+If you want to switch the AI, you only need make an instance for that AI and keep the rest. You just have to remove the old connection and create the new one.
+
+```
+Audio input: disconnect client from "AI"
+AI: stop server, disconnect client from "TTS"
+
+AI_2: start server, connect client to "TTS"
+Audio input: connect client to "AI_2"
+
+Audio input -> AI_2 -> TTS -> Audio output
+```
+
+# Workflow
+I try to make everything as easy to use as posible but stull have important functionality. 
+The messages are send in bytes to keep it open for all kind of messages to be sent. 
+To be able to know the message type, shikoni uses type_id with a combination of json to find the right Message class.
+
+It should be possible to add new message types later on.
+
+# Messages
+In [doc](https://github.com/VGDragon/shikoni/blob/main/doc) you can find a description 
+for each message that is currently implemented. 
+
+For a base structure of each message, you can look at
+[doc/message_overview.md](https://github.com/VGDragon/shikoni/blob/main/doc/message_overview.md)
+
+I want to use the listed message structure to write shikoni in other programming languages, but first I want
+to make it in python to be usable. The messages stricture should be the same for each language, to make a 
+connection between all instances possible.
+
+# Task before release
+Some important parts can change until I am sure everything important is added.
+
+I need some testing with different tools before I can make a real release.
+
+# Current status
+I am still working on the base scripts. 
+- ✅ Server Connection
+- ✅ Client Connection
+- ✅ start script
+- ✅ search for free ports (API)
+- ✅ forbid access for unauthorised users (using path)
+- ❌ setup script
+- ❌ make module and test it
+- ✅ test run with tools
```

