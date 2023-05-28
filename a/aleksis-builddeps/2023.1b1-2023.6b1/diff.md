# Comparing `tmp/aleksis_builddeps-2023.1b1.tar.gz` & `tmp/aleksis_builddeps-2023.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_builddeps-2023.1b1.tar", max compression
+gzip compressed data, was "aleksis_builddeps-2023.6b1.tar", max compression
```

## Comparing `aleksis_builddeps-2023.1b1.tar` & `aleksis_builddeps-2023.6b1.tar`

### file list

```diff
@@ -1,4 +1,3 @@
--rw-r--r--   0        0        0        0 2023-03-09 21:51:30.938247 aleksis_builddeps-2023.1b1/aleksis_builddeps.py
--rw-r--r--   0        0        0     1449 2023-03-09 21:51:30.938247 aleksis_builddeps-2023.1b1/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 aleksis_builddeps-2023.1b1/setup.py
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 aleksis_builddeps-2023.1b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 12:04:44.365658 aleksis_builddeps-2023.6b1/aleksis_builddeps.py
+-rw-r--r--   0        0        0     1449 2023-05-28 12:22:47.068994 aleksis_builddeps-2023.6b1/pyproject.toml
+-rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 aleksis_builddeps-2023.6b1/PKG-INFO
```

### Comparing `aleksis_builddeps-2023.1b1/pyproject.toml` & `aleksis_builddeps-2023.6b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Builddeps"
-version = "2023.1b1"
+version = "2023.6b1"
 packages = []
 
 description = "AlekSIS (School Information System) — Build/Dev dependencies for apps"
 authors = ["Dominik George <dominik.george@teckids.org>"]
 maintainers = ["Jonathan Weth <wethjo@katharineum.de>", "Dominik George <dominik.george@teckids.org>"]
 license = "EUPL-1.2-or-later"
 homepage = "https://aleksis.org/"
@@ -14,19 +14,19 @@
     "Development Status :: 3 - Alpha",
     "Framework :: Django :: 3.0",
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-sphinx = "^6.1"
+sphinx = "^7.0"
 sphinxcontrib-django = "^0.5.0"
 sphinxcontrib-svg2pdfconverter = "^1.1.1"
 sphinx-autodoc-typehints = "^1.7"
-django-stubs = "^1.1"
+django-stubs = "^4.2"
 pytest = "^7.2"
 pytest-django = "^4.1"
 pytest-django-testing-postgresql = "^0.2"
 selenium = "^4.0.0"
 safety = "^2.0.0"
 flake8 = "^6.0.0"
 flake8-django = "^1.0.0"
```

### Comparing `aleksis_builddeps-2023.1b1/PKG-INFO` & `aleksis_builddeps-2023.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-builddeps
-Version: 2023.1b1
+Version: 2023.6b1
 Summary: AlekSIS (School Information System) — Build/Dev dependencies for apps
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -16,15 +16,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=21.0)
 Requires-Dist: curlylint (>=0.13.0,<0.14.0)
-Requires-Dist: django-stubs (>=1.1,<2.0)
+Requires-Dist: django-stubs (>=4.2,<5.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: flake8-bandit (>=4.0.0,<5.0.0)
 Requires-Dist: flake8-black (>=0.3.0,<0.4.0)
 Requires-Dist: flake8-builtins (>=2.0.0,<3.0.0)
 Requires-Dist: flake8-django (>=1.0.0,<2.0.0)
 Requires-Dist: flake8-docstrings (>=1.5.0,<2.0.0)
 Requires-Dist: flake8-fixme (>=1.1.1,<2.0.0)
@@ -36,13 +36,13 @@
 Requires-Dist: pytest (>=7.2,<8.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-django (>=4.1,<5.0)
 Requires-Dist: pytest-django-testing-postgresql (>=0.2,<0.3)
 Requires-Dist: pytest-sugar (>=0.9.2,<0.10.0)
 Requires-Dist: safety (>=2.0.0,<3.0.0)
 Requires-Dist: selenium (>=4.0.0,<5.0.0)
-Requires-Dist: sphinx (>=6.1,<7.0)
+Requires-Dist: sphinx (>=7.0,<8.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.7,<2.0)
 Requires-Dist: sphinx_material (>=0.0.35,<0.0.36)
 Requires-Dist: sphinxcontrib-django (>=0.5.0,<0.6.0)
 Requires-Dist: sphinxcontrib-svg2pdfconverter (>=1.1.1,<2.0.0)
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS
```

