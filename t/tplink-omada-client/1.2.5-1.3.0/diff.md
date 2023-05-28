# Comparing `tmp/tplink_omada_client-1.2.5.tar.gz` & `tmp/tplink_omada_client-1.3.0.tar.gz`

## Comparing `tplink_omada_client-1.2.5.tar` & `tplink_omada_client-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,42 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.pylintrc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/Dockerfile.dev
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/requirements.txt
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    19064 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_default.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_gateway.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.pylintrc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/Dockerfile.dev
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/requirements.txt
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/clients.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    19177 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_block_client.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_client.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_clients.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_gateway.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_known_clients.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch_ports.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_unblock_client.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/PKG-INFO
```

### Comparing `tplink_omada_client-1.2.5/Dockerfile.dev` & `tplink_omada_client-1.3.0/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/sample_client.py` & `tplink_omada_client-1.3.0/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/.devcontainer/devcontainer.json` & `tplink_omada_client-1.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/.github/workflows/python-package.yml` & `tplink_omada_client-1.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/.github/workflows/python-publish.yml` & `tplink_omada_client-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/.vscode/launch.json` & `tplink_omada_client-1.3.0/.vscode/launch.json`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,22 @@
             "type": "python",
             "request": "launch",
             "module": "tplink_omada_client.cli",
             "justMyCode": true,
             "args": ["switch", "Main Switch", "--dump"]
         },
         {
+            "name": "CLI: Get Switch Ports",
+            "type": "python",
+            "request": "launch",
+            "module": "tplink_omada_client.cli",
+            "justMyCode": true,
+            "args": ["switch_ports", "Main Switch", "-t", "-p", "5"]
+        },
+        {
             "name": "CLI: Get Gateway",
             "type": "python",
             "request": "launch",
             "module": "tplink_omada_client.cli",
             "justMyCode": true,
             "args": ["gateway", "--dump"]
         }
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/definitions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 """ Definitions for Omada enums. """
 
+from abc import ABC
 from enum import IntEnum
+from typing import Any
 
+class OmadaApiData(ABC):
+    def __init__(self, data: dict[str, Any]):
+        self._data = data
+
+    def __repr__(self) -> str:
+        repr = self.__class__.__name__
+        repr += "{"
+        for name in self.__dir__():
+            if (
+                not name.startswith("_")
+                and name != "raw_data"
+            ):
+                repr += f"{name}={getattr(self, name)},"
+        repr += "}"
+        return repr
+
+    @property
+    def raw_data(self) -> dict[str, Any]:
+        return self._data
 
 class DeviceStatus(IntEnum):
     """Known status codes for devices."""
 
     DISCONNECTED = 0
     DISCONNECTED_MIGRATING = 1
     PROVISIONING = 10
@@ -102,10 +123,42 @@
     RATE_LIMIT = 1
     STORM_CONTROL = 2
 
 
 class PoEMode(IntEnum):
     """Settings for PoE policy."""
 
+    NONE = -1
     DISABLED = 0
     ENABLED = 1
     USE_DEVICE_SETTINGS = 2
+
+class AuthenticationStatus:
+    """ Client authentication status. """
+    CONNECTED = 0
+    PENDING = 1
+    AUTHORIZED = 2
+    AUTH_FREE = 3
+
+class ConnectType(IntEnum):
+    """ Client connection types. """
+    GUEST_WIRELESS = 0
+    WIRELESS = 1
+    WIRED = 2
+
+class RadioId(IntEnum):
+    """ WiFi radio frequencies """
+    FREQ_2_4 = 0
+    FREQ_5_1 = 1
+    FREQ_5_2 = 2
+    FREQ_6   = 3
+
+class WifiMode(IntEnum):
+    """ WiFi modes. """
+    A   = 0
+    B   = 1
+    G   = 2
+    NA  = 3
+    NG  = 4
+    AC  = 5
+    AXA = 6
+    AXG = 7
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,19 @@
     DeviceStatusCategory,
     Eth802Dot1X,
     GatewayPortMode,
     GatewayPortType,
     LinkDuplex,
     LinkSpeed,
     LinkStatus,
+    OmadaApiData,
     PoEMode,
     PortType,
 )
 
-class OmadaApiData:
-    def __init__(self, data: dict[str, Any]):
-        self._data = data
-
-    @property
-    def raw_data(self) -> dict[str, Any]:
-        return self._data
-
-
 class OmadaDevice(OmadaApiData):
     """Details of a device connected to the controller"""
 
     @property
     def type(self) -> str:
         """The type of the device. Its value can be "ap", "gateway", and "switch"."""
         return self._data["type"]
@@ -80,15 +72,15 @@
 
     @property
     def cpu_usage(self) -> int:
         if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
             return self._data["cpuUtil"]
         else:
             return 0
-        
+
     @property
     def mem_usage(self) -> int:
         if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
             return self._data["memUtil"]
         else:
             return 0
 
@@ -183,19 +175,17 @@
 
     @property
     def poe_active(self) -> bool:
         """Is the port powering a PoE device?"""
         return self._data["poe"]
 
     @property
-    def poe_power(self) -> float:
+    def poe_power(self) -> Optional[float]:
         """Power (W) supplied over PoE."""
-        if "poePower" in self._data:
-            return self._data["poePower"]
-        return 0.0
+        return self._data.get("poePower")
 
     @property
     def bytes_tx(self) -> int:
         """Number of bytes transmitted by the port."""
         return self._data["tx"]
 
     @property
@@ -395,27 +385,37 @@
 
     @property
     def max_speed(self) -> LinkSpeed:
         """The max speed of the port."""
         return LinkSpeed(self._data["maxSpeed"])
 
     @property
+    def link_speed(self) -> LinkSpeed:
+        """The link speed of the port."""
+        return LinkSpeed(self._data["linkSpeed"])
+
+    @property
+    def duplex(self) -> LinkDuplex:
+        """The link duplex state of the port."""
+        return LinkDuplex(self._data['duplex'])
+
+    @property
     def profile_name(self) -> str:
         """Name of the port's config profile"""
         return self._data["profileName"]
 
     @property
     def has_profile_override(self) -> bool:
         """True if the port's config profile has been overridden."""
         return self._data["profileOverrideEnable"]
 
     @property
     def poe_mode(self) -> PoEMode:
         """PoE config for this port."""
-        return self._data["poe"]
+        return PoEMode(self._data.get("poe", PoEMode.NONE))
 
     @property
     def bandwidth_limit_mode(self) -> BandwidthControl:
         """Type of bandwidth control applied."""
         return BandwidthControl(self._data["bandWidthCtrlType"])
 
     # "bandCtrl": {
@@ -485,15 +485,15 @@
     def name(self) -> str:
         """Name of the profile."""
         return self._data["name"]
 
     @property
     def poe_mode(self) -> PoEMode:
         """PoE mode."""
-        return PoEMode(self._data["poe"])
+        return PoEMode(self._data.get("poe", PoEMode.NONE))
 
     @property
     def bandwidth_limit_mode(self) -> BandwidthControl:
         """Type of bandwidth control applied."""
         return BandwidthControl(self._data["bandWidthCtrlType"])
 
     @property
@@ -552,15 +552,15 @@
     @property
     def release_notes(self) -> str:
         """Release notes for the new firmware."""
         return self._data["fwReleaseLog"]
 
 class OmadaGatewayPort(OmadaApiData):
 
-    
+
     @property
     def port_number(self) -> int:
         return self._data["port"]
 
     @property
     def name(self) -> str:
         """Port name"""
@@ -653,23 +653,23 @@
         """True if the device supports PoE."""
         return self._data["supportPoe"]
 
     @property
     def ip(self) -> str:
         """Gateway's LAN IP address."""
         return self._data["ip"]
-        
+
     @property
     def port_status(self) -> List[OmadaGatewayPort]:
         """Status of the gateway's ports."""
         return [
             OmadaGatewayPort(p) for p in self._data["portStats"]
         ]
 
-    @property 
+    @property
     def port_configs(self) -> List[OmadaGatewayPortConfig]:
         """Configuration of the gateway's ports. Also includes status..."""
         return [
             OmadaGatewayPortConfig(p) for p in self._data["portConfigs"]
         ]
 
     @property
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/omadaapiconnection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Internal Omada API client."""
 
 import time
-from typing import Any, Optional, Tuple
+from typing import Any, AsyncIterable, Optional, Tuple
 
 import re
 from urllib.parse import urlsplit, urljoin
 from aiohttp import client_exceptions, CookieJar
 from aiohttp.client import ClientSession
 from awesomeversion  import AwesomeVersion
 
@@ -15,14 +15,16 @@
     LoginFailed,
     LoginSessionClosed,
     RequestFailed,
     UnsupportedControllerVersion,
 )
 
 
+_PAGE_SIZE: int = 100
+
 class OmadaApiConnection:
     """Low level Omada API client."""
 
     _own_session: bool
     _controller_id: str
     _controller_version: str
     _csrf_token: Optional[str]
@@ -138,14 +140,37 @@
         """Get a REST url for the controller action"""
 
         if site:
             end_point = f"sites/{site}/{end_point}"
 
         return urljoin(self._url, f"/{self._controller_id}/api/v2/{end_point}")
 
+    async def iterate_pages(self, url: str, params: Optional[dict[str, Any]]=None) -> AsyncIterable[dict[str, Any]]:
+        """Iterates all the entries of a paged endpoint"""
+        request_params = {}
+        if params is not None:
+            request_params.update(params)
+        request_params["currentPageSize"] = _PAGE_SIZE
+
+        current_page = 1
+        has_next = True
+        while has_next:
+            request_params["currentPage"] = current_page
+            response = await self.request("get", url, request_params)
+            
+            # Setup next page request
+            current_page = int(response['currentPage']) + 1
+            current_size = int(response['currentSize'])
+            total_rows = int(response['totalRows'])
+            has_next = total_rows > current_page * current_size
+
+            data: list[dict[str, Any]] = response['data']
+            for item in data:
+                yield item
+
     async def request(self, method: str, url: str, params=None, payload=None) -> Any:
         """Perform a request specific to the controlller, with authentication"""
 
         if not await self._check_login():
             await self.login()
 
         return await self._do_request(method, url, params=params, payload=payload)
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/omadaclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/omadasiteclient.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Client for Omada Site requests."""
 
-from typing import List, Optional, Union
-from .omadaapiconnection import OmadaApiConnection
+from typing import Any, AsyncIterable, List, Optional, Union
 
+from .clients import (
+    OmadaClientDetails,
+    OmadaConnectedClient,
+    OmadaNetworkClient,
+    OmadaWiredClient,
+    OmadaWiredClientDetails,
+    OmadaWirelessClient,
+    OmadaWirelessClientDetails,
+)
+from .definitions import BandwidthControl, Eth802Dot1X, LinkDuplex, LinkSpeed, PoEMode
 from .devices import (
     OmadaAccessPoint,
     OmadaDevice,
     OmadaFirmwareUpdate,
     OmadaGateway,
     OmadaListDevice,
     OmadaPortProfile,
     OmadaSwitch,
     OmadaSwitchPort,
     OmadaSwitchPortDetails,
     OmadaAccesPointLanPortSettings,
 )
-
 from .exceptions import (
     InvalidDevice,
 )
-
-from .definitions import BandwidthControl, Eth802Dot1X, LinkDuplex, LinkSpeed, PoEMode
+from .omadaapiconnection import OmadaApiConnection
 
 
 class SwitchPortOverrides:
     """
     Overrides that can be applied to a switch port.
 
     Currently, we don't support bandwidth limits and mirroring modes.
@@ -75,14 +82,64 @@
 class OmadaSiteClient:
     """Client for querying an Omada site's devices."""
 
     def __init__(self, site_id: str, api: OmadaApiConnection):
         self._api = api
         self._site_id = site_id
 
+    async def block_client(self, mac_or_client: Union[str, OmadaNetworkClient]) -> None:
+        if isinstance(mac_or_client, OmadaConnectedClient):
+            mac = mac_or_client.mac
+        else:
+            mac = mac_or_client
+        await self._api.request(
+            "post", self._api.format_url(f"cmd/clients/{mac}/block", self._site_id)
+        )
+
+    async def unblock_client(self, mac_or_client: Union[str, OmadaNetworkClient]) -> None:
+        if isinstance(mac_or_client, OmadaConnectedClient):
+            mac = mac_or_client.mac
+        else:
+            mac = mac_or_client
+        await self._api.request(
+            "post", self._api.format_url(f"cmd/clients/{mac}/unblock", self._site_id)
+        )
+
+    async def get_client(self, mac_or_client: Union[str, OmadaNetworkClient]) -> OmadaClientDetails:
+        """Get the details of a client"""
+        if isinstance(mac_or_client, OmadaConnectedClient):
+            mac = mac_or_client.mac
+        else:
+            mac = mac_or_client
+
+        result = await self._api.request(
+            "get", self._api.format_url(f"clients/{mac}", self._site_id)
+        )
+
+        if result.get("wireless"):
+            return OmadaWirelessClientDetails(result)
+        else:
+            return OmadaWiredClientDetails(result)
+
+    async def get_connected_clients(self) -> AsyncIterable[OmadaConnectedClient]:
+        """Get the clients connected to the site network."""
+        async for client in self._api.iterate_pages(self._api.format_url("clients", self._site_id)):
+            if client["wireless"]:
+                yield OmadaWirelessClient(client)
+            else:
+                yield OmadaWiredClient(client)
+
+    async def get_known_clients(self) -> AsyncIterable[OmadaNetworkClient]:
+        """Get the clients connected to the site network."""
+        async for client in self._api.iterate_pages(self._api.format_url("insight/clients", self._site_id)):
+            if client["wireless"]:
+                yield OmadaWirelessClient(client)
+            else:
+                yield OmadaWiredClient(client)
+
     async def get_devices(self) -> List[OmadaListDevice]:
         """Get the list of devices on the site."""
 
         result = await self._api.request(
             "get", self._api.format_url("devices", self._site_id)
         )
 
@@ -139,15 +196,15 @@
         )
 
         return OmadaSwitch(result)
 
     async def get_switch_ports(
         self, mac_or_device: Union[str, OmadaDevice]
     ) -> List[OmadaSwitchPortDetails]:
-        """Get a switch by Mac address or Omada device."""
+        """Get ports of a switch by Mac address or Omada device."""
 
         if isinstance(mac_or_device, OmadaDevice):
             if mac_or_device.type != "switch":
                 raise InvalidDevice()
             mac = mac_or_device.mac
         else:
             mac = mac_or_device
@@ -159,15 +216,16 @@
         return [OmadaSwitchPortDetails(p) for p in result]
 
     async def get_switch_port(
         self,
         mac_or_device: Union[str, OmadaDevice],
         index_or_port: Union[int, OmadaSwitchPort],
     ) -> OmadaSwitchPortDetails:
-        """Get a switch by Mac address or Omada device."""
+        """Get a single port of a switch by Mac address or Omada device,
+            and port number or port object of OmadaSwitch device."""
 
         if isinstance(mac_or_device, OmadaDevice):
             if mac_or_device.type != "switch":
                 raise InvalidDevice()
             mac = mac_or_device.mac
         else:
             mac = mac_or_device
@@ -179,14 +237,54 @@
 
         result = await self._api.request(
             "get", self._api.format_url(f"switches/{mac}/ports/{port}", self._site_id)
         )
 
         return OmadaSwitchPortDetails(result)
 
+    async def get_switch_port_overrides(
+        self,
+        mac_or_device: Union[str, OmadaDevice],
+        index_or_port: Union[int, OmadaSwitchPort],
+    ) -> SwitchPortOverrides:
+        """Return the current override settings for the port of a switch, or the current profile settings as default."""
+
+        port = await self.get_switch_port(mac_or_device, index_or_port)
+
+        # Returns the current overrides
+        if port.has_profile_override:
+            return SwitchPortOverrides(
+                    enable_poe=(port.poe_mode == PoEMode.ENABLED),
+                    dot1x_mode=port.eth_802_1x_control,
+                    duplex=port.duplex,
+                    link_speed=port.link_speed,
+                    lldp_med_enable=port.lldp_med_enabled,
+                    loopback_detect=port.loopback_detect_enabled,
+                    spanning_tree_enable=port.spanning_tree_enabled,
+                    port_isolation=port.port_isolation_enabled
+            )
+
+        # Otherwise the profile's config values are returned
+        prof = await self.get_port_profile(port.profile_id)
+        
+        # The API doesn't provide the PoE mode of the switch (couldn't even find in Omada
+        # GUI how to set the PoE mode of a switch). Thus, use True as a default value.
+        poe_mode = (prof.poe_mode != PoEMode.DISABLED)
+
+        return SwitchPortOverrides(
+                enable_poe=poe_mode,
+                dot1x_mode=prof.eth_802_1x_control,
+                duplex=LinkDuplex.AUTO,
+                link_speed=LinkSpeed.SPEED_AUTO,
+                lldp_med_enable=prof.lldp_med_enabled,
+                loopback_detect=prof.loopback_detect_enabled,
+                spanning_tree_enable=prof.spanning_tree_enabled,
+                port_isolation=prof.port_isolation_enabled
+        )
+
     async def update_access_point_port(
         self,
         mac_or_device: Union[str, OmadaDevice],
         port_name: str,
         setting: AccessPointPortSettings,
     ) -> OmadaAccesPointLanPortSettings:
         """Update the settings for a lan port on the access point."""
@@ -271,14 +369,23 @@
             self._api.format_url(f"switches/{mac}/ports/{port.port}", self._site_id),
             payload=payload,
         )
 
         # Read back the new port settings
         return await self.get_switch_port(mac, port)
 
+    async def get_port_profile(self, profile_id: str) -> OmadaPortProfile:
+        profiles = await self.get_port_profiles()
+
+        profile = next((p for p in profiles if p.profile_id == profile_id), None)
+
+        if not profile:
+            raise InvalidDevice(f"Port profile {profile_id} does not exist")
+        return profile        
+
     async def get_port_profiles(self) -> List[OmadaPortProfile]:
         """Lists the available switch port profiles that can be applied."""
 
         result = await self._api.request(
             "get", self._api.format_url("setting/lan/profileSummary", self._site_id)
         )
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_default.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_default.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_devices.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_gateway.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Implementation for 'gateway' command"""
 
 from argparse import ArgumentParser
 
 from tplink_omada_client.definitions import GatewayPortMode, LinkStatus
 
 from .config import get_target_config, to_omada_connection
-from .util import dump_raw_data, get_mac, get_target_argument
+from .util import dump_raw_data, get_link_status_char, get_device_mac, get_target_argument
 
 async def command_gateway(args) -> int:
     """Executes 'gateway' command"""
     controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
         mac = args['mac']
         if mac:
-            mac = await get_mac(site_client, mac)
+            mac = await get_device_mac(site_client, mac)
         gateway = await site_client.get_gateway(mac)
         print(f"Name: {gateway.name}")
         print(f"Address: {gateway.mac} ({gateway.ip_address})")
         print(f"Status: {gateway.status.name} ({gateway.status_category.name})")
         print(f"Ports: {gateway.number_of_ports}")
         print(f"Supports PoE: {gateway.supports_poe}")
         print(f"Model: {gateway.model_display_name}")
@@ -30,16 +30,15 @@
         lan_ports = (p for p in gateway.port_status if p.mode == GatewayPortMode.LAN)
         print("WAN Ports:")
         for p in wan_ports:
             print(f"    Port: {p.port_number:>2} {p.type.name:7} {p.ip:>15} {p.wan_protocol:>8} ", end="")
             print('\u2611' if p.wan_connected else '\u2610')
         print("LAN Ports:")
         for p in lan_ports:
-            print(f"    Port: {p.port_number:>2} {p.type.name:7} ", end="")
-            print('\u2611' if p.link_status == LinkStatus.LINK_UP else '\u2610')
+            print(f"    Port: {p.port_number:>2} {p.type.name:7} {get_link_status_char(p.link_status)}")
 
         dump_raw_data(args, gateway)
 
     return 0
 
 def arg_parser(subparsers) -> None:
     """Configures arguments parser for 'gateway' command"""
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Implementation for 'switch' command"""
 
 from argparse import ArgumentParser
 
 from .config import get_target_config, to_omada_connection
-from .util import dump_raw_data, get_mac, get_target_argument
+from .util import dump_raw_data, get_device_mac, get_target_argument
 
 async def command_switch(args) -> int:
     """Executes 'switch' command"""
     controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
-        mac = await get_mac(site_client, args['mac'])
+        mac = await get_device_mac(site_client, args['mac'])
         switch = await site_client.get_switch(mac)
         print(f"Name: {switch.name}")
         print(f"Address: {switch.mac} ({switch.ip_address})")
         print(f"Status: {switch.status.name} ({switch.status_category.name})")
         print(f"Ports: {switch.number_of_ports}")
         print(f"Supports PoE: {switch.device_capabilities.supports_poe}")
         if switch.device_capabilities.supports_poe:
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switches.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 """Implementation for 'switches' command"""
 
 from argparse import _SubParsersAction
 
 from .config import get_target_config, to_omada_connection
-from .util import dump_raw_data, get_target_argument
+from .util import dump_raw_data, get_link_status_char, get_power_char, get_target_argument
 
 async def command_switches(args) -> int:
     """Executes 'switches' command"""
     controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
         for switch in await site_client.get_switches():
             print(f"{switch.mac} {switch.ip_address:>15}  {switch.name:20} ", end="")
             for port in switch.ports:
                 if port.is_disabled:
                     print("x", end="")
-                elif port.port_status.link_status:
-                    print("\u2611", end="")
                 else:
-                    print("\u2610", end="")
-                if port.port_status.poe_active:
-                    print("\u26a1", end="")
-                else:
-                    print("  ", end="")
+                    print(get_link_status_char(port.port_status.link_status), end="")
+                print(get_power_char(port.port_status.poe_active), end="")
 
-            dump_raw_data(args, switch)
             print()
+            dump_raw_data(args, switch)
     return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
     """Configures arguments parser for 'switches' command"""
     switches_parser = subparsers.add_parser(
         "switches",
         aliases=['s'],
```

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_target.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_targets.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/LICENSE` & `tplink_omada_client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/README.md` & `tplink_omada_client-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.5/pyproject.toml` & `tplink_omada_client-1.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.2.5"
+version = "1.3.0"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `tplink_omada_client-1.2.5/PKG-INFO` & `tplink_omada_client-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.2.5
+Version: 1.3.0
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

