# Comparing `tmp/solax-0.3.0.tar.gz` & `tmp/solax-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solax-0.3.0.tar", last modified: Sun Sep 11 06:55:14 2022, max compression
+gzip compressed data, was "solax-0.3.1.tar", last modified: Sat May 27 23:24:10 2023, max compression
```

## Comparing `solax-0.3.0.tar` & `solax-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.403752 solax-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.391752 solax-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.395752 solax-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-09-11 06:55:00.000000 solax-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-09-11 06:55:00.000000 solax-0.3.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-11 06:55:00.000000 solax-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-11 06:55:00.000000 solax-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-09-11 06:55:14.403752 solax-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-11 06:55:00.000000 solax-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-11 06:55:00.000000 solax-0.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-11 06:55:14.403752 solax-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-09-11 06:55:00.000000 solax-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.395752 solax-0.3.0/solax/
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-09-11 06:55:00.000000 solax-0.3.0/solax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-09-11 06:55:00.000000 solax-0.3.0/solax/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.399752 solax-0.3.0/solax/inverters/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/qvolt_hyb_g3_3p.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1_boost.py
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1_hybrid_gen4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1_mini.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1_mini_v34.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x1_smart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3410 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x3_v34.py
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-09-11 06:55:00.000000 solax-0.3.0/solax/inverters/x_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-11 06:55:00.000000 solax-0.3.0/solax/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-09-11 06:55:00.000000 solax-0.3.0/solax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.399752 solax-0.3.0/solax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-09-11 06:55:14.000000 solax-0.3.0/solax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-09-11 06:55:14.000000 solax-0.3.0/solax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 06:55:14.000000 solax-0.3.0/solax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-11 06:55:14.000000 solax-0.3.0/solax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-11 06:55:14.000000 solax-0.3.0/solax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.403752 solax-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:00.000000 solax-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-11 06:55:00.000000 solax-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6732 2022-09-11 06:55:00.000000 solax-0.3.0/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.403752 solax-0.3.0/tests/samples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 06:55:14.403752 solax-0.3.0/tests/samples/api/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-11 06:55:00.000000 solax-0.3.0/tests/samples/api/realTimeData.htm
--rw-r--r--   0 runner    (1001) docker     (121)    10719 2022-09-11 06:55:00.000000 solax-0.3.0/tests/samples/expected_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    31447 2022-09-11 06:55:00.000000 solax-0.3.0/tests/samples/responses.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_base_inverter.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_solax.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-09-11 06:55:00.000000 solax-0.3.0/tests/test_vol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.519456 solax-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.507456 solax-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.511457 solax-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-27 23:23:57.000000 solax-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-27 23:23:57.000000 solax-0.3.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 23:23:57.000000 solax-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-27 23:23:57.000000 solax-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-27 23:24:10.519456 solax-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-27 23:23:57.000000 solax-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 23:23:57.000000 solax-0.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 23:24:10.519456 solax-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-27 23:23:57.000000 solax-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-27 23:23:57.000000 solax-0.3.1/solax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-27 23:23:57.000000 solax-0.3.1/solax/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverter_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax/inverters/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/qvolt_hyb_g3_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_hybrid_gen4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_mini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_mini_v34.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3_hybrid_g4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3_v34.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-27 23:23:57.000000 solax-0.3.1/solax/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-27 23:23:57.000000 solax-0.3.1/solax/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-27 23:23:57.000000 solax-0.3.1/solax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:23:57.000000 solax-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-27 23:23:57.000000 solax-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-27 23:23:57.000000 solax-0.3.1/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/samples/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/api/realTimeData.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/expected_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35171 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_base_inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_solax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_vol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-27 23:23:57.000000 solax-0.3.1/verify.sh
```

### Comparing `solax-0.3.0/.github/workflows/publish.yml` & `solax-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `solax-0.3.0/.github/workflows/tests.yaml` & `solax-0.3.1/.github/workflows/tests.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -16,21 +16,24 @@
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python setup.py install
-        pip install --upgrade flake8 pylint pytest pytest-cov pytest-asyncio pytest-httpserver black mypy
+        pip install --upgrade flake8 pylint pytest pytest-cov pytest-asyncio pytest-httpserver black mypy isort
     - name: Check code style with black
       run: |
         black --check .
     - name: Check types with mypy
       run: |
         mypy .
+    - name: Check imports with isort
+      run: |
+        isort --check-only --profile black .
     - name: Lint with flake8
       run: |
         flake8 --ignore=E501 solax tests
     - name: Lint with pylint
       run: |
         pylint -d 'C0111' solax tests
     - name: Test with pytest
```

### Comparing `solax-0.3.0/LICENSE` & `solax-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solax-0.3.0/PKG-INFO` & `solax-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solax
-Version: 0.3.0
+Version: 0.3.1
 Summary: Solax inverter API client
 Home-page: https://github.com/squishykid/solax
 Author: Robin Wohlers-Reichel
 Author-email: me@robinwr.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solax-0.3.0/README.md` & `solax-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `solax-0.3.0/setup.py` & `solax-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.0/solax/__init__.py` & `solax-0.3.1/solax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Support for Solax inverter via local API."""
 import asyncio
-
 import logging
 
 import async_timeout
 
 from solax.discovery import discover
 from solax.inverter import Inverter, InverterResponse
```

### Comparing `solax-0.3.0/solax/inverters/qvolt_hyb_g3_3p.py` & `solax-0.3.1/solax/inverters/qvolt_hyb_g3_3p.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import voluptuous as vol
-import aiohttp
-from solax.inverter import InverterPost
+
+from solax import utils
+from solax.inverter import Inverter, InverterHttpClient, Method, ResponseParser
 from solax.units import Total, Units
-from solax.utils import (
-    div10,
-    div100,
-    pack_u16,
-    twoway_div10,
-    to_signed,
-    twoway_div100,
-)
+from solax.utils import div10, div100, pack_u16, to_signed, twoway_div10, twoway_div100
 
 
-class QVOLTHYBG33P(InverterPost):
+class QVOLTHYBG33P(Inverter):
     """
     QCells
     Q.VOLT HYB-G3-3P
     """
 
     class Processors:
         """
@@ -44,16 +38,18 @@
             return {
                 0: "Self Use Mode",
                 1: "Force Time Use",
                 2: "Back Up Mode",
                 3: "Feed-in Priority",
             }.get(value, f"unmapped value '{value}'")
 
-    def __init__(self, host, port, pwd=""):
-        super().__init__(host, port, pwd)
+    def __init__(
+        self, http_client: InverterHttpClient, response_parser: ResponseParser
+    ):
+        super().__init__(http_client, response_parser)
         self.manufacturer = "Qcells"
 
     _schema = vol.Schema(
         {
             vol.Required("type"): vol.All(int, 14),
             vol.Required("sn"): str,
             vol.Required("ver"): str,
@@ -161,17 +157,20 @@
             # 164,165,166 some curves
             "Battery Operation mode": (168, Units.NONE, cls.Processors.battery_modes),
             # 169: div100 same as [39]
             # 170-199: always 0
         }
 
     @classmethod
-    async def make_request(cls, host, port=80, pwd="", headers=None):
-
-        url = f"http://{host}:{port}/"
-        data = f"optType=ReadRealTimeData&pwd={pwd}"
+    def _build(cls, host, port, pwd="", params_in_query=True):
+        url = utils.to_url(host, port)
+        http_client = InverterHttpClient(url, Method.POST, pwd).with_default_data()
+
+        schema = cls._schema
+        response_decoder = cls.response_decoder()
+        response_parser = ResponseParser(schema, response_decoder)
+        return cls(http_client, response_parser)
 
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers, data=data) as req:
-                resp = await req.read()
-
-        return cls.handle_response(resp)
+    @classmethod
+    def build_all_variants(cls, host, port, pwd=""):
+        versions = [cls._build(host, port, pwd)]
+        return versions
```

### Comparing `solax-0.3.0/solax/inverters/x1.py` & `solax-0.3.1/solax/inverters/x1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import voluptuous as vol
-from solax.inverter import InverterPost
-from solax.units import Units, Total
+
+from solax.inverter import Inverter
+from solax.units import Total, Units
 from solax.utils import startswith
 
 
-class X1(InverterPost):
+class X1(Inverter):
     # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
             vol.Required("type"): vol.All(str, startswith("X1-")),
             vol.Required("SN"): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
```

### Comparing `solax-0.3.0/solax/inverters/x1_boost.py` & `solax-0.3.1/solax/inverters/x1_mini_v34.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import voluptuous as vol
-from solax.inverter import InverterPost
-from solax.units import Units, Total
-from solax.utils import div10, div100, to_signed
 
+from solax.inverter import Inverter
+from solax.units import Total, Units
+from solax.utils import div10, div100
 
-class X1Boost(InverterPost):
+
+class X1MiniV34(Inverter):
     """
-    X1-Boost with Pocket WiFi 2.034.06
-    Includes X-Forwarded-For for direct LAN API access
+    X1-Boost-Air-Mini with Wifi Pocket v2.034.06
+    SolarX disabled lan access with this custom
+    firmware you can access te Wifi Pocket from your internal lan:
+    https://blog.chrisoft.io/2021/02/14/
+    firmwares-modificados-para-solax-pocket-wifi-v2/
     """
 
     # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
             vol.Required("type", "type"): vol.All(int, 4),
             vol.Required(
                 "sn",
             ): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
                 vol.All(
                     [vol.Coerce(float)],
-                    vol.Length(min=200, max=200),
+                    vol.Any(
+                        vol.Length(min=69, max=69),
+                        vol.Length(min=200, max=200),
+                    ),
                 )
             ),
             vol.Required("Information"): vol.Schema(
-                vol.All(vol.Length(min=10, max=10))
+                vol.Any(vol.Length(min=9, max=9), vol.Length(min=10, max=10))
             ),
         },
         extra=vol.REMOVE_EXTRA,
     )
 
     @classmethod
     def response_decoder(cls):
         return {
-            "AC Voltage": (0, Units.V, div10),
-            "AC Output Current": (1, Units.A, div10),
-            "AC Output Power": (2, Units.W),
+            "Network Voltage": (0, Units.V, div10),
+            "Output Current": (1, Units.A, div10),
+            "AC Power": (2, Units.W),
             "PV1 Voltage": (3, Units.V, div10),
             "PV2 Voltage": (4, Units.V, div10),
             "PV1 Current": (5, Units.A, div10),
             "PV2 Current": (6, Units.A, div10),
             "PV1 Power": (7, Units.W),
             "PV2 Power": (8, Units.W),
-            "AC Frequency": (9, Units.HZ, div100),
-            "Total Generated Energy": (11, Total(Units.KWH), div10),
-            "Today's Generated Energy": (13, Total(Units.KWH), div10),
-            "Inverter Temperature": (39, Units.C),
-            "Exported Power": (48, Units.W, to_signed),
-            "Total Export Energy": (50, Total(Units.KWH), div100),
-            "Total Import Energy": (52, Total(Units.KWH), div100),
+            "Grid Frequency": (9, Units.HZ, div100),
+            "Total Energy": (11, Total(Units.KWH), div10),
+            "Today's Energy": (13, Units.KWH, div10),
+            "Total Feed-in Energy": (41, Total(Units.KWH), div10),
+            "Total Consumption": (42, Total(Units.KWH), div10),
+            "Power Now": (43, Units.W, div10),
+            "Inverter Temperature": (55, Units.C),
         }
 
-    @classmethod
-    async def make_request(cls, host, port=80, pwd="", headers=None):
-        headers = {"X-Forwarded-For": "5.8.8.8"}
-        return await super().make_request(host, port, pwd, headers=headers)
+    # pylint: enable=duplicate-code
```

### Comparing `solax-0.3.0/solax/inverters/x1_hybrid_gen4.py` & `solax-0.3.1/solax/inverters/x1_hybrid_gen4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import voluptuous as vol
-from solax.inverter import InverterPostData
-from solax.units import Units, Total
+
+from solax import utils
+from solax.inverter import Inverter, InverterHttpClient, Method, ResponseParser
+from solax.units import Total, Units
 from solax.utils import div10, div100, pack_u16, to_signed
 
 
-class X1HybridGen4(InverterPostData):
+class X1HybridGen4(Inverter):
     # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
             vol.Required("type"): vol.All(int, 15),
             vol.Required(
                 "sn",
             ): str,
@@ -21,14 +23,27 @@
             ),
             vol.Required("Information"): vol.Schema(vol.All(vol.Length(min=9, max=10))),
         },
         extra=vol.REMOVE_EXTRA,
     )
 
     @classmethod
+    def _build(cls, host, port, pwd="", params_in_query=True):
+        url = utils.to_url(host, port)
+        http_client = InverterHttpClient(url, Method.POST, pwd).with_default_data()
+
+        response_parser = ResponseParser(cls._schema, cls.response_decoder())
+        return cls(http_client, response_parser)
+
+    @classmethod
+    def build_all_variants(cls, host, port, pwd=""):
+        versions = [cls._build(host, port, pwd)]
+        return versions
+
+    @classmethod
     def response_decoder(cls):
         return {
             "AC voltage R": (0, Units.V, div10),
             "AC current": (1, Units.A, div10),
             "AC power": (2, Units.W),
             "Grid frequency": (3, Units.HZ, div100),
             "PV1 voltage": (4, Units.V, div10),
```

### Comparing `solax-0.3.0/solax/inverters/x1_mini.py` & `solax-0.3.1/solax/inverters/x1_mini.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import voluptuous as vol
-from solax.inverter import InverterPost
+
+from solax.inverter import Inverter
 from solax.units import Total, Units
 from solax.utils import startswith
 
 
-class X1Mini(InverterPost):
+class X1Mini(Inverter):
     # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
             vol.Required("type"): vol.All(str, startswith("X1-")),
             vol.Required("SN"): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
```

### Comparing `solax-0.3.0/solax/inverters/x1_mini_v34.py` & `solax-0.3.1/solax/inverters/x3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import voluptuous as vol
 
-from solax.inverter import InverterPost
-from solax.units import Units, Total
-from solax.utils import div10, div100
+from solax.inverter import Inverter
+from solax.units import Total, Units
+from solax.utils import startswith
 
 
-class X1MiniV34(InverterPost):
-    """
-    X1-Boost-Air-Mini with Wifi Pocket v2.034.06
-    SolarX disabled lan access with this custom
-    firmware you can access te Wifi Pocket from your internal lan:
-    https://blog.chrisoft.io/2021/02/14/
-    firmwares-modificados-para-solax-pocket-wifi-v2/
-    """
-
-    # pylint: disable=duplicate-code
+class X3(Inverter):
     _schema = vol.Schema(
         {
-            vol.Required("type", "type"): vol.All(int, 4),
-            vol.Required(
-                "sn",
-            ): str,
+            vol.Required("type"): vol.All(str, startswith("X3-")),
+            vol.Required("SN"): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
                 vol.All(
                     [vol.Coerce(float)],
-                    vol.Any(
-                        vol.Length(min=69, max=69),
-                        vol.Length(min=200, max=200),
-                    ),
+                    vol.Any(vol.Length(min=102, max=103), vol.Length(min=107, max=107)),
                 )
             ),
-            vol.Required("Information"): vol.Schema(
-                vol.Any(vol.Length(min=9, max=9), vol.Length(min=10, max=10))
-            ),
+            vol.Required("Information"): vol.Schema(vol.All(vol.Length(min=9, max=9))),
         },
         extra=vol.REMOVE_EXTRA,
     )
 
+    # pylint: disable=duplicate-code
     @classmethod
     def response_decoder(cls):
         return {
-            "Network Voltage": (0, Units.V, div10),
-            "Output Current": (1, Units.A, div10),
-            "AC Power": (2, Units.W),
-            "PV1 Voltage": (3, Units.V, div10),
-            "PV2 Voltage": (4, Units.V, div10),
-            "PV1 Current": (5, Units.A, div10),
-            "PV2 Current": (6, Units.A, div10),
-            "PV1 Power": (7, Units.W),
-            "PV2 Power": (8, Units.W),
-            "Grid Frequency": (9, Units.HZ, div100),
-            "Total Energy": (11, Total(Units.KWH), div10),
-            "Today's Energy": (13, Units.KWH, div10),
-            "Total Feed-in Energy": (41, Total(Units.KWH), div10),
-            "Total Consumption": (42, Total(Units.KWH), div10),
-            "Power Now": (43, Units.W, div10),
-            "Inverter Temperature": (55, Units.C),
+            "PV1 Current": (0, Units.A),
+            "PV2 Current": (1, Units.A),
+            "PV1 Voltage": (2, Units.V),
+            "PV2 Voltage": (3, Units.V),
+            "Output Current Phase 1": (4, Units.A),
+            "Network Voltage Phase 1": (5, Units.V),
+            "AC Power": (6, Units.W),
+            "Inverter Temperature": (7, Units.C),
+            "Today's Energy": (8, Units.KWH),
+            "Total Energy": (9, Total(Units.KWH)),
+            "Exported Power": (10, Units.W),
+            "PV1 Power": (11, Units.W),
+            "PV2 Power": (12, Units.W),
+            "Battery Voltage": (13, Units.V),
+            "Battery Current": (14, Units.A),
+            "Battery Power": (15, Units.W),
+            "Battery Temperature": (16, Units.C),
+            "Battery Remaining Capacity": (21, Units.PERCENT),
+            "Total Feed-in Energy": (41, Total(Units.KWH)),
+            "Total Consumption": (42, Total(Units.KWH)),
+            "Power Now Phase 1": (43, Units.W),
+            "Power Now Phase 2": (44, Units.W),
+            "Power Now Phase 3": (45, Units.W),
+            "Output Current Phase 2": (46, Units.A),
+            "Output Current Phase 3": (47, Units.A),
+            "Network Voltage Phase 2": (48, Units.V),
+            "Network Voltage Phase 3": (49, Units.V),
+            "Grid Frequency Phase 1": (50, Units.HZ),
+            "Grid Frequency Phase 2": (51, Units.HZ),
+            "Grid Frequency Phase 3": (52, Units.HZ),
+            "EPS Voltage": (53, Units.V),
+            "EPS Current": (54, Units.A),
+            "EPS Power": (55, Units.W),
+            "EPS Frequency": (56, Units.HZ),
         }
-
-    # pylint: enable=duplicate-code
```

### Comparing `solax-0.3.0/solax/inverters/x1_smart.py` & `solax-0.3.1/solax/inverters/x1_boost.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,79 @@
 import voluptuous as vol
-from solax.inverter import InverterPost
+
+from solax import utils
+from solax.inverter import Inverter, InverterHttpClient, Method, ResponseParser
 from solax.units import Total, Units
 from solax.utils import div10, div100, to_signed
 
 
-class X1Smart(InverterPost):
+class X1Boost(Inverter):
     """
-    X1-Smart with Pocket WiFi v2.033.20
+    X1-Boost with Pocket WiFi 2.034.06
     Includes X-Forwarded-For for direct LAN API access
     """
 
     # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
-            vol.Required("type", "type"): vol.All(int, 8),
+            vol.Required("type", "type"): vol.All(int, 4),
             vol.Required(
                 "sn",
             ): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
                 vol.All(
                     [vol.Coerce(float)],
                     vol.Length(min=200, max=200),
                 )
             ),
-            vol.Required("Information"): vol.Schema(vol.All(vol.Length(min=8, max=8))),
+            vol.Required("Information"): vol.Schema(
+                vol.All(vol.Length(min=10, max=10))
+            ),
         },
         extra=vol.REMOVE_EXTRA,
     )
 
     @classmethod
     def response_decoder(cls):
         return {
-            "Network Voltage": (0, Units.V, div10),
-            "Output Current": (1, Units.A, div10),
-            "AC Power": (2, Units.W),
+            "AC Voltage": (0, Units.V, div10),
+            "AC Output Current": (1, Units.A, div10),
+            "AC Output Power": (2, Units.W),
             "PV1 Voltage": (3, Units.V, div10),
             "PV2 Voltage": (4, Units.V, div10),
             "PV1 Current": (5, Units.A, div10),
             "PV2 Current": (6, Units.A, div10),
             "PV1 Power": (7, Units.W),
             "PV2 Power": (8, Units.W),
-            "Grid Frequency": (9, Units.HZ, div100),
-            "Total Energy": (11, Total(Units.KWH), div10),
-            "Today's Energy": (13, Units.KWH, div10),
+            "AC Frequency": (9, Units.HZ, div100),
+            "Total Generated Energy": (11, Total(Units.KWH), div10),
+            "Today's Generated Energy": (13, Total(Units.KWH), div10),
             "Inverter Temperature": (39, Units.C),
             "Exported Power": (48, Units.W, to_signed),
-            "Total Feed-in Energy": (50, Total(Units.KWH), div100),
-            "Total Consumption": (52, Total(Units.KWH), div100),
+            "Total Export Energy": (50, Total(Units.KWH), div100),
+            "Total Import Energy": (52, Total(Units.KWH), div100),
         }
 
     @classmethod
-    async def make_request(cls, host, port=80, pwd="", headers=None):
+    def _build(cls, host, port, pwd="", params_in_query=True):
+        url = utils.to_url(host, port)
+        http_client = InverterHttpClient(url, Method.POST, pwd)
+        if params_in_query:
+            http_client.with_default_query()
+        else:
+            http_client.with_default_data()
+
         headers = {"X-Forwarded-For": "5.8.8.8"}
-        return await super().make_request(host, port, pwd, headers=headers)
+        http_client.with_headers(headers)
+        schema = cls._schema
+        response_decoder = cls.response_decoder()
+        response_parser = ResponseParser(schema, response_decoder)
+        return cls(http_client, response_parser)
+
+    @classmethod
+    def build_all_variants(cls, host, port, pwd=""):
+        versions = [
+            cls._build(host, port, pwd, True),
+            cls._build(host, port, pwd, False),
+        ]
+        return versions
```

### Comparing `solax-0.3.0/solax/inverters/x3.py` & `solax-0.3.1/solax/inverters/x3_v34.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 import voluptuous as vol
-from solax.inverter import InverterPost
-from solax.units import Units, Total
-from solax.utils import startswith
 
+from solax.inverter import Inverter
+from solax.units import Total, Units
+from solax.utils import div10, div100, pack_u16, to_signed, twoway_div10, twoway_div100
 
-class X3(InverterPost):
+
+class X3V34(Inverter):
+    """X3 v2.034.06"""
+
+    # pylint: disable=duplicate-code
     _schema = vol.Schema(
         {
-            vol.Required("type"): vol.All(str, startswith("X3-")),
-            vol.Required("SN"): str,
+            vol.Required("type"): vol.All(int, 5),
+            vol.Required("sn"): str,
             vol.Required("ver"): str,
             vol.Required("Data"): vol.Schema(
                 vol.All(
                     [vol.Coerce(float)],
-                    vol.Any(vol.Length(min=102, max=103), vol.Length(min=107, max=107)),
+                    vol.Length(min=200, max=200),
                 )
             ),
-            vol.Required("Information"): vol.Schema(vol.All(vol.Length(min=9, max=9))),
+            vol.Required("Information"): vol.Schema(
+                vol.All(vol.Length(min=10, max=10))
+            ),
         },
         extra=vol.REMOVE_EXTRA,
     )
 
-    # pylint: disable=duplicate-code
     @classmethod
     def response_decoder(cls):
         return {
-            "PV1 Current": (0, Units.A),
-            "PV2 Current": (1, Units.A),
-            "PV1 Voltage": (2, Units.V),
-            "PV2 Voltage": (3, Units.V),
-            "Output Current Phase 1": (4, Units.A),
-            "Network Voltage Phase 1": (5, Units.V),
-            "AC Power": (6, Units.W),
-            "Inverter Temperature": (7, Units.C),
-            "Today's Energy": (8, Units.KWH),
-            "Total Energy": (9, Total(Units.KWH)),
-            "Exported Power": (10, Units.W),
-            "PV1 Power": (11, Units.W),
-            "PV2 Power": (12, Units.W),
-            "Battery Voltage": (13, Units.V),
-            "Battery Current": (14, Units.A),
-            "Battery Power": (15, Units.W),
-            "Battery Temperature": (16, Units.C),
-            "Battery Remaining Capacity": (21, Units.PERCENT),
-            "Total Feed-in Energy": (41, Total(Units.KWH)),
-            "Total Consumption": (42, Total(Units.KWH)),
-            "Power Now Phase 1": (43, Units.W),
-            "Power Now Phase 2": (44, Units.W),
-            "Power Now Phase 3": (45, Units.W),
-            "Output Current Phase 2": (46, Units.A),
-            "Output Current Phase 3": (47, Units.A),
-            "Network Voltage Phase 2": (48, Units.V),
-            "Network Voltage Phase 3": (49, Units.V),
-            "Grid Frequency Phase 1": (50, Units.HZ),
-            "Grid Frequency Phase 2": (51, Units.HZ),
-            "Grid Frequency Phase 3": (52, Units.HZ),
-            "EPS Voltage": (53, Units.V),
-            "EPS Current": (54, Units.A),
-            "EPS Power": (55, Units.W),
-            "EPS Frequency": (56, Units.HZ),
+            "Network Voltage Phase 1": (0, Units.V, div10),
+            "Network Voltage Phase 2": (1, Units.V, div10),
+            "Network Voltage Phase 3": (2, Units.V, div10),
+            "Output Current Phase 1": (3, Units.A, twoway_div10),
+            "Output Current Phase 2": (4, Units.A, twoway_div10),
+            "Output Current Phase 3": (5, Units.A, twoway_div10),
+            "Power Now Phase 1": (6, Units.W, to_signed),
+            "Power Now Phase 2": (7, Units.W, to_signed),
+            "Power Now Phase 3": (8, Units.W, to_signed),
+            "PV1 Voltage": (9, Units.V, div10),
+            "PV2 Voltage": (10, Units.V, div10),
+            "PV1 Current": (11, Units.A, div10),
+            "PV2 Current": (12, Units.A, div10),
+            "PV1 Power": (13, Units.W),
+            "PV2 Power": (14, Units.W),
+            "Total PV Energy": (pack_u16(89, 90), Total(Units.KWH), div10),
+            "Today's PV Energy": (112, Units.KWH, div10),
+            "Grid Frequency Phase 1": (15, Units.HZ, div100),
+            "Grid Frequency Phase 2": (16, Units.HZ, div100),
+            "Grid Frequency Phase 3": (17, Units.HZ, div100),
+            "Total Energy": (pack_u16(19, 20), Total(Units.KWH), div10),
+            "Today's Energy": (21, Units.KWH, div10),
+            "Battery Voltage": (24, Units.V, div100),
+            "Battery Current": (25, Units.A, twoway_div100),
+            "Battery Power": (26, Units.W, to_signed),
+            "Battery Temperature": (27, Units.C),
+            "Battery Remaining Capacity": (28, Units.PERCENT),
+            "Total Battery Discharge Energy": (
+                pack_u16(30, 31),
+                Total(Units.KWH),
+                div10,
+            ),
+            "Today's Battery Discharge Energy": (113, Units.KWH, div10),
+            "Battery Remaining Energy": (32, Units.KWH, div10),
+            "Total Battery Charge Energy": (
+                pack_u16(87, 88),
+                Total(Units.KWH),
+                div10,
+            ),
+            "Today's Battery Charge Energy": (114, Units.KWH, div10),
+            "Exported Power": (65, Units.W, to_signed),
+            "Total Feed-in Energy": (pack_u16(67, 68), Total(Units.KWH), div100),
+            "Total Consumption": (pack_u16(69, 70), Total(Units.KWH), div100),
+            "AC Power": (181, Units.W, to_signed),
+            "EPS Frequency": (63, Units.HZ, div100),
+            "EPS Total Energy": (pack_u16(110, 111), Units.KWH, div10),
         }
+
+    # pylint: enable=duplicate-code
```

### Comparing `solax-0.3.0/solax/units.py` & `solax-0.3.1/solax/units.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Units and different measrement types"""
+""" Units and different measurement types"""
 from enum import Enum
 from typing import NamedTuple, Union
 
 
 class Units(Enum):
     """All known Units."""
 
@@ -13,20 +13,20 @@
     C = "°C"
     HZ = "Hz"
     PERCENT = "%"
     NONE = ""
 
 
 class Measurement(NamedTuple):
-    """Respresention of measurement with a given unit and arbitrary values."""
+    """Representation of measurement with a given unit and arbitrary values."""
 
     unit: Units
     is_monotonic: bool = False
 
 
 class Total(Measurement):
-    """A Measuremeant where the values are continuously increasing."""
+    """A Measurement where the values are continuously increasing."""
 
     is_monotonic: bool = True
 
 
 SensorUnit = Union[Measurement, Total]
```

### Comparing `solax-0.3.0/solax/utils.py` & `solax-0.3.1/solax/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Protocol, Tuple
+
 from voluptuous import Invalid
 
 
 class Packer(Protocol):  # pragma: no cover
     # pylint: disable=R0903
     """
     Pack multiple raw values from the inverter
@@ -60,21 +61,32 @@
 
 
 def div100(val):
     return val / 100
 
 
 INT16_MAX = 0x7FFF
+INT32_MAX = 0x7FFFFFFF
 
 
 def to_signed(val):
     if val > INT16_MAX:
         val -= 2**16
     return val
 
 
+def to_signed32(val):
+    if val > INT32_MAX:
+        val -= 2**32
+    return val
+
+
 def twoway_div10(val):
     return to_signed(val) / 10
 
 
 def twoway_div100(val):
     return to_signed(val) / 100
+
+
+def to_url(host, port):
+    return f"http://{host}:{port}/"
```

### Comparing `solax-0.3.0/solax.egg-info/PKG-INFO` & `solax-0.3.1/solax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solax
-Version: 0.3.0
+Version: 0.3.1
 Summary: Solax inverter API client
 Home-page: https://github.com/squishykid/solax
 Author: Robin Wohlers-Reichel
 Author-email: me@robinwr.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solax-0.3.0/solax.egg-info/SOURCES.txt` & `solax-0.3.1/solax.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .gitignore
 LICENSE
 README.md
 mypy.ini
 setup.py
+verify.sh
 .github/workflows/publish.yml
 .github/workflows/tests.yaml
 solax/__init__.py
 solax/discovery.py
 solax/inverter.py
+solax/inverter_http_client.py
+solax/response_parser.py
 solax/units.py
 solax/utils.py
 solax.egg-info/PKG-INFO
 solax.egg-info/SOURCES.txt
 solax.egg-info/dependency_links.txt
 solax.egg-info/requires.txt
 solax.egg-info/top_level.txt
@@ -20,14 +23,15 @@
 solax/inverters/x1.py
 solax/inverters/x1_boost.py
 solax/inverters/x1_hybrid_gen4.py
 solax/inverters/x1_mini.py
 solax/inverters/x1_mini_v34.py
 solax/inverters/x1_smart.py
 solax/inverters/x3.py
+solax/inverters/x3_hybrid_g4.py
 solax/inverters/x3_v34.py
 solax/inverters/x_hybrid.py
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
 tests/test_base_inverter.py
 tests/test_discovery.py
```

### Comparing `solax-0.3.0/tests/fixtures.py` & `solax-0.3.1/tests/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from collections import namedtuple
+
 import pytest
+
 import solax.inverters as inverter
 from tests.samples.expected_values import (
     QVOLTHYBG33P_VALUES,
+    X1_BOOST_VALUES,
+    X1_HYBRID_G4_VALUES,
     X1_MINI_VALUES,
     X1_MINI_VALUES_V34,
     X1_SMART_VALUES,
     X1_VALUES,
+    X3_HYBRID_G4_VALUES,
     X3_HYBRID_VALUES,
     X3_VALUES,
     X3V34_HYBRID_VALUES,
     X3V34_HYBRID_VALUES_EPS_MODE,
     X3V34_HYBRID_VALUES_NEGATIVE_POWER,
     XHYBRID_VALUES,
-    X1_BOOST_VALUES,
-    X1_HYBRID_G4_VALUES,
 )
 from tests.samples.responses import (
     QVOLTHYBG33P_RESPONSE_V34,
     X1_BOOST_AIR_MINI_RESPONSE,
+    X1_BOOST_RESPONSE,
     X1_HYBRID_G3_2X_MPPT_RESPONSE,
     X1_HYBRID_G3_RESPONSE,
     X1_HYBRID_G4_RESPONSE,
     X1_MINI_RESPONSE_V34,
     X1_SMART_RESPONSE,
     X3_HYBRID_G3_2X_MPPT_RESPONSE,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34_EPS_MODE,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34_NEGATIVE_POWER,
     X3_HYBRID_G3_RESPONSE,
+    X3_HYBRID_G4_RESPONSE,
     X3_MIC_RESPONSE,
     XHYBRID_DE01_RESPONSE,
     XHYBRID_DE02_RESPONSE,
-    X1_BOOST_RESPONSE,
 )
 
 X_FORWARDED_HEADER = {"X-Forwarded-For": "5.8.8.8"}
 
 
 @pytest.fixture()
 def simple_http_fixture(httpserver):
@@ -201,14 +205,24 @@
         values=X3V34_HYBRID_VALUES_EPS_MODE,
         headers=None,
         data=None,
     ),
     InverterUnderTest(
         uri="/",
         method="POST",
+        query_string=None,
+        response=X3_HYBRID_G4_RESPONSE,
+        inverter=inverter.X3HybridG4,
+        values=X3_HYBRID_G4_VALUES,
+        headers=None,
+        data="optType=ReadRealTimeData",
+    ),
+    InverterUnderTest(
+        uri="/",
+        method="POST",
         query_string="",
         response=QVOLTHYBG33P_RESPONSE_V34,
         inverter=inverter.QVOLTHYBG33P,
         values=QVOLTHYBG33P_VALUES,
         headers=None,
         data=None,
     ),
```

### Comparing `solax-0.3.0/tests/samples/expected_values.py` & `solax-0.3.1/tests/samples/expected_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,55 @@
     "Total Feed-in Energy": 3174.83,
     "Total Consumption": 844.58,
     "AC Power": 0,
     "EPS Frequency": 50,
     "EPS Total Energy": 1.7,
 }
 
+X3_HYBRID_G4_VALUES = {
+    "Grid 1 Voltage": 238.3,
+    "Grid 2 Voltage": 239.7,
+    "Grid 3 Voltage": 237.7,
+    "Grid 1 Current": 1.0,
+    "Grid 2 Current": 1.1,
+    "Grid 3 Current": 1.1,
+    "Grid 1 Power": 33.0,
+    "Grid 2 Power": 81.0,
+    "Grid 3 Power": 76.0,
+    "PV1 Voltage": 248.3,
+    "PV2 Voltage": 230.5,
+    "PV1 Current": 0.1,
+    "PV2 Current": 0.2,
+    "PV1 Power": 45.0,
+    "PV2 Power": 58.0,
+    "Grid 1 Frequency": 50.01,
+    "Grid 2 Frequency": 50.01,
+    "Grid 3 Frequency": 50.01,
+    "Run mode": 2.0,
+    "Run mode text": "Normal",
+    "EPS 1 Voltage": 0.0,
+    "EPS 2 Voltage": 0.0,
+    "EPS 3 Voltage": 0.0,
+    "EPS 1 Current": 0.0,
+    "EPS 2 Current": 0.0,
+    "EPS 3 Current": 0.0,
+    "EPS 1 Power": 0.0,
+    "EPS 2 Power": 0.0,
+    "EPS 3 Power": 0.0,
+    "Feed-in Power ": -152.0,
+    "Battery Power": 0.0,
+    "Yield total": 4.4,
+    "Yield today": 0.1,
+    "Feed-in Energy": 0.0,
+    "Consumed Energy": 20.09,
+    "Battery Remaining Capacity": 30.0,
+    "Battery Temperature": 22.0,
+    "Battery Voltage": 234.6,
+}
+
 X1_VALUES = {
     "PV1 Current": 0,
     "PV2 Current": 1,
     "PV1 Voltage": 2,
     "PV2 Voltage": 3,
     "Output Current": 4,
     "Network Voltage": 5,
```

### Comparing `solax-0.3.0/tests/samples/responses.py` & `solax-0.3.1/tests/samples/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -2293,14 +2293,323 @@
         0,
         0,
         0,
     ],
     "Information": [8.000, 5, "XXXXXXXX", 1, 4.60, 0.00, 4.42, 1.05, 0.00, 1],
 }
 
+X3_HYBRID_G4_RESPONSE = {
+    "sn": "SR3xxxxxxx",
+    "ver": "3.006.04",
+    "type": 14,
+    "Data": [
+        2383,
+        2397,
+        2377,
+        10,
+        11,
+        11,
+        33,
+        81,
+        76,
+        190,
+        2483,
+        2305,
+        1,
+        2,
+        45,
+        58,
+        5001,
+        5001,
+        5001,
+        2,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        1,
+        65384,
+        65535,
+        0,
+        0,
+        0,
+        23460,
+        0,
+        0,
+        2349,
+        65534,
+        65490,
+        1,
+        37,
+        342,
+        256,
+        10542,
+        4616,
+        5644,
+        100,
+        0,
+        23,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        44,
+        0,
+        1,
+        0,
+        0,
+        0,
+        24,
+        0,
+        10,
+        0,
+        0,
+        0,
+        34,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        2009,
+        0,
+        0,
+        0,
+        209,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        1,
+        30,
+        1,
+        22,
+        33,
+        256,
+        2628,
+        1800,
+        250,
+        350,
+        163,
+        149,
+        33,
+        32,
+        1,
+        1115,
+        256,
+        9252,
+        9252,
+        0,
+        0,
+        0,
+        0,
+        3252,
+        3232,
+        13925,
+        0,
+        21302,
+        14389,
+        18757,
+        12855,
+        16689,
+        12355,
+        13363,
+        21302,
+        14389,
+        18757,
+        12855,
+        16689,
+        12355,
+        13363,
+        21302,
+        14389,
+        18758,
+        12855,
+        16691,
+        12611,
+        12341,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        2817,
+        3842,
+        258,
+        771,
+        0,
+        23460,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+    ],
+    "Information": [10.000, 14, "H34A**********", 8, 1.23, 0.00, 1.24, 1.09, 0.00, 1],
+}
+
 QVOLTHYBG33P_RESPONSE_V34 = {
     "sn": "SWX***",
     "ver": "2.034.06",
     "type": 14,
     "Data": [
         2214,
         2238,
```

### Comparing `solax-0.3.0/tests/test_discovery.py` & `solax-0.3.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.0/tests/test_smoke.py` & `solax-0.3.1/tests/test_smoke.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import pytest
+
 import solax
-from solax.inverter import InverterError
 from solax.discovery import REGISTRY
+from solax.inverter import Inverter, InverterError
 from solax.units import Measurement
 from tests import fixtures
 
 
+async def build_right_variant(inverter, conn) -> Inverter:
+    last_error: BaseException = BaseException("anticipating errors")
+    for i in inverter.build_all_variants(*conn):
+        try:
+            await i.get_data()
+            return i
+        except InverterError as ex:
+            last_error = ex
+    raise last_error
+
+
 @pytest.mark.asyncio
 async def test_smoke(inverters_fixture):
     conn, inverter_class, values = inverters_fixture
-    inv = inverter_class(*conn)
+    inv = await build_right_variant(inverter_class, conn)
     rt_api = solax.RealTimeAPI(inv)
     parsed = await rt_api.get_data()
 
     msg = "data size should match expected values"
     assert len(values) == len(parsed.data), msg
     for sensor, value in values.items():
         assert (
@@ -21,15 +33,15 @@
         ), f"{sensor}: expected {value} but got {parsed.data[sensor]}"
 
 
 @pytest.mark.asyncio
 async def test_throws_when_unable_to_parse(inverters_garbage_fixture):
     conn, inverter_class = inverters_garbage_fixture
     with pytest.raises(InverterError):
-        i = inverter_class(*conn)
+        i = await build_right_variant(inverter_class, conn)
         await i.get_data()
 
 
 def test_registry_matches_inverters_under_test():
     test_inverters = {i.inverter for i in fixtures.INVERTERS_UNDER_TEST}
     registry_inverters = set(REGISTRY)
     assert test_inverters == registry_inverters, "tests do not match registry"
```

### Comparing `solax-0.3.0/tests/test_solax.py` & `solax-0.3.1/tests/test_solax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from unittest.mock import Mock
 import asyncio
+from unittest.mock import Mock
+
 import pytest
+
 import solax
 
 
 @pytest.mark.asyncio
 async def test_waits_when_asked(monkeypatch):
     sleep_f = asyncio.Future()
     sleep_f.set_result(None)
```

