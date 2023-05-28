# Comparing `tmp/molcas_suite-1.21.0.tar.gz` & `tmp/molcas_suite-1.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.21.0.tar", last modified: Tue Mar  7 12:09:01 2023, max compression
+gzip compressed data, was "molcas_suite-1.22.0.tar", last modified: Sun May 28 14:32:12 2023, max compression
```

## Comparing `molcas_suite-1.21.0.tar` & `molcas_suite-1.22.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 12:09:01.432703 molcas_suite-1.21.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3618 2023-03-07 12:09:01.431702 molcas_suite-1.21.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 12:09:01.429702 molcas_suite-1.21.0/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-07 12:08:58.000000 molcas_suite-1.21.0/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    28028 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    31919 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18362 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25262 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21698 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 12:09:01.431702 molcas_suite-1.21.0/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3618 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-07 12:09:01.000000 molcas_suite-1.21.0/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-07 12:08:29.000000 molcas_suite-1.21.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-07 12:09:01.432703 molcas_suite-1.21.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-03-07 12:08:58.000000 molcas_suite-1.21.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.018009 molcas_suite-1.22.0/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-28 14:32:09.000000 molcas_suite-1.22.0/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    28028 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    31919 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18391 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25262 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21698 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.019009 molcas_suite-1.22.0/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-05-28 14:32:09.000000 molcas_suite-1.22.0/setup.py
```

### Comparing `molcas_suite-1.21.0/LICENSE` & `molcas_suite-1.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/PKG-INFO` & `molcas_suite-1.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.21.0
+Version: 1.22.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.21.0/README.md` & `molcas_suite-1.22.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/barrier.py` & `molcas_suite-1.22.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/cfp.py` & `molcas_suite-1.22.0/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/cli.py` & `molcas_suite-1.22.0/molcas_suite/cli.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/extractor.py` & `molcas_suite-1.22.0/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/generate_input.py` & `molcas_suite-1.22.0/molcas_suite/generate_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
              if isinstance(val, list) else (
                  "\n".join(map(str_indent, (f"{key}",) + val))
                  if isinstance(val, tuple) else str_indent(f"{key}= {val}"))
              for key, val in keywords_vals.items() if val is not None])
 
 
 class Gateway(MolcasProg):
-    def __init__(self, *args, **kwargs):
-        super().__init__('Gateway', *args, **kwargs)
+    def __init__(self, *args, group="NoSym", **kwargs):
+        super().__init__('Gateway', *args, **kwargs, group="NoSym")
 
 
 class Seward(MolcasProg):
     def __init__(self, *args, **kwargs):
         super().__init__('Seward', *args, **kwargs)
 
 
@@ -346,15 +346,15 @@
 
     sections = []
     sections.append(Gateway(
         "AMFI",
         *gateway_extra[0],
         "RICD" if decomp == 'RICD_acCD' else None,
         "acCD" if decomp == 'RICD_acCD' else None,
-        Coords=f"${{CurrDir}}/{rel_stem}_basis.xyz",
+        Coord=f"${{CurrDir}}/{rel_stem}_basis.xyz",
         XField=f"${{CurrDir}}/{rel_stem}.xfield" if xfield else None,
         Angmom=' '.join(map(str, coords[ctr_idx])) + " ANGSTROM",
         **gateway_extra[1]))
 
     sections.append(Seward(decomp if decomp != 'RICD_acCD' else None))
 
     # Get information on electronic states
```

### Comparing `molcas_suite-1.21.0/molcas_suite/generate_job.py` & `molcas_suite-1.22.0/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/h5tools.py` & `molcas_suite-1.22.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite/orbs.py` & `molcas_suite-1.22.0/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.21.0/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.22.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas-suite
-Version: 1.21.0
+Version: 1.22.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.21.0/setup.py` & `molcas_suite-1.22.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.21.0"
+__version__ = "1.22.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
```

