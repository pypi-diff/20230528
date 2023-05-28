# Comparing `tmp/aksharify-2.3.2.tar.gz` & `tmp/aksharify-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.3.2.tar", last modified: Sun May 28 05:44:09 2023, max compression
+gzip compressed data, was "aksharify-2.3.3.tar", last modified: Sun May 28 06:00:02 2023, max compression
```

## Comparing `aksharify-2.3.2.tar` & `aksharify-2.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.853717 aksharify-2.3.2/
--rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.2/LICENSE.md
--rw-rw-rw-   0        0        0     4874 2023-05-28 05:44:09.849695 aksharify-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.2/README.md
--rw-rw-rw-   0        0        0      622 2023-05-28 05:42:56.000000 aksharify-2.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 05:44:09.855740 aksharify-2.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.785028 aksharify-2.3.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.847176 aksharify-2.3.2/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4705 2023-05-28 05:34:29.000000 aksharify-2.3.2/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.631314 aksharify-2.3.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.3/LICENSE.md
+-rw-rw-rw-   0        0        0     4874 2023-05-28 06:00:02.631314 aksharify-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.3/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-28 05:59:24.000000 aksharify-2.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 06:00:02.631314 aksharify-2.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.585517 aksharify-2.3.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:00:02.626445 aksharify-2.3.3/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-28 06:00:02.000000 aksharify-2.3.3/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4704 2023-05-28 05:55:37.000000 aksharify-2.3.3/src/aksharify.py
```

### Comparing `aksharify-2.3.2/LICENSE.md` & `aksharify-2.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.2/PKG-INFO` & `aksharify-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.2
+Version: 2.3.3
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.2/README.md` & `aksharify-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.3.2/pyproject.toml` & `aksharify-2.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.3.2"
+version = "2.3.3"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.3.2/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.3.3/src/aksharify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.3.2
+Version: 2.3.3
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
-Metadata-Version: 2.1 Name: aksharify Version: 2.3.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
```

### Comparing `aksharify-2.3.2/src/aksharify.py` & `aksharify-2.3.3/src/aksharify.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,14 @@
             file += f'<text x="{x}" y="{y}">'
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 file += self.tspan(self.ascii_text[pixel], self.rgb2hex(color[pixel]), x)
                 x += 11.1
             file += '</text>'
             x = 20
             y += 20
-        #file += "</a>"
+        file += "</a>"
         file += "</svg>"
         self.ascii_svg = file
         
     def svg_output(self, fname):
         with open(fname + ".svg", "w") as file:
             file.write(self.ascii_svg)
```

