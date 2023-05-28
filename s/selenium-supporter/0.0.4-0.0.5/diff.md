# Comparing `tmp/selenium-supporter-0.0.4.tar.gz` & `tmp/selenium-supporter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-supporter-0.0.4.tar", last modified: Sat May 27 16:56:31 2023, max compression
+gzip compressed data, was "selenium-supporter-0.0.5.tar", last modified: Sun May 28 01:51:12 2023, max compression
```

## Comparing `selenium-supporter-0.0.4.tar` & `selenium-supporter-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.086913 selenium-supporter-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-27 16:56:31.085913 selenium-supporter-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.084913 selenium-supporter-0.0.4/selenium_supporter/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/drivers.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 16:56:31.085913 selenium-supporter-0.0.4/selenium_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/selenium_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 16:56:31.086913 selenium-supporter-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-05-27 16:56:30.000000 selenium-supporter-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.756601 selenium-supporter-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-28 01:51:12.755601 selenium-supporter-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.753601 selenium-supporter-0.0.5/selenium_supporter/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/drivers.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/selenium_supporter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 01:51:12.755601 selenium-supporter-0.0.5/selenium_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-28 01:51:12.000000 selenium-supporter-0.0.5/selenium_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 01:51:12.756601 selenium-supporter-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-28 01:51:11.000000 selenium-supporter-0.0.5/setup.py
```

### Comparing `selenium-supporter-0.0.4/PKG-INFO` & `selenium-supporter-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.4/README.md` & `selenium-supporter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.4/selenium_supporter/drivers.py` & `selenium-supporter-0.0.5/selenium_supporter/drivers.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.4/selenium_supporter/utils.py` & `selenium-supporter-0.0.5/selenium_supporter/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ##import socket
 from pathlib import Path
 import subprocess
 import os
-
 import platform
 from PIL import Image
 from io import StringIO
 from PIL import Image
 from io import BytesIO
 from io import BytesIO
 from pathlib import Path
@@ -38,20 +37,30 @@
         return path1
     elif os.path.exists(path2):
         return path2
     elif os.path.exists(path3):
         return path3
 
 def kill_all_chrome_web_browser_processes():
-    #https://stackoverflow.com/questions/57792469/kill-certain-chrome-process-in-python-not-all
-    subprocess.call("TASKKILL /f /IM CHROME.EXE")
+    if platform.system() == 'Darwin': #맥
+        pass
+    elif platform.system() == 'Windows': #윈도우
+        #https://stackoverflow.com/questions/57792469/kill-certain-chrome-process-in-python-not-all
+        subprocess.call("TASKKILL /f /IM CHROME.EXE")
+    elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+        pass
 
 def kill_all_chrome_web_browser_driver_processes():
-    subprocess.call("TASKKILL /f /IM CHROMEDRIVER.EXE")
-
+    if platform.system() == 'Darwin': #맥
+        pass
+    elif platform.system() == 'Windows': #윈도우
+        subprocess.call("TASKKILL /f /IM CHROMEDRIVER.EXE")
+    elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+        pass
+    
 def open_chrome_web_browser(user_data_dir=None, proxy_server=None):
     chrome_web_browser_path = get_chrome_web_browser_path()
     #https://not-to-be-reset.tistory.com/454
     user_data_dir_option = ""
     if user_data_dir:
         user_data_dir_option = f"--user-data-dir={user_data_dir}"
     #https://www.chromium.org/developers/design-documents/network-stack/socks-proxy/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `selenium-supporter-0.0.4/selenium_supporter.egg-info/PKG-INFO` & `selenium-supporter-0.0.5/selenium_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.4/setup.py` & `selenium-supporter-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='selenium-supporter',
-	version='0.0.4',
+	version='0.0.5',
 	description='Selenium supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/selenium-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

