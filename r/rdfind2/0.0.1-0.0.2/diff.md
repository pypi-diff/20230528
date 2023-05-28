# Comparing `tmp/rdfind2-0.0.1.tar.gz` & `tmp/rdfind2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.1.tar", last modified: Sun May 28 00:22:31 2023, max compression
+gzip compressed data, was "rdfind2-0.0.2.tar", last modified: Sun May 28 00:28:11 2023, max compression
```

## Comparing `rdfind2-0.0.1.tar` & `rdfind2-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:22:31.639752 rdfind2-0.0.1/
--rw-rw-rw-   0        0        0      900 2023-05-28 00:22:31.638752 rdfind2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-28 00:22:22.000000 rdfind2-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 00:22:31.637750 rdfind2-0.0.1/rdfind2.egg-info/
--rw-rw-rw-   0        0        0      900 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:22:31.000000 rdfind2-0.0.1/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7269 2023-05-28 00:04:30.000000 rdfind2-0.0.1/rdfind2.py
--rw-rw-rw-   0        0        0      533 2023-05-28 00:09:55.000000 rdfind2-0.0.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 00:22:31.639752 rdfind2-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:11.128140 rdfind2-0.0.2/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 00:28:11.127138 rdfind2-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-28 00:27:38.000000 rdfind2-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-28 00:28:11.126138 rdfind2-0.0.2/rdfind2.egg-info/
+-rw-rw-rw-   0        0        0     1008 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 00:28:11.000000 rdfind2-0.0.2/rdfind2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7198 2023-05-28 00:27:28.000000 rdfind2-0.0.2/rdfind2.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 00:25:09.000000 rdfind2-0.0.2/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 00:28:11.128140 rdfind2-0.0.2/setup.cfg
```

### Comparing `rdfind2-0.0.1/PKG-INFO` & `rdfind2-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
@@ -15,22 +15,30 @@
 
 [![](https://img.shields.io/pypi/v/rdfind2.svg)](https://pypi.python.org/pypi/rdfind2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdfind2)](https://pypi.org/project/rdfind2/)
 ![](https://img.shields.io/badge/License-MIT-blue.svg)
 
 find duplicated files (in one fs) very fast.
 
+rdfind2 will filter files by size, head, tail and inode.
+
+Only hash full files content when it's necessary.
+
+## Install
+
 with pipx:
 
 ```shell
 pipx install rdfind2
 ```
 
 with pip:
 
 ```shell
 pip install rdfind2
 ```
 
-rdfind2 will filter files by size, head, tail and inode.
+## Usage:
 
-Only hash full files content when it's necessary.
+```shell
+rdfind2 [--make-hardlink --delete] ./dir1 ./dir2 ...directory 
+```
```

### Comparing `rdfind2-0.0.1/pyproject.toml` & `rdfind2-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdfind2"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "trim21", email = "trim21.me@gmail.com" },
 ]
 description = "Find duplicated files very fast"
 readme = "readme.md"
 requires-python = ">=3.8,<4"
 license = { text = "MIT" }
```

### Comparing `rdfind2-0.0.1/rdfind2.egg-info/PKG-INFO` & `rdfind2-0.0.2/rdfind2.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find duplicated files very fast
 Author-email: trim21 <trim21.me@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
@@ -15,22 +15,30 @@
 
 [![](https://img.shields.io/pypi/v/rdfind2.svg)](https://pypi.python.org/pypi/rdfind2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdfind2)](https://pypi.org/project/rdfind2/)
 ![](https://img.shields.io/badge/License-MIT-blue.svg)
 
 find duplicated files (in one fs) very fast.
 
+rdfind2 will filter files by size, head, tail and inode.
+
+Only hash full files content when it's necessary.
+
+## Install
+
 with pipx:
 
 ```shell
 pipx install rdfind2
 ```
 
 with pip:
 
 ```shell
 pip install rdfind2
 ```
 
-rdfind2 will filter files by size, head, tail and inode.
+## Usage:
 
-Only hash full files content when it's necessary.
+```shell
+rdfind2 [--make-hardlink --delete] ./dir1 ./dir2 ...directory 
+```
```

### Comparing `rdfind2-0.0.1/rdfind2.py` & `rdfind2-0.0.2/rdfind2.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 @click.command()
 @click.argument(
     "location",
     required=True,
     nargs=-1,
     type=click.Path(exists=True, file_okay=False, readable=True, resolve_path=True),
 )
-@click.option("--make-hardlink", "hardlink", is_flag=True, default=False,help='used when you search duplicate files in same device')
+@click.option("--make-hardlink", "hardlink", is_flag=True, default=False,
+              help='used when you search duplicate files in same device')
 @click.option("--delete", "delete", is_flag=True, default=False)
 def rdfind2(location: Tuple[str], hardlink=False, delete=False):
     if hardlink and delete:
         click.secho("can't use '--make-hardlink' with '--delete'", fg="green", err=True)
     group_by_size = dedupe_by_size(location)
 
     groups: Dict[tuple, List[Entry]] = dedupe_by_head_tail(group_by_size)
@@ -107,17 +108,15 @@
 
     for _, headGroups in sorted(groups.items(), reverse=True):
         if len(headGroups) == 1:
             continue
 
         entry_groups.append(headGroups)
 
-    total = len(entry_groups)
-    for i, entry_group in enumerate(entry_groups):
-        click.secho(f"{i + 1}/{total}", fg="green")
+    for entry_group in tqdm.tqdm(entry_groups):
         entry_grouped = compare_groups(entry_group)
         for g in entry_grouped:
             if len(g) == 1:
                 continue
 
             if hardlink:
                 print("link files:")
```

### Comparing `rdfind2-0.0.1/readme.md` & `rdfind2-0.0.2/readme.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,30 @@
 
 [![](https://img.shields.io/pypi/v/rdfind2.svg)](https://pypi.python.org/pypi/rdfind2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rdfind2)](https://pypi.org/project/rdfind2/)
 ![](https://img.shields.io/badge/License-MIT-blue.svg)
 
 find duplicated files (in one fs) very fast.
 
+rdfind2 will filter files by size, head, tail and inode.
+
+Only hash full files content when it's necessary.
+
+## Install
+
 with pipx:
 
 ```shell
 pipx install rdfind2
 ```
 
 with pip:
 
 ```shell
 pip install rdfind2
 ```
 
-rdfind2 will filter files by size, head, tail and inode.
+## Usage:
 
-Only hash full files content when it's necessary.
+```shell
+rdfind2 [--make-hardlink --delete] ./dir1 ./dir2 ...directory 
+```
```

