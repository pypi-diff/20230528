# Comparing `tmp/pymodd-1.0.3.tar.gz` & `tmp/pymodd-1.0.4.tar.gz`

## Comparing `pymodd-1.0.3.tar` & `pymodd-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.3/Cargo.toml
--rw-r--r--   0     1001      123     2156 2023-05-25 21:01:48.000000 pymodd-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0     1001      123      372 2023-05-25 21:01:48.000000 pymodd-1.0.3/.github/workflows/test.yml
--rw-r--r--   0     1001      123     3103 2023-05-25 21:01:48.000000 pymodd-1.0.3/.gitignore
--rw-r--r--   0     1001      123     1043 2023-05-25 21:01:48.000000 pymodd-1.0.3/LICENSE.txt
--rw-r--r--   0     1001      123     2041 2023-05-25 21:01:48.000000 pymodd-1.0.3/README.rst
--rw-r--r--   0     1001      123     1059 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/entity_scripts.py
--rw-r--r--   0     1001      123     2823 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/game_variables.py
--rw-r--r--   0     1001      123      559 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/mapping.py
--rw-r--r--   0     1001      123     5672 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/scripts.py
--rw-r--r--   0     1001      123    78239 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/utils/game.json
--rw-r--r--   0     1001      123        0 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/__init__.py
--rw-r--r--   0     1001      123     1050 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/_pymodd_helper.pyi
--rw-r--r--   0     1001      123    46037 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/actions.py
--rw-r--r--   0     1001      123     3998 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/console_scripts/pymodd_command.py
--rw-r--r--   0     1001      123     2563 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/entity_script.py
--rw-r--r--   0     1001      123    51870 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/functions.py
--rw-r--r--   0     1001      123     6188 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/game.py
--rw-r--r--   0     1001      123       26 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/py.typed
--rw-r--r--   0     1001      123    15438 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/script.py
--rw-r--r--   0     1001      123   122364 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/utils/Default Game.json
--rw-r--r--   0     1001      123    38332 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/variable_types.py
--rw-r--r--   0     1001      123      790 2023-05-25 21:01:48.000000 pymodd-1.0.3/pyproject.toml
--rw-r--r--   0     1001      123       41 2023-05-25 21:01:48.000000 pymodd-1.0.3/requirements.txt
--rw-r--r--   0     1001      123     7772 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/actions.rs
--rw-r--r--   0     1001      123    20109 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/argument.rs
--rw-r--r--   0     1001      123     9875 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/directory.rs
--rw-r--r--   0     1001      123     5295 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/entity_types.rs
--rw-r--r--   0     1001      123    10379 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/variable_categories.rs
--rw-r--r--   0     1001      123     1799 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data.rs
--rw-r--r--   0     1001      123     1992 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/lib.rs
--rw-r--r--   0     1001      123    12703 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/entity_scripts_file.rs
--rw-r--r--   0     1001      123      183 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/game_json_file.rs
--rw-r--r--   0     1001      123    12760 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/game_variables_file.rs
--rw-r--r--   0     1001      123     4350 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/mapping_file.rs
--rw-r--r--   0     1001      123    44725 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/scripts_file.rs
--rw-r--r--   0     1001      123     9842 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators/argument_values_iterator.rs
--rw-r--r--   0     1001      123     1820 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators/directory_iterator.rs
--rw-r--r--   0     1001      123       62 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators.rs
--rw-r--r--   0     1001      123    10239 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/to_pymodd_maps.rs
--rw-r--r--   0     1001      123     2518 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils.rs
--rw-r--r--   0     1001      123     2442 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator.rs
--rw-r--r--   0     1001      123    12887 2023-05-25 21:01:48.000000 pymodd-1.0.3/Cargo.lock
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 pymodd-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.4/Cargo.toml
+-rw-r--r--   0     1001      123     2156 2023-05-28 19:16:59.000000 pymodd-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123      372 2023-05-28 19:16:59.000000 pymodd-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     3103 2023-05-28 19:16:59.000000 pymodd-1.0.4/.gitignore
+-rw-r--r--   0     1001      123     1043 2023-05-28 19:16:59.000000 pymodd-1.0.4/LICENSE.txt
+-rw-r--r--   0     1001      123     2093 2023-05-28 19:16:59.000000 pymodd-1.0.4/README.rst
+-rw-r--r--   0     1001      123     1059 2023-05-28 19:16:59.000000 pymodd-1.0.4/examples/froge/entity_scripts.py
+-rw-r--r--   0     1001      123     2823 2023-05-28 19:16:59.000000 pymodd-1.0.4/examples/froge/game_variables.py
+-rw-r--r--   0     1001      123      559 2023-05-28 19:16:59.000000 pymodd-1.0.4/examples/froge/mapping.py
+-rw-r--r--   0     1001      123     5672 2023-05-28 19:16:59.000000 pymodd-1.0.4/examples/froge/scripts.py
+-rw-r--r--   0     1001      123    78239 2023-05-28 19:16:59.000000 pymodd-1.0.4/examples/froge/utils/game.json
+-rw-r--r--   0     1001      123        0 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/__init__.py
+-rw-r--r--   0     1001      123     1050 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/_pymodd_helper.pyi
+-rw-r--r--   0     1001      123    46037 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/actions.py
+-rw-r--r--   0     1001      123     3998 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/console_scripts/pymodd_command.py
+-rw-r--r--   0     1001      123     2563 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/entity_script.py
+-rw-r--r--   0     1001      123    51870 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/functions.py
+-rw-r--r--   0     1001      123     6188 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/game.py
+-rw-r--r--   0     1001      123       26 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/py.typed
+-rw-r--r--   0     1001      123    15438 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/script.py
+-rw-r--r--   0     1001      123   122364 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/utils/Default Game.json
+-rw-r--r--   0     1001      123    38332 2023-05-28 19:16:59.000000 pymodd-1.0.4/pymodd/variable_types.py
+-rw-r--r--   0     1001      123      790 2023-05-28 19:16:59.000000 pymodd-1.0.4/pyproject.toml
+-rw-r--r--   0     1001      123       41 2023-05-28 19:16:59.000000 pymodd-1.0.4/requirements.txt
+-rw-r--r--   0     1001      123     7772 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data/actions.rs
+-rw-r--r--   0     1001      123    20109 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data/argument.rs
+-rw-r--r--   0     1001      123    13801 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data/directory.rs
+-rw-r--r--   0     1001      123     5295 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data/entity_types.rs
+-rw-r--r--   0     1001      123    10379 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data/variable_categories.rs
+-rw-r--r--   0     1001      123     1799 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/game_data.rs
+-rw-r--r--   0     1001      123     1992 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/lib.rs
+-rw-r--r--   0     1001      123    12632 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/entity_scripts_file.rs
+-rw-r--r--   0     1001      123      183 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/game_json_file.rs
+-rw-r--r--   0     1001      123    12760 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/game_variables_file.rs
+-rw-r--r--   0     1001      123     4341 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/mapping_file.rs
+-rw-r--r--   0     1001      123    44581 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/scripts_file.rs
+-rw-r--r--   0     1001      123     9842 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/utils/iterators/argument_values_iterator.rs
+-rw-r--r--   0     1001      123     1820 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/utils/iterators/directory_iterator.rs
+-rw-r--r--   0     1001      123       62 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/utils/iterators.rs
+-rw-r--r--   0     1001      123    10239 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/utils/to_pymodd_maps.rs
+-rw-r--r--   0     1001      123     2518 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator/utils.rs
+-rw-r--r--   0     1001      123     2442 2023-05-28 19:16:59.000000 pymodd-1.0.4/src/project_generator.rs
+-rw-r--r--   0     1001      123    12887 2023-05-28 19:16:59.000000 pymodd-1.0.4/Cargo.lock
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 pymodd-1.0.4/PKG-INFO
```

### Comparing `pymodd-1.0.3/.github/workflows/publish.yml` & `pymodd-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/.gitignore` & `pymodd-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/LICENSE.txt` & `pymodd-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/README.rst` & `pymodd-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pymodd
+Version: 1.0.4
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: case-converter==1.1.0
+License-File: LICENSE.txt
+Summary: create and edit modd.io games in python
+Author: Jeff
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+Project-URL: repository, https://github.com/jeff5343/pymodd
+Project-URL: changelog, https://github.com/jeff5343/pymodd/releases
+
 ======
 pymodd
 ======
 
 |Build| |Version| |License|
 
 pymodd is a python package for creating and editing modd.io games in python
@@ -22,33 +38,34 @@
 - a command to generate and compile a pymodd project
 
 Documentation
 -------------
 
 The pymodd wiki is located at `github.com/jeff5343/pymodd/wiki <https://github.com/jeff5343/pymodd/wiki>`_
 
-A brief outline of the wiki:
+A brief outline:
 
 - `Introduction <https://github.com/jeff5343/pymodd/wiki>`_
 - `Install Guide <https://github.com/jeff5343/pymodd/wiki/Install-Guide>`_
 - `Generating and Compiling a Pymodd Project <https://github.com/jeff5343/pymodd/wiki/Generating-and-Compiling-a-Pymodd-Project>`_
 - `Pymodd Project Structure <https://github.com/jeff5343/pymodd/wiki/Pymodd-Project-Structure>`_
 
 
 Quick Script Example
 --------------------
 
-view the ``examples/froge`` directory for an example of a pymodd project
+view the ``examples/froge`` directory in the `github repository <https://github.com/jeff5343/pymodd>`_ to view the entire pymodd project
 
 .. code:: py
 
     @script(triggers=[Trigger.EVERY_SECOND])
     def every_second():
         if NumberOfUnitsOfUnitType(UnitType.FROG) < 5:
             create_unit_for_player_at_position_with_rotation(UnitType.FROG, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
         else:
             if NumberOfUnitsOfUnitType(UnitType.FROG_BOSS) == 0:
                 if Variable.BOSS_TIMER <= 0:
                     create_unit_for_player_at_position_with_rotation(UnitType.FROG_BOSS, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
                     update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000)
                 decrease_variable_by_number(Variable.BOSS_TIMER, 1)
 
+
```

### Comparing `pymodd-1.0.3/examples/froge/entity_scripts.py` & `pymodd-1.0.4/examples/froge/entity_scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/examples/froge/game_variables.py` & `pymodd-1.0.4/examples/froge/game_variables.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/examples/froge/mapping.py` & `pymodd-1.0.4/examples/froge/mapping.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/examples/froge/scripts.py` & `pymodd-1.0.4/examples/froge/scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/examples/froge/utils/game.json` & `pymodd-1.0.4/examples/froge/utils/game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/_pymodd_helper.pyi` & `pymodd-1.0.4/pymodd/_pymodd_helper.pyi`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/actions.py` & `pymodd-1.0.4/pymodd/actions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/console_scripts/pymodd_command.py` & `pymodd-1.0.4/pymodd/console_scripts/pymodd_command.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/entity_script.py` & `pymodd-1.0.4/pymodd/entity_script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/functions.py` & `pymodd-1.0.4/pymodd/functions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/game.py` & `pymodd-1.0.4/pymodd/game.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/script.py` & `pymodd-1.0.4/pymodd/script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/utils/Default Game.json` & `pymodd-1.0.4/pymodd/utils/Default Game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pymodd/variable_types.py` & `pymodd-1.0.4/pymodd/variable_types.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/pyproject.toml` & `pymodd-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pymodd"
-version = "1.0.3"
+version = "1.0.4"
 description = "create and edit modd.io games in python"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Jeff"}
 ]
```

### Comparing `pymodd-1.0.3/src/game_data/actions.rs` & `pymodd-1.0.4/src/game_data/actions.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/game_data/argument.rs` & `pymodd-1.0.4/src/game_data/argument.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/game_data/directory.rs` & `pymodd-1.0.4/src/game_data/directory.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,22 @@
+use std::collections::{HashMap, VecDeque};
+
 use heck::ToSnakeCase;
 use serde_json::{map::Values, Map, Value};
 
 use crate::project_generator::utils::{
     is_valid_class_name, iterators::directory_iterator::DirectoryIterItem,
     to_pymodd_maps::TRIGGERS_TO_PYMODD_ENUM,
 };
 
 use super::actions::{self, Action};
 
 const UNDEFINED_STRING: &str = "UNDEFINED";
 
 #[derive(Debug, PartialEq, Eq)]
-pub enum DirectoryItem {
-    Directory(Directory),
-    Script(Script),
-}
-
-fn parse_key_of_item_to_string(key: &str, item_data: &Value) -> String {
-    item_data
-        .get(key)
-        .unwrap_or(&Value::Null)
-        .as_str()
-        .unwrap_or(UNDEFINED_STRING)
-        .to_string()
-}
-
-impl DirectoryItem {
-    fn parse(item_data: &Value) -> DirectoryItem {
-        match item_data.get("actions") {
-            Some(actions) => DirectoryItem::Script(Script {
-                name: parse_key_of_item_to_string("name", &item_data),
-                key: parse_key_of_item_to_string("key", &item_data),
-                triggers: item_data
-                    .get("triggers")
-                    .unwrap_or(&Value::Null)
-                    .as_array()
-                    .unwrap_or(&Vec::new())
-                    .into_iter()
-                    .map(|trigger| parse_key_of_item_to_string("type", &trigger))
-                    .collect(),
-                actions: actions::parse_actions(actions.as_array().unwrap_or(&Vec::new())),
-            }),
-            None => DirectoryItem::Directory(Directory {
-                children: Vec::new(),
-                name: parse_key_of_item_to_string("folderName", &item_data),
-                key: parse_key_of_item_to_string("key", &item_data),
-            }),
-        }
-    }
-}
-
-#[derive(Debug, PartialEq, Eq)]
 pub struct Directory {
     pub children: Vec<DirectoryItem>,
     pub name: String,
     key: String,
 }
 
 impl Directory {
@@ -78,39 +40,43 @@
         })
     }
 }
 
 fn root_children_from_scripts_data(scripts: &Value) -> Vec<DirectoryItem> {
     let empty_map = Map::new();
     let mut items: Vec<&Value> =
-        sort_based_on_order(scripts.as_object().unwrap_or(&empty_map).values());
+        sort_items_by_order(scripts.as_object().unwrap_or(&empty_map).values());
 
-    // filter out root level scripts and directories
-    let mut children = filter_out_children_of_parent(&mut items, None);
+    // remove root level scripts and directories
+    let mut children: Vec<DirectoryItem> = remove_children_of_parent_in_items(None, &mut items)
+        .into_iter()
+        .map(|val| DirectoryItem::parse(val))
+        .collect();
 
     let mut stack: Vec<&mut DirectoryItem> = children.iter_mut().collect();
     while stack.len() > 0 {
         if let DirectoryItem::Directory(directory) = stack.pop().unwrap() {
-            directory.children.extend(filter_out_children_of_parent(
-                &mut items,
-                Some(&directory.key),
-            ));
+            directory.children.extend(
+                remove_children_of_parent_in_items(Some(&directory.key), &mut items)
+                    .into_iter()
+                    .map(|val| DirectoryItem::parse(val)),
+            );
 
             stack.extend(
                 directory
                     .children
                     .iter_mut()
                     .collect::<Vec<&mut DirectoryItem>>(),
             );
         }
     }
-    children
+    resolve_duplicate_function_names_of_directory_items(children)
 }
 
-fn sort_based_on_order(items: Values) -> Vec<&Value> {
+fn sort_items_by_order(items: Values) -> Vec<&Value> {
     let mut items: Vec<&Value> = items.collect();
     items.sort_by(|item_a, item_b| {
         item_a
             .get("order")
             .unwrap_or(&Value::Null)
             .as_i64()
             .unwrap_or(-1)
@@ -121,50 +87,140 @@
                     .as_i64()
                     .unwrap_or(-1),
             )
     });
     items
 }
 
-/// `parent_name: None` represents the root
-fn filter_out_children_of_parent(
-    items: &mut Vec<&Value>,
+/// The key of the root directory is `None`
+///
+/// Returns the removed children
+fn remove_children_of_parent_in_items<'a>(
     parent_key: Option<&str>,
-) -> Vec<DirectoryItem> {
+    items: &mut Vec<&'a Value>,
+) -> Vec<&'a Value> {
     let mut children = Vec::new();
-    items.retain(|item| {
+    items.retain(|&item| {
         let item_parent = item.get("parent").unwrap_or(&Value::Null).as_str();
         if item_parent == parent_key {
-            children.push(DirectoryItem::parse(&item));
+            children.push(item);
             return false;
         }
         true
     });
     children
 }
 
+fn resolve_duplicate_function_names_of_directory_items(
+    mut directory_items: Vec<DirectoryItem>,
+) -> Vec<DirectoryItem> {
+    let mut function_names_to_occurances: HashMap<String, usize> = HashMap::new();
+    let mut stack: VecDeque<&mut DirectoryItem> = directory_items.iter_mut().collect();
+    while stack.len() > 0 {
+        let current_item = stack.pop_front().unwrap();
+        match current_item {
+            DirectoryItem::Script(script) => {
+                let function_name = script.function_name.clone();
+                if let Some(occurances) = function_names_to_occurances.get(&function_name) {
+                    script.function_name = format!("{}_{occurances}", function_name);
+                }
+                function_names_to_occurances.insert(
+                    function_name.clone(),
+                    function_names_to_occurances
+                        .get(&function_name)
+                        .unwrap_or(&0)
+                        + 1,
+                );
+            }
+            DirectoryItem::Directory(dir) => {
+                stack.extend(dir.children.iter_mut().collect::<Vec<&mut DirectoryItem>>())
+            }
+        }
+    }
+    directory_items
+}
+
+#[derive(Debug, PartialEq, Eq)]
+pub enum DirectoryItem {
+    Directory(Directory),
+    Script(Script),
+}
+
+fn parse_key_of_item_to_string(key: &str, item_data: &Value) -> String {
+    item_data
+        .get(key)
+        .unwrap_or(&Value::Null)
+        .as_str()
+        .unwrap_or(UNDEFINED_STRING)
+        .to_string()
+}
+
+impl DirectoryItem {
+    fn parse(item_data: &Value) -> DirectoryItem {
+        match item_data.get("actions") {
+            Some(actions) => DirectoryItem::Script({
+                Script::new(
+                    parse_key_of_item_to_string("name", &item_data),
+                    parse_key_of_item_to_string("key", &item_data),
+                    item_data
+                        .get("triggers")
+                        .unwrap_or(&Value::Null)
+                        .as_array()
+                        .unwrap_or(&Vec::new())
+                        .into_iter()
+                        .map(|trigger| parse_key_of_item_to_string("type", &trigger))
+                        .collect(),
+                    actions::parse_actions(actions.as_array().unwrap_or(&Vec::new())),
+                )
+            }),
+            None => DirectoryItem::Directory(Directory {
+                children: Vec::new(),
+                name: parse_key_of_item_to_string("folderName", &item_data),
+                key: parse_key_of_item_to_string("key", &item_data),
+            }),
+        }
+    }
+}
+
 #[derive(Debug, PartialEq, Eq)]
 pub struct Script {
     pub name: String,
+    pub function_name: String,
     pub key: String,
     pub triggers: Vec<String>,
     pub actions: Vec<Action>,
 }
 
 impl Script {
-    pub fn pymodd_function_name(&self) -> String {
-        let mut function_name = self.name.replace(['\'', '\"'], "").to_snake_case();
-        // use script key as name if script name is empty
+    fn new(name: String, key: String, triggers: Vec<String>, actions: Vec<Action>) -> Script {
+        Script {
+            function_name: Script::function_name_of(&name).unwrap_or(
+                Script::function_name_of(&key.to_lowercase()).unwrap_or(String::from("undefined")),
+            ),
+            name,
+            key,
+            triggers,
+            actions,
+        }
+    }
+
+    fn function_name_of(name: &str) -> Option<String> {
+        let function_name = name
+            .replace(
+                |c: char| !(c.is_alphabetic() || c.is_digit(10) || [' ', '_'].contains(&c)),
+                "",
+            )
+            .to_snake_case();
         if function_name.is_empty() {
-            function_name = self.key.to_string().to_lowercase()
+            return None;
         }
         if !is_valid_class_name(&function_name) {
-            format!("q{function_name}")
+            Some(format!("x{function_name}"))
         } else {
-            function_name
+            Some(function_name)
         }
     }
 
     pub fn triggers_into_pymodd_enums(&self) -> Vec<String> {
         self.triggers
             .iter()
             .map(|trigger| {
@@ -184,30 +240,51 @@
     use crate::game_data::{
         actions::Action,
         directory::{
             root_children_from_scripts_data, Directory, DirectoryItem, Script, UNDEFINED_STRING,
         },
     };
 
-    use super::filter_out_children_of_parent;
+    use super::remove_children_of_parent_in_items;
 
     impl Directory {
         pub fn new(name: &str, key: &str, children: Vec<DirectoryItem>) -> Directory {
             Directory {
                 name: name.to_string(),
                 key: key.to_string(),
                 children,
             }
         }
     }
 
     impl Script {
-        pub fn new(name: &str, key: &str, triggers: Vec<&str>, actions: Vec<Action>) -> Script {
+        /// q (quick) new function
+        pub fn qnew(name: &str, key: &str, triggers: Vec<&str>, actions: Vec<Action>) -> Script {
+            Script::new(
+                name.to_string(),
+                key.to_string(),
+                triggers
+                    .into_iter()
+                    .map(|string| string.to_string())
+                    .collect(),
+                actions,
+            )
+        }
+
+        /// f (full) new function
+        pub fn fnew(
+            name: &str,
+            function_name: &str,
+            key: &str,
+            triggers: Vec<&str>,
+            actions: Vec<Action>,
+        ) -> Script {
             Script {
                 name: name.to_string(),
+                function_name: function_name.to_string(),
                 key: key.to_string(),
                 triggers: triggers
                     .into_iter()
                     .map(|string| string.to_string())
                     .collect(),
                 actions,
             }
@@ -224,66 +301,90 @@
                                 "key": None::<&str>, "actions": [], "parent": "31IAD2B", "order": 2 },
                 "SDUW31W": { "triggers": [], "name": "change_state",
                                 "key": "SDUW31W", "actions": [], "parent": "31IAD2B", "order": 1 },
                 "HWI31WQ": { "triggers": [], "folderName": "other",
                                 "key": "HWI31WQ", "parent": "31IAD2B", "order": 3 },
                 "JK32Q03": { "triggers": [], "name": "destroy_server",
                                 "key": "JK32Q03", "actions": [], "parent": "HWI31WQ", "order": 1},
-                "WI31HDK": { "triggers": [ { "type": "gameStart"} ], "name": "initialize",
-                                "key": "WI31HDK", "actions": [], "parent": None::<&str>, "order": 1},
+                "3WI1HDK": { "triggers": [ { "type": "gameStart"} ], "name": "",
+                                "key": "3WI1HDK", "actions": [], "parent": None::<&str>, "order": 1},
             }))
             .as_slice(),
             [
-                DirectoryItem::Script(Script::new("initialize", "WI31HDK", vec!["gameStart"], Vec::new())),
+                DirectoryItem::Script(Script::fnew("", "x3wi1hdk", "3WI1HDK", vec!["gameStart"], Vec::new())),
                 DirectoryItem::Directory(Directory::new(
                     "utils",
                     "31IAD2B",
                     vec![
-                        DirectoryItem::Script(Script::new(
+                        DirectoryItem::Script(Script::qnew(
                             "change_state",
                             "SDUW31W",
                             vec![],
                             Vec::new()
                         )),
-                        DirectoryItem::Script(Script::new(
+                        DirectoryItem::Script(Script::qnew(
                             "check_players",
                             UNDEFINED_STRING,
                             vec!["secondTick"],
                             Vec::new()
                         )),
                         DirectoryItem::Directory(Directory::new(
                             "other",
                             "HWI31WQ",
-                            vec![DirectoryItem::Script(Script::new(
+                            vec![DirectoryItem::Script(Script::qnew(
                                 "destroy_server",
                                 "JK32Q03",
                                 vec![],
                                 Vec::new()
                             )),]
                         )),
                     ]
                 )),
             ]
         );
     }
 
     #[test]
+    fn parse_directory_of_scripts_with_same_function_name() {
+        assert_eq!(
+            root_children_from_scripts_data(&json!({
+                "Q31E2RS": { "triggers": [], "name": "destroy server",
+                                "key": "Q31E2RS", "actions": [], "parent": None::<&str>, "order": 1 },
+                "SDUW31W": { "triggers": [], "name": "destroy server",
+                                "key": "SDUW31W", "actions": [], "parent": None::<&str>, "order": 2 },
+                "JK32Q03": { "triggers": [], "name": "destroy server",
+                                "key": "JK32Q03", "actions": [], "parent": None::<&str>, "order": 3 },
+            }))
+            .as_slice(),
+            [
+                DirectoryItem::Script(Script::fnew("destroy server", "destroy_server", "Q31E2RS", Vec::new(), Vec::new())),
+                DirectoryItem::Script(Script::fnew("destroy server", "destroy_server_1", "SDUW31W", Vec::new(), Vec::new())),
+                DirectoryItem::Script(Script::fnew("destroy server", "destroy_server_2", "JK32Q03", Vec::new(), Vec::new())),
+            ]
+        );
+    }
+
+    #[test]
     fn filter_out_children_of_parent_from_items() {
         let data = &mut json!([
            { "name": "initialize", "key": "WI31HDK", "actions": [], "parent": None::<&str>, "order": 1},
            { "name": "change_state", "key": "SDUW31W", "actions": [], "parent": "31IAD2B", "order": 1 },
            { "name": "check_players", "key": "FWJ31WD", "actions": [], "parent": "31IAD2B", "order": 2 },
         ]);
         let mut items: Vec<&Value> = data.as_array().unwrap().iter().collect();
 
         assert_eq!(
-            filter_out_children_of_parent(&mut items, Some("31IAD2B")).as_slice(),
+            remove_children_of_parent_in_items(Some("31IAD2B"), &mut items)
+                .into_iter()
+                .map(|val| DirectoryItem::parse(val))
+                .collect::<Vec<DirectoryItem>>()
+                .as_slice(),
             [
-                DirectoryItem::Script(Script::new("change_state", "SDUW31W", vec![], Vec::new())),
-                DirectoryItem::Script(Script::new("check_players", "FWJ31WD", vec![], Vec::new())),
+                DirectoryItem::Script(Script::qnew("change_state", "SDUW31W", vec![], Vec::new())),
+                DirectoryItem::Script(Script::qnew("check_players", "FWJ31WD", vec![], Vec::new())),
             ]
         );
         assert_eq!(
             items.as_slice(),
             json!([
                { "name": "initialize", "key": "WI31HDK", "actions": [], "parent": None::<&str>, "order": 1},
             ]).as_array().unwrap().iter().collect::<Vec<&Value>>().as_slice(),
```

### Comparing `pymodd-1.0.3/src/game_data/entity_types.rs` & `pymodd-1.0.4/src/game_data/entity_types.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/game_data/variable_categories.rs` & `pymodd-1.0.4/src/game_data/variable_categories.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/game_data.rs` & `pymodd-1.0.4/src/game_data.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/lib.rs` & `pymodd-1.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/project_generator/entity_scripts_file.rs` & `pymodd-1.0.4/src/project_generator/entity_scripts_file.rs`

 * *Files 1% similar despite different names*

```diff
@@ -149,22 +149,22 @@
 ) -> String {
     if let Some(key) = key {
         if is_entity_type_script {
             if let DirectoryIterItem::Script(script) = entity_type_directory
                 .find_item_with_key(&key)
                 .unwrap_or(DirectoryIterItem::DirectoryEnd)
             {
-                return format!("self.{}()", script.pymodd_function_name());
+                return format!("self.{}()", script.function_name);
             };
         } else {
             if let DirectoryIterItem::Script(script) = game_directory
                 .find_item_with_key(&key)
                 .unwrap_or(DirectoryIterItem::DirectoryEnd)
             {
-                return format!("{}()", script.pymodd_function_name());
+                return format!("{}()", script.function_name);
             };
         };
     }
     String::from("None")
 }
 
 fn build_directory_elements_for_entity_type(entity_type: &EntityType) -> Vec<String> {
@@ -266,20 +266,20 @@
                         Keybinding::new("z", None, false, None, false)
                     ]
                 },
                 "unitTypes",
                 &Directory::new(
                     "root",
                     "null",
-                    vec![DirectoryItem::Script(Script {
-                        name: String::from("EndGame"),
-                        key: String::from("3FJ31WD"),
-                        triggers: Vec::new(),
-                        actions: Vec::new(),
-                    })]
+                    vec![DirectoryItem::Script(Script::qnew(
+                        "EndGame",
+                        "3FJ31WD",
+                        Vec::new(),
+                        Vec::new(),
+                    ))]
                 )
             )
             .as_str(),
             "class Bob(EntityScripts):\n\
                 \tdef _build(self):\n\
                     \t\tself.entity_type = UnitType.BOB\n\
                     \t\tself.keybindings = {\n\
```

### Comparing `pymodd-1.0.3/src/project_generator/game_variables_file.rs` & `pymodd-1.0.4/src/project_generator/game_variables_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/project_generator/mapping_file.rs` & `pymodd-1.0.4/src/project_generator/mapping_file.rs`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                     surround_string_with_quotes(&directory.name)
                 )
             }
             DirectoryIterItem::Script(script) => {
                 format!(
                     "{}{}(),",
                     "\t".repeat(curr_depth),
-                    script.pymodd_function_name()
+                    script.function_name
                 )
             }
             DirectoryIterItem::DirectoryEnd => {
                 curr_depth -= 1;
                 format!("{}]),", "\t".repeat(curr_depth))
             }
         })
```

### Comparing `pymodd-1.0.3/src/project_generator/scripts_file.rs` & `pymodd-1.0.4/src/project_generator/scripts_file.rs`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         ScriptsContentBuilder {
             categories_to_variables,
             root_directory,
         }
     }
 
     pub fn build_script_content(&self, script: &Script) -> String {
-        let function_name = script.pymodd_function_name();
+        let function_name = &script.function_name;
         format!(
             "@script(triggers=[{}]{})\n\
             def {function_name}():\n\
                 {}",
             script.triggers_into_pymodd_enums().join(", "),
             if script.name.is_ascii() {
                 String::new()
@@ -409,15 +409,15 @@
                 self.build_operation_content(&operation)
             }
             ArgumentValueIterItem::ScriptKey(key) => {
                 let item_with_key = self.root_directory.find_item_with_key(&key);
                 if item_with_key.is_some() {
                     if let DirectoryIterItem::Script(script) = item_with_key.unwrap() {
                         // run_script action accepts Script objects, not keys
-                        return format!("{}()", script.pymodd_function_name());
+                        return format!("{}()", script.function_name);
                     }
                 }
                 String::from("None")
             }
             ArgumentValueIterItem::None => String::from("None"),
             ArgumentValueIterItem::FunctionEnd => String::from(")"),
         }
@@ -513,15 +513,15 @@
     #[test]
     fn script_content() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
-            .build_script_content(&Script::new(
+            .build_script_content(&Script::qnew(
                 "initialize",
                 "WI31HDK",
                 vec!["gameStart"],
                 Vec::new()
             )),
             String::from(format!(
                 "@script(triggers=[Trigger.GAME_START])\n\
@@ -534,15 +534,15 @@
     #[test]
     fn script_with_non_ascii_name_content() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
-            .build_script_content(&Script::new(
+            .build_script_content(&Script::qnew(
                 "【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】",
                 "WI31HDK",
                 vec!["gameStart"],
                 Vec::new()
             )),
             String::from(format!(
                 "@script(triggers=[Trigger.GAME_START], name='【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】')\n\
@@ -555,20 +555,15 @@
     #[test]
     fn script_with_no_name() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
-            .build_script_content(&Script::new(
-                "",
-                "WI31HDK",
-                vec![],
-                Vec::new()
-            )),
+            .build_script_content(&Script::qnew("", "WI31HDK", vec![], Vec::new())),
             String::from(format!(
                 "@script(triggers=[])\n\
                 def wi31hdk():\n\
                     \tpass\n",
             ))
         );
     }
@@ -576,15 +571,15 @@
     #[test]
     fn script_content_with_commented_body() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
-            .build_script_content(&Script::new(
+            .build_script_content(&Script::qnew(
                 "initialize",
                 "WI31HDK",
                 vec!["gameStart"],
                 vec![Action::new("break", vec![], None, false, true)]
             )),
             String::from(format!(
                 "@script(triggers=[Trigger.GAME_START])\n\
@@ -1187,20 +1182,20 @@
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new(
                     "root",
                     "null",
                     vec![DirectoryItem::Directory(Directory::new(
                         "utils",
                         "n3DhW3",
-                        vec![DirectoryItem::Script(Script {
-                            name: String::from("spawn boss"),
-                            key: String::from("If2aW3B"),
-                            triggers: Vec::new(),
-                            actions: Vec::new()
-                        })]
+                        vec![DirectoryItem::Script(Script::qnew(
+                            "spawn boss",
+                            "If2aW3B",
+                            Vec::new(),
+                            Vec::new()
+                        ))]
                     ))]
                 )
             )
             .build_actions_content(&parse_actions(
                 json!([
                      { "type": "runScript", "scriptName": "If2aW3B" }
                 ])
```

### Comparing `pymodd-1.0.3/src/project_generator/utils/iterators/argument_values_iterator.rs` & `pymodd-1.0.4/src/project_generator/utils/iterators/argument_values_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/project_generator/utils/iterators/directory_iterator.rs` & `pymodd-1.0.4/src/project_generator/utils/iterators/directory_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/project_generator/utils/to_pymodd_maps.rs` & `pymodd-1.0.4/src/project_generator/utils/to_pymodd_maps.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/src/project_generator/utils.rs` & `pymodd-1.0.4/src/project_generator/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pub(crate) fn is_valid_class_name(class_name: &str) -> bool {
     !(class_name.is_empty()
         || string_starts_with_a_number(&class_name)
         || type_conflicts_with_a_category_class_name(&class_name))
 }
 
 fn string_starts_with_a_number(string: &str) -> bool {
-    string.chars().next().unwrap().is_numeric()
+    string.chars().next().unwrap().is_digit(10)
 }
 
 fn type_conflicts_with_a_category_class_name(class_name: &str) -> bool {
     SEPERATED_VARIABLE_CATEGORIES
         .into_iter()
         .chain([VARIABLES_CATEGORY_NAME])
         .collect::<Vec<&str>>()
```

### Comparing `pymodd-1.0.3/src/project_generator.rs` & `pymodd-1.0.4/src/project_generator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.3/Cargo.lock` & `pymodd-1.0.4/Cargo.lock`

 * *Files identical despite different names*

