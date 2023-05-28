# Comparing `tmp/pytest-md-report-0.3.0.tar.gz` & `tmp/pytest-md-report-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-md-report-0.3.0.tar", last modified: Sat Aug  6 17:07:38 2022, max compression
+gzip compressed data, was "pytest-md-report-0.3.1.tar", last modified: Sun May 28 14:55:33 2023, max compression
```

## Comparing `pytest-md-report-0.3.0.tar` & `pytest-md-report-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    12113 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    10648 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      763 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/pytest_md_report/
--rw-r--r--   0 toor      (1000) toor      (1000)      300 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pytest_md_report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pytest_md_report/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4337 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pytest_md_report/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16902 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pytest_md_report/plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/pytest_md_report/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/pytest_md_report.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    12113 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      609 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-08-06 17:07:19.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       94 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2022-08-06 17:07:38.000000 pytest-md-report-0.3.0/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       86 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2778 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-06 17:07:38.791550 pytest-md-report-0.3.0/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1034 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/tests/test_option.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5016 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      971 2022-08-06 17:07:18.000000 pytest-md-report-0.3.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    10153 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      764 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/pytest_md_report/
+-rw-r--r--   0 toor      (1000) toor      (1000)      300 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4447 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16902 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/pytest_md_report/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/pytest_md_report.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11619 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      609 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-28 14:55:25.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       94 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-05-28 14:55:33.000000 pytest-md-report-0.3.1/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       86 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2791 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-28 14:55:33.964043 pytest-md-report-0.3.1/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       30 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/conftest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1034 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/test_option.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5016 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tests/test_plugin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      917 2023-05-28 14:55:15.000000 pytest-md-report-0.3.1/tox.ini
```

### Comparing `pytest-md-report-0.3.0/LICENSE` & `pytest-md-report-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.0/PKG-INFO` & `pytest-md-report-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
@@ -12,26 +12,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pytest-md-report**
    :backlinks: top
    :depth: 2
@@ -51,19 +51,19 @@
     :target: https://pypi.org/project/pytest-md-report
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make a test results report with Markdown table format.
+A pytest plugin to make test results report with Markdown table format.
 
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
@@ -111,149 +111,123 @@
     | examples/test_pass.py    |      2 |        |       |         |         |         |        2 |
     | examples/test_skipped.py |        |        |       |       2 |         |         |        2 |
     | examples/test_xfailed.py |        |        |       |         |       2 |         |        2 |
     | examples/test_xpassed.py |        |        |       |         |         |       2 |        2 |
     | TOTAL                    |      2 |      2 |     2 |       2 |       2 |       2 |       12 |
 
 
+Config file examples
+--------------------------------------------
+You can set configurations with ``pyproject.toml`` or ``setup.cfg`` as follows.
+
+:Example of ``pyproject.toml``:
+    .. code-block:: toml
+
+        [tool.pytest.ini_options]
+        md_report = true
+        md_report_verbose = 0
+        md_report_color = "auto"
+
+:Example of ``setup.cfg``:
+    .. code-block:: ini
+
+        [tool:pytest]
+        md_report = True
+        md_report_verbose = 0
+        md_report_color = auto
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
     make test results report with markdown table format:
-      --md-report           create markdown report. you can also specify the value
-                            with PYTEST_MD_REPORT environment variable.
+      --md-report           Create Markdown report. you can also specify the value with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-md-report. if not set, using
-                            verbosity level of pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_VERBOSE environment variable.
+                            Verbosity level for pytest-md-report.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
-                            path to a file that outputs test report.
-                            overwrite a file content if the file already exists.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_OUTPUT environment variable.
-      --md-report-tee       output test report for both standard output and a file.
-                            you can also specify the value with PYTEST_MD_REPORT_TEE
-                            environment variable.
+                            Path to a file to the outputs test report.
+                            Overwrite a file content if the file already exists.
+                            you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
+      --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            auto: display colored (text and background) reports by
-                            using ANSI escape codes.
-                            text: display colored (text) reports by using ANSI
-                            escape codes.
-                            never: display report without color.
-                            defaults to 'auto'.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_COLOR environment variable.
+                            How to color output reports.
+                            auto: render colored (text and background) reports using ANSI escape codes.
+                            text: render colored text reports by using ANSI escape codes.
+                            never: render report without color.
+                            Defaults to 'auto'.
+                            you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
-                            margin size for each cells.
-                            defaults to 1.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_MARGIN environment variable.
+                            Margin size for each cell.
+                            Defaults to 1.
+                            you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
-                            rendering method for results of zero values.
+                            Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            defaults to number. defaults to empty when execution in
-                            ci.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ZEROS environment variable.
+                            Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
+                            otherwise 'number'.
+                            you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
-                            text color of succeeded results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_green.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
+                            Text color of succeeded results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_green'.
+                            you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
-                            text color of skipped results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_yellow.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SKIP_COLOR environment variable.
+                            Text color of skipped results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_yellow'.
+                            you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
-                            text color of failed results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_red.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+                            Text color of failed results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_red'.
+                            you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     create markdown report.
+  md_report (bool):     Create Markdown report.
   md_report_verbose (string):
-                        verbosity level for pytest-md-report. if not set, using
-                        verbosity level of pytest. defaults to 0.
+                        Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        auto: display colored (text and background) reports by
-                        using ANSI escape codes. text: display colored (text)
-                        reports by using ANSI escape codes. never: display
-                        report without color. defaults to 'auto'.
+                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
+                        render report without color. Defaults to 'auto'.
   md_report_output (string):
-                        path to a file that outputs test report. overwrite a
-                        file content if the file already exists.
+                        Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
-                        margin size for each cells. defaults to 1.
+                        Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        rendering method for results of zero values. number:
-                        render as a digit number (0). empty: not rendering.
-                        defaults to number. defaults to empty when execution in
-                        ci.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
+                        insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        text color of succeeded results. specify a color name
-                        (one of the black/red/green/yellow/blue/magenta/cyan/whi
-                        te/lightblack/lightred/lightgreen/lightyellow/lightblue/
-                        lightmagenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_green.
+                        Text color of succeeded results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_green'.
   md_report_skip_color (string):
-                        text color of skipped results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_yellow.
+                        Text color of skipped results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_yellow'.
   md_report_error_color (string):
-                        text color of failed results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_red.
-
-
-:Example of ``pyproject.toml``:
-    .. code-block:: toml
-
-        [tool.pytest.ini_options]
-        md_report = true
-        md_report_verbose = 0
-        md_report_color = "auto"
-
-:Example of ``setup.cfg``:
-    .. code-block:: ini
-
-        [tool:pytest]
-        md_report = True
-        md_report_verbose = 0
-        md_report_color = auto
+                        Text color of failed results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_red'.
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.0/README.rst` & `pytest-md-report-0.3.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     :target: https://pypi.org/project/pytest-md-report
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make a test results report with Markdown table format.
+A pytest plugin to make test results report with Markdown table format.
 
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
@@ -77,149 +77,123 @@
     | examples/test_pass.py    |      2 |        |       |         |         |         |        2 |
     | examples/test_skipped.py |        |        |       |       2 |         |         |        2 |
     | examples/test_xfailed.py |        |        |       |         |       2 |         |        2 |
     | examples/test_xpassed.py |        |        |       |         |         |       2 |        2 |
     | TOTAL                    |      2 |      2 |     2 |       2 |       2 |       2 |       12 |
 
 
+Config file examples
+--------------------------------------------
+You can set configurations with ``pyproject.toml`` or ``setup.cfg`` as follows.
+
+:Example of ``pyproject.toml``:
+    .. code-block:: toml
+
+        [tool.pytest.ini_options]
+        md_report = true
+        md_report_verbose = 0
+        md_report_color = "auto"
+
+:Example of ``setup.cfg``:
+    .. code-block:: ini
+
+        [tool:pytest]
+        md_report = True
+        md_report_verbose = 0
+        md_report_color = auto
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
     make test results report with markdown table format:
-      --md-report           create markdown report. you can also specify the value
-                            with PYTEST_MD_REPORT environment variable.
+      --md-report           Create Markdown report. you can also specify the value with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-md-report. if not set, using
-                            verbosity level of pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_VERBOSE environment variable.
+                            Verbosity level for pytest-md-report.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
-                            path to a file that outputs test report.
-                            overwrite a file content if the file already exists.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_OUTPUT environment variable.
-      --md-report-tee       output test report for both standard output and a file.
-                            you can also specify the value with PYTEST_MD_REPORT_TEE
-                            environment variable.
+                            Path to a file to the outputs test report.
+                            Overwrite a file content if the file already exists.
+                            you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
+      --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            auto: display colored (text and background) reports by
-                            using ANSI escape codes.
-                            text: display colored (text) reports by using ANSI
-                            escape codes.
-                            never: display report without color.
-                            defaults to 'auto'.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_COLOR environment variable.
+                            How to color output reports.
+                            auto: render colored (text and background) reports using ANSI escape codes.
+                            text: render colored text reports by using ANSI escape codes.
+                            never: render report without color.
+                            Defaults to 'auto'.
+                            you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
-                            margin size for each cells.
-                            defaults to 1.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_MARGIN environment variable.
+                            Margin size for each cell.
+                            Defaults to 1.
+                            you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
-                            rendering method for results of zero values.
+                            Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            defaults to number. defaults to empty when execution in
-                            ci.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ZEROS environment variable.
+                            Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
+                            otherwise 'number'.
+                            you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
-                            text color of succeeded results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_green.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
+                            Text color of succeeded results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_green'.
+                            you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
-                            text color of skipped results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_yellow.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SKIP_COLOR environment variable.
+                            Text color of skipped results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_yellow'.
+                            you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
-                            text color of failed results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_red.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+                            Text color of failed results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_red'.
+                            you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     create markdown report.
+  md_report (bool):     Create Markdown report.
   md_report_verbose (string):
-                        verbosity level for pytest-md-report. if not set, using
-                        verbosity level of pytest. defaults to 0.
+                        Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        auto: display colored (text and background) reports by
-                        using ANSI escape codes. text: display colored (text)
-                        reports by using ANSI escape codes. never: display
-                        report without color. defaults to 'auto'.
+                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
+                        render report without color. Defaults to 'auto'.
   md_report_output (string):
-                        path to a file that outputs test report. overwrite a
-                        file content if the file already exists.
+                        Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
-                        margin size for each cells. defaults to 1.
+                        Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        rendering method for results of zero values. number:
-                        render as a digit number (0). empty: not rendering.
-                        defaults to number. defaults to empty when execution in
-                        ci.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
+                        insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        text color of succeeded results. specify a color name
-                        (one of the black/red/green/yellow/blue/magenta/cyan/whi
-                        te/lightblack/lightred/lightgreen/lightyellow/lightblue/
-                        lightmagenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_green.
+                        Text color of succeeded results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_green'.
   md_report_skip_color (string):
-                        text color of skipped results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_yellow.
+                        Text color of skipped results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_yellow'.
   md_report_error_color (string):
-                        text color of failed results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_red.
-
-
-:Example of ``pyproject.toml``:
-    .. code-block:: toml
-
-        [tool.pytest.ini_options]
-        md_report = true
-        md_report_verbose = 0
-        md_report_color = "auto"
-
-:Example of ``setup.cfg``:
-    .. code-block:: ini
-
-        [tool:pytest]
-        md_report = True
-        md_report_verbose = 0
-        md_report_color = auto
+                        Text color of failed results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_red'.
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.0/pyproject.toml` & `pytest-md-report-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 known_third_party = [
     "mock",
 ]
 include_trailing_comma = true
 line_length = 100
@@ -32,15 +32,15 @@
     '*/.eggs/*',
     '*/.pytype/*',
     '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `pytest-md-report-0.3.0/pytest_md_report/_const.py` & `pytest-md-report-0.3.1/pytest_md_report/_const.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,95 +52,98 @@
 
 
 OPTION_PREFIX = "md-report"
 
 
 @unique
 class Option(Enum):
-    MD_REPORT = (OPTION_PREFIX, "create markdown report.")
+    MD_REPORT = (OPTION_PREFIX, "Create Markdown report.")
     MD_REPORT_VERBOSE = (
         f"{OPTION_PREFIX}-verbose",
         dedent(
             """\
-            verbosity level for pytest-md-report. if not set, using verbosity level of pytest.
-            defaults to 0.
+            Verbosity level for pytest-md-report.
+            If not set, use the verbosity level of pytest.
+            Defaults to 0.
             """
         ),
     )
     MD_REPORT_OUTPUT = (
         f"{OPTION_PREFIX}-output",
         dedent(
             """\
-            path to a file that outputs test report.
-            overwrite a file content if the file already exists.
+            Path to a file to the outputs test report.
+            Overwrite a file content if the file already exists.
             """
         ),
     )
     MD_REPORT_TEE = (
         f"{OPTION_PREFIX}-tee",
         "output test report for both standard output and a file.",
     )
     MD_REPORT_COLOR = (
         f"{OPTION_PREFIX}-color",
         dedent(
             """\
-            auto: display colored (text and background) reports by using ANSI escape codes.
-            text: display colored (text) reports by using ANSI escape codes.
-            never: display report without color.
-            defaults to '{default}'.
+            How to color output reports.
+            auto: render colored (text and background) reports using ANSI escape codes.
+            text: render colored text reports by using ANSI escape codes.
+            never: render report without color.
+            Defaults to '{default}'.
             """
         ).format(default=Default.COLOR),
     )
     MD_REPORT_MARGIN = (
         f"{OPTION_PREFIX}-margin",
         dedent(
             """\
-            margin size for each cells.
-            defaults to {default}.
+            Margin size for each cell.
+            Defaults to {default}.
             """
         ).format(default=Default.MARGIN),
     )
     MD_REPORT_ZEROS = (
         f"{OPTION_PREFIX}-zeros",
         dedent(
             """\
-            rendering method for results of zero values.
+            Rendering method for results of zero values.
             number: render as a digit number (0).
             empty: not rendering.
-            defaults to {default}. defaults to empty when execution in ci.
+            Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
+            otherwise '{default}'.
             """
         ).format(default=Default.ZEROS),
     )
     MD_REPORT_SUCCESS_COLOR = (
         f"{OPTION_PREFIX}-success-color",
         dedent(
             """\
-            text color of succeeded results.
-            specify a color name (one of the {names}) or a color code (e.g. #ff1020).
-            defaults to {default}.
+            Text color of succeeded results.
+            Specify a color name (one of the {names}) or a color code (e.g. #ff1020).
+            Defaults to '{default}'.
             """
         ).format(names=COLOR_NAMES, default=Default.FGColor.SUCCESS),
     )
     MD_REPORT_SKIP_COLOR = (
         f"{OPTION_PREFIX}-skip-color",
         dedent(
             """\
-            text color of skipped results.
-            specify a color name (one of the {names}) or a color code (e.g. #ff1020).
-            defaults to {default}.
+            Text color of skipped results.
+            Specify a color name (one of the {names}) or a color code (e.g. #ff1020).
+            Defaults to '{default}'.
             """
         ).format(names=COLOR_NAMES, default=Default.FGColor.SKIP),
     )
     MD_REPORT_ERROR_COLOR = (
         f"{OPTION_PREFIX}-error-color",
         dedent(
             """\
-            text color of failed results.
-            specify a color name (one of the {names}) or a color code (e.g. #ff1020).
-            defaults to {default}.
+            Text color of failed results.
+            Specify a color name (one of the {names}) or a color code (e.g. #ff1020).
+            Defaults to '{default}'.
             """
         ).format(names=COLOR_NAMES, default=Default.FGColor.ERROR),
     )
 
     @property
     def cmdoption_str(self) -> str:
         return "--" + self.__name.lower()
```

### Comparing `pytest-md-report-0.3.0/pytest_md_report/plugin.py` & `pytest-md-report-0.3.1/pytest_md_report/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.0/pytest_md_report.egg-info/PKG-INFO` & `pytest-md-report-0.3.1/pytest_md_report.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pytest plugin to make a test results report with Markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
@@ -12,26 +12,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **pytest-md-report**
    :backlinks: top
    :depth: 2
@@ -51,19 +51,19 @@
     :target: https://pypi.org/project/pytest-md-report
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make a test results report with Markdown table format.
+A pytest plugin to make test results report with Markdown table format.
 
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
@@ -111,149 +111,123 @@
     | examples/test_pass.py    |      2 |        |       |         |         |         |        2 |
     | examples/test_skipped.py |        |        |       |       2 |         |         |        2 |
     | examples/test_xfailed.py |        |        |       |         |       2 |         |        2 |
     | examples/test_xpassed.py |        |        |       |         |         |       2 |        2 |
     | TOTAL                    |      2 |      2 |     2 |       2 |       2 |       2 |       12 |
 
 
+Config file examples
+--------------------------------------------
+You can set configurations with ``pyproject.toml`` or ``setup.cfg`` as follows.
+
+:Example of ``pyproject.toml``:
+    .. code-block:: toml
+
+        [tool.pytest.ini_options]
+        md_report = true
+        md_report_verbose = 0
+        md_report_color = "auto"
+
+:Example of ``setup.cfg``:
+    .. code-block:: ini
+
+        [tool:pytest]
+        md_report = True
+        md_report_verbose = 0
+        md_report_color = auto
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
     make test results report with markdown table format:
-      --md-report           create markdown report. you can also specify the value
-                            with PYTEST_MD_REPORT environment variable.
+      --md-report           Create Markdown report. you can also specify the value with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
-                            verbosity level for pytest-md-report. if not set, using
-                            verbosity level of pytest.
-                            defaults to 0.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_VERBOSE environment variable.
+                            Verbosity level for pytest-md-report.
+                            If not set, use the verbosity level of pytest.
+                            Defaults to 0.
+                            you can also specify the value with PYTEST_MD_REPORT_VERBOSE environment variable.
       --md-report-output=FILEPATH
-                            path to a file that outputs test report.
-                            overwrite a file content if the file already exists.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_OUTPUT environment variable.
-      --md-report-tee       output test report for both standard output and a file.
-                            you can also specify the value with PYTEST_MD_REPORT_TEE
-                            environment variable.
+                            Path to a file to the outputs test report.
+                            Overwrite a file content if the file already exists.
+                            you can also specify the value with PYTEST_MD_REPORT_OUTPUT environment variable.
+      --md-report-tee       output test report for both standard output and a file. you can also specify the value with PYTEST_MD_REPORT_TEE environment variable.
       --md-report-color={auto,text,never}
-                            auto: display colored (text and background) reports by
-                            using ANSI escape codes.
-                            text: display colored (text) reports by using ANSI
-                            escape codes.
-                            never: display report without color.
-                            defaults to 'auto'.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_COLOR environment variable.
+                            How to color output reports.
+                            auto: render colored (text and background) reports using ANSI escape codes.
+                            text: render colored text reports by using ANSI escape codes.
+                            never: render report without color.
+                            Defaults to 'auto'.
+                            you can also specify the value with PYTEST_MD_REPORT_COLOR environment variable.
       --md-report-margin=MARGIN
-                            margin size for each cells.
-                            defaults to 1.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_MARGIN environment variable.
+                            Margin size for each cell.
+                            Defaults to 1.
+                            you can also specify the value with PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
-                            rendering method for results of zero values.
+                            Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            defaults to number. defaults to empty when execution in
-                            ci.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ZEROS environment variable.
+                            Defaults to 'empty' when CI environment variable is set to TRUE (case insensitive);
+                            otherwise 'number'.
+                            you can also specify the value with PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
-                            text color of succeeded results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_green.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
+                            Text color of succeeded results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_green'.
+                            you can also specify the value with PYTEST_MD_REPORT_SUCCESS_COLOR environment variable.
       --md-report-skip-color=MD_REPORT_SKIP_COLOR
-                            text color of skipped results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_yellow.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_SKIP_COLOR environment variable.
+                            Text color of skipped results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_yellow'.
+                            you can also specify the value with PYTEST_MD_REPORT_SKIP_COLOR environment variable.
       --md-report-error-color=MD_REPORT_ERROR_COLOR
-                            text color of failed results.
-                            specify a color name (one of the black/red/green/yellow/
-                            blue/magenta/cyan/white/lightblack/lightred/lightgreen/l
-                            ightyellow/lightblue/lightmagenta/lightcyan/lightwhite)
-                            or a color code (e.g. #ff1020).
-                            defaults to light_red.
-                            you can also specify the value with
-                            PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+                            Text color of failed results.
+                            Specify a color name (one of the black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a
+                            color code (e.g. #ff1020).
+                            Defaults to 'light_red'.
+                            you can also specify the value with PYTEST_MD_REPORT_ERROR_COLOR environment variable.
+
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     create markdown report.
+  md_report (bool):     Create Markdown report.
   md_report_verbose (string):
-                        verbosity level for pytest-md-report. if not set, using
-                        verbosity level of pytest. defaults to 0.
+                        Verbosity level for pytest-md-report. If not set, use the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
-                        auto: display colored (text and background) reports by
-                        using ANSI escape codes. text: display colored (text)
-                        reports by using ANSI escape codes. never: display
-                        report without color. defaults to 'auto'.
+                        How to color output reports. auto: render colored (text and background) reports using ANSI escape codes. text: render colored text reports by using ANSI escape codes. never:
+                        render report without color. Defaults to 'auto'.
   md_report_output (string):
-                        path to a file that outputs test report. overwrite a
-                        file content if the file already exists.
+                        Path to a file to the outputs test report. Overwrite a file content if the file already exists.
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
-                        margin size for each cells. defaults to 1.
+                        Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
-                        rendering method for results of zero values. number:
-                        render as a digit number (0). empty: not rendering.
-                        defaults to number. defaults to empty when execution in
-                        ci.
+                        Rendering method for results of zero values. number: render as a digit number (0). empty: not rendering. Defaults to 'empty' when CI environment variable is set to TRUE (case
+                        insensitive); otherwise 'number'.
   md_report_success_color (string):
-                        text color of succeeded results. specify a color name
-                        (one of the black/red/green/yellow/blue/magenta/cyan/whi
-                        te/lightblack/lightred/lightgreen/lightyellow/lightblue/
-                        lightmagenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_green.
+                        Text color of succeeded results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_green'.
   md_report_skip_color (string):
-                        text color of skipped results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_yellow.
+                        Text color of skipped results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_yellow'.
   md_report_error_color (string):
-                        text color of failed results. specify a color name (one
-                        of the black/red/green/yellow/blue/magenta/cyan/white/li
-                        ghtblack/lightred/lightgreen/lightyellow/lightblue/light
-                        magenta/lightcyan/lightwhite) or a color code (e.g.
-                        #ff1020). defaults to light_red.
-
-
-:Example of ``pyproject.toml``:
-    .. code-block:: toml
-
-        [tool.pytest.ini_options]
-        md_report = true
-        md_report_verbose = 0
-        md_report_color = "auto"
-
-:Example of ``setup.cfg``:
-    .. code-block:: ini
-
-        [tool:pytest]
-        md_report = True
-        md_report_verbose = 0
-        md_report_color = auto
+                        Text color of failed results. Specify a color name (one of the
+                        black/red/green/yellow/blue/magenta/cyan/white/lightblack/lightred/lightgreen/lightyellow/lightblue/lightmagenta/lightcyan/lightwhite) or a color code (e.g. #ff1020). Defaults
+                        to 'light_red'.
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.3.0/pytest_md_report.egg-info/SOURCES.txt` & `pytest-md-report-0.3.1/pytest_md_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.0/setup.py` & `pytest-md-report-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "pytest-md-report"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -48,30 +48,30 @@
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Testing",
         "Topic :: Text Processing",
         "Topic :: Text Processing :: Markup :: Markdown",
     ],
```

### Comparing `pytest-md-report-0.3.0/tests/test_option.py` & `pytest-md-report-0.3.1/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.0/tests/test_plugin.py` & `pytest-md-report-0.3.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.3.0/tox.ini` & `pytest-md-report-0.3.1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 [tox]
 envlist =
-    py{36,37,38,39,10}
+    py{37,38,39,310,311}
     pypy3
     build
-    clean
     fmt
     lint
 
 [testenv]
 extras =
     test
 commands =
     pytest tests {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
     twine
     wheel
 commands =
     python setup.py sdist bdist_wheel
     twine check dist/*.whl dist/*.tar.gz
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
-    black>=22.6
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py examples tests pytest_md_report
 
 [testenv:lint]
 skip_install = true
 deps =
     codespell
-    mypy>=0.971
-    pylama>=8.3.7
-    pyflakes<2.5
+    mypy>=1
+    pylama>=8.4.1
 commands =
     python setup.py check
     mypy pytest_md_report setup.py
     pylama
     - codespell pytest_md_report examples tests -q 2 --check-filenames
```

