# Comparing `tmp/pydoc_markdown-4.7.0.tar.gz` & `tmp/pydoc_markdown-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoc_markdown-4.7.0.tar", max compression
+gzip compressed data, was "pydoc_markdown-4.8.0.tar", max compression
```

## Comparing `pydoc_markdown-4.7.0.tar` & `pydoc_markdown-4.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.7.0/LICENSE
--rw-r--r--   0        0        0     4015 2023-05-28 02:49:02.897967 pydoc_markdown-4.7.0/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.7.0/readme.md
--rw-r--r--   0        0        0     8120 2023-05-28 02:49:02.921966 pydoc_markdown-4.7.0/src/pydoc_markdown/__init__.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/__init__.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/__init__.py
--rw-r--r--   0        0        0     5722 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/python.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/__init__.py
--rw-r--r--   0        0        0     5520 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/crossref.py
--rw-r--r--   0        0        0     3954 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/filter.py
--rw-r--r--   0        0        0     5971 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/google.py
--rw-r--r--   0        0        0     3875 2023-05-27 21:47:48.827975 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/pydocmd.py
--rw-r--r--   0        0        0     2740 2023-05-27 21:47:48.827975 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/smart.py
--rw-r--r--   0        0        0     5622 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/sphinx.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/__init__.py
--rw-r--r--   0        0        0     6850 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/docusaurus.py
--rw-r--r--   0        0        0    16915 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/hugo.py
--rw-r--r--   0        0        0     3949 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/jinja2.py
--rw-r--r--   0        0        0    22501 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/markdown.py
--rw-r--r--   0        0        0     7918 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/mkdocs.py
--rw-r--r--   0        0        0       81 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/__init__.py
--rw-r--r--   0        0        0     6647 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/git.py
--rw-r--r--   0        0        0     7220 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/interfaces.py
--rw-r--r--   0        0        0    13822 2023-05-28 00:17:51.716178 pydoc_markdown-4.7.0/src/pydoc_markdown/main.py
--rw-r--r--   0        0        0     6467 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/novella/preprocessor.py
--rw-r--r--   0        0        0        0 2022-11-12 22:49:35.857142 pydoc_markdown-4.7.0/src/pydoc_markdown/py.typed
--rw-r--r--   0        0        0     3375 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/static.py
--rw-r--r--   0        0        0        5 2022-11-12 22:49:35.857142 pydoc_markdown-4.7.0/src/pydoc_markdown/util/__init__.py
--rw-r--r--   0        0        0     4013 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/util/docspec.py
--rw-r--r--   0        0        0     4545 2022-11-21 08:38:49.340005 pydoc_markdown-4.7.0/src/pydoc_markdown/util/knownfiles.py
--rw-r--r--   0        0        0      930 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc.py
--rw-r--r--   0        0        0      378 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc_test.py
--rw-r--r--   0        0        0     6851 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/pages.py
--rw-r--r--   0        0        0     2492 2023-05-27 23:49:43.440168 pydoc_markdown-4.7.0/src/pydoc_markdown/util/watchdog.py
--rw-r--r--   0        0        0     2999 2023-05-27 21:46:22.746425 pydoc_markdown-4.7.0/src/pydoc_markdown/util/ytemplate.py
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pydoc_markdown-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1002 2022-11-12 22:49:35.853142 pydoc_markdown-4.8.0/LICENSE
+-rw-r--r--   0        0        0     4037 2023-05-28 19:40:12.890883 pydoc_markdown-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-05-28 00:16:10.151072 pydoc_markdown-4.8.0/readme.md
+-rw-r--r--   0        0        0     8446 2023-05-28 19:40:12.898883 pydoc_markdown-4.8.0/src/pydoc_markdown/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/__init__.py
+-rw-r--r--   0        0        0     5722 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/python.py
+-rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/__init__.py
+-rw-r--r--   0        0        0     5520 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/crossref.py
+-rw-r--r--   0        0        0     3954 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/filter.py
+-rw-r--r--   0        0        0     5971 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/google.py
+-rw-r--r--   0        0        0     3875 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/pydocmd.py
+-rw-r--r--   0        0        0     2740 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/smart.py
+-rw-r--r--   0        0        0     5622 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/sphinx.py
+-rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/__init__.py
+-rw-r--r--   0        0        0     6840 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/docusaurus.py
+-rw-r--r--   0        0        0    16957 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/hugo.py
+-rw-r--r--   0        0        0     3947 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/jinja2.py
+-rw-r--r--   0        0        0    22500 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/markdown.py
+-rw-r--r--   0        0        0     7848 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/mkdocs.py
+-rw-r--r--   0        0        0       81 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/__init__.py
+-rw-r--r--   0        0        0     6636 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/git.py
+-rw-r--r--   0        0        0     7085 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/interfaces.py
+-rw-r--r--   0        0        0    13878 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/main.py
+-rw-r--r--   0        0        0     6467 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/novella/preprocessor.py
+-rw-r--r--   0        0        0        0 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/py.typed
+-rw-r--r--   0        0        0     3375 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/static.py
+-rw-r--r--   0        0        0        5 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/__init__.py
+-rw-r--r--   0        0        0     4013 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/docspec.py
+-rw-r--r--   0        0        0     4545 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/knownfiles.py
+-rw-r--r--   0        0        0      930 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc.py
+-rw-r--r--   0        0        0      378 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc_test.py
+-rw-r--r--   0        0        0     6851 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/pages.py
+-rw-r--r--   0        0        0     2492 2023-05-28 11:03:30.810663 pydoc_markdown-4.8.0/src/pydoc_markdown/util/watchdog.py
+-rw-r--r--   0        0        0     2998 2023-05-28 19:28:10.391528 pydoc_markdown-4.8.0/src/pydoc_markdown/util/ytemplate.py
+-rw-r--r--   0        0        0     5787 1970-01-01 00:00:00.000000 pydoc_markdown-4.8.0/PKG-INFO
```

### Comparing `pydoc_markdown-4.7.0/LICENSE` & `pydoc_markdown-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/pyproject.toml` & `pydoc_markdown-4.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoc-markdown"
-version = "4.7.0"
+version = "4.8.0"
 description = "Create Python API documentation in Markdown format."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "pydoc_markdown", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -22,17 +22,18 @@
 
 [tool.poetry.urls]
 Homepage = "https://github.com/NiklasRosenstein/pydoc-markdown"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=7.1,<9.0"
-"databind" = "^1.5.0"
-docspec = "^2.0.0a1"
-docspec-python = "^2.0.0a1"
+"databind.core" = "^4.3.0"
+"databind.json" = "^4.3.0"
+docspec = "^2.2.1"
+docspec-python = "^2.2.1"
 docstring-parser = "^0.11"
 "nr.util" = ">=0.7.5,<1.0.0"
 jinja2 = "^3.0.0"
 requests = "^2.23.0"
 PyYAML = ">=5.0,<7.0"
 tomli = "^2.0.0"
 tomli_w = "^1.0.0"
@@ -43,15 +44,15 @@
 pytest = "*"
 pytest-coverage = "*"
 mypy = "*"
 types-deprecated = "*"
 types-requests = "*"
 types-PyYAML = "*"
 isort = "^5.10.1"
-black = "^22.3.0"
+black = "*"
 
 [tool.poetry.group.novella]
 optional = true
 
 [tool.poetry.group.novella.dependencies]
 novella = { version = " >=0.1.10,<0.3.0" }
```

### Comparing `pydoc_markdown-4.7.0/readme.md` & `pydoc_markdown-4.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/__init__.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 import dataclasses
 import logging
 import os
 import subprocess
 import typing as t
 from pathlib import Path
 
-import databind.core.annotations as A
 import databind.json
 import docspec
 import tomli
+from databind.core import Context as DatabindContext, ExtraKeys, Location, format_context_trace
 
 from pydoc_markdown.contrib.loaders.python import PythonLoader
 from pydoc_markdown.contrib.processors.crossref import CrossrefProcessor
 from pydoc_markdown.contrib.processors.filter import FilterProcessor
 from pydoc_markdown.contrib.processors.smart import SmartProcessor
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Loader, Processor, Renderer, Resolver
 from pydoc_markdown.util import ytemplate
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "4.7.0"
+__version__ = "4.8.0"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Hooks:
     pre_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "pre-render"})
@@ -76,15 +76,15 @@
     renderer: Renderer = dataclasses.field(default_factory=MarkdownRenderer)
 
     #: Hooks that can be executed at certain points in the pipeline. The commands
     #: are executed with the current `SHELL`.
     hooks: Hooks = dataclasses.field(default_factory=Hooks)
 
     # Hidden fields are filled at a later point in time and are not (de-) serialized.
-    unknown_fields: t.List[str] = dataclasses.field(default_factory=list)
+    unknown_fields: t.List[str] = dataclasses.field(default_factory=list, init=False)
 
     def __post_init__(self) -> None:
         self.resolver: t.Optional[Resolver] = None
         self._context: t.Optional[Context] = None
 
     def load_config(self, arg: t.Union[str, dict]) -> None:
         """
@@ -105,21 +105,31 @@
             else:
                 data = ytemplate.load(filename, {"env": ytemplate.Attributor(os.environ)})
             if filename == "pyproject.toml":
                 data = data["tool"]["pydoc-markdown"]
         else:
             data = arg
 
-        unknown_keys = A.collect_unknowns()
-        result = databind.json.new_mapper().deserialize(data, type(self), filename=filename, settings=[unknown_keys()])  # type: ignore[arg-type]  # noqa: E501  # Bad databind typehint
+        unknown_keys: t.List[t.Tuple[DatabindContext, t.Set[str]]] = []
+        result = databind.json.load(
+            data,
+            type(self),
+            filename=filename,
+            settings=[
+                ExtraKeys(
+                    allow=True,
+                    recorder=lambda ctx, extra_keys: unknown_keys.append((ctx, extra_keys)),
+                )
+            ],
+        )  # type: ignore[arg-type]  # noqa: E501  # Bad databind typehint
         vars(self).update(vars(result))
 
-        for loc, keys in unknown_keys:
-            for key in keys:
-                self.unknown_fields.append(str(loc.push_unknown(key).format()))
+        for ctx, keys in unknown_keys:
+            prefix = f'Unknown key(s) "{keys}" at:\n'
+            self.unknown_fields.append(prefix + format_context_trace(ctx))
 
     def init(self, context: Context) -> None:
         """
         Initialize all plugins with the specified *context*. Cannot be called multiple times.
         If omitted, the plugins will be initialized with a default context before the load,
         process or render phase.
         """
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/loaders/python.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/loaders/python.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/crossref.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/crossref.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/filter.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/filter.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/google.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/google.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/pydocmd.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/pydocmd.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/smart.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/smart.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/processors/sphinx.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/processors/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/docusaurus.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/docusaurus.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import dataclasses
 import json
 import logging
 import os
 import typing as t
 from pathlib import Path
 
-import databind.core.annotations as A
 import docspec
 import typing_extensions as te
+from databind.core import DeserializeAs
 
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Context, Renderer
 
 logger = logging.getLogger(__name__)
 
 
@@ -45,15 +45,15 @@
     [1]: https://v2.docusaurus.io/
     [2]: https://github.com/NiklasRosenstein/pydoc-markdown/tree/develop/examples/docusaurus
 
     ### Options
     """
 
     #: The #MarkdownRenderer configuration.
-    markdown: te.Annotated[MarkdownRenderer, A.typeinfo(deserialize_as=CustomizedMarkdownRenderer)] = dataclasses.field(
+    markdown: te.Annotated[MarkdownRenderer, DeserializeAs(CustomizedMarkdownRenderer)] = dataclasses.field(
         default_factory=CustomizedMarkdownRenderer
     )
 
     #: The path where the docusaurus docs content is. Defaults "docs" folder.
     docs_base_path: str = "docs"
 
     #: The output path inside the docs_base_path folder, used to output the
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/hugo.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/hugo.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 import subprocess
 import sys
 import tarfile
 import tempfile
 import typing as t
 from urllib.parse import urljoin, urlparse
 
-import databind.core.annotations as A
 import docspec
 import requests
 import tomli_w
 import typing_extensions as te
 import yaml
+from databind.core import Remainder
 from nr.util.fs import chmod
 
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Renderer, Resolver, Server
 from pydoc_markdown.util.knownfiles import KnownFiles
 from pydoc_markdown.util.pages import Page, Pages
 
@@ -151,17 +151,16 @@
 
     #: Language code. Default: `en-us`
     languageCode: t.Optional[str] = "en-us"
 
     #: This field collects all remaining options that do not match any of the above
     #: and will be forwarded directly into the Hugo `config.yaml` when it is rendered
     #: into the build directory.
-    additional_options: te.Annotated[t.Dict[str, t.Any], A.fieldinfo(flat=True)] = dataclasses.field(
-        default_factory=dict
-    )
+    # TODO(@NiklasRosenstein): Test if this still works as expected.
+    additional_options: te.Annotated[t.Dict[str, t.Any], Remainder()] = dataclasses.field(default_factory=dict)
 
     def to_toml(self, fp: t.TextIO) -> None:
         data = self.additional_options.copy()
         for field in dataclasses.fields(self):
             if field.name in ("additional_options", "theme", "serverURL", "serverPort"):
                 continue
             value = getattr(self, field.name)
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/jinja2.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/jinja2.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,26 @@
                 if m.name in args["modules"] or any(fnmatch.fnmatch(m.name, x) for x in args["modules"])
             ]
         return args
 
 
 @D.dataclass
 class RenderBlock:
-
     #: The path to the Jinja2 template that is used to render the output files.
     template: str
 
     #: A mapping for filename (without suffix) to a list of Module selectors.
     produces: t.Dict[str, Args]
 
     #: Settings for the Jinja2 Environment.
     jinja2_environment_settings: t.Dict[str, t.Any] = D.field(default_factory=dict)
 
 
 @D.dataclass
 class Jinja2Renderer(Renderer):
-
     #: Render instructions.
     renders: t.List[RenderBlock]
 
     #: Build directory where all the files are produced.
     build_directory: str = "build/docs"
 
     def render(self, modules: t.List[docspec.Module]) -> None:
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/markdown.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,14 @@
         if self.source_linker:
             self.source_linker.init(context)
         self._context = context
 
 
 @dataclasses.dataclass
 class MarkdownReferenceResolver(Resolver, ResolverV2):
-
     local: bool = True
     global_: bool = False
 
     def generate_object_id(self, obj: docspec.ApiObject) -> str:
         return ".".join(o.name for o in obj.path)
 
     def _resolve_reference_in_members(
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/renderers/mkdocs.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/renderers/mkdocs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 import dataclasses
 import logging
 import os
 import subprocess
 import typing as t
 from typing import Dict, List, Optional
 
-import databind.core.annotations as A
 import docspec
 import typing_extensions as te
 import yaml
+from databind.core import DeserializeAs
 
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Renderer, Resolver, Server
 from pydoc_markdown.util.knownfiles import KnownFiles
 from pydoc_markdown.util.pages import Page, Pages
 
 logger = logging.getLogger(__name__)
@@ -86,16 +86,15 @@
     clean_render: bool = True
 
     #: The pages to render into the output directory.
     # TODO (@NiklasRosenstein): Uh what exactly is this in new databind?
     pages: Pages[Page] = dataclasses.field(default_factory=Pages)
 
     #: Markdown renderer settings.
-    # TODO (@NiklasRosenstein): Use fieldinfo(serialize_as)
-    markdown: te.Annotated[MarkdownRenderer, A.typeinfo(deserialize_as=CustomizedMarkdownRenderer)] = dataclasses.field(
+    markdown: te.Annotated[MarkdownRenderer, DeserializeAs(CustomizedMarkdownRenderer)] = dataclasses.field(
         default_factory=CustomizedMarkdownRenderer
     )
 
     #: The name of the site. This will be carried into the `site_name` key
     #: of the #mkdocs_config.
     site_name: t.Optional[str] = None
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/contrib/source_linkers/git.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/contrib/source_linkers/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # IN THE SOFTWARE.
 
 import logging
 import os
 import typing as t
 from pathlib import Path
 
-import databind.core.dataclasses as dataclasses
 import docspec
+from databind.core import dataclasses
 from nr.util.git import Git, NoCurrentBranchError
 
 from pydoc_markdown.interfaces import Context, SourceLinker
 
 logger = logging.getLogger(__name__)
 
 
@@ -121,15 +121,14 @@
         logger.debug("project_root = %r", self._project_root)
         logger.debug("sha = %r", self._sha)
         logger.debug("branch = %r", self._branch)
 
 
 @dataclasses.dataclass
 class BaseGitServiceSourceLinker(BaseGitSourceLinker):
-
     #: The repository name, formatted as `owner/repo`.
     repo: str
 
     #: The host name of the Git service.
     host: str
 
     def get_context_vars(self) -> t.Dict[str, str]:
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/interfaces.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 import abc
 import subprocess
 import typing as t
 
 import docspec
-from databind.core import annotations as A
+from databind.core import Union
 
 if t.TYPE_CHECKING:
     from pydoc_markdown.util.docspec import ApiSuite
 
 
 class Context:
     """
@@ -46,19 +46,21 @@
 
 
 class PluginBase(abc.ABC):
     def init(self, context: Context) -> None:
         pass
 
 
-@A.unionclass(
-    A.unionclass.Subtypes.chain(
-        A.unionclass.Subtypes.entrypoint("pydoc_markdown.interfaces.Loader"), A.unionclass.Subtypes.import_()
-    ),
-    style=A.unionclass.Style.flat,
+# TODO(@NiklasRosenstein): Test that this works as expected.
+@Union(
+    [
+        "!pydoc_markdown.interfaces.Loader",
+        "<import>",
+    ],
+    style=Union.FLAT,
 )
 class Loader(PluginBase):
     """
     This interface describes an object that is capable of loading documentation
     data. The location from which the documentation is loaded must be defined
     with the configuration class.
     """
@@ -89,37 +91,41 @@
     """
 
     @abc.abstractmethod
     def resolve_reference(self, suite: "ApiSuite", scope: docspec.ApiObject, ref: str) -> t.Optional[docspec.ApiObject]:
         ...
 
 
-@A.unionclass(
-    A.unionclass.Subtypes.chain(
-        A.unionclass.Subtypes.entrypoint("pydoc_markdown.interfaces.Processor"), A.unionclass.Subtypes.import_()
-    ),
-    style=A.unionclass.Style.flat,
+# TODO(@NiklasRosenstein): Test that this works as expected.
+@Union(
+    [
+        "!pydoc_markdown.interfaces.Processor",
+        "<import>",
+    ],
+    style=Union.FLAT,
 )
 class Processor(PluginBase):
     """
     A processor is an object that takes a list of #docspec.Module#s as an input and
     transforms it in an arbitrary way. This usually processes docstrings to convert from
     various documentation syntaxes to plain Markdown.
     """
 
     @abc.abstractmethod
     def process(self, modules: t.List[docspec.Module], resolver: t.Optional[Resolver]) -> None:
         ...
 
 
-@A.unionclass(
-    A.unionclass.Subtypes.chain(
-        A.unionclass.Subtypes.entrypoint("pydoc_markdown.interfaces.Renderer"), A.unionclass.Subtypes.import_()
-    ),
-    style=A.unionclass.Style.flat,
+# TODO(@NiklasRosenstein): Test that this works as expected.
+@Union(
+    [
+        "!pydoc_markdown.interfaces.Renderer",
+        "<import>",
+    ],
+    style=Union.FLAT,
 )
 class Renderer(PluginBase):
     """
     A renderer is an object that takes a list of #docspec.Module#s as an input and produces
     output files or writes to stdout. It may also expose additional command-line arguments.
     There can only be one renderer at the end of the processor chain.
 
@@ -200,19 +206,21 @@
     def build(self, site_dir: str) -> None:
         """
         Invoke the build. The *site_dir* is the directory in which the output files should be
         placed. Otherwise, the directory may be determined by the builder.
         """
 
 
-@A.unionclass(
-    A.unionclass.Subtypes.chain(
-        A.unionclass.Subtypes.entrypoint("pydoc_markdown.interfaces.SourceLinker"), A.unionclass.Subtypes.import_()
-    ),
-    style=A.unionclass.Style.flat,
+# TODO(@NiklasRosenstein): Test that this works as expected.
+@Union(
+    [
+        "!pydoc_markdown.interfaces.SourceLinker",
+        "<import>",
+    ],
+    style=Union.FLAT,
 )
 class SourceLinker(PluginBase):
     """
     This interface is used to determine the URL to the source of an API object. Renderers
     can use it to place a link to the source in the generated documentation.
     """
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/main.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 import sys
 import typing as t
 import webbrowser
 from pathlib import Path
 
 import click
 import yaml
-from databind.core import ConcreteType, dataclass_to_schema
+from databind.core import convert_dataclass_to_schema
 from docspec import dump_module
+from typeapi import ClassTypeHint
 
 from pydoc_markdown import PydocMarkdown, __version__, static
 from pydoc_markdown.contrib.loaders.python import PythonLoader
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Context, Server
 from pydoc_markdown.util.watchdog import watch_paths
 
@@ -91,17 +92,17 @@
             if self.search_path:
                 loader.search_path = self.search_path
             if self.py2 is not None:
                 loader.parser.print_function = not self.py2
 
         if self.render_toc is not None:
             # Find the #MarkdownRenderer field for this renderer.
-            for field in dataclass_to_schema(type(config.renderer)).fields.values():
-                if isinstance(field.type, ConcreteType) and field.type.type == MarkdownRenderer:
-                    markdown: MarkdownRenderer = getattr(config.renderer, field.name)
+            for field_name, field in convert_dataclass_to_schema(type(config.renderer)).fields.items():
+                if isinstance(field.datatype, ClassTypeHint) and field.datatype.type == MarkdownRenderer:
+                    markdown: MarkdownRenderer = getattr(config.renderer, field_name)
                     break
             else:
                 if isinstance(config.renderer, MarkdownRenderer):
                     markdown = config.renderer
                 else:
                     error("renderer {!r} does not expose a MarkdownRenderer".format(type(config.renderer).__name__))
             markdown.render_toc = self.render_toc
```

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/novella/preprocessor.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/novella/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/static.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/static.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/docspec.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/docspec.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/knownfiles.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/knownfiles.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/misc.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/misc.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/pages.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/pages.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/watchdog.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/watchdog.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.7.0/src/pydoc_markdown/util/ytemplate.py` & `pydoc_markdown-4.8.0/src/pydoc_markdown/util/ytemplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
     if Loader is None:
         Loader = yaml.SafeLoader  # type: ignore
 
     yaml_code = []
     it = iter(file_)
     for line in it:
-
         # Parse Python code blocks.
         if line.startswith("#@"):
             block_lines = [line[2:]]
             for line in it:
                 if not line.startswith("#@"):
                     raise ValueError("missing #@ end")
                 if line[2:].strip() == "end":
```

### Comparing `pydoc_markdown-4.7.0/PKG-INFO` & `pydoc_markdown-4.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoc-markdown
-Version: 4.7.0
+Version: 4.8.0
 Summary: Create Python API documentation in Markdown format.
 License: MIT
 Keywords: documentation,docs,generator,markdown,pydoc
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -17,17 +17,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=5.0,<7.0)
 Requires-Dist: click (>=7.1,<9.0)
-Requires-Dist: databind (>=1.5.0,<2.0.0)
-Requires-Dist: docspec (>=2.0.0a1,<3.0.0)
-Requires-Dist: docspec-python (>=2.0.0a1,<3.0.0)
+Requires-Dist: databind.core (>=4.3.0,<5.0.0)
+Requires-Dist: databind.json (>=4.3.0,<5.0.0)
+Requires-Dist: docspec (>=2.2.1,<3.0.0)
+Requires-Dist: docspec-python (>=2.2.1,<3.0.0)
 Requires-Dist: docstring-parser (>=0.11,<0.12)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: nr.util (>=0.7.5,<1.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.0,<3.0.0)
 Requires-Dist: tomli_w (>=1.0.0,<2.0.0)
 Requires-Dist: watchdog
```

