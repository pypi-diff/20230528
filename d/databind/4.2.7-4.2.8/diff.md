# Comparing `tmp/databind-4.2.7.tar.gz` & `tmp/databind-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind-4.2.7.tar", max compression
+gzip compressed data, was "databind-4.2.8.tar", max compression
```

## Comparing `databind-4.2.7.tar` & `databind-4.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      612 2023-05-28 04:34:10.074427 databind-4.2.7/pyproject.toml
--rw-r--r--   0        0        0     1075 2023-05-28 03:01:35.972571 databind-4.2.7/readme.md
--rw-r--r--   0        0        0       22 2023-05-28 04:34:10.078427 databind-4.2.7/src/databind/_version/__init__.py
--rw-r--r--   0        0        0     1996 2023-05-28 04:34:22.211829 databind-4.2.7/setup.py
--rw-r--r--   0        0        0     1881 2023-05-28 04:34:22.211981 databind-4.2.7/PKG-INFO
+-rw-r--r--   0        0        0      612 2023-05-28 04:35:02.436938 databind-4.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1075 2023-05-28 03:01:35.972571 databind-4.2.8/readme.md
+-rw-r--r--   0        0        0       22 2023-05-28 04:35:02.444938 databind-4.2.8/src/databind/_version/__init__.py
+-rw-r--r--   0        0        0     1996 2023-05-28 04:35:09.833776 databind-4.2.8/setup.py
+-rw-r--r--   0        0        0     1881 2023-05-28 04:35:09.834108 databind-4.2.8/PKG-INFO
```

### Comparing `databind-4.2.7/pyproject.toml` & `databind-4.2.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "databind"
-version = "4.2.7"
+version = "4.2.8"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include="databind/_version", from="src" }]
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
-"databind.core" = "^4.2.7"
-"databind.json" = "^4.2.7"
+"databind.core" = "^4.2.8"
+"databind.json" = "^4.2.8"
 
 [build-system]
 requires = ["poetry-core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `databind-4.2.7/readme.md` & `databind-4.2.8/readme.md`

 * *Files identical despite different names*

### Comparing `databind-4.2.7/setup.py` & `databind-4.2.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['_version']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['databind.core>=4.2.7,<5.0.0', 'databind.json>=4.2.7,<5.0.0']
+['databind.core>=4.2.8,<5.0.0', 'databind.json>=4.2.8,<5.0.0']
 
 setup_kwargs = {
     'name': 'databind',
-    'version': '4.2.7',
+    'version': '4.2.8',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer.',
     'long_description': '# databind\n\n__Compatibility__: Python 3.6.3+\n\nDatabind is a library inspired by jackson-databind to de-/serialise Python dataclasses.\n\nIf you install the `databind` package, you will get the respective version of the\nfollowing packages:\n\n* [databind.core](https://pypi.org/project/databind.core/) &ndash; Provides the core framework.\n* [databind.json](https://pypi.org/project/databind.json/) &ndash; De-/serialize dataclasses to/from JSON payloads.\n\n## Supported features\n\n| Feature | Python version | Databind version |\n| ------- | -------------- | ---------------- |\n| [PEP585](https://www.python.org/dev/peps/pep-0585/) | 3.9 | 1.2.0 &ndash; *current* |\n| [PEP585](https://www.python.org/dev/peps/pep-0585/) (forward references) | 3.9 | 1.3.1? &ndash; *current* |\n| Resolve type parameters of specialised generic types | 3.x | 1.5.0 &ndash; *current* |\n| `typing.TypedDict` | 3.x | 2.0.0 &ndash; *current* |\n| Concretise type variables in parametrised generics | 3.x | 2.0.0 &ndash; *current* |\n\n---\n\n<p align="center">Copyright &copy; 2022 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind-4.2.7/PKG-INFO` & `databind-4.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: databind
-Version: 4.2.7
+Version: 4.2.8
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.2.7,<5.0.0)
-Requires-Dist: databind.json (>=4.2.7,<5.0.0)
+Requires-Dist: databind.core (>=4.2.8,<5.0.0)
+Requires-Dist: databind.json (>=4.2.8,<5.0.0)
 Description-Content-Type: text/markdown
 
 # databind
 
 __Compatibility__: Python 3.6.3+
 
 Databind is a library inspired by jackson-databind to de-/serialise Python dataclasses.
```

