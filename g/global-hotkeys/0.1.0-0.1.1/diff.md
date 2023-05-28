# Comparing `tmp/global_hotkeys-0.1.0.tar.gz` & `tmp/global_hotkeys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.0.tar", last modified: Sun May 28 07:12:33 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.1.tar", last modified: Sun May 28 12:19:41 2023, max compression
```

## Comparing `global_hotkeys-0.1.0.tar` & `global_hotkeys-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/
--rw-rw-rw-   0        0        0      901 2023-05-28 07:09:12.000000 global_hotkeys-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7234 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5799 2023-05-28 07:03:41.000000 global_hotkeys-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.593903 global_hotkeys-0.1.0/global_hotkeys/
--rw-rw-rw-   0        0        0     1183 2023-05-28 05:12:09.000000 global_hotkeys-0.1.0/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0     9445 2023-05-28 05:59:46.000000 global_hotkeys-0.1.0/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.0/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.612903 global_hotkeys-0.1.0/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     7234 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 07:12:33.000000 global_hotkeys-0.1.0/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 07:12:33.615902 global_hotkeys-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-28 07:03:54.000000 global_hotkeys-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 07:12:33.614903 global_hotkeys-0.1.0/tests/
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.0/tests/global_snippets.py
--rw-rw-rw-   0        0        0     1021 2023-05-28 06:32:01.000000 global_hotkeys-0.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.626712 global_hotkeys-0.1.1/
+-rw-rw-rw-   0        0        0     1073 2023-05-28 12:17:35.000000 global_hotkeys-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7760 2023-05-28 12:19:41.625939 global_hotkeys-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6153 2023-05-28 09:20:56.000000 global_hotkeys-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.602889 global_hotkeys-0.1.1/global_hotkeys/
+-rw-rw-rw-   0        0        0     1922 2023-05-28 12:12:13.000000 global_hotkeys-0.1.1/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     9920 2023-05-28 12:12:04.000000 global_hotkeys-0.1.1/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.1/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.622098 global_hotkeys-0.1.1/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     7760 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:19:41.626712 global_hotkeys-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-28 12:17:43.000000 global_hotkeys-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.625103 global_hotkeys-0.1.1/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.1/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.1/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     1021 2023-05-28 12:18:24.000000 global_hotkeys-0.1.1/tests/test.py
```

### Comparing `global_hotkeys-0.1.0/LICENSE.txt` & `global_hotkeys-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.0/PKG-INFO` & `global_hotkeys-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# Python Global Hotkey Binding manager for Windows
+# Python Global Hotkey Bindings for Windows
 
 Use this library to set system wide keybindings for your code to respond to.
 
 ## Installation
 
 ```
 pip install global-hotkeys -U
@@ -59,18 +59,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Bindings take on the form of <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
-# It's useful to have 'actuate_on_partial_release_flag' set to False, so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+# Bindings take on the form of:
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
 
-# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, and additional key chords are separated by commas. Spaces are ignored.
+# It's useful to have 'actuate_on_partial_release_flag' set to False, 
+# so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+
+# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
+# and additional key chords are separated by commas. Spaces are ignored.
 
 # Register all of our keybindings
 register_hotkeys(bindings)
 
 # Finally, start listening for keypresses
 start_checking_hotkeys()
 
@@ -85,15 +89,16 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-`I personally use the Hyperkey (which is basically Window+Control+Shift+Alt) to avoid clashing with most application's own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.`
+## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
 
@@ -102,18 +107,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Register a single keybinding (if it's not already registered). Returns True if the key didn't already exist and was added, else False (the binding is already registered - remove it first if you wish to overwrite it with new event handlers).
+# Register a single keybinding (if it's not already registered). 
+# Returns True if the key didn't already exist and was added, 
+# else False (the binding is already registered - remove it first if 
+# you wish to overwrite it with new event handlers).
 register_hotkey(bindings[0])
 
-# Remove a single keybinding (if it exists). Returns True if the key existed and was removed, else False (the binding is already gone).
+# Remove a single keybinding (if it exists). 
+# Returns True if the key existed and was removed, else False (the binding is already gone).
 remove_hotkey(bindings[0])
 
 # Register a list of keybindings.
 register_hotkeys(bindings)
 
 # Remove a list of keybindings.
 remove_hotkeys(bindings)
@@ -277,14 +286,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.1 (5/28/2023)
+-----------------
+- Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
+
 0.1.0 (5/28/2023)
 -----------------
 - Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
 
 0.0.6 (5/27/2023)
 -----------------
 - Fixed window key detection.
```

### Comparing `global_hotkeys-0.1.0/README.md` & `global_hotkeys-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python Global Hotkey Binding manager for Windows
+# Python Global Hotkey Bindings for Windows
 
 Use this library to set system wide keybindings for your code to respond to.
 
 ## Installation
 
 ```
 pip install global-hotkeys -U
@@ -42,18 +42,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Bindings take on the form of <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
-# It's useful to have 'actuate_on_partial_release_flag' set to False, so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+# Bindings take on the form of:
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
 
-# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, and additional key chords are separated by commas. Spaces are ignored.
+# It's useful to have 'actuate_on_partial_release_flag' set to False, 
+# so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+
+# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
+# and additional key chords are separated by commas. Spaces are ignored.
 
 # Register all of our keybindings
 register_hotkeys(bindings)
 
 # Finally, start listening for keypresses
 start_checking_hotkeys()
 
@@ -68,15 +72,16 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-`I personally use the Hyperkey (which is basically Window+Control+Shift+Alt) to avoid clashing with most application's own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.`
+## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
 
@@ -85,18 +90,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Register a single keybinding (if it's not already registered). Returns True if the key didn't already exist and was added, else False (the binding is already registered - remove it first if you wish to overwrite it with new event handlers).
+# Register a single keybinding (if it's not already registered). 
+# Returns True if the key didn't already exist and was added, 
+# else False (the binding is already registered - remove it first if 
+# you wish to overwrite it with new event handlers).
 register_hotkey(bindings[0])
 
-# Remove a single keybinding (if it exists). Returns True if the key existed and was removed, else False (the binding is already gone).
+# Remove a single keybinding (if it exists). 
+# Returns True if the key existed and was removed, else False (the binding is already gone).
 remove_hotkey(bindings[0])
 
 # Register a list of keybindings.
 register_hotkeys(bindings)
 
 # Remove a list of keybindings.
 remove_hotkeys(bindings)
```

### Comparing `global_hotkeys-0.1.0/global_hotkeys/__init__.py` & `global_hotkeys-0.1.1/global_hotkeys/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 from .hotkey_checker import hotkey_checker
 
+def _syntax_check(binding):
+    if(isinstance(binding, list)):
+        hotkey_string = str(binding)
+        valid_hotkey_string = " + ".join(binding)
+        raise Exception(
+            "You've specified the hotkey as a list. The syntax has changed to being specified as a string now.\n"+
+            f"Your hotkey {hotkey_string} should now be specified as \"{valid_hotkey_string}\""
+        )
+
 def register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release):
+    _syntax_check(binding)
+    return hotkey_checker.register_hotkey([hotkey.split("+") for hotkey in binding.replace(" ","").split(",")], press_callback, release_callback, actuate_on_partial_release)
+
+def _register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release):
 	return hotkey_checker.register_hotkey(binding, press_callback, release_callback, actuate_on_partial_release)
 
 def remove_hotkey(binding):
 	return hotkey_checker.remove_hotkey(binding)
 
 def start_checking_hotkeys():
 	hotkey_checker.start_checking_hotkeys()
@@ -13,16 +26,17 @@
 	hotkey_checker.shutdown_checker()
 
 def restart_checking_hotkeys():
 	hotkey_checker.restart_checker()
 
 def register_hotkeys(bindings):
     for _binding, keydown_function, keyup_function, actuate_on_partial_release in bindings:
+        _syntax_check(_binding)
         binding = [hotkey.split("+") for hotkey in _binding.replace(" ","").split(",")]
-        register_hotkey(binding, keydown_function, keyup_function, actuate_on_partial_release)
+        _register_hotkey(binding, keydown_function, keyup_function, actuate_on_partial_release)
 
 def remove_hotkeys(bindings):
     for _binding in bindings:
         binding = [hotkey.split("+") for hotkey in _binding.replace(" ","").split(",")]
         remove_hotkey(binding)
 
 # Remove all keybindings.
```

### Comparing `global_hotkeys-0.1.0/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.1/global_hotkeys/hotkey_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,21 @@
 
     def _is_valid_binding(self, binding):
         for chord in binding:
             for key in chord:
                 virtual_key = _to_virtualkey(key)
                 # If the key doesn't exist, throw an exception to bring attention to it.
                 if virtual_key == None:
+                    if(isinstance(key, list)):
+                        hotkey_string = str(key)
+                        valid_hotkey_string = " + ".join(key)
+                        raise Exception(
+                            "You've specified the hotkey as a list. The syntax has changed to being specified as a string now.\n"+
+                            f"Your hotkey {hotkey_string} should now be specified as \"{valid_hotkey_string}\""
+                        )
                     raise Exception(
                         "The key [%s] not a valid virtual keystroke." % key)
                     return False
     
     def remove_hotkey(self, binding):
         self._is_valid_binding(binding)
```

### Comparing `global_hotkeys-0.1.0/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.1/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.0/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.1/global_hotkeys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# Python Global Hotkey Binding manager for Windows
+# Python Global Hotkey Bindings for Windows
 
 Use this library to set system wide keybindings for your code to respond to.
 
 ## Installation
 
 ```
 pip install global-hotkeys -U
@@ -59,18 +59,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Bindings take on the form of <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
-# It's useful to have 'actuate_on_partial_release_flag' set to False, so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+# Bindings take on the form of:
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
 
-# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, and additional key chords are separated by commas. Spaces are ignored.
+# It's useful to have 'actuate_on_partial_release_flag' set to False, 
+# so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+
+# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
+# and additional key chords are separated by commas. Spaces are ignored.
 
 # Register all of our keybindings
 register_hotkeys(bindings)
 
 # Finally, start listening for keypresses
 start_checking_hotkeys()
 
@@ -85,15 +89,16 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-`I personally use the Hyperkey (which is basically Window+Control+Shift+Alt) to avoid clashing with most application's own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.`
+## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
 
@@ -102,18 +107,22 @@
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
-# Register a single keybinding (if it's not already registered). Returns True if the key didn't already exist and was added, else False (the binding is already registered - remove it first if you wish to overwrite it with new event handlers).
+# Register a single keybinding (if it's not already registered). 
+# Returns True if the key didn't already exist and was added, 
+# else False (the binding is already registered - remove it first if 
+# you wish to overwrite it with new event handlers).
 register_hotkey(bindings[0])
 
-# Remove a single keybinding (if it exists). Returns True if the key existed and was removed, else False (the binding is already gone).
+# Remove a single keybinding (if it exists). 
+# Returns True if the key existed and was removed, else False (the binding is already gone).
 remove_hotkey(bindings[0])
 
 # Register a list of keybindings.
 register_hotkeys(bindings)
 
 # Remove a list of keybindings.
 remove_hotkeys(bindings)
@@ -277,14 +286,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.1 (5/28/2023)
+-----------------
+- Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
+
 0.1.0 (5/28/2023)
 -----------------
 - Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
 
 0.0.6 (5/27/2023)
 -----------------
 - Fixed window key detection.
```

### Comparing `global_hotkeys-0.1.0/setup.py` & `global_hotkeys-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.0',
+  version='0.1.1',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
```

### Comparing `global_hotkeys-0.1.0/tests/global_snippets.py` & `global_hotkeys-0.1.1/tests/global_snippets.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.0/tests/test.py` & `global_hotkeys-0.1.1/tests/test.py`

 * *Files identical despite different names*

