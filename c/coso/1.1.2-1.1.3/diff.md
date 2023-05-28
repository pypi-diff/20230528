# Comparing `tmp/coso-1.1.2.tar.gz` & `tmp/coso-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.1.2.tar", last modified: Sun May 28 15:30:34 2023, max compression
+gzip compressed data, was "coso-1.1.3.tar", last modified: Sun May 28 16:08:22 2023, max compression
```

## Comparing `coso-1.1.2.tar` & `coso-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 15:30:34.480803 coso-1.1.2/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.1.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-27 08:22:38.000000 coso-1.1.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-28 15:30:34.480540 coso-1.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.1.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 15:30:34.465811 coso-1.1.2/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-28 15:30:34.000000 coso-1.1.2/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      571 2023-05-28 15:30:34.000000 coso-1.1.2/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-28 15:30:34.000000 coso-1.1.2/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-05-28 15:30:34.000000 coso-1.1.2/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-28 15:30:34.000000 coso-1.1.2/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.1.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-28 15:30:34.480881 coso-1.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1144 2023-05-28 15:30:25.000000 coso-1.1.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 15:30:34.477059 coso-1.1.2/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 15:30:34.479296 coso-1.1.2/src/VisCoSo/
--rwxrwxrwx   0 root         (0) root         (0)      165 2023-04-27 13:29:49.000000 coso-1.1.2/src/VisCoSo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.1.2/src/VisCoSo/header.html
--rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.1.2/src/VisCoSo/viscoso.css
--rwxrwxrwx   0 root         (0) root         (0)   113113 2023-04-27 14:09:51.000000 coso-1.1.2/src/VisCoSo/viscoso.html
--rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.1.2/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11427 2023-04-28 10:26:12.000000 coso-1.1.2/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.1.2/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.1.2/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15881 2023-04-27 14:10:35.000000 coso-1.1.2/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)     1998 2023-05-26 15:05:32.000000 coso-1.1.2/src/launcher.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.1.2/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.1.2/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8705 2023-05-26 06:18:26.000000 coso-1.1.2/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9646 2023-04-27 14:45:44.000000 coso-1.1.2/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-05-25 10:07:11.000000 coso-1.1.2/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.1.2/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.1.2/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43522 2023-04-27 14:11:45.000000 coso-1.1.2/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14453 2023-05-28 15:26:11.000000 coso-1.1.2/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)    21847 2023-05-26 08:04:01.000000 coso-1.1.2/src/venn.py
--rwxrwxrwx   0 root         (0) root         (0)    20217 2023-04-27 13:50:00.000000 coso-1.1.2/src/viscoso.py
--rwxrwxrwx   0 root         (0) root         (0)     3878 2023-04-27 15:07:27.000000 coso-1.1.2/src/viscoso_widget.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 16:08:22.211805 coso-1.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-27 08:22:38.000000 coso-1.1.3/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-28 16:08:22.211578 coso-1.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.1.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 16:08:22.201451 coso-1.1.3/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-28 16:08:22.000000 coso-1.1.3/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      571 2023-05-28 16:08:22.000000 coso-1.1.3/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-28 16:08:22.000000 coso-1.1.3/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-05-28 16:08:22.000000 coso-1.1.3/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-28 16:08:22.000000 coso-1.1.3/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.1.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-28 16:08:22.211872 coso-1.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1144 2023-05-28 16:07:06.000000 coso-1.1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 16:08:22.209273 coso-1.1.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 16:08:22.210626 coso-1.1.3/src/VisCoSo/
+-rwxrwxrwx   0 root         (0) root         (0)      165 2023-04-27 13:29:49.000000 coso-1.1.3/src/VisCoSo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.1.3/src/VisCoSo/header.html
+-rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.1.3/src/VisCoSo/viscoso.css
+-rwxrwxrwx   0 root         (0) root         (0)   113113 2023-04-27 14:09:51.000000 coso-1.1.3/src/VisCoSo/viscoso.html
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.1.3/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11427 2023-04-28 10:26:12.000000 coso-1.1.3/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.1.3/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.1.3/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15881 2023-04-27 14:10:35.000000 coso-1.1.3/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)     1998 2023-05-26 15:05:32.000000 coso-1.1.3/src/launcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.1.3/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.1.3/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8705 2023-05-26 06:18:26.000000 coso-1.1.3/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9646 2023-04-27 14:45:44.000000 coso-1.1.3/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-05-25 10:07:11.000000 coso-1.1.3/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.1.3/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.1.3/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43522 2023-04-27 14:11:45.000000 coso-1.1.3/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14476 2023-05-28 16:01:36.000000 coso-1.1.3/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    21847 2023-05-26 08:04:01.000000 coso-1.1.3/src/venn.py
+-rwxrwxrwx   0 root         (0) root         (0)    20217 2023-04-27 13:50:00.000000 coso-1.1.3/src/viscoso.py
+-rwxrwxrwx   0 root         (0) root         (0)     3878 2023-04-27 15:07:27.000000 coso-1.1.3/src/viscoso_widget.py
```

### Comparing `coso-1.1.2/LICENSE` & `coso-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/PKG-INFO` & `coso-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.1.2
+Version: 1.1.3
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.1.2/README.md` & `coso-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/coso.egg-info/PKG-INFO` & `coso-1.1.3/coso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.1.2
+Version: 1.1.3
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.1.2/coso.egg-info/SOURCES.txt` & `coso-1.1.3/coso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/setup.py` & `coso-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='coso',
-    version='1.1.2',    
+    version='1.1.3',    
     url='https://github.com/PietroTotis/CoSo',
     author='Pietro Totis',
     author_email='pietro.totis@kuleuven.be',
     license='GNU General Public License (GPL)',
 
     # packages=find_packages(),
     packages=['coso'],
```

### Comparing `coso-1.1.2/src/VisCoSo/header.html` & `coso-1.1.3/src/VisCoSo/header.html`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/VisCoSo/viscoso.css` & `coso-1.1.3/src/VisCoSo/viscoso.css`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/VisCoSo/viscoso.html` & `coso-1.1.3/src/VisCoSo/viscoso.html`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/__init__.py` & `coso-1.1.3/src/__init__.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/cola_parser.py` & `coso-1.1.3/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/configuration.py` & `coso-1.1.3/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/count.py` & `coso-1.1.3/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/gen_plots.py` & `coso-1.1.3/src/gen_plots.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/launcher.py` & `coso-1.1.3/src/launcher.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/level_1.py` & `coso-1.1.3/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/level_2.py` & `coso-1.1.3/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/logger.py` & `coso-1.1.3/src/logger.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/parsetab.py` & `coso-1.1.3/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/problem.py` & `coso-1.1.3/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/sharpCSP.py` & `coso-1.1.3/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/solver.py` & `coso-1.1.3/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/tester.py` & `coso-1.1.3/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/util.py` & `coso-1.1.3/src/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import os
 import sys
 import importlib.resources
 from pathlib import Path
 from portion.dict import IntervalDict
 from typing import Counter
 
-
-ROOT_DIR = Path(__file__).parent.parent
-if (ROOT_DIR / "src").exists():
-    VISCOSO_DIR = ROOT_DIR / "src" / "VisCoSo" 
-else:
+cwd = Path(__file__).parent
+if cwd.name == "coso":
+    ROOT_DIR = cwd
     VISCOSO_DIR = ROOT_DIR / "VisCoSo" 
+else:
+    ROOT_DIR = cwd.parent
+    VISCOSO_DIR = ROOT_DIR / "src" / "VisCoSo" 
 
 CSS_VISCOSO = VISCOSO_DIR / "viscoso.css"
 
 
 ######################
 ## Interval methods ##
 ######################
```

### Comparing `coso-1.1.2/src/venn.py` & `coso-1.1.3/src/venn.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/viscoso.py` & `coso-1.1.3/src/viscoso.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.2/src/viscoso_widget.py` & `coso-1.1.3/src/viscoso_widget.py`

 * *Files identical despite different names*

