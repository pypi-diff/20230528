# Comparing `tmp/PyGObject-stubs-2.7.0.tar.gz` & `tmp/PyGObject-stubs-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGObject-stubs-2.7.0.tar", last modified: Tue May  9 17:02:27 2023, max compression
+gzip compressed data, was "PyGObject-stubs-2.8.0.tar", last modified: Sun May 28 21:40:07 2023, max compression
```

## Comparing `PyGObject-stubs-2.7.0.tar` & `PyGObject-stubs-2.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/pep517backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pep517backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pep517backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/gi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/src/gi-stubs/repository/
--rw-r--r--   0 runner    (1001) docker     (123)   155987 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Adw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/AppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47065 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Atk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Farstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GIRepository.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   129078 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GLib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GModule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    75309 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GObject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GSound.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GdkPixbuf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Geoclue.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    63495 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Ggit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   304553 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Graphene.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gspell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   165678 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gst.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GstPbutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Manette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Pango.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/PangoCairo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Rsvg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Vte.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   128468 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   112437 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)  1058819 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   681586 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89364 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource5.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40235 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    49071 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.980974 PyGObject-stubs-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 21:40:07.976974 PyGObject-stubs-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.968974 PyGObject-stubs-2.8.0/pep517backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pep517backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pep517backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:40:07.980974 PyGObject-stubs-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.968974 PyGObject-stubs-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.972974 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.972974 PyGObject-stubs-2.8.0/src/gi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.976974 PyGObject-stubs-2.8.0/src/gi-stubs/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)   284195 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Adw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/AppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47065 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Atk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Farstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GIRepository.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   129078 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GLib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GModule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    75309 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GObject.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GSound.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GdkPixbuf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Geoclue.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    63495 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Ggit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   304553 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gio.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Graphene.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gspell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   165678 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gst.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GstPbutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Manette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Pango.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/PangoCairo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Rsvg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Vte.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   128468 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   112437 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)  1058819 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)  1067152 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    89364 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource5.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    40235 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    49071 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/__init__.pyi
```

### Comparing `PyGObject-stubs-2.7.0/CHANGELOG.md` & `PyGObject-stubs-2.8.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# 2.8.0 (24 May 2023)
+
+## Improvements
+
+* generator: Check nullability for __init__
+
+## Typing
+
+* Improve type hints for
+    - Adw
+    - Gtk4
+
+## Bug Fixes
+
+* generate: Force varargs if function has closure
+* parse: Ignore documentation
+
 # 2.7.0 (28 Apr 2023)
 
 ## Improvements
 
 * Extract class' docstring
 
 ## Typing
```

### Comparing `PyGObject-stubs-2.7.0/LICENSE` & `PyGObject-stubs-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/PKG-INFO` & `PyGObject-stubs-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.7.0
+Version: 2.8.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyGObject-stubs-2.7.0/README.md` & `PyGObject-stubs-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/pep517backend/backend.py` & `PyGObject-stubs-2.8.0/pep517backend/backend.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/pyproject.toml` & `PyGObject-stubs-2.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 65.0.0"]
 build-backend = "backend"
 backend-path = ["pep517backend"]
 
 [project]
 name = "PyGObject-stubs"
-version = "2.7.0"
+version = "2.8.0"
 description = "Typing stubs for PyGObject"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "LGPL-2.1"}
 authors = [
   {email = "reiter.christoph@gmail.com"},
   {name = "Christoph Reiter"}
```

### Comparing `PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/PKG-INFO` & `PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.7.0
+Version: 2.8.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/SOURCES.txt` & `PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/AppIndicator3.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/AppIndicator3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Atk.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Atk.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Farstream.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Farstream.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GIRepository.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GIRepository.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GLib.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GLib.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GModule.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GModule.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GObject.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GObject.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GSound.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GSound.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GdkPixbuf.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GdkPixbuf.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Geoclue.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Geoclue.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Ggit.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Ggit.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gio.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gio.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Graphene.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Graphene.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gsk.py` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gsk.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gspell.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gspell.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gst.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gst.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GstPbutils.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GstPbutils.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Manette.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Manette.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Pango.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Pango.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/PangoCairo.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/PangoCairo.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Rsvg.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Rsvg.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Vte.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Vte.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk3.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk4.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk4.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk3.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource4.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource4.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource5.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource5.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup2.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup2.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup3.pyi` & `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup3.pyi`

 * *Files identical despite different names*

