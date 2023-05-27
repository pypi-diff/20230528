# Comparing `tmp/chatcmd-1.0.33.tar.gz` & `tmp/chatcmd-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.33.tar", last modified: Sat May 27 22:35:26 2023, max compression
+gzip compressed data, was "chatcmd-1.0.34.tar", last modified: Sat May 27 22:38:45 2023, max compression
```

## Comparing `chatcmd-1.0.33.tar` & `chatcmd-1.0.34.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:35:26.151381 chatcmd-1.0.33/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.33/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:35:26.150846 chatcmd-1.0.33/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 22:35:05.000000 chatcmd-1.0.33/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:35:26.144911 chatcmd-1.0.33/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.33/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.33/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-27 22:35:05.000000 chatcmd-1.0.33/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.33/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1245 2023-05-27 22:35:05.000000 chatcmd-1.0.33/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2515 2023-05-27 22:35:05.000000 chatcmd-1.0.33/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:35:26.150040 chatcmd-1.0.33/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 22:35:26.000000 chatcmd-1.0.33/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-27 22:35:05.000000 chatcmd-1.0.33/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 22:35:26.151553 chatcmd-1.0.33/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-27 22:35:05.000000 chatcmd-1.0.33/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:38:45.775726 chatcmd-1.0.34/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.34/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:38:45.775174 chatcmd-1.0.34/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 22:38:15.000000 chatcmd-1.0.34/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:38:45.768739 chatcmd-1.0.34/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.34/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.34/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-27 22:38:15.000000 chatcmd-1.0.34/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.34/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1245 2023-05-27 22:35:05.000000 chatcmd-1.0.34/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2532 2023-05-27 22:37:11.000000 chatcmd-1.0.34/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:38:45.774348 chatcmd-1.0.34/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 22:38:45.000000 chatcmd-1.0.34/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-27 22:38:15.000000 chatcmd-1.0.34/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 22:38:45.775914 chatcmd-1.0.34/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-27 22:38:15.000000 chatcmd-1.0.34/setup.py
```

### Comparing `chatcmd-1.0.33/LICENSE` & `chatcmd-1.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.33/PKG-INFO` & `chatcmd-1.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.33
+Version: 1.0.34
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
-    Using cached chatcmd-1.0.33-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.34-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.33
+    Successfully installed chatcmd-1.0.34
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.33/README.md` & `chatcmd-1.0.34/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.33-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.34-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.33
+    Successfully installed chatcmd-1.0.34
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.33/chatcmd/api.py` & `chatcmd-1.0.34/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.33/chatcmd/chatcmd.py` & `chatcmd-1.0.34/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.33')
+            print('ChatCMD'+' 1.0.34')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.33/chatcmd/commands.py` & `chatcmd-1.0.34/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.33/chatcmd/helpers.py` & `chatcmd-1.0.34/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.33/chatcmd/lookup.py` & `chatcmd-1.0.34/chatcmd/lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .commands import *
 import openai
+import pyperclip
 
 def prompt(conn, cursor, api_key):
     print("""
 
      ######  ##     ##    ###    ########  ######  ##     ## ########
     ##    ## ##     ##   ## ##      ##    ##    ## ###   ### ##     ##
     ##       ##     ##  ##   ##     ##    ##       #### #### ##     ##
```

### Comparing `chatcmd-1.0.33/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.34/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.33
+Version: 1.0.34
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
-    Using cached chatcmd-1.0.33-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.34-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.33
+    Successfully installed chatcmd-1.0.34
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.33/pyproject.toml` & `chatcmd-1.0.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.33"
+version = "1.0.34"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.33/setup.py` & `chatcmd-1.0.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.33",
+    version="1.0.34",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

