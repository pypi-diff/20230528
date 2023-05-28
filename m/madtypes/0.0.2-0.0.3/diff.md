# Comparing `tmp/madtypes-0.0.2.tar.gz` & `tmp/madtypes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.2.tar", last modified: Sat May 27 09:19:48 2023, max compression
+gzip compressed data, was "madtypes-0.0.3.tar", last modified: Sun May 28 09:22:18 2023, max compression
```

## Comparing `madtypes-0.0.2.tar` & `madtypes-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 09:19:48.574770 madtypes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-27 09:19:36.000000 madtypes-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.570770 madtypes-0.0.2/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-27 09:19:36.000000 madtypes-0.0.2/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:19:48.574770 madtypes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-27 09:19:36.000000 madtypes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-27 09:19:36.000000 madtypes-0.0.2/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-28 09:22:18.951303 madtypes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-28 09:22:08.000000 madtypes-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-28 09:22:08.000000 madtypes-0.0.3/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 09:22:18.951303 madtypes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-28 09:22:08.000000 madtypes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-05-28 09:22:08.000000 madtypes-0.0.3/tests/test_schema.py
```

### Comparing `madtypes-0.0.2/setup.py` & `madtypes-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.2",
+    version="0.0.3",
     author="6r17",
     author_email="patrick.borowy@proton.me",
-    description="Python typing that will raise TypeError at runtime",
+    description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
     keywords=["typing", "json", "json-schema"],
     python_requires=">=3.9",
     classifiers=[
```

### Comparing `madtypes-0.0.2/tests/test_schema.py` & `madtypes-0.0.3/tests/test_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from madtypes import schema, Schema, Annotation
+from typing import Optional
+from madtypes import schema, Schema, Annotation, Immutable
 import pytest
 
 
 class Gender(Schema):
     female: int
     male: int
 
@@ -28,15 +29,15 @@
     a = Item(name="foo", gender=Gender(female=10, male=20))
     print(a)
     assert a.name == "foo"
     assert a["name"] == "foo"
 
 
 def test_attribute_set():
-    a = Item()
+    a = Item(name="bar", gender=Gender(female=10, male=20))
     a.name = "foo"
     assert a.name == "foo"
     assert a["name"] == "foo"
 
 
 def test_json_dumps():
     import json
@@ -54,21 +55,19 @@
 
     a = Item(name="foo", gender=Gender(female=10, male=20))
     print(a)
     assert json.loads(json.dumps(a)) == a
 
 
 def test_set():
-    a = Item()
-    with pytest.raises(AttributeError):
-        a.gender.male = 20
-    a.gender = Gender()
-    a.gender.male = 20
-    print(a)
-    assert a.gender.male == 20
+    a = Item(name="bob", gender=Gender(male=20, female=30))
+    a.gender = Gender(male=30, female=10)
+    assert a.gender.male == 30
+    with pytest.raises(TypeError):
+        a.gender.male = "foo"
 
 
 def test_int():
     assert schema(int) == {"type": "integer"}
 
 
 def test_array():
@@ -85,62 +84,72 @@
 def test_object():
     class Item(Schema):
         name: str
 
     assert schema(Item) == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
+        "required": ["name"],
     }
 
 
 def test_array_of_object():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         items: list[Item]
 
-    assert schema(Basket) == {
+    schem = schema(Basket)
+    print(schem)
+    assert schem == {
         "type": "object",
         "properties": {
             "items": {
                 "type": "array",
                 "items": {
                     "type": "object",
                     "properties": {"name": {"type": "string"}},
+                    "required": ["name"],
                 },
             }
         },
+        "required": ["items"],
     }
 
 
 def test_tuple_of_object():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         some_items: tuple[Item, Item]
 
-    assert schema(Basket) == {
+    schem = schema(Basket)
+    print(schem)
+    assert schem == {
         "type": "object",
         "properties": {
             "some_items": {
                 "type": "array",
                 "items": [
                     {
                         "type": "object",
                         "properties": {"name": {"type": "string"}},
+                        "required": ["name"],
                     },
                     {
                         "type": "object",
                         "properties": {"name": {"type": "string"}},
+                        "required": ["name"],
                     },
                 ],
             }
         },
+        "required": ["some_items"],
     }
 
 
 def test_json_schema():
     print(schema(Item))
     assert schema(Item) == {
         "type": "object",
@@ -148,16 +157,18 @@
             "name": {"type": "string"},
             "gender": {
                 "type": "object",
                 "properties": {
                     "female": {"type": "integer"},
                     "male": {"type": "integer"},
                 },
+                "required": ["female", "male"],
             },
         },
+        "required": ["name", "gender"],
     }
 
 
 class DescriptedString(Annotation):
     description = "Some description"
     annotation = str
 
@@ -172,27 +183,29 @@
         "type": "object",
         "properties": {
             "descripted": {
                 "type": "string",
                 "description": "Some description",
             },
         },
+        "required": ["descripted"],
     }
 
 
 class PrimitiveArray(Schema):
     items: list[str]
 
 
 def test_annotation_array():
     assert schema(PrimitiveArray) == {
         "type": "object",
         "properties": {
             "items": {"type": "array", "items": {"type": "string"}}
         },
+        "required": ["items"],
     }
 
 
 class PrimitiveDescriptiveArray(Annotation):
     annotation = list[int]
     description = "some description"
 
@@ -209,14 +222,15 @@
         "properties": {
             "descripted_array": {
                 "type": "array",
                 "items": {"type": "integer"},
                 "description": "some description",
             },
         },
+        "required": ["descripted_array"],
     }
 
 
 class Person(Schema):
     name: str
 
 
@@ -231,17 +245,19 @@
         "type": "object",
         "properties": {
             "persons": {
                 "type": "array",
                 "items": {
                     "type": "object",
                     "properties": {"name": {"type": "string"}},
+                    "required": ["name"],
                 },
             }
         },
+        "required": ["persons"],
     }
 
 
 class DescriptiveName(Annotation):
     annotation = str
     description = "How you'd call the beer"
 
@@ -262,27 +278,29 @@
 def test_descriptive_object_array():
     result = schema(ObjectDescriptedArray)
     print(result)
     assert result == {
         "type": "object",
         "properties": {
             "descripted_array": {
+                "description": "Lots of beers",
                 "type": "array",
                 "items": {
                     "type": "object",
                     "properties": {
                         "name": {
-                            "type": "string",
                             "description": "How you'd call the beer",
+                            "type": "string",
                         }
                     },
+                    "required": ["name"],
                 },
-                "description": "Lots of beers",
-            },
+            }
         },
+        "required": ["descripted_array"],
     }
 
 
 class PrimitiveTuple(Schema):
     tupled: tuple[int, str]
 
 
@@ -293,41 +311,40 @@
         "type": "object",
         "properties": {
             "tupled": {
                 "type": "array",
                 "items": [{"type": "integer"}, {"type": "string"}],
             }
         },
+        "required": ["tupled"],
     }
 
 
 def test_type_error():
     class Item(Schema):
         value: int
 
-    e = Item()
     with pytest.raises(TypeError):
-        e.value = "foo"
+        Item(value="foo")
 
 
 def test_instantiation_type_error():
     class Item(Schema):
         value: int
 
     with pytest.raises(TypeError):
         Item(value="foo")  # any easy way to enable linter here ?
 
 
 def test_complex_type_error():
     class Item(Schema):
         value: list[int]
 
-    e = Item()
     with pytest.raises(TypeError):
-        e.value = ["str", "str"]
+        Item(value=["str", "str"])
 
 
 def test_schemas_are_reprable():
     class Item(Schema):
         value: str
 
     e = Item(value="test")
@@ -336,7 +353,75 @@
 
 def test_schemas_expect_types():
     class Item(Schema):
         value: "str"
 
     with pytest.raises(SyntaxError):
         schema(Item)
+
+
+def test_immutable():
+    class SomeImmutable(Immutable):
+        name: str
+
+    e = SomeImmutable(name="foo")
+    with pytest.raises(TypeError):
+        e.name = "bar"
+
+    with pytest.raises(TypeError):
+        e["name"] = "bar"
+
+
+def test_copy():
+    class SomeImmutable(Immutable):
+        name: str
+        age: int
+
+    with pytest.raises(TypeError):
+        a = SomeImmutable(name="foo")  # missing age
+
+    class AnotherImmutable(Immutable):
+        name: str
+        age: Optional[int]
+
+    a = AnotherImmutable(name="foo")
+    b = AnotherImmutable(**a)
+    assert b.name == "foo"
+    c = SomeImmutable(age=2, **a)
+    assert c.name == "foo"
+    assert c.age == 2
+
+
+def test_custom_method():
+    class SomeClass(Schema):
+        name: str
+
+        def method(self) -> str:
+            return self.name
+
+    assert SomeClass(name="foo").method() == "foo"
+
+
+def test_optional_json_schema():
+    class SomeClassWithOptional(Schema):
+        name: Optional[str]
+
+    SomeClassWithOptional()
+    schem = schema(SomeClassWithOptional)
+    assert schem == {
+        "type": "object",
+        "properties": {"name": {"type": "string"}},
+    }
+
+
+def test_optional_json_schema_with_array():
+    class SomeClassWithOptional(Schema):
+        elements: Optional[list[int]]
+
+    SomeClassWithOptional()
+    schem = schema(SomeClassWithOptional)
+    assert schem == {
+        "type": "object",
+        "properties": {
+            "elements": {"type": "array", "items": {"type": "integer"}}
+        },
+    }
```

