# Comparing `tmp/phantom-types-1.2.2.tar.gz` & `tmp/phantom-types-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phantom-types-1.2.2.tar", last modified: Thu Mar 16 10:15:26 2023, max compression
+gzip compressed data, was "phantom-types-2.0.0.tar", last modified: Sun May 28 14:51:58 2023, max compression
```

## Comparing `phantom-types-1.2.2.tar` & `phantom-types-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-16 10:15:10.000000 phantom-types-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 10:15:10.000000 phantom-types-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-16 10:15:26.620258 phantom-types-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-03-16 10:15:10.000000 phantom-types-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-16 10:15:10.000000 phantom-types-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-16 10:15:26.620258 phantom-types-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 10:15:10.000000 phantom-types-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.616258 phantom-types-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/src/phantom/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_hypothesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/src/phantom/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/_utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/src/phantom/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/ext/phonenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/iso3166.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/negated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/src/phantom/predicates/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/predicates/re.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-03-16 10:15:10.000000 phantom-types-1.2.2/src/phantom/sized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:15:26.620258 phantom-types-1.2.2/src/phantom_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-16 10:15:26.000000 phantom-types-1.2.2/src/phantom_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-16 10:15:26.000000 phantom-types-1.2.2/src/phantom_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:15:26.000000 phantom-types-1.2.2/src/phantom_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-16 10:15:26.000000 phantom-types-1.2.2/src/phantom_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 10:15:26.000000 phantom-types-1.2.2/src/phantom_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.614686 phantom-types-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-28 14:51:49.000000 phantom-types-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 14:51:49.000000 phantom-types-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-28 14:51:58.614686 phantom-types-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-28 14:51:49.000000 phantom-types-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-28 14:51:49.000000 phantom-types-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-28 14:51:58.614686 phantom-types-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:51:49.000000 phantom-types-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.606685 phantom-types-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.610686 phantom-types-2.0.0/src/phantom/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/_hypothesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.610686 phantom-types-2.0.0/src/phantom/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/_utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.610686 phantom-types-2.0.0/src/phantom/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/ext/phonenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/iso3166.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/negated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.610686 phantom-types-2.0.0/src/phantom/predicates/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/predicates/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-28 14:51:49.000000 phantom-types-2.0.0/src/phantom/sized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:58.614686 phantom-types-2.0.0/src/phantom_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-28 14:51:58.000000 phantom-types-2.0.0/src/phantom_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-28 14:51:58.000000 phantom-types-2.0.0/src/phantom_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:51:58.000000 phantom-types-2.0.0/src/phantom_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-28 14:51:58.000000 phantom-types-2.0.0/src/phantom_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 14:51:58.000000 phantom-types-2.0.0/src/phantom_types.egg-info/top_level.txt
```

### Comparing `phantom-types-1.2.2/LICENSE` & `phantom-types-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/PKG-INFO` & `phantom-types-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 1.2.2
+Version: 2.0.0
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: phonenumbers
 Provides-Extra: pydantic
 Provides-Extra: dateutil
 Provides-Extra: hypothesis
 Provides-Extra: all
 Provides-Extra: test
```

### Comparing `phantom-types-1.2.2/README.md` & `phantom-types-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/pyproject.toml` & `phantom-types-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests", "src", "docs"]
 addopts = "--mypy-ini-file=setup.cfg --mypy-only-local-stub --doctest-modules"
 markers = [
   "external: mark tests that require extra dependencies",
   "no_external: mark tests that will fail if run with extra dependencies",
 ]
 
 [tool.ruff]
 fix = true
-target-version = "py37"
+target-version = "py38"
 extend-select = [
   # bugbear
   "B",
   # comprehensions
   "C4",
   # mccabe
   "C90",
```

### Comparing `phantom-types-1.2.2/setup.cfg` & `phantom-types-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Development Status :: 5 - Production/Stable
 author = Anton Agestam
 author_email = git@antonagestam.se
@@ -26,20 +25,19 @@
 	Documentation = https://phantom-types.readthedocs.io/en/stable/
 
 [options]
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	typeguard>=2.10,<3
 	typing_extensions>=4.3.0
-	numerary>=0.3.0,<0.4; python_version<'3.8'
-	numerary>=0.4.3; python_version>='3.8'
+	numerary>=0.4.3
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 phantom = py.typed
 
@@ -60,15 +58,15 @@
 test = 
 	mypy>=0.991
 	pytest
 	pytest-mypy-plugins>=1.9.3
 	coverage
 
 [mypy]
-python_version = 3.7
+python_version = 3.8
 show_error_codes = True
 pretty = True
 files = src, tests
 ignore_missing_imports = False
 no_implicit_reexport = True
 no_implicit_optional = True
 strict_equality = True
```

### Comparing `phantom-types-1.2.2/src/phantom/__init__.py` & `phantom-types-2.0.0/src/phantom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ._base import Phantom
 from ._base import PhantomBase
 from ._base import PhantomMeta
 from .bounds import get_bound_parser
 from .errors import BoundError
 from .predicates import Predicate
 
-__version__ = "1.2.2"
+__version__ = "2.0.0"
 __all__ = (
     "BoundError",
     "Phantom",
     "PhantomBase",
     "PhantomMeta",
     "get_bound_parser",
     "Predicate",
```

### Comparing `phantom-types-1.2.2/src/phantom/_base.py` & `phantom-types-2.0.0/src/phantom/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import abc
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Generic
 from typing import Iterable
 from typing import Iterator
+from typing import Protocol
 from typing import TypeVar
-
-from typing_extensions import Protocol
-from typing_extensions import runtime_checkable
+from typing import runtime_checkable
 
 from . import _hypothesis
 from ._utils.misc import BoundType
 from ._utils.misc import UnresolvedClassAttribute
 from ._utils.misc import fully_qualified_name
 from ._utils.misc import is_not_known_mutable_type
 from ._utils.misc import is_subtype
```

### Comparing `phantom-types-1.2.2/src/phantom/_hypothesis.py` & `phantom-types-2.0.0/src/phantom/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/_utils/misc.py` & `phantom-types-2.0.0/src/phantom/_utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Workaround for something that looks like this bug
 # https://github.com/pytest-dev/pytest/issues/4386
 from __future__ import annotations
 
 import types
 from dataclasses import is_dataclass
 from itertools import product
+from typing import Final
 from typing import MutableMapping
 from typing import MutableSequence
 from typing import MutableSet
 from typing import NewType
 from typing import Tuple
 from typing import Union
 
-from typing_extensions import Final
 from typing_extensions import TypeGuard
 from typing_extensions import get_args
 from typing_extensions import get_origin
 
 
 class UnresolvedClassAttribute(NotImplementedError):
     ...
@@ -132,15 +132,16 @@
 
 
 def is_not_known_mutable_instance(value: object) -> bool:
     return not (
         isinstance(value, mutable)
         or (
             is_dataclass(value)
-            and not value.__dataclass_params__.frozen  # type: ignore[attr-defined]
+            # https://github.com/python/typeshed/pull/9947#issue-1641078469
+            and not value.__dataclass_params__.frozen  # type: ignore[union-attr]
         )
     )
 
 
 MaybeUnionType: type | None
 try:
     MaybeUnionType = types.UnionType  # type: ignore[attr-defined]
```

### Comparing `phantom-types-1.2.2/src/phantom/_utils/types.py` & `phantom-types-2.0.0/src/phantom/_utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+from typing import Protocol
 from typing import TypeVar
+from typing import runtime_checkable
 
-from typing_extensions import Protocol
-from typing_extensions import runtime_checkable
-
-from .compat import CachingProtocolMeta
+from numerary.protocol import CachingProtocolMeta
 
 T_contra = TypeVar("T_contra", contravariant=True)
 U_co = TypeVar("U_co", covariant=True)
 
 
 @runtime_checkable
 class _SupportsLt(Protocol[T_contra]):
```

### Comparing `phantom-types-1.2.2/src/phantom/boolean.py` & `phantom-types-2.0.0/src/phantom/boolean.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/bounds.py` & `phantom-types-2.0.0/src/phantom/bounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
+from typing import Final
 from typing import Iterable
 from typing import Sequence
 from typing import TypeVar
 from typing import cast
 
-from typing_extensions import Final
 from typing_extensions import TypeAlias
 from typing_extensions import get_args
 
 from ._utils.misc import is_union
 from .errors import BoundError
 from .predicates.boolean import all_of
 from .predicates.generic import of_complex_type
```

### Comparing `phantom-types-1.2.2/src/phantom/datetime.py` & `phantom-types-2.0.0/src/phantom/datetime.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/ext/phonenumbers.py` & `phantom-types-2.0.0/src/phantom/ext/phonenumbers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 .. code-block:: bash
 
     $ python3 -m pip install phantom-types[phonenumbers]
 """
 from __future__ import annotations
 
+from typing import Final
 from typing import cast
 
 import phonenumbers
-from typing_extensions import Final
 
 from phantom import Phantom
 from phantom.bounds import parse_str
 from phantom.fn import excepts
 from phantom.schema import Schema
 
 __all__ = (
```

### Comparing `phantom-types-1.2.2/src/phantom/fn.py` & `phantom-types-2.0.0/src/phantom/fn.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/interval.py` & `phantom-types-2.0.0/src/phantom/interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,18 @@
 minimums and maximums to their schema representations.
 """
 
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Any
+from typing import Final
+from typing import Protocol
 from typing import TypeVar
 
-from typing_extensions import Final
-from typing_extensions import Protocol
-
 from . import Phantom
 from . import Predicate
 from . import _hypothesis
 from ._utils.misc import resolve_class_attr
 from ._utils.types import Comparable
 from ._utils.types import SupportsEq
 from .predicates import interval
```

### Comparing `phantom-types-1.2.2/src/phantom/iso3166.py` & `phantom-types-2.0.0/src/phantom/iso3166.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 .. code-block:: python
 
     countries: tuple[CountryCode] = ("SE", "DK", ParsedAlpha2.parse("FR"))
 """
 from __future__ import annotations
 
+from typing import Final
+from typing import Literal
 from typing import Union
 from typing import cast
 
-from typing_extensions import Final
-from typing_extensions import Literal
 from typing_extensions import get_args
 
 from phantom import Phantom
 from phantom import _hypothesis
 from phantom.bounds import parse_str
 from phantom.predicates.collection import contained
 from phantom.schema import Schema
```

### Comparing `phantom-types-1.2.2/src/phantom/negated.py` & `phantom-types-2.0.0/src/phantom/negated.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/_utils.py` & `phantom-types-2.0.0/src/phantom/predicates/_utils.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/boolean.py` & `phantom-types-2.0.0/src/phantom/predicates/boolean.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Iterable
+from typing import Literal
 from typing import TypeVar
 
-from typing_extensions import Literal
-
 from . import Predicate
 from ._utils import bind_name
 
 T_contra = TypeVar("T_contra", bound=object, contravariant=True)
 
 
 def true(_value: object) -> Literal[True]:
```

### Comparing `phantom-types-1.2.2/src/phantom/predicates/collection.py` & `phantom-types-2.0.0/src/phantom/predicates/collection.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/generic.py` & `phantom-types-2.0.0/src/phantom/predicates/generic.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/interval.py` & `phantom-types-2.0.0/src/phantom/predicates/interval.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/numeric.py` & `phantom-types-2.0.0/src/phantom/predicates/numeric.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/predicates/re.py` & `phantom-types-2.0.0/src/phantom/predicates/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/re.py` & `phantom-types-2.0.0/src/phantom/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-1.2.2/src/phantom/schema.py` & `phantom-types-2.0.0/src/phantom/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import Literal
 from typing import Optional
 from typing import Sequence
 
-from typing_extensions import Literal
 from typing_extensions import TypedDict
 from typing_extensions import final
 
 
 class Schema(TypedDict, total=False):
     title: str
     description: str
```

### Comparing `phantom-types-1.2.2/src/phantom/sized.py` & `phantom-types-2.0.0/src/phantom/sized.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,44 +22,38 @@
 
     class SizedStr(str, PhantomBound[str], max=255):
         ...
 
 """
 from __future__ import annotations
 
+# This is the closest I could find to documentation of _ProtocolMeta.
+# https://github.com/python/cpython/commit/74d7f76e2c953fbfdb7ce01b7319d91d471cc5ef
 from typing import Any
 from typing import Generic
 from typing import Iterable
+from typing import Protocol
 from typing import Sized
 from typing import TypeVar
+from typing import _ProtocolMeta
+from typing import runtime_checkable
 
-from typing_extensions import Protocol
 from typing_extensions import get_args
-from typing_extensions import runtime_checkable
 
 from . import Phantom
 from . import PhantomMeta
 from . import Predicate
 from . import _hypothesis
 from ._utils.misc import is_not_known_mutable_instance
 from .predicates import boolean
 from .predicates import collection
 from .predicates import interval
 from .predicates import numeric
 from .schema import Schema
 
-# We attempt to import _ProtocolMeta from typing_extensions to support Python 3.7 but
-# fall back the typing module to support Python 3.8+. This is the closest I could find
-# to documentation of _ProtocolMeta.
-# https://github.com/python/cpython/commit/74d7f76e2c953fbfdb7ce01b7319d91d471cc5ef
-try:
-    from typing_extensions import _ProtocolMeta  # type: ignore[attr-defined]
-except ImportError:
-    from typing import _ProtocolMeta
-
 __all__ = (
     "SizedIterable",
     "PhantomSized",
     "PhantomBound",
     "NonEmpty",
     "NonEmptyStr",
     "Empty",
@@ -70,15 +64,15 @@
 
 
 @runtime_checkable
 class SizedIterable(Sized, Iterable[T], Protocol[T]):
     """Intersection of :py:class:`typing.Sized` and :py:class:`typing.Iterable`."""
 
 
-class SizedIterablePhantomMeta(PhantomMeta, _ProtocolMeta):  # type: ignore[misc]
+class SizedIterablePhantomMeta(PhantomMeta, _ProtocolMeta):
     ...
 
 
 class PhantomSized(
     Phantom[Sized],
     SizedIterable[T],
     Generic[T],
```

### Comparing `phantom-types-1.2.2/src/phantom_types.egg-info/PKG-INFO` & `phantom-types-2.0.0/src/phantom_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 1.2.2
+Version: 2.0.0
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: phonenumbers
 Provides-Extra: pydantic
 Provides-Extra: dateutil
 Provides-Extra: hypothesis
 Provides-Extra: all
 Provides-Extra: test
```

### Comparing `phantom-types-1.2.2/src/phantom_types.egg-info/SOURCES.txt` & `phantom-types-2.0.0/src/phantom_types.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 src/phantom/iso3166.py
 src/phantom/negated.py
 src/phantom/py.typed
 src/phantom/re.py
 src/phantom/schema.py
 src/phantom/sized.py
 src/phantom/_utils/__init__.py
-src/phantom/_utils/compat.py
 src/phantom/_utils/misc.py
 src/phantom/_utils/types.py
 src/phantom/ext/__init__.py
 src/phantom/ext/phonenumbers.py
 src/phantom/predicates/__init__.py
 src/phantom/predicates/_base.py
 src/phantom/predicates/_utils.py
```

