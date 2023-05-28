# Comparing `tmp/rico-0.0.5.tar.gz` & `tmp/rico-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.0.5.tar", last modified: Sun May 21 09:50:45 2023, max compression
+gzip compressed data, was "rico-0.0.6.tar", last modified: Sun May 28 13:40:17 2023, max compression
```

## Comparing `rico-0.0.5.tar` & `rico-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-21 09:50:12.834578 rico-0.0.5/LICENSE
--rw-r--r--   0        0        0      715 2023-05-21 09:50:12.834578 rico-0.0.5/README.md
--rw-r--r--   0        0        0     2937 2023-05-21 09:50:45.610880 rico-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      391 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/__init__.py
--rw-r--r--   0        0        0      340 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/_version.py
--rw-r--r--   0        0        0    10646 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/content.py
--rw-r--r--   0        0        0     6861 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/html.py
--rw-r--r--   0        0        0       18 2023-05-21 09:50:12.834578 rico-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0    11383 2023-05-21 09:50:12.834578 rico-0.0.5/tests/test_content.py
--rw-r--r--   0        0        0     8843 2023-05-21 09:50:12.834578 rico-0.0.5/tests/test_html.py
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 rico-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-28 13:39:52.898590 rico-0.0.6/LICENSE
+-rw-r--r--   0        0        0      715 2023-05-28 13:39:52.898590 rico-0.0.6/README.md
+-rw-r--r--   0        0        0     2818 2023-05-28 13:40:17.066776 rico-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      454 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/__init__.py
+-rw-r--r--   0        0        0     2166 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_config.py
+-rw-r--r--   0        0        0    14582 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_content.py
+-rw-r--r--   0        0        0     7012 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-05-28 13:39:52.898590 rico-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__config.py
+-rw-r--r--   0        0        0    17176 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__content.py
+-rw-r--r--   0        0        0     9491 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__version.py
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 rico-0.0.6/PKG-INFO
```

### Comparing `rico-0.0.5/LICENSE` & `rico-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.0.5/README.md` & `rico-0.0.6/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # rico
 Rich content to HTML as easy as Doc([df, plot]).
 
 <br>
 
-[![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
-[![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
-[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
+[![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
+[![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
+[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
```

### Comparing `rico-0.0.5/pyproject.toml` & `rico-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 
@@ -56,25 +56,23 @@
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 lint = [
     "ruff",
     "pyright",
-    "isort",
 ]
 test = [
     "pytest",
     "coverage[toml]",
 ]
 
 [tool.pdm.scripts]
 test = "coverage run -m pytest"
 lint = "ruff check ."
-sort = "isort --check --diff ."
 type = "pyright"
 
 [tool.pdm.build]
 package-dir = "src"
 
 [tool.pdm.version]
 source = "scm"
@@ -88,24 +86,18 @@
 [tool.coverage.run]
 source = [
     "src/rico",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
-    "import",
+    "if TYPE_CHECKING:",
     "pragma: no cover",
 ]
 
-[tool.isort]
-force_sort_within_sections = true
-include_trailing_comma = true
-lines_after_imports = 2
-multi_line_output = 3
-
 [tool.pyright]
 typeCheckingMode = "strict"
 reportIncompatibleMethodOverride = false
 reportMissingTypeStubs = false
 
 [tool.ruff]
 select = [
@@ -145,27 +137,31 @@
     "ANN102",
     "ANN204",
     "ANN401",
     "B006",
     "N817",
     "PGH003",
     "PT001",
+    "PT011",
     "SLF001",
     "TRY003",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = [
     "ANN201",
     "D100",
     "D103",
     "PLR2004",
 ]
 
 [tool.ruff.isort]
+classes = [
+    "HTML",
+]
 force-sort-within-sections = true
 lines-after-imports = 2
 known-local-folder = [
     "rico",
 ]
 
 [tool.ruff.pydocstyle]
```

### Comparing `rico-0.0.5/src/rico/content.py` & `rico-0.0.6/src/rico/_content.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 """Rich content classes."""
 
 from __future__ import annotations
 
 import base64
 import io
 from typing import TYPE_CHECKING
+import urllib.request
 import xml.etree.ElementTree as ET
 
-import rico.html
+import rico._config
+import rico._html
 
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
 
 try:
     import altair as alt
     import vl_convert as vlc
-except ImportError:  # pragma: no cover
+except ImportError:
     alt = None
 
 try:
     import markdown
-except ImportError:  # pragma: no cover
+except ImportError:
     markdown = None
 
 try:
     import matplotlib.pyplot as plt
-except ImportError:  # pragma: no cover
+except ImportError:
     plt = None
 
 try:
     import seaborn.objects as so
-except ImportError:  # pragma: no cover
+except ImportError:
     so = None
 
 
 class ContentBase:
     """A base content definition.
 
     Creates a container element on init.
@@ -53,28 +55,34 @@
 
         Args:
             class_: The container element's class attribute.
         """
         attrib = {"class": class_} if class_ is not None else {}
         self.container = ET.Element("div", attrib=attrib)
 
-    def serialize(self, indent_space: str | None = None, strip: bool = False) -> str:
+    def serialize(
+        self,
+        indent: bool | None = None,
+        space: str | None = None,
+        strip: bool | None = None,
+    ) -> str:
         """Serialize the object to string in HTML format.
 
         Indent the object if `indent_space` is not None.
 
         Args:
-            indent_space: The whitespace for indentation.
+            indent: If True, indent the element.
+            space: The whitespace for indentation.
             strip: If True, strip unnecessary whitespace.
 
         Returns:
             The serialized object.
         """
-        return rico.html.serialize_html(
-            self.container, indent_space=indent_space, strip=strip)
+        return rico._html.serialize_html(
+            self.container, indent=indent, space=space, strip=strip)
 
     def __str__(self) -> str:
         """Serialize the object to string in HTML format."""
         return self.serialize()
 
 
 class Tag(ContentBase):
@@ -188,15 +196,15 @@
         Args:
             text: The HTML text.
             strip_dataframe_borders: Delete borders attributes from dataframes.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
-        for element in rico.html.parse_html(text):
+        for element in rico._html.parse_html(text):
             self.container.append(element)
 
         if strip_dataframe_borders:
             for table in self.container.iterfind(
                 './/table[@class="dataframe"][@border]',
             ):
                 del table.attrib["border"]
@@ -220,45 +228,48 @@
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to the `markdown.markdown` function.
 
         Raises:
             ImportError: The markdown package is not installed.
         """
         if markdown is None:
-            raise ImportError("The markdown package is not installed.")  # pragma: no cover  # noqa: E501
+            raise ImportError("The markdown package is not installed.")
 
         content = HTML(markdown.markdown(text, **kwargs), class_=class_)
         self.container = content.container
 
 
 class Image(ContentBase):
     """An Image content definition.
 
     Creates content elements using an image data and appends them to the container.
     """
     def __init__(
         self,
         data: bytes | str,
-        format: str,  # noqa: A002
+        format: str | None = None,  # noqa: A002
         class_: str | None = None,
     ):
         """Initialize content using image data.
 
         Args:
             data: The image data.
             format: The image format.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
+        if format is None:
+            format = rico._config.get_config("image_format")  # noqa: A001
+
         if format == "svg":
             if isinstance(data, bytes):
                 data = data.decode()
 
-            for element in rico.html.parse_html(data):
+            for element in rico._html.parse_html(data):
                 self.container.append(element)
         else:
             if isinstance(data, str):
                 data = data.encode()
             encoded_image = base64.b64encode(data).decode()
 
             element = ET.Element(
@@ -277,15 +288,15 @@
     - Altair Chart,
     - Pyplot Axes and Figure,
     - Seaborn Plot (seaborn.objects interface).
     """
     def __init__(
         self,
         obj: Any,
-        format: Literal["svg", "png"] = "svg",  # noqa: A002
+        format: Literal["svg", "png"] | None = None,  # noqa: A002
         class_: str | None = None,
         **kwargs: Any,
     ):
         """Initialize content from a chart object.
 
         Args:
             obj: The chart object.
@@ -294,41 +305,48 @@
             **kwargs: Keyword arguments passed to a function
                 which converts object to an image.
 
         Raises:
             TypeError: Chart type is not supported
                 or required extra package is not installed.
         """
+        if format is None:
+            format = rico._config.get_config("chart_format")  # noqa: A001
+
         if plt is not None and isinstance(obj, plt.Axes):
             obj = obj.figure
 
         if plt is not None and isinstance(obj, plt.Figure):  # type: ignore
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.savefig(stream, format=format, **kwargs)
             image = stream.getvalue()
         elif so is not None and isinstance(obj, so.Plot):
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.save(stream, format=format, **kwargs)
             image = stream.getvalue()
         elif alt is not None and isinstance(obj, alt.Chart):
             convert = vlc.vegalite_to_svg if format == "svg" else vlc.vegalite_to_png  # type: ignore  # noqa: E501
-            image = convert(obj.to_json(), **kwargs)  # type: ignore
-        else:  # pragma: no cover
+            image = convert(  # type: ignore
+                obj.to_json(),
+                vl_version="_".join(alt.SCHEMA_VERSION.split(".")[:2]),
+                **kwargs,
+            )
+        else:
             error_msg = (
                 f"Chart type {type(obj)} is not supported "
                 "or required extra package is not installed."
             )
             raise TypeError(error_msg)
 
         content = Image(data=image, format=format, class_=class_)  # type: ignore
         self.container = content.container
 
 
-class Content(ContentBase):
-    """A content definition.
+class Obj(ContentBase):
+    """An arbitrary content definition.
 
     Creates content elements from arbitrary objects and appends them to the container.
 
     Automatically determines the content type.
     """
     def __init__(self, *objects: Any, class_: str | None = None):
         """Initialize content from arbitrary objects.
@@ -348,7 +366,124 @@
             elif hasattr(obj, "_repr_html_") and callable(obj._repr_html_):
                 content = HTML(obj._repr_html_(), strip_dataframe_borders=True)
             else:
                 content = Text(obj)
 
             for element in content.container:
                 self.container.append(element)
+
+
+class Script(ContentBase):
+    """A script definition.
+
+    Attributes:
+        script (Element): The script element.
+        footer (bool): Defines whether the script should be placed at a document footer,
+            aftert all other content.
+    """
+    script: ET.Element
+    footer: bool = False
+
+    def __init__(
+        self,
+        text: str | None = None,
+        src: str | None = None,
+        inline: bool = False,
+        defer: bool = False,
+        attrib: dict[str, Any] = {},
+        **extra: Any,
+    ):
+        """Initialize script.
+
+        Either `text` or `src` should be used.
+
+        Args:
+            text: The script text.
+            src: The script source link.
+            inline: If True, load script inline, downdload it from source link
+                and use it as a text.
+            defer: The script "defer" attribute. For inline script defines whether
+                it should be placed at a document footer, aftert all other content.
+            attrib: The script attributes.
+            **extra: Extra attributes.
+
+        Raises:
+            ValueError: Both text and src are not None.
+            ValueError: Both text and src are None.
+        """
+        if text is not None and src is not None:
+            raise ValueError("Either `text` or `src` should be None.")
+
+        if text is None and src is None:
+            raise ValueError("Either `text` or `src` should be not None.")
+
+        if inline and src is not None:
+            with urllib.request.urlopen(src) as response:
+                text = response.read().decode()
+            src = None
+
+        if src is not None:
+            attrib = {"src": src, **attrib}
+            if defer:
+                attrib = {"defer": True, **attrib}
+        else:
+            self.footer = defer
+
+        self.script = ET.Element("script", {**attrib, **extra})
+        self.script.text = text
+        self.container = self.script
+
+
+class Style(ContentBase):
+    """A stylesheet definition.
+
+    Attributes:
+        style (Element): The style element.
+    """
+    style: ET.Element
+
+    def __init__(
+        self,
+        text: str | None = None,
+        src: str | None = None,
+        inline: bool = False,
+        attrib: dict[str, Any] = {},
+        **extra: Any,
+    ):
+        """Initialize stylesheet.
+
+        Either `text` or `src` should be used.
+
+        Args:
+            text: The stylesheet text.
+            src: The stylesheet source link.
+            inline: If True, load stylesheet inline, downdload it from source link
+                and use it as a text.
+            attrib: The stylesheet attributes.
+            **extra: Extra attributes.
+
+        Raises:
+            ValueError: Both text and src are not None.
+            ValueError: Both text and src are None.
+        """
+        if text is not None and src is not None:
+            raise ValueError("Either `text` or `src` should be None.")
+
+        if text is None and src is None:
+            raise ValueError("Either `text` or `src` should be not None.")
+
+        if inline and src is not None:
+            with urllib.request.urlopen(src) as response:
+                text = response.read().decode()
+            src = None
+
+        if src is not None:
+            tag = "link"
+            attrib = {"src": src, **attrib}
+            if "rel" not in attrib:
+                attrib = {**attrib, "rel": "stylesheet"}
+        else:
+            tag = "style"
+
+        self.style = ET.Element(tag, {**attrib, **extra})
+        self.style.text = text
+        self.container = self.style
```

### Comparing `rico-0.0.5/src/rico/html.py` & `rico-0.0.6/src/rico/_html.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 """HTML parser and serializer."""
 
 from __future__ import annotations
 
 import html.parser
 import xml.etree.ElementTree as ET
 
+import rico._config
+
 
 TAGS_EMPTY = {
     "area", "base", "basefont", "br", "col", "embed", "frame", "hr", "img",
     "input", "isindex", "link", "meta", "param", "path", "source", "track", "wbr",
 }
 
 TAGS_INLINE = {
     "a", "abbr", "b", "bdi", "bdo", "br", "cite", "code", "data", "dfn", "em",
     "i", "kbd", "mark", "q", "rp", "rt", "ruby", "s", "samp", "small", "span",
     "strong", "sub", "sup", "time", "u", "var", "wbr",
 }
 
 TAGS_NOT_ESCAPED = {"script", "style"}
-TAGS_PRE_FORMATTED = {"pre"}
+TAGS_PREFORMATTED = {"pre"}
 
 
 class HTMLParser(html.parser.HTMLParser):
     """Simple HTML parser. Returns a list of instances of ET.Element on close().
 
     Assigns None values to boolean attributes.
 
     Ignores comments, doctype declaration and processing instructions.
     Converts attribute names to lower case, even for SVG.
     """
 
-    def __init__(self):  # noqa: D107
+    def __init__(self):
         super().__init__()
         self._root = "root"
         self._builder = ET.TreeBuilder()
         self._builder.start(self._root, {})
 
-    def handle_starttag(  # noqa: D102
+    def handle_starttag(
         self,
         tag: str,
         attrs: list[tuple[str, str | None]],
     ) -> None:
         self._builder.start(tag, dict(attrs))
 
-    def handle_endtag(self, tag: str) -> None:  # noqa: D102
+    def handle_endtag(self, tag: str) -> None:
         self._builder.end(tag)
 
-    def handle_data(self, data: str) -> None:  # noqa: D102
+    def handle_data(self, data: str) -> None:
         self._builder.data(data)
 
-    def close(self) -> list[ET.Element]:  # noqa: D102
+    def close(self) -> list[ET.Element]:
         super().close()
         self._builder.end(self._root)
         return list(self._builder.close())
 
 
 def parse_html(data: str) -> list[ET.Element]:
     """Parse an HTML document from a string.
@@ -89,15 +91,15 @@
         element: The element to indent.
         space: The whitespace to insert for each indentation level.
         level: The initial indentation level. Should always be 0.
 
     Returns:
         The indented HTML element.
     """
-    if element.tag.lower() in TAGS_PRE_FORMATTED or not len(element):
+    if element.tag.lower() in TAGS_PREFORMATTED or not len(element):
         return element
 
     indented_element = ET.Element(element.tag, attrib=element.attrib)
     indented_element.text = element.text
     indented_element.tail = element.tail
 
     if not element.text or not element.text.strip():
@@ -107,16 +109,16 @@
         indented_child = indent_html(child, space=space, level=level + 1)
 
         if not indented_child.tail or not indented_child.tail.strip():
             indented_child.tail = "\n" + space * (level + 1)
 
         indented_element.append(indented_child)
 
-    if not indented_child.tail or not indented_child.tail.strip():  # pyright: ignore [reportUnboundVariable]  # noqa: E501
-        indented_child.tail = "\n" + space * level  # pyright: ignore [reportUnboundVariable]  # noqa: E501
+    if not indented_child.tail or not indented_child.tail.strip():  # type: ignore
+        indented_child.tail = "\n" + space * level  # type: ignore
 
     return indented_element
 
 
 def strip_html(element: ET.Element) -> ET.Element:
     """Strip an HTML element.
 
@@ -130,15 +132,15 @@
     Returns:
         The stripped HTML element.
     """
     stripped_element = ET.Element(element.tag, attrib=element.attrib)
     stripped_element.text = element.text
     stripped_element.tail = element.tail
 
-    if element.tag.lower() in TAGS_INLINE | TAGS_PRE_FORMATTED:
+    if element.tag.lower() in TAGS_INLINE | TAGS_PREFORMATTED:
         for child in element:
             stripped_element.append(child)
     else:
         for child in element:
             stripped_element.append(strip_html(child))
 
         if stripped_element.text:
@@ -177,43 +179,51 @@
         text = text.replace(">", "&gt;")
     if '"' in text:
         text = text.replace('"', "&quot;")
     return text
 
 def serialize_html(
     element: ET.Element,
-    indent_space: str | None = None,
-    strip: bool = False,
+    indent: bool | None = None,
+    space: str | None = None,
+    strip: bool | None = None,
 ) -> str:
-    """Serialize an HTML document to a string.
-
-    Indent the document if `indent_space` is not None.
+    """Serialize an HTML element to a string.
 
     Serialize attributes with None values as boolean.
 
     Args:
-        element: The HTML document.
-        indent_space: The whitespace for indentation.
+        element: The HTML element.
+        indent: If True, indent the element.
+        space: The whitespace for indentation.
         strip: If True, strip unnecessary whitespace.
 
     Returns:
-        The serialized HTML document.
+        The serialized HTML element.
     """
+    global_config = rico._config.get_config()
+    if indent is None:
+        indent = global_config["indent_html"]
+    if space is None:
+        space = global_config["indent_space"]
+    if strip is None:
+        strip = global_config["strip_html"]
+
     if strip:
         element = strip_html(element)
-
-    if indent_space is not None:
-        element = indent_html(element, space=indent_space)
+    if indent:
+        element = indent_html(element, space=space)  # type: ignore
 
     attrib = "".join(
         f' {k}="{_escape_attrib_html(v)}"'
-        if v is not None  # pyright: ignore [reportUnnecessaryComparison]
+        if v is not None and not isinstance(v, bool)  # type: ignore
         # Serialize attributes with None values as boolean.
         else f" {k}"
         for k, v in element.items()
+        if not isinstance(v, bool) or v
     )
 
     opening_tag = f"<{element.tag}{attrib}>"
     ltag = element.tag.lower()
 
     if element.text is not None:
         text = element.text if ltag in TAGS_NOT_ESCAPED else _escape_cdata(element.text)
```

### Comparing `rico-0.0.5/tests/test_html.py` & `rico-0.0.6/tests/test__html.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import textwrap
 import xml.etree.ElementTree as ET
 
 import pytest
 
-import rico.html
+import rico._html
 
 
 def elem_to_string(elem: ET.Element | list[ET.Element], sep: str = "") -> str:
     if isinstance(elem, list):
         return sep.join(elem_to_string(e) for e in elem)
     return ET.tostring(elem, encoding="unicode", method="html")
 
 
 def test_html_parser_two_elements():
     text = "<p>Hello</p><p>world</p>"
-    parser = rico.html.HTMLParser()
+    parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert elem_to_string(elements) == text
     assert isinstance(elements, list)
     assert len(elements) == 2
 
@@ -39,15 +39,15 @@
     assert p1.text == "world"
     assert p1.tail is None
     assert len(p1) == 0
 
 
 def test_html_parser_nested_tags():
     text = "<div><p>Hello <strong>world</strong>!</p></div>"
-    parser = rico.html.HTMLParser()
+    parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert elem_to_string(elements) == text
     assert isinstance(elements, list)
     assert len(elements) == 1
 
@@ -75,15 +75,15 @@
     assert strong.tail == "!"
     assert len(strong) == 0
 
 
 def test_html_parser_attributes():
     script_src = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     text = f"<script defer src='{script_src}' crossorigin='anonymous'></script>"
-    parser = rico.html.HTMLParser()
+    parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert isinstance(elements, list)
     assert len(elements) == 1
 
     script = elements[0]
@@ -103,15 +103,15 @@
     text = (
         '<svg xmlns="http://www.w3.org/2000/svg" '
         'xmlns:xlink="http://www.w3.org/1999/xlink" '
         'width="16" height="16" fill="currentColor" class="bi bi-dash">'
         '<path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>'
         "</svg>"
     )
-    parser = rico.html.HTMLParser()
+    parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert isinstance(elements, list)
     assert len(elements) == 1
 
     svg = elements[0]
@@ -138,15 +138,15 @@
     assert path.text is None
     assert path.tail is None
     assert len(path) == 0
 
 
 def test_parse_html():
     text = "<p>Hello world</p>"
-    elements = rico.html.parse_html(text)
+    elements = rico._html.parse_html(text)
 
     assert elem_to_string(elements) == text
     assert isinstance(elements, list)
     assert len(elements) == 1
 
     p = elements[0]
     assert isinstance(p, ET.Element)
@@ -196,15 +196,15 @@
           </div>
           <pre>
         <code> should not be indented </code>
         </pre>
           <p> Hello &gt;&amp;&lt; <br> world again </p>
         </div>""")
 
-    assert elem_to_string(rico.html.indent_html(sample_elem)) == expectation
+    assert elem_to_string(rico._html.indent_html(sample_elem)) == expectation
 
 
 def test_indent_html_custom_space(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
             <p> Hello <strong> world </strong> ! </p>
             <div class="&gt;&amp;&quot;">
@@ -213,15 +213,15 @@
             <pre>
         <code> should not be indented </code>
         </pre>
             <p> Hello &gt;&amp;&lt; <br> world again </p>
         </div>""")
 
     assert elem_to_string(
-        rico.html.indent_html(sample_elem, "    ")) == expectation
+        rico._html.indent_html(sample_elem, "    ")) == expectation
 
 
 def test_strip_html(sample_elem: ET.Element):
     p = ET.Element("p")
     p.text = " Hello world again again "
     sample_elem.append(p)
 
@@ -229,15 +229,15 @@
         '<div class="container"><p>Hello <strong> world </strong> !</p>'
         '<div class="&gt;&amp;&quot;"><code> should be indented </code></div><pre>\n'
         "<code> should not be indented </code>\n"
         "</pre><p>Hello &gt;&amp;&lt; <br>world again</p>"
         "<p>Hello world again again</p></div>"
     )
 
-    assert elem_to_string(rico.html.strip_html(sample_elem)) == expectation
+    assert elem_to_string(rico._html.strip_html(sample_elem)) == expectation
 
 
 def test_serialize_html_default(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
         <p> Hello <strong> world </strong> ! </p>
         <div class="&gt;&amp;&quot;">
@@ -245,15 +245,15 @@
         </div>
         <pre>
         <code> should not be indented </code>
         </pre>
         <p> Hello &gt;&amp;&lt; <br> world again </p>
         </div>""")
 
-    assert rico.html.serialize_html(sample_elem) == expectation
+    assert rico._html.serialize_html(sample_elem) == expectation
 
 
 def test_serialize_html_indent(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
             <p> Hello <strong> world </strong> ! </p>
             <div class="&gt;&amp;&quot;">
@@ -261,26 +261,27 @@
             </div>
             <pre>
         <code> should not be indented </code>
         </pre>
             <p> Hello &gt;&amp;&lt; <br> world again </p>
         </div>""")
 
-    assert rico.html.serialize_html(sample_elem, "    ") == expectation
+    assert rico._html.serialize_html(
+        sample_elem, indent=True, space="    ") == expectation
 
 
 def test_serialize_html_strip(sample_elem: ET.Element):
     expectation = (
         '<div class="container"><p>Hello <strong> world </strong> !</p>'
         '<div class="&gt;&amp;&quot;"><code> should be indented </code></div><pre>\n'
         "<code> should not be indented </code>\n"
         "</pre><p>Hello &gt;&amp;&lt; <br>world again</p></div>"
     )
 
-    assert rico.html.serialize_html(sample_elem, strip=True) == expectation
+    assert rico._html.serialize_html(sample_elem, strip=True) == expectation
 
 
 def test_serialize_html_bool_attr(sample_elem: ET.Element):
     sample_elem.set("autofocus", None)  # type: ignore
     expectation = textwrap.dedent("""\
         <div class="container" autofocus>
         <p> Hello <strong> world </strong> ! </p>
@@ -289,14 +290,30 @@
         </div>
         <pre>
         <code> should not be indented </code>
         </pre>
         <p> Hello &gt;&amp;&lt; <br> world again </p>
         </div>""")
 
-    assert rico.html.serialize_html(sample_elem) == expectation
+    assert rico._html.serialize_html(sample_elem) == expectation
+    sample_elem.set("autofocus", True)  # type: ignore
+    assert rico._html.serialize_html(sample_elem) == expectation
+
+    sample_elem.set("autofocus", False)  # type: ignore
+    expectation = textwrap.dedent("""\
+        <div class="container">
+        <p> Hello <strong> world </strong> ! </p>
+        <div class="&gt;&amp;&quot;">
+        <code> should be indented </code>
+        </div>
+        <pre>
+        <code> should not be indented </code>
+        </pre>
+        <p> Hello &gt;&amp;&lt; <br> world again </p>
+        </div>""")
+    assert rico._html.serialize_html(sample_elem) == expectation
 
 
 def test_serialize_html_style():
     elem = ET.Element("style")
     elem.text = ".>&< {border: none;}"
-    assert rico.html.serialize_html(elem) == "<style>.>&< {border: none;}</style>"
+    assert rico._html.serialize_html(elem) == "<style>.>&< {border: none;}</style>"
```

### Comparing `rico-0.0.5/PKG-INFO` & `rico-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.0.5
+Version: 0.0.6
 Summary: Rich content to HTML as easy as Doc([df, plot]).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -34,13 +34,13 @@
 Description-Content-Type: text/markdown
 
 # rico
 Rich content to HTML as easy as Doc([df, plot]).
 
 <br>
 
-[![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
-[![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
-[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
+[![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
+[![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
+[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
```

