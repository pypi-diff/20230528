# Comparing `tmp/folder_tree_generator-0.1.3.tar.gz` & `tmp/folder_tree_generator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folder_tree_generator-0.1.3.tar", max compression
+gzip compressed data, was "folder_tree_generator-0.1.4.tar", max compression
```

## Comparing `folder_tree_generator-0.1.3.tar` & `folder_tree_generator-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     2437 2023-04-11 23:35:17.507501 folder_tree_generator-0.1.3/README.md
--rw-r--r--   0        0        0     3003 2023-04-11 22:24:34.256693 folder_tree_generator-0.1.3/folder_tree_generator.py
--rw-r--r--   0        0        0      562 2023-04-11 23:35:27.187919 folder_tree_generator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 folder_tree_generator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2437 2023-04-12 06:31:17.603738 folder_tree_generator-0.1.4/README.md
+-rw-r--r--   0        0        0     3019 2023-05-28 07:57:42.724341 folder_tree_generator-0.1.4/folder_tree_generator.py
+-rw-r--r--   0        0        0      562 2023-05-28 07:57:14.591770 folder_tree_generator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.4/setup.py
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.4/PKG-INFO
```

### Comparing `folder_tree_generator-0.1.3/README.md` & `folder_tree_generator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `folder_tree_generator-0.1.3/folder_tree_generator.py` & `folder_tree_generator-0.1.4/folder_tree_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # Check if the root folder exists and is a directory
     if not Path(root_folder).is_dir():
         raise ValueError(f"{root_folder} is not a valid directory")
 
     return root_folder
 
 
-def generate_tree(root_folder: str, ignore_file_name: str = ".gitignore") -> str:
+def generate_tree(root_folder: str, ignore_file_name: str) -> str:
     """Generate a tree of a folder."""
     root = Path(root_folder)
     ignorefile_path = root / ignore_file_name
     ignored_patterns = (
         _parse_ignore_patterns(ignorefile_path) if ignorefile_path.exists() else []
     )
 
@@ -86,13 +86,13 @@
     tree_str += _generate_folder_tree(root, ignored_patterns=ignored_patterns)
     return tree_str
 
 
 def _main() -> None:
     """Main function."""
     root_folder = _parse_arguments()
-    output_text = generate_tree(root_folder)
+    output_text = generate_tree(root_folder, ignore_file_name=".gitignore")
     print(output_text)
 
 
 if __name__ == "__main__":
     _main()
```

### Comparing `folder_tree_generator-0.1.3/pyproject.toml` & `folder_tree_generator-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "folder-tree-generator"
-version = "0.1.3"
+version = "0.1.4"
 description = "Takes a folder path and outputs a text representation of the folders and files, supports ignore files."
 authors = ["Sean Dearnaley <SeanDearnaley@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-coverage = "^7.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.2"
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 ruff = "^0.0.261"
 black = "^23.3.0"
 pytest-mock = "^3.10.0"
+coverage = "^7.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `folder_tree_generator-0.1.3/PKG-INFO` & `folder_tree_generator-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: folder-tree-generator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Takes a folder path and outputs a text representation of the folders and files, supports ignore files.
 Author: Sean Dearnaley
 Author-email: SeanDearnaley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: coverage (>=7.2.3,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Folder Tree Generator
 
 
 [![PyPI version](https://badge.fury.io/py/folder-tree-generator.svg)](https://badge.fury.io/py/folder-tree-generator)
```

