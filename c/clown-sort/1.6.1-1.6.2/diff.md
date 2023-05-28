# Comparing `tmp/clown_sort-1.6.1.tar.gz` & `tmp/clown_sort-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.6.1.tar", max compression
+gzip compressed data, was "clown_sort-1.6.2.tar", max compression
```

## Comparing `clown_sort-1.6.1.tar` & `clown_sort-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2756 2023-05-27 22:18:56.661312 clown_sort-1.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.1/LICENSE
--rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.6.1/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     7834 2023-05-27 22:08:21.966625 clown_sort-1.6.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.6.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.6.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3276 2023-05-27 21:44:44.872765 clown_sort-1.6.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9634 2023-05-27 21:44:44.873210 clown_sort-1.6.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-05-27 22:18:56.667610 clown_sort-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 clown_sort-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2840 2023-05-28 21:14:51.544578 clown_sort-1.6.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.2/LICENSE
+-rw-r--r--   0        0        0     8340 2023-05-28 21:13:57.663794 clown_sort-1.6.2/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.2/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.2/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.6.2/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.2/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.2/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.6.2/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3276 2023-05-27 21:44:44.872765 clown_sort-1.6.2/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9634 2023-05-27 21:44:44.873210 clown_sort-1.6.2/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.2/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.2/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.2/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.2/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.2/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.2/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.2/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-05-28 21:14:51.549471 clown_sort-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9762 1970-01-01 00:00:00.000000 clown_sort-1.6.2/PKG-INFO
```

### Comparing `clown_sort-1.6.1/CHANGELOG.md` & `clown_sort-1.6.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # NEXT RELEASE
 
+### 1.6.2
+* Add `--force` and `[gui,pdf]` to the `pipx` installation instructions
+
 ### 1.6.1
 * Make the brackets print in the optional package install instructions
 * Only check for `pymupdf` once
 
 ## 1.6.0
 * PDF previews in manual sorting windows
 
 ### 1.5.2
 * Override premature release
 
 ### 1.5.1
 * Fix the install messages for missing packages
 
-# 1.5.0
+## 1.5.0
 * Combobox instead of radio buttons for manual fallback directory select
 * Replace fewer special characters in filenames
 * New default crypto sort rules
 
 ### 1.4.1
 * Make --manual-fallback and --only-if-match mutually exclusive
 * New default crypto sort rules
```

### Comparing `clown_sort-1.6.1/LICENSE` & `clown_sort-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/README.md` & `clown_sort-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 * Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.
 
 ## Quick Start
 ```sh
 # Installation with pipx is preferred if you have it but you can also use pip which comes standard
 # on almost all systems. pipx is only a noticeably better answer if you're a python programmer who
 # is concerned about side effects of pip upgrading system python packages.
-pip install clown_sort
+pip install clown_sort[gui,pdf]
 
 # Get help
 sort_screenshots -h
 
 # Dry run with default cryptocurrency sort rules (dry runs don't actually move anything,
 # they just show you what will happen if you run again with the --execute flag)
 sort_screenshots
@@ -61,19 +61,27 @@
 
 # Sort all but put up the manual folder / filename selector window if file doesn't match any sort rules
 sort_screenshots -a -mf -e
 ```
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
-```
-pipx install clown_sort
+
+```sh
+# Install with all packages including GUI and PDF handlers:
+pipx install 'clown_sort[gui,pdf]'
+
+# Install with optional GUI packages (required for --manual-fallback and --manual-sort options):
+pipx install 'clown_sort[gui]' --force
+
+# Install the minimal setup (no GUI, no encrypted PDF parsing):
+pipx install 'clown_sort'
 ```
 
-Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pdf]`.
+Some (not many) PDFs require the `pycryptodome` package to be parsed. This is installed when you install `clown_sort[pdf]`. If you don't install it these PDFS will not have their contents parsed and only the filename will be used for sorting.
 
 Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
```

### Comparing `clown_sort-1.6.1/clown_sort/__init__.py` & `clown_sort-1.6.2/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/config.py` & `clown_sort-1.6.2/clown_sort/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,17 +182,16 @@
         msg.append(
             ': PySimpleGUI package must be installed before you can use the manual selector. Try running:',
             style='bright_white'
         )
 
         log_optional_module_warning('gui', msg)
         console = Console()
-        console.line()
-        console.print(f"You make also need to install 'python-tk'.")
-        console.print("In macOS this can be installed with 'brew install python-tk'.")
+        #console.line()
+        console.print(f"You make also need to install 'python-tk'. In macOS this can be installed with 'brew install python-tk'.")
         sys.exit()
 
 
 def check_for_pymupdf() -> bool:
     try:
         import fitz
         return True
@@ -210,10 +209,10 @@
             style='bright_white'
         )
 
     console = Console()
     console.line()
     console.print(msg)
     console.line()
-    console.print(f"     pipx install clown_sort\[{module_name}]", style='bright_cyan')
+    console.print(f"     pipx install clown_sort\[{module_name}] --force", style='bright_cyan')
     console.line()
-    console.print(f"(or 'poetry install --all-extras' if you're in a development environment)")
+    console.print(f"'pip install' works if you're not using pipx. Use 'poetry install --all-extras' if you're in a development environment.")
```

### Comparing `clown_sort-1.6.1/clown_sort/filename_extractor.py` & `clown_sort-1.6.2/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/files/image_file.py` & `clown_sort-1.6.2/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/files/pdf_file.py` & `clown_sort-1.6.2/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/files/sortable_file.py` & `clown_sort-1.6.2/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/sort_selector.py` & `clown_sort-1.6.2/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.6.2/clown_sort/sorting_rules/crypto.csv`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/util/argument_parser.py` & `clown_sort-1.6.2/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/util/constants.py` & `clown_sort-1.6.2/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.6.2/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/util/rich_helper.py` & `clown_sort-1.6.2/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/clown_sort/util/string_helper.py` & `clown_sort-1.6.2/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.1/pyproject.toml` & `clown_sort-1.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.6.1"
+version = "1.6.2"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.6.1/PKG-INFO` & `clown_sort-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.6.1
+Version: 1.6.2
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,15 @@
 * Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.
 
 ## Quick Start
 ```sh
 # Installation with pipx is preferred if you have it but you can also use pip which comes standard
 # on almost all systems. pipx is only a noticeably better answer if you're a python programmer who
 # is concerned about side effects of pip upgrading system python packages.
-pip install clown_sort
+pip install clown_sort[gui,pdf]
 
 # Get help
 sort_screenshots -h
 
 # Dry run with default cryptocurrency sort rules (dry runs don't actually move anything,
 # they just show you what will happen if you run again with the --execute flag)
 sort_screenshots
@@ -94,19 +94,27 @@
 
 # Sort all but put up the manual folder / filename selector window if file doesn't match any sort rules
 sort_screenshots -a -mf -e
 ```
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
-```
-pipx install clown_sort
+
+```sh
+# Install with all packages including GUI and PDF handlers:
+pipx install 'clown_sort[gui,pdf]'
+
+# Install with optional GUI packages (required for --manual-fallback and --manual-sort options):
+pipx install 'clown_sort[gui]' --force
+
+# Install the minimal setup (no GUI, no encrypted PDF parsing):
+pipx install 'clown_sort'
 ```
 
-Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pdf]`.
+Some (not many) PDFs require the `pycryptodome` package to be parsed. This is installed when you install `clown_sort[pdf]`. If you don't install it these PDFS will not have their contents parsed and only the filename will be used for sorting.
 
 Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
```

