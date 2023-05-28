# Comparing `tmp/python_omnilogic_local-0.3.4.tar.gz` & `tmp/python_omnilogic_local-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.3.4.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.4.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.3.4.tar` & `python_omnilogic_local-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    20177 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3931 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7748 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9535 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     9040 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-27 14:56:04.915118 python_omnilogic_local-0.3.4/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-27 14:56:05.811131 python_omnilogic_local-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    20177 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3931 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7804 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9535 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     9040 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-28 01:21:30.049604 python_omnilogic_local-0.4.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-28 01:21:31.081668 python_omnilogic_local-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.3.4/README.md` & `python_omnilogic_local-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/api.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
 
 class MSPBackyard(OmniBase):
     _sub_devices = {"sensor", "bow"}
 
     omni_type: OmniType = OmniType.BACKYARD
     sensor: list[MSPSensor] | None = Field(alias="Sensor")
     bow: list[MSPBoW] | None = Field(alias="Body-of-water")
+    relay: list[MSPRelay] | None = Field(alias="Relay")
 
 
 class MSPSchedule(OmniBase):
     omni_type: OmniType = OmniType.SCHEDULE
     system_id: int = Field(alias="schedule-system-id")
     bow_id: int = Field(alias="bow-system-id")
     equipment_id: int = Field(alias="equipment-id")
```

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyomnilogic_local/types.py` & `python_omnilogic_local-0.4.0/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.4/pyproject.toml` & `python_omnilogic_local-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.3.4"
+version = "0.4.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.3.4/PKG-INFO` & `python_omnilogic_local-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.3.4
+Version: 0.4.0
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
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.4 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

