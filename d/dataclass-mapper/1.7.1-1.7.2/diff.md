# Comparing `tmp/dataclass_mapper-1.7.1.tar.gz` & `tmp/dataclass_mapper-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_mapper-1.7.1.tar", max compression
+gzip compressed data, was "dataclass_mapper-1.7.2.tar", max compression
```

## Comparing `dataclass_mapper-1.7.1.tar` & `dataclass_mapper-1.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1052 2023-02-22 15:14:49.374100 dataclass_mapper-1.7.1/LICENSE.md
--rw-r--r--   0        0        0     5721 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/README.rst
--rw-r--r--   0        0        0      490 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/__init__.py
--rw-r--r--   0        0        0      441 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/__init__.py
--rw-r--r--   0        0        0      487 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/assignment.py
--rw-r--r--   0        0        0      749 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/function.py
--rw-r--r--   0        0        0      752 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/list.py
--rw-r--r--   0        0        0      802 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/recursive.py
--rw-r--r--   0        0        0      272 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/simple.py
--rw-r--r--   0        0        0      559 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/assignments/utils.py
--rw-r--r--   0        0        0     3941 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/classmeta.py
--rw-r--r--   0        0        0     2186 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/enum.py
--rw-r--r--   0        0        0     2604 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/fieldmeta.py
--rw-r--r--   0        0        0    12324 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/mapper.py
--rw-r--r--   0        0        0     7793 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/mapping_method.py
--rw-r--r--   0        0        0      391 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/namespace.py
--rw-r--r--   0        0        0        0 2023-02-22 15:14:49.378100 dataclass_mapper-1.7.1/dataclass_mapper/py.typed
--rw-r--r--   0        0        0     1624 2023-02-22 15:16:00.407676 dataclass_mapper-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.1/setup.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/LICENSE.md
+-rw-r--r--   0        0        0     5722 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/README.rst
+-rw-r--r--   0        0        0      490 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/__init__.py
+-rw-r--r--   0        0        0      487 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/assignment.py
+-rw-r--r--   0        0        0     1183 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/function.py
+-rw-r--r--   0        0        0      752 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/list.py
+-rw-r--r--   0        0        0      780 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/recursive.py
+-rw-r--r--   0        0        0      272 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/simple.py
+-rw-r--r--   0        0        0      559 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/utils.py
+-rw-r--r--   0        0        0     3962 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/classmeta.py
+-rw-r--r--   0        0        0     2285 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/enum.py
+-rw-r--r--   0        0        0     2581 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/fieldmeta.py
+-rw-r--r--   0        0        0    12764 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/mapper.py
+-rw-r--r--   0        0        0     7876 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/mapping_method.py
+-rw-r--r--   0        0        0      391 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/namespace.py
+-rw-r--r--   0        0        0        0 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/py.typed
+-rw-r--r--   0        0        0     1683 2023-05-28 13:20:19.245045 dataclass_mapper-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6593 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.2/setup.py
+-rw-r--r--   0        0        0     6664 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.2/PKG-INFO
```

### Comparing `dataclass_mapper-1.7.1/LICENSE.md` & `dataclass_mapper-1.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.7.1/README.rst` & `dataclass_mapper-1.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
 .. code-block:: bash
 
    pip install dataclass-mapper
    # or for Pydantic support
    pip install 'dataclass-mapper[pydantic]'
 
-Small Example
--------------
+Example
+-------
 
 We have the following target data structure, a class called ``Person``.
 
 .. code-block:: python
 
    >>> from dataclasses import dataclass
 
@@ -91,15 +91,15 @@
    ...     age: int
 
 
 We want to have a mapper from the source data structure, a class called ``ContactInfo``.
 Notice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.
 Other than that, all the attribute names are the same.
 
-Instead of writing a mapper function by hand, you can let it autogenerate with:
+Instead of writing a mapper function by hand, you can let it autogenerate one using this library:
 
 .. code-block:: python
 
    >>> from dataclass_mapper import map_to, mapper
    >>>
    >>> @mapper(Person, {"second_name": "surname"})
    ... @dataclass
@@ -108,15 +108,15 @@
    ...     surname: str
    ...     age: int
    >>>
    >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)
    >>> map_to(contact, Person)
    Person(first_name='Henry', second_name='Kaye', age=42)
 
-The ``dataclass-mapper`` library autogenerated some a mapper, that can be used with the ``map_to`` function.
+The ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.
 All we had to specify was the name of the target class, and optionally specify which fields map to which other fields.
 Notice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,
 all other fields were mapped automatically because the field names didn't change.
 
 And the ``dataclass-mapper`` library will perform a lot of checks around this mapping.
 It will check if the data types match, if some fields would be left uninitialized, etc.
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/assignments/list.py` & `dataclass_mapper-1.7.2/dataclass_mapper/assignments/list.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/assignments/recursive.py` & `dataclass_mapper-1.7.2/dataclass_mapper/assignments/recursive.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 class RecursiveAssignment(Assignment):
     def applicable(self) -> bool:
         return is_mappable_to(self.source.type, self.target.type) and not (
             self.source.allow_none and self.target.disallow_none
         )
 
     def right_side(self) -> str:
-        return self._get_map_func(
-            get_var_name(self.source), target_cls=self.target.type, extra_str=self.extra_str()
-        )
+        return self._get_map_func(get_var_name(self.source), target_cls=self.target.type, extra_str=self.extra_str())
 
     def extra_str(self) -> str:
         return f'extra.get("{self.target.name}", {{}})'
 
     def _get_map_func(self, name: str, target_cls: Any, extra_str: str) -> str:
         func_name = get_map_to_func_name(target_cls)
         return f"{name}.{func_name}({extra_str})"
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/assignments/utils.py` & `dataclass_mapper-1.7.2/dataclass_mapper/assignments/utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/classmeta.py` & `dataclass_mapper-1.7.2/dataclass_mapper/classmeta.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     DATACLASSES = auto()
     PYDANTIC = auto()
 
 
 class ClassMeta(ABC):
     _type: DataclassType
 
-    def __init__(
-        self, name: str, fields: Dict[str, FieldMeta], alias_name: Optional[str] = None
-    ) -> None:
+    def __init__(self, name: str, fields: Dict[str, FieldMeta], alias_name: Optional[str] = None) -> None:
         self.name = name
         self.fields = fields
         self.alias_name = alias_name or f"_{uuid4().hex}"
 
     @abstractmethod
     def return_statement(self) -> str:
         ...
@@ -41,16 +39,15 @@
     def get_assignment_name(self, field: FieldMeta) -> str:
         return field.name
 
     @staticmethod
     def _fields(clazz: Any, namespace: Namespace) -> Dict[str, FieldMeta]:
         real_types = get_type_hints(clazz, globalns=namespace.globals, localns=namespace.locals)
         return {
-            field.name: FieldMeta.from_dataclass(field, real_type=real_types[field.name])
-            for field in fields(clazz)
+            field.name: FieldMeta.from_dataclass(field, real_type=real_types[field.name]) for field in fields(clazz)
         }
 
     @classmethod
     def from_clazz(cls, clazz: Any, namespace: Namespace) -> "DataclassClassMeta":
         return cls(name=cast(str, clazz.__name__), fields=cls._fields(clazz, namespace))
 
 
@@ -67,19 +64,15 @@
     ) -> None:
         super().__init__(name=name, fields=fields, alias_name=alias_name)
         self.use_construct = use_construct
         self.allow_population_by_field_name = allow_population_by_field_name
 
     @staticmethod
     def has_validators(clazz: Any) -> bool:
-        return (
-            bool(clazz.__validators__)
-            or bool(clazz.__pre_root_validators__)
-            or bool(clazz.__post_root_validators__)
-        )
+        return bool(clazz.__validators__) or bool(clazz.__pre_root_validators__) or bool(clazz.__post_root_validators__)
 
     def return_statement(self) -> str:
         if self.use_construct:
             return f"    return {self.alias_name}.construct(**d)"
         else:
             return f"    return {self.alias_name}(**d)"
 
@@ -96,23 +89,24 @@
 
     @classmethod
     def from_clazz(cls, clazz: Any, namespace: Namespace) -> "PydanticClassMeta":
         return cls(
             name=cast(str, clazz.__name__),
             fields=cls._fields(clazz, namespace=namespace),
             use_construct=not cls.has_validators(clazz),
-            allow_population_by_field_name=getattr(
-                clazz.Config, "allow_population_by_field_name", False
-            ),
+            allow_population_by_field_name=getattr(clazz.Config, "allow_population_by_field_name", False),
         )
 
 
 def get_class_meta(cls: Any, namespace: Namespace) -> ClassMeta:
     if is_dataclass(cls):
         return DataclassClassMeta.from_clazz(cls, namespace=namespace)
     try:
         pydantic = __import__("pydantic")
         if issubclass(cls, pydantic.BaseModel):
             return PydanticClassMeta.from_clazz(cls, namespace=namespace)
     except ImportError:
         pass
+
+    if issubclass(cls, Enum):
+        raise ValueError("`mapper` does not support enum classes, use `enum_mapper` instead")
     raise NotImplementedError("only dataclasses and pydantic classes are supported")
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/enum.py` & `dataclass_mapper-1.7.2/dataclass_mapper/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 ) -> str:
     if isinstance(member, str) and member in members:
         return member
     if isinstance(member, enum_cls) and isinstance(member, Enum):
         return cast(str, member.name)  # in 3.11.0 .name is of type Any
 
     raise ValueError(
-        f"The mapping key '{member}' is must be a member of the {class_description} enum "
+        f"The mapping key '{member}' must be a member of the {class_description} enum "
         f"'{enum_cls.__name__}' or a string with its name"
     )
 
 
 def make_enum_mapper(
     mapping: EnumMapping,
     source_cls: Any,
     target_cls: Any,
 ) -> Callable:
-    assert issubclass(source_cls, Enum)
-    assert issubclass(target_cls, Enum)
+    if not issubclass(source_cls, Enum) or not issubclass(target_cls, Enum):
+        raise ValueError("`enum_mapper` does only support enum classes, use `mapper` for other classes")
 
     source_members = {member.name: member for member in source_cls}
     target_members = {member.name: member for member in target_cls}
 
     name_mapping: Dict[str, str] = {}
     for source_member, target_member in mapping.items():
         source_member = member_to_name_and_raise(source_member, source_members, source_cls, "source")
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/fieldmeta.py` & `dataclass_mapper-1.7.2/dataclass_mapper/fieldmeta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
-from dataclasses import MISSING
+from dataclasses import MISSING, dataclass
 from dataclasses import Field as DataclassField
-from dataclasses import dataclass
 from typing import Any, Optional, Union, cast, get_args, get_origin
 
 
 def is_union_type(type_: Any) -> bool:
     origin = get_origin(type_)
     if sys.version_info < (3, 10):
         return origin is Union
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/mapper.py` & `dataclass_mapper-1.7.2/dataclass_mapper/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,20 @@
     )
     module = import_module(SourceCls.__module__)
 
     d: Dict = {}
     setattr(SourceCls, "__zip_longest", zip_longest)
     # Support older versions of python by calling {**a, **b} rather than a|b
     exec(map_code, {**module.__dict__, **context}, d)
-    setattr(SourceCls, get_map_to_func_name(TargetCls), d["convert"])
+    map_func_name = get_map_to_func_name(TargetCls)
+    if hasattr(SourceCls, map_func_name):
+        raise AttributeError(
+            f"There already exists a mapping between '{SourceCls.__name__}' and '{TargetCls.__name__}'"
+        )
+    setattr(SourceCls, map_func_name, d["convert"])
     for name, factory in factories.items():
         setattr(SourceCls, name, factory)
 
 
 def enum_mapper(TargetCls: Any, mapping: Optional[EnumMapping] = None) -> Callable[[T], T]:
     """Class decorator that adds a private mapper method, that maps the current enum class to the
     enum class ``TargetCls``. The mapper method can be called using the ``map_to`` function.
@@ -237,15 +242,20 @@
 
 def add_enum_mapper_function(SourceCls: Any, TargetCls: Any, mapping: Optional[EnumMapping]) -> None:
     convert_function = make_enum_mapper(
         source_cls=SourceCls,
         target_cls=TargetCls,
         mapping=mapping or cast(EnumMapping, {}),
     )
-    setattr(SourceCls, get_map_to_func_name(TargetCls), convert_function)
+    map_func_name = get_map_to_func_name(TargetCls)
+    if hasattr(SourceCls, map_func_name):
+        raise AttributeError(
+            f"There already exists a mapping between '{SourceCls.__name__}' and '{TargetCls.__name__}'"
+        )
+    setattr(SourceCls, map_func_name, convert_function)
 
 
 def map_to(obj, TargetCls: Type[T], extra: Optional[Dict[str, Any]] = None) -> T:
     """Maps the given object to an object of type ``TargetCls``, if such a safe mapping was defined for the
     type of the given object.
     Raises an ``NotImplementedError`` if no such mapping is defined.
```

### Comparing `dataclass_mapper-1.7.1/dataclass_mapper/mapping_method.py` & `dataclass_mapper-1.7.2/dataclass_mapper/mapping_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from enum import Enum, auto
-from inspect import isfunction
 from typing import Callable, Dict, List, Optional, Type, Union
 
 from .assignments import (
     Assignment,
+    CallableWithMax1Parameter,
     FunctionAssignment,
     ListRecursiveAssignment,
     RecursiveAssignment,
     SimpleAssignment,
     get_var_name,
 )
 from .classmeta import ClassMeta, DataclassType
@@ -56,15 +56,15 @@
 # the different types that can be used as origin (source) for mapping to a member
 # - str: the name of a different variable in the original class
 # - Callable: a function that produces the value (can use `self` as parameter)
 # - Other.USE_DEFAULT/IGNORE_MISSING_MAPPING/init_with_default(): Don't map to this variable
 #   (only allowed if there is a default value/factory for it)
 # - assume_not_none(): assume that the source field is not None
 # - provide_with_extra(): create no mapping between the classes, fill the field with a dictionary called `extra`
-Origin = Union[str, Callable, Spezial, InitWithDefault, AssumeNotNone, ProvideWithExtra]
+Origin = Union[str, CallableWithMax1Parameter, Spezial, InitWithDefault, AssumeNotNone, ProvideWithExtra]
 StringFieldMapping = Dict[str, Origin]
 
 
 @dataclass
 class AssignmentOptions:
     """
     Options for creating an assignment code (target = right_side).
@@ -164,16 +164,18 @@
         return lines
 
     def _get_assignment_str(self, target: FieldMeta, right_side: str, indent: int = 4) -> str:
         variable_name = self.target_cls.get_assignment_name(target)
         return f'{" "*indent}d["{variable_name}"] = {right_side}'
 
     def add_mapping(self, target: FieldMeta, source: Union[FieldMeta, Callable]) -> None:
-        if isfunction(source):
-            function_assignment = FunctionAssignment(function=source, target=target, methods=self.methods)
+        if callable(source):
+            function_assignment = FunctionAssignment(
+                function=source, target=target, methods=self.methods, target_cls_name=self.target_cls.name
+            )
             right_side = function_assignment.right_side()
             self.lines.append(self._get_assignment_str(target, right_side))
         else:
             assert isinstance(source, FieldMeta)
 
             options = AssignmentOptions.from_Metas(
                 source_cls=self.source_cls, target_cls=self.target_cls, source=source, target=target
```

### Comparing `dataclass_mapper-1.7.1/pyproject.toml` & `dataclass_mapper-1.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-mapper"
-version = "1.7.1"
+version = "1.7.2"
 description = "Autogenerate mappings between dataclasses"
 authors = ["Jakob Kogler <jakob.kogler@gmail.com>"]
 
 readme = "README.rst"
 license = "MIT"
 
 repository = "https://github.com/dataclass-mapper/dataclass-mapper"
@@ -20,61 +20,65 @@
 pydantic = { version = "^1.9.0", optional = true }
 
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0.0"
-black = "^22.3.0"
-isort = "^5.10.1"
-mypy = "^0.950"
+black = "^23.3.0"
+mypy = "^1.3.0"
 tox = "^3.25.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.222"
+ruff = "^0.0.270"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
+select = [
+  # Pyflakes
+  "F",
+  # Pycodestyle
+  "E",
+  "W",
+  # flake8-pie
+  "PIE",
+  # isort
+  "I001",
+]
 line-length = 120
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-profile = "black"
-line_length = 120
-
 [tool.mypy]
+check_untyped_defs = true
 warn_return_any = true
 files = ["dataclass_mapper", "tests"]
 plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
 module = "pytest"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--doctest-glob \"*.rst\""
 filterwarnings = ["error"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "pragma: no cover",
-  "@abstractmethod"
-]
+exclude_lines = ["pragma: no cover", "@abstractmethod"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
```

### Comparing `dataclass_mapper-1.7.1/setup.py` & `dataclass_mapper-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 extras_require = \
 {'pydantic': ['pydantic>=1.9.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-mapper',
-    'version': '1.7.1',
+    'version': '1.7.2',
     'description': 'Autogenerate mappings between dataclasses',
-    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/main/graphs/badge.svg?branch=main\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=main\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses and Pydantic models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n\nSmall Example\n-------------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate with:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated some a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydanitc support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.\n',
+    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/main/graphs/badge.svg?branch=main\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=main\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses and Pydantic models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydanitc support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.\n',
     'author': 'Jakob Kogler',
     'author_email': 'jakob.kogler@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dataclass-mapper.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dataclass_mapper-1.7.1/PKG-INFO` & `dataclass_mapper-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-mapper
-Version: 1.7.1
+Version: 1.7.2
 Summary: Autogenerate mappings between dataclasses
 Home-page: https://dataclass-mapper.readthedocs.io
 License: MIT
 Keywords: dataclass,pydantic,python,automation
 Author: Jakob Kogler
 Author-email: jakob.kogler@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -94,16 +94,16 @@
 
 .. code-block:: bash
 
    pip install dataclass-mapper
    # or for Pydantic support
    pip install 'dataclass-mapper[pydantic]'
 
-Small Example
--------------
+Example
+-------
 
 We have the following target data structure, a class called ``Person``.
 
 .. code-block:: python
 
    >>> from dataclasses import dataclass
 
@@ -114,15 +114,15 @@
    ...     age: int
 
 
 We want to have a mapper from the source data structure, a class called ``ContactInfo``.
 Notice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.
 Other than that, all the attribute names are the same.
 
-Instead of writing a mapper function by hand, you can let it autogenerate with:
+Instead of writing a mapper function by hand, you can let it autogenerate one using this library:
 
 .. code-block:: python
 
    >>> from dataclass_mapper import map_to, mapper
    >>>
    >>> @mapper(Person, {"second_name": "surname"})
    ... @dataclass
@@ -131,15 +131,15 @@
    ...     surname: str
    ...     age: int
    >>>
    >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)
    >>> map_to(contact, Person)
    Person(first_name='Henry', second_name='Kaye', age=42)
 
-The ``dataclass-mapper`` library autogenerated some a mapper, that can be used with the ``map_to`` function.
+The ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.
 All we had to specify was the name of the target class, and optionally specify which fields map to which other fields.
 Notice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,
 all other fields were mapped automatically because the field names didn't change.
 
 And the ``dataclass-mapper`` library will perform a lot of checks around this mapping.
 It will check if the data types match, if some fields would be left uninitialized, etc.
```

