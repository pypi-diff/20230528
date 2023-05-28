# Comparing `tmp/FlightRadarAPI-1.2.7.tar.gz` & `tmp/FlightRadarAPI-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.2.7.tar", last modified: Mon Apr  3 15:54:17 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.2.8.tar", last modified: Sun May 28 20:11:57 2023, max compression
```

## Comparing `FlightRadarAPI-1.2.7.tar` & `FlightRadarAPI-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 15:54:17.639079 FlightRadarAPI-1.2.7/
-drwxrwxrwx   0        0        0        0 2023-04-03 15:54:17.624574 FlightRadarAPI-1.2.7/FlightRadar24/
--rw-rw-rw-   0        0        0      469 2023-04-03 15:53:24.000000 FlightRadarAPI-1.2.7/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     5962 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2048 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/FlightRadar24/core.py
--rw-rw-rw-   0        0        0     9199 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     1753 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:54:17.639079 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3138 2023-04-03 15:54:17.000000 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-03 15:54:17.000000 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 15:54:17.000000 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-03 15:54:17.000000 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-03 15:54:17.000000 FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/LICENSE
--rw-rw-rw-   0        0        0     3138 2023-04-03 15:54:17.639079 FlightRadarAPI-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2467 2023-04-03 15:49:14.000000 FlightRadarAPI-1.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-03 15:54:17.639079 FlightRadarAPI-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.943747 FlightRadarAPI-1.2.8/
+drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.928744 FlightRadarAPI-1.2.8/FlightRadar24/
+-rw-rw-rw-   0        0        0      469 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     5840 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2048 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0     9199 2023-03-19 22:45:09.000000 FlightRadarAPI-1.2.8/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     1753 2023-03-19 22:52:21.000000 FlightRadarAPI-1.2.8/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.942740 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3138 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3138 2023-05-28 20:11:57.942740 FlightRadarAPI-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2467 2023-01-29 02:09:37.000000 FlightRadarAPI-1.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 20:11:57.943747 FlightRadarAPI-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/setup.py
```

### Comparing `FlightRadarAPI-1.2.7/FlightRadar24/api.py` & `FlightRadarAPI-1.2.8/FlightRadar24/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,23 +73,22 @@
         request = APIRequest(Core.airports_data_url, headers = Core.json_headers)
         return request.get_content()["rows"]
 
     def get_bounds(self, zone: Dict[str, float]) -> str:
         # Convert coordinate dictionary (tl_y, tl_x, br_y, br_x) to string "y1, y2, x1, x2".
         return "{},{},{},{}".format(zone["tl_y"], zone["br_y"] , zone["tl_x"], zone["br_x"])
 
-    @deprecated(version='1.2.1', reason="Sometimes, the FlightRadar24 route used by this method doesn't work")
     def get_country_flag(self, country: str) -> str:
         # Get the country flag image URL.
         flag_url = Core.country_flag_url.format(country.lower().replace(" ", "-"))
 
         headers = Core.image_headers.copy()
         
         if "origin" in headers:
-            headers = headers.pop("origin") # Doesn't work for this request
+            headers.pop("origin") # Doesn't work for this request
 
         # Check if there is a problem with the request. If not, the URL is returned.
         status_code = APIRequest(flag_url, headers = headers).get_status_code()
         if not str(status_code).startswith("4"): return flag_url
 
     def get_flight_details(self, flight_id: str) -> Dict:
         # Get the flight details from Data Live Flightradar24.
```

### Comparing `FlightRadarAPI-1.2.7/FlightRadar24/core.py` & `FlightRadarAPI-1.2.8/FlightRadar24/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # Airlines data URL.
     airlines_data_url = flightradar_base_url + "/_json/airlines.php"
 
     # Zones data URL.
     zones_data_url = flightradar_base_url + "/js/zones.js.php"
 
     # Country flag image URL.
-    country_flag_url = flightradar_base_url + "/static/images/data/flags-small/{}.gif"
+    country_flag_url = flightradar_base_url + "/static/images/data/flags-small/{}.svg"
 
     # Airline logo image URL.
     airline_logo_url = cdn_flightradar_base_url + "/assets/airlines/logotypes/{}_{}.png"
     alternative_airline_logo_url = flightradar_base_url + "/static/images/data/operators/{}_logo0.png"
 
     headers = {
         "accept-encoding": "gzip, br",
```

### Comparing `FlightRadarAPI-1.2.7/FlightRadar24/flight.py` & `FlightRadarAPI-1.2.8/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.7/FlightRadar24/request.py` & `FlightRadarAPI-1.2.8/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.7/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.2.7
+Version: 1.2.8
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.2.7/LICENSE` & `FlightRadarAPI-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.7/PKG-INFO` & `FlightRadarAPI-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.2.7
+Version: 1.2.8
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.2.7/README.md` & `FlightRadarAPI-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.7/setup.py` & `FlightRadarAPI-1.2.8/setup.py`

 * *Files identical despite different names*

