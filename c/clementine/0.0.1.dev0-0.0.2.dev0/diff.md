# Comparing `tmp/clementine-0.0.1.dev0.tar.gz` & `tmp/clementine-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementine-0.0.1.dev0.tar", last modified: Sun May 28 01:52:22 2023, max compression
+gzip compressed data, was "clementine-0.0.2.dev0.tar", last modified: Sun May 28 02:37:37 2023, max compression
```

## Comparing `clementine-0.0.1.dev0.tar` & `clementine-0.0.2.dev0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 01:52:22.915048 clementine-0.0.1.dev0/
--rw-r--r--   0 sue        (501) staff       (20)     1013 2023-05-28 01:52:22.914937 clementine-0.0.1.dev0/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      620 2023-05-28 01:52:01.000000 clementine-0.0.1.dev0/README.md
--rw-r--r--   0 sue        (501) staff       (20)      585 2023-05-28 01:52:12.000000 clementine-0.0.1.dev0/pyproject.toml
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-28 01:52:22.915078 clementine-0.0.1.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-28 01:46:57.000000 clementine-0.0.1.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 01:52:22.913611 clementine-0.0.1.dev0/src/
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 01:52:22.914175 clementine-0.0.1.dev0/src/clementine/
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-28 01:47:53.000000 clementine-0.0.1.dev0/src/clementine/__init__.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 01:52:22.914799 clementine-0.0.1.dev0/src/clementine.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)     1013 2023-05-28 01:52:22.000000 clementine-0.0.1.dev0/src/clementine.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      249 2023-05-28 01:52:22.000000 clementine-0.0.1.dev0/src/clementine.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-28 01:52:22.000000 clementine-0.0.1.dev0/src/clementine.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       49 2023-05-28 01:52:22.000000 clementine-0.0.1.dev0/src/clementine.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)       11 2023-05-28 01:52:22.000000 clementine-0.0.1.dev0/src/clementine.egg-info/top_level.txt
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.514394 clementine-0.0.2.dev0/
+-rw-r--r--   0 sue        (501) staff       (20)     1163 2023-05-28 02:37:37.514266 clementine-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      715 2023-05-28 02:24:32.000000 clementine-0.0.2.dev0/README.md
+-rw-r--r--   0 sue        (501) staff       (20)      696 2023-05-28 02:26:45.000000 clementine-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-28 02:37:37.514435 clementine-0.0.2.dev0/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-02-27 16:19:17.000000 clementine-0.0.2.dev0/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.512303 clementine-0.0.2.dev0/src/
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.513123 clementine-0.0.2.dev0/src/clementine/
+-rw-r--r--   0 sue        (501) staff       (20)       94 2023-05-28 02:10:59.000000 clementine-0.0.2.dev0/src/clementine/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)      137 2023-05-28 02:04:08.000000 clementine-0.0.2.dev0/src/clementine/cli.py
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-28 02:27:14.000000 clementine-0.0.2.dev0/src/clementine/version.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.513906 clementine-0.0.2.dev0/src/clementine.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)     1163 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      363 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       51 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)       88 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)       11 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/top_level.txt
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.514058 clementine-0.0.2.dev0/tests/
+-rw-r--r--   0 sue        (501) staff       (20)      101 2023-05-28 02:27:19.000000 clementine-0.0.2.dev0/tests/test_clementine.py
```

### Comparing `clementine-0.0.1.dev0/PKG-INFO` & `clementine-0.0.2.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 Metadata-Version: 2.1
 Name: clementine
-Version: 0.0.1.dev0
-Summary: A peachy little Python package
+Version: 0.0.2.dev0
+Summary: 🍊 A sweet little Python package
 Author-email: Suzen Fylke <codesue@users.noreply.github.com>
-Project-URL: repository, https://github.com/codesue/peach
+Project-URL: repository, https://github.com/codesue/clementine
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: ml
+Provides-Extra: packaging
 
-# peach: a peachy little Python package
+# clementine: a sweet little Python package
 
 [![GitHub][github_badge]][github_link]
-<!-- TODO (codesue): [![PyPI][pypi_badge]][pypi_link] -->
+[![PyPI][pypi_badge]][pypi_link]
 
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/codesue/clementine
 
 [pypi_badge]: https://badgen.net/pypi/v/clementine?icon=pypi&color=black&label
 [pypi_link]: https://pypi.org/project/clementine
 
 ## Installation
 
-<!-- TODO (codesue)
 Installing with pip:
 
 ```sh
 pip install clementine
 ```
--->
+
 
 Installing from source:
 
 ```sh
 git clone https://github.com/codesue/clementine.git
 cd clementine
 pip install -e .
 ```
+
+Building:
+
+```sh
+pip install -e ".[packaging]"
+python -m build
+twine check dist/*
+twine upload -r testpypi dist/*
+twine upload dist/*
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clementine-0.0.1.dev0/README.md` & `clementine-0.0.2.dev0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-# peach: a peachy little Python package
+# clementine: a sweet little Python package
 
 [![GitHub][github_badge]][github_link]
-<!-- TODO (codesue): [![PyPI][pypi_badge]][pypi_link] -->
+[![PyPI][pypi_badge]][pypi_link]
 
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/codesue/clementine
 
 [pypi_badge]: https://badgen.net/pypi/v/clementine?icon=pypi&color=black&label
 [pypi_link]: https://pypi.org/project/clementine
 
 ## Installation
 
-<!-- TODO (codesue)
 Installing with pip:
 
 ```sh
 pip install clementine
 ```
--->
+
 
 Installing from source:
 
 ```sh
 git clone https://github.com/codesue/clementine.git
 cd clementine
 pip install -e .
 ```
+
+Building:
+
+```sh
+pip install -e ".[packaging]"
+python -m build
+twine check dist/*
+twine upload -r testpypi dist/*
+twine upload dist/*
+```
```

### Comparing `clementine-0.0.1.dev0/src/clementine.egg-info/PKG-INFO` & `clementine-0.0.2.dev0/src/clementine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 Metadata-Version: 2.1
 Name: clementine
-Version: 0.0.1.dev0
-Summary: A peachy little Python package
+Version: 0.0.2.dev0
+Summary: 🍊 A sweet little Python package
 Author-email: Suzen Fylke <codesue@users.noreply.github.com>
-Project-URL: repository, https://github.com/codesue/peach
+Project-URL: repository, https://github.com/codesue/clementine
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: ml
+Provides-Extra: packaging
 
-# peach: a peachy little Python package
+# clementine: a sweet little Python package
 
 [![GitHub][github_badge]][github_link]
-<!-- TODO (codesue): [![PyPI][pypi_badge]][pypi_link] -->
+[![PyPI][pypi_badge]][pypi_link]
 
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/codesue/clementine
 
 [pypi_badge]: https://badgen.net/pypi/v/clementine?icon=pypi&color=black&label
 [pypi_link]: https://pypi.org/project/clementine
 
 ## Installation
 
-<!-- TODO (codesue)
 Installing with pip:
 
 ```sh
 pip install clementine
 ```
--->
+
 
 Installing from source:
 
 ```sh
 git clone https://github.com/codesue/clementine.git
 cd clementine
 pip install -e .
 ```
+
+Building:
+
+```sh
+pip install -e ".[packaging]"
+python -m build
+twine check dist/*
+twine upload -r testpypi dist/*
+twine upload dist/*
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

