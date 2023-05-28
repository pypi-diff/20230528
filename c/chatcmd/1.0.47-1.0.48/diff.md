# Comparing `tmp/chatcmd-1.0.47.tar.gz` & `tmp/chatcmd-1.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.47.tar", last modified: Sun May 28 11:45:52 2023, max compression
+gzip compressed data, was "chatcmd-1.0.48.tar", last modified: Sun May 28 14:12:25 2023, max compression
```

## Comparing `chatcmd-1.0.47.tar` & `chatcmd-1.0.48.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:45:52.628140 chatcmd-1.0.47/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.47/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:45:52.627739 chatcmd-1.0.47/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 11:45:31.000000 chatcmd-1.0.47/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:45:52.624476 chatcmd-1.0.47/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.47/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.47/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 11:45:31.000000 chatcmd-1.0.47/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.47/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1654 2023-05-28 11:45:17.000000 chatcmd-1.0.47/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2659 2023-05-28 11:25:52.000000 chatcmd-1.0.47/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:45:52.627229 chatcmd-1.0.47/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 11:45:52.000000 chatcmd-1.0.47/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 11:45:31.000000 chatcmd-1.0.47/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 11:45:52.628245 chatcmd-1.0.47/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 11:45:31.000000 chatcmd-1.0.47/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 14:12:25.850433 chatcmd-1.0.48/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.48/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 14:12:25.849805 chatcmd-1.0.48/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 14:11:54.000000 chatcmd-1.0.48/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 14:12:25.846290 chatcmd-1.0.48/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.48/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.48/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 14:11:54.000000 chatcmd-1.0.48/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.48/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1487 2023-05-28 13:56:39.000000 chatcmd-1.0.48/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2659 2023-05-28 11:25:52.000000 chatcmd-1.0.48/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 14:12:25.849249 chatcmd-1.0.48/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 14:12:25.000000 chatcmd-1.0.48/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 14:11:54.000000 chatcmd-1.0.48/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 14:12:25.850644 chatcmd-1.0.48/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 14:11:54.000000 chatcmd-1.0.48/setup.py
```

### Comparing `chatcmd-1.0.47/LICENSE` & `chatcmd-1.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.47/PKG-INFO` & `chatcmd-1.0.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.47
+Version: 1.0.48
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
-    Using cached chatcmd-1.0.47-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.48-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.47
+    Successfully installed chatcmd-1.0.48
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.47/README.md` & `chatcmd-1.0.48/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.47-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.48-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.47
+    Successfully installed chatcmd-1.0.48
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.47/chatcmd/api.py` & `chatcmd-1.0.48/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.47/chatcmd/chatcmd.py` & `chatcmd-1.0.48/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.47')
+            print('ChatCMD'+' 1.0.48')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.47/chatcmd/commands.py` & `chatcmd-1.0.48/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.47/chatcmd/lookup.py` & `chatcmd-1.0.48/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.47/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.48/chatcmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.47
+Version: 1.0.48
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
-    Using cached chatcmd-1.0.47-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.48-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.47
+    Successfully installed chatcmd-1.0.48
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.47/pyproject.toml` & `chatcmd-1.0.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.47"
+version = "1.0.48"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.47/setup.py` & `chatcmd-1.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.47",
+    version="1.0.48",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```
