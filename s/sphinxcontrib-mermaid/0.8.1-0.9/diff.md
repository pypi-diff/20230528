# Comparing `tmp/sphinxcontrib-mermaid-0.8.1.tar.gz` & `tmp/sphinxcontrib-mermaid-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-mermaid-0.8.1.tar", last modified: Sat Feb 25 22:47:13 2023, max compression
+gzip compressed data, was "sphinxcontrib-mermaid-0.9.tar", last modified: Sun May 28 13:56:38 2023, max compression
```

## Comparing `sphinxcontrib-mermaid-0.8.1.tar` & `sphinxcontrib-mermaid-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-02-25 22:47:13.298397 sphinxcontrib-mermaid-0.8.1/
--rw-rw-r--   0 tin       (1000) tin       (1000)     2680 2023-02-25 22:35:03.000000 sphinxcontrib-mermaid-0.8.1/CHANGELOG.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)     1370 2023-02-09 01:41:06.000000 sphinxcontrib-mermaid-0.8.1/LICENSE.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)      101 2023-02-09 01:41:06.000000 sphinxcontrib-mermaid-0.8.1/MANIFEST.in
--rw-rw-r--   0 tin       (1000) tin       (1000)    11533 2023-02-25 22:47:13.298397 sphinxcontrib-mermaid-0.8.1/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)     8263 2023-02-25 22:47:00.000000 sphinxcontrib-mermaid-0.8.1/README.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)       38 2023-02-25 22:47:13.298397 sphinxcontrib-mermaid-0.8.1/setup.cfg
--rw-rw-r--   0 tin       (1000) tin       (1000)     2328 2023-02-25 22:46:38.000000 sphinxcontrib-mermaid-0.8.1/setup.py
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-02-25 22:47:13.294397 sphinxcontrib-mermaid-0.8.1/sphinxcontrib/
--rw-rw-r--   0 tin       (1000) tin       (1000)      341 2023-02-09 01:41:06.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib/__init__.py
--rw-rw-r--   0 tin       (1000) tin       (1000)     1869 2023-02-09 12:21:10.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib/autoclassdiag.py
--rw-rw-r--   0 tin       (1000) tin       (1000)      104 2023-02-09 12:21:25.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib/exceptions.py
--rw-rw-r--   0 tin       (1000) tin       (1000)    13897 2023-02-25 22:18:49.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib/mermaid.py
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-02-25 22:47:13.298397 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/
--rw-rw-r--   0 tin       (1000) tin       (1000)    11533 2023-02-25 22:47:13.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)      420 2023-02-25 22:47:13.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/SOURCES.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)        1 2023-02-25 22:47:13.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/dependency_links.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       14 2023-02-25 22:47:13.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/namespace_packages.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       14 2023-02-25 22:47:13.000000 sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/top_level.txt
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-02-25 22:47:13.298397 sphinxcontrib-mermaid-0.8.1/tests/
--rw-rw-r--   0 tin       (1000) tin       (1000)     1880 2023-02-09 01:41:06.000000 sphinxcontrib-mermaid-0.8.1/tests/test_html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:56:38.792935 sphinxcontrib-mermaid-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-28 13:56:38.792935 sphinxcontrib-mermaid-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:56:38.792935 sphinxcontrib-mermaid-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:56:38.788936 sphinxcontrib-mermaid-0.9/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib/autoclassdiag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib/mermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:56:38.792935 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-28 13:56:38.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-28 13:56:38.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:56:38.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 13:56:38.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 13:56:38.000000 sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:56:38.792935 sphinxcontrib-mermaid-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-28 13:56:31.000000 sphinxcontrib-mermaid-0.9/tests/test_html.py
```

### Comparing `sphinxcontrib-mermaid-0.8.1/CHANGELOG.rst` & `sphinxcontrib-mermaid-0.9/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Changelog
 ---------
 
-0.8.1 (Feb 9, 2023)
+0.9.1 (May 28, 2023)
++++++++++++++++++++++
+
+- Implemented zoom on diagrams functionality. Contributed by `Daniel Althviz Moré <https://github.com/dalthviz>`_
+- Fix a bug on empty diagram generations. Contributed by `Kevin Deldycke <https://github.com/kdeldycke>`_.  
+- Upgrade default to Mermaid 10.2.0. 
+- Implement automatic releases from Github Actions when a tag is pushed 
+
+See full `set of changes <https://github.com/mgaitan/sphinxcontrib-mermaid/compare/0.9.1...0.8.1>`_.
+
+
+0.8.1 (Feb 25, 2023)
 +++++++++++++++++++++
 
 - Default to Mermaid 9.4.0 as 10.0 introduced incompatible changes. 
   See `the discussion <https://github.com/mermaid-js/mermaid/discussions/4148>`_. 
 
 0.8 (Feb 9, 2023)
 +++++++++++++++++++++
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sphinxcontrib-mermaid-0.8.1/LICENSE.rst` & `sphinxcontrib-mermaid-0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-mermaid-0.8.1/PKG-INFO` & `sphinxcontrib-mermaid-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-mermaid
-Version: 0.8.1
+Version: 0.9
 Summary: Mermaid diagrams in yours Sphinx powered docs
 Home-page: https://github.com/mgaitan/sphinxcontrib-mermaid
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-mermaid
 Author: Martín Gaitán
 Author-email: gaitan@gmail.com
 License: BSD
 Platform: any
@@ -27,16 +27,23 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 License-File: LICENSE.rst
 
 .. image:: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml/badge.svg
     :target: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml
 
-This extension allows you to embed `Mermaid <https://mermaid-js.github.io/mermaid>`_ graphs in your
-documents, including general flowcharts, sequence and gantt diagrams.
+.. image:: https://img.shields.io/pypi/v/sphinxcontrib-mermaid
+   :target: https://pypi.org/project/sphinxcontrib-mermaid/
+
+.. image:: https://img.shields.io/pypi/dm/shbin
+   :target: https://libraries.io/pypi/sphinxcontrib-mermaid/
+
+
+This extension allows you to embed `Mermaid <https://mermaid.js.org/>`_ graphs in your
+documents, including general flowcharts, sequence diagrams, gantt diagrams and more.
 
 It adds a directive to embed mermaid markup. For example::
 
   .. mermaid::
 
      sequenceDiagram
         participant Alice
@@ -119,26 +126,33 @@
 
 ``:alt:``: determines the image's alternate text for HTML output.  If not given, the alternate text defaults to the mermaid code.
 
 ``:align:``: determines the image's position. Valid options are ``'left'``, ``'center'``, ``'right'``
 
 ``:caption:``: can be used to give a caption to the diagram.
 
+``:zoom:``: can be used to enable zooming the diagram. For a global config see ``mermaid_d3_zoom``` bellow. 
+
+.. figure:: https://user-images.githubusercontent.com/16781833/228022911-c26d1e01-7f71-4ab7-bb33-ce53056f8343.gif
+   :align: center
+   
+   A preview after adding ``:zoom:`` option only to the first diagram example above:
+
 
 Config values
 -------------
 
 ``mermaid_output_format``
 
    The output format for Mermaid when building HTML files.  This must be either ``'raw'``
    ``'png'`` or ``'svg'``; the default is ``'raw'``. ``mermaid-cli`` is required if it's not ``raw``
 
 ``mermaid_version``
 
-  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"9.4.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
+  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"10.2.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
 
   If it's set to ``""``, the lib won't be automatically included from the CDN service and you'll need to add it as a local
   file in ``html_js_files``. For instance, if you download the lib to `_static/js/mermaid.js`, in ``conf.py``::
 
 
     html_js_files = [
        'js/mermaid.js',
@@ -179,14 +193,18 @@
     process.
 
 ``mermaid_pdfcrop``
 
     If using latex output, it might be useful to crop the pdf just to the needed space. For this, ``pdfcrop`` can be used.
     State binary name to use this extra function.
 
+``mermaid_d3_zoom``
+
+    Enables zooming in all the generated Mermaid diagrams.
+
 
 Markdown support
 ----------------
 
 You can include Mermaid diagrams in your Markdown documents in Sphinx.
 You just need to setup the `markdown support in Sphinx <https://www.sphinx-doc.org/en/master/usage/markdown.html>`_ via
 `myst-parser <https://myst-parser.readthedocs.io/>`_
@@ -261,15 +279,26 @@
 3. In your documentation ``conf.py`` file, add: ::
 
     mermaid_params = ['-p' 'puppeteer-config.json']
 
 Changelog
 ---------
 
-0.8.1 (Feb 9, 2023)
+0.9.1 (May 28, 2023)
++++++++++++++++++++++
+
+- Implemented zoom on diagrams functionality. Contributed by `Daniel Althviz Moré <https://github.com/dalthviz>`_
+- Fix a bug on empty diagram generations. Contributed by `Kevin Deldycke <https://github.com/kdeldycke>`_.  
+- Upgrade default to Mermaid 10.2.0. 
+- Implement automatic releases from Github Actions when a tag is pushed 
+
+See full `set of changes <https://github.com/mgaitan/sphinxcontrib-mermaid/compare/0.9.1...0.8.1>`_.
+
+
+0.8.1 (Feb 25, 2023)
 +++++++++++++++++++++
 
 - Default to Mermaid 9.4.0 as 10.0 introduced incompatible changes. 
   See `the discussion <https://github.com/mermaid-js/mermaid/discussions/4148>`_. 
 
 0.8 (Feb 9, 2023)
 +++++++++++++++++++++
```

### Comparing `sphinxcontrib-mermaid-0.8.1/README.rst` & `sphinxcontrib-mermaid-0.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. image:: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml/badge.svg
     :target: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml
 
-This extension allows you to embed `Mermaid <https://mermaid-js.github.io/mermaid>`_ graphs in your
-documents, including general flowcharts, sequence and gantt diagrams.
+.. image:: https://img.shields.io/pypi/v/sphinxcontrib-mermaid
+   :target: https://pypi.org/project/sphinxcontrib-mermaid/
+
+.. image:: https://img.shields.io/pypi/dm/shbin
+   :target: https://libraries.io/pypi/sphinxcontrib-mermaid/
+
+
+This extension allows you to embed `Mermaid <https://mermaid.js.org/>`_ graphs in your
+documents, including general flowcharts, sequence diagrams, gantt diagrams and more.
 
 It adds a directive to embed mermaid markup. For example::
 
   .. mermaid::
 
      sequenceDiagram
         participant Alice
@@ -105,26 +112,33 @@
 
 ``:alt:``: determines the image's alternate text for HTML output.  If not given, the alternate text defaults to the mermaid code.
 
 ``:align:``: determines the image's position. Valid options are ``'left'``, ``'center'``, ``'right'``
 
 ``:caption:``: can be used to give a caption to the diagram.
 
+``:zoom:``: can be used to enable zooming the diagram. For a global config see ``mermaid_d3_zoom``` bellow. 
+
+.. figure:: https://user-images.githubusercontent.com/16781833/228022911-c26d1e01-7f71-4ab7-bb33-ce53056f8343.gif
+   :align: center
+   
+   A preview after adding ``:zoom:`` option only to the first diagram example above:
+
 
 Config values
 -------------
 
 ``mermaid_output_format``
 
    The output format for Mermaid when building HTML files.  This must be either ``'raw'``
    ``'png'`` or ``'svg'``; the default is ``'raw'``. ``mermaid-cli`` is required if it's not ``raw``
 
 ``mermaid_version``
 
-  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"9.4.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
+  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"10.2.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
 
   If it's set to ``""``, the lib won't be automatically included from the CDN service and you'll need to add it as a local
   file in ``html_js_files``. For instance, if you download the lib to `_static/js/mermaid.js`, in ``conf.py``::
 
 
     html_js_files = [
        'js/mermaid.js',
@@ -167,14 +181,18 @@
     process.
 
 ``mermaid_pdfcrop``
 
     If using latex output, it might be useful to crop the pdf just to the needed space. For this, ``pdfcrop`` can be used.
     State binary name to use this extra function.
 
+``mermaid_d3_zoom``
+
+    Enables zooming in all the generated Mermaid diagrams.
+
 
 Markdown support
 ----------------
 
 You can include Mermaid diagrams in your Markdown documents in Sphinx.
 You just need to setup the `markdown support in Sphinx <https://www.sphinx-doc.org/en/master/usage/markdown.html>`_ via
 `myst-parser <https://myst-parser.readthedocs.io/>`_
```

### Comparing `sphinxcontrib-mermaid-0.8.1/setup.py` & `sphinxcontrib-mermaid-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 readme = open("README.rst", encoding="utf-8").read()
 changes = open("CHANGELOG.rst", encoding="utf-8").read()
-version = "0.8.1"
+version = "0.9"
 
 
 def long_description():
     """
     return readme + changes, removing directive blocks that are only valid in the context
     of sphinx doc"""
 
@@ -21,16 +21,14 @@
 
     readme_ = remove_block(readme, ".. mermaid::", margin=2)
     readme_ = remove_block(readme_, ".. autoclasstree::")
     readme_ = remove_block(readme_, ".. autoclasstree::")
     readme_ = remove_block(readme_, ".. versionchanged::")
     return f"{readme_}\n\n{changes}"
 
-print(long_description().splitlines()[107:111])
-
 
 setup(
     name="sphinxcontrib-mermaid",
     version=version,
     url="https://github.com/mgaitan/sphinxcontrib-mermaid",
     download_url="https://pypi.python.org/pypi/sphinxcontrib-mermaid",
     license="BSD",
```

### Comparing `sphinxcontrib-mermaid-0.8.1/sphinxcontrib/autoclassdiag.py` & `sphinxcontrib-mermaid-0.9/sphinxcontrib/autoclassdiag.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,17 @@
             inheritances.add((base.__name__, cls.__name__))
             if full:
                 get_tree(base)
 
     for cls in get_classes(*cls_or_modules, strict=strict):
         get_tree(cls)
 
+    if not inheritances:
+        return ""
+
     return "classDiagram\n" + "\n".join(
         f"  {a} <|-- {b}" for a, b in sorted(inheritances)
     )
 
 
 if __name__ == "__main__":
```

### Comparing `sphinxcontrib-mermaid-0.8.1/sphinxcontrib/mermaid.py` & `sphinxcontrib-mermaid-0.9/sphinxcontrib/mermaid.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 
     Allow mermaid diagrams to be included in Sphinx-generated
     documents inline.
 
     :copyright: Copyright 2016-2023 by Martín Gaitán and others
     :license: BSD, see LICENSE for details.
 """
+from __future__ import annotations
 
 import codecs
+import errno
 import os
+import posixpath
 import re
 from hashlib import sha1
 from subprocess import PIPE, Popen
 from tempfile import _get_default_tempdir
+import uuid
 
-import posixpath
 import sphinx
 from docutils import nodes
 from docutils.parsers.rst import Directive, directives
 from docutils.statemachine import ViewList
+from sphinx.application import Sphinx
 from sphinx.locale import _
 from sphinx.util import logging
 from sphinx.util.i18n import search_image_for_language
 from sphinx.util.osutil import ensuredir
 
 from .autoclassdiag import class_diagram
 from .exceptions import MermaidError
@@ -67,14 +71,15 @@
     required_arguments = 0
     optional_arguments = 1
     final_argument_whitespace = False
     option_spec = {
         "alt": directives.unchanged,
         "align": align_spec,
         "caption": directives.unchanged,
+        "zoom": directives.unchanged,
     }
 
     def get_mm_code(self):
         if self.arguments:
             # try to load mermaid code from an external file
             document = self.state.document
             if self.content:
@@ -99,34 +104,45 @@
                         "it failed" % filename,
                         line=self.lineno,
                     )
                 ]
         else:
             # inline mermaid code
             mmcode = "\n".join(self.content)
-            if not mmcode.strip():
-                return [
-                    self.state_machine.reporter.warning(
-                        'Ignoring "mermaid" directive without content.',
-                        line=self.lineno,
-                    )
-                ]
         return mmcode
 
     def run(self):
+        mmcode = self.get_mm_code()
+        # mmcode is a list, so it's a system message, not content to be included in the
+        # document.
+        if not isinstance(mmcode, str):
+            return mmcode
+
+        # if mmcode is empty, ignore the directive.
+        if not mmcode.strip():
+            return [
+                self.state_machine.reporter.warning(
+                    'Ignoring "mermaid" directive without content.',
+                    line=self.lineno,
+                )
+            ]
 
+        # Wrap the mermaid code into a code node.
         node = mermaid()
-        node["code"] = self.get_mm_code()
+        node["code"] = mmcode
         node["options"] = {}
         if "alt" in self.options:
             node["alt"] = self.options["alt"]
         if "align" in self.options:
             node["align"] = self.options["align"]
         if "inline" in self.options:
             node["inline"] = True
+        if "zoom" in self.options:
+            node["zoom"] = True
+            node["zoom_id"] = f"id-{uuid.uuid4()}"
 
         caption = self.options.get("caption")
         if caption:
             node = figure_wrapper(self, node, caption)
 
         return [node]
 
@@ -213,26 +229,36 @@
         )
     return relfn, outfn
 
 
 def _render_mm_html_raw(
     self, node, code, options, prefix="mermaid", imgcls=None, alt=None
 ):
-    if "align" in node:
+    if "align" in node and "zoom_id" in node:
+        tag_template = """<div align="{align}" id="{zoom_id}" class="mermaid align-{align}">
+            {code}
+        </div>
+        """
+    elif "align" in node and "zoom_id" not in node:
         tag_template = """<div align="{align}" class="mermaid align-{align}">
             {code}
         </div>
         """
+    elif "align" not in node and "zoom_id" in node:
+        tag_template = """<div id="{zoom_id}" class="mermaid">
+            {code}
+        </div>
+        """
     else:
         tag_template = """<div class="mermaid">
             {code}
         </div>"""
 
     self.body.append(
-        tag_template.format(align=node.get("align"), code=self.encode(code))
+        tag_template.format(align=node.get("align"), zoom_id=node.get("zoom_id"), code=self.encode(code))
     )
     raise nodes.SkipNode
 
 
 def render_mm_html(self, node, code, options, prefix="mermaid", imgcls=None, alt=None):
 
     _fmt = self.builder.config.mermaid_output_format
@@ -289,15 +315,15 @@
         raise nodes.SkipNode
 
     if self.builder.config.mermaid_pdfcrop != "":
         mm_args = [self.builder.config.mermaid_pdfcrop, outfn]
         try:
             p = Popen(mm_args, stdout=PIPE, stdin=PIPE, stderr=PIPE)
         except OSError as err:
-            if err.errno != ENOENT:  # No such file or directory
+            if err.errno != errno.ENOENT:   # No such file or directory
                 raise
             logger.warning(
                 f"command {self.builder.config.mermaid_pdfcrop!r} cannot be run (needed to crop pdf), check the mermaid_cmd setting"
             )
             return None, None
 
         stdout, stderr = p.communicate()
@@ -374,32 +400,90 @@
     if "alt" in node.attributes:
         self.body.append(_("[graph: %s]") % node["alt"])
     else:
         self.body.append(_("[graph]"))
     raise nodes.SkipNode
 
 
-def install_js(app, *args):
-    # add required javascript
+def install_js(
+    app: Sphinx,
+    pagename,
+    templatename: str,
+    context: dict,
+    doctree: nodes.document | None,
+) -> None:
+    # Skip for pages without Mermaid diagrams
+    if doctree and not doctree.next_node(mermaid):
+        return
+
+    # Add required JavaScript
     if not app.config.mermaid_version:
-        _mermaid_js_url = None  # asummed is local
+        _mermaid_js_url = None  # assume it is local
     elif app.config.mermaid_version == "latest":
         _mermaid_js_url = "https://unpkg.com/mermaid/dist/mermaid.min.js"
     else:
         _mermaid_js_url = f"https://unpkg.com/mermaid@{app.config.mermaid_version}/dist/mermaid.min.js"
     if _mermaid_js_url:
         app.add_js_file(_mermaid_js_url, priority=app.config.mermaid_js_priority)
 
     if app.config.mermaid_init_js:
         # If mermaid is local the init-call must be placed after `html_js_files` which has a priority of 800.
         priority = (
             app.config.mermaid_init_js_priority if _mermaid_js_url is not None else 801
         )
         app.add_js_file(None, body=app.config.mermaid_init_js, priority=priority)
 
+    if app.config.mermaid_output_format == "raw":
+        if app.config.mermaid_d3_zoom:
+            _d3_js_url = "https://unpkg.com/d3/dist/d3.min.js"
+            _d3_js_script = """
+            window.addEventListener("load", function () {
+              var svgs = d3.selectAll(".mermaid svg");
+              svgs.each(function() {
+                var svg = d3.select(this);
+                svg.html("<g>" + svg.html() + "</g>");
+                var inner = svg.select("g");
+                var zoom = d3.zoom().on("zoom", function(event) {
+                  inner.attr("transform", event.transform);
+                });
+                svg.call(zoom);
+              });
+            });
+            """
+            app.add_js_file(_d3_js_url, priority=app.config.mermaid_js_priority)
+            app.add_js_file(None, body=_d3_js_script, priority=app.config.mermaid_js_priority)
+        elif doctree:
+            mermaid_nodes = doctree.findall(mermaid)
+            _d3_selector = ""
+            for mermaid_node in mermaid_nodes:
+                if "zoom_id" in mermaid_node:
+                    _zoom_id = mermaid_node["zoom_id"]
+                    if _d3_selector == "":
+                        _d3_selector += f".mermaid#{_zoom_id} svg"
+                    else:
+                        _d3_selector += f", .mermaid#{_zoom_id} svg"
+            if _d3_selector != "":
+                _d3_js_url = "https://unpkg.com/d3/dist/d3.min.js"
+                _d3_js_script = f"""
+                window.addEventListener("load", function () {{
+                  var svgs = d3.selectAll("{_d3_selector}");
+                  svgs.each(function() {{
+                    var svg = d3.select(this);
+                    svg.html("<g>" + svg.html() + "</g>");
+                    var inner = svg.select("g");
+                    var zoom = d3.zoom().on("zoom", function(event) {{
+                      inner.attr("transform", event.transform);
+                    }});
+                    svg.call(zoom);
+                  }});
+                }});
+                """
+                app.add_js_file(_d3_js_url, priority=app.config.mermaid_js_priority)
+                app.add_js_file(None, body=_d3_js_script, priority=app.config.mermaid_js_priority)
+
 
 def setup(app):
     app.add_node(
         mermaid,
         html=(html_visit_mermaid, None),
         latex=(latex_visit_mermaid, None),
         texinfo=(texinfo_visit_mermaid, None),
@@ -417,16 +501,17 @@
     app.add_config_value("mermaid_verbose", False, "html")
     app.add_config_value("mermaid_sequence_config", False, "html")
     
     # Starting in version 10, mermaid is an "ESM only" package
     # thus it requires a different initialization code not yet supported. 
     # So the current latest version supported is this
     # Discussion: https://github.com/mermaid-js/mermaid/discussions/4148
-    app.add_config_value("mermaid_version", "9.4.0", "html")
+    app.add_config_value("mermaid_version", "10.2.0", "html")
     app.add_config_value("mermaid_js_priority", 500, "html")
     app.add_config_value("mermaid_init_js_priority", 500, "html")
     app.add_config_value(
         "mermaid_init_js", "mermaid.initialize({startOnLoad:true});", "html"
     )
+    app.add_config_value("mermaid_d3_zoom", False, "html")
     app.connect("html-page-context", install_js)
 
     return {"version": sphinx.__display_version__, "parallel_read_safe": True}
```

### Comparing `sphinxcontrib-mermaid-0.8.1/sphinxcontrib_mermaid.egg-info/PKG-INFO` & `sphinxcontrib-mermaid-0.9/sphinxcontrib_mermaid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-mermaid
-Version: 0.8.1
+Version: 0.9
 Summary: Mermaid diagrams in yours Sphinx powered docs
 Home-page: https://github.com/mgaitan/sphinxcontrib-mermaid
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-mermaid
 Author: Martín Gaitán
 Author-email: gaitan@gmail.com
 License: BSD
 Platform: any
@@ -27,16 +27,23 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 License-File: LICENSE.rst
 
 .. image:: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml/badge.svg
     :target: https://github.com/mgaitan/sphinxcontrib-mermaid/actions/workflows/test.yml
 
-This extension allows you to embed `Mermaid <https://mermaid-js.github.io/mermaid>`_ graphs in your
-documents, including general flowcharts, sequence and gantt diagrams.
+.. image:: https://img.shields.io/pypi/v/sphinxcontrib-mermaid
+   :target: https://pypi.org/project/sphinxcontrib-mermaid/
+
+.. image:: https://img.shields.io/pypi/dm/shbin
+   :target: https://libraries.io/pypi/sphinxcontrib-mermaid/
+
+
+This extension allows you to embed `Mermaid <https://mermaid.js.org/>`_ graphs in your
+documents, including general flowcharts, sequence diagrams, gantt diagrams and more.
 
 It adds a directive to embed mermaid markup. For example::
 
   .. mermaid::
 
      sequenceDiagram
         participant Alice
@@ -119,26 +126,33 @@
 
 ``:alt:``: determines the image's alternate text for HTML output.  If not given, the alternate text defaults to the mermaid code.
 
 ``:align:``: determines the image's position. Valid options are ``'left'``, ``'center'``, ``'right'``
 
 ``:caption:``: can be used to give a caption to the diagram.
 
+``:zoom:``: can be used to enable zooming the diagram. For a global config see ``mermaid_d3_zoom``` bellow. 
+
+.. figure:: https://user-images.githubusercontent.com/16781833/228022911-c26d1e01-7f71-4ab7-bb33-ce53056f8343.gif
+   :align: center
+   
+   A preview after adding ``:zoom:`` option only to the first diagram example above:
+
 
 Config values
 -------------
 
 ``mermaid_output_format``
 
    The output format for Mermaid when building HTML files.  This must be either ``'raw'``
    ``'png'`` or ``'svg'``; the default is ``'raw'``. ``mermaid-cli`` is required if it's not ``raw``
 
 ``mermaid_version``
 
-  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"9.4.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
+  The version of mermaid that will be used to parse ``raw`` output in HTML files. This should match a version available on https://unpkg.com/browse/mermaid/.  The default is ``"10.2.0"``. If you need a newer version, you'll need to add the custom initialization. See below. 
 
   If it's set to ``""``, the lib won't be automatically included from the CDN service and you'll need to add it as a local
   file in ``html_js_files``. For instance, if you download the lib to `_static/js/mermaid.js`, in ``conf.py``::
 
 
     html_js_files = [
        'js/mermaid.js',
@@ -179,14 +193,18 @@
     process.
 
 ``mermaid_pdfcrop``
 
     If using latex output, it might be useful to crop the pdf just to the needed space. For this, ``pdfcrop`` can be used.
     State binary name to use this extra function.
 
+``mermaid_d3_zoom``
+
+    Enables zooming in all the generated Mermaid diagrams.
+
 
 Markdown support
 ----------------
 
 You can include Mermaid diagrams in your Markdown documents in Sphinx.
 You just need to setup the `markdown support in Sphinx <https://www.sphinx-doc.org/en/master/usage/markdown.html>`_ via
 `myst-parser <https://myst-parser.readthedocs.io/>`_
@@ -261,15 +279,26 @@
 3. In your documentation ``conf.py`` file, add: ::
 
     mermaid_params = ['-p' 'puppeteer-config.json']
 
 Changelog
 ---------
 
-0.8.1 (Feb 9, 2023)
+0.9.1 (May 28, 2023)
++++++++++++++++++++++
+
+- Implemented zoom on diagrams functionality. Contributed by `Daniel Althviz Moré <https://github.com/dalthviz>`_
+- Fix a bug on empty diagram generations. Contributed by `Kevin Deldycke <https://github.com/kdeldycke>`_.  
+- Upgrade default to Mermaid 10.2.0. 
+- Implement automatic releases from Github Actions when a tag is pushed 
+
+See full `set of changes <https://github.com/mgaitan/sphinxcontrib-mermaid/compare/0.9.1...0.8.1>`_.
+
+
+0.8.1 (Feb 25, 2023)
 +++++++++++++++++++++
 
 - Default to Mermaid 9.4.0 as 10.0 introduced incompatible changes. 
   See `the discussion <https://github.com/mermaid-js/mermaid/discussions/4148>`_. 
 
 0.8 (Feb 9, 2023)
 +++++++++++++++++++++
```

