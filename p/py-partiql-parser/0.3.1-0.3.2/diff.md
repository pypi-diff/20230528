# Comparing `tmp/py-partiql-parser-0.3.1.tar.gz` & `tmp/py-partiql-parser-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.3.1.tar", last modified: Thu May 25 12:46:16 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.2.tar", last modified: Sun May 28 11:34:21 2023, max compression
```

## Comparing `py-partiql-parser-0.3.1.tar` & `py-partiql-parser-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.603204 py-partiql-parser-0.3.1/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.603204 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:46:16.000000 py-partiql-parser-0.3.1/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 12:46:06.000000 py-partiql-parser-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 12:46:16.611204 py-partiql-parser-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:46:16.607204 py-partiql-parser-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-25 12:45:51.000000 py-partiql-parser-0.3.1/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 11:34:14.000000 py-partiql-parser-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.1/LICENSE` & `py-partiql-parser-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/PKG-INFO` & `py-partiql-parser-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.1/README.md` & `py-partiql-parser-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/json_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,16 @@
         while True:
             c = tokenizer.next()
             if not c:
                 break
             if c == "{":
                 tokenizer.revert()  # Ensure we start the new parser with the initial {
                 result.append(self.parse(original, tokenizer, only_parse_initial=True))
+                if tokenizer.current() == "]":
+                    break
                 tokenizer.skip_until([","])
                 tokenizer.skip_white_space()
             elif c.isnumeric() and section is None:
                 result.append(int(c + tokenizer.next_until([",", "]"])))
                 current_phrase = ""
                 section = None
                 # Skip the comma, and any whitespace
@@ -196,8 +198,10 @@
         return result
 
 
 class SelectEncoder(JSONEncoder):
     def default(self, o):
         if isinstance(o, Variable) and o.value is None:
             return None
-        return o
+        if isinstance(o, CaseInsensitiveDict):
+            return dict(o.items())
+        return JSONEncoder.default(self, o)
```

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 
 from typing import Dict, Any, Union, List, AnyStr, Optional
 
 from .from_parser import FromParser
-from .json_parser import JsonParser
 from .select_parser import SelectParser
 from .where_parser import DynamoDBWhereParser, S3WhereParser, WhereParser
 from .utils import is_dict, QueryMetadata
 
 
 class Parser:
     RETURN_TYPE = Union[Dict[AnyStr, Any], List]
@@ -26,17 +25,17 @@
 
     def parse(self, query: str, parameters=None) -> List[Dict[str, Any]]:
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
         # First clause is whatever comes in front of SELECT - which should be nothing
         _ = clauses[0]
         # FROM
-        from_clauses = FromParser().parse(clauses[2])
-        source_data = self.documents[list(from_clauses.values())[0].lower()]
-        source_data = JsonParser().parse(source_data)
+        from_parser = FromParser()
+        from_clauses = from_parser.parse(clauses[2])
+        source_data = from_parser.get_source_data(self.documents)
         if is_dict(source_data):
             source_data = [source_data]  # type: ignore
 
         # WHERE
         if len(clauses) > 3:
             where_clause = clauses[3]
             source_data = self.where_parser(source_data).parse(where_clause, parameters)
```

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.3.2/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.3.2/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.1/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.3.2/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 py_partiql_parser/_internal/parser.py
 py_partiql_parser/_internal/select_parser.py
 py_partiql_parser/_internal/utils.py
 py_partiql_parser/_internal/where_parser.py
 tests/test_csv_converter.py
 tests/test_dynamodb_examples.py
 tests/test_from_parser.py
+tests/test_json_encoder.py
 tests/test_json_parser.py
 tests/test_query_metadata.py
 tests/test_s3_examples.py
 tests/test_select_functions.py
 tests/test_select_parser.py
 tests/test_utils.py
 tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.1/tests/test_csv_converter.py` & `py-partiql-parser-0.3.2/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.3.2/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_from_parser.py` & `py-partiql-parser-0.3.2/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_json_parser.py` & `py-partiql-parser-0.3.2/tests/test_json_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import sure  # noqa
+import pytest
 from py_partiql_parser._internal.json_parser import JsonParser, Variable
 
 
 def test_static_value():
     JsonParser().parse("a").should.equal(Variable("a"))
 
 
@@ -94,7 +95,19 @@
 {"a3": "z"
 }
     
     """
     JsonParser().parse(multi_object_string).should.equal(
         [{"a1": "v1", "a1": "v2"}, {"a2": "w1", "a2": "w2"}, {"a3": "z"}]
     )
+
+
+@pytest.mark.parametrize(
+    "source",
+    [
+        [{"staff": [{"name": "J M"}], "country": "USA"}],
+        {"staff": [{"name": "J M"}], "country": "USA"},
+        [{"staff": [{"name": "J M"}, {"name": "M, J"}], "country": "USA"}],
+    ],
+)
+def test_list_and_string_are_siblings(source):
+    assert JsonParser().parse(json.dumps(source)) == source
```

### Comparing `py-partiql-parser-0.3.1/tests/test_query_metadata.py` & `py-partiql-parser-0.3.2/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_s3_examples.py` & `py-partiql-parser-0.3.2/tests/test_s3_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import pytest
 import sure  # noqa
-from py_partiql_parser import S3SelectParser, SelectEncoder
-from . import input_json_list, json_as_lines
+from py_partiql_parser import S3SelectParser
+from . import input_json_list, json_as_lines, input_with_lists
 
 
 # https://aws.amazon.com/blogs/storage/querying-data-without-servers-or-databases-using-amazon-s3-select/
 
 
 input_data_csv = """Name,PhoneNumber,City,Occupation
 Sam,(949) 555-6701,Irvine,Solutions Architect
@@ -161,21 +161,15 @@
     )
     parser = S3SelectParser(source_data={"s3object": all_rows})
     assert parser.parse(query, parameters=None) == [
         {"Name": "Vinod", "City": "Los Angeles"}
     ]
 
 
-def test_json_output_can_be_dumped():
-    query = "select * from s3object s"
-    input_with_none = json.dumps(
-        [
-            {
-                "name": "Janelyn M",
-                "date": "2020-02-23T00:00:00",
-                "city": "Chicago",
-                "kids": None,
-            },
-        ]
-    )
-    result = S3SelectParser(source_data={"s3object": input_with_none}).parse(query)
-    assert input_with_none == json.dumps(result, cls=SelectEncoder)
+def test_select_root_objects():
+    query = "select * from s3object[*].staff[*] s"
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_with_lists)}
+    ).parse(query)
+    assert len(result) == 2
+    assert input_with_lists[0]["staff"][0] in result
+    assert input_with_lists[0]["staff"][1] in result
```

### Comparing `py-partiql-parser-0.3.1/tests/test_select_functions.py` & `py-partiql-parser-0.3.2/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_select_parser.py` & `py-partiql-parser-0.3.2/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_utils.py` & `py-partiql-parser-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.1/tests/test_where_parser.py` & `py-partiql-parser-0.3.2/tests/test_where_parser.py`

 * *Files identical despite different names*

