# Comparing `tmp/jsonfmt-0.2.2.tar.gz` & `tmp/jsonfmt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.2.tar", last modified: Fri May 26 06:14:42 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.3.tar", last modified: Sun May 28 15:24:21 2023, max compression
```

## Comparing `jsonfmt-0.2.2.tar` & `jsonfmt-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 06:14:42.000000 jsonfmt-0.2.2/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     7955 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:14:42.152842 jsonfmt-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-26 06:14:24.000000 jsonfmt-0.2.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:24:21.855527 jsonfmt-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 15:24:04.000000 jsonfmt-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-28 15:24:21.855527 jsonfmt-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-28 15:24:04.000000 jsonfmt-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:24:21.855527 jsonfmt-0.2.3/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 15:24:21.000000 jsonfmt-0.2.3/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-05-28 15:24:04.000000 jsonfmt-0.2.3/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-28 15:24:04.000000 jsonfmt-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:24:21.855527 jsonfmt-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:24:21.855527 jsonfmt-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-05-28 15:24:04.000000 jsonfmt-0.2.3/test/test.py
```

### Comparing `jsonfmt-0.2.2/LICENSE` & `jsonfmt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.2/PKG-INFO` & `jsonfmt-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
 Keywords: json,formatter,pretty-print,highlight,jsonpath
@@ -36,17 +36,17 @@
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
 1. [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
 2. [Minimize JSON to a single line.](#2-minimize-the-json-object)
-3. [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
-4. [Format JSON to TOML or YAML.](#4-format-json-to-toml-or-yaml)
-5. [Convert between other formats.](#5-convert-between-json-toml-and-yaml-formats)
+3. [Pick out parts from a large JSON via jsonpath.](#3-pick-out-parts-of-a-large-json-via-jsonpath)
+4. [Format JSON to TOML or YAML.](#4-format-json-as-toml-or-yaml)
+5. [Conversion between these three formats.](#5-conversion-between-json-toml-and-yaml-formats)
 6. [Copy the result to clipboard.](#6-copy-the-result-to-clipboard)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
@@ -142,52 +142,59 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 3. Use jsonpath to match part of the object.
+### 3. Pick out parts of a large JSON via JSONPath.
 
-**jsonfmt** uses a simplified jsonpath syntax.
+**JSONPath** is a way to query the sub-elements of a JSON document.
 
-- It matches JSON objects starting from the root node.
+It likes the XPath for xml, which can extract part of the content of a given JSON document through a simple syntax.
 
-- You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+JSONPath syntax reference <https://goessner.net/articles/JsonPath/> and <https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html>
+
+Some examples:
+
+- pick out the first actions in `example.json`
 
     ```shell
-    $ jsonfmt -p 'actions/0' test/example.json
+    $ jsonfmt -p '$.actions[0]' test/example.json
     ```
 
     *Output:*
 
     ```json
-    {
-        "calorie": 294.9,
-        "date": "2021-03-02",
-        "name": "eat"
-    }
+    [
+        {
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
+        }
+    ]
     ```
 
-- If you want to match all items in a list, just use `*` to match.
+- Filters all occurrences of the `name` field in the JSON.
 
     ```shell
-    $ jsonfmt -p 'actions/*/name' test/example.json
+    $ jsonfmt -p '$..name' test/example.json
     ```
 
     *Output:*
 
     ```json
     [
+        "Bob",
         "eat",
         "sport"
     ]
     ```
 
-### 4. Format JSON to TOML or YAML.
+### 4. Format JSON as TOML or YAML.
 
 ```shell
 $ jsonfmt test/example.json -f toml
 ```
 
 *Output:*
 
@@ -203,15 +210,15 @@
 
 [[actions]]
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
-### 5. Convert between JSON, TOML and YAML formats.
+### 5. Conversion between JSON, TOML and YAML formats.
 
 <div style="color: orange"><strong>Note this:</strong></div>
 The `null` value is invalid in TOML. Therefore, any null values in JSON or YAML will be removed when converting to TOML.
 
 ```shell
 # json to yaml
 $ jsonfmt test/example.json -f yaml
@@ -235,15 +242,15 @@
 Once you've done the above, you can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
 
 <div style="color: orange"><strong>Note these:</strong></div>
 
 - When you specify the `-C` option, any output destination other than the clipboard will be ignored.
 - When you process multiple files, only the last result will be preserved in the clipboard.
 
-### 7. Other usages
+### 7. Output to file.
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
 ```
```

### Comparing `jsonfmt-0.2.2/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.2.3/jsonfmt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
 Keywords: json,formatter,pretty-print,highlight,jsonpath
@@ -36,17 +36,17 @@
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
 1. [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
 2. [Minimize JSON to a single line.](#2-minimize-the-json-object)
-3. [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
-4. [Format JSON to TOML or YAML.](#4-format-json-to-toml-or-yaml)
-5. [Convert between other formats.](#5-convert-between-json-toml-and-yaml-formats)
+3. [Pick out parts from a large JSON via jsonpath.](#3-pick-out-parts-of-a-large-json-via-jsonpath)
+4. [Format JSON to TOML or YAML.](#4-format-json-as-toml-or-yaml)
+5. [Conversion between these three formats.](#5-conversion-between-json-toml-and-yaml-formats)
 6. [Copy the result to clipboard.](#6-copy-the-result-to-clipboard)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
@@ -142,52 +142,59 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 3. Use jsonpath to match part of the object.
+### 3. Pick out parts of a large JSON via JSONPath.
 
-**jsonfmt** uses a simplified jsonpath syntax.
+**JSONPath** is a way to query the sub-elements of a JSON document.
 
-- It matches JSON objects starting from the root node.
+It likes the XPath for xml, which can extract part of the content of a given JSON document through a simple syntax.
 
-- You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+JSONPath syntax reference <https://goessner.net/articles/JsonPath/> and <https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html>
+
+Some examples:
+
+- pick out the first actions in `example.json`
 
     ```shell
-    $ jsonfmt -p 'actions/0' test/example.json
+    $ jsonfmt -p '$.actions[0]' test/example.json
     ```
 
     *Output:*
 
     ```json
-    {
-        "calorie": 294.9,
-        "date": "2021-03-02",
-        "name": "eat"
-    }
+    [
+        {
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
+        }
+    ]
     ```
 
-- If you want to match all items in a list, just use `*` to match.
+- Filters all occurrences of the `name` field in the JSON.
 
     ```shell
-    $ jsonfmt -p 'actions/*/name' test/example.json
+    $ jsonfmt -p '$..name' test/example.json
     ```
 
     *Output:*
 
     ```json
     [
+        "Bob",
         "eat",
         "sport"
     ]
     ```
 
-### 4. Format JSON to TOML or YAML.
+### 4. Format JSON as TOML or YAML.
 
 ```shell
 $ jsonfmt test/example.json -f toml
 ```
 
 *Output:*
 
@@ -203,15 +210,15 @@
 
 [[actions]]
 calorie = -375
 date = "2023-04-27"
 name = "sport"
 ```
 
-### 5. Convert between JSON, TOML and YAML formats.
+### 5. Conversion between JSON, TOML and YAML formats.
 
 <div style="color: orange"><strong>Note this:</strong></div>
 The `null` value is invalid in TOML. Therefore, any null values in JSON or YAML will be removed when converting to TOML.
 
 ```shell
 # json to yaml
 $ jsonfmt test/example.json -f yaml
@@ -235,15 +242,15 @@
 Once you've done the above, you can then use <kbd>ctrl</kbd>+<kbd>v</kbd> or <kbd>cmd</kbd>+<kbd>v</kbd> to paste the result anywhere on your computer.
 
 <div style="color: orange"><strong>Note these:</strong></div>
 
 - When you specify the `-C` option, any output destination other than the clipboard will be ignored.
 - When you process multiple files, only the last result will be preserved in the clipboard.
 
-### 7. Other usages
+### 7. Output to file.
 
 - use the `-O` parameter to overwrite the file with the result.
 
 ```shell
 $ jsonfmt -O test/example.json
 ```
```

### Comparing `jsonfmt-0.2.2/jsonfmt.py` & `jsonfmt-0.2.3/jsonfmt.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,97 +3,69 @@
 
 import json
 import pyperclip
 import toml
 import yaml
 from argparse import ArgumentParser
 from functools import partial
+from jsonpath import jsonpath
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
 from sys import stdin, stdout, stderr, exit
-from typing import Any, List, IO, Optional, Sequence, Union
+from typing import Any, IO, Optional, Sequence
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 
-def print_inf(msg: str):
+def print_inf(msg: Any):
     print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m', file=stdout)
 
 
-def print_err(msg: str):
+def print_err(msg: Any):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
-class JSONPathError(Exception):
-    pass
-
-
 class ParseError(Exception):
     pass
 
 
 def is_clipboard_available() -> bool:
     copy_fn, paste_fn = pyperclip.determine_clipboard()
     return copy_fn.__class__.__name__ != 'ClipboardUnavailable' \
         and paste_fn.__class__.__name__ != 'ClipboardUnavailable'
 
 
-def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
-    '''parse the jsonpath into a list of pathname components'''
-    if jsonpath := jsonpath.strip().strip('/'):
-        components = jsonpath.split('/')
-        for i, component in enumerate(components):
-            if component.isdecimal():
-                components[i] = int(component)  # type: ignore
-        return components  # type: ignore
-    else:
-        return []
-
-
-def match_element(py_obj: Any, jpath_components: List[Union[str, int]]) -> Any:
-    for i, component in enumerate(jpath_components):
-        if component == '*' and isinstance(py_obj, list):
-            return [match_element(sub_obj, jpath_components[i + 1:])
-                    for sub_obj in py_obj]
-        else:
-            try:
-                py_obj = py_obj[component]
-            except (IndexError, KeyError, TypeError) as err:
-                raise JSONPathError(f'invalid path node `{component}`') from err
-
-    return py_obj
-
-
-def parse_to_pyobj(input_fp: IO, jsonpath: str) -> Any:
+def parse_to_pyobj(input_fp: IO, jpath: Optional[str]) -> Any:
     '''read json, toml or yaml from IO and then match sub-element by jsonpath'''
     # parse json, toml or yaml to python object
     obj_text = input_fp.read()
     yaml_load = partial(yaml.load, Loader=yaml.Loader)
     for fn_loads in [json.loads, toml.loads, yaml_load]:
         try:
             py_obj = fn_loads(obj_text)
             break
         except Exception:
             continue
     else:
-        print_err(f"no json, toml or yaml object in `{input_fp.name}`")
-        raise ParseError
+        raise ParseError(f"no json, toml or yaml object in `{input_fp.name}`")
 
-    # parse jsonpath and match the sub-element of py_obj
-    jpath_components = parse_jsonpath(jsonpath)
-    try:
-        return match_element(py_obj, jpath_components)
-    except JSONPathError as err:
-        print_err(f'{err}')
-        raise ParseError from err
+    if jpath is None:
+        return py_obj
+    else:
+        # match sub-elements via jsonpath
+        subelements = jsonpath(py_obj, jpath)
+        if subelements is False:
+            raise ParseError('wrong jsonpath')
+        else:
+            return subelements
 
 
-def output_json(py_obj: Any, output_fp: IO, *, cp2clip: bool, compact: bool,
-                escape: bool, indent: int):
+def output_json(py_obj: Any, output_fp: IO, *,
+                cp2clip: bool, compact: bool, escape: bool, indent: int):
     '''output formated json to file or stdout'''
     if compact:
         json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
                                separators=(',', ':'))
     else:
         json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
                                indent=indent)
@@ -132,15 +104,16 @@
     # highlight the toml code when output to TTY divice
     if output_fp.isatty():
         toml_text = highlight(toml_text, TOMLLexer(), TerminalFormatter())
 
     output_fp.write(toml_text)
 
 
-def output_yaml(py_obj: Any, output_fp: IO, *, cp2clip: bool, escape: bool, indent: int):
+def output_yaml(py_obj: Any, output_fp: IO, *,
+                cp2clip: bool, escape: bool, indent: int):
     '''output formated yaml to file or stdout'''
     yaml_text = yaml.safe_dump(py_obj, allow_unicode=not escape, indent=indent,
                                sort_keys=True)
 
     # copy the result to clipboard
     if cp2clip:
         pyperclip.copy(yaml_text)
@@ -165,15 +138,15 @@
     parser.add_argument('-f', dest='format', default='json',
                         choices=['json', 'toml', 'yaml'],
                         help='the format to output ''(default: %(default)s)')
     parser.add_argument('-i', dest='indent', type=int, default=2,
                         help='number of spaces for indentation (default: %(default)s)')
     parser.add_argument('-O', dest='overwrite', action='store_true',
                         help='overwrite the formated text to original file')
-    parser.add_argument('-p', dest='jsonpath', type=str, default='',
+    parser.add_argument('-p', dest='jsonpath', type=str,
                         help='output part of the object via jsonpath')
     parser.add_argument(dest='files', nargs='*',
                         help='the files that will be processed')
     parser.add_argument('-v', dest='version', action='version',
                         version=__version__, help="show the version")
     return parser.parse_args(args)
 
@@ -186,26 +159,28 @@
     if args.cp2clip and not cp2clip:
         print_err('clipboard unavailable')
 
     # match the specified output function
     fn_output = {
         'json': partial(output_json, cp2clip=cp2clip, compact=args.compact,
                         escape=args.escape, indent=args.indent),
-        'yaml': partial(output_yaml, cp2clip=cp2clip, escape=args.escape, indent=args.indent),
+        'yaml': partial(output_yaml, cp2clip=cp2clip, escape=args.escape,
+                        indent=args.indent),
         'toml': partial(output_toml, cp2clip=cp2clip),
     }[args.format]
 
     if args.files:
         for file in args.files:
             try:
                 # read from file
                 with open(file, 'r+') as input_fp:
                     try:
                         py_obj = parse_to_pyobj(input_fp, args.jsonpath)
-                    except ParseError:
+                    except ParseError as err:
+                        print_err(err)
                         exit(1)
                     else:
                         if args.overwrite:
                             # truncate file to zero length before overwrite
                             input_fp.seek(0)
                             input_fp.truncate()
                             output_fp = input_fp
@@ -215,15 +190,16 @@
                         fn_output(py_obj, output_fp)
             except FileNotFoundError:
                 print_err(f'no such file `{file}`')
     else:
         try:
             # read from stdin
             py_obj = parse_to_pyobj(stdin, args.jsonpath)
-        except ParseError:
+        except ParseError as err:
+            print_err(err)
             exit(2)
         else:
             fn_output(py_obj, stdout)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jsonfmt-0.2.2/pyproject.toml` & `jsonfmt-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 description = "A simple tool for formatting JSON object."
 readme = "README.md"
 keywords = ["json", "formatter", "pretty-print", "highlight", "jsonpath"]
 authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
 dependencies = [
+    "jsonpath==0.82",
     "Pygments >= 2.13.0",
     "pyperclip >= 1.8.2",
     "pyyaml >= 6.0",
     "toml >= 0.10.2"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `jsonfmt-0.2.2/test/test.py` & `jsonfmt-0.2.3/test/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,61 +63,44 @@
     name = '<stderr>'
 
 
 class JSONFormatToolTestCase(unittest.TestCase):
     def setUp(self):
         self.py_obj = json.loads(JSON_TEXT)
 
-    def test_parse_jsonpath(self):
-        # test empty jsonpaths
-        expected_components = []
-        for empty_path in ['', '/', '  ', '  /// ']:
-            components = jsonfmt.parse_jsonpath(empty_path)
-            self.assertEqual(components, expected_components)
-
-        # test jsonpath contains key, index and '*'
-        jsonpath = "history/0/items/*/ //name"
-        expected_components = ["history", 0, "items", "*", " ", "", "name"]
-        components = jsonfmt.parse_jsonpath(jsonpath)
-        self.assertEqual(components, expected_components)
-
-    def test_match_element(self):
-        element = jsonfmt.match_element(self.py_obj, ["actions", 0, "calorie"])
-        self.assertEqual(element, 294.9)
-
-        element = jsonfmt.match_element(self.py_obj, ["actions", "*", "name"])
-        self.assertEqual(element, ['eat', 'sport'])
-
-        with self.assertRaises(jsonfmt.JSONPathError):
-            jsonfmt.match_element(self.py_obj, ['not_exist_key'])
-
-        with self.assertRaises(jsonfmt.JSONPathError):
-            jsonfmt.match_element(self.py_obj, ['actions', 7])
+    def test_is_clipboard_available(self):
+        available = jsonfmt.is_clipboard_available()
+        self.assertIsInstance(available, bool)
 
     def test_parse_to_pyobj(self):
-        # normal parameters
         with open(f'{BASE_DIR}/test/example.json') as json_fp:
-            matched_obj = jsonfmt.parse_to_pyobj(json_fp, "actions/*/calorie")
+            # normal parameters
+            matched_obj = jsonfmt.parse_to_pyobj(json_fp, "$.actions[:].calorie")
             self.assertEqual(matched_obj, [294.9, -375])
 
-        # test empty jsonpath
-        with open(f'{BASE_DIR}/test/example.json') as json_fp:
-            matched_obj = jsonfmt.parse_to_pyobj(json_fp, "/")
-            self.assertEqual(matched_obj, self.py_obj)
-
-        with patch('jsonfmt.stderr', FakeStdErr()):
-            # test not exists key
-            with open(f'{BASE_DIR}/test/example.json') as json_fp,\
-                    self.assertRaises(jsonfmt.ParseError):
-                jsonfmt.parse_to_pyobj(json_fp, "not_exist_key")
-
-            # test non-json file
-            with open(__file__) as json_fp,\
-                    self.assertRaises(jsonfmt.ParseError):
-                matched_obj = jsonfmt.parse_to_pyobj(json_fp, "actions/*/date")
+            with patch('jsonfmt.stderr', FakeStdErr()):
+                # test empty jsonpath
+                with self.assertRaises(jsonfmt.ParseError):
+                    json_fp.seek(0)
+                    matched_obj = jsonfmt.parse_to_pyobj(json_fp, "")
+
+                # test not exists key
+                with self.assertRaises(jsonfmt.ParseError):
+                    json_fp.seek(0)
+                    jsonfmt.parse_to_pyobj(json_fp, "$.not_exist_key")
+
+                # test index out of range
+                with self.assertRaises(jsonfmt.ParseError):
+                    json_fp.seek(0)
+                    jsonfmt.parse_to_pyobj(json_fp, '$.actions[7]')
+
+        # test non-json file
+        with open(__file__) as json_fp,\
+                self.assertRaises(jsonfmt.ParseError):
+            matched_obj = jsonfmt.parse_to_pyobj(json_fp, "$.actions[0].calorie")
 
     @patch('jsonfmt.stdout', FakeStdOut())
     def test_output_json(self):
         py_obj = {"name": "约翰", "age": 30}
 
         # test output json to file (temp file)
         with_indent_output = '{\n "age": 30,\n "name": "\\u7ea6\\u7ff0"\n}\n'
@@ -179,15 +162,15 @@
         default_args = Namespace(
             compact=False,
             cp2clip=False,
             escape=False,
             format='json',
             indent=2,
             overwrite=False,
-            jsonpath='',
+            jsonpath=None,
             files=[]
         )
         actual_args = jsonfmt.parse_cmdline_args([])
         self.assertEqual(actual_args, default_args)
 
         # test specified parameters
         args = [
@@ -211,18 +194,18 @@
             jsonpath='path/to/json',
             files=['file1.json', 'file2.json']
         )
 
         actual_args = jsonfmt.parse_cmdline_args(args)
         self.assertEqual(actual_args, expected_args)
 
-    @patch.multiple(sys, argv=['jsonfmt', '-p', 'name', f'{BASE_DIR}/test/example.json'])
+    @patch.multiple(sys, argv=['jsonfmt', '-i', '4', '-p', '$.name', f'{BASE_DIR}/test/example.json'])
     @patch.multiple(jsonfmt, stdout=FakeStdOut())
     def test_main_with_file(self):
-        expected_output = color('"Bob"', 'json')
+        expected_output = color('[\n    "Bob"\n]', 'json')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), expected_output)
 
     @patch.multiple(sys, argv=['jsonfmt', '-f', 'yaml'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]'), stdout=FakeStdOut())
     def test_main_with_stdin(self):
         expected_output = color('- a\n- b', 'yaml')
@@ -288,17 +271,20 @@
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, TOML_TEXT.strip())
 
             with patch("sys.argv", ['jsonfmt', f'{BASE_DIR}/test/example.json', '-Cf', 'yaml']):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, YAML_TEXT.strip())
-        else:
-            errmsg = '\033[1;91mjsonfmt:\033[0m \033[0;91mclipboard unavailable\033[0m\n'
-            with patch.multiple(sys, argv=['jsonfmt', '-C']), \
-                    patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]')):
-                jsonfmt.main()
-                self.assertEqual(jsonfmt.stderr.read(), errmsg)
+
+    @patch.multiple(jsonfmt, is_clipboard_available=lambda: False)
+    @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
+    @patch.multiple(sys, argv=['jsonfmt', f'{BASE_DIR}/test/example.json', '-cC'])
+    def test_clipboard_unavailable(self):
+        errmsg = '\033[1;91mjsonfmt:\033[0m \033[0;91mclipboard unavailable\033[0m\n'
+        jsonfmt.main()
+        self.assertEqual(jsonfmt.stderr.read(), errmsg)
+        self.assertEqual(jsonfmt.stdout.read(), color(JSON_TEXT, 'json'))
 
 
 if __name__ == '__main__':
     unittest.main()
```

