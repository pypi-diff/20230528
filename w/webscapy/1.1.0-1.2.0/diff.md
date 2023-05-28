# Comparing `tmp/webscapy-1.1.0.tar.gz` & `tmp/webscapy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.1.0.tar", last modified: Sun May 28 08:53:03 2023, max compression
+gzip compressed data, was "webscapy-1.2.0.tar", last modified: Sun May 28 10:01:56 2023, max compression
```

## Comparing `webscapy-1.1.0.tar` & `webscapy-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.784985 webscapy-1.1.0/
--rw-rw-rw-   0        0        0      131 2023-05-28 08:53:03.780985 webscapy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       97 2023-05-28 06:36:34.000000 webscapy-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 08:53:03.785988 webscapy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      225 2023-05-28 08:53:00.000000 webscapy-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.737621 webscapy-1.1.0/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.1.0/webscapy/__init__.py
--rw-rw-rw-   0        0        0     4008 2023-05-28 08:48:45.000000 webscapy-1.1.0/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:53:03.775012 webscapy-1.1.0/webscapy.egg-info/
--rw-rw-rw-   0        0        0      131 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 08:52:41.000000 webscapy-1.1.0/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-28 08:53:03.000000 webscapy-1.1.0/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.237221 webscapy-1.2.0/
+-rw-rw-rw-   0        0        0      131 2023-05-28 10:01:56.235216 webscapy-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3697 2023-05-28 09:56:04.000000 webscapy-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 10:01:56.239243 webscapy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      225 2023-05-28 10:01:46.000000 webscapy-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.191211 webscapy-1.2.0/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.2.0/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     4177 2023-05-28 10:00:29.000000 webscapy-1.2.0/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:01:56.229213 webscapy-1.2.0/webscapy.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-28 10:01:56.000000 webscapy-1.2.0/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.1.0/webscapy/webscapy.py` & `webscapy-1.2.0/webscapy/webscapy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.action_chains import ActionChains
 from webdriver_manager.chrome import ChromeDriverManager
 import undetected_chromedriver as uc
 
 class Webscapy:
-    def __init__(self):
-        pass
+    def __init__(self, headless = True, executable_path = None, remote_url = None, undetected = False, version = None):
+        self.setup_driver(headless, executable_path, remote_url, undetected, version)
 
     def setup_driver(self, headless = True, executable_path = None, remote_url = None, undetected = False, version = None):
         if remote_url is not None:
             self.create_remote_driver(remote_url)
         else:
             if undetected:
                 self.create_undetected_driver(headless, executable_path, version)
```

