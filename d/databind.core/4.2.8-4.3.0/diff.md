# Comparing `tmp/databind.core-4.2.8.tar.gz` & `tmp/databind.core-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.8.tar", max compression
+gzip compressed data, was "databind.core-4.3.0.tar", max compression
```

## Comparing `databind.core-4.2.8.tar` & `databind.core-4.3.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0     1724 2023-05-28 04:19:55.966712 databind.core-4.2.8/pyproject.toml
--rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.8/readme.md
--rw-r--r--   0        0        0       22 2023-05-28 04:19:55.970711 databind.core-4.2.8/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/py.typed
--rw-r--r--   0        0        0    15319 2023-05-28 04:14:21.356217 databind.core-4.2.8/src/databind/core/schema.py
--rw-r--r--   0        0        0    26836 2023-05-28 04:18:51.936531 databind.core-4.2.8/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-05-28 04:20:01.628756 databind.core-4.2.8/setup.py
--rw-r--r--   0        0        0     2343 2023-05-28 04:20:01.628966 databind.core-4.2.8/PKG-INFO
+-rw-r--r--   0        0        0      337 2023-05-28 15:36:26.896939 databind.core-4.3.0/README.md
+-rw-r--r--   0        0        0     1687 2023-05-28 18:45:00.561567 databind.core-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1601 2023-05-28 18:45:00.561567 databind.core-4.3.0/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-05-28 03:24:09.913921 databind.core-4.3.0/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-05-28 03:24:09.913921 databind.core-4.3.0/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-05-28 15:25:57.110899 databind.core-4.3.0/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-05-28 15:25:57.110899 databind.core-4.3.0/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-05-28 03:24:09.913921 databind.core-4.3.0/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-05-28 15:09:30.547017 databind.core-4.3.0/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15494 2023-05-28 17:58:22.401654 databind.core-4.3.0/src/databind/core/schema.py
+-rw-r--r--   0        0        0    27732 2023-05-28 18:05:32.641319 databind.core-4.3.0/src/databind/core/settings.py
+-rw-r--r--   0        0        0     1044 2023-05-28 17:47:50.951787 databind.core-4.3.0/src/databind/core/tests/context_test.py
+-rw-r--r--   0        0        0     1275 2023-05-28 17:47:58.447573 databind.core-4.3.0/src/databind/core/tests/schema_docspec_example_test.py
+-rw-r--r--   0        0        0    11386 2023-05-28 18:41:44.327180 databind.core-4.3.0/src/databind/core/tests/schema_test.py
+-rw-r--r--   0        0        0      733 2023-05-28 03:01:35.968571 databind.core-4.3.0/src/databind/core/tests/schema_with_nested_dataclasses_test.py
+-rw-r--r--   0        0        0     8709 2023-05-28 03:24:09.917921 databind.core-4.3.0/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-05-28 03:24:09.917921 databind.core-4.3.0/src/databind/core/utils.py
+-rw-r--r--   0        0        0     1261 2023-05-28 18:45:08.820628 databind.core-4.3.0/setup.py
+-rw-r--r--   0        0        0     1435 2023-05-28 18:45:08.820877 databind.core-4.3.0/PKG-INFO
```

### Comparing `databind.core-4.2.8/pyproject.toml` & `databind.core-4.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.8"
+version = "4.3.0"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
-readme = "readme.md"
+readme = "README.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
 Documentation = "https://niklasrosenstein.github.io/python-databind/"
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/python-databind"
@@ -38,21 +38,21 @@
 [build-system]
 requires = ["poetry-core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.slap.test]
 check = "slap check"
 mypy = "dmypy run src/"
-pytest = "pytest tests/ -vv"
-black = "black --check src/ tests/"
-isort = "isort --check-only src/ tests/"
-flake8 = "flake8 src/ tests/"
+pytest = "pytest src/ -vv"
+black = "black --check src/"
+isort = "isort --check-only src/"
+flake8 = "flake8 src/"
 
 [tool.slap.run]
-fmt = "black src/ tests/ && isort src/ tests/"
+fmt = "black src/ && isort src/"
 
 [tool.mypy]
 python_version = "3.6"
 explicit_package_bases = true
 mypy_path = ["src"]
 namespace_packages = true
 pretty = true
```

### Comparing `databind.core-4.2.8/src/databind/core/context.py` & `databind.core-4.3.0/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/converter.py` & `databind.core-4.3.0/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/dataclasses.py` & `databind.core-4.3.0/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/dataclasses.pyi` & `databind.core-4.3.0/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/mapper.py` & `databind.core-4.3.0/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/schema.py` & `databind.core-4.3.0/src/databind/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,15 @@
 
 if sys.version_info[:2] <= (3, 8):
     GenericAlias = t.Any
 else:
     from types import GenericAlias
 
 if t.TYPE_CHECKING:
-
-    class Constructor(t.Protocol):
-        def __call__(self, **kwargs: t.Any) -> t.Any:
-            ...
+    Constructor = t.Callable[..., t.Any]
 
 
 __all__ = [
     "Field",
     "Schema",
     "convert_to_schema",
     "convert_dataclass_to_schema",
@@ -253,15 +250,15 @@
             assert isinstance(base_hint, ClassTypeHint), f"nani? {base_hint}"
             if dataclasses.is_dataclass(base_hint.type):
                 queue.append(base_hint)
 
     return Schema(fields, t.cast("Constructor", dataclass_type), dataclass_type)
 
 
-def convert_typed_dict_to_schema(typed_dict: TypedDictProtocol) -> Schema:
+def convert_typed_dict_to_schema(typed_dict: t.Union[TypedDictProtocol, t.Type[t.Any], TypeHint]) -> Schema:
     """Converts the definition of a #typing.TypedDict to a #Schema.
 
     !!! note
 
         This function will take into account default values assigned on the class-level of the typed dict (which is
         usually only relevant if the class-style declaration method was used, but default values can be assigned to
         the function-style declared type as well). Fields that have default values are considered not-required even
@@ -288,14 +285,19 @@
     assert convert_typed_dict_to_schema(Movie) == Schema({
       'name': Field(TypeHint(str)),
       'year': Field(TypeHint(int), False, 0),
     }, Movie)
     ```
     """
 
+    if isinstance(typed_dict, TypeHint):
+        if not isinstance(typed_dict, ClassTypeHint):
+            raise TypeError(f"expected ClassTypeHint, got {typed_dict}")
+        typed_dict = typed_dict.type
+
     assert is_typed_dict(typed_dict), typed_dict
 
     eval_context = vars(sys.modules[typed_dict.__module__])
 
     annotations = get_annotations(t.cast(type, typed_dict))
     fields: t.Dict[str, Field] = {}
     for key in typed_dict.__required_keys__ | typed_dict.__optional_keys__:
```

### Comparing `databind.core-4.2.8/src/databind/core/settings.py` & `databind.core-4.3.0/src/databind/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,18 +322,49 @@
 class SerializeDefaults(BooleanSetting):
     """Control whether default values are to be encoded in the serialized form of a structure. The default behaviour
     is up to the serializer implementation, though we consider it good practices to include values that match the
     default value of a field by default. However, using the setting defaults to #enabled having a value of `True` due
     to how the name of the setting appears assertive of the fact that the instance indicates the setting is enabled."""
 
 
-# NOTE(NiklasRosenstein): For Python 3.6, metadata passed into Annotated[...] must be hashable.
+@dataclasses.dataclass(frozen=True)
+class DeserializeAs(Setting):
+    """Indicates that a field should be deserialized as the given type instead of the type of the field. This is
+    typically used when a field should be typed as an abstract class or interface, but during deserialization of the
+    field, a concrete type should be used instead.
+
+    Example:
+
+    ```py
+    import typing
+    from dataclasses import dataclass
+    from databind.core.settings import DeserializeAs
+
+    @dataclass
+    class A:
+        pass
+
+    @dataclass
+    class B(A):
+        pass
+
+    @dataclass
+    class MyClass:
+      my_field: typing.Annotated[A, DeserializeAs(B)]
+    ```
 
+    Here, although `MyClass.my_field` is annotated as `A`, when a payload is deserialized into an instance of
+    `MyClass`, the value for `my_field` will be deserialized as an instance of `B` instead of `A`.
+    """
 
-@dataclasses.dataclass
+    type: t.Type[t.Any]
+    priority: Priority = Priority.NORMAL
+
+
+@dataclasses.dataclass(frozen=True)
 class Precision(Setting):
     """A setting to describe the precision for #decimal.Decimal fields."""
 
     prec: t.Optional[int] = None
     rounding: t.Optional[str] = None
     Emin: t.Optional[int] = None
     Emax: t.Optional[int] = None
@@ -495,15 +526,15 @@
     @staticmethod
     def import_() -> "ImportUnionMembers":
         from databind.core.union import ImportUnionMembers
 
         return ImportUnionMembers()
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(init=False, unsafe_hash=True)
 class DateFormat(Setting):
     """The #DateFormat setting is used to describe the date format to use for #datetime.datetime, #datetime.date
     and #datetime.time values when formatting them as a string, i.e. usually when the date/time is serialized, and
     when parsing them.
 
     The #nr.date module provides types to describe the format of a date, time and datetime (see #date_format,
     #time_format and #datetime_format), as well as an entire suite of formats for all types of date/time values.
```

### Comparing `databind.core-4.2.8/src/databind/core/union.py` & `databind.core-4.3.0/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.8/src/databind/core/utils.py` & `databind.core-4.3.0/src/databind/core/utils.py`

 * *Files identical despite different names*

