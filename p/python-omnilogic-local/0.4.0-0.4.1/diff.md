# Comparing `tmp/python_omnilogic_local-0.4.0.tar.gz` & `tmp/python_omnilogic_local-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.4.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.4.1.tar", max compression
```

## Comparing `python_omnilogic_local-0.4.0.tar` & `python_omnilogic_local-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    20177 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3931 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7804 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9535 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     9040 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-28 01:21:31.081668 python_omnilogic_local-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    20177 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3931 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7864 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9619 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     9040 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-28 14:15:08.841250 python_omnilogic_local-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.1/PKG-INFO
```

### Comparing `python_omnilogic_local-0.4.0/README.md` & `python_omnilogic_local-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/models/mspconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,57 +63,57 @@
     omni_type: OmniType = OmniType.SYSTEM
     vsp_speed_format: Literal["RPM", "Percent"] = Field(alias="Msp-Vsp-Speed-Format")
     units: Literal["Standard", "Metric"] = Field(alias="Units")
 
 
 class MSPSensor(OmniBase):
     omni_type: OmniType = OmniType.SENSOR
-    type: SensorType = Field(alias="Type")
-    units: SensorUnits = Field(alias="Units")
+    type: SensorType | str = Field(alias="Type")
+    units: SensorUnits | str = Field(alias="Units")
 
 
 class MSPFilter(OmniBase):
     omni_type: OmniType = OmniType.FILTER
-    type: FilterType = Field(alias="Filter-Type")
+    type: FilterType | str = Field(alias="Filter-Type")
     max_percent: int = Field(alias="Max-Pump-Speed")
     min_percent: int = Field(alias="Min-Pump-Speed")
     max_rpm: int = Field(alias="Max-Pump-RPM")
     min_rpm: int = Field(alias="Min-Pump-RPM")
     # We should figure out how to coerce this field into a True/False
     priming_enabled: Literal["yes", "no"] = Field(alias="Priming-Enabled")
     low_speed: int = Field(alias="Vsp-Low-Pump-Speed")
     medium_speed: int = Field(alias="Vsp-Medium-Pump-Speed")
     high_speed: int = Field(alias="Vsp-High-Pump-Speed")
 
 
 class MSPPump(OmniBase):
     omni_type: OmniType = OmniType.PUMP
-    type: PumpType = Field(alias="Type")
-    function: PumpFunction = Field(alias="Function")
+    type: PumpType | str = Field(alias="Type")
+    function: PumpFunction | str = Field(alias="Function")
     max_percent: int = Field(alias="Max-Pump-Speed")
     min_percent: int = Field(alias="Min-Pump-Speed")
     max_rpm: int = Field(alias="Max-Pump-RPM")
     min_rpm: int = Field(alias="Min-Pump-RPM")
     # We should figure out how to coerce this field into a True/False
     priming_enabled: Literal["yes", "no"] = Field(alias="Priming-Enabled")
     low_speed: int = Field(alias="Vsp-Low-Pump-Speed")
     medium_speed: int = Field(alias="Vsp-Medium-Pump-Speed")
     high_speed: int = Field(alias="Vsp-High-Pump-Speed")
 
 
 class MSPRelay(OmniBase):
     omni_type: OmniType = OmniType.RELAY
-    type: RelayType = Field(alias="Type")
-    function: RelayFunction = Field(alias="Function")
+    type: RelayType | str = Field(alias="Type")
+    function: RelayFunction | str = Field(alias="Function")
 
 
 class MSPHeaterEquip(OmniBase):
     omni_type: OmniType = OmniType.HEATER_EQUIP
     type: Literal["PET_HEATER"] = Field(alias="Type")
-    heater_type: HeaterType = Field(alias="Heater-Type")
+    heater_type: HeaterType | str = Field(alias="Heater-Type")
     enabled: Literal["yes", "no"] = Field(alias="Enabled")
     min_filter_speed: int = Field(alias="Min-Speed-For-Operation")
     sensor_id: int = Field(alias="Sensor-System-Id")
     supports_cooling: Literal["yes", "no"] | None = Field(alias="SupportsCooling")
 
 
 # This is the entry for the VirtualHeater, it does not use OmniBase because it has no name attribute
@@ -135,23 +135,23 @@
         # first filter down to just the heater equipment items, then populate our self.heater_equipment with parsed versions of those items.
         heater_equip_data = [op for op in data.get("Operation", {}) if OmniType.HEATER_EQUIP in op][0]
         self.heater_equipment = [MSPHeaterEquip.parse_obj(equip) for equip in heater_equip_data[OmniType.HEATER_EQUIP]]
 
 
 class MSPColorLogicLight(OmniBase):
     omni_type: OmniType = OmniType.CL_LIGHT
-    type: ColorLogicLightType = Field(alias="Type")
+    type: ColorLogicLightType | str = Field(alias="Type")
     v2_active: Literal["yes", "no"] = Field(alias="V2-Active")
 
 
 class MSPBoW(OmniBase):
     _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light"}
 
     omni_type: OmniType = OmniType.BOW
-    type: BodyOfWaterType = Field(alias="Type")
+    type: BodyOfWaterType | str = Field(alias="Type")
     filter: list[MSPFilter] | None = Field(alias="Filter")
     relay: list[MSPRelay] | None = Field(alias="Relay")
     heater: MSPVirtualHeater | None = Field(alias="Heater")
     sensor: list[MSPSensor] | None = Field(alias="Sensor")
     colorlogic_light: list[MSPColorLogicLight] | None = Field(alias="ColorLogic-Light")
 
     # We override the __init__ here so that we can trigger the propagation of the bow_id down to all of it's sub devices after the bow
```

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/models/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 class TelemetryBackyard(BaseModel):
     omni_type: OmniType = OmniType.BACKYARD
     system_id: int = Field(alias="@systemId")
     status_version: int = Field(alias="@statusVersion")
     air_temp: int = Field(alias="@airTemp")
-    state: BackyardState = Field(alias="@state")
+    state: BackyardState | int = Field(alias="@state")
     config_checksum: int = Field(alias="@ConfigChksum")
     msp_version: str = Field(alias="@mspVersion")
 
 
 class TelemetryBoW(BaseModel):
     omni_type: OmniType = OmniType.BOW
     system_id: int = Field(alias="@systemId")
@@ -64,86 +64,86 @@
     instant_salt_level: int = Field(alias="@instantSaltLevel")
     avg_salt_level: int = Field(alias="@avgSaltLevel")
     chlr_alert: int = Field(alias="@chlrAlert")
     chlr_error: int = Field(alias="@chlrError")
     sc_mode: int = Field(alias="@scMode")
     operating_state: int = Field(alias="@operatingState")
     timed_percent: int = Field(alias="@Timed-Percent")
-    operating_mode: ChlorinatorOperatingMode = Field(alias="@operatingMode")
+    operating_mode: ChlorinatorOperatingMode | int = Field(alias="@operatingMode")
     enable: bool = Field(alias="@enable")
 
 
 class TelemetryColorLogicLight(BaseModel):
     omni_type: OmniType = OmniType.CL_LIGHT
     system_id: int = Field(alias="@systemId")
-    state: ColorLogicPowerState = Field(alias="@lightState")
-    show: ColorLogicShow = Field(alias="@currentShow")
-    speed: ColorLogicSpeed = Field(alias="@speed")
-    brightness: ColorLogicBrightness = Field(alias="@brightness")
+    state: ColorLogicPowerState | int = Field(alias="@lightState")
+    show: ColorLogicShow | int = Field(alias="@currentShow")
+    speed: ColorLogicSpeed | int = Field(alias="@speed")
+    brightness: ColorLogicBrightness | int = Field(alias="@brightness")
     special_effect: int = Field(alias="@specialEffect")
 
 
 class TelemetryFilter(BaseModel):
     omni_type: OmniType = OmniType.FILTER
     system_id: int = Field(alias="@systemId")
-    state: FilterState = Field(alias="@filterState")
+    state: FilterState | int = Field(alias="@filterState")
     speed: int = Field(alias="@filterSpeed")
-    valve_position: FilterValvePosition = Field(alias="@valvePosition")
-    why_on: FilterWhyOn = Field(alias="@whyFilterIsOn")
+    valve_position: FilterValvePosition | int = Field(alias="@valvePosition")
+    why_on: FilterWhyOn | int = Field(alias="@whyFilterIsOn")
     reported_speed: int = Field(alias="@reportedFilterSpeed")
     power: int = Field(alias="@power")
     last_speed: int = Field(alias="@lastSpeed")
 
 
 class TelemetryGroup(BaseModel):
     omni_type: OmniType = OmniType.GROUP
     system_id: int = Field(alias="@systemId")
     state: int = Field(alias="@groupState")
 
 
 class TelemetryHeater(BaseModel):
     omni_type: OmniType = OmniType.HEATER
     system_id: int = Field(alias="@systemId")
-    state: HeaterState = Field(alias="@heaterState")
+    state: HeaterState | int = Field(alias="@heaterState")
     temp: int = Field(alias="@temp")
     enabled: bool = Field(alias="@enable")
     priority: int = Field(alias="@priority")
     maintain_for: int = Field(alias="@maintainFor")
 
 
 class TelemetryPump(BaseModel):
     omni_type: OmniType = OmniType.PUMP
     system_id: int = Field(alias="@systemId")
-    state: PumpState = Field(alias="@pumpState")
+    state: PumpState | int = Field(alias="@pumpState")
     speed: int = Field(alias="@pummpSpeed")
     last_speed: int = Field(alias="@lastSpeed")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryRelay(BaseModel):
     omni_type: OmniType = OmniType.RELAY
     system_id: int = Field(alias="@systemId")
-    state: RelayState = Field(alias="@relayState")
+    state: RelayState | int = Field(alias="@relayState")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryValveActuator(BaseModel):
     omni_type: OmniType = OmniType.VALVE_ACTUATOR
     system_id: int = Field(alias="@systemId")
-    state: ValveActuatorState = Field(alias="@valveActuatorState")
+    state: ValveActuatorState | int = Field(alias="@valveActuatorState")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryVirtualHeater(BaseModel):
     omni_type: OmniType = OmniType.VIRT_HEATER
     system_id: int = Field(alias="@systemId")
     current_set_point: int = Field(alias="@Current-Set-Point")
     enabled: bool = Field(alias="@enable")
     solar_set_point: int = Field(alias="@SolarSetPoint")
-    mode: HeaterMode = Field(alias="@Mode")
+    mode: HeaterMode | int = Field(alias="@Mode")
     silent_mode: int = Field(alias="@SilentMode")
     why_on: int = Field(alias="@whyHeaterIsOn")
 
 
 TelemetryType: TypeAlias = (
     TelemetryBackyard
     | TelemetryBoW
```

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.4.1/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.0/pyproject.toml` & `python_omnilogic_local-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.4.0"
+version = "0.4.1"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.4.0/PKG-INFO` & `python_omnilogic_local-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.1 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

