# Comparing `tmp/image-titler-2.3.4.tar.gz` & `tmp/image-titler-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-titler-2.3.4.tar", last modified: Fri Apr  8 05:16:56 2022, max compression
+gzip compressed data, was "image-titler-2.4.0.tar", last modified: Sun May 28 16:32:05 2023, max compression
```

## Comparing `image-titler-2.3.4.tar` & `image-titler-2.4.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.855562 image-titler-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-04-08 05:16:44.000000 image-titler-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-04-08 05:16:44.000000 image-titler-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-04-08 05:16:56.855562 image-titler-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-04-08 05:16:44.000000 image-titler-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.847562 image-titler-2.3.4/image_titler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-08 05:16:56.000000 image-titler-2.3.4/image_titler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.847562 image-titler-2.3.4/imagetitler/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.843562 image-titler-2.3.4/imagetitler/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.847562 image-titler-2.3.4/imagetitler/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    70656 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/fonts/BERNHC.TTF
--rw-r--r--   0 runner    (1001) docker     (121)  1036584 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/fonts/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   247240 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/fonts/gadugi.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.847562 image-titler-2.3.4/imagetitler/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    27550 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/icons/the-renegade-coder-sample-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    55909 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/icons/virtual-flat-sample-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.855562 image-titler-2.3.4/imagetitler/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)  1835865 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/23-tech-topics-to-tackle.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   614896 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/columbus-drivers-are-among-the-worst.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   498619 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/happy-new-year.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   663186 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/hello-world-in-matlab.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   494013 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/how-to-iterate-over-multiple-lists-at-the-same-time-in-python.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   409805 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/minimalism.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   819003 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/reflecting-on-my-third-semester-of-teaching.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   550387 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/the-art-of-simplification.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   552411 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/the-guide-to-causing-mass-panic.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   520515 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/assets/images/welcome-to-the-image-titler-by-the-renegade-coder.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    10564 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-04-08 05:16:44.000000 image-titler-2.3.4/imagetitler/store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:56.855562 image-titler-2.3.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 05:16:44.000000 image-titler-2.3.4/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-08 05:16:44.000000 image-titler-2.3.4/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    16576 2022-04-08 05:16:44.000000 image-titler-2.3.4/scripts/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-08 05:16:56.855562 image-titler-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-04-08 05:16:44.000000 image-titler-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.545036 image-titler-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-28 16:31:51.000000 image-titler-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-28 16:31:51.000000 image-titler-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-28 16:32:05.545036 image-titler-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-28 16:31:51.000000 image-titler-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.533036 image-titler-2.4.0/image_titler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 16:32:05.000000 image-titler-2.4.0/image_titler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.533036 image-titler-2.4.0/imagetitler/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.533036 image-titler-2.4.0/imagetitler/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.533036 image-titler-2.4.0/imagetitler/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    70656 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/fonts/BERNHC.TTF
+-rw-r--r--   0 runner    (1001) docker     (123)  1036584 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/fonts/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   247240 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/fonts/gadugi.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.533036 image-titler-2.4.0/imagetitler/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    27550 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/icons/the-renegade-coder-sample-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55909 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/icons/virtual-flat-sample-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.541036 image-titler-2.4.0/imagetitler/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1835865 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/23-tech-topics-to-tackle.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   353637 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/baklava-in-every-language.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   614896 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/columbus-drivers-are-among-the-worst.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   498619 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/happy-new-year.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   201127 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/hello-world-in-c.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   663186 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/hello-world-in-matlab.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   494013 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/how-to-iterate-over-multiple-lists-at-the-same-time-in-python.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   409805 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/minimalism.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   819003 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/reflecting-on-my-third-semester-of-teaching.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   550387 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/the-art-of-simplification.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   552411 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/the-guide-to-causing-mass-panic.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   520515 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/assets/images/welcome-to-the-image-titler-by-the-renegade-coder.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-28 16:31:51.000000 image-titler-2.4.0/imagetitler/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.545036 image-titler-2.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 16:31:52.000000 image-titler-2.4.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-28 16:31:52.000000 image-titler-2.4.0/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-28 16:31:52.000000 image-titler-2.4.0/scripts/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 16:32:05.545036 image-titler-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-28 16:31:52.000000 image-titler-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:05.545036 image-titler-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-28 16:31:52.000000 image-titler-2.4.0/tests/test_utilities.py
```

### Comparing `image-titler-2.3.4/LICENSE` & `image-titler-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/PKG-INFO` & `image-titler-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: image-titler
-Version: 2.3.4
+Version: 2.4.0
 Summary: An image processing utility which provides options for generating thumbnails for various social media platforms.
 Home-page: https://github.com/TheRenegadeCoder/image-titler
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -40,14 +38,15 @@
 image-titler --output_path "path/to/output"  # Sets the output path
 image-titler --path "path/to/image"  # Sets the image path
 image-titler --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler --batch  # Runs the program in batch mode on a directory
 image-titler --font "path/to/font"  # Changes the default title font
 image-titler --size YouTube  # Changes the aspect ratio of the output file
+image-titler --no_title  # Do not add title
 ```
 
 Alternatively, you can spin up the GUI version of the software as of 2.0.0 as follows:
 
 ```shell
 image-titler-gui
 
@@ -56,14 +55,15 @@
 image-titler-gui --output_path "path/to/output"  # Sets the output path
 image-titler-gui --path "path/to/image"  # Sets the image path
 image-titler-gui --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler-gui --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler-gui --batch  # Runs the program in batch mode on a directory
 image-titler-gui --font "path/to/font"  # Changes the default title font
 image-titler-gui --size YouTube  # Changes the aspect ratio of the output file
+image-titler-gui --no_title  # Do not add title
 ```
 
 ## Default Behavior
 
 Currently, the image-titler script makes a few assumptions about the images it 
 processes automatically: 
 
@@ -89,9 +89,8 @@
 | --font, -f | Any valid font file | Overrides the default title font |
 | --logo_path, -l | Any valid image file | Loads a logo onto the input image |
 | --output_path, -o | Any valid directory | Determines where files will be saved (has no effect in GUI) |  
 | --path, -p | Any valid file or directory | Loads the input image (or directory when in batch mode) |
 | --size, -s | Choose between "Twitter", "WordPress", and "YouTube" | Sets the aspect ratio of the output image |
 | --tier, -r | Choose between "free" (silver) or "premium" (gold) | Adds a border color to the title |
 | --title, -t | Any string | Overrides the automatic title feature |
-
-
+| --no_title, -n | | Do not add title |
```

### Comparing `image-titler-2.3.4/README.md` & `image-titler-2.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 image-titler --output_path "path/to/output"  # Sets the output path
 image-titler --path "path/to/image"  # Sets the image path
 image-titler --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler --batch  # Runs the program in batch mode on a directory
 image-titler --font "path/to/font"  # Changes the default title font
 image-titler --size YouTube  # Changes the aspect ratio of the output file
+image-titler --no_title  # Do not add title
 ```
 
 Alternatively, you can spin up the GUI version of the software as of 2.0.0 as follows:
 
 ```shell
 image-titler-gui
 
@@ -38,14 +39,15 @@
 image-titler-gui --output_path "path/to/output"  # Sets the output path
 image-titler-gui --path "path/to/image"  # Sets the image path
 image-titler-gui --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler-gui --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler-gui --batch  # Runs the program in batch mode on a directory
 image-titler-gui --font "path/to/font"  # Changes the default title font
 image-titler-gui --size YouTube  # Changes the aspect ratio of the output file
+image-titler-gui --no_title  # Do not add title
 ```
 
 ## Default Behavior
 
 Currently, the image-titler script makes a few assumptions about the images it 
 processes automatically: 
 
@@ -71,7 +73,8 @@
 | --font, -f | Any valid font file | Overrides the default title font |
 | --logo_path, -l | Any valid image file | Loads a logo onto the input image |
 | --output_path, -o | Any valid directory | Determines where files will be saved (has no effect in GUI) |  
 | --path, -p | Any valid file or directory | Loads the input image (or directory when in batch mode) |
 | --size, -s | Choose between "Twitter", "WordPress", and "YouTube" | Sets the aspect ratio of the output image |
 | --tier, -r | Choose between "free" (silver) or "premium" (gold) | Adds a border color to the title |
 | --title, -t | Any string | Overrides the automatic title feature |
+| --no_title, -n | | Do not add title |
```

### Comparing `image-titler-2.3.4/image_titler.egg-info/PKG-INFO` & `image-titler-2.4.0/image_titler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: image-titler
-Version: 2.3.4
+Version: 2.4.0
 Summary: An image processing utility which provides options for generating thumbnails for various social media platforms.
 Home-page: https://github.com/TheRenegadeCoder/image-titler
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -40,14 +38,15 @@
 image-titler --output_path "path/to/output"  # Sets the output path
 image-titler --path "path/to/image"  # Sets the image path
 image-titler --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler --batch  # Runs the program in batch mode on a directory
 image-titler --font "path/to/font"  # Changes the default title font
 image-titler --size YouTube  # Changes the aspect ratio of the output file
+image-titler --no_title  # Do not add title
 ```
 
 Alternatively, you can spin up the GUI version of the software as of 2.0.0 as follows:
 
 ```shell
 image-titler-gui
 
@@ -56,14 +55,15 @@
 image-titler-gui --output_path "path/to/output"  # Sets the output path
 image-titler-gui --path "path/to/image"  # Sets the image path
 image-titler-gui --tier "free"  # Sets the membership tier which changes the rectangle borders
 image-titler-gui --logo_path "path/to/logo"  # Adds a 145x145 logo to the lower left corner of the image
 image-titler-gui --batch  # Runs the program in batch mode on a directory
 image-titler-gui --font "path/to/font"  # Changes the default title font
 image-titler-gui --size YouTube  # Changes the aspect ratio of the output file
+image-titler-gui --no_title  # Do not add title
 ```
 
 ## Default Behavior
 
 Currently, the image-titler script makes a few assumptions about the images it 
 processes automatically: 
 
@@ -89,9 +89,8 @@
 | --font, -f | Any valid font file | Overrides the default title font |
 | --logo_path, -l | Any valid image file | Loads a logo onto the input image |
 | --output_path, -o | Any valid directory | Determines where files will be saved (has no effect in GUI) |  
 | --path, -p | Any valid file or directory | Loads the input image (or directory when in batch mode) |
 | --size, -s | Choose between "Twitter", "WordPress", and "YouTube" | Sets the aspect ratio of the output image |
 | --tier, -r | Choose between "free" (silver) or "premium" (gold) | Adds a border color to the title |
 | --title, -t | Any string | Overrides the automatic title feature |
-
-
+| --no_title, -n | | Do not add title |
```

### Comparing `image-titler-2.3.4/image_titler.egg-info/SOURCES.txt` & `image-titler-2.4.0/image_titler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 imagetitler/store.py
 imagetitler/assets/fonts/BERNHC.TTF
 imagetitler/assets/fonts/arial.ttf
 imagetitler/assets/fonts/gadugi.ttf
 imagetitler/assets/icons/the-renegade-coder-sample-icon.png
 imagetitler/assets/icons/virtual-flat-sample-icon.png
 imagetitler/assets/images/23-tech-topics-to-tackle.jpg
+imagetitler/assets/images/baklava-in-every-language.jpg
 imagetitler/assets/images/columbus-drivers-are-among-the-worst.jpg
 imagetitler/assets/images/happy-new-year.jpg
+imagetitler/assets/images/hello-world-in-c.jpg
 imagetitler/assets/images/hello-world-in-matlab.jpg
 imagetitler/assets/images/how-to-iterate-over-multiple-lists-at-the-same-time-in-python.jpg
 imagetitler/assets/images/minimalism.jpg
 imagetitler/assets/images/reflecting-on-my-third-semester-of-teaching.jpg
 imagetitler/assets/images/the-art-of-simplification.jpg
 imagetitler/assets/images/the-guide-to-causing-mass-panic.jpg
 imagetitler/assets/images/welcome-to-the-image-titler-by-the-renegade-coder.jpg
 scripts/__init__.py
 scripts/cli.py
-scripts/gui.py
+scripts/gui.py
+tests/test_utilities.py
```

### Comparing `image-titler-2.3.4/imagetitler/assets/fonts/BERNHC.TTF` & `image-titler-2.4.0/imagetitler/assets/fonts/BERNHC.TTF`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/fonts/arial.ttf` & `image-titler-2.4.0/imagetitler/assets/fonts/arial.ttf`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/fonts/gadugi.ttf` & `image-titler-2.4.0/imagetitler/assets/fonts/gadugi.ttf`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/icons/the-renegade-coder-sample-icon.png` & `image-titler-2.4.0/imagetitler/assets/icons/the-renegade-coder-sample-icon.png`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/icons/virtual-flat-sample-icon.png` & `image-titler-2.4.0/imagetitler/assets/icons/virtual-flat-sample-icon.png`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/23-tech-topics-to-tackle.jpg` & `image-titler-2.4.0/imagetitler/assets/images/23-tech-topics-to-tackle.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/columbus-drivers-are-among-the-worst.jpg` & `image-titler-2.4.0/imagetitler/assets/images/columbus-drivers-are-among-the-worst.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/happy-new-year.jpg` & `image-titler-2.4.0/imagetitler/assets/images/happy-new-year.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/hello-world-in-matlab.jpg` & `image-titler-2.4.0/imagetitler/assets/images/hello-world-in-matlab.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/how-to-iterate-over-multiple-lists-at-the-same-time-in-python.jpg` & `image-titler-2.4.0/imagetitler/assets/images/how-to-iterate-over-multiple-lists-at-the-same-time-in-python.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/minimalism.jpg` & `image-titler-2.4.0/imagetitler/assets/images/minimalism.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/reflecting-on-my-third-semester-of-teaching.jpg` & `image-titler-2.4.0/imagetitler/assets/images/reflecting-on-my-third-semester-of-teaching.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/the-art-of-simplification.jpg` & `image-titler-2.4.0/imagetitler/assets/images/the-art-of-simplification.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/the-guide-to-causing-mass-panic.jpg` & `image-titler-2.4.0/imagetitler/assets/images/the-guide-to-causing-mass-panic.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/assets/images/welcome-to-the-image-titler-by-the-renegade-coder.jpg` & `image-titler-2.4.0/imagetitler/assets/images/welcome-to-the-image-titler-by-the-renegade-coder.jpg`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/imagetitler/constants.py` & `image-titler-2.4.0/imagetitler/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 KEY_BATCH = "batch"
 KEY_FONT = "font"
 KEY_LOGO_PATH = "logo_path"
 KEY_PATH = "path"
 KEY_TIER = "tier"
 KEY_TITLE = "title"
+KEY_NO_TITLE = "no_title"
 KEY_OUTPUT_PATH = "output_path"
 KEY_SIZE = "size"
 
 FILE_TYPES = [('image files', ('.png', '.jpg', '.jpeg'))]
 
 SEPARATOR = "-"
```

### Comparing `image-titler-2.3.4/imagetitler/draw.py` & `image-titler-2.4.0/imagetitler/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     is_batch: bool = kwargs.get(KEY_BATCH)
     images = list()
     if is_batch:
         kwargs[KEY_PATH] = kwargs.get(KEY_PATH) if kwargs.get(KEY_PATH) else TRC_IMAGES
         images = _process_batch(**kwargs)
     else:
         kwargs[KEY_PATH] = kwargs.get(KEY_PATH) if kwargs.get(KEY_PATH) else TRC_IMAGE
-        kwargs[KEY_TITLE] = kwargs.get(KEY_TITLE) if kwargs.get(KEY_TITLE) else _convert_file_name_to_title(**kwargs)
+        if kwargs.get(KEY_NO_TITLE):
+            kwargs[KEY_TITLE] = ""
+        else:
+            kwargs[KEY_TITLE] = kwargs.get(KEY_TITLE) if kwargs.get(KEY_TITLE) else _convert_file_name_to_title(**kwargs)
         images.append(_process_image(**kwargs))
     return images
 
 
 def _process_batch(**kwargs) -> List[Image.Image]:
     """
     Processes a batch of images.
@@ -49,15 +52,19 @@
     """
     edited_images = list()
     input_path = kwargs.get(KEY_PATH)
     for path in os.listdir(input_path):
         absolute_path = os.path.join(input_path, path)
         image_kwargs = kwargs.copy()
         image_kwargs[KEY_PATH] = absolute_path
-        image_kwargs[KEY_TITLE] = kwargs.get(KEY_TITLE) if kwargs.get(KEY_TITLE) else _convert_file_name_to_title(**image_kwargs)
+        if kwargs.get(KEY_NO_TITLE):
+            image_kwargs[KEY_TITLE] = ""
+        else:
+            image_kwargs[KEY_TITLE] = kwargs.get(KEY_TITLE) if kwargs.get(KEY_TITLE) else _convert_file_name_to_title(**image_kwargs)
+
         edited_image = _process_image(**image_kwargs)
         edited_images.append(edited_image)
     return edited_images
 
 
 def _process_image(**kwargs) -> Image.Image:
     """
@@ -239,17 +246,17 @@
     """
     Draws text over an image.
 
     :param image: an image
     :return: the updated image
     """
     draw = ImageDraw.Draw(image)
-    font = _get_appropriate_font_size(**kwargs)
 
     if title := kwargs.get(KEY_TITLE):
+        font = _get_appropriate_font_size(**kwargs)
         title = title.strip()
         # Detect space (precondition for split)
         if len(title.split()) > 1:
             top_half_text, bottom_half_text = _split_string_by_nearest_middle_space(title)
         else:
             top_half_text, bottom_half_text = title, None
```

### Comparing `image-titler-2.3.4/imagetitler/parse.py` & `image-titler-2.4.0/imagetitler/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
     :return: None
     """
     parser.add_argument(
         '-t',
         f'--{KEY_TITLE}',
         help="add a custom title to the image"
     )
+    parser.add_argument(
+        '-n',
+        f'--{KEY_NO_TITLE}',
+        action="store_true",
+        help="do not add a custom title to the image"
+    )
 
 
 def _add_path_option(parser: argparse.ArgumentParser) -> None:
     """
     A helper function which sets up the path settings for the parser.
     The path setting determines which file or folder is to be processed.
```

### Comparing `image-titler-2.3.4/imagetitler/store.py` & `image-titler-2.4.0/imagetitler/store.py`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/scripts/cli.py` & `image-titler-2.4.0/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/scripts/gui.py` & `image-titler-2.4.0/scripts/gui.py`

 * *Files identical despite different names*

### Comparing `image-titler-2.3.4/setup.py` & `image-titler-2.4.0/setup.py`

 * *Files identical despite different names*

