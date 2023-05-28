# Comparing `tmp/reportlab_qr_code_generator-1.6.0.tar.gz` & `tmp/reportlab_qr_code_generator-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab_qr_code_generator-1.6.0.tar", last modified: Sun Oct 23 08:40:07 2022, max compression
+gzip compressed data, was "reportlab_qr_code_generator-1.7.0.tar", last modified: Sun May 28 10:25:33 2023, max compression
```

## Comparing `reportlab_qr_code_generator-1.6.0.tar` & `reportlab_qr_code_generator-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.996850 reportlab_qr_code_generator-1.6.0/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      128 2022-09-25 12:13:19.000000 reportlab_qr_code_generator-1.6.0/.editorconfig
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.994850 reportlab_qr_code_generator-1.6.0/.github/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.995850 reportlab_qr_code_generator-1.6.0/.github/workflows/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1010 2022-10-02 07:36:52.000000 reportlab_qr_code_generator-1.6.0/.github/workflows/python-package.yml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      137 2022-10-02 13:05:23.000000 reportlab_qr_code_generator-1.6.0/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-09-04 17:05:58.000000 reportlab_qr_code_generator-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-09-04 18:11:42.000000 reportlab_qr_code_generator-1.6.0/.pylintrc
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2018 2022-10-23 08:40:02.000000 reportlab_qr_code_generator-1.6.0/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-09-04 17:04:41.000000 reportlab_qr_code_generator-1.6.0/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      209 2022-10-09 15:26:01.000000 reportlab_qr_code_generator-1.6.0/Makefile
--rw-r--r--   0 mirec     (1000) mirec     (1000)    12883 2022-10-23 08:40:07.996850 reportlab_qr_code_generator-1.6.0/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)    12205 2022-10-23 08:39:46.000000 reportlab_qr_code_generator-1.6.0/README.rst
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1084 2022-10-23 08:40:02.000000 reportlab_qr_code_generator-1.6.0/pyproject.toml
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.995850 reportlab_qr_code_generator-1.6.0/reportlab_qr_code/
--rw-r--r--   0 mirec     (1000) mirec     (1000)    11662 2022-10-23 08:39:46.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5514 2022-10-23 08:39:46.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code/__main__.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.995850 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)    12883 2022-10-23 08:40:07.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      608 2022-10-23 08:40:07.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2022-10-23 08:40:07.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       64 2022-10-23 08:40:07.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2022-10-23 08:40:07.000000 reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/top_level.txt
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.995850 reportlab_qr_code_generator-1.6.0/sample_usage/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      208 2022-10-08 16:28:44.000000 reportlab_qr_code_generator-1.6.0/sample_usage/Makefile
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1087 2022-10-09 10:47:51.000000 reportlab_qr_code_generator-1.6.0/sample_usage/test.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5669 2022-10-08 17:30:00.000000 reportlab_qr_code_generator-1.6.0/sample_usage/test.rml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      372 2022-10-02 13:05:23.000000 reportlab_qr_code_generator-1.6.0/sample_usage/utils.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-10-23 08:40:07.996850 reportlab_qr_code_generator-1.6.0/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-09-04 17:14:53.000000 reportlab_qr_code_generator-1.6.0/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2022-10-23 08:40:07.996850 reportlab_qr_code_generator-1.6.0/tests/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-09-04 16:41:40.000000 reportlab_qr_code_generator-1.6.0/tests/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     6129 2022-10-23 08:39:46.000000 reportlab_qr_code_generator-1.6.0/tests/test_qrcode.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      388 2022-10-09 15:26:01.000000 reportlab_qr_code_generator-1.6.0/tox.ini
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.726022 reportlab_qr_code_generator-1.7.0/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      128 2022-09-25 12:13:19.000000 reportlab_qr_code_generator-1.7.0/.editorconfig
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.724022 reportlab_qr_code_generator-1.7.0/.github/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.725022 reportlab_qr_code_generator-1.7.0/.github/workflows/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1026 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/.github/workflows/python-package.yml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      137 2022-10-02 13:05:23.000000 reportlab_qr_code_generator-1.7.0/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-09-04 17:05:58.000000 reportlab_qr_code_generator-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-09-04 18:11:42.000000 reportlab_qr_code_generator-1.7.0/.pylintrc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2970 2023-05-28 10:25:28.000000 reportlab_qr_code_generator-1.7.0/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-09-04 17:04:41.000000 reportlab_qr_code_generator-1.7.0/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      209 2022-10-09 15:26:01.000000 reportlab_qr_code_generator-1.7.0/Makefile
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    14966 2023-05-28 10:25:33.726022 reportlab_qr_code_generator-1.7.0/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    14288 2023-05-28 10:25:06.000000 reportlab_qr_code_generator-1.7.0/README.rst
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1084 2023-05-28 10:25:28.000000 reportlab_qr_code_generator-1.7.0/pyproject.toml
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.725022 reportlab_qr_code_generator-1.7.0/reportlab_qr_code/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    20468 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     7121 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code/__main__.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.725022 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    14966 2023-05-28 10:25:33.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      632 2023-05-28 10:25:33.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-05-28 10:25:33.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       64 2023-05-28 10:25:33.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2023-05-28 10:25:33.000000 reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/top_level.txt
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.726022 reportlab_qr_code_generator-1.7.0/sample_usage/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      208 2022-10-08 16:28:44.000000 reportlab_qr_code_generator-1.7.0/sample_usage/Makefile
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1151 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/sample_usage/gitlab.svg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1087 2022-12-11 15:34:22.000000 reportlab_qr_code_generator-1.7.0/sample_usage/test.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     6765 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/sample_usage/test.rml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      372 2022-10-02 13:05:23.000000 reportlab_qr_code_generator-1.7.0/sample_usage/utils.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-28 10:25:33.726022 reportlab_qr_code_generator-1.7.0/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-09-04 17:14:53.000000 reportlab_qr_code_generator-1.7.0/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-28 10:25:33.726022 reportlab_qr_code_generator-1.7.0/tests/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-09-04 16:41:40.000000 reportlab_qr_code_generator-1.7.0/tests/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    12325 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/tests/test_qrcode.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      452 2023-05-28 10:21:38.000000 reportlab_qr_code_generator-1.7.0/tox.ini
```

### Comparing `reportlab_qr_code_generator-1.6.0/.github/workflows/python-package.yml` & `reportlab_qr_code_generator-1.7.0/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
 
     - name: Run tox
       run: tox
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v2
+      uses: codecov/codecov-action@v3
       with:
         fail_ci_if_error: true
```

### Comparing `reportlab_qr_code_generator-1.6.0/.pylintrc` & `reportlab_qr_code_generator-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `reportlab_qr_code_generator-1.6.0/CHANGELOG.md` & `reportlab_qr_code_generator-1.7.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,55 @@
+## 1.7.0 (2023-05-28)
+
+### Feat
+
+- Small optimalization - don't do masking if we need draw all
+- Allow draw command with = sign
+- Implemented partial draw for command line
+- Allow hightight align patterns
+- Added alignment pattern calculation
+- Added QR parts masking support
+- Added drawing stack
+- Parsing draw parts
+
+### Fix
+
+- Correctly combine graadients in commandline mode
+- Replaced fixed drawing fragment
+- Correct hole position
+- Don't throw exception without hole parameter
+- Consistent area naming
+- Partial draw fixes
+- Don't parse global and part params exactly same
+
+### Refactor
+
+- Reorganized conditions
+- Removing old commented code
+- Moved color parsing
+
+## 1.6.1 (2023-05-27)
+
+### Feat
+
+- Allow --hole commandline parameter
+- Implemented hole support
+- Implemented area to pixels conversion
+- Added area parsing
+
+### Fix
+
+- Fixed tests
+- Typo
+- Dont allow mixed units in area definition
+
+### Refactor
+
+- Canged Length to dataclass
+
 ## 1.6.0 (2022-10-23)
 
 ### Fix
 
 - Don't open file if arguments are not successfully parsed
 
 ### Feat
```

### Comparing `reportlab_qr_code_generator-1.6.0/LICENSE` & `reportlab_qr_code_generator-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportlab_qr_code_generator-1.6.0/PKG-INFO` & `reportlab_qr_code_generator-1.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-Metadata-Version: 2.1
-Name: reportlab_qr_code_generator
-Version: 1.6.0
-Summary: QR code plugin for reportlab and RML language
-Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/mireq/reportlab-qr-code
-Project-URL: documentation, https://github.com/mireq/reportlab-qr-code
-Project-URL: repository, https://github.com/mireq/reportlab-qr-code
-Project-URL: changelog, https://github.com/mireq/reportlab-qr-code/blob/master/CHANGELOG.md
-Keywords: qr code,rml,reportlab
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 =========================================
 QR code plugin for reportlab RML language
 =========================================
 
 |codecov| |version| |downloads| |license|
 
 Install
 -------
 
 .. code:: bash
 
 	pip install reportlab_qr_code_generator
 
+Example output
+--------------
+
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/custom_style.png?v2023-05-28
+
 Why is this better than x?
 --------------------------
 
 **Including image to PDF**
 
 Images are blurry.
 
@@ -130,14 +118,16 @@
 --bg                  Background color
 --invert              Invert
 --negative            Instead of invert bits, inverts whole image
 --radius              Round code (radius)
 --enhanced-path       Enhanced path rendering
 --no-enhanced-path    Disable path enhancement
 --gradient            Either ``"linear x1 y1 x2 y2 colors"`` or ``"radial x y radius colors"`` Dimensions are in range (0, 1), position (0, 0) is top left corner, (1, 1) is bottom right corner. Colors is list ``"[position] color"`` e.g. ``"0.0 #ffffff 1.0 #000000"``. Position is optional. Without position argument, distances are calculated automatically. Example: ``--gradient "linear 0.0 0.0 0.1 1.0 0.5 \#1050c0 0.3 \#1050c0 0.7 \#e0e000"``
+--hole                Coordinates in form ``x:y:w:h``. Allowed are absolute length units, relative units (%) and pixels (without unit suffix).
+--draw                Select area to draw. Possuble values are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``, ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``, ``'align'``, ``'alignpupils'``, ``'alignballs'``. It's possible to combine operations with +/- symbol e.g. all-eyes-align. To show only eye1 and eye3 without pupil it's possible to write something like ``eye1+eye3-eyepupil3``. Arguments passed before first draw are globally set. Arguments after draw are specific for preceding draw call.
 
 Some crazy examples:
 
 .. code:: bash
 
 	# 1
 	python -m reportlab_qr_code "Padding 1cm" \
@@ -215,14 +205,23 @@
 	  - error_correction passed to qr code library (can be L, M, Q or H)
 	* - ``x``
 	  - 0
 	  - x offset
 	* - ``y``
 	  - 0
 	  - y offset
+	* - ``hole``
+	  - []
+	  - list of holes in form ``x:y:w:h…`` (can be repeated)
+	* - ``draw``
+	  - +all
+	  - select elements to draw. Prefix + (plus) means include, - (minus)
+	    exclude. Allowed options are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``,
+	    ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``,
+	    ``'align'``, ``'alignpupils'`` and ``'alignballs'``
 
 Examples
 --------
 
 Python examle:
 
 .. code:: python
@@ -239,15 +238,14 @@
 	if __name__ == "__main__":
 		main()
 
 RML document example:
 
 .. code:: xml
 
-
 	<!DOCTYPE document SYSTEM "rml_1_0.dtd" [
 	<!ENTITY lines5 "
 		0cm 0cm 0cm 0.5cm
 		0cm 0cm 0.5cm 0cm
 		5cm 0cm 4.5cm 0cm
 		5cm 0cm 5cm 0.5cm
 		0cm 5cm 0.5cm 5cm
@@ -263,26 +261,19 @@
 		0cm 3cm 0.5cm 3cm
 		0cm 3cm 0cm 2.5cm
 		3cm 3cm 3cm 2.5cm
 		3cm 3cm 2.5cm 3cm
 	">
 	]>
 	<document filename="test.pdf" invariant="1" compression="1">
-	<!--
-	<template pagesize="a4">
-		<pageTemplate id="main" pagesize="a4 portrait">
-			<frame id="main" x1="1cm" y1="1cm" width="19cm" height="27.7cm"/>
-		</pageTemplate>
-	</template>
-	-->
 	<template>
-		<pageTemplate id="main" pagesize="17cm,32cm">
-			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="32cm"/>
+		<pageTemplate id="main" pagesize="17cm,39cm">
+			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="39cm"/>
 		</pageTemplate>
 	</template>
 	<stylesheet>
 		<paraStyle name="Normal" fontSize="12" leading="16" spaceBefore="16" />
 	</stylesheet>
 	<story>
 	
@@ -384,15 +375,14 @@
 	
 		<para style="Normal">Large radius</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic module="reportlab_qr_code" function="qr">radius=3.5;text;Large radius</plugInGraphic>
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 		</illustration>
 	
-		<!--
 		<condPageBreak height="7cm"/>
 	
 		<para>Inverted</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 			<plugInGraphic module="reportlab_qr_code" function="qr">padding=0,fg=#ffffff,invert=1;text;Inverted</plugInGraphic>
 			<lineMode width="2" />
@@ -404,22 +394,39 @@
 	
 		<para>Mask</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 			<plugInGraphic module="reportlab_qr_code" function="qr">mask=1,radius=0.5,enhanced_path=1;text;Mask</plugInGraphic>
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 		</illustration>
-		-->
 	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Hole</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">hole=20%:40%:60%:20%,error_correction=H,radius=0.3,enhanced_path=1;text;Hole inside QR code</plugInGraphic>
+			<setFont name="Helvetica" size="18"/>
+			<drawString x="1.8cm" y="2.35cm">Logo</drawString>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+		</illustration>
+	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Logo</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">padding=2,radius=0.5,hole=35%:35%:30%:30%,fg=#554488,error_correction=H,draw=all-align-eyes,draw=alignpupils,radius=0.25,draw=alignballs,fg=#e24329,radius=1,draw=eyeball2+eyeball3,radius=3.5,fg=#fca326,draw=eyeball1,radius=3.5,fg=#e24329,draw=eyepupils,fg=#44366d,radius=3.5;text;https://about.gitlab.com/</plugInGraphic>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+			<image file="gitlab.svg" x="1.8cm" y="1.8cm" width="1.4cm" height="1.4cm"/>
+		</illustration>
 	</story>
 	</document>
 
 Output:
 
-.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2022-10-08
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2023-05-28
 
 
 .. |codecov| image:: https://codecov.io/gh/mireq/reportlab-qr-code/branch/master/graph/badge.svg?token=QGY5B5X0F3
 	:target: https://codecov.io/gh/mireq/reportlab-qr-code
 
 .. |version| image:: https://badge.fury.io/py/reportlab-qr-code-generator.svg
 	:target: https://pypi.python.org/pypi/reportlab-qr-code-generator/
```

### Comparing `reportlab_qr_code_generator-1.6.0/README.rst` & `reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,42 @@
+Metadata-Version: 2.1
+Name: reportlab-qr-code-generator
+Version: 1.7.0
+Summary: QR code plugin for reportlab and RML language
+Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/mireq/reportlab-qr-code
+Project-URL: documentation, https://github.com/mireq/reportlab-qr-code
+Project-URL: repository, https://github.com/mireq/reportlab-qr-code
+Project-URL: changelog, https://github.com/mireq/reportlab-qr-code/blob/master/CHANGELOG.md
+Keywords: qr code,rml,reportlab
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 =========================================
 QR code plugin for reportlab RML language
 =========================================
 
 |codecov| |version| |downloads| |license|
 
 Install
 -------
 
 .. code:: bash
 
 	pip install reportlab_qr_code_generator
 
+Example output
+--------------
+
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/custom_style.png?v2023-05-28
+
 Why is this better than x?
 --------------------------
 
 **Including image to PDF**
 
 Images are blurry.
 
@@ -113,14 +135,16 @@
 --bg                  Background color
 --invert              Invert
 --negative            Instead of invert bits, inverts whole image
 --radius              Round code (radius)
 --enhanced-path       Enhanced path rendering
 --no-enhanced-path    Disable path enhancement
 --gradient            Either ``"linear x1 y1 x2 y2 colors"`` or ``"radial x y radius colors"`` Dimensions are in range (0, 1), position (0, 0) is top left corner, (1, 1) is bottom right corner. Colors is list ``"[position] color"`` e.g. ``"0.0 #ffffff 1.0 #000000"``. Position is optional. Without position argument, distances are calculated automatically. Example: ``--gradient "linear 0.0 0.0 0.1 1.0 0.5 \#1050c0 0.3 \#1050c0 0.7 \#e0e000"``
+--hole                Coordinates in form ``x:y:w:h``. Allowed are absolute length units, relative units (%) and pixels (without unit suffix).
+--draw                Select area to draw. Possuble values are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``, ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``, ``'align'``, ``'alignpupils'``, ``'alignballs'``. It's possible to combine operations with +/- symbol e.g. all-eyes-align. To show only eye1 and eye3 without pupil it's possible to write something like ``eye1+eye3-eyepupil3``. Arguments passed before first draw are globally set. Arguments after draw are specific for preceding draw call.
 
 Some crazy examples:
 
 .. code:: bash
 
 	# 1
 	python -m reportlab_qr_code "Padding 1cm" \
@@ -198,14 +222,23 @@
 	  - error_correction passed to qr code library (can be L, M, Q or H)
 	* - ``x``
 	  - 0
 	  - x offset
 	* - ``y``
 	  - 0
 	  - y offset
+	* - ``hole``
+	  - []
+	  - list of holes in form ``x:y:w:h…`` (can be repeated)
+	* - ``draw``
+	  - +all
+	  - select elements to draw. Prefix + (plus) means include, - (minus)
+	    exclude. Allowed options are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``,
+	    ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``,
+	    ``'align'``, ``'alignpupils'`` and ``'alignballs'``
 
 Examples
 --------
 
 Python examle:
 
 .. code:: python
@@ -222,15 +255,14 @@
 	if __name__ == "__main__":
 		main()
 
 RML document example:
 
 .. code:: xml
 
-
 	<!DOCTYPE document SYSTEM "rml_1_0.dtd" [
 	<!ENTITY lines5 "
 		0cm 0cm 0cm 0.5cm
 		0cm 0cm 0.5cm 0cm
 		5cm 0cm 4.5cm 0cm
 		5cm 0cm 5cm 0.5cm
 		0cm 5cm 0.5cm 5cm
@@ -246,26 +278,19 @@
 		0cm 3cm 0.5cm 3cm
 		0cm 3cm 0cm 2.5cm
 		3cm 3cm 3cm 2.5cm
 		3cm 3cm 2.5cm 3cm
 	">
 	]>
 	<document filename="test.pdf" invariant="1" compression="1">
-	<!--
-	<template pagesize="a4">
-		<pageTemplate id="main" pagesize="a4 portrait">
-			<frame id="main" x1="1cm" y1="1cm" width="19cm" height="27.7cm"/>
-		</pageTemplate>
-	</template>
-	-->
 	<template>
-		<pageTemplate id="main" pagesize="17cm,32cm">
-			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="32cm"/>
+		<pageTemplate id="main" pagesize="17cm,39cm">
+			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="39cm"/>
 		</pageTemplate>
 	</template>
 	<stylesheet>
 		<paraStyle name="Normal" fontSize="12" leading="16" spaceBefore="16" />
 	</stylesheet>
 	<story>
 	
@@ -367,15 +392,14 @@
 	
 		<para style="Normal">Large radius</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic module="reportlab_qr_code" function="qr">radius=3.5;text;Large radius</plugInGraphic>
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 		</illustration>
 	
-		<!--
 		<condPageBreak height="7cm"/>
 	
 		<para>Inverted</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 			<plugInGraphic module="reportlab_qr_code" function="qr">padding=0,fg=#ffffff,invert=1;text;Inverted</plugInGraphic>
 			<lineMode width="2" />
@@ -387,22 +411,39 @@
 	
 		<para>Mask</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 			<plugInGraphic module="reportlab_qr_code" function="qr">mask=1,radius=0.5,enhanced_path=1;text;Mask</plugInGraphic>
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 		</illustration>
-		-->
 	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Hole</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">hole=20%:40%:60%:20%,error_correction=H,radius=0.3,enhanced_path=1;text;Hole inside QR code</plugInGraphic>
+			<setFont name="Helvetica" size="18"/>
+			<drawString x="1.8cm" y="2.35cm">Logo</drawString>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+		</illustration>
+	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Logo</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">padding=2,radius=0.5,hole=35%:35%:30%:30%,fg=#554488,error_correction=H,draw=all-align-eyes,draw=alignpupils,radius=0.25,draw=alignballs,fg=#e24329,radius=1,draw=eyeball2+eyeball3,radius=3.5,fg=#fca326,draw=eyeball1,radius=3.5,fg=#e24329,draw=eyepupils,fg=#44366d,radius=3.5;text;https://about.gitlab.com/</plugInGraphic>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+			<image file="gitlab.svg" x="1.8cm" y="1.8cm" width="1.4cm" height="1.4cm"/>
+		</illustration>
 	</story>
 	</document>
 
 Output:
 
-.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2022-10-08
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2023-05-28
 
 
 .. |codecov| image:: https://codecov.io/gh/mireq/reportlab-qr-code/branch/master/graph/badge.svg?token=QGY5B5X0F3
 	:target: https://codecov.io/gh/mireq/reportlab-qr-code
 
 .. |version| image:: https://badge.fury.io/py/reportlab-qr-code-generator.svg
 	:target: https://pypi.python.org/pypi/reportlab-qr-code-generator/
```

### Comparing `reportlab_qr_code_generator-1.6.0/pyproject.toml` & `reportlab_qr_code_generator-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 [tool.setuptools]
 packages = ["reportlab_qr_code"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.6.0"
+version = "1.7.0"
 tag_format = "$version"
```

### Comparing `reportlab_qr_code_generator-1.6.0/reportlab_qr_code/__main__.py` & `reportlab_qr_code_generator-1.7.0/reportlab_qr_code/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,70 @@
 # -*- coding: utf-8 -*-
 import argparse
 import sys
 from base64 import b64decode
+from copy import deepcopy
 
 from reportlab.pdfgen import canvas
 
 from . import DEFAULT_PARAMS, clean_params, build_qrcode
 
 
-def generate(args):
-	text = args.text
-	if text is None:
-		text = sys.stdin.read()
-	if args.base64:
-		text = b64decode(text)
-
+def generate(text, c, **args):
 	params = DEFAULT_PARAMS.copy()
-	if args.version is not None:
-		params['version'] = args.version
-	if args.error_correction is not None:
-		params['error_correction'] = args.error_correction
-	params['size'] = args.size
-	params['padding'] = args.padding
-	if args.fg is not None:
-		params['fg'] = args.fg
-	if args.bg is not None:
-		params['bg'] = args.bg
-	params['invert'] = bool(args.invert)
-	params['negative'] = bool(args.negative)
-	params['radius'] = args.radius
-	if args.enhanced_path is not None:
-		params['enhanced_path'] = args.enhanced_path
-	if args.gradient:
+	if args['version'] is not None:
+		params['version'] = args['version']
+	if args['error_correction'] is not None:
+		params['error_correction'] = args['error_correction']
+	params['size'] = args['size']
+	params['padding'] = args['padding']
+	if args['fg'] is not None:
+		params['fg'] = args['fg']
+	if args['bg'] is not None:
+		params['bg'] = args['bg']
+	params['invert'] = bool(args['invert'])
+	params['negative'] = bool(args['negative'])
+	params['radius'] = args['radius']
+	if args['hole']:
+		params['hole'] = args['hole']
+	if args['enhanced_path'] is not None:
+		params['enhanced_path'] = args['enhanced_path']
+	if args['gradient']:
 		params['mask'] = True
+	if args['draw'] is not None:
+		params['draw_parts'] = [{'draw': args['draw']}]
 	clean_params(params)
 
 	if isinstance(text, str):
 		text = text.encode('utf-8')
 	qr = build_qrcode(params, text)
 
-	if not args.outfile or args.outfile == '-':
-		fp = sys.stdout.buffer
-	else:
-		fp = open(args.outfile, 'wb')
-
-	try:
-		c = canvas.Canvas(
-			fp,
-			pagesize=(qr.size, qr.size),
-			pageCompression=1 if args.compress else 0
-		)
-		qr.save(c)
-
-		if args.gradient:
-			gradient_type, coords, colors, positions = args.gradient
-			if len(colors) == 1:
-				c.setFillColor(colors[0][1])
-				c.rect(0, 0, qr.size, qr.size, fill=1, stroke=0)
+	c.setPageSize((qr.size, qr.size))
+	c.saveState()
+	qr.save(c)
+
+	if args['gradient']:
+		gradient_type, coords, colors, positions = args['gradient']
+		if len(colors) == 1:
+			c.setFillColor(colors[0][1])
+			c.rect(0, 0, qr.size, qr.size, fill=1, stroke=0)
+		else:
+			if gradient_type == 'linear':
+				coords = [
+					coords[0] * qr.size, (1.0 - coords[1]) * qr.size,
+					coords[2] * qr.size, (1.0 - coords[3]) * qr.size,
+				]
+				c.linearGradient(*coords, colors=colors, positions=positions)
 			else:
-				if gradient_type == 'linear':
-					coords = [
-						coords[0] * qr.size, (1.0 - coords[1]) * qr.size,
-						coords[2] * qr.size, (1.0 - coords[3]) * qr.size,
-					]
-					c.linearGradient(*coords, colors=colors, positions=positions)
-				else:
-					coords = [
-						coords[0] * qr.size, (1.0 - coords[1]) * qr.size,
-						coords[2] * qr.size,
-					]
-					c.radialGradient(*coords, colors=colors, positions=positions)
-
-		c.showPage()
-		c.save()
-	finally:
-		if fp is not sys.stdout.buffer:
-			fp.close()
+				coords = [
+					coords[0] * qr.size, (1.0 - coords[1]) * qr.size,
+					coords[2] * qr.size,
+				]
+				c.radialGradient(*coords, colors=colors, positions=positions)
+	c.restoreState()
 
 
 def parse_gradient(val):
 	try:
 		steps = []
 
 		val = val.split()
@@ -147,14 +132,27 @@
 Either "linear x1 y1 x2 y2 colors" or "radial x y radius colors" Dimensions are
 in range [0, 1], position (0, 0) is top left corner, (1, 1) is bottom right
 corner.
 Colors is list "[position] color" e.g. "0.0 #ffffff 1.0 #000000". Position is
 optional. Without position argument, distances are calculated automatically.
 Example: --gradient "linear 0.0 0.0 0.1 1.0 0.5 \#1050c0 0.3 \#1050c0 0.7 \#e0e000"
 	"""
+	area_help = """
+Coordinates in form x:y:w:h. Allowed are absolute length units, relative units (%%)
+and pixels (without unit suffix).
+"""
+	draw_help = """
+Select area to draw. Possuble values are: 'all', 'eye[1-3]', 'eyes',
+'eyepupil[1-3]', 'eyepupils', 'eyeball[1-3]', 'eyeballs', 'align',
+'alignpupils', 'alignballs'. It's possible to combine operations with +/-
+symbol e.g. all-eyes-align. To show only eye1 and eye3 without pupil it's
+possible to write something like eye1+eye3-eyepupil3. Arguments passed before
+first draw are globally set. Arguments after draw are specific for preceding
+draw call.
+"""
 
 	parser = argparse.ArgumentParser(description="Generate qr code")
 	parser.add_argument('text', nargs='?', type=str, help="Input text or stdin if omitted")
 	parser.add_argument('--outfile', nargs='?', help="Output file or stdout if omitted")
 	parser.add_argument('--base64', action='store_true', help="Base64 encoded text")
 	parser.add_argument('--compress', action='store_true', help="PDF compression (default enabled)")
 	parser.add_argument('--no-compress', dest='compress', action='store_false')
@@ -166,15 +164,60 @@
 	parser.add_argument('--bg', type=str, help="Background color")
 	parser.add_argument('--invert', action='store_true', help="Invert")
 	parser.add_argument('--negative', action='store_true', help="Render negative")
 	parser.add_argument('--radius', type=float, help="Round code (radius)", default=0.0)
 	parser.add_argument('--enhanced-path', action='store_true', help="Enhanced path rendering")
 	parser.add_argument('--no-enhanced-path', dest='enhanced_path', action='store_false')
 	parser.add_argument('--gradient', type=parse_gradient, help=gradient_help)
+	parser.add_argument('--hole', type=str, help=area_help)
+	parser.add_argument('--draw', type=str, help=draw_help)
 	parser.set_defaults(compress=True)
 	parser.set_defaults(enhanced_path=None)
-	args = parser.parse_args()
-	generate(args)
+
+	# split arguments with draw command
+	arg_list = []
+	arg_lists = [arg_list]
+	for arg in sys.argv[1:]:
+		if arg == '--draw' or arg.startswith('--draw='):
+			arg_list = ['--draw']
+			arg_lists.append(arg_list)
+			if arg.startswith('--draw='):
+				arg_list.append(arg[7:])
+		else:
+			arg_list.append(arg)
+
+	base_args = vars(parser.parse_args(arg_lists[0]))
+	text = base_args.pop('text')
+	if text is None:
+		text = sys.stdin.read()
+	if base_args['base64']:
+		text = b64decode(text)
+
+	if not base_args['outfile'] or base_args['outfile'] == '-':
+		output = sys.stdout.buffer
+	else:
+		output = open(base_args['outfile'], 'wb')
+
+	c = canvas.Canvas(
+		output,
+		pageCompression=1 if base_args['compress'] else 0
+	)
+
+	try:
+		if len(arg_lists) == 1:
+			generate(text, c, **base_args)
+		else:
+			for arg_list in arg_lists[1:]:
+				arguments = vars(parser.parse_args(arg_list))
+				arguments.pop('text')
+				args = deepcopy(base_args)
+				args.update(arguments)
+				generate(text, c, **args)
+		c.showPage()
+		c.save()
+	finally:
+		if output is not sys.stdout.buffer:
+			output.close()
 
 
 if __name__ == "__main__":
 	main()
```

### Comparing `reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/PKG-INFO` & `reportlab_qr_code_generator-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reportlab-qr-code-generator
-Version: 1.6.0
+Name: reportlab_qr_code_generator
+Version: 1.7.0
 Summary: QR code plugin for reportlab and RML language
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/reportlab-qr-code
 Project-URL: documentation, https://github.com/mireq/reportlab-qr-code
 Project-URL: repository, https://github.com/mireq/reportlab-qr-code
 Project-URL: changelog, https://github.com/mireq/reportlab-qr-code/blob/master/CHANGELOG.md
@@ -24,14 +24,19 @@
 Install
 -------
 
 .. code:: bash
 
 	pip install reportlab_qr_code_generator
 
+Example output
+--------------
+
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/custom_style.png?v2023-05-28
+
 Why is this better than x?
 --------------------------
 
 **Including image to PDF**
 
 Images are blurry.
 
@@ -130,14 +135,16 @@
 --bg                  Background color
 --invert              Invert
 --negative            Instead of invert bits, inverts whole image
 --radius              Round code (radius)
 --enhanced-path       Enhanced path rendering
 --no-enhanced-path    Disable path enhancement
 --gradient            Either ``"linear x1 y1 x2 y2 colors"`` or ``"radial x y radius colors"`` Dimensions are in range (0, 1), position (0, 0) is top left corner, (1, 1) is bottom right corner. Colors is list ``"[position] color"`` e.g. ``"0.0 #ffffff 1.0 #000000"``. Position is optional. Without position argument, distances are calculated automatically. Example: ``--gradient "linear 0.0 0.0 0.1 1.0 0.5 \#1050c0 0.3 \#1050c0 0.7 \#e0e000"``
+--hole                Coordinates in form ``x:y:w:h``. Allowed are absolute length units, relative units (%) and pixels (without unit suffix).
+--draw                Select area to draw. Possuble values are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``, ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``, ``'align'``, ``'alignpupils'``, ``'alignballs'``. It's possible to combine operations with +/- symbol e.g. all-eyes-align. To show only eye1 and eye3 without pupil it's possible to write something like ``eye1+eye3-eyepupil3``. Arguments passed before first draw are globally set. Arguments after draw are specific for preceding draw call.
 
 Some crazy examples:
 
 .. code:: bash
 
 	# 1
 	python -m reportlab_qr_code "Padding 1cm" \
@@ -215,14 +222,23 @@
 	  - error_correction passed to qr code library (can be L, M, Q or H)
 	* - ``x``
 	  - 0
 	  - x offset
 	* - ``y``
 	  - 0
 	  - y offset
+	* - ``hole``
+	  - []
+	  - list of holes in form ``x:y:w:h…`` (can be repeated)
+	* - ``draw``
+	  - +all
+	  - select elements to draw. Prefix + (plus) means include, - (minus)
+	    exclude. Allowed options are: ``'all'``, ``'eye[1-3]'``, ``'eyes'``,
+	    ``'eyepupil[1-3]'``, ``'eyepupils'``, ``'eyeball[1-3]'``, ``'eyeballs'``,
+	    ``'align'``, ``'alignpupils'`` and ``'alignballs'``
 
 Examples
 --------
 
 Python examle:
 
 .. code:: python
@@ -239,15 +255,14 @@
 	if __name__ == "__main__":
 		main()
 
 RML document example:
 
 .. code:: xml
 
-
 	<!DOCTYPE document SYSTEM "rml_1_0.dtd" [
 	<!ENTITY lines5 "
 		0cm 0cm 0cm 0.5cm
 		0cm 0cm 0.5cm 0cm
 		5cm 0cm 4.5cm 0cm
 		5cm 0cm 5cm 0.5cm
 		0cm 5cm 0.5cm 5cm
@@ -263,26 +278,19 @@
 		0cm 3cm 0.5cm 3cm
 		0cm 3cm 0cm 2.5cm
 		3cm 3cm 3cm 2.5cm
 		3cm 3cm 2.5cm 3cm
 	">
 	]>
 	<document filename="test.pdf" invariant="1" compression="1">
-	<!--
-	<template pagesize="a4">
-		<pageTemplate id="main" pagesize="a4 portrait">
-			<frame id="main" x1="1cm" y1="1cm" width="19cm" height="27.7cm"/>
-		</pageTemplate>
-	</template>
-	-->
 	<template>
-		<pageTemplate id="main" pagesize="17cm,32cm">
-			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="32cm"/>
-			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="32cm"/>
+		<pageTemplate id="main" pagesize="17cm,39cm">
+			<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="39cm"/>
+			<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="39cm"/>
 		</pageTemplate>
 	</template>
 	<stylesheet>
 		<paraStyle name="Normal" fontSize="12" leading="16" spaceBefore="16" />
 	</stylesheet>
 	<story>
 	
@@ -384,15 +392,14 @@
 	
 		<para style="Normal">Large radius</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic module="reportlab_qr_code" function="qr">radius=3.5;text;Large radius</plugInGraphic>
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 		</illustration>
 	
-		<!--
 		<condPageBreak height="7cm"/>
 	
 		<para>Inverted</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 			<plugInGraphic module="reportlab_qr_code" function="qr">padding=0,fg=#ffffff,invert=1;text;Inverted</plugInGraphic>
 			<lineMode width="2" />
@@ -404,22 +411,39 @@
 	
 		<para>Mask</para>
 		<illustration height="5cm" width="5cm" align="center">
 			<lineMode width="0.5" /><lines>&lines5;</lines>
 			<plugInGraphic module="reportlab_qr_code" function="qr">mask=1,radius=0.5,enhanced_path=1;text;Mask</plugInGraphic>
 			<plugInGraphic baseDir="." module="utils" function="gradient" />
 		</illustration>
-		-->
 	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Hole</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">hole=20%:40%:60%:20%,error_correction=H,radius=0.3,enhanced_path=1;text;Hole inside QR code</plugInGraphic>
+			<setFont name="Helvetica" size="18"/>
+			<drawString x="1.8cm" y="2.35cm">Logo</drawString>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+		</illustration>
+	
+		<condPageBreak height="7cm"/>
+	
+		<para style="Normal">Logo</para>
+		<illustration height="5cm" width="5cm" align="center">
+			<plugInGraphic module="reportlab_qr_code" function="qr">padding=2,radius=0.5,hole=35%:35%:30%:30%,fg=#554488,error_correction=H,draw=all-align-eyes,draw=alignpupils,radius=0.25,draw=alignballs,fg=#e24329,radius=1,draw=eyeball2+eyeball3,radius=3.5,fg=#fca326,draw=eyeball1,radius=3.5,fg=#e24329,draw=eyepupils,fg=#44366d,radius=3.5;text;https://about.gitlab.com/</plugInGraphic>
+			<lineMode width="0.5" /><lines>&lines5;</lines>
+			<image file="gitlab.svg" x="1.8cm" y="1.8cm" width="1.4cm" height="1.4cm"/>
+		</illustration>
 	</story>
 	</document>
 
 Output:
 
-.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2022-10-08
+.. image:: https://raw.github.com/wiki/mireq/reportlab-qr-code/codes.png?v2023-05-28
 
 
 .. |codecov| image:: https://codecov.io/gh/mireq/reportlab-qr-code/branch/master/graph/badge.svg?token=QGY5B5X0F3
 	:target: https://codecov.io/gh/mireq/reportlab-qr-code
 
 .. |version| image:: https://badge.fury.io/py/reportlab-qr-code-generator.svg
 	:target: https://pypi.python.org/pypi/reportlab-qr-code-generator/
```

### Comparing `reportlab_qr_code_generator-1.6.0/reportlab_qr_code_generator.egg-info/SOURCES.txt` & `reportlab_qr_code_generator-1.7.0/reportlab_qr_code_generator.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 reportlab_qr_code/__main__.py
 reportlab_qr_code_generator.egg-info/PKG-INFO
 reportlab_qr_code_generator.egg-info/SOURCES.txt
 reportlab_qr_code_generator.egg-info/dependency_links.txt
 reportlab_qr_code_generator.egg-info/requires.txt
 reportlab_qr_code_generator.egg-info/top_level.txt
 sample_usage/Makefile
+sample_usage/gitlab.svg
 sample_usage/test.py
 sample_usage/test.rml
 sample_usage/utils.py
 tests/__init__.py
 tests/test_qrcode.py
```

### Comparing `reportlab_qr_code_generator-1.6.0/sample_usage/test.py` & `reportlab_qr_code_generator-1.7.0/sample_usage/test.py`

 * *Files identical despite different names*

### Comparing `reportlab_qr_code_generator-1.6.0/sample_usage/test.rml` & `reportlab_qr_code_generator-1.7.0/sample_usage/test.rml`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 <template pagesize="a4">
 	<pageTemplate id="main" pagesize="a4 portrait">
 		<frame id="main" x1="1cm" y1="1cm" width="19cm" height="27.7cm"/>
 	</pageTemplate>
 </template>
 -->
 <template>
-	<pageTemplate id="main" pagesize="17cm,32cm">
-		<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="32cm"/>
-		<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="32cm"/>
-		<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="32cm"/>
+	<pageTemplate id="main" pagesize="17cm,39cm">
+		<frame id="main" x1="0.5cm" y1="0.0cm" width="5cm" height="39cm"/>
+		<frame id="main" x1="6cm" y1="0.0cm" width="5cm" height="39cm"/>
+		<frame id="main" x1="11.5cm" y1="0.0cm" width="5cm" height="39cm"/>
 	</pageTemplate>
 </template>
 <stylesheet>
 	<paraStyle name="Normal" fontSize="12" leading="16" spaceBefore="16" />
 </stylesheet>
 <story>
 
@@ -158,9 +158,27 @@
 	<para>Mask</para>
 	<illustration height="5cm" width="5cm" align="center">
 		<lineMode width="0.5" /><lines>&lines5;</lines>
 		<plugInGraphic module="reportlab_qr_code" function="qr">mask=1,radius=0.5,enhanced_path=1;text;Mask</plugInGraphic>
 		<plugInGraphic baseDir="." module="utils" function="gradient" />
 	</illustration>
 
+	<condPageBreak height="7cm"/>
+
+	<para style="Normal">Hole</para>
+	<illustration height="5cm" width="5cm" align="center">
+		<plugInGraphic module="reportlab_qr_code" function="qr">hole=20%:40%:60%:20%,error_correction=H,radius=0.3,enhanced_path=1;text;Hole inside QR code</plugInGraphic>
+		<setFont name="Helvetica" size="18"/>
+		<drawString x="1.8cm" y="2.35cm">Logo</drawString>
+		<lineMode width="0.5" /><lines>&lines5;</lines>
+	</illustration>
+
+	<condPageBreak height="7cm"/>
+
+	<para style="Normal">Logo</para>
+	<illustration height="5cm" width="5cm" align="center">
+		<plugInGraphic module="reportlab_qr_code" function="qr">padding=2,radius=0.5,hole=35%:35%:30%:30%,fg=#554488,error_correction=H,draw=all-align-eyes,draw=alignpupils,radius=0.25,draw=alignballs,fg=#e24329,radius=1,draw=eyeball2+eyeball3,radius=3.5,fg=#fca326,draw=eyeball1,radius=3.5,fg=#e24329,draw=eyepupils,fg=#44366d,radius=3.5;text;https://about.gitlab.com/</plugInGraphic>
+		<lineMode width="0.5" /><lines>&lines5;</lines>
+		<image file="gitlab.svg" x="1.8cm" y="1.8cm" width="1.4cm" height="1.4cm"/>
+	</illustration>
 </story>
 </document>
```

