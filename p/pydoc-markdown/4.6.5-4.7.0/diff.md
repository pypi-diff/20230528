# Comparing `tmp/pydoc_markdown-4.6.5.tar.gz` & `tmp/pydoc_markdown-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoc_markdown-4.6.5.tar", max compression
+gzip compressed data, was "pydoc_markdown-4.7.0.tar", max compression
```

## Comparing `pydoc_markdown-4.6.5.tar` & `pydoc_markdown-4.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.6.5/LICENSE
--rw-r--r--   0        0        0     4015 2023-05-28 02:47:20.788867 pydoc_markdown-4.6.5/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.6.5/readme.md
--rw-r--r--   0        0        0     8120 2023-05-28 02:47:20.788867 pydoc_markdown-4.6.5/src/pydoc_markdown/__init__.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/__init__.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/__init__.py
--rw-r--r--   0        0        0     5722 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/python.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/__init__.py
--rw-r--r--   0        0        0     5520 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/crossref.py
--rw-r--r--   0        0        0     3954 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/filter.py
--rw-r--r--   0        0        0     5971 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/google.py
--rw-r--r--   0        0        0     3875 2023-05-27 21:47:48.827975 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/pydocmd.py
--rw-r--r--   0        0        0     2740 2023-05-27 21:47:48.827975 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/smart.py
--rw-r--r--   0        0        0     5622 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/sphinx.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/__init__.py
--rw-r--r--   0        0        0     6850 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/docusaurus.py
--rw-r--r--   0        0        0    16915 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/hugo.py
--rw-r--r--   0        0        0     3949 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/jinja2.py
--rw-r--r--   0        0        0    22501 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/markdown.py
--rw-r--r--   0        0        0     7918 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/mkdocs.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/__init__.py
--rw-r--r--   0        0        0     6647 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/git.py
--rw-r--r--   0        0        0     7220 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/interfaces.py
--rw-r--r--   0        0        0    13822 2023-05-28 00:17:51.716178 pydoc_markdown-4.6.5/src/pydoc_markdown/main.py
--rw-r--r--   0        0        0     6467 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/novella/preprocessor.py
--rw-r--r--   0        0        0        0 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.5/src/pydoc_markdown/py.typed
--rw-r--r--   0        0        0     3375 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/static.py
--rw-r--r--   0        0        0        5 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.5/src/pydoc_markdown/util/__init__.py
--rw-r--r--   0        0        0     4013 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/util/docspec.py
--rw-r--r--   0        0        0     4545 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/util/knownfiles.py
--rw-r--r--   0        0        0      930 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/misc.py
--rw-r--r--   0        0        0      378 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/misc_test.py
--rw-r--r--   0        0        0     6851 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/pages.py
--rw-r--r--   0        0        0     2492 2023-05-27 23:49:43.440168 pydoc_markdown-4.6.5/src/pydoc_markdown/util/watchdog.py
--rw-r--r--   0        0        0     2999 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/ytemplate.py
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pydoc_markdown-4.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.7.0/LICENSE
+-rw-r--r--   0        0        0     4015 2023-05-28 02:49:02.897967 pydoc_markdown-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.7.0/readme.md
+-rw-r--r--   0        0        0     8120 2023-05-28 02:49:02.921966 pydoc_markdown-4.7.0/src/pydoc_markdown/__init__.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/__init__.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/__init__.py
+-rw-r--r--   0        0        0     5722 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/python.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/__init__.py
+-rw-r--r--   0        0        0     5520 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/crossref.py
+-rw-r--r--   0        0        0     3954 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/filter.py
+-rw-r--r--   0        0        0     5971 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/google.py
+-rw-r--r--   0        0        0     3875 2023-05-27 21:47:48.827975 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/pydocmd.py
+-rw-r--r--   0        0        0     2740 2023-05-27 21:47:48.827975 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/smart.py
+-rw-r--r--   0        0        0     5622 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/sphinx.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/__init__.py
+-rw-r--r--   0        0        0     6850 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/docusaurus.py
+-rw-r--r--   0        0        0    16915 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/hugo.py
+-rw-r--r--   0        0        0     3949 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/jinja2.py
+-rw-r--r--   0        0        0    22501 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/markdown.py
+-rw-r--r--   0        0        0     7918 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/mkdocs.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/__init__.py
+-rw-r--r--   0        0        0     6647 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/git.py
+-rw-r--r--   0        0        0     7220 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/interfaces.py
+-rw-r--r--   0        0        0    13822 2023-05-28 00:17:51.716178 pydoc_markdown-4.7.0/src/pydoc_markdown/main.py
+-rw-r--r--   0        0        0     6467 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/novella/preprocessor.py
+-rw-r--r--   0        0        0        0 2022-11-12 22:49:35.857142 pydoc_markdown-4.7.0/src/pydoc_markdown/py.typed
+-rw-r--r--   0        0        0     3375 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/static.py
+-rw-r--r--   0        0        0        5 2022-11-12 22:49:35.857142 pydoc_markdown-4.7.0/src/pydoc_markdown/util/__init__.py
+-rw-r--r--   0        0        0     4013 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/util/docspec.py
+-rw-r--r--   0        0        0     4545 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/util/knownfiles.py
+-rw-r--r--   0        0        0      930 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc.py
+-rw-r--r--   0        0        0      378 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc_test.py
+-rw-r--r--   0        0        0     6851 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/pages.py
+-rw-r--r--   0        0        0     2492 2023-05-27 23:49:43.440168 pydoc_markdown-4.7.0/src/pydoc_markdown/util/watchdog.py
+-rw-r--r--   0        0        0     2999 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/ytemplate.py
+-rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pydoc_markdown-4.7.0/PKG-INFO
```

### Comparing `pydoc_markdown-4.6.5/LICENSE` & `pydoc_markdown-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/pyproject.toml` & `pydoc_markdown-4.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoc-markdown"
-version = "4.6.5"
+version = "4.7.0"
 description = "Create Python API documentation in Markdown format."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "pydoc_markdown", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pydoc_markdown-4.6.5/readme.md` & `pydoc_markdown-4.7.0/readme.md`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/__init__.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from pydoc_markdown.contrib.processors.filter import FilterProcessor
 from pydoc_markdown.contrib.processors.smart import SmartProcessor
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Loader, Processor, Renderer, Resolver
 from pydoc_markdown.util import ytemplate
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "4.6.5"
+__version__ = "4.7.0"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Hooks:
     pre_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "pre-render"})
```

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/python.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/python.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/crossref.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/crossref.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/filter.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/filter.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/google.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/google.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/pydocmd.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/pydocmd.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/smart.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/smart.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/sphinx.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/docusaurus.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/docusaurus.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/hugo.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/hugo.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/jinja2.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/jinja2.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/markdown.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/mkdocs.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/mkdocs.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/git.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/git.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/interfaces.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/interfaces.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/main.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/main.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/novella/preprocessor.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/novella/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/static.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/static.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/docspec.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/docspec.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/knownfiles.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/knownfiles.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/misc.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/pages.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/pages.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/watchdog.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/watchdog.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/src/pydoc_markdown/util/ytemplate.py` & `pydoc_markdown-4.7.0/src/pydoc_markdown/util/ytemplate.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.5/PKG-INFO` & `pydoc_markdown-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoc-markdown
-Version: 4.6.5
+Version: 4.7.0
 Summary: Create Python API documentation in Markdown format.
 License: MIT
 Keywords: documentation,docs,generator,markdown,pydoc
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

