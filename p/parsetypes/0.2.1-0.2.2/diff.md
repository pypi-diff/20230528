# Comparing `tmp/parsetypes-0.2.1.tar.gz` & `tmp/parsetypes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.2.1.tar", last modified: Sun May 28 05:03:22 2023, max compression
+gzip compressed data, was "parsetypes-0.2.2.tar", last modified: Sun May 28 05:35:17 2023, max compression
```

## Comparing `parsetypes-0.2.1.tar` & `parsetypes-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.912196 parsetypes-0.2.1/
--rw-rw-rw-   0        0        0      785 2023-05-28 05:02:47.000000 parsetypes-0.2.1/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6606 2023-05-28 05:03:22.912196 parsetypes-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4116 2023-05-28 05:02:47.000000 parsetypes-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.896637 parsetypes-0.2.1/docs/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.904195 parsetypes-0.2.1/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-28 05:03:13.000000 parsetypes-0.2.1/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-28 05:03:13.000000 parsetypes-0.2.1/docs/html/index.html
--rw-rw-rw-   0        0        0   514568 2023-05-28 05:03:13.000000 parsetypes-0.2.1/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   222086 2023-05-28 05:03:13.000000 parsetypes-0.2.1/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 05:03:22.912196 parsetypes-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.896637 parsetypes-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.907195 parsetypes-0.2.1/src/parsetypes/
--rw-rw-rw-   0        0        0      621 2023-05-28 05:02:47.000000 parsetypes-0.2.1/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-05-28 04:48:55.000000 parsetypes-0.2.1/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.1/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    34451 2023-05-28 05:02:47.000000 parsetypes-0.2.1/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5345 2023-05-28 04:48:55.000000 parsetypes-0.2.1/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.910195 parsetypes-0.2.1/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     6606 2023-05-28 05:03:22.000000 parsetypes-0.2.1/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-28 05:03:22.000000 parsetypes-0.2.1/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 05:03:22.000000 parsetypes-0.2.1/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-28 05:03:22.000000 parsetypes-0.2.1/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 05:03:22.000000 parsetypes-0.2.1/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 05:03:22.911198 parsetypes-0.2.1/tests/
--rw-rw-rw-   0        0        0    60176 2023-05-28 04:48:55.000000 parsetypes-0.2.1/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.1/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.911326 parsetypes-0.2.2/
+-rw-rw-rw-   0        0        0      795 2023-05-28 05:32:22.000000 parsetypes-0.2.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6616 2023-05-28 05:35:17.911326 parsetypes-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4116 2023-05-28 05:02:47.000000 parsetypes-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.895325 parsetypes-0.2.2/docs/
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.903325 parsetypes-0.2.2/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/index.html
+-rw-rw-rw-   0        0        0   502932 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   208714 2023-05-28 05:35:08.000000 parsetypes-0.2.2/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 05:35:17.911326 parsetypes-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.896325 parsetypes-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.906329 parsetypes-0.2.2/src/parsetypes/
+-rw-rw-rw-   0        0        0      621 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-05-28 05:34:29.000000 parsetypes-0.2.2/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.2/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    34554 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.2/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.909326 parsetypes-0.2.2/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     6616 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 05:35:17.000000 parsetypes-0.2.2/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 05:35:17.910328 parsetypes-0.2.2/tests/
+-rw-rw-rw-   0        0        0    60176 2023-05-28 04:48:55.000000 parsetypes-0.2.2/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.2/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.2.1/CHANGELOG.md` & `parsetypes-0.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1
+### 0.2.1 and 0.2.2
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.1/PKG-INFO` & `parsetypes-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,15 +158,15 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1
+### 0.2.1 and 0.2.2
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.1/README.md` & `parsetypes-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.1/docs/html/favicon.png` & `parsetypes-0.2.2/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.1/docs/html/parsetypes.html` & `parsetypes-0.2.2/docs/html/parsetypes.html`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.1&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.2&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">)</span>
 </span></pre></div>
@@ -474,15 +474,15 @@
 </span><span id="TypeParser-303"><a href="#TypeParser-303"><span class="linenos">303</span></a><span class="sd">			`allow_negative`</span>
 </span><span id="TypeParser-304"><a href="#TypeParser-304"><span class="linenos">304</span></a><span class="sd">			: whether to accept negative values</span>
 </span><span id="TypeParser-305"><a href="#TypeParser-305"><span class="linenos">305</span></a>
 </span><span id="TypeParser-306"><a href="#TypeParser-306"><span class="linenos">306</span></a><span class="sd">			`allow_sign`</span>
 </span><span id="TypeParser-307"><a href="#TypeParser-307"><span class="linenos">307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser-308"><a href="#TypeParser-308"><span class="linenos">308</span></a>
 </span><span id="TypeParser-309"><a href="#TypeParser-309"><span class="linenos">309</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
 </span><span id="TypeParser-311"><a href="#TypeParser-311"><span class="linenos">311</span></a>
 </span><span id="TypeParser-312"><a href="#TypeParser-312"><span class="linenos">312</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser-313"><a href="#TypeParser-313"><span class="linenos">313</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser-314"><a href="#TypeParser-314"><span class="linenos">314</span></a><span class="sd">			whether it is an int</span>
 </span><span id="TypeParser-315"><a href="#TypeParser-315"><span class="linenos">315</span></a>
 </span><span id="TypeParser-316"><a href="#TypeParser-316"><span class="linenos">316</span></a><span class="sd">			Examples</span>
 </span><span id="TypeParser-317"><a href="#TypeParser-317"><span class="linenos">317</span></a><span class="sd">			--------</span>
@@ -543,15 +543,15 @@
 </span><span id="TypeParser-372"><a href="#TypeParser-372"><span class="linenos">372</span></a>
 </span><span id="TypeParser-373"><a href="#TypeParser-373"><span class="linenos">373</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-374"><a href="#TypeParser-374"><span class="linenos">374</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-375"><a href="#TypeParser-375"><span class="linenos">375</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-376"><a href="#TypeParser-376"><span class="linenos">376</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser-377"><a href="#TypeParser-377"><span class="linenos">377</span></a>
 </span><span id="TypeParser-378"><a href="#TypeParser-378"><span class="linenos">378</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-379"><a href="#TypeParser-379"><span class="linenos">379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-379"><a href="#TypeParser-379"><span class="linenos">379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser-380"><a href="#TypeParser-380"><span class="linenos">380</span></a>
 </span><span id="TypeParser-381"><a href="#TypeParser-381"><span class="linenos">381</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser-382"><a href="#TypeParser-382"><span class="linenos">382</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-383"><a href="#TypeParser-383"><span class="linenos">383</span></a>
 </span><span id="TypeParser-384"><a href="#TypeParser-384"><span class="linenos">384</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser-385"><a href="#TypeParser-385"><span class="linenos">385</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-386"><a href="#TypeParser-386"><span class="linenos">386</span></a>
@@ -695,15 +695,15 @@
 </span><span id="TypeParser-524"><a href="#TypeParser-524"><span class="linenos">524</span></a>
 </span><span id="TypeParser-525"><a href="#TypeParser-525"><span class="linenos">525</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-526"><a href="#TypeParser-526"><span class="linenos">526</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-527"><a href="#TypeParser-527"><span class="linenos">527</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-528"><a href="#TypeParser-528"><span class="linenos">528</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-529"><a href="#TypeParser-529"><span class="linenos">529</span></a>
 </span><span id="TypeParser-530"><a href="#TypeParser-530"><span class="linenos">530</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
 </span><span id="TypeParser-532"><a href="#TypeParser-532"><span class="linenos">532</span></a>
 </span><span id="TypeParser-533"><a href="#TypeParser-533"><span class="linenos">533</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser-534"><a href="#TypeParser-534"><span class="linenos">534</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser-535"><a href="#TypeParser-535"><span class="linenos">535</span></a><span class="sd">			parsed int value</span>
 </span><span id="TypeParser-536"><a href="#TypeParser-536"><span class="linenos">536</span></a>
 </span><span id="TypeParser-537"><a href="#TypeParser-537"><span class="linenos">537</span></a><span class="sd">			Raises</span>
 </span><span id="TypeParser-538"><a href="#TypeParser-538"><span class="linenos">538</span></a><span class="sd">			------</span>
@@ -794,15 +794,15 @@
 </span><span id="TypeParser-623"><a href="#TypeParser-623"><span class="linenos">623</span></a>
 </span><span id="TypeParser-624"><a href="#TypeParser-624"><span class="linenos">624</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-625"><a href="#TypeParser-625"><span class="linenos">625</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-626"><a href="#TypeParser-626"><span class="linenos">626</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-627"><a href="#TypeParser-627"><span class="linenos">627</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-628"><a href="#TypeParser-628"><span class="linenos">628</span></a>
 </span><span id="TypeParser-629"><a href="#TypeParser-629"><span class="linenos">629</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-630"><a href="#TypeParser-630"><span class="linenos">630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-630"><a href="#TypeParser-630"><span class="linenos">630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser-631"><a href="#TypeParser-631"><span class="linenos">631</span></a>
 </span><span id="TypeParser-632"><a href="#TypeParser-632"><span class="linenos">632</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser-633"><a href="#TypeParser-633"><span class="linenos">633</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-634"><a href="#TypeParser-634"><span class="linenos">634</span></a>
 </span><span id="TypeParser-635"><a href="#TypeParser-635"><span class="linenos">635</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser-636"><a href="#TypeParser-636"><span class="linenos">636</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-637"><a href="#TypeParser-637"><span class="linenos">637</span></a>
@@ -841,15 +841,15 @@
 </span><span id="TypeParser-670"><a href="#TypeParser-670"><span class="linenos">670</span></a>
 </span><span id="TypeParser-671"><a href="#TypeParser-671"><span class="linenos">671</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-672"><a href="#TypeParser-672"><span class="linenos">672</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-673"><a href="#TypeParser-673"><span class="linenos">673</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-674"><a href="#TypeParser-674"><span class="linenos">674</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-675"><a href="#TypeParser-675"><span class="linenos">675</span></a>
 </span><span id="TypeParser-676"><a href="#TypeParser-676"><span class="linenos">676</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-677"><a href="#TypeParser-677"><span class="linenos">677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-677"><a href="#TypeParser-677"><span class="linenos">677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser-678"><a href="#TypeParser-678"><span class="linenos">678</span></a>
 </span><span id="TypeParser-679"><a href="#TypeParser-679"><span class="linenos">679</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser-680"><a href="#TypeParser-680"><span class="linenos">680</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-681"><a href="#TypeParser-681"><span class="linenos">681</span></a>
 </span><span id="TypeParser-682"><a href="#TypeParser-682"><span class="linenos">682</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser-683"><a href="#TypeParser-683"><span class="linenos">683</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser-684"><a href="#TypeParser-684"><span class="linenos">684</span></a>
@@ -918,259 +918,258 @@
 </span><span id="TypeParser-747"><a href="#TypeParser-747"><span class="linenos">747</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
 </span><span id="TypeParser-748"><a href="#TypeParser-748"><span class="linenos">748</span></a>
 </span><span id="TypeParser-749"><a href="#TypeParser-749"><span class="linenos">749</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
 </span><span id="TypeParser-750"><a href="#TypeParser-750"><span class="linenos">750</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
 </span><span id="TypeParser-751"><a href="#TypeParser-751"><span class="linenos">751</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
 </span><span id="TypeParser-752"><a href="#TypeParser-752"><span class="linenos">752</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
 </span><span id="TypeParser-753"><a href="#TypeParser-753"><span class="linenos">753</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
-</span><span id="TypeParser-754"><a href="#TypeParser-754"><span class="linenos">754</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="n">AnyContainedType</span><span class="p">,</span> <span class="n">reduced_type</span><span class="p">)</span>
-</span><span id="TypeParser-755"><a href="#TypeParser-755"><span class="linenos">755</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
-</span><span id="TypeParser-756"><a href="#TypeParser-756"><span class="linenos">756</span></a>			<span class="k">return</span> <span class="n">r</span>  <span class="c1"># type: ignore</span>
-</span><span id="TypeParser-757"><a href="#TypeParser-757"><span class="linenos">757</span></a>
-</span><span id="TypeParser-758"><a href="#TypeParser-758"><span class="linenos">758</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="TypeParser-754"><a href="#TypeParser-754"><span class="linenos">754</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
+</span><span id="TypeParser-755"><a href="#TypeParser-755"><span class="linenos">755</span></a>			<span class="k">return</span> <span class="n">r</span>
+</span><span id="TypeParser-756"><a href="#TypeParser-756"><span class="linenos">756</span></a>
+</span><span id="TypeParser-757"><a href="#TypeParser-757"><span class="linenos">757</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="TypeParser-758"><a href="#TypeParser-758"><span class="linenos">758</span></a>
 </span><span id="TypeParser-759"><a href="#TypeParser-759"><span class="linenos">759</span></a>
-</span><span id="TypeParser-760"><a href="#TypeParser-760"><span class="linenos">760</span></a>
-</span><span id="TypeParser-761"><a href="#TypeParser-761"><span class="linenos">761</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser-762"><a href="#TypeParser-762"><span class="linenos">762</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-763"><a href="#TypeParser-763"><span class="linenos">763</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
-</span><span id="TypeParser-764"><a href="#TypeParser-764"><span class="linenos">764</span></a>
-</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos">765</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-766"><a href="#TypeParser-766"><span class="linenos">766</span></a>
-</span><span id="TypeParser-767"><a href="#TypeParser-767"><span class="linenos">767</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-768"><a href="#TypeParser-768"><span class="linenos">768</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-769"><a href="#TypeParser-769"><span class="linenos">769</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-770"><a href="#TypeParser-770"><span class="linenos">770</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
-</span><span id="TypeParser-771"><a href="#TypeParser-771"><span class="linenos">771</span></a>
-</span><span id="TypeParser-772"><a href="#TypeParser-772"><span class="linenos">772</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-773"><a href="#TypeParser-773"><span class="linenos">773</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-774"><a href="#TypeParser-774"><span class="linenos">774</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser-775"><a href="#TypeParser-775"><span class="linenos">775</span></a>
-</span><span id="TypeParser-776"><a href="#TypeParser-776"><span class="linenos">776</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-777"><a href="#TypeParser-777"><span class="linenos">777</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-778"><a href="#TypeParser-778"><span class="linenos">778</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos">779</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos">780</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
-</span><span id="TypeParser-781"><a href="#TypeParser-781"><span class="linenos">781</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
-</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos">782</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
-</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos">783</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos">784</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos">785</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-760"><a href="#TypeParser-760"><span class="linenos">760</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser-761"><a href="#TypeParser-761"><span class="linenos">761</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-762"><a href="#TypeParser-762"><span class="linenos">762</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
+</span><span id="TypeParser-763"><a href="#TypeParser-763"><span class="linenos">763</span></a>
+</span><span id="TypeParser-764"><a href="#TypeParser-764"><span class="linenos">764</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos">765</span></a>
+</span><span id="TypeParser-766"><a href="#TypeParser-766"><span class="linenos">766</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-767"><a href="#TypeParser-767"><span class="linenos">767</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-768"><a href="#TypeParser-768"><span class="linenos">768</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-769"><a href="#TypeParser-769"><span class="linenos">769</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
+</span><span id="TypeParser-770"><a href="#TypeParser-770"><span class="linenos">770</span></a>
+</span><span id="TypeParser-771"><a href="#TypeParser-771"><span class="linenos">771</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-772"><a href="#TypeParser-772"><span class="linenos">772</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-773"><a href="#TypeParser-773"><span class="linenos">773</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser-774"><a href="#TypeParser-774"><span class="linenos">774</span></a>
+</span><span id="TypeParser-775"><a href="#TypeParser-775"><span class="linenos">775</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-776"><a href="#TypeParser-776"><span class="linenos">776</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-777"><a href="#TypeParser-777"><span class="linenos">777</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-778"><a href="#TypeParser-778"><span class="linenos">778</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos">779</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
+</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos">780</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
+</span><span id="TypeParser-781"><a href="#TypeParser-781"><span class="linenos">781</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
+</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos">782</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos">783</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos">784</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos">785</span></a>
 </span><span id="TypeParser-786"><a href="#TypeParser-786"><span class="linenos">786</span></a>
-</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos">787</span></a>
-</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos">788</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
-</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos">789</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos">790</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
-</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos">791</span></a>
-</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos">792</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos">793</span></a>
-</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos">794</span></a><span class="sd">			Note that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos">795</span></a>
-</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos">796</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos">797</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos">798</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos">799</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
-</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos">800</span></a>
-</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos">801</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos">802</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos">803</span></a><span class="sd">			inferred types</span>
-</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos">804</span></a>
-</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos">805</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos">806</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos">807</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos">808</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos">809</span></a><span class="sd">			parser.infer_table([</span>
-</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos">810</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos">811</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos">812</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos">813</span></a><span class="sd">			])</span>
-</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos">814</span></a><span class="sd">			# [float, int, str]</span>
-</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos">815</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos">816</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos">817</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos">818</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-</span><span id="TypeParser-819"><a href="#TypeParser-819"><span class="linenos">819</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos">820</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos">821</span></a>
-</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos">822</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
-</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos">823</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos">824</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos">825</span></a>
-</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos">826</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
-</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos">827</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
-</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos">828</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
-</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos">829</span></a>
-</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos">830</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos">787</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
+</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos">788</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos">789</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
+</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos">790</span></a>
+</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos">791</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos">792</span></a>
+</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos">793</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos">794</span></a>
+</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos">795</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos">796</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos">797</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos">798</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
+</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos">799</span></a>
+</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos">800</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos">801</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos">802</span></a><span class="sd">			inferred types</span>
+</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos">803</span></a>
+</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos">804</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos">805</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos">806</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos">807</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos">808</span></a><span class="sd">			parser.infer_table([</span>
+</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos">809</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos">810</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos">811</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos">812</span></a><span class="sd">			])</span>
+</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos">813</span></a><span class="sd">			# [float, int, str]</span>
+</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos">814</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos">815</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos">816</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos">817</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos">818</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-819"><a href="#TypeParser-819"><span class="linenos">819</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos">820</span></a>
+</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos">821</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
+</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos">822</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos">823</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos">824</span></a>
+</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos">825</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
+</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos">826</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
+</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos">827</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
+</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos">828</span></a>
+</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos">829</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos">830</span></a>
 </span><span id="TypeParser-831"><a href="#TypeParser-831"><span class="linenos">831</span></a>
-</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos">832</span></a>
-</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos">833</span></a>	<span class="k">def</span> <span class="nf">_convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos">834</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
-</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos">835</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
-</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos">836</span></a>			<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos">837</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos">838</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos">839</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos">840</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos">841</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos">842</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos">843</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos">844</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos">845</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos">846</span></a>			<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos">847</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
-</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos">848</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos">849</span></a>				<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos">850</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos">851</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos">852</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos">853</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
-</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos">854</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos">855</span></a>					<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos">856</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
-</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos">857</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos">858</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos">859</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos">860</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos">861</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos">862</span></a>				<span class="k">return</span> <span class="n">cast</span><span class="p">(</span><span class="n">AnyContained</span><span class="p">,</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">])</span>
-</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos">863</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos">864</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
-</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos">865</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos">866</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos">832</span></a>	<span class="k">def</span> <span class="nf">_convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos">833</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
+</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos">834</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
+</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos">835</span></a>			<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos">836</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos">837</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos">838</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos">839</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos">840</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos">841</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos">842</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos">843</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos">844</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos">845</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos">846</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
+</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos">847</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos">848</span></a>				<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos">849</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos">850</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos">851</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos">852</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
+</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos">853</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos">854</span></a>					<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos">855</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
+</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos">856</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos">857</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos">858</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos">859</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos">860</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos">861</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos">862</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos">863</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
+</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos">864</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos">865</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos">866</span></a>
 </span><span id="TypeParser-867"><a href="#TypeParser-867"><span class="linenos">867</span></a>
-</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos">868</span></a>
-</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos">869</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-870"><a href="#TypeParser-870"><span class="linenos">870</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos">871</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos">872</span></a>
-</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos">873</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos">874</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos">875</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos">876</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos">877</span></a>
-</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos">878</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos">879</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos">880</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos">881</span></a>
-</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos">882</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos">883</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos">884</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos">885</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos">888</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos">889</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos">890</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos">891</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos">868</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos">869</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-870"><a href="#TypeParser-870"><span class="linenos">870</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos">871</span></a>
+</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos">872</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos">873</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos">874</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos">875</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos">876</span></a>
+</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos">877</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos">878</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos">879</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos">880</span></a>
+</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos">881</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos">882</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos">883</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos">884</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos">885</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos">888</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos">889</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos">890</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos">891</span></a>
 </span><span id="TypeParser-892"><a href="#TypeParser-892"><span class="linenos">892</span></a>
-</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos">893</span></a>
-</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos">894</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos">895</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos">896</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos">897</span></a>
-</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos">898</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos">899</span></a>
-</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos">900</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos">901</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos">902</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos">903</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos">904</span></a>
-</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos">905</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos">906</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos">907</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos">908</span></a>
-</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos">909</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos">910</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos">911</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos">912</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos">916</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos">917</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos">918</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos">919</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser-920"><a href="#TypeParser-920"><span class="linenos">920</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos">893</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos">894</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos">895</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos">896</span></a>
+</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos">897</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos">898</span></a>
+</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos">899</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos">900</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos">901</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos">902</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos">903</span></a>
+</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos">904</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos">905</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos">906</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos">907</span></a>
+</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos">908</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos">909</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos">910</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos">911</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos">912</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos">916</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos">917</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos">918</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos">919</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+</span><span id="TypeParser-920"><a href="#TypeParser-920"><span class="linenos">920</span></a>
 </span><span id="TypeParser-921"><a href="#TypeParser-921"><span class="linenos">921</span></a>
-</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos">922</span></a>
-</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos">923</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos">924</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos">925</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos">926</span></a>
-</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos">927</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos">928</span></a>
-</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos">929</span></a><span class="sd">			Note that the type inference requires that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos">930</span></a>
-</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos">931</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
-</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos">932</span></a>
-</span><span id="TypeParser-933"><a href="#TypeParser-933"><span class="linenos">933</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos">934</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos">935</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-936"><a href="#TypeParser-936"><span class="linenos">936</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos">937</span></a>
-</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos">938</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser-939"><a href="#TypeParser-939"><span class="linenos">939</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos">940</span></a>
-</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos">941</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos">942</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos">943</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos">944</span></a>
-</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos">945</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos">946</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos">947</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos">948</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos">949</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos">950</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos">951</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos">952</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos">953</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos">954</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos">955</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos">956</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos">957</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos">958</span></a><span class="sd">			]</span>
-</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos">959</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos">960</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos">961</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos">922</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos">923</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos">924</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
+</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos">925</span></a>
+</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos">926</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos">927</span></a>
+</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos">928</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos">929</span></a>
+</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos">930</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
+</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos">931</span></a>
+</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos">932</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-933"><a href="#TypeParser-933"><span class="linenos">933</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos">934</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos">935</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-936"><a href="#TypeParser-936"><span class="linenos">936</span></a>
+</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos">937</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos">938</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser-939"><a href="#TypeParser-939"><span class="linenos">939</span></a>
+</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos">940</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos">941</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos">942</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos">943</span></a>
+</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos">944</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos">945</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos">946</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos">947</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos">948</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos">949</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos">950</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos">951</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos">952</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos">953</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos">954</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos">955</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos">956</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos">957</span></a><span class="sd">			]</span>
+</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos">958</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos">959</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos">960</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos">961</span></a>
 </span><span id="TypeParser-962"><a href="#TypeParser-962"><span class="linenos">962</span></a>
-</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos">963</span></a>
-</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos">964</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos">965</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos">966</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos">967</span></a>
-</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos">968</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos">969</span></a>
-</span><span id="TypeParser-970"><a href="#TypeParser-970"><span class="linenos">970</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type inference still requires that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos">971</span></a>
-</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos">972</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos">973</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos">974</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos">975</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos">976</span></a>
-</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos">977</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos">978</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos">979</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos">980</span></a>
-</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos">981</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos">982</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos">983</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos">984</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos">985</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos">986</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos">987</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos">988</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos">989</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos">992</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos">993</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos">994</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos">995</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos">996</span></a>
-</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos">997</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser-998"><a href="#TypeParser-998"><span class="linenos">998</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos">963</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos">964</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos">965</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
+</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos">966</span></a>
+</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos">967</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos">968</span></a>
+</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos">969</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-970"><a href="#TypeParser-970"><span class="linenos">970</span></a>
+</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos">971</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos">972</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos">973</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos">974</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos">975</span></a>
+</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos">976</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos">977</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos">978</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos">979</span></a>
+</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos">980</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos">981</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos">982</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos">983</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos">984</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos">985</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos">986</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos">987</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos">988</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos">989</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos">992</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos">993</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos">994</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos">995</span></a>
+</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos">996</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos">997</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</p>
 
 <p>Instances of this class can be configured with different settings for the parser and inferrer. See the constructor for more details about the available options.</p></div>
@@ -1570,15 +1569,15 @@
 </span><span id="TypeParser.is_int-303"><a href="#TypeParser.is_int-303"><span class="linenos">303</span></a><span class="sd">			`allow_negative`</span>
 </span><span id="TypeParser.is_int-304"><a href="#TypeParser.is_int-304"><span class="linenos">304</span></a><span class="sd">			: whether to accept negative values</span>
 </span><span id="TypeParser.is_int-305"><a href="#TypeParser.is_int-305"><span class="linenos">305</span></a>
 </span><span id="TypeParser.is_int-306"><a href="#TypeParser.is_int-306"><span class="linenos">306</span></a><span class="sd">			`allow_sign`</span>
 </span><span id="TypeParser.is_int-307"><a href="#TypeParser.is_int-307"><span class="linenos">307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser.is_int-308"><a href="#TypeParser.is_int-308"><span class="linenos">308</span></a>
 </span><span id="TypeParser.is_int-309"><a href="#TypeParser.is_int-309"><span class="linenos">309</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.is_int-310"><a href="#TypeParser.is_int-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser.is_int-310"><a href="#TypeParser.is_int-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
 </span><span id="TypeParser.is_int-311"><a href="#TypeParser.is_int-311"><span class="linenos">311</span></a>
 </span><span id="TypeParser.is_int-312"><a href="#TypeParser.is_int-312"><span class="linenos">312</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser.is_int-313"><a href="#TypeParser.is_int-313"><span class="linenos">313</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser.is_int-314"><a href="#TypeParser.is_int-314"><span class="linenos">314</span></a><span class="sd">			whether it is an int</span>
 </span><span id="TypeParser.is_int-315"><a href="#TypeParser.is_int-315"><span class="linenos">315</span></a>
 </span><span id="TypeParser.is_int-316"><a href="#TypeParser.is_int-316"><span class="linenos">316</span></a><span class="sd">			Examples</span>
 </span><span id="TypeParser.is_int-317"><a href="#TypeParser.is_int-317"><span class="linenos">317</span></a><span class="sd">			--------</span>
@@ -1641,15 +1640,15 @@
 <p><code>allow_negative</code>
 : whether to accept negative values</p>
 
 <p><code>allow_sign</code>
 : whether to accept signed values. If False, it implies that <code>allow_negative</code> is False also.</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> <em>must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
 
 <h2 id="returns">Returns</h2>
 
 <p>whether it is an int</p>
 
 <h2 id="examples">Examples</h2>
 
@@ -1687,15 +1686,15 @@
 </span><span id="TypeParser.is_float-372"><a href="#TypeParser.is_float-372"><span class="linenos">372</span></a>
 </span><span id="TypeParser.is_float-373"><a href="#TypeParser.is_float-373"><span class="linenos">373</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.is_float-374"><a href="#TypeParser.is_float-374"><span class="linenos">374</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.is_float-375"><a href="#TypeParser.is_float-375"><span class="linenos">375</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.is_float-376"><a href="#TypeParser.is_float-376"><span class="linenos">376</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser.is_float-377"><a href="#TypeParser.is_float-377"><span class="linenos">377</span></a>
 </span><span id="TypeParser.is_float-378"><a href="#TypeParser.is_float-378"><span class="linenos">378</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.is_float-379"><a href="#TypeParser.is_float-379"><span class="linenos">379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser.is_float-379"><a href="#TypeParser.is_float-379"><span class="linenos">379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser.is_float-380"><a href="#TypeParser.is_float-380"><span class="linenos">380</span></a>
 </span><span id="TypeParser.is_float-381"><a href="#TypeParser.is_float-381"><span class="linenos">381</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser.is_float-382"><a href="#TypeParser.is_float-382"><span class="linenos">382</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.is_float-383"><a href="#TypeParser.is_float-383"><span class="linenos">383</span></a>
 </span><span id="TypeParser.is_float-384"><a href="#TypeParser.is_float-384"><span class="linenos">384</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser.is_float-385"><a href="#TypeParser.is_float-385"><span class="linenos">385</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.is_float-386"><a href="#TypeParser.is_float-386"><span class="linenos">386</span></a>
@@ -1759,15 +1758,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>value</code>
 : string to be checked</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
 
 <p><code>allow_inf</code>
 : whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
 <p><code>allow_nan</code>
 : whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
@@ -1996,15 +1995,15 @@
 </span><span id="TypeParser.parse_int-524"><a href="#TypeParser.parse_int-524"><span class="linenos">524</span></a>
 </span><span id="TypeParser.parse_int-525"><a href="#TypeParser.parse_int-525"><span class="linenos">525</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.parse_int-526"><a href="#TypeParser.parse_int-526"><span class="linenos">526</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.parse_int-527"><a href="#TypeParser.parse_int-527"><span class="linenos">527</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.parse_int-528"><a href="#TypeParser.parse_int-528"><span class="linenos">528</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_int-529"><a href="#TypeParser.parse_int-529"><span class="linenos">529</span></a>
 </span><span id="TypeParser.parse_int-530"><a href="#TypeParser.parse_int-530"><span class="linenos">530</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_int-531"><a href="#TypeParser.parse_int-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser.parse_int-531"><a href="#TypeParser.parse_int-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
 </span><span id="TypeParser.parse_int-532"><a href="#TypeParser.parse_int-532"><span class="linenos">532</span></a>
 </span><span id="TypeParser.parse_int-533"><a href="#TypeParser.parse_int-533"><span class="linenos">533</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser.parse_int-534"><a href="#TypeParser.parse_int-534"><span class="linenos">534</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser.parse_int-535"><a href="#TypeParser.parse_int-535"><span class="linenos">535</span></a><span class="sd">			parsed int value</span>
 </span><span id="TypeParser.parse_int-536"><a href="#TypeParser.parse_int-536"><span class="linenos">536</span></a>
 </span><span id="TypeParser.parse_int-537"><a href="#TypeParser.parse_int-537"><span class="linenos">537</span></a><span class="sd">			Raises</span>
 </span><span id="TypeParser.parse_int-538"><a href="#TypeParser.parse_int-538"><span class="linenos">538</span></a><span class="sd">			------</span>
@@ -2048,15 +2047,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>value</code>
 : string to be parsed</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> <em>must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
 
 <h2 id="returns">Returns</h2>
 
 <p>parsed int value</p>
 
 <h2 id="raises">Raises</h2>
 
@@ -2097,15 +2096,15 @@
 </span><span id="TypeParser.parse_float-623"><a href="#TypeParser.parse_float-623"><span class="linenos">623</span></a>
 </span><span id="TypeParser.parse_float-624"><a href="#TypeParser.parse_float-624"><span class="linenos">624</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.parse_float-625"><a href="#TypeParser.parse_float-625"><span class="linenos">625</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.parse_float-626"><a href="#TypeParser.parse_float-626"><span class="linenos">626</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.parse_float-627"><a href="#TypeParser.parse_float-627"><span class="linenos">627</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_float-628"><a href="#TypeParser.parse_float-628"><span class="linenos">628</span></a>
 </span><span id="TypeParser.parse_float-629"><a href="#TypeParser.parse_float-629"><span class="linenos">629</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_float-630"><a href="#TypeParser.parse_float-630"><span class="linenos">630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser.parse_float-630"><a href="#TypeParser.parse_float-630"><span class="linenos">630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser.parse_float-631"><a href="#TypeParser.parse_float-631"><span class="linenos">631</span></a>
 </span><span id="TypeParser.parse_float-632"><a href="#TypeParser.parse_float-632"><span class="linenos">632</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser.parse_float-633"><a href="#TypeParser.parse_float-633"><span class="linenos">633</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.parse_float-634"><a href="#TypeParser.parse_float-634"><span class="linenos">634</span></a>
 </span><span id="TypeParser.parse_float-635"><a href="#TypeParser.parse_float-635"><span class="linenos">635</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser.parse_float-636"><a href="#TypeParser.parse_float-636"><span class="linenos">636</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.parse_float-637"><a href="#TypeParser.parse_float-637"><span class="linenos">637</span></a>
@@ -2144,15 +2143,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>value</code>
 : string to be parsed</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
 
 <p><code>allow_inf</code>
 : whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
 <p><code>allow_nan</code>
 : whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
@@ -2200,15 +2199,15 @@
 </span><span id="TypeParser.parse_decimal-670"><a href="#TypeParser.parse_decimal-670"><span class="linenos">670</span></a>
 </span><span id="TypeParser.parse_decimal-671"><a href="#TypeParser.parse_decimal-671"><span class="linenos">671</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.parse_decimal-672"><a href="#TypeParser.parse_decimal-672"><span class="linenos">672</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.parse_decimal-673"><a href="#TypeParser.parse_decimal-673"><span class="linenos">673</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.parse_decimal-674"><a href="#TypeParser.parse_decimal-674"><span class="linenos">674</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_decimal-675"><a href="#TypeParser.parse_decimal-675"><span class="linenos">675</span></a>
 </span><span id="TypeParser.parse_decimal-676"><a href="#TypeParser.parse_decimal-676"><span class="linenos">676</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_decimal-677"><a href="#TypeParser.parse_decimal-677"><span class="linenos">677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form `&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;` will be interpreted as the expression `&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)`, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser.parse_decimal-677"><a href="#TypeParser.parse_decimal-677"><span class="linenos">677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser.parse_decimal-678"><a href="#TypeParser.parse_decimal-678"><span class="linenos">678</span></a>
 </span><span id="TypeParser.parse_decimal-679"><a href="#TypeParser.parse_decimal-679"><span class="linenos">679</span></a><span class="sd">			`allow_inf`</span>
 </span><span id="TypeParser.parse_decimal-680"><a href="#TypeParser.parse_decimal-680"><span class="linenos">680</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.parse_decimal-681"><a href="#TypeParser.parse_decimal-681"><span class="linenos">681</span></a>
 </span><span id="TypeParser.parse_decimal-682"><a href="#TypeParser.parse_decimal-682"><span class="linenos">682</span></a><span class="sd">			`allow_nan`</span>
 </span><span id="TypeParser.parse_decimal-683"><a href="#TypeParser.parse_decimal-683"><span class="linenos">683</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
 </span><span id="TypeParser.parse_decimal-684"><a href="#TypeParser.parse_decimal-684"><span class="linenos">684</span></a>
@@ -2247,15 +2246,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>value</code>
 : string to be parsed</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>
 
 <p><code>allow_inf</code>
 : whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
 <p><code>allow_nan</code>
 : whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>
 
@@ -2282,15 +2281,15 @@
 
                             </div>
                             <div id="TypeParser.infer" class="classattr">
                                         <input id="TypeParser.infer-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]</span>:</span></span>
+        <span class="name">infer</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer-710"><a href="#TypeParser.infer-710"><span class="linenos">710</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
@@ -2333,19 +2332,18 @@
 </span><span id="TypeParser.infer-747"><a href="#TypeParser.infer-747"><span class="linenos">747</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
 </span><span id="TypeParser.infer-748"><a href="#TypeParser.infer-748"><span class="linenos">748</span></a>
 </span><span id="TypeParser.infer-749"><a href="#TypeParser.infer-749"><span class="linenos">749</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
 </span><span id="TypeParser.infer-750"><a href="#TypeParser.infer-750"><span class="linenos">750</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
 </span><span id="TypeParser.infer-751"><a href="#TypeParser.infer-751"><span class="linenos">751</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
 </span><span id="TypeParser.infer-752"><a href="#TypeParser.infer-752"><span class="linenos">752</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
 </span><span id="TypeParser.infer-753"><a href="#TypeParser.infer-753"><span class="linenos">753</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
-</span><span id="TypeParser.infer-754"><a href="#TypeParser.infer-754"><span class="linenos">754</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="n">AnyContainedType</span><span class="p">,</span> <span class="n">reduced_type</span><span class="p">)</span>
-</span><span id="TypeParser.infer-755"><a href="#TypeParser.infer-755"><span class="linenos">755</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
-</span><span id="TypeParser.infer-756"><a href="#TypeParser.infer-756"><span class="linenos">756</span></a>			<span class="k">return</span> <span class="n">r</span>  <span class="c1"># type: ignore</span>
-</span><span id="TypeParser.infer-757"><a href="#TypeParser.infer-757"><span class="linenos">757</span></a>
-</span><span id="TypeParser.infer-758"><a href="#TypeParser.infer-758"><span class="linenos">758</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="TypeParser.infer-754"><a href="#TypeParser.infer-754"><span class="linenos">754</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
+</span><span id="TypeParser.infer-755"><a href="#TypeParser.infer-755"><span class="linenos">755</span></a>			<span class="k">return</span> <span class="n">r</span>
+</span><span id="TypeParser.infer-756"><a href="#TypeParser.infer-756"><span class="linenos">756</span></a>
+</span><span id="TypeParser.infer-757"><a href="#TypeParser.infer-757"><span class="linenos">757</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying type of a string</p>
 
 <p>Also check for inline lists if <code>self.list_delimiter</code> is not None.</p>
@@ -2373,46 +2371,46 @@
 
                             </div>
                             <div id="TypeParser.infer_series" class="classattr">
                                         <input id="TypeParser.infer_series-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]</span>:</span></span>
+        <span class="name">infer_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_series"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_series-761"><a href="#TypeParser.infer_series-761"><span class="linenos">761</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser.infer_series-762"><a href="#TypeParser.infer_series-762"><span class="linenos">762</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_series-763"><a href="#TypeParser.infer_series-763"><span class="linenos">763</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
-</span><span id="TypeParser.infer_series-764"><a href="#TypeParser.infer_series-764"><span class="linenos">764</span></a>
-</span><span id="TypeParser.infer_series-765"><a href="#TypeParser.infer_series-765"><span class="linenos">765</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.infer_series-766"><a href="#TypeParser.infer_series-766"><span class="linenos">766</span></a>
-</span><span id="TypeParser.infer_series-767"><a href="#TypeParser.infer_series-767"><span class="linenos">767</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.infer_series-768"><a href="#TypeParser.infer_series-768"><span class="linenos">768</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.infer_series-769"><a href="#TypeParser.infer_series-769"><span class="linenos">769</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser.infer_series-770"><a href="#TypeParser.infer_series-770"><span class="linenos">770</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
-</span><span id="TypeParser.infer_series-771"><a href="#TypeParser.infer_series-771"><span class="linenos">771</span></a>
-</span><span id="TypeParser.infer_series-772"><a href="#TypeParser.infer_series-772"><span class="linenos">772</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.infer_series-773"><a href="#TypeParser.infer_series-773"><span class="linenos">773</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.infer_series-774"><a href="#TypeParser.infer_series-774"><span class="linenos">774</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser.infer_series-775"><a href="#TypeParser.infer_series-775"><span class="linenos">775</span></a>
-</span><span id="TypeParser.infer_series-776"><a href="#TypeParser.infer_series-776"><span class="linenos">776</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.infer_series-777"><a href="#TypeParser.infer_series-777"><span class="linenos">777</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.infer_series-778"><a href="#TypeParser.infer_series-778"><span class="linenos">778</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.infer_series-779"><a href="#TypeParser.infer_series-779"><span class="linenos">779</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.infer_series-780"><a href="#TypeParser.infer_series-780"><span class="linenos">780</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
-</span><span id="TypeParser.infer_series-781"><a href="#TypeParser.infer_series-781"><span class="linenos">781</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
-</span><span id="TypeParser.infer_series-782"><a href="#TypeParser.infer_series-782"><span class="linenos">782</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
-</span><span id="TypeParser.infer_series-783"><a href="#TypeParser.infer_series-783"><span class="linenos">783</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.infer_series-784"><a href="#TypeParser.infer_series-784"><span class="linenos">784</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_series-785"><a href="#TypeParser.infer_series-785"><span class="linenos">785</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_series-760"><a href="#TypeParser.infer_series-760"><span class="linenos">760</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser.infer_series-761"><a href="#TypeParser.infer_series-761"><span class="linenos">761</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_series-762"><a href="#TypeParser.infer_series-762"><span class="linenos">762</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
+</span><span id="TypeParser.infer_series-763"><a href="#TypeParser.infer_series-763"><span class="linenos">763</span></a>
+</span><span id="TypeParser.infer_series-764"><a href="#TypeParser.infer_series-764"><span class="linenos">764</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.infer_series-765"><a href="#TypeParser.infer_series-765"><span class="linenos">765</span></a>
+</span><span id="TypeParser.infer_series-766"><a href="#TypeParser.infer_series-766"><span class="linenos">766</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.infer_series-767"><a href="#TypeParser.infer_series-767"><span class="linenos">767</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.infer_series-768"><a href="#TypeParser.infer_series-768"><span class="linenos">768</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser.infer_series-769"><a href="#TypeParser.infer_series-769"><span class="linenos">769</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
+</span><span id="TypeParser.infer_series-770"><a href="#TypeParser.infer_series-770"><span class="linenos">770</span></a>
+</span><span id="TypeParser.infer_series-771"><a href="#TypeParser.infer_series-771"><span class="linenos">771</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.infer_series-772"><a href="#TypeParser.infer_series-772"><span class="linenos">772</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.infer_series-773"><a href="#TypeParser.infer_series-773"><span class="linenos">773</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser.infer_series-774"><a href="#TypeParser.infer_series-774"><span class="linenos">774</span></a>
+</span><span id="TypeParser.infer_series-775"><a href="#TypeParser.infer_series-775"><span class="linenos">775</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.infer_series-776"><a href="#TypeParser.infer_series-776"><span class="linenos">776</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.infer_series-777"><a href="#TypeParser.infer_series-777"><span class="linenos">777</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.infer_series-778"><a href="#TypeParser.infer_series-778"><span class="linenos">778</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.infer_series-779"><a href="#TypeParser.infer_series-779"><span class="linenos">779</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
+</span><span id="TypeParser.infer_series-780"><a href="#TypeParser.infer_series-780"><span class="linenos">780</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
+</span><span id="TypeParser.infer_series-781"><a href="#TypeParser.infer_series-781"><span class="linenos">781</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
+</span><span id="TypeParser.infer_series-782"><a href="#TypeParser.infer_series-782"><span class="linenos">782</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.infer_series-783"><a href="#TypeParser.infer_series-783"><span class="linenos">783</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_series-784"><a href="#TypeParser.infer_series-784"><span class="linenos">784</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying common type of a series of strings</p>
 
 <p>If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2440,73 +2438,73 @@
 
                             </div>
                             <div id="TypeParser.infer_table" class="classattr">
                                         <input id="TypeParser.infer_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]]</span>:</span></span>
+        <span class="name">infer_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Type</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_table-788"><a href="#TypeParser.infer_table-788"><span class="linenos">788</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
-</span><span id="TypeParser.infer_table-789"><a href="#TypeParser.infer_table-789"><span class="linenos">789</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_table-790"><a href="#TypeParser.infer_table-790"><span class="linenos">790</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
-</span><span id="TypeParser.infer_table-791"><a href="#TypeParser.infer_table-791"><span class="linenos">791</span></a>
-</span><span id="TypeParser.infer_table-792"><a href="#TypeParser.infer_table-792"><span class="linenos">792</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.infer_table-793"><a href="#TypeParser.infer_table-793"><span class="linenos">793</span></a>
-</span><span id="TypeParser.infer_table-794"><a href="#TypeParser.infer_table-794"><span class="linenos">794</span></a><span class="sd">			Note that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.infer_table-795"><a href="#TypeParser.infer_table-795"><span class="linenos">795</span></a>
-</span><span id="TypeParser.infer_table-796"><a href="#TypeParser.infer_table-796"><span class="linenos">796</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.infer_table-797"><a href="#TypeParser.infer_table-797"><span class="linenos">797</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.infer_table-798"><a href="#TypeParser.infer_table-798"><span class="linenos">798</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.infer_table-799"><a href="#TypeParser.infer_table-799"><span class="linenos">799</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
-</span><span id="TypeParser.infer_table-800"><a href="#TypeParser.infer_table-800"><span class="linenos">800</span></a>
-</span><span id="TypeParser.infer_table-801"><a href="#TypeParser.infer_table-801"><span class="linenos">801</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.infer_table-802"><a href="#TypeParser.infer_table-802"><span class="linenos">802</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.infer_table-803"><a href="#TypeParser.infer_table-803"><span class="linenos">803</span></a><span class="sd">			inferred types</span>
-</span><span id="TypeParser.infer_table-804"><a href="#TypeParser.infer_table-804"><span class="linenos">804</span></a>
-</span><span id="TypeParser.infer_table-805"><a href="#TypeParser.infer_table-805"><span class="linenos">805</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.infer_table-806"><a href="#TypeParser.infer_table-806"><span class="linenos">806</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.infer_table-807"><a href="#TypeParser.infer_table-807"><span class="linenos">807</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.infer_table-808"><a href="#TypeParser.infer_table-808"><span class="linenos">808</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.infer_table-809"><a href="#TypeParser.infer_table-809"><span class="linenos">809</span></a><span class="sd">			parser.infer_table([</span>
-</span><span id="TypeParser.infer_table-810"><a href="#TypeParser.infer_table-810"><span class="linenos">810</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.infer_table-811"><a href="#TypeParser.infer_table-811"><span class="linenos">811</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.infer_table-812"><a href="#TypeParser.infer_table-812"><span class="linenos">812</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser.infer_table-813"><a href="#TypeParser.infer_table-813"><span class="linenos">813</span></a><span class="sd">			])</span>
-</span><span id="TypeParser.infer_table-814"><a href="#TypeParser.infer_table-814"><span class="linenos">814</span></a><span class="sd">			# [float, int, str]</span>
-</span><span id="TypeParser.infer_table-815"><a href="#TypeParser.infer_table-815"><span class="linenos">815</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.infer_table-816"><a href="#TypeParser.infer_table-816"><span class="linenos">816</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_table-817"><a href="#TypeParser.infer_table-817"><span class="linenos">817</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-818"><a href="#TypeParser.infer_table-818"><span class="linenos">818</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-819"><a href="#TypeParser.infer_table-819"><span class="linenos">819</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-820"><a href="#TypeParser.infer_table-820"><span class="linenos">820</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser.infer_table-821"><a href="#TypeParser.infer_table-821"><span class="linenos">821</span></a>
-</span><span id="TypeParser.infer_table-822"><a href="#TypeParser.infer_table-822"><span class="linenos">822</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-823"><a href="#TypeParser.infer_table-823"><span class="linenos">823</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-824"><a href="#TypeParser.infer_table-824"><span class="linenos">824</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser.infer_table-825"><a href="#TypeParser.infer_table-825"><span class="linenos">825</span></a>
-</span><span id="TypeParser.infer_table-826"><a href="#TypeParser.infer_table-826"><span class="linenos">826</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
-</span><span id="TypeParser.infer_table-827"><a href="#TypeParser.infer_table-827"><span class="linenos">827</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-828"><a href="#TypeParser.infer_table-828"><span class="linenos">828</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
-</span><span id="TypeParser.infer_table-829"><a href="#TypeParser.infer_table-829"><span class="linenos">829</span></a>
-</span><span id="TypeParser.infer_table-830"><a href="#TypeParser.infer_table-830"><span class="linenos">830</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_table-787"><a href="#TypeParser.infer_table-787"><span class="linenos">787</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
+</span><span id="TypeParser.infer_table-788"><a href="#TypeParser.infer_table-788"><span class="linenos">788</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_table-789"><a href="#TypeParser.infer_table-789"><span class="linenos">789</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
+</span><span id="TypeParser.infer_table-790"><a href="#TypeParser.infer_table-790"><span class="linenos">790</span></a>
+</span><span id="TypeParser.infer_table-791"><a href="#TypeParser.infer_table-791"><span class="linenos">791</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.infer_table-792"><a href="#TypeParser.infer_table-792"><span class="linenos">792</span></a>
+</span><span id="TypeParser.infer_table-793"><a href="#TypeParser.infer_table-793"><span class="linenos">793</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.infer_table-794"><a href="#TypeParser.infer_table-794"><span class="linenos">794</span></a>
+</span><span id="TypeParser.infer_table-795"><a href="#TypeParser.infer_table-795"><span class="linenos">795</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.infer_table-796"><a href="#TypeParser.infer_table-796"><span class="linenos">796</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.infer_table-797"><a href="#TypeParser.infer_table-797"><span class="linenos">797</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.infer_table-798"><a href="#TypeParser.infer_table-798"><span class="linenos">798</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
+</span><span id="TypeParser.infer_table-799"><a href="#TypeParser.infer_table-799"><span class="linenos">799</span></a>
+</span><span id="TypeParser.infer_table-800"><a href="#TypeParser.infer_table-800"><span class="linenos">800</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.infer_table-801"><a href="#TypeParser.infer_table-801"><span class="linenos">801</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.infer_table-802"><a href="#TypeParser.infer_table-802"><span class="linenos">802</span></a><span class="sd">			inferred types</span>
+</span><span id="TypeParser.infer_table-803"><a href="#TypeParser.infer_table-803"><span class="linenos">803</span></a>
+</span><span id="TypeParser.infer_table-804"><a href="#TypeParser.infer_table-804"><span class="linenos">804</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.infer_table-805"><a href="#TypeParser.infer_table-805"><span class="linenos">805</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.infer_table-806"><a href="#TypeParser.infer_table-806"><span class="linenos">806</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.infer_table-807"><a href="#TypeParser.infer_table-807"><span class="linenos">807</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.infer_table-808"><a href="#TypeParser.infer_table-808"><span class="linenos">808</span></a><span class="sd">			parser.infer_table([</span>
+</span><span id="TypeParser.infer_table-809"><a href="#TypeParser.infer_table-809"><span class="linenos">809</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.infer_table-810"><a href="#TypeParser.infer_table-810"><span class="linenos">810</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.infer_table-811"><a href="#TypeParser.infer_table-811"><span class="linenos">811</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser.infer_table-812"><a href="#TypeParser.infer_table-812"><span class="linenos">812</span></a><span class="sd">			])</span>
+</span><span id="TypeParser.infer_table-813"><a href="#TypeParser.infer_table-813"><span class="linenos">813</span></a><span class="sd">			# [float, int, str]</span>
+</span><span id="TypeParser.infer_table-814"><a href="#TypeParser.infer_table-814"><span class="linenos">814</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.infer_table-815"><a href="#TypeParser.infer_table-815"><span class="linenos">815</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_table-816"><a href="#TypeParser.infer_table-816"><span class="linenos">816</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-817"><a href="#TypeParser.infer_table-817"><span class="linenos">817</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-818"><a href="#TypeParser.infer_table-818"><span class="linenos">818</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-819"><a href="#TypeParser.infer_table-819"><span class="linenos">819</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser.infer_table-820"><a href="#TypeParser.infer_table-820"><span class="linenos">820</span></a>
+</span><span id="TypeParser.infer_table-821"><a href="#TypeParser.infer_table-821"><span class="linenos">821</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-822"><a href="#TypeParser.infer_table-822"><span class="linenos">822</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-823"><a href="#TypeParser.infer_table-823"><span class="linenos">823</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser.infer_table-824"><a href="#TypeParser.infer_table-824"><span class="linenos">824</span></a>
+</span><span id="TypeParser.infer_table-825"><a href="#TypeParser.infer_table-825"><span class="linenos">825</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
+</span><span id="TypeParser.infer_table-826"><a href="#TypeParser.infer_table-826"><span class="linenos">826</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-827"><a href="#TypeParser.infer_table-827"><span class="linenos">827</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
+</span><span id="TypeParser.infer_table-828"><a href="#TypeParser.infer_table-828"><span class="linenos">828</span></a>
+</span><span id="TypeParser.infer_table-829"><a href="#TypeParser.infer_table-829"><span class="linenos">829</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying common type for each column of a table of strings</p>
 
 <p>For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
 
-<p>Note that the inferred types of every individual value must all be able to fit into memory at once.</p>
+<p>Note that the individual inferred types of every value in the table must be able to fit into memory.</p>
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>rows</code>
 : table of strings for which the types should be inferred, in row-major order</p>
 
 <h2 id="returns">Returns</h2>
@@ -2530,44 +2528,44 @@
 
                             </div>
                             <div id="TypeParser.parse" class="classattr">
                                         <input id="TypeParser.parse-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">parse</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]</span>:</span></span>
+        <span class="name">parse</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-869"><a href="#TypeParser.parse-869"><span class="linenos">869</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser.parse-870"><a href="#TypeParser.parse-870"><span class="linenos">870</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-871"><a href="#TypeParser.parse-871"><span class="linenos">871</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser.parse-872"><a href="#TypeParser.parse-872"><span class="linenos">872</span></a>
-</span><span id="TypeParser.parse-873"><a href="#TypeParser.parse-873"><span class="linenos">873</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse-874"><a href="#TypeParser.parse-874"><span class="linenos">874</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse-875"><a href="#TypeParser.parse-875"><span class="linenos">875</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.parse-876"><a href="#TypeParser.parse-876"><span class="linenos">876</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser.parse-877"><a href="#TypeParser.parse-877"><span class="linenos">877</span></a>
-</span><span id="TypeParser.parse-878"><a href="#TypeParser.parse-878"><span class="linenos">878</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse-879"><a href="#TypeParser.parse-879"><span class="linenos">879</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse-880"><a href="#TypeParser.parse-880"><span class="linenos">880</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser.parse-881"><a href="#TypeParser.parse-881"><span class="linenos">881</span></a>
-</span><span id="TypeParser.parse-882"><a href="#TypeParser.parse-882"><span class="linenos">882</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse-883"><a href="#TypeParser.parse-883"><span class="linenos">883</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse-884"><a href="#TypeParser.parse-884"><span class="linenos">884</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse-885"><a href="#TypeParser.parse-885"><span class="linenos">885</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse-886"><a href="#TypeParser.parse-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser.parse-887"><a href="#TypeParser.parse-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser.parse-888"><a href="#TypeParser.parse-888"><span class="linenos">888</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser.parse-889"><a href="#TypeParser.parse-889"><span class="linenos">889</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse-890"><a href="#TypeParser.parse-890"><span class="linenos">890</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-891"><a href="#TypeParser.parse-891"><span class="linenos">891</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-868"><a href="#TypeParser.parse-868"><span class="linenos">868</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser.parse-869"><a href="#TypeParser.parse-869"><span class="linenos">869</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-870"><a href="#TypeParser.parse-870"><span class="linenos">870</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser.parse-871"><a href="#TypeParser.parse-871"><span class="linenos">871</span></a>
+</span><span id="TypeParser.parse-872"><a href="#TypeParser.parse-872"><span class="linenos">872</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse-873"><a href="#TypeParser.parse-873"><span class="linenos">873</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse-874"><a href="#TypeParser.parse-874"><span class="linenos">874</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.parse-875"><a href="#TypeParser.parse-875"><span class="linenos">875</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser.parse-876"><a href="#TypeParser.parse-876"><span class="linenos">876</span></a>
+</span><span id="TypeParser.parse-877"><a href="#TypeParser.parse-877"><span class="linenos">877</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse-878"><a href="#TypeParser.parse-878"><span class="linenos">878</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse-879"><a href="#TypeParser.parse-879"><span class="linenos">879</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser.parse-880"><a href="#TypeParser.parse-880"><span class="linenos">880</span></a>
+</span><span id="TypeParser.parse-881"><a href="#TypeParser.parse-881"><span class="linenos">881</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse-882"><a href="#TypeParser.parse-882"><span class="linenos">882</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse-883"><a href="#TypeParser.parse-883"><span class="linenos">883</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse-884"><a href="#TypeParser.parse-884"><span class="linenos">884</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse-885"><a href="#TypeParser.parse-885"><span class="linenos">885</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser.parse-886"><a href="#TypeParser.parse-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser.parse-887"><a href="#TypeParser.parse-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser.parse-888"><a href="#TypeParser.parse-888"><span class="linenos">888</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse-889"><a href="#TypeParser.parse-889"><span class="linenos">889</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-890"><a href="#TypeParser.parse-890"><span class="linenos">890</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and convert it to its underlying type</p>
 
 <h2 id="parameters">Parameters</h2>
@@ -2593,48 +2591,48 @@
 
                             </div>
                             <div id="TypeParser.parse_series" class="classattr">
                                         <input id="TypeParser.parse_series-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">parse_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]</span>:</span></span>
+        <span class="name">parse_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_series"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-894"><a href="#TypeParser.parse_series-894"><span class="linenos">894</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser.parse_series-895"><a href="#TypeParser.parse_series-895"><span class="linenos">895</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-896"><a href="#TypeParser.parse_series-896"><span class="linenos">896</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser.parse_series-897"><a href="#TypeParser.parse_series-897"><span class="linenos">897</span></a>
-</span><span id="TypeParser.parse_series-898"><a href="#TypeParser.parse_series-898"><span class="linenos">898</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_series-899"><a href="#TypeParser.parse_series-899"><span class="linenos">899</span></a>
-</span><span id="TypeParser.parse_series-900"><a href="#TypeParser.parse_series-900"><span class="linenos">900</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse_series-901"><a href="#TypeParser.parse_series-901"><span class="linenos">901</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse_series-902"><a href="#TypeParser.parse_series-902"><span class="linenos">902</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser.parse_series-903"><a href="#TypeParser.parse_series-903"><span class="linenos">903</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser.parse_series-904"><a href="#TypeParser.parse_series-904"><span class="linenos">904</span></a>
-</span><span id="TypeParser.parse_series-905"><a href="#TypeParser.parse_series-905"><span class="linenos">905</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_series-906"><a href="#TypeParser.parse_series-906"><span class="linenos">906</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_series-907"><a href="#TypeParser.parse_series-907"><span class="linenos">907</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser.parse_series-908"><a href="#TypeParser.parse_series-908"><span class="linenos">908</span></a>
-</span><span id="TypeParser.parse_series-909"><a href="#TypeParser.parse_series-909"><span class="linenos">909</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_series-910"><a href="#TypeParser.parse_series-910"><span class="linenos">910</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_series-911"><a href="#TypeParser.parse_series-911"><span class="linenos">911</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_series-912"><a href="#TypeParser.parse_series-912"><span class="linenos">912</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_series-913"><a href="#TypeParser.parse_series-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser.parse_series-914"><a href="#TypeParser.parse_series-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser.parse_series-915"><a href="#TypeParser.parse_series-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser.parse_series-916"><a href="#TypeParser.parse_series-916"><span class="linenos">916</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser.parse_series-917"><a href="#TypeParser.parse_series-917"><span class="linenos">917</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_series-918"><a href="#TypeParser.parse_series-918"><span class="linenos">918</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-919"><a href="#TypeParser.parse_series-919"><span class="linenos">919</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser.parse_series-920"><a href="#TypeParser.parse_series-920"><span class="linenos">920</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-893"><a href="#TypeParser.parse_series-893"><span class="linenos">893</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser.parse_series-894"><a href="#TypeParser.parse_series-894"><span class="linenos">894</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-895"><a href="#TypeParser.parse_series-895"><span class="linenos">895</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser.parse_series-896"><a href="#TypeParser.parse_series-896"><span class="linenos">896</span></a>
+</span><span id="TypeParser.parse_series-897"><a href="#TypeParser.parse_series-897"><span class="linenos">897</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_series-898"><a href="#TypeParser.parse_series-898"><span class="linenos">898</span></a>
+</span><span id="TypeParser.parse_series-899"><a href="#TypeParser.parse_series-899"><span class="linenos">899</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse_series-900"><a href="#TypeParser.parse_series-900"><span class="linenos">900</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse_series-901"><a href="#TypeParser.parse_series-901"><span class="linenos">901</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser.parse_series-902"><a href="#TypeParser.parse_series-902"><span class="linenos">902</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser.parse_series-903"><a href="#TypeParser.parse_series-903"><span class="linenos">903</span></a>
+</span><span id="TypeParser.parse_series-904"><a href="#TypeParser.parse_series-904"><span class="linenos">904</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_series-905"><a href="#TypeParser.parse_series-905"><span class="linenos">905</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_series-906"><a href="#TypeParser.parse_series-906"><span class="linenos">906</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser.parse_series-907"><a href="#TypeParser.parse_series-907"><span class="linenos">907</span></a>
+</span><span id="TypeParser.parse_series-908"><a href="#TypeParser.parse_series-908"><span class="linenos">908</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_series-909"><a href="#TypeParser.parse_series-909"><span class="linenos">909</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_series-910"><a href="#TypeParser.parse_series-910"><span class="linenos">910</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_series-911"><a href="#TypeParser.parse_series-911"><span class="linenos">911</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_series-912"><a href="#TypeParser.parse_series-912"><span class="linenos">912</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser.parse_series-913"><a href="#TypeParser.parse_series-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser.parse_series-914"><a href="#TypeParser.parse_series-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser.parse_series-915"><a href="#TypeParser.parse_series-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser.parse_series-916"><a href="#TypeParser.parse_series-916"><span class="linenos">916</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_series-917"><a href="#TypeParser.parse_series-917"><span class="linenos">917</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-918"><a href="#TypeParser.parse_series-918"><span class="linenos">918</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser.parse_series-919"><a href="#TypeParser.parse_series-919"><span class="linenos">919</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a series of strings and convert them to their underlying common type</p>
 
 <p>If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2663,69 +2661,69 @@
 
                             </div>
                             <div id="TypeParser.parse_table" class="classattr">
                                         <input id="TypeParser.parse_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">parse_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]]</span>:</span></span>
+        <span class="name">parse_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-923"><a href="#TypeParser.parse_table-923"><span class="linenos">923</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.parse_table-924"><a href="#TypeParser.parse_table-924"><span class="linenos">924</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-925"><a href="#TypeParser.parse_table-925"><span class="linenos">925</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser.parse_table-926"><a href="#TypeParser.parse_table-926"><span class="linenos">926</span></a>
-</span><span id="TypeParser.parse_table-927"><a href="#TypeParser.parse_table-927"><span class="linenos">927</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_table-928"><a href="#TypeParser.parse_table-928"><span class="linenos">928</span></a>
-</span><span id="TypeParser.parse_table-929"><a href="#TypeParser.parse_table-929"><span class="linenos">929</span></a><span class="sd">			Note that the type inference requires that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.parse_table-930"><a href="#TypeParser.parse_table-930"><span class="linenos">930</span></a>
-</span><span id="TypeParser.parse_table-931"><a href="#TypeParser.parse_table-931"><span class="linenos">931</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
-</span><span id="TypeParser.parse_table-932"><a href="#TypeParser.parse_table-932"><span class="linenos">932</span></a>
-</span><span id="TypeParser.parse_table-933"><a href="#TypeParser.parse_table-933"><span class="linenos">933</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse_table-934"><a href="#TypeParser.parse_table-934"><span class="linenos">934</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse_table-935"><a href="#TypeParser.parse_table-935"><span class="linenos">935</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.parse_table-936"><a href="#TypeParser.parse_table-936"><span class="linenos">936</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.parse_table-937"><a href="#TypeParser.parse_table-937"><span class="linenos">937</span></a>
-</span><span id="TypeParser.parse_table-938"><a href="#TypeParser.parse_table-938"><span class="linenos">938</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser.parse_table-939"><a href="#TypeParser.parse_table-939"><span class="linenos">939</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.parse_table-940"><a href="#TypeParser.parse_table-940"><span class="linenos">940</span></a>
-</span><span id="TypeParser.parse_table-941"><a href="#TypeParser.parse_table-941"><span class="linenos">941</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_table-942"><a href="#TypeParser.parse_table-942"><span class="linenos">942</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_table-943"><a href="#TypeParser.parse_table-943"><span class="linenos">943</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser.parse_table-944"><a href="#TypeParser.parse_table-944"><span class="linenos">944</span></a>
-</span><span id="TypeParser.parse_table-945"><a href="#TypeParser.parse_table-945"><span class="linenos">945</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_table-946"><a href="#TypeParser.parse_table-946"><span class="linenos">946</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_table-947"><a href="#TypeParser.parse_table-947"><span class="linenos">947</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_table-948"><a href="#TypeParser.parse_table-948"><span class="linenos">948</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_table-949"><a href="#TypeParser.parse_table-949"><span class="linenos">949</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser.parse_table-950"><a href="#TypeParser.parse_table-950"><span class="linenos">950</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-951"><a href="#TypeParser.parse_table-951"><span class="linenos">951</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-952"><a href="#TypeParser.parse_table-952"><span class="linenos">952</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-953"><a href="#TypeParser.parse_table-953"><span class="linenos">953</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.parse_table-954"><a href="#TypeParser.parse_table-954"><span class="linenos">954</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser.parse_table-955"><a href="#TypeParser.parse_table-955"><span class="linenos">955</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-956"><a href="#TypeParser.parse_table-956"><span class="linenos">956</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-957"><a href="#TypeParser.parse_table-957"><span class="linenos">957</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-958"><a href="#TypeParser.parse_table-958"><span class="linenos">958</span></a><span class="sd">			]</span>
-</span><span id="TypeParser.parse_table-959"><a href="#TypeParser.parse_table-959"><span class="linenos">959</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_table-960"><a href="#TypeParser.parse_table-960"><span class="linenos">960</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-961"><a href="#TypeParser.parse_table-961"><span class="linenos">961</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-922"><a href="#TypeParser.parse_table-922"><span class="linenos">922</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.parse_table-923"><a href="#TypeParser.parse_table-923"><span class="linenos">923</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-924"><a href="#TypeParser.parse_table-924"><span class="linenos">924</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
+</span><span id="TypeParser.parse_table-925"><a href="#TypeParser.parse_table-925"><span class="linenos">925</span></a>
+</span><span id="TypeParser.parse_table-926"><a href="#TypeParser.parse_table-926"><span class="linenos">926</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_table-927"><a href="#TypeParser.parse_table-927"><span class="linenos">927</span></a>
+</span><span id="TypeParser.parse_table-928"><a href="#TypeParser.parse_table-928"><span class="linenos">928</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.parse_table-929"><a href="#TypeParser.parse_table-929"><span class="linenos">929</span></a>
+</span><span id="TypeParser.parse_table-930"><a href="#TypeParser.parse_table-930"><span class="linenos">930</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
+</span><span id="TypeParser.parse_table-931"><a href="#TypeParser.parse_table-931"><span class="linenos">931</span></a>
+</span><span id="TypeParser.parse_table-932"><a href="#TypeParser.parse_table-932"><span class="linenos">932</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse_table-933"><a href="#TypeParser.parse_table-933"><span class="linenos">933</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse_table-934"><a href="#TypeParser.parse_table-934"><span class="linenos">934</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.parse_table-935"><a href="#TypeParser.parse_table-935"><span class="linenos">935</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.parse_table-936"><a href="#TypeParser.parse_table-936"><span class="linenos">936</span></a>
+</span><span id="TypeParser.parse_table-937"><a href="#TypeParser.parse_table-937"><span class="linenos">937</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser.parse_table-938"><a href="#TypeParser.parse_table-938"><span class="linenos">938</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser.parse_table-939"><a href="#TypeParser.parse_table-939"><span class="linenos">939</span></a>
+</span><span id="TypeParser.parse_table-940"><a href="#TypeParser.parse_table-940"><span class="linenos">940</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_table-941"><a href="#TypeParser.parse_table-941"><span class="linenos">941</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_table-942"><a href="#TypeParser.parse_table-942"><span class="linenos">942</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser.parse_table-943"><a href="#TypeParser.parse_table-943"><span class="linenos">943</span></a>
+</span><span id="TypeParser.parse_table-944"><a href="#TypeParser.parse_table-944"><span class="linenos">944</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_table-945"><a href="#TypeParser.parse_table-945"><span class="linenos">945</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_table-946"><a href="#TypeParser.parse_table-946"><span class="linenos">946</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_table-947"><a href="#TypeParser.parse_table-947"><span class="linenos">947</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_table-948"><a href="#TypeParser.parse_table-948"><span class="linenos">948</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser.parse_table-949"><a href="#TypeParser.parse_table-949"><span class="linenos">949</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-950"><a href="#TypeParser.parse_table-950"><span class="linenos">950</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-951"><a href="#TypeParser.parse_table-951"><span class="linenos">951</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-952"><a href="#TypeParser.parse_table-952"><span class="linenos">952</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.parse_table-953"><a href="#TypeParser.parse_table-953"><span class="linenos">953</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser.parse_table-954"><a href="#TypeParser.parse_table-954"><span class="linenos">954</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-955"><a href="#TypeParser.parse_table-955"><span class="linenos">955</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-956"><a href="#TypeParser.parse_table-956"><span class="linenos">956</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-957"><a href="#TypeParser.parse_table-957"><span class="linenos">957</span></a><span class="sd">			]</span>
+</span><span id="TypeParser.parse_table-958"><a href="#TypeParser.parse_table-958"><span class="linenos">958</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_table-959"><a href="#TypeParser.parse_table-959"><span class="linenos">959</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-960"><a href="#TypeParser.parse_table-960"><span class="linenos">960</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings and convert them to the underlying common type of each column</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
 
-<p>Note that the type inference requires that the inferred types of every individual value must all be able to fit into memory at once.</p>
+<p>Note that the type to which the values should be converted is determined by <code><a href="#TypeParser.infer_table">infer_table()</a></code>, and so the individual inferred types of every value in the table must be able to fit into memory.</p>
 
 <p>This is a function that computes the entire table and returns it all at once. The generator <code><a href="#TypeParser.iterate_table">iterate_table()</a></code> behaves analogously, except that it computes and yields each row one at a time.</p>
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>rows</code>
 : table of strings to be parsed, in row-major order</p>
@@ -2758,65 +2756,65 @@
 
                             </div>
                             <div id="TypeParser.iterate_table" class="classattr">
                                         <input id="TypeParser.iterate_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">iterate_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]]</span>:</span></span>
+        <span class="name">iterate_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.iterate_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.iterate_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-964"><a href="#TypeParser.iterate_table-964"><span class="linenos">964</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.iterate_table-965"><a href="#TypeParser.iterate_table-965"><span class="linenos">965</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-966"><a href="#TypeParser.iterate_table-966"><span class="linenos">966</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser.iterate_table-967"><a href="#TypeParser.iterate_table-967"><span class="linenos">967</span></a>
-</span><span id="TypeParser.iterate_table-968"><a href="#TypeParser.iterate_table-968"><span class="linenos">968</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.iterate_table-969"><a href="#TypeParser.iterate_table-969"><span class="linenos">969</span></a>
-</span><span id="TypeParser.iterate_table-970"><a href="#TypeParser.iterate_table-970"><span class="linenos">970</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type inference still requires that the inferred types of every individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.iterate_table-971"><a href="#TypeParser.iterate_table-971"><span class="linenos">971</span></a>
-</span><span id="TypeParser.iterate_table-972"><a href="#TypeParser.iterate_table-972"><span class="linenos">972</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.iterate_table-973"><a href="#TypeParser.iterate_table-973"><span class="linenos">973</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.iterate_table-974"><a href="#TypeParser.iterate_table-974"><span class="linenos">974</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.iterate_table-975"><a href="#TypeParser.iterate_table-975"><span class="linenos">975</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.iterate_table-976"><a href="#TypeParser.iterate_table-976"><span class="linenos">976</span></a>
-</span><span id="TypeParser.iterate_table-977"><a href="#TypeParser.iterate_table-977"><span class="linenos">977</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser.iterate_table-978"><a href="#TypeParser.iterate_table-978"><span class="linenos">978</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.iterate_table-979"><a href="#TypeParser.iterate_table-979"><span class="linenos">979</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser.iterate_table-980"><a href="#TypeParser.iterate_table-980"><span class="linenos">980</span></a>
-</span><span id="TypeParser.iterate_table-981"><a href="#TypeParser.iterate_table-981"><span class="linenos">981</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.iterate_table-982"><a href="#TypeParser.iterate_table-982"><span class="linenos">982</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.iterate_table-983"><a href="#TypeParser.iterate_table-983"><span class="linenos">983</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.iterate_table-984"><a href="#TypeParser.iterate_table-984"><span class="linenos">984</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.iterate_table-985"><a href="#TypeParser.iterate_table-985"><span class="linenos">985</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser.iterate_table-986"><a href="#TypeParser.iterate_table-986"><span class="linenos">986</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.iterate_table-987"><a href="#TypeParser.iterate_table-987"><span class="linenos">987</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.iterate_table-988"><a href="#TypeParser.iterate_table-988"><span class="linenos">988</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser.iterate_table-989"><a href="#TypeParser.iterate_table-989"><span class="linenos">989</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.iterate_table-990"><a href="#TypeParser.iterate_table-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser.iterate_table-991"><a href="#TypeParser.iterate_table-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser.iterate_table-992"><a href="#TypeParser.iterate_table-992"><span class="linenos">992</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser.iterate_table-993"><a href="#TypeParser.iterate_table-993"><span class="linenos">993</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.iterate_table-994"><a href="#TypeParser.iterate_table-994"><span class="linenos">994</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-995"><a href="#TypeParser.iterate_table-995"><span class="linenos">995</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser.iterate_table-996"><a href="#TypeParser.iterate_table-996"><span class="linenos">996</span></a>
-</span><span id="TypeParser.iterate_table-997"><a href="#TypeParser.iterate_table-997"><span class="linenos">997</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser.iterate_table-998"><a href="#TypeParser.iterate_table-998"><span class="linenos">998</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-963"><a href="#TypeParser.iterate_table-963"><span class="linenos">963</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.iterate_table-964"><a href="#TypeParser.iterate_table-964"><span class="linenos">964</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-965"><a href="#TypeParser.iterate_table-965"><span class="linenos">965</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
+</span><span id="TypeParser.iterate_table-966"><a href="#TypeParser.iterate_table-966"><span class="linenos">966</span></a>
+</span><span id="TypeParser.iterate_table-967"><a href="#TypeParser.iterate_table-967"><span class="linenos">967</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.iterate_table-968"><a href="#TypeParser.iterate_table-968"><span class="linenos">968</span></a>
+</span><span id="TypeParser.iterate_table-969"><a href="#TypeParser.iterate_table-969"><span class="linenos">969</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.iterate_table-970"><a href="#TypeParser.iterate_table-970"><span class="linenos">970</span></a>
+</span><span id="TypeParser.iterate_table-971"><a href="#TypeParser.iterate_table-971"><span class="linenos">971</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.iterate_table-972"><a href="#TypeParser.iterate_table-972"><span class="linenos">972</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.iterate_table-973"><a href="#TypeParser.iterate_table-973"><span class="linenos">973</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.iterate_table-974"><a href="#TypeParser.iterate_table-974"><span class="linenos">974</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.iterate_table-975"><a href="#TypeParser.iterate_table-975"><span class="linenos">975</span></a>
+</span><span id="TypeParser.iterate_table-976"><a href="#TypeParser.iterate_table-976"><span class="linenos">976</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser.iterate_table-977"><a href="#TypeParser.iterate_table-977"><span class="linenos">977</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.iterate_table-978"><a href="#TypeParser.iterate_table-978"><span class="linenos">978</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser.iterate_table-979"><a href="#TypeParser.iterate_table-979"><span class="linenos">979</span></a>
+</span><span id="TypeParser.iterate_table-980"><a href="#TypeParser.iterate_table-980"><span class="linenos">980</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.iterate_table-981"><a href="#TypeParser.iterate_table-981"><span class="linenos">981</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.iterate_table-982"><a href="#TypeParser.iterate_table-982"><span class="linenos">982</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.iterate_table-983"><a href="#TypeParser.iterate_table-983"><span class="linenos">983</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.iterate_table-984"><a href="#TypeParser.iterate_table-984"><span class="linenos">984</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser.iterate_table-985"><a href="#TypeParser.iterate_table-985"><span class="linenos">985</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.iterate_table-986"><a href="#TypeParser.iterate_table-986"><span class="linenos">986</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.iterate_table-987"><a href="#TypeParser.iterate_table-987"><span class="linenos">987</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser.iterate_table-988"><a href="#TypeParser.iterate_table-988"><span class="linenos">988</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.iterate_table-989"><a href="#TypeParser.iterate_table-989"><span class="linenos">989</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser.iterate_table-990"><a href="#TypeParser.iterate_table-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser.iterate_table-991"><a href="#TypeParser.iterate_table-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser.iterate_table-992"><a href="#TypeParser.iterate_table-992"><span class="linenos">992</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.iterate_table-993"><a href="#TypeParser.iterate_table-993"><span class="linenos">993</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-994"><a href="#TypeParser.iterate_table-994"><span class="linenos">994</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser.iterate_table-995"><a href="#TypeParser.iterate_table-995"><span class="linenos">995</span></a>
+</span><span id="TypeParser.iterate_table-996"><a href="#TypeParser.iterate_table-996"><span class="linenos">996</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser.iterate_table-997"><a href="#TypeParser.iterate_table-997"><span class="linenos">997</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings for the underlying common type of each column, then convert and yield each row</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
 
-<p>This is a generator that computes and yields each row one at a time. The function <code><a href="#TypeParser.parse_table">parse_table()</a></code> behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type inference still requires that the inferred types of every individual value must all be able to fit into memory at once.</p>
+<p>This is a generator that computes and yields each row one at a time. The function <code><a href="#TypeParser.parse_table">parse_table()</a></code> behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by <code><a href="#TypeParser.infer_table">infer_table()</a></code>, and so the individual inferred types of every value in the table must be able to fit into memory.</p>
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>rows</code>
 : table of strings to be parsed, in row-major order</p>
 
 <h2 id="yields">Yields</h2>
@@ -2872,60 +2870,60 @@
                             </div>
                 </section>
                 <section id="reduce_types">
                             <input id="reduce_types-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">reduce_types</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">int</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">float</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="nb">bool</span><span class="p">],</span> <span class="n">parsetypes</span><span class="o">.</span><span class="n">_common</span><span class="o">.</span><span class="n">Nullable</span><span class="p">[</span><span class="n">NoneType</span><span class="p">]]]</span>:</span></span>
+        <span class="name">reduce_types</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="reduce_types-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#reduce_types"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="reduce_types-157"><a href="#reduce_types-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">reduce_types</span><span class="p">(</span><span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="reduce_types-158"><a href="#reduce_types-158"><span class="linenos">158</span></a><span class="w">	</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="reduce_types-159"><a href="#reduce_types-159"><span class="linenos">159</span></a><span class="sd">		Reduce multiple types into a single common type.</span>
-</span><span id="reduce_types-160"><a href="#reduce_types-160"><span class="linenos">160</span></a>
-</span><span id="reduce_types-161"><a href="#reduce_types-161"><span class="linenos">161</span></a><span class="sd">		If the input types are not all the same, the resulting type will be narrowest possible type that will encompass all of the input types.</span>
-</span><span id="reduce_types-162"><a href="#reduce_types-162"><span class="linenos">162</span></a>
-</span><span id="reduce_types-163"><a href="#reduce_types-163"><span class="linenos">163</span></a><span class="sd">		This operation is useful in cases such as parsing a CSV file where each column should have a consistent type, but where the individual values in a column could be interpreted variously as ints or floats (or other types).</span>
-</span><span id="reduce_types-164"><a href="#reduce_types-164"><span class="linenos">164</span></a>
-</span><span id="reduce_types-165"><a href="#reduce_types-165"><span class="linenos">165</span></a><span class="sd">		Parameters</span>
-</span><span id="reduce_types-166"><a href="#reduce_types-166"><span class="linenos">166</span></a><span class="sd">		----------</span>
-</span><span id="reduce_types-167"><a href="#reduce_types-167"><span class="linenos">167</span></a><span class="sd">		`types`</span>
-</span><span id="reduce_types-168"><a href="#reduce_types-168"><span class="linenos">168</span></a><span class="sd">		: types to be reduced</span>
-</span><span id="reduce_types-169"><a href="#reduce_types-169"><span class="linenos">169</span></a>
-</span><span id="reduce_types-170"><a href="#reduce_types-170"><span class="linenos">170</span></a><span class="sd">		Returns</span>
-</span><span id="reduce_types-171"><a href="#reduce_types-171"><span class="linenos">171</span></a><span class="sd">		-------</span>
-</span><span id="reduce_types-172"><a href="#reduce_types-172"><span class="linenos">172</span></a><span class="sd">		common reduced type</span>
-</span><span id="reduce_types-173"><a href="#reduce_types-173"><span class="linenos">173</span></a>
-</span><span id="reduce_types-174"><a href="#reduce_types-174"><span class="linenos">174</span></a><span class="sd">		Examples</span>
-</span><span id="reduce_types-175"><a href="#reduce_types-175"><span class="linenos">175</span></a><span class="sd">		--------</span>
-</span><span id="reduce_types-176"><a href="#reduce_types-176"><span class="linenos">176</span></a><span class="sd">		```python</span>
-</span><span id="reduce_types-177"><a href="#reduce_types-177"><span class="linenos">177</span></a><span class="sd">		reduce_types([int, float])        # float</span>
-</span><span id="reduce_types-178"><a href="#reduce_types-178"><span class="linenos">178</span></a><span class="sd">		reduce_types([bool, int])         # int</span>
-</span><span id="reduce_types-179"><a href="#reduce_types-179"><span class="linenos">179</span></a><span class="sd">		reduce_types([int, float, str])   # str</span>
-</span><span id="reduce_types-180"><a href="#reduce_types-180"><span class="linenos">180</span></a><span class="sd">		```</span>
-</span><span id="reduce_types-181"><a href="#reduce_types-181"><span class="linenos">181</span></a><span class="sd">	&quot;&quot;&quot;</span>
-</span><span id="reduce_types-182"><a href="#reduce_types-182"><span class="linenos">182</span></a>	<span class="n">reduced_type</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">,</span> <span class="kc">None</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="reduce_types-183"><a href="#reduce_types-183"><span class="linenos">183</span></a>	<span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">types</span><span class="p">:</span>
-</span><span id="reduce_types-184"><a href="#reduce_types-184"><span class="linenos">184</span></a>		<span class="k">if</span> <span class="n">reduced_type</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="reduce_types-185"><a href="#reduce_types-185"><span class="linenos">185</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">t</span>
-</span><span id="reduce_types-186"><a href="#reduce_types-186"><span class="linenos">186</span></a>		<span class="k">elif</span> <span class="n">t</span> <span class="o">!=</span> <span class="n">reduced_type</span><span class="p">:</span>
-</span><span id="reduce_types-187"><a href="#reduce_types-187"><span class="linenos">187</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">_merge_types</span><span class="p">(</span><span class="n">reduced_type</span><span class="p">,</span> <span class="n">t</span><span class="p">)</span>
-</span><span id="reduce_types-188"><a href="#reduce_types-188"><span class="linenos">188</span></a>		<span class="k">if</span> <span class="n">reduced_type</span> <span class="o">==</span> <span class="n">_TerminalValue</span><span class="p">:</span>
-</span><span id="reduce_types-189"><a href="#reduce_types-189"><span class="linenos">189</span></a>			<span class="k">return</span> <span class="n">_TerminalValue</span>
-</span><span id="reduce_types-190"><a href="#reduce_types-190"><span class="linenos">190</span></a>
-</span><span id="reduce_types-191"><a href="#reduce_types-191"><span class="linenos">191</span></a>	<span class="k">if</span> <span class="n">reduced_type</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="reduce_types-192"><a href="#reduce_types-192"><span class="linenos">192</span></a>		<span class="c1"># types is empty</span>
-</span><span id="reduce_types-193"><a href="#reduce_types-193"><span class="linenos">193</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
-</span><span id="reduce_types-194"><a href="#reduce_types-194"><span class="linenos">194</span></a>	<span class="k">else</span><span class="p">:</span>
-</span><span id="reduce_types-195"><a href="#reduce_types-195"><span class="linenos">195</span></a>		<span class="k">return</span> <span class="n">reduced_type</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="reduce_types-156"><a href="#reduce_types-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">reduce_types</span><span class="p">(</span><span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="reduce_types-157"><a href="#reduce_types-157"><span class="linenos">157</span></a><span class="w">	</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="reduce_types-158"><a href="#reduce_types-158"><span class="linenos">158</span></a><span class="sd">		Reduce multiple types into a single common type.</span>
+</span><span id="reduce_types-159"><a href="#reduce_types-159"><span class="linenos">159</span></a>
+</span><span id="reduce_types-160"><a href="#reduce_types-160"><span class="linenos">160</span></a><span class="sd">		If the input types are not all the same, the resulting type will be narrowest possible type that will encompass all of the input types.</span>
+</span><span id="reduce_types-161"><a href="#reduce_types-161"><span class="linenos">161</span></a>
+</span><span id="reduce_types-162"><a href="#reduce_types-162"><span class="linenos">162</span></a><span class="sd">		This operation is useful in cases such as parsing a CSV file where each column should have a consistent type, but where the individual values in a column could be interpreted variously as ints or floats (or other types).</span>
+</span><span id="reduce_types-163"><a href="#reduce_types-163"><span class="linenos">163</span></a>
+</span><span id="reduce_types-164"><a href="#reduce_types-164"><span class="linenos">164</span></a><span class="sd">		Parameters</span>
+</span><span id="reduce_types-165"><a href="#reduce_types-165"><span class="linenos">165</span></a><span class="sd">		----------</span>
+</span><span id="reduce_types-166"><a href="#reduce_types-166"><span class="linenos">166</span></a><span class="sd">		`types`</span>
+</span><span id="reduce_types-167"><a href="#reduce_types-167"><span class="linenos">167</span></a><span class="sd">		: types to be reduced</span>
+</span><span id="reduce_types-168"><a href="#reduce_types-168"><span class="linenos">168</span></a>
+</span><span id="reduce_types-169"><a href="#reduce_types-169"><span class="linenos">169</span></a><span class="sd">		Returns</span>
+</span><span id="reduce_types-170"><a href="#reduce_types-170"><span class="linenos">170</span></a><span class="sd">		-------</span>
+</span><span id="reduce_types-171"><a href="#reduce_types-171"><span class="linenos">171</span></a><span class="sd">		common reduced type</span>
+</span><span id="reduce_types-172"><a href="#reduce_types-172"><span class="linenos">172</span></a>
+</span><span id="reduce_types-173"><a href="#reduce_types-173"><span class="linenos">173</span></a><span class="sd">		Examples</span>
+</span><span id="reduce_types-174"><a href="#reduce_types-174"><span class="linenos">174</span></a><span class="sd">		--------</span>
+</span><span id="reduce_types-175"><a href="#reduce_types-175"><span class="linenos">175</span></a><span class="sd">		```python</span>
+</span><span id="reduce_types-176"><a href="#reduce_types-176"><span class="linenos">176</span></a><span class="sd">		reduce_types([int, float])        # float</span>
+</span><span id="reduce_types-177"><a href="#reduce_types-177"><span class="linenos">177</span></a><span class="sd">		reduce_types([bool, int])         # int</span>
+</span><span id="reduce_types-178"><a href="#reduce_types-178"><span class="linenos">178</span></a><span class="sd">		reduce_types([int, float, str])   # str</span>
+</span><span id="reduce_types-179"><a href="#reduce_types-179"><span class="linenos">179</span></a><span class="sd">		```</span>
+</span><span id="reduce_types-180"><a href="#reduce_types-180"><span class="linenos">180</span></a><span class="sd">	&quot;&quot;&quot;</span>
+</span><span id="reduce_types-181"><a href="#reduce_types-181"><span class="linenos">181</span></a>	<span class="n">reduced_type</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">,</span> <span class="kc">None</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="reduce_types-182"><a href="#reduce_types-182"><span class="linenos">182</span></a>	<span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">types</span><span class="p">:</span>
+</span><span id="reduce_types-183"><a href="#reduce_types-183"><span class="linenos">183</span></a>		<span class="k">if</span> <span class="n">reduced_type</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="reduce_types-184"><a href="#reduce_types-184"><span class="linenos">184</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">t</span>
+</span><span id="reduce_types-185"><a href="#reduce_types-185"><span class="linenos">185</span></a>		<span class="k">elif</span> <span class="n">t</span> <span class="o">!=</span> <span class="n">reduced_type</span><span class="p">:</span>
+</span><span id="reduce_types-186"><a href="#reduce_types-186"><span class="linenos">186</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">_merge_types</span><span class="p">(</span><span class="n">reduced_type</span><span class="p">,</span> <span class="n">t</span><span class="p">)</span>
+</span><span id="reduce_types-187"><a href="#reduce_types-187"><span class="linenos">187</span></a>		<span class="k">if</span> <span class="n">reduced_type</span> <span class="o">==</span> <span class="n">_TerminalValue</span><span class="p">:</span>
+</span><span id="reduce_types-188"><a href="#reduce_types-188"><span class="linenos">188</span></a>			<span class="k">return</span> <span class="n">_TerminalValue</span>
+</span><span id="reduce_types-189"><a href="#reduce_types-189"><span class="linenos">189</span></a>
+</span><span id="reduce_types-190"><a href="#reduce_types-190"><span class="linenos">190</span></a>	<span class="k">if</span> <span class="n">reduced_type</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="reduce_types-191"><a href="#reduce_types-191"><span class="linenos">191</span></a>		<span class="c1"># types is empty</span>
+</span><span id="reduce_types-192"><a href="#reduce_types-192"><span class="linenos">192</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="reduce_types-193"><a href="#reduce_types-193"><span class="linenos">193</span></a>	<span class="k">else</span><span class="p">:</span>
+</span><span id="reduce_types-194"><a href="#reduce_types-194"><span class="linenos">194</span></a>		<span class="k">return</span> <span class="n">reduced_type</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Reduce multiple types into a single common type.</p>
 
 <p>If the input types are not all the same, the resulting type will be narrowest possible type that will encompass all of the input types.</p>
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
-11__version__ = "0.2.1"
+11__version__ = "0.2.2"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types')
@@ -544,19 +544,19 @@
 : whether to accept signed values. If False, it implies that `allow_negative`
 is False also.
 308
 309
 `allow_scientific`
 310
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and
-<var>X</var> *must* be a non-negative integer, even in cases where the above
-expression evaluates mathematically to an integer.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
+be an integer and <var>X</var> *must* be a non-negative integer, even in cases
+where the above expression evaluates mathematically to an integer.
 311
 312
 Returns
 313
 -------
 314
 whether it is an int
@@ -677,18 +677,18 @@
 376
 : string to be checked
 377
 378
 `allow_scientific`
 379
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 380
 381
 `allow_inf`
 382
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -975,19 +975,19 @@
 528
 : string to be parsed
 529
 530
 `allow_scientific`
 531
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and
-<var>X</var> *must* be a non-negative integer, even in cases where the above
-expression evaluates mathematically to an integer.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
+be an integer and <var>X</var> *must* be a non-negative integer, even in cases
+where the above expression evaluates mathematically to an integer.
 532
 533
 Returns
 534
 -------
 535
 parsed int value
@@ -1169,18 +1169,18 @@
 627
 : string to be parsed
 628
 629
 `allow_scientific`
 630
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 631
 632
 `allow_inf`
 633
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -1267,18 +1267,18 @@
 674
 : string to be parsed
 675
 676
 `allow_scientific`
 677
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 678
 679
 `allow_inf`
 680
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -1419,482 +1419,481 @@
 751
 if self.trim:
 752
 subvalues = [subvalue.strip() for subvalue in subvalues]
 753
 reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
 754
-reduced_type = cast(AnyContainedType, reduced_type)
-755
 r = list[reduced_type]
+755
+return r
 756
-return r  # type: ignore
 757
-758
 return GenericValue
+758
 759
 760
-761
 def infer_series(self, values: Iterable[str]) -> AnyValueType:
-762
+761
 """
-763
+762
 Infer the underlying common type of a series of strings
+763
 764
-765
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
+765
 766
-767
 Parameters
-768
+767
 ----------
-769
+768
 `values`
-770
+769
 : series of strings for which the type should be inferred
+770
 771
-772
 Returns
-773
+772
 -------
-774
+773
 inferred type
+774
 775
-776
 Examples
-777
+776
 --------
-778
+777
 ```python
-779
+778
 parser = TypeParser()
-780
+779
 parser.infer_series(["1", "2", "3.4"])       # float
-781
+780
 parser.infer_series(["true", "false", "2"])  # int
-782
+781
 parser.infer_series(["1", "2.3", "abc"])     # str
-783
+782
 ```
-784
+783
 """
-785
+784
 return reduce_types(self.infer(value) for value in values)
+785
 786
 787
-788
 def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
-789
+788
 """
-790
+789
 Infer the underlying common type for each column of a table of strings
+790
 791
-792
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See `parsetypes.reduce_types()` for more information.
+792
 793
+Note that the individual inferred types of every value in the table must be
+able to fit into memory.
 794
-Note that the inferred types of every individual value must all be able to fit
-into memory at once.
 795
-796
 Parameters
-797
+796
 ----------
-798
+797
 `rows`
-799
+798
 : table of strings for which the types should be inferred, in row-major order
+799
 800
-801
 Returns
-802
+801
 -------
-803
+802
 inferred types
+803
 804
-805
 Examples
-806
+805
 --------
-807
+806
 ```python
-808
+807
 parser = TypeParser()
-809
+808
 parser.infer_table([
-810
+809
 ["1",   "true",  "1"],
-811
+810
 ["2",   "false", "2.3"],
-812
+811
 ["3.4", "2",     "abc"],
-813
+812
 ])
-814
+813
 # [float, int, str]
-815
+814
 ```
-816
+815
 """
-817
+816
 rows_iter = iter(rows)
-818
+817
 first_row = next(rows_iter, None)
-819
+818
 if first_row is None:
-820
+819
 return []
+820
 821
-822
 num_cols = len(first_row)
-823
+822
 if num_cols == 0:
-824
+823
 return []
+824
 825
-826
 table = _TypeTable([[self.infer(value)] for value in first_row])
-827
+826
 for row in rows_iter:
-828
+827
 table.add_row([self.infer(value) for value in row])
+828
 829
-830
 return [reduce_types(col) for col in table.cols]
+830
 831
 832
-833
 def _convert(self, value: str, t: AnyValueType) -> AnyValue:
-834
+833
 base, type_args = _decompose_type(t)
-835
+834
 if base == NoneType:
-836
+835
 return None
-837
+836
 elif base == bool:
-838
+837
 return self.parse_bool(value)
-839
+838
 elif base == int:
-840
+839
 return self.parse_int(value)
-841
+840
 elif base == Decimal:
-842
+841
 return self.parse_decimal(value)
-843
+842
 elif base == float:
-844
+843
 return self.parse_float(value)
-845
+844
 elif base == str:
-846
+845
 return value
-847
+846
 elif base == Nullable:
-848
+847
 if self.is_none(value):
-849
+848
 return None
-850
+849
 else:
-851
+850
 if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
-852
+851
 inner_type = type_args[0]
-853
+852
 return self._convert(value, inner_type)
-854
+853
 else:
-855
+854
 return value
-856
+855
 elif base == list:
-857
+856
 subvalues = value.split(self.list_delimiter)
-858
+857
 if self.trim:
-859
+858
 subvalues = [subvalue.strip() for subvalue in subvalues]
-860
+859
 if type_args is not None and len(type_args) == 1 and type_args[0] != str:
-861
+860
 subtype = type_args[0]
+861
+return [self._convert(subvalue, subtype) for subvalue in subvalues]
 862
-return cast(AnyContained, [self._convert(subvalue, subtype) for subvalue in
-subvalues])
-863
 else:
-864
+863
 return subvalues
-865
+864
 else:
-866
+865
 return value
+866
 867
 868
-869
 def parse(self, value: str) -> AnyValue:
-870
+869
 """
-871
+870
 Parse a string and convert it to its underlying type
+871
 872
-873
 Parameters
-874
+873
 ----------
-875
+874
 `value`
-876
+875
 : the string to be parsed
+876
 877
-878
 Returns
-879
+878
 -------
-880
+879
 converted value
+880
 881
-882
 Examples
-883
+882
 --------
-884
+883
 ```python
-885
+884
 parser = TypeParser()
-886
+885
 parser.parse("true")  # True
-887
+886
 parser.parse("2.0")   # 2.
-888
+887
 parser.parse("abc")   # "abc"
-889
+888
 ```
-890
+889
 """
-891
+890
 return self._convert(value, self.infer(value))
+891
 892
 893
-894
 def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
-895
+894
 """
-896
+895
 Parse a series of strings and convert them to their underlying common type
+896
 897
-898
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
+898
 899
-900
 Parameters
-901
+900
 ----------
-902
+901
 `values`
-903
+902
 : series of strings to be parsed
+903
 904
-905
 Returns
-906
+905
 -------
-907
+906
 converted values
+907
 908
-909
 Examples
-910
+909
 --------
-911
+910
 ```python
-912
+911
 parser = TypeParser()
-913
+912
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
-914
+913
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-915
+914
 parser.parse_series(["true", "false", ""])  # [True, False, None]
-916
+915
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
-917
+916
 ```
-918
+917
 """
-919
+918
 inferred = self.infer_series(values)
-920
+919
 return [self._convert(value, inferred) for value in values]
+920
 921
 922
-923
 def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
-924
+923
 """
-925
+924
 Parse a table of strings and convert them to the underlying common type of each
 column
+925
 926
-927
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
+927
 928
+Note that the type to which the values should be converted is determined by
+`infer_table()`, and so the individual inferred types of every value in the
+table must be able to fit into memory.
 929
-Note that the type inference requires that the inferred types of every
-individual value must all be able to fit into memory at once.
 930
-931
 This is a function that computes the entire table and returns it all at once.
 The generator `iterate_table()` behaves analogously, except that it computes
 and yields each row one at a time.
+931
 932
-933
 Parameters
-934
+933
 ----------
-935
+934
 `rows`
-936
+935
 : table of strings to be parsed, in row-major order
+936
 937
-938
 `iterator`
-939
+938
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
+939
 940
-941
 Returns
-942
+941
 -------
-943
+942
 converted table of values, in row-major order
+943
 944
-945
 Examples
-946
+945
 --------
-947
+946
 ```python
-948
+947
 parser = TypeParser()
-949
+948
 table = parser.parse_table([
-950
+949
 ["1", "5",   "true",  "1"],
-951
+950
 ["2", "6.7", "false", "2.3"],
-952
+951
 ["3", "8.0", "",      "abc"],
-953
+952
 ]):
-954
+953
 assert table == [
-955
+954
 [1, 5.,  True,  "1"],
-956
+955
 [2, 6.7, False, "2.3"],
-957
+956
 [3, 8.,  None,  "abc"],
-958
+957
 ]
-959
+958
 ```
-960
+959
 """
-961
+960
 return [converted_row for converted_row in self.iterate_table(rows)]
+961
 962
 963
-964
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-965
+964
 """
-966
+965
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
+966
 967
-968
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
+968
 969
-970
 This is a generator that computes and yields each row one at a time. The
 function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists. However, note that although
-this is a generator, the type inference still requires that the inferred types
-of every individual value must all be able to fit into memory at once.
+this is a generator, the type to which the value sshould be converted is still
+determined by `infer_table()`, and so the individual inferred types of every
+value in the table must be able to fit into memory.
+970
 971
-972
 Parameters
-973
+972
 ----------
-974
+973
 `rows`
-975
+974
 : table of strings to be parsed, in row-major order
+975
 976
-977
 Yields
-978
+977
 -------
-979
+978
 each row of converted table values
+979
 980
-981
 Examples
-982
+981
 --------
-983
+982
 ```python
-984
+983
 parser = TypeParser()
-985
+984
 table = parser.iterate_table([
-986
+985
 ["1",   "true",  "1"],
-987
+986
 ["2",   "false", "2.3"],
-988
+987
 ["3.4", "2",     "abc"],
-989
+988
 ]):
-990
+989
 assert next(table) == [1.,  1, "1"]
-991
+990
 assert next(table) == [2.,  0, "2.3"]
-992
+991
 assert next(table) == [3.4, 2, "abc"]
-993
+992
 ```
-994
+993
 """
-995
+994
 inferred_types = self.infer_table(rows)
+995
 996
-997
 for row in rows:
-998
+997
 yield [self._convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 A parser that can be used to infer the underlying types of data serialised as
 strings, and to convert them into their original underlying types.
 Instances of this class can be configured with different settings for the
 parser and inferrer. See the constructor for more details about the available
 options.
@@ -2452,19 +2451,19 @@
 : whether to accept signed values. If False, it implies that `allow_negative`
 is False also.
 308
 309
 `allow_scientific`
 310
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and
-<var>X</var> *must* be a non-negative integer, even in cases where the above
-expression evaluates mathematically to an integer.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
+be an integer and <var>X</var> *must* be a non-negative integer, even in cases
+where the above expression evaluates mathematically to an integer.
 311
 312
 Returns
 313
 -------
 314
 whether it is an int
@@ -2563,19 +2562,18 @@
 Check if a string represents an int
 ***** Parameters *****
 value : string to be checked
 allow_negative : whether to accept negative values
 allow_sign : whether to accept signed values. If False, it implies that
 allow_negative is False also.
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "<var>M</var>e<var>X</var>" will be interpreted as the expression
-<var>M</var> * (10 ** <var>X</var>), where M is the mantissa/significand and X
-is the exponent. Note M must be an integer and X must be a non-negative
-integer, even in cases where the above expression evaluates mathematically to
-an integer.
+the form "MeX" will be interpreted as the expression M * (10 * X), where M is
+the mantissa/significand and X is the exponent. Note M *must
+ be an integer and X must be a non-negative integer, even in cases where the
+above expression evaluates mathematically to an integer.
 ***** Returns *****
 whether it is an int
 ***** Examples *****
 parser = TypeParser()
 parser.is_int("0")    # True
 parser.is_int("-1")   # True
 parser.is_int("abc")  # False
@@ -2611,18 +2609,18 @@
 376
 : string to be checked
 377
 378
 `allow_scientific`
 379
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 380
 381
 `allow_inf`
 382
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -2735,17 +2733,17 @@
 allow_scientific=False)
 Check if a string represents a float (or equivalently, a Decimal)
 This function will also return True if the string represents an int.
 Alias: is_decimal()
 ***** Parameters *****
 value : string to be checked
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "<var>M</var>e<var>X</var>" will be interpreted as the expression
-<var>M</var> * (10 ** <var>X</var>), where M is the mantissa/significand and X
-is the exponent. Note that X must be an integer, but can be negative.
+the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
+the mantissa/significand and X is the exponent. Note that X must be an integer,
+but can be negative.
 allow_inf : whether to accept positive and negative infinity values. If True,
 strings that match the values in self.inf_values (empty by default) are
 interpreted as infinity, or as negative infinity if prepended by a negative
 sign. The case sensitivity of this matching depends on
 self.float_case_sensitive, which is False by default.
 allow_nan : whether to accept NaN (not a number) representations. If True,
 strings that match the values in self.nan_values (empty by default) are
@@ -2973,19 +2971,19 @@
 528
 : string to be parsed
 529
 530
 `allow_scientific`
 531
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and
-<var>X</var> *must* be a non-negative integer, even in cases where the above
-expression evaluates mathematically to an integer.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
+be an integer and <var>X</var> *must* be a non-negative integer, even in cases
+where the above expression evaluates mathematically to an integer.
 532
 533
 Returns
 534
 -------
 535
 parsed int value
@@ -3054,19 +3052,18 @@
 raise ValueError(f"not an integer: {value}")
 Parse a string and return it as an int if possible
 If the string represents a bool, it will be converted to 1 for True and 0 for
 False.
 ***** Parameters *****
 value : string to be parsed
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "<var>M</var>e<var>X</var>" will be interpreted as the expression
-<var>M</var> * (10 ** <var>X</var>), where M is the mantissa/significand and X
-is the exponent. Note M must be an integer and X must be a non-negative
-integer, even in cases where the above expression evaluates mathematically to
-an integer.
+the form "MeX" will be interpreted as the expression M * (10 * X), where M is
+the mantissa/significand and X is the exponent. Note M *must
+ be an integer and X must be a non-negative integer, even in cases where the
+above expression evaluates mathematically to an integer.
 ***** Returns *****
 parsed int value
 ***** Raises *****
 ValueError if value cannot be parsed
 ***** Examples *****
 parser = TypeParser()
 parser.parse_int("0")    # 0
@@ -3106,18 +3103,18 @@
 627
 : string to be parsed
 628
 629
 `allow_scientific`
 630
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 631
 632
 `allow_inf`
 633
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -3180,17 +3177,17 @@
 If the string represents a bool, it will be converted to 1. for True and 0. for
 False. If the string represents an int, it will be converted to a float also.
 Behaves analogously to parse_decimal(), except that that returns an exact
 Decimal instead.
 ***** Parameters *****
 value : string to be parsed
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "<var>M</var>e<var>X</var>" will be interpreted as the expression
-<var>M</var> * (10 ** <var>X</var>), where M is the mantissa/significand and X
-is the exponent. Note that X must be an integer, but can be negative.
+the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
+the mantissa/significand and X is the exponent. Note that X must be an integer,
+but can be negative.
 allow_inf : whether to accept positive and negative infinity values. If True,
 strings that match the values in self.inf_values (empty by default) are
 interpreted as infinity, or as negative infinity if prepended by a negative
 sign. The case sensitivity of this matching depends on
 self.float_case_sensitive, which is False by default.
 allow_nan : whether to accept NaN (not a number) representations. If True,
 strings that match the values in self.nan_values (empty by default) are
@@ -3240,18 +3237,18 @@
 674
 : string to be parsed
 675
 676
 `allow_scientific`
 677
 : whether to accept scientific notation. If True, strings of the form
-`"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</
-var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand
-and <var>X</var> is the exponent. Note that <var>X</var> must be an integer,
-but can be negative.
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
+must be an integer, but can be negative.
 678
 679
 `allow_inf`
 680
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
@@ -3316,17 +3313,17 @@
 and Decimal(0) for False. If the string represents an int, it will be converted
 to a Decimal also.
 Behaves analogously to parse_float(), except that that returns a non-exact
 float instead.
 ***** Parameters *****
 value : string to be parsed
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "<var>M</var>e<var>X</var>" will be interpreted as the expression
-<var>M</var> * (10 ** <var>X</var>), where M is the mantissa/significand and X
-is the exponent. Note that X must be an integer, but can be negative.
+the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
+the mantissa/significand and X is the exponent. Note that X must be an integer,
+but can be negative.
 allow_inf : whether to accept positive and negative infinity values. If True,
 strings that match the values in self.inf_values (empty by default) are
 interpreted as infinity, or as negative infinity if prepended by a negative
 sign. The case sensitivity of this matching depends on
 self.float_case_sensitive, which is False by default.
 allow_nan : whether to accept NaN (not a number) representations. If True,
 strings that match the values in self.nan_values (empty by default) are
@@ -3342,18 +3339,15 @@
 parser.parse_decimal("1.23e2")   # Decimal(123)
 parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
 parser.parse_decimal("inf")      # Decimal(math.inf)
 ⁰
 def infer(
 self,
 value: str) -> Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
-parsetypes._common.Nullable[str], parsetypes._common.Nullable[int],
-parsetypes._common.Nullable[float], parsetypes._common.Nullable
-[decimal.Decimal], parsetypes._common.Nullable[bool],
-parsetypes._common.Nullable[NoneType]]]: View Source
+Nullable, list]]: View Source
 710
 def infer(self, value: str) -> AnyValueType:
 711
 """
 712
 Infer the underlying type of a string
 713
@@ -3429,21 +3423,19 @@
 751
 if self.trim:
 752
 subvalues = [subvalue.strip() for subvalue in subvalues]
 753
 reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
 754
-reduced_type = cast(AnyContainedType, reduced_type)
-755
 r = list[reduced_type]
+755
+return r
 756
-return r  # type: ignore
 757
-758
 return GenericValue
 Infer the underlying type of a string
 Also check for inline lists if self.list_delimiter is not None.
 ***** Parameters *****
 value : the string for which the type should be inferred
 ***** Returns *****
 inferred type
@@ -3452,65 +3444,62 @@
 parser.infer("true")  # bool
 parser.infer("2.0")   # float
 parser.infer("abc")   # str
 ⁰
 def infer_series(
 self,
 values: Iterable[str]) -> Type[Union[str, int, float, decimal.Decimal, bool,
-NoneType, parsetypes._common.Nullable[str], parsetypes._common.Nullable[int],
-parsetypes._common.Nullable[float], parsetypes._common.Nullable
-[decimal.Decimal], parsetypes._common.Nullable[bool],
-parsetypes._common.Nullable[NoneType]]]: View Source
-761
+NoneType, Nullable, list]]: View Source
+760
 def infer_series(self, values: Iterable[str]) -> AnyValueType:
-762
+761
 """
-763
+762
 Infer the underlying common type of a series of strings
+763
 764
-765
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
+765
 766
-767
 Parameters
-768
+767
 ----------
-769
+768
 `values`
-770
+769
 : series of strings for which the type should be inferred
+770
 771
-772
 Returns
-773
+772
 -------
-774
+773
 inferred type
+774
 775
-776
 Examples
-777
+776
 --------
-778
+777
 ```python
-779
+778
 parser = TypeParser()
-780
+779
 parser.infer_series(["1", "2", "3.4"])       # float
-781
+780
 parser.infer_series(["true", "false", "2"])  # int
-782
+781
 parser.infer_series(["1", "2.3", "abc"])     # str
-783
+782
 ```
-784
+783
 """
-785
+784
 return reduce_types(self.infer(value) for value in values)
 Infer the underlying common type of a series of strings
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See parsetypes.reduce_types() for more information.
 ***** Parameters *****
 values : series of strings for which the type should be inferred
@@ -3520,106 +3509,103 @@
 parser = TypeParser()
 parser.infer_series(["1", "2", "3.4"])       # float
 parser.infer_series(["true", "false", "2"])  # int
 parser.infer_series(["1", "2.3", "abc"])     # str
 ⁰
 def infer_table(
 self,
-rows: Iterable[Sequence[str]]) -> list[Type[Union[str, int, float,
-decimal.Decimal, bool, NoneType, parsetypes._common.Nullable[str],
-parsetypes._common.Nullable[int], parsetypes._common.Nullable[float],
-parsetypes._common.Nullable[decimal.Decimal], parsetypes._common.Nullable
-[bool], parsetypes._common.Nullable[NoneType]]]]: View Source
-788
+rows: Iterable[Sequence[str]]) -> list[typing.Type[typing.Union[str, int,
+float, decimal.Decimal, bool, NoneType, Nullable, list]]]: View Source
+787
 def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
-789
+788
 """
-790
+789
 Infer the underlying common type for each column of a table of strings
+790
 791
-792
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See `parsetypes.reduce_types()` for more information.
+792
 793
+Note that the individual inferred types of every value in the table must be
+able to fit into memory.
 794
-Note that the inferred types of every individual value must all be able to fit
-into memory at once.
 795
-796
 Parameters
-797
+796
 ----------
-798
+797
 `rows`
-799
+798
 : table of strings for which the types should be inferred, in row-major order
+799
 800
-801
 Returns
-802
+801
 -------
-803
+802
 inferred types
+803
 804
-805
 Examples
-806
+805
 --------
-807
+806
 ```python
-808
+807
 parser = TypeParser()
-809
+808
 parser.infer_table([
-810
+809
 ["1",   "true",  "1"],
-811
+810
 ["2",   "false", "2.3"],
-812
+811
 ["3.4", "2",     "abc"],
-813
+812
 ])
-814
+813
 # [float, int, str]
-815
+814
 ```
-816
+815
 """
-817
+816
 rows_iter = iter(rows)
-818
+817
 first_row = next(rows_iter, None)
-819
+818
 if first_row is None:
-820
+819
 return []
+820
 821
-822
 num_cols = len(first_row)
-823
+822
 if num_cols == 0:
-824
+823
 return []
+824
 825
-826
 table = _TypeTable([[self.infer(value)] for value in first_row])
-827
+826
 for row in rows_iter:
-828
+827
 table.add_row([self.infer(value) for value in row])
+828
 829
-830
 return [reduce_types(col) for col in table.cols]
 Infer the underlying common type for each column of a table of strings
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See parsetypes.reduce_types() for more information.
-Note that the inferred types of every individual value must all be able to fit
-into memory at once.
+Note that the individual inferred types of every value in the table must be
+able to fit into memory.
 ***** Parameters *****
 rows : table of strings for which the types should be inferred, in row-major
 order
 ***** Returns *****
 inferred types
 ***** Examples *****
 parser = TypeParser()
@@ -3628,131 +3614,125 @@
 	["2",   "false", "2.3"],
 	["3.4", "2",     "abc"],
 ])
 # [float, int, str]
 ⁰
 def parse(
 self,
-value: str) -> Union[str, int, float, decimal.Decimal, bool, NoneType,
-parsetypes._common.Nullable[str], parsetypes._common.Nullable[int],
-parsetypes._common.Nullable[float], parsetypes._common.Nullable
-[decimal.Decimal], parsetypes._common.Nullable[bool],
-parsetypes._common.Nullable[NoneType]]: View Source
-869
+value: str) -> Union[str, int, float, decimal.Decimal, bool, NoneType, list]:
+View Source
+868
 def parse(self, value: str) -> AnyValue:
-870
+869
 """
-871
+870
 Parse a string and convert it to its underlying type
+871
 872
-873
 Parameters
-874
+873
 ----------
-875
+874
 `value`
-876
+875
 : the string to be parsed
+876
 877
-878
 Returns
-879
+878
 -------
-880
+879
 converted value
+880
 881
-882
 Examples
-883
+882
 --------
-884
+883
 ```python
-885
+884
 parser = TypeParser()
-886
+885
 parser.parse("true")  # True
-887
+886
 parser.parse("2.0")   # 2.
-888
+887
 parser.parse("abc")   # "abc"
-889
+888
 ```
-890
+889
 """
-891
+890
 return self._convert(value, self.infer(value))
 Parse a string and convert it to its underlying type
 ***** Parameters *****
 value : the string to be parsed
 ***** Returns *****
 converted value
 ***** Examples *****
 parser = TypeParser()
 parser.parse("true")  # True
 parser.parse("2.0")   # 2.
 parser.parse("abc")   # "abc"
 ⁰
 def parse_series(
 self,
-values: Iterable[str]) -> list[Union[str, int, float, decimal.Decimal, bool,
-NoneType, parsetypes._common.Nullable[str], parsetypes._common.Nullable[int],
-parsetypes._common.Nullable[float], parsetypes._common.Nullable
-[decimal.Decimal], parsetypes._common.Nullable[bool],
-parsetypes._common.Nullable[NoneType]]]: View Source
-894
+values: Iterable[str]) -> list[typing.Union[str, int, float, decimal.Decimal,
+bool, NoneType, list]]: View Source
+893
 def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
-895
+894
 """
-896
+895
 Parse a series of strings and convert them to their underlying common type
+896
 897
-898
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
+898
 899
-900
 Parameters
-901
+900
 ----------
-902
+901
 `values`
-903
+902
 : series of strings to be parsed
+903
 904
-905
 Returns
-906
+905
 -------
-907
+906
 converted values
+907
 908
-909
 Examples
-910
+909
 --------
-911
+910
 ```python
-912
+911
 parser = TypeParser()
-913
+912
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
-914
+913
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-915
+914
 parser.parse_series(["true", "false", ""])  # [True, False, None]
-916
+915
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
-917
+916
 ```
-918
+917
 """
-919
+918
 inferred = self.infer_series(values)
-920
+919
 return [self._convert(value, inferred) for value in values]
 Parse a series of strings and convert them to their underlying common type
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See parsetypes.reduce_types() for more information.
 ***** Parameters *****
 values : series of strings to be parsed
@@ -3763,108 +3743,107 @@
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
 parser.parse_series(["true", "false", ""])  # [True, False, None]
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ⁰
 def parse_table(
 self,
-rows: Iterable[Sequence[str]]) -> list[list[Union[str, int, float,
-decimal.Decimal, bool, NoneType, parsetypes._common.Nullable[str],
-parsetypes._common.Nullable[int], parsetypes._common.Nullable[float],
-parsetypes._common.Nullable[decimal.Decimal], parsetypes._common.Nullable
-[bool], parsetypes._common.Nullable[NoneType]]]]: View Source
-923
+rows: Iterable[Sequence[str]]) -> list[list[typing.Union[str, int, float,
+decimal.Decimal, bool, NoneType, list]]]: View Source
+922
 def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
-924
+923
 """
-925
+924
 Parse a table of strings and convert them to the underlying common type of each
 column
+925
 926
-927
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
+927
 928
+Note that the type to which the values should be converted is determined by
+`infer_table()`, and so the individual inferred types of every value in the
+table must be able to fit into memory.
 929
-Note that the type inference requires that the inferred types of every
-individual value must all be able to fit into memory at once.
 930
-931
 This is a function that computes the entire table and returns it all at once.
 The generator `iterate_table()` behaves analogously, except that it computes
 and yields each row one at a time.
+931
 932
-933
 Parameters
-934
+933
 ----------
-935
+934
 `rows`
-936
+935
 : table of strings to be parsed, in row-major order
+936
 937
-938
 `iterator`
-939
+938
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
+939
 940
-941
 Returns
-942
+941
 -------
-943
+942
 converted table of values, in row-major order
+943
 944
-945
 Examples
-946
+945
 --------
-947
+946
 ```python
-948
+947
 parser = TypeParser()
-949
+948
 table = parser.parse_table([
-950
+949
 ["1", "5",   "true",  "1"],
-951
+950
 ["2", "6.7", "false", "2.3"],
-952
+951
 ["3", "8.0", "",      "abc"],
-953
+952
 ]):
-954
+953
 assert table == [
-955
+954
 [1, 5.,  True,  "1"],
-956
+955
 [2, 6.7, False, "2.3"],
-957
+956
 [3, 8.,  None,  "abc"],
-958
+957
 ]
-959
+958
 ```
-960
+959
 """
-961
+960
 return [converted_row for converted_row in self.iterate_table(rows)]
 Parse a table of strings and convert them to the underlying common type of each
 column
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
-Note that the type inference requires that the inferred types of every
-individual value must all be able to fit into memory at once.
+Note that the type to which the values should be converted is determined by
+infer_table(), and so the individual inferred types of every value in the table
+must be able to fit into memory.
 This is a function that computes the entire table and returns it all at once.
 The generator iterate_table() behaves analogously, except that it computes and
 yields each row one at a time.
 ***** Parameters *****
 rows : table of strings to be parsed, in row-major order
 iterator : whether the parsed values should be yielded as an iterator. If
 False, which is the default, the entire table is computed and returned as a
@@ -3886,101 +3865,100 @@
 	[2, 6.7, False, "2.3"],
 	[3, 8.,  None,  "abc"],
 ]
 ⁰
 def iterate_table(
 self,
 rows: Iterable[Sequence[str]]) -> Iterator[list[Union[str, int, float,
-decimal.Decimal, bool, NoneType, parsetypes._common.Nullable[str],
-parsetypes._common.Nullable[int], parsetypes._common.Nullable[float],
-parsetypes._common.Nullable[decimal.Decimal], parsetypes._common.Nullable
-[bool], parsetypes._common.Nullable[NoneType]]]]: View Source
-964
+decimal.Decimal, bool, NoneType, list]]]: View Source
+963
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-965
+964
 """
-966
+965
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
+966
 967
-968
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
+968
 969
-970
 This is a generator that computes and yields each row one at a time. The
 function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists. However, note that although
-this is a generator, the type inference still requires that the inferred types
-of every individual value must all be able to fit into memory at once.
+this is a generator, the type to which the value sshould be converted is still
+determined by `infer_table()`, and so the individual inferred types of every
+value in the table must be able to fit into memory.
+970
 971
-972
 Parameters
-973
+972
 ----------
-974
+973
 `rows`
-975
+974
 : table of strings to be parsed, in row-major order
+975
 976
-977
 Yields
-978
+977
 -------
-979
+978
 each row of converted table values
+979
 980
-981
 Examples
-982
+981
 --------
-983
+982
 ```python
-984
+983
 parser = TypeParser()
-985
+984
 table = parser.iterate_table([
-986
+985
 ["1",   "true",  "1"],
-987
+986
 ["2",   "false", "2.3"],
-988
+987
 ["3.4", "2",     "abc"],
-989
+988
 ]):
-990
+989
 assert next(table) == [1.,  1, "1"]
-991
+990
 assert next(table) == [2.,  0, "2.3"]
-992
+991
 assert next(table) == [3.4, 2, "abc"]
-993
+992
 ```
-994
+993
 """
-995
+994
 inferred_types = self.infer_table(rows)
+995
 996
-997
 for row in rows:
-998
+997
 yield [self._convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
 This is a generator that computes and yields each row one at a time. The
 function parse_table() behaves analogously, except that it computes the entire
 table and returns it as a list of lists. However, note that although this is a
-generator, the type inference still requires that the inferred types of every
-individual value must all be able to fit into memory at once.
+generator, the type to which the value sshould be converted is still determined
+by infer_table(), and so the individual inferred types of every value in the
+table must be able to fit into memory.
 ***** Parameters *****
 rows : table of strings to be parsed, in row-major order
 ***** Yields *****
 each row of converted table values
 ***** Examples *****
 parser = TypeParser()
 table = parser.iterate_table([
@@ -3991,95 +3969,89 @@
 assert next(table) == [1.,  1, "1"]
 assert next(table) == [2.,  0, "2.3"]
 assert next(table) == [3.4, 2, "abc"]
 ** Inherited Members **
   ⁰
 def reduce_types(
 types: Iterable[Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
-parsetypes._common.Nullable[str], parsetypes._common.Nullable[int],
-parsetypes._common.Nullable[float], parsetypes._common.Nullable
-[decimal.Decimal], parsetypes._common.Nullable[bool],
-parsetypes._common.Nullable[NoneType]]]]) -> Type[Union[str, int, float,
-decimal.Decimal, bool, NoneType, parsetypes._common.Nullable[str],
-parsetypes._common.Nullable[int], parsetypes._common.Nullable[float],
-parsetypes._common.Nullable[decimal.Decimal], parsetypes._common.Nullable
-[bool], parsetypes._common.Nullable[NoneType]]]: View Source
-157def reduce_types(types: Iterable[AnyValueType]) -> AnyValueType:
-158
+Nullable, list]]]) -> Type[Union[str, int, float, decimal.Decimal, bool,
+NoneType, Nullable, list]]: View Source
+156def reduce_types(types: Iterable[AnyValueType]) -> AnyValueType:
+157
 """
-159
+158
 Reduce multiple types into a single common type.
+159
 160
-161
 If the input types are not all the same, the resulting type will be narrowest
 possible type that will encompass all of the input types.
+161
 162
-163
 This operation is useful in cases such as parsing a CSV file where each column
 should have a consistent type, but where the individual values in a column
 could be interpreted variously as ints or floats (or other types).
+163
 164
-165
 Parameters
-166
+165
 ----------
-167
+166
 `types`
-168
+167
 : types to be reduced
+168
 169
-170
 Returns
-171
+170
 -------
-172
+171
 common reduced type
+172
 173
-174
 Examples
-175
+174
 --------
-176
+175
 ```python
-177
+176
 reduce_types([int, float])        # float
-178
+177
 reduce_types([bool, int])         # int
-179
+178
 reduce_types([int, float, str])   # str
-180
+179
 ```
-181
+180
 """
-182
+181
 reduced_type: Union[AnyValueType, None] = None
-183
+182
 for t in types:
-184
+183
 if reduced_type is None:
-185
+184
 reduced_type = t
-186
+185
 elif t != reduced_type:
-187
+186
 reduced_type = _merge_types(reduced_type, t)
-188
+187
 if reduced_type == _TerminalValue:
-189
+188
 return _TerminalValue
+189
 190
-191
 if reduced_type is None:
-192
+191
 # types is empty
-193
+192
 return GenericValue
-194
+193
 else:
-195
+194
 return reduced_type
 Reduce multiple types into a single common type.
 If the input types are not all the same, the resulting type will be narrowest
 possible type that will encompass all of the input types.
 This operation is useful in cases such as parsing a CSV file where each column
 should have a consistent type, but where the individual values in a column
 could be interpreted variously as ints or floats (or other types).
```

### Comparing `parsetypes-0.2.1/docs/html/search.js` & `parsetypes-0.2.2/docs/html/search.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -728,24 +728,24 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_int": {
                     "fullname": "parsetypes.TypeParser.is_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_int",
                     "kind": "function",
-                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_negative</code>\n: whether to accept negative values</p>\n\n<p><code>allow_sign</code>\n: whether to accept signed values. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;\"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> <em>must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_negative</code>\n: whether to accept negative values</p>\n\n<p><code>allow_sign</code>\n: whether to accept signed values. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_sign</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_negative</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_float": {
                     "fullname": "parsetypes.TypeParser.is_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_float",
                     "kind": "function",
-                    "doc": "<p>Check if a string represents a float (or equivalently, a Decimal)</p>\n\n<p>This function will also return True if the string represents an int.</p>\n\n<p>Alias: <code>is_decimal()</code></p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;\"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is a float or Decimal</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;12.3e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>         <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Check if a string represents a float (or equivalently, a Decimal)</p>\n\n<p>This function will also return True if the string represents an int.</p>\n\n<p>Alias: <code>is_decimal()</code></p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is a float or Decimal</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;12.3e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>         <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_inf</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_nan</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_decimal": {
                     "fullname": "parsetypes.TypeParser.is_decimal",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_decimal",
@@ -773,106 +773,106 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_int": {
                     "fullname": "parsetypes.TypeParser.parse_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_int",
                     "kind": "function",
-                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;\"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> <em>must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"o\">*</span>, </span><span class=\"param\"><span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "fullname": "parsetypes.TypeParser.parse_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_float",
                     "kind": "function",
-                    "doc": "<p>Parse a string and return it as a (non-exact) float if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1.</code> for True and <code>0.</code> for False. If the string represents an int, it will be converted to a float also.</p>\n\n<p>Behaves analogously to <code>parse_decimal()</code>, except that that returns an exact Decimal instead.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;\"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed float value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">(</span><span class=\"n\">inf_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">],</span> <span class=\"n\">nan_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;nan&quot;</span><span class=\"p\">])</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># 1.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e2&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># 123.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 0.0123</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># math.inf</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Parse a string and return it as a (non-exact) float if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1.</code> for True and <code>0.</code> for False. If the string represents an int, it will be converted to a float also.</p>\n\n<p>Behaves analogously to <code>parse_decimal()</code>, except that that returns an exact Decimal instead.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed float value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">(</span><span class=\"n\">inf_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">],</span> <span class=\"n\">nan_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;nan&quot;</span><span class=\"p\">])</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># 1.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e2&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># 123.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 0.0123</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_float</span><span class=\"p\">(</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># math.inf</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_inf</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_nan</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">float</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_decimal": {
                     "fullname": "parsetypes.TypeParser.parse_decimal",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_decimal",
                     "kind": "function",
-                    "doc": "<p>Parse a string and return it as an exact Decimal if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>Decimal(1)</code> for True and <code>Decimal(0)</code> for False. If the string represents an int, it will be converted to a Decimal also.</p>\n\n<p>Behaves analogously to <code>parse_float()</code>, except that that returns a non-exact float instead.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;\"</code> will be interpreted as the expression <code>&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed Decimal value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">(</span><span class=\"n\">inf_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">],</span> <span class=\"n\">nan_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;nan&quot;</span><span class=\"p\">])</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># Decimal(1)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e2&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># Decimal(123)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># Decimal(123) / Decimal(10000)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># Decimal(math.inf)</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Parse a string and return it as an exact Decimal if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>Decimal(1)</code> for True and <code>Decimal(0)</code> for False. If the string represents an int, it will be converted to a Decimal also.</p>\n\n<p>Behaves analogously to <code>parse_float()</code>, except that that returns a non-exact float instead.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.</p>\n\n<p><code>allow_inf</code>\n: whether to accept positive and negative infinity values. If True, strings that match the values in <code>self.inf_values</code> (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<p><code>allow_nan</code>\n: whether to accept NaN (not a number) representations. If True, strings that match the values in <code>self.nan_values</code> (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on <code>self.float_case_sensitive</code>, which is False by default.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed Decimal value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">(</span><span class=\"n\">inf_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">],</span> <span class=\"n\">nan_values</span><span class=\"o\">=</span><span class=\"p\">[</span><span class=\"s2\">&quot;nan&quot;</span><span class=\"p\">])</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.&quot;</span><span class=\"p\">)</span>       <span class=\"c1\"># Decimal(1)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e2&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># Decimal(123)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;1.23e-2&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># Decimal(123) / Decimal(10000)</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_decimal</span><span class=\"p\">(</span><span class=\"s2\">&quot;inf&quot;</span><span class=\"p\">)</span>      <span class=\"c1\"># Decimal(math.inf)</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_inf</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_nan</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.infer": {
                     "fullname": "parsetypes.TypeParser.infer",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.infer",
                     "kind": "function",
                     "doc": "<p>Infer the underlying type of a string</p>\n\n<p>Also check for inline lists if <code>self.list_delimiter</code> is not None.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: the string for which the type should be inferred</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>inferred type</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer</span><span class=\"p\">(</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># bool</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer</span><span class=\"p\">(</span><span class=\"s2\">&quot;2.0&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># float</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># str</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]</span>:</span></span>",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.infer_series": {
                     "fullname": "parsetypes.TypeParser.infer_series",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.infer_series",
                     "kind": "function",
                     "doc": "<p>Infer the underlying common type of a series of strings</p>\n\n<p>If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>values</code>\n: series of strings for which the type should be inferred</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>inferred type</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">])</span>       <span class=\"c1\"># float</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">])</span>  <span class=\"c1\"># int</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">])</span>     <span class=\"c1\"># str</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]</span>:</span></span>",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.infer_table": {
                     "fullname": "parsetypes.TypeParser.infer_table",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.infer_table",
                     "kind": "function",
-                    "doc": "<p>Infer the underlying common type for each column of a table of strings</p>\n\n<p>For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>Note that the inferred types of every individual value must all be able to fit into memory at once.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings for which the types should be inferred, in row-major order</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>inferred types</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>     <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">])</span>\n<span class=\"c1\"># [float, int, str]</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]]</span>:</span></span>",
+                    "doc": "<p>Infer the underlying common type for each column of a table of strings</p>\n\n<p>For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>Note that the individual inferred types of every value in the table must be able to fit into memory.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings for which the types should be inferred, in row-major order</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>inferred types</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>     <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">])</span>\n<span class=\"c1\"># [float, int, str]</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse": {
                     "fullname": "parsetypes.TypeParser.parse",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse",
                     "kind": "function",
                     "doc": "<p>Parse a string and convert it to its underlying type</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: the string to be parsed</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted value</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;2.0&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># 2.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># &quot;abc&quot;</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]</span>:</span></span>",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_series": {
                     "fullname": "parsetypes.TypeParser.parse_series",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_series",
                     "kind": "function",
                     "doc": "<p>Parse a series of strings and convert them to their underlying common type</p>\n\n<p>If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>values</code>\n: series of strings to be parsed</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted values</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;3&quot;</span><span class=\"p\">])</span>        <span class=\"c1\"># [1, 2, 3]</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;5&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;6.7&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;8.&quot;</span><span class=\"p\">])</span>     <span class=\"c1\"># [5., 6.7, 8.]</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;&quot;</span><span class=\"p\">])</span>  <span class=\"c1\"># [True, False, None]</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_series</span><span class=\"p\">([</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">])</span>    <span class=\"c1\"># [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]</span>:</span></span>",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_table": {
                     "fullname": "parsetypes.TypeParser.parse_table",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_table",
                     "kind": "function",
-                    "doc": "<p>Parse a table of strings and convert them to the underlying common type of each column</p>\n\n<p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>Note that the type inference requires that the inferred types of every individual value must all be able to fit into memory at once.</p>\n\n<p>This is a function that computes the entire table and returns it all at once. The generator <code>iterate_table()</code> behaves analogously, except that it computes and yields each row one at a time.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings to be parsed, in row-major order</p>\n\n<p><code>iterator</code>\n: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted table of values, in row-major order</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">table</span> <span class=\"o\">=</span> <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;5&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;6.7&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;8.0&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;&quot;</span><span class=\"p\">,</span>      <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]):</span>\n<span class=\"k\">assert</span> <span class=\"n\">table</span> <span class=\"o\">==</span> <span class=\"p\">[</span>\n        <span class=\"p\">[</span><span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"mf\">5.</span><span class=\"p\">,</span>  <span class=\"kc\">True</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"mi\">2</span><span class=\"p\">,</span> <span class=\"mf\">6.7</span><span class=\"p\">,</span> <span class=\"kc\">False</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"mi\">3</span><span class=\"p\">,</span> <span class=\"mf\">8.</span><span class=\"p\">,</span>  <span class=\"kc\">None</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]]</span>:</span></span>",
+                    "doc": "<p>Parse a table of strings and convert them to the underlying common type of each column</p>\n\n<p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>Note that the type to which the values should be converted is determined by <code>infer_table()</code>, and so the individual inferred types of every value in the table must be able to fit into memory.</p>\n\n<p>This is a function that computes the entire table and returns it all at once. The generator <code>iterate_table()</code> behaves analogously, except that it computes and yields each row one at a time.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings to be parsed, in row-major order</p>\n\n<p><code>iterator</code>\n: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted table of values, in row-major order</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">table</span> <span class=\"o\">=</span> <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;5&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;6.7&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;8.0&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;&quot;</span><span class=\"p\">,</span>      <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]):</span>\n<span class=\"k\">assert</span> <span class=\"n\">table</span> <span class=\"o\">==</span> <span class=\"p\">[</span>\n        <span class=\"p\">[</span><span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"mf\">5.</span><span class=\"p\">,</span>  <span class=\"kc\">True</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"mi\">2</span><span class=\"p\">,</span> <span class=\"mf\">6.7</span><span class=\"p\">,</span> <span class=\"kc\">False</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"mi\">3</span><span class=\"p\">,</span> <span class=\"mf\">8.</span><span class=\"p\">,</span>  <span class=\"kc\">None</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.iterate_table": {
                     "fullname": "parsetypes.TypeParser.iterate_table",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.iterate_table",
                     "kind": "function",
-                    "doc": "<p>Parse a table of strings for the underlying common type of each column, then convert and yield each row</p>\n\n<p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>This is a generator that computes and yields each row one at a time. The function <code>parse_table()</code> behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type inference still requires that the inferred types of every individual value must all be able to fit into memory at once.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings to be parsed, in row-major order</p>\n\n<h2 id=\"yields\">Yields</h2>\n\n<p>each row of converted table values</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">table</span> <span class=\"o\">=</span> <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">iterate_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>     <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]):</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">1.</span><span class=\"p\">,</span>  <span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">]</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">2.</span><span class=\"p\">,</span>  <span class=\"mi\">0</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">]</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">3.4</span><span class=\"p\">,</span> <span class=\"mi\">2</span><span class=\"p\">,</span> <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">]</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Iterator</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]]</span>:</span></span>",
+                    "doc": "<p>Parse a table of strings for the underlying common type of each column, then convert and yield each row</p>\n\n<p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>This is a generator that computes and yields each row one at a time. The function <code>parse_table()</code> behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by <code>infer_table()</code>, and so the individual inferred types of every value in the table must be able to fit into memory.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings to be parsed, in row-major order</p>\n\n<h2 id=\"yields\">Yields</h2>\n\n<p>each row of converted table values</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">table</span> <span class=\"o\">=</span> <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">iterate_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>     <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">]):</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">1.</span><span class=\"p\">,</span>  <span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">]</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">2.</span><span class=\"p\">,</span>  <span class=\"mi\">0</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">]</span>\n<span class=\"k\">assert</span> <span class=\"nb\">next</span><span class=\"p\">(</span><span class=\"n\">table</span><span class=\"p\">)</span> <span class=\"o\">==</span> <span class=\"p\">[</span><span class=\"mf\">3.4</span><span class=\"p\">,</span> <span class=\"mi\">2</span><span class=\"p\">,</span> <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">]</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Iterator</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.reduce_types": {
                     "fullname": "parsetypes.reduce_types",
                     "modulename": "parsetypes",
                     "qualname": "reduce_types",
                     "kind": "function",
                     "doc": "<p>Reduce multiple types into a single common type.</p>\n\n<p>If the input types are not all the same, the resulting type will be narrowest possible type that will encompass all of the input types.</p>\n\n<p>This operation is useful in cases such as parsing a CSV file where each column should have a consistent type, but where the individual values in a column could be interpreted variously as ints or floats (or other types).</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>types</code>\n: types to be reduced</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>common reduced type</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">])</span>        <span class=\"c1\"># float</span>\n<span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">])</span>         <span class=\"c1\"># int</span>\n<span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">])</span>   <span class=\"c1\"># str</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">types</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">float</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">],</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">[</span><span class=\"n\">NoneType</span><span class=\"p\">]]]</span>:</span></span>",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">types</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
                 }
             },
             "docInfo": {
                 "parsetypes": {
                     "qualname": 0,
                     "fullname": 1,
@@ -921,24 +921,24 @@
                 "parsetypes.TypeParser.is_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
                     "bases": 0,
-                    "doc": 308
+                    "doc": 289
                 },
                 "parsetypes.TypeParser.is_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
                     "bases": 0,
-                    "doc": 402
+                    "doc": 383
                 },
                 "parsetypes.TypeParser.is_decimal": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
@@ -966,103 +966,103 @@
                 "parsetypes.TypeParser.parse_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 47,
                     "bases": 0,
-                    "doc": 289
+                    "doc": 270
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
                     "bases": 0,
-                    "doc": 492
+                    "doc": 473
                 },
                 "parsetypes.TypeParser.parse_decimal": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 94,
                     "bases": 0,
-                    "doc": 502
+                    "doc": 483
                 },
                 "parsetypes.TypeParser.infer": {
                     "qualname": 2,
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 202,
+                    "signature": 94,
                     "bases": 0,
                     "doc": 151
                 },
                 "parsetypes.TypeParser.infer_series": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 208,
+                    "signature": 100,
                     "bases": 0,
                     "doc": 244
                 },
                 "parsetypes.TypeParser.infer_table": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 226,
+                    "signature": 118,
                     "bases": 0,
                     "doc": 256
                 },
                 "parsetypes.TypeParser.parse": {
                     "qualname": 2,
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 198,
+                    "signature": 73,
                     "bases": 0,
                     "doc": 137
                 },
                 "parsetypes.TypeParser.parse_series": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 213,
+                    "signature": 88,
                     "bases": 0,
                     "doc": 308
                 },
                 "parsetypes.TypeParser.parse_table": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 221,
+                    "signature": 96,
                     "bases": 0,
-                    "doc": 534
+                    "doc": 548
                 },
                 "parsetypes.TypeParser.iterate_table": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 216,
+                    "signature": 91,
                     "bases": 0,
-                    "doc": 442
+                    "doc": 456
                 },
                 "parsetypes.reduce_types": {
                     "qualname": 2,
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 376,
+                    "signature": 160,
                     "bases": 0,
                     "doc": 188
                 }
             },
             "length": 21,
             "save": true
         },
@@ -2118,36 +2118,36 @@
                         "parsetypes.TypeParser.parse_float": {
                             "tf": 8.54400374531753
                         },
                         "parsetypes.TypeParser.parse_decimal": {
                             "tf": 8.774964387392123
                         },
                         "parsetypes.TypeParser.infer": {
-                            "tf": 12.84523257866513
+                            "tf": 8.831760866327848
                         },
                         "parsetypes.TypeParser.infer_series": {
-                            "tf": 13.038404810405298
+                            "tf": 9.1104335791443
                         },
                         "parsetypes.TypeParser.infer_table": {
-                            "tf": 13.564659966250536
+                            "tf": 9.848857801796104
                         },
                         "parsetypes.TypeParser.parse": {
-                            "tf": 12.727922061357855
+                            "tf": 7.810249675906654
                         },
                         "parsetypes.TypeParser.parse_series": {
-                            "tf": 13.19090595827292
+                            "tf": 8.54400374531753
                         },
                         "parsetypes.TypeParser.parse_table": {
-                            "tf": 13.416407864998739
+                            "tf": 8.888194417315589
                         },
                         "parsetypes.TypeParser.iterate_table": {
-                            "tf": 13.2664991614216
+                            "tf": 8.660254037844387
                         },
                         "parsetypes.reduce_types": {
-                            "tf": 17.4928556845359
+                            "tf": 11.489125293076057
                         }
                     },
                     "df": 19,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "r": {
@@ -2290,36 +2290,36 @@
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.infer": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_series": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_table": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1
                                         },
                                         "parsetypes.reduce_types": {
-                                            "tf": 2
+                                            "tf": 1.4142135623730951
                                         }
                                     },
                                     "df": 18
                                 }
                             }
                         }
                     },
@@ -2403,36 +2403,36 @@
                                                     "parsetypes.TypeParser.__init__": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_decimal": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.infer": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.infer_series": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.infer_table": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_series": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_table": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.iterate_table": {
-                                                        "tf": 2
+                                                        "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.reduce_types": {
-                                                        "tf": 2.8284271247461903
+                                                        "tf": 2
                                                     }
                                                 },
                                                 "df": 10
                                             }
                                         }
                                     }
                                 }
@@ -2508,36 +2508,36 @@
                                             "parsetypes.TypeParser.__init__": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_series": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_series": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_table": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
-                                                "tf": 1.4142135623730951
+                                                "tf": 1
                                             },
                                             "parsetypes.reduce_types": {
-                                                "tf": 2
+                                                "tf": 1.4142135623730951
                                             }
                                         },
                                         "df": 10
                                     }
                                 }
                             }
                         }
@@ -2552,28 +2552,40 @@
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.infer": {
+                                            "tf": 1
+                                        },
+                                        "parsetypes.TypeParser.infer_series": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.infer_table": {
+                                            "tf": 1.4142135623730951
+                                        },
+                                        "parsetypes.TypeParser.parse": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_table": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
+                                        },
+                                        "parsetypes.reduce_types": {
+                                            "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 5
+                                    "df": 9
                                 }
                             }
                         }
                     },
                     "o": {
                         "docs": {},
                         "df": 0,
@@ -2648,36 +2660,36 @@
                                     "parsetypes.TypeParser.parse_float": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_decimal": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.infer_series": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.infer_table": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_series": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_table": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 1.4142135623730951
                                     },
                                     "parsetypes.reduce_types": {
-                                        "tf": 2
+                                        "tf": 1.4142135623730951
                                     }
                                 },
                                 "df": 19
                             }
                         },
                         "e": {
                             "docs": {},
@@ -2908,36 +2920,36 @@
                                             "df": 0,
                                             "p": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.infer": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_series": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_table": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.iterate_table": {
-                                                            "tf": 1.4142135623730951
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.reduce_types": {
-                                                            "tf": 2
+                                                            "tf": 1.4142135623730951
                                                         }
                                                     },
                                                     "df": 8
                                                 }
                                             }
                                         }
                                     }
@@ -3017,39 +3029,27 @@
                                             "df": 0,
                                             "l": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.infer": {
-                                                            "tf": 2.449489742783178
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
-                                                            "tf": 2.449489742783178
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
-                                                            "tf": 2.449489742783178
-                                                        },
-                                                        "parsetypes.TypeParser.parse": {
-                                                            "tf": 2.449489742783178
-                                                        },
-                                                        "parsetypes.TypeParser.parse_series": {
-                                                            "tf": 2.449489742783178
-                                                        },
-                                                        "parsetypes.TypeParser.parse_table": {
-                                                            "tf": 2.449489742783178
-                                                        },
-                                                        "parsetypes.TypeParser.iterate_table": {
-                                                            "tf": 2.449489742783178
+                                                            "tf": 1
                                                         },
                                                         "parsetypes.reduce_types": {
-                                                            "tf": 3.4641016151377544
+                                                            "tf": 1.4142135623730951
                                                         }
                                                     },
-                                                    "df": 8
+                                                    "df": 4
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
@@ -3202,36 +3202,36 @@
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_int": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_series": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_table": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
-                                        "tf": 2
+                                        "tf": 1.4142135623730951
                                     }
                                 },
                                 "df": 10
                             },
                             "f": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
@@ -3284,39 +3284,27 @@
                                     "df": 0,
                                     "o": {
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {
                                                 "parsetypes.TypeParser.infer": {
-                                                    "tf": 2.449489742783178
+                                                    "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
-                                                    "tf": 2.449489742783178
+                                                    "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
-                                                    "tf": 2.449489742783178
-                                                },
-                                                "parsetypes.TypeParser.parse": {
-                                                    "tf": 2.449489742783178
-                                                },
-                                                "parsetypes.TypeParser.parse_series": {
-                                                    "tf": 2.449489742783178
-                                                },
-                                                "parsetypes.TypeParser.parse_table": {
-                                                    "tf": 2.449489742783178
-                                                },
-                                                "parsetypes.TypeParser.iterate_table": {
-                                                    "tf": 2.449489742783178
+                                                    "tf": 1
                                                 },
                                                 "parsetypes.reduce_types": {
-                                                    "tf": 3.4641016151377544
+                                                    "tf": 1.4142135623730951
                                                 }
                                             },
-                                            "df": 8
+                                            "df": 4
                                         }
                                     }
                                 }
                             }
                         }
                     },
                     "a": {
@@ -3384,39 +3372,27 @@
                                                     "df": 0,
                                                     "e": {
                                                         "docs": {},
                                                         "df": 0,
                                                         "s": {
                                                             "docs": {
                                                                 "parsetypes.TypeParser.infer": {
-                                                                    "tf": 2.449489742783178
+                                                                    "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
-                                                                    "tf": 2.449489742783178
+                                                                    "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
-                                                                    "tf": 2.449489742783178
-                                                                },
-                                                                "parsetypes.TypeParser.parse": {
-                                                                    "tf": 2.449489742783178
-                                                                },
-                                                                "parsetypes.TypeParser.parse_series": {
-                                                                    "tf": 2.449489742783178
-                                                                },
-                                                                "parsetypes.TypeParser.parse_table": {
-                                                                    "tf": 2.449489742783178
-                                                                },
-                                                                "parsetypes.TypeParser.iterate_table": {
-                                                                    "tf": 2.449489742783178
+                                                                    "tf": 1
                                                                 },
                                                                 "parsetypes.reduce_types": {
-                                                                    "tf": 3.4641016151377544
+                                                                    "tf": 1.4142135623730951
                                                                 }
                                                             },
-                                                            "df": 8
+                                                            "df": 4
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -3782,36 +3758,36 @@
                         "parsetypes.TypeParser.is_none": {
                             "tf": 9.16515138991168
                         },
                         "parsetypes.TypeParser.is_bool": {
                             "tf": 10.392304845413264
                         },
                         "parsetypes.TypeParser.is_int": {
-                            "tf": 12.24744871391589
+                            "tf": 12.449899597988733
                         },
                         "parsetypes.TypeParser.is_float": {
-                            "tf": 12.649110640673518
+                            "tf": 12.84523257866513
                         },
                         "parsetypes.TypeParser.is_decimal": {
                             "tf": 2.23606797749979
                         },
                         "parsetypes.TypeParser.parse_none": {
                             "tf": 9.591663046625438
                         },
                         "parsetypes.TypeParser.parse_bool": {
                             "tf": 9.899494936611665
                         },
                         "parsetypes.TypeParser.parse_int": {
-                            "tf": 11.575836902790225
+                            "tf": 11.789826122551595
                         },
                         "parsetypes.TypeParser.parse_float": {
-                            "tf": 14.177446878757825
+                            "tf": 14.352700094407323
                         },
                         "parsetypes.TypeParser.parse_decimal": {
-                            "tf": 14.2828568570857
+                            "tf": 14.45683229480096
                         },
                         "parsetypes.TypeParser.infer": {
                             "tf": 9.797958971132712
                         },
                         "parsetypes.TypeParser.infer_series": {
                             "tf": 11.789826122551595
                         },
@@ -3821,18 +3797,18 @@
                         "parsetypes.TypeParser.parse": {
                             "tf": 9.643650760992955
                         },
                         "parsetypes.TypeParser.parse_series": {
                             "tf": 13.19090595827292
                         },
                         "parsetypes.TypeParser.parse_table": {
-                            "tf": 15.968719422671311
+                            "tf": 16.06237840420901
                         },
                         "parsetypes.TypeParser.iterate_table": {
-                            "tf": 15.427248620541512
+                            "tf": 15.524174696260024
                         },
                         "parsetypes.reduce_types": {
                             "tf": 9.433981132056603
                         }
                     },
                     "df": 21,
                     "t": {
@@ -3930,27 +3906,27 @@
                                     "parsetypes.TypeParser.infer": {
                                         "tf": 1.7320508075688772
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 2.6457513110645907
                                     },
                                     "parsetypes.TypeParser.infer_table": {
-                                        "tf": 2.6457513110645907
+                                        "tf": 2.8284271247461903
                                     },
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 2.449489742783178
                                     },
                                     "parsetypes.TypeParser.parse_table": {
-                                        "tf": 4
+                                        "tf": 4.242640687119285
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
-                                        "tf": 3.1622776601683795
+                                        "tf": 3.4641016151377544
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 2.23606797749979
                                     }
                                 },
                                 "df": 20,
                                 "i": {
@@ -4035,18 +4011,18 @@
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_table": {
-                                            "tf": 2.6457513110645907
+                                            "tf": 2.449489742783178
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
-                                            "tf": 2.23606797749979
+                                            "tf": 2
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
                                         }
                                     },
                                     "df": 16
                                 }
@@ -4096,18 +4072,18 @@
                                 "parsetypes.TypeParser.parse": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_table": {
-                                    "tf": 2.23606797749979
+                                    "tf": 2.449489742783178
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
                                 }
                             },
                             "df": 18,
                             "o": {
@@ -4415,21 +4391,21 @@
                                 "df": 0,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {
                                             "parsetypes.TypeParser.infer_table": {
-                                                "tf": 1.7320508075688772
+                                                "tf": 2
                                             },
                                             "parsetypes.TypeParser.parse_table": {
-                                                "tf": 3.1622776601683795
+                                                "tf": 3.4641016151377544
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
-                                                "tf": 3.1622776601683795
+                                                "tf": 3.4641016151377544
                                             }
                                         },
                                         "df": 3
                                     }
                                 }
                             },
                             "k": {
@@ -5709,15 +5685,15 @@
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_table": {
-                                                    "tf": 1
+                                                    "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
                                                 }
                                             },
                                             "df": 6
                                         }
@@ -5906,14 +5882,53 @@
                                             "tf": 1
                                         }
                                     },
                                     "df": 7
                                 }
                             }
                         },
+                        "o": {
+                            "docs": {
+                                "parsetypes.TypeParser.parse_table": {
+                                    "tf": 1
+                                },
+                                "parsetypes.TypeParser.iterate_table": {
+                                    "tf": 1
+                                }
+                            },
+                            "df": 2
+                        },
+                        "s": {
+                            "docs": {},
+                            "df": 0,
+                            "h": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "u": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "l": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "d": {
+                                                "docs": {
+                                                    "parsetypes.TypeParser.iterate_table": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        },
                         "u": {
                             "docs": {},
                             "df": 0,
                             "c": {
                                 "docs": {},
                                 "df": 0,
                                 "h": {
@@ -6040,14 +6055,45 @@
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
                                                 }
                                             },
                                             "df": 1
                                         }
+                                    },
+                                    "r": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "m": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "i": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "n": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "e": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "d": {
+                                                            "docs": {
+                                                                "parsetypes.TypeParser.parse_table": {
+                                                                    "tf": 1
+                                                                },
+                                                                "parsetypes.TypeParser.iterate_table": {
+                                                                    "tf": 1
+                                                                }
+                                                            },
+                                                            "df": 2
+                                                        }
+                                                    }
+                                                }
+                                            }
+                                        }
                                     }
                                 },
                                 "a": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
                                         "docs": {},
@@ -6622,21 +6668,18 @@
                                             "df": 0,
                                             "e": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "s": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.parse_table": {
-                                                            "tf": 1.4142135623730951
-                                                        },
-                                                        "parsetypes.TypeParser.iterate_table": {
                                                             "tf": 1
                                                         }
                                                     },
-                                                    "df": 2
+                                                    "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
@@ -6969,25 +7012,19 @@
                                 }
                             },
                             "c": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {
-                                        "parsetypes.TypeParser.infer_table": {
-                                            "tf": 1
-                                        },
                                         "parsetypes.TypeParser.parse_table": {
-                                            "tf": 1.7320508075688772
-                                        },
-                                        "parsetypes.TypeParser.iterate_table": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 3
+                                    "df": 1
                                 }
                             },
                             "e": {
                                 "docs": {
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 1.4142135623730951
                                     },
@@ -7279,18 +7316,18 @@
                                                             "parsetypes.TypeParser.parse": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_series": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_table": {
-                                                                "tf": 1
+                                                                "tf": 1.4142135623730951
                                                             },
                                                             "parsetypes.TypeParser.iterate_table": {
-                                                                "tf": 1
+                                                                "tf": 1.4142135623730951
                                                             }
                                                         },
                                                         "df": 7
                                                     }
                                                 }
                                             }
                                         }
@@ -7715,24 +7752,24 @@
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.infer_series": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.infer_table": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_table": {
-                                    "tf": 1.7320508075688772
+                                    "tf": 2
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.4142135623730951
                                 }
                             },
                             "df": 16,
                             "f": {
@@ -7769,17 +7806,23 @@
                                                 "tf": 2
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 2
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1.4142135623730951
+                                            },
+                                            "parsetypes.TypeParser.parse_table": {
+                                                "tf": 1
+                                            },
+                                            "parsetypes.TypeParser.iterate_table": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 5,
+                                        "df": 7,
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "n": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "c": {
@@ -7787,21 +7830,18 @@
                                                     "df": 0,
                                                     "e": {
                                                         "docs": {
                                                             "parsetypes": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_table": {
-                                                                "tf": 1.4142135623730951
-                                                            },
-                                                            "parsetypes.TypeParser.iterate_table": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 3
+                                                        "df": 2
                                                     }
                                                 }
                                             }
                                         },
                                         "r": {
                                             "docs": {},
                                             "df": 0,
@@ -8348,18 +8388,18 @@
                                 "parsetypes.TypeParser.infer": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_table": {
-                                    "tf": 2
+                                    "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
-                                    "tf": 1.7320508075688772
+                                    "tf": 2
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
                                 }
                             },
                             "df": 16
                         },
@@ -8758,18 +8798,18 @@
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
-                                        "tf": 2.449489742783178
+                                        "tf": 2.6457513110645907
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
-                                        "tf": 1.7320508075688772
+                                        "tf": 2
                                     }
                                 },
                                 "df": 15
                             },
                             "y": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
@@ -9096,25 +9136,22 @@
                                         }
                                     }
                                 }
                             }
                         },
                         "t": {
                             "docs": {
-                                "parsetypes.TypeParser.infer_table": {
-                                    "tf": 1
-                                },
                                 "parsetypes.TypeParser.parse_table": {
-                                    "tf": 2.23606797749979
+                                    "tf": 2
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1
                                 }
                             },
-                            "df": 3,
+                            "df": 2,
                             "t": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {},
                                     "df": 0,
                                     "m": {
@@ -9262,24 +9299,24 @@
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_table": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
-                                        "tf": 2
+                                        "tf": 1.7320508075688772
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1.4142135623730951
                                     }
                                 },
                                 "df": 7,
                                 "o": {
@@ -9510,18 +9547,18 @@
                                 "parsetypes.TypeParser.parse": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_table": {
-                                    "tf": 2
+                                    "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.7320508075688772
                                 }
                             },
                             "df": 20,
                             "h": {
@@ -9645,17 +9682,23 @@
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2.23606797749979
+                                },
+                                "parsetypes.TypeParser.parse_table": {
+                                    "tf": 1
+                                },
+                                "parsetypes.TypeParser.iterate_table": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 8
+                            "df": 10
                         },
                         "u": {
                             "docs": {},
                             "df": 0,
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_float": {
@@ -9919,18 +9962,21 @@
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_table": {
+                                                "tf": 1.4142135623730951
+                                            },
+                                            "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 12
+                                        "df": 13
                                     }
                                 }
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
@@ -10922,34 +10968,14 @@
                                             }
                                         },
                                         "df": 1
                                     }
                                 }
                             }
                         },
-                        "t": {
-                            "docs": {
-                                "parsetypes.TypeParser.is_int": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.is_float": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_int": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_float": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_decimal": {
-                                    "tf": 2.8284271247461903
-                                }
-                            },
-                            "df": 5
-                        },
                         "e": {
                             "docs": {},
                             "df": 0,
                             "n": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
@@ -11039,15 +11065,15 @@
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
-                                                "tf": 1
+                                                "tf": 1.4142135623730951
                                             }
                                         },
                                         "df": 15,
                                         "s": {
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
@@ -11085,15 +11111,15 @@
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.TypeParser.parse_series": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.parse_table": {
-                                                    "tf": 2
+                                                    "tf": 2.23606797749979
                                                 },
                                                 "parsetypes.TypeParser.iterate_table": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
                                                 }
@@ -11139,32 +11165,16 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             },
                             "r": {
-                                "docs": {
-                                    "parsetypes.TypeParser.is_int": {
-                                        "tf": 2.8284271247461903
-                                    },
-                                    "parsetypes.TypeParser.is_float": {
-                                        "tf": 2.8284271247461903
-                                    },
-                                    "parsetypes.TypeParser.parse_int": {
-                                        "tf": 2.8284271247461903
-                                    },
-                                    "parsetypes.TypeParser.parse_float": {
-                                        "tf": 2.8284271247461903
-                                    },
-                                    "parsetypes.TypeParser.parse_decimal": {
-                                        "tf": 2.8284271247461903
-                                    }
-                                },
-                                "df": 5,
+                                "docs": {},
+                                "df": 0,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "o": {
                                         "docs": {},
                                         "df": 0,
                                         "u": {
@@ -11267,34 +11277,14 @@
                                                 },
                                                 "df": 1
                                             }
                                         }
                                     }
                                 }
                             }
-                        },
-                        "t": {
-                            "docs": {
-                                "parsetypes.TypeParser.is_int": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.is_float": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_int": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_float": {
-                                    "tf": 2.8284271247461903
-                                },
-                                "parsetypes.TypeParser.parse_decimal": {
-                                    "tf": 2.8284271247461903
-                                }
-                            },
-                            "df": 5
                         }
                     },
                     "m": {
                         "docs": {
                             "parsetypes.TypeParser.is_int": {
                                 "tf": 2
                             },
```

### Comparing `parsetypes-0.2.1/pyproject.toml` & `parsetypes-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.1/src/parsetypes/__init__.py` & `parsetypes-0.2.2/src/parsetypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types')
```

### Comparing `parsetypes-0.2.1/src/parsetypes/_parser.py` & `parsetypes-0.2.2/src/parsetypes/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from decimal import Decimal
 from enum import Enum
 from typing import Callable, Iterable, Iterator, Optional, Sequence, TypeVar, cast
 
-from ._common import AnyContained, AnyContainedType, AnyValue, AnyValueType, GenericValue, Nullable
+from ._common import AnyValue, AnyValueType, GenericValue, Nullable
 from ._reduce_types import reduce_types, _decompose_type
 
 from ._compat import NoneType, Union
 
 
 _FloatLike = TypeVar('_FloatLike', float, Decimal)
 
@@ -302,15 +302,15 @@
 			`allow_negative`
 			: whether to accept negative values
 
 			`allow_sign`
 			: whether to accept signed values. If False, it implies that `allow_negative` is False also.
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form `"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
 
 			Returns
 			-------
 			whether it is an int
 
 			Examples
 			--------
@@ -371,15 +371,15 @@
 
 			Parameters
 			----------
 			`value`
 			: string to be checked
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form `"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
 
 			`allow_inf`
 			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
 			`allow_nan`
 			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
@@ -523,15 +523,15 @@
 
 			Parameters
 			----------
 			`value`
 			: string to be parsed
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form `"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
 
 			Returns
 			-------
 			parsed int value
 
 			Raises
 			------
@@ -622,15 +622,15 @@
 
 			Parameters
 			----------
 			`value`
 			: string to be parsed
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form `"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
 
 			`allow_inf`
 			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
 			`allow_nan`
 			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
@@ -669,15 +669,15 @@
 
 			Parameters
 			----------
 			`value`
 			: string to be parsed
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form `"<var>M</var>e<var>X</var>"` will be interpreted as the expression `<var>M</var> * (10 ** <var>X</var>)`, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var> must be an integer, but can be negative.
 
 			`allow_inf`
 			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
 			`allow_nan`
 			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.
 
@@ -746,17 +746,16 @@
 			value = value.strip()
 
 		if self.list_delimiter is not None and self.list_delimiter in value:
 			subvalues = value.split(self.list_delimiter)
 			if self.trim:
 				subvalues = [subvalue.strip() for subvalue in subvalues]
 			reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
-			reduced_type = cast(AnyContainedType, reduced_type)
 			r = list[reduced_type]
-			return r  # type: ignore
+			return r
 
 		return GenericValue
 
 
 	def infer_series(self, values: Iterable[str]) -> AnyValueType:
 		"""
 			Infer the underlying common type of a series of strings
@@ -786,15 +785,15 @@
 
 	def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
 		"""
 			Infer the underlying common type for each column of a table of strings
 
 			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.
 
-			Note that the inferred types of every individual value must all be able to fit into memory at once.
+			Note that the individual inferred types of every value in the table must be able to fit into memory.
 
 			Parameters
 			----------
 			`rows`
 			: table of strings for which the types should be inferred, in row-major order
 
 			Returns
@@ -854,15 +853,15 @@
 					return value
 		elif base == list:
 			subvalues = value.split(self.list_delimiter)
 			if self.trim:
 				subvalues = [subvalue.strip() for subvalue in subvalues]
 			if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 				subtype = type_args[0]
-				return cast(AnyContained, [self._convert(subvalue, subtype) for subvalue in subvalues])
+				return [self._convert(subvalue, subtype) for subvalue in subvalues]
 			else:
 				return subvalues
 		else:
 			return value
 
 
 	def parse(self, value: str) -> AnyValue:
@@ -921,15 +920,15 @@
 
 	def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
 		"""
 			Parse a table of strings and convert them to the underlying common type of each column
 
 			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.
 
-			Note that the type inference requires that the inferred types of every individual value must all be able to fit into memory at once.
+			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.
 
 			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.
 
 			Parameters
 			----------
 			`rows`
 			: table of strings to be parsed, in row-major order
@@ -962,15 +961,15 @@
 
 	def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list[AnyValue]]:
 		"""
 			Parse a table of strings for the underlying common type of each column, then convert and yield each row
 
 			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.
 
-			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type inference still requires that the inferred types of every individual value must all be able to fit into memory at once.
+			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.
 
 			Parameters
 			----------
 			`rows`
 			: table of strings to be parsed, in row-major order
 
 			Yields
```

### Comparing `parsetypes-0.2.1/src/parsetypes/_reduce_types.py` & `parsetypes-0.2.2/src/parsetypes/_reduce_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 from decimal import Decimal
 from typing import Iterable, Optional, cast
 
-from ._common import AnyBaseType, AnyContainedType, AnyContainerBaseType, AnyNullableType, AnyScalarType, AnyValueType, GenericValue, Nullable
+from ._common import AnyBaseType, AnyContainerBaseType, AnyScalarType, AnyValueType, GenericValue, Nullable
 
 from ._compat import Final, NoneType, Union
 
 
 _TerminalValue: 'Final[AnyBaseType]' = list
 
 _scalar_hierarchy: 'Final[dict[AnyBaseType, Union[AnyBaseType, None]]]' = {
@@ -39,15 +39,15 @@
 			return False
 		for arg in typing.get_args(t):
 			if not _is_valid_type(arg):
 				return False
 		return True
 
 
-def _decompose_type(t: AnyValueType) -> tuple[AnyBaseType, Union[tuple[AnyContainedType, ...], None]]:
+def _decompose_type(t: AnyValueType) -> tuple[AnyBaseType, Union[tuple[AnyValueType, ...], None]]:
 	base = typing.get_origin(t)
 	if base is None:
 		return t, None
 	else:
 		return base, typing.get_args(t)
 
 
@@ -61,37 +61,36 @@
 			return Nullable
 		else:
 			cue_base, cue_args = _decompose_type(cue)
 			if cue_base == Nullable:
 				if cue_args is not None and len(cue_args) == 1:
 					cue_arg = cast(AnyScalarType, cue_args[0])
 					r = Nullable[cue_arg]
-					return r  # type: ignore
+					return r
 				else:
 					return Nullable
 			elif cue_base == list:
 				return None
 			else:
 				cue_base = cast(AnyScalarType, cue_base)
 				r = Nullable[cue_base]
-				return r  # type: ignore
+				return r
 	elif base == Nullable:
 		if type_args is not None and len(type_args) == 1:
 			type_arg = cast(AnyScalarType, type_args[0])
 			r = list[type_arg]
-			return r  # type: ignore
+			return r
 		else:
 			if cue is None:
 				return list
 			else:
 				cue_base, cue_args = _decompose_type(cue)
 				if cue_base == Nullable:
-					cue = cast(AnyNullableType, cue)
 					r = list[cue]
-					return r  # type: ignore
+					return r
 				elif cue_base == list:
 					return None
 				else:
 					return list
 	elif base == list:
 		return None
 	else:
```

### Comparing `parsetypes-0.2.1/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.2.2/src/parsetypes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,15 +158,15 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
-### 0.2.1
+### 0.2.1 and 0.2.2
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.1/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.2.2/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.1/tests/test_parser.py` & `parsetypes-0.2.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.1/tests/test_reduce_types.py` & `parsetypes-0.2.2/tests/test_reduce_types.py`

 * *Files identical despite different names*

