# Comparing `tmp/kivy_garden.frostedglass-0.4.0.tar.gz` & `tmp/kivy_garden.frostedglass-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_garden.frostedglass-0.4.0.tar", last modified: Sun Apr 30 17:55:49 2023, max compression
+gzip compressed data, was "kivy_garden.frostedglass-0.5.0.tar", last modified: Sun May 28 15:15:11 2023, max compression
```

## Comparing `kivy_garden.frostedglass-0.4.0.tar` & `kivy_garden.frostedglass-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/
--rw-r--r--   0 alpha     (1000) alpha     (1000)        7 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/AUTHORS.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)     1096 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/LICENSE.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/PKG-INFO
--rw-r--r--   0 alpha     (1000) alpha     (1000)     6599 2023-03-02 15:33:41.000000 kivy_garden.frostedglass-0.4.0/README.md
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/
--rw-r--r--   0 alpha     (1000) alpha     (1000)    25768 2023-04-30 17:10:34.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/__init__.py
--rw-r--r--   0 alpha     (1000) alpha     (1000)       23 2023-04-30 17:46:52.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/_version.py
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/tests/
--rw-r--r--   0 alpha     (1000) alpha     (1000)      119 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/tests/test_import.py
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/
--rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/PKG-INFO
--rw-r--r--   0 alpha     (1000) alpha     (1000)      411 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/SOURCES.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)        1 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/dependency_links.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)       90 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/requires.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)       12 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/top_level.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)      200 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/setup.cfg
--rw-r--r--   0 alpha     (1000) alpha     (1000)     1826 2023-03-02 15:33:04.000000 kivy_garden.frostedglass-0.4.0/setup.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)        7 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/AUTHORS.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     1077 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/LICENSE.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/PKG-INFO
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     6372 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/README.md
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-05-28 15:15:11.937657 kivy_garden.frostedglass-0.5.0/kivy_garden/
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)    25024 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/__init__.py
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       22 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/_version.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/tests/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      113 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/tests/test_import.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-05-28 15:15:11.000000 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/PKG-INFO
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      411 2023-05-28 15:15:11.000000 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/SOURCES.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)        1 2023-05-28 15:15:11.000000 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/dependency_links.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       90 2023-05-28 15:15:11.000000 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/requires.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       12 2023-05-28 15:15:11.000000 kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/top_level.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      200 2023-05-28 15:15:11.947657 kivy_garden.frostedglass-0.5.0/setup.cfg
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     1769 2023-05-28 13:54:39.000000 kivy_garden.frostedglass-0.5.0/setup.py
```

### Comparing `kivy_garden.frostedglass-0.4.0/PKG-INFO` & `kivy_garden.frostedglass-0.5.0/kivy_garden.frostedglass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kivy_garden.frostedglass
-Version: 0.4.0
+Name: kivy-garden.frostedglass
+Version: 0.5.0
 Summary: FrostedGlass is a Kivy widget with frosted glass effect.
 Home-page: https://github.com/kivy-garden/frostedglass
 Author: Kivy
 Author-email: kivy@kivy.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/kivy-garden/frostedglass/issues
 Project-URL: Source, https://github.com/kivy-garden/frostedglass
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: ci
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # FrostedGlass
 
 **FrostedGlass** is a widget with translucent frosted glass effect, that
 creates a context with the background behind it.
```

### Comparing `kivy_garden.frostedglass-0.4.0/README.md` & `kivy_garden.frostedglass-0.5.0/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-# FrostedGlass
-
-**FrostedGlass** is a widget with translucent frosted glass effect, that
-creates a context with the background behind it.
-
-The effect created is based on the widget/layout passed in as the background.
-You can control the blur size, saturation, luminosity, overlay color, noise
-opacity, border radius and the outline (color and width).
-
-
-![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/example_1.png?raw=true)
-![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/example_2.gif?raw=true)
-
-[![Github Build Status](https://github.com/kivy-garden/frostedglass/workflows/Garden%20flower/badge.svg)](https://github.com/kivy-garden/frostedglass/actions)
-[![PyPI](https://img.shields.io/pypi/v/kivy_garden.frostedglass?)](https://pypi.org/project/kivy-garden.frostedglass/)
-
-## Install
-    pip install kivy_garden.frostedglass
-
-## Import
-
-**_python_ import:**
-
-    from kivy_garden.frostedglass import FrostedGlass
-
-**or _kvlang_ import:**
-
-    #: import FrostedGlass kivy_garden.frostedglass
-
-## Usage
-
-*FrostedGlass* will apply the effect to the background passed to it. Make sure you assign the correct id of the widget/layout that is behind *FrostedGlass* to the `background` property.
-
-## Example:
-
-<img src="https://github.com/kivy-garden/frostedglass/blob/main/doc/images/kivy_example.png?raw=true">
-
-```kvlang
-Image:
-    id: bg_image
-    pos_hint: {'center_x': 0.5, 'center_y': 0.5}
-    source: 'kivy_logo.png'
-
-FrostedGlass:
-    pos_hint: {'center_x': 0.5, 'center_y': 0.5}
-    size_hint: (None, None)
-    size: (180, 130)
-    background: bg_image
-    blur_size: 20
-    saturation: 1.0
-    luminosity: 1.5
-    overlay_color: "#FFB9008C"
-    noise_opacity: 0.15
-    border_radius:  dp(0), dp(100), dp(0), dp(100)
-    outline_color: "#000000"
-    outline_width: 1.2
-    Label:
-        text: 'FrostedGlass'
-        pos_hint: {'center_x': 0.5, 'center_y': 0.5}
-        bold: True
-        color: 'black'
-        font_size: dp(25)
-```
-
-<br>
-
-## FrostedGlass Showcase:
-
-**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/main/examples)🔷**
-
-https://user-images.githubusercontent.com/73297572/214139558-f995ac2c-77bb-4952-a82b-212e2f31d65f.mp4
-
-<br>
-
-## Overview of *FrostedGlass* creation process
-
-To reach the final result of the **FrostedGlass** widget, the steps described in the image below are followed:
-
-![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/FrostedgGlass_overview.png?raw=true)
-
-<br>
-
-## Features
-
-FrostedGlass is efficient and makes internal optimizations to deliver the best performance while maintaining the quality of the effect, regardless of implementation, for all platforms supported by Kivy.
-
-Overview:
-
-- Automatic effect update, with auto bind to background properties.
-- Updates effect only when needed. The effect update will only occur when some background or FrostedGlass property requires the update.
-- Avoid unnecessary computation of the effect. If any FrostedGlass widget is not visible, it will not be updated.
-- Full control over FrostedGlass properties. The widget is not limited to the frosted glass effect, it can be used simply as an option to achieve gaussian blur of some "background".
-
-<br>
-
-## Guidelines
-
-The FrostedGlass widget is designed to update the effect whenever there is a change to its properties or background properties that requires an effect update, to keep the effect in sync with the background. 
-
-But if it doesn't, you can call the `update_effect()` method manually to update the effect.
-
-If calling the `update_effect()` method did not update the effect, you may need to call the `refresh_effect()` method.
-
-<br>
-
----
-
-## **API**
-
-    background
-
-> Target widget/layout that will be used as a background to **FrostedGlass**.
-> The recomended way to pass the widget is through the widget/layout **id**.
-> 
-> `background` is defaults to `None`.
-
-<br/>
-
-    blur_size
-
-> Size of the gaussian blur aplied to the background.
-
-❗️*Note: Do not pass relative values such as **dp** or **sp**. **FrostedGlass** already
-    manages this automatically, according to the device's screen density.*
-
-> `blur_size` is defaults to `25`.
-
-<br/>
-
-    saturation
-
-> Saturation boost that will be aplied to the background.
-> 
-> `saturation` is defaults to `1.2`.
-
-<br/>
-
-    luminosity
-
-> Luminosity boost that will be aplied to the background.
-> 
-> `luminosity` is defaults to `1.3`.
-
-
-<br/>
-
-    overlay_color
-
-> Color/tint overlay that will be aplied over the background.
-> 
-> `overlay_color` is defaults to `[0.5, 0.5, 0.5, 0.35]`.
-
-<br/>
-
-    noise_opacity
-
-> Opacity of the noise texture layer.
-> 
-> `noise_opacity` is a defaults to `0.08`.
-
-<br/>
-
-    border_radius
-
-> Specifies the radius used for the rounded corners clockwise:
-> top-left, top-right, bottom-right, bottom-left.
-> 
-> `border_radius` is defaults to `[0, 0, 0, 0]`.
-
-<br/>
-
-    outline_color
-
-> Outline color.
-> 
-> `outline_color` is defaults to `[1, 1, 1, 1]`.
-
-<br/>
-
-    outline_width
-
-> Outline width.
-> 
-> `outline_width` is defaults to `1`.
-
-<br/>
-
-    update_effect()
-
-> Updates the effect only once with each method call.
-
-❗️*Note: Use this method to update the effect only if **FrostedGlass** doesn't update automatically.*
-
-<br/>
-
-    refresh_effect()
-
-> Updates the effect only once with each method call. Sould be used as an alternative, when `update_effect()` doesn't update the effect totally.
-
-❗️*Note: Use this method to update the effect only if **FrostedGlass** doesn't update automatically and `update_effect()` was not enough to update the effect.*
-
----
-
-<br>
-
-CI
---
-
-Every push or pull request run the [GitHub Action](https://github.com/kivy-garden/flower/actions) CI.
-It tests the code on various OS and also generates wheels that can be released on PyPI upon a
-tag. Docs are also generated and uploaded to the repo as well as artifacts of the CI.
-
-Contributing
---------------
-
-Check out our [contribution guide](CONTRIBUTING.md) and feel free to improve the FrostedGlass flower.
-
-🔴 If you have a bug or an idea, create a report to help us improve or suggest an idea for this project by opening an issue
-
-🔴 Every contribution is welcome and appreciated!!!
-
-License
----------
-
-This software is released under the terms of the MIT License.
-Please see the [LICENSE.txt](LICENSE.txt) file.
-
+# FrostedGlass
+
+**FrostedGlass** is a widget with translucent frosted glass effect, that
+creates a context with the background behind it.
+
+The effect created is based on the widget/layout passed in as the background.
+You can control the blur size, saturation, luminosity, overlay color, noise
+opacity, border radius and the outline (color and width).
+
+
+![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/example_1.png?raw=true)
+![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/example_2.gif?raw=true)
+
+[![Github Build Status](https://github.com/kivy-garden/frostedglass/workflows/Garden%20flower/badge.svg)](https://github.com/kivy-garden/frostedglass/actions)
+[![PyPI](https://img.shields.io/pypi/v/kivy_garden.frostedglass?)](https://pypi.org/project/kivy-garden.frostedglass/)
+
+## Install
+    pip install kivy_garden.frostedglass
+
+## Import
+
+**_python_ import:**
+
+    from kivy_garden.frostedglass import FrostedGlass
+
+**or _kvlang_ import:**
+
+    #: import FrostedGlass kivy_garden.frostedglass
+
+## Usage
+
+*FrostedGlass* will apply the effect to the background passed to it. Make sure you assign the correct id of the widget/layout that is behind *FrostedGlass* to the `background` property.
+
+## Example:
+
+<img src="https://github.com/kivy-garden/frostedglass/blob/main/doc/images/kivy_example.png?raw=true">
+
+```kvlang
+Image:
+    id: bg_image
+    pos_hint: {'center_x': 0.5, 'center_y': 0.5}
+    source: 'kivy_logo.png'
+
+FrostedGlass:
+    pos_hint: {'center_x': 0.5, 'center_y': 0.5}
+    size_hint: (None, None)
+    size: (180, 130)
+    background: bg_image
+    blur_size: 20
+    saturation: 1.0
+    luminosity: 1.5
+    overlay_color: "#FFB9008C"
+    noise_opacity: 0.15
+    border_radius:  dp(0), dp(100), dp(0), dp(100)
+    outline_color: "#000000"
+    outline_width: 1.2
+    Label:
+        text: 'FrostedGlass'
+        pos_hint: {'center_x': 0.5, 'center_y': 0.5}
+        bold: True
+        color: 'black'
+        font_size: dp(25)
+```
+
+<br>
+
+## FrostedGlass Showcase:
+
+**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/main/examples)🔷**
+
+https://user-images.githubusercontent.com/73297572/214139558-f995ac2c-77bb-4952-a82b-212e2f31d65f.mp4
+
+<br>
+
+## Overview of *FrostedGlass* creation process
+
+To reach the final result of the **FrostedGlass** widget, the steps described in the image below are followed:
+
+![](https://github.com/kivy-garden/frostedglass/blob/main/doc/images/FrostedgGlass_overview.png?raw=true)
+
+<br>
+
+## Features
+
+FrostedGlass is efficient and makes internal optimizations to deliver the best performance while maintaining the quality of the effect, regardless of implementation, for all platforms supported by Kivy.
+
+Overview:
+
+- Automatic effect update, with auto bind to background properties.
+- Updates effect only when needed. The effect update will only occur when some background or FrostedGlass property requires the update.
+- Avoid unnecessary computation of the effect. If any FrostedGlass widget is not visible, it will not be updated.
+- Full control over FrostedGlass properties. The widget is not limited to the frosted glass effect, it can be used simply as an option to achieve gaussian blur of some "background".
+
+<br>
+
+## Guidelines
+
+The FrostedGlass widget is designed to update the effect whenever there is a change to its properties or background properties that requires an effect update, to keep the effect in sync with the background. 
+
+But if it doesn't, you can call the `update_effect()` method manually to update the effect.
+
+If calling the `update_effect()` method did not update the effect, you may need to call the `refresh_effect()` method.
+
+<br>
+
+---
+
+## **API**
+
+    background
+
+> Target widget/layout that will be used as a background to **FrostedGlass**.
+> The recomended way to pass the widget is through the widget/layout **id**.
+> 
+> `background` is defaults to `None`.
+
+<br/>
+
+    blur_size
+
+> Size of the gaussian blur aplied to the background.
+
+❗️*Note: Do not pass relative values such as **dp** or **sp**. **FrostedGlass** already
+    manages this automatically, according to the device's screen density.*
+
+> `blur_size` is defaults to `25`.
+
+<br/>
+
+    saturation
+
+> Saturation boost that will be aplied to the background.
+> 
+> `saturation` is defaults to `1.2`.
+
+<br/>
+
+    luminosity
+
+> Luminosity boost that will be aplied to the background.
+> 
+> `luminosity` is defaults to `1.3`.
+
+
+<br/>
+
+    overlay_color
+
+> Color/tint overlay that will be aplied over the background.
+> 
+> `overlay_color` is defaults to `[0.5, 0.5, 0.5, 0.35]`.
+
+<br/>
+
+    noise_opacity
+
+> Opacity of the noise texture layer.
+> 
+> `noise_opacity` is a defaults to `0.08`.
+
+<br/>
+
+    border_radius
+
+> Specifies the radius used for the rounded corners clockwise:
+> top-left, top-right, bottom-right, bottom-left.
+> 
+> `border_radius` is defaults to `[0, 0, 0, 0]`.
+
+<br/>
+
+    outline_color
+
+> Outline color.
+> 
+> `outline_color` is defaults to `[1, 1, 1, 1]`.
+
+<br/>
+
+    outline_width
+
+> Outline width.
+> 
+> `outline_width` is defaults to `1`.
+
+<br/>
+
+    update_effect()
+
+> Updates the effect only once with each method call.
+
+❗️*Note: Use this method to update the effect only if **FrostedGlass** doesn't update automatically.*
+
+<br/>
+
+    refresh_effect()
+
+> Updates the effect only once with each method call. Sould be used as an alternative, when `update_effect()` doesn't update the effect totally.
+
+❗️*Note: Use this method to update the effect only if **FrostedGlass** doesn't update automatically and `update_effect()` was not enough to update the effect.*
+
+---
+
+<br>
+
+CI
+--
+
+Every push or pull request run the [GitHub Action](https://github.com/kivy-garden/flower/actions) CI.
+It tests the code on various OS and also generates wheels that can be released on PyPI upon a
+tag. Docs are also generated and uploaded to the repo as well as artifacts of the CI.
+
+Contributing
+--------------
+
+Check out our [contribution guide](CONTRIBUTING.md) and feel free to improve the FrostedGlass flower.
+
+🔴 If you have a bug or an idea, create a report to help us improve or suggest an idea for this project by opening an issue
+
+🔴 Every contribution is welcome and appreciated!!!
+
+License
+---------
+
+This software is released under the terms of the MIT License.
+Please see the [LICENSE.txt](LICENSE.txt) file.
+
```

### Comparing `kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/__init__.py` & `kivy_garden.frostedglass-0.5.0/kivy_garden/frostedglass/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,765 +1,769 @@
-"""
-============
-FrostedGlass
-============
-
-FrostedGlass is a widget with translucent frosted glass effect, that
-creates a context with the background behind it.
-
-The effect created is based on the widget/layout passed in as the background.
-You can control the blur size, saturation, luminosity, overlay color, noise
-opacity, border radius and the outline (color and width).
-"""
-
-__all__ = ("FrostedGlass",)
-
-from ._version import __version__
-
-import os
-from time import perf_counter as now
-
-from kivy.clock import Clock
-from kivy.core.window import Window
-from kivy.graphics import (
-    BindTexture,
-    ClearBuffers,
-    ClearColor,
-    Color,
-    Fbo,
-    Rectangle,
-    RenderContext,
-    RoundedRectangle,
-    Scale,
-    SmoothLine,
-    Translate,
-)
-from kivy.metrics import dp
-from kivy.properties import (
-    ColorProperty,
-    ListProperty,
-    NumericProperty,
-    ObjectProperty,
-)
-from kivy.uix.floatlayout import FloatLayout
-
-# Used for type checking
-from kivy.uix.image import Image
-from kivy.uix.modalview import ModalView
-from kivy.uix.screenmanager import Screen
-from kivy.uix.scrollview import ScrollView
-from kivy.uix.video import Video
-
-MEAN_RES = (Window.width + Window.height) / 2
-
-
-vertical_blur_shader = """
-#ifdef GL_ES
-    precision lowp float;
-#endif
-
-/* Outputs from the vertex shader */
-varying vec4 frag_color;
-varying vec2 tex_coord0;
-
-/* uniform texture samplers */
-uniform sampler2D texture0;
-
-uniform float mean_res;
-uniform float blur_size;
-
-vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
-{{
-    float dt = ((blur_size / 2.0) * 1.0 / mean_res);
-    vec4 sum = vec4(0.0);
-
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+3.0*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+2.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+2.0*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+1.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+1.0*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+0.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-0.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-1.0*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-1.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-2.0*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-2.5*dt))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-3.0*dt))*0.077;
-
-    return frag_color * vec4(sum.rgba);
-}}
-
-void main (void){
-  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
-  vec4 effect_color = effect(
-      normal_color, texture0, tex_coord0, gl_FragCoord.xy
-  );
-  gl_FragColor = effect_color;
-}
-"""
-
-
-horizontal_blur_shader = """
-#ifdef GL_ES
-    precision lowp float;
-#endif
-
-/* Outputs from the vertex shader */
-varying vec4 frag_color;
-varying vec2 tex_coord0;
-
-/* uniform texture samplers */
-uniform sampler2D texture0;
-
-uniform float mean_res;
-uniform float blur_size;
-
-vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
-{{
-    float dt = (blur_size / 2.0) * 1.0 / mean_res;
-    vec4 sum = vec4(0.0);
-
-    sum += texture2D(texture, vec2(tex_coords.x+3.0*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x+2.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x+2.0*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x+1.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x+1.0*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x+0.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-0.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-1.0*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-1.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-2.0*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-2.5*dt, tex_coords.y))*0.077;
-    sum += texture2D(texture, vec2(tex_coords.x-3.0*dt, tex_coords.y))*0.077;
-
-    return  frag_color * vec4(sum.rgba);
-}}
-
-void main (void){
-  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
-  vec4 effect_color = effect(
-      normal_color, texture0, tex_coord0, gl_FragCoord.xy
-  );
-  gl_FragColor = effect_color;
-}
-"""
-
-
-noise_shader = """
-#ifdef GL_ES
-    precision highp float;
-#endif
-
-/* Outputs from the vertex shader */
-varying vec4 frag_color;
-varying vec2 tex_coord0;
-
-/* uniform texture samplers */
-uniform sampler2D texture0;
-
-
-vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
-{{
-    vec4 sum = vec4(0.0);
-    float a = 12.9898;
-    float b = 78.233;
-    float c = 43758.5453;
-    float dt2 = dot(tex_coords.xy, vec2(a, b));
-    float sn= mod(dt2, 3.14);
-    vec4 noise = vec4(fract(sin(sn) * c));
-
-    vec4 bg = texture2D(texture0, tex_coord0);
-    sum = mix(bg, vec4(noise.xyz, 1.0), 1.0);
-
-    return vec4(sum.rgba);
-}}
-
-void main (void){
-  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
-  vec4 effect_color = effect(
-      normal_color, texture0, tex_coord0, gl_FragCoord.xy
-  );
-  gl_FragColor = effect_color;
-}
-"""
-
-
-final_shader_effect = """
-#ifdef GL_ES
-    precision highp float;
-#endif
-
-$HEADER$
-
-uniform int add_child_texture;
-uniform float opacity;
-uniform float luminosity;
-uniform float saturation;
-uniform float noise_opacity;
-uniform vec2 position;
-uniform vec2 resolution;
-uniform vec4 color_overlay;
-uniform sampler2D texture1;
-uniform sampler2D texture2;
-
-void main(void)
-{
-    vec2 pos = (gl_FragCoord.xy - position.xy) / resolution.xy;
-    float noise = 0.0;
-    vec4 textureResult = vec4(0.0);
-    vec4 effect_texture = texture2D(texture1, pos);
-    vec4 noise_texture = texture2D(texture2, tex_coord0);
-
-    const vec3 W = vec3(0.2125, 0.7154, 0.0721);
-    vec3 intensity = vec3(dot(effect_texture.rgb, W));
-    effect_texture = vec4(mix(intensity, effect_texture.rgb, saturation), 1.0);
-    effect_texture *= luminosity;
-
-    effect_texture = mix(
-        effect_texture.rgba,
-        vec4(color_overlay.rgb, 1.0),
-        min(1.0, color_overlay.a)
-    );
-    effect_texture = mix(
-        effect_texture.rgba,
-        vec4(noise_texture.rgb, 1.0),
-        min(1.0, noise_opacity)
-    );
-
-    gl_FragColor = vec4(effect_texture.rgb, opacity);
-}
-"""
-
-
-class VerticalBlur(Fbo):
-    def __init__(self, *args, **kwargs):
-        super(VerticalBlur, self).__init__(
-            *args, fs=vertical_blur_shader, **kwargs
-        )
-        self["mean_res"] = MEAN_RES
-        self["blur_size"] = dp(25)
-
-
-class HorizontalBlur(Fbo):
-    def __init__(self, *args, **kwargs):
-        super(HorizontalBlur, self).__init__(
-            *args, fs=horizontal_blur_shader, **kwargs
-        )
-        self.rect = Rectangle()
-        self["mean_res"] = MEAN_RES
-        self["blur_size"] = dp(25)
-
-
-class Noise(Fbo):
-    def __init__(self, *args, **kwargs):
-        super(Noise, self).__init__(*args, fs=noise_shader, **kwargs)
-        self.rect = Rectangle()
-
-
-class FrostedGlass(FloatLayout):
-
-    background = ObjectProperty(None, allownone=True)
-
-    """Target widget/layout that will be used as a background to FrostedGlass.
-    The recomended way to pass the widget is through the id.
-
-    :attr:`background` is a :class:`~kivy.properties.ObjectProperty` and
-    defaults to None."""
-
-    blur_size = NumericProperty(25)
-    """Size of the gaussian blur aplied to the background.
-
-    Note: Do not pass relative values such as dp or sp. FrostedGlass already
-    manages this automatically, according to the device's screen density.
-
-    :attr:`blur_size` is a :class:`~kivy.properties.NumericProperty` and
-    defaults to 25."""
-
-    noise_opacity = NumericProperty(0.1)
-    """Opacity of the noise layer.
-
-    :attr:`noise_opacity` is a :class:`~kivy.properties.NumericProperty` and
-    defaults to 0.1."""
-
-    saturation = NumericProperty(1.2)
-    """Saturation boost that will be aplied to the background.
-
-    :attr:`saturation` is a :class:`~kivy.properties.NumericProperty` and
-    defaults to 1.2."""
-
-    luminosity = NumericProperty(1.3)
-    """Luminosity boost that will be aplied to the background.
-
-    :attr:`luminosity` is a :class:`~kivy.properties.NumericProperty` and
-    defaults to 1.3."""
-
-    overlay_color = ColorProperty([0.5, 0.5, 0.5, 0.5])
-    """Color/tint overlay that will be aplied over the background.
-
-    :attr:`overlay_color` is a :class:`~kivy.properties.ColorProperty` and
-    defaults to [0.5, 0.5, 0.5, 0.35]."""
-
-    border_radius = ListProperty([0, 0, 0, 0])
-    """Specifies the radius used for the rounded corners clockwise:
-    top-left, top-right, bottom-right, bottom-left.
-
-    :attr:`border_radius` is a :class:`~kivy.properties.ListProperty` and
-    defaults to [0, 0, 0, 0]."""
-
-    outline_color = ColorProperty([1.0, 1.0, 1.0, 1.0])
-    """FrostedGlass outline color.
-
-    :attr:`outline_color` is a :class:`~kivy.properties.ColorProperty` and
-    defaults to [1.0, 1.0, 1.0, 1.0]."""
-
-    outline_width = NumericProperty(1)
-    """FrostedGlass outline width.
-
-    :attr:`outline_width` is a :class:`~kivy.properties.NumericProperty` and
-    defaults to 1."""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        fbind = self.fbind
-        fbind("outline_width", self._update_canvas)
-        fbind("outline_color", self._update_canvas)
-        fbind("border_radius", self._update_canvas)
-        fbind("noise_opacity", self.update_effect)
-        fbind("luminosity", self.update_effect)
-        fbind("saturation", self.update_effect)
-        fbind("overlay_color", self.update_effect)
-        fbind("border_radius", self.update_effect)
-
-        self.frosted_glass_effect = RenderContext(
-            use_parent_projection=True,
-            use_parent_modelview=True,
-            fs=final_shader_effect
-        )
-        with self.frosted_glass_effect:
-            self.bt_1 = BindTexture(index=1)
-            self.bt_2 = BindTexture(index=2)
-            self.fbo_rect = RoundedRectangle(
-                size=self.size,
-                pos=self.pos,
-                radius=self.border_radius,
-            )
-        self.frosted_glass_effect["texture1"] = 1
-        self.frosted_glass_effect["texture2"] = 2
-
-        self.canvas.add(self.frosted_glass_effect)
-
-        with self.canvas:
-            self._outline_color = Color(rgba=self.outline_color)
-            self.outline = SmoothLine(
-                width=1,
-                overdraw_width=2,
-                rounded_rectangle=(
-                    self.x, self.y,
-                    self.width, self.height,
-                    1, 1, 1, 1, 45,
-                ),
-            )
-
-        self.noise = Noise(size=(100, 100))
-        self.h_blur = HorizontalBlur(size=(100, 100))
-        self.v_blur = VerticalBlur(size=(100, 100))
-
-        with self.h_blur:
-            ClearColor(0, 0, 0, 0)
-            ClearBuffers()
-            self.h_blur_scale = Scale(1, 1, 1)
-            self.h_blur_translate = Translate(0, 0)
-
-        with self.v_blur:
-            ClearColor(0, 0, 0, 0)
-            ClearBuffers()
-            self.v_blur_scale = Scale(1, 1, 1)
-            self.v_blur_translate = Translate(0, 0)
-
-        self.last_value = 0
-        self.last_update_time = 0
-        self.last_value_list = [0, 0]
-        self.last_blur_size_value = None
-        self.last_fbo_pos = [None, None]
-        self._pos = [0, 0]
-        self.popup_parent = None
-        self.parent_screen = None
-        self.parents_list = []
-        self.background_children_list = []
-        self.background_parents_list = []
-        self._last_background_canvas = None
-
-        self.is_movable = False
-        self.adapted_fbo_size = False
-
-        self._update_glsl_ev = Clock.create_trigger(self._update_glsl, 0)
-        self._update_fbo_ev = Clock.create_trigger(self._update_fbo_effect, 0)
-        self._update_texture_ev = Clock.create_trigger(
-            self._set_final_texture, 0
-        )
-        self._refresh_effect_ev = Clock.create_trigger(
-            self.refresh_effect, 0.033333, True
-        )
-
-        if not os.environ.get("FG_ASK_UPDATE_CANVAS_ACTIVE"):
-            os.environ["FG_ASK_UPDATE_CANVAS_ACTIVE"] = "1"
-            Clock.schedule_interval(lambda dt: Window.canvas.ask_update(), 0)
-
-    def update_effect(self, *args):
-        self._update_glsl_ev()
-
-    def refresh_effect(self, *args):
-        self._update_fbo_ev()
-        self._update_glsl_ev()
-
-    def _update_glsl(self, *args):
-        self._pos = self.to_window(*self.pos)
-        if (
-            self.not_current_screen
-            or self.out_of_the_window
-            and self.background_loaded
-        ):
-            return
-
-        effect = self.frosted_glass_effect
-        effect["position"] = [float(v) for v in self._pos]
-        effect["resolution"] = [float(v) for v in self.size]
-        effect["luminosity"] = float(self.luminosity)
-        effect["saturation"] = float(self.saturation)
-        effect["noise_opacity"] = float(self.noise_opacity)
-        effect["color_overlay"] = [float(v) for v in self.overlay_color]
-
-        if self.is_movable:
-            if not self.adapted_fbo_size:
-                self.refresh_effect()
-                self.adapted_fbo_size = True
-
-            self.h_blur_translate.x = self.v_blur_translate.x = -self._pos[0]
-            self.h_blur_translate.y = self.v_blur_translate.y = (
-                -self._pos[1] - self.size[1]
-            )
-
-        self._update_texture_ev()
-
-    def _set_final_texture(self, pos):
-        if not self.background:
-            return
-
-        if self._last_background_canvas not in self.h_blur.children:
-            self.h_blur.add(self._last_background_canvas)
-            self.v_blur.add(self.h_blur.rect)
-
-        if self.h_blur.rect.texture != self.h_blur.texture:
-            self.h_blur.rect.texture = self.h_blur.texture
-
-        self.h_blur.rect.size = self.size
-        self.h_blur.rect.pos = self._pos
-
-        self.h_blur.draw()
-        self.v_blur.draw()
-        self.v_blur.ask_update()
-
-        self.bt_1.texture = self.v_blur.texture
-
-        if self._update_texture_ev.timeout == 0:
-            self._update_texture_ev.timeout = -1
-
-    def _update_noise_texture(self):
-        fbo_size = max(1, self.width / dp(1)), max(1, self.height / dp(1))
-        self.noise.size = fbo_size
-        self.noise.rect.size = self.size
-        self.noise.add(self.noise.rect)
-        self.noise.draw()
-        self.noise.remove(self.noise.rect)
-        self.bt_2.texture = self.noise.texture
-
-    def _update_fbo_effect(self, *args):
-        if self.is_movable:
-            fbo_size = (min(self.width, 150), min(self.height, 150))
-        else:
-            fbo_size = (min(self.width, 250), min(self.height, 250))
-
-        size = max(1, self.width), max(1, self.height)
-        fbo_size = max(1, fbo_size[0]), max(1, fbo_size[1])
-
-        self.h_blur.size = fbo_size
-        self.v_blur.size = fbo_size
-
-        pos = self.to_window(*self.pos)
-        x = 1 / (size[0] / fbo_size[0])
-        y = 1 / (size[1] / fbo_size[1])
-
-        self.h_blur_scale.x = self.v_blur_scale.x = x
-        self.h_blur_scale.y = self.v_blur_scale.y = -y
-        self.h_blur_translate.x = self.v_blur_translate.x = -pos[0]
-        self.h_blur_translate.y = self.v_blur_translate.y = -pos[1] - size[1]
-
-    def on_touch_down(self, touch):
-        if self.collide_point(*touch.pos):
-            super().on_touch_down(touch)
-            return True
-        return super().on_touch_down(touch)
-
-    def on_size(self, instance, size):
-        self._update_canvas()
-        self._update_noise_texture()
-        self.refresh_effect()
-
-    def on_pos(self, *args):
-        self._update_canvas()
-        self.refresh_effect()
-
-    def _update_canvas(self, *args):
-        border_radius = list(
-            map(
-                lambda x: max(1, min(min(self.width, self.height) / 2, x)),
-                self.border_radius,
-            )
-        )
-        self.fbo_rect.size = self.size
-        self.fbo_rect.pos = self.pos
-        self.fbo_rect.radius = border_radius
-
-        self._outline_color.rgba = self.outline_color
-        self.outline.width = self.outline_width
-        self.outline.rounded_rectangle = (
-            self.x, self.y,
-            self.width, self.height,
-            *reversed(border_radius), 45,
-        )
-
-    def on_blur_size(self, instance, blur_size):
-        blur_size = int(blur_size)
-        if blur_size != self.last_blur_size_value:
-            self.v_blur["blur_size"] = dp(blur_size)
-            self.h_blur["blur_size"] = dp(blur_size)
-            self.update_effect()
-            self.last_blur_size_value = blur_size
-
-    def on_background(self, _, background):
-        if not background:
-            return
-
-        if self._last_background_canvas in self.h_blur.children:
-            self.h_blur.remove(self._last_background_canvas)
-            self.update_effect()
-            self._unbind_parent_properties(self.background_parents_list)
-            self._unbind_children_properties(self.background_children_list)
-
-        self._last_background_canvas = background.canvas
-
-        self.background_parents_list = self._get_all_parents(self.background)
-        self.background_children_list = self._get_all_children(self.background)
-        self._bind_parent_properties(self.background_parents_list)
-        self._bind_children_properties(self.background_children_list)
-
-    def on_parent(self, _, parent):
-        if not parent:
-            return
-
-        self.parents_list = self._get_all_parents(parent)
-        for p in self.parents_list:
-            if isinstance(p, ModalView):
-                self.popup_parent = p
-            if isinstance(p, Screen):
-                self.parent_screen = p
-            if isinstance(p, ScrollView):
-                self.is_movable = True
-        self._bind_parent_properties(self.parents_list)
-
-    def _get_all_parents(self, widget):
-        widgets_list = []
-        parent = widget
-        while True:
-            widgets_list.append(parent)
-            if parent.parent and parent != parent.parent:
-                parent = parent.parent
-            else:
-                break
-        return widgets_list
-
-    def _get_all_children(self, widget):
-        widgets_list = [widget]
-        children_widgets = [widget]
-        while children_widgets:
-            parent_widgets = children_widgets
-            children_widgets = []
-            for w in parent_widgets:
-                if w.children:
-                    widgets_list.extend(w.children)
-                    children_widgets.extend(w.children)
-        return widgets_list
-
-    def _bind_children_properties(self, children_list):
-        properties_to_bind = (
-            "pos",
-            "size",
-            "scroll_x",
-            "scroll_y",
-            "on_open",
-            "on_enter",
-            "texture",
-        )
-        for widget in children_list:
-            for property in properties_to_bind:
-                try:
-                    if property == "texture":
-                        if isinstance(widget, Image):
-                            widget.bind(
-                                texture=self._trigger_update_effect
-                            )
-                        if isinstance(widget, Video):
-                            widget.bind(
-                                position=self._trigger_update_effect
-                            )
-                    elif hasattr(widget, property):
-                        widget.fbind(
-                            property,
-                            self._trigger_update_effect,
-                        )
-                except Exception as e:
-                    print(e)
-                    pass
-
-    def _bind_parent_properties(self, parents_list):
-        for widget in parents_list:
-
-            if isinstance(widget, ScrollView):
-                widget.bind(
-                    size=self._trigger_update_effect,
-                    pos=self._trigger_update_effect,
-                    scroll_x=self._trigger_update_effect,
-                    scroll_y=self._trigger_update_effect,
-                )
-            if isinstance(widget, ModalView):
-                widget.bind(
-                    on_pre_open=self._trigger_update_effect
-                )
-            elif isinstance(widget, Screen):
-                widget.bind(
-                    on_pre_enter=lambda *args: self._refresh_effect_ev()
-                )
-                widget.bind(
-                    on_enter=lambda *args: self._refresh_effect_ev.cancel()
-                )
-
-            else:
-                widget.bind(size=self._trigger_update_effect)
-                try:
-                    widget.bind(pos=self._trigger_update_effect)
-                except Exception:
-                    pass
-
-    def _unbind_children_properties(self, children_list):
-        properties_to_unbind = (
-            "pos",
-            "size",
-            "scroll_x",
-            "scroll_y",
-            "on_open",
-            "on_enter",
-            "texture",
-        )
-        for widget in children_list:
-            for property in properties_to_unbind:
-                try:
-                    if property == "texture":
-                        if isinstance(widget, Image):
-                            widget.unbind(
-                                texture=self._trigger_update_effect
-                            )
-                        if isinstance(widget, Video):
-                            widget.unbind(
-                                position=self._trigger_update_effect
-                            )
-                    elif hasattr(widget, property):
-                        widget.funbind(
-                            property,
-                            self._trigger_update_effect,
-                        )
-                except Exception as e:
-                    print(e)
-                    pass
-
-    def _unbind_parent_properties(self, parents_list):
-        for widget in parents_list:
-
-            if isinstance(widget, ScrollView):
-                widget.unbind(
-                    size=self._trigger_update_effect,
-                    pos=self._trigger_update_effect,
-                    scroll_x=self._trigger_update_effect,
-                    scroll_y=self._trigger_update_effect,
-                )
-            if isinstance(widget, ModalView):
-                widget.unbind(
-                    on_pre_open=self._trigger_update_effect
-                )
-            elif isinstance(widget, Screen):
-                widget.unbind(
-                    on_pre_enter=lambda *args: self._refresh_effect_ev()
-                )
-                widget.unbind(
-                    on_enter=lambda *args: self._refresh_effect_ev.cancel()
-                )
-
-            else:
-                widget.unbind(size=self._trigger_update_effect)
-                try:
-                    widget.unbind(pos=self._trigger_update_effect)
-                except Exception:
-                    pass
-
-    def _trigger_update_effect(self, widget, value=None):
-        if value is None and self.update_by_timeout:
-            self.update_effect()
-
-        if (
-            (isinstance(value, int) or isinstance(value, float))
-            and self.update_by_timeout
-            and round(value, 3) != self.last_value
-        ):
-            self.update_effect()
-            self.last_value = round(value, 3)
-
-        elif (
-            isinstance(value, list)
-            and self.update_by_timeout
-            and (
-                round(value[0], 2) != self.last_value_list[0]
-                or round(value[1], 2) != self.last_value_list[1]
-            )
-        ):
-            self.update_effect()
-            self.last_value_list = round(value[0], 2), round(value[1], 2)
-
-    @property
-    def popup_closed(self):
-        return self.popup_parent and not self.popup_parent.parent
-
-    @property
-    def not_current_screen(self):
-        if self.parent_screen is None or self.parent_screen.manager is None:
-            return False
-        return self.parent_screen.manager.current != self.parent_screen.name
-
-    @property
-    def out_of_the_window(self):
-        x, y = self.to_window(self.x, self.y)
-        right, top = self.to_window(self.right, self.top)
-        return right < 0 or top < 0 or x > Window.width or y > Window.height
-
-    @property
-    def update_by_timeout(self):
-        _now = now()
-        if _now - self.last_update_time >= 0.016666:
-            self.last_update_time = _now
-            return True
-        return False
-
-    @property
-    def background_loaded(self):
-        if not self.background:
-            return False
-        return self.background.canvas in self.h_blur.children
+"""
+============
+FrostedGlass
+============
+
+FrostedGlass is a widget with translucent frosted glass effect, that
+creates a context with the background behind it.
+
+The effect created is based on the widget/layout passed in as the background.
+You can control the blur size, saturation, luminosity, overlay color, noise
+opacity, border radius and the outline (color and width).
+"""
+
+__all__ = ("FrostedGlass",)
+
+from ._version import __version__
+
+import kivy
+kivy.require('2.2.0')
+
+import os
+from time import perf_counter as now
+
+from kivy.clock import Clock
+from kivy.core.window import Window
+from kivy.graphics import (
+    BindTexture,
+    ClearBuffers,
+    ClearColor,
+    Color,
+    Fbo,
+    Rectangle,
+    RenderContext,
+    RoundedRectangle,
+    Scale,
+    SmoothLine,
+    Translate,
+)
+from kivy.metrics import dp
+from kivy.properties import (
+    ColorProperty,
+    ListProperty,
+    NumericProperty,
+    ObjectProperty,
+)
+from kivy.uix.floatlayout import FloatLayout
+
+# Used for type checking
+from kivy.uix.image import Image
+from kivy.uix.modalview import ModalView
+from kivy.uix.screenmanager import Screen
+from kivy.uix.scrollview import ScrollView
+from kivy.uix.video import Video
+
+MEAN_RES = (Window.width + Window.height) / 2
+
+
+vertical_blur_shader = """
+#ifdef GL_ES
+    precision lowp float;
+#endif
+
+/* Outputs from the vertex shader */
+varying vec4 frag_color;
+varying vec2 tex_coord0;
+
+/* uniform texture samplers */
+uniform sampler2D texture0;
+
+uniform float mean_res;
+uniform float blur_size;
+
+vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
+{{
+    float dt = ((blur_size / 2.0) * 1.0 / mean_res);
+    vec4 sum = vec4(0.0);
+
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+3.0*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+2.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+2.0*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+1.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+1.0*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y+0.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-0.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-1.0*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-1.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-2.0*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-2.5*dt))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y-3.0*dt))*0.077;
+
+    return frag_color * vec4(sum.rgba);
+}}
+
+void main (void){
+  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
+  vec4 effect_color = effect(
+      normal_color, texture0, tex_coord0, gl_FragCoord.xy
+  );
+  gl_FragColor = effect_color;
+}
+"""
+
+
+horizontal_blur_shader = """
+#ifdef GL_ES
+    precision lowp float;
+#endif
+
+/* Outputs from the vertex shader */
+varying vec4 frag_color;
+varying vec2 tex_coord0;
+
+/* uniform texture samplers */
+uniform sampler2D texture0;
+
+uniform float mean_res;
+uniform float blur_size;
+
+vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
+{{
+    float dt = (blur_size / 2.0) * 1.0 / mean_res;
+    vec4 sum = vec4(0.0);
+
+    sum += texture2D(texture, vec2(tex_coords.x+3.0*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x+2.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x+2.0*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x+1.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x+1.0*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x+0.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-0.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-1.0*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-1.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-2.0*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-2.5*dt, tex_coords.y))*0.077;
+    sum += texture2D(texture, vec2(tex_coords.x-3.0*dt, tex_coords.y))*0.077;
+
+    return  frag_color * vec4(sum.rgba);
+}}
+
+void main (void){
+  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
+  vec4 effect_color = effect(
+      normal_color, texture0, tex_coord0, gl_FragCoord.xy
+  );
+  gl_FragColor = effect_color;
+}
+"""
+
+
+noise_shader = """
+#ifdef GL_ES
+    precision highp float;
+#endif
+
+/* Outputs from the vertex shader */
+varying vec4 frag_color;
+varying vec2 tex_coord0;
+
+/* uniform texture samplers */
+uniform sampler2D texture0;
+
+
+vec4 effect(vec4 color, sampler2D texture, vec2 tex_coords, vec2 coords)
+{{
+    vec4 sum = vec4(0.0);
+    float a = 12.9898;
+    float b = 78.233;
+    float c = 43758.5453;
+    float dt2 = dot(tex_coords.xy, vec2(a, b));
+    float sn= mod(dt2, 3.14);
+    vec4 noise = vec4(fract(sin(sn) * c));
+
+    vec4 bg = texture2D(texture0, tex_coord0);
+    sum = mix(bg, vec4(noise.xyz, 1.0), 1.0);
+
+    return vec4(sum.rgba);
+}}
+
+void main (void){
+  vec4 normal_color = frag_color * texture2D(texture0, tex_coord0);
+  vec4 effect_color = effect(
+      normal_color, texture0, tex_coord0, gl_FragCoord.xy
+  );
+  gl_FragColor = effect_color;
+}
+"""
+
+
+final_shader_effect = """
+#ifdef GL_ES
+    precision highp float;
+#endif
+
+$HEADER$
+
+uniform int add_child_texture;
+uniform float opacity;
+uniform float luminosity;
+uniform float saturation;
+uniform float noise_opacity;
+uniform vec2 position;
+uniform vec2 resolution;
+uniform vec4 color_overlay;
+uniform sampler2D texture1;
+uniform sampler2D texture2;
+
+void main(void)
+{
+    vec2 pos = (gl_FragCoord.xy - position.xy) / resolution.xy;
+    float noise = 0.0;
+    vec4 textureResult = vec4(0.0);
+    vec4 effect_texture = texture2D(texture1, pos);
+    vec4 noise_texture = texture2D(texture2, tex_coord0);
+
+    const vec3 W = vec3(0.2125, 0.7154, 0.0721);
+    vec3 intensity = vec3(dot(effect_texture.rgb, W));
+    effect_texture = vec4(mix(intensity, effect_texture.rgb, saturation), 1.0);
+    effect_texture *= luminosity;
+
+    effect_texture = mix(
+        effect_texture.rgba,
+        vec4(color_overlay.rgb, 1.0),
+        min(1.0, color_overlay.a)
+    );
+    effect_texture = mix(
+        effect_texture.rgba,
+        vec4(noise_texture.rgb, 1.0),
+        min(1.0, noise_opacity)
+    );
+
+    gl_FragColor = vec4(effect_texture.rgb, opacity);
+}
+"""
+
+
+class VerticalBlur(Fbo):
+    def __init__(self, *args, **kwargs):
+        super(VerticalBlur, self).__init__(
+            *args, fs=vertical_blur_shader, **kwargs
+        )
+        self["mean_res"] = MEAN_RES
+        self["blur_size"] = dp(25)
+
+
+class HorizontalBlur(Fbo):
+    def __init__(self, *args, **kwargs):
+        super(HorizontalBlur, self).__init__(
+            *args, fs=horizontal_blur_shader, **kwargs
+        )
+        self.rect = Rectangle()
+        self["mean_res"] = MEAN_RES
+        self["blur_size"] = dp(25)
+
+
+class Noise(Fbo):
+    def __init__(self, *args, **kwargs):
+        super(Noise, self).__init__(*args, fs=noise_shader, **kwargs)
+        self.rect = Rectangle()
+
+
+class FrostedGlass(FloatLayout):
+
+    background = ObjectProperty(None, allownone=True)
+
+    """Target widget/layout that will be used as a background to FrostedGlass.
+    The recomended way to pass the widget is through the id.
+
+    :attr:`background` is a :class:`~kivy.properties.ObjectProperty` and
+    defaults to None."""
+
+    blur_size = NumericProperty(25)
+    """Size of the gaussian blur aplied to the background.
+
+    Note: Do not pass relative values such as dp or sp. FrostedGlass already
+    manages this automatically, according to the device's screen density.
+
+    :attr:`blur_size` is a :class:`~kivy.properties.NumericProperty` and
+    defaults to 25."""
+
+    noise_opacity = NumericProperty(0.1)
+    """Opacity of the noise layer.
+
+    :attr:`noise_opacity` is a :class:`~kivy.properties.NumericProperty` and
+    defaults to 0.1."""
+
+    saturation = NumericProperty(1.2)
+    """Saturation boost that will be aplied to the background.
+
+    :attr:`saturation` is a :class:`~kivy.properties.NumericProperty` and
+    defaults to 1.2."""
+
+    luminosity = NumericProperty(1.3)
+    """Luminosity boost that will be aplied to the background.
+
+    :attr:`luminosity` is a :class:`~kivy.properties.NumericProperty` and
+    defaults to 1.3."""
+
+    overlay_color = ColorProperty([0.5, 0.5, 0.5, 0.5])
+    """Color/tint overlay that will be aplied over the background.
+
+    :attr:`overlay_color` is a :class:`~kivy.properties.ColorProperty` and
+    defaults to [0.5, 0.5, 0.5, 0.35]."""
+
+    border_radius = ListProperty([0, 0, 0, 0])
+    """Specifies the radius used for the rounded corners clockwise:
+    top-left, top-right, bottom-right, bottom-left.
+
+    :attr:`border_radius` is a :class:`~kivy.properties.ListProperty` and
+    defaults to [0, 0, 0, 0]."""
+
+    outline_color = ColorProperty([1.0, 1.0, 1.0, 1.0])
+    """FrostedGlass outline color.
+
+    :attr:`outline_color` is a :class:`~kivy.properties.ColorProperty` and
+    defaults to [1.0, 1.0, 1.0, 1.0]."""
+
+    outline_width = NumericProperty(1)
+    """FrostedGlass outline width.
+
+    :attr:`outline_width` is a :class:`~kivy.properties.NumericProperty` and
+    defaults to 1."""
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        fbind = self.fbind
+        fbind("outline_width", self._update_canvas)
+        fbind("outline_color", self._update_canvas)
+        fbind("border_radius", self._update_canvas)
+        fbind("noise_opacity", self.update_effect)
+        fbind("luminosity", self.update_effect)
+        fbind("saturation", self.update_effect)
+        fbind("overlay_color", self.update_effect)
+        fbind("border_radius", self.update_effect)
+
+        self.frosted_glass_effect = RenderContext(
+            use_parent_projection=True,
+            use_parent_modelview=True,
+            fs=final_shader_effect
+        )
+        with self.frosted_glass_effect:
+            self.bt_1 = BindTexture(index=1)
+            self.bt_2 = BindTexture(index=2)
+            self.fbo_rect = RoundedRectangle(
+                size=self.size,
+                pos=self.pos,
+                radius=self.border_radius,
+            )
+        self.frosted_glass_effect["texture1"] = 1
+        self.frosted_glass_effect["texture2"] = 2
+
+        self.canvas.add(self.frosted_glass_effect)
+
+        with self.canvas:
+            self._outline_color = Color(rgba=self.outline_color)
+            self.outline = SmoothLine(
+                width=1,
+                overdraw_width=2,
+                rounded_rectangle=(
+                    self.x, self.y,
+                    self.width, self.height,
+                    1, 1, 1, 1, 45,
+                ),
+            )
+
+        self.noise = Noise(size=(100, 100))
+        self.h_blur = HorizontalBlur(size=(100, 100))
+        self.v_blur = VerticalBlur(size=(100, 100))
+
+        with self.h_blur:
+            ClearColor(0, 0, 0, 0)
+            ClearBuffers()
+            self.h_blur_scale = Scale(1, 1, 1)
+            self.h_blur_translate = Translate(0, 0)
+
+        with self.v_blur:
+            ClearColor(0, 0, 0, 0)
+            ClearBuffers()
+            self.v_blur_scale = Scale(1, 1, 1)
+            self.v_blur_translate = Translate(0, 0)
+
+        self.last_value = 0
+        self.last_update_time = 0
+        self.last_value_list = [0, 0]
+        self.last_blur_size_value = None
+        self.last_fbo_pos = [None, None]
+        self._pos = [0, 0]
+        self.popup_parent = None
+        self.parent_screen = None
+        self.parents_list = []
+        self.background_children_list = []
+        self.background_parents_list = []
+        self._last_background_canvas = None
+
+        self.is_movable = False
+        self.adapted_fbo_size = False
+
+        self._update_glsl_ev = Clock.create_trigger(self._update_glsl, 0)
+        self._update_fbo_ev = Clock.create_trigger(self._update_fbo_effect, 0)
+        self._update_texture_ev = Clock.create_trigger(
+            self._set_final_texture, 0
+        )
+        self._refresh_effect_ev = Clock.create_trigger(
+            self.refresh_effect, 0.033333, True
+        )
+
+        if not os.environ.get("FG_ASK_UPDATE_CANVAS_ACTIVE"):
+            os.environ["FG_ASK_UPDATE_CANVAS_ACTIVE"] = "1"
+            Clock.schedule_interval(lambda dt: Window.canvas.ask_update(), 0)
+
+    def update_effect(self, *args):
+        self._update_glsl_ev()
+
+    def refresh_effect(self, *args):
+        self._update_fbo_ev()
+        self._update_glsl_ev()
+
+    def _update_glsl(self, *args):
+        self._pos = self.to_window(*self.pos)
+        if (
+            self.not_current_screen
+            or self.out_of_the_window
+            and self.background_loaded
+        ):
+            return
+
+        effect = self.frosted_glass_effect
+        effect["position"] = [float(v) for v in self._pos]
+        effect["resolution"] = [float(v) for v in self.size]
+        effect["luminosity"] = float(self.luminosity)
+        effect["saturation"] = float(self.saturation)
+        effect["noise_opacity"] = float(self.noise_opacity)
+        effect["color_overlay"] = [float(v) for v in self.overlay_color]
+
+        if self.is_movable:
+            if not self.adapted_fbo_size:
+                self.refresh_effect()
+                self.adapted_fbo_size = True
+
+            self.h_blur_translate.x = self.v_blur_translate.x = -self._pos[0]
+            self.h_blur_translate.y = self.v_blur_translate.y = (
+                -self._pos[1] - self.size[1]
+            )
+
+        self._update_texture_ev()
+
+    def _set_final_texture(self, pos):
+        if not self.background:
+            return
+
+        if self._last_background_canvas not in self.h_blur.children:
+            self.h_blur.add(self._last_background_canvas)
+            self.v_blur.add(self.h_blur.rect)
+
+        if self.h_blur.rect.texture != self.h_blur.texture:
+            self.h_blur.rect.texture = self.h_blur.texture
+
+        self.h_blur.rect.size = self.size
+        self.h_blur.rect.pos = self._pos
+
+        self.h_blur.draw()
+        self.h_blur.ask_update()
+        self.v_blur.draw()
+        self.v_blur.ask_update()
+
+        self.bt_1.texture = self.v_blur.texture
+
+        if self._update_texture_ev.timeout == 0:
+            self._update_texture_ev.timeout = -1
+
+    def _update_noise_texture(self):
+        fbo_size = max(1, self.width / dp(1)), max(1, self.height / dp(1))
+        self.noise.size = fbo_size
+        self.noise.rect.size = self.size
+        self.noise.add(self.noise.rect)
+        self.noise.draw()
+        self.noise.remove(self.noise.rect)
+        self.bt_2.texture = self.noise.texture
+
+    def _update_fbo_effect(self, *args):
+        if self.is_movable:
+            fbo_size = (min(self.width, 150), min(self.height, 150))
+        else:
+            fbo_size = (min(self.width, 250), min(self.height, 250))
+
+        size = max(1, self.width), max(1, self.height)
+        fbo_size = max(1, fbo_size[0]), max(1, fbo_size[1])
+
+        self.h_blur.size = fbo_size
+        self.v_blur.size = fbo_size
+
+        pos = self.to_window(*self.pos)
+        x = 1 / (size[0] / fbo_size[0])
+        y = 1 / (size[1] / fbo_size[1])
+
+        self.h_blur_scale.x = self.v_blur_scale.x = x
+        self.h_blur_scale.y = self.v_blur_scale.y = -y
+        self.h_blur_translate.x = self.v_blur_translate.x = -pos[0]
+        self.h_blur_translate.y = self.v_blur_translate.y = -pos[1] - size[1]
+
+    def on_touch_down(self, touch):
+        if self.collide_point(*touch.pos):
+            super().on_touch_down(touch)
+            return True
+        return super().on_touch_down(touch)
+
+    def on_size(self, instance, size):
+        self._update_canvas()
+        self._update_noise_texture()
+        self.refresh_effect()
+
+    def on_pos(self, *args):
+        self._update_canvas()
+        self.refresh_effect()
+
+    def _update_canvas(self, *args):
+        border_radius = list(
+            map(
+                lambda x: max(1, min(min(self.width, self.height) / 2, x)),
+                self.border_radius,
+            )
+        )
+        self.fbo_rect.size = self.size
+        self.fbo_rect.pos = self.pos
+        self.fbo_rect.radius = border_radius
+
+        self._outline_color.rgba = self.outline_color
+        self.outline.width = self.outline_width
+        self.outline.rounded_rectangle = (
+            self.x, self.y,
+            self.width, self.height,
+            *border_radius, 45,
+        )
+
+    def on_blur_size(self, instance, blur_size):
+        blur_size = int(blur_size)
+        if blur_size != self.last_blur_size_value:
+            self.v_blur["blur_size"] = dp(blur_size)
+            self.h_blur["blur_size"] = dp(blur_size)
+            self.update_effect()
+            self.last_blur_size_value = blur_size
+
+    def on_background(self, _, background):
+        if not background:
+            return
+
+        if self._last_background_canvas in self.h_blur.children:
+            self.h_blur.remove(self._last_background_canvas)
+            self.update_effect()
+            self._unbind_parent_properties(self.background_parents_list)
+            self._unbind_children_properties(self.background_children_list)
+
+        self._last_background_canvas = background.canvas
+
+        self.background_parents_list = self._get_all_parents(self.background)
+        self.background_children_list = self._get_all_children(self.background)
+        self._bind_parent_properties(self.background_parents_list)
+        self._bind_children_properties(self.background_children_list)
+
+    def on_parent(self, _, parent):
+        if not parent:
+            return
+
+        self.parents_list = self._get_all_parents(parent)
+        for p in self.parents_list:
+            if isinstance(p, ModalView):
+                self.popup_parent = p
+            if isinstance(p, Screen):
+                self.parent_screen = p
+            if isinstance(p, ScrollView):
+                self.is_movable = True
+        self._bind_parent_properties(self.parents_list)
+
+    def _get_all_parents(self, widget):
+        widgets_list = []
+        parent = widget
+        while True:
+            widgets_list.append(parent)
+            if parent.parent and parent != parent.parent:
+                parent = parent.parent
+            else:
+                break
+        return widgets_list
+
+    def _get_all_children(self, widget):
+        widgets_list = [widget]
+        children_widgets = [widget]
+        while children_widgets:
+            parent_widgets = children_widgets
+            children_widgets = []
+            for w in parent_widgets:
+                if w.children:
+                    widgets_list.extend(w.children)
+                    children_widgets.extend(w.children)
+        return widgets_list
+
+    def _bind_children_properties(self, children_list):
+        properties_to_bind = (
+            "pos",
+            "size",
+            "scroll_x",
+            "scroll_y",
+            "on_open",
+            "on_enter",
+            "texture",
+        )
+        for widget in children_list:
+            for property in properties_to_bind:
+                try:
+                    if property == "texture":
+                        if isinstance(widget, Image):
+                            widget.bind(
+                                texture=self._trigger_update_effect
+                            )
+                        if isinstance(widget, Video):
+                            widget.bind(
+                                position=self._trigger_update_effect
+                            )
+                    elif hasattr(widget, property):
+                        widget.fbind(
+                            property,
+                            self._trigger_update_effect,
+                        )
+                except Exception as e:
+                    print(e)
+                    pass
+
+    def _bind_parent_properties(self, parents_list):
+        for widget in parents_list:
+
+            if isinstance(widget, ScrollView):
+                widget.bind(
+                    size=self._trigger_update_effect,
+                    pos=self._trigger_update_effect,
+                    scroll_x=self._trigger_update_effect,
+                    scroll_y=self._trigger_update_effect,
+                )
+            if isinstance(widget, ModalView):
+                widget.bind(
+                    on_pre_open=self._trigger_update_effect
+                )
+            elif isinstance(widget, Screen):
+                widget.bind(
+                    on_pre_enter=lambda *args: self._refresh_effect_ev()
+                )
+                widget.bind(
+                    on_enter=lambda *args: self._refresh_effect_ev.cancel()
+                )
+
+            else:
+                widget.bind(size=self._trigger_update_effect)
+                try:
+                    widget.bind(pos=self._trigger_update_effect)
+                except Exception:
+                    pass
+
+    def _unbind_children_properties(self, children_list):
+        properties_to_unbind = (
+            "pos",
+            "size",
+            "scroll_x",
+            "scroll_y",
+            "on_open",
+            "on_enter",
+            "texture",
+        )
+        for widget in children_list:
+            for property in properties_to_unbind:
+                try:
+                    if property == "texture":
+                        if isinstance(widget, Image):
+                            widget.unbind(
+                                texture=self._trigger_update_effect
+                            )
+                        if isinstance(widget, Video):
+                            widget.unbind(
+                                position=self._trigger_update_effect
+                            )
+                    elif hasattr(widget, property):
+                        widget.funbind(
+                            property,
+                            self._trigger_update_effect,
+                        )
+                except Exception as e:
+                    print(e)
+                    pass
+
+    def _unbind_parent_properties(self, parents_list):
+        for widget in parents_list:
+
+            if isinstance(widget, ScrollView):
+                widget.unbind(
+                    size=self._trigger_update_effect,
+                    pos=self._trigger_update_effect,
+                    scroll_x=self._trigger_update_effect,
+                    scroll_y=self._trigger_update_effect,
+                )
+            if isinstance(widget, ModalView):
+                widget.unbind(
+                    on_pre_open=self._trigger_update_effect
+                )
+            elif isinstance(widget, Screen):
+                widget.unbind(
+                    on_pre_enter=lambda *args: self._refresh_effect_ev()
+                )
+                widget.unbind(
+                    on_enter=lambda *args: self._refresh_effect_ev.cancel()
+                )
+
+            else:
+                widget.unbind(size=self._trigger_update_effect)
+                try:
+                    widget.unbind(pos=self._trigger_update_effect)
+                except Exception:
+                    pass
+
+    def _trigger_update_effect(self, widget, value=None):
+        if (
+            isinstance(value, (int, float))
+            and self.update_by_timeout
+            and round(value, 3) != self.last_value
+        ):
+            self.update_effect()
+            self.last_value = round(value, 3)
+
+        elif (
+            isinstance(value, list)
+            and self.update_by_timeout
+            and (
+                round(value[0], 2) != self.last_value_list[0]
+                or round(value[1], 2) != self.last_value_list[1]
+            )
+        ):
+            self.update_effect()
+            self.last_value_list = round(value[0], 2), round(value[1], 2)
+
+        elif self.update_by_timeout:
+            self.update_effect()
+
+    @property
+    def popup_closed(self):
+        return self.popup_parent and not self.popup_parent.parent
+
+    @property
+    def not_current_screen(self):
+        if self.parent_screen is None or self.parent_screen.manager is None:
+            return False
+        return self.parent_screen.manager.current != self.parent_screen.name
+
+    @property
+    def out_of_the_window(self):
+        x, y = self.to_window(self.x, self.y)
+        right, top = self.to_window(self.right, self.top)
+        return right < 0 or top < 0 or x > Window.width or y > Window.height
+
+    @property
+    def update_by_timeout(self):
+        _now = now()
+        if _now - self.last_update_time >= 0.016666:
+            self.last_update_time = _now
+            return True
+        return False
+
+    @property
+    def background_loaded(self):
+        if not self.background:
+            return False
+        return self.background.canvas in self.h_blur.children
```

### Comparing `kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/PKG-INFO` & `kivy_garden.frostedglass-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kivy-garden.frostedglass
-Version: 0.4.0
+Name: kivy_garden.frostedglass
+Version: 0.5.0
 Summary: FrostedGlass is a Kivy widget with frosted glass effect.
 Home-page: https://github.com/kivy-garden/frostedglass
 Author: Kivy
 Author-email: kivy@kivy.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/kivy-garden/frostedglass/issues
 Project-URL: Source, https://github.com/kivy-garden/frostedglass
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: ci
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # FrostedGlass
 
 **FrostedGlass** is a widget with translucent frosted glass effect, that
 creates a context with the background behind it.
```

### Comparing `kivy_garden.frostedglass-0.4.0/setup.py` & `kivy_garden.frostedglass-0.5.0/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""See README.md for package documentation."""
-
-from setuptools import setup, find_namespace_packages
-
-from io import open
-from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-filename = path.join(here, 'kivy_garden', 'frostedglass', '_version.py')
-# change this                              ^^^^^^
-locals = {}
-with open(filename, "rb") as fh:
-    exec(compile(fh.read(), filename, 'exec'), globals(), locals)
-__version__ = locals['__version__']
-
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-URL = 'https://github.com/kivy-garden/frostedglass'
-
-setup(
-    name='kivy_garden.frostedglass',
-    version=__version__,
-    description='FrostedGlass is a Kivy widget with frosted glass effect.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url=URL,
-    author='Kivy',
-    author_email='kivy@kivy.org',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-    keywords='Kivy kivy-garden',
-
-    packages=find_namespace_packages(include=['kivy_garden.*']),
-    install_requires=[],
-    extras_require={
-        'dev': ['pytest>=3.6', 'pytest-cov', 'pytest-asyncio',
-                'sphinx_rtd_theme'],
-        'ci': ['coveralls', 'pycodestyle'],
-    },
-    package_data={},
-    data_files=[],
-    entry_points={},
-    project_urls={
-        'Bug Reports': URL + '/issues',
-        'Source': URL,
-    },
-)
+"""See README.md for package documentation."""
+
+from setuptools import setup, find_namespace_packages
+
+from io import open
+from os import path
+
+here = path.abspath(path.dirname(__file__))
+
+filename = path.join(here, 'kivy_garden', 'frostedglass', '_version.py')
+# change this                              ^^^^^^
+locals = {}
+with open(filename, "rb") as fh:
+    exec(compile(fh.read(), filename, 'exec'), globals(), locals)
+__version__ = locals['__version__']
+
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+URL = 'https://github.com/kivy-garden/frostedglass'
+
+setup(
+    name='kivy_garden.frostedglass',
+    version=__version__,
+    description='FrostedGlass is a Kivy widget with frosted glass effect.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url=URL,
+    author='Kivy',
+    author_email='kivy@kivy.org',
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+    ],
+    keywords='Kivy kivy-garden',
+
+    packages=find_namespace_packages(include=['kivy_garden.*']),
+    install_requires=[],
+    extras_require={
+        'dev': ['pytest>=3.6', 'pytest-cov', 'pytest-asyncio',
+                'sphinx_rtd_theme'],
+        'ci': ['coveralls', 'pycodestyle'],
+    },
+    package_data={},
+    data_files=[],
+    entry_points={},
+    project_urls={
+        'Bug Reports': URL + '/issues',
+        'Source': URL,
+    },
+)
```

