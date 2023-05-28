# Comparing `tmp/aksharify-2.5.2.tar.gz` & `tmp/aksharify-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.5.2.tar", last modified: Sun May 28 07:02:54 2023, max compression
+gzip compressed data, was "aksharify-2.5.3.tar", last modified: Sun May 28 07:13:50 2023, max compression
```

## Comparing `aksharify-2.5.2.tar` & `aksharify-2.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.312840 aksharify-2.5.2/
--rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.5.2/LICENSE.md
--rw-rw-rw-   0        0        0     4874 2023-05-28 07:02:54.311835 aksharify-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.5.2/README.md
--rw-rw-rw-   0        0        0      634 2023-05-28 07:01:04.000000 aksharify-2.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 07:02:54.313836 aksharify-2.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.258851 aksharify-2.5.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.5.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 07:02:54.309760 aksharify-2.5.2/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-28 07:02:54.000000 aksharify-2.5.2/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5541 2023-05-28 06:59:02.000000 aksharify-2.5.2/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.484324 aksharify-2.5.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.5.3/LICENSE.md
+-rw-rw-rw-   0        0        0     4874 2023-05-28 07:13:50.479965 aksharify-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.5.3/README.md
+-rw-rw-rw-   0        0        0      634 2023-05-28 07:12:56.000000 aksharify-2.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 07:13:50.484324 aksharify-2.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.436069 aksharify-2.5.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.5.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.475727 aksharify-2.5.3/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5573 2023-05-28 07:12:30.000000 aksharify-2.5.3/src/aksharify.py
```

### Comparing `aksharify-2.5.2/LICENSE.md` & `aksharify-2.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.5.2/PKG-INFO` & `aksharify-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.5.2
+Version: 2.5.3
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.5.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.5.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.5.2/README.md` & `aksharify-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.5.2/pyproject.toml` & `aksharify-2.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.5.2"
+version = "2.5.3"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.5.2/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.5.3/src/aksharify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.5.2
+Version: 2.5.3
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.5.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.5.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.5.2/src/aksharify.py` & `aksharify-2.5.3/src/aksharify.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def html_output(self, fname):
         with open(fname + ".html", "w") as file:
             file.write(self.ascii_html)
     
     def rgb2hex(self, rgba):
         return '#{:02x}{:02x}{:02x}'.format(rgba[0], rgba[1], rgba[2])
     
-    def svgify(self, bg_color):
+    def svgify(self, bg_color="None"):
         color = self.image.getdata()
         if self.ascii_text[:2] == "0b":
             self.ascii_text = self.ascii_text[2:]
         file = f'<?xml version="1.0" standalone="no"?><svg width="{int(self.w*11.087)+41}" height="{int(self.h*20)+41}" version="1.1" xmlns="http://www.w3.org/2000/svg" style="font-family: monospace; background-color:#ffffff; font-size:20;"><desc>Aksharify Art</desc>'
         file += f'<rect width="100%" height="100%" fill="{bg_color}" />'
         file += f'<a href="https://primepatel.github.io/aksharify-docs/">'
         y = 30
@@ -116,16 +116,16 @@
         file += "</svg>"
         self.ascii_svg = file
         
     def svg_output(self, fname):
         with open(fname + ".svg", "w") as file:
             file.write(self.ascii_svg)
 
-    def png_output(self, fname, height=None, width=None):
-        self.svgify()
+    def png_output(self, fname, bg_color="None", height=None, width=None):
+        self.svgify(bg_color)
         if height==None and width != None:
             svg2png(
                 bytestring=self.ascii_svg,
                 write_to= fname+'.png', 
                 output_width=width
             )
         elif width==None and height!=None:
```

