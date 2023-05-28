# Comparing `tmp/chatcmd-1.0.49.tar.gz` & `tmp/chatcmd-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.49.tar", last modified: Sun May 28 15:06:41 2023, max compression
+gzip compressed data, was "chatcmd-1.0.50.tar", last modified: Sun May 28 15:12:44 2023, max compression
```

## Comparing `chatcmd-1.0.49.tar` & `chatcmd-1.0.50.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:06:41.661471 chatcmd-1.0.49/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.49/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 15:06:41.661115 chatcmd-1.0.49/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 15:06:27.000000 chatcmd-1.0.49/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:06:41.658204 chatcmd-1.0.49/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.49/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.49/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3572 2023-05-28 15:06:27.000000 chatcmd-1.0.49/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.49/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1487 2023-05-28 13:56:39.000000 chatcmd-1.0.49/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2717 2023-05-28 15:02:56.000000 chatcmd-1.0.49/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:06:41.660616 chatcmd-1.0.49/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 15:06:41.000000 chatcmd-1.0.49/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 15:06:27.000000 chatcmd-1.0.49/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 15:06:41.661595 chatcmd-1.0.49/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 15:06:27.000000 chatcmd-1.0.49/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:12:44.447167 chatcmd-1.0.50/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.50/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 15:12:44.446743 chatcmd-1.0.50/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-28 15:11:56.000000 chatcmd-1.0.50/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:12:44.443718 chatcmd-1.0.50/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.50/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.50/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3572 2023-05-28 15:11:56.000000 chatcmd-1.0.50/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.0.50/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 15:11:25.000000 chatcmd-1.0.50/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2717 2023-05-28 15:02:56.000000 chatcmd-1.0.50/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:12:44.446330 chatcmd-1.0.50/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 15:12:44.000000 chatcmd-1.0.50/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1798 2023-05-28 15:11:56.000000 chatcmd-1.0.50/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 15:12:44.447298 chatcmd-1.0.50/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-05-28 15:11:56.000000 chatcmd-1.0.50/setup.py
```

### Comparing `chatcmd-1.0.49/LICENSE` & `chatcmd-1.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.49/PKG-INFO` & `chatcmd-1.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.49
+Version: 1.0.50
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
-    Using cached chatcmd-1.0.49-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.50-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.49
+    Successfully installed chatcmd-1.0.50
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.49/README.md` & `chatcmd-1.0.50/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.49-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.50-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.49
+    Successfully installed chatcmd-1.0.50
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.49/chatcmd/api.py` & `chatcmd-1.0.50/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.49/chatcmd/chatcmd.py` & `chatcmd-1.0.50/chatcmd/chatcmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.49')
+            print('ChatCMD'+' 1.0.50')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.49/chatcmd/commands.py` & `chatcmd-1.0.50/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.49/chatcmd/helpers.py` & `chatcmd-1.0.50/chatcmd/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     )
 
 
 def copy_to_clipboard(text):
     try:
         subprocess.run(['/usr/bin/xclip', '-selection', 'clipboard'], input=text, encoding='utf-8', check=True)
     except subprocess.CalledProcessError as e:
-        print(f"Failed to copy command to clipboard: {e}")
-
+        print(f"Failed to copy command to clipboard. If you are connected to Linux via SSH you can use -no-copy option to disable copy feature.")
 
 def clear_input(input):
     input = re.sub('[^a-zA-Z0-9 -_=]', '', input.strip())
     return input
 
 def validateInput(prompt):
     if len(prompt.split()) <= 2:
```

### Comparing `chatcmd-1.0.49/chatcmd/lookup.py` & `chatcmd-1.0.50/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.49/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.50/chatcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.49
+Version: 1.0.50
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
-    Using cached chatcmd-1.0.49-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.50-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.49
+    Successfully installed chatcmd-1.0.50
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.49/pyproject.toml` & `chatcmd-1.0.50/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.49"
+version = "1.0.50"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.49/setup.py` & `chatcmd-1.0.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.49",
+    version="1.0.50",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

