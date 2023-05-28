# Comparing `tmp/databind.core-4.2.6.tar.gz` & `tmp/databind.core-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.6.tar", max compression
+gzip compressed data, was "databind.core-4.2.7.tar", max compression
```

## Comparing `databind.core-4.2.6.tar` & `databind.core-4.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1724 2023-05-28 03:23:44.422647 databind.core-4.2.6/pyproject.toml
--rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.6/readme.md
--rw-r--r--   0        0        0       22 2023-05-28 03:23:44.422647 databind.core-4.2.6/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-05-28 02:51:13.242265 databind.core-4.2.6/src/databind/core/py.typed
--rw-r--r--   0        0        0    15324 2023-05-28 03:22:02.793541 databind.core-4.2.6/src/databind/core/schema.py
--rw-r--r--   0        0        0    26830 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-05-28 03:01:35.968571 databind.core-4.2.6/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-05-28 03:23:50.841356 databind.core-4.2.6/setup.py
--rw-r--r--   0        0        0     2343 2023-05-28 03:23:50.841568 databind.core-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1724 2023-05-28 04:15:23.442454 databind.core-4.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.7/readme.md
+-rw-r--r--   0        0        0       22 2023-05-28 04:15:23.442454 databind.core-4.2.7/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15319 2023-05-28 04:14:21.356217 databind.core-4.2.7/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26830 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-05-28 04:15:29.082090 databind.core-4.2.7/setup.py
+-rw-r--r--   0        0        0     2343 2023-05-28 04:15:29.082365 databind.core-4.2.7/PKG-INFO
```

### Comparing `databind.core-4.2.6/pyproject.toml` & `databind.core-4.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.6"
+version = "4.2.7"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind.core-4.2.6/readme.md` & `databind.core-4.2.7/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/context.py` & `databind.core-4.2.7/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/converter.py` & `databind.core-4.2.7/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/dataclasses.py` & `databind.core-4.2.7/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/dataclasses.pyi` & `databind.core-4.2.7/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/mapper.py` & `databind.core-4.2.7/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/schema.py` & `databind.core-4.2.7/src/databind/core/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,22 +201,21 @@
     }
 
     # Collect the members from the dataclass and its base classes.
     queue = [hint]
     fields: t.Dict[str, Field] = {}
     while queue:
         hint = queue.pop(0)
+        parameter_map = hint.get_parameter_map()
 
         if hint.type in eval_context_by_type:
             # Make sure forward references are resolved.
             hint = hint.evaluate(eval_context_by_type[hint.type])  # type: ignore[assignment]
             assert isinstance(hint, ClassTypeHint)
 
-            parameter_map = hint.get_parameter_map()
-
             for field in dataclasses.fields(hint.type):
                 if not field.init:
                     # If we cannot initialize the field in the constructor, we should also
                     # exclude it from the definition of the type for de-/serializing.
                     continue
                 if field.name in fields:
                     # Subclasses override their parent's fields.
```

### Comparing `databind.core-4.2.6/src/databind/core/settings.py` & `databind.core-4.2.7/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/union.py` & `databind.core-4.2.7/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/src/databind/core/utils.py` & `databind.core-4.2.7/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.6/setup.py` & `databind.core-4.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.6',
+    'version': '4.2.7',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.6/PKG-INFO` & `databind.core-4.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.6
+Version: 4.2.7
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

