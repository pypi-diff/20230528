# Comparing `tmp/cracker-0.7.2.tar.gz` & `tmp/cracker-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cracker-0.7.2.tar", last modified: Sat May 27 00:29:51 2023, max compression
+gzip compressed data, was "cracker-0.7.3.tar", last modified: Sun May 28 18:03:37 2023, max compression
```

## Comparing `cracker-0.7.2.tar` & `cracker-0.7.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.589784 cracker-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.593784 cracker-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 00:29:31.000000 cracker-0.7.2/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 00:29:31.000000 cracker-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:29:31.000000 cracker-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-27 00:29:31.000000 cracker-0.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-27 00:29:51.601784 cracker-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-27 00:29:31.000000 cracker-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/config/parser.json
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/cracker_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/icon.jpeg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/keylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/mp3_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/speaker/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/abstract_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/espeak.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/speaker/polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/ssml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/tests/test_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/cracker/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/config_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/parser_config_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-27 00:29:31.000000 cracker-0.7.2/cracker/view/speaker_config_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.597784 cracker-0.7.2/cracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 00:29:51.000000 cracker-0.7.2/cracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-27 00:29:31.000000 cracker-0.7.2/docs/macos.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 00:29:31.000000 cracker-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:29:51.601784 cracker-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:29:51.601784 cracker-0.7.2/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/cracker.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-27 00:29:31.000000 cracker-0.7.2/ubuntu/install_ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.319802 cracker-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.307801 cracker-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.311801 cracker-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-28 18:03:23.000000 cracker-0.7.3/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-28 18:03:23.000000 cracker-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 18:03:23.000000 cracker-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 18:03:23.000000 cracker-0.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-28 18:03:37.319802 cracker-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-28 18:03:23.000000 cracker-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.311801 cracker-0.7.3/cracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/config/parser.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/cracker_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/icon.jpeg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/keylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/mp3_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/speaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/abstract_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/espeak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/speaker/polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/ssml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/tests/test_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/config_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/parser_config_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-28 18:03:23.000000 cracker-0.7.3/cracker/view/speaker_config_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/cracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 18:03:37.000000 cracker-0.7.3/cracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.315801 cracker-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-28 18:03:23.000000 cracker-0.7.3/docs/macos.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 18:03:23.000000 cracker-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:03:37.319802 cracker-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:03:37.319802 cracker-0.7.3/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/cracker.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-28 18:03:23.000000 cracker-0.7.3/ubuntu/install_ubuntu.sh
```

### Comparing `cracker-0.7.2/.github/workflows/publish-pypi.yml` & `cracker-0.7.3/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/LICENSE` & `cracker-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/PKG-INFO` & `cracker-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.2
+Version: 0.7.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.2/README.md` & `cracker-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/config/configuration.py` & `cracker-0.7.3/cracker/config/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 import pkgutil
 from typing import Any, Dict, Optional
 
 import yaml
 
 from cracker.speaker import LANGUAGES
-from cracker.utils import deep_dict_merge, get_logger
+from cracker.utils import deep_dict_merge, get_logger, Singleton
 
 
-class Configuration:
+class Configuration(Singleton):
     """Holds configuration values for the application."""
 
     singleton = None
     _logger = get_logger(__name__)
 
     language_file = "voices.json"
     DEFAULT_CONFIG_PATH = "config/default.yaml"
@@ -28,19 +28,14 @@
     voices = []
     speed = 0
     credentials_file = {}
 
     regex_config = None
     raw_config: Optional[Dict] = None
 
-    def __new__(cls, *args, **kwargs):
-        if not cls.singleton:
-            cls.singleton = object.__new__(Configuration)
-        return cls.singleton
-
     def read_config(self) -> Dict[str, Any]:
         """Reads configuration from file system.
 
         Firstly checks whether there are any user defined config in ~/.config/cracker/.
         If config isn't there then it takes the default.
         """
         # Check defaults
```

### Comparing `cracker-0.7.2/cracker/config/parser.json` & `cracker-0.7.3/cracker/config/parser.json`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/cracker.py` & `cracker-0.7.3/cracker/cracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         return config
 
     def change_speaker(self, speaker_name):
         """Action on changing speaker.
 
         Important: Each speaker has its own configuration. These values should be updated on change.
         """
-        self.speaker = self.SPEAKER[speaker_name](self.player)
+        self.speaker = self.get_speaker(speaker_name, self.player)
         self.gui.change_speaker(speaker_name)
 
     def set_action(self):
         self.gui.stop_action.triggered.connect(self.stop_text)
         self.gui.read_action.triggered.connect(self.read_text_area)
         self.gui.clipboard_read_action.triggered.connect(self.toggle_read_text_clipboard)
         self.gui.toggle_action.triggered.connect(self.toggle_read)
```

### Comparing `cracker-0.7.2/cracker/cracker_gui.py` & `cracker-0.7.3/cracker/cracker_gui.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/icon.jpeg` & `cracker-0.7.3/cracker/icon.jpeg`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/icon.png` & `cracker-0.7.3/cracker/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/keylogger.py` & `cracker-0.7.3/cracker/keylogger.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/mp3_helper.py` & `cracker-0.7.3/cracker/mp3_helper.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/speaker/__init__.py` & `cracker-0.7.3/cracker/speaker/__init__.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/speaker/abstract_speaker.py` & `cracker-0.7.3/cracker/speaker/abstract_speaker.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/speaker/espeak.py` & `cracker-0.7.3/cracker/speaker/espeak.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/speaker/google.py` & `cracker-0.7.3/cracker/speaker/google.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/speaker/polly.py` & `cracker-0.7.3/cracker/speaker/polly.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/ssml.py` & `cracker-0.7.3/cracker/ssml.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/tests/test_config.py` & `cracker-0.7.3/cracker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/tests/test_text_parser.py` & `cracker-0.7.3/cracker/tests/test_text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/text_parser.py` & `cracker-0.7.3/cracker/text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/themes.py` & `cracker-0.7.3/cracker/themes.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/utils.py` & `cracker-0.7.3/cracker/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,43 @@
 import logging
 from collections.abc import MutableMapping
 from typing import Dict
 
 
+class Singleton(object):
+    _instances = {}
+
+    def __new__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            logging.debug(f"Creating new instance of '{cls}'")
+            cls._instances[cls] = super(Singleton, cls).__new__(cls, *args, **kwargs)
+        return cls._instances[cls]
+
+
+class LoggerConfig(Singleton):
+    _level: int = logging.INFO
+
+    @property
+    def level(self) -> int:
+        return self._level
+
+    @level.setter
+    def level(self, value: int) -> None:
+        self._level = value
+
+
 def get_logger(name: str) -> logging.Logger:
     """Returns a logger with the given name."""
+    logger_config = LoggerConfig()
     logger = logging.getLogger(name)
-    logger.setLevel(logging.DEBUG)
+    logger.setLevel(logger_config.level)
+
     formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     handler = logging.StreamHandler()
-    handler.setLevel(logging.DEBUG)
+    handler.setLevel(logger_config.level)
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     return logger
 
 
 def deep_dict_merge(d1: Dict, d2: Dict) -> Dict:
     """
```

### Comparing `cracker-0.7.2/cracker/view/config_window.py` & `cracker-0.7.3/cracker/view/config_window.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/view/parser_config_tab.py` & `cracker-0.7.3/cracker/view/parser_config_tab.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker/view/speaker_config_tab.py` & `cracker-0.7.3/cracker/view/speaker_config_tab.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/cracker.egg-info/PKG-INFO` & `cracker-0.7.3/cracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.2
+Version: 0.7.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.2/cracker.egg-info/SOURCES.txt` & `cracker-0.7.3/cracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/pyproject.toml` & `cracker-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/ubuntu/icon.png` & `cracker-0.7.3/ubuntu/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.2/ubuntu/install_ubuntu.sh` & `cracker-0.7.3/ubuntu/install_ubuntu.sh`

 * *Files identical despite different names*

