# Comparing `tmp/circuitpython-display_ht16k33-0.2.0.tar.gz` & `tmp/circuitpython-display_ht16k33-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-display_ht16k33-0.2.0.tar", last modified: Fri May 26 19:54:26 2023, max compression
+gzip compressed data, was "circuitpython-display_ht16k33-0.2.1.tar", last modified: Sun May 28 00:24:41 2023, max compression
```

## Comparing `circuitpython-display_ht16k33-0.2.0.tar` & `circuitpython-display_ht16k33-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.413729 circuitpython-display_ht16k33-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/display_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/7mwahe.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_segments_count_down.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_segments_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.533956 circuitpython-display_ht16k33-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.533956 circuitpython-display_ht16k33-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.533956 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-28 00:24:41.000000 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-28 00:24:41.000000 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 00:24:41.000000 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 00:24:41.000000 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 00:24:41.000000 circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.537956 circuitpython-display_ht16k33-0.2.1/display_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/display_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/display_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/display_ht16k33/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/display_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/7mwahe.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38124 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/docs/segments.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_segments_count_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_segments_custom_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-28 00:24:32.000000 circuitpython-display_ht16k33-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 00:24:16.000000 circuitpython-display_ht16k33-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 00:24:41.541956 circuitpython-display_ht16k33-0.2.1/setup.cfg
```

### Comparing `circuitpython-display_ht16k33-0.2.0/.github/workflows/build.yml` & `circuitpython-display_ht16k33-0.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/.github/workflows/release_gh.yml` & `circuitpython-display_ht16k33-0.2.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/.gitignore` & `circuitpython-display_ht16k33-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/.pre-commit-config.yaml` & `circuitpython-display_ht16k33-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/.pylintrc` & `circuitpython-display_ht16k33-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/LICENSE` & `circuitpython-display_ht16k33-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/PKG-INFO` & `circuitpython-display_ht16k33-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display_ht16k33
-Version: 0.2.0
+Version: 0.2.1
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,14 +41,19 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
+Also work with segments with a very similar sintax to the Adafruit Segments library
+
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
+
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython-display_ht16k33-0.2.0/README.rst` & `circuitpython-display_ht16k33-0.2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,19 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
+Also work with segments with a very similar sintax to the Adafruit Segments library
+
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
+
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/PKG-INFO` & `circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display-ht16k33
-Version: 0.2.0
+Version: 0.2.1
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,14 +41,19 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
+Also work with segments with a very similar sintax to the Adafruit Segments library
+
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
+
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt` & `circuitpython-display_ht16k33-0.2.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 docs/7mwahe.gif
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/font5x8.bin
 docs/index.rst
 docs/requirements.txt
+docs/segments.jpg
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display_ht16k33_segments_count_down.py
+examples/display_ht16k33_segments_custom_chars.py
 examples/display_ht16k33_segments_simpletest.py
 examples/display_ht16k33_simpletest.py
 examples/display_ht16k33_text.py
```

### Comparing `circuitpython-display_ht16k33-0.2.0/display_ht16k33/ht16k33.py` & `circuitpython-display_ht16k33-0.2.1/display_ht16k33/ht16k33.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,37 +10,44 @@
 Based on some code from https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git
 Authors: Radomir Dopieralski and Tony DiCola License: MIT
 
 * Author(s): Jose D. Montoya
 
 
 """
-import gc
 from vectorio import Circle
 import displayio
 import ulab.numpy as np
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
+# pylint: disable=too-many-arguments, too-many-instance-attributes
 class HT16K33:
     """
     Main class
     """
 
     def __init__(
         self,
+        x,
+        y,
+        radius=10,
+        text=False,
         num_led_x: int = 16,
         num_led_y: int = 8,
         register_width: int = 2,
     ) -> None:
+        self.x = x
+        self.y = y
         self.cols = num_led_x
         self.rows = num_led_y
+        self.radius = radius
 
         self.bit_mask = ((1 << self.cols) - 1) << 0
 
         self.buffer_rows = []
         for _ in range(self.rows):
             self.buffer_rows.append(bytearray(register_width))
 
@@ -48,27 +55,33 @@
         self.array = np.ndarray(np.empty((self.rows, self.cols)), dtype=np.uint8)
 
         self.length = register_width
 
         self.group = displayio.Group()
 
         palette = displayio.Palette(3)
-        palette[0] = 0x123456
-        palette[1] = 0x123456
+        palette[0] = 0x2263A4
+        palette[1] = 0x101010
         palette[2] = 0xFF5500
 
         self.matrix = []
-        for j in range(1, self.rows + 1):
+
+        if text:
+            y_range = range(1, self.rows + 1)
+        else:
+            y_range = range(self.rows + 1, 1, -1)
+
+        for j in y_range:
             row_buff = []
             for coord_x in range(1, self.cols + 1):
                 value = Circle(
                     pixel_shader=palette,
-                    radius=10,
-                    x=coord_x * 25,
-                    y=j * 25,
+                    radius=self.radius,
+                    x=self.x + coord_x * (self.radius * 2 + self.radius // 2),
+                    y=self.y + j * (self.radius * 2 + self.radius // 2),
                     color_index=1,
                 )
                 row_buff.append(value)
                 self.group.append(value)
             self.matrix.append(row_buff)
 
     @property
@@ -80,31 +93,26 @@
 
     def set(self, y, new_value: int) -> None:
         """
         Set a particular value in an specific row defined by y
         """
         reg = 0
 
-        if self.length == 2:
-            order = range(0, 2)
-        if self.length == 1:
-            order = range(0, 1)
+        order = range(0, self.length)
 
         for ind in order:
             reg = (reg << 8) | self.buffer_rows[y][ind]
 
         reg &= ~self.bit_mask
         reg |= new_value
 
         for ind2 in order:
             self.buffer_rows[y][ind2] = reg & 0xFF
             reg >>= 8
-
         self.convert_to_leds(y)
-        self.update(y)
 
     def pixel(self, x: int, y: int, color=True) -> None:
         """
         Set a specific pixel in the matrix
         """
         reg = 0
         order = range(0, self.length)
@@ -136,14 +144,15 @@
                 self.array[y][index] = buffval
                 index = index + 1
 
     def update(self, y) -> None:
         """
         Update a particular Row
         """
+
         for i, _ in enumerate(self.matrix[y]):
             if self.array[y][i]:
                 self.matrix[y][i].color_index = 2
             else:
                 self.matrix[y][i].color_index = 1
 
     def update_all(self):
@@ -162,15 +171,15 @@
         """
         if rotate:
             pass
         self.array = np.roll(self.array, y, axis=0)
         self.array = np.roll(self.array, x, axis=1)
 
         self.update_all()
-        gc.collect()
+        # gc.collect()
 
     def shift_right(self, rotate: bool = False) -> None:
         """
         Shift all pixels right
 
         :param rotate: (Optional) Rotate the shifted pixels to the left side (default=False)
         """
@@ -201,30 +210,12 @@
         self.shift(0, -1, rotate)
 
     def fill(self, color: bool) -> None:
         """
         fill the entire matrix
         """
         if color:
-            new_value = 0xFFFF
+            new_value = 0xFF
         else:
-            new_value = 0x0000
+            new_value = 0x00
         for ele in range(self.rows):
-            reg = 0
-
-            if self.length == 2:
-                order = range(0, 2)
-            if self.length == 1:
-                order = range(0, 1)
-
-            for ind in order:
-                reg = (reg << 8) | self.buffer_rows[ele][ind]
-
-            reg &= ~self.bit_mask
-            reg |= new_value
-
-            for ind2 in order:
-                self.buffer_rows[ele][ind2] = reg & 0xFF
-                reg >>= 8
-
-            self.convert_to_leds(ele)
-        self.update_all()
+            self.set(ele, new_value)
```

### Comparing `circuitpython-display_ht16k33-0.2.0/display_ht16k33/segments.py` & `circuitpython-display_ht16k33-0.2.1/display_ht16k33/segments.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,18 +10,25 @@
 Based on some code from https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git
 Authors: Radomir Dopieralski and Tony DiCola License: MIT
 
 * Author(s): Jose D. Montoya
 
 
 """
-from vectorio import Polygon
+
+from vectorio import Polygon, Circle
 import displayio
 
-__version__ = "0.2.0"
+
+try:
+    from typing import Optional, Dict
+except ImportError:
+    pass
+
+__version__ = "0.2.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 NUMBERS = (
     0x3F,  # 0
     0x06,  # 1
     0x5B,  # 2
@@ -55,40 +62,59 @@
     0x3E,  # U
     0x1C,  # v
     0x40,  # -
     0x40,  # -
     0x6E,  # y
     0x40,  # -
     0x40,  # -
+    0x00,  # Null
 )
 
+# pylint: disable=too-many-arguments, too-many-instance-attributes
+
 
 class SEG7x4:
     """
     Main class
+
+    :param dict char_dict: An optional dictionary mapping strings to bit settings integers used
+        for defining how to display custom letters
     """
 
     def __init__(
         self,
         x: int,
         y: int,
+        height: int = 40,
+        length: int = 40,
+        space: int = 70,
+        stroke: int = 4,
+        color_off: int = 0x123456,
+        color_on: int = 0xFF5500,
+        char_dict: Optional[Dict[str, int]] = None,
     ) -> None:
         self._x = x
         self.y = y
 
         self._digits = [None, None, None, None]
+        self.buffer = [None, None, None, None]
+        self._two_points_container = []
+
+        self._chardict = char_dict
+
         self.group = displayio.Group()
 
         self._palette = displayio.Palette(3)
-        self._palette[0] = 0x123456
-        self._palette[1] = 0x123456
-        self._palette[2] = 0xFF5500
-        self._stroke = 4
-        self._length = 40
-        self._height = 40
+        self._palette.make_transparent(0)
+        self._palette[1] = color_off
+        self._palette[2] = color_on
+        self._stroke = stroke
+        self._length = length
+        self._height = height
+        self._space = space
 
         self._pointsh = [
             (0, 0),
             (self._stroke, self._stroke // 2),
             (self._length - self._stroke, self._stroke // 2),
             (self._length, 0),
             (self._length - self._stroke, -self._stroke // 2),
@@ -100,18 +126,39 @@
             (-self._stroke // 2, self._stroke),
             (-self._stroke // 2, self._height - self._stroke),
             (0, self._height),
             (self._stroke // 2, self._height - self._stroke),
             (self._stroke // 2, self._stroke),
         ]
 
-        self._draw_digits(40, 3)
-        self._draw_digits(90, 2)
-        self._draw_digits(150, 1)
-        self._draw_digits(200, 0)
+        self._draw_digits(self._x, 3)
+        self._draw_digits(self._x + self._space, 2)
+        self._draw_digits(self._x + self._space * 2, 1)
+        self._draw_digits(self._x + self._space * 3, 0)
+        self._draw_two_points()
+
+    def _draw_two_points(self):
+        value = Circle(
+            pixel_shader=self._palette,
+            radius=self._height // 8,
+            x=self._x + self._space + self._length + (self._space - self._length) // 2,
+            y=self.y + self._height // 2 - (self._height // 16),
+            color_index=1,
+        )
+        self.group.append(value)
+        self._two_points_container.append(value)
+        value = Circle(
+            pixel_shader=self._palette,
+            radius=self._height // 8,
+            x=self._x + self._space + self._length + (self._space - self._length) // 2,
+            y=self.y + self._height + self._height // 2 - (self._height // 16),
+            color_index=1,
+        )
+        self.group.append(value)
+        self._two_points_container.append(value)
 
     def _draw_digits(self, x, pos):
         posx = x
 
         segments = []
 
         # Segment A
@@ -188,36 +235,83 @@
             y=self.y + self._height,
             color_index=1,
         )
         segments.append(value)
         self.group.append(value)
         self._digits[pos] = segments
 
+        value = Circle(
+            pixel_shader=self._palette,
+            radius=self._height // 8,
+            x=posx + self._length + (self._height // 4),
+            y=self.y + 2 * self._height - (self._height // 8),
+            color_index=1,
+        )
+        self.group.append(value)
+
     def print(self, value):
         """
         print the value given. for the time being only works with ints
         """
         self.clear()
+        if ":" in value:
+            value = value.replace(":", "")
+            self._two_points(True)
+
         value_string = str(value)
         for i in range(len(value_string)):
             self.print_digit(i, value_string[len(value_string) - 1 - i])
 
-    def print_digit(self, pos, value):
+    def print_digit(self, pos, char):
         """
-        Prints the desired value in the corresponding position. Works with ints only
+        Print a specific digit
         """
-        character = ord(value) - 48
-        new_value = NUMBERS[character]
+        char = char.lower()
+        if char in "abcdefghijklmnopqrstuvwxy":
+            character = ord(char) - 97 + 10
+        elif char == "-":
+            character = 36
+        elif char in "0123456789":
+            character = ord(char) - 48
+        elif char == "*":
+            character = 37
+
+        if self._chardict and char in self._chardict:
+            new_value = self._chardict[char]
+        else:
+            new_value = NUMBERS[character]
+
         for i in range(7):
             biff = new_value >> i & 1
 
             if biff:
                 self._digits[pos][i].color_index = 2
             else:
                 self._digits[pos][i].color_index = 1
 
     def clear(self):
         """
         Clear the digits
         """
         for i in range(4):
-            self.print_digit(i, "0")
+            self.print_digit(i, "*")
+        self._two_points(False)
+
+    def __setitem__(self, key: int, value: str) -> None:
+        self.print_digit(key, value)
+
+    def _two_points(self, show=True):
+        if show:
+            for i in range(2):
+                self._two_points_container[i].color_index = 2
+        else:
+            for i in range(2):
+                self._two_points_container[i].color_index = 1
+
+    def fill(self, value):
+        """
+        Fill function. to be compatible with the Hardware version
+        of the library
+        """
+        if value:
+            pass
+        self.clear()
```

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/7mwahe.gif` & `circuitpython-display_ht16k33-0.2.1/docs/7mwahe.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png` & `circuitpython-display_ht16k33-0.2.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico` & `circuitpython-display_ht16k33-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/conf.py` & `circuitpython-display_ht16k33-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/examples.rst` & `circuitpython-display_ht16k33-0.2.1/docs/examples.rst`

 * *Files 10% similar despite different names*

```diff
@@ -30,7 +30,16 @@
 --------------------------
 
 Segment countdown example
 
 .. literalinclude:: ../examples/display_ht16k33_segments_count_down.py
     :caption: examples/display_ht16k33_segments_count_down.py
     :lines: 5-
+
+Segment Custom Chars example
+------------------------------
+
+Segment Custom Chats example
+
+.. literalinclude:: ../examples/display_ht16k33_segments_custom_chars.py
+    :caption: examples/display_ht16k33_segments_custom_chars.py
+    :lines: 9-
```

### Comparing `circuitpython-display_ht16k33-0.2.0/docs/font5x8.bin` & `circuitpython-display_ht16k33-0.2.1/docs/font5x8.bin`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_simpletest.py` & `circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_text.py` & `circuitpython-display_ht16k33-0.2.1/examples/display_ht16k33_text.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.2.0/pyproject.toml` & `circuitpython-display_ht16k33-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-display_ht16k33"
 description = "On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices."
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxxy@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33"}
 keywords = [
     "sensor",
```

