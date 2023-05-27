# Comparing `tmp/chatcmd-1.0.29.tar.gz` & `tmp/chatcmd-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.29.tar", last modified: Sat May 27 21:53:47 2023, max compression
+gzip compressed data, was "chatcmd-1.0.30.tar", last modified: Sat May 27 22:07:20 2023, max compression
```

## Comparing `chatcmd-1.0.29.tar` & `chatcmd-1.0.30.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.731732 chatcmd-1.0.29/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.29/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:53:47.731485 chatcmd-1.0.29/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:53:24.000000 chatcmd-1.0.29/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.728931 chatcmd-1.0.29/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.29/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.29/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-27 21:53:24.000000 chatcmd-1.0.29/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3507 2023-05-27 21:48:02.000000 chatcmd-1.0.29/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1831 2023-05-27 21:45:32.000000 chatcmd-1.0.29/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2518 2023-05-27 21:45:32.000000 chatcmd-1.0.29/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.731121 chatcmd-1.0.29/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:53:24.000000 chatcmd-1.0.29/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:53:47.731809 chatcmd-1.0.29/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:53:24.000000 chatcmd-1.0.29/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:07:20.260363 chatcmd-1.0.30/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.30/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:07:20.260040 chatcmd-1.0.30/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 22:06:56.000000 chatcmd-1.0.30/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:07:20.257543 chatcmd-1.0.30/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.30/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.30/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-27 22:06:56.000000 chatcmd-1.0.30/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3983 2023-05-27 22:06:42.000000 chatcmd-1.0.30/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1831 2023-05-27 21:45:32.000000 chatcmd-1.0.30/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2518 2023-05-27 21:45:32.000000 chatcmd-1.0.30/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 22:07:20.259622 chatcmd-1.0.30/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 22:07:20.000000 chatcmd-1.0.30/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 22:06:56.000000 chatcmd-1.0.30/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 22:07:20.260449 chatcmd-1.0.30/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 22:06:56.000000 chatcmd-1.0.30/setup.py
```

### Comparing `chatcmd-1.0.29/LICENSE` & `chatcmd-1.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.29/PKG-INFO` & `chatcmd-1.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.29
+Version: 1.0.30
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
-    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.30-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.29
+    Successfully installed chatcmd-1.0.30
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.29/README.md` & `chatcmd-1.0.30/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.30-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.29
+    Successfully installed chatcmd-1.0.30
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.29/chatcmd/api.py` & `chatcmd-1.0.30/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.29/chatcmd/chatcmd.py` & `chatcmd-1.0.30/chatcmd/chatcmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.0.29')
+            print('ChatCMD'+' 1.0.30')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.29/chatcmd/commands.py` & `chatcmd-1.0.30/chatcmd/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,36 +49,47 @@
         print(str(ve))
     except sqlite3.Error as e:
         print(f"Error 1014: Failed to get last command from history: {e}")
     return False
 
 def delete_cmd(conn, cursor):
     try:
-       cursor.execute("DELETE FROM history ORDER BY id DESC LIMIT 1")
-       conn.commit()
-       print("Command deleted successfully.")
+       select_query = "SELECT * FROM history ORDER BY id DESC LIMIT 1"
+       cursor.execute(select_query)
+       latest_record = cursor.fetchone()
+
+       if latest_record:
+           delete_query = "DELETE FROM history WHERE id = ?"
+           cursor.execute(delete_query, (latest_record[0],))
+           conn.commit()
+           print("Latest command deleted successfully.")
+
     except sqlite3.Error as e:
         print(f"Error 1015: Failed deleting last command: {e}")
     return False
 
 def delete_last_num_cmd(conn, cursor, number):
     try:
         if get_commands_count(conn,cursor) == 0:
             print('History is empty.')
         else:
             number = int(number)
             if number < 1:
                 print('Please enter a correct number.')
             else:
-                cursor.execute("DELETE FROM history ORDER BY id DESC LIMIT "+str(number))
-                delete = conn.commit()
-                if number > 1:
-                    print("All "+str(number)+" commands deleted successfully")
-                else:
-                    print("Command deleted successfully")
+                select_query = "SELECT * FROM history ORDER BY id DESC LIMIT "+number
+                cursor.execute(select_query)
+                latest_records = cursor.fetchall()
+
+                if latest_records:
+                    record_ids = [record[0] for record in latest_records]
+                    delete_query = f"DELETE FROM history WHERE id IN ({','.join(['?']*len(record_ids))})"
+                    cursor.execute(delete_query, record_ids)
+                    conn.commit()
+                    print("Commands deleted successfully.")
     except sqlite3.Error as e:
         print(f"Error 1016: Failed to get last command from history: {e}")
 
 def clear_history(conn, cursor):
     try:
         cursor.execute('DELETE FROM history')
         conn.commit()
```

### Comparing `chatcmd-1.0.29/chatcmd/helpers.py` & `chatcmd-1.0.30/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.29/chatcmd/lookup.py` & `chatcmd-1.0.30/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.29/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.30/chatcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.29
+Version: 1.0.30
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
-    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.30-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.29
+    Successfully installed chatcmd-1.0.30
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.29/pyproject.toml` & `chatcmd-1.0.30/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "colorama >=0.4.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.29"
+version = "1.0.30"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.29/setup.py` & `chatcmd-1.0.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.29",
+    version="1.0.30",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

