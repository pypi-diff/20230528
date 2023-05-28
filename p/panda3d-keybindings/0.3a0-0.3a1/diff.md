# Comparing `tmp/panda3d_keybindings-0.3a0-py3-none-any.whl.zip` & `tmp/panda3d_keybindings-0.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11407 bytes, number of entries: 7
--rw-rw-r--  2.0 unx        0 b- defN 22-May-26 14:22 keybindings/__init__.py
--rw-rw-r--  2.0 unx    20405 b- defN 22-May-26 14:37 keybindings/device_listener.py
--rw-rw-r--  2.0 unx     1525 b- defN 22-Jun-17 17:46 panda3d_keybindings-0.3a0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11153 b- defN 22-Jun-17 17:46 panda3d_keybindings-0.3a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Jun-17 17:46 panda3d_keybindings-0.3a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 22-Jun-17 17:46 panda3d_keybindings-0.3a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      612 b- defN 22-Jun-17 17:46 panda3d_keybindings-0.3a0.dist-info/RECORD
-7 files, 33799 bytes uncompressed, 10309 bytes compressed:  69.5%
+Zip file size: 12075 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 17:27 keybindings/__init__.py
+-rw-r--r--  2.0 unx    22123 b- defN 23-May-28 13:34 keybindings/device_listener.py
+-rw-r--r--  2.0 unx     1525 b- defN 23-May-28 14:30 panda3d_keybindings-0.3a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12194 b- defN 23-May-28 14:30 panda3d_keybindings-0.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 14:30 panda3d_keybindings-0.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-28 14:30 panda3d_keybindings-0.3a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 23-May-28 14:30 panda3d_keybindings-0.3a1.dist-info/RECORD
+7 files, 36558 bytes uncompressed, 10977 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: keybindings/__init__.py
 Comment: 
 
 Filename: keybindings/device_listener.py
 Comment: 
 
-Filename: panda3d_keybindings-0.3a0.dist-info/LICENSE
+Filename: panda3d_keybindings-0.3a1.dist-info/LICENSE
 Comment: 
 
-Filename: panda3d_keybindings-0.3a0.dist-info/METADATA
+Filename: panda3d_keybindings-0.3a1.dist-info/METADATA
 Comment: 
 
-Filename: panda3d_keybindings-0.3a0.dist-info/WHEEL
+Filename: panda3d_keybindings-0.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: panda3d_keybindings-0.3a0.dist-info/top_level.txt
+Filename: panda3d_keybindings-0.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: panda3d_keybindings-0.3a0.dist-info/RECORD
+Filename: panda3d_keybindings-0.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keybindings/device_listener.py

```diff
@@ -1,13 +1,11 @@
 from collections import OrderedDict
 
 from pathlib import Path
 
-import toml
-
 from panda3d.core import InputDevice
 from panda3d.core import ButtonRegistry
 from panda3d.core import Vec2
 from panda3d.core import Vec3
 
 from direct.showbase.DirectObject import DirectObject
 
@@ -39,16 +37,16 @@
         flags = config[1:]
 
         self.sensor = sensor
         if self.sensor in axis_names:
             self.axis = True
         else:
             self.axis = False
-        self.mouse_pos = Vec2(0,0)
-        self.mouse_delta = Vec2(0,0)
+        self.mouse_pos = None
+        self.mouse_delta = None
 
         self.flags = OrderedDict()
         for flag in flags:
             name, arg = flag
             assert name in ['flip', 'scale', 'button<', 'button>', 'exp', 'deadzone']
             if name in ['scale', 'button<', 'button>', 'exp', 'deadzone']:
                 arg = float(arg)
@@ -64,45 +62,67 @@
                 arg = ''
             arg = str(arg)
             flags.append((name, arg))
         return [self.sensor] + flags
 
     def read_raw(self, device):
         """Read the sensor's current state."""
-        if not device is None:  # Not a keyboard
+        if not device in ['keyboard', 'callback']:  # A regular input device
             if self.axis:
                 axis = device.find_axis(InputDevice.Axis[self.sensor])
                 state = axis.value
             else:
                 button = device.find_button(self.sensor)
                 state = button.pressed
-        else:  # Keyboard
+        elif device == 'callback':
+            try:
+                state = base.device_listener.read_callback(self.sensor)
+            except KeyError:
+                state = None
+        elif device == 'keyboard':  # Keyboard
             if self.sensor in self.mouse_sensors:
                 # Do the actual reading
                 if self.sensor in self.mouse_sensors:
                     if base.mouseWatcherNode.has_mouse():
                         mouse_pos = base.mouseWatcherNode.get_mouse()
-                        self.mouse_delta = mouse_pos - self.mouse_pos
+                        if self.mouse_pos is not None:
+                            self.mouse_delta = mouse_pos - self.mouse_pos
+                        else:
+                            self.mouse_delta = None
                         self.mouse_pos = Vec2(mouse_pos)
-                print(self.mouse_delta)
+                    else:
+                        self.mouse_pos = None
+                        self.mouse_delta = None
 
                 # Interpretation
                 if self.sensor in self.delta_sensors:
-                    if self.sensor == "mouse_x_delta":
-                        state = self.mouse_delta.x
+                    if self.mouse_delta is None:
+                        state = None
                     else:
-                        state = self.mouse_delta.y
+                        if self.sensor == "mouse_x_delta":
+                            state = self.mouse_delta.x
+                        else:
+                            state = self.mouse_delta.y
                 else:
-                    if self.sensor == "mouse_x":
-                        state = self.mouse_pos.x
+                    if self.mouse_pos is None:
+                        state = None
                     else:
-                        state = self.mouse_pos.y
-            else:
-                button = ButtonRegistry.ptr().find_button(self.sensor)
-                state = base.mouseWatcherNode.is_button_down(button)
+                        if self.sensor == "mouse_x":
+                            state = self.mouse_pos.x
+                        else:
+                            state = self.mouse_pos.y
+            else:  ## Not a mouse sensor, so it's a regular old key.
+                if not self.sensor.startswith('raw-'):  # Not a raw key
+                    button = ButtonRegistry.ptr().find_button(self.sensor)
+                    state = base.mouseWatcherNode.is_button_down(button)
+                else:  # raw key
+                    button = ButtonRegistry.ptr().find_button(self.sensor[4:])
+                    state = base.mouseWatcherNode.is_raw_button_down(button)
+        else:
+            return ValueError(f"Unknown device '{device}'.")
         return state
 
     def read(self, device):
         """Read and post-process the sensor's current state."""
         state = self.read_raw(device)
         if state is not None:
             for name, arg in self.flags.items():
@@ -196,18 +216,16 @@
         for device, mapping in self.mappings:
             input_state = None
             input_active = False
 
             # Read the device
             if device in devices:
                 input_state = mapping.read(devices[device])
-            elif device == 'keyboard':
-                input_state = mapping.read(None)
-            else:
-                continue
+            elif device in ['keyboard', 'callback']:
+                input_state = mapping.read(device)
 
             # Process the input state
             if input_state is not None:
                 if all(s is None for s in input_state):
                     input_state = None
                 elif self.type in ['button', 'trigger', 'repeater']:
                     if len(input_state) == 1 and isinstance(input_state[0], bool):
@@ -410,15 +428,16 @@
     :assigner:
         FIXME
     :task:
         Creates a task on creation (at sort -10) that reads the state.
     """
     def __init__(self, assigner, config=None, config_file='keybindings.config',
                  task=True, task_args=None,
-                 debug=False):
+                 debug=False,
+                 callbacks=None):
         self.state = {}  # user: state
         self.debug = debug
 
         self.config_file = None
         if config is None:
             self.config_file = config_file
             main_dir = Path(base.main_dir)
@@ -435,14 +454,19 @@
                 task_args = dict(sort=-10)
             base.task_mgr.add(
                 self.freeze_state,
                 "device_listener",
                 **task_args,
             )
 
+        if callbacks is None:
+            self.callbacks = {}
+        else:
+            self.callbacks = callbacks
+
     def connect(self, device):
         """Event handler that is called when a device is discovered."""
 
         if self.debug:
             print("{} found".format(device.device_class.name))
         self.assigner.connect(device)
 
@@ -494,14 +518,27 @@
     def freeze_state(self, task, dt=None):
         users = self.assigner.get_users()
         contexts = self.contexts.keys()
         for user in users:
             self.read(user=user, dt=dt)
         return task.cont
 
+    def read_callback(self, name):
+        if name in self.callbacks:
+            state = self.callbacks[name]()
+        else:
+            state = None
+        return state
+
+    def set_callback(self, name, func):
+        self.callbacks[name] = func
+
+    def del_callback(self, name):
+        del self.callbacks[name]
+        
 
 def parse_config(config_text):
     input_types = [
         'button',
         'trigger',
         'repeater',
         'axis',
@@ -510,15 +547,17 @@
     ]
     config = {}
     config_lines = config_text.splitlines()
     context_name = None
     virtual_input_name = None
     virtual_input_type = None
     for config_line in config_lines:
-        if config_line.startswith('context '):
+        if not config_line or all(c==" " for c in config_line):
+            pass
+        elif config_line.startswith('context '):
             _, _, context_name = config_line.partition(' ')
             context_name = context_name.strip()
             assert context_name not in config, f"Context name '{context_name}' used multiple times."
             config[context_name] = {}
         elif any(config_line.startswith(f'  {it}') for it in input_types):
             config_line = config_line.strip()
             virtual_input_type, _, virtual_input_name = config_line.partition(' ')
@@ -559,18 +598,21 @@
                     sensors_strings.append(':'.join(sensor_strings))
                 sensors_string = ' '.join(sensors_strings)
                 config_string += f'    {device:15}    {sensors_string}\n'
     return config_string
 
 
 def add_device_listener(assigner=None, config=None,
-                        task=None, task_args=None):
+                        task=None, task_args=None,
+                        callbacks=None):
     if assigner is None:
         assigner = LastConnectedAssigner()
     args = {}
     if config is not None:
         args['config'] = config
     if task is not None:
         args['task'] = task
     if task_args is not None:
         args['task_args'] = task_args
+    if callbacks is not None:
+        args['callbacks'] = callbacks
     base.device_listener = DeviceListener(assigner, **args)
```

## Comparing `panda3d_keybindings-0.3a0.dist-info/LICENSE` & `panda3d_keybindings-0.3a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `panda3d_keybindings-0.3a0.dist-info/METADATA` & `panda3d_keybindings-0.3a1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-keybindings
-Version: 0.3a0
+Version: 0.3a1
 Summary: A more abstract interface for using input devices in Panda3D.
 Home-page: https://github.com/TheCheapestPixels/panda3d-keybindings
 Author: TheCheapestPixels
 Author-email: TheCheapestPixels@gmail.com
 License: UNKNOWN
 Keywords: panda3d keybinding keybindings keymapping
 Platform: UNKNOWN
@@ -12,19 +12,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5, <4.*
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: panda3d
-Requires-Dist: toml
 
 panda3d-keybindings
 ===================
 
 Panda3D comes with a nice API suite to work with input devices. In
 particular, it has one for USB HIDs, and one for mouse and keyboard.
 What it does not have is a mechanism to build an abstraction over these
@@ -46,21 +44,22 @@
 * devices connecting or disconnecting. From a game developer's
   perspective, these events should be dealt with under the hood.
 * how devices are identified. A player may use two flight sticks for a
   space simulator. If they're of different makes, they can be identified
   "uniquely", and should be mappable independent of one another. Even
   with two identical sticks, there should be a way to check which is
   which ("Press trigger on left stick"), and label them accordingly.
-  NOTE: Not implemented yet.
+  NOTE: Not implemented yet. May currently be impossible to do cleanly.
+  Uncleanly, Vendor/Product IDs could be used for devices of different
+  makes.
 * providing an interface to work with the mappings.
-  NOTE: Menu to display the current cofiguration exists, and
+  NOTE: Menu to display the current configuration exists, and
   functionality to save the current configuration back to file. The
   DeviceListener's API to change bindings, and menu functionality to do
-  so are missing. Also the menu so far exists only in
-  `examples/minimal/`.
+  so, are missing. See `examples/menu/`.
 * if the state, when polled at different times during a frame, is still
   the same; It just should be. This is quite an edge case, but may cause
   hard to reproduce bugs.
 
 
 Status
 ------
@@ -75,15 +74,15 @@
 
 `pip install panda3d-keybindings`
 
 
 Concepts
 --------
 
-* A `virtual input` a button or axis with a semantic to the game, like
+* A `virtual input` is an input with a semantic to the game, like
   jumping, turning around moving, etc.; It has
   * a type, which is one of
     * `button`: `True` if the button is pressed, `False` otherwise.
     * `trigger`: `True` for the frame in which the button is pressed.
     * `repeater`: `True` whenever its interval elapses and the button is
       still pressed.
     * `axis`: A `float`.
@@ -129,15 +128,15 @@
     )
 
 Now there is a `base.device_listener`. It assumes that the configuration
 file is named `keybindings.config` and is present in the application's
 `base.main_dir`, and it creates a task at `sort=-10` that freezes this
 frame's input state. Other names file names and ways to handle freezing
 can be configured.
-NOTE: Donnt remember off the top of my head how true that is.
+NOTE: Don't remember off the top of my head how true that is.
 
 A keybinding configuration could look like this:
 
     context demo_context
       button demo_button
         gamepad         face_a
         flight_stick    trigger
@@ -178,32 +177,35 @@
 and then kept pressed, it will return `True` in the first frame, then
 again for one frame after the initial cooldown has passed, and
 thereafter whenever the repeating cooldown has passed. For example, a
 repeater that fires after one second, and then every half second, would
 read `repeater:1.0:0.5`.
 
 The mapping lines each start with a device name as managed by the
-assigner (by default Panda3D's device type names are used), and then has
-one sensor for each dimension of the input. `button`, `trigger`,
-`repeater`, and `axis` are one-dimensional, and `axis2d` and `axis3d`
-are two- and three-dimensional respectively. However, in the case of
-axes, pairs of buttons can be used instead. For example:
+assigner (by default Panda3D's device type names are used, plus
+`callback`, see below), and then has one sensor for each dimension of
+the input. `button`, `trigger`, `repeater`, and `axis` are
+one-dimensional, and `axis2d` and `axis3d` are two- and
+three-dimensional respectively. However, in the case of axes, pairs of
+buttons can be used instead. For example:
 
     context demo_context
       axis turning
         gamepad         right_x
         keyboard        arrow_left arrow_right
 
 The arrow buttons will now be read, and their combined value of -1, 0,
 or 1 will be determined.
 
 Sensor names are as provided by Panda3D. Access to the mouse is given
 via the sensors `mouse_x`, `mouse_y`, `mouse_x_delta`, and
 `mouse_y_delta`, with the two latter tracking frame-to-frame changes
-(without respect to frame time).
+(without respect to frame time). For keyboard keys, raw keys may be
+accessed by prefixing the name with `raw-`. NOTE: Raw keys will be
+supported in Panda3D `1.11`.
 
 Each sensor may also be post-processed after being read. Each such step
 is indicated with a flag, some of which may bear a numeric argument, and
 they are again separated by `:` characters. For example, `right_x:flip`
 would invert the axis (multiplying it with -1), while
 `right_x:deadzone=0.02` would turn all results between -0.02 and 0.02 to
 0.0.
@@ -244,32 +246,62 @@
 much time has elapsed. If you want to determine that by yourself as well
 (which I would warn against; We're talking about inputs here, not the
 game world's clock), you *will* have to use your own call as described
 above, and pass a `dt` argument indicating the elapsed time. For a
 trivial example, see `examples/minimal/main_2_manual_task.py`.
 
 
+Callbacks
+---------
+
+So that's all fine and dandy for typical input devices. What if you want
+to treat something else entirely as an input device? As long as you can
+provide a function that takes no arguments, and returns a valid axis or
+button state, we have you covered.
+
+You can pass a dict with name -> function entries during startup:
+
+    add_device_listener(
+        callbacks=dict(
+    	    my_sensor=read_sensors_value,
+	),
+    )
+
+...or you can add and remove them at runtime:
+
+    base.device_listener.set_callback('my_sensor', read_sensors_value)
+    base.device_listener.del_callback('my_sensor')
+
+Then in the keybindings.config, use `callback` as device type, e.g.:
+
+    context demo_context
+      button my_weird_button
+        callback        my_sensor
+
+If no function is currently provided for a sensor, it will be treated
+like a disconnected device.
+
+An example showing how DirectGui widgets can be used as sensors is
+provided in `examples/callbacks/`.
+
+
 TODO
 ----
 
-* Upgrade examples
 * `doubleclick` and `multiclick` virtual input types
+* speed/acceleration-based postprocessors. Click if axis changes fast
+  enough.
+* Click-and-drag support for mouse
 * Uniquely identifying devices, and remove the NOTE above
 * Changing bindings at run time
   * Update DeviceListener / Assigner API
   * Add menu functionality
   * Remove the NOTE above
-* Menu
-  * Abstract it out of `examples/minimal/`
-  * Develop menu along with DeviceListener's change-bindings API
-  * Write a new `device_tester`
-* Multiplayer ...
-  * Assigner
-  * config file
-  * Remove the NOTEs above
-* Click-and-drag support for mouse
 * Sphinx documentation
-* Raw keys: `keyboard = "raw-z"`; Requires Panda3D API support.
 * Throw events
 * `setup.py`: Go over `packages=` again.
+* Multiplayer; Might need a full refactor.
+  * Assigner
+  * config file
+  * Remove the NOTEs above
```

