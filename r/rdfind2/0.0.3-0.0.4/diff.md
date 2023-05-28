# Comparing `tmp/rdfind2-0.0.3.tar.gz` & `tmp/rdfind2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.3.tar", last modified: Sun May 28 00:50:31 2023, max compression
+gzip compressed data, was "rdfind2-0.0.4.tar", last modified: Sun May 28 01:20:56 2023, max compression
```

## Comparing `rdfind2-0.0.3.tar` & `rdfind2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:50:31.197345 rdfind2-0.0.3/
--rw-rw-rw-   0        0        0     1008 2023-05-28 00:50:31.197345 rdfind2-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-28 00:50:15.000000 rdfind2-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 00:50:31.195343 rdfind2-0.0.3/rdfind2.egg-info/
--rw-rw-rw-   0        0        0     1008 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7269 2023-05-28 00:49:15.000000 rdfind2-0.0.3/rdfind2.py
--rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.3/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 00:50:31.197345 rdfind2-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 01:20:56.237944 rdfind2-0.0.4/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 01:20:56.236942 rdfind2-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-28 01:20:39.000000 rdfind2-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-28 01:20:56.235941 rdfind2-0.0.4/rdfind2.egg-info/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7506 2023-05-28 01:20:29.000000 rdfind2-0.0.4/rdfind2.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.4/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 01:20:56.237944 rdfind2-0.0.4/setup.cfg
```

### Comparing `rdfind2-0.0.3/PKG-INFO` & `rdfind2-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rdfind2-0.0.3/pyproject.toml` & `rdfind2-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdfind2"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "trim21", email = "trim21.me@gmail.com" },
 ]
 description = "Find duplicated files very fast"
 readme = "readme.md"
 requires-python = ">=3.8,<4"
 license = { text = "MIT" }
```

### Comparing `rdfind2-0.0.3/rdfind2.egg-info/PKG-INFO` & `rdfind2-0.0.4/rdfind2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rdfind2-0.0.3/rdfind2.py` & `rdfind2-0.0.4/rdfind2.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pathlib
 from collections import defaultdict
 from typing import Dict, Iterable, List, Optional, Tuple
 
 import click
 from tqdm import tqdm
 
+
 PROGRESS_SIZE = 128 * 1024 * 1024  # 512M
 CHUNK_SIZE = 16 * 1024  # 16k
 PARTIAL_SIZE = 16
 
 
 @dataclasses.dataclass
 class Entry:
@@ -78,15 +79,15 @@
     def check_key(self) -> tuple:
         return self.size, self.head, self.middle, self.tail
 
     @staticmethod
     def read_partial(p: pathlib.Path, size: int) -> Tuple[bytes, bytes, bytes]:
         with p.open("rb", buffering=0) as f:
             head = f.read(PARTIAL_SIZE)
-            f.seek(int(size / 2), io.SEEK_SET)
+            f.seek(size // 2, io.SEEK_SET)
             middle = f.read(PARTIAL_SIZE)
             f.seek(-min(PARTIAL_SIZE, size), io.SEEK_END)
             tail = f.read(PARTIAL_SIZE)
         return head, middle, tail
 
 
 @click.command()
@@ -110,52 +111,57 @@
 
     for _, headGroups in sorted(groups.items(), reverse=True):
         if len(headGroups) == 1:
             continue
 
         entry_groups.append(headGroups)
 
+    click.secho("check file hashed", fg='cyan')
     for entry_group in tqdm(entry_groups, ascii=True, position=0):
         entry_grouped = compare_groups(entry_group)
         for g in entry_grouped:
             if len(g) == 1:
                 continue
 
             if hardlink:
                 tqdm.write("link files:")
-                for file in g:
-                    tqdm.write(click.style(f"{file.path!s}", fg="red"))
 
                 link_src = g.pop()
+                tqdm.write(click.style(f"hard link target file {link_src.path!r}", fg="green"))
+                for file in g:
+                    tqdm.write(click.style(f"{file.path!s}", fg="red"))
 
                 for file in g:
                     if link_src.inode == file.inode:
                         continue
                     if file.path.name.endswith(".rdfind2.old"):
-                        tqdm.write(click.style(f"find internal temp file {file.path}", fg="red"))
+                        tqdm.write(click.style(f"find internal temp file {file.path!r}", fg="red"))
                         continue
                     temp_file_path = pathlib.Path(
                         file.path.with_name(file.path.name + ".rdfind2.old")
                     )
                     file.path.rename(temp_file_path)
                     os.link(src=link_src.path, dst=file.path)
                     temp_file_path.unlink()
 
             elif delete:
-                g.pop()
+                link_src = g.pop()
+                tqdm.write(click.style(f"find internal temp file {link_src.path}", fg="green"))
                 for file in g:
                     Stat.deleted += file.size
                     tqdm.write(click.style(f"remove file {file.path}", fg="red"))
                     os.unlink(file.path)
             else:
                 tqdm.write(tqdm.format_sizeof(g[0].size, suffix="B", divisor=1024))
                 for entry in sorted(g, key=lambda x: x.path):
                     tqdm.write(str(entry.path))
 
-    print(format_size(Stat.hashed))
+    print("hashed file size:", format_size(Stat.hashed))
+    if delete:
+        print("deleted file size:", format_size(Stat.deleted))
 
 
 def dedupe_by_size(locations: Iterable[str]):
     group_by_size: Dict[Tuple[int], List[Entry]] = defaultdict(list)
 
     with tqdm(desc="get all files", ascii=True) as bar:
         for locate in locations:
@@ -220,9 +226,7 @@
 
 def format_size(n: int):
     return tqdm.format_sizeof(n, "B", divisor=1024)
 
 
 if __name__ == "__main__":
     rdfind2()
-    print("hashed file size:", format_size(Stat.hashed))
-    print("deleted file size:", format_size(Stat.deleted))
```

### Comparing `rdfind2-0.0.3/readme.md` & `rdfind2-0.0.4/readme.md`

 * *Files identical despite different names*

