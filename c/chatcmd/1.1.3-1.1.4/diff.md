# Comparing `tmp/chatcmd-1.1.3.tar.gz` & `tmp/chatcmd-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.1.3.tar", last modified: Sun May 28 16:54:56 2023, max compression
+gzip compressed data, was "chatcmd-1.1.4.tar", last modified: Sun May 28 17:06:10 2023, max compression
```

## Comparing `chatcmd-1.1.3.tar` & `chatcmd-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:54:56.212854 chatcmd-1.1.3/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.3/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:54:56.212532 chatcmd-1.1.3/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 16:54:28.000000 chatcmd-1.1.3/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:54:56.209684 chatcmd-1.1.3/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.3/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.3/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 16:54:28.000000 chatcmd-1.1.3/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.3/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.3/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2938 2023-05-28 16:53:40.000000 chatcmd-1.1.3/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 16:54:56.212066 chatcmd-1.1.3/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 16:54:56.000000 chatcmd-1.1.3/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 16:54:28.000000 chatcmd-1.1.3/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 16:54:56.212984 chatcmd-1.1.3/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 16:54:28.000000 chatcmd-1.1.3/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.558565 chatcmd-1.1.4/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.4/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 17:06:10.558184 chatcmd-1.1.4/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 17:06:00.000000 chatcmd-1.1.4/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.555434 chatcmd-1.1.4/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.4/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.4/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 17:06:00.000000 chatcmd-1.1.4/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.4/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.4/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2947 2023-05-28 17:05:29.000000 chatcmd-1.1.4/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.557721 chatcmd-1.1.4/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 17:06:00.000000 chatcmd-1.1.4/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 17:06:10.558719 chatcmd-1.1.4/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 17:06:00.000000 chatcmd-1.1.4/setup.py
```

### Comparing `chatcmd-1.1.3/LICENSE` & `chatcmd-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.3/PKG-INFO` & `chatcmd-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.3
+Version: 1.1.4
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
-    Using cached chatcmd-1.1.3-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.3
+    Successfully installed chatcmd-1.1.4
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.3/README.md` & `chatcmd-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.3-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.3
+    Successfully installed chatcmd-1.1.4
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.3/chatcmd/api.py` & `chatcmd-1.1.4/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.3/chatcmd/chatcmd.py` & `chatcmd-1.1.4/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.1.3')
+            print('ChatCMD'+' 1.1.4')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.1.3/chatcmd/commands.py` & `chatcmd-1.1.4/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.3/chatcmd/helpers.py` & `chatcmd-1.1.4/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.3/chatcmd/lookup.py` & `chatcmd-1.1.4/chatcmd/lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,22 @@
         if validate_api_key(api_key) is False:
             print("Error 1009: API key is invalid or missing")
             exit()
 
         prompt = prompt
         print("Looking up...\n")
 
-        stop_keywords = ["###", "END", "stop", "Command:", "Syntax:", "Usage:","The command to install MySQL on Windows is:"]
+        stop_keywords = ["###", "END", "stop", "Command:", "Syntax:", "Usage:","Windows is:","is:"]
         response = openai.Completion.create(
             engine='text-davinci-003',
             prompt=f"Please help me with a CLI command lookup, I only need the command without any extra information: Show me the command for {prompt}",
             max_tokens=70,
             n=1,
             stop=None,
             temperature=0.7)
         message = response.choices[0].text.strip()
         return message
 
     except openai.error.OpenAIError as e:
-        print(f"Error 1010: OpenAI API error occurred: {e}")
+        print(f"Error 1010: OpenAI API error occurred: {e}. Please double check your API Key.")
     except Exception as e:
         print(f"Error 1011: Unhandled exception occurred: {e}")
```

### Comparing `chatcmd-1.1.3/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.1.4/chatcmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.3
+Version: 1.1.4
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
-    Using cached chatcmd-1.1.3-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.3
+    Successfully installed chatcmd-1.1.4
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
```

### Comparing `chatcmd-1.1.3/pyproject.toml` & `chatcmd-1.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.1.3"
+version = "1.1.4"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.1.3/setup.py` & `chatcmd-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.1.3",
+    version="1.1.4",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

