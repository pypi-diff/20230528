# Comparing `tmp/secat-1.1.4.tar.gz` & `tmp/secat-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secat-1.1.4.tar", last modified: Tue Apr  4 15:22:02 2023, max compression
+gzip compressed data, was "secat-1.1.5.tar", last modified: Sun May 28 19:31:47 2023, max compression
```

## Comparing `secat-1.1.4.tar` & `secat-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:02.059971 secat-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-04-04 15:21:47.000000 secat-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-04 15:22:02.059971 secat-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-04 15:21:47.000000 secat-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:02.059971 secat-1.1.4/secat/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-04 15:21:47.000000 secat-1.1.4/secat/EmpiricalBrownsMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:21:47.000000 secat-1.1.4/secat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-04-04 15:21:47.000000 secat-1.1.4/secat/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-04-04 15:21:47.000000 secat-1.1.4/secat/learn.py
--rw-r--r--   0 runner    (1001) docker     (123)    30676 2023-04-04 15:21:47.000000 secat-1.1.4/secat/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-04 15:21:47.000000 secat-1.1.4/secat/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    32689 2023-04-04 15:21:47.000000 secat-1.1.4/secat/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-04-04 15:21:47.000000 secat-1.1.4/secat/quantify.py
--rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-04-04 15:21:47.000000 secat-1.1.4/secat/score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:02.059971 secat-1.1.4/secat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-04 15:22:01.000000 secat-1.1.4/secat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-04 15:22:02.000000 secat-1.1.4/secat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:22:01.000000 secat-1.1.4/secat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 15:22:01.000000 secat-1.1.4/secat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-04 15:22:01.000000 secat-1.1.4/secat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 15:22:01.000000 secat-1.1.4/secat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 15:22:02.059971 secat-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-04 15:21:47.000000 secat-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:31:47.171515 secat-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-05-28 19:31:34.000000 secat-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-28 19:31:47.171515 secat-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-28 19:31:34.000000 secat-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:31:47.171515 secat-1.1.5/secat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-28 19:31:34.000000 secat-1.1.5/secat/EmpiricalBrownsMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 19:31:34.000000 secat-1.1.5/secat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-05-28 19:31:34.000000 secat-1.1.5/secat/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-05-28 19:31:34.000000 secat-1.1.5/secat/learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30677 2023-05-28 19:31:34.000000 secat-1.1.5/secat/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-28 19:31:34.000000 secat-1.1.5/secat/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32689 2023-05-28 19:31:34.000000 secat-1.1.5/secat/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-05-28 19:31:34.000000 secat-1.1.5/secat/quantify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-05-28 19:31:34.000000 secat-1.1.5/secat/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:31:47.171515 secat-1.1.5/secat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 19:31:47.000000 secat-1.1.5/secat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 19:31:47.171515 secat-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-28 19:31:34.000000 secat-1.1.5/setup.py
```

### Comparing `secat-1.1.4/LICENSE` & `secat-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/PKG-INFO` & `secat-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secat
-Version: 1.1.4
+Version: 1.1.5
 Summary: Size-Exclusion Chromatography Algorithmic Toolkit
 Home-page: https://github.com/grosenberger/secat
 Author: George Rosenberger
 Author-email: gr2578@cumc.columbia.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `secat-1.1.4/README.md` & `secat-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/EmpiricalBrownsMethod.py` & `secat-1.1.5/secat/EmpiricalBrownsMethod.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/export.py` & `secat-1.1.5/secat/export.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/learn.py` & `secat-1.1.5/secat/learn.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/main.py` & `secat-1.1.5/secat/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 @click.option('--level', default='bait', show_default=True, type=click.Choice(['bait', 'interaction']), help='Export either all interactions of bait proteins or individual interactions')
 @click.option('--id', required=False, type=str, help='Export specific UniProt bait_id (Q10000) or interaction_id (Q10000_P10000)')
 @click.option('--max_qvalue', default=0.01, show_default=True, type=float, help='Maximum q-value to export baits or interactions.')
 @click.option('--min_abs_log2fx', default=1.0, show_default=True, type=float, help='Minimum absolute log2 fold-change for integrated nodes.')
 @click.option('--mode', default='quantitative', show_default=True, type=click.Choice(['quantitative', 'detection']), help='Select mode to order interaction exported tables by.')
 @click.option('--combined/--no-combined', default=False, show_default=True, help='Select interactions and baits according to combined q-values.')
 @click.option('--peptide_rank', default=6, show_default=True, type=int, help='Number of most intense peptides to export.')
-@click.option('--extra', default=False, show_default=True, type=bool, help='Whether or not to export raw csv files of data used in `secat plot`')
+@click.option('--extras', default=False, show_default=True, type=bool, help='Whether or not to export raw csv files of data used in `secat plot`')
 def export(infile, level, id, max_qvalue, min_abs_log2fx, mode, combined, peptide_rank, extras):
     """
     Export SECAT results.
     """
     export_tables(infile, level, id, max_qvalue, min_abs_log2fx, mode, combined, peptide_rank, extras)
```

### Comparing `secat-1.1.4/secat/plot.py` & `secat-1.1.5/secat/plot.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/preprocess.py` & `secat-1.1.5/secat/preprocess.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/quantify.py` & `secat-1.1.5/secat/quantify.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat/score.py` & `secat-1.1.5/secat/score.py`

 * *Files identical despite different names*

### Comparing `secat-1.1.4/secat.egg-info/PKG-INFO` & `secat-1.1.5/secat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secat
-Version: 1.1.4
+Version: 1.1.5
 Summary: Size-Exclusion Chromatography Algorithmic Toolkit
 Home-page: https://github.com/grosenberger/secat
 Author: George Rosenberger
 Author-email: gr2578@cumc.columbia.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `secat-1.1.4/setup.py` & `secat-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='secat',
-    version='1.1.4',
+    version='1.1.5',
     description='Size-Exclusion Chromatography Algorithmic Toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/grosenberger/secat",
 	author="George Rosenberger",
 	author_email="gr2578@cumc.columbia.edu",
     classifiers=[
```

