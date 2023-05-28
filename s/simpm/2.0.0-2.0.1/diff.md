# Comparing `tmp/simpm-2.0.0.tar.gz` & `tmp/simpm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpm-2.0.0.tar", last modified: Sun May 28 05:27:12 2023, max compression
+gzip compressed data, was "simpm-2.0.1.tar", last modified: Sun May 28 16:59:13 2023, max compression
```

## Comparing `simpm-2.0.0.tar` & `simpm-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:27:12.459400 simpm-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 05:27:01.000000 simpm-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-28 05:27:12.459400 simpm-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-28 05:27:01.000000 simpm-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-28 05:27:12.459400 simpm-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 05:27:01.000000 simpm-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:27:12.455400 simpm-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:27:12.455400 simpm-2.0.0/src/simpm/
--rw-r--r--   0 runner    (1001) docker     (123)    32049 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/MovingEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40339 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/log_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-28 05:27:01.000000 simpm-2.0.0/src/simpm/mcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:27:12.459400 simpm-2.0.0/src/simpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 05:27:12.000000 simpm-2.0.0/src/simpm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 16:59:02.000000 simpm-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-28 16:59:13.138248 simpm-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-28 16:59:02.000000 simpm-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-28 16:59:13.138248 simpm-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 16:59:02.000000 simpm-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.134248 simpm-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/src/simpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40268 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/log_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/src/simpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/top_level.txt
```

### Comparing `simpm-2.0.0/LICENSE` & `simpm-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpm-2.0.0/README.md` & `simpm-2.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-# PmPy - Project Management in python
+# SimPM - Simulation Tool in Project Management
 
-![Github Workflow Deploy Package](https://img.shields.io/github/actions/workflow/status/Project-PmPy/pmpy/python-publish.yml?label=deploy)
-![Github Release Version](https://img.shields.io/github/v/release/Project-PmPy/pmpy)
-![Github Release Date](https://img.shields.io/github/release-date/project-pmpy/pmpy)
-![PyPi Package Version](https://img.shields.io/pypi/v/pmpy)
-![PyPi Package Downloads](https://img.shields.io/pypi/dm/pmpy)
-![Github License](https://img.shields.io/github/license/project-pmpy/pmpy)
-![Github Issues](https://img.shields.io/github/issues/project-pmpy/pmpy)
-![Github Pull Requests](https://img.shields.io/github/issues-pr/project-pmpy/pmpy)
+![Github Workflow Deploy Package](https://img.shields.io/github/actions/workflow/status/Project-SimPM/SimPM/python-publish.yml?label=deploy)
+![Github Release Version](https://img.shields.io/github/v/release/Project-SimPM/SimPM)
+![Github Release Date](https://img.shields.io/github/release-date/Project-SimPM/SimPM)
+![PyPi Package Version](https://img.shields.io/pypi/v/simpm)
+![PyPi Package Downloads](https://img.shields.io/pypi/dm/simpm)
+![Github License](https://img.shields.io/github/license/Project-SimPM/SimPM)
+![Github Issues](https://img.shields.io/github/issues/Project-SimPM/SimPM)
+![Github Pull Requests](https://img.shields.io/github/issues-pr/Project-SimPM/SimPM)
 
-PmPy offers project management tools in python.
+SimPM offers simulation tools in project management.
 
 Subpackages:
 - des (discrete event simulation)
-- consim (continuous simulation), 
-- abs (agent-based simulation)
-- mcs (monte carlo simulation)
-- dists (probability distributions) modules.
-## Using Pmpy
+- dists (probability distributions) modules
+
+## Using SimPM
 Getting started quickly:
 ```
-pip install pmpy
+pip install simpm
 ```
 ## Community
-- [Github Discussions](https://github.com/project-pmpy/pmpy/discussions)
+- [Github Discussions](https://github.com/Project-SimPM/SimPM/discussions)
 
-## Contributing back to PmPy
-If you run into an issue, please file a new [issue](https://github.com/project-pmpy/pmpy/issues) for us to discuss. If possible, follow up with a pull request.
+## Contributing back to SimPM
+If you run into an issue, please file a new [issue](https://github.com/Project-SimPM/SimPM/issues) for us to discuss. If possible, follow up with a pull request.
 
-If you would like to add a feature, please reach out via [issue](https://github.com/project-pmpy/pmpy/issues). A feature is most likely to be added if you build it!
+If you would like to add a feature, please reach out via [issue](https://github.com/Project-SimPM/SimPM/issues). A feature is most likely to be added if you build it!
```

### Comparing `simpm-2.0.0/setup.cfg` & `simpm-2.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = simpm
-author = Naima Sadeghi, Pedram Elmi
-author_email = <naima.sadeghi@gmail.com>, <pedram.elmi@gmail.com>
+author = Naimeh Sadeghi, Pedram Elmi
+author_email = "naima.sadeghi@gmail.com", "pedram.elmi@gmail.com"
 description = Simulation Tool in Project Management.
-long_description = file: README.md, CHANGES.md, AUTHORS.md
+long_description = file: README.md, AUTHORS.md
 long_description_content_type = text/markdown
 url = https://github.com/Project-SimPM
 keywords = 
 	python
 	project management
 	construction
 	simulation
```

### Comparing `simpm-2.0.0/setup.py` & `simpm-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.0/src/simpm/_utils.py` & `simpm-2.0.1/src/simpm/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Internal utility functions for the pmpy package.
+Internal utility functions for the SimPM package.
 
 These functions are intended for internal use only and are not part of the public API.
 """
 
 from typing import Any
 
 def _swap_dict_keys_values(original_dict: dict[Any,Any]) -> dict[Any,Any]:
```

### Comparing `simpm-2.0.0/src/simpm/des.py` & `simpm-2.0.1/src/simpm/des.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from pandas import DataFrame
 from numpy import array, append, nansum
 import simpy
 
 from simpm.dist import distribution
 from simpm._utils import _swap_dict_keys_values
 
-# import matplotlib.pyplot as plt
-# from simpm.log_cfg import logger
-
-
 class Entity:
     """
     A class that defines an entity with dictionary-like attributes. Entities are virtual objects essential to useful for modeling dynamic systems.
     Some examples of entities can be a customer, communication message, or any resource requiring service.
     ---
     Attributes
     ---
```

### Comparing `simpm-2.0.0/src/simpm/dist.py` & `simpm-2.0.1/src/simpm/dist.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.0/src/simpm/log_cfg.py` & `simpm-2.0.1/src/simpm/log_cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """
 ## SimPM Logging Module
 
 ---
 
+### Logging Levels:
+- `logging.DEBUG` = 10
+- `logging.INFO` = 20
+- `logging.WARNING` = 30
+- `logging.ERROR` = 40
+- `logging.CRITICAL` = 50
+
+---
+
 ### Module-level variables
- `logger` : This logger holds a `logging.Logger` object for logging messages in the "simpm" package.
+ `logger` : This logger holds a `logging.Logger` object for logging messages in the simpm package.
 
 ---
 
 ### Functions
- `current_config()`: Returns the last instance of `LogConfig` wich its properties can change
+ `log_config()`: Returns the `LogConfig` object that its properties can change
  
 ---
 
 ## LogConfig Class
  This module provides a  `LogConfig`  class that can be used to configure logging settings in a simpm.
  ### Overview
  The  `LogConfig`  class allows developers to configure logging settings such as log output destination, log level, and log formatting. It provides a way to customize the logging behavior of an application based on specific requirements.
@@ -173,15 +182,42 @@
     def last_instance(cls) -> LogConfig:
         """This function returns the last instance of the LogConfig class if one exists, otherwise it creates a new LogConfig with enabled set to False, console_level set to logging.DEBUG, file_level set to logging.DEBUG, and file_path set to "simpm.log"."""
         if cls._last_instance is None:
             return LogConfig(enabled=False, console_level=logging.DEBUG, file_level=logging.DEBUG,
                        file_path='simpm.log')
         return cls._last_instance
 
-def current_config() -> LogConfig:
+def log_config() -> LogConfig:
     """ 
-    Returns the last instance of `LogConfig` that its properties can change
+    Returns the `LogConfig` object that its properties can change
     """
     return LogConfig.last_instance()
 
 logger = logging.getLogger("simpm")
-"""This logger holds a `logging.Logger` object for logging messages in the "simpm" package."""
+"""
+This logger holds a `logging.Logger` object for logging messages in the simpm package.
+
+## Levels:
+- `logging.DEBUG` = 10
+- `logging.INFO` = 20
+- `logging.WARNING` = 30
+- `logging.ERROR` = 40
+- `logging.CRITICAL` = 50
+
+## How To Use
+### Using `log` method
+```python
+logger.log(logging.DEBUG,"This is a DEBUG message")
+logger.log(logging.INFO,"This is an INFO message")
+logger.log(logging.WARNING,"This is a WARNING message")
+logger.log(logging.ERROR,"This is a ERROR message")
+logger.log(logging.CRITICAL,"This is a CRITICAL message")
+```
+### Using `debug`, `info`, `warning`, `error` and `critical` methods
+```python
+logger.debug("This is a DEBUG message")
+logger.info("This is an INFO message")
+logger.warning("This is a WARNING message")
+logger.error("This is a ERROR message")
+logger.critical(logging.CRITICAL,"This is a CRITICAL message")
+```
+"""
```

