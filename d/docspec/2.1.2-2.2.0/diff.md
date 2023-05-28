# Comparing `tmp/docspec-2.1.2.tar.gz` & `tmp/docspec-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docspec-2.1.2.tar", max compression
+gzip compressed data, was "docspec-2.2.0.tar", max compression
```

## Comparing `docspec-2.1.2.tar` & `docspec-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1397 2023-03-15 23:30:17.816414 docspec-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      629 2023-03-09 22:37:16.042666 docspec-2.1.2/readme.md
--rw-r--r--   0        0        0    20722 2023-03-15 23:30:17.836413 docspec-2.1.2/src/docspec/__init__.py
--rw-r--r--   0        0        0     2822 2023-03-15 23:29:41.729436 docspec-2.1.2/src/docspec/__main__.py
--rw-r--r--   0        0        0        0 2023-03-09 22:37:16.042666 docspec-2.1.2/src/docspec/py.typed
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 docspec-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1466 2023-05-28 03:58:32.055219 docspec-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-05-13 09:55:38.864677 docspec-2.2.0/readme.md
+-rw-r--r--   0        0        0    21250 2023-05-28 03:58:32.067219 docspec-2.2.0/src/docspec/__init__.py
+-rw-r--r--   0        0        0     2822 2023-05-13 09:55:38.864677 docspec-2.2.0/src/docspec/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-13 09:55:38.864677 docspec-2.2.0/src/docspec/py.typed
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 docspec-2.2.0/PKG-INFO
```

### Comparing `docspec-2.1.2/readme.md` & `docspec-2.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `docspec-2.1.2/src/docspec/__init__.py` & `docspec-2.2.0/src/docspec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 __all__ = [
     "Location",
     "Decoration",
     "Docstring",
     "Argument",
     "ApiObject",
     "Indirection",
@@ -51,15 +51,15 @@
 import json
 import sys
 import typing as t
 import weakref
 
 import databind.json
 import typing_extensions as te
-from databind.core.annotations import alias, union
+from databind.core.settings import Alias, SerializeDefaults, Union
 
 
 @dataclasses.dataclass
 class Location:
     """
     Represents the location of an #ApiObject by a filename and line number.
     """
@@ -129,28 +129,28 @@
         """
         The type of the argument. This is currently very Python-centric, however most other languages should be able
         to represent the various argument types with a subset of these types without additions (e.g. Java or TypeScript
         only support #Positional and #PositionalRemainder arguments).
         """
 
         #: A positional only argument. Such arguments are denoted in Python like this: `def foo(a, b, /): ...`
-        POSITIONAL_ONLY: te.Annotated[int, alias("POSITIONAL_ONLY", "PositionalOnly")] = 0
+        POSITIONAL_ONLY: te.Annotated[int, Alias("POSITIONAL_ONLY", "PositionalOnly")] = 0
 
         #: A positional argument, which may also be given as a keyword argument. Basically that is just a normal
         #: argument as you would see most commonly in Python function definitions.
-        POSITIONAL: te.Annotated[int, alias("POSITIONAL", "Positional")] = 1
+        POSITIONAL: te.Annotated[int, Alias("POSITIONAL", "Positional")] = 1
 
         #: An argument that denotes the capture of additional positional arguments, aka. "args" or "varags".
-        POSITIONAL_REMAINDER: te.Annotated[int, alias("POSITIONAL_REMAINDER", "PositionalRemainder")] = 2
+        POSITIONAL_REMAINDER: te.Annotated[int, Alias("POSITIONAL_REMAINDER", "PositionalRemainder")] = 2
 
         #: A keyword-only argument is denoted in Python like thisL `def foo(*, kwonly): ...`
-        KEYWORD_ONLY: te.Annotated[int, alias("KEYWORD_ONLY", "KeywordOnly")] = 3
+        KEYWORD_ONLY: te.Annotated[int, Alias("KEYWORD_ONLY", "KeywordOnly")] = 3
 
         #: An argument that captures additional keyword arguments, aka. "kwargs".
-        KEYWORD_REMAINDER: te.Annotated[int, alias("KEYWORD_REMAINDER", "KeywordRemainder")] = 4
+        KEYWORD_REMAINDER: te.Annotated[int, Alias("KEYWORD_REMAINDER", "KeywordRemainder")] = 4
 
         # backwards compatibility, < 1.2.0
         PositionalOnly: t.ClassVar["Argument.Type"]
         Positional: t.ClassVar["Argument.Type"]
         PositionalRemainder: t.ClassVar["Argument.Type"]
         KeywordOnly: t.ClassVar["Argument.Type"]
         KeywordRemainder: t.ClassVar["Argument.Type"]
@@ -358,14 +358,15 @@
     #: A list of decorations used on the function.
     decorations: t.Optional[t.List[Decoration]]
 
     #: A list of hints that describe the object.
     semantic_hints: t.List[FunctionSemantic] = dataclasses.field(default_factory=list)
 
 
+@dataclasses.dataclass
 class HasMembers(ApiObject):
     """
     Base class for API objects that can have members, e.g. #Class and #Module.
     """
 
     #: The members of the API object.
     members: t.Sequence[ApiObject]
@@ -433,24 +434,24 @@
     #: A list of module members.
     members: t.List["_ModuleMemberType"]
 
 
 _Members = t.Union[Variable, Function, Class, Indirection]
 _MemberType = te.Annotated[
     _Members,
-    union({"data": Variable, "function": Function, "class": Class, "indirection": Indirection}, style=union.Style.flat),
+    Union({"data": Variable, "function": Function, "class": Class, "indirection": Indirection}, style=Union.FLAT),
 ]
 
 
 _ModuleMembers = t.Union[Variable, Function, Class, Module, Indirection]
 _ModuleMemberType = te.Annotated[
     _ModuleMembers,
-    union(
+    Union(
         {"data": Variable, "function": Function, "class": Class, "module": Module, "indirection": Indirection},
-        style=union.Style.flat,
+        style=Union.FLAT,
     ),
 ]
 
 
 def load_module(
     source: t.Union[str, t.TextIO, t.Dict[str, t.Any]],
     filename: t.Optional[str] = None,
@@ -527,25 +528,32 @@
     ...
 
 
 def dump_module(
     module: Module,
     target: t.Optional[t.Union[str, t.IO[str]]] = None,
     dumper: t.Callable[[t.Any, t.IO[str]], None] = json.dump,
+    serialize_defaults: bool = False,
 ) -> t.Optional[t.Dict[str, t.Any]]:
     """
     Dumps a module to the specified target or returns it as plain structured data.
+
+    :param module: The module to dump.
+    :param target: The target to dump to. If #None, the module will be returned as plain structured data.
+    :param dumper: A function for dumping plain structured data to a file-like object. Defaults to #json.dump().
+    :param serialize_defaults: If #True, default values will be serialized into the payload. Otherwise, they will be
+        omitted. Defaults to #False.
     """
 
     if isinstance(target, str):
         with io.open(target, "w", encoding="utf-8") as fp:
             dump_module(module, fp, dumper)
         return None
 
-    data = databind.json.dump(module, Module)
+    data = databind.json.dump(module, Module, settings=[SerializeDefaults(serialize_defaults)])
     if target:
         dumper(data, target)
         target.write("\n")
         return None
     else:
         return t.cast(t.Dict[str, t.Any], data)
```

### Comparing `docspec-2.1.2/src/docspec/__main__.py` & `docspec-2.2.0/src/docspec/__main__.py`

 * *Files identical despite different names*

### Comparing `docspec-2.1.2/PKG-INFO` & `docspec-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: docspec
-Version: 2.1.2
+Version: 2.2.0
 Summary: Docspec is a JSON object specification for representing API documentation of programming languages.
 Home-page: https://github.com/NiklasRosenstein/docspec/
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
-Requires-Dist: databind (>=1.5.0,<2.0.0)
+Requires-Dist: databind-core (>=4.2.6,<5.0.0)
+Requires-Dist: databind-json (>=4.2.6,<5.0.0)
 Description-Content-Type: text/markdown
 
 # docspec
 
 This Python packages provides
 
 * A library to (de-) serialize Docspec conformat JSON payloads
```

