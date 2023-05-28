# Comparing `tmp/meshtastic-2.1.6.tar.gz` & `tmp/meshtastic-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.1.6.tar", last modified: Tue Apr 11 15:06:19 2023, max compression
+gzip compressed data, was "meshtastic-2.1.7.tar", last modified: Sun May 28 14:34:01 2023, max compression
```

## Comparing `meshtastic-2.1.6.tar` & `meshtastic-2.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 15:06:05.000000 meshtastic-2.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 15:06:05.000000 meshtastic-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 15:06:19.637641 meshtastic-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-11 15:06:05.000000 meshtastic-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/device_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/xmodem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:06:19.637641 meshtastic-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-11 15:06:05.000000 meshtastic-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.295622 meshtastic-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-28 14:33:46.000000 meshtastic-2.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 14:33:46.000000 meshtastic-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 14:34:01.295622 meshtastic-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-28 14:33:46.000000 meshtastic-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.291622 meshtastic-2.1.7/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/device_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/xmodem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.295622 meshtastic-2.1.7/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:34:01.295622 meshtastic-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-28 14:33:46.000000 meshtastic-2.1.7/setup.py
```

### Comparing `meshtastic-2.1.6/LICENSE.txt` & `meshtastic-2.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/PKG-INFO` & `meshtastic-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.6/README.md` & `meshtastic-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/__init__.py` & `meshtastic-2.1.7/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/__main__.py` & `meshtastic-2.1.7/meshtastic/__main__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/admin_pb2.py` & `meshtastic-2.1.7/meshtastic/admin_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
+from meshtastic import connection_status_pb2 as meshtastic_dot_connection__status__pb2
+from meshtastic import deviceonly_pb2 as meshtastic_dot_deviceonly__pb2
 from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
-from meshtastic import connection_status_pb2 as meshtastic_dot_connection__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/admin.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\x1a\"meshtastic/connection_status.proto\"\xd8\x0c\n\x0c\x41\x64minMessage\x12\x1d\n\x13get_channel_request\x18\x01 \x01(\rH\x00\x12(\n\x14get_channel_response\x18\x02 \x01(\x0b\x32\x08.ChannelH\x00\x12\x1b\n\x11get_owner_request\x18\x03 \x01(\x08H\x00\x12#\n\x12get_owner_response\x18\x04 \x01(\x0b\x32\x05.UserH\x00\x12\x36\n\x12get_config_request\x18\x05 \x01(\x0e\x32\x18.AdminMessage.ConfigTypeH\x00\x12&\n\x13get_config_response\x18\x06 \x01(\x0b\x32\x07.ConfigH\x00\x12\x43\n\x19get_module_config_request\x18\x07 \x01(\x0e\x32\x1e.AdminMessage.ModuleConfigTypeH\x00\x12\x33\n\x1aget_module_config_response\x18\x08 \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x34\n*get_canned_message_module_messages_request\x18\n \x01(\x08H\x00\x12\x35\n+get_canned_message_module_messages_response\x18\x0b \x01(\tH\x00\x12%\n\x1bget_device_metadata_request\x18\x0c \x01(\x08H\x00\x12\x37\n\x1cget_device_metadata_response\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x12\x1e\n\x14get_ringtone_request\x18\x0e \x01(\x08H\x00\x12\x1f\n\x15get_ringtone_response\x18\x0f \x01(\tH\x00\x12.\n$get_device_connection_status_request\x18\x10 \x01(\x08H\x00\x12H\n%get_device_connection_status_response\x18\x11 \x01(\x0b\x32\x17.DeviceConnectionStatusH\x00\x12&\n\x0cset_ham_mode\x18\x12 \x01(\x0b\x32\x0e.HamParametersH\x00\x12\x1a\n\tset_owner\x18  \x01(\x0b\x32\x05.UserH\x00\x12\x1f\n\x0bset_channel\x18! \x01(\x0b\x32\x08.ChannelH\x00\x12\x1d\n\nset_config\x18\" \x01(\x0b\x32\x07.ConfigH\x00\x12*\n\x11set_module_config\x18# \x01(\x0b\x32\r.ModuleConfigH\x00\x12,\n\"set_canned_message_module_messages\x18$ \x01(\tH\x00\x12\x1e\n\x14set_ringtone_message\x18% \x01(\tH\x00\x12\x1d\n\x13\x62\x65gin_edit_settings\x18@ \x01(\x08H\x00\x12\x1e\n\x14\x63ommit_edit_settings\x18\x41 \x01(\x08H\x00\x12\x1c\n\x12reboot_ota_seconds\x18_ \x01(\x05H\x00\x12\x18\n\x0e\x65xit_simulator\x18` \x01(\x08H\x00\x12\x18\n\x0ereboot_seconds\x18\x61 \x01(\x05H\x00\x12\x1a\n\x10shutdown_seconds\x18\x62 \x01(\x05H\x00\x12\x17\n\rfactory_reset\x18\x63 \x01(\x05H\x00\x12\x16\n\x0cnodedb_reset\x18\x64 \x01(\x05H\x00\"\x95\x01\n\nConfigType\x12\x11\n\rDEVICE_CONFIG\x10\x00\x12\x13\n\x0fPOSITION_CONFIG\x10\x01\x12\x10\n\x0cPOWER_CONFIG\x10\x02\x12\x12\n\x0eNETWORK_CONFIG\x10\x03\x12\x12\n\x0e\x44ISPLAY_CONFIG\x10\x04\x12\x0f\n\x0bLORA_CONFIG\x10\x05\x12\x14\n\x10\x42LUETOOTH_CONFIG\x10\x06\"\xd3\x01\n\x10ModuleConfigType\x12\x0f\n\x0bMQTT_CONFIG\x10\x00\x12\x11\n\rSERIAL_CONFIG\x10\x01\x12\x13\n\x0f\x45XTNOTIF_CONFIG\x10\x02\x12\x17\n\x13STOREFORWARD_CONFIG\x10\x03\x12\x14\n\x10RANGETEST_CONFIG\x10\x04\x12\x14\n\x10TELEMETRY_CONFIG\x10\x05\x12\x14\n\x10\x43\x41NNEDMSG_CONFIG\x10\x06\x12\x10\n\x0c\x41UDIO_CONFIG\x10\x07\x12\x19\n\x15REMOTEHARDWARE_CONFIG\x10\x08\x42\x11\n\x0fpayload_variant\"[\n\rHamParameters\x12\x11\n\tcall_sign\x18\x01 \x01(\t\x12\x10\n\x08tx_power\x18\x02 \x01(\x05\x12\x11\n\tfrequency\x18\x03 \x01(\x02\x12\x12\n\nshort_name\x18\x04 \x01(\tB`\n\x13\x63om.geeksville.meshB\x0b\x41\x64minProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16meshtastic/admin.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\"meshtastic/connection_status.proto\x1a\x1bmeshtastic/deviceonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\"\xdc\r\n\x0c\x41\x64minMessage\x12\x1d\n\x13get_channel_request\x18\x01 \x01(\rH\x00\x12(\n\x14get_channel_response\x18\x02 \x01(\x0b\x32\x08.ChannelH\x00\x12\x1b\n\x11get_owner_request\x18\x03 \x01(\x08H\x00\x12#\n\x12get_owner_response\x18\x04 \x01(\x0b\x32\x05.UserH\x00\x12\x36\n\x12get_config_request\x18\x05 \x01(\x0e\x32\x18.AdminMessage.ConfigTypeH\x00\x12&\n\x13get_config_response\x18\x06 \x01(\x0b\x32\x07.ConfigH\x00\x12\x43\n\x19get_module_config_request\x18\x07 \x01(\x0e\x32\x1e.AdminMessage.ModuleConfigTypeH\x00\x12\x33\n\x1aget_module_config_response\x18\x08 \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x34\n*get_canned_message_module_messages_request\x18\n \x01(\x08H\x00\x12\x35\n+get_canned_message_module_messages_response\x18\x0b \x01(\tH\x00\x12%\n\x1bget_device_metadata_request\x18\x0c \x01(\x08H\x00\x12\x37\n\x1cget_device_metadata_response\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x12\x1e\n\x14get_ringtone_request\x18\x0e \x01(\x08H\x00\x12\x1f\n\x15get_ringtone_response\x18\x0f \x01(\tH\x00\x12.\n$get_device_connection_status_request\x18\x10 \x01(\x08H\x00\x12H\n%get_device_connection_status_response\x18\x11 \x01(\x0b\x32\x17.DeviceConnectionStatusH\x00\x12&\n\x0cset_ham_mode\x18\x12 \x01(\x0b\x32\x0e.HamParametersH\x00\x12/\n%get_node_remote_hardware_pins_request\x18\x13 \x01(\x08H\x00\x12Q\n&get_node_remote_hardware_pins_response\x18\x14 \x01(\x0b\x32\x1f.NodeRemoteHardwarePinsResponseH\x00\x12\x1a\n\tset_owner\x18  \x01(\x0b\x32\x05.UserH\x00\x12\x1f\n\x0bset_channel\x18! \x01(\x0b\x32\x08.ChannelH\x00\x12\x1d\n\nset_config\x18\" \x01(\x0b\x32\x07.ConfigH\x00\x12*\n\x11set_module_config\x18# \x01(\x0b\x32\r.ModuleConfigH\x00\x12,\n\"set_canned_message_module_messages\x18$ \x01(\tH\x00\x12\x1e\n\x14set_ringtone_message\x18% \x01(\tH\x00\x12\x1d\n\x13\x62\x65gin_edit_settings\x18@ \x01(\x08H\x00\x12\x1e\n\x14\x63ommit_edit_settings\x18\x41 \x01(\x08H\x00\x12\x1c\n\x12reboot_ota_seconds\x18_ \x01(\x05H\x00\x12\x18\n\x0e\x65xit_simulator\x18` \x01(\x08H\x00\x12\x18\n\x0ereboot_seconds\x18\x61 \x01(\x05H\x00\x12\x1a\n\x10shutdown_seconds\x18\x62 \x01(\x05H\x00\x12\x17\n\rfactory_reset\x18\x63 \x01(\x05H\x00\x12\x16\n\x0cnodedb_reset\x18\x64 \x01(\x05H\x00\"\x95\x01\n\nConfigType\x12\x11\n\rDEVICE_CONFIG\x10\x00\x12\x13\n\x0fPOSITION_CONFIG\x10\x01\x12\x10\n\x0cPOWER_CONFIG\x10\x02\x12\x12\n\x0eNETWORK_CONFIG\x10\x03\x12\x12\n\x0e\x44ISPLAY_CONFIG\x10\x04\x12\x0f\n\x0bLORA_CONFIG\x10\x05\x12\x14\n\x10\x42LUETOOTH_CONFIG\x10\x06\"\xd3\x01\n\x10ModuleConfigType\x12\x0f\n\x0bMQTT_CONFIG\x10\x00\x12\x11\n\rSERIAL_CONFIG\x10\x01\x12\x13\n\x0f\x45XTNOTIF_CONFIG\x10\x02\x12\x17\n\x13STOREFORWARD_CONFIG\x10\x03\x12\x14\n\x10RANGETEST_CONFIG\x10\x04\x12\x14\n\x10TELEMETRY_CONFIG\x10\x05\x12\x14\n\x10\x43\x41NNEDMSG_CONFIG\x10\x06\x12\x10\n\x0c\x41UDIO_CONFIG\x10\x07\x12\x19\n\x15REMOTEHARDWARE_CONFIG\x10\x08\x42\x11\n\x0fpayload_variant\"[\n\rHamParameters\x12\x11\n\tcall_sign\x18\x01 \x01(\t\x12\x10\n\x08tx_power\x18\x02 \x01(\x05\x12\x11\n\tfrequency\x18\x03 \x01(\x02\x12\x12\n\nshort_name\x18\x04 \x01(\t\"[\n\x1eNodeRemoteHardwarePinsResponse\x12\x39\n\x19node_remote_hardware_pins\x18\x01 \x03(\x0b\x32\x16.NodeRemoteHardwarePinB`\n\x13\x63om.geeksville.meshB\x0b\x41\x64minProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 
 
 _ADMINMESSAGE = DESCRIPTOR.message_types_by_name['AdminMessage']
 _HAMPARAMETERS = DESCRIPTOR.message_types_by_name['HamParameters']
+_NODEREMOTEHARDWAREPINSRESPONSE = DESCRIPTOR.message_types_by_name['NodeRemoteHardwarePinsResponse']
 _ADMINMESSAGE_CONFIGTYPE = _ADMINMESSAGE.enum_types_by_name['ConfigType']
 _ADMINMESSAGE_MODULECONFIGTYPE = _ADMINMESSAGE.enum_types_by_name['ModuleConfigType']
 AdminMessage = _reflection.GeneratedProtocolMessageType('AdminMessage', (_message.Message,), {
   'DESCRIPTOR' : _ADMINMESSAGE,
   '__module__' : 'meshtastic.admin_pb2'
   # @@protoc_insertion_point(class_scope:AdminMessage)
   })
@@ -37,20 +39,29 @@
 HamParameters = _reflection.GeneratedProtocolMessageType('HamParameters', (_message.Message,), {
   'DESCRIPTOR' : _HAMPARAMETERS,
   '__module__' : 'meshtastic.admin_pb2'
   # @@protoc_insertion_point(class_scope:HamParameters)
   })
 _sym_db.RegisterMessage(HamParameters)
 
+NodeRemoteHardwarePinsResponse = _reflection.GeneratedProtocolMessageType('NodeRemoteHardwarePinsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _NODEREMOTEHARDWAREPINSRESPONSE,
+  '__module__' : 'meshtastic.admin_pb2'
+  # @@protoc_insertion_point(class_scope:NodeRemoteHardwarePinsResponse)
+  })
+_sym_db.RegisterMessage(NodeRemoteHardwarePinsResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\013AdminProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _ADMINMESSAGE._serialized_start=169
-  _ADMINMESSAGE._serialized_end=1793
-  _ADMINMESSAGE_CONFIGTYPE._serialized_start=1411
-  _ADMINMESSAGE_CONFIGTYPE._serialized_end=1560
-  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_start=1563
-  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_end=1774
-  _HAMPARAMETERS._serialized_start=1795
-  _HAMPARAMETERS._serialized_end=1886
+  _ADMINMESSAGE._serialized_start=198
+  _ADMINMESSAGE._serialized_end=1954
+  _ADMINMESSAGE_CONFIGTYPE._serialized_start=1572
+  _ADMINMESSAGE_CONFIGTYPE._serialized_end=1721
+  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_start=1724
+  _ADMINMESSAGE_MODULECONFIGTYPE._serialized_end=1935
+  _HAMPARAMETERS._serialized_start=1956
+  _HAMPARAMETERS._serialized_end=2047
+  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_start=2049
+  _NODEREMOTEHARDWAREPINSRESPONSE._serialized_end=2140
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/apponly_pb2.py` & `meshtastic-2.1.7/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/ble_interface.py` & `meshtastic-2.1.7/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.1.7/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/channel_pb2.py` & `meshtastic-2.1.7/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/clientonly_pb2.py` & `meshtastic-2.1.7/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/config_pb2.py` & `meshtastic-2.1.7/meshtastic/config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\"\xfa\x1a\n\x06\x43onfig\x12&\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfigH\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfigH\x00\x12$\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfigH\x00\x12(\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfigH\x00\x12(\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfigH\x00\x12\"\n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfigH\x00\x12,\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfigH\x00\x1a\xc8\x03\n\x0c\x44\x65viceConfig\x12\'\n\x04role\x18\x01 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12>\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32$.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\"i\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\"A\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x1a\x80\x04\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x13\n\x0bgps_enabled\x18\x04 \x01(\x08\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x18\n\x10gps_attempt_time\x18\x06 \x01(\r\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\x1a\xe5\x01\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x1d\n\x15mesh_sds_timeout_secs\x18\x05 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x1a\xe8\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x37\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32!.Config.NetworkConfig.AddressMode\x12\x35\n\x0bipv4_config\x18\x08 \x01(\x0b\x32 .Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\x92\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12=\n\ngps_format\x18\x02 \x01(\x0e\x32).Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12\x31\n\x05units\x18\x06 \x01(\x0e\x32\".Config.DisplayConfig.DisplayUnits\x12,\n\x04oled\x18\x07 \x01(\x0e\x32\x1e.Config.DisplayConfig.OledType\x12\x36\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32!.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\xe1\x05\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12\x34\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12-\n\x06region\x18\x07 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\"\xa9\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xa2\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x31\n\x04mode\x18\x02 \x01(\x0e\x32#.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\"\x8e\x1b\n\x06\x43onfig\x12&\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfigH\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfigH\x00\x12$\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfigH\x00\x12(\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfigH\x00\x12(\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfigH\x00\x12\"\n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfigH\x00\x12,\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfigH\x00\x1a\xdc\x03\n\x0c\x44\x65viceConfig\x12\'\n\x04role\x18\x01 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12>\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32$.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\x12\x12\n\nis_managed\x18\t \x01(\x08\"i\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\"A\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x1a\x80\x04\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x13\n\x0bgps_enabled\x18\x04 \x01(\x08\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x18\n\x10gps_attempt_time\x18\x06 \x01(\r\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\x1a\xe5\x01\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x1d\n\x15mesh_sds_timeout_secs\x18\x05 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x1a\xe8\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x37\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32!.Config.NetworkConfig.AddressMode\x12\x35\n\x0bipv4_config\x18\x08 \x01(\x0b\x32 .Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\x92\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12=\n\ngps_format\x18\x02 \x01(\x0e\x32).Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12\x31\n\x05units\x18\x06 \x01(\x0e\x32\".Config.DisplayConfig.DisplayUnits\x12,\n\x04oled\x18\x07 \x01(\x0e\x32\x1e.Config.DisplayConfig.OledType\x12\x36\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32!.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\xe1\x05\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12\x34\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12-\n\x06region\x18\x07 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\"\xa9\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xa2\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x31\n\x04mode\x18\x02 \x01(\x0e\x32#.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 
 
 _CONFIG = DESCRIPTOR.message_types_by_name['Config']
 _CONFIG_DEVICECONFIG = _CONFIG.nested_types_by_name['DeviceConfig']
 _CONFIG_POSITIONCONFIG = _CONFIG.nested_types_by_name['PositionConfig']
 _CONFIG_POWERCONFIG = _CONFIG.nested_types_by_name['PowerConfig']
@@ -110,47 +110,47 @@
 _sym_db.RegisterMessage(Config.BluetoothConfig)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\014ConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _CONFIG._serialized_start=28
-  _CONFIG._serialized_end=3478
+  _CONFIG._serialized_end=3498
   _CONFIG_DEVICECONFIG._serialized_start=327
-  _CONFIG_DEVICECONFIG._serialized_end=783
-  _CONFIG_DEVICECONFIG_ROLE._serialized_start=611
-  _CONFIG_DEVICECONFIG_ROLE._serialized_end=716
-  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_start=718
-  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_end=783
-  _CONFIG_POSITIONCONFIG._serialized_start=786
-  _CONFIG_POSITIONCONFIG._serialized_end=1298
-  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_start=1127
-  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_end=1298
-  _CONFIG_POWERCONFIG._serialized_start=1301
-  _CONFIG_POWERCONFIG._serialized_end=1530
-  _CONFIG_NETWORKCONFIG._serialized_start=1533
-  _CONFIG_NETWORKCONFIG._serialized_end=1893
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=1786
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=1856
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=1858
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=1893
-  _CONFIG_DISPLAYCONFIG._serialized_start=1896
-  _CONFIG_DISPLAYCONFIG._serialized_end=2554
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2289
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2366
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2368
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2408
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2410
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2487
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2489
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=2554
-  _CONFIG_LORACONFIG._serialized_start=2557
-  _CONFIG_LORACONFIG._serialized_end=3294
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=2974
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3143
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3146
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3294
-  _CONFIG_BLUETOOTHCONFIG._serialized_start=3297
-  _CONFIG_BLUETOOTHCONFIG._serialized_end=3459
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3403
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=3459
+  _CONFIG_DEVICECONFIG._serialized_end=803
+  _CONFIG_DEVICECONFIG_ROLE._serialized_start=631
+  _CONFIG_DEVICECONFIG_ROLE._serialized_end=736
+  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_start=738
+  _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_end=803
+  _CONFIG_POSITIONCONFIG._serialized_start=806
+  _CONFIG_POSITIONCONFIG._serialized_end=1318
+  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_start=1147
+  _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_end=1318
+  _CONFIG_POWERCONFIG._serialized_start=1321
+  _CONFIG_POWERCONFIG._serialized_end=1550
+  _CONFIG_NETWORKCONFIG._serialized_start=1553
+  _CONFIG_NETWORKCONFIG._serialized_end=1913
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=1806
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=1876
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=1878
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=1913
+  _CONFIG_DISPLAYCONFIG._serialized_start=1916
+  _CONFIG_DISPLAYCONFIG._serialized_end=2574
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2309
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2386
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2388
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2428
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2430
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2507
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2509
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=2574
+  _CONFIG_LORACONFIG._serialized_start=2577
+  _CONFIG_LORACONFIG._serialized_end=3314
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=2994
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3163
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3166
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3314
+  _CONFIG_BLUETOOTHCONFIG._serialized_start=3317
+  _CONFIG_BLUETOOTHCONFIG._serialized_end=3479
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3423
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=3479
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/connection_status_pb2.py` & `meshtastic-2.1.7/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/device_metadata_pb2.py` & `meshtastic-2.1.7/meshtastic/device_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/deviceonly_pb2.py` & `meshtastic-2.1.7/meshtastic/deviceonly_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import localonly_pb2 as meshtastic_dot_localonly__pb2
 from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
+from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\"\xe0\x01\n\x0b\x44\x65viceState\x12\x1c\n\x07my_node\x18\x02 \x01(\x0b\x32\x0b.MyNodeInfo\x12\x14\n\x05owner\x18\x03 \x01(\x0b\x32\x05.User\x12\x1a\n\x07node_db\x18\x04 \x03(\x0b\x32\t.NodeInfo\x12\"\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12$\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07no_save\x18\t \x01(\x08\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\":\n\x0b\x43hannelFile\x12\x1a\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x08.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\xf6\x01\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12\x1e\n\x08oem_font\x18\x04 \x01(\x0e\x32\x0c.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12&\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x0c.LocalConfig\x12\x33\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x12.LocalModuleConfig*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42_\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\"\xbd\x02\n\x0b\x44\x65viceState\x12\x1c\n\x07my_node\x18\x02 \x01(\x0b\x32\x0b.MyNodeInfo\x12\x14\n\x05owner\x18\x03 \x01(\x0b\x32\x05.User\x12\x1a\n\x07node_db\x18\x04 \x03(\x0b\x32\t.NodeInfo\x12\"\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12$\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07no_save\x18\t \x01(\x08\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\x12 \n\x0brx_waypoint\x18\x0c \x01(\x0b\x32\x0b.MeshPacket\x12\x39\n\x19node_remote_hardware_pins\x18\r \x03(\x0b\x32\x16.NodeRemoteHardwarePin\":\n\x0b\x43hannelFile\x12\x1a\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x08.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\xf6\x01\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12\x1e\n\x08oem_font\x18\x04 \x01(\x0e\x32\x0c.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12&\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x0c.LocalConfig\x12\x33\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x12.LocalModuleConfig\"J\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12\x1f\n\x03pin\x18\x02 \x01(\x0b\x32\x12.RemoteHardwarePin*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42_\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _SCREENFONTS = DESCRIPTOR.enum_types_by_name['ScreenFonts']
 ScreenFonts = enum_type_wrapper.EnumTypeWrapper(_SCREENFONTS)
 FONT_SMALL = 0
 FONT_MEDIUM = 1
 FONT_LARGE = 2
 
 
 _DEVICESTATE = DESCRIPTOR.message_types_by_name['DeviceState']
 _CHANNELFILE = DESCRIPTOR.message_types_by_name['ChannelFile']
 _OEMSTORE = DESCRIPTOR.message_types_by_name['OEMStore']
+_NODEREMOTEHARDWAREPIN = DESCRIPTOR.message_types_by_name['NodeRemoteHardwarePin']
 DeviceState = _reflection.GeneratedProtocolMessageType('DeviceState', (_message.Message,), {
   'DESCRIPTOR' : _DEVICESTATE,
   '__module__' : 'meshtastic.deviceonly_pb2'
   # @@protoc_insertion_point(class_scope:DeviceState)
   })
 _sym_db.RegisterMessage(DeviceState)
 
@@ -47,20 +49,29 @@
 OEMStore = _reflection.GeneratedProtocolMessageType('OEMStore', (_message.Message,), {
   'DESCRIPTOR' : _OEMSTORE,
   '__module__' : 'meshtastic.deviceonly_pb2'
   # @@protoc_insertion_point(class_scope:OEMStore)
   })
 _sym_db.RegisterMessage(OEMStore)
 
+NodeRemoteHardwarePin = _reflection.GeneratedProtocolMessageType('NodeRemoteHardwarePin', (_message.Message,), {
+  'DESCRIPTOR' : _NODEREMOTEHARDWAREPIN,
+  '__module__' : 'meshtastic.deviceonly_pb2'
+  # @@protoc_insertion_point(class_scope:NodeRemoteHardwarePin)
+  })
+_sym_db.RegisterMessage(NodeRemoteHardwarePin)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _SCREENFONTS._serialized_start=644
-  _SCREENFONTS._serialized_end=706
-  _DEVICESTATE._serialized_start=109
-  _DEVICESTATE._serialized_end=333
-  _CHANNELFILE._serialized_start=335
-  _CHANNELFILE._serialized_end=393
-  _OEMSTORE._serialized_start=396
-  _OEMSTORE._serialized_end=642
+  _SCREENFONTS._serialized_start=845
+  _SCREENFONTS._serialized_end=907
+  _DEVICESTATE._serialized_start=141
+  _DEVICESTATE._serialized_end=458
+  _CHANNELFILE._serialized_start=460
+  _CHANNELFILE._serialized_end=518
+  _OEMSTORE._serialized_start=521
+  _OEMSTORE._serialized_end=767
+  _NODEREMOTEHARDWAREPIN._serialized_start=769
+  _NODEREMOTEHARDWAREPIN._serialized_end=843
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/globals.py` & `meshtastic-2.1.7/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/localonly_pb2.py` & `meshtastic-2.1.7/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/mesh_interface.py` & `meshtastic-2.1.7/meshtastic/mesh_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -894,66 +894,66 @@
             logging.warning(f"Not populating toId {ex}")
 
         # We could provide our objects as DotMaps - which work with . notation or as dictionaries
         # asObj = DotMap(asDict)
         topic = "meshtastic.receive"  # Generic unknown packet type
 
         decoded = None
+        portnum = portnums_pb2.PortNum.Name(portnums_pb2.PortNum.UNKNOWN_APP)
         if "decoded" in asDict:
             decoded = asDict["decoded"]
             # The default MessageToDict converts byte arrays into base64 strings.
             # We don't want that - it messes up data payload.  So slam in the correct
             # byte array.
             decoded["payload"] = meshPacket.decoded.payload
 
-        # UNKNOWN_APP is the default protobuf portnum value, and therefore if not
-        # set it will not be populated at all to make API usage easier, set
-        # it to prevent confusion
-        if decoded and "portnum" not in decoded:
-            new_portnum = portnums_pb2.PortNum.Name(portnums_pb2.PortNum.UNKNOWN_APP)
-            decoded["portnum"] = new_portnum
-            logging.warning(f"portnum was not in decoded. Setting to:{new_portnum}")
-
-        portnum = decoded["portnum"]
-
-        topic = f"meshtastic.receive.data.{portnum}"
-
-        # decode position protobufs and update nodedb, provide decoded version
-        # as "position" in the published msg move the following into a 'decoders'
-        # API that clients could register?
-        portNumInt = meshPacket.decoded.portnum  # we want portnum as an int
-        handler = protocols.get(portNumInt)
-        # The decoded protobuf as a dictionary (if we understand this message)
-        p = None
-        if handler is not None:
-            topic = f"meshtastic.receive.{handler.name}"
-
-            # Convert to protobuf if possible
-            if handler.protobufFactory is not None:
-                pb = handler.protobufFactory()
-                pb.ParseFromString(meshPacket.decoded.payload)
-                p = google.protobuf.json_format.MessageToDict(pb)
-                asDict["decoded"][handler.name] = p
-                # Also provide the protobuf raw
-                asDict["decoded"][handler.name]["raw"] = pb
-
-            # Call specialized onReceive if necessary
-            if handler.onReceive is not None:
-                handler.onReceive(self, asDict)
-
-        # Is this message in response to a request, if so, look for a handler
-        requestId = decoded.get("requestId")
-        if requestId is not None:
-            # We ignore ACK packets, but send NAKs and data responses to the handlers
-            routing = decoded.get("routing")
-            isAck = routing is not None and ("errorReason" not in routing)
-            if not isAck:
-                # we keep the responseHandler in dict until we get a non ack
-                handler = self.responseHandlers.pop(requestId, None)
-                if handler is not None:
-                    if not isAck or (isAck and handler.__name__ == "onAckNak"):
-                        handler.callback(asDict)
+            # UNKNOWN_APP is the default protobuf portnum value, and therefore if not
+            # set it will not be populated at all to make API usage easier, set
+            # it to prevent confusion
+            if "portnum" not in decoded:
+                decoded["portnum"] = portnum
+                logging.warning(f"portnum was not in decoded. Setting to:{portnum}")
+            else:
+                portnum = decoded["portnum"]
+
+            topic = f"meshtastic.receive.data.{portnum}"
+
+            # decode position protobufs and update nodedb, provide decoded version
+            # as "position" in the published msg move the following into a 'decoders'
+            # API that clients could register?
+            portNumInt = meshPacket.decoded.portnum  # we want portnum as an int
+            handler = protocols.get(portNumInt)
+            # The decoded protobuf as a dictionary (if we understand this message)
+            p = None
+            if handler is not None:
+                topic = f"meshtastic.receive.{handler.name}"
+
+                # Convert to protobuf if possible
+                if handler.protobufFactory is not None:
+                    pb = handler.protobufFactory()
+                    pb.ParseFromString(meshPacket.decoded.payload)
+                    p = google.protobuf.json_format.MessageToDict(pb)
+                    asDict["decoded"][handler.name] = p
+                    # Also provide the protobuf raw
+                    asDict["decoded"][handler.name]["raw"] = pb
+
+                # Call specialized onReceive if necessary
+                if handler.onReceive is not None:
+                    handler.onReceive(self, asDict)
+
+            # Is this message in response to a request, if so, look for a handler
+            requestId = decoded.get("requestId")
+            if requestId is not None:
+                # We ignore ACK packets, but send NAKs and data responses to the handlers
+                routing = decoded.get("routing")
+                isAck = routing is not None and ("errorReason" not in routing)
+                if not isAck:
+                    # we keep the responseHandler in dict until we get a non ack
+                    handler = self.responseHandlers.pop(requestId, None)
+                    if handler is not None:
+                        if not isAck or (isAck and handler.__name__ == "onAckNak"):
+                            handler.callback(asDict)
 
         logging.debug(f"Publishing {topic}: packet={stripnl(asDict)} ")
         publishingThread.queueWork(
             lambda: pub.sendMessage(topic, packet=asDict, interface=self)
         )
```

### Comparing `meshtastic-2.1.6/meshtastic/mesh_pb2.py` & `meshtastic-2.1.7/meshtastic/mesh_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x81\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x0f\n\x07macaddr\x18\x04 \x01(\x0c\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x86\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x0f\n\x07has_gps\x18\x02 \x01(\x08\x12\x14\n\x0cmax_channels\x18\x03 \x01(\r\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12&\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCode\x12\x15\n\rerror_address\x18\x06 \x01(\r\x12\x13\n\x0b\x65rror_count\x18\x07 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x0f\n\x07\x62itrate\x18\t \x01(\x02\x12\x1c\n\x14message_timeout_msec\x18\n \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x15\n\rair_period_tx\x18\x0c \x03(\r\x12\x15\n\rair_period_rx\x18\r \x03(\r\x12\x10\n\x08has_wifi\x18\x0e \x01(\x08\x12\x1b\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\xfc\x01\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel*\xce\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x81\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x0f\n\x07macaddr\x18\x04 \x01(\x0c\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x86\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x0f\n\x07has_gps\x18\x02 \x01(\x08\x12\x14\n\x0cmax_channels\x18\x03 \x01(\r\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12&\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCode\x12\x15\n\rerror_address\x18\x06 \x01(\r\x12\x13\n\x0b\x65rror_count\x18\x07 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x0f\n\x07\x62itrate\x18\t \x01(\x02\x12\x1c\n\x14message_timeout_msec\x18\n \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x15\n\rair_period_tx\x18\x0c \x03(\r\x12\x15\n\rair_period_rx\x18\r \x03(\r\x12\x10\n\x08has_wifi\x18\x0e \x01(\x08\x12\x1b\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"V\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12\x1c\n\tneighbors\x18\x03 \x03(\x0b\x32\t.Neighbor\"(\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08*\xce\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _HARDWAREMODEL = DESCRIPTOR.enum_types_by_name['HardwareModel']
 HardwareModel = enum_type_wrapper.EnumTypeWrapper(_HARDWAREMODEL)
 _CONSTANTS = DESCRIPTOR.enum_types_by_name['Constants']
 Constants = enum_type_wrapper.EnumTypeWrapper(_CONSTANTS)
 _CRITICALERRORCODE = DESCRIPTOR.enum_types_by_name['CriticalErrorCode']
 CriticalErrorCode = enum_type_wrapper.EnumTypeWrapper(_CRITICALERRORCODE)
@@ -90,14 +90,16 @@
 _NODEINFO = DESCRIPTOR.message_types_by_name['NodeInfo']
 _MYNODEINFO = DESCRIPTOR.message_types_by_name['MyNodeInfo']
 _LOGRECORD = DESCRIPTOR.message_types_by_name['LogRecord']
 _QUEUESTATUS = DESCRIPTOR.message_types_by_name['QueueStatus']
 _FROMRADIO = DESCRIPTOR.message_types_by_name['FromRadio']
 _TORADIO = DESCRIPTOR.message_types_by_name['ToRadio']
 _COMPRESSED = DESCRIPTOR.message_types_by_name['Compressed']
+_NEIGHBORINFO = DESCRIPTOR.message_types_by_name['NeighborInfo']
+_NEIGHBOR = DESCRIPTOR.message_types_by_name['Neighbor']
 _DEVICEMETADATA = DESCRIPTOR.message_types_by_name['DeviceMetadata']
 _POSITION_LOCSOURCE = _POSITION.enum_types_by_name['LocSource']
 _POSITION_ALTSOURCE = _POSITION.enum_types_by_name['AltSource']
 _ROUTING_ERROR = _ROUTING.enum_types_by_name['Error']
 _MESHPACKET_PRIORITY = _MESHPACKET.enum_types_by_name['Priority']
 _MESHPACKET_DELAYED = _MESHPACKET.enum_types_by_name['Delayed']
 _LOGRECORD_LEVEL = _LOGRECORD.enum_types_by_name['Level']
@@ -195,31 +197,45 @@
 Compressed = _reflection.GeneratedProtocolMessageType('Compressed', (_message.Message,), {
   'DESCRIPTOR' : _COMPRESSED,
   '__module__' : 'meshtastic.mesh_pb2'
   # @@protoc_insertion_point(class_scope:Compressed)
   })
 _sym_db.RegisterMessage(Compressed)
 
+NeighborInfo = _reflection.GeneratedProtocolMessageType('NeighborInfo', (_message.Message,), {
+  'DESCRIPTOR' : _NEIGHBORINFO,
+  '__module__' : 'meshtastic.mesh_pb2'
+  # @@protoc_insertion_point(class_scope:NeighborInfo)
+  })
+_sym_db.RegisterMessage(NeighborInfo)
+
+Neighbor = _reflection.GeneratedProtocolMessageType('Neighbor', (_message.Message,), {
+  'DESCRIPTOR' : _NEIGHBOR,
+  '__module__' : 'meshtastic.mesh_pb2'
+  # @@protoc_insertion_point(class_scope:Neighbor)
+  })
+_sym_db.RegisterMessage(Neighbor)
+
 DeviceMetadata = _reflection.GeneratedProtocolMessageType('DeviceMetadata', (_message.Message,), {
   'DESCRIPTOR' : _DEVICEMETADATA,
   '__module__' : 'meshtastic.mesh_pb2'
   # @@protoc_insertion_point(class_scope:DeviceMetadata)
   })
 _sym_db.RegisterMessage(DeviceMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _HARDWAREMODEL._serialized_start=3877
-  _HARDWAREMODEL._serialized_end=4467
-  _CONSTANTS._serialized_start=4469
-  _CONSTANTS._serialized_end=4513
-  _CRITICALERRORCODE._serialized_start=4516
-  _CRITICALERRORCODE._serialized_end=4754
+  _HARDWAREMODEL._serialized_start=4034
+  _HARDWAREMODEL._serialized_end=4624
+  _CONSTANTS._serialized_start=4626
+  _CONSTANTS._serialized_end=4670
+  _CRITICALERRORCODE._serialized_start=4673
+  _CRITICALERRORCODE._serialized_end=4911
   _POSITION._serialized_start=189
   _POSITION._serialized_end=884
   _POSITION_LOCSOURCE._serialized_start=706
   _POSITION_LOCSOURCE._serialized_end=784
   _POSITION_ALTSOURCE._serialized_start=786
   _POSITION_ALTSOURCE._serialized_end=884
   _USER._serialized_start=887
@@ -252,10 +268,14 @@
   _QUEUESTATUS._serialized_end=2995
   _FROMRADIO._serialized_start=2998
   _FROMRADIO._serialized_end=3421
   _TORADIO._serialized_start=3424
   _TORADIO._serialized_end=3564
   _COMPRESSED._serialized_start=3566
   _COMPRESSED._serialized_end=3619
-  _DEVICEMETADATA._serialized_start=3622
-  _DEVICEMETADATA._serialized_end=3874
+  _NEIGHBORINFO._serialized_start=3621
+  _NEIGHBORINFO._serialized_end=3707
+  _NEIGHBOR._serialized_start=3709
+  _NEIGHBOR._serialized_end=3749
+  _DEVICEMETADATA._serialized_start=3752
+  _DEVICEMETADATA._serialized_end=4031
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/module_config_pb2.py` & `meshtastic-2.1.7/meshtastic/module_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: meshtastic/module_config.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xb8\x17\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1a\'\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\x9b\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"H\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variantBg\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\x88\x18\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\x9b\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"H\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
+_REMOTEHARDWAREPINTYPE = DESCRIPTOR.enum_types_by_name['RemoteHardwarePinType']
+RemoteHardwarePinType = enum_type_wrapper.EnumTypeWrapper(_REMOTEHARDWAREPINTYPE)
+UNKNOWN = 0
+DIGITAL_READ = 1
+DIGITAL_WRITE = 2
 
 
 _MODULECONFIG = DESCRIPTOR.message_types_by_name['ModuleConfig']
 _MODULECONFIG_MQTTCONFIG = _MODULECONFIG.nested_types_by_name['MQTTConfig']
 _MODULECONFIG_REMOTEHARDWARECONFIG = _MODULECONFIG.nested_types_by_name['RemoteHardwareConfig']
 _MODULECONFIG_AUDIOCONFIG = _MODULECONFIG.nested_types_by_name['AudioConfig']
 _MODULECONFIG_SERIALCONFIG = _MODULECONFIG.nested_types_by_name['SerialConfig']
 _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG = _MODULECONFIG.nested_types_by_name['ExternalNotificationConfig']
 _MODULECONFIG_STOREFORWARDCONFIG = _MODULECONFIG.nested_types_by_name['StoreForwardConfig']
 _MODULECONFIG_RANGETESTCONFIG = _MODULECONFIG.nested_types_by_name['RangeTestConfig']
 _MODULECONFIG_TELEMETRYCONFIG = _MODULECONFIG.nested_types_by_name['TelemetryConfig']
 _MODULECONFIG_CANNEDMESSAGECONFIG = _MODULECONFIG.nested_types_by_name['CannedMessageConfig']
+_REMOTEHARDWAREPIN = DESCRIPTOR.message_types_by_name['RemoteHardwarePin']
 _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD = _MODULECONFIG_AUDIOCONFIG.enum_types_by_name['Audio_Baud']
 _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD = _MODULECONFIG_SERIALCONFIG.enum_types_by_name['Serial_Baud']
 _MODULECONFIG_SERIALCONFIG_SERIAL_MODE = _MODULECONFIG_SERIALCONFIG.enum_types_by_name['Serial_Mode']
 _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR = _MODULECONFIG_CANNEDMESSAGECONFIG.enum_types_by_name['InputEventChar']
 ModuleConfig = _reflection.GeneratedProtocolMessageType('ModuleConfig', (_message.Message,), {
 
   'MQTTConfig' : _reflection.GeneratedProtocolMessageType('MQTTConfig', (_message.Message,), {
@@ -107,40 +114,51 @@
 _sym_db.RegisterMessage(ModuleConfig.SerialConfig)
 _sym_db.RegisterMessage(ModuleConfig.ExternalNotificationConfig)
 _sym_db.RegisterMessage(ModuleConfig.StoreForwardConfig)
 _sym_db.RegisterMessage(ModuleConfig.RangeTestConfig)
 _sym_db.RegisterMessage(ModuleConfig.TelemetryConfig)
 _sym_db.RegisterMessage(ModuleConfig.CannedMessageConfig)
 
+RemoteHardwarePin = _reflection.GeneratedProtocolMessageType('RemoteHardwarePin', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTEHARDWAREPIN,
+  '__module__' : 'meshtastic.module_config_pb2'
+  # @@protoc_insertion_point(class_scope:RemoteHardwarePin)
+  })
+_sym_db.RegisterMessage(RemoteHardwarePin)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\022ModuleConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
+  _REMOTEHARDWAREPINTYPE._serialized_start=3208
+  _REMOTEHARDWAREPINTYPE._serialized_end=3281
   _MODULECONFIG._serialized_start=35
-  _MODULECONFIG._serialized_end=3035
+  _MODULECONFIG._serialized_end=3115
   _MODULECONFIG_MQTTCONFIG._serialized_start=547
   _MODULECONFIG_MQTTCONFIG._serialized_end=714
   _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=716
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=755
-  _MODULECONFIG_AUDIOCONFIG._serialized_start=758
-  _MODULECONFIG_AUDIOCONFIG._serialized_end=1103
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=936
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1103
-  _MODULECONFIG_SERIALCONFIG._serialized_start=1106
-  _MODULECONFIG_SERIALCONFIG._serialized_end=1645
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1305
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1571
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1573
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1645
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1648
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=1982
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=1985
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2117
-  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2119
-  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2183
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2186
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2448
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2451
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3016
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=2917
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3016
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=835
+  _MODULECONFIG_AUDIOCONFIG._serialized_start=838
+  _MODULECONFIG_AUDIOCONFIG._serialized_end=1183
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1016
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1183
+  _MODULECONFIG_SERIALCONFIG._serialized_start=1186
+  _MODULECONFIG_SERIALCONFIG._serialized_end=1725
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1385
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1651
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1653
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1725
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1728
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2062
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2065
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2197
+  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2199
+  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2263
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2266
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2528
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2531
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3096
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=2997
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3096
+  _REMOTEHARDWAREPIN._serialized_start=3117
+  _REMOTEHARDWAREPIN._serialized_end=3206
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/mqtt_pb2.py` & `meshtastic-2.1.7/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/node.py` & `meshtastic-2.1.7/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/portnums_pb2.py` & `meshtastic-2.1.7/meshtastic/portnums_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/portnums.proto*\xa4\x03\n\x07PortNum\x12\x0f\n\x0bUNKNOWN_APP\x10\x00\x12\x14\n\x10TEXT_MESSAGE_APP\x10\x01\x12\x17\n\x13REMOTE_HARDWARE_APP\x10\x02\x12\x10\n\x0cPOSITION_APP\x10\x03\x12\x10\n\x0cNODEINFO_APP\x10\x04\x12\x0f\n\x0bROUTING_APP\x10\x05\x12\r\n\tADMIN_APP\x10\x06\x12\x1f\n\x1bTEXT_MESSAGE_COMPRESSED_APP\x10\x07\x12\x10\n\x0cWAYPOINT_APP\x10\x08\x12\r\n\tAUDIO_APP\x10\t\x12\r\n\tREPLY_APP\x10 \x12\x11\n\rIP_TUNNEL_APP\x10!\x12\x0e\n\nSERIAL_APP\x10@\x12\x15\n\x11STORE_FORWARD_APP\x10\x41\x12\x12\n\x0eRANGE_TEST_APP\x10\x42\x12\x11\n\rTELEMETRY_APP\x10\x43\x12\x0b\n\x07ZPS_APP\x10\x44\x12\x11\n\rSIMULATOR_APP\x10\x45\x12\x12\n\x0eTRACEROUTE_APP\x10\x46\x12\x10\n\x0bPRIVATE_APP\x10\x80\x02\x12\x13\n\x0e\x41TAK_FORWARDER\x10\x81\x02\x12\x08\n\x03MAX\x10\xff\x03\x42]\n\x13\x63om.geeksville.meshB\x08PortnumsZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19meshtastic/portnums.proto*\xba\x03\n\x07PortNum\x12\x0f\n\x0bUNKNOWN_APP\x10\x00\x12\x14\n\x10TEXT_MESSAGE_APP\x10\x01\x12\x17\n\x13REMOTE_HARDWARE_APP\x10\x02\x12\x10\n\x0cPOSITION_APP\x10\x03\x12\x10\n\x0cNODEINFO_APP\x10\x04\x12\x0f\n\x0bROUTING_APP\x10\x05\x12\r\n\tADMIN_APP\x10\x06\x12\x1f\n\x1bTEXT_MESSAGE_COMPRESSED_APP\x10\x07\x12\x10\n\x0cWAYPOINT_APP\x10\x08\x12\r\n\tAUDIO_APP\x10\t\x12\r\n\tREPLY_APP\x10 \x12\x11\n\rIP_TUNNEL_APP\x10!\x12\x0e\n\nSERIAL_APP\x10@\x12\x15\n\x11STORE_FORWARD_APP\x10\x41\x12\x12\n\x0eRANGE_TEST_APP\x10\x42\x12\x11\n\rTELEMETRY_APP\x10\x43\x12\x0b\n\x07ZPS_APP\x10\x44\x12\x11\n\rSIMULATOR_APP\x10\x45\x12\x12\n\x0eTRACEROUTE_APP\x10\x46\x12\x14\n\x10NEIGHBORINFO_APP\x10G\x12\x10\n\x0bPRIVATE_APP\x10\x80\x02\x12\x13\n\x0e\x41TAK_FORWARDER\x10\x81\x02\x12\x08\n\x03MAX\x10\xff\x03\x42]\n\x13\x63om.geeksville.meshB\x08PortnumsZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _PORTNUM = DESCRIPTOR.enum_types_by_name['PortNum']
 PortNum = enum_type_wrapper.EnumTypeWrapper(_PORTNUM)
 UNKNOWN_APP = 0
 TEXT_MESSAGE_APP = 1
 REMOTE_HARDWARE_APP = 2
 POSITION_APP = 3
@@ -34,19 +34,20 @@
 SERIAL_APP = 64
 STORE_FORWARD_APP = 65
 RANGE_TEST_APP = 66
 TELEMETRY_APP = 67
 ZPS_APP = 68
 SIMULATOR_APP = 69
 TRACEROUTE_APP = 70
+NEIGHBORINFO_APP = 71
 PRIVATE_APP = 256
 ATAK_FORWARDER = 257
 MAX = 511
 
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\010PortnumsZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _PORTNUM._serialized_start=30
-  _PORTNUM._serialized_end=450
+  _PORTNUM._serialized_end=472
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.6/meshtastic/remote_hardware.py` & `meshtastic-2.1.7/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.1.7/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/rtttl_pb2.py` & `meshtastic-2.1.7/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/serial_interface.py` & `meshtastic-2.1.7/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/storeforward_pb2.py` & `meshtastic-2.1.7/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/stream_interface.py` & `meshtastic-2.1.7/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/supported_device.py` & `meshtastic-2.1.7/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/tcp_interface.py` & `meshtastic-2.1.7/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/telemetry_pb2.py` & `meshtastic-2.1.7/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/test.py` & `meshtastic-2.1.7/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/tunnel.py` & `meshtastic-2.1.7/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/util.py` & `meshtastic-2.1.7/meshtastic/util.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic/xmodem_pb2.py` & `meshtastic-2.1.7/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.1.7/meshtastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.6/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.1.7/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.6/setup.py` & `meshtastic-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.1.6",
+    version="2.1.7",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

