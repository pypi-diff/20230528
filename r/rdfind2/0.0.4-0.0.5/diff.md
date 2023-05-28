# Comparing `tmp/rdfind2-0.0.4.tar.gz` & `tmp/rdfind2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.4.tar", last modified: Sun May 28 01:20:56 2023, max compression
+gzip compressed data, was "rdfind2-0.0.5.tar", last modified: Sun May 28 01:29:20 2023, max compression
```

## Comparing `rdfind2-0.0.4.tar` & `rdfind2-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 01:20:56.237944 rdfind2-0.0.4/
--rw-rw-rw-   0        0        0     1008 2023-05-28 01:20:56.236942 rdfind2-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-28 01:20:39.000000 rdfind2-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 01:20:56.235941 rdfind2-0.0.4/rdfind2.egg-info/
--rw-rw-rw-   0        0        0     1008 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 01:20:56.000000 rdfind2-0.0.4/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7506 2023-05-28 01:20:29.000000 rdfind2-0.0.4/rdfind2.py
--rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.4/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 01:20:56.237944 rdfind2-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 01:29:20.251702 rdfind2-0.0.5/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 01:29:20.250701 rdfind2-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-28 01:28:57.000000 rdfind2-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-28 01:29:20.249700 rdfind2-0.0.5/rdfind2.egg-info/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 01:29:20.000000 rdfind2-0.0.5/rdfind2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7492 2023-05-28 01:28:51.000000 rdfind2-0.0.5/rdfind2.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.5/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 01:29:20.251702 rdfind2-0.0.5/setup.cfg
```

### Comparing `rdfind2-0.0.4/pyproject.toml` & `rdfind2-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdfind2"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "trim21", email = "trim21.me@gmail.com" },
 ]
 description = "Find duplicated files very fast"
 readme = "readme.md"
 requires-python = ">=3.8,<4"
 license = { text = "MIT" }
```

### Comparing `rdfind2-0.0.4/rdfind2.py` & `rdfind2-0.0.5/rdfind2.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,34 +122,34 @@
             if len(g) == 1:
                 continue
 
             if hardlink:
                 tqdm.write("link files:")
 
                 link_src = g.pop()
-                tqdm.write(click.style(f"hard link target file {link_src.path!r}", fg="green"))
+                tqdm.write(click.style(f"hard link target file {link_src.path!s}", fg="green"))
                 for file in g:
                     tqdm.write(click.style(f"{file.path!s}", fg="red"))
 
                 for file in g:
                     if link_src.inode == file.inode:
                         continue
                     if file.path.name.endswith(".rdfind2.old"):
-                        tqdm.write(click.style(f"find internal temp file {file.path!r}", fg="red"))
+                        tqdm.write(click.style(f"find internal temp file {file.path!s}", fg="red"))
                         continue
                     temp_file_path = pathlib.Path(
                         file.path.with_name(file.path.name + ".rdfind2.old")
                     )
                     file.path.rename(temp_file_path)
                     os.link(src=link_src.path, dst=file.path)
                     temp_file_path.unlink()
 
             elif delete:
                 link_src = g.pop()
-                tqdm.write(click.style(f"find internal temp file {link_src.path}", fg="green"))
+                tqdm.write(click.style(f"keep file {link_src.path}", fg="green"))
                 for file in g:
                     Stat.deleted += file.size
                     tqdm.write(click.style(f"remove file {file.path}", fg="red"))
                     os.unlink(file.path)
             else:
                 tqdm.write(tqdm.format_sizeof(g[0].size, suffix="B", divisor=1024))
                 for entry in sorted(g, key=lambda x: x.path):
```

### Comparing `rdfind2-0.0.4/readme.md` & `rdfind2-0.0.5/readme.md`

 * *Files identical despite different names*

