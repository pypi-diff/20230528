# Comparing `tmp/databind.core-4.2.7.tar.gz` & `tmp/databind.core-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.7.tar", max compression
+gzip compressed data, was "databind.core-4.2.8.tar", max compression
```

## Comparing `databind.core-4.2.7.tar` & `databind.core-4.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1724 2023-05-28 04:15:23.442454 databind.core-4.2.7/pyproject.toml
--rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.7/readme.md
--rw-r--r--   0        0        0       22 2023-05-28 04:15:23.442454 databind.core-4.2.7/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-05-28 03:24:09.913921 databind.core-4.2.7/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/py.typed
--rw-r--r--   0        0        0    15319 2023-05-28 04:14:21.356217 databind.core-4.2.7/src/databind/core/schema.py
--rw-r--r--   0        0        0    26830 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-05-28 03:24:09.917921 databind.core-4.2.7/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-05-28 04:15:29.082090 databind.core-4.2.7/setup.py
--rw-r--r--   0        0        0     2343 2023-05-28 04:15:29.082365 databind.core-4.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1724 2023-05-28 04:19:55.966712 databind.core-4.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1245 2022-11-06 01:30:31.114677 databind.core-4.2.8/readme.md
+-rw-r--r--   0        0        0       22 2023-05-28 04:19:55.970711 databind.core-4.2.8/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-05-28 03:24:09.913921 databind.core-4.2.8/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15319 2023-05-28 04:14:21.356217 databind.core-4.2.8/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26836 2023-05-28 04:18:51.936531 databind.core-4.2.8/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-05-28 03:24:09.917921 databind.core-4.2.8/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-05-28 04:20:01.628756 databind.core-4.2.8/setup.py
+-rw-r--r--   0        0        0     2343 2023-05-28 04:20:01.628966 databind.core-4.2.8/PKG-INFO
```

### Comparing `databind.core-4.2.7/pyproject.toml` & `databind.core-4.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.7"
+version = "4.2.8"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind.core-4.2.7/readme.md` & `databind.core-4.2.8/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/context.py` & `databind.core-4.2.8/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/converter.py` & `databind.core-4.2.8/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/dataclasses.py` & `databind.core-4.2.8/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/dataclasses.pyi` & `databind.core-4.2.8/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/mapper.py` & `databind.core-4.2.8/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/schema.py` & `databind.core-4.2.8/src/databind/core/schema.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/settings.py` & `databind.core-4.2.8/src/databind/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
     nesting_key: t.Optional[str] = None
 
     def __init__(
         self,
         members: t.Union[
             "UnionMembers",
             "StaticUnionMembers._MembersMappingType",
-            "t.List[UnionMembers | StaticUnionMembers._MembersMappingType]",
+            "t.List[UnionMembers | str | StaticUnionMembers._MembersMappingType]",
             str,
             None,
         ] = None,
         style: str = NESTED,
         discriminator_key: str = "type",
         nesting_key: t.Optional[str] = None,
     ) -> None:
```

### Comparing `databind.core-4.2.7/src/databind/core/union.py` & `databind.core-4.2.8/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/src/databind/core/utils.py` & `databind.core-4.2.8/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.7/setup.py` & `databind.core-4.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.7',
+    'version': '4.2.8',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.7/PKG-INFO` & `databind.core-4.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.7
+Version: 4.2.8
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

