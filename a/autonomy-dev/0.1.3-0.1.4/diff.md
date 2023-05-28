# Comparing `tmp/autonomy_dev-0.1.3.tar.gz` & `tmp/autonomy_dev-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.3.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.4.tar", max compression
```

## Comparing `autonomy_dev-0.1.3.tar` & `autonomy_dev-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      578 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/LICENSE
--rw-r--r--   0        0        0      117 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/__init__.py
--rw-r--r--   0        0        0     3151 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/cli.py
--rw-r--r--   0        0        0     2732 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/cli_executor.py
--rw-r--r--   0        0        0      301 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/constants.py
--rw-r--r--   0        0        0      529 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      464 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/test.py
--rw-r--r--   0        0        0     1083 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/utils.py
--rw-r--r--   0        0        0     2516 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/tests/test_cli.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 autonomy_dev-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/LICENSE
+-rw-r--r--   0        0        0      117 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/__init__.py
+-rw-r--r--   0        0        0     3151 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/cli.py
+-rw-r--r--   0        0        0     2732 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0      301 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/constants.py
+-rw-r--r--   0        0        0      577 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      464 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/test.py
+-rw-r--r--   0        0        0     1083 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/utils.py
+-rw-r--r--   0        0        0     2518 2023-05-28 17:46:15.833622 autonomy_dev-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1187 2023-05-28 17:46:15.833622 autonomy_dev-0.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 autonomy_dev-0.1.4/PKG-INFO
```

### Comparing `autonomy_dev-0.1.3/LICENSE` & `autonomy_dev-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.3/auto_dev/cli.py` & `autonomy_dev-0.1.4/auto_dev/cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.3/auto_dev/cli_executor.py` & `autonomy_dev-0.1.4/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.3/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.4/auto_dev/data/pylama.ini`

 * *Files 11% similar despite different names*

```diff
@@ -22,7 +22,13 @@
     .vscode,
     .github,
     .history,
     .idea
 
 [pylama:vulture]
 min-confidence = 90
+
+
+[pylama:mypy]
+ignore_missing_imports = True
+
+
```

### Comparing `autonomy_dev-0.1.3/auto_dev/utils.py` & `autonomy_dev-0.1.4/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.3/pyproject.toml` & `autonomy_dev-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -22,15 +22,15 @@
     { include = "auto_dev" },
     { include = "tests", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0"
-click = "8.0.2"
+click = ">=8.0.2"
 black = "^22.6.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 pytest-cov = "^3.0.0"
 tox = "^3.25.1"
 pip = "^22.2.2"
 mkdocs = "^1.3.1"
```

### Comparing `autonomy_dev-0.1.3/tests/test_cli.py` & `autonomy_dev-0.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.3/PKG-INFO` & `autonomy_dev-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,26 +12,23 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
-Requires-Dist: click (==8.0.2)
+Requires-Dist: click (>=8.0.2)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
```

