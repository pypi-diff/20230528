# Comparing `tmp/chatcmd-1.1.1.tar.gz` & `tmp/chatcmd-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.1.1.tar", last modified: Sun May 28 16:42:22 2023, max compression
+gzip compressed data, was "chatcmd-1.1.2.tar", last modified: Sun May 28 16:49:19 2023, max compression
```

## Comparing `chatcmd-1.1.1.tar` & `chatcmd-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.650475 chatcmd-1.1.1/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:42:22.650152 chatcmd-1.1.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 16:41:45.000000 chatcmd-1.1.1/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.647136 chatcmd-1.1.1/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.1/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.1/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 16:41:45.000000 chatcmd-1.1.1/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.1/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.1/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2905 2023-05-28 16:40:02.000000 chatcmd-1.1.1/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.649696 chatcmd-1.1.1/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 16:41:45.000000 chatcmd-1.1.1/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 16:42:22.650573 chatcmd-1.1.1/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 16:41:45.000000 chatcmd-1.1.1/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:49:19.275135 chatcmd-1.1.2/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:49:19.274803 chatcmd-1.1.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 16:49:04.000000 chatcmd-1.1.2/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:49:19.272296 chatcmd-1.1.2/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.2/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.2/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 16:49:04.000000 chatcmd-1.1.2/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.2/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.2/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2892 2023-05-28 16:48:54.000000 chatcmd-1.1.2/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:49:19.274312 chatcmd-1.1.2/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 16:49:19.000000 chatcmd-1.1.2/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 16:49:04.000000 chatcmd-1.1.2/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 16:49:19.275226 chatcmd-1.1.2/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 16:49:04.000000 chatcmd-1.1.2/setup.py
```

### Comparing `chatcmd-1.1.1/LICENSE` & `chatcmd-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.1/PKG-INFO` & `chatcmd-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.1
+Version: 1.1.2
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
-    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.2-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.1
+    Successfully installed chatcmd-1.1.2
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.1/README.md` & `chatcmd-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.2-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.1
+    Successfully installed chatcmd-1.1.2
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.1/chatcmd/api.py` & `chatcmd-1.1.2/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.1/chatcmd/chatcmd.py` & `chatcmd-1.1.2/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.1.1')
+            print('ChatCMD'+' 1.1.2')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.1.1/chatcmd/commands.py` & `chatcmd-1.1.2/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.1/chatcmd/helpers.py` & `chatcmd-1.1.2/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.1/chatcmd/lookup.py` & `chatcmd-1.1.2/chatcmd/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     if prompt == '':
         prompt(conn, cursor, api_key)
     if prompt == 'exit':
         print('bye...')
         exit()
     elif validateInput(prompt.strip()):
-        if len(str(prompt.split())) >= 3:
+        if len(prompt) >= 3:
             command = lookup(prompt, api_key)
             if command is not None:
                 if no_copy == False:
                     if platform.system() == "Linux":
                         copy_to_clipboard(command)
                     else:
                         pyperclip.copy(command)
```

### Comparing `chatcmd-1.1.1/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.1.2/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.1
+Version: 1.1.2
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
-    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.2-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.1
+    Successfully installed chatcmd-1.1.2
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.1/pyproject.toml` & `chatcmd-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.1.1"
+version = "1.1.2"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.1.1/setup.py` & `chatcmd-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.1.1",
+    version="1.1.2",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

