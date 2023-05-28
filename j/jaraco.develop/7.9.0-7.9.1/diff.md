# Comparing `tmp/jaraco.develop-7.9.0.tar.gz` & `tmp/jaraco.develop-7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.develop-7.9.0.tar", last modified: Wed Oct 20 21:07:41 2021, max compression
+gzip compressed data, was "jaraco.develop-7.9.1.tar", last modified: Wed Mar 23 13:56:17 2022, max compression
```

## Comparing `jaraco.develop-7.9.0.tar` & `jaraco.develop-7.9.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.785898 jaraco.develop-7.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.781898 jaraco.develop-7.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.781898 jaraco.develop-7.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5728 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-10-20 21:07:41.785898 jaraco.develop-7.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      827 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.781898 jaraco.develop-7.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.777897 jaraco.develop-7.9.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.785898 jaraco.develop-7.9.0/jaraco/develop/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/add-github-secret.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/add-github-secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/create-github-release.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/github.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/init-azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/macos-build-python.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/print-meta.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/remove-namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/jaraco/develop/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 21:07:41.781898 jaraco.develop-7.9.0/jaraco.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-10-20 21:07:41.000000 jaraco.develop-7.9.0/jaraco.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      865 2021-10-20 21:07:41.000000 jaraco.develop-7.9.0/jaraco.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-20 21:07:41.000000 jaraco.develop-7.9.0/jaraco.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      344 2021-10-20 21:07:41.000000 jaraco.develop-7.9.0/jaraco.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-20 21:07:41.000000 jaraco.develop-7.9.0/jaraco.develop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-10-20 21:07:41.785898 jaraco.develop-7.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/todo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-10-20 21:07:13.000000 jaraco.develop-7.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/jaraco/develop/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/add-github-secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/add-github-secrets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/create-github-release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/github.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/indent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/init-azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/macos-build-python.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/print-meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/remove-namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/jaraco.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-03-23 13:56:16.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 13:56:16.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/tox.ini
```

### Comparing `jaraco.develop-7.9.0/.github/workflows/main.yml` & `jaraco.develop-7.9.1/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push, pull_request]
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - 3.6
+        - 3.7
         - 3.9
         - "3.10"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
     runs-on: ${{ matrix.platform }}
```

### Comparing `jaraco.develop-7.9.0/CHANGES.rst` & `jaraco.develop-7.9.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v7.9.1
+======
+
+* bpo-46975: Fix error in LDFLAGS building Python on macOS.
+
 v7.9.0
 ======
 
 * Add ``print-meta`` command.
 
 v7.8.0
 ======
```

### Comparing `jaraco.develop-7.9.0/LICENSE` & `jaraco.develop-7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/PKG-INFO` & `jaraco.develop-7.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 7.9.0
+Version: 7.9.1
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.develop.svg
    :target: `PyPI link`_
 
@@ -32,11 +32,11 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.develop-7.9.0/README.rst` & `jaraco.develop-7.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.develop-7.9.0/docs/conf.py` & `jaraco.develop-7.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/add-github-secrets.py` & `jaraco.develop-7.9.1/jaraco/develop/add-github-secrets.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/compiler.py` & `jaraco.develop-7.9.1/jaraco/develop/compiler.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/github.py` & `jaraco.develop-7.9.1/jaraco/develop/github.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/indent.py` & `jaraco.develop-7.9.1/jaraco/develop/indent.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/init-azure.py` & `jaraco.develop-7.9.1/jaraco/develop/init-azure.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco/develop/macos-build-python.py` & `jaraco.develop-7.9.1/jaraco/develop/macos-build-python.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     zlib and openssl installed.
     """
     require_libs()
 
     env = dict(
         os.environ,
         CPPFLAGS=f'-I{brew_prefix()}/include',
-        LDFLAGS=f'-I{brew_prefix()}/lib',
+        LDFLAGS=f'-L{brew_prefix()}/lib',
     )
     cmd = ['./configure', f'--with-openssl={brew_prefix("openssl@1.1")}']
     cmd += ['--with-pydebug'] * debug
     subprocess.run(cmd, env=env)
     subprocess.run('make')
```

### Comparing `jaraco.develop-7.9.0/jaraco/develop/remove-namespace.py` & `jaraco.develop-7.9.1/jaraco/develop/remove-namespace.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.0/jaraco.develop.egg-info/PKG-INFO` & `jaraco.develop-7.9.1/jaraco.develop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 7.9.0
+Version: 7.9.1
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.develop.svg
    :target: `PyPI link`_
 
@@ -32,11 +32,11 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.develop-7.9.0/jaraco.develop.egg-info/SOURCES.txt` & `jaraco.develop-7.9.1/jaraco.develop.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 LICENSE
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
 todo.txt
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `jaraco.develop-7.9.0/setup.cfg` & `jaraco.develop-7.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	jaraco.ui
 	jaraco.context
 	jaraco.collections
 	keyring
 	autocommand
 	requests-toolbelt
@@ -39,20 +39,20 @@
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; \
+	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.0.1
 docs = 
 	sphinx
-	jaraco.packaging >= 8.2
+	jaraco.packaging >= 9
 	rst.linker >= 1.9
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jaraco.develop-7.9.0/tox.ini` & `jaraco.develop-7.9.1/tox.ini`

 * *Files identical despite different names*

