# Comparing `tmp/python_ms-1.0.2.tar.gz` & `tmp/python_ms-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ms-1.0.2.tar", max compression
+gzip compressed data, was "python_ms-1.1.0.tar", max compression
```

## Comparing `python_ms-1.0.2.tar` & `python_ms-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     3380 2023-02-09 03:25:28.770310 python_ms-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-02-09 03:25:28.770310 python_ms-1.0.2/LICENSE
--rw-r--r--   0        0        0     4908 2023-02-09 03:25:28.770310 python_ms-1.0.2/README.md
--rw-r--r--   0        0        0     2936 2023-02-09 03:25:28.770310 python_ms-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      176 2023-02-09 03:25:28.770310 python_ms-1.0.2/python_ms/__init__.py
--rw-r--r--   0        0        0     1210 2023-02-09 03:25:28.770310 python_ms-1.0.2/python_ms/config.py
--rw-r--r--   0        0        0     6208 2023-02-09 03:25:28.770310 python_ms-1.0.2/python_ms/ms.py
--rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 python_ms-1.0.2/setup.py
--rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 python_ms-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4013 2023-05-28 21:22:43.854573 python_ms-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-05-28 21:22:43.854573 python_ms-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4907 2023-05-28 21:22:43.854573 python_ms-1.1.0/README.md
+-rw-r--r--   0        0        0     4066 2023-05-28 21:22:43.858573 python_ms-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-05-28 21:22:43.858573 python_ms-1.1.0/python_ms/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-28 21:22:43.858573 python_ms-1.1.0/python_ms/config.py
+-rw-r--r--   0        0        0     6344 2023-05-28 21:22:43.858573 python_ms-1.1.0/python_ms/ms.py
+-rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 python_ms-1.1.0/PKG-INFO
```

### Comparing `python_ms-1.0.2/LICENSE` & `python_ms-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ms-1.0.2/README.md` & `python_ms-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,11 +79,11 @@
 ## Related Packages
 
 - [ms](https://github.com/vercel/ms) - The original JavaScript `ms` package
 
 ## Caught a Bug?
 
 1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device
-2. Install `poetry` (if it isn't alreeady installed)
+2. Install `poetry` (if it isn't already installed)
 3. Run `poetry install` in the project directory. This fetches development dependencies like `pytest` and sets up everything for you to start debugging
 
 As always, you can run the tests using: `poetry run pytest`
```

### Comparing `python_ms-1.0.2/pyproject.toml` & `python_ms-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 [build-system]
-requires = ['poetry-core>=1.0.0', 'wheel',]
+requires = ['poetry-core>=1.2.0', 'wheel',]
 build-backend = 'poetry.core.masonry.api'
 
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 omit = [
     '.tox/*',
     'tests/*',
 ]
 
 
-[tool.flake8]
-max-line-length = 120
-extend-ignore = ''  # https://www.flake8rules.com/
-max-complexity = 15  # Info: https://en.wikipedia.org/wiki/Cyclomatic_complexity
-per-file-ignores = """\
-# F401: Ignore "unused" imports
-# F403: Ignore star imports
-# F405: Ignore names from star imports
-__init__.py:F401,F403,F405\
-"""
-
-
 [tool.poetry]
 name = 'python_ms'
-version = '1.0.2'
+version = '1.1.0'
 description = "A Python equivalent to the JavaScript ms package."
 
 authors = ["Lari Liuhamo <lari.liuhamo+pypi@gmail.com>",]
 maintainers = ["Lari Liuhamo <lari.liuhamo+pypi@gmail.com>",]
 
 include = ['CHANGELOG.md', 'LICENSE',]
 license = 'MIT'
@@ -61,37 +49,111 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = '^3.10'
 
 
-[tool.poetry.dev-dependencies]
-coverage = {version = '^7.1.0', extras = ['toml',]}
-flake8 = '^6.0.0'
-mypy = '^1.0'
-pylint = '^2.16.1'
-pyproject-flake8 = '^6.0.0'
-pytest = '^7.2.1'
-pytest-cov = '^4.0.0'
-tox = '^3.28.0'
-tox-gh-actions = '^2.12.0'
+[tool.poetry.group.dev.dependencies]
+mypy = '^1.3.0'
+
+
+[tool.poetry.group.linters]
+optional = true
+
+
+[tool.poetry.group.linters.dependencies]
+ruff = '^0.0.269'
+
+
+[tool.poetry.group.tests]
+optional = true
+
+
+[tool.poetry.group.tests.dependencies]
+pytest = '^7.3.1'
+pytest-cov = '^4.1.0'
+tox = '^4.5.2'
+tox-gh-actions = '^3.1.1'
 
 
 [tool.poetry.urls]
 "Tracker" = 'https://github.com/Diapolo10/python-ms/issues'
 "Changelog" = 'https://github.com/Diapolo10/python-ms/blob/main/CHANGELOG.md'
 
 
-[tool.pylint.'MESSAGES CONTROL']
-max-line-length = 120
-disable = [
-    # https://vald-phoenix.github.io/pylint-errors/
-    'E1102',  # ms is not callable (not-callable)
+[tool.ruff]
+select = [
+    'A',   # Builtins
+    'ANN', # Annotations
+    'ARG', # Unused arguments
+    'B',   # Bugbear
+    'BLE', # Blind except
+    'C4',  # Comprehensions
+    'C90', # mccabe
+    'COM', # Commas
+    'DTZ', # Datetimes
+    'ERA', # Commented-out code
+    'EXE', # Executable
+    'G',   # Logging format
+    'I',   # Isort
+    'ICN', # Import conventions
+    'INP', # Disallow PEP-420 (Implicit namespace packages)
+    'INT', # gettext
+    'ISC', # Implicit str concat
+    'N',   # PEP-8 Naming
+    'NPY', # Numpy
+    'PGH', # Pygrep hooks
+    'PIE', # Unnecessary code
+    'PL',  # Pylint
+    'PT',  # Pytest
+    'PTH', # Use Pathlib
+    'PYI', # Stub files
+    'RET', # Return
+    'RUF', # Ruff
+    'RSE', # Raise
+    'S',   # Bandit
+    'SIM', # Code simplification
+    'SLF', # Private member access
+    'T20', # Print
+    'TCH', # Type checking
+    'TID', # Tidy imports
+    'UP',  # Pyupgrade
+    'W',   # Warnings
+    'YTT', # sys.version
 ]
+ignore = [
+    'ANN401',   # Disallow typing.Any
+    'PLR0913',  # Too many arguments
+]
+ignore-init-module-imports = true
+line-length = 120
+
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
+
+
+[tool.ruff.per-file-ignores]
+# https://beta.ruff.rs/docs/rules/
+'__init__.py' = ['F401','F403','F405',]
+'tests/*' = ['ANN201', 'ARG', 'PT011', 'S101', 'PLR2004',]
+'*/config.py' = ['S311',]
+
+
+[tool.ruff.pylint]
+max-args = 15
+max-branches = 20
+max-returns = 10
+max-statements = 80
+
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = """
 --doctest-modules \
 --cov=./ \
```

### Comparing `python_ms-1.0.2/python_ms/config.py` & `python_ms-1.1.0/python_ms/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Contains global constants used by the package"""
 
 import random
 import re
 
-
 # Basic units of time
 
 MILLISECOND = 1
 SECOND = 10**3 * MILLISECOND
 MINUTE = 60 * SECOND
 HOUR = 60 * MINUTE
 DAY = 24 * HOUR
@@ -32,15 +31,14 @@
 MILLENIUM = 10 * CENTURY
 
 
 # Esoteric units of time
 
 # https://en.wikipedia.org/wiki/List_of_humorous_units_of_measurement#Time
 JIFFY = random.randint(1, 10) * MILLISECOND
-# SHAKE = 10 * NANOSECOND
 MILLIDAY = DAY // 1000
 MICROCENTURY = 52 * MINUTE + 35 * SECOND + 700 * MILLISECOND
 NANOCENTURY = MICROCENTURY // 1000
 FRIEDMAN = 6 * MONTH
 SCARAMUCCI = 11 * DAY
 LUSTRUM = 5 * YEAR
 OLYMPIAD = 4 * YEAR
@@ -49,8 +47,8 @@
 JUBILEE = 50 * YEAR
 MEGAANNUM = 10**3 * MILLENIUM
 AEON = 10**3 * MEGAANNUM
 
 
 # Regular expressions
 
-TIME_REGEX = re.compile(r'^([+-]?\d*\.?\d*)\s?([a-zA-Z-]*)$')
+TIME_REGEX = re.compile(r'^([+-]?\d+(?:\.\d*)?|\.\d+)\s?([a-zA-Z-]*)$')
```

### Comparing `python_ms-1.0.2/python_ms/ms.py` & `python_ms-1.1.0/python_ms/ms.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,130 @@
 """Python equivalent of the JavaScript ms package"""
 
+from __future__ import annotations
+
 import types
 from typing import overload
 
 import python_ms.config as cfg
 
 
 def common_unit_conversion(unit: str) -> int:
     """
     Returns a suitable multiplier from milliseconds to the desired unit
 
     Raises ValueError if no suitable conversion is found.
     """
 
-    # pylint: disable=R0911
+    result = None
+
     match (unit):
         case 'a' | 'y' | 'yr' | 'yrs' | 'year' | 'years':
-            return cfg.YEAR
+            result = cfg.YEAR
         case 'mon' | 'mth' | 'mths' | 'month' | 'months':
-            return cfg.MONTH
+            result = cfg.MONTH
         case 'w' | 'wk' | 'wks' | 'week' | 'weeks':
-            return cfg.WEEK
+            result = cfg.WEEK
         case 'd' | 'day' | 'days':
-            return cfg.DAY
+            result = cfg.DAY
         case 'h' | 'hr' | 'hrs' | 'hour' | 'hours':
-            return cfg.HOUR
+            result = cfg.HOUR
         case 'm' | 'min' | 'mins' | 'minute' | 'minutes':
-            return cfg.MINUTE
+            result = cfg.MINUTE
         case 's' | 'sec' | 'secs' | 'second' | 'seconds':
-            return cfg.SECOND
+            result = cfg.SECOND
         case '' | 'ms' | 'msec' | 'msecs' | 'millisecond' | 'milliseconds':
-            return cfg.MILLISECOND
+            result = cfg.MILLISECOND
         case _:
-            return uncommon_unit_conversion(unit)
+            result = uncommon_unit_conversion(unit)
+
+    return result
 
 
 def uncommon_unit_conversion(unit: str) -> int:
     """
     Returns a suitable multiplier from milliseconds to the desired unit
 
     Raises ValueError if no suitable conversion is found.
     """
 
-    # pylint: disable=R0911
+    result = None
+
     match (unit):
         case 'mil' | 'mils' | 'millenium' | 'milleniums':
-            return cfg.MILLENIUM
+            result = cfg.MILLENIUM
         case 'cnt' | 'cnts' | 'ctr' | 'ctrs' | 'century' | 'centuries':
-            return cfg.CENTURY
+            result = cfg.CENTURY
         case 'dc' | 'dcs' | 'decade' | 'decades':
-            return cfg.DECADE
+            result = cfg.DECADE
         case 'f' | 'fn' | 'fns' | 'fortnight' | 'fortnights':
-            return cfg.FORTNIGHT
+            result = cfg.FORTNIGHT
         case 'Ys' | 'Ysec' | 'Ysecs' | 'yottasecond' | 'yottaseconds':
-            return cfg.YOTTASECOND
+            result = cfg.YOTTASECOND
         case 'Zs' | 'Zsec' | 'Zsecs' | 'zettasecond' | 'zettaseconds':
-            return cfg.ZETTASECOND
+            result = cfg.ZETTASECOND
         case 'Es' | 'Esec' | 'Esecs' | 'exasecond' | 'exaseconds':
-            return cfg.EXASECOND
+            result = cfg.EXASECOND
         case 'Ps' | 'Psec' | 'Psecs' | 'petasecond' | 'petaseconds':
-            return cfg.PETASECOND
+            result = cfg.PETASECOND
         case 'Ts' | 'Tsec' | 'Tsecs' | 'terasecond' | 'teraseconds':
-            return cfg.TERASECOND
+            result = cfg.TERASECOND
         case 'Gs' | 'Gsec' | 'Gsecs' | 'gigasecond' | 'gigaseconds':
-            return cfg.GIGASECOND
+            result = cfg.GIGASECOND
         case 'Ms' | 'Msec' | 'Msecs' | 'megasecond' | 'megaseconds':
-            return cfg.MEGASECOND
+            result = cfg.MEGASECOND
         case 'ks' | 'ksec' | 'ksecs' | 'kilosecond' | 'kiloseconds':
-            return cfg.KILOSECOND
+            result = cfg.KILOSECOND
         case _:
-            return esoteric_unit_conversion(unit)
+            result = esoteric_unit_conversion(unit)
+
+    return result
 
 
 def esoteric_unit_conversion(unit: str) -> int:
     """
     Returns a suitable multiplier from milliseconds to the desired unit
 
     Raises ValueError if no suitable conversion is found.
     """
 
-    # pylint: disable=R0911
+    result = None
+
     match (unit):
         case 'aeon' | 'aeons':
-            return cfg.AEON
+            result = cfg.AEON
         case 'Mann' | 'Manns' | 'megaannum' | 'megaannums' | 'mega-annum' | 'mega-annums':
-            return cfg.MEGAANNUM
+            result = cfg.MEGAANNUM
         case 'jubilee' | 'jubilees':
-            return cfg.JUBILEE
+            result = cfg.JUBILEE
         case 'score' | 'scores':
-            return cfg.SCORE
+            result = cfg.SCORE
         case 'ind' | 'inds' | 'indiction' | 'indictions':
-            return cfg.INDICTION
+            result = cfg.INDICTION
         case 'olympiad' | 'olympiads':
-            return cfg.OLYMPIAD
+            result = cfg.OLYMPIAD
         case 'lustrum' | 'lustrums':
-            return cfg.LUSTRUM
+            result = cfg.LUSTRUM
         case 'scara' | 'scaras' | 'scaramucci' | 'scaramuccis':
-            return cfg.SCARAMUCCI
+            result = cfg.SCARAMUCCI
         case 'Fm' | 'Fms' | 'fm' | 'fms' | 'friedman' | 'friedmans':
-            return cfg.FRIEDMAN
+            result = cfg.FRIEDMAN
         case 'nc' | 'ncs' | 'ncent' | 'ncents' | 'nanocentury' | 'nanocenturies':
-            return cfg.NANOCENTURY
+            result = cfg.NANOCENTURY
         case 'mc' | 'mcs' | 'mcent' | 'mcents' | 'microcentury' | 'microcenturies':
-            return cfg.MICROCENTURY
+            result = cfg.MICROCENTURY
         case 'md' | 'mds' | 'mday' | 'mdays' | 'milliday' | 'millidays':
-            return cfg.MILLIDAY
+            result = cfg.MILLIDAY
         case 'jiffy' | 'jiffies':
-            return cfg.JIFFY
+            result = cfg.JIFFY
         case _:
             raise ValueError("Unsupported unit")
 
+    return result
+
 
 def parse_time(time: str) -> int:
     """
     Parses time in string format to milliseconds
 
     NOTE: The function is case-sensitive in order to accommodate some types.
 
@@ -141,15 +152,15 @@
 
 def ms_to_string(time: int, long: bool = False) -> str:
     """Converts miliseconds to a time string"""
 
     forms = ('ms', ' millisecond', ' milliseconds')
     time_unit = cfg.MILLISECOND
 
-    if cfg.DAY <= abs(time):
+    if abs(time) >= cfg.DAY:
         forms = ('d', ' day', ' days')
         time_unit = cfg.DAY
     elif cfg.HOUR <= abs(time) < cfg.DAY:
         forms = ('h', ' hour', ' hours')
         time_unit = cfg.HOUR
     elif cfg.MINUTE <= abs(time) < cfg.HOUR:
         forms = ('m', ' minute', ' minutes')
@@ -163,27 +174,25 @@
     if long:
         form_idx += 1
         form_idx += final_time not in {1, -1}
     form = forms[form_idx]
     return f"{final_time}{form}"
 
 
-class _ms(types.ModuleType):
+class _ms(types.ModuleType):  # noqa: N801
     """Implements the module interface"""
 
-    # pylint: disable=R0903
-
     @overload
-    def __call__(self, value: str, long: bool) -> int:
+    def __call__(self: _ms, value: str, long: bool) -> int:
         pass
 
     @overload
-    def __call__(self, value: int, long: bool) -> str:
+    def __call__(self: _ms, value: int, long: bool) -> str:
         pass
 
-    def __call__(self, value: str | int, long: bool = False) -> int | str:
+    def __call__(self: _ms, value: str | int, long: bool = False) -> int | str:
         if isinstance(value, str):
             return parse_time(value)
         if isinstance(value, int):
             return ms_to_string(value, long)
 
         raise NotImplementedError("This type is not supported")
```

### Comparing `python_ms-1.0.2/setup.py` & `python_ms-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-ms
+Version: 1.1.0
+Summary: A Python equivalent to the JavaScript ms package.
+Home-page: https://pypi.org/project/python-ms/
+License: MIT
+Keywords: package,python3,time
+Author: Lari Liuhamo
+Author-email: lari.liuhamo+pypi@gmail.com
+Maintainer: Lari Liuhamo
+Maintainer-email: lari.liuhamo+pypi@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Project-URL: Changelog, https://github.com/Diapolo10/python-ms/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://github.com/Diapolo10/python-ms/tree/main/docs
+Project-URL: Repository, https://github.com/Diapolo10/python-ms
+Project-URL: Tracker, https://github.com/Diapolo10/python-ms/issues
+Description-Content-Type: text/markdown
 
-packages = \
-['python_ms']
+# Python-ms
 
-package_data = \
-{'': ['*']}
+A Python equivalent to the JavaScript `ms` package.
 
-setup_kwargs = {
-    'name': 'python-ms',
-    'version': '1.0.2',
-    'description': 'A Python equivalent to the JavaScript ms package.',
-    'long_description': '# Python-ms\n\nA Python equivalent to the JavaScript `ms` package.\n\nThis port of the original project supports some additional string-to-ms\nconversions, but otherwise the functionality is identical. This version\nalso uses integers for everything to avoid rounding errors with\nfloating-point numbers when using large values.\n\nUsing the project\'s unit tests as examples is recommended, as they cover\neverything.\n\n| Type         | Badges |\n|--------------|---|\n| PyPI         | ![Python versions](https://img.shields.io/pypi/pyversions/python-ms?logo=python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/python-ms) ![Wheel](https://img.shields.io/pypi/wheel/python-ms?logo=pypi) ![Downloads](https://img.shields.io/pypi/dm/python-ms?logo=pypi) [![Version](https://img.shields.io/pypi/v/python-ms)](https://pypi.org/project/python-ms/) |\n| Tests        | [![codecov](https://codecov.io/gh/Diapolo10/python-ms/branch/main/graph/badge.svg?token=zBlgCd32Aq)](https://codecov.io/gh/Diapolo10/python-ms) ![Unit tests](https://github.com/diapolo10/python-ms/workflows/Unit%20tests/badge.svg) ![Pylint](https://github.com/diapolo10/python-ms/workflows/Pylint/badge.svg) ![Flake8](https://github.com/diapolo10/python-ms/workflows/Flake8/badge.svg) ![Deploy to PyPI](https://github.com/diapolo10/python-ms/workflows/Deploy%20to%20PyPI/badge.svg) |\n| Activity     | ![GitHub contributors](https://img.shields.io/github/contributors/diapolo10/python-ms) ![Last commit](https://img.shields.io/github/last-commit/diapolo10/python-ms?logo=github) ![GitHub all releases](https://img.shields.io/github/downloads/diapolo10/python-ms/total?logo=github) ![GitHub issues](https://img.shields.io/github/issues/diapolo10/python-ms) ![GitHub closed issues](https://img.shields.io/github/issues-closed/diapolo10/python-ms) ![GitHub pull requests](https://img.shields.io/github/issues-pr/diapolo10/python-ms) ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/diapolo10/python-ms) |\n| QA           | [![CodeFactor](https://www.codefactor.io/repository/github/diapolo10/python-ms/badge?logo=codefactor)](https://www.codefactor.io/repository/github/diapolo10/python-ms) [![Rating](https://img.shields.io/librariesio/sourcerank/pypi/python-ms)](https://libraries.io/github/Diapolo10/python-ms/sourcerank) |\n| Other        | [![License](https://img.shields.io/github/license/diapolo10/python-ms)](https://opensource.org/licenses/MIT) [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDiapolo10%2Fpython-ms.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDiapolo10%2Fpython-ms?ref=badge_shield) [![Known Vulnerabilities](https://snyk.io/test/github/diapolo10/python-ms/badge.svg)](https://snyk.io/test/github/diapolo10/python-ms) ![Repository size](https://img.shields.io/github/repo-size/diapolo10/python-ms?logo=github) ![Code size](https://img.shields.io/github/languages/code-size/diapolo10/python-ms?logo=github) ![Lines of code](https://img.shields.io/tokei/lines/github/diapolo10/python-ms?logo=github) |\n\n## Installation\n\nThe project is available via PyPI:\n\n```sh\npip install python_ms\n```\n\n## Examples\n\n### Convert from strings\n\n```python\nimport python_ms as ms\n\nms(\'2 days\')  # 172_800_000\nms(\'1d\')      # 86_400_000\nms(\'10h\')     # 36_000_000\nms(\'2.5 hrs\') # 9_000_000\nms(\'2h\')      # 7_200_000\nms(\'1m\')      # 60_000\nms(\'5s\')      # 5_000\nms(\'1y\')      # 31_557_600_000\nms(\'100\')     # 100\nms(\'-3 days\') # -259_200_000\nms(\'-1h\')     # -3_600_000\nms(\'-200\')    # -200\n```\n\n### Convert from milliseconds\n\n```python\nimport python_ms as ms\n\nms(60_000)          # "1m"\nms(2 * 60_000)      # "2m"\nms(-3 * 60_000)     # "-3m"\nms(ms(\'10 hours\'))  # "10h"\n```\n\n### Time format written out\n\n```python\nimport python_ms as ms\n\nms(60_000, long=True)          # "1 minute"\nms(2 * 60_000, long=True)      # "2 minutes"\nms(-3 * 60_000, long=True)     # "-3 minutes"\nms(ms(\'10 hours\'), long=True)  # "10 hours"\n```\n\n## Features\n\n- Has no dependencies aside from the standard library\n- If a number is supplied to `python_ms`, a string with a unit is returned\n- If a string that contains the number is supplied, it returns it as a number (e.g.: it returns `100` for `\'100\'`)\n- If you pass a string with a number and a valid unit, the number of equivalent milliseconds is returned\n\n## Related Packages\n\n- [ms](https://github.com/vercel/ms) - The original JavaScript `ms` package\n\n## Caught a Bug?\n\n1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device\n2. Install `poetry` (if it isn\'t alreeady installed)\n3. Run `poetry install` in the project directory. This fetches development dependencies like `pytest` and sets up everything for you to start debugging\n\nAs always, you can run the tests using: `poetry run pytest`\n',
-    'author': 'Lari Liuhamo',
-    'author_email': 'lari.liuhamo+pypi@gmail.com',
-    'maintainer': 'Lari Liuhamo',
-    'maintainer_email': 'lari.liuhamo+pypi@gmail.com',
-    'url': 'https://pypi.org/project/python-ms/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+This port of the original project supports some additional string-to-ms
+conversions, but otherwise the functionality is identical. This version
+also uses integers for everything to avoid rounding errors with
+floating-point numbers when using large values.
 
+Using the project's unit tests as examples is recommended, as they cover
+everything.
+
+| Type         | Badges |
+|--------------|---|
+| PyPI         | ![Python versions](https://img.shields.io/pypi/pyversions/python-ms?logo=python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/python-ms) ![Wheel](https://img.shields.io/pypi/wheel/python-ms?logo=pypi) ![Downloads](https://img.shields.io/pypi/dm/python-ms?logo=pypi) [![Version](https://img.shields.io/pypi/v/python-ms)](https://pypi.org/project/python-ms/) |
+| Tests        | [![codecov](https://codecov.io/gh/Diapolo10/python-ms/branch/main/graph/badge.svg?token=zBlgCd32Aq)](https://codecov.io/gh/Diapolo10/python-ms) ![Unit tests](https://github.com/diapolo10/python-ms/workflows/Unit%20tests/badge.svg) ![Pylint](https://github.com/diapolo10/python-ms/workflows/Pylint/badge.svg) ![Flake8](https://github.com/diapolo10/python-ms/workflows/Flake8/badge.svg) ![Deploy to PyPI](https://github.com/diapolo10/python-ms/workflows/Deploy%20to%20PyPI/badge.svg) |
+| Activity     | ![GitHub contributors](https://img.shields.io/github/contributors/diapolo10/python-ms) ![Last commit](https://img.shields.io/github/last-commit/diapolo10/python-ms?logo=github) ![GitHub all releases](https://img.shields.io/github/downloads/diapolo10/python-ms/total?logo=github) ![GitHub issues](https://img.shields.io/github/issues/diapolo10/python-ms) ![GitHub closed issues](https://img.shields.io/github/issues-closed/diapolo10/python-ms) ![GitHub pull requests](https://img.shields.io/github/issues-pr/diapolo10/python-ms) ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/diapolo10/python-ms) |
+| QA           | [![CodeFactor](https://www.codefactor.io/repository/github/diapolo10/python-ms/badge?logo=codefactor)](https://www.codefactor.io/repository/github/diapolo10/python-ms) [![Rating](https://img.shields.io/librariesio/sourcerank/pypi/python-ms)](https://libraries.io/github/Diapolo10/python-ms/sourcerank) |
+| Other        | [![License](https://img.shields.io/github/license/diapolo10/python-ms)](https://opensource.org/licenses/MIT) [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDiapolo10%2Fpython-ms.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDiapolo10%2Fpython-ms?ref=badge_shield) [![Known Vulnerabilities](https://snyk.io/test/github/diapolo10/python-ms/badge.svg)](https://snyk.io/test/github/diapolo10/python-ms) ![Repository size](https://img.shields.io/github/repo-size/diapolo10/python-ms?logo=github) ![Code size](https://img.shields.io/github/languages/code-size/diapolo10/python-ms?logo=github) ![Lines of code](https://img.shields.io/tokei/lines/github/diapolo10/python-ms?logo=github) |
+
+## Installation
+
+The project is available via PyPI:
+
+```sh
+pip install python_ms
+```
+
+## Examples
+
+### Convert from strings
+
+```python
+import python_ms as ms
+
+ms('2 days')  # 172_800_000
+ms('1d')      # 86_400_000
+ms('10h')     # 36_000_000
+ms('2.5 hrs') # 9_000_000
+ms('2h')      # 7_200_000
+ms('1m')      # 60_000
+ms('5s')      # 5_000
+ms('1y')      # 31_557_600_000
+ms('100')     # 100
+ms('-3 days') # -259_200_000
+ms('-1h')     # -3_600_000
+ms('-200')    # -200
+```
+
+### Convert from milliseconds
+
+```python
+import python_ms as ms
+
+ms(60_000)          # "1m"
+ms(2 * 60_000)      # "2m"
+ms(-3 * 60_000)     # "-3m"
+ms(ms('10 hours'))  # "10h"
+```
+
+### Time format written out
+
+```python
+import python_ms as ms
+
+ms(60_000, long=True)          # "1 minute"
+ms(2 * 60_000, long=True)      # "2 minutes"
+ms(-3 * 60_000, long=True)     # "-3 minutes"
+ms(ms('10 hours'), long=True)  # "10 hours"
+```
+
+## Features
+
+- Has no dependencies aside from the standard library
+- If a number is supplied to `python_ms`, a string with a unit is returned
+- If a string that contains the number is supplied, it returns it as a number (e.g.: it returns `100` for `'100'`)
+- If you pass a string with a number and a valid unit, the number of equivalent milliseconds is returned
+
+## Related Packages
+
+- [ms](https://github.com/vercel/ms) - The original JavaScript `ms` package
+
+## Caught a Bug?
+
+1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device
+2. Install `poetry` (if it isn't already installed)
+3. Run `poetry install` in the project directory. This fetches development dependencies like `pytest` and sets up everything for you to start debugging
+
+As always, you can run the tests using: `poetry run pytest`
 
-setup(**setup_kwargs)
```

