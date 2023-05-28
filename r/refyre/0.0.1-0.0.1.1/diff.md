# Comparing `tmp/refyre-0.0.1.tar.gz` & `tmp/refyre-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refyre-0.0.1.tar", max compression
+gzip compressed data, was "refyre-0.0.1.1.tar", max compression
```

## Comparing `refyre-0.0.1.tar` & `refyre-0.0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      355 2023-05-28 20:41:21.539834 refyre-0.0.1/README.md
--rw-r--r--   0        0        0      817 2023-05-28 20:41:21.539834 refyre-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    18563 2023-05-28 20:41:21.539834 refyre-0.0.1/refyre/Refyre.py
--rw-r--r--   0        0        0      115 2023-05-28 20:41:21.539834 refyre-0.0.1/refyre/__init__.py
--rw-r--r--   0        0        0      441 2023-05-28 20:41:21.539834 refyre-0.0.1/refyre/core/AliasManager.py
--rw-r--r--   0        0        0      641 2023-05-28 20:41:21.539834 refyre-0.0.1/refyre/core/CodeManager.py
--rw-r--r--   0        0        0     2595 2023-05-28 20:41:21.539834 refyre-0.0.1/refyre/core/RecipePreprocessor.py
--rw-r--r--   0        0        0      126 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/core/__init__.py
--rw-r--r--   0        0        0     1532 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/datastack/DataStack.py
--rw-r--r--   0        0        0       34 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/datastack/__init__.py
--rw-r--r--   0        0        0     8380 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fcluster/AutoRefresher.py
--rw-r--r--   0        0        0    11904 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fcluster/FileCluster.py
--rw-r--r--   0        0        0      355 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fcluster/FileClusterIterator.py
--rw-r--r--   0        0        0       77 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fcluster/__init__.py
--rw-r--r--   0        0        0      802 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fgraph/FileGraph.py
--rw-r--r--   0        0        0     2012 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fgraph/FileGraphNode.py
--rw-r--r--   0        0        0       73 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/fgraph/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/ExpressionGenerator.py
--rw-r--r--   0        0        0     5585 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/Lexer.py
--rw-r--r--   0        0        0     2776 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/Parser.py
--rw-r--r--   0        0        0     1411 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/PatternGenerator.py
--rw-r--r--   0        0        0      270 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/__init__.py
--rw-r--r--   0        0        0      760 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/cogs/LexerToken.py
--rw-r--r--   0        0        0     2719 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/cogs/VariableParser.py
--rw-r--r--   0        0        0      618 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/reader/cogs/lexer_utils.py
--rw-r--r--   0        0        0      136 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/utils/__init__.py
--rw-r--r--   0        0        0      617 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/utils/clone.py
--rw-r--r--   0        0        0      413 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/utils/optional_imports.py
--rw-r--r--   0        0        0      589 2023-05-28 20:41:21.543834 refyre-0.0.1/refyre/utils/regex.py
--rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 refyre-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      355 2023-05-28 20:52:17.373930 refyre-0.0.1.1/README.md
+-rw-r--r--   0        0        0      814 2023-05-28 20:52:17.373930 refyre-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18563 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/Refyre.py
+-rw-r--r--   0        0        0      115 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/__init__.py
+-rw-r--r--   0        0        0      441 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/core/AliasManager.py
+-rw-r--r--   0        0        0      641 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/core/CodeManager.py
+-rw-r--r--   0        0        0     2595 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/core/RecipePreprocessor.py
+-rw-r--r--   0        0        0      126 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/core/__init__.py
+-rw-r--r--   0        0        0     1532 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/datastack/DataStack.py
+-rw-r--r--   0        0        0       34 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/datastack/__init__.py
+-rw-r--r--   0        0        0     8380 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fcluster/AutoRefresher.py
+-rw-r--r--   0        0        0    11904 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fcluster/FileCluster.py
+-rw-r--r--   0        0        0      355 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fcluster/FileClusterIterator.py
+-rw-r--r--   0        0        0       77 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fcluster/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fgraph/FileGraph.py
+-rw-r--r--   0        0        0     2012 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fgraph/FileGraphNode.py
+-rw-r--r--   0        0        0       73 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/fgraph/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/ExpressionGenerator.py
+-rw-r--r--   0        0        0     5585 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/Lexer.py
+-rw-r--r--   0        0        0     2776 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/Parser.py
+-rw-r--r--   0        0        0     1411 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/PatternGenerator.py
+-rw-r--r--   0        0        0      270 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/__init__.py
+-rw-r--r--   0        0        0      760 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/cogs/LexerToken.py
+-rw-r--r--   0        0        0     2719 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/cogs/VariableParser.py
+-rw-r--r--   0        0        0      618 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/reader/cogs/lexer_utils.py
+-rw-r--r--   0        0        0      136 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/utils/__init__.py
+-rw-r--r--   0        0        0      617 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/utils/clone.py
+-rw-r--r--   0        0        0      413 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/utils/optional_imports.py
+-rw-r--r--   0        0        0      589 2023-05-28 20:52:17.373930 refyre-0.0.1.1/refyre/utils/regex.py
+-rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 refyre-0.0.1.1/PKG-INFO
```

### Comparing `refyre-0.0.1/pyproject.toml` & `refyre-0.0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refyre"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Filesystem dominance is all you need."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/refyre"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
@@ -23,12 +23,12 @@
 python = ">=3.7"
 
 
 [tool.poetry.dev-dependencies]
 pytest = {version="^7.0.1", python = ">=3.7,<4.0"}
 
 [tool.poetry.scripts]
-refyre = "cli:__main__"
+refyre = "cli:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `refyre-0.0.1/refyre/Refyre.py` & `refyre-0.0.1.1/refyre/Refyre.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/core/CodeManager.py` & `refyre-0.0.1.1/refyre/core/CodeManager.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/core/RecipePreprocessor.py` & `refyre-0.0.1.1/refyre/core/RecipePreprocessor.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/datastack/DataStack.py` & `refyre-0.0.1.1/refyre/datastack/DataStack.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/fcluster/AutoRefresher.py` & `refyre-0.0.1.1/refyre/fcluster/AutoRefresher.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/fcluster/FileCluster.py` & `refyre-0.0.1.1/refyre/fcluster/FileCluster.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/fgraph/FileGraph.py` & `refyre-0.0.1.1/refyre/fgraph/FileGraph.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/fgraph/FileGraphNode.py` & `refyre-0.0.1.1/refyre/fgraph/FileGraphNode.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/ExpressionGenerator.py` & `refyre-0.0.1.1/refyre/reader/ExpressionGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/Lexer.py` & `refyre-0.0.1.1/refyre/reader/Lexer.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/Parser.py` & `refyre-0.0.1.1/refyre/reader/Parser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/PatternGenerator.py` & `refyre-0.0.1.1/refyre/reader/PatternGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/cogs/LexerToken.py` & `refyre-0.0.1.1/refyre/reader/cogs/LexerToken.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/cogs/VariableParser.py` & `refyre-0.0.1.1/refyre/reader/cogs/VariableParser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/reader/cogs/lexer_utils.py` & `refyre-0.0.1.1/refyre/reader/cogs/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/utils/clone.py` & `refyre-0.0.1.1/refyre/utils/clone.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/refyre/utils/regex.py` & `refyre-0.0.1.1/refyre/utils/regex.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1/PKG-INFO` & `refyre-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refyre
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Filesystem dominance is all you need.
 Home-page: https://github.com/flockfysh/refyre
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.7
```

