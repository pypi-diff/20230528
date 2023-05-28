# Comparing `tmp/docspec-2.2.0.tar.gz` & `tmp/docspec-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docspec-2.2.0.tar", max compression
+gzip compressed data, was "docspec-2.2.1.tar", max compression
```

## Comparing `docspec-2.2.0.tar` & `docspec-2.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1466 2023-05-28 03:58:32.055219 docspec-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      629 2023-05-13 09:55:38.864677 docspec-2.2.0/readme.md
--rw-r--r--   0        0        0    21250 2023-05-28 03:58:32.067219 docspec-2.2.0/src/docspec/__init__.py
--rw-r--r--   0        0        0     2822 2023-05-13 09:55:38.864677 docspec-2.2.0/src/docspec/__main__.py
--rw-r--r--   0        0        0        0 2023-05-13 09:55:38.864677 docspec-2.2.0/src/docspec/py.typed
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 docspec-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1470 2023-05-28 11:24:05.975418 docspec-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-05-13 09:55:38.864677 docspec-2.2.1/readme.md
+-rw-r--r--   0        0        0    21250 2023-05-28 11:24:05.979418 docspec-2.2.1/src/docspec/__init__.py
+-rw-r--r--   0        0        0     2822 2023-05-13 09:55:38.864677 docspec-2.2.1/src/docspec/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-13 09:55:38.864677 docspec-2.2.1/src/docspec/py.typed
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 docspec-2.2.1/PKG-INFO
```

### Comparing `docspec-2.2.0/pyproject.toml` & `docspec-2.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "docspec"
-version = "2.2.0"
+version = "2.2.1"
 description = "Docspec is a JSON object specification for representing API documentation of programming languages."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/NiklasRosenstein/docspec/"
 packages = [{include="docspec", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-databind-core = "^4.2.6"
-databind-json = "^4.2.6"
+"databind.core" = "^4.2.6"
+"databind.json" = "^4.2.6"
 Deprecated = "^1.2.12"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
```

### Comparing `docspec-2.2.0/readme.md` & `docspec-2.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `docspec-2.2.0/src/docspec/__init__.py` & `docspec-2.2.1/src/docspec/__init__.py`

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
     "Location",
     "Decoration",
     "Docstring",
     "Argument",
     "ApiObject",
     "Indirection",
```

### Comparing `docspec-2.2.0/src/docspec/__main__.py` & `docspec-2.2.1/src/docspec/__main__.py`

 * *Files identical despite different names*

### Comparing `docspec-2.2.0/PKG-INFO` & `docspec-2.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: docspec
-Version: 2.2.0
+Version: 2.2.1
 Summary: Docspec is a JSON object specification for representing API documentation of programming languages.
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
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
-Requires-Dist: databind-core (>=4.2.6,<5.0.0)
-Requires-Dist: databind-json (>=4.2.6,<5.0.0)
+Requires-Dist: databind.core (>=4.2.6,<5.0.0)
+Requires-Dist: databind.json (>=4.2.6,<5.0.0)
 Description-Content-Type: text/markdown
 
 # docspec
 
 This Python packages provides
 
 * A library to (de-) serialize Docspec conformat JSON payloads
```

