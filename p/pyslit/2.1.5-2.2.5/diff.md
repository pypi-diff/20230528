# Comparing `tmp/pyslit-2.1.5.tar.gz` & `tmp/pyslit-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslit-2.1.5.tar", last modified: Sat May 27 12:09:39 2023, max compression
+gzip compressed data, was "pyslit-2.2.5.tar", last modified: Sun May 28 06:55:45 2023, max compression
```

## Comparing `pyslit-2.1.5.tar` & `pyslit-2.2.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.842187 pyslit-2.1.5/
--rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     5541 2023-05-27 12:09:39.842187 pyslit-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4998 2023-05-27 12:09:09.000000 pyslit-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.782341 pyslit-2.1.5/pyslit/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.832653 pyslit-2.1.5/pyslit/src/
--rw-rw-rw-   0        0        0     8622 2023-05-27 11:52:33.000000 pyslit-2.1.5/pyslit/src/Music_player.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.822651 pyslit-2.1.5/pyslit/src/pyslit.egg-info/
--rw-rw-rw-   0        0        0     5541 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13307 2023-05-27 10:03:28.000000 pyslit-2.1.5/pyslit/src/pyslit.py
--rw-rw-rw-   0        0        0       42 2023-05-27 12:09:39.842187 pyslit-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1637 2023-05-27 12:07:08.000000 pyslit-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:55:45.756635 pyslit-2.2.5/
+-rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5541 2023-05-28 06:55:45.753638 pyslit-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2023-05-27 12:09:09.000000 pyslit-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 06:55:45.636710 pyslit-2.2.5/pyslit/
+drwxrwxrwx   0        0        0        0 2023-05-28 06:55:45.749641 pyslit-2.2.5/pyslit/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 06:55:45.733650 pyslit-2.2.5/pyslit/src/pyslit.egg-info/
+-rw-rw-rw-   0        0        0     5541 2023-05-28 06:55:44.000000 pyslit-2.2.5/pyslit/src/pyslit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-28 06:55:45.000000 pyslit-2.2.5/pyslit/src/pyslit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:55:44.000000 pyslit-2.2.5/pyslit/src/pyslit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-28 06:55:44.000000 pyslit-2.2.5/pyslit/src/pyslit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 06:55:44.000000 pyslit-2.2.5/pyslit/src/pyslit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13239 2023-05-28 06:47:53.000000 pyslit-2.2.5/pyslit/src/pyslit.py
+-rw-rw-rw-   0        0        0       42 2023-05-28 06:55:45.756635 pyslit-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-05-28 06:49:18.000000 pyslit-2.2.5/setup.py
```

### Comparing `pyslit-2.1.5/LICENSE.txt` & `pyslit-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslit-2.1.5/PKG-INFO` & `pyslit-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslit
-Version: 2.1.5
+Version: 2.2.5
 Summary: Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types
 Author: Ashraq
 Author-email: ashraqmohideen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pyslit-2.1.5/README.md` & `pyslit-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyslit-2.1.5/pyslit/src/pyslit.egg-info/PKG-INFO` & `pyslit-2.2.5/pyslit/src/pyslit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslit
-Version: 2.1.5
+Version: 2.2.5
 Summary: Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types
 Author: Ashraq
 Author-email: ashraqmohideen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pyslit-2.1.5/pyslit/src/pyslit.py` & `pyslit-2.2.5/pyslit/src/pyslit.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,14 @@
 
 
 
 #########################################################################################################
 
 import pyttsx3
 import pygame
-import Music_player
 import speech_recognition as sr
 import pywhatkit
 import wikipedia
 import os
 import requests
 from bs4 import BeautifulSoup
 import datetime
@@ -454,17 +453,14 @@
     pygame.mixer.music.pause()
 def unpause_music():
     pygame.mixer.music.unpause()
 def stop_music():
     pygame.mixer.music.stop()
     pygame.mixer.music.unload()
 
-def music_player():
-    Music_player.run()
-
 listener = sr.Recognizer()
 def listen():
     with sr.Microphone() as source:
         print("Listening.....")
         listener.adjust_for_ambient_noise(source, duration=0.5)
         voice = listener.listen(source)
     try:
```

### Comparing `pyslit-2.1.5/setup.py` & `pyslit-2.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyslit",                     # This is the name of the package
-    version="2.1.5",                        # The initial release version
+    version="2.2.5",                        # The initial release version
     author="Ashraq",                     # Full name of the author
     author_email='ashraqmohideen@gmail.com',
     description="Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

