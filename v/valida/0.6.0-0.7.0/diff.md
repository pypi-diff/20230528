# Comparing `tmp/valida-0.6.0.tar.gz` & `tmp/valida-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valida-0.6.0.tar", max compression
+gzip compressed data, was "valida-0.7.0.tar", max compression
```

## Comparing `valida-0.6.0.tar` & `valida-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-26 19:36:42.603934 valida-0.6.0/LICENSE
--rw-r--r--   0        0        0     1439 2023-05-26 19:36:42.603934 valida-0.6.0/README.md
--rw-r--r--   0        0        0      720 2023-05-26 19:36:42.607935 valida-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      200 2023-05-26 19:36:42.607935 valida-0.6.0/valida/__init__.py
--rw-r--r--   0        0        0     3015 2023-05-26 19:36:42.607935 valida-0.6.0/valida/callables.py
--rw-r--r--   0        0        0      353 2023-05-26 19:36:42.607935 valida-0.6.0/valida/casting.py
--rw-r--r--   0        0        0    31469 2023-05-26 19:36:42.607935 valida-0.6.0/valida/conditions.py
--rw-r--r--   0        0        0    10524 2023-05-26 19:36:42.607935 valida-0.6.0/valida/data.py
--rw-r--r--   0        0        0    29661 2023-05-26 19:36:42.607935 valida-0.6.0/valida/datapath.py
--rw-r--r--   0        0        0      485 2023-05-26 19:36:42.607935 valida-0.6.0/valida/errors.py
--rw-r--r--   0        0        0     6888 2023-05-26 19:36:42.607935 valida-0.6.0/valida/rules.py
--rw-r--r--   0        0        0    14363 2023-05-26 19:36:42.607935 valida-0.6.0/valida/schema.py
--rw-r--r--   0        0        0      968 2023-05-26 19:36:42.607935 valida-0.6.0/valida/utils.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-28 12:45:23.634978 valida-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1439 2023-05-28 12:45:23.634978 valida-0.7.0/README.md
+-rw-r--r--   0        0        0      720 2023-05-28 12:45:23.634978 valida-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-05-28 12:45:23.634978 valida-0.7.0/valida/__init__.py
+-rw-r--r--   0        0        0     3015 2023-05-28 12:45:23.634978 valida-0.7.0/valida/callables.py
+-rw-r--r--   0        0        0      353 2023-05-28 12:45:23.634978 valida-0.7.0/valida/casting.py
+-rw-r--r--   0        0        0    31649 2023-05-28 12:45:23.638978 valida-0.7.0/valida/conditions.py
+-rw-r--r--   0        0        0    10524 2023-05-28 12:45:23.638978 valida-0.7.0/valida/data.py
+-rw-r--r--   0        0        0    29661 2023-05-28 12:45:23.638978 valida-0.7.0/valida/datapath.py
+-rw-r--r--   0        0        0      485 2023-05-28 12:45:23.638978 valida-0.7.0/valida/errors.py
+-rw-r--r--   0        0        0     7454 2023-05-28 12:45:23.638978 valida-0.7.0/valida/rules.py
+-rw-r--r--   0        0        0    17764 2023-05-28 12:45:23.638978 valida-0.7.0/valida/schema.py
+-rw-r--r--   0        0        0      968 2023-05-28 12:45:23.638978 valida-0.7.0/valida/utils.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.7.0/PKG-INFO
```

### Comparing `valida-0.6.0/LICENSE` & `valida-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/README.md` & `valida-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/pyproject.toml` & `valida-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "valida"
-version = "0.6.0"
+version = "0.7.0"
 description = "Comprehensive validation library for nested data structures."
 authors = ["Adam J. Plowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -16,15 +16,15 @@
 pytest = "^6.2.5"
 commitizen = "^2.20.3"
 pre-commit = "^2.16.0"
 black = "^21.12b0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "0.7.0"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "valida/__init__.py"
 ]
 
 [build-system]
```

### Comparing `valida-0.6.0/valida/callables.py` & `valida-0.7.0/valida/callables.py`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/valida/conditions.py` & `valida-0.7.0/valida/conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,16 @@
                 # Check items for DataPath specs:
                 for idx, v in enumerate(spec_val):
                     try:
                         spec_val[idx] = valida.datapath.DataPath.from_spec(v)
                     except MalformedDataPathSpec:
                         pass
 
+            # invoke the condition method to construct the Condition object:
+
             if not any(
                 func_args[i]
                 for i in ("POSITIONAL_OR_KEYWORD", "VAR_POSITIONAL", "VAR_KEYWORD")
             ):
                 # no arguments, check value given is None and invoke:
                 if spec_val is not None:
                     warnings.warn(
@@ -562,14 +564,16 @@
         conditions, binary_ops = self.flatten()
         if not binary_ops or set(binary_ops) == {"and"}:
             for i in conditions:
                 if isinstance(i, KeyDataType):
                     out["key_data_type"].append(i)
                 elif isinstance(i, ValueDataType):
                     out["value_data_type"].append(i)
+                elif isinstance(i, ValueLength):
+                    out["value_data_type"].append(i)
                 elif isinstance(i, Value) and i.callable.name == "is_instance":
                     out["value_data_type"].append(i)
                 elif isinstance(i, Value) and i.callable.name == "in_":
                     out["value_data_type"].append(i)
                 elif isinstance(i, Value) and i.callable.name == "keys_is_instance":
                     out["key_data_type"].append(i)
         return out
```

### Comparing `valida-0.6.0/valida/data.py` & `valida-0.7.0/valida/data.py`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/valida/datapath.py` & `valida-0.7.0/valida/datapath.py`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/valida/rules.py` & `valida-0.7.0/valida/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import copy
-from typing import List, Optional
+from typing import Dict, Optional
 from valida.conditions import ConditionLike
 from valida.casting import CAST_DTYPE_LOOKUP, CAST_LOOKUP
 from valida.data import Data, set_datum
 from valida.datapath import DataPath
 from valida.errors import MalformedRuleSpec
 
 
 class Rule:
-    def __init__(self, path, condition, cast=None, doc: Optional[List[str]] = None):
+    def __init__(self, path, condition, cast=None, doc: Optional[Dict] = None):
         if not isinstance(path, DataPath):
             path = DataPath(*path)
 
         self.path = path
         self.condition = condition
         self.cast = cast
         self.doc = doc
@@ -37,20 +37,35 @@
     @classmethod
     def from_spec(cls, spec):
         path = DataPath.from_part_specs(*spec["path"])
         cond = ConditionLike.from_spec(spec["condition"])
         doc = spec.get("doc")
 
         if doc:
-            if not isinstance(doc, list):
-                doc = [doc]
+            if not isinstance(doc, dict):
+                if isinstance(doc, str):
+                    doc = [doc]
+
+                if isinstance(doc, list):
+                    doc = {"description": doc, "examples": []}
+
+            elif isinstance(doc["description"], str):
+                doc["description"] = [doc["description"]]
+
+            if "description" not in doc:
+                doc["description"] = []
+
+            if "examples" not in doc:
+                doc["examples"] = []
 
             # strip final new lines:
-            for idx, i in enumerate(doc):
-                doc[idx] = i.strip()
+            for idx, desc_i in enumerate(doc["description"]):
+                doc["description"][idx] = desc_i.strip()
+            for idx, ex_i in enumerate(doc["examples"]):
+                doc["examples"][idx] = ex_i.strip()
 
         cast = spec.get("cast")
         for cast_from in list((cast or {}).keys()):
             cast_to = cast.pop(cast_from)
             try:
                 cast_from = CAST_DTYPE_LOOKUP[cast_from]
             except KeyError:
```

### Comparing `valida-0.6.0/valida/schema.py` & `valida-0.7.0/valida/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,144 +14,205 @@
 
 def format_map_key_value_data_type_conditions(
     cnds: List[Union[KeyDataType, ValueDataType]]
 ) -> str:
     out = []
     for i in cnds:
         out_i = ""
-        if i.callable.name == "equal_to":
+
+        pre_proc = i.PRE_PROCESSOR
+
+        if pre_proc and pre_proc.__name__ == "len":
+            if i.callable.name == "equal_to":
+                val = i.callable.kwargs["value"]
+            elif i.callable.name == "in_":
+                val = " or ".join(str(j) for j in i.callable.kwargs["value"])
+            out_i += f"length: {val}"
+
+        elif i.callable.name == "equal_to":
             val = i.callable.kwargs["value"]
             try:
                 val = INV_DTYPE_LOOKUP[val]
             except KeyError:
                 pass
             out_i += f"{val}"
+
         elif i.callable.name in ("is_instance", "keys_is_instance"):
             arg_concat_i = []
             for arg_j in i.callable.args:
                 try:
                     arg_j = INV_DTYPE_LOOKUP[arg_j]
                 except KeyError:
                     pass
                 arg_concat_i.append(arg_j)
             arg_concat_i_str = " | ".join(str(i) for i in arg_concat_i)
             out_i += arg_concat_i_str
+
         elif i.callable.name == "in_":
             arg_concat_i = (repr(j) for j in i.callable.kwargs["value"])
             arg_concat_i_str = "(" + " | ".join(arg_concat_i) + ")"
             out_i += arg_concat_i_str
+
         out.append(out_i)
     if len(out) > 1:
         out_str = ", ".join(out)
     else:
         out_str = out[0]
     return out_str
 
 
-def write_tree_html(tree, _path=None, anchor_root: str = None):
-    empty_map_str = "map-value"
-    empty_lst_str = "list-value"
+def write_tree_html(
+    nested_tree,
+    _path=None,
+    anchor_root: str = None,
+    heading_start_level=1,
+    show_root_heading=True,
+    _depth=0,
+):
+    empty_map_str = "[map-value]"
+    empty_lst_str = "[list-value]"
     empty_map_span = (
-        f'<span class="valida-tree null-condition-path-elem">[{empty_map_str}]</span>'
+        f'<span class="valida-tree null-condition-path-elem">{empty_map_str}</span>'
     )
     empty_lst_span = (
-        f'<span class="valida-tree null-condition-path-elem">[{empty_lst_str}]</span>'
+        f'<span class="valida-tree null-condition-path-elem">{empty_lst_str}</span>'
+    )
+    top_node = " top-level-node" if _path is None else ""
+    node_html = (
+        f'<div class="valida-tree node{top_node}" data-node-path='
+        f'"{html.escape(str(_path or ""))}">'
     )
-    out = f'<div class="valida-tree node" data-node-path="{html.escape(str(_path) or "")}">'
-
-    for child in tree:
-        out += f'<div class="valida-tree node-child">'
-
-        path_fmt_lst = []
-        for i in child["path"]:
-            if i == MapValue():
-                i = empty_map_span
-            elif i == ListValue():
-                i = empty_lst_span
-            else:
-                i = html.escape(str(i))
-            path_fmt_lst.append(str(i))
-        path_fmt = " → ".join(path_fmt_lst)
 
-        path_anchor_lst = [] if not anchor_root else [anchor_root]
+    children_html = ""
+    for child in nested_tree:
+        child_html = ""
+
+        if child.get("type_info_in_parent") and not child.get("children"):
+            # this will need refining.
+            # TODO: also check that the only conditions are type
+            continue
+
+        child_html += f'<div class="valida-tree node-child">'
+
+        path_lst = [] if not anchor_root else [anchor_root]
+        title_lst = [] if not anchor_root else [anchor_root]
+        sec_ID_lst = [] if not anchor_root else [anchor_root]
         for i in child["path"]:
             if i == MapValue():
-                i = empty_map_str
+                i_p = empty_map_span
+                i_s = empty_map_str.replace("[", "%5B").replace("]", "%5D")
+                i_t = empty_map_str
             elif i == ListValue():
-                i = empty_lst_str
+                i_p = empty_lst_span
+                i_s = empty_lst_str.replace("[", "%5B").replace("]", "%5D")
+                i_t = empty_lst_str
             else:
-                i = html.escape(str(i))
-            path_anchor_lst.append(str(i))
+                i_p = i_s = i_t = html.escape(str(i))
 
-        path_anchor = "vld-" + "-".join(path_anchor_lst)
-        path_title = " → ".join(path_anchor_lst)
-        head_anchor = f"#{path_anchor}"
-
-        out += f'<section class="valida-tree-section" id={path_anchor}>'
-
-        if path_fmt:
-            head_lev = len(child["path"]) + 1
-            path_fmt_final = f"{path_fmt_lst[-1]}"  # not showing whole path?
-            out += f'<div class="valida-tree path-name"><h{head_lev} title="{path_title}">{path_fmt_final}<a class="headerlink" href="{head_anchor}">#</a></h{head_lev}></div>'
+            path_lst.append(str(i_p))
+            sec_ID_lst.append(str(i_s))
+            title_lst.append(str(i_t))
+
+        sec_id = "vld-" + "-".join(sec_ID_lst)
+        head_anchor = f"#{sec_id}"
+        path_title = " → ".join(title_lst)
+        child_html += f'<section class="valida-tree-section" id="{sec_id}">'
+
+        if path_lst:
+            if _depth > 0 or (_depth == 0 and show_root_heading):
+                head_lev = heading_start_level + _depth
+                path_fmt_final = path_lst[-1]
+                child_html += (
+                    f'<div class="valida-tree path-name"><h{head_lev} title='
+                    f'"{path_title}">{path_fmt_final}<a class="headerlink" href='
+                    f'"{head_anchor}">#</a></h{head_lev}></div>'
+                )
 
-        out += f'<div class="valida-tree node-info">'
-        out += f'<div class="valida-tree node-metadata">'
+        child_html += f'<div class="valida-tree node-info">'
+        child_html += f'<div class="valida-tree node-metadata">'
         type_line_lst = []
         chd_type = child.get("type_fmt")
         chd_key_type = child.get("key_type_fmt")
+        chd_val_type = child.get("map_value_type_fmt")
+        chd_list_type = child.get("list_value_type_fmt")
         chd_cnd = child.get("condition")
         if chd_type:
             chd_type = str(chd_type)
             type_line_lst.append(
-                f'<span class="valida-tree type-name">type: {html.escape(chd_type)}</span>'
+                f'<span class="valida-tree type-name">type: '
+                f"{html.escape(chd_type)}</span>"
             )
             if chd_key_type:
                 chd_key_type = str(chd_key_type)
                 type_line_lst[-1] += (
                     f' <span class="valida-tree key-type-name">(key: '
                     f"{html.escape(chd_key_type)})</span>"
                 )
+            if chd_val_type:
+                chd_val_type = str(chd_val_type)
+                type_line_lst[-1] += (
+                    f' <span class="valida-tree map-val-type-name">(value: '
+                    f"{html.escape(chd_val_type)})</span>"
+                )
+            if chd_list_type:
+                chd_list_type = str(chd_list_type)
+                type_line_lst[-1] += (
+                    f' <span class="valida-tree list-type-name">(of: '
+                    f"{html.escape(chd_list_type)})</span>"
+                )
 
-        chd_req = child.get("required")
-        if _path is None:
-            chd_req = True
-
-        type_line_lst.append(
-            f'<span class="valida-tree required-name">{"required" if chd_req else "optional"}</span>'
-        )
+        if _path is not None:
+            chd_req = child.get("required")
+            type_line_lst.append(
+                f'<span class="valida-tree required-name">'
+                f'{"required" if chd_req else "optional"}</span>'
+            )
 
-        out += ", ".join(type_line_lst)
+        child_html += ", ".join(type_line_lst)
 
-        if not chd_type and chd_cnd:
-            chd_cnd = str(chd_cnd)
-            out += (
-                f'<div class="tree condition">Condition: {html.escape(chd_cnd)}</div>'
-            )
-        out += "</div>"  # node-metadata
+        chd_cnd = str(chd_cnd)
+        child_html += (
+            f'<div class="valida-tree condition">Condition: <code>'
+            f"{html.escape(chd_cnd)}</code></div>"
+        )
+        child_html += "</div>"  # node-metadata
 
         chd_doc = child.get("doc")
         if chd_doc:
-            for doc_para in chd_doc:
+            for doc_para in chd_doc["description"]:
                 # search for back ticks and replace with `<code>` tags:
                 doc_para = html.escape(doc_para)
                 doc_para = re.sub(r"`(.*?)`", r"<code>\1</code>", doc_para)
-                out += f'<p class="valida-tree doc">{doc_para}</p>'
-        out += "</div>"  # node-info
+                child_html += f'<p class="valida-tree doc">{doc_para}</p>'
+            for doc_ex in chd_doc["examples"]:
+                doc_ex = html.escape(doc_ex)
+                doc_ex = re.sub(r"`(.*?)`", r"<code>\1</code>", doc_ex)
+                child_html += (
+                    f'<p class="valida-tree doc-example"><span class='
+                    f'"valida-tree doc-example-name">Example: </span>{doc_ex}</p>'
+                )
+        child_html += "</div>"  # node-info
 
         if "children" in child:
-            out += write_tree_html(
+            child_html += write_tree_html(
                 child["children"],
                 _path=child["path"],
                 anchor_root=anchor_root,
+                heading_start_level=heading_start_level,
+                _depth=_depth + 1,
             )
 
-        out += "</section>"
-        out += "</div>"
+        child_html += "</section>"
+        child_html += "</div>"
+        children_html += child_html
+
+    out = ""
+    if children_html:
+        out = node_html + children_html + "</div>"
 
-    out += "</div>"
     return out
 
 
 class Schema:
     def __init__(self, rules):
         self.rules = sorted(rules, key=lambda i: len(i.path))
         self.rule_tests = None  # Assigned by `self.validate`
@@ -259,55 +320,77 @@
             if path_str not in items:
                 items[path_str] = {}
 
             items[path_str]["condition"] = rule.condition
             items[path_str]["path"] = path_simple
             items[path_str]["doc"] = rule.doc
 
-            # add parent types that are implicitly defined:
-            imp_types = rule.path.resolve_implicit_types()[len(from_path_str) :]
-            if imp_types:
-                for idx, imp_type in enumerate(imp_types):
-                    if idx == 0:
-                        parent_path = []
-                    else:
-                        parent_path = rule.path.parts[len(from_path_str) : idx]
-                    parent_path_str = tuple(str(i) for i in parent_path)
-
-                    if parent_path_str not in items:
-                        items[parent_path_str] = {}
-                    items[parent_path_str]["type"] = IMP_TYPE_LOOKUP[imp_type]
-                    items[parent_path_str]["type_fmt"] = items[parent_path_str]["type"]
-
-            key_conditions = rule.condition.get_always_applicable_key_conditions()
-            for key_cnd in key_conditions:
+            key_cnds = rule.condition.get_always_applicable_key_conditions()
+            for key_cnd in key_cnds:
                 for key in key_cnd.callable.args:
                     path_simple_i = tuple(list(path_simple) + [key])
                     path_i = rule.path[len(from_path_str) :] / DataPath(key)
                     path_i_str = tuple(str(i) for i in path_i)
                     if path_i_str not in items:
                         items[path_i_str] = {"path": path_simple_i}
                     items[path_i_str]["required"] = (
                         key_cnd.callable.name == "required_keys"
                     )
 
-            kv_conditions = rule.condition.get_always_applicable_type_like_conditions()
-            if kv_conditions["key_data_type"]:
-                items[path_str]["key_type"] = kv_conditions["key_data_type"]
+            type_cnds = rule.condition.get_always_applicable_type_like_conditions()
+            if type_cnds["key_data_type"]:
+                items[path_str]["key_type"] = type_cnds["key_data_type"]
                 items[path_str][
                     "key_type_fmt"
                 ] = format_map_key_value_data_type_conditions(
                     items[path_str]["key_type"]
                 )
-            if kv_conditions["value_data_type"]:
-                items[path_str]["type"] = kv_conditions["value_data_type"]
+            if type_cnds["value_data_type"]:
+                items[path_str]["type"] = type_cnds["value_data_type"]
                 items[path_str]["type_fmt"] = format_map_key_value_data_type_conditions(
                     items[path_str]["type"]
                 )
 
+            # add parent container type that is implicitly defined:
+            imp_types = rule.path.resolve_implicit_types()
+            if imp_types:
+                par_implicit_type = imp_types[-1]
+
+                if len(imp_types) == 1:
+                    parent_path = DataPath()
+                else:
+                    parent_path = rule.path[len(from_path_str) : -1]
+
+                parent_path_str = tuple(str(i) for i in parent_path.parts)
+
+                if parent_path_str not in items:
+                    items[parent_path_str] = {}
+
+                if not items[parent_path_str].get("type"):
+                    items[parent_path_str]["type"] = IMP_TYPE_LOOKUP[par_implicit_type]
+                    items[parent_path_str]["type_fmt"] = items[parent_path_str]["type"]
+
+                if "type" in items[path_str] and rule.path.parts[-1] == ListValue():
+                    # this rule's type conditions can be contained in the parent node,
+                    # since they apply for all list values:
+                    items[parent_path_str]["list_value_type"] = items[path_str]["type"]
+                    items[parent_path_str]["list_value_type_fmt"] = items[path_str][
+                        "type_fmt"
+                    ]
+                    items[path_str]["type_info_in_parent"] = True
+
+                if "type" in items[path_str] and rule.path.parts[-1] == MapValue():
+                    # this rule's type conditions can be contained in the parent node,
+                    # since they apply for all list values:
+                    items[parent_path_str]["map_value_type"] = items[path_str]["type"]
+                    items[parent_path_str]["map_value_type_fmt"] = items[path_str][
+                        "type_fmt"
+                    ]
+                    items[path_str]["type_info_in_parent"] = True
+
         # convert to a list with parent references
         items_lst = []
         parent_refs = {tuple(): -1}
         for k, v in items.items():
             parent_path = k[:-1]
             v["parent"] = parent_refs[parent_path]
             v["path_str"] = k
```

### Comparing `valida-0.6.0/valida/utils.py` & `valida-0.7.0/valida/utils.py`

 * *Files identical despite different names*

### Comparing `valida-0.6.0/PKG-INFO` & `valida-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valida
-Version: 0.6.0
+Version: 0.7.0
 Summary: Comprehensive validation library for nested data structures.
 License: MIT
 Author: Adam J. Plowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

