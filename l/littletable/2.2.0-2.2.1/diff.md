# Comparing `tmp/littletable-2.2.0.tar.gz` & `tmp/littletable-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littletable-2.2.0.tar", last modified: Sun Apr 30 13:19:15 2023, max compression
+gzip compressed data, was "littletable-2.2.1.tar", last modified: Sun May 28 19:09:44 2023, max compression
```

## Comparing `littletable-2.2.0.tar` & `littletable-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-30 13:19:15.010700 littletable-2.2.0/
--rw-rw-r--   0 paul      (1000) paul      (1000)    35549 2023-04-30 13:18:52.000000 littletable-2.2.0/CHANGES
--rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.0/HowToUseLittletable.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.0/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.0/MANIFEST.in
--rw-rw-r--   0 paul      (1000) paul      (1000)     7490 2023-04-30 13:19:15.010700 littletable-2.2.0/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.0/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-30 13:19:15.010700 littletable-2.2.0/littletable.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7490 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-04-30 13:19:14.000000 littletable-2.2.0/littletable.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)   160733 2023-04-30 06:48:17.000000 littletable-2.2.0/littletable.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-04-30 13:19:15.014700 littletable-2.2.0/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.0/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)   105877 2023-04-30 07:01:19.000000 littletable-2.2.0/unit_tests.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:09:44.856880 littletable-2.2.1/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    36556 2023-05-28 19:07:07.000000 littletable-2.2.1/CHANGES
+-rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.1/HowToUseLittletable.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.1/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.1/MANIFEST.in
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:09:44.856880 littletable-2.2.1/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.1/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:09:44.856880 littletable-2.2.1/littletable.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)   163325 2023-05-28 19:07:07.000000 littletable-2.2.1/littletable.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-05-28 19:09:44.856880 littletable-2.2.1/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.1/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)   110775 2023-05-28 19:07:07.000000 littletable-2.2.1/unit_tests.py
```

### Comparing `littletable-2.2.0/CHANGES` & `littletable-2.2.1/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,45 @@
 NOTE: Deprecated features will be removed in the 3.0 release of littletable:
 - DataObject class, replace with typing.SimpleNamespace, dict, namedtuple, or
   other user-defined class
 - Table.re_match(patt) comparator is deprecated, replace with
   re.compile(patt).match
 
 
+Version 2.2.1
+-------------
+- Rewrote handling of multiple custom `JSONEncoder`s to use multiple
+  inheritance instead of explicit call chaining.
+
+- 20-30% performance speedup when creating a search index.
+
+- Better detection of English plurals when building search indexes. Searching
+  will also detect `Error`, `Exception`, and `Warning` word endings, which are
+  common in code documentation.
+
+- Added module-level convenience methods for building `Table`s and importing from
+  CSV, TSV, JSON, or Excel files, so that in place of:
+
+      import littletable as lt
+      tbl = lt.Table()
+      tbl.csv_import(csv_data_file)
+
+  You can just write:
+
+      import littletable as lt
+      tbl = lt.csv_import(csv_data_file)
+
+- Updated examples to new search return type, and new module-level `csv_import()`.
+  Also added new example `csv_import_examples.py` showing multiple snippets of
+  importing CSV data.
+
+- Tables now keep track of timestamps when they were created, last modified, and
+  last imported.
+
+
 Version 2.2.0
 -------------
 - BREAKING CHANGES:
 
     - Support for Python versions <3.9 is dropped in this version. To run on
       these older Python's, use `littletable` 2.1.2.
```

### Comparing `littletable-2.2.0/LICENSE` & `littletable-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `littletable-2.2.0/PKG-INFO` & `littletable-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
-Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
+Download-URL: https://pypi.org/project/littletable/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -206,7 +207,9 @@
 # print output as an HTML table
 print(wishlists().sort("unitprice desc")("Wishlists").as_html())
 
 # print output as a Markdown table
 print(wishlists().sort("unitprice desc")("Wishlists").as_markdown())
 
 ```
+
+
```

### Comparing `littletable-2.2.0/README.md` & `littletable-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `littletable-2.2.0/littletable.egg-info/PKG-INFO` & `littletable-2.2.1/littletable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
-Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
+Download-URL: https://pypi.org/project/littletable/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -206,7 +207,9 @@
 # print output as an HTML table
 print(wishlists().sort("unitprice desc")("Wishlists").as_html())
 
 # print output as a Markdown table
 print(wishlists().sort("unitprice desc")("Wishlists").as_markdown())
 
 ```
+
+
```

### Comparing `littletable-2.2.0/littletable.py` & `littletable-2.2.1/littletable.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,19 @@
     for item in wishlists().sort("unitprice desc"):
         print(item)
 """
 
 import copy
 import csv
 import datetime
+import functools
 import io
 import itertools
 import textwrap
+import typing
 import warnings
 from enum import Enum
 from io import StringIO
 import json
 import operator
 import os
 import random
@@ -151,69 +153,104 @@
     import rich
     from rich import box
 except ImportError:
     rich = None
     box = None
 
 version_info = namedtuple("version_info", "major minor micro release_level serial")
-__version_info__ = version_info(2, 2, 0, "final", 0)
+__version_info__ = version_info(2, 2, 1, "final", 0)
 __version__ = (
     "{}.{}.{}".format(*__version_info__[:3])
     + (f"{__version_info__.release_level[0]}{__version_info__.serial}", "")[
         __version_info__.release_level == "final"
     ]
 )
-__version_time__ = "30 Apr 2023 06:40 UTC"
+__version_time__ = "28 May 2023 18:46 UTC"
 __author__ = "Paul McGuire <ptmcg@austin.rr.com>"
 
+
+# custom Exception classes
+class SearchIndexInconsistentError(Exception):
+    """
+    Exception raised when using search method on table that has been
+    modified since the search index was built.
+    """
+
+
+class NoSuchIndexError(KeyError):
+    """
+    Exception raised when trying to access an index that does not exist.
+    """
+    def __init__(self, attrname):
+        super().__init__(attrname)
+
+    def __str__(self):
+        index_name = super().__str__()
+        return f"no such index {index_name!r}"
+
+
+class UnableToExtractAttributeNamesError(ValueError):
+    """
+    Exception raised when attributes cannot be determined from an object.
+    """
+
+
+class ReadonlyIndexAccessError(Exception):
+    """
+    Exception raised when trying to write to a readonly index.
+    """
+
+
 NL = os.linesep
 
 default_row_class = SimpleNamespace
 
-_numeric_type: tuple = (int, float)
-right_justify_types = (int, float, datetime.timedelta)
+_numeric_type: tuple[type, ...] = (int, float)
+right_justify_types: tuple[type, ...] = (int, float, datetime.timedelta)
 
 try:
     import numpy
 except ImportError:
-    pass
+    numpy = None
 else:
     _numeric_type += (numpy.number,)
 
 try:
     import openpyxl
 except ImportError:
     openpyxl = None
 
 PredicateFunction = Callable[[Any], bool]
 
 __all__ = [
-    "__author__",
-    "__version__",
-    "__version_info__",
-    "__version_time__",
     "DataObject",
     "FixedWidthReader",
     "Table",
+    "csv_import",
+    "tsv_import",
+    "json_import",
+    "excel_import",
 ]
 
 # define default stopwords for full_text_search
-_stopwords = set(
-    """\
-a about above after again against all am an and any are aren't as at be because been 
-before being below between both but by can't cannot could couldn't did didn't do does 
-doesn't doing don't down during each few for from further had hadn't has hasn't have 
-haven't having he he'd he'll he's her here here's hers herself him himself his how how's i i'd 
-i'll i'm i've if in into is isn't it it's its itself let's me more most mustn't my myself no nor not 
-of off on once only or other ought our ours ourselves out over own same shan't she she'd 
-she'll she's should shouldn't so some such than that that's the their theirs them themselves 
-then there there's these they they'd they'll they're they've this those through to too under 
-until up very was wasn't we we'd we'll we're we've were weren't what what's when when's 
-where where's which while who who's whom why why's with won't would wouldn't you 
-you'd you'll you're you've your yours yourself yourselves""".split()
+_stopwords = frozenset(
+    (*"""\
+     a about above after again against all am an and any are aren't as at be because been 
+     before being below between both but by can't cannot could couldn't did didn't do does 
+     doesn't doing don't down during each few for from further had hadn't has hasn't have haven't 
+     having he he'd he'll he's her here here's hers herself him himself his how how's i i'd i'll
+     i'm i've if in into is isn't it it's its itself let's me more most mustn't my myself no nor
+     not of off on once only or other ought our ours ourselves out over own same shan't she she'd 
+     she'll she's should shouldn't so some such than that that's the their theirs them themselves 
+     then there there's these they they'd they'll they're they've this those through to too under 
+     until up very was wasn't we we'd we'll we're we've were weren't what what's when when's 
+     where where's which while who who's whom why why's with won't would wouldn't you 
+     you'd you'll you're you've your yours yourself yourselves""".split(),
+     *"d ll m re s t ve".split(), "",
+     )
 )
 
 # irregular plurals and singulars for text search handling
 _common_english_irregular_plurals = {
     'addenda': 'addendum', 'addendums': 'addendum', 'alumnae': 'alumna', 'alumni': 'alumnus', 'analyses': 'analysis',
     'antennae': 'antenna', 'antennas': 'antenna', 'antitheses': 'antithesis',
     'appendices': 'appendix', 'appendixes': 'appendix', 'bacilli': 'bacillus', 'bacteria': 'bacterium',
@@ -239,16 +276,19 @@
     'kudos', 'species'
 ]
 _plurals_map = {
     **_common_english_irregular_plurals,
     **{s: s for s in _singulars_that_look_like_plurals}
 }
 
-class UnableToExtractAttributeNamesError(ValueError):
-    """Exception raised when attributes cannot be determined from an object."""
+_significant_word_endings = (
+    'error',
+    'warning',
+    'exception',
+)
 
 
 def _object_attrnames(obj):
     if hasattr(obj, "trait_names"):
         return obj.trait_names()
     if hasattr(obj, "__dict__"):
         # normal object
@@ -281,22 +321,14 @@
     raise UnableToExtractAttributeNamesError("object with unknown attributes")
 
 
 def _to_json(obj, enc_cls):
     return json.dumps(_to_dict(obj), cls=enc_cls)
 
 
-# special Exceptions
-class SearchIndexInconsistentError(Exception):
-    """
-    Exception raised when using search method on table that has been
-    modified since the search index was built.
-    """
-
-
 class DataObject:
     """
     A generic semi-mutable object for storing data values in a table. Attributes
     can be set by passing in named arguments in the constructor, or by setting them
     as C{object.attribute = value}. New attributes can be added any time, but updates
     are ignored.  Table joins are returned as a Table of DataObjects.
     """
@@ -509,17 +541,14 @@
         else:
             ret = self._table_template.copy_template()
             if k in self._index:
                 ret.insert_many(self._index[k])
             return ret
 
 
-class ReadonlyIndexAccessError(Exception): pass
-
-
 class _ReadonlyObjIndexWrapper(_ObjIndexWrapper):
     def __setitem__(self, k, value):
         raise ReadonlyIndexAccessError(f"no update access to index {self.attr!r}")
 
 
 class _TableAttributeValueLister:
     class UniquableIterator:
@@ -698,15 +727,15 @@
 
         self._iterobj: Iterable[str]
 
         if isinstance(seqobj, str):
             if "\n" in seqobj:
                 self._iterobj = iter(StringIO(seqobj))
                 self.type = ImportSourceType.string
-            elif seqobj.startswith("http"):
+            elif seqobj.startswith(("http://", "https://")):
                 self._iterobj = _decoder(urllib.request.urlopen(seqobj))
                 self.type = ImportSourceType.url
             else:
                 if seqobj.endswith(".gz"):
                     import gzip
 
                     self._iterobj = _decoder(gzip.GzipFile(filename=seqobj))
@@ -1096,14 +1125,18 @@
         self._indexes: dict[str, _ObjIndex] = {}
         self._uniqueIndexes: list[_UniqueObjIndex] = []
         self._search_indexes: dict[str, dict[str, list]] = {}
 
         self.import_source_type: Optional[ImportSourceType] = None
         self.import_source: Optional[str] = None
 
+        self.import_time = None
+        self.create_time = datetime.datetime.now().astimezone(datetime.UTC)
+        self.modify_time = self.create_time
+
         """
         C{'by'} is added as a pseudo-attribute on tables, to provide
         dict-like access to the underlying records in the table by index key, as in::
 
             employees.by.socsecnum["000-00-0000"]
             customers.by.zipcode["12345"]
 
@@ -1357,19 +1390,30 @@
         return self
 
     def get_index(self, attr: str):
         return _ReadonlyObjIndexWrapper(self._indexes[attr], self.copy_template())
 
     NON_WORD_STRIPPER_RE = re.compile(r"[^\w_]?([\w._-]*)[^\w.]*")
     NON_WORD_STRIPPER2_RE = re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)(!>_-)$")
+    ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
+    SIGNIFICANT_WORD_ENDING_RE = re.compile(rf".*({'|'.join(_significant_word_endings)})$")
+
     PLURAL_ENDING_IN_IES = re.compile(r"(.*[^aeiouy])ies$")
     PLURAL_ENDING_IN_ES = re.compile(r"(.*(?:ch|ss|sh|x))es$")
+    PLURAL_ENDING_IN_ES2 = re.compile(r"(.*(?:[bcdfghklmnprstuvwxz]|(qu))e)s$")
     PLURAL_ENDING_IN_S = re.compile(r"(.*[^aeious])s$")
     SINGULAR_ENDING_IN_S = re.compile(r"(.*(?:ness|ics))$")
-    ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
+
+    PLURAL_MATCH_SUBS = (
+        (PLURAL_ENDING_IN_IES, r"\1y"),
+        (PLURAL_ENDING_IN_ES, r"\1"),
+        (PLURAL_ENDING_IN_ES2, r"\1"),
+        (SINGULAR_ENDING_IN_S, r"\1"),
+        (PLURAL_ENDING_IN_S, r"\1"),
+    )
 
     @staticmethod
     def _normalize_word(s: str) -> str:
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
             re.compile(r"((?:\w\.){2,})"),
             # words that may be hyphenated or snake-case
@@ -1379,39 +1423,46 @@
         for match_re in match_res:
             if match := match_re.match(s):
                 ret = match.group(1).lower().replace(".", "")
                 return ret
         return ""
 
     @staticmethod
-    def _normalize_word_gen(s: str) -> Iterable[str]:
+    def _normalize_word_gen(s: str, sw: frozenset) -> Iterable[str]:
+        s = s.lower()
+        if s in sw:
+            return
+
         # strip non-word chars from front and back
         stripper = Table.NON_WORD_STRIPPER_RE
         s = stripper.match(s).group(1)
 
+        if s in sw:
+            return
+
         # catch plurals
-        if s.isalpha():
-            s = s.lower()
+        if (sa := s.rstrip(",.!?;:'\"-")).isalpha():
+            s = sa
+            if s in sw:
+                return
 
             # check common plurals - if not found, check common plural patterns
             if not (sing := _plurals_map.get(s)):
-
-                match_subs = (
-                    (Table.PLURAL_ENDING_IN_IES, r"\1y"),
-                    (Table.PLURAL_ENDING_IN_ES, r"\1"),
-                    (Table.SINGULAR_ENDING_IN_S, r"\1"),
-                    (Table.PLURAL_ENDING_IN_S, r"\1"),
-                )
-                sing = next((sub_match[0] for re_sub, re_repl in match_subs
+                sing = next((sub_match[0] for re_sub, re_repl in Table.PLURAL_MATCH_SUBS
                             if (sub_match := re_sub.subn(re_repl, s))[1]),
                             s)
 
             if sing and sing != s:
                 yield sing
             yield s
+
+            # # also add special ending words for code and documentation parsing
+            if s.endswith(_significant_word_endings):
+                yield Table.SIGNIFICANT_WORD_ENDING_RE.match(s)[1]
+
             return
 
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
             Table.ACRONYM_WITH_PERIODS,
             # words that may be hyphenated or snake-case
             # (strip off any leading single non-word character)
@@ -1425,25 +1476,25 @@
                     if sep in g1:
                         yield from filter(None, g1.split(sep))
                 break
         else:
             for sep in ".-":
                 if sep in s:
                     yield from (
-                        ss.lower() for ss in s.split(sep)
-                        if (ss.islower() or len(ss) > 1)
+                        ss for ss in s.split(sep)
+                        if len(ss) > 1
                     )
                     if sep == "." and all(len(ss) <= 1 for ss in s.split(".")):
-                        yield s.lower().replace(".", "")
-            yield s.lower()
+                        yield s.replace(".", "")
+            yield s
 
     @staticmethod
-    def _normalize_split(s: str) -> Iterable[str]:
+    def _normalize_split(s: str, sw: frozenset=frozenset()) -> Iterable[str]:
         return (
-            filter(None, (ss for wd in s.split() for ss in Table._normalize_word_gen(wd)))
+            ss for wd in s.split() for ss in Table._normalize_word_gen(wd, sw)
         )
 
     def create_search_index(
         self,
         attrname: str,
         stopwords: Optional[Iterable[str]] = None,
         force: bool = False,
@@ -1484,27 +1535,27 @@
         if attrname in self._search_indexes:
             if force or not self._search_indexes[attrname]["VALID"]:
                 # stale search index, rebuild
                 self._search_indexes.pop(attrname)
             else:
                 return self
 
-        stopwords_set: set[str]
+        stopwords_set: frozenset[str]
         if stopwords is None:
             stopwords_set = _stopwords
         else:
-            stopwords_set = set(stopwords)
+            stopwords_set = frozenset(stopwords)
 
         self._search_indexes[attrname] = defaultdict(list)
         new_index: dict[str, Any] = self._search_indexes[attrname]
         for i, rec in enumerate(self.obs):
             if not (attrvalue := getattr(rec, attrname, "")):
                 continue
-            words = self._normalize_split(attrvalue)
-            for wd in set(words) - stopwords_set:
+            words = self._normalize_split(attrvalue.lower(), stopwords_set)
+            for wd in set(words):
                 new_index[wd].append(i)
 
         # use uppercase keys for index metadata, since they should not
         # overlap with any search terms
         new_index["STOPWORDS"] = stopwords_set
         new_index["VALID"] = True
 
@@ -1519,74 +1570,58 @@
         search_index = self._search_indexes[attrname]
         if not search_index["VALID"]:
             msg = (
                 f"table has been modified since the search index for {attrname!r} was created,"
                 " rebuild using create_search_index()"
             )
             raise SearchIndexInconsistentError(msg)
-        stopwords = search_index["STOPWORDS"]
+        stopwords = typing.cast(frozenset[str], search_index["STOPWORDS"])
 
         plus_matches: dict[str, set[int]] = {}
         minus_matches: dict[str, list[int]] = {}
         opt_matches: dict[str, list[int]] = {}
         reqd_matches: set[int] = set()
         excl_matches: set[int] = set()
         reqd_words: dict[tuple[str], dict[str, set[int]]] = {}
 
         if isinstance(query, str):
             query = shlex.split(query.strip())
 
         for keyword in query:
             keyword = keyword.lower()
             if keyword.startswith("++"):
-                kwds = tuple(self._normalize_word_gen(keyword[2:]))
+                kwds = tuple(self._normalize_word_gen(keyword[2:], stopwords))
                 reqd_words[kwds] = {}
                 for kwd in kwds:
-                    # kwd = self._normalize_word(keyword[2:])
-                    if kwd in stopwords:
-                        continue
-
                     matched_entries = set(search_index.get(kwd, []))
                     reqd_words[kwds][kwd] = matched_entries
                     if not matched_entries:
                         continue
 
                     if kwd not in plus_matches:
                         plus_matches[kwd] = matched_entries
 
             elif keyword.startswith("--"):
-                # kwd = self._normalize_word(keyword[2:])
-                for kwd in self._normalize_word_gen(keyword[2:]):
-                    if kwd in stopwords:
-                        continue
+                for kwd in self._normalize_word_gen(keyword[2:], stopwords):
                     excl_matches |= set(search_index.get(kwd, []))
 
             elif keyword.startswith("+"):
-                # kwd = self._normalize_word(keyword[1:])
-                for kwd in self._normalize_word_gen(keyword[1:]):
-                    if kwd in stopwords:
-                        continue
+                for kwd in self._normalize_word_gen(keyword[1:], stopwords):
                     minus_matches.pop(kwd, None)
                     if kwd not in plus_matches and kwd not in reqd_matches:
                         plus_matches[kwd] = set(search_index.get(kwd, []))
 
             elif keyword.startswith("-"):
-                # kwd = self._normalize_word(keyword[1:])
-                for kwd in self._normalize_word_gen(keyword[1:]):
-                    if kwd in stopwords:
-                        continue
+                for kwd in self._normalize_word_gen(keyword[1:], stopwords):
                     plus_matches.pop(kwd, None)
                     if kwd not in minus_matches and kwd not in excl_matches:
                         minus_matches[kwd] = set(search_index.get(kwd, []))
 
             else:
-                # kwd = self._normalize_word(keyword)
-                for kwd in self._normalize_word_gen(keyword):
-                    if kwd in stopwords:
-                        continue
+                for kwd in self._normalize_word_gen(keyword, stopwords):
                     if kwd in plus_matches or kwd in minus_matches:
                         continue
                     opt_matches[kwd] = set(search_index.get(kwd, []))
 
         # process word groups to determine correct set of reqd_matches
         if reqd_words:
             reqd_matches = set(range(len(self.obs)))
@@ -1643,19 +1678,38 @@
                         setattr(rec, words_attr, tup[2])
             except AttributeError:
                 # not all record content types will accept new attributes
                 pass
 
         return ret
 
-    def delete_search_index(self, attrname: str):
+    def delete_search_index(self, attrname: str) -> "Table":
         """
         Deletes a previously-created search index on a particular attribute.
         """
         self._search_indexes.pop(attrname, None)
+        return self
+
+    def rebuild_search_index(self, attrname: str, force=True) -> "Table":
+        """
+        Rebuilds an existing search index if it has been invalidated, or if force=True.
+        """
+        try:
+            existing_search_index = self._search_indexes[attrname]
+        except KeyError:
+            raise NoSuchIndexError(attrname)
+
+        if not existing_search_index['VALID'] or force:
+            self.create_search_index(
+                attrname,
+                stopwords=existing_search_index["STOPWORDS"],
+                force=True,
+            )
+
+        return self
 
     def insert(self, obj: Any) -> "Table":
         """
         Insert a new object into this Table.
         @param obj: any Python object -
         Objects can be constructed using any Python object; C{littletable}
         introspects the object's C{__dict__}, C{__slots__}, or C{_fields} attributes
@@ -1783,20 +1837,23 @@
         del self.obs[:]
         for idx in self._indexes.values():
             idx._clear()
 
         self._search_indexes.clear()
         return self
 
-    def _contents_changed(self):
+    def _contents_changed(self, *, invalidate_search_indexes=True):
         """
         Internal method to be called whenever the contents of a table are modified.
         """
-        for idx in self._search_indexes.values():
-            idx["VALID"] = False
+        if invalidate_search_indexes:
+            for idx in self._search_indexes.values():
+                idx["VALID"] = False
+
+        self.modify_time = datetime.datetime.now().astimezone(datetime.UTC)
 
     def _query_attr_sort_fn(self, attr_val: tuple[str, Any]) -> int:
         """Used to order where keys by most selective key first"""
         attr, v = attr_val
         if attr in self._indexes:
             idx = self._indexes[attr]
             if v in idx:
@@ -2510,14 +2567,16 @@
                                            ):
                 # if url, strip off query args if any
                 if self.import_source_type is ImportSourceType.url:
                     source = str(source).partition("?")[0]
                 self.import_source = str(source)
                 self(str(source))
 
+        self.import_time = datetime.datetime.now().astimezone(datetime.UTC)
+        self._contents_changed()
         return self
 
     def csv_import(
         self,
         csv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
         transforms: dict = None,
@@ -2841,41 +2900,58 @@
         @type streaming: bool
         @param path: (only valid if streaming=False) a '.'-delimited path into the inbound JSON, in case
             the objects to import are not in a top-level JSON list
         @type path: str
         @param json_decoder: subclass of json.JSONDecoder to pass through to json.loads (default=None)
         @type json_decoder: json.JSONDecoder
         """
+        class PathNotFoundError(KeyError):
+            def __init__(self, key, path):
+                super().__init__(key)
+                self.key = key
+                self.path = path
+
+            def __str__(self):
+                return f"could not find {self.key!r} element of path {self.path!r} in imported JSON"
 
         class _JsonFileReader:
             def __init__(self, src):
                 self.source = src
                 self.streaming = streaming
 
             def __iter__(self):
                 if self.streaming:
+                    # incrementally read lines from source until a valid JSON object
+                    # can be parsed
                     current = ""
                     for line in self.source:
                         if current:
                             current += " "
                         current += line
                         try:
                             yield json.loads(current, cls=json_decoder)
                             current = ""
                         except Exception:
                             pass
                 else:
+                    # merge entire source into one JSON parseable object
                     inbound_json = '\n'.join(self.source)
                     obs = json.loads(inbound_json, cls=json_decoder)
+
+                    # descend into parsed JSON object by path
                     for path_item in filter(None, path.split(".")):
                         obs = obs.get(path_item)
                         if obs is None:
-                            raise KeyError(path_item)
+                            raise PathNotFoundError(path_item, path)
+
                     yield from obs
 
+        if path and streaming:
+            raise ValueError("cannot specify path and streaming=True")
+
         if row_class is None:
             row_class = default_row_class
         return self._import(
             source,
             encoding,
             transforms=transforms,
             reader=_JsonFileReader,
@@ -2910,32 +2986,22 @@
         @param json_encoder: an encoder or tuple of encoders to perform custom
             JSON encoding for fields in table objects
         @type json_encoder: json.JSONEncoder or tuple(json.JSONEncoder)
         """
         close_on_exit = False
         return_dest_value = False
 
-        class JsonEncoderChain(json.JSONEncoder):
-            def __init__(self, encoders, *args, **kwargs):
-                super().__init__(*args, **kwargs)
-                self.encoders = encoders
-
-            def default(self, oo):
-                self_vars = {**vars(self)}
-                self_vars.pop('encoders')
-                for enc in self.encoders:
-                    try:
-                        return enc(**self_vars).default(oo)
-                    except TypeError:
-                        pass
-                return super().default(oo)
-
         if json_encoder:
             if isinstance(json_encoder, tuple):
-                json_encoder = partial(JsonEncoderChain, encoders=json_encoder)
+                # use multiple inheritance to chain encoders
+                json_encoder = type(
+                    "compound_JSON_encoder",
+                    (*json_encoder, json.JSONEncoder),
+                    {}
+                )
 
         if dest is None:
             dest = io.StringIO()
             return_dest_value = True
         if isinstance(dest, Path):
             dest = str(Path)
         if isinstance(dest, str):
@@ -3059,14 +3125,16 @@
                     rec_.__dict__[attrname] = val
                 else:
                     setattr(rec_, attrname, val)
         except AttributeError:
             raise AttributeError(
                 f"cannot add/modify attribute {attrname!r} in table records"
             )
+
+        self._contents_changed(invalidate_search_indexes=False)
         return self
 
     def groupby(self, keyexpr, **outexprs):
         """
         simple prototype of group by, with support for expressions in the group-by clause
         and outputs
         @param keyexpr: grouping field and optional expression for computing the key value;
@@ -3164,14 +3232,17 @@
             "len": len(self),
             "name": self.table_name,
             "fields": self._attr_names(),
             "indexes": [
                 (idx_name, self._indexes[idx_name] in unique_indexes)
                 for idx_name in self._indexes
             ],
+            "created": self.create_time,
+            "modified": self.modify_time,
+            "last_import": self.import_time,
         }
 
     def head(self, n: int = 10) -> "Table":
         """
         Return a table of the first 'n' records in a table.
         :param n: (int, default=10) number of records to return
         :return: Table
@@ -3296,15 +3367,14 @@
         return field_names
 
     def _rich_table(self, fields=None, empty="", groupby=None, **kwargs):
         if rich is None:
             raise Exception("rich module not installed")
 
         from rich.table import Table as RichTable
-        from rich.markup import escape as rich_escape
 
         if fields is None:
             fields = self.info()["fields"]
 
         attr_names = []
         field_settings = []
 
@@ -3334,18 +3404,18 @@
             attr_names.append(name)
             header = field_spec.pop("header", None)
             if header is None:
                 header = name.replace("_", " ").title() if name.islower() else name
             field_settings.append((header, field_spec))
 
         grouping = False
-        group_attrs = ()
+        group_attrs = []
         if groupby is not None:
-            group_attrs = tuple(g for g in self._parse_fields_string(groupby)
-                                if g in attr_names)
+            group_attrs = [g for g in self._parse_fields_string(groupby)
+                           if g in attr_names]
             if group_attrs:
                 grouping = True
 
         table_defaults = dict(show_header=True, header_style="bold", box=box.ASCII)
         if getattr(sys.stdout, "isatty", lambda: False)():
             table_defaults["box"] = box.SIMPLE
         if self.table_name:
@@ -3450,18 +3520,18 @@
                 else:
                     str_v = ""
                 ret_tr.append(f'<td><div align="{align}">{str_v}</div></td>')
             ret_tr.append("</tr>\n")
             return "".join(ret_tr)
 
         grouping = False
-        group_attrs = ()
+        group_attrs = []
         if groupby is not None:
-            group_attrs = tuple(g for g in self._parse_fields_string(groupby)
-                                if g in attr_names)
+            group_attrs = [g for g in self._parse_fields_string(groupby)
+                           if g in attr_names]
             if group_attrs:
                 grouping = True
 
         if table_properties is not None:
             table_modifiers = "".join(f' {k}="{v}"' for k, v in table_properties.items())
         else:
             table_modifiers = ""
@@ -3516,18 +3586,18 @@
         fields = self._parse_fields_string(fields)
         if formats is None:
             formats = {}
         field_format_map = {}
         attr_names = fields
 
         grouping = False
-        group_attrs = ()
+        group_attrs = []
         if groupby is not None:
-            group_attrs = tuple(g for g in self._parse_fields_string(groupby)
-                                if g in attr_names)
+            group_attrs = [g for g in self._parse_fields_string(groupby)
+                           if g in attr_names]
             if group_attrs:
                 grouping = True
 
         center_vals = (True, False, 'Y', 'N', 'X', 'YES', 'NO', 'y', 'n', 'x', 'yes', 'no', 0, 1, None)
         field_align_map = {}
         for f in fields:
             align = "---"
@@ -3585,14 +3655,32 @@
 
         return ret
 
 
 Sequence.register(Table)
 
 
+# module-level convenience functions for Table.*_import() instance methods
+def _make_module_level_import_fn(name):
+    table_method = getattr(Table, name)
+
+    @functools.wraps(table_method)
+    def import_fn(*args, **kwargs):
+        ret = Table()
+        return table_method(ret, *args, **kwargs)
+
+    return import_fn
+
+
+csv_import = _make_module_level_import_fn("csv_import")
+tsv_import = _make_module_level_import_fn("tsv_import")
+json_import = _make_module_level_import_fn("json_import")
+excel_import = _make_module_level_import_fn("excel_import")
+
+
 class _PivotTable(Table):
     """Enhanced Table containing pivot results from calling table.pivot()."""
 
     def __init__(self, parent, attr_val_path, attrlist):
         """PivotTable initializer - do not create these directly, use
         L{Table.pivot}.
         """
```

### Comparing `littletable-2.2.0/setup.py` & `littletable-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `littletable-2.2.0/unit_tests.py` & `littletable-2.2.1/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,6618 +1,6924 @@
 00000000: 230a 2320 756e 6974 5f74 6573 7473 2e70  #.# unit_tests.p
 00000010: 790a 230a 2320 756e 6974 2074 6573 7473  y.#.# unit tests
 00000020: 2066 6f72 206c 6974 746c 6574 6162 6c65   for littletable
 00000030: 206c 6962 7261 7279 0a23 0a69 6d70 6f72   library.#.impor
-00000040: 7420 6173 740a 6672 6f6d 2063 6f6c 6c65  t ast.from colle
-00000050: 6374 696f 6e73 2069 6d70 6f72 7420 6e61  ctions import na
-00000060: 6d65 6474 7570 6c65 0a69 6d70 6f72 7420  medtuple.import 
-00000070: 636f 7079 0a69 6d70 6f72 7420 696f 0a69  copy.import io.i
-00000080: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
-00000090: 696d 706f 7274 206a 736f 6e0a 6672 6f6d  import json.from
-000000a0: 206f 7065 7261 746f 7220 696d 706f 7274   operator import
-000000b0: 2061 7474 7267 6574 7465 720a 696d 706f   attrgetter.impo
-000000c0: 7274 206f 730a 696d 706f 7274 2073 7973  rt os.import sys
-000000d0: 0a69 6d70 6f72 7420 7465 7874 7772 6170  .import textwrap
-000000e0: 0a66 726f 6d20 7479 7065 7320 696d 706f  .from types impo
-000000f0: 7274 2053 696d 706c 654e 616d 6573 7061  rt SimpleNamespa
-00000100: 6365 0a69 6d70 6f72 7420 756e 6974 7465  ce.import unitte
-00000110: 7374 0a66 726f 6d20 7479 7069 6e67 2069  st.from typing i
-00000120: 6d70 6f72 7420 4f70 7469 6f6e 616c 2c20  mport Optional, 
-00000130: 556e 696f 6e2c 204e 616d 6564 5475 706c  Union, NamedTupl
-00000140: 650a 0a70 7974 686f 6e5f 7665 7273 696f  e..python_versio
-00000150: 6e20 3d20 7379 732e 7665 7273 696f 6e5f  n = sys.version_
-00000160: 696e 666f 5b3a 325d 0a0a 696d 706f 7274  info[:2]..import
-00000170: 206c 6974 746c 6574 6162 6c65 2061 7320   littletable as 
-00000180: 6c74 0a0a 534b 4950 5f43 5356 5f49 4d50  lt..SKIP_CSV_IMP
-00000190: 4f52 545f 5553 494e 475f 5552 4c5f 5445  ORT_USING_URL_TE
-000001a0: 5354 5320 3d20 6f73 2e65 6e76 6972 6f6e  STS = os.environ
-000001b0: 2e67 6574 2822 534b 4950 5f43 5356 5f49  .get("SKIP_CSV_I
-000001c0: 4d50 4f52 545f 5553 494e 475f 5552 4c5f  MPORT_USING_URL_
-000001d0: 5445 5354 5322 2c20 2230 2229 203d 3d20  TESTS", "0") == 
-000001e0: 2231 220a 0a74 7279 3a0a 2020 2020 696d  "1"..try:.    im
-000001f0: 706f 7274 2064 6174 6163 6c61 7373 6573  port dataclasses
-00000200: 0a65 7863 6570 7420 496d 706f 7274 4572  .except ImportEr
-00000210: 726f 723a 0a20 2020 2070 7269 6e74 2822  ror:.    print("
-00000220: 6461 7461 636c 6173 7365 7320 7465 7374  dataclasses test
-00000230: 7320 6469 7361 626c 6564 2229 0a20 2020  s disabled").   
-00000240: 2023 2070 7265 2050 7933 2e37 2028 6f72   # pre Py3.7 (or
-00000250: 2033 2e36 2077 6974 6820 6261 636b 706f   3.6 with backpo
-00000260: 7274 6564 2064 6174 6163 6c61 7373 6573  rted dataclasses
-00000270: 290a 2020 2020 6461 7461 636c 6173 7365  ).    dataclasse
-00000280: 7320 3d20 4e6f 6e65 0a65 6c73 653a 0a20  s = None.else:. 
-00000290: 2020 2040 6461 7461 636c 6173 7365 732e     @dataclasses.
-000002a0: 6461 7461 636c 6173 730a 2020 2020 636c  dataclass.    cl
-000002b0: 6173 7320 4461 7461 4461 7461 636c 6173  ass DataDataclas
-000002c0: 733a 0a20 2020 2020 2020 2061 3a20 696e  s:.        a: in
-000002d0: 740a 2020 2020 2020 2020 623a 2069 6e74  t.        b: int
-000002e0: 0a20 2020 2020 2020 2063 3a20 696e 740a  .        c: int.
-000002f0: 0a74 7279 3a0a 2020 2020 696d 706f 7274  .try:.    import
-00000300: 2070 7964 616e 7469 630a 6578 6365 7074   pydantic.except
-00000310: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
-00000320: 2020 7072 696e 7428 2270 7964 616e 7469    print("pydanti
-00000330: 6320 7465 7374 7320 6469 7361 626c 6564  c tests disabled
-00000340: 2229 0a20 2020 2070 7964 616e 7469 6320  ").    pydantic 
-00000350: 3d20 4e6f 6e65 0a65 6c73 653a 0a20 2020  = None.else:.   
-00000360: 2063 6c61 7373 2044 6174 6150 7964 616e   class DataPydan
-00000370: 7469 634d 6f64 656c 2870 7964 616e 7469  ticModel(pydanti
-00000380: 632e 4261 7365 4d6f 6465 6c29 3a0a 2020  c.BaseModel):.  
-00000390: 2020 2020 2020 613a 204f 7074 696f 6e61        a: Optiona
-000003a0: 6c5b 556e 696f 6e5b 696e 742c 2073 7472  l[Union[int, str
-000003b0: 5d5d 0a20 2020 2020 2020 2062 3a20 4f70  ]].        b: Op
-000003c0: 7469 6f6e 616c 5b55 6e69 6f6e 5b69 6e74  tional[Union[int
-000003d0: 2c20 7374 725d 5d0a 2020 2020 2020 2020  , str]].        
-000003e0: 633a 204f 7074 696f 6e61 6c5b 556e 696f  c: Optional[Unio
-000003f0: 6e5b 696e 742c 2073 7472 5d5d 0a0a 2020  n[int, str]]..  
-00000400: 2020 636c 6173 7320 4461 7461 5079 6461    class DataPyda
-00000410: 6e74 6963 496d 6d75 7461 626c 654d 6f64  nticImmutableMod
-00000420: 656c 2870 7964 616e 7469 632e 4261 7365  el(pydantic.Base
-00000430: 4d6f 6465 6c29 3a0a 2020 2020 2020 2020  Model):.        
-00000440: 636c 6173 7320 436f 6e66 6967 3a0a 2020  class Config:.  
-00000450: 2020 2020 2020 2020 2020 616c 6c6f 775f            allow_
-00000460: 6d75 7461 7469 6f6e 203d 2046 616c 7365  mutation = False
-00000470: 0a0a 2020 2020 2020 2020 613a 204f 7074  ..        a: Opt
-00000480: 696f 6e61 6c5b 556e 696f 6e5b 696e 742c  ional[Union[int,
-00000490: 2073 7472 5d5d 0a20 2020 2020 2020 2062   str]].        b
-000004a0: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-000004b0: 5b69 6e74 2c20 7374 725d 5d0a 2020 2020  [int, str]].    
-000004c0: 2020 2020 633a 204f 7074 696f 6e61 6c5b      c: Optional[
-000004d0: 556e 696f 6e5b 696e 742c 2073 7472 5d5d  Union[int, str]]
-000004e0: 0a0a 2020 2020 636c 6173 7320 4461 7461  ..    class Data
-000004f0: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-00000500: 2870 7964 616e 7469 632e 4261 7365 4d6f  (pydantic.BaseMo
-00000510: 6465 6c29 3a0a 2020 2020 2020 2020 636c  del):.        cl
-00000520: 6173 7320 436f 6e66 6967 3a0a 2020 2020  ass Config:.    
-00000530: 2020 2020 2020 2020 6f72 6d5f 6d6f 6465          orm_mode
-00000540: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
-00000550: 2061 3a20 4f70 7469 6f6e 616c 5b55 6e69   a: Optional[Uni
-00000560: 6f6e 5b69 6e74 2c20 7374 725d 5d0a 2020  on[int, str]].  
-00000570: 2020 2020 2020 623a 204f 7074 696f 6e61        b: Optiona
-00000580: 6c5b 556e 696f 6e5b 696e 742c 2073 7472  l[Union[int, str
-00000590: 5d5d 0a20 2020 2020 2020 2063 3a20 4f70  ]].        c: Op
-000005a0: 7469 6f6e 616c 5b55 6e69 6f6e 5b69 6e74  tional[Union[int
-000005b0: 2c20 7374 725d 5d0a 0a74 7279 3a0a 2020  , str]]..try:.  
-000005c0: 2020 696d 706f 7274 2061 7474 720a 6578    import attr.ex
-000005d0: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
-000005e0: 3a0a 2020 2020 7072 696e 7428 2261 7474  :.    print("att
-000005f0: 7273 2074 6573 7473 2064 6973 6162 6c65  rs tests disable
-00000600: 6422 290a 2020 2020 6174 7472 203d 204e  d").    attr = N
-00000610: 6f6e 650a 656c 7365 3a0a 2020 2020 4174  one.else:.    At
-00000620: 7472 436c 6173 7320 3d20 6174 7472 2e6d  trClass = attr.m
-00000630: 616b 655f 636c 6173 7328 2241 7474 7243  ake_class("AttrC
-00000640: 6c61 7373 222c 205b 2261 222c 2022 6222  lass", ["a", "b"
-00000650: 2c20 2263 225d 290a 0a74 7279 3a0a 2020  , "c"])..try:.  
-00000660: 2020 696d 706f 7274 2074 7261 6974 6c65    import traitle
-00000670: 7473 0a65 7863 6570 7420 496d 706f 7274  ts.except Import
-00000680: 4572 726f 723a 0a20 2020 2070 7269 6e74  Error:.    print
-00000690: 2822 7472 6169 746c 6574 7320 7465 7374  ("traitlets test
-000006a0: 7320 6469 7361 626c 6564 2229 0a20 2020  s disabled").   
-000006b0: 2074 7261 6974 6c65 7473 203d 204e 6f6e   traitlets = Non
-000006c0: 650a 656c 7365 3a0a 2020 2020 636c 6173  e.else:.    clas
-000006d0: 7320 5472 6169 746c 6574 7343 6c61 7373  s TraitletsClass
-000006e0: 286c 742e 4861 7354 7261 6974 734d 6978  (lt.HasTraitsMix
-000006f0: 696e 2c20 7472 6169 746c 6574 732e 4861  in, traitlets.Ha
-00000700: 7354 7261 6974 7329 3a0a 2020 2020 2020  sTraits):.      
-00000710: 2020 6120 3d20 7472 6169 746c 6574 732e    a = traitlets.
-00000720: 556e 696f 6e28 5b74 7261 6974 6c65 7473  Union([traitlets
-00000730: 2e49 6e74 2829 2c20 7472 6169 746c 6574  .Int(), traitlet
-00000740: 732e 556e 6963 6f64 6528 295d 2c20 616c  s.Unicode()], al
-00000750: 6c6f 775f 6e6f 6e65 3d54 7275 6529 0a20  low_none=True). 
-00000760: 2020 2020 2020 2062 203d 2074 7261 6974         b = trait
-00000770: 6c65 7473 2e55 6e69 6f6e 285b 7472 6169  lets.Union([trai
-00000780: 746c 6574 732e 496e 7428 292c 2074 7261  tlets.Int(), tra
-00000790: 6974 6c65 7473 2e55 6e69 636f 6465 2829  itlets.Unicode()
-000007a0: 5d2c 2061 6c6c 6f77 5f6e 6f6e 653d 5472  ], allow_none=Tr
-000007b0: 7565 290a 2020 2020 2020 2020 6320 3d20  ue).        c = 
-000007c0: 7472 6169 746c 6574 732e 556e 696f 6e28  traitlets.Union(
-000007d0: 5b74 7261 6974 6c65 7473 2e49 6e74 2829  [traitlets.Int()
-000007e0: 2c20 7472 6169 746c 6574 732e 556e 6963  , traitlets.Unic
-000007f0: 6f64 6528 295d 2c20 616c 6c6f 775f 6e6f  ode()], allow_no
-00000800: 6e65 3d54 7275 6529 0a0a 2020 2020 2020  ne=True)..      
-00000810: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000820: 656c 662c 202a 2a6b 7761 7267 7329 3a0a  elf, **kwargs):.
-00000830: 2020 2020 2020 2020 2020 2020 7375 7065              supe
-00000840: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
-00000850: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00000860: 2c20 7720 696e 206b 7761 7267 732e 6974  , w in kwargs.it
-00000870: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00000880: 2020 2020 2020 2073 6574 6174 7472 2873         setattr(s
-00000890: 656c 662c 206b 2c20 7729 0a0a 2020 2020  elf, k, w)..    
-000008a0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-000008b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000008c0: 2020 2020 7265 7475 726e 2066 227b 7479      return f"{ty
-000008d0: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
-000008e0: 5f7d 3a28 613d 7b73 656c 662e 617d 2c20  _}:(a={self.a}, 
-000008f0: 623d 7b73 656c 662e 627d 2c20 633d 7b73  b={self.b}, c={s
-00000900: 656c 662e 637d 2922 0a0a 2020 2020 2020  elf.c})"..      
-00000910: 2020 6465 6620 5f5f 6469 725f 5f28 7365    def __dir__(se
-00000920: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
-00000930: 2072 6574 7572 6e20 7365 6c66 2e74 7261   return self.tra
-00000940: 6974 5f6e 616d 6573 2829 0a0a 4461 7461  it_names()..Data
-00000950: 5475 706c 6520 3d20 6e61 6d65 6474 7570  Tuple = namedtup
-00000960: 6c65 2822 4461 7461 5475 706c 6522 2c20  le("DataTuple", 
-00000970: 2261 2062 2063 2229 0a0a 0a63 6c61 7373  "a b c")...class
-00000980: 2044 6174 614e 616d 6564 5475 706c 6528   DataNamedTuple(
-00000990: 4e61 6d65 6454 7570 6c65 293a 0a20 2020  NamedTuple):.   
-000009a0: 2061 3a20 696e 740a 2020 2020 623a 2069   a: int.    b: i
-000009b0: 6e74 0a20 2020 2063 3a20 696e 740a 0a0a  nt.    c: int...
-000009c0: 2320 6966 2072 6963 6820 6973 206e 6f74  # if rich is not
-000009d0: 2069 6e73 7461 6c6c 6564 2c20 6469 7361   installed, disa
-000009e0: 626c 6520 7461 626c 652e 7072 6573 656e  ble table.presen
-000009f0: 7428 2920 6361 6c6c 730a 7472 793a 0a20  t() calls.try:. 
-00000a00: 2020 2069 6d70 6f72 7420 7269 6368 0a65     import rich.e
-00000a10: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-00000a20: 723a 0a20 2020 2072 6963 6820 3d20 4e6f  r:.    rich = No
-00000a30: 6e65 0a20 2020 2023 2064 6973 6162 6c65  ne.    # disable
-00000a40: 2070 7265 7365 6e74 2829 206d 6574 686f   present() metho
-00000a50: 642c 2073 696e 6365 2072 6963 6820 6973  d, since rich is
-00000a60: 206e 6f74 2061 7661 696c 6162 6c65 0a20   not available. 
-00000a70: 2020 206c 742e 5461 626c 652e 7072 6573     lt.Table.pres
-00000a80: 656e 7420 3d20 6c61 6d62 6461 202a 6172  ent = lambda *ar
-00000a90: 6773 2c20 2a2a 6b77 6172 6773 3a20 4e6f  gs, **kwargs: No
-00000aa0: 6e65 0a0a 0a63 6c61 7373 2053 6c6f 7474  ne...class Slott
-00000ab0: 6564 3a0a 2020 2020 5f5f 736c 6f74 735f  ed:.    __slots_
-00000ac0: 5f20 3d20 5b27 6127 2c20 2762 272c 2027  _ = ['a', 'b', '
-00000ad0: 6327 5d0a 0a20 2020 2064 6566 205f 5f69  c']..    def __i
-00000ae0: 6e69 745f 5f28 7365 6c66 2c20 612c 2062  nit__(self, a, b
-00000af0: 2c20 6329 3a0a 2020 2020 2020 2020 7365  , c):.        se
-00000b00: 6c66 2e61 203d 2061 0a20 2020 2020 2020  lf.a = a.       
-00000b10: 2073 656c 662e 6220 3d20 620a 2020 2020   self.b = b.    
-00000b20: 2020 2020 7365 6c66 2e63 203d 2063 0a0a      self.c = c..
-00000b30: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-00000b40: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00000b50: 2020 2020 2072 6574 7572 6e20 2869 7369       return (isi
-00000b60: 6e73 7461 6e63 6528 6f74 6865 722c 2053  nstance(other, S
-00000b70: 6c6f 7474 6564 2920 616e 640a 2020 2020  lotted) and.    
-00000b80: 2020 2020 2020 2020 2020 2020 616c 6c28              all(
-00000b90: 6765 7461 7474 7228 7365 6c66 2c20 6174  getattr(self, at
-00000ba0: 7472 2920 3d3d 2067 6574 6174 7472 286f  tr) == getattr(o
-00000bb0: 7468 6572 2c20 6174 7472 2920 666f 7220  ther, attr) for 
-00000bc0: 6174 7472 2069 6e20 7365 6c66 2e5f 5f73  attr in self.__s
-00000bd0: 6c6f 7473 5f5f 2929 0a0a 2020 2020 6465  lots__))..    de
-00000be0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-00000bf0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000c00: 2066 227b 7479 7065 2873 656c 6629 2e5f   f"{type(self)._
-00000c10: 5f6e 616d 655f 5f7d 3a28 613d 7b73 656c  _name__}:(a={sel
-00000c20: 662e 617d 2c20 623d 7b73 656c 662e 627d  f.a}, b={self.b}
-00000c30: 2c20 633d 7b73 656c 662e 637d 2922 0a0a  , c={self.c})"..
-00000c40: 0a69 6620 7079 7468 6f6e 5f76 6572 7369  .if python_versi
-00000c50: 6f6e 203e 3d20 2833 2c20 3829 3a0a 2020  on >= (3, 8):.  
-00000c60: 2020 636c 6173 7320 536c 6f74 7465 6457    class SlottedW
-00000c70: 6974 6844 6963 743a 0a20 2020 2020 2020  ithDict:.       
-00000c80: 205f 5f73 6c6f 7473 5f5f 203d 207b 2761   __slots__ = {'a
-00000c90: 273a 2027 6127 2c20 2762 273a 2027 6227  ': 'a', 'b': 'b'
-00000ca0: 2c20 2763 273a 2027 6327 7d0a 0a20 2020  , 'c': 'c'}..   
-00000cb0: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-00000cc0: 5f28 7365 6c66 2c20 612c 2062 2c20 6329  _(self, a, b, c)
-00000cd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00000ce0: 6c66 2e61 203d 2061 0a20 2020 2020 2020  lf.a = a.       
-00000cf0: 2020 2020 2073 656c 662e 6220 3d20 620a       self.b = b.
-00000d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000d10: 2e63 203d 2063 0a0a 2020 2020 2020 2020  .c = c..        
-00000d20: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00000d30: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00000d40: 2020 2020 2072 6574 7572 6e20 2869 7369       return (isi
-00000d50: 6e73 7461 6e63 6528 6f74 6865 722c 2053  nstance(other, S
-00000d60: 6c6f 7474 6564 5769 7468 4469 6374 2920  lottedWithDict) 
-00000d70: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00000d80: 2020 2020 2020 2020 616c 6c28 6765 7461          all(geta
-00000d90: 7474 7228 7365 6c66 2c20 6174 7472 2920  ttr(self, attr) 
-00000da0: 3d3d 2067 6574 6174 7472 286f 7468 6572  == getattr(other
-00000db0: 2c20 6174 7472 2920 666f 7220 6174 7472  , attr) for attr
-00000dc0: 2069 6e20 7365 6c66 2e5f 5f73 6c6f 7473   in self.__slots
-00000dd0: 5f5f 2929 0a0a 2020 2020 2020 2020 6465  __))..        de
-00000de0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-00000df0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000e00: 7475 726e 2066 227b 7479 7065 2873 656c  turn f"{type(sel
-00000e10: 6629 2e5f 5f6e 616d 655f 5f7d 3a28 613d  f).__name__}:(a=
-00000e20: 7b73 656c 662e 617d 2c20 623d 7b73 656c  {self.a}, b={sel
-00000e30: 662e 627d 2c20 633d 7b73 656c 662e 637d  f.b}, c={self.c}
-00000e40: 2922 0a65 6c73 653a 0a20 2020 2053 6c6f  )".else:.    Slo
-00000e50: 7474 6564 5769 7468 4469 6374 203d 204e  ttedWithDict = N
-00000e60: 6f6e 650a 0a0a 636c 6173 7320 5465 7374  one...class Test
-00000e70: 4461 7461 4f62 6a65 6374 7328 756e 6974  DataObjects(unit
-00000e80: 7465 7374 2e54 6573 7443 6173 6529 3a0a  test.TestCase):.
-00000e90: 2020 2020 6465 6620 7465 7374 5f73 6574      def test_set
-00000ea0: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
-00000eb0: 293a 0a20 2020 2020 2020 206f 6220 3d20  ):.        ob = 
-00000ec0: 6c74 2e44 6174 614f 626a 6563 7428 290a  lt.DataObject().
-00000ed0: 2020 2020 2020 2020 6f62 2e7a 203d 2032          ob.z = 2
-00000ee0: 3030 0a20 2020 2020 2020 206f 622e 6120  00.        ob.a 
-00000ef0: 3d20 3130 300a 2020 2020 2020 2020 7769  = 100.        wi
-00000f00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00000f10: 2274 6573 7420 4461 7461 4f62 6a65 6374  "test DataObject
-00000f20: 2061 7474 7269 6275 7465 2073 6574 7469   attribute setti
-00000f30: 6e67 2229 3a0a 2020 2020 2020 2020 2020  ng"):.          
-00000f40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00000f50: 616c 285b 2827 6127 2c20 3130 3029 2c20  al([('a', 100), 
-00000f60: 2827 7a27 2c20 3230 3029 5d2c 2073 6f72  ('z', 200)], sor
-00000f70: 7465 6428 6f62 2e5f 5f64 6963 745f 5f2e  ted(ob.__dict__.
-00000f80: 6974 656d 7328 2929 290a 0a20 2020 2020  items()))..     
-00000f90: 2020 2023 2074 6573 7420 7365 6d69 2d69     # test semi-i
-00000fa0: 6d6d 7574 6162 696c 6974 7920 2863 616e  mmutability (can
-00000fb0: 2774 206f 7665 7277 7269 7465 2065 7869  't overwrite exi
-00000fc0: 7374 696e 6720 6174 7472 6962 7574 6573  sting attributes
-00000fd0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00000fe0: 656c 662e 7375 6254 6573 7428 2274 6573  elf.subTest("tes
-00000ff0: 7420 4461 7461 4f62 6a65 6374 2077 7269  t DataObject wri
-00001000: 7465 2d6f 6e63 6520 2873 656d 692d 696d  te-once (semi-im
-00001010: 6d75 7461 6269 6c69 7479 2922 293a 0a20  mutability)"):. 
-00001020: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00001030: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-00001040: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
-00001050: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00001060: 2020 206f 622e 6120 3d20 3130 310a 0a20     ob.a = 101.. 
-00001070: 2020 2020 2020 2023 2065 7175 616c 6974         # equalit
-00001080: 7920 7465 7374 730a 2020 2020 2020 2020  y tests.        
-00001090: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-000010a0: 7428 2274 6573 7420 4461 7461 4f62 6a65  t("test DataObje
-000010b0: 6374 2065 7175 616c 6974 7922 293a 0a20  ct equality"):. 
-000010c0: 2020 2020 2020 2020 2020 206f 6232 203d             ob2 =
-000010d0: 206c 742e 4461 7461 4f62 6a65 6374 282a   lt.DataObject(*
-000010e0: 2a7b 2761 273a 2031 3030 2c20 277a 273a  *{'a': 100, 'z':
-000010f0: 2032 3030 7d29 0a20 2020 2020 2020 2020   200}).         
-00001100: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00001110: 7561 6c28 6f62 322c 206f 6229 0a0a 2020  ual(ob2, ob)..  
-00001120: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00001130: 7375 6254 6573 7428 2274 6573 7420 4461  subTest("test Da
-00001140: 7461 4f62 6a65 6374 2069 6e65 7175 616c  taObject inequal
-00001150: 6974 7922 293a 0a20 2020 2020 2020 2020  ity"):.         
-00001160: 2020 206f 6232 2e62 203d 2027 626c 6168     ob2.b = 'blah
-00001170: 270a 2020 2020 2020 2020 2020 2020 7365  '.            se
-00001180: 6c66 2e61 7373 6572 744e 6f74 4571 7561  lf.assertNotEqua
-00001190: 6c28 6f62 2c20 6f62 3229 0a0a 2020 2020  l(ob, ob2)..    
-000011a0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000011b0: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
-000011c0: 4f62 6a65 6374 2065 7175 616c 6974 7920  Object equality 
-000011d0: 6166 7465 7220 7570 6461 7465 7322 293a  after updates"):
-000011e0: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-000011f0: 206f 6232 2e62 0a20 2020 2020 2020 2020   ob2.b.         
-00001200: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00001210: 7561 6c28 6f62 322c 206f 6229 0a0a 2020  ual(ob2, ob)..  
-00001220: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00001230: 7375 6254 6573 7428 2274 6573 7420 4461  subTest("test Da
-00001240: 7461 4f62 6a65 6374 204b 6579 4572 726f  taObject KeyErro
-00001250: 7222 293a 0a20 2020 2020 2020 2020 2020  r"):.           
-00001260: 2064 656c 206f 6232 2e61 0a20 2020 2020   del ob2.a.     
-00001270: 2020 2020 2020 2064 656c 206f 6232 2e7a         del ob2.z
-00001280: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00001290: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-000012a0: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 6f62 325b 2761 275d 0a20 2020 2020 2020  ob2['a'].       
-000012d0: 2020 2020 206f 6232 5b27 6127 5d20 3d20       ob2['a'] = 
-000012e0: 3130 0a20 2020 2020 2020 2020 2020 206f  10.            o
-000012f0: 6232 5b27 6127 5d0a 0a20 2020 2020 2020  b2['a']..       
-00001300: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00001310: 7374 2822 7465 7374 2044 6174 614f 626a  st("test DataObj
-00001320: 6563 7420 4b65 7945 7272 6f72 2028 3229  ect KeyError (2)
-00001330: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00001340: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-00001350: 5261 6973 6573 284b 6579 4572 726f 7229  Raises(KeyError)
-00001360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001370: 2020 6f62 325b 2761 275d 203d 2031 300a    ob2['a'] = 10.
-00001380: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00001390: 6c66 2e73 7562 5465 7374 2822 7465 7374  lf.subTest("test
-000013a0: 2044 6174 614f 626a 6563 7420 7265 7072   DataObject repr
-000013b0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000013c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000013d0: 2822 7b27 6127 3a20 3130 7d22 2c20 7265  ("{'a': 10}", re
-000013e0: 7072 286f 6232 2929 0a0a 0a63 6c61 7373  pr(ob2))...class
-000013f0: 2054 6573 7454 6162 6c65 5479 7065 7328   TestTableTypes(
-00001400: 756e 6974 7465 7374 2e54 6573 7443 6173  unittest.TestCas
-00001410: 6529 3a0a 2020 2020 6465 6620 7465 7374  e):.    def test
-00001420: 5f74 7970 6573 2873 656c 6629 3a0a 0a20  _types(self):.. 
-00001430: 2020 2020 2020 2023 2063 6865 636b 2074         # check t
-00001440: 6861 7420 5461 626c 6520 616e 6420 496e  hat Table and In
-00001450: 6465 7820 6172 6520 7265 636f 676e 697a  dex are recogniz
-00001460: 6564 2061 7320 5365 7175 656e 6365 2061  ed as Sequence a
-00001470: 6e64 204d 6170 7069 6e67 2074 7970 6573  nd Mapping types
-00001480: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00001490: 6c66 2e73 7562 5465 7374 2822 6368 6563  lf.subTest("chec
-000014a0: 6b20 7468 6174 2054 6162 6c65 2069 7320  k that Table is 
-000014b0: 7265 636f 676e 697a 6564 2061 7320 5365  recognized as Se
-000014c0: 7175 656e 6365 2074 7970 6522 293a 0a20  quence type"):. 
-000014d0: 2020 2020 2020 2020 2020 2074 203d 206c             t = l
-000014e0: 742e 5461 626c 6528 290a 2020 2020 2020  t.Table().      
-000014f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00001500: 7454 7275 6528 6973 696e 7374 616e 6365  tTrue(isinstance
-00001510: 2874 2c20 6c74 2e53 6571 7565 6e63 6529  (t, lt.Sequence)
-00001520: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00001530: 7365 6c66 2e73 7562 5465 7374 2822 6368  self.subTest("ch
-00001540: 6563 6b20 7468 6174 2049 6e64 6578 2069  eck that Index i
-00001550: 7320 7265 636f 676e 697a 6564 2061 7320  s recognized as 
-00001560: 4d61 7070 696e 6720 7479 7065 2229 3a0a  Mapping type"):.
-00001570: 2020 2020 2020 2020 2020 2020 742e 6372              t.cr
-00001580: 6561 7465 5f69 6e64 6578 2822 7822 290a  eate_index("x").
-00001590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000015a0: 2e61 7373 6572 7454 7275 6528 6973 696e  .assertTrue(isin
-000015b0: 7374 616e 6365 2874 2e67 6574 5f69 6e64  stance(t.get_ind
-000015c0: 6578 2827 7827 292c 206c 742e 4d61 7070  ex('x'), lt.Mapp
-000015d0: 696e 6729 290a 0a20 2020 2020 2020 2023  ing))..        #
-000015e0: 206d 616b 6520 7375 7265 2067 6574 5f69   make sure get_i
-000015f0: 6e64 6578 2072 6574 7572 6e73 2061 2072  ndex returns a r
-00001600: 6561 642d 6f6e 6c79 2061 6363 6573 7320  ead-only access 
-00001610: 746f 2074 6865 2075 6e64 6572 6c79 696e  to the underlyin
-00001620: 6720 696e 6465 780a 2020 2020 2020 2020  g index.        
-00001630: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00001640: 7428 2263 6865 636b 2074 6861 7420 6765  t("check that ge
-00001650: 745f 696e 6465 7820 7265 7475 726e 7320  t_index returns 
-00001660: 6120 7265 6164 2d6f 6e6c 7920 6163 6365  a read-only acce
-00001670: 7373 2074 6f20 7468 6520 756e 6465 726c  ss to the underl
-00001680: 7969 6e67 2069 6e64 6578 2229 3a0a 2020  ying index"):.  
-00001690: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-000016a0: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-000016b0: 286c 742e 5265 6164 6f6e 6c79 496e 6465  (lt.ReadonlyInde
-000016c0: 7841 6363 6573 7345 7272 6f72 293a 0a20  xAccessError):. 
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000016e0: 2e67 6574 5f69 6e64 6578 2822 7822 295b  .get_index("x")[
-000016f0: 2761 275d 203d 2031 3030 0a0a 0a64 6566  'a'] = 100...def
-00001700: 2061 6e6e 6f75 6e63 655f 7465 7374 2866   announce_test(f
-00001710: 6e29 3a0a 2020 2020 6465 6620 5f69 6e6e  n):.    def _inn
-00001720: 6572 282a 6172 6773 293a 0a20 2020 2020  er(*args):.     
-00001730: 2020 2070 7269 6e74 2822 5c6e 2220 2b20     print("\n" + 
-00001740: 222d 2220 2a20 3530 290a 2020 2020 2020  "-" * 50).      
-00001750: 2020 7072 696e 7428 6622 7b74 7970 6528    print(f"{type(
-00001760: 6172 6773 5b30 5d29 2e5f 5f6e 616d 655f  args[0]).__name_
-00001770: 5f7d 2e7b 666e 2e5f 5f6e 616d 655f 5f7d  _}.{fn.__name__}
-00001780: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00001790: 6e20 666e 282a 6172 6773 290a 0a20 2020  n fn(*args)..   
-000017a0: 2072 6574 7572 6e20 5f69 6e6e 6572 0a0a   return _inner..
-000017b0: 0a64 6566 206d 616b 655f 7465 7374 5f63  .def make_test_c
-000017c0: 6c61 7373 282a 636c 6173 7365 7329 3a0a  lass(*classes):.
-000017d0: 0a20 2020 2063 6c61 7373 5f6e 616d 6520  .    class_name 
-000017e0: 3d20 225f 222e 6a6f 696e 2863 2e5f 5f6e  = "_".join(c.__n
-000017f0: 616d 655f 5f20 666f 7220 6320 696e 2063  ame__ for c in c
-00001800: 6c61 7373 6573 290a 2020 2020 6966 206e  lasses).    if n
-00001810: 6f74 2069 7373 7562 636c 6173 7328 636c  ot issubclass(cl
-00001820: 6173 7365 735b 305d 2c20 756e 6974 7465  asses[0], unitte
-00001830: 7374 2e54 6573 7443 6173 6529 3a0a 2020  st.TestCase):.  
-00001840: 2020 2020 2020 636c 7320 3d20 7479 7065        cls = type
-00001850: 2863 6c61 7373 5f6e 616d 652c 2028 756e  (class_name, (un
-00001860: 6974 7465 7374 2e54 6573 7443 6173 652c  ittest.TestCase,
-00001870: 202a 636c 6173 7365 7329 2c20 7b7d 290a   *classes), {}).
-00001880: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001890: 2020 636c 7320 3d20 7479 7065 2863 6c61    cls = type(cla
-000018a0: 7373 5f6e 616d 652c 2074 7570 6c65 2863  ss_name, tuple(c
-000018b0: 6c61 7373 6573 292c 207b 7d29 0a20 2020  lasses), {}).   
-000018c0: 2066 6f72 2061 7474 7220 696e 2064 6972   for attr in dir
-000018d0: 2863 6c73 293a 0a20 2020 2020 2020 2061  (cls):.        a
-000018e0: 7474 7276 616c 7565 203d 2067 6574 6174  ttrvalue = getat
-000018f0: 7472 2863 6c73 2c20 6174 7472 290a 2020  tr(cls, attr).  
-00001900: 2020 2020 2020 6966 2061 7474 722e 7374        if attr.st
-00001910: 6172 7473 7769 7468 2822 7465 7374 5f22  artswith("test_"
-00001920: 2920 616e 6420 6361 6c6c 6162 6c65 2861  ) and callable(a
-00001930: 7474 7276 616c 7565 293a 0a20 2020 2020  ttrvalue):.     
-00001940: 2020 2020 2020 2073 6574 6174 7472 2863         setattr(c
-00001950: 6c73 2c20 6174 7472 2c20 616e 6e6f 756e  ls, attr, announ
-00001960: 6365 5f74 6573 7428 6174 7472 7661 6c75  ce_test(attrvalu
-00001970: 6529 290a 2020 2020 676c 6f62 616c 7328  e)).    globals(
-00001980: 295b 636c 732e 5f5f 6e61 6d65 5f5f 5d20  )[cls.__name__] 
-00001990: 3d20 636c 730a 0a0a 6465 6620 6d61 6b65  = cls...def make
-000019a0: 5f74 6573 745f 636c 6173 7365 7328 636c  _test_classes(cl
-000019b0: 7329 3a0a 2020 2020 6d61 6b65 5f74 6573  s):.    make_tes
-000019c0: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
-000019d0: 6e67 4461 7461 4f62 6a65 6374 7329 0a20  ngDataObjects). 
-000019e0: 2020 206d 616b 655f 7465 7374 5f63 6c61     make_test_cla
-000019f0: 7373 2863 6c73 2c20 5573 696e 674e 616d  ss(cls, UsingNam
-00001a00: 6564 7475 706c 6573 290a 2020 2020 6d61  edtuples).    ma
-00001a10: 6b65 5f74 6573 745f 636c 6173 7328 636c  ke_test_class(cl
-00001a20: 732c 2055 7369 6e67 4461 7461 4e61 6d65  s, UsingDataName
-00001a30: 6474 7570 6c65 7329 0a20 2020 206d 616b  dtuples).    mak
-00001a40: 655f 7465 7374 5f63 6c61 7373 2863 6c73  e_test_class(cls
-00001a50: 2c20 5573 696e 6753 6c6f 7474 6564 4f62  , UsingSlottedOb
-00001a60: 6a65 6374 7329 0a20 2020 2069 6620 536c  jects).    if Sl
-00001a70: 6f74 7465 6457 6974 6844 6963 7420 6973  ottedWithDict is
-00001a80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00001a90: 2020 206d 616b 655f 7465 7374 5f63 6c61     make_test_cla
-00001aa0: 7373 2863 6c73 2c20 5573 696e 6753 6c6f  ss(cls, UsingSlo
-00001ab0: 7474 6564 5769 7468 4469 6374 4f62 6a65  ttedWithDictObje
-00001ac0: 6374 7329 0a20 2020 206d 616b 655f 7465  cts).    make_te
-00001ad0: 7374 5f63 6c61 7373 2863 6c73 2c20 5573  st_class(cls, Us
-00001ae0: 696e 6753 696d 706c 654e 616d 6573 7061  ingSimpleNamespa
-00001af0: 6365 290a 2020 2020 6966 2064 6174 6163  ce).    if datac
-00001b00: 6c61 7373 6573 2069 7320 6e6f 7420 4e6f  lasses is not No
-00001b10: 6e65 3a0a 2020 2020 2020 2020 6d61 6b65  ne:.        make
-00001b20: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
-00001b30: 2055 7369 6e67 4461 7461 636c 6173 7365   UsingDataclasse
-00001b40: 7329 0a20 2020 2069 6620 7079 6461 6e74  s).    if pydant
-00001b50: 6963 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ic is not None:.
-00001b60: 2020 2020 2020 2020 6d61 6b65 5f74 6573          make_tes
-00001b70: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
-00001b80: 6e67 5079 6461 6e74 6963 4d6f 6465 6c29  ngPydanticModel)
-00001b90: 0a20 2020 2020 2020 206d 616b 655f 7465  .        make_te
-00001ba0: 7374 5f63 6c61 7373 2863 6c73 2c20 5573  st_class(cls, Us
-00001bb0: 696e 6750 7964 616e 7469 6349 6d6d 7574  ingPydanticImmut
-00001bc0: 6162 6c65 4d6f 6465 6c29 0a20 2020 2020  ableModel).     
-00001bd0: 2020 206d 616b 655f 7465 7374 5f63 6c61     make_test_cla
-00001be0: 7373 2863 6c73 2c20 5573 696e 6750 7964  ss(cls, UsingPyd
-00001bf0: 616e 7469 634f 524d 4d6f 6465 6c29 0a20  anticORMModel). 
-00001c00: 2020 2069 6620 6174 7472 2069 7320 6e6f     if attr is no
-00001c10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00001c20: 6d61 6b65 5f74 6573 745f 636c 6173 7328  make_test_class(
-00001c30: 636c 732c 2055 7369 6e67 4174 7472 436c  cls, UsingAttrCl
-00001c40: 6173 7329 0a20 2020 2069 6620 7472 6169  ass).    if trai
-00001c50: 746c 6574 7320 6973 206e 6f74 204e 6f6e  tlets is not Non
-00001c60: 653a 0a20 2020 2020 2020 206d 616b 655f  e:.        make_
-00001c70: 7465 7374 5f63 6c61 7373 2863 6c73 2c20  test_class(cls, 
-00001c80: 5573 696e 6754 7261 6974 6c65 7473 436c  UsingTraitletsCl
-00001c90: 6173 7329 0a0a 0a63 6c61 7373 2041 6273  ass)...class Abs
-00001ca0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
-00001cb0: 4661 6374 6f72 793a 0a20 2020 2064 6174  Factory:.    dat
-00001cc0: 615f 6f62 6a65 6374 5f74 7970 653a 204f  a_object_type: O
-00001cd0: 7074 696f 6e61 6c5b 7479 7065 5d20 3d20  ptional[type] = 
-00001ce0: 4e6f 6e65 0a0a 2020 2020 4063 6c61 7373  None..    @class
-00001cf0: 6d65 7468 6f64 0a20 2020 2064 6566 206d  method.    def m
-00001d00: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00001d10: 636c 732c 2061 2c20 622c 2063 293a 0a20  cls, a, b, c):. 
-00001d20: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00001d30: 732e 6461 7461 5f6f 626a 6563 745f 7479  s.data_object_ty
-00001d40: 7065 2861 3d61 2c20 623d 622c 2063 3d63  pe(a=a, b=b, c=c
-00001d50: 290a 0a0a 636c 6173 7320 5573 696e 6744  )...class UsingD
-00001d60: 6174 614f 626a 6563 7473 2841 6273 7472  ataObjects(Abstr
-00001d70: 6163 7443 6f6e 7465 6e74 5479 7065 4661  actContentTypeFa
-00001d80: 6374 6f72 7929 3a0a 2020 2020 6461 7461  ctory):.    data
-00001d90: 5f6f 626a 6563 745f 7479 7065 203d 206c  _object_type = l
-00001da0: 742e 4461 7461 4f62 6a65 6374 0a0a 0a63  t.DataObject...c
-00001db0: 6c61 7373 2055 7369 6e67 4e61 6d65 6474  lass UsingNamedt
-00001dc0: 7570 6c65 7328 4162 7374 7261 6374 436f  uples(AbstractCo
-00001dd0: 6e74 656e 7454 7970 6546 6163 746f 7279  ntentTypeFactory
-00001de0: 293a 0a20 2020 2064 6174 615f 6f62 6a65  ):.    data_obje
-00001df0: 6374 5f74 7970 6520 3d20 4461 7461 5475  ct_type = DataTu
-00001e00: 706c 650a 0a0a 636c 6173 7320 5573 696e  ple...class Usin
-00001e10: 6744 6174 614e 616d 6564 7475 706c 6573  gDataNamedtuples
-00001e20: 2841 6273 7472 6163 7443 6f6e 7465 6e74  (AbstractContent
-00001e30: 5479 7065 4661 6374 6f72 7929 3a0a 2020  TypeFactory):.  
-00001e40: 2020 6461 7461 5f6f 626a 6563 745f 7479    data_object_ty
-00001e50: 7065 203d 2044 6174 614e 616d 6564 5475  pe = DataNamedTu
-00001e60: 706c 650a 0a0a 636c 6173 7320 5573 696e  ple...class Usin
-00001e70: 6753 6c6f 7474 6564 4f62 6a65 6374 7328  gSlottedObjects(
-00001e80: 4162 7374 7261 6374 436f 6e74 656e 7454  AbstractContentT
-00001e90: 7970 6546 6163 746f 7279 293a 0a20 2020  ypeFactory):.   
-00001ea0: 2064 6174 615f 6f62 6a65 6374 5f74 7970   data_object_typ
-00001eb0: 6520 3d20 536c 6f74 7465 640a 0a0a 6966  e = Slotted...if
-00001ec0: 2053 6c6f 7474 6564 5769 7468 4469 6374   SlottedWithDict
-00001ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00001ee0: 2020 636c 6173 7320 5573 696e 6753 6c6f    class UsingSlo
-00001ef0: 7474 6564 5769 7468 4469 6374 4f62 6a65  ttedWithDictObje
-00001f00: 6374 7328 4162 7374 7261 6374 436f 6e74  cts(AbstractCont
-00001f10: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
-00001f20: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
-00001f30: 6a65 6374 5f74 7970 6520 3d20 536c 6f74  ject_type = Slot
-00001f40: 7465 6457 6974 6844 6963 740a 656c 7365  tedWithDict.else
-00001f50: 3a0a 2020 2020 5573 696e 6753 6c6f 7474  :.    UsingSlott
-00001f60: 6564 5769 7468 4469 6374 4f62 6a65 6374  edWithDictObject
-00001f70: 7320 3d20 4162 7374 7261 6374 436f 6e74  s = AbstractCont
-00001f80: 656e 7454 7970 6546 6163 746f 7279 0a0a  entTypeFactory..
-00001f90: 0a63 6c61 7373 2055 7369 6e67 5369 6d70  .class UsingSimp
-00001fa0: 6c65 4e61 6d65 7370 6163 6528 4162 7374  leNamespace(Abst
-00001fb0: 7261 6374 436f 6e74 656e 7454 7970 6546  ractContentTypeF
-00001fc0: 6163 746f 7279 293a 0a20 2020 2064 6174  actory):.    dat
-00001fd0: 615f 6f62 6a65 6374 5f74 7970 6520 3d20  a_object_type = 
-00001fe0: 5369 6d70 6c65 4e61 6d65 7370 6163 650a  SimpleNamespace.
-00001ff0: 0a0a 6966 2064 6174 6163 6c61 7373 6573  ..if dataclasses
-00002000: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00002010: 2020 636c 6173 7320 5573 696e 6744 6174    class UsingDat
-00002020: 6163 6c61 7373 6573 2841 6273 7472 6163  aclasses(Abstrac
-00002030: 7443 6f6e 7465 6e74 5479 7065 4661 6374  tContentTypeFact
-00002040: 6f72 7929 3a0a 2020 2020 2020 2020 6461  ory):.        da
-00002050: 7461 5f6f 626a 6563 745f 7479 7065 203d  ta_object_type =
-00002060: 2044 6174 6144 6174 6163 6c61 7373 0a65   DataDataclass.e
-00002070: 6c73 653a 0a20 2020 2055 7369 6e67 4461  lse:.    UsingDa
-00002080: 7461 636c 6173 7365 7320 3d20 4162 7374  taclasses = Abst
-00002090: 7261 6374 436f 6e74 656e 7454 7970 6546  ractContentTypeF
-000020a0: 6163 746f 7279 0a0a 0a69 6620 7079 6461  actory...if pyda
-000020b0: 6e74 6963 2069 7320 6e6f 7420 4e6f 6e65  ntic is not None
-000020c0: 3a0a 2020 2020 636c 6173 7320 5573 696e  :.    class Usin
-000020d0: 6750 7964 616e 7469 634d 6f64 656c 2841  gPydanticModel(A
-000020e0: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
-000020f0: 7065 4661 6374 6f72 7929 3a0a 2020 2020  peFactory):.    
-00002100: 2020 2020 6461 7461 5f6f 626a 6563 745f      data_object_
-00002110: 7479 7065 203d 2044 6174 6150 7964 616e  type = DataPydan
-00002120: 7469 634d 6f64 656c 0a0a 2020 2020 636c  ticModel..    cl
-00002130: 6173 7320 5573 696e 6750 7964 616e 7469  ass UsingPydanti
-00002140: 6349 6d6d 7574 6162 6c65 4d6f 6465 6c28  cImmutableModel(
-00002150: 4162 7374 7261 6374 436f 6e74 656e 7454  AbstractContentT
-00002160: 7970 6546 6163 746f 7279 293a 0a20 2020  ypeFactory):.   
-00002170: 2020 2020 2064 6174 615f 6f62 6a65 6374       data_object
-00002180: 5f74 7970 6520 3d20 4461 7461 5079 6461  _type = DataPyda
-00002190: 6e74 6963 496d 6d75 7461 626c 654d 6f64  nticImmutableMod
-000021a0: 656c 0a0a 2020 2020 636c 6173 7320 5573  el..    class Us
-000021b0: 696e 6750 7964 616e 7469 634f 524d 4d6f  ingPydanticORMMo
-000021c0: 6465 6c28 4162 7374 7261 6374 436f 6e74  del(AbstractCont
-000021d0: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
-000021e0: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
-000021f0: 6a65 6374 5f74 7970 6520 3d20 4461 7461  ject_type = Data
-00002200: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-00002210: 0a0a 656c 7365 3a0a 2020 2020 5573 696e  ..else:.    Usin
-00002220: 6750 7964 616e 7469 634d 6f64 656c 203d  gPydanticModel =
-00002230: 2041 6273 7472 6163 7443 6f6e 7465 6e74   AbstractContent
-00002240: 5479 7065 4661 6374 6f72 790a 2020 2020  TypeFactory.    
-00002250: 5573 696e 6750 7964 616e 7469 6349 6d6d  UsingPydanticImm
-00002260: 7574 6162 6c65 4d6f 6465 6c20 3d20 4162  utableModel = Ab
-00002270: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
-00002280: 6546 6163 746f 7279 0a20 2020 2055 7369  eFactory.    Usi
-00002290: 6e67 5079 6461 6e74 6963 4f52 4d4d 6f64  ngPydanticORMMod
-000022a0: 656c 203d 2041 6273 7472 6163 7443 6f6e  el = AbstractCon
-000022b0: 7465 6e74 5479 7065 4661 6374 6f72 790a  tentTypeFactory.
-000022c0: 0a69 6620 6174 7472 2069 7320 6e6f 7420  .if attr is not 
-000022d0: 4e6f 6e65 3a0a 2020 2020 636c 6173 7320  None:.    class 
-000022e0: 5573 696e 6741 7474 7243 6c61 7373 2841  UsingAttrClass(A
+00000040: 7420 6173 740a 696d 706f 7274 2063 6f6e  t ast.import con
+00000050: 7465 7874 6c69 620a 696d 706f 7274 2074  textlib.import t
+00000060: 7970 696e 670a 6672 6f6d 2063 6f6c 6c65  yping.from colle
+00000070: 6374 696f 6e73 2069 6d70 6f72 7420 6e61  ctions import na
+00000080: 6d65 6474 7570 6c65 0a69 6d70 6f72 7420  medtuple.import 
+00000090: 636f 7079 0a69 6d70 6f72 7420 696f 0a69  copy.import io.i
+000000a0: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
+000000b0: 696d 706f 7274 206a 736f 6e0a 6672 6f6d  import json.from
+000000c0: 206f 7065 7261 746f 7220 696d 706f 7274   operator import
+000000d0: 2061 7474 7267 6574 7465 720a 696d 706f   attrgetter.impo
+000000e0: 7274 206f 730a 696d 706f 7274 2073 7973  rt os.import sys
+000000f0: 0a69 6d70 6f72 7420 7465 7874 7772 6170  .import textwrap
+00000100: 0a66 726f 6d20 7479 7065 7320 696d 706f  .from types impo
+00000110: 7274 2053 696d 706c 654e 616d 6573 7061  rt SimpleNamespa
+00000120: 6365 0a69 6d70 6f72 7420 756e 6974 7465  ce.import unitte
+00000130: 7374 0a66 726f 6d20 7479 7069 6e67 2069  st.from typing i
+00000140: 6d70 6f72 7420 4f70 7469 6f6e 616c 2c20  mport Optional, 
+00000150: 556e 696f 6e0a 0a69 6d70 6f72 7420 6c69  Union..import li
+00000160: 7474 6c65 7461 626c 6520 6173 206c 740a  ttletable as lt.
+00000170: 0a53 4b49 505f 4353 565f 494d 504f 5254  .SKIP_CSV_IMPORT
+00000180: 5f55 5349 4e47 5f55 524c 5f54 4553 5453  _USING_URL_TESTS
+00000190: 203d 206f 732e 656e 7669 726f 6e2e 6765   = os.environ.ge
+000001a0: 7428 2253 4b49 505f 4353 565f 494d 504f  t("SKIP_CSV_IMPO
+000001b0: 5254 5f55 5349 4e47 5f55 524c 5f54 4553  RT_USING_URL_TES
+000001c0: 5453 222c 2022 3022 2920 3d3d 2022 3122  TS", "0") == "1"
+000001d0: 0a0a 0a40 636f 6e74 6578 746c 6962 2e63  ...@contextlib.c
+000001e0: 6f6e 7465 7874 6d61 6e61 6765 720a 6465  ontextmanager.de
+000001f0: 6620 7469 6d65 7374 616d 705f 7374 6172  f timestamp_star
+00000200: 745f 656e 6428 6c61 6265 6c3d 4e6f 6e65  t_end(label=None
+00000210: 2c20 6669 6c65 3d4e 6f6e 6529 3a0a 2020  , file=None):.  
+00000220: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
+00000230: 650a 0a20 2020 2072 6574 203d 2053 696d  e..    ret = Sim
+00000240: 706c 654e 616d 6573 7061 6365 2829 0a20  pleNamespace(). 
+00000250: 2020 2072 6574 2e73 7461 7274 203d 2064     ret.start = d
+00000260: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00000270: 2e6e 6f77 2829 2e61 7374 696d 657a 6f6e  .now().astimezon
+00000280: 6528 6461 7465 7469 6d65 2e55 5443 290a  e(datetime.UTC).
+00000290: 2020 2020 6966 206c 6162 656c 3a0a 2020      if label:.  
+000002a0: 2020 2020 2020 7072 696e 7428 6622 5374        print(f"St
+000002b0: 6172 7420 2d20 7b6c 6162 656c 7d3a 207b  art - {label}: {
+000002c0: 7265 742e 7374 6172 747d 222c 2066 696c  ret.start}", fil
+000002d0: 653d 6669 6c65 290a 2020 2020 7969 656c  e=file).    yiel
+000002e0: 6420 7265 740a 2020 2020 7265 742e 656e  d ret.    ret.en
+000002f0: 6420 3d20 6461 7465 7469 6d65 2e64 6174  d = datetime.dat
+00000300: 6574 696d 652e 6e6f 7728 292e 6173 7469  etime.now().asti
+00000310: 6d65 7a6f 6e65 2864 6174 6574 696d 652e  mezone(datetime.
+00000320: 5554 4329 0a20 2020 2072 6574 2e65 6c61  UTC).    ret.ela
+00000330: 7073 6564 203d 2072 6574 2e65 6e64 202d  psed = ret.end -
+00000340: 2072 6574 2e73 7461 7274 0a20 2020 2069   ret.start.    i
+00000350: 6620 6c61 6265 6c3a 0a20 2020 2020 2020  f label:.       
+00000360: 2070 7269 6e74 2866 2245 6e64 2020 202d   print(f"End   -
+00000370: 207b 6c61 6265 6c7d 3a20 7b72 6574 2e65   {label}: {ret.e
+00000380: 6e64 7d22 2c20 6669 6c65 3d66 696c 6529  nd}", file=file)
+00000390: 0a0a 0a69 6d70 6f72 7420 6461 7461 636c  ...import datacl
+000003a0: 6173 7365 730a 4064 6174 6163 6c61 7373  asses.@dataclass
+000003b0: 6573 2e64 6174 6163 6c61 7373 0a63 6c61  es.dataclass.cla
+000003c0: 7373 2044 6174 6144 6174 6163 6c61 7373  ss DataDataclass
+000003d0: 3a0a 2020 2020 613a 2069 6e74 0a20 2020  :.    a: int.   
+000003e0: 2062 3a20 696e 740a 2020 2020 633a 2069   b: int.    c: i
+000003f0: 6e74 0a0a 7472 793a 0a20 2020 2069 6d70  nt..try:.    imp
+00000400: 6f72 7420 7079 6461 6e74 6963 0a65 7863  ort pydantic.exc
+00000410: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
+00000420: 0a20 2020 2070 7269 6e74 2822 7079 6461  .    print("pyda
+00000430: 6e74 6963 2074 6573 7473 2064 6973 6162  ntic tests disab
+00000440: 6c65 6422 290a 2020 2020 7079 6461 6e74  led").    pydant
+00000450: 6963 203d 204e 6f6e 650a 656c 7365 3a0a  ic = None.else:.
+00000460: 2020 2020 636c 6173 7320 4461 7461 5079      class DataPy
+00000470: 6461 6e74 6963 4d6f 6465 6c28 7079 6461  danticModel(pyda
+00000480: 6e74 6963 2e42 6173 654d 6f64 656c 293a  ntic.BaseModel):
+00000490: 0a20 2020 2020 2020 2061 3a20 4f70 7469  .        a: Opti
+000004a0: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
+000004b0: 7374 725d 5d0a 2020 2020 2020 2020 623a  str]].        b:
+000004c0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+000004d0: 696e 742c 2073 7472 5d5d 0a20 2020 2020  int, str]].     
+000004e0: 2020 2063 3a20 4f70 7469 6f6e 616c 5b55     c: Optional[U
+000004f0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d0a  nion[int, str]].
+00000500: 0a20 2020 2063 6c61 7373 2044 6174 6150  .    class DataP
+00000510: 7964 616e 7469 6349 6d6d 7574 6162 6c65  ydanticImmutable
+00000520: 4d6f 6465 6c28 7079 6461 6e74 6963 2e42  Model(pydantic.B
+00000530: 6173 654d 6f64 656c 293a 0a20 2020 2020  aseModel):.     
+00000540: 2020 2063 6c61 7373 2043 6f6e 6669 673a     class Config:
+00000550: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+00000560: 6f77 5f6d 7574 6174 696f 6e20 3d20 4661  ow_mutation = Fa
+00000570: 6c73 650a 0a20 2020 2020 2020 2061 3a20  lse..        a: 
+00000580: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b69  Optional[Union[i
+00000590: 6e74 2c20 7374 725d 5d0a 2020 2020 2020  nt, str]].      
+000005a0: 2020 623a 204f 7074 696f 6e61 6c5b 556e    b: Optional[Un
+000005b0: 696f 6e5b 696e 742c 2073 7472 5d5d 0a20  ion[int, str]]. 
+000005c0: 2020 2020 2020 2063 3a20 4f70 7469 6f6e         c: Option
+000005d0: 616c 5b55 6e69 6f6e 5b69 6e74 2c20 7374  al[Union[int, st
+000005e0: 725d 5d0a 0a20 2020 2063 6c61 7373 2044  r]]..    class D
+000005f0: 6174 6150 7964 616e 7469 634f 524d 4d6f  ataPydanticORMMo
+00000600: 6465 6c28 7079 6461 6e74 6963 2e42 6173  del(pydantic.Bas
+00000610: 654d 6f64 656c 293a 0a20 2020 2020 2020  eModel):.       
+00000620: 2063 6c61 7373 2043 6f6e 6669 673a 0a20   class Config:. 
+00000630: 2020 2020 2020 2020 2020 206f 726d 5f6d             orm_m
+00000640: 6f64 6520 3d20 5472 7565 0a0a 2020 2020  ode = True..    
+00000650: 2020 2020 613a 204f 7074 696f 6e61 6c5b      a: Optional[
+00000660: 556e 696f 6e5b 696e 742c 2073 7472 5d5d  Union[int, str]]
+00000670: 0a20 2020 2020 2020 2062 3a20 4f70 7469  .        b: Opti
+00000680: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
+00000690: 7374 725d 5d0a 2020 2020 2020 2020 633a  str]].        c:
+000006a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+000006b0: 696e 742c 2073 7472 5d5d 0a0a 7472 793a  int, str]]..try:
+000006c0: 0a20 2020 2069 6d70 6f72 7420 6174 7472  .    import attr
+000006d0: 0a65 7863 6570 7420 496d 706f 7274 4572  .except ImportEr
+000006e0: 726f 723a 0a20 2020 2070 7269 6e74 2822  ror:.    print("
+000006f0: 6174 7472 7320 7465 7374 7320 6469 7361  attrs tests disa
+00000700: 626c 6564 2229 0a20 2020 2061 7474 7220  bled").    attr 
+00000710: 3d20 4e6f 6e65 0a65 6c73 653a 0a20 2020  = None.else:.   
+00000720: 2041 7474 7243 6c61 7373 203d 2061 7474   AttrClass = att
+00000730: 722e 6d61 6b65 5f63 6c61 7373 2822 4174  r.make_class("At
+00000740: 7472 436c 6173 7322 2c20 5b22 6122 2c20  trClass", ["a", 
+00000750: 2262 222c 2022 6322 5d29 0a0a 7472 793a  "b", "c"])..try:
+00000760: 0a20 2020 2069 6d70 6f72 7420 7472 6169  .    import trai
+00000770: 746c 6574 730a 6578 6365 7074 2049 6d70  tlets.except Imp
+00000780: 6f72 7445 7272 6f72 3a0a 2020 2020 7072  ortError:.    pr
+00000790: 696e 7428 2274 7261 6974 6c65 7473 2074  int("traitlets t
+000007a0: 6573 7473 2064 6973 6162 6c65 6422 290a  ests disabled").
+000007b0: 2020 2020 7472 6169 746c 6574 7320 3d20      traitlets = 
+000007c0: 4e6f 6e65 0a65 6c73 653a 0a20 2020 2063  None.else:.    c
+000007d0: 6c61 7373 2054 7261 6974 6c65 7473 436c  lass TraitletsCl
+000007e0: 6173 7328 6c74 2e48 6173 5472 6169 7473  ass(lt.HasTraits
+000007f0: 4d69 7869 6e2c 2074 7261 6974 6c65 7473  Mixin, traitlets
+00000800: 2e48 6173 5472 6169 7473 293a 0a20 2020  .HasTraits):.   
+00000810: 2020 2020 2061 203d 2074 7261 6974 6c65       a = traitle
+00000820: 7473 2e55 6e69 6f6e 285b 7472 6169 746c  ts.Union([traitl
+00000830: 6574 732e 496e 7428 292c 2074 7261 6974  ets.Int(), trait
+00000840: 6c65 7473 2e55 6e69 636f 6465 2829 5d2c  lets.Unicode()],
+00000850: 2061 6c6c 6f77 5f6e 6f6e 653d 5472 7565   allow_none=True
+00000860: 290a 2020 2020 2020 2020 6220 3d20 7472  ).        b = tr
+00000870: 6169 746c 6574 732e 556e 696f 6e28 5b74  aitlets.Union([t
+00000880: 7261 6974 6c65 7473 2e49 6e74 2829 2c20  raitlets.Int(), 
+00000890: 7472 6169 746c 6574 732e 556e 6963 6f64  traitlets.Unicod
+000008a0: 6528 295d 2c20 616c 6c6f 775f 6e6f 6e65  e()], allow_none
+000008b0: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
+000008c0: 203d 2074 7261 6974 6c65 7473 2e55 6e69   = traitlets.Uni
+000008d0: 6f6e 285b 7472 6169 746c 6574 732e 496e  on([traitlets.In
+000008e0: 7428 292c 2074 7261 6974 6c65 7473 2e55  t(), traitlets.U
+000008f0: 6e69 636f 6465 2829 5d2c 2061 6c6c 6f77  nicode()], allow
+00000900: 5f6e 6f6e 653d 5472 7565 290a 0a20 2020  _none=True)..   
+00000910: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
+00000920: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
+00000930: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00000940: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00000950: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00000960: 7220 6b2c 2077 2069 6e20 6b77 6172 6773  r k, w in kwargs
+00000970: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00000980: 2020 2020 2020 2020 2020 7365 7461 7474            setatt
+00000990: 7228 7365 6c66 2c20 6b2c 2077 290a 0a20  r(self, k, w).. 
+000009a0: 2020 2020 2020 2064 6566 205f 5f72 6570         def __rep
+000009b0: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
+000009c0: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+000009d0: 7b74 7970 6528 7365 6c66 292e 5f5f 6e61  {type(self).__na
+000009e0: 6d65 5f5f 7d3a 2861 3d7b 7365 6c66 2e61  me__}:(a={self.a
+000009f0: 7d2c 2062 3d7b 7365 6c66 2e62 7d2c 2063  }, b={self.b}, c
+00000a00: 3d7b 7365 6c66 2e63 7d29 220a 0a20 2020  ={self.c})"..   
+00000a10: 2020 2020 2064 6566 205f 5f64 6972 5f5f       def __dir__
+00000a20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00000a30: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000a40: 7472 6169 745f 6e61 6d65 7328 290a 0a44  trait_names()..D
+00000a50: 6174 6154 7570 6c65 203d 206e 616d 6564  ataTuple = named
+00000a60: 7475 706c 6528 2244 6174 6154 7570 6c65  tuple("DataTuple
+00000a70: 222c 2022 6120 6220 6322 290a 0a0a 636c  ", "a b c")...cl
+00000a80: 6173 7320 5479 7069 6e67 4e61 6d65 6454  ass TypingNamedT
+00000a90: 7570 6c65 2874 7970 696e 672e 4e61 6d65  uple(typing.Name
+00000aa0: 6454 7570 6c65 293a 0a20 2020 2061 3a20  dTuple):.    a: 
+00000ab0: 696e 740a 2020 2020 623a 2069 6e74 0a20  int.    b: int. 
+00000ac0: 2020 2063 3a20 696e 740a 0a0a 2320 6966     c: int...# if
+00000ad0: 2072 6963 6820 6973 206e 6f74 2069 6e73   rich is not ins
+00000ae0: 7461 6c6c 6564 2c20 6469 7361 626c 6520  talled, disable 
+00000af0: 7461 626c 652e 7072 6573 656e 7428 2920  table.present() 
+00000b00: 6361 6c6c 730a 7472 793a 0a20 2020 2069  calls.try:.    i
+00000b10: 6d70 6f72 7420 7269 6368 0a65 7863 6570  mport rich.excep
+00000b20: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+00000b30: 2020 2072 6963 6820 3d20 4e6f 6e65 0a20     rich = None. 
+00000b40: 2020 2023 2064 6973 6162 6c65 2070 7265     # disable pre
+00000b50: 7365 6e74 2829 206d 6574 686f 642c 2073  sent() method, s
+00000b60: 696e 6365 2072 6963 6820 6973 206e 6f74  ince rich is not
+00000b70: 2061 7661 696c 6162 6c65 0a20 2020 206c   available.    l
+00000b80: 742e 5461 626c 652e 7072 6573 656e 7420  t.Table.present 
+00000b90: 3d20 6c61 6d62 6461 202a 6172 6773 2c20  = lambda *args, 
+00000ba0: 2a2a 6b77 6172 6773 3a20 4e6f 6e65 0a0a  **kwargs: None..
+00000bb0: 0a63 6c61 7373 2053 6c6f 7474 6564 3a0a  .class Slotted:.
+00000bc0: 2020 2020 5f5f 736c 6f74 735f 5f20 3d20      __slots__ = 
+00000bd0: 5b27 6127 2c20 2762 272c 2027 6327 5d0a  ['a', 'b', 'c'].
+00000be0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00000bf0: 5f28 7365 6c66 2c20 612c 2062 2c20 6329  _(self, a, b, c)
+00000c00: 3a0a 2020 2020 2020 2020 7365 6c66 2e61  :.        self.a
+00000c10: 203d 2061 0a20 2020 2020 2020 2073 656c   = a.        sel
+00000c20: 662e 6220 3d20 620a 2020 2020 2020 2020  f.b = b.        
+00000c30: 7365 6c66 2e63 203d 2063 0a0a 2020 2020  self.c = c..    
+00000c40: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
+00000c50: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00000c60: 2072 6574 7572 6e20 2869 7369 6e73 7461   return (isinsta
+00000c70: 6e63 6528 6f74 6865 722c 2053 6c6f 7474  nce(other, Slott
+00000c80: 6564 2920 616e 640a 2020 2020 2020 2020  ed) and.        
+00000c90: 2020 2020 2020 2020 616c 6c28 6765 7461          all(geta
+00000ca0: 7474 7228 7365 6c66 2c20 6174 7472 2920  ttr(self, attr) 
+00000cb0: 3d3d 2067 6574 6174 7472 286f 7468 6572  == getattr(other
+00000cc0: 2c20 6174 7472 2920 666f 7220 6174 7472  , attr) for attr
+00000cd0: 2069 6e20 7365 6c66 2e5f 5f73 6c6f 7473   in self.__slots
+00000ce0: 5f5f 2929 0a0a 2020 2020 6465 6620 5f5f  __))..    def __
+00000cf0: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00000d00: 2020 2020 2020 7265 7475 726e 2066 227b        return f"{
+00000d10: 7479 7065 2873 656c 6629 2e5f 5f6e 616d  type(self).__nam
+00000d20: 655f 5f7d 3a28 613d 7b73 656c 662e 617d  e__}:(a={self.a}
+00000d30: 2c20 623d 7b73 656c 662e 627d 2c20 633d  , b={self.b}, c=
+00000d40: 7b73 656c 662e 637d 2922 0a0a 0a63 6c61  {self.c})"...cla
+00000d50: 7373 2053 6c6f 7474 6564 5769 7468 4469  ss SlottedWithDi
+00000d60: 6374 3a0a 2020 2020 5f5f 736c 6f74 735f  ct:.    __slots_
+00000d70: 5f20 3d20 7b27 6127 3a20 2761 272c 2027  _ = {'a': 'a', '
+00000d80: 6227 3a20 2762 272c 2027 6327 3a20 2763  b': 'b', 'c': 'c
+00000d90: 277d 0a0a 2020 2020 6465 6620 5f5f 696e  '}..    def __in
+00000da0: 6974 5f5f 2873 656c 662c 2061 2c20 622c  it__(self, a, b,
+00000db0: 2063 293a 0a20 2020 2020 2020 2073 656c   c):.        sel
+00000dc0: 662e 6120 3d20 610a 2020 2020 2020 2020  f.a = a.        
+00000dd0: 7365 6c66 2e62 203d 2062 0a20 2020 2020  self.b = b.     
+00000de0: 2020 2073 656c 662e 6320 3d20 630a 0a20     self.c = c.. 
+00000df0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
+00000e00: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+00000e10: 2020 2020 7265 7475 726e 2028 6973 696e      return (isin
+00000e20: 7374 616e 6365 286f 7468 6572 2c20 536c  stance(other, Sl
+00000e30: 6f74 7465 6457 6974 6844 6963 7429 2061  ottedWithDict) a
+00000e40: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00000e50: 2020 2061 6c6c 2867 6574 6174 7472 2873     all(getattr(s
+00000e60: 656c 662c 2061 7474 7229 203d 3d20 6765  elf, attr) == ge
+00000e70: 7461 7474 7228 6f74 6865 722c 2061 7474  tattr(other, att
+00000e80: 7229 2066 6f72 2061 7474 7220 696e 2073  r) for attr in s
+00000e90: 656c 662e 5f5f 736c 6f74 735f 5f29 290a  elf.__slots__)).
+00000ea0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+00000eb0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00000ec0: 2072 6574 7572 6e20 6622 7b74 7970 6528   return f"{type(
+00000ed0: 7365 6c66 292e 5f5f 6e61 6d65 5f5f 7d3a  self).__name__}:
+00000ee0: 2861 3d7b 7365 6c66 2e61 7d2c 2062 3d7b  (a={self.a}, b={
+00000ef0: 7365 6c66 2e62 7d2c 2063 3d7b 7365 6c66  self.b}, c={self
+00000f00: 2e63 7d29 220a 0a0a 636c 6173 7320 5479  .c})"...class Ty
+00000f10: 7069 6e67 5479 7065 6444 6963 7428 7479  pingTypedDict(ty
+00000f20: 7069 6e67 2e54 7970 6564 4469 6374 293a  ping.TypedDict):
+00000f30: 0a20 2020 2061 3a20 696e 740a 2020 2020  .    a: int.    
+00000f40: 623a 2069 6e74 0a20 2020 2063 3a20 696e  b: int.    c: in
+00000f50: 740a 0a0a 636c 6173 7320 5465 7374 4461  t...class TestDa
+00000f60: 7461 4f62 6a65 6374 7328 756e 6974 7465  taObjects(unitte
+00000f70: 7374 2e54 6573 7443 6173 6529 3a0a 2020  st.TestCase):.  
+00000f80: 2020 6465 6620 7465 7374 5f73 6574 5f61    def test_set_a
+00000f90: 7474 7269 6275 7465 7328 7365 6c66 293a  ttributes(self):
+00000fa0: 0a20 2020 2020 2020 206f 6220 3d20 6c74  .        ob = lt
+00000fb0: 2e44 6174 614f 626a 6563 7428 290a 2020  .DataObject().  
+00000fc0: 2020 2020 2020 6f62 2e7a 203d 2032 3030        ob.z = 200
+00000fd0: 0a20 2020 2020 2020 206f 622e 6120 3d20  .        ob.a = 
+00000fe0: 3130 300a 2020 2020 2020 2020 7769 7468  100.        with
+00000ff0: 2073 656c 662e 7375 6254 6573 7428 2274   self.subTest("t
+00001000: 6573 7420 4461 7461 4f62 6a65 6374 2061  est DataObject a
+00001010: 7474 7269 6275 7465 2073 6574 7469 6e67  ttribute setting
+00001020: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00001030: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00001040: 285b 2827 6127 2c20 3130 3029 2c20 2827  ([('a', 100), ('
+00001050: 7a27 2c20 3230 3029 5d2c 2073 6f72 7465  z', 200)], sorte
+00001060: 6428 6f62 2e5f 5f64 6963 745f 5f2e 6974  d(ob.__dict__.it
+00001070: 656d 7328 2929 290a 0a20 2020 2020 2020  ems()))..       
+00001080: 2023 2074 6573 7420 7365 6d69 2d69 6d6d   # test semi-imm
+00001090: 7574 6162 696c 6974 7920 2863 616e 2774  utability (can't
+000010a0: 206f 7665 7277 7269 7465 2065 7869 7374   overwrite exist
+000010b0: 696e 6720 6174 7472 6962 7574 6573 290a  ing attributes).
+000010c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000010d0: 662e 7375 6254 6573 7428 2274 6573 7420  f.subTest("test 
+000010e0: 4461 7461 4f62 6a65 6374 2077 7269 7465  DataObject write
+000010f0: 2d6f 6e63 6520 2873 656d 692d 696d 6d75  -once (semi-immu
+00001100: 7461 6269 6c69 7479 2922 293a 0a20 2020  tability)"):.   
+00001110: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00001120: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+00001130: 4174 7472 6962 7574 6545 7272 6f72 293a  AttributeError):
+00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001150: 206f 622e 6120 3d20 3130 310a 0a20 2020   ob.a = 101..   
+00001160: 2020 2020 2023 2065 7175 616c 6974 7920       # equality 
+00001170: 7465 7374 730a 2020 2020 2020 2020 7769  tests.        wi
+00001180: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00001190: 2274 6573 7420 4461 7461 4f62 6a65 6374  "test DataObject
+000011a0: 2065 7175 616c 6974 7922 293a 0a20 2020   equality"):.   
+000011b0: 2020 2020 2020 2020 206f 6232 203d 206c           ob2 = l
+000011c0: 742e 4461 7461 4f62 6a65 6374 282a 2a7b  t.DataObject(**{
+000011d0: 2761 273a 2031 3030 2c20 277a 273a 2032  'a': 100, 'z': 2
+000011e0: 3030 7d29 0a20 2020 2020 2020 2020 2020  00}).           
+000011f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00001200: 6c28 6f62 322c 206f 6229 0a0a 2020 2020  l(ob2, ob)..    
+00001210: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00001220: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
+00001230: 4f62 6a65 6374 2069 6e65 7175 616c 6974  Object inequalit
+00001240: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
+00001250: 206f 6232 2e62 203d 2027 626c 6168 270a   ob2.b = 'blah'.
+00001260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001270: 2e61 7373 6572 744e 6f74 4571 7561 6c28  .assertNotEqual(
+00001280: 6f62 2c20 6f62 3229 0a0a 2020 2020 2020  ob, ob2)..      
+00001290: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+000012a0: 6573 7428 2274 6573 7420 4461 7461 4f62  est("test DataOb
+000012b0: 6a65 6374 2065 7175 616c 6974 7920 6166  ject equality af
+000012c0: 7465 7220 7570 6461 7465 7322 293a 0a20  ter updates"):. 
+000012d0: 2020 2020 2020 2020 2020 2064 656c 206f             del o
+000012e0: 6232 2e62 0a20 2020 2020 2020 2020 2020  b2.b.           
+000012f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00001300: 6c28 6f62 322c 206f 6229 0a0a 2020 2020  l(ob2, ob)..    
+00001310: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00001320: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
+00001330: 4f62 6a65 6374 204b 6579 4572 726f 7222  Object KeyError"
+00001340: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00001350: 656c 206f 6232 2e61 0a20 2020 2020 2020  el ob2.a.       
+00001360: 2020 2020 2064 656c 206f 6232 2e7a 0a0a       del ob2.z..
+00001370: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00001380: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00001390: 6573 284b 6579 4572 726f 7229 3a0a 2020  es(KeyError):.  
+000013a0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+000013b0: 325b 2761 275d 0a20 2020 2020 2020 2020  2['a'].         
+000013c0: 2020 206f 6232 5b27 6127 5d20 3d20 3130     ob2['a'] = 10
+000013d0: 0a20 2020 2020 2020 2020 2020 206f 6232  .            ob2
+000013e0: 5b27 6127 5d0a 0a20 2020 2020 2020 2077  ['a']..        w
+000013f0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00001400: 2822 7465 7374 2044 6174 614f 626a 6563  ("test DataObjec
+00001410: 7420 4b65 7945 7272 6f72 2028 3229 2229  t KeyError (2)")
+00001420: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00001430: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+00001440: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
+00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001460: 6f62 325b 2761 275d 203d 2031 300a 0a20  ob2['a'] = 10.. 
+00001470: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00001480: 2e73 7562 5465 7374 2822 7465 7374 2044  .subTest("test D
+00001490: 6174 614f 626a 6563 7420 7265 7072 2229  ataObject repr")
+000014a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000014b0: 6c66 2e61 7373 6572 7445 7175 616c 2822  lf.assertEqual("
+000014c0: 7b27 6127 3a20 3130 7d22 2c20 7265 7072  {'a': 10}", repr
+000014d0: 286f 6232 2929 0a0a 0a63 6c61 7373 2054  (ob2))...class T
+000014e0: 6573 7454 6162 6c65 5479 7065 7328 756e  estTableTypes(un
+000014f0: 6974 7465 7374 2e54 6573 7443 6173 6529  ittest.TestCase)
+00001500: 3a0a 2020 2020 6465 6620 7465 7374 5f74  :.    def test_t
+00001510: 7970 6573 2873 656c 6629 3a0a 0a20 2020  ypes(self):..   
+00001520: 2020 2020 2023 2063 6865 636b 2074 6861       # check tha
+00001530: 7420 5461 626c 6520 616e 6420 496e 6465  t Table and Inde
+00001540: 7820 6172 6520 7265 636f 676e 697a 6564  x are recognized
+00001550: 2061 7320 5365 7175 656e 6365 2061 6e64   as Sequence and
+00001560: 204d 6170 7069 6e67 2074 7970 6573 0a20   Mapping types. 
+00001570: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00001580: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
+00001590: 7468 6174 2054 6162 6c65 2069 7320 7265  that Table is re
+000015a0: 636f 676e 697a 6564 2061 7320 5365 7175  cognized as Sequ
+000015b0: 656e 6365 2074 7970 6522 293a 0a20 2020  ence type"):.   
+000015c0: 2020 2020 2020 2020 2074 203d 206c 742e           t = lt.
+000015d0: 5461 626c 6528 290a 2020 2020 2020 2020  Table().        
+000015e0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000015f0: 7275 6528 6973 696e 7374 616e 6365 2874  rue(isinstance(t
+00001600: 2c20 6c74 2e53 6571 7565 6e63 6529 290a  , lt.Sequence)).
+00001610: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00001620: 6c66 2e73 7562 5465 7374 2822 6368 6563  lf.subTest("chec
+00001630: 6b20 7468 6174 2049 6e64 6578 2069 7320  k that Index is 
+00001640: 7265 636f 676e 697a 6564 2061 7320 4d61  recognized as Ma
+00001650: 7070 696e 6720 7479 7065 2229 3a0a 2020  pping type"):.  
+00001660: 2020 2020 2020 2020 2020 742e 6372 6561            t.crea
+00001670: 7465 5f69 6e64 6578 2822 7822 290a 2020  te_index("x").  
+00001680: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00001690: 7373 6572 7454 7275 6528 6973 696e 7374  ssertTrue(isinst
+000016a0: 616e 6365 2874 2e67 6574 5f69 6e64 6578  ance(t.get_index
+000016b0: 2827 7827 292c 206c 742e 4d61 7070 696e  ('x'), lt.Mappin
+000016c0: 6729 290a 0a20 2020 2020 2020 2023 206d  g))..        # m
+000016d0: 616b 6520 7375 7265 2067 6574 5f69 6e64  ake sure get_ind
+000016e0: 6578 2072 6574 7572 6e73 2061 2072 6561  ex returns a rea
+000016f0: 642d 6f6e 6c79 2061 6363 6573 7320 746f  d-only access to
+00001700: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+00001710: 696e 6465 780a 2020 2020 2020 2020 7769  index.        wi
+00001720: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00001730: 2263 6865 636b 2074 6861 7420 6765 745f  "check that get_
+00001740: 696e 6465 7820 7265 7475 726e 7320 6120  index returns a 
+00001750: 7265 6164 2d6f 6e6c 7920 6163 6365 7373  read-only access
+00001760: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
+00001770: 6e67 2069 6e64 6578 2229 3a0a 2020 2020  ng index"):.    
+00001780: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00001790: 662e 6173 7365 7274 5261 6973 6573 286c  f.assertRaises(l
+000017a0: 742e 5265 6164 6f6e 6c79 496e 6465 7841  t.ReadonlyIndexA
+000017b0: 6363 6573 7345 7272 6f72 293a 0a20 2020  ccessError):.   
+000017c0: 2020 2020 2020 2020 2020 2020 2074 2e67               t.g
+000017d0: 6574 5f69 6e64 6578 2822 7822 295b 2761  et_index("x")['a
+000017e0: 275d 203d 2031 3030 0a0a 0a64 6566 2061  '] = 100...def a
+000017f0: 6e6e 6f75 6e63 655f 7465 7374 2866 6e29  nnounce_test(fn)
+00001800: 3a0a 2020 2020 6465 6620 5f69 6e6e 6572  :.    def _inner
+00001810: 282a 6172 6773 293a 0a20 2020 2020 2020  (*args):.       
+00001820: 2070 7269 6e74 2822 5c6e 2220 2b20 222d   print("\n" + "-
+00001830: 2220 2a20 3530 290a 2020 2020 2020 2020  " * 50).        
+00001840: 7072 696e 7428 6622 7b74 7970 6528 6172  print(f"{type(ar
+00001850: 6773 5b30 5d29 2e5f 5f6e 616d 655f 5f7d  gs[0]).__name__}
+00001860: 2e7b 666e 2e5f 5f6e 616d 655f 5f7d 2229  .{fn.__name__}")
+00001870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001880: 666e 282a 6172 6773 290a 0a20 2020 2072  fn(*args)..    r
+00001890: 6574 7572 6e20 5f69 6e6e 6572 0a0a 0a64  eturn _inner...d
+000018a0: 6566 206d 616b 655f 7465 7374 5f63 6c61  ef make_test_cla
+000018b0: 7373 282a 636c 6173 7365 7329 3a0a 0a20  ss(*classes):.. 
+000018c0: 2020 2063 6c61 7373 5f6e 616d 6520 3d20     class_name = 
+000018d0: 225f 222e 6a6f 696e 2863 2e5f 5f6e 616d  "_".join(c.__nam
+000018e0: 655f 5f20 666f 7220 6320 696e 2063 6c61  e__ for c in cla
+000018f0: 7373 6573 290a 2020 2020 6966 206e 6f74  sses).    if not
+00001900: 2069 7373 7562 636c 6173 7328 636c 6173   issubclass(clas
+00001910: 7365 735b 305d 2c20 756e 6974 7465 7374  ses[0], unittest
+00001920: 2e54 6573 7443 6173 6529 3a0a 2020 2020  .TestCase):.    
+00001930: 2020 2020 636c 7320 3d20 7479 7065 2863      cls = type(c
+00001940: 6c61 7373 5f6e 616d 652c 2028 756e 6974  lass_name, (unit
+00001950: 7465 7374 2e54 6573 7443 6173 652c 202a  test.TestCase, *
+00001960: 636c 6173 7365 7329 2c20 7b7d 290a 2020  classes), {}).  
+00001970: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001980: 636c 7320 3d20 7479 7065 2863 6c61 7373  cls = type(class
+00001990: 5f6e 616d 652c 2074 7570 6c65 2863 6c61  _name, tuple(cla
+000019a0: 7373 6573 292c 207b 7d29 0a20 2020 2066  sses), {}).    f
+000019b0: 6f72 2061 7474 7220 696e 2064 6972 2863  or attr in dir(c
+000019c0: 6c73 293a 0a20 2020 2020 2020 2061 7474  ls):.        att
+000019d0: 7276 616c 7565 203d 2067 6574 6174 7472  rvalue = getattr
+000019e0: 2863 6c73 2c20 6174 7472 290a 2020 2020  (cls, attr).    
+000019f0: 2020 2020 6966 2061 7474 722e 7374 6172      if attr.star
+00001a00: 7473 7769 7468 2822 7465 7374 5f22 2920  tswith("test_") 
+00001a10: 616e 6420 6361 6c6c 6162 6c65 2861 7474  and callable(att
+00001a20: 7276 616c 7565 293a 0a20 2020 2020 2020  rvalue):.       
+00001a30: 2020 2020 2073 6574 6174 7472 2863 6c73       setattr(cls
+00001a40: 2c20 6174 7472 2c20 616e 6e6f 756e 6365  , attr, announce
+00001a50: 5f74 6573 7428 6174 7472 7661 6c75 6529  _test(attrvalue)
+00001a60: 290a 2020 2020 676c 6f62 616c 7328 295b  ).    globals()[
+00001a70: 636c 732e 5f5f 6e61 6d65 5f5f 5d20 3d20  cls.__name__] = 
+00001a80: 636c 730a 0a0a 6465 6620 6d61 6b65 5f74  cls...def make_t
+00001a90: 6573 745f 636c 6173 7365 7328 636c 7329  est_classes(cls)
+00001aa0: 3a0a 2020 2020 6d61 6b65 5f74 6573 745f  :.    make_test_
+00001ab0: 636c 6173 7328 636c 732c 2055 7369 6e67  class(cls, Using
+00001ac0: 4461 7461 4f62 6a65 6374 7329 0a20 2020  DataObjects).   
+00001ad0: 206d 616b 655f 7465 7374 5f63 6c61 7373   make_test_class
+00001ae0: 2863 6c73 2c20 5573 696e 674e 616d 6564  (cls, UsingNamed
+00001af0: 7475 706c 6573 290a 2020 2020 6d61 6b65  tuples).    make
+00001b00: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
+00001b10: 2055 7369 6e67 5479 7069 6e67 4e61 6d65   UsingTypingName
+00001b20: 6454 7570 6c65 290a 2020 2020 6d61 6b65  dTuple).    make
+00001b30: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
+00001b40: 2055 7369 6e67 536c 6f74 7465 644f 626a   UsingSlottedObj
+00001b50: 6563 7473 290a 2020 2020 6966 2053 6c6f  ects).    if Slo
+00001b60: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
+00001b70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00001b80: 2020 6d61 6b65 5f74 6573 745f 636c 6173    make_test_clas
+00001b90: 7328 636c 732c 2055 7369 6e67 536c 6f74  s(cls, UsingSlot
+00001ba0: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
+00001bb0: 7473 290a 2020 2020 6d61 6b65 5f74 6573  ts).    make_tes
+00001bc0: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
+00001bd0: 6e67 5369 6d70 6c65 4e61 6d65 7370 6163  ngSimpleNamespac
+00001be0: 6529 0a20 2020 2069 6620 6461 7461 636c  e).    if datacl
+00001bf0: 6173 7365 7320 6973 206e 6f74 204e 6f6e  asses is not Non
+00001c00: 653a 0a20 2020 2020 2020 206d 616b 655f  e:.        make_
+00001c10: 7465 7374 5f63 6c61 7373 2863 6c73 2c20  test_class(cls, 
+00001c20: 5573 696e 6744 6174 6163 6c61 7373 6573  UsingDataclasses
+00001c30: 290a 2020 2020 6966 2070 7964 616e 7469  ).    if pydanti
+00001c40: 6320 6973 206e 6f74 204e 6f6e 653a 0a20  c is not None:. 
+00001c50: 2020 2020 2020 206d 616b 655f 7465 7374         make_test
+00001c60: 5f63 6c61 7373 2863 6c73 2c20 5573 696e  _class(cls, Usin
+00001c70: 6750 7964 616e 7469 634d 6f64 656c 290a  gPydanticModel).
+00001c80: 2020 2020 2020 2020 6d61 6b65 5f74 6573          make_tes
+00001c90: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
+00001ca0: 6e67 5079 6461 6e74 6963 496d 6d75 7461  ngPydanticImmuta
+00001cb0: 626c 654d 6f64 656c 290a 2020 2020 2020  bleModel).      
+00001cc0: 2020 6d61 6b65 5f74 6573 745f 636c 6173    make_test_clas
+00001cd0: 7328 636c 732c 2055 7369 6e67 5079 6461  s(cls, UsingPyda
+00001ce0: 6e74 6963 4f52 4d4d 6f64 656c 290a 2020  nticORMModel).  
+00001cf0: 2020 6966 2061 7474 7220 6973 206e 6f74    if attr is not
+00001d00: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
+00001d10: 616b 655f 7465 7374 5f63 6c61 7373 2863  ake_test_class(c
+00001d20: 6c73 2c20 5573 696e 6741 7474 7243 6c61  ls, UsingAttrCla
+00001d30: 7373 290a 2020 2020 6966 2074 7261 6974  ss).    if trait
+00001d40: 6c65 7473 2069 7320 6e6f 7420 4e6f 6e65  lets is not None
+00001d50: 3a0a 2020 2020 2020 2020 6d61 6b65 5f74  :.        make_t
+00001d60: 6573 745f 636c 6173 7328 636c 732c 2055  est_class(cls, U
+00001d70: 7369 6e67 5472 6169 746c 6574 7343 6c61  singTraitletsCla
+00001d80: 7373 290a 2020 2020 6d61 6b65 5f74 6573  ss).    make_tes
+00001d90: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
+00001da0: 6e67 5479 7069 6e67 5479 7065 6444 6963  ngTypingTypedDic
+00001db0: 7429 0a0a 0a63 6c61 7373 2041 6273 7472  t)...class Abstr
+00001dc0: 6163 7443 6f6e 7465 6e74 5479 7065 4661  actContentTypeFa
+00001dd0: 6374 6f72 793a 0a20 2020 2064 6174 615f  ctory:.    data_
+00001de0: 6f62 6a65 6374 5f74 7970 653a 204f 7074  object_type: Opt
+00001df0: 696f 6e61 6c5b 7479 7065 5d20 3d20 4e6f  ional[type] = No
+00001e00: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
+00001e10: 7468 6f64 0a20 2020 2064 6566 206d 616b  thod.    def mak
+00001e20: 655f 6461 7461 5f6f 626a 6563 7428 636c  e_data_object(cl
+00001e30: 732c 2061 2c20 622c 2063 293a 0a20 2020  s, a, b, c):.   
+00001e40: 2020 2020 2072 6574 7572 6e20 636c 732e       return cls.
+00001e50: 6461 7461 5f6f 626a 6563 745f 7479 7065  data_object_type
+00001e60: 2861 3d61 2c20 623d 622c 2063 3d63 290a  (a=a, b=b, c=c).
+00001e70: 0a0a 636c 6173 7320 5573 696e 6744 6174  ..class UsingDat
+00001e80: 614f 626a 6563 7473 2841 6273 7472 6163  aObjects(Abstrac
+00001e90: 7443 6f6e 7465 6e74 5479 7065 4661 6374  tContentTypeFact
+00001ea0: 6f72 7929 3a0a 2020 2020 6461 7461 5f6f  ory):.    data_o
+00001eb0: 626a 6563 745f 7479 7065 203d 206c 742e  bject_type = lt.
+00001ec0: 4461 7461 4f62 6a65 6374 0a0a 0a63 6c61  DataObject...cla
+00001ed0: 7373 2055 7369 6e67 4e61 6d65 6474 7570  ss UsingNamedtup
+00001ee0: 6c65 7328 4162 7374 7261 6374 436f 6e74  les(AbstractCont
+00001ef0: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
+00001f00: 0a20 2020 2064 6174 615f 6f62 6a65 6374  .    data_object
+00001f10: 5f74 7970 6520 3d20 4461 7461 5475 706c  _type = DataTupl
+00001f20: 650a 0a0a 636c 6173 7320 5573 696e 6753  e...class UsingS
+00001f30: 6c6f 7474 6564 4f62 6a65 6374 7328 4162  lottedObjects(Ab
+00001f40: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
+00001f50: 6546 6163 746f 7279 293a 0a20 2020 2064  eFactory):.    d
+00001f60: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
+00001f70: 3d20 536c 6f74 7465 640a 0a0a 6966 2053  = Slotted...if S
+00001f80: 6c6f 7474 6564 5769 7468 4469 6374 2069  lottedWithDict i
+00001f90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00001fa0: 636c 6173 7320 5573 696e 6753 6c6f 7474  class UsingSlott
+00001fb0: 6564 5769 7468 4469 6374 4f62 6a65 6374  edWithDictObject
+00001fc0: 7328 4162 7374 7261 6374 436f 6e74 656e  s(AbstractConten
+00001fd0: 7454 7970 6546 6163 746f 7279 293a 0a20  tTypeFactory):. 
+00001fe0: 2020 2020 2020 2064 6174 615f 6f62 6a65         data_obje
+00001ff0: 6374 5f74 7970 6520 3d20 536c 6f74 7465  ct_type = Slotte
+00002000: 6457 6974 6844 6963 740a 656c 7365 3a0a  dWithDict.else:.
+00002010: 2020 2020 5573 696e 6753 6c6f 7474 6564      UsingSlotted
+00002020: 5769 7468 4469 6374 4f62 6a65 6374 7320  WithDictObjects 
+00002030: 3d20 4162 7374 7261 6374 436f 6e74 656e  = AbstractConten
+00002040: 7454 7970 6546 6163 746f 7279 0a0a 0a63  tTypeFactory...c
+00002050: 6c61 7373 2055 7369 6e67 5369 6d70 6c65  lass UsingSimple
+00002060: 4e61 6d65 7370 6163 6528 4162 7374 7261  Namespace(Abstra
+00002070: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
+00002080: 746f 7279 293a 0a20 2020 2064 6174 615f  tory):.    data_
+00002090: 6f62 6a65 6374 5f74 7970 6520 3d20 5369  object_type = Si
+000020a0: 6d70 6c65 4e61 6d65 7370 6163 650a 0a0a  mpleNamespace...
+000020b0: 6966 2064 6174 6163 6c61 7373 6573 2069  if dataclasses i
+000020c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000020d0: 636c 6173 7320 5573 696e 6744 6174 6163  class UsingDatac
+000020e0: 6c61 7373 6573 2841 6273 7472 6163 7443  lasses(AbstractC
+000020f0: 6f6e 7465 6e74 5479 7065 4661 6374 6f72  ontentTypeFactor
+00002100: 7929 3a0a 2020 2020 2020 2020 6461 7461  y):.        data
+00002110: 5f6f 626a 6563 745f 7479 7065 203d 2044  _object_type = D
+00002120: 6174 6144 6174 6163 6c61 7373 0a65 6c73  ataDataclass.els
+00002130: 653a 0a20 2020 2055 7369 6e67 4461 7461  e:.    UsingData
+00002140: 636c 6173 7365 7320 3d20 4162 7374 7261  classes = Abstra
+00002150: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
+00002160: 746f 7279 0a0a 0a69 6620 7079 6461 6e74  tory...if pydant
+00002170: 6963 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ic is not None:.
+00002180: 2020 2020 636c 6173 7320 5573 696e 6750      class UsingP
+00002190: 7964 616e 7469 634d 6f64 656c 2841 6273  ydanticModel(Abs
+000021a0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
+000021b0: 4661 6374 6f72 7929 3a0a 2020 2020 2020  Factory):.      
+000021c0: 2020 6461 7461 5f6f 626a 6563 745f 7479    data_object_ty
+000021d0: 7065 203d 2044 6174 6150 7964 616e 7469  pe = DataPydanti
+000021e0: 634d 6f64 656c 0a0a 2020 2020 636c 6173  cModel..    clas
+000021f0: 7320 5573 696e 6750 7964 616e 7469 6349  s UsingPydanticI
+00002200: 6d6d 7574 6162 6c65 4d6f 6465 6c28 4162  mmutableModel(Ab
+00002210: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
+00002220: 6546 6163 746f 7279 293a 0a20 2020 2020  eFactory):.     
+00002230: 2020 2064 6174 615f 6f62 6a65 6374 5f74     data_object_t
+00002240: 7970 6520 3d20 4461 7461 5079 6461 6e74  ype = DataPydant
+00002250: 6963 496d 6d75 7461 626c 654d 6f64 656c  icImmutableModel
+00002260: 0a0a 2020 2020 636c 6173 7320 5573 696e  ..    class Usin
+00002270: 6750 7964 616e 7469 634f 524d 4d6f 6465  gPydanticORMMode
+00002280: 6c28 4162 7374 7261 6374 436f 6e74 656e  l(AbstractConten
+00002290: 7454 7970 6546 6163 746f 7279 293a 0a20  tTypeFactory):. 
+000022a0: 2020 2020 2020 2064 6174 615f 6f62 6a65         data_obje
+000022b0: 6374 5f74 7970 6520 3d20 4461 7461 5079  ct_type = DataPy
+000022c0: 6461 6e74 6963 4f52 4d4d 6f64 656c 0a0a  danticORMModel..
+000022d0: 656c 7365 3a0a 2020 2020 5573 696e 6750  else:.    UsingP
+000022e0: 7964 616e 7469 634d 6f64 656c 203d 2041  ydanticModel = A
 000022f0: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
-00002300: 7065 4661 6374 6f72 7929 3a0a 2020 2020  peFactory):.    
-00002310: 2020 2020 6461 7461 5f6f 626a 6563 745f      data_object_
-00002320: 7479 7065 203d 2041 7474 7243 6c61 7373  type = AttrClass
-00002330: 0a65 6c73 653a 0a20 2020 2055 7369 6e67  .else:.    Using
-00002340: 4174 7472 436c 6173 7320 3d20 4162 7374  AttrClass = Abst
-00002350: 7261 6374 436f 6e74 656e 7454 7970 6546  ractContentTypeF
-00002360: 6163 746f 7279 0a0a 6966 2074 7261 6974  actory..if trait
-00002370: 6c65 7473 2069 7320 6e6f 7420 4e6f 6e65  lets is not None
-00002380: 3a0a 2020 2020 636c 6173 7320 5573 696e  :.    class Usin
-00002390: 6754 7261 6974 6c65 7473 436c 6173 7328  gTraitletsClass(
-000023a0: 4162 7374 7261 6374 436f 6e74 656e 7454  AbstractContentT
-000023b0: 7970 6546 6163 746f 7279 293a 0a20 2020  ypeFactory):.   
-000023c0: 2020 2020 2064 6174 615f 6f62 6a65 6374       data_object
-000023d0: 5f74 7970 6520 3d20 5472 6169 746c 6574  _type = Traitlet
-000023e0: 7343 6c61 7373 0a65 6c73 653a 0a20 2020  sClass.else:.   
-000023f0: 2055 7369 6e67 5472 6169 746c 6574 7343   UsingTraitletsC
-00002400: 6c61 7373 203d 2041 6273 7472 6163 7443  lass = AbstractC
-00002410: 6f6e 7465 6e74 5479 7065 4661 6374 6f72  ontentTypeFactor
-00002420: 790a 0a0a 6465 6620 6c6f 6164 5f74 6162  y...def load_tab
-00002430: 6c65 2874 6162 6c65 2c20 7265 635f 6661  le(table, rec_fa
-00002440: 6374 6f72 795f 666e 2c20 7461 626c 655f  ctory_fn, table_
-00002450: 7369 7a65 293a 0a20 2020 2074 6573 745f  size):.    test_
-00002460: 7369 7a65 203d 2074 6162 6c65 5f73 697a  size = table_siz
-00002470: 650a 2020 2020 666f 7220 6161 2c20 6262  e.    for aa, bb
-00002480: 2c20 6363 2069 6e20 6974 6572 746f 6f6c  , cc in itertool
-00002490: 732e 7072 6f64 7563 7428 7261 6e67 6528  s.product(range(
-000024a0: 7465 7374 5f73 697a 6529 2c20 7265 7065  test_size), repe
-000024b0: 6174 3d33 293a 0a20 2020 2020 2020 2074  at=3):.        t
-000024c0: 6162 6c65 2e69 6e73 6572 7428 7265 635f  able.insert(rec_
-000024d0: 6661 6374 6f72 795f 666e 2861 612c 2062  factory_fn(aa, b
-000024e0: 622c 2063 6329 290a 0a0a 6465 6620 6d61  b, cc))...def ma
-000024f0: 6b65 5f74 6573 745f 7461 626c 6528 7265  ke_test_table(re
-00002500: 635f 6661 6374 6f72 795f 666e 2c20 7461  c_factory_fn, ta
-00002510: 626c 655f 7369 7a65 293a 0a20 2020 2074  ble_size):.    t
-00002520: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
-00002530: 290a 2020 2020 6c6f 6164 5f74 6162 6c65  ).    load_table
-00002540: 2874 6162 6c65 2c20 7265 635f 6661 6374  (table, rec_fact
-00002550: 6f72 795f 666e 2c20 7461 626c 655f 7369  ory_fn, table_si
-00002560: 7a65 290a 2020 2020 7265 7475 726e 2074  ze).    return t
-00002570: 6162 6c65 0a0a 0a64 6566 206d 616b 655f  able...def make_
-00002580: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
-00002590: 6f62 2872 6563 293a 0a20 2020 2072 6574  ob(rec):.    ret
-000025a0: 7572 6e20 6c74 2e44 6174 614f 626a 6563  urn lt.DataObjec
-000025b0: 7428 2a2a 7b6b 3a20 6765 7461 7474 7228  t(**{k: getattr(
-000025c0: 7265 632c 206b 2920 666f 7220 6b20 696e  rec, k) for k in
-000025d0: 206c 742e 5f6f 626a 6563 745f 6174 7472   lt._object_attr
-000025e0: 6e61 6d65 7328 7265 6329 7d29 0a0a 0a63  names(rec)})...c
-000025f0: 6c61 7373 2054 6162 6c65 5479 7065 5465  lass TableTypeTe
-00002600: 7374 7328 756e 6974 7465 7374 2e54 6573  sts(unittest.Tes
-00002610: 7443 6173 6529 3a0a 2020 2020 6465 6620  tCase):.    def 
-00002620: 7465 7374 5f74 7970 6573 2873 656c 6629  test_types(self)
-00002630: 3a0a 2020 2020 2020 2020 6672 6f6d 2063  :.        from c
-00002640: 6f6c 6c65 6374 696f 6e73 2e61 6263 2069  ollections.abc i
-00002650: 6d70 6f72 7420 2843 616c 6c61 626c 652c  mport (Callable,
-00002660: 2043 6f6e 7461 696e 6572 2c20 4974 6572   Container, Iter
-00002670: 6162 6c65 2c20 436f 6c6c 6563 7469 6f6e  able, Collection
-00002680: 2c20 4d61 7070 696e 672c 2052 6576 6572  , Mapping, Rever
-00002690: 7369 626c 652c 2053 6571 7565 6e63 652c  sible, Sequence,
-000026a0: 2053 697a 6564 290a 0a20 2020 2020 2020   Sized)..       
-000026b0: 2074 626c 203d 206c 742e 5461 626c 6528   tbl = lt.Table(
-000026c0: 290a 2020 2020 2020 2020 7462 6c2e 6372  ).        tbl.cr
-000026d0: 6561 7465 5f69 6e64 6578 2822 6964 7822  eate_index("idx"
-000026e0: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
-000026f0: 7570 6572 636c 6173 7320 696e 2028 4361  uperclass in (Ca
-00002700: 6c6c 6162 6c65 2c20 5369 7a65 642c 2049  llable, Sized, I
-00002710: 7465 7261 626c 652c 2043 6f6e 7461 696e  terable, Contain
-00002720: 6572 2c20 436f 6c6c 6563 7469 6f6e 2c20  er, Collection, 
-00002730: 5265 7665 7273 6962 6c65 2c20 5365 7175  Reversible, Sequ
-00002740: 656e 6365 293a 0a20 2020 2020 2020 2020  ence):.         
-00002750: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00002760: 5465 7374 2873 7570 6572 636c 6173 733d  Test(superclass=
-00002770: 7375 7065 7263 6c61 7373 293a 0a20 2020  superclass):.   
-00002780: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00002790: 6e74 2873 7570 6572 636c 6173 732e 5f5f  nt(superclass.__
-000027a0: 6e61 6d65 5f5f 290a 2020 2020 2020 2020  name__).        
-000027b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000027c0: 6572 7454 7275 6528 6973 696e 7374 616e  ertTrue(isinstan
-000027d0: 6365 2874 626c 2c20 7375 7065 7263 6c61  ce(tbl, supercla
-000027e0: 7373 2929 0a0a 2020 2020 2020 2020 7769  ss))..        wi
-000027f0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00002800: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-00002810: 7269 6e74 2822 6973 696e 7374 616e 6365  rint("isinstance
-00002820: 285f 4f62 6a49 6e64 6578 2c20 4d61 7070  (_ObjIndex, Mapp
-00002830: 696e 6729 2229 0a20 2020 2020 2020 2020  ing)").         
-00002840: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00002850: 7565 2869 7369 6e73 7461 6e63 6528 7462  ue(isinstance(tb
-00002860: 6c2e 5f69 6e64 6578 6573 5b22 6964 7822  l._indexes["idx"
-00002870: 5d2c 204d 6170 7069 6e67 2929 0a0a 2020  ], Mapping))..  
-00002880: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00002890: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-000028a0: 2020 2020 2020 2070 7269 6e74 2822 6973         print("is
-000028b0: 696e 7374 616e 6365 285f 4f62 6a49 6e64  instance(_ObjInd
-000028c0: 6578 5772 6170 7065 722c 204d 6170 7069  exWrapper, Mappi
-000028d0: 6e67 2922 290a 2020 2020 2020 2020 2020  ng)").          
-000028e0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-000028f0: 6528 6973 696e 7374 616e 6365 2874 626c  e(isinstance(tbl
-00002900: 2e62 792e 6964 782c 204d 6170 7069 6e67  .by.idx, Mapping
-00002910: 2929 0a0a 0a40 6d61 6b65 5f74 6573 745f  ))...@make_test_
-00002920: 636c 6173 7365 730a 636c 6173 7320 5461  classes.class Ta
-00002930: 626c 6543 7265 6174 6554 6573 7473 3a0a  bleCreateTests:.
-00002940: 2020 2020 6465 6620 7465 7374 5f69 6e73      def test_ins
-00002950: 6572 7473 2873 656c 6629 3a0a 2020 2020  erts(self):.    
-00002960: 2020 2020 7461 626c 6520 3d20 6c74 2e54      table = lt.T
-00002970: 6162 6c65 2829 0a20 2020 2020 2020 2074  able().        t
-00002980: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
-00002990: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-000029a0: 7428 312c 2032 2c20 3329 290a 2020 2020  t(1, 2, 3)).    
-000029b0: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
-000029c0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-000029d0: 6f62 6a65 6374 2834 2c20 352c 2036 2929  object(4, 5, 6))
-000029e0: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-000029f0: 7265 6174 655f 696e 6465 7828 2761 272c  reate_index('a',
-00002a00: 2075 6e69 7175 653d 5472 7565 290a 2020   unique=True).  
-00002a10: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00002a20: 7445 7175 616c 2873 656c 662e 6d61 6b65  tEqual(self.make
-00002a30: 5f64 6174 615f 6f62 6a65 6374 2834 2c20  _data_object(4, 
-00002a40: 352c 2036 292c 2074 6162 6c65 2e62 792e  5, 6), table.by.
-00002a50: 615b 345d 290a 0a20 2020 2020 2020 2077  a[4])..        w
-00002a60: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-00002a70: 6169 7365 7328 4b65 7945 7272 6f72 293a  aises(KeyError):
-00002a80: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00002a90: 6c65 2e69 6e73 6572 7428 7365 6c66 2e6d  le.insert(self.m
-00002aa0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00002ab0: 342c 2031 2c20 3029 290a 0a20 2020 2020  4, 1, 0))..     
-00002ac0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-00002ad0: 6572 7452 6169 7365 7328 4b65 7945 7272  ertRaises(KeyErr
-00002ae0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00002af0: 2074 6162 6c65 2e69 6e73 6572 7428 7365   table.insert(se
-00002b00: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00002b10: 6563 7428 4e6f 6e65 2c20 312c 2030 2929  ect(None, 1, 0))
-00002b20: 0a0a 2020 2020 2020 2020 7461 626c 652e  ..        table.
-00002b30: 6465 6c65 7465 5f69 6e64 6578 2827 6127  delete_index('a'
-00002b40: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-00002b50: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
-00002b60: 5f64 6174 615f 6f62 6a65 6374 2834 2c20  _data_object(4, 
-00002b70: 312c 2030 2929 0a0a 2020 2020 2020 2020  1, 0))..        
-00002b80: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-00002b90: 5261 6973 6573 284b 6579 4572 726f 7229  Raises(KeyError)
-00002ba0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00002bb0: 626c 652e 6372 6561 7465 5f69 6e64 6578  ble.create_index
-00002bc0: 2827 6127 2c20 756e 6971 7565 3d54 7275  ('a', unique=Tru
-00002bd0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
-00002be0: 5f69 6e73 6572 745f 6469 6374 7328 7365  _insert_dicts(se
-00002bf0: 6c66 293a 0a20 2020 2020 2020 2074 6162  lf):.        tab
-00002c00: 6c65 203d 206c 742e 5461 626c 6528 290a  le = lt.Table().
-00002c10: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
-00002c20: 7365 7274 287b 2261 223a 2031 2c20 2262  sert({"a": 1, "b
-00002c30: 223a 2032 2c20 2263 223a 2033 7d29 0a20  ": 2, "c": 3}). 
-00002c40: 2020 2020 2020 2074 6162 6c65 2e69 6e73         table.ins
-00002c50: 6572 7428 7b22 6122 3a20 342c 2022 6222  ert({"a": 4, "b"
-00002c60: 3a20 352c 2022 6322 3a20 367d 290a 2020  : 5, "c": 6}).  
-00002c70: 2020 2020 2020 7461 626c 652e 6372 6561        table.crea
-00002c80: 7465 5f69 6e64 6578 2827 6127 2c20 756e  te_index('a', un
-00002c90: 6971 7565 3d54 7275 6529 0a20 2020 2020  ique=True).     
-00002ca0: 2020 2072 6563 302c 2072 6563 3120 3d20     rec0, rec1 = 
-00002cb0: 7461 626c 650a 2020 2020 2020 2020 7365  table.        se
-00002cc0: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
-00002cd0: 2261 223a 2031 2c20 2262 223a 2032 2c20  "a": 1, "b": 2, 
-00002ce0: 2263 223a 2033 7d2c 2076 6172 7328 7265  "c": 3}, vars(re
-00002cf0: 6330 2929 0a20 2020 2020 2020 2073 656c  c0)).        sel
-00002d00: 662e 6173 7365 7274 4571 7561 6c28 6c74  f.assertEqual(lt
-00002d10: 2e64 6566 6175 6c74 5f72 6f77 5f63 6c61  .default_row_cla
-00002d20: 7373 2c20 7479 7065 2872 6563 3029 290a  ss, type(rec0)).
-00002d30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00002d40: 6572 7445 7175 616c 2831 2c20 6765 7461  ertEqual(1, geta
-00002d50: 7474 7228 7265 6330 2c20 2261 2229 290a  ttr(rec0, "a")).
-00002d60: 0a20 2020 2020 2020 2023 2069 6e73 6572  .        # inser
-00002d70: 7420 6120 6e65 7374 6564 2064 6963 740a  t a nested dict.
-00002d80: 2020 2020 2020 2020 7461 626c 652e 636c          table.cl
-00002d90: 6561 7228 290a 2020 2020 2020 2020 7461  ear().        ta
-00002da0: 626c 652e 696e 7365 7274 287b 2261 223a  ble.insert({"a":
-00002db0: 2031 2c20 2262 223a 2032 2c20 2263 223a   1, "b": 2, "c":
-00002dc0: 2033 2c20 2264 223a 207b 2278 223a 2031   3, "d": {"x": 1
-00002dd0: 3030 2c20 2279 223a 2032 3030 7d7d 290a  00, "y": 200}}).
-00002de0: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
-00002df0: 7365 7274 287b 2261 223a 2034 2c20 2262  sert({"a": 4, "b
-00002e00: 223a 2035 2c20 2263 223a 2036 2c20 2264  ": 5, "c": 6, "d
-00002e10: 223a 207b 2278 223a 2031 3031 2c20 2279  ": {"x": 101, "y
-00002e20: 223a 2032 3031 7d7d 290a 2020 2020 2020  ": 201}}).      
-00002e30: 2020 7265 6330 2c20 7265 6331 203d 2074    rec0, rec1 = t
-00002e40: 6162 6c65 0a20 2020 2020 2020 2073 656c  able.        sel
-00002e50: 662e 6173 7365 7274 4571 7561 6c28 3130  f.assertEqual(10
-00002e60: 302c 2072 6563 302e 642e 7829 0a20 2020  0, rec0.d.x).   
-00002e70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002e80: 4571 7561 6c28 3130 312c 2072 6563 312e  Equal(101, rec1.
-00002e90: 642e 7829 0a0a 2020 2020 6465 6620 7465  d.x)..    def te
-00002ea0: 7374 5f77 6865 7265 5f65 7175 616c 7328  st_where_equals(
-00002eb0: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00002ec0: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
-00002ed0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
-00002ee0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-00002ef0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00002f00: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-00002f10: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00002f20: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00002f30: 697a 652a 7465 7374 5f73 697a 652c 206c  ize*test_size, l
-00002f40: 656e 2874 6162 6c65 2e77 6865 7265 2861  en(table.where(a
-00002f50: 3d35 2929 290a 2020 2020 2020 2020 7365  =5))).        se
-00002f60: 6c66 2e61 7373 6572 7445 7175 616c 2830  lf.assertEqual(0
-00002f70: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00002f80: 6528 613d 2d31 2929 290a 0a20 2020 2064  e(a=-1)))..    d
-00002f90: 6566 2074 6573 745f 7768 6572 655f 6571  ef test_where_eq
-00002fa0: 7561 6c73 5f6e 6f6e 6528 7365 6c66 293a  uals_none(self):
-00002fb0: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-00002fc0: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
-00002fd0: 7461 626c 6520 3d20 6d61 6b65 5f74 6573  table = make_tes
-00002fe0: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00002ff0: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00003000: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
-00003010: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00003020: 7561 6c28 302c 206c 656e 2874 6162 6c65  ual(0, len(table
-00003030: 2e77 6865 7265 2861 3d35 2c20 623d 7465  .where(a=5, b=te
-00003040: 7374 5f73 697a 6529 2929 0a0a 2020 2020  st_size)))..    
-00003050: 6465 6620 7465 7374 5f77 6865 7265 5f65  def test_where_e
-00003060: 7175 616c 735f 7769 7468 5f69 6e64 6578  quals_with_index
-00003070: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003080: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
-00003090: 2020 2020 2020 2074 6162 6c65 203d 206d         table = m
-000030a0: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000030b0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000030c0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000030d0: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-000030e0: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
-000030f0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00003100: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-00003110: 7369 7a65 2a74 6573 745f 7369 7a65 2c20  size*test_size, 
-00003120: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003130: 613d 3529 2929 0a20 2020 2020 2020 2073  a=5))).        s
-00003140: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00003150: 302c 206c 656e 2874 6162 6c65 2e77 6865  0, len(table.whe
-00003160: 7265 2861 3d2d 3129 2929 0a0a 2020 2020  re(a=-1)))..    
-00003170: 6465 6620 7465 7374 5f77 6865 7265 5f72  def test_where_r
-00003180: 616e 6765 2873 656c 6629 3a0a 2020 2020  ange(self):.    
-00003190: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-000031a0: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-000031b0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000031c0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000031d0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-000031e0: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
-000031f0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00003200: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-00003210: 7a65 2c20 6c65 6e28 7461 626c 652e 7768  ze, len(table.wh
-00003220: 6572 6528 6c61 6d62 6461 2072 6563 3a20  ere(lambda rec: 
-00003230: 7265 632e 6120 3d3d 2072 6563 2e62 2929  rec.a == rec.b))
-00003240: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00003250: 7768 6572 655f 636f 6d70 6172 6174 6f72  where_comparator
-00003260: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003270: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
-00003280: 2020 2020 2020 2074 6162 6c65 203d 206d         table = m
-00003290: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000032a0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000032b0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000032c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000032d0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-000032e0: 7369 7a65 2a74 6573 745f 7369 7a65 2a34  size*test_size*4
-000032f0: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00003300: 6528 613d 6c74 2e54 6162 6c65 2e6c 7428  e(a=lt.Table.lt(
-00003310: 3429 2929 290a 2020 2020 2020 2020 7365  4)))).        se
-00003320: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00003330: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-00003340: 7a65 2a28 342b 3129 2c20 6c65 6e28 7461  ze*(4+1), len(ta
-00003350: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
-00003360: 6162 6c65 2e6c 6528 3429 2929 290a 2020  able.le(4)))).  
-00003370: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00003380: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-00003390: 2a74 6573 745f 7369 7a65 2a28 7465 7374  *test_size*(test
-000033a0: 5f73 697a 652d 342d 3129 2c20 6c65 6e28  _size-4-1), len(
-000033b0: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-000033c0: 2e54 6162 6c65 2e67 7428 3429 2929 290a  .Table.gt(4)))).
-000033d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000033e0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-000033f0: 7a65 2a74 6573 745f 7369 7a65 2a28 7465  ze*test_size*(te
-00003400: 7374 5f73 697a 652d 3429 2c20 6c65 6e28  st_size-4), len(
-00003410: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003420: 2e54 6162 6c65 2e67 6528 3429 2929 290a  .Table.ge(4)))).
-00003430: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003440: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00003450: 7a65 2a74 6573 745f 7369 7a65 2a28 7465  ze*test_size*(te
-00003460: 7374 5f73 697a 652d 3129 2c20 6c65 6e28  st_size-1), len(
-00003470: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003480: 2e54 6162 6c65 2e6e 6528 3429 2929 290a  .Table.ne(4)))).
-00003490: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000034a0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-000034b0: 7a65 2a74 6573 745f 7369 7a65 2c20 6c65  ze*test_size, le
-000034c0: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
-000034d0: 6c74 2e54 6162 6c65 2e65 7128 3429 2929  lt.Table.eq(4)))
-000034e0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000034f0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-00003500: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
-00003510: 7768 6572 6528 613d 6c74 2e54 6162 6c65  where(a=lt.Table
-00003520: 2e65 7128 3429 2c20 623d 6c74 2e54 6162  .eq(4), b=lt.Tab
-00003530: 6c65 2e65 7128 3429 2929 290a 2020 2020  le.eq(4)))).    
-00003540: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003550: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
-00003560: 6573 745f 7369 7a65 2a34 2c20 6c65 6e28  est_size*4, len(
-00003570: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003580: 2e54 6162 6c65 2e62 6574 7765 656e 2833  .Table.between(3
-00003590: 2c20 3829 2929 290a 2020 2020 2020 2020  , 8)))).        
-000035a0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000035b0: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
-000035c0: 7369 7a65 2a34 2c20 6c65 6e28 7461 626c  size*4, len(tabl
-000035d0: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
-000035e0: 6c65 2e77 6974 6869 6e28 322c 2035 2929  le.within(2, 5))
-000035f0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00003600: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-00003610: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-00003620: 332c 206c 656e 2874 6162 6c65 2e77 6865  3, len(table.whe
-00003630: 7265 2861 3d6c 742e 5461 626c 652e 696e  re(a=lt.Table.in
-00003640: 5f72 616e 6765 2832 2c20 3529 2929 290a  _range(2, 5)))).
-00003650: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003660: 6572 7445 7175 616c 2830 2c20 6c65 6e28  ertEqual(0, len(
-00003670: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003680: 2e54 6162 6c65 2e62 6574 7765 656e 2833  .Table.between(3
-00003690: 2c20 3329 2929 290a 2020 2020 2020 2020  , 3)))).        
-000036a0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000036b0: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
-000036c0: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
-000036d0: 7768 6572 6528 613d 6c74 2e54 6162 6c65  where(a=lt.Table
-000036e0: 2e77 6974 6869 6e28 332c 2033 2929 2929  .within(3, 3))))
-000036f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003700: 7365 7274 4571 7561 6c28 302c 206c 656e  sertEqual(0, len
-00003710: 2874 6162 6c65 2e77 6865 7265 2861 3d6c  (table.where(a=l
-00003720: 742e 5461 626c 652e 696e 5f72 616e 6765  t.Table.in_range
-00003730: 2833 2c20 3329 2929 290a 2020 2020 2020  (3, 3)))).      
-00003740: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003750: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-00003760: 745f 7369 7a65 2a34 2c20 6c65 6e28 7461  t_size*4, len(ta
-00003770: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
-00003780: 6162 6c65 2e69 735f 696e 285b 322c 2034  able.is_in([2, 4
-00003790: 2c20 362c 2038 5d29 2929 290a 2020 2020  , 6, 8])))).    
-000037a0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000037b0: 7175 616c 2830 2c20 6c65 6e28 7461 626c  qual(0, len(tabl
-000037c0: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
-000037d0: 6c65 2e69 735f 696e 285b 5d29 2929 290a  le.is_in([])))).
-000037e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000037f0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00003800: 7a65 2a74 6573 745f 7369 7a65 2a28 7465  ze*test_size*(te
-00003810: 7374 5f73 697a 652d 3429 2c20 6c65 6e28  st_size-4), len(
-00003820: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003830: 2e54 6162 6c65 2e6e 6f74 5f69 6e28 5b32  .Table.not_in([2
-00003840: 2c20 342c 2036 2c20 385d 2929 2929 0a20  , 4, 6, 8])))). 
-00003850: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00003860: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-00003870: 652a 7465 7374 5f73 697a 652a 7465 7374  e*test_size*test
-00003880: 5f73 697a 652c 206c 656e 2874 6162 6c65  _size, len(table
-00003890: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-000038a0: 652e 6e6f 745f 696e 285b 5d29 2929 290a  e.not_in([])))).
-000038b0: 0a20 2020 2020 2020 2023 2061 6464 2061  .        # add a
-000038c0: 2072 6563 6f72 6420 636f 6e74 6169 6e69   record containi
-000038d0: 6e67 2061 204e 6f6e 6520 7661 6c75 6520  ng a None value 
-000038e0: 746f 2074 6573 7420 6973 5f6e 6f6e 6520  to test is_none 
-000038f0: 616e 6420 6973 5f6e 6f74 5f6e 6f6e 6520  and is_not_none 
-00003900: 636f 6d70 6172 6174 6f72 730a 2020 2020  comparators.    
-00003910: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
-00003920: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00003930: 6f62 6a65 6374 2861 3d31 2c20 623d 322c  object(a=1, b=2,
-00003940: 2063 3d4e 6f6e 6529 290a 2020 2020 2020   c=None)).      
-00003950: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003960: 616c 2831 2c20 6c65 6e28 7461 626c 652e  al(1, len(table.
-00003970: 7768 6572 6528 633d 6c74 2e54 6162 6c65  where(c=lt.Table
-00003980: 2e69 735f 6e6f 6e65 2829 2929 290a 2020  .is_none()))).  
-00003990: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000039a0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-000039b0: 2a74 6573 745f 7369 7a65 2a74 6573 745f  *test_size*test_
-000039c0: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
-000039d0: 7768 6572 6528 633d 6c74 2e54 6162 6c65  where(c=lt.Table
-000039e0: 2e69 735f 6e6f 745f 6e6f 6e65 2829 2929  .is_not_none()))
-000039f0: 290a 0a20 2020 2020 2020 2023 2061 6464  )..        # add
-00003a00: 2061 2072 6563 6f72 6420 636f 6e74 6169   a record contai
-00003a10: 6e69 6e67 2061 206d 6973 7369 6e67 2076  ning a missing v
-00003a20: 616c 7565 2074 6f20 7465 7374 2069 735f  alue to test is_
-00003a30: 6e75 6c6c 2061 6e64 2069 735f 6e6f 745f  null and is_not_
-00003a40: 6e75 6c6c 2063 6f6d 7061 7261 746f 7273  null comparators
-00003a50: 0a20 2020 2020 2020 2074 6162 6c65 2e69  .        table.i
-00003a60: 6e73 6572 7428 7365 6c66 2e6d 616b 655f  nsert(self.make_
-00003a70: 6461 7461 5f6f 626a 6563 7428 613d 312c  data_object(a=1,
-00003a80: 2062 3d32 2c20 633d 2222 2929 0a20 2020   b=2, c="")).   
-00003a90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00003aa0: 4571 7561 6c28 322c 206c 656e 2874 6162  Equal(2, len(tab
-00003ab0: 6c65 2e77 6865 7265 2863 3d6c 742e 5461  le.where(c=lt.Ta
-00003ac0: 626c 652e 6973 5f6e 756c 6c28 2929 2929  ble.is_null())))
-00003ad0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003ae0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00003af0: 697a 6520 2a20 7465 7374 5f73 697a 6520  ize * test_size 
-00003b00: 2a20 7465 7374 5f73 697a 652c 206c 656e  * test_size, len
-00003b10: 2874 6162 6c65 2e77 6865 7265 2863 3d6c  (table.where(c=l
-00003b20: 742e 5461 626c 652e 6973 5f6e 6f74 5f6e  t.Table.is_not_n
-00003b30: 756c 6c28 2929 2929 0a0a 2020 2020 2020  ull())))..      
-00003b40: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00003b50: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
-00003b60: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-00003b70: 626a 6563 7428 613d 312c 2062 3d32 2929  bject(a=1, b=2))
-00003b80: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00003b90: 5479 7065 4572 726f 723a 0a20 2020 2020  TypeError:.     
-00003ba0: 2020 2020 2020 2023 206e 6f74 2061 6c6c         # not all
-00003bb0: 2064 6174 6120 6f62 6a65 6374 2074 7970   data object typ
-00003bc0: 6573 2062 6569 6e67 2074 6573 7465 6420  es being tested 
-00003bd0: 7375 7070 6f72 7420 6d69 7373 696e 6720  support missing 
-00003be0: 6174 7472 6962 7574 6573 0a20 2020 2020  attributes.     
-00003bf0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
-00003c00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003c10: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00003c20: 7445 7175 616c 2833 2c20 6c65 6e28 7461  tEqual(3, len(ta
-00003c30: 626c 652e 7768 6572 6528 633d 6c74 2e54  ble.where(c=lt.T
-00003c40: 6162 6c65 2e69 735f 6e75 6c6c 2829 2929  able.is_null()))
-00003c50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003c60: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00003c70: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-00003c80: 7369 7a65 202a 2074 6573 745f 7369 7a65  size * test_size
-00003c90: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00003ca0: 6528 633d 6c74 2e54 6162 6c65 2e69 735f  e(c=lt.Table.is_
-00003cb0: 6e6f 745f 6e75 6c6c 2829 2929 290a 0a20  not_null()))).. 
-00003cc0: 2020 2064 6566 2074 6573 745f 7768 6572     def test_wher
-00003cd0: 655f 7374 725f 636f 6d70 6172 6174 6f72  e_str_comparator
-00003ce0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003cf0: 756e 6963 6f64 655f 6e75 6d62 6572 7320  unicode_numbers 
-00003d00: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00003d10: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-00003d20: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-00003d30: 2020 2020 2020 2020 206e 616d 652c 636f           name,co
-00003d40: 6465 5f76 616c 7565 2c6e 756d 6572 6963  de_value,numeric
-00003d50: 5f76 616c 7565 0a20 2020 2020 2020 2020  _value.         
-00003d60: 2020 2052 4f4d 414e 204e 554d 4552 414c     ROMAN NUMERAL
-00003d70: 204f 4e45 2c38 3534 342c 310a 2020 2020   ONE,8544,1.    
-00003d80: 2020 2020 2020 2020 524f 4d41 4e20 4e55          ROMAN NU
-00003d90: 4d45 5241 4c20 5457 4f2c 3835 3435 2c32  MERAL TWO,8545,2
-00003da0: 0a20 2020 2020 2020 2020 2020 2052 4f4d  .            ROM
-00003db0: 414e 204e 554d 4552 414c 2054 4852 4545  AN NUMERAL THREE
-00003dc0: 2c38 3534 362c 330a 2020 2020 2020 2020  ,8546,3.        
-00003dd0: 2020 2020 524f 4d41 4e20 4e55 4d45 5241      ROMAN NUMERA
-00003de0: 4c20 464f 5552 2c38 3534 372c 340a 2020  L FOUR,8547,4.  
-00003df0: 2020 2020 2020 2020 2020 524f 4d41 4e20            ROMAN 
-00003e00: 4e55 4d45 5241 4c20 4649 5645 2c38 3534  NUMERAL FIVE,854
-00003e10: 382c 350a 2020 2020 2020 2020 2020 2020  8,5.            
-00003e20: 524f 4d41 4e20 4e55 4d45 5241 4c20 5349  ROMAN NUMERAL SI
-00003e30: 582c 3835 3439 2c36 0a20 2020 2020 2020  X,8549,6.       
-00003e40: 2020 2020 2052 4f4d 414e 204e 554d 4552       ROMAN NUMER
-00003e50: 414c 2053 4556 454e 2c38 3535 302c 370a  AL SEVEN,8550,7.
-00003e60: 2020 2020 2020 2020 2020 2020 524f 4d41              ROMA
-00003e70: 4e20 4e55 4d45 5241 4c20 4549 4748 542c  N NUMERAL EIGHT,
-00003e80: 3835 3531 2c38 0a20 2020 2020 2020 2020  8551,8.         
-00003e90: 2020 2052 4f4d 414e 204e 554d 4552 414c     ROMAN NUMERAL
-00003ea0: 204e 494e 452c 3835 3532 2c39 0a20 2020   NINE,8552,9.   
-00003eb0: 2020 2020 2020 2020 2052 4f4d 414e 204e           ROMAN N
-00003ec0: 554d 4552 414c 2054 454e 2c38 3535 332c  UMERAL TEN,8553,
-00003ed0: 3130 0a20 2020 2020 2020 2020 2020 2053  10.            S
-00003ee0: 5550 4552 5343 5249 5054 2054 574f 2c31  UPERSCRIPT TWO,1
-00003ef0: 3738 2c32 0a20 2020 2020 2020 2020 2020  78,2.           
-00003f00: 2053 5550 4552 5343 5249 5054 2054 4852   SUPERSCRIPT THR
-00003f10: 4545 2c31 3739 2c33 0a20 2020 2020 2020  EE,179,3.       
-00003f20: 2020 2020 2053 5550 4552 5343 5249 5054       SUPERSCRIPT
-00003f30: 204f 4e45 2c31 3835 2c31 0a20 2020 2020   ONE,185,1.     
-00003f40: 2020 2020 2020 2053 5550 4552 5343 5249         SUPERSCRI
-00003f50: 5054 205a 4552 4f2c 3833 3034 2c30 0a20  PT ZERO,8304,0. 
-00003f60: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
-00003f70: 5343 5249 5054 2046 4f55 522c 3833 3038  SCRIPT FOUR,8308
-00003f80: 2c34 0a20 2020 2020 2020 2020 2020 2053  ,4.            S
-00003f90: 5550 4552 5343 5249 5054 2046 4956 452c  UPERSCRIPT FIVE,
-00003fa0: 3833 3039 2c35 0a20 2020 2020 2020 2020  8309,5.         
-00003fb0: 2020 2053 5550 4552 5343 5249 5054 2053     SUPERSCRIPT S
-00003fc0: 4958 2c38 3331 302c 360a 2020 2020 2020  IX,8310,6.      
-00003fd0: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
-00003fe0: 5420 5345 5645 4e2c 3833 3131 2c37 0a20  T SEVEN,8311,7. 
-00003ff0: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
-00004000: 5343 5249 5054 2045 4947 4854 2c38 3331  SCRIPT EIGHT,831
-00004010: 322c 380a 2020 2020 2020 2020 2020 2020  2,8.            
-00004020: 5355 5045 5253 4352 4950 5420 4e49 4e45  SUPERSCRIPT NINE
-00004030: 2c38 3331 332c 390a 2020 2020 2020 2020  ,8313,9.        
-00004040: 2020 2020 4349 5243 4c45 4420 4449 4749      CIRCLED DIGI
-00004050: 5420 4f4e 452c 3933 3132 2c31 0a20 2020  T ONE,9312,1.   
-00004060: 2020 2020 2020 2020 2043 4952 434c 4544           CIRCLED
-00004070: 2044 4947 4954 2054 574f 2c39 3331 332c   DIGIT TWO,9313,
-00004080: 320a 2020 2020 2020 2020 2020 2020 4349  2.            CI
-00004090: 5243 4c45 4420 4449 4749 5420 5448 5245  RCLED DIGIT THRE
-000040a0: 452c 3933 3134 2c33 0a20 2020 2020 2020  E,9314,3.       
-000040b0: 2020 2020 2043 4952 434c 4544 2044 4947       CIRCLED DIG
-000040c0: 4954 2046 4f55 522c 3933 3135 2c34 0a20  IT FOUR,9315,4. 
-000040d0: 2020 2020 2020 2020 2020 2043 4952 434c             CIRCL
-000040e0: 4544 2044 4947 4954 2046 4956 452c 3933  ED DIGIT FIVE,93
-000040f0: 3136 2c35 0a20 2020 2020 2020 2020 2020  16,5.           
-00004100: 2043 4952 434c 4544 2044 4947 4954 2053   CIRCLED DIGIT S
-00004110: 4958 2c39 3331 372c 360a 2020 2020 2020  IX,9317,6.      
-00004120: 2020 2020 2020 4349 5243 4c45 4420 4449        CIRCLED DI
-00004130: 4749 5420 5345 5645 4e2c 3933 3138 2c37  GIT SEVEN,9318,7
-00004140: 0a20 2020 2020 2020 2020 2020 2043 4952  .            CIR
-00004150: 434c 4544 2044 4947 4954 2045 4947 4854  CLED DIGIT EIGHT
-00004160: 2c39 3331 392c 380a 2020 2020 2020 2020  ,9319,8.        
-00004170: 2020 2020 4349 5243 4c45 4420 4449 4749      CIRCLED DIGI
-00004180: 5420 4e49 4e45 2c39 3332 302c 390a 2020  T NINE,9320,9.  
-00004190: 2020 2020 2020 2020 2020 4349 5243 4c45            CIRCLE
-000041a0: 4420 4449 4749 5420 5a45 524f 2c39 3435  D DIGIT ZERO,945
-000041b0: 302c 300a 2020 2020 2020 2020 2020 2020  0,0.            
-000041c0: 2222 2229 290a 0a20 2020 2020 2020 206f  """))..        o
-000041d0: 6e65 7320 3d20 756e 6963 6f64 655f 6e75  nes = unicode_nu
-000041e0: 6d62 6572 732e 7768 6572 6528 6e61 6d65  mbers.where(name
-000041f0: 3d6c 742e 5461 626c 652e 656e 6473 7769  =lt.Table.endswi
-00004200: 7468 2822 4f4e 4522 2929 0a20 2020 2020  th("ONE")).     
-00004210: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00004220: 7561 6c28 332c 206c 656e 286f 6e65 7329  ual(3, len(ones)
-00004230: 290a 0a20 2020 2020 2020 2073 7570 6572  )..        super
-00004240: 7320 3d20 756e 6963 6f64 655f 6e75 6d62  s = unicode_numb
-00004250: 6572 732e 7768 6572 6528 6e61 6d65 3d6c  ers.where(name=l
-00004260: 742e 5461 626c 652e 7374 6172 7473 7769  t.Table.startswi
-00004270: 7468 2822 5355 5045 5253 4352 4950 5422  th("SUPERSCRIPT"
-00004280: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00004290: 6173 7365 7274 4571 7561 6c28 3130 2c20  assertEqual(10, 
-000042a0: 6c65 6e28 7375 7065 7273 2929 0a0a 2020  len(supers))..  
-000042b0: 2020 2020 2020 2320 696d 706f 7274 2072        # import r
-000042c0: 650a 2020 2020 2020 2020 2320 7365 7665  e.        # seve
-000042d0: 6e73 203d 2075 6e69 636f 6465 5f6e 756d  ns = unicode_num
-000042e0: 6265 7273 2e77 6865 7265 286c 616d 6264  bers.where(lambd
-000042f0: 6120 7265 633a 2072 652e 636f 6d70 696c  a rec: re.compil
-00004300: 6528 7222 2e2a 5345 5645 4e24 2229 2e6d  e(r".*SEVEN$").m
-00004310: 6174 6368 2872 6563 2e6e 616d 6529 290a  atch(rec.name)).
-00004320: 0a20 2020 2020 2020 2073 6576 656e 7320  .        sevens 
-00004330: 3d20 756e 6963 6f64 655f 6e75 6d62 6572  = unicode_number
-00004340: 732e 7768 6572 6528 6e61 6d65 3d6c 742e  s.where(name=lt.
-00004350: 5461 626c 652e 7265 5f6d 6174 6368 2872  Table.re_match(r
-00004360: 222e 2a53 4556 454e 2422 2929 0a20 2020  ".*SEVEN$")).   
-00004370: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00004380: 4571 7561 6c28 332c 206c 656e 2873 6576  Equal(3, len(sev
-00004390: 656e 7329 290a 0a20 2020 2020 2020 2023  ens))..        #
-000043a0: 206d 616b 6520 6e61 6d65 7320 616c 6c20   make names all 
-000043b0: 7469 746c 6520 6361 7365 0a20 2020 2020  title case.     
-000043c0: 2020 2075 6e69 636f 6465 5f6e 756d 6265     unicode_numbe
-000043d0: 7273 2e61 6464 5f66 6965 6c64 2822 6e61  rs.add_field("na
-000043e0: 6d65 222c 206c 616d 6264 6120 7265 633a  me", lambda rec:
-000043f0: 2072 6563 2e6e 616d 652e 7469 746c 6528   rec.name.title(
-00004400: 2929 0a20 2020 2020 2020 2023 2075 7365  )).        # use
-00004410: 2072 6567 6578 2077 6974 6820 7265 2066   regex with re f
-00004420: 6c61 670a 2020 2020 2020 2020 696d 706f  lag.        impo
-00004430: 7274 2072 650a 2020 2020 2020 2020 6369  rt re.        ci
-00004440: 7263 6c65 6420 3d20 756e 6963 6f64 655f  rcled = unicode_
-00004450: 6e75 6d62 6572 732e 7768 6572 6528 6e61  numbers.where(na
-00004460: 6d65 3d6c 742e 5461 626c 652e 7265 5f6d  me=lt.Table.re_m
-00004470: 6174 6368 2872 2263 6972 636c 6564 222c  atch(r"circled",
-00004480: 2066 6c61 6773 3d72 652e 4929 290a 2020   flags=re.I)).  
-00004490: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000044a0: 7445 7175 616c 2831 302c 206c 656e 2863  tEqual(10, len(c
-000044b0: 6972 636c 6564 2929 0a0a 2020 2020 6465  ircled))..    de
-000044c0: 6620 7465 7374 5f77 6865 7265 5f61 7474  f test_where_att
-000044d0: 725f 6675 6e63 7469 6f6e 2873 656c 6629  r_function(self)
-000044e0: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
-000044f0: 697a 6520 3d20 380a 2020 2020 2020 2020  ize = 8.        
-00004500: 7461 626c 6520 3d20 6d61 6b65 5f74 6573  table = make_tes
-00004510: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00004520: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00004530: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
-00004540: 2020 2064 6566 2069 735f 6f64 6428 7829     def is_odd(x)
-00004550: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004560: 7475 726e 2062 6f6f 6c28 7820 2520 3229  turn bool(x % 2)
-00004570: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00004580: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-00004590: 7369 7a65 2a74 6573 745f 7369 7a65 2a74  size*test_size*t
-000045a0: 6573 745f 7369 7a65 2f2f 322c 206c 656e  est_size//2, len
-000045b0: 2874 6162 6c65 2e77 6865 7265 2861 3d69  (table.where(a=i
-000045c0: 735f 6f64 6429 2929 0a0a 2020 2020 6465  s_odd)))..    de
-000045d0: 6620 7465 7374 5f67 6574 5f73 6c69 6365  f test_get_slice
-000045e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000045f0: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
-00004600: 2020 2020 2020 2074 6162 6c65 203d 206d         table = m
-00004610: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-00004620: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00004630: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-00004640: 0a0a 2020 2020 2020 2020 7375 6274 6162  ..        subtab
-00004650: 6c65 203d 2074 6162 6c65 5b30 3a3a 7465  le = table[0::te
-00004660: 7374 5f73 697a 655d 0a20 2020 2020 2020  st_size].       
-00004670: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00004680: 6c28 7465 7374 5f73 697a 6520 2a20 7465  l(test_size * te
-00004690: 7374 5f73 697a 652c 206c 656e 2873 7562  st_size, len(sub
-000046a0: 7461 626c 6529 290a 0a20 2020 2064 6566  table))..    def
-000046b0: 2074 6573 745f 696e 6465 7869 6e67 2873   test_indexing(s
-000046c0: 656c 6629 3a0a 2020 2020 2020 2020 6368  elf):.        ch
-000046d0: 6172 7320 3d20 2241 4243 4445 4647 4849  ars = "ABCDEFGHI
-000046e0: 4a4b 4c4d 4e4f 5051 5253 5455 5657 5859  JKLMNOPQRSTUVWXY
-000046f0: 5a22 0a20 2020 2020 2020 206d 616b 655f  Z".        make_
-00004700: 7265 6320 3d20 6c61 6d62 6461 2061 612c  rec = lambda aa,
-00004710: 2062 622c 2063 633a 2073 656c 662e 6d61   bb, cc: self.ma
-00004720: 6b65 5f64 6174 615f 6f62 6a65 6374 2863  ke_data_object(c
-00004730: 6861 7273 5b61 615d 2c20 6368 6172 735b  hars[aa], chars[
-00004740: 6262 5d2c 2063 6861 7273 5b63 635d 290a  bb], chars[cc]).
-00004750: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-00004760: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-00004770: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
-00004780: 5f74 6162 6c65 286d 616b 655f 7265 632c  _table(make_rec,
-00004790: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
-000047a0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-000047b0: 5f69 6e64 6578 2827 6127 290a 0a20 2020  _index('a')..   
-000047c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000047d0: 5472 7565 2827 4127 2069 6e20 7461 626c  True('A' in tabl
-000047e0: 652e 6279 2e61 290a 2020 2020 2020 2020  e.by.a).        
-000047f0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00004800: 2741 4127 206e 6f74 2069 6e20 7461 626c  'AA' not in tabl
-00004810: 652e 6279 2e61 290a 2020 2020 2020 2020  e.by.a).        
-00004820: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00004830: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
-00004840: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
-00004850: 652e 6279 2e61 5b27 4227 5d29 290a 2020  e.by.a['B'])).  
-00004860: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00004870: 7454 7275 6528 6973 696e 7374 616e 6365  tTrue(isinstance
-00004880: 2874 6162 6c65 2e62 792e 615b 2742 275d  (table.by.a['B']
-00004890: 2c20 6c74 2e54 6162 6c65 2929 0a20 2020  , lt.Table)).   
-000048a0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-000048b0: 7373 6572 7452 6169 7365 7328 4174 7472  ssertRaises(Attr
-000048c0: 6962 7574 6545 7272 6f72 293a 0a20 2020  ibuteError):.   
-000048d0: 2020 2020 2020 2020 2074 6162 6c65 2e62           table.b
-000048e0: 792e 7a0a 0a20 2020 2020 2020 2073 656c  y.z..        sel
-000048f0: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00004900: 7374 5f73 697a 652c 206c 656e 2874 6162  st_size, len(tab
-00004910: 6c65 2e62 792e 612e 6b65 7973 2829 2929  le.by.a.keys()))
-00004920: 0a0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
-00004930: 6e69 7175 655f 696e 6465 7869 6e67 2873  nique_indexing(s
-00004940: 656c 6629 3a0a 2020 2020 2020 2020 6368  elf):.        ch
-00004950: 6172 7320 3d20 2241 4243 4445 4647 4849  ars = "ABCDEFGHI
-00004960: 4a4b 4c4d 4e4f 5051 5253 5455 5657 5859  JKLMNOPQRSTUVWXY
-00004970: 5a22 0a20 2020 2020 2020 206d 616b 655f  Z".        make_
-00004980: 756e 6971 7565 5f6b 6579 203d 206c 616d  unique_key = lam
-00004990: 6264 6120 2a61 7267 733a 2027 272e 6a6f  bda *args: ''.jo
-000049a0: 696e 2863 6861 7273 5b61 7267 5d20 666f  in(chars[arg] fo
-000049b0: 7220 6172 6720 696e 2061 7267 7329 0a20  r arg in args). 
-000049c0: 2020 2020 2020 206d 616b 655f 7265 6320         make_rec 
-000049d0: 3d20 6c61 6d62 6461 2061 612c 2062 622c  = lambda aa, bb,
-000049e0: 2063 633a 2073 656c 662e 6d61 6b65 5f64   cc: self.make_d
-000049f0: 6174 615f 6f62 6a65 6374 286d 616b 655f  ata_object(make_
-00004a00: 756e 6971 7565 5f6b 6579 2861 612c 2062  unique_key(aa, b
-00004a10: 622c 2063 6329 2c20 6368 6172 735b 6262  b, cc), chars[bb
-00004a20: 5d2c 2063 6861 7273 5b63 635d 290a 2020  ], chars[cc]).  
-00004a30: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00004a40: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
-00004a50: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
-00004a60: 6162 6c65 286d 616b 655f 7265 632c 2074  able(make_rec, t
-00004a70: 6573 745f 7369 7a65 2928 2254 6162 6c65  est_size)("Table
-00004a80: 5f31 2229 0a20 2020 2020 2020 2074 6162  _1").        tab
-00004a90: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
-00004aa0: 2761 272c 2075 6e69 7175 653d 5472 7565  'a', unique=True
-00004ab0: 290a 2020 2020 2020 2020 7265 635f 7479  ).        rec_ty
-00004ac0: 7065 203d 2074 7970 6528 7365 6c66 2e6d  pe = type(self.m
-00004ad0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00004ae0: 302c 2030 2c20 3029 290a 0a20 2020 2020  0, 0, 0))..     
-00004af0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00004b00: 7565 2827 4141 4127 2069 6e20 7461 626c  ue('AAA' in tabl
-00004b10: 652e 6279 2e61 290a 2020 2020 2020 2020  e.by.a).        
-00004b20: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00004b30: 2741 4127 206e 6f74 2069 6e20 7461 626c  'AA' not in tabl
-00004b40: 652e 6279 2e61 290a 2020 2020 2020 2020  e.by.a).        
-00004b50: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00004b60: 6973 696e 7374 616e 6365 2874 6162 6c65  isinstance(table
-00004b70: 2e62 792e 615b 2742 4141 275d 2c20 7265  .by.a['BAA'], re
-00004b80: 635f 7479 7065 2929 0a20 2020 2020 2020  c_type)).       
-00004b90: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-00004ba0: 7452 6169 7365 7328 4b65 7945 7272 6f72  tRaises(KeyError
-00004bb0: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00004bc0: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
-00004bd0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00004be0: 7428 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  t(None, None, No
-00004bf0: 6e65 2929 0a0a 2020 2020 2020 2020 2320  ne))..        # 
-00004c00: 6372 6561 7465 2064 7570 6c69 6361 7465  create duplicate
-00004c10: 2069 6e64 6578 0a20 2020 2020 2020 2077   index.        w
-00004c20: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-00004c30: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
-00004c40: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00004c50: 6162 6c65 2e63 7265 6174 655f 696e 6465  able.create_inde
-00004c60: 7828 2761 272c 2075 6e69 7175 653d 5472  x('a', unique=Tr
-00004c70: 7565 2c20 6163 6365 7074 5f6e 6f6e 653d  ue, accept_none=
-00004c80: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
-00004c90: 2063 7265 6174 6520 756e 6971 7565 2069   create unique i
-00004ca0: 6e64 6578 2074 6861 7420 616c 6c6f 7773  ndex that allows
-00004cb0: 204e 6f6e 6520 7661 6c75 6573 0a20 2020   None values.   
-00004cc0: 2020 2020 2074 6162 6c65 2e64 656c 6574       table.delet
-00004cd0: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
-00004ce0: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-00004cf0: 655f 696e 6465 7828 2761 272c 2075 6e69  e_index('a', uni
-00004d00: 7175 653d 5472 7565 2c20 6163 6365 7074  que=True, accept
-00004d10: 5f6e 6f6e 653d 5472 7565 290a 2020 2020  _none=True).    
-00004d20: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
-00004d30: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00004d40: 6f62 6a65 6374 284e 6f6e 652c 204e 6f6e  object(None, Non
-00004d50: 652c 2027 4127 2929 0a0a 2020 2020 2020  e, 'A'))..      
-00004d60: 2020 7374 725f 6e6f 6e65 5f63 6f6d 7061    str_none_compa
-00004d70: 7265 203d 206c 616d 6264 6120 783a 2078  re = lambda x: x
-00004d80: 2069 6620 6973 696e 7374 616e 6365 2878   if isinstance(x
-00004d90: 2c20 7374 7229 2065 6c73 6520 6368 7228  , str) else chr(
-00004da0: 3235 3529 2a31 3030 0a20 2020 2020 2020  255)*100.       
-00004db0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00004dc0: 6c28 736f 7274 6564 2874 6162 6c65 2e62  l(sorted(table.b
-00004dd0: 792e 612e 6b65 7973 2829 2c20 6b65 793d  y.a.keys(), key=
-00004de0: 7374 725f 6e6f 6e65 5f63 6f6d 7061 7265  str_none_compare
-00004df0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00004e00: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-00004e10: 6564 2874 6162 6c65 2e61 6c6c 2e61 2c20  ed(table.all.a, 
-00004e20: 6b65 793d 7374 725f 6e6f 6e65 5f63 6f6d  key=str_none_com
-00004e30: 7061 7265 2929 0a0a 2020 2020 2020 2020  pare))..        
-00004e40: 2320 6e6f 7720 6472 6f70 2069 6e64 6578  # now drop index
-00004e50: 2061 6e64 2072 6563 7265 6174 6520 6e6f   and recreate no
-00004e60: 7420 7065 726d 6974 7469 6e67 204e 6f6e  t permitting Non
-00004e70: 652c 2073 686f 756c 6420 7261 6973 6520  e, should raise 
-00004e80: 6578 6365 7074 696f 6e0a 2020 2020 2020  exception.      
-00004e90: 2020 7461 626c 652e 6465 6c65 7465 5f69    table.delete_i
-00004ea0: 6e64 6578 2827 6127 290a 2020 2020 2020  ndex('a').      
-00004eb0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-00004ec0: 7274 5261 6973 6573 284b 6579 4572 726f  rtRaises(KeyErro
-00004ed0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00002300: 7065 4661 6374 6f72 790a 2020 2020 5573  peFactory.    Us
+00002310: 696e 6750 7964 616e 7469 6349 6d6d 7574  ingPydanticImmut
+00002320: 6162 6c65 4d6f 6465 6c20 3d20 4162 7374  ableModel = Abst
+00002330: 7261 6374 436f 6e74 656e 7454 7970 6546  ractContentTypeF
+00002340: 6163 746f 7279 0a20 2020 2055 7369 6e67  actory.    Using
+00002350: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
+00002360: 203d 2041 6273 7472 6163 7443 6f6e 7465   = AbstractConte
+00002370: 6e74 5479 7065 4661 6374 6f72 790a 0a69  ntTypeFactory..i
+00002380: 6620 6174 7472 2069 7320 6e6f 7420 4e6f  f attr is not No
+00002390: 6e65 3a0a 2020 2020 636c 6173 7320 5573  ne:.    class Us
+000023a0: 696e 6741 7474 7243 6c61 7373 2841 6273  ingAttrClass(Abs
+000023b0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
+000023c0: 4661 6374 6f72 7929 3a0a 2020 2020 2020  Factory):.      
+000023d0: 2020 6461 7461 5f6f 626a 6563 745f 7479    data_object_ty
+000023e0: 7065 203d 2041 7474 7243 6c61 7373 0a65  pe = AttrClass.e
+000023f0: 6c73 653a 0a20 2020 2055 7369 6e67 4174  lse:.    UsingAt
+00002400: 7472 436c 6173 7320 3d20 4162 7374 7261  trClass = Abstra
+00002410: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
+00002420: 746f 7279 0a0a 6966 2074 7261 6974 6c65  tory..if traitle
+00002430: 7473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ts is not None:.
+00002440: 2020 2020 636c 6173 7320 5573 696e 6754      class UsingT
+00002450: 7261 6974 6c65 7473 436c 6173 7328 4162  raitletsClass(Ab
+00002460: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
+00002470: 6546 6163 746f 7279 293a 0a20 2020 2020  eFactory):.     
+00002480: 2020 2064 6174 615f 6f62 6a65 6374 5f74     data_object_t
+00002490: 7970 6520 3d20 5472 6169 746c 6574 7343  ype = TraitletsC
+000024a0: 6c61 7373 0a65 6c73 653a 0a20 2020 2055  lass.else:.    U
+000024b0: 7369 6e67 5472 6169 746c 6574 7343 6c61  singTraitletsCla
+000024c0: 7373 203d 2041 6273 7472 6163 7443 6f6e  ss = AbstractCon
+000024d0: 7465 6e74 5479 7065 4661 6374 6f72 790a  tentTypeFactory.
+000024e0: 0a63 6c61 7373 2055 7369 6e67 5479 7069  .class UsingTypi
+000024f0: 6e67 4e61 6d65 6454 7570 6c65 2841 6273  ngNamedTuple(Abs
+00002500: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
+00002510: 4661 6374 6f72 7929 3a0a 2020 2020 6461  Factory):.    da
+00002520: 7461 5f6f 626a 6563 745f 7479 7065 203d  ta_object_type =
+00002530: 2054 7970 696e 674e 616d 6564 5475 706c   TypingNamedTupl
+00002540: 650a 0a63 6c61 7373 2055 7369 6e67 5479  e..class UsingTy
+00002550: 7069 6e67 5479 7065 6444 6963 7428 4162  pingTypedDict(Ab
+00002560: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
+00002570: 6546 6163 746f 7279 293a 0a20 2020 2064  eFactory):.    d
+00002580: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
+00002590: 3d20 5479 7069 6e67 5479 7065 6444 6963  = TypingTypedDic
+000025a0: 740a 0a20 2020 2040 636c 6173 736d 6574  t..    @classmet
+000025b0: 686f 640a 2020 2020 6465 6620 6d61 6b65  hod.    def make
+000025c0: 5f64 6174 615f 6f62 6a65 6374 2863 6c73  _data_object(cls
+000025d0: 2c20 612c 2062 2c20 6329 3a0a 2020 2020  , a, b, c):.    
+000025e0: 2020 2020 7265 7475 726e 2053 696d 706c      return Simpl
+000025f0: 654e 616d 6573 7061 6365 2861 3d61 2c20  eNamespace(a=a, 
+00002600: 623d 622c 2063 3d63 290a 0a64 6566 206c  b=b, c=c)..def l
+00002610: 6f61 645f 7461 626c 6528 7461 626c 652c  oad_table(table,
+00002620: 2072 6563 5f66 6163 746f 7279 5f66 6e2c   rec_factory_fn,
+00002630: 2074 6162 6c65 5f73 697a 6529 3a0a 2020   table_size):.  
+00002640: 2020 7465 7374 5f73 697a 6520 3d20 7461    test_size = ta
+00002650: 626c 655f 7369 7a65 0a20 2020 2074 6162  ble_size.    tab
+00002660: 6c65 2e69 6e73 6572 745f 6d61 6e79 280a  le.insert_many(.
+00002670: 2020 2020 2020 2020 7265 635f 6661 6374          rec_fact
+00002680: 6f72 795f 666e 2861 612c 2062 622c 2063  ory_fn(aa, bb, c
+00002690: 6329 0a20 2020 2020 2020 2066 6f72 2061  c).        for a
+000026a0: 612c 2062 622c 2063 6320 696e 2069 7465  a, bb, cc in ite
+000026b0: 7274 6f6f 6c73 2e70 726f 6475 6374 2872  rtools.product(r
+000026c0: 616e 6765 2874 6573 745f 7369 7a65 292c  ange(test_size),
+000026d0: 2072 6570 6561 743d 3329 0a20 2020 2029   repeat=3).    )
+000026e0: 0a0a 0a64 6566 206d 616b 655f 7465 7374  ...def make_test
+000026f0: 5f74 6162 6c65 2872 6563 5f66 6163 746f  _table(rec_facto
+00002700: 7279 5f66 6e2c 2074 6162 6c65 5f73 697a  ry_fn, table_siz
+00002710: 6529 3a0a 2020 2020 7461 626c 6520 3d20  e):.    table = 
+00002720: 6c74 2e54 6162 6c65 2829 0a20 2020 206c  lt.Table().    l
+00002730: 6f61 645f 7461 626c 6528 7461 626c 652c  oad_table(table,
+00002740: 2072 6563 5f66 6163 746f 7279 5f66 6e2c   rec_factory_fn,
+00002750: 2074 6162 6c65 5f73 697a 6529 0a20 2020   table_size).   
+00002760: 2072 6574 7572 6e20 7461 626c 650a 0a0a   return table...
+00002770: 6465 6620 6d61 6b65 5f64 6174 616f 626a  def make_dataobj
+00002780: 6563 745f 6672 6f6d 5f6f 6228 7265 6329  ect_from_ob(rec)
+00002790: 3a0a 2020 2020 7265 7475 726e 2053 696d  :.    return Sim
+000027a0: 706c 654e 616d 6573 7061 6365 282a 2a7b  pleNamespace(**{
+000027b0: 6b3a 2067 6574 6174 7472 2872 6563 2c20  k: getattr(rec, 
+000027c0: 6b29 2066 6f72 206b 2069 6e20 6c74 2e5f  k) for k in lt._
+000027d0: 6f62 6a65 6374 5f61 7474 726e 616d 6573  object_attrnames
+000027e0: 2872 6563 297d 290a 0a0a 636c 6173 7320  (rec)})...class 
+000027f0: 5461 626c 6554 7970 6554 6573 7473 2875  TableTypeTests(u
+00002800: 6e69 7474 6573 742e 5465 7374 4361 7365  nittest.TestCase
+00002810: 293a 0a20 2020 2064 6566 2074 6573 745f  ):.    def test_
+00002820: 7479 7065 7328 7365 6c66 293a 0a20 2020  types(self):.   
+00002830: 2020 2020 2066 726f 6d20 636f 6c6c 6563       from collec
+00002840: 7469 6f6e 732e 6162 6320 696d 706f 7274  tions.abc import
+00002850: 2028 4361 6c6c 6162 6c65 2c20 436f 6e74   (Callable, Cont
+00002860: 6169 6e65 722c 2049 7465 7261 626c 652c  ainer, Iterable,
+00002870: 2043 6f6c 6c65 6374 696f 6e2c 204d 6170   Collection, Map
+00002880: 7069 6e67 2c20 5265 7665 7273 6962 6c65  ping, Reversible
+00002890: 2c20 5365 7175 656e 6365 2c20 5369 7a65  , Sequence, Size
+000028a0: 6429 0a0a 2020 2020 2020 2020 7462 6c20  d)..        tbl 
+000028b0: 3d20 6c74 2e54 6162 6c65 2829 0a20 2020  = lt.Table().   
+000028c0: 2020 2020 2074 626c 2e63 7265 6174 655f       tbl.create_
+000028d0: 696e 6465 7828 2269 6478 2229 0a0a 2020  index("idx")..  
+000028e0: 2020 2020 2020 666f 7220 7375 7065 7263        for superc
+000028f0: 6c61 7373 2069 6e20 2843 616c 6c61 626c  lass in (Callabl
+00002900: 652c 2053 697a 6564 2c20 4974 6572 6162  e, Sized, Iterab
+00002910: 6c65 2c20 436f 6e74 6169 6e65 722c 2043  le, Container, C
+00002920: 6f6c 6c65 6374 696f 6e2c 2052 6576 6572  ollection, Rever
+00002930: 7369 626c 652c 2053 6571 7565 6e63 6529  sible, Sequence)
+00002940: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00002950: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00002960: 7375 7065 7263 6c61 7373 3d73 7570 6572  superclass=super
+00002970: 636c 6173 7329 3a0a 2020 2020 2020 2020  class):.        
+00002980: 2020 2020 2020 2020 7072 696e 7428 7375          print(su
+00002990: 7065 7263 6c61 7373 2e5f 5f6e 616d 655f  perclass.__name_
+000029a0: 5f29 0a20 2020 2020 2020 2020 2020 2020  _).             
+000029b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+000029c0: 7565 2869 7369 6e73 7461 6e63 6528 7462  ue(isinstance(tb
+000029d0: 6c2c 2073 7570 6572 636c 6173 7329 290a  l, superclass)).
+000029e0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+000029f0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00002a00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00002a10: 2269 7369 6e73 7461 6e63 6528 5f4f 626a  "isinstance(_Obj
+00002a20: 496e 6465 782c 204d 6170 7069 6e67 2922  Index, Mapping)"
+00002a30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00002a40: 6c66 2e61 7373 6572 7454 7275 6528 6973  lf.assertTrue(is
+00002a50: 696e 7374 616e 6365 2874 626c 2e5f 696e  instance(tbl._in
+00002a60: 6465 7865 735b 2269 6478 225d 2c20 4d61  dexes["idx"], Ma
+00002a70: 7070 696e 6729 290a 0a20 2020 2020 2020  pping))..       
+00002a80: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00002a90: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00002aa0: 2020 7072 696e 7428 2269 7369 6e73 7461    print("isinsta
+00002ab0: 6e63 6528 5f4f 626a 496e 6465 7857 7261  nce(_ObjIndexWra
+00002ac0: 7070 6572 2c20 4d61 7070 696e 6729 2229  pper, Mapping)")
+00002ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002ae0: 662e 6173 7365 7274 5472 7565 2869 7369  f.assertTrue(isi
+00002af0: 6e73 7461 6e63 6528 7462 6c2e 6279 2e69  nstance(tbl.by.i
+00002b00: 6478 2c20 4d61 7070 696e 6729 290a 0a0a  dx, Mapping))...
+00002b10: 406d 616b 655f 7465 7374 5f63 6c61 7373  @make_test_class
+00002b20: 6573 0a63 6c61 7373 2054 6162 6c65 4372  es.class TableCr
+00002b30: 6561 7465 5465 7374 733a 0a20 2020 2064  eateTests:.    d
+00002b40: 6566 2074 6573 745f 696e 7365 7274 7328  ef test_inserts(
+00002b50: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+00002b60: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+00002b70: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+00002b80: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
+00002b90: 5f64 6174 615f 6f62 6a65 6374 2831 2c20  _data_object(1, 
+00002ba0: 322c 2033 2929 0a20 2020 2020 2020 2074  2, 3)).        t
+00002bb0: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
+00002bc0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00002bd0: 7428 342c 2035 2c20 3629 290a 2020 2020  t(4, 5, 6)).    
+00002be0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
+00002bf0: 5f69 6e64 6578 2827 6127 2c20 756e 6971  _index('a', uniq
+00002c00: 7565 3d54 7275 6529 0a20 2020 2020 2020  ue=True).       
+00002c10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00002c20: 6c28 7365 6c66 2e6d 616b 655f 6461 7461  l(self.make_data
+00002c30: 5f6f 626a 6563 7428 342c 2035 2c20 3629  _object(4, 5, 6)
+00002c40: 2c20 7461 626c 652e 6279 2e61 5b34 5d29  , table.by.a[4])
+00002c50: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00002c60: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00002c70: 284b 6579 4572 726f 7229 3a0a 2020 2020  (KeyError):.    
+00002c80: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
+00002c90: 7365 7274 2873 656c 662e 6d61 6b65 5f64  sert(self.make_d
+00002ca0: 6174 615f 6f62 6a65 6374 2834 2c20 312c  ata_object(4, 1,
+00002cb0: 2030 2929 0a0a 2020 2020 2020 2020 7769   0))..        wi
+00002cc0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+00002cd0: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
+00002ce0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00002cf0: 652e 696e 7365 7274 2873 656c 662e 6d61  e.insert(self.ma
+00002d00: 6b65 5f64 6174 615f 6f62 6a65 6374 284e  ke_data_object(N
+00002d10: 6f6e 652c 2031 2c20 3029 290a 0a20 2020  one, 1, 0))..   
+00002d20: 2020 2020 2074 6162 6c65 2e64 656c 6574       table.delet
+00002d30: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
+00002d40: 2020 2020 2074 6162 6c65 2e69 6e73 6572       table.inser
+00002d50: 7428 7365 6c66 2e6d 616b 655f 6461 7461  t(self.make_data
+00002d60: 5f6f 626a 6563 7428 342c 2031 2c20 3029  _object(4, 1, 0)
+00002d70: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00002d80: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00002d90: 7328 4b65 7945 7272 6f72 293a 0a20 2020  s(KeyError):.   
+00002da0: 2020 2020 2020 2020 2074 6162 6c65 2e63           table.c
+00002db0: 7265 6174 655f 696e 6465 7828 2761 272c  reate_index('a',
+00002dc0: 2075 6e69 7175 653d 5472 7565 290a 0a20   unique=True).. 
+00002dd0: 2020 2064 6566 2074 6573 745f 696e 7365     def test_inse
+00002de0: 7274 5f64 6963 7473 2873 656c 6629 3a0a  rt_dicts(self):.
+00002df0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+00002e00: 6c74 2e54 6162 6c65 2829 0a20 2020 2020  lt.Table().     
+00002e10: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
+00002e20: 7b22 6122 3a20 312c 2022 6222 3a20 322c  {"a": 1, "b": 2,
+00002e30: 2022 6322 3a20 337d 290a 2020 2020 2020   "c": 3}).      
+00002e40: 2020 7461 626c 652e 696e 7365 7274 287b    table.insert({
+00002e50: 2261 223a 2034 2c20 2262 223a 2035 2c20  "a": 4, "b": 5, 
+00002e60: 2263 223a 2036 7d29 0a20 2020 2020 2020  "c": 6}).       
+00002e70: 2074 6162 6c65 2e63 7265 6174 655f 696e   table.create_in
+00002e80: 6465 7828 2761 272c 2075 6e69 7175 653d  dex('a', unique=
+00002e90: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
+00002ea0: 6330 2c20 7265 6331 203d 2074 6162 6c65  c0, rec1 = table
+00002eb0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00002ec0: 7365 7274 4571 7561 6c28 7b22 6122 3a20  sertEqual({"a": 
+00002ed0: 312c 2022 6222 3a20 322c 2022 6322 3a20  1, "b": 2, "c": 
+00002ee0: 337d 2c20 7661 7273 2872 6563 3029 290a  3}, vars(rec0)).
+00002ef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00002f00: 6572 7445 7175 616c 286c 742e 6465 6661  ertEqual(lt.defa
+00002f10: 756c 745f 726f 775f 636c 6173 732c 2074  ult_row_class, t
+00002f20: 7970 6528 7265 6330 2929 0a20 2020 2020  ype(rec0)).     
+00002f30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00002f40: 7561 6c28 312c 2067 6574 6174 7472 2872  ual(1, getattr(r
+00002f50: 6563 302c 2022 6122 2929 0a0a 2020 2020  ec0, "a"))..    
+00002f60: 2020 2020 2320 696e 7365 7274 2061 206e      # insert a n
+00002f70: 6573 7465 6420 6469 6374 0a20 2020 2020  ested dict.     
+00002f80: 2020 2074 6162 6c65 2e63 6c65 6172 2829     table.clear()
+00002f90: 0a20 2020 2020 2020 2074 6162 6c65 2e69  .        table.i
+00002fa0: 6e73 6572 7428 7b22 6122 3a20 312c 2022  nsert({"a": 1, "
+00002fb0: 6222 3a20 322c 2022 6322 3a20 332c 2022  b": 2, "c": 3, "
+00002fc0: 6422 3a20 7b22 7822 3a20 3130 302c 2022  d": {"x": 100, "
+00002fd0: 7922 3a20 3230 307d 7d29 0a20 2020 2020  y": 200}}).     
+00002fe0: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
+00002ff0: 7b22 6122 3a20 342c 2022 6222 3a20 352c  {"a": 4, "b": 5,
+00003000: 2022 6322 3a20 362c 2022 6422 3a20 7b22   "c": 6, "d": {"
+00003010: 7822 3a20 3130 312c 2022 7922 3a20 3230  x": 101, "y": 20
+00003020: 317d 7d29 0a20 2020 2020 2020 2072 6563  1}}).        rec
+00003030: 302c 2072 6563 3120 3d20 7461 626c 650a  0, rec1 = table.
+00003040: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003050: 6572 7445 7175 616c 2831 3030 2c20 7265  ertEqual(100, re
+00003060: 6330 2e64 2e78 290a 2020 2020 2020 2020  c0.d.x).        
+00003070: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003080: 2831 3031 2c20 7265 6331 2e64 2e78 290a  (101, rec1.d.x).
+00003090: 0a20 2020 2064 6566 2074 6573 745f 7768  .    def test_wh
+000030a0: 6572 655f 6571 7561 6c73 2873 656c 6629  ere_equals(self)
+000030b0: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
+000030c0: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
+000030d0: 2074 6162 6c65 203d 206d 616b 655f 7465   table = make_te
+000030e0: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+000030f0: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00003100: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+00003110: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003120: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
+00003130: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
+00003140: 626c 652e 7768 6572 6528 613d 3529 2929  ble.where(a=5)))
+00003150: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00003160: 7365 7274 4571 7561 6c28 302c 206c 656e  sertEqual(0, len
+00003170: 2874 6162 6c65 2e77 6865 7265 2861 3d2d  (table.where(a=-
+00003180: 3129 2929 0a0a 2020 2020 6465 6620 7465  1)))..    def te
+00003190: 7374 5f77 6865 7265 5f65 7175 616c 735f  st_where_equals_
+000031a0: 6e6f 6e65 2873 656c 6629 3a0a 2020 2020  none(self):.    
+000031b0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+000031c0: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
+000031d0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+000031e0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+000031f0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+00003200: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
+00003210: 6c66 2e61 7373 6572 7445 7175 616c 2830  lf.assertEqual(0
+00003220: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003230: 6528 613d 352c 2062 3d74 6573 745f 7369  e(a=5, b=test_si
+00003240: 7a65 2929 290a 0a20 2020 2064 6566 2074  ze)))..    def t
+00003250: 6573 745f 7768 6572 655f 6571 7561 6c73  est_where_equals
+00003260: 5f77 6974 685f 696e 6465 7828 7365 6c66  _with_index(self
+00003270: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+00003280: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00003290: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+000032a0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+000032b0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+000032c0: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
+000032d0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
+000032e0: 5f69 6e64 6578 2827 6127 290a 0a20 2020  _index('a')..   
+000032f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00003300: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
+00003310: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
+00003320: 6162 6c65 2e77 6865 7265 2861 3d35 2929  able.where(a=5))
+00003330: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003340: 7373 6572 7445 7175 616c 2830 2c20 6c65  ssertEqual(0, le
+00003350: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003360: 2d31 2929 290a 0a20 2020 2064 6566 2074  -1)))..    def t
+00003370: 6573 745f 7768 6572 655f 7261 6e67 6528  est_where_range(
+00003380: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+00003390: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
+000033a0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+000033b0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+000033c0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000033d0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+000033e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000033f0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00003400: 697a 652a 7465 7374 5f73 697a 652c 206c  ize*test_size, l
+00003410: 656e 2874 6162 6c65 2e77 6865 7265 286c  en(table.where(l
+00003420: 616d 6264 6120 7265 633a 2072 6563 2e61  ambda rec: rec.a
+00003430: 203d 3d20 7265 632e 6229 2929 0a0a 2020   == rec.b)))..  
+00003440: 2020 6465 6620 7465 7374 5f77 6865 7265    def test_where
+00003450: 5f63 6f6d 7061 7261 746f 7228 7365 6c66  _comparator(self
+00003460: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+00003470: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00003480: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00003490: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+000034a0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+000034b0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+000034c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000034d0: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
+000034e0: 7465 7374 5f73 697a 652a 342c 206c 656e  test_size*4, len
+000034f0: 2874 6162 6c65 2e77 6865 7265 2861 3d6c  (table.where(a=l
+00003500: 742e 5461 626c 652e 6c74 2834 2929 2929  t.Table.lt(4))))
+00003510: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00003520: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00003530: 697a 652a 7465 7374 5f73 697a 652a 2834  ize*test_size*(4
+00003540: 2b31 292c 206c 656e 2874 6162 6c65 2e77  +1), len(table.w
+00003550: 6865 7265 2861 3d6c 742e 5461 626c 652e  here(a=lt.Table.
+00003560: 6c65 2834 2929 2929 0a20 2020 2020 2020  le(4)))).       
+00003570: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00003580: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
+00003590: 5f73 697a 652a 2874 6573 745f 7369 7a65  _size*(test_size
+000035a0: 2d34 2d31 292c 206c 656e 2874 6162 6c65  -4-1), len(table
+000035b0: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+000035c0: 652e 6774 2834 2929 2929 0a20 2020 2020  e.gt(4)))).     
+000035d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000035e0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
+000035f0: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
+00003600: 7a65 2d34 292c 206c 656e 2874 6162 6c65  ze-4), len(table
+00003610: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+00003620: 652e 6765 2834 2929 2929 0a20 2020 2020  e.ge(4)))).     
+00003630: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00003640: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
+00003650: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
+00003660: 7a65 2d31 292c 206c 656e 2874 6162 6c65  ze-1), len(table
+00003670: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+00003680: 652e 6e65 2834 2929 2929 0a20 2020 2020  e.ne(4)))).     
+00003690: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000036a0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
+000036b0: 7374 5f73 697a 652c 206c 656e 2874 6162  st_size, len(tab
+000036c0: 6c65 2e77 6865 7265 2861 3d6c 742e 5461  le.where(a=lt.Ta
+000036d0: 626c 652e 6571 2834 2929 2929 0a20 2020  ble.eq(4)))).   
+000036e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000036f0: 4571 7561 6c28 7465 7374 5f73 697a 652c  Equal(test_size,
+00003700: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
+00003710: 2861 3d6c 742e 5461 626c 652e 6571 2834  (a=lt.Table.eq(4
+00003720: 292c 2062 3d6c 742e 5461 626c 652e 6571  ), b=lt.Table.eq
+00003730: 2834 2929 2929 0a20 2020 2020 2020 2073  (4)))).        s
+00003740: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003750: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
+00003760: 697a 652a 342c 206c 656e 2874 6162 6c65  ize*4, len(table
+00003770: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+00003780: 652e 6265 7477 6565 6e28 332c 2038 2929  e.between(3, 8))
+00003790: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000037a0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+000037b0: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
+000037c0: 342c 206c 656e 2874 6162 6c65 2e77 6865  4, len(table.whe
+000037d0: 7265 2861 3d6c 742e 5461 626c 652e 7769  re(a=lt.Table.wi
+000037e0: 7468 696e 2832 2c20 3529 2929 290a 2020  thin(2, 5)))).  
+000037f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00003800: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00003810: 2a74 6573 745f 7369 7a65 2a33 2c20 6c65  *test_size*3, le
+00003820: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003830: 6c74 2e54 6162 6c65 2e69 6e5f 7261 6e67  lt.Table.in_rang
+00003840: 6528 322c 2035 2929 2929 0a20 2020 2020  e(2, 5)))).     
+00003850: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00003860: 7561 6c28 302c 206c 656e 2874 6162 6c65  ual(0, len(table
+00003870: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+00003880: 652e 6265 7477 6565 6e28 332c 2033 2929  e.between(3, 3))
+00003890: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000038a0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+000038b0: 5f73 697a 652a 7465 7374 5f73 697a 652c  _size*test_size,
+000038c0: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
+000038d0: 2861 3d6c 742e 5461 626c 652e 7769 7468  (a=lt.Table.with
+000038e0: 696e 2833 2c20 3329 2929 290a 2020 2020  in(3, 3)))).    
+000038f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003900: 7175 616c 2830 2c20 6c65 6e28 7461 626c  qual(0, len(tabl
+00003910: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
+00003920: 6c65 2e69 6e5f 7261 6e67 6528 332c 2033  le.in_range(3, 3
+00003930: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
+00003940: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
+00003950: 7374 5f73 697a 652a 7465 7374 5f73 697a  st_size*test_siz
+00003960: 652a 342c 206c 656e 2874 6162 6c65 2e77  e*4, len(table.w
+00003970: 6865 7265 2861 3d6c 742e 5461 626c 652e  here(a=lt.Table.
+00003980: 6973 5f69 6e28 5b32 2c20 342c 2036 2c20  is_in([2, 4, 6, 
+00003990: 385d 2929 2929 0a20 2020 2020 2020 2073  8])))).        s
+000039a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000039b0: 302c 206c 656e 2874 6162 6c65 2e77 6865  0, len(table.whe
+000039c0: 7265 2861 3d6c 742e 5461 626c 652e 6973  re(a=lt.Table.is
+000039d0: 5f69 6e28 5b5d 2929 2929 0a20 2020 2020  _in([])))).     
+000039e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000039f0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
+00003a00: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
+00003a10: 7a65 2d34 292c 206c 656e 2874 6162 6c65  ze-4), len(table
+00003a20: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
+00003a30: 652e 6e6f 745f 696e 285b 322c 2034 2c20  e.not_in([2, 4, 
+00003a40: 362c 2038 5d29 2929 290a 2020 2020 2020  6, 8])))).      
+00003a50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00003a60: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
+00003a70: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+00003a80: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003a90: 6528 613d 6c74 2e54 6162 6c65 2e6e 6f74  e(a=lt.Table.not
+00003aa0: 5f69 6e28 5b5d 2929 2929 0a0a 2020 2020  _in([]))))..    
+00003ab0: 2020 2020 2320 6164 6420 6120 7265 636f      # add a reco
+00003ac0: 7264 2063 6f6e 7461 696e 696e 6720 6120  rd containing a 
+00003ad0: 4e6f 6e65 2076 616c 7565 2074 6f20 7465  None value to te
+00003ae0: 7374 2069 735f 6e6f 6e65 2061 6e64 2069  st is_none and i
+00003af0: 735f 6e6f 745f 6e6f 6e65 2063 6f6d 7061  s_not_none compa
+00003b00: 7261 746f 7273 0a20 2020 2020 2020 2074  rators.        t
+00003b10: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
+00003b20: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00003b30: 7428 613d 312c 2062 3d32 2c20 633d 4e6f  t(a=1, b=2, c=No
+00003b40: 6e65 2929 0a20 2020 2020 2020 2073 656c  ne)).        sel
+00003b50: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
+00003b60: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
+00003b70: 2863 3d6c 742e 5461 626c 652e 6973 5f6e  (c=lt.Table.is_n
+00003b80: 6f6e 6528 2929 2929 0a20 2020 2020 2020  one()))).       
+00003b90: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00003ba0: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
+00003bb0: 5f73 697a 652a 7465 7374 5f73 697a 652c  _size*test_size,
+00003bc0: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
+00003bd0: 2863 3d6c 742e 5461 626c 652e 6973 5f6e  (c=lt.Table.is_n
+00003be0: 6f74 5f6e 6f6e 6528 2929 2929 0a0a 2020  ot_none())))..  
+00003bf0: 2020 2020 2020 2320 6164 6420 6120 7265        # add a re
+00003c00: 636f 7264 2063 6f6e 7461 696e 696e 6720  cord containing 
+00003c10: 6120 6d69 7373 696e 6720 7661 6c75 6520  a missing value 
+00003c20: 746f 2074 6573 7420 6973 5f6e 756c 6c20  to test is_null 
+00003c30: 616e 6420 6973 5f6e 6f74 5f6e 756c 6c20  and is_not_null 
+00003c40: 636f 6d70 6172 6174 6f72 730a 2020 2020  comparators.    
+00003c50: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
+00003c60: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+00003c70: 6f62 6a65 6374 2861 3d31 2c20 623d 322c  object(a=1, b=2,
+00003c80: 2063 3d22 2229 290a 2020 2020 2020 2020   c="")).        
+00003c90: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003ca0: 2832 2c20 6c65 6e28 7461 626c 652e 7768  (2, len(table.wh
+00003cb0: 6572 6528 633d 6c74 2e54 6162 6c65 2e69  ere(c=lt.Table.i
+00003cc0: 735f 6e75 6c6c 2829 2929 290a 2020 2020  s_null()))).    
+00003cd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003ce0: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
+00003cf0: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
+00003d00: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
+00003d10: 652e 7768 6572 6528 633d 6c74 2e54 6162  e.where(c=lt.Tab
+00003d20: 6c65 2e69 735f 6e6f 745f 6e75 6c6c 2829  le.is_not_null()
+00003d30: 2929 290a 0a20 2020 2020 2020 2074 7279  )))..        try
+00003d40: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+00003d50: 626c 652e 696e 7365 7274 2873 656c 662e  ble.insert(self.
+00003d60: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00003d70: 2861 3d31 2c20 623d 3229 290a 2020 2020  (a=1, b=2)).    
+00003d80: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
+00003d90: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00003da0: 2020 2320 6e6f 7420 616c 6c20 6461 7461    # not all data
+00003db0: 206f 626a 6563 7420 7479 7065 7320 6265   object types be
+00003dc0: 696e 6720 7465 7374 6564 2073 7570 706f  ing tested suppo
+00003dd0: 7274 206d 6973 7369 6e67 2061 7474 7269  rt missing attri
+00003de0: 6275 7465 730a 2020 2020 2020 2020 2020  butes.          
+00003df0: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
+00003e00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003e10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00003e20: 6c28 332c 206c 656e 2874 6162 6c65 2e77  l(3, len(table.w
+00003e30: 6865 7265 2863 3d6c 742e 5461 626c 652e  here(c=lt.Table.
+00003e40: 6973 5f6e 756c 6c28 2929 2929 0a20 2020  is_null()))).   
+00003e50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00003e60: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00003e70: 697a 6520 2a20 7465 7374 5f73 697a 6520  ize * test_size 
+00003e80: 2a20 7465 7374 5f73 697a 652c 206c 656e  * test_size, len
+00003e90: 2874 6162 6c65 2e77 6865 7265 2863 3d6c  (table.where(c=l
+00003ea0: 742e 5461 626c 652e 6973 5f6e 6f74 5f6e  t.Table.is_not_n
+00003eb0: 756c 6c28 2929 2929 0a0a 2020 2020 6465  ull())))..    de
+00003ec0: 6620 7465 7374 5f77 6865 7265 5f73 7472  f test_where_str
+00003ed0: 5f63 6f6d 7061 7261 746f 7228 7365 6c66  _comparator(self
+00003ee0: 293a 0a20 2020 2020 2020 2075 6e69 636f  ):.        unico
+00003ef0: 6465 5f6e 756d 6265 7273 203d 206c 742e  de_numbers = lt.
+00003f00: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00003f10: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
+00003f20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+00003f30: 2020 2020 6e61 6d65 2c63 6f64 655f 7661      name,code_va
+00003f40: 6c75 652c 6e75 6d65 7269 635f 7661 6c75  lue,numeric_valu
+00003f50: 650a 2020 2020 2020 2020 2020 2020 524f  e.            RO
+00003f60: 4d41 4e20 4e55 4d45 5241 4c20 4f4e 452c  MAN NUMERAL ONE,
+00003f70: 3835 3434 2c31 0a20 2020 2020 2020 2020  8544,1.         
+00003f80: 2020 2052 4f4d 414e 204e 554d 4552 414c     ROMAN NUMERAL
+00003f90: 2054 574f 2c38 3534 352c 320a 2020 2020   TWO,8545,2.    
+00003fa0: 2020 2020 2020 2020 524f 4d41 4e20 4e55          ROMAN NU
+00003fb0: 4d45 5241 4c20 5448 5245 452c 3835 3436  MERAL THREE,8546
+00003fc0: 2c33 0a20 2020 2020 2020 2020 2020 2052  ,3.            R
+00003fd0: 4f4d 414e 204e 554d 4552 414c 2046 4f55  OMAN NUMERAL FOU
+00003fe0: 522c 3835 3437 2c34 0a20 2020 2020 2020  R,8547,4.       
+00003ff0: 2020 2020 2052 4f4d 414e 204e 554d 4552       ROMAN NUMER
+00004000: 414c 2046 4956 452c 3835 3438 2c35 0a20  AL FIVE,8548,5. 
+00004010: 2020 2020 2020 2020 2020 2052 4f4d 414e             ROMAN
+00004020: 204e 554d 4552 414c 2053 4958 2c38 3534   NUMERAL SIX,854
+00004030: 392c 360a 2020 2020 2020 2020 2020 2020  9,6.            
+00004040: 524f 4d41 4e20 4e55 4d45 5241 4c20 5345  ROMAN NUMERAL SE
+00004050: 5645 4e2c 3835 3530 2c37 0a20 2020 2020  VEN,8550,7.     
+00004060: 2020 2020 2020 2052 4f4d 414e 204e 554d         ROMAN NUM
+00004070: 4552 414c 2045 4947 4854 2c38 3535 312c  ERAL EIGHT,8551,
+00004080: 380a 2020 2020 2020 2020 2020 2020 524f  8.            RO
+00004090: 4d41 4e20 4e55 4d45 5241 4c20 4e49 4e45  MAN NUMERAL NINE
+000040a0: 2c38 3535 322c 390a 2020 2020 2020 2020  ,8552,9.        
+000040b0: 2020 2020 524f 4d41 4e20 4e55 4d45 5241      ROMAN NUMERA
+000040c0: 4c20 5445 4e2c 3835 3533 2c31 300a 2020  L TEN,8553,10.  
+000040d0: 2020 2020 2020 2020 2020 5355 5045 5253            SUPERS
+000040e0: 4352 4950 5420 5457 4f2c 3137 382c 320a  CRIPT TWO,178,2.
+000040f0: 2020 2020 2020 2020 2020 2020 5355 5045              SUPE
+00004100: 5253 4352 4950 5420 5448 5245 452c 3137  RSCRIPT THREE,17
+00004110: 392c 330a 2020 2020 2020 2020 2020 2020  9,3.            
+00004120: 5355 5045 5253 4352 4950 5420 4f4e 452c  SUPERSCRIPT ONE,
+00004130: 3138 352c 310a 2020 2020 2020 2020 2020  185,1.          
+00004140: 2020 5355 5045 5253 4352 4950 5420 5a45    SUPERSCRIPT ZE
+00004150: 524f 2c38 3330 342c 300a 2020 2020 2020  RO,8304,0.      
+00004160: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
+00004170: 5420 464f 5552 2c38 3330 382c 340a 2020  T FOUR,8308,4.  
+00004180: 2020 2020 2020 2020 2020 5355 5045 5253            SUPERS
+00004190: 4352 4950 5420 4649 5645 2c38 3330 392c  CRIPT FIVE,8309,
+000041a0: 350a 2020 2020 2020 2020 2020 2020 5355  5.            SU
+000041b0: 5045 5253 4352 4950 5420 5349 582c 3833  PERSCRIPT SIX,83
+000041c0: 3130 2c36 0a20 2020 2020 2020 2020 2020  10,6.           
+000041d0: 2053 5550 4552 5343 5249 5054 2053 4556   SUPERSCRIPT SEV
+000041e0: 454e 2c38 3331 312c 370a 2020 2020 2020  EN,8311,7.      
+000041f0: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
+00004200: 5420 4549 4748 542c 3833 3132 2c38 0a20  T EIGHT,8312,8. 
+00004210: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
+00004220: 5343 5249 5054 204e 494e 452c 3833 3133  SCRIPT NINE,8313
+00004230: 2c39 0a20 2020 2020 2020 2020 2020 2043  ,9.            C
+00004240: 4952 434c 4544 2044 4947 4954 204f 4e45  IRCLED DIGIT ONE
+00004250: 2c39 3331 322c 310a 2020 2020 2020 2020  ,9312,1.        
+00004260: 2020 2020 4349 5243 4c45 4420 4449 4749      CIRCLED DIGI
+00004270: 5420 5457 4f2c 3933 3133 2c32 0a20 2020  T TWO,9313,2.   
+00004280: 2020 2020 2020 2020 2043 4952 434c 4544           CIRCLED
+00004290: 2044 4947 4954 2054 4852 4545 2c39 3331   DIGIT THREE,931
+000042a0: 342c 330a 2020 2020 2020 2020 2020 2020  4,3.            
+000042b0: 4349 5243 4c45 4420 4449 4749 5420 464f  CIRCLED DIGIT FO
+000042c0: 5552 2c39 3331 352c 340a 2020 2020 2020  UR,9315,4.      
+000042d0: 2020 2020 2020 4349 5243 4c45 4420 4449        CIRCLED DI
+000042e0: 4749 5420 4649 5645 2c39 3331 362c 350a  GIT FIVE,9316,5.
+000042f0: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
+00004300: 4c45 4420 4449 4749 5420 5349 582c 3933  LED DIGIT SIX,93
+00004310: 3137 2c36 0a20 2020 2020 2020 2020 2020  17,6.           
+00004320: 2043 4952 434c 4544 2044 4947 4954 2053   CIRCLED DIGIT S
+00004330: 4556 454e 2c39 3331 382c 370a 2020 2020  EVEN,9318,7.    
+00004340: 2020 2020 2020 2020 4349 5243 4c45 4420          CIRCLED 
+00004350: 4449 4749 5420 4549 4748 542c 3933 3139  DIGIT EIGHT,9319
+00004360: 2c38 0a20 2020 2020 2020 2020 2020 2043  ,8.            C
+00004370: 4952 434c 4544 2044 4947 4954 204e 494e  IRCLED DIGIT NIN
+00004380: 452c 3933 3230 2c39 0a20 2020 2020 2020  E,9320,9.       
+00004390: 2020 2020 2043 4952 434c 4544 2044 4947       CIRCLED DIG
+000043a0: 4954 205a 4552 4f2c 3934 3530 2c30 0a20  IT ZERO,9450,0. 
+000043b0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+000043c0: 0a0a 2020 2020 2020 2020 6f6e 6573 203d  ..        ones =
+000043d0: 2075 6e69 636f 6465 5f6e 756d 6265 7273   unicode_numbers
+000043e0: 2e77 6865 7265 286e 616d 653d 6c74 2e54  .where(name=lt.T
+000043f0: 6162 6c65 2e65 6e64 7377 6974 6828 224f  able.endswith("O
+00004400: 4e45 2229 290a 2020 2020 2020 2020 7365  NE")).        se
+00004410: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00004420: 2c20 6c65 6e28 6f6e 6573 2929 0a0a 2020  , len(ones))..  
+00004430: 2020 2020 2020 7375 7065 7273 203d 2075        supers = u
+00004440: 6e69 636f 6465 5f6e 756d 6265 7273 2e77  nicode_numbers.w
+00004450: 6865 7265 286e 616d 653d 6c74 2e54 6162  here(name=lt.Tab
+00004460: 6c65 2e73 7461 7274 7377 6974 6828 2253  le.startswith("S
+00004470: 5550 4552 5343 5249 5054 2229 290a 2020  UPERSCRIPT")).  
+00004480: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00004490: 7445 7175 616c 2831 302c 206c 656e 2873  tEqual(10, len(s
+000044a0: 7570 6572 7329 290a 0a20 2020 2020 2020  upers))..       
+000044b0: 2023 2069 6d70 6f72 7420 7265 0a20 2020   # import re.   
+000044c0: 2020 2020 2023 2073 6576 656e 7320 3d20       # sevens = 
+000044d0: 756e 6963 6f64 655f 6e75 6d62 6572 732e  unicode_numbers.
+000044e0: 7768 6572 6528 6c61 6d62 6461 2072 6563  where(lambda rec
+000044f0: 3a20 7265 2e63 6f6d 7069 6c65 2872 222e  : re.compile(r".
+00004500: 2a53 4556 454e 2422 292e 6d61 7463 6828  *SEVEN$").match(
+00004510: 7265 632e 6e61 6d65 2929 0a0a 2020 2020  rec.name))..    
+00004520: 2020 2020 7365 7665 6e73 203d 2075 6e69      sevens = uni
+00004530: 636f 6465 5f6e 756d 6265 7273 2e77 6865  code_numbers.whe
+00004540: 7265 286e 616d 653d 6c74 2e54 6162 6c65  re(name=lt.Table
+00004550: 2e72 655f 6d61 7463 6828 7222 2e2a 5345  .re_match(r".*SE
+00004560: 5645 4e24 2229 290a 2020 2020 2020 2020  VEN$")).        
+00004570: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00004580: 2833 2c20 6c65 6e28 7365 7665 6e73 2929  (3, len(sevens))
+00004590: 0a0a 2020 2020 2020 2020 2320 6d61 6b65  ..        # make
+000045a0: 206e 616d 6573 2061 6c6c 2074 6974 6c65   names all title
+000045b0: 2063 6173 650a 2020 2020 2020 2020 756e   case.        un
+000045c0: 6963 6f64 655f 6e75 6d62 6572 732e 6164  icode_numbers.ad
+000045d0: 645f 6669 656c 6428 226e 616d 6522 2c20  d_field("name", 
+000045e0: 6c61 6d62 6461 2072 6563 3a20 7265 632e  lambda rec: rec.
+000045f0: 6e61 6d65 2e74 6974 6c65 2829 290a 2020  name.title()).  
+00004600: 2020 2020 2020 2320 7573 6520 7265 6765        # use rege
+00004610: 7820 7769 7468 2072 6520 666c 6167 0a20  x with re flag. 
+00004620: 2020 2020 2020 2069 6d70 6f72 7420 7265         import re
+00004630: 0a20 2020 2020 2020 2063 6972 636c 6564  .        circled
+00004640: 203d 2075 6e69 636f 6465 5f6e 756d 6265   = unicode_numbe
+00004650: 7273 2e77 6865 7265 286e 616d 653d 6c74  rs.where(name=lt
+00004660: 2e54 6162 6c65 2e72 655f 6d61 7463 6828  .Table.re_match(
+00004670: 7222 6369 7263 6c65 6422 2c20 666c 6167  r"circled", flag
+00004680: 733d 7265 2e49 2929 0a20 2020 2020 2020  s=re.I)).       
+00004690: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000046a0: 6c28 3130 2c20 6c65 6e28 6369 7263 6c65  l(10, len(circle
+000046b0: 6429 290a 0a20 2020 2064 6566 2074 6573  d))..    def tes
+000046c0: 745f 7768 6572 655f 6174 7472 5f66 756e  t_where_attr_fun
+000046d0: 6374 696f 6e28 7365 6c66 293a 0a20 2020  ction(self):.   
+000046e0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+000046f0: 2038 0a20 2020 2020 2020 2074 6162 6c65   8.        table
+00004700: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00004710: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+00004720: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+00004730: 697a 6529 0a0a 2020 2020 2020 2020 6465  ize)..        de
+00004740: 6620 6973 5f6f 6464 2878 293a 0a20 2020  f is_odd(x):.   
+00004750: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004760: 626f 6f6c 2878 2025 2032 290a 0a20 2020  bool(x % 2)..   
+00004770: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00004780: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
+00004790: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
+000047a0: 697a 652f 2f32 2c20 6c65 6e28 7461 626c  ize//2, len(tabl
+000047b0: 652e 7768 6572 6528 613d 6973 5f6f 6464  e.where(a=is_odd
+000047c0: 2929 290a 0a20 2020 2064 6566 2074 6573  )))..    def tes
+000047d0: 745f 6765 745f 736c 6963 6528 7365 6c66  t_get_slice(self
+000047e0: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+000047f0: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00004800: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00004810: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00004820: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00004830: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+00004840: 2020 2020 2073 7562 7461 626c 6520 3d20       subtable = 
+00004850: 7461 626c 655b 303a 3a74 6573 745f 7369  table[0::test_si
+00004860: 7a65 5d0a 2020 2020 2020 2020 7365 6c66  ze].        self
+00004870: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00004880: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
+00004890: 7a65 2c20 6c65 6e28 7375 6274 6162 6c65  ze, len(subtable
+000048a0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+000048b0: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
+000048c0: 0a20 2020 2020 2020 2063 6861 7273 203d  .        chars =
+000048d0: 2022 4142 4344 4546 4748 494a 4b4c 4d4e   "ABCDEFGHIJKLMN
+000048e0: 4f50 5152 5354 5556 5758 595a 220a 2020  OPQRSTUVWXYZ".  
+000048f0: 2020 2020 2020 6d61 6b65 5f72 6563 203d        make_rec =
+00004900: 206c 616d 6264 6120 6161 2c20 6262 2c20   lambda aa, bb, 
+00004910: 6363 3a20 7365 6c66 2e6d 616b 655f 6461  cc: self.make_da
+00004920: 7461 5f6f 626a 6563 7428 6368 6172 735b  ta_object(chars[
+00004930: 6161 5d2c 2063 6861 7273 5b62 625d 2c20  aa], chars[bb], 
+00004940: 6368 6172 735b 6363 5d29 0a20 2020 2020  chars[cc]).     
+00004950: 2020 2074 6573 745f 7369 7a65 203d 2031     test_size = 1
+00004960: 300a 2020 2020 2020 2020 7461 626c 6520  0.        table 
+00004970: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00004980: 6528 6d61 6b65 5f72 6563 2c20 7465 7374  e(make_rec, test
+00004990: 5f73 697a 6529 0a20 2020 2020 2020 2074  _size).        t
+000049a0: 6162 6c65 2e63 7265 6174 655f 696e 6465  able.create_inde
+000049b0: 7828 2761 2729 0a0a 2020 2020 2020 2020  x('a')..        
+000049c0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+000049d0: 2741 2720 696e 2074 6162 6c65 2e62 792e  'A' in table.by.
+000049e0: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+000049f0: 6173 7365 7274 5472 7565 2827 4141 2720  assertTrue('AA' 
+00004a00: 6e6f 7420 696e 2074 6162 6c65 2e62 792e  not in table.by.
+00004a10: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+00004a20: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+00004a30: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00004a40: 652c 206c 656e 2874 6162 6c65 2e62 792e  e, len(table.by.
+00004a50: 615b 2742 275d 2929 0a20 2020 2020 2020  a['B'])).       
+00004a60: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00004a70: 2869 7369 6e73 7461 6e63 6528 7461 626c  (isinstance(tabl
+00004a80: 652e 6279 2e61 5b27 4227 5d2c 206c 742e  e.by.a['B'], lt.
+00004a90: 5461 626c 6529 290a 2020 2020 2020 2020  Table)).        
+00004aa0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00004ab0: 5261 6973 6573 2841 7474 7269 6275 7465  Raises(Attribute
+00004ac0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+00004ad0: 2020 2020 7461 626c 652e 6279 2e7a 0a0a      table.by.z..
+00004ae0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00004af0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+00004b00: 7a65 2c20 6c65 6e28 7461 626c 652e 6279  ze, len(table.by
+00004b10: 2e61 2e6b 6579 7328 2929 290a 0a20 2020  .a.keys()))..   
+00004b20: 2064 6566 2074 6573 745f 756e 6971 7565   def test_unique
+00004b30: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
+00004b40: 0a20 2020 2020 2020 2063 6861 7273 203d  .        chars =
+00004b50: 2022 4142 4344 4546 4748 494a 4b4c 4d4e   "ABCDEFGHIJKLMN
+00004b60: 4f50 5152 5354 5556 5758 595a 220a 2020  OPQRSTUVWXYZ".  
+00004b70: 2020 2020 2020 6d61 6b65 5f75 6e69 7175        make_uniqu
+00004b80: 655f 6b65 7920 3d20 6c61 6d62 6461 202a  e_key = lambda *
+00004b90: 6172 6773 3a20 2727 2e6a 6f69 6e28 6368  args: ''.join(ch
+00004ba0: 6172 735b 6172 675d 2066 6f72 2061 7267  ars[arg] for arg
+00004bb0: 2069 6e20 6172 6773 290a 2020 2020 2020   in args).      
+00004bc0: 2020 6d61 6b65 5f72 6563 203d 206c 616d    make_rec = lam
+00004bd0: 6264 6120 6161 2c20 6262 2c20 6363 3a20  bda aa, bb, cc: 
+00004be0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+00004bf0: 626a 6563 7428 6d61 6b65 5f75 6e69 7175  bject(make_uniqu
+00004c00: 655f 6b65 7928 6161 2c20 6262 2c20 6363  e_key(aa, bb, cc
+00004c10: 292c 2063 6861 7273 5b62 625d 2c20 6368  ), chars[bb], ch
+00004c20: 6172 735b 6363 5d29 0a20 2020 2020 2020  ars[cc]).       
+00004c30: 2074 6573 745f 7369 7a65 203d 2031 300a   test_size = 10.
+00004c40: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+00004c50: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+00004c60: 6d61 6b65 5f72 6563 2c20 7465 7374 5f73  make_rec, test_s
+00004c70: 697a 6529 2822 5461 626c 655f 3122 290a  ize)("Table_1").
+00004c80: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
+00004c90: 6561 7465 5f69 6e64 6578 2827 6127 2c20  eate_index('a', 
+00004ca0: 756e 6971 7565 3d54 7275 6529 0a20 2020  unique=True).   
+00004cb0: 2020 2020 2072 6563 5f74 7970 6520 3d20       rec_type = 
+00004cc0: 7479 7065 2873 656c 662e 6d61 6b65 5f64  type(self.make_d
+00004cd0: 6174 615f 6f62 6a65 6374 2830 2c20 302c  ata_object(0, 0,
+00004ce0: 2030 2929 0a0a 2020 2020 2020 2020 7365   0))..        se
+00004cf0: 6c66 2e61 7373 6572 7454 7275 6528 2741  lf.assertTrue('A
+00004d00: 4141 2720 696e 2074 6162 6c65 2e62 792e  AA' in table.by.
+00004d10: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+00004d20: 6173 7365 7274 5472 7565 2827 4141 2720  assertTrue('AA' 
+00004d30: 6e6f 7420 696e 2074 6162 6c65 2e62 792e  not in table.by.
+00004d40: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+00004d50: 6173 7365 7274 5472 7565 2869 7369 6e73  assertTrue(isins
+00004d60: 7461 6e63 6528 7461 626c 652e 6279 2e61  tance(table.by.a
+00004d70: 5b27 4241 4127 5d2c 2072 6563 5f74 7970  ['BAA'], rec_typ
+00004d80: 6529 290a 2020 2020 2020 2020 7769 7468  e)).        with
+00004d90: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00004da0: 6573 284b 6579 4572 726f 7229 3a0a 2020  es(KeyError):.  
+00004db0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
+00004dc0: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
+00004dd0: 5f64 6174 615f 6f62 6a65 6374 284e 6f6e  _data_object(Non
+00004de0: 652c 204e 6f6e 652c 204e 6f6e 6529 290a  e, None, None)).
+00004df0: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
+00004e00: 6520 6475 706c 6963 6174 6520 696e 6465  e duplicate inde
+00004e10: 780a 2020 2020 2020 2020 7769 7468 2073  x.        with s
+00004e20: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00004e30: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
+00004e40: 2020 2020 2020 2020 2020 7461 626c 652e            table.
+00004e50: 6372 6561 7465 5f69 6e64 6578 2827 6127  create_index('a'
+00004e60: 2c20 756e 6971 7565 3d54 7275 652c 2061  , unique=True, a
+00004e70: 6363 6570 745f 6e6f 6e65 3d54 7275 6529  ccept_none=True)
+00004e80: 0a0a 2020 2020 2020 2020 2320 6372 6561  ..        # crea
+00004e90: 7465 2075 6e69 7175 6520 696e 6465 7820  te unique index 
+00004ea0: 7468 6174 2061 6c6c 6f77 7320 4e6f 6e65  that allows None
+00004eb0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+00004ec0: 7461 626c 652e 6465 6c65 7465 5f69 6e64  table.delete_ind
+00004ed0: 6578 2827 6127 290a 2020 2020 2020 2020  ex('a').        
 00004ee0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
 00004ef0: 6578 2827 6127 2c20 756e 6971 7565 3d54  ex('a', unique=T
 00004f00: 7275 652c 2061 6363 6570 745f 6e6f 6e65  rue, accept_none
-00004f10: 3d46 616c 7365 290a 0a20 2020 2020 2020  =False)..       
-00004f20: 2074 6162 6c65 2e63 7265 6174 655f 696e   table.create_in
-00004f30: 6465 7828 2761 272c 2075 6e69 7175 653d  dex('a', unique=
-00004f40: 5472 7565 2c20 6163 6365 7074 5f6e 6f6e  True, accept_non
-00004f50: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-00004f60: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-00004f70: 6578 2827 6327 290a 0a20 2020 2020 2020  ex('c')..       
-00004f80: 2069 6d70 6f72 7420 7070 7269 6e74 0a20   import pprint. 
-00004f90: 2020 2020 2020 2069 6e66 6f20 3d20 7461         info = ta
-00004fa0: 626c 652e 696e 666f 2829 0a20 2020 2020  ble.info().     
-00004fb0: 2020 2070 7072 696e 742e 7070 7269 6e74     pprint.pprint
-00004fc0: 2869 6e66 6f29 0a20 2020 2020 2020 2073  (info).        s
-00004fd0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00004fe0: 2754 6162 6c65 5f31 272c 2069 6e66 6f5b  'Table_1', info[
-00004ff0: 276e 616d 6527 5d29 0a20 2020 2020 2020  'name']).       
-00005000: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00005010: 6c28 5b27 6127 2c20 2762 272c 2027 6327  l(['a', 'b', 'c'
-00005020: 5d2c 206c 6973 7428 736f 7274 6564 2869  ], list(sorted(i
-00005030: 6e66 6f5b 2766 6965 6c64 7327 5d29 2929  nfo['fields'])))
-00005040: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00005050: 7365 7274 4571 7561 6c28 5b28 2761 272c  sertEqual([('a',
-00005060: 2054 7275 6529 2c20 2827 6327 2c20 4661   True), ('c', Fa
-00005070: 6c73 6529 5d2c 206c 6973 7428 736f 7274  lse)], list(sort
-00005080: 6564 2869 6e66 6f5b 2769 6e64 6578 6573  ed(info['indexes
-00005090: 275d 2929 290a 2020 2020 2020 2020 7365  ']))).        se
-000050a0: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
-000050b0: 3030 312c 2069 6e66 6f5b 276c 656e 275d  001, info['len']
-000050c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000050d0: 6368 6169 6e65 645f 696e 6465 7869 6e67  chained_indexing
-000050e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000050f0: 6368 6172 7320 3d20 2241 4243 4445 4647  chars = "ABCDEFG
-00005100: 4849 4a4b 4c4d 4e4f 5051 5253 5455 5657  HIJKLMNOPQRSTUVW
-00005110: 5859 5a22 0a20 2020 2020 2020 206d 616b  XYZ".        mak
-00005120: 655f 7265 6320 3d20 6c61 6d62 6461 2061  e_rec = lambda a
-00005130: 612c 2062 622c 2063 633a 2073 656c 662e  a, bb, cc: self.
-00005140: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00005150: 2863 6861 7273 5b61 6120 2520 6c65 6e28  (chars[aa % len(
-00005160: 6368 6172 7329 5d2c 0a20 2020 2020 2020  chars)],.       
-00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2063 6861 7273 5b62 6220 2520       chars[bb % 
-000051b0: 6c65 6e28 6368 6172 7329 5d2c 0a20 2020  len(chars)],.   
-000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2020 2020 2020 2020 2063 6861 7273 5b63           chars[c
-00005200: 6320 2520 6c65 6e28 6368 6172 7329 5d29  c % len(chars)])
-00005210: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-00005220: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
-00005230: 7461 626c 6520 3d20 6d61 6b65 5f74 6573  table = make_tes
-00005240: 745f 7461 626c 6528 6d61 6b65 5f72 6563  t_table(make_rec
-00005250: 2c20 7465 7374 5f73 697a 6529 0a20 2020  , test_size).   
-00005260: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-00005270: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
-00005280: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-00005290: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
-000052a0: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-000052b0: 655f 696e 6465 7828 2763 2729 0a0a 2020  e_index('c')..  
-000052c0: 2020 2020 2020 6368 6169 6e65 645f 7461        chained_ta
-000052d0: 626c 6520 3d20 7461 626c 652e 6279 2e62  ble = table.by.b
-000052e0: 5b27 4127 5d2e 6279 2e63 5b27 4327 5d0a  ['A'].by.c['C'].
-000052f0: 2020 2020 2020 2020 666f 7220 7265 6320          for rec 
-00005300: 696e 2063 6861 696e 6564 5f74 6162 6c65  in chained_table
-00005310: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00005320: 696e 7428 7265 6329 0a0a 2020 2020 2020  int(rec)..      
-00005330: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00005340: 616c 2874 6573 745f 7369 7a65 2c20 6c65  al(test_size, le
-00005350: 6e28 6368 6169 6e65 645f 7461 626c 6529  n(chained_table)
-00005360: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00005370: 7061 7273 655f 6461 7465 7469 6d65 5f74  parse_datetime_t
-00005380: 7261 6e73 666f 726d 2873 656c 6629 3a0a  ransform(self):.
-00005390: 2020 2020 2020 2020 696d 706f 7274 2064          import d
-000053a0: 6174 6574 696d 650a 0a20 2020 2020 2020  atetime..       
-000053b0: 2064 6174 6120 3d20 7465 7874 7772 6170   data = textwrap
-000053c0: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-000053d0: 2020 2020 2061 2c62 2c63 0a20 2020 2020       a,b,c.     
-000053e0: 2020 2032 3030 312d 3031 2d30 3120 3030     2001-01-01 00
-000053f0: 3a33 343a 3536 2c41 2c31 3030 0a20 2020  :34:56,A,100.   
-00005400: 2020 2020 2032 3030 312d 3031 2d30 3220       2001-01-02 
-00005410: 3031 3a33 343a 3536 2c42 2c31 3031 0a20  01:34:56,B,101. 
-00005420: 2020 2020 2020 2032 3030 312d 3032 2d33         2001-02-3
-00005430: 3020 3032 3a33 343a 3536 2c43 2c31 3032  0 02:34:56,C,102
-00005440: 0a20 2020 2020 2020 202c 442c 3130 330a  .        ,D,103.
-00005450: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
-00005460: 2020 2020 2074 6573 745f 6b77 6172 6773       test_kwargs
-00005470: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00005480: 207b 2765 6d70 7479 273a 2027 272c 2027   {'empty': '', '
-00005490: 6f6e 5f65 7272 6f72 273a 204e 6f6e 657d  on_error': None}
-000054a0: 2c0a 2020 2020 2020 2020 2020 2020 7b27  ,.            {'
-000054b0: 656d 7074 7927 3a20 274e 2f41 272c 2027  empty': 'N/A', '
-000054c0: 6f6e 5f65 7272 6f72 273a 2064 6174 6574  on_error': datet
-000054d0: 696d 652e 6461 7465 7469 6d65 2e6d 696e  ime.datetime.min
-000054e0: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-000054f0: 2765 6d70 7479 273a 2064 6174 6574 696d  'empty': datetim
-00005500: 652e 6461 7465 7469 6d65 2e6d 696e 2c20  e.datetime.min, 
-00005510: 276f 6e5f 6572 726f 7227 3a20 2727 7d2c  'on_error': ''},
-00005520: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00005530: 2020 2066 6f72 206b 7761 7267 7320 696e     for kwargs in
-00005540: 2074 6573 745f 6b77 6172 6773 3a0a 2020   test_kwargs:.  
-00005550: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
-00005560: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00005570: 6d70 6f72 7428 6461 7461 2c0a 2020 2020  mport(data,.    
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
-000055b0: 2761 273a 206c 742e 5461 626c 652e 7061  'a': lt.Table.pa
-000055c0: 7273 655f 6461 7465 7469 6d65 2827 2559  rse_datetime('%Y
-000055d0: 2d25 6d2d 2564 2025 483a 254d 3a25 5327  -%m-%d %H:%M:%S'
-000055e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 202a 2a6b 7761 7267 7329 7d29 0a20     **kwargs)}). 
-00005640: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00005650: 285b 7374 7228 6129 2066 6f72 2061 2069  ([str(a) for a i
-00005660: 6e20 7462 6c2e 616c 6c2e 615d 290a 0a20  n tbl.all.a]).. 
-00005670: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00005680: 7365 6c66 2e73 7562 5465 7374 2822 7465  self.subTest("te
-00005690: 7374 2054 6162 6c65 2e70 6172 7365 5f64  st Table.parse_d
-000056a0: 6174 655f 7469 6d65 2065 7272 6f72 7322  ate_time errors"
-000056b0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-000056c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000056d0: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 205b 6b77 6172 6773 5b22 6f6e 5f65     [kwargs["on_e
-00005700: 7272 6f72 225d 2c20 6b77 6172 6773 5b22  rror"], kwargs["
-00005710: 656d 7074 7922 5d5d 2c0a 2020 2020 2020  empty"]],.      
-00005720: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00005730: 7374 2874 626c 2e61 6c6c 2e61 295b 2d32  st(tbl.all.a)[-2
-00005740: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
-00005750: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00005760: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00005770: 6573 7428 2274 6573 7420 5461 626c 652e  est("test Table.
-00005780: 7061 7273 655f 6461 7465 5f74 696d 6520  parse_date_time 
-00005790: 7661 6c69 6422 2c20 2a2a 6b77 6172 6773  valid", **kwargs
-000057a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000057b0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000057c0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-000057d0: 2020 2020 2020 2020 205b 6461 7465 7469           [dateti
-000057e0: 6d65 2e64 6174 6574 696d 6528 3230 3031  me.datetime(2001
-000057f0: 2c20 312c 2031 2c20 302c 2033 342c 2035  , 1, 1, 0, 34, 5
-00005800: 3629 2c0a 2020 2020 2020 2020 2020 2020  6),.            
-00005810: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
-00005820: 652e 6461 7465 7469 6d65 2832 3030 312c  e.datetime(2001,
-00005830: 2031 2c20 322c 2031 2c20 3334 2c20 3536   1, 2, 1, 34, 56
-00005840: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-00005850: 2020 2020 2020 2020 6c69 7374 2874 626c          list(tbl
-00005860: 2e61 6c6c 2e61 295b 3a32 5d0a 2020 2020  .all.a)[:2].    
-00005870: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00005880: 2020 2064 6566 2074 6573 745f 7061 7273     def test_pars
-00005890: 655f 6461 7465 5f74 7261 6e73 666f 726d  e_date_transform
-000058a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000058b0: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
-000058c0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000058d0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-000058e0: 2222 225c 0a20 2020 2020 2020 2061 2c62  """\.        a,b
-000058f0: 2c63 0a20 2020 2020 2020 2032 3030 312d  ,c.        2001-
-00005900: 3031 2d30 3120 3030 3a33 343a 3536 2c41  01-01 00:34:56,A
-00005910: 2c31 3030 0a20 2020 2020 2020 2032 3030  ,100.        200
-00005920: 312d 3031 2d30 3220 3031 3a33 343a 3536  1-01-02 01:34:56
-00005930: 2c42 2c31 3031 0a20 2020 2020 2020 2032  ,B,101.        2
-00005940: 3030 312d 3032 2d33 3020 3032 3a33 343a  001-02-30 02:34:
-00005950: 3536 2c43 2c31 3032 0a20 2020 2020 2020  56,C,102.       
-00005960: 202c 442c 3130 330a 2020 2020 2020 2020   ,D,103.        
-00005970: 2222 2229 0a20 2020 2020 2020 2074 6573  """).        tes
-00005980: 745f 6b77 6172 6773 203d 205b 0a20 2020  t_kwargs = [.   
-00005990: 2020 2020 2020 2020 207b 2765 6d70 7479           {'empty
-000059a0: 273a 2027 272c 2027 6f6e 5f65 7272 6f72  ': '', 'on_error
-000059b0: 273a 204e 6f6e 657d 2c0a 2020 2020 2020  ': None},.      
-000059c0: 2020 2020 2020 7b27 656d 7074 7927 3a20        {'empty': 
-000059d0: 274e 2f41 272c 2027 6f6e 5f65 7272 6f72  'N/A', 'on_error
-000059e0: 273a 2064 6174 6574 696d 652e 6461 7465  ': datetime.date
-000059f0: 2e6d 696e 7d2c 0a20 2020 2020 2020 2020  .min},.         
-00005a00: 2020 207b 2765 6d70 7479 273a 2064 6174     {'empty': dat
-00005a10: 6574 696d 652e 6461 7465 2e6d 696e 2c20  etime.date.min, 
-00005a20: 276f 6e5f 6572 726f 7227 3a20 2727 7d2c  'on_error': ''},
-00005a30: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00005a40: 2020 2066 6f72 206b 7761 7267 7320 696e     for kwargs in
-00005a50: 2074 6573 745f 6b77 6172 6773 3a0a 2020   test_kwargs:.  
-00005a60: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
-00005a70: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00005a80: 6d70 6f72 7428 6461 7461 2c0a 2020 2020  mport(data,.    
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
-00005ac0: 2761 273a 206c 742e 5461 626c 652e 7061  'a': lt.Table.pa
-00005ad0: 7273 655f 6461 7465 2827 2559 2d25 6d2d  rse_date('%Y-%m-
-00005ae0: 2564 2025 483a 254d 3a25 5327 2c0a 2020  %d %H:%M:%S',.  
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00005b40: 7267 7329 7d29 0a20 2020 2020 2020 2020  rgs)}).         
-00005b50: 2020 2070 7269 6e74 285b 7374 7228 6129     print([str(a)
-00005b60: 2066 6f72 2061 2069 6e20 7462 6c2e 616c   for a in tbl.al
-00005b70: 6c2e 615d 290a 0a20 2020 2020 2020 2020  l.a])..         
-00005b80: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00005b90: 5465 7374 2822 7465 7374 2054 6162 6c65  Test("test Table
-00005ba0: 2e70 6172 7365 5f64 6174 655f 7469 6d65  .parse_date_time
-00005bb0: 2065 7272 6f72 7322 2c20 2a2a 6b77 6172   errors", **kwar
-00005bc0: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
-00005bd0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00005be0: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
-00005bf0: 2020 2020 2020 2020 2020 205b 6b77 6172             [kwar
-00005c00: 6773 5b22 6f6e 5f65 7272 6f72 225d 2c20  gs["on_error"], 
-00005c10: 6b77 6172 6773 5b22 656d 7074 7922 5d5d  kwargs["empty"]]
-00005c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005c30: 2020 2020 2020 6c69 7374 2874 626c 2e61        list(tbl.a
-00005c40: 6c6c 2e61 295b 2d32 3a5d 0a20 2020 2020  ll.a)[-2:].     
-00005c50: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00005c60: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-00005c70: 656c 662e 7375 6254 6573 7428 2274 6573  elf.subTest("tes
-00005c80: 7420 5461 626c 652e 7061 7273 655f 6461  t Table.parse_da
-00005c90: 7465 5f74 696d 6520 7661 6c69 6422 2c20  te_time valid", 
-00005ca0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00005cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005cc0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 205b 6461 7465 7469 6d65 2e64 6174 6528   [datetime.date(
-00005cf0: 3230 3031 2c20 312c 2031 292c 0a20 2020  2001, 1, 1),.   
+00004f10: 3d54 7275 6529 0a20 2020 2020 2020 2074  =True).        t
+00004f20: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
+00004f30: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00004f40: 7428 4e6f 6e65 2c20 4e6f 6e65 2c20 2741  t(None, None, 'A
+00004f50: 2729 290a 0a20 2020 2020 2020 2073 7472  '))..        str
+00004f60: 5f6e 6f6e 655f 636f 6d70 6172 6520 3d20  _none_compare = 
+00004f70: 6c61 6d62 6461 2078 3a20 7820 6966 2069  lambda x: x if i
+00004f80: 7369 6e73 7461 6e63 6528 782c 2073 7472  sinstance(x, str
+00004f90: 2920 656c 7365 2063 6872 2832 3535 292a  ) else chr(255)*
+00004fa0: 3130 300a 2020 2020 2020 2020 7365 6c66  100.        self
+00004fb0: 2e61 7373 6572 7445 7175 616c 2873 6f72  .assertEqual(sor
+00004fc0: 7465 6428 7461 626c 652e 6279 2e61 2e6b  ted(table.by.a.k
+00004fd0: 6579 7328 292c 206b 6579 3d73 7472 5f6e  eys(), key=str_n
+00004fe0: 6f6e 655f 636f 6d70 6172 6529 2c0a 2020  one_compare),.  
+00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005000: 2020 2020 2020 2073 6f72 7465 6428 7461         sorted(ta
+00005010: 626c 652e 616c 6c2e 612c 206b 6579 3d73  ble.all.a, key=s
+00005020: 7472 5f6e 6f6e 655f 636f 6d70 6172 6529  tr_none_compare)
+00005030: 290a 0a20 2020 2020 2020 2023 206e 6f77  )..        # now
+00005040: 2064 726f 7020 696e 6465 7820 616e 6420   drop index and 
+00005050: 7265 6372 6561 7465 206e 6f74 2070 6572  recreate not per
+00005060: 6d69 7474 696e 6720 4e6f 6e65 2c20 7368  mitting None, sh
+00005070: 6f75 6c64 2072 6169 7365 2065 7863 6570  ould raise excep
+00005080: 7469 6f6e 0a20 2020 2020 2020 2074 6162  tion.        tab
+00005090: 6c65 2e64 656c 6574 655f 696e 6465 7828  le.delete_index(
+000050a0: 2761 2729 0a20 2020 2020 2020 2077 6974  'a').        wit
+000050b0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+000050c0: 7365 7328 4b65 7945 7272 6f72 293a 0a20  ses(KeyError):. 
+000050d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000050e0: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
+000050f0: 272c 2075 6e69 7175 653d 5472 7565 2c20  ', unique=True, 
+00005100: 6163 6365 7074 5f6e 6f6e 653d 4661 6c73  accept_none=Fals
+00005110: 6529 0a0a 2020 2020 2020 2020 7461 626c  e)..        tabl
+00005120: 652e 6372 6561 7465 5f69 6e64 6578 2827  e.create_index('
+00005130: 6127 2c20 756e 6971 7565 3d54 7275 652c  a', unique=True,
+00005140: 2061 6363 6570 745f 6e6f 6e65 3d54 7275   accept_none=Tru
+00005150: 6529 0a20 2020 2020 2020 2074 6162 6c65  e).        table
+00005160: 2e63 7265 6174 655f 696e 6465 7828 2763  .create_index('c
+00005170: 2729 0a0a 2020 2020 2020 2020 696d 706f  ')..        impo
+00005180: 7274 2070 7072 696e 740a 2020 2020 2020  rt pprint.      
+00005190: 2020 696e 666f 203d 2074 6162 6c65 2e69    info = table.i
+000051a0: 6e66 6f28 290a 2020 2020 2020 2020 7070  nfo().        pp
+000051b0: 7269 6e74 2e70 7072 696e 7428 696e 666f  rint.pprint(info
+000051c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000051d0: 7373 6572 7445 7175 616c 2827 5461 626c  ssertEqual('Tabl
+000051e0: 655f 3127 2c20 696e 666f 5b27 6e61 6d65  e_1', info['name
+000051f0: 275d 290a 2020 2020 2020 2020 7365 6c66  ']).        self
+00005200: 2e61 7373 6572 7445 7175 616c 285b 2761  .assertEqual(['a
+00005210: 272c 2027 6227 2c20 2763 275d 2c20 6c69  ', 'b', 'c'], li
+00005220: 7374 2873 6f72 7465 6428 696e 666f 5b27  st(sorted(info['
+00005230: 6669 656c 6473 275d 2929 290a 2020 2020  fields']))).    
+00005240: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00005250: 7175 616c 285b 2827 6127 2c20 5472 7565  qual([('a', True
+00005260: 292c 2028 2763 272c 2046 616c 7365 295d  ), ('c', False)]
+00005270: 2c20 6c69 7374 2873 6f72 7465 6428 696e  , list(sorted(in
+00005280: 666f 5b27 696e 6465 7865 7327 5d29 2929  fo['indexes'])))
+00005290: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000052a0: 7365 7274 4571 7561 6c28 3130 3031 2c20  sertEqual(1001, 
+000052b0: 696e 666f 5b27 6c65 6e27 5d29 0a0a 2020  info['len'])..  
+000052c0: 2020 6465 6620 7465 7374 5f63 6861 696e    def test_chain
+000052d0: 6564 5f69 6e64 6578 696e 6728 7365 6c66  ed_indexing(self
+000052e0: 293a 0a20 2020 2020 2020 2063 6861 7273  ):.        chars
+000052f0: 203d 2022 4142 4344 4546 4748 494a 4b4c   = "ABCDEFGHIJKL
+00005300: 4d4e 4f50 5152 5354 5556 5758 595a 220a  MNOPQRSTUVWXYZ".
+00005310: 2020 2020 2020 2020 6d61 6b65 5f72 6563          make_rec
+00005320: 203d 206c 616d 6264 6120 6161 2c20 6262   = lambda aa, bb
+00005330: 2c20 6363 3a20 7365 6c66 2e6d 616b 655f  , cc: self.make_
+00005340: 6461 7461 5f6f 626a 6563 7428 6368 6172  data_object(char
+00005350: 735b 6161 2025 206c 656e 2863 6861 7273  s[aa % len(chars
+00005360: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 6368 6172 735b 6262 2025 206c 656e 2863  chars[bb % len(c
+000053b0: 6861 7273 295d 2c0a 2020 2020 2020 2020  hars)],.        
+000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053f0: 2020 2020 6368 6172 735b 6363 2025 206c      chars[cc % l
+00005400: 656e 2863 6861 7273 295d 290a 2020 2020  en(chars)]).    
+00005410: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+00005420: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
+00005430: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00005440: 6c65 286d 616b 655f 7265 632c 2074 6573  le(make_rec, tes
+00005450: 745f 7369 7a65 290a 2020 2020 2020 2020  t_size).        
+00005460: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+00005470: 6578 2827 6127 290a 2020 2020 2020 2020  ex('a').        
+00005480: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+00005490: 6578 2827 6227 290a 2020 2020 2020 2020  ex('b').        
+000054a0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+000054b0: 6578 2827 6327 290a 0a20 2020 2020 2020  ex('c')..       
+000054c0: 2063 6861 696e 6564 5f74 6162 6c65 203d   chained_table =
+000054d0: 2074 6162 6c65 2e62 792e 625b 2741 275d   table.by.b['A']
+000054e0: 2e62 792e 635b 2743 275d 0a20 2020 2020  .by.c['C'].     
+000054f0: 2020 2066 6f72 2072 6563 2069 6e20 6368     for rec in ch
+00005500: 6169 6e65 645f 7461 626c 653a 0a20 2020  ained_table:.   
+00005510: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
+00005520: 6563 290a 0a20 2020 2020 2020 2073 656c  ec)..        sel
+00005530: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
+00005540: 7374 5f73 697a 652c 206c 656e 2863 6861  st_size, len(cha
+00005550: 696e 6564 5f74 6162 6c65 2929 0a0a 2020  ined_table))..  
+00005560: 2020 6465 6620 7465 7374 5f70 6172 7365    def test_parse
+00005570: 5f64 6174 6574 696d 655f 7472 616e 7366  _datetime_transf
+00005580: 6f72 6d28 7365 6c66 293a 0a20 2020 2020  orm(self):.     
+00005590: 2020 2069 6d70 6f72 7420 6461 7465 7469     import dateti
+000055a0: 6d65 0a0a 2020 2020 2020 2020 6461 7461  me..        data
+000055b0: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+000055c0: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+000055d0: 612c 622c 630a 2020 2020 2020 2020 3230  a,b,c.        20
+000055e0: 3031 2d30 312d 3031 2030 303a 3334 3a35  01-01-01 00:34:5
+000055f0: 362c 412c 3130 300a 2020 2020 2020 2020  6,A,100.        
+00005600: 3230 3031 2d30 312d 3032 2030 313a 3334  2001-01-02 01:34
+00005610: 3a35 362c 422c 3130 310a 2020 2020 2020  :56,B,101.      
+00005620: 2020 3230 3031 2d30 322d 3330 2030 323a    2001-02-30 02:
+00005630: 3334 3a35 362c 432c 3130 320a 2020 2020  34:56,C,102.    
+00005640: 2020 2020 2c44 2c31 3033 0a20 2020 2020      ,D,103.     
+00005650: 2020 2022 2222 290a 2020 2020 2020 2020     """).        
+00005660: 7465 7374 5f6b 7761 7267 7320 3d20 5b0a  test_kwargs = [.
+00005670: 2020 2020 2020 2020 2020 2020 7b27 656d              {'em
+00005680: 7074 7927 3a20 2727 2c20 276f 6e5f 6572  pty': '', 'on_er
+00005690: 726f 7227 3a20 4e6f 6e65 7d2c 0a20 2020  ror': None},.   
+000056a0: 2020 2020 2020 2020 207b 2765 6d70 7479           {'empty
+000056b0: 273a 2027 4e2f 4127 2c20 276f 6e5f 6572  ': 'N/A', 'on_er
+000056c0: 726f 7227 3a20 6461 7465 7469 6d65 2e64  ror': datetime.d
+000056d0: 6174 6574 696d 652e 6d69 6e7d 2c0a 2020  atetime.min},.  
+000056e0: 2020 2020 2020 2020 2020 7b27 656d 7074            {'empt
+000056f0: 7927 3a20 6461 7465 7469 6d65 2e64 6174  y': datetime.dat
+00005700: 6574 696d 652e 6d69 6e2c 2027 6f6e 5f65  etime.min, 'on_e
+00005710: 7272 6f72 273a 2027 277d 2c0a 2020 2020  rror': ''},.    
+00005720: 2020 2020 5d0a 2020 2020 2020 2020 666f      ].        fo
+00005730: 7220 6b77 6172 6773 2069 6e20 7465 7374  r kwargs in test
+00005740: 5f6b 7761 7267 733a 0a20 2020 2020 2020  _kwargs:.       
+00005750: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+00005760: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00005770: 2864 6174 612c 0a20 2020 2020 2020 2020  (data,.         
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000057a0: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
+000057b0: 6c74 2e54 6162 6c65 2e70 6172 7365 5f64  lt.Table.parse_d
+000057c0: 6174 6574 696d 6528 2725 592d 256d 2d25  atetime('%Y-%m-%
+000057d0: 6420 2548 3a25 4d3a 2553 272c 0a20 2020  d %H:%M:%S',.   
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+00005830: 6b77 6172 6773 297d 290a 2020 2020 2020  kwargs)}).      
+00005840: 2020 2020 2020 7072 696e 7428 5b73 7472        print([str
+00005850: 2861 2920 666f 7220 6120 696e 2074 626c  (a) for a in tbl
+00005860: 2e61 6c6c 2e61 5d29 0a0a 2020 2020 2020  .all.a])..      
+00005870: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00005880: 7375 6254 6573 7428 2274 6573 7420 5461  subTest("test Ta
+00005890: 626c 652e 7061 7273 655f 6461 7465 5f74  ble.parse_date_t
+000058a0: 696d 6520 6572 726f 7273 222c 202a 2a6b  ime errors", **k
+000058b0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+000058c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000058d0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+000058e0: 2020 2020 2020 2020 2020 2020 2020 5b6b                [k
+000058f0: 7761 7267 735b 226f 6e5f 6572 726f 7222  wargs["on_error"
+00005900: 5d2c 206b 7761 7267 735b 2265 6d70 7479  ], kwargs["empty
+00005910: 225d 5d2c 0a20 2020 2020 2020 2020 2020  "]],.           
+00005920: 2020 2020 2020 2020 206c 6973 7428 7462           list(tb
+00005930: 6c2e 616c 6c2e 6129 5b2d 323a 5d0a 2020  l.all.a)[-2:].  
+00005940: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00005950: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00005960: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+00005970: 7465 7374 2054 6162 6c65 2e70 6172 7365  test Table.parse
+00005980: 5f64 6174 655f 7469 6d65 2076 616c 6964  _date_time valid
+00005990: 222c 202a 2a6b 7761 7267 7329 3a0a 2020  ", **kwargs):.  
+000059a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000059b0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 2020 2020 5b64 6174 6574 696d 652e 6461      [datetime.da
+000059e0: 7465 7469 6d65 2832 3030 312c 2031 2c20  tetime(2001, 1, 
+000059f0: 312c 2030 2c20 3334 2c20 3536 292c 0a20  1, 0, 34, 56),. 
+00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
+00005a20: 6574 696d 6528 3230 3031 2c20 312c 2032  etime(2001, 1, 2
+00005a30: 2c20 312c 2033 342c 2035 3629 5d2c 0a20  , 1, 34, 56)],. 
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2020 206c 6973 7428 7462 6c2e 616c 6c2e     list(tbl.all.
+00005a60: 6129 5b3a 325d 0a20 2020 2020 2020 2020  a)[:2].         
+00005a70: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00005a80: 6620 7465 7374 5f70 6172 7365 5f64 6174  f test_parse_dat
+00005a90: 655f 7472 616e 7366 6f72 6d28 7365 6c66  e_transform(self
+00005aa0: 293a 0a20 2020 2020 2020 2069 6d70 6f72  ):.        impor
+00005ab0: 7420 6461 7465 7469 6d65 0a0a 2020 2020  t datetime..    
+00005ac0: 2020 2020 6461 7461 203d 2074 6578 7477      data = textw
+00005ad0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+00005ae0: 2020 2020 2020 2020 612c 622c 630a 2020          a,b,c.  
+00005af0: 2020 2020 2020 3230 3031 2d30 312d 3031        2001-01-01
+00005b00: 2030 303a 3334 3a35 362c 412c 3130 300a   00:34:56,A,100.
+00005b10: 2020 2020 2020 2020 3230 3031 2d30 312d          2001-01-
+00005b20: 3032 2030 313a 3334 3a35 362c 422c 3130  02 01:34:56,B,10
+00005b30: 310a 2020 2020 2020 2020 3230 3031 2d30  1.        2001-0
+00005b40: 322d 3330 2030 323a 3334 3a35 362c 432c  2-30 02:34:56,C,
+00005b50: 3130 320a 2020 2020 2020 2020 2c44 2c31  102.        ,D,1
+00005b60: 3033 0a20 2020 2020 2020 2022 2222 290a  03.        """).
+00005b70: 2020 2020 2020 2020 7465 7374 5f6b 7761          test_kwa
+00005b80: 7267 7320 3d20 5b0a 2020 2020 2020 2020  rgs = [.        
+00005b90: 2020 2020 7b27 656d 7074 7927 3a20 2727      {'empty': ''
+00005ba0: 2c20 276f 6e5f 6572 726f 7227 3a20 4e6f  , 'on_error': No
+00005bb0: 6e65 7d2c 0a20 2020 2020 2020 2020 2020  ne},.           
+00005bc0: 207b 2765 6d70 7479 273a 2027 4e2f 4127   {'empty': 'N/A'
+00005bd0: 2c20 276f 6e5f 6572 726f 7227 3a20 6461  , 'on_error': da
+00005be0: 7465 7469 6d65 2e64 6174 652e 6d69 6e7d  tetime.date.min}
+00005bf0: 2c0a 2020 2020 2020 2020 2020 2020 7b27  ,.            {'
+00005c00: 656d 7074 7927 3a20 6461 7465 7469 6d65  empty': datetime
+00005c10: 2e64 6174 652e 6d69 6e2c 2027 6f6e 5f65  .date.min, 'on_e
+00005c20: 7272 6f72 273a 2027 277d 2c0a 2020 2020  rror': ''},.    
+00005c30: 2020 2020 5d0a 2020 2020 2020 2020 666f      ].        fo
+00005c40: 7220 6b77 6172 6773 2069 6e20 7465 7374  r kwargs in test
+00005c50: 5f6b 7761 7267 733a 0a20 2020 2020 2020  _kwargs:.       
+00005c60: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+00005c70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00005c80: 2864 6174 612c 0a20 2020 2020 2020 2020  (data,.         
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005cb0: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
+00005cc0: 6c74 2e54 6162 6c65 2e70 6172 7365 5f64  lt.Table.parse_d
+00005cd0: 6174 6528 2725 592d 256d 2d25 6420 2548  ate('%Y-%m-%d %H
+00005ce0: 3a25 4d3a 2553 272c 0a20 2020 2020 2020  :%M:%S',.       
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 6461 7465 7469 6d65 2e64 6174 6528    datetime.date(
-00005d20: 3230 3031 2c20 312c 2032 295d 2c0a 2020  2001, 1, 2)],.  
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 6c69 7374 2874 626c 2e61 6c6c 2e61    list(tbl.all.a
-00005d50: 295b 3a32 5d0a 2020 2020 2020 2020 2020  )[:2].          
-00005d60: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00005d70: 2074 6573 745f 7061 7273 655f 7469 6d65   test_parse_time
-00005d80: 6465 6c74 615f 7472 616e 7366 6f72 6d28  delta_transform(
-00005d90: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00005da0: 6d70 6f72 7420 6461 7465 7469 6d65 0a0a  mport datetime..
-00005db0: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
-00005dc0: 6461 7461 203d 2074 6578 7477 7261 702e  data = textwrap.
-00005dd0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
-00005de0: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
-00005df0: 7469 6d65 2c65 7170 742c 6576 656e 742c  time,eqpt,event,
-00005e00: 6c6f 742c 7069 6563 6573 0a20 2020 2020  lot,pieces.     
-00005e10: 2020 2020 2020 2030 3a30 303a 3030 2c44         0:00:00,D
-00005e20: 5249 4c4c 3031 2c4c 6f74 5374 6172 742c  RILL01,LotStart,
-00005e30: 5043 4231 3436 2c31 0a20 2020 2020 2020  PCB146,1.       
-00005e40: 2020 2020 2030 3a30 303a 3430 2c44 5249       0:00:40,DRI
-00005e50: 4c4c 3031 2c54 6f6f 6c31 2c50 4342 3134  LL01,Tool1,PCB14
-00005e60: 362c 320a 2020 2020 2020 2020 2020 2020  6,2.            
-00005e70: 303a 3033 3a34 352c 4452 494c 4c30 312c  0:03:45,DRILL01,
-00005e80: 546f 6f6c 322c 5043 4231 3436 2c34 0a20  Tool2,PCB146,4. 
-00005e90: 2020 2020 2020 2020 2020 2030 3a30 363a             0:06:
-00005ea0: 3136 2c44 5249 4c4c 3031 2c4c 6f74 456e  16,DRILL01,LotEn
-00005eb0: 642c 5043 4231 3436 2c38 0a20 2020 2020  d,PCB146,8.     
-00005ec0: 2020 2020 2020 2022 2222 290a 0a20 2020         """)..   
-00005ed0: 2020 2020 2074 7261 6e73 666f 726d 7320       transforms 
-00005ee0: 3d20 7b27 656c 6170 7365 645f 7469 6d65  = {'elapsed_time
-00005ef0: 273a 206c 742e 5461 626c 652e 7061 7273  ': lt.Table.pars
-00005f00: 655f 7469 6d65 6465 6c74 6128 2225 483a  e_timedelta("%H:
-00005f10: 254d 3a25 5322 292c 0a20 2020 2020 2020  %M:%S"),.       
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005f30: 7069 6563 6573 273a 2069 6e74 7d0a 2020  pieces': int}.  
-00005f40: 2020 2020 2020 6461 7461 203d 206c 742e        data = lt.
-00005f50: 5461 626c 6528 6622 5072 6f63 6573 7320  Table(f"Process 
-00005f60: 7374 6570 2065 6c61 7073 6564 2074 696d  step elapsed tim
-00005f70: 6573 2229 2e63 7376 5f69 6d70 6f72 7428  es").csv_import(
-00005f80: 7072 6f63 6573 735f 6461 7461 2c20 7472  process_data, tr
-00005f90: 616e 7366 6f72 6d73 3d74 7261 6e73 666f  ansforms=transfo
-00005fa0: 726d 7329 0a20 2020 2020 2020 2064 6174  rms).        dat
-00005fb0: 612e 6372 6561 7465 5f69 6e64 6578 2822  a.create_index("
-00005fc0: 656c 6170 7365 645f 7469 6d65 2229 0a0a  elapsed_time")..
-00005fd0: 2020 2020 2020 2020 5f30 305f 3031 5f33          _00_01_3
-00005fe0: 3020 3d20 6461 7465 7469 6d65 2e74 696d  0 = datetime.tim
-00005ff0: 6564 656c 7461 2873 6563 6f6e 6473 3d39  edelta(seconds=9
-00006000: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
-00006010: 6173 7365 7274 4571 7561 6c28 332c 2073  assertEqual(3, s
-00006020: 756d 2864 6174 612e 6279 2e65 6c61 7073  um(data.by.elaps
-00006030: 6564 5f74 696d 655b 3a5f 3030 5f30 315f  ed_time[:_00_01_
-00006040: 3330 5d2e 616c 6c2e 7069 6563 6573 2929  30].all.pieces))
-00006050: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
-00006060: 6c69 6365 645f 696e 6465 7869 6e67 2873  liced_indexing(s
-00006070: 656c 6629 3a0a 2020 2020 2020 2020 7472  elf):.        tr
-00006080: 616e 7366 6f72 6d73 203d 207b 0a20 2020  ansforms = {.   
-00006090: 2020 2020 2020 2020 2027 706f 7027 3a20           'pop': 
-000060a0: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-000060b0: 2027 656c 6576 273a 2069 6e74 2c0a 2020   'elev': int,.  
-000060c0: 2020 2020 2020 2020 2020 276c 6174 273a            'lat':
-000060d0: 2066 6c6f 6174 2c0a 2020 2020 2020 2020   float,.        
-000060e0: 2020 2020 276c 6f6e 6727 3a20 666c 6f61      'long': floa
-000060f0: 742c 0a20 2020 2020 2020 207d 0a20 2020  t,.        }.   
-00006100: 2020 2020 2075 735f 7070 6c20 3d20 6c74       us_ppl = lt
-00006110: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-00006120: 6f72 7428 2265 7861 6d70 6c65 732f 7573  ort("examples/us
-00006130: 5f70 706c 2e63 7376 222c 0a20 2020 2020  _ppl.csv",.     
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 7472 616e 7366 6f72 6d73 3d74 7261    transforms=tra
-00006170: 6e73 666f 726d 732c 0a20 2020 2020 2020  nsforms,.       
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 292e 7365 6c65 6374 2822 6964 206e 616d  ).select("id nam
-000061b0: 6520 656c 6576 206c 6174 206c 6f6e 6720  e elev lat long 
-000061c0: 706f 7022 290a 2020 2020 2020 2020 7072  pop").        pr
-000061d0: 696e 7428 7573 5f70 706c 2e69 6e66 6f28  int(us_ppl.info(
-000061e0: 2929 0a20 2020 2020 2020 2075 735f 7070  )).        us_pp
-000061f0: 6c2e 6372 6561 7465 5f69 6e64 6578 2822  l.create_index("
-00006200: 6e61 6d65 2229 0a20 2020 2020 2020 2075  name").        u
-00006210: 735f 7070 6c2e 6372 6561 7465 5f69 6e64  s_ppl.create_ind
-00006220: 6578 2822 656c 6576 2229 0a0a 2020 2020  ex("elev")..    
-00006230: 2020 2020 7465 7374 203d 2022 656c 6576      test = "elev
-00006240: 203c 2030 220a 2020 2020 2020 2020 6c6f   < 0".        lo
-00006250: 775f 7070 6c5f 7768 6572 6520 3d20 7573  w_ppl_where = us
-00006260: 5f70 706c 2e77 6865 7265 2865 6c65 763d  _ppl.where(elev=
-00006270: 6c74 2e54 6162 6c65 2e6c 7428 3029 2928  lt.Table.lt(0))(
-00006280: 7465 7374 290a 2020 2020 2020 2020 6c6f  test).        lo
-00006290: 775f 7070 6c5f 736c 6963 6520 3d20 7573  w_ppl_slice = us
-000062a0: 5f70 706c 2e62 792e 656c 6576 5b3a 305d  _ppl.by.elev[:0]
-000062b0: 2866 227b 7465 7374 7d20 2873 6c69 6365  (f"{test} (slice
-000062c0: 6429 2229 0a20 2020 2020 2020 206c 6f77  d)").        low
-000062d0: 5f70 706c 5f73 6c69 6365 2e70 7265 7365  _ppl_slice.prese
-000062e0: 6e74 2829 0a20 2020 2020 2020 2073 656c  nt().        sel
-000062f0: 662e 6173 7365 7274 4571 7561 6c28 6c69  f.assertEqual(li
-00006300: 7374 286c 6f77 5f70 706c 5f77 6865 7265  st(low_ppl_where
-00006310: 2e61 6c6c 2e69 6429 2c20 6c69 7374 286c  .all.id), list(l
-00006320: 6f77 5f70 706c 5f73 6c69 6365 2e61 6c6c  ow_ppl_slice.all
-00006330: 2e69 6429 290a 0a20 2020 2020 2020 2074  .id))..        t
-00006340: 6573 7420 3d20 2265 6c65 7620 3e3d 2031  est = "elev >= 1
-00006350: 3030 3022 0a20 2020 2020 2020 2068 695f  000".        hi_
-00006360: 7070 6c5f 7768 6572 6520 3d20 7573 5f70  ppl_where = us_p
-00006370: 706c 2e77 6865 7265 2865 6c65 763d 6c74  pl.where(elev=lt
-00006380: 2e54 6162 6c65 2e67 6528 3130 3030 2929  .Table.ge(1000))
-00006390: 2874 6573 7429 0a20 2020 2020 2020 2068  (test).        h
-000063a0: 695f 7070 6c5f 736c 6963 6520 3d20 7573  i_ppl_slice = us
-000063b0: 5f70 706c 2e62 792e 656c 6576 5b31 3030  _ppl.by.elev[100
-000063c0: 303a 5d28 6622 7b74 6573 747d 2028 736c  0:](f"{test} (sl
-000063d0: 6963 6564 2922 290a 2020 2020 2020 2020  iced)").        
-000063e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000063f0: 286c 6973 7428 6869 5f70 706c 5f77 6865  (list(hi_ppl_whe
-00006400: 7265 2e61 6c6c 2e69 6429 2c20 6c69 7374  re.all.id), list
-00006410: 2868 695f 7070 6c5f 736c 6963 652e 616c  (hi_ppl_slice.al
-00006420: 6c2e 6964 2929 0a0a 2020 2020 2020 2020  l.id))..        
-00006430: 7465 7374 203d 2022 3020 3c3d 2065 6c65  test = "0 <= ele
-00006440: 7620 3c20 3130 3022 0a20 2020 2020 2020  v < 100".       
-00006450: 206c 6f77 5f70 706c 5f77 6865 7265 203d   low_ppl_where =
-00006460: 2075 735f 7070 6c2e 7768 6572 6528 656c   us_ppl.where(el
-00006470: 6576 3d6c 742e 5461 626c 652e 6765 2830  ev=lt.Table.ge(0
-00006480: 2929 2e77 6865 7265 2865 6c65 763d 6c74  )).where(elev=lt
-00006490: 2e54 6162 6c65 2e6c 7428 3130 3029 2928  .Table.lt(100))(
-000064a0: 7465 7374 290a 2020 2020 2020 2020 6c6f  test).        lo
-000064b0: 775f 7070 6c5f 736c 6963 6520 3d20 7573  w_ppl_slice = us
-000064c0: 5f70 706c 2e62 792e 656c 6576 5b30 3a31  _ppl.by.elev[0:1
-000064d0: 3030 5d28 6622 7b74 6573 747d 2028 736c  00](f"{test} (sl
-000064e0: 6963 6564 2922 290a 2020 2020 2020 2020  iced)").        
-000064f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00006500: 286c 6973 7428 6c6f 775f 7070 6c5f 7768  (list(low_ppl_wh
-00006510: 6572 652e 616c 6c2e 6964 292c 206c 6973  ere.all.id), lis
-00006520: 7428 6c6f 775f 7070 6c5f 736c 6963 652e  t(low_ppl_slice.
-00006530: 616c 6c2e 6964 2929 0a0a 2020 2020 2020  all.id))..      
-00006540: 2020 615f 7070 6c5f 7768 6572 6520 3d20    a_ppl_where = 
-00006550: 7573 5f70 706c 2e77 6865 7265 286e 616d  us_ppl.where(nam
-00006560: 653d 6c74 2e54 6162 6c65 2e67 6528 2241  e=lt.Table.ge("A
-00006570: 2229 292e 7768 6572 6528 6e61 6d65 3d6c  ")).where(name=l
-00006580: 742e 5461 626c 652e 6c74 2822 4322 2929  t.Table.lt("C"))
-00006590: 0a20 2020 2020 2020 2061 5f70 706c 5f73  .        a_ppl_s
-000065a0: 6c69 6365 203d 2075 735f 7070 6c2e 6279  lice = us_ppl.by
-000065b0: 2e6e 616d 655b 2241 223a 2243 225d 0a20  .name["A":"C"]. 
-000065c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000065d0: 7274 4571 7561 6c28 6c69 7374 2861 5f70  rtEqual(list(a_p
-000065e0: 706c 5f77 6865 7265 2e61 6c6c 2e69 6429  pl_where.all.id)
-000065f0: 2c20 6c69 7374 2861 5f70 706c 5f73 6c69  , list(a_ppl_sli
-00006600: 6365 2e61 6c6c 2e69 6429 290a 0a20 2020  ce.all.id))..   
-00006610: 2064 6566 2074 6573 745f 6e6f 6e5f 696e   def test_non_in
-00006620: 7465 6765 725f 736c 6963 6564 5f69 6e64  teger_sliced_ind
-00006630: 6578 696e 6728 7365 6c66 293a 0a20 2020  exing(self):.   
-00006640: 2020 2020 2069 6d70 6f72 7420 6461 7465       import date
-00006650: 7469 6d65 0a0a 2020 2020 2020 2020 7361  time..        sa
-00006660: 6c65 735f 6461 7461 203d 2074 6578 7477  les_data = textw
-00006670: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-00006680: 2020 2020 2020 2020 2020 2020 6461 7465              date
-00006690: 2c63 7573 746f 6d65 722c 736b 752c 7174  ,customer,sku,qt
-000066a0: 790a 2020 2020 2020 2020 2020 2020 3230  y.            20
-000066b0: 3030 2f30 312f 3031 2c30 3032 302c 414e  00/01/01,0020,AN
-000066c0: 5649 4c2d 3030 312c 310a 2020 2020 2020  VIL-001,1.      
-000066d0: 2020 2020 2020 3230 3030 2f30 312f 3031        2000/01/01
-000066e0: 2c30 3032 302c 4252 4453 442d 3030 312c  ,0020,BRDSD-001,
-000066f0: 320a 2020 2020 2020 2020 2020 2020 3230  2.            20
-00006700: 3030 2f30 322f 3135 2c30 3032 302c 4252  00/02/15,0020,BR
-00006710: 4453 442d 3030 312c 340a 2020 2020 2020  DSD-001,4.      
-00006720: 2020 2020 2020 3230 3030 2f30 332f 3331        2000/03/31
-00006730: 2c30 3032 302c 4252 4453 442d 3030 312c  ,0020,BRDSD-001,
-00006740: 380a 2020 2020 2020 2020 2020 2020 3230  8.            20
-00006750: 3030 2f30 332f 3331 2c30 3032 302c 4d41  00/03/31,0020,MA
-00006760: 474e 542d 3030 312c 3136 0a20 2020 2020  GNT-001,16.     
-00006770: 2020 2020 2020 2032 3030 302f 3034 2f30         2000/04/0
-00006780: 312c 3030 3230 2c52 4f42 4f54 2d30 3031  1,0020,ROBOT-001
-00006790: 2c33 320a 2020 2020 2020 2020 2020 2020  ,32.            
-000067a0: 3230 3030 2f30 342f 3135 2c30 3032 302c  2000/04/15,0020,
-000067b0: 4252 4453 442d 3030 312c 3634 0a20 2020  BRDSD-001,64.   
-000067c0: 2020 2020 2020 2020 2022 2222 290a 0a20           """).. 
-000067d0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-000067e0: 7320 3d20 7b27 6461 7465 273a 206c 742e  s = {'date': lt.
-000067f0: 5461 626c 652e 7061 7273 655f 6461 7465  Table.parse_date
-00006800: 2822 2559 2f25 6d2f 2564 2229 2c0a 2020  ("%Y/%m/%d"),.  
-00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2771 7479 273a 2069 6e74 7d0a      'qty': int}.
-00006830: 2020 2020 2020 2020 7361 6c65 7320 3d20          sales = 
-00006840: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00006850: 6d70 6f72 7428 7361 6c65 735f 6461 7461  mport(sales_data
-00006860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00006890: 6d73 3d74 7261 6e73 666f 726d 732c 290a  ms=transforms,).
-000068a0: 0a20 2020 2020 2020 2073 616c 6573 2e63  .        sales.c
-000068b0: 7265 6174 655f 696e 6465 7828 2264 6174  reate_index("dat
-000068c0: 6522 290a 2020 2020 2020 2020 6a61 6e5f  e").        jan_
-000068d0: 3031 203d 2064 6174 6574 696d 652e 6461  01 = datetime.da
-000068e0: 7465 2832 3030 302c 2031 2c20 3129 0a20  te(2000, 1, 1). 
-000068f0: 2020 2020 2020 2061 7072 5f30 3120 3d20         apr_01 = 
-00006900: 6461 7465 7469 6d65 2e64 6174 6528 3230  datetime.date(20
-00006910: 3030 2c20 342c 2031 290a 2020 2020 2020  00, 4, 1).      
-00006920: 2020 6669 7273 745f 7174 725f 7361 6c65    first_qtr_sale
-00006930: 7320 3d20 7361 6c65 732e 6279 2e64 6174  s = sales.by.dat
-00006940: 655b 6a61 6e5f 3031 3a20 6170 725f 3031  e[jan_01: apr_01
-00006950: 5d0a 2020 2020 2020 2020 6669 7273 745f  ].        first_
-00006960: 7174 725f 7361 6c65 732e 7072 6573 656e  qtr_sales.presen
-00006970: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
-00006980: 7428 6c69 7374 2866 6972 7374 5f71 7472  t(list(first_qtr
-00006990: 5f73 616c 6573 2e61 6c6c 2e73 6b75 2929  _sales.all.sku))
-000069a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000069b0: 7373 6572 7445 7175 616c 286c 6973 7428  ssertEqual(list(
-000069c0: 6669 7273 745f 7174 725f 7361 6c65 732e  first_qtr_sales.
-000069d0: 616c 6c2e 736b 7529 2c0a 2020 2020 2020  all.sku),.      
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 205b 2741 4e56 494c 2d30 3031 272c     ['ANVIL-001',
-00006a00: 2027 4252 4453 442d 3030 3127 2c20 2742   'BRDSD-001', 'B
-00006a10: 5244 5344 2d30 3031 272c 2027 4252 4453  RDSD-001', 'BRDS
-00006a20: 442d 3030 3127 2c20 274d 4147 4e54 2d30  D-001', 'MAGNT-0
-00006a30: 3031 275d 2c0a 2020 2020 2020 2020 2020  01'],.          
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006a50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00006a60: 7365 7274 4571 7561 6c28 3331 2c20 7375  sertEqual(31, su
-00006a70: 6d28 6669 7273 745f 7174 725f 7361 6c65  m(first_qtr_sale
-00006a80: 732e 616c 6c2e 7174 7929 290a 0a20 2020  s.all.qty))..   
-00006a90: 2020 2020 2023 2075 7365 2064 6174 6520       # use date 
-00006aa0: 7374 7269 6e67 7320 6173 2072 616e 6765  strings as range
-00006ab0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00006ac0: 7472 616e 7366 6f72 6d73 203d 207b 2771  transforms = {'q
-00006ad0: 7479 273a 2069 6e74 7d0a 2020 2020 2020  ty': int}.      
-00006ae0: 2020 7361 6c65 7320 3d20 6c74 2e54 6162    sales = lt.Tab
-00006af0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00006b00: 7361 6c65 735f 6461 7461 2c0a 2020 2020  sales_data,.    
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 7472 616e 7366 6f72 6d73 3d74 7261    transforms=tra
-00006b40: 6e73 666f 726d 732c 290a 0a20 2020 2020  nsforms,)..     
-00006b50: 2020 2073 616c 6573 2e63 7265 6174 655f     sales.create_
-00006b60: 696e 6465 7828 2264 6174 6522 290a 2020  index("date").  
-00006b70: 2020 2020 2020 6669 7273 745f 7174 725f        first_qtr_
-00006b80: 7361 6c65 7320 3d20 7361 6c65 732e 6279  sales = sales.by
-00006b90: 2e64 6174 655b 2232 3030 302f 3031 2f30  .date["2000/01/0
-00006ba0: 3122 3a20 2232 3030 302f 3034 2f30 3122  1": "2000/04/01"
-00006bb0: 5d0a 2020 2020 2020 2020 6669 7273 745f  ].        first_
-00006bc0: 7174 725f 7361 6c65 732e 7072 6573 656e  qtr_sales.presen
-00006bd0: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
-00006be0: 7428 6c69 7374 2866 6972 7374 5f71 7472  t(list(first_qtr
-00006bf0: 5f73 616c 6573 2e61 6c6c 2e73 6b75 2929  _sales.all.sku))
-00006c00: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00006c10: 7373 6572 7445 7175 616c 286c 6973 7428  ssertEqual(list(
-00006c20: 6669 7273 745f 7174 725f 7361 6c65 732e  first_qtr_sales.
-00006c30: 616c 6c2e 736b 7529 2c0a 2020 2020 2020  all.sku),.      
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 205b 2741 4e56 494c 2d30 3031 272c     ['ANVIL-001',
-00006c60: 2027 4252 4453 442d 3030 3127 2c20 2742   'BRDSD-001', 'B
-00006c70: 5244 5344 2d30 3031 272c 2027 4252 4453  RDSD-001', 'BRDS
-00006c80: 442d 3030 3127 2c20 274d 4147 4e54 2d30  D-001', 'MAGNT-0
-00006c90: 3031 275d 2c0a 2020 2020 2020 2020 2020  01'],.          
-00006ca0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006cb0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00006cc0: 7365 7274 4571 7561 6c28 3331 2c20 7375  sertEqual(31, su
-00006cd0: 6d28 6669 7273 745f 7174 725f 7361 6c65  m(first_qtr_sale
-00006ce0: 732e 616c 6c2e 7174 7929 290a 0a20 2020  s.all.qty))..   
-00006cf0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006d00: 4571 7561 6c28 3331 2c20 7375 6d28 7361  Equal(31, sum(sa
-00006d10: 6c65 732e 6279 2e64 6174 655b 3a22 3230  les.by.date[:"20
-00006d20: 3030 2f30 342f 3031 225d 2e61 6c6c 2e71  00/04/01"].all.q
-00006d30: 7479 2929 0a20 2020 2020 2020 2073 656c  ty)).        sel
-00006d40: 662e 6173 7365 7274 4571 7561 6c28 3936  f.assertEqual(96
-00006d50: 2c20 7375 6d28 7361 6c65 732e 6279 2e64  , sum(sales.by.d
-00006d60: 6174 655b 2232 3030 302f 3034 2f30 3122  ate["2000/04/01"
-00006d70: 3a5d 2e61 6c6c 2e71 7479 2929 0a0a 2020  :].all.qty))..  
-00006d80: 2020 6465 6620 7465 7374 5f69 6e64 6578    def test_index
-00006d90: 5f64 6972 2873 656c 6629 3a0a 2020 2020  _dir(self):.    
-00006da0: 2020 2020 6368 6172 7320 3d20 2241 4243      chars = "ABC
-00006db0: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
-00006dc0: 5455 5657 5859 5a22 0a20 2020 2020 2020  TUVWXYZ".       
-00006dd0: 206d 616b 655f 7265 6320 3d20 6c61 6d62   make_rec = lamb
-00006de0: 6461 2061 612c 2062 622c 2063 633a 2073  da aa, bb, cc: s
-00006df0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00006e00: 6a65 6374 2863 6861 7273 5b61 6120 2520  ject(chars[aa % 
-00006e10: 6c65 6e28 6368 6172 7329 5d2c 0a20 2020  len(chars)],.   
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2020 2020 2020 2063 6861 7273 5b62           chars[b
-00006e60: 6220 2520 6c65 6e28 6368 6172 7329 5d2c  b % len(chars)],
-00006e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00006eb0: 7273 5b63 6320 2520 6c65 6e28 6368 6172  rs[cc % len(char
-00006ec0: 7329 5d29 0a20 2020 2020 2020 2074 6573  s)]).        tes
-00006ed0: 745f 7369 7a65 203d 2031 300a 2020 2020  t_size = 10.    
-00006ee0: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
-00006ef0: 5f74 6573 745f 7461 626c 6528 6d61 6b65  _test_table(make
-00006f00: 5f72 6563 2c20 7465 7374 5f73 697a 6529  _rec, test_size)
-00006f10: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-00006f20: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
-00006f30: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-00006f40: 7265 6174 655f 696e 6465 7828 2762 2729  reate_index('b')
-00006f50: 0a0a 2020 2020 2020 2020 6469 725f 6c69  ..        dir_li
-00006f60: 7374 203d 2064 6972 2874 6162 6c65 2e62  st = dir(table.b
-00006f70: 7929 0a20 2020 2020 2020 2070 7269 6e74  y).        print
-00006f80: 285b 6174 7472 2066 6f72 2061 7474 7220  ([attr for attr 
-00006f90: 696e 2064 6972 5f6c 6973 7420 6966 206e  in dir_list if n
-00006fa0: 6f74 2061 7474 722e 7374 6172 7473 7769  ot attr.startswi
-00006fb0: 7468 2822 5f22 295d 290a 0a20 2020 2020  th("_")])..     
-00006fc0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00006fd0: 7565 2828 2761 2720 696e 2064 6972 5f6c  ue(('a' in dir_l
-00006fe0: 6973 7429 2061 6e64 2028 2762 2720 696e  ist) and ('b' in
-00006ff0: 2064 6972 5f6c 6973 7429 2061 6e64 2028   dir_list) and (
-00007000: 2763 2720 6e6f 7420 696e 2064 6972 5f6c  'c' not in dir_l
-00007010: 6973 7429 290a 0a20 2020 2064 6566 2074  ist))..    def t
-00007020: 6573 745f 6465 6c65 7465 5f62 795f 6669  est_delete_by_fi
-00007030: 6c74 6572 2873 656c 6629 3a0a 2020 2020  lter(self):.    
-00007040: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00007050: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-00007060: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00007070: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-00007080: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00007090: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
-000070a0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-000070b0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-000070c0: 7a65 2c20 7461 626c 652e 6465 6c65 7465  ze, table.delete
-000070d0: 2862 3d35 2929 0a20 2020 2020 2020 2073  (b=5)).        s
-000070e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000070f0: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
-00007100: 697a 652a 2874 6573 745f 7369 7a65 2d31  ize*(test_size-1
-00007110: 292c 206c 656e 2874 6162 6c65 2929 0a20  ), len(table)). 
-00007120: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007130: 7274 4571 7561 6c28 302c 2074 6162 6c65  rtEqual(0, table
-00007140: 2e64 656c 6574 6528 623d 2d31 2929 0a20  .delete(b=-1)). 
-00007150: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007160: 7274 4571 7561 6c28 302c 2074 6162 6c65  rtEqual(0, table
-00007170: 2e64 656c 6574 6528 2929 0a0a 2020 2020  .delete())..    
-00007180: 6465 6620 7465 7374 5f72 656d 6f76 655f  def test_remove_
-00007190: 6d61 6e79 2873 656c 6629 3a0a 2020 2020  many(self):.    
-000071a0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-000071b0: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-000071c0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000071d0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000071e0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-000071f0: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
-00007200: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00007210: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-00007220: 7a65 2a74 6573 745f 7369 7a65 2f32 2c20  ze*test_size/2, 
-00007230: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00007240: 6c61 6d62 6461 2074 3a20 742e 6120 2520  lambda t: t.a % 
-00007250: 3229 2929 0a20 2020 2020 2020 2074 6162  2))).        tab
-00007260: 6c65 2e72 656d 6f76 655f 6d61 6e79 2874  le.remove_many(t
-00007270: 6162 6c65 2e77 6865 7265 286c 616d 6264  able.where(lambd
-00007280: 6120 743a 2074 2e61 2025 2032 2929 0a20  a t: t.a % 2)). 
-00007290: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000072a0: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-000072b0: 652a 7465 7374 5f73 697a 652a 7465 7374  e*test_size*test
-000072c0: 5f73 697a 652f 322c 206c 656e 2874 6162  _size/2, len(tab
-000072d0: 6c65 2929 0a20 2020 2020 2020 2074 6162  le)).        tab
-000072e0: 6c65 5f6c 656e 203d 206c 656e 2874 6162  le_len = len(tab
-000072f0: 6c65 290a 2020 2020 2020 2020 7461 626c  le).        tabl
-00007300: 652e 7265 6d6f 7665 2874 6162 6c65 5b31  e.remove(table[1
-00007310: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
-00007320: 6173 7365 7274 4571 7561 6c28 7461 626c  assertEqual(tabl
-00007330: 655f 6c65 6e2d 312c 206c 656e 2874 6162  e_len-1, len(tab
-00007340: 6c65 2929 0a0a 2020 2020 6465 6620 7465  le))..    def te
-00007350: 7374 5f61 6464 5f6e 6577 5f66 6965 6c64  st_add_new_field
-00007360: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007370: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
-00007380: 2020 2020 2020 2074 6162 6c65 203d 206d         table = m
-00007390: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000073a0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000073b0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000073c0: 0a0a 2020 2020 2020 2020 2320 6f6e 6c79  ..        # only
-000073d0: 2044 6174 614f 626a 6563 7473 2061 7265   DataObjects are
-000073e0: 206d 7574 6162 6c65 2069 6e20 7468 6573   mutable in thes
-000073f0: 6520 7465 7374 730a 2020 2020 2020 2020  e tests.        
-00007400: 6966 2069 7369 6e73 7461 6e63 6528 7461  if isinstance(ta
-00007410: 626c 655b 305d 2c20 6c74 2e44 6174 614f  ble[0], lt.DataO
-00007420: 626a 6563 7429 3a0a 2020 2020 2020 2020  bject):.        
-00007430: 2020 2020 7461 626c 652e 6164 645f 6669      table.add_fi
-00007440: 656c 6428 2764 272c 206c 616d 6264 6120  eld('d', lambda 
-00007450: 7265 633a 2072 6563 2e61 2b72 6563 2e62  rec: rec.a+rec.b
-00007460: 2b72 6563 2e63 290a 0a20 2020 2020 2020  +rec.c)..       
-00007470: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-00007480: 655f 696e 6465 7828 2764 2729 0a20 2020  e_index('d').   
-00007490: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000074a0: 7365 7274 4571 7561 6c28 6c65 6e28 7261  sertEqual(len(ra
-000074b0: 6e67 6528 302c 2032 372b 3129 292c 206c  nge(0, 27+1)), l
-000074c0: 656e 2874 6162 6c65 2e62 792e 642e 6b65  en(table.by.d.ke
-000074d0: 7973 2829 2929 0a0a 2020 2020 6465 6620  ys()))..    def 
-000074e0: 7465 7374 5f61 6464 5f74 776f 5f74 6162  test_add_two_tab
-000074f0: 6c65 7328 7365 6c66 293a 0a20 2020 2020  les(self):.     
-00007500: 2020 2074 6573 745f 7369 7a65 203d 2031     test_size = 1
-00007510: 300a 2020 2020 2020 2020 7431 203d 206d  0.        t1 = m
-00007520: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-00007530: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00007540: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-00007550: 0a20 2020 2020 2020 206d 616b 655f 7265  .        make_re
-00007560: 6320 3d20 6c61 6d62 6461 2061 2c62 2c63  c = lambda a,b,c
-00007570: 3a20 7365 6c66 2e6d 616b 655f 6461 7461  : self.make_data
-00007580: 5f6f 626a 6563 7428 612b 7465 7374 5f73  _object(a+test_s
-00007590: 697a 652c 2062 2c20 6329 0a20 2020 2020  ize, b, c).     
-000075a0: 2020 2074 3220 3d20 6d61 6b65 5f74 6573     t2 = make_tes
-000075b0: 745f 7461 626c 6528 6d61 6b65 5f72 6563  t_table(make_rec
-000075c0: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
-000075d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000075e0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-000075f0: 2a74 6573 745f 7369 7a65 2a74 6573 745f  *test_size*test_
-00007600: 7369 7a65 2a32 2c20 6c65 6e28 7431 2b74  size*2, len(t1+t
-00007610: 3229 290a 2020 2020 2020 2020 7365 6c66  2)).        self
-00007620: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00007630: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
-00007640: 7a65 202a 2074 6573 745f 7369 7a65 2c20  ze * test_size, 
-00007650: 6c65 6e28 7431 2929 0a0a 2020 2020 2020  len(t1))..      
-00007660: 2020 7431 202b 3d20 7432 0a20 2020 2020    t1 += t2.     
-00007670: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00007680: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
-00007690: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
-000076a0: 5f73 697a 6520 2a20 322c 206c 656e 2874  _size * 2, len(t
-000076b0: 3129 290a 0a20 2020 2020 2020 206f 6666  1))..        off
-000076c0: 7365 7420 3d20 7465 7374 5f73 697a 6520  set = test_size 
-000076d0: 2a20 7465 7374 5f73 697a 650a 2020 2020  * test_size.    
-000076e0: 2020 2020 7433 203d 2074 3120 2b20 2873      t3 = t1 + (s
-000076f0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00007700: 6a65 6374 2872 6563 2e61 2b6f 6666 7365  ject(rec.a+offse
-00007710: 742c 2072 6563 2e62 2c20 7265 632e 6329  t, rec.b, rec.c)
-00007720: 2066 6f72 2072 6563 2069 6e20 7432 290a   for rec in t2).
-00007730: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00007740: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00007750: 7a65 202a 2074 6573 745f 7369 7a65 202a  ze * test_size *
-00007760: 2074 6573 745f 7369 7a65 202a 2033 2c20   test_size * 3, 
-00007770: 6c65 6e28 7433 2929 0a0a 2020 2020 6465  len(t3))..    de
-00007780: 6620 7465 7374 5f74 6162 6c65 5f69 6e66  f test_table_inf
-00007790: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-000077a0: 2074 6573 745f 7369 7a65 203d 2031 300a   test_size = 10.
-000077b0: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
-000077c0: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
-000077d0: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-000077e0: 6374 2c20 7465 7374 5f73 697a 6529 2827  ct, test_size)('
-000077f0: 696e 666f 5f74 6573 7427 290a 2020 2020  info_test').    
-00007800: 2020 2020 7431 2e63 7265 6174 655f 696e      t1.create_in
-00007810: 6465 7828 2762 2729 0a20 2020 2020 2020  dex('b').       
-00007820: 2074 315f 696e 666f 203d 2074 312e 696e   t1_info = t1.in
-00007830: 666f 2829 0a20 2020 2020 2020 2023 206d  fo().        # m
-00007840: 7573 7420 736f 7274 2066 6965 6c64 7320  ust sort fields 
-00007850: 616e 6420 696e 6465 7865 7320 7661 6c75  and indexes valu
-00007860: 6573 2c20 666f 7220 7465 7374 2063 6f6d  es, for test com
-00007870: 7061 7269 736f 6e73 0a20 2020 2020 2020  parisons.       
-00007880: 2074 315f 696e 666f 5b27 6669 656c 6473   t1_info['fields
-00007890: 275d 2e73 6f72 7428 290a 2020 2020 2020  '].sort().      
-000078a0: 2020 7431 5f69 6e66 6f5b 2769 6e64 6578    t1_info['index
-000078b0: 6573 275d 2e73 6f72 7428 290a 2020 2020  es'].sort().    
-000078c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000078d0: 7175 616c 287b 2766 6965 6c64 7327 3a20  qual({'fields': 
-000078e0: 5b27 6127 2c20 2762 272c 2027 6327 5d2c  ['a', 'b', 'c'],
-000078f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007900: 2020 2020 2020 2020 2020 2027 696e 6465             'inde
-00007910: 7865 7327 3a20 5b28 2762 272c 2046 616c  xes': [('b', Fal
-00007920: 7365 295d 2c0a 2020 2020 2020 2020 2020  se)],.          
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 276c 656e 273a 2031 3030 302c 0a20 2020  'len': 1000,.   
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2027 6e61 6d65 273a 2027         'name': '
-00007970: 696e 666f 5f74 6573 7427 7d2c 0a20 2020  info_test'},.   
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 7431 5f69 6e66 6f2c 2022        t1_info, "
-000079a0: 696e 7661 6c69 6420 696e 666f 2072 6573  invalid info res
-000079b0: 756c 7473 2229 0a0a 0a40 6d61 6b65 5f74  ults")...@make_t
-000079c0: 6573 745f 636c 6173 7365 730a 636c 6173  est_classes.clas
-000079d0: 7320 5461 626c 654c 6973 7454 6573 7473  s TableListTests
-000079e0: 3a0a 2020 2020 6465 6620 5f74 6573 745f  :.    def _test_
-000079f0: 696e 6974 2873 656c 6629 3a0a 2020 2020  init(self):.    
-00007a00: 2020 2020 7365 6c66 2e74 6573 745f 7369      self.test_si
-00007a10: 7a65 203d 2033 0a20 2020 2020 2020 2073  ze = 3.        s
-00007a20: 656c 662e 7431 203d 206d 616b 655f 7465  elf.t1 = make_te
-00007a30: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-00007a40: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-00007a50: 7365 6c66 2e74 6573 745f 7369 7a65 290a  self.test_size).
-00007a60: 2020 2020 2020 2020 7365 6c66 2e74 6573          self.tes
-00007a70: 745f 7265 6320 3d20 7365 6c66 2e6d 616b  t_rec = self.mak
-00007a80: 655f 6461 7461 5f6f 626a 6563 7428 312c  e_data_object(1,
-00007a90: 2031 2c20 3129 0a0a 2020 2020 6465 6620   1, 1)..    def 
-00007aa0: 7465 7374 5f63 6f6e 7461 696e 7328 7365  test_contains(se
-00007ab0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00007ac0: 662e 5f74 6573 745f 696e 6974 2829 0a20  f._test_init(). 
-00007ad0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007ae0: 7274 5472 7565 2873 656c 662e 7465 7374  rtTrue(self.test
-00007af0: 5f72 6563 2069 6e20 7365 6c66 2e74 312c  _rec in self.t1,
-00007b00: 2022 6661 696c 6564 2027 696e 2720 2863   "failed 'in' (c
-00007b10: 6f6e 7461 696e 7329 2074 6573 7422 290a  ontains) test").
-00007b20: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
-00007b30: 6465 785f 6669 6e64 2873 656c 6629 3a0a  dex_find(self):.
-00007b40: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-00007b50: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
-00007b60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007b70: 616c 2831 332c 2073 656c 662e 7431 2e69  al(13, self.t1.i
-00007b80: 6e64 6578 2873 656c 662e 7465 7374 5f72  ndex(self.test_r
-00007b90: 6563 292c 2022 6661 696c 6564 2027 696e  ec), "failed 'in
-00007ba0: 6465 783b 2074 6573 7420 2865 7869 7374  dex; test (exist
-00007bb0: 7329 2229 0a20 2020 2020 2020 2069 6620  s)").        if 
-00007bc0: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
-00007bd0: 7465 7374 5f72 6563 2c20 5369 6d70 6c65  test_rec, Simple
-00007be0: 4e61 6d65 7370 6163 6529 3a0a 2020 2020  Namespace):.    
-00007bf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00007c00: 6572 7445 7175 616c 2831 332c 2073 656c  ertEqual(13, sel
-00007c10: 662e 7431 2e69 6e64 6578 2876 6172 7328  f.t1.index(vars(
-00007c20: 7365 6c66 2e74 6573 745f 7265 6329 292c  self.test_rec)),
-00007c30: 2022 6661 696c 6564 2027 696e 6465 783b   "failed 'index;
-00007c40: 2074 6573 7420 2865 7869 7374 7329 2229   test (exists)")
-00007c50: 0a0a 2020 2020 2020 2020 6e6f 5f73 7563  ..        no_suc
-00007c60: 685f 7265 6320 3d20 7365 6c66 2e6d 616b  h_rec = self.mak
-00007c70: 655f 6461 7461 5f6f 626a 6563 7428 7365  e_data_object(se
-00007c80: 6c66 2e74 6573 745f 7369 7a65 2b31 2c20  lf.test_size+1, 
-00007c90: 7365 6c66 2e74 6573 745f 7369 7a65 2b31  self.test_size+1
-00007ca0: 2c20 7365 6c66 2e74 6573 745f 7369 7a65  , self.test_size
-00007cb0: 2b31 290a 2020 2020 2020 2020 7769 7468  +1).        with
-00007cc0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00007cd0: 6573 2856 616c 7565 4572 726f 722c 206d  es(ValueError, m
-00007ce0: 7367 3d22 6661 696c 6564 2027 696e 6465  sg="failed 'inde
-00007cf0: 7827 2074 6573 7420 286e 6f74 2065 7869  x' test (not exi
-00007d00: 7374 7329 2229 3a0a 2020 2020 2020 2020  sts)"):.        
-00007d10: 2020 2020 7365 6c66 2e74 312e 696e 6465      self.t1.inde
-00007d20: 7828 6e6f 5f73 7563 685f 7265 6329 0a0a  x(no_such_rec)..
-00007d30: 2020 2020 6465 6620 7465 7374 5f72 656d      def test_rem
-00007d40: 6f76 6528 7365 6c66 293a 0a20 2020 2020  ove(self):.     
-00007d50: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-00007d60: 6974 2829 0a20 2020 2020 2020 2072 6563  it().        rec
-00007d70: 203d 2073 656c 662e 6d61 6b65 5f64 6174   = self.make_dat
-00007d80: 615f 6f62 6a65 6374 2831 2c20 312c 2031  a_object(1, 1, 1
-00007d90: 290a 2020 2020 2020 2020 7072 6576 5f6c  ).        prev_l
-00007da0: 656e 203d 206c 656e 2873 656c 662e 7431  en = len(self.t1
-00007db0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00007dc0: 312e 7265 6d6f 7665 2872 6563 290a 2020  1.remove(rec).  
-00007dd0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00007de0: 7446 616c 7365 2872 6563 2069 6e20 7365  tFalse(rec in se
-00007df0: 6c66 2e74 312c 2022 6661 696c 6564 2074  lf.t1, "failed t
-00007e00: 6f20 7265 6d6f 7665 2072 6563 6f72 6420  o remove record 
-00007e10: 6672 6f6d 2074 6162 6c65 2028 636f 6e74  from table (cont
-00007e20: 6169 6e73 2922 290a 2020 2020 2020 2020  ains)").        
-00007e30: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00007e40: 2870 7265 765f 6c65 6e2d 312c 206c 656e  (prev_len-1, len
-00007e50: 2873 656c 662e 7431 292c 2022 6661 696c  (self.t1), "fail
-00007e60: 6564 2074 6f20 7265 6d6f 7665 2072 6563  ed to remove rec
-00007e70: 6f72 6420 6672 6f6d 2074 6162 6c65 2028  ord from table (
-00007e80: 6c65 6e29 2229 0a0a 2020 2020 2020 2020  len)")..        
-00007e90: 6e6f 5f73 7563 685f 7265 6320 3d20 7365  no_such_rec = se
-00007ea0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00007eb0: 6563 7428 7365 6c66 2e74 6573 745f 7369  ect(self.test_si
-00007ec0: 7a65 2b31 2c20 7365 6c66 2e74 6573 745f  ze+1, self.test_
-00007ed0: 7369 7a65 2b31 2c20 7365 6c66 2e74 6573  size+1, self.tes
-00007ee0: 745f 7369 7a65 2b31 290a 2020 2020 2020  t_size+1).      
-00007ef0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-00007f00: 7365 286e 6f5f 7375 6368 5f72 6563 2069  se(no_such_rec i
-00007f10: 6e20 7365 6c66 2e74 312c 2022 6661 696c  n self.t1, "fail
-00007f20: 6564 2074 6f20 6372 6561 7465 206e 6f6e  ed to create non
-00007f30: 2d65 7869 7374 656e 7420 7265 636f 7264  -existent record
-00007f40: 2066 726f 6d20 7461 626c 6522 290a 2020   from table").  
-00007f50: 2020 2020 2020 7365 6c66 2e74 312e 7265        self.t1.re
-00007f60: 6d6f 7665 286e 6f5f 7375 6368 5f72 6563  move(no_such_rec
-00007f70: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00007f80: 7373 6572 7445 7175 616c 2870 7265 765f  ssertEqual(prev_
-00007f90: 6c65 6e2d 312c 206c 656e 2873 656c 662e  len-1, len(self.
-00007fa0: 7431 292c 2022 6661 696c 6564 2072 656d  t1), "failed rem
-00007fb0: 6f76 696e 6720 6e6f 6e2d 6578 6973 7465  oving non-existe
-00007fc0: 6e74 2072 6563 6f72 6420 6672 6f6d 2074  nt record from t
-00007fd0: 6162 6c65 2028 6c65 6e29 2229 0a0a 2020  able (len)")..  
-00007fe0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00007ff0: 6e63 6528 7365 6c66 2e74 6573 745f 7265  nce(self.test_re
-00008000: 632c 2053 696d 706c 654e 616d 6573 7061  c, SimpleNamespa
-00008010: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
-00008020: 2073 656c 662e 7431 2e72 656d 6f76 6528   self.t1.remove(
-00008030: 7661 7273 2873 656c 662e 7465 7374 5f72  vars(self.test_r
-00008040: 6563 2929 0a20 2020 2020 2020 2020 2020  ec)).           
-00008050: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00008060: 6c28 7072 6576 5f6c 656e 2d31 2c20 6c65  l(prev_len-1, le
-00008070: 6e28 7365 6c66 2e74 3129 2c20 2266 6169  n(self.t1), "fai
-00008080: 6c65 6420 746f 2072 656d 6f76 6520 7265  led to remove re
-00008090: 636f 7264 2061 7320 6469 6374 2066 726f  cord as dict fro
-000080a0: 6d20 7461 626c 6520 286c 656e 2922 290a  m table (len)").
-000080b0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
-000080c0: 6465 785f 6163 6365 7373 2873 656c 6629  dex_access(self)
-000080d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000080e0: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
-000080f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00008100: 7175 616c 2873 656c 662e 7465 7374 5f72  qual(self.test_r
-00008110: 6563 2c20 7365 6c66 2e74 315b 3133 5d2c  ec, self.t1[13],
-00008120: 2022 6661 696c 6564 2069 6e64 6578 2061   "failed index a
-00008130: 6363 6573 7320 7465 7374 2229 0a0a 2020  ccess test")..  
-00008140: 2020 6465 6620 7465 7374 5f63 6f75 6e74    def test_count
-00008150: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008160: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
-00008170: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00008180: 7373 6572 7454 7275 6528 7365 6c66 2e74  ssertTrue(self.t
-00008190: 312e 636f 756e 7428 7365 6c66 2e74 6573  1.count(self.tes
-000081a0: 745f 7265 6329 203d 3d20 312c 2022 6661  t_rec) == 1, "fa
-000081b0: 696c 6564 2063 6f75 6e74 2074 6573 7422  iled count test"
-000081c0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
-000081d0: 6e73 7461 6e63 6528 7365 6c66 2e74 6573  nstance(self.tes
-000081e0: 745f 7265 632c 2053 696d 706c 654e 616d  t_rec, SimpleNam
-000081f0: 6573 7061 6365 293a 0a20 2020 2020 2020  espace):.       
-00008200: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00008210: 5472 7565 2873 656c 662e 7431 2e63 6f75  True(self.t1.cou
-00008220: 6e74 2876 6172 7328 7365 6c66 2e74 6573  nt(vars(self.tes
-00008230: 745f 7265 6329 2920 3d3d 2031 2c20 2266  t_rec)) == 1, "f
-00008240: 6169 6c65 6420 636f 756e 7420 7465 7374  ailed count test
-00008250: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-00008260: 5f64 656c 2873 656c 6629 3a0a 2020 2020  _del(self):.    
-00008270: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
-00008280: 6e69 7428 290a 2020 2020 2020 2020 6265  nit().        be
-00008290: 666f 7265 5f64 656c 5f6c 656e 203d 206c  fore_del_len = l
-000082a0: 656e 2873 656c 662e 7431 290a 2020 2020  en(self.t1).    
-000082b0: 2020 2020 6465 6c20 7365 6c66 2e74 315b      del self.t1[
-000082c0: 3133 5d0a 2020 2020 2020 2020 7365 6c66  13].        self
-000082d0: 2e61 7373 6572 7446 616c 7365 2873 656c  .assertFalse(sel
-000082e0: 662e 7465 7374 5f72 6563 2069 6e20 7365  f.test_rec in se
-000082f0: 6c66 2e74 312c 2022 6661 696c 6564 2064  lf.t1, "failed d
-00008300: 656c 2074 6573 7422 290a 2020 2020 2020  el test").      
-00008310: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00008320: 616c 2862 6566 6f72 655f 6465 6c5f 6c65  al(before_del_le
-00008330: 6e20 2d20 312c 206c 656e 2873 656c 662e  n - 1, len(self.
-00008340: 7431 2929 0a0a 2020 2020 6465 6620 7465  t1))..    def te
-00008350: 7374 5f70 6f70 2873 656c 6629 3a0a 2020  st_pop(self):.  
-00008360: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
-00008370: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
-00008380: 6265 666f 7265 5f70 6f70 5f6c 656e 203d  before_pop_len =
-00008390: 206c 656e 2873 656c 662e 7431 290a 2020   len(self.t1).  
-000083a0: 2020 2020 2020 6f62 6a20 3d20 7365 6c66        obj = self
-000083b0: 2e74 312e 706f 7028 3133 290a 2020 2020  .t1.pop(13).    
-000083c0: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-000083d0: 616c 7365 286f 626a 2069 6e20 7365 6c66  alse(obj in self
-000083e0: 2e74 3129 0a20 2020 2020 2020 2073 656c  .t1).        sel
-000083f0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
-00008400: 6c66 2e74 6573 745f 7265 632c 206f 626a  lf.test_rec, obj
-00008410: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00008420: 7373 6572 7445 7175 616c 2862 6566 6f72  ssertEqual(befor
-00008430: 655f 706f 705f 6c65 6e20 2d20 312c 206c  e_pop_len - 1, l
-00008440: 656e 2873 656c 662e 7431 2929 0a0a 2020  en(self.t1))..  
-00008450: 2020 6465 6620 7465 7374 5f70 6f70 5f6c    def test_pop_l
-00008460: 6173 7428 7365 6c66 293a 0a20 2020 2020  ast(self):.     
-00008470: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-00008480: 6974 2829 0a20 2020 2020 2020 2062 6566  it().        bef
-00008490: 6f72 655f 706f 705f 6c65 6e20 3d20 6c65  ore_pop_len = le
-000084a0: 6e28 7365 6c66 2e74 3129 0a20 2020 2020  n(self.t1).     
-000084b0: 2020 2065 7870 6563 7465 645f 706f 7020     expected_pop 
-000084c0: 3d20 636f 7079 2e63 6f70 7928 7365 6c66  = copy.copy(self
-000084d0: 2e74 315b 2d31 5d29 0a20 2020 2020 2020  .t1[-1]).       
-000084e0: 206f 626a 203d 2073 656c 662e 7431 2e70   obj = self.t1.p
-000084f0: 6f70 2829 0a20 2020 2020 2020 2073 656c  op().        sel
-00008500: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-00008510: 7065 6374 6564 5f70 6f70 2c20 6f62 6a29  pected_pop, obj)
-00008520: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00008530: 7365 7274 4571 7561 6c28 6265 666f 7265  sertEqual(before
-00008540: 5f70 6f70 5f6c 656e 202d 2031 2c20 6c65  _pop_len - 1, le
-00008550: 6e28 7365 6c66 2e74 3129 290a 0a20 2020  n(self.t1))..   
-00008560: 2064 6566 2074 6573 745f 7265 7665 7273   def test_revers
-00008570: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-00008580: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
-00008590: 7428 290a 2020 2020 2020 2020 6c61 7374  t().        last
-000085a0: 5f72 6563 203d 206e 6578 7428 7265 7665  _rec = next(reve
-000085b0: 7273 6564 2873 656c 662e 7431 2929 0a20  rsed(self.t1)). 
-000085c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000085d0: 7274 4571 7561 6c28 7365 6c66 2e6d 616b  rtEqual(self.mak
-000085e0: 655f 6461 7461 5f6f 626a 6563 7428 322c  e_data_object(2,
-000085f0: 2032 2c20 3229 2c20 6c61 7374 5f72 6563   2, 2), last_rec
-00008600: 2c20 2266 6169 6c65 6420 7265 7665 7273  , "failed revers
-00008610: 6564 2074 6573 7422 290a 0a20 2020 2064  ed test")..    d
-00008620: 6566 2074 6573 745f 6974 6572 2873 656c  ef test_iter(sel
-00008630: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00008640: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-00008650: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00008660: 7454 7275 6528 7365 6c66 2e74 6573 745f  tTrue(self.test_
-00008670: 7265 6320 696e 2073 656c 662e 7431 2c20  rec in self.t1, 
-00008680: 2266 6169 6c65 6420 2769 6e27 2028 636f  "failed 'in' (co
-00008690: 6e74 6169 6e73 2920 7465 7374 2229 0a0a  ntains) test")..
-000086a0: 2020 2020 6465 6620 7465 7374 5f68 6561      def test_hea
-000086b0: 645f 616e 645f 7461 696c 2873 656c 6629  d_and_tail(self)
-000086c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000086d0: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
-000086e0: 2020 2020 7365 6c66 2e74 312e 6372 6561      self.t1.crea
-000086f0: 7465 5f69 6e64 6578 2822 6122 290a 2020  te_index("a").  
-00008700: 2020 2020 2020 7365 6c66 2e74 312e 6372        self.t1.cr
-00008710: 6561 7465 5f69 6e64 6578 2822 6322 290a  eate_index("c").
-00008720: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008730: 6572 7445 7175 616c 287b 2261 222c 2022  ertEqual({"a", "
-00008740: 6322 7d2c 2073 6574 2873 656c 662e 7431  c"}, set(self.t1
-00008750: 2e5f 696e 6465 7865 732e 6b65 7973 2829  ._indexes.keys()
-00008760: 292c 2022 6661 696c 6564 2074 6f20 6372  ), "failed to cr
-00008770: 6561 7465 2069 6e64 6578 6573 2229 0a0a  eate indexes")..
-00008780: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008790: 6572 7445 7175 616c 2873 6574 2873 656c  ertEqual(set(sel
-000087a0: 662e 7431 2e5f 696e 6465 7865 732e 6b65  f.t1._indexes.ke
-000087b0: 7973 2829 292c 0a20 2020 2020 2020 2020  ys()),.         
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 7365 7428 7365 6c66 2e74 312e 6865 6164  set(self.t1.head
-000087e0: 2829 2e5f 696e 6465 7865 732e 6b65 7973  ()._indexes.keys
-000087f0: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
-00008800: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00008810: 6169 6c65 6420 746f 2063 6f70 7920 696e  ailed to copy in
-00008820: 6465 7865 7320 746f 2068 6561 6428 2922  dexes to head()"
-00008830: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00008840: 7373 6572 7445 7175 616c 2873 6574 2873  ssertEqual(set(s
-00008850: 656c 662e 7431 2e5f 696e 6465 7865 732e  elf.t1._indexes.
-00008860: 6b65 7973 2829 292c 0a20 2020 2020 2020  keys()),.       
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 7365 7428 7365 6c66 2e74 312e 7461    set(self.t1.ta
-00008890: 696c 2829 2e5f 696e 6465 7865 732e 6b65  il()._indexes.ke
-000088a0: 7973 2829 292c 0a20 2020 2020 2020 2020  ys()),.         
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2266 6169 6c65 6420 746f 2063 6f70 7920  "failed to copy 
-000088d0: 696e 6465 7865 7320 746f 2074 6169 6c28  indexes to tail(
-000088e0: 2922 290a 0a20 2020 2064 6566 2074 6573  )")..    def tes
-000088f0: 745f 756e 6971 7565 2873 656c 6629 3a0a  t_unique(self):.
-00008900: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-00008910: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
-00008920: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00008930: 616c 285b 302c 2031 2c20 325d 2c20 736f  al([0, 1, 2], so
-00008940: 7274 6564 285b 726f 772e 6120 666f 7220  rted([row.a for 
-00008950: 726f 7720 696e 2073 656c 662e 7431 2e75  row in self.t1.u
-00008960: 6e69 7175 6528 2761 2729 5d29 2c20 2266  nique('a')]), "f
-00008970: 6169 6c65 6420 6361 6c6c 2074 6f20 756e  ailed call to un
-00008980: 6971 7565 2229 0a0a 2020 2020 6465 6620  ique")..    def 
-00008990: 7465 7374 5f61 6c6c 5f61 6363 6573 736f  test_all_accesso
-000089a0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-000089b0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
-000089c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000089d0: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
-000089e0: 285b 695d 2a73 656c 662e 7465 7374 5f73  ([i]*self.test_s
-000089f0: 697a 652a 2a32 2066 6f72 2069 2069 6e20  ize**2 for i in 
-00008a00: 7261 6e67 6528 7365 6c66 2e74 6573 745f  range(self.test_
-00008a10: 7369 7a65 2929 2c20 5b5d 292c 0a20 2020  size)), []),.   
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 2020 6c69 7374 2873 656c 662e        list(self.
-00008a40: 7431 2e61 6c6c 2e61 292c 0a20 2020 2020  t1.all.a),.     
-00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a60: 2020 2020 2266 6169 6c65 6420 746f 2073      "failed to s
-00008a70: 7563 6365 7373 6675 6c6c 7920 6765 7420  uccessfully get 
-00008a80: 616c 6c20 7661 6c75 6573 2069 6e20 2761  all values in 'a
-00008a90: 2722 290a 0a20 2020 2020 2020 2061 6c6c  '")..        all
-00008aa0: 5f61 7320 3d20 7365 6c66 2e74 312e 616c  _as = self.t1.al
-00008ab0: 6c2e 610a 2020 2020 2020 2020 7365 6c66  l.a.        self
-00008ac0: 2e61 7373 6572 7454 7275 6528 616c 6c5f  .assertTrue(all_
-00008ad0: 6173 2069 7320 6974 6572 2861 6c6c 5f61  as is iter(all_a
-00008ae0: 7329 2c20 2261 6c6c 2069 7465 7261 746f  s), "all iterato
-00008af0: 7220 6661 696c 7320 746f 2069 6465 6e74  r fails to ident
-00008b00: 6966 7920 6173 2069 7465 7228 7365 6c66  ify as iter(self
-00008b10: 2922 290a 0a20 2020 2064 6566 2074 6573  )")..    def tes
-00008b20: 745f 666f 726d 6174 2873 656c 6629 3a0a  t_format(self):.
-00008b30: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-00008b40: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
-00008b50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00008b60: 616c 285b 2730 3020 3020 3027 2c20 2730  al(['00 0 0', '0
-00008b70: 3020 3020 3127 2c20 2730 3020 3020 3227  0 0 1', '00 0 2'
-00008b80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00008b90: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00008ba0: 2873 656c 662e 7431 2e66 6f72 6d61 7428  (self.t1.format(
-00008bb0: 227b 613a 3032 647d 207b 627d 207b 637d  "{a:02d} {b} {c}
-00008bc0: 2229 295b 3a33 5d2c 0a20 2020 2020 2020  "))[:3],.       
-00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008be0: 2020 2266 6169 6c65 6420 746f 2063 7265    "failed to cre
-00008bf0: 6174 6520 666f 726d 6174 7465 6420 726f  ate formatted ro
-00008c00: 7773 2229 0a0a 2020 2020 6465 6620 7465  ws")..    def te
-00008c10: 7374 5f61 735f 6874 6d6c 2873 656c 6629  st_as_html(self)
-00008c20: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00008c30: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
-00008c40: 2020 2020 6874 6d6c 5f6f 7574 7075 7420      html_output 
-00008c50: 3d20 7365 6c66 2e74 315b 3a31 305d 2e61  = self.t1[:10].a
-00008c60: 735f 6874 6d6c 2866 6965 6c64 733d 2261  s_html(fields="a
-00008c70: 2062 2063 2229 0a20 2020 2020 2020 2070   b c").        p
-00008c80: 7269 6e74 2868 746d 6c5f 6f75 7470 7574  rint(html_output
-00008c90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00008ca0: 7373 6572 7454 7275 6528 223c 7468 6561  ssertTrue("<thea
-00008cb0: 643e 2220 696e 2068 746d 6c5f 6f75 7470  d>" in html_outp
-00008cc0: 7574 2061 6e64 2022 3c74 626f 6479 3e22  ut and "<tbody>"
-00008cd0: 2069 6e20 6874 6d6c 5f6f 7574 7075 742c   in html_output,
-00008ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008cf0: 2020 2020 2020 2020 2022 6173 5f68 746d           "as_htm
-00008d00: 6c20 646f 6573 206e 6f74 2069 6e63 6c75  l does not inclu
-00008d10: 6465 2074 6865 6164 2061 6e64 2074 626f  de thead and tbo
-00008d20: 6479 2074 6167 7322 290a 0a20 2020 2020  dy tags")..     
-00008d30: 2020 2068 746d 6c5f 6c69 6e65 7320 3d20     html_lines = 
-00008d40: 6874 6d6c 5f6f 7574 7075 742e 7370 6c69  html_output.spli
-00008d50: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
-00008d60: 2068 6472 5f6c 696e 6520 3d20 6e65 7874   hdr_line = next
-00008d70: 2868 2066 6f72 2068 2069 6e20 6874 6d6c  (h for h in html
-00008d80: 5f6c 696e 6573 2069 6620 2263 656e 7465  _lines if "cente
-00008d90: 7222 2069 6e20 6829 0a20 2020 2020 2020  r" in h).       
-00008da0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00008db0: 6c28 273c 7472 3e3c 7468 3e3c 6469 7620  l('<tr><th><div 
-00008dc0: 616c 6967 6e3d 2263 656e 7465 7222 3e61  align="center">a
-00008dd0: 3c2f 6469 763e 3c2f 7468 3e27 0a20 2020  </div></th>'.   
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 2020 2020 2020 273c 7468 3e3c 6469 7620        '<th><div 
-00008e00: 616c 6967 6e3d 2263 656e 7465 7222 3e62  align="center">b
-00008e10: 3c2f 6469 763e 3c2f 7468 3e27 0a20 2020  </div></th>'.   
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2020 273c 7468 3e3c 6469 7620        '<th><div 
-00008e40: 616c 6967 6e3d 2263 656e 7465 7222 3e63  align="center">c
-00008e50: 3c2f 6469 763e 3c2f 7468 3e3c 2f74 723e  </div></th></tr>
-00008e60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00008e70: 2020 2020 2020 2020 2020 2020 6864 725f              hdr_
-00008e80: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008ea0: 6661 696c 6564 2061 735f 6874 6d6c 2077  failed as_html w
-00008eb0: 6974 6820 616c 6c20 6669 656c 6473 2229  ith all fields")
-00008ec0: 0a0a 2020 2020 2020 2020 6874 6d6c 5f6f  ..        html_o
-00008ed0: 7574 7075 7420 3d20 7365 6c66 2e74 315b  utput = self.t1[
-00008ee0: 3a31 305d 2e61 735f 6874 6d6c 2866 6965  :10].as_html(fie
-00008ef0: 6c64 733d 2261 202d 6220 6322 290a 2020  lds="a -b c").  
-00008f00: 2020 2020 2020 7072 696e 7428 6874 6d6c        print(html
-00008f10: 5f6f 7574 7075 7429 0a20 2020 2020 2020  _output).       
-00008f20: 2068 746d 6c5f 6c69 6e65 7320 3d20 6874   html_lines = ht
-00008f30: 6d6c 5f6f 7574 7075 742e 7370 6c69 746c  ml_output.splitl
-00008f40: 696e 6573 2829 0a20 2020 2020 2020 2068  ines().        h
-00008f50: 6472 5f6c 696e 6520 3d20 6e65 7874 2868  dr_line = next(h
-00008f60: 2066 6f72 2068 2069 6e20 6874 6d6c 5f6c   for h in html_l
-00008f70: 696e 6573 2069 6620 2263 656e 7465 7222  ines if "center"
-00008f80: 2069 6e20 6829 0a20 2020 2020 2020 2073   in h).        s
-00008f90: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00008fa0: 273c 7472 3e3c 7468 3e3c 6469 7620 616c  '<tr><th><div al
-00008fb0: 6967 6e3d 2263 656e 7465 7222 3e61 3c2f  ign="center">a</
-00008fc0: 6469 763e 3c2f 7468 3e27 0a20 2020 2020  div></th>'.     
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 2020 2020 273c 7468 3e3c 6469 7620 616c      '<th><div al
-00008ff0: 6967 6e3d 2263 656e 7465 7222 3e63 3c2f  ign="center">c</
-00009000: 6469 763e 3c2f 7468 3e3c 2f74 723e 272c  div></th></tr>',
-00009010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009020: 2020 2020 2020 2020 2020 6864 725f 6c69            hdr_li
-00009030: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00009040: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00009050: 696c 6564 2061 735f 6874 6d6c 2077 6974  iled as_html wit
-00009060: 6820 6e65 6761 7465 6420 6669 656c 6422  h negated field"
-00009070: 290a 0a20 2020 2020 2020 2068 746d 6c5f  )..        html_
-00009080: 6f75 7470 7574 203d 2073 656c 662e 7431  output = self.t1
-00009090: 5b3a 3130 5d2e 6173 5f68 746d 6c28 6669  [:10].as_html(fi
-000090a0: 656c 6473 3d22 6120 6220 6322 2c20 666f  elds="a b c", fo
-000090b0: 726d 6174 733d 7b22 6222 3a20 227b 3a30  rmats={"b": "{:0
-000090c0: 3364 7d22 7d29 0a20 2020 2020 2020 2070  3d}"}).        p
-000090d0: 7269 6e74 2868 746d 6c5f 6f75 7470 7574  rint(html_output
-000090e0: 290a 2020 2020 2020 2020 6874 6d6c 5f6c  ).        html_l
-000090f0: 696e 6573 203d 2068 746d 6c5f 6f75 7470  ines = html_outp
-00009100: 7574 2e73 706c 6974 6c69 6e65 7328 290a  ut.splitlines().
-00009110: 2020 2020 2020 2020 6461 7461 5f6c 696e          data_lin
-00009120: 6520 3d20 6e65 7874 2868 2066 6f72 2068  e = next(h for h
-00009130: 2069 6e20 6874 6d6c 5f6c 696e 6573 2069   in html_lines i
-00009140: 6620 223c 7464 3e22 2069 6e20 6829 0a20  f "<td>" in h). 
-00009150: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00009160: 7274 4571 7561 6c28 273c 7462 6f64 793e  rtEqual('<tbody>
-00009170: 3c74 723e 3c74 643e 3c64 6976 2061 6c69  <tr><td><div ali
-00009180: 676e 3d22 7269 6768 7422 3e30 3c2f 6469  gn="right">0</di
-00009190: 763e 3c2f 7464 3e27 0a20 2020 2020 2020  v></td>'.       
-000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091b0: 2020 273c 7464 3e3c 6469 7620 616c 6967    '<td><div alig
-000091c0: 6e3d 2272 6967 6874 223e 3030 303c 2f64  n="right">000</d
-000091d0: 6976 3e3c 2f74 643e 270a 2020 2020 2020  iv></td>'.      
-000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091f0: 2020 2027 3c74 643e 3c64 6976 2061 6c69     '<td><div ali
-00009200: 676e 3d22 7269 6768 7422 3e30 3c2f 6469  gn="right">0</di
-00009210: 763e 3c2f 7464 3e3c 2f74 723e 272c 0a20  v></td></tr>',. 
-00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009230: 2020 2020 2020 2020 6461 7461 5f6c 696e          data_lin
-00009240: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00009250: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
-00009260: 6c65 6420 6173 5f68 746d 6c20 7769 7468  led as_html with
-00009270: 206e 616d 6564 2066 6965 6c64 2066 6f72   named field for
-00009280: 6d61 7420 666f 7220 7370 6563 6966 6963  mat for specific
-00009290: 2066 6965 6c64 2229 0a0a 2020 2020 2020   field")..      
-000092a0: 2020 6874 6d6c 5f6f 7574 7075 7420 3d20    html_output = 
-000092b0: 7365 6c66 2e74 315b 3a31 305d 2e61 735f  self.t1[:10].as_
-000092c0: 6874 6d6c 2866 6965 6c64 733d 2261 2062  html(fields="a b
-000092d0: 2063 222c 2066 6f72 6d61 7473 3d7b 696e   c", formats={in
-000092e0: 743a 2022 7b3a 3033 647d 227d 290a 2020  t: "{:03d}"}).  
-000092f0: 2020 2020 2020 7072 696e 7428 6874 6d6c        print(html
-00009300: 5f6f 7574 7075 7429 0a20 2020 2020 2020  _output).       
-00009310: 2068 746d 6c5f 6c69 6e65 7320 3d20 6874   html_lines = ht
-00009320: 6d6c 5f6f 7574 7075 742e 7370 6c69 746c  ml_output.splitl
-00009330: 696e 6573 2829 0a20 2020 2020 2020 2064  ines().        d
-00009340: 6174 615f 6c69 6e65 203d 206e 6578 7428  ata_line = next(
-00009350: 6820 666f 7220 6820 696e 2068 746d 6c5f  h for h in html_
-00009360: 6c69 6e65 7320 6966 2022 3c74 643e 2220  lines if "<td>" 
-00009370: 696e 2068 290a 2020 2020 2020 2020 7365  in h).        se
-00009380: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
-00009390: 3c74 626f 6479 3e3c 7472 3e3c 7464 3e3c  <tbody><tr><td><
-000093a0: 6469 7620 616c 6967 6e3d 2272 6967 6874  div align="right
-000093b0: 223e 3030 303c 2f64 6976 3e3c 2f74 643e  ">000</div></td>
-000093c0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000093d0: 2020 2020 2020 2020 2020 2027 3c74 643e             '<td>
-000093e0: 3c64 6976 2061 6c69 676e 3d22 7269 6768  <div align="righ
-000093f0: 7422 3e30 3030 3c2f 6469 763e 3c2f 7464  t">000</div></td
-00009400: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
-00009410: 2020 2020 2020 2020 2020 2020 273c 7464              '<td
-00009420: 3e3c 6469 7620 616c 6967 6e3d 2272 6967  ><div align="rig
-00009430: 6874 223e 3030 303c 2f64 6976 3e3c 2f74  ht">000</div></t
-00009440: 643e 3c2f 7472 3e27 2c0a 2020 2020 2020  d></tr>',.      
-00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009460: 2020 2064 6174 615f 6c69 6e65 2c0a 2020     data_line,.  
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 2020 2020 2020 2022 6661 696c 6564 2061         "failed a
-00009490: 735f 6874 6d6c 2077 6974 6820 6461 7461  s_html with data
-000094a0: 2074 7970 6520 666f 726d 6174 2066 6f72   type format for
-000094b0: 2061 6c6c 2066 6965 6c64 7322 290a 0a20   all fields").. 
-000094c0: 2020 2020 2020 2068 746d 6c5f 6f75 7470         html_outp
-000094d0: 7574 203d 2073 656c 662e 7431 5b3a 3130  ut = self.t1[:10
-000094e0: 5d2e 6173 5f68 746d 6c28 6669 656c 6473  ].as_html(fields
-000094f0: 3d22 6120 6220 6322 2c20 666f 726d 6174  ="a b c", format
-00009500: 733d 7b69 6e74 3a20 227b 3a30 3364 7d22  s={int: "{:03d}"
-00009510: 7d2c 2067 726f 7570 6279 3d22 6122 290a  }, groupby="a").
-00009520: 2020 2020 2020 2020 7072 696e 7428 6874          print(ht
-00009530: 6d6c 5f6f 7574 7075 7429 0a20 2020 2020  ml_output).     
-00009540: 2020 2068 746d 6c5f 6c69 6e65 7320 3d20     html_lines = 
-00009550: 6874 6d6c 5f6f 7574 7075 742e 7370 6c69  html_output.spli
-00009560: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
-00009570: 2064 6174 615f 6c69 6e65 203d 206e 6578   data_line = nex
-00009580: 7428 6820 666f 7220 6820 696e 2068 746d  t(h for h in htm
-00009590: 6c5f 6c69 6e65 7320 6966 2022 3c74 643e  l_lines if "<td>
-000095a0: 2220 696e 2068 290a 2020 2020 2020 2020  " in h).        
-000095b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000095c0: 2827 3c74 626f 6479 3e3c 7472 3e3c 7464  ('<tbody><tr><td
-000095d0: 3e3c 6469 7620 616c 6967 6e3d 2272 6967  ><div align="rig
-000095e0: 6874 223e 3030 303c 2f64 6976 3e3c 2f74  ht">000</div></t
-000095f0: 643e 270a 2020 2020 2020 2020 2020 2020  d>'.            
-00009600: 2020 2020 2020 2020 2020 2020 2027 3c74               '<t
-00009610: 643e 3c64 6976 2061 6c69 676e 3d22 7269  d><div align="ri
-00009620: 6768 7422 3e30 3030 3c2f 6469 763e 3c2f  ght">000</div></
-00009630: 7464 3e27 0a20 2020 2020 2020 2020 2020  td>'.           
-00009640: 2020 2020 2020 2020 2020 2020 2020 273c                '<
-00009650: 7464 3e3c 6469 7620 616c 6967 6e3d 2272  td><div align="r
-00009660: 6967 6874 223e 3030 303c 2f64 6976 3e3c  ight">000</div><
-00009670: 2f74 643e 3c2f 7472 3e27 2c0a 2020 2020  /td></tr>',.    
-00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009690: 2020 2020 2064 6174 615f 6c69 6e65 2c0a       data_line,.
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 2020 2020 2020 2022 6661 696c 6564           "failed
-000096c0: 2061 735f 6874 6d6c 2077 6974 6820 6772   as_html with gr
-000096d0: 6f75 7062 7922 290a 0a20 2020 2020 2020  oupby")..       
-000096e0: 2068 746d 6c5f 6f75 7470 7574 203d 2073   html_output = s
-000096f0: 656c 662e 7431 5b3a 3130 5d2e 6173 5f68  elf.t1[:10].as_h
-00009700: 746d 6c28 6669 656c 6473 3d22 6120 6220  tml(fields="a b 
-00009710: 6322 2c20 7461 626c 655f 7072 6f70 6572  c", table_proper
-00009720: 7469 6573 3d7b 2262 6f72 6465 7222 3a20  ties={"border": 
-00009730: 2232 227d 290a 2020 2020 2020 2020 7072  "2"}).        pr
-00009740: 696e 7428 6874 6d6c 5f6f 7574 7075 7429  int(html_output)
-00009750: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00009760: 7365 7274 5472 7565 2822 3c74 6865 6164  sertTrue("<thead
-00009770: 3e22 2069 6e20 6874 6d6c 5f6f 7574 7075  >" in html_outpu
-00009780: 7420 616e 6420 223c 7462 6f64 793e 2220  t and "<tbody>" 
-00009790: 696e 2068 746d 6c5f 6f75 7470 7574 2c0a  in html_output,.
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 2020 2020 2020 2261 735f 6874 6d6c          "as_html
-000097c0: 2064 6f65 7320 6e6f 7420 696e 636c 7564   does not includ
-000097d0: 6520 7468 6561 6420 616e 6420 7462 6f64  e thead and tbod
-000097e0: 7920 7461 6773 2229 0a0a 0a20 2020 2064  y tags")...    d
-000097f0: 6566 2074 6573 745f 6465 6c65 7465 5f73  ef test_delete_s
-00009800: 6c69 6365 7328 7365 6c66 293a 0a20 2020  lices(self):.   
-00009810: 2020 2020 2063 6f6d 7061 7265 5f6c 6973       compare_lis
-00009820: 7420 3d20 6c69 7374 2822 4142 4344 4546  t = list("ABCDEF
-00009830: 4748 494a 4b4c 4d4e 4f50 5152 5354 5556  GHIJKLMNOPQRSTUV
-00009840: 5758 595a 3031 3233 3435 3637 3839 6162  WXYZ0123456789ab
-00009850: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
-00009860: 7374 7576 7778 797a 2229 0a20 2020 2020  stuvwxyz").     
-00009870: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
-00009880: 2829 2e69 6e73 6572 745f 6d61 6e79 286c  ().insert_many(l
-00009890: 742e 4461 7461 4f62 6a65 6374 2841 3d63  t.DataObject(A=c
-000098a0: 2920 666f 7220 6320 696e 2063 6f6d 7061  ) for c in compa
-000098b0: 7265 5f6c 6973 7429 0a0a 2020 2020 2020  re_list)..      
-000098c0: 2020 6465 6620 6d69 6e69 5f74 6573 7428    def mini_test(
-000098d0: 736c 635f 7475 706c 6529 3a0a 2020 2020  slc_tuple):.    
-000098e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000098f0: 7461 6e63 6528 736c 635f 7475 706c 652c  tance(slc_tuple,
-00009900: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
-00009910: 2020 2020 2020 2020 206c 6162 656c 203d           label =
-00009920: 2022 5b7b 7d3a 7b7d 3a7b 7d5d 222e 666f   "[{}:{}:{}]".fo
-00009930: 726d 6174 282a 2869 2069 6620 6920 6973  rmat(*(i if i is
-00009940: 206e 6f74 204e 6f6e 6520 656c 7365 2027   not None else '
-00009950: 2720 666f 7220 6920 696e 2073 6c63 5f74  ' for i in slc_t
-00009960: 7570 6c65 2929 0a20 2020 2020 2020 2020  uple)).         
-00009970: 2020 2020 2020 2073 6c63 203d 2073 6c69         slc = sli
-00009980: 6365 282a 736c 635f 7475 706c 6529 0a20  ce(*slc_tuple). 
-00009990: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000099a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000099b0: 206c 6162 656c 203d 2073 7472 2873 6c63   label = str(slc
-000099c0: 5f74 7570 6c65 290a 2020 2020 2020 2020  _tuple).        
-000099d0: 2020 2020 2020 2020 736c 6320 3d20 736c          slc = sl
-000099e0: 635f 7475 706c 650a 0a20 2020 2020 2020  c_tuple..       
-000099f0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00009a00: 7562 5465 7374 286c 6162 656c 2c20 736c  ubTest(label, sl
-00009a10: 635f 7475 706c 653d 736c 635f 7475 706c  c_tuple=slc_tupl
-00009a20: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00009a30: 2020 2020 6465 6c20 636f 6d70 6172 655f      del compare_
-00009a40: 6c69 7374 5b73 6c63 5d0a 2020 2020 2020  list[slc].      
-00009a50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00009a60: 6c61 6265 6c29 0a20 2020 2020 2020 2020  label).         
-00009a70: 2020 2020 2020 2070 7269 6e74 2827 4578         print('Ex
-00009a80: 7065 6374 6564 272c 2063 6f6d 7061 7265  pected', compare
-00009a90: 5f6c 6973 7429 0a20 2020 2020 2020 2020  _list).         
-00009aa0: 2020 2020 2020 2064 656c 2074 315b 736c         del t1[sl
-00009ab0: 635d 0a20 2020 2020 2020 2020 2020 2020  c].             
-00009ac0: 2020 2070 7269 6e74 2827 4f62 7365 7276     print('Observ
-00009ad0: 6564 272c 206c 6973 7428 7431 2e61 6c6c  ed', list(t1.all
-00009ae0: 2e41 2929 0a20 2020 2020 2020 2020 2020  .A)).           
-00009af0: 2020 2020 2070 7269 6e74 2829 0a20 2020       print().   
-00009b00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009b10: 662e 6173 7365 7274 4571 7561 6c28 2727  f.assertEqual(''
-00009b20: 2e6a 6f69 6e28 636f 6d70 6172 655f 6c69  .join(compare_li
-00009b30: 7374 292c 2027 272e 6a6f 696e 2874 312e  st), ''.join(t1.
-00009b40: 616c 6c2e 4129 2c20 2266 6169 6c65 6420  all.A), "failed 
-00009b50: 2220 2b20 6c61 6265 6c29 0a0a 2020 2020  " + label)..    
-00009b60: 2020 2020 6d69 6e69 5f74 6573 7428 3529      mini_test(5)
-00009b70: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
-00009b80: 7374 282d 3529 0a20 2020 2020 2020 206d  st(-5).        m
-00009b90: 696e 695f 7465 7374 2828 2d35 2c20 4e6f  ini_test((-5, No
-00009ba0: 6e65 2c20 4e6f 6e65 2929 0a20 2020 2020  ne, None)).     
-00009bb0: 2020 206d 696e 695f 7465 7374 2828 4e6f     mini_test((No
-00009bc0: 6e65 2c20 332c 204e 6f6e 6529 290a 2020  ne, 3, None)).  
-00009bd0: 2020 2020 2020 6d69 6e69 5f74 6573 7428        mini_test(
-00009be0: 284e 6f6e 652c 202d 6c65 6e28 636f 6d70  (None, -len(comp
-00009bf0: 6172 655f 6c69 7374 292b 332c 204e 6f6e  are_list)+3, Non
-00009c00: 6529 290a 2020 2020 2020 2020 6d69 6e69  e)).        mini
-00009c10: 5f74 6573 7428 284e 6f6e 652c 204e 6f6e  _test((None, Non
-00009c20: 652c 2035 2929 0a20 2020 2020 2020 206d  e, 5)).        m
-00009c30: 696e 695f 7465 7374 2828 4e6f 6e65 2c20  ini_test((None, 
-00009c40: 4e6f 6e65 2c20 2d35 2929 0a20 2020 2020  None, -5)).     
-00009c50: 2020 206d 696e 695f 7465 7374 2828 2d35     mini_test((-5
-00009c60: 2c20 2d32 2c20 4e6f 6e65 2929 0a20 2020  , -2, None)).   
-00009c70: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
-00009c80: 2d32 2c20 2d35 2c20 2d31 2929 0a20 2020  -2, -5, -1)).   
-00009c90: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
-00009ca0: 352c 2032 302c 2032 2929 0a20 2020 2020  5, 20, 2)).     
-00009cb0: 2020 206d 696e 695f 7465 7374 2828 6c65     mini_test((le
-00009cc0: 6e28 636f 6d70 6172 655f 6c69 7374 292c  n(compare_list),
-00009cd0: 2035 2c20 2d33 2929 0a20 2020 2020 2020   5, -3)).       
-00009ce0: 206d 696e 695f 7465 7374 2828 3230 2c20   mini_test((20, 
-00009cf0: 3131 2c20 2d37 2929 0a20 2020 2020 2020  11, -7)).       
-00009d00: 206d 696e 695f 7465 7374 2828 352c 2035   mini_test((5, 5
-00009d10: 2c20 4e6f 6e65 2929 0a20 2020 2020 2020  , None)).       
-00009d20: 206d 696e 695f 7465 7374 2828 4e6f 6e65   mini_test((None
-00009d30: 2c20 2d31 302c 2035 2929 0a20 2020 2020  , -10, 5)).     
-00009d40: 2020 206d 696e 695f 7465 7374 2828 4e6f     mini_test((No
-00009d50: 6e65 2c20 2d31 302c 202d 3130 2929 0a20  ne, -10, -10)). 
-00009d60: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
-00009d70: 2828 3130 3030 2c20 3230 3030 2c20 4e6f  ((1000, 2000, No
-00009d80: 6e65 2929 0a20 2020 2020 2020 206d 696e  ne)).        min
-00009d90: 695f 7465 7374 2828 4e6f 6e65 2c20 4e6f  i_test((None, No
-00009da0: 6e65 2c20 2d31 2929 0a0a 2020 2020 6465  ne, -1))..    de
-00009db0: 6620 7465 7374 5f63 6c65 6172 2873 656c  f test_clear(sel
-00009dc0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00009dd0: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-00009de0: 2020 2020 2020 6e75 6d5f 6669 656c 6473        num_fields
-00009df0: 203d 206c 656e 2873 656c 662e 7431 2e69   = len(self.t1.i
-00009e00: 6e66 6f28 295b 2266 6965 6c64 7322 5d29  nfo()["fields"])
-00009e10: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00009e20: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00009e30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00009e40: 7373 6572 7445 7175 616c 2873 656c 662e  ssertEqual(self.
-00009e50: 7465 7374 5f73 697a 6520 2a2a 206e 756d  test_size ** num
-00009e60: 5f66 6965 6c64 732c 206c 656e 2873 656c  _fields, len(sel
-00009e70: 662e 7431 292c 2022 696e 7661 6c69 6420  f.t1), "invalid 
-00009e80: 6c65 6e22 290a 2020 2020 2020 2020 7365  len").        se
-00009e90: 6c66 2e74 312e 6372 6561 7465 5f69 6e64  lf.t1.create_ind
-00009ea0: 6578 2822 6122 290a 0a20 2020 2020 2020  ex("a")..       
-00009eb0: 2073 656c 662e 7431 2e63 6c65 6172 2829   self.t1.clear()
-00009ec0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00009ed0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00009ee0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00009ef0: 7373 6572 7445 7175 616c 2830 2c20 6c65  ssertEqual(0, le
-00009f00: 6e28 7365 6c66 2e74 3129 2c20 2269 6e76  n(self.t1), "inv
-00009f10: 616c 6964 206c 656e 2061 6674 6572 2063  alid len after c
-00009f20: 6c65 6172 2229 0a20 2020 2020 2020 2077  lear").        w
-00009f30: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00009f40: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00009f50: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00009f60: 2831 2c20 6c65 6e28 7365 6c66 2e74 312e  (1, len(self.t1.
-00009f70: 696e 666f 2829 5b22 696e 6465 7865 7322  info()["indexes"
-00009f80: 5d29 2c20 2269 6e76 616c 6964 2069 6e64  ]), "invalid ind
-00009f90: 6578 6573 2061 6674 6572 2063 6c65 6172  exes after clear
-00009fa0: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-00009fb0: 5f73 7461 7473 2873 656c 6629 3a0a 2020  _stats(self):.  
-00009fc0: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
-00009fd0: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
-00009fe0: 6669 656c 645f 6e61 6d65 7320 3d20 7365  field_names = se
-00009ff0: 6c66 2e74 312e 696e 666f 2829 5b22 6669  lf.t1.info()["fi
-0000a000: 656c 6473 225d 0a20 2020 2020 2020 206e  elds"].        n
-0000a010: 756d 5f66 6965 6c64 7320 3d20 6c65 6e28  um_fields = len(
-0000a020: 6669 656c 645f 6e61 6d65 7329 0a20 2020  field_names).   
-0000a030: 2020 2020 2074 315f 7374 6174 7320 3d20       t1_stats = 
-0000a040: 7365 6c66 2e74 312e 7374 6174 7328 292e  self.t1.stats().
-0000a050: 7365 6c65 6374 2822 6e61 6d65 2063 6f75  select("name cou
-0000a060: 6e74 206d 696e 206d 6178 206d 6561 6e22  nt min max mean"
-0000a070: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
-0000a080: 656c 646e 616d 6520 696e 2066 6965 6c64  eldname in field
-0000a090: 5f6e 616d 6573 3a0a 2020 2020 2020 2020  _names:.        
-0000a0a0: 2020 2020 7374 6174 5f72 6563 203d 2074      stat_rec = t
-0000a0b0: 315f 7374 6174 732e 6279 2e6e 616d 655b  1_stats.by.name[
-0000a0c0: 6669 656c 646e 616d 655d 0a20 2020 2020  fieldname].     
-0000a0d0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000a0e0: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
-0000a0f0: 636f 6d70 7574 6564 2073 7461 7422 2c20  computed stat", 
-0000a100: 6669 656c 646e 616d 653d 6669 656c 646e  fieldname=fieldn
-0000a110: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-0000a120: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a130: 7445 7175 616c 286c 742e 4461 7461 4f62  tEqual(lt.DataOb
-0000a140: 6a65 6374 286e 616d 653d 6669 656c 646e  ject(name=fieldn
-0000a150: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 636f 756e 743d 7365 6c66 2e74      count=self.t
-0000a190: 6573 745f 7369 7a65 202a 2a20 6e75 6d5f  est_size ** num_
-0000a1a0: 6669 656c 6473 2c0a 2020 2020 2020 2020  fields,.        
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 206d 696e 3d30 2c0a 2020         min=0,.  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 2020 2020 2020 2020 2020 206d 6178               max
-0000a210: 3d73 656c 662e 7465 7374 5f73 697a 6520  =self.test_size 
-0000a220: 2d20 312c 0a20 2020 2020 2020 2020 2020  - 1,.           
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 2020 6d65 616e 3d28 7365 6c66 2e74      mean=(self.t
-0000a260: 6573 745f 7369 7a65 202d 2031 2920 2f20  est_size - 1) / 
-0000a270: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2073 7461 745f 7265 632c 0a20       stat_rec,. 
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 6622 696e 7661 6c69 6420 7374 6174 2066  f"invalid stat f
-0000a2d0: 6f72 207b 6669 656c 646e 616d 657d 2229  or {fieldname}")
-0000a2e0: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
-0000a2f0: 7461 7473 3228 7365 6c66 293a 0a20 2020  tats2(self):.   
-0000a300: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-0000a310: 696e 6974 2829 0a20 2020 2020 2020 2066  init().        f
-0000a320: 6965 6c64 5f6e 616d 6573 203d 2073 656c  ield_names = sel
-0000a330: 662e 7431 2e69 6e66 6f28 295b 2266 6965  f.t1.info()["fie
-0000a340: 6c64 7322 5d0a 2020 2020 2020 2020 6e75  lds"].        nu
-0000a350: 6d5f 6669 656c 6473 203d 206c 656e 2866  m_fields = len(f
-0000a360: 6965 6c64 5f6e 616d 6573 290a 2020 2020  ield_names).    
-0000a370: 2020 2020 7431 5f73 7461 7473 203d 2073      t1_stats = s
-0000a380: 656c 662e 7431 2e73 7461 7473 2862 795f  elf.t1.stats(by_
-0000a390: 6669 656c 643d 4661 6c73 6529 0a20 2020  field=False).   
-0000a3a0: 2020 2020 2066 6f72 2073 7461 742c 2076       for stat, v
-0000a3b0: 616c 7565 2069 6e20 2828 276d 696e 272c  alue in (('min',
-0000a3c0: 2030 292c 2028 276d 6178 272c 2073 656c   0), ('max', sel
-0000a3d0: 662e 7465 7374 5f73 697a 6520 2d20 3129  f.test_size - 1)
-0000a3e0: 2c20 2827 636f 756e 7427 2c20 7365 6c66  , ('count', self
-0000a3f0: 2e74 6573 745f 7369 7a65 202a 2a20 6e75  .test_size ** nu
-0000a400: 6d5f 6669 656c 6473 292c 293a 0a20 2020  m_fields),):.   
-0000a410: 2020 2020 2020 2020 2066 6f72 2066 6965           for fie
-0000a420: 6c64 6e61 6d65 2069 6e20 6669 656c 645f  ldname in field_
-0000a430: 6e61 6d65 733a 0a20 2020 2020 2020 2020  names:.         
-0000a440: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000a450: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
-0000a460: 636f 6d70 7574 6564 2073 7461 7422 2c20  computed stat", 
-0000a470: 7374 6174 3d73 7461 742c 2066 6965 6c64  stat=stat, field
-0000a480: 6e61 6d65 3d66 6965 6c64 6e61 6d65 293a  name=fieldname):
-0000a490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000a4b0: 4571 7561 6c28 7661 6c75 652c 2067 6574  Equal(value, get
-0000a4c0: 6174 7472 2874 315f 7374 6174 732e 6279  attr(t1_stats.by
-0000a4d0: 2e73 7461 745b 7374 6174 5d2c 2066 6965  .stat[stat], fie
-0000a4e0: 6c64 6e61 6d65 292c 0a20 2020 2020 2020  ldname),.       
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2020 2020 2020 2a2a 6b77 6172 6773 297d        **kwargs)}
+00005d40: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00005d50: 696e 7428 5b73 7472 2861 2920 666f 7220  int([str(a) for 
+00005d60: 6120 696e 2074 626c 2e61 6c6c 2e61 5d29  a in tbl.all.a])
+00005d70: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00005d80: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00005d90: 2274 6573 7420 5461 626c 652e 7061 7273  "test Table.pars
+00005da0: 655f 6461 7465 5f74 696d 6520 6572 726f  e_date_time erro
+00005db0: 7273 222c 202a 2a6b 7761 7267 7329 3a0a  rs", **kwargs):.
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00005de0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005df0: 2020 2020 2020 5b6b 7761 7267 735b 226f        [kwargs["o
+00005e00: 6e5f 6572 726f 7222 5d2c 206b 7761 7267  n_error"], kwarg
+00005e10: 735b 2265 6d70 7479 225d 5d2c 0a20 2020  s["empty"]],.   
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 206c 6973 7428 7462 6c2e 616c 6c2e 6129   list(tbl.all.a)
+00005e40: 5b2d 323a 5d0a 2020 2020 2020 2020 2020  [-2:].          
+00005e50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00005e60: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00005e70: 7562 5465 7374 2822 7465 7374 2054 6162  ubTest("test Tab
+00005e80: 6c65 2e70 6172 7365 5f64 6174 655f 7469  le.parse_date_ti
+00005e90: 6d65 2076 616c 6964 222c 202a 2a6b 7761  me valid", **kwa
+00005ea0: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
+00005eb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00005ec0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+00005ed0: 2020 2020 2020 2020 2020 2020 5b64 6174              [dat
+00005ee0: 6574 696d 652e 6461 7465 2832 3030 312c  etime.date(2001,
+00005ef0: 2031 2c20 3129 2c0a 2020 2020 2020 2020   1, 1),.        
+00005f00: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00005f10: 6574 696d 652e 6461 7465 2832 3030 312c  etime.date(2001,
+00005f20: 2031 2c20 3229 5d2c 0a20 2020 2020 2020   1, 2)],.       
+00005f30: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00005f40: 7428 7462 6c2e 616c 6c2e 6129 5b3a 325d  t(tbl.all.a)[:2]
+00005f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f60: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
+00005f70: 5f70 6172 7365 5f74 696d 6564 656c 7461  _parse_timedelta
+00005f80: 5f74 7261 6e73 666f 726d 2873 656c 6629  _transform(self)
+00005f90: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
+00005fa0: 2064 6174 6574 696d 650a 0a20 2020 2020   datetime..     
+00005fb0: 2020 2070 726f 6365 7373 5f64 6174 6120     process_data 
+00005fc0: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
+00005fd0: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
+00005fe0: 2020 2065 6c61 7073 6564 5f74 696d 652c     elapsed_time,
+00005ff0: 6571 7074 2c65 7665 6e74 2c6c 6f74 2c70  eqpt,event,lot,p
+00006000: 6965 6365 730a 2020 2020 2020 2020 2020  ieces.          
+00006010: 2020 303a 3030 3a30 302c 4452 494c 4c30    0:00:00,DRILL0
+00006020: 312c 4c6f 7453 7461 7274 2c50 4342 3134  1,LotStart,PCB14
+00006030: 362c 310a 2020 2020 2020 2020 2020 2020  6,1.            
+00006040: 303a 3030 3a34 302c 4452 494c 4c30 312c  0:00:40,DRILL01,
+00006050: 546f 6f6c 312c 5043 4231 3436 2c32 0a20  Tool1,PCB146,2. 
+00006060: 2020 2020 2020 2020 2020 2030 3a30 333a             0:03:
+00006070: 3435 2c44 5249 4c4c 3031 2c54 6f6f 6c32  45,DRILL01,Tool2
+00006080: 2c50 4342 3134 362c 340a 2020 2020 2020  ,PCB146,4.      
+00006090: 2020 2020 2020 303a 3036 3a31 362c 4452        0:06:16,DR
+000060a0: 494c 4c30 312c 4c6f 7445 6e64 2c50 4342  ILL01,LotEnd,PCB
+000060b0: 3134 362c 380a 2020 2020 2020 2020 2020  146,8.          
+000060c0: 2020 2222 2229 0a0a 2020 2020 2020 2020    """)..        
+000060d0: 7472 616e 7366 6f72 6d73 203d 207b 2765  transforms = {'e
+000060e0: 6c61 7073 6564 5f74 696d 6527 3a20 6c74  lapsed_time': lt
+000060f0: 2e54 6162 6c65 2e70 6172 7365 5f74 696d  .Table.parse_tim
+00006100: 6564 656c 7461 2822 2548 3a25 4d3a 2553  edelta("%H:%M:%S
+00006110: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00006120: 2020 2020 2020 2020 2020 2770 6965 6365            'piece
+00006130: 7327 3a20 696e 747d 0a20 2020 2020 2020  s': int}.       
+00006140: 2064 6174 6120 3d20 6c74 2e54 6162 6c65   data = lt.Table
+00006150: 2866 2250 726f 6365 7373 2073 7465 7020  (f"Process step 
+00006160: 656c 6170 7365 6420 7469 6d65 7322 292e  elapsed times").
+00006170: 6373 765f 696d 706f 7274 2870 726f 6365  csv_import(proce
+00006180: 7373 5f64 6174 612c 2074 7261 6e73 666f  ss_data, transfo
+00006190: 726d 733d 7472 616e 7366 6f72 6d73 290a  rms=transforms).
+000061a0: 2020 2020 2020 2020 6461 7461 2e63 7265          data.cre
+000061b0: 6174 655f 696e 6465 7828 2265 6c61 7073  ate_index("elaps
+000061c0: 6564 5f74 696d 6522 290a 0a20 2020 2020  ed_time")..     
+000061d0: 2020 205f 3030 5f30 315f 3330 203d 2064     _00_01_30 = d
+000061e0: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
+000061f0: 6128 7365 636f 6e64 733d 3930 290a 2020  a(seconds=90).  
+00006200: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00006210: 7445 7175 616c 2833 2c20 7375 6d28 6461  tEqual(3, sum(da
+00006220: 7461 2e62 792e 656c 6170 7365 645f 7469  ta.by.elapsed_ti
+00006230: 6d65 5b3a 5f30 305f 3031 5f33 305d 2e61  me[:_00_01_30].a
+00006240: 6c6c 2e70 6965 6365 7329 290a 0a20 2020  ll.pieces))..   
+00006250: 2064 6566 2074 6573 745f 736c 6963 6564   def test_sliced
+00006260: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
+00006270: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
+00006280: 726d 7320 3d20 7b0a 2020 2020 2020 2020  rms = {.        
+00006290: 2020 2020 2770 6f70 273a 2069 6e74 2c0a      'pop': int,.
+000062a0: 2020 2020 2020 2020 2020 2020 2765 6c65              'ele
+000062b0: 7627 3a20 696e 742c 0a20 2020 2020 2020  v': int,.       
+000062c0: 2020 2020 2027 6c61 7427 3a20 666c 6f61       'lat': floa
+000062d0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+000062e0: 6c6f 6e67 273a 2066 6c6f 6174 2c0a 2020  long': float,.  
+000062f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00006300: 7573 5f70 706c 203d 206c 742e 5461 626c  us_ppl = lt.Tabl
+00006310: 6528 292e 6373 765f 696d 706f 7274 2822  e().csv_import("
+00006320: 6578 616d 706c 6573 2f75 735f 7070 6c2e  examples/us_ppl.
+00006330: 6373 7622 2c0a 2020 2020 2020 2020 2020  csv",.          
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00006360: 6e73 666f 726d 733d 7472 616e 7366 6f72  nsforms=transfor
+00006370: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2020 2020 2029 2e73 656c             ).sel
+000063a0: 6563 7428 2269 6420 6e61 6d65 2065 6c65  ect("id name ele
+000063b0: 7620 6c61 7420 6c6f 6e67 2070 6f70 2229  v lat long pop")
+000063c0: 0a20 2020 2020 2020 2070 7269 6e74 2875  .        print(u
+000063d0: 735f 7070 6c2e 696e 666f 2829 290a 2020  s_ppl.info()).  
+000063e0: 2020 2020 2020 7573 5f70 706c 2e63 7265        us_ppl.cre
+000063f0: 6174 655f 696e 6465 7828 226e 616d 6522  ate_index("name"
+00006400: 290a 2020 2020 2020 2020 7573 5f70 706c  ).        us_ppl
+00006410: 2e63 7265 6174 655f 696e 6465 7828 2265  .create_index("e
+00006420: 6c65 7622 290a 0a20 2020 2020 2020 2074  lev")..        t
+00006430: 6573 7420 3d20 2265 6c65 7620 3c20 3022  est = "elev < 0"
+00006440: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
+00006450: 5f77 6865 7265 203d 2075 735f 7070 6c2e  _where = us_ppl.
+00006460: 7768 6572 6528 656c 6576 3d6c 742e 5461  where(elev=lt.Ta
+00006470: 626c 652e 6c74 2830 2929 2874 6573 7429  ble.lt(0))(test)
+00006480: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
+00006490: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
+000064a0: 6279 2e65 6c65 765b 3a30 5d28 6622 7b74  by.elev[:0](f"{t
+000064b0: 6573 747d 2028 736c 6963 6564 2922 290a  est} (sliced)").
+000064c0: 2020 2020 2020 2020 6c6f 775f 7070 6c5f          low_ppl_
+000064d0: 736c 6963 652e 7072 6573 656e 7428 290a  slice.present().
+000064e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000064f0: 6572 7445 7175 616c 286c 6973 7428 6c6f  ertEqual(list(lo
+00006500: 775f 7070 6c5f 7768 6572 652e 616c 6c2e  w_ppl_where.all.
+00006510: 6964 292c 206c 6973 7428 6c6f 775f 7070  id), list(low_pp
+00006520: 6c5f 736c 6963 652e 616c 6c2e 6964 2929  l_slice.all.id))
+00006530: 0a0a 2020 2020 2020 2020 7465 7374 203d  ..        test =
+00006540: 2022 656c 6576 203e 3d20 3130 3030 220a   "elev >= 1000".
+00006550: 2020 2020 2020 2020 6869 5f70 706c 5f77          hi_ppl_w
+00006560: 6865 7265 203d 2075 735f 7070 6c2e 7768  here = us_ppl.wh
+00006570: 6572 6528 656c 6576 3d6c 742e 5461 626c  ere(elev=lt.Tabl
+00006580: 652e 6765 2831 3030 3029 2928 7465 7374  e.ge(1000))(test
+00006590: 290a 2020 2020 2020 2020 6869 5f70 706c  ).        hi_ppl
+000065a0: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
+000065b0: 6279 2e65 6c65 765b 3130 3030 3a5d 2866  by.elev[1000:](f
+000065c0: 227b 7465 7374 7d20 2873 6c69 6365 6429  "{test} (sliced)
+000065d0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000065e0: 6173 7365 7274 4571 7561 6c28 6c69 7374  assertEqual(list
+000065f0: 2868 695f 7070 6c5f 7768 6572 652e 616c  (hi_ppl_where.al
+00006600: 6c2e 6964 292c 206c 6973 7428 6869 5f70  l.id), list(hi_p
+00006610: 706c 5f73 6c69 6365 2e61 6c6c 2e69 6429  pl_slice.all.id)
+00006620: 290a 0a20 2020 2020 2020 2074 6573 7420  )..        test 
+00006630: 3d20 2230 203c 3d20 656c 6576 203c 2031  = "0 <= elev < 1
+00006640: 3030 220a 2020 2020 2020 2020 6c6f 775f  00".        low_
+00006650: 7070 6c5f 7768 6572 6520 3d20 7573 5f70  ppl_where = us_p
+00006660: 706c 2e77 6865 7265 2865 6c65 763d 6c74  pl.where(elev=lt
+00006670: 2e54 6162 6c65 2e67 6528 3029 292e 7768  .Table.ge(0)).wh
+00006680: 6572 6528 656c 6576 3d6c 742e 5461 626c  ere(elev=lt.Tabl
+00006690: 652e 6c74 2831 3030 2929 2874 6573 7429  e.lt(100))(test)
+000066a0: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
+000066b0: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
+000066c0: 6279 2e65 6c65 765b 303a 3130 305d 2866  by.elev[0:100](f
+000066d0: 227b 7465 7374 7d20 2873 6c69 6365 6429  "{test} (sliced)
+000066e0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000066f0: 6173 7365 7274 4571 7561 6c28 6c69 7374  assertEqual(list
+00006700: 286c 6f77 5f70 706c 5f77 6865 7265 2e61  (low_ppl_where.a
+00006710: 6c6c 2e69 6429 2c20 6c69 7374 286c 6f77  ll.id), list(low
+00006720: 5f70 706c 5f73 6c69 6365 2e61 6c6c 2e69  _ppl_slice.all.i
+00006730: 6429 290a 0a20 2020 2020 2020 2061 5f70  d))..        a_p
+00006740: 706c 5f77 6865 7265 203d 2075 735f 7070  pl_where = us_pp
+00006750: 6c2e 7768 6572 6528 6e61 6d65 3d6c 742e  l.where(name=lt.
+00006760: 5461 626c 652e 6765 2822 4122 2929 2e77  Table.ge("A")).w
+00006770: 6865 7265 286e 616d 653d 6c74 2e54 6162  here(name=lt.Tab
+00006780: 6c65 2e6c 7428 2243 2229 290a 2020 2020  le.lt("C")).    
+00006790: 2020 2020 615f 7070 6c5f 736c 6963 6520      a_ppl_slice 
+000067a0: 3d20 7573 5f70 706c 2e62 792e 6e61 6d65  = us_ppl.by.name
+000067b0: 5b22 4122 3a22 4322 5d0a 2020 2020 2020  ["A":"C"].      
+000067c0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000067d0: 616c 286c 6973 7428 615f 7070 6c5f 7768  al(list(a_ppl_wh
+000067e0: 6572 652e 616c 6c2e 6964 292c 206c 6973  ere.all.id), lis
+000067f0: 7428 615f 7070 6c5f 736c 6963 652e 616c  t(a_ppl_slice.al
+00006800: 6c2e 6964 2929 0a0a 2020 2020 6465 6620  l.id))..    def 
+00006810: 7465 7374 5f6e 6f6e 5f69 6e74 6567 6572  test_non_integer
+00006820: 5f73 6c69 6365 645f 696e 6465 7869 6e67  _sliced_indexing
+00006830: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006840: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
+00006850: 0a20 2020 2020 2020 2073 616c 6573 5f64  .        sales_d
+00006860: 6174 6120 3d20 7465 7874 7772 6170 2e64  ata = textwrap.d
+00006870: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
+00006880: 2020 2020 2020 2064 6174 652c 6375 7374         date,cust
+00006890: 6f6d 6572 2c73 6b75 2c71 7479 0a20 2020  omer,sku,qty.   
+000068a0: 2020 2020 2020 2020 2032 3030 302f 3031           2000/01
+000068b0: 2f30 312c 3030 3230 2c41 4e56 494c 2d30  /01,0020,ANVIL-0
+000068c0: 3031 2c31 0a20 2020 2020 2020 2020 2020  01,1.           
+000068d0: 2032 3030 302f 3031 2f30 312c 3030 3230   2000/01/01,0020
+000068e0: 2c42 5244 5344 2d30 3031 2c32 0a20 2020  ,BRDSD-001,2.   
+000068f0: 2020 2020 2020 2020 2032 3030 302f 3032           2000/02
+00006900: 2f31 352c 3030 3230 2c42 5244 5344 2d30  /15,0020,BRDSD-0
+00006910: 3031 2c34 0a20 2020 2020 2020 2020 2020  01,4.           
+00006920: 2032 3030 302f 3033 2f33 312c 3030 3230   2000/03/31,0020
+00006930: 2c42 5244 5344 2d30 3031 2c38 0a20 2020  ,BRDSD-001,8.   
+00006940: 2020 2020 2020 2020 2032 3030 302f 3033           2000/03
+00006950: 2f33 312c 3030 3230 2c4d 4147 4e54 2d30  /31,0020,MAGNT-0
+00006960: 3031 2c31 360a 2020 2020 2020 2020 2020  01,16.          
+00006970: 2020 3230 3030 2f30 342f 3031 2c30 3032    2000/04/01,002
+00006980: 302c 524f 424f 542d 3030 312c 3332 0a20  0,ROBOT-001,32. 
+00006990: 2020 2020 2020 2020 2020 2032 3030 302f             2000/
+000069a0: 3034 2f31 352c 3030 3230 2c42 5244 5344  04/15,0020,BRDSD
+000069b0: 2d30 3031 2c36 340a 2020 2020 2020 2020  -001,64.        
+000069c0: 2020 2020 2222 2229 0a0a 2020 2020 2020      """)..      
+000069d0: 2020 7472 616e 7366 6f72 6d73 203d 207b    transforms = {
+000069e0: 2764 6174 6527 3a20 6c74 2e54 6162 6c65  'date': lt.Table
+000069f0: 2e70 6172 7365 5f64 6174 6528 2225 592f  .parse_date("%Y/
+00006a00: 256d 2f25 6422 292c 0a20 2020 2020 2020  %m/%d"),.       
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006a20: 7174 7927 3a20 696e 747d 0a20 2020 2020  qty': int}.     
+00006a30: 2020 2073 616c 6573 203d 206c 742e 5461     sales = lt.Ta
+00006a40: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00006a50: 2873 616c 6573 5f64 6174 612c 0a20 2020  (sales_data,.   
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 2020 2074 7261 6e73 666f 726d 733d 7472     transforms=tr
+00006a90: 616e 7366 6f72 6d73 2c29 0a0a 2020 2020  ansforms,)..    
+00006aa0: 2020 2020 7361 6c65 732e 6372 6561 7465      sales.create
+00006ab0: 5f69 6e64 6578 2822 6461 7465 2229 0a20  _index("date"). 
+00006ac0: 2020 2020 2020 206a 616e 5f30 3120 3d20         jan_01 = 
+00006ad0: 6461 7465 7469 6d65 2e64 6174 6528 3230  datetime.date(20
+00006ae0: 3030 2c20 312c 2031 290a 2020 2020 2020  00, 1, 1).      
+00006af0: 2020 6170 725f 3031 203d 2064 6174 6574    apr_01 = datet
+00006b00: 696d 652e 6461 7465 2832 3030 302c 2034  ime.date(2000, 4
+00006b10: 2c20 3129 0a20 2020 2020 2020 2066 6972  , 1).        fir
+00006b20: 7374 5f71 7472 5f73 616c 6573 203d 2073  st_qtr_sales = s
+00006b30: 616c 6573 2e62 792e 6461 7465 5b6a 616e  ales.by.date[jan
+00006b40: 5f30 313a 2061 7072 5f30 315d 0a20 2020  _01: apr_01].   
+00006b50: 2020 2020 2066 6972 7374 5f71 7472 5f73       first_qtr_s
+00006b60: 616c 6573 2e70 7265 7365 6e74 2829 0a20  ales.present(). 
+00006b70: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
+00006b80: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
+00006b90: 732e 616c 6c2e 736b 7529 290a 0a20 2020  s.all.sku))..   
+00006ba0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00006bb0: 4571 7561 6c28 6c69 7374 2866 6972 7374  Equal(list(first
+00006bc0: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
+00006bd0: 6b75 292c 0a20 2020 2020 2020 2020 2020  ku),.           
+00006be0: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
+00006bf0: 414e 5649 4c2d 3030 3127 2c20 2742 5244  ANVIL-001', 'BRD
+00006c00: 5344 2d30 3031 272c 2027 4252 4453 442d  SD-001', 'BRDSD-
+00006c10: 3030 3127 2c20 2742 5244 5344 2d30 3031  001', 'BRDSD-001
+00006c20: 272c 2027 4d41 474e 542d 3030 3127 5d2c  ', 'MAGNT-001'],
+00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00006c50: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00006c60: 7175 616c 2833 312c 2073 756d 2866 6972  qual(31, sum(fir
+00006c70: 7374 5f71 7472 5f73 616c 6573 2e61 6c6c  st_qtr_sales.all
+00006c80: 2e71 7479 2929 0a0a 2020 2020 2020 2020  .qty))..        
+00006c90: 2320 7573 6520 6461 7465 2073 7472 696e  # use date strin
+00006ca0: 6773 2061 7320 7261 6e67 6520 7661 6c75  gs as range valu
+00006cb0: 6573 0a20 2020 2020 2020 2074 7261 6e73  es.        trans
+00006cc0: 666f 726d 7320 3d20 7b27 7174 7927 3a20  forms = {'qty': 
+00006cd0: 696e 747d 0a20 2020 2020 2020 2073 616c  int}.        sal
+00006ce0: 6573 203d 206c 742e 5461 626c 6528 292e  es = lt.Table().
+00006cf0: 6373 765f 696d 706f 7274 2873 616c 6573  csv_import(sales
+00006d00: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d20: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00006d30: 6e73 666f 726d 733d 7472 616e 7366 6f72  nsforms=transfor
+00006d40: 6d73 2c29 0a0a 2020 2020 2020 2020 7361  ms,)..        sa
+00006d50: 6c65 732e 6372 6561 7465 5f69 6e64 6578  les.create_index
+00006d60: 2822 6461 7465 2229 0a20 2020 2020 2020  ("date").       
+00006d70: 2066 6972 7374 5f71 7472 5f73 616c 6573   first_qtr_sales
+00006d80: 203d 2073 616c 6573 2e62 792e 6461 7465   = sales.by.date
+00006d90: 5b22 3230 3030 2f30 312f 3031 223a 2022  ["2000/01/01": "
+00006da0: 3230 3030 2f30 342f 3031 225d 0a20 2020  2000/04/01"].   
+00006db0: 2020 2020 2066 6972 7374 5f71 7472 5f73       first_qtr_s
+00006dc0: 616c 6573 2e70 7265 7365 6e74 2829 0a20  ales.present(). 
+00006dd0: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
+00006de0: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
+00006df0: 732e 616c 6c2e 736b 7529 290a 0a20 2020  s.all.sku))..   
+00006e00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00006e10: 4571 7561 6c28 6c69 7374 2866 6972 7374  Equal(list(first
+00006e20: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
+00006e30: 6b75 292c 0a20 2020 2020 2020 2020 2020  ku),.           
+00006e40: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
+00006e50: 414e 5649 4c2d 3030 3127 2c20 2742 5244  ANVIL-001', 'BRD
+00006e60: 5344 2d30 3031 272c 2027 4252 4453 442d  SD-001', 'BRDSD-
+00006e70: 3030 3127 2c20 2742 5244 5344 2d30 3031  001', 'BRDSD-001
+00006e80: 272c 2027 4d41 474e 542d 3030 3127 5d2c  ', 'MAGNT-001'],
+00006e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006ea0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00006eb0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00006ec0: 7175 616c 2833 312c 2073 756d 2866 6972  qual(31, sum(fir
+00006ed0: 7374 5f71 7472 5f73 616c 6573 2e61 6c6c  st_qtr_sales.all
+00006ee0: 2e71 7479 2929 0a0a 2020 2020 2020 2020  .qty))..        
+00006ef0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00006f00: 2833 312c 2073 756d 2873 616c 6573 2e62  (31, sum(sales.b
+00006f10: 792e 6461 7465 5b3a 2232 3030 302f 3034  y.date[:"2000/04
+00006f20: 2f30 3122 5d2e 616c 6c2e 7174 7929 290a  /01"].all.qty)).
+00006f30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006f40: 6572 7445 7175 616c 2839 362c 2073 756d  ertEqual(96, sum
+00006f50: 2873 616c 6573 2e62 792e 6461 7465 5b22  (sales.by.date["
+00006f60: 3230 3030 2f30 342f 3031 223a 5d2e 616c  2000/04/01":].al
+00006f70: 6c2e 7174 7929 290a 0a20 2020 2064 6566  l.qty))..    def
+00006f80: 2074 6573 745f 696e 6465 785f 6469 7228   test_index_dir(
+00006f90: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
+00006fa0: 6861 7273 203d 2022 4142 4344 4546 4748  hars = "ABCDEFGH
+00006fb0: 494a 4b4c 4d4e 4f50 5152 5354 5556 5758  IJKLMNOPQRSTUVWX
+00006fc0: 595a 220a 2020 2020 2020 2020 6d61 6b65  YZ".        make
+00006fd0: 5f72 6563 203d 206c 616d 6264 6120 6161  _rec = lambda aa
+00006fe0: 2c20 6262 2c20 6363 3a20 7365 6c66 2e6d  , bb, cc: self.m
+00006ff0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00007000: 6368 6172 735b 6161 2025 206c 656e 2863  chars[aa % len(c
+00007010: 6861 7273 295d 2c0a 2020 2020 2020 2020  hars)],.        
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 2020 6368 6172 735b 6262 2025 206c      chars[bb % l
+00007060: 656e 2863 6861 7273 295d 2c0a 2020 2020  en(chars)],.    
+00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 2020 2020 2020 2020 6368 6172 735b 6363          chars[cc
+000070b0: 2025 206c 656e 2863 6861 7273 295d 290a   % len(chars)]).
+000070c0: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
+000070d0: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
+000070e0: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
+000070f0: 5f74 6162 6c65 286d 616b 655f 7265 632c  _table(make_rec,
+00007100: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
+00007110: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
+00007120: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
+00007130: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
+00007140: 5f69 6e64 6578 2827 6227 290a 0a20 2020  _index('b')..   
+00007150: 2020 2020 2064 6972 5f6c 6973 7420 3d20       dir_list = 
+00007160: 6469 7228 7461 626c 652e 6279 290a 2020  dir(table.by).  
+00007170: 2020 2020 2020 7072 696e 7428 5b61 7474        print([att
+00007180: 7220 666f 7220 6174 7472 2069 6e20 6469  r for attr in di
+00007190: 725f 6c69 7374 2069 6620 6e6f 7420 6174  r_list if not at
+000071a0: 7472 2e73 7461 7274 7377 6974 6828 225f  tr.startswith("_
+000071b0: 2229 5d29 0a0a 2020 2020 2020 2020 7365  ")])..        se
+000071c0: 6c66 2e61 7373 6572 7454 7275 6528 2827  lf.assertTrue(('
+000071d0: 6127 2069 6e20 6469 725f 6c69 7374 2920  a' in dir_list) 
+000071e0: 616e 6420 2827 6227 2069 6e20 6469 725f  and ('b' in dir_
+000071f0: 6c69 7374 2920 616e 6420 2827 6327 206e  list) and ('c' n
+00007200: 6f74 2069 6e20 6469 725f 6c69 7374 2929  ot in dir_list))
+00007210: 0a0a 2020 2020 6465 6620 7465 7374 5f64  ..    def test_d
+00007220: 656c 6574 655f 6279 5f66 696c 7465 7228  elete_by_filter(
+00007230: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+00007240: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
+00007250: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+00007260: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+00007270: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00007280: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+00007290: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000072a0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+000072b0: 697a 652a 7465 7374 5f73 697a 652c 2074  ize*test_size, t
+000072c0: 6162 6c65 2e64 656c 6574 6528 623d 3529  able.delete(b=5)
+000072d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000072e0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+000072f0: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
+00007300: 7465 7374 5f73 697a 652d 3129 2c20 6c65  test_size-1), le
+00007310: 6e28 7461 626c 6529 290a 2020 2020 2020  n(table)).      
+00007320: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007330: 616c 2830 2c20 7461 626c 652e 6465 6c65  al(0, table.dele
+00007340: 7465 2862 3d2d 3129 290a 2020 2020 2020  te(b=-1)).      
+00007350: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007360: 616c 2830 2c20 7461 626c 652e 6465 6c65  al(0, table.dele
+00007370: 7465 2829 290a 0a20 2020 2064 6566 2074  te())..    def t
+00007380: 6573 745f 7265 6d6f 7665 5f6d 616e 7928  est_remove_many(
+00007390: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+000073a0: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
+000073b0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+000073c0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+000073d0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000073e0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+000073f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007400: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00007410: 697a 652a 7465 7374 5f73 697a 652a 7465  ize*test_size*te
+00007420: 7374 5f73 697a 652f 322c 206c 656e 2874  st_size/2, len(t
+00007430: 6162 6c65 2e77 6865 7265 286c 616d 6264  able.where(lambd
+00007440: 6120 743a 2074 2e61 2025 2032 2929 290a  a t: t.a % 2))).
+00007450: 2020 2020 2020 2020 7461 626c 652e 7265          table.re
+00007460: 6d6f 7665 5f6d 616e 7928 7461 626c 652e  move_many(table.
+00007470: 7768 6572 6528 6c61 6d62 6461 2074 3a20  where(lambda t: 
+00007480: 742e 6120 2520 3229 290a 2020 2020 2020  t.a % 2)).      
+00007490: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000074a0: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
+000074b0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+000074c0: 2f32 2c20 6c65 6e28 7461 626c 6529 290a  /2, len(table)).
+000074d0: 2020 2020 2020 2020 7461 626c 655f 6c65          table_le
+000074e0: 6e20 3d20 6c65 6e28 7461 626c 6529 0a20  n = len(table). 
+000074f0: 2020 2020 2020 2074 6162 6c65 2e72 656d         table.rem
+00007500: 6f76 6528 7461 626c 655b 315d 290a 2020  ove(table[1]).  
+00007510: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00007520: 7445 7175 616c 2874 6162 6c65 5f6c 656e  tEqual(table_len
+00007530: 2d31 2c20 6c65 6e28 7461 626c 6529 290a  -1, len(table)).
+00007540: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
+00007550: 645f 6e65 775f 6669 656c 6428 7365 6c66  d_new_field(self
+00007560: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+00007570: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00007580: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00007590: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+000075a0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+000075b0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+000075c0: 2020 2020 2023 206f 6e6c 7920 4461 7461       # only Data
+000075d0: 4f62 6a65 6374 7320 6172 6520 6d75 7461  Objects are muta
+000075e0: 626c 6520 696e 2074 6865 7365 2074 6573  ble in these tes
+000075f0: 7473 0a20 2020 2020 2020 2069 6620 6973  ts.        if is
+00007600: 696e 7374 616e 6365 2874 6162 6c65 5b30  instance(table[0
+00007610: 5d2c 206c 742e 4461 7461 4f62 6a65 6374  ], lt.DataObject
+00007620: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00007630: 6162 6c65 2e61 6464 5f66 6965 6c64 2827  able.add_field('
+00007640: 6427 2c20 6c61 6d62 6461 2072 6563 3a20  d', lambda rec: 
+00007650: 7265 632e 612b 7265 632e 622b 7265 632e  rec.a+rec.b+rec.
+00007660: 6329 0a0a 2020 2020 2020 2020 2020 2020  c)..            
+00007670: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+00007680: 6578 2827 6427 290a 2020 2020 2020 2020  ex('d').        
+00007690: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000076a0: 7175 616c 286c 656e 2872 616e 6765 2830  qual(len(range(0
+000076b0: 2c20 3237 2b31 2929 2c20 6c65 6e28 7461  , 27+1)), len(ta
+000076c0: 626c 652e 6279 2e64 2e6b 6579 7328 2929  ble.by.d.keys())
+000076d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000076e0: 6164 645f 7477 6f5f 7461 626c 6573 2873  add_two_tables(s
+000076f0: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
+00007700: 7374 5f73 697a 6520 3d20 3130 0a20 2020  st_size = 10.   
+00007710: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
+00007720: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00007730: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00007740: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
+00007750: 2020 2020 6d61 6b65 5f72 6563 203d 206c      make_rec = l
+00007760: 616d 6264 6120 612c 622c 633a 2073 656c  ambda a,b,c: sel
+00007770: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+00007780: 6374 2861 2b74 6573 745f 7369 7a65 2c20  ct(a+test_size, 
+00007790: 622c 2063 290a 2020 2020 2020 2020 7432  b, c).        t2
+000077a0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+000077b0: 6c65 286d 616b 655f 7265 632c 2074 6573  le(make_rec, tes
+000077c0: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+000077d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000077e0: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
+000077f0: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
+00007800: 322c 206c 656e 2874 312b 7432 2929 0a20  2, len(t1+t2)). 
+00007810: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00007820: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+00007830: 6520 2a20 7465 7374 5f73 697a 6520 2a20  e * test_size * 
+00007840: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
+00007850: 3129 290a 0a20 2020 2020 2020 2074 3120  1))..        t1 
+00007860: 2b3d 2074 320a 2020 2020 2020 2020 7365  += t2.        se
+00007870: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00007880: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
+00007890: 7369 7a65 202a 2074 6573 745f 7369 7a65  size * test_size
+000078a0: 202a 2032 2c20 6c65 6e28 7431 2929 0a0a   * 2, len(t1))..
+000078b0: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
+000078c0: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
+000078d0: 745f 7369 7a65 0a20 2020 2020 2020 2074  t_size.        t
+000078e0: 3320 3d20 7431 202b 2028 7365 6c66 2e6d  3 = t1 + (self.m
+000078f0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00007900: 7265 632e 612b 6f66 6673 6574 2c20 7265  rec.a+offset, re
+00007910: 632e 622c 2072 6563 2e63 2920 666f 7220  c.b, rec.c) for 
+00007920: 7265 6320 696e 2074 3229 0a20 2020 2020  rec in t2).     
+00007930: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007940: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
+00007950: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+00007960: 5f73 697a 6520 2a20 332c 206c 656e 2874  _size * 3, len(t
+00007970: 3329 290a 0a20 2020 2064 6566 2074 6573  3))..    def tes
+00007980: 745f 7461 626c 655f 696e 666f 2873 656c  t_table_info(sel
+00007990: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+000079a0: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
+000079b0: 2020 2077 6974 6820 7469 6d65 7374 616d     with timestam
+000079c0: 705f 7374 6172 745f 656e 6428 2920 6173  p_start_end() as
+000079d0: 2074 696d 696e 673a 0a20 2020 2020 2020   timing:.       
+000079e0: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
+000079f0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00007a00: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00007a10: 2074 6573 745f 7369 7a65 2928 2769 6e66   test_size)('inf
+00007a20: 6f5f 7465 7374 2729 0a0a 2020 2020 2020  o_test')..      
+00007a30: 2020 7431 2e63 7265 6174 655f 696e 6465    t1.create_inde
+00007a40: 7828 2762 2729 0a20 2020 2020 2020 2074  x('b').        t
+00007a50: 315f 696e 666f 203d 2074 312e 696e 666f  1_info = t1.info
+00007a60: 2829 0a20 2020 2020 2020 2023 206d 7573  ().        # mus
+00007a70: 7420 736f 7274 2066 6965 6c64 7320 616e  t sort fields an
+00007a80: 6420 696e 6465 7865 7320 7661 6c75 6573  d indexes values
+00007a90: 2c20 666f 7220 7465 7374 2063 6f6d 7061  , for test compa
+00007aa0: 7269 736f 6e73 0a20 2020 2020 2020 2074  risons.        t
+00007ab0: 315f 696e 666f 5b27 6669 656c 6473 275d  1_info['fields']
+00007ac0: 2e73 6f72 7428 290a 2020 2020 2020 2020  .sort().        
+00007ad0: 7431 5f69 6e66 6f5b 2769 6e64 6578 6573  t1_info['indexes
+00007ae0: 275d 2e73 6f72 7428 290a 2020 2020 2020  '].sort().      
+00007af0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007b00: 616c 284e 6f6e 652c 2074 315f 696e 666f  al(None, t1_info
+00007b10: 2e70 6f70 2822 6c61 7374 5f69 6d70 6f72  .pop("last_impor
+00007b20: 7422 2929 0a20 2020 2020 2020 2073 656c  t")).        sel
+00007b30: 662e 6173 7365 7274 5472 7565 2874 696d  f.assertTrue(tim
+00007b40: 696e 672e 7374 6172 7420 3c3d 2074 315f  ing.start <= t1_
+00007b50: 696e 666f 2e70 6f70 2822 6372 6561 7465  info.pop("create
+00007b60: 6422 2920 3c3d 2074 696d 696e 672e 656e  d") <= timing.en
+00007b70: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00007b80: 6173 7365 7274 5472 7565 2874 696d 696e  assertTrue(timin
+00007b90: 672e 7374 6172 7420 3c3d 2074 315f 696e  g.start <= t1_in
+00007ba0: 666f 2e70 6f70 2822 6d6f 6469 6669 6564  fo.pop("modified
+00007bb0: 2229 203c 3d20 7469 6d69 6e67 2e65 6e64  ") <= timing.end
+00007bc0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00007bd0: 7373 6572 7445 7175 616c 287b 2766 6965  ssertEqual({'fie
+00007be0: 6c64 7327 3a20 5b27 6127 2c20 2762 272c  lds': ['a', 'b',
+00007bf0: 2027 6327 5d2c 0a20 2020 2020 2020 2020   'c'],.         
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2027 696e 6465 7865 7327 3a20 5b28 2762   'indexes': [('b
+00007c20: 272c 2046 616c 7365 295d 2c0a 2020 2020  ', False)],.    
+00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 2020 2020 2020 276c 656e 273a 2031 3030        'len': 100
+00007c50: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00007c60: 2020 2020 2020 2020 2020 2020 2027 6e61               'na
+00007c70: 6d65 273a 2027 696e 666f 5f74 6573 7427  me': 'info_test'
+00007c80: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00007c90: 2020 2020 2020 2020 2020 2020 7431 5f69              t1_i
+00007ca0: 6e66 6f2c 2022 696e 7661 6c69 6420 696e  nfo, "invalid in
+00007cb0: 666f 2072 6573 756c 7473 2229 0a0a 0a40  fo results")...@
+00007cc0: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
+00007cd0: 730a 636c 6173 7320 5461 626c 654c 6973  s.class TableLis
+00007ce0: 7454 6573 7473 3a0a 2020 2020 6465 6620  tTests:.    def 
+00007cf0: 5f74 6573 745f 696e 6974 2873 656c 6629  _test_init(self)
+00007d00: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+00007d10: 6573 745f 7369 7a65 203d 2033 0a20 2020  est_size = 3.   
+00007d20: 2020 2020 2073 656c 662e 7431 203d 206d       self.t1 = m
+00007d30: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
+00007d40: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+00007d50: 6a65 6374 2c20 7365 6c66 2e74 6573 745f  ject, self.test_
+00007d60: 7369 7a65 290a 2020 2020 2020 2020 7365  size).        se
+00007d70: 6c66 2e74 6573 745f 7265 6320 3d20 7365  lf.test_rec = se
+00007d80: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00007d90: 6563 7428 312c 2031 2c20 3129 0a0a 2020  ect(1, 1, 1)..  
+00007da0: 2020 6465 6620 7465 7374 5f63 6f6e 7461    def test_conta
+00007db0: 696e 7328 7365 6c66 293a 0a20 2020 2020  ins(self):.     
+00007dc0: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
+00007dd0: 6974 2829 0a20 2020 2020 2020 2073 656c  it().        sel
+00007de0: 662e 6173 7365 7274 5472 7565 2873 656c  f.assertTrue(sel
+00007df0: 662e 7465 7374 5f72 6563 2069 6e20 7365  f.test_rec in se
+00007e00: 6c66 2e74 312c 2022 6661 696c 6564 2027  lf.t1, "failed '
+00007e10: 696e 2720 2863 6f6e 7461 696e 7329 2074  in' (contains) t
+00007e20: 6573 7422 290a 0a20 2020 2064 6566 2074  est")..    def t
+00007e30: 6573 745f 696e 6465 785f 6669 6e64 2873  est_index_find(s
+00007e40: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00007e50: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
+00007e60: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00007e70: 6572 7445 7175 616c 2831 332c 2073 656c  ertEqual(13, sel
+00007e80: 662e 7431 2e69 6e64 6578 2873 656c 662e  f.t1.index(self.
+00007e90: 7465 7374 5f72 6563 292c 2022 6661 696c  test_rec), "fail
+00007ea0: 6564 2027 696e 6465 783b 2074 6573 7420  ed 'index; test 
+00007eb0: 2865 7869 7374 7329 2229 0a20 2020 2020  (exists)").     
+00007ec0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00007ed0: 2873 656c 662e 7465 7374 5f72 6563 2c20  (self.test_rec, 
+00007ee0: 5369 6d70 6c65 4e61 6d65 7370 6163 6529  SimpleNamespace)
+00007ef0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007f00: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
+00007f10: 332c 2073 656c 662e 7431 2e69 6e64 6578  3, self.t1.index
+00007f20: 2876 6172 7328 7365 6c66 2e74 6573 745f  (vars(self.test_
+00007f30: 7265 6329 292c 2022 6661 696c 6564 2027  rec)), "failed '
+00007f40: 696e 6465 783b 2074 6573 7420 2865 7869  index; test (exi
+00007f50: 7374 7329 2229 0a0a 2020 2020 2020 2020  sts)")..        
+00007f60: 6e6f 5f73 7563 685f 7265 6320 3d20 7365  no_such_rec = se
+00007f70: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00007f80: 6563 7428 7365 6c66 2e74 6573 745f 7369  ect(self.test_si
+00007f90: 7a65 2b31 2c20 7365 6c66 2e74 6573 745f  ze+1, self.test_
+00007fa0: 7369 7a65 2b31 2c20 7365 6c66 2e74 6573  size+1, self.tes
+00007fb0: 745f 7369 7a65 2b31 290a 2020 2020 2020  t_size+1).      
+00007fc0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00007fd0: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
+00007fe0: 726f 722c 206d 7367 3d22 6661 696c 6564  ror, msg="failed
+00007ff0: 2027 696e 6465 7827 2074 6573 7420 286e   'index' test (n
+00008000: 6f74 2065 7869 7374 7329 2229 3a0a 2020  ot exists)"):.  
+00008010: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00008020: 312e 696e 6465 7828 6e6f 5f73 7563 685f  1.index(no_such_
+00008030: 7265 6329 0a0a 2020 2020 6465 6620 7465  rec)..    def te
+00008040: 7374 5f72 656d 6f76 6528 7365 6c66 293a  st_remove(self):
+00008050: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+00008060: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
+00008070: 2020 2072 6563 203d 2073 656c 662e 6d61     rec = self.ma
+00008080: 6b65 5f64 6174 615f 6f62 6a65 6374 2831  ke_data_object(1
+00008090: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
+000080a0: 7072 6576 5f6c 656e 203d 206c 656e 2873  prev_len = len(s
+000080b0: 656c 662e 7431 290a 2020 2020 2020 2020  elf.t1).        
+000080c0: 7365 6c66 2e74 312e 7265 6d6f 7665 2872  self.t1.remove(r
+000080d0: 6563 290a 2020 2020 2020 2020 7365 6c66  ec).        self
+000080e0: 2e61 7373 6572 7446 616c 7365 2872 6563  .assertFalse(rec
+000080f0: 2069 6e20 7365 6c66 2e74 312c 2022 6661   in self.t1, "fa
+00008100: 696c 6564 2074 6f20 7265 6d6f 7665 2072  iled to remove r
+00008110: 6563 6f72 6420 6672 6f6d 2074 6162 6c65  ecord from table
+00008120: 2028 636f 6e74 6169 6e73 2922 290a 2020   (contains)").  
+00008130: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008140: 7445 7175 616c 2870 7265 765f 6c65 6e2d  tEqual(prev_len-
+00008150: 312c 206c 656e 2873 656c 662e 7431 292c  1, len(self.t1),
+00008160: 2022 6661 696c 6564 2074 6f20 7265 6d6f   "failed to remo
+00008170: 7665 2072 6563 6f72 6420 6672 6f6d 2074  ve record from t
+00008180: 6162 6c65 2028 6c65 6e29 2229 0a0a 2020  able (len)")..  
+00008190: 2020 2020 2020 6e6f 5f73 7563 685f 7265        no_such_re
+000081a0: 6320 3d20 7365 6c66 2e6d 616b 655f 6461  c = self.make_da
+000081b0: 7461 5f6f 626a 6563 7428 7365 6c66 2e74  ta_object(self.t
+000081c0: 6573 745f 7369 7a65 2b31 2c20 7365 6c66  est_size+1, self
+000081d0: 2e74 6573 745f 7369 7a65 2b31 2c20 7365  .test_size+1, se
+000081e0: 6c66 2e74 6573 745f 7369 7a65 2b31 290a  lf.test_size+1).
+000081f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008200: 6572 7446 616c 7365 286e 6f5f 7375 6368  ertFalse(no_such
+00008210: 5f72 6563 2069 6e20 7365 6c66 2e74 312c  _rec in self.t1,
+00008220: 2022 6661 696c 6564 2074 6f20 6372 6561   "failed to crea
+00008230: 7465 206e 6f6e 2d65 7869 7374 656e 7420  te non-existent 
+00008240: 7265 636f 7264 2066 726f 6d20 7461 626c  record from tabl
+00008250: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00008260: 2e74 312e 7265 6d6f 7665 286e 6f5f 7375  .t1.remove(no_su
+00008270: 6368 5f72 6563 290a 2020 2020 2020 2020  ch_rec).        
+00008280: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008290: 2870 7265 765f 6c65 6e2d 312c 206c 656e  (prev_len-1, len
+000082a0: 2873 656c 662e 7431 292c 2022 6661 696c  (self.t1), "fail
+000082b0: 6564 2072 656d 6f76 696e 6720 6e6f 6e2d  ed removing non-
+000082c0: 6578 6973 7465 6e74 2072 6563 6f72 6420  existent record 
+000082d0: 6672 6f6d 2074 6162 6c65 2028 6c65 6e29  from table (len)
+000082e0: 2229 0a0a 2020 2020 2020 2020 6966 2069  ")..        if i
+000082f0: 7369 6e73 7461 6e63 6528 7365 6c66 2e74  sinstance(self.t
+00008300: 6573 745f 7265 632c 2053 696d 706c 654e  est_rec, SimpleN
+00008310: 616d 6573 7061 6365 293a 0a20 2020 2020  amespace):.     
+00008320: 2020 2020 2020 2073 656c 662e 7431 2e72         self.t1.r
+00008330: 656d 6f76 6528 7661 7273 2873 656c 662e  emove(vars(self.
+00008340: 7465 7374 5f72 6563 2929 0a20 2020 2020  test_rec)).     
+00008350: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00008360: 7274 4571 7561 6c28 7072 6576 5f6c 656e  rtEqual(prev_len
+00008370: 2d31 2c20 6c65 6e28 7365 6c66 2e74 3129  -1, len(self.t1)
+00008380: 2c20 2266 6169 6c65 6420 746f 2072 656d  , "failed to rem
+00008390: 6f76 6520 7265 636f 7264 2061 7320 6469  ove record as di
+000083a0: 6374 2066 726f 6d20 7461 626c 6520 286c  ct from table (l
+000083b0: 656e 2922 290a 0a20 2020 2064 6566 2074  en)")..    def t
+000083c0: 6573 745f 696e 6465 785f 6163 6365 7373  est_index_access
+000083d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000083e0: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
+000083f0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00008400: 7373 6572 7445 7175 616c 2873 656c 662e  ssertEqual(self.
+00008410: 7465 7374 5f72 6563 2c20 7365 6c66 2e74  test_rec, self.t
+00008420: 315b 3133 5d2c 2022 6661 696c 6564 2069  1[13], "failed i
+00008430: 6e64 6578 2061 6363 6573 7320 7465 7374  ndex access test
+00008440: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+00008450: 5f63 6f75 6e74 2873 656c 6629 3a0a 2020  _count(self):.  
+00008460: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+00008470: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+00008480: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00008490: 7365 6c66 2e74 312e 636f 756e 7428 7365  self.t1.count(se
+000084a0: 6c66 2e74 6573 745f 7265 6329 203d 3d20  lf.test_rec) == 
+000084b0: 312c 2022 6661 696c 6564 2063 6f75 6e74  1, "failed count
+000084c0: 2074 6573 7422 290a 2020 2020 2020 2020   test").        
+000084d0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+000084e0: 6c66 2e74 6573 745f 7265 632c 2053 696d  lf.test_rec, Sim
+000084f0: 706c 654e 616d 6573 7061 6365 293a 0a20  pleNamespace):. 
+00008500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008510: 6173 7365 7274 5472 7565 2873 656c 662e  assertTrue(self.
+00008520: 7431 2e63 6f75 6e74 2876 6172 7328 7365  t1.count(vars(se
+00008530: 6c66 2e74 6573 745f 7265 6329 2920 3d3d  lf.test_rec)) ==
+00008540: 2031 2c20 2266 6169 6c65 6420 636f 756e   1, "failed coun
+00008550: 7420 7465 7374 2229 0a0a 2020 2020 6465  t test")..    de
+00008560: 6620 7465 7374 5f64 656c 2873 656c 6629  f test_del(self)
+00008570: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00008580: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
+00008590: 2020 2020 6265 666f 7265 5f64 656c 5f6c      before_del_l
+000085a0: 656e 203d 206c 656e 2873 656c 662e 7431  en = len(self.t1
+000085b0: 290a 2020 2020 2020 2020 6465 6c20 7365  ).        del se
+000085c0: 6c66 2e74 315b 3133 5d0a 2020 2020 2020  lf.t1[13].      
+000085d0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+000085e0: 7365 2873 656c 662e 7465 7374 5f72 6563  se(self.test_rec
+000085f0: 2069 6e20 7365 6c66 2e74 312c 2022 6661   in self.t1, "fa
+00008600: 696c 6564 2064 656c 2074 6573 7422 290a  iled del test").
+00008610: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008620: 6572 7445 7175 616c 2862 6566 6f72 655f  ertEqual(before_
+00008630: 6465 6c5f 6c65 6e20 2d20 312c 206c 656e  del_len - 1, len
+00008640: 2873 656c 662e 7431 2929 0a0a 2020 2020  (self.t1))..    
+00008650: 6465 6620 7465 7374 5f70 6f70 2873 656c  def test_pop(sel
+00008660: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00008670: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
+00008680: 2020 2020 2020 6265 666f 7265 5f70 6f70        before_pop
+00008690: 5f6c 656e 203d 206c 656e 2873 656c 662e  _len = len(self.
+000086a0: 7431 290a 2020 2020 2020 2020 6f62 6a20  t1).        obj 
+000086b0: 3d20 7365 6c66 2e74 312e 706f 7028 3133  = self.t1.pop(13
+000086c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000086d0: 7373 6572 7446 616c 7365 286f 626a 2069  ssertFalse(obj i
+000086e0: 6e20 7365 6c66 2e74 3129 0a20 2020 2020  n self.t1).     
+000086f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00008700: 7561 6c28 7365 6c66 2e74 6573 745f 7265  ual(self.test_re
+00008710: 632c 206f 626a 290a 2020 2020 2020 2020  c, obj).        
+00008720: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008730: 2862 6566 6f72 655f 706f 705f 6c65 6e20  (before_pop_len 
+00008740: 2d20 312c 206c 656e 2873 656c 662e 7431  - 1, len(self.t1
+00008750: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00008760: 5f70 6f70 5f6c 6173 7428 7365 6c66 293a  _pop_last(self):
+00008770: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+00008780: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
+00008790: 2020 2062 6566 6f72 655f 706f 705f 6c65     before_pop_le
+000087a0: 6e20 3d20 6c65 6e28 7365 6c66 2e74 3129  n = len(self.t1)
+000087b0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+000087c0: 645f 706f 7020 3d20 636f 7079 2e63 6f70  d_pop = copy.cop
+000087d0: 7928 7365 6c66 2e74 315b 2d31 5d29 0a20  y(self.t1[-1]). 
+000087e0: 2020 2020 2020 206f 626a 203d 2073 656c         obj = sel
+000087f0: 662e 7431 2e70 6f70 2829 0a20 2020 2020  f.t1.pop().     
+00008800: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00008810: 7561 6c28 6578 7065 6374 6564 5f70 6f70  ual(expected_pop
+00008820: 2c20 6f62 6a29 0a20 2020 2020 2020 2073  , obj).        s
+00008830: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00008840: 6265 666f 7265 5f70 6f70 5f6c 656e 202d  before_pop_len -
+00008850: 2031 2c20 6c65 6e28 7365 6c66 2e74 3129   1, len(self.t1)
+00008860: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00008870: 7265 7665 7273 6564 2873 656c 6629 3a0a  reversed(self):.
+00008880: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00008890: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+000088a0: 2020 6c61 7374 5f72 6563 203d 206e 6578    last_rec = nex
+000088b0: 7428 7265 7665 7273 6564 2873 656c 662e  t(reversed(self.
+000088c0: 7431 2929 0a20 2020 2020 2020 2073 656c  t1)).        sel
+000088d0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+000088e0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000088f0: 6563 7428 322c 2032 2c20 3229 2c20 6c61  ect(2, 2, 2), la
+00008900: 7374 5f72 6563 2c20 2266 6169 6c65 6420  st_rec, "failed 
+00008910: 7265 7665 7273 6564 2074 6573 7422 290a  reversed test").
+00008920: 0a20 2020 2064 6566 2074 6573 745f 6974  .    def test_it
+00008930: 6572 2873 656c 6629 3a0a 2020 2020 2020  er(self):.      
+00008940: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+00008950: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00008960: 2e61 7373 6572 7454 7275 6528 7365 6c66  .assertTrue(self
+00008970: 2e74 6573 745f 7265 6320 696e 2073 656c  .test_rec in sel
+00008980: 662e 7431 2c20 2266 6169 6c65 6420 2769  f.t1, "failed 'i
+00008990: 6e27 2028 636f 6e74 6169 6e73 2920 7465  n' (contains) te
+000089a0: 7374 2229 0a0a 2020 2020 6465 6620 7465  st")..    def te
+000089b0: 7374 5f68 6561 645f 616e 645f 7461 696c  st_head_and_tail
+000089c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000089d0: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
+000089e0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+000089f0: 312e 6372 6561 7465 5f69 6e64 6578 2822  1.create_index("
+00008a00: 6122 290a 2020 2020 2020 2020 7365 6c66  a").        self
+00008a10: 2e74 312e 6372 6561 7465 5f69 6e64 6578  .t1.create_index
+00008a20: 2822 6322 290a 2020 2020 2020 2020 7365  ("c").        se
+00008a30: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
+00008a40: 2261 222c 2022 6322 7d2c 2073 6574 2873  "a", "c"}, set(s
+00008a50: 656c 662e 7431 2e5f 696e 6465 7865 732e  elf.t1._indexes.
+00008a60: 6b65 7973 2829 292c 2022 6661 696c 6564  keys()), "failed
+00008a70: 2074 6f20 6372 6561 7465 2069 6e64 6578   to create index
+00008a80: 6573 2229 0a0a 2020 2020 2020 2020 7365  es")..        se
+00008a90: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+00008aa0: 6574 2873 656c 662e 7431 2e5f 696e 6465  et(self.t1._inde
+00008ab0: 7865 732e 6b65 7973 2829 292c 0a20 2020  xes.keys()),.   
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2020 2020 2020 7365 7428 7365 6c66 2e74        set(self.t
+00008ae0: 312e 6865 6164 2829 2e5f 696e 6465 7865  1.head()._indexe
+00008af0: 732e 6b65 7973 2829 292c 0a20 2020 2020  s.keys()),.     
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 2020 2020 2266 6169 6c65 6420 746f 2063      "failed to c
+00008b20: 6f70 7920 696e 6465 7865 7320 746f 2068  opy indexes to h
+00008b30: 6561 6428 2922 290a 2020 2020 2020 2020  ead()").        
+00008b40: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008b50: 2873 6574 2873 656c 662e 7431 2e5f 696e  (set(self.t1._in
+00008b60: 6465 7865 732e 6b65 7973 2829 292c 0a20  dexes.keys()),. 
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 7365 7428 7365 6c66          set(self
+00008b90: 2e74 312e 7461 696c 2829 2e5f 696e 6465  .t1.tail()._inde
+00008ba0: 7865 732e 6b65 7973 2829 292c 0a20 2020  xes.keys()),.   
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 2020 2266 6169 6c65 6420 746f        "failed to
+00008bd0: 2063 6f70 7920 696e 6465 7865 7320 746f   copy indexes to
+00008be0: 2074 6169 6c28 2922 290a 0a20 2020 2064   tail()")..    d
+00008bf0: 6566 2074 6573 745f 756e 6971 7565 2873  ef test_unique(s
+00008c00: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00008c10: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
+00008c20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008c30: 6572 7445 7175 616c 285b 302c 2031 2c20  ertEqual([0, 1, 
+00008c40: 325d 2c20 736f 7274 6564 285b 726f 772e  2], sorted([row.
+00008c50: 6120 666f 7220 726f 7720 696e 2073 656c  a for row in sel
+00008c60: 662e 7431 2e75 6e69 7175 6528 2761 2729  f.t1.unique('a')
+00008c70: 5d29 2c20 2266 6169 6c65 6420 6361 6c6c  ]), "failed call
+00008c80: 2074 6f20 756e 6971 7565 2229 0a0a 2020   to unique")..  
+00008c90: 2020 6465 6620 7465 7374 5f61 6c6c 5f61    def test_all_a
+00008ca0: 6363 6573 736f 7228 7365 6c66 293a 0a20  ccessor(self):. 
+00008cb0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
+00008cc0: 745f 696e 6974 2829 0a20 2020 2020 2020  t_init().       
+00008cd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00008ce0: 6c28 7375 6d28 285b 695d 2a73 656c 662e  l(sum(([i]*self.
+00008cf0: 7465 7374 5f73 697a 652a 2a32 2066 6f72  test_size**2 for
+00008d00: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00008d10: 2e74 6573 745f 7369 7a65 2929 2c20 5b5d  .test_size)), []
+00008d20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008d30: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00008d40: 2873 656c 662e 7431 2e61 6c6c 2e61 292c  (self.t1.all.a),
+00008d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d60: 2020 2020 2020 2020 2020 2266 6169 6c65            "faile
+00008d70: 6420 746f 2073 7563 6365 7373 6675 6c6c  d to successfull
+00008d80: 7920 6765 7420 616c 6c20 7661 6c75 6573  y get all values
+00008d90: 2069 6e20 2761 2722 290a 0a20 2020 2020   in 'a'")..     
+00008da0: 2020 2061 6c6c 5f61 7320 3d20 7365 6c66     all_as = self
+00008db0: 2e74 312e 616c 6c2e 610a 2020 2020 2020  .t1.all.a.      
+00008dc0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00008dd0: 6528 616c 6c5f 6173 2069 7320 6974 6572  e(all_as is iter
+00008de0: 2861 6c6c 5f61 7329 2c20 2261 6c6c 2069  (all_as), "all i
+00008df0: 7465 7261 746f 7220 6661 696c 7320 746f  terator fails to
+00008e00: 2069 6465 6e74 6966 7920 6173 2069 7465   identify as ite
+00008e10: 7228 7365 6c66 2922 290a 0a20 2020 2064  r(self)")..    d
+00008e20: 6566 2074 6573 745f 666f 726d 6174 2873  ef test_format(s
+00008e30: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00008e40: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
+00008e50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008e60: 6572 7445 7175 616c 285b 2730 3020 3020  ertEqual(['00 0 
+00008e70: 3027 2c20 2730 3020 3020 3127 2c20 2730  0', '00 0 1', '0
+00008e80: 3020 3020 3227 5d2c 0a20 2020 2020 2020  0 0 2'],.       
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ea0: 2020 6c69 7374 2873 656c 662e 7431 2e66    list(self.t1.f
+00008eb0: 6f72 6d61 7428 227b 613a 3032 647d 207b  ormat("{a:02d} {
+00008ec0: 627d 207b 637d 2229 295b 3a33 5d2c 0a20  b} {c}"))[:3],. 
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 2020 2020 2020 2020 2266 6169 6c65 6420          "failed 
+00008ef0: 746f 2063 7265 6174 6520 666f 726d 6174  to create format
+00008f00: 7465 6420 726f 7773 2229 0a0a 2020 2020  ted rows")..    
+00008f10: 6465 6620 7465 7374 5f61 735f 6874 6d6c  def test_as_html
+00008f20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008f30: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
+00008f40: 290a 2020 2020 2020 2020 6874 6d6c 5f6f  ).        html_o
+00008f50: 7574 7075 7420 3d20 7365 6c66 2e74 315b  utput = self.t1[
+00008f60: 3a31 305d 2e61 735f 6874 6d6c 2866 6965  :10].as_html(fie
+00008f70: 6c64 733d 2261 2062 2063 2229 0a20 2020  lds="a b c").   
+00008f80: 2020 2020 2070 7269 6e74 2868 746d 6c5f       print(html_
+00008f90: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+00008fa0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00008fb0: 223c 7468 6561 643e 2220 696e 2068 746d  "<thead>" in htm
+00008fc0: 6c5f 6f75 7470 7574 2061 6e64 2022 3c74  l_output and "<t
+00008fd0: 626f 6479 3e22 2069 6e20 6874 6d6c 5f6f  body>" in html_o
+00008fe0: 7574 7075 742c 0a20 2020 2020 2020 2020  utput,.         
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009000: 6173 5f68 746d 6c20 646f 6573 206e 6f74  as_html does not
+00009010: 2069 6e63 6c75 6465 2074 6865 6164 2061   include thead a
+00009020: 6e64 2074 626f 6479 2074 6167 7322 290a  nd tbody tags").
+00009030: 0a20 2020 2020 2020 2068 746d 6c5f 6c69  .        html_li
+00009040: 6e65 7320 3d20 6874 6d6c 5f6f 7574 7075  nes = html_outpu
+00009050: 742e 7370 6c69 746c 696e 6573 2829 0a20  t.splitlines(). 
+00009060: 2020 2020 2020 2068 6472 5f6c 696e 6520         hdr_line 
+00009070: 3d20 6e65 7874 2868 2066 6f72 2068 2069  = next(h for h i
+00009080: 6e20 6874 6d6c 5f6c 696e 6573 2069 6620  n html_lines if 
+00009090: 2263 656e 7465 7222 2069 6e20 6829 0a20  "center" in h). 
+000090a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000090b0: 7274 4571 7561 6c28 273c 7472 3e3c 7468  rtEqual('<tr><th
+000090c0: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
+000090d0: 7465 7222 3e61 3c2f 6469 763e 3c2f 7468  ter">a</div></th
+000090e0: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
+000090f0: 2020 2020 2020 2020 2020 2020 273c 7468              '<th
+00009100: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
+00009110: 7465 7222 3e62 3c2f 6469 763e 3c2f 7468  ter">b</div></th
+00009120: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
+00009130: 2020 2020 2020 2020 2020 2020 273c 7468              '<th
+00009140: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
+00009150: 7465 7222 3e63 3c2f 6469 763e 3c2f 7468  ter">c</div></th
+00009160: 3e3c 2f74 723e 272c 0a20 2020 2020 2020  ></tr>',.       
+00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009180: 2020 6864 725f 6c69 6e65 2c0a 2020 2020    hdr_line,.    
+00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2020 2020 2022 6661 696c 6564 2061 735f       "failed as_
+000091b0: 6874 6d6c 2077 6974 6820 616c 6c20 6669  html with all fi
+000091c0: 656c 6473 2229 0a0a 2020 2020 2020 2020  elds")..        
+000091d0: 6874 6d6c 5f6f 7574 7075 7420 3d20 7365  html_output = se
+000091e0: 6c66 2e74 315b 3a31 305d 2e61 735f 6874  lf.t1[:10].as_ht
+000091f0: 6d6c 2866 6965 6c64 733d 2261 202d 6220  ml(fields="a -b 
+00009200: 6322 290a 2020 2020 2020 2020 7072 696e  c").        prin
+00009210: 7428 6874 6d6c 5f6f 7574 7075 7429 0a20  t(html_output). 
+00009220: 2020 2020 2020 2068 746d 6c5f 6c69 6e65         html_line
+00009230: 7320 3d20 6874 6d6c 5f6f 7574 7075 742e  s = html_output.
+00009240: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
+00009250: 2020 2020 2068 6472 5f6c 696e 6520 3d20       hdr_line = 
+00009260: 6e65 7874 2868 2066 6f72 2068 2069 6e20  next(h for h in 
+00009270: 6874 6d6c 5f6c 696e 6573 2069 6620 2263  html_lines if "c
+00009280: 656e 7465 7222 2069 6e20 6829 0a20 2020  enter" in h).   
+00009290: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000092a0: 4571 7561 6c28 273c 7472 3e3c 7468 3e3c  Equal('<tr><th><
+000092b0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+000092c0: 7222 3e61 3c2f 6469 763e 3c2f 7468 3e27  r">a</div></th>'
+000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092e0: 2020 2020 2020 2020 2020 273c 7468 3e3c            '<th><
+000092f0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00009300: 7222 3e63 3c2f 6469 763e 3c2f 7468 3e3c  r">c</div></th><
+00009310: 2f74 723e 272c 0a20 2020 2020 2020 2020  /tr>',.         
+00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009330: 6864 725f 6c69 6e65 2c0a 2020 2020 2020  hdr_line,.      
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 2020 2022 6661 696c 6564 2061 735f 6874     "failed as_ht
+00009360: 6d6c 2077 6974 6820 6e65 6761 7465 6420  ml with negated 
+00009370: 6669 656c 6422 290a 0a20 2020 2020 2020  field")..       
+00009380: 2068 746d 6c5f 6f75 7470 7574 203d 2073   html_output = s
+00009390: 656c 662e 7431 5b3a 3130 5d2e 6173 5f68  elf.t1[:10].as_h
+000093a0: 746d 6c28 6669 656c 6473 3d22 6120 6220  tml(fields="a b 
+000093b0: 6322 2c20 666f 726d 6174 733d 7b22 6222  c", formats={"b"
+000093c0: 3a20 227b 3a30 3364 7d22 7d29 0a20 2020  : "{:03d}"}).   
+000093d0: 2020 2020 2070 7269 6e74 2868 746d 6c5f       print(html_
+000093e0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+000093f0: 6874 6d6c 5f6c 696e 6573 203d 2068 746d  html_lines = htm
+00009400: 6c5f 6f75 7470 7574 2e73 706c 6974 6c69  l_output.splitli
+00009410: 6e65 7328 290a 2020 2020 2020 2020 6461  nes().        da
+00009420: 7461 5f6c 696e 6520 3d20 6e65 7874 2868  ta_line = next(h
+00009430: 2066 6f72 2068 2069 6e20 6874 6d6c 5f6c   for h in html_l
+00009440: 696e 6573 2069 6620 223c 7464 3e22 2069  ines if "<td>" i
+00009450: 6e20 6829 0a20 2020 2020 2020 2073 656c  n h).        sel
+00009460: 662e 6173 7365 7274 4571 7561 6c28 273c  f.assertEqual('<
+00009470: 7462 6f64 793e 3c74 723e 3c74 643e 3c64  tbody><tr><td><d
+00009480: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
+00009490: 3e30 3c2f 6469 763e 3c2f 7464 3e27 0a20  >0</div></td>'. 
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094b0: 2020 2020 2020 2020 273c 7464 3e3c 6469          '<td><di
+000094c0: 7620 616c 6967 6e3d 2272 6967 6874 223e  v align="right">
+000094d0: 3030 303c 2f64 6976 3e3c 2f74 643e 270a  000</div></td>'.
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 2027 3c74 643e 3c64           '<td><d
+00009500: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
+00009510: 3e30 3c2f 6469 763e 3c2f 7464 3e3c 2f74  >0</div></td></t
+00009520: 723e 272c 0a20 2020 2020 2020 2020 2020  r>',.           
+00009530: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00009540: 7461 5f6c 696e 652c 0a20 2020 2020 2020  ta_line,.       
+00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009560: 2020 2266 6169 6c65 6420 6173 5f68 746d    "failed as_htm
+00009570: 6c20 7769 7468 206e 616d 6564 2066 6965  l with named fie
+00009580: 6c64 2066 6f72 6d61 7420 666f 7220 7370  ld format for sp
+00009590: 6563 6966 6963 2066 6965 6c64 2229 0a0a  ecific field")..
+000095a0: 2020 2020 2020 2020 6874 6d6c 5f6f 7574          html_out
+000095b0: 7075 7420 3d20 7365 6c66 2e74 315b 3a31  put = self.t1[:1
+000095c0: 305d 2e61 735f 6874 6d6c 2866 6965 6c64  0].as_html(field
+000095d0: 733d 2261 2062 2063 222c 2066 6f72 6d61  s="a b c", forma
+000095e0: 7473 3d7b 696e 743a 2022 7b3a 3033 647d  ts={int: "{:03d}
+000095f0: 227d 290a 2020 2020 2020 2020 7072 696e  "}).        prin
+00009600: 7428 6874 6d6c 5f6f 7574 7075 7429 0a20  t(html_output). 
+00009610: 2020 2020 2020 2068 746d 6c5f 6c69 6e65         html_line
+00009620: 7320 3d20 6874 6d6c 5f6f 7574 7075 742e  s = html_output.
+00009630: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
+00009640: 2020 2020 2064 6174 615f 6c69 6e65 203d       data_line =
+00009650: 206e 6578 7428 6820 666f 7220 6820 696e   next(h for h in
+00009660: 2068 746d 6c5f 6c69 6e65 7320 6966 2022   html_lines if "
+00009670: 3c74 643e 2220 696e 2068 290a 2020 2020  <td>" in h).    
+00009680: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009690: 7175 616c 2827 3c74 626f 6479 3e3c 7472  qual('<tbody><tr
+000096a0: 3e3c 7464 3e3c 6469 7620 616c 6967 6e3d  ><td><div align=
+000096b0: 2272 6967 6874 223e 3030 303c 2f64 6976  "right">000</div
+000096c0: 3e3c 2f74 643e 270a 2020 2020 2020 2020  ></td>'.        
+000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096e0: 2027 3c74 643e 3c64 6976 2061 6c69 676e   '<td><div align
+000096f0: 3d22 7269 6768 7422 3e30 3030 3c2f 6469  ="right">000</di
+00009700: 763e 3c2f 7464 3e27 0a20 2020 2020 2020  v></td>'.       
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2020 273c 7464 3e3c 6469 7620 616c 6967    '<td><div alig
+00009730: 6e3d 2272 6967 6874 223e 3030 303c 2f64  n="right">000</d
+00009740: 6976 3e3c 2f74 643e 3c2f 7472 3e27 2c0a  iv></td></tr>',.
+00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009760: 2020 2020 2020 2020 2064 6174 615f 6c69           data_li
+00009770: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00009780: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
+00009790: 696c 6564 2061 735f 6874 6d6c 2077 6974  iled as_html wit
+000097a0: 6820 6461 7461 2074 7970 6520 666f 726d  h data type form
+000097b0: 6174 2066 6f72 2061 6c6c 2066 6965 6c64  at for all field
+000097c0: 7322 290a 0a20 2020 2020 2020 2068 746d  s")..        htm
+000097d0: 6c5f 6f75 7470 7574 203d 2073 656c 662e  l_output = self.
+000097e0: 7431 5b3a 3130 5d2e 6173 5f68 746d 6c28  t1[:10].as_html(
+000097f0: 6669 656c 6473 3d22 6120 6220 6322 2c20  fields="a b c", 
+00009800: 666f 726d 6174 733d 7b69 6e74 3a20 227b  formats={int: "{
+00009810: 3a30 3364 7d22 7d2c 2067 726f 7570 6279  :03d}"}, groupby
+00009820: 3d22 6122 290a 2020 2020 2020 2020 7072  ="a").        pr
+00009830: 696e 7428 6874 6d6c 5f6f 7574 7075 7429  int(html_output)
+00009840: 0a20 2020 2020 2020 2068 746d 6c5f 6c69  .        html_li
+00009850: 6e65 7320 3d20 6874 6d6c 5f6f 7574 7075  nes = html_outpu
+00009860: 742e 7370 6c69 746c 696e 6573 2829 0a20  t.splitlines(). 
+00009870: 2020 2020 2020 2064 6174 615f 6c69 6e65         data_line
+00009880: 203d 206e 6578 7428 6820 666f 7220 6820   = next(h for h 
+00009890: 696e 2068 746d 6c5f 6c69 6e65 7320 6966  in html_lines if
+000098a0: 2022 3c74 643e 2220 696e 2068 290a 2020   "<td>" in h).  
+000098b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000098c0: 7445 7175 616c 2827 3c74 626f 6479 3e3c  tEqual('<tbody><
+000098d0: 7472 3e3c 7464 3e3c 6469 7620 616c 6967  tr><td><div alig
+000098e0: 6e3d 2272 6967 6874 223e 3030 303c 2f64  n="right">000</d
+000098f0: 6976 3e3c 2f74 643e 270a 2020 2020 2020  iv></td>'.      
+00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009910: 2020 2027 3c74 643e 3c64 6976 2061 6c69     '<td><div ali
+00009920: 676e 3d22 7269 6768 7422 3e30 3030 3c2f  gn="right">000</
+00009930: 6469 763e 3c2f 7464 3e27 0a20 2020 2020  div></td>'.     
+00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009950: 2020 2020 273c 7464 3e3c 6469 7620 616c      '<td><div al
+00009960: 6967 6e3d 2272 6967 6874 223e 3030 303c  ign="right">000<
+00009970: 2f64 6976 3e3c 2f74 643e 3c2f 7472 3e27  /div></td></tr>'
+00009980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009990: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+000099a0: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000099c0: 6661 696c 6564 2061 735f 6874 6d6c 2077  failed as_html w
+000099d0: 6974 6820 6772 6f75 7062 7922 290a 0a20  ith groupby").. 
+000099e0: 2020 2020 2020 2068 746d 6c5f 6f75 7470         html_outp
+000099f0: 7574 203d 2073 656c 662e 7431 5b3a 3130  ut = self.t1[:10
+00009a00: 5d2e 6173 5f68 746d 6c28 6669 656c 6473  ].as_html(fields
+00009a10: 3d22 6120 6220 6322 2c20 7461 626c 655f  ="a b c", table_
+00009a20: 7072 6f70 6572 7469 6573 3d7b 2262 6f72  properties={"bor
+00009a30: 6465 7222 3a20 2232 227d 290a 2020 2020  der": "2"}).    
+00009a40: 2020 2020 7072 696e 7428 6874 6d6c 5f6f      print(html_o
+00009a50: 7574 7075 7429 0a20 2020 2020 2020 2073  utput).        s
+00009a60: 656c 662e 6173 7365 7274 5472 7565 2822  elf.assertTrue("
+00009a70: 3c74 6865 6164 3e22 2069 6e20 6874 6d6c  <thead>" in html
+00009a80: 5f6f 7574 7075 7420 616e 6420 223c 7462  _output and "<tb
+00009a90: 6f64 793e 2220 696e 2068 746d 6c5f 6f75  ody>" in html_ou
+00009aa0: 7470 7574 2c0a 2020 2020 2020 2020 2020  tput,.          
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00009ac0: 735f 6874 6d6c 2064 6f65 7320 6e6f 7420  s_html does not 
+00009ad0: 696e 636c 7564 6520 7468 6561 6420 616e  include thead an
+00009ae0: 6420 7462 6f64 7920 7461 6773 2229 0a0a  d tbody tags")..
+00009af0: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
+00009b00: 6c65 7465 5f73 6c69 6365 7328 7365 6c66  lete_slices(self
+00009b10: 293a 0a20 2020 2020 2020 2063 6f6d 7061  ):.        compa
+00009b20: 7265 5f6c 6973 7420 3d20 6c69 7374 2822  re_list = list("
+00009b30: 4142 4344 4546 4748 494a 4b4c 4d4e 4f50  ABCDEFGHIJKLMNOP
+00009b40: 5152 5354 5556 5758 595a 3031 3233 3435  QRSTUVWXYZ012345
+00009b50: 3637 3839 6162 6364 6566 6768 696a 6b6c  6789abcdefghijkl
+00009b60: 6d6e 6f70 7172 7374 7576 7778 797a 2229  mnopqrstuvwxyz")
+00009b70: 0a20 2020 2020 2020 2074 3120 3d20 6c74  .        t1 = lt
+00009b80: 2e54 6162 6c65 2829 2e69 6e73 6572 745f  .Table().insert_
+00009b90: 6d61 6e79 286c 742e 4461 7461 4f62 6a65  many(lt.DataObje
+00009ba0: 6374 2841 3d63 2920 666f 7220 6320 696e  ct(A=c) for c in
+00009bb0: 2063 6f6d 7061 7265 5f6c 6973 7429 0a0a   compare_list)..
+00009bc0: 2020 2020 2020 2020 6465 6620 6d69 6e69          def mini
+00009bd0: 5f74 6573 7428 736c 635f 7475 706c 6529  _test(slc_tuple)
+00009be0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00009bf0: 2069 7369 6e73 7461 6e63 6528 736c 635f   isinstance(slc_
+00009c00: 7475 706c 652c 2074 7570 6c65 293a 0a20  tuple, tuple):. 
+00009c10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00009c20: 6162 656c 203d 2022 5b7b 7d3a 7b7d 3a7b  abel = "[{}:{}:{
+00009c30: 7d5d 222e 666f 726d 6174 282a 2869 2069  }]".format(*(i i
+00009c40: 6620 6920 6973 206e 6f74 204e 6f6e 6520  f i is not None 
+00009c50: 656c 7365 2027 2720 666f 7220 6920 696e  else '' for i in
+00009c60: 2073 6c63 5f74 7570 6c65 2929 0a20 2020   slc_tuple)).   
+00009c70: 2020 2020 2020 2020 2020 2020 2073 6c63               slc
+00009c80: 203d 2073 6c69 6365 282a 736c 635f 7475   = slice(*slc_tu
+00009c90: 706c 6529 0a20 2020 2020 2020 2020 2020  ple).           
+00009ca0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009cb0: 2020 2020 2020 206c 6162 656c 203d 2073         label = s
+00009cc0: 7472 2873 6c63 5f74 7570 6c65 290a 2020  tr(slc_tuple).  
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00009ce0: 6320 3d20 736c 635f 7475 706c 650a 0a20  c = slc_tuple.. 
+00009cf0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00009d00: 7365 6c66 2e73 7562 5465 7374 286c 6162  self.subTest(lab
+00009d10: 656c 2c20 736c 635f 7475 706c 653d 736c  el, slc_tuple=sl
+00009d20: 635f 7475 706c 6529 3a0a 2020 2020 2020  c_tuple):.      
+00009d30: 2020 2020 2020 2020 2020 6465 6c20 636f            del co
+00009d40: 6d70 6172 655f 6c69 7374 5b73 6c63 5d0a  mpare_list[slc].
+00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d60: 7072 696e 7428 6c61 6265 6c29 0a20 2020  print(label).   
+00009d70: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00009d80: 6e74 2827 4578 7065 6374 6564 272c 2063  nt('Expected', c
+00009d90: 6f6d 7061 7265 5f6c 6973 7429 0a20 2020  ompare_list).   
+00009da0: 2020 2020 2020 2020 2020 2020 2064 656c               del
+00009db0: 2074 315b 736c 635d 0a20 2020 2020 2020   t1[slc].       
+00009dc0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00009dd0: 4f62 7365 7276 6564 272c 206c 6973 7428  Observed', list(
+00009de0: 7431 2e61 6c6c 2e41 2929 0a20 2020 2020  t1.all.A)).     
+00009df0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00009e00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00009e10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00009e20: 7561 6c28 2727 2e6a 6f69 6e28 636f 6d70  ual(''.join(comp
+00009e30: 6172 655f 6c69 7374 292c 2027 272e 6a6f  are_list), ''.jo
+00009e40: 696e 2874 312e 616c 6c2e 4129 2c20 2266  in(t1.all.A), "f
+00009e50: 6169 6c65 6420 2220 2b20 6c61 6265 6c29  ailed " + label)
+00009e60: 0a0a 2020 2020 2020 2020 6d69 6e69 5f74  ..        mini_t
+00009e70: 6573 7428 3529 0a20 2020 2020 2020 206d  est(5).        m
+00009e80: 696e 695f 7465 7374 282d 3529 0a20 2020  ini_test(-5).   
+00009e90: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
+00009ea0: 2d35 2c20 4e6f 6e65 2c20 4e6f 6e65 2929  -5, None, None))
+00009eb0: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
+00009ec0: 7374 2828 4e6f 6e65 2c20 332c 204e 6f6e  st((None, 3, Non
+00009ed0: 6529 290a 2020 2020 2020 2020 6d69 6e69  e)).        mini
+00009ee0: 5f74 6573 7428 284e 6f6e 652c 202d 6c65  _test((None, -le
+00009ef0: 6e28 636f 6d70 6172 655f 6c69 7374 292b  n(compare_list)+
+00009f00: 332c 204e 6f6e 6529 290a 2020 2020 2020  3, None)).      
+00009f10: 2020 6d69 6e69 5f74 6573 7428 284e 6f6e    mini_test((Non
+00009f20: 652c 204e 6f6e 652c 2035 2929 0a20 2020  e, None, 5)).   
+00009f30: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
+00009f40: 4e6f 6e65 2c20 4e6f 6e65 2c20 2d35 2929  None, None, -5))
+00009f50: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
+00009f60: 7374 2828 2d35 2c20 2d32 2c20 4e6f 6e65  st((-5, -2, None
+00009f70: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
+00009f80: 7465 7374 2828 2d32 2c20 2d35 2c20 2d31  test((-2, -5, -1
+00009f90: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
+00009fa0: 7465 7374 2828 352c 2032 302c 2032 2929  test((5, 20, 2))
+00009fb0: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
+00009fc0: 7374 2828 6c65 6e28 636f 6d70 6172 655f  st((len(compare_
+00009fd0: 6c69 7374 292c 2035 2c20 2d33 2929 0a20  list), 5, -3)). 
+00009fe0: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
+00009ff0: 2828 3230 2c20 3131 2c20 2d37 2929 0a20  ((20, 11, -7)). 
+0000a000: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
+0000a010: 2828 352c 2035 2c20 4e6f 6e65 2929 0a20  ((5, 5, None)). 
+0000a020: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
+0000a030: 2828 4e6f 6e65 2c20 2d31 302c 2035 2929  ((None, -10, 5))
+0000a040: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
+0000a050: 7374 2828 4e6f 6e65 2c20 2d31 302c 202d  st((None, -10, -
+0000a060: 3130 2929 0a20 2020 2020 2020 206d 696e  10)).        min
+0000a070: 695f 7465 7374 2828 3130 3030 2c20 3230  i_test((1000, 20
+0000a080: 3030 2c20 4e6f 6e65 2929 0a20 2020 2020  00, None)).     
+0000a090: 2020 206d 696e 695f 7465 7374 2828 4e6f     mini_test((No
+0000a0a0: 6e65 2c20 4e6f 6e65 2c20 2d31 2929 0a0a  ne, None, -1))..
+0000a0b0: 2020 2020 6465 6620 7465 7374 5f63 6c65      def test_cle
+0000a0c0: 6172 2873 656c 6629 3a0a 2020 2020 2020  ar(self):.      
+0000a0d0: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+0000a0e0: 7428 290a 2020 2020 2020 2020 6e75 6d5f  t().        num_
+0000a0f0: 6669 656c 6473 203d 206c 656e 2873 656c  fields = len(sel
+0000a100: 662e 7431 2e69 6e66 6f28 295b 2266 6965  f.t1.info()["fie
+0000a110: 6c64 7322 5d29 0a20 2020 2020 2020 2077  lds"]).        w
+0000a120: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000a130: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000a140: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000a150: 2873 656c 662e 7465 7374 5f73 697a 6520  (self.test_size 
+0000a160: 2a2a 206e 756d 5f66 6965 6c64 732c 206c  ** num_fields, l
+0000a170: 656e 2873 656c 662e 7431 292c 2022 696e  en(self.t1), "in
+0000a180: 7661 6c69 6420 6c65 6e22 290a 2020 2020  valid len").    
+0000a190: 2020 2020 7365 6c66 2e74 312e 6372 6561      self.t1.crea
+0000a1a0: 7465 5f69 6e64 6578 2822 6122 290a 0a20  te_index("a").. 
+0000a1b0: 2020 2020 2020 2073 656c 662e 7431 2e63         self.t1.c
+0000a1c0: 6c65 6172 2829 0a20 2020 2020 2020 2077  lear().        w
+0000a1d0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000a1e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000a1f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000a200: 2830 2c20 6c65 6e28 7365 6c66 2e74 3129  (0, len(self.t1)
+0000a210: 2c20 2269 6e76 616c 6964 206c 656e 2061  , "invalid len a
+0000a220: 6674 6572 2063 6c65 6172 2229 0a20 2020  fter clear").   
+0000a230: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000a240: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000a250: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000a260: 7445 7175 616c 2831 2c20 6c65 6e28 7365  tEqual(1, len(se
+0000a270: 6c66 2e74 312e 696e 666f 2829 5b22 696e  lf.t1.info()["in
+0000a280: 6465 7865 7322 5d29 2c20 2269 6e76 616c  dexes"]), "inval
+0000a290: 6964 2069 6e64 6578 6573 2061 6674 6572  id indexes after
+0000a2a0: 2063 6c65 6172 2229 0a0a 2020 2020 6465   clear")..    de
+0000a2b0: 6620 7465 7374 5f73 7461 7473 2873 656c  f test_stats(sel
+0000a2c0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0000a2d0: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
+0000a2e0: 2020 2020 2020 6669 656c 645f 6e61 6d65        field_name
+0000a2f0: 7320 3d20 7365 6c66 2e74 312e 696e 666f  s = self.t1.info
+0000a300: 2829 5b22 6669 656c 6473 225d 0a20 2020  ()["fields"].   
+0000a310: 2020 2020 206e 756d 5f66 6965 6c64 7320       num_fields 
+0000a320: 3d20 6c65 6e28 6669 656c 645f 6e61 6d65  = len(field_name
+0000a330: 7329 0a20 2020 2020 2020 2074 315f 7374  s).        t1_st
+0000a340: 6174 7320 3d20 7365 6c66 2e74 312e 7374  ats = self.t1.st
+0000a350: 6174 7328 292e 7365 6c65 6374 2822 6e61  ats().select("na
+0000a360: 6d65 2063 6f75 6e74 206d 696e 206d 6178  me count min max
+0000a370: 206d 6561 6e22 290a 2020 2020 2020 2020   mean").        
+0000a380: 666f 7220 6669 656c 646e 616d 6520 696e  for fieldname in
+0000a390: 2066 6965 6c64 5f6e 616d 6573 3a0a 2020   field_names:.  
+0000a3a0: 2020 2020 2020 2020 2020 7374 6174 5f72            stat_r
+0000a3b0: 6563 203d 2074 315f 7374 6174 732e 6279  ec = t1_stats.by
+0000a3c0: 2e6e 616d 655b 6669 656c 646e 616d 655d  .name[fieldname]
+0000a3d0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000a3e0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+0000a3f0: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
+0000a400: 7461 7422 2c20 6669 656c 646e 616d 653d  tat", fieldname=
+0000a410: 6669 656c 646e 616d 6529 3a0a 2020 2020  fieldname):.    
+0000a420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a430: 2e61 7373 6572 7445 7175 616c 286c 742e  .assertEqual(lt.
+0000a440: 4461 7461 4f62 6a65 6374 286e 616d 653d  DataObject(name=
+0000a450: 6669 656c 646e 616d 652c 0a20 2020 2020  fieldname,.     
+0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a480: 2020 2020 2020 2020 2020 636f 756e 743d            count=
+0000a490: 7365 6c66 2e74 6573 745f 7369 7a65 202a  self.test_size *
+0000a4a0: 2a20 6e75 6d5f 6669 656c 6473 2c0a 2020  * num_fields,.  
+0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 2020 2020 2020 206d 696e               min
+0000a4e0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
 0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-0000a510: 6c69 6420 7b73 7461 747d 2073 7461 7420  lid {stat} stat 
-0000a520: 666f 7220 7b66 6965 6c64 6e61 6d65 7d22  for {fieldname}"
-0000a530: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000a540: 7374 6174 7333 2873 656c 6629 3a0a 2020  stats3(self):.  
-0000a550: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
-0000a560: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
-0000a570: 6669 656c 645f 6e61 6d65 7320 3d20 7365  field_names = se
-0000a580: 6c66 2e74 312e 696e 666f 2829 5b22 6669  lf.t1.info()["fi
-0000a590: 656c 6473 225d 0a20 2020 2020 2020 206e  elds"].        n
-0000a5a0: 756d 5f66 6965 6c64 7320 3d20 6c65 6e28  um_fields = len(
-0000a5b0: 6669 656c 645f 6e61 6d65 7329 0a0a 2020  field_names)..  
-0000a5c0: 2020 2020 2020 2320 7665 7269 6679 2074        # verify t
-0000a5d0: 6861 7420 7374 6174 7320 6361 6e20 2273  hat stats can "s
-0000a5e0: 7465 7020 6f76 6572 2220 6e6f 6e2d 6e75  tep over" non-nu
-0000a5f0: 6d65 7269 6320 6461 7461 0a20 2020 2020  meric data.     
-0000a600: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000a610: 2020 2020 7365 6c66 2e74 315b 305d 2e61      self.t1[0].a
-0000a620: 203d 2022 6e6f 7420 6120 6e75 6d62 6572   = "not a number
-0000a630: 220a 2020 2020 2020 2020 6578 6365 7074  ".        except
-0000a640: 2028 4174 7472 6962 7574 6545 7272 6f72   (AttributeError
-0000a650: 2c20 5479 7065 4572 726f 7229 3a0a 2020  , TypeError):.  
-0000a660: 2020 2020 2020 2020 2020 2320 736f 6d65            # some
-0000a670: 2074 6573 7420 7479 7065 7320 6172 656e   test types aren
-0000a680: 2774 206d 7574 6162 6c65 2c20 6d75 7374  't mutable, must
-0000a690: 2072 6570 6c61 6365 2072 6563 2077 6974   replace rec wit
-0000a6a0: 6820 6120 6d6f 6469 6669 6564 206f 6e65  h a modified one
-0000a6b0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-0000a6c0: 5f72 6563 203d 2073 656c 662e 7431 2e70  _rec = self.t1.p
-0000a6d0: 6f70 2830 290a 2020 2020 2020 2020 2020  op(0).          
-0000a6e0: 2020 7265 635f 7479 7065 203d 2074 7970    rec_type = typ
-0000a6f0: 6528 6d6f 645f 7265 6329 0a20 2020 2020  e(mod_rec).     
-0000a700: 2020 2020 2020 206e 6577 5f72 6563 5f64         new_rec_d
-0000a710: 6963 7420 3d20 6c74 2e5f 746f 5f64 6963  ict = lt._to_dic
-0000a720: 7428 6d6f 645f 7265 6329 0a20 2020 2020  t(mod_rec).     
-0000a730: 2020 2020 2020 206e 6577 5f72 6563 5f64         new_rec_d
-0000a740: 6963 745b 2761 275d 203d 2022 6e6f 7420  ict['a'] = "not 
-0000a750: 6120 6e75 6d62 6572 220a 2020 2020 2020  a number".      
-0000a760: 2020 2020 2020 6e65 775f 7265 6320 3d20        new_rec = 
-0000a770: 7265 635f 7479 7065 282a 2a6e 6577 5f72  rec_type(**new_r
-0000a780: 6563 5f64 6963 7429 0a20 2020 2020 2020  ec_dict).       
-0000a790: 2020 2020 2073 656c 662e 7431 2e69 6e73       self.t1.ins
-0000a7a0: 6572 7428 6e65 775f 7265 6329 0a0a 2020  ert(new_rec)..  
-0000a7b0: 2020 2020 2020 7431 5f73 7461 7473 203d        t1_stats =
-0000a7c0: 2073 656c 662e 7431 2e73 7461 7473 2829   self.t1.stats()
-0000a7d0: 0a20 2020 2020 2020 2074 315f 7374 6174  .        t1_stat
-0000a7e0: 7328 2274 315f 7374 6174 7322 290a 2020  s("t1_stats").  
-0000a7f0: 2020 2020 2020 7431 5f73 7461 7473 2e63        t1_stats.c
-0000a800: 7376 5f65 7870 6f72 7428 7379 732e 7374  sv_export(sys.st
-0000a810: 646f 7574 290a 2020 2020 2020 2020 7431  dout).        t1
-0000a820: 5f73 7461 7473 2e70 7265 7365 6e74 2829  _stats.present()
-0000a830: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000a840: 7365 7274 4571 7561 6c28 7365 6c66 2e74  sertEqual(self.t
-0000a850: 6573 745f 7369 7a65 202a 2a20 6e75 6d5f  est_size ** num_
-0000a860: 6669 656c 6473 202d 2031 2c20 7431 5f73  fields - 1, t1_s
-0000a870: 7461 7473 2e62 792e 6e61 6d65 5b22 6122  tats.by.name["a"
-0000a880: 5d2e 636f 756e 7429 0a0a 2020 2020 6465  ].count)..    de
-0000a890: 6620 7465 7374 5f73 7461 7473 3428 7365  f test_stats4(se
-0000a8a0: 6c66 293a 0a20 2020 2020 2020 2074 3120  lf):.        t1 
-0000a8b0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-0000a8c0: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000a8d0: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000a8e0: 2020 2020 2061 2c62 0a20 2020 2020 2020       a,b.       
-0000a8f0: 2031 2c32 0a20 2020 2020 2020 2033 2c0a   1,2.        3,.
-0000a900: 2020 2020 2020 2020 352c 340a 2020 2020          5,4.    
-0000a910: 2020 2020 2222 2229 2c20 7472 616e 7366      """), transf
-0000a920: 6f72 6d73 3d7b 7d2e 6672 6f6d 6b65 7973  orms={}.fromkeys
-0000a930: 285b 2261 222c 2022 6222 5d2c 2069 6e74  (["a", "b"], int
-0000a940: 2929 0a20 2020 2020 2020 2074 315f 7374  )).        t1_st
-0000a950: 6174 7320 3d20 7431 2e73 7461 7473 2829  ats = t1.stats()
-0000a960: 0a20 2020 2020 2020 2074 315f 7374 6174  .        t1_stat
-0000a970: 732e 7072 6573 656e 7428 290a 2020 2020  s.present().    
-0000a980: 2020 2020 7072 696e 7428 7431 5f73 7461      print(t1_sta
-0000a990: 7473 2e69 6e66 6f28 2929 0a0a 2020 2020  ts.info())..    
-0000a9a0: 2020 2020 6578 7065 6374 6564 203d 206c      expected = l
-0000a9b0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-0000a9c0: 706f 7274 2874 6578 7477 7261 702e 6465  port(textwrap.de
-0000a9d0: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
-0000a9e0: 2020 6e61 6d65 2c6d 6561 6e2c 6d69 6e2c    name,mean,min,
-0000a9f0: 6d61 782c 7661 7269 616e 6365 2c73 7464  max,variance,std
-0000aa00: 5f64 6576 2c63 6f75 6e74 2c6d 6973 7369  _dev,count,missi
-0000aa10: 6e67 0a20 2020 2020 2020 2061 2c33 2e30  ng.        a,3.0
-0000aa20: 2c31 2c35 2c34 2c32 2e30 2c33 2c30 0a20  ,1,5,4,2.0,3,0. 
-0000aa30: 2020 2020 2020 2062 2c33 2e30 2c32 2c34         b,3.0,2,4
-0000aa40: 2c32 2c31 2e34 3134 2c32 2c31 0a20 2020  ,2,1.414,2,1.   
-0000aa50: 2020 2020 2022 2222 292c 2074 7261 6e73       """), trans
-0000aa60: 666f 726d 733d 7b7d 2e66 726f 6d6b 6579  forms={}.fromkey
-0000aa70: 7328 226d 6561 6e20 6d69 6e20 6d61 7820  s("mean min max 
-0000aa80: 7661 7269 616e 6365 2073 7464 5f64 6576  variance std_dev
-0000aa90: 2063 6f75 6e74 206d 6973 7369 6e67 222e   count missing".
-0000aaa0: 7370 6c69 7428 292c 2061 7374 2e6c 6974  split(), ast.lit
-0000aab0: 6572 616c 5f65 7661 6c29 290a 2020 2020  eral_eval)).    
-0000aac0: 2020 2020 6578 7065 6374 6564 2e70 7265      expected.pre
-0000aad0: 7365 6e74 2829 0a20 2020 2020 2020 2070  sent().        p
-0000aae0: 7269 6e74 2865 7870 6563 7465 642e 696e  rint(expected.in
-0000aaf0: 666f 2829 290a 0a20 2020 2020 2020 2077  fo())..        w
-0000ab00: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000ab10: 2822 6368 6563 6b20 636f 6d70 7574 6564  ("check computed
-0000ab20: 2073 7461 7420 6669 656c 6473 2229 3a0a   stat fields"):.
-0000ab30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ab40: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-0000ab50: 6563 7465 642e 696e 666f 2829 5b22 6669  ected.info()["fi
-0000ab60: 656c 6473 225d 2c20 7431 5f73 7461 7473  elds"], t1_stats
-0000ab70: 2e69 6e66 6f28 295b 2266 6965 6c64 7322  .info()["fields"
-0000ab80: 5d29 0a0a 2020 2020 2020 2020 666f 7220  ])..        for 
-0000ab90: 6578 7065 6374 6564 5f72 6f77 2c20 726f  expected_row, ro
-0000aba0: 7720 696e 207a 6970 2865 7870 6563 7465  w in zip(expecte
-0000abb0: 642c 2074 315f 7374 6174 7329 3a0a 2020  d, t1_stats):.  
-0000abc0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-0000abd0: 656c 662e 7375 6254 6573 7428 2263 6865  elf.subTest("che
-0000abe0: 636b 2063 6f6d 7075 7465 6420 7374 6174  ck computed stat
-0000abf0: 2061 7474 7269 6275 7465 2028 6e61 6d65   attribute (name
-0000ac00: 2922 2c20 726f 773d 726f 7729 3a0a 2020  )", row=row):.  
-0000ac10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ac20: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0000ac30: 7870 6563 7465 645f 726f 772e 6e61 6d65  xpected_row.name
-0000ac40: 2c20 726f 772e 6e61 6d65 290a 2020 2020  , row.name).    
-0000ac50: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000ac60: 662e 7375 6254 6573 7428 2263 6865 636b  f.subTest("check
-0000ac70: 2063 6f6d 7075 7465 6420 7374 6174 2061   computed stat a
-0000ac80: 7474 7269 6275 7465 2028 6d65 616e 2922  ttribute (mean)"
-0000ac90: 2c20 726f 773d 726f 7729 3a0a 2020 2020  , row=row):.    
-0000aca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000acb0: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-0000acc0: 6563 7465 645f 726f 772e 6d65 616e 2c20  ected_row.mean, 
-0000acd0: 726f 772e 6d65 616e 290a 2020 2020 2020  row.mean).      
-0000ace0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000acf0: 7375 6254 6573 7428 2263 6865 636b 2063  subTest("check c
-0000ad00: 6f6d 7075 7465 6420 7374 6174 2061 7474  omputed stat att
-0000ad10: 7269 6275 7465 2028 6d69 6e29 222c 2072  ribute (min)", r
-0000ad20: 6f77 3d72 6f77 293a 0a20 2020 2020 2020  ow=row):.       
-0000ad30: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000ad40: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000ad50: 6564 5f72 6f77 2e6d 696e 2c20 726f 772e  ed_row.min, row.
-0000ad60: 6d69 6e29 0a20 2020 2020 2020 2020 2020  min).           
-0000ad70: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000ad80: 7374 2822 6368 6563 6b20 636f 6d70 7574  st("check comput
-0000ad90: 6564 2073 7461 7420 6174 7472 6962 7574  ed stat attribut
-0000ada0: 6520 286d 6178 2922 2c20 726f 773d 726f  e (max)", row=ro
-0000adb0: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
-0000adc0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000add0: 7175 616c 2865 7870 6563 7465 645f 726f  qual(expected_ro
-0000ade0: 772e 6d61 782c 2072 6f77 2e6d 6178 290a  w.max, row.max).
-0000adf0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000ae00: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
-0000ae10: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
-0000ae20: 6174 2061 7474 7269 6275 7465 2028 7661  at attribute (va
-0000ae30: 7269 616e 6365 2922 2c20 726f 773d 726f  riance)", row=ro
-0000ae40: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
-0000ae50: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000ae60: 7175 616c 2865 7870 6563 7465 645f 726f  qual(expected_ro
-0000ae70: 772e 7661 7269 616e 6365 2c20 726f 772e  w.variance, row.
-0000ae80: 7661 7269 616e 6365 290a 2020 2020 2020  variance).      
-0000ae90: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000aea0: 7375 6254 6573 7428 2263 6865 636b 2063  subTest("check c
-0000aeb0: 6f6d 7075 7465 6420 7374 6174 2061 7474  omputed stat att
-0000aec0: 7269 6275 7465 2028 7374 645f 6465 7629  ribute (std_dev)
-0000aed0: 222c 2072 6f77 3d72 6f77 293a 0a20 2020  ", row=row):.   
-0000aee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000aef0: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000af00: 7065 6374 6564 5f72 6f77 2e73 7464 5f64  pected_row.std_d
-0000af10: 6576 2c20 726f 772e 7374 645f 6465 7629  ev, row.std_dev)
-0000af20: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000af30: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-0000af40: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
-0000af50: 7461 7420 6174 7472 6962 7574 6520 2863  tat attribute (c
-0000af60: 6f75 6e74 2922 2c20 726f 773d 726f 7729  ount)", row=row)
-0000af70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000af80: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000af90: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
-0000afa0: 636f 756e 742c 2072 6f77 2e63 6f75 6e74  count, row.count
-0000afb0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0000afc0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000afd0: 2263 6865 636b 2063 6f6d 7075 7465 6420  "check computed 
-0000afe0: 7374 6174 2061 7474 7269 6275 7465 2028  stat attribute (
-0000aff0: 6d69 7373 696e 6729 222c 2072 6f77 3d72  missing)", row=r
-0000b000: 6f77 293a 0a20 2020 2020 2020 2020 2020  ow):.           
-0000b010: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b020: 4571 7561 6c28 6578 7065 6374 6564 5f72  Equal(expected_r
-0000b030: 6f77 2e6d 6973 7369 6e67 2c20 726f 772e  ow.missing, row.
-0000b040: 6d69 7373 696e 6729 0a0a 2020 2020 6465  missing)..    de
-0000b050: 6620 7465 7374 5f73 706c 6974 6279 2873  f test_splitby(s
-0000b060: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0000b070: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
-0000b080: 2020 2020 2020 2020 6973 5f6f 6464 203d          is_odd =
-0000b090: 206c 616d 6264 6120 7265 633a 2072 6563   lambda rec: rec
-0000b0a0: 2e61 2025 2032 0a20 2020 2020 2020 2065  .a % 2.        e
-0000b0b0: 7665 6e73 2c20 6f64 6473 203d 2073 656c  vens, odds = sel
-0000b0c0: 662e 7431 2e73 706c 6974 6279 2869 735f  f.t1.splitby(is_
-0000b0d0: 6f64 6429 0a20 2020 2020 2020 2077 6974  odd).        wit
-0000b0e0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000b0f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000b100: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-0000b110: 656e 286f 6464 7329 202b 206c 656e 2865  en(odds) + len(e
-0000b120: 7665 6e73 292c 206c 656e 2873 656c 662e  vens), len(self.
-0000b130: 7431 2929 0a20 2020 2020 2020 2077 6974  t1)).        wit
-0000b140: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000b150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000b160: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-0000b170: 656e 286f 6464 7329 2c20 6c65 6e28 7365  en(odds), len(se
-0000b180: 6c66 2e74 312e 7768 6572 6528 6973 5f6f  lf.t1.where(is_o
-0000b190: 6464 2929 290a 0a20 2020 2020 2020 2065  dd)))..        e
-0000b1a0: 7665 6e5f 6576 656e 732c 206f 6464 5f65  ven_evens, odd_e
-0000b1b0: 7665 6e73 203d 2065 7665 6e73 2e73 706c  vens = evens.spl
-0000b1c0: 6974 6279 2869 735f 6f64 6429 0a20 2020  itby(is_odd).   
-0000b1d0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000b1e0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000b1f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000b200: 7445 7175 616c 2830 2c20 6c65 6e28 6f64  tEqual(0, len(od
-0000b210: 645f 6576 656e 7329 290a 2020 2020 2020  d_evens)).      
-0000b220: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000b230: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000b240: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000b250: 7561 6c28 6c65 6e28 6576 656e 5f65 7665  ual(len(even_eve
-0000b260: 6e73 292c 206c 656e 2865 7665 6e73 2929  ns), len(evens))
-0000b270: 0a0a 2020 2020 2020 2020 2320 6d61 6b65  ..        # make
-0000b280: 2073 7572 6520 696e 6465 7865 7320 6172   sure indexes ar
-0000b290: 6520 7072 6573 6572 7665 640a 2020 2020  e preserved.    
-0000b2a0: 2020 2020 7365 6c66 2e74 312e 6372 6561      self.t1.crea
-0000b2b0: 7465 5f69 6e64 6578 2822 6122 290a 2020  te_index("a").  
-0000b2c0: 2020 2020 2020 6576 656e 732c 206f 6464        evens, odd
-0000b2d0: 7320 3d20 7365 6c66 2e74 312e 7370 6c69  s = self.t1.spli
-0000b2e0: 7462 7928 6973 5f6f 6464 290a 2020 2020  tby(is_odd).    
-0000b2f0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000b300: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000b310: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b320: 4571 7561 6c28 7365 6c66 2e74 312e 696e  Equal(self.t1.in
-0000b330: 666f 2829 5b22 696e 6465 7865 7322 5d2c  fo()["indexes"],
-0000b340: 2065 7665 6e73 2e69 6e66 6f28 295b 2269   evens.info()["i
-0000b350: 6e64 6578 6573 225d 290a 0a20 2020 2020  ndexes"])..     
-0000b360: 2020 2023 2074 6573 7420 7061 7373 696e     # test passin
-0000b370: 6720 616e 2061 7474 7269 6275 7465 2061  g an attribute a
-0000b380: 7320 6120 6b65 790a 2020 2020 2020 2020  s a key.        
-0000b390: 7a65 726f 732c 206e 6f6e 5f7a 6572 6f73  zeros, non_zeros
-0000b3a0: 203d 2073 656c 662e 7431 2e73 706c 6974   = self.t1.split
-0000b3b0: 6279 2822 6122 290a 2020 2020 2020 2020  by("a").        
-0000b3c0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000b3d0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000b3e0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0000b3f0: 2861 6c6c 2872 6563 2e61 203d 3d20 3020  (all(rec.a == 0 
-0000b400: 666f 7220 7265 6320 696e 207a 6572 6f73  for rec in zeros
-0000b410: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-0000b420: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-0000b430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b440: 2e61 7373 6572 7454 7275 6528 616c 6c28  .assertTrue(all(
-0000b450: 7265 632e 6120 213d 2030 2066 6f72 2072  rec.a != 0 for r
-0000b460: 6563 2069 6e20 6e6f 6e5f 7a65 726f 7329  ec in non_zeros)
-0000b470: 290a 0a20 2020 2020 2020 2023 2074 6573  )..        # tes
-0000b480: 7420 7573 696e 6720 7072 6564 6963 6174  t using predicat
-0000b490: 6520 7468 6174 2064 6f65 7320 6e6f 7420  e that does not 
-0000b4a0: 616c 7761 7973 2072 6574 7572 6e20 3020  always return 0 
-0000b4b0: 6f72 2031 0a20 2020 2020 2020 2069 735f  or 1.        is_
-0000b4c0: 6e6f 745f 6d75 6c74 6970 6c65 5f6f 665f  not_multiple_of_
-0000b4d0: 3320 3d20 6c61 6d62 6461 2072 6563 3a20  3 = lambda rec: 
-0000b4e0: 7265 632e 6120 2520 330a 2020 2020 2020  rec.a % 3.      
-0000b4f0: 2020 6d75 6c74 735f 6f66 5f33 2c20 6e6f    mults_of_3, no
-0000b500: 6e5f 6d75 6c74 735f 6f66 5f33 203d 2073  n_mults_of_3 = s
-0000b510: 656c 662e 7431 2e73 706c 6974 6279 2869  elf.t1.splitby(i
-0000b520: 735f 6e6f 745f 6d75 6c74 6970 6c65 5f6f  s_not_multiple_o
-0000b530: 665f 3329 0a20 2020 2020 2020 2070 7269  f_3).        pri
-0000b540: 6e74 286c 6973 7428 6e6f 6e5f 6d75 6c74  nt(list(non_mult
-0000b550: 735f 6f66 5f33 2e61 6c6c 2e61 2929 0a20  s_of_3.all.a)). 
-0000b560: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
-0000b570: 7428 6d75 6c74 735f 6f66 5f33 2e61 6c6c  t(mults_of_3.all
-0000b580: 2e61 2929 0a20 2020 2020 2020 2023 2054  .a)).        # T
-0000b590: 4f44 4f20 2d20 6164 6420 6173 7365 7274  ODO - add assert
-0000b5a0: 7320 6865 7265 0a0a 0a40 6d61 6b65 5f74  s here...@make_t
-0000b5b0: 6573 745f 636c 6173 7365 730a 636c 6173  est_classes.clas
-0000b5c0: 7320 5461 626c 654a 6f69 6e54 6573 7473  s TableJoinTests
-0000b5d0: 3a0a 2020 2020 6465 6620 7465 7374 5f73  :.    def test_s
-0000b5e0: 696d 706c 655f 6a6f 696e 2873 656c 6629  imple_join(self)
-0000b5f0: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
-0000b600: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
-0000b610: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
-0000b620: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
-0000b630: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
-0000b640: 745f 7369 7a65 290a 2020 2020 2020 2020  t_size).        
-0000b650: 7431 2e63 7265 6174 655f 696e 6465 7828  t1.create_index(
-0000b660: 2761 2729 0a0a 2020 2020 2020 2020 7432  'a')..        t2
-0000b670: 203d 206c 742e 5461 626c 6528 290a 2020   = lt.Table().  
-0000b680: 2020 2020 2020 7432 2e63 7265 6174 655f        t2.create_
-0000b690: 696e 6465 7828 2761 2729 0a20 2020 2020  index('a').     
-0000b6a0: 2020 2074 322e 696e 7365 7274 286c 742e     t2.insert(lt.
-0000b6b0: 4461 7461 4f62 6a65 6374 2861 3d31 2c20  DataObject(a=1, 
-0000b6c0: 643d 3130 3029 290a 0a20 2020 2020 2020  d=100))..       
-0000b6d0: 206a 6f69 6e65 6420 3d20 2874 312e 6a6f   joined = (t1.jo
-0000b6e0: 696e 5f6f 6e28 2761 2729 202b 2074 322e  in_on('a') + t2.
-0000b6f0: 6a6f 696e 5f6f 6e28 2761 2729 2928 290a  join_on('a'))().
-0000b700: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000b710: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000b720: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000b730: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-0000b740: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
-0000b750: 206c 656e 286a 6f69 6e65 6429 290a 0a20   len(joined)).. 
-0000b760: 2020 2020 2020 206a 6f69 6e65 6420 3d20         joined = 
-0000b770: 2874 312e 6a6f 696e 5f6f 6e28 2761 2729  (t1.join_on('a')
-0000b780: 202b 2074 3229 2829 0a20 2020 2020 2020   + t2)().       
-0000b790: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000b7a0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000b7b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000b7c0: 616c 2874 6573 745f 7369 7a65 202a 2074  al(test_size * t
-0000b7d0: 6573 745f 7369 7a65 2c20 6c65 6e28 6a6f  est_size, len(jo
-0000b7e0: 696e 6564 2929 0a0a 2020 2020 2020 2020  ined))..        
-0000b7f0: 6a6f 696e 6564 203d 2028 7431 202b 2074  joined = (t1 + t
-0000b800: 322e 6a6f 696e 5f6f 6e28 2761 2729 2928  2.join_on('a'))(
-0000b810: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000b820: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000b830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b840: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-0000b850: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
-0000b860: 652c 206c 656e 286a 6f69 6e65 6429 290a  e, len(joined)).
-0000b870: 0a20 2020 2020 2020 2074 312e 6465 6c65  .        t1.dele
-0000b880: 7465 5f69 6e64 6578 2827 6127 290a 2020  te_index('a').  
-0000b890: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000b8a0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000b8b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000b8c0: 2e61 7373 6572 7452 6169 7365 7328 5661  .assertRaises(Va
-0000b8d0: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
-0000b8e0: 2020 2020 2020 2020 2020 206a 6f69 6e65             joine
-0000b8f0: 6420 3d20 2874 3120 2b20 7432 2e6a 6f69  d = (t1 + t2.joi
-0000b900: 6e5f 6f6e 2827 6127 2929 2829 0a0a 2020  n_on('a'))()..  
-0000b910: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000b920: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000b930: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000b940: 2e61 7373 6572 7452 6169 7365 7328 5479  .assertRaises(Ty
-0000b950: 7065 4572 726f 7229 3a0a 2020 2020 2020  peError):.      
-0000b960: 2020 2020 2020 2020 2020 2320 696e 7661            # inva
-0000b970: 6c69 6420 6a6f 696e 2c20 6e6f 206b 7761  lid join, no kwa
-0000b980: 7267 7320 6c69 7374 696e 6720 6174 7472  rgs listing attr
-0000b990: 6962 7574 6573 2074 6f20 6a6f 696e 206f  ibutes to join o
-0000b9a0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000b9b0: 2020 7433 203d 2074 312e 6a6f 696e 2874    t3 = t1.join(t
-0000b9c0: 322c 2027 612c 6427 290a 0a20 2020 2020  2, 'a,d')..     
-0000b9d0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000b9e0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000b9f0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-0000ba00: 7365 7274 5261 6973 6573 2856 616c 7565  sertRaises(Value
-0000ba10: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-0000ba20: 2020 2020 2020 2020 2320 696e 7661 6c69          # invali
-0000ba30: 6420 6a6f 696e 2c20 6e6f 2073 7563 6820  d join, no such 
-0000ba40: 6174 7472 6962 7574 6520 277a 270a 2020  attribute 'z'.  
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 7433                t3
-0000ba60: 203d 2074 312e 6a6f 696e 2874 322c 2027   = t1.join(t2, '
-0000ba70: 612c 642c 7a27 2c20 613d 2761 2729 0a0a  a,d,z', a='a')..
-0000ba80: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
-0000ba90: 6a6f 696e 2874 322c 2027 612c 6427 2c20  join(t2, 'a,d', 
-0000baa0: 613d 2761 2729 0a20 2020 2020 2020 2077  a='a').        w
-0000bab0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000bac0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000bad0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000bae0: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
-0000baf0: 745f 7369 7a65 2c20 6c65 6e28 7433 2929  t_size, len(t3))
-0000bb00: 0a0a 2020 2020 2020 2020 7434 203d 2074  ..        t4 = t
-0000bb10: 312e 6a6f 696e 2874 322c 2061 3d27 6127  1.join(t2, a='a'
-0000bb20: 292e 7365 6c65 6374 2827 6120 6320 6427  ).select('a c d'
-0000bb30: 2c20 653d 6c61 6d62 6461 2072 6563 3a20  , e=lambda rec: 
-0000bb40: 7265 632e 6120 2b20 7265 632e 6320 2b20  rec.a + rec.c + 
-0000bb50: 7265 632e 6429 0a20 2020 2020 2020 2077  rec.d).        w
-0000bb60: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000bb70: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000bb80: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-0000bb90: 616c 6c28 7265 632e 6520 3d3d 2072 6563  all(rec.e == rec
-0000bba0: 2e61 2b72 6563 2e63 2b72 6563 2e64 2066  .a+rec.c+rec.d f
-0000bbb0: 6f72 2072 6563 2069 6e20 7434 2929 0a0a  or rec in t4))..
-0000bbc0: 2020 2020 2020 2020 2320 6a6f 696e 2074          # join t
-0000bbd0: 6f20 656d 7074 7920 6c69 7374 2c20 7368  o empty list, sh
-0000bbe0: 6f75 6c64 2072 6574 7572 6e20 656d 7074  ould return empt
-0000bbf0: 7920 7461 626c 650a 2020 2020 2020 2020  y table.        
-0000bc00: 656d 7074 795f 7461 626c 6520 3d20 6c74  empty_table = lt
-0000bc10: 2e54 6162 6c65 2829 0a20 2020 2020 2020  .Table().       
-0000bc20: 2065 6d70 7479 5f74 6162 6c65 2e63 7265   empty_table.cre
-0000bc30: 6174 655f 696e 6465 7828 2761 2729 0a20  ate_index('a'). 
-0000bc40: 2020 2020 2020 2074 3520 3d20 2874 312e         t5 = (t1.
-0000bc50: 6a6f 696e 5f6f 6e28 2761 2729 202b 2065  join_on('a') + e
-0000bc60: 6d70 7479 5f74 6162 6c65 2928 290a 2020  mpty_table)().  
-0000bc70: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000bc80: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000bc90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000bca0: 7274 4571 7561 6c28 302c 206c 656e 2874  rtEqual(0, len(t
-0000bcb0: 3529 290a 0a20 2020 2064 6566 2074 6573  5))..    def tes
-0000bcc0: 745f 6f75 7465 725f 6a6f 696e 7328 7365  t_outer_joins(se
-0000bcd0: 6c66 293a 0a20 2020 2020 2020 2074 3120  lf):.        t1 
-0000bce0: 3d20 6c74 2e54 6162 6c65 2822 6361 7461  = lt.Table("cata
-0000bcf0: 6c6f 6722 290a 2020 2020 2020 2020 7431  log").        t1
-0000bd00: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-0000bd10: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000bd20: 0a20 2020 2020 2020 2020 2020 2073 6b75  .            sku
-0000bd30: 2c63 6f6c 6f72 2c73 697a 652c 6d61 7465  ,color,size,mate
-0000bd40: 7269 616c 0a20 2020 2020 2020 2020 2020  rial.           
-0000bd50: 2030 3031 2c72 6564 2c58 4c2c 636f 7474   001,red,XL,cott
-0000bd60: 6f6e 0a20 2020 2020 2020 2020 2020 2030  on.            0
-0000bd70: 3032 2c62 6c75 652c 584c 2c63 6f74 746f  02,blue,XL,cotto
-0000bd80: 6e2f 706f 6c79 0a20 2020 2020 2020 2020  n/poly.         
-0000bd90: 2020 2030 3033 2c62 6c75 652c 4c2c 6c69     003,blue,L,li
-0000bda0: 6e65 6e0a 2020 2020 2020 2020 2020 2020  nen.            
-0000bdb0: 3030 342c 7265 642c 4d2c 636f 7474 6f6e  004,red,M,cotton
-0000bdc0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000bdd0: 2929 0a0a 2020 2020 2020 2020 7432 203d  ))..        t2 =
-0000bde0: 206c 742e 5461 626c 6528 2270 7269 6365   lt.Table("price
-0000bdf0: 7322 290a 2020 2020 2020 2020 7432 2e63  s").        t2.c
-0000be00: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
-0000be10: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000be20: 2020 2020 2020 2020 2020 2073 6b75 2c75             sku,u
-0000be30: 6e69 745f 7072 6963 652c 7369 7a65 0a20  nit_price,size. 
-0000be40: 2020 2020 2020 2020 2020 2030 3031 2c31             001,1
-0000be50: 302c 4c0a 2020 2020 2020 2020 2020 2020  0,L.            
-0000be60: 3030 312c 3132 2c58 4c0a 2020 2020 2020  001,12,XL.      
-0000be70: 2020 2020 2020 3030 322c 3131 2c0a 2020        002,11,.  
-0000be80: 2020 2020 2020 2020 2020 3030 342c 392c            004,9,
-0000be90: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000bea0: 292c 2074 7261 6e73 666f 726d 733d 7b27  ), transforms={'
-0000beb0: 7369 7a65 273a 206c 616d 6264 6120 783a  size': lambda x:
-0000bec0: 2078 206f 7220 4e6f 6e65 7d29 0a20 2020   x or None}).   
-0000bed0: 2020 2020 2070 7269 6e74 2874 312e 696e       print(t1.in
-0000bee0: 666f 2829 290a 0a20 2020 2020 2020 2074  fo())..        t
-0000bef0: 312e 7072 6573 656e 7428 290a 2020 2020  1.present().    
-0000bf00: 2020 2020 7432 2e70 7265 7365 6e74 2829      t2.present()
-0000bf10: 0a0a 2020 2020 2020 2020 7433 203d 2074  ..        t3 = t
-0000bf20: 312e 6a6f 696e 2874 322c 2061 7574 6f5f  1.join(t2, auto_
-0000bf30: 6372 6561 7465 5f69 6e64 6578 6573 3d54  create_indexes=T
-0000bf40: 7275 652c 2073 6b75 3d22 736b 7522 290a  rue, sku="sku").
-0000bf50: 2020 2020 2020 2020 7072 696e 7428 7433          print(t3
-0000bf60: 2e69 6e66 6f28 2929 0a20 2020 2020 2020  .info()).       
-0000bf70: 2074 332e 7072 6573 656e 7428 290a 2020   t3.present().  
-0000bf80: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000bf90: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000bfa0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000bfb0: 7274 4571 7561 6c28 342c 206c 656e 2874  rtEqual(4, len(t
-0000bfc0: 3329 290a 0a20 2020 2020 2020 2074 3320  3))..        t3 
-0000bfd0: 3d20 7431 2e6a 6f69 6e28 7432 2c20 6175  = t1.join(t2, au
-0000bfe0: 746f 5f63 7265 6174 655f 696e 6465 7865  to_create_indexe
-0000bff0: 733d 5472 7565 2c20 736b 753d 2273 6b75  s=True, sku="sku
-0000c000: 222c 2073 697a 653d 2273 697a 6522 290a  ", size="size").
-0000c010: 2020 2020 2020 2020 7433 2822 696e 6e65          t3("inne
-0000c020: 7220 6a6f 696e 202d 2022 202b 2074 332e  r join - " + t3.
-0000c030: 7461 626c 655f 6e61 6d65 290a 2020 2020  table_name).    
-0000c040: 2020 2020 7072 696e 7428 7433 2e69 6e66      print(t3.inf
-0000c050: 6f28 2929 0a20 2020 2020 2020 2074 332e  o()).        t3.
-0000c060: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000c070: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000c080: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000c090: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000c0a0: 7561 6c28 312c 206c 656e 2874 3329 290a  ual(1, len(t3)).
-0000c0b0: 0a20 2020 2020 2020 2074 3320 3d20 7431  .        t3 = t1
-0000c0c0: 2e6f 7574 6572 5f6a 6f69 6e28 6c74 2e54  .outer_join(lt.T
-0000c0d0: 6162 6c65 2e52 4947 4854 5f4f 5554 4552  able.RIGHT_OUTER
-0000c0e0: 5f4a 4f49 4e2c 2074 322c 2073 6b75 3d22  _JOIN, t2, sku="
-0000c0f0: 736b 7522 2c20 7369 7a65 3d22 7369 7a65  sku", size="size
-0000c100: 2229 0a20 2020 2020 2020 2074 3328 2272  ").        t3("r
-0000c110: 6967 6874 206f 7574 6572 206a 6f69 6e20  ight outer join 
-0000c120: 2d20 2220 2b20 7433 2e74 6162 6c65 5f6e  - " + t3.table_n
-0000c130: 616d 6529 0a20 2020 2020 2020 2070 7269  ame).        pri
-0000c140: 6e74 2874 332e 696e 666f 2829 290a 2020  nt(t3.info()).  
-0000c150: 2020 2020 2020 7433 2e70 7265 7365 6e74        t3.present
-0000c160: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
-0000c170: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-0000c180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c190: 2e61 7373 6572 7445 7175 616c 2834 2c20  .assertEqual(4, 
-0000c1a0: 6c65 6e28 7433 2929 0a0a 2020 2020 2020  len(t3))..      
-0000c1b0: 2020 7433 203d 2074 312e 6f75 7465 725f    t3 = t1.outer_
-0000c1c0: 6a6f 696e 286c 742e 5461 626c 652e 4c45  join(lt.Table.LE
-0000c1d0: 4654 5f4f 5554 4552 5f4a 4f49 4e2c 2074  FT_OUTER_JOIN, t
-0000c1e0: 322c 2073 6b75 3d22 736b 7522 2c20 7369  2, sku="sku", si
-0000c1f0: 7a65 3d22 7369 7a65 2229 0a20 2020 2020  ze="size").     
-0000c200: 2020 2074 3328 226c 6566 7420 6f75 7465     t3("left oute
-0000c210: 7220 6a6f 696e 202d 2022 202b 2074 332e  r join - " + t3.
-0000c220: 7461 626c 655f 6e61 6d65 290a 2020 2020  table_name).    
-0000c230: 2020 2020 7072 696e 7428 7433 2e69 6e66      print(t3.inf
-0000c240: 6f28 2929 0a20 2020 2020 2020 2074 332e  o()).        t3.
-0000c250: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000c260: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000c270: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000c280: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000c290: 7561 6c28 322c 206c 656e 2874 3329 290a  ual(2, len(t3)).
-0000c2a0: 0a20 2020 2020 2020 2074 3320 3d20 7431  .        t3 = t1
-0000c2b0: 2e6f 7574 6572 5f6a 6f69 6e28 6c74 2e54  .outer_join(lt.T
-0000c2c0: 6162 6c65 2e46 554c 4c5f 4f55 5445 525f  able.FULL_OUTER_
-0000c2d0: 4a4f 494e 2c20 7432 2c20 736b 753d 2273  JOIN, t2, sku="s
-0000c2e0: 6b75 222c 2073 697a 653d 2273 697a 6522  ku", size="size"
-0000c2f0: 290a 2020 2020 2020 2020 7433 2822 6675  ).        t3("fu
-0000c300: 6c6c 206f 7574 6572 206a 6f69 6e20 2d20  ll outer join - 
-0000c310: 2220 2b20 7433 2e74 6162 6c65 5f6e 616d  " + t3.table_nam
-0000c320: 6529 0a20 2020 2020 2020 2070 7269 6e74  e).        print
-0000c330: 2874 332e 696e 666f 2829 290a 2020 2020  (t3.info()).    
-0000c340: 2020 2020 7433 2e70 7265 7365 6e74 2829      t3.present()
-0000c350: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000c360: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000c370: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000c380: 7373 6572 7445 7175 616c 2831 322c 206c  ssertEqual(12, l
-0000c390: 656e 2874 3329 290a 0a20 2020 2064 6566  en(t3))..    def
-0000c3a0: 2074 6573 745f 6f75 7465 725f 6a6f 696e   test_outer_join
-0000c3b0: 5f65 7861 6d70 6c65 2873 656c 6629 3a0a  _example(self):.
-0000c3c0: 2020 2020 2020 2020 2320 6465 6669 6e65          # define
-0000c3d0: 2073 7475 6465 6e74 2061 6e64 2072 6567   student and reg
-0000c3e0: 6973 7472 6174 696f 6e20 6461 7461 0a20  istration data. 
-0000c3f0: 2020 2020 2020 2073 7475 6465 6e74 7320         students 
-0000c400: 3d20 6c74 2e54 6162 6c65 2822 7374 7564  = lt.Table("stud
-0000c410: 656e 7473 2229 2e63 7376 5f69 6d70 6f72  ents").csv_impor
-0000c420: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000c430: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000c440: 2020 2073 7475 6465 6e74 5f69 642c 6e61     student_id,na
-0000c450: 6d65 0a20 2020 2020 2020 2020 2020 2030  me.            0
-0000c460: 3030 312c 416c 6963 650a 2020 2020 2020  001,Alice.      
-0000c470: 2020 2020 2020 3030 3032 2c42 6f62 0a20        0002,Bob. 
-0000c480: 2020 2020 2020 2020 2020 2030 3030 332c             0003,
-0000c490: 4368 6172 6c69 650a 2020 2020 2020 2020  Charlie.        
-0000c4a0: 2020 2020 3030 3034 2c44 6176 650a 2020      0004,Dave.  
-0000c4b0: 2020 2020 2020 2020 2020 3030 3035 2c45            0005,E
-0000c4c0: 6e69 640a 2020 2020 2020 2020 2020 2020  nid.            
-0000c4d0: 2222 2229 290a 0a20 2020 2020 2020 2072  """))..        r
-0000c4e0: 6567 6973 7472 6174 696f 6e73 203d 206c  egistrations = l
-0000c4f0: 742e 5461 626c 6528 2272 6567 6973 7472  t.Table("registr
-0000c500: 6174 696f 6e73 2229 2e63 7376 5f69 6d70  ations").csv_imp
-0000c510: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
-0000c520: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-0000c530: 2020 2020 2073 7475 6465 6e74 5f69 642c       student_id,
-0000c540: 636f 7572 7365 0a20 2020 2020 2020 2020  course.         
-0000c550: 2020 2030 3030 312c 5053 5943 4831 3031     0001,PSYCH101
-0000c560: 0a20 2020 2020 2020 2020 2020 2030 3030  .            000
-0000c570: 312c 4341 4c43 310a 2020 2020 2020 2020  1,CALC1.        
-0000c580: 2020 2020 3030 3033 2c42 494f 3230 300a      0003,BIO200.
-0000c590: 2020 2020 2020 2020 2020 2020 3030 3035              0005
-0000c5a0: 2c43 4845 4d31 3031 0a20 2020 2020 2020  ,CHEM101.       
-0000c5b0: 2020 2020 2030 3030 362c 5048 5931 3031       0006,PHY101
-0000c5c0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000c5d0: 2929 0a0a 2020 2020 2020 2020 636f 7572  ))..        cour
-0000c5e0: 7365 7320 3d20 6c74 2e54 6162 6c65 2822  ses = lt.Table("
-0000c5f0: 636f 7572 7365 7322 292e 6373 765f 696d  courses").csv_im
-0000c600: 706f 7274 2874 6578 7477 7261 702e 6465  port(textwrap.de
-0000c610: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
-0000c620: 2020 2020 2020 636f 7572 7365 0a20 2020        course.   
-0000c630: 2020 2020 2020 2020 2042 494f 3230 300a           BIO200.
-0000c640: 2020 2020 2020 2020 2020 2020 4341 4c43              CALC
-0000c650: 310a 2020 2020 2020 2020 2020 2020 4348  1.            CH
-0000c660: 454d 3130 310a 2020 2020 2020 2020 2020  EM101.          
-0000c670: 2020 5053 5943 4831 3031 0a20 2020 2020    PSYCH101.     
-0000c680: 2020 2020 2020 2050 4531 3031 0a20 2020         PE101.   
-0000c690: 2020 2020 2020 2020 2022 2222 2929 0a0a           """))..
-0000c6a0: 2020 2020 2020 2020 2320 7065 7266 6f72          # perfor
-0000c6b0: 6d20 6f75 7465 7220 6a6f 696e 2061 6e64  m outer join and
-0000c6c0: 2073 686f 7720 7265 7375 6c74 733a 0a20   show results:. 
-0000c6d0: 2020 2020 2020 206e 6f6e 5f72 6567 203d         non_reg =
-0000c6e0: 2073 7475 6465 6e74 732e 6f75 7465 725f   students.outer_
-0000c6f0: 6a6f 696e 286c 742e 5461 626c 652e 5249  join(lt.Table.RI
-0000c700: 4748 545f 4f55 5445 525f 4a4f 494e 2c0a  GHT_OUTER_JOIN,.
-0000c710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2020 2020 2020 7265 6769 7374 7261 7469        registrati
-0000c740: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 2020 2020 2020 2073 7475 6465             stude
-0000c770: 6e74 5f69 643d 2273 7475 6465 6e74 5f69  nt_id="student_i
-0000c780: 6422 292e 7768 6572 6528 636f 7572 7365  d").where(course
-0000c790: 3d4e 6f6e 6529 0a20 2020 2020 2020 206e  =None).        n
-0000c7a0: 6f6e 5f72 6567 2e70 7265 7365 6e74 2829  on_reg.present()
-0000c7b0: 0a20 2020 2020 2020 2070 7269 6e74 286c  .        print(l
-0000c7c0: 6973 7428 6e6f 6e5f 7265 672e 616c 6c2e  ist(non_reg.all.
-0000c7d0: 6e61 6d65 2929 0a20 2020 2020 2020 2077  name)).        w
-0000c7e0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000c7f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000c800: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000c810: 285b 2742 6f62 272c 2027 4461 7665 275d  (['Bob', 'Dave']
-0000c820: 2c20 736f 7274 6564 286e 6f6e 5f72 6567  , sorted(non_reg
-0000c830: 2e61 6c6c 2e6e 616d 6529 290a 0a20 2020  .all.name))..   
-0000c840: 2020 2020 2023 2063 6f75 7273 6573 2077       # courses w
-0000c850: 6974 6820 6e6f 2073 7475 6465 6e74 730a  ith no students.
-0000c860: 2020 2020 2020 2020 6e6f 5f73 7475 6465          no_stude
-0000c870: 6e74 7320 3d20 7265 6769 7374 7261 7469  nts = registrati
-0000c880: 6f6e 732e 6f75 7465 725f 6a6f 696e 286c  ons.outer_join(l
-0000c890: 742e 5461 626c 652e 4c45 4654 5f4f 5554  t.Table.LEFT_OUT
-0000c8a0: 4552 5f4a 4f49 4e2c 0a20 2020 2020 2020  ER_JOIN,.       
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8d0: 2020 636f 7572 7365 732c 0a20 2020 2020    courses,.     
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c900: 2020 2020 636f 7572 7365 3d22 636f 7572      course="cour
-0000c910: 7365 2229 2e77 6865 7265 2873 7475 6465  se").where(stude
-0000c920: 6e74 5f69 643d 4e6f 6e65 290a 2020 2020  nt_id=None).    
-0000c930: 2020 2020 6e6f 5f73 7475 6465 6e74 732e      no_students.
-0000c940: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000c950: 2020 7072 696e 7428 6c69 7374 286e 6f5f    print(list(no_
-0000c960: 7374 7564 656e 7473 2e61 6c6c 2e63 6f75  students.all.cou
-0000c970: 7273 6529 290a 2020 2020 2020 2020 7769  rse)).        wi
-0000c980: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000c990: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000c9a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000c9b0: 5b27 5045 3130 3127 5d2c 2073 6f72 7465  ['PE101'], sorte
-0000c9c0: 6428 6e6f 5f73 7475 6465 6e74 732e 616c  d(no_students.al
-0000c9d0: 6c2e 636f 7572 7365 2929 0a0a 0a20 2020  l.course))...   
-0000c9e0: 2020 2020 2066 756c 6c20 3d20 2073 7475       full =  stu
-0000c9f0: 6465 6e74 732e 6f75 7465 725f 6a6f 696e  dents.outer_join
-0000ca00: 286c 742e 5461 626c 652e 4655 4c4c 5f4f  (lt.Table.FULL_O
-0000ca10: 5554 4552 5f4a 4f49 4e2c 0a20 2020 2020  UTER_JOIN,.     
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 206d 6178 3d73 656c 662e 7465 7374     max=self.test
+0000a520: 5f73 697a 6520 2d20 312c 0a20 2020 2020  _size - 1,.     
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a550: 2020 2020 2020 2020 2020 6d65 616e 3d28            mean=(
+0000a560: 7365 6c66 2e74 6573 745f 7369 7a65 202d  self.test_size -
+0000a570: 2031 2920 2f20 3229 2c0a 2020 2020 2020   1) / 2),.      
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2020 2020 2020 2020 2073 7461 745f             stat_
+0000a5a0: 7265 632c 0a20 2020 2020 2020 2020 2020  rec,.           
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2020 2020 6622 696e 7661 6c69 6420        f"invalid 
+0000a5d0: 7374 6174 2066 6f72 207b 6669 656c 646e  stat for {fieldn
+0000a5e0: 616d 657d 2229 0a0a 2020 2020 6465 6620  ame}")..    def 
+0000a5f0: 7465 7374 5f73 7461 7473 3228 7365 6c66  test_stats2(self
+0000a600: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000a610: 5f74 6573 745f 696e 6974 2829 0a20 2020  _test_init().   
+0000a620: 2020 2020 2066 6965 6c64 5f6e 616d 6573       field_names
+0000a630: 203d 2073 656c 662e 7431 2e69 6e66 6f28   = self.t1.info(
+0000a640: 295b 2266 6965 6c64 7322 5d0a 2020 2020  )["fields"].    
+0000a650: 2020 2020 6e75 6d5f 6669 656c 6473 203d      num_fields =
+0000a660: 206c 656e 2866 6965 6c64 5f6e 616d 6573   len(field_names
+0000a670: 290a 2020 2020 2020 2020 7431 5f73 7461  ).        t1_sta
+0000a680: 7473 203d 2073 656c 662e 7431 2e73 7461  ts = self.t1.sta
+0000a690: 7473 2862 795f 6669 656c 643d 4661 6c73  ts(by_field=Fals
+0000a6a0: 6529 0a20 2020 2020 2020 2066 6f72 2073  e).        for s
+0000a6b0: 7461 742c 2076 616c 7565 2069 6e20 2828  tat, value in ((
+0000a6c0: 276d 696e 272c 2030 292c 2028 276d 6178  'min', 0), ('max
+0000a6d0: 272c 2073 656c 662e 7465 7374 5f73 697a  ', self.test_siz
+0000a6e0: 6520 2d20 3129 2c20 2827 636f 756e 7427  e - 1), ('count'
+0000a6f0: 2c20 7365 6c66 2e74 6573 745f 7369 7a65  , self.test_size
+0000a700: 202a 2a20 6e75 6d5f 6669 656c 6473 292c   ** num_fields),
+0000a710: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000a720: 6f72 2066 6965 6c64 6e61 6d65 2069 6e20  or fieldname in 
+0000a730: 6669 656c 645f 6e61 6d65 733a 0a20 2020  field_names:.   
+0000a740: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000a750: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+0000a760: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
+0000a770: 7461 7422 2c20 7374 6174 3d73 7461 742c  tat", stat=stat,
+0000a780: 2066 6965 6c64 6e61 6d65 3d66 6965 6c64   fieldname=field
+0000a790: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+0000a7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a7b0: 6173 7365 7274 4571 7561 6c28 7661 6c75  assertEqual(valu
+0000a7c0: 652c 2067 6574 6174 7472 2874 315f 7374  e, getattr(t1_st
+0000a7d0: 6174 732e 6279 2e73 7461 745b 7374 6174  ats.by.stat[stat
+0000a7e0: 5d2c 2066 6965 6c64 6e61 6d65 292c 0a20  ], fieldname),. 
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 6622 696e 7661 6c69 6420 7b73 7461 747d  f"invalid {stat}
+0000a820: 2073 7461 7420 666f 7220 7b66 6965 6c64   stat for {field
+0000a830: 6e61 6d65 7d22 290a 0a20 2020 2064 6566  name}")..    def
+0000a840: 2074 6573 745f 7374 6174 7333 2873 656c   test_stats3(sel
+0000a850: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0000a860: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
+0000a870: 2020 2020 2020 6669 656c 645f 6e61 6d65        field_name
+0000a880: 7320 3d20 7365 6c66 2e74 312e 696e 666f  s = self.t1.info
+0000a890: 2829 5b22 6669 656c 6473 225d 0a20 2020  ()["fields"].   
+0000a8a0: 2020 2020 206e 756d 5f66 6965 6c64 7320       num_fields 
+0000a8b0: 3d20 6c65 6e28 6669 656c 645f 6e61 6d65  = len(field_name
+0000a8c0: 7329 0a0a 2020 2020 2020 2020 2320 7665  s)..        # ve
+0000a8d0: 7269 6679 2074 6861 7420 7374 6174 7320  rify that stats 
+0000a8e0: 6361 6e20 2273 7465 7020 6f76 6572 2220  can "step over" 
+0000a8f0: 6e6f 6e2d 6e75 6d65 7269 6320 6461 7461  non-numeric data
+0000a900: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000a910: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000a920: 315b 305d 2e61 203d 2022 6e6f 7420 6120  1[0].a = "not a 
+0000a930: 6e75 6d62 6572 220a 2020 2020 2020 2020  number".        
+0000a940: 6578 6365 7074 2028 4174 7472 6962 7574  except (Attribut
+0000a950: 6545 7272 6f72 2c20 5479 7065 4572 726f  eError, TypeErro
+0000a960: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000a970: 2320 736f 6d65 2074 6573 7420 7479 7065  # some test type
+0000a980: 7320 6172 656e 2774 206d 7574 6162 6c65  s aren't mutable
+0000a990: 2c20 6d75 7374 2072 6570 6c61 6365 2072  , must replace r
+0000a9a0: 6563 2077 6974 6820 6120 6d6f 6469 6669  ec with a modifi
+0000a9b0: 6564 206f 6e65 0a20 2020 2020 2020 2020  ed one.         
+0000a9c0: 2020 206d 6f64 5f72 6563 203d 2073 656c     mod_rec = sel
+0000a9d0: 662e 7431 2e70 6f70 2830 290a 2020 2020  f.t1.pop(0).    
+0000a9e0: 2020 2020 2020 2020 7265 635f 7479 7065          rec_type
+0000a9f0: 203d 2074 7970 6528 6d6f 645f 7265 6329   = type(mod_rec)
+0000aa00: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000aa10: 5f72 6563 5f64 6963 7420 3d20 6c74 2e5f  _rec_dict = lt._
+0000aa20: 746f 5f64 6963 7428 6d6f 645f 7265 6329  to_dict(mod_rec)
+0000aa30: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000aa40: 5f72 6563 5f64 6963 745b 2761 275d 203d  _rec_dict['a'] =
+0000aa50: 2022 6e6f 7420 6120 6e75 6d62 6572 220a   "not a number".
+0000aa60: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000aa70: 7265 6320 3d20 7265 635f 7479 7065 282a  rec = rec_type(*
+0000aa80: 2a6e 6577 5f72 6563 5f64 6963 7429 0a20  *new_rec_dict). 
+0000aa90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000aaa0: 7431 2e69 6e73 6572 7428 6e65 775f 7265  t1.insert(new_re
+0000aab0: 6329 0a0a 2020 2020 2020 2020 7431 5f73  c)..        t1_s
+0000aac0: 7461 7473 203d 2073 656c 662e 7431 2e73  tats = self.t1.s
+0000aad0: 7461 7473 2829 0a20 2020 2020 2020 2074  tats().        t
+0000aae0: 315f 7374 6174 7328 2274 315f 7374 6174  1_stats("t1_stat
+0000aaf0: 7322 290a 2020 2020 2020 2020 7431 5f73  s").        t1_s
+0000ab00: 7461 7473 2e63 7376 5f65 7870 6f72 7428  tats.csv_export(
+0000ab10: 7379 732e 7374 646f 7574 290a 2020 2020  sys.stdout).    
+0000ab20: 2020 2020 7431 5f73 7461 7473 2e70 7265      t1_stats.pre
+0000ab30: 7365 6e74 2829 0a20 2020 2020 2020 2073  sent().        s
+0000ab40: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000ab50: 7365 6c66 2e74 6573 745f 7369 7a65 202a  self.test_size *
+0000ab60: 2a20 6e75 6d5f 6669 656c 6473 202d 2031  * num_fields - 1
+0000ab70: 2c20 7431 5f73 7461 7473 2e62 792e 6e61  , t1_stats.by.na
+0000ab80: 6d65 5b22 6122 5d2e 636f 756e 7429 0a0a  me["a"].count)..
+0000ab90: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
+0000aba0: 7473 3428 7365 6c66 293a 0a20 2020 2020  ts4(self):.     
+0000abb0: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
+0000abc0: 2829 2e63 7376 5f69 6d70 6f72 7428 7465  ().csv_import(te
+0000abd0: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
+0000abe0: 225c 0a20 2020 2020 2020 2061 2c62 0a20  "\.        a,b. 
+0000abf0: 2020 2020 2020 2031 2c32 0a20 2020 2020         1,2.     
+0000ac00: 2020 2033 2c0a 2020 2020 2020 2020 352c     3,.        5,
+0000ac10: 340a 2020 2020 2020 2020 2222 2229 2c20  4.        """), 
+0000ac20: 7472 616e 7366 6f72 6d73 3d7b 7d2e 6672  transforms={}.fr
+0000ac30: 6f6d 6b65 7973 285b 2261 222c 2022 6222  omkeys(["a", "b"
+0000ac40: 5d2c 2069 6e74 2929 0a20 2020 2020 2020  ], int)).       
+0000ac50: 2074 315f 7374 6174 7320 3d20 7431 2e73   t1_stats = t1.s
+0000ac60: 7461 7473 2829 0a20 2020 2020 2020 2074  tats().        t
+0000ac70: 315f 7374 6174 732e 7072 6573 656e 7428  1_stats.present(
+0000ac80: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000ac90: 7431 5f73 7461 7473 2e69 6e66 6f28 2929  t1_stats.info())
+0000aca0: 0a0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
+0000acb0: 6564 203d 206c 742e 5461 626c 6528 292e  ed = lt.Table().
+0000acc0: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
+0000acd0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000ace0: 2020 2020 2020 2020 6e61 6d65 2c6d 6561          name,mea
+0000acf0: 6e2c 6d69 6e2c 6d61 782c 7661 7269 616e  n,min,max,varian
+0000ad00: 6365 2c73 7464 5f64 6576 2c63 6f75 6e74  ce,std_dev,count
+0000ad10: 2c6d 6973 7369 6e67 0a20 2020 2020 2020  ,missing.       
+0000ad20: 2061 2c33 2e30 2c31 2c35 2c34 2c32 2e30   a,3.0,1,5,4,2.0
+0000ad30: 2c33 2c30 0a20 2020 2020 2020 2062 2c33  ,3,0.        b,3
+0000ad40: 2e30 2c32 2c34 2c32 2c31 2e34 3134 2c32  .0,2,4,2,1.414,2
+0000ad50: 2c31 0a20 2020 2020 2020 2022 2222 292c  ,1.        """),
+0000ad60: 2074 7261 6e73 666f 726d 733d 7b7d 2e66   transforms={}.f
+0000ad70: 726f 6d6b 6579 7328 226d 6561 6e20 6d69  romkeys("mean mi
+0000ad80: 6e20 6d61 7820 7661 7269 616e 6365 2073  n max variance s
+0000ad90: 7464 5f64 6576 2063 6f75 6e74 206d 6973  td_dev count mis
+0000ada0: 7369 6e67 222e 7370 6c69 7428 292c 2061  sing".split(), a
+0000adb0: 7374 2e6c 6974 6572 616c 5f65 7661 6c29  st.literal_eval)
+0000adc0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+0000add0: 6564 2e70 7265 7365 6e74 2829 0a20 2020  ed.present().   
+0000ade0: 2020 2020 2070 7269 6e74 2865 7870 6563       print(expec
+0000adf0: 7465 642e 696e 666f 2829 290a 0a20 2020  ted.info())..   
+0000ae00: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000ae10: 7562 5465 7374 2822 6368 6563 6b20 636f  ubTest("check co
+0000ae20: 6d70 7574 6564 2073 7461 7420 6669 656c  mputed stat fiel
+0000ae30: 6473 2229 3a0a 2020 2020 2020 2020 2020  ds"):.          
+0000ae40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000ae50: 616c 2865 7870 6563 7465 642e 696e 666f  al(expected.info
+0000ae60: 2829 5b22 6669 656c 6473 225d 2c20 7431  ()["fields"], t1
+0000ae70: 5f73 7461 7473 2e69 6e66 6f28 295b 2266  _stats.info()["f
+0000ae80: 6965 6c64 7322 5d29 0a0a 2020 2020 2020  ields"])..      
+0000ae90: 2020 666f 7220 6578 7065 6374 6564 5f72    for expected_r
+0000aea0: 6f77 2c20 726f 7720 696e 207a 6970 2865  ow, row in zip(e
+0000aeb0: 7870 6563 7465 642c 2074 315f 7374 6174  xpected, t1_stat
+0000aec0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000aed0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000aee0: 7428 2263 6865 636b 2063 6f6d 7075 7465  t("check compute
+0000aef0: 6420 7374 6174 2061 7474 7269 6275 7465  d stat attribute
+0000af00: 2028 6e61 6d65 2922 2c20 726f 773d 726f   (name)", row=ro
+0000af10: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
+0000af20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000af30: 7175 616c 2865 7870 6563 7465 645f 726f  qual(expected_ro
+0000af40: 772e 6e61 6d65 2c20 726f 772e 6e61 6d65  w.name, row.name
+0000af50: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+0000af60: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000af70: 2263 6865 636b 2063 6f6d 7075 7465 6420  "check computed 
+0000af80: 7374 6174 2061 7474 7269 6275 7465 2028  stat attribute (
+0000af90: 6d65 616e 2922 2c20 726f 773d 726f 7729  mean)", row=row)
+0000afa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000afb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000afc0: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
+0000afd0: 6d65 616e 2c20 726f 772e 6d65 616e 290a  mean, row.mean).
+0000afe0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000aff0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+0000b000: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
+0000b010: 6174 2061 7474 7269 6275 7465 2028 6d69  at attribute (mi
+0000b020: 6e29 222c 2072 6f77 3d72 6f77 293a 0a20  n)", row=row):. 
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b040: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000b050: 6578 7065 6374 6564 5f72 6f77 2e6d 696e  expected_row.min
+0000b060: 2c20 726f 772e 6d69 6e29 0a20 2020 2020  , row.min).     
+0000b070: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000b080: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
+0000b090: 636f 6d70 7574 6564 2073 7461 7420 6174  computed stat at
+0000b0a0: 7472 6962 7574 6520 286d 6178 2922 2c20  tribute (max)", 
+0000b0b0: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
+0000b0c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000b0d0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000b0e0: 7465 645f 726f 772e 6d61 782c 2072 6f77  ted_row.max, row
+0000b0f0: 2e6d 6178 290a 2020 2020 2020 2020 2020  .max).          
+0000b100: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000b110: 6573 7428 2263 6865 636b 2063 6f6d 7075  est("check compu
+0000b120: 7465 6420 7374 6174 2061 7474 7269 6275  ted stat attribu
+0000b130: 7465 2028 7661 7269 616e 6365 2922 2c20  te (variance)", 
+0000b140: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
+0000b150: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000b160: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000b170: 7465 645f 726f 772e 7661 7269 616e 6365  ted_row.variance
+0000b180: 2c20 726f 772e 7661 7269 616e 6365 290a  , row.variance).
+0000b190: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000b1a0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+0000b1b0: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
+0000b1c0: 6174 2061 7474 7269 6275 7465 2028 7374  at attribute (st
+0000b1d0: 645f 6465 7629 222c 2072 6f77 3d72 6f77  d_dev)", row=row
+0000b1e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000b1f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000b200: 7561 6c28 6578 7065 6374 6564 5f72 6f77  ual(expected_row
+0000b210: 2e73 7464 5f64 6576 2c20 726f 772e 7374  .std_dev, row.st
+0000b220: 645f 6465 7629 0a20 2020 2020 2020 2020  d_dev).         
+0000b230: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b240: 5465 7374 2822 6368 6563 6b20 636f 6d70  Test("check comp
+0000b250: 7574 6564 2073 7461 7420 6174 7472 6962  uted stat attrib
+0000b260: 7574 6520 2863 6f75 6e74 2922 2c20 726f  ute (count)", ro
+0000b270: 773d 726f 7729 3a0a 2020 2020 2020 2020  w=row):.        
+0000b280: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000b290: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0000b2a0: 645f 726f 772e 636f 756e 742c 2072 6f77  d_row.count, row
+0000b2b0: 2e63 6f75 6e74 290a 2020 2020 2020 2020  .count).        
+0000b2c0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000b2d0: 6254 6573 7428 2263 6865 636b 2063 6f6d  bTest("check com
+0000b2e0: 7075 7465 6420 7374 6174 2061 7474 7269  puted stat attri
+0000b2f0: 6275 7465 2028 6d69 7373 696e 6729 222c  bute (missing)",
+0000b300: 2072 6f77 3d72 6f77 293a 0a20 2020 2020   row=row):.     
+0000b310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b320: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+0000b330: 6374 6564 5f72 6f77 2e6d 6973 7369 6e67  cted_row.missing
+0000b340: 2c20 726f 772e 6d69 7373 696e 6729 0a0a  , row.missing)..
+0000b350: 2020 2020 6465 6620 7465 7374 5f73 706c      def test_spl
+0000b360: 6974 6279 2873 656c 6629 3a0a 2020 2020  itby(self):.    
+0000b370: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+0000b380: 6e69 7428 290a 2020 2020 2020 2020 6973  nit().        is
+0000b390: 5f6f 6464 203d 206c 616d 6264 6120 7265  _odd = lambda re
+0000b3a0: 633a 2072 6563 2e61 2025 2032 0a20 2020  c: rec.a % 2.   
+0000b3b0: 2020 2020 2065 7665 6e73 2c20 6f64 6473       evens, odds
+0000b3c0: 203d 2073 656c 662e 7431 2e73 706c 6974   = self.t1.split
+0000b3d0: 6279 2869 735f 6f64 6429 0a20 2020 2020  by(is_odd).     
+0000b3e0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b3f0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000b400: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000b410: 7175 616c 286c 656e 286f 6464 7329 202b  qual(len(odds) +
+0000b420: 206c 656e 2865 7665 6e73 292c 206c 656e   len(evens), len
+0000b430: 2873 656c 662e 7431 2929 0a20 2020 2020  (self.t1)).     
+0000b440: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b450: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000b460: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000b470: 7175 616c 286c 656e 286f 6464 7329 2c20  qual(len(odds), 
+0000b480: 6c65 6e28 7365 6c66 2e74 312e 7768 6572  len(self.t1.wher
+0000b490: 6528 6973 5f6f 6464 2929 290a 0a20 2020  e(is_odd)))..   
+0000b4a0: 2020 2020 2065 7665 6e5f 6576 656e 732c       even_evens,
+0000b4b0: 206f 6464 5f65 7665 6e73 203d 2065 7665   odd_evens = eve
+0000b4c0: 6e73 2e73 706c 6974 6279 2869 735f 6f64  ns.splitby(is_od
+0000b4d0: 6429 0a20 2020 2020 2020 2077 6974 6820  d).        with 
+0000b4e0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000b4f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b500: 2e61 7373 6572 7445 7175 616c 2830 2c20  .assertEqual(0, 
+0000b510: 6c65 6e28 6f64 645f 6576 656e 7329 290a  len(odd_evens)).
+0000b520: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000b530: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+0000b540: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000b550: 7365 7274 4571 7561 6c28 6c65 6e28 6576  sertEqual(len(ev
+0000b560: 656e 5f65 7665 6e73 292c 206c 656e 2865  en_evens), len(e
+0000b570: 7665 6e73 2929 0a0a 2020 2020 2020 2020  vens))..        
+0000b580: 2320 6d61 6b65 2073 7572 6520 696e 6465  # make sure inde
+0000b590: 7865 7320 6172 6520 7072 6573 6572 7665  xes are preserve
+0000b5a0: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
+0000b5b0: 312e 6372 6561 7465 5f69 6e64 6578 2822  1.create_index("
+0000b5c0: 6122 290a 2020 2020 2020 2020 6576 656e  a").        even
+0000b5d0: 732c 206f 6464 7320 3d20 7365 6c66 2e74  s, odds = self.t
+0000b5e0: 312e 7370 6c69 7462 7928 6973 5f6f 6464  1.splitby(is_odd
+0000b5f0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000b600: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000b610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b620: 6173 7365 7274 4571 7561 6c28 7365 6c66  assertEqual(self
+0000b630: 2e74 312e 696e 666f 2829 5b22 696e 6465  .t1.info()["inde
+0000b640: 7865 7322 5d2c 2065 7665 6e73 2e69 6e66  xes"], evens.inf
+0000b650: 6f28 295b 2269 6e64 6578 6573 225d 290a  o()["indexes"]).
+0000b660: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
+0000b670: 7061 7373 696e 6720 616e 2061 7474 7269  passing an attri
+0000b680: 6275 7465 2061 7320 6120 6b65 790a 2020  bute as a key.  
+0000b690: 2020 2020 2020 7a65 726f 732c 206e 6f6e        zeros, non
+0000b6a0: 5f7a 6572 6f73 203d 2073 656c 662e 7431  _zeros = self.t1
+0000b6b0: 2e73 706c 6974 6279 2822 6122 290a 2020  .splitby("a").  
+0000b6c0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000b6d0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+0000b6e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000b6f0: 7274 5472 7565 2861 6c6c 2872 6563 2e61  rtTrue(all(rec.a
+0000b700: 203d 3d20 3020 666f 7220 7265 6320 696e   == 0 for rec in
+0000b710: 207a 6572 6f73 2929 0a20 2020 2020 2020   zeros)).       
+0000b720: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000b730: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000b740: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0000b750: 6528 616c 6c28 7265 632e 6120 213d 2030  e(all(rec.a != 0
+0000b760: 2066 6f72 2072 6563 2069 6e20 6e6f 6e5f   for rec in non_
+0000b770: 7a65 726f 7329 290a 0a20 2020 2020 2020  zeros))..       
+0000b780: 2023 2074 6573 7420 7573 696e 6720 7072   # test using pr
+0000b790: 6564 6963 6174 6520 7468 6174 2064 6f65  edicate that doe
+0000b7a0: 7320 6e6f 7420 616c 7761 7973 2072 6574  s not always ret
+0000b7b0: 7572 6e20 3020 6f72 2031 0a20 2020 2020  urn 0 or 1.     
+0000b7c0: 2020 2069 735f 6e6f 745f 6d75 6c74 6970     is_not_multip
+0000b7d0: 6c65 5f6f 665f 3320 3d20 6c61 6d62 6461  le_of_3 = lambda
+0000b7e0: 2072 6563 3a20 7265 632e 6120 2520 330a   rec: rec.a % 3.
+0000b7f0: 2020 2020 2020 2020 6d75 6c74 735f 6f66          mults_of
+0000b800: 5f33 2c20 6e6f 6e5f 6d75 6c74 735f 6f66  _3, non_mults_of
+0000b810: 5f33 203d 2073 656c 662e 7431 2e73 706c  _3 = self.t1.spl
+0000b820: 6974 6279 2869 735f 6e6f 745f 6d75 6c74  itby(is_not_mult
+0000b830: 6970 6c65 5f6f 665f 3329 0a20 2020 2020  iple_of_3).     
+0000b840: 2020 2070 7269 6e74 286c 6973 7428 6e6f     print(list(no
+0000b850: 6e5f 6d75 6c74 735f 6f66 5f33 2e61 6c6c  n_mults_of_3.all
+0000b860: 2e61 2929 0a20 2020 2020 2020 2070 7269  .a)).        pri
+0000b870: 6e74 286c 6973 7428 6d75 6c74 735f 6f66  nt(list(mults_of
+0000b880: 5f33 2e61 6c6c 2e61 2929 0a20 2020 2020  _3.all.a)).     
+0000b890: 2020 2023 2054 4f44 4f20 2d20 6164 6420     # TODO - add 
+0000b8a0: 6173 7365 7274 7320 6865 7265 0a0a 0a40  asserts here...@
+0000b8b0: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
+0000b8c0: 730a 636c 6173 7320 5461 626c 654a 6f69  s.class TableJoi
+0000b8d0: 6e54 6573 7473 3a0a 2020 2020 6465 6620  nTests:.    def 
+0000b8e0: 7465 7374 5f73 696d 706c 655f 6a6f 696e  test_simple_join
+0000b8f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000b900: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
+0000b910: 2020 2020 2020 2074 3120 3d20 6d61 6b65         t1 = make
+0000b920: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
+0000b930: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+0000b940: 742c 2074 6573 745f 7369 7a65 290a 2020  t, test_size).  
+0000b950: 2020 2020 2020 7431 2e63 7265 6174 655f        t1.create_
+0000b960: 696e 6465 7828 2761 2729 0a0a 2020 2020  index('a')..    
+0000b970: 2020 2020 7432 203d 206c 742e 5461 626c      t2 = lt.Tabl
+0000b980: 6528 290a 2020 2020 2020 2020 7432 2e63  e().        t2.c
+0000b990: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
+0000b9a0: 0a20 2020 2020 2020 2074 322e 696e 7365  .        t2.inse
+0000b9b0: 7274 286c 742e 4461 7461 4f62 6a65 6374  rt(lt.DataObject
+0000b9c0: 2861 3d31 2c20 643d 3130 3029 290a 0a20  (a=1, d=100)).. 
+0000b9d0: 2020 2020 2020 206a 6f69 6e65 6420 3d20         joined = 
+0000b9e0: 2874 312e 6a6f 696e 5f6f 6e28 2761 2729  (t1.join_on('a')
+0000b9f0: 202b 2074 322e 6a6f 696e 5f6f 6e28 2761   + t2.join_on('a
+0000ba00: 2729 2928 290a 2020 2020 2020 2020 7769  '))().        wi
+0000ba10: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000ba20: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000ba30: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000ba40: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+0000ba50: 5f73 697a 652c 206c 656e 286a 6f69 6e65  _size, len(joine
+0000ba60: 6429 290a 0a20 2020 2020 2020 206a 6f69  d))..        joi
+0000ba70: 6e65 6420 3d20 2874 312e 6a6f 696e 5f6f  ned = (t1.join_o
+0000ba80: 6e28 2761 2729 202b 2074 3229 2829 0a20  n('a') + t2)(). 
+0000ba90: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000baa0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000bab0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000bac0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+0000bad0: 7a65 202a 2074 6573 745f 7369 7a65 2c20  ze * test_size, 
+0000bae0: 6c65 6e28 6a6f 696e 6564 2929 0a0a 2020  len(joined))..  
+0000baf0: 2020 2020 2020 6a6f 696e 6564 203d 2028        joined = (
+0000bb00: 7431 202b 2074 322e 6a6f 696e 5f6f 6e28  t1 + t2.join_on(
+0000bb10: 2761 2729 2928 290a 2020 2020 2020 2020  'a'))().        
+0000bb20: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000bb30: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000bb40: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000bb50: 6c28 7465 7374 5f73 697a 6520 2a20 7465  l(test_size * te
+0000bb60: 7374 5f73 697a 652c 206c 656e 286a 6f69  st_size, len(joi
+0000bb70: 6e65 6429 290a 0a20 2020 2020 2020 2074  ned))..        t
+0000bb80: 312e 6465 6c65 7465 5f69 6e64 6578 2827  1.delete_index('
+0000bb90: 6127 290a 2020 2020 2020 2020 7769 7468  a').        with
+0000bba0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000bbb0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000bbc0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+0000bbd0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
+0000bbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bbf0: 206a 6f69 6e65 6420 3d20 2874 3120 2b20   joined = (t1 + 
+0000bc00: 7432 2e6a 6f69 6e5f 6f6e 2827 6127 2929  t2.join_on('a'))
+0000bc10: 2829 0a0a 2020 2020 2020 2020 7769 7468  ()..        with
+0000bc20: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000bc30: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000bc40: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+0000bc50: 7365 7328 5479 7065 4572 726f 7229 3a0a  ses(TypeError):.
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc70: 2320 696e 7661 6c69 6420 6a6f 696e 2c20  # invalid join, 
+0000bc80: 6e6f 206b 7761 7267 7320 6c69 7374 696e  no kwargs listin
+0000bc90: 6720 6174 7472 6962 7574 6573 2074 6f20  g attributes to 
+0000bca0: 6a6f 696e 206f 6e0a 2020 2020 2020 2020  join on.        
+0000bcb0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
+0000bcc0: 6a6f 696e 2874 322c 2027 612c 6427 290a  join(t2, 'a,d').
+0000bcd0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000bce0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000bcf0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000bd00: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+0000bd10: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000bd30: 696e 7661 6c69 6420 6a6f 696e 2c20 6e6f  invalid join, no
+0000bd40: 2073 7563 6820 6174 7472 6962 7574 6520   such attribute 
+0000bd50: 277a 270a 2020 2020 2020 2020 2020 2020  'z'.            
+0000bd60: 2020 2020 7433 203d 2074 312e 6a6f 696e      t3 = t1.join
+0000bd70: 2874 322c 2027 612c 642c 7a27 2c20 613d  (t2, 'a,d,z', a=
+0000bd80: 2761 2729 0a0a 2020 2020 2020 2020 7433  'a')..        t3
+0000bd90: 203d 2074 312e 6a6f 696e 2874 322c 2027   = t1.join(t2, '
+0000bda0: 612c 6427 2c20 613d 2761 2729 0a20 2020  a,d', a='a').   
+0000bdb0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000bdc0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000bdd0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000bde0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+0000bdf0: 202a 2074 6573 745f 7369 7a65 2c20 6c65   * test_size, le
+0000be00: 6e28 7433 2929 0a0a 2020 2020 2020 2020  n(t3))..        
+0000be10: 7434 203d 2074 312e 6a6f 696e 2874 322c  t4 = t1.join(t2,
+0000be20: 2061 3d27 6127 292e 7365 6c65 6374 2827   a='a').select('
+0000be30: 6120 6320 6427 2c20 653d 6c61 6d62 6461  a c d', e=lambda
+0000be40: 2072 6563 3a20 7265 632e 6120 2b20 7265   rec: rec.a + re
+0000be50: 632e 6320 2b20 7265 632e 6429 0a20 2020  c.c + rec.d).   
+0000be60: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000be70: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000be80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000be90: 7454 7275 6528 616c 6c28 7265 632e 6520  tTrue(all(rec.e 
+0000bea0: 3d3d 2072 6563 2e61 2b72 6563 2e63 2b72  == rec.a+rec.c+r
+0000beb0: 6563 2e64 2066 6f72 2072 6563 2069 6e20  ec.d for rec in 
+0000bec0: 7434 2929 0a0a 2020 2020 2020 2020 2320  t4))..        # 
+0000bed0: 6a6f 696e 2074 6f20 656d 7074 7920 6c69  join to empty li
+0000bee0: 7374 2c20 7368 6f75 6c64 2072 6574 7572  st, should retur
+0000bef0: 6e20 656d 7074 7920 7461 626c 650a 2020  n empty table.  
+0000bf00: 2020 2020 2020 656d 7074 795f 7461 626c        empty_tabl
+0000bf10: 6520 3d20 6c74 2e54 6162 6c65 2829 0a20  e = lt.Table(). 
+0000bf20: 2020 2020 2020 2065 6d70 7479 5f74 6162         empty_tab
+0000bf30: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
+0000bf40: 2761 2729 0a20 2020 2020 2020 2074 3520  'a').        t5 
+0000bf50: 3d20 2874 312e 6a6f 696e 5f6f 6e28 2761  = (t1.join_on('a
+0000bf60: 2729 202b 2065 6d70 7479 5f74 6162 6c65  ') + empty_table
+0000bf70: 2928 290a 2020 2020 2020 2020 7769 7468  )().        with
+0000bf80: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000bf90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000bfa0: 662e 6173 7365 7274 4571 7561 6c28 302c  f.assertEqual(0,
+0000bfb0: 206c 656e 2874 3529 290a 0a20 2020 2064   len(t5))..    d
+0000bfc0: 6566 2074 6573 745f 6f75 7465 725f 6a6f  ef test_outer_jo
+0000bfd0: 696e 7328 7365 6c66 293a 0a20 2020 2020  ins(self):.     
+0000bfe0: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
+0000bff0: 2822 6361 7461 6c6f 6722 290a 2020 2020  ("catalog").    
+0000c000: 2020 2020 7431 2e63 7376 5f69 6d70 6f72      t1.csv_impor
+0000c010: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
+0000c020: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
+0000c030: 2020 2073 6b75 2c63 6f6c 6f72 2c73 697a     sku,color,siz
+0000c040: 652c 6d61 7465 7269 616c 0a20 2020 2020  e,material.     
+0000c050: 2020 2020 2020 2030 3031 2c72 6564 2c58         001,red,X
+0000c060: 4c2c 636f 7474 6f6e 0a20 2020 2020 2020  L,cotton.       
+0000c070: 2020 2020 2030 3032 2c62 6c75 652c 584c       002,blue,XL
+0000c080: 2c63 6f74 746f 6e2f 706f 6c79 0a20 2020  ,cotton/poly.   
+0000c090: 2020 2020 2020 2020 2030 3033 2c62 6c75           003,blu
+0000c0a0: 652c 4c2c 6c69 6e65 6e0a 2020 2020 2020  e,L,linen.      
+0000c0b0: 2020 2020 2020 3030 342c 7265 642c 4d2c        004,red,M,
+0000c0c0: 636f 7474 6f6e 0a20 2020 2020 2020 2020  cotton.         
+0000c0d0: 2020 2022 2222 2929 0a0a 2020 2020 2020     """))..      
+0000c0e0: 2020 7432 203d 206c 742e 5461 626c 6528    t2 = lt.Table(
+0000c0f0: 2270 7269 6365 7322 290a 2020 2020 2020  "prices").      
+0000c100: 2020 7432 2e63 7376 5f69 6d70 6f72 7428    t2.csv_import(
+0000c110: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000c120: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000c130: 2073 6b75 2c75 6e69 745f 7072 6963 652c   sku,unit_price,
+0000c140: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+0000c150: 2030 3031 2c31 302c 4c0a 2020 2020 2020   001,10,L.      
+0000c160: 2020 2020 2020 3030 312c 3132 2c58 4c0a        001,12,XL.
+0000c170: 2020 2020 2020 2020 2020 2020 3030 322c              002,
+0000c180: 3131 2c0a 2020 2020 2020 2020 2020 2020  11,.            
+0000c190: 3030 342c 392c 0a20 2020 2020 2020 2020  004,9,.         
+0000c1a0: 2020 2022 2222 292c 2074 7261 6e73 666f     """), transfo
+0000c1b0: 726d 733d 7b27 7369 7a65 273a 206c 616d  rms={'size': lam
+0000c1c0: 6264 6120 783a 2078 206f 7220 4e6f 6e65  bda x: x or None
+0000c1d0: 7d29 0a20 2020 2020 2020 2070 7269 6e74  }).        print
+0000c1e0: 2874 312e 696e 666f 2829 290a 0a20 2020  (t1.info())..   
+0000c1f0: 2020 2020 2074 312e 7072 6573 656e 7428       t1.present(
+0000c200: 290a 2020 2020 2020 2020 7432 2e70 7265  ).        t2.pre
+0000c210: 7365 6e74 2829 0a0a 2020 2020 2020 2020  sent()..        
+0000c220: 7433 203d 2074 312e 6a6f 696e 2874 322c  t3 = t1.join(t2,
+0000c230: 2061 7574 6f5f 6372 6561 7465 5f69 6e64   auto_create_ind
+0000c240: 6578 6573 3d54 7275 652c 2073 6b75 3d22  exes=True, sku="
+0000c250: 736b 7522 290a 2020 2020 2020 2020 7072  sku").        pr
+0000c260: 696e 7428 7433 2e69 6e66 6f28 2929 0a20  int(t3.info()). 
+0000c270: 2020 2020 2020 2074 332e 7072 6573 656e         t3.presen
+0000c280: 7428 290a 2020 2020 2020 2020 7769 7468  t().        with
+0000c290: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000c2a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c2b0: 662e 6173 7365 7274 4571 7561 6c28 342c  f.assertEqual(4,
+0000c2c0: 206c 656e 2874 3329 290a 0a20 2020 2020   len(t3))..     
+0000c2d0: 2020 2074 3320 3d20 7431 2e6a 6f69 6e28     t3 = t1.join(
+0000c2e0: 7432 2c20 6175 746f 5f63 7265 6174 655f  t2, auto_create_
+0000c2f0: 696e 6465 7865 733d 5472 7565 2c20 736b  indexes=True, sk
+0000c300: 753d 2273 6b75 222c 2073 697a 653d 2273  u="sku", size="s
+0000c310: 697a 6522 290a 2020 2020 2020 2020 7433  ize").        t3
+0000c320: 2822 696e 6e65 7220 6a6f 696e 202d 2022  ("inner join - "
+0000c330: 202b 2074 332e 7461 626c 655f 6e61 6d65   + t3.table_name
+0000c340: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000c350: 7433 2e69 6e66 6f28 2929 0a20 2020 2020  t3.info()).     
+0000c360: 2020 2074 332e 7072 6573 656e 7428 290a     t3.present().
+0000c370: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000c380: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+0000c390: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000c3a0: 7365 7274 4571 7561 6c28 312c 206c 656e  sertEqual(1, len
+0000c3b0: 2874 3329 290a 0a20 2020 2020 2020 2074  (t3))..        t
+0000c3c0: 3320 3d20 7431 2e6f 7574 6572 5f6a 6f69  3 = t1.outer_joi
+0000c3d0: 6e28 6c74 2e54 6162 6c65 2e52 4947 4854  n(lt.Table.RIGHT
+0000c3e0: 5f4f 5554 4552 5f4a 4f49 4e2c 2074 322c  _OUTER_JOIN, t2,
+0000c3f0: 2073 6b75 3d22 736b 7522 2c20 7369 7a65   sku="sku", size
+0000c400: 3d22 7369 7a65 2229 0a20 2020 2020 2020  ="size").       
+0000c410: 2074 3328 2272 6967 6874 206f 7574 6572   t3("right outer
+0000c420: 206a 6f69 6e20 2d20 2220 2b20 7433 2e74   join - " + t3.t
+0000c430: 6162 6c65 5f6e 616d 6529 0a20 2020 2020  able_name).     
+0000c440: 2020 2070 7269 6e74 2874 332e 696e 666f     print(t3.info
+0000c450: 2829 290a 2020 2020 2020 2020 7433 2e70  ()).        t3.p
+0000c460: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
+0000c470: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000c480: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000c490: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000c4a0: 616c 2834 2c20 6c65 6e28 7433 2929 0a0a  al(4, len(t3))..
+0000c4b0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
+0000c4c0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
+0000c4d0: 626c 652e 4c45 4654 5f4f 5554 4552 5f4a  ble.LEFT_OUTER_J
+0000c4e0: 4f49 4e2c 2074 322c 2073 6b75 3d22 736b  OIN, t2, sku="sk
+0000c4f0: 7522 2c20 7369 7a65 3d22 7369 7a65 2229  u", size="size")
+0000c500: 0a20 2020 2020 2020 2074 3328 226c 6566  .        t3("lef
+0000c510: 7420 6f75 7465 7220 6a6f 696e 202d 2022  t outer join - "
+0000c520: 202b 2074 332e 7461 626c 655f 6e61 6d65   + t3.table_name
+0000c530: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000c540: 7433 2e69 6e66 6f28 2929 0a20 2020 2020  t3.info()).     
+0000c550: 2020 2074 332e 7072 6573 656e 7428 290a     t3.present().
+0000c560: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000c570: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+0000c580: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000c590: 7365 7274 4571 7561 6c28 322c 206c 656e  sertEqual(2, len
+0000c5a0: 2874 3329 290a 0a20 2020 2020 2020 2074  (t3))..        t
+0000c5b0: 3320 3d20 7431 2e6f 7574 6572 5f6a 6f69  3 = t1.outer_joi
+0000c5c0: 6e28 6c74 2e54 6162 6c65 2e46 554c 4c5f  n(lt.Table.FULL_
+0000c5d0: 4f55 5445 525f 4a4f 494e 2c20 7432 2c20  OUTER_JOIN, t2, 
+0000c5e0: 736b 753d 2273 6b75 222c 2073 697a 653d  sku="sku", size=
+0000c5f0: 2273 697a 6522 290a 2020 2020 2020 2020  "size").        
+0000c600: 7433 2822 6675 6c6c 206f 7574 6572 206a  t3("full outer j
+0000c610: 6f69 6e20 2d20 2220 2b20 7433 2e74 6162  oin - " + t3.tab
+0000c620: 6c65 5f6e 616d 6529 0a20 2020 2020 2020  le_name).       
+0000c630: 2070 7269 6e74 2874 332e 696e 666f 2829   print(t3.info()
+0000c640: 290a 2020 2020 2020 2020 7433 2e70 7265  ).        t3.pre
+0000c650: 7365 6e74 2829 0a20 2020 2020 2020 2077  sent().        w
+0000c660: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000c670: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000c680: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000c690: 2831 322c 206c 656e 2874 3329 290a 0a20  (12, len(t3)).. 
+0000c6a0: 2020 2064 6566 2074 6573 745f 6f75 7465     def test_oute
+0000c6b0: 725f 6a6f 696e 5f65 7861 6d70 6c65 2873  r_join_example(s
+0000c6c0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+0000c6d0: 6465 6669 6e65 2073 7475 6465 6e74 2061  define student a
+0000c6e0: 6e64 2072 6567 6973 7472 6174 696f 6e20  nd registration 
+0000c6f0: 6461 7461 0a20 2020 2020 2020 2073 7475  data.        stu
+0000c700: 6465 6e74 7320 3d20 6c74 2e54 6162 6c65  dents = lt.Table
+0000c710: 2822 7374 7564 656e 7473 2229 2e63 7376  ("students").csv
+0000c720: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
+0000c730: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000c740: 2020 2020 2020 2020 2073 7475 6465 6e74           student
+0000c750: 5f69 642c 6e61 6d65 0a20 2020 2020 2020  _id,name.       
+0000c760: 2020 2020 2030 3030 312c 416c 6963 650a       0001,Alice.
+0000c770: 2020 2020 2020 2020 2020 2020 3030 3032              0002
+0000c780: 2c42 6f62 0a20 2020 2020 2020 2020 2020  ,Bob.           
+0000c790: 2030 3030 332c 4368 6172 6c69 650a 2020   0003,Charlie.  
+0000c7a0: 2020 2020 2020 2020 2020 3030 3034 2c44            0004,D
+0000c7b0: 6176 650a 2020 2020 2020 2020 2020 2020  ave.            
+0000c7c0: 3030 3035 2c45 6e69 640a 2020 2020 2020  0005,Enid.      
+0000c7d0: 2020 2020 2020 2222 2229 290a 0a20 2020        """))..   
+0000c7e0: 2020 2020 2072 6567 6973 7472 6174 696f       registratio
+0000c7f0: 6e73 203d 206c 742e 5461 626c 6528 2272  ns = lt.Table("r
+0000c800: 6567 6973 7472 6174 696f 6e73 2229 2e63  egistrations").c
+0000c810: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
+0000c820: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+0000c830: 2020 2020 2020 2020 2020 2073 7475 6465             stude
+0000c840: 6e74 5f69 642c 636f 7572 7365 0a20 2020  nt_id,course.   
+0000c850: 2020 2020 2020 2020 2030 3030 312c 5053           0001,PS
+0000c860: 5943 4831 3031 0a20 2020 2020 2020 2020  YCH101.         
+0000c870: 2020 2030 3030 312c 4341 4c43 310a 2020     0001,CALC1.  
+0000c880: 2020 2020 2020 2020 2020 3030 3033 2c42            0003,B
+0000c890: 494f 3230 300a 2020 2020 2020 2020 2020  IO200.          
+0000c8a0: 2020 3030 3035 2c43 4845 4d31 3031 0a20    0005,CHEM101. 
+0000c8b0: 2020 2020 2020 2020 2020 2030 3030 362c             0006,
+0000c8c0: 5048 5931 3031 0a20 2020 2020 2020 2020  PHY101.         
+0000c8d0: 2020 2022 2222 2929 0a0a 2020 2020 2020     """))..      
+0000c8e0: 2020 636f 7572 7365 7320 3d20 6c74 2e54    courses = lt.T
+0000c8f0: 6162 6c65 2822 636f 7572 7365 7322 292e  able("courses").
+0000c900: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
+0000c910: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000c920: 2020 2020 2020 2020 2020 2020 636f 7572              cour
+0000c930: 7365 0a20 2020 2020 2020 2020 2020 2042  se.            B
+0000c940: 494f 3230 300a 2020 2020 2020 2020 2020  IO200.          
+0000c950: 2020 4341 4c43 310a 2020 2020 2020 2020    CALC1.        
+0000c960: 2020 2020 4348 454d 3130 310a 2020 2020      CHEM101.    
+0000c970: 2020 2020 2020 2020 5053 5943 4831 3031          PSYCH101
+0000c980: 0a20 2020 2020 2020 2020 2020 2050 4531  .            PE1
+0000c990: 3031 0a20 2020 2020 2020 2020 2020 2022  01.            "
+0000c9a0: 2222 2929 0a0a 2020 2020 2020 2020 2320  ""))..        # 
+0000c9b0: 7065 7266 6f72 6d20 6f75 7465 7220 6a6f  perform outer jo
+0000c9c0: 696e 2061 6e64 2073 686f 7720 7265 7375  in and show resu
+0000c9d0: 6c74 733a 0a20 2020 2020 2020 206e 6f6e  lts:.        non
+0000c9e0: 5f72 6567 203d 2073 7475 6465 6e74 732e  _reg = students.
+0000c9f0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
+0000ca00: 626c 652e 5249 4748 545f 4f55 5445 525f  ble.RIGHT_OUTER_
+0000ca10: 4a4f 494e 2c0a 2020 2020 2020 2020 2020  JOIN,.          
 0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2072 6567 6973 7472 6174 696f 6e73 2c0a   registrations,.
+0000ca30: 2020 2020 2020 2020 2020 2020 7265 6769              regi
+0000ca40: 7374 7261 7469 6f6e 732c 0a20 2020 2020  strations,.     
 0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 2020 2020 7374 7564 656e 745f 6964        student_id
-0000ca80: 3d22 7374 7564 656e 745f 6964 2229 2e77  ="student_id").w
-0000ca90: 6865 7265 286c 616d 6264 6120 7265 633a  here(lambda rec:
-0000caa0: 2072 6563 2e63 6f75 7273 6520 6973 204e   rec.course is N
-0000cab0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 2020 2020 206f 7220 7265 632e 6e61 6d65       or rec.name
-0000cb10: 2069 7320 4e6f 6e65 290a 2020 2020 2020   is None).      
-0000cb20: 2020 6675 6c6c 2e70 7265 7365 6e74 2829    full.present()
-0000cb30: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
-0000cb40: 6f72 7465 6428 6675 6c6c 2e61 6c6c 2e73  orted(full.all.s
-0000cb50: 7475 6465 6e74 5f69 6429 290a 2020 2020  tudent_id)).    
-0000cb60: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000cb70: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000cb80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000cb90: 4571 7561 6c28 5b27 3030 3032 272c 2027  Equal(['0002', '
-0000cba0: 3030 3034 272c 2027 3030 3036 275d 2c20  0004', '0006'], 
-0000cbb0: 736f 7274 6564 2866 756c 6c2e 616c 6c2e  sorted(full.all.
-0000cbc0: 7374 7564 656e 745f 6964 2929 0a0a 0a40  student_id))...@
-0000cbd0: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
-0000cbe0: 730a 636c 6173 7320 5461 626c 6554 7261  s.class TableTra
-0000cbf0: 6e73 666f 726d 5465 7374 733a 0a20 2020  nsformTests:.   
-0000cc00: 2064 6566 2074 6573 745f 736f 7274 2873   def test_sort(s
-0000cc10: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
-0000cc20: 7374 5f73 697a 6520 3d20 3130 0a20 2020  st_size = 10.   
-0000cc30: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
-0000cc40: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-0000cc50: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-0000cc60: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-0000cc70: 2020 2020 2063 5f67 726f 7570 7320 3d20       c_groups = 
-0000cc80: 300a 2020 2020 2020 2020 666f 7220 635f  0.        for c_
-0000cc90: 7661 6c75 652c 2072 6563 7320 696e 2069  value, recs in i
-0000cca0: 7465 7274 6f6f 6c73 2e67 726f 7570 6279  tertools.groupby
-0000ccb0: 2874 312c 206b 6579 3d6c 616d 6264 6120  (t1, key=lambda 
-0000ccc0: 7265 633a 2072 6563 2e63 293a 0a20 2020  rec: rec.c):.   
-0000ccd0: 2020 2020 2020 2020 2063 5f67 726f 7570           c_group
-0000cce0: 7320 2b3d 2031 0a20 2020 2020 2020 2020  s += 1.         
-0000ccf0: 2020 206c 6973 7428 7265 6373 290a 2020     list(recs).  
-0000cd00: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000cd10: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000cd20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000cd30: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-0000cd40: 6520 2a20 7465 7374 5f73 697a 6520 2a20  e * test_size * 
-0000cd50: 7465 7374 5f73 697a 652c 2063 5f67 726f  test_size, c_gro
-0000cd60: 7570 7329 0a0a 2020 2020 2020 2020 7431  ups)..        t1
-0000cd70: 2e73 6f72 7428 2763 2729 0a20 2020 2020  .sort('c').     
-0000cd80: 2020 2063 5f67 726f 7570 7320 3d20 300a     c_groups = 0.
-0000cd90: 2020 2020 2020 2020 666f 7220 635f 7661          for c_va
-0000cda0: 6c75 652c 2072 6563 7320 696e 2069 7465  lue, recs in ite
-0000cdb0: 7274 6f6f 6c73 2e67 726f 7570 6279 2874  rtools.groupby(t
-0000cdc0: 312c 206b 6579 3d6c 616d 6264 6120 7265  1, key=lambda re
-0000cdd0: 633a 2072 6563 2e63 293a 0a20 2020 2020  c: rec.c):.     
-0000cde0: 2020 2020 2020 2063 5f67 726f 7570 7320         c_groups 
-0000cdf0: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
-0000ce00: 206c 6973 7428 7265 6373 290a 2020 2020   list(recs).    
-0000ce10: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000ce20: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000ce30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ce40: 4571 7561 6c28 7465 7374 5f73 697a 652c  Equal(test_size,
-0000ce50: 2063 5f67 726f 7570 7329 0a20 2020 2020   c_groups).     
-0000ce60: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000ce70: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000ce80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000ce90: 7175 616c 2830 2c20 7431 5b30 5d2e 6329  qual(0, t1[0].c)
-0000cea0: 0a0a 2020 2020 2020 2020 7431 2e73 6f72  ..        t1.sor
-0000ceb0: 7428 2763 2064 6573 6327 290a 2020 2020  t('c desc').    
-0000cec0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000ced0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000cee0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000cef0: 4571 7561 6c28 7465 7374 5f73 697a 652d  Equal(test_size-
-0000cf00: 312c 2074 315b 305d 2e63 290a 0a20 2020  1, t1[0].c)..   
-0000cf10: 2064 6566 2074 6573 745f 736f 7274 3228   def test_sort2(
-0000cf20: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-0000cf30: 726f 775f 7479 7065 203d 2074 7970 6528  row_type = type(
-0000cf40: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-0000cf50: 626a 6563 7428 302c 302c 3029 290a 2020  bject(0,0,0)).  
-0000cf60: 2020 2020 2020 7474 203d 206c 742e 5461        tt = lt.Ta
-0000cf70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000cf80: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000cf90: 2822 2222 5c0a 2020 2020 2020 2020 612c  ("""\.        a,
-0000cfa0: 632c 620a 2020 2020 2020 2020 312c 322c  c,b.        1,2,
-0000cfb0: 310a 2020 2020 2020 2020 322c 332c 300a  1.        2,3,0.
-0000cfc0: 2020 2020 2020 2020 352c 352c 2d31 0a20          5,5,-1. 
-0000cfd0: 2020 2020 2020 2033 2c34 2c2d 310a 2020         3,4,-1.  
-0000cfe0: 2020 2020 2020 322c 342c 2d33 2222 2229        2,4,-3""")
-0000cff0: 2c20 726f 775f 636c 6173 733d 726f 775f  , row_class=row_
-0000d000: 7479 7065 2c20 7472 616e 7366 6f72 6d73  type, transforms
-0000d010: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-0000d020: 6120 6220 6322 2e73 706c 6974 2829 2c20  a b c".split(), 
-0000d030: 696e 7429 290a 0a20 2020 2020 2020 2064  int))..        d
-0000d040: 6566 2074 6f5f 7475 706c 6573 2874 293a  ef to_tuples(t):
-0000d050: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d060: 7572 6e20 6c69 7374 286d 6170 2861 7474  urn list(map(att
-0000d070: 7267 6574 7465 7228 2a74 2e69 6e66 6f28  rgetter(*t.info(
-0000d080: 295b 2766 6965 6c64 7327 5d29 2c20 7429  )['fields']), t)
-0000d090: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-0000d0a0: 2874 742e 696e 666f 2829 5b27 6669 656c  (tt.info()['fiel
-0000d0b0: 6473 275d 290a 0a20 2020 2020 2020 2073  ds'])..        s
-0000d0c0: 6f72 745f 6172 6720 3d20 2263 2062 222e  ort_arg = "c b".
-0000d0d0: 7370 6c69 7428 290a 2020 2020 2020 2020  split().        
-0000d0e0: 7072 696e 7428 6622 536f 7274 696e 6720  print(f"Sorting 
-0000d0f0: 6279 207b 736f 7274 5f61 7267 2172 7d22  by {sort_arg!r}"
-0000d100: 290a 2020 2020 2020 2020 7474 2e73 6875  ).        tt.shu
-0000d110: 6666 6c65 2829 0a20 2020 2020 2020 2074  ffle().        t
-0000d120: 742e 736f 7274 2873 6f72 745f 6172 6729  t.sort(sort_arg)
-0000d130: 0a20 2020 2020 2020 2074 315f 7475 706c  .        t1_tupl
-0000d140: 6573 203d 2074 6f5f 7475 706c 6573 2874  es = to_tuples(t
-0000d150: 7429 0a20 2020 2020 2020 2066 6f72 2074  t).        for t
-0000d160: 2069 6e20 7431 5f74 7570 6c65 733a 0a20   in t1_tuples:. 
-0000d170: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000d180: 2874 290a 2020 2020 2020 2020 7072 696e  (t).        prin
-0000d190: 7428 290a 0a20 2020 2020 2020 2074 742e  t()..        tt.
-0000d1a0: 7368 7566 666c 6528 290a 2020 2020 2020  shuffle().      
-0000d1b0: 2020 7474 2e73 6f72 7428 2262 2229 0a20    tt.sort("b"). 
-0000d1c0: 2020 2020 2020 2074 742e 736f 7274 2822         tt.sort("
-0000d1d0: 6322 290a 2020 2020 2020 2020 7432 5f74  c").        t2_t
-0000d1e0: 7570 6c65 7320 3d20 746f 5f74 7570 6c65  uples = to_tuple
-0000d1f0: 7328 7474 290a 2020 2020 2020 2020 666f  s(tt).        fo
-0000d200: 7220 7420 696e 2074 325f 7475 706c 6573  r t in t2_tuples
-0000d210: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0000d220: 696e 7428 7429 0a20 2020 2020 2020 2070  int(t).        p
-0000d230: 7269 6e74 2829 0a0a 2020 2020 2020 2020  rint()..        
-0000d240: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000d250: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000d260: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000d270: 6c28 7431 5f74 7570 6c65 732c 2074 325f  l(t1_tuples, t2_
-0000d280: 7475 706c 6573 2c20 2266 6169 6c65 6420  tuples, "failed 
-0000d290: 6d75 6c74 692d 6174 7472 6962 7574 6520  multi-attribute 
-0000d2a0: 736f 7274 2c20 6769 7665 6e20 6c69 7374  sort, given list
-0000d2b0: 206f 6620 6174 7472 6962 7574 6573 2229   of attributes")
-0000d2c0: 0a0a 2020 2020 2020 2020 736f 7274 5f61  ..        sort_a
-0000d2d0: 7267 203d 2022 632c 6222 0a20 2020 2020  rg = "c,b".     
-0000d2e0: 2020 2070 7269 6e74 2866 2253 6f72 7469     print(f"Sorti
-0000d2f0: 6e67 2062 7920 7b73 6f72 745f 6172 6721  ng by {sort_arg!
-0000d300: 727d 2229 0a20 2020 2020 2020 2074 742e  r}").        tt.
-0000d310: 7368 7566 666c 6528 290a 2020 2020 2020  shuffle().      
-0000d320: 2020 7474 2e73 6f72 7428 736f 7274 5f61    tt.sort(sort_a
-0000d330: 7267 290a 2020 2020 2020 2020 7431 5f74  rg).        t1_t
-0000d340: 7570 6c65 7320 3d20 746f 5f74 7570 6c65  uples = to_tuple
-0000d350: 7328 7474 290a 2020 2020 2020 2020 666f  s(tt).        fo
-0000d360: 7220 7420 696e 2074 315f 7475 706c 6573  r t in t1_tuples
-0000d370: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0000d380: 696e 7428 7429 0a20 2020 2020 2020 2070  int(t).        p
-0000d390: 7269 6e74 2829 0a0a 2020 2020 2020 2020  rint()..        
-0000d3a0: 7474 2e73 6875 6666 6c65 2829 0a20 2020  tt.shuffle().   
-0000d3b0: 2020 2020 2074 742e 736f 7274 2822 6222       tt.sort("b"
-0000d3c0: 290a 2020 2020 2020 2020 7474 2e73 6f72  ).        tt.sor
-0000d3d0: 7428 2263 2229 0a20 2020 2020 2020 2074  t("c").        t
-0000d3e0: 325f 7475 706c 6573 203d 2074 6f5f 7475  2_tuples = to_tu
-0000d3f0: 706c 6573 2874 7429 0a20 2020 2020 2020  ples(tt).       
-0000d400: 2066 6f72 2074 2069 6e20 7432 5f74 7570   for t in t2_tup
-0000d410: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-0000d420: 2070 7269 6e74 2874 290a 2020 2020 2020   print(t).      
-0000d430: 2020 7072 696e 7428 290a 0a20 2020 2020    print()..     
-0000d440: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000d450: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000d460: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000d470: 7175 616c 2874 315f 7475 706c 6573 2c20  qual(t1_tuples, 
-0000d480: 7432 5f74 7570 6c65 732c 2022 6661 696c  t2_tuples, "fail
-0000d490: 6564 206d 756c 7469 2d61 7474 7269 6275  ed multi-attribu
-0000d4a0: 7465 2073 6f72 742c 2067 6976 656e 2063  te sort, given c
-0000d4b0: 6f6d 6d61 2d73 6570 6172 6174 6564 2061  omma-separated a
-0000d4c0: 7474 7269 6275 7465 7320 7374 7269 6e67  ttributes string
-0000d4d0: 2229 0a0a 2020 2020 2020 2020 736f 7274  ")..        sort
-0000d4e0: 5f61 7267 203d 2022 632c 6220 6465 7363  _arg = "c,b desc
-0000d4f0: 220a 2020 2020 2020 2020 7072 696e 7428  ".        print(
-0000d500: 6622 536f 7274 696e 6720 6279 207b 736f  f"Sorting by {so
-0000d510: 7274 5f61 7267 2172 7d22 290a 2020 2020  rt_arg!r}").    
-0000d520: 2020 2020 7474 2e73 6875 6666 6c65 2829      tt.shuffle()
-0000d530: 0a20 2020 2020 2020 2074 742e 736f 7274  .        tt.sort
-0000d540: 2873 6f72 745f 6172 6729 0a20 2020 2020  (sort_arg).     
-0000d550: 2020 2074 315f 7475 706c 6573 203d 2074     t1_tuples = t
-0000d560: 6f5f 7475 706c 6573 2874 7429 0a20 2020  o_tuples(tt).   
-0000d570: 2020 2020 2066 6f72 2074 2069 6e20 7431       for t in t1
-0000d580: 5f74 7570 6c65 733a 0a20 2020 2020 2020  _tuples:.       
-0000d590: 2020 2020 2070 7269 6e74 2874 290a 2020       print(t).  
-0000d5a0: 2020 2020 2020 7072 696e 7428 290a 0a20        print().. 
-0000d5b0: 2020 2020 2020 2074 742e 7368 7566 666c         tt.shuffl
-0000d5c0: 6528 290a 2020 2020 2020 2020 7474 2e73  e().        tt.s
-0000d5d0: 6f72 7428 2262 2064 6573 6322 290a 2020  ort("b desc").  
-0000d5e0: 2020 2020 2020 7474 2e73 6f72 7428 2263        tt.sort("c
-0000d5f0: 2229 0a20 2020 2020 2020 2074 325f 7475  ").        t2_tu
-0000d600: 706c 6573 203d 2074 6f5f 7475 706c 6573  ples = to_tuples
-0000d610: 2874 7429 0a20 2020 2020 2020 2066 6f72  (tt).        for
-0000d620: 2074 2069 6e20 7432 5f74 7570 6c65 733a   t in t2_tuples:
-0000d630: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000d640: 6e74 2874 290a 2020 2020 2020 2020 7072  nt(t).        pr
-0000d650: 696e 7428 290a 0a20 2020 2020 2020 2077  int()..        w
-0000d660: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000d670: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000d680: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000d690: 2874 315f 7475 706c 6573 2c20 7432 5f74  (t1_tuples, t2_t
-0000d6a0: 7570 6c65 732c 2022 6661 696c 6564 206d  uples, "failed m
-0000d6b0: 6978 6564 2061 7363 656e 6469 6e67 2f64  ixed ascending/d
-0000d6c0: 6573 6365 6e64 696e 6720 6d75 6c74 692d  escending multi-
-0000d6d0: 6174 7472 6962 7574 6520 736f 7274 2229  attribute sort")
-0000d6e0: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
-0000d6f0: 6f72 7433 2873 656c 6629 3a0a 2020 2020  ort3(self):.    
-0000d700: 2020 2020 656d 706c 6f79 6565 7320 3d20      employees = 
-0000d710: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-0000d720: 6d70 6f72 7428 7465 7874 7772 6170 2e64  mport(textwrap.d
-0000d730: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
-0000d740: 2020 2020 2020 2065 6d70 5f69 642c 6e61         emp_id,na
-0000d750: 6d65 2c64 6570 742c 7361 6c61 7279 2c63  me,dept,salary,c
-0000d760: 6f6d 6d69 7373 696f 6e0a 2020 2020 2020  ommission.      
-0000d770: 2020 2020 2020 3030 3031 2c41 6c69 6365        0001,Alice
-0000d780: 2c53 616c 6573 2c35 3030 3030 2c30 2e35  ,Sales,50000,0.5
-0000d790: 0a20 2020 2020 2020 2020 2020 2030 3030  .            000
-0000d7a0: 322c 426f 622c 456e 6769 6e65 6572 696e  2,Bob,Engineerin
-0000d7b0: 672c 3130 3030 3030 2c0a 2020 2020 2020  g,100000,.      
-0000d7c0: 2020 2020 2020 3030 3033 2c43 6861 726c        0003,Charl
-0000d7d0: 6573 2c53 616c 6573 2c34 3530 3030 2c30  es,Sales,45000,0
-0000d7e0: 2e37 0a20 2020 2020 2020 2020 2020 2030  .7.            0
-0000d7f0: 3030 342c 4461 7665 2c53 616c 6573 2c34  004,Dave,Sales,4
-0000d800: 3530 3030 2c30 2e36 0a20 2020 2020 2020  5000,0.6.       
-0000d810: 2020 2020 2030 3030 352c 456d 696c 792c       0005,Emily,
-0000d820: 5361 6c65 732c 3530 3030 302c 302e 340a  Sales,50000,0.4.
-0000d830: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000d840: 2c20 7472 616e 7366 6f72 6d73 3d7b 2273  , transforms={"s
-0000d850: 616c 6172 7922 3a20 696e 742c 2022 636f  alary": int, "co
-0000d860: 6d6d 6973 7369 6f6e 223a 2066 6c6f 6174  mmission": float
-0000d870: 7d29 0a0a 2020 2020 2020 2020 7361 6c65  })..        sale
-0000d880: 735f 656d 706c 6f79 6565 7320 3d20 656d  s_employees = em
-0000d890: 706c 6f79 6565 732e 7768 6572 6528 6465  ployees.where(de
-0000d8a0: 7074 3d22 5361 6c65 7322 292e 736f 7274  pt="Sales").sort
-0000d8b0: 2822 7361 6c61 7279 2064 6573 632c 636f  ("salary desc,co
-0000d8c0: 6d6d 6973 7369 6f6e 2229 0a0a 2020 2020  mmission")..    
-0000d8d0: 2020 2020 7361 6c65 735f 656d 706c 6f79      sales_employ
-0000d8e0: 6565 732e 7072 6573 656e 7428 290a 2020  ees.present().  
-0000d8f0: 2020 2020 2020 7072 696e 7428 6c69 7374        print(list
-0000d900: 2873 616c 6573 5f65 6d70 6c6f 7965 6573  (sales_employees
-0000d910: 2e61 6c6c 2e65 6d70 5f69 6429 290a 0a20  .all.emp_id)).. 
-0000d920: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000d930: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-0000d940: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000d950: 6572 7445 7175 616c 285b 2730 3030 3527  ertEqual(['0005'
-0000d960: 2c20 2730 3030 3127 2c20 2730 3030 3427  , '0001', '0004'
-0000d970: 2c20 2730 3030 3327 5d2c 0a20 2020 2020  , '0003'],.     
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 2020 2020 2020 2020 6c69 7374 2873 616c          list(sal
-0000d9a0: 6573 5f65 6d70 6c6f 7965 6573 2e61 6c6c  es_employees.all
-0000d9b0: 2e65 6d70 5f69 6429 290a 0a20 2020 2064  .emp_id))..    d
-0000d9c0: 6566 2074 6573 745f 756e 6971 7565 2873  ef test_unique(s
-0000d9d0: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
-0000d9e0: 7374 5f73 697a 6520 3d20 3130 0a20 2020  st_size = 10.   
-0000d9f0: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
-0000da00: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-0000da10: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-0000da20: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-0000da30: 2020 2020 2074 3220 3d20 7431 2e75 6e69       t2 = t1.uni
-0000da40: 7175 6528 290a 2020 2020 2020 2020 7769  que().        wi
-0000da50: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000da60: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000da70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000da80: 6c65 6e28 7431 292c 206c 656e 2874 3229  len(t1), len(t2)
-0000da90: 290a 0a20 2020 2020 2020 2074 3320 3d20  )..        t3 = 
-0000daa0: 7431 2e75 6e69 7175 6528 6b65 793d 6c61  t1.unique(key=la
-0000dab0: 6d62 6461 2072 6563 3a20 7265 632e 6329  mbda rec: rec.c)
-0000dac0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000dad0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000dae0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000daf0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-0000db00: 7369 7a65 2c20 6c65 6e28 7433 2929 0a0a  size, len(t3))..
-0000db10: 0a40 6d61 6b65 5f74 6573 745f 636c 6173  .@make_test_clas
-0000db20: 7365 730a 636c 6173 7320 5461 626c 654f  ses.class TableO
-0000db30: 7574 7075 7454 6573 7473 3a0a 2020 2020  utputTests:.    
-0000db40: 6465 6620 7465 7374 5f62 6173 6963 5f70  def test_basic_p
-0000db50: 7265 7365 6e74 2873 656c 6629 3a0a 2020  resent(self):.  
-0000db60: 2020 2020 2020 6966 2072 6963 6820 6973        if rich is
-0000db70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000db80: 2020 2069 6d70 6f72 7420 7761 726e 696e     import warnin
-0000db90: 6773 0a20 2020 2020 2020 2020 2020 2077  gs.            w
-0000dba0: 6172 6e69 6e67 732e 7761 726e 2822 7269  arnings.warn("ri
-0000dbb0: 6368 206e 6f74 2069 6e73 7461 6c6c 6564  ch not installed
-0000dbc0: 2c20 6361 6e6e 6f74 2072 756e 2074 6573  , cannot run tes
-0000dbd0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-0000dbe0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0000dbf0: 6672 6f6d 2072 6963 6820 696d 706f 7274  from rich import
-0000dc00: 2062 6f78 0a20 2020 2020 2020 2066 726f   box.        fro
-0000dc10: 6d20 696f 2069 6d70 6f72 7420 5374 7269  m io import Stri
-0000dc20: 6e67 494f 0a20 2020 2020 2020 2074 6162  ngIO.        tab
-0000dc30: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-0000dc40: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000dc50: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000dc60: 2020 2020 2020 2020 2020 2020 612c 620a              a,b.
-0000dc70: 2020 2020 2020 2020 2020 2020 3130 2c31              10,1
-0000dc80: 3030 0a20 2020 2020 2020 2020 2020 2032  00.            2
-0000dc90: 302c 3230 300a 2020 2020 2020 2020 2020  0,200.          
-0000dca0: 2020 2222 2229 290a 2020 2020 2020 2020    """)).        
-0000dcb0: 7461 626c 652e 7072 6573 656e 7428 290a  table.present().
-0000dcc0: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
-0000dcd0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-0000dce0: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
-0000dcf0: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
-0000dd00: 2e41 5343 4949 290a 2020 2020 2020 2020  .ASCII).        
-0000dd10: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
-0000dd20: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000dd30: 2020 2020 2020 2020 2020 2020 2b2d 2d2d              +---
-0000dd40: 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020 2020  -------+.       
-0000dd50: 2020 2020 207c 2041 2020 7c20 4220 2020       | A  | B   
-0000dd60: 7c0a 2020 2020 2020 2020 2020 2020 7c2d  |.            |-
-0000dd70: 2d2d 2d2b 2d2d 2d2d 2d7c 0a20 2020 2020  ---+-----|.     
-0000dd80: 2020 2020 2020 207c 2031 3020 7c20 3130         | 10 | 10
-0000dd90: 3020 7c0a 2020 2020 2020 2020 2020 2020  0 |.            
-0000dda0: 7c20 3230 207c 2032 3030 207c 0a20 2020  | 20 | 200 |.   
-0000ddb0: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
-0000ddc0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2020  ----+.          
-0000ddd0: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
-0000dde0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000ddf0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000de00: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000de10: 2865 7870 6563 7465 642c 206f 7574 2e67  (expected, out.g
-0000de20: 6574 7661 6c75 6528 2929 0a0a 2020 2020  etvalue())..    
-0000de30: 2020 2020 2320 7465 7374 2062 7567 6669      # test bugfi
-0000de40: 7820 7768 656e 2074 6162 6c65 2068 6173  x when table has
-0000de50: 2061 7474 7269 6275 7465 2022 6465 6661   attribute "defa
-0000de60: 756c 7422 0a20 2020 2020 2020 2074 6162  ult".        tab
-0000de70: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-0000de80: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000de90: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000dea0: 2020 2020 2020 2020 2020 2020 612c 622c              a,b,
-0000deb0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-0000dec0: 2020 2020 3130 2c31 3030 2c70 7572 706c      10,100,purpl
-0000ded0: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
-0000dee0: 2c31 3530 2c0a 2020 2020 2020 2020 2020  ,150,.          
-0000def0: 2020 3230 2c32 3030 2c6f 7261 6e67 650a    20,200,orange.
-0000df00: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000df10: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-0000df20: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000df30: 2020 6f75 7420 3d20 5374 7269 6e67 494f    out = StringIO
-0000df40: 2829 0a20 2020 2020 2020 2074 6162 6c65  ().        table
-0000df50: 2e70 7265 7365 6e74 2866 696c 653d 6f75  .present(file=ou
-0000df60: 742c 2062 6f78 3d62 6f78 2e41 5343 4949  t, box=box.ASCII
-0000df70: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
-0000df80: 6564 203d 2074 6578 7477 7261 702e 6465  ed = textwrap.de
-0000df90: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
-0000dfa0: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
-0000dfb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020  -----------+.   
-0000dfc0: 2020 2020 2020 2020 207c 2041 2020 7c20           | A  | 
-0000dfd0: 4220 2020 7c20 4465 6661 756c 7420 7c0a  B   | Default |.
-0000dfe0: 2020 2020 2020 2020 2020 2020 7c2d 2d2d              |---
-0000dff0: 2d2b 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -+-----+--------
-0000e000: 2d7c 0a20 2020 2020 2020 2020 2020 207c  -|.            |
-0000e010: 2031 3020 7c20 3130 3020 7c20 7075 7270   10 | 100 | purp
-0000e020: 6c65 2020 7c0a 2020 2020 2020 2020 2020  le  |.          
-0000e030: 2020 7c20 3135 207c 2031 3530 207c 2020    | 15 | 150 |  
-0000e040: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
-0000e050: 2020 2020 207c 2032 3020 7c20 3230 3020       | 20 | 200 
-0000e060: 7c20 6f72 616e 6765 2020 7c0a 2020 2020  | orange  |.    
-0000e070: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
-0000e080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20  -------------+. 
-0000e090: 2020 2020 2020 2020 2020 2022 2222 290a             """).
-0000e0a0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000e0b0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000e0c0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000e0d0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000e0e0: 6564 2c20 6f75 742e 6765 7476 616c 7565  ed, out.getvalue
-0000e0f0: 2829 290a 0a20 2020 2020 2020 2023 2074  ())..        # t
-0000e100: 6573 7420 6772 6f75 7062 790a 2020 2020  est groupby.    
-0000e110: 2020 2020 7461 626c 6520 3d20 6c74 2e54      table = lt.T
-0000e120: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-0000e130: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000e140: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000e150: 2020 2061 2c62 2c64 6566 6175 6c74 0a20     a,b,default. 
-0000e160: 2020 2020 2020 2020 2020 2031 302c 3130             10,10
-0000e170: 302c 7075 7270 6c65 0a20 2020 2020 2020  0,purple.       
-0000e180: 2020 2020 2031 352c 3135 302c 7075 7270       15,150,purp
-0000e190: 6c65 0a20 2020 2020 2020 2020 2020 2032  le.            2
-0000e1a0: 302c 3230 302c 6f72 616e 6765 0a20 2020  0,200,orange.   
-0000e1b0: 2020 2020 2020 2020 2022 2222 2929 0a20           """)). 
-0000e1c0: 2020 2020 2020 2074 6162 6c65 2e70 7265         table.pre
-0000e1d0: 7365 6e74 2829 0a20 2020 2020 2020 2074  sent().        t
-0000e1e0: 6162 6c65 2e70 7265 7365 6e74 2862 6f78  able.present(box
-0000e1f0: 3d62 6f78 2e41 5343 4949 2c20 6772 6f75  =box.ASCII, grou
-0000e200: 7062 793d 2264 6566 6175 6c74 2229 0a20  pby="default"). 
-0000e210: 2020 2020 2020 206f 7574 203d 2053 7472         out = Str
-0000e220: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
-0000e230: 7461 626c 652e 7072 6573 656e 7428 6669  table.present(fi
-0000e240: 6c65 3d6f 7574 2c20 626f 783d 626f 782e  le=out, box=box.
-0000e250: 4153 4349 492c 2067 726f 7570 6279 3d22  ASCII, groupby="
-0000e260: 6465 6661 756c 7422 290a 2020 2020 2020  default").      
-0000e270: 2020 6578 7065 6374 6564 203d 2074 6578    expected = tex
-0000e280: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
-0000e290: 5c0a 2020 2020 2020 2020 2020 2020 2b2d  \.            +-
-0000e2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e2b0: 2d2d 2d2b 0a20 2020 2020 2020 2020 2020  ---+.           
-0000e2c0: 207c 2041 2020 7c20 4220 2020 7c20 4465   | A  | B   | De
-0000e2d0: 6661 756c 7420 7c0a 2020 2020 2020 2020  fault |.        
-0000e2e0: 2020 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d2b      |----+-----+
-0000e2f0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 2020  ---------|.     
-0000e300: 2020 2020 2020 207c 2031 3020 7c20 3130         | 10 | 10
-0000e310: 3020 7c20 7075 7270 6c65 2020 7c0a 2020  0 | purple  |.  
-0000e320: 2020 2020 2020 2020 2020 7c20 3135 207c            | 15 |
-0000e330: 2031 3530 207c 2020 2020 2020 2020 207c   150 |         |
-0000e340: 0a20 2020 2020 2020 2020 2020 207c 2032  .            | 2
-0000e350: 3020 7c20 3230 3020 7c20 6f72 616e 6765  0 | 200 | orange
-0000e360: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000e370: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-0000e380: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2020  -----+.         
-0000e390: 2020 2022 2222 290a 2020 2020 2020 2020     """).        
-0000e3a0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000e3b0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000e3c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000e3d0: 6c28 6578 7065 6374 6564 2c20 6f75 742e  l(expected, out.
-0000e3e0: 6765 7476 616c 7565 2829 290a 0a20 2020  getvalue())..   
-0000e3f0: 2020 2020 2074 6162 6c65 203d 206c 742e       table = lt.
-0000e400: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-0000e410: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
-0000e420: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000e430: 2020 2020 612c 622c 6465 6661 756c 740a      a,b,default.
-0000e440: 2020 2020 2020 2020 2020 2020 3130 2c31              10,1
-0000e450: 3030 2c70 7572 706c 650a 2020 2020 2020  00,purple.      
-0000e460: 2020 2020 2020 3135 2c31 3530 2c70 7572        15,150,pur
-0000e470: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-0000e480: 3135 2c32 3030 2c6f 7261 6e67 650a 2020  15,200,orange.  
-0000e490: 2020 2020 2020 2020 2020 3135 2c32 3530            15,250
-0000e4a0: 2c6f 7261 6e67 650a 2020 2020 2020 2020  ,orange.        
-0000e4b0: 2020 2020 3230 2c32 3530 2c6f 7261 6e67      20,250,orang
-0000e4c0: 650a 2020 2020 2020 2020 2020 2020 2222  e.            ""
-0000e4d0: 2229 290a 2020 2020 2020 2020 7461 626c  ")).        tabl
-0000e4e0: 652e 7072 6573 656e 7428 290a 2020 2020  e.present().    
-0000e4f0: 2020 2020 7461 626c 652e 7072 6573 656e      table.presen
-0000e500: 7428 626f 783d 626f 782e 4153 4349 492c  t(box=box.ASCII,
-0000e510: 2067 726f 7570 6279 3d22 6465 6661 756c   groupby="defaul
-0000e520: 7420 6122 290a 2020 2020 2020 2020 6f75  t a").        ou
-0000e530: 7420 3d20 5374 7269 6e67 494f 2829 0a20  t = StringIO(). 
-0000e540: 2020 2020 2020 2074 6162 6c65 2e70 7265         table.pre
-0000e550: 7365 6e74 2866 696c 653d 6f75 742c 2062  sent(file=out, b
-0000e560: 6f78 3d62 6f78 2e41 5343 4949 2c20 6772  ox=box.ASCII, gr
-0000e570: 6f75 7062 793d 2264 6566 6175 6c74 2061  oupby="default a
-0000e580: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
-0000e590: 7465 6420 3d20 7465 7874 7772 6170 2e64  ted = textwrap.d
-0000e5a0: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
-0000e5b0: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-0000e5c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ------------+.  
-0000e5d0: 2020 2020 2020 2020 2020 7c20 4120 207c            | A  |
-0000e5e0: 2042 2020 207c 2044 6566 6175 6c74 207c   B   | Default |
-0000e5f0: 0a20 2020 2020 2020 2020 2020 207c 2d2d  .            |--
-0000e600: 2d2d 2b2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --+-----+-------
-0000e610: 2d2d 7c0a 2020 2020 2020 2020 2020 2020  --|.            
-0000e620: 7c20 3130 207c 2031 3030 207c 2070 7572  | 10 | 100 | pur
-0000e630: 706c 6520 207c 0a20 2020 2020 2020 2020  ple  |.         
-0000e640: 2020 207c 2031 3520 7c20 3135 3020 7c20     | 15 | 150 | 
-0000e650: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
-0000e660: 2020 2020 2020 7c20 3135 207c 2032 3030        | 15 | 200
-0000e670: 207c 206f 7261 6e67 6520 207c 0a20 2020   | orange  |.   
-0000e680: 2020 2020 2020 2020 207c 2020 2020 7c20           |    | 
-0000e690: 3235 3020 7c20 2020 2020 2020 2020 7c0a  250 |         |.
-0000e6a0: 2020 2020 2020 2020 2020 2020 7c20 3230              | 20
-0000e6b0: 207c 2032 3530 207c 2020 2020 2020 2020   | 250 |        
-0000e6c0: 207c 0a20 2020 2020 2020 2020 2020 202b   |.            +
-0000e6d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e6e0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2020  ----+.          
-0000e6f0: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
-0000e700: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000e710: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000e720: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000e730: 2865 7870 6563 7465 642c 206f 7574 2e67  (expected, out.g
-0000e740: 6574 7661 6c75 6528 2929 0a0a 2020 2020  etvalue())..    
-0000e750: 2020 2020 7461 626c 6520 3d20 6c74 2e54      table = lt.T
-0000e760: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-0000e770: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000e780: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000e790: 2020 2061 2c62 2c64 6566 6175 6c74 0a20     a,b,default. 
-0000e7a0: 2020 2020 2020 2020 2020 2031 302c 3130             10,10
-0000e7b0: 302c 7075 7270 6c65 0a20 2020 2020 2020  0,purple.       
-0000e7c0: 2020 2020 2031 352c 3230 302c 6f72 616e       15,200,oran
-0000e7d0: 6765 0a20 2020 2020 2020 2020 2020 2031  ge.            1
-0000e7e0: 352c 3135 302c 7075 7270 6c65 0a20 2020  5,150,purple.   
-0000e7f0: 2020 2020 2020 2020 2032 302c 3235 302c           20,250,
-0000e800: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
-0000e810: 2020 2031 352c 3235 302c 6f72 616e 6765     15,250,orange
-0000e820: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000e830: 2929 0a20 2020 2020 2020 2074 6162 6c65  )).        table
-0000e840: 2e73 6f72 7428 2264 6566 6175 6c74 2064  .sort("default d
-0000e850: 6573 632c 6122 290a 2020 2020 2020 2020  esc,a").        
-0000e860: 7461 626c 652e 7072 6573 656e 7428 290a  table.present().
-0000e870: 2020 2020 2020 2020 7461 626c 652e 7072          table.pr
-0000e880: 6573 656e 7428 626f 783d 626f 782e 4153  esent(box=box.AS
-0000e890: 4349 492c 2067 726f 7570 6279 3d22 6465  CII, groupby="de
-0000e8a0: 6661 756c 7420 6122 290a 2020 2020 2020  fault a").      
-0000e8b0: 2020 6f75 7420 3d20 5374 7269 6e67 494f    out = StringIO
-0000e8c0: 2829 0a20 2020 2020 2020 2074 6162 6c65  ().        table
-0000e8d0: 2e70 7265 7365 6e74 2866 696c 653d 6f75  .present(file=ou
-0000e8e0: 742c 2062 6f78 3d62 6f78 2e41 5343 4949  t, box=box.ASCII
-0000e8f0: 2c20 6772 6f75 7062 793d 2264 6566 6175  , groupby="defau
-0000e900: 6c74 2061 2229 0a20 2020 2020 2020 2065  lt a").        e
-0000e910: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
-0000e920: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000e930: 2020 2020 2020 2020 2020 202b 2d2d 2d2d             +----
-0000e940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e950: 2b0a 2020 2020 2020 2020 2020 2020 7c20  +.            | 
-0000e960: 4120 207c 2042 2020 207c 2044 6566 6175  A  | B   | Defau
-0000e970: 6c74 207c 0a20 2020 2020 2020 2020 2020  lt |.           
-0000e980: 207c 2d2d 2d2d 2b2d 2d2d 2d2d 2b2d 2d2d   |----+-----+---
-0000e990: 2d2d 2d2d 2d2d 7c0a 2020 2020 2020 2020  ------|.        
-0000e9a0: 2020 2020 7c20 3130 207c 2031 3030 207c      | 10 | 100 |
-0000e9b0: 2070 7572 706c 6520 207c 0a20 2020 2020   purple  |.     
-0000e9c0: 2020 2020 2020 207c 2031 3520 7c20 3135         | 15 | 15
-0000e9d0: 3020 7c20 2020 2020 2020 2020 7c0a 2020  0 |         |.  
-0000e9e0: 2020 2020 2020 2020 2020 7c20 3135 207c            | 15 |
-0000e9f0: 2032 3030 207c 206f 7261 6e67 6520 207c   200 | orange  |
-0000ea00: 0a20 2020 2020 2020 2020 2020 207c 2020  .            |  
-0000ea10: 2020 7c20 3235 3020 7c20 2020 2020 2020    | 250 |       
-0000ea20: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000ea30: 7c20 3230 207c 2032 3530 207c 2020 2020  | 20 | 250 |    
-0000ea40: 2020 2020 207c 0a20 2020 2020 2020 2020       |.         
-0000ea50: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     +------------
-0000ea60: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
-0000ea70: 2020 2020 2020 2222 2229 0a20 2020 2020        """).     
-0000ea80: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000ea90: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000eaa0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000eab0: 7175 616c 2865 7870 6563 7465 642c 206f  qual(expected, o
-0000eac0: 7574 2e67 6574 7661 6c75 6528 2929 0a0a  ut.getvalue())..
-0000ead0: 2020 2020 6465 6620 7465 7374 5f6d 6172      def test_mar
-0000eae0: 6b64 6f77 6e28 7365 6c66 293a 0a20 2020  kdown(self):.   
-0000eaf0: 2020 2020 2074 6162 6c65 203d 206c 742e       table = lt.
-0000eb00: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-0000eb10: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
-0000eb20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000eb30: 2020 2020 612c 620a 2020 2020 2020 2020      a,b.        
-0000eb40: 2020 2020 3130 2c31 3030 0a20 2020 2020      10,100.     
-0000eb50: 2020 2020 2020 2032 302c 3230 300a 2020         20,200.  
-0000eb60: 2020 2020 2020 2020 2020 2222 2229 290a            """)).
-0000eb70: 2020 2020 2020 2020 6f75 745f 6d61 726b          out_mark
-0000eb80: 646f 776e 203d 2074 6162 6c65 2e61 735f  down = table.as_
-0000eb90: 6d61 726b 646f 776e 2829 0a20 2020 2020  markdown().     
-0000eba0: 2020 2070 7269 6e74 286f 7574 5f6d 6172     print(out_mar
-0000ebb0: 6b64 6f77 6e29 0a20 2020 2020 2020 2065  kdown).        e
-0000ebc0: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
-0000ebd0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000ebe0: 2020 2020 2020 2020 2020 207c 2061 207c             | a |
-0000ebf0: 2062 207c 0a20 2020 2020 2020 2020 2020   b |.           
-0000ec00: 207c 2d2d 2d7c 2d2d 2d7c 0a20 2020 2020   |---|---|.     
-0000ec10: 2020 2020 2020 207c 2031 3020 7c20 3130         | 10 | 10
-0000ec20: 3020 7c0a 2020 2020 2020 2020 2020 2020  0 |.            
-0000ec30: 7c20 3230 207c 2032 3030 207c 0a20 2020  | 20 | 200 |.   
-0000ec40: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
-0000ec50: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000ec60: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000ec70: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000ec80: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-0000ec90: 2c20 6f75 745f 6d61 726b 646f 776e 290a  , out_markdown).
-0000eca0: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
-0000ecb0: 6275 6766 6978 2077 6865 6e20 7461 626c  bugfix when tabl
-0000ecc0: 6520 6861 7320 6174 7472 6962 7574 6520  e has attribute 
-0000ecd0: 2264 6566 6175 6c74 220a 2020 2020 2020  "default".      
-0000ece0: 2020 7461 626c 6520 3d20 6c74 2e54 6162    table = lt.Tab
-0000ecf0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-0000ed00: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-0000ed10: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
-0000ed20: 2061 2c62 2c64 6566 6175 6c74 0a20 2020   a,b,default.   
-0000ed30: 2020 2020 2020 2020 2031 302c 3130 302c           10,100,
-0000ed40: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
-0000ed50: 2020 2031 352c 3135 302c 0a20 2020 2020     15,150,.     
-0000ed60: 2020 2020 2020 2032 302c 3230 302c 6f72         20,200,or
-0000ed70: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
-0000ed80: 2022 2222 2929 0a20 2020 2020 2020 206f   """)).        o
-0000ed90: 7574 5f6d 6172 6b64 6f77 6e20 3d20 7461  ut_markdown = ta
-0000eda0: 626c 652e 6173 5f6d 6172 6b64 6f77 6e28  ble.as_markdown(
-0000edb0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000edc0: 6f75 745f 6d61 726b 646f 776e 290a 2020  out_markdown).  
-0000edd0: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
-0000ede0: 2074 6578 7477 7261 702e 6465 6465 6e74   textwrap.dedent
-0000edf0: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000ee00: 2020 7c20 6120 7c20 6220 7c20 6465 6661    | a | b | defa
-0000ee10: 756c 7420 7c0a 2020 2020 2020 2020 2020  ult |.          
-0000ee20: 2020 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a    |---|---|---|.
-0000ee30: 2020 2020 2020 2020 2020 2020 7c20 3130              | 10
-0000ee40: 207c 2031 3030 207c 2070 7572 706c 6520   | 100 | purple 
-0000ee50: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
-0000ee60: 3135 207c 2031 3530 207c 2020 7c0a 2020  15 | 150 |  |.  
-0000ee70: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
-0000ee80: 2032 3030 207c 206f 7261 6e67 6520 7c0a   200 | orange |.
-0000ee90: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000eea0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000eeb0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000eec0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000eed0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000eee0: 7465 642c 206f 7574 5f6d 6172 6b64 6f77  ted, out_markdow
-0000eef0: 6e29 0a0a 2020 2020 2020 2020 2320 7465  n)..        # te
-0000ef00: 7374 2067 726f 7570 696e 6720 696e 2061  st grouping in a
-0000ef10: 735f 6d61 726b 646f 776e 0a20 2020 2020  s_markdown.     
-0000ef20: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
-0000ef30: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000ef40: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000ef50: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000ef60: 2020 612c 622c 6465 6661 756c 740a 2020    a,b,default.  
-0000ef70: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
-0000ef80: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
-0000ef90: 2020 2020 3135 2c31 3530 2c70 7572 706c      15,150,purpl
-0000efa0: 650a 2020 2020 2020 2020 2020 2020 3230  e.            20
-0000efb0: 2c32 3030 2c6f 7261 6e67 650a 2020 2020  ,200,orange.    
-0000efc0: 2020 2020 2020 2020 2222 2229 290a 2020          """)).  
-0000efd0: 2020 2020 2020 6f75 745f 6d61 726b 646f        out_markdo
-0000efe0: 776e 203d 2074 6162 6c65 2e61 735f 6d61  wn = table.as_ma
-0000eff0: 726b 646f 776e 2867 726f 7570 6279 3d22  rkdown(groupby="
-0000f000: 6465 6661 756c 7422 290a 2020 2020 2020  default").      
-0000f010: 2020 7072 696e 7428 6f75 745f 6d61 726b    print(out_mark
-0000f020: 646f 776e 290a 2020 2020 2020 2020 6578  down).        ex
-0000f030: 7065 6374 6564 203d 2074 6578 7477 7261  pected = textwra
-0000f040: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-0000f050: 2020 2020 2020 2020 2020 7c20 6120 7c20            | a | 
-0000f060: 6220 7c20 6465 6661 756c 7420 7c0a 2020  b | default |.  
-0000f070: 2020 2020 2020 2020 2020 7c2d 2d2d 7c2d            |---|-
-0000f080: 2d2d 7c2d 2d2d 7c0a 2020 2020 2020 2020  --|---|.        
-0000f090: 2020 2020 7c20 3130 207c 2031 3030 207c      | 10 | 100 |
-0000f0a0: 2070 7572 706c 6520 7c0a 2020 2020 2020   purple |.      
-0000f0b0: 2020 2020 2020 7c20 3135 207c 2031 3530        | 15 | 150
-0000f0c0: 207c 2020 7c0a 2020 2020 2020 2020 2020   |  |.          
-0000f0d0: 2020 7c20 3230 207c 2032 3030 207c 206f    | 20 | 200 | o
-0000f0e0: 7261 6e67 6520 7c0a 2020 2020 2020 2020  range |.        
-0000f0f0: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
-0000f100: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000f110: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000f120: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000f130: 616c 2865 7870 6563 7465 642c 206f 7574  al(expected, out
-0000f140: 5f6d 6172 6b64 6f77 6e29 0a0a 2020 2020  _markdown)..    
-0000f150: 2020 2020 7461 626c 6520 3d20 6c74 2e54      table = lt.T
-0000f160: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-0000f170: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000f180: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000f190: 2020 2061 2c62 2c64 6566 6175 6c74 0a20     a,b,default. 
-0000f1a0: 2020 2020 2020 2020 2020 2031 302c 3130             10,10
-0000f1b0: 302c 7075 7270 6c65 0a20 2020 2020 2020  0,purple.       
-0000f1c0: 2020 2020 2031 352c 3230 302c 6f72 616e       15,200,oran
-0000f1d0: 6765 0a20 2020 2020 2020 2020 2020 2031  ge.            1
-0000f1e0: 352c 3135 302c 7075 7270 6c65 0a20 2020  5,150,purple.   
-0000f1f0: 2020 2020 2020 2020 2032 302c 3235 302c           20,250,
-0000f200: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
-0000f210: 2020 2031 352c 3235 302c 6f72 616e 6765     15,250,orange
-0000f220: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000f230: 2929 0a20 2020 2020 2020 2074 6162 6c65  )).        table
-0000f240: 2e73 6f72 7428 2264 6566 6175 6c74 2064  .sort("default d
-0000f250: 6573 632c 6122 290a 2020 2020 2020 2020  esc,a").        
-0000f260: 6f75 745f 6d61 726b 646f 776e 203d 2074  out_markdown = t
-0000f270: 6162 6c65 2e61 735f 6d61 726b 646f 776e  able.as_markdown
-0000f280: 2867 726f 7570 6279 3d22 6465 6661 756c  (groupby="defaul
-0000f290: 7420 6122 290a 2020 2020 2020 2020 7072  t a").        pr
-0000f2a0: 696e 7428 6f75 745f 6d61 726b 646f 776e  int(out_markdown
-0000f2b0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
-0000f2c0: 6564 203d 2074 6578 7477 7261 702e 6465  ed = textwrap.de
-0000f2d0: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
-0000f2e0: 2020 2020 2020 7c20 6120 7c20 6220 7c20        | a | b | 
-0000f2f0: 6465 6661 756c 7420 7c0a 2020 2020 2020  default |.      
-0000f300: 2020 2020 2020 7c2d 2d2d 7c2d 2d2d 7c2d        |---|---|-
-0000f310: 2d2d 7c0a 2020 2020 2020 2020 2020 2020  --|.            
-0000f320: 7c20 3130 207c 2031 3030 207c 2070 7572  | 10 | 100 | pur
-0000f330: 706c 6520 7c0a 2020 2020 2020 2020 2020  ple |.          
-0000f340: 2020 7c20 3135 207c 2031 3530 207c 2020    | 15 | 150 |  
-0000f350: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
-0000f360: 3135 207c 2032 3030 207c 206f 7261 6e67  15 | 200 | orang
-0000f370: 6520 7c0a 2020 2020 2020 2020 2020 2020  e |.            
-0000f380: 7c20 207c 2032 3530 207c 2020 7c0a 2020  |  | 250 |  |.  
-0000f390: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
-0000f3a0: 2032 3530 207c 2020 7c0a 2020 2020 2020   250 |  |.      
-0000f3b0: 2020 2020 2020 2222 2229 0a20 2020 2020        """).     
-0000f3c0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000f3d0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000f3e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000f3f0: 7175 616c 2865 7870 6563 7465 642c 206f  qual(expected, o
-0000f400: 7574 5f6d 6172 6b64 6f77 6e29 0a0a 2320  ut_markdown)..# 
-0000f410: 7361 6d70 6c65 2069 6d70 6f72 7420 6461  sample import da
-0000f420: 7461 2073 6574 730a 6373 765f 6461 7461  ta sets.csv_data
-0000f430: 203d 2022 2222 5c0a 612c 622c 630a 302c   = """\.a,b,c.0,
-0000f440: 302c 300a 302c 302c 310a 302c 302c 320a  0,0.0,0,1.0,0,2.
-0000f450: 302c 312c 300a 302c 312c 310a 302c 312c  0,1,0.0,1,1.0,1,
-0000f460: 320a 302c 322c 300a 302c 322c 310a 302c  2.0,2,0.0,2,1.0,
-0000f470: 322c 320a 312c 302c 300a 312c 302c 310a  2,2.1,0,0.1,0,1.
-0000f480: 312c 302c 320a 312c 312c 300a 312c 312c  1,0,2.1,1,0.1,1,
-0000f490: 310a 312c 312c 320a 312c 322c 300a 312c  1.1,1,2.1,2,0.1,
-0000f4a0: 322c 310a 312c 322c 320a 322c 302c 300a  2,1.1,2,2.2,0,0.
-0000f4b0: 322c 302c 310a 322c 302c 320a 322c 312c  2,0,1.2,0,2.2,1,
-0000f4c0: 300a 322c 312c 310a 322c 312c 320a 322c  0.2,1,1.2,1,2.2,
-0000f4d0: 322c 300a 322c 322c 310a 322c 322c 320a  2,0.2,2,1.2,2,2.
-0000f4e0: 0a22 2222 0a0a 6a73 6f6e 5f64 6174 6120  ."""..json_data 
-0000f4f0: 3d20 2222 225c 0a20 2020 207b 2261 223a  = """\.    {"a":
-0000f500: 2030 2c20 2262 223a 2030 2c20 2263 223a   0, "b": 0, "c":
-0000f510: 2030 7d0a 2020 2020 7b22 6122 3a20 302c   0}.    {"a": 0,
-0000f520: 2022 6222 3a20 302c 2022 6322 3a20 317d   "b": 0, "c": 1}
-0000f530: 0a20 2020 207b 2261 223a 2030 2c20 2262  .    {"a": 0, "b
-0000f540: 223a 2030 2c20 2263 223a 2032 7d0a 2020  ": 0, "c": 2}.  
-0000f550: 2020 7b22 6122 3a20 302c 2022 6222 3a20    {"a": 0, "b": 
-0000f560: 312c 2022 6322 3a20 307d 0a20 2020 207b  1, "c": 0}.    {
-0000f570: 2261 223a 2030 2c20 2262 223a 2031 2c20  "a": 0, "b": 1, 
-0000f580: 2263 223a 2031 7d0a 2020 2020 7b22 6122  "c": 1}.    {"a"
-0000f590: 3a20 302c 2022 6222 3a20 312c 2022 6322  : 0, "b": 1, "c"
-0000f5a0: 3a20 327d 0a20 2020 207b 2261 223a 2030  : 2}.    {"a": 0
-0000f5b0: 2c20 2262 223a 2032 2c20 2263 223a 2030  , "b": 2, "c": 0
-0000f5c0: 7d0a 2020 2020 7b22 6122 3a20 302c 2022  }.    {"a": 0, "
-0000f5d0: 6222 3a20 322c 2022 6322 3a20 317d 0a20  b": 2, "c": 1}. 
-0000f5e0: 2020 207b 2261 223a 2030 2c20 2262 223a     {"a": 0, "b":
-0000f5f0: 2032 2c20 2263 223a 2032 7d0a 2020 2020   2, "c": 2}.    
-0000f600: 7b22 6122 3a20 312c 2022 6222 3a20 302c  {"a": 1, "b": 0,
-0000f610: 2022 6322 3a20 307d 0a20 2020 207b 2261   "c": 0}.    {"a
-0000f620: 223a 2031 2c20 2262 223a 2030 2c20 2263  ": 1, "b": 0, "c
-0000f630: 223a 2031 7d0a 2020 2020 7b22 6122 3a20  ": 1}.    {"a": 
-0000f640: 312c 2022 6222 3a20 302c 2022 6322 3a20  1, "b": 0, "c": 
-0000f650: 327d 0a20 2020 207b 2261 223a 2031 2c20  2}.    {"a": 1, 
-0000f660: 2262 223a 2031 2c20 2263 223a 2030 7d0a  "b": 1, "c": 0}.
-0000f670: 2020 2020 7b22 6122 3a20 312c 2022 6222      {"a": 1, "b"
-0000f680: 3a20 312c 2022 6322 3a20 317d 0a20 2020  : 1, "c": 1}.   
-0000f690: 207b 2261 223a 2031 2c20 2262 223a 2031   {"a": 1, "b": 1
-0000f6a0: 2c20 2263 223a 2032 7d0a 2020 2020 7b22  , "c": 2}.    {"
-0000f6b0: 6122 3a20 312c 2022 6222 3a20 322c 2022  a": 1, "b": 2, "
-0000f6c0: 6322 3a20 307d 0a20 2020 207b 2261 223a  c": 0}.    {"a":
-0000f6d0: 2031 2c20 2262 223a 2032 2c20 2263 223a   1, "b": 2, "c":
-0000f6e0: 2031 7d0a 2020 2020 7b22 6122 3a20 312c   1}.    {"a": 1,
-0000f6f0: 2022 6222 3a20 322c 2022 6322 3a20 327d   "b": 2, "c": 2}
-0000f700: 0a20 2020 207b 2261 223a 2032 2c20 2262  .    {"a": 2, "b
-0000f710: 223a 2030 2c20 2263 223a 2030 7d0a 2020  ": 0, "c": 0}.  
-0000f720: 2020 7b22 6122 3a20 322c 2022 6222 3a20    {"a": 2, "b": 
-0000f730: 302c 2022 6322 3a20 317d 0a20 2020 207b  0, "c": 1}.    {
-0000f740: 2261 223a 2032 2c20 2262 223a 2030 2c20  "a": 2, "b": 0, 
-0000f750: 2263 223a 2032 7d0a 2020 2020 7b22 6122  "c": 2}.    {"a"
-0000f760: 3a20 322c 2022 6222 3a20 312c 2022 6322  : 2, "b": 1, "c"
-0000f770: 3a20 307d 0a20 2020 207b 2261 223a 2032  : 0}.    {"a": 2
-0000f780: 2c20 2262 223a 2031 2c20 2263 223a 2031  , "b": 1, "c": 1
-0000f790: 7d0a 2020 2020 7b22 6122 3a20 322c 2022  }.    {"a": 2, "
-0000f7a0: 6222 3a20 312c 2022 6322 3a20 327d 0a20  b": 1, "c": 2}. 
-0000f7b0: 2020 207b 2261 223a 2032 2c20 2262 223a     {"a": 2, "b":
-0000f7c0: 2032 2c20 2263 223a 2030 7d0a 2020 2020   2, "c": 0}.    
-0000f7d0: 7b22 6122 3a20 322c 2022 6222 3a20 322c  {"a": 2, "b": 2,
-0000f7e0: 2022 6322 3a20 317d 0a20 2020 207b 2261   "c": 1}.    {"a
-0000f7f0: 223a 2032 2c20 2262 223a 2032 2c20 2263  ": 2, "b": 2, "c
-0000f800: 223a 2032 7d0a 0a22 2222 0a0a 6669 7865  ": 2}.."""..fixe
-0000f810: 645f 7769 6474 685f 6461 7461 203d 2022  d_width_data = "
-0000f820: 2222 5c0a 3020 3020 300a 3020 3020 310a  ""\.0 0 0.0 0 1.
-0000f830: 3020 3020 320a 3020 3120 300a 3020 3120  0 0 2.0 1 0.0 1 
-0000f840: 310a 3020 3120 320a 3020 3220 300a 3020  1.0 1 2.0 2 0.0 
-0000f850: 3220 310a 3020 3220 320a 3120 3020 300a  2 1.0 2 2.1 0 0.
-0000f860: 3120 3020 310a 3120 3020 320a 3120 3120  1 0 1.1 0 2.1 1 
-0000f870: 300a 3120 3120 310a 3120 3120 320a 3120  0.1 1 1.1 1 2.1 
-0000f880: 3220 300a 3120 3220 310a 3120 3220 320a  2 0.1 2 1.1 2 2.
-0000f890: 3220 3020 300a 3220 3020 310a 3220 3020  2 0 0.2 0 1.2 0 
-0000f8a0: 320a 3220 3120 300a 3220 3120 310a 3220  2.2 1 0.2 1 1.2 
-0000f8b0: 3120 320a 3220 3220 300a 3220 3220 310a  1 2.2 2 0.2 2 1.
-0000f8c0: 3220 3220 320a 0a22 2222 0a0a 0a40 6d61  2 2 2.."""...@ma
-0000f8d0: 6b65 5f74 6573 745f 636c 6173 7365 730a  ke_test_classes.
-0000f8e0: 636c 6173 7320 5461 626c 6549 6d70 6f72  class TableImpor
-0000f8f0: 7445 7870 6f72 7454 6573 7473 3a0a 2020  tExportTests:.  
-0000f900: 2020 6465 6620 7465 7374 5f63 7376 5f65    def test_csv_e
-0000f910: 7870 6f72 7428 7365 6c66 293a 0a20 2020  xport(self):.   
-0000f920: 2020 2020 2066 726f 6d20 6974 6572 746f       from iterto
-0000f930: 6f6c 7320 696d 706f 7274 2070 6572 6d75  ols import permu
-0000f940: 7461 7469 6f6e 730a 2020 2020 2020 2020  tations.        
-0000f950: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
-0000f960: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
-0000f970: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
-0000f980: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-0000f990: 2c20 7465 7374 5f73 697a 6529 0a20 2020  , test_size).   
-0000f9a0: 2020 2020 2066 6f72 2066 6965 6c64 6e61       for fieldna
-0000f9b0: 6d65 7320 696e 2070 6572 6d75 7461 7469  mes in permutati
-0000f9c0: 6f6e 7328 6c69 7374 2827 6162 6327 2929  ons(list('abc'))
-0000f9d0: 3a0a 2020 2020 2020 2020 2020 2020 6f75  :.            ou
-0000f9e0: 7420 3d20 696f 2e53 7472 696e 6749 4f28  t = io.StringIO(
-0000f9f0: 290a 2020 2020 2020 2020 2020 2020 7431  ).            t1
-0000fa00: 2e63 7376 5f65 7870 6f72 7428 6f75 742c  .csv_export(out,
-0000fa10: 2066 6965 6c64 6e61 6d65 7329 0a20 2020   fieldnames).   
-0000fa20: 2020 2020 2020 2020 206f 7574 2e73 6565           out.see
-0000fa30: 6b28 3029 0a20 2020 2020 2020 2020 2020  k(0).           
-0000fa40: 206f 7574 6c69 6e65 7320 3d20 6f75 742e   outlines = out.
-0000fa50: 7265 6164 2829 2e73 706c 6974 6c69 6e65  read().splitline
-0000fa60: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000fa70: 6f75 742e 636c 6f73 6528 290a 2020 2020  out.close().    
-0000fa80: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000fa90: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000faa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fab0: 662e 6173 7365 7274 4571 7561 6c28 272c  f.assertEqual(',
-0000fac0: 272e 6a6f 696e 2866 6965 6c64 6e61 6d65  '.join(fieldname
-0000fad0: 7329 2c20 6f75 746c 696e 6573 5b30 5d29  s), outlines[0])
-0000fae0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000faf0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000fb00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fb10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000fb20: 616c 2874 6573 745f 7369 7a65 2a2a 332b  al(test_size**3+
-0000fb30: 312c 206c 656e 286f 7574 6c69 6e65 7329  1, len(outlines)
-0000fb40: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000fb50: 7220 6f62 2c20 6c69 6e65 2069 6e20 7a69  r ob, line in zi
-0000fb60: 7028 7431 2c20 6f75 746c 696e 6573 5b31  p(t1, outlines[1
-0000fb70: 3a5d 293a 0a20 2020 2020 2020 2020 2020  :]):.           
-0000fb80: 2020 2020 2063 7376 5f76 616c 7320 3d20       csv_vals = 
-0000fb90: 6c69 6e65 2e73 706c 6974 2827 2c27 290a  line.split(',').
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbb0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000fbc0: 7428 6f62 3d6f 622c 2063 7376 5f76 616c  t(ob=ob, csv_val
-0000fbd0: 733d 6373 765f 7661 6c73 293a 0a20 2020  s=csv_vals):.   
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0000fc00: 2861 6c6c 280a 2020 2020 2020 2020 2020  (all(.          
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000fc20: 7428 6373 765f 7661 6c73 5b69 5d29 203d  t(csv_vals[i]) =
-0000fc30: 3d20 6765 7461 7474 7228 6f62 2c20 666c  = getattr(ob, fl
-0000fc40: 6429 2066 6f72 2069 2c20 666c 6420 696e  d) for i, fld in
-0000fc50: 2065 6e75 6d65 7261 7465 2866 6965 6c64   enumerate(field
-0000fc60: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
-0000fc70: 2020 2020 2020 2020 2020 2029 290a 0a20             )).. 
-0000fc80: 2020 2020 2020 2023 2072 6572 756e 2075         # rerun u
-0000fc90: 7369 6e67 2061 6e20 656d 7074 7920 7461  sing an empty ta
-0000fca0: 626c 650a 2020 2020 2020 2020 7431 203d  ble.        t1 =
-0000fcb0: 206c 742e 5461 626c 6528 290a 2020 2020   lt.Table().    
-0000fcc0: 2020 2020 666f 7220 6669 656c 646e 616d      for fieldnam
-0000fcd0: 6573 2069 6e20 7065 726d 7574 6174 696f  es in permutatio
-0000fce0: 6e73 286c 6973 7428 2761 6263 2729 293a  ns(list('abc')):
-0000fcf0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-0000fd00: 203d 2069 6f2e 5374 7269 6e67 494f 2829   = io.StringIO()
-0000fd10: 0a20 2020 2020 2020 2020 2020 2074 312e  .            t1.
-0000fd20: 6373 765f 6578 706f 7274 286f 7574 2c20  csv_export(out, 
-0000fd30: 6669 656c 646e 616d 6573 290a 2020 2020  fieldnames).    
-0000fd40: 2020 2020 2020 2020 6f75 742e 7365 656b          out.seek
-0000fd50: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
-0000fd60: 6f75 746c 696e 6573 203d 206f 7574 2e72  outlines = out.r
-0000fd70: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
-0000fd80: 2829 0a20 2020 2020 2020 2020 2020 206f  ().            o
-0000fd90: 7574 2e63 6c6f 7365 2829 0a20 2020 2020  ut.close().     
-0000fda0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000fdb0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-0000fdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fdd0: 2e61 7373 6572 7445 7175 616c 2827 2c27  .assertEqual(','
-0000fde0: 2e6a 6f69 6e28 6669 656c 646e 616d 6573  .join(fieldnames
-0000fdf0: 292c 206f 7574 6c69 6e65 735b 305d 290a  ), outlines[0]).
-0000fe00: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000fe10: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000fe20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe30: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000fe40: 6c28 312c 206c 656e 286f 7574 6c69 6e65  l(1, len(outline
-0000fe50: 7329 290a 0a20 2020 2020 2020 2023 2072  s))..        # r
-0000fe60: 6572 756e 2075 7369 6e67 2061 6e20 656d  erun using an em
-0000fe70: 7074 7920 7461 626c 652c 2077 6974 6820  pty table, with 
-0000fe80: 696e 6465 7865 7320 746f 2064 6963 7461  indexes to dicta
-0000fe90: 7465 2066 6965 6c64 6e61 6d65 730a 2020  te fieldnames.  
-0000fea0: 2020 2020 2020 666f 7220 6669 656c 646e        for fieldn
-0000feb0: 616d 6573 2069 6e20 7065 726d 7574 6174  ames in permutat
-0000fec0: 696f 6e73 286c 6973 7428 2761 6263 2729  ions(list('abc')
-0000fed0: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-0000fee0: 3120 3d20 6c74 2e54 6162 6c65 2829 0a20  1 = lt.Table(). 
-0000fef0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-0000ff00: 6c64 2069 6e20 6669 656c 646e 616d 6573  ld in fieldnames
-0000ff10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ff20: 2020 7431 2e63 7265 6174 655f 696e 6465    t1.create_inde
-0000ff30: 7828 666c 6429 0a20 2020 2020 2020 2020  x(fld).         
-0000ff40: 2020 206f 7574 203d 2069 6f2e 5374 7269     out = io.Stri
-0000ff50: 6e67 494f 2829 0a20 2020 2020 2020 2020  ngIO().         
-0000ff60: 2020 2074 312e 6373 765f 6578 706f 7274     t1.csv_export
-0000ff70: 286f 7574 290a 2020 2020 2020 2020 2020  (out).          
-0000ff80: 2020 6f75 742e 7365 656b 2830 290a 2020    out.seek(0).  
-0000ff90: 2020 2020 2020 2020 2020 6f75 746c 696e            outlin
-0000ffa0: 6573 203d 206f 7574 2e72 6561 6428 292e  es = out.read().
-0000ffb0: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
-0000ffc0: 2020 2020 2020 2020 206f 7574 2e63 6c6f           out.clo
-0000ffd0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-0000ffe0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000fff0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00010000: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010010: 7445 7175 616c 2873 6574 2866 6965 6c64  tEqual(set(field
-00010020: 6e61 6d65 7329 2c20 7365 7428 6f75 746c  names), set(outl
-00010030: 696e 6573 5b30 5d2e 7370 6c69 7428 272c  ines[0].split(',
-00010040: 2729 2929 0a20 2020 2020 2020 2020 2020  '))).           
-00010050: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00010060: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00010070: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010080: 7445 7175 616c 2831 2c20 6c65 6e28 6f75  tEqual(1, len(ou
-00010090: 746c 696e 6573 2929 0a0a 2020 2020 6465  tlines))..    de
-000100a0: 6620 7465 7374 5f63 7376 5f65 7870 6f72  f test_csv_expor
-000100b0: 745f 746f 5f73 7472 696e 6728 7365 6c66  t_to_string(self
-000100c0: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
-000100d0: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-000100e0: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
-000100f0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00010100: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-00010110: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00010120: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00010130: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-00010140: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
-00010150: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
-00010160: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
-00010170: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
-00010180: 2020 2020 6f75 745f 7374 7269 6e67 203d      out_string =
-00010190: 2074 312e 6373 765f 6578 706f 7274 284e   t1.csv_export(N
-000101a0: 6f6e 652c 2066 6965 6c64 6e61 6d65 7329  one, fieldnames)
-000101b0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-000101c0: 6c69 6e65 7320 3d20 6f75 745f 7374 7269  lines = out_stri
-000101d0: 6e67 2e73 706c 6974 6c69 6e65 7328 290a  ng.splitlines().
-000101e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-000101f0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00010200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010210: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00010220: 6c28 272c 272e 6a6f 696e 2866 6965 6c64  l(','.join(field
-00010230: 6e61 6d65 7329 2c20 6f75 746c 696e 6573  names), outlines
-00010240: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-00010250: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00010260: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00010270: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010280: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-00010290: 202a 2a20 3320 2b20 312c 206c 656e 286f   ** 3 + 1, len(o
-000102a0: 7574 6c69 6e65 7329 290a 2020 2020 2020  utlines)).      
-000102b0: 2020 2020 2020 666f 7220 6f62 2c20 6c69        for ob, li
-000102c0: 6e65 2069 6e20 7a69 7028 7431 2c20 6f75  ne in zip(t1, ou
-000102d0: 746c 696e 6573 5b31 3a5d 293a 0a20 2020  tlines[1:]):.   
-000102e0: 2020 2020 2020 2020 2020 2020 2063 7376               csv
-000102f0: 5f76 616c 7320 3d20 6c69 6e65 2e73 706c  _vals = line.spl
-00010300: 6974 2827 2c27 290a 2020 2020 2020 2020  it(',').        
-00010310: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010320: 662e 7375 6254 6573 7428 6f62 3d6f 622c  f.subTest(ob=ob,
-00010330: 2063 7376 5f76 616c 733d 6373 765f 7661   csv_vals=csv_va
-00010340: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00010350: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00010360: 7365 7274 5472 7565 2861 6c6c 280a 2020  sertTrue(all(.  
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 2020 2020 696e 7428 6373 765f 7661        int(csv_va
-00010390: 6c73 5b69 5d29 203d 3d20 6765 7461 7474  ls[i]) == getatt
-000103a0: 7228 6f62 2c20 666c 6429 2066 6f72 2069  r(ob, fld) for i
-000103b0: 2c20 666c 6420 696e 2065 6e75 6d65 7261  , fld in enumera
-000103c0: 7465 2866 6965 6c64 6e61 6d65 7329 0a20  te(fieldnames). 
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 2029 290a 0a20 2020 2064 6566 2074     ))..    def t
-000103f0: 6573 745f 6373 765f 696d 706f 7274 2873  est_csv_import(s
-00010400: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00010410: 7461 203d 2063 7376 5f64 6174 610a 2020  ta = csv_data.  
-00010420: 2020 2020 2020 696e 6373 7620 3d20 696f        incsv = io
-00010430: 2e53 7472 696e 6749 4f28 6461 7461 290a  .StringIO(data).
-00010440: 2020 2020 2020 2020 6373 7674 6162 6c65          csvtable
-00010450: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-00010460: 765f 696d 706f 7274 2869 6e63 7376 2c20  v_import(incsv, 
-00010470: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
-00010480: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
-00010490: 2763 273a 2069 6e74 7d29 0a0a 2020 2020  'c': int})..    
-000104a0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-000104b0: 330a 2020 2020 2020 2020 7431 203d 206d  3.        t1 = m
-000104c0: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000104d0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000104e0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000104f0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00010500: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00010510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010520: 6173 7365 7274 5472 7565 2861 6c6c 286d  assertTrue(all(m
-00010530: 616b 655f 6461 7461 6f62 6a65 6374 5f66  ake_dataobject_f
-00010540: 726f 6d5f 6f62 2872 6563 3129 203d 3d20  rom_ob(rec1) == 
-00010550: 7265 6332 2066 6f72 2072 6563 312c 2072  rec2 for rec1, r
-00010560: 6563 3220 696e 207a 6970 2874 312c 2063  ec2 in zip(t1, c
-00010570: 7376 7461 626c 6529 2929 0a20 2020 2020  svtable))).     
-00010580: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00010590: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000105a0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000105b0: 7175 616c 2873 756d 2831 2066 6f72 206c  qual(sum(1 for l
-000105c0: 696e 6520 696e 2064 6174 612e 7370 6c69  ine in data.spli
-000105d0: 746c 696e 6573 2829 2069 6620 6c69 6e65  tlines() if line
-000105e0: 2e73 7472 6970 2829 292d 312c 206c 656e  .strip())-1, len
-000105f0: 2863 7376 7461 626c 6529 290a 0a20 2020  (csvtable))..   
-00010600: 2020 2020 2069 6e63 7376 203d 2069 6f2e       incsv = io.
-00010610: 5374 7269 6e67 494f 2864 6174 6129 0a20  StringIO(data). 
-00010620: 2020 2020 2020 2072 6f77 5f70 726f 746f         row_proto
-00010630: 7479 7065 203d 2073 656c 662e 6d61 6b65  type = self.make
-00010640: 5f64 6174 615f 6f62 6a65 6374 2830 2c20  _data_object(0, 
-00010650: 302c 2030 290a 2020 2020 2020 2020 6373  0, 0).        cs
-00010660: 7674 6162 6c65 3220 3d20 6c74 2e54 6162  vtable2 = lt.Tab
-00010670: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00010680: 696e 6373 762c 2074 7261 6e73 666f 726d  incsv, transform
-00010690: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
-000106a0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
-000106b0: 2c20 726f 775f 636c 6173 733d 7479 7065  , row_class=type
-000106c0: 2872 6f77 5f70 726f 746f 7479 7065 2929  (row_prototype))
-000106d0: 5b3a 335d 0a0a 2020 2020 2020 2020 7072  [:3]..        pr
-000106e0: 696e 7428 7479 7065 2874 315b 305d 292e  int(type(t1[0]).
-000106f0: 5f5f 6e61 6d65 5f5f 2c20 7431 5b30 5d29  __name__, t1[0])
-00010700: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
-00010710: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
-00010720: 292e 5f5f 6e61 6d65 5f5f 2c20 6373 7674  ).__name__, csvt
-00010730: 6162 6c65 325b 305d 290a 2020 2020 2020  able2[0]).      
-00010740: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00010750: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00010760: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00010770: 7561 6c28 7479 7065 2874 315b 305d 292c  ual(type(t1[0]),
-00010780: 2074 7970 6528 6373 7674 6162 6c65 325b   type(csvtable2[
-00010790: 305d 2929 0a0a 2020 2020 6465 6620 7465  0]))..    def te
-000107a0: 7374 5f63 7376 5f63 6f6d 7072 6573 7365  st_csv_compresse
-000107b0: 645f 696d 706f 7274 2873 656c 6629 3a0a  d_import(self):.
-000107c0: 2020 2020 2020 2020 7474 203d 206c 742e          tt = lt.
-000107d0: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-000107e0: 7274 2822 7465 7374 2f61 6263 2e63 7376  rt("test/abc.csv
-000107f0: 222c 2074 7261 6e73 666f 726d 733d 6469  ", transforms=di
-00010800: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
-00010810: 222c 2069 6e74 2929 0a20 2020 2020 2020  ", int)).       
-00010820: 2070 7269 6e74 2822 6162 632e 6373 7622   print("abc.csv"
-00010830: 2c20 7474 2e69 6e66 6f28 2929 0a0a 2020  , tt.info())..  
-00010840: 2020 2020 2020 636f 6d70 7265 7373 6564        compressed
-00010850: 5f66 696c 6573 203d 205b 0a20 2020 2020  _files = [.     
-00010860: 2020 2020 2020 2022 6162 632e 6373 762e         "abc.csv.
-00010870: 7a69 7022 2c0a 2020 2020 2020 2020 2020  zip",.          
-00010880: 2020 2261 6263 2e63 7376 2e67 7a22 2c0a    "abc.csv.gz",.
-00010890: 2020 2020 2020 2020 2020 2020 2261 6263              "abc
-000108a0: 2e63 7376 2e78 7a22 2c0a 2020 2020 2020  .csv.xz",.      
-000108b0: 2020 5d0a 2020 2020 2020 2020 666f 7220    ].        for 
-000108c0: 6e61 6d65 2069 6e20 636f 6d70 7265 7373  name in compress
-000108d0: 6564 5f66 696c 6573 3a0a 2020 2020 2020  ed_files:.      
-000108e0: 2020 2020 2020 696d 706f 7274 5f73 6f75        import_sou
-000108f0: 7263 655f 6e61 6d65 203d 2022 7465 7374  rce_name = "test
-00010900: 2f22 202b 206e 616d 650a 2020 2020 2020  /" + name.      
-00010910: 2020 2020 2020 7474 3220 3d20 6c74 2e54        tt2 = lt.T
-00010920: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-00010930: 7428 696d 706f 7274 5f73 6f75 7263 655f  t(import_source_
-00010940: 6e61 6d65 2c20 7472 616e 7366 6f72 6d73  name, transforms
-00010950: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00010960: 6162 6322 2c20 696e 7429 290a 2020 2020  abc", int)).    
-00010970: 2020 2020 2020 2020 7072 696e 7428 6e61          print(na
-00010980: 6d65 2c20 7474 322e 696e 666f 2829 290a  me, tt2.info()).
-00010990: 2020 2020 2020 2020 2020 2020 6578 7065              expe
-000109a0: 6374 6564 5f69 6e66 6f20 3d20 7b2a 2a74  cted_info = {**t
-000109b0: 742e 696e 666f 2829 2c20 226e 616d 6522  t.info(), "name"
-000109c0: 3a20 696d 706f 7274 5f73 6f75 7263 655f  : import_source_
-000109d0: 6e61 6d65 7d0a 2020 2020 2020 2020 2020  name}.          
-000109e0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-000109f0: 6573 7428 6e61 6d65 3d6e 616d 6529 3a0a  est(name=name):.
-00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00010a20: 2865 7870 6563 7465 645f 696e 666f 2c20  (expected_info, 
-00010a30: 7474 322e 696e 666f 2829 290a 2020 2020  tt2.info()).    
+0000ca70: 2073 7475 6465 6e74 5f69 643d 2273 7475   student_id="stu
+0000ca80: 6465 6e74 5f69 6422 292e 7768 6572 6528  dent_id").where(
+0000ca90: 636f 7572 7365 3d4e 6f6e 6529 0a20 2020  course=None).   
+0000caa0: 2020 2020 206e 6f6e 5f72 6567 2e70 7265       non_reg.pre
+0000cab0: 7365 6e74 2829 0a20 2020 2020 2020 2070  sent().        p
+0000cac0: 7269 6e74 286c 6973 7428 6e6f 6e5f 7265  rint(list(non_re
+0000cad0: 672e 616c 6c2e 6e61 6d65 2929 0a20 2020  g.all.name)).   
+0000cae0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000caf0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000cb00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000cb10: 7445 7175 616c 285b 2742 6f62 272c 2027  tEqual(['Bob', '
+0000cb20: 4461 7665 275d 2c20 736f 7274 6564 286e  Dave'], sorted(n
+0000cb30: 6f6e 5f72 6567 2e61 6c6c 2e6e 616d 6529  on_reg.all.name)
+0000cb40: 290a 0a20 2020 2020 2020 2023 2063 6f75  )..        # cou
+0000cb50: 7273 6573 2077 6974 6820 6e6f 2073 7475  rses with no stu
+0000cb60: 6465 6e74 730a 2020 2020 2020 2020 6e6f  dents.        no
+0000cb70: 5f73 7475 6465 6e74 7320 3d20 7265 6769  _students = regi
+0000cb80: 7374 7261 7469 6f6e 732e 6f75 7465 725f  strations.outer_
+0000cb90: 6a6f 696e 286c 742e 5461 626c 652e 4c45  join(lt.Table.LE
+0000cba0: 4654 5f4f 5554 4552 5f4a 4f49 4e2c 0a20  FT_OUTER_JOIN,. 
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 2020 2020 2020 2020 636f 7572 7365 732c          courses,
+0000cbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc00: 2020 2020 2020 2020 2020 636f 7572 7365            course
+0000cc10: 3d22 636f 7572 7365 2229 2e77 6865 7265  ="course").where
+0000cc20: 2873 7475 6465 6e74 5f69 643d 4e6f 6e65  (student_id=None
+0000cc30: 290a 2020 2020 2020 2020 6e6f 5f73 7475  ).        no_stu
+0000cc40: 6465 6e74 732e 7072 6573 656e 7428 290a  dents.present().
+0000cc50: 2020 2020 2020 2020 7072 696e 7428 6c69          print(li
+0000cc60: 7374 286e 6f5f 7374 7564 656e 7473 2e61  st(no_students.a
+0000cc70: 6c6c 2e63 6f75 7273 6529 290a 2020 2020  ll.course)).    
+0000cc80: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000cc90: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000cca0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000ccb0: 4571 7561 6c28 5b27 5045 3130 3127 5d2c  Equal(['PE101'],
+0000ccc0: 2073 6f72 7465 6428 6e6f 5f73 7475 6465   sorted(no_stude
+0000ccd0: 6e74 732e 616c 6c2e 636f 7572 7365 2929  nts.all.course))
+0000cce0: 0a0a 0a20 2020 2020 2020 2066 756c 6c20  ...        full 
+0000ccf0: 3d20 2073 7475 6465 6e74 732e 6f75 7465  =  students.oute
+0000cd00: 725f 6a6f 696e 286c 742e 5461 626c 652e  r_join(lt.Table.
+0000cd10: 4655 4c4c 5f4f 5554 4552 5f4a 4f49 4e2c  FULL_OUTER_JOIN,
+0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd40: 2020 2020 2020 2072 6567 6973 7472 6174         registrat
+0000cd50: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 2020 2020 2020 7374 7564              stud
+0000cd80: 656e 745f 6964 3d22 7374 7564 656e 745f  ent_id="student_
+0000cd90: 6964 2229 2e77 6865 7265 286c 616d 6264  id").where(lambd
+0000cda0: 6120 7265 633a 2072 6563 2e63 6f75 7273  a rec: rec.cours
+0000cdb0: 6520 6973 204e 6f6e 650a 2020 2020 2020  e is None.      
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 2020 2020 2020 206f 7220 7265             or re
+0000ce10: 632e 6e61 6d65 2069 7320 4e6f 6e65 290a  c.name is None).
+0000ce20: 2020 2020 2020 2020 6675 6c6c 2e70 7265          full.pre
+0000ce30: 7365 6e74 2829 0a20 2020 2020 2020 2070  sent().        p
+0000ce40: 7269 6e74 2873 6f72 7465 6428 6675 6c6c  rint(sorted(full
+0000ce50: 2e61 6c6c 2e73 7475 6465 6e74 5f69 6429  .all.student_id)
+0000ce60: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000ce70: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000ce80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ce90: 6173 7365 7274 4571 7561 6c28 5b27 3030  assertEqual(['00
+0000cea0: 3032 272c 2027 3030 3034 272c 2027 3030  02', '0004', '00
+0000ceb0: 3036 275d 2c20 736f 7274 6564 2866 756c  06'], sorted(ful
+0000cec0: 6c2e 616c 6c2e 7374 7564 656e 745f 6964  l.all.student_id
+0000ced0: 2929 0a0a 0a40 6d61 6b65 5f74 6573 745f  ))...@make_test_
+0000cee0: 636c 6173 7365 730a 636c 6173 7320 5461  classes.class Ta
+0000cef0: 626c 6554 7261 6e73 666f 726d 5465 7374  bleTransformTest
+0000cf00: 733a 0a20 2020 2064 6566 2074 6573 745f  s:.    def test_
+0000cf10: 736f 7274 2873 656c 6629 3a0a 2020 2020  sort(self):.    
+0000cf20: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+0000cf30: 3130 0a20 2020 2020 2020 2074 3120 3d20  10.        t1 = 
+0000cf40: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+0000cf50: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+0000cf60: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+0000cf70: 290a 0a20 2020 2020 2020 2063 5f67 726f  )..        c_gro
+0000cf80: 7570 7320 3d20 300a 2020 2020 2020 2020  ups = 0.        
+0000cf90: 666f 7220 635f 7661 6c75 652c 2072 6563  for c_value, rec
+0000cfa0: 7320 696e 2069 7465 7274 6f6f 6c73 2e67  s in itertools.g
+0000cfb0: 726f 7570 6279 2874 312c 206b 6579 3d6c  roupby(t1, key=l
+0000cfc0: 616d 6264 6120 7265 633a 2072 6563 2e63  ambda rec: rec.c
+0000cfd0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0000cfe0: 5f67 726f 7570 7320 2b3d 2031 0a20 2020  _groups += 1.   
+0000cff0: 2020 2020 2020 2020 206c 6973 7428 7265           list(re
+0000d000: 6373 290a 2020 2020 2020 2020 7769 7468  cs).        with
+0000d010: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000d020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d030: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
+0000d040: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
+0000d050: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
+0000d060: 2063 5f67 726f 7570 7329 0a0a 2020 2020   c_groups)..    
+0000d070: 2020 2020 7431 2e73 6f72 7428 2763 2729      t1.sort('c')
+0000d080: 0a20 2020 2020 2020 2063 5f67 726f 7570  .        c_group
+0000d090: 7320 3d20 300a 2020 2020 2020 2020 666f  s = 0.        fo
+0000d0a0: 7220 635f 7661 6c75 652c 2072 6563 7320  r c_value, recs 
+0000d0b0: 696e 2069 7465 7274 6f6f 6c73 2e67 726f  in itertools.gro
+0000d0c0: 7570 6279 2874 312c 206b 6579 3d6c 616d  upby(t1, key=lam
+0000d0d0: 6264 6120 7265 633a 2072 6563 2e63 293a  bda rec: rec.c):
+0000d0e0: 0a20 2020 2020 2020 2020 2020 2063 5f67  .            c_g
+0000d0f0: 726f 7570 7320 2b3d 2031 0a20 2020 2020  roups += 1.     
+0000d100: 2020 2020 2020 206c 6973 7428 7265 6373         list(recs
+0000d110: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000d120: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000d130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d140: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+0000d150: 5f73 697a 652c 2063 5f67 726f 7570 7329  _size, c_groups)
+0000d160: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000d170: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000d180: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000d190: 7373 6572 7445 7175 616c 2830 2c20 7431  ssertEqual(0, t1
+0000d1a0: 5b30 5d2e 6329 0a0a 2020 2020 2020 2020  [0].c)..        
+0000d1b0: 7431 2e73 6f72 7428 2763 2064 6573 6327  t1.sort('c desc'
+0000d1c0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000d1d0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000d1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d1f0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+0000d200: 5f73 697a 652d 312c 2074 315b 305d 2e63  _size-1, t1[0].c
+0000d210: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000d220: 736f 7274 3228 7365 6c66 293a 0a0a 2020  sort2(self):..  
+0000d230: 2020 2020 2020 726f 775f 7479 7065 203d        row_type =
+0000d240: 2074 7970 6528 7365 6c66 2e6d 616b 655f   type(self.make_
+0000d250: 6461 7461 5f6f 626a 6563 7428 302c 302c  data_object(0,0,
+0000d260: 3029 290a 2020 2020 2020 2020 7474 203d  0)).        tt =
+0000d270: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+0000d280: 696d 706f 7274 2874 6578 7477 7261 702e  import(textwrap.
+0000d290: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+0000d2a0: 2020 2020 612c 632c 620a 2020 2020 2020      a,c,b.      
+0000d2b0: 2020 312c 322c 310a 2020 2020 2020 2020    1,2,1.        
+0000d2c0: 322c 332c 300a 2020 2020 2020 2020 352c  2,3,0.        5,
+0000d2d0: 352c 2d31 0a20 2020 2020 2020 2033 2c34  5,-1.        3,4
+0000d2e0: 2c2d 310a 2020 2020 2020 2020 322c 342c  ,-1.        2,4,
+0000d2f0: 2d33 2222 2229 2c20 726f 775f 636c 6173  -3"""), row_clas
+0000d300: 733d 726f 775f 7479 7065 2c20 7472 616e  s=row_type, tran
+0000d310: 7366 6f72 6d73 3d64 6963 742e 6672 6f6d  sforms=dict.from
+0000d320: 6b65 7973 2822 6120 6220 6322 2e73 706c  keys("a b c".spl
+0000d330: 6974 2829 2c20 696e 7429 290a 0a20 2020  it(), int))..   
+0000d340: 2020 2020 2064 6566 2074 6f5f 7475 706c       def to_tupl
+0000d350: 6573 2874 293a 0a20 2020 2020 2020 2020  es(t):.         
+0000d360: 2020 2072 6574 7572 6e20 6c69 7374 286d     return list(m
+0000d370: 6170 2861 7474 7267 6574 7465 7228 2a74  ap(attrgetter(*t
+0000d380: 2e69 6e66 6f28 295b 2766 6965 6c64 7327  .info()['fields'
+0000d390: 5d29 2c20 7429 290a 0a20 2020 2020 2020  ]), t))..       
+0000d3a0: 2070 7269 6e74 2874 742e 696e 666f 2829   print(tt.info()
+0000d3b0: 5b27 6669 656c 6473 275d 290a 0a20 2020  ['fields'])..   
+0000d3c0: 2020 2020 2073 6f72 745f 6172 6720 3d20       sort_arg = 
+0000d3d0: 2263 2062 222e 7370 6c69 7428 290a 2020  "c b".split().  
+0000d3e0: 2020 2020 2020 7072 696e 7428 6622 536f        print(f"So
+0000d3f0: 7274 696e 6720 6279 207b 736f 7274 5f61  rting by {sort_a
+0000d400: 7267 2172 7d22 290a 2020 2020 2020 2020  rg!r}").        
+0000d410: 7474 2e73 6875 6666 6c65 2829 0a20 2020  tt.shuffle().   
+0000d420: 2020 2020 2074 742e 736f 7274 2873 6f72       tt.sort(sor
+0000d430: 745f 6172 6729 0a20 2020 2020 2020 2074  t_arg).        t
+0000d440: 315f 7475 706c 6573 203d 2074 6f5f 7475  1_tuples = to_tu
+0000d450: 706c 6573 2874 7429 0a20 2020 2020 2020  ples(tt).       
+0000d460: 2066 6f72 2074 2069 6e20 7431 5f74 7570   for t in t1_tup
+0000d470: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
+0000d480: 2070 7269 6e74 2874 290a 2020 2020 2020   print(t).      
+0000d490: 2020 7072 696e 7428 290a 0a20 2020 2020    print()..     
+0000d4a0: 2020 2074 742e 7368 7566 666c 6528 290a     tt.shuffle().
+0000d4b0: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
+0000d4c0: 2262 2229 0a20 2020 2020 2020 2074 742e  "b").        tt.
+0000d4d0: 736f 7274 2822 6322 290a 2020 2020 2020  sort("c").      
+0000d4e0: 2020 7432 5f74 7570 6c65 7320 3d20 746f    t2_tuples = to
+0000d4f0: 5f74 7570 6c65 7328 7474 290a 2020 2020  _tuples(tt).    
+0000d500: 2020 2020 666f 7220 7420 696e 2074 325f      for t in t2_
+0000d510: 7475 706c 6573 3a0a 2020 2020 2020 2020  tuples:.        
+0000d520: 2020 2020 7072 696e 7428 7429 0a20 2020      print(t).   
+0000d530: 2020 2020 2070 7269 6e74 2829 0a0a 2020       print()..  
+0000d540: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000d550: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+0000d560: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000d570: 7274 4571 7561 6c28 7431 5f74 7570 6c65  rtEqual(t1_tuple
+0000d580: 732c 2074 325f 7475 706c 6573 2c20 2266  s, t2_tuples, "f
+0000d590: 6169 6c65 6420 6d75 6c74 692d 6174 7472  ailed multi-attr
+0000d5a0: 6962 7574 6520 736f 7274 2c20 6769 7665  ibute sort, give
+0000d5b0: 6e20 6c69 7374 206f 6620 6174 7472 6962  n list of attrib
+0000d5c0: 7574 6573 2229 0a0a 2020 2020 2020 2020  utes")..        
+0000d5d0: 736f 7274 5f61 7267 203d 2022 632c 6222  sort_arg = "c,b"
+0000d5e0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+0000d5f0: 2253 6f72 7469 6e67 2062 7920 7b73 6f72  "Sorting by {sor
+0000d600: 745f 6172 6721 727d 2229 0a20 2020 2020  t_arg!r}").     
+0000d610: 2020 2074 742e 7368 7566 666c 6528 290a     tt.shuffle().
+0000d620: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
+0000d630: 736f 7274 5f61 7267 290a 2020 2020 2020  sort_arg).      
+0000d640: 2020 7431 5f74 7570 6c65 7320 3d20 746f    t1_tuples = to
+0000d650: 5f74 7570 6c65 7328 7474 290a 2020 2020  _tuples(tt).    
+0000d660: 2020 2020 666f 7220 7420 696e 2074 315f      for t in t1_
+0000d670: 7475 706c 6573 3a0a 2020 2020 2020 2020  tuples:.        
+0000d680: 2020 2020 7072 696e 7428 7429 0a20 2020      print(t).   
+0000d690: 2020 2020 2070 7269 6e74 2829 0a0a 2020       print()..  
+0000d6a0: 2020 2020 2020 7474 2e73 6875 6666 6c65        tt.shuffle
+0000d6b0: 2829 0a20 2020 2020 2020 2074 742e 736f  ().        tt.so
+0000d6c0: 7274 2822 6222 290a 2020 2020 2020 2020  rt("b").        
+0000d6d0: 7474 2e73 6f72 7428 2263 2229 0a20 2020  tt.sort("c").   
+0000d6e0: 2020 2020 2074 325f 7475 706c 6573 203d       t2_tuples =
+0000d6f0: 2074 6f5f 7475 706c 6573 2874 7429 0a20   to_tuples(tt). 
+0000d700: 2020 2020 2020 2066 6f72 2074 2069 6e20         for t in 
+0000d710: 7432 5f74 7570 6c65 733a 0a20 2020 2020  t2_tuples:.     
+0000d720: 2020 2020 2020 2070 7269 6e74 2874 290a         print(t).
+0000d730: 2020 2020 2020 2020 7072 696e 7428 290a          print().
+0000d740: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000d750: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000d760: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000d770: 7373 6572 7445 7175 616c 2874 315f 7475  ssertEqual(t1_tu
+0000d780: 706c 6573 2c20 7432 5f74 7570 6c65 732c  ples, t2_tuples,
+0000d790: 2022 6661 696c 6564 206d 756c 7469 2d61   "failed multi-a
+0000d7a0: 7474 7269 6275 7465 2073 6f72 742c 2067  ttribute sort, g
+0000d7b0: 6976 656e 2063 6f6d 6d61 2d73 6570 6172  iven comma-separ
+0000d7c0: 6174 6564 2061 7474 7269 6275 7465 7320  ated attributes 
+0000d7d0: 7374 7269 6e67 2229 0a0a 2020 2020 2020  string")..      
+0000d7e0: 2020 736f 7274 5f61 7267 203d 2022 632c    sort_arg = "c,
+0000d7f0: 6220 6465 7363 220a 2020 2020 2020 2020  b desc".        
+0000d800: 7072 696e 7428 6622 536f 7274 696e 6720  print(f"Sorting 
+0000d810: 6279 207b 736f 7274 5f61 7267 2172 7d22  by {sort_arg!r}"
+0000d820: 290a 2020 2020 2020 2020 7474 2e73 6875  ).        tt.shu
+0000d830: 6666 6c65 2829 0a20 2020 2020 2020 2074  ffle().        t
+0000d840: 742e 736f 7274 2873 6f72 745f 6172 6729  t.sort(sort_arg)
+0000d850: 0a20 2020 2020 2020 2074 315f 7475 706c  .        t1_tupl
+0000d860: 6573 203d 2074 6f5f 7475 706c 6573 2874  es = to_tuples(t
+0000d870: 7429 0a20 2020 2020 2020 2066 6f72 2074  t).        for t
+0000d880: 2069 6e20 7431 5f74 7570 6c65 733a 0a20   in t1_tuples:. 
+0000d890: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000d8a0: 2874 290a 2020 2020 2020 2020 7072 696e  (t).        prin
+0000d8b0: 7428 290a 0a20 2020 2020 2020 2074 742e  t()..        tt.
+0000d8c0: 7368 7566 666c 6528 290a 2020 2020 2020  shuffle().      
+0000d8d0: 2020 7474 2e73 6f72 7428 2262 2064 6573    tt.sort("b des
+0000d8e0: 6322 290a 2020 2020 2020 2020 7474 2e73  c").        tt.s
+0000d8f0: 6f72 7428 2263 2229 0a20 2020 2020 2020  ort("c").       
+0000d900: 2074 325f 7475 706c 6573 203d 2074 6f5f   t2_tuples = to_
+0000d910: 7475 706c 6573 2874 7429 0a20 2020 2020  tuples(tt).     
+0000d920: 2020 2066 6f72 2074 2069 6e20 7432 5f74     for t in t2_t
+0000d930: 7570 6c65 733a 0a20 2020 2020 2020 2020  uples:.         
+0000d940: 2020 2070 7269 6e74 2874 290a 2020 2020     print(t).    
+0000d950: 2020 2020 7072 696e 7428 290a 0a20 2020      print()..   
+0000d960: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000d970: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000d980: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000d990: 7445 7175 616c 2874 315f 7475 706c 6573  tEqual(t1_tuples
+0000d9a0: 2c20 7432 5f74 7570 6c65 732c 2022 6661  , t2_tuples, "fa
+0000d9b0: 696c 6564 206d 6978 6564 2061 7363 656e  iled mixed ascen
+0000d9c0: 6469 6e67 2f64 6573 6365 6e64 696e 6720  ding/descending 
+0000d9d0: 6d75 6c74 692d 6174 7472 6962 7574 6520  multi-attribute 
+0000d9e0: 736f 7274 2229 0a0a 2020 2020 6465 6620  sort")..    def 
+0000d9f0: 7465 7374 5f73 6f72 7433 2873 656c 6629  test_sort3(self)
+0000da00: 3a0a 2020 2020 2020 2020 656d 706c 6f79  :.        employ
+0000da10: 6565 7320 3d20 6c74 2e54 6162 6c65 2829  ees = lt.Table()
+0000da20: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
+0000da30: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+0000da40: 0a20 2020 2020 2020 2020 2020 2065 6d70  .            emp
+0000da50: 5f69 642c 6e61 6d65 2c64 6570 742c 7361  _id,name,dept,sa
+0000da60: 6c61 7279 2c63 6f6d 6d69 7373 696f 6e0a  lary,commission.
+0000da70: 2020 2020 2020 2020 2020 2020 3030 3031              0001
+0000da80: 2c41 6c69 6365 2c53 616c 6573 2c35 3030  ,Alice,Sales,500
+0000da90: 3030 2c30 2e35 0a20 2020 2020 2020 2020  00,0.5.         
+0000daa0: 2020 2030 3030 322c 426f 622c 456e 6769     0002,Bob,Engi
+0000dab0: 6e65 6572 696e 672c 3130 3030 3030 2c0a  neering,100000,.
+0000dac0: 2020 2020 2020 2020 2020 2020 3030 3033              0003
+0000dad0: 2c43 6861 726c 6573 2c53 616c 6573 2c34  ,Charles,Sales,4
+0000dae0: 3530 3030 2c30 2e37 0a20 2020 2020 2020  5000,0.7.       
+0000daf0: 2020 2020 2030 3030 342c 4461 7665 2c53       0004,Dave,S
+0000db00: 616c 6573 2c34 3530 3030 2c30 2e36 0a20  ales,45000,0.6. 
+0000db10: 2020 2020 2020 2020 2020 2030 3030 352c             0005,
+0000db20: 456d 696c 792c 5361 6c65 732c 3530 3030  Emily,Sales,5000
+0000db30: 302c 302e 340a 2020 2020 2020 2020 2020  0,0.4.          
+0000db40: 2020 2222 2229 2c20 7472 616e 7366 6f72    """), transfor
+0000db50: 6d73 3d7b 2273 616c 6172 7922 3a20 696e  ms={"salary": in
+0000db60: 742c 2022 636f 6d6d 6973 7369 6f6e 223a  t, "commission":
+0000db70: 2066 6c6f 6174 7d29 0a0a 2020 2020 2020   float})..      
+0000db80: 2020 7361 6c65 735f 656d 706c 6f79 6565    sales_employee
+0000db90: 7320 3d20 656d 706c 6f79 6565 732e 7768  s = employees.wh
+0000dba0: 6572 6528 6465 7074 3d22 5361 6c65 7322  ere(dept="Sales"
+0000dbb0: 292e 736f 7274 2822 7361 6c61 7279 2064  ).sort("salary d
+0000dbc0: 6573 632c 636f 6d6d 6973 7369 6f6e 2229  esc,commission")
+0000dbd0: 0a0a 2020 2020 2020 2020 7361 6c65 735f  ..        sales_
+0000dbe0: 656d 706c 6f79 6565 732e 7072 6573 656e  employees.presen
+0000dbf0: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
+0000dc00: 7428 6c69 7374 2873 616c 6573 5f65 6d70  t(list(sales_emp
+0000dc10: 6c6f 7965 6573 2e61 6c6c 2e65 6d70 5f69  loyees.all.emp_i
+0000dc20: 6429 290a 0a20 2020 2020 2020 2077 6974  d))..        wit
+0000dc30: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000dc40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dc50: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+0000dc60: 2730 3030 3527 2c20 2730 3030 3127 2c20  '0005', '0001', 
+0000dc70: 2730 3030 3427 2c20 2730 3030 3327 5d2c  '0004', '0003'],
+0000dc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000dca0: 7374 2873 616c 6573 5f65 6d70 6c6f 7965  st(sales_employe
+0000dcb0: 6573 2e61 6c6c 2e65 6d70 5f69 6429 290a  es.all.emp_id)).
+0000dcc0: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
+0000dcd0: 6971 7565 2873 656c 6629 3a0a 2020 2020  ique(self):.    
+0000dce0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+0000dcf0: 3130 0a20 2020 2020 2020 2074 3120 3d20  10.        t1 = 
+0000dd00: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+0000dd10: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+0000dd20: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+0000dd30: 290a 0a20 2020 2020 2020 2074 3220 3d20  )..        t2 = 
+0000dd40: 7431 2e75 6e69 7175 6528 290a 2020 2020  t1.unique().    
+0000dd50: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000dd60: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000dd70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000dd80: 4571 7561 6c28 6c65 6e28 7431 292c 206c  Equal(len(t1), l
+0000dd90: 656e 2874 3229 290a 0a20 2020 2020 2020  en(t2))..       
+0000dda0: 2074 3320 3d20 7431 2e75 6e69 7175 6528   t3 = t1.unique(
+0000ddb0: 6b65 793d 6c61 6d62 6461 2072 6563 3a20  key=lambda rec: 
+0000ddc0: 7265 632e 6329 0a20 2020 2020 2020 2077  rec.c).        w
+0000ddd0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000dde0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000ddf0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000de00: 2874 6573 745f 7369 7a65 2c20 6c65 6e28  (test_size, len(
+0000de10: 7433 2929 0a0a 0a40 6d61 6b65 5f74 6573  t3))...@make_tes
+0000de20: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
+0000de30: 5461 626c 654f 7574 7075 7454 6573 7473  TableOutputTests
+0000de40: 3a0a 2020 2020 6465 6620 7465 7374 5f62  :.    def test_b
+0000de50: 6173 6963 5f70 7265 7365 6e74 2873 656c  asic_present(sel
+0000de60: 6629 3a0a 2020 2020 2020 2020 6966 2072  f):.        if r
+0000de70: 6963 6820 6973 204e 6f6e 653a 0a20 2020  ich is None:.   
+0000de80: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
+0000de90: 7761 726e 696e 6773 0a20 2020 2020 2020  warnings.       
+0000dea0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+0000deb0: 726e 2822 7269 6368 206e 6f74 2069 6e73  rn("rich not ins
+0000dec0: 7461 6c6c 6564 2c20 6361 6e6e 6f74 2072  talled, cannot r
+0000ded0: 756e 2074 6573 7422 290a 2020 2020 2020  un test").      
+0000dee0: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+0000def0: 2020 2020 2020 6672 6f6d 2072 6963 6820        from rich 
+0000df00: 696d 706f 7274 2062 6f78 0a20 2020 2020  import box.     
+0000df10: 2020 2066 726f 6d20 696f 2069 6d70 6f72     from io impor
+0000df20: 7420 5374 7269 6e67 494f 0a20 2020 2020  t StringIO.     
+0000df30: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
+0000df40: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+0000df50: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000df60: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000df70: 2020 612c 620a 2020 2020 2020 2020 2020    a,b.          
+0000df80: 2020 3130 2c31 3030 0a20 2020 2020 2020    10,100.       
+0000df90: 2020 2020 2032 302c 3230 300a 2020 2020       20,200.    
+0000dfa0: 2020 2020 2020 2020 2222 2229 290a 2020          """)).  
+0000dfb0: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
+0000dfc0: 656e 7428 290a 2020 2020 2020 2020 6f75  ent().        ou
+0000dfd0: 7420 3d20 5374 7269 6e67 494f 2829 0a20  t = StringIO(). 
+0000dfe0: 2020 2020 2020 2074 6162 6c65 2e70 7265         table.pre
+0000dff0: 7365 6e74 2866 696c 653d 6f75 742c 2062  sent(file=out, b
+0000e000: 6f78 3d62 6f78 2e41 5343 4949 290a 2020  ox=box.ASCII).  
+0000e010: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+0000e020: 2074 6578 7477 7261 702e 6465 6465 6e74   textwrap.dedent
+0000e030: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000e040: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20    +----------+. 
+0000e050: 2020 2020 2020 2020 2020 207c 2041 2020             | A  
+0000e060: 7c20 4220 2020 7c0a 2020 2020 2020 2020  | B   |.        
+0000e070: 2020 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d7c      |----+-----|
+0000e080: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000e090: 3020 7c20 3130 3020 7c0a 2020 2020 2020  0 | 100 |.      
+0000e0a0: 2020 2020 2020 7c20 3230 207c 2032 3030        | 20 | 200
+0000e0b0: 207c 0a20 2020 2020 2020 2020 2020 202b   |.            +
+0000e0c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
+0000e0d0: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
+0000e0e0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000e0f0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000e100: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e110: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
+0000e120: 206f 7574 2e67 6574 7661 6c75 6528 2929   out.getvalue())
+0000e130: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
+0000e140: 2062 7567 6669 7820 7768 656e 2074 6162   bugfix when tab
+0000e150: 6c65 2068 6173 2061 7474 7269 6275 7465  le has attribute
+0000e160: 2022 6465 6661 756c 7422 0a20 2020 2020   "default".     
+0000e170: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
+0000e180: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+0000e190: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000e1a0: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000e1b0: 2020 612c 622c 6465 6661 756c 740a 2020    a,b,default.  
+0000e1c0: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
+0000e1d0: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
+0000e1e0: 2020 2020 3135 2c31 3530 2c0a 2020 2020      15,150,.    
+0000e1f0: 2020 2020 2020 2020 3230 2c32 3030 2c6f          20,200,o
+0000e200: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
+0000e210: 2020 2222 2229 290a 2020 2020 2020 2020    """)).        
+0000e220: 7461 626c 652e 7072 6573 656e 7428 290a  table.present().
+0000e230: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
+0000e240: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
+0000e250: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
+0000e260: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
+0000e270: 2e41 5343 4949 290a 2020 2020 2020 2020  .ASCII).        
+0000e280: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
+0000e290: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000e2a0: 2020 2020 2020 2020 2020 2020 2b2d 2d2d              +---
+0000e2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e2c0: 2d2b 0a20 2020 2020 2020 2020 2020 207c  -+.            |
+0000e2d0: 2041 2020 7c20 4220 2020 7c20 4465 6661   A  | B   | Defa
+0000e2e0: 756c 7420 7c0a 2020 2020 2020 2020 2020  ult |.          
+0000e2f0: 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d    |----+-----+--
+0000e300: 2d2d 2d2d 2d2d 2d7c 0a20 2020 2020 2020  -------|.       
+0000e310: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
+0000e320: 7c20 7075 7270 6c65 2020 7c0a 2020 2020  | purple  |.    
+0000e330: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
+0000e340: 3530 207c 2020 2020 2020 2020 207c 0a20  50 |         |. 
+0000e350: 2020 2020 2020 2020 2020 207c 2032 3020             | 20 
+0000e360: 7c20 3230 3020 7c20 6f72 616e 6765 2020  | 200 | orange  
+0000e370: 7c0a 2020 2020 2020 2020 2020 2020 2b2d  |.            +-
+0000e380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e390: 2d2d 2d2b 0a20 2020 2020 2020 2020 2020  ---+.           
+0000e3a0: 2022 2222 290a 2020 2020 2020 2020 7769   """).        wi
+0000e3b0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000e3c0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000e3d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000e3e0: 6578 7065 6374 6564 2c20 6f75 742e 6765  expected, out.ge
+0000e3f0: 7476 616c 7565 2829 290a 0a20 2020 2020  tvalue())..     
+0000e400: 2020 2023 2074 6573 7420 6772 6f75 7062     # test groupb
+0000e410: 790a 2020 2020 2020 2020 7461 626c 6520  y.        table 
+0000e420: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+0000e430: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
+0000e440: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000e450: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
+0000e460: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
+0000e470: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
+0000e480: 2020 2020 2020 2020 2020 2031 352c 3135             15,15
+0000e490: 302c 7075 7270 6c65 0a20 2020 2020 2020  0,purple.       
+0000e4a0: 2020 2020 2032 302c 3230 302c 6f72 616e       20,200,oran
+0000e4b0: 6765 0a20 2020 2020 2020 2020 2020 2022  ge.            "
+0000e4c0: 2222 2929 0a20 2020 2020 2020 2074 6162  "")).        tab
+0000e4d0: 6c65 2e70 7265 7365 6e74 2829 0a20 2020  le.present().   
+0000e4e0: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
+0000e4f0: 6e74 2862 6f78 3d62 6f78 2e41 5343 4949  nt(box=box.ASCII
+0000e500: 2c20 6772 6f75 7062 793d 2264 6566 6175  , groupby="defau
+0000e510: 6c74 2229 0a20 2020 2020 2020 206f 7574  lt").        out
+0000e520: 203d 2053 7472 696e 6749 4f28 290a 2020   = StringIO().  
+0000e530: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
+0000e540: 656e 7428 6669 6c65 3d6f 7574 2c20 626f  ent(file=out, bo
+0000e550: 783d 626f 782e 4153 4349 492c 2067 726f  x=box.ASCII, gro
+0000e560: 7570 6279 3d22 6465 6661 756c 7422 290a  upby="default").
+0000e570: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+0000e580: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+0000e590: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000e5a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d      +-----------
+0000e5b0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
+0000e5c0: 2020 2020 2020 207c 2041 2020 7c20 4220         | A  | B 
+0000e5d0: 2020 7c20 4465 6661 756c 7420 7c0a 2020    | Default |.  
+0000e5e0: 2020 2020 2020 2020 2020 7c2d 2d2d 2d2b            |----+
+0000e5f0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c  -----+---------|
+0000e600: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000e610: 3020 7c20 3130 3020 7c20 7075 7270 6c65  0 | 100 | purple
+0000e620: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000e630: 7c20 3135 207c 2031 3530 207c 2020 2020  | 15 | 150 |    
+0000e640: 2020 2020 207c 0a20 2020 2020 2020 2020       |.         
+0000e650: 2020 207c 2032 3020 7c20 3230 3020 7c20     | 20 | 200 | 
+0000e660: 6f72 616e 6765 2020 7c0a 2020 2020 2020  orange  |.      
+0000e670: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+0000e680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020  -----------+.   
+0000e690: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
+0000e6a0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000e6b0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+0000e6c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000e6d0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0000e6e0: 2c20 6f75 742e 6765 7476 616c 7565 2829  , out.getvalue()
+0000e6f0: 290a 0a20 2020 2020 2020 2074 6162 6c65  )..        table
+0000e700: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+0000e710: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
+0000e720: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000e730: 2020 2020 2020 2020 2020 612c 622c 6465            a,b,de
+0000e740: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
+0000e750: 2020 3130 2c31 3030 2c70 7572 706c 650a    10,100,purple.
+0000e760: 2020 2020 2020 2020 2020 2020 3135 2c31              15,1
+0000e770: 3530 2c70 7572 706c 650a 2020 2020 2020  50,purple.      
+0000e780: 2020 2020 2020 3135 2c32 3030 2c6f 7261        15,200,ora
+0000e790: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
+0000e7a0: 3135 2c32 3530 2c6f 7261 6e67 650a 2020  15,250,orange.  
+0000e7b0: 2020 2020 2020 2020 2020 3230 2c32 3530            20,250
+0000e7c0: 2c6f 7261 6e67 650a 2020 2020 2020 2020  ,orange.        
+0000e7d0: 2020 2020 2222 2229 290a 2020 2020 2020      """)).      
+0000e7e0: 2020 7461 626c 652e 7072 6573 656e 7428    table.present(
+0000e7f0: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+0000e800: 7072 6573 656e 7428 626f 783d 626f 782e  present(box=box.
+0000e810: 4153 4349 492c 2067 726f 7570 6279 3d22  ASCII, groupby="
+0000e820: 6465 6661 756c 7420 6122 290a 2020 2020  default a").    
+0000e830: 2020 2020 6f75 7420 3d20 5374 7269 6e67      out = String
+0000e840: 494f 2829 0a20 2020 2020 2020 2074 6162  IO().        tab
+0000e850: 6c65 2e70 7265 7365 6e74 2866 696c 653d  le.present(file=
+0000e860: 6f75 742c 2062 6f78 3d62 6f78 2e41 5343  out, box=box.ASC
+0000e870: 4949 2c20 6772 6f75 7062 793d 2264 6566  II, groupby="def
+0000e880: 6175 6c74 2061 2229 0a20 2020 2020 2020  ault a").       
+0000e890: 2065 7870 6563 7465 6420 3d20 7465 7874   expected = text
+0000e8a0: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+0000e8b0: 0a20 2020 2020 2020 2020 2020 202b 2d2d  .            +--
+0000e8c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e8d0: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
+0000e8e0: 7c20 4120 207c 2042 2020 207c 2044 6566  | A  | B   | Def
+0000e8f0: 6175 6c74 207c 0a20 2020 2020 2020 2020  ault |.         
+0000e900: 2020 207c 2d2d 2d2d 2b2d 2d2d 2d2d 2b2d     |----+-----+-
+0000e910: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 2020  --------|.      
+0000e920: 2020 2020 2020 7c20 3130 207c 2031 3030        | 10 | 100
+0000e930: 207c 2070 7572 706c 6520 207c 0a20 2020   | purple  |.   
+0000e940: 2020 2020 2020 2020 207c 2031 3520 7c20           | 15 | 
+0000e950: 3135 3020 7c20 2020 2020 2020 2020 7c0a  150 |         |.
+0000e960: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+0000e970: 207c 2032 3030 207c 206f 7261 6e67 6520   | 200 | orange 
+0000e980: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
+0000e990: 2020 2020 7c20 3235 3020 7c20 2020 2020      | 250 |     
+0000e9a0: 2020 2020 7c0a 2020 2020 2020 2020 2020      |.          
+0000e9b0: 2020 7c20 3230 207c 2032 3530 207c 2020    | 20 | 250 |  
+0000e9c0: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
+0000e9d0: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
+0000e9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
+0000e9f0: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
+0000ea00: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000ea10: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000ea20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ea30: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
+0000ea40: 206f 7574 2e67 6574 7661 6c75 6528 2929   out.getvalue())
+0000ea50: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
+0000ea60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+0000ea70: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
+0000ea80: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000ea90: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
+0000eaa0: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
+0000eab0: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
+0000eac0: 2020 2020 2020 2020 2020 2031 352c 3230             15,20
+0000ead0: 302c 6f72 616e 6765 0a20 2020 2020 2020  0,orange.       
+0000eae0: 2020 2020 2031 352c 3135 302c 7075 7270       15,150,purp
+0000eaf0: 6c65 0a20 2020 2020 2020 2020 2020 2032  le.            2
+0000eb00: 302c 3235 302c 6f72 616e 6765 0a20 2020  0,250,orange.   
+0000eb10: 2020 2020 2020 2020 2031 352c 3235 302c           15,250,
+0000eb20: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
+0000eb30: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
+0000eb40: 2074 6162 6c65 2e73 6f72 7428 2264 6566   table.sort("def
+0000eb50: 6175 6c74 2064 6573 632c 6122 290a 2020  ault desc,a").  
+0000eb60: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
+0000eb70: 656e 7428 290a 2020 2020 2020 2020 7461  ent().        ta
+0000eb80: 626c 652e 7072 6573 656e 7428 626f 783d  ble.present(box=
+0000eb90: 626f 782e 4153 4349 492c 2067 726f 7570  box.ASCII, group
+0000eba0: 6279 3d22 6465 6661 756c 7420 6122 290a  by="default a").
+0000ebb0: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
+0000ebc0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
+0000ebd0: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
+0000ebe0: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
+0000ebf0: 2e41 5343 4949 2c20 6772 6f75 7062 793d  .ASCII, groupby=
+0000ec00: 2264 6566 6175 6c74 2061 2229 0a20 2020  "default a").   
+0000ec10: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+0000ec20: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000ec30: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000ec40: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
+0000ec50: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+0000ec60: 2020 2020 7c20 4120 207c 2042 2020 207c      | A  | B   |
+0000ec70: 2044 6566 6175 6c74 207c 0a20 2020 2020   Default |.     
+0000ec80: 2020 2020 2020 207c 2d2d 2d2d 2b2d 2d2d         |----+---
+0000ec90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  --+---------|.  
+0000eca0: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
+0000ecb0: 2031 3030 207c 2070 7572 706c 6520 207c   100 | purple  |
+0000ecc0: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000ecd0: 3520 7c20 3135 3020 7c20 2020 2020 2020  5 | 150 |       
+0000ece0: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000ecf0: 7c20 3135 207c 2032 3030 207c 206f 7261  | 15 | 200 | ora
+0000ed00: 6e67 6520 207c 0a20 2020 2020 2020 2020  nge  |.         
+0000ed10: 2020 207c 2020 2020 7c20 3235 3020 7c20     |    | 250 | 
+0000ed20: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
+0000ed30: 2020 2020 2020 7c20 3230 207c 2032 3530        | 20 | 250
+0000ed40: 207c 2020 2020 2020 2020 207c 0a20 2020   |         |.   
+0000ed50: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
+0000ed60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+0000ed70: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000ed80: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000ed90: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000eda0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000edb0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000edc0: 7465 642c 206f 7574 2e67 6574 7661 6c75  ted, out.getvalu
+0000edd0: 6528 2929 0a0a 2020 2020 6465 6620 7465  e())..    def te
+0000ede0: 7374 5f6d 6172 6b64 6f77 6e28 7365 6c66  st_markdown(self
+0000edf0: 293a 0a20 2020 2020 2020 2074 6162 6c65  ):.        table
+0000ee00: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+0000ee10: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
+0000ee20: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000ee30: 2020 2020 2020 2020 2020 612c 620a 2020            a,b.  
+0000ee40: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
+0000ee50: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
+0000ee60: 3230 300a 2020 2020 2020 2020 2020 2020  200.            
+0000ee70: 2222 2229 290a 2020 2020 2020 2020 6f75  """)).        ou
+0000ee80: 745f 6d61 726b 646f 776e 203d 2074 6162  t_markdown = tab
+0000ee90: 6c65 2e61 735f 6d61 726b 646f 776e 2829  le.as_markdown()
+0000eea0: 0a20 2020 2020 2020 2070 7269 6e74 286f  .        print(o
+0000eeb0: 7574 5f6d 6172 6b64 6f77 6e29 0a20 2020  ut_markdown).   
+0000eec0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+0000eed0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000eee0: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000eef0: 207c 2061 207c 2062 207c 0a20 2020 2020   | a | b |.     
+0000ef00: 2020 2020 2020 207c 2d2d 2d7c 2d2d 2d7c         |---|---|
+0000ef10: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000ef20: 3020 7c20 3130 3020 7c0a 2020 2020 2020  0 | 100 |.      
+0000ef30: 2020 2020 2020 7c20 3230 207c 2032 3030        | 20 | 200
+0000ef40: 207c 0a20 2020 2020 2020 2020 2020 2022   |.            "
+0000ef50: 2222 290a 2020 2020 2020 2020 7769 7468  "").        with
+0000ef60: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000ef70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ef80: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+0000ef90: 7065 6374 6564 2c20 6f75 745f 6d61 726b  pected, out_mark
+0000efa0: 646f 776e 290a 0a20 2020 2020 2020 2023  down)..        #
+0000efb0: 2074 6573 7420 6275 6766 6978 2077 6865   test bugfix whe
+0000efc0: 6e20 7461 626c 6520 6861 7320 6174 7472  n table has attr
+0000efd0: 6962 7574 6520 2264 6566 6175 6c74 220a  ibute "default".
+0000efe0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+0000eff0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+0000f000: 6d70 6f72 7428 7465 7874 7772 6170 2e64  mport(textwrap.d
+0000f010: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
+0000f020: 2020 2020 2020 2061 2c62 2c64 6566 6175         a,b,defau
+0000f030: 6c74 0a20 2020 2020 2020 2020 2020 2031  lt.            1
+0000f040: 302c 3130 302c 7075 7270 6c65 0a20 2020  0,100,purple.   
+0000f050: 2020 2020 2020 2020 2031 352c 3135 302c           15,150,
+0000f060: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
+0000f070: 3230 302c 6f72 616e 6765 0a20 2020 2020  200,orange.     
+0000f080: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
+0000f090: 2020 2020 206f 7574 5f6d 6172 6b64 6f77       out_markdow
+0000f0a0: 6e20 3d20 7461 626c 652e 6173 5f6d 6172  n = table.as_mar
+0000f0b0: 6b64 6f77 6e28 290a 2020 2020 2020 2020  kdown().        
+0000f0c0: 7072 696e 7428 6f75 745f 6d61 726b 646f  print(out_markdo
+0000f0d0: 776e 290a 2020 2020 2020 2020 6578 7065  wn).        expe
+0000f0e0: 6374 6564 203d 2074 6578 7477 7261 702e  cted = textwrap.
+0000f0f0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+0000f100: 2020 2020 2020 2020 7c20 6120 7c20 6220          | a | b 
+0000f110: 7c20 6465 6661 756c 7420 7c0a 2020 2020  | default |.    
+0000f120: 2020 2020 2020 2020 7c2d 2d2d 7c2d 2d2d          |---|---
+0000f130: 7c2d 2d2d 7c0a 2020 2020 2020 2020 2020  |---|.          
+0000f140: 2020 7c20 3130 207c 2031 3030 207c 2070    | 10 | 100 | p
+0000f150: 7572 706c 6520 7c0a 2020 2020 2020 2020  urple |.        
+0000f160: 2020 2020 7c20 3135 207c 2031 3530 207c      | 15 | 150 |
+0000f170: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000f180: 7c20 3230 207c 2032 3030 207c 206f 7261  | 20 | 200 | ora
+0000f190: 6e67 6520 7c0a 2020 2020 2020 2020 2020  nge |.          
+0000f1a0: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
+0000f1b0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000f1c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f1d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000f1e0: 2865 7870 6563 7465 642c 206f 7574 5f6d  (expected, out_m
+0000f1f0: 6172 6b64 6f77 6e29 0a0a 2020 2020 2020  arkdown)..      
+0000f200: 2020 2320 7465 7374 2067 726f 7570 696e    # test groupin
+0000f210: 6720 696e 2061 735f 6d61 726b 646f 776e  g in as_markdown
+0000f220: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+0000f230: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+0000f240: 696d 706f 7274 2874 6578 7477 7261 702e  import(textwrap.
+0000f250: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+0000f260: 2020 2020 2020 2020 612c 622c 6465 6661          a,b,defa
+0000f270: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
+0000f280: 3130 2c31 3030 2c70 7572 706c 650a 2020  10,100,purple.  
+0000f290: 2020 2020 2020 2020 2020 3135 2c31 3530            15,150
+0000f2a0: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
+0000f2b0: 2020 2020 3230 2c32 3030 2c6f 7261 6e67      20,200,orang
+0000f2c0: 650a 2020 2020 2020 2020 2020 2020 2222  e.            ""
+0000f2d0: 2229 290a 2020 2020 2020 2020 6f75 745f  ")).        out_
+0000f2e0: 6d61 726b 646f 776e 203d 2074 6162 6c65  markdown = table
+0000f2f0: 2e61 735f 6d61 726b 646f 776e 2867 726f  .as_markdown(gro
+0000f300: 7570 6279 3d22 6465 6661 756c 7422 290a  upby="default").
+0000f310: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
+0000f320: 745f 6d61 726b 646f 776e 290a 2020 2020  t_markdown).    
+0000f330: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
+0000f340: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+0000f350: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
+0000f360: 7c20 6120 7c20 6220 7c20 6465 6661 756c  | a | b | defaul
+0000f370: 7420 7c0a 2020 2020 2020 2020 2020 2020  t |.            
+0000f380: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a 2020  |---|---|---|.  
+0000f390: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
+0000f3a0: 2031 3030 207c 2070 7572 706c 6520 7c0a   100 | purple |.
+0000f3b0: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+0000f3c0: 207c 2031 3530 207c 2020 7c0a 2020 2020   | 150 |  |.    
+0000f3d0: 2020 2020 2020 2020 7c20 3230 207c 2032          | 20 | 2
+0000f3e0: 3030 207c 206f 7261 6e67 6520 7c0a 2020  00 | orange |.  
+0000f3f0: 2020 2020 2020 2020 2020 2222 2229 0a20            """). 
+0000f400: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000f410: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000f420: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000f430: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0000f440: 642c 206f 7574 5f6d 6172 6b64 6f77 6e29  d, out_markdown)
+0000f450: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
+0000f460: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+0000f470: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
+0000f480: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000f490: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
+0000f4a0: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
+0000f4b0: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
+0000f4c0: 2020 2020 2020 2020 2020 2031 352c 3230             15,20
+0000f4d0: 302c 6f72 616e 6765 0a20 2020 2020 2020  0,orange.       
+0000f4e0: 2020 2020 2031 352c 3135 302c 7075 7270       15,150,purp
+0000f4f0: 6c65 0a20 2020 2020 2020 2020 2020 2032  le.            2
+0000f500: 302c 3235 302c 6f72 616e 6765 0a20 2020  0,250,orange.   
+0000f510: 2020 2020 2020 2020 2031 352c 3235 302c           15,250,
+0000f520: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
+0000f530: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
+0000f540: 2074 6162 6c65 2e73 6f72 7428 2264 6566   table.sort("def
+0000f550: 6175 6c74 2064 6573 632c 6122 290a 2020  ault desc,a").  
+0000f560: 2020 2020 2020 6f75 745f 6d61 726b 646f        out_markdo
+0000f570: 776e 203d 2074 6162 6c65 2e61 735f 6d61  wn = table.as_ma
+0000f580: 726b 646f 776e 2867 726f 7570 6279 3d22  rkdown(groupby="
+0000f590: 6465 6661 756c 7420 6122 290a 2020 2020  default a").    
+0000f5a0: 2020 2020 7072 696e 7428 6f75 745f 6d61      print(out_ma
+0000f5b0: 726b 646f 776e 290a 2020 2020 2020 2020  rkdown).        
+0000f5c0: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
+0000f5d0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000f5e0: 2020 2020 2020 2020 2020 2020 7c20 6120              | a 
+0000f5f0: 7c20 6220 7c20 6465 6661 756c 7420 7c0a  | b | default |.
+0000f600: 2020 2020 2020 2020 2020 2020 7c2d 2d2d              |---
+0000f610: 7c2d 2d2d 7c2d 2d2d 7c0a 2020 2020 2020  |---|---|.      
+0000f620: 2020 2020 2020 7c20 3130 207c 2031 3030        | 10 | 100
+0000f630: 207c 2070 7572 706c 6520 7c0a 2020 2020   | purple |.    
+0000f640: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
+0000f650: 3530 207c 2020 7c0a 2020 2020 2020 2020  50 |  |.        
+0000f660: 2020 2020 7c20 3135 207c 2032 3030 207c      | 15 | 200 |
+0000f670: 206f 7261 6e67 6520 7c0a 2020 2020 2020   orange |.      
+0000f680: 2020 2020 2020 7c20 207c 2032 3530 207c        |  | 250 |
+0000f690: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000f6a0: 7c20 3230 207c 2032 3530 207c 2020 7c0a  | 20 | 250 |  |.
+0000f6b0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000f6c0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000f6d0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000f6e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000f6f0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000f700: 7465 642c 206f 7574 5f6d 6172 6b64 6f77  ted, out_markdow
+0000f710: 6e29 0a0a 2320 7361 6d70 6c65 2069 6d70  n)..# sample imp
+0000f720: 6f72 7420 6461 7461 2073 6574 730a 6373  ort data sets.cs
+0000f730: 765f 6461 7461 203d 2022 2222 5c0a 612c  v_data = """\.a,
+0000f740: 622c 630a 302c 302c 300a 302c 302c 310a  b,c.0,0,0.0,0,1.
+0000f750: 302c 302c 320a 302c 312c 300a 302c 312c  0,0,2.0,1,0.0,1,
+0000f760: 310a 302c 312c 320a 302c 322c 300a 302c  1.0,1,2.0,2,0.0,
+0000f770: 322c 310a 302c 322c 320a 312c 302c 300a  2,1.0,2,2.1,0,0.
+0000f780: 312c 302c 310a 312c 302c 320a 312c 312c  1,0,1.1,0,2.1,1,
+0000f790: 300a 312c 312c 310a 312c 312c 320a 312c  0.1,1,1.1,1,2.1,
+0000f7a0: 322c 300a 312c 322c 310a 312c 322c 320a  2,0.1,2,1.1,2,2.
+0000f7b0: 322c 302c 300a 322c 302c 310a 322c 302c  2,0,0.2,0,1.2,0,
+0000f7c0: 320a 322c 312c 300a 322c 312c 310a 322c  2.2,1,0.2,1,1.2,
+0000f7d0: 312c 320a 322c 322c 300a 322c 322c 310a  1,2.2,2,0.2,2,1.
+0000f7e0: 322c 322c 320a 0a22 2222 0a0a 6a73 6f6e  2,2,2.."""..json
+0000f7f0: 5f64 6174 6120 3d20 2222 225c 0a20 2020  _data = """\.   
+0000f800: 207b 2261 223a 2030 2c20 2262 223a 2030   {"a": 0, "b": 0
+0000f810: 2c20 2263 223a 2030 7d0a 2020 2020 7b22  , "c": 0}.    {"
+0000f820: 6122 3a20 302c 2022 6222 3a20 302c 2022  a": 0, "b": 0, "
+0000f830: 6322 3a20 317d 0a20 2020 207b 2261 223a  c": 1}.    {"a":
+0000f840: 2030 2c20 2262 223a 2030 2c20 2263 223a   0, "b": 0, "c":
+0000f850: 2032 7d0a 2020 2020 7b22 6122 3a20 302c   2}.    {"a": 0,
+0000f860: 2022 6222 3a20 312c 2022 6322 3a20 307d   "b": 1, "c": 0}
+0000f870: 0a20 2020 207b 2261 223a 2030 2c20 2262  .    {"a": 0, "b
+0000f880: 223a 2031 2c20 2263 223a 2031 7d0a 2020  ": 1, "c": 1}.  
+0000f890: 2020 7b22 6122 3a20 302c 2022 6222 3a20    {"a": 0, "b": 
+0000f8a0: 312c 2022 6322 3a20 327d 0a20 2020 207b  1, "c": 2}.    {
+0000f8b0: 2261 223a 2030 2c20 2262 223a 2032 2c20  "a": 0, "b": 2, 
+0000f8c0: 2263 223a 2030 7d0a 2020 2020 7b22 6122  "c": 0}.    {"a"
+0000f8d0: 3a20 302c 2022 6222 3a20 322c 2022 6322  : 0, "b": 2, "c"
+0000f8e0: 3a20 317d 0a20 2020 207b 2261 223a 2030  : 1}.    {"a": 0
+0000f8f0: 2c20 2262 223a 2032 2c20 2263 223a 2032  , "b": 2, "c": 2
+0000f900: 7d0a 2020 2020 7b22 6122 3a20 312c 2022  }.    {"a": 1, "
+0000f910: 6222 3a20 302c 2022 6322 3a20 307d 0a20  b": 0, "c": 0}. 
+0000f920: 2020 207b 2261 223a 2031 2c20 2262 223a     {"a": 1, "b":
+0000f930: 2030 2c20 2263 223a 2031 7d0a 2020 2020   0, "c": 1}.    
+0000f940: 7b22 6122 3a20 312c 2022 6222 3a20 302c  {"a": 1, "b": 0,
+0000f950: 2022 6322 3a20 327d 0a20 2020 207b 2261   "c": 2}.    {"a
+0000f960: 223a 2031 2c20 2262 223a 2031 2c20 2263  ": 1, "b": 1, "c
+0000f970: 223a 2030 7d0a 2020 2020 7b22 6122 3a20  ": 0}.    {"a": 
+0000f980: 312c 2022 6222 3a20 312c 2022 6322 3a20  1, "b": 1, "c": 
+0000f990: 317d 0a20 2020 207b 2261 223a 2031 2c20  1}.    {"a": 1, 
+0000f9a0: 2262 223a 2031 2c20 2263 223a 2032 7d0a  "b": 1, "c": 2}.
+0000f9b0: 2020 2020 7b22 6122 3a20 312c 2022 6222      {"a": 1, "b"
+0000f9c0: 3a20 322c 2022 6322 3a20 307d 0a20 2020  : 2, "c": 0}.   
+0000f9d0: 207b 2261 223a 2031 2c20 2262 223a 2032   {"a": 1, "b": 2
+0000f9e0: 2c20 2263 223a 2031 7d0a 2020 2020 7b22  , "c": 1}.    {"
+0000f9f0: 6122 3a20 312c 2022 6222 3a20 322c 2022  a": 1, "b": 2, "
+0000fa00: 6322 3a20 327d 0a20 2020 207b 2261 223a  c": 2}.    {"a":
+0000fa10: 2032 2c20 2262 223a 2030 2c20 2263 223a   2, "b": 0, "c":
+0000fa20: 2030 7d0a 2020 2020 7b22 6122 3a20 322c   0}.    {"a": 2,
+0000fa30: 2022 6222 3a20 302c 2022 6322 3a20 317d   "b": 0, "c": 1}
+0000fa40: 0a20 2020 207b 2261 223a 2032 2c20 2262  .    {"a": 2, "b
+0000fa50: 223a 2030 2c20 2263 223a 2032 7d0a 2020  ": 0, "c": 2}.  
+0000fa60: 2020 7b22 6122 3a20 322c 2022 6222 3a20    {"a": 2, "b": 
+0000fa70: 312c 2022 6322 3a20 307d 0a20 2020 207b  1, "c": 0}.    {
+0000fa80: 2261 223a 2032 2c20 2262 223a 2031 2c20  "a": 2, "b": 1, 
+0000fa90: 2263 223a 2031 7d0a 2020 2020 7b22 6122  "c": 1}.    {"a"
+0000faa0: 3a20 322c 2022 6222 3a20 312c 2022 6322  : 2, "b": 1, "c"
+0000fab0: 3a20 327d 0a20 2020 207b 2261 223a 2032  : 2}.    {"a": 2
+0000fac0: 2c20 2262 223a 2032 2c20 2263 223a 2030  , "b": 2, "c": 0
+0000fad0: 7d0a 2020 2020 7b22 6122 3a20 322c 2022  }.    {"a": 2, "
+0000fae0: 6222 3a20 322c 2022 6322 3a20 317d 0a20  b": 2, "c": 1}. 
+0000faf0: 2020 207b 2261 223a 2032 2c20 2262 223a     {"a": 2, "b":
+0000fb00: 2032 2c20 2263 223a 2032 7d0a 0a22 2222   2, "c": 2}.."""
+0000fb10: 0a0a 6669 7865 645f 7769 6474 685f 6461  ..fixed_width_da
+0000fb20: 7461 203d 2022 2222 5c0a 3020 3020 300a  ta = """\.0 0 0.
+0000fb30: 3020 3020 310a 3020 3020 320a 3020 3120  0 0 1.0 0 2.0 1 
+0000fb40: 300a 3020 3120 310a 3020 3120 320a 3020  0.0 1 1.0 1 2.0 
+0000fb50: 3220 300a 3020 3220 310a 3020 3220 320a  2 0.0 2 1.0 2 2.
+0000fb60: 3120 3020 300a 3120 3020 310a 3120 3020  1 0 0.1 0 1.1 0 
+0000fb70: 320a 3120 3120 300a 3120 3120 310a 3120  2.1 1 0.1 1 1.1 
+0000fb80: 3120 320a 3120 3220 300a 3120 3220 310a  1 2.1 2 0.1 2 1.
+0000fb90: 3120 3220 320a 3220 3020 300a 3220 3020  1 2 2.2 0 0.2 0 
+0000fba0: 310a 3220 3020 320a 3220 3120 300a 3220  1.2 0 2.2 1 0.2 
+0000fbb0: 3120 310a 3220 3120 320a 3220 3220 300a  1 1.2 1 2.2 2 0.
+0000fbc0: 3220 3220 310a 3220 3220 320a 0a22 2222  2 2 1.2 2 2.."""
+0000fbd0: 0a0a 0a40 6d61 6b65 5f74 6573 745f 636c  ...@make_test_cl
+0000fbe0: 6173 7365 730a 636c 6173 7320 5461 626c  asses.class Tabl
+0000fbf0: 6549 6d70 6f72 7445 7870 6f72 7454 6573  eImportExportTes
+0000fc00: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
+0000fc10: 5f63 7376 5f65 7870 6f72 7428 7365 6c66  _csv_export(self
+0000fc20: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
+0000fc30: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
+0000fc40: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
+0000fc50: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+0000fc60: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
+0000fc70: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+0000fc80: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+0000fc90: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+0000fca0: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
+0000fcb0: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
+0000fcc0: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
+0000fcd0: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
+0000fce0: 2020 2020 6f75 7420 3d20 696f 2e53 7472      out = io.Str
+0000fcf0: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
+0000fd00: 2020 2020 7431 2e63 7376 5f65 7870 6f72      t1.csv_expor
+0000fd10: 7428 6f75 742c 2066 6965 6c64 6e61 6d65  t(out, fieldname
+0000fd20: 7329 0a20 2020 2020 2020 2020 2020 206f  s).            o
+0000fd30: 7574 2e73 6565 6b28 3029 0a20 2020 2020  ut.seek(0).     
+0000fd40: 2020 2020 2020 206f 7574 6c69 6e65 7320         outlines 
+0000fd50: 3d20 6f75 742e 7265 6164 2829 2e73 706c  = out.read().spl
+0000fd60: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
+0000fd70: 2020 2020 2020 6f75 742e 636c 6f73 6528        out.close(
+0000fd80: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+0000fd90: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000fda0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000fdb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000fdc0: 7561 6c28 272c 272e 6a6f 696e 2866 6965  ual(','.join(fie
+0000fdd0: 6c64 6e61 6d65 7329 2c20 6f75 746c 696e  ldnames), outlin
+0000fde0: 6573 5b30 5d29 0a20 2020 2020 2020 2020  es[0]).         
+0000fdf0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000fe00: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000fe10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000fe20: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+0000fe30: 7a65 2a2a 332b 312c 206c 656e 286f 7574  ze**3+1, len(out
+0000fe40: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
+0000fe50: 2020 2020 666f 7220 6f62 2c20 6c69 6e65      for ob, line
+0000fe60: 2069 6e20 7a69 7028 7431 2c20 6f75 746c   in zip(t1, outl
+0000fe70: 696e 6573 5b31 3a5d 293a 0a20 2020 2020  ines[1:]):.     
+0000fe80: 2020 2020 2020 2020 2020 2063 7376 5f76             csv_v
+0000fe90: 616c 7320 3d20 6c69 6e65 2e73 706c 6974  als = line.split
+0000fea0: 2827 2c27 290a 2020 2020 2020 2020 2020  (',').          
+0000feb0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000fec0: 7375 6254 6573 7428 6f62 3d6f 622c 2063  subTest(ob=ob, c
+0000fed0: 7376 5f76 616c 733d 6373 765f 7661 6c73  sv_vals=csv_vals
+0000fee0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000fef0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000ff00: 7274 5472 7565 2861 6c6c 280a 2020 2020  rtTrue(all(.    
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 2020 696e 7428 6373 765f 7661 6c73      int(csv_vals
+0000ff30: 5b69 5d29 203d 3d20 6765 7461 7474 7228  [i]) == getattr(
+0000ff40: 6f62 2c20 666c 6429 2066 6f72 2069 2c20  ob, fld) for i, 
+0000ff50: 666c 6420 696e 2065 6e75 6d65 7261 7465  fld in enumerate
+0000ff60: 2866 6965 6c64 6e61 6d65 7329 0a20 2020  (fieldnames).   
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff80: 2029 290a 0a20 2020 2020 2020 2023 2072   ))..        # r
+0000ff90: 6572 756e 2075 7369 6e67 2061 6e20 656d  erun using an em
+0000ffa0: 7074 7920 7461 626c 650a 2020 2020 2020  pty table.      
+0000ffb0: 2020 7431 203d 206c 742e 5461 626c 6528    t1 = lt.Table(
+0000ffc0: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
+0000ffd0: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
+0000ffe0: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
+0000fff0: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
+00010000: 2020 206f 7574 203d 2069 6f2e 5374 7269     out = io.Stri
+00010010: 6e67 494f 2829 0a20 2020 2020 2020 2020  ngIO().         
+00010020: 2020 2074 312e 6373 765f 6578 706f 7274     t1.csv_export
+00010030: 286f 7574 2c20 6669 656c 646e 616d 6573  (out, fieldnames
+00010040: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+00010050: 742e 7365 656b 2830 290a 2020 2020 2020  t.seek(0).      
+00010060: 2020 2020 2020 6f75 746c 696e 6573 203d        outlines =
+00010070: 206f 7574 2e72 6561 6428 292e 7370 6c69   out.read().spli
+00010080: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
+00010090: 2020 2020 206f 7574 2e63 6c6f 7365 2829       out.close()
+000100a0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+000100b0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+000100c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000100d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000100e0: 616c 2827 2c27 2e6a 6f69 6e28 6669 656c  al(','.join(fiel
+000100f0: 646e 616d 6573 292c 206f 7574 6c69 6e65  dnames), outline
+00010100: 735b 305d 290a 2020 2020 2020 2020 2020  s[0]).          
+00010110: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00010120: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00010130: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010140: 7274 4571 7561 6c28 312c 206c 656e 286f  rtEqual(1, len(o
+00010150: 7574 6c69 6e65 7329 290a 0a20 2020 2020  utlines))..     
+00010160: 2020 2023 2072 6572 756e 2075 7369 6e67     # rerun using
+00010170: 2061 6e20 656d 7074 7920 7461 626c 652c   an empty table,
+00010180: 2077 6974 6820 696e 6465 7865 7320 746f   with indexes to
+00010190: 2064 6963 7461 7465 2066 6965 6c64 6e61   dictate fieldna
+000101a0: 6d65 730a 2020 2020 2020 2020 666f 7220  mes.        for 
+000101b0: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
+000101c0: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
+000101d0: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
+000101e0: 2020 2020 2074 3120 3d20 6c74 2e54 6162       t1 = lt.Tab
+000101f0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+00010200: 2066 6f72 2066 6c64 2069 6e20 6669 656c   for fld in fiel
+00010210: 646e 616d 6573 3a0a 2020 2020 2020 2020  dnames:.        
+00010220: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
+00010230: 655f 696e 6465 7828 666c 6429 0a20 2020  e_index(fld).   
+00010240: 2020 2020 2020 2020 206f 7574 203d 2069           out = i
+00010250: 6f2e 5374 7269 6e67 494f 2829 0a20 2020  o.StringIO().   
+00010260: 2020 2020 2020 2020 2074 312e 6373 765f           t1.csv_
+00010270: 6578 706f 7274 286f 7574 290a 2020 2020  export(out).    
+00010280: 2020 2020 2020 2020 6f75 742e 7365 656b          out.seek
+00010290: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+000102a0: 6f75 746c 696e 6573 203d 206f 7574 2e72  outlines = out.r
+000102b0: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
+000102c0: 2829 0a20 2020 2020 2020 2020 2020 206f  ().            o
+000102d0: 7574 2e63 6c6f 7365 2829 0a20 2020 2020  ut.close().     
+000102e0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000102f0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00010300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010310: 2e61 7373 6572 7445 7175 616c 2873 6574  .assertEqual(set
+00010320: 2866 6965 6c64 6e61 6d65 7329 2c20 7365  (fieldnames), se
+00010330: 7428 6f75 746c 696e 6573 5b30 5d2e 7370  t(outlines[0].sp
+00010340: 6c69 7428 272c 2729 2929 0a20 2020 2020  lit(','))).     
+00010350: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00010360: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00010370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010380: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
+00010390: 6c65 6e28 6f75 746c 696e 6573 2929 0a0a  len(outlines))..
+000103a0: 2020 2020 6465 6620 7465 7374 5f63 7376      def test_csv
+000103b0: 5f65 7870 6f72 745f 746f 5f73 7472 696e  _export_to_strin
+000103c0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+000103d0: 2066 726f 6d20 6974 6572 746f 6f6c 7320   from itertools 
+000103e0: 696d 706f 7274 2070 6572 6d75 7461 7469  import permutati
+000103f0: 6f6e 730a 2020 2020 2020 2020 7465 7374  ons.        test
+00010400: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+00010410: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00010420: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00010430: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00010440: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
+00010450: 2066 6f72 2066 6965 6c64 6e61 6d65 7320   for fieldnames 
+00010460: 696e 2070 6572 6d75 7461 7469 6f6e 7328  in permutations(
+00010470: 6c69 7374 2827 6162 6327 2929 3a0a 2020  list('abc')):.  
+00010480: 2020 2020 2020 2020 2020 6f75 745f 7374            out_st
+00010490: 7269 6e67 203d 2074 312e 6373 765f 6578  ring = t1.csv_ex
+000104a0: 706f 7274 284e 6f6e 652c 2066 6965 6c64  port(None, field
+000104b0: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
+000104c0: 2020 206f 7574 6c69 6e65 7320 3d20 6f75     outlines = ou
+000104d0: 745f 7374 7269 6e67 2e73 706c 6974 6c69  t_string.splitli
+000104e0: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
+000104f0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00010500: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00010510: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010520: 7274 4571 7561 6c28 272c 272e 6a6f 696e  rtEqual(','.join
+00010530: 2866 6965 6c64 6e61 6d65 7329 2c20 6f75  (fieldnames), ou
+00010540: 746c 696e 6573 5b30 5d29 0a20 2020 2020  tlines[0]).     
+00010550: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00010560: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00010570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010580: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00010590: 745f 7369 7a65 202a 2a20 3320 2b20 312c  t_size ** 3 + 1,
+000105a0: 206c 656e 286f 7574 6c69 6e65 7329 290a   len(outlines)).
+000105b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000105c0: 6f62 2c20 6c69 6e65 2069 6e20 7a69 7028  ob, line in zip(
+000105d0: 7431 2c20 6f75 746c 696e 6573 5b31 3a5d  t1, outlines[1:]
+000105e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000105f0: 2020 2063 7376 5f76 616c 7320 3d20 6c69     csv_vals = li
+00010600: 6e65 2e73 706c 6974 2827 2c27 290a 2020  ne.split(',').  
+00010610: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00010620: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00010630: 6f62 3d6f 622c 2063 7376 5f76 616c 733d  ob=ob, csv_vals=
+00010640: 6373 765f 7661 6c73 293a 0a20 2020 2020  csv_vals):.     
+00010650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010660: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+00010670: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
+00010680: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+00010690: 6373 765f 7661 6c73 5b69 5d29 203d 3d20  csv_vals[i]) == 
+000106a0: 6765 7461 7474 7228 6f62 2c20 666c 6429  getattr(ob, fld)
+000106b0: 2066 6f72 2069 2c20 666c 6420 696e 2065   for i, fld in e
+000106c0: 6e75 6d65 7261 7465 2866 6965 6c64 6e61  numerate(fieldna
+000106d0: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
+000106e0: 2020 2020 2020 2020 2029 290a 0a20 2020           ))..   
+000106f0: 2064 6566 2074 6573 745f 6373 765f 696d   def test_csv_im
+00010700: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
+00010710: 2020 2020 6461 7461 203d 2063 7376 5f64      data = csv_d
+00010720: 6174 610a 2020 2020 2020 2020 696e 6373  ata.        incs
+00010730: 7620 3d20 696f 2e53 7472 696e 6749 4f28  v = io.StringIO(
+00010740: 6461 7461 290a 2020 2020 2020 2020 6373  data).        cs
+00010750: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
+00010760: 6528 292e 6373 765f 696d 706f 7274 2869  e().csv_import(i
+00010770: 6e63 7376 2c20 7472 616e 7366 6f72 6d73  ncsv, transforms
+00010780: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
+00010790: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
+000107a0: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
+000107b0: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+000107c0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
+000107d0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+000107e0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+000107f0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00010800: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00010810: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00010820: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00010830: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
+00010840: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
+00010850: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
+00010860: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
+00010870: 2874 312c 2063 7376 7461 626c 6529 2929  (t1, csvtable)))
+00010880: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00010890: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+000108a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000108b0: 7373 6572 7445 7175 616c 2873 756d 2831  ssertEqual(sum(1
+000108c0: 2066 6f72 206c 696e 6520 696e 2064 6174   for line in dat
+000108d0: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
+000108e0: 6620 6c69 6e65 2e73 7472 6970 2829 292d  f line.strip())-
+000108f0: 312c 206c 656e 2863 7376 7461 626c 6529  1, len(csvtable)
+00010900: 290a 0a20 2020 2020 2020 2069 6e63 7376  )..        incsv
+00010910: 203d 2069 6f2e 5374 7269 6e67 494f 2864   = io.StringIO(d
+00010920: 6174 6129 0a20 2020 2020 2020 2072 6f77  ata).        row
+00010930: 5f70 726f 746f 7479 7065 203d 2073 656c  _prototype = sel
+00010940: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+00010950: 6374 2830 2c20 302c 2030 290a 2020 2020  ct(0, 0, 0).    
+00010960: 2020 2020 6373 7674 6162 6c65 3220 3d20      csvtable2 = 
+00010970: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00010980: 6d70 6f72 7428 696e 6373 762c 2074 7261  mport(incsv, tra
+00010990: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
+000109a0: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
+000109b0: 3a20 696e 747d 2c20 726f 775f 636c 6173  : int}, row_clas
+000109c0: 733d 7479 7065 2872 6f77 5f70 726f 746f  s=type(row_proto
+000109d0: 7479 7065 2929 5b3a 335d 0a0a 2020 2020  type))[:3]..    
+000109e0: 2020 2020 7072 696e 7428 7479 7065 2874      print(type(t
+000109f0: 315b 305d 292e 5f5f 6e61 6d65 5f5f 2c20  1[0]).__name__, 
+00010a00: 7431 5b30 5d29 0a20 2020 2020 2020 2070  t1[0]).        p
+00010a10: 7269 6e74 2874 7970 6528 6373 7674 6162  rint(type(csvtab
+00010a20: 6c65 325b 305d 292e 5f5f 6e61 6d65 5f5f  le2[0]).__name__
+00010a30: 2c20 6373 7674 6162 6c65 325b 305d 290a  , csvtable2[0]).
 00010a40: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010a50: 662e 7375 6254 6573 7428 6e61 6d65 3d6e  f.subTest(name=n
-00010a60: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-00010a70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010a80: 7445 7175 616c 2873 756d 2874 742e 616c  tEqual(sum(tt.al
-00010a90: 6c2e 6129 2c20 7375 6d28 7474 322e 616c  l.a), sum(tt2.al
-00010aa0: 6c2e 6129 290a 2020 2020 2020 2020 2020  l.a)).          
-00010ab0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00010ac0: 6573 7428 6e61 6d65 3d6e 616d 6529 3a0a  est(name=name):.
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ae0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00010af0: 2873 756d 2874 742e 616c 6c2e 6229 2c20  (sum(tt.all.b), 
-00010b00: 7375 6d28 7474 322e 616c 6c2e 6229 290a  sum(tt2.all.b)).
-00010b10: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00010b20: 2073 656c 662e 7375 6254 6573 7428 6e61   self.subTest(na
-00010b30: 6d65 3d6e 616d 6529 3a0a 2020 2020 2020  me=name):.      
-00010b40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00010b50: 7373 6572 7445 7175 616c 2873 756d 2874  ssertEqual(sum(t
-00010b60: 742e 616c 6c2e 6329 2c20 7375 6d28 7474  t.all.c), sum(tt
-00010b70: 322e 616c 6c2e 6329 290a 0a20 2020 2020  2.all.c))..     
-00010b80: 2020 2023 2074 6573 7420 7365 7061 7261     # test separa
-00010b90: 7465 6c79 2c20 6e6f 2074 7261 6e73 666f  tely, no transfo
-00010ba0: 726d 7320 666f 7220 4a53 4f4e 2069 6d70  rms for JSON imp
-00010bb0: 6f72 7473 0a20 2020 2020 2020 2069 6d70  orts.        imp
-00010bc0: 6f72 745f 736f 7572 6365 5f6e 616d 6520  ort_source_name 
-00010bd0: 3d20 2274 6573 742f 6162 632e 6a73 6f6e  = "test/abc.json
-00010be0: 2e67 7a22 0a20 2020 2020 2020 2074 7432  .gz".        tt2
-00010bf0: 203d 206c 742e 5461 626c 6528 292e 6a73   = lt.Table().js
-00010c00: 6f6e 5f69 6d70 6f72 7428 2274 6573 742f  on_import("test/
-00010c10: 6162 632e 6a73 6f6e 2e67 7a22 2c20 7374  abc.json.gz", st
-00010c20: 7265 616d 696e 673d 5472 7565 290a 2020  reaming=True).  
-00010c30: 2020 2020 2020 7072 696e 7428 2261 6263        print("abc
-00010c40: 2e6a 736f 6e2e 677a 222c 2074 7432 2e69  .json.gz", tt2.i
-00010c50: 6e66 6f28 2929 0a20 2020 2020 2020 2065  nfo()).        e
-00010c60: 7870 6563 7465 645f 696e 666f 203d 207b  xpected_info = {
-00010c70: 2a2a 7474 2e69 6e66 6f28 292c 2022 6e61  **tt.info(), "na
-00010c80: 6d65 223a 2069 6d70 6f72 745f 736f 7572  me": import_sour
-00010c90: 6365 5f6e 616d 657d 0a20 2020 2020 2020  ce_name}.       
-00010ca0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00010cb0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00010cc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00010cd0: 616c 2865 7870 6563 7465 645f 696e 666f  al(expected_info
-00010ce0: 2c20 7474 322e 696e 666f 2829 290a 2020  , tt2.info()).  
-00010cf0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00010d00: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00010d10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00010d20: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
-00010d30: 6c6c 2e61 292c 2073 756d 2874 7432 2e61  ll.a), sum(tt2.a
-00010d40: 6c6c 2e61 2929 0a20 2020 2020 2020 2077  ll.a)).        w
-00010d50: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00010d60: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00010d70: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00010d80: 2873 756d 2874 742e 616c 6c2e 6229 2c20  (sum(tt.all.b), 
-00010d90: 7375 6d28 7474 322e 616c 6c2e 6229 290a  sum(tt2.all.b)).
-00010da0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010db0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00010dc0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00010dd0: 7365 7274 4571 7561 6c28 7375 6d28 7474  sertEqual(sum(tt
-00010de0: 2e61 6c6c 2e63 292c 2073 756d 2874 7432  .all.c), sum(tt2
-00010df0: 2e61 6c6c 2e63 2929 0a0a 2020 2020 6465  .all.c))..    de
-00010e00: 6620 7465 7374 5f63 7376 5f69 6d70 6f72  f test_csv_impor
-00010e10: 745f 736f 7572 6365 5f69 6e66 6f28 7365  t_source_info(se
-00010e20: 6c66 293a 0a20 2020 2020 2020 2069 6d70  lf):.        imp
-00010e30: 6f72 7473 203d 205b 0a20 2020 2020 2020  orts = [.       
-00010e40: 2020 2020 2028 2261 6263 2e63 7376 222c       ("abc.csv",
-00010e50: 206c 742e 496d 706f 7274 536f 7572 6365   lt.ImportSource
-00010e60: 5479 7065 2e66 696c 6529 2c0a 2020 2020  Type.file),.    
-00010e70: 2020 2020 2020 2020 2822 6162 632e 7473          ("abc.ts
-00010e80: 7622 2c20 6c74 2e49 6d70 6f72 7453 6f75  v", lt.ImportSou
-00010e90: 7263 6554 7970 652e 6669 6c65 292c 0a20  rceType.file),. 
-00010ea0: 2020 2020 2020 2020 2020 2028 2261 6263             ("abc
-00010eb0: 2e78 6c73 7822 2c20 6c74 2e49 6d70 6f72  .xlsx", lt.Impor
-00010ec0: 7453 6f75 7263 6554 7970 652e 6669 6c65  tSourceType.file
-00010ed0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00010ee0: 2261 6263 2e63 7376 2e7a 6970 222c 206c  "abc.csv.zip", l
-00010ef0: 742e 496d 706f 7274 536f 7572 6365 5479  t.ImportSourceTy
-00010f00: 7065 2e7a 6970 292c 0a20 2020 2020 2020  pe.zip),.       
-00010f10: 2020 2020 2028 2261 6263 2e63 7376 2e67       ("abc.csv.g
-00010f20: 7a22 2c20 6c74 2e49 6d70 6f72 7453 6f75  z", lt.ImportSou
-00010f30: 7263 6554 7970 652e 677a 6970 292c 0a20  rceType.gzip),. 
-00010f40: 2020 2020 2020 2020 2020 2028 2261 6263             ("abc
-00010f50: 2e63 7376 2e78 7a22 2c20 6c74 2e49 6d70  .csv.xz", lt.Imp
-00010f60: 6f72 7453 6f75 7263 6554 7970 652e 6c7a  ortSourceType.lz
-00010f70: 6d61 292c 0a20 2020 2020 2020 2020 2020  ma),.           
-00010f80: 2028 2261 2c62 2c63 5c6e 312c 322c 3322   ("a,b,c\n1,2,3"
-00010f90: 2c20 6c74 2e49 6d70 6f72 7453 6f75 7263  , lt.ImportSourc
-00010fa0: 6554 7970 652e 7374 7269 6e67 292c 0a20  eType.string),. 
-00010fb0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00010fc0: 2066 6f72 2066 6e61 6d65 2c20 6578 7065   for fname, expe
-00010fd0: 6374 6564 5f74 7970 6520 696e 2069 6d70  cted_type in imp
-00010fe0: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
-00010ff0: 2020 6966 2022 5c6e 2220 6e6f 7420 696e    if "\n" not in
-00011000: 2066 6e61 6d65 3a0a 2020 2020 2020 2020   fname:.        
-00011010: 2020 2020 2020 2020 696d 706f 7274 5f6e          import_n
-00011020: 616d 6520 3d20 2274 6573 742f 2220 2b20  ame = "test/" + 
-00011030: 666e 616d 650a 2020 2020 2020 2020 2020  fname.          
-00011040: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011050: 2020 2020 2020 2020 696d 706f 7274 5f6e          import_n
-00011060: 616d 6520 3d20 666e 616d 650a 2020 2020  ame = fname.    
-00011070: 2020 2020 2020 2020 6966 2069 6d70 6f72          if impor
-00011080: 745f 6e61 6d65 2e65 6e64 7377 6974 6828  t_name.endswith(
-00011090: 222e 6373 7622 293a 0a20 2020 2020 2020  ".csv"):.       
-000110a0: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
-000110b0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-000110c0: 706f 7274 2869 6d70 6f72 745f 6e61 6d65  port(import_name
-000110d0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000110e0: 6966 2069 6d70 6f72 745f 6e61 6d65 2e65  if import_name.e
-000110f0: 6e64 7377 6974 6828 222e 786c 7378 2229  ndswith(".xlsx")
-00011100: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011110: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
-00011120: 2829 2e65 7863 656c 5f69 6d70 6f72 7428  ().excel_import(
-00011130: 696d 706f 7274 5f6e 616d 6529 0a20 2020  import_name).   
-00011140: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011150: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00011160: 626c 203d 206c 742e 5461 626c 6528 292e  bl = lt.Table().
-00011170: 7473 765f 696d 706f 7274 2869 6d70 6f72  tsv_import(impor
-00011180: 745f 6e61 6d65 290a 0a20 2020 2020 2020  t_name)..       
-00011190: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
-000111a0: 696d 706f 7274 5f6e 616d 6529 2c20 7462  import_name), tb
-000111b0: 6c2e 696d 706f 7274 5f73 6f75 7263 652c  l.import_source,
-000111c0: 2074 626c 2e69 6d70 6f72 745f 736f 7572   tbl.import_sour
-000111d0: 6365 5f74 7970 6529 0a0a 2020 2020 2020  ce_type)..      
-000111e0: 2020 2020 2020 6966 2022 5c6e 2220 6e6f        if "\n" no
-000111f0: 7420 696e 2066 6e61 6d65 3a0a 2020 2020  t in fname:.    
-00011200: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00011210: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00011220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011230: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00011240: 4571 7561 6c28 696d 706f 7274 5f6e 616d  Equal(import_nam
-00011250: 652c 2074 626c 2e69 6d70 6f72 745f 736f  e, tbl.import_so
-00011260: 7572 6365 290a 2020 2020 2020 2020 2020  urce).          
-00011270: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011280: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00011290: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000112c0: 6c28 4e6f 6e65 2c20 7462 6c2e 696d 706f  l(None, tbl.impo
-000112d0: 7274 5f73 6f75 7263 6529 0a20 2020 2020  rt_source).     
-000112e0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-000112f0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00011300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011310: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-00011320: 6563 7465 645f 7479 7065 2c20 7462 6c2e  ected_type, tbl.
-00011330: 696d 706f 7274 5f73 6f75 7263 655f 7479  import_source_ty
-00011340: 7065 290a 0a20 2020 2064 6566 2074 6573  pe)..    def tes
-00011350: 745f 6373 765f 696d 706f 7274 5f66 726f  t_csv_import_fro
-00011360: 6d5f 7572 6c28 7365 6c66 293a 0a20 2020  m_url(self):.   
-00011370: 2020 2020 2066 726f 6d20 6874 7470 2e73       from http.s
-00011380: 6572 7665 7220 696d 706f 7274 2048 5454  erver import HTT
-00011390: 5053 6572 7665 722c 2042 6173 6548 5454  PServer, BaseHTT
-000113a0: 5052 6571 7565 7374 4861 6e64 6c65 720a  PRequestHandler.
-000113b0: 2020 2020 2020 2020 6672 6f6d 2068 7474          from htt
-000113c0: 7020 696d 706f 7274 2048 5454 5053 7461  p import HTTPSta
-000113d0: 7475 730a 2020 2020 2020 2020 696d 706f  tus.        impo
-000113e0: 7274 2074 6872 6561 6469 6e67 0a20 2020  rt threading.   
-000113f0: 2020 2020 2069 6d70 6f72 7420 7469 6d65       import time
-00011400: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00011410: 7572 6c6c 6962 2e65 7272 6f72 0a20 2020  urllib.error.   
-00011420: 2020 2020 2069 6d70 6f72 7420 7572 6c6c       import urll
-00011430: 6962 2e72 6571 7565 7374 0a0a 2020 2020  ib.request..    
-00011440: 2020 2020 6966 2053 4b49 505f 4353 565f      if SKIP_CSV_
-00011450: 494d 504f 5254 5f55 5349 4e47 5f55 524c  IMPORT_USING_URL
-00011460: 5f54 4553 5453 3a0a 2020 2020 2020 2020  _TESTS:.        
-00011470: 2020 2020 7365 6c66 2e73 6b69 7054 6573      self.skipTes
-00011480: 7428 2243 5356 2069 6d70 6f72 7420 7465  t("CSV import te
-00011490: 7374 7320 736b 6970 7065 6422 290a 0a20  sts skipped").. 
-000114a0: 2020 2020 2020 2063 6c61 7373 2043 5356         class CSV
-000114b0: 5465 7374 5265 7175 6573 7448 616e 646c  TestRequestHandl
-000114c0: 6572 2842 6173 6548 5454 5052 6571 7565  er(BaseHTTPReque
-000114d0: 7374 4861 6e64 6c65 7229 3a0a 2020 2020  stHandler):.    
-000114e0: 2020 2020 2020 2020 6465 6620 646f 5f47          def do_G
-000114f0: 4554 2873 656c 6629 3a0a 2020 2020 2020  ET(self):.      
-00011500: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00011510: 6f67 5f6d 6573 7361 6765 2822 7265 6365  og_message("rece
-00011520: 6976 6564 2025 7320 2573 222c 2073 656c  ived %s %s", sel
-00011530: 662e 636f 6d6d 616e 642c 2073 656c 662e  f.command, self.
-00011540: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-00011550: 2020 2020 2020 7061 7468 203d 2073 656c        path = sel
-00011560: 662e 7061 7468 0a20 2020 2020 2020 2020  f.path.         
-00011570: 2020 2020 2020 2069 6620 7061 7468 203d         if path =
-00011580: 3d20 222f 4558 4954 223a 0a20 2020 2020  = "/EXIT":.     
-00011590: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000115a0: 656c 662e 7365 6e64 5f72 6573 706f 6e73  elf.send_respons
-000115b0: 6528 4854 5450 5374 6174 7573 2e4f 4b29  e(HTTPStatus.OK)
-000115c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115d0: 2020 2020 2073 656c 662e 656e 645f 6865       self.end_he
-000115e0: 6164 6572 7328 290a 2020 2020 2020 2020  aders().        
-000115f0: 2020 2020 2020 2020 2020 2020 7468 7265              thre
-00011600: 6164 696e 672e 5468 7265 6164 2874 6172  ading.Thread(tar
-00011610: 6765 743d 6c61 6d62 6461 3a20 7365 6c66  get=lambda: self
-00011620: 2e73 6572 7665 722e 7368 7574 646f 776e  .server.shutdown
-00011630: 2829 292e 7374 6172 7428 290a 0a20 2020  ()).start()..   
-00011640: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00011650: 6620 7061 7468 203d 3d20 222f 223a 0a20  f path == "/":. 
-00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011670: 2020 2073 656c 662e 7365 6e64 5f72 6573     self.send_res
-00011680: 706f 6e73 6528 4854 5450 5374 6174 7573  ponse(HTTPStatus
-00011690: 2e4f 4b29 0a20 2020 2020 2020 2020 2020  .OK).           
-000116a0: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
-000116b0: 645f 6865 6164 6572 7328 290a 0a20 2020  d_headers()..   
-000116c0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000116d0: 6620 7061 7468 2e73 7461 7274 7377 6974  f path.startswit
-000116e0: 6828 222f 6162 632e 6373 7622 293a 0a20  h("/abc.csv"):. 
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2073 656e 645f 6279 7465 7320 3d20     send_bytes = 
-00011710: 6222 612c 622c 635c 6e31 2c32 2c33 5c6e  b"a,b,c\n1,2,3\n
-00011720: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00011730: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00011740: 7265 7370 6f6e 7365 2848 5454 5053 7461  response(HTTPSta
-00011750: 7475 732e 4f4b 290a 2020 2020 2020 2020  tus.OK).        
-00011760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011770: 2e65 6e64 5f68 6561 6465 7273 2829 0a20  .end_headers(). 
-00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011790: 2020 2073 656c 662e 7766 696c 652e 7772     self.wfile.wr
-000117a0: 6974 6528 7365 6e64 5f62 7974 6573 290a  ite(send_bytes).
-000117b0: 0a20 2020 2020 2020 2064 6566 2072 756e  .        def run
-000117c0: 2873 6572 7665 725f 636c 6173 733d 4854  (server_class=HT
-000117d0: 5450 5365 7276 6572 2c20 6861 6e64 6c65  TPServer, handle
-000117e0: 725f 636c 6173 733d 4353 5654 6573 7452  r_class=CSVTestR
-000117f0: 6571 7565 7374 4861 6e64 6c65 7229 3a0a  equestHandler):.
-00011800: 2020 2020 2020 2020 2020 2020 7365 7276              serv
-00011810: 6572 5f61 6464 7265 7373 203d 2028 2727  er_address = (''
-00011820: 2c20 3838 3838 290a 2020 2020 2020 2020  , 8888).        
-00011830: 2020 2020 6874 7470 6420 3d20 7365 7276      httpd = serv
-00011840: 6572 5f63 6c61 7373 2873 6572 7665 725f  er_class(server_
-00011850: 6164 6472 6573 732c 2068 616e 646c 6572  address, handler
-00011860: 5f63 6c61 7373 290a 2020 2020 2020 2020  _class).        
-00011870: 2020 2020 6874 7470 642e 7365 7276 655f      httpd.serve_
-00011880: 666f 7265 7665 7228 290a 0a20 2020 2020  forever()..     
-00011890: 2020 2064 6566 2072 756e 5f62 6163 6b67     def run_backg
-000118a0: 726f 756e 645f 7465 7374 5f73 6572 7665  round_test_serve
-000118b0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-000118c0: 2070 203d 2074 6872 6561 6469 6e67 2e54   p = threading.T
-000118d0: 6872 6561 6428 7461 7267 6574 3d72 756e  hread(target=run
-000118e0: 290a 2020 2020 2020 2020 2020 2020 702e  ).            p.
-000118f0: 7374 6172 7428 290a 0a20 2020 2020 2020  start()..       
-00011900: 2020 2020 2066 6f72 2074 7269 6573 5f72       for tries_r
-00011910: 656d 6169 6e69 6e67 2069 6e20 7265 7665  emaining in reve
-00011920: 7273 6564 2872 616e 6765 2832 3029 293a  rsed(range(20)):
-00011930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011940: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00011950: 2020 2020 2020 2020 2020 7769 7468 2075            with u
-00011960: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
-00011970: 6c6f 7065 6e28 2268 7474 703a 2f2f 6c6f  lopen("http://lo
-00011980: 6361 6c68 6f73 743a 3838 3838 2f22 293a  calhost:8888/"):
-00011990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119a0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000119c0: 7863 6570 7420 7572 6c6c 6962 2e65 7272  xcept urllib.err
-000119d0: 6f72 2e55 524c 4572 726f 723a 0a20 2020  or.URLError:.   
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 2069 6620 7472 6965 735f 7265 6d61 696e   if tries_remain
-00011a00: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00011a10: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00011a20: 652e 736c 6565 7028 302e 3235 290a 0a20  e.sleep(0.25).. 
-00011a30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00011a40: 6e20 700a 0a20 2020 2020 2020 2077 6562  n p..        web
-00011a50: 5f61 6464 7265 7373 203d 2022 6874 7470  _address = "http
-00011a60: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3838  ://localhost:888
-00011a70: 3822 0a20 2020 2020 2020 2070 203d 2072  8".        p = r
-00011a80: 756e 5f62 6163 6b67 726f 756e 645f 7465  un_background_te
-00011a90: 7374 5f73 6572 7665 7228 290a 0a20 2020  st_server()..   
-00011aa0: 2020 2020 2075 726c 203d 2077 6562 5f61       url = web_a
-00011ab0: 6464 7265 7373 202b 2022 2f61 6263 2e63  ddress + "/abc.c
-00011ac0: 7376 220a 2020 2020 2020 2020 7472 793a  sv".        try:
-00011ad0: 0a20 2020 2020 2020 2020 2020 2074 626c  .            tbl
-00011ae0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-00011af0: 765f 696d 706f 7274 2875 726c 290a 2020  v_import(url).  
-00011b00: 2020 2020 2020 6669 6e61 6c6c 793a 0a20        finally:. 
-00011b10: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00011b20: 7572 6c6c 6962 2e72 6571 7565 7374 2e75  urllib.request.u
-00011b30: 726c 6f70 656e 2877 6562 5f61 6464 7265  rlopen(web_addre
-00011b40: 7373 202b 2022 2f45 5849 5422 293a 0a20  ss + "/EXIT"):. 
-00011b50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011b60: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00011b70: 702e 6a6f 696e 2829 0a0a 2020 2020 2020  p.join()..      
-00011b80: 2020 7462 6c2e 7072 6573 656e 7428 290a    tbl.present().
-00011b90: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00011ba0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00011bb0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00011bc0: 7365 7274 4571 7561 6c28 7572 6c2c 2074  sertEqual(url, t
-00011bd0: 626c 2e69 6d70 6f72 745f 736f 7572 6365  bl.import_source
-00011be0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00011bf0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00011c00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011c10: 6173 7365 7274 4571 7561 6c28 6c74 2e49  assertEqual(lt.I
-00011c20: 6d70 6f72 7453 6f75 7263 6554 7970 652e  mportSourceType.
-00011c30: 7572 6c2c 2074 626c 2e69 6d70 6f72 745f  url, tbl.import_
-00011c40: 736f 7572 6365 5f74 7970 6529 0a0a 2020  source_type)..  
-00011c50: 2020 6465 6620 7465 7374 5f63 7376 5f66    def test_csv_f
-00011c60: 696c 7465 7265 645f 696d 706f 7274 2873  iltered_import(s
-00011c70: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
-00011c80: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
-00011c90: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
-00011ca0: 6528 292e 6373 765f 696d 706f 7274 2822  e().csv_import("
-00011cb0: 7465 7374 2f61 6263 2e63 7376 222c 2074  test/abc.csv", t
-00011cc0: 7261 6e73 666f 726d 733d 6469 6374 2e66  ransforms=dict.f
-00011cd0: 726f 6d6b 6579 7328 2261 6263 222c 2069  romkeys("abc", i
-00011ce0: 6e74 2929 0a20 2020 2020 2020 2070 7269  nt)).        pri
-00011cf0: 6e74 2822 6162 632e 6373 7622 2c20 7474  nt("abc.csv", tt
-00011d00: 2e69 6e66 6f28 2929 0a0a 2020 2020 2020  .info())..      
-00011d10: 2020 7474 203d 206c 742e 5461 626c 6528    tt = lt.Table(
-00011d20: 292e 6373 765f 696d 706f 7274 2822 7465  ).csv_import("te
-00011d30: 7374 2f61 6263 2e63 7376 222c 2074 7261  st/abc.csv", tra
-00011d40: 6e73 666f 726d 733d 6469 6374 2e66 726f  nsforms=dict.fro
-00011d50: 6d6b 6579 7328 2261 6263 222c 2069 6e74  mkeys("abc", int
-00011d60: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d80: 2020 2020 2020 6669 6c74 6572 733d 7b22        filters={"
-00011d90: 6322 3a20 6c74 2e54 6162 6c65 2e65 7128  c": lt.Table.eq(
-00011da0: 3129 7d29 0a20 2020 2020 2020 2070 7269  1)}).        pri
-00011db0: 6e74 2874 742e 696e 666f 2829 290a 2020  nt(tt.info()).  
-00011dc0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00011dd0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00011de0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011df0: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-00011e00: 6520 2a20 7465 7374 5f73 697a 652c 206c  e * test_size, l
-00011e10: 656e 2874 7429 290a 0a20 2020 2020 2020  en(tt))..       
-00011e20: 2074 7420 3d20 6c74 2e54 6162 6c65 2829   tt = lt.Table()
-00011e30: 2e63 7376 5f69 6d70 6f72 7428 2274 6573  .csv_import("tes
-00011e40: 742f 6162 632e 6373 7622 2c20 7472 616e  t/abc.csv", tran
-00011e50: 7366 6f72 6d73 3d64 6963 742e 6672 6f6d  sforms=dict.from
-00011e60: 6b65 7973 2822 6162 6322 2c20 696e 7429  keys("abc", int)
-00011e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2066 696c 7465 7273 3d7b 2263       filters={"c
-00011ea0: 223a 2031 7d29 0a20 2020 2020 2020 2070  ": 1}).        p
-00011eb0: 7269 6e74 2874 742e 696e 666f 2829 290a  rint(tt.info()).
-00011ec0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00011ed0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00011ee0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00011ef0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00011f00: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
-00011f10: 206c 656e 2874 7429 290a 0a20 2020 2020   len(tt))..     
-00011f20: 2020 2074 7420 3d20 6c74 2e54 6162 6c65     tt = lt.Table
-00011f30: 2829 2e63 7376 5f69 6d70 6f72 7428 2274  ().csv_import("t
-00011f40: 6573 742f 6162 632e 6373 7622 2c20 7472  est/abc.csv", tr
-00011f50: 616e 7366 6f72 6d73 3d64 6963 742e 6672  ansforms=dict.fr
-00011f60: 6f6d 6b65 7973 2822 6162 6322 2c20 696e  omkeys("abc", in
-00011f70: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2020 2020 2020 2066 696c 7465 7273 3d7b         filters={
-00011fa0: 2263 223a 206c 616d 6264 6120 783a 2030  "c": lambda x: 0
-00011fb0: 203c 2078 203c 2032 7d29 0a20 2020 2020   < x < 2}).     
-00011fc0: 2020 2070 7269 6e74 2874 742e 696e 666f     print(tt.info
-00011fd0: 2829 290a 2020 2020 2020 2020 7769 7468  ()).        with
-00011fe0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00011ff0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012000: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00012010: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
-00012020: 697a 652c 206c 656e 2874 7429 290a 0a20  ize, len(tt)).. 
-00012030: 2020 2020 2020 2023 2074 6573 7420 616c         # test al
-00012040: 6c20 7370 6563 6961 6c20 636f 6d70 6172  l special compar
-00012050: 6174 6f72 7320 7768 656e 2075 7365 6420  ators when used 
-00012060: 6173 2066 696c 7465 7273 0a20 2020 2020  as filters.     
-00012070: 2020 2023 2020 2020 2069 735f 6e6f 6e65     #     is_none
-00012080: 202d 2061 7474 7269 6275 7465 2076 616c   - attribute val
-00012090: 7565 2069 7320 4e6f 6e65 0a20 2020 2020  ue is None.     
-000120a0: 2020 2023 2020 2020 2069 735f 6e6f 745f     #     is_not_
-000120b0: 6e6f 6e65 202d 2061 7474 7269 6275 7465  none - attribute
-000120c0: 2076 616c 7565 2069 7320 6e6f 7420 4e6f   value is not No
-000120d0: 6e65 0a20 2020 2020 2020 2023 2020 2020  ne.        #    
-000120e0: 2069 735f 6e75 6c6c 202d 2061 7474 7269   is_null - attri
-000120f0: 6275 7465 2076 616c 7565 2069 7320 4e6f  bute value is No
-00012100: 6e65 2c20 2222 2c20 6f72 206e 6f74 2064  ne, "", or not d
-00012110: 6566 696e 6564 0a20 2020 2020 2020 2023  efined.        #
-00012120: 2020 2020 2069 735f 6e6f 745f 6e75 6c6c       is_not_null
-00012130: 202d 2061 7474 7269 6275 7465 2076 616c   - attribute val
-00012140: 7565 2069 7320 6465 6669 6e65 642c 2061  ue is defined, a
-00012150: 6e64 2069 7320 6e6f 7420 4e6f 6e65 206f  nd is not None o
-00012160: 7220 2222 0a20 2020 2020 2020 2023 2020  r "".        #  
-00012170: 2020 2073 7461 7274 7377 6974 6820 2d20     startswith - 
-00012180: 6174 7472 6962 7574 6520 7661 6c75 6520  attribute value 
-00012190: 7374 6172 7473 2077 6974 6820 6120 6769  starts with a gi
-000121a0: 7665 6e20 7374 7269 6e67 0a20 2020 2020  ven string.     
-000121b0: 2020 2023 2020 2020 2065 6e64 7377 6974     #     endswit
-000121c0: 6820 2d20 6174 7472 6962 7574 6520 7661  h - attribute va
-000121d0: 6c75 6520 656e 6473 2077 6974 6820 6120  lue ends with a 
-000121e0: 6769 7665 6e20 7374 7269 6e67 0a20 2020  given string.   
-000121f0: 2020 2020 2023 2020 2020 2072 655f 6d61       #     re_ma
-00012200: 7463 6820 2d20 6174 7472 6962 7574 6520  tch - attribute 
-00012210: 7661 6c75 6520 6d61 7463 6865 7320 6120  value matches a 
-00012220: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-00012230: 6f6e 0a0a 2020 2020 2020 2020 7072 696e  on..        prin
-00012240: 7428 290a 2020 2020 2020 2020 696e 7075  t().        inpu
-00012250: 745f 6461 7461 203d 2074 6578 7477 7261  t_data = textwra
-00012260: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-00012270: 2020 2020 2020 6e61 6d65 2c61 2c62 2c63        name,a,b,c
-00012280: 0a20 2020 2020 2020 2022 4122 2c31 3030  .        "A",100
-00012290: 2c31 3030 2c31 3030 0a20 2020 2020 2020  ,100,100.       
-000122a0: 2022 4222 2c32 3030 2c2c 3230 300a 2020   "B",200,,200.  
-000122b0: 2020 2020 2020 2241 3122 2c31 3031 2c31        "A1",101,1
-000122c0: 3031 2c31 3031 0a20 2020 2020 2020 2022  01,101.        "
-000122d0: 4231 222c 3230 312c 2c32 3031 0a20 2020  B1",201,,201.   
-000122e0: 2020 2020 2022 4331 222c 3330 312c 2c33       "C1",301,,3
-000122f0: 3031 0a20 2020 2020 2020 202c 3939 2c39  01.        ,99,9
-00012300: 392c 3939 0a20 2020 2020 2020 2022 2222  9,99.        """
-00012310: 290a 2020 2020 2020 2020 6c74 2e54 6162  ).        lt.Tab
-00012320: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00012330: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-00012360: 6f72 6d73 3d64 6963 742e 6672 6f6d 6b65  orms=dict.fromke
-00012370: 7973 2822 6162 6322 2c20 696e 7429 2c0a  ys("abc", int),.
-00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 2020 2020 2020 2020 292e                ).
-000123a0: 7072 6573 656e 7428 290a 0a20 2020 2020  present()..     
-000123b0: 2020 2022 2222 0a20 2020 2020 2020 202b     """.        +
-000123c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000123d0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
-000123e0: 2020 207c 204e 616d 6520 7c20 2020 4120     | Name |   A 
-000123f0: 7c20 2020 2042 207c 2020 2043 207c 0a20  |    B |   C |. 
-00012400: 2020 2020 2020 207c 2d2d 2d2d 2d2d 2b2d         |------+-
-00012410: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2b 2d2d 2d2d  ----+------+----
-00012420: 2d7c 0a20 2020 2020 2020 207c 2041 2020  -|.        | A  
-00012430: 2020 7c20 3130 3020 7c20 2031 3030 207c    | 100 |  100 |
-00012440: 2031 3030 207c 0a20 2020 2020 2020 207c   100 |.        |
-00012450: 2042 2020 2020 7c20 3230 3020 7c20 4e6f   B    | 200 | No
-00012460: 6e65 207c 2032 3030 207c 0a20 2020 2020  ne | 200 |.     
-00012470: 2020 207c 2041 3120 2020 7c20 3130 3120     | A1   | 101 
-00012480: 7c20 2031 3031 207c 2031 3031 207c 0a20  |  101 | 101 |. 
-00012490: 2020 2020 2020 207c 2042 3120 2020 7c20         | B1   | 
-000124a0: 3230 3120 7c20 4e6f 6e65 207c 2032 3031  201 | None | 201
-000124b0: 207c 0a20 2020 2020 2020 207c 2043 3120   |.        | C1 
-000124c0: 2020 7c20 3330 3120 7c20 4e6f 6e65 207c    | 301 | None |
-000124d0: 2033 3031 207c 0a20 2020 2020 2020 207c   301 |.        |
-000124e0: 2020 2020 2020 7c20 2039 3920 7c20 2020        |  99 |   
-000124f0: 3939 207c 2020 3939 207c 0a20 2020 2020  99 |  99 |.     
-00012500: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     +------------
-00012510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20  -------------+. 
-00012520: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00012530: 2020 2020 7072 696e 7428 2269 735f 6e6f      print("is_no
-00012540: 6e65 2829 2229 0a20 2020 2020 2020 2078  ne()").        x
-00012550: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-00012560: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
-00012570: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012590: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000125a0: 616e 7366 6f72 6d73 3d64 6963 742e 6672  ansforms=dict.fr
-000125b0: 6f6d 6b65 7973 2822 6162 6322 2c20 696e  omkeys("abc", in
-000125c0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000125f0: 7465 7273 3d7b 2262 223a 206c 742e 5461  ters={"b": lt.Ta
-00012600: 626c 652e 6973 5f6e 6f6e 6528 297d 290a  ble.is_none()}).
-00012610: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00012620: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00012630: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00012640: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
-00012650: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
-00012660: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00012670: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012680: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-00012690: 6c28 6220 6973 204e 6f6e 6520 666f 7220  l(b is None for 
-000126a0: 6220 696e 2078 2e61 6c6c 2e62 2929 0a0a  b in x.all.b))..
-000126b0: 2020 2020 2020 2020 7072 696e 7428 2269          print("i
-000126c0: 735f 6e6f 745f 6e6f 6e65 2829 2229 0a20  s_not_none()"). 
-000126d0: 2020 2020 2020 2078 203d 206c 742e 5461         x = lt.Ta
-000126e0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-000126f0: 2869 6e70 7574 5f64 6174 612c 0a20 2020  (input_data,.   
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012720: 7261 6e73 666f 726d 733d 6469 6374 2e66  ransforms=dict.f
-00012730: 726f 6d6b 6579 7328 2261 6263 222c 2069  romkeys("abc", i
-00012740: 6e74 292c 0a20 2020 2020 2020 2020 2020  nt),.           
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 2020 2066 696c 7465 7273 3d7b         filters={
-00012770: 2262 223a 206c 742e 5461 626c 652e 6973  "b": lt.Table.is
-00012780: 5f6e 6f74 5f6e 6f6e 6528 297d 290a 2020  _not_none()}).  
-00012790: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000127a0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-000127b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000127c0: 7274 4571 7561 6c28 332c 206c 656e 2878  rtEqual(3, len(x
-000127d0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-000127e0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-000127f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012800: 2e61 7373 6572 7445 7175 616c 2833 3030  .assertEqual(300
-00012810: 2c20 7375 6d28 782e 616c 6c2e 6229 290a  , sum(x.all.b)).
-00012820: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00012830: 6220 6973 5f6e 756c 6c28 2922 290a 2020  b is_null()").  
-00012840: 2020 2020 2020 7820 3d20 6c74 2e54 6162        x = lt.Tab
-00012850: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00012860: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012880: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00012890: 616e 7366 6f72 6d73 3d64 6963 742e 6672  ansforms=dict.fr
-000128a0: 6f6d 6b65 7973 2822 6162 6322 2c20 696e  omkeys("abc", in
-000128b0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 2020 2020 2020 6669 6c74 6572 733d 7b22        filters={"
-000128e0: 6222 3a20 6c74 2e54 6162 6c65 2e69 735f  b": lt.Table.is_
-000128f0: 6e75 6c6c 2829 7d29 0a20 2020 2020 2020  null()}).       
-00012900: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00012910: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00012920: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00012930: 616c 2833 2c20 6c65 6e28 7829 290a 2020  al(3, len(x)).  
-00012940: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00012950: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00012960: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00012970: 7274 5472 7565 2861 6c6c 2862 2069 7320  rtTrue(all(b is 
-00012980: 4e6f 6e65 2066 6f72 2062 2069 6e20 782e  None for b in x.
-00012990: 616c 6c2e 6229 290a 0a20 2020 2020 2020  all.b))..       
-000129a0: 2070 7269 6e74 2822 6220 6973 5f6e 6f74   print("b is_not
-000129b0: 5f6e 756c 6c28 2922 290a 2020 2020 2020  _null()").      
-000129c0: 2020 7820 3d20 6c74 2e54 6162 6c65 2829    x = lt.Table()
-000129d0: 2e63 7376 5f69 6d70 6f72 7428 696e 7075  .csv_import(inpu
-000129e0: 745f 6461 7461 2c0a 2020 2020 2020 2020  t_data,.        
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-00012a10: 6f72 6d73 3d64 6963 742e 6672 6f6d 6b65  orms=dict.fromke
-00012a20: 7973 2822 6162 6322 2c20 696e 7429 2c0a  ys("abc", int),.
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 2020 6669 6c74 6572 733d 7b22 6222 3a20    filters={"b": 
-00012a60: 6c74 2e54 6162 6c65 2e69 735f 6e6f 745f  lt.Table.is_not_
-00012a70: 6e75 6c6c 2829 7d29 0a20 2020 2020 2020  null()}).       
-00012a80: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00012a90: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00012aa0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00012ab0: 616c 2833 2c20 6c65 6e28 7829 290a 2020  al(3, len(x)).  
-00012ac0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00012ad0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00012ae0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00012af0: 7274 4571 7561 6c28 3330 302c 2073 756d  rtEqual(300, sum
-00012b00: 2878 2e61 6c6c 2e62 2929 0a0a 2020 2020  (x.all.b))..    
-00012b10: 2020 2020 7072 696e 7428 226e 616d 6520      print("name 
-00012b20: 6973 5f6e 756c 6c28 2922 290a 2020 2020  is_null()").    
-00012b30: 2020 2020 7820 3d20 6c74 2e54 6162 6c65      x = lt.Table
-00012b40: 2829 2e63 7376 5f69 6d70 6f72 7428 696e  ().csv_import(in
-00012b50: 7075 745f 6461 7461 2c0a 2020 2020 2020  put_data,.      
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b70: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-00012b80: 7366 6f72 6d73 3d64 6963 742e 6672 6f6d  sforms=dict.from
-00012b90: 6b65 7973 2822 6162 6322 2c20 696e 7429  keys("abc", int)
-00012ba0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 6669 6c74 6572 733d 7b22 6e61      filters={"na
-00012bd0: 6d65 223a 206c 742e 5461 626c 652e 6973  me": lt.Table.is
-00012be0: 5f6e 756c 6c28 297d 290a 2020 2020 2020  _null()}).      
-00012bf0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00012c00: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00012c10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00012c20: 7561 6c28 312c 206c 656e 2878 2929 0a20  ual(1, len(x)). 
-00012c30: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00012c40: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00012c50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00012c60: 6572 7445 7175 616c 2833 2a39 392c 2078  ertEqual(3*99, x
-00012c70: 5b30 5d2e 6120 2b20 785b 305d 2e62 202b  [0].a + x[0].b +
-00012c80: 2078 5b30 5d2e 6329 0a0a 2020 2020 2020   x[0].c)..      
-00012c90: 2020 7072 696e 7428 226e 616d 6520 6973    print("name is
-00012ca0: 5f6e 6f74 5f6e 756c 6c28 2922 290a 2020  _not_null()").  
-00012cb0: 2020 2020 2020 7820 3d20 6c74 2e54 6162        x = lt.Tab
-00012cc0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00012cd0: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00012d00: 616e 7366 6f72 6d73 3d64 6963 742e 6672  ansforms=dict.fr
-00012d10: 6f6d 6b65 7973 2822 6162 6322 2c20 696e  omkeys("abc", in
-00012d20: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 2020 6669 6c74 6572 733d 7b22        filters={"
-00012d50: 6e61 6d65 223a 206c 742e 5461 626c 652e  name": lt.Table.
-00012d60: 6973 5f6e 6f74 5f6e 756c 6c28 297d 290a  is_not_null()}).
-00012d70: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00012d80: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00012d90: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00012da0: 7365 7274 4571 7561 6c28 352c 206c 656e  sertEqual(5, len
-00012db0: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
-00012dc0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00012dd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012de0: 6c66 2e61 7373 6572 7445 7175 616c 2822  lf.assertEqual("
-00012df0: 4120 4220 4131 2042 3120 4331 222e 7370  A B A1 B1 C1".sp
-00012e00: 6c69 7428 292c 206c 6973 7428 782e 616c  lit(), list(x.al
-00012e10: 6c2e 6e61 6d65 2929 0a0a 2020 2020 2020  l.name))..      
-00012e20: 2020 7072 696e 7428 226e 616d 6520 7374    print("name st
-00012e30: 6172 7473 7769 7468 2827 4227 2922 290a  artswith('B')").
-00012e40: 2020 2020 2020 2020 7820 3d20 6c74 2e54          x = lt.T
-00012e50: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-00012e60: 7428 696e 7075 745f 6461 7461 2c0a 2020  t(input_data,.  
-00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e90: 7472 616e 7366 6f72 6d73 3d64 6963 742e  transforms=dict.
-00012ea0: 6672 6f6d 6b65 7973 2822 6162 6322 2c20  fromkeys("abc", 
-00012eb0: 696e 7429 2c0a 2020 2020 2020 2020 2020  int),.          
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2020 2020 2020 2020 6669 6c74 6572 733d          filters=
-00012ee0: 7b22 6e61 6d65 223a 206c 742e 5461 626c  {"name": lt.Tabl
-00012ef0: 652e 7374 6172 7473 7769 7468 2822 4222  e.startswith("B"
-00012f00: 297d 290a 2020 2020 2020 2020 7769 7468  )}).        with
-00012f10: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00012f20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012f30: 662e 6173 7365 7274 4571 7561 6c28 322c  f.assertEqual(2,
-00012f40: 206c 656e 2878 2929 0a20 2020 2020 2020   len(x)).       
-00012f50: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00012f60: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00012f70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00012f80: 616c 2822 4220 4231 222e 7370 6c69 7428  al("B B1".split(
-00012f90: 292c 206c 6973 7428 782e 616c 6c2e 6e61  ), list(x.all.na
-00012fa0: 6d65 2929 0a0a 2020 2020 2020 2020 7072  me))..        pr
-00012fb0: 696e 7428 226e 616d 6520 656e 6473 7769  int("name endswi
-00012fc0: 7468 2827 3127 2922 290a 2020 2020 2020  th('1')").      
-00012fd0: 2020 7820 3d20 6c74 2e54 6162 6c65 2829    x = lt.Table()
-00012fe0: 2e63 7376 5f69 6d70 6f72 7428 696e 7075  .csv_import(inpu
-00012ff0: 745f 6461 7461 2c0a 2020 2020 2020 2020  t_data,.        
-00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-00013020: 6f72 6d73 3d64 6963 742e 6672 6f6d 6b65  orms=dict.fromke
-00013030: 7973 2822 6162 6322 2c20 696e 7429 2c0a  ys("abc", int),.
-00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2020 6669 6c74 6572 733d 7b22 6e61 6d65    filters={"name
-00013070: 223a 206c 742e 5461 626c 652e 656e 6473  ": lt.Table.ends
-00013080: 7769 7468 2822 3122 297d 290a 2020 2020  with("1")}).    
-00013090: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000130a0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000130b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000130c0: 4571 7561 6c28 332c 206c 656e 2878 2929  Equal(3, len(x))
-000130d0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000130e0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-000130f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00013100: 7373 6572 7445 7175 616c 2822 4131 2042  ssertEqual("A1 B
-00013110: 3120 4331 222e 7370 6c69 7428 292c 206c  1 C1".split(), l
-00013120: 6973 7428 782e 616c 6c2e 6e61 6d65 2929  ist(x.all.name))
-00013130: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00013140: 7222 6e61 6d65 2072 655f 6d61 7463 6828  r"name re_match(
-00013150: 7227 5b41 425d 5c64 2729 2229 0a20 2020  r'[AB]\d')").   
-00013160: 2020 2020 2078 203d 206c 742e 5461 626c       x = lt.Tabl
-00013170: 6528 292e 6373 765f 696d 706f 7274 2869  e().csv_import(i
-00013180: 6e70 7574 5f64 6174 612c 0a20 2020 2020  nput_data,.     
-00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000131b0: 6e73 666f 726d 733d 6469 6374 2e66 726f  nsforms=dict.fro
-000131c0: 6d6b 6579 7328 2261 6263 222c 2069 6e74  mkeys("abc", int
-000131d0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 2020 2066 696c 7465 7273 3d7b 226e       filters={"n
-00013200: 616d 6522 3a20 6c74 2e54 6162 6c65 2e72  ame": lt.Table.r
-00013210: 655f 6d61 7463 6828 7222 5b41 425d 5c64  e_match(r"[AB]\d
-00013220: 2229 7d29 0a20 2020 2020 2020 2077 6974  ")}).        wit
-00013230: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00013240: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00013250: 6c66 2e61 7373 6572 7445 7175 616c 2832  lf.assertEqual(2
-00013260: 2c20 6c65 6e28 7829 290a 2020 2020 2020  , len(x)).      
-00013270: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00013280: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00013290: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000132a0: 7561 6c28 2241 3120 4231 222e 7370 6c69  ual("A1 B1".spli
-000132b0: 7428 292c 206c 6973 7428 782e 616c 6c2e  t(), list(x.all.
-000132c0: 6e61 6d65 2929 0a0a 2020 2020 6465 6620  name))..    def 
-000132d0: 7465 7374 5f63 7376 5f73 7472 696e 675f  test_csv_string_
-000132e0: 696d 706f 7274 2873 656c 6629 3a0a 2020  import(self):.  
-000132f0: 2020 2020 2020 6461 7461 203d 2063 7376        data = csv
-00013300: 5f64 6174 610a 2020 2020 2020 2020 6373  _data.        cs
-00013310: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
-00013320: 6528 292e 6373 765f 696d 706f 7274 2863  e().csv_import(c
-00013330: 7376 5f73 6f75 7263 653d 6461 7461 2c20  sv_source=data, 
-00013340: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
-00013350: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
-00013360: 2763 273a 2069 6e74 7d29 0a0a 2020 2020  'c': int})..    
-00013370: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00013380: 330a 2020 2020 2020 2020 7431 203d 206d  3.        t1 = m
-00013390: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000133a0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000133b0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000133c0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-000133d0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-000133e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000133f0: 6173 7365 7274 5472 7565 2861 6c6c 286d  assertTrue(all(m
-00013400: 616b 655f 6461 7461 6f62 6a65 6374 5f66  ake_dataobject_f
-00013410: 726f 6d5f 6f62 2872 6563 3129 203d 3d20  rom_ob(rec1) == 
-00013420: 7265 6332 2066 6f72 2072 6563 312c 2072  rec2 for rec1, r
-00013430: 6563 3220 696e 207a 6970 2874 312c 2063  ec2 in zip(t1, c
-00013440: 7376 7461 626c 6529 2929 0a20 2020 2020  svtable))).     
-00013450: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00013460: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00013470: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00013480: 7175 616c 2873 756d 2831 2066 6f72 206c  qual(sum(1 for l
-00013490: 696e 6520 696e 2064 6174 612e 7370 6c69  ine in data.spli
-000134a0: 746c 696e 6573 2829 2069 6620 6c69 6e65  tlines() if line
-000134b0: 2e73 7472 6970 2829 292d 312c 206c 656e  .strip())-1, len
-000134c0: 2863 7376 7461 626c 6529 290a 0a20 2020  (csvtable))..   
-000134d0: 2020 2020 2072 6f77 5f70 726f 746f 7479       row_prototy
-000134e0: 7065 203d 2073 656c 662e 6d61 6b65 5f64  pe = self.make_d
-000134f0: 6174 615f 6f62 6a65 6374 2830 2c20 302c  ata_object(0, 0,
-00013500: 2030 290a 2020 2020 2020 2020 6373 7674   0).        csvt
-00013510: 6162 6c65 3220 3d20 6c74 2e54 6162 6c65  able2 = lt.Table
-00013520: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
-00013530: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
-00013540: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
-00013550: 6e74 2c20 2763 273a 2069 6e74 7d2c 0a20  nt, 'c': int},. 
-00013560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 2020 2020 2020 2020 2072 6f77 5f63 6c61           row_cla
-00013590: 7373 3d74 7970 6528 726f 775f 7072 6f74  ss=type(row_prot
-000135a0: 6f74 7970 6529 295b 3a33 5d0a 0a20 2020  otype))[:3]..   
-000135b0: 2020 2020 2070 7269 6e74 2874 7970 6528       print(type(
-000135c0: 7431 5b30 5d29 2e5f 5f6e 616d 655f 5f2c  t1[0]).__name__,
-000135d0: 2074 315b 305d 290a 2020 2020 2020 2020   t1[0]).        
-000135e0: 7072 696e 7428 7479 7065 2863 7376 7461  print(type(csvta
-000135f0: 626c 6532 5b30 5d29 2e5f 5f6e 616d 655f  ble2[0]).__name_
-00013600: 5f2c 2063 7376 7461 626c 6532 5b30 5d29  _, csvtable2[0])
-00013610: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00013620: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00013630: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00013640: 7373 6572 7445 7175 616c 2874 7970 6528  ssertEqual(type(
-00013650: 7431 5b30 5d29 2c20 7479 7065 2863 7376  t1[0]), type(csv
-00013660: 7461 626c 6532 5b30 5d29 290a 0a20 2020  table2[0]))..   
-00013670: 2064 6566 2074 6573 745f 6373 765f 6c69   def test_csv_li
-00013680: 6d69 745f 696d 706f 7274 2873 656c 6629  mit_import(self)
-00013690: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-000136a0: 2063 7376 5f64 6174 610a 2020 2020 2020   csv_data.      
-000136b0: 2020 696d 706f 7274 5f6c 696d 6974 203d    import_limit =
-000136c0: 2031 300a 2020 2020 2020 2020 6373 7674   10.        csvt
-000136d0: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
-000136e0: 292e 6373 765f 696d 706f 7274 2863 7376  ).csv_import(csv
-000136f0: 5f73 6f75 7263 653d 6461 7461 2c20 7472  _source=data, tr
-00013700: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
-00013710: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
-00013720: 273a 2069 6e74 7d2c 0a20 2020 2020 2020  ': int},.       
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 2020 6c69 6d69 743d 696d 706f 7274 5f6c    limit=import_l
-00013760: 696d 6974 290a 0a20 2020 2020 2020 2077  imit)..        w
-00013770: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00013780: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00013790: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000137a0: 2869 6d70 6f72 745f 6c69 6d69 742c 206c  (import_limit, l
-000137b0: 656e 2863 7376 7461 626c 6529 290a 0a20  en(csvtable)).. 
-000137c0: 2020 2020 2020 2063 7376 7461 626c 6520         csvtable 
-000137d0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-000137e0: 5f69 6d70 6f72 7428 6373 765f 736f 7572  _import(csv_sour
-000137f0: 6365 3d64 6174 612c 2074 7261 6e73 666f  ce=data, transfo
-00013800: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
-00013810: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
-00013820: 747d 2c0a 2020 2020 2020 2020 2020 2020  t},.            
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 2020 206c 696d               lim
-00013850: 6974 3d30 290a 0a20 2020 2020 2020 2077  it=0)..        w
-00013860: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00013870: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00013880: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00013890: 2830 2c20 6c65 6e28 6373 7674 6162 6c65  (0, len(csvtable
-000138a0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-000138b0: 5f63 7376 5f73 7472 696e 675f 6c69 7374  _csv_string_list
-000138c0: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
-000138d0: 2020 2020 2020 2064 6174 6120 3d20 6373         data = cs
-000138e0: 765f 6461 7461 0a20 2020 2020 2020 2063  v_data.        c
-000138f0: 7376 7461 626c 6520 3d20 6c74 2e54 6162  svtable = lt.Tab
-00013900: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00013910: 6373 765f 736f 7572 6365 3d64 6174 612e  csv_source=data.
-00013920: 7370 6c69 746c 696e 6573 2829 2c20 7472  splitlines(), tr
-00013930: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
-00013940: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
-00013950: 273a 2069 6e74 7d29 0a0a 2020 2020 2020  ': int})..      
-00013960: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
-00013970: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
-00013980: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
-00013990: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-000139a0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
-000139b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000139c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000139d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000139e0: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
-000139f0: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
-00013a00: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
-00013a10: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
-00013a20: 3220 696e 207a 6970 2874 312c 2063 7376  2 in zip(t1, csv
-00013a30: 7461 626c 6529 2929 0a20 2020 2020 2020  table))).       
-00013a40: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00013a50: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00013a60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00013a70: 616c 2873 756d 2831 2066 6f72 206c 696e  al(sum(1 for lin
-00013a80: 6520 696e 2064 6174 612e 7370 6c69 746c  e in data.splitl
-00013a90: 696e 6573 2829 2069 6620 6c69 6e65 2e73  ines() if line.s
-00013aa0: 7472 6970 2829 292d 312c 206c 656e 2863  trip())-1, len(c
-00013ab0: 7376 7461 626c 6529 290a 0a20 2020 2020  svtable))..     
-00013ac0: 2020 2072 6f77 5f70 726f 746f 7479 7065     row_prototype
-00013ad0: 203d 2073 656c 662e 6d61 6b65 5f64 6174   = self.make_dat
-00013ae0: 615f 6f62 6a65 6374 2830 2c20 302c 2030  a_object(0, 0, 0
-00013af0: 290a 2020 2020 2020 2020 6373 7674 6162  ).        csvtab
-00013b00: 6c65 3220 3d20 6c74 2e54 6162 6c65 2829  le2 = lt.Table()
-00013b10: 2e63 7376 5f69 6d70 6f72 7428 6461 7461  .csv_import(data
-00013b20: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
-00013b30: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
-00013b40: 2c20 2763 273a 2069 6e74 7d2c 0a20 2020  , 'c': int},.   
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b70: 2020 2020 2020 2072 6f77 5f63 6c61 7373         row_class
-00013b80: 3d74 7970 6528 726f 775f 7072 6f74 6f74  =type(row_protot
-00013b90: 7970 6529 295b 3a33 5d0a 0a20 2020 2020  ype))[:3]..     
-00013ba0: 2020 2070 7269 6e74 2874 7970 6528 7431     print(type(t1
-00013bb0: 5b30 5d29 2e5f 5f6e 616d 655f 5f2c 2074  [0]).__name__, t
-00013bc0: 315b 305d 290a 2020 2020 2020 2020 7072  1[0]).        pr
-00013bd0: 696e 7428 7479 7065 2863 7376 7461 626c  int(type(csvtabl
-00013be0: 6532 5b30 5d29 2e5f 5f6e 616d 655f 5f2c  e2[0]).__name__,
-00013bf0: 2063 7376 7461 626c 6532 5b30 5d29 0a20   csvtable2[0]). 
-00013c00: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00013c10: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00013c20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00013c30: 6572 7445 7175 616c 2874 7970 6528 7431  ertEqual(type(t1
-00013c40: 5b30 5d29 2c20 7479 7065 2863 7376 7461  [0]), type(csvta
-00013c50: 626c 6532 5b30 5d29 290a 0a20 2020 2064  ble2[0]))..    d
-00013c60: 6566 2074 6573 745f 6373 765f 6e75 6d65  ef test_csv_nume
-00013c70: 7269 635f 7472 616e 7366 6f72 6d73 2873  ric_transforms(s
-00013c80: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00013c90: 7461 203d 2074 6578 7477 7261 702e 6465  ta = textwrap.de
-00013ca0: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
-00013cb0: 2020 2020 2020 7479 7065 2c76 616c 7565        type,value
-00013cc0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-00013cd0: 2c31 3030 300a 2020 2020 2020 2020 2020  ,1000.          
-00013ce0: 2020 666c 6f61 742c 332e 3134 0a20 2020    float,3.14.   
-00013cf0: 2020 2020 2020 2020 2065 6d70 7479 2c0a           empty,.
-00013d00: 2020 2020 2020 2020 2020 2020 7374 722c              str,
-00013d10: e293 a02a 6265 7274 0a20 2020 2020 2020  ...*bert.       
-00013d20: 2020 2020 2022 2222 290a 0a20 2020 2020       """)..     
-00013d30: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00013d40: 5465 7374 2822 636f 6e76 6572 745f 6e75  Test("convert_nu
-00013d50: 6d65 7269 6322 293a 0a20 2020 2020 2020  meric"):.       
-00013d60: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
-00013d70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00013d80: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
-00013d90: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
-00013da0: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
-00013db0: 6572 6963 7d29 0a20 2020 2020 2020 2020  eric}).         
-00013dc0: 2020 2074 626c 2e70 7265 7365 6e74 2829     tbl.present()
-00013dd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013de0: 662e 6173 7365 7274 4571 7561 6c28 5b31  f.assertEqual([1
-00013df0: 3030 302c 2033 2e31 342c 2027 272c 2027  000, 3.14, '', '
-00013e00: e293 a02a 6265 7274 275d 2c20 6c69 7374  ...*bert'], list
-00013e10: 2874 626c 2e61 6c6c 2e76 616c 7565 2929  (tbl.all.value))
-00013e20: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00013e30: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
-00013e40: 7665 7274 5f6e 756d 6572 6963 2829 2229  vert_numeric()")
-00013e50: 3a0a 2020 2020 2020 2020 2020 2020 7462  :.            tb
-00013e60: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e63  l = lt.Table().c
-00013e70: 7376 5f69 6d70 6f72 7428 6461 7461 2c20  sv_import(data, 
-00013e80: 7472 616e 7366 6f72 6d73 3d7b 2776 616c  transforms={'val
-00013e90: 7565 273a 206c 742e 5461 626c 652e 636f  ue': lt.Table.co
-00013ea0: 6e76 6572 745f 6e75 6d65 7269 6328 297d  nvert_numeric()}
-00013eb0: 290a 2020 2020 2020 2020 2020 2020 7462  ).            tb
-00013ec0: 6c2e 7072 6573 656e 7428 290a 2020 2020  l.present().    
-00013ed0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00013ee0: 6572 7445 7175 616c 285b 3130 3030 2c20  ertEqual([1000, 
-00013ef0: 332e 3134 2c20 2727 2c20 27e2 93a0 2a62  3.14, '', '...*b
-00013f00: 6572 7427 5d2c 206c 6973 7428 7462 6c2e  ert'], list(tbl.
-00013f10: 616c 6c2e 7661 6c75 6529 290a 0a20 2020  all.value))..   
-00013f20: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00013f30: 7562 5465 7374 2822 636f 6e76 6572 745f  ubTest("convert_
-00013f40: 6e75 6d65 7269 6328 6e6f 6e5f 6e75 6d65  numeric(non_nume
-00013f50: 7269 633d 4e6f 6e65 2922 293a 0a20 2020  ric=None)"):.   
-00013f60: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
-00013f70: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-00013f80: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
-00013f90: 666f 726d 733d 7b27 7661 6c75 6527 3a20  forms={'value': 
-00013fa0: 6c74 2e54 6162 6c65 2e63 6f6e 7665 7274  lt.Table.convert
-00013fb0: 5f6e 756d 6572 6963 286e 6f6e 5f6e 756d  _numeric(non_num
-00013fc0: 6572 6963 3d4e 6f6e 6529 7d29 0a20 2020  eric=None)}).   
-00013fd0: 2020 2020 2020 2020 2074 626c 2e70 7265           tbl.pre
-00013fe0: 7365 6e74 2829 0a20 2020 2020 2020 2020  sent().         
-00013ff0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00014000: 7561 6c28 5b31 3030 302c 2033 2e31 342c  ual([1000, 3.14,
-00014010: 2027 272c 204e 6f6e 655d 2c20 6c69 7374   '', None], list
-00014020: 2874 626c 2e61 6c6c 2e76 616c 7565 2929  (tbl.all.value))
-00014030: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00014040: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
-00014050: 7665 7274 5f6e 756d 6572 6963 286e 6f6e  vert_numeric(non
-00014060: 5f6e 756d 6572 6963 3d30 2922 293a 0a20  _numeric=0)"):. 
-00014070: 2020 2020 2020 2020 2020 2074 626c 203d             tbl =
-00014080: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00014090: 696d 706f 7274 2864 6174 612c 2074 7261  import(data, tra
-000140a0: 6e73 666f 726d 733d 7b27 7661 6c75 6527  nsforms={'value'
-000140b0: 3a20 6c74 2e54 6162 6c65 2e63 6f6e 7665  : lt.Table.conve
-000140c0: 7274 5f6e 756d 6572 6963 286e 6f6e 5f6e  rt_numeric(non_n
-000140d0: 756d 6572 6963 3d30 297d 290a 2020 2020  umeric=0)}).    
-000140e0: 2020 2020 2020 2020 7462 6c2e 7072 6573          tbl.pres
-000140f0: 656e 7428 290a 2020 2020 2020 2020 2020  ent().          
-00014100: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00014110: 616c 285b 3130 3030 2c20 332e 3134 2c20  al([1000, 3.14, 
-00014120: 2727 2c20 305d 2c20 6c69 7374 2874 626c  '', 0], list(tbl
-00014130: 2e61 6c6c 2e76 616c 7565 2929 0a0a 2020  .all.value))..  
-00014140: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00014150: 7375 6254 6573 7428 2263 6f6e 7665 7274  subTest("convert
-00014160: 5f6e 756d 6572 6963 2869 6e74 5f74 6f5f  _numeric(int_to_
-00014170: 666c 6f61 743d 5472 7565 2922 293a 0a20  float=True)"):. 
-00014180: 2020 2020 2020 2020 2020 2074 626c 203d             tbl =
-00014190: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-000141a0: 696d 706f 7274 2864 6174 612c 2074 7261  import(data, tra
-000141b0: 6e73 666f 726d 733d 7b27 7661 6c75 6527  nsforms={'value'
-000141c0: 3a20 6c74 2e54 6162 6c65 2e63 6f6e 7665  : lt.Table.conve
-000141d0: 7274 5f6e 756d 6572 6963 2866 6f72 6365  rt_numeric(force
-000141e0: 5f66 6c6f 6174 3d54 7275 6529 7d29 0a20  _float=True)}). 
-000141f0: 2020 2020 2020 2020 2020 2074 626c 2e70             tbl.p
-00014200: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-00014210: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00014220: 4571 7561 6c28 5b31 3030 302e 302c 2033  Equal([1000.0, 3
-00014230: 2e31 342c 2027 272c 2027 e293 a02a 6265  .14, '', '...*be
-00014240: 7274 275d 2c20 6c69 7374 2874 626c 2e61  rt'], list(tbl.a
-00014250: 6c6c 2e76 616c 7565 2929 0a20 2020 2020  ll.value)).     
-00014260: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00014270: 7274 4571 7561 6c28 5b66 6c6f 6174 2c20  rtEqual([float, 
-00014280: 666c 6f61 742c 2073 7472 2c20 7374 725d  float, str, str]
-00014290: 2c20 6c69 7374 2874 7970 6528 7629 2066  , list(type(v) f
-000142a0: 6f72 2076 2069 6e20 7462 6c2e 616c 6c2e  or v in tbl.all.
-000142b0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
-000142c0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-000142d0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
-000142e0: 7269 6328 6e6f 6e5f 6e75 6d65 7269 633d  ric(non_numeric=
-000142f0: 4e6f 6e65 2c20 656d 7074 793d 4e6f 6e65  None, empty=None
-00014300: 2922 293a 0a20 2020 2020 2020 2020 2020  )"):.           
-00014310: 2074 626c 203d 206c 742e 5461 626c 6528   tbl = lt.Table(
-00014320: 292e 6373 765f 696d 706f 7274 2864 6174  ).csv_import(dat
-00014330: 612c 2074 7261 6e73 666f 726d 733d 7b27  a, transforms={'
-00014340: 7661 6c75 6527 3a20 6c74 2e54 6162 6c65  value': lt.Table
-00014350: 2e63 6f6e 7665 7274 5f6e 756d 6572 6963  .convert_numeric
-00014360: 286e 6f6e 5f6e 756d 6572 6963 3d4e 6f6e  (non_numeric=Non
-00014370: 652c 2065 6d70 7479 3d4e 6f6e 6529 7d29  e, empty=None)})
-00014380: 0a20 2020 2020 2020 2020 2020 2074 626c  .            tbl
-00014390: 2e70 7265 7365 6e74 2829 0a20 2020 2020  .present().     
-000143a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000143b0: 7274 4571 7561 6c28 5b31 3030 302c 2033  rtEqual([1000, 3
-000143c0: 2e31 342c 204e 6f6e 652c 204e 6f6e 655d  .14, None, None]
-000143d0: 2c20 6c69 7374 2874 626c 2e61 6c6c 2e76  , list(tbl.all.v
-000143e0: 616c 7565 2929 0a0a 2020 2020 2020 2020  alue))..        
-000143f0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00014400: 7428 2263 6f6e 7665 7274 5f6e 756d 6572  t("convert_numer
-00014410: 6963 2865 6d70 7479 3d4e 6f6e 6529 2229  ic(empty=None)")
-00014420: 3a0a 2020 2020 2020 2020 2020 2020 7462  :.            tb
-00014430: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e63  l = lt.Table().c
-00014440: 7376 5f69 6d70 6f72 7428 6461 7461 2c20  sv_import(data, 
-00014450: 7472 616e 7366 6f72 6d73 3d7b 2776 616c  transforms={'val
-00014460: 7565 273a 206c 742e 5461 626c 652e 636f  ue': lt.Table.co
-00014470: 6e76 6572 745f 6e75 6d65 7269 6328 656d  nvert_numeric(em
-00014480: 7074 793d 4e6f 6e65 297d 290a 2020 2020  pty=None)}).    
-00014490: 2020 2020 2020 2020 7462 6c2e 7072 6573          tbl.pres
-000144a0: 656e 7428 290a 2020 2020 2020 2020 2020  ent().          
-000144b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000144c0: 616c 285b 3130 3030 2c20 332e 3134 2c20  al([1000, 3.14, 
-000144d0: 4e6f 6e65 2c20 27e2 93a0 2a62 6572 7427  None, '...*bert'
-000144e0: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
-000144f0: 7661 6c75 6529 290a 0a20 2020 2064 6566  value))..    def
-00014500: 2074 6573 745f 6a73 6f6e 5f65 7870 6f72   test_json_expor
-00014510: 745f 7374 7265 616d 696e 6728 7365 6c66  t_streaming(self
-00014520: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
-00014530: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-00014540: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
-00014550: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00014560: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-00014570: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00014580: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00014590: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-000145a0: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
-000145b0: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
-000145c0: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
-000145d0: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
-000145e0: 2020 2020 6f75 745f 7374 7269 6e67 203d      out_string =
-000145f0: 2074 312e 6a73 6f6e 5f65 7870 6f72 7428   t1.json_export(
-00014600: 4e6f 6e65 2c20 6669 656c 646e 616d 6573  None, fieldnames
-00014610: 3d66 6965 6c64 6e61 6d65 732c 2073 7472  =fieldnames, str
-00014620: 6561 6d69 6e67 3d54 7275 6529 0a20 2020  eaming=True).   
-00014630: 2020 2020 2020 2020 206f 7574 6c69 6e65           outline
-00014640: 7320 3d20 6f75 745f 7374 7269 6e67 2e73  s = out_string.s
-00014650: 706c 6974 6c69 6e65 7328 290a 0a20 2020  plitlines()..   
-00014660: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-00014670: 6c66 2e73 7562 5465 7374 2866 6965 6c64  lf.subTest(field
-00014680: 6e61 6d65 733d 6669 656c 646e 616d 6573  names=fieldnames
-00014690: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000146a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000146b0: 7561 6c28 7465 7374 5f73 697a 652a 2a33  ual(test_size**3
-000146c0: 2c20 6c65 6e28 6f75 746c 696e 6573 2929  , len(outlines))
-000146d0: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-000146e0: 7220 6f62 2c20 6c69 6e65 2069 6e20 7a69  r ob, line in zi
-000146f0: 7028 7431 2c20 6f75 746c 696e 6573 293a  p(t1, outlines):
-00014700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014710: 206a 736f 6e5f 6469 6374 203d 206a 736f   json_dict = jso
-00014720: 6e2e 6c6f 6164 7328 6c69 6e65 290a 2020  n.loads(line).  
-00014730: 2020 2020 2020 2020 2020 2020 2020 7431                t1
-00014740: 5f64 6174 616f 626a 203d 206d 616b 655f  _dataobj = make_
-00014750: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
-00014760: 6f62 286f 6229 0a20 2020 2020 2020 2020  ob(ob).         
-00014770: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00014780: 2e73 7562 5465 7374 286f 623d 6f62 2c20  .subTest(ob=ob, 
-00014790: 6c69 6e65 3d6c 696e 6529 3a0a 2020 2020  line=line):.    
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000147c0: 2874 315f 6461 7461 6f62 6a2c 206c 742e  (t1_dataobj, lt.
-000147d0: 4461 7461 4f62 6a65 6374 282a 2a6a 736f  DataObject(**jso
-000147e0: 6e5f 6469 6374 2929 0a0a 2020 2020 6465  n_dict))..    de
-000147f0: 6620 7465 7374 5f6a 736f 6e5f 6578 706f  f test_json_expo
-00014800: 7274 5f6e 6f6e 7374 7265 616d 696e 6728  rt_nonstreaming(
-00014810: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-00014820: 726f 6d20 6974 6572 746f 6f6c 7320 696d  rom itertools im
-00014830: 706f 7274 2070 6572 6d75 7461 7469 6f6e  port permutation
-00014840: 730a 2020 2020 2020 2020 696d 706f 7274  s.        import
-00014850: 206a 736f 6e0a 2020 2020 2020 2020 7465   json.        te
-00014860: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
-00014870: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
-00014880: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-00014890: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-000148a0: 7465 7374 5f73 697a 6529 0a20 2020 2020  test_size).     
-000148b0: 2020 2066 6f72 2066 6965 6c64 6e61 6d65     for fieldname
-000148c0: 7320 696e 2070 6572 6d75 7461 7469 6f6e  s in permutation
-000148d0: 7328 6c69 7374 2827 6162 6327 2929 3a0a  s(list('abc')):.
-000148e0: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
-000148f0: 7374 7269 6e67 203d 2074 312e 6a73 6f6e  string = t1.json
-00014900: 5f65 7870 6f72 7428 4e6f 6e65 2c20 6669  _export(None, fi
-00014910: 656c 646e 616d 6573 3d66 6965 6c64 6e61  eldnames=fieldna
-00014920: 6d65 732c 2073 7472 6561 6d69 6e67 3d46  mes, streaming=F
-00014930: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00014940: 2020 6f62 7365 7276 6564 5f6a 736f 6e20    observed_json 
-00014950: 3d20 6a73 6f6e 2e6c 6f61 6473 286f 7574  = json.loads(out
-00014960: 5f73 7472 696e 6729 0a0a 2020 2020 2020  _string)..      
-00014970: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00014980: 7375 6254 6573 7428 6669 656c 646e 616d  subTest(fieldnam
-00014990: 6573 3d66 6965 6c64 6e61 6d65 7329 3a0a  es=fieldnames):.
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000149c0: 2874 6573 745f 7369 7a65 2a2a 332c 206c  (test_size**3, l
-000149d0: 656e 286f 6273 6572 7665 645f 6a73 6f6e  en(observed_json
-000149e0: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-000149f0: 666f 7220 6f62 2c20 6a73 6f6e 5f64 6963  for ob, json_dic
-00014a00: 7420 696e 207a 6970 2874 312c 206f 6273  t in zip(t1, obs
-00014a10: 6572 7665 645f 6a73 6f6e 293a 0a20 2020  erved_json):.   
-00014a20: 2020 2020 2020 2020 2020 2020 2074 315f               t1_
-00014a30: 6461 7461 6f62 6a20 3d20 6d61 6b65 5f64  dataobj = make_d
-00014a40: 6174 616f 626a 6563 745f 6672 6f6d 5f6f  ataobject_from_o
-00014a50: 6228 6f62 290a 2020 2020 2020 2020 2020  b(ob).          
-00014a60: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00014a70: 7375 6254 6573 7428 6f62 3d6f 622c 206a  subTest(ob=ob, j
-00014a80: 736f 6e5f 6469 6374 3d6a 736f 6e5f 6469  son_dict=json_di
-00014a90: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-00014aa0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00014ab0: 7365 7274 4571 7561 6c28 7431 5f64 6174  sertEqual(t1_dat
-00014ac0: 616f 626a 2c20 6c74 2e44 6174 614f 626a  aobj, lt.DataObj
-00014ad0: 6563 7428 2a2a 6a73 6f6e 5f64 6963 7429  ect(**json_dict)
-00014ae0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00014af0: 6a73 6f6e 5f69 6d70 6f72 7428 7365 6c66  json_import(self
-00014b00: 293a 0a20 2020 2020 2020 2064 6174 6120  ):.        data 
-00014b10: 3d20 6a73 6f6e 5f64 6174 610a 2020 2020  = json_data.    
-00014b20: 2020 2020 696e 6a73 6f6e 203d 2069 6f2e      injson = io.
-00014b30: 5374 7269 6e67 494f 2864 6174 6129 0a20  StringIO(data). 
-00014b40: 2020 2020 2020 206a 736f 6e74 6162 6c65         jsontable
-00014b50: 203d 206c 742e 5461 626c 6528 292e 6a73   = lt.Table().js
-00014b60: 6f6e 5f69 6d70 6f72 7428 696e 6a73 6f6e  on_import(injson
-00014b70: 2c20 7374 7265 616d 696e 673d 5472 7565  , streaming=True
-00014b80: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
-00014b90: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
-00014ba0: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
-00014bb0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00014bc0: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-00014bd0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00014be0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00014bf0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-00014c00: 6529 0a0a 2020 2020 2020 2020 7769 7468  e)..        with
-00014c10: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00014c20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014c30: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
-00014c40: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
-00014c50: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
-00014c60: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
-00014c70: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
-00014c80: 206a 736f 6e74 6162 6c65 2929 290a 2020   jsontable))).  
-00014c90: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00014ca0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00014cb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00014cc0: 7274 4571 7561 6c28 6c65 6e28 5b64 2066  rtEqual(len([d f
-00014cd0: 6f72 2064 2069 6e20 6461 7461 2e73 706c  or d in data.spl
-00014ce0: 6974 6c69 6e65 7328 2920 6966 2064 2e73  itlines() if d.s
-00014cf0: 7472 6970 2829 5d29 2c20 6c65 6e28 6a73  trip()]), len(js
-00014d00: 6f6e 7461 626c 6529 290a 0a20 2020 2064  ontable))..    d
-00014d10: 6566 2074 6573 745f 6a73 6f6e 5f73 7472  ef test_json_str
-00014d20: 696e 675f 696d 706f 7274 2873 656c 6629  ing_import(self)
-00014d30: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-00014d40: 206a 736f 6e5f 6461 7461 0a20 2020 2020   json_data.     
-00014d50: 2020 206a 736f 6e74 6162 6c65 203d 206c     jsontable = l
-00014d60: 742e 5461 626c 6528 292e 6a73 6f6e 5f69  t.Table().json_i
-00014d70: 6d70 6f72 7428 6461 7461 2c20 7374 7265  mport(data, stre
-00014d80: 616d 696e 673d 5472 7565 2c20 7472 616e  aming=True, tran
-00014d90: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
-00014da0: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
-00014db0: 2069 6e74 7d29 0a0a 2020 2020 2020 2020   int})..        
-00014dc0: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
-00014dd0: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
-00014de0: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
-00014df0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00014e00: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
-00014e10: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00014e20: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00010a50: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00010a60: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00010a70: 7365 7274 4571 7561 6c28 7479 7065 2874  sertEqual(type(t
+00010a80: 315b 305d 292c 2074 7970 6528 6373 7674  1[0]), type(csvt
+00010a90: 6162 6c65 325b 305d 2929 0a0a 2020 2020  able2[0]))..    
+00010aa0: 6465 6620 7465 7374 5f63 7376 5f63 6f6d  def test_csv_com
+00010ab0: 7072 6573 7365 645f 696d 706f 7274 2873  pressed_import(s
+00010ac0: 656c 6629 3a0a 0a20 2020 2020 2020 2064  elf):..        d
+00010ad0: 6566 2076 6572 6966 795f 7469 6d65 7374  ef verify_timest
+00010ae0: 616d 7073 2874 312c 2074 322c 2069 6e66  amps(t1, t2, inf
+00010af0: 6f5f 6469 6374 293a 0a20 2020 2020 2020  o_dict):.       
+00010b00: 2020 2020 2066 6f72 2074 696d 6573 7461       for timesta
+00010b10: 6d70 5f61 7474 725f 6e61 6d65 2069 6e20  mp_attr_name in 
+00010b20: 2263 7265 6174 6564 206d 6f64 6966 6965  "created modifie
+00010b30: 6420 6c61 7374 5f69 6d70 6f72 7422 2e73  d last_import".s
+00010b40: 706c 6974 2829 3a0a 2020 2020 2020 2020  plit():.        
+00010b50: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+00010b60: 705f 7661 6c75 6520 3d20 696e 666f 5f64  p_value = info_d
+00010b70: 6963 742e 706f 7028 7469 6d65 7374 616d  ict.pop(timestam
+00010b80: 705f 6174 7472 5f6e 616d 6529 0a20 2020  p_attr_name).   
+00010b90: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00010ba0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00010bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010bc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00010bd0: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
+00010be0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010bf0: 3120 3c3d 2074 696d 6573 7461 6d70 5f76  1 <= timestamp_v
+00010c00: 616c 7565 203c 3d20 7432 2c0a 2020 2020  alue <= t2,.    
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c20: 2020 2020 6622 696e 636f 7272 6563 7420      f"incorrect 
+00010c30: 7b74 696d 6573 7461 6d70 5f61 7474 725f  {timestamp_attr_
+00010c40: 6e61 6d65 7d20 7469 6d65 220a 2020 2020  name} time".    
+00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c60: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00010c70: 7469 6d65 7374 616d 705f 7374 6172 745f  timestamp_start_
+00010c80: 656e 6428 2920 6173 2074 696d 696e 673a  end() as timing:
+00010c90: 0a20 2020 2020 2020 2020 2020 2074 7420  .            tt 
+00010ca0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00010cb0: 5f69 6d70 6f72 7428 2274 6573 742f 6162  _import("test/ab
+00010cc0: 632e 6373 7622 2c20 7472 616e 7366 6f72  c.csv", transfor
+00010cd0: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
+00010ce0: 2822 6162 6322 2c20 696e 7429 290a 0a20  ("abc", int)).. 
+00010cf0: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
+00010d00: 696e 666f 5f62 6173 6520 3d20 7474 2e69  info_base = tt.i
+00010d10: 6e66 6f28 290a 2020 2020 2020 2020 7665  nfo().        ve
+00010d20: 7269 6679 5f74 696d 6573 7461 6d70 7328  rify_timestamps(
+00010d30: 7469 6d69 6e67 2e73 7461 7274 2c20 7469  timing.start, ti
+00010d40: 6d69 6e67 2e65 6e64 2c20 6578 7065 6374  ming.end, expect
+00010d50: 6564 5f69 6e66 6f5f 6261 7365 290a 0a20  ed_info_base).. 
+00010d60: 2020 2020 2020 2070 7269 6e74 2822 6162         print("ab
+00010d70: 632e 6373 7622 2c20 6578 7065 6374 6564  c.csv", expected
+00010d80: 5f69 6e66 6f5f 6261 7365 290a 0a20 2020  _info_base)..   
+00010d90: 2020 2020 2063 6f6d 7072 6573 7365 645f       compressed_
+00010da0: 6669 6c65 7320 3d20 5b0a 2020 2020 2020  files = [.      
+00010db0: 2020 2020 2020 2261 6263 2e63 7376 2e7a        "abc.csv.z
+00010dc0: 6970 222c 0a20 2020 2020 2020 2020 2020  ip",.           
+00010dd0: 2022 6162 632e 6373 762e 677a 222c 0a20   "abc.csv.gz",. 
+00010de0: 2020 2020 2020 2020 2020 2022 6162 632e             "abc.
+00010df0: 6373 762e 787a 222c 0a20 2020 2020 2020  csv.xz",.       
+00010e00: 205d 0a20 2020 2020 2020 2066 6f72 206e   ].        for n
+00010e10: 616d 6520 696e 2063 6f6d 7072 6573 7365  ame in compresse
+00010e20: 645f 6669 6c65 733a 0a20 2020 2020 2020  d_files:.       
+00010e30: 2020 2020 2069 6d70 6f72 745f 736f 7572       import_sour
+00010e40: 6365 5f6e 616d 6520 3d20 2274 6573 742f  ce_name = "test/
+00010e50: 2220 2b20 6e61 6d65 0a20 2020 2020 2020  " + name.       
+00010e60: 2020 2020 2077 6974 6820 7469 6d65 7374       with timest
+00010e70: 616d 705f 7374 6172 745f 656e 6428 2920  amp_start_end() 
+00010e80: 6173 2074 696d 696e 673a 0a20 2020 2020  as timing:.     
+00010e90: 2020 2020 2020 2020 2020 2074 7432 203d             tt2 =
+00010ea0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00010eb0: 696d 706f 7274 2869 6d70 6f72 745f 736f  import(import_so
+00010ec0: 7572 6365 5f6e 616d 652c 2074 7261 6e73  urce_name, trans
+00010ed0: 666f 726d 733d 6469 6374 2e66 726f 6d6b  forms=dict.fromk
+00010ee0: 6579 7328 2261 6263 222c 2069 6e74 2929  eys("abc", int))
+00010ef0: 0a0a 2020 2020 2020 2020 2020 2020 7474  ..            tt
+00010f00: 325f 696e 666f 203d 2074 7432 2e69 6e66  2_info = tt2.inf
+00010f10: 6f28 290a 2020 2020 2020 2020 2020 2020  o().            
+00010f20: 7072 696e 7428 6e61 6d65 2c20 7474 325f  print(name, tt2_
+00010f30: 696e 666f 290a 0a20 2020 2020 2020 2020  info)..         
+00010f40: 2020 2076 6572 6966 795f 7469 6d65 7374     verify_timest
+00010f50: 616d 7073 2874 696d 696e 672e 7374 6172  amps(timing.star
+00010f60: 742c 2074 696d 696e 672e 656e 642c 2074  t, timing.end, t
+00010f70: 7432 5f69 6e66 6f29 0a0a 2020 2020 2020  t2_info)..      
+00010f80: 2020 2020 2020 6578 7065 6374 6564 5f69        expected_i
+00010f90: 6e66 6f20 3d20 7b2a 2a65 7870 6563 7465  nfo = {**expecte
+00010fa0: 645f 696e 666f 5f62 6173 652c 2022 6e61  d_info_base, "na
+00010fb0: 6d65 223a 2069 6d70 6f72 745f 736f 7572  me": import_sour
+00010fc0: 6365 5f6e 616d 657d 0a20 2020 2020 2020  ce_name}.       
+00010fd0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00010fe0: 7562 5465 7374 286e 616d 653d 6e61 6d65  ubTest(name=name
+00010ff0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011000: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00011010: 7561 6c28 6578 7065 6374 6564 5f69 6e66  ual(expected_inf
+00011020: 6f2c 2074 7432 5f69 6e66 6f29 0a20 2020  o, tt2_info).   
+00011030: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00011040: 6c66 2e73 7562 5465 7374 286e 616d 653d  lf.subTest(name=
+00011050: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+00011060: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011070: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
+00011080: 6c6c 2e61 292c 2073 756d 2874 7432 2e61  ll.a), sum(tt2.a
+00011090: 6c6c 2e61 2929 0a20 2020 2020 2020 2020  ll.a)).         
+000110a0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000110b0: 5465 7374 286e 616d 653d 6e61 6d65 293a  Test(name=name):
+000110c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000110d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000110e0: 6c28 7375 6d28 7474 2e61 6c6c 2e62 292c  l(sum(tt.all.b),
+000110f0: 2073 756d 2874 7432 2e61 6c6c 2e62 2929   sum(tt2.all.b))
+00011100: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00011110: 6820 7365 6c66 2e73 7562 5465 7374 286e  h self.subTest(n
+00011120: 616d 653d 6e61 6d65 293a 0a20 2020 2020  ame=name):.     
+00011130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011140: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00011150: 7474 2e61 6c6c 2e63 292c 2073 756d 2874  tt.all.c), sum(t
+00011160: 7432 2e61 6c6c 2e63 2929 0a0a 2020 2020  t2.all.c))..    
+00011170: 2020 2020 2320 7465 7374 2073 6570 6172      # test separ
+00011180: 6174 656c 792c 206e 6f20 7472 616e 7366  ately, no transf
+00011190: 6f72 6d73 2066 6f72 204a 534f 4e20 696d  orms for JSON im
+000111a0: 706f 7274 730a 2020 2020 2020 2020 696d  ports.        im
+000111b0: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
+000111c0: 203d 2022 7465 7374 2f61 6263 2e6a 736f   = "test/abc.jso
+000111d0: 6e2e 677a 220a 2020 2020 2020 2020 7769  n.gz".        wi
+000111e0: 7468 2074 696d 6573 7461 6d70 5f73 7461  th timestamp_sta
+000111f0: 7274 5f65 6e64 2829 2061 7320 7469 6d69  rt_end() as timi
+00011200: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00011210: 7474 3220 3d20 6c74 2e54 6162 6c65 2829  tt2 = lt.Table()
+00011220: 2e6a 736f 6e5f 696d 706f 7274 2822 7465  .json_import("te
+00011230: 7374 2f61 6263 2e6a 736f 6e2e 677a 222c  st/abc.json.gz",
+00011240: 2073 7472 6561 6d69 6e67 3d54 7275 6529   streaming=True)
+00011250: 0a0a 2020 2020 2020 2020 7474 325f 696e  ..        tt2_in
+00011260: 666f 203d 2074 7432 2e69 6e66 6f28 290a  fo = tt2.info().
+00011270: 2020 2020 2020 2020 7072 696e 7428 2261          print("a
+00011280: 6263 2e6a 736f 6e2e 677a 222c 2074 7432  bc.json.gz", tt2
+00011290: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
+000112a0: 7665 7269 6679 5f74 696d 6573 7461 6d70  verify_timestamp
+000112b0: 7328 7469 6d69 6e67 2e73 7461 7274 2c20  s(timing.start, 
+000112c0: 7469 6d69 6e67 2e65 6e64 2c20 7474 325f  timing.end, tt2_
+000112d0: 696e 666f 290a 0a20 2020 2020 2020 2065  info)..        e
+000112e0: 7870 6563 7465 645f 696e 666f 203d 207b  xpected_info = {
+000112f0: 2a2a 6578 7065 6374 6564 5f69 6e66 6f5f  **expected_info_
+00011300: 6261 7365 2c20 226e 616d 6522 3a20 696d  base, "name": im
+00011310: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
+00011320: 7d0a 2020 2020 2020 2020 7769 7468 2073  }.        with s
+00011330: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00011340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011350: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00011360: 6374 6564 5f69 6e66 6f2c 2074 7432 5f69  cted_info, tt2_i
+00011370: 6e66 6f29 0a20 2020 2020 2020 2077 6974  nfo).        wit
+00011380: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00011390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000113a0: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+000113b0: 756d 2874 742e 616c 6c2e 6129 2c20 7375  um(tt.all.a), su
+000113c0: 6d28 7474 322e 616c 6c2e 6129 290a 2020  m(tt2.all.a)).  
+000113d0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+000113e0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+000113f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011400: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
+00011410: 6c6c 2e62 292c 2073 756d 2874 7432 2e61  ll.b), sum(tt2.a
+00011420: 6c6c 2e62 2929 0a20 2020 2020 2020 2077  ll.b)).        w
+00011430: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00011440: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00011450: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00011460: 2873 756d 2874 742e 616c 6c2e 6329 2c20  (sum(tt.all.c), 
+00011470: 7375 6d28 7474 322e 616c 6c2e 6329 290a  sum(tt2.all.c)).
+00011480: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
+00011490: 765f 696d 706f 7274 5f73 6f75 7263 655f  v_import_source_
+000114a0: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
+000114b0: 2020 2020 696d 706f 7274 7320 3d20 5b0a      imports = [.
+000114c0: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
+000114d0: 632e 6373 7622 2c20 6c74 2e49 6d70 6f72  c.csv", lt.Impor
+000114e0: 7453 6f75 7263 6554 7970 652e 6669 6c65  tSourceType.file
+000114f0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00011500: 2261 6263 2e74 7376 222c 206c 742e 496d  "abc.tsv", lt.Im
+00011510: 706f 7274 536f 7572 6365 5479 7065 2e66  portSourceType.f
+00011520: 696c 6529 2c0a 2020 2020 2020 2020 2020  ile),.          
+00011530: 2020 2822 6162 632e 786c 7378 222c 206c    ("abc.xlsx", l
+00011540: 742e 496d 706f 7274 536f 7572 6365 5479  t.ImportSourceTy
+00011550: 7065 2e66 696c 6529 2c0a 2020 2020 2020  pe.file),.      
+00011560: 2020 2020 2020 2822 6162 632e 6373 762e        ("abc.csv.
+00011570: 7a69 7022 2c20 6c74 2e49 6d70 6f72 7453  zip", lt.ImportS
+00011580: 6f75 7263 6554 7970 652e 7a69 7029 2c0a  ourceType.zip),.
+00011590: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
+000115a0: 632e 6373 762e 677a 222c 206c 742e 496d  c.csv.gz", lt.Im
+000115b0: 706f 7274 536f 7572 6365 5479 7065 2e67  portSourceType.g
+000115c0: 7a69 7029 2c0a 2020 2020 2020 2020 2020  zip),.          
+000115d0: 2020 2822 6162 632e 6373 762e 787a 222c    ("abc.csv.xz",
+000115e0: 206c 742e 496d 706f 7274 536f 7572 6365   lt.ImportSource
+000115f0: 5479 7065 2e6c 7a6d 6129 2c0a 2020 2020  Type.lzma),.    
+00011600: 2020 2020 2020 2020 2822 612c 622c 635c          ("a,b,c\
+00011610: 6e31 2c32 2c33 222c 206c 742e 496d 706f  n1,2,3", lt.Impo
+00011620: 7274 536f 7572 6365 5479 7065 2e73 7472  rtSourceType.str
+00011630: 696e 6729 2c0a 2020 2020 2020 2020 5d0a  ing),.        ].
+00011640: 2020 2020 2020 2020 666f 7220 666e 616d          for fnam
+00011650: 652c 2065 7870 6563 7465 645f 7479 7065  e, expected_type
+00011660: 2069 6e20 696d 706f 7274 733a 0a20 2020   in imports:.   
+00011670: 2020 2020 2020 2020 2069 6620 225c 6e22           if "\n"
+00011680: 206e 6f74 2069 6e20 666e 616d 653a 0a20   not in fname:. 
+00011690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000116a0: 6d70 6f72 745f 6e61 6d65 203d 2022 7465  mport_name = "te
+000116b0: 7374 2f22 202b 2066 6e61 6d65 0a20 2020  st/" + fname.   
+000116c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000116d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000116e0: 6d70 6f72 745f 6e61 6d65 203d 2066 6e61  mport_name = fna
+000116f0: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
+00011700: 6620 696d 706f 7274 5f6e 616d 652e 656e  f import_name.en
+00011710: 6473 7769 7468 2822 2e63 7376 2229 3a0a  dswith(".csv"):.
+00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011730: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
+00011740: 2e63 7376 5f69 6d70 6f72 7428 696d 706f  .csv_import(impo
+00011750: 7274 5f6e 616d 6529 0a20 2020 2020 2020  rt_name).       
+00011760: 2020 2020 2065 6c69 6620 696d 706f 7274       elif import
+00011770: 5f6e 616d 652e 656e 6473 7769 7468 2822  _name.endswith("
+00011780: 2e78 6c73 7822 293a 0a20 2020 2020 2020  .xlsx"):.       
+00011790: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
+000117a0: 742e 5461 626c 6528 292e 6578 6365 6c5f  t.Table().excel_
+000117b0: 696d 706f 7274 2869 6d70 6f72 745f 6e61  import(import_na
+000117c0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+000117d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000117e0: 2020 2020 2020 7462 6c20 3d20 6c74 2e54        tbl = lt.T
+000117f0: 6162 6c65 2829 2e74 7376 5f69 6d70 6f72  able().tsv_impor
+00011800: 7428 696d 706f 7274 5f6e 616d 6529 0a0a  t(import_name)..
+00011810: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011820: 7428 7265 7072 2869 6d70 6f72 745f 6e61  t(repr(import_na
+00011830: 6d65 292c 2074 626c 2e69 6d70 6f72 745f  me), tbl.import_
+00011840: 736f 7572 6365 2c20 7462 6c2e 696d 706f  source, tbl.impo
+00011850: 7274 5f73 6f75 7263 655f 7479 7065 290a  rt_source_type).
+00011860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011870: 225c 6e22 206e 6f74 2069 6e20 666e 616d  "\n" not in fnam
+00011880: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011890: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000118a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000118b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000118c0: 2e61 7373 6572 7445 7175 616c 2869 6d70  .assertEqual(imp
+000118d0: 6f72 745f 6e61 6d65 2c20 7462 6c2e 696d  ort_name, tbl.im
+000118e0: 706f 7274 5f73 6f75 7263 6529 0a20 2020  port_source).   
+000118f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00011900: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00011910: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00011920: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00011930: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00011940: 6572 7445 7175 616c 284e 6f6e 652c 2074  ertEqual(None, t
+00011950: 626c 2e69 6d70 6f72 745f 736f 7572 6365  bl.import_source
+00011960: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00011970: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00011980: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011990: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000119a0: 7561 6c28 6578 7065 6374 6564 5f74 7970  ual(expected_typ
+000119b0: 652c 2074 626c 2e69 6d70 6f72 745f 736f  e, tbl.import_so
+000119c0: 7572 6365 5f74 7970 6529 0a0a 2020 2020  urce_type)..    
+000119d0: 6465 6620 7465 7374 5f63 7376 5f69 6d70  def test_csv_imp
+000119e0: 6f72 745f 6672 6f6d 5f75 726c 2873 656c  ort_from_url(sel
+000119f0: 6629 3a0a 2020 2020 2020 2020 6672 6f6d  f):.        from
+00011a00: 2068 7474 702e 7365 7276 6572 2069 6d70   http.server imp
+00011a10: 6f72 7420 4854 5450 5365 7276 6572 2c20  ort HTTPServer, 
+00011a20: 4261 7365 4854 5450 5265 7175 6573 7448  BaseHTTPRequestH
+00011a30: 616e 646c 6572 0a20 2020 2020 2020 2066  andler.        f
+00011a40: 726f 6d20 6874 7470 2069 6d70 6f72 7420  rom http import 
+00011a50: 4854 5450 5374 6174 7573 0a20 2020 2020  HTTPStatus.     
+00011a60: 2020 2069 6d70 6f72 7420 7468 7265 6164     import thread
+00011a70: 696e 670a 2020 2020 2020 2020 696d 706f  ing.        impo
+00011a80: 7274 2074 696d 650a 2020 2020 2020 2020  rt time.        
+00011a90: 696d 706f 7274 2075 726c 6c69 622e 6572  import urllib.er
+00011aa0: 726f 720a 2020 2020 2020 2020 696d 706f  ror.        impo
+00011ab0: 7274 2075 726c 6c69 622e 7265 7175 6573  rt urllib.reques
+00011ac0: 740a 0a20 2020 2020 2020 2069 6620 534b  t..        if SK
+00011ad0: 4950 5f43 5356 5f49 4d50 4f52 545f 5553  IP_CSV_IMPORT_US
+00011ae0: 494e 475f 5552 4c5f 5445 5354 533a 0a20  ING_URL_TESTS:. 
+00011af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011b00: 736b 6970 5465 7374 2822 4353 5620 696d  skipTest("CSV im
+00011b10: 706f 7274 2074 6573 7473 2073 6b69 7070  port tests skipp
+00011b20: 6564 2229 0a0a 2020 2020 2020 2020 636c  ed")..        cl
+00011b30: 6173 7320 4353 5654 6573 7452 6571 7565  ass CSVTestReque
+00011b40: 7374 4861 6e64 6c65 7228 4261 7365 4854  stHandler(BaseHT
+00011b50: 5450 5265 7175 6573 7448 616e 646c 6572  TPRequestHandler
+00011b60: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00011b70: 6566 2064 6f5f 4745 5428 7365 6c66 293a  ef do_GET(self):
+00011b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b90: 2073 656c 662e 6c6f 675f 6d65 7373 6167   self.log_messag
+00011ba0: 6528 2272 6563 6569 7665 6420 2573 2025  e("received %s %
+00011bb0: 7322 2c20 7365 6c66 2e63 6f6d 6d61 6e64  s", self.command
+00011bc0: 2c20 7365 6c66 2e70 6174 6829 0a20 2020  , self.path).   
+00011bd0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+00011be0: 6820 3d20 7365 6c66 2e70 6174 680a 2020  h = self.path.  
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011c00: 2070 6174 6820 3d3d 2022 2f45 5849 5422   path == "/EXIT"
+00011c10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011c20: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
+00011c30: 7265 7370 6f6e 7365 2848 5454 5053 7461  response(HTTPSta
+00011c40: 7475 732e 4f4b 290a 2020 2020 2020 2020  tus.OK).        
+00011c50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011c60: 2e65 6e64 5f68 6561 6465 7273 2829 0a20  .end_headers(). 
+00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c80: 2020 2074 6872 6561 6469 6e67 2e54 6872     threading.Thr
+00011c90: 6561 6428 7461 7267 6574 3d6c 616d 6264  ead(target=lambd
+00011ca0: 613a 2073 656c 662e 7365 7276 6572 2e73  a: self.server.s
+00011cb0: 6875 7464 6f77 6e28 2929 2e73 7461 7274  hutdown()).start
+00011cc0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00011cd0: 2020 2020 656c 6966 2070 6174 6820 3d3d      elif path ==
+00011ce0: 2022 2f22 3a0a 2020 2020 2020 2020 2020   "/":.          
+00011cf0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00011d00: 656e 645f 7265 7370 6f6e 7365 2848 5454  end_response(HTT
+00011d10: 5053 7461 7475 732e 4f4b 290a 2020 2020  PStatus.OK).    
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 7365 6c66 2e65 6e64 5f68 6561 6465 7273  self.end_headers
+00011d40: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00011d50: 2020 2020 656c 6966 2070 6174 682e 7374      elif path.st
+00011d60: 6172 7473 7769 7468 2822 2f61 6263 2e63  artswith("/abc.c
+00011d70: 7376 2229 3a0a 2020 2020 2020 2020 2020  sv"):.          
+00011d80: 2020 2020 2020 2020 2020 7365 6e64 5f62            send_b
+00011d90: 7974 6573 203d 2062 2261 2c62 2c63 5c6e  ytes = b"a,b,c\n
+00011da0: 312c 322c 335c 6e22 0a20 2020 2020 2020  1,2,3\n".       
+00011db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011dc0: 662e 7365 6e64 5f72 6573 706f 6e73 6528  f.send_response(
+00011dd0: 4854 5450 5374 6174 7573 2e4f 4b29 0a20  HTTPStatus.OK). 
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011df0: 2020 2073 656c 662e 656e 645f 6865 6164     self.end_head
+00011e00: 6572 7328 290a 2020 2020 2020 2020 2020  ers().          
+00011e10: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+00011e20: 6669 6c65 2e77 7269 7465 2873 656e 645f  file.write(send_
+00011e30: 6279 7465 7329 0a0a 2020 2020 2020 2020  bytes)..        
+00011e40: 6465 6620 7275 6e28 7365 7276 6572 5f63  def run(server_c
+00011e50: 6c61 7373 3d48 5454 5053 6572 7665 722c  lass=HTTPServer,
+00011e60: 2068 616e 646c 6572 5f63 6c61 7373 3d43   handler_class=C
+00011e70: 5356 5465 7374 5265 7175 6573 7448 616e  SVTestRequestHan
+00011e80: 646c 6572 293a 0a20 2020 2020 2020 2020  dler):.         
+00011e90: 2020 2073 6572 7665 725f 6164 6472 6573     server_addres
+00011ea0: 7320 3d20 2827 272c 2038 3838 3829 0a20  s = ('', 8888). 
+00011eb0: 2020 2020 2020 2020 2020 2068 7474 7064             httpd
+00011ec0: 203d 2073 6572 7665 725f 636c 6173 7328   = server_class(
+00011ed0: 7365 7276 6572 5f61 6464 7265 7373 2c20  server_address, 
+00011ee0: 6861 6e64 6c65 725f 636c 6173 7329 0a20  handler_class). 
+00011ef0: 2020 2020 2020 2020 2020 2068 7474 7064             httpd
+00011f00: 2e73 6572 7665 5f66 6f72 6576 6572 2829  .serve_forever()
+00011f10: 0a0a 2020 2020 2020 2020 6465 6620 7275  ..        def ru
+00011f20: 6e5f 6261 636b 6772 6f75 6e64 5f74 6573  n_background_tes
+00011f30: 745f 7365 7276 6572 2829 3a0a 2020 2020  t_server():.    
+00011f40: 2020 2020 2020 2020 7020 3d20 7468 7265          p = thre
+00011f50: 6164 696e 672e 5468 7265 6164 2874 6172  ading.Thread(tar
+00011f60: 6765 743d 7275 6e29 0a20 2020 2020 2020  get=run).       
+00011f70: 2020 2020 2070 2e73 7461 7274 2829 0a0a       p.start()..
+00011f80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011f90: 7472 6965 735f 7265 6d61 696e 696e 6720  tries_remaining 
+00011fa0: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
+00011fb0: 6528 3230 2929 3a0a 2020 2020 2020 2020  e(20)):.        
+00011fc0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fe0: 2077 6974 6820 7572 6c6c 6962 2e72 6571   with urllib.req
+00011ff0: 7565 7374 2e75 726c 6f70 656e 2822 6874  uest.urlopen("ht
+00012000: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a38  tp://localhost:8
+00012010: 3838 382f 2229 3a0a 2020 2020 2020 2020  888/"):.        
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00012040: 2020 2020 2020 6578 6365 7074 2075 726c        except url
+00012050: 6c69 622e 6572 726f 722e 5552 4c45 7272  lib.error.URLErr
+00012060: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00012070: 2020 2020 2020 2020 6966 2074 7269 6573          if tries
+00012080: 5f72 656d 6169 6e69 6e67 3a0a 2020 2020  _remaining:.    
+00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120a0: 2020 2020 7469 6d65 2e73 6c65 6570 2830      time.sleep(0
+000120b0: 2e32 3529 0a0a 2020 2020 2020 2020 2020  .25)..          
+000120c0: 2020 7265 7475 726e 2070 0a0a 2020 2020    return p..    
+000120d0: 2020 2020 7765 625f 6164 6472 6573 7320      web_address 
+000120e0: 3d20 2268 7474 703a 2f2f 6c6f 6361 6c68  = "http://localh
+000120f0: 6f73 743a 3838 3838 220a 2020 2020 2020  ost:8888".      
+00012100: 2020 7020 3d20 7275 6e5f 6261 636b 6772    p = run_backgr
+00012110: 6f75 6e64 5f74 6573 745f 7365 7276 6572  ound_test_server
+00012120: 2829 0a0a 2020 2020 2020 2020 7572 6c20  ()..        url 
+00012130: 3d20 7765 625f 6164 6472 6573 7320 2b20  = web_address + 
+00012140: 222f 6162 632e 6373 7622 0a20 2020 2020  "/abc.csv".     
+00012150: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00012160: 2020 2020 7462 6c20 3d20 6c74 2e54 6162      tbl = lt.Tab
+00012170: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+00012180: 7572 6c29 0a20 2020 2020 2020 2066 696e  url).        fin
+00012190: 616c 6c79 3a0a 2020 2020 2020 2020 2020  ally:.          
+000121a0: 2020 7769 7468 2075 726c 6c69 622e 7265    with urllib.re
+000121b0: 7175 6573 742e 7572 6c6f 7065 6e28 7765  quest.urlopen(we
+000121c0: 625f 6164 6472 6573 7320 2b20 222f 4558  b_address + "/EX
+000121d0: 4954 2229 3a0a 2020 2020 2020 2020 2020  IT"):.          
+000121e0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+000121f0: 2020 2020 2020 2070 2e6a 6f69 6e28 290a         p.join().
+00012200: 0a20 2020 2020 2020 2074 626c 2e70 7265  .        tbl.pre
+00012210: 7365 6e74 2829 0a20 2020 2020 2020 2077  sent().        w
+00012220: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00012230: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012240: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00012250: 2875 726c 2c20 7462 6c2e 696d 706f 7274  (url, tbl.import
+00012260: 5f73 6f75 7263 6529 0a20 2020 2020 2020  _source).       
+00012270: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00012280: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00012290: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000122a0: 616c 286c 742e 496d 706f 7274 536f 7572  al(lt.ImportSour
+000122b0: 6365 5479 7065 2e75 726c 2c20 7462 6c2e  ceType.url, tbl.
+000122c0: 696d 706f 7274 5f73 6f75 7263 655f 7479  import_source_ty
+000122d0: 7065 290a 0a20 2020 2064 6566 2074 6573  pe)..    def tes
+000122e0: 745f 6373 765f 6669 6c74 6572 6564 5f69  t_csv_filtered_i
+000122f0: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
+00012300: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+00012310: 2033 0a20 2020 2020 2020 2074 7420 3d20   3.        tt = 
+00012320: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00012330: 6d70 6f72 7428 2274 6573 742f 6162 632e  mport("test/abc.
+00012340: 6373 7622 2c20 7472 616e 7366 6f72 6d73  csv", transforms
+00012350: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00012360: 6162 6322 2c20 696e 7429 290a 2020 2020  abc", int)).    
+00012370: 2020 2020 7072 696e 7428 2261 6263 2e63      print("abc.c
+00012380: 7376 222c 2074 742e 696e 666f 2829 290a  sv", tt.info()).
+00012390: 0a20 2020 2020 2020 2074 7420 3d20 6c74  .        tt = lt
+000123a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+000123b0: 6f72 7428 2274 6573 742f 6162 632e 6373  ort("test/abc.cs
+000123c0: 7622 2c20 7472 616e 7366 6f72 6d73 3d64  v", transforms=d
+000123d0: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
+000123e0: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012400: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00012410: 7465 7273 3d7b 2263 223a 206c 742e 5461  ters={"c": lt.Ta
+00012420: 626c 652e 6571 2831 297d 290a 2020 2020  ble.eq(1)}).    
+00012430: 2020 2020 7072 696e 7428 7474 2e69 6e66      print(tt.inf
+00012440: 6f28 2929 0a20 2020 2020 2020 2077 6974  o()).        wit
+00012450: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00012460: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012470: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00012480: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
+00012490: 7369 7a65 2c20 6c65 6e28 7474 2929 0a0a  size, len(tt))..
+000124a0: 2020 2020 2020 2020 7474 203d 206c 742e          tt = lt.
+000124b0: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+000124c0: 7274 2822 7465 7374 2f61 6263 2e63 7376  rt("test/abc.csv
+000124d0: 222c 2074 7261 6e73 666f 726d 733d 6469  ", transforms=di
+000124e0: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+000124f0: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012510: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00012520: 6572 733d 7b22 6322 3a20 317d 290a 2020  ers={"c": 1}).  
+00012530: 2020 2020 2020 7072 696e 7428 7474 2e69        print(tt.i
+00012540: 6e66 6f28 2929 0a20 2020 2020 2020 2077  nfo()).        w
+00012550: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00012560: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012570: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00012580: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+00012590: 745f 7369 7a65 2c20 6c65 6e28 7474 2929  t_size, len(tt))
+000125a0: 0a0a 2020 2020 2020 2020 7474 203d 206c  ..        tt = l
+000125b0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+000125c0: 706f 7274 2822 7465 7374 2f61 6263 2e63  port("test/abc.c
+000125d0: 7376 222c 2074 7261 6e73 666f 726d 733d  sv", transforms=
+000125e0: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+000125f0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012610: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00012620: 6c74 6572 733d 7b22 6322 3a20 6c61 6d62  lters={"c": lamb
+00012630: 6461 2078 3a20 3020 3c20 7820 3c20 327d  da x: 0 < x < 2}
+00012640: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00012650: 7474 2e69 6e66 6f28 2929 0a20 2020 2020  tt.info()).     
+00012660: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00012670: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00012680: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00012690: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
+000126a0: 2074 6573 745f 7369 7a65 2c20 6c65 6e28   test_size, len(
+000126b0: 7474 2929 0a0a 2020 2020 2020 2020 2320  tt))..        # 
+000126c0: 7465 7374 2061 6c6c 2073 7065 6369 616c  test all special
+000126d0: 2063 6f6d 7061 7261 746f 7273 2077 6865   comparators whe
+000126e0: 6e20 7573 6564 2061 7320 6669 6c74 6572  n used as filter
+000126f0: 730a 2020 2020 2020 2020 2320 2020 2020  s.        #     
+00012700: 6973 5f6e 6f6e 6520 2d20 6174 7472 6962  is_none - attrib
+00012710: 7574 6520 7661 6c75 6520 6973 204e 6f6e  ute value is Non
+00012720: 650a 2020 2020 2020 2020 2320 2020 2020  e.        #     
+00012730: 6973 5f6e 6f74 5f6e 6f6e 6520 2d20 6174  is_not_none - at
+00012740: 7472 6962 7574 6520 7661 6c75 6520 6973  tribute value is
+00012750: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00012760: 2020 2320 2020 2020 6973 5f6e 756c 6c20    #     is_null 
+00012770: 2d20 6174 7472 6962 7574 6520 7661 6c75  - attribute valu
+00012780: 6520 6973 204e 6f6e 652c 2022 222c 206f  e is None, "", o
+00012790: 7220 6e6f 7420 6465 6669 6e65 640a 2020  r not defined.  
+000127a0: 2020 2020 2020 2320 2020 2020 6973 5f6e        #     is_n
+000127b0: 6f74 5f6e 756c 6c20 2d20 6174 7472 6962  ot_null - attrib
+000127c0: 7574 6520 7661 6c75 6520 6973 2064 6566  ute value is def
+000127d0: 696e 6564 2c20 616e 6420 6973 206e 6f74  ined, and is not
+000127e0: 204e 6f6e 6520 6f72 2022 220a 2020 2020   None or "".    
+000127f0: 2020 2020 2320 2020 2020 7374 6172 7473      #     starts
+00012800: 7769 7468 202d 2061 7474 7269 6275 7465  with - attribute
+00012810: 2076 616c 7565 2073 7461 7274 7320 7769   value starts wi
+00012820: 7468 2061 2067 6976 656e 2073 7472 696e  th a given strin
+00012830: 670a 2020 2020 2020 2020 2320 2020 2020  g.        #     
+00012840: 656e 6473 7769 7468 202d 2061 7474 7269  endswith - attri
+00012850: 6275 7465 2076 616c 7565 2065 6e64 7320  bute value ends 
+00012860: 7769 7468 2061 2067 6976 656e 2073 7472  with a given str
+00012870: 696e 670a 2020 2020 2020 2020 2320 2020  ing.        #   
+00012880: 2020 7265 5f6d 6174 6368 202d 2061 7474    re_match - att
+00012890: 7269 6275 7465 2076 616c 7565 206d 6174  ribute value mat
+000128a0: 6368 6573 2061 2072 6567 756c 6172 2065  ches a regular e
+000128b0: 7870 7265 7373 696f 6e0a 0a20 2020 2020  xpression..     
+000128c0: 2020 2070 7269 6e74 2829 0a20 2020 2020     print().     
+000128d0: 2020 2069 6e70 7574 5f64 6174 6120 3d20     input_data = 
+000128e0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+000128f0: 2222 225c 0a20 2020 2020 2020 206e 616d  """\.        nam
+00012900: 652c 612c 622c 630a 2020 2020 2020 2020  e,a,b,c.        
+00012910: 2241 222c 3130 302c 3130 302c 3130 300a  "A",100,100,100.
+00012920: 2020 2020 2020 2020 2242 222c 3230 302c          "B",200,
+00012930: 2c32 3030 0a20 2020 2020 2020 2022 4131  ,200.        "A1
+00012940: 222c 3130 312c 3130 312c 3130 310a 2020  ",101,101,101.  
+00012950: 2020 2020 2020 2242 3122 2c32 3031 2c2c        "B1",201,,
+00012960: 3230 310a 2020 2020 2020 2020 2243 3122  201.        "C1"
+00012970: 2c33 3031 2c2c 3330 310a 2020 2020 2020  ,301,,301.      
+00012980: 2020 2c39 392c 3939 2c39 390a 2020 2020    ,99,99,99.    
+00012990: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
+000129a0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+000129b0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+000129c0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129e0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+000129f0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+00012a00: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
+00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a20: 2020 2020 2029 2e70 7265 7365 6e74 2829       ).present()
+00012a30: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00012a40: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+00012a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012a60: 2b0a 2020 2020 2020 2020 7c20 4e61 6d65  +.        | Name
+00012a70: 207c 2020 2041 207c 2020 2020 4220 7c20   |   A |    B | 
+00012a80: 2020 4320 7c0a 2020 2020 2020 2020 7c2d    C |.        |-
+00012a90: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d 2d2d  -----+-----+----
+00012aa0: 2d2d 2b2d 2d2d 2d2d 7c0a 2020 2020 2020  --+-----|.      
+00012ab0: 2020 7c20 4120 2020 207c 2031 3030 207c    | A    | 100 |
+00012ac0: 2020 3130 3020 7c20 3130 3020 7c0a 2020    100 | 100 |.  
+00012ad0: 2020 2020 2020 7c20 4220 2020 207c 2032        | B    | 2
+00012ae0: 3030 207c 204e 6f6e 6520 7c20 3230 3020  00 | None | 200 
+00012af0: 7c0a 2020 2020 2020 2020 7c20 4131 2020  |.        | A1  
+00012b00: 207c 2031 3031 207c 2020 3130 3120 7c20   | 101 |  101 | 
+00012b10: 3130 3120 7c0a 2020 2020 2020 2020 7c20  101 |.        | 
+00012b20: 4231 2020 207c 2032 3031 207c 204e 6f6e  B1   | 201 | Non
+00012b30: 6520 7c20 3230 3120 7c0a 2020 2020 2020  e | 201 |.      
+00012b40: 2020 7c20 4331 2020 207c 2033 3031 207c    | C1   | 301 |
+00012b50: 204e 6f6e 6520 7c20 3330 3120 7c0a 2020   None | 301 |.  
+00012b60: 2020 2020 2020 7c20 2020 2020 207c 2020        |      |  
+00012b70: 3939 207c 2020 2039 3920 7c20 2039 3920  99 |   99 |  99 
+00012b80: 7c0a 2020 2020 2020 2020 2b2d 2d2d 2d2d  |.        +-----
+00012b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012ba0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+00012bb0: 220a 0a20 2020 2020 2020 2070 7269 6e74  "..        print
+00012bc0: 2822 6973 5f6e 6f6e 6528 2922 290a 2020  ("is_none()").  
+00012bd0: 2020 2020 2020 7820 3d20 6c74 2e54 6162        x = lt.Tab
+00012be0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+00012bf0: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00012c30: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00012c40: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c70: 2020 2020 6669 6c74 6572 733d 7b22 6222      filters={"b"
+00012c80: 3a20 6c74 2e54 6162 6c65 2e69 735f 6e6f  : lt.Table.is_no
+00012c90: 6e65 2829 7d29 0a20 2020 2020 2020 2077  ne()}).        w
+00012ca0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00012cb0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012cc0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00012cd0: 2833 2c20 6c65 6e28 7829 290a 2020 2020  (3, len(x)).    
+00012ce0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00012cf0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00012d00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00012d10: 5472 7565 2861 6c6c 2862 2069 7320 4e6f  True(all(b is No
+00012d20: 6e65 2066 6f72 2062 2069 6e20 782e 616c  ne for b in x.al
+00012d30: 6c2e 6229 290a 0a20 2020 2020 2020 2070  l.b))..        p
+00012d40: 7269 6e74 2822 6973 5f6e 6f74 5f6e 6f6e  rint("is_not_non
+00012d50: 6528 2922 290a 2020 2020 2020 2020 7820  e()").        x 
+00012d60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00012d70: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
+00012d80: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+00012db0: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00012dc0: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012de0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00012df0: 6c74 6572 733d 7b22 6222 3a20 6c74 2e54  lters={"b": lt.T
+00012e00: 6162 6c65 2e69 735f 6e6f 745f 6e6f 6e65  able.is_not_none
+00012e10: 2829 7d29 0a20 2020 2020 2020 2077 6974  ()}).        wit
+00012e20: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00012e30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012e40: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00012e50: 2c20 6c65 6e28 7829 290a 2020 2020 2020  , len(x)).      
+00012e60: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00012e70: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00012e80: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00012e90: 7561 6c28 3330 302c 2073 756d 2878 2e61  ual(300, sum(x.a
+00012ea0: 6c6c 2e62 2929 0a0a 2020 2020 2020 2020  ll.b))..        
+00012eb0: 7072 696e 7428 2262 2069 735f 6e75 6c6c  print("b is_null
+00012ec0: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
+00012ed0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00012ee0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+00012ef0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f10: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00012f20: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00012f30: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00012f60: 7465 7273 3d7b 2262 223a 206c 742e 5461  ters={"b": lt.Ta
+00012f70: 626c 652e 6973 5f6e 756c 6c28 297d 290a  ble.is_null()}).
+00012f80: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00012f90: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00012fa0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012fb0: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
+00012fc0: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
+00012fd0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00012fe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012ff0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+00013000: 6c28 6220 6973 204e 6f6e 6520 666f 7220  l(b is None for 
+00013010: 6220 696e 2078 2e61 6c6c 2e62 2929 0a0a  b in x.all.b))..
+00013020: 2020 2020 2020 2020 7072 696e 7428 2262          print("b
+00013030: 2069 735f 6e6f 745f 6e75 6c6c 2829 2229   is_not_null()")
+00013040: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
+00013050: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00013060: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013090: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+000130a0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+000130b0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
+000130e0: 3d7b 2262 223a 206c 742e 5461 626c 652e  ={"b": lt.Table.
+000130f0: 6973 5f6e 6f74 5f6e 756c 6c28 297d 290a  is_not_null()}).
+00013100: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00013110: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00013120: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013130: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
+00013140: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
+00013150: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00013160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013170: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00013180: 3030 2c20 7375 6d28 782e 616c 6c2e 6229  00, sum(x.all.b)
+00013190: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+000131a0: 2822 6e61 6d65 2069 735f 6e75 6c6c 2829  ("name is_null()
+000131b0: 2229 0a20 2020 2020 2020 2078 203d 206c  ").        x = l
+000131c0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+000131d0: 706f 7274 2869 6e70 7574 5f64 6174 612c  port(input_data,
+000131e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
+00013210: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+00013220: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013240: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00013250: 7273 3d7b 226e 616d 6522 3a20 6c74 2e54  rs={"name": lt.T
+00013260: 6162 6c65 2e69 735f 6e75 6c6c 2829 7d29  able.is_null()})
+00013270: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00013280: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00013290: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000132a0: 7373 6572 7445 7175 616c 2831 2c20 6c65  ssertEqual(1, le
+000132b0: 6e28 7829 290a 2020 2020 2020 2020 7769  n(x)).        wi
+000132c0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+000132d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000132e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000132f0: 332a 3939 2c20 785b 305d 2e61 202b 2078  3*99, x[0].a + x
+00013300: 5b30 5d2e 6220 2b20 785b 305d 2e63 290a  [0].b + x[0].c).
+00013310: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00013320: 6e61 6d65 2069 735f 6e6f 745f 6e75 6c6c  name is_not_null
+00013330: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
+00013340: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00013350: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+00013360: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013380: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00013390: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+000133a0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133c0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000133d0: 7465 7273 3d7b 226e 616d 6522 3a20 6c74  ters={"name": lt
+000133e0: 2e54 6162 6c65 2e69 735f 6e6f 745f 6e75  .Table.is_not_nu
+000133f0: 6c6c 2829 7d29 0a20 2020 2020 2020 2077  ll()}).        w
+00013400: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00013410: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00013420: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013430: 2835 2c20 6c65 6e28 7829 290a 2020 2020  (5, len(x)).    
+00013440: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00013450: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00013460: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00013470: 4571 7561 6c28 2241 2042 2041 3120 4231  Equal("A B A1 B1
+00013480: 2043 3122 2e73 706c 6974 2829 2c20 6c69   C1".split(), li
+00013490: 7374 2878 2e61 6c6c 2e6e 616d 6529 290a  st(x.all.name)).
+000134a0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+000134b0: 6e61 6d65 2073 7461 7274 7377 6974 6828  name startswith(
+000134c0: 2742 2729 2229 0a20 2020 2020 2020 2078  'B')").        x
+000134d0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+000134e0: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
+000134f0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00013520: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00013530: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013550: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013560: 696c 7465 7273 3d7b 226e 616d 6522 3a20  ilters={"name": 
+00013570: 6c74 2e54 6162 6c65 2e73 7461 7274 7377  lt.Table.startsw
+00013580: 6974 6828 2242 2229 7d29 0a20 2020 2020  ith("B")}).     
+00013590: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000135a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000135b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000135c0: 7175 616c 2832 2c20 6c65 6e28 7829 290a  qual(2, len(x)).
+000135d0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000135e0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000135f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013600: 7365 7274 4571 7561 6c28 2242 2042 3122  sertEqual("B B1"
+00013610: 2e73 706c 6974 2829 2c20 6c69 7374 2878  .split(), list(x
+00013620: 2e61 6c6c 2e6e 616d 6529 290a 0a20 2020  .all.name))..   
+00013630: 2020 2020 2070 7269 6e74 2822 6e61 6d65       print("name
+00013640: 2065 6e64 7377 6974 6828 2731 2729 2229   endswith('1')")
+00013650: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
+00013660: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00013670: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
+00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136a0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+000136b0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+000136c0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
+000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136e0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
+000136f0: 3d7b 226e 616d 6522 3a20 6c74 2e54 6162  ={"name": lt.Tab
+00013700: 6c65 2e65 6e64 7377 6974 6828 2231 2229  le.endswith("1")
+00013710: 7d29 0a20 2020 2020 2020 2077 6974 6820  }).        with 
+00013720: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00013730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013740: 2e61 7373 6572 7445 7175 616c 2833 2c20  .assertEqual(3, 
+00013750: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
+00013760: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00013770: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00013780: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00013790: 6c28 2241 3120 4231 2043 3122 2e73 706c  l("A1 B1 C1".spl
+000137a0: 6974 2829 2c20 6c69 7374 2878 2e61 6c6c  it(), list(x.all
+000137b0: 2e6e 616d 6529 290a 0a20 2020 2020 2020  .name))..       
+000137c0: 2070 7269 6e74 2872 226e 616d 6520 7265   print(r"name re
+000137d0: 5f6d 6174 6368 2872 275b 4142 5d5c 6427  _match(r'[AB]\d'
+000137e0: 2922 290a 2020 2020 2020 2020 7820 3d20  )").        x = 
+000137f0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00013800: 6d70 6f72 7428 696e 7075 745f 6461 7461  mport(input_data
+00013810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013830: 2020 2020 7472 616e 7366 6f72 6d73 3d64      transforms=d
+00013840: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
+00013850: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
+00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013870: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00013880: 6572 733d 7b22 6e61 6d65 223a 206c 742e  ers={"name": lt.
+00013890: 5461 626c 652e 7265 5f6d 6174 6368 2872  Table.re_match(r
+000138a0: 225b 4142 5d5c 6422 297d 290a 2020 2020  "[AB]\d")}).    
+000138b0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+000138c0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+000138d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000138e0: 4571 7561 6c28 322c 206c 656e 2878 2929  Equal(2, len(x))
+000138f0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00013900: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00013910: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00013920: 7373 6572 7445 7175 616c 2822 4131 2042  ssertEqual("A1 B
+00013930: 3122 2e73 706c 6974 2829 2c20 6c69 7374  1".split(), list
+00013940: 2878 2e61 6c6c 2e6e 616d 6529 290a 0a20  (x.all.name)).. 
+00013950: 2020 2064 6566 2074 6573 745f 6373 765f     def test_csv_
+00013960: 7374 7269 6e67 5f69 6d70 6f72 7428 7365  string_import(se
+00013970: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
+00013980: 6120 3d20 6373 765f 6461 7461 0a20 2020  a = csv_data.   
+00013990: 2020 2020 2063 7376 7461 626c 6520 3d20       csvtable = 
+000139a0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+000139b0: 6d70 6f72 7428 6373 765f 736f 7572 6365  mport(csv_source
+000139c0: 3d64 6174 612c 2074 7261 6e73 666f 726d  =data, transform
+000139d0: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
+000139e0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
+000139f0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
+00013a00: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
+00013a10: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
+00013a20: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
+00013a30: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
+00013a40: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+00013a50: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00013a60: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00013a70: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00013a80: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
+00013a90: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
+00013aa0: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
+00013ab0: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
+00013ac0: 7028 7431 2c20 6373 7674 6162 6c65 2929  p(t1, csvtable))
+00013ad0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00013ae0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00013af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013b00: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00013b10: 3120 666f 7220 6c69 6e65 2069 6e20 6461  1 for line in da
+00013b20: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
+00013b30: 6966 206c 696e 652e 7374 7269 7028 2929  if line.strip())
+00013b40: 2d31 2c20 6c65 6e28 6373 7674 6162 6c65  -1, len(csvtable
+00013b50: 2929 0a0a 2020 2020 2020 2020 726f 775f  ))..        row_
+00013b60: 7072 6f74 6f74 7970 6520 3d20 7365 6c66  prototype = self
+00013b70: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00013b80: 7428 302c 2030 2c20 3029 0a20 2020 2020  t(0, 0, 0).     
+00013b90: 2020 2063 7376 7461 626c 6532 203d 206c     csvtable2 = l
+00013ba0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00013bb0: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
+00013bc0: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+00013bd0: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+00013be0: 696e 747d 2c0a 2020 2020 2020 2020 2020  int},.          
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c10: 726f 775f 636c 6173 733d 7479 7065 2872  row_class=type(r
+00013c20: 6f77 5f70 726f 746f 7479 7065 2929 5b3a  ow_prototype))[:
+00013c30: 335d 0a0a 2020 2020 2020 2020 7072 696e  3]..        prin
+00013c40: 7428 7479 7065 2874 315b 305d 292e 5f5f  t(type(t1[0]).__
+00013c50: 6e61 6d65 5f5f 2c20 7431 5b30 5d29 0a20  name__, t1[0]). 
+00013c60: 2020 2020 2020 2070 7269 6e74 2874 7970         print(typ
+00013c70: 6528 6373 7674 6162 6c65 325b 305d 292e  e(csvtable2[0]).
+00013c80: 5f5f 6e61 6d65 5f5f 2c20 6373 7674 6162  __name__, csvtab
+00013c90: 6c65 325b 305d 290a 2020 2020 2020 2020  le2[0]).        
+00013ca0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00013cb0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00013cc0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00013cd0: 6c28 7479 7065 2874 315b 305d 292c 2074  l(type(t1[0]), t
+00013ce0: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+00013cf0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00013d00: 5f63 7376 5f6c 696d 6974 5f69 6d70 6f72  _csv_limit_impor
+00013d10: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00013d20: 2064 6174 6120 3d20 6373 765f 6461 7461   data = csv_data
+00013d30: 0a20 2020 2020 2020 2069 6d70 6f72 745f  .        import_
+00013d40: 6c69 6d69 7420 3d20 3130 0a20 2020 2020  limit = 10.     
+00013d50: 2020 2063 7376 7461 626c 6520 3d20 6c74     csvtable = lt
+00013d60: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+00013d70: 6f72 7428 6373 765f 736f 7572 6365 3d64  ort(csv_source=d
+00013d80: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
+00013d90: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
+00013da0: 696e 742c 2027 6327 3a20 696e 747d 2c0a  int, 'c': int},.
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dd0: 2020 2020 2020 2020 206c 696d 6974 3d69           limit=i
+00013de0: 6d70 6f72 745f 6c69 6d69 7429 0a0a 2020  mport_limit)..  
+00013df0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00013e00: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00013e10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00013e20: 7274 4571 7561 6c28 696d 706f 7274 5f6c  rtEqual(import_l
+00013e30: 696d 6974 2c20 6c65 6e28 6373 7674 6162  imit, len(csvtab
+00013e40: 6c65 2929 0a0a 2020 2020 2020 2020 6373  le))..        cs
+00013e50: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
+00013e60: 6528 292e 6373 765f 696d 706f 7274 2863  e().csv_import(c
+00013e70: 7376 5f73 6f75 7263 653d 6461 7461 2c20  sv_source=data, 
+00013e80: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
+00013e90: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
+00013ea0: 2763 273a 2069 6e74 7d2c 0a20 2020 2020  'c': int},.     
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ed0: 2020 2020 6c69 6d69 743d 3029 0a0a 2020      limit=0)..  
+00013ee0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00013ef0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00013f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00013f10: 7274 4571 7561 6c28 302c 206c 656e 2863  rtEqual(0, len(c
+00013f20: 7376 7461 626c 6529 290a 0a20 2020 2064  svtable))..    d
+00013f30: 6566 2074 6573 745f 6373 765f 7374 7269  ef test_csv_stri
+00013f40: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
+00013f50: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
+00013f60: 7461 203d 2063 7376 5f64 6174 610a 2020  ta = csv_data.  
+00013f70: 2020 2020 2020 6373 7674 6162 6c65 203d        csvtable =
+00013f80: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00013f90: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
+00013fa0: 653d 6461 7461 2e73 706c 6974 6c69 6e65  e=data.splitline
+00013fb0: 7328 292c 2074 7261 6e73 666f 726d 733d  s(), transforms=
+00013fc0: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
+00013fd0: 696e 742c 2027 6327 3a20 696e 747d 290a  int, 'c': int}).
+00013fe0: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00013ff0: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
+00014000: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
+00014010: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+00014020: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+00014030: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
+00014040: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014050: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014060: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00014070: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+00014080: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+00014090: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+000140a0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+000140b0: 7431 2c20 6373 7674 6162 6c65 2929 290a  t1, csvtable))).
+000140c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000140d0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000140e0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000140f0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
+00014100: 666f 7220 6c69 6e65 2069 6e20 6461 7461  for line in data
+00014110: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
+00014120: 206c 696e 652e 7374 7269 7028 2929 2d31   line.strip())-1
+00014130: 2c20 6c65 6e28 6373 7674 6162 6c65 2929  , len(csvtable))
+00014140: 0a0a 2020 2020 2020 2020 726f 775f 7072  ..        row_pr
+00014150: 6f74 6f74 7970 6520 3d20 7365 6c66 2e6d  ototype = self.m
+00014160: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00014170: 302c 2030 2c20 3029 0a20 2020 2020 2020  0, 0, 0).       
+00014180: 2063 7376 7461 626c 6532 203d 206c 742e   csvtable2 = lt.
+00014190: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+000141a0: 7274 2864 6174 612c 2074 7261 6e73 666f  rt(data, transfo
+000141b0: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
+000141c0: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
+000141d0: 747d 2c0a 2020 2020 2020 2020 2020 2020  t},.            
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141f0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00014200: 775f 636c 6173 733d 7479 7065 2872 6f77  w_class=type(row
+00014210: 5f70 726f 746f 7479 7065 2929 5b3a 335d  _prototype))[:3]
+00014220: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00014230: 7479 7065 2874 315b 305d 292e 5f5f 6e61  type(t1[0]).__na
+00014240: 6d65 5f5f 2c20 7431 5b30 5d29 0a20 2020  me__, t1[0]).   
+00014250: 2020 2020 2070 7269 6e74 2874 7970 6528       print(type(
+00014260: 6373 7674 6162 6c65 325b 305d 292e 5f5f  csvtable2[0]).__
+00014270: 6e61 6d65 5f5f 2c20 6373 7674 6162 6c65  name__, csvtable
+00014280: 325b 305d 290a 2020 2020 2020 2020 7769  2[0]).        wi
+00014290: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+000142a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000142b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000142c0: 7479 7065 2874 315b 305d 292c 2074 7970  type(t1[0]), typ
+000142d0: 6528 6373 7674 6162 6c65 325b 305d 2929  e(csvtable2[0]))
+000142e0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+000142f0: 7376 5f6e 756d 6572 6963 5f74 7261 6e73  sv_numeric_trans
+00014300: 666f 726d 7328 7365 6c66 293a 0a20 2020  forms(self):.   
+00014310: 2020 2020 2064 6174 6120 3d20 7465 7874       data = text
+00014320: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+00014330: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+00014340: 652c 7661 6c75 650a 2020 2020 2020 2020  e,value.        
+00014350: 2020 2020 696e 742c 3130 3030 0a20 2020      int,1000.   
+00014360: 2020 2020 2020 2020 2066 6c6f 6174 2c33           float,3
+00014370: 2e31 340a 2020 2020 2020 2020 2020 2020  .14.            
+00014380: 656d 7074 792c 0a20 2020 2020 2020 2020  empty,.         
+00014390: 2020 2073 7472 2ce2 93a0 2a62 6572 740a     str,...*bert.
+000143a0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+000143b0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+000143c0: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
+000143d0: 7665 7274 5f6e 756d 6572 6963 2229 3a0a  vert_numeric"):.
+000143e0: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
+000143f0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00014400: 5f69 6d70 6f72 7428 6461 7461 2c20 7472  _import(data, tr
+00014410: 616e 7366 6f72 6d73 3d7b 2776 616c 7565  ansforms={'value
+00014420: 273a 206c 742e 5461 626c 652e 636f 6e76  ': lt.Table.conv
+00014430: 6572 745f 6e75 6d65 7269 637d 290a 2020  ert_numeric}).  
+00014440: 2020 2020 2020 2020 2020 7462 6c2e 7072            tbl.pr
+00014450: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+00014460: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00014470: 7175 616c 285b 3130 3030 2c20 332e 3134  qual([1000, 3.14
+00014480: 2c20 2727 2c20 27e2 93a0 2a62 6572 7427  , '', '...*bert'
+00014490: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
+000144a0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
+000144b0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000144c0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
+000144d0: 7269 6328 2922 293a 0a20 2020 2020 2020  ric()"):.       
+000144e0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+000144f0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00014500: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
+00014510: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
+00014520: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
+00014530: 6572 6963 2829 7d29 0a20 2020 2020 2020  eric()}).       
+00014540: 2020 2020 2074 626c 2e70 7265 7365 6e74       tbl.present
+00014550: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00014560: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00014570: 5b31 3030 302c 2033 2e31 342c 2027 272c  [1000, 3.14, '',
+00014580: 2027 e293 a02a 6265 7274 275d 2c20 6c69   '...*bert'], li
+00014590: 7374 2874 626c 2e61 6c6c 2e76 616c 7565  st(tbl.all.value
+000145a0: 2929 0a0a 2020 2020 2020 2020 7769 7468  ))..        with
+000145b0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+000145c0: 6f6e 7665 7274 5f6e 756d 6572 6963 286e  onvert_numeric(n
+000145d0: 6f6e 5f6e 756d 6572 6963 3d4e 6f6e 6529  on_numeric=None)
+000145e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000145f0: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
+00014600: 2e63 7376 5f69 6d70 6f72 7428 6461 7461  .csv_import(data
+00014610: 2c20 7472 616e 7366 6f72 6d73 3d7b 2776  , transforms={'v
+00014620: 616c 7565 273a 206c 742e 5461 626c 652e  alue': lt.Table.
+00014630: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
+00014640: 6e6f 6e5f 6e75 6d65 7269 633d 4e6f 6e65  non_numeric=None
+00014650: 297d 290a 2020 2020 2020 2020 2020 2020  )}).            
+00014660: 7462 6c2e 7072 6573 656e 7428 290a 2020  tbl.present().  
+00014670: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00014680: 7373 6572 7445 7175 616c 285b 3130 3030  ssertEqual([1000
+00014690: 2c20 332e 3134 2c20 2727 2c20 4e6f 6e65  , 3.14, '', None
+000146a0: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
+000146b0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
+000146c0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000146d0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
+000146e0: 7269 6328 6e6f 6e5f 6e75 6d65 7269 633d  ric(non_numeric=
+000146f0: 3029 2229 3a0a 2020 2020 2020 2020 2020  0)"):.          
+00014700: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00014710: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
+00014720: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
+00014730: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
+00014740: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
+00014750: 6328 6e6f 6e5f 6e75 6d65 7269 633d 3029  c(non_numeric=0)
+00014760: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+00014770: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
+00014780: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00014790: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
+000147a0: 2033 2e31 342c 2027 272c 2030 5d2c 206c   3.14, '', 0], l
+000147b0: 6973 7428 7462 6c2e 616c 6c2e 7661 6c75  ist(tbl.all.valu
+000147c0: 6529 290a 0a20 2020 2020 2020 2077 6974  e))..        wit
+000147d0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+000147e0: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
+000147f0: 696e 745f 746f 5f66 6c6f 6174 3d54 7275  int_to_float=Tru
+00014800: 6529 2229 3a0a 2020 2020 2020 2020 2020  e)"):.          
+00014810: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00014820: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
+00014830: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
+00014840: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
+00014850: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
+00014860: 6328 666f 7263 655f 666c 6f61 743d 5472  c(force_float=Tr
+00014870: 7565 297d 290a 2020 2020 2020 2020 2020  ue)}).          
+00014880: 2020 7462 6c2e 7072 6573 656e 7428 290a    tbl.present().
+00014890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000148a0: 2e61 7373 6572 7445 7175 616c 285b 3130  .assertEqual([10
+000148b0: 3030 2e30 2c20 332e 3134 2c20 2727 2c20  00.0, 3.14, '', 
+000148c0: 27e2 93a0 2a62 6572 7427 5d2c 206c 6973  '...*bert'], lis
+000148d0: 7428 7462 6c2e 616c 6c2e 7661 6c75 6529  t(tbl.all.value)
+000148e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000148f0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00014900: 666c 6f61 742c 2066 6c6f 6174 2c20 7374  float, float, st
+00014910: 722c 2073 7472 5d2c 206c 6973 7428 7479  r, str], list(ty
+00014920: 7065 2876 2920 666f 7220 7620 696e 2074  pe(v) for v in t
+00014930: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
+00014940: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00014950: 662e 7375 6254 6573 7428 2263 6f6e 7665  f.subTest("conve
+00014960: 7274 5f6e 756d 6572 6963 286e 6f6e 5f6e  rt_numeric(non_n
+00014970: 756d 6572 6963 3d4e 6f6e 652c 2065 6d70  umeric=None, emp
+00014980: 7479 3d4e 6f6e 6529 2229 3a0a 2020 2020  ty=None)"):.    
+00014990: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
+000149a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+000149b0: 6f72 7428 6461 7461 2c20 7472 616e 7366  ort(data, transf
+000149c0: 6f72 6d73 3d7b 2776 616c 7565 273a 206c  orms={'value': l
+000149d0: 742e 5461 626c 652e 636f 6e76 6572 745f  t.Table.convert_
+000149e0: 6e75 6d65 7269 6328 6e6f 6e5f 6e75 6d65  numeric(non_nume
+000149f0: 7269 633d 4e6f 6e65 2c20 656d 7074 793d  ric=None, empty=
+00014a00: 4e6f 6e65 297d 290a 2020 2020 2020 2020  None)}).        
+00014a10: 2020 2020 7462 6c2e 7072 6573 656e 7428      tbl.present(
+00014a20: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00014a30: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00014a40: 3130 3030 2c20 332e 3134 2c20 4e6f 6e65  1000, 3.14, None
+00014a50: 2c20 4e6f 6e65 5d2c 206c 6973 7428 7462  , None], list(tb
+00014a60: 6c2e 616c 6c2e 7661 6c75 6529 290a 0a20  l.all.value)).. 
+00014a70: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00014a80: 2e73 7562 5465 7374 2822 636f 6e76 6572  .subTest("conver
+00014a90: 745f 6e75 6d65 7269 6328 656d 7074 793d  t_numeric(empty=
+00014aa0: 4e6f 6e65 2922 293a 0a20 2020 2020 2020  None)"):.       
+00014ab0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+00014ac0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00014ad0: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
+00014ae0: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
+00014af0: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
+00014b00: 6572 6963 2865 6d70 7479 3d4e 6f6e 6529  eric(empty=None)
+00014b10: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+00014b20: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
+00014b30: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00014b40: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
+00014b50: 2033 2e31 342c 204e 6f6e 652c 2027 e293   3.14, None, '..
+00014b60: a02a 6265 7274 275d 2c20 6c69 7374 2874  .*bert'], list(t
+00014b70: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
+00014b80: 2020 2020 6465 6620 7465 7374 5f6a 736f      def test_jso
+00014b90: 6e5f 6578 706f 7274 5f73 7472 6561 6d69  n_export_streami
+00014ba0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
+00014bb0: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
+00014bc0: 2069 6d70 6f72 7420 7065 726d 7574 6174   import permutat
+00014bd0: 696f 6e73 0a20 2020 2020 2020 2074 6573  ions.        tes
+00014be0: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
+00014bf0: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+00014c00: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+00014c10: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+00014c20: 6573 745f 7369 7a65 290a 2020 2020 2020  est_size).      
+00014c30: 2020 666f 7220 6669 656c 646e 616d 6573    for fieldnames
+00014c40: 2069 6e20 7065 726d 7574 6174 696f 6e73   in permutations
+00014c50: 286c 6973 7428 2761 6263 2729 293a 0a20  (list('abc')):. 
+00014c60: 2020 2020 2020 2020 2020 206f 7574 5f73             out_s
+00014c70: 7472 696e 6720 3d20 7431 2e6a 736f 6e5f  tring = t1.json_
+00014c80: 6578 706f 7274 284e 6f6e 652c 2066 6965  export(None, fie
+00014c90: 6c64 6e61 6d65 733d 6669 656c 646e 616d  ldnames=fieldnam
+00014ca0: 6573 2c20 7374 7265 616d 696e 673d 5472  es, streaming=Tr
+00014cb0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00014cc0: 6f75 746c 696e 6573 203d 206f 7574 5f73  outlines = out_s
+00014cd0: 7472 696e 672e 7370 6c69 746c 696e 6573  tring.splitlines
+00014ce0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00014cf0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00014d00: 7428 6669 656c 646e 616d 6573 3d66 6965  t(fieldnames=fie
+00014d10: 6c64 6e61 6d65 7329 3a0a 2020 2020 2020  ldnames):.      
+00014d20: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00014d30: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00014d40: 7369 7a65 2a2a 332c 206c 656e 286f 7574  size**3, len(out
+00014d50: 6c69 6e65 7329 290a 0a20 2020 2020 2020  lines))..       
+00014d60: 2020 2020 2066 6f72 206f 622c 206c 696e       for ob, lin
+00014d70: 6520 696e 207a 6970 2874 312c 206f 7574  e in zip(t1, out
+00014d80: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
+00014d90: 2020 2020 2020 2020 6a73 6f6e 5f64 6963          json_dic
+00014da0: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 286c  t = json.loads(l
+00014db0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
+00014dc0: 2020 2020 2074 315f 6461 7461 6f62 6a20       t1_dataobj 
+00014dd0: 3d20 6d61 6b65 5f64 6174 616f 626a 6563  = make_dataobjec
+00014de0: 745f 6672 6f6d 5f6f 6228 6f62 290a 2020  t_from_ob(ob).  
+00014df0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00014e00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00014e10: 6f62 3d6f 622c 206c 696e 653d 6c69 6e65  ob=ob, line=line
+00014e20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
 00014e30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00014e40: 7274 5472 7565 2861 6c6c 286d 616b 655f  rtTrue(all(make_
-00014e50: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
-00014e60: 6f62 2872 6563 3129 203d 3d20 7265 6332  ob(rec1) == rec2
-00014e70: 2066 6f72 2072 6563 312c 2072 6563 3220   for rec1, rec2 
-00014e80: 696e 207a 6970 2874 312c 206a 736f 6e74  in zip(t1, jsont
-00014e90: 6162 6c65 2929 290a 2020 2020 2020 2020  able))).        
-00014ea0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00014eb0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00014ec0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00014ed0: 6c28 6c65 6e28 5b64 2066 6f72 2064 2069  l(len([d for d i
-00014ee0: 6e20 6461 7461 2e73 706c 6974 6c69 6e65  n data.splitline
-00014ef0: 7328 2920 6966 2064 2e73 7472 6970 2829  s() if d.strip()
-00014f00: 5d29 2c20 6c65 6e28 6a73 6f6e 7461 626c  ]), len(jsontabl
-00014f10: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
-00014f20: 745f 6a73 6f6e 5f73 7472 696e 675f 6c69  t_json_string_li
-00014f30: 7374 5f69 6d70 6f72 7428 7365 6c66 293a  st_import(self):
-00014f40: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00014f50: 6a73 6f6e 5f64 6174 610a 2020 2020 2020  json_data.      
-00014f60: 2020 6a73 6f6e 7461 626c 6520 3d20 6c74    jsontable = lt
-00014f70: 2e54 6162 6c65 2829 2e6a 736f 6e5f 696d  .Table().json_im
-00014f80: 706f 7274 2864 6174 612e 7370 6c69 746c  port(data.splitl
-00014f90: 696e 6573 2829 2c20 7374 7265 616d 696e  ines(), streamin
-00014fa0: 673d 5472 7565 2c20 7472 616e 7366 6f72  g=True, transfor
-00014fb0: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
-00014fc0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
-00014fd0: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
-00014fe0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
-00014ff0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
-00015000: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-00015010: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00015020: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-00015030: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00015040: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00015050: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00015060: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
-00015070: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
-00015080: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
-00015090: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
-000150a0: 6970 2874 312c 206a 736f 6e74 6162 6c65  ip(t1, jsontable
-000150b0: 2929 290a 2020 2020 2020 2020 7769 7468  ))).        with
-000150c0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-000150d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000150e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-000150f0: 6e28 5b64 2066 6f72 2064 2069 6e20 6461  n([d for d in da
-00015100: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
-00015110: 6966 2064 2e73 7472 6970 2829 5d29 2c20  if d.strip()]), 
-00015120: 6c65 6e28 6a73 6f6e 7461 626c 6529 290a  len(jsontable)).
-00015130: 0a20 2020 2064 6566 2074 6573 745f 6a73  .    def test_js
-00015140: 6f6e 5f6e 6f6e 7374 7265 616d 696e 675f  on_nonstreaming_
-00015150: 7769 7468 5f70 6174 685f 696d 706f 7274  with_path_import
-00015160: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00015170: 6461 7461 203d 206a 736f 6e5f 6461 7461  data = json_data
-00015180: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00015190: 272c 5c6e 272e 6a6f 696e 2864 6174 612e  ',\n'.join(data.
-000151a0: 7273 7472 6970 2829 2e73 706c 6974 6c69  rstrip().splitli
-000151b0: 6e65 7328 2929 0a20 2020 2020 2020 206a  nes()).        j
-000151c0: 736f 6e5f 696e 7075 7430 203d 2027 5b27  son_input0 = '['
-000151d0: 202b 2064 6174 6120 2b20 275d 270a 2020   + data + ']'.  
-000151e0: 2020 2020 2020 6a73 6f6e 5f69 6e70 7574        json_input
-000151f0: 3120 3d20 277b 2022 6461 7461 223a 205b  1 = '{ "data": [
-00015200: 2720 2b20 6461 7461 202b 2027 5d7d 270a  ' + data + ']}'.
-00015210: 2020 2020 2020 2020 6a73 6f6e 5f69 6e70          json_inp
-00015220: 7574 3220 3d20 277b 2022 6461 7461 223a  ut2 = '{ "data":
-00015230: 207b 2022 6974 656d 7322 3a20 5b27 202b   { "items": [' +
-00015240: 2064 6174 6120 2b20 275d 7d7d 270a 0a20   data + ']}}'.. 
-00015250: 2020 2020 2020 2066 6f72 206a 736f 6e5f         for json_
-00015260: 696e 7075 742c 2070 6174 6820 696e 205b  input, path in [
-00015270: 0a20 2020 2020 2020 2020 2020 2028 6a73  .            (js
-00015280: 6f6e 5f69 6e70 7574 302c 2022 2229 2c0a  on_input0, ""),.
-00015290: 2020 2020 2020 2020 2020 2020 286a 736f              (jso
-000152a0: 6e5f 696e 7075 7431 2c20 2264 6174 6122  n_input1, "data"
-000152b0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000152c0: 6a73 6f6e 5f69 6e70 7574 322c 2022 6461  json_input2, "da
-000152d0: 7461 2e69 7465 6d73 2229 2c0a 2020 2020  ta.items"),.    
-000152e0: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
-000152f0: 2020 206a 736f 6e74 6162 6c65 203d 206c     jsontable = l
-00015300: 742e 5461 626c 6528 292e 6a73 6f6e 5f69  t.Table().json_i
-00015310: 6d70 6f72 7428 6a73 6f6e 5f69 6e70 7574  mport(json_input
-00015320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015350: 2070 6174 683d 7061 7468 2c0a 2020 2020   path=path,.    
-00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015380: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00015390: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
-000153a0: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
-000153b0: 696e 747d 290a 0a20 2020 2020 2020 2020  int})..         
-000153c0: 2020 2074 6573 745f 7369 7a65 203d 2033     test_size = 3
-000153d0: 0a20 2020 2020 2020 2020 2020 2074 3120  .            t1 
-000153e0: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-000153f0: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00015400: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-00015410: 7a65 290a 0a20 2020 2020 2020 2020 2020  ze)..           
-00015420: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00015430: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00015440: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00015450: 7454 7275 6528 616c 6c28 6d61 6b65 5f64  tTrue(all(make_d
-00015460: 6174 616f 626a 6563 745f 6672 6f6d 5f6f  ataobject_from_o
-00015470: 6228 7265 6331 2920 3d3d 2072 6563 3220  b(rec1) == rec2 
-00015480: 666f 7220 7265 6331 2c20 7265 6332 2069  for rec1, rec2 i
-00015490: 6e20 7a69 7028 7431 2c20 6a73 6f6e 7461  n zip(t1, jsonta
-000154a0: 626c 6529 2929 0a20 2020 2020 2020 2020  ble))).         
-000154b0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000154c0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000154d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000154e0: 6572 7445 7175 616c 286c 656e 285b 6420  ertEqual(len([d 
-000154f0: 666f 7220 6420 696e 2064 6174 612e 7370  for d in data.sp
-00015500: 6c69 746c 696e 6573 2829 2069 6620 642e  litlines() if d.
-00015510: 7374 7269 7028 295d 292c 206c 656e 286a  strip()]), len(j
-00015520: 736f 6e74 6162 6c65 2929 0a0a 2020 2020  sontable))..    
-00015530: 6465 6620 7465 7374 5f6a 736f 6e5f 696d  def test_json_im
-00015540: 706f 7274 5f77 6974 685f 6375 7374 6f6d  port_with_custom
-00015550: 5f65 6e63 6f64 6572 2873 656c 6629 3a0a  _encoder(self):.
-00015560: 2020 2020 2020 2020 6672 6f6d 2064 6174          from dat
-00015570: 6574 696d 6520 696d 706f 7274 2064 6174  etime import dat
-00015580: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-00015590: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
-000155a0: 2761 273a 2031 3030 2c20 2762 273a 2064  'a': 100, 'b': d
-000155b0: 6174 6528 3230 3030 2c20 312c 2031 292c  ate(2000, 1, 1),
-000155c0: 2027 6327 3a20 3230 307d 2c0a 2020 2020   'c': 200},.    
-000155d0: 2020 2020 2020 2020 7b27 6127 3a20 3130          {'a': 10
-000155e0: 312c 2027 6227 3a20 6461 7465 2832 3030  1, 'b': date(200
-000155f0: 312c 2031 2c20 3129 2c20 2763 273a 2032  1, 1, 1), 'c': 2
-00015600: 3031 7d2c 0a20 2020 2020 2020 205d 0a20  01},.        ]. 
-00015610: 2020 2020 2020 2074 626c 203d 206c 742e         tbl = lt.
-00015620: 5461 626c 6528 292e 696e 7365 7274 5f6d  Table().insert_m
-00015630: 616e 7928 6461 7461 290a 2020 2020 2020  any(data).      
-00015640: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-00015650: 7274 5261 6973 6573 2854 7970 6545 7272  rtRaises(TypeErr
-00015660: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00015670: 2078 203d 2074 626c 2e6a 736f 6e5f 6578   x = tbl.json_ex
-00015680: 706f 7274 2829 0a0a 2020 2020 2020 2020  port()..        
-00015690: 636c 6173 7320 4a73 6f6e 4461 7465 456e  class JsonDateEn
-000156a0: 636f 6465 7228 6a73 6f6e 2e4a 534f 4e45  coder(json.JSONE
-000156b0: 6e63 6f64 6572 293a 0a20 2020 2020 2020  ncoder):.       
-000156c0: 2020 2020 2064 6566 2064 6566 6175 6c74       def default
-000156d0: 2873 656c 662c 206f 293a 0a20 2020 2020  (self, o):.     
-000156e0: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
-000156f0: 7420 6461 7465 7469 6d65 0a20 2020 2020  t datetime.     
-00015700: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00015710: 696e 7374 616e 6365 286f 2c20 6461 7465  instance(o, date
-00015720: 7469 6d65 2e64 6174 6529 3a0a 2020 2020  time.date):.    
-00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015740: 7265 7475 726e 2073 7472 286f 290a 2020  return str(o).  
-00015750: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015760: 7475 726e 2073 7570 6572 2829 2e64 6566  turn super().def
-00015770: 6175 6c74 286f 290a 0a20 2020 2020 2020  ault(o)..       
-00015780: 2065 7870 6563 7465 6420 3d20 7465 7874   expected = text
-00015790: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-000157a0: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-000157b0: 2020 2020 2020 2020 2020 207b 2261 223a             {"a":
-000157c0: 2031 3030 2c20 2262 223a 2022 3230 3030   100, "b": "2000
-000157d0: 2d30 312d 3031 222c 2022 6322 3a20 3230  -01-01", "c": 20
-000157e0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-000157f0: 7b22 6122 3a20 3130 312c 2022 6222 3a20  {"a": 101, "b": 
-00015800: 2232 3030 312d 3031 2d30 3122 2c20 2263  "2001-01-01", "c
-00015810: 223a 2032 3031 7d0a 2020 2020 2020 2020  ": 201}.        
-00015820: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00015830: 2020 2222 2229 0a20 2020 2020 2020 206a    """).        j
-00015840: 736f 6e5f 7265 7375 6c74 203d 2074 626c  son_result = tbl
-00015850: 2e6a 736f 6e5f 6578 706f 7274 286a 736f  .json_export(jso
-00015860: 6e5f 656e 636f 6465 723d 4a73 6f6e 4461  n_encoder=JsonDa
-00015870: 7465 456e 636f 6465 7229 0a20 2020 2020  teEncoder).     
-00015880: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00015890: 7561 6c28 6578 7065 6374 6564 2c20 6a73  ual(expected, js
-000158a0: 6f6e 5f72 6573 756c 7429 0a0a 2020 2020  on_result)..    
-000158b0: 6465 6620 7465 7374 5f6a 736f 6e5f 696d  def test_json_im
-000158c0: 706f 7274 5f77 6974 685f 6d75 6c74 6970  port_with_multip
-000158d0: 6c65 5f63 7573 746f 6d5f 656e 636f 6465  le_custom_encode
-000158e0: 7273 2873 656c 6629 3a0a 2020 2020 2020  rs(self):.      
-000158f0: 2020 6672 6f6d 2064 6174 6574 696d 6520    from datetime 
-00015900: 696d 706f 7274 2064 6174 650a 0a20 2020  import date..   
-00015910: 2020 2020 2063 6c61 7373 2041 4141 3a0a       class AAA:.
-00015920: 2020 2020 2020 2020 2020 2020 6465 6620              def 
-00015930: 5f5f 696e 6974 5f5f 2873 656c 662c 206e  __init__(self, n
-00015940: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-00015950: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00015960: 3d20 6e61 6d65 0a0a 2020 2020 2020 2020  = name..        
-00015970: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00015980: 2020 2020 207b 2761 273a 2031 3030 2c20       {'a': 100, 
-00015990: 2762 273a 2064 6174 6528 3230 3030 2c20  'b': date(2000, 
-000159a0: 312c 2031 292c 2027 6327 3a20 3230 302c  1, 1), 'c': 200,
-000159b0: 2027 6427 3a20 4141 4128 2241 6c69 6365   'd': AAA("Alice
-000159c0: 2229 7d2c 0a20 2020 2020 2020 2020 2020  ")},.           
-000159d0: 207b 2761 273a 2031 3031 2c20 2762 273a   {'a': 101, 'b':
-000159e0: 2064 6174 6528 3230 3031 2c20 312c 2031   date(2001, 1, 1
-000159f0: 292c 2027 6327 3a20 3230 312c 2027 6427  ), 'c': 201, 'd'
-00015a00: 3a20 4141 4128 2242 6f62 2229 7d2c 0a20  : AAA("Bob")},. 
-00015a10: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00015a20: 2074 626c 203d 206c 742e 5461 626c 6528   tbl = lt.Table(
-00015a30: 292e 696e 7365 7274 5f6d 616e 7928 6461  ).insert_many(da
-00015a40: 7461 290a 2020 2020 2020 2020 7769 7468  ta).        with
-00015a50: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00015a60: 6573 2854 7970 6545 7272 6f72 293a 0a20  es(TypeError):. 
-00015a70: 2020 2020 2020 2020 2020 2078 203d 2074             x = t
-00015a80: 626c 2e6a 736f 6e5f 6578 706f 7274 2829  bl.json_export()
-00015a90: 0a0a 2020 2020 2020 2020 636c 6173 7320  ..        class 
-00015aa0: 4a73 6f6e 4461 7465 456e 636f 6465 7228  JsonDateEncoder(
-00015ab0: 6a73 6f6e 2e4a 534f 4e45 6e63 6f64 6572  json.JSONEncoder
-00015ac0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00015ad0: 6566 2064 6566 6175 6c74 2873 656c 662c  ef default(self,
-00015ae0: 206f 293a 0a20 2020 2020 2020 2020 2020   o):.           
-00015af0: 2020 2020 2069 6d70 6f72 7420 6461 7465       import date
-00015b00: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
-00015b10: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00015b20: 6365 286f 2c20 6461 7465 7469 6d65 2e64  ce(o, datetime.d
-00015b30: 6174 6529 3a0a 2020 2020 2020 2020 2020  ate):.          
-00015b40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00015b50: 2073 7472 286f 290a 2020 2020 2020 2020   str(o).        
-00015b60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00015b70: 7570 6572 2829 2e64 6566 6175 6c74 286f  uper().default(o
-00015b80: 290a 0a20 2020 2020 2020 2063 6c61 7373  )..        class
-00015b90: 204a 736f 6e41 4141 456e 636f 6465 7228   JsonAAAEncoder(
-00015ba0: 6a73 6f6e 2e4a 534f 4e45 6e63 6f64 6572  json.JSONEncoder
-00015bb0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00015bc0: 6566 2064 6566 6175 6c74 2873 656c 662c  ef default(self,
-00015bd0: 206f 293a 0a20 2020 2020 2020 2020 2020   o):.           
-00015be0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00015bf0: 6365 286f 2c20 4141 4129 3a0a 2020 2020  ce(o, AAA):.    
-00015c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c10: 7265 7475 726e 2066 2241 4141 286e 616d  return f"AAA(nam
-00015c20: 653d 7b6f 2e6e 616d 6521 727d 2922 0a0a  e={o.name!r})"..
-00015c30: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00015c40: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-00015c50: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-00015c60: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00015c70: 2020 7b22 6122 3a20 3130 302c 2022 6222    {"a": 100, "b"
-00015c80: 3a20 2232 3030 302d 3031 2d30 3122 2c20  : "2000-01-01", 
-00015c90: 2263 223a 2032 3030 2c20 2264 223a 2022  "c": 200, "d": "
-00015ca0: 4141 4128 6e61 6d65 3d27 416c 6963 6527  AAA(name='Alice'
-00015cb0: 2922 7d2c 0a20 2020 2020 2020 2020 2020  )"},.           
-00015cc0: 207b 2261 223a 2031 3031 2c20 2262 223a   {"a": 101, "b":
-00015cd0: 2022 3230 3031 2d30 312d 3031 222c 2022   "2001-01-01", "
-00015ce0: 6322 3a20 3230 312c 2022 6422 3a20 2241  c": 201, "d": "A
-00015cf0: 4141 286e 616d 653d 2742 6f62 2729 227d  AA(name='Bob')"}
-00015d00: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00015d10: 2020 2020 2020 2022 2222 290a 0a20 2020         """)..   
-00015d20: 2020 2020 206a 736f 6e5f 7265 7375 6c74       json_result
-00015d30: 203d 2074 626c 2e6a 736f 6e5f 6578 706f   = tbl.json_expo
-00015d40: 7274 286a 736f 6e5f 656e 636f 6465 723d  rt(json_encoder=
-00015d50: 284a 736f 6e44 6174 6545 6e63 6f64 6572  (JsonDateEncoder
-00015d60: 2c20 4a73 6f6e 4141 4145 6e63 6f64 6572  , JsonAAAEncoder
-00015d70: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00015d80: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-00015d90: 6374 6564 2c20 6a73 6f6e 5f72 6573 756c  cted, json_resul
-00015da0: 7429 0a0a 2020 2020 6465 6620 7465 7374  t)..    def test
-00015db0: 5f66 6978 6564 5f77 6964 7468 5f69 6d70  _fixed_width_imp
-00015dc0: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
-00015dd0: 2020 2064 6174 6120 3d20 6669 7865 645f     data = fixed_
-00015de0: 7769 6474 685f 6461 7461 0a20 2020 2020  width_data.     
-00015df0: 2020 2064 6174 615f 6669 6c65 203d 2069     data_file = i
-00015e00: 6f2e 5374 7269 6e67 494f 2864 6174 6129  o.StringIO(data)
-00015e10: 0a20 2020 2020 2020 2066 775f 7370 6563  .        fw_spec
-00015e20: 203d 205b 2827 6127 2c20 302c 204e 6f6e   = [('a', 0, Non
-00015e30: 652c 2069 6e74 292c 2028 2762 272c 2032  e, int), ('b', 2
-00015e40: 2c20 4e6f 6e65 2c20 696e 7429 2c20 2827  , None, int), ('
-00015e50: 6327 2c20 342c 204e 6f6e 652c 2069 6e74  c', 4, None, int
-00015e60: 292c 205d 0a20 2020 2020 2020 2074 7420  ), ].        tt 
-00015e70: 3d20 6c74 2e54 6162 6c65 2829 2e69 6e73  = lt.Table().ins
-00015e80: 6572 745f 6d61 6e79 286c 742e 4461 7461  ert_many(lt.Data
-00015e90: 4f62 6a65 6374 282a 2a72 6563 2920 666f  Object(**rec) fo
-00015ea0: 7220 7265 6320 696e 206c 742e 4669 7865  r rec in lt.Fixe
-00015eb0: 6457 6964 7468 5265 6164 6572 2866 775f  dWidthReader(fw_
-00015ec0: 7370 6563 2c20 6461 7461 5f66 696c 6529  spec, data_file)
-00015ed0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
-00015ee0: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
-00015ef0: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
-00015f00: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
-00015f10: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
-00015f20: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-00015f30: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00015f40: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00015f50: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00015f60: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
-00015f70: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
-00015f80: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
-00015f90: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
-00015fa0: 7028 7431 2c20 7474 2929 290a 2020 2020  p(t1, tt))).    
-00015fb0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00015fc0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-00015fd0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00015fe0: 4571 7561 6c28 6c65 6e28 5b64 2066 6f72  Equal(len([d for
-00015ff0: 2064 2069 6e20 6461 7461 2e73 706c 6974   d in data.split
-00016000: 6c69 6e65 7328 2920 6966 2064 2e73 7472  lines() if d.str
-00016010: 6970 2829 5d29 2c20 6c65 6e28 7474 2929  ip()]), len(tt))
-00016020: 0a0a 2020 2020 6465 6620 7465 7374 5f66  ..    def test_f
-00016030: 6978 6564 5f77 6964 7468 5f73 7472 696e  ixed_width_strin
-00016040: 675f 696d 706f 7274 2873 656c 6629 3a0a  g_import(self):.
-00016050: 2020 2020 2020 2020 6461 7461 203d 2066          data = f
-00016060: 6978 6564 5f77 6964 7468 5f64 6174 610a  ixed_width_data.
-00016070: 2020 2020 2020 2020 6677 5f73 7065 6320          fw_spec 
-00016080: 3d20 5b28 2761 272c 2030 2c20 4e6f 6e65  = [('a', 0, None
-00016090: 2c20 696e 7429 2c20 2827 6227 2c20 322c  , int), ('b', 2,
-000160a0: 204e 6f6e 652c 2069 6e74 292c 2028 2763   None, int), ('c
-000160b0: 272c 2034 2c20 4e6f 6e65 2c20 696e 7429  ', 4, None, int)
-000160c0: 2c20 5d0a 2020 2020 2020 2020 7474 203d  , ].        tt =
-000160d0: 206c 742e 5461 626c 6528 292e 696e 7365   lt.Table().inse
-000160e0: 7274 5f6d 616e 7928 6c74 2e44 6174 614f  rt_many(lt.DataO
-000160f0: 626a 6563 7428 2a2a 7265 6329 2066 6f72  bject(**rec) for
-00016100: 2072 6563 2069 6e20 6c74 2e46 6978 6564   rec in lt.Fixed
-00016110: 5769 6474 6852 6561 6465 7228 6677 5f73  WidthReader(fw_s
-00016120: 7065 632c 2064 6174 6129 290a 0a20 2020  pec, data))..   
-00016130: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
-00016140: 2033 0a20 2020 2020 2020 2074 3120 3d20   3.        t1 = 
-00016150: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-00016160: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-00016170: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
-00016180: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00016190: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-000161a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000161b0: 2e61 7373 6572 7454 7275 6528 616c 6c28  .assertTrue(all(
-000161c0: 6d61 6b65 5f64 6174 616f 626a 6563 745f  make_dataobject_
-000161d0: 6672 6f6d 5f6f 6228 7265 6331 2920 3d3d  from_ob(rec1) ==
-000161e0: 2072 6563 3220 666f 7220 7265 6331 2c20   rec2 for rec1, 
-000161f0: 7265 6332 2069 6e20 7a69 7028 7431 2c20  rec2 in zip(t1, 
-00016200: 7474 2929 290a 2020 2020 2020 2020 7769  tt))).        wi
-00016210: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00016220: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00016230: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00016240: 6c65 6e28 5b64 2066 6f72 2064 2069 6e20  len([d for d in 
-00016250: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
-00016260: 2920 6966 2064 2e73 7472 6970 2829 5d29  ) if d.strip()])
-00016270: 2c20 6c65 6e28 7474 2929 0a0a 2020 2020  , len(tt))..    
-00016280: 6465 6620 7465 7374 5f66 6978 6564 5f77  def test_fixed_w
-00016290: 6964 7468 5f73 7472 696e 675f 6c69 7374  idth_string_list
-000162a0: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
-000162b0: 2020 2020 2020 2064 6174 6120 3d20 6669         data = fi
-000162c0: 7865 645f 7769 6474 685f 6461 7461 0a20  xed_width_data. 
-000162d0: 2020 2020 2020 2066 775f 7370 6563 203d         fw_spec =
-000162e0: 205b 2827 6127 2c20 302c 204e 6f6e 652c   [('a', 0, None,
-000162f0: 2069 6e74 292c 2028 2762 272c 2032 2c20   int), ('b', 2, 
-00016300: 4e6f 6e65 2c20 696e 7429 2c20 2827 6327  None, int), ('c'
-00016310: 2c20 342c 204e 6f6e 652c 2069 6e74 292c  , 4, None, int),
-00016320: 5d0a 2020 2020 2020 2020 7474 203d 206c  ].        tt = l
-00016330: 742e 5461 626c 6528 292e 696e 7365 7274  t.Table().insert
-00016340: 5f6d 616e 7928 6c74 2e44 6174 614f 626a  _many(lt.DataObj
-00016350: 6563 7428 2a2a 7265 6329 2066 6f72 2072  ect(**rec) for r
-00016360: 6563 2069 6e20 6c74 2e46 6978 6564 5769  ec in lt.FixedWi
-00016370: 6474 6852 6561 6465 7228 6677 5f73 7065  dthReader(fw_spe
-00016380: 632c 2064 6174 612e 7370 6c69 746c 696e  c, data.splitlin
-00016390: 6573 2829 2929 0a0a 2020 2020 2020 2020  es()))..        
-000163a0: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
-000163b0: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
-000163c0: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
-000163d0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-000163e0: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
-000163f0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00016400: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00016410: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00016420: 7274 5472 7565 2861 6c6c 286d 616b 655f  rtTrue(all(make_
-00016430: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
-00016440: 6f62 2872 6563 3129 203d 3d20 7265 6332  ob(rec1) == rec2
-00016450: 2066 6f72 2072 6563 312c 2072 6563 3220   for rec1, rec2 
-00016460: 696e 207a 6970 2874 312c 2074 7429 2929  in zip(t1, tt)))
-00016470: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00016480: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00016490: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000164a0: 7373 6572 7445 7175 616c 286c 656e 285b  ssertEqual(len([
-000164b0: 6420 666f 7220 6420 696e 2064 6174 612e  d for d in data.
-000164c0: 7370 6c69 746c 696e 6573 2829 2069 6620  splitlines() if 
-000164d0: 642e 7374 7269 7028 295d 292c 206c 656e  d.strip()]), len
-000164e0: 2874 7429 290a 0a20 2020 2064 6566 2074  (tt))..    def t
-000164f0: 6573 745f 6578 6365 6c5f 696d 706f 7274  est_excel_import
-00016500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016510: 6669 6c65 5f6e 616d 6520 3d20 2274 6573  file_name = "tes
-00016520: 742f 6162 632e 786c 7378 220a 2020 2020  t/abc.xlsx".    
-00016530: 2020 2020 6578 6365 6c5f 7461 626c 6520      excel_table 
-00016540: 3d20 6c74 2e54 6162 6c65 2829 2e65 7863  = lt.Table().exc
-00016550: 656c 5f69 6d70 6f72 7428 6669 6c65 5f6e  el_import(file_n
-00016560: 616d 652c 2074 7261 6e73 666f 726d 733d  ame, transforms=
-00016570: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
-00016580: 696e 742c 2027 6327 3a20 696e 747d 290a  int, 'c': int}).
-00016590: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-000165a0: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
-000165b0: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
-000165c0: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
-000165d0: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
-000165e0: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
-000165f0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00016600: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00016610: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00016620: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
-00016630: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
-00016640: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
-00016650: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
-00016660: 7431 2c20 6578 6365 6c5f 7461 626c 6529  t1, excel_table)
-00016670: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-00016680: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00016690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000166a0: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
-000166b0: 2831 2066 6f72 206c 696e 6520 696e 2063  (1 for line in c
-000166c0: 7376 5f64 6174 612e 7370 6c69 746c 696e  sv_data.splitlin
-000166d0: 6573 2829 2069 6620 6c69 6e65 2e73 7472  es() if line.str
-000166e0: 6970 2829 292d 312c 206c 656e 2865 7863  ip())-1, len(exc
-000166f0: 656c 5f74 6162 6c65 2929 0a0a 2020 2020  el_table))..    
-00016700: 2020 2020 726f 775f 7072 6f74 6f74 7970      row_prototyp
-00016710: 6520 3d20 7365 6c66 2e6d 616b 655f 6461  e = self.make_da
-00016720: 7461 5f6f 626a 6563 7428 302c 2030 2c20  ta_object(0, 0, 
-00016730: 3029 0a20 2020 2020 2020 2063 7376 7461  0).        csvta
-00016740: 626c 6532 203d 206c 742e 5461 626c 6528  ble2 = lt.Table(
-00016750: 292e 6578 6365 6c5f 696d 706f 7274 280a  ).excel_import(.
-00016760: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00016770: 5f6e 616d 652c 2074 7261 6e73 666f 726d  _name, transform
-00016780: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
-00016790: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
-000167a0: 2c20 726f 775f 636c 6173 733d 7479 7065  , row_class=type
-000167b0: 2872 6f77 5f70 726f 746f 7479 7065 290a  (row_prototype).
-000167c0: 2020 2020 2020 2020 295b 3a33 5d0a 0a20          )[:3].. 
-000167d0: 2020 2020 2020 2070 7269 6e74 2874 7970         print(typ
-000167e0: 6528 7431 5b30 5d29 2e5f 5f6e 616d 655f  e(t1[0]).__name_
-000167f0: 5f2c 2074 315b 305d 290a 2020 2020 2020  _, t1[0]).      
-00016800: 2020 7072 696e 7428 7479 7065 2863 7376    print(type(csv
-00016810: 7461 626c 6532 5b30 5d29 2e5f 5f6e 616d  table2[0]).__nam
-00016820: 655f 5f2c 2063 7376 7461 626c 6532 5b30  e__, csvtable2[0
-00016830: 5d29 0a20 2020 2020 2020 2077 6974 6820  ]).        with 
-00016840: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00016850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016860: 2e61 7373 6572 7445 7175 616c 2874 7970  .assertEqual(typ
-00016870: 6528 7431 5b30 5d29 2c20 7479 7065 2863  e(t1[0]), type(c
-00016880: 7376 7461 626c 6532 5b30 5d29 290a 0a20  svtable2[0])).. 
-00016890: 2020 2064 6566 2074 6573 745f 6578 6365     def test_exce
-000168a0: 6c5f 6578 706f 7274 2873 656c 6629 3a0a  l_export(self):.
-000168b0: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
-000168c0: 6520 3d20 2274 6573 742f 6162 632e 786c  e = "test/abc.xl
-000168d0: 7378 220a 2020 2020 2020 2020 6578 6365  sx".        exce
-000168e0: 6c5f 7461 626c 6520 3d20 6c74 2e54 6162  l_table = lt.Tab
-000168f0: 6c65 2829 2e65 7863 656c 5f69 6d70 6f72  le().excel_impor
-00016900: 7428 6669 6c65 5f6e 616d 652c 2074 7261  t(file_name, tra
-00016910: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
-00016920: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
-00016930: 3a20 696e 747d 2c20 6c69 6d69 743d 3129  : int}, limit=1)
-00016940: 0a20 2020 2020 2020 206f 7574 6669 6c65  .        outfile
-00016950: 203d 2069 6f2e 4279 7465 7349 4f28 290a   = io.BytesIO().
-00016960: 2020 2020 2020 2020 6578 6365 6c5f 7461          excel_ta
-00016970: 626c 652e 6578 6365 6c5f 6578 706f 7274  ble.excel_export
-00016980: 286f 7574 6669 6c65 290a 2020 2020 2020  (outfile).      
-00016990: 2020 6578 706f 7274 6564 5f74 6162 6c65    exported_table
-000169a0: 203d 206c 742e 5461 626c 6528 292e 6578   = lt.Table().ex
-000169b0: 6365 6c5f 696d 706f 7274 286f 7574 6669  cel_import(outfi
-000169c0: 6c65 2c20 7472 616e 7366 6f72 6d73 3d7b  le, transforms={
-000169d0: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
-000169e0: 6e74 2c20 2763 273a 2069 6e74 7d29 0a0a  nt, 'c': int})..
-000169f0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00016a00: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00016a10: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00016a20: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
-00016a30: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
-00016a40: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
-00016a50: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
-00016a60: 3220 696e 207a 6970 2865 7870 6f72 7465  2 in zip(exporte
-00016a70: 645f 7461 626c 652c 2065 7863 656c 5f74  d_table, excel_t
-00016a80: 6162 6c65 2929 290a 0a0a 406d 616b 655f  able)))...@make_
-00016a90: 7465 7374 5f63 6c61 7373 6573 0a63 6c61  test_classes.cla
-00016aa0: 7373 2054 6162 6c65 5069 766f 7454 6573  ss TablePivotTes
-00016ab0: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
-00016ac0: 5f70 6976 6f74 2873 656c 6629 3a0a 2020  _pivot(self):.  
-00016ad0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00016ae0: 3d20 350a 2020 2020 2020 2020 7431 203d  = 5.        t1 =
-00016af0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00016b00: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00016b10: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-00016b20: 6529 0a20 2020 2020 2020 2074 312e 6372  e).        t1.cr
-00016b30: 6561 7465 5f69 6e64 6578 2827 6127 290a  eate_index('a').
-00016b40: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
-00016b50: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
-00016b60: 2020 2020 2074 3170 6976 6f74 203d 2074       t1pivot = t
-00016b70: 312e 7069 766f 7428 2761 2729 0a20 2020  1.pivot('a').   
-00016b80: 2020 2020 2074 3170 6976 6f74 2e64 756d       t1pivot.dum
-00016b90: 7028 290a 2020 2020 2020 2020 7431 7069  p().        t1pi
-00016ba0: 766f 742e 6475 6d70 5f63 6f75 6e74 7328  vot.dump_counts(
-00016bb0: 290a 2020 2020 2020 2020 7431 7069 766f  ).        t1pivo
-00016bc0: 742e 7375 6d6d 6172 795f 636f 756e 7473  t.summary_counts
-00016bd0: 2829 0a0a 2020 2020 2020 2020 7432 7069  ()..        t2pi
-00016be0: 766f 7420 3d20 7431 2e70 6976 6f74 2827  vot = t1.pivot('
-00016bf0: 6120 6227 290a 2020 2020 2020 2020 7432  a b').        t2
-00016c00: 7069 766f 742e 6475 6d70 2829 0a20 2020  pivot.dump().   
-00016c10: 2020 2020 2074 3270 6976 6f74 2e64 756d       t2pivot.dum
-00016c20: 705f 636f 756e 7473 2829 0a20 2020 2020  p_counts().     
-00016c30: 2020 2074 3270 6976 6f74 2e73 756d 6d61     t2pivot.summa
-00016c40: 7279 5f63 6f75 6e74 7328 290a 0a20 2020  ry_counts()..   
-00016c50: 2020 2020 2023 2054 4f44 4f20 2d20 6164       # TODO - ad
-00016c60: 6420 6173 7365 7274 730a 0a0a 636c 6173  d asserts...clas
-00016c70: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
-00016c80: 7473 2875 6e69 7474 6573 742e 5465 7374  ts(unittest.Test
-00016c90: 4361 7365 293a 0a20 2020 2072 6563 6970  Case):.    recip
-00016ca0: 655f 6461 7461 203d 2074 6578 7477 7261  e_data = textwra
-00016cb0: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-00016cc0: 2020 2020 2020 6964 2c74 6974 6c65 2c69        id,title,i
-00016cd0: 6e67 7265 6469 656e 7473 0a20 2020 2020  ngredients.     
-00016ce0: 2020 2031 2c54 756e 6120 6361 7373 6572     1,Tuna casser
-00016cf0: 6f6c 652c 2274 756e 612c 206e 6f6f 646c  ole,"tuna, noodl
-00016d00: 6573 2c20 4372 6561 6d20 6f66 204d 7573  es, Cream of Mus
-00016d10: 6872 6f6f 6d20 536f 7570 220a 2020 2020  hroom Soup".    
-00016d20: 2020 2020 322c 4861 7761 6969 616e 2070      2,Hawaiian p
-00016d30: 697a 7a61 2c70 697a 7a61 2064 6f75 6768  izza,pizza dough
-00016d40: 2070 696e 6561 7070 6c65 2068 616d 2074   pineapple ham t
-00016d50: 6f6d 6174 6f20 7361 7563 650a 2020 2020  omato sauce.    
-00016d60: 2020 2020 332c 4d61 7267 6865 7269 7461      3,Margherita
-00016d70: 2070 697a 7a61 2c70 697a 7a61 2064 6f75   pizza,pizza dou
-00016d80: 6768 2063 6865 6573 6520 7065 7374 6f20  gh cheese pesto 
-00016d90: 6172 7469 6368 6f6b 6520 6865 6172 7473  artichoke hearts
-00016da0: 0a20 2020 2020 2020 2034 2c50 6570 7065  .        4,Peppe
-00016db0: 726f 6e69 2070 697a 7a61 2c70 697a 7a61  roni pizza,pizza
-00016dc0: 2064 6f75 6768 2063 6865 6573 6520 746f   dough cheese to
-00016dd0: 6d61 746f 2073 6175 6365 2070 6570 7065  mato sauce peppe
-00016de0: 726f 6e69 0a20 2020 2020 2020 2035 2c47  roni.        5,G
-00016df0: 7269 6c6c 6564 2063 6865 6573 6520 7361  rilled cheese sa
-00016e00: 6e64 7769 6368 2c62 7265 6164 2063 6865  ndwich,bread che
-00016e10: 6573 6520 6275 7474 6572 0a20 2020 2020  ese butter.     
-00016e20: 2020 2036 2c54 756e 6120 6d65 6c74 2c74     6,Tuna melt,t
-00016e30: 756e 6120 6d61 796f 6e6e 6169 7365 2074  una mayonnaise t
-00016e40: 6f6d 6174 6f20 6272 6561 6420 6368 6565  omato bread chee
-00016e50: 7365 0a20 2020 2020 2020 2037 2c43 6869  se.        7,Chi
-00016e60: 6c69 2064 6f67 2c68 6f74 2064 6f67 2063  li dog,hot dog c
-00016e70: 6869 6c69 206f 6e69 6f6e 2062 756e 0a20  hili onion bun. 
-00016e80: 2020 2020 2020 2038 2c46 7265 6e63 6820         8,French 
-00016e90: 746f 6173 742c 6567 6720 6d69 6c6b 2076  toast,egg milk v
-00016ea0: 616e 696c 6c61 2062 7265 6164 206d 6170  anilla bread map
-00016eb0: 6c65 2073 7972 7570 0a20 2020 2020 2020  le syrup.       
-00016ec0: 2039 2c42 4c54 2c62 7265 6164 2062 6163   9,BLT,bread bac
-00016ed0: 6f6e 206c 6574 7475 6365 2074 6f6d 6174  on lettuce tomat
-00016ee0: 6f20 6d61 796f 6e6e 6169 7365 0a20 2020  o mayonnaise.   
-00016ef0: 2020 2020 2031 302c 5265 7562 656e 2073       10,Reuben s
-00016f00: 616e 6477 6963 682c 7279 6520 6272 6561  andwich,rye brea
-00016f10: 6420 7361 7565 726b 7261 7574 2063 6f72  d sauerkraut cor
-00016f20: 6e65 6420 6265 6566 2073 7769 7373 2063  ned beef swiss c
-00016f30: 6865 6573 6520 7275 7373 6961 6e20 6472  heese russian dr
-00016f40: 6573 7369 6e67 2074 686f 7573 616e 6420  essing thousand 
-00016f50: 6973 6c61 6e64 0a20 2020 2020 2020 2031  island.        1
-00016f60: 312c 4861 6d62 7572 6765 722c 6772 6f75  1,Hamburger,grou
-00016f70: 6e64 2062 6565 6620 6275 6e20 6c65 7474  nd beef bun lett
-00016f80: 7563 6520 6b65 7463 6875 7020 6d75 7374  uce ketchup must
-00016f90: 6172 6420 7069 636b 6c65 0a20 2020 2020  ard pickle.     
-00016fa0: 2020 2031 322c 4368 6565 7365 6275 7267     12,Cheeseburg
-00016fb0: 6572 2c67 726f 756e 6420 6265 6566 2062  er,ground beef b
-00016fc0: 756e 206c 6574 7475 6365 206b 6574 6368  un lettuce ketch
-00016fd0: 7570 206d 7573 7461 7264 2070 6963 6b6c  up mustard pickl
-00016fe0: 6520 6368 6565 7365 0a20 2020 2020 2020  e cheese.       
-00016ff0: 2031 332c 4261 636f 6e20 6368 6565 7365   13,Bacon cheese
-00017000: 6275 7267 6572 2c67 726f 756e 6420 6265  burger,ground be
-00017010: 6566 2062 756e 206c 6574 7475 6365 206b  ef bun lettuce k
-00017020: 6574 6368 7570 206d 7573 7461 7264 2070  etchup mustard p
-00017030: 6963 6b6c 6520 6368 6565 7365 2062 6163  ickle cheese bac
-00017040: 6f6e 0a20 2020 2020 2020 2022 2222 290a  on.        """).
-00017050: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
-00017060: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00017070: 6c66 2e72 6563 6970 6573 203d 206c 742e  lf.recipes = lt.
-00017080: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-00017090: 7274 2873 656c 662e 7265 6369 7065 5f64  rt(self.recipe_d
-000170a0: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
-000170b0: 6469 6374 2869 643d 696e 7429 290a 2020  dict(id=int)).  
-000170c0: 2020 2020 2020 7365 6c66 2e72 6563 6970        self.recip
-000170d0: 6573 2e63 7265 6174 655f 696e 6465 7828  es.create_index(
-000170e0: 2269 6422 2c20 756e 6971 7565 3d54 7275  "id", unique=Tru
-000170f0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00017100: 7265 6369 7065 732e 6372 6561 7465 5f73  recipes.create_s
-00017110: 6561 7263 685f 696e 6465 7828 2269 6e67  earch_index("ing
-00017120: 7265 6469 656e 7473 2229 0a0a 2020 2020  redients")..    
-00017130: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-00017140: 2020 2064 6566 2074 6573 745f 6163 6365     def test_acce
-00017150: 7373 5f6e 6f6e 5f65 7869 7374 656e 745f  ss_non_existent_
-00017160: 7365 6172 6368 5f61 7474 7269 6275 7465  search_attribute
-00017170: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017180: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-00017190: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
-000171a0: 722c 206d 7367 3d22 6661 696c 6564 2074  r, msg="failed t
-000171b0: 6f20 7261 6973 6520 5661 6c75 6545 7272  o raise ValueErr
-000171c0: 6f72 2077 6865 6e20 6163 6365 7373 696e  or when accessin
-000171d0: 6720 6e6f 6e2d 6578 6973 7465 6e74 2073  g non-existent s
-000171e0: 6561 7263 6820 696e 6465 7822 293a 0a20  earch index"):. 
-000171f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017200: 7265 6369 7065 732e 7365 6172 6368 2e74  recipes.search.t
-00017210: 6974 6c65 2822 7879 7a22 290a 0a20 2020  itle("xyz")..   
-00017220: 2040 616e 6e6f 756e 6365 5f74 6573 740a   @announce_test.
-00017230: 2020 2020 6465 6620 7465 7374 5f73 6561      def test_sea
-00017240: 7263 685f 6469 7228 7365 6c66 293a 0a20  rch_dir(self):. 
-00017250: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00017260: 7274 4571 7561 6c28 5b27 696e 6772 6564  rtEqual(['ingred
-00017270: 6965 6e74 7327 5d2c 2064 6972 2873 656c  ients'], dir(sel
-00017280: 662e 7265 6369 7065 732e 7365 6172 6368  f.recipes.search
-00017290: 292c 2022 6661 696c 6564 2074 6f20 6765  ), "failed to ge
-000172a0: 6e65 7261 7465 2063 6f72 7265 6374 2064  nerate correct d
-000172b0: 6972 2829 2072 6573 706f 6e73 6522 290a  ir() response").
-000172c0: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
-000172d0: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
-000172e0: 5f74 6578 745f 7365 6172 6368 2873 656c  _text_search(sel
-000172f0: 6629 3a0a 2020 2020 2020 2020 666f 7220  f):.        for 
-00017300: 7175 6572 792c 2065 7870 6563 7465 6420  query, expected 
-00017310: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
-00017320: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
-00017330: 2020 2020 2020 2028 2274 756e 6122 2c20         ("tuna", 
-00017340: 5b31 2c20 365d 292c 0a20 2020 2020 2020  [1, 6]),.       
-00017350: 2020 2020 2028 2274 756e 6120 2b63 6865       ("tuna +che
-00017360: 6573 6522 2c20 5b36 2c20 332c 2034 2c20  ese", [6, 3, 4, 
-00017370: 352c 2031 302c 2031 322c 2031 332c 2031  5, 10, 12, 13, 1
-00017380: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00017390: 2822 7069 6e65 6170 706c 6520 2b62 6163  ("pineapple +bac
-000173a0: 6f6e 206c 6574 7475 6365 2062 6565 6620  on lettuce beef 
-000173b0: 2d73 6175 6572 6b72 6175 7420 746f 6d61  -sauerkraut toma
-000173c0: 746f 222c 205b 392c 2031 332c 2032 2c20  to", [9, 13, 2, 
-000173d0: 3131 2c20 3132 2c20 342c 2036 2c20 3130  11, 12, 4, 6, 10
-000173e0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000173f0: 2822 7069 7a7a 6120 646f 7567 6820 2d70  ("pizza dough -p
-00017400: 696e 6561 7070 6c65 222c 205b 332c 2034  ineapple", [3, 4
-00017410: 2c20 325d 292c 0a20 2020 2020 2020 2020  , 2]),.         
-00017420: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
-00017430: 202d 2d70 696e 6561 7070 6c65 222c 205b   --pineapple", [
-00017440: 332c 2034 5d29 2c0a 2020 2020 2020 2020  3, 4]),.        
-00017450: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
-00017460: 6e22 2c20 5b39 2c20 352c 2036 2c20 382c  n", [9, 5, 6, 8,
-00017470: 2031 302c 2031 335d 292c 0a20 2020 2020   10, 13]),.     
-00017480: 2020 2020 2020 2028 2262 7265 6164 202b         ("bread +
-00017490: 2b62 6163 6f6e 222c 205b 392c 2031 335d  +bacon", [9, 13]
-000174a0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000174b0: 2262 7265 6164 202b 2b61 6e63 686f 7669  "bread ++anchovi
-000174c0: 6573 222c 205b 5d29 2c0a 2020 2020 2020  es", []),.      
-000174d0: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
-000174e0: 6261 636f 6e20 2b2b 616e 6368 6f76 6965  bacon ++anchovie
-000174f0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
-00017500: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
-00017510: 6f6e 202d 2d61 6e63 686f 7669 6573 222c  on --anchovies",
-00017520: 205b 392c 2035 2c20 362c 2038 2c20 3130   [9, 5, 6, 8, 10
-00017530: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
-00017540: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
-00017550: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
-00017560: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
-00017570: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-00017580: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
-00017590: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
-000175a0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-000175b0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-000175c0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-000175d0: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
-000175e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000175f0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
-00017600: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
-00017610: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
-00017620: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
-00017630: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
-00017640: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00017650: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
-00017660: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017670: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00017680: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
-00017690: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
-000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176b0: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-000176c0: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
-000176d0: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
-000176e0: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
-000176f0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
-00017700: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
-00017710: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-00017720: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
-00017730: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
-00017740: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00017750: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
-00017760: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-00017770: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
-00017780: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
-00017790: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
-000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177b0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-000177c0: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
-000177d0: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
-000177e0: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
-000177f0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
-00017800: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00017810: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
-00017820: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
-00017830: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
-00017840: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
-00017850: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
-00017860: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
-00017870: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
-00017880: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
-00017890: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000178b0: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
-000178c0: 5b7b 2774 756e 6127 2c20 2763 7265 616d  [{'tuna', 'cream
-000178d0: 272c 2027 736f 7570 272c 2027 6e6f 6f64  ', 'soup', 'nood
-000178e0: 6c65 7327 2c20 276d 7573 6872 6f6f 6d27  les', 'mushroom'
-000178f0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017910: 2020 2020 207b 2774 6f6d 6174 6f27 2c20       {'tomato', 
-00017920: 2774 756e 6127 2c20 276d 6179 6f6e 6e61  'tuna', 'mayonna
-00017930: 6973 6527 2c20 2762 7265 6164 272c 2027  ise', 'bread', '
-00017940: 6368 6565 7365 277d 5d29 2c0a 2020 2020  cheese'}]),.    
-00017950: 2020 2020 2020 2020 2020 2020 5d3a 0a20              ]:. 
-00017960: 2020 2020 2020 2020 2020 206d 6174 6368             match
-00017970: 6573 203d 2073 656c 662e 7265 6369 7065  es = self.recipe
-00017980: 732e 7365 6172 6368 2e69 6e67 7265 6469  s.search.ingredi
-00017990: 656e 7473 2871 7565 7279 2c20 6d69 6e5f  ents(query, min_
-000179a0: 7363 6f72 653d 2d31 3030 3030 2c20 6173  score=-10000, as
-000179b0: 5f74 6162 6c65 3d46 616c 7365 2c20 696e  _table=False, in
-000179c0: 636c 7564 655f 776f 7264 733d 5472 7565  clude_words=True
-000179d0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-000179e0: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-000179f0: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-00017a00: 2073 636f 7265 2c20 776f 7264 7320 696e   score, words in
-00017a10: 206d 6174 6368 6573 5d0a 2020 2020 2020   matches].      
-00017a20: 2020 2020 2020 7072 696e 7428 7265 7072        print(repr
-00017a30: 2871 7565 7279 292c 2027 2d3e 272c 205b  (query), '->', [
-00017a40: 2872 6563 6970 652e 6964 2c20 7363 6f72  (recipe.id, scor
-00017a50: 652c 2077 6f72 6473 2920 666f 7220 7265  e, words) for re
-00017a60: 6369 7065 2c20 7363 6f72 652c 2077 6f72  cipe, score, wor
-00017a70: 6473 2069 6e20 6d61 7463 6865 735d 290a  ds in matches]).
-00017a80: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00017a90: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00017aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ab0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00017ac0: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
-00017ad0: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
-00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017af0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
-00017b00: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
-00017b10: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
-00017b20: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
-00017b30: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
-00017b40: 6473 7d22 290a 2020 2020 2020 2020 2020  ds}").          
-00017b50: 2020 6d61 7463 685f 776f 7264 7320 3d20    match_words = 
-00017b60: 5b73 6574 2877 6f72 6473 2920 666f 7220  [set(words) for 
-00017b70: 7265 6369 7065 2c20 7363 6f72 652c 2077  recipe, score, w
-00017b80: 6f72 6473 2069 6e20 6d61 7463 6865 735d  ords in matches]
-00017b90: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00017ba0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00017bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017bc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00017bd0: 616c 2865 7870 6563 7465 645f 776f 7264  al(expected_word
-00017be0: 732c 206d 6174 6368 5f77 6f72 6473 2c0a  s, match_words,.
-00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c10: 2022 696e 7661 6c69 6420 6d61 7463 6820   "invalid match 
-00017c20: 776f 7264 7320 666f 7220 7175 6572 7920  words for query 
-00017c30: 7b21 727d 2c20 6578 7065 6374 6564 207b  {!r}, expected {
-00017c40: 7d2c 2067 6f74 207b 7d22 2e66 6f72 6d61  }, got {}".forma
-00017c50: 7428 7175 6572 792c 0a20 2020 2020 2020  t(query,.       
-00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cb0: 2020 2020 2020 2020 2020 2065 7870 6563             expec
-00017cc0: 7465 645f 776f 7264 732c 0a20 2020 2020  ted_words,.     
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d20: 2020 2020 2020 2020 2020 2020 206d 6174               mat
-00017d30: 6368 5f77 6f72 6473 2929 0a0a 2020 2020  ch_words))..    
-00017d40: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-00017d50: 2020 2064 6566 2074 6573 745f 7365 6172     def test_sear
-00017d60: 6368 5f77 6974 685f 6c69 6d69 7428 7365  ch_with_limit(se
-00017d70: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
-00017d80: 2071 7565 7279 2c20 6578 7065 6374 6564   query, expected
-00017d90: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-00017da0: 2020 2822 222c 205b 5d29 2c0a 2020 2020    ("", []),.    
-00017db0: 2020 2020 2020 2020 2822 7475 6e61 222c          ("tuna",
-00017dc0: 205b 312c 2036 5d29 2c0a 2020 2020 2020   [1, 6]),.      
-00017dd0: 2020 2020 2020 2822 7475 6e61 202b 6368        ("tuna +ch
-00017de0: 6565 7365 222c 205b 362c 2033 2c20 345d  eese", [6, 3, 4]
-00017df0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00017e00: 2270 696e 6561 7070 6c65 202b 6261 636f  "pineapple +baco
-00017e10: 6e20 6c65 7474 7563 6520 6265 6566 202d  n lettuce beef -
-00017e20: 7361 7565 726b 7261 7574 2074 6f6d 6174  sauerkraut tomat
-00017e30: 6f22 2c20 5b39 2c20 3133 2c20 325d 292c  o", [9, 13, 2]),
-00017e40: 0a20 2020 2020 2020 2020 2020 2028 2270  .            ("p
-00017e50: 697a 7a61 2064 6f75 6768 202d 7069 6e65  izza dough -pine
-00017e60: 6170 706c 6522 2c20 5b33 2c20 342c 2032  apple", [3, 4, 2
-00017e70: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00017e80: 2822 7069 7a7a 6120 646f 7567 6820 2d2d  ("pizza dough --
-00017e90: 7069 6e65 6170 706c 6522 2c20 5b33 2c20  pineapple", [3, 
-00017ea0: 345d 292c 0a20 2020 2020 2020 2020 2020  4]),.           
-00017eb0: 2028 2262 7265 6164 2062 6163 6f6e 222c   ("bread bacon",
-00017ec0: 205b 392c 2035 2c20 365d 292c 0a20 2020   [9, 5, 6]),.   
-00017ed0: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
-00017ee0: 202b 2b62 6163 6f6e 222c 205b 392c 2031   ++bacon", [9, 1
-00017ef0: 335d 292c 0a20 2020 2020 2020 2020 2020  3]),.           
-00017f00: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
-00017f10: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
-00017f20: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00017f30: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
-00017f40: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-00017f50: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
-00017f60: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
-00017f70: 222c 205b 392c 2035 2c20 365d 292c 0a20  ", [9, 5, 6]),. 
-00017f80: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
-00017f90: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
-00017fa0: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
-00017fb0: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
-00017fc0: 7175 6572 792c 2061 735f 7461 626c 653d  query, as_table=
-00017fd0: 4661 6c73 652c 206d 696e 5f73 636f 7265  False, min_score
-00017fe0: 3d2d 3130 3030 302c 206c 696d 6974 3d33  =-10000, limit=3
-00017ff0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-00018000: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-00018010: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-00018020: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
-00018030: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018040: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
-00018050: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
-00018060: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
-00018070: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
-00018080: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
-00018090: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000180a0: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
-000180b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000180c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000180d0: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
-000180e0: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-00018110: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
-00018120: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
-00018130: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
-00018140: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
-00018150: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
-00018160: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-00018170: 6465 6620 7465 7374 5f73 6561 7263 685f  def test_search_
-00018180: 7769 7468 5f6d 696e 5f73 636f 7265 2873  with_min_score(s
-00018190: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
-000181a0: 7220 7175 6572 792c 2065 7870 6563 7465  r query, expecte
-000181b0: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
-000181c0: 2020 2028 2222 2c20 5b5d 292c 0a20 2020     ("", []),.   
-000181d0: 2020 2020 2020 2020 2028 2274 756e 6122           ("tuna"
-000181e0: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
-000181f0: 2020 2028 2274 756e 6120 2b63 6865 6573     ("tuna +chees
-00018200: 6522 2c20 5b36 2c5d 292c 0a20 2020 2020  e", [6,]),.     
-00018210: 2020 2020 2020 2028 2270 696e 6561 7070         ("pineapp
-00018220: 6c65 202b 6261 636f 6e20 6c65 7474 7563  le +bacon lettuc
-00018230: 6520 6265 6566 202d 7361 7565 726b 7261  e beef -sauerkra
-00018240: 7574 2074 6f6d 6174 6f22 2c20 5b39 2c20  ut tomato", [9, 
-00018250: 3133 5d29 2c0a 2020 2020 2020 2020 2020  13]),.          
-00018260: 2020 2822 7069 7a7a 6120 646f 7567 6820    ("pizza dough 
-00018270: 2d70 696e 6561 7070 6c65 222c 205b 5d29  -pineapple", [])
-00018280: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00018290: 7069 7a7a 6120 646f 7567 6820 2d2d 7069  pizza dough --pi
-000182a0: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
-000182b0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-000182c0: 6164 2062 6163 6f6e 222c 205b 5d29 2c0a  ad bacon", []),.
-000182d0: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
-000182e0: 6561 6420 2b2b 6261 636f 6e22 2c20 5b39  ead ++bacon", [9
-000182f0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
-00018300: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
-00018310: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
-00018320: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00018330: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
-00018340: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-00018350: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
-00018360: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
-00018370: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
-00018380: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
-00018390: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
-000183a0: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
-000183b0: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-000183c0: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
-000183d0: 6d69 6e5f 7363 6f72 653d 3130 3030 290a  min_score=1000).
-000183e0: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-000183f0: 685f 6964 7320 3d20 5b72 6563 6970 652e  h_ids = [recipe.
-00018400: 6964 2066 6f72 2072 6563 6970 652c 205f  id for recipe, _
-00018410: 2069 6e20 6d61 7463 6865 735d 0a20 2020   in matches].   
-00018420: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
-00018430: 6570 7228 7175 6572 7929 2c20 272d 3e27  epr(query), '->'
-00018440: 2c20 5b28 7265 6369 7065 2e69 642c 2073  , [(recipe.id, s
-00018450: 636f 7265 2920 666f 7220 7265 6369 7065  core) for recipe
-00018460: 2c20 7363 6f72 6520 696e 206d 6174 6368  , score in match
-00018470: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
-00018480: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00018490: 7374 2871 7565 7279 3d71 7565 7279 293a  st(query=query):
-000184a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000184b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000184c0: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
-000184d0: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
-000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184f0: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
-00018500: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
-00018510: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
-00018520: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
-00018530: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
-00018540: 6473 7d22 290a 0a20 2020 2040 616e 6e6f  ds}")..    @anno
-00018550: 756e 6365 5f74 6573 740a 2020 2020 6465  unce_test.    de
-00018560: 6620 7465 7374 5f73 6561 7263 685f 7769  f test_search_wi
-00018570: 7468 5f61 735f 7461 626c 6528 7365 6c66  th_as_table(self
-00018580: 293a 0a20 2020 2020 2020 2066 6f72 2071  ):.        for q
-00018590: 7565 7279 2c20 6578 7065 6374 6564 2069  uery, expected i
-000185a0: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
-000185b0: 2822 222c 205b 5d29 2c0a 2020 2020 2020  ("", []),.      
-000185c0: 2020 2020 2020 2822 7475 6e61 222c 205b        ("tuna", [
-000185d0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000185e0: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
-000185f0: 205b 362c 5d29 2c0a 2020 2020 2020 2020   [6,]),.        
-00018600: 2020 2020 2822 7069 6e65 6170 706c 6520      ("pineapple 
-00018610: 2b62 6163 6f6e 206c 6574 7475 6365 2062  +bacon lettuce b
-00018620: 6565 6620 2d73 6175 6572 6b72 6175 7420  eef -sauerkraut 
-00018630: 746f 6d61 746f 222c 205b 392c 2031 335d  tomato", [9, 13]
-00018640: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00018650: 2270 697a 7a61 2064 6f75 6768 202d 7069  "pizza dough -pi
-00018660: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
-00018670: 2020 2020 2020 2020 2020 2028 2270 697a             ("piz
-00018680: 7a61 2064 6f75 6768 202d 2d70 696e 6561  za dough --pinea
-00018690: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
-000186a0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-000186b0: 6261 636f 6e22 2c20 5b5d 292c 0a20 2020  bacon", []),.   
-000186c0: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
-000186d0: 202b 2b62 6163 6f6e 222c 205b 392c 5d29   ++bacon", [9,])
-000186e0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000186f0: 6272 6561 6420 2b2b 616e 6368 6f76 6965  bread ++anchovie
-00018700: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
-00018710: 2020 2020 2028 2262 7265 6164 202b 2b62       ("bread ++b
-00018720: 6163 6f6e 202b 2b61 6e63 686f 7669 6573  acon ++anchovies
-00018730: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
-00018740: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
-00018750: 6e20 2d2d 616e 6368 6f76 6965 7322 2c20  n --anchovies", 
-00018760: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
-00018770: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-00018780: 6865 7320 3d20 7365 6c66 2e72 6563 6970  hes = self.recip
-00018790: 6573 2e73 6561 7263 682e 696e 6772 6564  es.search.ingred
-000187a0: 6965 6e74 7328 7175 6572 792c 206d 696e  ients(query, min
-000187b0: 5f73 636f 7265 3d31 3030 302c 2061 735f  _score=1000, as_
-000187c0: 7461 626c 653d 5472 7565 290a 2020 2020  table=True).    
-000187d0: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
-000187e0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
-000187f0: 6f72 2072 6563 6970 6520 696e 206d 6174  or recipe in mat
-00018800: 6368 6573 5d0a 2020 2020 2020 2020 2020  ches].          
-00018810: 2020 7072 696e 7428 7265 7072 2871 7565    print(repr(que
-00018820: 7279 292c 2027 2d3e 272c 205b 2872 6563  ry), '->', [(rec
-00018830: 6970 652e 6964 2c20 7265 6369 7065 2e69  ipe.id, recipe.i
-00018840: 6e67 7265 6469 656e 7473 5f73 6561 7263  ngredients_searc
-00018850: 685f 7363 6f72 6529 2066 6f72 2072 6563  h_score) for rec
-00018860: 6970 6520 696e 206d 6174 6368 6573 5d29  ipe in matches])
-00018870: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00018880: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
-00018890: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
-000188a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000188b0: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-000188c0: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
-000188d0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
-00018900: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
-00018910: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
-00018920: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
-00018930: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
-00018940: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00018950: 636f 7265 5f61 7474 7220 3d20 2269 6e67  core_attr = "ing
-00018960: 7265 6469 656e 7473 5f73 6561 7263 685f  redients_search_
-00018970: 7363 6f72 6522 0a20 2020 2020 2020 2020  score".         
-00018980: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00018990: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-000189a0: 2020 2020 616c 6c28 0a20 2020 2020 2020      all(.       
-000189b0: 2020 2020 2020 2020 2020 2020 2068 6173               has
-000189c0: 6174 7472 286d 6174 6368 6573 2e62 792e  attr(matches.by.
-000189d0: 6964 5b6d 6964 5d2c 2073 636f 7265 5f61  id[mid], score_a
-000189e0: 7474 7229 0a20 2020 2020 2020 2020 2020  ttr).           
-000189f0: 2020 2020 2020 2020 2066 6f72 206d 6964           for mid
-00018a00: 2069 6e20 6d61 7463 685f 6964 730a 2020   in match_ids.  
-00018a10: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-00018a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a30: 2066 2261 735f 7461 626c 6520 6469 6420   f"as_table did 
-00018a40: 6e6f 7420 706f 7075 6c61 7465 2073 6f6d  not populate som
-00018a50: 6520 7365 6172 6368 2072 6563 6f72 6473  e search records
-00018a60: 2077 6974 6820 7b73 636f 7265 5f61 7474   with {score_att
-00018a70: 7221 727d 220a 2020 2020 2020 2020 2020  r!r}".          
-00018a80: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00018a90: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-00018aa0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00018ab0: 2020 2061 6e79 280a 2020 2020 2020 2020     any(.        
-00018ac0: 2020 2020 2020 2020 2020 2020 6861 7361              hasa
-00018ad0: 7474 7228 7365 6c66 2e72 6563 6970 6573  ttr(self.recipes
-00018ae0: 2e62 792e 6964 5b6d 6964 5d2c 2073 636f  .by.id[mid], sco
-00018af0: 7265 5f61 7474 7229 0a20 2020 2020 2020  re_attr).       
-00018b00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00018b10: 206d 6964 2069 6e20 6d61 7463 685f 6964   mid in match_id
-00018b20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00018b30: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00018b40: 2020 2020 2066 2261 735f 7461 626c 6520       f"as_table 
-00018b50: 706f 7075 6c61 7465 6420 736f 6d65 206f  populated some o
-00018b60: 7269 6769 6e61 6c20 7265 636f 7264 7320  riginal records 
-00018b70: 7769 7468 207b 7363 6f72 655f 6174 7472  with {score_attr
-00018b80: 2172 7d22 0a20 2020 2020 2020 2020 2020  !r}".           
-00018b90: 2029 0a0a 636c 6173 7320 5461 626c 6553   )..class TableS
-00018ba0: 6561 7263 6854 6573 7473 5f44 6174 614f  earchTests_DataO
-00018bb0: 626a 6563 7473 2854 6162 6c65 5365 6172  bjects(TableSear
-00018bc0: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
-00018bd0: 7461 4f62 6a65 6374 7329 3a0a 2020 2020  taObjects):.    
-00018be0: 7061 7373 0a0a 636c 6173 7320 5461 626c  pass..class Tabl
-00018bf0: 6553 6561 7263 6854 6573 7473 5f4e 616d  eSearchTests_Nam
-00018c00: 6564 7475 706c 6573 2854 6162 6c65 5365  edtuples(TableSe
-00018c10: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
-00018c20: 4e61 6d65 6474 7570 6c65 7329 3a0a 2020  Namedtuples):.  
-00018c30: 2020 7061 7373 0a0a 636c 6173 7320 5461    pass..class Ta
-00018c40: 626c 6553 6561 7263 6854 6573 7473 5f44  bleSearchTests_D
-00018c50: 6174 614e 616d 6564 7475 706c 6573 2854  ataNamedtuples(T
-00018c60: 6162 6c65 5365 6172 6368 5465 7374 732c  ableSearchTests,
-00018c70: 2055 7369 6e67 4461 7461 4e61 6d65 6474   UsingDataNamedt
-00018c80: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
-00018c90: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
-00018ca0: 7263 6854 6573 7473 5f53 6c6f 7474 6564  rchTests_Slotted
-00018cb0: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
-00018cc0: 732c 2055 7369 6e67 536c 6f74 7465 644f  s, UsingSlottedO
-00018cd0: 626a 6563 7473 293a 0a20 2020 2070 6173  bjects):.    pas
-00018ce0: 730a 0a63 6c61 7373 2054 6162 6c65 5365  s..class TableSe
-00018cf0: 6172 6368 5465 7374 735f 5369 6d70 6c65  archTests_Simple
-00018d00: 4e61 6d65 7370 6163 6528 5461 626c 6553  Namespace(TableS
-00018d10: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
-00018d20: 6753 696d 706c 654e 616d 6573 7061 6365  gSimpleNamespace
-00018d30: 293a 0a20 2020 2070 6173 730a 0a69 6620  ):.    pass..if 
-00018d40: 6461 7461 636c 6173 7365 7320 6973 206e  dataclasses is n
-00018d50: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
-00018d60: 7373 2054 6162 6c65 5365 6172 6368 5465  ss TableSearchTe
-00018d70: 7374 735f 4461 7461 636c 6173 7365 7328  sts_Dataclasses(
-00018d80: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00018d90: 2c20 5573 696e 6744 6174 6163 6c61 7373  , UsingDataclass
-00018da0: 6573 293a 0a20 2020 2020 2020 2070 6173  es):.        pas
-00018db0: 730a 0a69 6620 7079 6461 6e74 6963 2069  s..if pydantic i
-00018dc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00018dd0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-00018de0: 6854 6573 7473 5f50 7964 616e 7469 634d  hTests_PydanticM
-00018df0: 6f64 656c 7328 5461 626c 6553 6561 7263  odels(TableSearc
-00018e00: 6854 6573 7473 2c20 5573 696e 6750 7964  hTests, UsingPyd
-00018e10: 616e 7469 634d 6f64 656c 293a 0a20 2020  anticModel):.   
-00018e20: 2020 2020 2070 6173 730a 0a20 2020 2063       pass..    c
-00018e30: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
-00018e40: 5465 7374 735f 5079 6461 6e74 6963 496d  Tests_PydanticIm
-00018e50: 6d75 7461 626c 654d 6f64 656c 7328 5461  mutableModels(Ta
-00018e60: 626c 6553 6561 7263 6854 6573 7473 2c20  bleSearchTests, 
-00018e70: 5573 696e 6750 7964 616e 7469 6349 6d6d  UsingPydanticImm
-00018e80: 7574 6162 6c65 4d6f 6465 6c29 3a0a 2020  utableModel):.  
-00018e90: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00018ea0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-00018eb0: 6854 6573 7473 5f50 7964 616e 7469 634f  hTests_PydanticO
-00018ec0: 524d 4d6f 6465 6c73 2854 6162 6c65 5365  RMModels(TableSe
-00018ed0: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
-00018ee0: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-00018ef0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00018f00: 0a69 6620 6174 7472 2069 7320 6e6f 7420  .if attr is not 
-00018f10: 4e6f 6e65 3a0a 2020 2020 636c 6173 7320  None:.    class 
-00018f20: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00018f30: 5f41 7474 7243 6c61 7373 6573 2854 6162  _AttrClasses(Tab
-00018f40: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
-00018f50: 7369 6e67 4174 7472 436c 6173 7329 3a0a  singAttrClass):.
-00018f60: 2020 2020 2020 2020 7061 7373 0a0a 6966          pass..if
-00018f70: 2074 7261 6974 6c65 7473 2069 7320 6e6f   traitlets is no
-00018f80: 7420 4e6f 6e65 3a0a 2020 2020 636c 6173  t None:.    clas
-00018f90: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
-00018fa0: 7473 5f54 7261 6974 6c65 7473 436c 6173  ts_TraitletsClas
-00018fb0: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
-00018fc0: 6573 7473 2c20 5573 696e 6754 7261 6974  ests, UsingTrait
-00018fd0: 6c65 7473 436c 6173 7329 3a0a 2020 2020  letsClass):.    
-00018fe0: 2020 2020 7061 7373 0a0a 6966 2053 6c6f      pass..if Slo
-00018ff0: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
-00019000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 636c  not None:.    cl
-00019010: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
-00019020: 6573 7473 5f53 6c6f 7474 6564 5769 7468  ests_SlottedWith
-00019030: 4469 6374 2854 6162 6c65 5365 6172 6368  Dict(TableSearch
-00019040: 5465 7374 732c 2055 7369 6e67 536c 6f74  Tests, UsingSlot
-00019050: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
-00019060: 7473 293a 0a20 2020 2020 2020 2070 6173  ts):.        pas
-00019070: 730a 0a0a 636c 6173 7320 496e 6974 6961  s...class Initia
-00019080: 6c54 6573 7428 756e 6974 7465 7374 2e54  lTest(unittest.T
-00019090: 6573 7443 6173 6529 3a0a 2020 2020 6672  estCase):.    fr
-000190a0: 6f6d 206c 6974 746c 6574 6162 6c65 2069  om littletable i
-000190b0: 6d70 6f72 7420 280a 2020 2020 2020 2020  mport (.        
-000190c0: 5f5f 7665 7273 696f 6e5f 5f20 6173 206c  __version__ as l
-000190d0: 6974 746c 6574 6162 6c65 5f76 6572 7369  ittletable_versi
-000190e0: 6f6e 2c0a 2020 2020 2020 2020 5f5f 7665  on,.        __ve
-000190f0: 7273 696f 6e5f 7469 6d65 5f5f 2061 7320  rsion_time__ as 
-00019100: 6c69 7474 6c65 7461 626c 655f 7665 7273  littletable_vers
-00019110: 696f 6e5f 7469 6d65 2c0a 2020 2020 2020  ion_time,.      
-00019120: 2020 5f5f 7665 7273 696f 6e5f 696e 666f    __version_info
-00019130: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
-00019140: 655f 7665 7273 696f 6e5f 696e 666f 2c0a  e_version_info,.
-00019150: 2020 2020 290a 0a20 2020 2070 7269 6e74      )..    print
-00019160: 280a 2020 2020 2020 2020 6622 4265 6769  (.        f"Begi
-00019170: 6e6e 696e 6720 7465 7374 206f 6620 6c69  nning test of li
-00019180: 7474 6c65 7461 626c 652c 2076 6572 7369  ttletable, versi
-00019190: 6f6e 207b 6c69 7474 6c65 7461 626c 655f  on {littletable_
-000191a0: 7665 7273 696f 6e7d 2c20 7b6c 6974 746c  version}, {littl
-000191b0: 6574 6162 6c65 5f76 6572 7369 6f6e 5f74  etable_version_t
-000191c0: 696d 657d 222c 0a20 2020 2029 0a20 2020  ime}",.    ).   
-000191d0: 2070 7269 6e74 286c 6974 746c 6574 6162   print(littletab
-000191e0: 6c65 5f76 6572 7369 6f6e 5f69 6e66 6f29  le_version_info)
-000191f0: 0a20 2020 2070 7269 6e74 2822 5079 7468  .    print("Pyth
-00019200: 6f6e 2076 6572 7369 6f6e 222c 2073 7973  on version", sys
-00019210: 2e76 6572 7369 6f6e 290a 2020 2020 7072  .version).    pr
-00019220: 696e 7428 290a 0a0a 636c 6173 7320 5374  int()...class St
-00019230: 6f72 6167 6549 6e64 6570 656e 6465 6e74  orageIndependent
-00019240: 5465 7374 7328 756e 6974 7465 7374 2e54  Tests(unittest.T
-00019250: 6573 7443 6173 6529 3a0a 2020 2020 4061  estCase):.    @a
-00019260: 6e6e 6f75 6e63 655f 7465 7374 0a20 2020  nnounce_test.   
-00019270: 2064 6566 2074 6573 745f 6e6f 726d 616c   def test_normal
-00019280: 697a 655f 7374 7228 7365 6c66 293a 0a20  ize_str(self):. 
-00019290: 2020 2020 2020 2066 6f72 2069 6e5f 776f         for in_wo
-000192a0: 7264 2c20 6578 7065 6374 6564 5f77 6f72  rd, expected_wor
-000192b0: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
-000192c0: 2020 2028 226e 6f63 6861 6e67 6522 2c20     ("nochange", 
-000192d0: 226e 6f63 6861 6e67 6522 292c 0a20 2020  "nochange"),.   
-000192e0: 2020 2020 2020 2020 2028 2254 6f4c 6f77           ("ToLow
-000192f0: 6572 222c 2022 746f 6c6f 7765 7222 292c  er", "tolower"),
-00019300: 0a20 2020 2020 2020 2020 2020 2028 2249  .            ("I
-00019310: 2e42 2e4d 2e22 2c20 2269 626d 2229 2c0a  .B.M.", "ibm"),.
-00019320: 2020 2020 2020 2020 2020 2020 2822 472e              ("G.
-00019330: 452e 222c 2022 6765 2229 2c0a 2020 2020  E.", "ge"),.    
-00019340: 2020 2020 2020 2020 2822 4d2e 222c 2022          ("M.", "
-00019350: 6d22 292c 0a20 2020 2020 2020 2020 2020  m"),.           
-00019360: 2028 224d 2e78 797a 222c 2022 6d22 292c   ("M.xyz", "m"),
-00019370: 0a20 2020 2020 2020 2020 2020 2028 222a  .            ("*
-00019380: 7878 782d 6868 6822 2c20 2278 7878 2d68  xxx-hhh", "xxx-h
-00019390: 6868 2229 2c0a 2020 2020 2020 2020 2020  hh"),.          
-000193a0: 2020 2822 2b62 6c61 6846 6f6f 222c 2022    ("+blahFoo", "
-000193b0: 626c 6168 666f 6f22 292c 0a20 2020 2020  blahfoo"),.     
-000193c0: 2020 2020 2020 2023 2028 2266 6f78 6573         # ("foxes
-000193d0: 222c 2022 666f 7822 292c 0a20 2020 2020  ", "fox"),.     
-000193e0: 2020 2020 2020 2023 2028 2263 6875 7263         # ("churc
-000193f0: 6865 7322 2c20 2263 6875 7263 6822 292c  hes", "church"),
-00019400: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
-00019410: 2264 7265 7373 6573 222c 2022 6472 6573  "dresses", "dres
-00019420: 7322 292c 0a20 2020 2020 2020 205d 3a0a  s"),.        ]:.
-00019430: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00019440: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
-00019450: 5f77 6f72 6429 3a0a 2020 2020 2020 2020  _word):.        
-00019460: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00019470: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
-00019480: 645f 776f 7264 2c20 6c74 2e54 6162 6c65  d_word, lt.Table
-00019490: 2e5f 6e6f 726d 616c 697a 655f 776f 7264  ._normalize_word
-000194a0: 2869 6e5f 776f 7264 2929 0a0a 2020 2020  (in_word))..    
-000194b0: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
-000194c0: 7a65 5f73 7472 5f67 656e 2873 656c 6629  ze_str_gen(self)
-000194d0: 3a0a 2020 2020 2020 2020 666f 7220 696e  :.        for in
-000194e0: 5f77 6f72 642c 2065 7870 6563 7465 645f  _word, expected_
-000194f0: 776f 7264 7320 696e 205b 0a20 2020 2020  words in [.     
-00019500: 2020 2020 2020 2028 226e 6f63 6861 6e67         ("nochang
-00019510: 6522 2c20 5b22 6e6f 6368 616e 6765 225d  e", ["nochange"]
-00019520: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00019530: 2254 6f4c 6f77 6572 222c 205b 2274 6f6c  "ToLower", ["tol
-00019540: 6f77 6572 225d 292c 0a20 2020 2020 2020  ower"]),.       
-00019550: 2020 2020 2028 2249 2e42 2e4d 2e22 2c20       ("I.B.M.", 
-00019560: 5b22 692e 622e 6d2e 222c 2022 6962 6d22  ["i.b.m.", "ibm"
-00019570: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019580: 2822 472e 452e 222c 205b 2267 2e65 2e22  ("G.E.", ["g.e."
-00019590: 2c20 2267 6522 5d29 2c0a 2020 2020 2020  , "ge"]),.      
-000195a0: 2020 2020 2020 2822 412e 492e 222c 205b        ("A.I.", [
-000195b0: 2261 2e69 2e22 2c20 2261 6922 5d29 2c0a  "a.i.", "ai"]),.
-000195c0: 2020 2020 2020 2020 2020 2020 2822 4149              ("AI
-000195d0: 222c 205b 2261 6922 5d29 2c0a 2020 2020  ", ["ai"]),.    
-000195e0: 2020 2020 2020 2020 2822 4d2e 222c 205b          ("M.", [
-000195f0: 226d 222c 2022 6d2e 225d 292c 0a20 2020  "m", "m."]),.   
-00019600: 2020 2020 2020 2020 2028 226d 2e78 797a           ("m.xyz
-00019610: 222c 205b 226d 222c 2022 6d2e 7879 7a22  ", ["m", "m.xyz"
-00019620: 2c20 2278 797a 225d 292c 0a20 2020 2020  , "xyz"]),.     
-00019630: 2020 2020 2020 2028 224d 2e78 797a 222c         ("M.xyz",
-00019640: 205b 226d 2e78 797a 222c 2022 7879 7a22   ["m.xyz", "xyz"
-00019650: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019660: 2822 5468 7265 6164 696e 672e 6973 416c  ("Threading.isAl
-00019670: 6976 6528 2922 2c20 5b27 6973 616c 6976  ive()", ['isaliv
-00019680: 6527 2c20 2774 6872 6561 6469 6e67 272c  e', 'threading',
-00019690: 2027 7468 7265 6164 696e 672e 6973 616c   'threading.isal
-000196a0: 6976 6527 5d29 2c0a 2020 2020 2020 2020  ive']),.        
-000196b0: 2020 2020 2822 2a78 7878 2d68 6868 222c      ("*xxx-hhh",
-000196c0: 205b 2768 6868 272c 2027 7878 7827 2c20   ['hhh', 'xxx', 
-000196d0: 2778 7878 2d68 6868 275d 292c 0a20 2020  'xxx-hhh']),.   
-000196e0: 2020 2020 2020 2020 2028 222b 626c 6168           ("+blah
-000196f0: 466f 6f22 2c20 5b22 626c 6168 666f 6f22  Foo", ["blahfoo"
-00019700: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019710: 2822 7374 722e 6c73 7472 6970 222c 205b  ("str.lstrip", [
-00019720: 226c 7374 7269 7022 2c20 2273 7472 222c  "lstrip", "str",
-00019730: 2022 7374 722e 6c73 7472 6970 225d 292c   "str.lstrip"]),
-00019740: 0a20 2020 2020 2020 2020 2020 2028 2273  .            ("s
-00019750: 7472 2e6c 7374 7269 7028 2922 2c20 5b22  tr.lstrip()", ["
-00019760: 6c73 7472 6970 222c 2022 7374 7222 2c20  lstrip", "str", 
-00019770: 2273 7472 2e6c 7374 7269 7022 5d29 2c0a  "str.lstrip"]),.
-00019780: 2020 2020 2020 2020 2020 2020 2822 7365              ("se
-00019790: 6c66 2e61 7373 6572 7445 7175 616c 7322  lf.assertEquals"
-000197a0: 2c20 5b22 6173 7365 7274 6571 7561 6c73  , ["assertequals
-000197b0: 222c 2022 7365 6c66 222c 2022 7365 6c66  ", "self", "self
-000197c0: 2e61 7373 6572 7465 7175 616c 7322 5d29  .assertequals"])
-000197d0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000197e0: 5465 7374 4361 7365 2e61 7373 6572 7445  TestCase.assertE
-000197f0: 7175 616c 7322 2c20 5b22 6173 7365 7274  quals", ["assert
-00019800: 6571 7561 6c73 222c 2022 7465 7374 6361  equals", "testca
-00019810: 7365 222c 2022 7465 7374 6361 7365 2e61  se", "testcase.a
-00019820: 7373 6572 7465 7175 616c 7322 5d29 2c0a  ssertequals"]),.
-00019830: 2020 2020 2020 2020 2020 2020 2822 756e              ("un
-00019840: 6974 7465 7374 2e54 6573 7443 6173 652e  ittest.TestCase.
-00019850: 6173 7365 7274 4571 7561 6c73 222c 0a20  assertEquals",. 
-00019860: 2020 2020 2020 2020 2020 2020 5b22 6173              ["as
-00019870: 7365 7274 6571 7561 6c73 222c 2022 7465  sertequals", "te
-00019880: 7374 6361 7365 222c 2022 756e 6974 7465  stcase", "unitte
-00019890: 7374 222c 2022 756e 6974 7465 7374 2e74  st", "unittest.t
-000198a0: 6573 7463 6173 652e 6173 7365 7274 6571  estcase.asserteq
-000198b0: 7561 6c73 225d 292c 0a20 2020 2020 2020  uals"]),.       
-000198c0: 2020 2020 2028 2266 6f78 6573 222c 205b       ("foxes", [
-000198d0: 2266 6f78 222c 2022 666f 7865 7322 5d29  "fox", "foxes"])
-000198e0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000198f0: 6368 7572 6368 6573 222c 205b 2263 6875  churches", ["chu
-00019900: 7263 6822 2c20 2263 6875 7263 6865 7322  rch", "churches"
-00019910: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019920: 2822 6472 6573 7365 7322 2c20 5b22 6472  ("dresses", ["dr
-00019930: 6573 7322 2c20 2264 7265 7373 6573 225d  ess", "dresses"]
-00019940: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00019950: 2264 7265 7373 222c 205b 2264 7265 7373  "dress", ["dress
-00019960: 222c 205d 292c 0a20 2020 2020 2020 2020  ", ]),.         
-00019970: 2020 2028 2262 6961 7322 2c20 5b22 6269     ("bias", ["bi
-00019980: 6173 222c 205d 292c 0a20 2020 2020 2020  as", ]),.       
-00019990: 2020 2020 2028 2274 6f79 7322 2c20 5b22       ("toys", ["
-000199a0: 746f 7922 2c20 2274 6f79 7322 5d29 2c0a  toy", "toys"]),.
-000199b0: 2020 2020 2020 2020 2020 2020 2822 6261              ("ba
-000199c0: 6269 6573 222c 205b 2262 6162 6965 7322  bies", ["babies"
-000199d0: 2c20 2262 6162 7922 5d29 2c0a 2020 2020  , "baby"]),.    
-000199e0: 2020 2020 2020 2020 2822 6164 6465 6e64          ("addend
-000199f0: 6122 2c20 5b22 6164 6465 6e64 6122 2c20  a", ["addenda", 
-00019a00: 2261 6464 656e 6475 6d22 5d29 2c0a 2020  "addendum"]),.  
-00019a10: 2020 2020 2020 2020 2020 2822 7261 6269            ("rabi
-00019a20: 6573 222c 205b 2272 6162 6965 7322 5d29  es", ["rabies"])
-00019a30: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00019a40: 6c61 7a69 6e65 7373 222c 205b 226c 617a  laziness", ["laz
-00019a50: 696e 6573 7322 5d29 2c0a 2020 2020 2020  iness"]),.      
-00019a60: 2020 2020 2020 2822 7068 7973 6963 7322        ("physics"
-00019a70: 2c20 5b22 7068 7973 6963 7322 5d29 2c0a  , ["physics"]),.
-00019a80: 2020 2020 2020 2020 2020 2020 2822 5079              ("Py
-00019a90: 7468 6f6e 2773 222c 205b 2270 7974 686f  thon's", ["pytho
-00019aa0: 6e22 5d29 2c0a 2020 2020 2020 2020 5d3a  n"]),.        ]:
-00019ab0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00019ac0: 6820 7365 6c66 2e73 7562 5465 7374 2869  h self.subTest(i
-00019ad0: 6e5f 776f 7264 293a 0a20 2020 2020 2020  n_word):.       
-00019ae0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00019af0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-00019b00: 6564 5f77 6f72 6473 2c0a 2020 2020 2020  ed_words,.      
-00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b20: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00019b30: 6428 6c69 7374 286c 742e 5461 626c 652e  d(list(lt.Table.
-00019b40: 5f6e 6f72 6d61 6c69 7a65 5f77 6f72 645f  _normalize_word_
-00019b50: 6765 6e28 696e 5f77 6f72 6429 2929 290a  gen(in_word)))).
-00019b60: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
-00019b70: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
-00019b80: 5f6e 6f72 6d61 6c69 7a65 5f73 706c 6974  _normalize_split
-00019b90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00019ba0: 666f 7220 696e 5f73 7472 2c20 6578 7065  for in_str, expe
-00019bb0: 6374 6564 5f73 7472 5f73 6574 2069 6e20  cted_str_set in 
-00019bc0: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
-00019bd0: 7374 722e 6c73 7472 6970 2829 222c 205b  str.lstrip()", [
-00019be0: 226c 7374 7269 7022 2c20 2273 7472 222c  "lstrip", "str",
-00019bf0: 2022 7374 722e 6c73 7472 6970 225d 292c   "str.lstrip"]),
-00019c00: 0a20 2020 2020 2020 2020 2020 2028 2273  .            ("s
-00019c10: 7472 2e6c 7374 7269 7028 2920 7374 722e  tr.lstrip() str.
-00019c20: 7273 7472 6970 2829 222c 205b 226c 7374  rstrip()", ["lst
-00019c30: 7269 7022 2c20 2272 7374 7269 7022 2c20  rip", "rstrip", 
-00019c40: 2273 7472 222c 2022 7374 722e 6c73 7472  "str", "str.lstr
-00019c50: 6970 222c 2022 7374 722e 7273 7472 6970  ip", "str.rstrip
-00019c60: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-00019c70: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
-00019c80: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
-00019c90: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-00019ca0: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
-00019cb0: 2020 2020 205d 3a0a 2020 2020 2020 2020       ]:.        
-00019cc0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00019cd0: 6254 6573 7428 696e 5f73 7472 293a 0a20  bTest(in_str):. 
-00019ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019cf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00019d00: 6578 7065 6374 6564 5f73 7472 5f73 6574  expected_str_set
-00019d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d30: 2020 2073 6f72 7465 6428 7365 7428 6c74     sorted(set(lt
-00019d40: 2e54 6162 6c65 2e5f 6e6f 726d 616c 697a  .Table._normaliz
-00019d50: 655f 7370 6c69 7428 696e 5f73 7472 2929  e_split(in_str))
-00019d60: 2929 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ))...if __name__
-00019d70: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0a   == '__main__':.
-00019d80: 0a20 2020 2075 6e69 7474 6573 742e 6d61  .    unittest.ma
-00019d90: 696e 2829 0a                             in().
+00014e40: 7274 4571 7561 6c28 7431 5f64 6174 616f  rtEqual(t1_datao
+00014e50: 626a 2c20 6c74 2e44 6174 614f 626a 6563  bj, lt.DataObjec
+00014e60: 7428 2a2a 6a73 6f6e 5f64 6963 7429 290a  t(**json_dict)).
+00014e70: 0a20 2020 2064 6566 2074 6573 745f 6a73  .    def test_js
+00014e80: 6f6e 5f65 7870 6f72 745f 6e6f 6e73 7472  on_export_nonstr
+00014e90: 6561 6d69 6e67 2873 656c 6629 3a0a 2020  eaming(self):.  
+00014ea0: 2020 2020 2020 6672 6f6d 2069 7465 7274        from itert
+00014eb0: 6f6f 6c73 2069 6d70 6f72 7420 7065 726d  ools import perm
+00014ec0: 7574 6174 696f 6e73 0a20 2020 2020 2020  utations.       
+00014ed0: 2069 6d70 6f72 7420 6a73 6f6e 0a20 2020   import json.   
+00014ee0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+00014ef0: 2033 0a20 2020 2020 2020 2074 3120 3d20   3.        t1 = 
+00014f00: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+00014f10: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+00014f20: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+00014f30: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
+00014f40: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
+00014f50: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
+00014f60: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
+00014f70: 2020 206f 7574 5f73 7472 696e 6720 3d20     out_string = 
+00014f80: 7431 2e6a 736f 6e5f 6578 706f 7274 284e  t1.json_export(N
+00014f90: 6f6e 652c 2066 6965 6c64 6e61 6d65 733d  one, fieldnames=
+00014fa0: 6669 656c 646e 616d 6573 2c20 7374 7265  fieldnames, stre
+00014fb0: 616d 696e 673d 4661 6c73 6529 0a20 2020  aming=False).   
+00014fc0: 2020 2020 2020 2020 206f 6273 6572 7665           observe
+00014fd0: 645f 6a73 6f6e 203d 206a 736f 6e2e 6c6f  d_json = json.lo
+00014fe0: 6164 7328 6f75 745f 7374 7269 6e67 290a  ads(out_string).
+00014ff0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00015000: 6820 7365 6c66 2e73 7562 5465 7374 2866  h self.subTest(f
+00015010: 6965 6c64 6e61 6d65 733d 6669 656c 646e  ieldnames=fieldn
+00015020: 616d 6573 293a 0a20 2020 2020 2020 2020  ames):.         
+00015030: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00015040: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+00015050: 652a 2a33 2c20 6c65 6e28 6f62 7365 7276  e**3, len(observ
+00015060: 6564 5f6a 736f 6e29 290a 0a20 2020 2020  ed_json))..     
+00015070: 2020 2020 2020 2066 6f72 206f 622c 206a         for ob, j
+00015080: 736f 6e5f 6469 6374 2069 6e20 7a69 7028  son_dict in zip(
+00015090: 7431 2c20 6f62 7365 7276 6564 5f6a 736f  t1, observed_jso
+000150a0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+000150b0: 2020 2020 7431 5f64 6174 616f 626a 203d      t1_dataobj =
+000150c0: 206d 616b 655f 6461 7461 6f62 6a65 6374   make_dataobject
+000150d0: 5f66 726f 6d5f 6f62 286f 6229 0a20 2020  _from_ob(ob).   
+000150e0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+000150f0: 6820 7365 6c66 2e73 7562 5465 7374 286f  h self.subTest(o
+00015100: 623d 6f62 2c20 6a73 6f6e 5f64 6963 743d  b=ob, json_dict=
+00015110: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
+00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015130: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00015140: 2874 315f 6461 7461 6f62 6a2c 206c 742e  (t1_dataobj, lt.
+00015150: 4461 7461 4f62 6a65 6374 282a 2a6a 736f  DataObject(**jso
+00015160: 6e5f 6469 6374 2929 0a0a 2020 2020 6465  n_dict))..    de
+00015170: 6620 7465 7374 5f6a 736f 6e5f 696d 706f  f test_json_impo
+00015180: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+00015190: 2020 6461 7461 203d 206a 736f 6e5f 6461    data = json_da
+000151a0: 7461 0a20 2020 2020 2020 2069 6e6a 736f  ta.        injso
+000151b0: 6e20 3d20 696f 2e53 7472 696e 6749 4f28  n = io.StringIO(
+000151c0: 6461 7461 290a 2020 2020 2020 2020 6a73  data).        js
+000151d0: 6f6e 7461 626c 6520 3d20 6c74 2e54 6162  ontable = lt.Tab
+000151e0: 6c65 2829 2e6a 736f 6e5f 696d 706f 7274  le().json_import
+000151f0: 2869 6e6a 736f 6e2c 2073 7472 6561 6d69  (injson, streami
+00015200: 6e67 3d54 7275 652c 2074 7261 6e73 666f  ng=True, transfo
+00015210: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
+00015220: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
+00015230: 747d 290a 0a20 2020 2020 2020 2074 6573  t})..        tes
+00015240: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
+00015250: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+00015260: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+00015270: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+00015280: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
+00015290: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000152a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000152b0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000152c0: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
+000152d0: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
+000152e0: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
+000152f0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
+00015300: 7a69 7028 7431 2c20 6a73 6f6e 7461 626c  zip(t1, jsontabl
+00015310: 6529 2929 0a20 2020 2020 2020 2077 6974  e))).        wit
+00015320: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00015330: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015340: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00015350: 656e 285b 6420 666f 7220 6420 696e 2064  en([d for d in d
+00015360: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+00015370: 2069 6620 642e 7374 7269 7028 295d 292c   if d.strip()]),
+00015380: 206c 656e 286a 736f 6e74 6162 6c65 2929   len(jsontable))
+00015390: 0a0a 2020 2020 6465 6620 7465 7374 5f6a  ..    def test_j
+000153a0: 736f 6e5f 7374 7269 6e67 5f69 6d70 6f72  son_string_impor
+000153b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+000153c0: 2064 6174 6120 3d20 6a73 6f6e 5f64 6174   data = json_dat
+000153d0: 610a 2020 2020 2020 2020 6a73 6f6e 7461  a.        jsonta
+000153e0: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+000153f0: 2e6a 736f 6e5f 696d 706f 7274 2864 6174  .json_import(dat
+00015400: 612c 2073 7472 6561 6d69 6e67 3d54 7275  a, streaming=Tru
+00015410: 652c 2074 7261 6e73 666f 726d 733d 7b27  e, transforms={'
+00015420: 6127 3a20 696e 742c 2027 6227 3a20 696e  a': int, 'b': in
+00015430: 742c 2027 6327 3a20 696e 747d 290a 0a20  t, 'c': int}).. 
+00015440: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00015450: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
+00015460: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00015470: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00015480: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00015490: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
+000154a0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+000154b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000154c0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+000154d0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
+000154e0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
+000154f0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
+00015500: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
+00015510: 2c20 6a73 6f6e 7461 626c 6529 2929 0a20  , jsontable))). 
+00015520: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00015530: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00015540: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00015550: 6572 7445 7175 616c 286c 656e 285b 6420  ertEqual(len([d 
+00015560: 666f 7220 6420 696e 2064 6174 612e 7370  for d in data.sp
+00015570: 6c69 746c 696e 6573 2829 2069 6620 642e  litlines() if d.
+00015580: 7374 7269 7028 295d 292c 206c 656e 286a  strip()]), len(j
+00015590: 736f 6e74 6162 6c65 2929 0a0a 2020 2020  sontable))..    
+000155a0: 6465 6620 7465 7374 5f6a 736f 6e5f 7374  def test_json_st
+000155b0: 7269 6e67 5f6c 6973 745f 696d 706f 7274  ring_list_import
+000155c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000155d0: 6461 7461 203d 206a 736f 6e5f 6461 7461  data = json_data
+000155e0: 0a20 2020 2020 2020 206a 736f 6e74 6162  .        jsontab
+000155f0: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
+00015600: 6a73 6f6e 5f69 6d70 6f72 7428 6461 7461  json_import(data
+00015610: 2e73 706c 6974 6c69 6e65 7328 292c 2073  .splitlines(), s
+00015620: 7472 6561 6d69 6e67 3d54 7275 652c 2074  treaming=True, t
+00015630: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
+00015640: 696e 742c 2027 6227 3a20 696e 742c 2027  int, 'b': int, '
+00015650: 6327 3a20 696e 747d 290a 0a20 2020 2020  c': int})..     
+00015660: 2020 2074 6573 745f 7369 7a65 203d 2033     test_size = 3
+00015670: 0a20 2020 2020 2020 2074 3120 3d20 6d61  .        t1 = ma
+00015680: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+00015690: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000156a0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+000156b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+000156c0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+000156d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000156e0: 7373 6572 7454 7275 6528 616c 6c28 6d61  ssertTrue(all(ma
+000156f0: 6b65 5f64 6174 616f 626a 6563 745f 6672  ke_dataobject_fr
+00015700: 6f6d 5f6f 6228 7265 6331 2920 3d3d 2072  om_ob(rec1) == r
+00015710: 6563 3220 666f 7220 7265 6331 2c20 7265  ec2 for rec1, re
+00015720: 6332 2069 6e20 7a69 7028 7431 2c20 6a73  c2 in zip(t1, js
+00015730: 6f6e 7461 626c 6529 2929 0a20 2020 2020  ontable))).     
+00015740: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00015750: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00015760: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00015770: 7175 616c 286c 656e 285b 6420 666f 7220  qual(len([d for 
+00015780: 6420 696e 2064 6174 612e 7370 6c69 746c  d in data.splitl
+00015790: 696e 6573 2829 2069 6620 642e 7374 7269  ines() if d.stri
+000157a0: 7028 295d 292c 206c 656e 286a 736f 6e74  p()]), len(jsont
+000157b0: 6162 6c65 2929 0a0a 2020 2020 6465 6620  able))..    def 
+000157c0: 7465 7374 5f6a 736f 6e5f 6e6f 6e73 7472  test_json_nonstr
+000157d0: 6561 6d69 6e67 5f77 6974 685f 7061 7468  eaming_with_path
+000157e0: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+000157f0: 2020 2020 2020 2064 6174 6120 3d20 6a73         data = js
+00015800: 6f6e 5f64 6174 610a 2020 2020 2020 2020  on_data.        
+00015810: 6461 7461 203d 2027 2c5c 6e27 2e6a 6f69  data = ',\n'.joi
+00015820: 6e28 6461 7461 2e72 7374 7269 7028 292e  n(data.rstrip().
+00015830: 7370 6c69 746c 696e 6573 2829 290a 2020  splitlines()).  
+00015840: 2020 2020 2020 6a73 6f6e 5f69 6e70 7574        json_input
+00015850: 3020 3d20 275b 2720 2b20 6461 7461 202b  0 = '[' + data +
+00015860: 2027 5d27 0a20 2020 2020 2020 206a 736f   ']'.        jso
+00015870: 6e5f 696e 7075 7431 203d 2027 7b20 2264  n_input1 = '{ "d
+00015880: 6174 6122 3a20 5b27 202b 2064 6174 6120  ata": [' + data 
+00015890: 2b20 275d 7d27 0a20 2020 2020 2020 206a  + ']}'.        j
+000158a0: 736f 6e5f 696e 7075 7432 203d 2027 7b20  son_input2 = '{ 
+000158b0: 2264 6174 6122 3a20 7b20 2269 7465 6d73  "data": { "items
+000158c0: 223a 205b 2720 2b20 6461 7461 202b 2027  ": [' + data + '
+000158d0: 5d7d 7d27 0a0a 2020 2020 2020 2020 666f  ]}}'..        fo
+000158e0: 7220 6a73 6f6e 5f69 6e70 7574 2c20 7061  r json_input, pa
+000158f0: 7468 2069 6e20 5b0a 2020 2020 2020 2020  th in [.        
+00015900: 2020 2020 286a 736f 6e5f 696e 7075 7430      (json_input0
+00015910: 2c20 2222 292c 0a20 2020 2020 2020 2020  , ""),.         
+00015920: 2020 2028 6a73 6f6e 5f69 6e70 7574 312c     (json_input1,
+00015930: 2022 6461 7461 2229 2c0a 2020 2020 2020   "data"),.      
+00015940: 2020 2020 2020 286a 736f 6e5f 696e 7075        (json_inpu
+00015950: 7432 2c20 2264 6174 612e 6974 656d 7322  t2, "data.items"
+00015960: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
+00015970: 2020 2020 2020 2020 2020 6a73 6f6e 7461            jsonta
+00015980: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+00015990: 2e6a 736f 6e5f 696d 706f 7274 286a 736f  .json_import(jso
+000159a0: 6e5f 696e 7075 742c 0a20 2020 2020 2020  n_input,.       
+000159b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159d0: 2020 2020 2020 2020 7061 7468 3d70 6174          path=pat
+000159e0: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a10: 2020 7472 616e 7366 6f72 6d73 3d7b 2761    transforms={'a
+00015a20: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
+00015a30: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
+00015a40: 2020 2020 2020 2020 2020 7465 7374 5f73            test_s
+00015a50: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+00015a60: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
+00015a70: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+00015a80: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00015a90: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+00015aa0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00015ab0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00015ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ad0: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
+00015ae0: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
+00015af0: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
+00015b00: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
+00015b10: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
+00015b20: 206a 736f 6e74 6162 6c65 2929 290a 2020   jsontable))).  
+00015b30: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00015b40: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00015b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015b60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00015b70: 6c65 6e28 5b64 2066 6f72 2064 2069 6e20  len([d for d in 
+00015b80: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
+00015b90: 2920 6966 2064 2e73 7472 6970 2829 5d29  ) if d.strip()])
+00015ba0: 2c20 6c65 6e28 6a73 6f6e 7461 626c 6529  , len(jsontable)
+00015bb0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00015bc0: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
+00015bd0: 5f63 7573 746f 6d5f 656e 636f 6465 7228  _custom_encoder(
+00015be0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+00015bf0: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
+00015c00: 6f72 7420 6461 7465 0a20 2020 2020 2020  ort date.       
+00015c10: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+00015c20: 2020 2020 2020 7b27 6127 3a20 3130 302c        {'a': 100,
+00015c30: 2027 6227 3a20 6461 7465 2832 3030 302c   'b': date(2000,
+00015c40: 2031 2c20 3129 2c20 2763 273a 2032 3030   1, 1), 'c': 200
+00015c50: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
+00015c60: 2761 273a 2031 3031 2c20 2762 273a 2064  'a': 101, 'b': d
+00015c70: 6174 6528 3230 3031 2c20 312c 2031 292c  ate(2001, 1, 1),
+00015c80: 2027 6327 3a20 3230 317d 2c0a 2020 2020   'c': 201},.    
+00015c90: 2020 2020 5d0a 2020 2020 2020 2020 7462      ].        tb
+00015ca0: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e69  l = lt.Table().i
+00015cb0: 6e73 6572 745f 6d61 6e79 2864 6174 6129  nsert_many(data)
+00015cc0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00015cd0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+00015ce0: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
+00015cf0: 2020 2020 2020 2020 7820 3d20 7462 6c2e          x = tbl.
+00015d00: 6a73 6f6e 5f65 7870 6f72 7428 290a 0a20  json_export().. 
+00015d10: 2020 2020 2020 2063 6c61 7373 204a 736f         class Jso
+00015d20: 6e44 6174 6545 6e63 6f64 6572 286a 736f  nDateEncoder(jso
+00015d30: 6e2e 4a53 4f4e 456e 636f 6465 7229 3a0a  n.JSONEncoder):.
+00015d40: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00015d50: 6465 6661 756c 7428 7365 6c66 2c20 6f29  default(self, o)
+00015d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015d70: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
+00015d80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015d90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00015da0: 6f2c 2064 6174 6574 696d 652e 6461 7465  o, datetime.date
+00015db0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015dc0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00015dd0: 7228 6f29 0a20 2020 2020 2020 2020 2020  r(o).           
+00015de0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00015df0: 7228 292e 6465 6661 756c 7428 6f29 0a0a  r().default(o)..
+00015e00: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00015e10: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+00015e20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+00015e30: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00015e40: 2020 7b22 6122 3a20 3130 302c 2022 6222    {"a": 100, "b"
+00015e50: 3a20 2232 3030 302d 3031 2d30 3122 2c20  : "2000-01-01", 
+00015e60: 2263 223a 2032 3030 7d2c 0a20 2020 2020  "c": 200},.     
+00015e70: 2020 2020 2020 207b 2261 223a 2031 3031         {"a": 101
+00015e80: 2c20 2262 223a 2022 3230 3031 2d30 312d  , "b": "2001-01-
+00015e90: 3031 222c 2022 6322 3a20 3230 317d 0a20  01", "c": 201}. 
+00015ea0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00015eb0: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
+00015ec0: 2020 2020 2020 6a73 6f6e 5f72 6573 756c        json_resul
+00015ed0: 7420 3d20 7462 6c2e 6a73 6f6e 5f65 7870  t = tbl.json_exp
+00015ee0: 6f72 7428 6a73 6f6e 5f65 6e63 6f64 6572  ort(json_encoder
+00015ef0: 3d4a 736f 6e44 6174 6545 6e63 6f64 6572  =JsonDateEncoder
+00015f00: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00015f10: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+00015f20: 7465 642c 206a 736f 6e5f 7265 7375 6c74  ted, json_result
+00015f30: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00015f40: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
+00015f50: 5f6d 756c 7469 706c 655f 6375 7374 6f6d  _multiple_custom
+00015f60: 5f65 6e63 6f64 6572 7328 7365 6c66 293a  _encoders(self):
+00015f70: 0a20 2020 2020 2020 2066 726f 6d20 6461  .        from da
+00015f80: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
+00015f90: 7465 0a0a 2020 2020 2020 2020 636c 6173  te..        clas
+00015fa0: 7320 4141 413a 0a20 2020 2020 2020 2020  s AAA:.         
+00015fb0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00015fc0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
+00015fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015fe0: 662e 6e61 6d65 203d 206e 616d 650a 0a20  f.name = name.. 
+00015ff0: 2020 2020 2020 2064 6174 6120 3d20 5b0a         data = [.
+00016000: 2020 2020 2020 2020 2020 2020 7b27 6127              {'a'
+00016010: 3a20 3130 302c 2027 6227 3a20 6461 7465  : 100, 'b': date
+00016020: 2832 3030 302c 2031 2c20 3129 2c20 2763  (2000, 1, 1), 'c
+00016030: 273a 2032 3030 2c20 2764 273a 2041 4141  ': 200, 'd': AAA
+00016040: 2822 416c 6963 6522 297d 2c0a 2020 2020  ("Alice")},.    
+00016050: 2020 2020 2020 2020 7b27 6127 3a20 3130          {'a': 10
+00016060: 312c 2027 6227 3a20 6461 7465 2832 3030  1, 'b': date(200
+00016070: 312c 2031 2c20 3129 2c20 2763 273a 2032  1, 1, 1), 'c': 2
+00016080: 3031 2c20 2764 273a 2041 4141 2822 426f  01, 'd': AAA("Bo
+00016090: 6222 297d 2c0a 2020 2020 2020 2020 5d0a  b")},.        ].
+000160a0: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
+000160b0: 2e54 6162 6c65 2829 2e69 6e73 6572 745f  .Table().insert_
+000160c0: 6d61 6e79 2864 6174 6129 0a20 2020 2020  many(data).     
+000160d0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+000160e0: 6572 7452 6169 7365 7328 5479 7065 4572  ertRaises(TypeEr
+000160f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00016100: 2020 7820 3d20 7462 6c2e 6a73 6f6e 5f65    x = tbl.json_e
+00016110: 7870 6f72 7428 290a 0a20 2020 2020 2020  xport()..       
+00016120: 2063 6c61 7373 204a 736f 6e44 6174 6545   class JsonDateE
+00016130: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
+00016140: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
+00016150: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
+00016160: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
+00016170: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+00016180: 7274 2064 6174 6574 696d 650a 2020 2020  rt datetime.    
+00016190: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000161a0: 7369 6e73 7461 6e63 6528 6f2c 2064 6174  sinstance(o, dat
+000161b0: 6574 696d 652e 6461 7465 293a 0a20 2020  etime.date):.   
+000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161d0: 2072 6574 7572 6e20 7374 7228 6f29 0a20   return str(o). 
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000161f0: 6574 7572 6e20 7375 7065 7228 292e 6465  eturn super().de
+00016200: 6661 756c 7428 6f29 0a0a 2020 2020 2020  fault(o)..      
+00016210: 2020 636c 6173 7320 4a73 6f6e 4141 4145    class JsonAAAE
+00016220: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
+00016230: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
+00016240: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
+00016250: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
+00016260: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00016270: 7369 6e73 7461 6e63 6528 6f2c 2041 4141  sinstance(o, AAA
+00016280: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00016290: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+000162a0: 4141 4128 6e61 6d65 3d7b 6f2e 6e61 6d65  AAA(name={o.name
+000162b0: 2172 7d29 220a 0a20 2020 2020 2020 2065  !r})"..        e
+000162c0: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
+000162d0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+000162e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+000162f0: 2020 2020 2020 2020 207b 2261 223a 2031           {"a": 1
+00016300: 3030 2c20 2262 223a 2022 3230 3030 2d30  00, "b": "2000-0
+00016310: 312d 3031 222c 2022 6322 3a20 3230 302c  1-01", "c": 200,
+00016320: 2022 6422 3a20 2241 4141 286e 616d 653d   "d": "AAA(name=
+00016330: 2741 6c69 6365 2729 227d 2c0a 2020 2020  'Alice')"},.    
+00016340: 2020 2020 2020 2020 7b22 6122 3a20 3130          {"a": 10
+00016350: 312c 2022 6222 3a20 2232 3030 312d 3031  1, "b": "2001-01
+00016360: 2d30 3122 2c20 2263 223a 2032 3031 2c20  -01", "c": 201, 
+00016370: 2264 223a 2022 4141 4128 6e61 6d65 3d27  "d": "AAA(name='
+00016380: 426f 6227 2922 7d0a 2020 2020 2020 2020  Bob')"}.        
+00016390: 2020 2020 5d0a 2020 2020 2020 2020 2222      ].        ""
+000163a0: 2229 0a0a 2020 2020 2020 2020 6a73 6f6e  ")..        json
+000163b0: 5f72 6573 756c 7420 3d20 7462 6c2e 6a73  _result = tbl.js
+000163c0: 6f6e 5f65 7870 6f72 7428 6a73 6f6e 5f65  on_export(json_e
+000163d0: 6e63 6f64 6572 3d28 4a73 6f6e 4461 7465  ncoder=(JsonDate
+000163e0: 456e 636f 6465 722c 204a 736f 6e41 4141  Encoder, JsonAAA
+000163f0: 456e 636f 6465 7229 290a 2020 2020 2020  Encoder)).      
+00016400: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00016410: 616c 2865 7870 6563 7465 642c 206a 736f  al(expected, jso
+00016420: 6e5f 7265 7375 6c74 290a 0a20 2020 2064  n_result)..    d
+00016430: 6566 2074 6573 745f 6669 7865 645f 7769  ef test_fixed_wi
+00016440: 6474 685f 696d 706f 7274 2873 656c 6629  dth_import(self)
+00016450: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
+00016460: 2066 6978 6564 5f77 6964 7468 5f64 6174   fixed_width_dat
+00016470: 610a 2020 2020 2020 2020 6461 7461 5f66  a.        data_f
+00016480: 696c 6520 3d20 696f 2e53 7472 696e 6749  ile = io.StringI
+00016490: 4f28 6461 7461 290a 2020 2020 2020 2020  O(data).        
+000164a0: 6677 5f73 7065 6320 3d20 5b28 2761 272c  fw_spec = [('a',
+000164b0: 2030 2c20 4e6f 6e65 2c20 696e 7429 2c20   0, None, int), 
+000164c0: 2827 6227 2c20 322c 204e 6f6e 652c 2069  ('b', 2, None, i
+000164d0: 6e74 292c 2028 2763 272c 2034 2c20 4e6f  nt), ('c', 4, No
+000164e0: 6e65 2c20 696e 7429 2c20 5d0a 2020 2020  ne, int), ].    
+000164f0: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
+00016500: 6528 292e 696e 7365 7274 5f6d 616e 7928  e().insert_many(
+00016510: 6c74 2e44 6174 614f 626a 6563 7428 2a2a  lt.DataObject(**
+00016520: 7265 6329 2066 6f72 2072 6563 2069 6e20  rec) for rec in 
+00016530: 6c74 2e46 6978 6564 5769 6474 6852 6561  lt.FixedWidthRea
+00016540: 6465 7228 6677 5f73 7065 632c 2064 6174  der(fw_spec, dat
+00016550: 615f 6669 6c65 2929 0a0a 2020 2020 2020  a_file))..      
+00016560: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
+00016570: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
+00016580: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
+00016590: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+000165a0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
+000165b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000165c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000165d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000165e0: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
+000165f0: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
+00016600: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
+00016610: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
+00016620: 3220 696e 207a 6970 2874 312c 2074 7429  2 in zip(t1, tt)
+00016630: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00016640: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00016650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016660: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+00016670: 285b 6420 666f 7220 6420 696e 2064 6174  ([d for d in dat
+00016680: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
+00016690: 6620 642e 7374 7269 7028 295d 292c 206c  f d.strip()]), l
+000166a0: 656e 2874 7429 290a 0a20 2020 2064 6566  en(tt))..    def
+000166b0: 2074 6573 745f 6669 7865 645f 7769 6474   test_fixed_widt
+000166c0: 685f 7374 7269 6e67 5f69 6d70 6f72 7428  h_string_import(
+000166d0: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
+000166e0: 6174 6120 3d20 6669 7865 645f 7769 6474  ata = fixed_widt
+000166f0: 685f 6461 7461 0a20 2020 2020 2020 2066  h_data.        f
+00016700: 775f 7370 6563 203d 205b 2827 6127 2c20  w_spec = [('a', 
+00016710: 302c 204e 6f6e 652c 2069 6e74 292c 2028  0, None, int), (
+00016720: 2762 272c 2032 2c20 4e6f 6e65 2c20 696e  'b', 2, None, in
+00016730: 7429 2c20 2827 6327 2c20 342c 204e 6f6e  t), ('c', 4, Non
+00016740: 652c 2069 6e74 292c 205d 0a20 2020 2020  e, int), ].     
+00016750: 2020 2074 7420 3d20 6c74 2e54 6162 6c65     tt = lt.Table
+00016760: 2829 2e69 6e73 6572 745f 6d61 6e79 286c  ().insert_many(l
+00016770: 742e 4461 7461 4f62 6a65 6374 282a 2a72  t.DataObject(**r
+00016780: 6563 2920 666f 7220 7265 6320 696e 206c  ec) for rec in l
+00016790: 742e 4669 7865 6457 6964 7468 5265 6164  t.FixedWidthRead
+000167a0: 6572 2866 775f 7370 6563 2c20 6461 7461  er(fw_spec, data
+000167b0: 2929 0a0a 2020 2020 2020 2020 7465 7374  ))..        test
+000167c0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+000167d0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+000167e0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+000167f0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00016800: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00016810: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00016820: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00016830: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00016840: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00016850: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00016860: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00016870: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00016880: 6970 2874 312c 2074 7429 2929 0a20 2020  ip(t1, tt))).   
+00016890: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000168a0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+000168b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000168c0: 7445 7175 616c 286c 656e 285b 6420 666f  tEqual(len([d fo
+000168d0: 7220 6420 696e 2064 6174 612e 7370 6c69  r d in data.spli
+000168e0: 746c 696e 6573 2829 2069 6620 642e 7374  tlines() if d.st
+000168f0: 7269 7028 295d 292c 206c 656e 2874 7429  rip()]), len(tt)
+00016900: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00016910: 6669 7865 645f 7769 6474 685f 7374 7269  fixed_width_stri
+00016920: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
+00016930: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
+00016940: 7461 203d 2066 6978 6564 5f77 6964 7468  ta = fixed_width
+00016950: 5f64 6174 610a 2020 2020 2020 2020 6677  _data.        fw
+00016960: 5f73 7065 6320 3d20 5b28 2761 272c 2030  _spec = [('a', 0
+00016970: 2c20 4e6f 6e65 2c20 696e 7429 2c20 2827  , None, int), ('
+00016980: 6227 2c20 322c 204e 6f6e 652c 2069 6e74  b', 2, None, int
+00016990: 292c 2028 2763 272c 2034 2c20 4e6f 6e65  ), ('c', 4, None
+000169a0: 2c20 696e 7429 2c5d 0a20 2020 2020 2020  , int),].       
+000169b0: 2074 7420 3d20 6c74 2e54 6162 6c65 2829   tt = lt.Table()
+000169c0: 2e69 6e73 6572 745f 6d61 6e79 286c 742e  .insert_many(lt.
+000169d0: 4461 7461 4f62 6a65 6374 282a 2a72 6563  DataObject(**rec
+000169e0: 2920 666f 7220 7265 6320 696e 206c 742e  ) for rec in lt.
+000169f0: 4669 7865 6457 6964 7468 5265 6164 6572  FixedWidthReader
+00016a00: 2866 775f 7370 6563 2c20 6461 7461 2e73  (fw_spec, data.s
+00016a10: 706c 6974 6c69 6e65 7328 2929 290a 0a20  plitlines())).. 
+00016a20: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00016a30: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
+00016a40: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00016a50: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00016a60: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00016a70: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
+00016a80: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00016a90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016aa0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+00016ab0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
+00016ac0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
+00016ad0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
+00016ae0: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
+00016af0: 2c20 7474 2929 290a 2020 2020 2020 2020  , tt))).        
+00016b00: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00016b10: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00016b20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016b30: 6c28 6c65 6e28 5b64 2066 6f72 2064 2069  l(len([d for d i
+00016b40: 6e20 6461 7461 2e73 706c 6974 6c69 6e65  n data.splitline
+00016b50: 7328 2920 6966 2064 2e73 7472 6970 2829  s() if d.strip()
+00016b60: 5d29 2c20 6c65 6e28 7474 2929 0a0a 2020  ]), len(tt))..  
+00016b70: 2020 6465 6620 7465 7374 5f65 7863 656c    def test_excel
+00016b80: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+00016b90: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+00016ba0: 203d 2022 7465 7374 2f61 6263 2e78 6c73   = "test/abc.xls
+00016bb0: 7822 0a20 2020 2020 2020 2065 7863 656c  x".        excel
+00016bc0: 5f74 6162 6c65 203d 206c 742e 5461 626c  _table = lt.Tabl
+00016bd0: 6528 292e 6578 6365 6c5f 696d 706f 7274  e().excel_import
+00016be0: 2866 696c 655f 6e61 6d65 2c20 7472 616e  (file_name, tran
+00016bf0: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
+00016c00: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
+00016c10: 2069 6e74 7d29 0a0a 2020 2020 2020 2020   int})..        
+00016c20: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
+00016c30: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
+00016c40: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
+00016c50: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00016c60: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
+00016c70: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00016c80: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00016c90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00016ca0: 7274 5472 7565 2861 6c6c 286d 616b 655f  rtTrue(all(make_
+00016cb0: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
+00016cc0: 6f62 2872 6563 3129 203d 3d20 7265 6332  ob(rec1) == rec2
+00016cd0: 2066 6f72 2072 6563 312c 2072 6563 3220   for rec1, rec2 
+00016ce0: 696e 207a 6970 2874 312c 2065 7863 656c  in zip(t1, excel
+00016cf0: 5f74 6162 6c65 2929 290a 2020 2020 2020  _table))).      
+00016d00: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00016d10: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00016d20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00016d30: 7561 6c28 7375 6d28 3120 666f 7220 6c69  ual(sum(1 for li
+00016d40: 6e65 2069 6e20 6373 765f 6461 7461 2e73  ne in csv_data.s
+00016d50: 706c 6974 6c69 6e65 7328 2920 6966 206c  plitlines() if l
+00016d60: 696e 652e 7374 7269 7028 2929 2d31 2c20  ine.strip())-1, 
+00016d70: 6c65 6e28 6578 6365 6c5f 7461 626c 6529  len(excel_table)
+00016d80: 290a 0a20 2020 2020 2020 2072 6f77 5f70  )..        row_p
+00016d90: 726f 746f 7479 7065 203d 2073 656c 662e  rototype = self.
+00016da0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00016db0: 2830 2c20 302c 2030 290a 2020 2020 2020  (0, 0, 0).      
+00016dc0: 2020 6373 7674 6162 6c65 3220 3d20 6c74    csvtable2 = lt
+00016dd0: 2e54 6162 6c65 2829 2e65 7863 656c 5f69  .Table().excel_i
+00016de0: 6d70 6f72 7428 0a20 2020 2020 2020 2020  mport(.         
+00016df0: 2020 2066 696c 655f 6e61 6d65 2c20 7472     file_name, tr
+00016e00: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
+00016e10: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
+00016e20: 273a 2069 6e74 7d2c 2072 6f77 5f63 6c61  ': int}, row_cla
+00016e30: 7373 3d74 7970 6528 726f 775f 7072 6f74  ss=type(row_prot
+00016e40: 6f74 7970 6529 0a20 2020 2020 2020 2029  otype).        )
+00016e50: 5b3a 335d 0a0a 2020 2020 2020 2020 7072  [:3]..        pr
+00016e60: 696e 7428 7479 7065 2874 315b 305d 292e  int(type(t1[0]).
+00016e70: 5f5f 6e61 6d65 5f5f 2c20 7431 5b30 5d29  __name__, t1[0])
+00016e80: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
+00016e90: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+00016ea0: 292e 5f5f 6e61 6d65 5f5f 2c20 6373 7674  ).__name__, csvt
+00016eb0: 6162 6c65 325b 305d 290a 2020 2020 2020  able2[0]).      
+00016ec0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00016ed0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00016ee0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00016ef0: 7561 6c28 7479 7065 2874 315b 305d 292c  ual(type(t1[0]),
+00016f00: 2074 7970 6528 6373 7674 6162 6c65 325b   type(csvtable2[
+00016f10: 305d 2929 0a0a 2020 2020 6465 6620 7465  0]))..    def te
+00016f20: 7374 5f65 7863 656c 5f65 7870 6f72 7428  st_excel_export(
+00016f30: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+00016f40: 696c 655f 6e61 6d65 203d 2022 7465 7374  ile_name = "test
+00016f50: 2f61 6263 2e78 6c73 7822 0a20 2020 2020  /abc.xlsx".     
+00016f60: 2020 2065 7863 656c 5f74 6162 6c65 203d     excel_table =
+00016f70: 206c 742e 5461 626c 6528 292e 6578 6365   lt.Table().exce
+00016f80: 6c5f 696d 706f 7274 2866 696c 655f 6e61  l_import(file_na
+00016f90: 6d65 2c20 7472 616e 7366 6f72 6d73 3d7b  me, transforms={
+00016fa0: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
+00016fb0: 6e74 2c20 2763 273a 2069 6e74 7d2c 206c  nt, 'c': int}, l
+00016fc0: 696d 6974 3d31 290a 2020 2020 2020 2020  imit=1).        
+00016fd0: 6f75 7466 696c 6520 3d20 696f 2e42 7974  outfile = io.Byt
+00016fe0: 6573 494f 2829 0a20 2020 2020 2020 2065  esIO().        e
+00016ff0: 7863 656c 5f74 6162 6c65 2e65 7863 656c  xcel_table.excel
+00017000: 5f65 7870 6f72 7428 6f75 7466 696c 6529  _export(outfile)
+00017010: 0a20 2020 2020 2020 2065 7870 6f72 7465  .        exporte
+00017020: 645f 7461 626c 6520 3d20 6c74 2e54 6162  d_table = lt.Tab
+00017030: 6c65 2829 2e65 7863 656c 5f69 6d70 6f72  le().excel_impor
+00017040: 7428 6f75 7466 696c 652c 2074 7261 6e73  t(outfile, trans
+00017050: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+00017060: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+00017070: 696e 747d 290a 0a20 2020 2020 2020 2077  int})..        w
+00017080: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00017090: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000170a0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+000170b0: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+000170c0: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+000170d0: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+000170e0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+000170f0: 6578 706f 7274 6564 5f74 6162 6c65 2c20  exported_table, 
+00017100: 6578 6365 6c5f 7461 626c 6529 2929 0a0a  excel_table)))..
+00017110: 2020 2020 6465 6620 7465 7374 5f6d 6f64      def test_mod
+00017120: 756c 655f 6c65 7665 6c5f 6373 765f 696d  ule_level_csv_im
+00017130: 706f 7274 6572 2873 656c 6629 3a0a 2020  porter(self):.  
+00017140: 2020 2020 2020 6461 7461 203d 2063 7376        data = csv
+00017150: 5f64 6174 610a 2020 2020 2020 2020 6373  _data.        cs
+00017160: 7674 6162 6c65 203d 206c 742e 6373 765f  vtable = lt.csv_
+00017170: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
+00017180: 653d 6461 7461 2c20 7472 616e 7366 6f72  e=data, transfor
+00017190: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
+000171a0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
+000171b0: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
+000171c0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+000171d0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+000171e0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+000171f0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00017200: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00017210: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00017220: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00017230: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00017240: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00017250: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00017260: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00017270: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00017280: 6970 2874 312c 2063 7376 7461 626c 6529  ip(t1, csvtable)
+00017290: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+000172a0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+000172b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000172c0: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
+000172d0: 2831 2066 6f72 206c 696e 6520 696e 2064  (1 for line in d
+000172e0: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+000172f0: 2069 6620 6c69 6e65 2e73 7472 6970 2829   if line.strip()
+00017300: 292d 312c 206c 656e 2863 7376 7461 626c  )-1, len(csvtabl
+00017310: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
+00017320: 745f 6d6f 6475 6c65 5f6c 6576 656c 5f6a  t_module_level_j
+00017330: 736f 6e5f 696d 706f 7274 6572 2873 656c  son_importer(sel
+00017340: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
+00017350: 203d 206a 736f 6e5f 6461 7461 0a20 2020   = json_data.   
+00017360: 2020 2020 206a 736f 6e74 6162 6c65 203d       jsontable =
+00017370: 206c 742e 6a73 6f6e 5f69 6d70 6f72 7428   lt.json_import(
+00017380: 6461 7461 2c20 7374 7265 616d 696e 673d  data, streaming=
+00017390: 5472 7565 2c20 7472 616e 7366 6f72 6d73  True, transforms
+000173a0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
+000173b0: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
+000173c0: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
+000173d0: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+000173e0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
+000173f0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00017400: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+00017410: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00017420: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00017430: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00017440: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00017450: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
+00017460: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
+00017470: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
+00017480: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
+00017490: 2874 312c 206a 736f 6e74 6162 6c65 2929  (t1, jsontable))
+000174a0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+000174b0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+000174c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000174d0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+000174e0: 5b64 2066 6f72 2064 2069 6e20 6461 7461  [d for d in data
+000174f0: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
+00017500: 2064 2e73 7472 6970 2829 5d29 2c20 6c65   d.strip()]), le
+00017510: 6e28 6a73 6f6e 7461 626c 6529 290a 0a20  n(jsontable)).. 
+00017520: 2020 2064 6566 2074 6573 745f 6d6f 6475     def test_modu
+00017530: 6c65 5f6c 6576 656c 5f65 7863 656c 5f69  le_level_excel_i
+00017540: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
+00017550: 2020 2020 2066 696c 655f 6e61 6d65 203d       file_name =
+00017560: 2022 7465 7374 2f61 6263 2e78 6c73 7822   "test/abc.xlsx"
+00017570: 0a20 2020 2020 2020 2065 7863 656c 5f74  .        excel_t
+00017580: 6162 6c65 203d 206c 742e 6578 6365 6c5f  able = lt.excel_
+00017590: 696d 706f 7274 2866 696c 655f 6e61 6d65  import(file_name
+000175a0: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
+000175b0: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
+000175c0: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
+000175d0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+000175e0: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
+000175f0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00017600: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+00017610: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+00017620: 6529 0a0a 2020 2020 2020 2020 7769 7468  e)..        with
+00017630: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00017640: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00017650: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
+00017660: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
+00017670: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
+00017680: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
+00017690: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
+000176a0: 2065 7863 656c 5f74 6162 6c65 2929 290a   excel_table))).
+000176b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000176c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000176d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000176e0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
+000176f0: 666f 7220 6c69 6e65 2069 6e20 6373 765f  for line in csv_
+00017700: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
+00017710: 2920 6966 206c 696e 652e 7374 7269 7028  ) if line.strip(
+00017720: 2929 2d31 2c20 6c65 6e28 6578 6365 6c5f  ))-1, len(excel_
+00017730: 7461 626c 6529 290a 0a0a 406d 616b 655f  table))...@make_
+00017740: 7465 7374 5f63 6c61 7373 6573 0a63 6c61  test_classes.cla
+00017750: 7373 2054 6162 6c65 5069 766f 7454 6573  ss TablePivotTes
+00017760: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
+00017770: 5f70 6976 6f74 2873 656c 6629 3a0a 2020  _pivot(self):.  
+00017780: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00017790: 3d20 350a 2020 2020 2020 2020 7431 203d  = 5.        t1 =
+000177a0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+000177b0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+000177c0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+000177d0: 6529 0a20 2020 2020 2020 2074 312e 6372  e).        t1.cr
+000177e0: 6561 7465 5f69 6e64 6578 2827 6127 290a  eate_index('a').
+000177f0: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
+00017800: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
+00017810: 2020 2020 2074 3170 6976 6f74 203d 2074       t1pivot = t
+00017820: 312e 7069 766f 7428 2761 2729 0a20 2020  1.pivot('a').   
+00017830: 2020 2020 2074 3170 6976 6f74 2e64 756d       t1pivot.dum
+00017840: 7028 290a 2020 2020 2020 2020 7431 7069  p().        t1pi
+00017850: 766f 742e 6475 6d70 5f63 6f75 6e74 7328  vot.dump_counts(
+00017860: 290a 2020 2020 2020 2020 7431 7069 766f  ).        t1pivo
+00017870: 742e 7375 6d6d 6172 795f 636f 756e 7473  t.summary_counts
+00017880: 2829 0a0a 2020 2020 2020 2020 7432 7069  ()..        t2pi
+00017890: 766f 7420 3d20 7431 2e70 6976 6f74 2827  vot = t1.pivot('
+000178a0: 6120 6227 290a 2020 2020 2020 2020 7432  a b').        t2
+000178b0: 7069 766f 742e 6475 6d70 2829 0a20 2020  pivot.dump().   
+000178c0: 2020 2020 2074 3270 6976 6f74 2e64 756d       t2pivot.dum
+000178d0: 705f 636f 756e 7473 2829 0a20 2020 2020  p_counts().     
+000178e0: 2020 2074 3270 6976 6f74 2e73 756d 6d61     t2pivot.summa
+000178f0: 7279 5f63 6f75 6e74 7328 290a 0a20 2020  ry_counts()..   
+00017900: 2020 2020 2023 2054 4f44 4f20 2d20 6164       # TODO - ad
+00017910: 6420 6173 7365 7274 730a 0a0a 636c 6173  d asserts...clas
+00017920: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
+00017930: 7473 2875 6e69 7474 6573 742e 5465 7374  ts(unittest.Test
+00017940: 4361 7365 293a 0a20 2020 2072 6563 6970  Case):.    recip
+00017950: 655f 6461 7461 203d 2074 6578 7477 7261  e_data = textwra
+00017960: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+00017970: 2020 2020 2020 6964 2c74 6974 6c65 2c69        id,title,i
+00017980: 6e67 7265 6469 656e 7473 0a20 2020 2020  ngredients.     
+00017990: 2020 2031 2c54 756e 6120 6361 7373 6572     1,Tuna casser
+000179a0: 6f6c 652c 2274 756e 612c 206e 6f6f 646c  ole,"tuna, noodl
+000179b0: 6573 2c20 4372 6561 6d20 6f66 204d 7573  es, Cream of Mus
+000179c0: 6872 6f6f 6d20 536f 7570 220a 2020 2020  hroom Soup".    
+000179d0: 2020 2020 322c 4861 7761 6969 616e 2070      2,Hawaiian p
+000179e0: 697a 7a61 2c70 697a 7a61 2064 6f75 6768  izza,pizza dough
+000179f0: 2070 696e 6561 7070 6c65 2068 616d 2074   pineapple ham t
+00017a00: 6f6d 6174 6f20 7361 7563 650a 2020 2020  omato sauce.    
+00017a10: 2020 2020 332c 4d61 7267 6865 7269 7461      3,Margherita
+00017a20: 2070 697a 7a61 2c70 697a 7a61 2064 6f75   pizza,pizza dou
+00017a30: 6768 2063 6865 6573 6520 7065 7374 6f20  gh cheese pesto 
+00017a40: 6172 7469 6368 6f6b 6520 6865 6172 7473  artichoke hearts
+00017a50: 0a20 2020 2020 2020 2034 2c50 6570 7065  .        4,Peppe
+00017a60: 726f 6e69 2070 697a 7a61 2c70 697a 7a61  roni pizza,pizza
+00017a70: 2064 6f75 6768 2063 6865 6573 6520 746f   dough cheese to
+00017a80: 6d61 746f 2073 6175 6365 2070 6570 7065  mato sauce peppe
+00017a90: 726f 6e69 0a20 2020 2020 2020 2035 2c47  roni.        5,G
+00017aa0: 7269 6c6c 6564 2063 6865 6573 6520 7361  rilled cheese sa
+00017ab0: 6e64 7769 6368 2c62 7265 6164 2063 6865  ndwich,bread che
+00017ac0: 6573 6520 6275 7474 6572 0a20 2020 2020  ese butter.     
+00017ad0: 2020 2036 2c54 756e 6120 6d65 6c74 2c74     6,Tuna melt,t
+00017ae0: 756e 6120 6d61 796f 6e6e 6169 7365 2074  una mayonnaise t
+00017af0: 6f6d 6174 6f20 6272 6561 6420 6368 6565  omato bread chee
+00017b00: 7365 0a20 2020 2020 2020 2037 2c43 6869  se.        7,Chi
+00017b10: 6c69 2064 6f67 2c68 6f74 2064 6f67 2063  li dog,hot dog c
+00017b20: 6869 6c69 206f 6e69 6f6e 2062 756e 0a20  hili onion bun. 
+00017b30: 2020 2020 2020 2038 2c46 7265 6e63 6820         8,French 
+00017b40: 746f 6173 742c 6567 6720 6d69 6c6b 2076  toast,egg milk v
+00017b50: 616e 696c 6c61 2062 7265 6164 206d 6170  anilla bread map
+00017b60: 6c65 2073 7972 7570 0a20 2020 2020 2020  le syrup.       
+00017b70: 2039 2c42 4c54 2c62 7265 6164 2062 6163   9,BLT,bread bac
+00017b80: 6f6e 206c 6574 7475 6365 2074 6f6d 6174  on lettuce tomat
+00017b90: 6f20 6d61 796f 6e6e 6169 7365 0a20 2020  o mayonnaise.   
+00017ba0: 2020 2020 2031 302c 5265 7562 656e 2073       10,Reuben s
+00017bb0: 616e 6477 6963 682c 7279 6520 6272 6561  andwich,rye brea
+00017bc0: 6420 7361 7565 726b 7261 7574 2063 6f72  d sauerkraut cor
+00017bd0: 6e65 6420 6265 6566 2073 7769 7373 2063  ned beef swiss c
+00017be0: 6865 6573 6520 7275 7373 6961 6e20 6472  heese russian dr
+00017bf0: 6573 7369 6e67 2074 686f 7573 616e 6420  essing thousand 
+00017c00: 6973 6c61 6e64 0a20 2020 2020 2020 2031  island.        1
+00017c10: 312c 4861 6d62 7572 6765 722c 6772 6f75  1,Hamburger,grou
+00017c20: 6e64 2062 6565 6620 6275 6e20 6c65 7474  nd beef bun lett
+00017c30: 7563 6520 6b65 7463 6875 7020 6d75 7374  uce ketchup must
+00017c40: 6172 6420 7069 636b 6c65 0a20 2020 2020  ard pickle.     
+00017c50: 2020 2031 322c 4368 6565 7365 6275 7267     12,Cheeseburg
+00017c60: 6572 2c67 726f 756e 6420 6265 6566 2062  er,ground beef b
+00017c70: 756e 206c 6574 7475 6365 206b 6574 6368  un lettuce ketch
+00017c80: 7570 206d 7573 7461 7264 2070 6963 6b6c  up mustard pickl
+00017c90: 6520 6368 6565 7365 0a20 2020 2020 2020  e cheese.       
+00017ca0: 2031 332c 4261 636f 6e20 6368 6565 7365   13,Bacon cheese
+00017cb0: 6275 7267 6572 2c67 726f 756e 6420 6265  burger,ground be
+00017cc0: 6566 2062 756e 206c 6574 7475 6365 206b  ef bun lettuce k
+00017cd0: 6574 6368 7570 206d 7573 7461 7264 2070  etchup mustard p
+00017ce0: 6963 6b6c 6520 6368 6565 7365 2062 6163  ickle cheese bac
+00017cf0: 6f6e 0a20 2020 2020 2020 2022 2222 290a  on.        """).
+00017d00: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+00017d10: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00017d20: 6c66 2e72 6563 6970 6573 203d 206c 742e  lf.recipes = lt.
+00017d30: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00017d40: 7274 2873 656c 662e 7265 6369 7065 5f64  rt(self.recipe_d
+00017d50: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
+00017d60: 6469 6374 2869 643d 696e 7429 290a 2020  dict(id=int)).  
+00017d70: 2020 2020 2020 7365 6c66 2e72 6563 6970        self.recip
+00017d80: 6573 2e63 7265 6174 655f 696e 6465 7828  es.create_index(
+00017d90: 2269 6422 2c20 756e 6971 7565 3d54 7275  "id", unique=Tru
+00017da0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00017db0: 7265 6369 7065 732e 6372 6561 7465 5f73  recipes.create_s
+00017dc0: 6561 7263 685f 696e 6465 7828 2269 6e67  earch_index("ing
+00017dd0: 7265 6469 656e 7473 2229 0a0a 2020 2020  redients")..    
+00017de0: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+00017df0: 2020 2064 6566 2074 6573 745f 6163 6365     def test_acce
+00017e00: 7373 5f6e 6f6e 5f65 7869 7374 656e 745f  ss_non_existent_
+00017e10: 7365 6172 6368 5f61 7474 7269 6275 7465  search_attribute
+00017e20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00017e30: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00017e40: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
+00017e50: 722c 206d 7367 3d22 6661 696c 6564 2074  r, msg="failed t
+00017e60: 6f20 7261 6973 6520 5661 6c75 6545 7272  o raise ValueErr
+00017e70: 6f72 2077 6865 6e20 6163 6365 7373 696e  or when accessin
+00017e80: 6720 6e6f 6e2d 6578 6973 7465 6e74 2073  g non-existent s
+00017e90: 6561 7263 6820 696e 6465 7822 293a 0a20  earch index"):. 
+00017ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017eb0: 7265 6369 7065 732e 7365 6172 6368 2e74  recipes.search.t
+00017ec0: 6974 6c65 2822 7879 7a22 290a 0a20 2020  itle("xyz")..   
+00017ed0: 2040 616e 6e6f 756e 6365 5f74 6573 740a   @announce_test.
+00017ee0: 2020 2020 6465 6620 7465 7374 5f73 6561      def test_sea
+00017ef0: 7263 685f 6469 7228 7365 6c66 293a 0a20  rch_dir(self):. 
+00017f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00017f10: 7274 4571 7561 6c28 5b27 696e 6772 6564  rtEqual(['ingred
+00017f20: 6965 6e74 7327 5d2c 2064 6972 2873 656c  ients'], dir(sel
+00017f30: 662e 7265 6369 7065 732e 7365 6172 6368  f.recipes.search
+00017f40: 292c 2022 6661 696c 6564 2074 6f20 6765  ), "failed to ge
+00017f50: 6e65 7261 7465 2063 6f72 7265 6374 2064  nerate correct d
+00017f60: 6972 2829 2072 6573 706f 6e73 6522 290a  ir() response").
+00017f70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+00017f80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+00017f90: 5f74 6578 745f 7365 6172 6368 2873 656c  _text_search(sel
+00017fa0: 6629 3a0a 2020 2020 2020 2020 666f 7220  f):.        for 
+00017fb0: 7175 6572 792c 2065 7870 6563 7465 6420  query, expected 
+00017fc0: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
+00017fd0: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
+00017fe0: 2020 2020 2020 2028 2274 756e 6122 2c20         ("tuna", 
+00017ff0: 5b31 2c20 365d 292c 0a20 2020 2020 2020  [1, 6]),.       
+00018000: 2020 2020 2028 2274 756e 6120 2b63 6865       ("tuna +che
+00018010: 6573 6522 2c20 5b36 2c20 332c 2034 2c20  ese", [6, 3, 4, 
+00018020: 352c 2031 302c 2031 322c 2031 332c 2031  5, 10, 12, 13, 1
+00018030: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00018040: 2822 7069 6e65 6170 706c 6520 2b62 6163  ("pineapple +bac
+00018050: 6f6e 206c 6574 7475 6365 2062 6565 6620  on lettuce beef 
+00018060: 2d73 6175 6572 6b72 6175 7420 746f 6d61  -sauerkraut toma
+00018070: 746f 222c 205b 392c 2031 332c 2032 2c20  to", [9, 13, 2, 
+00018080: 3131 2c20 3132 2c20 342c 2036 2c20 3130  11, 12, 4, 6, 10
+00018090: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+000180a0: 2822 7069 7a7a 6120 646f 7567 6820 2d70  ("pizza dough -p
+000180b0: 696e 6561 7070 6c65 222c 205b 332c 2034  ineapple", [3, 4
+000180c0: 2c20 325d 292c 0a20 2020 2020 2020 2020  , 2]),.         
+000180d0: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
+000180e0: 202d 2d70 696e 6561 7070 6c65 222c 205b   --pineapple", [
+000180f0: 332c 2034 5d29 2c0a 2020 2020 2020 2020  3, 4]),.        
+00018100: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
+00018110: 6e22 2c20 5b39 2c20 352c 2036 2c20 382c  n", [9, 5, 6, 8,
+00018120: 2031 302c 2031 335d 292c 0a20 2020 2020   10, 13]),.     
+00018130: 2020 2020 2020 2028 2262 7265 6164 202b         ("bread +
+00018140: 2b62 6163 6f6e 222c 205b 392c 2031 335d  +bacon", [9, 13]
+00018150: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00018160: 2262 7265 6164 202b 2b61 6e63 686f 7669  "bread ++anchovi
+00018170: 6573 222c 205b 5d29 2c0a 2020 2020 2020  es", []),.      
+00018180: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
+00018190: 6261 636f 6e20 2b2b 616e 6368 6f76 6965  bacon ++anchovie
+000181a0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
+000181b0: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
+000181c0: 6f6e 202d 2d61 6e63 686f 7669 6573 222c  on --anchovies",
+000181d0: 205b 392c 2035 2c20 362c 2038 2c20 3130   [9, 5, 6, 8, 10
+000181e0: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
+000181f0: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
+00018200: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
+00018210: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
+00018220: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
+00018230: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
+00018240: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
+00018250: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+00018260: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
+00018270: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
+00018280: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
+00018290: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000182a0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
+000182b0: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
+000182c0: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
+000182d0: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
+000182e0: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
+000182f0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00018300: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
+00018310: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00018320: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00018330: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
+00018340: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
+00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018360: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
+00018370: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
+00018380: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
+00018390: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
+000183a0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
+000183b0: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
+000183c0: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+000183d0: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
+000183e0: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
+000183f0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00018400: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
+00018410: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00018420: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
+00018430: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
+00018440: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
+00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018460: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00018470: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
+00018480: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
+00018490: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
+000184a0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
+000184b0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+000184c0: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
+000184d0: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
+000184e0: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
+000184f0: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
+00018500: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
+00018510: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
+00018520: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
+00018530: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
+00018540: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
+00018550: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00018560: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
+00018570: 5b7b 276e 6f6f 646c 6573 272c 2027 6e6f  [{'noodles', 'no
+00018580: 6f64 6c65 272c 2027 7475 6e61 272c 2027  odle', 'tuna', '
+00018590: 736f 7570 272c 2027 6372 6561 6d27 2c20  soup', 'cream', 
+000185a0: 276d 7573 6872 6f6f 6d27 7d2c 0a20 2020  'mushroom'},.   
+000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000185d0: 2774 6f6d 6174 6f27 2c20 2774 756e 6127  'tomato', 'tuna'
+000185e0: 2c20 276d 6179 6f6e 6e61 6973 6527 2c20  , 'mayonnaise', 
+000185f0: 2762 7265 6164 272c 2027 6368 6565 7365  'bread', 'cheese
+00018600: 277d 5d29 2c0a 2020 2020 2020 2020 2020  '}]),.          
+00018610: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
+00018620: 2020 2020 206d 6174 6368 6573 203d 2073       matches = s
+00018630: 656c 662e 7265 6369 7065 732e 7365 6172  elf.recipes.sear
+00018640: 6368 2e69 6e67 7265 6469 656e 7473 2871  ch.ingredients(q
+00018650: 7565 7279 2c20 6d69 6e5f 7363 6f72 653d  uery, min_score=
+00018660: 2d31 3030 3030 2c20 6173 5f74 6162 6c65  -10000, as_table
+00018670: 3d46 616c 7365 2c20 696e 636c 7564 655f  =False, include_
+00018680: 776f 7264 733d 5472 7565 290a 2020 2020  words=True).    
+00018690: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+000186a0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+000186b0: 6f72 2072 6563 6970 652c 2073 636f 7265  or recipe, score
+000186c0: 2c20 776f 7264 7320 696e 206d 6174 6368  , words in match
+000186d0: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
+000186e0: 7072 696e 7428 7265 7072 2871 7565 7279  print(repr(query
+000186f0: 292c 2027 2d3e 272c 205b 2872 6563 6970  ), '->', [(recip
+00018700: 652e 6964 2c20 7363 6f72 652c 2077 6f72  e.id, score, wor
+00018710: 6473 2920 666f 7220 7265 6369 7065 2c20  ds) for recipe, 
+00018720: 7363 6f72 652c 2077 6f72 6473 2069 6e20  score, words in 
+00018730: 6d61 7463 6865 735d 290a 2020 2020 2020  matches]).      
+00018740: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00018750: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00018760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018770: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00018780: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
+00018790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187b0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
+000187c0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
+000187d0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
+000187e0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
+000187f0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
+00018800: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00018810: 685f 776f 7264 7320 3d20 5b73 6574 2877  h_words = [set(w
+00018820: 6f72 6473 2920 666f 7220 7265 6369 7065  ords) for recipe
+00018830: 2c20 7363 6f72 652c 2077 6f72 6473 2069  , score, words i
+00018840: 6e20 6d61 7463 6865 735d 0a20 2020 2020  n matches].     
+00018850: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00018860: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00018870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018880: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
+00018890: 6563 7465 645f 776f 7264 732c 206d 6174  ected_words, mat
+000188a0: 6368 5f77 6f72 6473 2c0a 2020 2020 2020  ch_words,.      
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 2020 2020 2020 2020 2020 2022 696e 7661             "inva
+000188d0: 6c69 6420 6d61 7463 6820 776f 7264 7320  lid match words 
+000188e0: 666f 7220 7175 6572 7920 7b21 727d 2c20  for query {!r}, 
+000188f0: 6578 7065 6374 6564 207b 7d2c 2067 6f74  expected {}, got
+00018900: 207b 7d22 2e66 6f72 6d61 7428 7175 6572   {}".format(quer
+00018910: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018970: 2020 2020 2065 7870 6563 7465 645f 776f       expected_wo
+00018980: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
+00018990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189e0: 2020 2020 2020 206d 6174 6368 5f77 6f72         match_wor
+000189f0: 6473 2929 0a0a 2020 2020 4061 6e6e 6f75  ds))..    @annou
+00018a00: 6e63 655f 7465 7374 0a20 2020 2064 6566  nce_test.    def
+00018a10: 2074 6573 745f 7365 6172 6368 5f77 6974   test_search_wit
+00018a20: 685f 6c69 6d69 7428 7365 6c66 293a 0a20  h_limit(self):. 
+00018a30: 2020 2020 2020 2066 6f72 2071 7565 7279         for query
+00018a40: 2c20 6578 7065 6374 6564 2069 6e20 5b0a  , expected in [.
+00018a50: 2020 2020 2020 2020 2020 2020 2822 222c              ("",
+00018a60: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00018a70: 2020 2822 7475 6e61 222c 205b 312c 2036    ("tuna", [1, 6
+00018a80: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00018a90: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
+00018aa0: 205b 362c 2033 2c20 345d 292c 0a20 2020   [6, 3, 4]),.   
+00018ab0: 2020 2020 2020 2020 2028 2270 696e 6561           ("pinea
+00018ac0: 7070 6c65 202b 6261 636f 6e20 6c65 7474  pple +bacon lett
+00018ad0: 7563 6520 6265 6566 202d 7361 7565 726b  uce beef -sauerk
+00018ae0: 7261 7574 2074 6f6d 6174 6f22 2c20 5b39  raut tomato", [9
+00018af0: 2c20 3133 2c20 325d 292c 0a20 2020 2020  , 13, 2]),.     
+00018b00: 2020 2020 2020 2028 2270 697a 7a61 2064         ("pizza d
+00018b10: 6f75 6768 202d 7069 6e65 6170 706c 6522  ough -pineapple"
+00018b20: 2c20 5b33 2c20 342c 2032 5d29 2c0a 2020  , [3, 4, 2]),.  
+00018b30: 2020 2020 2020 2020 2020 2822 7069 7a7a            ("pizz
+00018b40: 6120 646f 7567 6820 2d2d 7069 6e65 6170  a dough --pineap
+00018b50: 706c 6522 2c20 5b33 2c20 345d 292c 0a20  ple", [3, 4]),. 
+00018b60: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+00018b70: 6164 2062 6163 6f6e 222c 205b 392c 2035  ad bacon", [9, 5
+00018b80: 2c20 365d 292c 0a20 2020 2020 2020 2020  , 6]),.         
+00018b90: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
+00018ba0: 6f6e 222c 205b 392c 2031 335d 292c 0a20  on", [9, 13]),. 
+00018bb0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+00018bc0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
+00018bd0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00018be0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
+00018bf0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
+00018c00: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00018c10: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
+00018c20: 2d61 6e63 686f 7669 6573 222c 205b 392c  -anchovies", [9,
+00018c30: 2035 2c20 365d 292c 0a20 2020 2020 2020   5, 6]),.       
+00018c40: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
+00018c50: 6d61 7463 6865 7320 3d20 7365 6c66 2e72  matches = self.r
+00018c60: 6563 6970 6573 2e73 6561 7263 682e 696e  ecipes.search.in
+00018c70: 6772 6564 6965 6e74 7328 7175 6572 792c  gredients(query,
+00018c80: 2061 735f 7461 626c 653d 4661 6c73 652c   as_table=False,
+00018c90: 206d 696e 5f73 636f 7265 3d2d 3130 3030   min_score=-1000
+00018ca0: 302c 206c 696d 6974 3d33 290a 2020 2020  0, limit=3).    
+00018cb0: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+00018cc0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+00018cd0: 6f72 2072 6563 6970 652c 205f 2069 6e20  or recipe, _ in 
+00018ce0: 6d61 7463 6865 735d 0a20 2020 2020 2020  matches].       
+00018cf0: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
+00018d00: 7175 6572 7929 2c20 272d 3e27 2c20 5b28  query), '->', [(
+00018d10: 7265 6369 7065 2e69 642c 2073 636f 7265  recipe.id, score
+00018d20: 2920 666f 7220 7265 6369 7065 2c20 7363  ) for recipe, sc
+00018d30: 6f72 6520 696e 206d 6174 6368 6573 5d29  ore in matches])
+00018d40: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00018d50: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
+00018d60: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
+00018d70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018d80: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+00018d90: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
+00018da0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018dc0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
+00018dd0: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
+00018de0: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
+00018df0: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
+00018e00: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
+00018e10: 290a 0a20 2020 2040 616e 6e6f 756e 6365  )..    @announce
+00018e20: 5f74 6573 740a 2020 2020 6465 6620 7465  _test.    def te
+00018e30: 7374 5f73 6561 7263 685f 7769 7468 5f6d  st_search_with_m
+00018e40: 696e 5f73 636f 7265 2873 656c 6629 3a0a  in_score(self):.
+00018e50: 2020 2020 2020 2020 666f 7220 7175 6572          for quer
+00018e60: 792c 2065 7870 6563 7465 6420 696e 205b  y, expected in [
+00018e70: 0a20 2020 2020 2020 2020 2020 2028 2222  .            (""
+00018e80: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
+00018e90: 2020 2028 2274 756e 6122 2c20 5b5d 292c     ("tuna", []),
+00018ea0: 0a20 2020 2020 2020 2020 2020 2028 2274  .            ("t
+00018eb0: 756e 6120 2b63 6865 6573 6522 2c20 5b36  una +cheese", [6
+00018ec0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
+00018ed0: 2028 2270 696e 6561 7070 6c65 202b 6261   ("pineapple +ba
+00018ee0: 636f 6e20 6c65 7474 7563 6520 6265 6566  con lettuce beef
+00018ef0: 202d 7361 7565 726b 7261 7574 2074 6f6d   -sauerkraut tom
+00018f00: 6174 6f22 2c20 5b39 2c20 3133 5d29 2c0a  ato", [9, 13]),.
+00018f10: 2020 2020 2020 2020 2020 2020 2822 7069              ("pi
+00018f20: 7a7a 6120 646f 7567 6820 2d70 696e 6561  zza dough -pinea
+00018f30: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
+00018f40: 2020 2020 2020 2020 2822 7069 7a7a 6120          ("pizza 
+00018f50: 646f 7567 6820 2d2d 7069 6e65 6170 706c  dough --pineappl
+00018f60: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
+00018f70: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
+00018f80: 6f6e 222c 205b 5d29 2c0a 2020 2020 2020  on", []),.      
+00018f90: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
+00018fa0: 6261 636f 6e22 2c20 5b39 2c5d 292c 0a20  bacon", [9,]),. 
+00018fb0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+00018fc0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
+00018fd0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00018fe0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
+00018ff0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
+00019000: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00019010: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
+00019020: 2d61 6e63 686f 7669 6573 222c 205b 5d29  -anchovies", [])
+00019030: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+00019040: 2020 2020 2020 2020 206d 6174 6368 6573           matches
+00019050: 203d 2073 656c 662e 7265 6369 7065 732e   = self.recipes.
+00019060: 7365 6172 6368 2e69 6e67 7265 6469 656e  search.ingredien
+00019070: 7473 2871 7565 7279 2c20 6173 5f74 6162  ts(query, as_tab
+00019080: 6c65 3d46 616c 7365 2c20 6d69 6e5f 7363  le=False, min_sc
+00019090: 6f72 653d 3130 3030 290a 2020 2020 2020  ore=1000).      
+000190a0: 2020 2020 2020 6d61 7463 685f 6964 7320        match_ids 
+000190b0: 3d20 5b72 6563 6970 652e 6964 2066 6f72  = [recipe.id for
+000190c0: 2072 6563 6970 652c 205f 2069 6e20 6d61   recipe, _ in ma
+000190d0: 7463 6865 735d 0a20 2020 2020 2020 2020  tches].         
+000190e0: 2020 2070 7269 6e74 2872 6570 7228 7175     print(repr(qu
+000190f0: 6572 7929 2c20 272d 3e27 2c20 5b28 7265  ery), '->', [(re
+00019100: 6369 7065 2e69 642c 2073 636f 7265 2920  cipe.id, score) 
+00019110: 666f 7220 7265 6369 7065 2c20 7363 6f72  for recipe, scor
+00019120: 6520 696e 206d 6174 6368 6573 5d29 0a20  e in matches]). 
+00019130: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00019140: 7365 6c66 2e73 7562 5465 7374 2871 7565  self.subTest(que
+00019150: 7279 3d71 7565 7279 293a 0a20 2020 2020  ry=query):.     
+00019160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019170: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00019180: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
+00019190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
+000191c0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
+000191d0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
+000191e0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
+000191f0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
+00019200: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+00019210: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+00019220: 5f73 6561 7263 685f 7769 7468 5f61 735f  _search_with_as_
+00019230: 7461 626c 6528 7365 6c66 293a 0a20 2020  table(self):.   
+00019240: 2020 2020 2066 6f72 2071 7565 7279 2c20       for query, 
+00019250: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
+00019260: 2020 2020 2020 2020 2020 2822 222c 205b            ("", [
+00019270: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019280: 2822 7475 6e61 222c 205b 5d29 2c0a 2020  ("tuna", []),.  
+00019290: 2020 2020 2020 2020 2020 2822 7475 6e61            ("tuna
+000192a0: 202b 6368 6565 7365 222c 205b 362c 5d29   +cheese", [6,])
+000192b0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000192c0: 7069 6e65 6170 706c 6520 2b62 6163 6f6e  pineapple +bacon
+000192d0: 206c 6574 7475 6365 2062 6565 6620 2d73   lettuce beef -s
+000192e0: 6175 6572 6b72 6175 7420 746f 6d61 746f  auerkraut tomato
+000192f0: 222c 205b 392c 2031 335d 292c 0a20 2020  ", [9, 13]),.   
+00019300: 2020 2020 2020 2020 2028 2270 697a 7a61           ("pizza
+00019310: 2064 6f75 6768 202d 7069 6e65 6170 706c   dough -pineappl
+00019320: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
+00019330: 2020 2020 2028 2270 697a 7a61 2064 6f75       ("pizza dou
+00019340: 6768 202d 2d70 696e 6561 7070 6c65 222c  gh --pineapple",
+00019350: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00019360: 2020 2822 6272 6561 6420 6261 636f 6e22    ("bread bacon"
+00019370: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
+00019380: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
+00019390: 6f6e 222c 205b 392c 5d29 2c0a 2020 2020  on", [9,]),.    
+000193a0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+000193b0: 2b2b 616e 6368 6f76 6965 7322 2c20 5b5d  ++anchovies", []
+000193c0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+000193d0: 2262 7265 6164 202b 2b62 6163 6f6e 202b  "bread ++bacon +
+000193e0: 2b61 6e63 686f 7669 6573 222c 205b 5d29  +anchovies", [])
+000193f0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00019400: 6272 6561 6420 6261 636f 6e20 2d2d 616e  bread bacon --an
+00019410: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
+00019420: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+00019430: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
+00019440: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
+00019450: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
+00019460: 7175 6572 792c 206d 696e 5f73 636f 7265  query, min_score
+00019470: 3d31 3030 302c 2061 735f 7461 626c 653d  =1000, as_table=
+00019480: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00019490: 2020 6d61 7463 685f 6964 7320 3d20 5b72    match_ids = [r
+000194a0: 6563 6970 652e 6964 2066 6f72 2072 6563  ecipe.id for rec
+000194b0: 6970 6520 696e 206d 6174 6368 6573 5d0a  ipe in matches].
+000194c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000194d0: 7428 7265 7072 2871 7565 7279 292c 2027  t(repr(query), '
+000194e0: 2d3e 272c 205b 2872 6563 6970 652e 6964  ->', [(recipe.id
+000194f0: 2c20 7265 6369 7065 2e69 6e67 7265 6469  , recipe.ingredi
+00019500: 656e 7473 5f73 6561 7263 685f 7363 6f72  ents_search_scor
+00019510: 6529 2066 6f72 2072 6563 6970 6520 696e  e) for recipe in
+00019520: 206d 6174 6368 6573 5d29 0a20 2020 2020   matches]).     
+00019530: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00019540: 2e73 7562 5465 7374 2871 7565 7279 3d71  .subTest(query=q
+00019550: 7565 7279 293a 0a20 2020 2020 2020 2020  uery):.         
+00019560: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00019570: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+00019580: 2c20 6d61 7463 685f 6964 732c 0a20 2020  , match_ids,.   
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000195b0: 696e 7661 6c69 6420 7265 7375 6c74 7320  invalid results 
+000195c0: 666f 7220 7175 6572 7920 7b71 7565 7279  for query {query
+000195d0: 2172 7d2c 2065 7870 6563 7465 6420 7b65  !r}, expected {e
+000195e0: 7870 6563 7465 647d 2c20 676f 7420 7b6d  xpected}, got {m
+000195f0: 6174 6368 5f69 6473 7d22 290a 0a20 2020  atch_ids}")..   
+00019600: 2020 2020 2020 2020 2073 636f 7265 5f61           score_a
+00019610: 7474 7220 3d20 2269 6e67 7265 6469 656e  ttr = "ingredien
+00019620: 7473 5f73 6561 7263 685f 7363 6f72 6522  ts_search_score"
+00019630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019640: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+00019650: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00019660: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00019670: 2020 2020 2020 2068 6173 6174 7472 286d         hasattr(m
+00019680: 6174 6368 6573 2e62 792e 6964 5b6d 6964  atches.by.id[mid
+00019690: 5d2c 2073 636f 7265 5f61 7474 7229 0a20  ], score_attr). 
+000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196b0: 2020 2066 6f72 206d 6964 2069 6e20 6d61     for mid in ma
+000196c0: 7463 685f 6964 730a 2020 2020 2020 2020  tch_ids.        
+000196d0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000196e0: 2020 2020 2020 2020 2020 2066 2261 735f             f"as_
+000196f0: 7461 626c 6520 6469 6420 6e6f 7420 706f  table did not po
+00019700: 7075 6c61 7465 2073 6f6d 6520 7365 6172  pulate some sear
+00019710: 6368 2072 6563 6f72 6473 2077 6974 6820  ch records with 
+00019720: 7b73 636f 7265 5f61 7474 7221 727d 220a  {score_attr!r}".
+00019730: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00019740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019750: 6173 7365 7274 4661 6c73 6528 0a20 2020  assertFalse(.   
+00019760: 2020 2020 2020 2020 2020 2020 2061 6e79               any
+00019770: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00019780: 2020 2020 2020 6861 7361 7474 7228 7365        hasattr(se
+00019790: 6c66 2e72 6563 6970 6573 2e62 792e 6964  lf.recipes.by.id
+000197a0: 5b6d 6964 5d2c 2073 636f 7265 5f61 7474  [mid], score_att
+000197b0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+000197c0: 2020 2020 2020 2066 6f72 206d 6964 2069         for mid i
+000197d0: 6e20 6d61 7463 685f 6964 730a 2020 2020  n match_ids.    
+000197e0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+000197f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00019800: 2261 735f 7461 626c 6520 706f 7075 6c61  "as_table popula
+00019810: 7465 6420 736f 6d65 206f 7269 6769 6e61  ted some origina
+00019820: 6c20 7265 636f 7264 7320 7769 7468 207b  l records with {
+00019830: 7363 6f72 655f 6174 7472 2172 7d22 0a20  score_attr!r}". 
+00019840: 2020 2020 2020 2020 2020 2029 0a0a 636c             )..cl
+00019850: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
+00019860: 6573 7473 5f44 6174 614f 626a 6563 7473  ests_DataObjects
+00019870: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+00019880: 732c 2055 7369 6e67 4461 7461 4f62 6a65  s, UsingDataObje
+00019890: 6374 7329 3a0a 2020 2020 7061 7373 0a0a  cts):.    pass..
+000198a0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
+000198b0: 6854 6573 7473 5f4e 616d 6564 7475 706c  hTests_Namedtupl
+000198c0: 6573 2854 6162 6c65 5365 6172 6368 5465  es(TableSearchTe
+000198d0: 7374 732c 2055 7369 6e67 4e61 6d65 6474  sts, UsingNamedt
+000198e0: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
+000198f0: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
+00019900: 7263 6854 6573 7473 5f54 7970 696e 674e  rchTests_TypingN
+00019910: 616d 6564 7475 706c 6573 2854 6162 6c65  amedtuples(Table
+00019920: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+00019930: 6e67 5479 7069 6e67 4e61 6d65 6454 7570  ngTypingNamedTup
+00019940: 6c65 293a 0a20 2020 2070 6173 730a 0a63  le):.    pass..c
+00019950: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
+00019960: 5465 7374 735f 5479 7069 6e67 5479 7065  Tests_TypingType
+00019970: 6444 6963 7428 5461 626c 6553 6561 7263  dDict(TableSearc
+00019980: 6854 6573 7473 2c20 5573 696e 6754 7970  hTests, UsingTyp
+00019990: 696e 6754 7970 6564 4469 6374 293a 0a20  ingTypedDict):. 
+000199a0: 2020 2070 6173 730a 0a63 6c61 7373 2054     pass..class T
+000199b0: 6162 6c65 5365 6172 6368 5465 7374 735f  ableSearchTests_
+000199c0: 536c 6f74 7465 6428 5461 626c 6553 6561  Slotted(TableSea
+000199d0: 7263 6854 6573 7473 2c20 5573 696e 6753  rchTests, UsingS
+000199e0: 6c6f 7474 6564 4f62 6a65 6374 7329 3a0a  lottedObjects):.
+000199f0: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
+00019a00: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+00019a10: 5f53 696d 706c 654e 616d 6573 7061 6365  _SimpleNamespace
+00019a20: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+00019a30: 732c 2055 7369 6e67 5369 6d70 6c65 4e61  s, UsingSimpleNa
+00019a40: 6d65 7370 6163 6529 3a0a 2020 2020 7061  mespace):.    pa
+00019a50: 7373 0a0a 6966 2064 6174 6163 6c61 7373  ss..if dataclass
+00019a60: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00019a70: 2020 2020 636c 6173 7320 5461 626c 6553      class TableS
+00019a80: 6561 7263 6854 6573 7473 5f44 6174 6163  earchTests_Datac
+00019a90: 6c61 7373 6573 2854 6162 6c65 5365 6172  lasses(TableSear
+00019aa0: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
+00019ab0: 7461 636c 6173 7365 7329 3a0a 2020 2020  taclasses):.    
+00019ac0: 2020 2020 7061 7373 0a0a 6966 2070 7964      pass..if pyd
+00019ad0: 616e 7469 6320 6973 206e 6f74 204e 6f6e  antic is not Non
+00019ae0: 653a 0a20 2020 2063 6c61 7373 2054 6162  e:.    class Tab
+00019af0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
+00019b00: 6461 6e74 6963 4d6f 6465 6c73 2854 6162  danticModels(Tab
+00019b10: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
+00019b20: 7369 6e67 5079 6461 6e74 6963 4d6f 6465  singPydanticMode
+00019b30: 6c29 3a0a 2020 2020 2020 2020 7061 7373  l):.        pass
+00019b40: 0a0a 2020 2020 636c 6173 7320 5461 626c  ..    class Tabl
+00019b50: 6553 6561 7263 6854 6573 7473 5f50 7964  eSearchTests_Pyd
+00019b60: 616e 7469 6349 6d6d 7574 6162 6c65 4d6f  anticImmutableMo
+00019b70: 6465 6c73 2854 6162 6c65 5365 6172 6368  dels(TableSearch
+00019b80: 5465 7374 732c 2055 7369 6e67 5079 6461  Tests, UsingPyda
+00019b90: 6e74 6963 496d 6d75 7461 626c 654d 6f64  nticImmutableMod
+00019ba0: 656c 293a 0a20 2020 2020 2020 2070 6173  el):.        pas
+00019bb0: 730a 0a20 2020 2063 6c61 7373 2054 6162  s..    class Tab
+00019bc0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
+00019bd0: 6461 6e74 6963 4f52 4d4d 6f64 656c 7328  danticORMModels(
+00019be0: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+00019bf0: 2c20 5573 696e 6750 7964 616e 7469 634f  , UsingPydanticO
+00019c00: 524d 4d6f 6465 6c29 3a0a 2020 2020 2020  RMModel):.      
+00019c10: 2020 7061 7373 0a0a 6966 2061 7474 7220    pass..if attr 
+00019c20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00019c30: 2063 6c61 7373 2054 6162 6c65 5365 6172   class TableSear
+00019c40: 6368 5465 7374 735f 4174 7472 436c 6173  chTests_AttrClas
+00019c50: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
+00019c60: 6573 7473 2c20 5573 696e 6741 7474 7243  ests, UsingAttrC
+00019c70: 6c61 7373 293a 0a20 2020 2020 2020 2070  lass):.        p
+00019c80: 6173 730a 0a69 6620 7472 6169 746c 6574  ass..if traitlet
+00019c90: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00019ca0: 2020 2063 6c61 7373 2054 6162 6c65 5365     class TableSe
+00019cb0: 6172 6368 5465 7374 735f 5472 6169 746c  archTests_Traitl
+00019cc0: 6574 7343 6c61 7373 6573 2854 6162 6c65  etsClasses(Table
+00019cd0: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+00019ce0: 6e67 5472 6169 746c 6574 7343 6c61 7373  ngTraitletsClass
+00019cf0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00019d00: 0a69 6620 536c 6f74 7465 6457 6974 6844  .if SlottedWithD
+00019d10: 6963 7420 6973 206e 6f74 204e 6f6e 653a  ict is not None:
+00019d20: 0a20 2020 2063 6c61 7373 2054 6162 6c65  .    class Table
+00019d30: 5365 6172 6368 5465 7374 735f 536c 6f74  SearchTests_Slot
+00019d40: 7465 6457 6974 6844 6963 7428 5461 626c  tedWithDict(Tabl
+00019d50: 6553 6561 7263 6854 6573 7473 2c20 5573  eSearchTests, Us
+00019d60: 696e 6753 6c6f 7474 6564 5769 7468 4469  ingSlottedWithDi
+00019d70: 6374 4f62 6a65 6374 7329 3a0a 2020 2020  ctObjects):.    
+00019d80: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+00019d90: 2049 6e69 7469 616c 5465 7374 2875 6e69   InitialTest(uni
+00019da0: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
+00019db0: 0a20 2020 2066 726f 6d20 6c69 7474 6c65  .    from little
+00019dc0: 7461 626c 6520 696d 706f 7274 2028 0a20  table import (. 
+00019dd0: 2020 2020 2020 205f 5f76 6572 7369 6f6e         __version
+00019de0: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
+00019df0: 655f 7665 7273 696f 6e2c 0a20 2020 2020  e_version,.     
+00019e00: 2020 205f 5f76 6572 7369 6f6e 5f74 696d     __version_tim
+00019e10: 655f 5f20 6173 206c 6974 746c 6574 6162  e__ as littletab
+00019e20: 6c65 5f76 6572 7369 6f6e 5f74 696d 652c  le_version_time,
+00019e30: 0a20 2020 2020 2020 205f 5f76 6572 7369  .        __versi
+00019e40: 6f6e 5f69 6e66 6f5f 5f20 6173 206c 6974  on_info__ as lit
+00019e50: 746c 6574 6162 6c65 5f76 6572 7369 6f6e  tletable_version
+00019e60: 5f69 6e66 6f2c 0a20 2020 2029 0a0a 2020  _info,.    )..  
+00019e70: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+00019e80: 2066 2242 6567 696e 6e69 6e67 2074 6573   f"Beginning tes
+00019e90: 7420 6f66 206c 6974 746c 6574 6162 6c65  t of littletable
+00019ea0: 2c20 7665 7273 696f 6e20 7b6c 6974 746c  , version {littl
+00019eb0: 6574 6162 6c65 5f76 6572 7369 6f6e 7d2c  etable_version},
+00019ec0: 207b 6c69 7474 6c65 7461 626c 655f 7665   {littletable_ve
+00019ed0: 7273 696f 6e5f 7469 6d65 7d22 2c0a 2020  rsion_time}",.  
+00019ee0: 2020 290a 2020 2020 7072 696e 7428 6c69    ).    print(li
+00019ef0: 7474 6c65 7461 626c 655f 7665 7273 696f  ttletable_versio
+00019f00: 6e5f 696e 666f 290a 2020 2020 7072 696e  n_info).    prin
+00019f10: 7428 2250 7974 686f 6e20 7665 7273 696f  t("Python versio
+00019f20: 6e22 2c20 7379 732e 7665 7273 696f 6e29  n", sys.version)
+00019f30: 0a20 2020 2070 7269 6e74 2829 0a0a 0a63  .    print()...c
+00019f40: 6c61 7373 2053 746f 7261 6765 496e 6465  lass StorageInde
+00019f50: 7065 6e64 656e 7454 6573 7473 2875 6e69  pendentTests(uni
+00019f60: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
+00019f70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+00019f80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+00019f90: 5f6e 6f72 6d61 6c69 7a65 5f73 7472 2873  _normalize_str(s
+00019fa0: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
+00019fb0: 7220 696e 5f77 6f72 642c 2065 7870 6563  r in_word, expec
+00019fc0: 7465 645f 776f 7264 2069 6e20 5b0a 2020  ted_word in [.  
+00019fd0: 2020 2020 2020 2020 2020 2822 6e6f 6368            ("noch
+00019fe0: 616e 6765 222c 2022 6e6f 6368 616e 6765  ange", "nochange
+00019ff0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0001a000: 2822 546f 4c6f 7765 7222 2c20 2274 6f6c  ("ToLower", "tol
+0001a010: 6f77 6572 2229 2c0a 2020 2020 2020 2020  ower"),.        
+0001a020: 2020 2020 2822 492e 422e 4d2e 222c 2022      ("I.B.M.", "
+0001a030: 6962 6d22 292c 0a20 2020 2020 2020 2020  ibm"),.         
+0001a040: 2020 2028 2247 2e45 2e22 2c20 2267 6522     ("G.E.", "ge"
+0001a050: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001a060: 224d 2e22 2c20 226d 2229 2c0a 2020 2020  "M.", "m"),.    
+0001a070: 2020 2020 2020 2020 2822 4d2e 7879 7a22          ("M.xyz"
+0001a080: 2c20 226d 2229 2c0a 2020 2020 2020 2020  , "m"),.        
+0001a090: 2020 2020 2822 2a78 7878 2d68 6868 222c      ("*xxx-hhh",
+0001a0a0: 2022 7878 782d 6868 6822 292c 0a20 2020   "xxx-hhh"),.   
+0001a0b0: 2020 2020 2020 2020 2028 222b 626c 6168           ("+blah
+0001a0c0: 466f 6f22 2c20 2262 6c61 6866 6f6f 2229  Foo", "blahfoo")
+0001a0d0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0001a0e0: 2822 666f 7865 7322 2c20 2266 6f78 2229  ("foxes", "fox")
+0001a0f0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0001a100: 2822 6368 7572 6368 6573 222c 2022 6368  ("churches", "ch
+0001a110: 7572 6368 2229 2c0a 2020 2020 2020 2020  urch"),.        
+0001a120: 2020 2020 2320 2822 6472 6573 7365 7322      # ("dresses"
+0001a130: 2c20 2264 7265 7373 2229 2c0a 2020 2020  , "dress"),.    
+0001a140: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
+0001a150: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0001a160: 5465 7374 2869 6e5f 776f 7264 293a 0a20  Test(in_word):. 
+0001a170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a180: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001a190: 6578 7065 6374 6564 5f77 6f72 642c 206c  expected_word, l
+0001a1a0: 742e 5461 626c 652e 5f6e 6f72 6d61 6c69  t.Table._normali
+0001a1b0: 7a65 5f77 6f72 6428 696e 5f77 6f72 6429  ze_word(in_word)
+0001a1c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001a1d0: 6e6f 726d 616c 697a 655f 7374 725f 6765  normalize_str_ge
+0001a1e0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+0001a1f0: 2066 6f72 2069 6e5f 776f 7264 2c20 6578   for in_word, ex
+0001a200: 7065 6374 6564 5f77 6f72 6473 2069 6e20  pected_words in 
+0001a210: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
+0001a220: 6e6f 6368 616e 6765 222c 205b 226e 6f63  nochange", ["noc
+0001a230: 6861 6e67 6522 5d29 2c0a 2020 2020 2020  hange"]),.      
+0001a240: 2020 2020 2020 2822 546f 4c6f 7765 7222        ("ToLower"
+0001a250: 2c20 5b22 746f 6c6f 7765 7222 5d29 2c0a  , ["tolower"]),.
+0001a260: 2020 2020 2020 2020 2020 2020 2822 492e              ("I.
+0001a270: 422e 4d2e 222c 205b 2269 2e62 2e6d 2e22  B.M.", ["i.b.m."
+0001a280: 2c20 2269 626d 225d 292c 0a20 2020 2020  , "ibm"]),.     
+0001a290: 2020 2020 2020 2028 2247 2e45 2e22 2c20         ("G.E.", 
+0001a2a0: 5b22 672e 652e 222c 2022 6765 225d 292c  ["g.e.", "ge"]),
+0001a2b0: 0a20 2020 2020 2020 2020 2020 2028 2241  .            ("A
+0001a2c0: 2e49 2e22 2c20 5b22 612e 692e 222c 2022  .I.", ["a.i.", "
+0001a2d0: 6169 225d 292c 0a20 2020 2020 2020 2020  ai"]),.         
+0001a2e0: 2020 2028 2241 4922 2c20 5b22 6169 225d     ("AI", ["ai"]
+0001a2f0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001a300: 224d 2e22 2c20 5b22 6d22 5d29 2c0a 2020  "M.", ["m"]),.  
+0001a310: 2020 2020 2020 2020 2020 2822 6d6d 2e78            ("mm.x
+0001a320: 797a 222c 205b 226d 6d22 2c20 226d 6d2e  yz", ["mm", "mm.
+0001a330: 7879 7a22 2c20 2278 797a 225d 292c 0a20  xyz", "xyz"]),. 
+0001a340: 2020 2020 2020 2020 2020 2028 224d 4d2e             ("MM.
+0001a350: 7879 7a22 2c20 5b22 6d6d 222c 2022 6d6d  xyz", ["mm", "mm
+0001a360: 2e78 797a 222c 2022 7879 7a22 5d29 2c0a  .xyz", "xyz"]),.
+0001a370: 2020 2020 2020 2020 2020 2020 2822 5468              ("Th
+0001a380: 7265 6164 696e 672e 6973 416c 6976 6528  reading.isAlive(
+0001a390: 2922 2c20 5b27 6973 616c 6976 6527 2c20  )", ['isalive', 
+0001a3a0: 2774 6872 6561 6469 6e67 272c 2027 7468  'threading', 'th
+0001a3b0: 7265 6164 696e 672e 6973 616c 6976 6527  reading.isalive'
+0001a3c0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001a3d0: 2822 2a78 7878 2d68 6868 222c 205b 2768  ("*xxx-hhh", ['h
+0001a3e0: 6868 272c 2027 7878 7827 2c20 2778 7878  hh', 'xxx', 'xxx
+0001a3f0: 2d68 6868 275d 292c 0a20 2020 2020 2020  -hhh']),.       
+0001a400: 2020 2020 2028 222b 626c 6168 466f 6f22       ("+blahFoo"
+0001a410: 2c20 5b22 626c 6168 666f 6f22 5d29 2c0a  , ["blahfoo"]),.
+0001a420: 2020 2020 2020 2020 2020 2020 2822 7374              ("st
+0001a430: 722e 6c73 7472 6970 222c 205b 226c 7374  r.lstrip", ["lst
+0001a440: 7269 7022 2c20 2273 7472 222c 2022 7374  rip", "str", "st
+0001a450: 722e 6c73 7472 6970 225d 292c 0a20 2020  r.lstrip"]),.   
+0001a460: 2020 2020 2020 2020 2028 2273 7472 2e6c           ("str.l
+0001a470: 7374 7269 7028 2922 2c20 5b22 6c73 7472  strip()", ["lstr
+0001a480: 6970 222c 2022 7374 7222 2c20 2273 7472  ip", "str", "str
+0001a490: 2e6c 7374 7269 7022 5d29 2c0a 2020 2020  .lstrip"]),.    
+0001a4a0: 2020 2020 2020 2020 2822 7365 6c66 2e61          ("self.a
+0001a4b0: 7373 6572 7445 7175 616c 7322 2c20 5b22  ssertEquals", ["
+0001a4c0: 6173 7365 7274 6571 7561 6c73 222c 2022  assertequals", "
+0001a4d0: 7365 6c66 222c 2022 7365 6c66 2e61 7373  self", "self.ass
+0001a4e0: 6572 7465 7175 616c 7322 5d29 2c0a 2020  ertequals"]),.  
+0001a4f0: 2020 2020 2020 2020 2020 2822 5465 7374            ("Test
+0001a500: 4361 7365 2e61 7373 6572 7445 7175 616c  Case.assertEqual
+0001a510: 7322 2c20 5b22 6173 7365 7274 6571 7561  s", ["assertequa
+0001a520: 6c73 222c 2022 7465 7374 6361 7365 222c  ls", "testcase",
+0001a530: 2022 7465 7374 6361 7365 2e61 7373 6572   "testcase.asser
+0001a540: 7465 7175 616c 7322 5d29 2c0a 2020 2020  tequals"]),.    
+0001a550: 2020 2020 2020 2020 2822 756e 6974 7465          ("unitte
+0001a560: 7374 2e54 6573 7443 6173 652e 6173 7365  st.TestCase.asse
+0001a570: 7274 4571 7561 6c73 222c 0a20 2020 2020  rtEquals",.     
+0001a580: 2020 2020 2020 2020 5b22 6173 7365 7274          ["assert
+0001a590: 6571 7561 6c73 222c 2022 7465 7374 6361  equals", "testca
+0001a5a0: 7365 222c 2022 756e 6974 7465 7374 222c  se", "unittest",
+0001a5b0: 2022 756e 6974 7465 7374 2e74 6573 7463   "unittest.testc
+0001a5c0: 6173 652e 6173 7365 7274 6571 7561 6c73  ase.assertequals
+0001a5d0: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
+0001a5e0: 2028 2266 6f78 6573 222c 205b 2266 6f78   ("foxes", ["fox
+0001a5f0: 222c 2022 666f 7865 7322 5d29 2c0a 2020  ", "foxes"]),.  
+0001a600: 2020 2020 2020 2020 2020 2822 6368 7572            ("chur
+0001a610: 6368 6573 222c 205b 2263 6875 7263 6822  ches", ["church"
+0001a620: 2c20 2263 6875 7263 6865 7322 5d29 2c0a  , "churches"]),.
+0001a630: 2020 2020 2020 2020 2020 2020 2822 6472              ("dr
+0001a640: 6573 7365 7322 2c20 5b22 6472 6573 7322  esses", ["dress"
+0001a650: 2c20 2264 7265 7373 6573 225d 292c 0a20  , "dresses"]),. 
+0001a660: 2020 2020 2020 2020 2020 2028 2264 7265             ("dre
+0001a670: 7373 222c 205b 2264 7265 7373 222c 205d  ss", ["dress", ]
+0001a680: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001a690: 2262 6961 7322 2c20 5b22 6269 6173 222c  "bias", ["bias",
+0001a6a0: 205d 292c 0a20 2020 2020 2020 2020 2020   ]),.           
+0001a6b0: 2028 2274 6f79 7322 2c20 5b22 746f 7922   ("toys", ["toy"
+0001a6c0: 2c20 2274 6f79 7322 5d29 2c0a 2020 2020  , "toys"]),.    
+0001a6d0: 2020 2020 2020 2020 2822 6261 6269 6573          ("babies
+0001a6e0: 222c 205b 2262 6162 6965 7322 2c20 2262  ", ["babies", "b
+0001a6f0: 6162 7922 5d29 2c0a 2020 2020 2020 2020  aby"]),.        
+0001a700: 2020 2020 2822 6164 6465 6e64 6122 2c20      ("addenda", 
+0001a710: 5b22 6164 6465 6e64 6122 2c20 2261 6464  ["addenda", "add
+0001a720: 656e 6475 6d22 5d29 2c0a 2020 2020 2020  endum"]),.      
+0001a730: 2020 2020 2020 2822 7261 6269 6573 222c        ("rabies",
+0001a740: 205b 2272 6162 6965 7322 5d29 2c0a 2020   ["rabies"]),.  
+0001a750: 2020 2020 2020 2020 2020 2822 6c61 7a69            ("lazi
+0001a760: 6e65 7373 222c 205b 226c 617a 696e 6573  ness", ["lazines
+0001a770: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
+0001a780: 2020 2822 7068 7973 6963 7322 2c20 5b22    ("physics", ["
+0001a790: 7068 7973 6963 7322 5d29 2c0a 2020 2020  physics"]),.    
+0001a7a0: 2020 2020 2020 2020 2822 5079 7468 6f6e          ("Python
+0001a7b0: 2773 222c 205b 2270 7974 686f 6e22 5d29  's", ["python"])
+0001a7c0: 2c0a 2020 2020 2020 2020 2020 2020 2827  ,.            ('
+0001a7d0: 5661 6c75 6545 7272 6f72 272c 205b 2765  ValueError', ['e
+0001a7e0: 7272 6f72 272c 2027 7661 6c75 6565 7272  rror', 'valueerr
+0001a7f0: 6f72 275d 292c 0a20 2020 2020 2020 2020  or']),.         
+0001a800: 2020 2028 2744 6570 7265 6361 7469 6f6e     ('Deprecation
+0001a810: 5761 726e 696e 6727 2c20 5b27 6465 7072  Warning', ['depr
+0001a820: 6563 6174 696f 6e77 6172 6e69 6e67 272c  ecationwarning',
+0001a830: 2027 7761 726e 696e 6727 5d29 2c0a 2020   'warning']),.  
+0001a840: 2020 2020 2020 2020 2020 2827 4375 7374            ('Cust
+0001a850: 6f6d 4578 6365 7074 696f 6e27 2c20 5b27  omException', ['
+0001a860: 6375 7374 6f6d 6578 6365 7074 696f 6e27  customexception'
+0001a870: 2c20 2765 7863 6570 7469 6f6e 275d 292c  , 'exception']),
+0001a880: 0a20 2020 2020 2020 205d 3a0a 2020 2020  .        ]:.    
+0001a890: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0001a8a0: 662e 7375 6254 6573 7428 696e 5f77 6f72  f.subTest(in_wor
+0001a8b0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+0001a8c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001a8d0: 7175 616c 2865 7870 6563 7465 645f 776f  qual(expected_wo
+0001a8e0: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
+0001a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a900: 2020 2020 2020 736f 7274 6564 286c 6973        sorted(lis
+0001a910: 7428 6c74 2e54 6162 6c65 2e5f 6e6f 726d  t(lt.Table._norm
+0001a920: 616c 697a 655f 776f 7264 5f67 656e 2869  alize_word_gen(i
+0001a930: 6e5f 776f 7264 2c20 6672 6f7a 656e 7365  n_word, frozense
+0001a940: 7428 2929 2929 290a 0a20 2020 2040 616e  t()))))..    @an
+0001a950: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+0001a960: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
+0001a970: 7a65 5f73 706c 6974 2873 656c 6629 3a0a  ze_split(self):.
+0001a980: 2020 2020 2020 2020 666f 7220 696e 5f73          for in_s
+0001a990: 7472 2c20 6578 7065 6374 6564 5f73 7472  tr, expected_str
+0001a9a0: 5f73 6574 2069 6e20 5b0a 2020 2020 2020  _set in [.      
+0001a9b0: 2020 2020 2020 2822 7374 722e 6c73 7472        ("str.lstr
+0001a9c0: 6970 2829 222c 205b 226c 7374 7269 7022  ip()", ["lstrip"
+0001a9d0: 2c20 2273 7472 222c 2022 7374 722e 6c73  , "str", "str.ls
+0001a9e0: 7472 6970 225d 292c 0a20 2020 2020 2020  trip"]),.       
+0001a9f0: 2020 2020 2028 2273 7472 2e6c 7374 7269       ("str.lstri
+0001aa00: 7028 2920 7374 722e 7273 7472 6970 2829  p() str.rstrip()
+0001aa10: 222c 205b 226c 7374 7269 7022 2c20 2272  ", ["lstrip", "r
+0001aa20: 7374 7269 7022 2c20 2273 7472 222c 2022  strip", "str", "
+0001aa30: 7374 722e 6c73 7472 6970 222c 2022 7374  str.lstrip", "st
+0001aa40: 722e 7273 7472 6970 225d 292c 0a20 2020  r.rstrip"]),.   
+0001aa50: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
+0001aa60: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+0001aa70: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
+0001aa80: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
+0001aa90: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
+0001aaa0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001aab0: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
+0001aac0: 5f73 7472 293a 0a20 2020 2020 2020 2020  _str):.         
+0001aad0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001aae0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0001aaf0: 5f73 7472 5f73 6574 2c0a 2020 2020 2020  _str_set,.      
+0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab10: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0001ab20: 6428 7365 7428 6c74 2e54 6162 6c65 2e5f  d(set(lt.Table._
+0001ab30: 6e6f 726d 616c 697a 655f 7370 6c69 7428  normalize_split(
+0001ab40: 696e 5f73 7472 2929 2929 0a0a 2020 2020  in_str))))..    
+0001ab50: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+0001ab60: 2020 2064 6566 2074 6573 745f 706c 7572     def test_plur
+0001ab70: 616c 735f 7769 7468 5f74 7261 696c 696e  als_with_trailin
+0001ab80: 675f 7075 6e63 7475 6174 696f 6e28 7365  g_punctuation(se
+0001ab90: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
+0001aba0: 2028 6c69 6e65 2c20 6578 7065 6374 6564   (line, expected
+0001abb0: 2920 696e 205b 0a20 2020 2020 2020 2020  ) in [.         
+0001abc0: 2020 2028 2749 2063 6f75 6c64 2068 6561     ('I could hea
+0001abd0: 7220 7468 6520 6261 6269 6573 2063 7269  r the babies cri
+0001abe0: 6573 2e27 2c20 5b27 6261 6269 6573 272c  es.', ['babies',
+0001abf0: 2027 6261 6279 272c 2027 636f 756c 6427   'baby', 'could'
+0001ac00: 2c20 2763 7269 6573 272c 2027 6372 7927  , 'cries', 'cry'
+0001ac10: 2c20 2768 6561 7227 2c20 2769 272c 2027  , 'hear', 'i', '
+0001ac20: 7468 6527 5d29 2c0a 2020 2020 2020 2020  the']),.        
+0001ac30: 2020 2020 2827 5768 6f20 6172 6520 7468      ('Who are th
+0001ac40: 6f73 6520 6261 6269 6573 3f27 2c20 5b27  ose babies?', ['
+0001ac50: 6172 6527 2c20 2762 6162 6965 7327 2c20  are', 'babies', 
+0001ac60: 2762 6162 7927 2c20 2774 686f 7365 272c  'baby', 'those',
+0001ac70: 2027 7768 6f27 5d29 2c0a 2020 2020 2020   'who']),.      
+0001ac80: 2020 2020 2020 2822 5768 6f20 746f 6f6b        ("Who took
+0001ac90: 2074 6865 2062 6162 6965 7327 2072 6174   the babies' rat
+0001aca0: 746c 6573 2074 6869 7320 7469 6d65 3f22  tles this time?"
+0001acb0: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
+0001acc0: 2762 6162 6965 7327 2c20 2762 6162 7927  'babies', 'baby'
+0001acd0: 2c20 2772 6174 746c 6527 2c20 2772 6174  , 'rattle', 'rat
+0001ace0: 746c 6573 272c 2027 7468 6527 2c20 2774  tles', 'the', 't
+0001acf0: 6869 7327 2c20 2774 696d 6527 2c20 2774  his', 'time', 't
+0001ad00: 6f6f 6b27 2c20 2777 686f 275d 292c 0a20  ook', 'who']),. 
+0001ad10: 2020 2020 2020 2020 2020 2028 2749 206c             ('I l
+0001ad20: 6f76 6520 7468 6573 6520 6361 6b65 7321  ove these cakes!
+0001ad30: 272c 205b 2763 616b 6527 2c20 2763 616b  ', ['cake', 'cak
+0001ad40: 6573 272c 2027 6927 2c20 276c 6f76 6527  es', 'i', 'love'
+0001ad50: 2c20 2774 6865 7365 275d 292c 0a20 2020  , 'these']),.   
+0001ad60: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
+0001ad70: 6d79 2077 6966 6520 636f 6f6b 732c 2073  my wife cooks, s
+0001ad80: 6865 2062 616b 6573 2e27 2c20 5b27 6261  he bakes.', ['ba
+0001ad90: 6b65 272c 2027 6261 6b65 7327 2c20 2763  ke', 'bakes', 'c
+0001ada0: 6f6f 6b27 2c20 2763 6f6f 6b73 272c 2027  ook', 'cooks', '
+0001adb0: 6d79 272c 2027 7368 6527 2c20 2777 6865  my', 'she', 'whe
+0001adc0: 6e27 2c20 2777 6966 6527 5d29 2c0a 2020  n', 'wife']),.  
+0001add0: 2020 2020 2020 2020 2020 2822 4c65 7427            ("Let'
+0001ade0: 7320 676f 2073 686f 7070 696e 6720 666f  s go shopping fo
+0001adf0: 7220 616e 7469 7175 6573 2122 2c20 5b27  r antiques!", ['
+0001ae00: 616e 7469 7175 6527 2c20 2761 6e74 6971  antique', 'antiq
+0001ae10: 7565 7327 2c20 2766 6f72 272c 2027 676f  ues', 'for', 'go
+0001ae20: 272c 2027 6c65 7427 2c20 2773 686f 7070  ', 'let', 'shopp
+0001ae30: 696e 6727 5d29 2c0a 2020 2020 2020 2020  ing']),.        
+0001ae40: 2020 2020 2827 5468 6973 2069 7320 616e      ('This is an
+0001ae50: 2061 6e74 6971 7565 2076 6173 652c 2077   antique vase, w
+0001ae60: 6f72 7468 2074 686f 7573 616e 6473 2127  orth thousands!'
+0001ae70: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
+0001ae80: 2761 6e27 2c20 2761 6e74 6971 7565 272c  'an', 'antique',
+0001ae90: 2027 6973 272c 2027 7468 6973 272c 2027   'is', 'this', '
+0001aea0: 7468 6f75 7361 6e64 272c 2027 7468 6f75  thousand', 'thou
+0001aeb0: 7361 6e64 7327 2c20 2776 6173 6527 2c20  sands', 'vase', 
+0001aec0: 2777 6f72 7468 275d 292c 0a20 2020 2020  'worth']),.     
+0001aed0: 2020 2020 2020 2028 2757 6865 6e20 7765         ('When we
+0001aee0: 206d 6565 742c 2079 6f75 2061 7265 2061   meet, you are a
+0001aef0: 2067 6961 6e74 2061 6d6f 6e67 206d 656e   giant among men
+0001af00: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+0001af10: 205b 2761 272c 2027 616d 6f6e 6727 2c20   ['a', 'among', 
+0001af20: 2761 7265 272c 2027 6769 616e 7427 2c20  'are', 'giant', 
+0001af30: 276d 616e 272c 2027 6d65 6574 272c 2027  'man', 'meet', '
+0001af40: 6d65 6e27 2c20 2777 6527 2c20 2777 6865  men', 'we', 'whe
+0001af50: 6e27 2c20 2779 6f75 275d 292c 0a20 2020  n', 'you']),.   
+0001af60: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
+0001af70: 7765 2061 7265 2061 6d6f 6e67 206d 656e  we are among men
+0001af80: 2c20 796f 7520 6172 6520 6120 6769 616e  , you are a gian
+0001af90: 7420 6d65 6174 6261 6c6c 2e27 2c0a 2020  t meatball.',.  
+0001afa0: 2020 2020 2020 2020 2020 205b 2761 272c             ['a',
+0001afb0: 2027 616d 6f6e 6727 2c20 2761 7265 272c   'among', 'are',
+0001afc0: 2027 6172 6527 2c20 2767 6961 6e74 272c   'are', 'giant',
+0001afd0: 2027 6d61 6e27 2c20 276d 6561 7462 616c   'man', 'meatbal
+0001afe0: 6c27 2c20 276d 656e 272c 2027 7765 272c  l', 'men', 'we',
+0001aff0: 2027 7768 656e 272c 2027 796f 7527 5d29   'when', 'you'])
+0001b000: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+0001b010: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+0001b020: 6c66 2e73 7562 5465 7374 286c 696e 6529  lf.subTest(line)
+0001b030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b040: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001b050: 616c 2865 7870 6563 7465 642c 2073 6f72  al(expected, sor
+0001b060: 7465 6428 6c74 2e54 6162 6c65 2e5f 6e6f  ted(lt.Table._no
+0001b070: 726d 616c 697a 655f 7370 6c69 7428 6c69  rmalize_split(li
+0001b080: 6e65 2929 290a 0a0a 6966 205f 5f6e 616d  ne)))...if __nam
+0001b090: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
+0001b0a0: 273a 0a20 2020 2075 6e69 7474 6573 742e  ':.    unittest.
+0001b0b0: 6d61 696e 2829 0a                        main().
```

