# Comparing `tmp/clown_sort-1.6.0.tar.gz` & `tmp/clown_sort-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.6.0.tar", max compression
+gzip compressed data, was "clown_sort-1.6.1.tar", max compression
```

## Comparing `clown_sort-1.6.0.tar` & `clown_sort-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2642 2023-05-27 21:45:05.298554 clown_sort-1.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.0/LICENSE
--rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.6.0/README.md
--rw-r--r--   0        0        0     3328 2023-05-27 21:44:44.872061 clown_sort-1.6.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     7615 2023-05-27 20:45:42.054203 clown_sort-1.6.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.6.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1802 2023-05-27 21:44:44.872422 clown_sort-1.6.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.6.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3276 2023-05-27 21:44:44.872765 clown_sort-1.6.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9634 2023-05-27 21:44:44.873210 clown_sort-1.6.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.6.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-05-27 21:44:59.464813 clown_sort-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 clown_sort-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2756 2023-05-27 22:18:56.661312 clown_sort-1.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.1/LICENSE
+-rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.6.1/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7834 2023-05-27 22:08:21.966625 clown_sort-1.6.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.6.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     2199 2023-05-27 22:17:44.883449 clown_sort-1.6.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.6.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3276 2023-05-27 21:44:44.872765 clown_sort-1.6.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9634 2023-05-27 21:44:44.873210 clown_sort-1.6.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.6.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-05-27 22:18:56.667610 clown_sort-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 clown_sort-1.6.1/PKG-INFO
```

### Comparing `clown_sort-1.6.0/CHANGELOG.md` & `clown_sort-1.6.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+### 1.6.1
+* Make the brackets print in the optional package install instructions
+* Only check for `pymupdf` once
+
 ## 1.6.0
 * PDF previews in manual sorting windows
 
 ### 1.5.2
 * Override premature release
 
 ### 1.5.1
```

### Comparing `clown_sort-1.6.0/LICENSE` & `clown_sort-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/README.md` & `clown_sort-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/__init__.py` & `clown_sort-1.6.1/clown_sort/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # load_dotenv() should be called as soon as possible (before parsing local classes) but not for pytest
 if not environ.get('INVOKED_BY_PYTEST', False):
     for dotenv_file in [path.join(dir, '.clown_sort') for dir in [getcwd(), Path.home()]]:
         if path.exists(dotenv_file):
             load_dotenv(dotenv_path=dotenv_file)
             break
 
-from clown_sort.config import Config
+from clown_sort.config import Config, check_for_pymupdf
 from clown_sort.files.image_file import ImageFile
 from clown_sort.files.pdf_file import PdfFile
 from clown_sort.files.sortable_file import SortableFile
 from clown_sort.sort_selector import process_file_with_popup
 from clown_sort.util.filesystem_helper import (IMAGE_FILE_EXTENSIONS, files_in_dir, is_image,
       is_pdf, set_timestamp_based_on_screenshot_filename)
 from clown_sort.util.logging import log
@@ -26,23 +26,22 @@
 def sort_screenshots():
     Config.configure()
 
     if Config.rescan_sorted:
         _rescan_sorted_screenshots()
         return
 
-    for image in screenshot_paths(Config.screenshots_dir):
+    for file_to_sort in screenshot_paths(Config.screenshots_dir):
         if Config.manual_sort:
-            if not isinstance(image, (ImageFile, PdfFile)):
-                print(f"'{image.file_path}' is not suitable for manual sort, skipping...")
-                continue
-
-            process_file_with_popup(image)
+            if file_to_sort._can_be_presented_in_popup():
+                process_file_with_popup(file_to_sort)
+            else:
+                print(f"'{file_to_sort.file_path}' is not suitable for manual sort, skipping...")
         else:
-            image.sort_file()
+            file_to_sort.sort_file()
 
 
 def set_screenshot_timestamps():
     Config.configure()
 
     for image in screenshot_paths(Config.screenshots_dir):
         set_timestamp_based_on_screenshot_filename(image.file_path)
```

### Comparing `clown_sort-1.6.0/clown_sort/config.py` & `clown_sort-1.6.1/clown_sort/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,37 +173,47 @@
         log.debug(f"processed_screenshots_dir: {cls.processed_screenshots_dir}")
 
 
 def _check_for_pysimplegui():
     try:
         import PySimpleGUI as sg
     except ModuleNotFoundError:
-        msg = Text('ERROR: ', style='bright_red')
+        msg = Text('ERROR', style='bright_red')
 
         msg.append(
-            'PySimpleGUI package must be installed before you can use the manual selector. Try running:',
+            ': PySimpleGUI package must be installed before you can use the manual selector. Try running:',
             style='bright_white'
         )
 
         log_optional_module_warning('gui', msg)
+        console = Console()
+        console.line()
+        console.print(f"You make also need to install 'python-tk'.")
+        console.print("In macOS this can be installed with 'brew install python-tk'.")
         sys.exit()
 
 
+def check_for_pymupdf() -> bool:
+    try:
+        import fitz
+        return True
+    except ModuleNotFoundError:
+        log_optional_module_warning('pdf')
+        return False
+
+
 # TODO: it sucks that this is here but it's dependency hell otherwise
 def log_optional_module_warning(module_name: str, msg: Optional[Text] = None) -> None:
     """msg is optional argument for a custom message, otherwise it's a warning"""
     if msg is None:
-        msg = Text('WARNING: ', style='bright_red').append(
-            f"Optional package '{module_name}' not installed. . Try running:",
+        msg = Text('WARNING', style='bright_red').append(
+            f": Optional package '{module_name}' not installed. Try running:",
             style='bright_white'
         )
 
     console = Console()
     console.line()
     console.print(msg)
     console.line()
-    console.print(f"     pipx install clown_sort[{module_name}]", style='bright_cyan')
+    console.print(f"     pipx install clown_sort\[{module_name}]", style='bright_cyan')
     console.line()
     console.print(f"(or 'poetry install --all-extras' if you're in a development environment)")
-    console.line()
-    console.print(f"You make also need to install 'python-tk'.")
-    console.print("In macOS this can be installed with 'brew install python-tk'.")
```

### Comparing `clown_sort-1.6.0/clown_sort/filename_extractor.py` & `clown_sort-1.6.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/files/image_file.py` & `clown_sort-1.6.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/files/sortable_file.py` & `clown_sort-1.6.1/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/sort_selector.py` & `clown_sort-1.6.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.6.1/clown_sort/sorting_rules/crypto.csv`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/util/argument_parser.py` & `clown_sort-1.6.1/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/util/constants.py` & `clown_sort-1.6.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.6.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/clown_sort/util/rich_helper.py` & `clown_sort-1.6.1/clown_sort/util/rich_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from rich.theme import Theme
 
 from clown_sort.config import Config
 
 ARROW_BULLET = '➤ '
 INDENTED_BULLET = f"  {ARROW_BULLET}"
 NOT = Text('').append('(Not) ', style='dim')
+WARNING = Text('').append('WARNING', style='bright_yellow').append(': ')
 
 ### Printing ###
 BYTES = 'color(100) dim'
 BYTES_NO_DIM = 'color(100)'
 BYTES_BRIGHTEST = 'color(220)'
 BYTES_BRIGHTER = 'orange1'
 BYTES_HIGHLIGHT = 'color(136)'
```

### Comparing `clown_sort-1.6.0/clown_sort/util/string_helper.py` & `clown_sort-1.6.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.0/pyproject.toml` & `clown_sort-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.6.0"
+version = "1.6.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.6.0/PKG-INFO` & `clown_sort-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.6.0
+Version: 1.6.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

