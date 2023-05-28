# Comparing `tmp/whats_that_code-0.1.9.tar.gz` & `tmp/whats_that_code-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whats_that_code-0.1.9.tar", last modified: Sat Jan 23 17:05:30 2021, max compression
+gzip compressed data, was "whats_that_code-0.2.0.tar", max compression
```

## Comparing `whats_that_code-0.1.9.tar` & `whats_that_code-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1092 2020-12-20 17:22:38.829000 whats_that_code-0.1.9/LICENSE
--rw-r--r--   0        0        0     3081 2021-01-23 17:05:27.456377 whats_that_code-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1926 2021-01-17 16:52:29.430395 whats_that_code-0.1.9/README.md
--rw-r--r--   0        0        0        0 2021-01-03 15:10:37.118000 whats_that_code-0.1.9/whats_that_code/__init__.py
--rw-r--r--   0        0        0      871 2021-01-17 16:37:19.536151 whats_that_code-0.1.9/whats_that_code/__main__.py
--rw-r--r--   0        0        0       93 2021-01-17 18:26:46.656171 whats_that_code-0.1.9/whats_that_code/_version.py
--rw-r--r--   0        0        0    16440 2021-01-18 01:19:51.714757 whats_that_code-0.1.9/whats_that_code/codex_markers.py
--rw-r--r--   0        0        0        0 2021-01-18 13:07:09.172671 whats_that_code-0.1.9/whats_that_code/commands/__init__.py
--rw-r--r--   0        0        0     4757 2021-01-23 16:28:48.383925 whats_that_code-0.1.9/whats_that_code/election.py
--rw-r--r--   0        0        0      912 2021-01-17 15:20:04.261102 whats_that_code-0.1.9/whats_that_code/extension_based.py
--rw-r--r--   0        0        0      643 2021-01-17 15:20:04.096106 whats_that_code-0.1.9/whats_that_code/guess_by_code_and_tags.py
--rw-r--r--   0        0        0      458 2021-01-18 01:23:53.835905 whats_that_code-0.1.9/whats_that_code/guess_by_popularity.py
--rw-r--r--   0        0        0    44381 2021-01-18 01:23:55.680903 whats_that_code-0.1.9/whats_that_code/keyword_based.py
--rw-r--r--   0        0        0    15784 2021-01-23 15:59:10.781196 whats_that_code-0.1.9/whats_that_code/known_languages.py
--rw-r--r--   0        0        0     1751 2021-01-17 04:39:11.242959 whats_that_code-0.1.9/whats_that_code/parsing_based.py
--rw-r--r--   0        0        0     1657 2021-01-17 18:26:21.561736 whats_that_code-0.1.9/whats_that_code/pygments_based.py
--rw-r--r--   0        0        0      981 2021-01-17 15:20:04.215102 whats_that_code-0.1.9/whats_that_code/regex_based.py
--rw-r--r--   0        0        0     1685 2021-01-17 15:20:04.232103 whats_that_code-0.1.9/whats_that_code/shebang_based.py
--rw-r--r--   0        0        0     1251 2021-01-23 17:00:15.783905 whats_that_code-0.1.9/whats_that_code/tag_based.py
--rw-r--r--   0        0        0   237444 2021-01-19 00:18:54.612878 whats_that_code-0.1.9/whats_that_code/tags_data.py
--rw-r--r--   0        0        0     2727 2021-01-23 17:05:31.979378 whats_that_code-0.1.9/setup.py
--rw-r--r--   0        0        0     3217 2021-01-23 17:05:31.980378 whats_that_code-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-28 20:35:30.767053 whats_that_code-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2532 2023-05-28 20:35:30.767053 whats_that_code-0.2.0/README.md
+-rw-r--r--   0        0        0     3025 2023-05-28 20:35:30.767053 whats_that_code-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/__main__.py
+-rw-r--r--   0        0        0       93 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/_version.py
+-rw-r--r--   0        0        0    16440 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/codex_markers.py
+-rw-r--r--   0        0        0        0 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/commands/__init__.py
+-rw-r--r--   0        0        0     4757 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/election.py
+-rw-r--r--   0        0        0     1032 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/extension_based.py
+-rw-r--r--   0        0        0      643 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/guess_by_code_and_tags.py
+-rw-r--r--   0        0        0      504 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/guess_by_popularity.py
+-rw-r--r--   0        0        0    44381 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/keyword_based.py
+-rw-r--r--   0        0        0    15784 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/known_languages.py
+-rw-r--r--   0        0        0     1751 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/parsing_based.py
+-rw-r--r--   0        0        0     1657 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/pygments_based.py
+-rw-r--r--   0        0        0      981 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/regex_based.py
+-rw-r--r--   0        0        0     1685 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/shebang_based.py
+-rw-r--r--   0        0        0     1251 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/tag_based.py
+-rw-r--r--   0        0        0   237444 2023-05-28 20:35:30.771053 whats_that_code-0.2.0/whats_that_code/tags_data.py
+-rw-r--r--   0        0        0     3976 1970-01-01 00:00:00.000000 whats_that_code-0.2.0/PKG-INFO
```

### Comparing `whats_that_code-0.1.9/LICENSE` & `whats_that_code-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Matthew Martin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Matthew Martin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `whats_that_code-0.1.9/README.md` & `whats_that_code-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,29 @@
 
 I created this because I wanted
 - a pure python programming language detector
 - no machine learning dependencies
 
 Tested on python 3.6 through 3.9.
 
+Badges
+------
+[![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/whats_that_code?longCache=true&style=flat-square)](https://libraries.io/github/matthewdeanmartin/whats_that_code/sourcerank)
+
+[![Downloads](https://static.pepy.tech/badge/whats-that-code/month)](https://pepy.tech/project/whats-that-code)
+
+
+[![CodeFactor](https://www.codefactor.io/repository/github/matthewdeanmartin/whats_that_code/badge)](https://www.codefactor.io/repository/github/matthewdeanmartin/whats_that_code)
+
 ## Usage
-```
-> code = "def yo():\n   print('hello')"
-> guess_language_all_methods(code, file_name="yo.py")
-["python"]
+```python
+from whats_that_code.election import guess_language_all_methods
+code = "def yo():\n   print('hello')"
+result = guess_language_all_methods(code, file_name="yo.py")
+assert result == ["python"]
 ```
 
 ## How it Works
 1) Inspects file extension if available.
 2) Inspects shebang
 3) Looks for keywords
 4) Counts regexes for common patterns
```

### Comparing `whats_that_code-0.1.9/whats_that_code/__main__.py` & `whats_that_code-0.2.0/whats_that_code/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import logging
 import sys
 
 import docopt
 
 from whats_that_code import _version as meta
 
-
 # Do these need to stick around?
 LOGGERS = []
 
 LOGGER = logging.getLogger(__name__)
 
 
 def main() -> int:
```

### Comparing `whats_that_code-0.1.9/whats_that_code/codex_markers.py` & `whats_that_code-0.2.0/whats_that_code/codex_markers.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/election.py` & `whats_that_code-0.2.0/whats_that_code/election.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/extension_based.py` & `whats_that_code-0.2.0/whats_that_code/extension_based.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """
 Guess by extension
 """
+import os
 from typing import List
 
 from whats_that_code.known_languages import FILE_EXTENSIONS
 
 
 def guess_by_extension(file_name: str = "", text: str = "") -> List[str]:
     """
     Guess by extensions
     """
     if not file_name and not text:
         return []
+    _, extension_part = os.path.splitext(file_name)
+
+    if not extension_part:
+        return []
 
     guesses = set()
     extensions = []
     if file_name:
-        extensions.append("." + file_name.split(".")[1])
+        # TODO: use
+        extensions.append(extension_part)
     if text:
         words = [_ for _ in text.split(" ") if "." in _]
         for word in words:
             if word.endswith("."):
                 continue
-            extension = word.split(".")[1]
+            _, extension = os.path.splitext(word)
             if 1 < len(extension) < 5:
                 extensions.append(extension)
 
     for key, value in FILE_EXTENSIONS.items():
         for extension in extensions:
             for alternative in value:
                 if extension == alternative:
```

### Comparing `whats_that_code-0.1.9/whats_that_code/guess_by_code_and_tags.py` & `whats_that_code-0.2.0/whats_that_code/guess_by_code_and_tags.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/keyword_based.py` & `whats_that_code-0.2.0/whats_that_code/keyword_based.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/known_languages.py` & `whats_that_code-0.2.0/whats_that_code/known_languages.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/parsing_based.py` & `whats_that_code-0.2.0/whats_that_code/parsing_based.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/pygments_based.py` & `whats_that_code-0.2.0/whats_that_code/pygments_based.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/regex_based.py` & `whats_that_code-0.2.0/whats_that_code/regex_based.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/shebang_based.py` & `whats_that_code-0.2.0/whats_that_code/shebang_based.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/whats_that_code/tag_based.py` & `whats_that_code-0.2.0/whats_that_code/tag_based.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             continue
         if tag in FILE_EXTENSIONS:
             strong_guesses.add(tag)
 
     # e.g. tagged, numpy, which is commonly related to python
     weak_guesses = set()
     for tag in tags:
-        for key, value in RELATED_TAGS[0:3].items():
-            if tag in value:
+        for key, value in RELATED_TAGS.items():
+            if tag in value[0:3]:
                 weak_guesses.add(key)
 
     new_weak_guesses = []
     for guess in weak_guesses:
         if guess not in strong_guesses:
             new_weak_guesses.append(guess)
     return list(strong_guesses) + list(new_weak_guesses)
```

### Comparing `whats_that_code-0.1.9/whats_that_code/tags_data.py` & `whats_that_code-0.2.0/whats_that_code/tags_data.py`

 * *Files identical despite different names*

### Comparing `whats_that_code-0.1.9/PKG-INFO` & `whats_that_code-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whats-that-code
-Version: 0.1.9
+Version: 0.2.0
 Summary: Guess programming language from a string or file.
 Home-page: https://github.com/matthewdeanmartin/whats_that_code
 License: MIT
 Keywords: language detection,programming language detection
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -14,14 +14,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: defusedxml
 Requires-Dist: pygments
 Requires-Dist: pyrankvote
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/whats_that_code/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/whats_that_code/blob/main/docs/CHANGES.md
 Project-URL: Documentation, https://github.com/matthewdeanmartin/whats_that_code
 Project-URL: Repository, https://github.com/matthewdeanmartin/whats_that_code
@@ -36,19 +39,29 @@
 
 I created this because I wanted
 - a pure python programming language detector
 - no machine learning dependencies
 
 Tested on python 3.6 through 3.9.
 
+Badges
+------
+[![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/whats_that_code?longCache=true&style=flat-square)](https://libraries.io/github/matthewdeanmartin/whats_that_code/sourcerank)
+
+[![Downloads](https://static.pepy.tech/badge/whats-that-code/month)](https://pepy.tech/project/whats-that-code)
+
+
+[![CodeFactor](https://www.codefactor.io/repository/github/matthewdeanmartin/whats_that_code/badge)](https://www.codefactor.io/repository/github/matthewdeanmartin/whats_that_code)
+
 ## Usage
-```
-> code = "def yo():\n   print('hello')"
-> guess_language_all_methods(code, file_name="yo.py")
-["python"]
+```python
+from whats_that_code.election import guess_language_all_methods
+code = "def yo():\n   print('hello')"
+result = guess_language_all_methods(code, file_name="yo.py")
+assert result == ["python"]
 ```
 
 ## How it Works
 1) Inspects file extension if available.
 2) Inspects shebang
 3) Looks for keywords
 4) Counts regexes for common patterns
```

