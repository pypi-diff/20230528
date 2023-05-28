# Comparing `tmp/parceqt-0.8.5.tar.gz` & `tmp/parceqt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parceqt-0.8.5.tar", last modified: Sat Apr 25 08:12:34 2020, max compression
+gzip compressed data, was "dist/parceqt-0.9.0.tar", last modified: Mon May  4 16:20:02 2020, max compression
```

## Comparing `parceqt-0.8.5.tar` & `parceqt-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1594 2020-04-25 08:10:46.000000 parceqt-0.8.5/ChangeLog
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    35149 2020-01-22 13:08:40.000000 parceqt-0.8.5/LICENSE
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      105 2020-04-25 08:11:24.000000 parceqt-0.8.5/MANIFEST.in
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1637 2020-04-25 08:12:34.000000 parceqt-0.8.5/PKG-INFO
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      804 2020-02-09 15:58:23.000000 parceqt-0.8.5/README.rst
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/docs/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      784 2020-02-07 20:08:45.000000 parceqt-0.8.5/docs/Makefile
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/docs/source/
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/docs/source/_static/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      952 2020-03-28 06:52:05.000000 parceqt-0.8.5/docs/source/_static/custom.css
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       39 2020-03-20 06:37:58.000000 parceqt-0.8.5/docs/source/changelog.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6193 2020-02-11 10:26:17.000000 parceqt-0.8.5/docs/source/conf.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      123 2020-03-22 12:15:33.000000 parceqt-0.8.5/docs/source/debug.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      132 2020-02-07 20:23:55.000000 parceqt-0.8.5/docs/source/document.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      135 2020-02-11 10:22:50.000000 parceqt-0.8.5/docs/source/formatter.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      141 2020-02-07 20:23:59.000000 parceqt-0.8.5/docs/source/highlighter.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      367 2020-03-22 12:15:04.000000 parceqt-0.8.5/docs/source/index.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-03-20 06:37:58.000000 parceqt-0.8.5/docs/source/license.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      131 2020-02-07 20:23:33.000000 parceqt-0.8.5/docs/source/parceqt.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      141 2020-02-07 20:23:09.000000 parceqt-0.8.5/docs/source/treebuilder.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      135 2020-03-20 06:37:58.000000 parceqt-0.8.5/docs/source/treemodel.rst
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      120 2020-02-07 20:21:18.000000 parceqt-0.8.5/docs/source/util.rst
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/parceqt/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4592 2020-04-18 09:51:39.000000 parceqt-0.8.5/parceqt/__init__.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    25145 2020-04-18 15:34:14.000000 parceqt-0.8.5/parceqt/debug.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4487 2020-03-25 09:45:45.000000 parceqt-0.8.5/parceqt/document.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8596 2020-04-18 18:56:32.000000 parceqt-0.8.5/parceqt/formatter.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8512 2020-04-18 12:02:17.000000 parceqt-0.8.5/parceqt/highlighter.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1613 2020-04-15 21:44:08.000000 parceqt-0.8.5/parceqt/pkginfo.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4165 2020-04-09 17:41:37.000000 parceqt-0.8.5/parceqt/treebuilder.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8690 2020-04-07 12:13:25.000000 parceqt-0.8.5/parceqt/treemodel.py
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4826 2020-04-04 09:42:42.000000 parceqt-0.8.5/parceqt/util.py
-drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-04-25 08:12:34.000000 parceqt-0.8.5/parceqt.egg-info/
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1637 2020-04-25 08:12:33.000000 parceqt-0.8.5/parceqt.egg-info/PKG-INFO
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      690 2020-04-25 08:12:34.000000 parceqt-0.8.5/parceqt.egg-info/SOURCES.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        1 2020-04-25 08:12:33.000000 parceqt-0.8.5/parceqt.egg-info/dependency_links.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        8 2020-04-25 08:12:33.000000 parceqt-0.8.5/parceqt.egg-info/top_level.txt
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       38 2020-04-25 08:12:34.000000 parceqt-0.8.5/setup.cfg
--rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2176 2020-01-22 13:08:40.000000 parceqt-0.8.5/setup.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1705 2020-05-04 16:19:12.000000 parceqt-0.9.0/ChangeLog
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    35149 2020-01-22 13:08:40.000000 parceqt-0.9.0/LICENSE
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      105 2020-04-25 08:11:24.000000 parceqt-0.9.0/MANIFEST.in
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1637 2020-05-04 16:20:02.000000 parceqt-0.9.0/PKG-INFO
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      804 2020-02-09 15:58:23.000000 parceqt-0.9.0/README.rst
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/docs/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      784 2020-02-07 20:08:45.000000 parceqt-0.9.0/docs/Makefile
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/docs/source/
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/docs/source/_static/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      952 2020-03-28 06:52:05.000000 parceqt-0.9.0/docs/source/_static/custom.css
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       39 2020-03-20 06:37:58.000000 parceqt-0.9.0/docs/source/changelog.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     6193 2020-02-11 10:26:17.000000 parceqt-0.9.0/docs/source/conf.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      123 2020-03-22 12:15:33.000000 parceqt-0.9.0/docs/source/debug.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      132 2020-02-07 20:23:55.000000 parceqt-0.9.0/docs/source/document.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      135 2020-02-11 10:22:50.000000 parceqt-0.9.0/docs/source/formatter.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      141 2020-02-07 20:23:59.000000 parceqt-0.9.0/docs/source/highlighter.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      367 2020-03-22 12:15:04.000000 parceqt-0.9.0/docs/source/index.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      127 2020-03-20 06:37:58.000000 parceqt-0.9.0/docs/source/license.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      131 2020-02-07 20:23:33.000000 parceqt-0.9.0/docs/source/parceqt.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      141 2020-02-07 20:23:09.000000 parceqt-0.9.0/docs/source/treebuilder.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      135 2020-03-20 06:37:58.000000 parceqt-0.9.0/docs/source/treemodel.rst
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      120 2020-02-07 20:21:18.000000 parceqt-0.9.0/docs/source/util.rst
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4592 2020-04-18 09:51:39.000000 parceqt-0.9.0/parceqt/__init__.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)    25177 2020-04-27 15:39:32.000000 parceqt-0.9.0/parceqt/debug.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4487 2020-03-25 09:45:45.000000 parceqt-0.9.0/parceqt/document.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8596 2020-04-18 18:56:32.000000 parceqt-0.9.0/parceqt/formatter.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8512 2020-04-18 12:02:17.000000 parceqt-0.9.0/parceqt/highlighter.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1613 2020-05-04 16:19:12.000000 parceqt-0.9.0/parceqt/pkginfo.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4268 2020-05-04 06:42:33.000000 parceqt-0.9.0/parceqt/treebuilder.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     8672 2020-04-27 10:26:19.000000 parceqt-0.9.0/parceqt/treemodel.py
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     4826 2020-04-04 09:42:42.000000 parceqt-0.9.0/parceqt/util.py
+drwxrwxr-x   0 wilbert   (1000) wilbert   (1000)        0 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt.egg-info/
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     1637 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt.egg-info/PKG-INFO
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)      690 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        1 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)        8 2020-05-04 16:20:02.000000 parceqt-0.9.0/parceqt.egg-info/top_level.txt
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)       38 2020-05-04 16:20:02.000000 parceqt-0.9.0/setup.cfg
+-rw-rw-r--   0 wilbert   (1000) wilbert   (1000)     2176 2020-01-22 13:08:40.000000 parceqt-0.9.0/setup.py
```

### Comparing `parceqt-0.8.5/ChangeLog` & `parceqt-0.9.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ChangeLog
 =========
 
 
+2020-05-04: parceqt-0.9.0
+
+- some small api adjustments to parce-0.9.0
+- set window title of debugger window
+
+
 2020-04-25: parceqt-0.8.5
 
 - add "Debug Unparsed Text" theme, highlighting unparsed text
 - adjust treebuilder and highlighter to the new peek() call of parce.treebuilder
 - debug window:
   - when opening a file, automatically guess the language to use
   - new commands to show/hide the tree and to reload the theme stylesheet
```

### Comparing `parceqt-0.8.5/LICENSE` & `parceqt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/PKG-INFO` & `parceqt-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: parceqt
-Version: 0.8.5
+Version: 0.9.0
 Summary: The parceqt Python module
 Home-page: https://github.com/wbsoft/parceqt
 Maintainer: Wilbert Berendsen
 Maintainer-email: info@wilbertberendsen.nl
 License: GPL
 Description: parceqt
         =======
```

### Comparing `parceqt-0.8.5/README.rst` & `parceqt-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/docs/Makefile` & `parceqt-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/docs/source/_static/custom.css` & `parceqt-0.9.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/docs/source/conf.py` & `parceqt-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt/__init__.py` & `parceqt-0.9.0/parceqt/__init__.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt/debug.py` & `parceqt-0.9.0/parceqt/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     and the displayed ancestor path.
 
     """
 
     show_updated_region_enabled = False
 
     def __init__(self, parent=None):
-        super().__init__(parent)
+        super().__init__(parent, windowTitle="parceqt debugger")
 
         f = self._updated_format = QTextCharFormat()
         c = QColor("palegreen")
         c.setAlpha(64)
         f.setBackground(c)
         f = self._currentline_format = QTextCharFormat()
         f.setProperty(QTextCharFormat.FullWidthSelection, True)
```

### Comparing `parceqt-0.8.5/parceqt/document.py` & `parceqt-0.9.0/parceqt/document.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt/formatter.py` & `parceqt-0.9.0/parceqt/formatter.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt/highlighter.py` & `parceqt-0.9.0/parceqt/highlighter.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt/pkginfo.py` & `parceqt-0.9.0/parceqt/pkginfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 
 #: name of the package
 name = "parceqt"
 
 #: the current version
-version = Version(0, 8, 5)
+version = Version(0, 9, 0)
 version_suffix = ""
 version_string = "{}.{}.{}".format(*version) + version_suffix
 
 #: short description
 description = "The parceqt Python module"
 
 #: long description
```

### Comparing `parceqt-0.8.5/parceqt/treebuilder.py` & `parceqt-0.9.0/parceqt/treebuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,34 @@
         """Run the background (build) part of the process."""
         for stage in self._process:
             break
 
     def process_started(self):
         """Reimplemented to emit the ``started`` signal."""
         self.started.emit()
+        super().process_started()
 
     def process_finished(self):
         """Reimplemented to emit the ``updated`` signal."""
         self.updated.emit(self.start, self.end)
+        super().process_finished()
 
     def wait(self):
         """Wait for completion if a background job is running."""
         if self.busy:
             # we can't simply job.wait() because signals that are executed
             # in the main thread would then deadlock.
             loop = QEventLoop()
             self.updated.connect(loop.quit)
             loop.exec_()
 
     def peek(self, start, tree):
         """Reimplemented to get a sneak preview."""
         self.preview.emit(start, tree)
+        super().peek(start, tree)
 
     def root_lexicon(self):
         """Return the current root lexicon."""
         return self.root.lexicon
 
     def set_root_lexicon(self, root_lexicon):
         """Set the root lexicon to use to tokenize the text. Triggers a rebuild."""
```

### Comparing `parceqt-0.8.5/parceqt/treemodel.py` & `parceqt-0.9.0/parceqt/treemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 This can be used for debugging the tree using a Qt gui.
 See also the debug module.
 
 """
 
 
-from PyQt5.QtCore import QAbstractItemModel, QModelIndex, Qt
-
+import reprlib
 
-import parce.util
+from PyQt5.QtCore import QAbstractItemModel, QModelIndex, Qt
 
 
 class TreeModel(QAbstractItemModel):
     """TreeModel implements QAbstractItemModel to show a parce tree in
     Qt widgets such as a QTreeView.
 
     """
@@ -201,15 +200,15 @@
         d = dict(
             pos = node.pos,
             end = node.end,
             length = node.end - node.pos,
         )
         if node.is_token:
             d.update(
-                text = parce.util.abbreviate_repr(node.text),
+                text = reprlib.repr(node.text),
                 action = node.action,
                 group = format(node.group.index(node)) if node.group else "",
             )
         else:
             d.update(
                 name = node.lexicon,
                 count = "1 child" if len(node) == 1 else f"{len(node)} children"
```

### Comparing `parceqt-0.8.5/parceqt/util.py` & `parceqt-0.9.0/parceqt/util.py`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/parceqt.egg-info/PKG-INFO` & `parceqt-0.9.0/parceqt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: parceqt
-Version: 0.8.5
+Version: 0.9.0
 Summary: The parceqt Python module
 Home-page: https://github.com/wbsoft/parceqt
 Maintainer: Wilbert Berendsen
 Maintainer-email: info@wilbertberendsen.nl
 License: GPL
 Description: parceqt
         =======
```

### Comparing `parceqt-0.8.5/parceqt.egg-info/SOURCES.txt` & `parceqt-0.9.0/parceqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parceqt-0.8.5/setup.py` & `parceqt-0.9.0/setup.py`

 * *Files identical despite different names*

