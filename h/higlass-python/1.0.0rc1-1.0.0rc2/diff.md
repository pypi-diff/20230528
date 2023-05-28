# Comparing `tmp/higlass_python-1.0.0rc1.tar.gz` & `tmp/higlass_python-1.0.0rc2.tar.gz`

## Comparing `higlass_python-1.0.0rc1.tar` & `higlass_python-1.0.0rc2.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/Makefile
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/README.md
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/build.sh
--rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/conf.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/environment.yml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/examples.rst
--rw-r--r--   0        0        0    17760 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/getting_started.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/index.rst
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/python_api.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/requirements.txt
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/serve.sh
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/_templates/layout.html
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/higlass_theme/navigation.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/higlass_theme/theme.conf
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/higlass_theme/static/higlass.css
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/beditems.png
--rw-r--r--   0        0        0   339723 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/divided-by-track.png
--rw-r--r--   0        0        0   173688 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/eggholder-function.png
--rw-r--r--   0        0        0    19973 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/genome-position-search-box.png
--rw-r--r--   0        0        0   806451 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/geojson-jupyter.png
--rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/jupyter-bigwig.png
--rw-r--r--   0        0        0   253837 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/jupyter-hic-heatmap.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/jupyter-labelled-points.png
--rw-r--r--   0        0        0    36606 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/jupyter-pileup-no-code.png
--rw-r--r--   0        0        0   146248 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/jupyter-pileup-with-code.png
--rw-r--r--   0        0        0   206714 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/remote-hic.png
--rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/docs/img/two-simple-views.png
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/notebooks/Examples.ipynb
--rw-r--r--   0        0        0   297484 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/notebooks/Fuse.ipynb
--rw-r--r--   0        0        0    28183 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/notebooks/Plugin.ipynb
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/notebooks/View_Projection.ipynb
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/__init__.py
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/_display.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/_scale.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/_utils.py
--rw-r--r--   0        0        0    26729 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/api.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/tilesets.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/fuse/__init__.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/fuse/_httpfs.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/server/__init__.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/server/_background_server.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/higlass/server/_provider.py
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/test/test_api.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/test/test_display.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/test/test_scale.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/test/test_utils.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/README.md
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/Makefile
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/README.md
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/build.sh
+-rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/conf.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/environment.yml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/examples.rst
+-rw-r--r--   0        0        0    17760 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/getting_started.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/index.rst
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/python_api.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/requirements.txt
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/serve.sh
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/_templates/layout.html
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/higlass_theme/navigation.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/higlass_theme/theme.conf
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/higlass_theme/static/higlass.css
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/beditems.png
+-rw-r--r--   0        0        0   339723 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/divided-by-track.png
+-rw-r--r--   0        0        0   173688 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/eggholder-function.png
+-rw-r--r--   0        0        0    19973 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/genome-position-search-box.png
+-rw-r--r--   0        0        0   806451 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/geojson-jupyter.png
+-rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/jupyter-bigwig.png
+-rw-r--r--   0        0        0   253837 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/jupyter-hic-heatmap.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/jupyter-labelled-points.png
+-rw-r--r--   0        0        0    36606 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/jupyter-pileup-no-code.png
+-rw-r--r--   0        0        0   146248 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/jupyter-pileup-with-code.png
+-rw-r--r--   0        0        0   206714 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/remote-hic.png
+-rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/docs/img/two-simple-views.png
+-rw-r--r--   0        0        0    13043 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/examples/Examples.ipynb
+-rw-r--r--   0        0        0   297230 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/examples/Fuse.ipynb
+-rw-r--r--   0        0        0    27929 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/examples/Plugin.ipynb
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/examples/View_Projection.ipynb
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/__init__.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/_display.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/_scale.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/_utils.py
+-rw-r--r--   0        0        0    26729 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/api.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/server.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/tilesets.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/fuse/__init__.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/higlass/fuse/_httpfs.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/test/test_api.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/test/test_display.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/test/test_scale.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/test/test_server.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/test/test_utils.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 higlass_python-1.0.0rc2/PKG-INFO
```

### Comparing `higlass_python-1.0.0rc1/CHANGELOG.md` & `higlass_python-1.0.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/.github/workflows/ci.yml` & `higlass_python-1.0.0rc2/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,46 @@
 name: CI
 
 on:
   push:
     branches:
-      - master
+      - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
-    branches: master
+    branches: main
 
 jobs:
   Lint:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "3.x"
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -e .[dev]
-
-    - name: Linting with Ruff
-      run: ruff .
-
-    - name: Formatting with Black
-      run: black --check .
+    - run: |
+        python -m pip install --upgrade hatch
+        hatch run lint
 
   Test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
-
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-
-    - name: Install dependencies
-      run: |
+    - run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
-
-    - name: Test with pytest
-      run: |
         pytest
 
   Release:
     needs: [Lint, Test]
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags')
     steps:
```

### Comparing `higlass_python-1.0.0rc1/.github/workflows/docs.yml` & `higlass_python-1.0.0rc2/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Deploy static content to Pages
 
 on:
   # Runs on pushes targeting the default branch
   push:
-    branches: master
+    branches: main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: read
```

### Comparing `higlass_python-1.0.0rc1/docs/Makefile` & `higlass_python-1.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/README.md` & `higlass_python-1.0.0rc2/docs/README.md`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/conf.py` & `higlass_python-1.0.0rc2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 
 from docutils import nodes
 from docutils.parsers.rst import Directive, directives
-from higlass import __version__
 from pkg_resources import parse_version
 
+from higlass import __version__
+
 # -*- coding: utf-8 -*-
 #
 # higlass documentation build configuration file, created by
 # sphinx-quickstart on Mon Jul  3 16:40:45 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
```

### Comparing `higlass_python-1.0.0rc1/docs/examples.rst` & `higlass_python-1.0.0rc2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/getting_started.rst` & `higlass_python-1.0.0rc2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/index.rst` & `higlass_python-1.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/_templates/layout.html` & `higlass_python-1.0.0rc2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/higlass_theme/static/higlass.css` & `higlass_python-1.0.0rc2/docs/higlass_theme/static/higlass.css`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/beditems.png` & `higlass_python-1.0.0rc2/docs/img/beditems.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/divided-by-track.png` & `higlass_python-1.0.0rc2/docs/img/divided-by-track.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/eggholder-function.png` & `higlass_python-1.0.0rc2/docs/img/eggholder-function.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/genome-position-search-box.png` & `higlass_python-1.0.0rc2/docs/img/genome-position-search-box.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/geojson-jupyter.png` & `higlass_python-1.0.0rc2/docs/img/geojson-jupyter.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/jupyter-bigwig.png` & `higlass_python-1.0.0rc2/docs/img/jupyter-bigwig.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/jupyter-hic-heatmap.png` & `higlass_python-1.0.0rc2/docs/img/jupyter-hic-heatmap.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/jupyter-labelled-points.png` & `higlass_python-1.0.0rc2/docs/img/jupyter-labelled-points.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/jupyter-pileup-no-code.png` & `higlass_python-1.0.0rc2/docs/img/jupyter-pileup-no-code.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/jupyter-pileup-with-code.png` & `higlass_python-1.0.0rc2/docs/img/jupyter-pileup-with-code.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/remote-hic.png` & `higlass_python-1.0.0rc2/docs/img/remote-hic.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/docs/img/two-simple-views.png` & `higlass_python-1.0.0rc2/docs/img/two-simple-views.png`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/notebooks/Examples.ipynb` & `higlass_python-1.0.0rc2/examples/Examples.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995833333333333%*

 * *Differences: {"'cells'": "{1: {'source': ['!pip install --pre higlass-python']}}"}*

```diff
@@ -12,22 +12,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import os\n",
-                "import sys\n",
-                "\n",
-                "# Install if in Google colab notebook\n",
-                "if \"google.colab\" in sys.modules:\n",
-                "    os.system(\n",
-                "        \"python -m pip install --upgrade --force-reinstall git+https://github.com/higlass/higlass-python\"\n",
-                "    )"
+                "!pip install --pre higlass-python"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Synced heatmaps"
```

### Comparing `higlass_python-1.0.0rc1/notebooks/Fuse.ipynb` & `higlass_python-1.0.0rc2/examples/Fuse.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'cells'": "{1: {'source': ['!pip install --pre higlass-python']}}"}*

```diff
@@ -15,22 +15,15 @@
             "execution_count": null,
             "id": "7cf0EOX4ybNo",
             "metadata": {
                 "id": "7cf0EOX4ybNo"
             },
             "outputs": [],
             "source": [
-                "import os\n",
-                "import sys\n",
-                "\n",
-                "# Install if in Google colab notebook\n",
-                "if \"google.colab\" in sys.modules:\n",
-                "    os.system(\n",
-                "        \"python -m pip install --upgrade --force-reinstall git+https://github.com/higlass/higlass-python\"\n",
-                "    )"
+                "!pip install --pre higlass-python"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "H75RFhpI0bdr",
             "metadata": {
```

### Comparing `higlass_python-1.0.0rc1/notebooks/Plugin.ipynb` & `higlass_python-1.0.0rc2/examples/Plugin.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993872549019608%*

 * *Differences: {"'cells'": "{0: {'source': ['!pip install --pre higlass-python']}}"}*

```diff
@@ -3,22 +3,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dc78fb28",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import os\n",
-                "import sys\n",
-                "\n",
-                "# Install if in Google colab notebook\n",
-                "if \"google.colab\" in sys.modules:\n",
-                "    os.system(\n",
-                "        \"python -m pip install --upgrade --force-reinstall git+https://github.com/higlass/higlass-python\"\n",
-                "    )"
+                "!pip install --pre higlass-python"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "113ff05d",
             "metadata": {},
```

### Comparing `higlass_python-1.0.0rc1/notebooks/View_Projection.ipynb` & `higlass_python-1.0.0rc2/examples/View_Projection.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'cells'": "{0: {'source': ['!pip install --pre higlass-python']}}"}*

```diff
@@ -3,22 +3,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d1373f88",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import os\n",
-                "import sys\n",
-                "\n",
-                "# Install if in Google colab notebook\n",
-                "if \"google.colab\" in sys.modules:\n",
-                "    os.system(\n",
-                "        \"python -m pip install --upgrade --force-reinstall git+https://github.com/higlass/higlass-python\"\n",
-                "    )"
+                "!pip install --pre higlass-python"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8ae5be58",
             "metadata": {},
```

### Comparing `higlass_python-1.0.0rc1/higlass/_display.py` & `higlass_python-1.0.0rc2/higlass/_display.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import json
 import uuid
 from dataclasses import dataclass, field
 from typing import Protocol
 
 import jinja2
 
@@ -32,15 +33,15 @@
 </html>
 """  # noqa
 )
 
 
 def viewconf_to_html(
     viewconf: dict,
-    higlass_version: str = "1.11",
+    higlass_version: str = "1.12",
     react_version: str = "17",
     pixijs_version: str = "6",
     output_div: str = "vis",
     json_kwds: dict | None = None,
     plugin_urls: list[str] | None = None,
 ):
     """Embed the viewconf into an HTML template.
@@ -136,14 +137,32 @@
     def __call__(self, viewconf: dict, **metadata):
         kwargs = self.kwargs.copy()
         kwargs.update(metadata)
         html = viewconf_to_html(viewconf=viewconf, output_div=self.output_div, **kwargs)
         return {"text/html": html}
 
 
+@contextlib.contextmanager
+def managed_enable(registry: RendererRegistry, reset: str | None):
+    """Temporarily enables a renderer.
+
+    Parameters
+    ----------
+    registry : PluginRegistry
+        The plugin registry to potentially reset the active plugin.
+
+    reset : str | None
+        The previous name of the active plugin.
+    """
+    try:
+        yield registry.get()
+    finally:
+        registry.active = reset
+
+
 @dataclass
 class RendererRegistry:
     """A registery for multiple HiGlass renderers.
 
     Allows for multiple renders to be registered, and dynamically enabled/disabled
     for the viewconf.
 
@@ -181,15 +200,17 @@
         ----------
 
         name : str
             The name of a previously registered renderer.
         """
         if name not in self.renderers:
             raise ValueError(f"Renderer '{name}' has not been registered.")
+        prev = self.active
         self.active = name
+        return managed_enable(self, prev)
 
     def get(self):
         """Get the enabled renderer."""
         if self.active is None:
             raise ValueError("No renderer enabled.")
         return self.renderers[self.active]
```

### Comparing `higlass_python-1.0.0rc1/higlass/_scale.py` & `higlass_python-1.0.0rc2/higlass/_scale.py`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/higlass/_utils.py` & `higlass_python-1.0.0rc2/higlass/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,14 +47,26 @@
     return str(uuid.uuid4())
 
 
 T = TypeVar("T")
 
 
 def ensure_list(x: T | list[T] | None) -> list[T]:
+    """Ensures that x is a list.
+
+    Parameters
+    ----------
+    x : T | list[T] | None
+        The object to be converted to a list.
+
+    Returns
+    -------
+    list[T]
+        The object as a list.
+    """
     if x is None:
         return []
     return x if isinstance(x, list) else [x]
 
 
 ModelT = TypeVar("ModelT", bound=BaseModel)
```

### Comparing `higlass_python-1.0.0rc1/higlass/api.py` & `higlass_python-1.0.0rc2/higlass/api.py`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/higlass/tilesets.py` & `higlass_python-1.0.0rc2/higlass/tilesets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import functools
 import hashlib
 import pathlib
+import typing
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Literal, Optional, Sequence
 
 from ._utils import TrackType
 from .api import track
 
 __all__ = [
     "LocalTileset",
     "RemoteTileset",
@@ -14,35 +16,48 @@
     "bigwig",
     "multivec",
     "cooler",
     "hitile",
     "bed2ddb",
 ]
 
-TileId = str
-Tile = Dict[str, Any]
-TilesetInfo = Dict[str, Any]
-
-DataType = Literal["vector", "multivec", "matrix"]
+DataType = typing.Literal["vector", "multivec", "matrix"]
 
 
-@dataclass
 class LocalTileset:
-    tiles: Callable[[Sequence[TileId]], List[Tile]]
-    info: Callable[[], TilesetInfo]
-    uid: str
-    datatype: Optional[DataType] = None
-    name: Optional[str] = None
+    def __init__(
+        self,
+        datatype: DataType,
+        tiles: typing.Callable[[typing.Sequence[str]], list[typing.Any]],
+        info: typing.Callable[[], typing.Any],
+        uid: str,
+        name: str | None = None,
+    ):
+        self.datatype = datatype
+        self._tiles = tiles
+        self._info = info
+        self._uid = uid
+        self.name = name
+
+    @property
+    def uid(self) -> str:
+        return self._uid
+
+    def tiles(self, tile_ids: typing.Sequence[str]) -> list[typing.Any]:
+        return self._tiles(tile_ids)
+
+    def info(self) -> typing.Any:
+        return self._info()
 
 
 @dataclass
 class RemoteTileset:
     uid: str
     server: str
-    name: Optional[str] = None
+    name: str | None = None
 
     def track(self, type_: TrackType, **kwargs):
         t = track(
             type_=type_,
             server=self.server,
             tilesetUid=self.uid,
             **kwargs,
@@ -52,16 +67,18 @@
         return t
 
 
 def remote(uid: str, server: str = "https://higlass.io/api/v1", **kwargs):
     return RemoteTileset(uid, server, **kwargs)
 
 
-def hash_absolute_filepath_as_default_uid(fn: Callable[[str, str], LocalTileset]):
-    def wrapper(filepath: str, uid: Optional[str] = None):
+def hash_absolute_filepath_as_default_uid(
+    fn: typing.Callable[[str, str], LocalTileset]
+):
+    def wrapper(filepath: str, uid: None | str = None):
         if uid is None:
             abspath = pathlib.Path(filepath).absolute()
             uid = hashlib.md5(str(abspath).encode()).hexdigest()
         return fn(filepath, uid)
 
     return wrapper
```

### Comparing `higlass_python-1.0.0rc1/higlass/fuse/__init__.py` & `higlass_python-1.0.0rc2/higlass/fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/higlass/fuse/_httpfs.py` & `higlass_python-1.0.0rc2/higlass/fuse/_httpfs.py`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/test/test_api.py` & `higlass_python-1.0.0rc2/test/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-import higlass as hg
 import pytest
 
+import higlass as hg
+
 
 @pytest.mark.parametrize(
     "args,expected",
     [
         ("horizontal-line", hg.EnumTrack),
         ("multivec", hg.EnumTrack),
         ("1d-heatmap", hg.EnumTrack),
```

### Comparing `higlass_python-1.0.0rc1/test/test_display.py` & `higlass_python-1.0.0rc2/test/test_display.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from unittest.mock import MagicMock
+
 import pytest
+
 from higlass._display import HTMLRenderer, RendererRegistry, renderers
 
 
 def test_registry():
     registery = RendererRegistry()
 
     with pytest.raises(ValueError):
@@ -27,14 +30,40 @@
 
     mimebundle = render({})
 
     assert isinstance(mimebundle, dict)
     assert mimebundle["text/plain"] == "some content"
 
 
+def test_temporary_renderer():
+    registry = RendererRegistry()
+    mock = MagicMock()
+
+    def renderer(viewconf: dict, **metadata):
+        return {
+            "text/plain": "some content",
+        }
+
+    registry.register("foo", renderer)
+    registry.register("mock", mock)
+
+    registry.enable("foo")
+
+    with registry.enable("mock") as render:
+        assert registry.active == "mock"
+        render({"hello": "world"})
+
+    mock.assert_called_once_with({"hello": "world"})
+
+    render = registry.get()
+    mimebundle = render({})
+    assert registry.active == "foo"
+    assert mimebundle["text/plain"] == "some content"
+
+
 def test_html_renderer():
     """Just a smoke test to make sure our html gets a unique ID"""
 
     default_renderer = renderers.get()
     assert isinstance(default_renderer, HTMLRenderer)
 
     mimebundle = default_renderer(
```

### Comparing `higlass_python-1.0.0rc1/test/test_scale.py` & `higlass_python-1.0.0rc2/test/test_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from higlass._scale import Scale
 
 
 @pytest.fixture
 def scale():
     chromsizes = [("chr1", 10000), ("chr2", 20000), ("chr3", 30000)]
     binsize = 1000
```

### Comparing `higlass_python-1.0.0rc1/test/test_utils.py` & `higlass_python-1.0.0rc2/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import pytest
-from higlass._utils import copy_unique, ensure_list
 from pydantic import BaseModel
 
+from higlass._utils import copy_unique, ensure_list
+
 
 def test_copy_unique():
     class Person(BaseModel):
         name: str
 
     person = Person(name="foo")
```

### Comparing `higlass_python-1.0.0rc1/LICENSE` & `higlass_python-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `higlass_python-1.0.0rc1/README.md` & `higlass_python-1.0.0rc2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-# higlass-python v2 🔎
+# higlass-python 🔎
 
 a fresh python library for [`higlass`](https://github.com/higlass/higlass) built 
 on top of [`higlass-schema`](https://github.com/higlass/higlass-schema) and
 [`higlass-widget`](https://github.com/higlass/higlass-widget).
 
-[![License](https://img.shields.io/pypi/l/higlass-python.svg?color=green)](https://github.com/higlass/higlass-python/raw/master/LICENSE)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/higlass/higlass-python/blob/main/notebooks/Examples.ipynb)
+[![License](https://img.shields.io/pypi/l/higlass-python.svg?color=green)](https://github.com/higlass/higlass-python/raw/main/LICENSE)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/higlass/higlass-python/blob/main/examples/Examples.ipynb)
 
 ## Usage
 
+> **Note** A release candidate for `higlass-python` v1 is now available on 
+> PyPI and can be installed via pip:
+
+```sh
+pip install --pre higlass-python
+```
+
 ```python
 import higlass as hg
 
 # Remote data source (tileset)
 tileset1 = hg.remote(
     uid="CQMd6V_cRw6iCI_-Unl3PQ",
     server="https://higlass.io/api/v1/",
@@ -35,14 +42,17 @@
 
 # Concatenate views horizontally and apply synchronization lock
 (view1 | view2).locks(view_lock)
 ```
 
 ![Side-by-side Hi-C heatmaps, linked by pan and zoom](https://user-images.githubusercontent.com/24403730/159050305-e6a48f03-fba1-4ff7-8eee-2e9c5c40ef88.gif)
 
+
+To learn more about the new API, check out the [updated documentation](https://higlass.io/higlass-python).
+
 ## Development
 
 **higlass-python** uses [the recommended](https://packaging.python.org/en/latest/flow/#) `hatchling` build-system,
 which is convenient to use via the [`hatch` CLI](https://hatch.pypa.io/latest/). We recommend installing `hatch` 
 globally (e.g., via `pipx`) and running the various commands defined within `pyproject.toml`. `hatch` will take care
 of creating and synchronizing a virtual environment with all dependencies defined in `pyproject.toml`.
```

### Comparing `higlass_python-1.0.0rc1/pyproject.toml` & `higlass_python-1.0.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,20 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 license = { text = "MIT" }
 dynamic = ["version"]
 readme = "README.md"
 dependencies = [
-    "higlass-schema",
-    "higlass-widget",
+    "servir>=0.0.5",
+    "higlass-schema>=0.0.6",
+    "higlass-widget>=0.0.7",
     "jinja2",
-    "portpicker",
-    "uvicorn",
-    "starlette",
-    "jupyter-server-proxy",
+    "jupyter-server-proxy>=3.0",
+    "typing-extensions ; python_version<'3.9'",
 ]
 urls = { homepage = "https://github.com/higlass/higlass-python" }
 
 [project.optional-dependencies]
 dev = [
     "black[jupyter]",
     "pytest",
@@ -92,7 +91,10 @@
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = [
     "F403", # unused-star-used
     "F401", # unused import
 ]
+
+[tool.ruff.isort]
+known-first-party = ["higlass"]
```

### Comparing `higlass_python-1.0.0rc1/PKG-INFO` & `higlass_python-1.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: higlass-python
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Python bindings for HiGlass
 Project-URL: homepage, https://github.com/higlass/higlass-python
 Author-email: Fritz Lekschas <code@lekschas.de>, Nezar Abdennur <nabdennur@gmail.com>, Peter Kerpdjiev <pkerpedjiev@gmail.com>, Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: higlass-schema
-Requires-Dist: higlass-widget
+Requires-Dist: higlass-schema>=0.0.6
+Requires-Dist: higlass-widget>=0.0.7
 Requires-Dist: jinja2
-Requires-Dist: jupyter-server-proxy
-Requires-Dist: portpicker
-Requires-Dist: starlette
-Requires-Dist: uvicorn
+Requires-Dist: jupyter-server-proxy>=3.0
+Requires-Dist: servir>=0.0.5
+Requires-Dist: typing-extensions; python_version < '3.9'
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: markupsafe==2.0.1; extra == 'docs'
@@ -33,25 +32,32 @@
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-js; extra == 'docs'
 Provides-Extra: fuse
 Requires-Dist: fusepy; extra == 'fuse'
 Requires-Dist: simple-httpfs; extra == 'fuse'
 Description-Content-Type: text/markdown
 
-# higlass-python v2 🔎
+# higlass-python 🔎
 
 a fresh python library for [`higlass`](https://github.com/higlass/higlass) built 
 on top of [`higlass-schema`](https://github.com/higlass/higlass-schema) and
 [`higlass-widget`](https://github.com/higlass/higlass-widget).
 
-[![License](https://img.shields.io/pypi/l/higlass-python.svg?color=green)](https://github.com/higlass/higlass-python/raw/master/LICENSE)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/higlass/higlass-python/blob/main/notebooks/Examples.ipynb)
+[![License](https://img.shields.io/pypi/l/higlass-python.svg?color=green)](https://github.com/higlass/higlass-python/raw/main/LICENSE)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/higlass/higlass-python/blob/main/examples/Examples.ipynb)
 
 ## Usage
 
+> **Note** A release candidate for `higlass-python` v1 is now available on 
+> PyPI and can be installed via pip:
+
+```sh
+pip install --pre higlass-python
+```
+
 ```python
 import higlass as hg
 
 # Remote data source (tileset)
 tileset1 = hg.remote(
     uid="CQMd6V_cRw6iCI_-Unl3PQ",
     server="https://higlass.io/api/v1/",
@@ -74,14 +80,17 @@
 
 # Concatenate views horizontally and apply synchronization lock
 (view1 | view2).locks(view_lock)
 ```
 
 ![Side-by-side Hi-C heatmaps, linked by pan and zoom](https://user-images.githubusercontent.com/24403730/159050305-e6a48f03-fba1-4ff7-8eee-2e9c5c40ef88.gif)
 
+
+To learn more about the new API, check out the [updated documentation](https://higlass.io/higlass-python).
+
 ## Development
 
 **higlass-python** uses [the recommended](https://packaging.python.org/en/latest/flow/#) `hatchling` build-system,
 which is convenient to use via the [`hatch` CLI](https://hatch.pypa.io/latest/). We recommend installing `hatch` 
 globally (e.g., via `pipx`) and running the various commands defined within `pyproject.toml`. `hatch` will take care
 of creating and synchronizing a virtual environment with all dependencies defined in `pyproject.toml`.
```

