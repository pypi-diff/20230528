# Comparing `tmp/chatcmd-1.1.4.tar.gz` & `tmp/chatcmd-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.1.4.tar", last modified: Sun May 28 17:06:10 2023, max compression
+gzip compressed data, was "chatcmd-1.1.6.tar", last modified: Sun May 28 17:46:37 2023, max compression
```

## Comparing `chatcmd-1.1.4.tar` & `chatcmd-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.558565 chatcmd-1.1.4/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.4/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 17:06:10.558184 chatcmd-1.1.4/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4763 2023-05-28 17:06:00.000000 chatcmd-1.1.4/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.555434 chatcmd-1.1.4/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.4/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.4/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 17:06:00.000000 chatcmd-1.1.4/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.4/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.4/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2947 2023-05-28 17:05:29.000000 chatcmd-1.1.4/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:06:10.557721 chatcmd-1.1.4/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     6384 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 17:06:10.000000 chatcmd-1.1.4/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 17:06:00.000000 chatcmd-1.1.4/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 17:06:10.558719 chatcmd-1.1.4/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 17:06:00.000000 chatcmd-1.1.4/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:46:37.226367 chatcmd-1.1.6/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.1.6/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     6492 2023-05-28 17:46:37.225816 chatcmd-1.1.6/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4871 2023-05-28 17:46:19.000000 chatcmd-1.1.6/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:46:37.219084 chatcmd-1.1.6/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.1.6/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.1.6/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3571 2023-05-28 17:46:19.000000 chatcmd-1.1.6/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3985 2023-05-27 22:10:29.000000 chatcmd-1.1.6/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1573 2023-05-28 16:39:19.000000 chatcmd-1.1.6/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2947 2023-05-28 17:05:29.000000 chatcmd-1.1.6/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-28 17:46:37.224878 chatcmd-1.1.6/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     6492 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-28 17:46:37.000000 chatcmd-1.1.6/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-05-28 17:46:19.000000 chatcmd-1.1.6/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-28 17:46:37.226577 chatcmd-1.1.6/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-28 17:46:19.000000 chatcmd-1.1.6/setup.py
```

### Comparing `chatcmd-1.1.4/LICENSE` & `chatcmd-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.4/PKG-INFO` & `chatcmd-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.4
+Version: 1.1.6
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -32,17 +32,18 @@
 License-File: LICENSE
 
 # ChatCMD #
 #### **ChatCMD** is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input. ####
 
 #### Boost Your Productivity, ***Say Goodbye*** to Manual Searches ####
 
-## Features
+## Features ##
 - CLI-based command lookup using ChatGPT.
 - Auto copy command to clipboard.
+- Disable copy feature.
 - Store Data in Sqlite Database.
 - Add or update ChatGPT API key.
 - Validate ChatGPT API key.
 - Display ChatGPT API Key.
 - Display last command.
 - Display last {number} of commands.
 - Delete last Command.
@@ -51,46 +52,46 @@
 - Clear all history records.
 - Display the database file size.
 - Clear and validate user inputs.
 - Clear and validate lookup results to ensure only valid CLI commands are returned.
 - Error handling
 - Display library information.
 
-## Requirements
+## Requirements ##
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
-## Installation
+## Installation ##
     pip3 install chatcmd
     
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.6-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.4
+    Successfully installed chatcmd-1.1.6
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
-## Usage
+## Usage ##
 
 ```
 Usage:
 
 chatcmd [options]
   
 Options:
@@ -106,15 +107,15 @@
   -h, --help                        display this screen.
   -n, --no-copy                     disable copy feature.
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
-## Error Codes
+## Error Codes ##
 Include an exception message for each error if occurs.
 
 | Code |             Description             |
 |------|:-----------------------------------:|
 | 1001 |          General exception          |
 | 1002 |    Failed to connect to database    |
 | 1003 | Failed to get API key from database |
@@ -131,33 +132,40 @@
 | 1014 |    Failed to get list of command    |
 | 1015 |    Failed deleting last command     |
 | 1016 |     Failed to get last command      |
 | 1017 |       Failed clearing history       |
 | 1018 |       Failed to copy command        |
 
 ### Linux copy command issue
-    In order to perform a Graphics-related job in a Unix environment,
-    the DISPLAY variable needs to be set initially.
-    An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
-    To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
-    Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
-    
-    To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
+In order to perform a Graphics-related job in a Unix environment,
+the DISPLAY variable needs to be set initially.
+An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
+To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
+Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
+
+To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
 
-## Screenshots
+## Screenshots ##
 ### Help screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
+### Tested on: ###
+ - Ubuntu 22.04
+ - Windows Server 2022
+ - macOS Ventura 13.0
+
+## Support ##
+[Issues](https://github.com/naifalshaye/chatcmd/issues)
+
+
+Developed and maintained by:
+[Naif Alshaye](https://naif.io) | [https://naif.io](https://naif.io)
 
-## Support
-[New Issue](https://github.com/naifalshaye/chatcmd/issues/new)\
-[naif@naif.io](mailto:naif@naif.io)
 
-Developed by: [Naif Alshaye](https://naif.io)
 ## License
 The MIT License (MIT). Please see License File [MIT License](https://choosealicense.com/licenses/mit/) for more information.
```

### Comparing `chatcmd-1.1.4/README.md` & `chatcmd-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # ChatCMD #
 #### **ChatCMD** is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input. ####
 
 #### Boost Your Productivity, ***Say Goodbye*** to Manual Searches ####
 
-## Features
+## Features ##
 - CLI-based command lookup using ChatGPT.
 - Auto copy command to clipboard.
+- Disable copy feature.
 - Store Data in Sqlite Database.
 - Add or update ChatGPT API key.
 - Validate ChatGPT API key.
 - Display ChatGPT API Key.
 - Display last command.
 - Display last {number} of commands.
 - Delete last Command.
@@ -18,46 +19,46 @@
 - Clear all history records.
 - Display the database file size.
 - Clear and validate user inputs.
 - Clear and validate lookup results to ensure only valid CLI commands are returned.
 - Error handling
 - Display library information.
 
-## Requirements
+## Requirements ##
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
-## Installation
+## Installation ##
     pip3 install chatcmd
     
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.6-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.4
+    Successfully installed chatcmd-1.1.6
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
-## Usage
+## Usage ##
 
 ```
 Usage:
 
 chatcmd [options]
   
 Options:
@@ -73,15 +74,15 @@
   -h, --help                        display this screen.
   -n, --no-copy                     disable copy feature.
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
-## Error Codes
+## Error Codes ##
 Include an exception message for each error if occurs.
 
 | Code |             Description             |
 |------|:-----------------------------------:|
 | 1001 |          General exception          |
 | 1002 |    Failed to connect to database    |
 | 1003 | Failed to get API key from database |
@@ -98,33 +99,40 @@
 | 1014 |    Failed to get list of command    |
 | 1015 |    Failed deleting last command     |
 | 1016 |     Failed to get last command      |
 | 1017 |       Failed clearing history       |
 | 1018 |       Failed to copy command        |
 
 ### Linux copy command issue
-    In order to perform a Graphics-related job in a Unix environment,
-    the DISPLAY variable needs to be set initially.
-    An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
-    To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
-    Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
-    
-    To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
+In order to perform a Graphics-related job in a Unix environment,
+the DISPLAY variable needs to be set initially.
+An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
+To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
+Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
+
+To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
 
-## Screenshots
+## Screenshots ##
 ### Help screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
+### Tested on: ###
+ - Ubuntu 22.04
+ - Windows Server 2022
+ - macOS Ventura 13.0
+
+## Support ##
+[Issues](https://github.com/naifalshaye/chatcmd/issues)
+
+
+Developed and maintained by:
+[Naif Alshaye](https://naif.io) | [https://naif.io](https://naif.io)
 
-## Support
-[New Issue](https://github.com/naifalshaye/chatcmd/issues/new)\
-[naif@naif.io](mailto:naif@naif.io)
 
-Developed by: [Naif Alshaye](https://naif.io)
 ## License
 The MIT License (MIT). Please see License File [MIT License](https://choosealicense.com/licenses/mit/) for more information.
```

### Comparing `chatcmd-1.1.4/chatcmd/api.py` & `chatcmd-1.1.6/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.4/chatcmd/chatcmd.py` & `chatcmd-1.1.6/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD'+' 1.1.4')
+            print('ChatCMD'+' 1.1.6')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.1.4/chatcmd/commands.py` & `chatcmd-1.1.6/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.4/chatcmd/helpers.py` & `chatcmd-1.1.6/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.4/chatcmd/lookup.py` & `chatcmd-1.1.6/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.1.4/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.1.6/chatcmd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.1.4
+Version: 1.1.6
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -32,17 +32,18 @@
 License-File: LICENSE
 
 # ChatCMD #
 #### **ChatCMD** is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input. ####
 
 #### Boost Your Productivity, ***Say Goodbye*** to Manual Searches ####
 
-## Features
+## Features ##
 - CLI-based command lookup using ChatGPT.
 - Auto copy command to clipboard.
+- Disable copy feature.
 - Store Data in Sqlite Database.
 - Add or update ChatGPT API key.
 - Validate ChatGPT API key.
 - Display ChatGPT API Key.
 - Display last command.
 - Display last {number} of commands.
 - Delete last Command.
@@ -51,46 +52,46 @@
 - Clear all history records.
 - Display the database file size.
 - Clear and validate user inputs.
 - Clear and validate lookup results to ensure only valid CLI commands are returned.
 - Error handling
 - Display library information.
 
-## Requirements
+## Requirements ##
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
-## Installation
+## Installation ##
     pip3 install chatcmd
     
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.1.4-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.1.6-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.1.4
+    Successfully installed chatcmd-1.1.6
 
 ### Upgrade ###
     pip3 install --upgrade chatcmd
 
 If pip not installed:
 
     python3 -m pip install --upgrade chatcmd
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
-## Usage
+## Usage ##
 
 ```
 Usage:
 
 chatcmd [options]
   
 Options:
@@ -106,15 +107,15 @@
   -h, --help                        display this screen.
   -n, --no-copy                     disable copy feature.
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
-## Error Codes
+## Error Codes ##
 Include an exception message for each error if occurs.
 
 | Code |             Description             |
 |------|:-----------------------------------:|
 | 1001 |          General exception          |
 | 1002 |    Failed to connect to database    |
 | 1003 | Failed to get API key from database |
@@ -131,33 +132,40 @@
 | 1014 |    Failed to get list of command    |
 | 1015 |    Failed deleting last command     |
 | 1016 |     Failed to get last command      |
 | 1017 |       Failed clearing history       |
 | 1018 |       Failed to copy command        |
 
 ### Linux copy command issue
-    In order to perform a Graphics-related job in a Unix environment,
-    the DISPLAY variable needs to be set initially.
-    An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
-    To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
-    Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
-    
-    To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
+In order to perform a Graphics-related job in a Unix environment,
+the DISPLAY variable needs to be set initially.
+An error can occur when connecting to Linux via SSH, particularly if there is no copy/paste mechanism like Xclip installed.
+To resolve this, you can try installing Xclip using the following command: "sudo apt-get install xclip".
+Additionally, you need to export the DISPLAY variable by running: "export DISPLAY=:0.0".
+
+To avoid the error message, you can use the "-no-copy" option when looking up a command, as it disables the copy feature.
 
-## Screenshots
+## Screenshots ##
 ### Help screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
 <img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
+### Tested on: ###
+ - Ubuntu 22.04
+ - Windows Server 2022
+ - macOS Ventura 13.0
+
+## Support ##
+[Issues](https://github.com/naifalshaye/chatcmd/issues)
+
+
+Developed and maintained by:
+[Naif Alshaye](https://naif.io) | [https://naif.io](https://naif.io)
 
-## Support
-[New Issue](https://github.com/naifalshaye/chatcmd/issues/new)\
-[naif@naif.io](mailto:naif@naif.io)
 
-Developed by: [Naif Alshaye](https://naif.io)
 ## License
 The MIT License (MIT). Please see License File [MIT License](https://choosealicense.com/licenses/mit/) for more information.
```

### Comparing `chatcmd-1.1.4/pyproject.toml` & `chatcmd-1.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "pyperclip >=1.8.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.1.4"
+version = "1.1.6"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.1.4/setup.py` & `chatcmd-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.1.4",
+    version="1.1.6",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

