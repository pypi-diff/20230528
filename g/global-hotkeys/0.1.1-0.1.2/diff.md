# Comparing `tmp/global_hotkeys-0.1.1.tar.gz` & `tmp/global_hotkeys-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.1.tar", last modified: Sun May 28 12:19:41 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.2.tar", last modified: Sun May 28 21:40:56 2023, max compression
```

## Comparing `global_hotkeys-0.1.1.tar` & `global_hotkeys-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.626712 global_hotkeys-0.1.1/
--rw-rw-rw-   0        0        0     1073 2023-05-28 12:17:35.000000 global_hotkeys-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7760 2023-05-28 12:19:41.625939 global_hotkeys-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6153 2023-05-28 09:20:56.000000 global_hotkeys-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.602889 global_hotkeys-0.1.1/global_hotkeys/
--rw-rw-rw-   0        0        0     1922 2023-05-28 12:12:13.000000 global_hotkeys-0.1.1/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0     9920 2023-05-28 12:12:04.000000 global_hotkeys-0.1.1/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.1/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.622098 global_hotkeys-0.1.1/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     7760 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 12:19:41.000000 global_hotkeys-0.1.1/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 12:19:41.626712 global_hotkeys-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-28 12:17:43.000000 global_hotkeys-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:19:41.625103 global_hotkeys-0.1.1/tests/
--rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.1/tests/_t.py
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.1/tests/global_snippets.py
--rw-rw-rw-   0        0        0     1021 2023-05-28 12:18:24.000000 global_hotkeys-0.1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.717408 global_hotkeys-0.1.2/
+-rw-rw-rw-   0        0        0     1218 2023-05-28 21:40:10.000000 global_hotkeys-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8736 2023-05-28 21:40:56.716407 global_hotkeys-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6984 2023-05-28 21:39:05.000000 global_hotkeys-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.700407 global_hotkeys-0.1.2/global_hotkeys/
+-rw-rw-rw-   0        0        0     3306 2023-05-28 21:29:56.000000 global_hotkeys-0.1.2/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0    10334 2023-05-28 21:25:45.000000 global_hotkeys-0.1.2/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.2/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.713409 global_hotkeys-0.1.2/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     8736 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:40:56.717408 global_hotkeys-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-28 21:39:20.000000 global_hotkeys-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.715408 global_hotkeys-0.1.2/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.2/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.2/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     1381 2023-05-28 21:29:00.000000 global_hotkeys-0.1.2/tests/test.py
```

### Comparing `global_hotkeys-0.1.1/CHANGELOG.txt` & `global_hotkeys-0.1.2/CHANGELOG.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Change Log
 ==========
 
+0.1.2 (5/28/2023)
+-----------------
+- Added dict binding format support. Also added support for supplying callback parameters for bindings.
+
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
 
 0.1.0 (5/28/2023)
 -----------------
 - Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
```

### Comparing `global_hotkeys-0.1.1/LICENSE.txt` & `global_hotkeys-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.1/PKG-INFO` & `global_hotkeys-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -43,32 +43,58 @@
 
 def print_foo():
     print("Foo")
 
 def print_bar():
     print("Bar")
 
+def print_with_params(params):
+    print(params["test"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
+    ["control + 6", None, print_with_params, False, {"test":5}],
+    
+    # We can even use a dict format now for our bindings as well:
+    {
+        "hotkey": "control + 4",
+        "on_press_callback": None,
+        "on_release_callback": print_with_params,
+        "actuate_on_partial_release": False,
+        "callback_params": {"test": "testing"},
+
+    },
+
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
-#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag, callback_params
+#
+# *Note that callback_params will be passed to both press and release callback functions
+#
+# Or in explicit dict format:
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": <a variable or expression can go here>)
+# }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
 
@@ -89,15 +115,15 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+### Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
 I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
@@ -286,14 +312,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.2 (5/28/2023)
+-----------------
+- Added dict binding format support. Also added support for supplying callback parameters for bindings.
+
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
 
 0.1.0 (5/28/2023)
 -----------------
 - Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
```

### Comparing `global_hotkeys-0.1.1/README.md` & `global_hotkeys-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,58 @@
 
 def print_foo():
     print("Foo")
 
 def print_bar():
     print("Bar")
 
+def print_with_params(params):
+    print(params["test"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
+    ["control + 6", None, print_with_params, False, {"test":5}],
+    
+    # We can even use a dict format now for our bindings as well:
+    {
+        "hotkey": "control + 4",
+        "on_press_callback": None,
+        "on_release_callback": print_with_params,
+        "actuate_on_partial_release": False,
+        "callback_params": {"test": "testing"},
+
+    },
+
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
-#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag, callback_params
+#
+# *Note that callback_params will be passed to both press and release callback functions
+#
+# Or in explicit dict format:
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": <a variable or expression can go here>)
+# }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
 
@@ -72,15 +98,15 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+### Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
 I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
```

### Comparing `global_hotkeys-0.1.1/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.2/global_hotkeys/hotkey_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         return True
 
     def _reset_binding_press_state(self, hotkey_id):
         for i in range(0, len(self.hotkey_actions[hotkey_id][2])):
             self.hotkey_actions[hotkey_id][2][i] = 0
 
-    def register_hotkey(self, binding, press_callback, release_callback, actuate_on_partial_release):
+    def register_hotkey(self, binding, press_callback, release_callback, actuate_on_partial_release, callback_params):
         self._is_valid_binding(binding)
         
         self.hotkey_counter += 1
         id = self.hotkey_counter
 
         hotkey_id = self._find_hotkey_id(binding)
         if hotkey_id != None:
@@ -110,15 +110,15 @@
             )
             return False
 
         # we want to track how far along the binding's chording sequence we've progressed.
         binding_press_state = [0 for i in range(0, len(binding))]
 
         self.hotkeys[id] = binding
-        self.hotkey_actions[id] = [press_callback, release_callback, binding_press_state, actuate_on_partial_release]
+        self.hotkey_actions[id] = [press_callback, release_callback, binding_press_state, actuate_on_partial_release, callback_params]
 
         # print(f"id: {id}")
         # print(str(self.hotkeys))
         # print(str(self.hotkey_actions))
         # print("------")
 
         return True
@@ -191,15 +191,15 @@
             time.sleep(0.02)
             # Exit out if the main thread has terminated.
             if not main_thread().is_alive():
                 break
 
             for id in id_list:
                 hotkey = self.hotkeys[id]
-                press_callback, release_callback, binding_press_state, actuate_on_partial_release = self.hotkey_actions[id]
+                press_callback, release_callback, binding_press_state, actuate_on_partial_release, callback_params = self.hotkey_actions[id]
                 key_state_id = self._find_index_of_first_item_not_matching_in_list(binding_press_state, 2)
                 if(key_state_id is None):
                     raise Exception("binding_press_state was not reset after completion!")
                     continue
                 key_state = binding_press_state[key_state_id]
                 chord = [_to_virtualkey(key) if key != "window" else "window" for key in hotkey[key_state_id]]
 
@@ -229,21 +229,27 @@
                     pressed = self._are_all_keys_not_pressed_in_chord(non_allowed_modifiers)
 
                 if pressed:
                     this_is_the_last_chord = key_state_id == len(hotkey) - 1
                     self.hotkey_actions[id][2][key_state_id] = 1
                     if (key_state != 1) and (this_is_the_last_chord):
                         if press_callback != None:
-                            press_callback()
+                            if callback_params != None:
+                                press_callback(callback_params)
+                            else:
+                                press_callback(callback_params)
                 else:
                     this_is_the_last_chord = key_state_id == len(hotkey) - 1
                     #self.hotkey_actions[id][2] = False
                     if (key_state == 1):
                         if this_is_the_last_chord:
                             if fully_not_pressed or actuate_on_partial_release:
                                 self._reset_binding_press_state(id)
                                 if release_callback != None:
-                                    release_callback()
+                                    if callback_params != None:
+                                        release_callback(callback_params)
+                                    else:
+                                        release_callback()
                         else:
                             self.hotkey_actions[id][2][key_state_id] = 2
 
 hotkey_checker = HotkeyChecker()
```

### Comparing `global_hotkeys-0.1.1/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.2/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.1/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.2/global_hotkeys.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -43,32 +43,58 @@
 
 def print_foo():
     print("Foo")
 
 def print_bar():
     print("Bar")
 
+def print_with_params(params):
+    print(params["test"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
+    ["control + 6", None, print_with_params, False, {"test":5}],
+    
+    # We can even use a dict format now for our bindings as well:
+    {
+        "hotkey": "control + 4",
+        "on_press_callback": None,
+        "on_release_callback": print_with_params,
+        "actuate_on_partial_release": False,
+        "callback_params": {"test": "testing"},
+
+    },
+
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
-#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag, callback_params
+#
+# *Note that callback_params will be passed to both press and release callback functions
+#
+# Or in explicit dict format:
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": <a variable or expression can go here>)
+# }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
 
@@ -89,15 +115,15 @@
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
 Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
 
-## Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+### Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
 I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
 
 ## Additional functionality
 
 You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
 
 ```python
@@ -286,14 +312,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.2 (5/28/2023)
+-----------------
+- Added dict binding format support. Also added support for supplying callback parameters for bindings.
+
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
 
 0.1.0 (5/28/2023)
 -----------------
 - Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
```

### Comparing `global_hotkeys-0.1.1/setup.py` & `global_hotkeys-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.1',
+  version='0.1.2',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
```

### Comparing `global_hotkeys-0.1.1/tests/global_snippets.py` & `global_hotkeys-0.1.2/tests/global_snippets.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.1/tests/test.py` & `global_hotkeys-0.1.2/tests/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,25 +13,37 @@
 
 def print_foo():
     print("Foo")
 
 def print_bar():
     print("Bar")
 
+def print_with_params(params):
+    print(params["test"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
+    ["control + 6", None, print_with_params, False, {"test":5}],
+    {
+        "hotkey": "control + 4",
+        "on_press_callback": None,
+        "on_release_callback": print_with_params,
+        "actuate_on_partial_release": False,
+        "callback_params": {"test": "testing"},
+
+    },
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Register all of our keybindings
 register_hotkeys(bindings)
```

