# Comparing `tmp/docspec_python-2.2.0.tar.gz` & `tmp/docspec_python-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docspec_python-2.2.0.tar", max compression
+gzip compressed data, was "docspec_python-2.2.1.tar", max compression
```

## Comparing `docspec_python-2.2.0.tar` & `docspec_python-2.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1508 2023-05-28 03:58:32.067219 docspec_python-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      646 2023-05-13 09:55:38.864677 docspec_python-2.2.0/readme.md
--rw-r--r--   0        0        0     9887 2023-05-28 03:58:32.067219 docspec_python-2.2.0/src/docspec_python/__init__.py
--rw-r--r--   0        0        0     4082 2023-05-13 09:55:38.864677 docspec_python-2.2.0/src/docspec_python/__main__.py
--rw-r--r--   0        0        0    32980 2023-05-13 09:55:38.864677 docspec_python-2.2.0/src/docspec_python/parser.py
--rw-r--r--   0        0        0        0 2023-05-13 09:55:38.864677 docspec_python-2.2.0/src/docspec_python/py.typed
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 docspec_python-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1508 2023-05-28 11:24:05.979418 docspec_python-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      646 2023-05-13 09:55:38.864677 docspec_python-2.2.1/readme.md
+-rw-r--r--   0        0        0     9887 2023-05-28 11:24:05.979418 docspec_python-2.2.1/src/docspec_python/__init__.py
+-rw-r--r--   0        0        0     4082 2023-05-13 09:55:38.864677 docspec_python-2.2.1/src/docspec_python/__main__.py
+-rw-r--r--   0        0        0    32980 2023-05-13 09:55:38.864677 docspec_python-2.2.1/src/docspec_python/parser.py
+-rw-r--r--   0        0        0        0 2023-05-13 09:55:38.864677 docspec_python-2.2.1/src/docspec_python/py.typed
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 docspec_python-2.2.1/PKG-INFO
```

### Comparing `docspec_python-2.2.0/pyproject.toml` & `docspec_python-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "docspec-python"
-version = "2.2.0"
+version = "2.2.1"
 description = "A parser based on lib2to3 producing docspec data from Python source code."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/NiklasRosenstein/docspec/"
 packages = [{ include = "docspec_python", from="src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-docspec = "^2.2.0"
+docspec = "^2.2.1"
 "nr.util" = ">=0.7.0"
 black = "^23.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
```

### Comparing `docspec_python-2.2.0/readme.md` & `docspec_python-2.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `docspec_python-2.2.0/src/docspec_python/__init__.py` & `docspec_python-2.2.1/src/docspec_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __all__ = [
     "Parser",
     "ParserOptions",
     "load_python_modules",
     "parse_python_module",
     "find_module",
     "iter_package_files",
```

### Comparing `docspec_python-2.2.0/src/docspec_python/__main__.py` & `docspec_python-2.2.1/src/docspec_python/__main__.py`

 * *Files identical despite different names*

### Comparing `docspec_python-2.2.0/src/docspec_python/parser.py` & `docspec_python-2.2.1/src/docspec_python/parser.py`

 * *Files identical despite different names*

### Comparing `docspec_python-2.2.0/PKG-INFO` & `docspec_python-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: docspec-python
-Version: 2.2.0
+Version: 2.2.1
 Summary: A parser based on lib2to3 producing docspec data from Python source code.
 Home-page: https://github.com/NiklasRosenstein/docspec/
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0)
-Requires-Dist: docspec (>=2.2.0,<3.0.0)
+Requires-Dist: docspec (>=2.2.1,<3.0.0)
 Requires-Dist: nr.util (>=0.7.0)
 Description-Content-Type: text/markdown
 
   [docspec]: https://github.com/NiklasRosenstein/docspec
 
 # docspec-python
```

