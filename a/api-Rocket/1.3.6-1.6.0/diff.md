# Comparing `tmp/api-Rocket-1.3.6.tar.gz` & `tmp/api-Rocket-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.3.6.tar", last modified: Tue Apr 25 06:58:21 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.6.0.tar", last modified: Sun May 28 19:01:55 2023, max compression
```

## Comparing `api-Rocket-1.3.6.tar` & `api-Rocket-1.6.0.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.699218 api-Rocket-1.3.6/
--rw-rw-rw-   0        0        0       20 2023-04-25 06:58:20.000000 api-Rocket-1.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0      526 2023-04-25 06:58:21.700195 api-Rocket-1.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.677734 api-Rocket-1.3.6/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-04-25 06:57:19.000000 api-Rocket-1.3.6/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.660156 api-Rocket-1.3.6/api_Rocket/lib/
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.694336 api-Rocket-1.3.6/api_Rocket/lib/clients/
--rw-rw-rw-   0        0        0      418 2023-03-20 11:34:29.000000 api-Rocket-1.3.6/api_Rocket/lib/clients/async_client.py
--rw-rw-rw-   0        0        0     5648 2023-04-21 14:19:08.000000 api-Rocket-1.3.6/api_Rocket/lib/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.697265 api-Rocket-1.3.6/api_Rocket/lib/clients/exception/
--rw-rw-rw-   0        0        0     1718 2023-03-24 14:12:55.000000 api-Rocket-1.3.6/api_Rocket/lib/clients/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:58:21.689453 api-Rocket-1.3.6/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-25 06:58:21.000000 api-Rocket-1.3.6/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-25 06:58:21.000000 api-Rocket-1.3.6/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:58:21.000000 api-Rocket-1.3.6/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 06:58:21.000000 api-Rocket-1.3.6/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:58:21.702148 api-Rocket-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-04-25 06:58:20.000000 api-Rocket-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.204625 api-Rocket-1.6.0/
+-rw-rw-rw-   0        0        0       20 2023-05-28 19:01:53.000000 api-Rocket-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:01:55.205601 api-Rocket-1.6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.195836 api-Rocket-1.6.0/api_Rocket/
+-rw-rw-rw-   0        0        0      685 2023-05-28 18:53:58.000000 api-Rocket-1.6.0/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:01:55.203648 api-Rocket-1.6.0/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-28 19:01:55.000000 api-Rocket-1.6.0/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 19:01:54.000000 api-Rocket-1.6.0/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:01:55.206578 api-Rocket-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-05-28 19:01:53.000000 api-Rocket-1.6.0/setup.py
```

### Comparing `api-Rocket-1.3.6/api_Rocket/__init__.py` & `api-Rocket-1.6.0/api_Rocket/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .lib.clients.client import Client
+from .lib.clients.client import Client, Trade_Client
 from .lib.clients.async_client import async_Client
 import requests
 import json
 
 
 #information
 __title__ = "api-Rocket"
 
 __author__ = "Redpiar"
 
 __license__ = "MIT"
 
 __copyright__ = "Copyright 2023 Redpiar"
 
-__version__ = '1.3.6'
+__version__ = '1.6.0'
 
 __status__ = "(Beta)"
 
 __newest__ = json.loads(requests.get("https://pypi.org/pypi/api-Rocket/json").text)["info"]["version"]
 
 if __version__ != __newest__:
 	print(f"""
```

