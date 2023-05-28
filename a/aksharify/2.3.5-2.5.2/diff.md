# Comparing `tmp/aksharify-2.3.5.tar.gz` & `tmp/aksharify-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.3.5.tar", last modified: Sun May 28 06:31:21 2023, max compression
+gzip compressed data, was "aksharify-2.5.2.tar", last modified: Sun May 28 07:02:54 2023, max compression
```

## Comparing `aksharify-2.3.5.tar` & `aksharify-2.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.247267 aksharify-2.3.5/
--rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.5/LICENSE.md
--rw-rw-rw-   0        0        0     4874 2023-05-28 06:31:21.244944 aksharify-2.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.5/README.md
--rw-rw-rw-   0        0        0      622 2023-05-28 06:30:35.000000 aksharify-2.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 06:31:21.247267 aksharify-2.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.192387 aksharify-2.3.5/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.239539 aksharify-2.3.5/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4640 2023-05-28 06:29:31.000000 aksharify-2.3.5/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.312840 aksharify-2.5.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.5.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4874 2023-05-28 07:02:54.311835 aksharify-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.5.2/README.md
+-rw-rw-rw-   0        0        0      634 2023-05-28 07:01:04.000000 aksharify-2.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 07:02:54.313836 aksharify-2.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.258851 aksharify-2.5.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.5.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.309760 aksharify-2.5.2/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5541 2023-05-28 06:59:02.000000 aksharify-2.5.2/src/aksharify.py
```

### Comparing `aksharify-2.3.5/LICENSE.md` & `aksharify-2.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.5/PKG-INFO` & `aksharify-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.5
+Version: 2.5.2
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.5 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.5.2 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.5/README.md` & `aksharify-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.5/pyproject.toml` & `aksharify-2.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.3.5"
+version = "2.5.2"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
 
-dependencies = ["Pillow"]
+dependencies = ["Pillow", "cairosvg"]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
```

### Comparing `aksharify-2.3.5/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.5.2/src/aksharify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.5
+Version: 2.5.2
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.5 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.5.2 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.5/src/aksharify.py` & `aksharify-2.5.2/src/aksharify.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from PIL import Image
+from cairosvg import svg2png
 
 
 class TextArt:
     def __init__(self, image) -> None:
         self.image = Image.open(image)
         self.w, self.h = self.image.size
         self.ascii_chars = list('01')
@@ -114,7 +115,34 @@
         file += "</a>"
         file += "</svg>"
         self.ascii_svg = file
         
     def svg_output(self, fname):
         with open(fname + ".svg", "w") as file:
             file.write(self.ascii_svg)
+
+    def png_output(self, fname, height=None, width=None):
+        self.svgify()
+        if height==None and width != None:
+            svg2png(
+                bytestring=self.ascii_svg,
+                write_to= fname+'.png', 
+                output_width=width
+            )
+        elif width==None and height!=None:
+            svg2png(
+                bytestring=self.ascii_svg,
+                write_to= fname+'.png', 
+                output_height=height
+            )
+        elif height == None and width == None:
+            svg2png(
+                bytestring=self.ascii_svg,
+                write_to= fname+'.png'
+            )
+        else:
+            svg2png(
+                bytestring=self.ascii_svg,
+                write_to= fname+'.png',
+                output_height=height,
+                output_width=width
+            )
```

