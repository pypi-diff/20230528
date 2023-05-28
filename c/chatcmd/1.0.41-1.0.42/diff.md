# Comparing `tmp/chatcmd-1.0.41.tar.gz` & `tmp/chatcmd-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.41.tar", last modified: Sun May 28 10:56:58 2023, max compression
+gzip compressed data, was "chatcmd-1.0.42.tar", last modified: Sun May 28 10:58:56 2023, max compression
```

## Comparing `chatcmd-1.0.41.tar` & `chatcmd-1.0.42.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:56:58.198316 chatcmd-1.0.41/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.41/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 10:56:58.197963 chatcmd-1.0.41/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 10:56:29.000000 chatcmd-1.0.41/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:56:58.195046 chatcmd-1.0.41/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.41/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.41/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 10:56:29.000000 chatcmd-1.0.41/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.41/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1555 2023-05-28 10:56:12.000000 chatcmd-1.0.41/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2701 2023-05-28 10:56:12.000000 chatcmd-1.0.41/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:56:58.197418 chatcmd-1.0.41/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 10:56:58.000000 chatcmd-1.0.41/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 10:56:29.000000 chatcmd-1.0.41/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 10:56:58.198451 chatcmd-1.0.41/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 10:56:29.000000 chatcmd-1.0.41/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:58:56.394977 chatcmd-1.0.42/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.42/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 10:58:56.394627 chatcmd-1.0.42/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 10:58:39.000000 chatcmd-1.0.42/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:58:56.391343 chatcmd-1.0.42/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.42/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.42/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 10:58:39.000000 chatcmd-1.0.42/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.42/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1477 2023-05-28 10:58:19.000000 chatcmd-1.0.42/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2701 2023-05-28 10:56:12.000000 chatcmd-1.0.42/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 10:58:56.394062 chatcmd-1.0.42/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 10:58:56.000000 chatcmd-1.0.42/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 10:58:39.000000 chatcmd-1.0.42/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 10:58:56.395076 chatcmd-1.0.42/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 10:58:39.000000 chatcmd-1.0.42/setup.py
```

### Comparing `chatcmd-1.0.41/LICENSE` & `chatcmd-1.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.41/PKG-INFO` & `chatcmd-1.0.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.41
+Version: 1.0.42
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.41-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.42-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.41
+    Successfully installed chatcmd-1.0.42
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.41/README.md` & `chatcmd-1.0.42/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.41-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.42-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.41
+    Successfully installed chatcmd-1.0.42
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.41/chatcmd/api.py` & `chatcmd-1.0.42/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.41/chatcmd/chatcmd.py` & `chatcmd-1.0.42/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.41')
+            print('ChatCMD'+' 1.0.42')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.41/chatcmd/commands.py` & `chatcmd-1.0.42/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.41/chatcmd/helpers.py` & `chatcmd-1.0.42/chatcmd/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import re
 import inspect
 import subprocess
 import sys
-import gi
-gi.require_version('Gtk', '3.0')
-from gi.repository import Gtk, Gdk
 
 def library_info():
     print(
     "----------------------------------------------------------------\n"
     "  Library Name: ChatCMD\n"
     "  Library Source [PyPi]: https://pypi.org/naifalshaye/chatcmd\n"
     "  Library Source [Github]: https://github.com/naifalshaye/chatcmd\n"
```

### Comparing `chatcmd-1.0.41/chatcmd/lookup.py` & `chatcmd-1.0.42/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.41/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.42/chatcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.41
+Version: 1.0.42
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.41-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.42-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.41
+    Successfully installed chatcmd-1.0.42
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.41/pyproject.toml` & `chatcmd-1.0.42/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.41"
+version = "1.0.42"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.41/setup.py` & `chatcmd-1.0.42/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.41",
+    version="1.0.42",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

