# Comparing `tmp/bibleref-0.15.0.tar.gz` & `tmp/bibleref-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibleref-0.15.0.tar", last modified: Sun May 28 04:52:47 2023, max compression
+gzip compressed data, was "bibleref-0.9.0.tar", last modified: Sat Jan 21 12:45:08 2023, max compression
```

## Comparing `bibleref-0.15.0.tar` & `bibleref-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-28 04:52:47.356945 bibleref-0.15.0/
--rw-r--r--   0 james      (501) staff       (20)     1075 2023-01-20 09:07:43.000000 bibleref-0.15.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     8155 2023-05-28 04:52:47.356796 bibleref-0.15.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     7472 2023-02-10 12:39:09.000000 bibleref-0.15.0/README.md
--rw-r--r--   0 james      (501) staff       (20)      869 2023-05-28 04:47:35.000000 bibleref-0.15.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-05-28 04:52:47.356979 bibleref-0.15.0/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-28 04:52:47.353675 bibleref-0.15.0/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-28 04:52:47.355270 bibleref-0.15.0/src/bibleref/
--rw-r--r--   0 james      (501) staff       (20)     8361 2023-02-10 12:39:22.000000 bibleref-0.15.0/src/bibleref/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    22521 2023-01-20 09:07:43.000000 bibleref-0.15.0/src/bibleref/data.py
--rw-r--r--   0 james      (501) staff       (20)     9543 2023-01-25 13:11:46.000000 bibleref-0.15.0/src/bibleref/parser.py
--rw-r--r--   0 james      (501) staff       (20)    92831 2023-05-28 04:40:10.000000 bibleref-0.15.0/src/bibleref/ref.py
--rw-r--r--   0 james      (501) staff       (20)    27565 2023-01-25 13:11:46.000000 bibleref-0.15.0/src/bibleref/util.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-28 04:52:47.356069 bibleref-0.15.0/src/bibleref.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     8155 2023-05-28 04:52:47.000000 bibleref-0.15.0/src/bibleref.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      404 2023-05-28 04:52:47.000000 bibleref-0.15.0/src/bibleref.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-28 04:52:47.000000 bibleref-0.15.0/src/bibleref.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-05-28 04:52:47.000000 bibleref-0.15.0/src/bibleref.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        9 2023-05-28 04:52:47.000000 bibleref-0.15.0/src/bibleref.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-28 04:52:47.356606 bibleref-0.15.0/test/
--rw-r--r--   0 james      (501) staff       (20)     1166 2023-01-20 13:14:02.000000 bibleref-0.15.0/test/test_bibleref.py
--rw-r--r--   0 james      (501) staff       (20)     1844 2023-05-28 04:26:53.000000 bibleref-0.15.0/test/test_parser.py
--rw-r--r--   0 james      (501) staff       (20)    58981 2023-05-27 13:43:16.000000 bibleref-0.15.0/test/test_reference.py
--rw-r--r--   0 james      (501) staff       (20)    15625 2023-01-25 13:11:46.000000 bibleref-0.15.0/test/test_util.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-01-21 12:45:08.849358 bibleref-0.9.0/
+-rw-r--r--   0 james      (501) staff       (20)     1075 2023-01-20 09:07:43.000000 bibleref-0.9.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     5315 2023-01-21 12:45:08.849225 bibleref-0.9.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     4633 2023-01-21 12:44:16.000000 bibleref-0.9.0/README.md
+-rw-r--r--   0 james      (501) staff       (20)      868 2023-01-20 14:02:45.000000 bibleref-0.9.0/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-01-21 12:45:08.849394 bibleref-0.9.0/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-01-21 12:45:08.841365 bibleref-0.9.0/src/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-01-21 12:45:08.844637 bibleref-0.9.0/src/bibleref/
+-rw-r--r--   0 james      (501) staff       (20)     5522 2023-01-21 12:44:16.000000 bibleref-0.9.0/src/bibleref/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    22521 2023-01-20 09:07:43.000000 bibleref-0.9.0/src/bibleref/data.py
+-rw-r--r--   0 james      (501) staff       (20)     9465 2023-01-20 09:07:43.000000 bibleref-0.9.0/src/bibleref/parser.py
+-rw-r--r--   0 james      (501) staff       (20)    76728 2023-01-20 09:07:43.000000 bibleref-0.9.0/src/bibleref/ref.py
+-rw-r--r--   0 james      (501) staff       (20)    26650 2023-01-20 09:07:43.000000 bibleref-0.9.0/src/bibleref/util.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-01-21 12:45:08.847612 bibleref-0.9.0/src/bibleref.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     5315 2023-01-21 12:45:08.000000 bibleref-0.9.0/src/bibleref.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      404 2023-01-21 12:45:08.000000 bibleref-0.9.0/src/bibleref.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-01-21 12:45:08.000000 bibleref-0.9.0/src/bibleref.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-01-21 12:45:08.000000 bibleref-0.9.0/src/bibleref.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        9 2023-01-21 12:45:08.000000 bibleref-0.9.0/src/bibleref.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-01-21 12:45:08.849014 bibleref-0.9.0/test/
+-rw-r--r--   0 james      (501) staff       (20)     1166 2023-01-20 13:14:02.000000 bibleref-0.9.0/test/test_bibleref.py
+-rw-r--r--   0 james      (501) staff       (20)     1525 2023-01-20 09:07:43.000000 bibleref-0.9.0/test/test_parser.py
+-rw-r--r--   0 james      (501) staff       (20)    50065 2023-01-20 09:07:43.000000 bibleref-0.9.0/test/test_reference.py
+-rw-r--r--   0 james      (501) staff       (20)    15974 2023-01-20 09:07:43.000000 bibleref-0.9.0/test/test_util.py
```

### Comparing `bibleref-0.15.0/LICENSE` & `bibleref-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bibleref-0.15.0/PKG-INFO` & `bibleref-0.9.0/src/bibleref/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,193 +1,96 @@
-Metadata-Version: 2.1
-Name: bibleref
-Version: 0.15.0
-Summary: A package for handling references to Bible books, verses and verse-ranges.
-Project-URL: Documentation, https://multiscript.app/bibleref
-Project-URL: Source, https://github.com/multiscript/bibleref
-Project-URL: Issue Tracker, https://github.com/multiscript/bibleref/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Religion
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bibleref
-
-## Overview
+'''
+# Overview
 
 **bibleref is a Python package for handling references to Bible books, verses and verse-ranges, including string
-parsing and conversion.** Its only dependency is the [Lark](https://github.com/lark-parser/lark) parsing toolkit.
+parsing and conversion.** It's designed for future use with [Multiscript](https://multiscript.app), but it can be
+used as a standalone package. Its only dependency is the [Lark](https://github.com/lark-parser/lark) parsing toolkit.
 
 `bibleref` defines the following primary classes:
   - `bibleref.ref.BibleBook`:      An Enum of books in the Bible, with extra methods.
   - `bibleref.ref.BibleVerse`:     A reference to a single Bible verse (e.g. Matt 2:3)
   - `bibleref.ref.BibleRange`:     A reference to a continuous range of Bible verses (e.g. Matt 2:3-4:5)
   - `bibleref.ref.BibleRangeList`: A specialised list of `BibleRange` elements, allowing for grouping and
   set-style operations.
 
 (There is no `BibleChapter` class, as chapters are usually best handled as a `BibleRange`.)
 
 For convenience these classes can be directly imported from `bibleref`. They can each convert to and from strings.
 `BibleRange` and `BibleRangeList` implement common set operations (such as union, intersection, difference and 
 symmetric difference).
 
-## Docs
-
-See [multiscript.app/bibleref](https://multiscript.app/bibleref)
-
-## Examples
+# Examples
 
 ```python
->>> import bibleref
 >>> from bibleref import *
->>>                             # Parse from string
+>>> # Parse a string of Bible ranges...
 >>> range_list = BibleRangeList("Mark 2-3:6; 4; 6:1-6, 30-44, 56; Luke 2")
->>> print(range_list)           # Convert back to a string
+>>> print(range_list)               # Convert back to string
 Mark 2-3:6; 4; 6:1-6, 30-44, 56; Luke 2
 >>> len(range_list)
 6
->>> range_list[0]               # Individual ranges from a list
+>>> range_list[0]                   # Indiv ranges from a list
 BibleRange(Mark 2-3:6)
->>> range_list[1]
-BibleRange(Mark 4)
->>> range_list[5].start         # Start and...
+>>> range_list[5].start             # Start and...
 BibleVerse(Luke 2:1)
->>> range_list[5].end           # ...end verses of a range.
+>>> range_list[5].end               # ...end verses of a range.
 BibleVerse(Luke 2:52)
->>> range_list[5].end.book      # Verse attributes
+>>> range_list[5].end.book          # Verse attributes
 <BibleBook.Luke: 'Luke'>
 >>> range_list[5].end.chap_num
 2
 >>> range_list[5].end.verse_num
 52
 >>> len(range_list.groups)
 4
->>> range_list.groups[2]        # Indivdual range groups from a list
+>>> range_list.groups[2]            # Range groups from a list
 GroupView([BibleRange(Mark 6:1-6), BibleRange(Mark 6:30-44), BibleRange(Mark 6:56)])
->>> range_list.groups[2][0]     # Individual ranges within the group
+>>> range_list.groups[2][0]         # Indiv ranges within the group
 BibleRange(Mark 6:1-6)
 >>> range_list.groups[2][1]        
 BibleRange(Mark 6:30-44)
 >>> range_list.groups[2][2]
 BibleRange(Mark 6:56)
->>> BibleVerse('Mark 2:23') + 10 # Verse addition / subtraction
+>>> BibleVerse('Mark 2:23') + 10    # Verse addition / subtraction
 BibleVerse(Mark 3:5)
->>> BibleVerse('Mark 3:5') - BibleVerse('Mark 2:23')
-10
->>> BibleRange('1 John').split(by_chap=True, num_verses=15) # Range splits
-BibleRangeList("1 John 1, 2:1-15, 16-29, 3:1-15, 16-24, 4:1-15, 16-21, 5:1-15, 16-21")
->>> for verse in BibleRange('Mark 6:1-3'): # Range iteration
-...     print(verse)
+>>> BibleRange('1 John').split(by_chap=True, num_verses=10) # Range splits
+BibleRangeList("1 John 1, 2:1-10, 11-20, 21-29, 3:1-10, 11-20, 21-24, 4:1-10, 11-20, 21, 5:1-10, 11-20, 21")
+>>> for verse in BibleRange('Mark 6:1-3'): 
+...     print(verse)                # Range iteration
 ... 
 Mark 6:1
 Mark 6:2
 Mark 6:3
->>> bibleref.flags = BibleFlag.MULTIBOOK   # Enable multi-book ranges
->>> BibleRange('Matt 10-John 10')
-BibleRange(Matthew 10-John 10)
+>>> BibleRange('Matt 2:3-John 4:5', flags=BibleFlag.MULTIBOOK) # Multibook ranges
+BibleRange(Matthew 2:3-John 4:5)
 >>> list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-16")
->>> list_2 = BibleRangeList("John 1-3; Luke 9; Matt 3-5; Mark 12")
->>> list_1 | list_2                     # Union
-BibleRangeList("Matthew 2-5; Mark 6-8; 12; Luke 9-12; John 1-3; 14-16")
->>> list_1 & list_2                     # Intersection
-BibleRangeList("Matthew 3-4")
->>> list_1 - list_2                     # Difference
-BibleRangeList("Matthew 2; Mark 6-8; Luke 10-12; John 14-16")
->>> list_1 ^ list_2                     # Symmetric difference
-BibleRangeList("Matthew 2; 5; Mark 6-8; 12; Luke 9-12; John 1-3; 14-16")
->>> range_list = BibleRangeList("Mark 3:2-4:5; 1 John 1:5-3 John 8;")
->>> range_list.verse_count()            # Count of verses
-161
->>> range_list.chap_count()             # Count of chapters (incl partial)
-9
->>> range_list.chap_count(whole=True)   # Count of chapters (whole only)
-5
->>> range_list.book_count()             # Count of books (incl partial)
-4
->>> range_list.book_count(whole=True)   # Count of books (whole only)
-1
+>>> list_2 = BibleRangeList("John 1-3; Luke 9-11, 13; Matt 3-5; Mark 12")
+>>> list_1 | list_2                 # Union of range lists
+BibleRangeList("Matthew 2-5, Mark 6-8, 12, Luke 9-13, John 1-3, 14-16")
+>>> list_1 & list_2                 # Intersection range lists
+BibleRangeList("Matthew 3-4, Luke 10-11")
+>>> list_1 - list_2                 # Difference of range lists
+BibleRangeList("Matthew 2, Mark 6-8, Luke 12, John 14-16")
+>>> list_1 ^ list_2                 # Symmetric difference of range lists
+BibleRangeList("Matthew 2, 5, Mark 6-8, 12, Luke 9, 12-13, John 1-3, 14-16")
 ```
 
-## List Grouping
-
-Bible ranges in a list can be separated by two different characters, known here as the *major list separator*
-('`;`' by default), and the *minor list separator* ('`,`' by default). These separators play two roles: distinguishing
-between 'bare' chapter and verse numbers (i.e. those not preceded by book names), and controlling how Bible ranges are
-grouped within a list.
-
-The major list separator (`;`) indicates any bare number that follows is a chapter number. It also marks the start of
-a new group. It is usually used between ranges in different chapters.
-
-The minor list separator (`,`) indicates any bare number that follows is of the same kind as the previous number
-(whether a chapter or verse number). It also marks the continuation of the same group. It is usually used between
-ranges within the same chapter.
-
-The groups of a `BibleRangeList` are accessed through its `groups` property. Alternative, you can index each
-`BibleRange` directly (e.g. `range_list[1]`), ignoring the groupings.
-
-For example:
-```python
->>> from bibleref import *
->>> range_list = BibleRangeList("Matt 2:3-4, 5-7, 9-12") # One group of three verse ranges
->>> len(range_list.groups)
-1
->>> range_list[0]
-BibleRange(Matthew 2:3-4)
->>> range_list[1]
-BibleRange(Matthew 2:5-7)
->>> range_list[2]
-BibleRange(Matthew 2:9-12)
->>> range_list = BibleRangeList("Matt 2:3-4; 5-7, 9-12") # Two groups: one verse range, two chapter ranges
->>> len(range_list.groups)
-2
->>> range_list[0]             # Range access directly
-BibleRange(Matthew 2:3-4)
->>> range_list.groups[0][0]   # Same range accessed through its group
-BibleRange(Matthew 2:3-4)
->>> range_list.groups[1]      # Next group
-GroupView([BibleRange(Matthew 5-7), BibleRange(Matthew 9-12)])
->>> range_list.groups[1][0]
-BibleRange(Matthew 5-7)
->>> range_list.groups[1][1]   
-BibleRange(Matthew 9-12)
->>> range_list[2]             # Same range as previous line, but accessed directly
-BibleRange(Matthew 9-12)
->>> range_list = BibleRangeList("Matt 2:3-4, Matt 5-7, 9-12") # One group: one verse range, two chapter ranges
->>> len(range_list.groups)
-1
->>> range_list[1]
-BibleRange(Matthew 5-7)
->>> range_list[2]
-BibleRange(Matthew 9-12)
-```
-
-`bibleref.ref.BibleRangeList.regroup()` removes the existing groups in the list, and places the list items into
-their most natural new groupings.
-
-The major and minor list separator characters can be changed through the `bibleref.data.BibleData` singleton returned
-by `bible_data()`.
-
-## Attribution
+# Attribution
 
 The set operations and linked-list implementation in this package are derived from
 [python-ranges](https://github.com/Superbird11/ranges), under the MIT Licence.
 
 Other ideas in this package were developed from [python-scriptures](https://github.com/davisd/python-scriptures),
 under the BSD-3-Clause license.
 
-## Installation
+# Installation
 
    `pip install bibleref`
 
-## Build Instructions
+# Build Instructions
 
 Use these instructions if you’re building from the source. bibleref has been developed on Python 3.10, but should
 work on several earlier versions as well.
 
 1. `git clone https://github.com/multiscript/bibleref/`
 1. `cd bibleref`
 1. `python3 -m venv venv` (Create a virtual environment.)
@@ -196,7 +99,31 @@
    - In Windows cmd.exe: `venv\Scripts\\activate.bat`
    - In Windows powershell: `.\\venv\Scripts\Activate.ps1` You may first need to run `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`
 1. For development work...
    - `pip install -e .` (Creates an editable local install)
 1. ...or to build the package:
    - `pip install build`
    - `python -m build`
+
+# Top-Level Objects
+'''
+
+def bible_data():
+    '''Returns the package `bibleref.data.BibleData` singleton, containing the data for each Bible book.
+    The default Bible data is obtained from the `bibleref.data` submodule, but can be changed by setting properties
+    on this singleton.
+    '''
+    return _bible_data
+
+_bible_data = None  # Will be set by data submodule.
+
+flags = None # Will be set by ref submodule.
+'''Global package attribute that is a `bibleref.ref.BibleFlag` enum whose elements control package-wide behaviour.
+Many methods take a `flags` keyword-argument that overrides this global `flags` attribute during the
+execution of that method. The `bibleref.ref` submodule sets the default value to `bibleref.ref.BibleFlag.NONE`.
+'''
+
+class BibleRefException(Exception):
+    '''Parent class for all Exception types in this package.'''
+
+
+from .ref import BibleBook, BibleVerse, BibleRange, BibleRangeList, BibleRef, BibleFlag, BibleVersePart
```

### Comparing `bibleref-0.15.0/pyproject.toml` & `bibleref-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bibleref"
-version = "0.15.0"
+version = "0.9.0"
 
 description = "A package for handling references to Bible books, verses and verse-ranges."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "lark>=1.1.5",
 ]
```

### Comparing `bibleref-0.15.0/src/bibleref/data.py` & `bibleref-0.9.0/src/bibleref/data.py`

 * *Files identical despite different names*

### Comparing `bibleref-0.15.0/src/bibleref/parser.py` & `bibleref-0.9.0/src/bibleref/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''Submodule for parsing strings into Bible references. The contents of this submodule should be considered an
 implementation detail and not relied upon.
 '''
 from lark import Lark, UnexpectedInput
 from lark import Transformer, v_args
 from lark.visitors import VisitError
 
-import bibleref
 from bibleref import ref, bible_data
 
 
 MAJOR_LIST_SEP_SENTINEL = object()
 MINOR_LIST_SEP_SENTINEL = object()
 
 
@@ -48,15 +47,14 @@
         end_pos=orig.pos_in_stream + 1
         new_error = ref.BibleRefParsingError(f"Unexpected text: {string[start_pos:end_pos]}",
                                          start_pos, end_pos)
         new_error.orig = orig
         raise new_error
     
     try:
-        flags = flags or bibleref.flags or ref.BibleFlag.NONE
         _transformer().flags = flags
         range_groups_list = _transformer().transform(tree)
     except VisitError as e:
         raise e.orig_exc
     return range_groups_list
 
 def _meta_info_to_pos(meta_info):
```

### Comparing `bibleref-0.15.0/src/bibleref/ref.py` & `bibleref-0.9.0/src/bibleref/ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,5802 +1,4796 @@
 00000000: 0a23 2054 4f44 4f3a 2043 7265 6174 6520  .# TODO: Create 
-00000010: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
-00000020: 746f 2074 656d 706f 7261 7269 6c79 2073  to temporarily s
-00000030: 6574 206f 7220 756e 7365 7420 7061 7274  et or unset part
-00000040: 6963 756c 6172 2066 6c61 6773 0a23 2054  icular flags.# T
-00000050: 4f44 4f3a 2043 7265 6174 6520 6d6f 6475  ODO: Create modu
-00000060: 6c65 206d 6574 686f 6420 746f 206d 616b  le method to mak
-00000070: 6520 6974 2065 6173 6965 7220 746f 206b  e it easier to k
-00000080: 6565 7020 6578 6973 7469 6e67 2066 6c61  eep existing fla
-00000090: 6773 2062 7574 2073 6574 2f75 6e73 6574  gs but set/unset
+00000010: 6d6f 6475 6c65 206d 6574 686f 6420 746f  module method to
+00000020: 206d 616b 6520 6974 2065 6173 6965 7220   make it easier 
+00000030: 746f 206b 6565 7020 6578 6973 7469 6e67  to keep existing
+00000040: 2066 6c61 6773 2062 7574 2073 6574 2f75   flags but set/u
+00000050: 6e73 6574 2070 6172 7469 6375 6c61 7220  nset particular 
+00000060: 666c 6167 730a 2320 544f 444f 3a20 4372  flags.# TODO: Cr
+00000070: 6561 7465 2063 6f6e 7465 7874 206d 616e  eate context man
+00000080: 6167 6572 2074 6f20 7465 6d70 6f72 6172  ager to temporar
+00000090: 696c 7920 7365 7420 6f72 2075 6e73 6574  ily set or unset
 000000a0: 2070 6172 7469 6375 6c61 7220 666c 6167   particular flag
-000000b0: 730a 0a66 726f 6d20 6461 7461 636c 6173  s..from dataclas
-000000c0: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
-000000d0: 6c61 7373 0a66 726f 6d20 656e 756d 2069  lass.from enum i
-000000e0: 6d70 6f72 7420 456e 756d 2c20 466c 6167  mport Enum, Flag
-000000f0: 2c20 6175 746f 0a66 726f 6d20 7479 7069  , auto.from typi
-00000100: 6e67 2069 6d70 6f72 7420 556e 696f 6e0a  ng import Union.
-00000110: 0a69 6d70 6f72 7420 6269 626c 6572 6566  .import bibleref
-00000120: 0a66 726f 6d20 6269 626c 6572 6566 2069  .from bibleref i
-00000130: 6d70 6f72 7420 4269 626c 6552 6566 4578  mport BibleRefEx
-00000140: 6365 7074 696f 6e2c 2062 6962 6c65 5f64  ception, bible_d
-00000150: 6174 610a 0a23 0a23 2053 6574 2d73 7479  ata..#.# Set-sty
-00000160: 6c65 206f 7065 7261 7469 6f6e 7320 696e  le operations in
-00000170: 2074 6869 7320 6d6f 6475 6c65 2061 7265   this module are
-00000180: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
-00000190: 6520 7079 7468 6f6e 2d72 616e 6765 7320  e python-ranges 
-000001a0: 6d6f 6475 6c65 0a23 2061 7420 6874 7470  module.# at http
-000001b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000001c0: 7570 6572 6269 7264 3131 2f72 616e 6765  uperbird11/range
-000001d0: 732c 2075 6e64 6572 2074 6865 204d 4954  s, under the MIT
-000001e0: 204c 6963 656e 6365 0a23 0a0a 636c 6173   Licence.#..clas
-000001f0: 7320 4269 626c 6546 6c61 6728 466c 6167  s BibleFlag(Flag
-00000200: 293a 0a20 2020 2027 2727 466c 6167 7320  ):.    '''Flags 
-00000210: 7573 6564 2066 6f72 2063 6f6e 7472 6f6c  used for control
-00000220: 6c69 6e67 2076 6172 696f 7573 2062 6568  ling various beh
-00000230: 6176 696f 7572 7320 7468 726f 7567 686f  aviours througho
-00000240: 7574 2074 6865 2070 6163 6b61 6765 2e20  ut the package. 
-00000250: 5468 6573 6520 6361 6e20 6265 2073 6574  These can be set
-00000260: 2067 6c6f 6261 6c6c 7920 666f 7220 7468   globally for th
-00000270: 6520 7061 636b 6167 650a 2020 2020 7573  e package.    us
-00000280: 696e 6720 7468 6520 6062 6962 6c65 7265  ing the `biblere
-00000290: 662e 666c 6167 7360 2061 7474 7269 6275  f.flags` attribu
-000002a0: 7465 2c20 6f72 2070 6572 2d6d 6574 686f  te, or per-metho
-000002b0: 6420 666f 7220 6d65 7468 6f64 7320 7468  d for methods th
-000002c0: 6174 2069 6e63 6c75 6465 7320 6120 6066  at includes a `f
-000002d0: 6c61 6773 6020 6b65 7977 6f72 6420 6172  lags` keyword ar
-000002e0: 6775 6d65 6e74 2e0a 2020 2020 2727 270a  gument..    '''.
-000002f0: 2020 2020 4e4f 4e45 203d 2030 0a20 2020      NONE = 0.   
-00000300: 2027 2727 4e6f 2060 4269 626c 6546 6c61   '''No `BibleFla
-00000310: 6760 2066 6c61 6773 2061 7265 2073 6574  g` flags are set
-00000320: 2e20 4465 6661 756c 7420 7661 6c75 6520  . Default value 
-00000330: 666f 7220 6062 6962 6c65 7265 662e 666c  for `bibleref.fl
-00000340: 6167 7360 2e27 2727 0a0a 2020 2020 4d55  ags`.'''..    MU
-00000350: 4c54 4942 4f4f 4b20 3d20 6175 746f 2829  LTIBOOK = auto()
-00000360: 0a20 2020 2027 2727 5768 656e 2073 6574  .    '''When set
-00000370: 2c20 6120 6042 6962 6c65 5261 6e67 6560  , a `BibleRange`
-00000380: 2063 616e 2062 6520 636f 6e73 7472 7563   can be construc
-00000390: 7465 6420 7468 6174 2073 7061 6e73 206d  ted that spans m
-000003a0: 756c 7469 706c 6520 4269 626c 6520 626f  ultiple Bible bo
-000003b0: 6f6b 732e 2045 7869 7374 696e 6720 6d75  oks. Existing mu
-000003c0: 6c74 6962 6f6f 6b0a 2020 2020 7261 6e67  ltibook.    rang
-000003d0: 6573 2062 6568 6176 6520 636f 7272 6563  es behave correc
-000003e0: 746c 7920 6576 656e 2077 6865 6e20 604d  tly even when `M
-000003f0: 554c 5449 424f 4f4b 6020 6973 2075 6e73  ULTIBOOK` is uns
-00000400: 6574 2e27 2727 0a0a 2020 2020 5645 5253  et.'''..    VERS
-00000410: 455f 3020 3d20 6175 746f 2829 0a20 2020  E_0 = auto().   
-00000420: 2027 2727 5768 656e 2073 6574 2c20 6120   '''When set, a 
-00000430: 6042 6962 6c65 5665 7273 6560 2063 616e  `BibleVerse` can
-00000440: 2062 6520 636f 6e73 7472 7563 7465 6420   be constructed 
-00000450: 7768 6572 6520 7468 6520 6669 7273 7420  where the first 
-00000460: 7665 7273 6520 6e75 6d62 6572 206f 6620  verse number of 
-00000470: 736f 6d65 2063 6861 7074 6572 730a 2020  some chapters.  
-00000480: 2020 6973 2030 2c20 6e6f 7420 312e 2028    is 0, not 1. (
-00000490: 5468 6973 2069 7320 6375 7272 656e 746c  This is currentl
-000004a0: 7920 7472 7565 206f 6e6c 7920 666f 7220  y true only for 
-000004b0: 7468 6520 5073 616c 6d73 2074 6861 7420  the Psalms that 
-000004c0: 6861 7665 2073 7570 6572 7363 7269 7074  have superscript
-000004d0: 696f 6e73 2e29 2057 6865 6e20 796f 7520  ions.) When you 
-000004e0: 6e65 6564 2074 6f20 6d69 780a 2020 2020  need to mix.    
-000004f0: 7265 6665 7265 6e63 6573 2074 6861 7420  references that 
-00000500: 646f 206f 7220 646f 6e27 7420 616c 6c6f  do or don't allo
-00000510: 7720 666f 7220 7665 7273 6520 302c 2069  w for verse 0, i
-00000520: 7420 6d61 7920 6265 2065 6173 6965 7220  t may be easier 
-00000530: 746f 2073 6574 206f 7220 636c 6561 7220  to set or clear 
-00000540: 6056 4552 5345 5f30 6020 666f 7220 616c  `VERSE_0` for al
-00000550: 6c20 796f 7572 2063 6f64 652c 2061 6e64  l your code, and
-00000560: 0a20 2020 2074 6865 6e20 7573 6520 7468  .    then use th
-00000570: 6520 6076 6572 7365 5f30 5f74 6f5f 3128  e `verse_0_to_1(
-00000580: 2960 2061 6e64 2060 7665 7273 655f 315f  )` and `verse_1_
-00000590: 746f 5f30 2829 6020 6d65 7468 6f64 7320  to_0()` methods 
-000005a0: 6f6e 2060 4269 626c 6556 6572 7365 602c  on `BibleVerse`,
-000005b0: 2060 4269 626c 6552 616e 6765 6020 616e   `BibleRange` an
-000005c0: 6420 6042 6962 6c65 5261 6e67 654c 6973  d `BibleRangeLis
-000005d0: 7460 0a20 2020 2061 7320 6e65 6365 7373  t`.    as necess
-000005e0: 6172 792e 2727 270a 0a20 2020 2041 4c4c  ary.'''..    ALL
-000005f0: 203d 204d 554c 5449 424f 4f4b 207c 2056   = MULTIBOOK | V
-00000600: 4552 5345 5f30 0a20 2020 2027 2727 416c  ERSE_0.    '''Al
-00000610: 6c20 6042 6962 6c65 466c 6167 6020 666c  l `BibleFlag` fl
-00000620: 6167 7320 6172 6520 7365 742e 2727 270a  ags are set.'''.
-00000630: 0a62 6962 6c65 7265 662e 666c 6167 7320  .bibleref.flags 
-00000640: 3d20 4269 626c 6546 6c61 672e 4e4f 4e45  = BibleFlag.NONE
-00000650: 2023 2044 6566 6175 6c74 2073 6574 7469   # Default setti
-00000660: 6e67 2066 6f72 2067 6c6f 6261 6c20 666c  ng for global fl
-00000670: 6167 7320 6174 7472 6962 7574 652e 0a0a  ags attribute...
-00000680: 0a63 6c61 7373 2042 6962 6c65 426f 6f6b  .class BibleBook
-00000690: 2845 6e75 6d29 3a0a 2020 2020 2727 2741  (Enum):.    '''A
-000006a0: 6e20 656e 756d 206f 6620 626f 6f6b 7320  n enum of books 
-000006b0: 696e 2074 6865 2042 6962 6c65 2e0a 0a20  in the Bible... 
-000006c0: 2020 2041 2060 4269 626c 6542 6f6f 6b60     A `BibleBook`
-000006d0: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
-000006e0: 6e67 2065 7874 7261 2061 7474 7269 6275  ng extra attribu
-000006f0: 7465 7320 2861 6464 6564 2064 7572 696e  tes (added durin
-00000700: 6720 7061 636b 6167 6520 696d 706f 7274  g package import
-00000710: 293a 0a20 2020 2020 202d 2060 6162 6272  ):.      - `abbr
-00000720: 6576 603a 2020 2054 6865 2061 6262 7265  ev`:   The abbre
-00000730: 7669 6174 6564 206e 616d 6520 6f66 2074  viated name of t
-00000740: 6865 2062 6f6f 6b0a 2020 2020 2020 2d20  he book.      - 
-00000750: 6074 6974 6c65 603a 2020 2020 5468 6520  `title`:    The 
-00000760: 6675 6c6c 2074 6974 6c65 206f 6620 7468  full title of th
-00000770: 6520 626f 6f6b 2e0a 2020 2020 2020 2d20  e book..      - 
-00000780: 6072 6567 6578 603a 2020 2020 4120 7265  `regex`:    A re
-00000790: 6765 7820 7768 6963 6820 6d61 7463 6865  gex which matche
-000007a0: 7320 616e 7920 6163 6365 7074 6162 6c65  s any acceptable
-000007b0: 206e 616d 652f 6162 6272 6576 2066 6f72   name/abbrev for
-000007c0: 2074 6865 2062 6f6f 6b2e 0a20 2020 2020   the book..     
-000007d0: 202d 2060 6f72 6465 7260 3a20 2020 2041   - `order`:    A
-000007e0: 6e20 696e 7465 6765 7220 696e 6469 6361  n integer indica
-000007f0: 7469 6e67 2069 7473 206f 7264 6572 696e  ting its orderin
-00000800: 6720 696e 2074 6865 2063 6f6c 6c65 6374  g in the collect
-00000810: 696f 6e20 6f66 2062 6f6f 6b73 2028 302d  ion of books (0-
-00000820: 6261 7365 6429 2e0a 2020 2020 0a20 2020  based)..    .   
-00000830: 2054 776f 2060 4269 626c 6542 6f6f 6b60   Two `BibleBook`
-00000840: 7320 6361 6e20 6265 2063 6f6d 7061 7265  s can be compare
-00000850: 6420 7573 696e 6720 7468 6520 7374 616e  d using the stan
-00000860: 6461 7264 2063 6f6d 7061 7269 736f 6e20  dard comparison 
-00000870: 6f70 6572 6174 6f72 732c 2077 6869 6368  operators, which
-00000880: 2063 6f6d 7061 7265 2074 6865 0a20 2020   compare the.   
-00000890: 2062 6f6f 6b73 2720 706f 7369 7469 6f6e   books' position
-000008a0: 2069 6e20 7468 6520 626f 6f6b 206f 7264   in the book ord
-000008b0: 6572 696e 672e 0a20 2020 2027 2727 0a20  ering..    '''. 
-000008c0: 2020 2023 2045 7874 7261 2070 7269 7661     # Extra priva
-000008d0: 7465 2061 7474 7269 6275 7465 733a 0a20  te attributes:. 
-000008e0: 2020 2023 205f 6d61 785f 7665 7273 6573     # _max_verses
-000008f0: 3a20 204c 6973 7420 6f66 206d 6178 2076  :  List of max v
-00000900: 6572 7365 206e 756d 6265 7220 666f 7220  erse number for 
-00000910: 6561 6368 2063 6861 7074 6572 2028 6173  each chapter (as
-00000920: 6365 6e64 696e 6720 6279 2063 6861 7074  cending by chapt
-00000930: 6572 292e 0a20 2020 2023 2020 2020 2020  er)..    #      
-00000940: 2020 2020 2020 2020 2020 204c 656e 206f             Len o
-00000950: 6620 6c69 7374 2069 7320 6e75 6d62 6572  f list is number
-00000960: 206f 6620 6368 6170 7465 7273 2e20 4e6f   of chapters. No
-00000970: 6e65 2069 6620 6e6f 206d 6178 5f76 6572  ne if no max_ver
-00000980: 7365 2064 6174 6120 7375 7070 6c69 6564  se data supplied
-00000990: 2e0a 2020 2020 2320 5f76 6572 7365 5f30  ..    # _verse_0
-000009a0: 733a 2020 2020 5365 7420 6f66 2063 6861  s:    Set of cha
-000009b0: 7074 6572 206e 756d 6265 7273 2028 312d  pter numbers (1-
-000009c0: 696e 6465 7865 6429 2074 6861 7420 6361  indexed) that ca
-000009d0: 6e20 6265 6769 6e20 7769 7468 2061 2076  n begin with a v
-000009e0: 6572 7365 2030 2e20 456d 7074 7920 7365  erse 0. Empty se
-000009f0: 740a 2020 2020 2320 2020 2020 2020 2020  t.    #         
-00000a00: 2020 2020 2020 2020 6966 206e 6f20 6368          if no ch
-00000a10: 6170 7465 7273 2063 616e 2062 6567 696e  apters can begin
-00000a20: 2077 6974 6820 6120 7665 7273 6520 302e   with a verse 0.
-00000a30: 0a20 2020 2023 0a20 2020 2047 656e 2020  .    #.    Gen  
-00000a40: 2020 203d 2022 4765 6e22 200a 2020 2020     = "Gen" .    
-00000a50: 4578 6f64 2020 2020 3d20 2245 786f 6422  Exod    = "Exod"
-00000a60: 0a20 2020 204c 6576 2020 2020 203d 2022  .    Lev     = "
-00000a70: 4c65 7622 0a20 2020 204e 756d 2020 2020  Lev".    Num    
-00000a80: 203d 2022 4e75 6d22 0a20 2020 2044 6575   = "Num".    Deu
-00000a90: 7420 2020 203d 2022 4465 7574 220a 2020  t    = "Deut".  
-00000aa0: 2020 4a6f 7368 2020 2020 3d20 224a 6f73    Josh    = "Jos
-00000ab0: 6822 0a20 2020 204a 7564 6720 2020 203d  h".    Judg    =
-00000ac0: 2022 4a75 6467 220a 2020 2020 5275 7468   "Judg".    Ruth
-00000ad0: 2020 2020 3d20 2252 7574 6822 0a20 2020      = "Ruth".   
-00000ae0: 2049 5361 6d20 2020 203d 2022 3153 616d   ISam    = "1Sam
-00000af0: 220a 2020 2020 4949 5361 6d20 2020 3d20  ".    IISam   = 
-00000b00: 2232 5361 6d22 0a20 2020 2049 4b67 7320  "2Sam".    IKgs 
-00000b10: 2020 203d 2022 314b 6773 220a 2020 2020     = "1Kgs".    
-00000b20: 4949 4b67 7320 2020 3d20 2232 4b67 7322  IIKgs   = "2Kgs"
-00000b30: 0a20 2020 2049 4368 7220 2020 203d 2022  .    IChr    = "
-00000b40: 3143 6872 220a 2020 2020 4949 4368 7220  1Chr".    IIChr 
-00000b50: 2020 3d20 2232 4368 7222 0a20 2020 2045    = "2Chr".    E
-00000b60: 7a72 6120 2020 203d 2022 457a 7261 220a  zra    = "Ezra".
-00000b70: 2020 2020 4e65 6820 2020 2020 3d20 224e      Neh     = "N
-00000b80: 6568 220a 2020 2020 4573 7468 2020 2020  eh".    Esth    
-00000b90: 3d20 2245 7374 6822 0a20 2020 204a 6f62  = "Esth".    Job
-00000ba0: 2020 2020 203d 2022 4a6f 6222 0a20 2020       = "Job".   
-00000bb0: 2050 7361 2020 2020 203d 2022 5073 6122   Psa     = "Psa"
-00000bc0: 0a20 2020 2050 726f 7620 2020 203d 2022  .    Prov    = "
-00000bd0: 5072 6f76 220a 2020 2020 4563 636c 2020  Prov".    Eccl  
-00000be0: 2020 3d20 2245 6363 6c22 0a20 2020 2053    = "Eccl".    S
-00000bf0: 6f6e 6720 2020 203d 2022 536f 6e67 220a  ong    = "Song".
-00000c00: 2020 2020 4973 6120 2020 2020 3d20 2249      Isa     = "I
-00000c10: 7361 220a 2020 2020 4a65 7220 2020 2020  sa".    Jer     
-00000c20: 3d20 224a 6572 220a 2020 2020 4c61 6d20  = "Jer".    Lam 
-00000c30: 2020 2020 3d20 224c 616d 220a 2020 2020      = "Lam".    
-00000c40: 457a 656b 2020 2020 3d20 2245 7a65 6b22  Ezek    = "Ezek"
-00000c50: 0a20 2020 2044 616e 2020 2020 203d 2022  .    Dan     = "
-00000c60: 4461 6e22 0a20 2020 2048 6f73 2020 2020  Dan".    Hos    
-00000c70: 203d 2022 486f 7322 0a20 2020 204a 6f65   = "Hos".    Joe
-00000c80: 6c20 2020 203d 2022 4a6f 656c 220a 2020  l    = "Joel".  
-00000c90: 2020 416d 6f73 2020 2020 3d20 2241 6d6f    Amos    = "Amo
-00000ca0: 7322 0a20 2020 204f 6261 6420 2020 203d  s".    Obad    =
-00000cb0: 2022 4f62 6164 220a 2020 2020 4a6f 6e61   "Obad".    Jona
-00000cc0: 6820 2020 3d20 224a 6f6e 6168 220a 2020  h   = "Jonah".  
-00000cd0: 2020 4d69 6320 2020 2020 3d20 224d 6963    Mic     = "Mic
-00000ce0: 220a 2020 2020 4e61 6820 2020 2020 3d20  ".    Nah     = 
-00000cf0: 224e 6168 220a 2020 2020 4861 6220 2020  "Nah".    Hab   
-00000d00: 2020 3d20 2248 6162 220a 2020 2020 5a65    = "Hab".    Ze
-00000d10: 7068 2020 2020 3d20 225a 6570 6822 0a20  ph    = "Zeph". 
-00000d20: 2020 2048 6167 2020 2020 203d 2022 4861     Hag     = "Ha
-00000d30: 6722 0a20 2020 205a 6563 6820 2020 203d  g".    Zech    =
-00000d40: 2022 5a65 6368 220a 2020 2020 4d61 6c20   "Zech".    Mal 
-00000d50: 2020 2020 3d20 224d 616c 220a 2020 2020      = "Mal".    
-00000d60: 4d61 7474 2020 2020 3d20 224d 6174 7422  Matt    = "Matt"
-00000d70: 0a20 2020 204d 6172 6b20 2020 203d 2022  .    Mark    = "
-00000d80: 4d61 726b 220a 2020 2020 4c75 6b65 2020  Mark".    Luke  
-00000d90: 2020 3d20 224c 756b 6522 0a20 2020 204a    = "Luke".    J
-00000da0: 6f68 6e20 2020 203d 2022 4a6f 686e 220a  ohn    = "John".
-00000db0: 2020 2020 4163 7473 2020 2020 3d20 2241      Acts    = "A
-00000dc0: 6374 7322 0a20 2020 2052 6f6d 2020 2020  cts".    Rom    
-00000dd0: 203d 2022 526f 6d22 0a20 2020 2049 436f   = "Rom".    ICo
-00000de0: 7220 2020 203d 2022 3143 6f72 220a 2020  r    = "1Cor".  
-00000df0: 2020 4949 436f 7220 2020 3d20 2232 436f    IICor   = "2Co
-00000e00: 7222 0a20 2020 2047 616c 2020 2020 203d  r".    Gal     =
-00000e10: 2022 4761 6c22 0a20 2020 2045 7068 2020   "Gal".    Eph  
-00000e20: 2020 203d 2022 4570 6822 0a20 2020 2050     = "Eph".    P
-00000e30: 6869 6c20 2020 203d 2022 5068 696c 220a  hil    = "Phil".
-00000e40: 2020 2020 436f 6c20 2020 2020 3d20 2243      Col     = "C
-00000e50: 6f6c 220a 2020 2020 4954 6820 2020 2020  ol".    ITh     
-00000e60: 3d20 2231 5468 220a 2020 2020 4949 5468  = "1Th".    IITh
-00000e70: 2020 2020 3d20 2232 5468 220a 2020 2020      = "2Th".    
-00000e80: 4954 696d 2020 2020 3d20 2231 5469 6d22  ITim    = "1Tim"
-00000e90: 0a20 2020 2049 4954 696d 2020 203d 2022  .    IITim   = "
-00000ea0: 3254 696d 220a 2020 2020 5469 7475 7320  2Tim".    Titus 
-00000eb0: 2020 3d20 2254 6974 7573 220a 2020 2020    = "Titus".    
-00000ec0: 5068 6c6d 2020 2020 3d20 2250 686c 6d22  Phlm    = "Phlm"
-00000ed0: 0a20 2020 2048 6562 2020 2020 203d 2022  .    Heb     = "
-00000ee0: 4865 6222 0a20 2020 204a 616d 2020 2020  Heb".    Jam    
-00000ef0: 203d 2022 4a61 6d22 0a20 2020 2049 5065   = "Jam".    IPe
-00000f00: 7420 2020 203d 2022 3150 6574 220a 2020  t    = "1Pet".  
-00000f10: 2020 4949 5065 7420 2020 3d20 2232 5065    IIPet   = "2Pe
-00000f20: 7422 0a20 2020 2049 4a6e 2020 2020 203d  t".    IJn     =
-00000f30: 2022 314a 6e22 0a20 2020 2049 494a 6e20   "1Jn".    IIJn 
-00000f40: 2020 203d 2022 324a 6e22 0a20 2020 2049     = "2Jn".    I
-00000f50: 4949 4a6e 2020 203d 2022 334a 6e22 0a20  IIJn   = "3Jn". 
-00000f60: 2020 204a 7564 6520 2020 203d 2022 4a75     Jude    = "Ju
-00000f70: 6465 220a 2020 2020 5265 7620 2020 2020  de".    Rev     
-00000f80: 3d20 2252 6576 220a 0a20 2020 2040 636c  = "Rev"..    @cl
-00000f90: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00000fa0: 6620 6672 6f6d 5f73 7472 2863 6c73 2c20  f from_str(cls, 
-00000fb0: 7374 7269 6e67 3a20 7374 722c 2072 6169  string: str, rai
-00000fc0: 7365 5f65 7272 6f72 3a20 626f 6f6c 203d  se_error: bool =
-00000fd0: 2046 616c 7365 2920 2d3e 2027 4269 626c   False) -> 'Bibl
-00000fe0: 6542 6f6f 6b27 3a0a 2020 2020 2020 2020  eBook':.        
-00000ff0: 2727 2752 6574 7572 6e20 7468 6520 4269  '''Return the Bi
-00001000: 626c 6542 6f6f 6b20 6d61 7463 6869 6e67  bleBook matching
-00001010: 2074 6865 2067 6976 656e 2073 7472 696e   the given strin
-00001020: 6720 6e61 6d65 2e0a 2020 2020 2020 2020  g name..        
-00001030: 5768 6974 6573 7061 6365 2069 6e20 6073  Whitespace in `s
-00001040: 7472 696e 6760 2069 7320 7374 7269 7070  tring` is stripp
-00001050: 6564 2062 6566 6f72 6520 6d61 7463 6869  ed before matchi
-00001060: 6e67 2e0a 2020 2020 2020 2020 0a20 2020  ng..        .   
-00001070: 2020 2020 2049 6620 6e6f 2062 6f6f 6b20       If no book 
-00001080: 6d61 7463 6865 7320 616e 6420 7261 6973  matches and rais
-00001090: 655f 6572 726f 7220 6973 2046 616c 7365  e_error is False
-000010a0: 2028 7468 6520 6465 6661 756c 7429 2c20   (the default), 
-000010b0: 4e6f 6e65 2069 7320 7265 7475 726e 6564  None is returned
-000010c0: 2e0a 2020 2020 2020 2020 4966 206e 6f20  ..        If no 
-000010d0: 626f 6f6b 206d 6174 6368 6573 2061 6e64  book matches and
-000010e0: 2072 6169 7365 5f65 7272 6f72 2069 7320   raise_error is 
-000010f0: 5472 7565 2c20 616e 2060 496e 7661 6c69  True, an `Invali
-00001100: 6452 6566 6572 656e 6365 4572 726f 7260  dReferenceError`
-00001110: 2069 7320 7261 6973 6564 2e0a 2020 2020   is raised..    
-00001120: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00001130: 7374 7269 6e67 203d 2073 7472 696e 672e  string = string.
-00001140: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
-00001150: 6d61 7463 6820 3d20 4661 6c73 650a 2020  match = False.  
-00001160: 2020 2020 2020 666f 7220 626f 6f6b 2069        for book i
-00001170: 6e20 4269 626c 6542 6f6f 6b3a 0a20 2020  n BibleBook:.   
-00001180: 2020 2020 2020 2020 2069 6620 626f 6f6b           if book
-00001190: 2e72 6567 6578 2069 7320 6e6f 7420 4e6f  .regex is not No
-000011a0: 6e65 2061 6e64 2062 6f6f 6b2e 7265 6765  ne and book.rege
-000011b0: 782e 6675 6c6c 6d61 7463 6828 7374 7269  x.fullmatch(stri
-000011c0: 6e67 2920 6973 206e 6f74 204e 6f6e 653a  ng) is not None:
-000011d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011e0: 206d 6174 6368 203d 2054 7275 650a 2020   match = True.  
-000011f0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00001200: 6561 6b0a 2020 2020 2020 2020 6966 206d  eak.        if m
-00001210: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-00001220: 2020 7265 7475 726e 2062 6f6f 6b0a 2020    return book.  
-00001230: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001240: 2020 2020 2020 2020 6966 2072 6169 7365          if raise
-00001250: 5f65 7272 6f72 3a0a 2020 2020 2020 2020  _error:.        
-00001260: 2020 2020 2020 2020 7261 6973 6520 496e          raise In
-00001270: 7661 6c69 6452 6566 6572 656e 6365 4572  validReferenceEr
-00001280: 726f 7228 6622 4e6f 2062 6f6f 6b20 666f  ror(f"No book fo
-00001290: 756e 6420 666f 7220 7374 7269 6e67 2027  und for string '
-000012a0: 7b73 7472 696e 677d 2722 290a 2020 2020  {string}'").    
-000012b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000012d0: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-000012e0: 6566 2076 6572 7365 5f63 6f75 6e74 2873  ef verse_count(s
-000012f0: 656c 662c 2066 6c61 6773 3a20 4269 626c  elf, flags: Bibl
-00001300: 6546 6c61 6720 3d20 4e6f 6e65 2920 2d3e  eFlag = None) ->
-00001310: 2069 6e74 3a0a 2020 2020 2020 2020 2727   int:.        ''
-00001320: 2752 6574 7572 6e73 2074 6865 206e 756d  'Returns the num
-00001330: 6265 7220 6f66 2076 6572 7365 7320 696e  ber of verses in
-00001340: 2074 6869 7320 6042 6962 6c65 426f 6f6b   this `BibleBook
-00001350: 602e 2727 270a 2020 2020 2020 2020 636f  `.'''.        co
-00001360: 756e 7420 3d20 300a 2020 2020 2020 2020  unt = 0.        
-00001370: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00001380: 656c 662e 6368 6170 5f63 6f75 6e74 2829  elf.chap_count()
-00001390: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-000013a0: 6f75 6e74 202b 3d20 2873 656c 662e 6d61  ount += (self.ma
-000013b0: 785f 7665 7273 655f 6e75 6d28 692b 3129  x_verse_num(i+1)
-000013c0: 202d 2073 656c 662e 6d69 6e5f 7665 7273   - self.min_vers
-000013d0: 655f 6e75 6d28 692b 312c 2066 6c61 6773  e_num(i+1, flags
-000013e0: 3d66 6c61 6773 2920 2b20 3129 0a20 2020  =flags) + 1).   
-000013f0: 2020 2020 2072 6574 7572 6e20 636f 756e       return coun
-00001400: 740a 0a20 2020 2064 6566 2063 6861 705f  t..    def chap_
-00001410: 636f 756e 7428 7365 6c66 2920 2d3e 2069  count(self) -> i
-00001420: 6e74 3a0a 2020 2020 2020 2020 2727 2752  nt:.        '''R
-00001430: 6574 7572 6e73 2074 6865 206e 756d 6265  eturns the numbe
-00001440: 7220 6f66 2063 6861 7074 6572 7320 696e  r of chapters in
-00001450: 2074 6869 7320 6042 6962 6c65 426f 6f6b   this `BibleBook
-00001460: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
-00001470: 2020 2020 2020 2072 6574 7572 6e20 2873         return (s
-00001480: 656c 662e 6d61 785f 6368 6170 5f6e 756d  elf.max_chap_num
-00001490: 2829 202d 2073 656c 662e 6d69 6e5f 6368  () - self.min_ch
-000014a0: 6170 5f6e 756d 2829 202b 2031 290a 0a20  ap_num() + 1).. 
-000014b0: 2020 2064 6566 206d 696e 5f63 6861 705f     def min_chap_
-000014c0: 6e75 6d28 7365 6c66 2920 2d3e 2069 6e74  num(self) -> int
-000014d0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
-000014e0: 7572 6e20 6c6f 7765 7374 2063 6861 7074  urn lowest chapt
-000014f0: 6572 206e 756d 6265 7220 2863 7572 7265  er number (curre
-00001500: 6e74 6c79 2061 6c77 6179 7320 3129 2066  ntly always 1) f
-00001510: 6f72 2074 6869 7320 6042 6962 6c65 426f  or this `BibleBo
-00001520: 6f6b 602e 0a20 2020 2020 2020 2027 2727  ok`..        '''
-00001530: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00001540: 2e5f 6d61 785f 7665 7273 6573 2069 7320  ._max_verses is 
-00001550: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00001560: 2020 7265 7475 726e 2030 0a20 2020 2020    return 0.     
-00001570: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00001580: 2020 2020 2072 6574 7572 6e20 3120 2020       return 1   
-00001590: 2023 2043 7572 7265 6e74 6c79 2061 6c77   # Currently alw
-000015a0: 6179 7320 312e 2050 6572 6861 7073 2069  ays 1. Perhaps i
-000015b0: 6e20 6675 7475 7265 2073 6f6d 6520 626f  n future some bo
-000015c0: 6f6b 7320 6d61 7920 6861 7665 2061 2063  oks may have a c
-000015d0: 6861 7074 6572 2d30 2070 726f 6c6f 6775  hapter-0 prologu
-000015e0: 6520 696e 636c 7564 6564 3f0a 0a20 2020  e included?..   
-000015f0: 2064 6566 206d 6178 5f63 6861 705f 6e75   def max_chap_nu
-00001600: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
-00001610: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-00001620: 6e20 6869 6768 6573 7420 6368 6170 7465  n highest chapte
-00001630: 7220 6e75 6d62 6572 2066 6f72 2074 6869  r number for thi
-00001640: 7320 6042 6962 6c65 426f 6f6b 602e 0a20  s `BibleBook`.. 
-00001650: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00001660: 2020 2069 6620 7365 6c66 2e5f 6d61 785f     if self._max_
-00001670: 7665 7273 6573 2069 7320 4e6f 6e65 3a0a  verses is None:.
-00001680: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001690: 726e 2030 0a20 2020 2020 2020 2065 6c73  rn 0.        els
-000016a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000016b0: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
-000016c0: 6d61 785f 7665 7273 6573 290a 0a20 2020  max_verses)..   
-000016d0: 2064 6566 206d 696e 5f76 6572 7365 5f6e   def min_verse_n
-000016e0: 756d 2873 656c 662c 2063 6861 705f 6e75  um(self, chap_nu
-000016f0: 6d3a 2069 6e74 2c20 666c 6167 733a 2042  m: int, flags: B
-00001700: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-00001710: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00001720: 2027 2727 5265 7475 726e 2074 6865 206c   '''Return the l
-00001730: 6f77 6573 7420 7665 7273 6520 6e75 6d62  owest verse numb
-00001740: 6572 2028 3020 6f72 2031 2920 666f 7220  er (0 or 1) for 
-00001750: 7468 6520 7370 6563 6966 6965 6420 6368  the specified ch
-00001760: 6170 7465 7220 6e75 6d62 6572 206f 6620  apter number of 
-00001770: 7468 6973 2060 4269 626c 6542 6f6f 6b60  this `BibleBook`
-00001780: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00001790: 2020 2020 2020 666c 6167 7320 3d20 666c        flags = fl
-000017a0: 6167 7320 6f72 2062 6962 6c65 7265 662e  ags or bibleref.
-000017b0: 666c 6167 7320 6f72 2042 6962 6c65 466c  flags or BibleFl
-000017c0: 6167 2e4e 4f4e 450a 2020 2020 2020 2020  ag.NONE.        
-000017d0: 6966 2063 6861 705f 6e75 6d20 3c20 7365  if chap_num < se
-000017e0: 6c66 2e6d 696e 5f63 6861 705f 6e75 6d28  lf.min_chap_num(
-000017f0: 2920 6f72 2063 6861 705f 6e75 6d20 3e20  ) or chap_num > 
-00001800: 7365 6c66 2e6d 6178 5f63 6861 705f 6e75  self.max_chap_nu
-00001810: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
-00001820: 2072 6169 7365 2049 6e76 616c 6964 5265   raise InvalidRe
-00001830: 6665 7265 6e63 6545 7272 6f72 2866 224e  ferenceError(f"N
-00001840: 6f20 6368 6170 7465 7220 7b63 6861 705f  o chapter {chap_
-00001850: 6e75 6d7d 2069 6e20 7b73 656c 662e 7469  num} in {self.ti
-00001860: 746c 657d 2229 0a20 2020 2020 2020 2072  tle}").        r
-00001870: 6574 7572 6e20 3020 6966 2028 4269 626c  eturn 0 if (Bibl
-00001880: 6546 6c61 672e 5645 5253 455f 3020 696e  eFlag.VERSE_0 in
-00001890: 2066 6c61 6773 2061 6e64 2063 6861 705f   flags and chap_
-000018a0: 6e75 6d20 696e 2073 656c 662e 5f76 6572  num in self._ver
-000018b0: 7365 5f30 7329 2065 6c73 6520 310a 0a20  se_0s) else 1.. 
-000018c0: 2020 2064 6566 206d 6178 5f76 6572 7365     def max_verse
-000018d0: 5f6e 756d 2873 656c 662c 2063 6861 705f  _num(self, chap_
-000018e0: 6e75 6d3a 2069 6e74 2920 2d3e 2069 6e74  num: int) -> int
-000018f0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
-00001900: 7572 6e20 7468 6520 6869 6768 6573 7420  urn the highest 
-00001910: 7665 7273 6520 6e75 6d62 6572 2066 6f72  verse number for
-00001920: 2074 6865 2073 7065 6369 6669 6564 2063   the specified c
-00001930: 6861 7074 6572 206e 756d 6265 7220 6f66  hapter number of
-00001940: 2074 6869 7320 6042 6962 6c65 426f 6f6b   this `BibleBook
-00001950: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
-00001960: 2020 2020 2020 2069 6620 6368 6170 5f6e         if chap_n
-00001970: 756d 203c 2073 656c 662e 6d69 6e5f 6368  um < self.min_ch
-00001980: 6170 5f6e 756d 2829 206f 7220 6368 6170  ap_num() or chap
-00001990: 5f6e 756d 203e 2073 656c 662e 6d61 785f  _num > self.max_
-000019a0: 6368 6170 5f6e 756d 2829 3a0a 2020 2020  chap_num():.    
-000019b0: 2020 2020 2020 2020 7261 6973 6520 496e          raise In
-000019c0: 7661 6c69 6452 6566 6572 656e 6365 4572  validReferenceEr
-000019d0: 726f 7228 6622 4e6f 2063 6861 7074 6572  ror(f"No chapter
-000019e0: 207b 6368 6170 5f6e 756d 7d20 696e 207b   {chap_num} in {
-000019f0: 7365 6c66 2e74 6974 6c65 7d22 290a 2020  self.title}").  
-00001a00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001a10: 662e 5f6d 6178 5f76 6572 7365 735b 6368  f._max_verses[ch
-00001a20: 6170 5f6e 756d 2d31 5d0a 0a20 2020 2064  ap_num-1]..    d
-00001a30: 6566 2066 6972 7374 5f76 6572 7365 2873  ef first_verse(s
-00001a40: 656c 662c 2063 6861 705f 6e75 6d3a 2069  elf, chap_num: i
-00001a50: 6e74 203d 204e 6f6e 652c 2066 6c61 6773  nt = None, flags
-00001a60: 3a20 4269 626c 6546 6c61 6720 3d20 4e6f  : BibleFlag = No
-00001a70: 6e65 2920 2d3e 2027 4269 626c 6556 6572  ne) -> 'BibleVer
-00001a80: 7365 273a 0a20 2020 2020 2020 2027 2727  se':.        '''
-00001a90: 5265 7475 726e 7320 6120 6042 6962 6c65  Returns a `Bible
-00001aa0: 5665 7273 6560 2066 6f72 2074 6865 2066  Verse` for the f
-00001ab0: 6972 7374 2076 6572 7365 206f 6620 7468  irst verse of th
-00001ac0: 6520 7370 6563 6966 6965 6420 6368 6170  e specified chap
-00001ad0: 7465 7220 6f66 2074 6869 7320 6042 6962  ter of this `Bib
-00001ae0: 6c65 426f 6f6b 602e 0a20 2020 2020 2020  leBook`..       
-00001af0: 2049 6620 6368 6170 2069 7320 604e 6f6e   If chap is `Non
-00001b00: 6560 2c20 6974 2072 6574 7572 6e73 2074  e`, it returns t
-00001b10: 6865 2066 6972 7374 2076 6572 7365 206f  he first verse o
-00001b20: 6620 7468 6520 656e 7469 7265 2062 6f6f  f the entire boo
-00001b30: 6b2e 0a20 2020 2020 2020 2027 2727 0a20  k..        '''. 
-00001b40: 2020 2020 2020 2069 6620 6368 6170 5f6e         if chap_n
-00001b50: 756d 2069 7320 4e6f 6e65 3a0a 2020 2020  um is None:.    
-00001b60: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
-00001b70: 203d 2073 656c 662e 6d69 6e5f 6368 6170   = self.min_chap
-00001b80: 5f6e 756d 2829 0a20 2020 2020 2020 2072  _num().        r
-00001b90: 6574 7572 6e20 4269 626c 6556 6572 7365  eturn BibleVerse
-00001ba0: 2873 656c 662c 2063 6861 705f 6e75 6d2c  (self, chap_num,
-00001bb0: 2073 656c 662e 6d69 6e5f 7665 7273 655f   self.min_verse_
-00001bc0: 6e75 6d28 6368 6170 5f6e 756d 2c20 666c  num(chap_num, fl
-00001bd0: 6167 7329 2920 2020 2020 2020 200a 0a20  ags))        .. 
-00001be0: 2020 2064 6566 206c 6173 745f 7665 7273     def last_vers
-00001bf0: 6528 7365 6c66 2c20 6368 6170 5f6e 756d  e(self, chap_num
-00001c00: 3a20 696e 7420 3d20 4e6f 6e65 2920 2d3e  : int = None) ->
-00001c10: 2027 4269 626c 6556 6572 7365 273a 0a20   'BibleVerse':. 
-00001c20: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-00001c30: 7320 6120 6042 6962 6c65 5665 7273 6560  s a `BibleVerse`
-00001c40: 2066 6f72 2074 6865 206c 6173 7420 7665   for the last ve
-00001c50: 7273 6520 6f66 2074 6865 2073 7065 6369  rse of the speci
-00001c60: 6669 6564 2063 6861 7074 6572 206f 6620  fied chapter of 
-00001c70: 7468 6973 2060 4269 626c 6542 6f6f 6b60  this `BibleBook`
-00001c80: 2e0a 2020 2020 2020 2020 4966 2063 6861  ..        If cha
-00001c90: 7020 6973 2060 4e6f 6e65 602c 2069 7420  p is `None`, it 
-00001ca0: 7265 7475 726e 7320 7468 6520 6c61 7374  returns the last
-00001cb0: 2076 6572 7365 206f 6620 7468 6520 656e   verse of the en
-00001cc0: 7469 7265 2062 6f6f 6b2e 0a20 2020 2020  tire book..     
-00001cd0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-00001ce0: 6620 6368 6170 5f6e 756d 2069 7320 4e6f  f chap_num is No
-00001cf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001d00: 6368 6170 5f6e 756d 203d 2073 656c 662e  chap_num = self.
-00001d10: 6d61 785f 6368 6170 5f6e 756d 2829 0a20  max_chap_num(). 
-00001d20: 2020 2020 2020 2072 6574 7572 6e20 4269         return Bi
-00001d30: 626c 6556 6572 7365 2873 656c 662c 2063  bleVerse(self, c
-00001d40: 6861 705f 6e75 6d2c 2073 656c 662e 6d61  hap_num, self.ma
-00001d50: 785f 7665 7273 655f 6e75 6d28 6368 6170  x_verse_num(chap
-00001d60: 5f6e 756d 2929 2020 2020 2020 2020 0a0a  _num))        ..
-00001d70: 2020 2020 6465 6620 6e65 7874 2873 656c      def next(sel
-00001d80: 6629 202d 3e20 2742 6962 6c65 426f 6f6b  f) -> 'BibleBook
-00001d90: 273a 0a20 2020 2020 2020 2027 2727 5265  ':.        '''Re
-00001da0: 7475 726e 7320 7468 6520 6e65 7874 2060  turns the next `
-00001db0: 4269 626c 6542 6f6f 6b60 2069 6e20 7468  BibleBook` in th
-00001dc0: 6520 626f 6f6b 206f 7264 6572 696e 672c  e book ordering,
-00001dd0: 206f 7220 604e 6f6e 6560 2069 6620 7468   or `None` if th
-00001de0: 6973 2069 7320 7468 6520 6669 6e61 6c20  is is the final 
-00001df0: 626f 6f6b 2c0a 2020 2020 2020 2020 6f72  book,.        or
-00001e00: 2069 7320 6e6f 7420 7061 7274 206f 6620   is not part of 
-00001e10: 7468 6520 6f72 6465 7269 6e67 2e0a 2020  the ordering..  
-00001e20: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00001e30: 2020 6966 2073 656c 662e 6f72 6465 7220    if self.order 
-00001e40: 6973 204e 6f6e 6520 6f72 2073 656c 662e  is None or self.
-00001e50: 6f72 6465 7220 3d3d 206c 656e 2862 6962  order == len(bib
-00001e60: 6c65 5f64 6174 6128 292e 626f 6f6b 5f6f  le_data().book_o
-00001e70: 7264 6572 292d 313a 0a20 2020 2020 2020  rder)-1:.       
-00001e80: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00001e90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001ea0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001eb0: 6e20 6269 626c 655f 6461 7461 2829 2e62  n bible_data().b
-00001ec0: 6f6f 6b5f 6f72 6465 725b 7365 6c66 2e6f  ook_order[self.o
-00001ed0: 7264 6572 2b31 5d0a 0a20 2020 2064 6566  rder+1]..    def
-00001ee0: 2070 7265 7628 7365 6c66 2920 2d3e 2027   prev(self) -> '
-00001ef0: 4269 626c 6542 6f6f 6b27 3a0a 2020 2020  BibleBook':.    
-00001f00: 2020 2020 2727 2752 6574 7572 6e73 2074      '''Returns t
-00001f10: 6865 2070 7265 7669 6f75 7320 6042 6962  he previous `Bib
-00001f20: 6c65 426f 6f6b 6020 696e 2074 6865 2062  leBook` in the b
-00001f30: 6f6f 6b20 6f72 6465 7269 6e67 2c20 6f72  ook ordering, or
-00001f40: 2060 4e6f 6e65 6020 6966 2074 6869 7320   `None` if this 
-00001f50: 6973 2074 6865 2066 6972 7374 2062 6f6f  is the first boo
-00001f60: 6b2c 0a20 2020 2020 2020 206f 7220 6973  k,.        or is
-00001f70: 206e 6f74 2070 6172 7420 6f66 2074 6865   not part of the
-00001f80: 206f 7264 6572 696e 672e 0a20 2020 2020   ordering..     
-00001f90: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-00001fa0: 6620 7365 6c66 2e6f 7264 6572 2069 7320  f self.order is 
-00001fb0: 4e6f 6e65 206f 7220 7365 6c66 2e6f 7264  None or self.ord
-00001fc0: 6572 203d 3d20 303a 0a20 2020 2020 2020  er == 0:.       
-00001fd0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00001fe0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002000: 6e20 6269 626c 655f 6461 7461 2829 2e62  n bible_data().b
-00002010: 6f6f 6b5f 6f72 6465 725b 7365 6c66 2e6f  ook_order[self.o
-00002020: 7264 6572 2d31 5d0a 0a20 2020 2064 6566  rder-1]..    def
-00002030: 2072 616e 6765 2873 656c 662c 2066 6c61   range(self, fla
-00002040: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-00002050: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
-00002060: 616e 6765 273a 0a20 2020 2020 2020 2027  ange':.        '
-00002070: 2727 5265 7475 726e 7320 6120 6042 6962  ''Returns a `Bib
-00002080: 6c65 5261 6e67 6560 2073 7061 6e6e 696e  leRange` spannin
-00002090: 6720 7468 6973 2065 6e74 6972 6520 6042  g this entire `B
-000020a0: 6962 6c65 426f 6f6b 602e 0a20 2020 2020  ibleBook`..     
-000020b0: 2020 2027 2727 0a20 2020 2020 2020 2072     '''.        r
-000020c0: 6574 7572 6e20 4269 626c 6552 616e 6765  eturn BibleRange
-000020d0: 2873 7461 7274 3d73 656c 662e 6669 7273  (start=self.firs
-000020e0: 745f 7665 7273 6528 666c 6167 733d 666c  t_verse(flags=fl
-000020f0: 6167 7329 2c20 656e 643d 7365 6c66 2e6c  ags), end=self.l
-00002100: 6173 745f 7665 7273 6528 292c 2066 6c61  ast_verse(), fla
-00002110: 6773 3d66 6c61 6773 290a 0a20 2020 2064  gs=flags)..    d
-00002120: 6566 2063 6861 705f 7261 6e67 6528 7365  ef chap_range(se
-00002130: 6c66 2c20 6368 6170 5f6e 756d 3a20 696e  lf, chap_num: in
-00002140: 742c 2066 6c61 6773 3a20 4269 626c 6546  t, flags: BibleF
-00002150: 6c61 6720 3d20 4e6f 6e65 2920 2d3e 2027  lag = None) -> '
-00002160: 4269 626c 6552 616e 6765 273a 0a20 2020  BibleRange':.   
-00002170: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
-00002180: 6120 6042 6962 6c65 5261 6e67 6560 2073  a `BibleRange` s
-00002190: 7061 6e6e 696e 6720 7468 6520 656e 7469  panning the enti
-000021a0: 7265 6420 7370 6563 6966 6965 6420 6368  red specified ch
-000021b0: 6170 7465 7220 6f66 2074 6869 7320 6042  apter of this `B
-000021c0: 6962 6c65 426f 6f6b 602e 0a20 2020 2020  ibleBook`..     
-000021d0: 2020 2027 2727 0a20 2020 2020 2020 2072     '''.        r
-000021e0: 6574 7572 6e20 4269 626c 6552 616e 6765  eturn BibleRange
-000021f0: 2873 7461 7274 3d73 656c 662e 6669 7273  (start=self.firs
-00002200: 745f 7665 7273 6528 6368 6170 5f6e 756d  t_verse(chap_num
-00002210: 2c20 666c 6167 733d 666c 6167 7329 2c20  , flags=flags), 
-00002220: 656e 643d 7365 6c66 2e6c 6173 745f 7665  end=self.last_ve
-00002230: 7273 6528 6368 6170 5f6e 756d 292c 2066  rse(chap_num), f
-00002240: 6c61 6773 3d66 6c61 6773 290a 0a20 2020  lags=flags)..   
-00002250: 2064 6566 2063 6861 705f 7261 6e67 6573   def chap_ranges
-00002260: 2873 656c 662c 2072 6567 726f 7570 3a20  (self, regroup: 
-00002270: 626f 6f6c 203d 2054 7275 652c 2066 6c61  bool = True, fla
-00002280: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-00002290: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
-000022a0: 616e 6765 4c69 7374 273a 0a20 2020 2020  angeList':.     
-000022b0: 2020 2027 2727 436f 6e76 656e 6965 6e63     '''Convenienc
-000022c0: 6520 6d65 7468 6f64 2074 6861 7420 7265  e method that re
-000022d0: 7475 726e 7320 6120 6042 6962 6c65 5261  turns a `BibleRa
-000022e0: 6e67 654c 6973 7460 206f 6620 7468 6520  ngeList` of the 
-000022f0: 7261 6e67 6573 2066 6f72 2065 6163 6820  ranges for each 
-00002300: 6368 6170 7465 7220 696e 2074 6869 7320  chapter in this 
-00002310: 6042 6962 6c65 426f 6f6b 602e 0a20 2020  `BibleBook`..   
-00002320: 2020 2020 200a 2020 2020 2020 2020 4966       .        If
-00002330: 2060 7265 6772 6f75 7060 2069 7320 6054   `regroup` is `T
-00002340: 7275 6560 2c20 7265 6772 6f75 7028 2920  rue`, regroup() 
-00002350: 6973 2063 616c 6c65 6420 6f6e 2074 6865  is called on the
-00002360: 2072 6573 756c 7469 6e67 2060 4269 626c   resulting `Bibl
-00002370: 6552 616e 6765 4c69 7374 602e 0a0a 2020  eRangeList`...  
-00002380: 2020 2020 2020 4571 7569 7661 6c65 6e74        Equivalent
-00002390: 2074 6f20 6073 656c 662e 7261 6e67 6528   to `self.range(
-000023a0: 666c 6167 733d 666c 6167 7329 2e73 706c  flags=flags).spl
-000023b0: 6974 2862 795f 6368 6170 3d54 7275 652c  it(by_chap=True,
-000023c0: 2072 6567 726f 7570 3d72 6567 726f 7570   regroup=regroup
-000023d0: 2c20 666c 6167 733d 666c 6167 7329 600a  , flags=flags)`.
-000023e0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000023f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002400: 7261 6e67 6528 666c 6167 733d 666c 6167  range(flags=flag
-00002410: 7329 2e73 706c 6974 2862 795f 6368 6170  s).split(by_chap
-00002420: 3d54 7275 652c 2072 6567 726f 7570 3d72  =True, regroup=r
-00002430: 6567 726f 7570 2c20 666c 6167 733d 666c  egroup, flags=fl
-00002440: 6167 7329 0a0a 2020 2020 6465 6620 5f5f  ags)..    def __
-00002450: 6c74 5f5f 2873 656c 662c 206f 7468 6572  lt__(self, other
-00002460: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-00002470: 7420 6973 696e 7374 616e 6365 286f 7468  t isinstance(oth
-00002480: 6572 2c20 4269 626c 6542 6f6f 6b29 3a0a  er, BibleBook):.
-00002490: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000024a0: 726e 204e 6f74 496d 706c 656d 656e 7465  rn NotImplemente
-000024b0: 640a 2020 2020 2020 2020 656c 7365 3a0a  d.        else:.
-000024c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000024d0: 726e 2073 656c 662e 6f72 6465 7220 3c20  rn self.order < 
-000024e0: 6f74 6865 722e 6f72 6465 720a 0a20 2020  other.order..   
-000024f0: 2064 6566 205f 5f6c 655f 5f28 7365 6c66   def __le__(self
-00002500: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00002510: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00002520: 6e63 6528 6f74 6865 722c 2042 6962 6c65  nce(other, Bible
-00002530: 426f 6f6b 293a 0a20 2020 2020 2020 2020  Book):.         
-00002540: 2020 2072 6574 7572 6e20 4e6f 7449 6d70     return NotImp
-00002550: 6c65 6d65 6e74 6564 0a20 2020 2020 2020  lemented.       
-00002560: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002570: 2020 2072 6574 7572 6e20 7365 6c66 2e6f     return self.o
-00002580: 7264 6572 203c 3d20 6f74 6865 722e 6f72  rder <= other.or
-00002590: 6465 720a 0a20 2020 2064 6566 205f 5f67  der..    def __g
-000025a0: 745f 5f28 7365 6c66 2c20 6f74 6865 7229  t__(self, other)
-000025b0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-000025c0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-000025d0: 722c 2042 6962 6c65 426f 6f6b 293a 0a20  r, BibleBook):. 
-000025e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000025f0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
-00002600: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00002610: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002620: 6e20 7365 6c66 2e6f 7264 6572 203e 206f  n self.order > o
-00002630: 7468 6572 2e6f 7264 6572 0a0a 2020 2020  ther.order..    
-00002640: 6465 6620 5f5f 6765 5f5f 2873 656c 662c  def __ge__(self,
-00002650: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00002660: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00002670: 6365 286f 7468 6572 2c20 4269 626c 6542  ce(other, BibleB
-00002680: 6f6f 6b29 3a0a 2020 2020 2020 2020 2020  ook):.          
-00002690: 2020 7265 7475 726e 204e 6f74 496d 706c    return NotImpl
-000026a0: 656d 656e 7465 640a 2020 2020 2020 2020  emented.        
-000026b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000026c0: 2020 7265 7475 726e 2073 656c 662e 6f72    return self.or
-000026d0: 6465 7220 3e3d 206f 7468 6572 2e6f 7264  der >= other.ord
-000026e0: 6572 0a0a 0a23 2057 6520 6465 6c61 7920  er...# We delay 
-000026f0: 7468 6573 6520 696d 706f 7274 7320 756e  these imports un
-00002700: 7469 6c20 7468 6973 2070 6f69 6e74 2073  til this point s
-00002710: 6f20 7468 6174 2042 6962 6c65 426f 6f6b  o that BibleBook
-00002720: 2061 6e64 2069 7473 2072 656c 6174 6564   and its related
-00002730: 2063 6c61 7373 6573 0a23 2061 7265 2061   classes.# are a
-00002740: 6c72 6561 6479 2064 6566 696e 6564 2061  lready defined a
-00002750: 6e64 2063 616e 2062 6520 7573 6564 2062  nd can be used b
-00002760: 7920 6f74 6865 7220 7369 626c 696e 6720  y other sibling 
-00002770: 6d6f 6475 6c65 730a 6672 6f6d 202e 2069  modules.from . i
-00002780: 6d70 6f72 7420 7061 7273 6572 0a66 726f  mport parser.fro
-00002790: 6d20 2e20 696d 706f 7274 2075 7469 6c0a  m . import util.
-000027a0: 6672 6f6d 202e 2069 6d70 6f72 7420 6461  from . import da
-000027b0: 7461 0a0a 0a63 6c61 7373 2042 6962 6c65  ta...class Bible
-000027c0: 5665 7273 6550 6172 7428 466c 6167 293a  VersePart(Flag):
-000027d0: 0a20 2020 2027 2727 466c 6167 7320 666f  .    '''Flags fo
-000027e0: 7220 7265 6665 7272 696e 6720 746f 2074  r referring to t
-000027f0: 6865 2033 2070 7269 6d61 7279 2061 7474  he 3 primary att
-00002800: 7269 6275 7465 7320 6f66 2061 2042 6962  ributes of a Bib
-00002810: 6c65 5665 7273 652e 0a20 2020 200a 2020  leVerse..    .  
-00002820: 2020 4d61 696e 6c79 2075 7365 6420 696e    Mainly used in
-00002830: 7465 726e 616c 6c79 2066 6f72 2063 6f6e  ternally for con
-00002840: 7665 7274 696e 6720 4269 626c 6520 7265  verting Bible re
-00002850: 6665 7265 6e63 6573 2073 7472 696e 6773  ferences strings
-00002860: 2c20 746f 2069 6e64 6963 6174 6520 7768  , to indicate wh
-00002870: 6963 6820 6174 7472 6962 7574 6573 2077  ich attributes w
-00002880: 696c 6c20 6469 7370 6c61 7920 696e 0a20  ill display in. 
-00002890: 2020 2061 2073 7472 696e 6720 7265 7072     a string repr
-000028a0: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
-000028b0: 2727 270a 2020 2020 4e4f 4e45 2020 2020  '''.    NONE    
-000028c0: 3d20 300a 2020 2020 424f 4f4b 2020 2020  = 0.    BOOK    
-000028d0: 3d20 6175 746f 2829 2020 200a 2020 2020  = auto()   .    
-000028e0: 4348 4150 2020 2020 3d20 6175 746f 2829  CHAP    = auto()
-000028f0: 0a20 2020 2056 4552 5345 2020 203d 2061  .    VERSE   = a
-00002900: 7574 6f28 290a 2020 2020 4655 4c4c 5f52  uto().    FULL_R
-00002910: 4546 2020 2020 3d20 424f 4f4b 207c 2043  EF    = BOOK | C
-00002920: 4841 5020 7c20 5645 5253 450a 2020 2020  HAP | VERSE.    
-00002930: 424f 4f4b 5f43 4841 5020 2020 3d20 424f  BOOK_CHAP   = BO
-00002940: 4f4b 207c 2043 4841 500a 2020 2020 424f  OK | CHAP.    BO
-00002950: 4f4b 5f56 4552 5345 2020 3d20 424f 4f4b  OK_VERSE  = BOOK
-00002960: 207c 2056 4552 5345 0a20 2020 2043 4841   | VERSE.    CHA
-00002970: 505f 5645 5253 4520 203d 2043 4841 5020  P_VERSE  = CHAP 
-00002980: 7c20 5645 5253 450a 0a0a 4064 6174 6163  | VERSE...@datac
-00002990: 6c61 7373 2869 6e69 743d 4661 6c73 652c  lass(init=False,
-000029a0: 2072 6570 723d 4661 6c73 652c 2065 713d   repr=False, eq=
-000029b0: 5472 7565 2c20 6f72 6465 723d 5472 7565  True, order=True
-000029c0: 2c20 6672 6f7a 656e 3d54 7275 6529 0a63  , frozen=True).c
-000029d0: 6c61 7373 2042 6962 6c65 5665 7273 653a  lass BibleVerse:
-000029e0: 0a20 2020 2027 2727 4120 7265 6665 7265  .    '''A refere
-000029f0: 6e63 6520 746f 2061 2073 696e 676c 6520  nce to a single 
-00002a00: 4269 626c 6520 7665 7273 6520 2865 2e67  Bible verse (e.g
-00002a10: 2e20 4d61 7474 2032 3a33 292e 0a0a 2020  . Matt 2:3)...  
-00002a20: 2020 436f 6e74 6169 6e73 2033 2070 7269    Contains 3 pri
-00002a30: 6d61 7279 2061 7474 7269 6275 7465 733a  mary attributes:
-00002a40: 0a20 2020 2020 2d20 6062 6f6f 6b60 3a20  .     - `book`: 
-00002a50: 2020 2020 2020 5468 6520 6042 6962 6c65        The `Bible
-00002a60: 426f 6f6b 6020 6f66 2074 6865 2062 6f6f  Book` of the boo
-00002a70: 6b20 6f66 2074 6865 2072 6566 6572 656e  k of the referen
-00002a80: 6365 2e0a 2020 2020 202d 2060 6368 6170  ce..     - `chap
-00002a90: 5f6e 756d 603a 2020 2054 6865 2063 6861  _num`:   The cha
-00002aa0: 7074 6572 206e 756d 6265 7220 2869 6e64  pter number (ind
-00002ab0: 6578 6564 2066 726f 6d20 3129 206f 6620  exed from 1) of 
-00002ac0: 7468 6520 7265 6665 7265 6e63 652e 0a20  the reference.. 
-00002ad0: 2020 2020 2d20 6076 6572 7365 5f6e 756d      - `verse_num
-00002ae0: 603a 2020 5468 6520 7665 7273 6520 6e75  `:  The verse nu
-00002af0: 6d62 6572 2028 696e 6465 7865 6420 6672  mber (indexed fr
-00002b00: 6f6d 2030 206f 7220 3129 206f 6620 7468  om 0 or 1) of th
-00002b10: 6520 7265 6665 7265 6e63 652e 0a0a 2020  e reference...  
-00002b20: 2020 4269 626c 6556 6572 7365 7320 6172    BibleVerses ar
-00002b30: 6520 696d 6d75 7461 626c 652e 2054 6865  e immutable. The
-00002b40: 7920 6361 6e20 6265 2063 6f6d 7061 7265  y can be compare
-00002b50: 6420 7573 696e 6720 7468 6520 7374 616e  d using the stan
-00002b60: 6461 7264 2063 6f6d 7061 7269 736f 6e20  dard comparison 
-00002b70: 6f70 6572 6174 6f72 732c 2077 6869 6368  operators, which
-00002b80: 2063 6f6d 7061 7265 2074 6865 0a20 2020   compare the.   
-00002b90: 2060 626f 6f6b 602c 2060 6368 6170 5f6e   `book`, `chap_n
-00002ba0: 756d 6020 616e 6420 6076 6572 7365 5f6e  um` and `verse_n
-00002bb0: 756d 6020 696e 2074 6861 7420 6f72 6465  um` in that orde
-00002bc0: 722e 0a20 2020 2027 2727 0a20 2020 2062  r..    '''.    b
-00002bd0: 6f6f 6b3a 2020 2020 2020 2042 6962 6c65  ook:       Bible
-00002be0: 426f 6f6b 0a20 2020 2063 6861 705f 6e75  Book.    chap_nu
-00002bf0: 6d3a 2020 2069 6e74 0a20 2020 2076 6572  m:   int.    ver
-00002c00: 7365 5f6e 756d 3a20 2069 6e74 0a0a 2020  se_num:  int..  
-00002c10: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00002c20: 656c 662c 202a 6172 6773 2c20 666c 6167  elf, *args, flag
-00002c30: 733a 2042 6962 6c65 466c 6167 203d 204e  s: BibleFlag = N
-00002c40: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
-00002c50: 2741 2060 4269 626c 6556 6572 7365 6020  'A `BibleVerse` 
-00002c60: 6361 6e20 6265 2063 6f6e 7374 7275 6374  can be construct
-00002c70: 6564 2069 6e20 616e 7920 6f66 2074 6865  ed in any of the
-00002c80: 2066 6f6c 6c6f 7769 6e67 2077 6179 733a   following ways:
-00002c90: 0a0a 2020 2020 2020 2020 312e 2046 726f  ..        1. Fro
-00002ca0: 6d20 6120 7369 6e67 6c65 2073 7472 696e  m a single strin
-00002cb0: 673a 2060 4269 626c 6556 6572 7365 2822  g: `BibleVerse("
-00002cc0: 4d61 726b 2032 3a33 2229 600a 0a20 2020  Mark 2:3")`..   
-00002cd0: 2020 2020 2020 2020 5261 6973 6573 2061          Raises a
-00002ce0: 2060 4269 626c 6552 6566 5061 7273 696e   `BibleRefParsin
-00002cf0: 6745 7272 6f72 6020 6966 2074 6865 2073  gError` if the s
-00002d00: 7472 696e 6720 6361 6e6e 6f74 2062 6520  tring cannot be 
-00002d10: 7061 7273 6564 2e0a 0a20 2020 2020 2020  parsed...       
-00002d20: 2032 2e20 4672 6f6d 2061 2042 6962 6c65   2. From a Bible
-00002d30: 2062 6f6f 6b2c 2063 6861 7074 6572 2061   book, chapter a
-00002d40: 6e64 2076 6572 7365 206e 756d 6265 7273  nd verse numbers
-00002d50: 2e20 5468 6520 4269 626c 6520 626f 6f6b  . The Bible book
-00002d60: 2063 616e 2062 6520 6120 7374 7269 6e67   can be a string
-00002d70: 206e 616d 652c 206f 7220 6120 6042 6962   name, or a `Bib
-00002d80: 6c65 426f 6f6b 6020 656e 756d 3a0a 2020  leBook` enum:.  
-00002d90: 2020 2020 2020 2020 2060 4269 626c 6556           `BibleV
-00002da0: 6572 7365 2822 4d61 726b 222c 2032 2c20  erse("Mark", 2, 
-00002db0: 3329 602c 206f 7220 6042 6962 6c65 5665  3)`, or `BibleVe
-00002dc0: 7273 6528 4269 626c 6542 6f6f 6b2e 4d61  rse(BibleBook.Ma
-00002dd0: 726b 2c20 322c 2033 2960 0a20 2020 2020  rk, 2, 3)`.     
-00002de0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002df0: 332e 2041 7320 6120 636f 7079 206f 6620  3. As a copy of 
-00002e00: 616e 6f74 6865 7220 4269 626c 6556 6572  another BibleVer
-00002e10: 7365 3a20 6042 6962 6c65 5665 7273 6528  se: `BibleVerse(
-00002e20: 6578 6973 7469 6e67 5f62 6962 6c65 5f76  existing_bible_v
-00002e30: 6572 7365 2960 0a0a 2020 2020 2020 2020  erse)`..        
-00002e40: 4966 2074 6865 2073 7570 706c 6965 6420  If the supplied 
-00002e50: 6172 6775 6d65 6e74 7320 6172 6520 6e6f  arguments are no
-00002e60: 7420 6120 7661 6c69 6420 7665 7273 652c  t a valid verse,
-00002e70: 2061 6e20 6049 6e76 616c 6964 5265 6665   an `InvalidRefe
-00002e80: 7265 6e63 6545 7272 6f72 6020 6973 2072  renceError` is r
-00002e90: 6169 7365 642e 0a20 2020 2020 2020 2027  aised..        '
-00002ea0: 2727 0a20 2020 2020 2020 2069 6620 6c65  ''.        if le
-00002eb0: 6e28 6172 6773 2920 3d3d 2031 3a0a 2020  n(args) == 1:.  
-00002ec0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00002ed0: 6e73 7461 6e63 6528 6172 6773 5b30 5d2c  nstance(args[0],
-00002ee0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00002ef0: 2020 2020 2020 2072 616e 6765 5f6c 6973         range_lis
-00002f00: 7420 3d20 4269 626c 6552 616e 6765 4c69  t = BibleRangeLi
-00002f10: 7374 2861 7267 735b 305d 2c20 666c 6167  st(args[0], flag
-00002f20: 733d 666c 6167 7329 0a20 2020 2020 2020  s=flags).       
-00002f30: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00002f40: 7261 6e67 655f 6c69 7374 2920 213d 2031  range_list) != 1
-00002f50: 206f 7220 6e6f 7420 7261 6e67 655f 6c69   or not range_li
-00002f60: 7374 5b30 5d2e 6973 5f73 696e 676c 655f  st[0].is_single_
-00002f70: 7665 7273 6528 293a 0a20 2020 2020 2020  verse():.       
-00002f80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00002f90: 7365 2049 6e76 616c 6964 5265 6665 7265  se InvalidRefere
-00002fa0: 6e63 6545 7272 6f72 2866 2253 7472 696e  nceError(f"Strin
-00002fb0: 6720 6973 206e 6f74 2061 2073 696e 676c  g is not a singl
-00002fc0: 6520 7665 7273 653a 207b 6172 6773 5b30  e verse: {args[0
-00002fd0: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00002fe0: 2020 2020 206f 626a 6563 742e 5f5f 7365       object.__se
-00002ff0: 7461 7474 725f 5f28 7365 6c66 2c20 2262  tattr__(self, "b
-00003000: 6f6f 6b22 2c20 7261 6e67 655f 6c69 7374  ook", range_list
-00003010: 5b30 5d2e 7374 6172 742e 626f 6f6b 290a  [0].start.book).
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
-00003040: 5f5f 2873 656c 662c 2022 6368 6170 5f6e  __(self, "chap_n
-00003050: 756d 222c 2072 616e 6765 5f6c 6973 745b  um", range_list[
-00003060: 305d 2e73 7461 7274 2e63 6861 705f 6e75  0].start.chap_nu
-00003070: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-00003080: 2020 206f 626a 6563 742e 5f5f 7365 7461     object.__seta
-00003090: 7474 725f 5f28 7365 6c66 2c20 2276 6572  ttr__(self, "ver
-000030a0: 7365 5f6e 756d 222c 2072 616e 6765 5f6c  se_num", range_l
-000030b0: 6973 745b 305d 2e73 7461 7274 2e76 6572  ist[0].start.ver
-000030c0: 7365 5f6e 756d 290a 2020 2020 2020 2020  se_num).        
-000030d0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-000030e0: 6e63 6528 6172 6773 5b30 5d2c 2042 6962  nce(args[0], Bib
-000030f0: 6c65 5665 7273 6529 3a0a 2020 2020 2020  leVerse):.      
-00003100: 2020 2020 2020 2020 2020 2320 5765 2068            # We h
-00003110: 6176 6520 746f 2075 7365 206f 626a 6563  ave to use objec
-00003120: 742e 5f5f 7365 7461 7474 725f 5f20 6265  t.__setattr__ be
-00003130: 6361 7573 6520 7468 6520 636c 6173 7320  cause the class 
-00003140: 6973 2066 726f 7a65 6e0a 2020 2020 2020  is frozen.      
-00003150: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-00003160: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
-00003170: 662c 2022 626f 6f6b 222c 2061 7267 735b  f, "book", args[
-00003180: 305d 2e62 6f6f 6b29 0a20 2020 2020 2020  0].book).       
-00003190: 2020 2020 2020 2020 206f 626a 6563 742e           object.
-000031a0: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
-000031b0: 2c20 2263 6861 705f 6e75 6d22 2c20 6172  , "chap_num", ar
-000031c0: 6773 5b30 5d2e 6368 6170 5f6e 756d 290a  gs[0].chap_num).
-000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031e0: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
-000031f0: 5f5f 2873 656c 662c 2022 7665 7273 655f  __(self, "verse_
-00003200: 6e75 6d22 2c20 6172 6773 5b30 5d2e 7665  num", args[0].ve
-00003210: 7273 655f 6e75 6d29 0a20 2020 2020 2020  rse_num).       
-00003220: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003230: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003240: 2056 616c 7565 4572 726f 7228 2253 696e   ValueError("Sin
-00003250: 676c 6520 6172 6775 6d65 6e74 2074 6f20  gle argument to 
-00003260: 4269 626c 6556 6572 7365 2063 616e 206f  BibleVerse can o
-00003270: 6e6c 7920 6265 2061 2073 7472 696e 6720  nly be a string 
-00003280: 6f72 2061 6e6f 7468 6572 2042 6962 6c65  or another Bible
-00003290: 5665 7273 6522 290a 2020 2020 2020 2020  Verse").        
-000032a0: 656c 6966 206c 656e 2861 7267 7329 203e  elif len(args) >
-000032b0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
-000032c0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000032d0: 2822 546f 6f20 6d61 6e79 2061 7267 756d  ("Too many argum
-000032e0: 656e 7473 2073 7570 706c 6965 6420 746f  ents supplied to
-000032f0: 2042 6962 6c65 5665 7273 6522 290a 2020   BibleVerse").  
-00003300: 2020 2020 2020 656c 6966 206c 656e 2861        elif len(a
-00003310: 7267 7329 203c 2033 3a0a 2020 2020 2020  rgs) < 3:.      
-00003320: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003330: 6545 7272 6f72 2822 546f 6f20 6665 7720  eError("Too few 
-00003340: 6172 6775 6d65 6e74 7320 7375 7070 6c69  arguments suppli
-00003350: 6564 2074 6f20 4269 626c 6556 6572 7365  ed to BibleVerse
-00003360: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
-00003370: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
-00003380: 6b20 3d20 6172 6773 5b30 5d0a 2020 2020  k = args[0].    
-00003390: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
-000033a0: 3a20 696e 7420 3d20 6172 6773 5b31 5d0a  : int = args[1].
-000033b0: 2020 2020 2020 2020 2020 2020 7665 7273              vers
-000033c0: 655f 6e75 6d3a 2069 6e74 203d 2061 7267  e_num: int = arg
-000033d0: 735b 325d 0a20 2020 2020 2020 2020 2020  s[2].           
-000033e0: 2069 6620 6973 696e 7374 616e 6365 2862   if isinstance(b
-000033f0: 6f6f 6b2c 2073 7472 293a 0a20 2020 2020  ook, str):.     
-00003400: 2020 2020 2020 2020 2020 2062 6f6f 6b20             book 
-00003410: 3d20 4269 626c 6542 6f6f 6b2e 6672 6f6d  = BibleBook.from
-00003420: 5f73 7472 2862 6f6f 6b2c 2072 6169 7365  _str(book, raise
-00003430: 5f65 7272 6f72 3d54 7275 6529 0a20 2020  _error=True).   
-00003440: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
-00003450: 7420 6973 696e 7374 616e 6365 2862 6f6f  t isinstance(boo
-00003460: 6b2c 2042 6962 6c65 426f 6f6b 293a 0a20  k, BibleBook):. 
-00003470: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003480: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00003490: 6622 7b62 6f6f 6b7d 206d 7573 7420 6265  f"{book} must be
-000034a0: 2061 2073 7472 696e 6720 6f72 2061 6e20   a string or an 
-000034b0: 696e 7374 616e 6365 206f 6620 4269 626c  instance of Bibl
-000034c0: 6542 6f6f 6b22 290a 2020 2020 2020 2020  eBook").        
-000034d0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-000034e0: 7461 6e63 6528 6368 6170 5f6e 756d 2c20  tance(chap_num, 
-000034f0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00003500: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003510: 6545 7272 6f72 2866 227b 6368 6170 5f6e  eError(f"{chap_n
-00003520: 756d 7d20 6973 206e 6f74 2061 6e20 696e  um} is not an in
-00003530: 7465 6765 7220 6368 6170 7465 7220 6e75  teger chapter nu
-00003540: 6d62 6572 2229 0a20 2020 2020 2020 2020  mber").         
-00003550: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00003560: 616e 6365 2876 6572 7365 5f6e 756d 2c20  ance(verse_num, 
-00003570: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00003580: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003590: 6545 7272 6f72 2866 227b 6368 6170 5f6e  eError(f"{chap_n
-000035a0: 756d 7d20 6973 206e 6f74 2061 6e20 696e  um} is not an in
-000035b0: 7465 6765 7220 7665 7273 6520 6e75 6d62  teger verse numb
-000035c0: 6572 2229 0a20 2020 2020 2020 2020 2020  er").           
-000035d0: 2069 6620 6368 6170 5f6e 756d 203c 2062   if chap_num < b
-000035e0: 6f6f 6b2e 6d69 6e5f 6368 6170 5f6e 756d  ook.min_chap_num
-000035f0: 2829 206f 7220 6368 6170 5f6e 756d 203e  () or chap_num >
-00003600: 2062 6f6f 6b2e 6d61 785f 6368 6170 5f6e   book.max_chap_n
-00003610: 756d 2829 3a0a 2020 2020 2020 2020 2020  um():.          
-00003620: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
-00003630: 6c69 6452 6566 6572 656e 6365 4572 726f  lidReferenceErro
-00003640: 7228 6622 4e6f 2063 6861 7074 6572 207b  r(f"No chapter {
-00003650: 6368 6170 5f6e 756d 7d20 696e 207b 626f  chap_num} in {bo
-00003660: 6f6b 2e74 6974 6c65 7d22 290a 2020 2020  ok.title}").    
-00003670: 2020 2020 2020 2020 6966 2076 6572 7365          if verse
-00003680: 5f6e 756d 203c 2062 6f6f 6b2e 6d69 6e5f  _num < book.min_
-00003690: 7665 7273 655f 6e75 6d28 6368 6170 5f6e  verse_num(chap_n
-000036a0: 756d 2c20 666c 6167 7329 206f 7220 7665  um, flags) or ve
-000036b0: 7273 655f 6e75 6d20 3e20 626f 6f6b 2e6d  rse_num > book.m
-000036c0: 6178 5f76 6572 7365 5f6e 756d 2863 6861  ax_verse_num(cha
-000036d0: 705f 6e75 6d29 3a0a 2020 2020 2020 2020  p_num):.        
-000036e0: 2020 2020 2020 2020 7261 6973 6520 496e          raise In
-000036f0: 7661 6c69 6452 6566 6572 656e 6365 4572  validReferenceEr
-00003700: 726f 7228 6622 4e6f 2076 6572 7365 207b  ror(f"No verse {
-00003710: 7665 7273 655f 6e75 6d7d 2069 6e20 7b62  verse_num} in {b
-00003720: 6f6f 6b2e 7469 746c 657d 207b 6368 6170  ook.title} {chap
-00003730: 5f6e 756d 7d22 290a 2020 2020 2020 2020  _num}").        
-00003740: 2020 2020 6f62 6a65 6374 2e5f 5f73 6574      object.__set
-00003750: 6174 7472 5f5f 2873 656c 662c 2022 626f  attr__(self, "bo
-00003760: 6f6b 222c 2062 6f6f 6b29 2023 2057 6520  ok", book) # We 
-00003770: 6861 7665 2074 6f20 7573 6520 6f62 6a65  have to use obje
-00003780: 6374 2e5f 5f73 6574 6174 7472 5f5f 2062  ct.__setattr__ b
-00003790: 6563 6175 7365 2074 6865 2063 6c61 7373  ecause the class
-000037a0: 2069 7320 6672 6f7a 656e 0a20 2020 2020   is frozen.     
-000037b0: 2020 2020 2020 206f 626a 6563 742e 5f5f         object.__
-000037c0: 7365 7461 7474 725f 5f28 7365 6c66 2c20  setattr__(self, 
-000037d0: 2263 6861 705f 6e75 6d22 2c20 6368 6170  "chap_num", chap
-000037e0: 5f6e 756d 290a 2020 2020 2020 2020 2020  _num).          
-000037f0: 2020 6f62 6a65 6374 2e5f 5f73 6574 6174    object.__setat
-00003800: 7472 5f5f 2873 656c 662c 2022 7665 7273  tr__(self, "vers
-00003810: 655f 6e75 6d22 2c20 7665 7273 655f 6e75  e_num", verse_nu
-00003820: 6d29 0a0a 2020 2020 6465 6620 7665 7273  m)..    def vers
-00003830: 655f 305f 746f 5f31 2873 656c 6629 202d  e_0_to_1(self) -
-00003840: 3e20 2742 6962 6c65 5665 7273 6527 3a0a  > 'BibleVerse':.
-00003850: 2020 2020 2020 2020 2727 2749 6620 7468          '''If th
-00003860: 6520 6076 6572 7365 5f6e 756d 6020 6f66  e `verse_num` of
-00003870: 2074 6869 7320 6042 6962 6c65 5665 7273   this `BibleVers
-00003880: 6560 2069 7320 302c 2072 6574 7572 6e73  e` is 0, returns
-00003890: 2061 6e20 6964 656e 7469 6361 6c20 4269   an identical Bi
-000038a0: 626c 6556 6572 7365 2065 7863 6570 7420  bleVerse except 
-000038b0: 7769 7468 2060 7665 7273 655f 6e75 6d60  with `verse_num`
-000038c0: 0a20 2020 2020 2020 2073 6574 2074 6f20  .        set to 
-000038d0: 312e 204f 7468 6572 7769 7365 2c20 7265  1. Otherwise, re
-000038e0: 7475 726e 7320 7468 6520 6f72 6967 696e  turns the origin
-000038f0: 616c 2060 4269 626c 6556 6572 7365 602e  al `BibleVerse`.
-00003900: 2727 270a 2020 2020 2020 2020 6966 2073  '''.        if s
-00003910: 656c 662e 7665 7273 655f 6e75 6d20 3d3d  elf.verse_num ==
-00003920: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00003930: 7265 7475 726e 2042 6962 6c65 5665 7273  return BibleVers
-00003940: 6528 7365 6c66 2e62 6f6f 6b2c 2073 656c  e(self.book, sel
-00003950: 662e 6368 6170 5f6e 756d 2c20 3129 0a20  f.chap_num, 1). 
-00003960: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003970: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003980: 7365 6c66 0a20 2020 200a 2020 2020 6465  self.    .    de
-00003990: 6620 7665 7273 655f 315f 746f 5f30 2873  f verse_1_to_0(s
-000039a0: 656c 6629 202d 3e20 2742 6962 6c65 5665  elf) -> 'BibleVe
-000039b0: 7273 6527 3a0a 2020 2020 2020 2020 2727  rse':.        ''
-000039c0: 2749 6620 7468 6520 6076 6572 7365 5f6e  'If the `verse_n
-000039d0: 756d 6020 6f66 2074 6869 7320 6042 6962  um` of this `Bib
-000039e0: 6c65 5665 7273 6560 2069 7320 312c 2061  leVerse` is 1, a
-000039f0: 6e64 2061 2076 6572 7365 2030 2069 7320  nd a verse 0 is 
-00003a00: 706f 7373 6962 6c65 2066 6f72 2074 6865  possible for the
-00003a10: 0a20 2020 2020 2020 2073 616d 6520 6368  .        same ch
-00003a20: 6170 7465 722c 2072 6574 7572 6e73 2061  apter, returns a
-00003a30: 6e20 6964 656e 7469 6361 6c20 6042 6962  n identical `Bib
-00003a40: 6c65 5665 7273 6560 2065 7863 6570 7420  leVerse` except 
-00003a50: 7769 7468 2060 7665 7273 655f 6e75 6d60  with `verse_num`
-00003a60: 2073 6574 2074 6f20 302e 204f 7468 6572   set to 0. Other
-00003a70: 7769 7365 2c20 7265 7475 726e 7320 7468  wise, returns th
-00003a80: 650a 2020 2020 2020 2020 6f72 6967 696e  e.        origin
-00003a90: 616c 2060 4269 626c 6556 6572 7365 602e  al `BibleVerse`.
-00003aa0: 202a 2a4e 6f74 652a 2a3a 2054 6865 2076   **Note**: The v
-00003ab0: 616c 7565 206f 6620 7468 6520 676c 6f62  alue of the glob
-00003ac0: 616c 2061 7474 7269 6275 7465 2060 6269  al attribute `bi
-00003ad0: 626c 6572 6566 2e72 6566 2e66 6c61 6773  bleref.ref.flags
-00003ae0: 6020 6973 202a 6967 6e6f 7265 642a 2e27  ` is *ignored*.'
-00003af0: 2727 0a20 2020 2020 2020 2069 6620 7365  ''.        if se
-00003b00: 6c66 2e76 6572 7365 5f6e 756d 203d 3d20  lf.verse_num == 
-00003b10: 3120 616e 6420 7365 6c66 2e6d 696e 5f76  1 and self.min_v
-00003b20: 6572 7365 5f6e 756d 2873 656c 662e 6368  erse_num(self.ch
-00003b30: 6170 5f6e 756d 2c20 666c 6167 733d 4269  ap_num, flags=Bi
-00003b40: 626c 6546 6c61 672e 5645 5253 455f 3029  bleFlag.VERSE_0)
-00003b50: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00003b60: 2020 2072 6574 7572 6e20 4269 626c 6556     return BibleV
-00003b70: 6572 7365 2873 656c 662e 626f 6f6b 2c20  erse(self.book, 
-00003b80: 7365 6c66 2e63 6861 705f 6e75 6d2c 2030  self.chap_num, 0
-00003b90: 2c20 666c 6167 733d 4269 626c 6546 6c61  , flags=BibleFla
-00003ba0: 672e 5645 5253 455f 3029 0a20 2020 2020  g.VERSE_0).     
-00003bb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003bc0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00003bd0: 0a0a 2020 2020 6465 6620 6d69 6e5f 6368  ..    def min_ch
-00003be0: 6170 5f6e 756d 2873 656c 6629 202d 3e20  ap_num(self) -> 
-00003bf0: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
-00003c00: 5265 7475 726e 206c 6f77 6573 7420 6368  Return lowest ch
-00003c10: 6170 7465 7220 6e75 6d62 6572 2028 696e  apter number (in
-00003c20: 6465 7865 6420 6672 6f6d 2031 2920 6f66  dexed from 1) of
-00003c30: 2074 6865 2060 4269 626c 6542 6f6f 6b60   the `BibleBook`
-00003c40: 2063 6f6e 7461 696e 696e 6720 7468 6973   containing this
-00003c50: 2076 6572 7365 2e0a 2020 2020 2020 2020   verse..        
-00003c60: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
-00003c70: 726e 2073 656c 662e 626f 6f6b 2e6d 696e  rn self.book.min
-00003c80: 5f63 6861 705f 6e75 6d28 290a 0a20 2020  _chap_num()..   
-00003c90: 2064 6566 206d 6178 5f63 6861 705f 6e75   def max_chap_nu
-00003ca0: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
-00003cb0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-00003cc0: 6e20 6869 6768 6573 7420 6368 6170 7465  n highest chapte
-00003cd0: 7220 6e75 6d62 6572 2028 696e 6465 7865  r number (indexe
-00003ce0: 6420 6672 6f6d 2031 2920 6f66 2074 6865  d from 1) of the
-00003cf0: 2060 4269 626c 6542 6f6f 6b60 2063 6f6e   `BibleBook` con
-00003d00: 7461 696e 696e 6720 7468 6973 2076 6572  taining this ver
-00003d10: 7365 2e0a 2020 2020 2020 2020 2727 270a  se..        '''.
-00003d20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003d30: 656c 662e 626f 6f6b 2e6d 6178 5f63 6861  elf.book.max_cha
-00003d40: 705f 6e75 6d28 290a 2020 2020 0a20 2020  p_num().    .   
-00003d50: 2064 6566 206d 696e 5f76 6572 7365 5f6e   def min_verse_n
-00003d60: 756d 2873 656c 662c 2063 6861 705f 6e75  um(self, chap_nu
-00003d70: 6d3a 2069 6e74 203d 204e 6f6e 652c 2066  m: int = None, f
-00003d80: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
-00003d90: 3d20 4e6f 6e65 2920 2d3e 2069 6e74 3a0a  = None) -> int:.
-00003da0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-00003db0: 6e20 7468 6520 6c6f 7765 7374 2076 6572  n the lowest ver
-00003dc0: 7365 206e 756d 6265 7220 2830 206f 7220  se number (0 or 
-00003dd0: 3129 2066 6f72 2074 6865 2073 7065 6369  1) for the speci
-00003de0: 6669 6564 2063 6861 7074 6572 206f 6620  fied chapter of 
-00003df0: 7468 6520 6042 6962 6c65 426f 6f6b 6020  the `BibleBook` 
-00003e00: 636f 6e74 6169 6e69 6e67 0a20 2020 2020  containing.     
-00003e10: 2020 2074 6869 7320 7665 7273 652e 2049     this verse. I
-00003e20: 6620 6e6f 2063 6861 7074 6572 2069 7320  f no chapter is 
-00003e30: 7370 6563 6966 6965 642c 2069 7420 7265  specified, it re
-00003e40: 7475 726e 7320 7468 6520 6c6f 7765 7374  turns the lowest
-00003e50: 2076 6572 7365 206e 756d 6265 7220 6f66   verse number of
-00003e60: 2074 6865 2063 6861 7074 6572 2063 6f6e   the chapter con
-00003e70: 7461 696e 696e 670a 2020 2020 2020 2020  taining.        
-00003e80: 7468 6973 2060 4269 626c 6556 6572 7365  this `BibleVerse
-00003e90: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
-00003ea0: 2020 2020 2020 2069 6620 6368 6170 5f6e         if chap_n
-00003eb0: 756d 2069 7320 4e6f 6e65 3a0a 2020 2020  um is None:.    
-00003ec0: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
-00003ed0: 203d 2073 656c 662e 6368 6170 5f6e 756d   = self.chap_num
-00003ee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003ef0: 7365 6c66 2e62 6f6f 6b2e 6d69 6e5f 7665  self.book.min_ve
-00003f00: 7273 655f 6e75 6d28 6368 6170 5f6e 756d  rse_num(chap_num
-00003f10: 2c20 666c 6167 733d 666c 6167 7329 0a0a  , flags=flags)..
-00003f20: 2020 2020 6465 6620 6d61 785f 7665 7273      def max_vers
-00003f30: 655f 6e75 6d28 7365 6c66 2c20 6368 6170  e_num(self, chap
-00003f40: 5f6e 756d 3a20 696e 7429 202d 3e20 696e  _num: int) -> in
-00003f50: 743a 0a20 2020 2020 2020 2027 2727 5265  t:.        '''Re
-00003f60: 7475 726e 2074 6865 2068 6967 6865 7374  turn the highest
-00003f70: 2076 6572 7365 206e 756d 6265 7220 666f   verse number fo
-00003f80: 7220 7468 6520 7370 6563 6966 6965 6420  r the specified 
-00003f90: 6368 6170 7465 7220 6f66 2074 6865 2060  chapter of the `
-00003fa0: 4269 626c 6542 6f6f 6b60 2063 6f6e 7461  BibleBook` conta
-00003fb0: 696e 696e 6720 7468 6973 2076 6572 7365  ining this verse
-00003fc0: 2e0a 2020 2020 2020 2020 4966 206e 6f20  ..        If no 
-00003fd0: 6368 6170 7465 7220 6973 2073 7065 6369  chapter is speci
-00003fe0: 6669 6564 2c20 6974 2072 6574 7572 6e73  fied, it returns
-00003ff0: 2074 6865 2068 6967 6865 7374 2076 6572   the highest ver
-00004000: 7365 206e 756d 6265 7220 6f66 2074 6865  se number of the
-00004010: 2063 6861 7074 6572 2063 6f6e 7461 696e   chapter contain
-00004020: 696e 6720 7468 6973 2060 4269 626c 6556  ing this `BibleV
-00004030: 6572 7365 602e 0a20 2020 2020 2020 2027  erse`..        '
-00004040: 2727 0a20 2020 2020 2020 2069 6620 6368  ''.        if ch
-00004050: 6170 5f6e 756d 2069 7320 4e6f 6e65 3a0a  ap_num is None:.
-00004060: 2020 2020 2020 2020 2020 2020 6368 6170              chap
-00004070: 5f6e 756d 203d 2073 656c 662e 6368 6170  _num = self.chap
-00004080: 5f6e 756d 0a20 2020 2020 2020 2072 6574  _num.        ret
-00004090: 7572 6e20 7365 6c66 2e62 6f6f 6b2e 6d61  urn self.book.ma
-000040a0: 785f 7665 7273 655f 6e75 6d28 6368 6170  x_verse_num(chap
-000040b0: 5f6e 756d 290a 0a20 2020 2064 6566 2066  _num)..    def f
-000040c0: 6972 7374 5f76 6572 7365 2873 656c 662c  irst_verse(self,
-000040d0: 2063 6861 705f 6e75 6d3a 2069 6e74 203d   chap_num: int =
-000040e0: 204e 6f6e 652c 2066 6c61 6773 3a20 4269   None, flags: Bi
-000040f0: 626c 6546 6c61 6720 3d20 4e6f 6e65 2920  bleFlag = None) 
-00004100: 2d3e 2027 4269 626c 6556 6572 7365 273a  -> 'BibleVerse':
-00004110: 0a20 2020 2020 2020 2027 2727 5265 7475  .        '''Retu
-00004120: 726e 7320 7468 6520 6669 7273 7420 6042  rns the first `B
-00004130: 6962 6c65 5665 7273 6560 206f 6620 7468  ibleVerse` of th
-00004140: 6520 7370 6563 6966 6965 6420 6368 6170  e specified chap
-00004150: 7465 7220 6f66 2074 6865 2060 4269 626c  ter of the `Bibl
-00004160: 6542 6f6f 6b60 2063 6f6e 7461 696e 696e  eBook` containin
-00004170: 670a 2020 2020 2020 2020 7468 6973 2076  g.        this v
-00004180: 6572 7365 2e20 4966 2063 6861 7020 6973  erse. If chap is
-00004190: 2060 4e6f 6e65 602c 2069 7420 7265 7475   `None`, it retu
-000041a0: 726e 7320 7468 6520 6669 7273 7420 6042  rns the first `B
-000041b0: 6962 6c65 5665 7273 6560 206f 6620 7468  ibleVerse` of th
-000041c0: 6520 6368 6170 7465 7220 636f 6e74 6169  e chapter contai
-000041d0: 6e69 6e67 2074 6869 730a 2020 2020 2020  ning this.      
-000041e0: 2020 6042 6962 6c65 5665 7273 6560 2e0a    `BibleVerse`..
-000041f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00004200: 2020 2020 6966 2063 6861 705f 6e75 6d20      if chap_num 
-00004210: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00004220: 2020 2020 2063 6861 705f 6e75 6d20 3d20       chap_num = 
-00004230: 7365 6c66 2e63 6861 705f 6e75 6d0a 2020  self.chap_num.  
-00004240: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004250: 662e 626f 6f6b 2e66 6972 7374 5f76 6572  f.book.first_ver
-00004260: 7365 2863 6861 705f 6e75 6d2c 2066 6c61  se(chap_num, fla
-00004270: 6773 3d66 6c61 6773 290a 0a20 2020 2064  gs=flags)..    d
-00004280: 6566 206c 6173 745f 7665 7273 6528 7365  ef last_verse(se
-00004290: 6c66 2c20 6368 6170 5f6e 756d 3a20 696e  lf, chap_num: in
-000042a0: 7420 3d20 4e6f 6e65 2920 2d3e 2027 4269  t = None) -> 'Bi
-000042b0: 626c 6556 6572 7365 273a 0a20 2020 2020  bleVerse':.     
-000042c0: 2020 2027 2727 5265 7475 726e 7320 7468     '''Returns th
-000042d0: 6520 6c61 7374 2060 4269 626c 6556 6572  e last `BibleVer
-000042e0: 7365 6020 6f66 2074 6865 2073 7065 6369  se` of the speci
-000042f0: 6669 6564 2063 6861 7074 6572 206f 6620  fied chapter of 
-00004300: 7468 6520 6042 6962 6c65 426f 6f6b 6020  the `BibleBook` 
-00004310: 636f 6e74 6169 6e69 6e67 0a20 2020 2020  containing.     
-00004320: 2020 2074 6869 7320 7665 7273 652e 2049     this verse. I
-00004330: 6620 6368 6170 2069 7320 604e 6f6e 6560  f chap is `None`
-00004340: 2c20 6974 2072 6574 7572 6e73 2074 6865  , it returns the
-00004350: 206c 6173 7420 6042 6962 6c65 5665 7273   last `BibleVers
-00004360: 6560 206f 6620 7468 6520 6368 6170 7465  e` of the chapte
-00004370: 7220 636f 6e74 6169 6e69 6e67 2074 6869  r containing thi
-00004380: 730a 2020 2020 2020 2020 6042 6962 6c65  s.        `Bible
-00004390: 5665 7273 6560 2e0a 2020 2020 2020 2020  Verse`..        
-000043a0: 2727 270a 2020 2020 2020 2020 6966 2063  '''.        if c
-000043b0: 6861 705f 6e75 6d20 6973 204e 6f6e 653a  hap_num is None:
-000043c0: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-000043d0: 705f 6e75 6d20 3d20 7365 6c66 2e63 6861  p_num = self.cha
-000043e0: 705f 6e75 6d0a 2020 2020 2020 2020 7265  p_num.        re
-000043f0: 7475 726e 2073 656c 662e 626f 6f6b 2e6c  turn self.book.l
-00004400: 6173 745f 7665 7273 6528 6368 6170 5f6e  ast_verse(chap_n
-00004410: 756d 290a 0a20 2020 2064 6566 2069 735f  um)..    def is_
-00004420: 6669 7273 745f 696e 5f63 6861 7028 7365  first_in_chap(se
-00004430: 6c66 2c20 6368 6170 5f6e 756d 3a20 696e  lf, chap_num: in
-00004440: 7420 3d20 4e6f 6e65 2c20 666c 6167 733a  t = None, flags:
-00004450: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-00004460: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
-00004470: 2020 2020 2727 2752 6574 7572 6e73 2060      '''Returns `
-00004480: 5472 7565 6020 6966 2074 6869 7320 6042  True` if this `B
-00004490: 6962 6c65 5665 7273 6560 2069 7320 7468  ibleVerse` is th
-000044a0: 6520 6669 7273 7420 7665 7273 6520 696e  e first verse in
-000044b0: 2074 6865 2073 7065 6369 6669 6564 2063   the specified c
-000044c0: 6861 7074 6572 206f 6620 7468 6520 6042  hapter of the `B
-000044d0: 6962 6c65 426f 6f6b 600a 2020 2020 2020  ibleBook`.      
-000044e0: 2020 636f 6e74 6169 6e69 6e67 2074 6869    containing thi
-000044f0: 7320 7665 7273 652e 2049 6620 6063 6861  s verse. If `cha
-00004500: 705f 6e75 6d60 2069 7320 604e 6f6e 6560  p_num` is `None`
-00004510: 2c20 7468 6520 6368 6170 7465 7220 636f  , the chapter co
-00004520: 6e74 6169 6e69 6e67 2074 6869 7320 7665  ntaining this ve
-00004530: 7273 6520 6973 2075 7365 642e 0a20 2020  rse is used..   
-00004540: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00004550: 2072 6574 7572 6e20 7365 6c66 203d 3d20   return self == 
-00004560: 7365 6c66 2e66 6972 7374 5f76 6572 7365  self.first_verse
-00004570: 2863 6861 705f 6e75 6d2c 2066 6c61 6773  (chap_num, flags
-00004580: 3d66 6c61 6773 290a 0a20 2020 2064 6566  =flags)..    def
-00004590: 2069 735f 6c61 7374 5f69 6e5f 6368 6170   is_last_in_chap
-000045a0: 2873 656c 662c 2063 6861 705f 6e75 6d3a  (self, chap_num:
-000045b0: 2069 6e74 203d 204e 6f6e 6529 202d 3e20   int = None) -> 
-000045c0: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-000045d0: 2752 6574 7572 6e73 2060 5472 7565 6020  'Returns `True` 
-000045e0: 6966 2074 6869 7320 6042 6962 6c65 5665  if this `BibleVe
-000045f0: 7273 6560 2069 7320 7468 6520 6c61 7374  rse` is the last
-00004600: 2076 6572 7365 2069 6e20 7468 6520 7370   verse in the sp
-00004610: 6563 6966 6965 6420 6368 6170 7465 7220  ecified chapter 
-00004620: 6f66 2074 6865 2060 4269 626c 6542 6f6f  of the `BibleBoo
-00004630: 6b60 0a20 2020 2020 2020 2063 6f6e 7461  k`.        conta
-00004640: 696e 696e 6720 7468 6973 2076 6572 7365  ining this verse
-00004650: 2e20 4966 2060 6368 6170 5f6e 756d 6020  . If `chap_num` 
-00004660: 6973 2060 4e6f 6e65 602c 2074 6865 2063  is `None`, the c
-00004670: 6861 7074 6572 2063 6f6e 7461 696e 696e  hapter containin
-00004680: 6720 7468 6973 2076 6572 7365 2069 7320  g this verse is 
-00004690: 7573 6564 2e0a 2020 2020 2020 2020 2727  used..        ''
-000046a0: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-000046b0: 2073 656c 6620 3d3d 2073 656c 662e 6c61   self == self.la
-000046c0: 7374 5f76 6572 7365 2863 6861 705f 6e75  st_verse(chap_nu
-000046d0: 6d29 0a0a 2020 2020 6465 6620 6973 5f66  m)..    def is_f
-000046e0: 6972 7374 5f69 6e5f 626f 6f6b 2873 656c  irst_in_book(sel
-000046f0: 662c 2062 6f6f 6b3a 2042 6962 6c65 426f  f, book: BibleBo
-00004700: 6f6b 203d 204e 6f6e 652c 2066 6c61 6773  ok = None, flags
-00004710: 3a20 4269 626c 6546 6c61 6720 3d20 4e6f  : BibleFlag = No
-00004720: 6e65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ne) -> bool:.   
-00004730: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
-00004740: 6054 7275 6560 2069 6620 7468 6973 2060  `True` if this `
-00004750: 4269 626c 6556 6572 7365 6020 6973 2074  BibleVerse` is t
-00004760: 6865 2066 6972 7374 2076 6572 7365 2069  he first verse i
-00004770: 6e20 7468 6520 7370 6563 6966 6965 6420  n the specified 
-00004780: 6042 6962 6c65 426f 6f6b 602e 0a20 2020  `BibleBook`..   
-00004790: 2020 2020 2049 6620 6062 6f6f 6b60 2069       If `book` i
-000047a0: 7320 604e 6f6e 6560 2c20 7468 6520 6042  s `None`, the `B
-000047b0: 6962 6c65 426f 6f6b 6020 636f 6e74 6169  ibleBook` contai
-000047c0: 6e69 6e67 2074 6869 7320 7665 7273 6520  ning this verse 
-000047d0: 6973 2075 7365 642e 0a20 2020 2020 2020  is used..       
-000047e0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
-000047f0: 626f 6f6b 2069 7320 4e6f 6e65 3a0a 2020  book is None:.  
-00004800: 2020 2020 2020 2020 2020 626f 6f6b 203d            book =
-00004810: 2073 656c 662e 626f 6f6b 0a20 2020 2020   self.book.     
-00004820: 2020 2072 6574 7572 6e20 7365 6c66 203d     return self =
-00004830: 3d20 626f 6f6b 2e66 6972 7374 5f76 6572  = book.first_ver
-00004840: 7365 284e 6f6e 652c 2066 6c61 6773 3d66  se(None, flags=f
-00004850: 6c61 6773 290a 0a20 2020 2064 6566 2069  lags)..    def i
-00004860: 735f 6c61 7374 5f69 6e5f 626f 6f6b 2873  s_last_in_book(s
-00004870: 656c 662c 2062 6f6f 6b3a 2042 6962 6c65  elf, book: Bible
-00004880: 426f 6f6b 203d 204e 6f6e 6529 202d 3e20  Book = None) -> 
-00004890: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-000048a0: 2752 6574 7572 6e73 2060 5472 7565 6020  'Returns `True` 
-000048b0: 6966 2074 6869 7320 6042 6962 6c65 5665  if this `BibleVe
-000048c0: 7273 6560 2069 7320 7468 6520 6c61 7374  rse` is the last
-000048d0: 2076 6572 7365 2069 6e20 7468 6520 7370   verse in the sp
-000048e0: 6563 6966 6965 6420 6042 6962 6c65 426f  ecified `BibleBo
-000048f0: 6f6b 602e 0a20 2020 2020 2020 2049 6620  ok`..        If 
-00004900: 6062 6f6f 6b60 2069 7320 604e 6f6e 6560  `book` is `None`
-00004910: 2c20 7468 6520 6042 6962 6c65 426f 6f6b  , the `BibleBook
-00004920: 6020 636f 6e74 6169 6e69 6e67 2074 6869  ` containing thi
-00004930: 7320 7665 7273 6520 6973 2075 7365 642e  s verse is used.
-00004940: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00004950: 2020 2020 2069 6620 626f 6f6b 2069 7320       if book is 
-00004960: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00004970: 2020 626f 6f6b 203d 2073 656c 662e 626f    book = self.bo
-00004980: 6f6b 0a20 2020 2020 2020 2072 6574 7572  ok.        retur
-00004990: 6e20 7365 6c66 203d 3d20 626f 6f6b 2e6c  n self == book.l
-000049a0: 6173 745f 7665 7273 6528 4e6f 6e65 290a  ast_verse(None).
-000049b0: 0a20 2020 2064 6566 2063 6861 705f 7261  .    def chap_ra
-000049c0: 6e67 6528 7365 6c66 2c20 666c 6167 733a  nge(self, flags:
-000049d0: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-000049e0: 6529 202d 3e20 2742 6962 6c65 5261 6e67  e) -> 'BibleRang
-000049f0: 6527 3a0a 2020 2020 2020 2020 2727 2752  e':.        '''R
-00004a00: 6574 7572 6e73 2074 6865 2060 4269 626c  eturns the `Bibl
-00004a10: 6552 616e 6765 6020 7370 616e 6e69 6e67  eRange` spanning
-00004a20: 2074 6865 2077 686f 6c65 206f 6620 7468   the whole of th
-00004a30: 6520 6368 6170 7465 7220 636f 6e74 6169  e chapter contai
-00004a40: 6e69 6e67 2074 6869 7320 7665 7273 652e  ning this verse.
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00004a70: 2020 2020 2072 6574 7572 6e20 4269 626c       return Bibl
-00004a80: 6552 616e 6765 2873 7461 7274 3d73 656c  eRange(start=sel
-00004a90: 662e 6669 7273 745f 7665 7273 6528 666c  f.first_verse(fl
-00004aa0: 6167 733d 666c 6167 7329 2c20 656e 643d  ags=flags), end=
-00004ab0: 7365 6c66 2e6c 6173 745f 7665 7273 6528  self.last_verse(
-00004ac0: 292c 2066 6c61 6773 3d66 6c61 6773 290a  ), flags=flags).
-00004ad0: 0a20 2020 2064 6566 2062 6f6f 6b5f 7261  .    def book_ra
-00004ae0: 6e67 6528 7365 6c66 2c20 666c 6167 733a  nge(self, flags:
-00004af0: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-00004b00: 6529 202d 3e20 2742 6962 6c65 5261 6e67  e) -> 'BibleRang
-00004b10: 6527 3a0a 2020 2020 2020 2020 2727 2752  e':.        '''R
-00004b20: 6574 7572 6e73 2074 6865 2060 4269 626c  eturns the `Bibl
-00004b30: 6552 616e 6765 6020 7370 616e 6e69 6e67  eRange` spanning
-00004b40: 2074 6865 2077 686f 6c65 206f 6620 7468   the whole of th
-00004b50: 6520 626f 6f6b 2063 6f6e 7461 696e 696e  e book containin
-00004b60: 6720 7468 6973 2076 6572 7365 2e20 2020  g this verse.   
-00004b70: 2020 2020 200a 2020 2020 2020 2020 2727       .        ''
-00004b80: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-00004b90: 2073 656c 662e 626f 6f6b 2e72 616e 6765   self.book.range
-00004ba0: 2866 6c61 6773 3d66 6c61 6773 290a 0a20  (flags=flags).. 
-00004bb0: 2020 2064 6566 2061 6464 2873 656c 662c     def add(self,
-00004bc0: 206e 756d 5f76 6572 7365 733a 2069 6e74   num_verses: int
-00004bd0: 2c20 666c 6167 733a 2042 6962 6c65 466c  , flags: BibleFl
-00004be0: 6167 203d 204e 6f6e 6529 202d 3e20 2742  ag = None) -> 'B
-00004bf0: 6962 6c65 5665 7273 6527 3a0a 2020 2020  ibleVerse':.    
-00004c00: 2020 2020 2727 2752 6574 7572 6e73 2061      '''Returns a
-00004c10: 206e 6577 2060 4269 626c 6556 6572 7365   new `BibleVerse
-00004c20: 6020 7468 6174 2069 7320 606e 756d 5f76  ` that is `num_v
-00004c30: 6572 7365 7360 2061 6674 6572 2074 6869  erses` after thi
-00004c40: 7320 6042 6962 6c65 5665 7273 6560 2e0a  s `BibleVerse`..
-00004c50: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004c60: 2049 6620 6042 6962 6c65 466c 6167 2e4d   If `BibleFlag.M
-00004c70: 554c 5449 424f 4f4b 6020 6973 2073 6574  ULTIBOOK` is set
-00004c80: 2028 6569 7468 6572 2062 7920 7468 6520   (either by the 
-00004c90: 6066 6c61 6773 6020 6172 6775 6d65 6e74  `flags` argument
-00004ca0: 206f 722c 2069 6620 604e 6f6e 6560 2c20   or, if `None`, 
-00004cb0: 6279 2074 6865 2067 6c6f 6261 6c20 6174  by the global at
-00004cc0: 7472 6962 7574 6529 2c20 616e 640a 2020  tribute), and.  
-00004cd0: 2020 2020 2020 7468 6520 7265 7375 6c74        the result
-00004ce0: 2077 6f75 6c64 2062 6520 6265 796f 6e64   would be beyond
-00004cf0: 2074 6865 2063 7572 7265 6e74 2062 6f6f   the current boo
-00004d00: 6b2c 2061 2076 6572 7365 2069 6e20 7468  k, a verse in th
-00004d10: 6520 6e65 7874 2062 6f6f 6b20 6973 2072  e next book is r
-00004d20: 6574 7572 6e65 642e 204f 7468 6572 7769  eturned. Otherwi
-00004d30: 7365 2c20 6966 2074 6865 2076 6572 7365  se, if the verse
-00004d40: 0a20 2020 2020 2020 2064 6f65 7320 6e6f  .        does no
-00004d50: 7420 6578 6973 742c 2060 4e6f 6e65 6020  t exist, `None` 
-00004d60: 6973 2072 6574 7572 6e65 642e 2049 6620  is returned. If 
-00004d70: 7468 6520 6076 6572 7365 5f6e 756d 6020  the `verse_num` 
-00004d80: 6f66 2074 6869 7320 6042 6962 6c65 5665  of this `BibleVe
-00004d90: 7273 6560 2069 7320 616c 7265 6164 7920  rse` is already 
-00004da0: 302c 0a20 2020 2020 2020 2060 4269 626c  0,.        `Bibl
-00004db0: 6546 6c61 672e 5645 5253 455f 3060 2069  eFlag.VERSE_0` i
-00004dc0: 7320 666f 7263 6520 7365 7420 6f6e 2074  s force set on t
-00004dd0: 6865 2060 666c 6167 7360 2061 7267 756d  he `flags` argum
-00004de0: 656e 7420 666f 7220 7468 6973 2063 616c  ent for this cal
-00004df0: 6c2e 0a0a 2020 2020 2020 2020 5573 696e  l...        Usin
-00004e00: 6720 7468 6520 602b 6020 6f70 6572 6174  g the `+` operat
-00004e10: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
-00004e20: 2074 6f20 6361 6c6c 696e 6720 6061 6464   to calling `add
-00004e30: 2829 6020 7769 7468 2060 666c 6167 7320  ()` with `flags 
-00004e40: 3d20 4e6f 6e65 602e 0a20 2020 2020 2020  = None`..       
-00004e50: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
-00004e60: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
-00004e70: 756d 5f76 6572 7365 732c 2069 6e74 293a  um_verses, int):
-00004e80: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00004e90: 7365 2054 7970 6545 7272 6f72 2866 2243  se TypeError(f"C
-00004ea0: 616e 6e6f 7420 6164 6420 6120 7b74 7970  annot add a {typ
-00004eb0: 6528 6e75 6d5f 7665 7273 6573 297d 2074  e(num_verses)} t
-00004ec0: 6f20 6120 4269 626c 6556 6572 7365 2229  o a BibleVerse")
-00004ed0: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
-00004ee0: 2066 6c61 6773 206f 7220 6269 626c 6572   flags or bibler
-00004ef0: 6566 2e66 6c61 6773 206f 7220 4269 626c  ef.flags or Bibl
-00004f00: 6546 6c61 672e 4e4f 4e45 0a20 2020 2020  eFlag.NONE.     
-00004f10: 2020 2062 6f6f 6b20 3d20 7365 6c66 2e62     book = self.b
-00004f20: 6f6f 6b0a 2020 2020 2020 2020 6368 6170  ook.        chap
-00004f30: 5f6e 756d 203d 2073 656c 662e 6368 6170  _num = self.chap
-00004f40: 5f6e 756d 0a20 2020 2020 2020 2069 6620  _num.        if 
-00004f50: 7365 6c66 2e76 6572 7365 5f6e 756d 203d  self.verse_num =
-00004f60: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00004f70: 2066 6c61 6773 203d 2066 6c61 6773 207c   flags = flags |
-00004f80: 2042 6962 6c65 466c 6167 2e56 4552 5345   BibleFlag.VERSE
-00004f90: 5f30 2023 2048 6f6e 6f75 7220 6578 6973  _0 # Honour exis
-00004fa0: 7469 6e67 2076 6572 7365 2030 730a 2020  ting verse 0s.  
-00004fb0: 2020 2020 2020 7665 7273 655f 6e75 6d20        verse_num 
-00004fc0: 3d20 7365 6c66 2e76 6572 7365 5f6e 756d  = self.verse_num
-00004fd0: 202b 206e 756d 5f76 6572 7365 730a 2020   + num_verses.  
-00004fe0: 2020 2020 2020 6d61 785f 7665 7273 655f        max_verse_
-00004ff0: 6e75 6d20 3d20 626f 6f6b 2e6d 6178 5f76  num = book.max_v
-00005000: 6572 7365 5f6e 756d 2863 6861 705f 6e75  erse_num(chap_nu
-00005010: 6d29 0a20 2020 2020 2020 2077 6869 6c65  m).        while
-00005020: 2076 6572 7365 5f6e 756d 203e 206d 6178   verse_num > max
-00005030: 5f76 6572 7365 5f6e 756d 3a0a 2020 2020  _verse_num:.    
-00005040: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
-00005050: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00005060: 2020 6966 2063 6861 705f 6e75 6d20 3e20    if chap_num > 
-00005070: 626f 6f6b 2e6d 6178 5f63 6861 705f 6e75  book.max_chap_nu
-00005080: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
-00005090: 2020 2020 2069 6620 4269 626c 6546 6c61       if BibleFla
-000050a0: 672e 4d55 4c54 4942 4f4f 4b20 6e6f 7420  g.MULTIBOOK not 
-000050b0: 696e 2066 6c61 6773 3a0a 2020 2020 2020  in flags:.      
-000050c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000050d0: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-000050e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2020 626f 6f6b 203d 2062 6f6f 6b2e      book = book.
-00005110: 6e65 7874 2829 0a20 2020 2020 2020 2020  next().         
-00005120: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-00005130: 6f6b 2069 7320 4e6f 6e65 3a0a 2020 2020  ok is None:.    
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 6368 6170 5f6e 756d 203d 2062      chap_num = b
-00005180: 6f6f 6b2e 6d69 6e5f 6368 6170 5f6e 756d  ook.min_chap_num
-00005190: 2829 0a20 2020 2020 2020 2020 2020 200a  ().            .
-000051a0: 2020 2020 2020 2020 2020 2020 7665 7273              vers
-000051b0: 655f 6e75 6d20 3d20 7665 7273 655f 6e75  e_num = verse_nu
-000051c0: 6d20 2d20 6d61 785f 7665 7273 655f 6e75  m - max_verse_nu
-000051d0: 6d20 2b20 626f 6f6b 2e6d 696e 5f76 6572  m + book.min_ver
-000051e0: 7365 5f6e 756d 2863 6861 705f 6e75 6d2c  se_num(chap_num,
-000051f0: 2066 6c61 6773 2920 2d20 3120 0a20 2020   flags) - 1 .   
-00005200: 2020 2020 2020 2020 206d 6178 5f76 6572           max_ver
-00005210: 7365 5f6e 756d 203d 2062 6f6f 6b2e 6d61  se_num = book.ma
-00005220: 785f 7665 7273 655f 6e75 6d28 6368 6170  x_verse_num(chap
-00005230: 5f6e 756d 290a 0a20 2020 2020 2020 2072  _num)..        r
-00005240: 6574 7572 6e20 4269 626c 6556 6572 7365  eturn BibleVerse
-00005250: 2862 6f6f 6b2c 2063 6861 705f 6e75 6d2c  (book, chap_num,
-00005260: 2076 6572 7365 5f6e 756d 2c20 666c 6167   verse_num, flag
-00005270: 733d 666c 6167 7329 0a0a 2020 2020 6465  s=flags)..    de
-00005280: 6620 7375 6274 7261 6374 2873 656c 662c  f subtract(self,
-00005290: 206f 7468 6572 3a20 556e 696f 6e5b 696e   other: Union[in
-000052a0: 742c 2027 4269 626c 6556 6572 7365 275d  t, 'BibleVerse']
-000052b0: 2c20 666c 6167 733a 2042 6962 6c65 466c  , flags: BibleFl
-000052c0: 6167 203d 204e 6f6e 6529 202d 3e20 556e  ag = None) -> Un
-000052d0: 696f 6e5b 696e 742c 2027 4269 626c 6556  ion[int, 'BibleV
-000052e0: 6572 7365 275d 3a0a 2020 2020 2020 2020  erse']:.        
-000052f0: 2727 270a 2020 2020 2020 2020 2d20 4966  '''.        - If
-00005300: 2060 6f74 6865 7260 2069 7320 616e 2060   `other` is an `
-00005310: 696e 7460 2c20 7265 7475 726e 7320 6120  int`, returns a 
-00005320: 6e65 7720 6042 6962 6c65 5665 7273 6560  new `BibleVerse`
-00005330: 2074 6861 7420 6973 2060 6f74 6865 7260   that is `other`
-00005340: 2076 6572 7365 7320 6265 666f 7265 2074   verses before t
-00005350: 6869 7320 6042 6962 6c65 5665 7273 6560  his `BibleVerse`
-00005360: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00005370: 2020 2020 2049 6620 6042 6962 6c65 466c       If `BibleFl
-00005380: 6167 2e4d 554c 5449 424f 4f4b 6020 6973  ag.MULTIBOOK` is
-00005390: 2073 6574 2028 6569 7468 6572 2073 6574   set (either set
-000053a0: 2062 7920 7468 6520 6066 6c61 6773 6020   by the `flags` 
-000053b0: 6172 6775 6d65 6e74 206f 722c 2069 6620  argument or, if 
-000053c0: 604e 6f6e 6560 2c20 7468 6520 676c 6f62  `None`, the glob
-000053d0: 616c 2061 7474 7269 6275 7465 292c 0a20  al attribute),. 
-000053e0: 2020 2020 2020 2020 2061 6e64 2074 6865           and the
-000053f0: 2072 6573 756c 7420 776f 756c 6420 6265   result would be
-00005400: 2062 6566 6f72 6520 7468 6520 6375 7272   before the curr
-00005410: 656e 7420 626f 6f6b 2c20 6120 7665 7273  ent book, a vers
-00005420: 6520 696e 2074 6865 2070 7265 7669 6f75  e in the previou
-00005430: 7320 626f 6f6b 2069 7320 7265 7475 726e  s book is return
-00005440: 6564 2e20 4f74 6865 7277 6973 652c 2069  ed. Otherwise, i
-00005450: 660a 2020 2020 2020 2020 2020 7468 6520  f.          the 
-00005460: 7665 7273 6520 646f 6573 206e 6f74 2065  verse does not e
-00005470: 7869 7374 2c20 4e6f 6e65 2069 7320 7265  xist, None is re
-00005480: 7475 726e 6564 2e20 4966 2074 6865 2060  turned. If the `
-00005490: 7665 7273 655f 6e75 6d60 206f 6620 7468  verse_num` of th
-000054a0: 6973 2060 4269 626c 6556 6572 7365 6020  is `BibleVerse` 
-000054b0: 6973 2061 6c72 6561 6479 2030 2c0a 2020  is already 0,.  
-000054c0: 2020 2020 2020 2020 6042 6962 6c65 466c          `BibleFl
-000054d0: 6167 2e56 4552 5345 5f30 6020 6973 2066  ag.VERSE_0` is f
-000054e0: 6f72 6365 2073 6574 206f 6e20 7468 6520  orce set on the 
-000054f0: 6066 6c61 6773 6020 6172 6775 6d65 6e74  `flags` argument
-00005500: 2066 6f72 2074 6869 7320 6361 6c6c 2e0a   for this call..
-00005510: 0a20 2020 2020 2020 202d 2049 6620 606f  .        - If `o
-00005520: 7468 6572 6020 6973 2061 6e6f 7468 6572  ther` is another
-00005530: 2060 4269 626c 6556 6572 7365 602c 2072   `BibleVerse`, r
-00005540: 6574 7572 6e73 2074 6865 2069 6e74 6567  eturns the integ
-00005550: 6572 206e 756d 6265 7220 6f66 2076 6572  er number of ver
-00005560: 7365 7320 6265 7477 6565 6e20 7468 6973  ses between this
-00005570: 2042 6962 6c65 5665 7273 6520 616e 6420   BibleVerse and 
-00005580: 606f 7468 6572 602e 0a20 2020 2020 2020  `other`..       
-00005590: 2020 2054 6865 206e 756d 6265 7220 6973     The number is
-000055a0: 2070 6f73 6974 6976 6520 6966 2074 6869   positive if thi
-000055b0: 7320 7665 7273 6520 3e20 606f 7468 6572  s verse > `other
-000055c0: 602c 206f 7220 6e65 6761 7469 7665 2069  `, or negative i
-000055d0: 6620 7468 6973 2076 6572 7365 203c 2060  f this verse < `
-000055e0: 6f74 6865 7260 2e0a 0a20 2020 2020 2020  other`...       
-000055f0: 2055 7369 6e67 2074 6865 2060 2d60 206f   Using the `-` o
-00005600: 7065 7261 746f 7220 6973 2065 7175 6976  perator is equiv
-00005610: 616c 656e 7420 746f 2063 616c 6c69 6e67  alent to calling
-00005620: 2060 7375 6274 7261 6374 2829 6020 7769   `subtract()` wi
-00005630: 7468 2060 666c 6167 7320 3d20 4e6f 6e65  th `flags = None
-00005640: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
-00005650: 2020 2020 2020 2066 6c61 6773 203d 2066         flags = f
-00005660: 6c61 6773 206f 7220 6269 626c 6572 6566  lags or bibleref
-00005670: 2e66 6c61 6773 206f 7220 4269 626c 6546  .flags or BibleF
-00005680: 6c61 672e 4e4f 4e45 0a20 2020 2020 2020  lag.NONE.       
-00005690: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
-000056a0: 7468 6572 2c20 696e 7429 3a0a 2020 2020  ther, int):.    
-000056b0: 2020 2020 2020 2020 626f 6f6b 203d 2073          book = s
-000056c0: 656c 662e 626f 6f6b 0a20 2020 2020 2020  elf.book.       
-000056d0: 2020 2020 2063 6861 705f 6e75 6d20 3d20       chap_num = 
-000056e0: 7365 6c66 2e63 6861 705f 6e75 6d0a 2020  self.chap_num.  
-000056f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005700: 662e 7665 7273 655f 6e75 6d20 3d3d 2030  f.verse_num == 0
-00005710: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005720: 2020 666c 6167 7320 3d20 666c 6167 7320    flags = flags 
-00005730: 7c20 4269 626c 6546 6c61 672e 5645 5253  | BibleFlag.VERS
-00005740: 455f 3020 2320 486f 6e6f 7572 2065 7869  E_0 # Honour exi
-00005750: 7374 696e 6720 7665 7273 6520 3073 0a20  sting verse 0s. 
-00005760: 2020 2020 2020 2020 2020 2076 6572 7365             verse
-00005770: 5f6e 756d 203d 2073 656c 662e 7665 7273  _num = self.vers
-00005780: 655f 6e75 6d20 2d20 6f74 6865 720a 2020  e_num - other.  
-00005790: 2020 2020 2020 2020 2020 6d69 6e5f 7665            min_ve
-000057a0: 7273 655f 6e75 6d20 3d20 626f 6f6b 2e6d  rse_num = book.m
-000057b0: 696e 5f76 6572 7365 5f6e 756d 2863 6861  in_verse_num(cha
-000057c0: 705f 6e75 6d2c 2066 6c61 6773 290a 2020  p_num, flags).  
-000057d0: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-000057e0: 7665 7273 655f 6e75 6d20 3c20 6d69 6e5f  verse_num < min_
-000057f0: 7665 7273 655f 6e75 6d3a 0a20 2020 2020  verse_num:.     
-00005800: 2020 2020 2020 2020 2020 2063 6861 705f             chap_
-00005810: 6e75 6d20 2d3d 2031 0a20 2020 2020 2020  num -= 1.       
-00005820: 2020 2020 2020 2020 2069 6620 6368 6170           if chap
-00005830: 5f6e 756d 203c 2062 6f6f 6b2e 6d69 6e5f  _num < book.min_
-00005840: 6368 6170 5f6e 756d 2829 3a0a 2020 2020  chap_num():.    
-00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005860: 6966 2042 6962 6c65 466c 6167 2e4d 554c  if BibleFlag.MUL
-00005870: 5449 424f 4f4b 206e 6f74 2069 6e20 666c  TIBOOK not in fl
-00005880: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
-00005890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000058a0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-000058b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000058c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000058d0: 2020 2020 2020 2020 2020 2062 6f6f 6b20             book 
-000058e0: 3d20 626f 6f6b 2e70 7265 7628 290a 2020  = book.prev().  
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2020 2020 6966 2062 6f6f 6b20 6973        if book is
-00005910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005930: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+000000b0: 730a 2320 544f 444f 3a20 496d 706c 656d  s.# TODO: Implem
+000000c0: 656e 7420 636f 756e 7420 6f66 2063 6861  ent count of cha
+000000d0: 7074 6572 7320 616e 6420 7665 7273 6573  pters and verses
+000000e0: 2069 6e20 6120 4269 626c 6552 616e 6765   in a BibleRange
+000000f0: 2061 6e64 2042 6962 6c65 5261 6e67 654c   and BibleRangeL
+00000100: 6973 740a 0a66 726f 6d20 6461 7461 636c  ist..from datacl
+00000110: 6173 7365 7320 696d 706f 7274 2064 6174  asses import dat
+00000120: 6163 6c61 7373 0a66 726f 6d20 656e 756d  aclass.from enum
+00000130: 2069 6d70 6f72 7420 456e 756d 2c20 466c   import Enum, Fl
+00000140: 6167 2c20 6175 746f 0a66 726f 6d20 7479  ag, auto.from ty
+00000150: 7069 6e67 2069 6d70 6f72 7420 556e 696f  ping import Unio
+00000160: 6e0a 0a66 726f 6d20 6269 626c 6572 6566  n..from bibleref
+00000170: 2069 6d70 6f72 7420 4269 626c 6552 6566   import BibleRef
+00000180: 4578 6365 7074 696f 6e2c 2062 6962 6c65  Exception, bible
+00000190: 5f64 6174 612c 2066 6c61 6773 0a0a 230a  _data, flags..#.
+000001a0: 2320 5365 742d 7374 796c 6520 6f70 6572  # Set-style oper
+000001b0: 6174 696f 6e73 2069 6e20 7468 6973 206d  ations in this m
+000001c0: 6f64 756c 6520 6172 6520 6465 7269 7665  odule are derive
+000001d0: 6420 6672 6f6d 2074 6865 2070 7974 686f  d from the pytho
+000001e0: 6e2d 7261 6e67 6573 206d 6f64 756c 650a  n-ranges module.
+000001f0: 2320 6174 2068 7474 7073 3a2f 2f67 6974  # at https://git
+00000200: 6875 622e 636f 6d2f 5375 7065 7262 6972  hub.com/Superbir
+00000210: 6431 312f 7261 6e67 6573 2c20 756e 6465  d11/ranges, unde
+00000220: 7220 7468 6520 4d49 5420 4c69 6365 6e63  r the MIT Licenc
+00000230: 650a 230a 0a63 6c61 7373 2042 6962 6c65  e.#..class Bible
+00000240: 466c 6167 2846 6c61 6729 3a0a 2020 2020  Flag(Flag):.    
+00000250: 2727 2746 6c61 6773 2075 7365 6420 666f  '''Flags used fo
+00000260: 7220 636f 6e74 726f 6c6c 696e 6720 7661  r controlling va
+00000270: 7269 6f75 7320 6265 6861 7669 6f75 7273  rious behaviours
+00000280: 2074 6872 6f75 6768 6f75 7420 7468 6520   throughout the 
+00000290: 7061 636b 6167 652e 2054 6865 7365 2063  package. These c
+000002a0: 616e 2062 6520 7365 7420 676c 6f62 616c  an be set global
+000002b0: 6c79 2066 6f72 2074 6865 2070 6163 6b61  ly for the packa
+000002c0: 6765 0a20 2020 2075 7369 6e67 2074 6865  ge.    using the
+000002d0: 2060 6269 626c 6572 6566 2e72 6566 2e66   `bibleref.ref.f
+000002e0: 6c61 6773 6020 6174 7472 6962 7574 652c  lags` attribute,
+000002f0: 206f 7220 7065 722d 6d65 7468 6f64 2066   or per-method f
+00000300: 6f72 206d 6574 686f 6473 2074 6861 7420  or methods that 
+00000310: 696e 636c 7564 6573 2061 2060 666c 6167  includes a `flag
+00000320: 7360 206b 6579 776f 7264 2061 7267 756d  s` keyword argum
+00000330: 656e 742e 0a20 2020 2027 2727 0a20 2020  ent..    '''.   
+00000340: 204e 4f4e 4520 3d20 300a 2020 2020 2727   NONE = 0.    ''
+00000350: 274e 6f20 6042 6962 6c65 466c 6167 6020  'No `BibleFlag` 
+00000360: 666c 6167 7320 6172 6520 7365 742e 2044  flags are set. D
+00000370: 6566 6175 6c74 2076 616c 7565 2066 6f72  efault value for
+00000380: 2060 6269 626c 6572 6566 2e66 6c61 6773   `bibleref.flags
+00000390: 602e 2727 270a 0a20 2020 204d 554c 5449  `.'''..    MULTI
+000003a0: 424f 4f4b 203d 2061 7574 6f28 290a 2020  BOOK = auto().  
+000003b0: 2020 2727 2757 6865 6e20 7365 742c 2061    '''When set, a
+000003c0: 2060 4269 626c 6552 616e 6765 6020 6361   `BibleRange` ca
+000003d0: 6e20 6265 2063 6f6e 7374 7275 6374 6564  n be constructed
+000003e0: 2074 6861 7420 7370 616e 7320 6d75 6c74   that spans mult
+000003f0: 6970 6c65 2042 6962 6c65 2062 6f6f 6b73  iple Bible books
+00000400: 2e20 4578 6973 7469 6e67 206d 756c 7469  . Existing multi
+00000410: 626f 6f6b 0a20 2020 2072 616e 6765 7320  book.    ranges 
+00000420: 6265 6861 7665 2063 6f72 7265 6374 6c79  behave correctly
+00000430: 2065 7665 6e20 7768 656e 2060 4d55 4c54   even when `MULT
+00000440: 4942 4f4f 4b60 2069 7320 756e 7365 742e  IBOOK` is unset.
+00000450: 2727 270a 0a20 2020 2056 4552 5345 5f30  '''..    VERSE_0
+00000460: 203d 2061 7574 6f28 290a 2020 2020 2727   = auto().    ''
+00000470: 2757 6865 6e20 7365 742c 2061 2060 4269  'When set, a `Bi
+00000480: 626c 6556 6572 7365 6020 6361 6e20 6265  bleVerse` can be
+00000490: 2063 6f6e 7374 7275 6374 6564 2077 6865   constructed whe
+000004a0: 7265 2074 6865 2066 6972 7374 2076 6572  re the first ver
+000004b0: 7365 206e 756d 6265 7220 6f66 2073 6f6d  se number of som
+000004c0: 6520 6368 6170 7465 7273 0a20 2020 2069  e chapters.    i
+000004d0: 7320 302c 206e 6f74 2031 2e20 2854 6869  s 0, not 1. (Thi
+000004e0: 7320 6973 2063 7572 7265 6e74 6c79 2074  s is currently t
+000004f0: 7275 6520 6f6e 6c79 2066 6f72 2074 6865  rue only for the
+00000500: 2050 7361 6c6d 7320 7468 6174 2068 6176   Psalms that hav
+00000510: 6520 7375 7065 7273 6372 6970 7469 6f6e  e superscription
+00000520: 732e 2920 5768 656e 2079 6f75 206e 6565  s.) When you nee
+00000530: 6420 746f 206d 6978 0a20 2020 2072 6566  d to mix.    ref
+00000540: 6572 656e 6365 7320 7468 6174 2064 6f20  erences that do 
+00000550: 6f72 2064 6f6e 2774 2061 6c6c 6f77 2066  or don't allow f
+00000560: 6f72 2076 6572 7365 2030 2c20 6974 206d  or verse 0, it m
+00000570: 6179 2062 6520 6561 7369 6572 2074 6f20  ay be easier to 
+00000580: 7365 7420 6f72 2063 6c65 6172 2060 5645  set or clear `VE
+00000590: 5253 455f 3060 2066 6f72 2061 6c6c 2079  RSE_0` for all y
+000005a0: 6f75 7220 636f 6465 2c20 616e 640a 2020  our code, and.  
+000005b0: 2020 7468 656e 2075 7365 2074 6865 2060    then use the `
+000005c0: 7665 7273 655f 305f 746f 5f31 2829 6020  verse_0_to_1()` 
+000005d0: 616e 6420 6076 6572 7365 5f31 5f74 6f5f  and `verse_1_to_
+000005e0: 3028 2960 206d 6574 686f 6473 206f 6e20  0()` methods on 
+000005f0: 6042 6962 6c65 5665 7273 6560 2c20 6042  `BibleVerse`, `B
+00000600: 6962 6c65 5261 6e67 6560 2061 6e64 2060  ibleRange` and `
+00000610: 4269 626c 6552 616e 6765 4c69 7374 600a  BibleRangeList`.
+00000620: 2020 2020 6173 206e 6563 6573 7361 7279      as necessary
+00000630: 2e27 2727 0a0a 2020 2020 414c 4c20 3d20  .'''..    ALL = 
+00000640: 4d55 4c54 4942 4f4f 4b20 7c20 5645 5253  MULTIBOOK | VERS
+00000650: 455f 300a 2020 2020 2727 2741 6c6c 2060  E_0.    '''All `
+00000660: 4269 626c 6546 6c61 6760 2066 6c61 6773  BibleFlag` flags
+00000670: 2061 7265 2073 6574 2e27 2727 0a0a 666c   are set.'''..fl
+00000680: 6167 7320 3d20 4269 626c 6546 6c61 672e  ags = BibleFlag.
+00000690: 4e4f 4e45 2023 2044 6566 6175 6c74 2073  NONE # Default s
+000006a0: 6574 7469 6e67 2066 6f72 2067 6c6f 6261  etting for globa
+000006b0: 6c20 666c 6167 7320 6174 7472 6962 7574  l flags attribut
+000006c0: 652e 0a0a 0a63 6c61 7373 2042 6962 6c65  e....class Bible
+000006d0: 426f 6f6b 2845 6e75 6d29 3a0a 2020 2020  Book(Enum):.    
+000006e0: 2727 2741 6e20 656e 756d 206f 6620 626f  '''An enum of bo
+000006f0: 6f6b 7320 696e 2074 6865 2042 6962 6c65  oks in the Bible
+00000700: 2e0a 0a20 2020 2041 2060 4269 626c 6542  ...    A `BibleB
+00000710: 6f6f 6b60 2068 6173 2074 6865 2066 6f6c  ook` has the fol
+00000720: 6c6f 7769 6e67 2065 7874 7261 2061 7474  lowing extra att
+00000730: 7269 6275 7465 7320 2861 6464 6564 2064  ributes (added d
+00000740: 7572 696e 6720 7061 636b 6167 6520 696d  uring package im
+00000750: 706f 7274 293a 0a20 2020 2020 202d 2060  port):.      - `
+00000760: 6162 6272 6576 603a 2020 2054 6865 2061  abbrev`:   The a
+00000770: 6262 7265 7669 6174 6564 206e 616d 6520  bbreviated name 
+00000780: 6f66 2074 6865 2062 6f6f 6b0a 2020 2020  of the book.    
+00000790: 2020 2d20 6074 6974 6c65 603a 2020 2020    - `title`:    
+000007a0: 5468 6520 6675 6c6c 2074 6974 6c65 206f  The full title o
+000007b0: 6620 7468 6520 626f 6f6b 2e0a 2020 2020  f the book..    
+000007c0: 2020 2d20 6072 6567 6578 603a 2020 2020    - `regex`:    
+000007d0: 4120 7265 6765 7820 7768 6963 6820 6d61  A regex which ma
+000007e0: 7463 6865 7320 616e 7920 6163 6365 7074  tches any accept
+000007f0: 6162 6c65 206e 616d 652f 6162 6272 6576  able name/abbrev
+00000800: 2066 6f72 2074 6865 2062 6f6f 6b2e 0a20   for the book.. 
+00000810: 2020 2020 202d 2060 6f72 6465 7260 3a20       - `order`: 
+00000820: 2020 2041 6e20 696e 7465 6765 7220 696e     An integer in
+00000830: 6469 6361 7469 6e67 2069 7473 206f 7264  dicating its ord
+00000840: 6572 696e 6720 696e 2074 6865 2063 6f6c  ering in the col
+00000850: 6c65 6374 696f 6e20 6f66 2062 6f6f 6b73  lection of books
+00000860: 2028 302d 6261 7365 6429 2e0a 2020 2020   (0-based)..    
+00000870: 0a20 2020 2054 776f 2060 4269 626c 6542  .    Two `BibleB
+00000880: 6f6f 6b60 7320 6361 6e20 6265 2063 6f6d  ook`s can be com
+00000890: 7061 7265 6420 7573 696e 6720 7468 6520  pared using the 
+000008a0: 7374 616e 6461 7264 2063 6f6d 7061 7269  standard compari
+000008b0: 736f 6e20 6f70 6572 6174 6f72 732c 2077  son operators, w
+000008c0: 6869 6368 2063 6f6d 7061 7265 2074 6865  hich compare the
+000008d0: 0a20 2020 2062 6f6f 6b73 2720 706f 7369  .    books' posi
+000008e0: 7469 6f6e 2069 6e20 7468 6520 626f 6f6b  tion in the book
+000008f0: 206f 7264 6572 696e 672e 0a20 2020 2027   ordering..    '
+00000900: 2727 0a20 2020 2023 2045 7874 7261 2070  ''.    # Extra p
+00000910: 7269 7661 7465 2061 7474 7269 6275 7465  rivate attribute
+00000920: 733a 0a20 2020 2023 205f 6d61 785f 7665  s:.    # _max_ve
+00000930: 7273 6573 3a20 204c 6973 7420 6f66 206d  rses:  List of m
+00000940: 6178 2076 6572 7365 206e 756d 6265 7220  ax verse number 
+00000950: 666f 7220 6561 6368 2063 6861 7074 6572  for each chapter
+00000960: 2028 6173 6365 6e64 696e 6720 6279 2063   (ascending by c
+00000970: 6861 7074 6572 292e 0a20 2020 2023 2020  hapter)..    #  
+00000980: 2020 2020 2020 2020 2020 2020 2020 204c                 L
+00000990: 656e 206f 6620 6c69 7374 2069 7320 6e75  en of list is nu
+000009a0: 6d62 6572 206f 6620 6368 6170 7465 7273  mber of chapters
+000009b0: 2e20 4e6f 6e65 2069 6620 6e6f 206d 6178  . None if no max
+000009c0: 5f76 6572 7365 2064 6174 6120 7375 7070  _verse data supp
+000009d0: 6c69 6564 2e0a 2020 2020 2320 5f76 6572  lied..    # _ver
+000009e0: 7365 5f30 733a 2020 2020 5365 7420 6f66  se_0s:    Set of
+000009f0: 2063 6861 7074 6572 206e 756d 6265 7273   chapter numbers
+00000a00: 2028 312d 696e 6465 7865 6429 2074 6861   (1-indexed) tha
+00000a10: 7420 6361 6e20 6265 6769 6e20 7769 7468  t can begin with
+00000a20: 2061 2076 6572 7365 2030 2e20 456d 7074   a verse 0. Empt
+00000a30: 7920 7365 740a 2020 2020 2320 2020 2020  y set.    #     
+00000a40: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00000a50: 6f20 6368 6170 7465 7273 2063 616e 2062  o chapters can b
+00000a60: 6567 696e 2077 6974 6820 6120 7665 7273  egin with a vers
+00000a70: 6520 302e 0a20 2020 2023 0a20 2020 2047  e 0..    #.    G
+00000a80: 656e 2020 2020 203d 2022 4765 6e22 200a  en     = "Gen" .
+00000a90: 2020 2020 4578 6f64 2020 2020 3d20 2245      Exod    = "E
+00000aa0: 786f 6422 0a20 2020 204c 6576 2020 2020  xod".    Lev    
+00000ab0: 203d 2022 4c65 7622 0a20 2020 204e 756d   = "Lev".    Num
+00000ac0: 2020 2020 203d 2022 4e75 6d22 0a20 2020       = "Num".   
+00000ad0: 2044 6575 7420 2020 203d 2022 4465 7574   Deut    = "Deut
+00000ae0: 220a 2020 2020 4a6f 7368 2020 2020 3d20  ".    Josh    = 
+00000af0: 224a 6f73 6822 0a20 2020 204a 7564 6720  "Josh".    Judg 
+00000b00: 2020 203d 2022 4a75 6467 220a 2020 2020     = "Judg".    
+00000b10: 5275 7468 2020 2020 3d20 2252 7574 6822  Ruth    = "Ruth"
+00000b20: 0a20 2020 2049 5361 6d20 2020 203d 2022  .    ISam    = "
+00000b30: 3153 616d 220a 2020 2020 4949 5361 6d20  1Sam".    IISam 
+00000b40: 2020 3d20 2232 5361 6d22 0a20 2020 2049    = "2Sam".    I
+00000b50: 4b67 7320 2020 203d 2022 314b 6773 220a  Kgs    = "1Kgs".
+00000b60: 2020 2020 4949 4b67 7320 2020 3d20 2232      IIKgs   = "2
+00000b70: 4b67 7322 0a20 2020 2049 4368 7220 2020  Kgs".    IChr   
+00000b80: 203d 2022 3143 6872 220a 2020 2020 4949   = "1Chr".    II
+00000b90: 4368 7220 2020 3d20 2232 4368 7222 0a20  Chr   = "2Chr". 
+00000ba0: 2020 2045 7a72 6120 2020 203d 2022 457a     Ezra    = "Ez
+00000bb0: 7261 220a 2020 2020 4e65 6820 2020 2020  ra".    Neh     
+00000bc0: 3d20 224e 6568 220a 2020 2020 4573 7468  = "Neh".    Esth
+00000bd0: 2020 2020 3d20 2245 7374 6822 0a20 2020      = "Esth".   
+00000be0: 204a 6f62 2020 2020 203d 2022 4a6f 6222   Job     = "Job"
+00000bf0: 0a20 2020 2050 7361 2020 2020 203d 2022  .    Psa     = "
+00000c00: 5073 6122 0a20 2020 2050 726f 7620 2020  Psa".    Prov   
+00000c10: 203d 2022 5072 6f76 220a 2020 2020 4563   = "Prov".    Ec
+00000c20: 636c 2020 2020 3d20 2245 6363 6c22 0a20  cl    = "Eccl". 
+00000c30: 2020 2053 6f6e 6720 2020 203d 2022 536f     Song    = "So
+00000c40: 6e67 220a 2020 2020 4973 6120 2020 2020  ng".    Isa     
+00000c50: 3d20 2249 7361 220a 2020 2020 4a65 7220  = "Isa".    Jer 
+00000c60: 2020 2020 3d20 224a 6572 220a 2020 2020      = "Jer".    
+00000c70: 4c61 6d20 2020 2020 3d20 224c 616d 220a  Lam     = "Lam".
+00000c80: 2020 2020 457a 656b 2020 2020 3d20 2245      Ezek    = "E
+00000c90: 7a65 6b22 0a20 2020 2044 616e 2020 2020  zek".    Dan    
+00000ca0: 203d 2022 4461 6e22 0a20 2020 2048 6f73   = "Dan".    Hos
+00000cb0: 2020 2020 203d 2022 486f 7322 0a20 2020       = "Hos".   
+00000cc0: 204a 6f65 6c20 2020 203d 2022 4a6f 656c   Joel    = "Joel
+00000cd0: 220a 2020 2020 416d 6f73 2020 2020 3d20  ".    Amos    = 
+00000ce0: 2241 6d6f 7322 0a20 2020 204f 6261 6420  "Amos".    Obad 
+00000cf0: 2020 203d 2022 4f62 6164 220a 2020 2020     = "Obad".    
+00000d00: 4a6f 6e61 6820 2020 3d20 224a 6f6e 6168  Jonah   = "Jonah
+00000d10: 220a 2020 2020 4d69 6320 2020 2020 3d20  ".    Mic     = 
+00000d20: 224d 6963 220a 2020 2020 4e61 6820 2020  "Mic".    Nah   
+00000d30: 2020 3d20 224e 6168 220a 2020 2020 4861    = "Nah".    Ha
+00000d40: 6220 2020 2020 3d20 2248 6162 220a 2020  b     = "Hab".  
+00000d50: 2020 5a65 7068 2020 2020 3d20 225a 6570    Zeph    = "Zep
+00000d60: 6822 0a20 2020 2048 6167 2020 2020 203d  h".    Hag     =
+00000d70: 2022 4861 6722 0a20 2020 205a 6563 6820   "Hag".    Zech 
+00000d80: 2020 203d 2022 5a65 6368 220a 2020 2020     = "Zech".    
+00000d90: 4d61 6c20 2020 2020 3d20 224d 616c 220a  Mal     = "Mal".
+00000da0: 2020 2020 4d61 7474 2020 2020 3d20 224d      Matt    = "M
+00000db0: 6174 7422 0a20 2020 204d 6172 6b20 2020  att".    Mark   
+00000dc0: 203d 2022 4d61 726b 220a 2020 2020 4c75   = "Mark".    Lu
+00000dd0: 6b65 2020 2020 3d20 224c 756b 6522 0a20  ke    = "Luke". 
+00000de0: 2020 204a 6f68 6e20 2020 203d 2022 4a6f     John    = "Jo
+00000df0: 686e 220a 2020 2020 4163 7473 2020 2020  hn".    Acts    
+00000e00: 3d20 2241 6374 7322 0a20 2020 2052 6f6d  = "Acts".    Rom
+00000e10: 2020 2020 203d 2022 526f 6d22 0a20 2020       = "Rom".   
+00000e20: 2049 436f 7220 2020 203d 2022 3143 6f72   ICor    = "1Cor
+00000e30: 220a 2020 2020 4949 436f 7220 2020 3d20  ".    IICor   = 
+00000e40: 2232 436f 7222 0a20 2020 2047 616c 2020  "2Cor".    Gal  
+00000e50: 2020 203d 2022 4761 6c22 0a20 2020 2045     = "Gal".    E
+00000e60: 7068 2020 2020 203d 2022 4570 6822 0a20  ph     = "Eph". 
+00000e70: 2020 2050 6869 6c20 2020 203d 2022 5068     Phil    = "Ph
+00000e80: 696c 220a 2020 2020 436f 6c20 2020 2020  il".    Col     
+00000e90: 3d20 2243 6f6c 220a 2020 2020 4954 6820  = "Col".    ITh 
+00000ea0: 2020 2020 3d20 2231 5468 220a 2020 2020      = "1Th".    
+00000eb0: 4949 5468 2020 2020 3d20 2232 5468 220a  IITh    = "2Th".
+00000ec0: 2020 2020 4954 696d 2020 2020 3d20 2231      ITim    = "1
+00000ed0: 5469 6d22 0a20 2020 2049 4954 696d 2020  Tim".    IITim  
+00000ee0: 203d 2022 3254 696d 220a 2020 2020 5469   = "2Tim".    Ti
+00000ef0: 7475 7320 2020 3d20 2254 6974 7573 220a  tus   = "Titus".
+00000f00: 2020 2020 5068 6c6d 2020 2020 3d20 2250      Phlm    = "P
+00000f10: 686c 6d22 0a20 2020 2048 6562 2020 2020  hlm".    Heb    
+00000f20: 203d 2022 4865 6222 0a20 2020 204a 616d   = "Heb".    Jam
+00000f30: 2020 2020 203d 2022 4a61 6d22 0a20 2020       = "Jam".   
+00000f40: 2049 5065 7420 2020 203d 2022 3150 6574   IPet    = "1Pet
+00000f50: 220a 2020 2020 4949 5065 7420 2020 3d20  ".    IIPet   = 
+00000f60: 2232 5065 7422 0a20 2020 2049 4a6e 2020  "2Pet".    IJn  
+00000f70: 2020 203d 2022 314a 6e22 0a20 2020 2049     = "1Jn".    I
+00000f80: 494a 6e20 2020 203d 2022 324a 6e22 0a20  IJn    = "2Jn". 
+00000f90: 2020 2049 4949 4a6e 2020 203d 2022 334a     IIIJn   = "3J
+00000fa0: 6e22 0a20 2020 204a 7564 6520 2020 203d  n".    Jude    =
+00000fb0: 2022 4a75 6465 220a 2020 2020 5265 7620   "Jude".    Rev 
+00000fc0: 2020 2020 3d20 2252 6576 220a 0a20 2020      = "Rev"..   
+00000fd0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00000fe0: 2020 6465 6620 6672 6f6d 5f73 7472 2863    def from_str(c
+00000ff0: 6c73 2c20 7374 7269 6e67 3a20 7374 722c  ls, string: str,
+00001000: 2072 6169 7365 5f65 7272 6f72 3a20 626f   raise_error: bo
+00001010: 6f6c 203d 2046 616c 7365 2920 2d3e 2027  ol = False) -> '
+00001020: 4269 626c 6542 6f6f 6b27 3a0a 2020 2020  BibleBook':.    
+00001030: 2020 2020 2727 2752 6574 7572 6e20 7468      '''Return th
+00001040: 6520 4269 626c 6542 6f6f 6b20 6d61 7463  e BibleBook matc
+00001050: 6869 6e67 2074 6865 2067 6976 656e 2073  hing the given s
+00001060: 7472 696e 6720 6e61 6d65 2e0a 2020 2020  tring name..    
+00001070: 2020 2020 5768 6974 6573 7061 6365 2069      Whitespace i
+00001080: 6e20 6073 7472 696e 6760 2069 7320 7374  n `string` is st
+00001090: 7269 7070 6564 2062 6566 6f72 6520 6d61  ripped before ma
+000010a0: 7463 6869 6e67 2e0a 2020 2020 2020 2020  tching..        
+000010b0: 0a20 2020 2020 2020 2049 6620 6e6f 2062  .        If no b
+000010c0: 6f6f 6b20 6d61 7463 6865 7320 616e 6420  ook matches and 
+000010d0: 7261 6973 655f 6572 726f 7220 6973 2046  raise_error is F
+000010e0: 616c 7365 2028 7468 6520 6465 6661 756c  alse (the defaul
+000010f0: 7429 2c20 4e6f 6e65 2069 7320 7265 7475  t), None is retu
+00001100: 726e 6564 2e0a 2020 2020 2020 2020 4966  rned..        If
+00001110: 206e 6f20 626f 6f6b 206d 6174 6368 6573   no book matches
+00001120: 2061 6e64 2072 6169 7365 5f65 7272 6f72   and raise_error
+00001130: 2069 7320 5472 7565 2c20 616e 2060 496e   is True, an `In
+00001140: 7661 6c69 6452 6566 6572 656e 6365 4572  validReferenceEr
+00001150: 726f 7260 2069 7320 7261 6973 6564 2e0a  ror` is raised..
+00001160: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001170: 2020 2020 7374 7269 6e67 203d 2073 7472      string = str
+00001180: 696e 672e 7374 7269 7028 290a 2020 2020  ing.strip().    
+00001190: 2020 2020 6d61 7463 6820 3d20 4661 6c73      match = Fals
+000011a0: 650a 2020 2020 2020 2020 666f 7220 626f  e.        for bo
+000011b0: 6f6b 2069 6e20 4269 626c 6542 6f6f 6b3a  ok in BibleBook:
+000011c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000011d0: 626f 6f6b 2e72 6567 6578 2069 7320 6e6f  book.regex is no
+000011e0: 7420 4e6f 6e65 2061 6e64 2062 6f6f 6b2e  t None and book.
+000011f0: 7265 6765 782e 6675 6c6c 6d61 7463 6828  regex.fullmatch(
+00001200: 7374 7269 6e67 2920 6973 206e 6f74 204e  string) is not N
+00001210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001220: 2020 2020 206d 6174 6368 203d 2054 7275       match = Tru
+00001230: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001240: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00001250: 6966 206d 6174 6368 3a0a 2020 2020 2020  if match:.      
+00001260: 2020 2020 2020 7265 7475 726e 2062 6f6f        return boo
+00001270: 6b0a 2020 2020 2020 2020 656c 7365 3a0a  k.        else:.
+00001280: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00001290: 6169 7365 5f65 7272 6f72 3a0a 2020 2020  aise_error:.    
+000012a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000012b0: 6520 496e 7661 6c69 6452 6566 6572 656e  e InvalidReferen
+000012c0: 6365 4572 726f 7228 6622 4e6f 2062 6f6f  ceError(f"No boo
+000012d0: 6b20 666f 756e 6420 666f 7220 7374 7269  k found for stri
+000012e0: 6e67 2027 7b73 7472 696e 677d 2722 290a  ng '{string}'").
+000012f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001310: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+00001320: 2020 2064 6566 206d 696e 5f63 6861 705f     def min_chap_
+00001330: 6e75 6d28 7365 6c66 2920 2d3e 2069 6e74  num(self) -> int
+00001340: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+00001350: 7572 6e20 6c6f 7765 7374 2063 6861 7074  urn lowest chapt
+00001360: 6572 206e 756d 6265 7220 2863 7572 7265  er number (curre
+00001370: 6e74 6c79 2061 6c77 6179 7320 3129 2066  ntly always 1) f
+00001380: 6f72 2074 6869 7320 6042 6962 6c65 426f  or this `BibleBo
+00001390: 6f6b 602e 0a20 2020 2020 2020 2027 2727  ok`..        '''
+000013a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000013b0: 2e5f 6d61 785f 7665 7273 6573 2069 7320  ._max_verses is 
+000013c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000013d0: 2020 7265 7475 726e 2030 0a20 2020 2020    return 0.     
+000013e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000013f0: 2020 2020 2072 6574 7572 6e20 3120 2020       return 1   
+00001400: 2023 2043 7572 7265 6e74 6c79 2061 6c77   # Currently alw
+00001410: 6179 7320 312e 2050 6572 6861 7073 2069  ays 1. Perhaps i
+00001420: 6e20 6675 7475 7265 2073 6f6d 6520 626f  n future some bo
+00001430: 6f6b 7320 6d61 7920 6861 7665 2061 2063  oks may have a c
+00001440: 6861 7074 6572 2d30 2070 726f 6c6f 6775  hapter-0 prologu
+00001450: 6520 696e 636c 7564 6564 3f0a 0a20 2020  e included?..   
+00001460: 2064 6566 206d 6178 5f63 6861 705f 6e75   def max_chap_nu
+00001470: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
+00001480: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
+00001490: 6e20 6869 6768 6573 7420 6368 6170 7465  n highest chapte
+000014a0: 7220 6e75 6d62 6572 2066 6f72 2074 6869  r number for thi
+000014b0: 7320 6042 6962 6c65 426f 6f6b 602e 0a20  s `BibleBook`.. 
+000014c0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000014d0: 2020 2069 6620 7365 6c66 2e5f 6d61 785f     if self._max_
+000014e0: 7665 7273 6573 2069 7320 4e6f 6e65 3a0a  verses is None:.
+000014f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001500: 726e 2030 0a20 2020 2020 2020 2065 6c73  rn 0.        els
+00001510: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00001520: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
+00001530: 6d61 785f 7665 7273 6573 290a 2020 2020  max_verses).    
+00001540: 0a20 2020 2064 6566 2063 6861 705f 636f  .    def chap_co
+00001550: 756e 7428 7365 6c66 293a 0a20 2020 2020  unt(self):.     
+00001560: 2020 2027 2727 5265 7475 726e 7320 7468     '''Returns th
+00001570: 6520 6e75 6d62 6572 206f 6620 6368 6170  e number of chap
+00001580: 7465 7273 2069 6e20 7468 6973 2060 4269  ters in this `Bi
+00001590: 626c 6542 6f6f 6b60 2e0a 2020 2020 2020  bleBook`..      
+000015a0: 2020 2727 270a 2020 2020 2020 2020 7265    '''.        re
+000015b0: 7475 726e 2028 7365 6c66 2e6d 6178 5f63  turn (self.max_c
+000015c0: 6861 705f 6e75 6d28 2920 2d20 7365 6c66  hap_num() - self
+000015d0: 2e6d 696e 5f63 6861 705f 6e75 6d28 2920  .min_chap_num() 
+000015e0: 2b20 3129 0a0a 2020 2020 6465 6620 6d69  + 1)..    def mi
+000015f0: 6e5f 7665 7273 655f 6e75 6d28 7365 6c66  n_verse_num(self
+00001600: 2c20 6368 6170 5f6e 756d 3a20 696e 742c  , chap_num: int,
+00001610: 2066 6c61 6773 3a20 4269 626c 6546 6c61   flags: BibleFla
+00001620: 6720 3d20 4e6f 6e65 2920 2d3e 2069 6e74  g = None) -> int
+00001630: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+00001640: 7572 6e20 7468 6520 6c6f 7765 7374 2076  urn the lowest v
+00001650: 6572 7365 206e 756d 6265 7220 2830 206f  erse number (0 o
+00001660: 7220 3129 2066 6f72 2074 6865 2073 7065  r 1) for the spe
+00001670: 6369 6669 6564 2063 6861 7074 6572 206e  cified chapter n
+00001680: 756d 6265 7220 6f66 2074 6869 7320 6042  umber of this `B
+00001690: 6962 6c65 426f 6f6b 602e 0a20 2020 2020  ibleBook`..     
+000016a0: 2020 2027 2727 0a20 2020 2020 2020 2066     '''.        f
+000016b0: 6c61 6773 203d 2066 6c61 6773 206f 7220  lags = flags or 
+000016c0: 676c 6f62 616c 7328 295b 2766 6c61 6773  globals()['flags
+000016d0: 275d 206f 7220 4269 626c 6546 6c61 672e  '] or BibleFlag.
+000016e0: 4e4f 4e45 0a20 2020 2020 2020 2069 6620  NONE.        if 
+000016f0: 6368 6170 5f6e 756d 203c 2073 656c 662e  chap_num < self.
+00001700: 6d69 6e5f 6368 6170 5f6e 756d 2829 206f  min_chap_num() o
+00001710: 7220 6368 6170 5f6e 756d 203e 2073 656c  r chap_num > sel
+00001720: 662e 6d61 785f 6368 6170 5f6e 756d 2829  f.max_chap_num()
+00001730: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00001740: 6973 6520 496e 7661 6c69 6452 6566 6572  ise InvalidRefer
+00001750: 656e 6365 4572 726f 7228 6622 4e6f 2063  enceError(f"No c
+00001760: 6861 7074 6572 207b 6368 6170 5f6e 756d  hapter {chap_num
+00001770: 7d20 696e 207b 7365 6c66 2e74 6974 6c65  } in {self.title
+00001780: 7d22 290a 2020 2020 2020 2020 7265 7475  }").        retu
+00001790: 726e 2030 2069 6620 2842 6962 6c65 466c  rn 0 if (BibleFl
+000017a0: 6167 2e56 4552 5345 5f30 2069 6e20 666c  ag.VERSE_0 in fl
+000017b0: 6167 7320 616e 6420 6368 6170 5f6e 756d  ags and chap_num
+000017c0: 2069 6e20 7365 6c66 2e5f 7665 7273 655f   in self._verse_
+000017d0: 3073 2920 656c 7365 2031 0a0a 2020 2020  0s) else 1..    
+000017e0: 6465 6620 6d61 785f 7665 7273 655f 6e75  def max_verse_nu
+000017f0: 6d28 7365 6c66 2c20 6368 6170 5f6e 756d  m(self, chap_num
+00001800: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+00001810: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
+00001820: 2074 6865 2068 6967 6865 7374 2076 6572   the highest ver
+00001830: 7365 206e 756d 6265 7220 666f 7220 7468  se number for th
+00001840: 6520 7370 6563 6966 6965 6420 6368 6170  e specified chap
+00001850: 7465 7220 6e75 6d62 6572 206f 6620 7468  ter number of th
+00001860: 6973 2060 4269 626c 6542 6f6f 6b60 2e0a  is `BibleBook`..
+00001870: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001880: 2020 2020 6966 2063 6861 705f 6e75 6d20      if chap_num 
+00001890: 3c20 7365 6c66 2e6d 696e 5f63 6861 705f  < self.min_chap_
+000018a0: 6e75 6d28 2920 6f72 2063 6861 705f 6e75  num() or chap_nu
+000018b0: 6d20 3e20 7365 6c66 2e6d 6178 5f63 6861  m > self.max_cha
+000018c0: 705f 6e75 6d28 293a 0a20 2020 2020 2020  p_num():.       
+000018d0: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
+000018e0: 6964 5265 6665 7265 6e63 6545 7272 6f72  idReferenceError
+000018f0: 2866 224e 6f20 6368 6170 7465 7220 7b63  (f"No chapter {c
+00001900: 6861 705f 6e75 6d7d 2069 6e20 7b73 656c  hap_num} in {sel
+00001910: 662e 7469 746c 657d 2229 0a20 2020 2020  f.title}").     
+00001920: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00001930: 6d61 785f 7665 7273 6573 5b63 6861 705f  max_verses[chap_
+00001940: 6e75 6d2d 315d 0a0a 2020 2020 6465 6620  num-1]..    def 
+00001950: 6669 7273 745f 7665 7273 6528 7365 6c66  first_verse(self
+00001960: 2c20 6368 6170 5f6e 756d 3a20 696e 7420  , chap_num: int 
+00001970: 3d20 4e6f 6e65 2c20 666c 6167 733a 2042  = None, flags: B
+00001980: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
+00001990: 202d 3e20 2742 6962 6c65 5665 7273 6527   -> 'BibleVerse'
+000019a0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+000019b0: 7572 6e73 2061 2060 4269 626c 6556 6572  urns a `BibleVer
+000019c0: 7365 6020 666f 7220 7468 6520 6669 7273  se` for the firs
+000019d0: 7420 7665 7273 6520 6f66 2074 6865 2073  t verse of the s
+000019e0: 7065 6369 6669 6564 2063 6861 7074 6572  pecified chapter
+000019f0: 206f 6620 7468 6973 2060 4269 626c 6542   of this `BibleB
+00001a00: 6f6f 6b60 2e0a 2020 2020 2020 2020 4966  ook`..        If
+00001a10: 2063 6861 7020 6973 2060 4e6f 6e65 602c   chap is `None`,
+00001a20: 2069 7420 7265 7475 726e 7320 7468 6520   it returns the 
+00001a30: 6669 7273 7420 7665 7273 6520 6f66 2074  first verse of t
+00001a40: 6865 2065 6e74 6972 6520 626f 6f6b 2e0a  he entire book..
+00001a50: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001a60: 2020 2020 6966 2063 6861 705f 6e75 6d20      if chap_num 
+00001a70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00001a80: 2020 2020 2063 6861 705f 6e75 6d20 3d20       chap_num = 
+00001a90: 7365 6c66 2e6d 696e 5f63 6861 705f 6e75  self.min_chap_nu
+00001aa0: 6d28 290a 2020 2020 2020 2020 7265 7475  m().        retu
+00001ab0: 726e 2042 6962 6c65 5665 7273 6528 7365  rn BibleVerse(se
+00001ac0: 6c66 2c20 6368 6170 5f6e 756d 2c20 7365  lf, chap_num, se
+00001ad0: 6c66 2e6d 696e 5f76 6572 7365 5f6e 756d  lf.min_verse_num
+00001ae0: 2863 6861 705f 6e75 6d2c 2066 6c61 6773  (chap_num, flags
+00001af0: 2929 2020 2020 2020 2020 0a0a 2020 2020  ))        ..    
+00001b00: 6465 6620 6c61 7374 5f76 6572 7365 2873  def last_verse(s
+00001b10: 656c 662c 2063 6861 705f 6e75 6d3a 2069  elf, chap_num: i
+00001b20: 6e74 203d 204e 6f6e 6529 202d 3e20 2742  nt = None) -> 'B
+00001b30: 6962 6c65 5665 7273 6527 3a0a 2020 2020  ibleVerse':.    
+00001b40: 2020 2020 2727 2752 6574 7572 6e73 2061      '''Returns a
+00001b50: 2060 4269 626c 6556 6572 7365 6020 666f   `BibleVerse` fo
+00001b60: 7220 7468 6520 6c61 7374 2076 6572 7365  r the last verse
+00001b70: 206f 6620 7468 6520 7370 6563 6966 6965   of the specifie
+00001b80: 6420 6368 6170 7465 7220 6f66 2074 6869  d chapter of thi
+00001b90: 7320 6042 6962 6c65 426f 6f6b 602e 0a20  s `BibleBook`.. 
+00001ba0: 2020 2020 2020 2049 6620 6368 6170 2069         If chap i
+00001bb0: 7320 604e 6f6e 6560 2c20 6974 2072 6574  s `None`, it ret
+00001bc0: 7572 6e73 2074 6865 206c 6173 7420 7665  urns the last ve
+00001bd0: 7273 6520 6f66 2074 6865 2065 6e74 6972  rse of the entir
+00001be0: 6520 626f 6f6b 2e0a 2020 2020 2020 2020  e book..        
+00001bf0: 2727 270a 2020 2020 2020 2020 6966 2063  '''.        if c
+00001c00: 6861 705f 6e75 6d20 6973 204e 6f6e 653a  hap_num is None:
+00001c10: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00001c20: 705f 6e75 6d20 3d20 7365 6c66 2e6d 6178  p_num = self.max
+00001c30: 5f63 6861 705f 6e75 6d28 290a 2020 2020  _chap_num().    
+00001c40: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+00001c50: 5665 7273 6528 7365 6c66 2c20 6368 6170  Verse(self, chap
+00001c60: 5f6e 756d 2c20 7365 6c66 2e6d 6178 5f76  _num, self.max_v
+00001c70: 6572 7365 5f6e 756d 2863 6861 705f 6e75  erse_num(chap_nu
+00001c80: 6d29 2920 2020 2020 2020 200a 0a20 2020  m))        ..   
+00001c90: 2064 6566 206e 6578 7428 7365 6c66 2920   def next(self) 
+00001ca0: 2d3e 2027 4269 626c 6542 6f6f 6b27 3a0a  -> 'BibleBook':.
+00001cb0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
+00001cc0: 6e73 2074 6865 206e 6578 7420 6042 6962  ns the next `Bib
+00001cd0: 6c65 426f 6f6b 6020 696e 2074 6865 2062  leBook` in the b
+00001ce0: 6f6f 6b20 6f72 6465 7269 6e67 2c20 6f72  ook ordering, or
+00001cf0: 2060 4e6f 6e65 6020 6966 2074 6869 7320   `None` if this 
+00001d00: 6973 2074 6865 2066 696e 616c 2062 6f6f  is the final boo
+00001d10: 6b2c 0a20 2020 2020 2020 206f 7220 6973  k,.        or is
+00001d20: 206e 6f74 2070 6172 7420 6f66 2074 6865   not part of the
+00001d30: 206f 7264 6572 696e 672e 0a20 2020 2020   ordering..     
+00001d40: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+00001d50: 6620 7365 6c66 2e6f 7264 6572 2069 7320  f self.order is 
+00001d60: 4e6f 6e65 206f 7220 7365 6c66 2e6f 7264  None or self.ord
+00001d70: 6572 203d 3d20 6c65 6e28 6269 626c 655f  er == len(bible_
+00001d80: 6461 7461 2829 2e62 6f6f 6b5f 6f72 6465  data().book_orde
+00001d90: 7229 2d31 3a0a 2020 2020 2020 2020 2020  r)-1:.          
+00001da0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00001db0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001dc0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00001dd0: 6962 6c65 5f64 6174 6128 292e 626f 6f6b  ible_data().book
+00001de0: 5f6f 7264 6572 5b73 656c 662e 6f72 6465  _order[self.orde
+00001df0: 722b 315d 0a0a 2020 2020 6465 6620 7072  r+1]..    def pr
+00001e00: 6576 2873 656c 6629 202d 3e20 2742 6962  ev(self) -> 'Bib
+00001e10: 6c65 426f 6f6b 273a 0a20 2020 2020 2020  leBook':.       
+00001e20: 2027 2727 5265 7475 726e 7320 7468 6520   '''Returns the 
+00001e30: 7072 6576 696f 7573 2060 4269 626c 6542  previous `BibleB
+00001e40: 6f6f 6b60 2069 6e20 7468 6520 626f 6f6b  ook` in the book
+00001e50: 206f 7264 6572 696e 672c 206f 7220 604e   ordering, or `N
+00001e60: 6f6e 6560 2069 6620 7468 6973 2069 7320  one` if this is 
+00001e70: 7468 6520 6669 7273 7420 626f 6f6b 2c0a  the first book,.
+00001e80: 2020 2020 2020 2020 6f72 2069 7320 6e6f          or is no
+00001e90: 7420 7061 7274 206f 6620 7468 6520 6f72  t part of the or
+00001ea0: 6465 7269 6e67 2e0a 2020 2020 2020 2020  dering..        
+00001eb0: 2727 270a 2020 2020 2020 2020 6966 2073  '''.        if s
+00001ec0: 656c 662e 6f72 6465 7220 6973 204e 6f6e  elf.order is Non
+00001ed0: 6520 6f72 2073 656c 662e 6f72 6465 7220  e or self.order 
+00001ee0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00001ef0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00001f00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001f10: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00001f20: 6962 6c65 5f64 6174 6128 292e 626f 6f6b  ible_data().book
+00001f30: 5f6f 7264 6572 5b73 656c 662e 6f72 6465  _order[self.orde
+00001f40: 722d 315d 0a0a 2020 2020 6465 6620 5f5f  r-1]..    def __
+00001f50: 6c74 5f5f 2873 656c 662c 206f 7468 6572  lt__(self, other
+00001f60: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
+00001f70: 7420 6973 696e 7374 616e 6365 286f 7468  t isinstance(oth
+00001f80: 6572 2c20 4269 626c 6542 6f6f 6b29 3a0a  er, BibleBook):.
+00001f90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001fa0: 726e 204e 6f74 496d 706c 656d 656e 7465  rn NotImplemente
+00001fb0: 640a 2020 2020 2020 2020 656c 7365 3a0a  d.        else:.
+00001fc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001fd0: 726e 2073 656c 662e 6f72 6465 7220 3c20  rn self.order < 
+00001fe0: 6f74 6865 722e 6f72 6465 720a 0a20 2020  other.order..   
+00001ff0: 2064 6566 205f 5f6c 655f 5f28 7365 6c66   def __le__(self
+00002000: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00002010: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00002020: 6e63 6528 6f74 6865 722c 2042 6962 6c65  nce(other, Bible
+00002030: 426f 6f6b 293a 0a20 2020 2020 2020 2020  Book):.         
+00002040: 2020 2072 6574 7572 6e20 4e6f 7449 6d70     return NotImp
+00002050: 6c65 6d65 6e74 6564 0a20 2020 2020 2020  lemented.       
+00002060: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00002070: 2020 2072 6574 7572 6e20 7365 6c66 2e6f     return self.o
+00002080: 7264 6572 203c 3d20 6f74 6865 722e 6f72  rder <= other.or
+00002090: 6465 720a 0a20 2020 2064 6566 205f 5f67  der..    def __g
+000020a0: 745f 5f28 7365 6c66 2c20 6f74 6865 7229  t__(self, other)
+000020b0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+000020c0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+000020d0: 722c 2042 6962 6c65 426f 6f6b 293a 0a20  r, BibleBook):. 
+000020e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000020f0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00002100: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00002110: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002120: 6e20 7365 6c66 2e6f 7264 6572 203e 206f  n self.order > o
+00002130: 7468 6572 2e6f 7264 6572 0a0a 2020 2020  ther.order..    
+00002140: 6465 6620 5f5f 6765 5f5f 2873 656c 662c  def __ge__(self,
+00002150: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00002160: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00002170: 6365 286f 7468 6572 2c20 4269 626c 6542  ce(other, BibleB
+00002180: 6f6f 6b29 3a0a 2020 2020 2020 2020 2020  ook):.          
+00002190: 2020 7265 7475 726e 204e 6f74 496d 706c    return NotImpl
+000021a0: 656d 656e 7465 640a 2020 2020 2020 2020  emented.        
+000021b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000021c0: 2020 7265 7475 726e 2073 656c 662e 6f72    return self.or
+000021d0: 6465 7220 3e3d 206f 7468 6572 2e6f 7264  der >= other.ord
+000021e0: 6572 0a0a 0a23 2057 6520 6465 6c61 7920  er...# We delay 
+000021f0: 7468 6573 6520 696d 706f 7274 7320 756e  these imports un
+00002200: 7469 6c20 7468 6973 2070 6f69 6e74 2073  til this point s
+00002210: 6f20 7468 6174 2042 6962 6c65 426f 6f6b  o that BibleBook
+00002220: 2061 6e64 2069 7473 2072 656c 6174 6564   and its related
+00002230: 2063 6c61 7373 6573 0a23 2061 7265 2061   classes.# are a
+00002240: 6c72 6561 6479 2064 6566 696e 6564 2061  lready defined a
+00002250: 6e64 2063 616e 2062 6520 7573 6564 2062  nd can be used b
+00002260: 7920 6f74 6865 7220 7369 626c 696e 6720  y other sibling 
+00002270: 6d6f 6475 6c65 730a 6672 6f6d 202e 2069  modules.from . i
+00002280: 6d70 6f72 7420 7061 7273 6572 0a66 726f  mport parser.fro
+00002290: 6d20 2e20 696d 706f 7274 2075 7469 6c0a  m . import util.
+000022a0: 6672 6f6d 202e 2069 6d70 6f72 7420 6461  from . import da
+000022b0: 7461 0a0a 0a63 6c61 7373 2042 6962 6c65  ta...class Bible
+000022c0: 5665 7273 6550 6172 7428 466c 6167 293a  VersePart(Flag):
+000022d0: 0a20 2020 2027 2727 466c 6167 7320 666f  .    '''Flags fo
+000022e0: 7220 7265 6665 7272 696e 6720 746f 2074  r referring to t
+000022f0: 6865 2033 2070 7269 6d61 7279 2061 7474  he 3 primary att
+00002300: 7269 6275 7465 7320 6f66 2061 2042 6962  ributes of a Bib
+00002310: 6c65 5665 7273 652e 0a20 2020 200a 2020  leVerse..    .  
+00002320: 2020 4d61 696e 6c79 2075 7365 6420 696e    Mainly used in
+00002330: 7465 726e 616c 6c79 2066 6f72 2063 6f6e  ternally for con
+00002340: 7665 7274 696e 6720 4269 626c 6520 7265  verting Bible re
+00002350: 6665 7265 6e63 6573 2073 7472 696e 6773  ferences strings
+00002360: 2c20 746f 2069 6e64 6963 6174 6520 7768  , to indicate wh
+00002370: 6963 6820 6174 7472 6962 7574 6573 2077  ich attributes w
+00002380: 696c 6c20 6469 7370 6c61 7920 696e 0a20  ill display in. 
+00002390: 2020 2061 2073 7472 696e 6720 7265 7072     a string repr
+000023a0: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
+000023b0: 2727 270a 2020 2020 4e4f 4e45 2020 2020  '''.    NONE    
+000023c0: 3d20 300a 2020 2020 424f 4f4b 2020 2020  = 0.    BOOK    
+000023d0: 3d20 6175 746f 2829 2020 200a 2020 2020  = auto()   .    
+000023e0: 4348 4150 2020 2020 3d20 6175 746f 2829  CHAP    = auto()
+000023f0: 0a20 2020 2056 4552 5345 2020 203d 2061  .    VERSE   = a
+00002400: 7574 6f28 290a 2020 2020 4655 4c4c 5f52  uto().    FULL_R
+00002410: 4546 2020 2020 3d20 424f 4f4b 207c 2043  EF    = BOOK | C
+00002420: 4841 5020 7c20 5645 5253 450a 2020 2020  HAP | VERSE.    
+00002430: 424f 4f4b 5f43 4841 5020 2020 3d20 424f  BOOK_CHAP   = BO
+00002440: 4f4b 207c 2043 4841 500a 2020 2020 424f  OK | CHAP.    BO
+00002450: 4f4b 5f56 4552 5345 2020 3d20 424f 4f4b  OK_VERSE  = BOOK
+00002460: 207c 2056 4552 5345 0a20 2020 2043 4841   | VERSE.    CHA
+00002470: 505f 5645 5253 4520 203d 2043 4841 5020  P_VERSE  = CHAP 
+00002480: 7c20 5645 5253 450a 0a0a 4064 6174 6163  | VERSE...@datac
+00002490: 6c61 7373 2869 6e69 743d 4661 6c73 652c  lass(init=False,
+000024a0: 2072 6570 723d 4661 6c73 652c 2065 713d   repr=False, eq=
+000024b0: 5472 7565 2c20 6f72 6465 723d 5472 7565  True, order=True
+000024c0: 2c20 6672 6f7a 656e 3d54 7275 6529 0a63  , frozen=True).c
+000024d0: 6c61 7373 2042 6962 6c65 5665 7273 653a  lass BibleVerse:
+000024e0: 0a20 2020 2027 2727 4120 7265 6665 7265  .    '''A refere
+000024f0: 6e63 6520 746f 2061 2073 696e 676c 6520  nce to a single 
+00002500: 4269 626c 6520 7665 7273 6520 2865 2e67  Bible verse (e.g
+00002510: 2e20 4d61 7474 2032 3a33 292e 0a0a 2020  . Matt 2:3)...  
+00002520: 2020 436f 6e74 6169 6e73 2033 2070 7269    Contains 3 pri
+00002530: 6d61 7279 2061 7474 7269 6275 7465 733a  mary attributes:
+00002540: 0a20 2020 2020 2d20 6062 6f6f 6b60 3a20  .     - `book`: 
+00002550: 2020 2020 2020 5468 6520 6042 6962 6c65        The `Bible
+00002560: 426f 6f6b 6020 6f66 2074 6865 2062 6f6f  Book` of the boo
+00002570: 6b20 6f66 2074 6865 2072 6566 6572 656e  k of the referen
+00002580: 6365 2e0a 2020 2020 202d 2060 6368 6170  ce..     - `chap
+00002590: 5f6e 756d 603a 2020 2054 6865 2063 6861  _num`:   The cha
+000025a0: 7074 6572 206e 756d 6265 7220 2869 6e64  pter number (ind
+000025b0: 6578 6564 2066 726f 6d20 3129 206f 6620  exed from 1) of 
+000025c0: 7468 6520 7265 6665 7265 6e63 652e 0a20  the reference.. 
+000025d0: 2020 2020 2d20 6076 6572 7365 5f6e 756d      - `verse_num
+000025e0: 603a 2020 5468 6520 7665 7273 6520 6e75  `:  The verse nu
+000025f0: 6d62 6572 2028 696e 6465 7865 6420 6672  mber (indexed fr
+00002600: 6f6d 2030 206f 7220 3129 206f 6620 7468  om 0 or 1) of th
+00002610: 6520 7265 6665 7265 6e63 652e 0a0a 2020  e reference...  
+00002620: 2020 4269 626c 6556 6572 7365 7320 6172    BibleVerses ar
+00002630: 6520 696d 6d75 7461 626c 652e 2054 6865  e immutable. The
+00002640: 7920 6361 6e20 6265 2063 6f6d 7061 7265  y can be compare
+00002650: 6420 7573 696e 6720 7468 6520 7374 616e  d using the stan
+00002660: 6461 7264 2063 6f6d 7061 7269 736f 6e20  dard comparison 
+00002670: 6f70 6572 6174 6f72 732c 2077 6869 6368  operators, which
+00002680: 2063 6f6d 7061 7265 2074 6865 0a20 2020   compare the.   
+00002690: 2060 626f 6f6b 602c 2060 6368 6170 5f6e   `book`, `chap_n
+000026a0: 756d 6020 616e 6420 6076 6572 7365 5f6e  um` and `verse_n
+000026b0: 756d 6020 696e 2074 6861 7420 6f72 6465  um` in that orde
+000026c0: 722e 0a20 2020 2027 2727 0a20 2020 2062  r..    '''.    b
+000026d0: 6f6f 6b3a 2020 2020 2020 2042 6962 6c65  ook:       Bible
+000026e0: 426f 6f6b 0a20 2020 2063 6861 705f 6e75  Book.    chap_nu
+000026f0: 6d3a 2020 2069 6e74 0a20 2020 2076 6572  m:   int.    ver
+00002700: 7365 5f6e 756d 3a20 2069 6e74 0a0a 2020  se_num:  int..  
+00002710: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00002720: 656c 662c 202a 6172 6773 2c20 666c 6167  elf, *args, flag
+00002730: 733a 2042 6962 6c65 466c 6167 203d 204e  s: BibleFlag = N
+00002740: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
+00002750: 2741 2060 4269 626c 6556 6572 7365 6020  'A `BibleVerse` 
+00002760: 6361 6e20 6265 2063 6f6e 7374 7275 6374  can be construct
+00002770: 6564 2069 6e20 616e 7920 6f66 2074 6865  ed in any of the
+00002780: 2066 6f6c 6c6f 7769 6e67 2077 6179 733a   following ways:
+00002790: 0a0a 2020 2020 2020 2020 312e 2046 726f  ..        1. Fro
+000027a0: 6d20 6120 7369 6e67 6c65 2073 7472 696e  m a single strin
+000027b0: 673a 2060 4269 626c 6556 6572 7365 2822  g: `BibleVerse("
+000027c0: 4d61 726b 2032 3a33 2229 600a 0a20 2020  Mark 2:3")`..   
+000027d0: 2020 2020 2020 2020 5261 6973 6573 2061          Raises a
+000027e0: 2060 4269 626c 6552 6566 5061 7273 696e   `BibleRefParsin
+000027f0: 6745 7272 6f72 6020 6966 2074 6865 2073  gError` if the s
+00002800: 7472 696e 6720 6361 6e6e 6f74 2062 6520  tring cannot be 
+00002810: 7061 7273 6564 2e0a 0a20 2020 2020 2020  parsed...       
+00002820: 2032 2e20 4672 6f6d 2061 2042 6962 6c65   2. From a Bible
+00002830: 2062 6f6f 6b2c 2063 6861 7074 6572 2061   book, chapter a
+00002840: 6e64 2076 6572 7365 206e 756d 6265 7273  nd verse numbers
+00002850: 2e20 5468 6520 4269 626c 6520 626f 6f6b  . The Bible book
+00002860: 2063 616e 2062 6520 6120 7374 7269 6e67   can be a string
+00002870: 206e 616d 652c 206f 7220 6120 6042 6962   name, or a `Bib
+00002880: 6c65 426f 6f6b 6020 656e 756d 3a0a 2020  leBook` enum:.  
+00002890: 2020 2020 2020 2020 2060 4269 626c 6556           `BibleV
+000028a0: 6572 7365 2822 4d61 726b 222c 2032 2c20  erse("Mark", 2, 
+000028b0: 3329 602c 206f 7220 6042 6962 6c65 5665  3)`, or `BibleVe
+000028c0: 7273 6528 4269 626c 6542 6f6f 6b2e 4d61  rse(BibleBook.Ma
+000028d0: 726b 2c20 322c 2033 2960 0a20 2020 2020  rk, 2, 3)`.     
+000028e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000028f0: 332e 2041 7320 6120 636f 7079 206f 6620  3. As a copy of 
+00002900: 616e 6f74 6865 7220 4269 626c 6556 6572  another BibleVer
+00002910: 7365 3a20 6042 6962 6c65 5665 7273 6528  se: `BibleVerse(
+00002920: 6578 6973 7469 6e67 5f62 6962 6c65 5f76  existing_bible_v
+00002930: 6572 7365 2960 0a0a 2020 2020 2020 2020  erse)`..        
+00002940: 4966 2074 6865 2073 7570 706c 6965 6420  If the supplied 
+00002950: 6172 6775 6d65 6e74 7320 6172 6520 6e6f  arguments are no
+00002960: 7420 6120 7661 6c69 6420 7665 7273 652c  t a valid verse,
+00002970: 2061 6e20 6049 6e76 616c 6964 5265 6665   an `InvalidRefe
+00002980: 7265 6e63 6545 7272 6f72 6020 6973 2072  renceError` is r
+00002990: 6169 7365 642e 0a20 2020 2020 2020 2027  aised..        '
+000029a0: 2727 0a20 2020 2020 2020 2069 6620 6c65  ''.        if le
+000029b0: 6e28 6172 6773 2920 3d3d 2031 3a0a 2020  n(args) == 1:.  
+000029c0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000029d0: 6e73 7461 6e63 6528 6172 6773 5b30 5d2c  nstance(args[0],
+000029e0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+000029f0: 2020 2020 2020 2072 616e 6765 5f6c 6973         range_lis
+00002a00: 7420 3d20 4269 626c 6552 616e 6765 4c69  t = BibleRangeLi
+00002a10: 7374 2861 7267 735b 305d 2c20 666c 6167  st(args[0], flag
+00002a20: 733d 666c 6167 7329 0a20 2020 2020 2020  s=flags).       
+00002a30: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00002a40: 7261 6e67 655f 6c69 7374 2920 213d 2031  range_list) != 1
+00002a50: 206f 7220 6e6f 7420 7261 6e67 655f 6c69   or not range_li
+00002a60: 7374 5b30 5d2e 6973 5f73 696e 676c 655f  st[0].is_single_
+00002a70: 7665 7273 6528 293a 0a20 2020 2020 2020  verse():.       
+00002a80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00002a90: 7365 2049 6e76 616c 6964 5265 6665 7265  se InvalidRefere
+00002aa0: 6e63 6545 7272 6f72 2866 2253 7472 696e  nceError(f"Strin
+00002ab0: 6720 6973 206e 6f74 2061 2073 696e 676c  g is not a singl
+00002ac0: 6520 7665 7273 653a 207b 6172 6773 5b30  e verse: {args[0
+00002ad0: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00002ae0: 2020 2020 206f 626a 6563 742e 5f5f 7365       object.__se
+00002af0: 7461 7474 725f 5f28 7365 6c66 2c20 2262  tattr__(self, "b
+00002b00: 6f6f 6b22 2c20 7261 6e67 655f 6c69 7374  ook", range_list
+00002b10: 5b30 5d2e 7374 6172 742e 626f 6f6b 290a  [0].start.book).
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
+00002b40: 5f5f 2873 656c 662c 2022 6368 6170 5f6e  __(self, "chap_n
+00002b50: 756d 222c 2072 616e 6765 5f6c 6973 745b  um", range_list[
+00002b60: 305d 2e73 7461 7274 2e63 6861 705f 6e75  0].start.chap_nu
+00002b70: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+00002b80: 2020 206f 626a 6563 742e 5f5f 7365 7461     object.__seta
+00002b90: 7474 725f 5f28 7365 6c66 2c20 2276 6572  ttr__(self, "ver
+00002ba0: 7365 5f6e 756d 222c 2072 616e 6765 5f6c  se_num", range_l
+00002bb0: 6973 745b 305d 2e73 7461 7274 2e76 6572  ist[0].start.ver
+00002bc0: 7365 5f6e 756d 290a 2020 2020 2020 2020  se_num).        
+00002bd0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00002be0: 6e63 6528 6172 6773 5b30 5d2c 2042 6962  nce(args[0], Bib
+00002bf0: 6c65 5665 7273 6529 3a0a 2020 2020 2020  leVerse):.      
+00002c00: 2020 2020 2020 2020 2020 2320 5765 2068            # We h
+00002c10: 6176 6520 746f 2075 7365 206f 626a 6563  ave to use objec
+00002c20: 742e 5f5f 7365 7461 7474 725f 5f20 6265  t.__setattr__ be
+00002c30: 6361 7573 6520 7468 6520 636c 6173 7320  cause the class 
+00002c40: 6973 2066 726f 7a65 6e0a 2020 2020 2020  is frozen.      
+00002c50: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+00002c60: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
+00002c70: 662c 2022 626f 6f6b 222c 2061 7267 735b  f, "book", args[
+00002c80: 305d 2e62 6f6f 6b29 0a20 2020 2020 2020  0].book).       
+00002c90: 2020 2020 2020 2020 206f 626a 6563 742e           object.
+00002ca0: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
+00002cb0: 2c20 2263 6861 705f 6e75 6d22 2c20 6172  , "chap_num", ar
+00002cc0: 6773 5b30 5d2e 6368 6170 5f6e 756d 290a  gs[0].chap_num).
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
+00002cf0: 5f5f 2873 656c 662c 2022 7665 7273 655f  __(self, "verse_
+00002d00: 6e75 6d22 2c20 6172 6773 5b30 5d2e 7665  num", args[0].ve
+00002d10: 7273 655f 6e75 6d29 0a20 2020 2020 2020  rse_num).       
+00002d20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002d30: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002d40: 2056 616c 7565 4572 726f 7228 2253 696e   ValueError("Sin
+00002d50: 676c 6520 6172 6775 6d65 6e74 2074 6f20  gle argument to 
+00002d60: 4269 626c 6556 6572 7365 2063 616e 206f  BibleVerse can o
+00002d70: 6e6c 7920 6265 2061 2073 7472 696e 6720  nly be a string 
+00002d80: 6f72 2061 6e6f 7468 6572 2042 6962 6c65  or another Bible
+00002d90: 5665 7273 6522 290a 2020 2020 2020 2020  Verse").        
+00002da0: 656c 6966 206c 656e 2861 7267 7329 203e  elif len(args) >
+00002db0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+00002dc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00002dd0: 2822 546f 6f20 6d61 6e79 2061 7267 756d  ("Too many argum
+00002de0: 656e 7473 2073 7570 706c 6965 6420 746f  ents supplied to
+00002df0: 2042 6962 6c65 5665 7273 6522 290a 2020   BibleVerse").  
+00002e00: 2020 2020 2020 656c 6966 206c 656e 2861        elif len(a
+00002e10: 7267 7329 203c 2033 3a0a 2020 2020 2020  rgs) < 3:.      
+00002e20: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00002e30: 6545 7272 6f72 2822 546f 6f20 6665 7720  eError("Too few 
+00002e40: 6172 6775 6d65 6e74 7320 7375 7070 6c69  arguments suppli
+00002e50: 6564 2074 6f20 4269 626c 6556 6572 7365  ed to BibleVerse
+00002e60: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00002e70: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
+00002e80: 6b20 3d20 6172 6773 5b30 5d0a 2020 2020  k = args[0].    
+00002e90: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
+00002ea0: 3a20 696e 7420 3d20 6172 6773 5b31 5d0a  : int = args[1].
+00002eb0: 2020 2020 2020 2020 2020 2020 7665 7273              vers
+00002ec0: 655f 6e75 6d3a 2069 6e74 203d 2061 7267  e_num: int = arg
+00002ed0: 735b 325d 0a20 2020 2020 2020 2020 2020  s[2].           
+00002ee0: 2069 6620 6973 696e 7374 616e 6365 2862   if isinstance(b
+00002ef0: 6f6f 6b2c 2073 7472 293a 0a20 2020 2020  ook, str):.     
+00002f00: 2020 2020 2020 2020 2020 2062 6f6f 6b20             book 
+00002f10: 3d20 4269 626c 6542 6f6f 6b2e 6672 6f6d  = BibleBook.from
+00002f20: 5f73 7472 2862 6f6f 6b2c 2072 6169 7365  _str(book, raise
+00002f30: 5f65 7272 6f72 3d54 7275 6529 0a20 2020  _error=True).   
+00002f40: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
+00002f50: 7420 6973 696e 7374 616e 6365 2862 6f6f  t isinstance(boo
+00002f60: 6b2c 2042 6962 6c65 426f 6f6b 293a 0a20  k, BibleBook):. 
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002f80: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00002f90: 6622 7b62 6f6f 6b7d 206d 7573 7420 6265  f"{book} must be
+00002fa0: 2061 2073 7472 696e 6720 6f72 2061 6e20   a string or an 
+00002fb0: 696e 7374 616e 6365 206f 6620 4269 626c  instance of Bibl
+00002fc0: 6542 6f6f 6b22 290a 2020 2020 2020 2020  eBook").        
+00002fd0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00002fe0: 7461 6e63 6528 6368 6170 5f6e 756d 2c20  tance(chap_num, 
+00002ff0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00003000: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00003010: 6545 7272 6f72 2866 227b 6368 6170 5f6e  eError(f"{chap_n
+00003020: 756d 7d20 6973 206e 6f74 2061 6e20 696e  um} is not an in
+00003030: 7465 6765 7220 6368 6170 7465 7220 6e75  teger chapter nu
+00003040: 6d62 6572 2229 0a20 2020 2020 2020 2020  mber").         
+00003050: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00003060: 616e 6365 2876 6572 7365 5f6e 756d 2c20  ance(verse_num, 
+00003070: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00003080: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00003090: 6545 7272 6f72 2866 227b 6368 6170 5f6e  eError(f"{chap_n
+000030a0: 756d 7d20 6973 206e 6f74 2061 6e20 696e  um} is not an in
+000030b0: 7465 6765 7220 7665 7273 6520 6e75 6d62  teger verse numb
+000030c0: 6572 2229 0a20 2020 2020 2020 2020 2020  er").           
+000030d0: 2069 6620 6368 6170 5f6e 756d 203c 2062   if chap_num < b
+000030e0: 6f6f 6b2e 6d69 6e5f 6368 6170 5f6e 756d  ook.min_chap_num
+000030f0: 2829 206f 7220 6368 6170 5f6e 756d 203e  () or chap_num >
+00003100: 2062 6f6f 6b2e 6d61 785f 6368 6170 5f6e   book.max_chap_n
+00003110: 756d 2829 3a0a 2020 2020 2020 2020 2020  um():.          
+00003120: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
+00003130: 6c69 6452 6566 6572 656e 6365 4572 726f  lidReferenceErro
+00003140: 7228 6622 4e6f 2063 6861 7074 6572 207b  r(f"No chapter {
+00003150: 6368 6170 5f6e 756d 7d20 696e 207b 626f  chap_num} in {bo
+00003160: 6f6b 2e74 6974 6c65 7d22 290a 2020 2020  ok.title}").    
+00003170: 2020 2020 2020 2020 6966 2076 6572 7365          if verse
+00003180: 5f6e 756d 203c 2062 6f6f 6b2e 6d69 6e5f  _num < book.min_
+00003190: 7665 7273 655f 6e75 6d28 6368 6170 5f6e  verse_num(chap_n
+000031a0: 756d 2c20 666c 6167 7329 206f 7220 7665  um, flags) or ve
+000031b0: 7273 655f 6e75 6d20 3e20 626f 6f6b 2e6d  rse_num > book.m
+000031c0: 6178 5f76 6572 7365 5f6e 756d 2863 6861  ax_verse_num(cha
+000031d0: 705f 6e75 6d29 3a0a 2020 2020 2020 2020  p_num):.        
+000031e0: 2020 2020 2020 2020 7261 6973 6520 496e          raise In
+000031f0: 7661 6c69 6452 6566 6572 656e 6365 4572  validReferenceEr
+00003200: 726f 7228 6622 4e6f 2076 6572 7365 207b  ror(f"No verse {
+00003210: 7665 7273 655f 6e75 6d7d 2069 6e20 7b62  verse_num} in {b
+00003220: 6f6f 6b2e 7469 746c 657d 207b 6368 6170  ook.title} {chap
+00003230: 5f6e 756d 7d22 290a 2020 2020 2020 2020  _num}").        
+00003240: 2020 2020 6f62 6a65 6374 2e5f 5f73 6574      object.__set
+00003250: 6174 7472 5f5f 2873 656c 662c 2022 626f  attr__(self, "bo
+00003260: 6f6b 222c 2062 6f6f 6b29 2023 2057 6520  ok", book) # We 
+00003270: 6861 7665 2074 6f20 7573 6520 6f62 6a65  have to use obje
+00003280: 6374 2e5f 5f73 6574 6174 7472 5f5f 2062  ct.__setattr__ b
+00003290: 6563 6175 7365 2074 6865 2063 6c61 7373  ecause the class
+000032a0: 2069 7320 6672 6f7a 656e 0a20 2020 2020   is frozen.     
+000032b0: 2020 2020 2020 206f 626a 6563 742e 5f5f         object.__
+000032c0: 7365 7461 7474 725f 5f28 7365 6c66 2c20  setattr__(self, 
+000032d0: 2263 6861 705f 6e75 6d22 2c20 6368 6170  "chap_num", chap
+000032e0: 5f6e 756d 290a 2020 2020 2020 2020 2020  _num).          
+000032f0: 2020 6f62 6a65 6374 2e5f 5f73 6574 6174    object.__setat
+00003300: 7472 5f5f 2873 656c 662c 2022 7665 7273  tr__(self, "vers
+00003310: 655f 6e75 6d22 2c20 7665 7273 655f 6e75  e_num", verse_nu
+00003320: 6d29 0a0a 2020 2020 6465 6620 6d69 6e5f  m)..    def min_
+00003330: 6368 6170 5f6e 756d 2873 656c 6629 202d  chap_num(self) -
+00003340: 3e20 696e 743a 0a20 2020 2020 2020 2027  > int:.        '
+00003350: 2727 5265 7475 726e 206c 6f77 6573 7420  ''Return lowest 
+00003360: 6368 6170 7465 7220 6e75 6d62 6572 2028  chapter number (
+00003370: 696e 6465 7865 6420 6672 6f6d 2031 2920  indexed from 1) 
+00003380: 6f66 2074 6865 2060 4269 626c 6542 6f6f  of the `BibleBoo
+00003390: 6b60 2063 6f6e 7461 696e 696e 6720 7468  k` containing th
+000033a0: 6973 2076 6572 7365 2e0a 2020 2020 2020  is verse..      
+000033b0: 2020 2727 270a 2020 2020 2020 2020 7265    '''.        re
+000033c0: 7475 726e 2073 656c 662e 626f 6f6b 2e6d  turn self.book.m
+000033d0: 696e 5f63 6861 705f 6e75 6d28 290a 0a20  in_chap_num().. 
+000033e0: 2020 2064 6566 206d 6178 5f63 6861 705f     def max_chap_
+000033f0: 6e75 6d28 7365 6c66 2920 2d3e 2069 6e74  num(self) -> int
+00003400: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+00003410: 7572 6e20 6869 6768 6573 7420 6368 6170  urn highest chap
+00003420: 7465 7220 6e75 6d62 6572 2028 696e 6465  ter number (inde
+00003430: 7865 6420 6672 6f6d 2031 2920 6f66 2074  xed from 1) of t
+00003440: 6865 2060 4269 626c 6542 6f6f 6b60 2063  he `BibleBook` c
+00003450: 6f6e 7461 696e 696e 6720 7468 6973 2076  ontaining this v
+00003460: 6572 7365 2e0a 2020 2020 2020 2020 2727  erse..        ''
+00003470: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
+00003480: 2073 656c 662e 626f 6f6b 2e6d 6178 5f63   self.book.max_c
+00003490: 6861 705f 6e75 6d28 290a 2020 2020 0a20  hap_num().    . 
+000034a0: 2020 2064 6566 2063 6861 705f 636f 756e     def chap_coun
+000034b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+000034c0: 2027 2727 5265 7475 726e 7320 7468 6520   '''Returns the 
+000034d0: 6e75 6d62 6572 206f 6620 6368 6170 7465  number of chapte
+000034e0: 7273 2069 6e20 7468 6520 6042 6962 6c65  rs in the `Bible
+000034f0: 426f 6f6b 6020 636f 6e74 6169 6e69 6e67  Book` containing
+00003500: 2074 6869 7320 7665 7273 652e 0a20 2020   this verse..   
+00003510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003520: 2072 6574 7572 6e20 7365 6c66 2e62 6f6f   return self.boo
+00003530: 6b2e 6368 6170 5f63 6f75 6e74 2829 0a0a  k.chap_count()..
+00003540: 2020 2020 6465 6620 6d69 6e5f 7665 7273      def min_vers
+00003550: 655f 6e75 6d28 7365 6c66 2c20 6368 6170  e_num(self, chap
+00003560: 5f6e 756d 3a20 696e 7420 3d20 4e6f 6e65  _num: int = None
+00003570: 2c20 666c 6167 733a 2042 6962 6c65 466c  , flags: BibleFl
+00003580: 6167 203d 204e 6f6e 6529 202d 3e20 696e  ag = None) -> in
+00003590: 743a 0a20 2020 2020 2020 2027 2727 5265  t:.        '''Re
+000035a0: 7475 726e 2074 6865 206c 6f77 6573 7420  turn the lowest 
+000035b0: 7665 7273 6520 6e75 6d62 6572 2028 3020  verse number (0 
+000035c0: 6f72 2031 2920 666f 7220 7468 6520 7370  or 1) for the sp
+000035d0: 6563 6966 6965 6420 6368 6170 7465 7220  ecified chapter 
+000035e0: 6f66 2074 6865 2060 4269 626c 6542 6f6f  of the `BibleBoo
+000035f0: 6b60 2063 6f6e 7461 696e 696e 670a 2020  k` containing.  
+00003600: 2020 2020 2020 7468 6973 2076 6572 7365        this verse
+00003610: 2e20 4966 206e 6f20 6368 6170 7465 7220  . If no chapter 
+00003620: 6973 2073 7065 6369 6669 6564 2c20 6974  is specified, it
+00003630: 2072 6574 7572 6e73 2074 6865 206c 6f77   returns the low
+00003640: 6573 7420 7665 7273 6520 6e75 6d62 6572  est verse number
+00003650: 206f 6620 7468 6520 6368 6170 7465 7220   of the chapter 
+00003660: 636f 6e74 6169 6e69 6e67 0a20 2020 2020  containing.     
+00003670: 2020 2074 6869 7320 6042 6962 6c65 5665     this `BibleVe
+00003680: 7273 6560 2e0a 2020 2020 2020 2020 2727  rse`..        ''
+00003690: 270a 2020 2020 2020 2020 6966 2063 6861  '.        if cha
+000036a0: 705f 6e75 6d20 6973 204e 6f6e 653a 0a20  p_num is None:. 
+000036b0: 2020 2020 2020 2020 2020 2063 6861 705f             chap_
+000036c0: 6e75 6d20 3d20 7365 6c66 2e63 6861 705f  num = self.chap_
+000036d0: 6e75 6d0a 2020 2020 2020 2020 7265 7475  num.        retu
+000036e0: 726e 2073 656c 662e 626f 6f6b 2e6d 696e  rn self.book.min
+000036f0: 5f76 6572 7365 5f6e 756d 2863 6861 705f  _verse_num(chap_
+00003700: 6e75 6d2c 2066 6c61 6773 3d66 6c61 6773  num, flags=flags
+00003710: 290a 0a20 2020 2064 6566 206d 6178 5f76  )..    def max_v
+00003720: 6572 7365 5f6e 756d 2873 656c 662c 2063  erse_num(self, c
+00003730: 6861 705f 6e75 6d3a 2069 6e74 2920 2d3e  hap_num: int) ->
+00003740: 2069 6e74 3a0a 2020 2020 2020 2020 2727   int:.        ''
+00003750: 2752 6574 7572 6e20 7468 6520 6869 6768  'Return the high
+00003760: 6573 7420 7665 7273 6520 6e75 6d62 6572  est verse number
+00003770: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
+00003780: 6564 2063 6861 7074 6572 206f 6620 7468  ed chapter of th
+00003790: 6520 6042 6962 6c65 426f 6f6b 6020 636f  e `BibleBook` co
+000037a0: 6e74 6169 6e69 6e67 2074 6869 7320 7665  ntaining this ve
+000037b0: 7273 652e 0a20 2020 2020 2020 2049 6620  rse..        If 
+000037c0: 6e6f 2063 6861 7074 6572 2069 7320 7370  no chapter is sp
+000037d0: 6563 6966 6965 642c 2069 7420 7265 7475  ecified, it retu
+000037e0: 726e 7320 7468 6520 6869 6768 6573 7420  rns the highest 
+000037f0: 7665 7273 6520 6e75 6d62 6572 206f 6620  verse number of 
+00003800: 7468 6520 6368 6170 7465 7220 636f 6e74  the chapter cont
+00003810: 6169 6e69 6e67 2074 6869 7320 6042 6962  aining this `Bib
+00003820: 6c65 5665 7273 6560 2e0a 2020 2020 2020  leVerse`..      
+00003830: 2020 2727 270a 2020 2020 2020 2020 6966    '''.        if
+00003840: 2063 6861 705f 6e75 6d20 6973 204e 6f6e   chap_num is Non
+00003850: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00003860: 6861 705f 6e75 6d20 3d20 7365 6c66 2e63  hap_num = self.c
+00003870: 6861 705f 6e75 6d0a 2020 2020 2020 2020  hap_num.        
+00003880: 7265 7475 726e 2073 656c 662e 626f 6f6b  return self.book
+00003890: 2e6d 6178 5f76 6572 7365 5f6e 756d 2863  .max_verse_num(c
+000038a0: 6861 705f 6e75 6d29 0a0a 2020 2020 6465  hap_num)..    de
+000038b0: 6620 6669 7273 745f 7665 7273 6528 7365  f first_verse(se
+000038c0: 6c66 2c20 6368 6170 5f6e 756d 3a20 696e  lf, chap_num: in
+000038d0: 7420 3d20 4e6f 6e65 2c20 666c 6167 733a  t = None, flags:
+000038e0: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
+000038f0: 6529 202d 3e20 2742 6962 6c65 5665 7273  e) -> 'BibleVers
+00003900: 6527 3a0a 2020 2020 2020 2020 2727 2752  e':.        '''R
+00003910: 6574 7572 6e73 2074 6865 2066 6972 7374  eturns the first
+00003920: 2060 4269 626c 6556 6572 7365 6020 6f66   `BibleVerse` of
+00003930: 2074 6865 2073 7065 6369 6669 6564 2063   the specified c
+00003940: 6861 7074 6572 206f 6620 7468 6520 6042  hapter of the `B
+00003950: 6962 6c65 426f 6f6b 6020 636f 6e74 6169  ibleBook` contai
+00003960: 6e69 6e67 0a20 2020 2020 2020 2074 6869  ning.        thi
+00003970: 7320 7665 7273 652e 2049 6620 6368 6170  s verse. If chap
+00003980: 2069 7320 604e 6f6e 6560 2c20 6974 2072   is `None`, it r
+00003990: 6574 7572 6e73 2074 6865 2066 6972 7374  eturns the first
+000039a0: 2060 4269 626c 6556 6572 7365 6020 6f66   `BibleVerse` of
+000039b0: 2074 6865 2063 6861 7074 6572 2063 6f6e   the chapter con
+000039c0: 7461 696e 696e 6720 7468 6973 0a20 2020  taining this.   
+000039d0: 2020 2020 2060 4269 626c 6556 6572 7365       `BibleVerse
+000039e0: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
+000039f0: 2020 2020 2020 2069 6620 6368 6170 5f6e         if chap_n
+00003a00: 756d 2069 7320 4e6f 6e65 3a0a 2020 2020  um is None:.    
+00003a10: 2020 2020 2020 2020 6368 6170 5f6e 756d          chap_num
+00003a20: 203d 2073 656c 662e 6368 6170 5f6e 756d   = self.chap_num
+00003a30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003a40: 7365 6c66 2e62 6f6f 6b2e 6669 7273 745f  self.book.first_
+00003a50: 7665 7273 6528 6368 6170 5f6e 756d 2c20  verse(chap_num, 
+00003a60: 666c 6167 733d 666c 6167 7329 0a0a 2020  flags=flags)..  
+00003a70: 2020 6465 6620 6c61 7374 5f76 6572 7365    def last_verse
+00003a80: 2873 656c 662c 2063 6861 705f 6e75 6d3a  (self, chap_num:
+00003a90: 2069 6e74 203d 204e 6f6e 6529 202d 3e20   int = None) -> 
+00003aa0: 2742 6962 6c65 5665 7273 6527 3a0a 2020  'BibleVerse':.  
+00003ab0: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+00003ac0: 2074 6865 206c 6173 7420 6042 6962 6c65   the last `Bible
+00003ad0: 5665 7273 6560 206f 6620 7468 6520 7370  Verse` of the sp
+00003ae0: 6563 6966 6965 6420 6368 6170 7465 7220  ecified chapter 
+00003af0: 6f66 2074 6865 2060 4269 626c 6542 6f6f  of the `BibleBoo
+00003b00: 6b60 2063 6f6e 7461 696e 696e 670a 2020  k` containing.  
+00003b10: 2020 2020 2020 7468 6973 2076 6572 7365        this verse
+00003b20: 2e20 4966 2063 6861 7020 6973 2060 4e6f  . If chap is `No
+00003b30: 6e65 602c 2069 7420 7265 7475 726e 7320  ne`, it returns 
+00003b40: 7468 6520 6c61 7374 2060 4269 626c 6556  the last `BibleV
+00003b50: 6572 7365 6020 6f66 2074 6865 2063 6861  erse` of the cha
+00003b60: 7074 6572 2063 6f6e 7461 696e 696e 6720  pter containing 
+00003b70: 7468 6973 0a20 2020 2020 2020 2060 4269  this.        `Bi
+00003b80: 626c 6556 6572 7365 602e 0a20 2020 2020  bleVerse`..     
+00003b90: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+00003ba0: 6620 6368 6170 5f6e 756d 2069 7320 4e6f  f chap_num is No
+00003bb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003bc0: 6368 6170 5f6e 756d 203d 2073 656c 662e  chap_num = self.
+00003bd0: 6368 6170 5f6e 756d 0a20 2020 2020 2020  chap_num.       
+00003be0: 2072 6574 7572 6e20 7365 6c66 2e62 6f6f   return self.boo
+00003bf0: 6b2e 6c61 7374 5f76 6572 7365 2863 6861  k.last_verse(cha
+00003c00: 705f 6e75 6d29 0a0a 2020 2020 6465 6620  p_num)..    def 
+00003c10: 7665 7273 655f 305f 746f 5f31 2873 656c  verse_0_to_1(sel
+00003c20: 6629 202d 3e20 2742 6962 6c65 5665 7273  f) -> 'BibleVers
+00003c30: 6527 3a0a 2020 2020 2020 2020 2727 2749  e':.        '''I
+00003c40: 6620 7468 6520 6076 6572 7365 5f6e 756d  f the `verse_num
+00003c50: 6020 6f66 2074 6869 7320 6042 6962 6c65  ` of this `Bible
+00003c60: 5665 7273 6560 2069 7320 302c 2072 6574  Verse` is 0, ret
+00003c70: 7572 6e73 2061 6e20 6964 656e 7469 6361  urns an identica
+00003c80: 6c20 4269 626c 6556 6572 7365 2065 7863  l BibleVerse exc
+00003c90: 6570 7420 7769 7468 2060 7665 7273 655f  ept with `verse_
+00003ca0: 6e75 6d60 0a20 2020 2020 2020 2073 6574  num`.        set
+00003cb0: 2074 6f20 312e 204f 7468 6572 7769 7365   to 1. Otherwise
+00003cc0: 2c20 7265 7475 726e 7320 7468 6520 6f72  , returns the or
+00003cd0: 6967 696e 616c 2060 4269 626c 6556 6572  iginal `BibleVer
+00003ce0: 7365 602e 2727 270a 2020 2020 2020 2020  se`.'''.        
+00003cf0: 6966 2073 656c 662e 7665 7273 655f 6e75  if self.verse_nu
+00003d00: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
+00003d10: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+00003d20: 5665 7273 6528 7365 6c66 2e62 6f6f 6b2c  Verse(self.book,
+00003d30: 2073 656c 662e 6368 6170 5f6e 756d 2c20   self.chap_num, 
+00003d40: 3129 0a20 2020 2020 2020 2065 6c73 653a  1).        else:
+00003d50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003d60: 7572 6e20 7365 6c66 0a20 2020 200a 2020  urn self.    .  
+00003d70: 2020 6465 6620 7665 7273 655f 315f 746f    def verse_1_to
+00003d80: 5f30 2873 656c 6629 202d 3e20 2742 6962  _0(self) -> 'Bib
+00003d90: 6c65 5665 7273 6527 3a0a 2020 2020 2020  leVerse':.      
+00003da0: 2020 2727 2749 6620 7468 6520 6076 6572    '''If the `ver
+00003db0: 7365 5f6e 756d 6020 6f66 2074 6869 7320  se_num` of this 
+00003dc0: 6042 6962 6c65 5665 7273 6560 2069 7320  `BibleVerse` is 
+00003dd0: 312c 2061 6e64 2061 2076 6572 7365 2030  1, and a verse 0
+00003de0: 2069 7320 706f 7373 6962 6c65 2066 6f72   is possible for
+00003df0: 2074 6865 0a20 2020 2020 2020 2073 616d   the.        sam
+00003e00: 6520 6368 6170 7465 722c 2072 6574 7572  e chapter, retur
+00003e10: 6e73 2061 6e20 6964 656e 7469 6361 6c20  ns an identical 
+00003e20: 6042 6962 6c65 5665 7273 6560 2065 7863  `BibleVerse` exc
+00003e30: 6570 7420 7769 7468 2060 7665 7273 655f  ept with `verse_
+00003e40: 6e75 6d60 2073 6574 2074 6f20 302e 204f  num` set to 0. O
+00003e50: 7468 6572 7769 7365 2c20 7265 7475 726e  therwise, return
+00003e60: 7320 7468 650a 2020 2020 2020 2020 6f72  s the.        or
+00003e70: 6967 696e 616c 2060 4269 626c 6556 6572  iginal `BibleVer
+00003e80: 7365 602e 202a 2a4e 6f74 652a 2a3a 2054  se`. **Note**: T
+00003e90: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00003ea0: 676c 6f62 616c 2061 7474 7269 6275 7465  global attribute
+00003eb0: 2060 6269 626c 6572 6566 2e72 6566 2e66   `bibleref.ref.f
+00003ec0: 6c61 6773 6020 6973 202a 6967 6e6f 7265  lags` is *ignore
+00003ed0: 642a 2e27 2727 0a20 2020 2020 2020 2069  d*.'''.        i
+00003ee0: 6620 7365 6c66 2e76 6572 7365 5f6e 756d  f self.verse_num
+00003ef0: 203d 3d20 3120 616e 6420 7365 6c66 2e6d   == 1 and self.m
+00003f00: 696e 5f76 6572 7365 5f6e 756d 2873 656c  in_verse_num(sel
+00003f10: 662e 6368 6170 5f6e 756d 2c20 666c 6167  f.chap_num, flag
+00003f20: 733d 4269 626c 6546 6c61 672e 5645 5253  s=BibleFlag.VERS
+00003f30: 455f 3029 203d 3d20 303a 0a20 2020 2020  E_0) == 0:.     
+00003f40: 2020 2020 2020 2072 6574 7572 6e20 4269         return Bi
+00003f50: 626c 6556 6572 7365 2873 656c 662e 626f  bleVerse(self.bo
+00003f60: 6f6b 2c20 7365 6c66 2e63 6861 705f 6e75  ok, self.chap_nu
+00003f70: 6d2c 2030 2c20 666c 6167 733d 4269 626c  m, 0, flags=Bibl
+00003f80: 6546 6c61 672e 5645 5253 455f 3029 0a20  eFlag.VERSE_0). 
+00003f90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003fa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003fb0: 7365 6c66 0a0a 2020 2020 6465 6620 6164  self..    def ad
+00003fc0: 645f 6e75 6d5f 7665 7273 6573 2873 656c  d_num_verses(sel
+00003fd0: 662c 206e 756d 5f76 6572 7365 733a 2069  f, num_verses: i
+00003fe0: 6e74 2c20 666c 6167 733a 2042 6962 6c65  nt, flags: Bible
+00003ff0: 466c 6167 203d 204e 6f6e 6529 202d 3e20  Flag = None) -> 
+00004000: 2742 6962 6c65 5665 7273 6527 3a0a 2020  'BibleVerse':.  
+00004010: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+00004020: 2061 206e 6577 2060 4269 626c 6556 6572   a new `BibleVer
+00004030: 7365 6020 7468 6174 2069 7320 606e 756d  se` that is `num
+00004040: 5f76 6572 7365 7360 2061 6674 6572 2074  _verses` after t
+00004050: 6869 7320 6042 6962 6c65 5665 7273 6560  his `BibleVerse`
+00004060: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00004070: 2020 2049 6620 6042 6962 6c65 466c 6167     If `BibleFlag
+00004080: 2e4d 554c 5449 424f 4f4b 6020 6973 2073  .MULTIBOOK` is s
+00004090: 6574 2028 6569 7468 6572 2062 7920 7468  et (either by th
+000040a0: 6520 6066 6c61 6773 6020 6172 6775 6d65  e `flags` argume
+000040b0: 6e74 206f 722c 2069 6620 604e 6f6e 6560  nt or, if `None`
+000040c0: 2c20 6279 2074 6865 2067 6c6f 6261 6c20  , by the global 
+000040d0: 6174 7472 6962 7574 6529 2c20 616e 640a  attribute), and.
+000040e0: 2020 2020 2020 2020 7468 6520 7265 7375          the resu
+000040f0: 6c74 2077 6f75 6c64 2062 6520 6265 796f  lt would be beyo
+00004100: 6e64 2074 6865 2063 7572 7265 6e74 2062  nd the current b
+00004110: 6f6f 6b2c 2061 2076 6572 7365 2069 6e20  ook, a verse in 
+00004120: 7468 6520 6e65 7874 2062 6f6f 6b20 6973  the next book is
+00004130: 2072 6574 7572 6e65 642e 204f 7468 6572   returned. Other
+00004140: 7769 7365 2c20 6966 2074 6865 2076 6572  wise, if the ver
+00004150: 7365 0a20 2020 2020 2020 2064 6f65 7320  se.        does 
+00004160: 6e6f 7420 6578 6973 742c 2060 4e6f 6e65  not exist, `None
+00004170: 6020 6973 2072 6574 7572 6e65 642e 2049  ` is returned. I
+00004180: 6620 7468 6520 6076 6572 7365 5f6e 756d  f the `verse_num
+00004190: 6020 6f66 2074 6869 7320 6042 6962 6c65  ` of this `Bible
+000041a0: 5665 7273 6560 2069 7320 616c 7265 6164  Verse` is alread
+000041b0: 7920 302c 0a20 2020 2020 2020 2060 4269  y 0,.        `Bi
+000041c0: 626c 6546 6c61 672e 5645 5253 455f 3060  bleFlag.VERSE_0`
+000041d0: 2069 7320 666f 7263 6520 7365 7420 6f6e   is force set on
+000041e0: 2074 6865 2060 666c 6167 7360 2061 7267   the `flags` arg
+000041f0: 756d 656e 7420 666f 7220 7468 6973 2063  ument for this c
+00004200: 616c 6c2e 0a0a 2020 2020 2020 2020 5573  all...        Us
+00004210: 696e 6720 7468 6520 602b 6020 6f70 6572  ing the `+` oper
+00004220: 6174 6f72 2069 7320 6571 7569 7661 6c65  ator is equivale
+00004230: 6e74 2074 6f20 6361 6c6c 696e 6720 6061  nt to calling `a
+00004240: 6464 5f6e 756d 5f76 6572 7365 7328 2960  dd_num_verses()`
+00004250: 2077 6974 6820 6066 6c61 6773 203d 204e   with `flags = N
+00004260: 6f6e 6560 2e0a 2020 2020 2020 2020 2727  one`..        ''
+00004270: 270a 2020 2020 2020 2020 666c 6167 7320  '.        flags 
+00004280: 3d20 666c 6167 7320 6f72 2067 6c6f 6261  = flags or globa
+00004290: 6c73 2829 5b27 666c 6167 7327 5d20 6f72  ls()['flags'] or
+000042a0: 2042 6962 6c65 466c 6167 2e4e 4f4e 450a   BibleFlag.NONE.
+000042b0: 2020 2020 2020 2020 626f 6f6b 203d 2073          book = s
+000042c0: 656c 662e 626f 6f6b 0a20 2020 2020 2020  elf.book.       
+000042d0: 2063 6861 705f 6e75 6d20 3d20 7365 6c66   chap_num = self
+000042e0: 2e63 6861 705f 6e75 6d0a 2020 2020 2020  .chap_num.      
+000042f0: 2020 6966 2073 656c 662e 7665 7273 655f    if self.verse_
+00004300: 6e75 6d20 3d3d 2030 3a0a 2020 2020 2020  num == 0:.      
+00004310: 2020 2020 2020 666c 6167 7320 3d20 666c        flags = fl
+00004320: 6167 7320 7c20 4269 626c 6546 6c61 672e  ags | BibleFlag.
+00004330: 5645 5253 455f 3020 2320 486f 6e6f 7572  VERSE_0 # Honour
+00004340: 2065 7869 7374 696e 6720 7665 7273 6520   existing verse 
+00004350: 3073 0a20 2020 2020 2020 2076 6572 7365  0s.        verse
+00004360: 5f6e 756d 203d 2073 656c 662e 7665 7273  _num = self.vers
+00004370: 655f 6e75 6d20 2b20 6e75 6d5f 7665 7273  e_num + num_vers
+00004380: 6573 0a20 2020 2020 2020 206d 6178 5f76  es.        max_v
+00004390: 6572 7365 5f6e 756d 203d 2062 6f6f 6b2e  erse_num = book.
+000043a0: 6d61 785f 7665 7273 655f 6e75 6d28 6368  max_verse_num(ch
+000043b0: 6170 5f6e 756d 290a 2020 2020 2020 2020  ap_num).        
+000043c0: 7768 696c 6520 7665 7273 655f 6e75 6d20  while verse_num 
+000043d0: 3e20 6d61 785f 7665 7273 655f 6e75 6d3a  > max_verse_num:
+000043e0: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+000043f0: 705f 6e75 6d20 2b3d 2031 0a20 2020 2020  p_num += 1.     
+00004400: 2020 2020 2020 2069 6620 6368 6170 5f6e         if chap_n
+00004410: 756d 203e 2062 6f6f 6b2e 6d61 785f 6368  um > book.max_ch
+00004420: 6170 5f6e 756d 2829 3a0a 2020 2020 2020  ap_num():.      
+00004430: 2020 2020 2020 2020 2020 6966 2042 6962            if Bib
+00004440: 6c65 466c 6167 2e4d 554c 5449 424f 4f4b  leFlag.MULTIBOOK
+00004450: 206e 6f74 2069 6e20 666c 6167 733a 0a20   not in flags:. 
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00004480: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004490: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000044a0: 2020 2020 2020 2020 2062 6f6f 6b20 3d20           book = 
+000044b0: 626f 6f6b 2e6e 6578 7428 290a 2020 2020  book.next().    
+000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044d0: 6966 2062 6f6f 6b20 6973 204e 6f6e 653a  if book is None:
+000044e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000044f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004500: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00004510: 2020 2020 2020 2020 2063 6861 705f 6e75           chap_nu
+00004520: 6d20 3d20 626f 6f6b 2e6d 696e 5f63 6861  m = book.min_cha
+00004530: 705f 6e75 6d28 290a 2020 2020 2020 2020  p_num().        
+00004540: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00004550: 2076 6572 7365 5f6e 756d 203d 2076 6572   verse_num = ver
+00004560: 7365 5f6e 756d 202d 206d 6178 5f76 6572  se_num - max_ver
+00004570: 7365 5f6e 756d 202b 2062 6f6f 6b2e 6d69  se_num + book.mi
+00004580: 6e5f 7665 7273 655f 6e75 6d28 6368 6170  n_verse_num(chap
+00004590: 5f6e 756d 2c20 666c 6167 7329 202d 2031  _num, flags) - 1
+000045a0: 200a 2020 2020 2020 2020 2020 2020 6d61   .            ma
+000045b0: 785f 7665 7273 655f 6e75 6d20 3d20 626f  x_verse_num = bo
+000045c0: 6f6b 2e6d 6178 5f76 6572 7365 5f6e 756d  ok.max_verse_num
+000045d0: 2863 6861 705f 6e75 6d29 0a0a 2020 2020  (chap_num)..    
+000045e0: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+000045f0: 5665 7273 6528 626f 6f6b 2c20 6368 6170  Verse(book, chap
+00004600: 5f6e 756d 2c20 7665 7273 655f 6e75 6d2c  _num, verse_num,
+00004610: 2066 6c61 6773 3d66 6c61 6773 290a 0a20   flags=flags).. 
+00004620: 2020 2064 6566 2073 7562 5f6e 756d 5f76     def sub_num_v
+00004630: 6572 7365 7328 7365 6c66 2c20 6e75 6d5f  erses(self, num_
+00004640: 7665 7273 6573 3a20 696e 742c 2066 6c61  verses: int, fla
+00004650: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
+00004660: 4e6f 6e65 2920 2d3e 2027 4269 626c 6556  None) -> 'BibleV
+00004670: 6572 7365 273a 0a20 2020 2020 2020 2027  erse':.        '
+00004680: 2727 5265 7475 726e 2061 206e 6577 2060  ''Return a new `
+00004690: 4269 626c 6556 6572 7365 6020 7468 6174  BibleVerse` that
+000046a0: 2069 7320 606e 756d 5f76 6572 7365 7360   is `num_verses`
+000046b0: 2062 6566 6f72 6520 7468 6973 2060 4269   before this `Bi
+000046c0: 626c 6556 6572 7365 602e 0a20 2020 2020  bleVerse`..     
+000046d0: 2020 200a 2020 2020 2020 2020 4966 2060     .        If `
+000046e0: 4269 626c 6546 6c61 672e 4d55 4c54 4942  BibleFlag.MULTIB
+000046f0: 4f4f 4b60 2069 7320 7365 7420 2865 6974  OOK` is set (eit
+00004700: 6865 7220 7365 7420 6279 2074 6865 2060  her set by the `
+00004710: 666c 6167 7360 2061 7267 756d 656e 7420  flags` argument 
+00004720: 6f72 2c20 6966 2060 4e6f 6e65 602c 2074  or, if `None`, t
+00004730: 6865 2067 6c6f 6261 6c20 6174 7472 6962  he global attrib
+00004740: 7574 6529 2c20 616e 640a 2020 2020 2020  ute), and.      
+00004750: 2020 7468 6520 7265 7375 6c74 2077 6f75    the result wou
+00004760: 6c64 2062 6520 6265 666f 7265 2074 6865  ld be before the
+00004770: 2063 7572 7265 6e74 2062 6f6f 6b2c 2061   current book, a
+00004780: 2076 6572 7365 2069 6e20 7468 6520 7072   verse in the pr
+00004790: 6576 696f 7573 2062 6f6f 6b20 6973 2072  evious book is r
+000047a0: 6574 7572 6e65 642e 204f 7468 6572 7769  eturned. Otherwi
+000047b0: 7365 2c20 6966 2074 6865 0a20 2020 2020  se, if the.     
+000047c0: 2020 2076 6572 7365 2064 6f65 7320 6e6f     verse does no
+000047d0: 7420 6578 6973 742c 204e 6f6e 6520 6973  t exist, None is
+000047e0: 2072 6574 7572 6e65 642e 2049 6620 7468   returned. If th
+000047f0: 6520 6076 6572 7365 5f6e 756d 6020 6f66  e `verse_num` of
+00004800: 2074 6869 7320 6042 6962 6c65 5665 7273   this `BibleVers
+00004810: 6560 2069 7320 616c 7265 6164 7920 302c  e` is already 0,
+00004820: 0a20 2020 2020 2020 2060 4269 626c 6546  .        `BibleF
+00004830: 6c61 672e 5645 5253 455f 3060 2069 7320  lag.VERSE_0` is 
+00004840: 666f 7263 6520 7365 7420 6f6e 2074 6865  force set on the
+00004850: 2060 666c 6167 7360 2061 7267 756d 656e   `flags` argumen
+00004860: 7420 666f 7220 7468 6973 2063 616c 6c2e  t for this call.
+00004870: 0a0a 2020 2020 2020 2020 5573 696e 6720  ..        Using 
+00004880: 7468 6520 602d 6020 6f70 6572 6174 6f72  the `-` operator
+00004890: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
+000048a0: 6f20 6361 6c6c 696e 6720 6061 6464 5f6e  o calling `add_n
+000048b0: 756d 5f76 6572 7365 7328 2960 2077 6974  um_verses()` wit
+000048c0: 6820 6066 6c61 6773 203d 204e 6f6e 6560  h `flags = None`
+000048d0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+000048e0: 2020 2020 2020 666c 6167 7320 3d20 666c        flags = fl
+000048f0: 6167 7320 6f72 2067 6c6f 6261 6c73 2829  ags or globals()
+00004900: 5b27 666c 6167 7327 5d20 6f72 2042 6962  ['flags'] or Bib
+00004910: 6c65 466c 6167 2e4e 4f4e 450a 2020 2020  leFlag.NONE.    
+00004920: 2020 2020 626f 6f6b 203d 2073 656c 662e      book = self.
+00004930: 626f 6f6b 0a20 2020 2020 2020 2063 6861  book.        cha
+00004940: 705f 6e75 6d20 3d20 7365 6c66 2e63 6861  p_num = self.cha
+00004950: 705f 6e75 6d0a 2020 2020 2020 2020 6966  p_num.        if
+00004960: 2073 656c 662e 7665 7273 655f 6e75 6d20   self.verse_num 
+00004970: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00004980: 2020 666c 6167 7320 3d20 666c 6167 7320    flags = flags 
+00004990: 7c20 4269 626c 6546 6c61 672e 5645 5253  | BibleFlag.VERS
+000049a0: 455f 3020 2320 486f 6e6f 7572 2065 7869  E_0 # Honour exi
+000049b0: 7374 696e 6720 7665 7273 6520 3073 0a20  sting verse 0s. 
+000049c0: 2020 2020 2020 2076 6572 7365 5f6e 756d         verse_num
+000049d0: 203d 2073 656c 662e 7665 7273 655f 6e75   = self.verse_nu
+000049e0: 6d20 2d20 6e75 6d5f 7665 7273 6573 0a20  m - num_verses. 
+000049f0: 2020 2020 2020 206d 696e 5f76 6572 7365         min_verse
+00004a00: 5f6e 756d 203d 2062 6f6f 6b2e 6d69 6e5f  _num = book.min_
+00004a10: 7665 7273 655f 6e75 6d28 6368 6170 5f6e  verse_num(chap_n
+00004a20: 756d 2c20 666c 6167 7329 0a20 2020 2020  um, flags).     
+00004a30: 2020 2077 6869 6c65 2076 6572 7365 5f6e     while verse_n
+00004a40: 756d 203c 206d 696e 5f76 6572 7365 5f6e  um < min_verse_n
+00004a50: 756d 3a0a 2020 2020 2020 2020 2020 2020  um:.            
+00004a60: 6368 6170 5f6e 756d 202d 3d20 310a 2020  chap_num -= 1.  
+00004a70: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
+00004a80: 705f 6e75 6d20 3c20 626f 6f6b 2e6d 696e  p_num < book.min
+00004a90: 5f63 6861 705f 6e75 6d28 293a 0a20 2020  _chap_num():.   
+00004aa0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004ab0: 4269 626c 6546 6c61 672e 4d55 4c54 4942  BibleFlag.MULTIB
+00004ac0: 4f4f 4b20 6e6f 7420 696e 2066 6c61 6773  OOK not in flags
+00004ad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004ae0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00004af0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00004b00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004b10: 2020 2020 2020 2020 2020 2020 626f 6f6b              book
+00004b20: 203d 2062 6f6f 6b2e 7072 6576 2829 0a20   = book.prev(). 
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2069 6620 626f 6f6b 2069 7320 4e6f     if book is No
+00004b50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004b60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004b70: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00004b80: 2020 2020 2020 2020 2020 2020 6368 6170              chap
+00004b90: 5f6e 756d 203d 2062 6f6f 6b2e 6d61 785f  _num = book.max_
+00004ba0: 6368 6170 5f6e 756d 2829 0a20 2020 2020  chap_num().     
+00004bb0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004bc0: 2020 2020 2076 6572 7365 5f6e 756d 203d       verse_num =
+00004bd0: 2076 6572 7365 5f6e 756d 202b 2062 6f6f   verse_num + boo
+00004be0: 6b2e 6d61 785f 7665 7273 655f 6e75 6d28  k.max_verse_num(
+00004bf0: 6368 6170 5f6e 756d 2920 2d20 6d69 6e5f  chap_num) - min_
+00004c00: 7665 7273 655f 6e75 6d20 2b20 3120 0a20  verse_num + 1 . 
+00004c10: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
+00004c20: 6572 7365 5f6e 756d 203d 2062 6f6f 6b2e  erse_num = book.
+00004c30: 6d69 6e5f 7665 7273 655f 6e75 6d28 6368  min_verse_num(ch
+00004c40: 6170 5f6e 756d 290a 0a20 2020 2020 2020  ap_num)..       
+00004c50: 2072 6574 7572 6e20 4269 626c 6556 6572   return BibleVer
+00004c60: 7365 2862 6f6f 6b2c 2063 6861 705f 6e75  se(book, chap_nu
+00004c70: 6d2c 2076 6572 7365 5f6e 756d 2c20 666c  m, verse_num, fl
+00004c80: 6167 733d 666c 6167 7329 0a0a 2020 2020  ags=flags)..    
+00004c90: 6465 6620 5f5f 6164 645f 5f28 7365 6c66  def __add__(self
+00004ca0: 2c20 6e75 6d5f 7665 7273 6573 3a20 696e  , num_verses: in
+00004cb0: 7429 202d 3e20 2742 6962 6c65 5665 7273  t) -> 'BibleVers
+00004cc0: 6527 3a0a 2020 2020 2020 2020 6966 206e  e':.        if n
+00004cd0: 6f74 2069 7369 6e73 7461 6e63 6528 6e75  ot isinstance(nu
+00004ce0: 6d5f 7665 7273 6573 2c20 696e 7429 3a0a  m_verses, int):.
+00004cf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004d00: 726e 204e 6f74 496d 706c 656d 656e 7465  rn NotImplemente
+00004d10: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00004d20: 2073 656c 662e 6164 645f 6e75 6d5f 7665   self.add_num_ve
+00004d30: 7273 6573 286e 756d 5f76 6572 7365 7329  rses(num_verses)
+00004d40: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
+00004d50: 7375 625f 5f28 7365 6c66 2c20 6e75 6d5f  sub__(self, num_
+00004d60: 7665 7273 6573 3a20 696e 7429 202d 3e20  verses: int) -> 
+00004d70: 2742 6962 6c65 5665 7273 6527 3a0a 2020  'BibleVerse':.  
+00004d80: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00004d90: 6e73 7461 6e63 6528 6e75 6d5f 7665 7273  nstance(num_vers
+00004da0: 6573 2c20 696e 7429 3a0a 2020 2020 2020  es, int):.      
+00004db0: 2020 2020 2020 7265 7475 726e 204e 6f74        return Not
+00004dc0: 496d 706c 656d 656e 7465 640a 2020 2020  Implemented.    
+00004dd0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004de0: 7375 625f 6e75 6d5f 7665 7273 6573 286e  sub_num_verses(n
+00004df0: 756d 5f76 6572 7365 7329 0a0a 2020 2020  um_verses)..    
+00004e00: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+00004e10: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00004e20: 726e 2066 2242 6962 6c65 5665 7273 6528  rn f"BibleVerse(
+00004e30: 7b73 656c 662e 7374 7228 6162 6272 6576  {self.str(abbrev
+00004e40: 3d54 7275 6529 7d29 220a 0a20 2020 2064  =True)})"..    d
+00004e50: 6566 205f 5f73 7472 5f5f 2873 656c 6629  ef __str__(self)
+00004e60: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00004e70: 2073 656c 662e 7374 7228 290a 0a20 2020   self.str()..   
+00004e80: 2064 6566 2073 7472 2873 656c 662c 2061   def str(self, a
+00004e90: 6262 7265 763a 2062 6f6f 6c20 3d20 4661  bbrev: bool = Fa
+00004ea0: 6c73 652c 2061 6c74 5f73 6570 3a20 626f  lse, alt_sep: bo
+00004eb0: 6f6c 203d 2046 616c 7365 2c20 6e6f 7370  ol = False, nosp
+00004ec0: 6163 653a 2062 6f6f 6c20 3d20 4661 6c73  ace: bool = Fals
+00004ed0: 652c 0a20 2020 2020 2020 2020 2020 2076  e,.            v
+00004ee0: 6572 7365 5f70 6172 7473 3a20 4269 626c  erse_parts: Bibl
+00004ef0: 6556 6572 7365 5061 7274 203d 2042 6962  eVersePart = Bib
+00004f00: 6c65 5665 7273 6550 6172 742e 4655 4c4c  leVersePart.FULL
+00004f10: 5f52 4546 2920 2d3e 2073 7472 3a0a 2020  _REF) -> str:.  
+00004f20: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+00004f30: 2061 2063 6f6e 6669 6775 7261 626c 6520   a configurable 
+00004f40: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
+00004f50: 6174 696f 6e20 6f66 2074 6869 7320 4269  ation of this Bi
+00004f60: 626c 6556 6572 7365 2c20 6173 2066 6f6c  bleVerse, as fol
+00004f70: 6c6f 7773 3a0a 0a20 2020 2020 2020 202d  lows:..        -
+00004f80: 2049 6620 6061 6262 7265 7660 2069 7320   If `abbrev` is 
+00004f90: 5472 7565 2c20 7468 6520 6162 6272 6576  True, the abbrev
+00004fa0: 6961 7465 6420 6e61 6d65 206f 6620 7468  iated name of th
+00004fb0: 6520 626f 6f6b 2069 7320 7573 6564 2028  e book is used (
+00004fc0: 696e 7374 6561 6420 6f66 2074 6865 2066  instead of the f
+00004fd0: 756c 6c20 6e61 6d65 292e 0a20 2020 2020  ull name)..     
+00004fe0: 2020 202d 2049 6620 6061 6c74 5f73 6570     - If `alt_sep
+00004ff0: 6020 6973 2054 7275 652c 2063 6861 7074  ` is True, chapt
+00005000: 6572 2061 6e64 2076 6572 7365 206e 756d  er and verse num
+00005010: 6265 7273 2061 7265 2073 6570 6172 6174  bers are separat
+00005020: 6564 2062 7920 7468 6520 616c 7465 726e  ed by the altern
+00005030: 6174 650a 2020 2020 2020 2020 2020 7365  ate.          se
+00005040: 7061 7261 746f 7220 2860 2e60 2062 7920  parator (`.` by 
+00005050: 6465 6661 756c 7429 2069 6e73 7465 6164  default) instead
+00005060: 206f 6620 7468 6520 7374 616e 6461 7264   of the standard
+00005070: 2073 6570 6172 6174 6f72 2028 603a 6020   separator (`:` 
+00005080: 6279 2064 6566 6175 6c74 292e 0a20 2020  by default)..   
+00005090: 2020 2020 202d 2049 6620 606e 6f73 7061       - If `nospa
+000050a0: 6365 6020 6973 2054 7275 652c 206e 6f20  ce` is True, no 
+000050b0: 7370 6163 6573 2061 7265 2069 6e63 6c75  spaces are inclu
+000050c0: 6465 6420 696e 2074 6865 2073 7472 696e  ded in the strin
+000050d0: 672e 0a20 2020 2020 2020 202d 2060 7665  g..        - `ve
+000050e0: 7273 655f 7061 7274 7360 2069 7320 6120  rse_parts` is a 
+000050f0: 636f 6d62 696e 6174 696f 6e20 6f66 2060  combination of `
+00005100: 4269 626c 6556 6572 7365 5061 7274 6020  BibleVersePart` 
+00005110: 666c 6167 732c 2063 6f6e 7472 6f6c 6c69  flags, controlli
+00005120: 6e67 2077 6861 7420 636f 6d62 696e 6174  ng what combinat
+00005130: 696f 6e20 6f66 2062 6f6f 6b2c 0a20 2020  ion of book,.   
+00005140: 2020 2020 2020 2063 6861 7074 6572 2026         chapter &
+00005150: 2076 6572 7365 2061 7265 2064 6973 706c   verse are displ
+00005160: 6179 6564 2e0a 2020 2020 2020 2020 2727  ayed..        ''
+00005170: 270a 2020 2020 2020 2020 6966 2073 656c  '.        if sel
+00005180: 662e 626f 6f6b 2e63 6861 705f 636f 756e  f.book.chap_coun
+00005190: 7428 2920 3d3d 2031 3a0a 2020 2020 2020  t() == 1:.      
+000051a0: 2020 2020 2020 7665 7273 655f 7061 7274        verse_part
+000051b0: 7320 263d 207e 4269 626c 6556 6572 7365  s &= ~BibleVerse
+000051c0: 5061 7274 2e43 4841 5020 2320 446f 6e27  Part.CHAP # Don'
+000051d0: 7420 6469 7370 6c61 7920 6368 6170 0a20  t display chap. 
+000051e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000051f0: 6966 2042 6962 6c65 5665 7273 6550 6172  if BibleVersePar
+00005200: 742e 424f 4f4b 2069 6e20 7665 7273 655f  t.BOOK in verse_
+00005210: 7061 7274 733a 0a20 2020 2020 2020 2020  parts:.         
+00005220: 2020 2062 6f6f 6b5f 6e61 6d65 203d 2073     book_name = s
+00005230: 656c 662e 626f 6f6b 2e61 6262 7265 7620  elf.book.abbrev 
+00005240: 6966 2061 6262 7265 7620 656c 7365 2073  if abbrev else s
+00005250: 656c 662e 626f 6f6b 2e74 6974 6c65 0a20  elf.book.title. 
+00005260: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005270: 2020 2020 2020 2020 2062 6f6f 6b5f 6e61           book_na
+00005280: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
+00005290: 0a20 2020 2020 2020 2063 6861 705f 7374  .        chap_st
+000052a0: 7220 3d20 7374 7228 7365 6c66 2e63 6861  r = str(self.cha
+000052b0: 705f 6e75 6d29 2069 6620 4269 626c 6556  p_num) if BibleV
+000052c0: 6572 7365 5061 7274 2e43 4841 5020 696e  ersePart.CHAP in
+000052d0: 2076 6572 7365 5f70 6172 7473 2065 6c73   verse_parts els
+000052e0: 6520 2222 0a20 2020 2020 2020 2076 6572  e "".        ver
+000052f0: 7365 5f73 7472 203d 2073 7472 2873 656c  se_str = str(sel
+00005300: 662e 7665 7273 655f 6e75 6d29 2069 6620  f.verse_num) if 
+00005310: 4269 626c 6556 6572 7365 5061 7274 2e56  BibleVersePart.V
+00005320: 4552 5345 2069 6e20 7665 7273 655f 7061  ERSE in verse_pa
+00005330: 7274 7320 656c 7365 2022 220a 2020 2020  rts else "".    
+00005340: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
+00005350: 4269 626c 6556 6572 7365 5061 7274 2e43  BibleVersePart.C
+00005360: 4841 505f 5645 5253 4520 696e 2076 6572  HAP_VERSE in ver
+00005370: 7365 5f70 6172 7473 3a0a 2020 2020 2020  se_parts:.      
+00005380: 2020 2020 2020 7665 7273 655f 7365 7020        verse_sep 
+00005390: 3d20 6269 626c 655f 6461 7461 2829 2e76  = bible_data().v
+000053a0: 6572 7365 5f73 6570 5f61 6c74 2069 6620  erse_sep_alt if 
+000053b0: 616c 745f 7365 7020 656c 7365 2062 6962  alt_sep else bib
+000053c0: 6c65 5f64 6174 6128 292e 7665 7273 655f  le_data().verse_
+000053d0: 7365 705f 7374 640a 2020 2020 2020 2020  sep_std.        
+000053e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000053f0: 2020 7665 7273 655f 7365 7020 3d20 2222    verse_sep = ""
+00005400: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00005410: 203d 2066 227b 626f 6f6b 5f6e 616d 657d   = f"{book_name}
+00005420: 207b 6368 6170 5f73 7472 7d7b 7665 7273   {chap_str}{vers
+00005430: 655f 7365 707d 7b76 6572 7365 5f73 7472  e_sep}{verse_str
+00005440: 7d22 0a0a 2020 2020 2020 2020 6966 206e  }"..        if n
+00005450: 6f73 7061 6365 3a0a 2020 2020 2020 2020  ospace:.        
+00005460: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00005470: 742e 7265 706c 6163 6528 2220 222c 2022  t.replace(" ", "
+00005480: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00005490: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000054a0: 7572 6e20 7265 7375 6c74 2e73 7472 6970  urn result.strip
+000054b0: 2829 0a0a 0a40 6461 7461 636c 6173 7328  ()...@dataclass(
+000054c0: 696e 6974 3d46 616c 7365 2c20 7265 7072  init=False, repr
+000054d0: 3d46 616c 7365 2c20 6571 3d54 7275 652c  =False, eq=True,
+000054e0: 206f 7264 6572 3d54 7275 652c 2066 726f   order=True, fro
+000054f0: 7a65 6e3d 5472 7565 290a 636c 6173 7320  zen=True).class 
+00005500: 4269 626c 6552 616e 6765 3a0a 2020 2020  BibleRange:.    
+00005510: 2727 2741 2072 6566 6572 656e 6365 2074  '''A reference t
+00005520: 6f20 6120 636f 6e74 696e 756f 7573 2072  o a continuous r
+00005530: 616e 6765 206f 6620 4269 626c 6520 7665  ange of Bible ve
+00005540: 7273 6573 2028 652e 672e 204d 6174 7420  rses (e.g. Matt 
+00005550: 323a 332d 343a 3529 2e0a 0a20 2020 2043  2:3-4:5)...    C
+00005560: 6f6e 7461 696e 7320 3220 7072 696d 6172  ontains 2 primar
+00005570: 7920 6174 7472 6962 7574 6573 3a0a 2020  y attributes:.  
+00005580: 2020 202d 2060 7374 6172 7460 3a20 2054     - `start`:  T
+00005590: 6865 2066 6972 7374 2060 4269 626c 6556  he first `BibleV
+000055a0: 6572 7365 6020 696e 2074 6865 2072 616e  erse` in the ran
+000055b0: 6765 2028 696e 636c 7573 6976 6529 2e0a  ge (inclusive)..
+000055c0: 2020 2020 202d 2060 656e 6460 3a20 2020       - `end`:   
+000055d0: 2054 6865 206c 6173 7420 6042 6962 6c65   The last `Bible
+000055e0: 5665 7273 6560 2069 6e20 7468 6520 7261  Verse` in the ra
+000055f0: 6e67 6520 2869 6e63 6c75 7369 7665 292e  nge (inclusive).
+00005600: 0a20 2020 200a 2020 2020 4269 626c 6552  .    .    BibleR
+00005610: 616e 6765 7320 6172 6520 696d 6d75 7461  anges are immuta
+00005620: 626c 652e 2054 6865 7920 6361 6e20 6265  ble. They can be
+00005630: 2063 6f6d 7061 7265 6420 7573 696e 6720   compared using 
+00005640: 7468 6520 7374 616e 6461 7264 2063 6f6d  the standard com
+00005650: 7061 7269 736f 6e20 6f70 6572 6174 6f72  parison operator
+00005660: 732c 2077 6869 6368 2063 6f6d 7061 7265  s, which compare
+00005670: 2074 6865 0a20 2020 2060 7374 6172 7460   the.    `start`
+00005680: 2061 6e64 2060 656e 6460 2069 6e20 7468   and `end` in th
+00005690: 6174 206f 7264 6572 2e0a 0a20 2020 2049  at order...    I
+000056a0: 7465 7261 7469 6e67 206f 7665 7220 6120  terating over a 
+000056b0: 6042 6962 6c65 5261 6e67 6560 2072 6574  `BibleRange` ret
+000056c0: 7572 6e73 2065 6163 6820 6042 6962 6c65  urns each `Bible
+000056d0: 5665 7273 6560 2063 6f6e 7461 696e 6564  Verse` contained
+000056e0: 2077 6974 6869 6e20 7468 6520 7261 6e67   within the rang
+000056f0: 652e 0a20 2020 2027 2727 0a20 2020 2073  e..    '''.    s
+00005700: 7461 7274 3a20 4269 626c 6556 6572 7365  tart: BibleVerse
+00005710: 0a20 2020 2065 6e64 3a20 4269 626c 6556  .    end: BibleV
+00005720: 6572 7365 0a0a 2020 2020 4063 6c61 7373  erse..    @class
+00005730: 6d65 7468 6f64 0a20 2020 2064 6566 2077  method.    def w
+00005740: 686f 6c65 5f62 6962 6c65 2863 6c73 2c20  hole_bible(cls, 
+00005750: 666c 6167 733a 2042 6962 6c65 466c 6167  flags: BibleFlag
+00005760: 203d 204e 6f6e 6529 202d 3e20 2742 6962   = None) -> 'Bib
+00005770: 6c65 5261 6e67 6527 3a0a 2020 2020 2020  leRange':.      
+00005780: 2020 2727 2752 6574 7572 6e73 2061 2060    '''Returns a `
+00005790: 4269 626c 6552 616e 6765 6020 7265 7072  BibleRange` repr
+000057a0: 6573 656e 7469 6e67 2074 6865 2077 686f  esenting the who
+000057b0: 6c65 2042 6962 6c65 2e0a 2020 2020 2020  le Bible..      
+000057c0: 2020 2727 270a 2020 2020 2020 2020 666c    '''.        fl
+000057d0: 6167 7320 3d20 666c 6167 7320 6f72 2067  ags = flags or g
+000057e0: 6c6f 6261 6c73 2829 5b27 666c 6167 7327  lobals()['flags'
+000057f0: 5d20 6f72 2042 6962 6c65 466c 6167 2e4e  ] or BibleFlag.N
+00005800: 4f4e 450a 2020 2020 2020 2020 2320 4279  ONE.        # By
+00005810: 2064 6566 696e 6974 696f 6e2c 2077 6520   definition, we 
+00005820: 6e65 6564 2074 6f20 616c 6c6f 7720 6d75  need to allow mu
+00005830: 6c74 6962 6f6f 6b20 746f 2065 6e63 6f6d  ltibook to encom
+00005840: 7061 7373 2077 686f 6c65 2042 6962 6c65  pass whole Bible
+00005850: 0a20 2020 2020 2020 2066 6c61 6773 207c  .        flags |
+00005860: 3d20 4269 626c 6546 6c61 672e 4d55 4c54  = BibleFlag.MULT
+00005870: 4942 4f4f 4b0a 2020 2020 2020 2020 7374  IBOOK.        st
+00005880: 6172 745f 626f 6f6b 203d 2062 6962 6c65  art_book = bible
+00005890: 5f64 6174 6128 292e 626f 6f6b 5f6f 7264  _data().book_ord
+000058a0: 6572 5b30 5d0a 2020 2020 2020 2020 656e  er[0].        en
+000058b0: 645f 626f 6f6b 203d 2062 6962 6c65 5f64  d_book = bible_d
+000058c0: 6174 6128 292e 626f 6f6b 5f6f 7264 6572  ata().book_order
+000058d0: 5b6c 656e 2862 6962 6c65 5f64 6174 6128  [len(bible_data(
+000058e0: 292e 626f 6f6b 5f6f 7264 6572 292d 315d  ).book_order)-1]
+000058f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005900: 4269 626c 6552 616e 6765 2873 7461 7274  BibleRange(start
+00005910: 3d73 7461 7274 5f62 6f6f 6b2e 6669 7273  =start_book.firs
+00005920: 745f 7665 7273 6528 666c 6167 733d 666c  t_verse(flags=fl
+00005930: 6167 7329 2c0a 2020 2020 2020 2020 2020  ags),.          
 00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 2020 2020 2020 2063 6861 705f 6e75 6d20         chap_num 
-00005960: 3d20 626f 6f6b 2e6d 6178 5f63 6861 705f  = book.max_chap_
-00005970: 6e75 6d28 290a 2020 2020 2020 2020 2020  num().          
-00005980: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005990: 2020 2020 2020 2076 6572 7365 5f6e 756d         verse_num
-000059a0: 203d 2076 6572 7365 5f6e 756d 202b 2062   = verse_num + b
-000059b0: 6f6f 6b2e 6d61 785f 7665 7273 655f 6e75  ook.max_verse_nu
-000059c0: 6d28 6368 6170 5f6e 756d 2920 2d20 6d69  m(chap_num) - mi
-000059d0: 6e5f 7665 7273 655f 6e75 6d20 2b20 3120  n_verse_num + 1 
-000059e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059f0: 206d 696e 5f76 6572 7365 5f6e 756d 203d   min_verse_num =
-00005a00: 2062 6f6f 6b2e 6d69 6e5f 7665 7273 655f   book.min_verse_
-00005a10: 6e75 6d28 6368 6170 5f6e 756d 290a 2020  num(chap_num).  
-00005a20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005a30: 2042 6962 6c65 5665 7273 6528 626f 6f6b   BibleVerse(book
-00005a40: 2c20 6368 6170 5f6e 756d 2c20 7665 7273  , chap_num, vers
-00005a50: 655f 6e75 6d2c 2066 6c61 6773 3d66 6c61  e_num, flags=fla
-00005a60: 6773 290a 2020 2020 2020 2020 656c 6966  gs).        elif
-00005a70: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-00005a80: 722c 2042 6962 6c65 5665 7273 6529 3a0a  r, BibleVerse):.
-00005a90: 2020 2020 2020 2020 2020 2020 6269 626c              bibl
-00005aa0: 655f 7261 6e67 6520 3d20 4269 626c 6552  e_range = BibleR
-00005ab0: 616e 6765 2873 7461 7274 3d73 656c 662c  ange(start=self,
-00005ac0: 2065 6e64 3d6f 7468 6572 2920 2320 4269   end=other) # Bi
-00005ad0: 626c 6520 7769 6c6c 2073 7761 7020 7374  ble will swap st
-00005ae0: 6172 7420 616e 6420 656e 6420 6173 206e  art and end as n
-00005af0: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-00005b00: 2020 2020 2064 6966 6665 7265 6e63 6520       difference 
-00005b10: 3d20 6269 626c 655f 7261 6e67 652e 7665  = bible_range.ve
-00005b20: 7273 655f 636f 756e 7428 2920 2d20 310a  rse_count() - 1.
-00005b30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005b40: 656c 6620 3c20 6f74 6865 723a 0a20 2020  elf < other:.   
-00005b50: 2020 2020 2020 2020 2020 2020 2064 6966               dif
-00005b60: 6665 7265 6e63 6520 2a3d 202d 310a 2020  ference *= -1.  
-00005b70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005b80: 2064 6966 6665 7265 6e63 650a 2020 2020   difference.    
-00005b90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005ba0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00005bb0: 4572 726f 7228 6622 4361 6e6e 6f74 2073  Error(f"Cannot s
-00005bc0: 7562 7472 6163 7420 6120 7b74 7970 6528  ubtract a {type(
-00005bd0: 6f74 6865 7229 7d20 6672 6f6d 2061 2042  other)} from a B
-00005be0: 6962 6c65 5665 7273 6522 290a 0a20 2020  ibleVerse")..   
-00005bf0: 2064 6566 205f 5f61 6464 5f5f 2873 656c   def __add__(sel
-00005c00: 662c 206e 756d 5f76 6572 7365 733a 2069  f, num_verses: i
-00005c10: 6e74 2920 2d3e 2027 4269 626c 6556 6572  nt) -> 'BibleVer
-00005c20: 7365 273a 0a20 2020 2020 2020 2069 6620  se':.        if 
-00005c30: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
-00005c40: 756d 5f76 6572 7365 732c 2069 6e74 293a  um_verses, int):
-00005c50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005c60: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
-00005c70: 6564 0a20 2020 2020 2020 2072 6574 7572  ed.        retur
-00005c80: 6e20 7365 6c66 2e61 6464 286e 756d 5f76  n self.add(num_v
-00005c90: 6572 7365 7329 0a20 2020 200a 2020 2020  erses).    .    
-00005ca0: 6465 6620 5f5f 7375 625f 5f28 7365 6c66  def __sub__(self
-00005cb0: 2c20 6f74 6865 723a 2055 6e69 6f6e 5b69  , other: Union[i
-00005cc0: 6e74 2c20 2742 6962 6c65 5665 7273 6527  nt, 'BibleVerse'
-00005cd0: 5d29 202d 3e20 556e 696f 6e5b 696e 742c  ]) -> Union[int,
-00005ce0: 2027 4269 626c 6556 6572 7365 275d 3a0a   'BibleVerse']:.
-00005cf0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00005d00: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-00005d10: 2069 6e74 2920 616e 6420 6e6f 7420 6973   int) and not is
-00005d20: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
-00005d30: 4269 626c 6556 6572 7365 293a 0a20 2020  BibleVerse):.   
-00005d40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005d50: 4e6f 7449 6d70 6c65 6d65 6e74 6564 0a20  NotImplemented. 
-00005d60: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00005d70: 6c66 2e73 7562 7472 6163 7428 6f74 6865  lf.subtract(othe
-00005d80: 7229 0a0a 2020 2020 6465 6620 5f5f 7265  r)..    def __re
-00005d90: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00005da0: 2020 2020 7265 7475 726e 2066 2242 6962      return f"Bib
-00005db0: 6c65 5665 7273 6528 7b73 656c 662e 7374  leVerse({self.st
-00005dc0: 7228 6162 6272 6576 3d54 7275 6529 7d29  r(abbrev=True)})
-00005dd0: 220a 0a20 2020 2064 6566 205f 5f73 7472  "..    def __str
-00005de0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00005df0: 2020 7265 7475 726e 2073 656c 662e 7374    return self.st
-00005e00: 7228 290a 0a20 2020 2064 6566 2073 7472  r()..    def str
-00005e10: 2873 656c 662c 2061 6262 7265 763a 2062  (self, abbrev: b
-00005e20: 6f6f 6c20 3d20 4661 6c73 652c 2061 6c74  ool = False, alt
-00005e30: 5f73 6570 3a20 626f 6f6c 203d 2046 616c  _sep: bool = Fal
-00005e40: 7365 2c20 6e6f 7370 6163 653a 2062 6f6f  se, nospace: boo
-00005e50: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00005e60: 2020 2020 2020 2076 6572 7365 5f70 6172         verse_par
-00005e70: 7473 3a20 4269 626c 6556 6572 7365 5061  ts: BibleVersePa
-00005e80: 7274 203d 2042 6962 6c65 5665 7273 6550  rt = BibleVerseP
-00005e90: 6172 742e 4655 4c4c 5f52 4546 2920 2d3e  art.FULL_REF) ->
-00005ea0: 2073 7472 3a0a 2020 2020 2020 2020 2727   str:.        ''
-00005eb0: 2752 6574 7572 6e73 2061 2063 6f6e 6669  'Returns a confi
-00005ec0: 6775 7261 626c 6520 7374 7269 6e67 2072  gurable string r
-00005ed0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00005ee0: 2074 6869 7320 4269 626c 6556 6572 7365   this BibleVerse
-00005ef0: 2c20 6173 2066 6f6c 6c6f 7773 3a0a 0a20  , as follows:.. 
-00005f00: 2020 2020 2020 202d 2049 6620 6061 6262         - If `abb
-00005f10: 7265 7660 2069 7320 5472 7565 2c20 7468  rev` is True, th
-00005f20: 6520 6162 6272 6576 6961 7465 6420 6e61  e abbreviated na
-00005f30: 6d65 206f 6620 7468 6520 626f 6f6b 2069  me of the book i
-00005f40: 7320 7573 6564 2028 696e 7374 6561 6420  s used (instead 
-00005f50: 6f66 2074 6865 2066 756c 6c20 6e61 6d65  of the full name
-00005f60: 292e 0a20 2020 2020 2020 202d 2049 6620  )..        - If 
-00005f70: 6061 6c74 5f73 6570 6020 6973 2054 7275  `alt_sep` is Tru
-00005f80: 652c 2063 6861 7074 6572 2061 6e64 2076  e, chapter and v
-00005f90: 6572 7365 206e 756d 6265 7273 2061 7265  erse numbers are
-00005fa0: 2073 6570 6172 6174 6564 2062 7920 7468   separated by th
-00005fb0: 6520 616c 7465 726e 6174 650a 2020 2020  e alternate.    
-00005fc0: 2020 2020 2020 7365 7061 7261 746f 7220        separator 
-00005fd0: 2860 2e60 2062 7920 6465 6661 756c 7429  (`.` by default)
-00005fe0: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-00005ff0: 7374 616e 6461 7264 2073 6570 6172 6174  standard separat
-00006000: 6f72 2028 603a 6020 6279 2064 6566 6175  or (`:` by defau
-00006010: 6c74 292e 0a20 2020 2020 2020 202d 2049  lt)..        - I
-00006020: 6620 606e 6f73 7061 6365 6020 6973 2054  f `nospace` is T
-00006030: 7275 652c 206e 6f20 7370 6163 6573 2061  rue, no spaces a
-00006040: 7265 2069 6e63 6c75 6465 6420 696e 2074  re included in t
-00006050: 6865 2073 7472 696e 672e 0a20 2020 2020  he string..     
-00006060: 2020 202d 2060 7665 7273 655f 7061 7274     - `verse_part
-00006070: 7360 2069 7320 6120 636f 6d62 696e 6174  s` is a combinat
-00006080: 696f 6e20 6f66 2060 4269 626c 6556 6572  ion of `BibleVer
-00006090: 7365 5061 7274 6020 666c 6167 732c 2063  sePart` flags, c
-000060a0: 6f6e 7472 6f6c 6c69 6e67 2077 6861 7420  ontrolling what 
-000060b0: 636f 6d62 696e 6174 696f 6e20 6f66 2062  combination of b
-000060c0: 6f6f 6b2c 0a20 2020 2020 2020 2020 2063  ook,.          c
-000060d0: 6861 7074 6572 2026 2076 6572 7365 2061  hapter & verse a
-000060e0: 7265 2064 6973 706c 6179 6564 2e0a 2020  re displayed..  
-000060f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00006100: 2020 6966 2073 656c 662e 626f 6f6b 2e63    if self.book.c
-00006110: 6861 705f 636f 756e 7428 2920 3d3d 2031  hap_count() == 1
-00006120: 3a0a 2020 2020 2020 2020 2020 2020 7665  :.            ve
-00006130: 7273 655f 7061 7274 7320 263d 207e 4269  rse_parts &= ~Bi
-00006140: 626c 6556 6572 7365 5061 7274 2e43 4841  bleVersePart.CHA
-00006150: 5020 2320 446f 6e27 7420 6469 7370 6c61  P # Don't displa
-00006160: 7920 6368 6170 0a20 2020 2020 2020 200a  y chap.        .
-00006170: 2020 2020 2020 2020 6966 2042 6962 6c65          if Bible
-00006180: 5665 7273 6550 6172 742e 424f 4f4b 2069  VersePart.BOOK i
-00006190: 6e20 7665 7273 655f 7061 7274 733a 0a20  n verse_parts:. 
-000061a0: 2020 2020 2020 2020 2020 2062 6f6f 6b5f             book_
-000061b0: 6e61 6d65 203d 2073 656c 662e 626f 6f6b  name = self.book
-000061c0: 2e61 6262 7265 7620 6966 2061 6262 7265  .abbrev if abbre
-000061d0: 7620 656c 7365 2073 656c 662e 626f 6f6b  v else self.book
-000061e0: 2e74 6974 6c65 0a20 2020 2020 2020 2065  .title.        e
-000061f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00006200: 2062 6f6f 6b5f 6e61 6d65 203d 2022 220a   book_name = "".
-00006210: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006220: 2063 6861 705f 7374 7220 3d20 7374 7228   chap_str = str(
-00006230: 7365 6c66 2e63 6861 705f 6e75 6d29 2069  self.chap_num) i
-00006240: 6620 4269 626c 6556 6572 7365 5061 7274  f BibleVersePart
-00006250: 2e43 4841 5020 696e 2076 6572 7365 5f70  .CHAP in verse_p
-00006260: 6172 7473 2065 6c73 6520 2222 0a20 2020  arts else "".   
-00006270: 2020 2020 2076 6572 7365 5f73 7472 203d       verse_str =
-00006280: 2073 7472 2873 656c 662e 7665 7273 655f   str(self.verse_
-00006290: 6e75 6d29 2069 6620 4269 626c 6556 6572  num) if BibleVer
-000062a0: 7365 5061 7274 2e56 4552 5345 2069 6e20  sePart.VERSE in 
-000062b0: 7665 7273 655f 7061 7274 7320 656c 7365  verse_parts else
-000062c0: 2022 220a 2020 2020 2020 2020 0a20 2020   "".        .   
-000062d0: 2020 2020 2069 6620 4269 626c 6556 6572       if BibleVer
-000062e0: 7365 5061 7274 2e43 4841 505f 5645 5253  sePart.CHAP_VERS
-000062f0: 4520 696e 2076 6572 7365 5f70 6172 7473  E in verse_parts
-00006300: 3a0a 2020 2020 2020 2020 2020 2020 7665  :.            ve
-00006310: 7273 655f 7365 7020 3d20 6269 626c 655f  rse_sep = bible_
-00006320: 6461 7461 2829 2e76 6572 7365 5f73 6570  data().verse_sep
-00006330: 5f61 6c74 2069 6620 616c 745f 7365 7020  _alt if alt_sep 
-00006340: 656c 7365 2062 6962 6c65 5f64 6174 6128  else bible_data(
-00006350: 292e 7665 7273 655f 7365 705f 7374 640a  ).verse_sep_std.
-00006360: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006370: 2020 2020 2020 2020 2020 7665 7273 655f            verse_
-00006380: 7365 7020 3d20 2222 0a0a 2020 2020 2020  sep = ""..      
-00006390: 2020 7265 7375 6c74 203d 2066 227b 626f    result = f"{bo
-000063a0: 6f6b 5f6e 616d 657d 207b 6368 6170 5f73  ok_name} {chap_s
-000063b0: 7472 7d7b 7665 7273 655f 7365 707d 7b76  tr}{verse_sep}{v
-000063c0: 6572 7365 5f73 7472 7d22 0a0a 2020 2020  erse_str}"..    
-000063d0: 2020 2020 6966 206e 6f73 7061 6365 3a0a      if nospace:.
-000063e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000063f0: 726e 2072 6573 756c 742e 7265 706c 6163  rn result.replac
-00006400: 6528 2220 222c 2022 2229 0a20 2020 2020  e(" ", "").     
-00006410: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00006420: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00006430: 6c74 2e73 7472 6970 2829 0a0a 0a40 6461  lt.strip()...@da
-00006440: 7461 636c 6173 7328 696e 6974 3d46 616c  taclass(init=Fal
-00006450: 7365 2c20 7265 7072 3d46 616c 7365 2c20  se, repr=False, 
-00006460: 6571 3d54 7275 652c 206f 7264 6572 3d54  eq=True, order=T
-00006470: 7275 652c 2066 726f 7a65 6e3d 5472 7565  rue, frozen=True
-00006480: 290a 636c 6173 7320 4269 626c 6552 616e  ).class BibleRan
-00006490: 6765 3a0a 2020 2020 2727 2741 2072 6566  ge:.    '''A ref
-000064a0: 6572 656e 6365 2074 6f20 6120 636f 6e74  erence to a cont
-000064b0: 696e 756f 7573 2072 616e 6765 206f 6620  inuous range of 
-000064c0: 4269 626c 6520 7665 7273 6573 2028 652e  Bible verses (e.
-000064d0: 672e 204d 6174 7420 323a 332d 343a 3529  g. Matt 2:3-4:5)
-000064e0: 2e0a 0a20 2020 2043 6f6e 7461 696e 7320  ...    Contains 
-000064f0: 3220 7072 696d 6172 7920 6174 7472 6962  2 primary attrib
-00006500: 7574 6573 3a0a 2020 2020 202d 2060 7374  utes:.     - `st
-00006510: 6172 7460 3a20 2054 6865 2066 6972 7374  art`:  The first
-00006520: 2060 4269 626c 6556 6572 7365 6020 696e   `BibleVerse` in
-00006530: 2074 6865 2072 616e 6765 2028 696e 636c   the range (incl
-00006540: 7573 6976 6529 2e0a 2020 2020 202d 2060  usive)..     - `
-00006550: 656e 6460 3a20 2020 2054 6865 206c 6173  end`:    The las
-00006560: 7420 6042 6962 6c65 5665 7273 6560 2069  t `BibleVerse` i
-00006570: 6e20 7468 6520 7261 6e67 6520 2869 6e63  n the range (inc
-00006580: 6c75 7369 7665 292e 0a20 2020 200a 2020  lusive)..    .  
-00006590: 2020 4269 626c 6552 616e 6765 7320 6172    BibleRanges ar
-000065a0: 6520 696d 6d75 7461 626c 652e 2054 6865  e immutable. The
-000065b0: 7920 6361 6e20 6265 2063 6f6d 7061 7265  y can be compare
-000065c0: 6420 7573 696e 6720 7468 6520 7374 616e  d using the stan
-000065d0: 6461 7264 2063 6f6d 7061 7269 736f 6e20  dard comparison 
-000065e0: 6f70 6572 6174 6f72 732c 2077 6869 6368  operators, which
-000065f0: 2063 6f6d 7061 7265 2074 6865 0a20 2020   compare the.   
-00006600: 2060 7374 6172 7460 2061 6e64 2060 656e   `start` and `en
-00006610: 6460 2069 6e20 7468 6174 206f 7264 6572  d` in that order
-00006620: 2e0a 0a20 2020 2049 7465 7261 7469 6e67  ...    Iterating
-00006630: 206f 7665 7220 6120 6042 6962 6c65 5261   over a `BibleRa
-00006640: 6e67 6560 2072 6574 7572 6e73 2065 6163  nge` returns eac
-00006650: 6820 6042 6962 6c65 5665 7273 6560 2063  h `BibleVerse` c
-00006660: 6f6e 7461 696e 6564 2077 6974 6869 6e20  ontained within 
-00006670: 7468 6520 7261 6e67 652e 0a20 2020 2027  the range..    '
-00006680: 2727 0a20 2020 2073 7461 7274 3a20 4269  ''.    start: Bi
-00006690: 626c 6556 6572 7365 0a20 2020 2065 6e64  bleVerse.    end
-000066a0: 3a20 4269 626c 6556 6572 7365 0a0a 2020  : BibleVerse..  
-000066b0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000066c0: 2020 2064 6566 2077 686f 6c65 5f62 6962     def whole_bib
-000066d0: 6c65 2863 6c73 2c20 666c 6167 733a 2042  le(cls, flags: B
-000066e0: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-000066f0: 202d 3e20 2742 6962 6c65 5261 6e67 6527   -> 'BibleRange'
-00006700: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
-00006710: 7572 6e73 2061 2060 4269 626c 6552 616e  urns a `BibleRan
-00006720: 6765 6020 7265 7072 6573 656e 7469 6e67  ge` representing
-00006730: 2074 6865 2077 686f 6c65 2042 6962 6c65   the whole Bible
-00006740: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00006750: 2020 2020 2020 666c 6167 7320 3d20 666c        flags = fl
-00006760: 6167 7320 6f72 2062 6962 6c65 7265 662e  ags or bibleref.
-00006770: 666c 6167 7320 6f72 2042 6962 6c65 466c  flags or BibleFl
-00006780: 6167 2e4e 4f4e 450a 2020 2020 2020 2020  ag.NONE.        
-00006790: 2320 4279 2064 6566 696e 6974 696f 6e2c  # By definition,
-000067a0: 2077 6520 6e65 6564 2074 6f20 616c 6c6f   we need to allo
-000067b0: 7720 6d75 6c74 6962 6f6f 6b20 746f 2065  w multibook to e
-000067c0: 6e63 6f6d 7061 7373 2077 686f 6c65 2042  ncompass whole B
-000067d0: 6962 6c65 0a20 2020 2020 2020 2066 6c61  ible.        fla
-000067e0: 6773 207c 3d20 4269 626c 6546 6c61 672e  gs |= BibleFlag.
-000067f0: 4d55 4c54 4942 4f4f 4b0a 2020 2020 2020  MULTIBOOK.      
-00006800: 2020 7374 6172 745f 626f 6f6b 203d 2062    start_book = b
-00006810: 6962 6c65 5f64 6174 6128 292e 626f 6f6b  ible_data().book
-00006820: 5f6f 7264 6572 5b30 5d0a 2020 2020 2020  _order[0].      
-00006830: 2020 656e 645f 626f 6f6b 203d 2062 6962    end_book = bib
-00006840: 6c65 5f64 6174 6128 292e 626f 6f6b 5f6f  le_data().book_o
-00006850: 7264 6572 5b6c 656e 2862 6962 6c65 5f64  rder[len(bible_d
-00006860: 6174 6128 292e 626f 6f6b 5f6f 7264 6572  ata().book_order
-00006870: 292d 315d 0a20 2020 2020 2020 2072 6574  )-1].        ret
-00006880: 7572 6e20 4269 626c 6552 616e 6765 2873  urn BibleRange(s
-00006890: 7461 7274 3d73 7461 7274 5f62 6f6f 6b2e  tart=start_book.
-000068a0: 6669 7273 745f 7665 7273 6528 666c 6167  first_verse(flag
-000068b0: 733d 666c 6167 7329 2c0a 2020 2020 2020  s=flags),.      
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 656e 643d 656e 645f 626f 6f6b      end=end_book
-000068e0: 2e6c 6173 745f 7665 7273 6528 292c 2066  .last_verse(), f
-000068f0: 6c61 6773 3d66 6c61 6773 290a 0a20 2020  lags=flags)..   
-00006900: 2023 2054 4f44 4f3a 2043 6f6e 7369 6465   # TODO: Conside
-00006910: 7220 616c 6c6f 7769 6e67 2061 2062 6f6f  r allowing a boo
-00006920: 6b20 616e 6420 7665 7273 652c 2077 6974  k and verse, wit
-00006930: 686f 7574 2061 2063 6861 7074 6572 2e20  hout a chapter. 
-00006940: 4173 7375 6d65 2066 6972 7374 206f 7220  Assume first or 
-00006950: 6c61 7374 2063 6861 7074 6572 2061 7320  last chapter as 
-00006960: 6e65 6365 7373 6172 792e 0a20 2020 2064  necessary..    d
-00006970: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00006980: 2c20 2a61 7267 732c 2073 7461 7274 3a20  , *args, start: 
-00006990: 4269 626c 6556 6572 7365 203d 204e 6f6e  BibleVerse = Non
-000069a0: 652c 2065 6e64 3a20 4269 626c 6556 6572  e, end: BibleVer
-000069b0: 7365 203d 204e 6f6e 652c 0a20 2020 2020  se = None,.     
-000069c0: 2020 2020 2020 2020 2020 2020 666c 6167              flag
-000069d0: 733a 2042 6962 6c65 466c 6167 203d 204e  s: BibleFlag = N
-000069e0: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
-000069f0: 2741 2060 4269 626c 6552 616e 6765 6020  'A `BibleRange` 
-00006a00: 6361 6e20 6265 2063 6f6e 7374 7275 6374  can be construct
-00006a10: 6564 2069 6e20 616e 7920 6f66 2074 6865  ed in any of the
-00006a20: 2066 6f6c 6c6f 7769 6e67 2077 6179 733a   following ways:
-00006a30: 0a0a 2020 2020 2020 2020 312e 2046 726f  ..        1. Fro
-00006a40: 6d20 6120 7369 6e67 6c65 2073 7472 696e  m a single strin
-00006a50: 673a 2060 4269 626c 6552 616e 6765 2822  g: `BibleRange("
-00006a60: 4d61 726b 2033 3a31 2d34 3a32 2229 600a  Mark 3:1-4:2")`.
-00006a70: 0a20 2020 2020 2020 2020 2020 5261 6973  .           Rais
-00006a80: 6573 2061 2060 4269 626c 6552 6566 5061  es a `BibleRefPa
-00006a90: 7273 696e 6745 7272 6f72 6020 6966 2074  rsingError` if t
-00006aa0: 6865 2073 7472 696e 6720 6361 6e6e 6f74  he string cannot
-00006ab0: 2062 6520 7061 7273 6564 2e0a 0a20 2020   be parsed...   
-00006ac0: 2020 2020 2032 2e20 4672 6f6d 2061 2073       2. From a s
-00006ad0: 7461 7274 2061 6e64 2065 6e64 2060 4269  tart and end `Bi
-00006ae0: 626c 6556 6572 7365 602c 2077 6869 6368  bleVerse`, which
-00006af0: 206d 7573 7420 6265 2073 7065 6369 6669   must be specifi
-00006b00: 6564 2075 7369 6e67 2074 6865 206b 6579  ed using the key
-00006b10: 776f 7264 2061 7267 756d 656e 7473 0a20  word arguments. 
-00006b20: 2020 2020 2020 2020 2020 6073 7461 7274            `start
-00006b30: 6020 616e 6420 6065 6e64 603a 2060 4269  ` and `end`: `Bi
-00006b40: 626c 6552 616e 6765 2873 7461 7274 3d42  bleRange(start=B
-00006b50: 6962 6c65 5665 7273 6528 224d 6172 6b20  ibleVerse("Mark 
-00006b60: 333a 3122 292c 2065 6e64 3d42 6962 6c65  3:1"), end=Bible
-00006b70: 5665 7273 6528 224d 6172 6b20 343a 3222  Verse("Mark 4:2"
-00006b80: 2929 600a 0a20 2020 2020 2020 2033 2e20  ))`..        3. 
-00006b90: 4173 2061 2063 6f70 7920 6f66 2061 6e20  As a copy of an 
-00006ba0: 6578 6973 7469 6e67 2042 6962 6c65 5261  existing BibleRa
-00006bb0: 6e67 653a 2060 4269 626c 6552 616e 6765  nge: `BibleRange
-00006bc0: 2865 7869 7374 696e 675f 6269 626c 655f  (existing_bible_
-00006bd0: 7261 6e67 6529 600a 0a20 2020 2020 2020  range)`..       
-00006be0: 2034 2e20 4672 6f6d 2070 6f73 6974 696f   4. From positio
-00006bf0: 6e61 6c20 6172 6775 6d65 6e74 7320 696e  nal arguments in
-00006c00: 2074 6865 2066 6f6c 6c6f 7769 6e67 206f   the following o
-00006c10: 7264 6572 3a0a 2020 2020 2020 2020 2020  rder:.          
-00006c20: 2053 7461 7274 2062 6f6f 6b2c 2073 7461   Start book, sta
-00006c30: 7274 2060 6368 6170 5f6e 756d 602c 2073  rt `chap_num`, s
-00006c40: 7461 7274 2060 7665 7273 655f 6e75 6d60  tart `verse_num`
-00006c50: 2c20 656e 6420 626f 6f6b 2c20 656e 6420  , end book, end 
-00006c60: 6063 6861 705f 6e75 6d60 2c20 656e 6420  `chap_num`, end 
-00006c70: 6076 6572 7365 5f6e 756d 602e 0a20 2020  `verse_num`..   
-00006c80: 2020 2020 2020 2020 5374 6172 7420 616e          Start an
-00006c90: 6420 656e 6420 626f 6f6b 7320 6361 6e20  d end books can 
-00006ca0: 6265 2073 7472 696e 6720 6e61 6d65 7320  be string names 
-00006cb0: 6f72 2060 4269 626c 6542 6f6f 6b60 2065  or `BibleBook` e
-00006cc0: 6e75 6d73 2e0a 2020 2020 2020 2020 2020  nums..          
-00006cd0: 204c 6174 6572 2061 7267 756d 656e 7473   Later arguments
-00006ce0: 2063 616e 2062 6520 6f6d 6974 7465 6420   can be omitted 
-00006cf0: 6f72 2073 6574 2074 6f20 604e 6f6e 6560  or set to `None`
-00006d00: 2c20 6173 2069 6e20 7468 6573 6520 6578  , as in these ex
-00006d10: 616d 706c 6573 3a0a 0a20 2020 2020 2020  amples:..       
-00006d20: 2020 2020 6042 6962 6c65 5261 6e67 6528      `BibleRange(
-00006d30: 4269 626c 6542 6f6f 6b2e 4d61 7474 2c20  BibleBook.Matt, 
-00006d40: 322c 2033 2c20 4269 626c 6542 6f6f 6b2e  2, 3, BibleBook.
-00006d50: 4a6f 686e 2c20 342c 2036 2c20 666c 6167  John, 4, 6, flag
-00006d60: 733d 4269 626c 6546 6c61 672e 4d55 4c54  s=BibleFlag.MULT
-00006d70: 4942 4f4f 4b29 2023 204d 6174 7420 323a  IBOOK) # Matt 2:
-00006d80: 332d 4a6f 686e 2034 3a36 600a 2020 2020  3-John 4:6`.    
-00006d90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006da0: 2020 2060 4269 626c 6552 616e 6765 2842     `BibleRange(B
-00006db0: 6962 6c65 426f 6f6b 2e4d 6174 7429 2023  ibleBook.Matt) #
-00006dc0: 2045 6e74 6972 6520 626f 6f6b 3a20 4d61   Entire book: Ma
-00006dd0: 7474 2031 3a31 2d32 383a 3230 600a 2020  tt 1:1-28:20`.  
-00006de0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00006df0: 2020 2020 2060 4269 626c 6552 616e 6765       `BibleRange
-00006e00: 2842 6962 6c65 426f 6f6b 2e4d 6174 742c  (BibleBook.Matt,
-00006e10: 2032 2920 2320 456e 7469 7265 2063 6861   2) # Entire cha
-00006e20: 7074 6572 3a20 4d61 7474 2032 3a31 2d32  pter: Matt 2:1-2
-00006e30: 3360 0a20 2020 2020 2020 2020 2020 0a20  3`.           . 
-00006e40: 2020 2020 2020 2020 2020 6042 6962 6c65            `Bible
-00006e50: 5261 6e67 6528 4269 626c 6542 6f6f 6b2e  Range(BibleBook.
-00006e60: 4d61 7474 2c20 322c 2033 2920 2320 5369  Matt, 2, 3) # Si
-00006e70: 6e67 6c65 2076 6572 7365 3a20 4d61 7474  ngle verse: Matt
-00006e80: 2032 3a33 600a 2020 2020 2020 2020 2020   2:3`.          
-00006e90: 200a 2020 2020 2020 2020 2020 2060 4269   .           `Bi
-00006ea0: 626c 6552 616e 6765 2842 6962 6c65 426f  bleRange(BibleBo
-00006eb0: 6f6b 2e4d 6174 742c 204e 6f6e 652c 204e  ok.Matt, None, N
-00006ec0: 6f6e 652c 2042 6962 6c65 426f 6f6b 2e4a  one, BibleBook.J
-00006ed0: 6f68 6e2c 2066 6c61 6773 3d42 6962 6c65  ohn, flags=Bible
-00006ee0: 466c 6167 2e4d 554c 5449 424f 4f4b 2920  Flag.MULTIBOOK) 
-00006ef0: 2320 4d61 7474 2031 3a31 2d4a 6f68 6e20  # Matt 1:1-John 
-00006f00: 3231 3a32 3560 0a20 2020 2020 2020 2020  21:25`.         
-00006f10: 2020 0a20 2020 2020 2020 2020 2020 6042    .           `B
-00006f20: 6962 6c65 5261 6e67 6528 4269 626c 6542  ibleRange(BibleB
-00006f30: 6f6f 6b2e 4d61 7474 2c20 4e6f 6e65 2c20  ook.Matt, None, 
-00006f40: 4e6f 6e65 2c20 4e6f 6e65 2c20 3429 2023  None, None, 4) #
-00006f50: 204d 6174 7420 313a 312d 343a 3235 600a   Matt 1:1-4:25`.
-00006f60: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00006f70: 2020 2020 2020 2060 4269 626c 6552 616e         `BibleRan
-00006f80: 6765 2842 6962 6c65 426f 6f6b 2e4d 6174  ge(BibleBook.Mat
-00006f90: 742c 204e 6f6e 652c 204e 6f6e 652c 204e  t, None, None, N
-00006fa0: 6f6e 652c 204e 6f6e 652c 2036 2920 2320  one, None, 6) # 
-00006fb0: 4d61 7474 2031 3a31 2d31 3a36 600a 2020  Matt 1:1-1:6`.  
-00006fc0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00006fd0: 2020 2020 2060 4269 626c 6552 616e 6765       `BibleRange
-00006fe0: 2842 6962 6c65 426f 6f6b 2e4d 6174 742c  (BibleBook.Matt,
-00006ff0: 2032 2c20 332c 204e 6f6e 652c 2034 2c20   2, 3, None, 4, 
-00007000: 3629 2023 204d 6174 7420 323a 332d 343a  6) # Matt 2:3-4:
-00007010: 3660 0a0a 2020 2020 2020 2049 6620 7468  6`..       If th
-00007020: 6520 7374 6172 7420 7665 7273 6520 6973  e start verse is
-00007030: 206f 6276 696f 7573 6c79 2067 7265 6174   obviously great
-00007040: 6572 2074 6861 6e20 7468 6520 656e 6420  er than the end 
-00007050: 7665 7273 652c 2074 6865 7920 6172 6520  verse, they are 
-00007060: 7377 6170 7065 6420 6172 6f75 6e64 2e0a  swapped around..
-00007070: 2020 2020 2020 2020 4e6f 7465 2074 6861          Note tha
-00007080: 7420 6974 2069 7320 736f 6d65 7469 6d65  t it is sometime
-00007090: 7320 6e6f 7420 706f 7373 6962 6c65 2074  s not possible t
-000070a0: 6f20 6469 7374 696e 6775 6973 6820 6120  o distinguish a 
-000070b0: 7377 6170 7065 6420 7374 6172 7420 616e  swapped start an
-000070c0: 6420 656e 6420 6672 6f6d 0a20 2020 2020  d end from.     
-000070d0: 2020 206d 6973 666f 726d 6564 2061 7267     misformed arg
-000070e0: 756d 656e 7473 2e0a 0a20 2020 2020 2020  uments...       
-000070f0: 2049 6620 7468 6520 7375 7070 6c69 6564   If the supplied
-00007100: 2061 7267 756d 656e 7473 2061 7265 206e   arguments are n
-00007110: 6f74 2061 2076 616c 6964 2076 6572 7365  ot a valid verse
-00007120: 2c20 616e 2060 496e 7661 6c69 6452 6566  , an `InvalidRef
-00007130: 6572 656e 6365 4572 726f 7260 2069 7320  erenceError` is 
-00007140: 7261 6973 6564 2e0a 2020 2020 2020 2020  raised..        
-00007150: 4966 2074 6865 2073 7461 7274 2061 6e64  If the start and
-00007160: 2065 6e64 2076 6572 7365 7320 6172 6520   end verses are 
-00007170: 6672 6f6d 2064 6966 6665 7265 6e74 2060  from different `
-00007180: 4269 626c 6542 6f6f 6b73 6020 616e 6420  BibleBooks` and 
-00007190: 6042 6962 6c65 466c 6167 2e4d 554c 5449  `BibleFlag.MULTI
-000071a0: 424f 4f4b 6020 6973 206e 6f74 2073 6574  BOOK` is not set
-000071b0: 2067 6c6f 6261 6c6c 790a 2020 2020 2020   globally.      
-000071c0: 2020 6f72 2075 7369 6e67 2074 6865 2060    or using the `
-000071d0: 666c 6167 7360 2061 7267 756d 656e 742c  flags` argument,
-000071e0: 2061 2060 4d75 6c74 6962 6f6f 6b52 616e   a `MultibookRan
-000071f0: 6765 4e6f 7441 6c6c 6f77 6564 4572 726f  geNotAllowedErro
-00007200: 7260 2069 7320 7261 6973 6564 2e20 4966  r` is raised. If
-00007210: 2074 6865 2061 7267 756d 656e 7473 2061   the arguments a
-00007220: 7265 206f 6620 616e 0a20 2020 2020 2020  re of an.       
-00007230: 2069 6e63 6f72 7265 6374 206e 756d 6265   incorrect numbe
-00007240: 7220 6f72 2074 7970 652c 2061 2060 5661  r or type, a `Va
-00007250: 6c75 6545 7272 6f72 6020 6973 2072 6169  lueError` is rai
-00007260: 7365 642e 2020 2020 200a 2020 2020 2020  sed.     .      
-00007270: 2020 2727 270a 2020 2020 2020 2020 666c    '''.        fl
-00007280: 6167 7320 3d20 666c 6167 7320 6f72 2062  ags = flags or b
-00007290: 6962 6c65 7265 662e 666c 6167 7320 6f72  ibleref.flags or
-000072a0: 2042 6962 6c65 466c 6167 2e4e 4f4e 450a   BibleFlag.NONE.
-000072b0: 2020 2020 2020 2020 6966 206c 656e 2861          if len(a
-000072c0: 7267 7329 203d 3d20 303a 0a20 2020 2020  rgs) == 0:.     
-000072d0: 2020 2020 2020 2069 6620 4269 626c 6546         if BibleF
-000072e0: 6c61 672e 4d55 4c54 4942 4f4f 4b20 6e6f  lag.MULTIBOOK no
-000072f0: 7420 696e 2066 6c61 6773 2061 6e64 2073  t in flags and s
-00007300: 7461 7274 2e62 6f6f 6b20 213d 2065 6e64  tart.book != end
-00007310: 2e62 6f6f 6b3a 0a20 2020 2020 2020 2020  .book:.         
-00007320: 2020 2020 2020 2072 6169 7365 204d 756c         raise Mul
-00007330: 7469 626f 6f6b 5261 6e67 654e 6f74 416c  tibookRangeNotAl
-00007340: 6c6f 7765 6445 7272 6f72 2866 224d 756c  lowedError(f"Mul
-00007350: 7469 2d62 6f6f 6b20 7261 6e67 6573 206e  ti-book ranges n
-00007360: 6f74 2061 6c6c 6f77 6564 2022 202b 200a  ot allowed " + .
-00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 2020 6622 287b 7374 6172 742e 626f      f"({start.bo
-000073b0: 6f6b 2e61 6262 7265 767d 2061 6e64 207b  ok.abbrev} and {
-000073c0: 656e 642e 626f 6f6b 2e61 6262 7265 767d  end.book.abbrev}
-000073d0: 2061 7265 2064 6966 6665 7265 6e74 2922   are different)"
-000073e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000073f0: 2073 7461 7274 203e 2065 6e64 3a0a 2020   start > end:.  
-00007400: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-00007410: 7461 7274 2c20 656e 6429 203d 2028 656e  tart, end) = (en
-00007420: 642c 2073 7461 7274 290a 2020 2020 2020  d, start).      
-00007430: 2020 2020 2020 6f62 6a65 6374 2e5f 5f73        object.__s
-00007440: 6574 6174 7472 5f5f 2873 656c 662c 2022  etattr__(self, "
-00007450: 7374 6172 7422 2c20 7374 6172 7429 0a20  start", start). 
-00007460: 2020 2020 2020 2020 2020 206f 626a 6563             objec
-00007470: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
-00007480: 6c66 2c20 2265 6e64 222c 2065 6e64 290a  lf, "end", end).
-00007490: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000074a0: 726e 0a20 2020 2020 2020 2065 6c69 6620  rn.        elif 
-000074b0: 6c65 6e28 6172 6773 2920 3e20 363a 0a20  len(args) > 6:. 
-000074c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000074d0: 2056 616c 7565 4572 726f 7228 2254 6f6f   ValueError("Too
-000074e0: 206d 616e 7920 6172 6775 6d65 6e74 7320   many arguments 
-000074f0: 7375 7070 6c69 6564 2074 6f20 4269 626c  supplied to Bibl
-00007500: 6552 616e 6765 2229 0a20 2020 2020 2020  eRange").       
-00007510: 2069 6620 6c65 6e28 6172 6773 2920 3d3d   if len(args) ==
-00007520: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00007530: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
-00007540: 6773 5b30 5d2c 2073 7472 293a 0a20 2020  gs[0], str):.   
-00007550: 2020 2020 2020 2020 2020 2020 2072 616e               ran
-00007560: 6765 5f6c 6973 7420 3d20 4269 626c 6552  ge_list = BibleR
-00007570: 616e 6765 4c69 7374 2861 7267 735b 305d  angeList(args[0]
-00007580: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
-00007590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000075a0: 6620 6c65 6e28 7261 6e67 655f 6c69 7374  f len(range_list
-000075b0: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
-000075c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000075d0: 6520 496e 7661 6c69 6452 6566 6572 656e  e InvalidReferen
-000075e0: 6365 4572 726f 7228 6622 5374 7269 6e67  ceError(f"String
-000075f0: 2069 7320 6e6f 7420 6120 7369 6e67 6c65   is not a single
-00007600: 2076 6572 7365 2072 616e 6765 3a20 7b61   verse range: {a
-00007610: 7267 735b 305d 7d22 290a 2020 2020 2020  rgs[0]}").      
-00007620: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-00007630: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
-00007640: 662c 2022 7374 6172 7422 2c20 7261 6e67  f, "start", rang
-00007650: 655f 6c69 7374 5b30 5d2e 7374 6172 7429  e_list[0].start)
-00007660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007670: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
-00007680: 725f 5f28 7365 6c66 2c20 2265 6e64 222c  r__(self, "end",
-00007690: 2072 616e 6765 5f6c 6973 745b 305d 2e65   range_list[0].e
-000076a0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-000076b0: 2020 2020 7265 7475 726e 2020 2020 2020      return      
-000076c0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000076d0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-000076e0: 7374 616e 6365 2861 7267 735b 305d 2c20  stance(args[0], 
-000076f0: 4269 626c 6552 616e 6765 293a 0a20 2020  BibleRange):.   
-00007700: 2020 2020 2020 2020 2020 2020 206f 626a               obj
-00007710: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
-00007720: 7365 6c66 2c20 2273 7461 7274 222c 2061  self, "start", a
-00007730: 7267 735b 305d 2e73 7461 7274 290a 2020  rgs[0].start).  
-00007740: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
-00007750: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
-00007760: 2873 656c 662c 2022 656e 6422 2c20 6172  (self, "end", ar
-00007770: 6773 5b30 5d2e 656e 6429 0a20 2020 2020  gs[0].end).     
-00007780: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007790: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
-000077a0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-000077b0: 6528 6172 6773 5b30 5d2c 2042 6962 6c65  e(args[0], Bible
-000077c0: 426f 6f6b 293a 0a20 2020 2020 2020 2020  Book):.         
-000077d0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000077e0: 7565 4572 726f 7228 2253 696e 676c 6520  ueError("Single 
-000077f0: 6172 6775 6d65 6e74 2074 6f20 4269 626c  argument to Bibl
-00007800: 6552 616e 6765 2063 616e 206f 6e6c 7920  eRange can only 
-00007810: 6265 2061 2073 7472 696e 672c 2042 6962  be a string, Bib
-00007820: 6c65 426f 6f6b 206f 7220 616e 6f74 6865  leBook or anothe
-00007830: 7220 4269 626c 6552 616e 6765 2229 0a0a  r BibleRange")..
-00007840: 2020 2020 2020 2020 7374 6172 745f 626f          start_bo
-00007850: 6f6b 203d 2061 7267 735b 305d 0a20 2020  ok = args[0].   
-00007860: 2020 2020 2073 7461 7274 5f63 6861 7020       start_chap 
-00007870: 3d20 6172 6773 5b31 5d20 6966 206c 656e  = args[1] if len
-00007880: 2861 7267 7329 203e 2031 2065 6c73 6520  (args) > 1 else 
-00007890: 4e6f 6e65 0a20 2020 2020 2020 2073 7461  None.        sta
-000078a0: 7274 5f76 6572 7365 203d 2061 7267 735b  rt_verse = args[
-000078b0: 325d 2069 6620 6c65 6e28 6172 6773 2920  2] if len(args) 
-000078c0: 3e20 3220 656c 7365 204e 6f6e 650a 2020  > 2 else None.  
-000078d0: 2020 2020 2020 656e 645f 626f 6f6b 203d        end_book =
-000078e0: 2061 7267 735b 335d 2069 6620 6c65 6e28   args[3] if len(
-000078f0: 6172 6773 2920 3e20 3320 656c 7365 204e  args) > 3 else N
-00007900: 6f6e 650a 2020 2020 2020 2020 656e 645f  one.        end_
-00007910: 6368 6170 203d 2061 7267 735b 345d 2069  chap = args[4] i
-00007920: 6620 6c65 6e28 6172 6773 2920 3e20 3420  f len(args) > 4 
-00007930: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-00007940: 2020 656e 645f 7665 7273 6520 3d20 6172    end_verse = ar
-00007950: 6773 5b35 5d20 6966 206c 656e 2861 7267  gs[5] if len(arg
-00007960: 7329 203e 2035 2065 6c73 6520 4e6f 6e65  s) > 5 else None
-00007970: 0a0a 2020 2020 2020 2020 6966 2073 7461  ..        if sta
-00007980: 7274 5f62 6f6f 6b20 6973 206e 6f74 204e  rt_book is not N
-00007990: 6f6e 6520 616e 6420 6973 696e 7374 616e  one and isinstan
-000079a0: 6365 2873 7461 7274 5f62 6f6f 6b2c 2073  ce(start_book, s
-000079b0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000079c0: 2073 7461 7274 5f62 6f6f 6b20 3d20 4269   start_book = Bi
-000079d0: 626c 6542 6f6f 6b2e 6672 6f6d 5f73 7472  bleBook.from_str
-000079e0: 2873 7461 7274 5f62 6f6f 6b2c 2072 6169  (start_book, rai
-000079f0: 7365 5f65 7272 6f72 3d54 7275 6529 0a20  se_error=True). 
-00007a00: 2020 2020 2020 2065 6c69 6620 7374 6172         elif star
-00007a10: 745f 626f 6f6b 2069 7320 6e6f 7420 4e6f  t_book is not No
-00007a20: 6e65 2061 6e64 206e 6f74 2069 7369 6e73  ne and not isins
-00007a30: 7461 6e63 6528 7374 6172 745f 626f 6f6b  tance(start_book
-00007a40: 2c20 4269 626c 6542 6f6f 6b29 3a0a 2020  , BibleBook):.  
-00007a50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00007a60: 496e 7661 6c69 6452 6566 6572 656e 6365  InvalidReference
-00007a70: 4572 726f 7228 6622 7b73 7461 7274 5f62  Error(f"{start_b
-00007a80: 6f6f 6b7d 2069 7320 6e6f 7420 6120 7661  ook} is not a va
-00007a90: 6c69 6420 4269 626c 6542 6f6f 6b22 290a  lid BibleBook").
-00007aa0: 0a20 2020 2020 2020 2069 6620 656e 645f  .        if end_
-00007ab0: 626f 6f6b 2069 7320 6e6f 7420 4e6f 6e65  book is not None
-00007ac0: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
-00007ad0: 656e 645f 626f 6f6b 2c20 7374 7229 3a0a  end_book, str):.
-00007ae0: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-00007af0: 626f 6f6b 203d 2042 6962 6c65 426f 6f6b  book = BibleBook
-00007b00: 2e66 726f 6d5f 7374 7228 656e 645f 626f  .from_str(end_bo
-00007b10: 6f6b 2c20 7261 6973 655f 6572 726f 723d  ok, raise_error=
-00007b20: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
-00007b30: 6966 2065 6e64 5f62 6f6f 6b20 6973 206e  if end_book is n
-00007b40: 6f74 204e 6f6e 6520 616e 6420 6e6f 7420  ot None and not 
-00007b50: 6973 696e 7374 616e 6365 2865 6e64 5f62  isinstance(end_b
-00007b60: 6f6f 6b2c 2042 6962 6c65 426f 6f6b 293a  ook, BibleBook):
-00007b70: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00007b80: 7365 2049 6e76 616c 6964 5265 6665 7265  se InvalidRefere
-00007b90: 6e63 6545 7272 6f72 2866 227b 656e 645f  nceError(f"{end_
-00007ba0: 626f 6f6b 7d20 6973 206e 6f74 2061 2076  book} is not a v
-00007bb0: 616c 6964 2042 6962 6c65 426f 6f6b 2229  alid BibleBook")
-00007bc0: 0a0a 2020 2020 2020 2020 2320 4966 2073  ..        # If s
-00007bd0: 7461 7274 203e 2065 6e64 2c20 7377 6170  tart > end, swap
-00007be0: 2061 726f 756e 642e 2054 6865 206c 6f67   around. The log
-00007bf0: 6963 2069 7320 6d65 7373 7920 6475 6520  ic is messy due 
-00007c00: 746f 2069 6d70 6c69 6564 2076 616c 7565  to implied value
-00007c10: 7320 7768 656e 2061 7267 7320 6172 6520  s when args are 
-00007c20: 4e6f 6e65 2e0a 2020 2020 2020 2020 6966  None..        if
-00007c30: 2073 7461 7274 5f62 6f6f 6b20 6973 206e   start_book is n
-00007c40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007c50: 2020 2020 2069 6620 656e 645f 626f 6f6b       if end_book
-00007c60: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00007c70: 2073 7461 7274 5f62 6f6f 6b20 3e20 656e   start_book > en
-00007c80: 645f 626f 6f6b 3a0a 2020 2020 2020 2020  d_book:.        
-00007c90: 2020 2020 2020 2020 2873 7461 7274 5f62          (start_b
-00007ca0: 6f6f 6b2c 2065 6e64 5f62 6f6f 6b29 203d  ook, end_book) =
-00007cb0: 2028 656e 645f 626f 6f6b 2c20 7374 6172   (end_book, star
-00007cc0: 745f 626f 6f6b 290a 2020 2020 2020 2020  t_book).        
-00007cd0: 2020 2020 2020 2020 2873 7461 7274 5f63          (start_c
-00007ce0: 6861 702c 2065 6e64 5f63 6861 7029 203d  hap, end_chap) =
-00007cf0: 2028 656e 645f 6368 6170 2c20 7374 6172   (end_chap, star
-00007d00: 745f 6368 6170 290a 2020 2020 2020 2020  t_chap).        
-00007d10: 2020 2020 2020 2020 2873 7461 7274 5f76          (start_v
-00007d20: 6572 7365 2c20 656e 645f 7665 7273 6529  erse, end_verse)
-00007d30: 203d 2028 656e 645f 7665 7273 652c 2073   = (end_verse, s
-00007d40: 7461 7274 5f76 6572 7365 290a 2020 2020  tart_verse).    
-00007d50: 2020 2020 2020 2020 656c 6966 2028 656e          elif (en
-00007d60: 645f 626f 6f6b 2069 7320 4e6f 6e65 206f  d_book is None o
-00007d70: 7220 656e 645f 626f 6f6b 203d 3d20 7374  r end_book == st
-00007d80: 6172 745f 626f 6f6b 2920 616e 6420 7374  art_book) and st
-00007d90: 6172 745f 6368 6170 2069 7320 6e6f 7420  art_chap is not 
-00007da0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00007db0: 2020 2020 2020 6966 2065 6e64 5f63 6861        if end_cha
-00007dc0: 7020 6973 206e 6f74 204e 6f6e 6520 616e  p is not None an
-00007dd0: 6420 7374 6172 745f 6368 6170 203e 2065  d start_chap > e
-00007de0: 6e64 5f63 6861 703a 0a20 2020 2020 2020  nd_chap:.       
-00007df0: 2020 2020 2020 2020 2020 2020 2028 7374               (st
-00007e00: 6172 745f 6368 6170 2c20 656e 645f 6368  art_chap, end_ch
-00007e10: 6170 2920 3d20 2865 6e64 5f63 6861 702c  ap) = (end_chap,
-00007e20: 2073 7461 7274 5f63 6861 7029 0a20 2020   start_chap).   
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2028 7374 6172 745f 7665 7273 652c 2065   (start_verse, e
-00007e50: 6e64 5f76 6572 7365 2920 3d20 2865 6e64  nd_verse) = (end
-00007e60: 5f76 6572 7365 2c20 7374 6172 745f 7665  _verse, start_ve
-00007e70: 7273 6529 0a20 2020 2020 2020 2020 2020  rse).           
-00007e80: 2020 2020 2065 6c69 6620 2865 6e64 5f63       elif (end_c
-00007e90: 6861 7020 6973 204e 6f6e 6520 6f72 2065  hap is None or e
-00007ea0: 6e64 5f63 6861 7020 3d3d 2073 7461 7274  nd_chap == start
-00007eb0: 5f63 6861 7029 2061 6e64 2073 7461 7274  _chap) and start
-00007ec0: 5f76 6572 7365 2069 7320 6e6f 7420 4e6f  _verse is not No
-00007ed0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007ee0: 2020 2020 2020 2020 6966 2065 6e64 5f76          if end_v
-00007ef0: 6572 7365 2069 7320 6e6f 7420 4e6f 6e65  erse is not None
-00007f00: 2061 6e64 2073 7461 7274 5f76 6572 7365   and start_verse
-00007f10: 203e 2065 6e64 5f76 6572 7365 3a0a 2020   > end_verse:.  
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 2020 2020 2873 7461 7274 5f76 6572        (start_ver
-00007f40: 7365 2c20 656e 645f 7665 7273 6529 203d  se, end_verse) =
-00007f50: 2028 656e 645f 7665 7273 652c 2073 7461   (end_verse, sta
-00007f60: 7274 5f76 6572 7365 290a 0a20 2020 2020  rt_verse)..     
-00007f70: 2020 2068 6176 655f 656e 6420 3d20 2865     have_end = (e
-00007f80: 6e64 5f62 6f6f 6b20 6973 206e 6f74 204e  nd_book is not N
-00007f90: 6f6e 6529 206f 7220 2865 6e64 5f63 6861  one) or (end_cha
-00007fa0: 7020 6973 206e 6f74 204e 6f6e 6529 206f  p is not None) o
-00007fb0: 7220 2865 6e64 5f76 6572 7365 2069 7320  r (end_verse is 
-00007fc0: 6e6f 7420 4e6f 6e65 290a 0a20 2020 2020  not None)..     
-00007fd0: 2020 2069 6620 7374 6172 745f 626f 6f6b     if start_book
-00007fe0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00007ff0: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
-00008000: 6c69 6452 6566 6572 656e 6365 4572 726f  lidReferenceErro
-00008010: 7228 6622 4120 7374 6172 7420 626f 6f6b  r(f"A start book
-00008020: 2069 7320 6e65 6564 6564 2066 6f72 2061   is needed for a
-00008030: 2042 6962 6c65 5261 6e67 6522 290a 2020   BibleRange").  
-00008040: 2020 2020 2020 6966 2073 7461 7274 5f63        if start_c
-00008050: 6861 7020 6973 204e 6f6e 6520 616e 6420  hap is None and 
-00008060: 7374 6172 745f 7665 7273 6520 6973 206e  start_verse is n
-00008070: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008080: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
-00008090: 6964 5265 6665 7265 6e63 6545 7272 6f72  idReferenceError
-000080a0: 2822 5374 6172 7420 7665 7273 6520 6973  ("Start verse is
-000080b0: 206d 6973 7369 6e67 2061 2073 7461 7274   missing a start
-000080c0: 2063 6861 7074 6572 2229 0a0a 2020 2020   chapter")..    
-000080d0: 2020 2020 6966 2073 7461 7274 5f63 6861      if start_cha
-000080e0: 7020 6973 204e 6f6e 653a 2023 2053 7461  p is None: # Sta
-000080f0: 7274 2069 7320 626f 6f6b 206f 6e6c 790a  rt is book only.
-00008100: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00008110: 7420 3d20 7374 6172 745f 626f 6f6b 2e66  t = start_book.f
-00008120: 6972 7374 5f76 6572 7365 284e 6f6e 652c  irst_verse(None,
-00008130: 2066 6c61 6773 290a 2020 2020 2020 2020   flags).        
-00008140: 2020 2020 6966 206e 6f74 2068 6176 655f      if not have_
-00008150: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
-00008160: 2020 2020 2065 6e64 203d 2073 7461 7274       end = start
-00008170: 5f62 6f6f 6b2e 6c61 7374 5f76 6572 7365  _book.last_verse
-00008180: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
-00008190: 7374 6172 745f 7665 7273 6520 6973 204e  start_verse is N
-000081a0: 6f6e 653a 2023 2053 7461 7274 2069 7320  one: # Start is 
-000081b0: 626f 6f6b 2061 6e64 2063 6861 7020 6f6e  book and chap on
-000081c0: 6c79 0a20 2020 2020 2020 2020 2020 2073  ly.            s
-000081d0: 7461 7274 203d 2073 7461 7274 5f62 6f6f  tart = start_boo
-000081e0: 6b2e 6669 7273 745f 7665 7273 6528 696e  k.first_verse(in
-000081f0: 7428 7374 6172 745f 6368 6170 292c 2066  t(start_chap), f
-00008200: 6c61 6773 3d66 6c61 6773 290a 2020 2020  lags=flags).    
-00008210: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-00008220: 6176 655f 656e 643a 0a20 2020 2020 2020  ave_end:.       
-00008230: 2020 2020 2020 2020 2065 6e64 203d 2073           end = s
-00008240: 7461 7274 5f62 6f6f 6b2e 6c61 7374 5f76  tart_book.last_v
-00008250: 6572 7365 2869 6e74 2873 7461 7274 5f63  erse(int(start_c
-00008260: 6861 7029 290a 2020 2020 2020 2020 656c  hap)).        el
-00008270: 7365 3a20 2320 5374 6172 7420 6973 2062  se: # Start is b
-00008280: 6f6f 6b2c 2063 6861 7020 616e 6420 7665  ook, chap and ve
-00008290: 7273 650a 2020 2020 2020 2020 2020 2020  rse.            
-000082a0: 7374 6172 7420 3d20 4269 626c 6556 6572  start = BibleVer
-000082b0: 7365 2873 7461 7274 5f62 6f6f 6b2c 2069  se(start_book, i
-000082c0: 6e74 2873 7461 7274 5f63 6861 7029 2c20  nt(start_chap), 
-000082d0: 696e 7428 7374 6172 745f 7665 7273 6529  int(start_verse)
-000082e0: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
-000082f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00008300: 7420 6861 7665 5f65 6e64 3a20 2320 5369  t have_end: # Si
-00008310: 6e67 6c65 2076 6572 7365 2072 6566 6572  ngle verse refer
-00008320: 656e 6365 2c20 736f 2065 6e64 2069 7320  ence, so end is 
-00008330: 7361 6d65 2061 7320 7374 6172 740a 2020  same as start.  
-00008340: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00008350: 6420 3d20 4269 626c 6556 6572 7365 2873  d = BibleVerse(s
-00008360: 7461 7274 5f62 6f6f 6b2c 2069 6e74 2873  tart_book, int(s
-00008370: 7461 7274 5f63 6861 7029 2c20 696e 7428  tart_chap), int(
-00008380: 7374 6172 745f 7665 7273 6529 2c20 666c  start_verse), fl
-00008390: 6167 733d 666c 6167 7329 0a20 2020 2020  ags=flags).     
-000083a0: 2020 200a 2020 2020 2020 2020 6966 2068     .        if h
-000083b0: 6176 655f 656e 643a 2023 2057 6520 6861  ave_end: # We ha
-000083c0: 7665 2065 6e64 2d70 6f69 6e74 2069 6e66  ve end-point inf
-000083d0: 6f0a 2020 2020 2020 2020 2020 2020 6966  o.            if
-000083e0: 2065 6e64 5f62 6f6f 6b20 6973 204e 6f6e   end_book is Non
-000083f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00008400: 2020 2065 6e64 5f62 6f6f 6b20 3d20 7374     end_book = st
-00008410: 6172 745f 626f 6f6b 0a20 2020 2020 2020  art_book.       
-00008420: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00008430: 2020 6966 2065 6e64 5f63 6861 7020 6973    if end_chap is
-00008440: 204e 6f6e 6520 616e 6420 656e 645f 7665   None and end_ve
-00008450: 7273 6520 6973 204e 6f6e 653a 2023 2045  rse is None: # E
-00008460: 6e64 2069 7320 626f 6f6b 206f 6e6c 790a  nd is book only.
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 656e 6420 3d20 656e 645f 626f 6f6b 2e6c  end = end_book.l
-00008490: 6173 745f 7665 7273 6528 290a 2020 2020  ast_verse().    
-000084a0: 2020 2020 2020 2020 656c 6966 2065 6e64          elif end
-000084b0: 5f76 6572 7365 2069 7320 4e6f 6e65 3a20  _verse is None: 
-000084c0: 2320 456e 6420 6973 2062 6f6f 6b20 616e  # End is book an
-000084d0: 6420 6368 6170 206f 6e6c 790a 2020 2020  d chap only.    
-000084e0: 2020 2020 2020 2020 2020 2020 656e 6420              end 
-000084f0: 3d20 656e 645f 626f 6f6b 2e6c 6173 745f  = end_book.last_
-00008500: 7665 7273 6528 696e 7428 656e 645f 6368  verse(int(end_ch
-00008510: 6170 2929 0a20 2020 2020 2020 2020 2020  ap)).           
-00008520: 2065 6c69 6620 656e 645f 6368 6170 2069   elif end_chap i
-00008530: 7320 4e6f 6e65 3a20 2320 456e 6420 6973  s None: # End is
-00008540: 2062 6f6f 6b20 616e 6420 7665 7273 6520   book and verse 
-00008550: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
-00008560: 2020 2020 2069 6620 7374 6172 745f 626f       if start_bo
-00008570: 6f6b 2021 3d20 656e 645f 626f 6f6b 3a0a  ok != end_book:.
-00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008590: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
-000085a0: 6452 6566 6572 656e 6365 4572 726f 7228  dReferenceError(
-000085b0: 2245 6e64 2076 6572 7365 2069 7320 6d69  "End verse is mi
-000085c0: 7373 696e 6720 616e 2065 6e64 2063 6861  ssing an end cha
-000085d0: 7074 6572 2229 0a20 2020 2020 2020 2020  pter").         
-000085e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2065 6e64 203d 2042 6962 6c65 5665 7273   end = BibleVers
-00008610: 6528 656e 645f 626f 6f6b 2c20 696e 7428  e(end_book, int(
-00008620: 7374 6172 742e 6368 6170 5f6e 756d 292c  start.chap_num),
-00008630: 2069 6e74 2865 6e64 5f76 6572 7365 292c   int(end_verse),
-00008640: 2066 6c61 6773 3d66 6c61 6773 290a 2020   flags=flags).  
-00008650: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008670: 656e 6420 3d20 4269 626c 6556 6572 7365  end = BibleVerse
-00008680: 2865 6e64 5f62 6f6f 6b2c 2069 6e74 2865  (end_book, int(e
-00008690: 6e64 5f63 6861 7029 2c20 696e 7428 656e  nd_chap), int(en
-000086a0: 645f 7665 7273 6529 2c20 666c 6167 733d  d_verse), flags=
-000086b0: 666c 6167 7329 0a0a 2020 2020 2020 2020  flags)..        
-000086c0: 6966 2042 6962 6c65 466c 6167 2e4d 554c  if BibleFlag.MUL
-000086d0: 5449 424f 4f4b 206e 6f74 2069 6e20 666c  TIBOOK not in fl
-000086e0: 6167 7320 616e 6420 7374 6172 742e 626f  ags and start.bo
-000086f0: 6f6b 2021 3d20 656e 642e 626f 6f6b 3a0a  ok != end.book:.
-00008700: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008710: 6520 4d75 6c74 6962 6f6f 6b52 616e 6765  e MultibookRange
-00008720: 4e6f 7441 6c6c 6f77 6564 4572 726f 7228  NotAllowedError(
-00008730: 6622 4d75 6c74 692d 626f 6f6b 2072 616e  f"Multi-book ran
-00008740: 6765 7320 6e6f 7420 616c 6c6f 7765 6420  ges not allowed 
-00008750: 2220 2b20 0a20 2020 2020 2020 2020 2020  " + .           
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2066 2228 7b73 7461 7274 2e62       f"({start.b
-00008790: 6f6f 6b2e 6162 6272 6576 7d20 616e 6420  ook.abbrev} and 
-000087a0: 7b65 6e64 2e62 6f6f 6b2e 6162 6272 6576  {end.book.abbrev
-000087b0: 7d20 6172 6520 6469 6666 6572 656e 7429  } are different)
-000087c0: 2229 0a0a 2020 2020 2020 2020 6f62 6a65  ")..        obje
-000087d0: 6374 2e5f 5f73 6574 6174 7472 5f5f 2873  ct.__setattr__(s
-000087e0: 656c 662c 2022 7374 6172 7422 2c20 7374  elf, "start", st
-000087f0: 6172 7429 0a20 2020 2020 2020 206f 626a  art).        obj
-00008800: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
-00008810: 7365 6c66 2c20 2265 6e64 222c 2065 6e64  self, "end", end
-00008820: 290a 0a20 2020 2064 6566 2076 6572 7365  )..    def verse
-00008830: 5f30 5f74 6f5f 3128 7365 6c66 2920 2d3e  _0_to_1(self) ->
-00008840: 2027 4269 626c 6552 616e 6765 273a 0a20   'BibleRange':. 
-00008850: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-00008860: 7320 6120 6e65 7720 6042 6962 6c65 5261  s a new `BibleRa
-00008870: 6e67 6560 2063 7265 6174 6564 2062 7920  nge` created by 
-00008880: 6361 6c6c 696e 6720 6076 6572 7365 5f30  calling `verse_0
-00008890: 5f74 6f5f 3128 2960 206f 6e20 626f 7468  _to_1()` on both
-000088a0: 2074 6865 2060 7374 6172 7460 2061 6e64   the `start` and
-000088b0: 2060 656e 6460 0a20 2020 2020 2020 2060   `end`.        `
-000088c0: 4269 626c 6556 6572 7365 6020 6174 7472  BibleVerse` attr
-000088d0: 6962 7574 6573 2e27 2727 0a20 2020 2020  ibutes.'''.     
-000088e0: 2020 2072 6574 7572 6e20 4269 626c 6552     return BibleR
-000088f0: 616e 6765 2873 7461 7274 3d73 656c 662e  ange(start=self.
-00008900: 7374 6172 742e 7665 7273 655f 305f 746f  start.verse_0_to
-00008910: 5f31 2829 2c20 656e 643d 7365 6c66 2e65  _1(), end=self.e
-00008920: 6e64 2e76 6572 7365 5f30 5f74 6f5f 3128  nd.verse_0_to_1(
-00008930: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00008940: 2020 2020 2020 2020 2020 2020 2066 6c61               fla
-00008950: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
-00008960: 290a 0a20 2020 2064 6566 2076 6572 7365  )..    def verse
-00008970: 5f31 5f74 6f5f 3028 7365 6c66 2920 2d3e  _1_to_0(self) ->
-00008980: 2027 4269 626c 6552 616e 6765 273a 0a20   'BibleRange':. 
-00008990: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-000089a0: 7320 6120 6e65 7720 6042 6962 6c65 5261  s a new `BibleRa
-000089b0: 6e67 6560 2063 7265 6174 6564 2062 7920  nge` created by 
-000089c0: 6361 6c6c 696e 6720 6076 6572 7365 5f31  calling `verse_1
-000089d0: 5f74 6f5f 3028 2960 206f 6e20 626f 7468  _to_0()` on both
-000089e0: 2074 6865 2060 7374 6172 7460 2061 6e64   the `start` and
-000089f0: 2060 656e 6460 0a20 2020 2020 2020 2060   `end`.        `
-00008a00: 4269 626c 6556 6572 7365 6020 6174 7472  BibleVerse` attr
-00008a10: 6962 7574 6573 2e20 2a2a 4e6f 7465 2a2a  ibutes. **Note**
-00008a20: 3a20 5468 6520 7661 6c75 6520 6f66 2074  : The value of t
-00008a30: 6865 2067 6c6f 6261 6c20 6174 7472 6962  he global attrib
-00008a40: 7574 6520 6062 6962 6c65 7265 662e 7265  ute `bibleref.re
-00008a50: 662e 666c 6167 7360 2069 7320 2a69 676e  f.flags` is *ign
-00008a60: 6f72 6564 2a2e 2727 270a 2020 2020 2020  ored*.'''.      
-00008a70: 2020 7265 7475 726e 2042 6962 6c65 5261    return BibleRa
-00008a80: 6e67 6528 7374 6172 743d 7365 6c66 2e73  nge(start=self.s
-00008a90: 7461 7274 2e76 6572 7365 5f31 5f74 6f5f  tart.verse_1_to_
-00008aa0: 3028 292c 2065 6e64 3d73 656c 662e 656e  0(), end=self.en
-00008ab0: 642e 7665 7273 655f 315f 746f 5f30 2829  d.verse_1_to_0()
-00008ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008ad0: 2020 2020 2020 2020 2020 2020 666c 6167              flag
-00008ae0: 733d 4269 626c 6546 6c61 672e 414c 4c29  s=BibleFlag.ALL)
-00008af0: 0a0a 2020 2020 6465 6620 6973 5f73 696e  ..    def is_sin
-00008b00: 676c 655f 7665 7273 6528 7365 6c66 2920  gle_verse(self) 
-00008b10: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00008b20: 2027 2727 5265 7475 726e 7320 6054 7275   '''Returns `Tru
-00008b30: 6560 2069 6620 7468 6520 6042 6962 6c65  e` if the `Bible
-00008b40: 5261 6e67 6560 2065 7861 6374 6c79 2063  Range` exactly c
-00008b50: 6f6e 7461 696e 7320 6120 7369 6e67 6c65  ontains a single
-00008b60: 2076 6572 7365 2c20 656c 7365 2060 4661   verse, else `Fa
-00008b70: 6c73 6560 2e27 2727 0a20 2020 2020 2020  lse`.'''.       
-00008b80: 2072 6574 7572 6e20 2028 7365 6c66 2e73   return  (self.s
-00008b90: 7461 7274 203d 3d20 7365 6c66 2e65 6e64  tart == self.end
-00008ba0: 290a 0a20 2020 2064 6566 2069 735f 7768  )..    def is_wh
-00008bb0: 6f6c 655f 6368 6170 2873 656c 662c 2066  ole_chap(self, f
-00008bc0: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
-00008bd0: 3d20 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a  = None) -> bool:
-00008be0: 0a20 2020 2020 2020 2027 2727 5265 7475  .        '''Retu
-00008bf0: 726e 7320 6054 7275 6560 2069 6620 7468  rns `True` if th
-00008c00: 6973 2060 4269 626c 6552 616e 6765 6020  is `BibleRange` 
-00008c10: 6578 6163 746c 7920 7370 616e 7320 6f6e  exactly spans on
-00008c20: 6520 7768 6f6c 6520 6368 6170 7465 722c  e whole chapter,
-00008c30: 2065 6c73 6520 6046 616c 7365 602e 2727   else `False`.''
-00008c40: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-00008c50: 2020 2873 656c 662e 7374 6172 742e 626f    (self.start.bo
-00008c60: 6f6b 203d 3d20 7365 6c66 2e65 6e64 2e62  ok == self.end.b
-00008c70: 6f6f 6b29 2061 6e64 205c 0a20 2020 2020  ook) and \.     
-00008c80: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
-00008c90: 2e73 7461 7274 203d 3d20 7365 6c66 2e73  .start == self.s
-00008ca0: 7461 7274 2e62 6f6f 6b2e 6669 7273 745f  tart.book.first_
-00008cb0: 7665 7273 6528 7365 6c66 2e73 7461 7274  verse(self.start
-00008cc0: 2e63 6861 705f 6e75 6d2c 2066 6c61 6773  .chap_num, flags
-00008cd0: 3d66 6c61 6773 2929 2061 6e64 205c 0a20  =flags)) and \. 
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00008cf0: 7365 6c66 2e65 6e64 203d 3d20 7365 6c66  self.end == self
-00008d00: 2e65 6e64 2e62 6f6f 6b2e 6c61 7374 5f76  .end.book.last_v
-00008d10: 6572 7365 2873 656c 662e 7374 6172 742e  erse(self.start.
-00008d20: 6368 6170 5f6e 756d 2929 0a0a 2020 2020  chap_num))..    
-00008d30: 6465 6620 7370 616e 735f 7374 6172 745f  def spans_start_
-00008d40: 6368 6170 2873 656c 662c 2066 6c61 6773  chap(self, flags
-00008d50: 3a20 4269 626c 6546 6c61 6720 3d20 4e6f  : BibleFlag = No
-00008d60: 6e65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ne) -> bool:.   
-00008d70: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
-00008d80: 6054 7275 6560 2069 6620 7468 6973 2060  `True` if this `
-00008d90: 4269 626c 6552 616e 6765 6020 696e 636c  BibleRange` incl
-00008da0: 7564 6573 2074 6865 2077 686f 6c65 2063  udes the whole c
-00008db0: 6861 7074 6572 2074 6861 7420 636f 6e74  hapter that cont
-00008dc0: 6169 6e73 2074 6865 2060 7374 6172 7460  ains the `start`
-00008dd0: 2076 6572 7365 2c0a 2020 2020 2020 2020   verse,.        
-00008de0: 656c 7365 2060 4661 6c73 6560 2e27 2727  else `False`.'''
-00008df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008e00: 2028 7365 6c66 2e73 7461 7274 203d 3d20   (self.start == 
-00008e10: 7365 6c66 2e73 7461 7274 2e62 6f6f 6b2e  self.start.book.
-00008e20: 6669 7273 745f 7665 7273 6528 7365 6c66  first_verse(self
-00008e30: 2e73 7461 7274 2e63 6861 705f 6e75 6d2c  .start.chap_num,
-00008e40: 2066 6c61 6773 3d66 6c61 6773 2929 2061   flags=flags)) a
-00008e50: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
-00008e60: 2020 2020 2028 7365 6c66 2e65 6e64 203e       (self.end >
-00008e70: 3d20 7365 6c66 2e73 7461 7274 2e62 6f6f  = self.start.boo
-00008e80: 6b2e 6c61 7374 5f76 6572 7365 2873 656c  k.last_verse(sel
-00008e90: 662e 7374 6172 742e 6368 6170 5f6e 756d  f.start.chap_num
-00008ea0: 2929 0a0a 2020 2020 6465 6620 7370 616e  ))..    def span
-00008eb0: 735f 656e 645f 6368 6170 2873 656c 662c  s_end_chap(self,
-00008ec0: 2066 6c61 6773 3a20 4269 626c 6546 6c61   flags: BibleFla
-00008ed0: 6720 3d20 4e6f 6e65 2920 2d3e 2062 6f6f  g = None) -> boo
-00008ee0: 6c3a 0a20 2020 2020 2020 2027 2727 5265  l:.        '''Re
-00008ef0: 7475 726e 7320 6054 7275 6560 2069 6620  turns `True` if 
-00008f00: 7468 6973 2060 4269 626c 6552 616e 6765  this `BibleRange
-00008f10: 6020 696e 636c 7564 6573 2074 6865 2077  ` includes the w
-00008f20: 686f 6c65 2063 6861 7074 6572 2074 6861  hole chapter tha
-00008f30: 7420 636f 6e74 6169 6e73 2074 6865 2060  t contains the `
-00008f40: 656e 6460 2076 6572 7365 2c0a 2020 2020  end` verse,.    
-00008f50: 2020 2020 656c 7365 2060 4661 6c73 6560      else `False`
-00008f60: 2e27 2727 0a20 2020 2020 2020 2072 6574  .'''.        ret
-00008f70: 7572 6e20 2028 7365 6c66 2e65 6e64 203d  urn  (self.end =
-00008f80: 3d20 7365 6c66 2e65 6e64 2e62 6f6f 6b2e  = self.end.book.
-00008f90: 6c61 7374 5f76 6572 7365 2873 656c 662e  last_verse(self.
-00008fa0: 656e 642e 6368 6170 5f6e 756d 2929 2061  end.chap_num)) a
-00008fb0: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
-00008fc0: 2020 2020 2028 7365 6c66 2e73 7461 7274       (self.start
-00008fd0: 203c 3d20 7365 6c66 2e65 6e64 2e62 6f6f   <= self.end.boo
-00008fe0: 6b2e 6669 7273 745f 7665 7273 6528 7365  k.first_verse(se
-00008ff0: 6c66 2e65 6e64 2e63 6861 705f 6e75 6d2c  lf.end.chap_num,
-00009000: 2066 6c61 6773 3d66 6c61 6773 2929 0a0a   flags=flags))..
-00009010: 2020 2020 6465 6620 6973 5f77 686f 6c65      def is_whole
-00009020: 5f62 6f6f 6b28 7365 6c66 2c20 666c 6167  _book(self, flag
-00009030: 733a 2042 6962 6c65 466c 6167 203d 204e  s: BibleFlag = N
-00009040: 6f6e 6529 202d 3e20 626f 6f6c 3a0a 2020  one) -> bool:.  
-00009050: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
-00009060: 2060 5472 7565 6020 6966 2074 6869 7320   `True` if this 
-00009070: 6042 6962 6c65 5261 6e67 6560 2065 7861  `BibleRange` exa
-00009080: 6374 6c79 2073 7061 6e73 206f 6e65 2077  ctly spans one w
-00009090: 686f 6c65 2062 6f6f 6b2c 2065 6c73 6520  hole book, else 
-000090a0: 6046 616c 7365 602e 2727 270a 2020 2020  `False`.'''.    
-000090b0: 2020 2020 7265 7475 726e 2020 2873 656c      return  (sel
-000090c0: 662e 7374 6172 742e 626f 6f6b 203d 3d20  f.start.book == 
-000090d0: 7365 6c66 2e65 6e64 2e62 6f6f 6b29 2061  self.end.book) a
-000090e0: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
-000090f0: 2020 2020 2028 7365 6c66 2e73 7461 7274       (self.start
-00009100: 203d 3d20 7365 6c66 2e73 7461 7274 2e62   == self.start.b
-00009110: 6f6f 6b2e 6669 7273 745f 7665 7273 6528  ook.first_verse(
-00009120: 4e6f 6e65 2c20 666c 6167 7329 2920 616e  None, flags)) an
-00009130: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
-00009140: 2020 2020 2873 656c 662e 656e 6420 3d3d      (self.end ==
-00009150: 2073 656c 662e 656e 642e 626f 6f6b 2e6c   self.end.book.l
-00009160: 6173 745f 7665 7273 6528 2929 0a0a 2020  ast_verse())..  
-00009170: 2020 6465 6620 7370 616e 735f 7374 6172    def spans_star
-00009180: 745f 626f 6f6b 2873 656c 662c 2066 6c61  t_book(self, fla
-00009190: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-000091a0: 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a 0a20  None) -> bool:. 
-000091b0: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-000091c0: 7320 6054 7275 6560 2069 6620 7468 6973  s `True` if this
-000091d0: 2060 4269 626c 6552 616e 6765 6020 696e   `BibleRange` in
-000091e0: 636c 7564 6573 2074 6865 2077 686f 6c65  cludes the whole
-000091f0: 2062 6f6f 6b20 7468 6174 2063 6f6e 7461   book that conta
-00009200: 696e 7320 7468 6520 6073 7461 7274 6020  ins the `start` 
-00009210: 7665 7273 652c 0a20 2020 2020 2020 2065  verse,.        e
-00009220: 6c73 6520 6046 616c 7365 602e 2727 270a  lse `False`.'''.
-00009230: 2020 2020 2020 2020 7265 7475 726e 2020          return  
-00009240: 2873 656c 662e 7374 6172 7420 3d3d 2073  (self.start == s
-00009250: 656c 662e 7374 6172 742e 626f 6f6b 2e66  elf.start.book.f
-00009260: 6972 7374 5f76 6572 7365 284e 6f6e 652c  irst_verse(None,
-00009270: 2066 6c61 6773 2929 2061 6e64 205c 0a20   flags)) and \. 
-00009280: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00009290: 7365 6c66 2e65 6e64 203e 3d20 7365 6c66  self.end >= self
-000092a0: 2e73 7461 7274 2e62 6f6f 6b2e 6c61 7374  .start.book.last
-000092b0: 5f76 6572 7365 2829 290a 0a20 2020 2064  _verse())..    d
-000092c0: 6566 2073 7061 6e73 5f65 6e64 5f62 6f6f  ef spans_end_boo
-000092d0: 6b28 7365 6c66 2c20 666c 6167 733a 2042  k(self, flags: B
-000092e0: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-000092f0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00009300: 2020 2727 2752 6574 7572 6e73 2060 5472    '''Returns `Tr
-00009310: 7565 6020 6966 2074 6869 7320 6042 6962  ue` if this `Bib
-00009320: 6c65 5261 6e67 6560 2069 6e63 6c75 6465  leRange` include
-00009330: 7320 7468 6520 7768 6f6c 6520 626f 6f6b  s the whole book
-00009340: 2074 6861 7420 636f 6e74 6169 6e73 2074   that contains t
-00009350: 6865 2060 656e 6460 2076 6572 7365 2c0a  he `end` verse,.
-00009360: 2020 2020 2020 2020 656c 7365 2060 4661          else `Fa
-00009370: 6c73 6560 2e27 2727 0a20 2020 2020 2020  lse`.'''.       
-00009380: 2072 6574 7572 6e20 2028 7365 6c66 2e65   return  (self.e
-00009390: 6e64 203d 3d20 7365 6c66 2e65 6e64 2e62  nd == self.end.b
-000093a0: 6f6f 6b2e 6c61 7374 5f76 6572 7365 2829  ook.last_verse()
-000093b0: 2920 616e 6420 5c0a 2020 2020 2020 2020  ) and \.        
-000093c0: 2020 2020 2020 2020 2873 656c 662e 7374          (self.st
-000093d0: 6172 7420 3c3d 2073 656c 662e 656e 642e  art <= self.end.
-000093e0: 626f 6f6b 2e66 6972 7374 5f76 6572 7365  book.first_verse
-000093f0: 284e 6f6e 652c 2066 6c61 6773 2929 0a0a  (None, flags))..
-00009400: 2020 2020 6465 6620 7665 7273 655f 636f      def verse_co
-00009410: 756e 7428 7365 6c66 2c20 666c 6167 733a  unt(self, flags:
-00009420: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-00009430: 6529 3a0a 2020 2020 2020 2020 2727 2752  e):.        '''R
-00009440: 6574 7572 6e73 2074 6865 206e 756d 6265  eturns the numbe
-00009450: 7220 6f66 2076 6572 7365 7320 696e 2074  r of verses in t
-00009460: 6869 7320 7261 6e67 652e 2727 270a 2020  his range.'''.  
-00009470: 2020 2020 2020 2320 5765 2073 706c 6974        # We split
-00009480: 2074 6865 2072 616e 6765 2069 6e74 6f20   the range into 
-00009490: 6368 6170 7465 7273 2c20 7768 6963 6820  chapters, which 
-000094a0: 6973 206e 6f74 2074 6865 206d 6f73 7420  is not the most 
-000094b0: 6566 6669 6369 656e 7420 6170 7072 6f61  efficient approa
-000094c0: 6368 2c20 6275 7420 6d61 6b65 7320 7468  ch, but makes th
-000094d0: 6520 636f 756e 7469 6e67 2073 696d 706c  e counting simpl
-000094e0: 652e 0a20 2020 2020 2020 2062 6962 6c65  e..        bible
-000094f0: 5f72 616e 6765 7320 3d20 7365 6c66 2e73  _ranges = self.s
-00009500: 706c 6974 2862 795f 6368 6170 3d54 7275  plit(by_chap=Tru
-00009510: 6529 2023 2045 6163 6820 7261 6e67 6520  e) # Each range 
-00009520: 7769 6c6c 2074 6875 7320 6265 2077 6974  will thus be wit
-00009530: 6869 6e20 6974 7320 6f77 6e20 6368 6170  hin its own chap
-00009540: 7465 720a 2020 2020 2020 2020 636f 756e  ter.        coun
-00009550: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
-00009560: 7220 6269 626c 655f 7261 6e67 6520 696e  r bible_range in
-00009570: 2062 6962 6c65 5f72 616e 6765 733a 0a20   bible_ranges:. 
-00009580: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00009590: 202b 3d20 2862 6962 6c65 5f72 616e 6765   += (bible_range
-000095a0: 2e65 6e64 2e76 6572 7365 5f6e 756d 202d  .end.verse_num -
-000095b0: 2062 6962 6c65 5f72 616e 6765 2e73 7461   bible_range.sta
-000095c0: 7274 2e76 6572 7365 5f6e 756d 202b 2031  rt.verse_num + 1
-000095d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000095e0: 2063 6f75 6e74 0a0a 2020 2020 6465 6620   count..    def 
-000095f0: 6368 6170 5f63 6f75 6e74 2873 656c 662c  chap_count(self,
-00009600: 2077 686f 6c65 3a20 626f 6f6c 203d 2046   whole: bool = F
-00009610: 616c 7365 2c20 666c 6167 733a 2042 6962  alse, flags: Bib
-00009620: 6c65 466c 6167 203d 204e 6f6e 6529 3a0a  leFlag = None):.
-00009630: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-00009640: 6e73 2074 6865 206e 756d 6265 7220 6f66  ns the number of
-00009650: 2063 6861 7074 6572 7320 696e 2074 6869   chapters in thi
-00009660: 7320 7261 6e67 652e 0a20 2020 2020 2020  s range..       
-00009670: 200a 2020 2020 2020 2020 4966 2060 7768   .        If `wh
-00009680: 6f6c 6560 2069 7320 5472 7565 2c20 6f6e  ole` is True, on
-00009690: 6c79 2077 686f 6c65 2063 6861 7074 6572  ly whole chapter
-000096a0: 7320 6172 6520 636f 756e 7465 642e 204f  s are counted. O
-000096b0: 7468 6572 7769 7365 2070 6172 7469 616c  therwise partial
-000096c0: 2063 6861 7074 6572 7320 6172 6520 616c   chapters are al
-000096d0: 736f 2069 6e63 6c75 6465 6420 696e 2074  so included in t
-000096e0: 6865 0a20 2020 2020 2020 2063 6f75 6e74  he.        count
-000096f0: 2e27 2727 0a20 2020 2020 2020 2023 2057  .'''.        # W
-00009700: 6520 7370 6c69 7420 7468 6520 7261 6e67  e split the rang
-00009710: 6520 696e 746f 2063 6861 7074 6572 732c  e into chapters,
-00009720: 2077 6869 6368 2069 7320 6e6f 7420 7468   which is not th
-00009730: 6520 6d6f 7374 2065 6666 6963 6965 6e74  e most efficient
-00009740: 2061 7070 726f 6163 682c 2062 7574 206d   approach, but m
-00009750: 616b 6573 2074 6865 2063 6f75 6e74 696e  akes the countin
-00009760: 6720 7369 6d70 6c65 2e0a 2020 2020 2020  g simple..      
-00009770: 2020 6269 626c 655f 7261 6e67 6573 203d    bible_ranges =
-00009780: 2073 656c 662e 7370 6c69 7428 6279 5f63   self.split(by_c
-00009790: 6861 703d 5472 7565 290a 2020 2020 2020  hap=True).      
-000097a0: 2020 636f 756e 7420 3d20 6c65 6e28 6269    count = len(bi
-000097b0: 626c 655f 7261 6e67 6573 290a 2020 2020  ble_ranges).    
-000097c0: 2020 2020 6966 2077 686f 6c65 3a0a 2020      if whole:.  
-000097d0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000097e0: 2062 6962 6c65 5f72 616e 6765 735b 305d   bible_ranges[0]
-000097f0: 2e69 735f 7768 6f6c 655f 6368 6170 2829  .is_whole_chap()
-00009800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009810: 2020 636f 756e 7420 2d3d 2031 0a20 2020    count -= 1.   
-00009820: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00009830: 6269 626c 655f 7261 6e67 6573 2920 3e20  bible_ranges) > 
-00009840: 3120 616e 6420 6e6f 7420 6269 626c 655f  1 and not bible_
-00009850: 7261 6e67 6573 5b2d 315d 2e69 735f 7768  ranges[-1].is_wh
-00009860: 6f6c 655f 6368 6170 2829 3a0a 2020 2020  ole_chap():.    
-00009870: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-00009880: 7420 2d3d 2031 0a20 2020 2020 2020 2072  t -= 1.        r
-00009890: 6574 7572 6e20 636f 756e 740a 0a20 2020  eturn count..   
-000098a0: 2064 6566 2062 6f6f 6b5f 636f 756e 7428   def book_count(
-000098b0: 7365 6c66 2c20 7768 6f6c 653a 2062 6f6f  self, whole: boo
-000098c0: 6c20 3d20 4661 6c73 652c 2066 6c61 6773  l = False, flags
-000098d0: 3a20 4269 626c 6546 6c61 6720 3d20 4e6f  : BibleFlag = No
-000098e0: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
-000098f0: 5265 7475 726e 7320 7468 6520 6e75 6d62  Returns the numb
-00009900: 6572 206f 6620 4269 626c 6520 626f 6f6b  er of Bible book
-00009910: 7320 696e 2074 6869 7320 7261 6e67 652e  s in this range.
-00009920: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00009930: 2020 4966 2060 7768 6f6c 6560 2069 7320    If `whole` is 
-00009940: 5472 7565 2c20 6f6e 6c79 2077 686f 6c65  True, only whole
-00009950: 2062 6f6f 6b73 2061 7265 2063 6f75 6e74   books are count
-00009960: 6564 2e20 4f74 6865 7277 6973 652c 2070  ed. Otherwise, p
-00009970: 6172 7469 616c 2062 6f6f 6b73 2061 7265  artial books are
-00009980: 2061 6c73 6f20 696e 636c 7564 6564 2069   also included i
-00009990: 6e20 7468 6520 636f 756e 742e 2727 270a  n the count.'''.
-000099a0: 2020 2020 2020 2020 2320 5765 2073 706c          # We spl
-000099b0: 6974 2074 6865 2072 616e 6765 2069 6e74  it the range int
-000099c0: 6f20 626f 6f6b 732c 2077 6869 6368 2069  o books, which i
-000099d0: 7320 6e6f 7420 7468 6520 6d6f 7374 2065  s not the most e
-000099e0: 6666 6963 6965 6e74 2061 7070 726f 6163  fficient approac
-000099f0: 682c 2062 7574 206d 616b 6573 2074 6865  h, but makes the
-00009a00: 2063 6f75 6e74 696e 6720 7369 6d70 6c65   counting simple
-00009a10: 2e0a 2020 2020 2020 2020 6269 626c 655f  ..        bible_
-00009a20: 7261 6e67 6573 203d 2073 656c 662e 7370  ranges = self.sp
-00009a30: 6c69 7428 6279 5f62 6f6f 6b3d 5472 7565  lit(by_book=True
-00009a40: 290a 2020 2020 2020 2020 636f 756e 7420  ).        count 
-00009a50: 3d20 6c65 6e28 6269 626c 655f 7261 6e67  = len(bible_rang
-00009a60: 6573 290a 2020 2020 2020 2020 6966 2077  es).        if w
-00009a70: 686f 6c65 3a0a 2020 2020 2020 2020 2020  hole:.          
-00009a80: 2020 6966 206e 6f74 2062 6962 6c65 5f72    if not bible_r
-00009a90: 616e 6765 735b 305d 2e69 735f 7768 6f6c  anges[0].is_whol
-00009aa0: 655f 626f 6f6b 2829 3a0a 2020 2020 2020  e_book():.      
-00009ab0: 2020 2020 2020 2020 2020 636f 756e 7420            count 
-00009ac0: 2d3d 2031 0a20 2020 2020 2020 2020 2020  -= 1.           
-00009ad0: 2069 6620 6c65 6e28 6269 626c 655f 7261   if len(bible_ra
-00009ae0: 6e67 6573 2920 3e20 3120 616e 6420 6e6f  nges) > 1 and no
-00009af0: 7420 6269 626c 655f 7261 6e67 6573 5b2d  t bible_ranges[-
-00009b00: 315d 2e69 735f 7768 6f6c 655f 626f 6f6b  1].is_whole_book
-00009b10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00009b20: 2020 2020 636f 756e 7420 2d3d 2031 0a20      count -= 1. 
-00009b30: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-00009b40: 756e 740a 0a20 2020 2064 6566 2063 6861  unt..    def cha
-00009b50: 705f 7261 6e67 6528 7365 6c66 2c20 666c  p_range(self, fl
-00009b60: 6167 733a 2042 6962 6c65 466c 6167 203d  ags: BibleFlag =
-00009b70: 204e 6f6e 6529 202d 3e20 2742 6962 6c65   None) -> 'Bible
-00009b80: 5261 6e67 6527 3a0a 2020 2020 2020 2020  Range':.        
-00009b90: 2727 2752 6574 7572 6e73 2061 206e 6577  '''Returns a new
-00009ba0: 206d 696e 696d 756d 2060 4269 626c 6552   minimum `BibleR
-00009bb0: 616e 6765 6020 7468 6174 2069 6e63 6c75  ange` that inclu
-00009bc0: 6465 7320 7468 6973 2072 616e 6765 2061  des this range a
-00009bd0: 6e64 2062 6567 696e 7320 616e 6420 656e  nd begins and en
-00009be0: 6473 2061 7420 6368 6170 7465 7220 626f  ds at chapter bo
-00009bf0: 756e 6461 7269 6573 2e0a 2020 2020 2020  undaries..      
-00009c00: 2020 0a20 2020 2020 2020 2042 6962 6c65    .        Bible
-00009c10: 466c 6167 2e4d 554c 5449 424f 4f4b 2069  Flag.MULTIBOOK i
-00009c20: 7320 616c 7761 7973 2073 6574 2066 6f72  s always set for
-00009c30: 2074 6869 7320 6d65 7468 6f64 2c20 7265   this method, re
-00009c40: 6761 7264 6c65 7373 206f 6620 7468 6520  gardless of the 
-00009c50: 7661 6c75 6520 6f66 2060 666c 6167 7360  value of `flags`
-00009c60: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00009c70: 2020 2020 2020 666c 6167 7320 3d20 666c        flags = fl
-00009c80: 6167 7320 6f72 2062 6962 6c65 7265 662e  ags or bibleref.
-00009c90: 666c 6167 7320 6f72 2042 6962 6c65 466c  flags or BibleFl
-00009ca0: 6167 2e4e 4f4e 450a 2020 2020 2020 2020  ag.NONE.        
-00009cb0: 666c 6167 7320 7c3d 2042 6962 6c65 466c  flags |= BibleFl
-00009cc0: 6167 2e4d 554c 5449 424f 4f4b 0a20 2020  ag.MULTIBOOK.   
-00009cd0: 2020 2020 2072 6574 7572 6e20 4269 626c       return Bibl
-00009ce0: 6552 616e 6765 2873 7461 7274 3d73 656c  eRange(start=sel
-00009cf0: 662e 7374 6172 742e 6669 7273 745f 7665  f.start.first_ve
-00009d00: 7273 6528 666c 6167 733d 666c 6167 7329  rse(flags=flags)
-00009d10: 2c20 656e 643d 7365 6c66 2e65 6e64 2e6c  , end=self.end.l
-00009d20: 6173 745f 7665 7273 6528 292c 2066 6c61  ast_verse(), fla
-00009d30: 6773 3d66 6c61 6773 290a 0a20 2020 2064  gs=flags)..    d
-00009d40: 6566 2062 6f6f 6b5f 7261 6e67 6528 7365  ef book_range(se
-00009d50: 6c66 2c20 666c 6167 733a 2042 6962 6c65  lf, flags: Bible
-00009d60: 466c 6167 203d 204e 6f6e 6529 202d 3e20  Flag = None) -> 
-00009d70: 2742 6962 6c65 5261 6e67 6527 3a0a 2020  'BibleRange':.  
-00009d80: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
-00009d90: 2061 206e 6577 206d 696e 696d 756d 2060   a new minimum `
-00009da0: 4269 626c 6552 616e 6765 6020 7468 6174  BibleRange` that
-00009db0: 2069 6e63 6c75 6465 7320 7468 6973 2072   includes this r
-00009dc0: 616e 6765 2061 6e64 2062 6567 696e 7320  ange and begins 
-00009dd0: 616e 6420 656e 6473 2061 7420 626f 6f6b  and ends at book
-00009de0: 2062 6f75 6e64 6172 6965 732e 0a20 2020   boundaries..   
-00009df0: 2020 2020 200a 2020 2020 2020 2020 4269       .        Bi
-00009e00: 626c 6546 6c61 672e 4d55 4c54 4942 4f4f  bleFlag.MULTIBOO
-00009e10: 4b20 6973 2061 6c77 6179 7320 7365 7420  K is always set 
-00009e20: 666f 7220 7468 6973 206d 6574 686f 642c  for this method,
-00009e30: 2072 6567 6172 646c 6573 7320 6f66 2074   regardless of t
-00009e40: 6865 2076 616c 7565 206f 6620 6066 6c61  he value of `fla
-00009e50: 6773 602e 0a20 2020 2020 2020 2027 2727  gs`..        '''
-00009e60: 0a20 2020 2020 2020 2066 6c61 6773 203d  .        flags =
-00009e70: 2066 6c61 6773 206f 7220 6269 626c 6572   flags or bibler
-00009e80: 6566 2e66 6c61 6773 206f 7220 4269 626c  ef.flags or Bibl
-00009e90: 6546 6c61 672e 4e4f 4e45 0a20 2020 2020  eFlag.NONE.     
-00009ea0: 2020 2066 6c61 6773 207c 3d20 4269 626c     flags |= Bibl
-00009eb0: 6546 6c61 672e 4d55 4c54 4942 4f4f 4b0a  eFlag.MULTIBOOK.
-00009ec0: 2020 2020 2020 2020 7265 7475 726e 2042          return B
-00009ed0: 6962 6c65 5261 6e67 6528 7374 6172 743d  ibleRange(start=
-00009ee0: 7365 6c66 2e73 7461 7274 2e62 6f6f 6b2e  self.start.book.
-00009ef0: 6669 7273 745f 7665 7273 6528 666c 6167  first_verse(flag
-00009f00: 733d 666c 6167 7329 2c20 656e 643d 7365  s=flags), end=se
-00009f10: 6c66 2e65 6e64 2e62 6f6f 6b2e 6c61 7374  lf.end.book.last
-00009f20: 5f76 6572 7365 2829 2c20 666c 6167 733d  _verse(), flags=
-00009f30: 666c 6167 7329 0a0a 2020 2020 6465 6620  flags)..    def 
-00009f40: 7370 6c69 7428 7365 6c66 2c20 2a2c 2062  split(self, *, b
-00009f50: 795f 626f 6f6b 3a20 626f 6f6c 203d 2046  y_book: bool = F
-00009f60: 616c 7365 2c20 6279 5f63 6861 703a 2062  alse, by_chap: b
-00009f70: 6f6f 6c20 3d20 4661 6c73 652c 206e 756d  ool = False, num
-00009f80: 5f76 6572 7365 733a 2062 6f6f 6c20 3d20  _verses: bool = 
-00009f90: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00009fa0: 2020 2020 7265 6772 6f75 703a 2062 6f6f      regroup: boo
-00009fb0: 6c20 3d20 5472 7565 2c20 666c 6167 733a  l = True, flags:
-00009fc0: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-00009fd0: 6529 202d 3e20 2742 6962 6c65 5261 6e67  e) -> 'BibleRang
-00009fe0: 654c 6973 7427 3a0a 2020 2020 2020 2020  eList':.        
-00009ff0: 2727 2753 706c 6974 2074 6869 7320 6042  '''Split this `B
-0000a000: 6962 6c65 5261 6e67 6560 2069 6e74 6f20  ibleRange` into 
-0000a010: 6120 6042 6962 6c65 5261 6e67 654c 6973  a `BibleRangeLis
-0000a020: 7460 206f 6620 736d 616c 6c65 7220 636f  t` of smaller co
-0000a030: 6e73 6563 7574 6976 6520 7261 6e67 6573  nsecutive ranges
-0000a040: 2c20 6173 2066 6f6c 6c6f 7773 3a0a 2020  , as follows:.  
-0000a050: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-0000a060: 2049 6620 6062 795f 626f 6f6b 6020 6973   If `by_book` is
-0000a070: 2060 5472 7565 602c 2073 706c 6974 7320   `True`, splits 
-0000a080: 6172 6520 6d61 6465 2061 7420 7468 6520  are made at the 
-0000a090: 656e 6420 6f66 2065 6163 6820 626f 6f6b  end of each book
-0000a0a0: 2e0a 2020 2020 2020 2020 2d20 4966 2060  ..        - If `
-0000a0b0: 6279 5f63 6861 7060 2069 7320 6054 7275  by_chap` is `Tru
-0000a0c0: 6560 2c20 7370 6c69 7473 2061 7265 206d  e`, splits are m
-0000a0d0: 6164 6520 656e 6420 6f66 2065 6163 6820  ade end of each 
-0000a0e0: 6368 6170 7465 722e 0a20 2020 2020 2020  chapter..       
-0000a0f0: 202d 2049 6620 606e 756d 5f76 6572 7365   - If `num_verse
-0000a100: 7360 2069 7320 7370 6563 6966 6965 642c  s` is specified,
-0000a110: 2073 706c 6974 7320 6172 6520 6d61 6465   splits are made
-0000a120: 2061 6674 6572 2028 6e6f 206d 6f72 6520   after (no more 
-0000a130: 7468 616e 2920 7468 6520 7370 6563 6966  than) the specif
-0000a140: 6965 6420 6e75 6d62 6572 206f 6620 7665  ied number of ve
-0000a150: 7273 6573 2e0a 2020 2020 2020 2020 2d20  rses..        - 
-0000a160: 6062 795f 626f 6f6b 602c 2060 6279 5f63  `by_book`, `by_c
-0000a170: 6861 7060 2061 6e64 2060 6e75 6d5f 7665  hap` and `num_ve
-0000a180: 7273 6573 6020 6361 6e20 6265 2073 6574  rses` can be set
-0000a190: 2069 6e20 616e 7920 636f 6d62 696e 6174   in any combinat
-0000a1a0: 696f 6e2e 2049 6620 6e6f 6e65 206f 6620  ion. If none of 
-0000a1b0: 7468 656d 2061 7265 2073 6574 2c20 7468  them are set, th
-0000a1c0: 6520 7265 7375 6c74 696e 670a 2020 2020  e resulting.    
-0000a1d0: 2020 2020 2020 6042 6962 6c65 5261 6e67        `BibleRang
-0000a1e0: 654c 6973 7460 2077 696c 6c20 636f 6e74  eList` will cont
-0000a1f0: 6169 6e20 7468 6973 2072 616e 6765 206f  ain this range o
-0000a200: 6e6c 792e 0a20 2020 2020 2020 202d 2049  nly..        - I
-0000a210: 6620 6072 6567 726f 7570 6020 6973 2060  f `regroup` is `
-0000a220: 5472 7565 602c 2072 6567 726f 7570 2829  True`, regroup()
-0000a230: 2069 7320 6361 6c6c 6564 206f 6e20 7468   is called on th
-0000a240: 6520 7265 7375 6c74 696e 6720 6042 6962  e resulting `Bib
-0000a250: 6c65 5261 6e67 654c 6973 7460 2e0a 2020  leRangeList`..  
-0000a260: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000a270: 2020 666c 6167 7320 3d20 666c 6167 7320    flags = flags 
-0000a280: 6f72 2062 6962 6c65 7265 662e 666c 6167  or bibleref.flag
-0000a290: 7320 6f72 2042 6962 6c65 466c 6167 2e4e  s or BibleFlag.N
-0000a2a0: 4f4e 450a 2020 2020 2020 2020 2320 5365  ONE.        # Se
-0000a2b0: 7420 666c 6167 7320 6966 206f 7572 2061  t flags if our a
-0000a2c0: 7474 7269 6275 7465 7320 696d 706c 7920  ttributes imply 
-0000a2d0: 7468 6579 2073 686f 756c 6420 6265 2073  they should be s
-0000a2e0: 6574 0a20 2020 2020 2020 2069 6620 7365  et.        if se
-0000a2f0: 6c66 2e73 7461 7274 2e62 6f6f 6b20 213d  lf.start.book !=
-0000a300: 2073 656c 662e 656e 642e 626f 6f6b 3a0a   self.end.book:.
-0000a310: 2020 2020 2020 2020 2020 2020 666c 6167              flag
-0000a320: 7320 7c3d 2042 6962 6c65 466c 6167 2e4d  s |= BibleFlag.M
-0000a330: 554c 5449 424f 4f4b 0a20 2020 2020 2020  ULTIBOOK.       
-0000a340: 2069 6620 7365 6c66 2e73 7461 7274 2e76   if self.start.v
-0000a350: 6572 7365 5f6e 756d 203d 3d20 3020 6f72  erse_num == 0 or
-0000a360: 2073 656c 662e 656e 642e 7665 7273 655f   self.end.verse_
-0000a370: 6e75 6d20 3d3d 2030 3a0a 2020 2020 2020  num == 0:.      
-0000a380: 2020 2020 2020 666c 6167 7320 7c3d 2042        flags |= B
-0000a390: 6962 6c65 466c 6167 2e56 4552 5345 5f30  ibleFlag.VERSE_0
-0000a3a0: 0a0a 2020 2020 2020 2020 7370 6c69 745f  ..        split_
-0000a3b0: 7265 7375 6c74 203d 205b 7365 6c66 5d0a  result = [self].
-0000a3c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000a3d0: 2069 6620 6279 5f62 6f6f 6b3a 0a20 2020   if by_book:.   
-0000a3e0: 2020 2020 2020 2020 206e 6577 5f73 706c           new_spl
-0000a3f0: 6974 203d 205b 5d0a 2020 2020 2020 2020  it = [].        
-0000a400: 2020 2020 666f 7220 7261 6e67 655f 746f      for range_to
-0000a410: 5f73 706c 6974 2069 6e20 7370 6c69 745f  _split in split_
-0000a420: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
-0000a430: 2020 2020 2020 2020 7261 6e67 655f 7374          range_st
-0000a440: 6172 7420 3d20 7261 6e67 655f 746f 5f73  art = range_to_s
-0000a450: 706c 6974 2e73 7461 7274 0a20 2020 2020  plit.start.     
-0000a460: 2020 2020 2020 2020 2020 2072 616e 6765             range
-0000a470: 5f65 6e64 203d 2072 616e 6765 5f73 7461  _end = range_sta
-0000a480: 7274 2e62 6f6f 6b2e 6c61 7374 5f76 6572  rt.book.last_ver
-0000a490: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-0000a4a0: 2020 2020 2077 6869 6c65 2072 616e 6765       while range
-0000a4b0: 5f65 6e64 203c 2072 616e 6765 5f74 6f5f  _end < range_to_
-0000a4c0: 7370 6c69 742e 656e 643a 0a20 2020 2020  split.end:.     
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000a4e0: 6577 5f73 706c 6974 2e61 7070 656e 6428  ew_split.append(
-0000a4f0: 4269 626c 6552 616e 6765 2873 7461 7274  BibleRange(start
-0000a500: 3d72 616e 6765 5f73 7461 7274 2c20 656e  =range_start, en
-0000a510: 643d 7261 6e67 655f 656e 642c 2066 6c61  d=range_end, fla
-0000a520: 6773 3d66 6c61 6773 2929 0a20 2020 2020  gs=flags)).     
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a540: 616e 6765 5f73 7461 7274 203d 2072 616e  ange_start = ran
-0000a550: 6765 5f65 6e64 2e61 6464 2831 2c20 666c  ge_end.add(1, fl
-0000a560: 6167 733d 666c 6167 7329 0a20 2020 2020  ags=flags).     
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a580: 616e 6765 5f65 6e64 203d 2072 616e 6765  ange_end = range
-0000a590: 5f73 7461 7274 2e62 6f6f 6b2e 6c61 7374  _start.book.last
-0000a5a0: 5f76 6572 7365 2829 0a20 2020 2020 2020  _verse().       
-0000a5b0: 2020 2020 2020 2020 206e 6577 5f73 706c           new_spl
-0000a5c0: 6974 2e61 7070 656e 6428 4269 626c 6552  it.append(BibleR
-0000a5d0: 616e 6765 2873 7461 7274 3d72 616e 6765  ange(start=range
-0000a5e0: 5f73 7461 7274 2c20 656e 643d 7261 6e67  _start, end=rang
-0000a5f0: 655f 746f 5f73 706c 6974 2e65 6e64 2c20  e_to_split.end, 
-0000a600: 666c 6167 733d 666c 6167 7329 290a 2020  flags=flags)).  
-0000a610: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
-0000a620: 7265 7375 6c74 203d 206e 6577 5f73 706c  result = new_spl
-0000a630: 6974 0a0a 2020 2020 2020 2020 6966 2062  it..        if b
-0000a640: 795f 6368 6170 3a0a 2020 2020 2020 2020  y_chap:.        
-0000a650: 2020 2020 6e65 775f 7370 6c69 7420 3d20      new_split = 
-0000a660: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0000a670: 6f72 2072 616e 6765 5f74 6f5f 7370 6c69  or range_to_spli
-0000a680: 7420 696e 2073 706c 6974 5f72 6573 756c  t in split_resul
-0000a690: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000a6a0: 2020 2072 616e 6765 5f73 7461 7274 203d     range_start =
-0000a6b0: 2072 616e 6765 5f74 6f5f 7370 6c69 742e   range_to_split.
-0000a6c0: 7374 6172 740a 2020 2020 2020 2020 2020  start.          
-0000a6d0: 2020 2020 2020 7261 6e67 655f 656e 6420        range_end 
-0000a6e0: 3d20 7261 6e67 655f 7374 6172 742e 6c61  = range_start.la
-0000a6f0: 7374 5f76 6572 7365 2829 0a20 2020 2020  st_verse().     
-0000a700: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-0000a710: 2072 616e 6765 5f65 6e64 203c 2072 616e   range_end < ran
-0000a720: 6765 5f74 6f5f 7370 6c69 742e 656e 643a  ge_to_split.end:
-0000a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a740: 2020 2020 206e 6577 5f73 706c 6974 2e61       new_split.a
-0000a750: 7070 656e 6428 4269 626c 6552 616e 6765  ppend(BibleRange
-0000a760: 2873 7461 7274 3d72 616e 6765 5f73 7461  (start=range_sta
-0000a770: 7274 2c20 656e 643d 7261 6e67 655f 656e  rt, end=range_en
-0000a780: 642c 2066 6c61 6773 3d66 6c61 6773 2929  d, flags=flags))
-0000a790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7a0: 2020 2020 2072 616e 6765 5f73 7461 7274       range_start
-0000a7b0: 203d 2072 616e 6765 5f65 6e64 2e61 6464   = range_end.add
-0000a7c0: 2831 2c20 666c 6167 733d 666c 6167 7329  (1, flags=flags)
-0000a7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7e0: 2020 2020 2072 616e 6765 5f65 6e64 203d       range_end =
-0000a7f0: 2072 616e 6765 5f73 7461 7274 2e6c 6173   range_start.las
-0000a800: 745f 7665 7273 6528 290a 2020 2020 2020  t_verse().      
-0000a810: 2020 2020 2020 2020 2020 6e65 775f 7370            new_sp
-0000a820: 6c69 742e 6170 7065 6e64 2842 6962 6c65  lit.append(Bible
-0000a830: 5261 6e67 6528 7374 6172 743d 7261 6e67  Range(start=rang
-0000a840: 655f 7374 6172 742c 2065 6e64 3d72 616e  e_start, end=ran
-0000a850: 6765 5f74 6f5f 7370 6c69 742e 656e 642c  ge_to_split.end,
-0000a860: 2066 6c61 6773 3d66 6c61 6773 2929 0a20   flags=flags)). 
-0000a870: 2020 2020 2020 2020 2020 2073 706c 6974             split
-0000a880: 5f72 6573 756c 7420 3d20 6e65 775f 7370  _result = new_sp
-0000a890: 6c69 740a 0a20 2020 2020 2020 2069 6620  lit..        if 
-0000a8a0: 6e75 6d5f 7665 7273 6573 2069 7320 6e6f  num_verses is no
-0000a8b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000a8c0: 2020 2020 6e65 775f 7370 6c69 7420 3d20      new_split = 
-0000a8d0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0000a8e0: 6f72 2072 616e 6765 5f74 6f5f 7370 6c69  or range_to_spli
-0000a8f0: 7420 696e 2073 706c 6974 5f72 6573 756c  t in split_resul
-0000a900: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000a910: 2020 2072 616e 6765 5f73 7461 7274 203d     range_start =
-0000a920: 2042 6962 6c65 5665 7273 6528 7261 6e67   BibleVerse(rang
-0000a930: 655f 746f 5f73 706c 6974 2e73 7461 7274  e_to_split.start
-0000a940: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a960: 616e 6765 5f65 6e64 203d 2072 616e 6765  ange_end = range
-0000a970: 5f73 7461 7274 2e61 6464 286e 756d 5f76  _start.add(num_v
-0000a980: 6572 7365 7320 2d20 312c 2066 6c61 6773  erses - 1, flags
-0000a990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a9a0: 2020 7768 696c 6520 7261 6e67 655f 656e    while range_en
-0000a9b0: 6420 6973 206e 6f74 204e 6f6e 6520 616e  d is not None an
-0000a9c0: 6420 7261 6e67 655f 656e 6420 3c20 7261  d range_end < ra
-0000a9d0: 6e67 655f 746f 5f73 706c 6974 2e65 6e64  nge_to_split.end
-0000a9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a9f0: 2020 2020 2020 6e65 775f 7370 6c69 742e        new_split.
-0000aa00: 6170 7065 6e64 2842 6962 6c65 5261 6e67  append(BibleRang
-0000aa10: 6528 7374 6172 743d 7261 6e67 655f 7374  e(start=range_st
-0000aa20: 6172 742c 2065 6e64 3d72 616e 6765 5f65  art, end=range_e
-0000aa30: 6e64 2c20 666c 6167 733d 666c 6167 7329  nd, flags=flags)
-0000aa40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000aa50: 2020 2020 2020 7261 6e67 655f 7374 6172        range_star
-0000aa60: 7420 3d20 7261 6e67 655f 656e 642e 6164  t = range_end.ad
-0000aa70: 6428 312c 2066 6c61 6773 290a 2020 2020  d(1, flags).    
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 7261 6e67 655f 656e 6420 3d20 7261 6e67  range_end = rang
-0000aaa0: 655f 656e 642e 6164 6428 6e75 6d5f 7665  e_end.add(num_ve
-0000aab0: 7273 6573 2c20 666c 6167 7329 0a20 2020  rses, flags).   
-0000aac0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000aad0: 5f73 706c 6974 2e61 7070 656e 6428 4269  _split.append(Bi
-0000aae0: 626c 6552 616e 6765 2873 7461 7274 3d72  bleRange(start=r
-0000aaf0: 616e 6765 5f73 7461 7274 2c20 656e 643d  ange_start, end=
-0000ab00: 7261 6e67 655f 746f 5f73 706c 6974 2e65  range_to_split.e
-0000ab10: 6e64 2c20 666c 6167 733d 666c 6167 7329  nd, flags=flags)
-0000ab20: 290a 2020 2020 2020 2020 2020 2020 7370  ).            sp
-0000ab30: 6c69 745f 7265 7375 6c74 203d 206e 6577  lit_result = new
-0000ab40: 5f73 706c 6974 0a20 2020 2020 2020 200a  _split.        .
-0000ab50: 2020 2020 2020 2020 7261 6e67 655f 6c69          range_li
-0000ab60: 7374 203d 2042 6962 6c65 5261 6e67 654c  st = BibleRangeL
-0000ab70: 6973 7428 7370 6c69 745f 7265 7375 6c74  ist(split_result
-0000ab80: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
-0000ab90: 2020 2020 2020 2069 6620 7265 6772 6f75         if regrou
-0000aba0: 703a 0a20 2020 2020 2020 2020 2020 2072  p:.            r
-0000abb0: 616e 6765 5f6c 6973 742e 7265 6772 6f75  ange_list.regrou
-0000abc0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0000abd0: 726e 2072 616e 6765 5f6c 6973 740a 0a20  rn range_list.. 
-0000abe0: 2020 2064 6566 2069 735f 6469 736a 6f69     def is_disjoi
-0000abf0: 6e74 2873 656c 662c 206f 7468 6572 5f72  nt(self, other_r
-0000ac00: 6566 3a20 2742 6962 6c65 5265 6627 2920  ef: 'BibleRef') 
-0000ac10: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000ac20: 2027 2727 5265 7475 726e 7320 6054 7275   '''Returns `Tru
-0000ac30: 6560 2069 6620 7468 6973 2072 616e 6765  e` if this range
-0000ac40: 2064 6f65 736e 2774 206f 7665 726c 6170   doesn't overlap
-0000ac50: 2077 6974 6820 616e 7920 7665 7273 6573   with any verses
-0000ac60: 2069 6e20 606f 7468 6572 5f72 6566 602c   in `other_ref`,
-0000ac70: 206f 7468 6572 7769 7365 2060 4661 6c73   otherwise `Fals
-0000ac80: 6560 2e0a 2020 2020 2020 2020 2727 270a  e`..        '''.
-0000ac90: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000aca0: 7461 6e63 6528 6f74 6865 725f 7265 662c  tance(other_ref,
-0000acb0: 2042 6962 6c65 5261 6e67 654c 6973 7429   BibleRangeList)
-0000acc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000acd0: 7475 726e 206f 7468 6572 5f72 6566 2e69  turn other_ref.i
-0000ace0: 735f 6469 736a 6f69 6e74 2873 656c 6629  s_disjoint(self)
-0000acf0: 2023 2069 735f 6469 736a 6f69 6e74 2829   # is_disjoint()
-0000ad00: 2069 7320 636f 6d6d 7574 6174 6976 652c   is commutative,
-0000ad10: 2073 6f20 7573 6520 7468 6520 6c69 7374   so use the list
-0000ad20: 2069 6d70 6c65 6d65 6e74 6174 696f 6e0a   implementation.
-0000ad30: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000ad40: 7461 6e63 6528 6f74 6865 725f 7265 662c  tance(other_ref,
-0000ad50: 2042 6962 6c65 5665 7273 6529 3a0a 2020   BibleVerse):.  
-0000ad60: 2020 2020 2020 2020 2020 2320 436f 6e76            # Conv
-0000ad70: 6572 7420 746f 2042 6962 6c65 5261 6e67  ert to BibleRang
-0000ad80: 6520 2861 6e64 2077 6520 646f 6e27 7420  e (and we don't 
-0000ad90: 656e 666f 7263 6520 6578 6973 7469 6e67  enforce existing
-0000ada0: 2066 6c61 6773 2066 6f72 2063 6f6e 7665   flags for conve
-0000adb0: 7273 696f 6e73 290a 2020 2020 2020 2020  rsions).        
-0000adc0: 2020 2020 6f74 6865 725f 7265 6620 3d20      other_ref = 
-0000add0: 4269 626c 6552 616e 6765 2873 7461 7274  BibleRange(start
-0000ade0: 3d6f 7468 6572 5f72 6566 2c20 656e 643d  =other_ref, end=
-0000adf0: 6f74 6865 725f 7265 662c 2066 6c61 6773  other_ref, flags
-0000ae00: 3d42 6962 6c65 466c 6167 2e41 4c4c 290a  =BibleFlag.ALL).
-0000ae10: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000ae20: 7461 6e63 6528 6f74 6865 725f 7265 662c  tance(other_ref,
-0000ae30: 2042 6962 6c65 5261 6e67 6529 3a0a 2020   BibleRange):.  
-0000ae40: 2020 2020 2020 2020 2020 6c6f 7765 722c            lower,
-0000ae50: 2068 6967 6865 7220 3d20 2873 656c 662c   higher = (self,
-0000ae60: 206f 7468 6572 5f72 6566 2920 6966 2073   other_ref) if s
-0000ae70: 656c 6620 3c20 6f74 6865 725f 7265 6620  elf < other_ref 
-0000ae80: 656c 7365 2028 6f74 6865 725f 7265 662c  else (other_ref,
-0000ae90: 2073 656c 6629 0a20 2020 2020 2020 2020   self).         
-0000aea0: 2020 2072 6574 7572 6e20 6c6f 7765 722e     return lower.
-0000aeb0: 656e 6420 3c20 6869 6768 6572 2e73 7461  end < higher.sta
-0000aec0: 7274 0a20 2020 2020 2020 2065 6c73 653a  rt.        else:
-0000aed0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000aee0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
-0000aef0: 7b6f 7468 6572 5f72 6566 7d20 6973 206e  {other_ref} is n
-0000af00: 6f74 2061 2076 616c 6964 2042 6962 6c65  ot a valid Bible
-0000af10: 5265 6622 290a 0a20 2020 2064 6566 2069  Ref")..    def i
-0000af20: 735f 6164 6a61 6365 6e74 2873 656c 662c  s_adjacent(self,
-0000af30: 206f 7468 6572 5f72 6566 3a20 2742 6962   other_ref: 'Bib
-0000af40: 6c65 5265 6627 2c20 666c 6167 733a 2042  leRef', flags: B
-0000af50: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-0000af60: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000af70: 2020 2727 2752 6574 7572 6e73 2060 5472    '''Returns `Tr
-0000af80: 7565 6020 6966 2074 6869 7320 7261 6e67  ue` if this rang
-0000af90: 6520 6973 2061 646a 6163 656e 7420 746f  e is adjacent to
-0000afa0: 2060 6f74 6865 725f 7265 6660 2c20 6f74   `other_ref`, ot
-0000afb0: 6865 7277 6973 6520 6046 616c 7365 602e  herwise `False`.
-0000afc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000afd0: 2020 4120 6042 6962 6c65 5261 6e67 6560    A `BibleRange`
-0000afe0: 2069 7320 636f 6e73 6964 6572 6564 2061   is considered a
-0000aff0: 646a 6163 656e 7420 746f 2061 6e6f 7468  djacent to anoth
-0000b000: 6572 2060 4269 626c 6556 6572 7365 6020  er `BibleVerse` 
-0000b010: 6f72 2060 4269 626c 6552 616e 6765 6020  or `BibleRange` 
-0000b020: 6966 2074 6865 6972 2062 6f75 6e64 7320  if their bounds 
-0000b030: 6172 6520 6120 7369 6e67 6c65 0a20 2020  are a single.   
-0000b040: 2020 2020 2076 6572 7365 2061 7061 7274       verse apart
-0000b050: 2e20 4120 6042 6962 6c65 5261 6e67 6560  . A `BibleRange`
-0000b060: 2069 7320 636f 6e73 6964 6572 6564 2061   is considered a
-0000b070: 646a 6163 656e 7420 746f 2061 2060 4269  djacent to a `Bi
-0000b080: 626c 6552 616e 6765 4c69 7374 6020 6966  bleRangeList` if
-0000b090: 2069 7420 6973 2064 6973 6a6f 696e 740a   it is disjoint.
-0000b0a0: 2020 2020 2020 2020 746f 2074 6865 2065          to the e
-0000b0b0: 6e74 6972 6520 6c69 7374 2061 6e64 2061  ntire list and a
-0000b0c0: 646a 6163 656e 7420 746f 2061 7420 6c65  djacent to at le
-0000b0d0: 6173 7420 6f6e 6520 6042 6962 6c65 5261  ast one `BibleRa
-0000b0e0: 6e67 6560 2069 6e20 7468 6520 6c69 7374  nge` in the list
-0000b0f0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-0000b100: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000b110: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
-0000b120: 6962 6c65 5261 6e67 654c 6973 7429 3a0a  ibleRangeList):.
-0000b130: 2020 2020 2020 2020 2020 2020 2320 4269              # Bi
-0000b140: 626c 6552 616e 6765 4c69 7374 2064 6f65  bleRangeList doe
-0000b150: 736e 2774 2064 6566 696e 6520 6973 5f61  sn't define is_a
-0000b160: 646a 6163 656e 7428 292c 2073 6f20 7765  djacent(), so we
-0000b170: 2068 6176 6520 746f 2069 6d70 6c65 6d65   have to impleme
-0000b180: 6e74 2068 6572 650a 2020 2020 2020 2020  nt here.        
-0000b190: 2020 2020 7265 7475 726e 206f 7468 6572      return other
-0000b1a0: 5f72 6566 2e69 735f 6469 736a 6f69 6e74  _ref.is_disjoint
-0000b1b0: 2873 656c 6629 2061 6e64 205c 0a20 2020  (self) and \.   
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 616e 7928 7365 6c66 2e69 735f 6164 6a61  any(self.is_adja
-0000b1e0: 6365 6e74 286f 7468 6572 5f72 616e 6765  cent(other_range
-0000b1f0: 2920 666f 7220 6f74 6865 725f 7261 6e67  ) for other_rang
-0000b200: 6520 696e 206f 7468 6572 5f72 6566 2920  e in other_ref) 
-0000b210: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000b220: 7374 616e 6365 286f 7468 6572 5f72 6566  stance(other_ref
-0000b230: 2c20 4269 626c 6556 6572 7365 293a 0a20  , BibleVerse):. 
-0000b240: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
-0000b250: 7665 7274 2074 6f20 4269 626c 6552 616e  vert to BibleRan
-0000b260: 6765 2028 616e 6420 7765 2064 6f6e 2774  ge (and we don't
-0000b270: 2065 6e66 6f72 6365 2065 7869 7374 696e   enforce existin
-0000b280: 6720 666c 6167 7320 666f 7220 636f 6e76  g flags for conv
-0000b290: 6572 7369 6f6e 7329 0a20 2020 2020 2020  ersions).       
-0000b2a0: 2020 2020 206f 7468 6572 5f72 6566 203d       other_ref =
-0000b2b0: 2042 6962 6c65 5261 6e67 6528 7374 6172   BibleRange(star
-0000b2c0: 743d 6f74 6865 725f 7265 662c 2065 6e64  t=other_ref, end
-0000b2d0: 3d6f 7468 6572 5f72 6566 2c20 666c 6167  =other_ref, flag
-0000b2e0: 733d 4269 626c 6546 6c61 672e 414c 4c29  s=BibleFlag.ALL)
-0000b2f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000b300: 7374 616e 6365 286f 7468 6572 5f72 6566  stance(other_ref
-0000b310: 2c20 4269 626c 6552 616e 6765 293a 2020  , BibleRange):  
-0000b320: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0000b330: 2020 206c 6f77 6572 2c20 6869 6768 6572     lower, higher
-0000b340: 203d 2028 7365 6c66 2c20 6f74 6865 725f   = (self, other_
-0000b350: 7265 6629 2069 6620 7365 6c66 203c 206f  ref) if self < o
-0000b360: 7468 6572 5f72 6566 2065 6c73 6520 286f  ther_ref else (o
-0000b370: 7468 6572 5f72 6566 2c20 7365 6c66 290a  ther_ref, self).
-0000b380: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b390: 726e 2028 6c6f 7765 722e 656e 642e 6164  rn (lower.end.ad
-0000b3a0: 6428 312c 2066 6c61 6773 3d66 6c61 6773  d(1, flags=flags
-0000b3b0: 2920 3d3d 2068 6967 6865 722e 7374 6172  ) == higher.star
-0000b3c0: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
-0000b3d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000b3e0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
-0000b3f0: 7b6f 7468 6572 5f72 6566 7d20 6973 206e  {other_ref} is n
-0000b400: 6f74 2061 2076 616c 6964 2042 6962 6c65  ot a valid Bible
-0000b410: 5265 6622 290a 0a20 2020 2064 6566 2063  Ref")..    def c
-0000b420: 6f6e 7461 696e 7328 7365 6c66 2c20 6f74  ontains(self, ot
-0000b430: 6865 725f 7265 663a 2027 4269 626c 6552  her_ref: 'BibleR
-0000b440: 6566 2729 202d 3e20 626f 6f6c 3a0a 2020  ef') -> bool:.  
-0000b450: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
-0000b460: 2060 5472 7565 6020 6966 2061 6c6c 2074   `True` if all t
-0000b470: 6865 2076 6572 7365 7320 696e 2060 6f74  he verses in `ot
-0000b480: 6865 725f 7265 6660 2066 616c 6c20 7769  her_ref` fall wi
-0000b490: 7468 696e 2074 6869 7320 6042 6962 6c65  thin this `Bible
-0000b4a0: 5261 6e67 6560 2e20 4f74 6865 7277 6973  Range`. Otherwis
-0000b4b0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000b4c0: 7320 6046 616c 7365 602e 0a0a 2020 2020  s `False`...    
-0000b4d0: 2020 2020 5468 6520 7361 6d65 2072 6573      The same res
-0000b4e0: 756c 7420 6973 2072 6574 7572 6e65 6420  ult is returned 
-0000b4f0: 7573 696e 6720 7468 6520 2769 6e27 206f  using the 'in' o
-0000b500: 7065 7261 746f 7220 2869 2e65 2e20 606f  perator (i.e. `o
-0000b510: 7468 6572 5f72 6566 2069 6e20 6269 626c  ther_ref in bibl
-0000b520: 655f 7261 6e67 6560 292e 0a20 2020 2020  e_range`)..     
-0000b530: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-0000b540: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-0000b550: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
-0000b560: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
-0000b570: 2020 2020 2023 2063 6f6e 7461 696e 7328       # contains(
-0000b580: 2920 6973 206e 6f74 2063 6f6d 6d75 7461  ) is not commuta
-0000b590: 7469 7665 2c20 6275 7420 7765 2073 7469  tive, but we sti
-0000b5a0: 6c6c 2075 7365 2074 6865 2042 6962 6c65  ll use the Bible
-0000b5b0: 5261 6e67 654c 6973 7420 696d 706c 656d  RangeList implem
-0000b5c0: 656e 7461 7469 6f6e 2e0a 2020 2020 2020  entation..      
-0000b5d0: 2020 2020 2020 7265 7475 726e 2042 6962        return Bib
-0000b5e0: 6c65 5261 6e67 654c 6973 7428 5b73 656c  leRangeList([sel
-0000b5f0: 665d 292e 636f 6e74 6169 6e73 286f 7468  f]).contains(oth
-0000b600: 6572 5f72 6566 290a 2020 2020 2020 2020  er_ref).        
-0000b610: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-0000b620: 6865 725f 7265 662c 2042 6962 6c65 5665  her_ref, BibleVe
-0000b630: 7273 6529 3a0a 2020 2020 2020 2020 2020  rse):.          
-0000b640: 2020 2320 436f 6e76 6572 7420 746f 2042    # Convert to B
-0000b650: 6962 6c65 5261 6e67 6520 2861 6e64 2077  ibleRange (and w
-0000b660: 6520 646f 6e27 7420 656e 666f 7263 6520  e don't enforce 
-0000b670: 6578 6973 7469 6e67 2066 6c61 6773 2066  existing flags f
-0000b680: 6f72 2063 6f6e 7665 7273 696f 6e73 290a  or conversions).
-0000b690: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000b6a0: 725f 7265 6620 3d20 4269 626c 6552 616e  r_ref = BibleRan
-0000b6b0: 6765 2873 7461 7274 3d6f 7468 6572 5f72  ge(start=other_r
-0000b6c0: 6566 2c20 656e 643d 6f74 6865 725f 7265  ef, end=other_re
-0000b6d0: 662c 2066 6c61 6773 3d42 6962 6c65 466c  f, flags=BibleFl
-0000b6e0: 6167 2e41 4c4c 290a 2020 2020 2020 2020  ag.ALL).        
-0000b6f0: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-0000b700: 6865 725f 7265 662c 2042 6962 6c65 5261  her_ref, BibleRa
-0000b710: 6e67 6529 3a0a 2020 2020 2020 2020 2020  nge):.          
-0000b720: 2020 7265 7475 726e 2028 6f74 6865 725f    return (other_
-0000b730: 7265 662e 7374 6172 7420 3e3d 2073 656c  ref.start >= sel
-0000b740: 662e 7374 6172 7420 616e 6420 6f74 6865  f.start and othe
-0000b750: 725f 7265 662e 7374 6172 7420 3c3d 2073  r_ref.start <= s
-0000b760: 656c 662e 656e 6429 2061 6e64 205c 0a20  elf.end) and \. 
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 286f 7468 6572 5f72 6566 2e65 6e64    (other_ref.end
-0000b790: 203e 3d20 7365 6c66 2e73 7461 7274 2061   >= self.start a
-0000b7a0: 6e64 206f 7468 6572 5f72 6566 2e65 6e64  nd other_ref.end
-0000b7b0: 203c 3d20 7365 6c66 2e65 6e64 290a 2020   <= self.end).  
-0000b7c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000b7d0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000b7e0: 6c75 6545 7272 6f72 2866 227b 6f74 6865  lueError(f"{othe
-0000b7f0: 725f 7265 667d 2069 7320 6e6f 7420 6120  r_ref} is not a 
-0000b800: 7661 6c69 6420 4269 626c 6552 6566 2229  valid BibleRef")
-0000b810: 0a0a 2020 2020 6465 6620 7375 7272 6f75  ..    def surrou
-0000b820: 6e64 7328 7365 6c66 2c20 6f74 6865 725f  nds(self, other_
-0000b830: 7265 663a 2027 4269 626c 6552 6566 2729  ref: 'BibleRef')
-0000b840: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000b850: 2020 2727 2752 6574 7572 6e73 2060 5472    '''Returns `Tr
-0000b860: 7565 6020 6966 2061 6c6c 2074 6865 2076  ue` if all the v
-0000b870: 6572 7365 7320 696e 2060 6f74 6865 725f  erses in `other_
-0000b880: 7265 6660 2066 616c 6c20 7769 7468 696e  ref` fall within
-0000b890: 2074 6869 7320 6042 6962 6c65 5261 6e67   this `BibleRang
-0000b8a0: 6560 2c20 2a77 6974 686f 7574 2a0a 2020  e`, *without*.  
-0000b8b0: 2020 2020 2020 696e 636c 7564 696e 6720        including 
-0000b8c0: 7468 6973 2072 616e 6765 2773 2060 7374  this range's `st
-0000b8d0: 6172 7460 206f 7220 6065 6e64 6020 6042  art` or `end` `B
-0000b8e0: 6962 6c65 5665 7273 6560 2e20 4f74 6865  ibleVerse`. Othe
-0000b8f0: 7277 6973 652c 2072 6574 7572 6e73 2060  rwise, returns `
-0000b900: 4661 6c73 6560 2e0a 2020 2020 2020 2020  False`..        
-0000b910: 2727 270a 2020 2020 2020 2020 6966 2069  '''.        if i
-0000b920: 7369 6e73 7461 6e63 6528 6f74 6865 725f  sinstance(other_
-0000b930: 7265 662c 2042 6962 6c65 5261 6e67 654c  ref, BibleRangeL
-0000b940: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-0000b950: 2020 2320 4269 626c 6552 616e 6765 4c69    # BibleRangeLi
-0000b960: 7374 2064 6f65 736e 2774 2064 6566 696e  st doesn't defin
-0000b970: 6520 7375 7272 6f75 6e64 7328 292c 2073  e surrounds(), s
-0000b980: 6f20 7765 2068 6176 6520 746f 2069 6d70  o we have to imp
-0000b990: 6c65 6d65 6e74 2068 6572 650a 2020 2020  lement here.    
-0000b9a0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0000b9b0: 6c6c 2873 656c 662e 7375 7272 6f75 6e64  ll(self.surround
-0000b9c0: 7328 6f74 6865 725f 7261 6e67 6529 2066  s(other_range) f
-0000b9d0: 6f72 206f 7468 6572 5f72 616e 6765 2069  or other_range i
-0000b9e0: 6e20 6f74 6865 725f 7265 6629 200a 2020  n other_ref) .  
-0000b9f0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000ba00: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
-0000ba10: 6962 6c65 5665 7273 6529 3a0a 2020 2020  ibleVerse):.    
-0000ba20: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-0000ba30: 7420 746f 2042 6962 6c65 5261 6e67 6520  t to BibleRange 
-0000ba40: 2861 6e64 2077 6520 646f 6e27 7420 656e  (and we don't en
-0000ba50: 666f 7263 6520 6578 6973 7469 6e67 2066  force existing f
-0000ba60: 6c61 6773 2066 6f72 2063 6f6e 7665 7273  lags for convers
-0000ba70: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
-0000ba80: 2020 6f74 6865 725f 7265 6620 3d20 4269    other_ref = Bi
-0000ba90: 626c 6552 616e 6765 2873 7461 7274 3d6f  bleRange(start=o
-0000baa0: 7468 6572 5f72 6566 2c20 656e 643d 6f74  ther_ref, end=ot
-0000bab0: 6865 725f 7265 662c 2066 6c61 6773 3d42  her_ref, flags=B
-0000bac0: 6962 6c65 466c 6167 2e41 4c4c 290a 2020  ibleFlag.ALL).  
-0000bad0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000bae0: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
-0000baf0: 6962 6c65 5261 6e67 6529 3a0a 2020 2020  ibleRange):.    
-0000bb00: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0000bb10: 6f74 6865 725f 7265 662e 7374 6172 7420  other_ref.start 
-0000bb20: 3e20 7365 6c66 2e73 7461 7274 2061 6e64  > self.start and
-0000bb30: 206f 7468 6572 5f72 6566 2e73 7461 7274   other_ref.start
-0000bb40: 203c 2073 656c 662e 656e 6429 2061 6e64   < self.end) and
-0000bb50: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0000bb60: 2020 2020 2020 286f 7468 6572 5f72 6566        (other_ref
-0000bb70: 2e65 6e64 203e 2073 656c 662e 7374 6172  .end > self.star
-0000bb80: 7420 616e 6420 6f74 6865 725f 7265 662e  t and other_ref.
-0000bb90: 656e 6420 3c20 7365 6c66 2e65 6e64 290a  end < self.end).
-0000bba0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000bbb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000bbc0: 5661 6c75 6545 7272 6f72 2866 227b 6f74  ValueError(f"{ot
-0000bbd0: 6865 725f 7265 667d 2069 7320 6e6f 7420  her_ref} is not 
-0000bbe0: 6120 7661 6c69 6420 4269 626c 6552 6566  a valid BibleRef
-0000bbf0: 2229 0a0a 2020 2020 6465 6620 756e 696f  ")..    def unio
-0000bc00: 6e28 7365 6c66 2c20 6f74 6865 725f 7265  n(self, other_re
-0000bc10: 663a 2027 4269 626c 6552 6566 272c 2066  f: 'BibleRef', f
-0000bc20: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
-0000bc30: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
-0000bc40: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
-0000bc50: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
-0000bc60: 6120 6e65 7720 6042 6962 6c65 5261 6e67  a new `BibleRang
-0000bc70: 654c 6973 7460 206f 6620 7665 7273 6573  eList` of verses
-0000bc80: 2074 6861 7420 6172 6520 6569 7468 6572   that are either
-0000bc90: 2069 6e20 7468 6973 2072 616e 6765 206f   in this range o
-0000bca0: 7220 606f 7468 6572 5f72 6566 602e 0a20  r `other_ref`.. 
-0000bcb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000bcc0: 4966 2074 6869 7320 7261 6e67 6520 616e  If this range an
-0000bcd0: 6420 606f 7468 6572 5f72 6566 6020 6f76  d `other_ref` ov
-0000bce0: 6572 6c61 7020 6f72 2061 7265 2061 646a  erlap or are adj
-0000bcf0: 6163 656e 742c 2074 6865 2072 6573 756c  acent, the resul
-0000bd00: 7469 6e67 2060 4269 626c 6552 616e 6765  ting `BibleRange
-0000bd10: 4c69 7374 6020 636f 6e74 6169 6e73 206f  List` contains o
-0000bd20: 6e65 2065 6c65 6d65 6e74 3a0a 2020 2020  ne element:.    
-0000bd30: 2020 2020 6120 7369 6e67 6c65 2060 4269      a single `Bi
-0000bd40: 626c 6552 616e 6765 6020 656e 636f 6d70  bleRange` encomp
-0000bd50: 6173 7369 6e67 2074 6865 6d20 626f 7468  assing them both
-0000bd60: 2e20 4f74 6865 7277 6973 652c 2074 6865  . Otherwise, the
-0000bd70: 206c 6973 7420 636f 6e74 6169 6e73 2074   list contains t
-0000bd80: 776f 2065 6c65 6d65 6e74 733a 0a20 2020  wo elements:.   
-0000bd90: 2020 2020 2074 6869 7320 6042 6962 6c65       this `Bible
-0000bda0: 5261 6e67 6560 2061 6e64 2060 6f74 6865  Range` and `othe
-0000bdb0: 725f 7265 6660 2028 636f 6e76 6572 7465  r_ref` (converte
-0000bdc0: 6420 746f 2061 2060 4269 626c 6552 616e  d to a `BibleRan
-0000bdd0: 6765 6020 6966 206e 6563 6573 7361 7279  ge` if necessary
-0000bde0: 292e 0a0a 2020 2020 2020 2020 5573 696e  )...        Usin
-0000bdf0: 6720 7468 6520 607c 6020 6f70 6572 6174  g the `|` operat
-0000be00: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
-0000be10: 2074 6f20 6361 6c6c 696e 6720 6075 6e69   to calling `uni
-0000be20: 6f6e 2829 6020 7769 7468 2060 666c 6167  on()` with `flag
-0000be30: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
-0000be40: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-0000be50: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-0000be60: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
-0000be70: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
-0000be80: 2020 2020 2023 2055 7365 2074 6865 2042       # Use the B
-0000be90: 6962 6c65 5261 6e67 654c 6973 7420 696d  ibleRangeList im
-0000bea0: 706c 656d 656e 7461 7469 6f6e 0a20 2020  plementation.   
-0000beb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000bec0: 6f74 6865 725f 7265 662e 756e 696f 6e28  other_ref.union(
-0000bed0: 7365 6c66 2c20 666c 6167 733d 666c 6167  self, flags=flag
-0000bee0: 7329 0a20 2020 2020 2020 2069 6620 6973  s).        if is
-0000bef0: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
-0000bf00: 6566 2c20 4269 626c 6556 6572 7365 293a  ef, BibleVerse):
-0000bf10: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-0000bf20: 6f6e 7665 7274 2074 6f20 4269 626c 6552  onvert to BibleR
-0000bf30: 616e 6765 2028 616e 6420 7765 2064 6f6e  ange (and we don
-0000bf40: 2774 2065 6e66 6f72 6365 2065 7869 7374  't enforce exist
-0000bf50: 696e 6720 666c 6167 7320 666f 7220 636f  ing flags for co
-0000bf60: 6e76 6572 7369 6f6e 7329 0a20 2020 2020  nversions).     
-0000bf70: 2020 2020 2020 206f 7468 6572 5f72 6566         other_ref
-0000bf80: 203d 2042 6962 6c65 5261 6e67 6528 7374   = BibleRange(st
-0000bf90: 6172 743d 6f74 6865 725f 7265 662c 2065  art=other_ref, e
-0000bfa0: 6e64 3d6f 7468 6572 5f72 6566 2c20 666c  nd=other_ref, fl
-0000bfb0: 6167 733d 4269 626c 6546 6c61 672e 414c  ags=BibleFlag.AL
-0000bfc0: 4c29 0a20 2020 2020 2020 2069 6620 6973  L).        if is
-0000bfd0: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
-0000bfe0: 6566 2c20 4269 626c 6552 616e 6765 293a  ef, BibleRange):
-0000bff0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c000: 7365 6c66 2e69 735f 6469 736a 6f69 6e74  self.is_disjoint
-0000c010: 286f 7468 6572 5f72 6566 2920 616e 6420  (other_ref) and 
-0000c020: 6e6f 7420 7365 6c66 2e69 735f 6164 6a61  not self.is_adja
-0000c030: 6365 6e74 286f 7468 6572 5f72 6566 2c20  cent(other_ref, 
-0000c040: 666c 6167 733d 666c 6167 7329 3a0a 2020  flags=flags):.  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000c060: 7765 722c 2068 6967 6865 7220 3d20 2873  wer, higher = (s
-0000c070: 656c 662c 206f 7468 6572 5f72 6566 2920  elf, other_ref) 
-0000c080: 6966 2073 656c 6620 3c20 6f74 6865 725f  if self < other_
-0000c090: 7265 6620 656c 7365 2028 6f74 6865 725f  ref else (other_
-0000c0a0: 7265 662c 2073 656c 6629 200a 2020 2020  ref, self) .    
-0000c0b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c0c0: 726e 2042 6962 6c65 5261 6e67 654c 6973  rn BibleRangeLis
-0000c0d0: 7428 5b6c 6f77 6572 2c20 6869 6768 6572  t([lower, higher
-0000c0e0: 5d2c 2066 6c61 6773 3d42 6962 6c65 466c  ], flags=BibleFl
-0000c0f0: 6167 2e41 4c4c 290a 2020 2020 2020 2020  ag.ALL).        
-0000c100: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c110: 2020 2020 2020 2020 2020 7374 6172 7420            start 
-0000c120: 3d20 6d69 6e28 7365 6c66 2e73 7461 7274  = min(self.start
-0000c130: 2c20 6f74 6865 725f 7265 662e 7374 6172  , other_ref.star
-0000c140: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-0000c150: 2020 2065 6e64 203d 206d 6178 2873 656c     end = max(sel
-0000c160: 662e 656e 642c 206f 7468 6572 5f72 6566  f.end, other_ref
-0000c170: 2e65 6e64 290a 2020 2020 2020 2020 2020  .end).          
-0000c180: 2020 2020 2020 7265 7475 726e 2042 6962        return Bib
-0000c190: 6c65 5261 6e67 654c 6973 7428 5b42 6962  leRangeList([Bib
-0000c1a0: 6c65 5261 6e67 6528 7374 6172 743d 7374  leRange(start=st
-0000c1b0: 6172 742c 2065 6e64 3d65 6e64 2c20 666c  art, end=end, fl
-0000c1c0: 6167 733d 666c 6167 7329 5d2c 2066 6c61  ags=flags)], fla
-0000c1d0: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
-0000c1e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000c1f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000c200: 6520 5661 6c75 6545 7272 6f72 2866 227b  e ValueError(f"{
-0000c210: 6f74 6865 725f 7265 667d 2069 7320 6e6f  other_ref} is no
-0000c220: 7420 6120 7661 6c69 6420 4269 626c 6552  t a valid BibleR
-0000c230: 6566 2229 0a0a 2020 2020 6465 6620 696e  ef")..    def in
-0000c240: 7465 7273 6563 7469 6f6e 2873 656c 662c  tersection(self,
-0000c250: 206f 7468 6572 5f72 6566 3a20 2742 6962   other_ref: 'Bib
-0000c260: 6c65 5265 6627 2c20 666c 6167 733a 2042  leRef', flags: B
-0000c270: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-0000c280: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
-0000c290: 6973 7427 3a0a 2020 2020 2020 2020 2727  ist':.        ''
-0000c2a0: 2752 6574 7572 6e73 2061 206e 6577 2060  'Returns a new `
-0000c2b0: 4269 626c 6552 616e 6765 4c69 7374 6020  BibleRangeList` 
-0000c2c0: 6f66 2076 6572 7365 7320 7468 6174 2061  of verses that a
-0000c2d0: 7265 2063 6f6d 6d6f 6e20 746f 2062 6f74  re common to bot
-0000c2e0: 6820 7468 6973 2072 616e 6765 2061 6e64  h this range and
-0000c2f0: 2060 6f74 6865 725f 7265 6660 2e0a 2020   `other_ref`..  
-0000c300: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
-0000c310: 6620 7468 6572 6520 6172 6520 7665 7273  f there are vers
-0000c320: 6573 2069 6e20 636f 6d6d 6f6e 2c20 7468  es in common, th
-0000c330: 6520 6c69 7374 2063 6f6e 7461 696e 7320  e list contains 
-0000c340: 6120 7369 6e67 6c65 2060 4269 626c 6552  a single `BibleR
-0000c350: 616e 6765 6020 656c 656d 656e 742e 0a20  ange` element.. 
-0000c360: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
-0000c370: 6172 6520 6e6f 2076 6572 7365 7320 696e  are no verses in
-0000c380: 2063 6f6d 6d6f 6e2c 2074 6865 206c 6973   common, the lis
-0000c390: 7420 6973 2065 6d70 7479 2e0a 0a20 2020  t is empty...   
-0000c3a0: 2020 2020 2055 7369 6e67 2074 6865 2060       Using the `
-0000c3b0: 2660 206f 7065 7261 746f 7220 6973 2065  &` operator is e
-0000c3c0: 7175 6976 616c 656e 7420 746f 2063 616c  quivalent to cal
-0000c3d0: 6c69 6e67 2060 696e 7465 7273 6563 7469  ling `intersecti
-0000c3e0: 6f6e 2829 6020 7769 7468 2060 666c 6167  on()` with `flag
-0000c3f0: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
-0000c400: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-0000c410: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-0000c420: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
-0000c430: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
-0000c440: 2020 2020 2023 2055 7365 2074 6865 2042       # Use the B
-0000c450: 6962 6c65 5261 6e67 654c 6973 7420 696d  ibleRangeList im
-0000c460: 706c 656d 656e 7461 7469 6f6e 0a20 2020  plementation.   
-0000c470: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c480: 6f74 6865 725f 7265 662e 696e 7465 7273  other_ref.inters
-0000c490: 6563 7469 6f6e 2873 656c 662c 2066 6c61  ection(self, fla
-0000c4a0: 6773 3d66 6c61 6773 290a 2020 2020 2020  gs=flags).      
-0000c4b0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000c4c0: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
-0000c4d0: 5665 7273 6529 3a0a 2020 2020 2020 2020  Verse):.        
-0000c4e0: 2020 2020 2320 436f 6e76 6572 7420 746f      # Convert to
-0000c4f0: 2042 6962 6c65 5261 6e67 6520 2861 6e64   BibleRange (and
-0000c500: 2077 6520 646f 6e27 7420 656e 666f 7263   we don't enforc
-0000c510: 6520 6578 6973 7469 6e67 2066 6c61 6773  e existing flags
-0000c520: 2066 6f72 2063 6f6e 7665 7273 696f 6e73   for conversions
-0000c530: 290a 2020 2020 2020 2020 2020 2020 6f74  ).            ot
-0000c540: 6865 725f 7265 6620 3d20 4269 626c 6552  her_ref = BibleR
-0000c550: 616e 6765 2873 7461 7274 3d6f 7468 6572  ange(start=other
-0000c560: 5f72 6566 2c20 656e 643d 6f74 6865 725f  _ref, end=other_
-0000c570: 7265 662c 2066 6c61 6773 3d42 6962 6c65  ref, flags=Bible
-0000c580: 466c 6167 2e41 4c4c 290a 2020 2020 2020  Flag.ALL).      
-0000c590: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000c5a0: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
-0000c5b0: 5261 6e67 6529 3a0a 2020 2020 2020 2020  Range):.        
-0000c5c0: 2020 2020 6966 2073 656c 662e 6973 5f64      if self.is_d
-0000c5d0: 6973 6a6f 696e 7428 6f74 6865 725f 7265  isjoint(other_re
-0000c5e0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0000c5f0: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
-0000c600: 5261 6e67 654c 6973 7428 290a 2020 2020  RangeList().    
-0000c610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000c620: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000c630: 6172 7420 3d20 6d61 7828 7365 6c66 2e73  art = max(self.s
-0000c640: 7461 7274 2c20 6f74 6865 725f 7265 662e  tart, other_ref.
-0000c650: 7374 6172 7429 0a20 2020 2020 2020 2020  start).         
-0000c660: 2020 2020 2020 2065 6e64 203d 206d 696e         end = min
-0000c670: 2873 656c 662e 656e 642c 206f 7468 6572  (self.end, other
-0000c680: 5f72 6566 2e65 6e64 290a 2020 2020 2020  _ref.end).      
-0000c690: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c6a0: 2042 6962 6c65 5261 6e67 654c 6973 7428   BibleRangeList(
-0000c6b0: 5b42 6962 6c65 5261 6e67 6528 7374 6172  [BibleRange(star
-0000c6c0: 743d 7374 6172 742c 2065 6e64 3d65 6e64  t=start, end=end
-0000c6d0: 2c20 666c 6167 733d 666c 6167 7329 5d2c  , flags=flags)],
-0000c6e0: 2066 6c61 6773 3d42 6962 6c65 466c 6167   flags=BibleFlag
-0000c6f0: 2e41 4c4c 290a 2020 2020 2020 2020 656c  .ALL).        el
-0000c700: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000c710: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000c720: 2866 227b 6f74 6865 725f 7265 667d 2069  (f"{other_ref} i
-0000c730: 7320 6e6f 7420 6120 7661 6c69 6420 4269  s not a valid Bi
-0000c740: 626c 6552 6566 2229 0a0a 2020 2020 6465  bleRef")..    de
-0000c750: 6620 6469 6666 6572 656e 6365 2873 656c  f difference(sel
-0000c760: 662c 206f 7468 6572 5f72 6566 3a20 556e  f, other_ref: Un
-0000c770: 696f 6e5b 4269 626c 6556 6572 7365 2c20  ion[BibleVerse, 
-0000c780: 2742 6962 6c65 5261 6e67 6527 5d2c 0a20  'BibleRange'],. 
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 666c 6167 733a 2042 6962 6c65 466c    flags: BibleFl
-0000c7b0: 6167 203d 204e 6f6e 6529 202d 3e20 2742  ag = None) -> 'B
-0000c7c0: 6962 6c65 5261 6e67 654c 6973 7427 3a0a  ibleRangeList':.
-0000c7d0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-0000c7e0: 6e73 2061 206e 6577 2060 4269 626c 6552  ns a new `BibleR
-0000c7f0: 616e 6765 4c69 7374 6020 6f66 2076 6572  angeList` of ver
-0000c800: 7365 7320 7468 6174 2061 7265 2069 6e20  ses that are in 
-0000c810: 7468 6973 2072 616e 6765 2c20 6275 7420  this range, but 
-0000c820: 6e6f 7420 696e 2060 6f74 6865 725f 7265  not in `other_re
-0000c830: 6660 2e0a 0a20 2020 2020 2020 2049 6620  f`...        If 
-0000c840: 7468 6973 2072 616e 6765 2061 6e64 2060  this range and `
-0000c850: 6f74 6865 725f 7265 6660 2061 7265 2064  other_ref` are d
-0000c860: 6973 6a6f 696e 742c 2074 6865 206c 6973  isjoint, the lis
-0000c870: 7420 636f 6e74 6169 6e73 206f 6e65 2065  t contains one e
-0000c880: 6c65 6d65 6e74 3a20 6120 636f 7079 206f  lement: a copy o
-0000c890: 6620 7468 6973 2060 4269 626c 6552 616e  f this `BibleRan
-0000c8a0: 6765 602e 0a20 2020 2020 2020 2049 6620  ge`..        If 
-0000c8b0: 7468 6973 2072 616e 6765 2073 7572 726f  this range surro
-0000c8c0: 756e 6473 2060 6f74 6865 725f 7265 6660  unds `other_ref`
-0000c8d0: 2c20 7468 6520 6c69 7374 2063 6f6e 7461  , the list conta
-0000c8e0: 696e 7320 7477 6f20 656c 656d 656e 7473  ins two elements
-0000c8f0: 3a0a 2020 2020 2020 2020 2020 2020 6120  :.            a 
-0000c900: 6c6f 7765 722d 7365 6374 696f 6e20 6042  lower-section `B
-0000c910: 6962 6c65 5261 6e67 6560 2c20 616e 6420  ibleRange`, and 
-0000c920: 616e 2075 7070 6572 2d73 6563 7469 6f6e  an upper-section
-0000c930: 2060 4269 626c 6552 616e 6765 602e 0a20   `BibleRange`.. 
-0000c940: 2020 2020 2020 2049 6620 606f 7468 6572         If `other
-0000c950: 5f72 6566 6020 636f 6e74 6169 6e73 2074  _ref` contains t
-0000c960: 6869 7320 7261 6e67 652c 2074 6865 206c  his range, the l
-0000c970: 6973 7420 6973 2065 6d70 7479 2e0a 0a20  ist is empty... 
-0000c980: 2020 2020 2020 2055 7369 6e67 2074 6865         Using the
-0000c990: 2060 2d60 206f 7065 7261 746f 7220 6973   `-` operator is
-0000c9a0: 2065 7175 6976 616c 656e 7420 746f 2063   equivalent to c
-0000c9b0: 616c 6c69 6e67 2060 6469 6666 6572 656e  alling `differen
-0000c9c0: 6365 2829 6020 7769 7468 2060 666c 6167  ce()` with `flag
-0000c9d0: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
-0000c9e0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-0000c9f0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-0000ca00: 6572 5f72 6566 2c20 4269 626c 6556 6572  er_ref, BibleVer
-0000ca10: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-0000ca20: 2023 2043 6f6e 7665 7274 2074 6f20 4269   # Convert to Bi
-0000ca30: 626c 6552 616e 6765 2028 616e 6420 7765  bleRange (and we
-0000ca40: 2064 6f6e 2774 2065 6e66 6f72 6365 2065   don't enforce e
-0000ca50: 7869 7374 696e 6720 666c 6167 7320 666f  xisting flags fo
-0000ca60: 7220 636f 6e76 6572 7369 6f6e 7329 0a20  r conversions). 
-0000ca70: 2020 2020 2020 2020 2020 206f 7468 6572             other
-0000ca80: 5f72 6566 203d 2042 6962 6c65 5261 6e67  _ref = BibleRang
-0000ca90: 6528 7374 6172 743d 6f74 6865 725f 7265  e(start=other_re
-0000caa0: 662c 2065 6e64 3d6f 7468 6572 5f72 6566  f, end=other_ref
-0000cab0: 2c20 666c 6167 733d 4269 626c 6546 6c61  , flags=BibleFla
-0000cac0: 672e 414c 4c29 0a20 2020 2020 2020 2069  g.ALL).        i
-0000cad0: 6620 7365 6c66 2e69 735f 6469 736a 6f69  f self.is_disjoi
-0000cae0: 6e74 286f 7468 6572 5f72 6566 293a 0a20  nt(other_ref):. 
-0000caf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000cb00: 6e20 4269 626c 6552 616e 6765 4c69 7374  n BibleRangeList
-0000cb10: 285b 7365 6c66 5d2c 2066 6c61 6773 3d42  ([self], flags=B
-0000cb20: 6962 6c65 466c 6167 2e41 4c4c 290a 2020  ibleFlag.ALL).  
-0000cb30: 2020 2020 2020 6966 206f 7468 6572 5f72        if other_r
-0000cb40: 6566 2e63 6f6e 7461 696e 7328 7365 6c66  ef.contains(self
-0000cb50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000cb60: 6574 7572 6e20 4269 626c 6552 616e 6765  eturn BibleRange
-0000cb70: 4c69 7374 2829 0a0a 2020 2020 2020 2020  List()..        
-0000cb80: 6c6f 7765 725f 7261 6e67 6520 3d20 4269  lower_range = Bi
-0000cb90: 626c 6552 616e 6765 2873 7461 7274 3d73  bleRange(start=s
-0000cba0: 656c 662e 7374 6172 742c 2065 6e64 3d6f  elf.start, end=o
-0000cbb0: 7468 6572 5f72 6566 2e73 7461 7274 2e73  ther_ref.start.s
-0000cbc0: 7562 7472 6163 7428 312c 2066 6c61 6773  ubtract(1, flags
-0000cbd0: 3d66 6c61 6773 2929 0a20 2020 2020 2020  =flags)).       
-0000cbe0: 2075 7070 6572 5f72 616e 6765 203d 2042   upper_range = B
-0000cbf0: 6962 6c65 5261 6e67 6528 7374 6172 743d  ibleRange(start=
-0000cc00: 6f74 6865 725f 7265 662e 656e 642e 6164  other_ref.end.ad
-0000cc10: 6428 312c 2066 6c61 6773 3d66 6c61 6773  d(1, flags=flags
-0000cc20: 292c 2065 6e64 3d73 656c 662e 656e 6429  ), end=self.end)
-0000cc30: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000cc40: 2e73 7572 726f 756e 6473 286f 7468 6572  .surrounds(other
-0000cc50: 5f72 6566 293a 0a20 2020 2020 2020 2020  _ref):.         
-0000cc60: 2020 2072 6574 7572 6e20 4269 626c 6552     return BibleR
-0000cc70: 616e 6765 4c69 7374 285b 6c6f 7765 725f  angeList([lower_
-0000cc80: 7261 6e67 652c 2075 7070 6572 5f72 616e  range, upper_ran
-0000cc90: 6765 5d2c 2066 6c61 6773 3d42 6962 6c65  ge], flags=Bible
-0000cca0: 466c 6167 2e41 4c4c 290a 2020 2020 2020  Flag.ALL).      
-0000ccb0: 2020 6966 2073 656c 6620 3c20 6f74 6865    if self < othe
-0000ccc0: 725f 7265 663a 0a20 2020 2020 2020 2020  r_ref:.         
-0000ccd0: 2020 2072 6574 7572 6e20 4269 626c 6552     return BibleR
-0000cce0: 616e 6765 4c69 7374 285b 6c6f 7765 725f  angeList([lower_
-0000ccf0: 7261 6e67 655d 2c20 666c 6167 733d 4269  range], flags=Bi
-0000cd00: 626c 6546 6c61 672e 414c 4c29 0a20 2020  bleFlag.ALL).   
-0000cd10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000cd20: 2020 2020 2020 2072 6574 7572 6e20 4269         return Bi
-0000cd30: 626c 6552 616e 6765 4c69 7374 285b 7570  bleRangeList([up
-0000cd40: 7065 725f 7261 6e67 655d 2c20 666c 6167  per_range], flag
-0000cd50: 733d 4269 626c 6546 6c61 672e 414c 4c29  s=BibleFlag.ALL)
-0000cd60: 0a0a 2020 2020 6465 6620 7379 6d5f 6469  ..    def sym_di
-0000cd70: 6666 6572 656e 6365 2873 656c 662c 206f  fference(self, o
-0000cd80: 7468 6572 5f72 6566 3a20 556e 696f 6e5b  ther_ref: Union[
-0000cd90: 4269 626c 6556 6572 7365 2c20 2742 6962  BibleVerse, 'Bib
-0000cda0: 6c65 5261 6e67 6527 5d2c 0a20 2020 2020  leRange'],.     
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-0000cdc0: 6167 733a 2042 6962 6c65 466c 6167 203d  ags: BibleFlag =
-0000cdd0: 204e 6f6e 6529 202d 3e20 2742 6962 6c65   None) -> 'Bible
-0000cde0: 5261 6e67 654c 6973 7427 3a0a 2020 2020  RangeList':.    
-0000cdf0: 2020 2020 2727 2752 6574 7572 6e73 2061      '''Returns a
-0000ce00: 206e 6577 2060 4269 626c 6552 616e 6765   new `BibleRange
-0000ce10: 4c69 7374 6020 6f66 2076 6572 7365 7320  List` of verses 
-0000ce20: 7468 6174 2061 7265 2065 6974 6865 7220  that are either 
-0000ce30: 696e 2074 6869 7320 7261 6e67 652c 206f  in this range, o
-0000ce40: 7220 696e 2060 6f74 6865 725f 7265 6660  r in `other_ref`
-0000ce50: 2c0a 2020 2020 2020 2020 6275 7420 6e6f  ,.        but no
-0000ce60: 7420 626f 7468 2e0a 0a20 2020 2020 2020  t both...       
-0000ce70: 2044 6570 656e 6469 6e67 206f 6e20 7468   Depending on th
-0000ce80: 6973 2072 616e 6765 2061 6e64 2060 6f74  is range and `ot
-0000ce90: 6865 725f 7265 6660 2c20 7468 6520 6042  her_ref`, the `B
-0000cea0: 6962 6c65 5261 6e67 654c 6973 7460 2063  ibleRangeList` c
-0000ceb0: 6f6e 7461 696e 7320 6569 7468 6572 206f  ontains either o
-0000cec0: 6e65 206f 7220 7477 6f0a 2020 2020 2020  ne or two.      
-0000ced0: 2020 6042 6962 6c65 5261 6e67 6560 2065    `BibleRange` e
-0000cee0: 6c65 6d65 6e74 732e 2049 6620 7468 6973  lements. If this
-0000cef0: 2072 616e 6765 2061 6e64 2060 6f74 6865   range and `othe
-0000cf00: 725f 7265 6660 2061 7265 2065 7861 6374  r_ref` are exact
-0000cf10: 6c79 2065 7175 616c 2c20 7468 6973 206c  ly equal, this l
-0000cf20: 6973 7420 6973 2065 6d70 7479 2e0a 0a20  ist is empty... 
-0000cf30: 2020 2020 2020 2055 7369 6e67 2074 6865         Using the
-0000cf40: 2060 5e60 206f 7065 7261 746f 7220 6973   `^` operator is
-0000cf50: 2065 7175 6976 616c 656e 7420 746f 2063   equivalent to c
-0000cf60: 616c 6c69 6e67 2060 7379 6d5f 6469 6666  alling `sym_diff
-0000cf70: 6572 656e 6365 2829 6020 7769 7468 2060  erence()` with `
-0000cf80: 666c 6167 7320 3d20 4e6f 6e65 602e 0a20  flags = None`.. 
-0000cf90: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0000cfa0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000cfb0: 286f 7468 6572 5f72 6566 2c20 4269 626c  (other_ref, Bibl
-0000cfc0: 6556 6572 7365 293a 0a20 2020 2020 2020  eVerse):.       
-0000cfd0: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
-0000cfe0: 6f20 4269 626c 6552 616e 6765 2028 616e  o BibleRange (an
-0000cff0: 6420 7765 2064 6f6e 2774 2065 6e66 6f72  d we don't enfor
-0000d000: 6365 2065 7869 7374 696e 6720 666c 6167  ce existing flag
-0000d010: 7320 666f 7220 636f 6e76 6572 7369 6f6e  s for conversion
-0000d020: 7329 0a20 2020 2020 2020 2020 2020 206f  s).            o
-0000d030: 7468 6572 5f72 6566 203d 2042 6962 6c65  ther_ref = Bible
-0000d040: 5261 6e67 6528 7374 6172 743d 6f74 6865  Range(start=othe
-0000d050: 725f 7265 662c 2065 6e64 3d6f 7468 6572  r_ref, end=other
-0000d060: 5f72 6566 2c20 666c 6167 733d 4269 626c  _ref, flags=Bibl
-0000d070: 6546 6c61 672e 414c 4c29 0a20 2020 2020  eFlag.ALL).     
-0000d080: 2020 2069 6620 7365 6c66 203d 3d20 6f74     if self == ot
-0000d090: 6865 725f 7265 663a 0a20 2020 2020 2020  her_ref:.       
-0000d0a0: 2020 2020 2072 6574 7572 6e20 4269 626c       return Bibl
-0000d0b0: 6552 616e 6765 4c69 7374 2829 0a20 2020  eRangeList().   
-0000d0c0: 2020 2020 2075 6e69 6f6e 203d 2073 656c       union = sel
-0000d0d0: 662e 756e 696f 6e28 6f74 6865 725f 7265  f.union(other_re
-0000d0e0: 662c 2066 6c61 6773 3d66 6c61 6773 290a  f, flags=flags).
-0000d0f0: 2020 2020 2020 2020 696e 7465 7273 6563          intersec
-0000d100: 7469 6f6e 203d 2073 656c 662e 696e 7465  tion = self.inte
-0000d110: 7273 6563 7469 6f6e 286f 7468 6572 5f72  rsection(other_r
-0000d120: 6566 2c20 666c 6167 733d 666c 6167 7329  ef, flags=flags)
-0000d130: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000d140: 756e 696f 6e29 203e 2031 206f 7220 6c65  union) > 1 or le
-0000d150: 6e28 696e 7465 7273 6563 7469 6f6e 2920  n(intersection) 
-0000d160: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-0000d170: 2020 2320 5365 6c66 2061 6e64 206f 7468    # Self and oth
-0000d180: 6572 5f72 6566 2061 7265 2064 6973 6a6f  er_ref are disjo
-0000d190: 696e 7420 616e 642f 6f72 2061 646a 6163  int and/or adjac
-0000d1a0: 656e 742c 2073 6f20 7468 6520 756e 696f  ent, so the unio
-0000d1b0: 6e20 6973 2074 6865 2073 616d 650a 2020  n is the same.  
-0000d1c0: 2020 2020 2020 2020 2020 2320 6173 2074            # as t
-0000d1d0: 6865 2073 796d 6d65 7472 6963 2064 6966  he symmetric dif
-0000d1e0: 6665 7265 6e63 650a 2020 2020 2020 2020  ference.        
-0000d1f0: 2020 2020 7265 7475 726e 2075 6e69 6f6e      return union
-0000d200: 0a20 2020 2020 2020 2065 6c73 653a 2023  .        else: #
-0000d210: 2053 656c 6620 616e 6420 6f74 6865 725f   Self and other_
-0000d220: 7265 6620 6f76 6572 6c61 700a 2020 2020  ref overlap.    
-0000d230: 2020 2020 2020 2020 7265 7475 726e 2075          return u
-0000d240: 6e69 6f6e 5b30 5d2e 6469 6666 6572 656e  nion[0].differen
-0000d250: 6365 2869 6e74 6572 7365 6374 696f 6e5b  ce(intersection[
-0000d260: 305d 290a 0a20 2020 2064 6566 205f 5f69  0])..    def __i
-0000d270: 7465 725f 5f28 7365 6c66 293a 0a20 2020  ter__(self):.   
-0000d280: 2020 2020 2076 6572 7365 203d 2073 656c       verse = sel
-0000d290: 662e 7374 6172 740a 2020 2020 2020 2020  f.start.        
-0000d2a0: 7768 696c 6520 7665 7273 6520 3c3d 2073  while verse <= s
-0000d2b0: 656c 662e 656e 643a 0a20 2020 2020 2020  elf.end:.       
-0000d2c0: 2020 2020 2079 6965 6c64 2076 6572 7365       yield verse
-0000d2d0: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-0000d2e0: 7365 203d 2076 6572 7365 2e61 6464 2831  se = verse.add(1
-0000d2f0: 2c20 4269 626c 6546 6c61 672e 4d55 4c54  , BibleFlag.MULT
-0000d300: 4942 4f4f 4b29 0a0a 2020 2020 6465 6620  IBOOK)..    def 
-0000d310: 5f5f 636f 6e74 6169 6e73 5f5f 2873 656c  __contains__(sel
-0000d320: 662c 2062 6962 6c65 5f72 6566 2920 2d3e  f, bible_ref) ->
-0000d330: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
-0000d340: 2727 5265 7475 726e 7320 5472 7565 2069  ''Returns True i
-0000d350: 6620 6974 656d 2069 7320 6120 4269 626c  f item is a Bibl
-0000d360: 6552 6566 2074 6861 7420 6661 6c6c 7320  eRef that falls 
-0000d370: 7769 7468 696e 2074 6869 7320 7261 6e67  within this rang
-0000d380: 652c 206f 7468 6572 7769 7365 2046 616c  e, otherwise Fal
-0000d390: 7365 2e0a 2020 2020 2020 2020 2727 270a  se..        '''.
-0000d3a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d3b0: 656c 662e 636f 6e74 6169 6e73 2862 6962  elf.contains(bib
-0000d3c0: 6c65 5f72 6566 290a 2020 2020 0a20 2020  le_ref).    .   
-0000d3d0: 2064 6566 205f 5f6f 725f 5f28 7365 6c66   def __or__(self
-0000d3e0: 2c20 6f74 6865 725f 7265 663a 2027 4269  , other_ref: 'Bi
-0000d3f0: 626c 6552 6566 2729 202d 3e20 2742 6962  bleRef') -> 'Bib
-0000d400: 6c65 5261 6e67 654c 6973 7427 3a0a 2020  leRangeList':.  
-0000d410: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d420: 662e 756e 696f 6e28 6f74 6865 725f 7265  f.union(other_re
-0000d430: 6629 0a0a 2020 2020 6465 6620 5f5f 616e  f)..    def __an
-0000d440: 645f 5f28 7365 6c66 2c20 6f74 6865 725f  d__(self, other_
-0000d450: 7265 663a 2027 4269 626c 6552 6566 2729  ref: 'BibleRef')
-0000d460: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
-0000d470: 6973 7427 3a0a 2020 2020 2020 2020 7265  ist':.        re
-0000d480: 7475 726e 2073 656c 662e 696e 7465 7273  turn self.inters
-0000d490: 6563 7469 6f6e 286f 7468 6572 5f72 6566  ection(other_ref
-0000d4a0: 290a 0a20 2020 2064 6566 205f 5f73 7562  )..    def __sub
-0000d4b0: 5f5f 2873 656c 662c 206f 7468 6572 5f72  __(self, other_r
-0000d4c0: 6566 3a20 2742 6962 6c65 5265 6627 2920  ef: 'BibleRef') 
-0000d4d0: 2d3e 2027 4269 626c 6552 616e 6765 4c69  -> 'BibleRangeLi
-0000d4e0: 7374 273a 0a20 2020 2020 2020 2072 6574  st':.        ret
-0000d4f0: 7572 6e20 7365 6c66 2e64 6966 6665 7265  urn self.differe
-0000d500: 6e63 6528 6f74 6865 725f 7265 6629 0a0a  nce(other_ref)..
-0000d510: 2020 2020 6465 6620 5f5f 786f 725f 5f28      def __xor__(
-0000d520: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
-0000d530: 2027 4269 626c 6552 6566 2729 202d 3e20   'BibleRef') -> 
-0000d540: 2742 6962 6c65 5261 6e67 654c 6973 7427  'BibleRangeList'
-0000d550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000d560: 2073 656c 662e 7379 6d5f 6469 6666 6572   self.sym_differ
-0000d570: 656e 6365 286f 7468 6572 5f72 6566 290a  ence(other_ref).
-0000d580: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-0000d590: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-0000d5a0: 2072 6574 7572 6e20 6622 4269 626c 6552   return f"BibleR
-0000d5b0: 616e 6765 287b 7365 6c66 2e73 7472 2829  ange({self.str()
-0000d5c0: 7d29 220a 2020 2020 0a20 2020 2064 6566  })".    .    def
-0000d5d0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
-0000d5e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d5f0: 656c 662e 7374 7228 290a 0a20 2020 2064  elf.str()..    d
-0000d600: 6566 2073 7472 2873 656c 662c 2061 6262  ef str(self, abb
-0000d610: 7265 763d 4661 6c73 652c 2061 6c74 5f73  rev=False, alt_s
-0000d620: 6570 3d46 616c 7365 2c20 6e6f 7370 6163  ep=False, nospac
-0000d630: 653d 4661 6c73 652c 2066 6f72 6365 5f73  e=False, force_s
-0000d640: 7461 7274 5f76 6572 7365 733a 2062 6f6f  tart_verses: boo
-0000d650: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-0000d660: 2020 2020 2020 2066 6c61 6773 3a20 4269         flags: Bi
-0000d670: 626c 6546 6c61 6720 3d20 4e6f 6e65 293a  bleFlag = None):
-0000d680: 0a20 2020 2020 2020 2027 2727 5265 7475  .        '''Retu
-0000d690: 726e 7320 6120 636f 6e66 6967 7572 6162  rns a configurab
-0000d6a0: 6c65 2073 7472 696e 6720 7265 7072 6573  le string repres
-0000d6b0: 656e 7461 7469 6f6e 206f 6620 7468 6973  entation of this
-0000d6c0: 2060 4269 626c 6552 616e 6765 602c 2061   `BibleRange`, a
-0000d6d0: 7320 666f 6c6c 6f77 733a 0a0a 2020 2020  s follows:..    
-0000d6e0: 2020 2020 2d20 4966 2060 6162 6272 6576      - If `abbrev
-0000d6f0: 6020 6973 2060 5472 7565 602c 2074 6865  ` is `True`, the
-0000d700: 2061 6262 7265 7669 6174 6564 206e 616d   abbreviated nam
-0000d710: 6520 6f66 2074 6865 2062 6f6f 6b20 6973  e of the book is
-0000d720: 2075 7365 6420 2869 6e73 7465 6164 206f   used (instead o
-0000d730: 6620 7468 6520 6675 6c6c 206e 616d 6529  f the full name)
-0000d740: 2e0a 2020 2020 2020 2020 2d20 4966 2060  ..        - If `
-0000d750: 616c 745f 7365 7060 2069 7320 6054 7275  alt_sep` is `Tru
-0000d760: 6560 2c20 6368 6170 7465 7220 616e 6420  e`, chapter and 
-0000d770: 7665 7273 6520 6e75 6d62 6572 7320 6172  verse numbers ar
-0000d780: 6520 7365 7061 7261 7465 6420 6279 2074  e separated by t
-0000d790: 6865 2061 6c74 6572 6e61 7465 0a20 2020  he alternate.   
-0000d7a0: 2020 2020 2020 2073 6570 6172 6174 6f72         separator
-0000d7b0: 2028 6465 6661 756c 7473 2074 6f20 602e   (defaults to `.
-0000d7c0: 6029 2069 6e73 7465 6164 206f 6620 7468  `) instead of th
-0000d7d0: 6520 7374 616e 6461 7264 2073 6570 6172  e standard separ
-0000d7e0: 6174 6f72 2028 6465 6661 756c 7473 2074  ator (defaults t
-0000d7f0: 6f20 603a 6029 2e0a 2020 2020 2020 2020  o `:`)..        
-0000d800: 2d20 4966 2060 6e6f 7370 6163 6560 2069  - If `nospace` i
-0000d810: 7320 6054 7275 6560 2c20 6e6f 2073 7061  s `True`, no spa
-0000d820: 6365 7320 6172 6520 696e 636c 7564 6564  ces are included
-0000d830: 2069 6e20 7468 6520 7374 7269 6e67 2e0a   in the string..
-0000d840: 2020 2020 2020 2020 2d20 4966 2060 666f          - If `fo
-0000d850: 7263 655f 7374 6172 745f 7665 7273 6573  rce_start_verses
-0000d860: 6020 6973 2060 5472 7565 602c 2074 6865  ` is `True`, the
-0000d870: 2073 7461 7274 2076 6572 7365 206f 6620   start verse of 
-0000d880: 6120 7261 6e67 6520 6973 206d 6164 6520  a range is made 
-0000d890: 6578 706c 6963 6974 2069 6620 7468 6520  explicit if the 
-0000d8a0: 656e 640a 2020 2020 2020 2020 2020 7665  end.          ve
-0000d8b0: 7273 6520 6f66 2074 6865 2072 616e 6765  rse of the range
-0000d8c0: 2069 7320 616c 736f 2062 6569 6e67 2073   is also being s
-0000d8d0: 686f 776e 2e20 4f74 6865 7277 6973 652c  hown. Otherwise,
-0000d8e0: 2074 6865 2073 7461 7274 2076 6572 7365   the start verse
-0000d8f0: 2069 7320 6f6d 6974 7465 6420 7768 6572   is omitted wher
-0000d900: 6520 706f 7373 6962 6c65 2e0a 2020 2020  e possible..    
-0000d910: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000d920: 6966 2073 656c 662e 7370 616e 735f 7374  if self.spans_st
-0000d930: 6172 745f 626f 6f6b 2829 3a0a 2020 2020  art_book():.    
-0000d940: 2020 2020 2020 2020 7374 6172 745f 7061          start_pa
-0000d950: 7274 7320 3d20 4269 626c 6556 6572 7365  rts = BibleVerse
-0000d960: 5061 7274 2e42 4f4f 4b0a 2020 2020 2020  Part.BOOK.      
-0000d970: 2020 2020 2020 6174 5f76 6572 7365 5f6c        at_verse_l
-0000d980: 6576 656c 203d 2046 616c 7365 0a20 2020  evel = False.   
-0000d990: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
-0000d9a0: 7061 6e73 5f73 7461 7274 5f63 6861 7028  pans_start_chap(
-0000d9b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-0000d9c0: 6620 666f 7263 655f 7374 6172 745f 7665  f force_start_ve
-0000d9d0: 7273 6573 2061 6e64 206e 6f74 2073 656c  rses and not sel
-0000d9e0: 662e 7370 616e 735f 656e 645f 6368 6170  f.spans_end_chap
-0000d9f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000da00: 2020 2020 7374 6172 745f 7061 7274 7320      start_parts 
-0000da10: 3d20 4269 626c 6556 6572 7365 5061 7274  = BibleVersePart
-0000da20: 2e46 554c 4c5f 5245 460a 2020 2020 2020  .FULL_REF.      
-0000da30: 2020 2020 2020 2020 2020 6174 5f76 6572            at_ver
-0000da40: 7365 5f6c 6576 656c 203d 2054 7275 650a  se_level = True.
-0000da50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000da60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000da70: 2020 7374 6172 745f 7061 7274 7320 3d20    start_parts = 
-0000da80: 4269 626c 6556 6572 7365 5061 7274 2e42  BibleVersePart.B
-0000da90: 4f4f 4b5f 4348 4150 0a20 2020 2020 2020  OOK_CHAP.       
-0000daa0: 2020 2020 2020 2020 2061 745f 7665 7273           at_vers
-0000dab0: 655f 6c65 7665 6c20 3d20 4661 6c73 650a  e_level = False.
-0000dac0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000dad0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-0000dae0: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
-0000daf0: 7365 5061 7274 2e46 554c 4c5f 5245 460a  sePart.FULL_REF.
-0000db00: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
-0000db10: 6572 7365 5f6c 6576 656c 203d 2054 7275  erse_level = Tru
-0000db20: 650a 2020 2020 2020 2020 7374 6172 745f  e.        start_
-0000db30: 7374 7220 3d20 7365 6c66 2e73 7461 7274  str = self.start
-0000db40: 2e73 7472 2861 6262 7265 762c 2061 6c74  .str(abbrev, alt
-0000db50: 5f73 6570 2c20 6e6f 7370 6163 652c 2073  _sep, nospace, s
-0000db60: 7461 7274 5f70 6172 7473 2920 0a20 2020  tart_parts) .   
-0000db70: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
-0000db80: 2073 656c 662e 6973 5f77 686f 6c65 5f62   self.is_whole_b
-0000db90: 6f6f 6b28 666c 6167 7329 206f 7220 7365  ook(flags) or se
-0000dba0: 6c66 2e69 735f 7768 6f6c 655f 6368 6170  lf.is_whole_chap
-0000dbb0: 2866 6c61 6773 2920 6f72 2073 656c 662e  (flags) or self.
-0000dbc0: 6973 5f73 696e 676c 655f 7665 7273 6528  is_single_verse(
-0000dbd0: 293a 2023 2053 696e 676c 6520 7265 6665  ): # Single refe
-0000dbe0: 7265 6e63 650a 2020 2020 2020 2020 2020  rence.          
-0000dbf0: 2020 656e 645f 7374 7220 3d20 2222 0a20    end_str = "". 
-0000dc00: 2020 2020 2020 2020 2020 2072 616e 6765             range
-0000dc10: 5f73 6570 203d 2022 220a 2020 2020 2020  _sep = "".      
-0000dc20: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
-0000dc30: 2020 2020 2072 616e 6765 5f73 6570 203d       range_sep =
-0000dc40: 2062 6962 6c65 5f64 6174 6128 292e 7261   bible_data().ra
-0000dc50: 6e67 655f 7365 700a 2020 2020 2020 2020  nge_sep.        
-0000dc60: 2020 2020 6966 2073 656c 662e 656e 642e      if self.end.
-0000dc70: 626f 6f6b 2021 3d20 7365 6c66 2e73 7461  book != self.sta
-0000dc80: 7274 2e62 6f6f 6b3a 0a20 2020 2020 2020  rt.book:.       
-0000dc90: 2020 2020 2020 2020 2061 745f 7665 7273           at_vers
-0000dca0: 655f 6c65 7665 6c20 3d20 4661 6c73 650a  e_level = False.
-0000dcb0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000dcc0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000dcd0: 2e73 7061 6e73 5f65 6e64 5f62 6f6f 6b28  .spans_end_book(
-0000dce0: 666c 6167 7329 3a0a 2020 2020 2020 2020  flags):.        
-0000dcf0: 2020 2020 2020 2020 656e 645f 7061 7274          end_part
-0000dd00: 7320 3d20 4269 626c 6556 6572 7365 5061  s = BibleVersePa
-0000dd10: 7274 2e42 4f4f 4b0a 2020 2020 2020 2020  rt.BOOK.        
-0000dd20: 2020 2020 656c 6966 206e 6f74 2061 745f      elif not at_
-0000dd30: 7665 7273 655f 6c65 7665 6c20 616e 6420  verse_level and 
-0000dd40: 7365 6c66 2e73 7061 6e73 5f65 6e64 5f63  self.spans_end_c
-0000dd50: 6861 7028 666c 6167 7329 3a0a 2020 2020  hap(flags):.    
-0000dd60: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-0000dd70: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
-0000dd80: 7365 5061 7274 2e42 4f4f 4b5f 4348 4150  sePart.BOOK_CHAP
-0000dd90: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000dda0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ddb0: 2020 2065 6e64 5f70 6172 7473 203d 2042     end_parts = B
-0000ddc0: 6962 6c65 5665 7273 6550 6172 742e 4655  ibleVersePart.FU
-0000ddd0: 4c4c 5f52 4546 0a20 2020 2020 2020 2020  LL_REF.         
-0000dde0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0000ddf0: 6966 2073 656c 662e 7374 6172 742e 626f  if self.start.bo
-0000de00: 6f6b 203d 3d20 7365 6c66 2e65 6e64 2e62  ok == self.end.b
-0000de10: 6f6f 6b3a 0a20 2020 2020 2020 2020 2020  ook:.           
-0000de20: 2020 2020 2065 6e64 5f70 6172 7473 2026       end_parts &
-0000de30: 3d20 7e42 6962 6c65 5665 7273 6550 6172  = ~BibleVersePar
-0000de40: 742e 424f 4f4b 2023 204f 6d69 7420 626f  t.BOOK # Omit bo
-0000de50: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
-0000de60: 2020 2069 6620 7365 6c66 2e73 7461 7274     if self.start
-0000de70: 2e63 6861 705f 6e75 6d20 3d3d 2073 656c  .chap_num == sel
-0000de80: 662e 656e 642e 6368 6170 5f6e 756d 3a0a  f.end.chap_num:.
-0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 2020 2020 656e 645f 7061 7274 7320 263d      end_parts &=
-0000deb0: 207e 4269 626c 6556 6572 7365 5061 7274   ~BibleVersePart
-0000dec0: 2e43 4841 5020 2320 4f6d 6974 2063 6861  .CHAP # Omit cha
-0000ded0: 7074 6572 0a20 2020 2020 2020 2020 2020  pter.           
-0000dee0: 200a 2020 2020 2020 2020 2020 2020 656e   .            en
-0000def0: 645f 7374 7220 3d20 7365 6c66 2e65 6e64  d_str = self.end
-0000df00: 2e73 7472 2861 6262 7265 762c 2061 6c74  .str(abbrev, alt
-0000df10: 5f73 6570 2c20 6e6f 7370 6163 652c 2065  _sep, nospace, e
-0000df20: 6e64 5f70 6172 7473 2920 0a20 2020 2020  nd_parts) .     
-0000df30: 2020 200a 2020 2020 2020 2020 7265 7375     .        resu
-0000df40: 6c74 203d 2066 227b 7374 6172 745f 7374  lt = f"{start_st
-0000df50: 727d 7b72 616e 6765 5f73 6570 7d7b 656e  r}{range_sep}{en
-0000df60: 645f 7374 727d 220a 2020 2020 2020 2020  d_str}".        
-0000df70: 6966 206e 6f73 7061 6365 3a0a 2020 2020  if nospace:.    
-0000df80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000df90: 6573 756c 742e 7265 706c 6163 6528 2220  esult.replace(" 
-0000dfa0: 222c 2022 2229 0a20 2020 2020 2020 2065  ", "").        e
-0000dfb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000dfc0: 2072 6574 7572 6e20 7265 7375 6c74 2e73   return result.s
-0000dfd0: 7472 6970 2829 0a0a 0a63 6c61 7373 2042  trip()...class B
-0000dfe0: 6962 6c65 5261 6e67 654c 6973 7428 7574  ibleRangeList(ut
-0000dff0: 696c 2e47 726f 7570 6564 4c69 7374 293a  il.GroupedList):
-0000e000: 0a20 2020 2027 2727 4120 6c69 7374 206f  .    '''A list o
-0000e010: 6620 6042 6962 6c65 5261 6e67 6560 2065  f `BibleRange` e
-0000e020: 6c65 6d65 6e74 732c 2061 6c6c 6f77 696e  lements, allowin
-0000e030: 6720 666f 7220 6772 6f75 7069 6e67 2061  g for grouping a
-0000e040: 6e64 2073 6574 2d73 7479 6c65 206f 7065  nd set-style ope
-0000e050: 7261 7469 6f6e 732e 0a0a 2020 2020 4375  rations...    Cu
-0000e060: 7272 656e 746c 7920 7468 6520 6772 6f75  rrently the grou
-0000e070: 7069 6e67 2066 756e 6374 696f 6e61 6c69  ping functionali
-0000e080: 7479 2069 7320 7072 6f76 6964 6564 2076  ty is provided v
-0000e090: 6961 2061 2073 7570 6572 636c 6173 7320  ia a superclass 
-0000e0a0: 2860 6269 626c 6572 6566 2e75 7469 6c2e  (`bibleref.util.
-0000e0b0: 4772 6f75 7065 644c 6973 7460 2c20 6120  GroupedList`, a 
-0000e0c0: 646f 7562 6c79 2d6c 696e 6b65 640a 2020  doubly-linked.  
-0000e0d0: 2020 6c69 7374 292c 2074 686f 7567 6820    list), though 
-0000e0e0: 7468 6973 2073 686f 756c 6420 6265 2063  this should be c
-0000e0f0: 6f6e 7369 6465 7265 6420 616e 2069 6d70  onsidered an imp
-0000e100: 6c65 6d65 6e74 6174 696f 6e20 6465 7461  lementation deta
-0000e110: 696c 2e0a 2020 2020 2727 270a 2020 2020  il..    '''.    
-0000e120: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000e130: 662c 202a 6172 6773 2c20 666c 6167 733a  f, *args, flags:
-0000e140: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-0000e150: 6529 3a0a 2020 2020 2020 2020 2727 2741  e):.        '''A
-0000e160: 2042 6962 6c65 5261 6e67 6520 6361 6e20   BibleRange can 
-0000e170: 6265 2063 6f6e 7374 7275 6374 6564 2069  be constructed i
-0000e180: 6e20 616e 7920 6f66 2074 6865 2066 6f6c  n any of the fol
-0000e190: 6c6f 7769 6e67 2077 6179 733a 0a0a 2020  lowing ways:..  
-0000e1a0: 2020 2020 2020 312e 2046 726f 6d20 6120        1. From a 
-0000e1b0: 7369 6e67 6c65 2073 7472 696e 673a 2060  single string: `
-0000e1c0: 4269 626c 6552 616e 6765 4c69 7374 2822  BibleRangeList("
-0000e1d0: 4d61 726b 2033 3a31 2d34 3a32 3b20 353a  Mark 3:1-4:2; 5:
-0000e1e0: 362d 382c 2031 303b 204d 6174 7420 3422  6-8, 10; Matt 4"
-0000e1f0: 2960 0a0a 2020 2020 2020 2020 2020 2052  )`..           R
-0000e200: 6169 7365 7320 6120 6042 6962 6c65 5265  aises a `BibleRe
-0000e210: 6650 6172 7369 6e67 4572 726f 7260 2069  fParsingError` i
-0000e220: 6620 7468 6520 7374 7269 6e67 2063 616e  f the string can
-0000e230: 6e6f 7420 6265 2070 6172 7365 642e 0a0a  not be parsed...
-0000e240: 2020 2020 2020 2020 2020 2057 6865 6e20             When 
-0000e250: 7061 7273 696e 6720 6120 7374 7269 6e67  parsing a string
-0000e260: 2c20 6561 6368 206d 616a 6f72 2067 726f  , each major gro
-0000e270: 7570 2d73 6570 6172 6174 6f72 2028 603b  up-separator (`;
-0000e280: 6020 6279 2064 6566 6175 6c74 2920 706c  ` by default) pl
-0000e290: 6163 6573 2073 7562 7365 7175 656e 740a  aces subsequent.
-0000e2a0: 2020 2020 2020 2020 2020 2042 6962 6c65             Bible
-0000e2b0: 2072 616e 6765 7320 696e 746f 2061 206e   ranges into a n
-0000e2c0: 6577 2067 726f 7570 2e20 4561 6368 206d  ew group. Each m
-0000e2d0: 696e 6f72 2067 726f 7570 2d73 6570 6172  inor group-separ
-0000e2e0: 6174 6f72 2028 602c 6020 6279 2064 6566  ator (`,` by def
-0000e2f0: 6175 6c74 2920 706c 6163 6573 2073 7562  ault) places sub
-0000e300: 7365 7175 656e 740a 2020 2020 2020 2020  sequent.        
-0000e310: 2020 2070 6173 7361 6765 7320 696e 746f     passages into
-0000e320: 2074 6865 2073 616d 6520 6772 6f75 702e   the same group.
-0000e330: 0a0a 2020 2020 2020 2020 2020 2020 6060  ..            ``
-0000e340: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-0000e350: 2020 2020 3e3e 3e20 6672 6f6d 2062 6962      >>> from bib
-0000e360: 6c65 7265 6620 696d 706f 7274 202a 0a20  leref import *. 
-0000e370: 2020 2020 2020 2020 2020 203e 3e3e 2072             >>> r
-0000e380: 616e 6765 5f6c 6973 7420 3d20 4269 626c  ange_list = Bibl
-0000e390: 6552 616e 6765 4c69 7374 2822 4d61 726b  eRangeList("Mark
-0000e3a0: 2033 3a31 2d34 3a32 3b20 353a 362d 382c   3:1-4:2; 5:6-8,
-0000e3b0: 2031 303b 204d 6174 7420 3422 290a 2020   10; Matt 4").  
-0000e3c0: 2020 2020 2020 2020 2020 3e3e 3e20 6c65            >>> le
-0000e3d0: 6e28 7261 6e67 655f 6c69 7374 2e67 726f  n(range_list.gro
-0000e3e0: 7570 7329 0a20 2020 2020 2020 2020 2020  ups).           
-0000e3f0: 2033 0a20 2020 2020 2020 2020 2020 203e   3.            >
-0000e400: 3e3e 2072 616e 6765 5f6c 6973 742e 6772  >> range_list.gr
-0000e410: 6f75 7073 5b30 5d0a 2020 2020 2020 2020  oups[0].        
-0000e420: 2020 2020 4772 6f75 7056 6965 7728 5b42      GroupView([B
-0000e430: 6962 6c65 5261 6e67 6528 4d61 726b 2033  ibleRange(Mark 3
-0000e440: 2d34 3a32 295d 290a 2020 2020 2020 2020  -4:2)]).        
-0000e450: 2020 2020 3e3e 3e20 7261 6e67 655f 6c69      >>> range_li
-0000e460: 7374 2e67 726f 7570 735b 315d 0a20 2020  st.groups[1].   
-0000e470: 2020 2020 2020 2020 2047 726f 7570 5669           GroupVi
-0000e480: 6577 285b 4269 626c 6552 616e 6765 284d  ew([BibleRange(M
-0000e490: 6172 6b20 353a 362d 353a 3829 2c20 4269  ark 5:6-5:8), Bi
-0000e4a0: 626c 6552 616e 6765 284d 6172 6b20 353a  bleRange(Mark 5:
-0000e4b0: 3130 295d 290a 2020 2020 2020 2020 2020  10)]).          
-0000e4c0: 2020 3e3e 3e20 7261 6e67 655f 6c69 7374    >>> range_list
-0000e4d0: 2e67 726f 7570 735b 325d 0a20 2020 2020  .groups[2].     
-0000e4e0: 2020 2020 2020 2047 726f 7570 5669 6577         GroupView
-0000e4f0: 285b 4269 626c 6552 616e 6765 284d 6174  ([BibleRange(Mat
-0000e500: 7468 6577 2034 295d 290a 2020 2020 2020  thew 4)]).      
-0000e510: 2020 2020 2020 3e3e 3e20 7261 6e67 655f        >>> range_
-0000e520: 6c69 7374 2e67 726f 7570 735b 315d 5b30  list.groups[1][0
-0000e530: 5d0a 2020 2020 2020 2020 2020 2020 4269  ].            Bi
-0000e540: 626c 6552 616e 6765 284d 6172 6b20 353a  bleRange(Mark 5:
-0000e550: 362d 353a 3829 0a20 2020 2020 2020 2020  6-5:8).         
-0000e560: 2020 203e 3e3e 2072 616e 6765 5f6c 6973     >>> range_lis
-0000e570: 742e 6772 6f75 7073 5b31 5d5b 315d 0a20  t.groups[1][1]. 
-0000e580: 2020 2020 2020 2020 2020 2042 6962 6c65             Bible
-0000e590: 5261 6e67 6528 4d61 726b 2035 3a31 3029  Range(Mark 5:10)
-0000e5a0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-0000e5b0: 0a20 2020 2020 2020 2032 2e20 4672 6f6d  .        2. From
-0000e5c0: 2061 6e79 2069 7465 7261 626c 6520 636f   any iterable co
-0000e5d0: 6e74 6169 6e69 6e67 2042 6962 6c65 5261  ntaining BibleRa
-0000e5e0: 6e67 6573 3a0a 2020 2020 2020 2020 2020  nges:.          
-0000e5f0: 2060 4269 626c 6552 616e 6765 4c69 7374   `BibleRangeList
-0000e600: 285b 4269 626c 6552 616e 6765 2822 4d61  ([BibleRange("Ma
-0000e610: 726b 2033 3a31 2d34 3a32 2229 2c20 4269  rk 3:1-4:2"), Bi
-0000e620: 626c 6552 616e 6765 2822 4d61 726b 2035  bleRange("Mark 5
-0000e630: 3a36 2d38 2229 2c0a 2020 2020 2020 2020  :6-8"),.        
+00005950: 656e 643d 656e 645f 626f 6f6b 2e6c 6173  end=end_book.las
+00005960: 745f 7665 7273 6528 292c 2066 6c61 6773  t_verse(), flags
+00005970: 3d66 6c61 6773 290a 0a20 2020 2023 2054  =flags)..    # T
+00005980: 4f44 4f3a 2043 6f6e 7369 6465 7220 616c  ODO: Consider al
+00005990: 6c6f 7769 6e67 2061 2062 6f6f 6b20 616e  lowing a book an
+000059a0: 6420 7665 7273 652c 2077 6974 686f 7574  d verse, without
+000059b0: 2061 2063 6861 7074 6572 2e20 4173 7375   a chapter. Assu
+000059c0: 6d65 2066 6972 7374 206f 7220 6c61 7374  me first or last
+000059d0: 2063 6861 7074 6572 2061 7320 6e65 6365   chapter as nece
+000059e0: 7373 6172 792e 0a20 2020 2064 6566 205f  ssary..    def _
+000059f0: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
+00005a00: 7267 732c 2073 7461 7274 3a20 4269 626c  rgs, start: Bibl
+00005a10: 6556 6572 7365 203d 204e 6f6e 652c 2065  eVerse = None, e
+00005a20: 6e64 3a20 4269 626c 6556 6572 7365 203d  nd: BibleVerse =
+00005a30: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00005a40: 2020 2020 2020 2020 666c 6167 733a 2042          flags: B
+00005a50: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
+00005a60: 3a0a 2020 2020 2020 2020 2727 2741 2060  :.        '''A `
+00005a70: 4269 626c 6552 616e 6765 6020 6361 6e20  BibleRange` can 
+00005a80: 6265 2063 6f6e 7374 7275 6374 6564 2069  be constructed i
+00005a90: 6e20 616e 7920 6f66 2074 6865 2066 6f6c  n any of the fol
+00005aa0: 6c6f 7769 6e67 2077 6179 733a 0a0a 2020  lowing ways:..  
+00005ab0: 2020 2020 2020 312e 2046 726f 6d20 6120        1. From a 
+00005ac0: 7369 6e67 6c65 2073 7472 696e 673a 2060  single string: `
+00005ad0: 4269 626c 6552 616e 6765 2822 4d61 726b  BibleRange("Mark
+00005ae0: 2033 3a31 2d34 3a32 2229 600a 0a20 2020   3:1-4:2")`..   
+00005af0: 2020 2020 2020 2020 5261 6973 6573 2061          Raises a
+00005b00: 2060 4269 626c 6552 6566 5061 7273 696e   `BibleRefParsin
+00005b10: 6745 7272 6f72 6020 6966 2074 6865 2073  gError` if the s
+00005b20: 7472 696e 6720 6361 6e6e 6f74 2062 6520  tring cannot be 
+00005b30: 7061 7273 6564 2e0a 0a20 2020 2020 2020  parsed...       
+00005b40: 2032 2e20 4672 6f6d 2061 2073 7461 7274   2. From a start
+00005b50: 2061 6e64 2065 6e64 2060 4269 626c 6556   and end `BibleV
+00005b60: 6572 7365 602c 2077 6869 6368 206d 7573  erse`, which mus
+00005b70: 7420 6265 2073 7065 6369 6669 6564 2075  t be specified u
+00005b80: 7369 6e67 2074 6865 206b 6579 776f 7264  sing the keyword
+00005b90: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
+00005ba0: 2020 2020 2020 6073 7461 7274 6020 616e        `start` an
+00005bb0: 6420 6065 6e64 603a 2060 4269 626c 6552  d `end`: `BibleR
+00005bc0: 616e 6765 2873 7461 7274 3d42 6962 6c65  ange(start=Bible
+00005bd0: 5665 7273 6528 224d 6172 6b20 333a 3122  Verse("Mark 3:1"
+00005be0: 292c 2065 6e64 3d42 6962 6c65 5665 7273  ), end=BibleVers
+00005bf0: 6528 224d 6172 6b20 343a 3222 2929 600a  e("Mark 4:2"))`.
+00005c00: 0a20 2020 2020 2020 2033 2e20 4173 2061  .        3. As a
+00005c10: 2063 6f70 7920 6f66 2061 6e20 6578 6973   copy of an exis
+00005c20: 7469 6e67 2042 6962 6c65 5261 6e67 653a  ting BibleRange:
+00005c30: 2060 4269 626c 6552 616e 6765 2865 7869   `BibleRange(exi
+00005c40: 7374 696e 675f 6269 626c 655f 7261 6e67  sting_bible_rang
+00005c50: 6529 600a 0a20 2020 2020 2020 2034 2e20  e)`..        4. 
+00005c60: 4672 6f6d 2070 6f73 6974 696f 6e61 6c20  From positional 
+00005c70: 6172 6775 6d65 6e74 7320 696e 2074 6865  arguments in the
+00005c80: 2066 6f6c 6c6f 7769 6e67 206f 7264 6572   following order
+00005c90: 3a0a 2020 2020 2020 2020 2020 2053 7461  :.           Sta
+00005ca0: 7274 2062 6f6f 6b2c 2073 7461 7274 2060  rt book, start `
+00005cb0: 6368 6170 5f6e 756d 602c 2073 7461 7274  chap_num`, start
+00005cc0: 2060 7665 7273 655f 6e75 6d60 2c20 656e   `verse_num`, en
+00005cd0: 6420 626f 6f6b 2c20 656e 6420 6063 6861  d book, end `cha
+00005ce0: 705f 6e75 6d60 2c20 656e 6420 6076 6572  p_num`, end `ver
+00005cf0: 7365 5f6e 756d 602e 0a20 2020 2020 2020  se_num`..       
+00005d00: 2020 2020 5374 6172 7420 616e 6420 656e      Start and en
+00005d10: 6420 626f 6f6b 7320 6361 6e20 6265 2073  d books can be s
+00005d20: 7472 696e 6720 6e61 6d65 7320 6f72 2060  tring names or `
+00005d30: 4269 626c 6542 6f6f 6b60 2065 6e75 6d73  BibleBook` enums
+00005d40: 2e0a 2020 2020 2020 2020 2020 204c 6174  ..           Lat
+00005d50: 6572 2061 7267 756d 656e 7473 2063 616e  er arguments can
+00005d60: 2062 6520 6f6d 6974 7465 6420 6f72 2073   be omitted or s
+00005d70: 6574 2074 6f20 604e 6f6e 6560 2c20 6173  et to `None`, as
+00005d80: 2069 6e20 7468 6573 6520 6578 616d 706c   in these exampl
+00005d90: 6573 3a0a 0a20 2020 2020 2020 2020 2020  es:..           
+00005da0: 6042 6962 6c65 5261 6e67 6528 4269 626c  `BibleRange(Bibl
+00005db0: 6542 6f6f 6b2e 4d61 7474 2c20 322c 2033  eBook.Matt, 2, 3
+00005dc0: 2c20 4269 626c 6542 6f6f 6b2e 4a6f 686e  , BibleBook.John
+00005dd0: 2c20 342c 2036 2c20 666c 6167 733d 4269  , 4, 6, flags=Bi
+00005de0: 626c 6546 6c61 672e 4d55 4c54 4942 4f4f  bleFlag.MULTIBOO
+00005df0: 4b29 2023 204d 6174 7420 323a 332d 4a6f  K) # Matt 2:3-Jo
+00005e00: 686e 2034 3a36 600a 2020 2020 2020 2020  hn 4:6`.        
+00005e10: 2020 200a 2020 2020 2020 2020 2020 2060     .           `
+00005e20: 4269 626c 6552 616e 6765 2842 6962 6c65  BibleRange(Bible
+00005e30: 426f 6f6b 2e4d 6174 7429 2023 2045 6e74  Book.Matt) # Ent
+00005e40: 6972 6520 626f 6f6b 3a20 4d61 7474 2031  ire book: Matt 1
+00005e50: 3a31 2d32 383a 3230 600a 2020 2020 2020  :1-28:20`.      
+00005e60: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00005e70: 2060 4269 626c 6552 616e 6765 2842 6962   `BibleRange(Bib
+00005e80: 6c65 426f 6f6b 2e4d 6174 742c 2032 2920  leBook.Matt, 2) 
+00005e90: 2320 456e 7469 7265 2063 6861 7074 6572  # Entire chapter
+00005ea0: 3a20 4d61 7474 2032 3a31 2d32 3360 0a20  : Matt 2:1-23`. 
+00005eb0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00005ec0: 2020 2020 2020 6042 6962 6c65 5261 6e67        `BibleRang
+00005ed0: 6528 4269 626c 6542 6f6f 6b2e 4d61 7474  e(BibleBook.Matt
+00005ee0: 2c20 322c 2033 2920 2320 5369 6e67 6c65  , 2, 3) # Single
+00005ef0: 2076 6572 7365 3a20 4d61 7474 2032 3a33   verse: Matt 2:3
+00005f00: 600a 2020 2020 2020 2020 2020 200a 2020  `.           .  
+00005f10: 2020 2020 2020 2020 2060 4269 626c 6552           `BibleR
+00005f20: 616e 6765 2842 6962 6c65 426f 6f6b 2e4d  ange(BibleBook.M
+00005f30: 6174 742c 204e 6f6e 652c 204e 6f6e 652c  att, None, None,
+00005f40: 2042 6962 6c65 426f 6f6b 2e4a 6f68 6e2c   BibleBook.John,
+00005f50: 2066 6c61 6773 3d42 6962 6c65 466c 6167   flags=BibleFlag
+00005f60: 2e4d 554c 5449 424f 4f4b 2920 2320 4d61  .MULTIBOOK) # Ma
+00005f70: 7474 2031 3a31 2d4a 6f68 6e20 3231 3a32  tt 1:1-John 21:2
+00005f80: 3560 0a20 2020 2020 2020 2020 2020 0a20  5`.           . 
+00005f90: 2020 2020 2020 2020 2020 6042 6962 6c65            `Bible
+00005fa0: 5261 6e67 6528 4269 626c 6542 6f6f 6b2e  Range(BibleBook.
+00005fb0: 4d61 7474 2c20 4e6f 6e65 2c20 4e6f 6e65  Matt, None, None
+00005fc0: 2c20 4e6f 6e65 2c20 3429 2023 204d 6174  , None, 4) # Mat
+00005fd0: 7420 313a 312d 343a 3235 600a 2020 2020  t 1:1-4:25`.    
+00005fe0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005ff0: 2020 2060 4269 626c 6552 616e 6765 2842     `BibleRange(B
+00006000: 6962 6c65 426f 6f6b 2e4d 6174 742c 204e  ibleBook.Matt, N
+00006010: 6f6e 652c 204e 6f6e 652c 204e 6f6e 652c  one, None, None,
+00006020: 204e 6f6e 652c 2036 2920 2320 4d61 7474   None, 6) # Matt
+00006030: 2031 3a31 2d31 3a36 600a 2020 2020 2020   1:1-1:6`.      
+00006040: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00006050: 2060 4269 626c 6552 616e 6765 2842 6962   `BibleRange(Bib
+00006060: 6c65 426f 6f6b 2e4d 6174 742c 2032 2c20  leBook.Matt, 2, 
+00006070: 332c 204e 6f6e 652c 2034 2c20 3629 2023  3, None, 4, 6) #
+00006080: 204d 6174 7420 323a 332d 343a 3660 0a0a   Matt 2:3-4:6`..
+00006090: 2020 2020 2020 2049 6620 7468 6520 7374         If the st
+000060a0: 6172 7420 7665 7273 6520 6973 206f 6276  art verse is obv
+000060b0: 696f 7573 6c79 2067 7265 6174 6572 2074  iously greater t
+000060c0: 6861 6e20 7468 6520 656e 6420 7665 7273  han the end vers
+000060d0: 652c 2074 6865 7920 6172 6520 7377 6170  e, they are swap
+000060e0: 7065 6420 6172 6f75 6e64 2e0a 2020 2020  ped around..    
+000060f0: 2020 2020 4e6f 7465 2074 6861 7420 6974      Note that it
+00006100: 2069 7320 736f 6d65 7469 6d65 7320 6e6f   is sometimes no
+00006110: 7420 706f 7373 6962 6c65 2074 6f20 6469  t possible to di
+00006120: 7374 696e 6775 6973 6820 6120 7377 6170  stinguish a swap
+00006130: 7065 6420 7374 6172 7420 616e 6420 656e  ped start and en
+00006140: 6420 6672 6f6d 0a20 2020 2020 2020 206d  d from.        m
+00006150: 6973 666f 726d 6564 2061 7267 756d 656e  isformed argumen
+00006160: 7473 2e0a 0a20 2020 2020 2020 2049 6620  ts...        If 
+00006170: 7468 6520 7375 7070 6c69 6564 2061 7267  the supplied arg
+00006180: 756d 656e 7473 2061 7265 206e 6f74 2061  uments are not a
+00006190: 2076 616c 6964 2076 6572 7365 2c20 616e   valid verse, an
+000061a0: 2060 496e 7661 6c69 6452 6566 6572 656e   `InvalidReferen
+000061b0: 6365 4572 726f 7260 2069 7320 7261 6973  ceError` is rais
+000061c0: 6564 2e0a 2020 2020 2020 2020 4966 2074  ed..        If t
+000061d0: 6865 2073 7461 7274 2061 6e64 2065 6e64  he start and end
+000061e0: 2076 6572 7365 7320 6172 6520 6672 6f6d   verses are from
+000061f0: 2064 6966 6665 7265 6e74 2060 4269 626c   different `Bibl
+00006200: 6542 6f6f 6b73 6020 616e 6420 6042 6962  eBooks` and `Bib
+00006210: 6c65 466c 6167 2e4d 554c 5449 424f 4f4b  leFlag.MULTIBOOK
+00006220: 6020 6973 206e 6f74 2073 6574 2067 6c6f  ` is not set glo
+00006230: 6261 6c6c 790a 2020 2020 2020 2020 6f72  bally.        or
+00006240: 2075 7369 6e67 2074 6865 2060 666c 6167   using the `flag
+00006250: 7360 2061 7267 756d 656e 742c 2061 2060  s` argument, a `
+00006260: 4d75 6c74 6962 6f6f 6b52 616e 6765 4e6f  MultibookRangeNo
+00006270: 7441 6c6c 6f77 6564 4572 726f 7260 2069  tAllowedError` i
+00006280: 7320 7261 6973 6564 2e20 4966 2074 6865  s raised. If the
+00006290: 2061 7267 756d 656e 7473 2061 7265 206f   arguments are o
+000062a0: 6620 616e 0a20 2020 2020 2020 2069 6e63  f an.        inc
+000062b0: 6f72 7265 6374 206e 756d 6265 7220 6f72  orrect number or
+000062c0: 2074 7970 652c 2061 2060 5661 6c75 6545   type, a `ValueE
+000062d0: 7272 6f72 6020 6973 2072 6169 7365 642e  rror` is raised.
+000062e0: 2020 2020 200a 2020 2020 2020 2020 2727       .        ''
+000062f0: 270a 2020 2020 2020 2020 666c 6167 7320  '.        flags 
+00006300: 3d20 666c 6167 7320 6f72 2067 6c6f 6261  = flags or globa
+00006310: 6c73 2829 5b27 666c 6167 7327 5d20 6f72  ls()['flags'] or
+00006320: 2042 6962 6c65 466c 6167 2e4e 4f4e 450a   BibleFlag.NONE.
+00006330: 2020 2020 2020 2020 6966 206c 656e 2861          if len(a
+00006340: 7267 7329 203d 3d20 303a 0a20 2020 2020  rgs) == 0:.     
+00006350: 2020 2020 2020 2069 6620 4269 626c 6546         if BibleF
+00006360: 6c61 672e 4d55 4c54 4942 4f4f 4b20 6e6f  lag.MULTIBOOK no
+00006370: 7420 696e 2066 6c61 6773 2061 6e64 2073  t in flags and s
+00006380: 7461 7274 2e62 6f6f 6b20 213d 2065 6e64  tart.book != end
+00006390: 2e62 6f6f 6b3a 0a20 2020 2020 2020 2020  .book:.         
+000063a0: 2020 2020 2020 2072 6169 7365 204d 756c         raise Mul
+000063b0: 7469 626f 6f6b 5261 6e67 654e 6f74 416c  tibookRangeNotAl
+000063c0: 6c6f 7765 6445 7272 6f72 2866 224d 756c  lowedError(f"Mul
+000063d0: 7469 2d62 6f6f 6b20 7261 6e67 6573 206e  ti-book ranges n
+000063e0: 6f74 2061 6c6c 6f77 6564 2022 202b 200a  ot allowed " + .
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2020 2020 6622 287b 7374 6172 742e 626f      f"({start.bo
+00006430: 6f6b 2e61 6262 7265 767d 2061 6e64 207b  ok.abbrev} and {
+00006440: 656e 642e 626f 6f6b 2e61 6262 7265 767d  end.book.abbrev}
+00006450: 2061 7265 2064 6966 6665 7265 6e74 2922   are different)"
+00006460: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00006470: 2073 7461 7274 203e 2065 6e64 3a0a 2020   start > end:.  
+00006480: 2020 2020 2020 2020 2020 2020 2020 2873                (s
+00006490: 7461 7274 2c20 656e 6429 203d 2028 656e  tart, end) = (en
+000064a0: 642c 2073 7461 7274 290a 2020 2020 2020  d, start).      
+000064b0: 2020 2020 2020 6f62 6a65 6374 2e5f 5f73        object.__s
+000064c0: 6574 6174 7472 5f5f 2873 656c 662c 2022  etattr__(self, "
+000064d0: 7374 6172 7422 2c20 7374 6172 7429 0a20  start", start). 
+000064e0: 2020 2020 2020 2020 2020 206f 626a 6563             objec
+000064f0: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
+00006500: 6c66 2c20 2265 6e64 222c 2065 6e64 290a  lf, "end", end).
+00006510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006520: 726e 0a20 2020 2020 2020 2065 6c69 6620  rn.        elif 
+00006530: 6c65 6e28 6172 6773 2920 3e20 363a 0a20  len(args) > 6:. 
+00006540: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00006550: 2056 616c 7565 4572 726f 7228 2254 6f6f   ValueError("Too
+00006560: 206d 616e 7920 6172 6775 6d65 6e74 7320   many arguments 
+00006570: 7375 7070 6c69 6564 2074 6f20 4269 626c  supplied to Bibl
+00006580: 6552 616e 6765 2229 0a20 2020 2020 2020  eRange").       
+00006590: 2069 6620 6c65 6e28 6172 6773 2920 3d3d   if len(args) ==
+000065a0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+000065b0: 6966 2069 7369 6e73 7461 6e63 6528 6172  if isinstance(ar
+000065c0: 6773 5b30 5d2c 2073 7472 293a 0a20 2020  gs[0], str):.   
+000065d0: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+000065e0: 6765 5f6c 6973 7420 3d20 4269 626c 6552  ge_list = BibleR
+000065f0: 616e 6765 4c69 7374 2861 7267 735b 305d  angeList(args[0]
+00006600: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
+00006610: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006620: 6620 6c65 6e28 7261 6e67 655f 6c69 7374  f len(range_list
+00006630: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
+00006640: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00006650: 6520 496e 7661 6c69 6452 6566 6572 656e  e InvalidReferen
+00006660: 6365 4572 726f 7228 6622 5374 7269 6e67  ceError(f"String
+00006670: 2069 7320 6e6f 7420 6120 7369 6e67 6c65   is not a single
+00006680: 2076 6572 7365 2072 616e 6765 3a20 7b61   verse range: {a
+00006690: 7267 735b 305d 7d22 290a 2020 2020 2020  rgs[0]}").      
+000066a0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+000066b0: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
+000066c0: 662c 2022 7374 6172 7422 2c20 7261 6e67  f, "start", rang
+000066d0: 655f 6c69 7374 5b30 5d2e 7374 6172 7429  e_list[0].start)
+000066e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066f0: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
+00006700: 725f 5f28 7365 6c66 2c20 2265 6e64 222c  r__(self, "end",
+00006710: 2072 616e 6765 5f6c 6973 745b 305d 2e65   range_list[0].e
+00006720: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+00006730: 2020 2020 7265 7475 726e 2020 2020 2020      return      
+00006740: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00006750: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00006760: 7374 616e 6365 2861 7267 735b 305d 2c20  stance(args[0], 
+00006770: 4269 626c 6552 616e 6765 293a 0a20 2020  BibleRange):.   
+00006780: 2020 2020 2020 2020 2020 2020 206f 626a               obj
+00006790: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
+000067a0: 7365 6c66 2c20 2273 7461 7274 222c 2061  self, "start", a
+000067b0: 7267 735b 305d 2e73 7461 7274 290a 2020  rgs[0].start).  
+000067c0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+000067d0: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
+000067e0: 2873 656c 662c 2022 656e 6422 2c20 6172  (self, "end", ar
+000067f0: 6773 5b30 5d2e 656e 6429 0a20 2020 2020  gs[0].end).     
+00006800: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006810: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
+00006820: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00006830: 6528 6172 6773 5b30 5d2c 2042 6962 6c65  e(args[0], Bible
+00006840: 426f 6f6b 293a 0a20 2020 2020 2020 2020  Book):.         
+00006850: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00006860: 7565 4572 726f 7228 2253 696e 676c 6520  ueError("Single 
+00006870: 6172 6775 6d65 6e74 2074 6f20 4269 626c  argument to Bibl
+00006880: 6552 616e 6765 2063 616e 206f 6e6c 7920  eRange can only 
+00006890: 6265 2061 2073 7472 696e 672c 2042 6962  be a string, Bib
+000068a0: 6c65 426f 6f6b 206f 7220 616e 6f74 6865  leBook or anothe
+000068b0: 7220 4269 626c 6552 616e 6765 2229 0a0a  r BibleRange")..
+000068c0: 2020 2020 2020 2020 7374 6172 745f 626f          start_bo
+000068d0: 6f6b 203d 2061 7267 735b 305d 0a20 2020  ok = args[0].   
+000068e0: 2020 2020 2073 7461 7274 5f63 6861 7020       start_chap 
+000068f0: 3d20 6172 6773 5b31 5d20 6966 206c 656e  = args[1] if len
+00006900: 2861 7267 7329 203e 2031 2065 6c73 6520  (args) > 1 else 
+00006910: 4e6f 6e65 0a20 2020 2020 2020 2073 7461  None.        sta
+00006920: 7274 5f76 6572 7365 203d 2061 7267 735b  rt_verse = args[
+00006930: 325d 2069 6620 6c65 6e28 6172 6773 2920  2] if len(args) 
+00006940: 3e20 3220 656c 7365 204e 6f6e 650a 2020  > 2 else None.  
+00006950: 2020 2020 2020 656e 645f 626f 6f6b 203d        end_book =
+00006960: 2061 7267 735b 335d 2069 6620 6c65 6e28   args[3] if len(
+00006970: 6172 6773 2920 3e20 3320 656c 7365 204e  args) > 3 else N
+00006980: 6f6e 650a 2020 2020 2020 2020 656e 645f  one.        end_
+00006990: 6368 6170 203d 2061 7267 735b 345d 2069  chap = args[4] i
+000069a0: 6620 6c65 6e28 6172 6773 2920 3e20 3420  f len(args) > 4 
+000069b0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+000069c0: 2020 656e 645f 7665 7273 6520 3d20 6172    end_verse = ar
+000069d0: 6773 5b35 5d20 6966 206c 656e 2861 7267  gs[5] if len(arg
+000069e0: 7329 203e 2035 2065 6c73 6520 4e6f 6e65  s) > 5 else None
+000069f0: 0a0a 2020 2020 2020 2020 6966 2073 7461  ..        if sta
+00006a00: 7274 5f62 6f6f 6b20 6973 206e 6f74 204e  rt_book is not N
+00006a10: 6f6e 6520 616e 6420 6973 696e 7374 616e  one and isinstan
+00006a20: 6365 2873 7461 7274 5f62 6f6f 6b2c 2073  ce(start_book, s
+00006a30: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00006a40: 2073 7461 7274 5f62 6f6f 6b20 3d20 4269   start_book = Bi
+00006a50: 626c 6542 6f6f 6b2e 6672 6f6d 5f73 7472  bleBook.from_str
+00006a60: 2873 7461 7274 5f62 6f6f 6b2c 2072 6169  (start_book, rai
+00006a70: 7365 5f65 7272 6f72 3d54 7275 6529 0a20  se_error=True). 
+00006a80: 2020 2020 2020 2065 6c69 6620 7374 6172         elif star
+00006a90: 745f 626f 6f6b 2069 7320 6e6f 7420 4e6f  t_book is not No
+00006aa0: 6e65 2061 6e64 206e 6f74 2069 7369 6e73  ne and not isins
+00006ab0: 7461 6e63 6528 7374 6172 745f 626f 6f6b  tance(start_book
+00006ac0: 2c20 4269 626c 6542 6f6f 6b29 3a0a 2020  , BibleBook):.  
+00006ad0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006ae0: 496e 7661 6c69 6452 6566 6572 656e 6365  InvalidReference
+00006af0: 4572 726f 7228 6622 7b73 7461 7274 5f62  Error(f"{start_b
+00006b00: 6f6f 6b7d 2069 7320 6e6f 7420 6120 7661  ook} is not a va
+00006b10: 6c69 6420 4269 626c 6542 6f6f 6b22 290a  lid BibleBook").
+00006b20: 0a20 2020 2020 2020 2069 6620 656e 645f  .        if end_
+00006b30: 626f 6f6b 2069 7320 6e6f 7420 4e6f 6e65  book is not None
+00006b40: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
+00006b50: 656e 645f 626f 6f6b 2c20 7374 7229 3a0a  end_book, str):.
+00006b60: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+00006b70: 626f 6f6b 203d 2042 6962 6c65 426f 6f6b  book = BibleBook
+00006b80: 2e66 726f 6d5f 7374 7228 656e 645f 626f  .from_str(end_bo
+00006b90: 6f6b 2c20 7261 6973 655f 6572 726f 723d  ok, raise_error=
+00006ba0: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
+00006bb0: 6966 2065 6e64 5f62 6f6f 6b20 6973 206e  if end_book is n
+00006bc0: 6f74 204e 6f6e 6520 616e 6420 6e6f 7420  ot None and not 
+00006bd0: 6973 696e 7374 616e 6365 2865 6e64 5f62  isinstance(end_b
+00006be0: 6f6f 6b2c 2042 6962 6c65 426f 6f6b 293a  ook, BibleBook):
+00006bf0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00006c00: 7365 2049 6e76 616c 6964 5265 6665 7265  se InvalidRefere
+00006c10: 6e63 6545 7272 6f72 2866 227b 656e 645f  nceError(f"{end_
+00006c20: 626f 6f6b 7d20 6973 206e 6f74 2061 2076  book} is not a v
+00006c30: 616c 6964 2042 6962 6c65 426f 6f6b 2229  alid BibleBook")
+00006c40: 0a0a 2020 2020 2020 2020 2320 4966 2073  ..        # If s
+00006c50: 7461 7274 203e 2065 6e64 2c20 7377 6170  tart > end, swap
+00006c60: 2061 726f 756e 642e 2054 6865 206c 6f67   around. The log
+00006c70: 6963 2069 7320 6d65 7373 7920 6475 6520  ic is messy due 
+00006c80: 746f 2069 6d70 6c69 6564 2076 616c 7565  to implied value
+00006c90: 7320 7768 656e 2061 7267 7320 6172 6520  s when args are 
+00006ca0: 4e6f 6e65 2e0a 2020 2020 2020 2020 6966  None..        if
+00006cb0: 2073 7461 7274 5f62 6f6f 6b20 6973 206e   start_book is n
+00006cc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00006cd0: 2020 2020 2069 6620 656e 645f 626f 6f6b       if end_book
+00006ce0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00006cf0: 2073 7461 7274 5f62 6f6f 6b20 3e20 656e   start_book > en
+00006d00: 645f 626f 6f6b 3a0a 2020 2020 2020 2020  d_book:.        
+00006d10: 2020 2020 2020 2020 2873 7461 7274 5f62          (start_b
+00006d20: 6f6f 6b2c 2065 6e64 5f62 6f6f 6b29 203d  ook, end_book) =
+00006d30: 2028 656e 645f 626f 6f6b 2c20 7374 6172   (end_book, star
+00006d40: 745f 626f 6f6b 290a 2020 2020 2020 2020  t_book).        
+00006d50: 2020 2020 2020 2020 2873 7461 7274 5f63          (start_c
+00006d60: 6861 702c 2065 6e64 5f63 6861 7029 203d  hap, end_chap) =
+00006d70: 2028 656e 645f 6368 6170 2c20 7374 6172   (end_chap, star
+00006d80: 745f 6368 6170 290a 2020 2020 2020 2020  t_chap).        
+00006d90: 2020 2020 2020 2020 2873 7461 7274 5f76          (start_v
+00006da0: 6572 7365 2c20 656e 645f 7665 7273 6529  erse, end_verse)
+00006db0: 203d 2028 656e 645f 7665 7273 652c 2073   = (end_verse, s
+00006dc0: 7461 7274 5f76 6572 7365 290a 2020 2020  tart_verse).    
+00006dd0: 2020 2020 2020 2020 656c 6966 2028 656e          elif (en
+00006de0: 645f 626f 6f6b 2069 7320 4e6f 6e65 206f  d_book is None o
+00006df0: 7220 656e 645f 626f 6f6b 203d 3d20 7374  r end_book == st
+00006e00: 6172 745f 626f 6f6b 2920 616e 6420 7374  art_book) and st
+00006e10: 6172 745f 6368 6170 2069 7320 6e6f 7420  art_chap is not 
+00006e20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006e30: 2020 2020 2020 6966 2065 6e64 5f63 6861        if end_cha
+00006e40: 7020 6973 206e 6f74 204e 6f6e 6520 616e  p is not None an
+00006e50: 6420 7374 6172 745f 6368 6170 203e 2065  d start_chap > e
+00006e60: 6e64 5f63 6861 703a 0a20 2020 2020 2020  nd_chap:.       
+00006e70: 2020 2020 2020 2020 2020 2020 2028 7374               (st
+00006e80: 6172 745f 6368 6170 2c20 656e 645f 6368  art_chap, end_ch
+00006e90: 6170 2920 3d20 2865 6e64 5f63 6861 702c  ap) = (end_chap,
+00006ea0: 2073 7461 7274 5f63 6861 7029 0a20 2020   start_chap).   
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2028 7374 6172 745f 7665 7273 652c 2065   (start_verse, e
+00006ed0: 6e64 5f76 6572 7365 2920 3d20 2865 6e64  nd_verse) = (end
+00006ee0: 5f76 6572 7365 2c20 7374 6172 745f 7665  _verse, start_ve
+00006ef0: 7273 6529 0a20 2020 2020 2020 2020 2020  rse).           
+00006f00: 2020 2020 2065 6c69 6620 2865 6e64 5f63       elif (end_c
+00006f10: 6861 7020 6973 204e 6f6e 6520 6f72 2065  hap is None or e
+00006f20: 6e64 5f63 6861 7020 3d3d 2073 7461 7274  nd_chap == start
+00006f30: 5f63 6861 7029 2061 6e64 2073 7461 7274  _chap) and start
+00006f40: 5f76 6572 7365 2069 7320 6e6f 7420 4e6f  _verse is not No
+00006f50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00006f60: 2020 2020 2020 2020 6966 2065 6e64 5f76          if end_v
+00006f70: 6572 7365 2069 7320 6e6f 7420 4e6f 6e65  erse is not None
+00006f80: 2061 6e64 2073 7461 7274 5f76 6572 7365   and start_verse
+00006f90: 203e 2065 6e64 5f76 6572 7365 3a0a 2020   > end_verse:.  
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2020 2020 2873 7461 7274 5f76 6572        (start_ver
+00006fc0: 7365 2c20 656e 645f 7665 7273 6529 203d  se, end_verse) =
+00006fd0: 2028 656e 645f 7665 7273 652c 2073 7461   (end_verse, sta
+00006fe0: 7274 5f76 6572 7365 290a 0a20 2020 2020  rt_verse)..     
+00006ff0: 2020 2068 6176 655f 656e 6420 3d20 2865     have_end = (e
+00007000: 6e64 5f62 6f6f 6b20 6973 206e 6f74 204e  nd_book is not N
+00007010: 6f6e 6529 206f 7220 2865 6e64 5f63 6861  one) or (end_cha
+00007020: 7020 6973 206e 6f74 204e 6f6e 6529 206f  p is not None) o
+00007030: 7220 2865 6e64 5f76 6572 7365 2069 7320  r (end_verse is 
+00007040: 6e6f 7420 4e6f 6e65 290a 0a20 2020 2020  not None)..     
+00007050: 2020 2069 6620 7374 6172 745f 626f 6f6b     if start_book
+00007060: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007070: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
+00007080: 6c69 6452 6566 6572 656e 6365 4572 726f  lidReferenceErro
+00007090: 7228 6622 4120 7374 6172 7420 626f 6f6b  r(f"A start book
+000070a0: 2069 7320 6e65 6564 6564 2066 6f72 2061   is needed for a
+000070b0: 2042 6962 6c65 5261 6e67 6522 290a 2020   BibleRange").  
+000070c0: 2020 2020 2020 6966 2073 7461 7274 5f63        if start_c
+000070d0: 6861 7020 6973 204e 6f6e 6520 616e 6420  hap is None and 
+000070e0: 7374 6172 745f 7665 7273 6520 6973 206e  start_verse is n
+000070f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007100: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
+00007110: 6964 5265 6665 7265 6e63 6545 7272 6f72  idReferenceError
+00007120: 2822 5374 6172 7420 7665 7273 6520 6973  ("Start verse is
+00007130: 206d 6973 7369 6e67 2061 2073 7461 7274   missing a start
+00007140: 2063 6861 7074 6572 2229 0a0a 2020 2020   chapter")..    
+00007150: 2020 2020 6966 2073 7461 7274 5f63 6861      if start_cha
+00007160: 7020 6973 204e 6f6e 653a 2023 2053 7461  p is None: # Sta
+00007170: 7274 2069 7320 626f 6f6b 206f 6e6c 790a  rt is book only.
+00007180: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00007190: 7420 3d20 7374 6172 745f 626f 6f6b 2e66  t = start_book.f
+000071a0: 6972 7374 5f76 6572 7365 284e 6f6e 652c  irst_verse(None,
+000071b0: 2066 6c61 6773 290a 2020 2020 2020 2020   flags).        
+000071c0: 2020 2020 6966 206e 6f74 2068 6176 655f      if not have_
+000071d0: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
+000071e0: 2020 2020 2065 6e64 203d 2073 7461 7274       end = start
+000071f0: 5f62 6f6f 6b2e 6c61 7374 5f76 6572 7365  _book.last_verse
+00007200: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+00007210: 7374 6172 745f 7665 7273 6520 6973 204e  start_verse is N
+00007220: 6f6e 653a 2023 2053 7461 7274 2069 7320  one: # Start is 
+00007230: 626f 6f6b 2061 6e64 2063 6861 7020 6f6e  book and chap on
+00007240: 6c79 0a20 2020 2020 2020 2020 2020 2073  ly.            s
+00007250: 7461 7274 203d 2073 7461 7274 5f62 6f6f  tart = start_boo
+00007260: 6b2e 6669 7273 745f 7665 7273 6528 696e  k.first_verse(in
+00007270: 7428 7374 6172 745f 6368 6170 292c 2066  t(start_chap), f
+00007280: 6c61 6773 3d66 6c61 6773 290a 2020 2020  lags=flags).    
+00007290: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
+000072a0: 6176 655f 656e 643a 0a20 2020 2020 2020  ave_end:.       
+000072b0: 2020 2020 2020 2020 2065 6e64 203d 2073           end = s
+000072c0: 7461 7274 5f62 6f6f 6b2e 6c61 7374 5f76  tart_book.last_v
+000072d0: 6572 7365 2869 6e74 2873 7461 7274 5f63  erse(int(start_c
+000072e0: 6861 7029 290a 2020 2020 2020 2020 656c  hap)).        el
+000072f0: 7365 3a20 2320 5374 6172 7420 6973 2062  se: # Start is b
+00007300: 6f6f 6b2c 2063 6861 7020 616e 6420 7665  ook, chap and ve
+00007310: 7273 650a 2020 2020 2020 2020 2020 2020  rse.            
+00007320: 7374 6172 7420 3d20 4269 626c 6556 6572  start = BibleVer
+00007330: 7365 2873 7461 7274 5f62 6f6f 6b2c 2069  se(start_book, i
+00007340: 6e74 2873 7461 7274 5f63 6861 7029 2c20  nt(start_chap), 
+00007350: 696e 7428 7374 6172 745f 7665 7273 6529  int(start_verse)
+00007360: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
+00007370: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00007380: 7420 6861 7665 5f65 6e64 3a20 2320 5369  t have_end: # Si
+00007390: 6e67 6c65 2076 6572 7365 2072 6566 6572  ngle verse refer
+000073a0: 656e 6365 2c20 736f 2065 6e64 2069 7320  ence, so end is 
+000073b0: 7361 6d65 2061 7320 7374 6172 740a 2020  same as start.  
+000073c0: 2020 2020 2020 2020 2020 2020 2020 656e                en
+000073d0: 6420 3d20 4269 626c 6556 6572 7365 2873  d = BibleVerse(s
+000073e0: 7461 7274 5f62 6f6f 6b2c 2069 6e74 2873  tart_book, int(s
+000073f0: 7461 7274 5f63 6861 7029 2c20 696e 7428  tart_chap), int(
+00007400: 7374 6172 745f 7665 7273 6529 2c20 666c  start_verse), fl
+00007410: 6167 733d 666c 6167 7329 0a20 2020 2020  ags=flags).     
+00007420: 2020 200a 2020 2020 2020 2020 6966 2068     .        if h
+00007430: 6176 655f 656e 643a 2023 2057 6520 6861  ave_end: # We ha
+00007440: 7665 2065 6e64 2d70 6f69 6e74 2069 6e66  ve end-point inf
+00007450: 6f0a 2020 2020 2020 2020 2020 2020 6966  o.            if
+00007460: 2065 6e64 5f62 6f6f 6b20 6973 204e 6f6e   end_book is Non
+00007470: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007480: 2020 2065 6e64 5f62 6f6f 6b20 3d20 7374     end_book = st
+00007490: 6172 745f 626f 6f6b 0a20 2020 2020 2020  art_book.       
+000074a0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+000074b0: 2020 6966 2065 6e64 5f63 6861 7020 6973    if end_chap is
+000074c0: 204e 6f6e 6520 616e 6420 656e 645f 7665   None and end_ve
+000074d0: 7273 6520 6973 204e 6f6e 653a 2023 2045  rse is None: # E
+000074e0: 6e64 2069 7320 626f 6f6b 206f 6e6c 790a  nd is book only.
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 656e 6420 3d20 656e 645f 626f 6f6b 2e6c  end = end_book.l
+00007510: 6173 745f 7665 7273 6528 290a 2020 2020  ast_verse().    
+00007520: 2020 2020 2020 2020 656c 6966 2065 6e64          elif end
+00007530: 5f76 6572 7365 2069 7320 4e6f 6e65 3a20  _verse is None: 
+00007540: 2320 456e 6420 6973 2062 6f6f 6b20 616e  # End is book an
+00007550: 6420 6368 6170 206f 6e6c 790a 2020 2020  d chap only.    
+00007560: 2020 2020 2020 2020 2020 2020 656e 6420              end 
+00007570: 3d20 656e 645f 626f 6f6b 2e6c 6173 745f  = end_book.last_
+00007580: 7665 7273 6528 696e 7428 656e 645f 6368  verse(int(end_ch
+00007590: 6170 2929 0a20 2020 2020 2020 2020 2020  ap)).           
+000075a0: 2065 6c69 6620 656e 645f 6368 6170 2069   elif end_chap i
+000075b0: 7320 4e6f 6e65 3a20 2320 456e 6420 6973  s None: # End is
+000075c0: 2062 6f6f 6b20 616e 6420 7665 7273 6520   book and verse 
+000075d0: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
+000075e0: 2020 2020 2069 6620 7374 6172 745f 626f       if start_bo
+000075f0: 6f6b 2021 3d20 656e 645f 626f 6f6b 3a0a  ok != end_book:.
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
+00007620: 6452 6566 6572 656e 6365 4572 726f 7228  dReferenceError(
+00007630: 2245 6e64 2076 6572 7365 2069 7320 6d69  "End verse is mi
+00007640: 7373 696e 6720 616e 2065 6e64 2063 6861  ssing an end cha
+00007650: 7074 6572 2229 0a20 2020 2020 2020 2020  pter").         
+00007660: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2065 6e64 203d 2042 6962 6c65 5665 7273   end = BibleVers
+00007690: 6528 656e 645f 626f 6f6b 2c20 696e 7428  e(end_book, int(
+000076a0: 7374 6172 742e 6368 6170 5f6e 756d 292c  start.chap_num),
+000076b0: 2069 6e74 2865 6e64 5f76 6572 7365 292c   int(end_verse),
+000076c0: 2066 6c61 6773 3d66 6c61 6773 290a 2020   flags=flags).  
+000076d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 656e 6420 3d20 4269 626c 6556 6572 7365  end = BibleVerse
+00007700: 2865 6e64 5f62 6f6f 6b2c 2069 6e74 2865  (end_book, int(e
+00007710: 6e64 5f63 6861 7029 2c20 696e 7428 656e  nd_chap), int(en
+00007720: 645f 7665 7273 6529 2c20 666c 6167 733d  d_verse), flags=
+00007730: 666c 6167 7329 0a0a 2020 2020 2020 2020  flags)..        
+00007740: 6966 2042 6962 6c65 466c 6167 2e4d 554c  if BibleFlag.MUL
+00007750: 5449 424f 4f4b 206e 6f74 2069 6e20 666c  TIBOOK not in fl
+00007760: 6167 7320 616e 6420 7374 6172 742e 626f  ags and start.bo
+00007770: 6f6b 2021 3d20 656e 642e 626f 6f6b 3a0a  ok != end.book:.
+00007780: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00007790: 6520 4d75 6c74 6962 6f6f 6b52 616e 6765  e MultibookRange
+000077a0: 4e6f 7441 6c6c 6f77 6564 4572 726f 7228  NotAllowedError(
+000077b0: 6622 4d75 6c74 692d 626f 6f6b 2072 616e  f"Multi-book ran
+000077c0: 6765 7320 6e6f 7420 616c 6c6f 7765 6420  ges not allowed 
+000077d0: 2220 2b20 0a20 2020 2020 2020 2020 2020  " + .           
+000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007800: 2020 2020 2066 2228 7b73 7461 7274 2e62       f"({start.b
+00007810: 6f6f 6b2e 6162 6272 6576 7d20 616e 6420  ook.abbrev} and 
+00007820: 7b65 6e64 2e62 6f6f 6b2e 6162 6272 6576  {end.book.abbrev
+00007830: 7d20 6172 6520 6469 6666 6572 656e 7429  } are different)
+00007840: 2229 0a0a 2020 2020 2020 2020 6f62 6a65  ")..        obje
+00007850: 6374 2e5f 5f73 6574 6174 7472 5f5f 2873  ct.__setattr__(s
+00007860: 656c 662c 2022 7374 6172 7422 2c20 7374  elf, "start", st
+00007870: 6172 7429 0a20 2020 2020 2020 206f 626a  art).        obj
+00007880: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
+00007890: 7365 6c66 2c20 2265 6e64 222c 2065 6e64  self, "end", end
+000078a0: 290a 0a20 2020 2064 6566 2076 6572 7365  )..    def verse
+000078b0: 5f30 5f74 6f5f 3128 7365 6c66 2920 2d3e  _0_to_1(self) ->
+000078c0: 2027 4269 626c 6552 616e 6765 273a 0a20   'BibleRange':. 
+000078d0: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
+000078e0: 7320 6120 6e65 7720 6042 6962 6c65 5261  s a new `BibleRa
+000078f0: 6e67 6560 2063 7265 6174 6564 2062 7920  nge` created by 
+00007900: 6361 6c6c 696e 6720 6076 6572 7365 5f30  calling `verse_0
+00007910: 5f74 6f5f 3128 2960 206f 6e20 626f 7468  _to_1()` on both
+00007920: 2074 6865 2060 7374 6172 7460 2061 6e64   the `start` and
+00007930: 2060 656e 6460 0a20 2020 2020 2020 2060   `end`.        `
+00007940: 4269 626c 6556 6572 7365 6020 6174 7472  BibleVerse` attr
+00007950: 6962 7574 6573 2e27 2727 0a20 2020 2020  ibutes.'''.     
+00007960: 2020 2072 6574 7572 6e20 4269 626c 6552     return BibleR
+00007970: 616e 6765 2873 7461 7274 3d73 656c 662e  ange(start=self.
+00007980: 7374 6172 742e 7665 7273 655f 305f 746f  start.verse_0_to
+00007990: 5f31 2829 2c20 656e 643d 7365 6c66 2e65  _1(), end=self.e
+000079a0: 6e64 2e76 6572 7365 5f30 5f74 6f5f 3128  nd.verse_0_to_1(
+000079b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000079c0: 2020 2020 2020 2020 2020 2020 2066 6c61               fla
+000079d0: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
+000079e0: 290a 0a20 2020 2064 6566 2076 6572 7365  )..    def verse
+000079f0: 5f31 5f74 6f5f 3028 7365 6c66 2920 2d3e  _1_to_0(self) ->
+00007a00: 2027 4269 626c 6552 616e 6765 273a 0a20   'BibleRange':. 
+00007a10: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
+00007a20: 7320 6120 6e65 7720 6042 6962 6c65 5261  s a new `BibleRa
+00007a30: 6e67 6560 2063 7265 6174 6564 2062 7920  nge` created by 
+00007a40: 6361 6c6c 696e 6720 6076 6572 7365 5f31  calling `verse_1
+00007a50: 5f74 6f5f 3028 2960 206f 6e20 626f 7468  _to_0()` on both
+00007a60: 2074 6865 2060 7374 6172 7460 2061 6e64   the `start` and
+00007a70: 2060 656e 6460 0a20 2020 2020 2020 2060   `end`.        `
+00007a80: 4269 626c 6556 6572 7365 6020 6174 7472  BibleVerse` attr
+00007a90: 6962 7574 6573 2e20 2a2a 4e6f 7465 2a2a  ibutes. **Note**
+00007aa0: 3a20 5468 6520 7661 6c75 6520 6f66 2074  : The value of t
+00007ab0: 6865 2067 6c6f 6261 6c20 6174 7472 6962  he global attrib
+00007ac0: 7574 6520 6062 6962 6c65 7265 662e 7265  ute `bibleref.re
+00007ad0: 662e 666c 6167 7360 2069 7320 2a69 676e  f.flags` is *ign
+00007ae0: 6f72 6564 2a2e 2727 270a 2020 2020 2020  ored*.'''.      
+00007af0: 2020 7265 7475 726e 2042 6962 6c65 5261    return BibleRa
+00007b00: 6e67 6528 7374 6172 743d 7365 6c66 2e73  nge(start=self.s
+00007b10: 7461 7274 2e76 6572 7365 5f31 5f74 6f5f  tart.verse_1_to_
+00007b20: 3028 292c 2065 6e64 3d73 656c 662e 656e  0(), end=self.en
+00007b30: 642e 7665 7273 655f 315f 746f 5f30 2829  d.verse_1_to_0()
+00007b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007b50: 2020 2020 2020 2020 2020 2020 666c 6167              flag
+00007b60: 733d 4269 626c 6546 6c61 672e 414c 4c29  s=BibleFlag.ALL)
+00007b70: 0a0a 2020 2020 6465 6620 6973 5f77 686f  ..    def is_who
+00007b80: 6c65 5f62 6f6f 6b28 7365 6c66 2c20 666c  le_book(self, fl
+00007b90: 6167 733a 2042 6962 6c65 466c 6167 203d  ags: BibleFlag =
+00007ba0: 204e 6f6e 6529 202d 3e20 626f 6f6c 3a0a   None) -> bool:.
+00007bb0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
+00007bc0: 6e73 2060 5472 7565 6020 6966 2074 6869  ns `True` if thi
+00007bd0: 7320 6042 6962 6c65 5261 6e67 6560 2065  s `BibleRange` e
+00007be0: 7861 6374 6c79 2073 7061 6e73 206f 6e65  xactly spans one
+00007bf0: 2077 686f 6c65 2062 6f6f 6b2c 2065 6c73   whole book, els
+00007c00: 6520 6046 616c 7365 602e 2727 270a 2020  e `False`.'''.  
+00007c10: 2020 2020 2020 7265 7475 726e 2020 2873        return  (s
+00007c20: 656c 662e 7374 6172 742e 626f 6f6b 203d  elf.start.book =
+00007c30: 3d20 7365 6c66 2e65 6e64 2e62 6f6f 6b29  = self.end.book)
+00007c40: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+00007c50: 2020 2020 2020 2028 7365 6c66 2e73 7461         (self.sta
+00007c60: 7274 203d 3d20 7365 6c66 2e73 7461 7274  rt == self.start
+00007c70: 2e62 6f6f 6b2e 6669 7273 745f 7665 7273  .book.first_vers
+00007c80: 6528 4e6f 6e65 2c20 666c 6167 7329 2920  e(None, flags)) 
+00007c90: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
+00007ca0: 2020 2020 2020 2873 656c 662e 656e 6420        (self.end 
+00007cb0: 3d3d 2073 656c 662e 656e 642e 626f 6f6b  == self.end.book
+00007cc0: 2e6c 6173 745f 7665 7273 6528 2929 0a0a  .last_verse())..
+00007cd0: 2020 2020 6465 6620 7370 616e 735f 7374      def spans_st
+00007ce0: 6172 745f 626f 6f6b 2873 656c 662c 2066  art_book(self, f
+00007cf0: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+00007d00: 3d20 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a  = None) -> bool:
+00007d10: 0a20 2020 2020 2020 2027 2727 5265 7475  .        '''Retu
+00007d20: 726e 7320 6054 7275 6560 2069 6620 7468  rns `True` if th
+00007d30: 6973 2060 4269 626c 6552 616e 6765 6020  is `BibleRange` 
+00007d40: 696e 636c 7564 6573 2074 6865 2077 686f  includes the who
+00007d50: 6c65 2062 6f6f 6b20 7468 6174 2063 6f6e  le book that con
+00007d60: 7461 696e 7320 7468 6520 6073 7461 7274  tains the `start
+00007d70: 6020 7665 7273 652c 0a20 2020 2020 2020  ` verse,.       
+00007d80: 2065 6c73 6520 6046 616c 7365 602e 2727   else `False`.''
+00007d90: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
+00007da0: 2020 2873 656c 662e 7374 6172 7420 3d3d    (self.start ==
+00007db0: 2073 656c 662e 7374 6172 742e 626f 6f6b   self.start.book
+00007dc0: 2e66 6972 7374 5f76 6572 7365 284e 6f6e  .first_verse(Non
+00007dd0: 652c 2066 6c61 6773 2929 2061 6e64 205c  e, flags)) and \
+00007de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007df0: 2028 7365 6c66 2e65 6e64 203e 3d20 7365   (self.end >= se
+00007e00: 6c66 2e73 7461 7274 2e62 6f6f 6b2e 6c61  lf.start.book.la
+00007e10: 7374 5f76 6572 7365 2829 290a 0a20 2020  st_verse())..   
+00007e20: 2064 6566 2073 7061 6e73 5f65 6e64 5f62   def spans_end_b
+00007e30: 6f6f 6b28 7365 6c66 2c20 666c 6167 733a  ook(self, flags:
+00007e40: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
+00007e50: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
+00007e60: 2020 2020 2727 2752 6574 7572 6e73 2060      '''Returns `
+00007e70: 5472 7565 6020 6966 2074 6869 7320 6042  True` if this `B
+00007e80: 6962 6c65 5261 6e67 6560 2069 6e63 6c75  ibleRange` inclu
+00007e90: 6465 7320 7468 6520 7768 6f6c 6520 626f  des the whole bo
+00007ea0: 6f6b 2074 6861 7420 636f 6e74 6169 6e73  ok that contains
+00007eb0: 2074 6865 2060 656e 6460 2076 6572 7365   the `end` verse
+00007ec0: 2c0a 2020 2020 2020 2020 656c 7365 2060  ,.        else `
+00007ed0: 4661 6c73 6560 2e27 2727 0a20 2020 2020  False`.'''.     
+00007ee0: 2020 2072 6574 7572 6e20 2028 7365 6c66     return  (self
+00007ef0: 2e65 6e64 203d 3d20 7365 6c66 2e65 6e64  .end == self.end
+00007f00: 2e62 6f6f 6b2e 6c61 7374 5f76 6572 7365  .book.last_verse
+00007f10: 2829 2920 616e 6420 5c0a 2020 2020 2020  ()) and \.      
+00007f20: 2020 2020 2020 2020 2020 2873 656c 662e            (self.
+00007f30: 7374 6172 7420 3c3d 2073 656c 662e 656e  start <= self.en
+00007f40: 642e 626f 6f6b 2e66 6972 7374 5f76 6572  d.book.first_ver
+00007f50: 7365 284e 6f6e 652c 2066 6c61 6773 2929  se(None, flags))
+00007f60: 0a0a 2020 2020 6465 6620 6973 5f77 686f  ..    def is_who
+00007f70: 6c65 5f63 6861 7028 7365 6c66 2c20 666c  le_chap(self, fl
+00007f80: 6167 733a 2042 6962 6c65 466c 6167 203d  ags: BibleFlag =
+00007f90: 204e 6f6e 6529 202d 3e20 626f 6f6c 3a0a   None) -> bool:.
+00007fa0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
+00007fb0: 6e73 2060 5472 7565 6020 6966 2074 6869  ns `True` if thi
+00007fc0: 7320 6042 6962 6c65 5261 6e67 6560 2065  s `BibleRange` e
+00007fd0: 7861 6374 6c79 2073 7061 6e73 206f 6e65  xactly spans one
+00007fe0: 2077 686f 6c65 2063 6861 7074 6572 2c20   whole chapter, 
+00007ff0: 656c 7365 2060 4661 6c73 6560 2e27 2727  else `False`.'''
+00008000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008010: 2028 7365 6c66 2e73 7461 7274 2e62 6f6f   (self.start.boo
+00008020: 6b20 3d3d 2073 656c 662e 656e 642e 626f  k == self.end.bo
+00008030: 6f6b 2920 616e 6420 5c0a 2020 2020 2020  ok) and \.      
+00008040: 2020 2020 2020 2020 2020 2873 656c 662e            (self.
+00008050: 7374 6172 7420 3d3d 2073 656c 662e 7374  start == self.st
+00008060: 6172 742e 626f 6f6b 2e66 6972 7374 5f76  art.book.first_v
+00008070: 6572 7365 2873 656c 662e 7374 6172 742e  erse(self.start.
+00008080: 6368 6170 5f6e 756d 2c20 666c 6167 733d  chap_num, flags=
+00008090: 666c 6167 7329 2920 616e 6420 5c0a 2020  flags)) and \.  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2873                (s
+000080b0: 656c 662e 656e 6420 3d3d 2073 656c 662e  elf.end == self.
+000080c0: 656e 642e 626f 6f6b 2e6c 6173 745f 7665  end.book.last_ve
+000080d0: 7273 6528 7365 6c66 2e73 7461 7274 2e63  rse(self.start.c
+000080e0: 6861 705f 6e75 6d29 290a 0a20 2020 2064  hap_num))..    d
+000080f0: 6566 2073 7061 6e73 5f73 7461 7274 5f63  ef spans_start_c
+00008100: 6861 7028 7365 6c66 2c20 666c 6167 733a  hap(self, flags:
+00008110: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
+00008120: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
+00008130: 2020 2020 2727 2752 6574 7572 6e73 2060      '''Returns `
+00008140: 5472 7565 6020 6966 2074 6869 7320 6042  True` if this `B
+00008150: 6962 6c65 5261 6e67 6560 2069 6e63 6c75  ibleRange` inclu
+00008160: 6465 7320 7468 6520 7768 6f6c 6520 6368  des the whole ch
+00008170: 6170 7465 7220 7468 6174 2063 6f6e 7461  apter that conta
+00008180: 696e 7320 7468 6520 6073 7461 7274 6020  ins the `start` 
+00008190: 7665 7273 652c 0a20 2020 2020 2020 2065  verse,.        e
+000081a0: 6c73 6520 6046 616c 7365 602e 2727 270a  lse `False`.'''.
+000081b0: 2020 2020 2020 2020 7265 7475 726e 2020          return  
+000081c0: 2873 656c 662e 7374 6172 7420 3d3d 2073  (self.start == s
+000081d0: 656c 662e 7374 6172 742e 626f 6f6b 2e66  elf.start.book.f
+000081e0: 6972 7374 5f76 6572 7365 2873 656c 662e  irst_verse(self.
+000081f0: 7374 6172 742e 6368 6170 5f6e 756d 2c20  start.chap_num, 
+00008200: 666c 6167 733d 666c 6167 7329 2920 616e  flags=flags)) an
+00008210: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00008220: 2020 2020 2873 656c 662e 656e 6420 3e3d      (self.end >=
+00008230: 2073 656c 662e 7374 6172 742e 626f 6f6b   self.start.book
+00008240: 2e6c 6173 745f 7665 7273 6528 7365 6c66  .last_verse(self
+00008250: 2e73 7461 7274 2e63 6861 705f 6e75 6d29  .start.chap_num)
+00008260: 290a 0a20 2020 2064 6566 2073 7061 6e73  )..    def spans
+00008270: 5f65 6e64 5f63 6861 7028 7365 6c66 2c20  _end_chap(self, 
+00008280: 666c 6167 733a 2042 6962 6c65 466c 6167  flags: BibleFlag
+00008290: 203d 204e 6f6e 6529 202d 3e20 626f 6f6c   = None) -> bool
+000082a0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+000082b0: 7572 6e73 2060 5472 7565 6020 6966 2074  urns `True` if t
+000082c0: 6869 7320 6042 6962 6c65 5261 6e67 6560  his `BibleRange`
+000082d0: 2069 6e63 6c75 6465 7320 7468 6520 7768   includes the wh
+000082e0: 6f6c 6520 6368 6170 7465 7220 7468 6174  ole chapter that
+000082f0: 2063 6f6e 7461 696e 7320 7468 6520 6065   contains the `e
+00008300: 6e64 6020 7665 7273 652c 0a20 2020 2020  nd` verse,.     
+00008310: 2020 2065 6c73 6520 6046 616c 7365 602e     else `False`.
+00008320: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
+00008330: 726e 2020 2873 656c 662e 656e 6420 3d3d  rn  (self.end ==
+00008340: 2073 656c 662e 656e 642e 626f 6f6b 2e6c   self.end.book.l
+00008350: 6173 745f 7665 7273 6528 7365 6c66 2e65  ast_verse(self.e
+00008360: 6e64 2e63 6861 705f 6e75 6d29 2920 616e  nd.chap_num)) an
+00008370: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00008380: 2020 2020 2873 656c 662e 7374 6172 7420      (self.start 
+00008390: 3c3d 2073 656c 662e 656e 642e 626f 6f6b  <= self.end.book
+000083a0: 2e66 6972 7374 5f76 6572 7365 2873 656c  .first_verse(sel
+000083b0: 662e 656e 642e 6368 6170 5f6e 756d 2c20  f.end.chap_num, 
+000083c0: 666c 6167 733d 666c 6167 7329 290a 0a20  flags=flags)).. 
+000083d0: 2020 2064 6566 2069 735f 7369 6e67 6c65     def is_single
+000083e0: 5f76 6572 7365 2873 656c 6629 202d 3e20  _verse(self) -> 
+000083f0: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00008400: 2752 6574 7572 6e73 2060 5472 7565 6020  'Returns `True` 
+00008410: 6966 2074 6865 2060 4269 626c 6552 616e  if the `BibleRan
+00008420: 6765 6020 6578 6163 746c 7920 636f 6e74  ge` exactly cont
+00008430: 6169 6e73 2061 2073 696e 676c 6520 7665  ains a single ve
+00008440: 7273 652c 2065 6c73 6520 6046 616c 7365  rse, else `False
+00008450: 602e 2727 270a 2020 2020 2020 2020 7265  `.'''.        re
+00008460: 7475 726e 2020 2873 656c 662e 7374 6172  turn  (self.star
+00008470: 7420 3d3d 2073 656c 662e 656e 6429 0a0a  t == self.end)..
+00008480: 2020 2020 6465 6620 7370 6c69 7428 7365      def split(se
+00008490: 6c66 2c20 2a2c 2062 795f 626f 6f6b 3a20  lf, *, by_book: 
+000084a0: 626f 6f6c 203d 2046 616c 7365 2c20 6279  bool = False, by
+000084b0: 5f63 6861 703a 2062 6f6f 6c20 3d20 4661  _chap: bool = Fa
+000084c0: 6c73 652c 206e 756d 5f76 6572 7365 733a  lse, num_verses:
+000084d0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+000084e0: 2020 2020 2020 2020 2020 2020 666c 6167              flag
+000084f0: 733a 2042 6962 6c65 466c 6167 203d 204e  s: BibleFlag = N
+00008500: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
+00008510: 2753 706c 6974 2074 6869 7320 6042 6962  'Split this `Bib
+00008520: 6c65 5261 6e67 6560 2069 6e74 6f20 6120  leRange` into a 
+00008530: 6042 6962 6c65 5261 6e67 654c 6973 7460  `BibleRangeList`
+00008540: 206f 6620 736d 616c 6c65 7220 636f 6e73   of smaller cons
+00008550: 6563 7574 6976 6520 7261 6e67 6573 2c20  ecutive ranges, 
+00008560: 6173 2066 6f6c 6c6f 7773 3a0a 2020 2020  as follows:.    
+00008570: 2020 2020 0a20 2020 2020 2020 202d 2049      .        - I
+00008580: 6620 6062 795f 626f 6f6b 6020 6973 2060  f `by_book` is `
+00008590: 5472 7565 602c 2073 706c 6974 7320 6172  True`, splits ar
+000085a0: 6520 6d61 6465 2061 7420 7468 6520 656e  e made at the en
+000085b0: 6420 6f66 2065 6163 6820 626f 6f6b 2e0a  d of each book..
+000085c0: 2020 2020 2020 2020 2d20 4966 2060 6279          - If `by
+000085d0: 5f63 6861 7060 2069 7320 6054 7275 6560  _chap` is `True`
+000085e0: 2c20 7370 6c69 7473 2061 7265 206d 6164  , splits are mad
+000085f0: 6520 656e 6420 6f66 2065 6163 6820 6368  e end of each ch
+00008600: 6170 7465 722e 0a20 2020 2020 2020 202d  apter..        -
+00008610: 2049 6620 606e 756d 5f76 6572 7365 7360   If `num_verses`
+00008620: 2069 7320 7370 6563 6966 6965 642c 2073   is specified, s
+00008630: 706c 6974 7320 6172 6520 6d61 6465 2061  plits are made a
+00008640: 6674 6572 2028 6e6f 206d 6f72 6520 7468  fter (no more th
+00008650: 616e 2920 7468 6520 7370 6563 6966 6965  an) the specifie
+00008660: 6420 6e75 6d62 6572 206f 6620 7665 7273  d number of vers
+00008670: 6573 2e0a 2020 2020 2020 2020 2d20 6062  es..        - `b
+00008680: 795f 626f 6f6b 602c 2060 6279 5f63 6861  y_book`, `by_cha
+00008690: 7060 2061 6e64 2060 6e75 6d5f 7665 7273  p` and `num_vers
+000086a0: 6573 6020 6361 6e20 6265 2073 6574 2069  es` can be set i
+000086b0: 6e20 616e 7920 636f 6d62 696e 6174 696f  n any combinatio
+000086c0: 6e2c 2062 7574 206f 6e65 206f 6620 7468  n, but one of th
+000086d0: 656d 206d 7573 7420 6265 2060 5472 7565  em must be `True
+000086e0: 602c 0a20 2020 2020 2020 2020 206f 7468  `,.          oth
+000086f0: 6572 7769 7365 2061 2060 5661 6c75 6545  erwise a `ValueE
+00008700: 7272 6f72 6020 7769 6c6c 2062 6520 7261  rror` will be ra
+00008710: 6973 6564 2e0a 2020 2020 2020 2020 2727  ised..        ''
+00008720: 270a 2020 2020 2020 2020 6966 206e 6f74  '.        if not
+00008730: 2028 6279 5f62 6f6f 6b20 6f72 2062 795f   (by_book or by_
+00008740: 6368 6170 206f 7220 6e75 6d5f 7665 7273  chap or num_vers
+00008750: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00008760: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00008770: 7228 224d 7573 7420 7370 6c69 7420 6279  r("Must split by
+00008780: 2061 7420 6c65 6173 7420 6f6e 6520 6f66   at least one of
+00008790: 2062 6f6f 6b2c 2063 6861 7074 6572 2c20   book, chapter, 
+000087a0: 6f72 206e 756d 6265 7220 6f66 2076 6572  or number of ver
+000087b0: 7365 7322 290a 0a20 2020 2020 2020 2066  ses")..        f
+000087c0: 6c61 6773 203d 2028 666c 6167 7320 6f72  lags = (flags or
+000087d0: 2067 6c6f 6261 6c73 2829 5b27 666c 6167   globals()['flag
+000087e0: 7327 5d20 6f72 2042 6962 6c65 466c 6167  s'] or BibleFlag
+000087f0: 2e4e 4f4e 4529 0a20 2020 2020 2020 2023  .NONE).        #
+00008800: 2053 6574 2066 6c61 6773 2069 6620 6f75   Set flags if ou
+00008810: 7220 6174 7472 6962 7574 6573 2069 6d70  r attributes imp
+00008820: 6c79 2074 6865 7920 7368 6f75 6c64 2062  ly they should b
+00008830: 6520 7365 740a 2020 2020 2020 2020 6966  e set.        if
+00008840: 2073 656c 662e 7374 6172 742e 626f 6f6b   self.start.book
+00008850: 2021 3d20 7365 6c66 2e65 6e64 2e62 6f6f   != self.end.boo
+00008860: 6b3a 0a20 2020 2020 2020 2020 2020 2066  k:.            f
+00008870: 6c61 6773 207c 3d20 4269 626c 6546 6c61  lags |= BibleFla
+00008880: 672e 4d55 4c54 4942 4f4f 4b0a 2020 2020  g.MULTIBOOK.    
+00008890: 2020 2020 6966 2073 656c 662e 7374 6172      if self.star
+000088a0: 742e 7665 7273 655f 6e75 6d20 3d3d 2030  t.verse_num == 0
+000088b0: 206f 7220 7365 6c66 2e65 6e64 2e76 6572   or self.end.ver
+000088c0: 7365 5f6e 756d 203d 3d20 303a 0a20 2020  se_num == 0:.   
+000088d0: 2020 2020 2020 2020 2066 6c61 6773 207c           flags |
+000088e0: 3d20 4269 626c 6546 6c61 672e 5645 5253  = BibleFlag.VERS
+000088f0: 455f 300a 0a20 2020 2020 2020 2073 706c  E_0..        spl
+00008900: 6974 5f72 6573 756c 7420 3d20 5b73 656c  it_result = [sel
+00008910: 665d 0a20 2020 2020 2020 200a 2020 2020  f].        .    
+00008920: 2020 2020 6966 2062 795f 626f 6f6b 3a0a      if by_book:.
+00008930: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00008940: 7370 6c69 7420 3d20 5b5d 0a20 2020 2020  split = [].     
+00008950: 2020 2020 2020 2066 6f72 2072 616e 6765         for range
+00008960: 5f74 6f5f 7370 6c69 7420 696e 2073 706c  _to_split in spl
+00008970: 6974 5f72 6573 756c 743a 0a20 2020 2020  it_result:.     
+00008980: 2020 2020 2020 2020 2020 2072 616e 6765             range
+00008990: 5f73 7461 7274 203d 2072 616e 6765 5f74  _start = range_t
+000089a0: 6f5f 7370 6c69 742e 7374 6172 740a 2020  o_split.start.  
+000089b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000089c0: 6e67 655f 656e 6420 3d20 7261 6e67 655f  nge_end = range_
+000089d0: 7374 6172 742e 626f 6f6b 2e6c 6173 745f  start.book.last_
+000089e0: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
+000089f0: 2020 2020 2020 2020 7768 696c 6520 7261          while ra
+00008a00: 6e67 655f 656e 6420 3c20 7261 6e67 655f  nge_end < range_
+00008a10: 746f 5f73 706c 6974 2e65 6e64 3a0a 2020  to_split.end:.  
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 2020 6e65 775f 7370 6c69 742e 6170 7065    new_split.appe
+00008a40: 6e64 2842 6962 6c65 5261 6e67 6528 7374  nd(BibleRange(st
+00008a50: 6172 743d 7261 6e67 655f 7374 6172 742c  art=range_start,
+00008a60: 2065 6e64 3d72 616e 6765 5f65 6e64 2c20   end=range_end, 
+00008a70: 666c 6167 733d 666c 6167 7329 290a 2020  flags=flags)).  
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 7261 6e67 655f 7374 6172 7420 3d20    range_start = 
+00008aa0: 7261 6e67 655f 656e 642e 6164 645f 6e75  range_end.add_nu
+00008ab0: 6d5f 7665 7273 6573 2831 2c20 666c 6167  m_verses(1, flag
+00008ac0: 733d 666c 6167 7329 0a20 2020 2020 2020  s=flags).       
+00008ad0: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+00008ae0: 6765 5f65 6e64 203d 2072 616e 6765 5f73  ge_end = range_s
+00008af0: 7461 7274 2e62 6f6f 6b2e 6c61 7374 5f76  tart.book.last_v
+00008b00: 6572 7365 2829 0a20 2020 2020 2020 2020  erse().         
+00008b10: 2020 2020 2020 206e 6577 5f73 706c 6974         new_split
+00008b20: 2e61 7070 656e 6428 4269 626c 6552 616e  .append(BibleRan
+00008b30: 6765 2873 7461 7274 3d72 616e 6765 5f73  ge(start=range_s
+00008b40: 7461 7274 2c20 656e 643d 7261 6e67 655f  tart, end=range_
+00008b50: 746f 5f73 706c 6974 2e65 6e64 2c20 666c  to_split.end, fl
+00008b60: 6167 733d 666c 6167 7329 290a 2020 2020  ags=flags)).    
+00008b70: 2020 2020 2020 2020 7370 6c69 745f 7265          split_re
+00008b80: 7375 6c74 203d 206e 6577 5f73 706c 6974  sult = new_split
+00008b90: 0a0a 2020 2020 2020 2020 6966 2062 795f  ..        if by_
+00008ba0: 6368 6170 3a0a 2020 2020 2020 2020 2020  chap:.          
+00008bb0: 2020 6e65 775f 7370 6c69 7420 3d20 5b5d    new_split = []
+00008bc0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00008bd0: 2072 616e 6765 5f74 6f5f 7370 6c69 7420   range_to_split 
+00008be0: 696e 2073 706c 6974 5f72 6573 756c 743a  in split_result:
+00008bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c00: 2072 616e 6765 5f73 7461 7274 203d 2072   range_start = r
+00008c10: 616e 6765 5f74 6f5f 7370 6c69 742e 7374  ange_to_split.st
+00008c20: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
+00008c30: 2020 2020 7261 6e67 655f 656e 6420 3d20      range_end = 
+00008c40: 7261 6e67 655f 7374 6172 742e 6c61 7374  range_start.last
+00008c50: 5f76 6572 7365 2829 0a20 2020 2020 2020  _verse().       
+00008c60: 2020 2020 2020 2020 2077 6869 6c65 2072           while r
+00008c70: 616e 6765 5f65 6e64 203c 2072 616e 6765  ange_end < range
+00008c80: 5f74 6f5f 7370 6c69 742e 656e 643a 0a20  _to_split.end:. 
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 206e 6577 5f73 706c 6974 2e61 7070     new_split.app
+00008cb0: 656e 6428 4269 626c 6552 616e 6765 2873  end(BibleRange(s
+00008cc0: 7461 7274 3d72 616e 6765 5f73 7461 7274  tart=range_start
+00008cd0: 2c20 656e 643d 7261 6e67 655f 656e 642c  , end=range_end,
+00008ce0: 2066 6c61 6773 3d66 6c61 6773 2929 0a20   flags=flags)). 
+00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 2072 616e 6765 5f73 7461 7274 203d     range_start =
+00008d10: 2072 616e 6765 5f65 6e64 2e61 6464 5f6e   range_end.add_n
+00008d20: 756d 5f76 6572 7365 7328 312c 2066 6c61  um_verses(1, fla
+00008d30: 6773 3d66 6c61 6773 290a 2020 2020 2020  gs=flags).      
+00008d40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00008d50: 6e67 655f 656e 6420 3d20 7261 6e67 655f  nge_end = range_
+00008d60: 7374 6172 742e 6c61 7374 5f76 6572 7365  start.last_verse
+00008d70: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00008d80: 2020 206e 6577 5f73 706c 6974 2e61 7070     new_split.app
+00008d90: 656e 6428 4269 626c 6552 616e 6765 2873  end(BibleRange(s
+00008da0: 7461 7274 3d72 616e 6765 5f73 7461 7274  tart=range_start
+00008db0: 2c20 656e 643d 7261 6e67 655f 746f 5f73  , end=range_to_s
+00008dc0: 706c 6974 2e65 6e64 2c20 666c 6167 733d  plit.end, flags=
+00008dd0: 666c 6167 7329 290a 2020 2020 2020 2020  flags)).        
+00008de0: 2020 2020 7370 6c69 745f 7265 7375 6c74      split_result
+00008df0: 203d 206e 6577 5f73 706c 6974 0a0a 2020   = new_split..  
+00008e00: 2020 2020 2020 6966 206e 756d 5f76 6572        if num_ver
+00008e10: 7365 7320 6973 206e 6f74 204e 6f6e 653a  ses is not None:
+00008e20: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+00008e30: 5f73 706c 6974 203d 205b 5d0a 2020 2020  _split = [].    
+00008e40: 2020 2020 2020 2020 666f 7220 7261 6e67          for rang
+00008e50: 655f 746f 5f73 706c 6974 2069 6e20 7370  e_to_split in sp
+00008e60: 6c69 745f 7265 7375 6c74 3a0a 2020 2020  lit_result:.    
+00008e70: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+00008e80: 655f 7374 6172 7420 3d20 4269 626c 6556  e_start = BibleV
+00008e90: 6572 7365 2872 616e 6765 5f74 6f5f 7370  erse(range_to_sp
+00008ea0: 6c69 742e 7374 6172 742c 2066 6c61 6773  lit.start, flags
+00008eb0: 3d66 6c61 6773 290a 2020 2020 2020 2020  =flags).        
+00008ec0: 2020 2020 2020 2020 7261 6e67 655f 656e          range_en
+00008ed0: 6420 3d20 7261 6e67 655f 7374 6172 742e  d = range_start.
+00008ee0: 6164 645f 6e75 6d5f 7665 7273 6573 286e  add_num_verses(n
+00008ef0: 756d 5f76 6572 7365 7320 2d20 312c 2066  um_verses - 1, f
+00008f00: 6c61 6773 290a 2020 2020 2020 2020 2020  lags).          
+00008f10: 2020 2020 2020 7768 696c 6520 7261 6e67        while rang
+00008f20: 655f 656e 6420 6973 206e 6f74 204e 6f6e  e_end is not Non
+00008f30: 6520 616e 6420 7261 6e67 655f 656e 6420  e and range_end 
+00008f40: 3c20 7261 6e67 655f 746f 5f73 706c 6974  < range_to_split
+00008f50: 2e65 6e64 3a0a 2020 2020 2020 2020 2020  .end:.          
+00008f60: 2020 2020 2020 2020 2020 6e65 775f 7370            new_sp
+00008f70: 6c69 742e 6170 7065 6e64 2842 6962 6c65  lit.append(Bible
+00008f80: 5261 6e67 6528 7374 6172 743d 7261 6e67  Range(start=rang
+00008f90: 655f 7374 6172 742c 2065 6e64 3d72 616e  e_start, end=ran
+00008fa0: 6765 5f65 6e64 2c20 666c 6167 733d 666c  ge_end, flags=fl
+00008fb0: 6167 7329 290a 2020 2020 2020 2020 2020  ags)).          
+00008fc0: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
+00008fd0: 7374 6172 7420 3d20 7261 6e67 655f 656e  start = range_en
+00008fe0: 642e 6164 645f 6e75 6d5f 7665 7273 6573  d.add_num_verses
+00008ff0: 2831 2c20 666c 6167 7329 0a20 2020 2020  (1, flags).     
+00009000: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009010: 616e 6765 5f65 6e64 203d 2072 616e 6765  ange_end = range
+00009020: 5f65 6e64 2e61 6464 5f6e 756d 5f76 6572  _end.add_num_ver
+00009030: 7365 7328 6e75 6d5f 7665 7273 6573 2c20  ses(num_verses, 
+00009040: 666c 6167 7329 0a20 2020 2020 2020 2020  flags).         
+00009050: 2020 2020 2020 206e 6577 5f73 706c 6974         new_split
+00009060: 2e61 7070 656e 6428 4269 626c 6552 616e  .append(BibleRan
+00009070: 6765 2873 7461 7274 3d72 616e 6765 5f73  ge(start=range_s
+00009080: 7461 7274 2c20 656e 643d 7261 6e67 655f  tart, end=range_
+00009090: 746f 5f73 706c 6974 2e65 6e64 2c20 666c  to_split.end, fl
+000090a0: 6167 733d 666c 6167 7329 290a 2020 2020  ags=flags)).    
+000090b0: 2020 2020 2020 2020 7370 6c69 745f 7265          split_re
+000090c0: 7375 6c74 203d 206e 6577 5f73 706c 6974  sult = new_split
+000090d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000090e0: 2020 7265 7475 726e 2042 6962 6c65 5261    return BibleRa
+000090f0: 6e67 654c 6973 7428 7370 6c69 745f 7265  ngeList(split_re
+00009100: 7375 6c74 2c20 666c 6167 733d 666c 6167  sult, flags=flag
+00009110: 7329 0a0a 2020 2020 6465 6620 6973 5f64  s)..    def is_d
+00009120: 6973 6a6f 696e 7428 7365 6c66 2c20 6f74  isjoint(self, ot
+00009130: 6865 725f 7265 663a 2027 4269 626c 6552  her_ref: 'BibleR
+00009140: 6566 2729 202d 3e20 626f 6f6c 3a0a 2020  ef') -> bool:.  
+00009150: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+00009160: 2060 5472 7565 6020 6966 2074 6869 7320   `True` if this 
+00009170: 7261 6e67 6520 646f 6573 6e27 7420 6f76  range doesn't ov
+00009180: 6572 6c61 7020 7769 7468 2061 6e79 2076  erlap with any v
+00009190: 6572 7365 7320 696e 2060 6f74 6865 725f  erses in `other_
+000091a0: 7265 6660 2c20 6f74 6865 7277 6973 6520  ref`, otherwise 
+000091b0: 6046 616c 7365 602e 0a20 2020 2020 2020  `False`..       
+000091c0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
+000091d0: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+000091e0: 5f72 6566 2c20 4269 626c 6552 616e 6765  _ref, BibleRange
+000091f0: 4c69 7374 293a 0a20 2020 2020 2020 2020  List):.         
+00009200: 2020 2072 6574 7572 6e20 6f74 6865 725f     return other_
+00009210: 7265 662e 6973 5f64 6973 6a6f 696e 7428  ref.is_disjoint(
+00009220: 7365 6c66 2920 2320 6973 5f64 6973 6a6f  self) # is_disjo
+00009230: 696e 7428 2920 6973 2063 6f6d 6d75 7461  int() is commuta
+00009240: 7469 7665 2c20 736f 2075 7365 2074 6865  tive, so use the
+00009250: 206c 6973 7420 696d 706c 656d 656e 7461   list implementa
+00009260: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+00009270: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+00009280: 5f72 6566 2c20 4269 626c 6556 6572 7365  _ref, BibleVerse
+00009290: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+000092a0: 2043 6f6e 7665 7274 2074 6f20 4269 626c   Convert to Bibl
+000092b0: 6552 616e 6765 2028 616e 6420 7765 2064  eRange (and we d
+000092c0: 6f6e 2774 2065 6e66 6f72 6365 2065 7869  on't enforce exi
+000092d0: 7374 696e 6720 666c 6167 7320 666f 7220  sting flags for 
+000092e0: 636f 6e76 6572 7369 6f6e 7329 0a20 2020  conversions).   
+000092f0: 2020 2020 2020 2020 206f 7468 6572 5f72           other_r
+00009300: 6566 203d 2042 6962 6c65 5261 6e67 6528  ef = BibleRange(
+00009310: 7374 6172 743d 6f74 6865 725f 7265 662c  start=other_ref,
+00009320: 2065 6e64 3d6f 7468 6572 5f72 6566 2c20   end=other_ref, 
+00009330: 666c 6167 733d 4269 626c 6546 6c61 672e  flags=BibleFlag.
+00009340: 414c 4c29 0a20 2020 2020 2020 2069 6620  ALL).        if 
+00009350: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+00009360: 5f72 6566 2c20 4269 626c 6552 616e 6765  _ref, BibleRange
+00009370: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00009380: 6f77 6572 2c20 6869 6768 6572 203d 2028  ower, higher = (
+00009390: 7365 6c66 2c20 6f74 6865 725f 7265 6629  self, other_ref)
+000093a0: 2069 6620 7365 6c66 203c 206f 7468 6572   if self < other
+000093b0: 5f72 6566 2065 6c73 6520 286f 7468 6572  _ref else (other
+000093c0: 5f72 6566 2c20 7365 6c66 290a 2020 2020  _ref, self).    
+000093d0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+000093e0: 6f77 6572 2e65 6e64 203c 2068 6967 6865  ower.end < highe
+000093f0: 722e 7374 6172 740a 2020 2020 2020 2020  r.start.        
+00009400: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009410: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00009420: 6f72 2866 227b 6f74 6865 725f 7265 667d  or(f"{other_ref}
+00009430: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
+00009440: 4269 626c 6552 6566 2229 0a0a 2020 2020  BibleRef")..    
+00009450: 6465 6620 6973 5f61 646a 6163 656e 7428  def is_adjacent(
+00009460: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
+00009470: 2027 4269 626c 6552 6566 272c 2066 6c61   'BibleRef', fla
+00009480: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
+00009490: 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a 0a20  None) -> bool:. 
+000094a0: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
+000094b0: 7320 6054 7275 6560 2069 6620 7468 6973  s `True` if this
+000094c0: 2072 616e 6765 2069 7320 6164 6a61 6365   range is adjace
+000094d0: 6e74 2074 6f20 606f 7468 6572 5f72 6566  nt to `other_ref
+000094e0: 602c 206f 7468 6572 7769 7365 2060 4661  `, otherwise `Fa
+000094f0: 6c73 6560 2e0a 2020 2020 2020 2020 0a20  lse`..        . 
+00009500: 2020 2020 2020 2041 2060 4269 626c 6552         A `BibleR
+00009510: 616e 6765 6020 6973 2063 6f6e 7369 6465  ange` is conside
+00009520: 7265 6420 6164 6a61 6365 6e74 2074 6f20  red adjacent to 
+00009530: 616e 6f74 6865 7220 6042 6962 6c65 5665  another `BibleVe
+00009540: 7273 6560 206f 7220 6042 6962 6c65 5261  rse` or `BibleRa
+00009550: 6e67 6560 2069 6620 7468 6569 7220 626f  nge` if their bo
+00009560: 756e 6473 2061 7265 2061 2073 696e 676c  unds are a singl
+00009570: 650a 2020 2020 2020 2020 7665 7273 6520  e.        verse 
+00009580: 6170 6172 742e 2041 2060 4269 626c 6552  apart. A `BibleR
+00009590: 616e 6765 6020 6973 2063 6f6e 7369 6465  ange` is conside
+000095a0: 7265 6420 6164 6a61 6365 6e74 2074 6f20  red adjacent to 
+000095b0: 6120 6042 6962 6c65 5261 6e67 654c 6973  a `BibleRangeLis
+000095c0: 7460 2069 6620 6974 2069 7320 6469 736a  t` if it is disj
+000095d0: 6f69 6e74 0a20 2020 2020 2020 2074 6f20  oint.        to 
+000095e0: 7468 6520 656e 7469 7265 206c 6973 7420  the entire list 
+000095f0: 616e 6420 6164 6a61 6365 6e74 2074 6f20  and adjacent to 
+00009600: 6174 206c 6561 7374 206f 6e65 2060 4269  at least one `Bi
+00009610: 626c 6552 616e 6765 6020 696e 2074 6865  bleRange` in the
+00009620: 206c 6973 742e 0a20 2020 2020 2020 2027   list..        '
+00009630: 2727 0a20 2020 2020 2020 2069 6620 6973  ''.        if is
+00009640: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+00009650: 6566 2c20 4269 626c 6552 616e 6765 4c69  ef, BibleRangeLi
+00009660: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00009670: 2023 2042 6962 6c65 5261 6e67 654c 6973   # BibleRangeLis
+00009680: 7420 646f 6573 6e27 7420 6465 6669 6e65  t doesn't define
+00009690: 2069 735f 6164 6a61 6365 6e74 2829 2c20   is_adjacent(), 
+000096a0: 736f 2077 6520 6861 7665 2074 6f20 696d  so we have to im
+000096b0: 706c 656d 656e 7420 6865 7265 0a20 2020  plement here.   
+000096c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000096d0: 6f74 6865 725f 7265 662e 6973 5f64 6973  other_ref.is_dis
+000096e0: 6a6f 696e 7428 7365 6c66 2920 616e 6420  joint(self) and 
+000096f0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+00009700: 2020 2020 2061 6e79 2873 656c 662e 6973       any(self.is
+00009710: 5f61 646a 6163 656e 7428 6f74 6865 725f  _adjacent(other_
+00009720: 7261 6e67 6529 2066 6f72 206f 7468 6572  range) for other
+00009730: 5f72 616e 6765 2069 6e20 6f74 6865 725f  _range in other_
+00009740: 7265 6629 200a 2020 2020 2020 2020 6966  ref) .        if
+00009750: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+00009760: 725f 7265 662c 2042 6962 6c65 5665 7273  r_ref, BibleVers
+00009770: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00009780: 2320 436f 6e76 6572 7420 746f 2042 6962  # Convert to Bib
+00009790: 6c65 5261 6e67 6520 2861 6e64 2077 6520  leRange (and we 
+000097a0: 646f 6e27 7420 656e 666f 7263 6520 6578  don't enforce ex
+000097b0: 6973 7469 6e67 2066 6c61 6773 2066 6f72  isting flags for
+000097c0: 2063 6f6e 7665 7273 696f 6e73 290a 2020   conversions).  
+000097d0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+000097e0: 7265 6620 3d20 4269 626c 6552 616e 6765  ref = BibleRange
+000097f0: 2873 7461 7274 3d6f 7468 6572 5f72 6566  (start=other_ref
+00009800: 2c20 656e 643d 6f74 6865 725f 7265 662c  , end=other_ref,
+00009810: 2066 6c61 6773 3d42 6962 6c65 466c 6167   flags=BibleFlag
+00009820: 2e41 4c4c 290a 2020 2020 2020 2020 6966  .ALL).        if
+00009830: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+00009840: 725f 7265 662c 2042 6962 6c65 5261 6e67  r_ref, BibleRang
+00009850: 6529 3a20 2020 2020 2020 200a 2020 2020  e):        .    
+00009860: 2020 2020 2020 2020 6c6f 7765 722c 2068          lower, h
+00009870: 6967 6865 7220 3d20 2873 656c 662c 206f  igher = (self, o
+00009880: 7468 6572 5f72 6566 2920 6966 2073 656c  ther_ref) if sel
+00009890: 6620 3c20 6f74 6865 725f 7265 6620 656c  f < other_ref el
+000098a0: 7365 2028 6f74 6865 725f 7265 662c 2073  se (other_ref, s
+000098b0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
+000098c0: 2072 6574 7572 6e20 286c 6f77 6572 2e65   return (lower.e
+000098d0: 6e64 2e61 6464 5f6e 756d 5f76 6572 7365  nd.add_num_verse
+000098e0: 7328 312c 2066 6c61 6773 3d66 6c61 6773  s(1, flags=flags
+000098f0: 2920 3d3d 2068 6967 6865 722e 7374 6172  ) == higher.star
+00009900: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
+00009910: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00009920: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00009930: 7b6f 7468 6572 5f72 6566 7d20 6973 206e  {other_ref} is n
+00009940: 6f74 2061 2076 616c 6964 2042 6962 6c65  ot a valid Bible
+00009950: 5265 6622 290a 0a20 2020 2064 6566 2063  Ref")..    def c
+00009960: 6f6e 7461 696e 7328 7365 6c66 2c20 6f74  ontains(self, ot
+00009970: 6865 725f 7265 663a 2027 4269 626c 6552  her_ref: 'BibleR
+00009980: 6566 2729 202d 3e20 626f 6f6c 3a0a 2020  ef') -> bool:.  
+00009990: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+000099a0: 2060 5472 7565 6020 6966 2061 6c6c 2074   `True` if all t
+000099b0: 6865 2076 6572 7365 7320 696e 2060 6f74  he verses in `ot
+000099c0: 6865 725f 7265 6660 2066 616c 6c20 7769  her_ref` fall wi
+000099d0: 7468 696e 2074 6869 7320 6042 6962 6c65  thin this `Bible
+000099e0: 5261 6e67 6560 2e20 4f74 6865 7277 6973  Range`. Otherwis
+000099f0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00009a00: 7320 6046 616c 7365 602e 0a0a 2020 2020  s `False`...    
+00009a10: 2020 2020 5468 6520 7361 6d65 2072 6573      The same res
+00009a20: 756c 7420 6973 2072 6574 7572 6e65 6420  ult is returned 
+00009a30: 7573 696e 6720 7468 6520 2769 6e27 206f  using the 'in' o
+00009a40: 7065 7261 746f 7220 2869 2e65 2e20 606f  perator (i.e. `o
+00009a50: 7468 6572 5f72 6566 2069 6e20 6269 626c  ther_ref in bibl
+00009a60: 655f 7261 6e67 6560 292e 0a20 2020 2020  e_range`)..     
+00009a70: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+00009a80: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+00009a90: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
+00009aa0: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
+00009ab0: 2020 2020 2023 2063 6f6e 7461 696e 7328       # contains(
+00009ac0: 2920 6973 206e 6f74 2063 6f6d 6d75 7461  ) is not commuta
+00009ad0: 7469 7665 2c20 6275 7420 7765 2073 7469  tive, but we sti
+00009ae0: 6c6c 2075 7365 2074 6865 2042 6962 6c65  ll use the Bible
+00009af0: 5261 6e67 654c 6973 7420 696d 706c 656d  RangeList implem
+00009b00: 656e 7461 7469 6f6e 2e0a 2020 2020 2020  entation..      
+00009b10: 2020 2020 2020 7265 7475 726e 2042 6962        return Bib
+00009b20: 6c65 5261 6e67 654c 6973 7428 5b73 656c  leRangeList([sel
+00009b30: 665d 292e 636f 6e74 6169 6e73 286f 7468  f]).contains(oth
+00009b40: 6572 5f72 6566 290a 2020 2020 2020 2020  er_ref).        
+00009b50: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00009b60: 6865 725f 7265 662c 2042 6962 6c65 5665  her_ref, BibleVe
+00009b70: 7273 6529 3a0a 2020 2020 2020 2020 2020  rse):.          
+00009b80: 2020 2320 436f 6e76 6572 7420 746f 2042    # Convert to B
+00009b90: 6962 6c65 5261 6e67 6520 2861 6e64 2077  ibleRange (and w
+00009ba0: 6520 646f 6e27 7420 656e 666f 7263 6520  e don't enforce 
+00009bb0: 6578 6973 7469 6e67 2066 6c61 6773 2066  existing flags f
+00009bc0: 6f72 2063 6f6e 7665 7273 696f 6e73 290a  or conversions).
+00009bd0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+00009be0: 725f 7265 6620 3d20 4269 626c 6552 616e  r_ref = BibleRan
+00009bf0: 6765 2873 7461 7274 3d6f 7468 6572 5f72  ge(start=other_r
+00009c00: 6566 2c20 656e 643d 6f74 6865 725f 7265  ef, end=other_re
+00009c10: 662c 2066 6c61 6773 3d42 6962 6c65 466c  f, flags=BibleFl
+00009c20: 6167 2e41 4c4c 290a 2020 2020 2020 2020  ag.ALL).        
+00009c30: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00009c40: 6865 725f 7265 662c 2042 6962 6c65 5261  her_ref, BibleRa
+00009c50: 6e67 6529 3a0a 2020 2020 2020 2020 2020  nge):.          
+00009c60: 2020 7265 7475 726e 2028 6f74 6865 725f    return (other_
+00009c70: 7265 662e 7374 6172 7420 3e3d 2073 656c  ref.start >= sel
+00009c80: 662e 7374 6172 7420 616e 6420 6f74 6865  f.start and othe
+00009c90: 725f 7265 662e 7374 6172 7420 3c3d 2073  r_ref.start <= s
+00009ca0: 656c 662e 656e 6429 2061 6e64 205c 0a20  elf.end) and \. 
+00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cc0: 2020 286f 7468 6572 5f72 6566 2e65 6e64    (other_ref.end
+00009cd0: 203e 3d20 7365 6c66 2e73 7461 7274 2061   >= self.start a
+00009ce0: 6e64 206f 7468 6572 5f72 6566 2e65 6e64  nd other_ref.end
+00009cf0: 203c 3d20 7365 6c66 2e65 6e64 290a 2020   <= self.end).  
+00009d00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009d10: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00009d20: 6c75 6545 7272 6f72 2866 227b 6f74 6865  lueError(f"{othe
+00009d30: 725f 7265 667d 2069 7320 6e6f 7420 6120  r_ref} is not a 
+00009d40: 7661 6c69 6420 4269 626c 6552 6566 2229  valid BibleRef")
+00009d50: 0a0a 2020 2020 6465 6620 7375 7272 6f75  ..    def surrou
+00009d60: 6e64 7328 7365 6c66 2c20 6f74 6865 725f  nds(self, other_
+00009d70: 7265 663a 2027 4269 626c 6552 6566 2729  ref: 'BibleRef')
+00009d80: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00009d90: 2020 2727 2752 6574 7572 6e73 2060 5472    '''Returns `Tr
+00009da0: 7565 6020 6966 2061 6c6c 2074 6865 2076  ue` if all the v
+00009db0: 6572 7365 7320 696e 2060 6f74 6865 725f  erses in `other_
+00009dc0: 7265 6660 2066 616c 6c20 7769 7468 696e  ref` fall within
+00009dd0: 2074 6869 7320 6042 6962 6c65 5261 6e67   this `BibleRang
+00009de0: 6560 2c20 2a77 6974 686f 7574 2a0a 2020  e`, *without*.  
+00009df0: 2020 2020 2020 696e 636c 7564 696e 6720        including 
+00009e00: 7468 6973 2072 616e 6765 2773 2060 7374  this range's `st
+00009e10: 6172 7460 206f 7220 6065 6e64 6020 6042  art` or `end` `B
+00009e20: 6962 6c65 5665 7273 6560 2e20 4f74 6865  ibleVerse`. Othe
+00009e30: 7277 6973 652c 2072 6574 7572 6e73 2060  rwise, returns `
+00009e40: 4661 6c73 6560 2e0a 2020 2020 2020 2020  False`..        
+00009e50: 2727 270a 2020 2020 2020 2020 6966 2069  '''.        if i
+00009e60: 7369 6e73 7461 6e63 6528 6f74 6865 725f  sinstance(other_
+00009e70: 7265 662c 2042 6962 6c65 5261 6e67 654c  ref, BibleRangeL
+00009e80: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+00009e90: 2020 2320 4269 626c 6552 616e 6765 4c69    # BibleRangeLi
+00009ea0: 7374 2064 6f65 736e 2774 2064 6566 696e  st doesn't defin
+00009eb0: 6520 7375 7272 6f75 6e64 7328 292c 2073  e surrounds(), s
+00009ec0: 6f20 7765 2068 6176 6520 746f 2069 6d70  o we have to imp
+00009ed0: 6c65 6d65 6e74 2068 6572 650a 2020 2020  lement here.    
+00009ee0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00009ef0: 6c6c 2873 656c 662e 7375 7272 6f75 6e64  ll(self.surround
+00009f00: 7328 6f74 6865 725f 7261 6e67 6529 2066  s(other_range) f
+00009f10: 6f72 206f 7468 6572 5f72 616e 6765 2069  or other_range i
+00009f20: 6e20 6f74 6865 725f 7265 6629 200a 2020  n other_ref) .  
+00009f30: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00009f40: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
+00009f50: 6962 6c65 5665 7273 6529 3a0a 2020 2020  ibleVerse):.    
+00009f60: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+00009f70: 7420 746f 2042 6962 6c65 5261 6e67 6520  t to BibleRange 
+00009f80: 2861 6e64 2077 6520 646f 6e27 7420 656e  (and we don't en
+00009f90: 666f 7263 6520 6578 6973 7469 6e67 2066  force existing f
+00009fa0: 6c61 6773 2066 6f72 2063 6f6e 7665 7273  lags for convers
+00009fb0: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
+00009fc0: 2020 6f74 6865 725f 7265 6620 3d20 4269    other_ref = Bi
+00009fd0: 626c 6552 616e 6765 2873 7461 7274 3d6f  bleRange(start=o
+00009fe0: 7468 6572 5f72 6566 2c20 656e 643d 6f74  ther_ref, end=ot
+00009ff0: 6865 725f 7265 662c 2066 6c61 6773 3d42  her_ref, flags=B
+0000a000: 6962 6c65 466c 6167 2e41 4c4c 290a 2020  ibleFlag.ALL).  
+0000a010: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a020: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
+0000a030: 6962 6c65 5261 6e67 6529 3a0a 2020 2020  ibleRange):.    
+0000a040: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000a050: 6f74 6865 725f 7265 662e 7374 6172 7420  other_ref.start 
+0000a060: 3e20 7365 6c66 2e73 7461 7274 2061 6e64  > self.start and
+0000a070: 206f 7468 6572 5f72 6566 2e73 7461 7274   other_ref.start
+0000a080: 203c 2073 656c 662e 656e 6429 2061 6e64   < self.end) and
+0000a090: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+0000a0a0: 2020 2020 2020 286f 7468 6572 5f72 6566        (other_ref
+0000a0b0: 2e65 6e64 203e 2073 656c 662e 7374 6172  .end > self.star
+0000a0c0: 7420 616e 6420 6f74 6865 725f 7265 662e  t and other_ref.
+0000a0d0: 656e 6420 3c20 7365 6c66 2e65 6e64 290a  end < self.end).
+0000a0e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000a0f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000a100: 5661 6c75 6545 7272 6f72 2866 227b 6f74  ValueError(f"{ot
+0000a110: 6865 725f 7265 667d 2069 7320 6e6f 7420  her_ref} is not 
+0000a120: 6120 7661 6c69 6420 4269 626c 6552 6566  a valid BibleRef
+0000a130: 2229 0a0a 2020 2020 6465 6620 756e 696f  ")..    def unio
+0000a140: 6e28 7365 6c66 2c20 6f74 6865 725f 7265  n(self, other_re
+0000a150: 663a 2027 4269 626c 6552 6566 272c 2066  f: 'BibleRef', f
+0000a160: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+0000a170: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
+0000a180: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
+0000a190: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
+0000a1a0: 6120 6e65 7720 6042 6962 6c65 5261 6e67  a new `BibleRang
+0000a1b0: 654c 6973 7460 206f 6620 7665 7273 6573  eList` of verses
+0000a1c0: 2074 6861 7420 6172 6520 6569 7468 6572   that are either
+0000a1d0: 2069 6e20 7468 6973 2072 616e 6765 206f   in this range o
+0000a1e0: 7220 606f 7468 6572 5f72 6566 602e 0a20  r `other_ref`.. 
+0000a1f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a200: 4966 2074 6869 7320 7261 6e67 6520 616e  If this range an
+0000a210: 6420 606f 7468 6572 5f72 6566 6020 6f76  d `other_ref` ov
+0000a220: 6572 6c61 7020 6f72 2061 7265 2061 646a  erlap or are adj
+0000a230: 6163 656e 742c 2074 6865 2072 6573 756c  acent, the resul
+0000a240: 7469 6e67 2060 4269 626c 6552 616e 6765  ting `BibleRange
+0000a250: 4c69 7374 6020 636f 6e74 6169 6e73 206f  List` contains o
+0000a260: 6e65 2065 6c65 6d65 6e74 3a0a 2020 2020  ne element:.    
+0000a270: 2020 2020 6120 7369 6e67 6c65 2060 4269      a single `Bi
+0000a280: 626c 6552 616e 6765 6020 656e 636f 6d70  bleRange` encomp
+0000a290: 6173 7369 6e67 2074 6865 6d20 626f 7468  assing them both
+0000a2a0: 2e20 4f74 6865 7277 6973 652c 2074 6865  . Otherwise, the
+0000a2b0: 206c 6973 7420 636f 6e74 6169 6e73 2074   list contains t
+0000a2c0: 776f 2065 6c65 6d65 6e74 733a 0a20 2020  wo elements:.   
+0000a2d0: 2020 2020 2074 6869 7320 6042 6962 6c65       this `Bible
+0000a2e0: 5261 6e67 6560 2061 6e64 2060 6f74 6865  Range` and `othe
+0000a2f0: 725f 7265 6660 2028 636f 6e76 6572 7465  r_ref` (converte
+0000a300: 6420 746f 2061 2060 4269 626c 6552 616e  d to a `BibleRan
+0000a310: 6765 6020 6966 206e 6563 6573 7361 7279  ge` if necessary
+0000a320: 292e 0a0a 2020 2020 2020 2020 5573 696e  )...        Usin
+0000a330: 6720 7468 6520 607c 6020 6f70 6572 6174  g the `|` operat
+0000a340: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
+0000a350: 2074 6f20 6361 6c6c 696e 6720 6075 6e69   to calling `uni
+0000a360: 6f6e 2829 6020 7769 7468 2060 666c 6167  on()` with `flag
+0000a370: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
+0000a380: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+0000a390: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+0000a3a0: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
+0000a3b0: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
+0000a3c0: 2020 2020 2023 2055 7365 2074 6865 2042       # Use the B
+0000a3d0: 6962 6c65 5261 6e67 654c 6973 7420 696d  ibleRangeList im
+0000a3e0: 706c 656d 656e 7461 7469 6f6e 0a20 2020  plementation.   
+0000a3f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a400: 6f74 6865 725f 7265 662e 756e 696f 6e28  other_ref.union(
+0000a410: 7365 6c66 2c20 666c 6167 733d 666c 6167  self, flags=flag
+0000a420: 7329 0a20 2020 2020 2020 2069 6620 6973  s).        if is
+0000a430: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+0000a440: 6566 2c20 4269 626c 6556 6572 7365 293a  ef, BibleVerse):
+0000a450: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000a460: 6f6e 7665 7274 2074 6f20 4269 626c 6552  onvert to BibleR
+0000a470: 616e 6765 2028 616e 6420 7765 2064 6f6e  ange (and we don
+0000a480: 2774 2065 6e66 6f72 6365 2065 7869 7374  't enforce exist
+0000a490: 696e 6720 666c 6167 7320 666f 7220 636f  ing flags for co
+0000a4a0: 6e76 6572 7369 6f6e 7329 0a20 2020 2020  nversions).     
+0000a4b0: 2020 2020 2020 206f 7468 6572 5f72 6566         other_ref
+0000a4c0: 203d 2042 6962 6c65 5261 6e67 6528 7374   = BibleRange(st
+0000a4d0: 6172 743d 6f74 6865 725f 7265 662c 2065  art=other_ref, e
+0000a4e0: 6e64 3d6f 7468 6572 5f72 6566 2c20 666c  nd=other_ref, fl
+0000a4f0: 6167 733d 4269 626c 6546 6c61 672e 414c  ags=BibleFlag.AL
+0000a500: 4c29 0a20 2020 2020 2020 2069 6620 6973  L).        if is
+0000a510: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+0000a520: 6566 2c20 4269 626c 6552 616e 6765 293a  ef, BibleRange):
+0000a530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a540: 7365 6c66 2e69 735f 6469 736a 6f69 6e74  self.is_disjoint
+0000a550: 286f 7468 6572 5f72 6566 2920 616e 6420  (other_ref) and 
+0000a560: 6e6f 7420 7365 6c66 2e69 735f 6164 6a61  not self.is_adja
+0000a570: 6365 6e74 286f 7468 6572 5f72 6566 2c20  cent(other_ref, 
+0000a580: 666c 6167 733d 666c 6167 7329 3a0a 2020  flags=flags):.  
+0000a590: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000a5a0: 7765 722c 2068 6967 6865 7220 3d20 2873  wer, higher = (s
+0000a5b0: 656c 662c 206f 7468 6572 5f72 6566 2920  elf, other_ref) 
+0000a5c0: 6966 2073 656c 6620 3c20 6f74 6865 725f  if self < other_
+0000a5d0: 7265 6620 656c 7365 2028 6f74 6865 725f  ref else (other_
+0000a5e0: 7265 662c 2073 656c 6629 200a 2020 2020  ref, self) .    
+0000a5f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a600: 726e 2042 6962 6c65 5261 6e67 654c 6973  rn BibleRangeLis
+0000a610: 7428 5b6c 6f77 6572 2c20 6869 6768 6572  t([lower, higher
+0000a620: 5d2c 2066 6c61 6773 3d42 6962 6c65 466c  ], flags=BibleFl
+0000a630: 6167 2e41 4c4c 290a 2020 2020 2020 2020  ag.ALL).        
+0000a640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a650: 2020 2020 2020 2020 2020 7374 6172 7420            start 
+0000a660: 3d20 6d69 6e28 7365 6c66 2e73 7461 7274  = min(self.start
+0000a670: 2c20 6f74 6865 725f 7265 662e 7374 6172  , other_ref.star
+0000a680: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0000a690: 2020 2065 6e64 203d 206d 6178 2873 656c     end = max(sel
+0000a6a0: 662e 656e 642c 206f 7468 6572 5f72 6566  f.end, other_ref
+0000a6b0: 2e65 6e64 290a 2020 2020 2020 2020 2020  .end).          
+0000a6c0: 2020 2020 2020 7265 7475 726e 2042 6962        return Bib
+0000a6d0: 6c65 5261 6e67 654c 6973 7428 5b42 6962  leRangeList([Bib
+0000a6e0: 6c65 5261 6e67 6528 7374 6172 743d 7374  leRange(start=st
+0000a6f0: 6172 742c 2065 6e64 3d65 6e64 2c20 666c  art, end=end, fl
+0000a700: 6167 733d 666c 6167 7329 5d2c 2066 6c61  ags=flags)], fla
+0000a710: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
+0000a720: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000a730: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000a740: 6520 5661 6c75 6545 7272 6f72 2866 227b  e ValueError(f"{
+0000a750: 6f74 6865 725f 7265 667d 2069 7320 6e6f  other_ref} is no
+0000a760: 7420 6120 7661 6c69 6420 4269 626c 6552  t a valid BibleR
+0000a770: 6566 2229 0a0a 2020 2020 6465 6620 696e  ef")..    def in
+0000a780: 7465 7273 6563 7469 6f6e 2873 656c 662c  tersection(self,
+0000a790: 206f 7468 6572 5f72 6566 3a20 2742 6962   other_ref: 'Bib
+0000a7a0: 6c65 5265 6627 2c20 666c 6167 733a 2042  leRef', flags: B
+0000a7b0: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
+0000a7c0: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
+0000a7d0: 6973 7427 3a0a 2020 2020 2020 2020 2727  ist':.        ''
+0000a7e0: 2752 6574 7572 6e73 2061 206e 6577 2060  'Returns a new `
+0000a7f0: 4269 626c 6552 616e 6765 4c69 7374 6020  BibleRangeList` 
+0000a800: 6f66 2076 6572 7365 7320 7468 6174 2061  of verses that a
+0000a810: 7265 2063 6f6d 6d6f 6e20 746f 2062 6f74  re common to bot
+0000a820: 6820 7468 6973 2072 616e 6765 2061 6e64  h this range and
+0000a830: 2060 6f74 6865 725f 7265 6660 2e0a 2020   `other_ref`..  
+0000a840: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
+0000a850: 6620 7468 6572 6520 6172 6520 7665 7273  f there are vers
+0000a860: 6573 2069 6e20 636f 6d6d 6f6e 2c20 7468  es in common, th
+0000a870: 6520 6c69 7374 2063 6f6e 7461 696e 7320  e list contains 
+0000a880: 6120 7369 6e67 6c65 2060 4269 626c 6552  a single `BibleR
+0000a890: 616e 6765 6020 656c 656d 656e 742e 0a20  ange` element.. 
+0000a8a0: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
+0000a8b0: 6172 6520 6e6f 2076 6572 7365 7320 696e  are no verses in
+0000a8c0: 2063 6f6d 6d6f 6e2c 2074 6865 206c 6973   common, the lis
+0000a8d0: 7420 6973 2065 6d70 7479 2e0a 0a20 2020  t is empty...   
+0000a8e0: 2020 2020 2055 7369 6e67 2074 6865 2060       Using the `
+0000a8f0: 2660 206f 7065 7261 746f 7220 6973 2065  &` operator is e
+0000a900: 7175 6976 616c 656e 7420 746f 2063 616c  quivalent to cal
+0000a910: 6c69 6e67 2060 696e 7465 7273 6563 7469  ling `intersecti
+0000a920: 6f6e 2829 6020 7769 7468 2060 666c 6167  on()` with `flag
+0000a930: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
+0000a940: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+0000a950: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+0000a960: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
+0000a970: 6765 4c69 7374 293a 0a20 2020 2020 2020  geList):.       
+0000a980: 2020 2020 2023 2055 7365 2074 6865 2042       # Use the B
+0000a990: 6962 6c65 5261 6e67 654c 6973 7420 696d  ibleRangeList im
+0000a9a0: 706c 656d 656e 7461 7469 6f6e 0a20 2020  plementation.   
+0000a9b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a9c0: 6f74 6865 725f 7265 662e 696e 7465 7273  other_ref.inters
+0000a9d0: 6563 7469 6f6e 2873 656c 662c 2066 6c61  ection(self, fla
+0000a9e0: 6773 3d66 6c61 6773 290a 2020 2020 2020  gs=flags).      
+0000a9f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000aa00: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
+0000aa10: 5665 7273 6529 3a0a 2020 2020 2020 2020  Verse):.        
+0000aa20: 2020 2020 2320 436f 6e76 6572 7420 746f      # Convert to
+0000aa30: 2042 6962 6c65 5261 6e67 6520 2861 6e64   BibleRange (and
+0000aa40: 2077 6520 646f 6e27 7420 656e 666f 7263   we don't enforc
+0000aa50: 6520 6578 6973 7469 6e67 2066 6c61 6773  e existing flags
+0000aa60: 2066 6f72 2063 6f6e 7665 7273 696f 6e73   for conversions
+0000aa70: 290a 2020 2020 2020 2020 2020 2020 6f74  ).            ot
+0000aa80: 6865 725f 7265 6620 3d20 4269 626c 6552  her_ref = BibleR
+0000aa90: 616e 6765 2873 7461 7274 3d6f 7468 6572  ange(start=other
+0000aaa0: 5f72 6566 2c20 656e 643d 6f74 6865 725f  _ref, end=other_
+0000aab0: 7265 662c 2066 6c61 6773 3d42 6962 6c65  ref, flags=Bible
+0000aac0: 466c 6167 2e41 4c4c 290a 2020 2020 2020  Flag.ALL).      
+0000aad0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000aae0: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
+0000aaf0: 5261 6e67 6529 3a0a 2020 2020 2020 2020  Range):.        
+0000ab00: 2020 2020 6966 2073 656c 662e 6973 5f64      if self.is_d
+0000ab10: 6973 6a6f 696e 7428 6f74 6865 725f 7265  isjoint(other_re
+0000ab20: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0000ab30: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+0000ab40: 5261 6e67 654c 6973 7428 290a 2020 2020  RangeList().    
+0000ab50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000ab70: 6172 7420 3d20 6d61 7828 7365 6c66 2e73  art = max(self.s
+0000ab80: 7461 7274 2c20 6f74 6865 725f 7265 662e  tart, other_ref.
+0000ab90: 7374 6172 7429 0a20 2020 2020 2020 2020  start).         
+0000aba0: 2020 2020 2020 2065 6e64 203d 206d 696e         end = min
+0000abb0: 2873 656c 662e 656e 642c 206f 7468 6572  (self.end, other
+0000abc0: 5f72 6566 2e65 6e64 290a 2020 2020 2020  _ref.end).      
+0000abd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000abe0: 2042 6962 6c65 5261 6e67 654c 6973 7428   BibleRangeList(
+0000abf0: 5b42 6962 6c65 5261 6e67 6528 7374 6172  [BibleRange(star
+0000ac00: 743d 7374 6172 742c 2065 6e64 3d65 6e64  t=start, end=end
+0000ac10: 2c20 666c 6167 733d 666c 6167 7329 5d2c  , flags=flags)],
+0000ac20: 2066 6c61 6773 3d42 6962 6c65 466c 6167   flags=BibleFlag
+0000ac30: 2e41 4c4c 290a 2020 2020 2020 2020 656c  .ALL).        el
+0000ac40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000ac50: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000ac60: 2866 227b 6f74 6865 725f 7265 667d 2069  (f"{other_ref} i
+0000ac70: 7320 6e6f 7420 6120 7661 6c69 6420 4269  s not a valid Bi
+0000ac80: 626c 6552 6566 2229 0a0a 2020 2020 6465  bleRef")..    de
+0000ac90: 6620 6469 6666 6572 656e 6365 2873 656c  f difference(sel
+0000aca0: 662c 206f 7468 6572 5f72 6566 3a20 556e  f, other_ref: Un
+0000acb0: 696f 6e5b 4269 626c 6556 6572 7365 2c20  ion[BibleVerse, 
+0000acc0: 2742 6962 6c65 5261 6e67 6527 5d2c 0a20  'BibleRange'],. 
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2020 666c 6167 733a 2042 6962 6c65 466c    flags: BibleFl
+0000acf0: 6167 203d 204e 6f6e 6529 202d 3e20 2742  ag = None) -> 'B
+0000ad00: 6962 6c65 5261 6e67 654c 6973 7427 3a0a  ibleRangeList':.
+0000ad10: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
+0000ad20: 6e73 2061 206e 6577 2060 4269 626c 6552  ns a new `BibleR
+0000ad30: 616e 6765 4c69 7374 6020 6f66 2076 6572  angeList` of ver
+0000ad40: 7365 7320 7468 6174 2061 7265 2069 6e20  ses that are in 
+0000ad50: 7468 6973 2072 616e 6765 2c20 6275 7420  this range, but 
+0000ad60: 6e6f 7420 696e 2060 6f74 6865 725f 7265  not in `other_re
+0000ad70: 6660 2e0a 0a20 2020 2020 2020 2049 6620  f`...        If 
+0000ad80: 7468 6973 2072 616e 6765 2061 6e64 2060  this range and `
+0000ad90: 6f74 6865 725f 7265 6660 2061 7265 2064  other_ref` are d
+0000ada0: 6973 6a6f 696e 742c 2074 6865 206c 6973  isjoint, the lis
+0000adb0: 7420 636f 6e74 6169 6e73 206f 6e65 2065  t contains one e
+0000adc0: 6c65 6d65 6e74 3a20 6120 636f 7079 206f  lement: a copy o
+0000add0: 6620 7468 6973 2060 4269 626c 6552 616e  f this `BibleRan
+0000ade0: 6765 602e 0a20 2020 2020 2020 2049 6620  ge`..        If 
+0000adf0: 7468 6973 2072 616e 6765 2073 7572 726f  this range surro
+0000ae00: 756e 6473 2060 6f74 6865 725f 7265 6660  unds `other_ref`
+0000ae10: 2c20 7468 6520 6c69 7374 2063 6f6e 7461  , the list conta
+0000ae20: 696e 7320 7477 6f20 656c 656d 656e 7473  ins two elements
+0000ae30: 3a0a 2020 2020 2020 2020 2020 2020 6120  :.            a 
+0000ae40: 6c6f 7765 722d 7365 6374 696f 6e20 6042  lower-section `B
+0000ae50: 6962 6c65 5261 6e67 6560 2c20 616e 6420  ibleRange`, and 
+0000ae60: 616e 2075 7070 6572 2d73 6563 7469 6f6e  an upper-section
+0000ae70: 2060 4269 626c 6552 616e 6765 602e 0a20   `BibleRange`.. 
+0000ae80: 2020 2020 2020 2049 6620 606f 7468 6572         If `other
+0000ae90: 5f72 6566 6020 636f 6e74 6169 6e73 2074  _ref` contains t
+0000aea0: 6869 7320 7261 6e67 652c 2074 6865 206c  his range, the l
+0000aeb0: 6973 7420 6973 2065 6d70 7479 2e0a 0a20  ist is empty... 
+0000aec0: 2020 2020 2020 2055 7369 6e67 2074 6865         Using the
+0000aed0: 2060 2d60 206f 7065 7261 746f 7220 6973   `-` operator is
+0000aee0: 2065 7175 6976 616c 656e 7420 746f 2063   equivalent to c
+0000aef0: 616c 6c69 6e67 2060 6469 6666 6572 656e  alling `differen
+0000af00: 6365 2829 6020 7769 7468 2060 666c 6167  ce()` with `flag
+0000af10: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
+0000af20: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+0000af30: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+0000af40: 6572 5f72 6566 2c20 4269 626c 6556 6572  er_ref, BibleVer
+0000af50: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+0000af60: 2023 2043 6f6e 7665 7274 2074 6f20 4269   # Convert to Bi
+0000af70: 626c 6552 616e 6765 2028 616e 6420 7765  bleRange (and we
+0000af80: 2064 6f6e 2774 2065 6e66 6f72 6365 2065   don't enforce e
+0000af90: 7869 7374 696e 6720 666c 6167 7320 666f  xisting flags fo
+0000afa0: 7220 636f 6e76 6572 7369 6f6e 7329 0a20  r conversions). 
+0000afb0: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000afc0: 5f72 6566 203d 2042 6962 6c65 5261 6e67  _ref = BibleRang
+0000afd0: 6528 7374 6172 743d 6f74 6865 725f 7265  e(start=other_re
+0000afe0: 662c 2065 6e64 3d6f 7468 6572 5f72 6566  f, end=other_ref
+0000aff0: 2c20 666c 6167 733d 4269 626c 6546 6c61  , flags=BibleFla
+0000b000: 672e 414c 4c29 0a20 2020 2020 2020 2069  g.ALL).        i
+0000b010: 6620 7365 6c66 2e69 735f 6469 736a 6f69  f self.is_disjoi
+0000b020: 6e74 286f 7468 6572 5f72 6566 293a 0a20  nt(other_ref):. 
+0000b030: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b040: 6e20 4269 626c 6552 616e 6765 4c69 7374  n BibleRangeList
+0000b050: 285b 7365 6c66 5d2c 2066 6c61 6773 3d42  ([self], flags=B
+0000b060: 6962 6c65 466c 6167 2e41 4c4c 290a 2020  ibleFlag.ALL).  
+0000b070: 2020 2020 2020 6966 206f 7468 6572 5f72        if other_r
+0000b080: 6566 2e63 6f6e 7461 696e 7328 7365 6c66  ef.contains(self
+0000b090: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000b0a0: 6574 7572 6e20 4269 626c 6552 616e 6765  eturn BibleRange
+0000b0b0: 4c69 7374 2829 0a0a 2020 2020 2020 2020  List()..        
+0000b0c0: 6c6f 7765 725f 7261 6e67 6520 3d20 4269  lower_range = Bi
+0000b0d0: 626c 6552 616e 6765 2873 7461 7274 3d73  bleRange(start=s
+0000b0e0: 656c 662e 7374 6172 742c 2065 6e64 3d6f  elf.start, end=o
+0000b0f0: 7468 6572 5f72 6566 2e73 7461 7274 2e73  ther_ref.start.s
+0000b100: 7562 5f6e 756d 5f76 6572 7365 7328 312c  ub_num_verses(1,
+0000b110: 2066 6c61 6773 3d66 6c61 6773 2929 0a20   flags=flags)). 
+0000b120: 2020 2020 2020 2075 7070 6572 5f72 616e         upper_ran
+0000b130: 6765 203d 2042 6962 6c65 5261 6e67 6528  ge = BibleRange(
+0000b140: 7374 6172 743d 6f74 6865 725f 7265 662e  start=other_ref.
+0000b150: 656e 642e 6164 645f 6e75 6d5f 7665 7273  end.add_num_vers
+0000b160: 6573 2831 2c20 666c 6167 733d 666c 6167  es(1, flags=flag
+0000b170: 7329 2c20 656e 643d 7365 6c66 2e65 6e64  s), end=self.end
+0000b180: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000b190: 662e 7375 7272 6f75 6e64 7328 6f74 6865  f.surrounds(othe
+0000b1a0: 725f 7265 6629 3a0a 2020 2020 2020 2020  r_ref):.        
+0000b1b0: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+0000b1c0: 5261 6e67 654c 6973 7428 5b6c 6f77 6572  RangeList([lower
+0000b1d0: 5f72 616e 6765 2c20 7570 7065 725f 7261  _range, upper_ra
+0000b1e0: 6e67 655d 2c20 666c 6167 733d 4269 626c  nge], flags=Bibl
+0000b1f0: 6546 6c61 672e 414c 4c29 0a20 2020 2020  eFlag.ALL).     
+0000b200: 2020 2069 6620 7365 6c66 203c 206f 7468     if self < oth
+0000b210: 6572 5f72 6566 3a0a 2020 2020 2020 2020  er_ref:.        
+0000b220: 2020 2020 7265 7475 726e 2042 6962 6c65      return Bible
+0000b230: 5261 6e67 654c 6973 7428 5b6c 6f77 6572  RangeList([lower
+0000b240: 5f72 616e 6765 5d2c 2066 6c61 6773 3d42  _range], flags=B
+0000b250: 6962 6c65 466c 6167 2e41 4c4c 290a 2020  ibleFlag.ALL).  
+0000b260: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000b270: 2020 2020 2020 2020 7265 7475 726e 2042          return B
+0000b280: 6962 6c65 5261 6e67 654c 6973 7428 5b75  ibleRangeList([u
+0000b290: 7070 6572 5f72 616e 6765 5d2c 2066 6c61  pper_range], fla
+0000b2a0: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
+0000b2b0: 290a 0a20 2020 2064 6566 2073 796d 5f64  )..    def sym_d
+0000b2c0: 6966 6665 7265 6e63 6528 7365 6c66 2c20  ifference(self, 
+0000b2d0: 6f74 6865 725f 7265 663a 2055 6e69 6f6e  other_ref: Union
+0000b2e0: 5b42 6962 6c65 5665 7273 652c 2027 4269  [BibleVerse, 'Bi
+0000b2f0: 626c 6552 616e 6765 275d 2c0a 2020 2020  bleRange'],.    
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b310: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+0000b320: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
+0000b330: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
+0000b340: 2020 2020 2027 2727 5265 7475 726e 7320       '''Returns 
+0000b350: 6120 6e65 7720 6042 6962 6c65 5261 6e67  a new `BibleRang
+0000b360: 654c 6973 7460 206f 6620 7665 7273 6573  eList` of verses
+0000b370: 2074 6861 7420 6172 6520 6569 7468 6572   that are either
+0000b380: 2069 6e20 7468 6973 2072 616e 6765 2c20   in this range, 
+0000b390: 6f72 2069 6e20 606f 7468 6572 5f72 6566  or in `other_ref
+0000b3a0: 602c 0a20 2020 2020 2020 2062 7574 206e  `,.        but n
+0000b3b0: 6f74 2062 6f74 682e 0a0a 2020 2020 2020  ot both...      
+0000b3c0: 2020 4465 7065 6e64 696e 6720 6f6e 2074    Depending on t
+0000b3d0: 6869 7320 7261 6e67 6520 616e 6420 606f  his range and `o
+0000b3e0: 7468 6572 5f72 6566 602c 2074 6865 2060  ther_ref`, the `
+0000b3f0: 4269 626c 6552 616e 6765 4c69 7374 6020  BibleRangeList` 
+0000b400: 636f 6e74 6169 6e73 2065 6974 6865 7220  contains either 
+0000b410: 6f6e 6520 6f72 2074 776f 0a20 2020 2020  one or two.     
+0000b420: 2020 2060 4269 626c 6552 616e 6765 6020     `BibleRange` 
+0000b430: 656c 656d 656e 7473 2e20 4966 2074 6869  elements. If thi
+0000b440: 7320 7261 6e67 6520 616e 6420 606f 7468  s range and `oth
+0000b450: 6572 5f72 6566 6020 6172 6520 6578 6163  er_ref` are exac
+0000b460: 746c 7920 6571 7561 6c2c 2074 6869 7320  tly equal, this 
+0000b470: 6c69 7374 2069 7320 656d 7074 792e 0a0a  list is empty...
+0000b480: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
+0000b490: 6520 605e 6020 6f70 6572 6174 6f72 2069  e `^` operator i
+0000b4a0: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
+0000b4b0: 6361 6c6c 696e 6720 6073 796d 5f64 6966  calling `sym_dif
+0000b4c0: 6665 7265 6e63 6528 2960 2077 6974 6820  ference()` with 
+0000b4d0: 6066 6c61 6773 203d 204e 6f6e 6560 2e0a  `flags = None`..
+0000b4e0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000b4f0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000b500: 6528 6f74 6865 725f 7265 662c 2042 6962  e(other_ref, Bib
+0000b510: 6c65 5665 7273 6529 3a0a 2020 2020 2020  leVerse):.      
+0000b520: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+0000b530: 746f 2042 6962 6c65 5261 6e67 6520 2861  to BibleRange (a
+0000b540: 6e64 2077 6520 646f 6e27 7420 656e 666f  nd we don't enfo
+0000b550: 7263 6520 6578 6973 7469 6e67 2066 6c61  rce existing fla
+0000b560: 6773 2066 6f72 2063 6f6e 7665 7273 696f  gs for conversio
+0000b570: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
+0000b580: 6f74 6865 725f 7265 6620 3d20 4269 626c  other_ref = Bibl
+0000b590: 6552 616e 6765 2873 7461 7274 3d6f 7468  eRange(start=oth
+0000b5a0: 6572 5f72 6566 2c20 656e 643d 6f74 6865  er_ref, end=othe
+0000b5b0: 725f 7265 662c 2066 6c61 6773 3d42 6962  r_ref, flags=Bib
+0000b5c0: 6c65 466c 6167 2e41 4c4c 290a 2020 2020  leFlag.ALL).    
+0000b5d0: 2020 2020 6966 2073 656c 6620 3d3d 206f      if self == o
+0000b5e0: 7468 6572 5f72 6566 3a0a 2020 2020 2020  ther_ref:.      
+0000b5f0: 2020 2020 2020 7265 7475 726e 2042 6962        return Bib
+0000b600: 6c65 5261 6e67 654c 6973 7428 290a 2020  leRangeList().  
+0000b610: 2020 2020 2020 756e 696f 6e20 3d20 7365        union = se
+0000b620: 6c66 2e75 6e69 6f6e 286f 7468 6572 5f72  lf.union(other_r
+0000b630: 6566 2c20 666c 6167 733d 666c 6167 7329  ef, flags=flags)
+0000b640: 0a20 2020 2020 2020 2069 6e74 6572 7365  .        interse
+0000b650: 6374 696f 6e20 3d20 7365 6c66 2e69 6e74  ction = self.int
+0000b660: 6572 7365 6374 696f 6e28 6f74 6865 725f  ersection(other_
+0000b670: 7265 662c 2066 6c61 6773 3d66 6c61 6773  ref, flags=flags
+0000b680: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+0000b690: 2875 6e69 6f6e 2920 3e20 3120 6f72 206c  (union) > 1 or l
+0000b6a0: 656e 2869 6e74 6572 7365 6374 696f 6e29  en(intersection)
+0000b6b0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0000b6c0: 2020 2023 2053 656c 6620 616e 6420 6f74     # Self and ot
+0000b6d0: 6865 725f 7265 6620 6172 6520 6469 736a  her_ref are disj
+0000b6e0: 6f69 6e74 2061 6e64 2f6f 7220 6164 6a61  oint and/or adja
+0000b6f0: 6365 6e74 2c20 736f 2074 6865 2075 6e69  cent, so the uni
+0000b700: 6f6e 2069 7320 7468 6520 7361 6d65 0a20  on is the same. 
+0000b710: 2020 2020 2020 2020 2020 2023 2061 7320             # as 
+0000b720: 7468 6520 7379 6d6d 6574 7269 6320 6469  the symmetric di
+0000b730: 6666 6572 656e 6365 0a20 2020 2020 2020  fference.       
+0000b740: 2020 2020 2072 6574 7572 6e20 756e 696f       return unio
+0000b750: 6e0a 2020 2020 2020 2020 656c 7365 3a20  n.        else: 
+0000b760: 2320 5365 6c66 2061 6e64 206f 7468 6572  # Self and other
+0000b770: 5f72 6566 206f 7665 726c 6170 0a20 2020  _ref overlap.   
+0000b780: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000b790: 756e 696f 6e5b 305d 2e64 6966 6665 7265  union[0].differe
+0000b7a0: 6e63 6528 696e 7465 7273 6563 7469 6f6e  nce(intersection
+0000b7b0: 5b30 5d29 0a0a 2020 2020 6465 6620 5f5f  [0])..    def __
+0000b7c0: 6974 6572 5f5f 2873 656c 6629 3a0a 2020  iter__(self):.  
+0000b7d0: 2020 2020 2020 7665 7273 6520 3d20 7365        verse = se
+0000b7e0: 6c66 2e73 7461 7274 0a20 2020 2020 2020  lf.start.       
+0000b7f0: 2077 6869 6c65 2076 6572 7365 203c 3d20   while verse <= 
+0000b800: 7365 6c66 2e65 6e64 3a0a 2020 2020 2020  self.end:.      
+0000b810: 2020 2020 2020 7969 656c 6420 7665 7273        yield vers
+0000b820: 650a 2020 2020 2020 2020 2020 2020 7665  e.            ve
+0000b830: 7273 6520 3d20 7665 7273 652e 6164 645f  rse = verse.add_
+0000b840: 6e75 6d5f 7665 7273 6573 2831 2c20 4269  num_verses(1, Bi
+0000b850: 626c 6546 6c61 672e 4d55 4c54 4942 4f4f  bleFlag.MULTIBOO
+0000b860: 4b29 0a0a 2020 2020 6465 6620 5f5f 636f  K)..    def __co
+0000b870: 6e74 6169 6e73 5f5f 2873 656c 662c 2062  ntains__(self, b
+0000b880: 6962 6c65 5f72 6566 2920 2d3e 2062 6f6f  ible_ref) -> boo
+0000b890: 6c3a 0a20 2020 2020 2020 2027 2727 5265  l:.        '''Re
+0000b8a0: 7475 726e 7320 5472 7565 2069 6620 6974  turns True if it
+0000b8b0: 656d 2069 7320 6120 4269 626c 6552 6566  em is a BibleRef
+0000b8c0: 2074 6861 7420 6661 6c6c 7320 7769 7468   that falls with
+0000b8d0: 696e 2074 6869 7320 7261 6e67 652c 206f  in this range, o
+0000b8e0: 7468 6572 7769 7365 2046 616c 7365 2e0a  therwise False..
+0000b8f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000b900: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000b910: 636f 6e74 6169 6e73 2862 6962 6c65 5f72  contains(bible_r
+0000b920: 6566 290a 2020 2020 0a20 2020 2064 6566  ef).    .    def
+0000b930: 205f 5f6f 725f 5f28 7365 6c66 2c20 6f74   __or__(self, ot
+0000b940: 6865 725f 7265 663a 2027 4269 626c 6552  her_ref: 'BibleR
+0000b950: 6566 2729 202d 3e20 2742 6962 6c65 5261  ef') -> 'BibleRa
+0000b960: 6e67 654c 6973 7427 3a0a 2020 2020 2020  ngeList':.      
+0000b970: 2020 7265 7475 726e 2073 656c 662e 756e    return self.un
+0000b980: 696f 6e28 6f74 6865 725f 7265 6629 0a0a  ion(other_ref)..
+0000b990: 2020 2020 6465 6620 5f5f 616e 645f 5f28      def __and__(
+0000b9a0: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
+0000b9b0: 2027 4269 626c 6552 6566 2729 202d 3e20   'BibleRef') -> 
+0000b9c0: 2742 6962 6c65 5261 6e67 654c 6973 7427  'BibleRangeList'
+0000b9d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000b9e0: 2073 656c 662e 696e 7465 7273 6563 7469   self.intersecti
+0000b9f0: 6f6e 286f 7468 6572 5f72 6566 290a 0a20  on(other_ref).. 
+0000ba00: 2020 2064 6566 205f 5f73 7562 5f5f 2873     def __sub__(s
+0000ba10: 656c 662c 206f 7468 6572 5f72 6566 3a20  elf, other_ref: 
+0000ba20: 2742 6962 6c65 5265 6627 2920 2d3e 2027  'BibleRef') -> '
+0000ba30: 4269 626c 6552 616e 6765 4c69 7374 273a  BibleRangeList':
+0000ba40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ba50: 7365 6c66 2e64 6966 6665 7265 6e63 6528  self.difference(
+0000ba60: 6f74 6865 725f 7265 6629 0a0a 2020 2020  other_ref)..    
+0000ba70: 6465 6620 5f5f 786f 725f 5f28 7365 6c66  def __xor__(self
+0000ba80: 2c20 6f74 6865 725f 7265 663a 2027 4269  , other_ref: 'Bi
+0000ba90: 626c 6552 6566 2729 202d 3e20 2742 6962  bleRef') -> 'Bib
+0000baa0: 6c65 5261 6e67 654c 6973 7427 3a0a 2020  leRangeList':.  
+0000bab0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000bac0: 662e 7379 6d5f 6469 6666 6572 656e 6365  f.sym_difference
+0000bad0: 286f 7468 6572 5f72 6566 290a 0a20 2020  (other_ref)..   
+0000bae0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+0000baf0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0000bb00: 7572 6e20 6622 4269 626c 6552 616e 6765  urn f"BibleRange
+0000bb10: 287b 7365 6c66 2e73 7472 2829 7d29 220a  ({self.str()})".
+0000bb20: 2020 2020 0a20 2020 2064 6566 205f 5f73      .    def __s
+0000bb30: 7472 5f5f 2873 656c 6629 3a0a 2020 2020  tr__(self):.    
+0000bb40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000bb50: 7374 7228 290a 0a20 2020 2064 6566 2073  str()..    def s
+0000bb60: 7472 2873 656c 662c 2061 6262 7265 763d  tr(self, abbrev=
+0000bb70: 4661 6c73 652c 2061 6c74 5f73 6570 3d46  False, alt_sep=F
+0000bb80: 616c 7365 2c20 6e6f 7370 6163 653d 4661  alse, nospace=Fa
+0000bb90: 6c73 652c 2066 6c61 6773 3a20 4269 626c  lse, flags: Bibl
+0000bba0: 6546 6c61 6720 3d20 4e6f 6e65 293a 0a20  eFlag = None):. 
+0000bbb0: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
+0000bbc0: 7320 6120 636f 6e66 6967 7572 6162 6c65  s a configurable
+0000bbd0: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+0000bbe0: 7461 7469 6f6e 206f 6620 7468 6973 2060  tation of this `
+0000bbf0: 4269 626c 6552 616e 6765 602c 2061 7320  BibleRange`, as 
+0000bc00: 666f 6c6c 6f77 733a 0a0a 2020 2020 2020  follows:..      
+0000bc10: 2020 2d20 4966 2060 6162 6272 6576 6020    - If `abbrev` 
+0000bc20: 6973 2060 5472 7565 602c 2074 6865 2061  is `True`, the a
+0000bc30: 6262 7265 7669 6174 6564 206e 616d 6520  bbreviated name 
+0000bc40: 6f66 2074 6865 2062 6f6f 6b20 6973 2075  of the book is u
+0000bc50: 7365 6420 2869 6e73 7465 6164 206f 6620  sed (instead of 
+0000bc60: 7468 6520 6675 6c6c 206e 616d 6529 2e0a  the full name)..
+0000bc70: 2020 2020 2020 2020 2d20 4966 2060 616c          - If `al
+0000bc80: 745f 7365 7060 2069 7320 6054 7275 6560  t_sep` is `True`
+0000bc90: 2c20 6368 6170 7465 7220 616e 6420 7665  , chapter and ve
+0000bca0: 7273 6520 6e75 6d62 6572 7320 6172 6520  rse numbers are 
+0000bcb0: 7365 7061 7261 7465 6420 6279 2074 6865  separated by the
+0000bcc0: 2061 6c74 6572 6e61 7465 0a20 2020 2020   alternate.     
+0000bcd0: 2020 2020 2073 6570 6172 6174 6f72 2028       separator (
+0000bce0: 6465 6661 756c 7473 2074 6f20 602e 6029  defaults to `.`)
+0000bcf0: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
+0000bd00: 7374 616e 6461 7264 2073 6570 6172 6174  standard separat
+0000bd10: 6f72 2028 6465 6661 756c 7473 2074 6f20  or (defaults to 
+0000bd20: 603a 6029 2e0a 2020 2020 2020 2020 2d20  `:`)..        - 
+0000bd30: 4966 2060 6e6f 7370 6163 6560 2069 7320  If `nospace` is 
+0000bd40: 6054 7275 6560 2c20 6e6f 2073 7061 6365  `True`, no space
+0000bd50: 7320 6172 6520 696e 636c 7564 6564 2069  s are included i
+0000bd60: 6e20 7468 6520 7374 7269 6e67 2e0a 2020  n the string..  
+0000bd70: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0000bd80: 2020 6966 2073 656c 662e 7370 616e 735f    if self.spans_
+0000bd90: 7374 6172 745f 626f 6f6b 2829 3a0a 2020  start_book():.  
+0000bda0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000bdb0: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
+0000bdc0: 7365 5061 7274 2e42 4f4f 4b0a 2020 2020  sePart.BOOK.    
+0000bdd0: 2020 2020 2020 2020 6174 5f76 6572 7365          at_verse
+0000bde0: 5f6c 6576 656c 203d 2046 616c 7365 0a20  _level = False. 
+0000bdf0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0000be00: 2e73 7061 6e73 5f73 7461 7274 5f63 6861  .spans_start_cha
+0000be10: 7028 293a 0a20 2020 2020 2020 2020 2020  p():.           
+0000be20: 2073 7461 7274 5f70 6172 7473 203d 2042   start_parts = B
+0000be30: 6962 6c65 5665 7273 6550 6172 742e 424f  ibleVersePart.BO
+0000be40: 4f4b 5f43 4841 500a 2020 2020 2020 2020  OK_CHAP.        
+0000be50: 2020 2020 6174 5f76 6572 7365 5f6c 6576      at_verse_lev
+0000be60: 656c 203d 2046 616c 7365 0a20 2020 2020  el = False.     
+0000be70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000be80: 2020 2020 2073 7461 7274 5f70 6172 7473       start_parts
+0000be90: 203d 2042 6962 6c65 5665 7273 6550 6172   = BibleVersePar
+0000bea0: 742e 4655 4c4c 5f52 4546 0a20 2020 2020  t.FULL_REF.     
+0000beb0: 2020 2020 2020 2061 745f 7665 7273 655f         at_verse_
+0000bec0: 6c65 7665 6c20 3d20 5472 7565 0a20 2020  level = True.   
+0000bed0: 2020 2020 2073 7461 7274 5f73 7472 203d       start_str =
+0000bee0: 2073 656c 662e 7374 6172 742e 7374 7228   self.start.str(
+0000bef0: 6162 6272 6576 2c20 616c 745f 7365 702c  abbrev, alt_sep,
+0000bf00: 206e 6f73 7061 6365 2c20 7374 6172 745f   nospace, start_
+0000bf10: 7061 7274 7329 200a 2020 2020 2020 2020  parts) .        
+0000bf20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000bf30: 2e69 735f 7768 6f6c 655f 626f 6f6b 2866  .is_whole_book(f
+0000bf40: 6c61 6773 2920 6f72 2073 656c 662e 6973  lags) or self.is
+0000bf50: 5f77 686f 6c65 5f63 6861 7028 666c 6167  _whole_chap(flag
+0000bf60: 7329 206f 7220 7365 6c66 2e69 735f 7369  s) or self.is_si
+0000bf70: 6e67 6c65 5f76 6572 7365 2829 3a20 2320  ngle_verse(): # 
+0000bf80: 5369 6e67 6c65 2072 6566 6572 656e 6365  Single reference
+0000bf90: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+0000bfa0: 5f73 7472 203d 2022 220a 2020 2020 2020  _str = "".      
+0000bfb0: 2020 2020 2020 7261 6e67 655f 7365 7020        range_sep 
+0000bfc0: 3d20 2222 0a20 2020 2020 2020 2065 6c73  = "".        els
+0000bfd0: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
+0000bfe0: 7261 6e67 655f 7365 7020 3d20 6269 626c  range_sep = bibl
+0000bff0: 655f 6461 7461 2829 2e72 616e 6765 5f73  e_data().range_s
+0000c000: 6570 0a20 2020 2020 2020 2020 2020 2069  ep.            i
+0000c010: 6620 7365 6c66 2e65 6e64 2e62 6f6f 6b20  f self.end.book 
+0000c020: 213d 2073 656c 662e 7374 6172 742e 626f  != self.start.bo
+0000c030: 6f6b 3a0a 2020 2020 2020 2020 2020 2020  ok:.            
+0000c040: 2020 2020 6174 5f76 6572 7365 5f6c 6576      at_verse_lev
+0000c050: 656c 203d 2046 616c 7365 0a20 2020 2020  el = False.     
+0000c060: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000c070: 2020 2020 6966 2073 656c 662e 7370 616e      if self.span
+0000c080: 735f 656e 645f 626f 6f6b 2866 6c61 6773  s_end_book(flags
+0000c090: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c0a0: 2020 2065 6e64 5f70 6172 7473 203d 2042     end_parts = B
+0000c0b0: 6962 6c65 5665 7273 6550 6172 742e 424f  ibleVersePart.BO
+0000c0c0: 4f4b 0a20 2020 2020 2020 2020 2020 2065  OK.            e
+0000c0d0: 6c69 6620 6e6f 7420 6174 5f76 6572 7365  lif not at_verse
+0000c0e0: 5f6c 6576 656c 2061 6e64 2073 656c 662e  _level and self.
+0000c0f0: 7370 616e 735f 656e 645f 6368 6170 2866  spans_end_chap(f
+0000c100: 6c61 6773 293a 0a20 2020 2020 2020 2020  lags):.         
+0000c110: 2020 2020 2020 2065 6e64 5f70 6172 7473         end_parts
+0000c120: 203d 2042 6962 6c65 5665 7273 6550 6172   = BibleVersePar
+0000c130: 742e 424f 4f4b 5f43 4841 500a 2020 2020  t.BOOK_CHAP.    
+0000c140: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000c150: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000c160: 645f 7061 7274 7320 3d20 4269 626c 6556  d_parts = BibleV
+0000c170: 6572 7365 5061 7274 2e46 554c 4c5f 5245  ersePart.FULL_RE
+0000c180: 460a 2020 2020 2020 2020 2020 2020 0a20  F.            . 
+0000c190: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c1a0: 6c66 2e73 7461 7274 2e62 6f6f 6b20 3d3d  lf.start.book ==
+0000c1b0: 2073 656c 662e 656e 642e 626f 6f6b 3a0a   self.end.book:.
+0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1d0: 656e 645f 7061 7274 7320 263d 207e 4269  end_parts &= ~Bi
+0000c1e0: 626c 6556 6572 7365 5061 7274 2e42 4f4f  bleVersePart.BOO
+0000c1f0: 4b20 2320 4f6d 6974 2062 6f6f 6b0a 2020  K # Omit book.  
+0000c200: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c210: 2073 656c 662e 7374 6172 742e 6368 6170   self.start.chap
+0000c220: 5f6e 756d 203d 3d20 7365 6c66 2e65 6e64  _num == self.end
+0000c230: 2e63 6861 705f 6e75 6d3a 0a20 2020 2020  .chap_num:.     
+0000c240: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000c250: 6e64 5f70 6172 7473 2026 3d20 7e42 6962  nd_parts &= ~Bib
+0000c260: 6c65 5665 7273 6550 6172 742e 4348 4150  leVersePart.CHAP
+0000c270: 2023 204f 6d69 7420 6368 6170 7465 720a   # Omit chapter.
+0000c280: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000c290: 2020 2020 2020 2020 2065 6e64 5f73 7472           end_str
+0000c2a0: 203d 2073 656c 662e 656e 642e 7374 7228   = self.end.str(
+0000c2b0: 6162 6272 6576 2c20 616c 745f 7365 702c  abbrev, alt_sep,
+0000c2c0: 206e 6f73 7061 6365 2c20 656e 645f 7061   nospace, end_pa
+0000c2d0: 7274 7329 200a 2020 2020 2020 2020 0a20  rts) .        . 
+0000c2e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000c2f0: 6622 7b73 7461 7274 5f73 7472 7d7b 7261  f"{start_str}{ra
+0000c300: 6e67 655f 7365 707d 7b65 6e64 5f73 7472  nge_sep}{end_str
+0000c310: 7d22 0a20 2020 2020 2020 2069 6620 6e6f  }".        if no
+0000c320: 7370 6163 653a 0a20 2020 2020 2020 2020  space:.         
+0000c330: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000c340: 2e72 6570 6c61 6365 2822 2022 2c20 2222  .replace(" ", ""
+0000c350: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000c360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c370: 726e 2072 6573 756c 742e 7374 7269 7028  rn result.strip(
+0000c380: 290a 0a0a 636c 6173 7320 4269 626c 6552  )...class BibleR
+0000c390: 616e 6765 4c69 7374 2875 7469 6c2e 4772  angeList(util.Gr
+0000c3a0: 6f75 7065 644c 6973 7429 3a0a 2020 2020  oupedList):.    
+0000c3b0: 2727 2741 206c 6973 7420 6f66 2060 4269  '''A list of `Bi
+0000c3c0: 626c 6552 616e 6765 6020 656c 656d 656e  bleRange` elemen
+0000c3d0: 7473 2c20 616c 6c6f 7769 6e67 2066 6f72  ts, allowing for
+0000c3e0: 2067 726f 7570 696e 6720 616e 6420 7365   grouping and se
+0000c3f0: 742d 7374 796c 6520 6f70 6572 6174 696f  t-style operatio
+0000c400: 6e73 2e0a 0a20 2020 2043 7572 7265 6e74  ns...    Current
+0000c410: 6c79 2074 6865 2067 726f 7570 696e 6720  ly the grouping 
+0000c420: 6675 6e63 7469 6f6e 616c 6974 7920 6973  functionality is
+0000c430: 2070 726f 7669 6465 6420 7669 6120 6120   provided via a 
+0000c440: 7375 7065 7263 6c61 7373 2028 6062 6962  superclass (`bib
+0000c450: 6c65 7265 662e 7574 696c 2e47 726f 7570  leref.util.Group
+0000c460: 6564 4c69 7374 602c 2061 2064 6f75 626c  edList`, a doubl
+0000c470: 792d 6c69 6e6b 6564 0a20 2020 206c 6973  y-linked.    lis
+0000c480: 7429 2c20 7468 6f75 6768 2074 6869 7320  t), though this 
+0000c490: 7368 6f75 6c64 2062 6520 636f 6e73 6964  should be consid
+0000c4a0: 6572 6564 2061 6e20 696d 706c 656d 656e  ered an implemen
+0000c4b0: 7461 7469 6f6e 2064 6574 6169 6c2e 0a20  tation detail.. 
+0000c4c0: 2020 2027 2727 0a20 2020 2064 6566 205f     '''.    def _
+0000c4d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
+0000c4e0: 7267 732c 2066 6c61 6773 3a20 4269 626c  rgs, flags: Bibl
+0000c4f0: 6546 6c61 6720 3d20 4e6f 6e65 293a 0a20  eFlag = None):. 
+0000c500: 2020 2020 2020 2027 2727 4120 4269 626c         '''A Bibl
+0000c510: 6552 616e 6765 2063 616e 2062 6520 636f  eRange can be co
+0000c520: 6e73 7472 7563 7465 6420 696e 2061 6e79  nstructed in any
+0000c530: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+0000c540: 6720 7761 7973 3a0a 0a20 2020 2020 2020  g ways:..       
+0000c550: 2031 2e20 4672 6f6d 2061 2073 696e 676c   1. From a singl
+0000c560: 6520 7374 7269 6e67 3a20 6042 6962 6c65  e string: `Bible
+0000c570: 5261 6e67 654c 6973 7428 224d 6172 6b20  RangeList("Mark 
+0000c580: 333a 312d 343a 323b 2035 3a36 2d38 2c20  3:1-4:2; 5:6-8, 
+0000c590: 3130 3b20 4d61 7474 2034 2229 600a 0a20  10; Matt 4")`.. 
+0000c5a0: 2020 2020 2020 2020 2020 5261 6973 6573            Raises
+0000c5b0: 2061 2060 4269 626c 6552 6566 5061 7273   a `BibleRefPars
+0000c5c0: 696e 6745 7272 6f72 6020 6966 2074 6865  ingError` if the
+0000c5d0: 2073 7472 696e 6720 6361 6e6e 6f74 2062   string cannot b
+0000c5e0: 6520 7061 7273 6564 2e0a 0a20 2020 2020  e parsed...     
+0000c5f0: 2020 2020 2020 5768 656e 2070 6172 7369        When parsi
+0000c600: 6e67 2061 2073 7472 696e 672c 2065 6163  ng a string, eac
+0000c610: 6820 6d61 6a6f 7220 6772 6f75 702d 7365  h major group-se
+0000c620: 7061 7261 746f 7220 2860 3b60 2062 7920  parator (`;` by 
+0000c630: 6465 6661 756c 7429 2070 6c61 6365 7320  default) places 
+0000c640: 7375 6273 6571 7565 6e74 0a20 2020 2020  subsequent.     
+0000c650: 2020 2020 2020 4269 626c 6520 7261 6e67        Bible rang
+0000c660: 6573 2069 6e74 6f20 6120 6e65 7720 6772  es into a new gr
+0000c670: 6f75 702e 2045 6163 6820 6d69 6e6f 7220  oup. Each minor 
+0000c680: 6772 6f75 702d 7365 7061 7261 746f 7220  group-separator 
+0000c690: 2860 2c60 2062 7920 6465 6661 756c 7429  (`,` by default)
+0000c6a0: 2070 6c61 6365 7320 7375 6273 6571 7565   places subseque
+0000c6b0: 6e74 0a20 2020 2020 2020 2020 2020 7061  nt.           pa
+0000c6c0: 7373 6167 6573 2069 6e74 6f20 7468 6520  ssages into the 
+0000c6d0: 7361 6d65 2067 726f 7570 2e0a 0a20 2020  same group...   
+0000c6e0: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+0000c6f0: 6f6e 0a20 2020 2020 2020 2020 2020 203e  on.            >
+0000c700: 3e3e 2066 726f 6d20 6269 626c 6572 6566  >> from bibleref
+0000c710: 2069 6d70 6f72 7420 2a0a 2020 2020 2020   import *.      
+0000c720: 2020 2020 2020 3e3e 3e20 7261 6e67 655f        >>> range_
+0000c730: 6c69 7374 203d 2042 6962 6c65 5261 6e67  list = BibleRang
+0000c740: 654c 6973 7428 224d 6172 6b20 333a 312d  eList("Mark 3:1-
+0000c750: 343a 323b 2035 3a36 2d38 2c20 3130 3b20  4:2; 5:6-8, 10; 
+0000c760: 4d61 7474 2034 2229 0a20 2020 2020 2020  Matt 4").       
+0000c770: 2020 2020 203e 3e3e 206c 656e 2872 616e       >>> len(ran
+0000c780: 6765 5f6c 6973 742e 6772 6f75 7073 290a  ge_list.groups).
+0000c790: 2020 2020 2020 2020 2020 2020 330a 2020              3.  
+0000c7a0: 2020 2020 2020 2020 2020 3e3e 3e20 7261            >>> ra
+0000c7b0: 6e67 655f 6c69 7374 2e67 726f 7570 735b  nge_list.groups[
+0000c7c0: 305d 0a20 2020 2020 2020 2020 2020 2047  0].            G
+0000c7d0: 726f 7570 5669 6577 285b 4269 626c 6552  roupView([BibleR
+0000c7e0: 616e 6765 284d 6172 6b20 332d 343a 3229  ange(Mark 3-4:2)
+0000c7f0: 5d29 0a20 2020 2020 2020 2020 2020 203e  ]).            >
+0000c800: 3e3e 2072 616e 6765 5f6c 6973 742e 6772  >> range_list.gr
+0000c810: 6f75 7073 5b31 5d0a 2020 2020 2020 2020  oups[1].        
+0000c820: 2020 2020 4772 6f75 7056 6965 7728 5b42      GroupView([B
+0000c830: 6962 6c65 5261 6e67 6528 4d61 726b 2035  ibleRange(Mark 5
+0000c840: 3a36 2d35 3a38 292c 2042 6962 6c65 5261  :6-5:8), BibleRa
+0000c850: 6e67 6528 4d61 726b 2035 3a31 3029 5d29  nge(Mark 5:10)])
+0000c860: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+0000c870: 2072 616e 6765 5f6c 6973 742e 6772 6f75   range_list.grou
+0000c880: 7073 5b32 5d0a 2020 2020 2020 2020 2020  ps[2].          
+0000c890: 2020 4772 6f75 7056 6965 7728 5b42 6962    GroupView([Bib
+0000c8a0: 6c65 5261 6e67 6528 4d61 7474 6865 7720  leRange(Matthew 
+0000c8b0: 3429 5d29 0a20 2020 2020 2020 2020 2020  4)]).           
+0000c8c0: 203e 3e3e 2072 616e 6765 5f6c 6973 742e   >>> range_list.
+0000c8d0: 6772 6f75 7073 5b31 5d5b 305d 0a20 2020  groups[1][0].   
+0000c8e0: 2020 2020 2020 2020 2042 6962 6c65 5261           BibleRa
+0000c8f0: 6e67 6528 4d61 726b 2035 3a36 2d35 3a38  nge(Mark 5:6-5:8
+0000c900: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+0000c910: 3e20 7261 6e67 655f 6c69 7374 2e67 726f  > range_list.gro
+0000c920: 7570 735b 315d 5b31 5d0a 2020 2020 2020  ups[1][1].      
+0000c930: 2020 2020 2020 4269 626c 6552 616e 6765        BibleRange
+0000c940: 284d 6172 6b20 353a 3130 290a 2020 2020  (Mark 5:10).    
+0000c950: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+0000c960: 2020 2020 322e 2046 726f 6d20 616e 7920      2. From any 
+0000c970: 6974 6572 6162 6c65 2063 6f6e 7461 696e  iterable contain
+0000c980: 696e 6720 4269 626c 6552 616e 6765 733a  ing BibleRanges:
+0000c990: 0a20 2020 2020 2020 2020 2020 6042 6962  .           `Bib
+0000c9a0: 6c65 5261 6e67 654c 6973 7428 5b42 6962  leRangeList([Bib
+0000c9b0: 6c65 5261 6e67 6528 224d 6172 6b20 333a  leRange("Mark 3:
+0000c9c0: 312d 343a 3222 292c 2042 6962 6c65 5261  1-4:2"), BibleRa
+0000c9d0: 6e67 6528 224d 6172 6b20 353a 362d 3822  nge("Mark 5:6-8"
+0000c9e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2042                 B
+0000ca00: 6962 6c65 5261 6e67 6528 224d 6172 6b20  ibleRange("Mark 
+0000ca10: 353a 3130 2229 2c20 4269 626c 6552 616e  5:10"), BibleRan
+0000ca20: 6765 2822 4d61 7474 2034 2229 5d29 600a  ge("Matt 4")])`.
+0000ca30: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000ca40: 2020 2020 2033 2e20 4173 2061 2063 6f70       3. As a cop
+0000ca50: 7920 6f66 2061 6e20 6578 6973 7469 6e67  y of an existing
+0000ca60: 2042 6962 6c65 5261 6e67 654c 6973 743a   BibleRangeList:
+0000ca70: 2060 4269 626c 6552 616e 6765 4c69 7374   `BibleRangeList
+0000ca80: 2865 7869 7374 696e 675f 6269 626c 655f  (existing_bible_
+0000ca90: 7261 6e67 655f 6c69 7374 2960 0a20 2020  range_list)`.   
+0000caa0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0000cab0: 2066 6c61 6773 203d 2066 6c61 6773 206f   flags = flags o
+0000cac0: 7220 676c 6f62 616c 7328 295b 2766 6c61  r globals()['fla
+0000cad0: 6773 275d 0a0a 2020 2020 2020 2020 6966  gs']..        if
+0000cae0: 206c 656e 2861 7267 7329 203d 3d20 313a   len(args) == 1:
+0000caf0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cb00: 6973 696e 7374 616e 6365 2861 7267 735b  isinstance(args[
+0000cb10: 305d 2c20 7374 7229 3a0a 2020 2020 2020  0], str):.      
+0000cb20: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
+0000cb30: 6772 6f75 7073 5f6c 6973 7420 3d20 7061  groups_list = pa
+0000cb40: 7273 6572 2e5f 7061 7273 6528 6172 6773  rser._parse(args
+0000cb50: 5b30 5d2c 2066 6c61 6773 290a 2020 2020  [0], flags).    
+0000cb60: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+0000cb70: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
+0000cb80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000cb90: 6f72 2067 726f 7570 2069 6e20 7261 6e67  or group in rang
+0000cba0: 655f 6772 6f75 7073 5f6c 6973 743a 0a20  e_groups_list:. 
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 2073 656c 662e 6170 7065 6e64 5f67     self.append_g
+0000cbd0: 726f 7570 2867 726f 7570 290a 2020 2020  roup(group).    
+0000cbe0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+0000cbf0: 6e73 7461 6e63 6528 6172 6773 5b30 5d2c  nstance(args[0],
+0000cc00: 2042 6962 6c65 5261 6e67 654c 6973 7429   BibleRangeList)
+0000cc10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cc20: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+0000cc30: 5f5f 2829 0a20 2020 2020 2020 2020 2020  __().           
+0000cc40: 2020 2020 2066 6f72 2067 726f 7570 2069       for group i
+0000cc50: 6e20 6172 6773 5b30 5d2e 6772 6f75 7073  n args[0].groups
+0000cc60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cc70: 2020 2020 2020 7365 6c66 2e61 7070 656e        self.appen
+0000cc80: 645f 6772 6f75 7028 6772 6f75 7029 0a20  d_group(group). 
+0000cc90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000cca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ccb0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+0000ccc0: 5f28 2a61 7267 7329 0a20 2020 2020 2020  _(*args).       
+0000ccd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000cce0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+0000ccf0: 745f 5f28 6172 6773 290a 0a20 2020 2040  t__(args)..    @
+0000cd00: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000cd10: 2067 726f 7570 7328 7365 6c66 2920 2d3e   groups(self) ->
+0000cd20: 2075 7469 6c2e 4772 6f75 7065 644c 6973   util.GroupedLis
+0000cd30: 742e 4772 6f75 7056 6965 7773 3a0a 2020  t.GroupViews:.  
+0000cd40: 2020 2020 2020 2727 2752 6574 7572 6e73        '''Returns
+0000cd50: 2074 6865 2060 6269 626c 6572 6566 2e75   the `bibleref.u
+0000cd60: 7469 6c2e 4772 6f75 7065 644c 6973 742e  til.GroupedList.
+0000cd70: 4772 6f75 7056 6965 7773 6020 636f 6c6c  GroupViews` coll
+0000cd80: 6563 7469 6f6e 2066 6f72 2074 6869 7320  ection for this 
+0000cd90: 6c69 7374 2e27 2727 0a20 2020 2020 2020  list.'''.       
+0000cda0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+0000cdb0: 6772 6f75 7073 2020 2020 0a0a 2020 2020  groups    ..    
+0000cdc0: 6465 6620 5f63 6865 636b 5f74 7970 6528  def _check_type(
+0000cdd0: 7365 6c66 2c20 7661 6c75 6529 3a0a 2020  self, value):.  
+0000cde0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0000cdf0: 6e73 7461 6e63 6528 7661 6c75 652c 2042  nstance(value, B
+0000ce00: 6962 6c65 5261 6e67 6529 3a0a 2020 2020  ibleRange):.    
+0000ce10: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0000ce20: 7065 4572 726f 7228 6622 4974 656d 2069  peError(f"Item i
+0000ce30: 7320 6e6f 7420 6120 4269 626c 6552 616e  s not a BibleRan
+0000ce40: 6765 3a20 7b76 616c 7565 7d22 290a 0a20  ge: {value}").. 
+0000ce50: 2020 2064 6566 2076 6572 7365 5f30 5f74     def verse_0_t
+0000ce60: 6f5f 3128 7365 6c66 293a 0a20 2020 2020  o_1(self):.     
+0000ce70: 2020 2027 2727 4d6f 6469 6669 6573 2074     '''Modifies t
+0000ce80: 6869 7320 6c69 7374 202a 696e 2d70 6c61  his list *in-pla
+0000ce90: 6365 2a20 6279 2063 616c 6c69 6e67 2060  ce* by calling `
+0000cea0: 7665 7273 655f 305f 746f 5f31 2829 6020  verse_0_to_1()` 
+0000ceb0: 6f6e 2065 7665 7279 2060 4269 626c 6552  on every `BibleR
+0000cec0: 616e 6765 6020 696e 2074 6865 206c 6973  ange` in the lis
+0000ced0: 740a 2020 2020 2020 2020 616e 6420 7573  t.        and us
+0000cee0: 696e 6720 7468 6520 7265 7375 6c74 2074  ing the result t
+0000cef0: 6f20 7265 706c 6163 6520 7468 6520 6f72  o replace the or
+0000cf00: 6967 696e 616c 2072 616e 6765 2e20 5265  iginal range. Re
+0000cf10: 7475 726e 7320 604e 6f6e 6560 2e27 2727  turns `None`.'''
+0000cf20: 0a20 2020 2020 2020 2066 6f72 206e 6f64  .        for nod
+0000cf30: 6520 696e 2073 656c 662e 5f6e 6f64 655f  e in self._node_
+0000cf40: 6974 6572 2829 3a0a 2020 2020 2020 2020  iter():.        
+0000cf50: 2020 2020 6e6f 6465 2e76 616c 7565 203d      node.value =
+0000cf60: 206e 6f64 652e 7661 6c75 652e 7665 7273   node.value.vers
+0000cf70: 655f 305f 746f 5f31 2829 0a20 2020 2020  e_0_to_1().     
+0000cf80: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+0000cf90: 2020 2020 6465 6620 7665 7273 655f 315f      def verse_1_
+0000cfa0: 746f 5f30 2873 656c 6629 3a0a 2020 2020  to_0(self):.    
+0000cfb0: 2020 2020 2727 274d 6f64 6966 6965 7320      '''Modifies 
+0000cfc0: 7468 6973 206c 6973 7420 2a69 6e2d 706c  this list *in-pl
+0000cfd0: 6163 652a 2062 7920 6361 6c6c 696e 6720  ace* by calling 
+0000cfe0: 6076 6572 7365 5f31 5f74 6f5f 3028 2960  `verse_1_to_0()`
+0000cff0: 206f 6e20 6576 6572 7920 6042 6962 6c65   on every `Bible
+0000d000: 5261 6e67 6560 2069 6e20 7468 6520 6c69  Range` in the li
+0000d010: 7374 0a20 2020 2020 2020 2061 6e64 2075  st.        and u
+0000d020: 7369 6e67 2074 6865 2072 6573 756c 7420  sing the result 
+0000d030: 746f 2072 6570 6c61 6365 2074 6865 206f  to replace the o
+0000d040: 7269 6769 6e61 6c20 7261 6e67 652e 2052  riginal range. R
+0000d050: 6574 7572 6e73 2060 4e6f 6e65 602e 0a20  eturns `None`.. 
+0000d060: 2020 2020 2020 202a 2a4e 6f74 652a 2a3a         **Note**:
+0000d070: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
+0000d080: 6520 676c 6f62 616c 2061 7474 7269 6275  e global attribu
+0000d090: 7465 2060 6269 626c 6572 6566 2e72 6566  te `bibleref.ref
+0000d0a0: 2e66 6c61 6773 6020 6973 202a 6967 6e6f  .flags` is *igno
+0000d0b0: 7265 642a 2e27 2727 0a20 2020 2020 2020  red*.'''.       
+0000d0c0: 2066 6f72 206e 6f64 6520 696e 2073 656c   for node in sel
+0000d0d0: 662e 5f6e 6f64 655f 6974 6572 2829 3a0a  f._node_iter():.
+0000d0e0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+0000d0f0: 2e76 616c 7565 203d 206e 6f64 652e 7661  .value = node.va
+0000d100: 6c75 652e 7665 7273 655f 315f 746f 5f30  lue.verse_1_to_0
+0000d110: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0000d120: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+0000d130: 636f 6e73 6f6c 6964 6174 6528 7365 6c66  consolidate(self
+0000d140: 2c20 666c 6167 733a 2042 6962 6c65 466c  , flags: BibleFl
+0000d150: 6167 203d 204e 6f6e 6529 3a0a 2020 2020  ag = None):.    
+0000d160: 2020 2020 2727 2753 6f72 7473 2074 6869      '''Sorts thi
+0000d170: 7320 6c69 7374 2069 6e2d 706c 6163 6520  s list in-place 
+0000d180: 616e 6420 6d65 7267 6573 2072 616e 6765  and merges range
+0000d190: 7320 7768 6572 6576 6572 2070 6f73 7369  s wherever possi
+0000d1a0: 626c 652e 2054 6865 2072 6573 756c 7420  ble. The result 
+0000d1b0: 6973 2074 6865 2073 6d61 6c6c 6573 740a  is the smallest.
+0000d1c0: 2020 2020 2020 2020 6c69 7374 206f 6620          list of 
+0000d1d0: 6469 736a 6f69 6e74 2c20 6e6f 6e2d 6164  disjoint, non-ad
+0000d1e0: 6a61 6365 6e74 2060 4269 626c 6552 616e  jacent `BibleRan
+0000d1f0: 6765 6020 656c 656d 656e 7473 2073 7061  ge` elements spa
+0000d200: 6e6e 696e 6720 7468 6520 7361 6d65 2076  nning the same v
+0000d210: 6572 7365 7320 6173 2069 6e20 7468 6520  erses as in the 
+0000d220: 6f72 6967 696e 616c 0a20 2020 2020 2020  original.       
+0000d230: 206c 6973 742e 0a0a 2020 2020 2020 2020   list...        
+0000d240: 416c 6c20 6772 6f75 7073 2061 7265 2072  All groups are r
+0000d250: 656d 6f76 6564 2061 6e64 2072 6570 6c61  emoved and repla
+0000d260: 6365 6420 7769 7468 2061 2073 696e 676c  ced with a singl
+0000d270: 6520 6772 6f75 702e 0a20 2020 2020 2020  e group..       
+0000d280: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
+0000d290: 662e 736f 7274 2829 0a20 2020 2020 2020  f.sort().       
+0000d2a0: 206e 6f64 6520 3d20 7365 6c66 2e5f 6669   node = self._fi
+0000d2b0: 7273 740a 2020 2020 2020 2020 7768 696c  rst.        whil
+0000d2c0: 6520 6e6f 6465 2069 7320 6e6f 7420 4e6f  e node is not No
+0000d2d0: 6e65 2061 6e64 206e 6f64 652e 6e65 7874  ne and node.next
+0000d2e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000d2f0: 2020 2020 2020 2020 2020 756e 696f 6e20            union 
+0000d300: 3d20 6e6f 6465 2e76 616c 7565 2e75 6e69  = node.value.uni
+0000d310: 6f6e 286e 6f64 652e 6e65 7874 2e76 616c  on(node.next.val
+0000d320: 7565 2c20 666c 6167 733d 666c 6167 7329  ue, flags=flags)
+0000d330: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d340: 6c65 6e28 756e 696f 6e29 203d 3d20 313a  len(union) == 1:
+0000d350: 2023 2043 616e 206d 6572 6765 2074 6865   # Can merge the
+0000d360: 7365 2074 776f 2072 616e 6765 7320 7769  se two ranges wi
+0000d370: 7468 2074 6865 6972 2075 6e69 6f6e 0a20  th their union. 
+0000d380: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000d390: 6f64 652e 7661 6c75 6520 3d20 756e 696f  ode.value = unio
+0000d3a0: 6e5b 305d 0a20 2020 2020 2020 2020 2020  n[0].           
+0000d3b0: 2020 2020 2073 656c 662e 5f70 6f70 5f61       self._pop_a
+0000d3c0: 6674 6572 286e 6f64 6529 0a20 2020 2020  fter(node).     
+0000d3d0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+0000d3e0: 646f 6e27 7420 6d6f 7665 206f 6e20 7965  don't move on ye
+0000d3f0: 742c 2073 6f20 7765 2063 616e 2063 6f6d  t, so we can com
+0000d400: 7061 7265 2074 6865 206e 6577 6c79 206d  pare the newly m
+0000d410: 6572 6765 6420 7261 6e67 650a 2020 2020  erged range.    
+0000d420: 2020 2020 2020 2020 2020 2020 2320 7769              # wi
+0000d430: 7468 2074 6865 2028 6e65 7729 206e 6578  th the (new) nex
+0000d440: 7420 6e6f 6465 0a20 2020 2020 2020 2020  t node.         
+0000d450: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000d460: 2020 2020 2020 2020 2023 2054 6865 2074           # The t
+0000d470: 776f 2072 616e 6765 7320 6361 6e27 7420  wo ranges can't 
+0000d480: 6265 206d 6572 6765 642c 2073 6f20 6d6f  be merged, so mo
+0000d490: 7665 206f 6e0a 2020 2020 2020 2020 2020  ve on.          
+0000d4a0: 2020 2020 2020 6e6f 6465 203d 206e 6f64        node = nod
+0000d4b0: 652e 6e65 7874 0a0a 2020 2020 6465 6620  e.next..    def 
+0000d4c0: 6973 5f64 6973 6a6f 696e 7428 7365 6c66  is_disjoint(self
+0000d4d0: 2c20 6f74 6865 725f 7265 663a 2027 4269  , other_ref: 'Bi
+0000d4e0: 626c 6552 6566 2729 202d 3e20 626f 6f6c  bleRef') -> bool
+0000d4f0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+0000d500: 7572 6e73 2060 5472 7565 6020 6966 2065  urns `True` if e
+0000d510: 7665 7279 2060 4269 626c 6552 616e 6765  very `BibleRange
+0000d520: 6020 6973 2064 6973 6a6f 696e 7420 7769  ` is disjoint wi
+0000d530: 7468 2061 6c6c 2074 6865 2076 6572 7365  th all the verse
+0000d540: 7320 696e 2060 6f74 6865 725f 7265 6660  s in `other_ref`
+0000d550: 2c20 6f74 6865 7277 6973 6520 6046 616c  , otherwise `Fal
+0000d560: 7365 602e 0a20 2020 2020 2020 2027 2727  se`..        '''
+0000d570: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0000d580: 7374 616e 6365 286f 7468 6572 5f72 6566  stance(other_ref
+0000d590: 2c20 4269 626c 6556 6572 7365 293a 0a20  , BibleVerse):. 
+0000d5a0: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
+0000d5b0: 7665 7274 2074 6f20 4269 626c 6552 616e  vert to BibleRan
+0000d5c0: 6765 4c69 7374 2028 616e 6420 7765 2064  geList (and we d
+0000d5d0: 6f6e 2774 2065 6e66 6f72 6365 2065 7869  on't enforce exi
+0000d5e0: 7374 696e 6720 666c 6167 7320 666f 7220  sting flags for 
+0000d5f0: 636f 6e76 6572 7369 6f6e 7329 0a20 2020  conversions).   
+0000d600: 2020 2020 2020 2020 206f 7468 6572 5f72           other_r
+0000d610: 6566 203d 2042 6962 6c65 5261 6e67 654c  ef = BibleRangeL
+0000d620: 6973 7428 5b42 6962 6c65 5261 6e67 6528  ist([BibleRange(
+0000d630: 7374 6172 743d 6f74 6865 725f 7265 662c  start=other_ref,
+0000d640: 2065 6e64 3d6f 7468 6572 5f72 6566 2c20   end=other_ref, 
+0000d650: 666c 6167 733d 4269 626c 6546 6c61 672e  flags=BibleFlag.
+0000d660: 414c 4c29 5d29 0a20 2020 2020 2020 2065  ALL)]).        e
+0000d670: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
+0000d680: 7468 6572 5f72 6566 2c20 4269 626c 6552  ther_ref, BibleR
+0000d690: 616e 6765 293a 0a20 2020 2020 2020 2020  ange):.         
+0000d6a0: 2020 206f 7468 6572 5f72 6566 203d 2042     other_ref = B
+0000d6b0: 6962 6c65 5261 6e67 654c 6973 7428 5b6f  ibleRangeList([o
+0000d6c0: 7468 6572 5f72 6566 5d29 0a20 2020 2020  ther_ref]).     
+0000d6d0: 2020 2072 6574 7572 6e20 616c 6c28 7365     return all(se
+0000d6e0: 6c66 5f72 616e 6765 2e69 735f 6469 736a  lf_range.is_disj
+0000d6f0: 6f69 6e74 286f 7468 6572 5f72 616e 6765  oint(other_range
+0000d700: 2920 666f 7220 7365 6c66 5f72 616e 6765  ) for self_range
+0000d710: 2069 6e20 7365 6c66 2066 6f72 206f 7468   in self for oth
+0000d720: 6572 5f72 616e 6765 2069 6e20 6f74 6865  er_range in othe
+0000d730: 725f 7265 6629 0a0a 2020 2020 6465 6620  r_ref)..    def 
+0000d740: 636f 6e74 6169 6e73 2873 656c 662c 206f  contains(self, o
+0000d750: 7468 6572 5f72 6566 3a20 2742 6962 6c65  ther_ref: 'Bible
+0000d760: 5265 6627 2c20 666c 6167 733a 2042 6962  Ref', flags: Bib
+0000d770: 6c65 466c 6167 203d 204e 6f6e 6529 202d  leFlag = None) -
+0000d780: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000d790: 2727 2752 6574 7572 6e73 2060 5472 7565  '''Returns `True
+0000d7a0: 6020 6966 2061 6c6c 2074 6865 2076 6572  ` if all the ver
+0000d7b0: 7365 7320 696e 2060 6f74 6865 725f 7265  ses in `other_re
+0000d7c0: 6660 2066 616c 6c20 7769 7468 696e 2061  f` fall within a
+0000d7d0: 7420 6c65 6173 7420 6f6e 6520 6f66 2074  t least one of t
+0000d7e0: 6865 2060 4269 626c 6552 616e 6765 6020  he `BibleRange` 
+0000d7f0: 656c 656d 656e 7473 0a20 2020 2020 2020  elements.       
+0000d800: 2069 6e20 7468 6973 206c 6973 742e 204f   in this list. O
+0000d810: 7468 6572 7769 7365 2072 6574 7572 6e73  therwise returns
+0000d820: 2060 4661 6c73 6560 2e0a 0a20 2020 2020   `False`...     
+0000d830: 2020 2054 6865 2073 616d 6520 7265 7375     The same resu
+0000d840: 6c74 2069 7320 7265 7475 726e 6564 2075  lt is returned u
+0000d850: 7369 6e67 2074 6865 2027 696e 2720 6f70  sing the 'in' op
+0000d860: 6572 6174 6f72 2028 692e 652e 2060 6f74  erator (i.e. `ot
+0000d870: 6865 725f 7265 6620 696e 2062 6962 6c65  her_ref in bible
+0000d880: 5f72 616e 6765 5f6c 6973 7460 292e 0a20  _range_list`).. 
+0000d890: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000d8a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000d8b0: 286f 7468 6572 5f72 6566 2c20 4269 626c  (other_ref, Bibl
+0000d8c0: 6556 6572 7365 293a 0a20 2020 2020 2020  eVerse):.       
+0000d8d0: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
+0000d8e0: 6f20 4269 626c 6552 616e 6765 4c69 7374  o BibleRangeList
+0000d8f0: 2028 616e 6420 7765 2064 6f6e 2774 2065   (and we don't e
+0000d900: 6e66 6f72 6365 2065 7869 7374 696e 6720  nforce existing 
+0000d910: 666c 6167 7320 666f 7220 636f 6e76 6572  flags for conver
+0000d920: 7369 6f6e 7329 0a20 2020 2020 2020 2020  sions).         
+0000d930: 2020 206f 7468 6572 5f72 6566 203d 2042     other_ref = B
+0000d940: 6962 6c65 5261 6e67 654c 6973 7428 5b42  ibleRangeList([B
+0000d950: 6962 6c65 5261 6e67 6528 7374 6172 743d  ibleRange(start=
+0000d960: 6f74 6865 725f 7265 662c 2065 6e64 3d6f  other_ref, end=o
+0000d970: 7468 6572 5f72 6566 2c20 666c 6167 733d  ther_ref, flags=
+0000d980: 4269 626c 6546 6c61 672e 414c 4c29 5d29  BibleFlag.ALL)])
+0000d990: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+0000d9a0: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+0000d9b0: 6566 2c20 4269 626c 6552 616e 6765 293a  ef, BibleRange):
+0000d9c0: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
+0000d9d0: 6572 5f72 6566 203d 2042 6962 6c65 5261  er_ref = BibleRa
+0000d9e0: 6e67 654c 6973 7428 5b6f 7468 6572 5f72  ngeList([other_r
+0000d9f0: 6566 5d29 0a20 2020 2020 2020 2023 2043  ef]).        # C
+0000da00: 7265 6174 6520 6120 636f 6e73 6f6c 6964  reate a consolid
+0000da10: 6174 6564 2063 6f70 7920 6f66 206f 7572  ated copy of our
+0000da20: 7365 6c76 6573 0a20 2020 2020 2020 2073  selves.        s
+0000da30: 656c 665f 636f 7079 203d 2042 6962 6c65  elf_copy = Bible
+0000da40: 5261 6e67 654c 6973 7428 7365 6c66 290a  RangeList(self).
+0000da50: 2020 2020 2020 2020 7365 6c66 5f63 6f70          self_cop
+0000da60: 792e 636f 6e73 6f6c 6964 6174 6528 666c  y.consolidate(fl
+0000da70: 6167 733d 666c 6167 7329 0a20 2020 2020  ags=flags).     
+0000da80: 2020 2023 2045 7665 7279 206f 6e65 206f     # Every one o
+0000da90: 6620 7468 6520 6f74 6865 7220 6c69 7374  f the other list
+0000daa0: 2773 2072 616e 6765 7320 6d75 7374 2062  's ranges must b
+0000dab0: 6520 636f 6e74 6169 6e65 6420 6279 2061  e contained by a
+0000dac0: 7420 6c65 6173 7420 6f6e 6520 6f66 2074  t least one of t
+0000dad0: 6865 206f 7572 2072 616e 6765 730a 2020  he our ranges.  
+0000dae0: 2020 2020 2020 7265 7475 726e 2061 6c6c        return all
+0000daf0: 2861 6e79 2873 656c 665f 7261 6e67 652e  (any(self_range.
+0000db00: 636f 6e74 6169 6e73 286f 7468 6572 5f72  contains(other_r
+0000db10: 616e 6765 2920 666f 7220 7365 6c66 5f72  ange) for self_r
+0000db20: 616e 6765 2069 6e20 7365 6c66 5f63 6f70  ange in self_cop
+0000db30: 7929 2066 6f72 206f 7468 6572 5f72 616e  y) for other_ran
+0000db40: 6765 2069 6e20 6f74 6865 725f 7265 6629  ge in other_ref)
+0000db50: 0a0a 2020 2020 6465 6620 756e 696f 6e28  ..    def union(
+0000db60: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
+0000db70: 2027 4269 626c 6552 6566 272c 2066 6c61   'BibleRef', fla
+0000db80: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
+0000db90: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
+0000dba0: 616e 6765 4c69 7374 273a 0a20 2020 2020  angeList':.     
+0000dbb0: 2020 2027 2727 4372 6561 7465 7320 6120     '''Creates a 
+0000dbc0: 6e65 7720 6042 6962 6c65 5261 6e67 654c  new `BibleRangeL
+0000dbd0: 6973 7460 2074 6861 7420 636f 6e74 6169  ist` that contai
+0000dbe0: 6e73 2061 6c6c 2074 6865 2076 6572 7365  ns all the verse
+0000dbf0: 7320 696e 2074 6869 7320 6042 6962 6c65  s in this `Bible
+0000dc00: 5261 6e67 654c 6973 7460 0a20 2020 2020  RangeList`.     
+0000dc10: 2020 2061 6e64 2061 6c6c 2074 6865 2076     and all the v
+0000dc20: 6572 7365 7320 696e 2060 6f74 6865 725f  erses in `other_
+0000dc30: 7265 6660 2c20 7468 656e 2063 6f6e 736f  ref`, then conso
+0000dc40: 6c69 6461 7465 7320 7468 6520 7265 7375  lidates the resu
+0000dc50: 6c74 2061 6e64 2072 6574 7572 6e73 2069  lt and returns i
+0000dc60: 742e 0a0a 2020 2020 2020 2020 5573 696e  t...        Usin
+0000dc70: 6720 7468 6520 607c 6020 6f70 6572 6174  g the `|` operat
+0000dc80: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
+0000dc90: 2074 6f20 6361 6c6c 696e 6720 6075 6e69   to calling `uni
+0000dca0: 6f6e 2829 6020 7769 7468 2060 666c 6167  on()` with `flag
+0000dcb0: 7320 3d20 4e6f 6e65 602e 0a20 2020 2020  s = None`..     
+0000dcc0: 2020 2027 2727 0a20 2020 2020 2020 206e     '''.        n
+0000dcd0: 6577 5f6c 6973 7420 3d20 4269 626c 6552  ew_list = BibleR
+0000dce0: 616e 6765 4c69 7374 2873 656c 6629 0a20  angeList(self). 
+0000dcf0: 2020 2020 2020 206e 6577 5f6c 6973 742e         new_list.
+0000dd00: 756e 696f 6e5f 7570 6461 7465 286f 7468  union_update(oth
+0000dd10: 6572 5f72 6566 2c20 666c 6167 733d 666c  er_ref, flags=fl
+0000dd20: 6167 7329 0a20 2020 2020 2020 2072 6574  ags).        ret
+0000dd30: 7572 6e20 6e65 775f 6c69 7374 0a0a 2020  urn new_list..  
+0000dd40: 2020 6465 6620 756e 696f 6e5f 7570 6461    def union_upda
+0000dd50: 7465 2873 656c 662c 206f 7468 6572 5f72  te(self, other_r
+0000dd60: 6566 3a20 2742 6962 6c65 5265 6627 2c20  ef: 'BibleRef', 
+0000dd70: 666c 6167 733a 2042 6962 6c65 466c 6167  flags: BibleFlag
+0000dd80: 203d 204e 6f6e 6529 202d 3e20 2742 6962   = None) -> 'Bib
+0000dd90: 6c65 5261 6e67 654c 6973 7427 3a0a 2020  leRangeList':.  
+0000dda0: 2020 2020 2020 2727 2755 7064 6174 6573        '''Updates
+0000ddb0: 2074 6869 7320 6c69 7374 2074 6f20 6265   this list to be
+0000ddc0: 2074 6865 2075 6e69 6f6e 206f 6620 6974   the union of it
+0000ddd0: 7320 6578 6973 7469 6e67 2065 6c65 6d65  s existing eleme
+0000dde0: 6e74 7320 616e 6420 606f 7468 6572 5f72  nts and `other_r
+0000ddf0: 6566 602c 2074 6865 6e20 636f 6e73 6f6c  ef`, then consol
+0000de00: 6964 6174 6573 2074 6869 7320 6c69 7374  idates this list
+0000de10: 2e0a 0a20 2020 2020 2020 2055 7369 6e67  ...        Using
+0000de20: 2074 6865 2060 7c3d 6020 6f70 6572 6174   the `|=` operat
+0000de30: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
+0000de40: 2074 6f20 6361 6c6c 696e 6720 6075 6e69   to calling `uni
+0000de50: 6f6e 5f75 7064 6174 6528 2960 2077 6974  on_update()` wit
+0000de60: 6820 6066 6c61 6773 203d 204e 6f6e 6560  h `flags = None`
+0000de70: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+0000de80: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000de90: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
+0000dea0: 6962 6c65 5665 7273 6529 3a0a 2020 2020  ibleVerse):.    
+0000deb0: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+0000dec0: 7420 746f 2042 6962 6c65 5261 6e67 654c  t to BibleRangeL
+0000ded0: 6973 7420 2861 6e64 2077 6520 646f 6e27  ist (and we don'
+0000dee0: 7420 656e 666f 7263 6520 6578 6973 7469  t enforce existi
+0000def0: 6e67 2066 6c61 6773 2066 6f72 2063 6f6e  ng flags for con
+0000df00: 7665 7273 696f 6e73 290a 2020 2020 2020  versions).      
+0000df10: 2020 2020 2020 6f74 6865 725f 7265 6620        other_ref 
+0000df20: 3d20 4269 626c 6552 616e 6765 4c69 7374  = BibleRangeList
+0000df30: 285b 4269 626c 6552 616e 6765 2873 7461  ([BibleRange(sta
+0000df40: 7274 3d6f 7468 6572 5f72 6566 2c20 656e  rt=other_ref, en
+0000df50: 643d 6f74 6865 725f 7265 662c 2066 6c61  d=other_ref, fla
+0000df60: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
+0000df70: 295d 290a 2020 2020 2020 2020 656c 6966  )]).        elif
+0000df80: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+0000df90: 725f 7265 662c 2042 6962 6c65 5261 6e67  r_ref, BibleRang
+0000dfa0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000dfb0: 6f74 6865 725f 7265 6620 3d20 4269 626c  other_ref = Bibl
+0000dfc0: 6552 616e 6765 4c69 7374 285b 6f74 6865  eRangeList([othe
+0000dfd0: 725f 7265 665d 290a 2020 2020 2020 2020  r_ref]).        
+0000dfe0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000dff0: 6528 6f74 6865 725f 7265 662c 2042 6962  e(other_ref, Bib
+0000e000: 6c65 5261 6e67 654c 6973 7429 3a0a 2020  leRangeList):.  
+0000e010: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000e020: 5661 6c75 6545 7272 6f72 2866 227b 6f74  ValueError(f"{ot
+0000e030: 6865 725f 7265 667d 2069 7320 6e6f 7420  her_ref} is not 
+0000e040: 6120 7661 6c69 6420 4269 626c 6552 6566  a valid BibleRef
+0000e050: 2229 2020 2020 2020 2020 0a0a 2020 2020  ")        ..    
+0000e060: 2020 2020 7365 6c66 2e65 7874 656e 6428      self.extend(
+0000e070: 6f74 6865 725f 7265 6629 0a20 2020 2020  other_ref).     
+0000e080: 2020 2073 656c 662e 636f 6e73 6f6c 6964     self.consolid
+0000e090: 6174 6528 666c 6167 733d 666c 6167 7329  ate(flags=flags)
+0000e0a0: 0a0a 2020 2020 6465 6620 696e 7465 7273  ..    def inters
+0000e0b0: 6563 7469 6f6e 2873 656c 662c 206f 7468  ection(self, oth
+0000e0c0: 6572 5f72 6566 3a20 2742 6962 6c65 5265  er_ref: 'BibleRe
+0000e0d0: 6627 2c20 666c 6167 733a 2042 6962 6c65  f', flags: Bible
+0000e0e0: 466c 6167 203d 204e 6f6e 6529 202d 3e20  Flag = None) -> 
+0000e0f0: 2742 6962 6c65 5261 6e67 654c 6973 7427  'BibleRangeList'
+0000e100: 3a0a 2020 2020 2020 2020 2727 2743 7265  :.        '''Cre
+0000e110: 6174 6573 2061 206e 6577 2060 4269 626c  ates a new `Bibl
+0000e120: 6552 616e 6765 4c69 7374 6020 6f66 2076  eRangeList` of v
+0000e130: 6572 7365 7320 7468 6174 2061 7265 2063  erses that are c
+0000e140: 6f6d 6d6f 6e20 746f 2062 6f74 6820 7468  ommon to both th
+0000e150: 6973 2060 4269 626c 6552 616e 6765 4c69  is `BibleRangeLi
+0000e160: 7374 6020 616e 6420 606f 7468 6572 5f72  st` and `other_r
+0000e170: 6566 602c 0a20 2020 2020 2020 2074 6865  ef`,.        the
+0000e180: 6e20 636f 6e73 6f6c 6964 6174 6573 2074  n consolidates t
+0000e190: 6865 2072 6573 756c 7420 616e 6420 7265  he result and re
+0000e1a0: 7475 726e 7320 6974 2e20 4966 2074 6865  turns it. If the
+0000e1b0: 7265 2061 7265 206e 6f20 7665 7273 6573  re are no verses
+0000e1c0: 2069 6e20 636f 6d6d 6f6e 2c20 7468 6520   in common, the 
+0000e1d0: 7265 7475 726e 6564 206c 6973 7420 6973  returned list is
+0000e1e0: 2065 6d70 7479 2e0a 0a20 2020 2020 2020   empty...       
+0000e1f0: 2055 7369 6e67 2074 6865 2060 2660 206f   Using the `&` o
+0000e200: 7065 7261 746f 7220 6973 2065 7175 6976  perator is equiv
+0000e210: 616c 656e 7420 746f 2063 616c 6c69 6e67  alent to calling
+0000e220: 2060 696e 7465 7273 6563 7469 6f6e 2829   `intersection()
+0000e230: 6020 7769 7468 2060 666c 6167 7320 3d20  ` with `flags = 
+0000e240: 4e6f 6e65 602e 0a20 2020 2020 2020 2027  None`..        '
+0000e250: 2727 0a20 2020 2020 2020 2069 6620 6973  ''.        if is
+0000e260: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
+0000e270: 6566 2c20 4269 626c 6556 6572 7365 293a  ef, BibleVerse):
+0000e280: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000e290: 6f6e 7665 7274 2074 6f20 4269 626c 6552  onvert to BibleR
+0000e2a0: 616e 6765 4c69 7374 2028 616e 6420 7765  angeList (and we
+0000e2b0: 2064 6f6e 2774 2065 6e66 6f72 6365 2065   don't enforce e
+0000e2c0: 7869 7374 696e 6720 666c 6167 7320 666f  xisting flags fo
+0000e2d0: 7220 636f 6e76 6572 7369 6f6e 7329 0a20  r conversions). 
+0000e2e0: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000e2f0: 5f72 6566 203d 2042 6962 6c65 5261 6e67  _ref = BibleRang
+0000e300: 654c 6973 7428 5b42 6962 6c65 5261 6e67  eList([BibleRang
+0000e310: 6528 7374 6172 743d 6f74 6865 725f 7265  e(start=other_re
+0000e320: 662c 2065 6e64 3d6f 7468 6572 5f72 6566  f, end=other_ref
+0000e330: 2c20 666c 6167 733d 4269 626c 6546 6c61  , flags=BibleFla
+0000e340: 672e 414c 4c29 5d29 0a20 2020 2020 2020  g.ALL)]).       
+0000e350: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0000e360: 286f 7468 6572 5f72 6566 2c20 4269 626c  (other_ref, Bibl
+0000e370: 6552 616e 6765 293a 0a20 2020 2020 2020  eRange):.       
+0000e380: 2020 2020 206f 7468 6572 5f72 6566 203d       other_ref =
+0000e390: 2042 6962 6c65 5261 6e67 654c 6973 7428   BibleRangeList(
+0000e3a0: 5b6f 7468 6572 5f72 6566 5d29 0a20 2020  [other_ref]).   
+0000e3b0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000e3c0: 7374 616e 6365 286f 7468 6572 5f72 6566  stance(other_ref
+0000e3d0: 2c20 4269 626c 6552 616e 6765 4c69 7374  , BibleRangeList
+0000e3e0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000e3f0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000e400: 6622 7b6f 7468 6572 5f72 6566 7d20 6973  f"{other_ref} is
+0000e410: 206e 6f74 2061 2076 616c 6964 2042 6962   not a valid Bib
+0000e420: 6c65 5265 6622 2920 2020 2020 2020 200a  leRef")        .
+0000e430: 0a20 2020 2020 2020 2023 2045 6163 6820  .        # Each 
+0000e440: 4269 626c 6552 6566 4c69 7374 2069 7320  BibleRefList is 
+0000e450: 6566 6665 6374 6976 656c 7920 6120 756e  effectively a un
+0000e460: 696f 6e20 6f66 2069 7473 2065 6c65 6d65  ion of its eleme
+0000e470: 6e74 732e 0a20 2020 2020 2020 2023 204b  nts..        # K
+0000e480: 6579 2073 6574 2074 6865 6f72 7920 6964  ey set theory id
+0000e490: 656e 7469 7479 3a0a 2020 2020 2020 2020  entity:.        
+0000e4a0: 2320 2020 2841 3020 e288 aa20 4131 2920  #   (A0 ... A1) 
+0000e4b0: e288 a920 2842 3020 e288 aa20 4231 2920  ... (B0 ... B1) 
+0000e4c0: 3d20 2841 3020 e288 a920 4230 2920 e288  = (A0 ... B0) ..
+0000e4d0: aa20 2841 3020 e288 a920 4231 2920 e288  . (A0 ... B1) ..
+0000e4e0: aa20 2841 3120 e288 a920 4230 2920 e288  . (A1 ... B0) ..
+0000e4f0: aa20 2841 3120 e288 a920 4231 290a 2020  . (A1 ... B1).  
+0000e500: 2020 2020 2020 2320 536f 2074 6865 2069        # So the i
+0000e510: 6e74 6572 7365 6374 696f 6e20 6f66 2074  ntersection of t
+0000e520: 776f 2042 6962 6c65 5265 664c 6973 7473  wo BibleRefLists
+0000e530: 2069 7320 6120 6e65 7720 6c69 7374 206f   is a new list o
+0000e540: 6620 7468 6520 696e 7465 7273 6563 7469  f the intersecti
+0000e550: 6f6e 206f 6620 6561 6368 2069 7465 6d0a  on of each item.
+0000e560: 2020 2020 2020 2020 2320 636f 6d62 696e          # combin
+0000e570: 6174 696f 6e2e 0a20 2020 2020 2020 206e  ation..        n
+0000e580: 6577 5f6c 6973 7420 3d20 4269 626c 6552  ew_list = BibleR
+0000e590: 616e 6765 4c69 7374 2829 0a20 2020 2020  angeList().     
+0000e5a0: 2020 2066 6f72 2073 656c 665f 7261 6e67     for self_rang
+0000e5b0: 6520 696e 2073 656c 663a 0a20 2020 2020  e in self:.     
+0000e5c0: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
+0000e5d0: 5f72 616e 6765 2069 6e20 6f74 6865 725f  _range in other_
+0000e5e0: 7265 663a 0a20 2020 2020 2020 2020 2020  ref:.           
+0000e5f0: 2020 2020 2069 7465 6d5f 696e 7465 7273       item_inters
+0000e600: 6563 7469 6f6e 5f6c 6973 7420 3d20 7365  ection_list = se
+0000e610: 6c66 5f72 616e 6765 2e69 6e74 6572 7365  lf_range.interse
+0000e620: 6374 696f 6e28 6f74 6865 725f 7261 6e67  ction(other_rang
+0000e630: 652c 2066 6c61 6773 3d66 6c61 6773 290a  e, flags=flags).
 0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 4269 626c 6552 616e 6765 2822      BibleRange("
-0000e660: 4d61 726b 2035 3a31 3022 292c 2042 6962  Mark 5:10"), Bib
-0000e670: 6c65 5261 6e67 6528 224d 6174 7420 3422  leRange("Matt 4"
-0000e680: 295d 2960 0a20 2020 2020 2020 200a 2020  )])`.        .  
-0000e690: 2020 2020 2020 2020 2049 6620 7468 6520           If the 
-0000e6a0: 6974 6572 6162 6c65 2773 2069 7465 6d73  iterable's items
-0000e6b0: 2061 7265 2050 7974 686f 6e20 6c69 7374   are Python list
-0000e6c0: 7320 6f72 2074 7570 6c65 732c 2065 6163  s or tuples, eac
-0000e6d0: 6820 6974 656d 206f 6620 7468 6520 6974  h item of the it
-0000e6e0: 6572 6162 6c65 2069 7320 6164 6465 6420  erable is added 
-0000e6f0: 6173 2061 0a20 2020 2020 2020 2020 2020  as a.           
-0000e700: 7365 7061 7261 7465 2067 726f 7570 3a0a  separate group:.
-0000e710: 2020 2020 2020 2020 2020 2060 4269 626c             `Bibl
-0000e720: 6552 616e 6765 4c69 7374 285b 5b42 6962  eRangeList([[Bib
-0000e730: 6c65 5261 6e67 6528 224d 6172 6b20 333a  leRange("Mark 3:
-0000e740: 312d 343a 3222 292c 2042 6962 6c65 5261  1-4:2"), BibleRa
-0000e750: 6e67 6528 224d 6172 6b20 353a 362d 3822  nge("Mark 5:6-8"
-0000e760: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 5b42 6962 6c65 5261 6e67 6528 224d 6172  [BibleRange("Mar
-0000e790: 6b20 353a 3130 2229 2c20 4269 626c 6552  k 5:10"), BibleR
-0000e7a0: 616e 6765 2822 4d61 7474 2034 2229 5d5d  ange("Matt 4")]]
-0000e7b0: 2960 0a20 2020 2020 2020 2020 2020 200a  )`.            .
-0000e7c0: 2020 2020 2020 2020 332e 2041 7320 6120          3. As a 
-0000e7d0: 636f 7079 206f 6620 616e 2065 7869 7374  copy of an exist
-0000e7e0: 696e 6720 4269 626c 6552 616e 6765 4c69  ing BibleRangeLi
-0000e7f0: 7374 3a20 6042 6962 6c65 5261 6e67 654c  st: `BibleRangeL
-0000e800: 6973 7428 6578 6973 7469 6e67 5f62 6962  ist(existing_bib
-0000e810: 6c65 5f72 616e 6765 5f6c 6973 7429 600a  le_range_list)`.
-0000e820: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000e830: 2020 2020 666c 6167 7320 3d20 666c 6167      flags = flag
-0000e840: 7320 6f72 2062 6962 6c65 7265 662e 666c  s or bibleref.fl
-0000e850: 6167 7320 6f72 2042 6962 6c65 466c 6167  ags or BibleFlag
-0000e860: 2e4e 4f4e 450a 0a20 2020 2020 2020 2069  .NONE..        i
-0000e870: 6620 6c65 6e28 6172 6773 2920 3d3d 2031  f len(args) == 1
-0000e880: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000e890: 2069 7369 6e73 7461 6e63 6528 6172 6773   isinstance(args
-0000e8a0: 5b30 5d2c 2073 7472 293a 0a20 2020 2020  [0], str):.     
-0000e8b0: 2020 2020 2020 2020 2020 2072 616e 6765             range
-0000e8c0: 5f67 726f 7570 735f 6c69 7374 203d 2070  _groups_list = p
-0000e8d0: 6172 7365 722e 5f70 6172 7365 2861 7267  arser._parse(arg
-0000e8e0: 735b 305d 2c20 666c 6167 7329 0a20 2020  s[0], flags).   
-0000e8f0: 2020 2020 2020 2020 2020 2020 2073 7570               sup
-0000e900: 6572 2829 2e5f 5f69 6e69 745f 5f28 290a  er().__init__().
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e920: 666f 7220 6772 6f75 7020 696e 2072 616e  for group in ran
-0000e930: 6765 5f67 726f 7570 735f 6c69 7374 3a0a  ge_groups_list:.
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
-0000e960: 6772 6f75 7028 6772 6f75 7029 0a20 2020  group(group).   
-0000e970: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-0000e980: 696e 7374 616e 6365 2861 7267 735b 305d  instance(args[0]
-0000e990: 2c20 4269 626c 6552 616e 6765 4c69 7374  , BibleRangeList
-0000e9a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e9b0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000e9c0: 745f 5f28 290a 2020 2020 2020 2020 2020  t__().          
-0000e9d0: 2020 2020 2020 666f 7220 6772 6f75 7020        for group 
-0000e9e0: 696e 2061 7267 735b 305d 2e67 726f 7570  in args[0].group
-0000e9f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000ea00: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
-0000ea10: 6e64 5f67 726f 7570 2867 726f 7570 290a  nd_group(group).
-0000ea20: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000ea30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ea40: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-0000ea50: 5f5f 282a 6172 6773 290a 2020 2020 2020  __(*args).      
-0000ea60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ea70: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0000ea80: 6974 5f5f 2861 7267 7329 0a0a 2020 2020  it__(args)..    
-0000ea90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000eaa0: 6620 6772 6f75 7073 2873 656c 6629 202d  f groups(self) -
-0000eab0: 3e20 7574 696c 2e47 726f 7570 6564 4c69  > util.GroupedLi
-0000eac0: 7374 2e47 726f 7570 5669 6577 733a 0a20  st.GroupViews:. 
-0000ead0: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-0000eae0: 7320 7468 6520 6062 6962 6c65 7265 662e  s the `bibleref.
-0000eaf0: 7574 696c 2e47 726f 7570 6564 4c69 7374  util.GroupedList
-0000eb00: 2e47 726f 7570 5669 6577 7360 2063 6f6c  .GroupViews` col
-0000eb10: 6c65 6374 696f 6e20 666f 7220 7468 6973  lection for this
-0000eb20: 206c 6973 742e 0a20 2020 2020 2020 200a   list..        .
-0000eb30: 2020 2020 2020 2020 4e6f 7465 3a20 4375          Note: Cu
-0000eb40: 7272 656e 746c 792c 2074 6f20 636f 6e76  rrently, to conv
-0000eb50: 6572 7420 616e 2069 6e64 6976 6964 7561  ert an individua
-0000eb60: 6c20 6772 6f75 7020 746f 2061 2070 726f  l group to a pro
-0000eb70: 7065 726c 792d 666f 726d 6174 7465 6420  perly-formatted 
-0000eb80: 4269 626c 6520 7265 6665 7265 6e63 6520  Bible reference 
-0000eb90: 7374 7269 6e67 2079 6f75 206e 6565 6420  string you need 
-0000eba0: 746f 0a20 2020 2020 2020 2063 7265 6174  to.        creat
-0000ebb0: 6520 6120 6e65 7720 4269 626c 6552 616e  e a new BibleRan
-0000ebc0: 6765 4c69 7374 2066 726f 6d20 7468 6520  geList from the 
-0000ebd0: 6772 6f75 702e 2046 6f72 2065 7861 6d70  group. For examp
-0000ebe0: 6c65 3a0a 2020 2020 2020 2020 0a20 2020  le:.        .   
-0000ebf0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-0000ec00: 2020 2020 2020 203e 3e3e 2072 616e 6765         >>> range
-0000ec10: 5f6c 6973 7420 3d20 4269 626c 6552 616e  _list = BibleRan
-0000ec20: 6765 4c69 7374 2822 4d61 726b 2033 3a31  geList("Mark 3:1
-0000ec30: 2d34 3a32 3b20 353a 362d 382c 2031 303b  -4:2; 5:6-8, 10;
-0000ec40: 204d 6174 7420 3422 290a 2020 2020 2020   Matt 4").      
-0000ec50: 2020 3e3e 3e20 7261 6e67 655f 6c69 7374    >>> range_list
-0000ec60: 2e67 726f 7570 735b 315d 0a20 2020 2020  .groups[1].     
-0000ec70: 2020 2047 726f 7570 5669 6577 285b 4269     GroupView([Bi
-0000ec80: 626c 6552 616e 6765 284d 6172 6b20 353a  bleRange(Mark 5:
-0000ec90: 362d 3829 2c20 4269 626c 6552 616e 6765  6-8), BibleRange
-0000eca0: 284d 6172 6b20 353a 3130 295d 290a 2020  (Mark 5:10)]).  
-0000ecb0: 2020 2020 2020 3e3e 3e20 7374 7228 7261        >>> str(ra
-0000ecc0: 6e67 655f 6c69 7374 2e67 726f 7570 735b  nge_list.groups[
-0000ecd0: 315d 290a 2020 2020 2020 2020 275b 4269  1]).        '[Bi
-0000ece0: 626c 6552 616e 6765 284d 6172 6b20 353a  bleRange(Mark 5:
-0000ecf0: 362d 3829 2c20 4269 626c 6552 616e 6765  6-8), BibleRange
-0000ed00: 284d 6172 6b20 353a 3130 295d 270a 2020  (Mark 5:10)]'.  
-0000ed10: 2020 2020 2020 3e3e 3e20 7374 7228 4269        >>> str(Bi
-0000ed20: 626c 6552 616e 6765 4c69 7374 2872 616e  bleRangeList(ran
-0000ed30: 6765 5f6c 6973 742e 6772 6f75 7073 5b31  ge_list.groups[1
-0000ed40: 5d29 290a 2020 2020 2020 2020 274d 6172  ])).        'Mar
-0000ed50: 6b20 353a 362d 382c 2031 3027 2020 2020  k 5:6-8, 10'    
-0000ed60: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-0000ed70: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000ed80: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-0000ed90: 7228 292e 6772 6f75 7073 2020 2020 0a0a  r().groups    ..
-0000eda0: 2020 2020 6465 6620 5f63 6865 636b 5f74      def _check_t
-0000edb0: 7970 6528 7365 6c66 2c20 7661 6c75 6529  ype(self, value)
-0000edc0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-0000edd0: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-0000ede0: 652c 2042 6962 6c65 5261 6e67 6529 3a0a  e, BibleRange):.
-0000edf0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000ee00: 6520 5479 7065 4572 726f 7228 6622 4974  e TypeError(f"It
-0000ee10: 656d 2069 7320 6e6f 7420 6120 4269 626c  em is not a Bibl
-0000ee20: 6552 616e 6765 3a20 7b76 616c 7565 7d22  eRange: {value}"
-0000ee30: 290a 0a20 2020 2064 6566 2076 6572 7365  )..    def verse
-0000ee40: 5f30 5f74 6f5f 3128 7365 6c66 293a 0a20  _0_to_1(self):. 
-0000ee50: 2020 2020 2020 2027 2727 4d6f 6469 6669         '''Modifi
-0000ee60: 6573 2074 6869 7320 6c69 7374 202a 696e  es this list *in
-0000ee70: 2d70 6c61 6365 2a20 6279 2063 616c 6c69  -place* by calli
-0000ee80: 6e67 2060 7665 7273 655f 305f 746f 5f31  ng `verse_0_to_1
-0000ee90: 2829 6020 6f6e 2065 7665 7279 2060 4269  ()` on every `Bi
-0000eea0: 626c 6552 616e 6765 6020 696e 2074 6865  bleRange` in the
-0000eeb0: 206c 6973 740a 2020 2020 2020 2020 616e   list.        an
-0000eec0: 6420 7573 696e 6720 7468 6520 7265 7375  d using the resu
-0000eed0: 6c74 2074 6f20 7265 706c 6163 6520 7468  lt to replace th
-0000eee0: 6520 6f72 6967 696e 616c 2072 616e 6765  e original range
-0000eef0: 2e20 5265 7475 726e 7320 604e 6f6e 6560  . Returns `None`
-0000ef00: 2e27 2727 0a20 2020 2020 2020 2066 6f72  .'''.        for
-0000ef10: 206e 6f64 6520 696e 2073 656c 662e 5f6e   node in self._n
-0000ef20: 6f64 655f 6974 6572 2829 3a0a 2020 2020  ode_iter():.    
-0000ef30: 2020 2020 2020 2020 6e6f 6465 2e76 616c          node.val
-0000ef40: 7565 203d 206e 6f64 652e 7661 6c75 652e  ue = node.value.
-0000ef50: 7665 7273 655f 305f 746f 5f31 2829 0a20  verse_0_to_1(). 
-0000ef60: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-0000ef70: 6e65 0a0a 2020 2020 6465 6620 7665 7273  ne..    def vers
-0000ef80: 655f 315f 746f 5f30 2873 656c 6629 3a0a  e_1_to_0(self):.
-0000ef90: 2020 2020 2020 2020 2727 274d 6f64 6966          '''Modif
-0000efa0: 6965 7320 7468 6973 206c 6973 7420 2a69  ies this list *i
-0000efb0: 6e2d 706c 6163 652a 2062 7920 6361 6c6c  n-place* by call
-0000efc0: 696e 6720 6076 6572 7365 5f31 5f74 6f5f  ing `verse_1_to_
-0000efd0: 3028 2960 206f 6e20 6576 6572 7920 6042  0()` on every `B
-0000efe0: 6962 6c65 5261 6e67 6560 2069 6e20 7468  ibleRange` in th
-0000eff0: 6520 6c69 7374 0a20 2020 2020 2020 2061  e list.        a
-0000f000: 6e64 2075 7369 6e67 2074 6865 2072 6573  nd using the res
-0000f010: 756c 7420 746f 2072 6570 6c61 6365 2074  ult to replace t
-0000f020: 6865 206f 7269 6769 6e61 6c20 7261 6e67  he original rang
-0000f030: 652e 2052 6574 7572 6e73 2060 4e6f 6e65  e. Returns `None
-0000f040: 602e 0a20 2020 2020 2020 202a 2a4e 6f74  `..        **Not
-0000f050: 652a 2a3a 2054 6865 2076 616c 7565 206f  e**: The value o
-0000f060: 6620 7468 6520 676c 6f62 616c 2061 7474  f the global att
-0000f070: 7269 6275 7465 2060 6269 626c 6572 6566  ribute `bibleref
-0000f080: 2e72 6566 2e66 6c61 6773 6020 6973 202a  .ref.flags` is *
-0000f090: 6967 6e6f 7265 642a 2e27 2727 0a20 2020  ignored*.'''.   
-0000f0a0: 2020 2020 2066 6f72 206e 6f64 6520 696e       for node in
-0000f0b0: 2073 656c 662e 5f6e 6f64 655f 6974 6572   self._node_iter
-0000f0c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000f0d0: 6e6f 6465 2e76 616c 7565 203d 206e 6f64  node.value = nod
-0000f0e0: 652e 7661 6c75 652e 7665 7273 655f 315f  e.value.verse_1_
-0000f0f0: 746f 5f30 2829 0a20 2020 2020 2020 2072  to_0().        r
-0000f100: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000f110: 6465 6620 7665 7273 655f 636f 756e 7428  def verse_count(
-0000f120: 7365 6c66 2c20 666c 6167 733a 2042 6962  self, flags: Bib
-0000f130: 6c65 466c 6167 203d 204e 6f6e 6529 3a0a  leFlag = None):.
-0000f140: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-0000f150: 6e73 2074 6865 2074 6f74 616c 206e 756d  ns the total num
-0000f160: 6265 7220 6f66 2076 6572 7365 7320 696e  ber of verses in
-0000f170: 2074 6865 2072 616e 6765 7320 696e 2074   the ranges in t
-0000f180: 6865 206c 6973 742e 2727 270a 2020 2020  he list.'''.    
-0000f190: 2020 2020 7265 7475 726e 2073 756d 285b      return sum([
-0000f1a0: 6269 626c 655f 7261 6e67 652e 7665 7273  bible_range.vers
-0000f1b0: 655f 636f 756e 7428 666c 6167 733d 666c  e_count(flags=fl
-0000f1c0: 6167 7329 2066 6f72 2062 6962 6c65 5f72  ags) for bible_r
-0000f1d0: 616e 6765 2069 6e20 7365 6c66 5d29 0a0a  ange in self])..
-0000f1e0: 2020 2020 6465 6620 6368 6170 5f63 6f75      def chap_cou
-0000f1f0: 6e74 2873 656c 662c 2077 686f 6c65 3a20  nt(self, whole: 
-0000f200: 626f 6f6c 203d 2046 616c 7365 2c20 666c  bool = False, fl
-0000f210: 6167 733a 2042 6962 6c65 466c 6167 203d  ags: BibleFlag =
-0000f220: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0000f230: 2727 2752 6574 7572 6e73 2074 6865 2074  '''Returns the t
-0000f240: 6f74 616c 206e 756d 6265 7220 6f66 2063  otal number of c
-0000f250: 6861 7074 6572 7320 696e 2074 6865 2072  hapters in the r
-0000f260: 616e 6765 7320 696e 2074 6865 206c 6973  anges in the lis
-0000f270: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-0000f280: 2020 2020 4966 2060 7768 6f6c 6560 2069      If `whole` i
-0000f290: 7320 5472 7565 2c20 6f6e 6c79 2077 686f  s True, only who
-0000f2a0: 6c65 2063 6861 7074 6572 7320 6172 6520  le chapters are 
-0000f2b0: 636f 756e 7465 642e 204f 7468 6572 7769  counted. Otherwi
-0000f2c0: 7365 2070 6172 7469 616c 2063 6861 7074  se partial chapt
-0000f2d0: 6572 7320 6172 6520 616c 736f 2069 6e63  ers are also inc
-0000f2e0: 6c75 6465 6420 696e 2074 6865 0a20 2020  luded in the.   
-0000f2f0: 2020 2020 2063 6f75 6e74 2e27 2727 0a20       count.'''. 
-0000f300: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-0000f310: 6d28 5b62 6962 6c65 5f72 616e 6765 2e63  m([bible_range.c
-0000f320: 6861 705f 636f 756e 7428 7768 6f6c 653d  hap_count(whole=
-0000f330: 7768 6f6c 652c 2066 6c61 6773 3d66 6c61  whole, flags=fla
-0000f340: 6773 2920 666f 7220 6269 626c 655f 7261  gs) for bible_ra
-0000f350: 6e67 6520 696e 2073 656c 665d 290a 0a20  nge in self]).. 
-0000f360: 2020 2064 6566 2062 6f6f 6b5f 636f 756e     def book_coun
-0000f370: 7428 7365 6c66 2c20 7768 6f6c 653a 2062  t(self, whole: b
-0000f380: 6f6f 6c20 3d20 4661 6c73 652c 2066 6c61  ool = False, fla
-0000f390: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-0000f3a0: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
-0000f3b0: 2727 5265 7475 726e 7320 7468 6520 746f  ''Returns the to
-0000f3c0: 7461 6c20 6e75 6d62 6572 206f 6620 4269  tal number of Bi
-0000f3d0: 626c 6520 626f 6f6b 7320 696e 2074 6865  ble books in the
-0000f3e0: 2072 616e 6765 7320 696e 2074 6865 206c   ranges in the l
-0000f3f0: 6973 742e 0a20 2020 2020 2020 200a 2020  ist..        .  
-0000f400: 2020 2020 2020 4966 2060 7768 6f6c 6560        If `whole`
-0000f410: 2069 7320 5472 7565 2c20 6f6e 6c79 2077   is True, only w
-0000f420: 686f 6c65 2062 6f6f 6b73 2061 7265 2063  hole books are c
-0000f430: 6f75 6e74 6564 2e20 4f74 6865 7277 6973  ounted. Otherwis
-0000f440: 652c 2070 6172 7469 616c 2062 6f6f 6b73  e, partial books
-0000f450: 2061 7265 2061 6c73 6f20 696e 636c 7564   are also includ
-0000f460: 6564 2069 6e20 7468 6520 636f 756e 742e  ed in the count.
-0000f470: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
-0000f480: 726e 2073 756d 285b 6269 626c 655f 7261  rn sum([bible_ra
-0000f490: 6e67 652e 626f 6f6b 5f63 6f75 6e74 2877  nge.book_count(w
-0000f4a0: 686f 6c65 3d77 686f 6c65 2c20 666c 6167  hole=whole, flag
-0000f4b0: 733d 666c 6167 7329 2066 6f72 2062 6962  s=flags) for bib
-0000f4c0: 6c65 5f72 616e 6765 2069 6e20 7365 6c66  le_range in self
-0000f4d0: 5d29 0a0a 2020 2020 6465 6620 7261 6e67  ])..    def rang
-0000f4e0: 6528 7365 6c66 2920 2d3e 2027 4269 626c  e(self) -> 'Bibl
-0000f4f0: 6552 616e 6765 273a 0a20 2020 2020 2020  eRange':.       
-0000f500: 2027 2727 5265 7475 726e 7320 6120 6e65   '''Returns a ne
-0000f510: 7720 6d69 6e69 6d75 6d20 6042 6962 6c65  w minimum `Bible
-0000f520: 5261 6e67 6560 2074 6861 7420 696e 636c  Range` that incl
-0000f530: 7564 6573 2065 7665 7279 2076 6572 7365  udes every verse
-0000f540: 2069 6e20 7468 6973 206c 6973 742e 0a20   in this list.. 
-0000f550: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000f560: 4269 626c 6546 6c61 672e 414c 4c20 6973  BibleFlag.ALL is
-0000f570: 2061 6c77 6179 7320 7365 7420 666f 7220   always set for 
-0000f580: 7468 6973 206d 6574 686f 642c 2072 6567  this method, reg
-0000f590: 6172 646c 6573 7320 6f66 2074 6865 2076  ardless of the v
-0000f5a0: 616c 7565 206f 6620 6062 6962 6c65 7265  alue of `biblere
-0000f5b0: 662e 666c 6167 7360 2e0a 2020 2020 2020  f.flags`..      
-0000f5c0: 2020 2727 270a 2020 2020 2020 2020 6d69    '''.        mi
-0000f5d0: 6e5f 7261 6e67 653a 2042 6962 6c65 5261  n_range: BibleRa
-0000f5e0: 6e67 6520 3d20 6d69 6e28 7365 6c66 290a  nge = min(self).
-0000f5f0: 2020 2020 2020 2020 6d61 785f 7261 6e67          max_rang
-0000f600: 653a 2042 6962 6c65 5261 6e67 6520 3d20  e: BibleRange = 
-0000f610: 6d61 7828 7365 6c66 290a 2020 2020 2020  max(self).      
-0000f620: 2020 7265 7475 726e 2042 6962 6c65 5261    return BibleRa
-0000f630: 6e67 6528 7374 6172 743d 6d69 6e5f 7261  nge(start=min_ra
-0000f640: 6e67 652e 7374 6172 742c 2065 6e64 3d6d  nge.start, end=m
-0000f650: 6178 5f72 616e 6765 2e65 6e64 2c20 666c  ax_range.end, fl
-0000f660: 6167 733d 4269 626c 6546 6c61 672e 414c  ags=BibleFlag.AL
-0000f670: 4c29 0a0a 2020 2020 6465 6620 6368 6170  L)..    def chap
-0000f680: 5f72 616e 6765 2873 656c 662c 2066 6c61  _range(self, fla
-0000f690: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-0000f6a0: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
-0000f6b0: 616e 6765 273a 0a20 2020 2020 2020 2027  ange':.        '
-0000f6c0: 2727 5265 7475 726e 7320 6120 6e65 7720  ''Returns a new 
-0000f6d0: 6d69 6e69 6d75 6d20 6042 6962 6c65 5261  minimum `BibleRa
-0000f6e0: 6e67 6560 2074 6861 7420 696e 636c 7564  nge` that includ
-0000f6f0: 6573 2065 7665 7279 2076 6572 7365 2069  es every verse i
-0000f700: 6e20 7468 6973 206c 6973 742c 2061 6e64  n this list, and
-0000f710: 2062 6567 696e 7320 616e 6420 656e 6473   begins and ends
-0000f720: 2061 740a 2020 2020 2020 2020 6368 6170   at.        chap
-0000f730: 7465 7220 626f 756e 6461 7269 6573 2e0a  ter boundaries..
-0000f740: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000f750: 2042 6962 6c65 466c 6167 2e4d 554c 5449   BibleFlag.MULTI
-0000f760: 424f 4f4b 2069 7320 616c 7761 7973 2073  BOOK is always s
-0000f770: 6574 2066 6f72 2074 6869 7320 6d65 7468  et for this meth
-0000f780: 6f64 2c20 7265 6761 7264 6c65 7373 206f  od, regardless o
-0000f790: 6620 7468 6520 7661 6c75 6520 6f66 2060  f the value of `
-0000f7a0: 666c 6167 7360 2e0a 2020 2020 2020 2020  flags`..        
-0000f7b0: 2727 270a 2020 2020 2020 2020 666c 6167  '''.        flag
-0000f7c0: 7320 3d20 666c 6167 7320 6f72 2062 6962  s = flags or bib
-0000f7d0: 6c65 7265 662e 666c 6167 7320 6f72 2042  leref.flags or B
-0000f7e0: 6962 6c65 466c 6167 2e4e 4f4e 450a 2020  ibleFlag.NONE.  
-0000f7f0: 2020 2020 2020 666c 6167 7320 7c3d 2042        flags |= B
-0000f800: 6962 6c65 466c 6167 2e4d 554c 5449 424f  ibleFlag.MULTIBO
-0000f810: 4f4b 0a20 2020 2020 2020 206d 696e 5f72  OK.        min_r
-0000f820: 616e 6765 3a20 4269 626c 6552 616e 6765  ange: BibleRange
-0000f830: 203d 206d 696e 2873 656c 6629 0a20 2020   = min(self).   
-0000f840: 2020 2020 206d 6178 5f72 616e 6765 3a20       max_range: 
-0000f850: 4269 626c 6552 616e 6765 203d 206d 6178  BibleRange = max
-0000f860: 2873 656c 6629 0a20 2020 2020 2020 2072  (self).        r
-0000f870: 6574 7572 6e20 4269 626c 6552 616e 6765  eturn BibleRange
-0000f880: 2873 7461 7274 3d6d 696e 5f72 616e 6765  (start=min_range
-0000f890: 2e73 7461 7274 2e66 6972 7374 5f76 6572  .start.first_ver
-0000f8a0: 7365 2866 6c61 6773 3d66 6c61 6773 292c  se(flags=flags),
-0000f8b0: 2065 6e64 3d6d 6178 5f72 616e 6765 2e65   end=max_range.e
-0000f8c0: 6e64 2e6c 6173 745f 7665 7273 6528 292c  nd.last_verse(),
-0000f8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f8e0: 2020 2020 2020 2020 2020 2066 6c61 6773             flags
-0000f8f0: 3d66 6c61 6773 290a 0a20 2020 2064 6566  =flags)..    def
-0000f900: 2062 6f6f 6b5f 7261 6e67 6528 7365 6c66   book_range(self
-0000f910: 2c20 666c 6167 733a 2042 6962 6c65 466c  , flags: BibleFl
-0000f920: 6167 203d 204e 6f6e 6529 202d 3e20 2742  ag = None) -> 'B
-0000f930: 6962 6c65 5261 6e67 6527 3a0a 2020 2020  ibleRange':.    
-0000f940: 2020 2020 2727 2752 6574 7572 6e73 2061      '''Returns a
-0000f950: 206e 6577 206d 696e 696d 756d 2060 4269   new minimum `Bi
-0000f960: 626c 6552 616e 6765 6020 7468 6174 2069  bleRange` that i
-0000f970: 6e63 6c75 6465 7320 6576 6572 7920 7665  ncludes every ve
-0000f980: 7273 6520 696e 2074 6869 7320 6c69 7374  rse in this list
-0000f990: 2c20 616e 6420 6265 6769 6e73 2061 6e64  , and begins and
-0000f9a0: 2065 6e64 7320 6174 0a20 2020 2020 2020   ends at.       
-0000f9b0: 2062 6f6f 6b20 626f 756e 6461 7269 6573   book boundaries
-0000f9c0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-0000f9d0: 2020 2042 6962 6c65 466c 6167 2e4d 554c     BibleFlag.MUL
-0000f9e0: 5449 424f 4f4b 2069 7320 616c 7761 7973  TIBOOK is always
-0000f9f0: 2073 6574 2066 6f72 2074 6869 7320 6d65   set for this me
-0000fa00: 7468 6f64 2c20 7265 6761 7264 6c65 7373  thod, regardless
-0000fa10: 206f 6620 7468 6520 7661 6c75 6520 6f66   of the value of
-0000fa20: 2060 666c 6167 7360 2e0a 2020 2020 2020   `flags`..      
-0000fa30: 2020 2727 270a 2020 2020 2020 2020 666c    '''.        fl
-0000fa40: 6167 7320 3d20 666c 6167 7320 6f72 2062  ags = flags or b
-0000fa50: 6962 6c65 7265 662e 666c 6167 7320 6f72  ibleref.flags or
-0000fa60: 2042 6962 6c65 466c 6167 2e4e 4f4e 450a   BibleFlag.NONE.
-0000fa70: 2020 2020 2020 2020 666c 6167 7320 7c3d          flags |=
-0000fa80: 2042 6962 6c65 466c 6167 2e4d 554c 5449   BibleFlag.MULTI
-0000fa90: 424f 4f4b 0a20 2020 2020 2020 206d 696e  BOOK.        min
-0000faa0: 5f72 616e 6765 3a20 4269 626c 6552 616e  _range: BibleRan
-0000fab0: 6765 203d 206d 696e 2873 656c 6629 0a20  ge = min(self). 
-0000fac0: 2020 2020 2020 206d 6178 5f72 616e 6765         max_range
-0000fad0: 3a20 4269 626c 6552 616e 6765 203d 206d  : BibleRange = m
-0000fae0: 6178 2873 656c 6629 0a20 2020 2020 2020  ax(self).       
-0000faf0: 2072 6574 7572 6e20 4269 626c 6552 616e   return BibleRan
-0000fb00: 6765 2873 7461 7274 3d6d 696e 5f72 616e  ge(start=min_ran
-0000fb10: 6765 2e73 7461 7274 2e62 6f6f 6b2e 6669  ge.start.book.fi
-0000fb20: 7273 745f 7665 7273 6528 666c 6167 733d  rst_verse(flags=
-0000fb30: 666c 6167 7329 2c20 656e 643d 6d61 785f  flags), end=max_
-0000fb40: 7261 6e67 652e 656e 642e 626f 6f6b 2e6c  range.end.book.l
-0000fb50: 6173 745f 7665 7273 6528 292c 0a20 2020  ast_verse(),.   
-0000fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb70: 2020 2020 2020 2066 6c61 6773 3d66 6c61         flags=fla
-0000fb80: 6773 290a 0a20 2020 2064 6566 2073 6f72  gs)..    def sor
-0000fb90: 7428 7365 6c66 2c20 7265 6772 6f75 703a  t(self, regroup:
-0000fba0: 2062 6f6f 6c20 3d20 5472 7565 293a 0a20   bool = True):. 
-0000fbb0: 2020 2020 2020 2027 2727 536f 7274 7320         '''Sorts 
-0000fbc0: 7468 6973 206c 6973 7420 696e 2d70 6c61  this list in-pla
-0000fbd0: 6365 2e20 416c 6c20 6578 6973 7469 6e67  ce. All existing
-0000fbe0: 2067 726f 7570 7320 6172 6520 636c 6561   groups are clea
-0000fbf0: 7265 6420 616e 6420 7265 706c 6163 6564  red and replaced
-0000fc00: 2077 6974 6820 6120 7369 6e67 6c65 0a20   with a single. 
-0000fc10: 2020 2020 2020 206e 6577 2067 726f 7570         new group
-0000fc20: 2e20 5468 656e 2072 6567 726f 7570 7320  . Then regroups 
-0000fc30: 6966 2060 7265 6772 6f75 7060 2069 7320  if `regroup` is 
-0000fc40: 5472 7565 2e27 2727 0a20 2020 2020 2020  True.'''.       
-0000fc50: 2073 7570 6572 2829 2e73 6f72 7428 290a   super().sort().
-0000fc60: 2020 2020 2020 2020 6966 2072 6567 726f          if regro
-0000fc70: 7570 3a0a 2020 2020 2020 2020 2020 2020  up:.            
-0000fc80: 7365 6c66 2e72 6567 726f 7570 2829 0a0a  self.regroup()..
-0000fc90: 2020 2020 6465 6620 6d65 7267 6528 7365      def merge(se
-0000fca0: 6c66 2c20 666c 6167 733a 2042 6962 6c65  lf, flags: Bible
-0000fcb0: 466c 6167 203d 204e 6f6e 6529 3a0a 2020  Flag = None):.  
-0000fcc0: 2020 2020 2020 2727 2753 6f72 7473 2074        '''Sorts t
-0000fcd0: 6869 7320 6c69 7374 2069 6e2d 706c 6163  his list in-plac
-0000fce0: 6520 616e 6420 6d65 7267 6573 2072 616e  e and merges ran
-0000fcf0: 6765 7320 7768 6572 6576 6572 2070 6f73  ges wherever pos
-0000fd00: 7369 626c 652c 2074 6865 6e20 7265 6772  sible, then regr
-0000fd10: 6f75 7073 2e20 5468 6520 7265 7375 6c74  oups. The result
-0000fd20: 2069 7320 7468 6520 736d 616c 6c65 7374   is the smallest
-0000fd30: 0a20 2020 2020 2020 206c 6973 7420 6f66  .        list of
-0000fd40: 2064 6973 6a6f 696e 742c 206e 6f6e 2d61   disjoint, non-a
-0000fd50: 646a 6163 656e 7420 6042 6962 6c65 5261  djacent `BibleRa
-0000fd60: 6e67 6560 2065 6c65 6d65 6e74 7320 7370  nge` elements sp
-0000fd70: 616e 6e69 6e67 2074 6865 2073 616d 6520  anning the same 
-0000fd80: 7665 7273 6573 2061 7320 696e 2074 6865  verses as in the
-0000fd90: 206f 7269 6769 6e61 6c0a 2020 2020 2020   original.      
-0000fda0: 2020 6c69 7374 2e0a 2020 2020 2020 2020    list..        
-0000fdb0: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
-0000fdc0: 2e73 6f72 7428 7265 6772 6f75 703d 4661  .sort(regroup=Fa
-0000fdd0: 6c73 6529 0a20 2020 2020 2020 206e 6f64  lse).        nod
-0000fde0: 6520 3d20 7365 6c66 2e5f 6669 7273 740a  e = self._first.
-0000fdf0: 2020 2020 2020 2020 7768 696c 6520 6e6f          while no
-0000fe00: 6465 2069 7320 6e6f 7420 4e6f 6e65 2061  de is not None a
-0000fe10: 6e64 206e 6f64 652e 6e65 7874 2069 7320  nd node.next is 
-0000fe20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000fe30: 2020 2020 2020 756e 696f 6e20 3d20 6e6f        union = no
-0000fe40: 6465 2e76 616c 7565 2e75 6e69 6f6e 286e  de.value.union(n
-0000fe50: 6f64 652e 6e65 7874 2e76 616c 7565 2c20  ode.next.value, 
-0000fe60: 666c 6167 733d 666c 6167 7329 0a20 2020  flags=flags).   
-0000fe70: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000fe80: 756e 696f 6e29 203d 3d20 313a 2023 2043  union) == 1: # C
-0000fe90: 616e 206d 6572 6765 2074 6865 7365 2074  an merge these t
-0000fea0: 776f 2072 616e 6765 7320 7769 7468 2074  wo ranges with t
-0000feb0: 6865 6972 2075 6e69 6f6e 0a20 2020 2020  heir union.     
-0000fec0: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
-0000fed0: 7661 6c75 6520 3d20 756e 696f 6e5b 305d  value = union[0]
-0000fee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fef0: 2073 656c 662e 5f70 6f70 5f61 6674 6572   self._pop_after
-0000ff00: 286e 6f64 6529 0a20 2020 2020 2020 2020  (node).         
-0000ff10: 2020 2020 2020 2023 2057 6520 646f 6e27         # We don'
-0000ff20: 7420 6d6f 7665 206f 6e20 7965 742c 2073  t move on yet, s
-0000ff30: 6f20 7765 2063 616e 2063 6f6d 7061 7265  o we can compare
-0000ff40: 2074 6865 206e 6577 6c79 206d 6572 6765   the newly merge
-0000ff50: 6420 7261 6e67 650a 2020 2020 2020 2020  d range.        
-0000ff60: 2020 2020 2020 2020 2320 7769 7468 2074          # with t
-0000ff70: 6865 2028 6e65 7729 206e 6578 7420 6e6f  he (new) next no
-0000ff80: 6465 0a20 2020 2020 2020 2020 2020 2065  de.            e
-0000ff90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ffa0: 2020 2020 2023 2054 6865 2074 776f 2072       # The two r
-0000ffb0: 616e 6765 7320 6361 6e27 7420 6265 206d  anges can't be m
-0000ffc0: 6572 6765 642c 2073 6f20 6d6f 7665 206f  erged, so move o
-0000ffd0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000ffe0: 2020 6e6f 6465 203d 206e 6f64 652e 6e65    node = node.ne
-0000fff0: 7874 0a20 2020 2020 2020 2073 656c 662e  xt.        self.
-00010000: 7265 6772 6f75 7028 290a 0a20 2020 2064  regroup()..    d
-00010010: 6566 2069 735f 6469 736a 6f69 6e74 2873  ef is_disjoint(s
-00010020: 656c 662c 206f 7468 6572 5f72 6566 3a20  elf, other_ref: 
-00010030: 2742 6962 6c65 5265 6627 2920 2d3e 2062  'BibleRef') -> b
-00010040: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-00010050: 5265 7475 726e 7320 6054 7275 6560 2069  Returns `True` i
-00010060: 6620 6576 6572 7920 6042 6962 6c65 5261  f every `BibleRa
-00010070: 6e67 6560 2069 7320 6469 736a 6f69 6e74  nge` is disjoint
-00010080: 2077 6974 6820 616c 6c20 7468 6520 7665   with all the ve
-00010090: 7273 6573 2069 6e20 606f 7468 6572 5f72  rses in `other_r
-000100a0: 6566 602c 206f 7468 6572 7769 7365 2060  ef`, otherwise `
-000100b0: 4661 6c73 6560 2e0a 2020 2020 2020 2020  False`..        
-000100c0: 2727 270a 2020 2020 2020 2020 6966 2069  '''.        if i
-000100d0: 7369 6e73 7461 6e63 6528 6f74 6865 725f  sinstance(other_
-000100e0: 7265 662c 2042 6962 6c65 5665 7273 6529  ref, BibleVerse)
-000100f0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00010100: 436f 6e76 6572 7420 746f 2042 6962 6c65  Convert to Bible
-00010110: 5261 6e67 654c 6973 7420 2861 6e64 2077  RangeList (and w
-00010120: 6520 646f 6e27 7420 656e 666f 7263 6520  e don't enforce 
-00010130: 6578 6973 7469 6e67 2066 6c61 6773 2066  existing flags f
-00010140: 6f72 2063 6f6e 7665 7273 696f 6e73 290a  or conversions).
-00010150: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00010160: 725f 7265 6620 3d20 4269 626c 6552 616e  r_ref = BibleRan
-00010170: 6765 4c69 7374 285b 4269 626c 6552 616e  geList([BibleRan
-00010180: 6765 2873 7461 7274 3d6f 7468 6572 5f72  ge(start=other_r
-00010190: 6566 2c20 656e 643d 6f74 6865 725f 7265  ef, end=other_re
-000101a0: 662c 2066 6c61 6773 3d42 6962 6c65 466c  f, flags=BibleFl
-000101b0: 6167 2e41 4c4c 295d 290a 2020 2020 2020  ag.ALL)]).      
-000101c0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-000101d0: 6528 6f74 6865 725f 7265 662c 2042 6962  e(other_ref, Bib
-000101e0: 6c65 5261 6e67 6529 3a0a 2020 2020 2020  leRange):.      
-000101f0: 2020 2020 2020 6f74 6865 725f 7265 6620        other_ref 
-00010200: 3d20 4269 626c 6552 616e 6765 4c69 7374  = BibleRangeList
-00010210: 285b 6f74 6865 725f 7265 665d 290a 2020  ([other_ref]).  
-00010220: 2020 2020 2020 7265 7475 726e 2061 6c6c        return all
-00010230: 2873 656c 665f 7261 6e67 652e 6973 5f64  (self_range.is_d
-00010240: 6973 6a6f 696e 7428 6f74 6865 725f 7261  isjoint(other_ra
-00010250: 6e67 6529 2066 6f72 2073 656c 665f 7261  nge) for self_ra
-00010260: 6e67 6520 696e 2073 656c 6620 666f 7220  nge in self for 
-00010270: 6f74 6865 725f 7261 6e67 6520 696e 206f  other_range in o
-00010280: 7468 6572 5f72 6566 290a 0a20 2020 2064  ther_ref)..    d
-00010290: 6566 2063 6f6e 7461 696e 7328 7365 6c66  ef contains(self
-000102a0: 2c20 6f74 6865 725f 7265 663a 2027 4269  , other_ref: 'Bi
-000102b0: 626c 6552 6566 272c 2066 6c61 6773 3a20  bleRef', flags: 
-000102c0: 4269 626c 6546 6c61 6720 3d20 4e6f 6e65  BibleFlag = None
-000102d0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-000102e0: 2020 2027 2727 5265 7475 726e 7320 6054     '''Returns `T
-000102f0: 7275 6560 2069 6620 616c 6c20 7468 6520  rue` if all the 
-00010300: 7665 7273 6573 2069 6e20 606f 7468 6572  verses in `other
-00010310: 5f72 6566 6020 6661 6c6c 2077 6974 6869  _ref` fall withi
-00010320: 6e20 6174 206c 6561 7374 206f 6e65 206f  n at least one o
-00010330: 6620 7468 6520 6042 6962 6c65 5261 6e67  f the `BibleRang
-00010340: 6560 2065 6c65 6d65 6e74 730a 2020 2020  e` elements.    
-00010350: 2020 2020 696e 2074 6869 7320 6c69 7374      in this list
-00010360: 2e20 4f74 6865 7277 6973 6520 7265 7475  . Otherwise retu
-00010370: 726e 7320 6046 616c 7365 602e 0a0a 2020  rns `False`...  
-00010380: 2020 2020 2020 5468 6520 7361 6d65 2072        The same r
-00010390: 6573 756c 7420 6973 2072 6574 7572 6e65  esult is returne
-000103a0: 6420 7573 696e 6720 7468 6520 2769 6e27  d using the 'in'
-000103b0: 206f 7065 7261 746f 7220 2869 2e65 2e20   operator (i.e. 
-000103c0: 606f 7468 6572 5f72 6566 2069 6e20 6269  `other_ref in bi
-000103d0: 626c 655f 7261 6e67 655f 6c69 7374 6029  ble_range_list`)
-000103e0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-000103f0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00010400: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
-00010410: 6962 6c65 5665 7273 6529 3a0a 2020 2020  ibleVerse):.    
-00010420: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-00010430: 7420 746f 2042 6962 6c65 5261 6e67 654c  t to BibleRangeL
-00010440: 6973 7420 2861 6e64 2077 6520 646f 6e27  ist (and we don'
-00010450: 7420 656e 666f 7263 6520 6578 6973 7469  t enforce existi
-00010460: 6e67 2066 6c61 6773 2066 6f72 2063 6f6e  ng flags for con
-00010470: 7665 7273 696f 6e73 290a 2020 2020 2020  versions).      
-00010480: 2020 2020 2020 6f74 6865 725f 7265 6620        other_ref 
-00010490: 3d20 4269 626c 6552 616e 6765 4c69 7374  = BibleRangeList
-000104a0: 285b 4269 626c 6552 616e 6765 2873 7461  ([BibleRange(sta
-000104b0: 7274 3d6f 7468 6572 5f72 6566 2c20 656e  rt=other_ref, en
-000104c0: 643d 6f74 6865 725f 7265 662c 2066 6c61  d=other_ref, fla
-000104d0: 6773 3d42 6962 6c65 466c 6167 2e41 4c4c  gs=BibleFlag.ALL
-000104e0: 295d 290a 2020 2020 2020 2020 656c 6966  )]).        elif
-000104f0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-00010500: 725f 7265 662c 2042 6962 6c65 5261 6e67  r_ref, BibleRang
-00010510: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00010520: 6f74 6865 725f 7265 6620 3d20 4269 626c  other_ref = Bibl
-00010530: 6552 616e 6765 4c69 7374 285b 6f74 6865  eRangeList([othe
-00010540: 725f 7265 665d 290a 2020 2020 2020 2020  r_ref]).        
-00010550: 2320 4372 6561 7465 2061 2063 6f6e 736f  # Create a conso
-00010560: 6c69 6461 7465 6420 636f 7079 206f 6620  lidated copy of 
-00010570: 6f75 7273 656c 7665 730a 2020 2020 2020  ourselves.      
-00010580: 2020 7365 6c66 5f63 6f70 7920 3d20 4269    self_copy = Bi
-00010590: 626c 6552 616e 6765 4c69 7374 2873 656c  bleRangeList(sel
-000105a0: 6629 0a20 2020 2020 2020 2073 656c 665f  f).        self_
-000105b0: 636f 7079 2e6d 6572 6765 2866 6c61 6773  copy.merge(flags
-000105c0: 3d66 6c61 6773 290a 2020 2020 2020 2020  =flags).        
-000105d0: 2320 4576 6572 7920 6f6e 6520 6f66 2074  # Every one of t
-000105e0: 6865 206f 7468 6572 206c 6973 7427 7320  he other list's 
-000105f0: 7261 6e67 6573 206d 7573 7420 6265 2063  ranges must be c
-00010600: 6f6e 7461 696e 6564 2062 7920 6174 206c  ontained by at l
-00010610: 6561 7374 206f 6e65 206f 6620 7468 6520  east one of the 
-00010620: 6f75 7220 7261 6e67 6573 0a20 2020 2020  our ranges.     
-00010630: 2020 2072 6574 7572 6e20 616c 6c28 616e     return all(an
-00010640: 7928 7365 6c66 5f72 616e 6765 2e63 6f6e  y(self_range.con
-00010650: 7461 696e 7328 6f74 6865 725f 7261 6e67  tains(other_rang
-00010660: 6529 2066 6f72 2073 656c 665f 7261 6e67  e) for self_rang
-00010670: 6520 696e 2073 656c 665f 636f 7079 2920  e in self_copy) 
-00010680: 666f 7220 6f74 6865 725f 7261 6e67 6520  for other_range 
-00010690: 696e 206f 7468 6572 5f72 6566 290a 0a20  in other_ref).. 
-000106a0: 2020 2064 6566 2075 6e69 6f6e 2873 656c     def union(sel
-000106b0: 662c 206f 7468 6572 5f72 6566 3a20 2742  f, other_ref: 'B
-000106c0: 6962 6c65 5265 6627 2c20 666c 6167 733a  ibleRef', flags:
-000106d0: 2042 6962 6c65 466c 6167 203d 204e 6f6e   BibleFlag = Non
-000106e0: 6529 202d 3e20 2742 6962 6c65 5261 6e67  e) -> 'BibleRang
-000106f0: 654c 6973 7427 3a0a 2020 2020 2020 2020  eList':.        
-00010700: 2727 2743 7265 6174 6573 2061 206e 6577  '''Creates a new
-00010710: 2060 4269 626c 6552 616e 6765 4c69 7374   `BibleRangeList
-00010720: 6020 7468 6174 2063 6f6e 7461 696e 7320  ` that contains 
-00010730: 616c 6c20 7468 6520 7665 7273 6573 2069  all the verses i
-00010740: 6e20 7468 6973 2060 4269 626c 6552 616e  n this `BibleRan
-00010750: 6765 4c69 7374 600a 2020 2020 2020 2020  geList`.        
-00010760: 616e 6420 616c 6c20 7468 6520 7665 7273  and all the vers
-00010770: 6573 2069 6e20 606f 7468 6572 5f72 6566  es in `other_ref
-00010780: 602c 2074 6865 6e20 636f 6e73 6f6c 6964  `, then consolid
-00010790: 6174 6573 2074 6865 2072 6573 756c 7420  ates the result 
-000107a0: 616e 6420 7265 7475 726e 7320 6974 2e0a  and returns it..
-000107b0: 0a20 2020 2020 2020 2055 7369 6e67 2074  .        Using t
-000107c0: 6865 2060 7c60 206f 7065 7261 746f 7220  he `|` operator 
-000107d0: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
-000107e0: 2063 616c 6c69 6e67 2060 756e 696f 6e28   calling `union(
-000107f0: 2960 2077 6974 6820 6066 6c61 6773 203d  )` with `flags =
-00010800: 204e 6f6e 6560 2e0a 2020 2020 2020 2020   None`..        
-00010810: 2727 270a 2020 2020 2020 2020 6e65 775f  '''.        new_
-00010820: 6c69 7374 203d 2042 6962 6c65 5261 6e67  list = BibleRang
-00010830: 654c 6973 7428 7365 6c66 290a 2020 2020  eList(self).    
-00010840: 2020 2020 6e65 775f 6c69 7374 2e75 6e69      new_list.uni
-00010850: 6f6e 5f75 7064 6174 6528 6f74 6865 725f  on_update(other_
-00010860: 7265 662c 2066 6c61 6773 3d66 6c61 6773  ref, flags=flags
-00010870: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010880: 206e 6577 5f6c 6973 740a 0a20 2020 2064   new_list..    d
-00010890: 6566 2075 6e69 6f6e 5f75 7064 6174 6528  ef union_update(
-000108a0: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
-000108b0: 2027 4269 626c 6552 6566 272c 2066 6c61   'BibleRef', fla
-000108c0: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-000108d0: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
-000108e0: 616e 6765 4c69 7374 273a 0a20 2020 2020  angeList':.     
-000108f0: 2020 2027 2727 5570 6461 7465 7320 7468     '''Updates th
-00010900: 6973 206c 6973 7420 746f 2062 6520 7468  is list to be th
-00010910: 6520 756e 696f 6e20 6f66 2069 7473 2065  e union of its e
-00010920: 7869 7374 696e 6720 656c 656d 656e 7473  xisting elements
-00010930: 2061 6e64 2060 6f74 6865 725f 7265 6660   and `other_ref`
-00010940: 2c20 7468 656e 2063 6f6e 736f 6c69 6461  , then consolida
-00010950: 7465 7320 7468 6973 206c 6973 742e 0a0a  tes this list...
-00010960: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
-00010970: 6520 607c 3d60 206f 7065 7261 746f 7220  e `|=` operator 
-00010980: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
-00010990: 2063 616c 6c69 6e67 2060 756e 696f 6e5f   calling `union_
-000109a0: 7570 6461 7465 2829 6020 7769 7468 2060  update()` with `
-000109b0: 666c 6167 7320 3d20 4e6f 6e65 602e 0a20  flags = None`.. 
-000109c0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-000109d0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000109e0: 286f 7468 6572 5f72 6566 2c20 4269 626c  (other_ref, Bibl
-000109f0: 6556 6572 7365 293a 0a20 2020 2020 2020  eVerse):.       
-00010a00: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
-00010a10: 6f20 4269 626c 6552 616e 6765 4c69 7374  o BibleRangeList
-00010a20: 2028 616e 6420 7765 2064 6f6e 2774 2065   (and we don't e
-00010a30: 6e66 6f72 6365 2065 7869 7374 696e 6720  nforce existing 
-00010a40: 666c 6167 7320 666f 7220 636f 6e76 6572  flags for conver
-00010a50: 7369 6f6e 7329 0a20 2020 2020 2020 2020  sions).         
-00010a60: 2020 206f 7468 6572 5f72 6566 203d 2042     other_ref = B
-00010a70: 6962 6c65 5261 6e67 654c 6973 7428 5b42  ibleRangeList([B
-00010a80: 6962 6c65 5261 6e67 6528 7374 6172 743d  ibleRange(start=
-00010a90: 6f74 6865 725f 7265 662c 2065 6e64 3d6f  other_ref, end=o
-00010aa0: 7468 6572 5f72 6566 2c20 666c 6167 733d  ther_ref, flags=
-00010ab0: 4269 626c 6546 6c61 672e 414c 4c29 5d29  BibleFlag.ALL)])
-00010ac0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00010ad0: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
-00010ae0: 6566 2c20 4269 626c 6552 616e 6765 293a  ef, BibleRange):
-00010af0: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
-00010b00: 6572 5f72 6566 203d 2042 6962 6c65 5261  er_ref = BibleRa
-00010b10: 6e67 654c 6973 7428 5b6f 7468 6572 5f72  ngeList([other_r
-00010b20: 6566 5d29 0a20 2020 2020 2020 2069 6620  ef]).        if 
-00010b30: 6e6f 7420 6973 696e 7374 616e 6365 286f  not isinstance(o
-00010b40: 7468 6572 5f72 6566 2c20 4269 626c 6552  ther_ref, BibleR
-00010b50: 616e 6765 4c69 7374 293a 0a20 2020 2020  angeList):.     
-00010b60: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00010b70: 7565 4572 726f 7228 6622 7b6f 7468 6572  ueError(f"{other
-00010b80: 5f72 6566 7d20 6973 206e 6f74 2061 2076  _ref} is not a v
-00010b90: 616c 6964 2042 6962 6c65 5265 6622 2920  alid BibleRef") 
-00010ba0: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-00010bb0: 2073 656c 662e 6578 7465 6e64 286f 7468   self.extend(oth
-00010bc0: 6572 5f72 6566 290a 2020 2020 2020 2020  er_ref).        
-00010bd0: 7365 6c66 2e6d 6572 6765 2866 6c61 6773  self.merge(flags
-00010be0: 3d66 6c61 6773 290a 0a20 2020 2064 6566  =flags)..    def
-00010bf0: 2069 6e74 6572 7365 6374 696f 6e28 7365   intersection(se
-00010c00: 6c66 2c20 6f74 6865 725f 7265 663a 2027  lf, other_ref: '
-00010c10: 4269 626c 6552 6566 272c 2066 6c61 6773  BibleRef', flags
-00010c20: 3a20 4269 626c 6546 6c61 6720 3d20 4e6f  : BibleFlag = No
-00010c30: 6e65 2920 2d3e 2027 4269 626c 6552 616e  ne) -> 'BibleRan
-00010c40: 6765 4c69 7374 273a 0a20 2020 2020 2020  geList':.       
-00010c50: 2027 2727 4372 6561 7465 7320 6120 6e65   '''Creates a ne
-00010c60: 7720 6042 6962 6c65 5261 6e67 654c 6973  w `BibleRangeLis
-00010c70: 7460 206f 6620 7665 7273 6573 2074 6861  t` of verses tha
-00010c80: 7420 6172 6520 636f 6d6d 6f6e 2074 6f20  t are common to 
-00010c90: 626f 7468 2074 6869 7320 6042 6962 6c65  both this `Bible
-00010ca0: 5261 6e67 654c 6973 7460 2061 6e64 2060  RangeList` and `
-00010cb0: 6f74 6865 725f 7265 6660 2c0a 2020 2020  other_ref`,.    
-00010cc0: 2020 2020 7468 656e 2063 6f6e 736f 6c69      then consoli
-00010cd0: 6461 7465 7320 7468 6520 7265 7375 6c74  dates the result
-00010ce0: 2061 6e64 2072 6574 7572 6e73 2069 742e   and returns it.
-00010cf0: 2049 6620 7468 6572 6520 6172 6520 6e6f   If there are no
-00010d00: 2076 6572 7365 7320 696e 2063 6f6d 6d6f   verses in commo
-00010d10: 6e2c 2074 6865 2072 6574 7572 6e65 6420  n, the returned 
-00010d20: 6c69 7374 2069 7320 656d 7074 792e 0a0a  list is empty...
-00010d30: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
-00010d40: 6520 6026 6020 6f70 6572 6174 6f72 2069  e `&` operator i
-00010d50: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
-00010d60: 6361 6c6c 696e 6720 6069 6e74 6572 7365  calling `interse
-00010d70: 6374 696f 6e28 2960 2077 6974 6820 6066  ction()` with `f
-00010d80: 6c61 6773 203d 204e 6f6e 6560 2e0a 2020  lags = None`..  
-00010d90: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00010da0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00010db0: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
-00010dc0: 5665 7273 6529 3a0a 2020 2020 2020 2020  Verse):.        
-00010dd0: 2020 2020 2320 436f 6e76 6572 7420 746f      # Convert to
-00010de0: 2042 6962 6c65 5261 6e67 654c 6973 7420   BibleRangeList 
-00010df0: 2861 6e64 2077 6520 646f 6e27 7420 656e  (and we don't en
-00010e00: 666f 7263 6520 6578 6973 7469 6e67 2066  force existing f
-00010e10: 6c61 6773 2066 6f72 2063 6f6e 7665 7273  lags for convers
-00010e20: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
-00010e30: 2020 6f74 6865 725f 7265 6620 3d20 4269    other_ref = Bi
-00010e40: 626c 6552 616e 6765 4c69 7374 285b 4269  bleRangeList([Bi
-00010e50: 626c 6552 616e 6765 2873 7461 7274 3d6f  bleRange(start=o
-00010e60: 7468 6572 5f72 6566 2c20 656e 643d 6f74  ther_ref, end=ot
-00010e70: 6865 725f 7265 662c 2066 6c61 6773 3d42  her_ref, flags=B
-00010e80: 6962 6c65 466c 6167 2e41 4c4c 295d 290a  ibleFlag.ALL)]).
-00010e90: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00010ea0: 6e73 7461 6e63 6528 6f74 6865 725f 7265  nstance(other_re
-00010eb0: 662c 2042 6962 6c65 5261 6e67 6529 3a0a  f, BibleRange):.
-00010ec0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00010ed0: 725f 7265 6620 3d20 4269 626c 6552 616e  r_ref = BibleRan
-00010ee0: 6765 4c69 7374 285b 6f74 6865 725f 7265  geList([other_re
-00010ef0: 665d 290a 2020 2020 2020 2020 6966 206e  f]).        if n
-00010f00: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
-00010f10: 6865 725f 7265 662c 2042 6962 6c65 5261  her_ref, BibleRa
-00010f20: 6e67 654c 6973 7429 3a0a 2020 2020 2020  ngeList):.      
-00010f30: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00010f40: 6545 7272 6f72 2866 227b 6f74 6865 725f  eError(f"{other_
-00010f50: 7265 667d 2069 7320 6e6f 7420 6120 7661  ref} is not a va
-00010f60: 6c69 6420 4269 626c 6552 6566 2229 2020  lid BibleRef")  
-00010f70: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
-00010f80: 2320 4561 6368 2042 6962 6c65 5265 664c  # Each BibleRefL
-00010f90: 6973 7420 6973 2065 6666 6563 7469 7665  ist is effective
-00010fa0: 6c79 2061 2075 6e69 6f6e 206f 6620 6974  ly a union of it
-00010fb0: 7320 656c 656d 656e 7473 2e0a 2020 2020  s elements..    
-00010fc0: 2020 2020 2320 4b65 7920 7365 7420 7468      # Key set th
-00010fd0: 656f 7279 2069 6465 6e74 6974 793a 0a20  eory identity:. 
-00010fe0: 2020 2020 2020 2023 2020 2028 4130 20e2         #   (A0 .
-00010ff0: 88aa 2041 3129 20e2 88a9 2028 4230 20e2  .. A1) ... (B0 .
-00011000: 88aa 2042 3129 203d 2028 4130 20e2 88a9  .. B1) = (A0 ...
-00011010: 2042 3029 20e2 88aa 2028 4130 20e2 88a9   B0) ... (A0 ...
-00011020: 2042 3129 20e2 88aa 2028 4131 20e2 88a9   B1) ... (A1 ...
-00011030: 2042 3029 20e2 88aa 2028 4131 20e2 88a9   B0) ... (A1 ...
-00011040: 2042 3129 0a20 2020 2020 2020 2023 2053   B1).        # S
-00011050: 6f20 7468 6520 696e 7465 7273 6563 7469  o the intersecti
-00011060: 6f6e 206f 6620 7477 6f20 4269 626c 6552  on of two BibleR
-00011070: 6566 4c69 7374 7320 6973 2061 206e 6577  efLists is a new
-00011080: 206c 6973 7420 6f66 2074 6865 2069 6e74   list of the int
-00011090: 6572 7365 6374 696f 6e20 6f66 2065 6163  ersection of eac
-000110a0: 6820 6974 656d 0a20 2020 2020 2020 2023  h item.        #
-000110b0: 2063 6f6d 6269 6e61 7469 6f6e 2e0a 2020   combination..  
-000110c0: 2020 2020 2020 6e65 775f 6c69 7374 203d        new_list =
-000110d0: 2042 6962 6c65 5261 6e67 654c 6973 7428   BibleRangeList(
-000110e0: 290a 2020 2020 2020 2020 666f 7220 7365  ).        for se
-000110f0: 6c66 5f72 616e 6765 2069 6e20 7365 6c66  lf_range in self
-00011100: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00011110: 7220 6f74 6865 725f 7261 6e67 6520 696e  r other_range in
-00011120: 206f 7468 6572 5f72 6566 3a0a 2020 2020   other_ref:.    
-00011130: 2020 2020 2020 2020 2020 2020 6974 656d              item
-00011140: 5f69 6e74 6572 7365 6374 696f 6e5f 6c69  _intersection_li
-00011150: 7374 203d 2073 656c 665f 7261 6e67 652e  st = self_range.
-00011160: 696e 7465 7273 6563 7469 6f6e 286f 7468  intersection(oth
-00011170: 6572 5f72 616e 6765 2c20 666c 6167 733d  er_range, flags=
-00011180: 666c 6167 7329 0a20 2020 2020 2020 2020  flags).         
-00011190: 2020 2020 2020 2069 6620 6c65 6e28 6974         if len(it
-000111a0: 656d 5f69 6e74 6572 7365 6374 696f 6e5f  em_intersection_
-000111b0: 6c69 7374 2920 3e20 303a 0a20 2020 2020  list) > 0:.     
-000111c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000111d0: 6577 5f6c 6973 742e 6170 7065 6e64 2869  ew_list.append(i
-000111e0: 7465 6d5f 696e 7465 7273 6563 7469 6f6e  tem_intersection
-000111f0: 5f6c 6973 745b 305d 290a 2020 2020 2020  _list[0]).      
-00011200: 2020 6e65 775f 6c69 7374 2e6d 6572 6765    new_list.merge
-00011210: 2866 6c61 6773 3d66 6c61 6773 290a 2020  (flags=flags).  
-00011220: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-00011230: 5f6c 6973 740a 0a20 2020 2064 6566 2069  _list..    def i
-00011240: 6e74 6572 7365 6374 696f 6e5f 7570 6461  ntersection_upda
-00011250: 7465 2873 656c 662c 206f 7468 6572 5f72  te(self, other_r
-00011260: 6566 3a20 2742 6962 6c65 5265 6627 2c20  ef: 'BibleRef', 
-00011270: 666c 6167 733a 2042 6962 6c65 466c 6167  flags: BibleFlag
-00011280: 203d 204e 6f6e 6529 202d 3e20 2742 6962   = None) -> 'Bib
-00011290: 6c65 5261 6e67 654c 6973 7427 3a0a 2020  leRangeList':.  
-000112a0: 2020 2020 2020 2727 2755 7064 6174 6573        '''Updates
-000112b0: 2074 6869 7320 6c69 7374 2074 6f20 6265   this list to be
-000112c0: 2074 6865 2069 6e74 6572 7365 6374 696f   the intersectio
-000112d0: 6e20 6f66 2069 7473 2065 7869 7374 696e  n of its existin
-000112e0: 6720 656c 656d 656e 7473 2061 6e64 2060  g elements and `
-000112f0: 6f74 6865 725f 7265 6660 2c20 7468 656e  other_ref`, then
-00011300: 2063 6f6e 736f 6c69 6461 7465 730a 2020   consolidates.  
-00011310: 2020 2020 2020 7468 6973 206c 6973 742e        this list.
-00011320: 0a0a 2020 2020 2020 2020 5573 696e 6720  ..        Using 
-00011330: 7468 6520 6026 3d60 206f 7065 7261 746f  the `&=` operato
-00011340: 7220 6973 2065 7175 6976 616c 656e 7420  r is equivalent 
-00011350: 746f 2063 616c 6c69 6e67 2060 696e 7465  to calling `inte
-00011360: 7273 6563 7469 6f6e 5f75 7064 6174 6528  rsection_update(
-00011370: 2960 2077 6974 6820 6066 6c61 6773 203d  )` with `flags =
-00011380: 204e 6f6e 6560 2e0a 2020 2020 2020 2020   None`..        
-00011390: 2727 270a 2020 2020 2020 2020 696e 7465  '''.        inte
-000113a0: 7273 6563 7469 6f6e 5f6c 6973 7420 3d20  rsection_list = 
-000113b0: 7365 6c66 2e69 6e74 6572 7365 6374 696f  self.intersectio
-000113c0: 6e28 6f74 6865 725f 7265 662c 2066 6c61  n(other_ref, fla
-000113d0: 6773 3d66 6c61 6773 290a 2020 2020 2020  gs=flags).      
-000113e0: 2020 7365 6c66 2e63 6c65 6172 2829 0a20    self.clear(). 
-000113f0: 2020 2020 2020 2073 656c 662e 6578 7465         self.exte
-00011400: 6e64 2869 6e74 6572 7365 6374 696f 6e5f  nd(intersection_
-00011410: 6c69 7374 290a 0a20 2020 2064 6566 2064  list)..    def d
-00011420: 6966 6665 7265 6e63 6528 7365 6c66 2c20  ifference(self, 
-00011430: 6f74 6865 725f 7265 663a 2027 4269 626c  other_ref: 'Bibl
-00011440: 6552 6566 272c 2066 6c61 6773 3a20 4269  eRef', flags: Bi
-00011450: 626c 6546 6c61 6720 3d20 4e6f 6e65 2920  bleFlag = None) 
-00011460: 2d3e 2027 4269 626c 6552 616e 6765 4c69  -> 'BibleRangeLi
-00011470: 7374 273a 0a20 2020 2020 2020 2027 2727  st':.        '''
-00011480: 5265 7475 726e 7320 6120 6e65 7720 6042  Returns a new `B
-00011490: 6962 6c65 5261 6e67 654c 6973 7460 206f  ibleRangeList` o
-000114a0: 6620 7665 7273 6573 2074 6861 7420 6172  f verses that ar
-000114b0: 6520 696e 2074 6869 7320 6042 6962 6c65  e in this `Bible
-000114c0: 5261 6e67 654c 6973 7460 2c20 6275 7420  RangeList`, but 
-000114d0: 6e6f 7420 696e 2060 6f74 6865 725f 7265  not in `other_re
-000114e0: 6660 2e0a 0a20 2020 2020 2020 2055 7369  f`...        Usi
-000114f0: 6e67 2074 6865 2060 2d60 206f 7065 7261  ng the `-` opera
-00011500: 746f 7220 6973 2065 7175 6976 616c 656e  tor is equivalen
-00011510: 7420 746f 2063 616c 6c69 6e67 2060 6469  t to calling `di
-00011520: 6666 6572 656e 6365 2829 6020 7769 7468  fference()` with
-00011530: 2060 666c 6167 7320 3d20 4e6f 6e65 602e   `flags = None`.
-00011540: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00011550: 2020 2020 206e 6577 5f6c 6973 7420 3d20       new_list = 
-00011560: 4269 626c 6552 616e 6765 4c69 7374 2873  BibleRangeList(s
-00011570: 656c 6629 0a20 2020 2020 2020 206e 6577  elf).        new
-00011580: 5f6c 6973 742e 6469 6666 6572 656e 6365  _list.difference
-00011590: 5f75 7064 6174 6528 6f74 6865 725f 7265  _update(other_re
-000115a0: 662c 2066 6c61 6773 3d66 6c61 6773 290a  f, flags=flags).
-000115b0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-000115c0: 6577 5f6c 6973 740a 0a20 2020 2064 6566  ew_list..    def
-000115d0: 2064 6966 6665 7265 6e63 655f 7570 6461   difference_upda
-000115e0: 7465 2873 656c 662c 206f 7468 6572 5f72  te(self, other_r
-000115f0: 6566 3a20 2742 6962 6c65 5265 6627 2c20  ef: 'BibleRef', 
-00011600: 666c 6167 733a 2042 6962 6c65 466c 6167  flags: BibleFlag
-00011610: 203d 204e 6f6e 6529 202d 3e20 2742 6962   = None) -> 'Bib
-00011620: 6c65 5261 6e67 654c 6973 7427 3a0a 2020  leRangeList':.  
-00011630: 2020 2020 2020 2727 2755 7064 6174 6573        '''Updates
-00011640: 2074 6869 7320 6c69 7374 2074 6f20 6265   this list to be
-00011650: 2074 6865 2064 6966 6665 7265 6e63 6520   the difference 
-00011660: 6f66 2069 7473 2065 7869 7374 696e 6720  of its existing 
-00011670: 656c 656d 656e 7473 2061 6e64 2060 6f74  elements and `ot
-00011680: 6865 725f 7265 6660 2c20 7468 656e 2063  her_ref`, then c
-00011690: 6f6e 736f 6c69 6461 7465 730a 2020 2020  onsolidates.    
-000116a0: 2020 2020 7468 6973 206c 6973 742e 0a0a      this list...
-000116b0: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
-000116c0: 6520 602d 3d60 206f 7065 7261 746f 7220  e `-=` operator 
-000116d0: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
-000116e0: 2063 616c 6c69 6e67 2060 6469 6666 6572   calling `differ
-000116f0: 656e 6365 5f75 7064 6174 6528 2960 2077  ence_update()` w
-00011700: 6974 6820 6066 6c61 6773 203d 204e 6f6e  ith `flags = Non
-00011710: 6560 2e0a 2020 2020 2020 2020 2727 270a  e`..        '''.
-00011720: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00011730: 7461 6e63 6528 6f74 6865 725f 7265 662c  tance(other_ref,
-00011740: 2042 6962 6c65 5665 7273 6529 3a0a 2020   BibleVerse):.  
-00011750: 2020 2020 2020 2020 2020 2320 436f 6e76            # Conv
-00011760: 6572 7420 746f 2042 6962 6c65 5261 6e67  ert to BibleRang
-00011770: 654c 6973 7420 2861 6e64 2077 6520 646f  eList (and we do
-00011780: 6e27 7420 656e 666f 7263 6520 6578 6973  n't enforce exis
-00011790: 7469 6e67 2066 6c61 6773 2066 6f72 2063  ting flags for c
-000117a0: 6f6e 7665 7273 696f 6e73 290a 2020 2020  onversions).    
-000117b0: 2020 2020 2020 2020 6f74 6865 725f 7265          other_re
-000117c0: 6620 3d20 4269 626c 6552 616e 6765 4c69  f = BibleRangeLi
-000117d0: 7374 285b 4269 626c 6552 616e 6765 2873  st([BibleRange(s
-000117e0: 7461 7274 3d6f 7468 6572 5f72 6566 2c20  tart=other_ref, 
-000117f0: 656e 643d 6f74 6865 725f 7265 662c 2066  end=other_ref, f
-00011800: 6c61 6773 3d42 6962 6c65 466c 6167 2e41  lags=BibleFlag.A
-00011810: 4c4c 295d 290a 2020 2020 2020 2020 656c  LL)]).        el
-00011820: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-00011830: 6865 725f 7265 662c 2042 6962 6c65 5261  her_ref, BibleRa
-00011840: 6e67 6529 3a0a 2020 2020 2020 2020 2020  nge):.          
-00011850: 2020 6f74 6865 725f 7265 6620 3d20 4269    other_ref = Bi
-00011860: 626c 6552 616e 6765 4c69 7374 285b 6f74  bleRangeList([ot
-00011870: 6865 725f 7265 665d 290a 2020 2020 2020  her_ref]).      
-00011880: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00011890: 6e63 6528 6f74 6865 725f 7265 662c 2042  nce(other_ref, B
-000118a0: 6962 6c65 5261 6e67 654c 6973 7429 3a0a  ibleRangeList):.
-000118b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000118c0: 6520 5661 6c75 6545 7272 6f72 2866 227b  e ValueError(f"{
-000118d0: 6f74 6865 725f 7265 667d 2069 7320 6e6f  other_ref} is no
-000118e0: 7420 6120 7661 6c69 6420 4269 626c 6552  t a valid BibleR
-000118f0: 6566 2229 2020 2020 2020 2020 0a0a 2020  ef")        ..  
-00011900: 2020 2020 2020 2320 4561 6368 2042 6962        # Each Bib
-00011910: 6c65 5265 664c 6973 7420 6973 2065 6666  leRefList is eff
-00011920: 6563 7469 7665 6c79 2061 2075 6e69 6f6e  ectively a union
-00011930: 206f 6620 6974 7320 656c 656d 656e 7473   of its elements
-00011940: 2e0a 2020 2020 2020 2020 2320 4b65 7920  ..        # Key 
-00011950: 7365 7420 7468 656f 7279 2069 6465 6e74  set theory ident
-00011960: 6974 793a 2028 7768 6572 6520 5c20 6d65  ity: (where \ me
-00011970: 616e 7320 7365 7420 6469 6666 6572 656e  ans set differen
-00011980: 6365 2c20 736f 2041 205c 2042 203d 2041  ce, so A \ B = A
-00011990: 202d 2042 290a 2020 2020 2020 2020 2320   - B).        # 
-000119a0: 2020 2841 3020 e288 aa20 4131 2920 5c20    (A0 ... A1) \ 
-000119b0: 2842 3020 e288 aa20 4231 2920 3d20 5b28  (B0 ... B1) = [(
-000119c0: 4130 205c 2042 3029 205c 2042 315d 20e2  A0 \ B0) \ B1] .
-000119d0: 88aa 205b 2841 3120 5c20 4230 2920 5c20  .. [(A1 \ B0) \ 
-000119e0: 4231 5d0a 2020 2020 2020 2020 2320 536f  B1].        # So
-000119f0: 2074 6865 2064 6966 6665 7265 6e63 6520   the difference 
-00011a00: 6f66 2074 776f 2042 6962 6c65 5265 664c  of two BibleRefL
-00011a10: 6973 7473 2069 7320 6120 6e65 7720 6c69  ists is a new li
-00011a20: 7374 206f 6620 7468 6520 6375 6d75 6c61  st of the cumula
-00011a30: 7469 7665 2064 6966 6665 7265 6e63 6520  tive difference 
-00011a40: 6f66 2065 6163 680a 2020 2020 2020 2020  of each.        
-00011a50: 2320 6974 656d 2069 6e20 7468 6520 7365  # item in the se
-00011a60: 636f 6e64 206c 6973 7420 6672 6f6d 2065  cond list from e
-00011a70: 6163 6820 6974 656d 2069 6e20 7468 6520  ach item in the 
-00011a80: 6669 7273 7420 6c69 7374 2e0a 2020 2020  first list..    
-00011a90: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-00011aa0: 5768 6174 2773 2061 206c 6974 746c 6520  What's a little 
-00011ab0: 6469 6666 6963 756c 7420 6973 2074 6861  difficult is tha
-00011ac0: 7420 7468 6520 6469 6666 6572 656e 6365  t the difference
-00011ad0: 206f 6620 7477 6f20 6974 656d 7320 6361   of two items ca
-00011ae0: 6e20 6974 7365 6c66 2072 6573 756c 7420  n itself result 
-00011af0: 696e 2061 206c 6973 740a 2020 2020 2020  in a list.      
-00011b00: 2020 2320 286f 6620 7477 6f20 6974 656d    # (of two item
-00011b10: 7329 2e20 4173 2061 2072 6573 756c 742c  s). As a result,
-00011b20: 2069 7427 7320 6561 7369 6573 7420 746f   it's easiest to
-00011b30: 2063 616c 6375 6c61 7465 2074 6865 2064   calculate the d
-00011b40: 6966 6665 7265 6e63 6520 696e 2d70 6c61  ifference in-pla
-00011b50: 6365 2e0a 2020 2020 2020 2020 230a 2020  ce..        #.  
-00011b60: 2020 2020 2020 2320 496e 2d70 6c61 6365        # In-place
-00011b70: 2073 6574 2064 6966 6665 7265 6e63 6520   set difference 
-00011b80: 7265 7175 6972 6573 2075 7320 746f 206d  requires us to m
-00011b90: 616b 6520 6d61 6e79 2075 7064 6174 6573  ake many updates
-00011ba0: 2074 6f20 7468 6973 206c 6973 7420 6475   to this list du
-00011bb0: 7269 6e67 2069 7465 7261 7469 6f6e 2c0a  ring iteration,.
-00011bc0: 2020 2020 2020 2020 2320 6265 796f 6e64          # beyond
-00011bd0: 2077 6861 7420 6120 666f 722d 6c6f 6f70   what a for-loop
-00011be0: 2063 616e 2063 6f70 6520 7769 7468 2e20   can cope with. 
-00011bf0: 5468 6572 6566 6f72 6520 7765 2075 7365  Therefore we use
-00011c00: 2061 2077 6869 6c65 206c 6f6f 702e 0a20   a while loop.. 
-00011c10: 2020 2020 2020 2073 656c 665f 6e6f 6465         self_node
-00011c20: 203d 2073 656c 662e 5f66 6972 7374 0a20   = self._first. 
-00011c30: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
-00011c40: 665f 6e6f 6465 2069 7320 6e6f 7420 4e6f  f_node is not No
-00011c50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011c60: 666f 7220 6f74 6865 725f 7261 6e67 6520  for other_range 
-00011c70: 696e 206f 7468 6572 5f72 6566 3a0a 2020  in other_ref:.  
-00011c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011c90: 6c66 5f72 616e 6765 203d 2073 656c 665f  lf_range = self_
-00011ca0: 6e6f 6465 2e76 616c 7565 0a20 2020 2020  node.value.     
-00011cb0: 2020 2020 2020 2020 2020 2069 7465 6d5f             item_
-00011cc0: 6469 6666 6572 656e 6365 5f6c 6973 7420  difference_list 
-00011cd0: 3d20 7365 6c66 5f72 616e 6765 2e64 6966  = self_range.dif
-00011ce0: 6665 7265 6e63 6528 6f74 6865 725f 7261  ference(other_ra
-00011cf0: 6e67 652c 2066 6c61 6773 3d66 6c61 6773  nge, flags=flags
-00011d00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011d10: 2020 6966 206c 656e 2869 7465 6d5f 6469    if len(item_di
-00011d20: 6666 6572 656e 6365 5f6c 6973 7429 203e  fference_list) >
-00011d30: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00011d40: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
-00011d50: 7465 6d5f 6469 6666 6572 656e 6365 5f6c  tem_difference_l
-00011d60: 6973 7420 6e6f 7720 7368 6f75 6c64 2072  ist now should r
-00011d70: 6570 6c61 6365 2073 656c 665f 6e6f 6465  eplace self_node
-00011d80: 2c20 616e 6420 7365 6c66 5f6e 6f64 650a  , and self_node.
+0000e650: 6966 206c 656e 2869 7465 6d5f 696e 7465  if len(item_inte
+0000e660: 7273 6563 7469 6f6e 5f6c 6973 7429 203e  rsection_list) >
+0000e670: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000e680: 2020 2020 2020 2020 6e65 775f 6c69 7374          new_list
+0000e690: 2e61 7070 656e 6428 6974 656d 5f69 6e74  .append(item_int
+0000e6a0: 6572 7365 6374 696f 6e5f 6c69 7374 5b30  ersection_list[0
+0000e6b0: 5d29 0a20 2020 2020 2020 206e 6577 5f6c  ]).        new_l
+0000e6c0: 6973 742e 636f 6e73 6f6c 6964 6174 6528  ist.consolidate(
+0000e6d0: 666c 6167 733d 666c 6167 7329 0a20 2020  flags=flags).   
+0000e6e0: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
+0000e6f0: 6c69 7374 0a0a 2020 2020 6465 6620 696e  list..    def in
+0000e700: 7465 7273 6563 7469 6f6e 5f75 7064 6174  tersection_updat
+0000e710: 6528 7365 6c66 2c20 6f74 6865 725f 7265  e(self, other_re
+0000e720: 663a 2027 4269 626c 6552 6566 272c 2066  f: 'BibleRef', f
+0000e730: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+0000e740: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
+0000e750: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
+0000e760: 2020 2020 2027 2727 5570 6461 7465 7320       '''Updates 
+0000e770: 7468 6973 206c 6973 7420 746f 2062 6520  this list to be 
+0000e780: 7468 6520 696e 7465 7273 6563 7469 6f6e  the intersection
+0000e790: 206f 6620 6974 7320 6578 6973 7469 6e67   of its existing
+0000e7a0: 2065 6c65 6d65 6e74 7320 616e 6420 606f   elements and `o
+0000e7b0: 7468 6572 5f72 6566 602c 2074 6865 6e20  ther_ref`, then 
+0000e7c0: 636f 6e73 6f6c 6964 6174 6573 0a20 2020  consolidates.   
+0000e7d0: 2020 2020 2074 6869 7320 6c69 7374 2e0a       this list..
+0000e7e0: 0a20 2020 2020 2020 2055 7369 6e67 2074  .        Using t
+0000e7f0: 6865 2060 263d 6020 6f70 6572 6174 6f72  he `&=` operator
+0000e800: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
+0000e810: 6f20 6361 6c6c 696e 6720 6069 6e74 6572  o calling `inter
+0000e820: 7365 6374 696f 6e5f 7570 6461 7465 2829  section_update()
+0000e830: 6020 7769 7468 2060 666c 6167 7320 3d20  ` with `flags = 
+0000e840: 4e6f 6e65 602e 0a20 2020 2020 2020 2027  None`..        '
+0000e850: 2727 0a20 2020 2020 2020 2069 6e74 6572  ''.        inter
+0000e860: 7365 6374 696f 6e5f 6c69 7374 203d 2073  section_list = s
+0000e870: 656c 662e 696e 7465 7273 6563 7469 6f6e  elf.intersection
+0000e880: 286f 7468 6572 5f72 6566 2c20 666c 6167  (other_ref, flag
+0000e890: 733d 666c 6167 7329 0a20 2020 2020 2020  s=flags).       
+0000e8a0: 2073 656c 662e 636c 6561 7228 290a 2020   self.clear().  
+0000e8b0: 2020 2020 2020 7365 6c66 2e65 7874 656e        self.exten
+0000e8c0: 6428 696e 7465 7273 6563 7469 6f6e 5f6c  d(intersection_l
+0000e8d0: 6973 7429 0a0a 2020 2020 6465 6620 6469  ist)..    def di
+0000e8e0: 6666 6572 656e 6365 2873 656c 662c 206f  fference(self, o
+0000e8f0: 7468 6572 5f72 6566 3a20 2742 6962 6c65  ther_ref: 'Bible
+0000e900: 5265 6627 2c20 666c 6167 733a 2042 6962  Ref', flags: Bib
+0000e910: 6c65 466c 6167 203d 204e 6f6e 6529 202d  leFlag = None) -
+0000e920: 3e20 2742 6962 6c65 5261 6e67 654c 6973  > 'BibleRangeLis
+0000e930: 7427 3a0a 2020 2020 2020 2020 2727 2752  t':.        '''R
+0000e940: 6574 7572 6e73 2061 206e 6577 2060 4269  eturns a new `Bi
+0000e950: 626c 6552 616e 6765 4c69 7374 6020 6f66  bleRangeList` of
+0000e960: 2076 6572 7365 7320 7468 6174 2061 7265   verses that are
+0000e970: 2069 6e20 7468 6973 2060 4269 626c 6552   in this `BibleR
+0000e980: 616e 6765 4c69 7374 602c 2062 7574 206e  angeList`, but n
+0000e990: 6f74 2069 6e20 606f 7468 6572 5f72 6566  ot in `other_ref
+0000e9a0: 602e 0a0a 2020 2020 2020 2020 5573 696e  `...        Usin
+0000e9b0: 6720 7468 6520 602d 6020 6f70 6572 6174  g the `-` operat
+0000e9c0: 6f72 2069 7320 6571 7569 7661 6c65 6e74  or is equivalent
+0000e9d0: 2074 6f20 6361 6c6c 696e 6720 6064 6966   to calling `dif
+0000e9e0: 6665 7265 6e63 6528 2960 2077 6974 6820  ference()` with 
+0000e9f0: 6066 6c61 6773 203d 204e 6f6e 6560 2e0a  `flags = None`..
+0000ea00: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000ea10: 2020 2020 6e65 775f 6c69 7374 203d 2042      new_list = B
+0000ea20: 6962 6c65 5261 6e67 654c 6973 7428 7365  ibleRangeList(se
+0000ea30: 6c66 290a 2020 2020 2020 2020 6e65 775f  lf).        new_
+0000ea40: 6c69 7374 2e64 6966 6665 7265 6e63 655f  list.difference_
+0000ea50: 7570 6461 7465 286f 7468 6572 5f72 6566  update(other_ref
+0000ea60: 2c20 666c 6167 733d 666c 6167 7329 0a20  , flags=flags). 
+0000ea70: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
+0000ea80: 775f 6c69 7374 0a0a 2020 2020 6465 6620  w_list..    def 
+0000ea90: 6469 6666 6572 656e 6365 5f75 7064 6174  difference_updat
+0000eaa0: 6528 7365 6c66 2c20 6f74 6865 725f 7265  e(self, other_re
+0000eab0: 663a 2027 4269 626c 6552 6566 272c 2066  f: 'BibleRef', f
+0000eac0: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+0000ead0: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
+0000eae0: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
+0000eaf0: 2020 2020 2027 2727 5570 6461 7465 7320       '''Updates 
+0000eb00: 7468 6973 206c 6973 7420 746f 2062 6520  this list to be 
+0000eb10: 7468 6520 6469 6666 6572 656e 6365 206f  the difference o
+0000eb20: 6620 6974 7320 6578 6973 7469 6e67 2065  f its existing e
+0000eb30: 6c65 6d65 6e74 7320 616e 6420 606f 7468  lements and `oth
+0000eb40: 6572 5f72 6566 602c 2074 6865 6e20 636f  er_ref`, then co
+0000eb50: 6e73 6f6c 6964 6174 6573 0a20 2020 2020  nsolidates.     
+0000eb60: 2020 2074 6869 7320 6c69 7374 2e0a 0a20     this list... 
+0000eb70: 2020 2020 2020 2055 7369 6e67 2074 6865         Using the
+0000eb80: 2060 2d3d 6020 6f70 6572 6174 6f72 2069   `-=` operator i
+0000eb90: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
+0000eba0: 6361 6c6c 696e 6720 6064 6966 6665 7265  calling `differe
+0000ebb0: 6e63 655f 7570 6461 7465 2829 6020 7769  nce_update()` wi
+0000ebc0: 7468 2060 666c 6167 7320 3d20 4e6f 6e65  th `flags = None
+0000ebd0: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
+0000ebe0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000ebf0: 616e 6365 286f 7468 6572 5f72 6566 2c20  ance(other_ref, 
+0000ec00: 4269 626c 6556 6572 7365 293a 0a20 2020  BibleVerse):.   
+0000ec10: 2020 2020 2020 2020 2023 2043 6f6e 7665           # Conve
+0000ec20: 7274 2074 6f20 4269 626c 6552 616e 6765  rt to BibleRange
+0000ec30: 4c69 7374 2028 616e 6420 7765 2064 6f6e  List (and we don
+0000ec40: 2774 2065 6e66 6f72 6365 2065 7869 7374  't enforce exist
+0000ec50: 696e 6720 666c 6167 7320 666f 7220 636f  ing flags for co
+0000ec60: 6e76 6572 7369 6f6e 7329 0a20 2020 2020  nversions).     
+0000ec70: 2020 2020 2020 206f 7468 6572 5f72 6566         other_ref
+0000ec80: 203d 2042 6962 6c65 5261 6e67 654c 6973   = BibleRangeLis
+0000ec90: 7428 5b42 6962 6c65 5261 6e67 6528 7374  t([BibleRange(st
+0000eca0: 6172 743d 6f74 6865 725f 7265 662c 2065  art=other_ref, e
+0000ecb0: 6e64 3d6f 7468 6572 5f72 6566 2c20 666c  nd=other_ref, fl
+0000ecc0: 6167 733d 4269 626c 6546 6c61 672e 414c  ags=BibleFlag.AL
+0000ecd0: 4c29 5d29 0a20 2020 2020 2020 2065 6c69  L)]).        eli
+0000ece0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+0000ecf0: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
+0000ed00: 6765 293a 0a20 2020 2020 2020 2020 2020  ge):.           
+0000ed10: 206f 7468 6572 5f72 6566 203d 2042 6962   other_ref = Bib
+0000ed20: 6c65 5261 6e67 654c 6973 7428 5b6f 7468  leRangeList([oth
+0000ed30: 6572 5f72 6566 5d29 0a20 2020 2020 2020  er_ref]).       
+0000ed40: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000ed50: 6365 286f 7468 6572 5f72 6566 2c20 4269  ce(other_ref, Bi
+0000ed60: 626c 6552 616e 6765 4c69 7374 293a 0a20  bleRangeList):. 
+0000ed70: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000ed80: 2056 616c 7565 4572 726f 7228 6622 7b6f   ValueError(f"{o
+0000ed90: 7468 6572 5f72 6566 7d20 6973 206e 6f74  ther_ref} is not
+0000eda0: 2061 2076 616c 6964 2042 6962 6c65 5265   a valid BibleRe
+0000edb0: 6622 2920 2020 2020 2020 200a 0a20 2020  f")        ..   
+0000edc0: 2020 2020 2023 2045 6163 6820 4269 626c       # Each Bibl
+0000edd0: 6552 6566 4c69 7374 2069 7320 6566 6665  eRefList is effe
+0000ede0: 6374 6976 656c 7920 6120 756e 696f 6e20  ctively a union 
+0000edf0: 6f66 2069 7473 2065 6c65 6d65 6e74 732e  of its elements.
+0000ee00: 0a20 2020 2020 2020 2023 204b 6579 2073  .        # Key s
+0000ee10: 6574 2074 6865 6f72 7920 6964 656e 7469  et theory identi
+0000ee20: 7479 3a20 2877 6865 7265 205c 206d 6561  ty: (where \ mea
+0000ee30: 6e73 2073 6574 2064 6966 6665 7265 6e63  ns set differenc
+0000ee40: 652c 2073 6f20 4120 5c20 4220 3d20 4120  e, so A \ B = A 
+0000ee50: 2d20 4229 0a20 2020 2020 2020 2023 2020  - B).        #  
+0000ee60: 2028 4130 20e2 88aa 2041 3129 205c 2028   (A0 ... A1) \ (
+0000ee70: 4230 20e2 88aa 2042 3129 203d 205b 2841  B0 ... B1) = [(A
+0000ee80: 3020 5c20 4230 2920 5c20 4231 5d20 e288  0 \ B0) \ B1] ..
+0000ee90: aa20 5b28 4131 205c 2042 3029 205c 2042  . [(A1 \ B0) \ B
+0000eea0: 315d 0a20 2020 2020 2020 2023 2053 6f20  1].        # So 
+0000eeb0: 7468 6520 6469 6666 6572 656e 6365 206f  the difference o
+0000eec0: 6620 7477 6f20 4269 626c 6552 6566 4c69  f two BibleRefLi
+0000eed0: 7374 7320 6973 2061 206e 6577 206c 6973  sts is a new lis
+0000eee0: 7420 6f66 2074 6865 2063 756d 756c 6174  t of the cumulat
+0000eef0: 6976 6520 6469 6666 6572 656e 6365 206f  ive difference o
+0000ef00: 6620 6561 6368 0a20 2020 2020 2020 2023  f each.        #
+0000ef10: 2069 7465 6d20 696e 2074 6865 2073 6563   item in the sec
+0000ef20: 6f6e 6420 6c69 7374 2066 726f 6d20 6561  ond list from ea
+0000ef30: 6368 2069 7465 6d20 696e 2074 6865 2066  ch item in the f
+0000ef40: 6972 7374 206c 6973 742e 0a20 2020 2020  irst list..     
+0000ef50: 2020 2023 0a20 2020 2020 2020 2023 2057     #.        # W
+0000ef60: 6861 7427 7320 6120 6c69 7474 6c65 2064  hat's a little d
+0000ef70: 6966 6669 6375 6c74 2069 7320 7468 6174  ifficult is that
+0000ef80: 2074 6865 2064 6966 6665 7265 6e63 6520   the difference 
+0000ef90: 6f66 2074 776f 2069 7465 6d73 2063 616e  of two items can
+0000efa0: 2069 7473 656c 6620 7265 7375 6c74 2069   itself result i
+0000efb0: 6e20 6120 6c69 7374 0a20 2020 2020 2020  n a list.       
+0000efc0: 2023 2028 6f66 2074 776f 2069 7465 6d73   # (of two items
+0000efd0: 292e 2041 7320 6120 7265 7375 6c74 2c20  ). As a result, 
+0000efe0: 6974 2773 2065 6173 6965 7374 2074 6f20  it's easiest to 
+0000eff0: 6361 6c63 756c 6174 6520 7468 6520 6469  calculate the di
+0000f000: 6666 6572 656e 6365 2069 6e2d 706c 6163  fference in-plac
+0000f010: 652e 0a20 2020 2020 2020 2023 0a20 2020  e..        #.   
+0000f020: 2020 2020 2023 2049 6e2d 706c 6163 6520       # In-place 
+0000f030: 7365 7420 6469 6666 6572 656e 6365 2072  set difference r
+0000f040: 6571 7569 7265 7320 7573 2074 6f20 6d61  equires us to ma
+0000f050: 6b65 206d 616e 7920 7570 6461 7465 7320  ke many updates 
+0000f060: 746f 2074 6869 7320 6c69 7374 2064 7572  to this list dur
+0000f070: 696e 6720 6974 6572 6174 696f 6e2c 0a20  ing iteration,. 
+0000f080: 2020 2020 2020 2023 2062 6579 6f6e 6420         # beyond 
+0000f090: 7768 6174 2061 2066 6f72 2d6c 6f6f 7020  what a for-loop 
+0000f0a0: 6361 6e20 636f 7065 2077 6974 682e 2054  can cope with. T
+0000f0b0: 6865 7265 666f 7265 2077 6520 7573 6520  herefore we use 
+0000f0c0: 6120 7768 696c 6520 6c6f 6f70 2e0a 2020  a while loop..  
+0000f0d0: 2020 2020 2020 7365 6c66 5f6e 6f64 6520        self_node 
+0000f0e0: 3d20 7365 6c66 2e5f 6669 7273 740a 2020  = self._first.  
+0000f0f0: 2020 2020 2020 7768 696c 6520 7365 6c66        while self
+0000f100: 5f6e 6f64 6520 6973 206e 6f74 204e 6f6e  _node is not Non
+0000f110: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0000f120: 6f72 206f 7468 6572 5f72 616e 6765 2069  or other_range i
+0000f130: 6e20 6f74 6865 725f 7265 663a 0a20 2020  n other_ref:.   
+0000f140: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f150: 665f 7261 6e67 6520 3d20 7365 6c66 5f6e  f_range = self_n
+0000f160: 6f64 652e 7661 6c75 650a 2020 2020 2020  ode.value.      
+0000f170: 2020 2020 2020 2020 2020 6974 656d 5f64            item_d
+0000f180: 6966 6665 7265 6e63 655f 6c69 7374 203d  ifference_list =
+0000f190: 2073 656c 665f 7261 6e67 652e 6469 6666   self_range.diff
+0000f1a0: 6572 656e 6365 286f 7468 6572 5f72 616e  erence(other_ran
+0000f1b0: 6765 2c20 666c 6167 733d 666c 6167 7329  ge, flags=flags)
+0000f1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f1d0: 2069 6620 6c65 6e28 6974 656d 5f64 6966   if len(item_dif
+0000f1e0: 6665 7265 6e63 655f 6c69 7374 2920 3e20  ference_list) > 
+0000f1f0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000f200: 2020 2020 2020 2023 2054 6869 7320 6974         # This it
+0000f210: 656d 5f64 6966 6665 7265 6e63 655f 6c69  em_difference_li
+0000f220: 7374 206e 6f77 2073 686f 756c 6420 7265  st now should re
+0000f230: 706c 6163 6520 7365 6c66 5f6e 6f64 652c  place self_node,
+0000f240: 2061 6e64 2073 656c 665f 6e6f 6465 0a20   and self_node. 
+0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f260: 2020 2023 2063 6861 6e67 6564 2074 6f20     # changed to 
+0000f270: 706f 696e 7420 746f 2074 6865 2066 6972  point to the fir
+0000f280: 7374 206f 6620 7468 6520 7265 7375 6c74  st of the result
+0000f290: 2069 7465 6d73 2e20 5468 6520 6561 7369   items. The easi
+0000f2a0: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
+0000f2b0: 2020 2020 2020 2020 2320 7761 7920 746f          # way to
+0000f2c0: 2064 6f20 7468 6973 2069 7320 746f 2069   do this is to i
+0000f2d0: 6e73 6572 7420 7468 6520 7265 7375 6c74  nsert the result
+0000f2e0: 2069 7465 6d73 2073 7461 7274 696e 6720   items starting 
+0000f2f0: 6672 6f6d 2074 6865 2065 6e64 3a0a 2020  from the end:.  
+0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f310: 2020 6f6c 645f 7365 6c66 5f6e 6f64 6520    old_self_node 
+0000f320: 3d20 7365 6c66 5f6e 6f64 650a 2020 2020  = self_node.    
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 666f 7220 6469 6666 6572 656e 6365 5f72  for difference_r
+0000f350: 616e 6765 2069 6e20 7265 7665 7273 6564  ange in reversed
+0000f360: 2869 7465 6d5f 6469 6666 6572 656e 6365  (item_difference
+0000f370: 5f6c 6973 7429 3a0a 2020 2020 2020 2020  _list):.        
+0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f390: 7365 6c66 2e5f 696e 7365 7274 5f62 6566  self._insert_bef
+0000f3a0: 6f72 6528 7365 6c66 5f6e 6f64 652c 2064  ore(self_node, d
+0000f3b0: 6966 6665 7265 6e63 655f 7261 6e67 6529  ifference_range)
+0000f3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f3d0: 2020 2020 2020 2020 2073 656c 665f 6e6f           self_no
+0000f3e0: 6465 203d 2073 656c 665f 6e6f 6465 2e70  de = self_node.p
+0000f3f0: 7265 760a 2020 2020 2020 2020 2020 2020  rev.            
+0000f400: 2020 2020 2020 2020 7365 6c66 2e5f 706f          self._po
+0000f410: 705f 6e6f 6465 286f 6c64 5f73 656c 665f  p_node(old_self_
+0000f420: 6e6f 6465 290a 2020 2020 2020 2020 2020  node).          
+0000f430: 2020 7365 6c66 5f6e 6f64 6520 3d20 7365    self_node = se
+0000f440: 6c66 5f6e 6f64 652e 6e65 7874 0a20 2020  lf_node.next.   
+0000f450: 2020 2020 2073 656c 662e 636f 6e73 6f6c       self.consol
+0000f460: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0000f470: 2073 796d 5f64 6966 6665 7265 6e63 6528   sym_difference(
+0000f480: 7365 6c66 2c20 6f74 6865 725f 7265 663a  self, other_ref:
+0000f490: 2027 4269 626c 6552 6566 272c 2066 6c61   'BibleRef', fla
+0000f4a0: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
+0000f4b0: 4e6f 6e65 2920 2d3e 2027 4269 626c 6552  None) -> 'BibleR
+0000f4c0: 616e 6765 4c69 7374 273a 0a20 2020 2020  angeList':.     
+0000f4d0: 2020 2027 2727 5265 7475 726e 7320 6120     '''Returns a 
+0000f4e0: 6e65 7720 6042 6962 6c65 5261 6e67 654c  new `BibleRangeL
+0000f4f0: 6973 7460 206f 6620 7665 7273 6573 2074  ist` of verses t
+0000f500: 6861 7420 6172 6520 6569 7468 6572 2069  hat are either i
+0000f510: 6e20 7468 6973 2060 4269 626c 6552 616e  n this `BibleRan
+0000f520: 6765 4c69 7374 602c 206f 7220 696e 2060  geList`, or in `
+0000f530: 6f74 6865 725f 7265 6660 2c0a 2020 2020  other_ref`,.    
+0000f540: 2020 2020 6275 7420 6e6f 7420 626f 7468      but not both
+0000f550: 2e0a 0a20 2020 2020 2020 2055 7369 6e67  ...        Using
+0000f560: 2074 6865 2060 5e60 206f 7065 7261 746f   the `^` operato
+0000f570: 7220 6973 2065 7175 6976 616c 656e 7420  r is equivalent 
+0000f580: 746f 2063 616c 6c69 6e67 2060 7379 6d5f  to calling `sym_
+0000f590: 6469 6666 6572 656e 6365 2829 6020 7769  difference()` wi
+0000f5a0: 7468 2060 666c 6167 7320 3d20 4e6f 6e65  th `flags = None
+0000f5b0: 602e 0a20 2020 2020 2020 2027 2727 0a20  `..        '''. 
+0000f5c0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000f5d0: 616e 6365 286f 7468 6572 5f72 6566 2c20  ance(other_ref, 
+0000f5e0: 4269 626c 6556 6572 7365 293a 0a20 2020  BibleVerse):.   
+0000f5f0: 2020 2020 2020 2020 2023 2043 6f6e 7665           # Conve
+0000f600: 7274 2074 6f20 4269 626c 6552 616e 6765  rt to BibleRange
+0000f610: 4c69 7374 2028 616e 6420 7765 2064 6f6e  List (and we don
+0000f620: 2774 2065 6e66 6f72 6365 2065 7869 7374  't enforce exist
+0000f630: 696e 6720 666c 6167 7320 666f 7220 636f  ing flags for co
+0000f640: 6e76 6572 7369 6f6e 7329 0a20 2020 2020  nversions).     
+0000f650: 2020 2020 2020 206f 7468 6572 5f72 6566         other_ref
+0000f660: 203d 2042 6962 6c65 5261 6e67 654c 6973   = BibleRangeLis
+0000f670: 7428 5b42 6962 6c65 5261 6e67 6528 7374  t([BibleRange(st
+0000f680: 6172 743d 6f74 6865 725f 7265 662c 2065  art=other_ref, e
+0000f690: 6e64 3d6f 7468 6572 5f72 6566 2c20 666c  nd=other_ref, fl
+0000f6a0: 6167 733d 4269 626c 6546 6c61 672e 414c  ags=BibleFlag.AL
+0000f6b0: 4c29 5d29 0a20 2020 2020 2020 2065 6c69  L)]).        eli
+0000f6c0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+0000f6d0: 6572 5f72 6566 2c20 4269 626c 6552 616e  er_ref, BibleRan
+0000f6e0: 6765 293a 0a20 2020 2020 2020 2020 2020  ge):.           
+0000f6f0: 206f 7468 6572 5f72 6566 203d 2042 6962   other_ref = Bib
+0000f700: 6c65 5261 6e67 654c 6973 7428 5b6f 7468  leRangeList([oth
+0000f710: 6572 5f72 6566 5d29 0a20 2020 2020 2020  er_ref]).       
+0000f720: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000f730: 6365 286f 7468 6572 5f72 6566 2c20 4269  ce(other_ref, Bi
+0000f740: 626c 6552 616e 6765 4c69 7374 293a 0a20  bleRangeList):. 
+0000f750: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f760: 2056 616c 7565 4572 726f 7228 6622 7b6f   ValueError(f"{o
+0000f770: 7468 6572 5f72 6566 7d20 6973 206e 6f74  ther_ref} is not
+0000f780: 2061 2076 616c 6964 2042 6962 6c65 5265   a valid BibleRe
+0000f790: 6622 2920 2020 2020 2020 200a 2020 2020  f")        .    
+0000f7a0: 2020 2020 0a20 2020 2020 2020 2075 6e69      .        uni
+0000f7b0: 6f6e 5f6c 6973 7420 3d20 7365 6c66 2e75  on_list = self.u
+0000f7c0: 6e69 6f6e 286f 7468 6572 5f72 6566 2c20  nion(other_ref, 
+0000f7d0: 666c 6167 733d 666c 6167 7329 0a20 2020  flags=flags).   
+0000f7e0: 2020 2020 2069 6e74 6572 7365 6374 696f       intersectio
+0000f7f0: 6e5f 6c69 7374 203d 2073 656c 662e 696e  n_list = self.in
+0000f800: 7465 7273 6563 7469 6f6e 286f 7468 6572  tersection(other
+0000f810: 5f72 6566 2c20 666c 6167 733d 666c 6167  _ref, flags=flag
+0000f820: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+0000f830: 6e20 756e 696f 6e5f 6c69 7374 2e64 6966  n union_list.dif
+0000f840: 6665 7265 6e63 6528 696e 7465 7273 6563  ference(intersec
+0000f850: 7469 6f6e 5f6c 6973 742c 2066 6c61 6773  tion_list, flags
+0000f860: 3d66 6c61 6773 290a 0a20 2020 2064 6566  =flags)..    def
+0000f870: 2073 796d 5f64 6966 6665 7265 6e63 655f   sym_difference_
+0000f880: 7570 6461 7465 2873 656c 662c 206f 7468  update(self, oth
+0000f890: 6572 5f72 6566 3a20 2742 6962 6c65 5265  er_ref: 'BibleRe
+0000f8a0: 6627 2c20 666c 6167 733a 2042 6962 6c65  f', flags: Bible
+0000f8b0: 466c 6167 203d 204e 6f6e 6529 202d 3e20  Flag = None) -> 
+0000f8c0: 2742 6962 6c65 5261 6e67 654c 6973 7427  'BibleRangeList'
+0000f8d0: 3a0a 2020 2020 2020 2020 2727 2755 7064  :.        '''Upd
+0000f8e0: 6174 6573 2074 6869 7320 6c69 7374 2074  ates this list t
+0000f8f0: 6f20 6265 2074 6865 2073 796d 6d65 7472  o be the symmetr
+0000f900: 6963 2064 6966 6665 7265 6e63 6520 6f66  ic difference of
+0000f910: 2069 7473 2065 7869 7374 696e 6720 656c   its existing el
+0000f920: 656d 656e 7473 2061 6e64 2060 6f74 6865  ements and `othe
+0000f930: 725f 7265 6660 2c20 7468 656e 0a20 2020  r_ref`, then.   
+0000f940: 2020 2020 2063 6f6e 736f 6c69 6461 7465       consolidate
+0000f950: 7320 7468 6973 206c 6973 742e 0a0a 2020  s this list...  
+0000f960: 2020 2020 2020 5573 696e 6720 7468 6520        Using the 
+0000f970: 605e 3d60 206f 7065 7261 746f 7220 6973  `^=` operator is
+0000f980: 2065 7175 6976 616c 656e 7420 746f 2063   equivalent to c
+0000f990: 616c 6c69 6e67 2060 7379 6d5f 6469 6666  alling `sym_diff
+0000f9a0: 6572 656e 6365 5f75 7064 6174 6528 2960  erence_update()`
+0000f9b0: 2077 6974 6820 6066 6c61 6773 203d 204e   with `flags = N
+0000f9c0: 6f6e 6560 2e0a 2020 2020 2020 2020 2727  one`..        ''
+0000f9d0: 270a 2020 2020 2020 2020 7379 6d5f 6469  '.        sym_di
+0000f9e0: 6666 6572 656e 6365 5f6c 6973 7420 3d20  fference_list = 
+0000f9f0: 7365 6c66 2e73 796d 5f64 6966 6665 7265  self.sym_differe
+0000fa00: 6e63 6528 6f74 6865 725f 7265 662c 2066  nce(other_ref, f
+0000fa10: 6c61 6773 3d66 6c61 6773 290a 2020 2020  lags=flags).    
+0000fa20: 2020 2020 7365 6c66 2e63 6c65 6172 2829      self.clear()
+0000fa30: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
+0000fa40: 7465 6e64 2873 796d 5f64 6966 6665 7265  tend(sym_differe
+0000fa50: 6e63 655f 6c69 7374 290a 0a20 2020 2064  nce_list)..    d
+0000fa60: 6566 205f 5f63 6f6e 7461 696e 735f 5f28  ef __contains__(
+0000fa70: 7365 6c66 2c20 6269 626c 655f 7265 6629  self, bible_ref)
+0000fa80: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000fa90: 2020 2727 2752 6574 7572 6e73 2054 7275    '''Returns Tru
+0000faa0: 6520 6966 2069 7465 6d20 6973 2061 2042  e if item is a B
+0000fab0: 6962 6c65 5265 6620 7468 6174 2066 616c  ibleRef that fal
+0000fac0: 6c73 2077 6974 6869 6e20 7468 6973 2072  ls within this r
+0000fad0: 616e 6765 2c20 6f74 6865 7277 6973 6520  ange, otherwise 
+0000fae0: 4661 6c73 652e 0a20 2020 2020 2020 2027  False..        '
+0000faf0: 2727 0a20 2020 2020 2020 2072 6574 7572  ''.        retur
+0000fb00: 6e20 7365 6c66 2e63 6f6e 7461 696e 7328  n self.contains(
+0000fb10: 6269 626c 655f 7265 6629 0a0a 2020 2020  bible_ref)..    
+0000fb20: 6465 6620 5f5f 6f72 5f5f 2873 656c 662c  def __or__(self,
+0000fb30: 206f 7468 6572 5f72 6566 3a20 2742 6962   other_ref: 'Bib
+0000fb40: 6c65 5265 6627 2920 2d3e 2027 4269 626c  leRef') -> 'Bibl
+0000fb50: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
+0000fb60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000fb70: 2e75 6e69 6f6e 286f 7468 6572 5f72 6566  .union(other_ref
+0000fb80: 290a 2020 2020 0a20 2020 2064 6566 205f  ).    .    def _
+0000fb90: 5f61 6e64 5f5f 2873 656c 662c 206f 7468  _and__(self, oth
+0000fba0: 6572 5f72 6566 3a20 2742 6962 6c65 5265  er_ref: 'BibleRe
+0000fbb0: 6627 2920 2d3e 2027 4269 626c 6552 616e  f') -> 'BibleRan
+0000fbc0: 6765 4c69 7374 273a 0a20 2020 2020 2020  geList':.       
+0000fbd0: 2072 6574 7572 6e20 7365 6c66 2e69 6e74   return self.int
+0000fbe0: 6572 7365 6374 696f 6e28 6f74 6865 725f  ersection(other_
+0000fbf0: 7265 6629 0a0a 2020 2020 6465 6620 5f5f  ref)..    def __
+0000fc00: 7375 625f 5f28 7365 6c66 2c20 6f74 6865  sub__(self, othe
+0000fc10: 725f 7265 663a 2027 4269 626c 6552 6566  r_ref: 'BibleRef
+0000fc20: 2729 202d 3e20 2742 6962 6c65 5261 6e67  ') -> 'BibleRang
+0000fc30: 654c 6973 7427 3a0a 2020 2020 2020 2020  eList':.        
+0000fc40: 7265 7475 726e 2073 656c 662e 6469 6666  return self.diff
+0000fc50: 6572 656e 6365 286f 7468 6572 5f72 6566  erence(other_ref
+0000fc60: 290a 0a20 2020 2064 6566 205f 5f78 6f72  )..    def __xor
+0000fc70: 5f5f 2873 656c 662c 206f 7468 6572 5f72  __(self, other_r
+0000fc80: 6566 3a20 2742 6962 6c65 5265 6627 2920  ef: 'BibleRef') 
+0000fc90: 2d3e 2027 4269 626c 6552 616e 6765 4c69  -> 'BibleRangeLi
+0000fca0: 7374 273a 0a20 2020 2020 2020 2072 6574  st':.        ret
+0000fcb0: 7572 6e20 7365 6c66 2e73 796d 5f64 6966  urn self.sym_dif
+0000fcc0: 6665 7265 6e63 6528 6f74 6865 725f 7265  ference(other_re
+0000fcd0: 6629 0a0a 2020 2020 6465 6620 5f5f 696f  f)..    def __io
+0000fce0: 725f 5f28 7365 6c66 2c20 6f74 6865 725f  r__(self, other_
+0000fcf0: 7265 663a 2027 4269 626c 6552 6566 2729  ref: 'BibleRef')
+0000fd00: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
+0000fd10: 6973 7427 3a0a 2020 2020 2020 2020 7265  ist':.        re
+0000fd20: 7475 726e 2073 656c 662e 756e 696f 6e5f  turn self.union_
+0000fd30: 7570 6461 7465 286f 7468 6572 5f72 6566  update(other_ref
+0000fd40: 2920 2020 200a 0a20 2020 2064 6566 205f  )    ..    def _
+0000fd50: 5f69 616e 645f 5f28 7365 6c66 2c20 6f74  _iand__(self, ot
+0000fd60: 6865 725f 7265 663a 2027 4269 626c 6552  her_ref: 'BibleR
+0000fd70: 6566 2729 202d 3e20 2742 6962 6c65 5261  ef') -> 'BibleRa
+0000fd80: 6e67 654c 6973 7427 3a0a 2020 2020 2020  ngeList':.      
+0000fd90: 2020 7265 7475 726e 2073 656c 662e 696e    return self.in
+0000fda0: 7465 7273 6563 7469 6f6e 5f75 7064 6174  tersection_updat
+0000fdb0: 6528 6f74 6865 725f 7265 6629 0a0a 2020  e(other_ref)..  
+0000fdc0: 2020 6465 6620 5f5f 6973 7562 5f5f 2873    def __isub__(s
+0000fdd0: 656c 662c 206f 7468 6572 5f72 6566 3a20  elf, other_ref: 
+0000fde0: 2742 6962 6c65 5265 6627 2920 2d3e 2027  'BibleRef') -> '
+0000fdf0: 4269 626c 6552 616e 6765 4c69 7374 273a  BibleRangeList':
+0000fe00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fe10: 7365 6c66 2e64 6966 6665 7265 6e63 655f  self.difference_
+0000fe20: 7570 6461 7465 286f 7468 6572 5f72 6566  update(other_ref
+0000fe30: 290a 0a20 2020 2064 6566 205f 5f69 786f  )..    def __ixo
+0000fe40: 725f 5f28 7365 6c66 2c20 6f74 6865 725f  r__(self, other_
+0000fe50: 7265 663a 2027 4269 626c 6552 6566 2729  ref: 'BibleRef')
+0000fe60: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
+0000fe70: 6973 7427 3a0a 2020 2020 2020 2020 7265  ist':.        re
+0000fe80: 7475 726e 2073 656c 662e 7379 6d5f 6469  turn self.sym_di
+0000fe90: 6666 6572 656e 6365 5f75 7064 6174 6528  fference_update(
+0000fea0: 6f74 6865 725f 7265 6629 0a0a 2020 2020  other_ref)..    
+0000feb0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+0000fec0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0000fed0: 726e 2066 2742 6962 6c65 5261 6e67 654c  rn f'BibleRangeL
+0000fee0: 6973 7428 227b 7365 6c66 2e73 7472 2829  ist("{self.str()
+0000fef0: 7d22 2927 0a20 2020 200a 2020 2020 6465  }")'.    .    de
+0000ff00: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
+0000ff10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ff20: 7365 6c66 2e73 7472 2829 0a0a 2020 2020  self.str()..    
+0000ff30: 6465 6620 7374 7228 7365 6c66 2c20 6162  def str(self, ab
+0000ff40: 6272 6576 3a20 626f 6f6c 203d 2046 616c  brev: bool = Fal
+0000ff50: 7365 2c20 616c 745f 7365 703a 2062 6f6f  se, alt_sep: boo
+0000ff60: 6c20 3d20 4661 6c73 652c 206e 6f73 7061  l = False, nospa
+0000ff70: 6365 3a20 626f 6f6c 203d 2046 616c 7365  ce: bool = False
+0000ff80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ff90: 2070 7265 7365 7276 655f 6772 6f75 7073   preserve_groups
+0000ffa0: 3a20 626f 6f6c 203d 2054 7275 652c 2066  : bool = True, f
+0000ffb0: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
+0000ffc0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0000ffd0: 2027 2727 5265 7475 726e 7320 6120 636f   '''Returns a co
+0000ffe0: 6e66 6967 7572 6174 626c 6520 7374 7269  nfiguratble stri
+0000fff0: 6e67 2072 6570 7265 7365 6e74 6174 696f  ng representatio
+00010000: 6e20 6f66 2074 6869 7320 4269 626c 6552  n of this BibleR
+00010010: 616e 6765 4c69 7374 2c20 6173 2066 6f6c  angeList, as fol
+00010020: 6c6f 7773 3a0a 0a20 2020 2020 2020 202d  lows:..        -
+00010030: 2049 6620 6061 6262 7265 7660 2069 7320   If `abbrev` is 
+00010040: 6054 7275 6560 2c20 7468 6520 6162 6272  `True`, the abbr
+00010050: 6576 6961 7465 6420 6e61 6d65 206f 6620  eviated name of 
+00010060: 7468 6520 626f 6f6b 2069 7320 7573 6564  the book is used
+00010070: 2028 696e 7374 6561 6420 6f66 2074 6865   (instead of the
+00010080: 2066 756c 6c20 6e61 6d65 292e 0a20 2020   full name)..   
+00010090: 2020 2020 202d 2049 6620 6061 6c74 5f73       - If `alt_s
+000100a0: 6570 6020 6973 2060 5472 7565 602c 2063  ep` is `True`, c
+000100b0: 6861 7074 6572 2061 6e64 2076 6572 7365  hapter and verse
+000100c0: 206e 756d 6265 7273 2061 7265 2073 6570   numbers are sep
+000100d0: 6172 6174 6564 2062 7920 7468 6520 616c  arated by the al
+000100e0: 7465 726e 6174 650a 2020 2020 2020 2020  ternate.        
+000100f0: 2020 7365 7061 7261 746f 7220 2864 6566    separator (def
+00010100: 6175 6c74 7320 746f 2060 2e60 2920 696e  aults to `.`) in
+00010110: 7374 6561 6420 6f66 2074 6865 2073 7461  stead of the sta
+00010120: 6e64 6172 6420 7365 7061 7261 746f 7220  ndard separator 
+00010130: 2864 6566 6175 6c74 7320 746f 2060 3a60  (defaults to `:`
+00010140: 292e 0a20 2020 2020 2020 202d 2049 6620  )..        - If 
+00010150: 606e 6f73 7061 6365 6020 6973 2060 5472  `nospace` is `Tr
+00010160: 7565 602c 206e 6f20 7370 6163 6573 2061  ue`, no spaces a
+00010170: 7265 2069 6e63 6c75 6465 6420 696e 2074  re included in t
+00010180: 6865 2073 7472 696e 672e 0a20 2020 2020  he string..     
+00010190: 2020 202d 2049 6620 6070 7265 7365 7276     - If `preserv
+000101a0: 655f 6772 6f75 7073 6020 6973 2060 5472  e_groups` is `Tr
+000101b0: 7565 602c 2074 6865 206d 616a 6f72 2067  ue`, the major g
+000101c0: 726f 7570 2073 6570 6172 6174 6f72 2069  roup separator i
+000101d0: 7320 616c 7761 7973 2075 7365 6420 6265  s always used be
+000101e0: 7477 6565 6e20 6772 6f75 7073 2c0a 2020  tween groups,.  
+000101f0: 2020 2020 2020 2020 616e 6420 6f6e 6c79          and only
+00010200: 2062 6574 7765 656e 2067 726f 7570 732c   between groups,
+00010210: 2077 6974 6820 7468 6520 6d69 6e6f 7220   with the minor 
+00010220: 6772 6f75 7020 7365 7061 7261 746f 7220  group separator 
+00010230: 7573 6564 2065 7863 6c75 7369 7665 6c79  used exclusively
+00010240: 2077 6974 6869 6e0a 2020 2020 2020 2020   within.        
+00010250: 2020 6772 6f75 7073 2e20 5061 7273 696e    groups. Parsin
+00010260: 6720 7468 6520 7265 7375 6c74 696e 6720  g the resulting 
+00010270: 7374 7269 6e67 2073 686f 756c 6420 7969  string should yi
+00010280: 656c 6420 616e 2065 7175 6976 616c 656e  eld an equivalen
+00010290: 7420 6042 6962 6c65 5261 6e67 654c 6973  t `BibleRangeLis
+000102a0: 7460 2e0a 2020 2020 2020 2020 2d20 4966  t`..        - If
+000102b0: 2060 7072 6573 6572 7665 5f67 726f 7570   `preserve_group
+000102c0: 7360 2069 7320 6046 616c 7365 602c 206d  s` is `False`, m
+000102d0: 616a 6f72 2061 6e64 206d 696e 6f72 2067  ajor and minor g
+000102e0: 726f 7570 2073 6570 6172 6174 6f72 7320  roup separators 
+000102f0: 6172 6520 7573 6564 2061 7320 6e65 6365  are used as nece
+00010300: 7373 6172 790a 2020 2020 2020 2020 2020  ssary.          
+00010310: 746f 2063 7265 6174 6520 7468 6520 6d6f  to create the mo
+00010320: 7374 2063 6f6e 7665 6e74 696f 6e61 6c20  st conventional 
+00010330: 7265 7375 6c74 696e 6720 7374 7269 6e67  resulting string
+00010340: 2c20 7768 6963 6820 6d61 7920 7265 7375  , which may resu
+00010350: 6c74 2069 6e20 6469 6666 6572 656e 740a  lt in different.
+00010360: 2020 2020 2020 2020 2020 7061 7373 6167            passag
+00010370: 6520 6772 6f75 7069 6e67 732e 0a20 2020  e groupings..   
+00010380: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00010390: 2063 7572 5f62 6f6f 6b20 3d20 4e6f 6e65   cur_book = None
+000103a0: 0a20 2020 2020 2020 2063 7572 5f63 6861  .        cur_cha
+000103b0: 7020 3d20 4e6f 6e65 0a20 2020 2020 2020  p = None.       
+000103c0: 2061 745f 7665 7273 655f 6c65 7665 6c20   at_verse_level 
+000103d0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000103e0: 6669 7273 745f 7261 6e67 6520 3d20 5472  first_range = Tr
+000103f0: 7565 0a20 2020 2020 2020 206c 6973 745f  ue.        list_
+00010400: 7365 7020 3d20 2222 0a20 2020 2020 2020  sep = "".       
+00010410: 2072 6573 756c 745f 7374 7220 3d20 2222   result_str = ""
+00010420: 0a20 2020 2020 2020 2066 6f72 6365 5f64  .        force_d
+00010430: 7561 6c5f 7265 6620 3d20 4661 6c73 6520  ual_ref = False 
+00010440: 2320 5472 7565 2069 6620 7765 2072 6571  # True if we req
+00010450: 7569 7265 2061 2073 696e 676c 6520 7265  uire a single re
+00010460: 6665 7265 6e63 6520 746f 2064 6973 706c  ference to displ
+00010470: 6179 2061 7320 6120 6475 616c 5f72 6566  ay as a dual_ref
+00010480: 6572 656e 6365 5f72 616e 6765 0a0a 2020  erence_range..  
+00010490: 2020 2020 2020 666f 7220 6772 6f75 7020        for group 
+000104a0: 696e 2073 656c 662e 6772 6f75 7073 3a0a  in self.groups:.
+000104b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000104c0: 6272 2069 6e20 6772 6f75 703a 0a20 2020  br in group:.   
+000104d0: 2020 2020 2020 2020 2020 2020 2062 6962               bib
+000104e0: 6c65 5f72 616e 6765 3a20 4269 626c 6552  le_range: BibleR
+000104f0: 616e 6765 203d 2062 7220 2320 5479 7065  ange = br # Type
+00010500: 6361 7374 2020 2020 2020 2020 2020 2020  cast            
+00010510: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00010520: 2020 2020 2069 6620 6269 626c 655f 7261       if bible_ra
+00010530: 6e67 652e 7370 616e 735f 7374 6172 745f  nge.spans_start_
+00010540: 626f 6f6b 2866 6c61 6773 293a 2023 2052  book(flags): # R
+00010550: 616e 6765 2073 7461 7274 2069 6e63 6c75  ange start inclu
+00010560: 6465 7320 616e 2065 6e74 6972 6520 626f  des an entire bo
+00010570: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
+00010580: 2020 2020 2020 2023 2045 7665 6e20 6966         # Even if
+00010590: 2061 6c72 6561 6479 2069 6e20 7361 6d65   already in same
+000105a0: 2062 6f6f 6b2c 2077 686f 6c65 2062 6f6f   book, whole boo
+000105b0: 6b20 7265 6665 7265 6e63 6573 2072 6570  k references rep
+000105c0: 6561 7420 7468 6520 7768 6f6c 6520 626f  eat the whole bo
+000105d0: 6f6b 206e 616d 652e 0a20 2020 2020 2020  ok name..       
+000105e0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+000105f0: 7274 5f70 6172 7473 203d 2042 6962 6c65  rt_parts = Bible
+00010600: 5665 7273 6550 6172 742e 424f 4f4b 0a20  VersePart.BOOK. 
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2063 7572 5f63 6861 7020 3d20 4e6f     cur_chap = No
+00010630: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00010640: 2020 2020 2020 2061 745f 7665 7273 655f         at_verse_
+00010650: 6c65 7665 6c20 3d20 4661 6c73 650a 2020  level = False.  
+00010660: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00010670: 6966 2062 6962 6c65 5f72 616e 6765 2e73  if bible_range.s
+00010680: 7061 6e73 5f73 7461 7274 5f63 6861 7028  pans_start_chap(
+00010690: 666c 6167 7329 3a20 2320 5261 6e67 6520  flags): # Range 
+000106a0: 7374 6172 7420 696e 636c 7564 6573 2061  start includes a
+000106b0: 6e20 656e 7469 7265 2063 6861 700a 2020  n entire chap.  
+000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106d0: 2020 6966 2063 7572 5f62 6f6f 6b20 3d3d    if cur_book ==
+000106e0: 2062 6962 6c65 5f72 616e 6765 2e73 7461   bible_range.sta
+000106f0: 7274 2e62 6f6f 6b3a 2023 2043 6f6e 7469  rt.book: # Conti
+00010700: 6e75 696e 6720 7361 6d65 2062 6f6f 6b0a  nuing same book.
+00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010720: 2020 2020 2020 2020 6966 2061 745f 7665          if at_ve
+00010730: 7273 655f 6c65 7665 6c3a 2023 2057 6527  rse_level: # We'
+00010740: 7265 2069 6e20 6120 6c69 7374 206f 6620  re in a list of 
+00010750: 7665 7273 6573 0a20 2020 2020 2020 2020  verses.         
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2020 2069 6620 6e6f 7420 7072 6573 6572     if not preser
+00010780: 7665 5f67 726f 7570 733a 2023 2055 7365  ve_groups: # Use
+00010790: 206d 616a 6f72 206c 6973 7420 7365 7020   major list sep 
+000107a0: 746f 2072 6574 7572 6e20 746f 2063 6861  to return to cha
+000107b0: 7074 6572 730a 2020 2020 2020 2020 2020  pters.          
+000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107d0: 2020 2020 2020 6c69 7374 5f73 6570 203d        list_sep =
+000107e0: 2062 6962 6c65 5f64 6174 6128 292e 6d61   bible_data().ma
+000107f0: 6a6f 725f 6c69 7374 5f73 6570 0a20 2020  jor_list_sep.   
+00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010810: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00010820: 7274 5f70 6172 7473 203d 2042 6962 6c65  rt_parts = Bible
+00010830: 5665 7273 6550 6172 742e 4348 4150 0a20  VersePart.CHAP. 
+00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010850: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010860: 745f 7665 7273 655f 6c65 7665 6c20 3d20  t_verse_level = 
+00010870: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 2020 656c 7365 3a20 2320 5072 6573 6572    else: # Preser
+000108a0: 7669 6e67 2067 726f 7570 730a 2020 2020  ving groups.    
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000108d0: 6973 745f 7365 7020 3d3d 2062 6962 6c65  ist_sep == bible
+000108e0: 5f64 6174 6128 292e 6d61 6a6f 725f 6c69  _data().major_li
+000108f0: 7374 5f73 6570 3a0a 2020 2020 2020 2020  st_sep:.        
+00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010910: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00010920: 2772 6520 7374 7261 6967 6874 2061 6674  're straight aft
+00010930: 6572 2061 206d 616a 6f72 206c 6973 7420  er a major list 
+00010940: 7265 662c 2073 6f20 6d75 7374 2072 6574  ref, so must ret
+00010950: 7572 6e20 746f 2063 6861 7020 6c65 7665  urn to chap leve
+00010960: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 2020 2020 2020 7374 6172 745f 7061 7274        start_part
+00010990: 7320 3d20 4269 626c 6556 6572 7365 5061  s = BibleVersePa
+000109a0: 7274 2e43 4841 500a 2020 2020 2020 2020  rt.CHAP.        
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109c0: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
+000109d0: 6572 7365 5f6c 6576 656c 203d 2046 616c  erse_level = Fal
+000109e0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a00: 2020 2065 6c73 653a 2023 2057 6527 7265     else: # We're
+00010a10: 2061 6674 6572 2061 206d 696e 6f72 206c   after a minor l
+00010a20: 6973 7420 7265 662c 2073 6f20 7765 2063  ist ref, so we c
+00010a30: 616e 2774 2072 6574 7572 6e20 746f 2063  an't return to c
+00010a40: 6861 7020 6c65 7665 6c2c 0a20 2020 2020  hap level,.     
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a70: 2023 2073 6f20 7765 2066 6f72 6365 2064   # so we force d
+00010a80: 6973 706c 6179 2074 6865 2077 686f 6c65  isplay the whole
+00010a90: 2072 616e 6765 0a20 2020 2020 2020 2020   range.         
+00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00010ac0: 5f70 6172 7473 203d 2042 6962 6c65 5665  _parts = BibleVe
+00010ad0: 7273 6550 6172 742e 4348 4150 5f56 4552  rsePart.CHAP_VER
+00010ae0: 5345 0a20 2020 2020 2020 2020 2020 2020  SE.             
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 2020 2061 745f 7665 7273 655f         at_verse_
+00010b10: 6c65 7665 6c20 3d20 5472 7565 0a20 2020  level = True.   
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b40: 2066 6f72 6365 5f64 7561 6c5f 7265 6620   force_dual_ref 
+00010b50: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+00010b60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00010b70: 6c73 653a 2023 2057 6527 7265 2069 6e20  lse: # We're in 
+00010b80: 6120 6c69 7374 206f 6620 6368 6170 7465  a list of chapte
+00010b90: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010bb0: 6620 6e6f 7420 7072 6573 6572 7665 5f67  f not preserve_g
+00010bc0: 726f 7570 733a 2023 2055 7365 206d 616a  roups: # Use maj
+00010bd0: 6f72 206c 6973 7420 7365 7020 6265 7477  or list sep betw
+00010be0: 6565 6e20 6368 6170 7465 7273 0a20 2020  een chapters.   
+00010bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c00: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00010c10: 745f 7365 7020 3d20 6269 626c 655f 6461  t_sep = bible_da
+00010c20: 7461 2829 2e6d 616a 6f72 5f6c 6973 745f  ta().major_list_
+00010c30: 7365 700a 2020 2020 2020 2020 2020 2020  sep.            
+00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c50: 2020 2020 7374 6172 745f 7061 7274 7320      start_parts 
+00010c60: 3d20 4269 626c 6556 6572 7365 5061 7274  = BibleVersePart
+00010c70: 2e43 4841 500a 2020 2020 2020 2020 2020  .CHAP.          
+00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c90: 2020 2020 2020 6174 5f76 6572 7365 5f6c        at_verse_l
+00010ca0: 6576 656c 203d 2046 616c 7365 0a20 2020  evel = False.   
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cc0: 2020 2020 2020 2020 2065 6c73 653a 2023           else: #
+00010cd0: 2050 7265 7365 7276 696e 6720 6772 6f75   Preserving grou
+00010ce0: 7073 0a20 2020 2020 2020 2020 2020 2020  ps.             
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d00: 2020 2069 6620 6c69 7374 5f73 6570 203d     if list_sep =
+00010d10: 3d20 6269 626c 655f 6461 7461 2829 2e6d  = bible_data().m
+00010d20: 616a 6f72 5f6c 6973 745f 7365 703a 0a20  ajor_list_sep:. 
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d50: 2020 2023 2057 6527 7265 2073 7472 6169     # We're strai
+00010d60: 6768 7420 6166 7465 7220 6120 6d61 6a6f  ght after a majo
+00010d70: 7220 6c69 7374 2072 6566 2c20 736f 2063  r list ref, so c
+00010d80: 616e 2072 6574 7572 6e20 746f 2063 6861  an return to cha
+00010d90: 7020 6c65 7665 6c0a 2020 2020 2020 2020  p level.        
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010db0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00010dc0: 745f 7061 7274 7320 3d20 4269 626c 6556  t_parts = BibleV
+00010dd0: 6572 7365 5061 7274 2e43 4841 500a 2020  ersePart.CHAP.  
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 6174 5f76 6572 7365 5f6c 6576 656c    at_verse_level
+00010e10: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e30: 2020 2020 2020 2020 2065 6c73 653a 2023           else: #
+00010e40: 2057 6527 7265 2061 6674 6572 2061 206d   We're after a m
+00010e50: 696e 6f72 206c 6973 7420 7265 660a 2020  inor list ref.  
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e80: 2020 6966 2062 6962 6c65 5f72 616e 6765    if bible_range
+00010e90: 2e73 7061 6e73 5f65 6e64 5f63 6861 7028  .spans_end_chap(
+00010ea0: 666c 6167 7329 3a0a 2020 2020 2020 2020  flags):.        
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2320 5468 6973 2072 616e 6765 2069 7320  # This range is 
+00010ee0: 6120 7768 6f6c 6520 7365 7420 6f66 2063  a whole set of c
+00010ef0: 6861 7074 6572 732c 2073 6f20 6a75 7374  hapters, so just
+00010f00: 2064 6973 706c 6179 2063 6861 7074 6572   display chapter
+00010f10: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+00010f40: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
+00010f50: 7365 5061 7274 2e43 4841 500a 2020 2020  sePart.CHAP.    
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 6174 5f76 6572 7365 5f6c 6576      at_verse_lev
+00010f90: 656c 203d 2046 616c 7365 0a20 2020 2020  el = False.     
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00010fc0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00010ff0: 6869 7320 7261 6e67 6520 696e 766f 6c76  his range involv
+00011000: 6573 2076 6572 7365 732c 2069 6e20 6120  es verses, in a 
+00011010: 6c69 7374 2074 6861 7427 7320 6f74 6865  list that's othe
+00011020: 7277 6973 6520 6368 6170 7465 7273 2c0a  rwise chapters,.
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2320 736f 2069 7427          # so it'
+00011060: 7320 636c 6561 7265 7220 746f 2064 6973  s clearer to dis
+00011070: 706c 6179 2075 7369 6e67 2076 6572 7365  play using verse
+00011080: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+000110b0: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
+000110c0: 7365 5061 7274 2e43 4841 505f 5645 5253  sePart.CHAP_VERS
+000110d0: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 2020 2020 6174 5f76 6572            at_ver
+00011100: 7365 5f6c 6576 656c 203d 2054 7275 650a  se_level = True.
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011130: 2020 2020 2020 2020 666f 7263 655f 6475          force_du
+00011140: 616c 5f72 6566 203d 2054 7275 650a 2020  al_ref = True.  
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 656c 7365 3a20 2320 5374 6172 7420    else: # Start 
+00011170: 6f66 2061 2064 6966 6665 7265 6e74 2062  of a different b
+00011180: 6f6f 6b0a 2020 2020 2020 2020 2020 2020  ook.            
+00011190: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000111a0: 6f74 2070 7265 7365 7276 655f 6772 6f75  ot preserve_grou
+000111b0: 7073 3a20 2320 5573 6520 6d61 6a6f 7220  ps: # Use major 
+000111c0: 6c69 7374 2073 6570 2062 6574 7765 656e  list sep between
+000111d0: 2062 6f6f 6b73 0a20 2020 2020 2020 2020   books.         
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 206c 6973 745f 7365 7020 3d20 6269     list_sep = bi
+00011200: 626c 655f 6461 7461 2829 2e6d 616a 6f72  ble_data().major
+00011210: 5f6c 6973 745f 7365 700a 2020 2020 2020  _list_sep.      
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 7374 6172 745f 7061 7274 7320 3d20    start_parts = 
+00011240: 4269 626c 6556 6572 7365 5061 7274 2e42  BibleVersePart.B
+00011250: 4f4f 4b5f 4348 4150 0a20 2020 2020 2020  OOK_CHAP.       
+00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011270: 2061 745f 7665 7273 655f 6c65 7665 6c20   at_verse_level 
+00011280: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00011290: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
+000112a0: 6368 6170 203d 2062 6962 6c65 5f72 616e  chap = bible_ran
+000112b0: 6765 2e73 7461 7274 2e63 6861 705f 6e75  ge.start.chap_nu
+000112c0: 6d0a 2020 2020 2020 2020 2020 2020 2020  m.              
+000112d0: 2020 656c 7365 3a20 2320 5261 6e67 6520    else: # Range 
+000112e0: 7374 6172 7420 6973 206a 7573 7420 6120  start is just a 
+000112f0: 7061 7274 6963 756c 6172 2076 6572 7365  particular verse
+00011300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011310: 2020 2020 2069 6620 6375 725f 626f 6f6b       if cur_book
+00011320: 203d 3d20 6269 626c 655f 7261 6e67 652e   == bible_range.
+00011330: 7374 6172 742e 626f 6f6b 3a20 2320 436f  start.book: # Co
+00011340: 6e74 696e 7569 6e67 2073 616d 6520 626f  ntinuing same bo
+00011350: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
+00011360: 2020 2020 2020 2020 2020 2069 6620 6174             if at
+00011370: 5f76 6572 7365 5f6c 6576 656c 2061 6e64  _verse_level and
+00011380: 2063 7572 5f63 6861 7020 3d3d 2062 6962   cur_chap == bib
+00011390: 6c65 5f72 616e 6765 2e73 7461 7274 2e63  le_range.start.c
+000113a0: 6861 705f 6e75 6d3a 2023 2043 6f6e 7469  hap_num: # Conti
+000113b0: 6e75 696e 6720 7361 6d65 2063 6861 700a  nuing same chap.
+000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113d0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+000113e0: 745f 7061 7274 7320 3d20 4269 626c 6556  t_parts = BibleV
+000113f0: 6572 7365 5061 7274 2e56 4552 5345 0a20  ersePart.VERSE. 
+00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011410: 2020 2020 2020 2065 6c73 653a 2023 2041         else: # A
+00011420: 7420 6368 6170 206c 6576 656c 206f 7220  t chap level or 
+00011430: 7665 7273 6520 6c65 7665 6c20 696e 2061  verse level in a
+00011440: 2064 6966 6665 7265 6e74 2063 6861 700a   different chap.
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00011470: 6f74 2070 7265 7365 7276 655f 6772 6f75  ot preserve_grou
+00011480: 7073 3a20 2320 5573 6520 6d61 6a6f 7220  ps: # Use major 
+00011490: 6c69 7374 2073 6570 2062 6574 7765 656e  list sep between
+000114a0: 2063 6861 7074 6572 730a 2020 2020 2020   chapters.      
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2020 2020 2020 2020 6c69 7374 5f73            list_s
+000114d0: 6570 203d 2062 6962 6c65 5f64 6174 6128  ep = bible_data(
+000114e0: 292e 6d61 6a6f 725f 6c69 7374 5f73 6570  ).major_list_sep
+000114f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011500: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00011510: 7274 5f70 6172 7473 203d 2042 6962 6c65  rt_parts = Bible
+00011520: 5665 7273 6550 6172 742e 4348 4150 5f56  VersePart.CHAP_V
+00011530: 4552 5345 0a20 2020 2020 2020 2020 2020  ERSE.           
+00011540: 2020 2020 2020 2020 2065 6c73 653a 2023           else: #
+00011550: 2044 6966 6665 7265 6e74 2062 6f6f 6b0a   Different book.
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2020 6966 206e 6f74 2070          if not p
+00011580: 7265 7365 7276 655f 6772 6f75 7073 3a20  reserve_groups: 
+00011590: 2320 5573 6520 6d61 6a6f 7220 6c69 7374  # Use major list
+000115a0: 2073 6570 2062 6574 7765 656e 2062 6f6f   sep between boo
+000115b0: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
+000115c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000115d0: 6973 745f 7365 7020 3d20 6269 626c 655f  ist_sep = bible_
+000115e0: 6461 7461 2829 2e6d 616a 6f72 5f6c 6973  data().major_lis
+000115f0: 745f 7365 700a 2020 2020 2020 2020 2020  t_sep.          
+00011600: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00011610: 6172 745f 7061 7274 7320 3d20 4269 626c  art_parts = Bibl
+00011620: 6556 6572 7365 5061 7274 2e46 554c 4c5f  eVersePart.FULL_
+00011630: 5245 460a 2020 2020 2020 2020 2020 2020  REF.            
+00011640: 2020 2020 2020 2020 6375 725f 6368 6170          cur_chap
+00011650: 203d 2062 6962 6c65 5f72 616e 6765 2e73   = bible_range.s
+00011660: 7461 7274 2e63 6861 705f 6e75 6d0a 2020  tart.chap_num.  
+00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011680: 2020 6174 5f76 6572 7365 5f6c 6576 656c    at_verse_level
+00011690: 203d 2054 7275 6520 2320 416c 6c20 7369   = True # All si
+000116a0: 6e67 6c65 2076 6572 7365 7320 6d6f 7665  ngle verses move
+000116b0: 2075 7320 746f 2076 6572 7365 206c 6576   us to verse lev
+000116c0: 656c 0a20 2020 2020 2020 2020 2020 2020  el.             
+000116d0: 2020 2063 7572 5f62 6f6f 6b20 3d20 6269     cur_book = bi
+000116e0: 626c 655f 7261 6e67 652e 7374 6172 742e  ble_range.start.
+000116f0: 626f 6f6b 0a20 2020 2020 2020 2020 2020  book.           
+00011700: 2020 2020 2073 7461 7274 5f73 7472 203d       start_str =
+00011710: 2062 6962 6c65 5f72 616e 6765 2e73 7461   bible_range.sta
+00011720: 7274 2e73 7472 2861 6262 7265 762c 2061  rt.str(abbrev, a
+00011730: 6c74 5f73 6570 2c20 6e6f 7370 6163 652c  lt_sep, nospace,
+00011740: 2073 7461 7274 5f70 6172 7473 2920 0a0a   start_parts) ..
+00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011760: 6966 206e 6f74 2066 6f72 6365 5f64 7561  if not force_dua
+00011770: 6c5f 7265 6620 616e 6420 2862 6962 6c65  l_ref and (bible
+00011780: 5f72 616e 6765 2e69 735f 7768 6f6c 655f  _range.is_whole_
+00011790: 626f 6f6b 2866 6c61 6773 2920 6f72 0a20  book(flags) or. 
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117c0: 2020 2020 2020 2020 2020 6269 626c 655f            bible_
+000117d0: 7261 6e67 652e 6973 5f77 686f 6c65 5f63  range.is_whole_c
+000117e0: 6861 7028 666c 6167 7329 206f 7220 5c0a  hap(flags) or \.
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011810: 2020 2020 2020 2020 2020 2062 6962 6c65             bible
+00011820: 5f72 616e 6765 2e69 735f 7369 6e67 6c65  _range.is_single
+00011830: 5f76 6572 7365 2829 293a 0a20 2020 2020  _verse()):.     
+00011840: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011850: 2053 696e 676c 6520 7265 6665 7265 6e63   Single referenc
+00011860: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00011870: 2020 2020 2020 656e 645f 7374 7220 3d20        end_str = 
+00011880: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00011890: 2020 2020 2020 2072 616e 6765 5f73 6570         range_sep
+000118a0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+000118b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 7261 6e67 655f 7365 7020 3d20 6269 626c  range_sep = bibl
+000118e0: 655f 6461 7461 2829 2e72 616e 6765 5f73  e_data().range_s
+000118f0: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+00011900: 2020 2020 2020 2069 6620 6269 626c 655f         if bible_
+00011910: 7261 6e67 652e 656e 642e 626f 6f6b 2021  range.end.book !
+00011920: 3d20 6269 626c 655f 7261 6e67 652e 7374  = bible_range.st
+00011930: 6172 742e 626f 6f6b 3a0a 2020 2020 2020  art.book:.      
+00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 2020 6174 5f76 6572 7365 5f6c 6576 656c    at_verse_level
+00011960: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
+00011970: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011980: 2062 6962 6c65 5f72 616e 6765 2e73 7061   bible_range.spa
+00011990: 6e73 5f65 6e64 5f62 6f6f 6b28 666c 6167  ns_end_book(flag
+000119a0: 7329 3a20 2320 5261 6e67 6520 656e 6420  s): # Range end 
+000119b0: 696e 636c 7564 6573 2061 6e20 656e 7469  includes an enti
+000119c0: 7265 2062 6f6f 6b0a 2020 2020 2020 2020  re book.        
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119e0: 656e 645f 7061 7274 7320 3d20 4269 626c  end_parts = Bibl
+000119f0: 6556 6572 7365 5061 7274 2e42 4f4f 4b0a  eVersePart.BOOK.
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 2020 2020 2020 6375 725f 6368 6170          cur_chap
+00011a20: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 6174 5f76 6572 7365 5f6c 6576 656c 203d  at_verse_level =
+00011a50: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00011a60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00011a70: 6e6f 7420 6174 5f76 6572 7365 5f6c 6576  not at_verse_lev
+00011a80: 656c 2061 6e64 2062 6962 6c65 5f72 616e  el and bible_ran
+00011a90: 6765 2e73 7061 6e73 5f65 6e64 5f63 6861  ge.spans_end_cha
+00011aa0: 7028 666c 6167 7329 3a20 2320 5261 6e67  p(flags): # Rang
+00011ab0: 6520 656e 6420 696e 636c 7564 6573 2061  e end includes a
+00011ac0: 6e20 656e 7469 7265 2063 6861 700a 2020  n entire chap.  
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 6966 2063 7572 5f62 6f6f        if cur_boo
+00011af0: 6b20 3d3d 2062 6962 6c65 5f72 616e 6765  k == bible_range
+00011b00: 2e65 6e64 2e62 6f6f 6b3a 2023 2043 6f6e  .end.book: # Con
+00011b10: 7469 6e75 696e 6720 7361 6d65 2062 6f6f  tinuing same boo
+00011b20: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00011b30: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00011b40: 645f 7061 7274 7320 3d20 4269 626c 6556  d_parts = BibleV
+00011b50: 6572 7365 5061 7274 2e43 4841 500a 2020  ersePart.CHAP.  
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b70: 2020 2020 2020 656c 7365 3a20 2320 4469        else: # Di
+00011b80: 6666 6572 656e 7420 626f 6f6b 0a20 2020  fferent book.   
+00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ba0: 2020 2020 2020 2020 2065 6e64 5f70 6172           end_par
+00011bb0: 7473 203d 2042 6962 6c65 5665 7273 6550  ts = BibleVerseP
+00011bc0: 6172 742e 424f 4f4b 5f43 4841 500a 2020  art.BOOK_CHAP.  
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 2020 6375 725f 6368 6170 203d        cur_chap =
+00011bf0: 2062 6962 6c65 5f72 616e 6765 2e65 6e64   bible_range.end
+00011c00: 2e63 6861 705f 6e75 6d0a 2020 2020 2020  .chap_num.      
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2020 6174 5f76 6572 7365 5f6c 6576 656c    at_verse_level
+00011c30: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00011c40: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00011c50: 653a 2023 2052 616e 6765 2065 6e64 2069  e: # Range end i
+00011c60: 7320 6120 7768 6f6c 6520 6368 6170 2061  s a whole chap a
+00011c70: 6674 6572 2061 2070 6172 7469 6375 6c61  fter a particula
+00011c80: 7220 7665 7273 652c 206f 7220 6120 7061  r verse, or a pa
+00011c90: 7274 6963 756c 6172 2076 6572 7365 0a20  rticular verse. 
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 2020 2020 2069 6620 6375 725f 626f         if cur_bo
+00011cc0: 6f6b 203d 3d20 6269 626c 655f 7261 6e67  ok == bible_rang
+00011cd0: 652e 656e 642e 626f 6f6b 3a20 2320 436f  e.end.book: # Co
+00011ce0: 6e74 696e 7569 6e67 2073 616d 6520 626f  ntinuing same bo
+00011cf0: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011d10: 6620 6375 725f 6368 6170 203d 3d20 6269  f cur_chap == bi
+00011d20: 626c 655f 7261 6e67 652e 656e 642e 6368  ble_range.end.ch
+00011d30: 6170 5f6e 756d 3a20 2320 436f 6e74 696e  ap_num: # Contin
+00011d40: 7569 6e67 2073 616d 6520 6368 6170 0a20  uing same chap. 
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011d70: 6e64 5f70 6172 7473 203d 2042 6962 6c65  nd_parts = Bible
+00011d80: 5665 7273 6550 6172 742e 5645 5253 450a  VersePart.VERSE.
 00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2320 6368 616e 6765 6420 746f      # changed to
-00011db0: 2070 6f69 6e74 2074 6f20 7468 6520 6669   point to the fi
-00011dc0: 7273 7420 6f66 2074 6865 2072 6573 756c  rst of the resul
-00011dd0: 7420 6974 656d 732e 2054 6865 2065 6173  t items. The eas
-00011de0: 6965 7374 0a20 2020 2020 2020 2020 2020  iest.           
-00011df0: 2020 2020 2020 2020 2023 2077 6179 2074           # way t
-00011e00: 6f20 646f 2074 6869 7320 6973 2074 6f20  o do this is to 
-00011e10: 696e 7365 7274 2074 6865 2072 6573 756c  insert the resul
-00011e20: 7420 6974 656d 7320 7374 6172 7469 6e67  t items starting
-00011e30: 2066 726f 6d20 7468 6520 656e 643a 0a20   from the end:. 
+00011da0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00011db0: 3a20 2320 4469 6666 6572 656e 7420 6368  : # Different ch
+00011dc0: 6170 0a20 2020 2020 2020 2020 2020 2020  ap.             
+00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011de0: 2020 2065 6e64 5f70 6172 7473 203d 2042     end_parts = B
+00011df0: 6962 6c65 5665 7273 6550 6172 742e 4348  ibleVersePart.CH
+00011e00: 4150 5f56 4552 5345 0a20 2020 2020 2020  AP_VERSE.       
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 2065 6c73 653a 2023 2044 6966 6665 7265   else: # Differe
+00011e30: 6e74 2062 6f6f 6b0a 2020 2020 2020 2020  nt book.        
 00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 206f 6c64 5f73 656c 665f 6e6f 6465     old_self_node
-00011e60: 203d 2073 656c 665f 6e6f 6465 0a20 2020   = self_node.   
-00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e80: 2066 6f72 2064 6966 6665 7265 6e63 655f   for difference_
-00011e90: 7261 6e67 6520 696e 2072 6576 6572 7365  range in reverse
-00011ea0: 6428 6974 656d 5f64 6966 6665 7265 6e63  d(item_differenc
-00011eb0: 655f 6c69 7374 293a 0a20 2020 2020 2020  e_list):.       
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2073 656c 662e 5f69 6e73 6572 745f 6265   self._insert_be
-00011ee0: 666f 7265 2873 656c 665f 6e6f 6465 2c20  fore(self_node, 
-00011ef0: 6469 6666 6572 656e 6365 5f72 616e 6765  difference_range
-00011f00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011f10: 2020 2020 2020 2020 2020 7365 6c66 5f6e            self_n
-00011f20: 6f64 6520 3d20 7365 6c66 5f6e 6f64 652e  ode = self_node.
-00011f30: 7072 6576 0a20 2020 2020 2020 2020 2020  prev.           
-00011f40: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00011f50: 6f70 5f6e 6f64 6528 6f6c 645f 7365 6c66  op_node(old_self
-00011f60: 5f6e 6f64 6529 0a20 2020 2020 2020 2020  _node).         
-00011f70: 2020 2073 656c 665f 6e6f 6465 203d 2073     self_node = s
-00011f80: 656c 665f 6e6f 6465 2e6e 6578 740a 2020  elf_node.next.  
-00011f90: 2020 2020 2020 7365 6c66 2e6d 6572 6765        self.merge
-00011fa0: 2829 0a0a 2020 2020 6465 6620 7379 6d5f  ()..    def sym_
-00011fb0: 6469 6666 6572 656e 6365 2873 656c 662c  difference(self,
-00011fc0: 206f 7468 6572 5f72 6566 3a20 2742 6962   other_ref: 'Bib
-00011fd0: 6c65 5265 6627 2c20 666c 6167 733a 2042  leRef', flags: B
-00011fe0: 6962 6c65 466c 6167 203d 204e 6f6e 6529  ibleFlag = None)
-00011ff0: 202d 3e20 2742 6962 6c65 5261 6e67 654c   -> 'BibleRangeL
-00012000: 6973 7427 3a0a 2020 2020 2020 2020 2727  ist':.        ''
-00012010: 2752 6574 7572 6e73 2061 206e 6577 2060  'Returns a new `
-00012020: 4269 626c 6552 616e 6765 4c69 7374 6020  BibleRangeList` 
-00012030: 6f66 2076 6572 7365 7320 7468 6174 2061  of verses that a
-00012040: 7265 2065 6974 6865 7220 696e 2074 6869  re either in thi
-00012050: 7320 6042 6962 6c65 5261 6e67 654c 6973  s `BibleRangeLis
-00012060: 7460 2c20 6f72 2069 6e20 606f 7468 6572  t`, or in `other
-00012070: 5f72 6566 602c 0a20 2020 2020 2020 2062  _ref`,.        b
-00012080: 7574 206e 6f74 2062 6f74 682e 0a0a 2020  ut not both...  
-00012090: 2020 2020 2020 5573 696e 6720 7468 6520        Using the 
-000120a0: 605e 6020 6f70 6572 6174 6f72 2069 7320  `^` operator is 
-000120b0: 6571 7569 7661 6c65 6e74 2074 6f20 6361  equivalent to ca
-000120c0: 6c6c 696e 6720 6073 796d 5f64 6966 6665  lling `sym_diffe
-000120d0: 7265 6e63 6528 2960 2077 6974 6820 6066  rence()` with `f
-000120e0: 6c61 6773 203d 204e 6f6e 6560 2e0a 2020  lags = None`..  
-000120f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00012100: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00012110: 6f74 6865 725f 7265 662c 2042 6962 6c65  other_ref, Bible
-00012120: 5665 7273 6529 3a0a 2020 2020 2020 2020  Verse):.        
-00012130: 2020 2020 2320 436f 6e76 6572 7420 746f      # Convert to
-00012140: 2042 6962 6c65 5261 6e67 654c 6973 7420   BibleRangeList 
-00012150: 2861 6e64 2077 6520 646f 6e27 7420 656e  (and we don't en
-00012160: 666f 7263 6520 6578 6973 7469 6e67 2066  force existing f
-00012170: 6c61 6773 2066 6f72 2063 6f6e 7665 7273  lags for convers
-00012180: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
-00012190: 2020 6f74 6865 725f 7265 6620 3d20 4269    other_ref = Bi
-000121a0: 626c 6552 616e 6765 4c69 7374 285b 4269  bleRangeList([Bi
-000121b0: 626c 6552 616e 6765 2873 7461 7274 3d6f  bleRange(start=o
-000121c0: 7468 6572 5f72 6566 2c20 656e 643d 6f74  ther_ref, end=ot
-000121d0: 6865 725f 7265 662c 2066 6c61 6773 3d42  her_ref, flags=B
-000121e0: 6962 6c65 466c 6167 2e41 4c4c 295d 290a  ibleFlag.ALL)]).
-000121f0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00012200: 6e73 7461 6e63 6528 6f74 6865 725f 7265  nstance(other_re
-00012210: 662c 2042 6962 6c65 5261 6e67 6529 3a0a  f, BibleRange):.
-00012220: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00012230: 725f 7265 6620 3d20 4269 626c 6552 616e  r_ref = BibleRan
-00012240: 6765 4c69 7374 285b 6f74 6865 725f 7265  geList([other_re
-00012250: 665d 290a 2020 2020 2020 2020 6966 206e  f]).        if n
-00012260: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
-00012270: 6865 725f 7265 662c 2042 6962 6c65 5261  her_ref, BibleRa
-00012280: 6e67 654c 6973 7429 3a0a 2020 2020 2020  ngeList):.      
-00012290: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000122a0: 6545 7272 6f72 2866 227b 6f74 6865 725f  eError(f"{other_
-000122b0: 7265 667d 2069 7320 6e6f 7420 6120 7661  ref} is not a va
-000122c0: 6c69 6420 4269 626c 6552 6566 2229 2020  lid BibleRef")  
-000122d0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-000122e0: 2020 2020 2020 2020 756e 696f 6e5f 6c69          union_li
-000122f0: 7374 203d 2073 656c 662e 756e 696f 6e28  st = self.union(
-00012300: 6f74 6865 725f 7265 662c 2066 6c61 6773  other_ref, flags
-00012310: 3d66 6c61 6773 290a 2020 2020 2020 2020  =flags).        
-00012320: 696e 7465 7273 6563 7469 6f6e 5f6c 6973  intersection_lis
-00012330: 7420 3d20 7365 6c66 2e69 6e74 6572 7365  t = self.interse
-00012340: 6374 696f 6e28 6f74 6865 725f 7265 662c  ction(other_ref,
-00012350: 2066 6c61 6773 3d66 6c61 6773 290a 2020   flags=flags).  
-00012360: 2020 2020 2020 7265 7475 726e 2075 6e69        return uni
-00012370: 6f6e 5f6c 6973 742e 6469 6666 6572 656e  on_list.differen
-00012380: 6365 2869 6e74 6572 7365 6374 696f 6e5f  ce(intersection_
-00012390: 6c69 7374 2c20 666c 6167 733d 666c 6167  list, flags=flag
-000123a0: 7329 0a0a 2020 2020 6465 6620 7379 6d5f  s)..    def sym_
-000123b0: 6469 6666 6572 656e 6365 5f75 7064 6174  difference_updat
-000123c0: 6528 7365 6c66 2c20 6f74 6865 725f 7265  e(self, other_re
-000123d0: 663a 2027 4269 626c 6552 6566 272c 2066  f: 'BibleRef', f
-000123e0: 6c61 6773 3a20 4269 626c 6546 6c61 6720  lags: BibleFlag 
-000123f0: 3d20 4e6f 6e65 2920 2d3e 2027 4269 626c  = None) -> 'Bibl
-00012400: 6552 616e 6765 4c69 7374 273a 0a20 2020  eRangeList':.   
-00012410: 2020 2020 2027 2727 5570 6461 7465 7320       '''Updates 
-00012420: 7468 6973 206c 6973 7420 746f 2062 6520  this list to be 
-00012430: 7468 6520 7379 6d6d 6574 7269 6320 6469  the symmetric di
-00012440: 6666 6572 656e 6365 206f 6620 6974 7320  fference of its 
-00012450: 6578 6973 7469 6e67 2065 6c65 6d65 6e74  existing element
-00012460: 7320 616e 6420 606f 7468 6572 5f72 6566  s and `other_ref
-00012470: 602c 2074 6865 6e0a 2020 2020 2020 2020  `, then.        
-00012480: 636f 6e73 6f6c 6964 6174 6573 2074 6869  consolidates thi
-00012490: 7320 6c69 7374 2e0a 0a20 2020 2020 2020  s list...       
-000124a0: 2055 7369 6e67 2074 6865 2060 5e3d 6020   Using the `^=` 
-000124b0: 6f70 6572 6174 6f72 2069 7320 6571 7569  operator is equi
-000124c0: 7661 6c65 6e74 2074 6f20 6361 6c6c 696e  valent to callin
-000124d0: 6720 6073 796d 5f64 6966 6665 7265 6e63  g `sym_differenc
-000124e0: 655f 7570 6461 7465 2829 6020 7769 7468  e_update()` with
-000124f0: 2060 666c 6167 7320 3d20 4e6f 6e65 602e   `flags = None`.
-00012500: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00012510: 2020 2020 2073 796d 5f64 6966 6665 7265       sym_differe
-00012520: 6e63 655f 6c69 7374 203d 2073 656c 662e  nce_list = self.
-00012530: 7379 6d5f 6469 6666 6572 656e 6365 286f  sym_difference(o
-00012540: 7468 6572 5f72 6566 2c20 666c 6167 733d  ther_ref, flags=
-00012550: 666c 6167 7329 0a20 2020 2020 2020 2073  flags).        s
-00012560: 656c 662e 636c 6561 7228 290a 2020 2020  elf.clear().    
-00012570: 2020 2020 7365 6c66 2e65 7874 656e 6428      self.extend(
-00012580: 7379 6d5f 6469 6666 6572 656e 6365 5f6c  sym_difference_l
-00012590: 6973 7429 0a0a 2020 2020 6465 6620 5f5f  ist)..    def __
-000125a0: 636f 6e74 6169 6e73 5f5f 2873 656c 662c  contains__(self,
-000125b0: 2062 6962 6c65 5f72 6566 2920 2d3e 2062   bible_ref) -> b
-000125c0: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-000125d0: 5265 7475 726e 7320 5472 7565 2069 6620  Returns True if 
-000125e0: 6974 656d 2069 7320 6120 4269 626c 6552  item is a BibleR
-000125f0: 6566 2074 6861 7420 6661 6c6c 7320 7769  ef that falls wi
-00012600: 7468 696e 2074 6869 7320 7261 6e67 652c  thin this range,
-00012610: 206f 7468 6572 7769 7365 2046 616c 7365   otherwise False
-00012620: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00012630: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00012640: 662e 636f 6e74 6169 6e73 2862 6962 6c65  f.contains(bible
-00012650: 5f72 6566 290a 0a20 2020 2064 6566 205f  _ref)..    def _
-00012660: 5f6f 725f 5f28 7365 6c66 2c20 6f74 6865  _or__(self, othe
-00012670: 725f 7265 663a 2027 4269 626c 6552 6566  r_ref: 'BibleRef
-00012680: 2729 202d 3e20 2742 6962 6c65 5261 6e67  ') -> 'BibleRang
-00012690: 654c 6973 7427 3a0a 2020 2020 2020 2020  eList':.        
-000126a0: 7265 7475 726e 2073 656c 662e 756e 696f  return self.unio
-000126b0: 6e28 6f74 6865 725f 7265 6629 0a20 2020  n(other_ref).   
-000126c0: 200a 2020 2020 6465 6620 5f5f 616e 645f   .    def __and_
-000126d0: 5f28 7365 6c66 2c20 6f74 6865 725f 7265  _(self, other_re
-000126e0: 663a 2027 4269 626c 6552 6566 2729 202d  f: 'BibleRef') -
-000126f0: 3e20 2742 6962 6c65 5261 6e67 654c 6973  > 'BibleRangeLis
-00012700: 7427 3a0a 2020 2020 2020 2020 7265 7475  t':.        retu
-00012710: 726e 2073 656c 662e 696e 7465 7273 6563  rn self.intersec
-00012720: 7469 6f6e 286f 7468 6572 5f72 6566 290a  tion(other_ref).
-00012730: 0a20 2020 2064 6566 205f 5f73 7562 5f5f  .    def __sub__
-00012740: 2873 656c 662c 206f 7468 6572 5f72 6566  (self, other_ref
-00012750: 3a20 2742 6962 6c65 5265 6627 2920 2d3e  : 'BibleRef') ->
-00012760: 2027 4269 626c 6552 616e 6765 4c69 7374   'BibleRangeList
-00012770: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
-00012780: 6e20 7365 6c66 2e64 6966 6665 7265 6e63  n self.differenc
-00012790: 6528 6f74 6865 725f 7265 6629 0a0a 2020  e(other_ref)..  
-000127a0: 2020 6465 6620 5f5f 786f 725f 5f28 7365    def __xor__(se
-000127b0: 6c66 2c20 6f74 6865 725f 7265 663a 2027  lf, other_ref: '
-000127c0: 4269 626c 6552 6566 2729 202d 3e20 2742  BibleRef') -> 'B
-000127d0: 6962 6c65 5261 6e67 654c 6973 7427 3a0a  ibleRangeList':.
-000127e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000127f0: 656c 662e 7379 6d5f 6469 6666 6572 656e  elf.sym_differen
-00012800: 6365 286f 7468 6572 5f72 6566 290a 0a20  ce(other_ref).. 
-00012810: 2020 2064 6566 205f 5f69 6f72 5f5f 2873     def __ior__(s
-00012820: 656c 662c 206f 7468 6572 5f72 6566 3a20  elf, other_ref: 
-00012830: 2742 6962 6c65 5265 6627 2920 2d3e 2027  'BibleRef') -> '
-00012840: 4269 626c 6552 616e 6765 4c69 7374 273a  BibleRangeList':
-00012850: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012860: 7365 6c66 2e75 6e69 6f6e 5f75 7064 6174  self.union_updat
-00012870: 6528 6f74 6865 725f 7265 6629 2020 2020  e(other_ref)    
-00012880: 0a0a 2020 2020 6465 6620 5f5f 6961 6e64  ..    def __iand
-00012890: 5f5f 2873 656c 662c 206f 7468 6572 5f72  __(self, other_r
-000128a0: 6566 3a20 2742 6962 6c65 5265 6627 2920  ef: 'BibleRef') 
-000128b0: 2d3e 2027 4269 626c 6552 616e 6765 4c69  -> 'BibleRangeLi
-000128c0: 7374 273a 0a20 2020 2020 2020 2072 6574  st':.        ret
-000128d0: 7572 6e20 7365 6c66 2e69 6e74 6572 7365  urn self.interse
-000128e0: 6374 696f 6e5f 7570 6461 7465 286f 7468  ction_update(oth
-000128f0: 6572 5f72 6566 290a 0a20 2020 2064 6566  er_ref)..    def
-00012900: 205f 5f69 7375 625f 5f28 7365 6c66 2c20   __isub__(self, 
-00012910: 6f74 6865 725f 7265 663a 2027 4269 626c  other_ref: 'Bibl
-00012920: 6552 6566 2729 202d 3e20 2742 6962 6c65  eRef') -> 'Bible
-00012930: 5261 6e67 654c 6973 7427 3a0a 2020 2020  RangeList':.    
-00012940: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00012950: 6469 6666 6572 656e 6365 5f75 7064 6174  difference_updat
-00012960: 6528 6f74 6865 725f 7265 6629 0a0a 2020  e(other_ref)..  
-00012970: 2020 6465 6620 5f5f 6978 6f72 5f5f 2873    def __ixor__(s
-00012980: 656c 662c 206f 7468 6572 5f72 6566 3a20  elf, other_ref: 
-00012990: 2742 6962 6c65 5265 6627 2920 2d3e 2027  'BibleRef') -> '
-000129a0: 4269 626c 6552 616e 6765 4c69 7374 273a  BibleRangeList':
-000129b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000129c0: 7365 6c66 2e73 796d 5f64 6966 6665 7265  self.sym_differe
-000129d0: 6e63 655f 7570 6461 7465 286f 7468 6572  nce_update(other
-000129e0: 5f72 6566 290a 0a20 2020 2064 6566 205f  _ref)..    def _
-000129f0: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-00012a00: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-00012a10: 4269 626c 6552 616e 6765 4c69 7374 2822  BibleRangeList("
-00012a20: 7b73 656c 662e 7374 7228 297d 2229 270a  {self.str()}")'.
-00012a30: 2020 2020 0a20 2020 2064 6566 205f 5f73      .    def __s
-00012a40: 7472 5f5f 2873 656c 6629 3a0a 2020 2020  tr__(self):.    
-00012a50: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00012a60: 7374 7228 290a 0a20 2020 2064 6566 2072  str()..    def r
-00012a70: 6567 726f 7570 2873 656c 662c 2066 6c61  egroup(self, fla
-00012a80: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-00012a90: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
-00012aa0: 2727 5265 6d6f 7665 7320 7468 6520 6578  ''Removes the ex
-00012ab0: 6973 7469 6e67 2067 726f 7570 7320 696e  isting groups in
-00012ac0: 2074 6865 206c 6973 742c 2061 6e64 2070   the list, and p
-00012ad0: 6c61 6365 7320 7468 6520 6c69 7374 2069  laces the list i
-00012ae0: 7465 6d73 2069 6e74 6f20 7468 6569 7220  tems into their 
-00012af0: 6d6f 7374 206e 6174 7572 616c 206e 6577  most natural new
-00012b00: 2067 726f 7570 696e 6773 2c0a 2020 2020   groupings,.    
-00012b10: 2020 2020 7468 6174 2066 6974 2074 6865      that fit the
-00012b20: 206d 6f73 7420 636f 6e76 656e 7469 6f6e   most convention
-00012b30: 616c 2073 7472 696e 6720 7265 7072 6573  al string repres
-00012b40: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00012b50: 6c69 7374 2e20 2846 6f72 2065 7861 6d70  list. (For examp
-00012b60: 6c65 2c20 7468 6973 2074 7970 6963 616c  le, this typical
-00012b70: 6c79 0a20 2020 2020 2020 2070 6c61 6365  ly.        place
-00012b80: 7320 7261 6e67 6573 2069 6e20 6469 6666  s ranges in diff
-00012b90: 6572 656e 7420 6368 6170 7465 7273 2069  erent chapters i
-00012ba0: 6e74 6f20 6469 6666 6572 656e 7420 6772  nto different gr
-00012bb0: 6f75 7073 2e29 0a20 2020 2020 2020 2027  oups.).        '
-00012bc0: 2727 0a20 2020 2020 2020 2023 2054 6869  ''.        # Thi
-00012bd0: 7320 6d65 7468 6f64 2069 7320 6465 7269  s method is deri
-00012be0: 7665 6420 6672 6f6d 2074 6865 2073 7472  ved from the str
-00012bf0: 2829 206d 6574 686f 6420 6265 6c6f 772c  () method below,
-00012c00: 2061 6e64 2069 7320 6265 7374 2072 6561   and is best rea
-00012c10: 6420 6166 7465 7220 7468 6174 206d 6574  d after that met
-00012c20: 686f 642e 0a20 2020 2020 2020 2023 2043  hod..        # C
-00012c30: 6861 6e67 6573 2074 6f20 7468 6520 696e  hanges to the in
-00012c40: 7465 726e 616c 206c 6f67 6963 206f 6620  ternal logic of 
-00012c50: 7374 7228 2920 6c69 6b65 6c79 2072 6571  str() likely req
-00012c60: 7569 7265 2063 6f72 7265 7370 6f6e 6469  uire correspondi
-00012c70: 6e67 2063 6861 6e67 6573 2074 6f20 7468  ng changes to th
-00012c80: 6520 696e 7465 726e 616c 206c 6f67 6963  e internal logic
-00012c90: 206f 660a 2020 2020 2020 2020 2320 7468   of.        # th
-00012ca0: 6973 206d 6574 686f 642e 0a20 2020 2020  is method..     
-00012cb0: 2020 2073 656c 662e 636c 6561 725f 6772     self.clear_gr
-00012cc0: 6f75 7073 2829 0a0a 2020 2020 2020 2020  oups()..        
-00012cd0: 6375 725f 626f 6f6b 203d 204e 6f6e 650a  cur_book = None.
-00012ce0: 2020 2020 2020 2020 6375 725f 6368 6170          cur_chap
-00012cf0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00012d00: 6174 5f76 6572 7365 5f6c 6576 656c 203d  at_verse_level =
-00012d10: 2046 616c 7365 0a20 2020 2020 2020 2073   False.        s
-00012d20: 686f 775f 7374 6172 745f 7665 7273 6520  how_start_verse 
-00012d30: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00012d40: 0a20 2020 2020 2020 2066 6f72 206e 6f64  .        for nod
-00012d50: 6520 696e 2073 656c 662e 5f6e 6f64 655f  e in self._node_
-00012d60: 6974 6572 2829 3a0a 2020 2020 2020 2020  iter():.        
-00012d70: 2020 2020 6269 626c 655f 7261 6e67 653a      bible_range:
-00012d80: 2042 6962 6c65 5261 6e67 6520 3d20 6e6f   BibleRange = no
-00012d90: 6465 2e76 616c 7565 2020 2020 2020 2020  de.value        
-00012da0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00012db0: 2020 2020 2069 6620 6269 626c 655f 7261       if bible_ra
-00012dc0: 6e67 652e 7370 616e 735f 7374 6172 745f  nge.spans_start_
-00012dd0: 626f 6f6b 2866 6c61 6773 293a 2023 2052  book(flags): # R
-00012de0: 616e 6765 2073 7461 7274 2069 6e63 6c75  ange start inclu
-00012df0: 6465 7320 616e 2065 6e74 6972 6520 626f  des an entire bo
-00012e00: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
-00012e10: 2020 2023 2045 7665 6e20 6966 2061 6c72     # Even if alr
-00012e20: 6561 6479 2069 6e20 7361 6d65 2062 6f6f  eady in same boo
-00012e30: 6b2c 2077 686f 6c65 2062 6f6f 6b20 7265  k, whole book re
-00012e40: 6665 7265 6e63 6573 2072 6570 6561 7420  ferences repeat 
-00012e50: 7468 6520 7768 6f6c 6520 626f 6f6b 206e  the whole book n
-00012e60: 616d 652e 0a20 2020 2020 2020 2020 2020  ame..           
-00012e70: 2020 2020 2073 656c 662e 5f69 6e73 6572       self._inser
-00012e80: 745f 6e65 775f 6772 6f75 705f 6174 5f6e  t_new_group_at_n
-00012e90: 6f64 6528 6e6f 6465 290a 2020 2020 2020  ode(node).      
-00012ea0: 2020 2020 2020 2020 2020 6375 725f 626f            cur_bo
-00012eb0: 6f6b 203d 2062 6962 6c65 5f72 616e 6765  ok = bible_range
-00012ec0: 2e73 7461 7274 2e62 6f6f 6b0a 2020 2020  .start.book.    
-00012ed0: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
-00012ee0: 6368 6170 203d 204e 6f6e 650a 2020 2020  chap = None.    
-00012ef0: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
-00012f00: 6572 7365 5f6c 6576 656c 203d 2046 616c  erse_level = Fal
-00012f10: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00012f20: 2020 2073 686f 775f 7374 6172 745f 7665     show_start_ve
-00012f30: 7273 6520 3d20 4661 6c73 650a 2020 2020  rse = False.    
-00012f40: 2020 2020 2020 2020 656c 6966 2062 6962          elif bib
-00012f50: 6c65 5f72 616e 6765 2e73 7061 6e73 5f73  le_range.spans_s
-00012f60: 7461 7274 5f63 6861 7028 666c 6167 7329  tart_chap(flags)
-00012f70: 3a20 2320 5261 6e67 6520 7374 6172 7420  : # Range start 
-00012f80: 696e 636c 7564 6573 2061 6e20 656e 7469  includes an enti
-00012f90: 7265 2063 6861 700a 2020 2020 2020 2020  re chap.        
-00012fa0: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
-00012fb0: 7365 7274 5f6e 6577 5f67 726f 7570 5f61  sert_new_group_a
-00012fc0: 745f 6e6f 6465 286e 6f64 6529 0a20 2020  t_node(node).   
-00012fd0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012fe0: 5f63 6861 7020 3d20 6269 626c 655f 7261  _chap = bible_ra
-00012ff0: 6e67 652e 7374 6172 742e 6368 6170 5f6e  nge.start.chap_n
-00013000: 756d 0a20 2020 2020 2020 2020 2020 2020  um.             
-00013010: 2020 2061 745f 7665 7273 655f 6c65 7665     at_verse_leve
-00013020: 6c20 3d20 4661 6c73 650a 2020 2020 2020  l = False.      
-00013030: 2020 2020 2020 2020 2020 7368 6f77 5f73            show_s
-00013040: 7461 7274 5f76 6572 7365 203d 2046 616c  tart_verse = Fal
-00013050: 7365 0a20 2020 2020 2020 2020 2020 2065  se.            e
-00013060: 6c73 653a 2023 2052 616e 6765 2073 7461  lse: # Range sta
-00013070: 7274 2069 7320 6a75 7374 2061 2070 6172  rt is just a par
-00013080: 7469 6375 6c61 7220 7665 7273 650a 2020  ticular verse.  
-00013090: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000130a0: 2063 7572 5f62 6f6f 6b20 3d3d 2062 6962   cur_book == bib
-000130b0: 6c65 5f72 616e 6765 2e73 7461 7274 2e62  le_range.start.b
-000130c0: 6f6f 6b3a 2023 2043 6f6e 7469 6e75 696e  ook: # Continuin
-000130d0: 6720 7361 6d65 2062 6f6f 6b0a 2020 2020  g same book.    
-000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 6966 2028 6e6f 7420 6174 5f76 6572 7365  if (not at_verse
-00013100: 5f6c 6576 656c 2920 6f72 2028 6375 725f  _level) or (cur_
-00013110: 6368 6170 2021 3d20 6269 626c 655f 7261  chap != bible_ra
-00013120: 6e67 652e 7374 6172 742e 6368 6170 5f6e  nge.start.chap_n
-00013130: 756d 2920 6f72 205c 0a20 2020 2020 2020  um) or \.       
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2862 6962 6c65 5f72 616e 6765 2e63 6861  (bible_range.cha
-00013160: 705f 636f 756e 7428 666c 6167 733d 666c  p_count(flags=fl
-00013170: 6167 7329 203e 2031 293a 0a20 2020 2020  ags) > 1):.     
-00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2023 2041 7420 6368 6170 206c 6576     # At chap lev
-000131a0: 656c 206f 7220 7665 7273 6520 6c65 7665  el or verse leve
-000131b0: 6c20 696e 2061 2064 6966 6665 7265 6e74  l in a different
-000131c0: 2063 6861 700a 2020 2020 2020 2020 2020   chap.          
-000131d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000131e0: 6c66 2e5f 696e 7365 7274 5f6e 6577 5f67  lf._insert_new_g
-000131f0: 726f 7570 5f61 745f 6e6f 6465 286e 6f64  roup_at_node(nod
-00013200: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00013210: 2020 2065 6c73 653a 2023 2044 6966 6665     else: # Diffe
-00013220: 7265 6e74 2062 6f6f 6b0a 2020 2020 2020  rent book.      
-00013230: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013240: 6c66 2e5f 696e 7365 7274 5f6e 6577 5f67  lf._insert_new_g
-00013250: 726f 7570 5f61 745f 6e6f 6465 286e 6f64  roup_at_node(nod
-00013260: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00013270: 2020 2063 7572 5f63 6861 7020 3d20 6269     cur_chap = bi
-00013280: 626c 655f 7261 6e67 652e 7374 6172 742e  ble_range.start.
-00013290: 6368 6170 5f6e 756d 0a20 2020 2020 2020  chap_num.       
-000132a0: 2020 2020 2020 2020 2061 745f 7665 7273           at_vers
-000132b0: 655f 6c65 7665 6c20 3d20 5472 7565 2023  e_level = True #
-000132c0: 2041 6c6c 2073 696e 676c 6520 7665 7273   All single vers
-000132d0: 6573 206d 6f76 6520 7573 2074 6f20 7665  es move us to ve
-000132e0: 7273 6520 6c65 7665 6c0a 2020 2020 2020  rse level.      
-000132f0: 2020 2020 2020 2020 2020 7368 6f77 5f73            show_s
-00013300: 7461 7274 5f76 6572 7365 203d 2054 7275  tart_verse = Tru
-00013310: 650a 0a20 2020 2020 2020 2020 2020 2063  e..            c
-00013320: 7572 5f62 6f6f 6b20 3d20 6269 626c 655f  ur_book = bible_
-00013330: 7261 6e67 652e 7374 6172 742e 626f 6f6b  range.start.book
-00013340: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013350: 286e 6f74 2073 686f 775f 7374 6172 745f  (not show_start_
-00013360: 7665 7273 6529 2061 6e64 2028 6e6f 7420  verse) and (not 
-00013370: 6269 626c 655f 7261 6e67 652e 7370 616e  bible_range.span
-00013380: 735f 656e 645f 6368 6170 2829 293a 0a20  s_end_chap()):. 
-00013390: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000133a0: 2045 6e64 2076 6572 7365 2077 696c 6c20   End verse will 
-000133b0: 7368 6f77 2076 6572 7365 206e 756d 2c20  show verse num, 
-000133c0: 616e 6420 7765 2776 6520 6265 656e 2061  and we've been a
-000133d0: 736b 6564 2074 6f20 7368 6f77 2073 7461  sked to show sta
-000133e0: 7274 2076 6572 7365 206e 756d 2069 6e20  rt verse num in 
-000133f0: 7375 6368 2063 6173 6573 0a20 2020 2020  such cases.     
-00013400: 2020 2020 2020 2020 2020 2073 686f 775f             show_
-00013410: 7374 6172 745f 7665 7273 6520 3d20 5472  start_verse = Tr
-00013420: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00013430: 2020 2061 745f 7665 7273 655f 6c65 7665     at_verse_leve
-00013440: 6c20 3d20 5472 7565 0a0a 2020 2020 2020  l = True..      
-00013450: 2020 2020 2020 6966 2028 6e6f 7420 6269        if (not bi
-00013460: 626c 655f 7261 6e67 652e 6973 5f77 686f  ble_range.is_who
-00013470: 6c65 5f62 6f6f 6b28 666c 6167 7329 2920  le_book(flags)) 
-00013480: 616e 6420 286e 6f74 2062 6962 6c65 5f72  and (not bible_r
-00013490: 616e 6765 2e69 735f 7768 6f6c 655f 6368  ange.is_whole_ch
-000134a0: 6170 2866 6c61 6773 2929 2061 6e64 205c  ap(flags)) and \
-000134b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000134c0: 286e 6f74 2062 6962 6c65 5f72 616e 6765  (not bible_range
-000134d0: 2e69 735f 7369 6e67 6c65 5f76 6572 7365  .is_single_verse
-000134e0: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-000134f0: 2020 2020 2069 6620 6269 626c 655f 7261       if bible_ra
-00013500: 6e67 652e 656e 642e 626f 6f6b 2021 3d20  nge.end.book != 
-00013510: 6269 626c 655f 7261 6e67 652e 7374 6172  bible_range.star
-00013520: 742e 626f 6f6b 3a0a 2020 2020 2020 2020  t.book:.        
-00013530: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
-00013540: 6572 7365 5f6c 6576 656c 203d 2046 616c  erse_level = Fal
-00013550: 7365 0a0a 2020 2020 2020 2020 2020 2020  se..            
-00013560: 2020 2020 6966 2062 6962 6c65 5f72 616e      if bible_ran
-00013570: 6765 2e73 7061 6e73 5f65 6e64 5f62 6f6f  ge.spans_end_boo
-00013580: 6b28 666c 6167 7329 3a20 2320 5261 6e67  k(flags): # Rang
-00013590: 6520 656e 6420 696e 636c 7564 6573 2061  e end includes a
-000135a0: 6e20 656e 7469 7265 2062 6f6f 6b0a 2020  n entire book.  
-000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135c0: 2020 6375 725f 6368 6170 203d 204e 6f6e    cur_chap = Non
-000135d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000135e0: 2020 2020 2020 6174 5f76 6572 7365 5f6c        at_verse_l
-000135f0: 6576 656c 203d 2046 616c 7365 0a20 2020  evel = False.   
-00013600: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00013610: 6620 6e6f 7420 6174 5f76 6572 7365 5f6c  f not at_verse_l
-00013620: 6576 656c 2061 6e64 2062 6962 6c65 5f72  evel and bible_r
-00013630: 616e 6765 2e73 7061 6e73 5f65 6e64 5f63  ange.spans_end_c
-00013640: 6861 7028 666c 6167 7329 3a20 2320 5261  hap(flags): # Ra
-00013650: 6e67 6520 656e 6420 696e 636c 7564 6573  nge end includes
-00013660: 2061 6e20 656e 7469 7265 2063 6861 700a   an entire chap.
-00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013680: 2020 2020 6375 725f 6368 6170 203d 2062      cur_chap = b
-00013690: 6962 6c65 5f72 616e 6765 2e65 6e64 2e63  ible_range.end.c
-000136a0: 6861 705f 6e75 6d0a 2020 2020 2020 2020  hap_num.        
-000136b0: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
-000136c0: 6572 7365 5f6c 6576 656c 203d 2046 616c  erse_level = Fal
-000136d0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-000136e0: 2020 2065 6c73 653a 2023 2052 616e 6765     else: # Range
-000136f0: 2065 6e64 2069 7320 6120 7768 6f6c 6520   end is a whole 
-00013700: 6368 6170 2061 6674 6572 2061 2070 6172  chap after a par
-00013710: 7469 6375 6c61 7220 7665 7273 652c 206f  ticular verse, o
-00013720: 7220 6120 7061 7274 6963 756c 6172 2076  r a particular v
-00013730: 6572 7365 0a20 2020 2020 2020 2020 2020  erse.           
-00013740: 2020 2020 2020 2020 2063 7572 5f63 6861           cur_cha
-00013750: 7020 3d20 6269 626c 655f 7261 6e67 652e  p = bible_range.
-00013760: 656e 642e 6368 6170 5f6e 756d 0a20 2020  end.chap_num.   
-00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 2061 745f 7665 7273 655f 6c65 7665 6c20   at_verse_level 
-00013790: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-000137a0: 2020 2020 2020 2063 7572 5f62 6f6f 6b20         cur_book 
-000137b0: 3d20 6269 626c 655f 7261 6e67 652e 656e  = bible_range.en
-000137c0: 642e 626f 6f6b 0a0a 2020 2020 6465 6620  d.book..    def 
-000137d0: 7374 7228 7365 6c66 2c20 6162 6272 6576  str(self, abbrev
-000137e0: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-000137f0: 616c 745f 7365 703a 2062 6f6f 6c20 3d20  alt_sep: bool = 
-00013800: 4661 6c73 652c 206e 6f73 7061 6365 3a20  False, nospace: 
-00013810: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00013820: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00013830: 7365 7276 655f 6772 6f75 7073 3a20 626f  serve_groups: bo
-00013840: 6f6c 203d 2054 7275 652c 2066 6f72 6365  ol = True, force
-00013850: 5f73 7461 7274 5f76 6572 7365 733a 2062  _start_verses: b
-00013860: 6f6f 6c20 3d20 4661 6c73 652c 2066 6c61  ool = False, fla
-00013870: 6773 3a20 4269 626c 6546 6c61 6720 3d20  gs: BibleFlag = 
-00013880: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
-00013890: 2727 5265 7475 726e 7320 6120 636f 6e66  ''Returns a conf
-000138a0: 6967 7572 6174 626c 6520 7374 7269 6e67  iguratble string
-000138b0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-000138c0: 6f66 2074 6869 7320 4269 626c 6552 616e  of this BibleRan
-000138d0: 6765 4c69 7374 2c20 6173 2066 6f6c 6c6f  geList, as follo
-000138e0: 7773 3a0a 0a20 2020 2020 2020 202d 2049  ws:..        - I
-000138f0: 6620 6061 6262 7265 7660 2069 7320 6054  f `abbrev` is `T
-00013900: 7275 6560 2c20 7468 6520 6162 6272 6576  rue`, the abbrev
-00013910: 6961 7465 6420 6e61 6d65 206f 6620 7468  iated name of th
-00013920: 6520 626f 6f6b 2069 7320 7573 6564 2028  e book is used (
-00013930: 696e 7374 6561 6420 6f66 2074 6865 2066  instead of the f
-00013940: 756c 6c20 6e61 6d65 292e 0a20 2020 2020  ull name)..     
-00013950: 2020 202d 2049 6620 6061 6c74 5f73 6570     - If `alt_sep
-00013960: 6020 6973 2060 5472 7565 602c 2063 6861  ` is `True`, cha
-00013970: 7074 6572 2061 6e64 2076 6572 7365 206e  pter and verse n
-00013980: 756d 6265 7273 2061 7265 2073 6570 6172  umbers are separ
-00013990: 6174 6564 2062 7920 7468 6520 616c 7465  ated by the alte
-000139a0: 726e 6174 650a 2020 2020 2020 2020 2020  rnate.          
-000139b0: 7365 7061 7261 746f 7220 2864 6566 6175  separator (defau
-000139c0: 6c74 7320 746f 2060 2e60 2920 696e 7374  lts to `.`) inst
-000139d0: 6561 6420 6f66 2074 6865 2073 7461 6e64  ead of the stand
-000139e0: 6172 6420 7365 7061 7261 746f 7220 2864  ard separator (d
-000139f0: 6566 6175 6c74 7320 746f 2060 3a60 292e  efaults to `:`).
-00013a00: 0a20 2020 2020 2020 202d 2049 6620 606e  .        - If `n
-00013a10: 6f73 7061 6365 6020 6973 2060 5472 7565  ospace` is `True
-00013a20: 602c 206e 6f20 7370 6163 6573 2061 7265  `, no spaces are
-00013a30: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
-00013a40: 2073 7472 696e 672e 0a20 2020 2020 2020   string..       
-00013a50: 202d 2049 6620 6070 7265 7365 7276 655f   - If `preserve_
-00013a60: 6772 6f75 7073 6020 6973 2060 5472 7565  groups` is `True
-00013a70: 602c 2074 6865 206d 616a 6f72 2067 726f  `, the major gro
-00013a80: 7570 2073 6570 6172 6174 6f72 2069 7320  up separator is 
-00013a90: 616c 7761 7973 2075 7365 6420 6265 7477  always used betw
-00013aa0: 6565 6e20 6772 6f75 7073 2c0a 2020 2020  een groups,.    
-00013ab0: 2020 2020 2020 616e 6420 6f6e 6c79 2062        and only b
-00013ac0: 6574 7765 656e 2067 726f 7570 732c 2077  etween groups, w
-00013ad0: 6974 6820 7468 6520 6d69 6e6f 7220 6772  ith the minor gr
-00013ae0: 6f75 7020 7365 7061 7261 746f 7220 7573  oup separator us
-00013af0: 6564 2065 7863 6c75 7369 7665 6c79 2077  ed exclusively w
-00013b00: 6974 6869 6e0a 2020 2020 2020 2020 2020  ithin.          
-00013b10: 6772 6f75 7073 2e20 5061 7273 696e 6720  groups. Parsing 
-00013b20: 7468 6520 7265 7375 6c74 696e 6720 7374  the resulting st
-00013b30: 7269 6e67 2073 686f 756c 6420 7969 656c  ring should yiel
-00013b40: 6420 616e 2065 7175 6976 616c 656e 7420  d an equivalent 
-00013b50: 6042 6962 6c65 5261 6e67 654c 6973 7460  `BibleRangeList`
-00013b60: 2e0a 2020 2020 2020 2020 2d20 4966 2060  ..        - If `
-00013b70: 7072 6573 6572 7665 5f67 726f 7570 7360  preserve_groups`
-00013b80: 2069 7320 6046 616c 7365 602c 206d 616a   is `False`, maj
-00013b90: 6f72 2061 6e64 206d 696e 6f72 2067 726f  or and minor gro
-00013ba0: 7570 2073 6570 6172 6174 6f72 7320 6172  up separators ar
-00013bb0: 6520 7573 6564 2061 7320 6e65 6365 7373  e used as necess
-00013bc0: 6172 790a 2020 2020 2020 2020 2020 746f  ary.          to
-00013bd0: 2063 7265 6174 6520 7468 6520 6d6f 7374   create the most
-00013be0: 2063 6f6e 7665 6e74 696f 6e61 6c20 7265   conventional re
-00013bf0: 7375 6c74 696e 6720 7374 7269 6e67 2c20  sulting string, 
-00013c00: 7768 6963 6820 6d61 7920 7265 7375 6c74  which may result
-00013c10: 2069 6e20 6469 6666 6572 656e 740a 2020   in different.  
-00013c20: 2020 2020 2020 2020 7061 7373 6167 6520          passage 
-00013c30: 6772 6f75 7069 6e67 732e 0a20 2020 2020  groupings..     
-00013c40: 2020 202d 2049 6620 6066 6f72 6365 5f73     - If `force_s
-00013c50: 7461 7274 5f76 6572 7365 7360 2069 7320  tart_verses` is 
-00013c60: 6054 7275 6560 2c20 7468 6520 7374 6172  `True`, the star
-00013c70: 7420 7665 7273 6520 6e75 6d62 6572 206f  t verse number o
-00013c80: 6620 6120 7261 6e67 6520 6973 206d 6164  f a range is mad
-00013c90: 6520 6578 706c 6963 6974 2069 6620 7468  e explicit if th
-00013ca0: 6520 656e 640a 2020 2020 2020 2020 2020  e end.          
-00013cb0: 7665 7273 6520 6f66 2074 6865 2072 616e  verse of the ran
-00013cc0: 6765 2069 7320 616c 736f 2062 6569 6e67  ge is also being
-00013cd0: 2073 686f 776e 2e20 4f74 6865 7277 6973   shown. Otherwis
-00013ce0: 652c 2074 6865 2073 7461 7274 2076 6572  e, the start ver
-00013cf0: 7365 206e 756d 6265 7220 6973 206f 6d69  se number is omi
-00013d00: 7474 6564 2077 6865 7265 7665 7220 706f  tted wherever po
-00013d10: 7373 6962 6c65 2e0a 2020 2020 2020 2020  ssible..        
-00013d20: 2727 270a 2020 2020 2020 2020 2320 5468  '''.        # Th
-00013d30: 6520 7265 6772 6f75 7028 2920 6d65 7468  e regroup() meth
-00013d40: 6f64 2069 7320 6465 7269 7665 6420 6672  od is derived fr
-00013d50: 6f6d 2074 6869 7320 7374 7228 2920 6d65  om this str() me
-00013d60: 7468 6f64 2e20 4368 616e 6765 7320 746f  thod. Changes to
-00013d70: 2074 6865 2069 6e74 6572 6e61 6c20 6c6f   the internal lo
-00013d80: 6769 6320 6f66 2074 6869 7320 6d65 7468  gic of this meth
-00013d90: 6f64 0a20 2020 2020 2020 2023 206c 696b  od.        # lik
-00013da0: 656c 7920 7265 7175 6972 6520 636f 7272  ely require corr
-00013db0: 6573 706f 6e64 696e 6720 6368 616e 6765  esponding change
-00013dc0: 7320 746f 2074 6865 2069 6e74 6572 6e61  s to the interna
-00013dd0: 6c20 6c6f 6769 6320 6f66 2072 6567 726f  l logic of regro
-00013de0: 7570 2829 2e0a 0a20 2020 2020 2020 2063  up()...        c
-00013df0: 7572 5f62 6f6f 6b20 3d20 4e6f 6e65 0a20  ur_book = None. 
-00013e00: 2020 2020 2020 2063 7572 5f63 6861 7020         cur_chap 
-00013e10: 3d20 4e6f 6e65 0a20 2020 2020 2020 2061  = None.        a
-00013e20: 745f 7665 7273 655f 6c65 7665 6c20 3d20  t_verse_level = 
-00013e30: 4661 6c73 650a 2020 2020 2020 2020 6669  False.        fi
-00013e40: 7273 745f 7261 6e67 6520 3d20 5472 7565  rst_range = True
-00013e50: 0a20 2020 2020 2020 206c 6973 745f 7365  .        list_se
-00013e60: 7020 3d20 2222 0a20 2020 2020 2020 2072  p = "".        r
-00013e70: 6573 756c 745f 7374 7220 3d20 2222 0a20  esult_str = "". 
-00013e80: 2020 2020 2020 2066 6f72 6365 5f64 7561         force_dua
-00013e90: 6c5f 7265 6620 3d20 4661 6c73 6520 2320  l_ref = False # 
-00013ea0: 5472 7565 2069 6620 7765 2072 6571 7569  True if we requi
-00013eb0: 7265 2061 2073 696e 676c 6520 7265 6665  re a single refe
-00013ec0: 7265 6e63 6520 746f 2064 6973 706c 6179  rence to display
-00013ed0: 2061 7320 6120 6475 616c 5f72 6566 6572   as a dual_refer
-00013ee0: 656e 6365 5f72 616e 6765 0a0a 2020 2020  ence_range..    
-00013ef0: 2020 2020 666f 7220 6772 6f75 7020 696e      for group in
-00013f00: 2073 656c 662e 6772 6f75 7073 3a0a 2020   self.groups:.  
-00013f10: 2020 2020 2020 2020 2020 666f 7220 6269            for bi
-00013f20: 626c 655f 7261 6e67 6520 696e 2067 726f  ble_range in gro
-00013f30: 7570 3a0a 2020 2020 2020 2020 2020 2020  up:.            
-00013f40: 2020 2020 6269 626c 655f 7261 6e67 653a      bible_range:
-00013f50: 2042 6962 6c65 5261 6e67 6520 3d20 6269   BibleRange = bi
-00013f60: 626c 655f 7261 6e67 6520 2320 5479 7065  ble_range # Type
-00013f70: 6361 7374 2020 2020 2020 2020 2020 2020  cast            
-00013f80: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00013f90: 2020 2020 2069 6620 6269 626c 655f 7261       if bible_ra
-00013fa0: 6e67 652e 7370 616e 735f 7374 6172 745f  nge.spans_start_
-00013fb0: 626f 6f6b 2866 6c61 6773 293a 2023 2052  book(flags): # R
-00013fc0: 616e 6765 2073 7461 7274 2069 6e63 6c75  ange start inclu
-00013fd0: 6465 7320 616e 2065 6e74 6972 6520 626f  des an entire bo
-00013fe0: 6f6b 0a20 2020 2020 2020 2020 2020 2020  ok.             
-00013ff0: 2020 2020 2020 2023 2045 7665 6e20 6966         # Even if
-00014000: 2061 6c72 6561 6479 2069 6e20 7361 6d65   already in same
-00014010: 2062 6f6f 6b2c 2077 686f 6c65 2062 6f6f   book, whole boo
-00014020: 6b20 7265 6665 7265 6e63 6573 2072 6570  k references rep
-00014030: 6561 7420 7468 6520 7768 6f6c 6520 626f  eat the whole bo
-00014040: 6f6b 206e 616d 652e 0a20 2020 2020 2020  ok name..       
-00014050: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00014060: 7274 5f70 6172 7473 203d 2042 6962 6c65  rt_parts = Bible
-00014070: 5665 7273 6550 6172 742e 424f 4f4b 0a20  VersePart.BOOK. 
-00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2063 7572 5f62 6f6f 6b20 3d20 6269     cur_book = bi
-000140a0: 626c 655f 7261 6e67 652e 7374 6172 742e  ble_range.start.
-000140b0: 626f 6f6b 0a20 2020 2020 2020 2020 2020  book.           
-000140c0: 2020 2020 2020 2020 2063 7572 5f63 6861           cur_cha
-000140d0: 7020 3d20 4e6f 6e65 0a20 2020 2020 2020  p = None.       
-000140e0: 2020 2020 2020 2020 2020 2020 2061 745f               at_
-000140f0: 7665 7273 655f 6c65 7665 6c20 3d20 4661  verse_level = Fa
-00014100: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014110: 2020 2020 2020 2020 6966 206e 6f74 2070          if not p
-00014120: 7265 7365 7276 655f 6772 6f75 7073 3a0a  reserve_groups:.
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2020 2020 2020 6c69 7374 5f73 6570          list_sep
-00014150: 203d 2062 6962 6c65 5f64 6174 6128 292e   = bible_data().
-00014160: 6d61 6a6f 725f 6c69 7374 5f73 6570 0a20  major_list_sep. 
-00014170: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00014180: 6c69 6620 6269 626c 655f 7261 6e67 652e  lif bible_range.
-00014190: 7370 616e 735f 7374 6172 745f 6368 6170  spans_start_chap
-000141a0: 2866 6c61 6773 293a 2023 2052 616e 6765  (flags): # Range
-000141b0: 2073 7461 7274 2069 6e63 6c75 6465 7320   start includes 
-000141c0: 616e 2065 6e74 6972 6520 6368 6170 0a20  an entire chap. 
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2020 2069 6620 6375 725f 626f 6f6b 203d     if cur_book =
-000141f0: 3d20 6269 626c 655f 7261 6e67 652e 7374  = bible_range.st
-00014200: 6172 742e 626f 6f6b 3a20 2320 436f 6e74  art.book: # Cont
-00014210: 696e 7569 6e67 2073 616d 6520 626f 6f6b  inuing same book
-00014220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014230: 2020 2020 2020 2020 2069 6620 6174 5f76           if at_v
-00014240: 6572 7365 5f6c 6576 656c 3a20 2320 5765  erse_level: # We
-00014250: 2772 6520 696e 2061 206c 6973 7420 6f66  're in a list of
-00014260: 2076 6572 7365 730a 2020 2020 2020 2020   verses.        
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 2020 2020 6966 206e 6f74 2070 7265 7365      if not prese
-00014290: 7276 655f 6772 6f75 7073 3a20 2320 5573  rve_groups: # Us
-000142a0: 6520 6d61 6a6f 7220 6c69 7374 2073 6570  e major list sep
-000142b0: 2074 6f20 7265 7475 726e 2074 6f20 6368   to return to ch
-000142c0: 6170 7465 7273 0a20 2020 2020 2020 2020  apters.         
-000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142e0: 2020 2020 2020 206c 6973 745f 7365 7020         list_sep 
-000142f0: 3d20 6269 626c 655f 6461 7461 2829 2e6d  = bible_data().m
-00014300: 616a 6f72 5f6c 6973 745f 7365 700a 2020  ajor_list_sep.  
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00014330: 6172 745f 7061 7274 7320 3d20 4269 626c  art_parts = Bibl
-00014340: 6556 6572 7365 5061 7274 2e43 4841 500a  eVersePart.CHAP.
-00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 6174 5f76 6572 7365 5f6c 6576 656c 203d  at_verse_level =
-00014380: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 2020 2065 6c73 653a 2023 2050 7265 7365     else: # Prese
-000143b0: 7276 696e 6720 6772 6f75 7073 0a20 2020  rving groups.   
-000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000143e0: 6c69 7374 5f73 6570 203d 3d20 6269 626c  list_sep == bibl
-000143f0: 655f 6461 7461 2829 2e6d 616a 6f72 5f6c  e_data().major_l
-00014400: 6973 745f 7365 703a 0a20 2020 2020 2020  ist_sep:.       
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2020 2020 2020 2020 2020 2023 2057               # W
-00014430: 6527 7265 2073 7472 6169 6768 7420 6166  e're straight af
-00014440: 7465 7220 6120 6d61 6a6f 7220 6c69 7374  ter a major list
-00014450: 2072 6566 2c20 736f 206d 7573 7420 7265   ref, so must re
-00014460: 7475 726e 2074 6f20 6368 6170 206c 6576  turn to chap lev
-00014470: 656c 0a20 2020 2020 2020 2020 2020 2020  el.             
-00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014490: 2020 2020 2020 2073 7461 7274 5f70 6172         start_par
-000144a0: 7473 203d 2042 6962 6c65 5665 7273 6550  ts = BibleVerseP
-000144b0: 6172 742e 4348 4150 0a20 2020 2020 2020  art.CHAP.       
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144d0: 2020 2020 2020 2020 2020 2020 2061 745f               at_
-000144e0: 7665 7273 655f 6c65 7665 6c20 3d20 4661  verse_level = Fa
-000144f0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014510: 2020 2020 656c 7365 3a20 2320 5765 2772      else: # We'r
-00014520: 6520 6166 7465 7220 6120 6d69 6e6f 7220  e after a minor 
-00014530: 6c69 7374 2072 6566 2c20 736f 2077 6520  list ref, so we 
-00014540: 6361 6e27 7420 7265 7475 726e 2074 6f20  can't return to 
-00014550: 6368 6170 206c 6576 656c 2c0a 2020 2020  chap level,.    
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2020 2320 736f 2077 6520 666f 7263 6520    # so we force 
-00014590: 6469 7370 6c61 7920 7468 6520 7768 6f6c  display the whol
-000145a0: 6520 7261 6e67 650a 2020 2020 2020 2020  e range.        
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-000145d0: 745f 7061 7274 7320 3d20 4269 626c 6556  t_parts = BibleV
-000145e0: 6572 7365 5061 7274 2e43 4841 505f 5645  ersePart.CHAP_VE
-000145f0: 5253 450a 2020 2020 2020 2020 2020 2020  RSE.            
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 2020 2020 2020 2020 6174 5f76 6572 7365          at_verse
-00014620: 5f6c 6576 656c 203d 2054 7275 650a 2020  _level = True.  
-00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014650: 2020 666f 7263 655f 6475 616c 5f72 6566    force_dual_ref
-00014660: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014680: 656c 7365 3a20 2320 5765 2772 6520 696e  else: # We're in
-00014690: 2061 206c 6973 7420 6f66 2063 6861 7074   a list of chapt
-000146a0: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 6966 206e 6f74 2070 7265 7365 7276 655f  if not preserve_
-000146d0: 6772 6f75 7073 3a20 2320 5573 6520 6d61  groups: # Use ma
-000146e0: 6a6f 7220 6c69 7374 2073 6570 2062 6574  jor list sep bet
-000146f0: 7765 656e 2063 6861 7074 6572 730a 2020  ween chapters.  
-00014700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014710: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00014720: 7374 5f73 6570 203d 2062 6962 6c65 5f64  st_sep = bible_d
-00014730: 6174 6128 292e 6d61 6a6f 725f 6c69 7374  ata().major_list
-00014740: 5f73 6570 0a20 2020 2020 2020 2020 2020  _sep.           
-00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2020 2020 2073 7461 7274 5f70 6172 7473       start_parts
-00014770: 203d 2042 6962 6c65 5665 7273 6550 6172   = BibleVersePar
-00014780: 742e 4348 4150 0a20 2020 2020 2020 2020  t.CHAP.         
-00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147a0: 2020 2020 2020 2061 745f 7665 7273 655f         at_verse_
-000147b0: 6c65 7665 6c20 3d20 4661 6c73 650a 2020  level = False.  
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-000147e0: 2320 5072 6573 6572 7669 6e67 2067 726f  # Preserving gro
-000147f0: 7570 730a 2020 2020 2020 2020 2020 2020  ups.            
-00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014810: 2020 2020 6966 206c 6973 745f 7365 7020      if list_sep 
-00014820: 3d3d 2062 6962 6c65 5f64 6174 6128 292e  == bible_data().
-00014830: 6d61 6a6f 725f 6c69 7374 5f73 6570 3a0a  major_list_sep:.
-00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014860: 2020 2020 2320 5765 2772 6520 7374 7261      # We're stra
-00014870: 6967 6874 2061 6674 6572 2061 206d 616a  ight after a maj
-00014880: 6f72 206c 6973 7420 7265 662c 2073 6f20  or list ref, so 
-00014890: 6361 6e20 7265 7475 726e 2074 6f20 6368  can return to ch
-000148a0: 6170 206c 6576 656c 0a20 2020 2020 2020  ap level.       
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-000148d0: 7274 5f70 6172 7473 203d 2042 6962 6c65  rt_parts = Bible
-000148e0: 5665 7273 6550 6172 742e 4348 4150 0a20  VersePart.CHAP. 
-000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2061 745f 7665 7273 655f 6c65 7665     at_verse_leve
-00014920: 6c20 3d20 4661 6c73 650a 2020 2020 2020  l = False.      
-00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014940: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-00014950: 2320 5765 2772 6520 6166 7465 7220 6120  # We're after a 
-00014960: 6d69 6e6f 7220 6c69 7374 2072 6566 0a20  minor list ref. 
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014990: 2020 2069 6620 6269 626c 655f 7261 6e67     if bible_rang
-000149a0: 652e 7370 616e 735f 656e 645f 6368 6170  e.spans_end_chap
-000149b0: 2866 6c61 6773 293a 0a20 2020 2020 2020  (flags):.       
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149e0: 2023 2054 6869 7320 7261 6e67 6520 6973   # This range is
-000149f0: 2061 2077 686f 6c65 2073 6574 206f 6620   a whole set of 
-00014a00: 6368 6170 7465 7273 2c20 736f 206a 7573  chapters, so jus
-00014a10: 7420 6469 7370 6c61 7920 6368 6170 7465  t display chapte
-00014a20: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
-00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a40: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00014a50: 5f70 6172 7473 203d 2042 6962 6c65 5665  _parts = BibleVe
-00014a60: 7273 6550 6172 742e 4348 4150 0a20 2020  rsePart.CHAP.   
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 2020 2020 2061 745f 7665 7273 655f 6c65       at_verse_le
-00014aa0: 7665 6c20 3d20 4661 6c73 650a 2020 2020  vel = False.    
-00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ad0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014af0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00014b00: 5468 6973 2072 616e 6765 2069 6e76 6f6c  This range invol
-00014b10: 7665 7320 7665 7273 6573 2c20 696e 2061  ves verses, in a
-00014b20: 206c 6973 7420 7468 6174 2773 206f 7468   list that's oth
-00014b30: 6572 7769 7365 2063 6861 7074 6572 732c  erwise chapters,
-00014b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b60: 2020 2020 2020 2020 2023 2073 6f20 6974           # so it
-00014b70: 2773 2063 6c65 6172 6572 2074 6f20 6469  's clearer to di
-00014b80: 7370 6c61 7920 7573 696e 6720 7665 7273  splay using vers
-00014b90: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bb0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00014bc0: 5f70 6172 7473 203d 2042 6962 6c65 5665  _parts = BibleVe
-00014bd0: 7273 6550 6172 742e 4348 4150 5f56 4552  rsePart.CHAP_VER
-00014be0: 5345 0a20 2020 2020 2020 2020 2020 2020  SE.             
-00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c00: 2020 2020 2020 2020 2020 2061 745f 7665             at_ve
-00014c10: 7273 655f 6c65 7665 6c20 3d20 5472 7565  rse_level = True
-00014c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c40: 2020 2020 2020 2020 2066 6f72 6365 5f64           force_d
-00014c50: 7561 6c5f 7265 6620 3d20 5472 7565 0a20  ual_ref = True. 
-00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c70: 2020 2065 6c73 653a 2023 2053 7461 7274     else: # Start
-00014c80: 206f 6620 6120 6469 6666 6572 656e 7420   of a different 
-00014c90: 626f 6f6b 0a20 2020 2020 2020 2020 2020  book.           
-00014ca0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014cb0: 6e6f 7420 7072 6573 6572 7665 5f67 726f  not preserve_gro
-00014cc0: 7570 733a 2023 2055 7365 206d 616a 6f72  ups: # Use major
-00014cd0: 206c 6973 7420 7365 7020 6265 7477 6565   list sep betwee
-00014ce0: 6e20 626f 6f6b 730a 2020 2020 2020 2020  n books.        
-00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d00: 2020 2020 6c69 7374 5f73 6570 203d 2062      list_sep = b
-00014d10: 6962 6c65 5f64 6174 6128 292e 6d61 6a6f  ible_data().majo
-00014d20: 725f 6c69 7374 5f73 6570 0a20 2020 2020  r_list_sep.     
-00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2020 2073 7461 7274 5f70 6172 7473 203d     start_parts =
-00014d50: 2042 6962 6c65 5665 7273 6550 6172 742e   BibleVersePart.
-00014d60: 424f 4f4b 5f43 4841 500a 2020 2020 2020  BOOK_CHAP.      
-00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d80: 2020 6174 5f76 6572 7365 5f6c 6576 656c    at_verse_level
-00014d90: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00014da0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00014db0: 5f63 6861 7020 3d20 6269 626c 655f 7261  _chap = bible_ra
-00014dc0: 6e67 652e 7374 6172 742e 6368 6170 5f6e  nge.start.chap_n
-00014dd0: 756d 0a20 2020 2020 2020 2020 2020 2020  um.             
-00014de0: 2020 2065 6c73 653a 2023 2052 616e 6765     else: # Range
-00014df0: 2073 7461 7274 2069 7320 6a75 7374 2061   start is just a
-00014e00: 2070 6172 7469 6375 6c61 7220 7665 7273   particular vers
-00014e10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00014e20: 2020 2020 2020 6966 2063 7572 5f62 6f6f        if cur_boo
-00014e30: 6b20 3d3d 2062 6962 6c65 5f72 616e 6765  k == bible_range
-00014e40: 2e73 7461 7274 2e62 6f6f 6b3a 2023 2043  .start.book: # C
-00014e50: 6f6e 7469 6e75 696e 6720 7361 6d65 2062  ontinuing same b
-00014e60: 6f6f 6b0a 2020 2020 2020 2020 2020 2020  ook.            
-00014e70: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00014e80: 745f 7665 7273 655f 6c65 7665 6c20 616e  t_verse_level an
-00014e90: 6420 6375 725f 6368 6170 203d 3d20 6269  d cur_chap == bi
-00014ea0: 626c 655f 7261 6e67 652e 7374 6172 742e  ble_range.start.
-00014eb0: 6368 6170 5f6e 756d 3a20 2320 436f 6e74  chap_num: # Cont
-00014ec0: 696e 7569 6e67 2073 616d 6520 6368 6170  inuing same chap
-00014ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014ef0: 6269 626c 655f 7261 6e67 652e 6368 6170  bible_range.chap
-00014f00: 5f63 6f75 6e74 2866 6c61 6773 3d66 6c61  _count(flags=fla
-00014f10: 6773 2920 3e20 313a 0a20 2020 2020 2020  gs) > 1:.       
-00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f30: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00014f40: 7265 6620 6372 6f73 7365 7320 6368 6170  ref crosses chap
-00014f50: 2f62 6f6f 6b20 626f 756e 6461 7269 6573  /book boundaries
-00014f60: 2069 6e20 6120 7665 7273 6520 6c69 7374   in a verse list
-00014f70: 2c20 736f 2069 7427 7320 636c 6561 7265  , so it's cleare
-00014f80: 7220 746f 2072 6570 6561 740a 2020 2020  r to repeat.    
-00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fa0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-00014fb0: 6520 7374 6172 7469 6e67 2063 6861 7020  e starting chap 
-00014fc0: 6e75 6d0a 2020 2020 2020 2020 2020 2020  num.            
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fe0: 2020 2020 7374 6172 745f 7061 7274 7320      start_parts 
-00014ff0: 3d20 4269 626c 6556 6572 7365 5061 7274  = BibleVersePart
-00015000: 2e43 4841 505f 5645 5253 450a 2020 2020  .CHAP_VERSE.    
-00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015020: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00015030: 6f74 2070 7265 7365 7276 655f 6772 6f75  ot preserve_grou
-00015040: 7073 3a20 2320 5573 6520 6d61 6a6f 7220  ps: # Use major 
-00015050: 6c69 7374 2073 6570 2062 6574 7765 656e  list sep between
-00015060: 206d 756c 7469 2d63 6861 7020 7261 6e67   multi-chap rang
-00015070: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 2020 2020 2020 206c 6973 745f 7365 7020         list_sep 
-000150a0: 3d20 6269 626c 655f 6461 7461 2829 2e6d  = bible_data().m
-000150b0: 616a 6f72 5f6c 6973 745f 7365 700a 2020  ajor_list_sep.  
-000150c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2320 5468 6973 2072 6566 2073 7461 7973  # This ref stays
-00015110: 2077 6974 6869 6e20 7468 6520 7361 6d65   within the same
-00015120: 2063 6861 7020 6e75 6d0a 2020 2020 2020   chap num.      
-00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015140: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-00015150: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
-00015160: 7365 5061 7274 2e56 4552 5345 0a20 2020  sePart.VERSE.   
-00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015180: 2020 2020 2065 6c73 653a 2023 2041 7420       else: # At 
-00015190: 6368 6170 206c 6576 656c 206f 7220 7665  chap level or ve
-000151a0: 7273 6520 6c65 7665 6c20 696e 2061 2064  rse level in a d
-000151b0: 6966 6665 7265 6e74 2063 6861 700a 2020  ifferent chap.  
-000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151d0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000151e0: 2070 7265 7365 7276 655f 6772 6f75 7073   preserve_groups
-000151f0: 3a20 2320 5573 6520 6d61 6a6f 7220 6c69  : # Use major li
-00015200: 7374 2073 6570 2062 6574 7765 656e 2063  st sep between c
-00015210: 6861 7074 6572 730a 2020 2020 2020 2020  hapters.        
-00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015230: 2020 2020 2020 2020 6c69 7374 5f73 6570          list_sep
-00015240: 203d 2062 6962 6c65 5f64 6174 6128 292e   = bible_data().
-00015250: 6d61 6a6f 725f 6c69 7374 5f73 6570 0a20  major_list_sep. 
-00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015270: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00015280: 5f70 6172 7473 203d 2042 6962 6c65 5665  _parts = BibleVe
-00015290: 7273 6550 6172 742e 4348 4150 5f56 4552  rsePart.CHAP_VER
-000152a0: 5345 0a20 2020 2020 2020 2020 2020 2020  SE.             
-000152b0: 2020 2020 2020 2065 6c73 653a 2023 2044         else: # D
-000152c0: 6966 6665 7265 6e74 2062 6f6f 6b0a 2020  ifferent book.  
-000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152e0: 2020 2020 2020 6966 206e 6f74 2070 7265        if not pre
-000152f0: 7365 7276 655f 6772 6f75 7073 3a20 2320  serve_groups: # 
-00015300: 5573 6520 6d61 6a6f 7220 6c69 7374 2073  Use major list s
-00015310: 6570 2062 6574 7765 656e 2062 6f6f 6b73  ep between books
-00015320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015330: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-00015340: 745f 7365 7020 3d20 6269 626c 655f 6461  t_sep = bible_da
-00015350: 7461 2829 2e6d 616a 6f72 5f6c 6973 745f  ta().major_list_
-00015360: 7365 700a 2020 2020 2020 2020 2020 2020  sep.            
-00015370: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00015380: 745f 7061 7274 7320 3d20 4269 626c 6556  t_parts = BibleV
-00015390: 6572 7365 5061 7274 2e46 554c 4c5f 5245  ersePart.FULL_RE
-000153a0: 460a 2020 2020 2020 2020 2020 2020 2020  F.              
-000153b0: 2020 2020 2020 6375 725f 6368 6170 203d        cur_chap =
-000153c0: 2062 6962 6c65 5f72 616e 6765 2e73 7461   bible_range.sta
-000153d0: 7274 2e63 6861 705f 6e75 6d0a 2020 2020  rt.chap_num.    
-000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153f0: 6174 5f76 6572 7365 5f6c 6576 656c 203d  at_verse_level =
-00015400: 2054 7275 6520 2320 416c 6c20 7369 6e67   True # All sing
-00015410: 6c65 2076 6572 7365 7320 6d6f 7665 2075  le verses move u
-00015420: 7320 746f 2076 6572 7365 206c 6576 656c  s to verse level
-00015430: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015440: 2020 6375 725f 626f 6f6b 203d 2062 6962    cur_book = bib
-00015450: 6c65 5f72 616e 6765 2e73 7461 7274 2e62  le_range.start.b
-00015460: 6f6f 6b0a 2020 2020 2020 2020 2020 2020  ook.            
-00015470: 2020 2020 6966 2066 6f72 6365 5f73 7461      if force_sta
-00015480: 7274 5f76 6572 7365 7320 616e 6420 2842  rt_verses and (B
-00015490: 6962 6c65 5665 7273 6550 6172 742e 5645  ibleVersePart.VE
-000154a0: 5253 4520 6e6f 7420 696e 2073 7461 7274  RSE not in start
-000154b0: 5f70 6172 7473 2920 616e 6420 5c0a 2020  _parts) and \.  
-000154c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154d0: 2028 6e6f 7420 6269 626c 655f 7261 6e67   (not bible_rang
-000154e0: 652e 7370 616e 735f 656e 645f 6368 6170  e.spans_end_chap
-000154f0: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-00015500: 2020 2020 2020 2020 2023 2045 6e64 2076           # End v
-00015510: 6572 7365 2077 696c 6c20 7368 6f77 2076  erse will show v
-00015520: 6572 7365 206e 756d 2c20 616e 6420 7765  erse num, and we
-00015530: 2776 6520 6265 656e 2061 736b 6564 2074  've been asked t
-00015540: 6f20 7368 6f77 2073 7461 7274 2076 6572  o show start ver
-00015550: 7365 206e 756d 2069 6e20 7375 6368 2063  se num in such c
-00015560: 6173 6573 0a20 2020 2020 2020 2020 2020  ases.           
-00015570: 2020 2020 2020 2020 2073 7461 7274 5f70           start_p
-00015580: 6172 7473 207c 3d20 4269 626c 6556 6572  arts |= BibleVer
-00015590: 7365 5061 7274 2e56 4552 5345 0a20 2020  sePart.VERSE.   
-000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155b0: 2061 745f 7665 7273 655f 6c65 7665 6c20   at_verse_level 
-000155c0: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
-000155d0: 2020 2020 2020 2020 7374 6172 745f 7374          start_st
-000155e0: 7220 3d20 6269 626c 655f 7261 6e67 652e  r = bible_range.
-000155f0: 7374 6172 742e 7374 7228 6162 6272 6576  start.str(abbrev
-00015600: 2c20 616c 745f 7365 702c 206e 6f73 7061  , alt_sep, nospa
-00015610: 6365 2c20 7374 6172 745f 7061 7274 7329  ce, start_parts)
-00015620: 200a 0a20 2020 2020 2020 2020 2020 2020   ..             
-00015630: 2020 2069 6620 6e6f 7420 666f 7263 655f     if not force_
-00015640: 6475 616c 5f72 6566 2061 6e64 2028 6269  dual_ref and (bi
-00015650: 626c 655f 7261 6e67 652e 6973 5f77 686f  ble_range.is_who
-00015660: 6c65 5f62 6f6f 6b28 666c 6167 7329 206f  le_book(flags) o
-00015670: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2020 2020 2020 2020 2020 2020 2062 6962               bib
-000156a0: 6c65 5f72 616e 6765 2e69 735f 7768 6f6c  le_range.is_whol
-000156b0: 655f 6368 6170 2866 6c61 6773 2920 6f72  e_chap(flags) or
-000156c0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-000156d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156e0: 2020 2020 2020 2020 2020 2020 2020 6269                bi
-000156f0: 626c 655f 7261 6e67 652e 6973 5f73 696e  ble_range.is_sin
-00015700: 676c 655f 7665 7273 6528 2929 3a0a 2020  gle_verse()):.  
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015720: 2020 2320 5369 6e67 6c65 2072 6566 6572    # Single refer
-00015730: 656e 6365 0a20 2020 2020 2020 2020 2020  ence.           
-00015740: 2020 2020 2020 2020 2065 6e64 5f73 7472           end_str
-00015750: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
-00015760: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
-00015770: 7365 7020 3d20 2222 0a20 2020 2020 2020  sep = "".       
-00015780: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157a0: 2020 2072 616e 6765 5f73 6570 203d 2062     range_sep = b
-000157b0: 6962 6c65 5f64 6174 6128 292e 7261 6e67  ible_data().rang
-000157c0: 655f 7365 700a 2020 2020 2020 2020 2020  e_sep.          
-000157d0: 2020 2020 2020 2020 2020 6966 2062 6962            if bib
-000157e0: 6c65 5f72 616e 6765 2e65 6e64 2e62 6f6f  le_range.end.boo
-000157f0: 6b20 213d 2062 6962 6c65 5f72 616e 6765  k != bible_range
-00015800: 2e73 7461 7274 2e62 6f6f 6b3a 0a20 2020  .start.book:.   
-00015810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015820: 2020 2020 2061 745f 7665 7273 655f 6c65       at_verse_le
-00015830: 7665 6c20 3d20 4661 6c73 650a 0a20 2020  vel = False..   
-00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015850: 2069 6620 6269 626c 655f 7261 6e67 652e   if bible_range.
-00015860: 7370 616e 735f 656e 645f 626f 6f6b 2866  spans_end_book(f
-00015870: 6c61 6773 293a 2023 2052 616e 6765 2065  lags): # Range e
-00015880: 6e64 2069 6e63 6c75 6465 7320 616e 2065  nd includes an e
-00015890: 6e74 6972 6520 626f 6f6b 0a20 2020 2020  ntire book.     
-000158a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158b0: 2020 2065 6e64 5f70 6172 7473 203d 2042     end_parts = B
-000158c0: 6962 6c65 5665 7273 6550 6172 742e 424f  ibleVersePart.BO
-000158d0: 4f4b 0a20 2020 2020 2020 2020 2020 2020  OK.             
-000158e0: 2020 2020 2020 2020 2020 2063 7572 5f63             cur_c
-000158f0: 6861 7020 3d20 4e6f 6e65 0a20 2020 2020  hap = None.     
-00015900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015910: 2020 2061 745f 7665 7273 655f 6c65 7665     at_verse_leve
-00015920: 6c20 3d20 4661 6c73 650a 2020 2020 2020  l = False.      
-00015930: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00015940: 6966 206e 6f74 2061 745f 7665 7273 655f  if not at_verse_
-00015950: 6c65 7665 6c20 616e 6420 6269 626c 655f  level and bible_
-00015960: 7261 6e67 652e 7370 616e 735f 656e 645f  range.spans_end_
-00015970: 6368 6170 2866 6c61 6773 293a 2023 2052  chap(flags): # R
-00015980: 616e 6765 2065 6e64 2069 6e63 6c75 6465  ange end include
-00015990: 7320 616e 2065 6e74 6972 6520 6368 6170  s an entire chap
-000159a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000159b0: 2020 2020 2020 2020 2069 6620 6375 725f           if cur_
-000159c0: 626f 6f6b 203d 3d20 6269 626c 655f 7261  book == bible_ra
-000159d0: 6e67 652e 656e 642e 626f 6f6b 3a20 2320  nge.end.book: # 
-000159e0: 436f 6e74 696e 7569 6e67 2073 616d 6520  Continuing same 
-000159f0: 626f 6f6b 0a20 2020 2020 2020 2020 2020  book.           
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 2065 6e64 5f70 6172 7473 203d 2042 6962   end_parts = Bib
-00015a20: 6c65 5665 7273 6550 6172 742e 4348 4150  leVersePart.CHAP
-00015a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a40: 2020 2020 2020 2020 2065 6c73 653a 2023           else: #
-00015a50: 2044 6966 6665 7265 6e74 2062 6f6f 6b0a   Different book.
-00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a70: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-00015a80: 7061 7274 7320 3d20 4269 626c 6556 6572  parts = BibleVer
-00015a90: 7365 5061 7274 2e42 4f4f 4b5f 4348 4150  sePart.BOOK_CHAP
-00015aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ab0: 2020 2020 2020 2020 2063 7572 5f63 6861           cur_cha
-00015ac0: 7020 3d20 6269 626c 655f 7261 6e67 652e  p = bible_range.
-00015ad0: 656e 642e 6368 6170 5f6e 756d 0a20 2020  end.chap_num.   
-00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015af0: 2020 2020 2061 745f 7665 7273 655f 6c65       at_verse_le
-00015b00: 7665 6c20 3d20 4661 6c73 650a 2020 2020  vel = False.    
-00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b20: 656c 7365 3a20 2320 5261 6e67 6520 656e  else: # Range en
-00015b30: 6420 6973 2061 2077 686f 6c65 2063 6861  d is a whole cha
-00015b40: 7020 6166 7465 7220 6120 7061 7274 6963  p after a partic
-00015b50: 756c 6172 2076 6572 7365 2c20 6f72 2061  ular verse, or a
-00015b60: 2070 6172 7469 6375 6c61 7220 7665 7273   particular vers
-00015b70: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00015b80: 2020 2020 2020 2020 2020 6966 2063 7572            if cur
-00015b90: 5f62 6f6f 6b20 3d3d 2062 6962 6c65 5f72  _book == bible_r
-00015ba0: 616e 6765 2e65 6e64 2e62 6f6f 6b3a 2023  ange.end.book: #
-00015bb0: 2043 6f6e 7469 6e75 696e 6720 7361 6d65   Continuing same
-00015bc0: 2062 6f6f 6b0a 2020 2020 2020 2020 2020   book.          
-00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015be0: 2020 6966 2063 7572 5f63 6861 7020 3d3d    if cur_chap ==
-00015bf0: 2062 6962 6c65 5f72 616e 6765 2e65 6e64   bible_range.end
-00015c00: 2e63 6861 705f 6e75 6d3a 2023 2043 6f6e  .chap_num: # Con
-00015c10: 7469 6e75 696e 6720 7361 6d65 2063 6861  tinuing same cha
-00015c20: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00015c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c40: 2020 656e 645f 7061 7274 7320 3d20 4269    end_parts = Bi
-00015c50: 626c 6556 6572 7365 5061 7274 2e56 4552  bleVersePart.VER
-00015c60: 5345 0a20 2020 2020 2020 2020 2020 2020  SE.             
-00015c70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00015c80: 6c73 653a 2023 2044 6966 6665 7265 6e74  lse: # Different
-00015c90: 2063 6861 700a 2020 2020 2020 2020 2020   chap.          
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cb0: 2020 2020 2020 656e 645f 7061 7274 7320        end_parts 
-00015cc0: 3d20 4269 626c 6556 6572 7365 5061 7274  = BibleVersePart
-00015cd0: 2e43 4841 505f 5645 5253 450a 2020 2020  .CHAP_VERSE.    
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 2020 656c 7365 3a20 2320 4469 6666      else: # Diff
-00015d00: 6572 656e 7420 626f 6f6b 0a20 2020 2020  erent book.     
-00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d20: 2020 2020 2020 2065 6e64 5f70 6172 7473         end_parts
-00015d30: 203d 2042 6962 6c65 5665 7273 6550 6172   = BibleVersePar
-00015d40: 742e 4655 4c4c 5f52 4546 0a20 2020 2020  t.FULL_REF.     
-00015d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d60: 2020 2063 7572 5f63 6861 7020 3d20 6269     cur_chap = bi
-00015d70: 626c 655f 7261 6e67 652e 656e 642e 6368  ble_range.end.ch
-00015d80: 6170 5f6e 756d 0a20 2020 2020 2020 2020  ap_num.         
-00015d90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00015da0: 745f 7665 7273 655f 6c65 7665 6c20 3d20  t_verse_level = 
-00015db0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-00015dc0: 2020 2020 2020 2020 2063 7572 5f62 6f6f           cur_boo
-00015dd0: 6b20 3d20 6269 626c 655f 7261 6e67 652e  k = bible_range.
-00015de0: 656e 642e 626f 6f6b 0a20 2020 2020 2020  end.book.       
-00015df0: 2020 2020 2020 2020 2020 2020 2065 6e64               end
-00015e00: 5f73 7472 203d 2062 6962 6c65 5f72 616e  _str = bible_ran
-00015e10: 6765 2e65 6e64 2e73 7472 2861 6262 7265  ge.end.str(abbre
-00015e20: 762c 2061 6c74 5f73 6570 2c20 6e6f 7370  v, alt_sep, nosp
-00015e30: 6163 652c 2065 6e64 5f70 6172 7473 2920  ace, end_parts) 
-00015e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00015e60: 2020 6966 2066 6972 7374 5f72 616e 6765    if first_range
-00015e70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015e80: 2020 2020 2020 6c69 7374 5f73 6570 203d        list_sep =
-00015e90: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-00015ea0: 2020 2020 2020 2020 6669 7273 745f 7261          first_ra
-00015eb0: 6e67 6520 3d20 4661 6c73 650a 2020 2020  nge = False.    
-00015ec0: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-00015ed0: 655f 7374 7220 3d20 6622 7b6c 6973 745f  e_str = f"{list_
-00015ee0: 7365 707d 207b 7374 6172 745f 7374 727d  sep} {start_str}
-00015ef0: 7b72 616e 6765 5f73 6570 7d7b 656e 645f  {range_sep}{end_
-00015f00: 7374 727d 220a 0a20 2020 2020 2020 2020  str}"..         
-00015f10: 2020 2020 2020 2069 6620 6e6f 7370 6163         if nospac
-00015f20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00015f30: 2020 2020 2020 2072 6573 756c 745f 7374         result_st
-00015f40: 7220 2b3d 2072 616e 6765 5f73 7472 2e72  r += range_str.r
-00015f50: 6570 6c61 6365 2822 2022 2c20 2222 290a  eplace(" ", "").
-00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015f80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00015f90: 5f73 7472 202b 3d20 7261 6e67 655f 7374  _str += range_st
-00015fa0: 722e 7374 7269 7028 290a 0a20 2020 2020  r.strip()..     
-00015fb0: 2020 2020 2020 2020 2020 206c 6973 745f             list_
-00015fc0: 7365 7020 3d20 6269 626c 655f 6461 7461  sep = bible_data
-00015fd0: 2829 2e6d 696e 6f72 5f6c 6973 745f 7365  ().minor_list_se
-00015fe0: 7020 2320 4d69 6e6f 7220 6c69 7374 2073  p # Minor list s
-00015ff0: 6570 6172 6174 6f72 2062 7920 6465 6661  eparator by defa
-00016000: 756c 7420 7769 7468 696e 2067 726f 7570  ult within group
-00016010: 730a 2020 2020 2020 2020 2020 2020 0a20  s.            . 
-00016020: 2020 2020 2020 2020 2020 2023 2057 6527             # We'
-00016030: 7665 2068 6176 6520 636f 6d70 6c65 7465  ve have complete
-00016040: 6420 7468 6520 6772 6f75 700a 2020 2020  d the group.    
-00016050: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
-00016060: 7276 655f 6772 6f75 7073 3a0a 2020 2020  rve_groups:.    
-00016070: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00016080: 5f73 6570 203d 2062 6962 6c65 5f64 6174  _sep = bible_dat
-00016090: 6128 292e 6d61 6a6f 725f 6c69 7374 5f73  a().major_list_s
-000160a0: 6570 2023 204d 616a 6f72 206c 6973 7420  ep # Major list 
-000160b0: 7365 7061 7261 746f 7220 6265 7477 6565  separator betwee
-000160c0: 6e20 6772 6f75 7073 0a20 2020 2020 2020  n groups.       
-000160d0: 2020 2020 2020 2020 2061 745f 7665 7273           at_vers
-000160e0: 655f 6c65 7665 6c3d 4661 6c73 650a 2020  e_level=False.  
-000160f0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00016100: 2057 6527 7665 2063 6f6d 706c 6574 6564   We've completed
-00016110: 2061 6c6c 2067 726f 7570 730a 2020 2020   all groups.    
-00016120: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00016130: 745f 7374 720a 0a20 2020 2023 0a20 2020  t_str..    #.   
-00016140: 2023 2057 6520 7772 6170 206f 7572 2070   # We wrap our p
-00016150: 7562 6c69 6320 7375 7065 7263 6c61 7373  ublic superclass
-00016160: 206d 6574 686f 6473 2c20 736f 2074 6861   methods, so tha
-00016170: 7420 7064 6f63 2061 7574 6f2d 6765 6e65  t pdoc auto-gene
-00016180: 7261 7465 7320 6f75 7220 646f 6375 6d65  rates our docume
-00016190: 6e74 6174 696f 6e2c 2061 6e64 2061 6c73  ntation, and als
-000161a0: 6f20 746f 2065 6d70 6861 7369 7365 0a20  o to emphasise. 
-000161b0: 2020 2023 2074 6861 7420 7468 6520 696d     # that the im
-000161c0: 706c 656d 656e 7461 7469 6f6e 2063 6f75  plementation cou
-000161d0: 6c64 2063 6861 6e67 652e 0a20 2020 2023  ld change..    #
-000161e0: 0a0a 2020 2020 6465 6620 696e 6465 7828  ..    def index(
-000161f0: 7365 6c66 2c20 7661 6c75 652c 206d 696e  self, value, min
-00016200: 5f69 6e64 6578 3a20 696e 7420 3d20 4e6f  _index: int = No
-00016210: 6e65 2c20 6c69 6d69 745f 696e 6465 783a  ne, limit_index:
-00016220: 2069 6e74 203d 4e6f 6e65 293a 0a20 2020   int =None):.   
-00016230: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00016240: 7228 292e 696e 6465 7828 7661 6c75 652c  r().index(value,
-00016250: 206d 696e 5f69 6e64 6578 2c20 6c69 6d69   min_index, limi
-00016260: 745f 696e 6465 7829 0a0a 2020 2020 6465  t_index)..    de
-00016270: 6620 636f 756e 7428 7365 6c66 2c20 7661  f count(self, va
-00016280: 6c75 6529 3a0a 2020 2020 2020 2020 7265  lue):.        re
-00016290: 7475 726e 2073 7570 6572 2829 2e63 6f75  turn super().cou
-000162a0: 6e74 2876 616c 7565 290a 0a20 2020 2064  nt(value)..    d
-000162b0: 6566 2070 7265 7065 6e64 2873 656c 662c  ef prepend(self,
-000162c0: 2076 616c 7565 2c20 6e65 775f 6772 6f75   value, new_grou
-000162d0: 703a 2062 6f6f 6c20 3d20 4661 6c73 6529  p: bool = False)
-000162e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000162f0: 2073 7570 6572 2829 2e70 7265 7065 6e64   super().prepend
-00016300: 2876 616c 7565 2c20 6e65 775f 6772 6f75  (value, new_grou
-00016310: 7029 0a20 2020 200a 2020 2020 6465 6620  p).    .    def 
-00016320: 6170 7065 6e64 2873 656c 662c 2076 616c  append(self, val
-00016330: 7565 2c20 6e65 775f 6772 6f75 703a 2062  ue, new_group: b
-00016340: 6f6f 6c20 3d20 4661 6c73 6529 3a0a 2020  ool = False):.  
-00016350: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00016360: 6572 2829 2e61 7070 656e 6428 7661 6c75  er().append(valu
-00016370: 652c 206e 6577 5f67 726f 7570 290a 0a20  e, new_group).. 
-00016380: 2020 2064 6566 2061 7070 656e 645f 6772     def append_gr
-00016390: 6f75 7028 7365 6c66 2c20 6974 6572 6162  oup(self, iterab
-000163a0: 6c65 293a 0a20 2020 2020 2020 2072 6574  le):.        ret
-000163b0: 7572 6e20 7375 7065 7228 292e 6170 7065  urn super().appe
-000163c0: 6e64 5f67 726f 7570 2869 7465 7261 626c  nd_group(iterabl
-000163d0: 6529 0a0a 2020 2020 6465 6620 6578 7465  e)..    def exte
-000163e0: 6e64 2873 656c 662c 2069 7465 7261 626c  nd(self, iterabl
-000163f0: 6529 3a0a 2020 2020 2020 2020 7265 7475  e):.        retu
-00016400: 726e 2073 7570 6572 2829 2e65 7874 656e  rn super().exten
-00016410: 6428 6974 6572 6162 6c65 290a 2020 2020  d(iterable).    
-00016420: 0a20 2020 2064 6566 2069 6e73 6572 7428  .    def insert(
-00016430: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
-00016440: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
-00016450: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00016460: 2e69 6e73 6572 7428 696e 6465 782c 2076  .insert(index, v
-00016470: 616c 7565 290a 0a20 2020 2064 6566 2070  alue)..    def p
-00016480: 6f70 2873 656c 662c 2069 6e64 6578 3a20  op(self, index: 
-00016490: 696e 7420 3d20 4e6f 6e65 293a 0a20 2020  int = None):.   
-000164a0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000164b0: 7228 292e 706f 7028 696e 6465 7829 0a0a  r().pop(index)..
-000164c0: 2020 2020 6465 6620 7265 6d6f 7665 2873      def remove(s
-000164d0: 656c 662c 2076 616c 7565 293a 0a20 2020  elf, value):.   
-000164e0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000164f0: 7228 292e 7265 6d6f 7665 2876 616c 7565  r().remove(value
-00016500: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
-00016510: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016520: 7265 7475 726e 2073 7570 6572 2829 2e63  return super().c
-00016530: 6c65 6172 2829 0a20 2020 200a 2020 2020  lear().    .    
-00016540: 6465 6620 636c 6561 725f 6772 6f75 7073  def clear_groups
-00016550: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016560: 7265 7475 726e 2073 7570 6572 2829 2e63  return super().c
-00016570: 6c65 6172 5f67 726f 7570 7328 290a 0a20  lear_groups().. 
-00016580: 2020 2064 6566 2072 6576 6572 7365 2873     def reverse(s
-00016590: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-000165a0: 7475 726e 2073 7570 6572 2829 2e72 6576  turn super().rev
-000165b0: 6572 7365 2829 0a20 2020 200a 2020 2020  erse().    .    
-000165c0: 6465 6620 6571 7561 6c73 2873 656c 662c  def equals(self,
-000165d0: 206f 7468 6572 5f69 7465 7261 626c 652c   other_iterable,
-000165e0: 2063 6f6d 7061 7265 5f67 726f 7570 733d   compare_groups=
-000165f0: 5472 7565 2920 2d3e 2062 6f6f 6c3a 0a20  True) -> bool:. 
-00016600: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00016610: 7065 7228 292e 6571 7561 6c73 286f 7468  per().equals(oth
-00016620: 6572 5f69 7465 7261 626c 652c 2063 6f6d  er_iterable, com
-00016630: 7061 7265 5f67 726f 7570 7329 0a0a 0a42  pare_groups)...B
-00016640: 6962 6c65 5265 6620 3d20 556e 696f 6e5b  ibleRef = Union[
-00016650: 4269 626c 6556 6572 7365 2c20 4269 626c  BibleVerse, Bibl
-00016660: 6552 616e 6765 2c20 4269 626c 6552 616e  eRange, BibleRan
-00016670: 6765 4c69 7374 5d0a 2727 2741 2063 6f6e  geList].'''A con
-00016680: 7665 6e69 656e 6365 2074 7970 6520 746f  venience type to
-00016690: 2069 6e64 6963 6174 6520 6569 7468 6572   indicate either
-000166a0: 2061 2060 4269 626c 6556 6572 7365 602c   a `BibleVerse`,
-000166b0: 2060 4269 626c 6552 616e 6765 6020 6f72   `BibleRange` or
-000166c0: 2060 4269 626c 6552 616e 6765 4c69 7374   `BibleRangeList
-000166d0: 602e 2727 270a 0a0a 636c 6173 7320 4d75  `.'''...class Mu
-000166e0: 6c74 6962 6f6f 6b52 616e 6765 4e6f 7441  ltibookRangeNotA
-000166f0: 6c6c 6f77 6564 4572 726f 7228 4269 626c  llowedError(Bibl
-00016700: 6552 6566 4578 6365 7074 696f 6e29 3a0a  eRefException):.
-00016710: 2020 2020 2727 2752 6169 7365 6420 7768      '''Raised wh
-00016720: 656e 2074 7279 696e 6720 746f 2063 7265  en trying to cre
-00016730: 6174 6520 6120 6042 6962 6c65 5261 6e67  ate a `BibleRang
-00016740: 6560 2077 6974 6820 6120 6469 6666 6572  e` with a differ
-00016750: 656e 7420 7374 6172 7420 616e 6420 656e  ent start and en
-00016760: 6420 6042 6962 6c65 426f 6f6b 6020 616e  d `BibleBook` an
-00016770: 640a 2020 2020 6042 6962 6c65 466c 6167  d.    `BibleFlag
-00016780: 2e4d 554c 5449 424f 4f4b 6020 6973 206e  .MULTIBOOK` is n
-00016790: 6f74 2073 6574 2028 6569 7468 6572 2067  ot set (either g
-000167a0: 6c6f 6261 6c6c 7920 6f72 2069 6e20 6120  lobally or in a 
-000167b0: 6066 6c61 6773 6020 6d65 7468 6f64 2061  `flags` method a
-000167c0: 7267 756d 656e 7429 2e27 2727 0a0a 0a63  rgument).'''...c
-000167d0: 6c61 7373 2049 6e76 616c 6964 5265 6665  lass InvalidRefe
-000167e0: 7265 6e63 6545 7272 6f72 2842 6962 6c65  renceError(Bible
-000167f0: 5265 6645 7863 6570 7469 6f6e 293a 0a20  RefException):. 
-00016800: 2020 2027 2727 5261 6964 6564 2077 6865     '''Raided whe
-00016810: 6e20 7472 7969 6e67 2074 6f20 696e 7374  n trying to inst
-00016820: 616e 7469 6174 6520 6120 4269 626c 6542  antiate a BibleB
-00016830: 6f6f 6b2c 2042 6962 6c65 5665 7273 6520  ook, BibleVerse 
-00016840: 6f72 2042 6962 6c65 5261 6e67 6520 7468  or BibleRange th
-00016850: 6174 2069 7320 6e6f 7420 6120 7661 6c69  at is not a vali
-00016860: 640a 2020 2020 4269 626c 6520 7265 6665  d.    Bible refe
-00016870: 7265 6e63 652e 2727 270a 0a0a 636c 6173  rence.'''...clas
-00016880: 7320 4269 626c 6552 6566 5061 7273 696e  s BibleRefParsin
-00016890: 6745 7272 6f72 2842 6962 6c65 5265 6645  gError(BibleRefE
-000168a0: 7863 6570 7469 6f6e 293a 0a20 2020 2027  xception):.    '
-000168b0: 2727 5261 6973 6564 2077 6865 6e20 7468  ''Raised when th
-000168c0: 6572 6520 6973 2061 6e20 6572 726f 7220  ere is an error 
-000168d0: 7061 7273 696e 6720 6120 7374 7269 6e67  parsing a string
-000168e0: 2069 6e74 6f20 6120 4269 626c 6520 7265   into a Bible re
-000168f0: 6665 7265 6e63 652e 0a20 2020 200a 2020  ference..    .  
-00016900: 2020 436f 6e74 6169 6e73 2074 776f 2065    Contains two e
-00016910: 7874 7261 2061 7474 7269 6275 7465 733a  xtra attributes:
-00016920: 0a20 2020 200a 2020 2020 202d 2060 7374  .    .     - `st
-00016930: 6172 745f 706f 7360 3a20 696e 6465 7820  art_pos`: index 
-00016940: 6f66 2074 6865 2066 6972 7374 2075 6e65  of the first une
-00016950: 7870 6563 7465 6420 6368 6172 6163 7465  xpected characte
-00016960: 7220 696e 2074 6865 2073 7472 696e 6720  r in the string 
-00016970: 666f 7220 7061 7273 696e 672e 0a20 2020  for parsing..   
-00016980: 2020 2d20 6065 6e64 5f70 6f73 603a 2020    - `end_pos`:  
-00016990: 2069 6e64 6578 202b 2031 206f 6620 7468   index + 1 of th
-000169a0: 6520 6c61 7374 2075 6e65 7870 6563 7465  e last unexpecte
-000169b0: 6420 6368 6172 6163 7465 7220 696e 2074  d character in t
-000169c0: 6865 2073 7472 696e 6720 666f 7220 7061  he string for pa
-000169d0: 7273 696e 672e 0a20 2020 2027 2727 0a20  rsing..    '''. 
-000169e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000169f0: 7365 6c66 2c20 6d65 7367 2c20 7374 6172  self, mesg, star
-00016a00: 745f 706f 733d 4e6f 6e65 2c20 656e 645f  t_pos=None, end_
-00016a10: 706f 733d 4e6f 6e65 2c20 2a61 7267 732c  pos=None, *args,
-00016a20: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00016a30: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00016a40: 6974 5f5f 286d 6573 672c 202a 6172 6773  it__(mesg, *args
-00016a50: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-00016a60: 2020 2020 7365 6c66 2e73 7461 7274 5f70      self.start_p
-00016a70: 6f73 203d 2073 7461 7274 5f70 6f73 0a20  os = start_pos. 
-00016a80: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
-00016a90: 706f 7320 3d20 656e 645f 706f 730a 0a    pos = end_pos..
+00011e50: 2020 2020 656e 645f 7061 7274 7320 3d20      end_parts = 
+00011e60: 4269 626c 6556 6572 7365 5061 7274 2e46  BibleVersePart.F
+00011e70: 554c 4c5f 5245 460a 2020 2020 2020 2020  ULL_REF.        
+00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 6375 725f 6368 6170 203d 2062 6962 6c65  cur_chap = bible
+00011ea0: 5f72 616e 6765 2e65 6e64 2e63 6861 705f  _range.end.chap_
+00011eb0: 6e75 6d0a 2020 2020 2020 2020 2020 2020  num.            
+00011ec0: 2020 2020 2020 2020 2020 2020 6174 5f76              at_v
+00011ed0: 6572 7365 5f6c 6576 656c 203d 2054 7275  erse_level = Tru
+00011ee0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00011ef0: 2020 2020 2020 6375 725f 626f 6f6b 203d        cur_book =
+00011f00: 2062 6962 6c65 5f72 616e 6765 2e65 6e64   bible_range.end
+00011f10: 2e62 6f6f 6b0a 2020 2020 2020 2020 2020  .book.          
+00011f20: 2020 2020 2020 2020 2020 656e 645f 7374            end_st
+00011f30: 7220 3d20 6269 626c 655f 7261 6e67 652e  r = bible_range.
+00011f40: 656e 642e 7374 7228 6162 6272 6576 2c20  end.str(abbrev, 
+00011f50: 616c 745f 7365 702c 206e 6f73 7061 6365  alt_sep, nospace
+00011f60: 2c20 656e 645f 7061 7274 7329 200a 2020  , end_parts) .  
+00011f70: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011f90: 6620 6669 7273 745f 7261 6e67 653a 0a20  f first_range:. 
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2020 206c 6973 745f 7365 7020 3d20 2222     list_sep = ""
+00011fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011fd0: 2020 2020 2066 6972 7374 5f72 616e 6765       first_range
+00011fe0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00011ff0: 2020 2020 2020 2020 2072 616e 6765 5f73           range_s
+00012000: 7472 203d 2066 227b 6c69 7374 5f73 6570  tr = f"{list_sep
+00012010: 7d20 7b73 7461 7274 5f73 7472 7d7b 7261  } {start_str}{ra
+00012020: 6e67 655f 7365 707d 7b65 6e64 5f73 7472  nge_sep}{end_str
+00012030: 7d22 0a0a 2020 2020 2020 2020 2020 2020  }"..            
+00012040: 2020 2020 6966 206e 6f73 7061 6365 3a0a      if nospace:.
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 7265 7375 6c74 5f73 7472 202b      result_str +
+00012070: 3d20 7261 6e67 655f 7374 722e 7265 706c  = range_str.repl
+00012080: 6163 6528 2220 222c 2022 2229 0a20 2020  ace(" ", "").   
+00012090: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000120a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000120b0: 2020 2020 2020 2072 6573 756c 745f 7374         result_st
+000120c0: 7220 2b3d 2072 616e 6765 5f73 7472 2e73  r += range_str.s
+000120d0: 7472 6970 2829 0a0a 2020 2020 2020 2020  trip()..        
+000120e0: 2020 2020 2020 2020 6c69 7374 5f73 6570          list_sep
+000120f0: 203d 2062 6962 6c65 5f64 6174 6128 292e   = bible_data().
+00012100: 6d69 6e6f 725f 6c69 7374 5f73 6570 2023  minor_list_sep #
+00012110: 204d 696e 6f72 206c 6973 7420 7365 7061   Minor list sepa
+00012120: 7261 746f 7220 6279 2064 6566 6175 6c74  rator by default
+00012130: 2077 6974 6869 6e20 6772 6f75 7073 0a20   within groups. 
+00012140: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00012150: 2020 2020 2020 2020 2320 5765 2776 6520          # We've 
+00012160: 6861 7665 2063 6f6d 706c 6574 6564 2074  have completed t
+00012170: 6865 2067 726f 7570 0a20 2020 2020 2020  he group.       
+00012180: 2020 2020 2069 6620 7072 6573 6572 7665       if preserve
+00012190: 5f67 726f 7570 733a 0a20 2020 2020 2020  _groups:.       
+000121a0: 2020 2020 2020 2020 206c 6973 745f 7365           list_se
+000121b0: 7020 3d20 6269 626c 655f 6461 7461 2829  p = bible_data()
+000121c0: 2e6d 616a 6f72 5f6c 6973 745f 7365 7020  .major_list_sep 
+000121d0: 2320 4d61 6a6f 7220 6c69 7374 2073 6570  # Major list sep
+000121e0: 6172 6174 6f72 2062 6574 7765 656e 2067  arator between g
+000121f0: 726f 7570 730a 2020 2020 2020 2020 2020  roups.          
+00012200: 2020 2020 2020 6174 5f76 6572 7365 5f6c        at_verse_l
+00012210: 6576 656c 3d46 616c 7365 0a20 2020 2020  evel=False.     
+00012220: 2020 200a 2020 2020 2020 2020 2320 5765     .        # We
+00012230: 2776 6520 636f 6d70 6c65 7465 6420 616c  've completed al
+00012240: 6c20 6772 6f75 7073 0a20 2020 2020 2020  l groups.       
+00012250: 2072 6574 7572 6e20 7265 7375 6c74 5f73   return result_s
+00012260: 7472 0a0a 2020 2020 230a 2020 2020 2320  tr..    #.    # 
+00012270: 5765 2077 7261 7020 6f75 7220 7075 626c  We wrap our publ
+00012280: 6963 2073 7570 6572 636c 6173 7320 6d65  ic superclass me
+00012290: 7468 6f64 732c 2073 6f20 7468 6174 2070  thods, so that p
+000122a0: 646f 6320 6175 746f 2d67 656e 6572 6174  doc auto-generat
+000122b0: 6573 206f 7572 2064 6f63 756d 656e 7461  es our documenta
+000122c0: 7469 6f6e 2c20 616e 6420 616c 736f 2074  tion, and also t
+000122d0: 6f20 656d 7068 6173 6973 650a 2020 2020  o emphasise.    
+000122e0: 2320 7468 6174 2074 6865 2069 6d70 6c65  # that the imple
+000122f0: 6d65 6e74 6174 696f 6e20 636f 756c 6420  mentation could 
+00012300: 6368 616e 6765 2e0a 2020 2020 230a 0a20  change..    #.. 
+00012310: 2020 2064 6566 2069 6e64 6578 2873 656c     def index(sel
+00012320: 662c 2076 616c 7565 2c20 6d69 6e5f 696e  f, value, min_in
+00012330: 6465 783a 2069 6e74 203d 204e 6f6e 652c  dex: int = None,
+00012340: 206c 696d 6974 5f69 6e64 6578 3a20 696e   limit_index: in
+00012350: 7420 3d4e 6f6e 6529 3a0a 2020 2020 2020  t =None):.      
+00012360: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00012370: 2e69 6e64 6578 2876 616c 7565 2c20 6d69  .index(value, mi
+00012380: 6e5f 696e 6465 782c 206c 696d 6974 5f69  n_index, limit_i
+00012390: 6e64 6578 290a 0a20 2020 2064 6566 2063  ndex)..    def c
+000123a0: 6f75 6e74 2873 656c 662c 2076 616c 7565  ount(self, value
+000123b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000123c0: 6e20 7375 7065 7228 292e 636f 756e 7428  n super().count(
+000123d0: 7661 6c75 6529 0a0a 2020 2020 6465 6620  value)..    def 
+000123e0: 7072 6570 656e 6428 7365 6c66 2c20 7661  prepend(self, va
+000123f0: 6c75 652c 206e 6577 5f67 726f 7570 3a20  lue, new_group: 
+00012400: 626f 6f6c 203d 2046 616c 7365 293a 0a20  bool = False):. 
+00012410: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+00012420: 7065 7228 292e 7072 6570 656e 6428 7661  per().prepend(va
+00012430: 6c75 652c 206e 6577 5f67 726f 7570 290a  lue, new_group).
+00012440: 2020 2020 0a20 2020 2064 6566 2061 7070      .    def app
+00012450: 656e 6428 7365 6c66 2c20 7661 6c75 652c  end(self, value,
+00012460: 206e 6577 5f67 726f 7570 3a20 626f 6f6c   new_group: bool
+00012470: 203d 2046 616c 7365 293a 0a20 2020 2020   = False):.     
+00012480: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00012490: 292e 6170 7065 6e64 2876 616c 7565 2c20  ).append(value, 
+000124a0: 6e65 775f 6772 6f75 7029 0a0a 2020 2020  new_group)..    
+000124b0: 6465 6620 6170 7065 6e64 5f67 726f 7570  def append_group
+000124c0: 2873 656c 662c 2069 7465 7261 626c 6529  (self, iterable)
+000124d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000124e0: 2073 7570 6572 2829 2e61 7070 656e 645f   super().append_
+000124f0: 6772 6f75 7028 6974 6572 6162 6c65 290a  group(iterable).
+00012500: 0a20 2020 2064 6566 2065 7874 656e 6428  .    def extend(
+00012510: 7365 6c66 2c20 6974 6572 6162 6c65 293a  self, iterable):
+00012520: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012530: 7375 7065 7228 292e 6578 7465 6e64 2869  super().extend(i
+00012540: 7465 7261 626c 6529 0a20 2020 200a 2020  terable).    .  
+00012550: 2020 6465 6620 696e 7365 7274 2873 656c    def insert(sel
+00012560: 662c 2069 6e64 6578 3a20 696e 742c 2076  f, index: int, v
+00012570: 616c 7565 293a 0a20 2020 2020 2020 2072  alue):.        r
+00012580: 6574 7572 6e20 7375 7065 7228 292e 696e  eturn super().in
+00012590: 7365 7274 2869 6e64 6578 2c20 7661 6c75  sert(index, valu
+000125a0: 6529 0a0a 2020 2020 6465 6620 706f 7028  e)..    def pop(
+000125b0: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
+000125c0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000125d0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000125e0: 2e70 6f70 2869 6e64 6578 290a 0a20 2020  .pop(index)..   
+000125f0: 2064 6566 2072 656d 6f76 6528 7365 6c66   def remove(self
+00012600: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
+00012610: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00012620: 2e72 656d 6f76 6528 7661 6c75 6529 0a0a  .remove(value)..
+00012630: 2020 2020 6465 6620 636c 6561 7228 7365      def clear(se
+00012640: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00012650: 7572 6e20 7375 7065 7228 292e 636c 6561  urn super().clea
+00012660: 7228 290a 2020 2020 0a20 2020 2064 6566  r().    .    def
+00012670: 2072 6576 6572 7365 2873 656c 6629 3a0a   reverse(self):.
+00012680: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00012690: 7570 6572 2829 2e72 6576 6572 7365 2829  uper().reverse()
+000126a0: 0a20 2020 200a 2020 2020 6465 6620 736f  .    .    def so
+000126b0: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+000126c0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000126d0: 2e73 6f72 7428 290a 0a20 2020 2064 6566  .sort()..    def
+000126e0: 2065 7175 616c 7328 7365 6c66 2c20 6f74   equals(self, ot
+000126f0: 6865 725f 6974 6572 6162 6c65 2c20 636f  her_iterable, co
+00012700: 6d70 6172 655f 6772 6f75 7073 3d54 7275  mpare_groups=Tru
+00012710: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
+00012720: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00012730: 2829 2e65 7175 616c 7328 6f74 6865 725f  ().equals(other_
+00012740: 6974 6572 6162 6c65 2c20 636f 6d70 6172  iterable, compar
+00012750: 655f 6772 6f75 7073 290a 0a0a 4269 626c  e_groups)...Bibl
+00012760: 6552 6566 203d 2055 6e69 6f6e 5b42 6962  eRef = Union[Bib
+00012770: 6c65 5665 7273 652c 2042 6962 6c65 5261  leVerse, BibleRa
+00012780: 6e67 652c 2042 6962 6c65 5261 6e67 654c  nge, BibleRangeL
+00012790: 6973 745d 0a27 2727 4120 636f 6e76 656e  ist].'''A conven
+000127a0: 6965 6e63 6520 7479 7065 2074 6f20 696e  ience type to in
+000127b0: 6469 6361 7465 2065 6974 6865 7220 6120  dicate either a 
+000127c0: 6042 6962 6c65 5665 7273 6560 2c20 6042  `BibleVerse`, `B
+000127d0: 6962 6c65 5261 6e67 6560 206f 7220 6042  ibleRange` or `B
+000127e0: 6962 6c65 5261 6e67 654c 6973 7460 2e27  ibleRangeList`.'
+000127f0: 2727 0a0a 0a63 6c61 7373 204d 756c 7469  ''...class Multi
+00012800: 626f 6f6b 5261 6e67 654e 6f74 416c 6c6f  bookRangeNotAllo
+00012810: 7765 6445 7272 6f72 2842 6962 6c65 5265  wedError(BibleRe
+00012820: 6645 7863 6570 7469 6f6e 293a 0a20 2020  fException):.   
+00012830: 2027 2727 5261 6973 6564 2077 6865 6e20   '''Raised when 
+00012840: 7472 7969 6e67 2074 6f20 6372 6561 7465  trying to create
+00012850: 2061 2060 4269 626c 6552 616e 6765 6020   a `BibleRange` 
+00012860: 7769 7468 2061 2064 6966 6665 7265 6e74  with a different
+00012870: 2073 7461 7274 2061 6e64 2065 6e64 2060   start and end `
+00012880: 4269 626c 6542 6f6f 6b60 2061 6e64 0a20  BibleBook` and. 
+00012890: 2020 2060 4269 626c 6546 6c61 672e 4d55     `BibleFlag.MU
+000128a0: 4c54 4942 4f4f 4b60 2069 7320 6e6f 7420  LTIBOOK` is not 
+000128b0: 7365 7420 2865 6974 6865 7220 676c 6f62  set (either glob
+000128c0: 616c 6c79 206f 7220 696e 2061 2060 666c  ally or in a `fl
+000128d0: 6167 7360 206d 6574 686f 6420 6172 6775  ags` method argu
+000128e0: 6d65 6e74 292e 2727 270a 0a0a 636c 6173  ment).'''...clas
+000128f0: 7320 496e 7661 6c69 6452 6566 6572 656e  s InvalidReferen
+00012900: 6365 4572 726f 7228 4269 626c 6552 6566  ceError(BibleRef
+00012910: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+00012920: 2727 2752 6169 6465 6420 7768 656e 2074  '''Raided when t
+00012930: 7279 696e 6720 746f 2069 6e73 7461 6e74  rying to instant
+00012940: 6961 7465 2061 2042 6962 6c65 426f 6f6b  iate a BibleBook
+00012950: 2c20 4269 626c 6556 6572 7365 206f 7220  , BibleVerse or 
+00012960: 4269 626c 6552 616e 6765 2074 6861 7420  BibleRange that 
+00012970: 6973 206e 6f74 2061 2076 616c 6964 0a20  is not a valid. 
+00012980: 2020 2042 6962 6c65 2072 6566 6572 656e     Bible referen
+00012990: 6365 2e27 2727 0a0a 0a63 6c61 7373 2042  ce.'''...class B
+000129a0: 6962 6c65 5265 6650 6172 7369 6e67 4572  ibleRefParsingEr
+000129b0: 726f 7228 4269 626c 6552 6566 4578 6365  ror(BibleRefExce
+000129c0: 7074 696f 6e29 3a0a 2020 2020 2727 2752  ption):.    '''R
+000129d0: 6169 7365 6420 7768 656e 2074 6865 7265  aised when there
+000129e0: 2069 7320 616e 2065 7272 6f72 2070 6172   is an error par
+000129f0: 7369 6e67 2061 2073 7472 696e 6720 696e  sing a string in
+00012a00: 746f 2061 2042 6962 6c65 2072 6566 6572  to a Bible refer
+00012a10: 656e 6365 2e0a 2020 2020 0a20 2020 2043  ence..    .    C
+00012a20: 6f6e 7461 696e 7320 7477 6f20 6578 7472  ontains two extr
+00012a30: 6120 6174 7472 6962 7574 6573 3a0a 2020  a attributes:.  
+00012a40: 2020 0a20 2020 2020 2d20 6073 7461 7274    .     - `start
+00012a50: 5f70 6f73 603a 2069 6e64 6578 206f 6620  _pos`: index of 
+00012a60: 7468 6520 6669 7273 7420 756e 6578 7065  the first unexpe
+00012a70: 6374 6564 2063 6861 7261 6374 6572 2069  cted character i
+00012a80: 6e20 7468 6520 7374 7269 6e67 2066 6f72  n the string for
+00012a90: 2070 6172 7369 6e67 2e0a 2020 2020 202d   parsing..     -
+00012aa0: 2060 656e 645f 706f 7360 3a20 2020 696e   `end_pos`:   in
+00012ab0: 6465 7820 6f66 2074 6865 206c 6173 7420  dex of the last 
+00012ac0: 756e 6578 7065 6374 6564 2063 6861 7261  unexpected chara
+00012ad0: 6374 6572 2069 6e20 7468 6520 7374 7269  cter in the stri
+00012ae0: 6e67 2066 6f72 2070 6172 7369 6e67 2e0a  ng for parsing..
+00012af0: 2020 2020 2727 270a 2020 2020 6465 6620      '''.    def 
+00012b00: 5f5f 696e 6974 5f5f 2873 656c 662c 206d  __init__(self, m
+00012b10: 6573 672c 2073 7461 7274 5f70 6f73 3d4e  esg, start_pos=N
+00012b20: 6f6e 652c 2065 6e64 5f70 6f73 3d4e 6f6e  one, end_pos=Non
+00012b30: 652c 202a 6172 6773 2c20 2a2a 6b77 6172  e, *args, **kwar
+00012b40: 6773 293a 0a20 2020 2020 2020 2073 7570  gs):.        sup
+00012b50: 6572 2829 2e5f 5f69 6e69 745f 5f28 6d65  er().__init__(me
+00012b60: 7367 2c20 2a61 7267 732c 202a 2a6b 7761  sg, *args, **kwa
+00012b70: 7267 7329 0a20 2020 2020 2020 2073 656c  rgs).        sel
+00012b80: 662e 7374 6172 745f 706f 7320 3d20 7374  f.start_pos = st
+00012b90: 6172 745f 706f 730a 2020 2020 2020 2020  art_pos.        
+00012ba0: 7365 6c66 2e65 6e64 5f70 6f73 203d 2065  self.end_pos = e
+00012bb0: 6e64 5f70 6f73 0a0a                      nd_pos..
```

### Comparing `bibleref-0.15.0/src/bibleref/util.py` & `bibleref-0.9.0/src/bibleref/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,26 +182,17 @@
         def __repr__(self):
             return f"GroupView({str(self)})"
 
         def __str__(self):
             return str(list(self))
 
     def __init__(self, iterable: Iterable = None):
-        '''Creates a new `GroupedList` and adds the items in `iterable` to this list.
-        
-        If the items of `iterable` are Python lists or tuples, each element of `iterable` is added as a
-        separate group.'''
         self.clear()
-        if iterable is None:
-            return
-        for item in iterable:
-            if isinstance(item, list) or isinstance(item, tuple):
-                self.append_group(item)
-            else:
-                self.append(item)
+        if iterable is not None:
+            self.extend(iterable)
 
     def _check_type(self, value):
         '''Subclasses can override to raise an exception if the provided
         value is not of a certain type.
         '''
         pass
 
@@ -231,15 +222,15 @@
             # Node is closer to the end, so seach from there
             node = self._last
             for i in range(self._node_count - index - 1):
                 node = node.prev
             return node
 
     def _insert_first(self, value):
-        '''Inserts `value` as the first item of the list.'''
+        '''Inserts `value` as the first element of the list.'''
         self._first = self._Node(value, parent=self)
         self._last = self._first
         self._node_count += 1
         # First node also forms the head of the first group
         self._setup_single_group()
 
     def _setup_single_group(self):
@@ -314,31 +305,28 @@
             elif self._last_head is old_head:
                 self._last_head = node
             old_head.clear_group_head()
         if self._first_head is old_head:
             self._first_head = node
 
     def _insert_new_group_at_node(self, node: 'GroupedList._Node'):
-        if node is self._first:
-            # First node is always already a group.
-            return
         node.is_group_head = True
         prev_group_head = self._find_group_head(node.prev)
         node.prev_head = prev_group_head
         node.next_head = prev_group_head.next_head
         if prev_group_head.next_head is not None:
             prev_group_head.next_head.prev_head = node
         prev_group_head.next_head = node
         if self._last_head is prev_group_head:
             self._last_head = node
         self._group_count += 1
 
     def _find_group_head(self, node: 'GroupedList._Node') -> 'GroupedList._Node':
         '''Search for the next group head, beginning at `node`, and returning the group head node.'''
-        while node is not None and not node.is_group_head:
+        while not node.is_group_head:
             node = node.prev
         return node
 
     def _pop_node(self, node: 'GroupedList._Node'):
         '''Remove `node` from this list, and returns the node's value.'''
         self._check_is_child(node)
         if self._node_count == 1:
@@ -474,41 +462,37 @@
         self._check_type(value)
         if self._node_count == 0:
             self._insert_first(value)
         else:
             self._insert_after(self._last, value, new_group)
                
     def append_group(self, iterable):
-        '''Appends each item of `iterable` to the end of this list.
+        '''Appends each element of `iterable` to the end of this list.
         
-        The new items all form a single new group.'''
+        The new elements all form a single new group.'''
         is_first_item = True
         for item in iterable:
             self.append(item, new_group=is_first_item)
             is_first_item = False
 
     def extend(self, iterable):
-        '''Appends each item of `iterable` to the end of this list.'''
+        '''Appends each element of `iterable` to the end of this list.'''
         for item in iterable:
             self.append(item)
 
     def insert(self, index: int, value):
         '''Inserts `value` into this list at the given `index`.'''
         self._check_type(value)
         if index == 0:
             self.prepend(value)
         elif index == self._node_count:
             self.append(value)
         else:
             self._insert_before(self._node_at(index), value)
 
-    def insert_group_at(self, index: int = None):
-        index = self._conform_index(index)
-        self._insert_new_group_at_node(self._node_at(index))
-
     def pop(self, index: int = None):
         '''Removes the item at the given `index`, and returns its value.'''
         if index is None:
             index = self._node_count - 1
         index = self._conform_index(index)
         return self._pop_node(self._node_at(index))
 
@@ -529,25 +513,19 @@
         self._first: GroupedList._Node = None          # First node
         self._last: GroupedList._Node = None           # Last node
         self._node_count: int = 0                    # Count of nodes
         self._first_head: GroupedList._Node = None     # First node that is a group head
         self._last_head: GroupedList._Node = None      # Last node that is a group head
         self._group_count: int = 0                   # Count of groups
 
-    def clear_groups(self):
-        '''Clears all existing groups and replaces them with a single new group containing all the items
-        in the list.'''
-        for node in self._node_iter():
-            node.clear_group_head()
-        self._setup_single_group()
-
     def reverse(self):
-        '''Reverses the items of this list in-place.
+        '''Reverses the elements of this list in-place.
         
-        For simplicity, this also clears all existing groups and places all list items in one new group.
+        For simplicity, this also clears all existing groups and places all elements
+        in one new group.
         '''
         if self._node_count == 0:
             return
         node = self._last
         while node is not None:
             (node.next, node.prev) = (node.prev, node.next) # Swap next and prev links
             # Clear groups:
@@ -641,15 +619,15 @@
             yield node.value
             node = node.next
 
     def __eq__(self, other) -> bool:
         return self.equals(other)
 
     def equals(self, other_iterable, compare_groups=True) -> bool:
-        '''Returns `True` if each item in this list equals the corresponding item in `other_iterable`,
+        '''Returns `True` if each element of this list equals the corresponding element in `other_iterable`,
         otherwise `False`.
         
         If `compare_groups` is `True`, `other_iterable` must also be a `GroupedList` and the groups of the
         two lists must match, otherwise returns `False`.'''
         if len(self) != len(other_iterable):
             return False
         if compare_groups:
```

### Comparing `bibleref-0.15.0/src/bibleref.egg-info/PKG-INFO` & `bibleref-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibleref
-Version: 0.15.0
+Version: 0.9.0
 Summary: A package for handling references to Bible books, verses and verse-ranges.
 Project-URL: Documentation, https://multiscript.app/bibleref
 Project-URL: Source, https://github.com/multiscript/bibleref
 Project-URL: Issue Tracker, https://github.com/multiscript/bibleref/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,190 +13,114 @@
 Classifier: Topic :: Religion
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bibleref
 
-## Overview
-
 **bibleref is a Python package for handling references to Bible books, verses and verse-ranges, including string
-parsing and conversion.** Its only dependency is the [Lark](https://github.com/lark-parser/lark) parsing toolkit.
+parsing and conversion.** It's designed for future use with [Multiscript](https://multiscript.app), but it can be
+used as a standalone package. Its only dependency is the [Lark](https://github.com/lark-parser/lark) parsing toolkit.
 
 `bibleref` defines the following primary classes:
   - `bibleref.ref.BibleBook`:      An Enum of books in the Bible, with extra methods.
   - `bibleref.ref.BibleVerse`:     A reference to a single Bible verse (e.g. Matt 2:3)
   - `bibleref.ref.BibleRange`:     A reference to a continuous range of Bible verses (e.g. Matt 2:3-4:5)
   - `bibleref.ref.BibleRangeList`: A specialised list of `BibleRange` elements, allowing for grouping and
   set-style operations.
 
 (There is no `BibleChapter` class, as chapters are usually best handled as a `BibleRange`.)
 
 For convenience these classes can be directly imported from `bibleref`. They can each convert to and from strings.
 `BibleRange` and `BibleRangeList` implement common set operations (such as union, intersection, difference and 
 symmetric difference).
 
-## Docs
+# Docs
 
 See [multiscript.app/bibleref](https://multiscript.app/bibleref)
 
-## Examples
+# Examples
 
 ```python
->>> import bibleref
 >>> from bibleref import *
->>>                             # Parse from string
+>>> # Parse a string of Bible ranges...
 >>> range_list = BibleRangeList("Mark 2-3:6; 4; 6:1-6, 30-44, 56; Luke 2")
->>> print(range_list)           # Convert back to a string
+>>> print(range_list)               # Convert back to string
 Mark 2-3:6; 4; 6:1-6, 30-44, 56; Luke 2
 >>> len(range_list)
 6
->>> range_list[0]               # Individual ranges from a list
+>>> range_list[0]                   # Indiv ranges from a list
 BibleRange(Mark 2-3:6)
->>> range_list[1]
-BibleRange(Mark 4)
->>> range_list[5].start         # Start and...
+>>> range_list[5].start             # Start and...
 BibleVerse(Luke 2:1)
->>> range_list[5].end           # ...end verses of a range.
+>>> range_list[5].end               # ...end verses of a range.
 BibleVerse(Luke 2:52)
->>> range_list[5].end.book      # Verse attributes
+>>> range_list[5].end.book          # Verse attributes
 <BibleBook.Luke: 'Luke'>
 >>> range_list[5].end.chap_num
 2
 >>> range_list[5].end.verse_num
 52
 >>> len(range_list.groups)
 4
->>> range_list.groups[2]        # Indivdual range groups from a list
+>>> range_list.groups[2]            # Range groups from a list
 GroupView([BibleRange(Mark 6:1-6), BibleRange(Mark 6:30-44), BibleRange(Mark 6:56)])
->>> range_list.groups[2][0]     # Individual ranges within the group
+>>> range_list.groups[2][0]         # Indiv ranges within the group
 BibleRange(Mark 6:1-6)
 >>> range_list.groups[2][1]        
 BibleRange(Mark 6:30-44)
 >>> range_list.groups[2][2]
 BibleRange(Mark 6:56)
->>> BibleVerse('Mark 2:23') + 10 # Verse addition / subtraction
+>>> BibleVerse('Mark 2:23') + 10    # Verse addition / subtraction
 BibleVerse(Mark 3:5)
->>> BibleVerse('Mark 3:5') - BibleVerse('Mark 2:23')
-10
->>> BibleRange('1 John').split(by_chap=True, num_verses=15) # Range splits
-BibleRangeList("1 John 1, 2:1-15, 16-29, 3:1-15, 16-24, 4:1-15, 16-21, 5:1-15, 16-21")
->>> for verse in BibleRange('Mark 6:1-3'): # Range iteration
-...     print(verse)
+>>> BibleRange('1 John').split(by_chap=True, num_verses=10) # Range splits
+BibleRangeList("1 John 1, 2:1-10, 11-20, 21-29, 3:1-10, 11-20, 21-24, 4:1-10, 11-20, 21, 5:1-10, 11-20, 21")
+>>> for verse in BibleRange('Mark 6:1-3'): 
+...     print(verse)                # Range iteration
 ... 
 Mark 6:1
 Mark 6:2
 Mark 6:3
->>> bibleref.flags = BibleFlag.MULTIBOOK   # Enable multi-book ranges
->>> BibleRange('Matt 10-John 10')
-BibleRange(Matthew 10-John 10)
+>>> BibleRange('Matt 2:3-John 4:5', flags=BibleFlag.MULTIBOOK) # Multibook ranges
+BibleRange(Matthew 2:3-John 4:5)
 >>> list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-16")
->>> list_2 = BibleRangeList("John 1-3; Luke 9; Matt 3-5; Mark 12")
->>> list_1 | list_2                     # Union
-BibleRangeList("Matthew 2-5; Mark 6-8; 12; Luke 9-12; John 1-3; 14-16")
->>> list_1 & list_2                     # Intersection
-BibleRangeList("Matthew 3-4")
->>> list_1 - list_2                     # Difference
-BibleRangeList("Matthew 2; Mark 6-8; Luke 10-12; John 14-16")
->>> list_1 ^ list_2                     # Symmetric difference
-BibleRangeList("Matthew 2; 5; Mark 6-8; 12; Luke 9-12; John 1-3; 14-16")
->>> range_list = BibleRangeList("Mark 3:2-4:5; 1 John 1:5-3 John 8;")
->>> range_list.verse_count()            # Count of verses
-161
->>> range_list.chap_count()             # Count of chapters (incl partial)
-9
->>> range_list.chap_count(whole=True)   # Count of chapters (whole only)
-5
->>> range_list.book_count()             # Count of books (incl partial)
-4
->>> range_list.book_count(whole=True)   # Count of books (whole only)
-1
-```
-
-## List Grouping
-
-Bible ranges in a list can be separated by two different characters, known here as the *major list separator*
-('`;`' by default), and the *minor list separator* ('`,`' by default). These separators play two roles: distinguishing
-between 'bare' chapter and verse numbers (i.e. those not preceded by book names), and controlling how Bible ranges are
-grouped within a list.
-
-The major list separator (`;`) indicates any bare number that follows is a chapter number. It also marks the start of
-a new group. It is usually used between ranges in different chapters.
-
-The minor list separator (`,`) indicates any bare number that follows is of the same kind as the previous number
-(whether a chapter or verse number). It also marks the continuation of the same group. It is usually used between
-ranges within the same chapter.
-
-The groups of a `BibleRangeList` are accessed through its `groups` property. Alternative, you can index each
-`BibleRange` directly (e.g. `range_list[1]`), ignoring the groupings.
-
-For example:
-```python
->>> from bibleref import *
->>> range_list = BibleRangeList("Matt 2:3-4, 5-7, 9-12") # One group of three verse ranges
->>> len(range_list.groups)
-1
->>> range_list[0]
-BibleRange(Matthew 2:3-4)
->>> range_list[1]
-BibleRange(Matthew 2:5-7)
->>> range_list[2]
-BibleRange(Matthew 2:9-12)
->>> range_list = BibleRangeList("Matt 2:3-4; 5-7, 9-12") # Two groups: one verse range, two chapter ranges
->>> len(range_list.groups)
-2
->>> range_list[0]             # Range access directly
-BibleRange(Matthew 2:3-4)
->>> range_list.groups[0][0]   # Same range accessed through its group
-BibleRange(Matthew 2:3-4)
->>> range_list.groups[1]      # Next group
-GroupView([BibleRange(Matthew 5-7), BibleRange(Matthew 9-12)])
->>> range_list.groups[1][0]
-BibleRange(Matthew 5-7)
->>> range_list.groups[1][1]   
-BibleRange(Matthew 9-12)
->>> range_list[2]             # Same range as previous line, but accessed directly
-BibleRange(Matthew 9-12)
->>> range_list = BibleRangeList("Matt 2:3-4, Matt 5-7, 9-12") # One group: one verse range, two chapter ranges
->>> len(range_list.groups)
-1
->>> range_list[1]
-BibleRange(Matthew 5-7)
->>> range_list[2]
-BibleRange(Matthew 9-12)
+>>> list_2 = BibleRangeList("John 1-3; Luke 9-11, 13; Matt 3-5; Mark 12")
+>>> list_1 | list_2                 # Union of range lists
+BibleRangeList("Matthew 2-5, Mark 6-8, 12, Luke 9-13, John 1-3, 14-16")
+>>> list_1 & list_2                 # Intersection range lists
+BibleRangeList("Matthew 3-4, Luke 10-11")
+>>> list_1 - list_2                 # Difference of range lists
+BibleRangeList("Matthew 2, Mark 6-8, Luke 12, John 14-16")
+>>> list_1 ^ list_2                 # Symmetric difference of range lists
+BibleRangeList("Matthew 2, 5, Mark 6-8, 12, Luke 9, 12-13, John 1-3, 14-16")
 ```
 
-`bibleref.ref.BibleRangeList.regroup()` removes the existing groups in the list, and places the list items into
-their most natural new groupings.
-
-The major and minor list separator characters can be changed through the `bibleref.data.BibleData` singleton returned
-by `bible_data()`.
-
-## Attribution
+# Attribution
 
 The set operations and linked-list implementation in this package are derived from
 [python-ranges](https://github.com/Superbird11/ranges), under the MIT Licence.
 
 Other ideas in this package were developed from [python-scriptures](https://github.com/davisd/python-scriptures),
 under the BSD-3-Clause license.
 
-## Installation
+# Installation
 
    `pip install bibleref`
 
-## Build Instructions
+# Build Instructions
 
 Use these instructions if you’re building from the source. bibleref has been developed on Python 3.10, but should
 work on several earlier versions as well.
 
 1. `git clone https://github.com/multiscript/bibleref/`
 1. `cd bibleref`
 1. `python3 -m venv venv` (Create a virtual environment.)
    - On Windows: `python -m venv venv`
 1. `source venv/bin/activate` (Activate the virtual environment.)
-   - In Windows cmd.exe: `venv\Scripts\\activate.bat`
-   - In Windows powershell: `.\\venv\Scripts\Activate.ps1` You may first need to run `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`
+   - In Windows cmd.exe: `venv\Scripts\activate.bat`
+   - In Windows powershell: `.\venv\Scripts\Activate.ps1` You may first need to run `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`
 1. For development work...
    - `pip install -e .` (Creates an editable local install)
 1. ...or to build the package:
    - `pip install build`
    - `python -m build`
+
```

### Comparing `bibleref-0.15.0/test/test_bibleref.py` & `bibleref-0.9.0/test/test_bibleref.py`

 * *Files identical despite different names*

### Comparing `bibleref-0.15.0/test/test_parser.py` & `bibleref-0.9.0/test/test_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pprint import pprint
 import unittest
 
 from bibleref.ref import BibleBook, BibleRange, BibleRefParsingError
 from bibleref.parser import _parse
 
 class TestBibleParser(unittest.TestCase):
-    def test_parse_success(self):
+    def test_parse(self):
         try:
             range_groups_list = _parse("Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3.16-18; 10-14:2;" + 
                                       "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10")
         except BibleRefParsingError as e:
             self.fail(str([str(e), e.start_pos, e.end_pos]))
 
         # print(tree.pretty())
@@ -30,19 +30,7 @@
                 BibleRange(BibleBook.Rom, 4, 2, None, 5, 2),
                 BibleRange(BibleBook.Rom, 5, 10),
             ]
         ]
         pprint(range_groups_list)
         # pprint(expected_list)
         self.assertEqual(range_groups_list, expected_list)
-
-    def test_parse_failure(self):
-        error = None
-        try:
-            _parse("Mark 2, 20, 3")
-        except BibleRefParsingError as e:
-            error = e
-        
-        self.assertIsNotNone(error)
-        self.assertEqual(error.start_pos, 8)
-        self.assertEqual(error.end_pos, 10)
-
```

### Comparing `bibleref-0.15.0/test/test_reference.py` & `bibleref-0.9.0/test/test_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,19 @@
 import unittest
-
-import bibleref
 from bibleref.ref import BibleBook, BibleVerse, BibleRange, BibleRangeList, \
                             BibleFlag, BibleVersePart as BVP, InvalidReferenceError, \
                             MultibookRangeNotAllowedError
 
 
 class TestBibleReference(unittest.TestCase):
     def test_bible_books(self):
         self.assertEqual(BibleBook.from_str("Gen"), BibleBook.Gen)
         self.assertEqual(BibleBook.from_str("Mt"), BibleBook.Matt)
         self.assertEqual(BibleBook.from_str("Rev"), BibleBook.Rev)
 
-    def test_bible_book_ranges(self):
-        self.assertEqual(BibleBook.Matt.range(), BibleRange("Matt 1:1-28:20"))
-        self.assertEqual(BibleBook.Matt.chap_range(2), BibleRange("Matt 2:1-23"))
-
-    def test_bible_book_counts(self):
-        self.assertEqual(BibleBook.Phil.verse_count(), 104) # Check one book manually
-        for book in BibleBook:
-            self.assertEqual(book.verse_count(), BibleRange(book.title).verse_count())
-            self.assertEqual(book.chap_count(), BibleRange(book.title).chap_count())
-
-    def test_bible_book_chap_ranges(self):
-        self.assertEqual(BibleBook.Mark.chap_ranges(),
-            BibleRangeList("Mark 1; 2; 3; 4; 5; 6; 7; 8; 9; 10; 11; 12; 13; 14; 15; 16"))
-
-        self.assertEqual(BibleBook.Mark.chap_ranges(regroup=False),
-            BibleRangeList("Mark 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16"))
-
     def test_bible_verses(self):
         self.assertRaises(ValueError, lambda: BibleVerse(BibleBook.Matt, 2, 3, 4))
         self.assertRaises(ValueError, lambda: BibleVerse(BibleBook.Matt, 2))
         self.assertRaises(ValueError, lambda: BibleVerse(True))
         self.assertRaises(InvalidReferenceError, lambda: BibleVerse("Not real book", 2, 3))
         self.assertRaises(ValueError, lambda: BibleVerse(BibleBook.Matt, [], []))
         self.assertRaises(InvalidReferenceError, lambda: BibleVerse(BibleBook.Matt, 50, 3))
@@ -80,51 +61,22 @@
         verse_with_1 = BibleVerse(BibleBook.Psa, 3, 1)
         no_verse_0 = BibleVerse(BibleBook.Matt, 2, 3)
         self.assertEqual(verse_with_0.verse_0_to_1(), verse_with_1)
         self.assertEqual(verse_with_1.verse_1_to_0(), verse_with_0)
         self.assertEqual(no_verse_0.verse_0_to_1(), no_verse_0)
         self.assertEqual(no_verse_0.verse_1_to_0(), no_verse_0)
 
-    def test_bible_verse_bool_tests(self):
-        self.assertTrue(BibleVerse(BibleBook.Matt, 2, 1).is_first_in_chap())
-        self.assertFalse(BibleVerse(BibleBook.Matt, 2, 2).is_first_in_chap())
-        self.assertTrue(BibleVerse(BibleBook.Matt, 2, 23).is_last_in_chap())
-        self.assertFalse(BibleVerse(BibleBook.Matt, 2, 22).is_last_in_chap())
-
-        self.assertTrue(BibleVerse(BibleBook.Matt, 1, 1).is_first_in_book())
-        self.assertFalse(BibleVerse(BibleBook.Matt, 1, 2).is_first_in_book())
-        self.assertTrue(BibleVerse(BibleBook.Matt, 28, 20).is_last_in_book())
-        self.assertFalse(BibleVerse(BibleBook.Matt, 28, 19).is_last_in_book())
-
-    def test_verse_ranges(self):
-        bible_verse = BibleVerse("Matt 3:8")
-        self.assertEqual(bible_verse.chap_range(), BibleRange("Matt 3"))
-        self.assertEqual(bible_verse.book_range(), BibleRange("Matt"))
-
     def test_verse_arithmetic(self):
         self.assertEqual(BibleVerse("Ps 3:8") + 1, BibleVerse("Ps 4:1"))
         self.assertEqual(BibleVerse("Ps 4:1") - 1, BibleVerse("Ps 3:8"))
-        self.assertEqual(BibleVerse("Ps 3:8") - BibleVerse("Ps 4:1"), -1)
-        self.assertEqual(BibleVerse("Ps 4:1") - BibleVerse("Ps 3:8"), 1)
-
-        self.assertEqual(BibleVerse("Ps 3:8").add(1, flags=BibleFlag.VERSE_0),
+        self.assertEqual(BibleVerse("Ps 3:8").add_num_verses(1, flags=BibleFlag.VERSE_0),
                         BibleVerse("Ps 4:0", flags=BibleFlag.VERSE_0))
         self.assertEqual(BibleVerse("Ps 4:0", flags=BibleFlag.VERSE_0) - 1, BibleVerse("Ps 3:8"))
-        self.assertEqual(BibleVerse("Ps 3:8").subtract(BibleVerse("Ps 4:0", flags=BibleFlag.VERSE_0),
-                         flags=BibleFlag.VERSE_0), -1)
-        self.assertEqual(BibleVerse("Ps 4:0", flags=BibleFlag.VERSE_0).subtract(BibleVerse("Ps 3:8"),
-                         flags=BibleFlag.VERSE_0), 1)
-        
         self.assertEqual(BibleVerse("John 1:50") + 11, BibleVerse("John 2:10"))
-        self.assertEqual(BibleVerse("John 1:50") - BibleVerse("John 2:10"), -11)
-        self.assertEqual(BibleVerse("John 2:10") - BibleVerse("John 1:50"), 11)
-
         self.assertEqual(BibleVerse("John 2:10") - 12, BibleVerse("John 1:49"))
-        self.assertEqual(BibleVerse("John 2:10") - BibleVerse("John 1:49"), 12)
-        self.assertEqual(BibleVerse("John 1:49") - BibleVerse("John 2:10"), -12)
 
     def test_bible_verse_to_string(self):
         verse = BibleVerse(BibleBook.Matt, 5, 3)
         self.assertEqual(str(verse), "Matthew 5:3")
         self.assertEqual(verse.str(abbrev=True), "Matt 5:3")
         self.assertEqual(verse.str(alt_sep=True), "Matthew 5.3")
         self.assertEqual(verse.str(nospace=True), "Matthew5:3")
@@ -206,26 +158,14 @@
         self.assertEqual(BibleRange(BibleBook.John,    5, None, BibleBook.Matt,    2,    3, flags=BibleFlag.MULTIBOOK), BibleRange("Matt 2:3-John 5", flags=BibleFlag.MULTIBOOK))
         self.assertEqual(BibleRange(BibleBook.Matt,    6,    7,           None,    2, None), BibleRange("Matt 2-6:7"))
         self.assertEqual(BibleRange(BibleBook.Matt,    6,    7,           None,    2,    3), BibleRange("Matt 2:3-6:7"))
         self.assertEqual(BibleRange(BibleBook.John,    8,   10, BibleBook.Matt, None, None, flags=BibleFlag.MULTIBOOK), BibleRange("Matt-John 8:10", flags=BibleFlag.MULTIBOOK))
         self.assertEqual(BibleRange(BibleBook.John,    8,   10, BibleBook.Matt,    2, None, flags=BibleFlag.MULTIBOOK), BibleRange("Matt 2-John 8:10", flags=BibleFlag.MULTIBOOK))
         self.assertEqual(BibleRange(BibleBook.John,    8,   10, BibleBook.Matt,    2,    3, flags=BibleFlag.MULTIBOOK), BibleRange("Matt 2:3-John 8:10", flags=BibleFlag.MULTIBOOK))
 
-    def test_bibleref_flags(self):
-        orig_flags = bibleref.flags
-        bibleref.flags = BibleFlag.NONE
-        self.assertRaises(bibleref.ref.MultibookRangeNotAllowedError, lambda: BibleRange(BibleBook.Matt, None, None, BibleBook.John))
-        self.assertRaises(bibleref.ref.InvalidReferenceError, lambda: BibleVerse(BibleBook.Psa, 3, 0))
-        
-        bibleref.flags = BibleFlag.ALL
-        bible_range = BibleRange(BibleBook.Matt, None, None, BibleBook.John)
-        bible_verse = BibleVerse(BibleBook.Psa, 3, 0)
-        
-        bibleref.flags = orig_flags
-
     def test_whole_bible(self):
         self.assertEqual(BibleRange.whole_bible(), BibleRange("Gen-Rev", flags=BibleFlag.MULTIBOOK))
 
     def test_bible_range_comparison(self):
         self.assertTrue(BibleRange("Matt 2:3-4:5") < BibleRange("Matt 2:3-4:6"))
         self.assertTrue(BibleRange("Matt 2:3-4:5") <= BibleRange("Matt 2:3-4:6"))
         self.assertFalse(BibleRange("Matt 2:3-4:5") == BibleRange("Matt 2:3-4:6"))
@@ -273,72 +213,63 @@
             BibleVerse(BibleBook.Matt, 28, 20),
             BibleVerse(BibleBook.Mark, 1, 1),
             BibleVerse(BibleBook.Mark, 1, 2),
             BibleVerse(BibleBook.Mark, 1, 3),                         
         ]
         self.assertEqual(list(bible_range), expected_list)       
 
-    def test_range_ranges(self):
-        bible_range = BibleRange("Matt 3:8-John 4:9", flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(bible_range.chap_range(), BibleRange("Matt 3-John 4", flags=BibleFlag.MULTIBOOK))
-        self.assertEqual(bible_range.book_range(), BibleRange("Matt-John", flags=BibleFlag.MULTIBOOK))
-
-    def test_range_counts(self):
-        # Multi-book range
-        bible_range = BibleRange("1 John 1:5-3 John 8", flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(bible_range.verse_count(), 122)
-        self.assertEqual(bible_range.chap_count(), 7)
-        self.assertEqual(bible_range.chap_count(whole=True), 5)
-        self.assertEqual(bible_range.book_count(), 3)
-        self.assertEqual(bible_range.book_count(whole=True), 1)
-
-        # Range across 3 chapters
-        bible_range = BibleRange("1 John 1:5-3:10", flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(bible_range.verse_count(), 45)
-        self.assertEqual(bible_range.chap_count(), 3)
-        self.assertEqual(bible_range.chap_count(whole=True), 1)
-        self.assertEqual(bible_range.book_count(), 1)
-        self.assertEqual(bible_range.book_count(whole=True), 0)
-
-        # Range across 2 chapters
-        bible_range = BibleRange("1 John 1:5-2:11", flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(bible_range.verse_count(), 17)
-        self.assertEqual(bible_range.chap_count(), 2)
-        self.assertEqual(bible_range.chap_count(whole=True), 0)
-        self.assertEqual(bible_range.book_count(), 1)
-        self.assertEqual(bible_range.book_count(whole=True), 0)
-
-        # Range across 1 chapter
-        bible_range = BibleRange("3 John 5-10")
-        self.assertEqual(bible_range.verse_count(), 6)
-        self.assertEqual(bible_range.chap_count(), 1)
-        self.assertEqual(bible_range.chap_count(whole=True), 0)
-        self.assertEqual(bible_range.book_count(), 1)
-        self.assertEqual(bible_range.book_count(whole=True), 0)
-
     def test_range_split(self):
         ref = BibleRange("Matt 1:5-John 10:11", flags=BibleFlag.MULTIBOOK)
-        split = ref.split()
-        self.assertEqual(split, BibleRangeList("Matt 1:5-John 10:11", flags=BibleFlag.MULTIBOOK))
+        self.assertRaises(ValueError, lambda: ref.split())
 
         ref = BibleRange("Matt 1:5-John 10:11", flags=BibleFlag.MULTIBOOK)
         split = ref.split(by_book=True)
-        self.assertEqual(split, BibleRangeList("Matt 1:5-28:20; Mark; Luke; John 1-10:11"))
+        print(split)
+        expected =  BibleRangeList(
+                        BibleRange("Matt 1:5-28:20"),
+                        BibleRange("Mark"),
+                        BibleRange("Luke"),
+                        BibleRange("John 1-10:11"),
+                    )
+        self.assertEqual(split, expected)
 
         ref = BibleRange("John 1:11-10:5")
         split = ref.split(by_chap=True)
-        self.assertEqual(split, BibleRangeList("John 1:11-51; 2; 3; 4; 5; 6; 7; 8; 9; 10:1-5"))
+        expected =  BibleRangeList(
+                        BibleRange("John 1:11-51"),
+                        BibleRange("John 2"),
+                        BibleRange("John 3"),
+                        BibleRange("John 4"),
+                        BibleRange("John 5"),
+                        BibleRange("John 6"),
+                        BibleRange("John 7"),
+                        BibleRange("John 8"),
+                        BibleRange("John 9"),
+                        BibleRange("John 10:1-5")
+                    )
+        self.assertEqual(split, expected)
 
         ref = BibleRange("John 1:1-11")
         split = ref.split(by_chap=False, num_verses=10)
-        self.assertEqual(split, BibleRangeList("John 1:1-10, 11"))
+        expected =  BibleRangeList(
+                        BibleRange("John 1:1-10"),
+                        BibleRange("John 1:11"),
+                    )
+        self.assertEqual(split, expected)
 
         ref = BibleRange("John 1:11-10:5")
         split = ref.split(by_chap=False, num_verses=100)
-        self.assertEqual(split, BibleRangeList("John 1:11-3:34; 3:35-5:44; 5:45-7:26; 7:27-9:14; 9:15-10:5"))
+        expected =  BibleRangeList(
+                        BibleRange("John 1:11-3:34"),
+                        BibleRange("John 3:35-5:44"),
+                        BibleRange("John 5:45-7:26"),
+                        BibleRange("John 7:27-9:14"),
+                        BibleRange("John 9:15-10:5")
+                    )
+        self.assertEqual(split, expected)
 
     def test_range_is_disjoint(self):
         test_range = BibleRange("Matt 1:10-15")
         
         self.assertTrue(test_range.is_disjoint(BibleVerse("Matt 1:9")))
         self.assertFalse(test_range.is_disjoint(BibleVerse("Matt 1:10")))        
         
@@ -454,22 +385,18 @@
         self.assertEqual(test_range | BibleRange("Matt 1:13-15"), BibleRangeList("Matt 1:10-15"))
         self.assertEqual(test_range | BibleRange("Matt 1:10-15"), BibleRangeList("Matt 1:10-15"))
         self.assertEqual(test_range | BibleRange("Matt 1:14-20"), BibleRangeList("Matt 1:10-20"))
         self.assertEqual(test_range | BibleRange("Matt 1:15-20"), BibleRangeList("Matt 1:10-20"))
         self.assertEqual(test_range | BibleRange("Matt 1:16-20"), BibleRangeList("Matt 1:10-20"))
         self.assertEqual(test_range | BibleRange("Matt 1:17-20"), BibleRangeList("Matt 1:10-15, 17-20"))
 
-        self.assertEqual(test_range | BibleRangeList("Matt 1:5-8; Mark 1-3"),
-                         BibleRangeList("Matt 1:5-8, 10-15; Mark 1-3"))
-        self.assertEqual(test_range | BibleRangeList("Matt 1:5-9; Mark 1-3"),
-                         BibleRangeList("Matt 1:5-15; Mark 1-3"))
-        self.assertEqual(test_range | BibleRangeList("Matt 1:5-10; Mark 1-3"),
-                         BibleRangeList("Matt 1:5-15; Mark 1-3"))
-        self.assertEqual(test_range | BibleRangeList("Mark 4-6; Matt 1:5-9, 16-20"),
-                         BibleRangeList("Matt 1:5-20; Mark 4-6"))
+        self.assertEqual(test_range | BibleRangeList("Matt 1:5-8; Mark 1-3"), BibleRangeList("Matt 1:5-8, 10-15, Mark 1-3"))
+        self.assertEqual(test_range | BibleRangeList("Matt 1:5-9; Mark 1-3"), BibleRangeList("Matt 1:5-15, Mark 1-3"))
+        self.assertEqual(test_range | BibleRangeList("Matt 1:5-10; Mark 1-3"), BibleRangeList("Matt 1:5-15, Mark 1-3"))
+        self.assertEqual(test_range | BibleRangeList("Mark 4-6; Matt 1:5-9, 16-20"), BibleRangeList("Matt 1:5-20, Mark 4-6"))
 
     def test_range_intersection(self):
         test_range = BibleRange("Matt 1:10-15")
 
         self.assertEqual(test_range & BibleVerse("Matt 1:8"), BibleRangeList())
         self.assertEqual(test_range & BibleVerse("Matt 1:9"), BibleRangeList())
         self.assertEqual(test_range & BibleVerse("Matt 1:10"), BibleRangeList("Matt 1:10"))
@@ -556,16 +483,15 @@
         rng = BibleRange(BibleBook.Exod, 7, 4, None, 10, 29)
         self.assertEqual(str(rng), "Exodus 7:4-10:29")
 
         rng = BibleRange(BibleBook.Exod, 7, 4, None, None, 8)
         self.assertEqual(str(rng), "Exodus 7:4-8")
 
         rng = BibleRange(BibleBook.Exod, 7, 1, None, 10, 12)
-        self.assertEqual(rng.str(force_start_verses=False), "Exodus 7-10:12")
-        self.assertEqual(rng.str(force_start_verses=True), "Exodus 7:1-10:12")
+        self.assertEqual(str(rng), "Exodus 7-10:12")
 
         rng = BibleRange(BibleBook.ICor, 15, 1, BibleBook.IICor, 1, 24, flags=BibleFlag.MULTIBOOK)
         self.assertEqual(str(rng), "1 Corinthians 15-2 Corinthians 1")
 
         rng = BibleRange(BibleBook.Obad, 1, 10, None, 1, 12)
         self.assertEqual(str(rng), "Obadiah 10-12")
 
@@ -605,21 +531,19 @@
             string = orig_range.str(abbrev=False)
             final_range = BibleRange(string)
             self.assertEqual(orig_range, final_range)
 
     def test_bible_range_list(self):
         range_list = BibleRangeList("Mark 3:1-4:2; Mark 5:6-8; Mark 5:10; Matt 4")
         expected_range_str = "Mark 3-4:2; 5:6-8, 10; Matt 4"
-        self.assertEqual(range_list.str(abbrev=True, preserve_groups=False,
-                                        force_start_verses=False), expected_range_str)
+        self.assertEqual(range_list.str(abbrev=True, preserve_groups=False), expected_range_str)
 
         range_list = BibleRangeList([BibleRange("Mark 3:1-4:2"), BibleRange("Mark 5:6-8"),
                                      BibleRange("Mark 5:10"), BibleRange("Matt 4")])
-        self.assertEqual(range_list.str(abbrev=True, preserve_groups=False,
-                                        force_start_verses=False), expected_range_str)
+        self.assertEqual(range_list.str(abbrev=True, preserve_groups=False), expected_range_str)
 
         range_list = BibleRangeList("Mark 3:1-4:2; Mark 5:6-8; Mark 5:10; Matt 4")
         self.assertEqual(range_list, BibleRangeList(range_list))
 
     def test_bible_range_list_verse_0(self):
         list_with_0 = BibleRangeList("Ps 3:0-4:0; Matt 2:3-4:5", flags=BibleFlag.VERSE_0)
         list_with_1 = BibleRangeList("Ps 3:1-4:1; Matt 2:3-4:5", flags=BibleFlag.VERSE_0)
@@ -630,54 +554,21 @@
         list_with_1.verse_1_to_0()
         self.assertEqual(list_with_0, list_with_1)
         no_verse_0.verse_0_to_1()
         self.assertEqual(no_verse_0, BibleRangeList("Matt 2:3-4:5; Mark 6:7-8:9"))
         no_verse_0.verse_1_to_0()
         self.assertEqual(no_verse_0, BibleRangeList("Matt 2:3-4:5; Mark 6:7-8:9"))
 
-    def test_range_list_ranges(self):
-        range_list = BibleRangeList("John 4:9; Luke 1:12; Mark 7:3; Matt 3:8")
-        self.assertEqual(range_list.range(), BibleRange("Matt 3:8-John 4:9", flags=BibleFlag.MULTIBOOK))
-        self.assertEqual(range_list.chap_range(), BibleRange("Matt 3-John 4", flags=BibleFlag.MULTIBOOK))
-        self.assertEqual(range_list.book_range(), BibleRange("Matt-John", flags=BibleFlag.MULTIBOOK))
-
-    def test_range_list_counts(self):
-        range_list = BibleRangeList("1 John 1:5-3 John 8; 1 John 1:5-3:10; 1 John 1:5-2:11; 3 John 5-10",
-                                    flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(range_list.verse_count(), 190)
-        self.assertEqual(range_list.chap_count(), 13)
-        self.assertEqual(range_list.chap_count(whole=True), 6)
-        self.assertEqual(range_list.book_count(), 6)
-        self.assertEqual(range_list.book_count(whole=True), 1)
-
-    def test_regroup(self):
-        range_list = BibleRangeList("Matt 1:4-7, 9-15, 17-20, Luke, John")
-        range_list.regroup()
-        self.assertEqual(range_list, BibleRangeList("Matt 1:4-7, 9-15, 17-20; Luke; John"))
-
-        range_list = BibleRangeList("Matt 1:4-7, 9-15, 17-20, John 2, 3, Luke 2:1-5, 6-10, 11-15")
-        range_list.regroup()
-        self.assertEqual(range_list, BibleRangeList("Matt 1:4-7, 9-15, 17-20; John 2; 3; Luke 2:1-5, 6-10, 11-15"))
-
-    def test_bible_range_list_merge(self):
-        range_list = BibleRangeList("John; Luke; Matt 1:17-20, 12-15, 9-11, 5-7, 4-6", flags=BibleFlag.MULTIBOOK)
-        range_list.sort()
-        range_list.merge(flags=BibleFlag.NONE)
-        self.assertEqual(range_list, BibleRangeList("Matt 1:4-7, 9-15, 17-20; Luke; John"))
-        range_list.merge(flags=BibleFlag.MULTIBOOK)
-        self.assertEqual(range_list, BibleRangeList("Matt 1:4-7, 9-15, 17-20; Luke-John", flags=BibleFlag.MULTIBOOK))
-
-        # Test groups
-        range_list = BibleRangeList([[BibleRange("Mark 3:1-4:2"), BibleRange("Mark 5:6-8")],
-                                      [BibleRange("Mark 5:10"), BibleRange("Matt 4")]])
-        self.assertEqual(len(range_list.groups), 2)
-        self.assertEqual(range_list.groups[0][0], BibleRange("Mark 3:1-4:2"))
-        self.assertEqual(range_list.groups[0][1], BibleRange("Mark 5:6-8"))
-        self.assertEqual(range_list.groups[1][0], BibleRange("Mark 5:10"))
-        self.assertEqual(range_list.groups[1][1], BibleRange("Matt 4"))
+    def test_bible_range_list_compress(self):
+        range = BibleRangeList("John; Luke; Matt 1:17-20, 12-15, 9-11, 5-7, 4-6", flags=BibleFlag.MULTIBOOK)
+        range.sort()
+        range.consolidate(flags=BibleFlag.NONE)
+        self.assertEqual(range, BibleRangeList("Matt 1:4-7, 9-15, 17-20, Luke, John"))
+        range.consolidate(flags=BibleFlag.MULTIBOOK)
+        self.assertEqual(range, BibleRangeList("Matt 1:4-7, 9-15, 17-20, Luke-John", flags=BibleFlag.MULTIBOOK))
 
     def test_bible_range_list_is_disjoint(self):
         test_list = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-16")
 
         self.assertTrue(test_list.is_disjoint(BibleRangeList("Matt 5-7; Mark 9-11; Luke 13-15; John 17-19")))
         self.assertFalse(test_list.is_disjoint(BibleRangeList("Matt 5-7; Mark 9-11; Luke 12-15; John 17-19")))
         self.assertFalse(test_list.is_disjoint(BibleRangeList("Matt 5-7; Mark 8:38-Mark 11; Luke 13-15; John 17-19")))
@@ -691,118 +582,88 @@
         self.assertFalse(test_list in BibleRangeList("Matt 2-3, 4-5; Mark 6-9; Luke 10:2-Luke 12; John"))
         self.assertFalse(test_list in BibleRangeList("Matt 2-3, 4-5; Mark 6-9; Luke 10:2-Luke 12; John 14:2-John 16"))
 
     def test_bible_range_list_union(self):
         list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-16")
         
         list_2 = BibleRangeList("John 1-3; Luke 9; Matt 3-5; Mark 12")
-        self.assertEqual(list_1 | list_2, BibleRangeList("Matt 2-5; Mark 6-8; 12; Luke 9-12; John 1-3; 14-16"))
+        self.assertEqual(list_1 | list_2, BibleRangeList("Matt 2-5, Mark 6-8, 12, Luke 9-12, John 1-3, 14-16"))
 
         list_2 = BibleRangeList("John 12-13; Luke 13-15; Mark 1-3; Matt 15-16")
-        self.assertEqual(list_1 | list_2, BibleRangeList("Matt 2-4; 15-16; Mark 1-3; 6-8; Luke 10-15; John 12-16"))
+        self.assertEqual(list_1 | list_2, BibleRangeList("Matt 2-4, 15-16, Mark 1-3, 6-8, Luke 10-15, John 12-16"))
 
     def test_bible_range_list_intersection(self):
         list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-16")
         
         list_2 = BibleRangeList("John 1-3; Luke 9-10; Matt 3-5; Mark 12")
-        self.assertEqual(list_1 & list_2, BibleRangeList("Matt 3-4; Luke 10"))
+        self.assertEqual(list_1 & list_2, BibleRangeList("Matt 3-4, Luke 10"))
 
         list_2 = BibleRangeList("John 12-15; Luke 12-15; Mark 1-3; Matt 15-16")
-        self.assertEqual(list_1 & list_2, BibleRangeList("Luke 12; John 14-15"))
+        self.assertEqual(list_1 & list_2, BibleRangeList("Luke 12, John 14-15"))
 
     def test_bible_range_list_difference(self):
         list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-18")
         
         list_2 = BibleRangeList("John 1-3; Luke 9-10; Matt 3-5; Mark 12")
-        self.assertEqual(list_1 - list_2, BibleRangeList("Matt 2; Mark 6-8; Luke 11-12; John 14-18"))
+        self.assertEqual(list_1 - list_2, BibleRangeList("Matt 2, Mark 6-8, Luke 11-12, John 14-18"))
 
         list_2 = BibleRangeList("John 16; Luke 11; Mark 1-3; Matt 15-16")
-        self.assertEqual(list_1 - list_2, BibleRangeList("Matt 2-4; Mark 6-8; Luke 10; 12; John 14-15; 17-18"))
+        self.assertEqual(list_1 - list_2, BibleRangeList("Matt 2-4, Mark 6-8, Luke 10, 12, John 14-15, 17-18"))
 
     def test_bible_range_list_sym_difference(self):
         list_1 = BibleRangeList("Matt 2-4; Mark 6-8; Luke 10-12; John 14-18")
         
         list_2 = BibleRangeList("John 1-3; Luke 9-10; Matt 3-5; Mark 12")
-        self.assertEqual(list_1 ^ list_2, BibleRangeList("Matt 2; 5; Mark 6-8; 12; Luke 9; 11-12; John 1-3; 14-18"))
+        self.assertEqual(list_1 ^ list_2, BibleRangeList("Matt 2, 5, Mark 6-8, 12, Luke 9, 11-12, John 1-3, 14-18"))
 
         list_2 = BibleRangeList("John 16; Luke 11; Mark 1-3; Matt 15-16")
         self.assertEqual(list_1 ^ list_2,
-                         BibleRangeList("Matt 2-4; 15-16; Mark 1-3; 6-8; Luke 10; 12; John 14-15; 17-18"))
+                         BibleRangeList("Matt 2-4, 15-16, Mark 1-3, 6-8, Luke 10, 12, John 14-15, 17-18"))
 
     def test_bible_range_list_to_string(self):
         # Start range spans a book, after a ref from same book
         self.assertEqual(BibleRangeList(
             "Matthew 2:3-4:5; Matthew-Mark", flags=BibleFlag.MULTIBOOK).str(),  # Start range spans book
             "Matthew 2:3-4:5; Matthew-Mark")
 
         # Start range spans a chapter from same book, when at verse level
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Don't force start verse to display
-            "Matthew 2:3, Matthew 3-4:5").str(preserve_groups=False, force_start_verses=False),
+        self.assertEqual(BibleRangeList(  # Don't preserve groups
+            "Matthew 2:3, Matthew 3-4:5").str(preserve_groups=False),
             "Matthew 2:3; 3-4:5")
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Force start verse to display
-            "Matthew 2:3, Matthew 3-4:5").str(preserve_groups=False, force_start_verses=True),
-            "Matthew 2:3; 3:1-4:5")
-        self.assertEqual(BibleRangeList(  # Preserve groups, after major sep.
-            "Matthew 2:3; Matthew 3-4:5").str(force_start_verses=False),
+        self.assertEqual(BibleRangeList(  # Preserve groups, after major sep
+            "Matthew 2:3; Matthew 3-4:5").str(),
             "Matthew 2:3; 3-4:5")
-        self.assertEqual(BibleRangeList(  # Preserve groups, after major sep.
-            "Matthew 2:3; Matthew 3-4:5").str(force_start_verses=True),
-            "Matthew 2:3; 3:1-4:5")
         self.assertEqual(BibleRangeList(  # Preserve groups, after minor sep
             "Matthew 2:3, Matthew 3-4").str(),
             "Matthew 2:3, 3:1-4:25")
         # Start range spans a chapter from same book, when at chap level
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Don't force start verse to display
-            "Matthew 2, Matthew 3-4:5").str(preserve_groups=False, force_start_verses=False),
+        self.assertEqual(BibleRangeList(  # Don't preserve groups
+            "Matthew 2, Matthew 3-4:5").str(preserve_groups=False),
             "Matthew 2; 3-4:5")
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Force start verse to display
-            "Matthew 2, Matthew 3-4:5").str(preserve_groups=False, force_start_verses=True),
-            "Matthew 2; 3:1-4:5")
         self.assertEqual(BibleRangeList(  # Preserve groups, after major sep
-            "Matthew 2; Matthew 3-4:5").str(preserve_groups=False, force_start_verses=False),
+            "Matthew 2; Matthew 3-4:5").str(preserve_groups=False),
             "Matthew 2; 3-4:5")
-        self.assertEqual(BibleRangeList(  # Preserve groups, after major sep
-            "Matthew 2; Matthew 3-4:5").str(preserve_groups=False, force_start_verses=True),
-            "Matthew 2; 3:1-4:5")
-        self.assertEqual(BibleRangeList(  # Preserve groups, after minor sep, spanning whole chaps
-            "Matthew 2, Matthew 3:1-4:25").str(force_start_verses=False),
-            "Matthew 2, 3-4")
         self.assertEqual(BibleRangeList(  # Preserve groups, after minor sep, spanning whole chaps
-            "Matthew 2, Matthew 3:1-4:25").str(force_start_verses=True),
+            "Matthew 2, Matthew 3:1-4:25").str(),
             "Matthew 2, 3-4")
         self.assertEqual(BibleRangeList(  # Preserve groups, after minor sep, spanning partial chaps
             "Matthew 2, Matthew 3:1-4:5").str(),
             "Matthew 2, 3:1-4:5")
         # Start range spans a chapter from different book
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Don't force start verse display
-            "Matthew 2:3, Mark 3-4:5").str(preserve_groups=False, force_start_verses=False),
+        self.assertEqual(BibleRangeList(  # Don't preserve groups
+            "Matthew 2:3, Mark 3-4:5").str(preserve_groups=False),
             "Matthew 2:3; Mark 3-4:5")
-        self.assertEqual(BibleRangeList(  # Don't preserve groups. Force start verse display
-            "Matthew 2:3, Mark 3-4:5").str(preserve_groups=False, force_start_verses=True),
-            "Matthew 2:3; Mark 3:1-4:5")
         self.assertEqual(BibleRangeList(  # Preserve groups
-            "Matthew 2:3, Mark 3-4:5").str(force_start_verses=False),
+            "Matthew 2:3, Mark 3-4:5").str(),
             "Matthew 2:3, Mark 3-4:5")
-        self.assertEqual(BibleRangeList(  # Preserve groups
-            "Matthew 2:3, Mark 3-4:5").str(force_start_verses=True),
-            "Matthew 2:3, Mark 3:1-4:5")
   
         # Start range is just a verse from same book
-        self.assertEqual(BibleRangeList(  # Same chap at verse level. End verse within same chap
-            "Matthew 2:3, Matthew 2:6-10").str(),
-            "Matthew 2:3, 6-10")
-        self.assertEqual(BibleRangeList(  # Same chap at verse level. End verse in a different chap
+        self.assertEqual(BibleRangeList(  # Same chap at verse level
             "Matthew 2:3, Matthew 2:6-5:7").str(),
-            "Matthew 2:3, 2:6-5:7")
-        self.assertEqual(BibleRangeList(  # Same chap at verse level. End verse in diff chap. Don't preserve groups.
-            "Matthew 2:3, Matthew 2:6-5:7").str(preserve_groups=False),
-            "Matthew 2:3; 2:6-5:7")
-        self.assertEqual(BibleRangeList(  # Same chap at verse level. End verse in a different book
-            "Matthew 2:3, Matthew 2:6-John 5:7", flags=BibleFlag.MULTIBOOK).str(),
-            "Matthew 2:3, 2:6-John 5:7")
+            "Matthew 2:3, 6-5:7")
         self.assertEqual(BibleRangeList(  # Same chap at chap level, don't preserve groups
             "Matthew 2, Matthew 2:6-5:7").str(preserve_groups=False),
             "Matthew 2; 2:6-5:7")
         self.assertEqual(BibleRangeList(  # Same chap at chap level, preserve groups
             "Matthew 2, Matthew 2:6-5:7").str(),
             "Matthew 2, 2:6-5:7")
         self.assertEqual(BibleRangeList(  # Different chap, don't preserve groups
@@ -883,34 +744,33 @@
             "Matthew 2:3-4:5, 7; Matthew 4:9, Matthew 11-12").str(preserve_groups=False),
             "Matthew 2:3-4:5, 7, 9; 11-12")
 
 
         # Test a variety of types
         self.assertEqual(BibleRangeList(
             "Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3:16-18; 10-14:2; " + 
-            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(force_start_verses=False),
+            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(),
             "Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3:16-18; 10-14:2; " +
             "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10")
         # Test a variety of types, with abbreviations
         self.assertEqual(BibleRangeList(
             "Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3:16-18; 10-14:2; " + 
-            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True, force_start_verses=False),
+            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True),
             "Matt; Mark 2; Jude 5; 8; Obad 2-3; John 3:16-18; 10-14:2; " +
             "Rom 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10")
         # Test a variety of types, with abbreviations, with alt verse separator
         self.assertEqual(BibleRangeList(
             "Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3:16-18; 10-14:2; " + 
-            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True, alt_sep=True, force_start_verses=False),
+            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True, alt_sep=True),
             "Matt; Mark 2; Jude 5; 8; Obad 2-3; John 3.16-18; 10-14.2; " +
             "Rom 1.10-22; 2; 3.20-22, 24, 4.2-5.2, 10")
         # Test a variety of types, with abbreviations, with alt verse separator, with no space
         self.assertEqual(BibleRangeList(
             "Matthew; Mark 2; Jude 5; 8; Obadiah 2-3; John 3:16-18; 10-14:2; " + 
-            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True, alt_sep=True, nospace=True,
-                                                               force_start_verses=False),
+            "Romans 1:10-22; 2; 3:20-22, 24, 4:2-5:2, 10").str(abbrev=True, alt_sep=True, nospace=True),
             "Matt;Mark2;Jude5;8;Obad2-3;John3.16-18;10-14.2;" +
             "Rom1.10-22;2;3.20-22,24,4.2-5.2,10")
 
     def test_bible_range_list_sort(self):
         range_list_str = "Matt 2:3-4:5; Mark 3:4-5:6; Mark 3:4-5:5; Gen 1:2-3:4; " + \
                          "Matt 2:3-4:4; 1 Sam 2:2-3:3; Matt 1:2-11:1"
         range_list = BibleRangeList(range_list_str)
```

### Comparing `bibleref-0.15.0/test/test_util.py` & `bibleref-0.9.0/test/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,39 +181,51 @@
 
     def test_iadd(self):
         test_list = GroupedList([5, 8, 2, 7, 3, 10])
         test_list += [12, 9, 20]
         self.assertListEqual(list(test_list), [5, 8, 2, 7, 3, 10, 12, 9, 20])
 
     def test_group_construction(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6], [3, 7, 5]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
+        test_list.append_group([3, 7, 5])
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6], [3, 7, 5]])
 
     def test_groups_view(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6], [3, 7, 5]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
+        test_list.append_group([3, 7, 5])
         self.assertEqual(len(test_list.groups), 3)
         self.assertEqual(test_list.groups[2].group_head.value, 3)
         group_list = list(test_list.groups)
         self.assertEqual(group_list[0].group_head.value, 2)
         self.assertEqual(group_list[1].group_head.value, 1)
         self.assertEqual(group_list[2].group_head.value, 3)
 
     def test_group_view(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6], [3, 7, 5]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
+        test_list.append_group([3, 7, 5])
         group_0 = test_list.groups[0]
         self.assertEqual(group_0[0], 2)
         self.assertEqual(group_0[1], 8)
         self.assertEqual(group_0[2], 4)
 
         self.assertEqual(test_list.groups[2][0], 3)
         self.assertEqual(test_list.groups[2][1], 7)
         self.assertEqual(test_list.groups[2][2], 5)
 
     def test_group_head_deletion(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6], [3, 7, 5]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
+        test_list.append_group([3, 7, 5])
         group_1 = test_list.groups[1]
         group_2 = test_list.groups[2]
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6], [3, 7, 5]])
         self.assertEqual(len(test_list.groups), 3)
         self.assertEqual(group_1[0], 1)
         self.assertEqual(group_2[0], 3)
 
@@ -238,23 +250,27 @@
         del test_list[3]
         del test_list[3]
         del test_list[3]
         self.assertEqual(len(test_list.groups), 1)
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4]])
 
     def test_group_prepend(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6]])
         test_list.prepend(3, new_group=False)
         self.assertEqual(test_list.to_nested_lists(), [[3, 2, 8, 4], [1, 9, 6]])
         test_list.prepend(7, new_group=True)
         self.assertEqual(test_list.to_nested_lists(), [[7], [3, 2, 8, 4], [1, 9, 6]])
 
     def test_group_insert_before(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6]])
         self.assertIs(test_list._first_head, test_list._node_at(0))
         self.assertIs(test_list._last_head, test_list._node_at(3))
 
         test_list._insert_before(test_list._node_at(3), 7, new_group=False)
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [7, 1, 9, 6]])
         self.assertIs(test_list._first_head, test_list._node_at(0))
@@ -278,70 +294,72 @@
         test_list = GroupedList([5])
         test_list._insert_before(test_list._node_at(0), 6, new_group=False)
         self.assertEqual(test_list.to_nested_lists(), [[6, 5]])
         self.assertIs(test_list._first_head, test_list._node_at(0))
         self.assertIs(test_list._last_head, test_list._node_at(0))
 
     def test_group_pop_node(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6]])
         self.assertIs(test_list._first_head, test_list._node_at(0))
         self.assertIs(test_list._last_head, test_list._node_at(3))
         test_list.pop(0)
         self.assertEqual(test_list.to_nested_lists(), [[8, 4], [1, 9, 6]])
         self.assertIs(test_list._first_head, test_list._node_at(0))
         self.assertIs(test_list._last_head, test_list._node_at(2))
 
     def test_group_item_modify(self):
-        test_list = GroupedList([[2, 8, 4], [1, 9, 6], [3, 7, 5]])
+        test_list = GroupedList()
+        test_list.append_group([2, 8, 4])
+        test_list.append_group([1, 9, 6])
+        test_list.append_group([3, 7, 5])
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 6], [3, 7, 5]])
         test_list.groups[1][2] = 20
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9, 20], [3, 7, 5]])
 
         del test_list.groups[1][2]
         self.assertEqual(test_list.to_nested_lists(), [[2, 8, 4], [1, 9], [3, 7, 5]])
 
     def test_group_equals(self):
-        list_1 = GroupedList([[1, 2, 3], [4, 5, 6], [7, 8], [9, 10]])
-        list_2 = GroupedList([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]])
+        list_1 = GroupedList()
+        list_1.append_group([1, 2, 3])
+        list_1.append_group([4, 5, 6])
+        list_1.append_group([7, 8])
+        list_1.append_group([9, 10])
+        list_2 = GroupedList()
+        list_2.append_group([1, 2, 3])
+        list_2.append_group([4, 5, 6])
+        list_2.append_group([7, 8, 9])
+        list_2.append_group([10])
         self.assertFalse(list_1.equals(list_2, compare_groups=True))
         self.assertTrue(list_1.equals(list_2, compare_groups=False))
         self.assertTrue(list_1.equals([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], compare_groups=False))
 
         list_3 = GroupedList([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
         list_4 = GroupedList([1, 2, 3, 4, 5, 6, 7, 8, 9, 11])
         self.assertFalse(list_3 == list_4)
-
-    def test_group_insert_at_index(self):
-        test_list = GroupedList([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-        test_list.insert_group_at(3)
-        test_list.insert_group_at(7)
-        self.assertEquals(test_list, GroupedList([[1, 2, 3], [4, 5, 6, 7], [8, 9, 10]]))
-
-    def test_clear(self):
-        list_1 = GroupedList([[1, 2, 3], [4, 5, 6], [7, 8], [9, 10]])
-        list_1.clear()
-        self.assertTrue(list_1.equals(GroupedList()))
-
-    def test_clear_groups(self):
-        list_1 = GroupedList([[1, 2, 3], [4, 5, 6], [7, 8], [9, 10]])
-        list_1.clear_groups()
-        self.assertTrue(list_1.equals(GroupedList([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]), compare_groups=True))
-
+    
     def test_basic_sort(self):
         values = [10, 1, 9, 2, 8, 3, 7, 4, 6, 5]
         test_list = GroupedList(values)
         test_list.sort()
         self.assertEqual(test_list, GroupedList(sorted(values)))
         self.assertEqual(test_list._first.value, 1)
         self.assertEqual(test_list._last.value, 10)
         self.assertTrue(self.verify_is_single_group(test_list))
 
     def test_sort_of_groups(self):
-        test_list = GroupedList([[12, 3, 20], [18, 5, 11], [1, 8], [15], [2, 6, 14]])
+        test_list = GroupedList()
+        test_list.append_group([12, 3, 20])
+        test_list.append_group([18, 5, 11])
+        test_list.append_group([1, 8])
+        test_list.append_group([15])
+        test_list.append_group([2, 6, 14])
         test_list.sort()
         self.assertEqual(test_list, GroupedList([1, 2, 3, 5, 6, 8, 11, 12, 14, 15, 18, 20]))
         self.assertEqual(test_list._first.value, 1)
         self.assertEqual(test_list._last.value, 20)
         self.assertTrue(self.verify_is_single_group(test_list))
 
     def verify_is_single_group(self, linked_list: GroupedList):
```

