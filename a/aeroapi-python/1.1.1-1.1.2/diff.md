# Comparing `tmp/aeroapi-python-1.1.1.tar.gz` & `tmp/aeroapi-python-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroapi-python-1.1.1.tar", last modified: Sun May 28 17:14:40 2023, max compression
+gzip compressed data, was "aeroapi-python-1.1.2.tar", last modified: Sun May 28 17:39:40 2023, max compression
```

## Comparing `aeroapi-python-1.1.1.tar` & `aeroapi-python-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:14:40.612282 aeroapi-python-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-28 17:14:40.612282 aeroapi-python-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:14:40.612282 aeroapi-python-1.1.1/aeroapi_python/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/APICaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/AeroAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/Airports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/Flights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/History.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/Miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/aeroapi_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:14:40.612282 aeroapi-python-1.1.1/aeroapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-28 17:14:40.000000 aeroapi-python-1.1.1/aeroapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-28 17:14:40.000000 aeroapi-python-1.1.1/aeroapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:14:40.000000 aeroapi-python-1.1.1/aeroapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 17:14:40.000000 aeroapi-python-1.1.1/aeroapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 17:14:40.000000 aeroapi-python-1.1.1/aeroapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:14:40.612282 aeroapi-python-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-28 17:14:29.000000 aeroapi-python-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/aeroapi_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/APICaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/AeroAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Airports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Flights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/aeroapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/setup.py
```

### Comparing `aeroapi-python-1.1.1/PKG-INFO` & `aeroapi-python-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroapi-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: FlightAware AeroAPI Caller for Python
 Home-page: https://github.com/derens99/aeroapi-python
 Author: Deren S
 Author-email: derens9999@gmail.com
 License: MIT
 Keywords: python aeroapi flightaware flightaware-api flightaware-aeroapi flightaware-aeroapi-python flightaware-aeroapi-python3 flightaware-aeroapi-python3.5 flightaware-aeroapi-python3.6 flightaware-aeroapi-python3.7 flightaware-aeroapi-python3.8 flightaware-aeroapi-python3.9
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,23 +20,48 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # AeroApi Python
 
-The (Unofficial) FlightAware AeroAPI Python Wrapper is a Python package that provides a convenient and easy-to-use interface for interacting with the FlightAware AeroAPI. This package simplifies the process of making API calls to FlightAware, retrieving and processing flight data, and integrating it into your Python applications.
+Python wrapper for the FlightAware's AeroAPI
+
+## Description
+
+AeroAPI (formerly FlightXML) is FlightAware's live flight data API that provides powerful, reliable information about real-time and historical flight information. This Python wrapper allows for easier interaction with the AeroAPI from Python applications.
+
+## FlightAware AeroAPI Reference
+[AeroAPI](https://flightaware.com/aeroapi)
 
 ## Installation
 
 ```bash
 pip install aeroapi-python
 ```
     
 ### Using test pypi, install with this command.
-'''bash
+```bash
 pip install --index-url https://pypi.org/simple/ --extra-index-url https://test.pypi.org/simple/ aeroapi-python
-'''
+```
+
+## Usage
+
+```python
+from aeroapi_python import AeroApi
+
+# initialize with your AeroAPI username and API Key
+aero_api = AeroAPI('your-api-key')
+```
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+## Authors
+
+- [@derens99](https://www.github.com/derens99)
```

### Comparing `aeroapi-python-1.1.1/aeroapi_python/APICaller.py` & `aeroapi-python-1.1.2/aeroapi_python/APICaller.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python/AeroAPI.py` & `aeroapi-python-1.1.2/aeroapi_python/AeroAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from typing import Optional
 from .Operators import Operators
 from .APICaller import APICaller
 from .Airports import Airports
 from .History import History
 from .Miscellaneous import Miscellaneous
 from .Flights import Flights
 
-
 class AeroAPI:
     """
     A class for interacting with the FlightAware AeroAPI.
 
     Attributes:
         base_url (str): The base URL for the AeroAPI.
         api_key (str): The API key for the AeroAPI.
```

### Comparing `aeroapi-python-1.1.1/aeroapi_python/Airports.py` & `aeroapi-python-1.1.2/aeroapi_python/Airports.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python/Flights.py` & `aeroapi-python-1.1.2/aeroapi_python/Flights.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python/History.py` & `aeroapi-python-1.1.2/aeroapi_python/History.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python/Miscellaneous.py` & `aeroapi-python-1.1.2/aeroapi_python/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python/Operators.py` & `aeroapi-python-1.1.2/aeroapi_python/Operators.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.1/aeroapi_python.egg-info/PKG-INFO` & `aeroapi-python-1.1.2/aeroapi_python.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroapi-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: FlightAware AeroAPI Caller for Python
 Home-page: https://github.com/derens99/aeroapi-python
 Author: Deren S
 Author-email: derens9999@gmail.com
 License: MIT
 Keywords: python aeroapi flightaware flightaware-api flightaware-aeroapi flightaware-aeroapi-python flightaware-aeroapi-python3 flightaware-aeroapi-python3.5 flightaware-aeroapi-python3.6 flightaware-aeroapi-python3.7 flightaware-aeroapi-python3.8 flightaware-aeroapi-python3.9
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,23 +20,48 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # AeroApi Python
 
-The (Unofficial) FlightAware AeroAPI Python Wrapper is a Python package that provides a convenient and easy-to-use interface for interacting with the FlightAware AeroAPI. This package simplifies the process of making API calls to FlightAware, retrieving and processing flight data, and integrating it into your Python applications.
+Python wrapper for the FlightAware's AeroAPI
+
+## Description
+
+AeroAPI (formerly FlightXML) is FlightAware's live flight data API that provides powerful, reliable information about real-time and historical flight information. This Python wrapper allows for easier interaction with the AeroAPI from Python applications.
+
+## FlightAware AeroAPI Reference
+[AeroAPI](https://flightaware.com/aeroapi)
 
 ## Installation
 
 ```bash
 pip install aeroapi-python
 ```
     
 ### Using test pypi, install with this command.
-'''bash
+```bash
 pip install --index-url https://pypi.org/simple/ --extra-index-url https://test.pypi.org/simple/ aeroapi-python
-'''
+```
+
+## Usage
+
+```python
+from aeroapi_python import AeroApi
+
+# initialize with your AeroAPI username and API Key
+aero_api = AeroAPI('your-api-key')
+```
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+## Authors
+
+- [@derens99](https://www.github.com/derens99)
```

### Comparing `aeroapi-python-1.1.1/setup.py` & `aeroapi-python-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     requirements = f.read().splitlines()
 
 readme_path = pathlib.Path("README.md")
 requirements_path = pathlib.Path("requirements.txt")
 
 setuptools.setup(
     name="aeroapi-python",
-    version="1.1.01",
+    version="1.1.2",
     description='FlightAware AeroAPI Caller for Python',
     long_description=readme_path.read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/derens99/aeroapi-python",
     author="Deren S",
     author_email="derens9999@gmail.com",
     license="MIT",
```

