# Comparing `tmp/aij-1.1.4.tar.gz` & `tmp/aij-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.1.4.tar", last modified: Fri May 26 21:02:21 2023, max compression
+gzip compressed data, was "aij-1.1.5.tar", last modified: Sat May 27 23:40:45 2023, max compression
```

## Comparing `aij-1.1.4.tar` & `aij-1.1.5.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.758662 aij-1.1.4/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-26 21:02:21.757667 aij-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.4/README.md
--rw-rw-rw-   0        0        0     7018 2023-05-26 21:02:09.000000 aij-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 21:02:21.758662 aij-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.684180 aij-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.719184 aij-1.1.4/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      502 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      167 2023-05-26 21:02:21.000000 aij-1.1.4/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.720183 aij-1.1.4/src/animation/
--rw-rw-rw-   0        0        0     5739 2023-05-25 21:36:22.000000 aij-1.1.4/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.722707 aij-1.1.4/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.1.4/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.723707 aij-1.1.4/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.4/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.725706 aij-1.1.4/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.1.4/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.727706 aij-1.1.4/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.1.4/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.728706 aij-1.1.4/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.1.4/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.731100 aij-1.1.4/src/fact_check/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.1.4/src/fact_check/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.732103 aij-1.1.4/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.4/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.734099 aij-1.1.4/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.1.4/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.736109 aij-1.1.4/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.1.4/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.737109 aij-1.1.4/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.4/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.739113 aij-1.1.4/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.4/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.740109 aij-1.1.4/src/scrape/
--rw-rw-rw-   0        0        0     1823 2023-05-26 12:53:00.000000 aij-1.1.4/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.742114 aij-1.1.4/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.1.4/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.744109 aij-1.1.4/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.4/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.745109 aij-1.1.4/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.4/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.747111 aij-1.1.4/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.4/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.748110 aij-1.1.4/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.4/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.751172 aij-1.1.4/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.4/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.752653 aij-1.1.4/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.1.4/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:02:21.754666 aij-1.1.4/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.4/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.445083 aij-1.1.5/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-27 23:40:45.444081 aij-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.5/README.md
+-rw-rw-rw-   0        0        0     7185 2023-05-27 23:40:32.000000 aij-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 23:40:45.445083 aij-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.370756 aij-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.403757 aij-1.1.5/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      203 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.404754 aij-1.1.5/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.1.5/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.406756 aij-1.1.5/src/category/
+-rw-rw-rw-   0        0        0     6518 2023-05-27 23:18:50.000000 aij-1.1.5/src/category/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.407754 aij-1.1.5/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.1.5/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.408755 aij-1.1.5/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.5/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.410752 aij-1.1.5/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.1.5/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.411756 aij-1.1.5/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.1.5/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.413756 aij-1.1.5/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.1.5/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.414757 aij-1.1.5/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.1.5/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.415754 aij-1.1.5/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.5/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.417756 aij-1.1.5/src/keyboard/
+-rw-rw-rw-   0        0        0     6518 2023-05-27 23:12:06.000000 aij-1.1.5/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.418754 aij-1.1.5/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.1.5/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.420754 aij-1.1.5/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.1.5/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.421754 aij-1.1.5/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.5/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.423756 aij-1.1.5/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.5/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.424754 aij-1.1.5/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.1.5/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.426751 aij-1.1.5/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.1.5/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.428786 aij-1.1.5/src/selfie/
+-rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.1.5/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.430063 aij-1.1.5/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.1.5/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.431073 aij-1.1.5/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.5/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.433070 aij-1.1.5/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.5/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.434073 aij-1.1.5/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.5/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.435083 aij-1.1.5/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.5/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.437083 aij-1.1.5/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.5/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.438082 aij-1.1.5/src/volume/
+-rw-rw-rw-   0        0        0     6737 2023-05-27 23:26:16.000000 aij-1.1.5/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.440084 aij-1.1.5/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.1.5/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.441081 aij-1.1.5/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.5/src/webcam2/__init__.py
```

### Comparing `aij-1.1.4/LICENSE.txt` & `aij-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/PKG-INFO` & `aij-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.4
+Version: 1.1.5
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.4/README.md` & `aij-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/pyproject.toml` & `aij-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.04"
+version = "1.1.05"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -140,15 +140,24 @@
     "deepface",
     "speechbrain",
     "soundfile",
     "transformers",
     "langchain",
     "pytube3",
     "nltk",
-    "spacy"
+    "spacy",
+    "jupyter",
+    "jupyterlab",
+    "jupyterlab-code-formatter",
+    "jupyterlab-git",
+    "jupyterlab-lsp",
+    "pynput",
+    "pynput",
+    "comtypes",
+    "pycaw"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-1.1.4/src/aij.egg-info/PKG-INFO` & `aij-1.1.5/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.4
+Version: 1.1.5
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.4/src/aij.egg-info/SOURCES.txt` & `aij-1.1.5/src/aij.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 src/aij.egg-info/PKG-INFO
 src/aij.egg-info/SOURCES.txt
 src/aij.egg-info/dependency_links.txt
 src/aij.egg-info/entry_points.txt
 src/aij.egg-info/requires.txt
 src/aij.egg-info/top_level.txt
 src/animation/__init__.py
+src/category/__init__.py
 src/chat/__init__.py
 src/download/__init__.py
 src/emotion/__init__.py
 src/entity/__init__.py
 src/face/__init__.py
-src/fact_check/__init__.py
+src/fake/__init__.py
 src/intro/__init__.py
+src/keyboard/__init__.py
 src/knowledge/__init__.py
 src/language/__init__.py
 src/messaging/__init__.py
 src/news/__init__.py
+src/objectron/__init__.py
 src/scrape/__init__.py
+src/selfie/__ini__.py
 src/sentiment/__init__.py
 src/setup/__init__.py
 src/stream/__init__.py
 src/transcribe/__init__.py
 src/translate/__init__.py
 src/voice/__init__.py
+src/volume/__init__.py
 src/webcam/__init__.py
 src/webcam2/__init__.py
```

### Comparing `aij-1.1.4/src/animation/__init__.py` & `aij-1.1.5/src/animation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import os
 import random
 import numpy as np
 import cv2
 
+import docker
+
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
+
 class Animation:
     """
     This class generates an animation of random shapes on a canvas.
     The animation is displayed in a window and then a text message is added to the last frame.
     """
 
     def __init__(self, width, height):
```

### Comparing `aij-1.1.4/src/chat/__init__.py` & `aij-1.1.5/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/download/__init__.py` & `aij-1.1.5/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/emotion/__init__.py` & `aij-1.1.5/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/entity/__init__.py` & `aij-1.1.5/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/face/__init__.py` & `aij-1.1.5/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/fact_check/__init__.py` & `aij-1.1.5/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/intro/__init__.py` & `aij-1.1.5/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/knowledge/__init__.py` & `aij-1.1.5/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/messaging/__init__.py` & `aij-1.1.5/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/news/__init__.py` & `aij-1.1.5/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/scrape/__init__.py` & `aij-1.1.5/src/scrape/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,8 +59,12 @@
     news_text = [preprocess(text) for text in news_text]
     social_media_text = [preprocess(text) for text in social_media_text]
     blog_text = [preprocess(text) for text in blog_text]
 
     # combine the datasets
     training_data = news_text + social_media_text + blog_text
     
-    print(training_data)
+    print(training_data)
+    
+    
+if __name__ == "__main__":
+    main()
```

### Comparing `aij-1.1.4/src/sentiment/__init__.py` & `aij-1.1.5/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/setup/__init__.py` & `aij-1.1.5/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/stream/__init__.py` & `aij-1.1.5/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/transcribe/__init__.py` & `aij-1.1.5/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/translate/__init__.py` & `aij-1.1.5/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/voice/__init__.py` & `aij-1.1.5/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/webcam/__init__.py` & `aij-1.1.5/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.4/src/webcam2/__init__.py` & `aij-1.1.5/src/webcam2/__init__.py`

 * *Files identical despite different names*

