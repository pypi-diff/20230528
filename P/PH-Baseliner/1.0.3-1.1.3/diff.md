# Comparing `tmp/PH-Baseliner-1.0.3.tar.gz` & `tmp/PH-Baseliner-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-Baseliner-1.0.3.tar", last modified: Mon May  1 15:44:42 2023, max compression
+gzip compressed data, was "dist/PH-Baseliner-1.1.3.tar", last modified: Sun May 28 15:41:44 2023, max compression
```

## Comparing `PH-Baseliner-1.0.3.tar` & `PH-Baseliner-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PH_Baseliner.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2524 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PH_Baseliner.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      616 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PH_Baseliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PH_Baseliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PH_Baseliner.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2524 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/README.md
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/ph_baseliner/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/
--rw-r--r--   0 runner     (501) staff       (20)    12440 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/ECCCNYS_2020.json
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2071 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/lighting_space_types.py
--rw-r--r--   0 runner     (501) staff       (20)     7415 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/model.py
--rw-r--r--   0 runner     (501) staff       (20)      764 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/codes/options.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4264 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1776 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/components.py
--rw-r--r--   0 runner     (501) staff       (20)     1664 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     5540 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/u_values.py
--rw-r--r--   0 runner     (501) staff       (20)     5123 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/ph_baseliner/phpp/windows.py
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      839 2023-05-01 15:44:42.000000 PH-Baseliner-1.0.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-05-01 15:43:13.000000 PH-Baseliner-1.0.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      616 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/
+-rw-r--r--   0 runner     (501) staff       (20)    13031 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/ECCCNYS_2020.json
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2071 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/lighting_space_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    17467 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/options.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4647 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1776 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     1664 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     5549 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)     4952 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/windows.py
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      839 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/setup.py
```

### Comparing `PH-Baseliner-1.0.3/.github/workflows/ci.yaml` & `PH-Baseliner-1.1.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/LICENSE` & `PH-Baseliner-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/PH_Baseliner.egg-info/PKG-INFO` & `PH-Baseliner-1.1.3/PH_Baseliner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.0.3
+Version: 1.1.3
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
@@ -36,15 +36,15 @@
         Note: The baseliner will change the values of the PHPP file, and so you should 
         be sure to make a backup copy before using this tool.
         
         - - - 
         ![Tests](https://github.com/PH-Tools/PHX/actions/workflows/ci.yaml/badge.svg )
         ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
         [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
-        
+        ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `PH-Baseliner-1.0.3/PH_Baseliner.egg-info/SOURCES.txt` & `PH-Baseliner-1.1.3/PH_Baseliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/PKG-INFO` & `PH-Baseliner-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.0.3
+Version: 1.1.3
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
@@ -36,15 +36,15 @@
         Note: The baseliner will change the values of the PHPP file, and so you should 
         be sure to make a backup copy before using this tool.
         
         - - - 
         ![Tests](https://github.com/PH-Tools/PHX/actions/workflows/ci.yaml/badge.svg )
         ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
         [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
-        
+        ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `PH-Baseliner-1.0.3/README.md` & `PH-Baseliner-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 Note: The baseliner will change the values of the PHPP file, and so you should 
 be sure to make a backup copy before using this tool.
 
 - - - 
 ![Tests](https://github.com/PH-Tools/PHX/actions/workflows/ci.yaml/badge.svg )
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
+![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
```

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/codes/ECCCNYS_2020.json` & `PH-Baseliner-1.1.3/ph_baseliner/codes/ECCCNYS_2020.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'tables'": "{'fenestration_u_factors': {'fixed_windows': {'shgc': {'CZ4': {replace: "*

 * *             "OrderedDict([('pf_under_20', 0.36), ('pf_20_to_50', 0.43), ('pf_over_50', 0.58)])}, "*

 * *             "'CZ5': {replace: OrderedDict([('pf_under_20', 0.38), ('pf_20_to_50', 0.46), "*

 * *             "('pf_over_50', 0.48)])}, 'CZ6': {replace: OrderedDict([('pf_under_20', 0.4), "*

 * *             "('pf_20_to_50', 0.48), ('pf_over_50', 0.64)])}}}, 'operable_windows': {'shgc': "*

 * *             "{'CZ4': {replace: OrderedDict( […]*

```diff
@@ -12,24 +12,27 @@
     "source_url": "https://up.codes/viewer/new_york/ny-energy-conservation-code-2020",
     "state": "NY",
     "tables": {
         "fenestration_u_factors": {
             "entrance_doors": {
                 "shgc": {
                     "CZ4": {
-                        "all_other": 0.43,
-                        "group_r": 0.43
+                        "pf_20_to_50": 0.43,
+                        "pf_over_50": 0.58,
+                        "pf_under_20": 0.36
                     },
                     "CZ5": {
-                        "all_other": 0.46,
-                        "group_r": 0.46
+                        "pf_20_to_50": 0.46,
+                        "pf_over_50": 0.48,
+                        "pf_under_20": 0.38
                     },
                     "CZ6": {
-                        "all_other": 0.48,
-                        "group_r": 0.48
+                        "pf_20_to_50": 0.48,
+                        "pf_over_50": 0.64,
+                        "pf_under_20": 0.4
                     }
                 },
                 "u_factors": {
                     "CZ4": {
                         "all_other": 0.77,
                         "group_r": 0.77
                     },
@@ -42,24 +45,27 @@
                         "group_r": 0.77
                     }
                 }
             },
             "fixed_windows": {
                 "shgc": {
                     "CZ4": {
-                        "all_other": 0.43,
-                        "group_r": 0.43
+                        "pf_20_to_50": 0.43,
+                        "pf_over_50": 0.58,
+                        "pf_under_20": 0.36
                     },
                     "CZ5": {
-                        "all_other": 0.46,
-                        "group_r": 0.46
+                        "pf_20_to_50": 0.46,
+                        "pf_over_50": 0.48,
+                        "pf_under_20": 0.38
                     },
                     "CZ6": {
-                        "all_other": 0.48,
-                        "group_r": 0.48
+                        "pf_20_to_50": 0.48,
+                        "pf_over_50": 0.64,
+                        "pf_under_20": 0.4
                     }
                 },
                 "u_factors": {
                     "CZ4": {
                         "all_other": 0.38,
                         "group_r": 0.38
                     },
@@ -73,24 +79,27 @@
                     }
                 }
             },
             "name": "Building Envelope Fenestration Maximum U-Factor and SHGC Requirements",
             "operable_windows": {
                 "shgc": {
                     "CZ4": {
-                        "all_other": 0.43,
-                        "group_r": 0.43
+                        "pf_20_to_50": 0.43,
+                        "pf_over_50": 0.58,
+                        "pf_under_20": 0.36
                     },
                     "CZ5": {
-                        "all_other": 0.46,
-                        "group_r": 0.46
+                        "pf_20_to_50": 0.46,
+                        "pf_over_50": 0.48,
+                        "pf_under_20": 0.38
                     },
                     "CZ6": {
-                        "all_other": 0.48,
-                        "group_r": 0.48
+                        "pf_20_to_50": 0.48,
+                        "pf_over_50": 0.64,
+                        "pf_under_20": 0.4
                     }
                 },
                 "u_factors": {
                     "CZ4": {
                         "all_other": 0.45,
                         "group_r": 0.45
                     },
@@ -104,24 +113,27 @@
                     }
                 }
             },
             "section": "C402.4",
             "skylights": {
                 "shgc": {
                     "CZ4": {
-                        "all_other": 0.4,
-                        "group_r": 0.4
+                        "pf_20_to_50": 0.4,
+                        "pf_over_50": 0.4,
+                        "pf_under_20": 0.4
                     },
                     "CZ5": {
-                        "all_other": 0.4,
-                        "group_r": 0.4
+                        "pf_20_to_50": 0.4,
+                        "pf_over_50": 0.4,
+                        "pf_under_20": 0.4
                     },
                     "CZ6": {
-                        "all_other": 0.4,
-                        "group_r": 0.4
+                        "pf_20_to_50": 0.4,
+                        "pf_over_50": 0.4,
+                        "pf_under_20": 0.4
                     }
                 },
                 "u_factors": {
                     "CZ4": {
                         "all_other": 0.5,
                         "group_r": 0.5
                     },
```

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/codes/lighting_space_types.py` & `PH-Baseliner-1.1.3/ph_baseliner/codes/lighting_space_types.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/phpp/areas.py` & `PH-Baseliner-1.1.3/ph_baseliner/phpp/areas.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,81 +4,114 @@
 """Functions for setting the PHPP envelope constructions to the baseline values. """
 
 from PHX.PHPP import phpp_app
 from PHX.PHPP.phpp_model.areas_surface import ExistingSurfaceRow
 from PHX.model.enums.building import ComponentFaceType, ComponentExposureExterior
 
 from ph_baseliner.codes.model import BaselineCode
-from ph_baseliner.codes.options import ClimateZones
-from ph_baseliner.phpp.u_values import (create_baseline_constructions, 
-            add_baseline_constructions_to_phpp, BaselineConstructionPHPPids)
+from ph_baseliner.codes.options import ClimateZones, Use_Groups
+from ph_baseliner.phpp.u_values import (
+    create_baseline_constructions,
+    add_baseline_constructions_to_phpp,
+    BaselineConstructionPHPPids,
+)
+
 
 def set_baseline_envelope_constructions(
-        phpp_conn: phpp_app.PHPPConnection,
-        baseline_code: BaselineCode,
-        climate_zone: ClimateZones,
+    phpp_conn: phpp_app.PHPPConnection,
+    baseline_code: BaselineCode,
+    climate_zone: ClimateZones,
+    use_group: Use_Groups,
 ) -> None:
     """Set the PHPP Areas worksheet envelope constructions to the baseline values.
-    
-    Will create and add new Constructions to the PHPP U-Values worksheet, and the 
+
+    Will create and add new Constructions to the PHPP U-Values worksheet, and the
     PHPP Areas worksheet surfaces will each be updated to use the new constructions.
 
     Arguments:
     ----------
         * phpp_conn: phpp_app.PHPPConnection:
             The PHPP Connection
         * baseline_code: BaselineCode:
             The baseline code
         * climate_zone: ClimateZones:
             The climate zone
+        * use_group: Use_Groups:
+            The use group
     """
-    baseline_constructions = create_baseline_constructions(baseline_code, climate_zone)
-    construction_phpp_ids = add_baseline_constructions_to_phpp(phpp_conn, baseline_constructions)
+    baseline_constructions = create_baseline_constructions(
+        baseline_code, climate_zone, use_group
+    )
+    construction_phpp_ids = add_baseline_constructions_to_phpp(
+        phpp_conn, baseline_constructions
+    )
     reset_phpp_areas_constructions(phpp_conn, construction_phpp_ids)
 
+
 def reset_phpp_areas_constructions(
-        phpp_conn: phpp_app.PHPPConnection, 
-        construction_ids: BaselineConstructionPHPPids
+    phpp_conn: phpp_app.PHPPConnection, construction_ids: BaselineConstructionPHPPids
 ) -> None:
     """Reset the PHPP Areas worksheet to the baseline constructions."""
-    
+
     def row_is_exposed_wall(row_data: ExistingSurfaceRow) -> bool:
         """Exposed wall is a wall that is not a ground floor."""
-        return row_data.face_type == ComponentFaceType.WALL and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
+        return (
+            row_data.face_type == ComponentFaceType.WALL
+            and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
+        )
 
     def row_is_ground_wall(row_data: ExistingSurfaceRow) -> bool:
         """Ground wall is a wall that is a ground floor."""
-        return row_data.face_type == ComponentFaceType.WALL and row_data.face_exposure == ComponentExposureExterior.GROUND
+        return (
+            row_data.face_type == ComponentFaceType.WALL
+            and row_data.face_exposure == ComponentExposureExterior.GROUND
+        )
 
     def row_is_roof(row_data: ExistingSurfaceRow) -> bool:
         """Roof is a roof that is not a ground floor."""
-        return row_data.face_type == ComponentFaceType.ROOF_CEILING and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
+        return (
+            row_data.face_type == ComponentFaceType.ROOF_CEILING
+            and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
+        )
 
     def row_is_ground_floor(row_data: ExistingSurfaceRow) -> bool:
         """Ground floor is a floor that is a ground floor."""
-        return row_data.face_type == ComponentFaceType.FLOOR and row_data.face_exposure == ComponentExposureExterior.GROUND
+        return (
+            row_data.face_type == ComponentFaceType.FLOOR
+            and row_data.face_exposure == ComponentExposureExterior.GROUND
+        )
 
     def row_is_exposed_floor(row_data: ExistingSurfaceRow) -> bool:
         """Exposed floor is a floor that is not a ground floor."""
-        return row_data.face_type == ComponentFaceType.FLOOR and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
-        
+        return (
+            row_data.face_type == ComponentFaceType.FLOOR
+            and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
+        )
+
     for i, surface_row_data in phpp_conn.areas.surfaces.all_surface_rows:
-        
         if surface_row_data.no_name:
             continue
-        
+
         if row_is_roof(surface_row_data):
             phpp_conn.areas.set_surface_row_construction(i, construction_ids.roof)
             phpp_conn.areas.set_surface_row_solar_absorptivity(i, 0.75)
             phpp_conn.areas.set_surface_row_emissivity(i, 0.90)
         elif row_is_exposed_wall(surface_row_data):
-            phpp_conn.areas.set_surface_row_construction(i, construction_ids.exposed_wall)
+            phpp_conn.areas.set_surface_row_construction(
+                i, construction_ids.exposed_wall
+            )
             phpp_conn.areas.set_surface_row_solar_absorptivity(i, 0.75)
             phpp_conn.areas.set_surface_row_emissivity(i, 0.90)
         elif row_is_ground_wall(surface_row_data):
-            phpp_conn.areas.set_surface_row_construction(i, construction_ids.ground_wall)
+            phpp_conn.areas.set_surface_row_construction(
+                i, construction_ids.ground_wall
+            )
         elif row_is_exposed_floor(surface_row_data):
-            phpp_conn.areas.set_surface_row_construction(i, construction_ids.exposed_floor)
+            phpp_conn.areas.set_surface_row_construction(
+                i, construction_ids.exposed_floor
+            )
             phpp_conn.areas.set_surface_row_solar_absorptivity(i, 0.75)
             phpp_conn.areas.set_surface_row_emissivity(i, 0.90)
         elif row_is_ground_floor(surface_row_data):
-            phpp_conn.areas.set_surface_row_construction(i, construction_ids.ground_floor)
+            phpp_conn.areas.set_surface_row_construction(
+                i, construction_ids.ground_floor
+            )
```

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/phpp/components.py` & `PH-Baseliner-1.1.3/ph_baseliner/phpp/components.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/phpp/lighting.py` & `PH-Baseliner-1.1.3/ph_baseliner/phpp/lighting.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/phpp/u_values.py` & `PH-Baseliner-1.1.3/ph_baseliner/phpp/u_values.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,86 +6,113 @@
 from copy import copy
 from typing import NamedTuple
 
 from PHX.PHPP import phpp_app
 from PHX.model.constructions import PhxConstructionOpaque
 
 from ph_baseliner.codes.model import BaselineCode
-from ph_baseliner.codes.options import ClimateZones
+from ph_baseliner.codes.options import ClimateZones, Use_Groups
 
 
 class BaselinePHXConstructions(NamedTuple):
     """NamedTuple: The baseline PHX constructions for the PHPP U-Values Worksheet."""
+
     roof: PhxConstructionOpaque
     exposed_wall: PhxConstructionOpaque
     ground_wall: PhxConstructionOpaque
     exposed_floor: PhxConstructionOpaque
     ground_floor: PhxConstructionOpaque
 
 
 class BaselineConstructionPHPPids(NamedTuple):
     """NamedTuple: Output of the add_baseline_constructions_to_phpp function."""
+
     roof: str
     exposed_wall: str
     ground_wall: str
     exposed_floor: str
     ground_floor: str
 
 
 def create_baseline_constructions(
-        baseline_code: BaselineCode,
-        climate_zone: ClimateZones,
+    baseline_code: BaselineCode, climate_zone: ClimateZones, use_group: Use_Groups
 ) -> BaselinePHXConstructions:
     """Create the baseline constructions from the code baseline model."""
-    table_max_u_values = baseline_code.tables.maximum_u_factors
-    
-    roof_u_values = getattr(table_max_u_values.roofs.insulation_above_deck, climate_zone.name)
+
+    # -- Roofs
     new_roof_phx_construction = PhxConstructionOpaque.from_total_u_value(
-        roof_u_values.group_r, "BASELINE: ROOF"
+        baseline_code.get_baseline_roof_u_value(climate_zone, use_group),
+        "BASELINE: ROOF",
     )
 
-    exposed_wall_u_values = getattr(table_max_u_values.walls.mass, climate_zone.name)
+    # -- Exposed Walls (Above Grade)
     new_exposed_wall_phx_construction = PhxConstructionOpaque.from_total_u_value(
-        exposed_wall_u_values.group_r, "BASELINE: EXPOSED WALL"
+        baseline_code.get_baseline_exposed_wall_u_value(climate_zone, use_group),
+        "BASELINE: EXPOSED WALL",
     )
 
-    ground_wall_u_values = getattr(table_max_u_values.walls.below_grade, climate_zone.name)
+    # -- Ground Walls (Below Grade)
     new_ground_wall_phx_construction = PhxConstructionOpaque.from_total_u_value(
-        ground_wall_u_values.group_r, "BASELINE: GROUND WALL"
+        baseline_code.get_baseline_ground_wall_c_factor(climate_zone, use_group),
+        "BASELINE: GROUND WALL",
     )
 
-    exposed_floor_u_values = getattr(table_max_u_values.floors.mass, climate_zone.name)
+    # -- Exposed Floors
     new_exposed_floor_phx_construction = PhxConstructionOpaque.from_total_u_value(
-        exposed_floor_u_values.group_r, "BASELINE: EXPOSED FLOOR"
+        baseline_code.get_baseline_exposed_floor_u_value(climate_zone, use_group),
+        "BASELINE: EXPOSED FLOOR",
     )
-    
-    ground_floor_u_values = getattr(table_max_u_values.floors.unheated_slab, climate_zone.name)
+
+    # -- Ground Floors
     new_ground_floor_phx_construction = PhxConstructionOpaque.from_total_u_value(
-        ground_floor_u_values.group_r,"BASELINE: GROUND FLOOR"
+        baseline_code.get_baseline_ground_floor_f_factor(climate_zone, use_group),
+        "BASELINE: GROUND FLOOR",
     )
 
     return BaselinePHXConstructions(
         new_roof_phx_construction,
         new_exposed_wall_phx_construction,
         new_ground_wall_phx_construction,
         new_exposed_floor_phx_construction,
         new_ground_floor_phx_construction,
     )
 
-def add_baseline_constructions_to_phpp(phpp_conn: phpp_app.PHPPConnection, baseline_constructions: BaselinePHXConstructions) -> BaselineConstructionPHPPids:
+
+def add_baseline_constructions_to_phpp(
+    phpp_conn: phpp_app.PHPPConnection, baseline_constructions: BaselinePHXConstructions
+) -> BaselineConstructionPHPPids:
     """Add the baseline constructions to the PHPP U-Values Worksheet."""
-    roof_phpp_id = phpp_conn.u_values.add_new_phx_construction(baseline_constructions.roof)
-    exposed_wall_phpp_id = phpp_conn.u_values.add_new_phx_construction(baseline_constructions.exposed_wall)
-    ground_wall_phpp_id = phpp_conn.u_values.add_new_phx_construction(baseline_constructions.ground_wall)
-    exposed_floor_phpp_id = phpp_conn.u_values.add_new_phx_construction(baseline_constructions.exposed_floor)
-    ground_floor_phpp_id = phpp_conn.u_values.add_new_phx_construction(baseline_constructions.ground_floor)
+    roof_phpp_id = phpp_conn.u_values.add_new_phx_construction(
+        baseline_constructions.roof
+    )
+    exposed_wall_phpp_id = phpp_conn.u_values.add_new_phx_construction(
+        baseline_constructions.exposed_wall
+    )
+    ground_wall_phpp_id = phpp_conn.u_values.add_new_phx_construction(
+        baseline_constructions.ground_wall
+    )
+    exposed_floor_phpp_id = phpp_conn.u_values.add_new_phx_construction(
+        baseline_constructions.exposed_floor
+    )
+    ground_floor_phpp_id = phpp_conn.u_values.add_new_phx_construction(
+        baseline_constructions.ground_floor
+    )
 
-    return BaselineConstructionPHPPids(roof_phpp_id, exposed_wall_phpp_id, ground_wall_phpp_id, exposed_floor_phpp_id, ground_floor_phpp_id)
+    return BaselineConstructionPHPPids(
+        roof_phpp_id,
+        exposed_wall_phpp_id,
+        ground_wall_phpp_id,
+        exposed_floor_phpp_id,
+        ground_floor_phpp_id,
+    )
 
-def replace_u_values_with_baseline_constructions(phpp_conn: phpp_app.PHPPConnection, baseline_constructions: BaselinePHXConstructions) -> None:
+
+def replace_u_values_with_baseline_constructions(
+    phpp_conn: phpp_app.PHPPConnection, baseline_constructions: BaselinePHXConstructions
+) -> None:
     """Replace the existing U-Values with the baseline constructions."""
 
     def is_roof(_input: str):
         """Return True if the R_si type is a 'Roof'."""
         return "ROOF" in str(_input).upper()
 
     def is_wall(_input: str):
@@ -100,26 +127,26 @@
         """Return True if the R_se type is a 'Ground'."""
         return "GROUND" in str(_input).upper()
 
     for row_num in phpp_conn.u_values.used_constructor_start_rows:
         constructor_name = phpp_conn.u_values.get_constructor_name(row_num)
         r_si_type = phpp_conn.u_values.get_constructor_r_si_type(row_num)
         r_se_type = phpp_conn.u_values.get_constructor_r_se_type(row_num)
-        
+
         if is_roof(r_si_type):
             _phx_const = copy(baseline_constructions.roof)
         elif is_wall(r_si_type) and is_below_grade(r_se_type):
             _phx_const = copy(baseline_constructions.ground_wall)
         elif is_wall(r_si_type) and not is_below_grade(r_se_type):
             _phx_const = copy(baseline_constructions.exposed_wall)
         elif is_floor(r_si_type) and is_below_grade(r_se_type):
             _phx_const = copy(baseline_constructions.ground_floor)
         elif is_floor(r_si_type) and not is_below_grade(r_se_type):
             _phx_const = copy(baseline_constructions.exposed_floor)
         else:
             continue
 
         _phx_const.display_name = constructor_name
-        
+
         # -- Update the PHPP
         phpp_conn.u_values.clear_single_constructor_data(row_num, False)
-        phpp_conn.u_values.write_single_PHX_construction(_phx_const, row_num)
+        phpp_conn.u_values.write_single_PHX_construction(_phx_const, row_num)
```

### Comparing `PH-Baseliner-1.0.3/ph_baseliner/phpp/windows.py` & `PH-Baseliner-1.1.3/ph_baseliner/phpp/windows.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,122 +2,138 @@
 # -*- Python Version: 3.7 -*-
 
 """Functions to set baseline PHPP windows."""
 
 from PHX.PHPP import phpp_app
 
 from ph_baseliner.codes.model import BaselineCode
-from ph_baseliner.codes.options import ClimateZones
-from ph_baseliner.phpp.components import (add_new_baseline_window_glazing, 
-            add_new_baseline_window_frame, create_new_baseline_window_glazing)
+from ph_baseliner.codes.options import ClimateZones, PF_Groups, Use_Groups
+from ph_baseliner.phpp.components import (
+    add_new_baseline_window_glazing,
+    add_new_baseline_window_frame,
+    create_new_baseline_window_glazing,
+)
 
 
-def get_baseline_u_value(_baseline_code: BaselineCode, _climate_zone: ClimateZones) -> float:
+def get_baseline_u_value(
+    _baseline_code: BaselineCode, _climate_zone: ClimateZones, _use_group: Use_Groups
+) -> float:
     """Get the baseline U-Value for the specified climate zone."""
-    u_values = _baseline_code.tables.fenestration_u_factors.operable_windows.u_factors
-    u_values = getattr(u_values, _climate_zone.name)
-    return u_values.group_r
-
-def get_baseline_SHGC(_baseline_code: BaselineCode, _climate_zone: ClimateZones) -> float:
-    """Get the baseline SHGC for the specified climate zone."""
-    shgcs = _baseline_code.tables.fenestration_u_factors.operable_windows.shgc
-    shgcs = getattr(shgcs, _climate_zone.name)
-    return shgcs.group_r
+    all_u_values = _baseline_code.get_window_u_values()
+    cz_uvalues = all_u_values.get_u_value_for_climate(_climate_zone)
+    u_value = cz_uvalues.get_u_values_for_use_group(_use_group)
+    return u_value
+
+
+def get_baseline_SHGC(
+    _baseline_code: BaselineCode, _climate_zone: ClimateZones, _pf_group: PF_Groups
+) -> float:
+    """Get the baseline SHGC for the specified climate zone and Projection Factor group."""
+    all_shgcs = _baseline_code.get_window_shgcs()
+    cz_shgcs = all_shgcs.get_shgcs_for_climate(_climate_zone)
+    pf_shgc = cz_shgcs.get_shgc_for_pf(_pf_group)
+    return pf_shgc
+
 
 def set_baseline_window_construction(
-        _phpp_conn: phpp_app.PHPPConnection, 
-        _baseline_code: BaselineCode,
-        _climate_zone: ClimateZones,
+    _phpp_conn: phpp_app.PHPPConnection,
+    _baseline_code: BaselineCode,
+    _climate_zone: ClimateZones,
+    _pf_group: PF_Groups,
+    _use_group: Use_Groups,
 ) -> None:
     """Set the baseline window construction in the PHPP Windows Worksheet.
-    
+
     Arguments:
-    -----
+    ----------
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
-    
+
     # -- Get the baseline values for U-Value and SHGC
-    u_value = get_baseline_u_value(_baseline_code, _climate_zone)
-    shgc =  get_baseline_SHGC(_baseline_code, _climate_zone)
+    u_value = get_baseline_u_value(_baseline_code, _climate_zone, _use_group)
+    shgc = get_baseline_SHGC(_baseline_code, _climate_zone, _pf_group)
 
     # -- Create the new baseline window construction
     baseline_phx_window = create_new_baseline_window_glazing(u_value, shgc)
     phpp_glazing_id = add_new_baseline_window_glazing(_phpp_conn, baseline_phx_window)
     phpp_frame_id = add_new_baseline_window_frame(_phpp_conn, baseline_phx_window)
 
     # -- Set the window constructions in the Windows Worksheet
     for row_num in _phpp_conn.windows.used_window_row_numbers:
-        _phpp_conn.windows.set_single_window_construction_ids(row_num, phpp_glazing_id, phpp_frame_id)
-
-def get_baseline_max_wwr(_baseline_code: BaselineCode) -> float:
-    """Get the maximum window-to-wall ratio from the baseline code."""
-    return _baseline_code.sections.maximum_fenestration_area.maximum_window_percent_of_wall
+        _phpp_conn.windows.set_single_window_construction_ids(
+            row_num, phpp_glazing_id, phpp_frame_id
+        )
 
-def get_baseline_max_srr(_baseline_code: BaselineCode) -> float:
-    """Get the maximum skylight-to-roof ratio from the baseline code."""
-    return _baseline_code.sections.maximum_fenestration_area.maximum_skylight_percent_of_roof
 
-def set_baseline_window_area(_phpp_conn: phpp_app.PHPPConnection, _baseline_code: BaselineCode) -> None:
+def set_baseline_window_area(
+    _phpp_conn: phpp_app.PHPPConnection, _baseline_code: BaselineCode
+) -> None:
     """Set the maximum window-to-wall ratio in the PHPP Windows Worksheet.
-    
+
     Arguments:
     ----------
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
-    maximum_wwr = get_baseline_max_wwr(_baseline_code)
+    maximum_wwr = _baseline_code.get_baseline_max_wwr()
     current_wall_area = _phpp_conn.areas.get_total_wall_area()
     current_window_area = _phpp_conn.windows.get_total_window_area()
     current_wwr = current_window_area / (current_wall_area + current_window_area)
 
     if current_wwr < maximum_wwr:
         print(f"Current WWR {current_wwr:.2%} is less than maximum {maximum_wwr:.0%}.")
         return None
 
-    print(f"Current WWR {current_wwr:.2%} is greater than maximum {maximum_wwr:.0%}. Scaling windows.")
-    
+    print(
+        f"Current WWR {current_wwr:.2%} is greater than maximum {maximum_wwr:.0%}. Scaling windows."
+    )
+
     # -- Figure out the right scale factor
     scale_factor = maximum_wwr / current_wwr
 
     # -- Scale the window areas
     for row_num in _phpp_conn.windows.used_window_row_numbers:
         if not _phpp_conn.windows.row_is_window(row_num):
             continue
 
         _phpp_conn.windows.scale_window_size(row_num, scale_factor)
 
 
-def set_baseline_skylight_area(_phpp_conn: phpp_app.PHPPConnection, _baseline_code: BaselineCode) -> None:
+def set_baseline_skylight_area(
+    _phpp_conn: phpp_app.PHPPConnection, _baseline_code: BaselineCode
+) -> None:
     """Set the maximum skylight-to-roof ratio in the PHPP Windows Worksheet.
-    
+
     Arguments:
     ----------
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
-    maximum_srr = get_baseline_max_srr(_baseline_code)
+    maximum_srr = _baseline_code.get_baseline_max_srr()
     current_roof_area = _phpp_conn.areas.get_total_roof_area()
     current_skylight_area = _phpp_conn.windows.get_total_skylight_area()
     current_srr = current_skylight_area / (current_roof_area + current_skylight_area)
 
     if current_srr < maximum_srr:
         print(f"Current SRR {current_srr:.2%} is less than maximum {maximum_srr:.0%}.")
         return None
 
-    print(f"Current SRR {current_srr:.2%} is greater than maximum {maximum_srr:.0%}. Scaling Skylights.")
-    
+    print(
+        f"Current SRR {current_srr:.2%} is greater than maximum {maximum_srr:.0%}. Scaling Skylights."
+    )
+
     # -- Figure out the right scale factor
     scale_factor = maximum_srr / current_srr
 
     # -- Scale the window areas
     for row_num in _phpp_conn.windows.used_window_row_numbers:
         if not _phpp_conn.windows.row_is_skylight(row_num):
             continue
 
-        _phpp_conn.windows.scale_window_size(row_num, scale_factor) 
+        _phpp_conn.windows.scale_window_size(row_num, scale_factor)
```

### Comparing `PH-Baseliner-1.0.3/setup.cfg` & `PH-Baseliner-1.1.3/setup.cfg`

 * *Files identical despite different names*

