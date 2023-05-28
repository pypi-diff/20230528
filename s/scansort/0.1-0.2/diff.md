# Comparing `tmp/scansort-0.1.tar.gz` & `tmp/scansort-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scansort-0.1.tar", last modified: Wed Dec  7 19:43:21 2016, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `scansort-0.1.tar` & `scansort-0.2.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxr-xr-x   0 mkuznets  (1000) mkuznets  (1000)        0 2016-12-07 19:43:21.000000 scansort-0.1/
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)       59 2016-12-07 19:43:21.000000 scansort-0.1/setup.cfg
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)      592 2016-12-07 19:43:21.000000 scansort-0.1/PKG-INFO
--rw-rw-r--   0 mkuznets  (1000) mkuznets  (1000)     3683 2016-12-07 19:27:31.000000 scansort-0.1/README.rst
-drwxr-xr-x   0 mkuznets  (1000) mkuznets  (1000)        0 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)        1 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/dependency_links.txt
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)        7 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/requires.txt
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)        9 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/top_level.txt
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)      592 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/PKG-INFO
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)      255 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/SOURCES.txt
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)       53 2016-12-07 19:43:21.000000 scansort-0.1/scansort.egg-info/entry_points.txt
--rw-r--r--   0 mkuznets  (1000) mkuznets  (1000)      792 2016-12-07 19:39:23.000000 scansort-0.1/setup.py
-drwxr-xr-x   0 mkuznets  (1000) mkuznets  (1000)        0 2016-12-07 19:43:21.000000 scansort-0.1/scansort/
--rw-rw-r--   0 mkuznets  (1000) mkuznets  (1000)        0 2016-09-28 14:28:19.000000 scansort-0.1/scansort/__init__.py
--rwxr-xr-x   0 mkuznets  (1000) mkuznets  (1000)     5410 2016-12-07 19:36:47.000000 scansort-0.1/scansort/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scansort-0.2/scansort/__init__.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scansort-0.2/scansort/__main__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 scansort-0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 scansort-0.2/LICENSE
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 scansort-0.2/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scansort-0.2/pyproject.toml
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 scansort-0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scansort-0.1/README.rst` & `scansort-0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,129 @@
---------
-Scansort
---------
+# Scansort
 
 **Scansort** helps to collate and rename book scan images
 
-============
-Installation
-============
+## Installation
 
-.. code-block::
+``` 
+pip install scansort
+```
 
-    pip install scansort
+## Synopsis
 
-========
-Synopsis
-========
+``` 
+scansort [-h] [-v]
+         -odd ODD -even EVEN [-missing MISSING]
+         [-action {move,copy}] [-o OUTPUT] workdir
+```
 
-.. code-block::
+## Desctiption
 
-    scansort [-h] [-v]
-             -odd ODD -even EVEN [-missing MISSING]
-             [-action {move,copy}] [-o OUTPUT] workdir
+When using a book-edge scanner (such as Plustek OpticBook), it is handy
+to scan two sides of a book separately. This way you do not need to
+rotate the book to scan the next page. Scanned images from different
+sides normally make their way into separate directories.
 
-===========
-Desctiption
-===========
-
-When using a book-edge scanner (such as Plustek OpticBook),
-it is handy to scan two sides of a book separately.
-This way you do not need to rotate the book to scan the next page.
-Scanned images from different sides normally
-make their way into separate directories.
-
-**Scansort** helps one to collate these directories
-and rename images accodring to the actual page numbers.
+**Scansort** helps one to collate these directories and rename images
+accodring to the actual page numbers.
 
 The utility assumes that:
 
-* The collection of images covers
-  a monotonically increasing range of page numbers
-  (with known missing numbers possible).
-  This implies that front-, body-, and (possibly) back-matter
-  must be scanned and processed separately.
-* Even- and odd-numbered pages are put into separate directories.
-
-Also, see an example_ of the indented workflow.
-
-=======
-Options
-=======
+-   The collection of images covers a monotonically increasing range of
+    page numbers (with known missing numbers possible). This implies
+    that front-, body-, and (possibly) back-matter must be scanned and
+    processed separately.
+-   Even- and odd-numbered pages are put into separate directories.
 
-``workdir`` argument defines a working directory
-relative to which all other directory names and paths are interpreted.
-By default the current directory is used.
+Also, see an [example](#example) of the indented workflow.
 
-All page numbers must correspond to
-the actual "physical" page numbering in the book.
+## Options
 
-``-odd, -even`` *directory name/path*
-    Source directories with scanned images of odd- and even-numbered pages.
+`workdir` argument defines a working directory relative to which all
+other directory names and paths are interpreted. By default the current
+directory is used.
 
-``-missing`` *num[,num]\**
-    Comma-separated list of page numbers missing in the source directories
-    (either accidentally skipped during scanning or not present at all).
+All page numbers must correspond to the actual "physical" page numbering
+in the book.
 
-``-action`` *{move,copy}*
-    Whether to preserve or delete the original images
-    from the source directories. Defaults to ``copy``.
+`-odd, -even` directory name/path  
+Source directories with scanned images of odd- and even-numbered pages.
 
-``-o`` *directory name/path*
-    Output directory for renamed scanned images. Defaults to ``out``
-    and will be created automatically if does not exist.
+`-missing` num\[,num\]\*  
+Comma-separated list of page numbers missing in the source directories
+(either accidentally skipped during scanning or not present at all).
 
-``-h, --help``
-    Show a help message and exit.
+`-action` {move,copy}  
+Whether to preserve or delete the original images from the source
+directories. Defaults to `copy`.
 
-``-v, --version``
-    Show a version information and exit.
+`-o` directory name/path  
+Output directory for renamed scanned images. Defaults to `out` and will
+be created automatically if does not exist.
 
+`-h, --help`  
+Show a help message and exit.
 
-.. _example:
+`-v, --version`  
+Show a version information and exit.
 
-=======
-Example
-=======
+## Example
 
 After scanning a book I am normally left with something like this:
 
-.. code-block::
-
-    $ tree ./book
-    ./book
-    ├── lside
-    │   ├── scan0001.tiff
-    │   ├── scan0002.tiff
-    │     ...
-    └── rside
-        ├── scan0001.tiff
-        ├── scan0002.tiff
-          ...
-
-    2 directories, 198 files
-
-where ``rside`` contains even-numbered pages. Suppose I skimmed through
-the directories and realised I missed two pages: 2 and 10.
-
-Then I run ``scansort`` to collate the directories:
-
-.. code-block::
-
-    $ scansort -odd lside -even rside -missing 2,6 ./book
-
+``` 
+$ tree ./book
+./book
+├── lside
+│   ├── scan0001.tiff
+│   ├── scan0002.tiff
+│     ...
+└── rside
+    ├── scan0001.tiff
+    ├── scan0002.tiff
+      ...
+
+2 directories, 198 files
+```
+
+where `rside` contains even-numbered pages. Suppose I skimmed through
+the directories and realised I missed two pages: 2 and 6.
+
+Then I run `scansort` to collate the directories:
+
+``` 
+$ scansort -odd lside -even rside -missing 2,6 ./book
+```
 
 The utility opens an editor to review the result:
 
-.. code-block::
-
-    # Please review the correspondence between files and book pages
-    './book/lside/scan0001.tiff':   1
-    './book/lside/scan0002.tiff':   3
-    './book/rside/scan0001.tiff':   4
-    './book/lside/scan0003.tiff':   5
-    './book/lside/scan0004.tiff':   7
-    './book/rside/scan0002.tiff':   8
+``` 
+# Please review the correspondence between files and book pages
+'./book/lside/scan0001.tiff':   1
+'./book/lside/scan0002.tiff':   3
+'./book/rside/scan0001.tiff':   4
+'./book/lside/scan0003.tiff':   5
+'./book/lside/scan0004.tiff':   7
+'./book/rside/scan0002.tiff':   8
+...
+```
+
+I can edit the page numbers right away or remove all lines to cancel the
+operation (e.g. if it turns out there are more pages missing). Then I
+save and close the editor and the pages are collated:
+
+``` 
+$ tree ./book/out
+./book/out
+├── scan0001.tif
+├── scan0003.tif
+├── scan0004.tif
+├── scan0005.tif
+├── scan0007.tif
     ...
+└── scan0200.tif
 
-I can edit the page numbers right away
-or remove all lines to cancel the operation
-(e.g. if it turns out there are more pages missing).
-Then I save and close the editor and the pages are collated:
-
-.. code-block::
-
-    $ tree ./book/out
-    ./book/out
-    ├── scan0001.tif
-    ├── scan0003.tif
-    ├── scan0004.tif
-    ├── scan0005.tif
-    ├── scan0007.tif
-        ...
-    └── scan0200.tif
-
-    0 directories, 198 files
+0 directories, 198 files
+```
 
-Note that the missing page number are omitted. I can then scan those separately
-and put in place.
+Note that the missing page number are omitted. I can then scan those
+separately and put in place.
```

### Comparing `scansort-0.1/scansort/__main__.py` & `scansort-0.2/scansort/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,62 +6,61 @@
     Scansort executable
 
     :copyright: (c) 2016, Max Kuznetsov
     :license: MIT, see LICENSE for more details.
 """
 
 import os
+import shutil
 import subprocess
 import tempfile
-import shutil
-import yaml
 from enum import Enum
-from typing import Callable, Iterable, Mapping, Tuple
+from typing import Callable, Dict, Iterable, List, Mapping, Tuple
 
+import yaml
 
-__version__ = '0.1'
+__version__ = "0.2"
 
-ACTIONS = {
-    'move': shutil.move,
-    'copy': shutil.copy
-}
+ACTIONS = {"move": shutil.move, "copy": shutil.copy}
 
 
 class Reviewer:
     def __init__(self, mapping: Mapping) -> None:
         self.mapping = mapping
 
     @staticmethod
     def _readable_to_map(text: str) -> Mapping:
-        return yaml.load(text)
+        return yaml.safe_load(text)
 
     @staticmethod
     def _map_to_readable(data: Mapping) -> str:
         max_page = max(data.values())
         padding = len(str(max_page))
-        fmt = '%%s:%% %dd' % (padding+1)
+        fmt = "%%s:%% %dd" % (padding + 1)
 
-        content = "\n".join(fmt % (repr(f), p) for f, p in
-                            sorted(data.items(), key=lambda x: x[1]))
+        content = "\n".join(
+            fmt % (repr(f), p) for f, p in sorted(data.items(), key=lambda x: x[1])
+        )
         return content
 
     def review(self) -> Mapping:
         json_map = self._map_to_readable(self.mapping)
 
-        with tempfile.NamedTemporaryFile(mode='w+', delete=False) as f:
-            f.write("# Please review the correspondence "
-                    "between files and book pages\n")
+        with tempfile.NamedTemporaryFile(mode="w+", delete=False) as f:
+            f.write(
+                "# Please review the correspondence " "between files and book pages\n"
+            )
             f.write(json_map)
             tmp_file = f.name
 
-        subprocess.run(['vi', tmp_file])
+        subprocess.run(["vi", tmp_file])
 
-        with open(tmp_file, 'r') as ff:
+        with open(tmp_file, "r") as ff:
             lines = (line.strip() for line in ff)
-            edited_json = "\n".join(l for l in lines if not l.startswith('#'))
+            edited_json = "\n".join(line for line in lines if not line.startswith("#"))
         os.unlink(tmp_file)
 
         return self._readable_to_map(edited_json)
 
 
 class Page(Enum):
     odd = 1
@@ -69,127 +68,144 @@
 
     @staticmethod
     def test(type_: Enum) -> Callable[[int], bool]:
         return lambda n: (n % 2) == (type_.value % 2)
 
     @staticmethod
     def range(n: int, type_: Enum) -> Iterable[int]:
-        return range(type_.value, n+1, 2)
+        return range(type_.value, n + 1, 2)
 
 
 class Book:
-    def __init__(self):
-        self.files = {}
-        self.missing = {}
+    def __init__(self) -> None:
+        self.files: Dict[Page, List[str]] = {}
+        self.missing: Dict[Page, List[int]] = {}
 
     @property
     def n_all(self) -> int:
         return sum(self.n(t) for t in Page)
 
     @property
     def is_valid(self) -> bool:
         return self.n(Page.odd) - self.n(Page.even) == self.n_all % 2
 
     def n(self, type_: Page) -> int:
         return len(self.files[type_]) + len(self.missing[type_])
 
     def add_files_from(self, type_: Page, directory: str) -> None:
-        self.files[type_] = sorted(e.path for e in os.scandir(directory)
-                                   if e.is_file())
+        self.files[type_] = sorted(e.path for e in os.scandir(directory) if e.is_file())
 
     def add_missing(self, missing: Iterable[int]) -> None:
         for type_ in Page:
             self.missing[type_] = list(filter(Page.test(type_), missing))
 
     def map_files_to_pages(self) -> Mapping:
         mapping = {}
 
         for type_, files in self.files.items():
             missing = self.missing[type_]
-            pages = filter(lambda x: x not in missing,
-                           Page.range(self.n_all, type_))
+            pages = filter(lambda x: x not in missing, Page.range(self.n_all, type_))
             mapping.update({files[i]: p for i, p in enumerate(pages)})
 
         return mapping
 
 
-def scansort(work_dir: str, odd_dir: str, even_dir: str, missing: tuple,
-         output_dir: str, action: str, fmt: str) -> None:
-
+def scansort(
+    work_dir: str,
+    odd_dir: str,
+    even_dir: str,
+    missing: tuple,
+    output_dir: str,
+    action: str,
+    fmt: str,
+) -> None:
     book = Book()
 
     book.add_missing(missing)
 
     for type_, dir_ in ((Page.odd, odd_dir), (Page.even, even_dir)):
         book.add_files_from(type_, os.path.join(work_dir, dir_))
 
     if not book.is_valid:
-        raise ValueError('Page numbers does not correspond')
+        raise ValueError("Page numbers does not correspond")
 
     rev = Reviewer(book.map_files_to_pages())
     files_to_pages = rev.review()
 
     if not files_to_pages:
         print("Nothing to do, sorting is cancelled.")
         return
 
     output_path = os.path.join(work_dir, output_dir)
     os.makedirs(output_path, exist_ok=True)
 
-    act = ACTIONS[action]
     output_fmt = os.path.join(output_path, fmt)
 
     for file_, page in files_to_pages.items():
-        act(file_, output_fmt % page)
-
-    print('%d files have been processed.' % len(files_to_pages))
+        destination = output_fmt % page
+        if action == "move":
+            shutil.move(file_, destination)
+        elif action == "copy":
+            shutil.copy2(file_, destination)
+        else:
+            raise ValueError("Unknown action: %s" % action)
 
+    print("%d files have been processed." % len(files_to_pages))
 
-def main():
 
+def main() -> None:
     from argparse import ArgumentParser
 
     def comma_split(s: str) -> Tuple:
         if not s:
             return ()
         else:
-            return tuple(map(int, s.split(',')))
-
+            return tuple(map(int, s.split(",")))
 
     parser = ArgumentParser(
-        description='Scansort helps to collate and rename book scan images'
+        description="Scansort helps to collate and rename book scan images"
     )
 
-    parser.add_argument('-v', '--version', action='version',
-                        version='scansort %s' % __version__)
-    parser.add_argument('workdir', default='.',
-                        help='working directory for input and output files')
-    parser.add_argument('-odd', required=True,
-                        help='directory with odd-numbered pages')
-    parser.add_argument('-even', required=True,
-                        help='directory with even-numbered pages')
     parser.add_argument(
-        '-missing', default='', type=comma_split,
-        help='comma-separated list of pages numbers (e.g. 1,24,35)'
+        "-v", "--version", action="version", version="scansort %s" % __version__
+    )
+    parser.add_argument(
+        "workdir", default=".", help="working directory for input and output files"
+    )
+    parser.add_argument("-odd", required=True, help="directory with odd-numbered pages")
+    parser.add_argument(
+        "-even", required=True, help="directory with even-numbered pages"
+    )
+    parser.add_argument(
+        "-missing",
+        default="",
+        type=comma_split,
+        help="comma-separated list of pages numbers (e.g. 1,24,35)",
+    )
+    parser.add_argument(
+        "-action",
+        default="copy",
+        choices=("copy", "move"),
+        help="action performed to the selected files (default: %(default)s)",
     )
     parser.add_argument(
-        '-action', default='copy', choices=ACTIONS.keys(),
-        help='action performed to the selected files (default: %(default)s)'
+        "-o",
+        default="out",
+        dest="output",
+        help="output directory (default: %(default)s)",
     )
-    parser.add_argument('-o', default='out', dest='output',
-                        help='output directory (default: %(default)s)')
 
     args = parser.parse_args()
 
     scansort(
         work_dir=args.workdir,
         odd_dir=args.odd,
         even_dir=args.even,
         missing=args.missing,
         action=args.action,
         output_dir=args.output,
-        fmt='scan%04d.tif'
+        fmt="scan%04d.tif",
     )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

