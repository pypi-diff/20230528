# Comparing `tmp/pytest_lazy_fixtures-1.0.0.tar.gz` & `tmp/pytest_lazy_fixtures-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_lazy_fixtures-1.0.0.tar", max compression
+gzip compressed data, was "pytest_lazy_fixtures-1.0.1.tar", max compression
```

## Comparing `pytest_lazy_fixtures-1.0.0.tar` & `pytest_lazy_fixtures-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/LICENSE
--rw-r--r--   0        0        0     3669 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/README.md
--rw-r--r--   0        0        0     1578 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/__init__.py
--rw-r--r--   0        0        0      839 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/lazy_fixture.py
--rw-r--r--   0        0        0      966 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/lazy_fixture_callable.py
--rw-r--r--   0        0        0      761 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/loader.py
--rw-r--r--   0        0        0      427 2023-03-11 10:18:56.922311 pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/plugin.py
--rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 pytest_lazy_fixtures-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3669 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/README.md
+-rw-r--r--   0        0        0     1578 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/__init__.py
+-rw-r--r--   0        0        0      839 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/lazy_fixture.py
+-rw-r--r--   0        0        0      966 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/lazy_fixture_callable.py
+-rw-r--r--   0        0        0      761 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/loader.py
+-rw-r--r--   0        0        0      427 2023-05-28 09:23:50.103144 pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/plugin.py
+-rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 pytest_lazy_fixtures-1.0.1/PKG-INFO
```

### Comparing `pytest_lazy_fixtures-1.0.0/LICENSE` & `pytest_lazy_fixtures-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_lazy_fixtures-1.0.0/README.md` & `pytest_lazy_fixtures-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_lazy_fixtures-1.0.0/pyproject.toml` & `pytest_lazy_fixtures-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pytest-lazy-fixtures"
-version = "1.0.0"
+version = "1.0.1"
 description = "Allows you to use fixtures in @pytest.mark.parametrize."
 authors = ["Petrov Anton <antonp2@yandex.ru>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/dev-petrov/pytest-lazy-fixtures"
 repository = "https://github.com/dev-petrov/pytest-lazy-fixtures"
 keywords = ["tests", "pytest", "lazy", "fixture"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pytest = "^7.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 pre-commit = "^2.20.0"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.254"
```

### Comparing `pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/lazy_fixture.py` & `pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/lazy_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/lazy_fixture_callable.py` & `pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/lazy_fixture_callable.py`

 * *Files identical despite different names*

### Comparing `pytest_lazy_fixtures-1.0.0/pytest_lazy_fixtures/loader.py` & `pytest_lazy_fixtures-1.0.1/pytest_lazy_fixtures/loader.py`

 * *Files identical despite different names*

### Comparing `pytest_lazy_fixtures-1.0.0/PKG-INFO` & `pytest_lazy_fixtures-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pytest-lazy-fixtures
-Version: 1.0.0
+Version: 1.0.1
 Summary: Allows you to use fixtures in @pytest.mark.parametrize.
 Home-page: https://github.com/dev-petrov/pytest-lazy-fixtures
 License: MIT
 Keywords: tests,pytest,lazy,fixture
 Author: Petrov Anton
 Author-email: antonp2@yandex.ru
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Project-URL: Repository, https://github.com/dev-petrov/pytest-lazy-fixtures
 Description-Content-Type: text/markdown
```

