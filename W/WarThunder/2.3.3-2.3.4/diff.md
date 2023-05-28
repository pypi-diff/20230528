# Comparing `tmp/WarThunder-2.3.3.tar.gz` & `tmp/WarThunder-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WarThunder-2.3.3.tar", last modified: Thu Mar 30 02:23:03 2023, max compression
+gzip compressed data, was "WarThunder-2.3.4.tar", last modified: Sun May 28 02:54:41 2023, max compression
```

## Comparing `WarThunder-2.3.3.tar` & `WarThunder-2.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 02:23:03.912697 WarThunder-2.3.3/
--rw-rw-rw-   0        0        0    10550 2023-03-30 02:23:03.913017 WarThunder-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     9793 2023-03-30 02:22:30.000000 WarThunder-2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 02:23:03.903190 WarThunder-2.3.3/WarThunder/
--rw-rw-rw-   0        0        0       17 2023-03-30 02:22:30.000000 WarThunder-2.3.3/WarThunder/__init__.py
--rw-rw-rw-   0        0        0     6856 2023-03-30 02:22:30.000000 WarThunder-2.3.3/WarThunder/acmi.py
--rw-rw-rw-   0        0        0      280 2023-03-30 02:22:30.000000 WarThunder-2.3.3/WarThunder/general.py
--rw-rw-rw-   0        0        0    25651 2023-03-30 02:22:30.000000 WarThunder-2.3.3/WarThunder/mapinfo.py
--rw-rw-rw-   0        0        0    12480 2023-03-30 02:22:30.000000 WarThunder-2.3.3/WarThunder/maps.py
--rw-rw-rw-   0        0        0     9347 2023-03-30 02:22:32.000000 WarThunder-2.3.3/WarThunder/telemetry.py
-drwxrwxrwx   0        0        0        0 2023-03-30 02:23:03.911697 WarThunder-2.3.3/WarThunder.egg-info/
--rw-rw-rw-   0        0        0    10550 2023-03-30 02:23:03.000000 WarThunder-2.3.3/WarThunder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-30 02:23:03.000000 WarThunder-2.3.3/WarThunder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 02:23:03.000000 WarThunder-2.3.3/WarThunder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-03-30 02:23:03.000000 WarThunder-2.3.3/WarThunder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-30 02:23:03.000000 WarThunder-2.3.3/WarThunder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-30 02:23:03.913017 WarThunder-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-03-30 02:22:32.000000 WarThunder-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 02:54:41.159569 WarThunder-2.3.4/
+-rw-rw-rw-   0        0        0    10526 2023-05-28 02:54:41.159569 WarThunder-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9810 2023-05-28 02:54:21.000000 WarThunder-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 02:54:41.155190 WarThunder-2.3.4/WarThunder/
+-rw-rw-rw-   0        0        0       17 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/__init__.py
+-rw-rw-rw-   0        0        0     6856 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/acmi.py
+-rw-rw-rw-   0        0        0      280 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/general.py
+-rw-rw-rw-   0        0        0    25766 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/mapinfo.py
+-rw-rw-rw-   0        0        0    12480 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/maps.py
+-rw-rw-rw-   0        0        0     9347 2023-05-28 02:54:21.000000 WarThunder-2.3.4/WarThunder/telemetry.py
+drwxrwxrwx   0        0        0        0 2023-05-28 02:54:41.158569 WarThunder-2.3.4/WarThunder.egg-info/
+-rw-rw-rw-   0        0        0    10526 2023-05-28 02:54:41.000000 WarThunder-2.3.4/WarThunder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-28 02:54:41.000000 WarThunder-2.3.4/WarThunder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 02:54:41.000000 WarThunder-2.3.4/WarThunder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-28 02:54:41.000000 WarThunder-2.3.4/WarThunder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 02:54:41.000000 WarThunder-2.3.4/WarThunder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-28 02:54:41.160570 WarThunder-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-05-28 02:54:21.000000 WarThunder-2.3.4/setup.py
```

### Comparing `WarThunder-2.3.3/PKG-INFO` & `WarThunder-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: WarThunder
-Version: 2.3.3
+Version: 2.3.4
 Summary: Python package used to access air vehicle telemetry while in War Thunder air battles
 Home-page: https://github.com/PowerBroker2/WarThunder
-Download-URL: https://github.com/PowerBroker2/WarThunder/archive/2.3.3.tar.gz
+Download-URL: https://github.com/PowerBroker2/WarThunder/archive/2.3.4.tar.gz
 Author: Power_Broker
 Author-email: gitstuff2@gmail.com
-License: UNKNOWN
 Keywords: War Thunder
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 [![GitHub version](https://badge.fury.io/gh/PowerBroker2%2FWarThunder.svg)](https://badge.fury.io/gh/PowerBroker2%2FWarThunder) [![PyPI version](https://badge.fury.io/py/WarThunder.svg)](https://badge.fury.io/py/WarThunder)
 
 # Overview
 Python package to access vehicle telemetry and match data in real-time while in War Thunder air battles (NOT tanks). Here are some things you can access/do with this package:
 - Get telemetry information on your vehicle and others identified on user's mini map
@@ -113,18 +111,18 @@
     else:
         print('\tNone')
     print('')
 
 def find_bomb_points(friendly=True):
     if friendly:
         print('Friendly Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.defend_points() if obj.friendly]
     else:
         print('Enemy Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if not obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.bombing_points() if not obj.friendly]
     
     if bomb_points:
         for bomb_point in bomb_points:
             print('\tBombing Point: {}'.format(bomb_point.position_ll))
     else:
         print('\tNone')
     print(' ')
@@ -310,9 +308,7 @@
 {'damage': [{'enemy': False,
              'id': 1,
              'mode': '',
              'msg': 'yn1/error/82220002',
              'sender': ''}],
  'events': []}
  ```
-
-
```

### Comparing `WarThunder-2.3.3/README.md` & `WarThunder-2.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,18 +100,18 @@
     else:
         print('\tNone')
     print('')
 
 def find_bomb_points(friendly=True):
     if friendly:
         print('Friendly Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.defend_points() if obj.friendly]
     else:
         print('Enemy Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if not obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.bombing_points() if not obj.friendly]
     
     if bomb_points:
         for bomb_point in bomb_points:
             print('\tBombing Point: {}'.format(bomb_point.position_ll))
     else:
         print('\tNone')
     print(' ')
```

### Comparing `WarThunder-2.3.3/WarThunder/acmi.py` & `WarThunder-2.3.4/WarThunder/acmi.py`

 * *Files identical despite different names*

### Comparing `WarThunder-2.3.3/WarThunder/mapinfo.py` & `WarThunder-2.3.4/WarThunder/mapinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,14 @@
         self.east_end       = [0, 0] # ONLY for airfield
         
         self.position_ll   = [0, 0] # NOT for airfield
         self.south_end_ll  = [0, 0] # ONLY for airfield
         self.east_end_ll   = [0, 0] # ONLY for airfield
         self.runway_dir    = 0      # ONLY for airfield
         self.airfield      = False
-        self.base          = False
         self.heavy_tank    = False
         self.medium_tank   = False
         self.light_tank    = False
         self.spg           = False
         self.spaa          = False
         self.wheeled       = False # AI only
         self.tracked       = False # AI only
@@ -250,14 +249,15 @@
         self.ship          = False
         self.torpedo_boat  = False
         self.tank_respawn  = False
         self.bomber_respawn  = False
         self.fighter_respawn = False
         self.capture_zone  = False
         self.defend_point  = False
+        self.bombing_point = False
         
         self.hdg = 0
         
         if map_obj_entry:
             self.update(map_obj_entry, map_size, ULHC_lat, ULHC_lon)
     
     def update(self, map_obj_entry: dict, map_size: float, ULHC_lat: float, ULHC_lon: float):
@@ -308,17 +308,18 @@
                
         if self.type.lower() == 'airfield':
             self.airfield = True
         else:
             self.airfield = False
             
         if self.icon.lower() == 'bombing_point':
-            self.base = True
+            self.bombing_point = True
+            self.friendly      = False
         else:
-            self.base = False
+            self.bombing_point = False
         
         if self.icon.lower() == 'heavytank':
             self.heavy_tank = True
         else:
             self.heavy_tank = False
         
         if self.icon.lower() == 'mediumtank':
@@ -399,14 +400,15 @@
         if self.icon.lower() == 'capture_zone':
             self.capture_zone = True
         else:
             self.capture_zone = False
         
         if self.icon.lower() == 'defending_point':
             self.defend_point = True
+            self.friendly     = True
         else:
             self.defend_point = False
         
         try:
             self.position = [map_obj_entry['x'], map_obj_entry['y']]
         except KeyError:
             self.position = [0, 0]
@@ -554,23 +556,23 @@
         
         Returns:
                 List of map_objs of found airfields
         '''
         
         return [obj for obj in self.map_objs if obj.airfield]
     
-    def bases(self) -> list:
+    def bombing_points(self) -> list:
         '''
-        Return a list of map_objs that includes all bases (bomb points) currently in the match
+        Return a list of map_objs that includes all bomb points currently in the match
         
         Returns:
-                List of map_objs of found bases 
+                List of map_objs of found bombing points 
         '''
         
-        return [obj for obj in self.map_objs if obj.base]
+        return [obj for obj in self.map_objs if obj.bombing_point]
     
     def heavy_tanks(self) -> list:
         '''
         Return a list of map_objs that includes all heavy tanks currently in the match
         
         Returns:
                 List of map_objs of found heavy tanks
```

### Comparing `WarThunder-2.3.3/WarThunder/maps.py` & `WarThunder-2.3.4/WarThunder/maps.py`

 * *Files identical despite different names*

### Comparing `WarThunder-2.3.3/WarThunder/telemetry.py` & `WarThunder-2.3.4/WarThunder/telemetry.py`

 * *Files identical despite different names*

### Comparing `WarThunder-2.3.3/WarThunder.egg-info/PKG-INFO` & `WarThunder-2.3.4/WarThunder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: WarThunder
-Version: 2.3.3
+Version: 2.3.4
 Summary: Python package used to access air vehicle telemetry while in War Thunder air battles
 Home-page: https://github.com/PowerBroker2/WarThunder
-Download-URL: https://github.com/PowerBroker2/WarThunder/archive/2.3.3.tar.gz
+Download-URL: https://github.com/PowerBroker2/WarThunder/archive/2.3.4.tar.gz
 Author: Power_Broker
 Author-email: gitstuff2@gmail.com
-License: UNKNOWN
 Keywords: War Thunder
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 [![GitHub version](https://badge.fury.io/gh/PowerBroker2%2FWarThunder.svg)](https://badge.fury.io/gh/PowerBroker2%2FWarThunder) [![PyPI version](https://badge.fury.io/py/WarThunder.svg)](https://badge.fury.io/py/WarThunder)
 
 # Overview
 Python package to access vehicle telemetry and match data in real-time while in War Thunder air battles (NOT tanks). Here are some things you can access/do with this package:
 - Get telemetry information on your vehicle and others identified on user's mini map
@@ -113,18 +111,18 @@
     else:
         print('\tNone')
     print('')
 
 def find_bomb_points(friendly=True):
     if friendly:
         print('Friendly Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.defend_points() if obj.friendly]
     else:
         print('Enemy Bomb Points:')
-        bomb_points = [obj for obj in telem.map_info.bases() if not obj.friendly]
+        bomb_points = [obj for obj in telem.map_info.bombing_points() if not obj.friendly]
     
     if bomb_points:
         for bomb_point in bomb_points:
             print('\tBombing Point: {}'.format(bomb_point.position_ll))
     else:
         print('\tNone')
     print(' ')
@@ -310,9 +308,7 @@
 {'damage': [{'enemy': False,
              'id': 1,
              'mode': '',
              'msg': 'yn1/error/82220002',
              'sender': ''}],
  'events': []}
  ```
-
-
```

### Comparing `WarThunder-2.3.3/setup.py` & `WarThunder-2.3.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name             = 'WarThunder',
     packages         = ['WarThunder'],
-    version          = '2.3.3',
+    version          = '2.3.4',
     description      = 'Python package used to access air vehicle telemetry while in War Thunder air battles',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author           = 'Power_Broker',
     author_email     = 'gitstuff2@gmail.com',
     url              = 'https://github.com/PowerBroker2/WarThunder',
-    download_url     = 'https://github.com/PowerBroker2/WarThunder/archive/2.3.3.tar.gz',
+    download_url     = 'https://github.com/PowerBroker2/WarThunder/archive/2.3.4.tar.gz',
     keywords         = ['War Thunder'],
     classifiers      = [],
     install_requires = ['imagehash', 'requests', 'Pillow', 'simplejson']
 )
```

