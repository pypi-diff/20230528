# Comparing `tmp/parsetypes-0.2.2.tar.gz` & `tmp/parsetypes-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.2.2.tar", last modified: Sun May 28 05:35:17 2023, max compression
+gzip compressed data, was "parsetypes-0.2.3.tar", last modified: Sun May 28 05:49:15 2023, max compression
```

## Comparing `parsetypes-0.2.2.tar` & `parsetypes-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.911326 parsetypes-0.2.2/
--rw-rw-rw-   0        0        0      795 2023-05-28 05:32:22.000000 parsetypes-0.2.2/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6616 2023-05-28 05:35:17.911326 parsetypes-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4116 2023-05-28 05:02:47.000000 parsetypes-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.895325 parsetypes-0.2.2/docs/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.903325 parsetypes-0.2.2/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/index.html
--rw-rw-rw-   0        0        0   502932 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   208714 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 05:35:17.911326 parsetypes-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.896325 parsetypes-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.906329 parsetypes-0.2.2/src/parsetypes/
--rw-rw-rw-   0        0        0      621 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-05-28 05:34:29.000000 parsetypes-0.2.2/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.2/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    34554 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.909326 parsetypes-0.2.2/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     6616 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.910328 parsetypes-0.2.2/tests/
--rw-rw-rw-   0        0        0    60176 2023-05-28 04:48:55.000000 parsetypes-0.2.2/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.2/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.966756 parsetypes-0.2.3/
+-rw-rw-rw-   0        0        0      798 2023-05-28 05:48:36.000000 parsetypes-0.2.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6617 2023-05-28 05:49:15.966756 parsetypes-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4114 2023-05-28 05:48:36.000000 parsetypes-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.950755 parsetypes-0.2.3/docs/
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.957754 parsetypes-0.2.3/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/index.html
+-rw-rw-rw-   0        0        0   502932 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   208714 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 05:49:15.966756 parsetypes-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.951756 parsetypes-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.961755 parsetypes-0.2.3/src/parsetypes/
+-rw-rw-rw-   0        0        0      621 2023-05-28 05:43:14.000000 parsetypes-0.2.3/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.3/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.3/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    34554 2023-05-28 05:32:22.000000 parsetypes-0.2.3/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.3/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.964755 parsetypes-0.2.3/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     6617 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.965758 parsetypes-0.2.3/tests/
+-rw-rw-rw-   0        0        0    60176 2023-05-28 04:48:55.000000 parsetypes-0.2.3/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.3/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.2.2/CHANGELOG.md` & `parsetypes-0.2.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
-The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
+The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1 and 0.2.2
+### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.2/PKG-INFO` & `parsetypes-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -71,18 +71,18 @@
 parser.parse("true")  # True
 parser.parse("")      # None
 ```
 
 Parsing a series so that it has a consistent type:
 ```python
 parser = TypeParser()
-parser.infer_series(["1", "2", "3"])        # [1, 2, 3]
-parser.infer_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-parser.infer_series(["true", "false", ""])  # [True, False, None]
-parser.infer_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
+parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
+parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
+parser.parse_series(["true", "false", ""])  # [True, False, None]
+parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ```
 
 Parsing a table so that each column is of a consistent type:
 ```python
 parser = TypeParser()
 table = parser.parse_table([
 	["1", "5",   "true",  "1"],
@@ -142,31 +142,31 @@
 
 The documentation is generated in `docs/html/`, using template files in `docs/template/`.
 
 #### Packaging
 
 Before packaging, check the package metadata by running `pyroma .` or `tox r -m metadata`.
 
-To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
+To generate sdist and wheel packages, delete `dist/` and `parsetypes.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
 
 ### Config files
 
 - `MANIFEST.in` Additional files to include in published sdist package
 - `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
 - `tox.ini` Config file for tox
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
-The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
+The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1 and 0.2.2
+### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.2/README.md` & `parsetypes-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 parser.parse("true")  # True
 parser.parse("")      # None
 ```
 
 Parsing a series so that it has a consistent type:
 ```python
 parser = TypeParser()
-parser.infer_series(["1", "2", "3"])        # [1, 2, 3]
-parser.infer_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-parser.infer_series(["true", "false", ""])  # [True, False, None]
-parser.infer_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
+parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
+parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
+parser.parse_series(["true", "false", ""])  # [True, False, None]
+parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ```
 
 Parsing a table so that each column is of a consistent type:
 ```python
 parser = TypeParser()
 table = parser.parse_table([
 	["1", "5",   "true",  "1"],
@@ -102,15 +102,15 @@
 
 The documentation is generated in `docs/html/`, using template files in `docs/template/`.
 
 #### Packaging
 
 Before packaging, check the package metadata by running `pyroma .` or `tox r -m metadata`.
 
-To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
+To generate sdist and wheel packages, delete `dist/` and `parsetypes.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
 
 ### Config files
 
 - `MANIFEST.in` Additional files to include in published sdist package
 - `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
```

### Comparing `parsetypes-0.2.2/docs/html/favicon.png` & `parsetypes-0.2.3/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/docs/html/parsetypes.html` & `parsetypes-0.2.3/docs/html/parsetypes.html`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.2&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.3&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">)</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.2.2"
+11__version__ = "0.2.3"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types')
```

### Comparing `parsetypes-0.2.2/docs/html/search.js` & `parsetypes-0.2.3/docs/html/search.js`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/pyproject.toml` & `parsetypes-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/src/parsetypes/__init__.py` & `parsetypes-0.2.3/src/parsetypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types')
```

### Comparing `parsetypes-0.2.2/src/parsetypes/_common.py` & `parsetypes-0.2.3/src/parsetypes/_common.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/src/parsetypes/_parser.py` & `parsetypes-0.2.3/src/parsetypes/_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/src/parsetypes/_reduce_types.py` & `parsetypes-0.2.3/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.2.3/src/parsetypes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -71,18 +71,18 @@
 parser.parse("true")  # True
 parser.parse("")      # None
 ```
 
 Parsing a series so that it has a consistent type:
 ```python
 parser = TypeParser()
-parser.infer_series(["1", "2", "3"])        # [1, 2, 3]
-parser.infer_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-parser.infer_series(["true", "false", ""])  # [True, False, None]
-parser.infer_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
+parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
+parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
+parser.parse_series(["true", "false", ""])  # [True, False, None]
+parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ```
 
 Parsing a table so that each column is of a consistent type:
 ```python
 parser = TypeParser()
 table = parser.parse_table([
 	["1", "5",   "true",  "1"],
@@ -142,31 +142,31 @@
 
 The documentation is generated in `docs/html/`, using template files in `docs/template/`.
 
 #### Packaging
 
 Before packaging, check the package metadata by running `pyroma .` or `tox r -m metadata`.
 
-To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
+To generate sdist and wheel packages, delete `dist/` and `parsetypes.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
 
 ### Config files
 
 - `MANIFEST.in` Additional files to include in published sdist package
 - `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
 - `tox.ini` Config file for tox
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
-The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
+The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1 and 0.2.2
+### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.2/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.2.3/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/tests/test_parser.py` & `parsetypes-0.2.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.2/tests/test_reduce_types.py` & `parsetypes-0.2.3/tests/test_reduce_types.py`

 * *Files identical despite different names*

