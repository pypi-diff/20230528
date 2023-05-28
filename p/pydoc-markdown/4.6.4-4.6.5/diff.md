# Comparing `tmp/pydoc_markdown-4.6.4.tar.gz` & `tmp/pydoc_markdown-4.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoc_markdown-4.6.4.tar", max compression
+gzip compressed data, was "pydoc_markdown-4.6.5.tar", max compression
```

## Comparing `pydoc_markdown-4.6.4.tar` & `pydoc_markdown-4.6.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.6.4/LICENSE
--rw-r--r--   0        0        0     3824 2022-11-13 00:50:45.636867 pydoc_markdown-4.6.4/pyproject.toml
--rw-r--r--   0        0        0     3383 2022-11-13 00:46:13.636810 pydoc_markdown-4.6.4/readme.md
--rw-r--r--   0        0        0     8120 2022-11-13 00:50:45.636867 pydoc_markdown-4.6.4/src/pydoc_markdown/__init__.py
--rw-r--r--   0        0        0       81 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/__init__.py
--rw-r--r--   0        0        0       81 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/loaders/__init__.py
--rw-r--r--   0        0        0     5631 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/loaders/python.py
--rw-r--r--   0        0        0       81 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/__init__.py
--rw-r--r--   0        0        0     5520 2022-11-12 23:02:00.771408 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/crossref.py
--rw-r--r--   0        0        0     3954 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/filter.py
--rw-r--r--   0        0        0     5962 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/google.py
--rw-r--r--   0        0        0     3875 2022-11-13 00:39:19.684900 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/pydocmd.py
--rw-r--r--   0        0        0     2740 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/smart.py
--rw-r--r--   0        0        0     5622 2022-11-13 00:46:46.587848 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/sphinx.py
--rw-r--r--   0        0        0       81 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/__init__.py
--rw-r--r--   0        0        0     6817 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/docusaurus.py
--rw-r--r--   0        0        0    16828 2022-11-12 23:51:47.932204 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/hugo.py
--rw-r--r--   0        0        0     3949 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/jinja2.py
--rw-r--r--   0        0        0    22372 2022-11-12 23:56:43.623597 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/markdown.py
--rw-r--r--   0        0        0     7918 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/mkdocs.py
--rw-r--r--   0        0        0       81 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/source_linkers/__init__.py
--rw-r--r--   0        0        0     6647 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/source_linkers/git.py
--rw-r--r--   0        0        0     7220 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/interfaces.py
--rw-r--r--   0        0        0    13822 2022-11-12 23:53:10.221810 pydoc_markdown-4.6.4/src/pydoc_markdown/main.py
--rw-r--r--   0        0        0     6467 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/novella/preprocessor.py
--rw-r--r--   0        0        0        0 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/py.typed
--rw-r--r--   0        0        0     3375 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/static.py
--rw-r--r--   0        0        0        5 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/util/__init__.py
--rw-r--r--   0        0        0     4013 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/util/docspec.py
--rw-r--r--   0        0        0     4545 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/util/knownfiles.py
--rw-r--r--   0        0        0     6764 2022-11-12 23:29:43.810768 pydoc_markdown-4.6.4/src/pydoc_markdown/util/pages.py
--rw-r--r--   0        0        0     2424 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.4/src/pydoc_markdown/util/watchdog.py
--rw-r--r--   0        0        0     2984 2022-11-12 23:29:18.931495 pydoc_markdown-4.6.4/src/pydoc_markdown/util/ytemplate.py
--rw-r--r--   0        0        0     7618 1970-01-01 00:00:00.000000 pydoc_markdown-4.6.4/setup.py
--rw-r--r--   0        0        0     5107 1970-01-01 00:00:00.000000 pydoc_markdown-4.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.6.5/LICENSE
+-rw-r--r--   0        0        0     4015 2023-05-28 02:47:20.788867 pydoc_markdown-4.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.6.5/readme.md
+-rw-r--r--   0        0        0     8120 2023-05-28 02:47:20.788867 pydoc_markdown-4.6.5/src/pydoc_markdown/__init__.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/__init__.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/__init__.py
+-rw-r--r--   0        0        0     5722 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/python.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/__init__.py
+-rw-r--r--   0        0        0     5520 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/crossref.py
+-rw-r--r--   0        0        0     3954 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/filter.py
+-rw-r--r--   0        0        0     5971 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/google.py
+-rw-r--r--   0        0        0     3875 2023-05-27 21:47:48.827975 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/pydocmd.py
+-rw-r--r--   0        0        0     2740 2023-05-27 21:47:48.827975 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/smart.py
+-rw-r--r--   0        0        0     5622 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/sphinx.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/__init__.py
+-rw-r--r--   0        0        0     6850 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/docusaurus.py
+-rw-r--r--   0        0        0    16915 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/hugo.py
+-rw-r--r--   0        0        0     3949 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/jinja2.py
+-rw-r--r--   0        0        0    22501 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/markdown.py
+-rw-r--r--   0        0        0     7918 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/mkdocs.py
+-rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/__init__.py
+-rw-r--r--   0        0        0     6647 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/git.py
+-rw-r--r--   0        0        0     7220 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/interfaces.py
+-rw-r--r--   0        0        0    13822 2023-05-28 00:17:51.716178 pydoc_markdown-4.6.5/src/pydoc_markdown/main.py
+-rw-r--r--   0        0        0     6467 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/novella/preprocessor.py
+-rw-r--r--   0        0        0        0 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.5/src/pydoc_markdown/py.typed
+-rw-r--r--   0        0        0     3375 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/static.py
+-rw-r--r--   0        0        0        5 2022-11-12 22:49:35.857142 pydoc_markdown-4.6.5/src/pydoc_markdown/util/__init__.py
+-rw-r--r--   0        0        0     4013 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/util/docspec.py
+-rw-r--r--   0        0        0     4545 2022-11-21 08:38:49.340005 pydoc_markdown-4.6.5/src/pydoc_markdown/util/knownfiles.py
+-rw-r--r--   0        0        0      930 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/misc.py
+-rw-r--r--   0        0        0      378 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/misc_test.py
+-rw-r--r--   0        0        0     6851 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/pages.py
+-rw-r--r--   0        0        0     2492 2023-05-27 23:49:43.440168 pydoc_markdown-4.6.5/src/pydoc_markdown/util/watchdog.py
+-rw-r--r--   0        0        0     2999 2023-05-27 21:46:22.746425 pydoc_markdown-4.6.5/src/pydoc_markdown/util/ytemplate.py
+-rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pydoc_markdown-4.6.5/PKG-INFO
```

### Comparing `pydoc_markdown-4.6.4/LICENSE` & `pydoc_markdown-4.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/pyproject.toml` & `pydoc_markdown-4.6.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 [tool.poetry]
 name = "pydoc-markdown"
-version = "4.6.4"
+version = "4.6.5"
 description = "Create Python API documentation in Markdown format."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
-packages = [{include = "pydoc_markdown", from = "src"}]
+packages = [{ include = "pydoc_markdown", from = "src" }]
 classifiers = [
-  "Development Status :: 3 - Alpha",
-  "Intended Audience :: Developers",
-  "Intended Audience :: End Users/Desktop",
-  "Topic :: Software Development :: Code Generators",
-  "Topic :: Utilities",
-  "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "Topic :: Software Development :: Code Generators",
+    "Topic :: Utilities",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
 ]
-keywords = [ "documentation", "docs", "generator", "markdown", "pydoc" ]
+keywords = ["documentation", "docs", "generator", "markdown", "pydoc"]
+
+[tool.poetry.urls]
+Homepage = "https://github.com/NiklasRosenstein/pydoc-markdown"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=7.1,<9.0"
 "databind" = "^1.5.0"
 docspec = "^2.0.0a1"
 docspec-python = "^2.0.0a1"
 docstring-parser = "^0.11"
 "nr.util" = ">=0.7.5,<1.0.0"
 jinja2 = "^3.0.0"
 requests = "^2.23.0"
-PyYAML = "^5.3"
+PyYAML = ">=5.0,<7.0"
 tomli = "^2.0.0"
 tomli_w = "^1.0.0"
 yapf = ">=0.30.0"
 watchdog = "*"
 
-[tool.poetry.urls]
-Homepage = "https://github.com/NiklasRosenstein/pydoc-markdown"
-
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-coverage = "*"
 mypy = "*"
 types-deprecated = "*"
 types-requests = "*"
 types-PyYAML = "*"
 isort = "^5.10.1"
 black = "^22.3.0"
 
-[tool.poetry.extras]
-novella = ["novella >=0.1.10,<0.3.0"]
-docs = ["novella >=0.1.10,<0.3.0", "mkdocs", "mkdocs-material"]
+[tool.poetry.group.novella]
+optional = true
+
+[tool.poetry.group.novella.dependencies]
+novella = { version = " >=0.1.10,<0.3.0" }
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+novella = { version = " >=0.1.10,<0.3.0" }
+mkdocs = "*"
+mkdocs-material = "*"
 
 [tool.poetry.scripts]
 pydoc-markdown = "pydoc_markdown.main:cli"
 
 [tool.poetry.plugins."pydoc_markdown.interfaces.Loader"]
 python = "pydoc_markdown.contrib.loaders.python:PythonLoader"
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/__init__.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from pydoc_markdown.contrib.processors.filter import FilterProcessor
 from pydoc_markdown.contrib.processors.smart import SmartProcessor
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Loader, Processor, Renderer, Resolver
 from pydoc_markdown.util import ytemplate
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "4.6.4"
+__version__ = "4.6.5"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Hooks:
     pre_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "pre-render"})
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/loaders/python.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/loaders/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,17 @@
     #: List of modules to ignore when using module discovery on the #search_path.
     ignore_when_discovered: t.List[str] = dataclasses.field(default_factory=lambda: ["test", "tests", "setup"])
 
     #: Options for the Python parser.
     parser: docspec_python.ParserOptions = dataclasses.field(default_factory=docspec_python.ParserOptions)
 
     #: The encoding to use when reading the Python source files.
-    encoding: t.Optional[str] = None
+    #:
+    #: Changed in 4.7.0: Default changed from `None` (system default encoding) to `"utf-8"`.
+    encoding: str = "utf-8"
 
     def __post_init__(self) -> None:
         self._context: t.Optional[Context] = None
 
     def get_effective_search_path(self) -> t.List[str]:
         if self.search_path is None:
             search_path = [".", "src"] if self.modules is None else list(sys.path)
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/crossref.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/crossref.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/filter.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/filter.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/google.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             if keyword:
                 generate_sections_markdown(lines, {keyword: current_lines})
             else:
                 lines.extend(current_lines)
             current_lines.clear()
 
         for line in node.docstring.content.split("\n"):
-            if line.startswith("```"):
+            if line.lstrip().startswith("```"):
                 in_codeblock = not in_codeblock
                 current_lines.append(line)
                 continue
 
             if in_codeblock:
                 current_lines.append(line)
                 continue
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/pydocmd.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/pydocmd.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/smart.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/smart.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/processors/sphinx.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/processors/sphinx.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     def _process(self, node: docspec.ApiObject) -> None:
         if not node.docstring:
             return
 
         lines = []
         components: t.Dict[str, t.List[str]] = {}
 
-        parsed_docstring = docstring_parser.parse(node.docstring.content, docstring_parser.DocstringStyle.REST)
+        parsed_docstring = docstring_parser.parse(node.docstring.content, docstring_parser.DocstringStyle.AUTO)
         components["Arguments"] = self._convert_params(parsed_docstring.params)
         components["Raises"] = self._convert_raises(parsed_docstring.raises)
         return_doc = self._convert_returns(parsed_docstring.returns)
         if return_doc:
             components["Returns"] = [return_doc]
 
         if parsed_docstring.short_description:
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/docusaurus.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/docusaurus.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 # descend to the file
                 filepath = filepath / module_part
 
             # create intermediary missing directories and get the full path
             filepath.mkdir(parents=True, exist_ok=True)
             filepath = filepath / f"{module_parts[-1]}.md"
 
-            with filepath.open("w") as fp:
+            with filepath.open("w", encoding=self.markdown.encoding) as fp:
                 logger.info("Render file %s", filepath)
                 self.markdown.render_single_page(fp, [module])
 
             # only update the relative module tree if the file is not empty
             relative_module_tree["edges"].append(os.path.splitext(str(filepath.relative_to(self.docs_base_path)))[0])
 
         self._render_side_bar_config(module_tree)
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/hugo.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/hugo.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,15 @@
     os.makedirs(os.path.dirname(to), exist_ok=True)
     with tempfile.TemporaryDirectory() as tempdir:
         path = os.path.join(tempdir, filename)
         with open(path, "wb") as fp:
             shutil.copyfileobj(requests.get(files[filename], stream=True).raw, fp)
         with tarfile.open(path) as archive:
             with open(to, "wb") as fp:
-                shutil.copyfileobj(t.cast(t.IO[bytes], archive.extractfile("hugo")), t.cast(t.IO[bytes], fp))
+                shutil.copyfileobj(t.cast(t.IO[bytes], archive.extractfile("hugo")), t.cast(t.IO[bytes], fp))  # type: ignore[misc]  # See https://github.com/python/mypy/issues/15031  # noqa: E501
 
     chmod.update(to, "+x")
     logger.info('Hugo v%s installed to "%s"', version, to)
 
 
 def get_github_releases(repo: str) -> t.Generator[dict, None, None]:
     """
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/jinja2.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/jinja2.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/markdown.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 from __future__ import annotations
 
 import dataclasses
-import html
 import io
 import sys
 import typing as t
 from pathlib import Path
 
 import docspec
 from docspec_python import format_arglist
@@ -38,14 +37,15 @@
     Resolver,
     ResolverV2,
     SingleObjectRenderer,
     SinglePageRenderer,
     SourceLinker,
 )
 from pydoc_markdown.util.docspec import ApiSuite, format_function_signature, is_method
+from pydoc_markdown.util.misc import escape_except_blockquotes
 
 
 def dotted_name(obj: docspec.ApiObject) -> str:
     return ".".join(x.name for x in obj.path)
 
 
 @dataclasses.dataclass
@@ -365,15 +365,19 @@
         self._render_signature_block(fp, obj)
 
         if render_view_source:
             if source_string and self.source_position == "after signature":
                 fp.write(source_string + "\n\n")
 
         if obj.docstring:
-            docstring = html.escape(obj.docstring.content) if self.escape_html_in_docstring else obj.docstring.content
+            docstring = (
+                escape_except_blockquotes(obj.docstring.content)
+                if self.escape_html_in_docstring
+                else obj.docstring.content
+            )
             lines = docstring.split("\n")
             if self.docstrings_as_blockquote:
                 lines = ["> " + x for x in lines]
             fp.write("\n".join(lines))
             fp.write("\n\n")
 
     def _render_recursive(self, fp: t.TextIO, level: int, obj: docspec.ApiObject):
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/renderers/mkdocs.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/renderers/mkdocs.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/contrib/source_linkers/git.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/contrib/source_linkers/git.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/interfaces.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/interfaces.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/main.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/main.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/novella/preprocessor.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/novella/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/static.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/static.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/util/docspec.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/util/docspec.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/util/knownfiles.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/util/knownfiles.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/util/pages.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/util/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,11 +171,11 @@
         with open(filename, "w") as fp:
             if write_prefix:
                 write_prefix(fp)
             if self.source:
                 src_path = os.path.join(context_directory, self.source)
                 logger.info('Writing "%s" (source: "%s")', filename, src_path)
                 with open(src_path, "rb") as src:
-                    shutil.copyfileobj(src, fp.buffer)
+                    shutil.copyfileobj(src, fp.buffer)  # type: ignore[misc]  # See https://github.com/python/mypy/issues/15031  # noqa: E501
             else:
                 logger.info('Rendering "%s"', filename)
                 renderer.render_single_page(fp, self.filtered_modules(modules), self.title)
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/util/watchdog.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/util/watchdog.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import logging
 import os
 import threading
 from typing import List, Tuple
 
 from watchdog.events import FileSystemEventHandler  # type: ignore
 from watchdog.observers import Observer  # type: ignore
+from watchdog.observers.api import BaseObserver  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 
 class _CallbackEventHandler(FileSystemEventHandler):
     def __init__(self, callback, filter_paths=None):
         self._callback = callback
@@ -39,15 +40,15 @@
 
     def on_any_event(self, event):
         if self._filter_paths and event.src_path not in self._filter_paths:
             return
         self._callback(event)
 
 
-def watch_paths(paths: List[str], recursive: bool = False) -> Tuple[Observer, threading.Event]:
+def watch_paths(paths: List[str], recursive: bool = False) -> Tuple[BaseObserver, threading.Event]:
     """Creates an observer for the specified *paths* and returns it together
     with a #threading.Event object. The event will be set when event occurred.
     """
 
     paths = [os.path.abspath(os.path.normpath(x)) for x in paths]
     directories = set(os.path.dirname(x) for x in paths)
```

### Comparing `pydoc_markdown-4.6.4/src/pydoc_markdown/util/ytemplate.py` & `pydoc_markdown-4.6.5/src/pydoc_markdown/util/ytemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         # Inline replacements.
         index = line.find("#@")
         if index > 0:
             line = line[:index] + json.dumps(eval(line[index + 2 :], context, context)) + "\n"
 
         yaml_code.append(line)
 
-    return yaml.load("".join(yaml_code), Loader)
+    return yaml.load("".join(yaml_code), Loader or yaml.Loader)
 
 
 class Attributor:
     def __init__(self, data: Mapping, default: Any = None) -> None:
         self._data = data
         self._default = default
```

### Comparing `pydoc_markdown-4.6.4/PKG-INFO` & `pydoc_markdown-4.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoc-markdown
-Version: 4.6.4
+Version: 4.6.5
 Summary: Create Python API documentation in Markdown format.
 License: MIT
 Keywords: documentation,docs,generator,markdown,pydoc
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,23 +13,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
-Provides-Extra: docs
-Provides-Extra: novella
-Requires-Dist: PyYAML (>=5.3,<6.0)
+Requires-Dist: PyYAML (>=5.0,<7.0)
 Requires-Dist: click (>=7.1,<9.0)
 Requires-Dist: databind (>=1.5.0,<2.0.0)
 Requires-Dist: docspec (>=2.0.0a1,<3.0.0)
 Requires-Dist: docspec-python (>=2.0.0a1,<3.0.0)
 Requires-Dist: docstring-parser (>=0.11,<0.12)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: nr.util (>=0.7.5,<1.0.0)
@@ -37,71 +31,97 @@
 Requires-Dist: tomli (>=2.0.0,<3.0.0)
 Requires-Dist: tomli_w (>=1.0.0,<2.0.0)
 Requires-Dist: watchdog
 Requires-Dist: yapf (>=0.30.0)
 Project-URL: Homepage, https://github.com/NiklasRosenstein/pydoc-markdown
 Description-Content-Type: text/markdown
 
-# Pydoc-Markdown
+# Pydoc-Markdown 📃
 
 ![Python versions](https://img.shields.io/pypi/pyversions/pydoc-markdown?style=for-the-badge)
 [![Pypi version](https://img.shields.io/pypi/v/pydoc-markdown?style=for-the-badge)](https://pypi.org/project/pydoc-markdown/)
-[![Build status](https://img.shields.io/github/workflow/status/NiklasRosenstein/pydoc-markdown/Python%20package?style=for-the-badge)](https://github.com/NiklasRosenstein/pydoc-markdown/actions)
-[![Gitter chat](https://img.shields.io/badge/Chat-On%20Gitter-%2386f4e4?style=for-the-badge)](https://gitter.im/NiklasRosenstein/pydoc-markdown)
 
 Pydoc-Markdown is a tool to create Python API documentation in Markdown format. Instead of executing your Python
-code like so many other documentation tools, it parses it using [docspec][] instead. To run Pydoc-Markdown, you
-need to use at least Python 3.7.
+code like so many other documentation tools, it parses it using [docspec][] instead.
 
-[>> Go to the Documentation][Documentation]
+[→ Go to the Documentation 📘][Documentation]
 
   [contrib]: https://github.com/NiklasRosenstein/pydoc-markdown/blob/develop/.github/CONTRIBUTING.md
   [docspec]: https://niklasrosenstein.github.io/docspec/
   [Documentation]: https://niklasrosenstein.github.io/pydoc-markdown/
   [MkDocs]: https://www.mkdocs.org/
   [Novella]: https://niklasrosenstein.github.io/novella/
   [Novella build backend]: https://niklasrosenstein.github.io/pydoc-markdown/usage/novella/
 
-### Installation
+__Table of Contents__
 
-I recommend to install Pydoc-Markdown using Pipx.
+* [Installation 📦](#installation-)
+* [Features 🌟](#features-)
+* [News 📢](#news-)
+  * [4.7.0 (Undeprecating YAML configuration)](#470-undeprecating-yaml-configuration)
+  * [4.6.0 (Novella integration)](#460-novella-integration)
+* [Contributing to Pydoc-Markdown 🤝](#contributing-to-pydoc-markdown-)
+* [Questions / Need help? 🤔](#questions--need-help-)
+* [Projects using Pydoc-Markdown 📚](#projects-using-pydoc-markdown-)
 
-    $ pipx install novella
-    $ pipx inject novella pydoc-markdown[novella]
+### Installation 📦
 
-If you need access to the Pydoc-Markdown CLI instead, because you rely on the "old-style" pre-4.6.0
-YAML configuration, you should install the package directly through Pipx.
+You can install Pydoc-Markdown using Pipx:
 
     $ pipx install pydoc-markdown
 
-> Note: You can also use `pipx install pydoc-markdown[novella] --include-deps`, but be aware that this
-> also adds other programs in Pydoc-Markdown's dependency tree to your PATH.
+If you plan on using the [Novella][] integration, you may want to install it as:
+
+    $ pipx install novella
+    $ pipx inject novella pydoc-markdown[novella]
+
+You need at least Python 3.7 to run Pydoc-Markdown. The Python version compatibility of the package you are looking to
+generate documentation for is irrelevant.
 
-### Features
+### Features 🌟
 
 * Understands multiple documentation styles (Sphinx, Google, Pydoc-Markdown specific) and converts them to properly
   formatted Markdown
 * Can parse docstrings for variables thanks to [docspec][] (`#:` block before or string literal after the statement)
 * Generates links to other API objects per the documentation syntax (e.g. `#OtherClass` for the Pydoc-Markdown style)
+* Configure the output using a YAML file or `pyProject.toml`, then you're only one command away to generate the
+  documentation in Markdown format
+* Or use [Novella][] to tightly integrate with static site generators like MkDocs and Hugo with with additional
+  features such as Markdown pre-processing
+
+### News 📢
+
+#### 4.7.0 (Undeprecating YAML configuration)
 
-### News
+Many users prefer the YAML configuration over the using [Novella][], which is why starting with __4.7.0__, the YAML
+style configuration is officially un-deprecated and will continue to be supported.
+
+#### 4.6.0 (Novella integration)
 
 Starting with __4.6.0__, development focuses on integrating with [Novella][] and use it as a replacement for
 tool-specific renderers thus far provided directly by Pydoc-Markdown (i.e. integrations with MkDocs, Hugo and
 Docusuraus). Such integrations are/will be provided by Novella instead.
 
 With the Novella integration, you can now place generated API content in Markdown format inline with your
 existing Markdown documentation source files using `@pydoc` tags. Check out the [Documentation][] for more
 information on how to use Pydoc-Markdown with Novella.
 
 The old style of using Pydoc-Markdown with a YAML or PyProject configuration to generate files and kick off the
 build is now deprecated but will be maintained for the foreseeable future (at least until the next major version
 bump). It is strongly recommended to migrate your existing projects to using the Novella build backend.
 
-### Contributing to Pydoc-Markdown
+### Contributing to Pydoc-Markdown 🤝
 
 All contributions are welcome! Check out the [Contribution Guidelines][contrib].
 
-### Questions / Need help?
+### Questions / Need help? 🤔
 
 Feel free to open a topic on [GitHub Discussions](https://github.com/NiklasRosenstein/pydoc-markdown/discussions)!
 
+### Projects using Pydoc-Markdown 📚
+
+An incomplete list of projects that use Pydoc-Markdown to generate their API documentation. Feel free to open a
+pull request to add your project to this list!
+
+* [tensorchord/envd](https://envd.tensorchord.ai/api/starlark/v0/config.html)
+* [tqdm](https://tqdm.github.io/)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

