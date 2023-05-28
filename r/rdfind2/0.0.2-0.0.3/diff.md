# Comparing `tmp/rdfind2-0.0.2.tar.gz` & `tmp/rdfind2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.2.tar", last modified: Sun May 28 00:28:11 2023, max compression
+gzip compressed data, was "rdfind2-0.0.3.tar", last modified: Sun May 28 00:50:31 2023, max compression
```

## Comparing `rdfind2-0.0.2.tar` & `rdfind2-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:11.128140 rdfind2-0.0.2/
--rw-rw-rw-   0        0        0     1008 2023-05-28 00:28:11.127138 rdfind2-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-28 00:27:38.000000 rdfind2-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:11.126138 rdfind2-0.0.2/rdfind2.egg-info/
--rw-rw-rw-   0        0        0     1008 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7198 2023-05-28 00:27:28.000000 rdfind2-0.0.2/rdfind2.py
--rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.2/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 00:28:11.128140 rdfind2-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 00:50:31.197345 rdfind2-0.0.3/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 00:50:31.197345 rdfind2-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-28 00:50:15.000000 rdfind2-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-28 00:50:31.195343 rdfind2-0.0.3/rdfind2.egg-info/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 00:50:31.000000 rdfind2-0.0.3/rdfind2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7269 2023-05-28 00:49:15.000000 rdfind2-0.0.3/rdfind2.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.3/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 00:50:31.197345 rdfind2-0.0.3/setup.cfg
```

### Comparing `rdfind2-0.0.2/PKG-INFO` & `rdfind2-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rdfind2-0.0.2/pyproject.toml` & `rdfind2-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdfind2"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "trim21", email = "trim21.me@gmail.com" },
 ]
 description = "Find duplicated files very fast"
 readme = "readme.md"
 requires-python = ">=3.8,<4"
 license = { text = "MIT" }
```

### Comparing `rdfind2-0.0.2/rdfind2.egg-info/PKG-INFO` & `rdfind2-0.0.3/rdfind2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rdfind2-0.0.2/rdfind2.py` & `rdfind2-0.0.3/rdfind2.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import io
 import os
 import pathlib
 from collections import defaultdict
 from typing import Dict, Iterable, List, Optional, Tuple
 
 import click
-import tqdm
+from tqdm import tqdm
 
 PROGRESS_SIZE = 128 * 1024 * 1024  # 512M
 CHUNK_SIZE = 16 * 1024  # 16k
 PARTIAL_SIZE = 16
 
 
 @dataclasses.dataclass
@@ -57,19 +57,21 @@
 
         return self.b2sum
 
     @contextlib.contextmanager
     def open(self) -> io.BytesIO:
         if self.size > PROGRESS_SIZE:
             with self.path.open("rb") as f:
-                with tqdm.tqdm.wrapattr(
+                with tqdm.wrapattr(
                         f,
                         "read",
                         total=self.size,
-                        bar_format="{desc}: {percentage:3.0f}% {r_bar}",
+                        ascii=True,
+                        leave=False,
+                        position=1,
                 ) as reader:
                     yield reader
             return
         with self.path.open("rb") as f:
             yield f
 
     @property
@@ -108,59 +110,58 @@
 
     for _, headGroups in sorted(groups.items(), reverse=True):
         if len(headGroups) == 1:
             continue
 
         entry_groups.append(headGroups)
 
-    for entry_group in tqdm.tqdm(entry_groups):
+    for entry_group in tqdm(entry_groups, ascii=True, position=0):
         entry_grouped = compare_groups(entry_group)
         for g in entry_grouped:
             if len(g) == 1:
                 continue
 
             if hardlink:
-                print("link files:")
+                tqdm.write("link files:")
                 for file in g:
-                    click.secho(f"{file.path!s}", fg="red")
+                    tqdm.write(click.style(f"{file.path!s}", fg="red"))
 
                 link_src = g.pop()
 
                 for file in g:
                     if link_src.inode == file.inode:
                         continue
                     if file.path.name.endswith(".rdfind2.old"):
-                        click.secho(f"find internal temp file {file.path}", fg="red")
+                        tqdm.write(click.style(f"find internal temp file {file.path}", fg="red"))
                         continue
                     temp_file_path = pathlib.Path(
                         file.path.with_name(file.path.name + ".rdfind2.old")
                     )
                     file.path.rename(temp_file_path)
                     os.link(src=link_src.path, dst=file.path)
                     temp_file_path.unlink()
 
             elif delete:
                 g.pop()
                 for file in g:
                     Stat.deleted += file.size
-                    click.secho(f"remove file {file.path}", fg="red")
+                    tqdm.write(click.style(f"remove file {file.path}", fg="red"))
                     os.unlink(file.path)
             else:
-                print("")
-                print(tqdm.tqdm.format_sizeof(g[0].size, suffix="B", divisor=1024))
+                tqdm.write(tqdm.format_sizeof(g[0].size, suffix="B", divisor=1024))
                 for entry in sorted(g, key=lambda x: x.path):
-                    print(entry.path)
+                    tqdm.write(str(entry.path))
 
     print(format_size(Stat.hashed))
 
 
 def dedupe_by_size(locations: Iterable[str]):
     group_by_size: Dict[Tuple[int], List[Entry]] = defaultdict(list)
 
-    with tqdm.tqdm(desc="get all files", ascii=True) as bar:
+    with tqdm(desc="get all files", ascii=True) as bar:
         for locate in locations:
             for top, _, files in os.walk(locate):
                 t = pathlib.Path(top).absolute()
                 for file in files:
                     bar.update()
                     p = t.joinpath(file)
                     stat = p.stat()
@@ -174,15 +175,15 @@
 
 def dedupe_by_head_tail(
         group_by_size: Dict[Tuple[int], List[Entry]]
 ) -> Dict[Tuple[int, bytes, bytes], List[Entry]]:
     groups: Dict[Tuple[int, bytes, bytes], List[Entry]] = defaultdict(list)
     total = sum(len(x) for x in group_by_size.values())
 
-    with tqdm.tqdm(
+    with tqdm(
             total=total,
             desc="dedupe by file head/tail",
             ascii=True,
     ) as bar:
         for _, sizeGroups in sorted(group_by_size.items()):
             for e in sizeGroups:
                 bar.update()
@@ -214,14 +215,14 @@
         hash = hash_map[e.inode]
         result[hash].append(e)
 
     return list(result.values())
 
 
 def format_size(n: int):
-    return tqdm.tqdm.format_sizeof(n, "B", divisor=1024)
+    return tqdm.format_sizeof(n, "B", divisor=1024)
 
 
 if __name__ == "__main__":
     rdfind2()
     print("hashed file size:", format_size(Stat.hashed))
     print("deleted file size:", format_size(Stat.deleted))
```

### Comparing `rdfind2-0.0.2/readme.md` & `rdfind2-0.0.3/readme.md`

 * *Files identical despite different names*

