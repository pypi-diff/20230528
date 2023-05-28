# Comparing `tmp/bipartitepandas-1.1.5.tar.gz` & `tmp/bipartitepandas-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipartitepandas-1.1.5.tar", last modified: Fri May 26 18:48:02 2023, max compression
+gzip compressed data, was "bipartitepandas-1.1.6.tar", last modified: Sun May 28 03:42:06 2023, max compression
```

## Comparing `bipartitepandas-1.1.5.tar` & `bipartitepandas-1.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.650304 bipartitepandas-1.1.5/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/LICENSE
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-05-26 18:48:02.650394 bipartitepandas-1.1.5/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2201 2023-01-08 21:39:31.000000 bipartitepandas-1.1.5/README.rst
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.647316 bipartitepandas-1.1.5/bipartitepandas/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.5/bipartitepandas/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-26 18:39:16.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitebase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitedataframe.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelong.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelongbase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelongcollapsed.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648379 bipartitepandas-1.1.5/bipartitepandas/grouping/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/grouping/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3162 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/grouping/grouping.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648664 bipartitepandas-1.1.5/bipartitepandas/measures/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/measures/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8462 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/measures/measures.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.5/bipartitepandas/simbipartite.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.5/bipartitepandas/util.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648099 bipartitepandas-1.1.5/bipartitepandas.egg-info/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/SOURCES.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/dependency_links.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/requires.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/top_level.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.5/pyproject.toml
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-26 18:48:02.650776 bipartitepandas-1.1.5/setup.cfg
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.5/setup.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.650175 bipartitepandas-1.1.5/tests/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.5/tests/test_bpd_base.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17659 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_clustering.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.5/tests/test_bpd_connectedness.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_custom.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_df.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_es.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_es_collapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.5/tests/test_bpd_long.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.5/tests/test_bpd_long_collapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.743100 bipartitepandas-1.1.6/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/LICENSE
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-28 03:42:06.743205 bipartitepandas-1.1.6/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2204 2023-05-28 03:41:14.000000 bipartitepandas-1.1.6/README.rst
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.738546 bipartitepandas-1.1.6/bipartitepandas/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.6/bipartitepandas/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-28 02:35:42.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitebase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitedataframe.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelong.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelongbase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelongcollapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.739566 bipartitepandas-1.1.6/bipartitepandas/grouping/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/bipartitepandas/grouping/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3162 2023-05-28 02:59:45.000000 bipartitepandas-1.1.6/bipartitepandas/grouping/grouping.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.740127 bipartitepandas-1.1.6/bipartitepandas/measures/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/bipartitepandas/measures/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     6778 2023-05-28 03:40:11.000000 bipartitepandas-1.1.6/bipartitepandas/measures/measures.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.6/bipartitepandas/simbipartite.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.6/bipartitepandas/util.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.739273 bipartitepandas-1.1.6/bipartitepandas.egg-info/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/SOURCES.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/dependency_links.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/requires.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/top_level.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.6/pyproject.toml
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-28 03:42:06.743629 bipartitepandas-1.1.6/setup.cfg
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.6/setup.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.742961 bipartitepandas-1.1.6/tests/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.6/tests/test_bpd_base.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17148 2023-05-28 03:00:38.000000 bipartitepandas-1.1.6/tests/test_bpd_clustering.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.6/tests/test_bpd_connectedness.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_custom.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_df.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_es.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_es_collapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.6/tests/test_bpd_long.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.6/tests/test_bpd_long_collapsed.py
```

### Comparing `bipartitepandas-1.1.5/LICENSE` & `bipartitepandas-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/PKG-INFO` & `bipartitepandas-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +65,9 @@
 
 Thibaut Lamadon,
 Assistant Professor in Economics, University of Chicago,
 lamadon@uchicago.edu
 
 
 Adam A. Oppenheimer,
-Research Professional, University of Chicago,
-oppenheimer@uchicago.edu
+Graduate Student, University of Minnesota - Twin Cities,
+oppen040@umn.edu
```

### Comparing `bipartitepandas-1.1.5/README.rst` & `bipartitepandas-1.1.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -49,9 +49,9 @@
 
 Thibaut Lamadon,
 Assistant Professor in Economics, University of Chicago,
 lamadon@uchicago.edu
 
 
 Adam A. Oppenheimer,
-Research Professional, University of Chicago,
-oppenheimer@uchicago.edu
+Graduate Student, University of Minnesota - Twin Cities,
+oppen040@umn.edu
```

### Comparing `bipartitepandas-1.1.5/bipartitepandas/__init__.py` & `bipartitepandas-1.1.6/bipartitepandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartitebase.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartitebase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartitedataframe.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartitedataframe.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudy.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudybase.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudycollapsed.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudy.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudybase.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudycollapsed.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartitelong.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartitelong.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartitelongbase.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartitelongbase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/bipartitelongcollapsed.py` & `bipartitepandas-1.1.6/bipartitepandas/bipartitelongcollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/grouping/grouping.py` & `bipartitepandas-1.1.6/bipartitepandas/grouping/grouping.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/measures/measures.py` & `bipartitepandas-1.1.6/bipartitepandas/measures/measures.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class CDFs:
     '''
     Generate cdfs of compensation for firms. Used for clustering.
 
     Arguments:
         cdf_resolution (int): how many values to use to approximate the cdfs
-        measure (str): how to compute the cdfs ('quantile_all' to get quantiles from entire set of data, then have firm-level values between 0 and 1; 'quantile_firm_small' to get quantiles at the firm-level and have values be compensations if small data; 'quantile_firm_large' to get quantiles at the firm-level and have values be compensations if large data, note that this is up to 50 times slower than 'quantile_firm_small' and should only be used if the dataset is too large to copy into a dictionary
+        measure (str): how to compute the cdfs ('quantile_all' to get quantiles from entire set of data, then have firm-level values between 0 and 1; 'quantile_firm' to get quantiles at the firm-level and have values be compensations)
     '''
 
     def __init__(self, cdf_resolution=10, measure='quantile_all'):
         self.cdf_resolution = cdf_resolution
         self.measure = measure
 
     def _compute_measure(self, frame, jids):
@@ -24,91 +24,87 @@
             frame (Pandas DataFrame): data to use
             jids (list): sorted list of firm ids in frame (since frame could be a subset of self, this is not necessarily all firms in self)
         Returns:
             (NumPy Array): NumPy array of firm cdfs
         '''
         cdf_resolution = self.cdf_resolution
         measure = self.measure
-
-        ## Initialize cdf array
-        # Can't use self.n_firms() since data could be a subset of self
         n_firms = len(jids)
+
+        ## Initialize cdf array ##
         cdfs = np.zeros([n_firms, cdf_resolution])
 
         # Create quantiles of interest
         quantiles = np.linspace(1 / cdf_resolution, 1, cdf_resolution)
 
         # Group by income cdfs
         if measure == 'quantile_all':
+            # Convert columns to NumPy
+            j = frame.loc[:, 'j'].to_numpy()
+            y = frame.loc[:, 'y'].to_numpy()
+            w = frame.loc[:, 'row_weights'].to_numpy()
+
+            # Force j and jids to be integers so np.bincount and indexing work correctly
+            if jids.dtype == 'O':
+                jids = jids.astype(int, copy=True)
+            if j.dtype == 'O':
+                j = j.astype(int, copy=True)
+
             # Get quantiles from all data
-            quantile_groups = DescrStatsW(frame.loc[:, 'y'].to_numpy(), weights=frame.loc[:, 'row_weights'].to_numpy()).quantile(quantiles, return_pandas=False)
+            quantile_groups = DescrStatsW(y, weights=w).quantile(quantiles, return_pandas=False)
 
-            ## Generate firm-level cdfs
-            # Required for aggregate_transform
-            # NOTE: don't sort in-place, otherwise modifies external data
-            frame = frame.sort_values('j', inplace=False)
+            ## Generate firm-level cdfs ##
             for i, quant in enumerate(quantile_groups):
-                frame.loc[:, 'quant'] = (frame.loc[:, 'y'].to_numpy() <= quant).astype(int, copy=False)
-                cdfs_col = aggregate_transform(frame, col_groupby='j', col_grouped='quant', func='sum', weights='row_weights', merge=False) # aggregate(frame['fid'], firm_quant, func='sum', fill_value=-1)
-                cdfs[:, i] = cdfs_col[cdfs_col >= 0]
-            frame.drop('quant', axis=1, inplace=True)
-            del cdfs_col
+                # Weighted number of observations at or below quantile
+                cdfs[:, i] = np.bincount(j, w * (y <= quant))[jids]
 
             # Normalize by firm size (convert to cdf)
-            jsize = frame.groupby('j', sort=False)['row_weights'].sum().to_numpy()
+            jsize = np.bincount(j, w)[jids]
             cdfs = (cdfs.T / jsize.T).T
 
-        elif measure in ['quantile_firm_small', 'quantile_firm_large']:
-            # Sort frame by compensation (do this once now, so that don't need to do it again later) (also note it is faster to sort then manually compute quantiles than to use built-in quantile functions)
+        elif measure == 'quantile_firm':
+            # Sort frame by firm + compensation (do this once now, so that don't need to do it again later) (also note it is faster to sort and then manually compute quantiles than to use built-in quantile functions)
             # NOTE: don't sort in-place, otherwise modifies external data
-            frame = frame.sort_values('y', inplace=False)
+            frame = frame.sort_values(['j', 'y'], inplace=False)
+            frame.reset_index(drop=True, inplace=True)
+            frame.reset_index(drop=False, inplace=True)
+
+            # Convert columns to NumPy (after sorting)
+            y = frame.loc[:, 'y'].to_numpy()
+            w = frame.loc[:, 'row_weights'].to_numpy()
+
+            # Find min + max index for each firm
+            groupby_j = frame.groupby('j', sort=False)['index']
+            j_min_idx = groupby_j.min().to_numpy()
+            j_max_idx = groupby_j.max().to_numpy()
+            del groupby_j
 
-            if measure == 'quantile_firm_small':
-                # Convert pandas dataframe into a dictionary to access data faster
-                # Source for idea: https://stackoverflow.com/questions/57208997/looking-for-the-fastest-way-to-slice-a-row-in-a-huge-pandas-dataframe
-                # Source for how to actually format data correctly: https://stackoverflow.com/questions/56064677/pandas-series-to-dict-with-repeated-indices-make-dict-with-list-values
-                # frame_dict = frame['y'].groupby(level=0).agg(list).to_dict()
-                frame_groupby_j = frame.groupby('j')
-                frame_dict = frame_groupby_j['y'].agg(list).to_dict()
-                weights_dict = frame_groupby_j['row_weights'].agg(list).to_dict()
-                del frame_groupby_j
-                # frame.sort_values(['j', 'y'], inplace=True) # Required for aggregate_transform
-                # frame_dict = pd.Series(aggregate_transform(frame, col_groupby='j', col_grouped='y', func='array', merge=False), index=np.unique(frame['j'])).to_dict()
-                # with warnings.catch_warnings():
-                #     warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
-                #     frame_dict = pd.Series(aggregate(frame['j'], frame['y'], func='array', fill_value=[]), index=np.unique(frame['j'])).to_dict()
-
-            # Generate the cdfs
-            for i, jid in enumerate(jids):
+            ## Generate the cdfs ##
+            for j in range(n_firms):
                 # Get the firm-level compensation data (don't need to sort because already sorted)
-                if measure == 'quantile_firm_small':
-                    y = np.array(frame_dict[jid])
-                    w = np.array(weights_dict[jid])
-                elif measure == 'quantile_firm_large':
-                    y = frame.loc[frame.loc[:, 'j'].to_numpy() == jid, 'y'].to_numpy()
-                    w = frame.loc[frame.loc[:, 'j'].to_numpy() == jid, 'row_weights'].to_numpy()
+                y_j = y[j_min_idx[j]: j_max_idx[j] + 1]
+                w_j = w[j_min_idx[j]: j_max_idx[j] + 1]
+
                 # Cumulative weight
-                cum_w = w.cumsum()
+                cum_w = w_j.cumsum()
+
                 # Weighted number of observations
-                weighted_n = w.sum()
-                # Generate the firm-level cdf
-                # Note: update numpy array element by element
-                # Source: https://stackoverflow.com/questions/30012362/faster-way-to-convert-list-of-objects-to-numpy-array/30012403
-                for j, quantile in enumerate(quantiles):
-                    # index = max(len(y) * (j + 1) // cdf_resolution - 1, 0) # Don't want negative index
+                weighted_n = w_j.sum()
+
+                for q, quantile in enumerate(quantiles):
+                    ## Generate the firm-level cdf ##
                     # Income index at particular quantile
-                    index = 0
-                    for cum_w_val in cum_w[1:]:
-                        # Skip first weight because it is always true
+                    idx = 0
+                    for cum_w_val in cum_w:
                         if cum_w_val / weighted_n <= quantile:
-                            index += 1
+                            idx += 1
                         else:
                             break
                     # Update cdfs with the firm-level cdf
-                    cdfs[i, j] = y[index]
+                    cdfs[j, q] = y_j[min(idx, len(y_j) - 1)]
 
         return cdfs
 
 class Moments:
     '''
     Generate compensation moments for firms. Used for clustering.
 
@@ -119,35 +115,43 @@
     def __init__(self, measures='mean'):
         self.measures = measures
 
     def _compute_measure(self, frame, jids):
         '''
         Arguments:
             frame (Pandas DataFrame): data to use
-            jids (list): sorted list of firm ids in frame (since frame could be a subset of full dataset, this is not necessarily all firms in self)
+            jids (list): sorted list of firm ids in frame (since frame could be a subset of self, this is not necessarily all firms in self)
 
         Returns:
             (NumPy Array): NumPy array of firm moments
         '''
-        measures = self.measures
-
-        # Can't use data.n_firms() since data could be a subset of self
         n_firms = len(jids)
+        measures = self.measures
         n_measures = len(to_list(measures))
+
+        ## Initialize moments array ##
         moments = np.zeros([n_firms, n_measures])
 
         # Required for aggregate_transform
         # NOTE: don't sort in-place, otherwise modifies external data
         frame = frame.sort_values('j', inplace=False)
 
         for j, measure in enumerate(to_list(measures)):
             if measure == 'mean':
                 # Group by mean income
-                frame['one'] = 1
-                moments[:, j] = aggregate_transform(frame, 'j', 'y', 'sum', weights='row_weights', merge=False) / aggregate_transform(frame, 'j', 'one', 'sum', weights='row_weights', merge=False)
+                j_ = frame.loc[:, 'j'].to_numpy()
+                y = frame.loc[:, 'y'].to_numpy()
+                w = frame.loc[:, 'row_weights'].to_numpy()
+                # Force j and jids to be integers so np.bincount and indexing work correctly
+                if jids.dtype == 'O':
+                    jids = jids.astype(int, copy=True)
+                if j_.dtype == 'O':
+                    j_ = j_.astype(int, copy=True)
+                moments[:, j] = np.bincount(j_, w * y)[jids] / np.bincount(j_, w)[jids]
+                del j_, y, w
             elif measure == 'var':
                 # Group by variance of income
                 moments[:, j] = aggregate_transform(frame, 'j', 'y', 'var', weights='row_weights', merge=False)
             elif measure == 'max':
                 moments[:, j] = frame.groupby('j', sort=False)['y'].max().to_numpy()
             elif measure == 'min':
                 moments[:, j] = frame.groupby('j', sort=False)['y'].min().to_numpy()
```

### Comparing `bipartitepandas-1.1.5/bipartitepandas/simbipartite.py` & `bipartitepandas-1.1.6/bipartitepandas/simbipartite.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas/util.py` & `bipartitepandas-1.1.6/bipartitepandas/util.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/bipartitepandas.egg-info/PKG-INFO` & `bipartitepandas-1.1.6/bipartitepandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +65,9 @@
 
 Thibaut Lamadon,
 Assistant Professor in Economics, University of Chicago,
 lamadon@uchicago.edu
 
 
 Adam A. Oppenheimer,
-Research Professional, University of Chicago,
-oppenheimer@uchicago.edu
+Graduate Student, University of Minnesota - Twin Cities,
+oppen040@umn.edu
```

### Comparing `bipartitepandas-1.1.5/bipartitepandas.egg-info/SOURCES.txt` & `bipartitepandas-1.1.6/bipartitepandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/setup.cfg` & `bipartitepandas-1.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bipartitepandas
-version = 1.1.5
+version = 1.1.6
 author = Thibaut Lamadon
 author_email = thibaut.lamadon@gmail.com
 description = Python tools for bipartite labor data
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/tlamadon/bipartitepandas/
 project_urls =
```

### Comparing `bipartitepandas-1.1.5/tests/test_bpd.py` & `bipartitepandas-1.1.6/tests/test_bpd.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_base.py` & `bipartitepandas-1.1.6/tests/test_bpd_base.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_clustering.py` & `bipartitepandas-1.1.6/tests/test_bpd_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # Test cluster function is working correctly for long format.
     rng = np.random.default_rng(2345)
     nk = 10
     sim_data = bpd.SimBipartite(bpd.sim_params({'nk': nk})).simulate(rng)
     bdf = bpd.BipartiteLong(sim_data[['i', 'j', 'y', 't']])
     bdf = bdf.clean()
 
-    for measure in ['quantile_all', 'quantile_firm_small', 'quantile_firm_large']:
+    for measure in ['quantile_all', 'quantile_firm']:
         for stayers_movers in [None, 'stayers', 'movers']:
             measures = bpd.measures.CDFs(measure=measure)
             grouping = bpd.grouping.KMeans(n_clusters=nk)
             bdf = bdf.cluster(bpd.cluster_params({'measures': measures, 'grouping': grouping, 'stayers_movers': stayers_movers}), rng)
 
             clusters_true = sim_data[~bdf['g'].isna()]['psi'].astype('category', copy=False).cat.codes.astype(int, copy=False).to_numpy() # Skip firms that aren't clustered
             clusters_estimated = bdf[~bdf['g'].isna()]['g'].astype(int, copy=False).to_numpy() # Skip firms that aren't clustered
@@ -61,34 +61,32 @@
             match_df = pd.DataFrame({'psi': clusters_match, 'psi_est': matches_match}, index=np.arange(nk))
             # replace_df = replace_df.groupby('psi').apply(lambda a: a.value_counts().index[0][1])
 
             clusters_merged = pd.merge(pd.DataFrame({'psi': clusters_true}), match_df, how='left', on='psi')
 
             wrong_cluster = np.sum(clusters_merged['psi_est'] != clusters_estimated)
             if measure == 'quantile_all':
-                bound = 5000 # 10% error
-            elif measure == 'quantile_firm_small':
-                bound = 10000 # 20% error
-            elif measure == 'quantile_firm_large':
-                bound = 10000 # 20% error
+                bound = 1100 # 2.2% error
+            elif measure == 'quantile_firm':
+                bound = 1100 # 2.2% error
             if stayers_movers == 'stayers':
                 bound = 35000 # 70% error
 
             assert wrong_cluster < bound, 'error is {} for {}'.format(wrong_cluster, measure)
 
 def test_cluster_2():
     # Test cluster function is working correctly for event study format.
     rng = np.random.default_rng(3456)
     nk = 10
     sim_data = bpd.SimBipartite(bpd.sim_params({'nk': nk})).simulate(rng)
     bdf = bpd.BipartiteLong(sim_data[['i', 'j', 'y', 't']])
     bdf = bdf.clean()
     bdf = bdf.to_eventstudy()
 
-    for measure in ['quantile_all', 'quantile_firm_small', 'quantile_firm_large']:
+    for measure in ['quantile_all', 'quantile_firm']:
         for stayers_movers in [None, 'stayers', 'movers']:
             measures = bpd.measures.CDFs(measure=measure)
             grouping = bpd.grouping.KMeans(n_clusters=nk)
             bdf = bdf.cluster(bpd.cluster_params({'measures': measures, 'grouping': grouping, 'stayers_movers': stayers_movers}), rng)
 
             to_long = bdf.to_long()
             clusters_true = sim_data[~to_long['g'].isna()]['psi'].astype('category', copy=False).cat.codes.astype(int, copy=False).to_numpy() # Skip firms that aren't clustered
@@ -127,19 +125,17 @@
             match_df = pd.DataFrame({'psi': clusters_match, 'psi_est': matches_match}, index=np.arange(nk))
             # replace_df = replace_df.groupby('psi').apply(lambda a: a.value_counts().index[0][1])
 
             clusters_merged = pd.merge(pd.DataFrame({'psi': clusters_true}), match_df, how='left', on='psi')
 
             wrong_cluster = np.sum(clusters_merged['psi_est'] != clusters_estimated)
             if measure == 'quantile_all':
-                bound = 5000 # 10% error
-            elif measure == 'quantile_firm_small':
-                bound = 10000 # 20% error
-            elif measure == 'quantile_firm_large':
-                bound = 10500 # 21% error
+                bound = 1300 # 2.6% error
+            elif measure == 'quantile_firm':
+                bound = 2600 # 5.2% error
             if stayers_movers == 'stayers':
                 bound = 35000 # 70% error
 
             assert wrong_cluster < bound, 'error is {} for {}'.format(wrong_cluster, measure)
 
 def test_cluster_3():
     # Test cluster function is working correctly for collapsed long format.
@@ -152,15 +148,15 @@
     # Compute spells
     sim_data['i_l1'] = sim_data['i'].shift(1)
     sim_data['j_l1'] = sim_data['j'].shift(1)
     sim_data['new_spell'] = (sim_data['i'] != sim_data['i_l1']) | (sim_data['j'] != sim_data['j_l1'])
     sim_data['spell'] = sim_data['new_spell'].cumsum()
     sim_data_spell = sim_data.groupby('spell').first()
 
-    for measure in ['quantile_all', 'quantile_firm_small', 'quantile_firm_large']:
+    for measure in ['quantile_all', 'quantile_firm']:
         for stayers_movers in [None, 'stayers', 'movers']:
             measures = bpd.measures.CDFs(measure=measure)
             grouping = bpd.grouping.KMeans(n_clusters=nk)
             bdf = bdf.cluster(bpd.cluster_params({'measures': measures, 'grouping': grouping, 'stayers_movers': stayers_movers}), rng)
             remaining_jids = bdf.dropna()['j'].unique()
 
             clusters_true = sim_data_spell[sim_data_spell['j'].isin(remaining_jids)]['psi'].astype('category', copy=False).cat.codes.astype(int, copy=False).to_numpy() # Skip firms that aren't clustered
@@ -199,19 +195,17 @@
             match_df = pd.DataFrame({'psi': clusters_match, 'psi_est': matches_match}, index=np.arange(nk))
             # replace_df = replace_df.groupby('psi').apply(lambda a: a.value_counts().index[0][1])
 
             clusters_merged = pd.merge(pd.DataFrame({'psi': clusters_true}), match_df, how='left', on='psi')
 
             wrong_cluster = np.sum(clusters_merged['psi_est'] != clusters_estimated)
             if measure == 'quantile_all':
-                bound = 5000 # 10% error
-            elif measure == 'quantile_firm_small':
-                bound = 10000 # 20% error
-            elif measure == 'quantile_firm_large':
-                bound = 10000 # 20% error
+                bound = 800 # 1.6% error
+            elif measure == 'quantile_firm':
+                bound = 1900 # 3.8% error
             if stayers_movers == 'stayers':
                 bound = 35000 # 70% error
 
             assert wrong_cluster < bound, 'error is {} for {}'.format(wrong_cluster, measure)
 
 def test_cluster_4():
     # Test cluster function is working correctly for collapsed event study format.
@@ -224,15 +218,15 @@
     # Compute spells
     sim_data['i_l1'] = sim_data['i'].shift(1)
     sim_data['j_l1'] = sim_data['j'].shift(1)
     sim_data['new_spell'] = (sim_data['i'] != sim_data['i_l1']) | (sim_data['j'] != sim_data['j_l1'])
     sim_data['spell'] = sim_data['new_spell'].cumsum()
     sim_data_spell = sim_data.groupby('spell').first()
 
-    for measure in ['quantile_all', 'quantile_firm_small', 'quantile_firm_large']:
+    for measure in ['quantile_all', 'quantile_firm']:
         for stayers_movers in [None, 'stayers', 'movers']:
             measures = bpd.measures.CDFs(measure=measure)
             grouping = bpd.grouping.KMeans(n_clusters=nk)
             bdf = bdf.cluster(bpd.cluster_params({'measures': measures, 'grouping': grouping, 'stayers_movers': stayers_movers}), rng)
 
             collapse = bdf.to_long()
             remaining_jids = collapse.dropna()['j'].unique()
@@ -273,19 +267,17 @@
             match_df = pd.DataFrame({'psi': clusters_match, 'psi_est': matches_match}, index=np.arange(nk))
             # replace_df = replace_df.groupby('psi').apply(lambda a: a.value_counts().index[0][1])
 
             clusters_merged = pd.merge(pd.DataFrame({'psi': clusters_true}), match_df, how='left', on='psi')
 
             wrong_cluster = np.sum(clusters_merged['psi_est'] != clusters_estimated)
             if measure == 'quantile_all':
+                bound = 900 # 1.8% error
+            elif measure == 'quantile_firm':
                 bound = 5000 # 10% error
-            elif measure == 'quantile_firm_small':
-                bound = 10000 # 20% error
-            elif measure == 'quantile_firm_large':
-                bound = 10000 # 20% error
             if stayers_movers == 'stayers':
                 bound = 35000 # 70% error
 
             assert wrong_cluster < bound, 'error is {} for {}'.format(wrong_cluster, measure)
 
 def test_cluster_5():
     # Test cluster function works with moments-quantiles options.
```

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_connectedness.py` & `bipartitepandas-1.1.6/tests/test_bpd_connectedness.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_custom.py` & `bipartitepandas-1.1.6/tests/test_bpd_custom.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_df.py` & `bipartitepandas-1.1.6/tests/test_bpd_df.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_es.py` & `bipartitepandas-1.1.6/tests/test_bpd_es.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_es_collapsed.py` & `bipartitepandas-1.1.6/tests/test_bpd_es_collapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_long.py` & `bipartitepandas-1.1.6/tests/test_bpd_long.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.5/tests/test_bpd_long_collapsed.py` & `bipartitepandas-1.1.6/tests/test_bpd_long_collapsed.py`

 * *Files identical despite different names*

