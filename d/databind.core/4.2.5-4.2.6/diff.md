# Comparing `tmp/databind.core-4.2.5.tar.gz` & `tmp/databind.core-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.5.tar", max compression
+gzip compressed data, was "databind.core-4.2.6.tar", max compression
```

## Comparing `databind.core-4.2.5.tar` & `databind.core-4.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1727 2023-04-29 16:35:15.655751 databind.core-4.2.5/pyproject.toml
--rw-r--r--   0        0        0     1245 2023-04-29 16:34:38.888783 databind.core-4.2.5/readme.md
--rw-r--r--   0        0        0       22 2023-04-29 16:35:15.655751 databind.core-4.2.5/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/py.typed
--rw-r--r--   0        0        0    15234 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/schema.py
--rw-r--r--   0        0        0    26830 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-04-29 16:35:23.687455 databind.core-4.2.5/setup.py
--rw-r--r--   0        0        0     2343 2023-04-29 16:35:23.687663 databind.core-4.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1724 2023-05-28 03:23:44.422647 databind.core-4.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.6/readme.md
+-rw-r--r--   0        0        0       22 2023-05-28 03:23:44.422647 databind.core-4.2.6/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-05-28 02:51:13.242265 databind.core-4.2.6/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15324 2023-05-28 03:22:02.793541 databind.core-4.2.6/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26830 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-05-28 03:23:50.841356 databind.core-4.2.6/setup.py
+-rw-r--r--   0        0        0     2343 2023-05-28 03:23:50.841568 databind.core-4.2.6/PKG-INFO
```

### Comparing `databind.core-4.2.5/pyproject.toml` & `databind.core-4.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.5"
+version = "4.2.6"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
@@ -25,15 +25,15 @@
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
 mypy = "*"
 types-dataclasses = "*"
 types-deprecated = "*"
-types-pkg_resources = "*"
+types-setuptools = "*"
 types-termcolor = "*"
 
 [tool.slap]
 typed = true
 
 [build-system]
 requires = ["poetry-core==1.0.8"]
```

### Comparing `databind.core-4.2.5/readme.md` & `databind.core-4.2.6/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/context.py` & `databind.core-4.2.6/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/converter.py` & `databind.core-4.2.6/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/dataclasses.py` & `databind.core-4.2.6/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/dataclasses.pyi` & `databind.core-4.2.6/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/mapper.py` & `databind.core-4.2.6/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/schema.py` & `databind.core-4.2.6/src/databind/core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,63 +196,61 @@
 
     # Retrieve the context in which type hints from each field origin type need to be
     # evaluated.
     eval_context_by_type: t.Dict[type, t.Mapping[str, t.Any]] = {
         type_: vars(sys.modules[type_.__module__]) for type_ in set(field_origin.values())
     }
 
-    # import pdb; pdb.set_trace()
-
     # Collect the members from the dataclass and its base classes.
     queue = [hint]
     fields: t.Dict[str, Field] = {}
     while queue:
         hint = queue.pop(0)
 
-        if hint.type not in eval_context_by_type:
+        if hint.type in eval_context_by_type:
+            # Make sure forward references are resolved.
+            hint = hint.evaluate(eval_context_by_type[hint.type])  # type: ignore[assignment]
+            assert isinstance(hint, ClassTypeHint)
+
+            parameter_map = hint.get_parameter_map()
+
+            for field in dataclasses.fields(hint.type):
+                if not field.init:
+                    # If we cannot initialize the field in the constructor, we should also
+                    # exclude it from the definition of the type for de-/serializing.
+                    continue
+                if field.name in fields:
+                    # Subclasses override their parent's fields.
+                    continue
+                if field_origin[field.name] != hint.type:
+                    # If this field does not belong to the current type
+                    continue
+
+                field_hint = TypeHint(field.type, field_origin[field.name]).evaluate().parameterize(parameter_map)
+
+                # NOTE(NiklasRosenstein): In Python 3.6, Mypy complains about "Callable does not accept self argument",
+                #       but we also cannot ignore it because of warn_unused_ignores.
+                _field_default_factory = getattr(field, "default_factory")
+
+                default = NotSet.Value if field.default == MISSING else field.default
+                default_factory = NotSet.Value if _field_default_factory == MISSING else _field_default_factory
+                has_default = default != NotSet.Value or default_factory != NotSet.Value
+                required = _is_required(field_hint, not has_default)
+
+                fields[field.name] = Field(
+                    datatype=field_hint,
+                    required=required,
+                    default=None if not required and not has_default else default,
+                    default_factory=default_factory,
+                    flattened=_is_flat(field_hint, False),
+                )
+        else:
             # This could mean that a base class is a dataclass but all of its members
             # are overwritten by other fields.
-            continue
-
-        # Make sure forward references are resolved.
-        hint = hint.evaluate(eval_context_by_type[hint.type])  # type: ignore[assignment]
-        assert isinstance(hint, ClassTypeHint)
-
-        parameter_map = hint.get_parameter_map()
-
-        for field in dataclasses.fields(hint.type):
-            if not field.init:
-                # If we cannot initialize the field in the constructor, we should also
-                # exclude it from the definition of the type for de-/serializing.
-                continue
-            if field.name in fields:
-                # Subclasses override their parent's fields.
-                continue
-            if field_origin[field.name] != hint.type:
-                # If this field does not belong to the current type
-                continue
-
-            field_hint = TypeHint(field.type, field_origin[field.name]).evaluate().parameterize(parameter_map)
-
-            # NOTE(NiklasRosenstein): In Python 3.6, Mypy complains about "Callable does not accept self argument",
-            #       but we also cannot ignore it because of warn_unused_ignores.
-            _field_default_factory = getattr(field, "default_factory")
-
-            default = NotSet.Value if field.default == MISSING else field.default
-            default_factory = NotSet.Value if _field_default_factory == MISSING else _field_default_factory
-            has_default = default != NotSet.Value or default_factory != NotSet.Value
-            required = _is_required(field_hint, not has_default)
-
-            fields[field.name] = Field(
-                datatype=field_hint,
-                required=required,
-                default=None if not required and not has_default else default,
-                default_factory=default_factory,
-                flattened=_is_flat(field_hint, False),
-            )
+            pass
 
         # Continue with the base classes.
         for base in hint.bases or hint.type.__bases__:
             base_hint = TypeHint(base).parameterize(parameter_map)
             assert isinstance(base_hint, ClassTypeHint), f"nani? {base_hint}"
             if dataclasses.is_dataclass(base_hint.type):
                 queue.append(base_hint)
```

### Comparing `databind.core-4.2.5/src/databind/core/settings.py` & `databind.core-4.2.6/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/union.py` & `databind.core-4.2.6/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/src/databind/core/utils.py` & `databind.core-4.2.6/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.5/setup.py` & `databind.core-4.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.5',
+    'version': '4.2.6',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.5/PKG-INFO` & `databind.core-4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.5
+Version: 4.2.6
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

