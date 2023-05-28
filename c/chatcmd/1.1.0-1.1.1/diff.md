# Comparing `tmp/chatcmd-1.1.0.tar.gz` & `tmp/chatcmd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.1.0.tar", last modified: Sun May 28 15:44:16 2023, max compression
+gzip compressed data, was "chatcmd-1.1.1.tar", last modified: Sun May 28 16:42:22 2023, max compression
```

## Comparing `chatcmd-1.1.0.tar` & `chatcmd-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:44:16.283564 chatcmd-1.1.0/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 15:44:16.283150 chatcmd-1.1.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 15:44:02.000000 chatcmd-1.1.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:44:16.279719 chatcmd-1.1.0/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.0/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.0/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 15:41:38.000000 chatcmd-1.1.0/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.0/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1533 2023-05-28 15:17:48.000000 chatcmd-1.1.0/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2717 2023-05-28 15:02:56.000000 chatcmd-1.1.0/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 15:44:16.282709 chatcmd-1.1.0/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 15:44:16.000000 chatcmd-1.1.0/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 15:41:38.000000 chatcmd-1.1.0/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 15:44:16.283700 chatcmd-1.1.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 15:41:38.000000 chatcmd-1.1.0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.650475 chatcmd-1.1.1/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.1/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:42:22.650152 chatcmd-1.1.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 16:41:45.000000 chatcmd-1.1.1/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.647136 chatcmd-1.1.1/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.1/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.1/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 16:41:45.000000 chatcmd-1.1.1/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.1/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.1/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2905 2023-05-28 16:40:02.000000 chatcmd-1.1.1/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:42:22.649696 chatcmd-1.1.1/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 16:42:22.000000 chatcmd-1.1.1/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 16:41:45.000000 chatcmd-1.1.1/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 16:42:22.650573 chatcmd-1.1.1/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 16:41:45.000000 chatcmd-1.1.1/setup.py
```

### Comparing `chatcmd-1.1.0/LICENSE` & `chatcmd-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.0/PKG-INFO` & `chatcmd-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.0
+Version: 1.1.1
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
-    Using cached chatcmd-1.1.0-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.0
+    Successfully installed chatcmd-1.1.1
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.0/README.md` & `chatcmd-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.0-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.0
+    Successfully installed chatcmd-1.1.1
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.0/chatcmd/api.py` & `chatcmd-1.1.1/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.0/chatcmd/chatcmd.py` & `chatcmd-1.1.1/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.1.0')
+            print('ChatCMD'+' 1.1.1')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.1.0/chatcmd/commands.py` & `chatcmd-1.1.1/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.0/chatcmd/helpers.py` & `chatcmd-1.1.1/chatcmd/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         print(f"Failed to copy command to clipboard. Find how to avoid this error in the documentation.")
 
 def clear_input(input):
     input = re.sub('[^a-zA-Z0-9 -_=]', '', input.strip())
     return input
 
 def validateInput(prompt):
-    if len(prompt.split()) <= 2:
-        return False
-    return True
+    pattern = r'^[A-Za-z0-9 ]+$'
+    if re.match(pattern, str(prompt)):
+        return True
+
+    return False
 
 def validate_api_key(api_key):
     if api_key[0:3] != 'sk-':
         return False
     if len(api_key) != 51:
         return False
     if not re.match("^[a-zA-Z0-9-]+$", api_key):
```

### Comparing `chatcmd-1.1.0/chatcmd/lookup.py` & `chatcmd-1.1.1/chatcmd/lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,35 +20,38 @@
     prompt = clear_input(input("Prompt: "))
 
     if prompt == '':
         prompt(conn, cursor, api_key)
     if prompt == 'exit':
         print('bye...')
         exit()
-    elif validateInput(prompt):
-        command = lookup(prompt, api_key)
-        if command is not None:
-            if no_copy == False:
-                if platform.system() == "Linux":
-                    copy_to_clipboard(command)
-                else:
-                    pyperclip.copy(command)
+    elif validateInput(prompt.strip()):
+        if len(str(prompt.split())) >= 3:
+            command = lookup(prompt, api_key)
+            if command is not None:
+                if no_copy == False:
+                    if platform.system() == "Linux":
+                        copy_to_clipboard(command)
+                    else:
+                        pyperclip.copy(command)
 
-            command = clear_input(command)
+                command = clear_input(command)
 
-            if command.find('there is no command') is True and command.find('There is no specific command') is True:
-                print('there is no command for this!')
-            else:
-                history = add_cmd(conn, cursor, prompt, command.strip())
-                if history is False:
-                    print("Error 1008 Failed to add command to history")
-                print(" " + command.strip())
-                print('')
+                if command.find('there is no command') is True and command.find('There is no specific command') is True:
+                    print('there is no command for this!')
+                else:
+                    history = add_cmd(conn, cursor, prompt, command.strip())
+                    if history is False:
+                        print("Error 1008 Failed to add command to history")
+                    print(" " + command.strip())
+                    print('')
+        else:
+            print("\nPlease type in more than two words.\n")
     else:
-        print("Please type in more than two words.\n")
+        print("\nOnly English characters allowed.\n")
 
 
 def lookup(prompt, api_key):
     try:
         if validate_api_key(api_key) is False:
             print("Error 1009: API key is invalid or missing")
             exit()
```

### Comparing `chatcmd-1.1.0/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.1.1/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.0
+Version: 1.1.1
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
-    Using cached chatcmd-1.1.0-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.1-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.0
+    Successfully installed chatcmd-1.1.1
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.0/pyproject.toml` & `chatcmd-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.1.0"
+version = "1.1.1"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.1.0/setup.py` & `chatcmd-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.1.0",
+    version="1.1.1",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

