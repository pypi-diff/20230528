# Comparing `tmp/chatcmd-1.0.39.tar.gz` & `tmp/chatcmd-1.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.39.tar", last modified: Sun May 28 00:26:33 2023, max compression
+gzip compressed data, was "chatcmd-1.0.40.tar", last modified: Sun May 28 00:29:36 2023, max compression
```

## Comparing `chatcmd-1.0.39.tar` & `chatcmd-1.0.40.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:26:33.177220 chatcmd-1.0.39/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.39/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 00:26:33.176892 chatcmd-1.0.39/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 00:26:19.000000 chatcmd-1.0.39/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:26:33.174134 chatcmd-1.0.39/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.39/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.39/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 00:26:19.000000 chatcmd-1.0.39/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.39/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1468 2023-05-28 00:19:46.000000 chatcmd-1.0.39/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2659 2023-05-28 00:26:04.000000 chatcmd-1.0.39/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:26:33.176511 chatcmd-1.0.39/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 00:26:33.000000 chatcmd-1.0.39/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 00:26:19.000000 chatcmd-1.0.39/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 00:26:33.177308 chatcmd-1.0.39/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 00:26:19.000000 chatcmd-1.0.39/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:29:36.360453 chatcmd-1.0.40/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.40/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 00:29:36.360205 chatcmd-1.0.40/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 00:29:22.000000 chatcmd-1.0.40/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:29:36.357398 chatcmd-1.0.40/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.40/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.40/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-28 00:29:22.000000 chatcmd-1.0.40/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.40/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1477 2023-05-28 00:29:05.000000 chatcmd-1.0.40/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2659 2023-05-28 00:26:04.000000 chatcmd-1.0.40/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 00:29:36.359830 chatcmd-1.0.40/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 00:29:36.000000 chatcmd-1.0.40/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 00:29:22.000000 chatcmd-1.0.40/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 00:29:36.360538 chatcmd-1.0.40/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 00:29:22.000000 chatcmd-1.0.40/setup.py
```

### Comparing `chatcmd-1.0.39/LICENSE` & `chatcmd-1.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.39/PKG-INFO` & `chatcmd-1.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.39
+Version: 1.0.40
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
-    Using cached chatcmd-1.0.39-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.40-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.39
+    Successfully installed chatcmd-1.0.40
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.39/README.md` & `chatcmd-1.0.40/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.39-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.40-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.39
+    Successfully installed chatcmd-1.0.40
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.39/chatcmd/api.py` & `chatcmd-1.0.40/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.39/chatcmd/chatcmd.py` & `chatcmd-1.0.40/chatcmd/chatcmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.39')
+            print('ChatCMD'+' 1.0.40')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.39/chatcmd/commands.py` & `chatcmd-1.0.40/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.39/chatcmd/helpers.py` & `chatcmd-1.0.40/chatcmd/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "  Author Website: https://naif.io\n"
     "----------------------------------------------------------------"
     )
 
 
 def copy_to_clipboard(text):
     try:
-        subprocess.run(['xclip', '-selection', 'clipboard'], input=text, encoding='utf-8', check=True)
+        subprocess.run(['/usr/bin/xclip', '-selection', 'clipboard'], input=text, encoding='utf-8', check=True)
     except subprocess.CalledProcessError:
         print("Failed to copy command to clipboard.")
 
 
 def clear_input(input):
     input = re.sub('[^a-zA-Z0-9 -_=]', '', input.strip())
     return input
```

### Comparing `chatcmd-1.0.39/chatcmd/lookup.py` & `chatcmd-1.0.40/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.39/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.40/chatcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.39
+Version: 1.0.40
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
-    Using cached chatcmd-1.0.39-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.40-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.39
+    Successfully installed chatcmd-1.0.40
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.39/pyproject.toml` & `chatcmd-1.0.40/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.39"
+version = "1.0.40"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.39/setup.py` & `chatcmd-1.0.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.39",
+    version="1.0.40",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

