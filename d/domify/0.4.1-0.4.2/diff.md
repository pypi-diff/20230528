# Comparing `tmp/domify-0.4.1.tar.gz` & `tmp/domify-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domify-0.4.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `domify-0.4.1.tar` & `domify-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-02-03 14:54:53.544517 domify-0.4.1/LICENSE
--rw-r--r--   0        0        0     5498 2023-02-03 14:54:53.544517 domify-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-02-03 14:54:53.544517 domify-0.4.1/domify/__init__.py
--rw-r--r--   0        0        0    12041 2023-02-03 14:54:53.544517 domify-0.4.1/domify/base_element.py
--rw-r--r--   0        0        0      977 2023-02-03 14:54:53.544517 domify-0.4.1/domify/exc.py
--rw-r--r--   0        0        0    25263 2023-02-03 14:54:53.544517 domify-0.4.1/domify/html_elements.py
--rw-r--r--   0        0        0        0 2023-02-03 14:54:53.544517 domify-0.4.1/domify/py.typed
--rw-r--r--   0        0        0     2769 2023-02-03 14:54:53.544517 domify-0.4.1/domify/validators.py
--rw-r--r--   0        0        0     3150 2023-02-03 14:54:53.548517 domify-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 domify-0.4.1/setup.py
--rw-r--r--   0        0        0     6502 1970-01-01 00:00:00.000000 domify-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 domify-0.4.2/domify/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.2/domify/__init__.py
+-rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 domify-0.4.2/domify/base_element.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 domify-0.4.2/domify/exc.py
+-rw-r--r--   0        0        0    25411 2020-02-02 00:00:00.000000 domify-0.4.2/domify/html_elements.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domify-0.4.2/domify/py.typed
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 domify-0.4.2/domify/validators.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 domify-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 domify-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 domify-0.4.2/README.md
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 domify-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 domify-0.4.2/PKG-INFO
```

### Comparing `domify-0.4.1/LICENSE` & `domify-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domify-0.4.1/README.md` & `domify-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `domify-0.4.1/domify/base_element.py` & `domify-0.4.2/domify/base_element.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+from __future__ import annotations
+
 import sys
 import warnings
 from contextvars import ContextVar
 from html import escape
 from types import TracebackType
 from typing import (
     Callable,
     Dict,
     Iterable,
     Iterator,
-    List,
-    Optional,
     Set,
-    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-from . import exc
-from . import validators as v
+from domify import exc
+from domify import validators as v
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
@@ -39,23 +38,23 @@
     is_empty = False
     global_attributes: _T_attributes_dict = {}
     element_attributes: _T_attributes_dict = {}
     any_attribute = False
 
     _default_prepend_doctype = False
 
-    _stack_var: ContextVar[Optional[List[List["BaseElement"]]]] = ContextVar(
+    _stack_var: ContextVar[list[list[BaseElement]] | None] = ContextVar(
         "stack", default=None
     )
 
     def __init__(
         self,
         *args: _T_child,
-        _prepend_doctype: Optional[bool] = None,
-        **kwargs: Optional[_T_attribute],
+        _prepend_doctype: bool | None = None,
+        **kwargs: _T_attribute | None,
     ) -> None:
         """
         Args:
             *args: The element's children. A `TextNode` is automatically created when
                 passing anything other than a subclass of `BaseElement`.
             _prepend_doctype: Whether a `DOCTYPE` declaration should be prepended.
                 Defaults to the value of the class attribute `_default_prepend_doctype`
@@ -72,40 +71,40 @@
         """
         if self.is_empty and args:
             raise exc.EmptyElementChildrenError()
 
         if _prepend_doctype is None:
             _prepend_doctype = self._default_prepend_doctype
         self._prepend_doctype = _prepend_doctype
-        self._attributes: Dict[str, Union[str, Literal[True]]] = {}
-        self._children: List["BaseElement"] = []
+        self._attributes: dict[str, str | Literal[True]] = {}
+        self._children: list[BaseElement] = []
 
         self._add_to_stack(self)
 
         for child in args:
             self._add_child(child)
 
         for key, val in kwargs.items():
             if val is None:
                 continue
             self._set_attribute(key, val)
 
     @property
-    def _stack(self) -> List[List["BaseElement"]]:
+    def _stack(self) -> list[list[BaseElement]]:
         stack = self._stack_var.get()
         if stack is None:
             stack = []
             self._stack_var.set(stack)
         return stack
 
-    def _add_to_stack(self, element: "BaseElement") -> None:
+    def _add_to_stack(self, element: BaseElement) -> None:
         if self._stack:
             self._stack[-1].append(element)
 
-    def _remove_from_stack(self, element: "BaseElement") -> None:
+    def _remove_from_stack(self, element: BaseElement) -> None:
         if self._stack and element in self._stack[-1]:
             self._stack[-1].remove(element)
         self._maybe_clear_stack()
 
     def _maybe_clear_stack(self) -> None:
         if not self._stack:
             self._stack_var.set(None)
@@ -115,15 +114,15 @@
         """
         Returns:
             The lowercase name of the element, with trailing underscores removed.
         """
         return type(self).__name__.rstrip("_").lower()
 
     # Attributes
-    def get_classes(self) -> List[str]:
+    def get_classes(self) -> list[str]:
         """Get the current element's classes
 
         Returns:
             The current element's classes as a list of strings.
         """
         classes = self._attributes.get("class", True)
         if classes is True:
@@ -198,18 +197,18 @@
 
     # Children
     @overload
     def add(self, child: _T_BaseElement) -> _T_BaseElement:
         ...
 
     @overload
-    def add(self, child: _T_child) -> "BaseElement":
+    def add(self, child: _T_child) -> BaseElement:
         ...
 
-    def add(self, child: _T_child) -> "BaseElement":
+    def add(self, child: _T_child) -> BaseElement:
         """Add a child to the current element
 
         Args:
             child: The child. A `TextNode` is automatically created when passing
                 anything other than a subclass of `BaseElement`.
 
         Returns:
@@ -218,18 +217,18 @@
         return self._add_child(child)
 
     @overload
     def insert(self, idx: int, child: _T_BaseElement) -> _T_BaseElement:
         ...
 
     @overload
-    def insert(self, idx: int, child: _T_child) -> "BaseElement":
+    def insert(self, idx: int, child: _T_child) -> BaseElement:
         ...
 
-    def insert(self, idx: int, child: _T_child) -> "BaseElement":
+    def insert(self, idx: int, child: _T_child) -> BaseElement:
         """Insert a child before the index specified
 
         Args:
             idx: The index.
             child: The child. A `TextNode` is automatically created when passing
                 anything other than a subclass of `BaseElement`.
 
@@ -238,33 +237,33 @@
         """
         return self._add_child(child, idx=idx)
 
     def _add_child(
         self,
         child: _T_child,
         *,
-        idx: Optional[int] = None,
+        idx: int | None = None,
         idx_replace: bool = False,
         exit_context_manager: bool = False,
-    ) -> "BaseElement":
+    ) -> BaseElement:
         if not isinstance(child, BaseElement):
             child = TextNode(child)
         if idx is None:
             self._children.append(child)
         elif idx_replace:
             self._children[idx] = child
         else:
             self._children.insert(idx, child)
         if not exit_context_manager:
             self._remove_from_stack(child)
         return child
 
     # Render
-    def _render(self) -> List[str]:
-        if type(self) is BaseElement:  # pylint: disable=unidiomatic-typecheck
+    def _render(self) -> list[str]:
+        if type(self) is BaseElement:
             return [str(child) for child in self._children]
 
         data = []
         if self._prepend_doctype:
             data.append("<!DOCTYPE html>")
         attrs = []
         for key, val in self._attributes.items():
@@ -279,28 +278,28 @@
                 data.append(str(child))
             data.append(f"</{self.name}>")
 
         return data
 
     # Dunder methods
     @overload
-    def __getitem__(self, key: str) -> Union[str, bool]:
+    def __getitem__(self, key: str) -> str | bool:
         ...
 
     @overload
-    def __getitem__(self, key: int) -> "BaseElement":
+    def __getitem__(self, key: int) -> BaseElement:
         ...
 
     @overload
-    def __getitem__(self, key: slice) -> List["BaseElement"]:
+    def __getitem__(self, key: slice) -> list[BaseElement]:
         ...
 
     def __getitem__(
-        self, key: Union[str, int, slice]
-    ) -> Union[Union[str, bool], "BaseElement", List["BaseElement"]]:
+        self, key: str | int | slice
+    ) -> str | bool | BaseElement | list[BaseElement]:
         if isinstance(key, str):
             return self._attributes.get(key, False)
         return self._children[key]
 
     @overload
     def __setitem__(self, key: str, val: _T_attribute) -> None:
         ...
@@ -311,16 +310,16 @@
 
     @overload
     def __setitem__(self, key: slice, val: Iterable[_T_child]) -> None:
         ...
 
     def __setitem__(
         self,
-        key: Union[str, int, slice],
-        val: Union[_T_attribute, _T_child, Iterable[_T_child]],
+        key: str | int | slice,
+        val: _T_attribute | _T_child | Iterable[_T_child],
     ) -> None:
         if isinstance(key, str):
             val = cast(_T_attribute, val)
             self._set_attribute(key, val)
         elif isinstance(key, int):
             val = cast(_T_child, val)
             self._add_child(val, idx=key, idx_replace=True)
@@ -330,69 +329,69 @@
                 TextNode(child) if not isinstance(child, BaseElement) else child
                 for child in val
             ]
             self._children[key] = children
             for child in children:
                 self._remove_from_stack(child)
 
-    def __delitem__(self, key: Union[str, int, slice]) -> None:
+    def __delitem__(self, key: str | int | slice) -> None:
         if isinstance(key, str):
             del self._attributes[key]
         else:
             del self._children[key]
 
-    def __add__(self, other: _T_child) -> "BaseElement":
+    def __add__(self, other: _T_child) -> BaseElement:
         return BaseElement(self, other)
 
-    def __radd__(self, other: _T_child) -> "BaseElement":
+    def __radd__(self, other: _T_child) -> BaseElement:
         return BaseElement(other, self)
 
     def __enter__(self: _T_BaseElement) -> _T_BaseElement:
         self._stack.append([])
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
     ) -> None:
         for child in self._stack.pop():
             self._add_child(child, exit_context_manager=True)
         self._maybe_clear_stack()
 
     def __len__(self) -> int:
         return len(self._children)  # pragma: no cover
 
-    def __iter__(self) -> Iterator["BaseElement"]:
+    def __iter__(self) -> Iterator[BaseElement]:
         return self._children.__iter__()  # pragma: no cover
 
     def __bool__(self) -> bool:
         return True  # pragma: no cover
 
     def __str__(self) -> str:
         return "".join(self._render())
 
 
 class TextNode(BaseElement):
     """Class representing a text node"""
 
-    def __init__(self, text: Union[str, float]) -> None:
+    def __init__(self, text: str | float) -> None:
         """
         Args:
             text: The content of the text node.
         """
         if not isinstance(text, str):
             text = str(text)
         self.text = text
 
         super().__init__()
 
-    def _render(self) -> List[str]:
+    def _render(self) -> list[str]:
         return [escape(self.text)]
 
 
 class RawTextNode(TextNode):
     """Class representing a text node, without escaping the content"""
 
-    def _render(self) -> List[str]:
+    def _render(self) -> list[str]:
         return [self.text]
```

### Comparing `domify-0.4.1/domify/exc.py` & `domify-0.4.2/domify/exc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from .base_element import BaseElement
+    from domify.base_element import BaseElement
 
 
 class EmptyElementChildrenError(Exception):
     """Trying to add a children to a empty element"""
 
 
 class InvalidAttributeWarning(UserWarning):
     """Invalid element attribute"""
 
-    def __init__(self, element: "BaseElement", attribute: str) -> None:
+    def __init__(self, element: BaseElement, attribute: str) -> None:
         self.element = element.name
         self.attribute = attribute
         super().__init__(
             f"Attribute `{self.attribute}` not allowed on element `{self.element}`"
         )
 
 
 class InvalidAttributeValueWarning(UserWarning):
     """Invalid attribute value"""
 
-    def __init__(self, element: "BaseElement", attribute: str, value: str) -> None:
+    def __init__(self, element: BaseElement, attribute: str, value: str) -> None:
         self.element = element.name
         self.attribute = attribute
         self.value = value
         super().__init__(
             f"Bad value `{self.value}` "
             f"for attribute `{self.attribute}` "
             f"on element `{self.element}'"
```

### Comparing `domify-0.4.1/domify/html_elements.py` & `domify-0.4.2/domify/html_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# pylint: disable=too-many-lines
+# ruff: noqa: E742
 
-from . import validators as v
-from .base_element import BaseElement
-from .base_element import RawTextNode as RawTextNode  # pylint: disable=unused-import
-from .base_element import TextNode as TextNode  # pylint: disable=unused-import
+from __future__ import annotations
+
+from domify import validators as v
+from domify.base_element import BaseElement
+from domify.base_element import RawTextNode as RawTextNode
+from domify.base_element import TextNode as TextNode
 
 # begin automatic
 
 
 class HtmlElement(BaseElement):
     """
     Base class for html elements, contains global attributes.
@@ -16,15 +18,15 @@
     global_attributes = {
         "accesskey": v.attribute_all(
             v.attribute_unique_set, lambda x: max(len(t) for t in str(x).split()) <= 1
         ),
         "autocapitalize": {"on", "off", "none", "sentences", "words", "characters"},
         "autofocus": v.attribute_bool,
         "class": v.attribute_str,
-        "contenteditable": {"true", "false"},
+        "contenteditable": {"true", "plaintext-only", "false"},
         "dir": {"ltr", "rtl", "auto"},
         "draggable": {"true", "false"},
         "enterkeyhint": {"enter", "done", "go", "next", "previous", "search", "send"},
         "hidden": {"until-found", "hidden", ""},
         "id": v.attribute_str,
         "inert": v.attribute_bool,
         "inputmode": {
@@ -284,17 +286,16 @@
             "multipart/form-data",
             "text/plain",
         },
         "formmethod": {"GET", "POST", "dialog"},
         "formnovalidate": v.attribute_bool,
         "formtarget": v.attribute_str,
         "name": v.attribute_str,
-        "popoverhidetarget": v.attribute_str,
-        "popovershowtarget": v.attribute_str,
-        "popovertoggletarget": v.attribute_str,
+        "popovertarget": v.attribute_str,
+        "popovertargetaction": {"toggle", "show", "hide"},
         "type": {"submit", "reset", "button"},
         "value": v.attribute_str,
     }
 
 
 class Canvas(HtmlElement):
     """
@@ -598,14 +599,15 @@
     """
 
     is_empty = True
     element_attributes = {
         "alt": v.attribute_str,
         "crossorigin": {"anonymous", "use-credentials"},
         "decoding": {"sync", "async", "auto"},
+        "fetchpriority": {"auto", "high", "low"},
         "height": v.attribute_int_ge_zero,
         "ismap": v.attribute_bool,
         "loading": {"lazy", "eager"},
         "referrerpolicy": v.attribute_str,
         "sizes": v.attribute_str,
         "src": v.attribute_str,
         "srcset": v.attribute_str,
@@ -643,17 +645,16 @@
         "maxlength": v.attribute_int_ge_zero,
         "min": v.attribute_str,
         "minlength": v.attribute_int_ge_zero,
         "multiple": v.attribute_bool,
         "name": v.attribute_str,
         "pattern": v.attribute_str,
         "placeholder": v.attribute_str,
-        "popoverhidetarget": v.attribute_str,
-        "popovershowtarget": v.attribute_str,
-        "popovertoggletarget": v.attribute_str,
+        "popovertarget": v.attribute_str,
+        "popovertargetaction": {"toggle", "show", "hide"},
         "readonly": v.attribute_bool,
         "required": v.attribute_bool,
         "size": v.attribute_int_gt_zero,
         "src": v.attribute_str,
         "step": v.attribute_any(
             v.attribute_float_gt_zero, v.attribute_str_literal("any")
         ),
@@ -730,14 +731,15 @@
     is_empty = True
     element_attributes = {
         "as": v.attribute_str,
         "blocking": v.attribute_unique_set,
         "color": v.attribute_str,
         "crossorigin": {"anonymous", "use-credentials"},
         "disabled": v.attribute_bool,
+        "fetchpriority": {"auto", "high", "low"},
         "href": v.attribute_str,
         "hreflang": v.attribute_str,
         "imagesizes": v.attribute_str,
         "imagesrcset": v.attribute_str,
         "integrity": v.attribute_str,
         "media": v.attribute_str,
         "referrerpolicy": v.attribute_str,
@@ -957,22 +959,29 @@
     """
 
     element_attributes = {
         "async": v.attribute_bool,
         "blocking": v.attribute_unique_set,
         "crossorigin": {"anonymous", "use-credentials"},
         "defer": v.attribute_bool,
+        "fetchpriority": {"auto", "high", "low"},
         "integrity": v.attribute_str,
         "nomodule": v.attribute_bool,
         "referrerpolicy": v.attribute_str,
         "src": v.attribute_str,
         "type": v.attribute_str,
     }
 
 
+class Search(HtmlElement):
+    """
+    Container for search controls
+    """
+
+
 class Section(HtmlElement):
     """
     Generic document or application section
     """
 
 
 class Select(HtmlElement):
```

### Comparing `domify-0.4.1/domify/validators.py` & `domify-0.4.2/domify/validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# pylint: disable=missing-function-docstring
+from __future__ import annotations
 
 from functools import partial
-from typing import TYPE_CHECKING, Callable, Iterable, Optional
+from typing import TYPE_CHECKING, Callable, Iterable
 
 if TYPE_CHECKING:
-    from .base_element import _T_attribute
+    from domify.base_element import _T_attribute
 
 
-def _attribute_to_string(x: "_T_attribute", case_insensitive: bool) -> str:
+def _attribute_to_string(x: _T_attribute, case_insensitive: bool) -> str:
     x = str(x)
     if case_insensitive:
         x = x.lower()
     return x
 
 
 def attribute_all(
-    *funcs: Callable[["_T_attribute"], bool]
-) -> Callable[["_T_attribute"], bool]:
+    *funcs: Callable[[_T_attribute], bool]
+) -> Callable[[_T_attribute], bool]:
     return lambda x: all(f(x) for f in funcs)
 
 
 def attribute_any(
-    *funcs: Callable[["_T_attribute"], bool]
-) -> Callable[["_T_attribute"], bool]:
+    *funcs: Callable[[_T_attribute], bool]
+) -> Callable[[_T_attribute], bool]:
     return lambda x: any(f(x) for f in funcs)
 
 
-def attribute_bool(x: "_T_attribute") -> bool:
+def attribute_bool(x: _T_attribute) -> bool:
     return isinstance(x, bool)
 
 
-def attribute_int(x: "_T_attribute") -> bool:
+def attribute_int(x: _T_attribute) -> bool:
     return isinstance(x, int)
 
 
-def attribute_int_ge_zero(x: "_T_attribute") -> bool:
+def attribute_int_ge_zero(x: _T_attribute) -> bool:
     return isinstance(x, int) and x >= 0
 
 
-def attribute_int_gt_zero(x: "_T_attribute") -> bool:
+def attribute_int_gt_zero(x: _T_attribute) -> bool:
     return isinstance(x, int) and x > 0
 
 
-def attribute_float(x: "_T_attribute") -> bool:
+def attribute_float(x: _T_attribute) -> bool:
     return isinstance(x, (float, int))
 
 
-def attribute_float_gt_zero(x: "_T_attribute") -> bool:
+def attribute_float_gt_zero(x: _T_attribute) -> bool:
     return isinstance(x, (float, int)) and x > 0
 
 
 def attribute_str(
-    x: "_T_attribute",
+    x: _T_attribute,
     *,
-    values: Optional[Iterable[str]] = None,
-    case_insensitive: bool = False
+    values: Iterable[str] | None = None,
+    case_insensitive: bool = False,
 ) -> bool:
     if isinstance(x, bool):
         return False
     if values:
         x = _attribute_to_string(x, case_insensitive)
         if x not in values:
             return False
@@ -66,27 +66,27 @@
 
 
 attribute_str_ci = partial(attribute_str, case_insensitive=True)
 
 
 def attribute_str_literal(
     *values: str, case_insensitive: bool = False
-) -> Callable[["_T_attribute"], bool]:
+) -> Callable[[_T_attribute], bool]:
     return partial(attribute_str, values=values, case_insensitive=case_insensitive)
 
 
 attribute_str_literal_ci = partial(attribute_str_literal, case_insensitive=True)
 
 
 def attribute_unique_set(
-    x: "_T_attribute",
+    x: _T_attribute,
     *,
-    values: Optional[Iterable[str]] = None,
+    values: Iterable[str] | None = None,
     sep: str = " ",
-    case_insensitive: bool = False
+    case_insensitive: bool = False,
 ) -> bool:
     if isinstance(x, bool):
         return False
     x = _attribute_to_string(x, case_insensitive)
     parts = x.split(sep)
     if len(parts) != len(set(parts)):
         return False
@@ -96,15 +96,15 @@
 
 
 attribute_unique_set_ci = partial(attribute_unique_set, case_insensitive=True)
 
 
 def attribute_unique_set_literal(
     *values: str, sep: str = " ", case_insensitive: bool = False
-) -> Callable[["_T_attribute"], bool]:
+) -> Callable[[_T_attribute], bool]:
     return partial(
         attribute_unique_set, values=values, sep=sep, case_insensitive=case_insensitive
     )
 
 
 attribute_unique_set_literal_ci = partial(
     attribute_unique_set_literal, case_insensitive=True
```

### Comparing `domify-0.4.1/PKG-INFO` & `domify-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: domify
-Version: 0.4.1
+Version: 0.4.2
 Summary: HTML generator using pure Python
-Home-page: https://github.com/Parnassius/domify
-License: MIT
-Author: Parnassius
-Author-email: Parnassius@users.noreply.github.com
-Requires-Python: >=3.7.2,<4.0.0
+Project-URL: homepage, https://github.com/Parnassius/domify
+Author-email: Parnassius <Parnassius@users.noreply.github.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Typing :: Typed
-Requires-Dist: typing-extensions (>=3.7) ; python_version < "3.8"
-Project-URL: Repository, https://github.com/Parnassius/domify
+Requires-Python: >=3.7
+Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Description-Content-Type: text/markdown
 
 # domify
 
 HTML generator using pure Python.
 
 [![PyPI](https://img.shields.io/pypi/v/domify)](https://pypi.org/project/domify/)
@@ -242,8 +235,7 @@
 ```html
 <p>
   &lt;i&gt;TextNode&lt;/i&gt;
   <br>
   <i>RawTextNode</i>
 </p>
 ```
-
```

