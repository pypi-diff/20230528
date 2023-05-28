# Comparing `tmp/aksharify-2.3.3.tar.gz` & `tmp/aksharify-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.3.3.tar", last modified: Sun May 28 06:00:02 2023, max compression
+gzip compressed data, was "aksharify-2.3.5.tar", last modified: Sun May 28 06:31:21 2023, max compression
```

## Comparing `aksharify-2.3.3.tar` & `aksharify-2.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.631314 aksharify-2.3.3/
--rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.3/LICENSE.md
--rw-rw-rw-   0        0        0     4874 2023-05-28 06:00:02.631314 aksharify-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.3/README.md
--rw-rw-rw-   0        0        0      622 2023-05-28 05:59:24.000000 aksharify-2.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 06:00:02.631314 aksharify-2.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.585517 aksharify-2.3.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.626445 aksharify-2.3.3/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4704 2023-05-28 05:55:37.000000 aksharify-2.3.3/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.247267 aksharify-2.3.5/
+-rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.5/LICENSE.md
+-rw-rw-rw-   0        0        0     4874 2023-05-28 06:31:21.244944 aksharify-2.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.5/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-28 06:30:35.000000 aksharify-2.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 06:31:21.247267 aksharify-2.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.192387 aksharify-2.3.5/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:31:21.239539 aksharify-2.3.5/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-28 06:31:21.000000 aksharify-2.3.5/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4640 2023-05-28 06:29:31.000000 aksharify-2.3.5/src/aksharify.py
```

### Comparing `aksharify-2.3.3/LICENSE.md` & `aksharify-2.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.3/PKG-INFO` & `aksharify-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.3
+Version: 2.3.5
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.3 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.5 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.3/README.md` & `aksharify-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.3/pyproject.toml` & `aksharify-2.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.3.3"
+version = "2.3.5"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.3.3/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.3.5/src/aksharify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.3
+Version: 2.3.5
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.3 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.5 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.3/src/aksharify.py` & `aksharify-2.3.5/src/aksharify.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,20 +90,20 @@
     def html_output(self, fname):
         with open(fname + ".html", "w") as file:
             file.write(self.ascii_html)
     
     def rgb2hex(self, rgba):
         return '#{:02x}{:02x}{:02x}'.format(rgba[0], rgba[1], rgba[2])
     
-    def svgify(self):
+    def svgify(self, bg_color):
         color = self.image.getdata()
         if self.ascii_text[:2] == "0b":
             self.ascii_text = self.ascii_text[2:]
         file = f'<?xml version="1.0" standalone="no"?><svg width="{int(self.w*11.087)+41}" height="{int(self.h*20)+41}" version="1.1" xmlns="http://www.w3.org/2000/svg" style="font-family: monospace; background-color:#ffffff; font-size:20;"><desc>Aksharify Art</desc>'
-        #file += f'<rect x="20" y="20" width="{int(self.w*11.087)+21}" height="{int(self.h*20)+21}" fill="none" stroke="blue" stroke-width="2" />'
+        file += f'<rect width="100%" height="100%" fill="{bg_color}" />'
         file += f'<a href="https://primepatel.github.io/aksharify-docs/">'
         y = 30
         x = 20
         for line_no in range(self.h):
             file += f'<text x="{x}" y="{y}">'
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 file += self.tspan(self.ascii_text[pixel], self.rgb2hex(color[pixel]), x)
```

