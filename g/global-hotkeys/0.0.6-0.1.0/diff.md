# Comparing `tmp/global_hotkeys-0.0.6.tar.gz` & `tmp/global_hotkeys-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.0.6.tar", last modified: Sat May 27 09:50:05 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.0.tar", last modified: Sun May 28 07:12:33 2023, max compression
```

## Comparing `global_hotkeys-0.0.6.tar` & `global_hotkeys-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/
--rw-rw-rw-   0        0        0      510 2023-05-27 09:40:22.000000 global_hotkeys-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4648 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3604 2023-05-27 09:48:24.000000 global_hotkeys-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.664204 global_hotkeys-0.0.6/global_hotkeys/
--rw-rw-rw-   0        0        0     1455 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6445 2023-05-27 09:45:49.000000 global_hotkeys-0.0.6/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     2605 2023-05-27 07:53:05.000000 global_hotkeys-0.0.6/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.680204 global_hotkeys-0.0.6/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-27 09:47:39.000000 global_hotkeys-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.684216 global_hotkeys-0.0.6/tests/
--rw-rw-rw-   0        0        0      808 2023-05-27 09:47:24.000000 global_hotkeys-0.0.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/
+-rw-rw-rw-   0        0        0      901 2023-05-28 07:09:12.000000 global_hotkeys-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7234 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5799 2023-05-28 07:03:41.000000 global_hotkeys-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.593903 global_hotkeys-0.1.0/global_hotkeys/
+-rw-rw-rw-   0        0        0     1183 2023-05-28 05:12:09.000000 global_hotkeys-0.1.0/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     9445 2023-05-28 05:59:46.000000 global_hotkeys-0.1.0/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.0/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.612903 global_hotkeys-0.1.0/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     7234 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-28 07:03:54.000000 global_hotkeys-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.614903 global_hotkeys-0.1.0/tests/
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.0/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     1021 2023-05-28 06:32:01.000000 global_hotkeys-0.1.0/tests/test.py
```

### Comparing `global_hotkeys-0.0.6/LICENSE.txt` & `global_hotkeys-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.0.6/global_hotkeys/__init__.py` & `global_hotkeys-0.1.0/global_hotkeys/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 from .hotkey_checker import hotkey_checker
 
-def register_hotkey(key, modifiers, press_callback, release_callback=None):
-	return hotkey_checker.register_hotkey(key, modifiers, press_callback, release_callback)
+def register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release):
+	return hotkey_checker.register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release)
 
-def remove_hotkey(key, modifiers):
-	return hotkey_checker.remove_hotkey(key, modifiers)
+def remove_hotkey(binding):
+	return hotkey_checker.remove_hotkey(binding)
 
 def start_checking_hotkeys():
 	hotkey_checker.start_checking_hotkeys()
 
 def stop_checking_hotkeys():
 	hotkey_checker.shutdown_checker()
 
 def restart_checking_hotkeys():
 	hotkey_checker.restart_checker()
 
 def register_hotkeys(bindings):
-    for binding, keydown_function, keyup_function in bindings:
-        key = binding[-1]
-        modifiers = []
-        for i in range(0, len(binding) - 1):
-            modifiers.append(binding[i])
-
-        register_hotkey(key, modifiers, keydown_function, keyup_function)
+    for _binding, keydown_function, keyup_function, actuate_on_partial_release in bindings:
+        binding = [hotkey.split("+") for hotkey in _binding.replace(" ","").split(",")]
+        register_hotkey(binding, keydown_function, keyup_function, actuate_on_partial_release)
 
 def remove_hotkeys(bindings):
-    for binding in bindings:
-        # To accommodate simply reusing the full binding definition ([key_combo], key-down_handler, key-up handler), we'll get just the keybinding.
-        if isinstance(binding[0], list):
-            binding = binding[0]
-        
-        key = binding[-1]
-        modifiers = []
-        for i in range(0, len(binding) - 1):
-            modifiers.append(binding[i])
-
-        remove_hotkey(key, modifiers)
+    for _binding in bindings:
+        binding = [hotkey.split("+") for hotkey in _binding.replace(" ","").split(",")]
+        remove_hotkey(binding)
 
 # Remove all keybindings.
 # *Note that this also stops the hotkey checking thread.
 def clear_hotkeys():
     hotkey_checker.clear_bindings()
```

