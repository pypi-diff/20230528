# Comparing `tmp/pygame_imslider-1.0.1.tar.gz` & `tmp/pygame-imslider-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_imslider-1.0.1.tar", last modified: Thu Mar  2 12:00:44 2023, max compression
+gzip compressed data, was "pygame-imslider-1.0.2.tar", last modified: Sun May 28 12:23:11 2023, max compression
```

## Comparing `pygame_imslider-1.0.1.tar` & `pygame-imslider-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:44.379702 pygame_imslider-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-03-02 12:00:44.379702 pygame_imslider-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7233 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:44.375702 pygame_imslider-1.0.1/pygame_imslider/
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4245 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/dot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:44.375702 pygame_imslider-1.0.1/pygame_imslider/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/default.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      245 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/fade.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:44.379702 pygame_imslider-1.0.1/pygame_imslider/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character0.png
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character1.png
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character2.png
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character3.png
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character4.png
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character5.png
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character6.png
--rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character7.png
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character8.png
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/images/character9.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/multiple.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      243 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/one_per_move.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/examples/small_loop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12021 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/layouts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4749 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/left.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9516 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/renderers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4763 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    16662 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/slider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13821 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/pygame_imslider/sprites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:00:44.375702 pygame_imslider-1.0.1/pygame_imslider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-02 12:00:44.000000 pygame_imslider-1.0.1/pygame_imslider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 12:00:44.379702 pygame_imslider-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2094 2023-03-02 12:00:29.000000 pygame_imslider-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:23:11.083945 pygame-imslider-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-28 12:23:11.083945 pygame-imslider-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7223 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:23:11.079945 pygame-imslider-1.0.2/pygame_imslider/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4245 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/dot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:23:11.083945 pygame-imslider-1.0.2/pygame_imslider/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      245 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/fade.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:23:11.083945 pygame-imslider-1.0.2/pygame_imslider/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character7.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character8.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/images/character9.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/multiple.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      243 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/one_per_move.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/examples/small_loop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12021 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/layouts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4749 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/left.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9516 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/renderers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4763 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/right.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16724 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/slider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13821 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/pygame_imslider/sprites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:23:11.079945 pygame-imslider-1.0.2/pygame_imslider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 12:23:11.000000 pygame-imslider-1.0.2/pygame_imslider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:23:11.083945 pygame-imslider-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-05-28 12:22:55.000000 pygame-imslider-1.0.2/setup.py
```

### Comparing `pygame_imslider-1.0.1/LICENSE` & `pygame-imslider-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/PKG-INFO` & `pygame-imslider-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pygame_imslider
-Version: 1.0.1
+Name: pygame-imslider
+Version: 1.0.2
 Summary: Flexible images slider highly customizable for pygame.
 Home-page: https://github.com/anxuae/pygame-imslider
-Download-URL: https://github.com/anxuae/pygame-imslider/archive/1.0.1.tar.gz
+Download-URL: https://github.com/anxuae/pygame-imslider/archive/1.0.2.tar.gz
 Author: Antoine Rousseaux
 Keywords: pygame,widget
 Platform: unix
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
@@ -108,22 +108,22 @@
     # Initializes and activates ImSlider
     slider = ImSlider((300, 100), callback=consumer)
     slider.load_images(['image1.png', 'image2.png', 'image3.png',])
 
 The slider has the following optional parameters:
 
 - **stype**: determine a slider type: STYPE_SLIDE, STYPE_LOOP or STYPE_FADE
-- **per_page**: determine how many slides should be displayed per page. If
-  stype=STYPE_FADE, this option is ignored.
+- **per_page**: determine how many slides should be displayed per page. Ignored if
+  stype=STYPE_FADE.
 - **per_move**: determine how many slides should be moved when a slider goes
-  to next or perv. If stype=STYPE_FADE, this option is ignored.
+  to next or perv. Ignored if stype=STYPE_FADE.
 - **focus**: determine which slide should be focused if there are multiple
   slides in a page. A string "center" is acceptable for centering slides.
 - **rewind**: whether to rewind a slider before the first slide or after the
-  last one. If stype=STYPE_LOOP, this option is ignored.
+  last one. Ignored if stype=STYPE_LOOP.
 - **speed**: transition duration in seconds.
 - **renderer**: a ImSliderRenderer to customize colors of the slider
 - **callback**: callback called each time the selection is changed.
 
 Event management
 ----------------
 
@@ -192,19 +192,19 @@
 - ImSliderRenderer.DARK
 
 A custom ``ImSliderRenderer`` can be built using following constructor :
 
 .. code-block:: python
 
     renderer = ImSliderRenderer(
-        # RGB tuple for arrow color (one per state: released, pressed).
+        # RGB tuple for arrow color (one tuple per state: released, pressed).
         ((255, 255, 255), (54, 54, 54)),
-        # RGB tuple for page-dot color (one tuple per state).
+        # RGB tuple for page-dot color (one tuple per state: released, pressed).
         ((120, 120, 120), (54, 54, 54)),
-        # RGB tuple for sldie color.
+        # RGB tuple for slide color.
         (242, 195, 195),
         # RGB tuple for selected image color.
         (245, 95, 76),
         # RGB tuple for selected page-dot color.
         (255, 255, 255),
         # RGB tuple for background color.
         (32, 135, 156)
@@ -233,15 +233,15 @@
     # Load a sequence of image files.
     slider.load_images(['image1.png', 'image2.png', 'image3.png'])
 
     # Get a pygame.Rect object in which the slider is included.
     slider.get_rect()
 
     # Get the current pygame image (optionally resized).
-    slider.get_image()
+    slider.get_image(resized=False)
 
     # Get the current index.
     slider.get_index()
 
     # Set the current index.
     slider.set_index(2)
```

### Comparing `pygame_imslider-1.0.1/README.rst` & `pygame-imslider-1.0.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -83,22 +83,22 @@
     # Initializes and activates ImSlider
     slider = ImSlider((300, 100), callback=consumer)
     slider.load_images(['image1.png', 'image2.png', 'image3.png',])
 
 The slider has the following optional parameters:
 
 - **stype**: determine a slider type: STYPE_SLIDE, STYPE_LOOP or STYPE_FADE
-- **per_page**: determine how many slides should be displayed per page. If
-  stype=STYPE_FADE, this option is ignored.
+- **per_page**: determine how many slides should be displayed per page. Ignored if
+  stype=STYPE_FADE.
 - **per_move**: determine how many slides should be moved when a slider goes
-  to next or perv. If stype=STYPE_FADE, this option is ignored.
+  to next or perv. Ignored if stype=STYPE_FADE.
 - **focus**: determine which slide should be focused if there are multiple
   slides in a page. A string "center" is acceptable for centering slides.
 - **rewind**: whether to rewind a slider before the first slide or after the
-  last one. If stype=STYPE_LOOP, this option is ignored.
+  last one. Ignored if stype=STYPE_LOOP.
 - **speed**: transition duration in seconds.
 - **renderer**: a ImSliderRenderer to customize colors of the slider
 - **callback**: callback called each time the selection is changed.
 
 Event management
 ----------------
 
@@ -167,19 +167,19 @@
 - ImSliderRenderer.DARK
 
 A custom ``ImSliderRenderer`` can be built using following constructor :
 
 .. code-block:: python
 
     renderer = ImSliderRenderer(
-        # RGB tuple for arrow color (one per state: released, pressed).
+        # RGB tuple for arrow color (one tuple per state: released, pressed).
         ((255, 255, 255), (54, 54, 54)),
-        # RGB tuple for page-dot color (one tuple per state).
+        # RGB tuple for page-dot color (one tuple per state: released, pressed).
         ((120, 120, 120), (54, 54, 54)),
-        # RGB tuple for sldie color.
+        # RGB tuple for slide color.
         (242, 195, 195),
         # RGB tuple for selected image color.
         (245, 95, 76),
         # RGB tuple for selected page-dot color.
         (255, 255, 255),
         # RGB tuple for background color.
         (32, 135, 156)
@@ -208,15 +208,15 @@
     # Load a sequence of image files.
     slider.load_images(['image1.png', 'image2.png', 'image3.png'])
 
     # Get a pygame.Rect object in which the slider is included.
     slider.get_rect()
 
     # Get the current pygame image (optionally resized).
-    slider.get_image()
+    slider.get_image(resized=False)
 
     # Get the current index.
     slider.get_index()
 
     # Set the current index.
     slider.set_index(2)
```

### Comparing `pygame_imslider-1.0.1/pygame_imslider/animations.py` & `pygame-imslider-1.0.2/pygame_imslider/animations.py`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/dot.png` & `pygame-imslider-1.0.2/pygame_imslider/dot.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/default.py` & `pygame-imslider-1.0.2/pygame_imslider/examples/default.py`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character0.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character0.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character1.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character1.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character2.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character2.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character3.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character3.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character4.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character4.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character5.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character5.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character6.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character6.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character7.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character7.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character8.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character8.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/examples/images/character9.png` & `pygame-imslider-1.0.2/pygame_imslider/examples/images/character9.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/layouts.py` & `pygame-imslider-1.0.2/pygame_imslider/layouts.py`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/left.png` & `pygame-imslider-1.0.2/pygame_imslider/left.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/renderers.py` & `pygame-imslider-1.0.2/pygame_imslider/renderers.py`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/right.png` & `pygame-imslider-1.0.2/pygame_imslider/right.png`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider/slider.py` & `pygame-imslider-1.0.2/pygame_imslider/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
     """Flexible images slider for Pygame engine.
 
     :param size: size of the image slider
     :type size: tuple
     :param stype: determine a slider type
     :type stype: str
-    :param per_page: determine how many slides should be displayed per page. If
-                     stype=STYPE_FADE, this option is ignored.
+    :param per_page: determine how many slides should be displayed per page.
+                     Ignored if stype=STYPE_FADE.
     :type per_page: int
     :param per_move: determine how many slides should be moved when a slider goes
-                     to next or perv. If stype=STYPE_FADE, this option is ignored.
+                     to next or perv. Ignored if stype=STYPE_FADE.
     :type per_move: int
     :param focus: determine which slide should be focused if there are multiple
                   slides in a page. A string "center" is acceptable for centering slides.
     :type focus: bool or str
     :param rewind: whether to rewind a slider before the first slide or after the
-                   last one. If stype=STYPE_LOOP, this option is ignored.
+                   last one. Ignored if stype=STYPE_LOOP.
     :type rewind: bool
     :param speed: transition duration in seconds.
     :type speed: int
     :param renderer: renderer to customize colors of the slider.
     :type renderer: :py:class:`ImSliderRenderer`
     :param callback: callback called each time the selection is changed.
     :type callback: function
@@ -80,19 +80,19 @@
         self.sprites = pygame.sprite.LayeredDirty()
         self.sprites.add(self.background, layer=0)
         for arrow in self.arrows:
             self.sprites.add(arrow, layer=1)
 
         self.set_size(*size)
 
-        # On Raspberry Pi, the time to update dirty sprites is long (120-180ms
+        # On Raspberry Pi, the time to update dirty sprites is long (200-300ms
         # tested), increasing the treshold permits to avoid blitting full screen
         # at each draw() call.
-        self.sprites.set_timing_threshold(200)
-        self.layout.set_timing_threshold(200)
+        self.sprites.set_timing_threshold(600)
+        self.layout.set_timing_threshold(600)
 
     @property
     def per_page(self):
         return self._per_page if self.stype != STYPE_FADE else 1
 
     @property
     def per_move(self):
@@ -279,14 +279,16 @@
 
         :param events: list of events to process.
         :type events: list
         """
         dt = self.clock.tick() / 1000  # Amount of seconds between each loop.
         update_eraser = self.background.image is None
         self.sprites.update(events, dt)
+        # Synchronize update method between groups
+        self.layout._use_update = self.sprites._use_update
 
         if self.layout.is_animated():
             self.layout.update(events, dt)
             return  # Let's finish the current animations
 
         if self.arrows[0].pressed_time > self.pressed_repeat_time:
             self.arrows[0].pressed_time = 0
```

### Comparing `pygame_imslider-1.0.1/pygame_imslider/sprites.py` & `pygame-imslider-1.0.2/pygame_imslider/sprites.py`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/pygame_imslider.egg-info/PKG-INFO` & `pygame-imslider-1.0.2/pygame_imslider.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pygame-imslider
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flexible images slider highly customizable for pygame.
 Home-page: https://github.com/anxuae/pygame-imslider
-Download-URL: https://github.com/anxuae/pygame-imslider/archive/1.0.1.tar.gz
+Download-URL: https://github.com/anxuae/pygame-imslider/archive/1.0.2.tar.gz
 Author: Antoine Rousseaux
 Keywords: pygame,widget
 Platform: unix
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
@@ -108,22 +108,22 @@
     # Initializes and activates ImSlider
     slider = ImSlider((300, 100), callback=consumer)
     slider.load_images(['image1.png', 'image2.png', 'image3.png',])
 
 The slider has the following optional parameters:
 
 - **stype**: determine a slider type: STYPE_SLIDE, STYPE_LOOP or STYPE_FADE
-- **per_page**: determine how many slides should be displayed per page. If
-  stype=STYPE_FADE, this option is ignored.
+- **per_page**: determine how many slides should be displayed per page. Ignored if
+  stype=STYPE_FADE.
 - **per_move**: determine how many slides should be moved when a slider goes
-  to next or perv. If stype=STYPE_FADE, this option is ignored.
+  to next or perv. Ignored if stype=STYPE_FADE.
 - **focus**: determine which slide should be focused if there are multiple
   slides in a page. A string "center" is acceptable for centering slides.
 - **rewind**: whether to rewind a slider before the first slide or after the
-  last one. If stype=STYPE_LOOP, this option is ignored.
+  last one. Ignored if stype=STYPE_LOOP.
 - **speed**: transition duration in seconds.
 - **renderer**: a ImSliderRenderer to customize colors of the slider
 - **callback**: callback called each time the selection is changed.
 
 Event management
 ----------------
 
@@ -192,19 +192,19 @@
 - ImSliderRenderer.DARK
 
 A custom ``ImSliderRenderer`` can be built using following constructor :
 
 .. code-block:: python
 
     renderer = ImSliderRenderer(
-        # RGB tuple for arrow color (one per state: released, pressed).
+        # RGB tuple for arrow color (one tuple per state: released, pressed).
         ((255, 255, 255), (54, 54, 54)),
-        # RGB tuple for page-dot color (one tuple per state).
+        # RGB tuple for page-dot color (one tuple per state: released, pressed).
         ((120, 120, 120), (54, 54, 54)),
-        # RGB tuple for sldie color.
+        # RGB tuple for slide color.
         (242, 195, 195),
         # RGB tuple for selected image color.
         (245, 95, 76),
         # RGB tuple for selected page-dot color.
         (255, 255, 255),
         # RGB tuple for background color.
         (32, 135, 156)
@@ -233,15 +233,15 @@
     # Load a sequence of image files.
     slider.load_images(['image1.png', 'image2.png', 'image3.png'])
 
     # Get a pygame.Rect object in which the slider is included.
     slider.get_rect()
 
     # Get the current pygame image (optionally resized).
-    slider.get_image()
+    slider.get_image(resized=False)
 
     # Get the current index.
     slider.get_index()
 
     # Set the current index.
     slider.set_index(2)
```

### Comparing `pygame_imslider-1.0.1/pygame_imslider.egg-info/SOURCES.txt` & `pygame-imslider-1.0.2/pygame_imslider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygame_imslider-1.0.1/setup.py` & `pygame-imslider-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HERE = osp.abspath(osp.dirname(__file__))
 sys.path.insert(0, HERE)
 import pygame_imslider  # nopep8 : import shall be done after adding setup to paths
 
 
 def main():
     setup(
-        name=pygame_imslider.__name__,
+        name='pygame-imslider',
         version=pygame_imslider.__version__,
         description=pygame_imslider.__doc__,
         long_description=open(osp.join(HERE, 'README.rst'), encoding='utf-8').read(),
         long_description_content_type='text/x-rst',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Other Environment',
```

