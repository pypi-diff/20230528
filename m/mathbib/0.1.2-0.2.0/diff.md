# Comparing `tmp/mathbib-0.1.2.tar.gz` & `tmp/mathbib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.1.2.tar", last modified: Sun May 28 15:55:31 2023, max compression
+gzip compressed data, was "mathbib-0.2.0.tar", last modified: Sun May 28 17:11:31 2023, max compression
```

## Comparing `mathbib-0.1.2.tar` & `mathbib-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.685167 mathbib-0.1.2/
--rw-r--r--   0 alexrutar   (501) staff       (20)       51 2023-05-25 15:29:52.000000 mathbib-0.1.2/MANIFEST.in
--rw-r--r--   0 alexrutar   (501) staff       (20)     5815 2023-05-28 15:55:31.685499 mathbib-0.1.2/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     5354 2023-05-28 15:53:57.000000 mathbib-0.1.2/README.md
--rw-r--r--   0 alexrutar   (501) staff       (20)      318 2023-05-10 21:34:37.000000 mathbib-0.1.2/pyproject.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)     1023 2023-05-28 15:55:31.686635 mathbib-0.1.2/setup.cfg
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.666445 mathbib-0.1.2/src/
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.671730 mathbib-0.1.2/src/mathbib/
--rw-r--r--   0 alexrutar   (501) staff       (20)      217 2023-05-28 15:42:16.000000 mathbib-0.1.2/src/mathbib/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 21:47:55.000000 mathbib-0.1.2/src/mathbib/__main__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1402 2023-05-28 11:08:27.000000 mathbib-0.1.2/src/mathbib/bibtex.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2831 2023-05-28 15:54:03.000000 mathbib-0.1.2/src/mathbib/citegen.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9936 2023-05-28 15:54:03.000000 mathbib-0.1.2/src/mathbib/command.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2632 2023-05-28 15:08:09.000000 mathbib-0.1.2/src/mathbib/partition.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9459 2023-05-28 15:11:22.000000 mathbib-0.1.2/src/mathbib/record.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.679612 mathbib-0.1.2/src/mathbib/remote/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5481 2023-05-28 13:40:33.000000 mathbib-0.1.2/src/mathbib/remote/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     3088 2023-05-28 12:38:27.000000 mathbib-0.1.2/src/mathbib/remote/arxiv.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      923 2023-05-27 20:04:18.000000 mathbib-0.1.2/src/mathbib/remote/doi.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      855 2023-05-28 09:33:03.000000 mathbib-0.1.2/src/mathbib/remote/error.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1475 2023-05-27 20:04:18.000000 mathbib-0.1.2/src/mathbib/remote/isbn.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1194 2023-05-27 18:35:57.000000 mathbib-0.1.2/src/mathbib/remote/ol.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     4257 2023-05-28 15:10:12.000000 mathbib-0.1.2/src/mathbib/remote/utils.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      597 2023-05-25 12:11:18.000000 mathbib-0.1.2/src/mathbib/remote/zbl.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1816 2023-05-28 12:19:04.000000 mathbib-0.1.2/src/mathbib/remote/zbmath.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5552 2023-05-28 12:31:57.000000 mathbib-0.1.2/src/mathbib/request.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.680701 mathbib-0.1.2/src/mathbib/resources/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2023-05-25 15:24:07.000000 mathbib-0.1.2/src/mathbib/resources/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)   270192 2023-05-25 15:19:42.000000 mathbib-0.1.2/src/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0 alexrutar   (501) staff       (20)     2613 2023-05-28 12:14:16.000000 mathbib-0.1.2/src/mathbib/session.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      705 2023-05-25 11:53:39.000000 mathbib-0.1.2/src/mathbib/term.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.674636 mathbib-0.1.2/src/mathbib.egg-info/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5815 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)      835 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/SOURCES.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/dependency_links.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       45 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/entry_points.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)      131 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/requires.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        8 2023-05-28 15:55:31.000000 mathbib-0.1.2/src/mathbib.egg-info/top_level.txt
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 15:55:31.684031 mathbib-0.1.2/test/
--rw-r--r--   0 alexrutar   (501) staff       (20)      719 2023-05-27 20:04:18.000000 mathbib-0.1.2/test/test_partition.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.757627 mathbib-0.2.0/
+-rw-r--r--   0 alexrutar   (501) staff       (20)       51 2023-05-25 15:29:52.000000 mathbib-0.2.0/MANIFEST.in
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5818 2023-05-28 17:11:31.757848 mathbib-0.2.0/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5354 2023-05-28 15:53:57.000000 mathbib-0.2.0/README.md
+-rw-r--r--   0 alexrutar   (501) staff       (20)      318 2023-05-10 21:34:37.000000 mathbib-0.2.0/pyproject.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1026 2023-05-28 17:11:31.759044 mathbib-0.2.0/setup.cfg
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.738276 mathbib-0.2.0/src/
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.743960 mathbib-0.2.0/src/mathbib/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      220 2023-05-28 17:10:17.000000 mathbib-0.2.0/src/mathbib/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 21:47:55.000000 mathbib-0.2.0/src/mathbib/__main__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1402 2023-05-28 11:08:27.000000 mathbib-0.2.0/src/mathbib/bibtex.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2831 2023-05-28 15:54:03.000000 mathbib-0.2.0/src/mathbib/citegen.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     9963 2023-05-28 16:57:04.000000 mathbib-0.2.0/src/mathbib/command.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2841 2023-05-28 16:33:13.000000 mathbib-0.2.0/src/mathbib/partition.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     9459 2023-05-28 15:11:22.000000 mathbib-0.2.0/src/mathbib/record.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.751658 mathbib-0.2.0/src/mathbib/remote/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5481 2023-05-28 13:40:33.000000 mathbib-0.2.0/src/mathbib/remote/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     3088 2023-05-28 12:38:27.000000 mathbib-0.2.0/src/mathbib/remote/arxiv.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      923 2023-05-27 20:04:18.000000 mathbib-0.2.0/src/mathbib/remote/doi.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      855 2023-05-28 09:33:03.000000 mathbib-0.2.0/src/mathbib/remote/error.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1475 2023-05-27 20:04:18.000000 mathbib-0.2.0/src/mathbib/remote/isbn.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1194 2023-05-27 18:35:57.000000 mathbib-0.2.0/src/mathbib/remote/ol.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4257 2023-05-28 15:10:12.000000 mathbib-0.2.0/src/mathbib/remote/utils.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      597 2023-05-25 12:11:18.000000 mathbib-0.2.0/src/mathbib/remote/zbl.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1816 2023-05-28 12:19:04.000000 mathbib-0.2.0/src/mathbib/remote/zbmath.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5552 2023-05-28 12:31:57.000000 mathbib-0.2.0/src/mathbib/request.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.752581 mathbib-0.2.0/src/mathbib/resources/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2023-05-25 15:24:07.000000 mathbib-0.2.0/src/mathbib/resources/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)   270192 2023-05-25 15:19:42.000000 mathbib-0.2.0/src/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0 alexrutar   (501) staff       (20)     2613 2023-05-28 12:14:16.000000 mathbib-0.2.0/src/mathbib/session.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)      705 2023-05-25 11:53:39.000000 mathbib-0.2.0/src/mathbib/term.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.747002 mathbib-0.2.0/src/mathbib.egg-info/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5818 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)      835 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/SOURCES.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/dependency_links.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       45 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/entry_points.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)      131 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/requires.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        8 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/top_level.txt
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.755687 mathbib-0.2.0/test/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      719 2023-05-27 20:04:18.000000 mathbib-0.2.0/test/test_partition.py
```

### Comparing `mathbib-0.1.2/PKG-INFO` & `mathbib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.1.2
+Version: 0.2.0
 Summary: A mathematics BibLaTeX bibliography manager.
-Home-page: https://github.com/alexrutar/mathbib
+Home-page: https://github.com/alexrutar/mathbib-py
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
```

### Comparing `mathbib-0.1.2/README.md` & `mathbib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/setup.cfg` & `mathbib-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = mathbib
 version = attr: mathbib.__version__
 author = Alex Rutar
 author_email = alex@rutar.org
 description = A mathematics BibLaTeX bibliography manager.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/alexrutar/mathbib
+url = https://github.com/alexrutar/mathbib-py
 classifiers = 
 	Development Status :: 3 - Alpha
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
```

### Comparing `mathbib-0.1.2/src/mathbib/bibtex.py` & `mathbib-0.2.0/src/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/citegen.py` & `mathbib-0.2.0/src/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/command.py` & `mathbib-0.2.0/src/mathbib/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,17 +97,15 @@
 
 
 @cli.command(short_help="Generate citations from keys in file.")
 @texfile_argument
 @click.option(
     "--out",
     "out",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, writable=True, path_type=Path
-    ),
+    type=click.Path(file_okay=True, dir_okay=False, writable=True, path_type=Path),
     help="Output file path.",
 )
 @click.pass_context
 def generate(ctx: click.Context, texfile: Iterable[Path], out: Optional[Path]):
     """Parse TEXFILE and generate bibtex entries corresponding to keys.
     If option --out is specified, write generated text to the given file.
     """
@@ -169,30 +167,14 @@
         click.launch(str(download_file))
         return
 
     # if there is no file, try to download it
     raise click.ClickException("Could not find associated file.")
 
 
-@file_group.command(name="list", short_help="List all files.")
-@click.pass_obj
-def file_list(session: CLISession):
-    """List all the files saved on your device, along with the corresponding"""
-    root = xdg_data_home() / "mathbib" / "files"
-    for pat in (xdg_data_home() / "mathbib" / "files").glob("**/*.pdf"):
-        key = pat.relative_to(root).parents[-2]
-        val = pat.relative_to(root / key).with_suffix("")
-        record = ArchiveRecord.from_str(f"{key}:{val}", session).as_bibtex()
-        click.echo(record["ID"], nl=False)
-        for src in ("author", "title"):
-            if src in record.keys():
-                click.echo(" - " + record[src], nl=False)
-        click.echo()
-
-
 # TODO: add --force to overwrite manually
 @file_group.command(name="add", short_help="Add new file for record.")
 @record_argument
 @click.argument(
     "source",
     type=click.Path(exists=True, file_okay=True, dir_okay=False, path_type=Path),
     metavar="PDF",
@@ -306,7 +288,35 @@
             for k, v in session.alias.items()
             if k in get_citekeys_from_paths(*key_sources)
         }
     else:
         alias_dict = session.alias
 
     click.echo(dumps(alias_dict), nl=False)
+
+
+@cli.command(name="list", short_help="List all records.")
+@click.option(
+    "--sep",
+    "sep",
+    type=str,
+    default=" - ",
+    help="Separator for titles.",
+)
+@click.pass_obj
+def list_cmd(session: CLISession, sep: str):
+    """List all records. The records are printed in the format"""
+    for keyid in session.relations.iter_canonical():
+        record = ArchiveRecord(
+            AliasedKeyId(keyid.key, keyid.identifier), session
+        ).as_bibtex()
+        click.echo(
+            sep.join(
+                str(elem)
+                for elem in (
+                    keyid,
+                    record.get("author"),
+                    record.get("year"),
+                    record.get("title"),
+                )
+            )
+        )
```

### Comparing `mathbib-0.1.2/src/mathbib/partition.py` & `mathbib-0.2.0/src/mathbib/partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Iterable
+
 import json
 
 from .remote import KeyId
 
 
 class Partition:
     """This is a class which defines a partition of a set of objects.
@@ -11,14 +17,17 @@
         self._dict: dict[KeyId, list[KeyId]] = {}
         self._lookup: dict[KeyId, KeyId] = {}
 
     def canonical(self, elem: KeyId) -> KeyId:
         """Get the canonical record associated with an element."""
         return self._lookup[elem]
 
+    def iter_canonical(self) -> Iterable[KeyId]:
+        return iter(self._dict.keys())
+
     def related(self, elem: KeyId) -> list[KeyId]:
         """Get the canonical record associated with an element."""
         return self._dict[self._lookup[elem]]
 
     def add(self, *elements: KeyId):
         """Add all possible new relations between elements."""
```

### Comparing `mathbib-0.1.2/src/mathbib/record.py` & `mathbib-0.2.0/src/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/__init__.py` & `mathbib-0.2.0/src/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/arxiv.py` & `mathbib-0.2.0/src/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/doi.py` & `mathbib-0.2.0/src/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/error.py` & `mathbib-0.2.0/src/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/isbn.py` & `mathbib-0.2.0/src/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/ol.py` & `mathbib-0.2.0/src/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/utils.py` & `mathbib-0.2.0/src/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/zbl.py` & `mathbib-0.2.0/src/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/remote/zbmath.py` & `mathbib-0.2.0/src/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/request.py` & `mathbib-0.2.0/src/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/resources/journal_abbrevs.json` & `mathbib-0.2.0/src/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/session.py` & `mathbib-0.2.0/src/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib/term.py` & `mathbib-0.2.0/src/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/src/mathbib.egg-info/PKG-INFO` & `mathbib-0.2.0/src/mathbib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.1.2
+Version: 0.2.0
 Summary: A mathematics BibLaTeX bibliography manager.
-Home-page: https://github.com/alexrutar/mathbib
+Home-page: https://github.com/alexrutar/mathbib-py
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
```

### Comparing `mathbib-0.1.2/src/mathbib.egg-info/SOURCES.txt` & `mathbib-0.2.0/src/mathbib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathbib-0.1.2/test/test_partition.py` & `mathbib-0.2.0/test/test_partition.py`

 * *Files identical despite different names*

