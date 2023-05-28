# Comparing `tmp/raspauto-0.3.0.tar.gz` & `tmp/raspauto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspauto-0.3.0.tar", last modified: Sun May 28 18:49:39 2023, max compression
+gzip compressed data, was "raspauto-0.3.1.tar", last modified: Sun May 28 18:55:54 2023, max compression
```

## Comparing `raspauto-0.3.0.tar` & `raspauto-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.523830 raspauto-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-05-28 18:49:27.000000 raspauto-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-28 18:49:39.523830 raspauto-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-28 18:49:27.000000 raspauto-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.519830 raspauto-0.3.0/raspauto/
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-05-28 18:49:27.000000 raspauto-0.3.0/raspauto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.519830 raspauto-0.3.0/raspauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:49:39.523830 raspauto-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-28 18:49:27.000000 raspauto-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:55:54.378171 raspauto-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-05-28 18:55:40.000000 raspauto-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-28 18:55:54.378171 raspauto-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-28 18:55:40.000000 raspauto-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:55:54.378171 raspauto-0.3.1/raspauto/
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-05-28 18:55:40.000000 raspauto-0.3.1/raspauto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:55:54.378171 raspauto-0.3.1/raspauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-28 18:55:54.000000 raspauto-0.3.1/raspauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-28 18:55:54.000000 raspauto-0.3.1/raspauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:55:54.000000 raspauto-0.3.1/raspauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 18:55:54.000000 raspauto-0.3.1/raspauto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 18:55:54.000000 raspauto-0.3.1/raspauto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:55:54.378171 raspauto-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-28 18:55:40.000000 raspauto-0.3.1/setup.py
```

### Comparing `raspauto-0.3.0/LICENSE` & `raspauto-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raspauto-0.3.0/PKG-INFO` & `raspauto-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspauto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Raspberry Automation Library and Voice Recognition
 Home-page: https://github.com/aattk/raspauto
 Download-URL: https://pypi.org/project/raspauto/
 Author: Alpaslan Tetik
 Author-email: 232arslan104@gmail.com
 License: GNU
 Keywords: raspberry,automotion,control
@@ -51,15 +51,15 @@
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
 import raspauto as ra
-ra.set("telegram_bot_token","bot_password")
+ra.set("Telegram_ID","Password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
```

### Comparing `raspauto-0.3.0/README.md` & `raspauto-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
 import raspauto as ra
-ra.set("telegram_bot_token","bot_password")
+ra.set("Telegram_ID","Password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
```

### Comparing `raspauto-0.3.0/raspauto/__init__.py` & `raspauto-0.3.1/raspauto/__init__.py`

 * *Files identical despite different names*

### Comparing `raspauto-0.3.0/raspauto.egg-info/PKG-INFO` & `raspauto-0.3.1/raspauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspauto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Raspberry Automation Library and Voice Recognition
 Home-page: https://github.com/aattk/raspauto
 Download-URL: https://pypi.org/project/raspauto/
 Author: Alpaslan Tetik
 Author-email: 232arslan104@gmail.com
 License: GNU
 Keywords: raspberry,automotion,control
@@ -51,15 +51,15 @@
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
 import raspauto as ra
-ra.set("telegram_bot_token","bot_password")
+ra.set("Telegram_ID","Password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
```

### Comparing `raspauto-0.3.0/setup.py` & `raspauto-0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 setup_args = dict(
     name='raspauto',
-    version='0.3.0',
+    version='0.3.1',
     description='Raspberry Automation Library and Voice Recognition',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GNU',
     packages=find_packages(),
     author='Alpaslan Tetik',
     author_email='232arslan104@gmail.com',
```

