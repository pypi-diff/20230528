# Comparing `tmp/crackerjack-0.2.1.tar.gz` & `tmp/crackerjack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.1.tar", last modified: Sat May 27 13:29:37 2023, max compression
+gzip compressed data, was "crackerjack-0.2.2.tar", last modified: Sun May 28 13:33:52 2023, max compression
```

## Comparing `crackerjack-0.2.1.tar` & `crackerjack-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.1/LICENSE
--rw-r--r--   0        0        0     3142 2023-05-26 14:01:21.577314 crackerjack-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-27 13:29:05.329337 crackerjack-0.2.1/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-05-27 13:29:05.314340 crackerjack-0.2.1/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-05-27 13:29:05.325590 crackerjack-0.2.1/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2055 2023-05-27 13:29:05.320587 crackerjack-0.2.1/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.1/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.1/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.1/crackerjack/__init__.py
--rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.1/crackerjack/__main__.py
--rw-r--r--   0        0        0     5554 2023-05-27 13:28:36.772941 crackerjack-0.2.1/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1603 2023-05-27 13:29:06.128636 crackerjack-0.2.1/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1722 2023-05-27 13:29:37.699118 crackerjack-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 crackerjack-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3142 2023-05-26 14:01:21.577314 crackerjack-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 13:33:24.314672 crackerjack-0.2.2/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-05-28 13:33:24.303856 crackerjack-0.2.2/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-05-28 13:33:24.312399 crackerjack-0.2.2/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2055 2023-05-28 13:33:24.308666 crackerjack-0.2.2/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.2/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.2/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.2/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.2/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5554 2023-05-27 13:28:36.772941 crackerjack-0.2.2/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1603 2023-05-28 13:33:25.056325 crackerjack-0.2.2/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1744 2023-05-28 13:33:52.297252 crackerjack-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 crackerjack-0.2.2/PKG-INFO
```

### Comparing `crackerjack-0.2.1/LICENSE` & `crackerjack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/README.md` & `crackerjack-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.2/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.2/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/crackerjack/__main__.py` & `crackerjack-0.2.2/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/crackerjack/crackerjack.py` & `crackerjack-0.2.2/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.1/crackerjack/pyproject.toml` & `crackerjack-0.2.2/crackerjack/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 enable_all = true
 
 [tool.pytype]
 inputs = ["package_name"]
 
 [project]
 name = "Crackerjack"
-version = "0.2.1"
+version = "0.2.2"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = ["black", "ruff", "mypy", "creosote", "refurb"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.11"]
 dependencies = ["click>=8.1.3", "pdoc3>=0.10.0", "pdm-bump>=0.7.0", "pydantic>=1.10.7", "aiopath>=0.6.11", "acb>=0.1.2", "aioconsole>=0.6.1", "inflection>=0.5.1"]
```

### Comparing `crackerjack-0.2.1/pyproject.toml` & `crackerjack-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 [tool.mypy]
 strict = false
 pretty = true
 ignore_missing_imports = false
 plugins = [
     "pydantic.mypy",
 ]
+python_version = 3.11
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
-version = "0.2.1"
+version = "0.2.2"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.2.1/PKG-INFO` & `crackerjack-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.2.1
+Version: 0.2.2
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

