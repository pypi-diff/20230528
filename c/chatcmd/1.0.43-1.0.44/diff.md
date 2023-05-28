# Comparing `tmp/chatcmd-1.0.43.tar.gz` & `tmp/chatcmd-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.43.tar", last modified: Sun May 28 11:23:24 2023, max compression
+gzip compressed data, was "chatcmd-1.0.44.tar", last modified: Sun May 28 11:26:04 2023, max compression
```

## Comparing `chatcmd-1.0.43.tar` & `chatcmd-1.0.44.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:23:24.715281 chatcmd-1.0.43/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.43/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:23:24.714809 chatcmd-1.0.43/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 11:22:44.000000 chatcmd-1.0.43/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:23:24.711235 chatcmd-1.0.43/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.43/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.43/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 11:22:44.000000 chatcmd-1.0.43/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.43/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1546 2023-05-28 11:22:28.000000 chatcmd-1.0.43/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2701 2023-05-28 10:56:12.000000 chatcmd-1.0.43/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:23:24.714212 chatcmd-1.0.43/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 11:23:24.000000 chatcmd-1.0.43/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 11:22:44.000000 chatcmd-1.0.43/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 11:23:24.715479 chatcmd-1.0.43/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 11:22:44.000000 chatcmd-1.0.43/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:26:04.160090 chatcmd-1.0.44/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.44/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:26:04.159640 chatcmd-1.0.44/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 11:25:47.000000 chatcmd-1.0.44/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:26:04.156908 chatcmd-1.0.44/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.44/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.44/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 11:25:47.000000 chatcmd-1.0.44/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.44/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1546 2023-05-28 11:22:28.000000 chatcmd-1.0.44/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2659 2023-05-28 11:25:52.000000 chatcmd-1.0.44/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 11:26:04.159109 chatcmd-1.0.44/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 11:26:04.000000 chatcmd-1.0.44/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 11:25:47.000000 chatcmd-1.0.44/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 11:26:04.160209 chatcmd-1.0.44/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 11:25:47.000000 chatcmd-1.0.44/setup.py
```

### Comparing `chatcmd-1.0.43/LICENSE` & `chatcmd-1.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.43/PKG-INFO` & `chatcmd-1.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.43
+Version: 1.0.44
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
-    Using cached chatcmd-1.0.43-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.44-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.43
+    Successfully installed chatcmd-1.0.44
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.43/README.md` & `chatcmd-1.0.44/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.43-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.44-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.43
+    Successfully installed chatcmd-1.0.44
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.43/chatcmd/api.py` & `chatcmd-1.0.44/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.43/chatcmd/chatcmd.py` & `chatcmd-1.0.44/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.43')
+            print('ChatCMD'+' 1.0.44')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.43/chatcmd/commands.py` & `chatcmd-1.0.44/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.43/chatcmd/helpers.py` & `chatcmd-1.0.44/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.43/chatcmd/lookup.py` & `chatcmd-1.0.44/chatcmd/lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     if prompt == 'exit':
         print('bye...')
         exit()
     elif validateInput(prompt):
         command = lookup(prompt, api_key)
         if command is not None:
             if platform.system() == "Linux":
-#                 copy_to_clipboard(command)
-                pyperclip.copy(command)
+                copy_to_clipboard(command)
             else:
                 pyperclip.copy(command)
 
             command = clear_input(command)
 
             if command.find('there is no command') is True and command.find('There is no specific command') is True:
                 print('there is no command for this!')
```

### Comparing `chatcmd-1.0.43/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.44/chatcmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.43
+Version: 1.0.44
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
-    Using cached chatcmd-1.0.43-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.44-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.43
+    Successfully installed chatcmd-1.0.44
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.43/pyproject.toml` & `chatcmd-1.0.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.43"
+version = "1.0.44"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.43/setup.py` & `chatcmd-1.0.44/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.43",
+    version="1.0.44",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

