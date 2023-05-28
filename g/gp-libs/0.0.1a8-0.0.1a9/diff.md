# Comparing `tmp/gp-libs-0.0.1a8.tar.gz` & `tmp/gp-libs-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp-libs-0.0.1a8.tar", max compression
+gzip compressed data, was "gp-libs-0.0.1a9.tar", max compression
```

## Comparing `gp-libs-0.0.1a8.tar` & `gp-libs-0.0.1a9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2022-09-05 23:33:50.706532 gp-libs-0.0.1a8/LICENSE
--rw-r--r--   0        0        0     4301 2022-09-05 23:33:50.706532 gp-libs-0.0.1a8/README.md
--rw-r--r--   0        0        0     2523 2022-09-05 23:33:50.710533 gp-libs-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0    18205 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/src/doctest_docutils.py
--rw-r--r--   0        0        0      462 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/src/gp_libs.py
--rw-r--r--   0        0        0     2472 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/src/linkify_issues.py
--rw-r--r--   0        0        0     6809 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/src/pytest_doctest_docutils.py
--rw-r--r--   0        0        0     8787 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/src/sphinx_toctree_autodoc_fix.py
--rw-r--r--   0        0        0        0 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/__init__.py
--rw-r--r--   0        0        0     1906 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/conftest.py
--rw-r--r--   0        0        0     3921 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/test_doctest_docutils.py
--rw-r--r--   0        0        0     1370 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/test_linkify_issues.py
--rw-r--r--   0        0        0     3423 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/test_pytest_doctest_docutils.py
--rw-r--r--   0        0        0     1747 2022-09-05 23:33:50.714532 gp-libs-0.0.1a8/tests/test_sphinx_toctree_autodoc_fix.py
--rw-r--r--   0        0        0     5343 2022-09-05 23:34:24.361292 gp-libs-0.0.1a8/setup.py
--rw-r--r--   0        0        0     5685 2022-09-05 23:34:24.361758 gp-libs-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-06 03:00:22.682798 gp-libs-0.0.1a9/LICENSE
+-rw-r--r--   0        0        0     4301 2022-09-06 03:00:22.682798 gp-libs-0.0.1a9/README.md
+-rw-r--r--   0        0        0     2523 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0    18205 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/src/doctest_docutils.py
+-rw-r--r--   0        0        0      462 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/src/gp_libs.py
+-rw-r--r--   0        0        0     2472 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/src/linkify_issues.py
+-rw-r--r--   0        0        0     7906 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/src/pytest_doctest_docutils.py
+-rw-r--r--   0        0        0     8787 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/src/sphinx_toctree_autodoc_fix.py
+-rw-r--r--   0        0        0        0 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/__init__.py
+-rw-r--r--   0        0        0     1906 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/conftest.py
+-rw-r--r--   0        0        0     3921 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/test_doctest_docutils.py
+-rw-r--r--   0        0        0     1370 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/test_linkify_issues.py
+-rw-r--r--   0        0        0     3938 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/test_pytest_doctest_docutils.py
+-rw-r--r--   0        0        0     1747 2022-09-06 03:00:22.686798 gp-libs-0.0.1a9/tests/test_sphinx_toctree_autodoc_fix.py
+-rw-r--r--   0        0        0     5343 2022-09-06 03:00:53.975917 gp-libs-0.0.1a9/setup.py
+-rw-r--r--   0        0        0     5685 2022-09-06 03:00:53.976372 gp-libs-0.0.1a9/PKG-INFO
```

### Comparing `gp-libs-0.0.1a8/LICENSE` & `gp-libs-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/README.md` & `gp-libs-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/pyproject.toml` & `gp-libs-0.0.1a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gp-libs"
-version = "0.0.1a8"
+version = "0.0.1a9"
 description = "Internal utilities for projects following git-pull python package spec"
 license = "MIT"
 authors = ["Tony Narlock <tony@git-pull.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
```

### Comparing `gp-libs-0.0.1a8/src/doctest_docutils.py` & `gp-libs-0.0.1a9/src/doctest_docutils.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/src/linkify_issues.py` & `gp-libs-0.0.1a9/src/linkify_issues.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/src/pytest_doctest_docutils.py` & `gp-libs-0.0.1a9/src/pytest_doctest_docutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,22 +26,41 @@
 from _pytest.outcomes import OutcomeException
 
 from doctest_docutils import DocutilsDocTestFinder, setup
 
 if TYPE_CHECKING:
     from doctest import _Out
 
+    from _pytest.config.argparsing import Parser
     from _pytest.doctest import DoctestItem
 
+
 logger = logging.getLogger(__name__)
 
 # Lazy definition of runner class
 RUNNER_CLASS = None
 
 
+def pytest_addoption(parser: "Parser") -> None:
+    group = parser.getgroup("collect")
+    group.addoption(
+        "--doctest-docutils-modules",
+        action="store_true",
+        default=False,
+        help="run doctest-doctests in .py modules (pass-through to pytest-doctest)",
+        dest="doctestmodules",
+    )
+    group.addoption(
+        "--no-doctest-docutils-modules",
+        action="store_false",
+        help="disable doctest-doctests in .py modules (pass-through to pytest-doctest)",
+        dest="doctestmodules",
+    )
+
+
 def pytest_configure(config: pytest.Config) -> None:
     """Disable pytest.doctest to prevent running tests twice.
 
     Todo: Find a way to make these plugins cooperate without collecting twice.
     """
     if config.pluginmanager.has_plugin("doctest"):
         config.pluginmanager.set_blocked("doctest")
@@ -51,17 +70,29 @@
     global RUNNER_CLASS
 
     RUNNER_CLASS = None
 
 
 def pytest_collect_file(
     file_path: Path, parent: pytest.Collector
-) -> Optional["DocTestDocutilsFile"]:
+) -> Optional[Tuple["DocTestDocutilsFile", "_pytest.doctest.DoctestModule"]]:
     config = parent.config
-    if _is_doctest(config, file_path, parent):
+    if file_path.suffix == ".py":
+        if config.option.doctestmodules and not any(
+            # if not any(
+            (
+                _pytest.doctest._is_setup_py(file_path),
+                _pytest.doctest._is_main_py(file_path),
+            )
+        ):
+            mod: Tuple[
+                "DocTestDocutilsFile", "_pytest.doctest.DoctestModule"
+            ] = _pytest.doctest.DoctestModule.from_parent(parent, path=file_path)
+            return mod
+    elif _is_doctest(config, file_path, parent):
         return DocTestDocutilsFile.from_parent(parent, path=file_path)  # type: ignore
     return None
 
 
 def _is_doctest(config: pytest.Config, path: Path, parent: pytest.Collector) -> bool:
     if path.suffix in (".rst", ".md") and parent.session.isinitpath(path):
         return True
```

### Comparing `gp-libs-0.0.1a8/src/sphinx_toctree_autodoc_fix.py` & `gp-libs-0.0.1a9/src/sphinx_toctree_autodoc_fix.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/tests/conftest.py` & `gp-libs-0.0.1a9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/tests/test_doctest_docutils.py` & `gp-libs-0.0.1a9/tests/test_doctest_docutils.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/tests/test_linkify_issues.py` & `gp-libs-0.0.1a9/tests/test_linkify_issues.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/tests/test_pytest_doctest_docutils.py` & `gp-libs-0.0.1a9/tests/test_pytest_doctest_docutils.py`

 * *Files 13% similar despite different names*

```diff
@@ -139,14 +139,35 @@
       8
 ```
         """
             )
         },
         tests_found=1,
     ),
+    #
+    # .py should still work
+    #
+    PytestDocTestFinderFixture(
+        test_id="python-reST-doctest_block",
+        files={
+            "example.py": textwrap.dedent(
+                """
+def hello(statement: str) -> None:
+    '''Say hello.
+
+    >>> hello(f'hello world {2 * 3}')
+    hello world 6
+    '''
+    print(statement)
+
+        """
+            )
+        },
+        tests_found=1,
+    ),
 ]
 
 
 @pytest.mark.parametrize(
     PytestDocTestFinderFixture._fields, FIXTURES, ids=[f.test_id for f in FIXTURES]
 )
 def test_pluginDocutilsDocTestFinder(
@@ -155,24 +176,33 @@
     monkeypatch: pytest.MonkeyPatch,
     test_id: str,
     files: FixtureFileDict,
     tests_found: int,
 ) -> None:
     # Initialize variables
     pytester.plugins = ["pytest_doctest_docutils"]
-    pytester.makefile(".ini", pytest="[pytest]\naddopts=-p no:doctest -vv\n")
+    pytester.makefile(
+        ".ini",
+        pytest=textwrap.dedent(
+            """
+[pytest]
+addopts=-p no:doctest -vv
+
+        """.strip()
+        ),
+    )
     tests_path = tmp_path / "tests"
     first_test_key = list(files.keys())[0]
     first_test_filename = str(tests_path / first_test_key)
 
     # Setup: Files
     tests_path.mkdir()
     for file_name, text in files.items():
         rst_file = tests_path / file_name
         rst_file.write_text(
             text,
             encoding="utf-8",
         )
 
     # Test
-    result = pytester.runpytest(str(first_test_filename))
+    result = pytester.runpytest(str(first_test_filename), "--doctest-docutils-modules")
     result.assert_outcomes(passed=tests_found)
```

### Comparing `gp-libs-0.0.1a8/tests/test_sphinx_toctree_autodoc_fix.py` & `gp-libs-0.0.1a9/tests/test_sphinx_toctree_autodoc_fix.py`

 * *Files identical despite different names*

### Comparing `gp-libs-0.0.1a8/setup.py` & `gp-libs-0.0.1a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['docutils>=0.18.0,<0.19.0', 'myst_parser']
 
 entry_points = \
 {'pytest11': ['sphinx = pytest_doctest_docutils']}
 
 setup_kwargs = {
     'name': 'gp-libs',
-    'version': '0.0.1a8',
+    'version': '0.0.1a9',
     'description': 'Internal utilities for projects following git-pull python package spec',
     'long_description': '# gp-libs &middot; [![Python Package](https://img.shields.io/pypi/v/gp-libs.svg)](https://pypi.org/project/gp-libs/) [![License](https://img.shields.io/github/license/git-pull/gp-libs.svg)](https://github.com/git-pull/gp-libs/blob/master/LICENSE) [![Code Coverage](https://codecov.io/gh/git-pull/gp-libs/branch/master/graph/badge.svg)](https://codecov.io/gh/git-pull/gp-libs)\n\nIncubating / [dogfooding] some sphinx extensions and pytest plugins on\ngit-pull projects, e.g. [cihai], [vcs-python], or [tmux-python].\n\n[dogfooding]: https://en.wikipedia.org/wiki/Eating_your_own_dog_food\n[cihai]: https://github.com/cihai\n[vcs-python]: https://github.com/vcs-python\n[tmux-python]: https://github.com/tmux-python\n\n## doctest helpers (for docutils)\n\nTwo parts:\n\n1. doctest module: Same specification as doctest, but can parse reStructuredText\n   and markdown\n2. pytest plugin: Collects pytest for reStructuredText and markdown files\n\n### doctest module\n\nThis extends standard library `doctest` to support anything docutils can parse.\nIt can parse reStructuredText (.rst) and markdown (.md).\n\nSee more: <https://gp-libs.git-pull.com/doctest/>\n\n#### Writing doctests\n\nIt supports two barebones directives:\n\n- docutils\' `doctest_block`\n\n  ```rst\n  >>> 2 + 2\n  4\n  ```\n\n- `.. doctest::` directive\n\n  reStructuredText:\n\n  ```rst\n  .. doctest::\n\n     >>> 2 + 2\n     4\n  ```\n\n  Markdown (requires [myst-parser]):\n\n  ````markdown\n  ```{doctest}\n  >>> 2 + 2\n  4\n  ```\n  ````\n\n[myst-parser]: https://myst-parser.readthedocs.io/en/latest/\n\n#### Test your docs\n\n##### reStructuredText\n\n```console\n$ python -m doctest_docutils README.rst -v\n```\n\nThat\'s what `doctest` does by design.\n\n##### Markdown\n\nIf you install [myst-parser], doctest will run on .md files.\n\n```console\n$ python -m doctest_docutils README.md -v\n```\n\n### pytest plugin\n\n_This plugin disables [pytest\'s standard `doctest` plugin]._\n\nThis plugin integrates with the above module.\n\n```console\n$ pytest docs/\n```\n\nLike the above module, it supports docutils\' own `doctest_block` and a basic\n`.. doctest::` directive.\n\nSee more: <https://gp-libs.git-pull.com/doctest/pytest.html>\n\n[pytest\'s standard `doctest` plugin]: https://docs.pytest.org/en/stable/how-to/doctest.html#doctest\n\n## sphinx plugins\n\n### Plain-text issue linker (`linkify-issues`)\n\nWe need to parse plain text, e.g. #99999, to point to the project tracker at\nhttps://github.com/git-pull/gp-libs/issues/99999. This way the markdown looks\ngood anywhere you render it, including GitHub and GitLab.\n\n#### Configuration\n\nIn your _conf.py_:\n\n1. Add `\'linkify_issues\'` to `extensions`\n\n   ```python\n   extensions = [\n       # ...\n       "linkify_issues",\n   ]\n   ```\n\n2. Configure your issue URL, `issue_url_tpl`:\n\n   ```python\n   # linkify_issues\n   issue_url_tpl = \'https://github.com/git-pull/gp-libs/issues/{issue_id}\'\n   ```\n\n   The config variable is formatted via {meth}`str.format` where `issue_id` is\n   `42` if the text is \\#42.\n\nSee more: <https://gp-libs.git-pull.com/linkify_issues/>\n\n### Table of contents for autodoc\n\n`sphinx.ext.autodoc` doesn\'t link objects in the table of contents. So we need a\nplugin to help.\n\nSee more: <https://gp-libs.git-pull.com/sphinx_toctree_autodoc_fix/>\n\n#### Configuration\n\n1. Add `\'sphinx_toctree_autodoc_fix\'` to `extensions`\n\n   ```python\n   extensions = [\n       # ...\n       "sphinx_toctree_autodoc_fix",\n   ]\n   ```\n\n## Install\n\n```console\n$ pip install --user gp-libs\n```\n\n### Developmental releases\n\nYou can test the unpublished version of g before its released.\n\n- [pip](https://pip.pypa.io/en/stable/):\n\n  ```console\n  $ pip install --user --upgrade --pre gp-libs\n  ```\n\n# More information\n\n- Python support: >= 3.7, pypy\n- Source: <https://github.com/git-pull/gp-libs>\n- Docs: <https://gp-libs.git-pull.com>\n- Changelog: <https://gp-libs.git-pull.com/history.html>\n- Issues: <https://github.com/git-pull/gp-libs/issues>\n- Test Coverage: <https://codecov.io/gh/git-pull/gp-libs>\n- pypi: <https://pypi.python.org/pypi/gp-libs>\n- License: [MIT](https://opensource.org/licenses/MIT).\n\n[![Docs](https://github.com/git-pull/gp-libs/workflows/docs/badge.svg)](https://gp-libs.git-pull.com)\n[![Build Status](https://github.com/git-pull/gp-libs/workflows/tests/badge.svg)](https://github.com/git-pull/gp-libs/actions?query=workflow%3A%22tests%22)\n',
     'author': 'Tony Narlock',
     'author_email': 'tony@git-pull.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gp-libs.git-pull.com',
```

### Comparing `gp-libs-0.0.1a8/PKG-INFO` & `gp-libs-0.0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp-libs
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Internal utilities for projects following git-pull python package spec
 Home-page: https://gp-libs.git-pull.com
 License: MIT
 Author: Tony Narlock
 Author-email: tony@git-pull.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

