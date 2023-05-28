# Comparing `tmp/littletable-2.2.1.tar.gz` & `tmp/littletable-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littletable-2.2.1.tar", last modified: Sun May 28 19:09:44 2023, max compression
+gzip compressed data, was "littletable-2.2.2.tar", last modified: Sun May 28 19:24:44 2023, max compression
```

## Comparing `littletable-2.2.1.tar` & `littletable-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:09:44.856880 littletable-2.2.1/
--rw-rw-r--   0 paul      (1000) paul      (1000)    36556 2023-05-28 19:07:07.000000 littletable-2.2.1/CHANGES
--rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.1/HowToUseLittletable.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.1/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.1/MANIFEST.in
--rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:09:44.856880 littletable-2.2.1/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.1/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:09:44.856880 littletable-2.2.1/littletable.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-05-28 19:09:44.000000 littletable-2.2.1/littletable.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)   163325 2023-05-28 19:07:07.000000 littletable-2.2.1/littletable.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-05-28 19:09:44.856880 littletable-2.2.1/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.1/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)   110775 2023-05-28 19:07:07.000000 littletable-2.2.1/unit_tests.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:24:44.237011 littletable-2.2.2/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    36660 2023-05-28 19:24:38.000000 littletable-2.2.2/CHANGES
+-rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.2/HowToUseLittletable.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.2/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.2/MANIFEST.in
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:24:44.237011 littletable-2.2.2/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.2/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:24:44.237011 littletable-2.2.2/littletable.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)   163352 2023-05-28 19:24:38.000000 littletable-2.2.2/littletable.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-05-28 19:24:44.237011 littletable-2.2.2/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.2/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)   110775 2023-05-28 19:07:07.000000 littletable-2.2.2/unit_tests.py
```

### Comparing `littletable-2.2.1/CHANGES` & `littletable-2.2.2/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 NOTE: Deprecated features will be removed in the 3.0 release of littletable:
 - DataObject class, replace with typing.SimpleNamespace, dict, namedtuple, or
   other user-defined class
 - Table.re_match(patt) comparator is deprecated, replace with
   re.compile(patt).match
 
+Version 2.2.2
+-------------
+- Fixed bug using datetime.UTC (only available under Python 3.11 - sorry!)
+
 
 Version 2.2.1
 -------------
 - Rewrote handling of multiple custom `JSONEncoder`s to use multiple
   inheritance instead of explicit call chaining.
 
 - 20-30% performance speedup when creating a search index.
```

### Comparing `littletable-2.2.1/LICENSE` & `littletable-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `littletable-2.2.1/PKG-INFO` & `littletable-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Download-URL: https://pypi.org/project/littletable/
 Platform: UNKNOWN
```

### Comparing `littletable-2.2.1/README.md` & `littletable-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `littletable-2.2.1/littletable.egg-info/PKG-INFO` & `littletable-2.2.2/littletable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Download-URL: https://pypi.org/project/littletable/
 Platform: UNKNOWN
```

### Comparing `littletable-2.2.1/littletable.py` & `littletable-2.2.2/littletable.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,22 +153,22 @@
     import rich
     from rich import box
 except ImportError:
     rich = None
     box = None
 
 version_info = namedtuple("version_info", "major minor micro release_level serial")
-__version_info__ = version_info(2, 2, 1, "final", 0)
+__version_info__ = version_info(2, 2, 2, "final", 0)
 __version__ = (
     "{}.{}.{}".format(*__version_info__[:3])
     + (f"{__version_info__.release_level[0]}{__version_info__.serial}", "")[
         __version_info__.release_level == "final"
     ]
 )
-__version_time__ = "28 May 2023 18:46 UTC"
+__version_time__ = "28 May 2023 19:19 UTC"
 __author__ = "Paul McGuire <ptmcg@austin.rr.com>"
 
 
 # custom Exception classes
 class SearchIndexInconsistentError(Exception):
     """
     Exception raised when using search method on table that has been
@@ -1126,15 +1126,15 @@
         self._uniqueIndexes: list[_UniqueObjIndex] = []
         self._search_indexes: dict[str, dict[str, list]] = {}
 
         self.import_source_type: Optional[ImportSourceType] = None
         self.import_source: Optional[str] = None
 
         self.import_time = None
-        self.create_time = datetime.datetime.now().astimezone(datetime.UTC)
+        self.create_time = datetime.datetime.now().astimezone(datetime.timezone.utc)
         self.modify_time = self.create_time
 
         """
         C{'by'} is added as a pseudo-attribute on tables, to provide
         dict-like access to the underlying records in the table by index key, as in::
 
             employees.by.socsecnum["000-00-0000"]
@@ -1845,15 +1845,15 @@
         """
         Internal method to be called whenever the contents of a table are modified.
         """
         if invalidate_search_indexes:
             for idx in self._search_indexes.values():
                 idx["VALID"] = False
 
-        self.modify_time = datetime.datetime.now().astimezone(datetime.UTC)
+        self.modify_time = datetime.datetime.now().astimezone(datetime.timezone.utc)
 
     def _query_attr_sort_fn(self, attr_val: tuple[str, Any]) -> int:
         """Used to order where keys by most selective key first"""
         attr, v = attr_val
         if attr in self._indexes:
             idx = self._indexes[attr]
             if v in idx:
@@ -2567,15 +2567,15 @@
                                            ):
                 # if url, strip off query args if any
                 if self.import_source_type is ImportSourceType.url:
                     source = str(source).partition("?")[0]
                 self.import_source = str(source)
                 self(str(source))
 
-        self.import_time = datetime.datetime.now().astimezone(datetime.UTC)
+        self.import_time = datetime.datetime.now().astimezone(datetime.timezone.utc)
         self._contents_changed()
         return self
 
     def csv_import(
         self,
         csv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
```

### Comparing `littletable-2.2.1/setup.py` & `littletable-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `littletable-2.2.1/unit_tests.py` & `littletable-2.2.2/unit_tests.py`

 * *Files identical despite different names*

