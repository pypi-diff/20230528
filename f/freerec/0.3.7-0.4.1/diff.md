# Comparing `tmp/freerec-0.3.7.tar.gz` & `tmp/freerec-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.3.7.tar", last modified: Thu May 25 01:55:28 2023, max compression
+gzip compressed data, was "freerec-0.4.1.tar", last modified: Sun May 28 12:32:05 2023, max compression
```

## Comparing `freerec-0.3.7.tar` & `freerec-0.4.1.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.358850 freerec-0.3.7/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     3280 2023-05-25 01:55:28.357850 freerec-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     2815 2023-05-25 01:23:33.000000 freerec-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.250983 freerec-0.3.7/freerec/
--rw-rw-rw-   0        0        0      505 2023-05-25 01:50:18.000000 freerec-0.3.7/freerec/__init__.py
--rw-rw-rw-   0        0        0     4188 2023-03-27 11:31:30.000000 freerec-0.3.7/freerec/__main__.py
--rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.3.7/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.299849 freerec-0.3.7/freerec/data/
--rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/__init__.py
--rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.3.7/freerec/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.304858 freerec-0.3.7/freerec/data/datasets/
--rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.3.7/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    17997 2023-05-24 14:09:12.000000 freerec-0.3.7/freerec/data/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.307850 freerec-0.3.7/freerec/data/datasets/context/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.3.7/freerec/data/datasets/context/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/datasets/context/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.312850 freerec-0.3.7/freerec/data/datasets/general/
--rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/datasets/general/__init__.py
--rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.3.7/freerec/data/datasets/general/amazon.py
--rw-rw-rw-   0        0        0     3876 2023-04-26 08:41:43.000000 freerec-0.3.7/freerec/data/datasets/general/base.py
--rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.3.7/freerec/data/datasets/general/gowalla.py
--rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.3.7/freerec/data/datasets/general/movielens.py
--rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.3.7/freerec/data/datasets/general/yelp.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.314848 freerec-0.3.7/freerec/data/datasets/knowledge/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.3.7/freerec/data/datasets/knowledge/__init__.py
--rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/datasets/knowledge/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.327848 freerec-0.3.7/freerec/data/datasets/sequential/
--rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.3.7/freerec/data/datasets/sequential/__init__.py
--rw-rw-rw-   0        0        0    10771 2023-04-26 07:43:46.000000 freerec-0.3.7/freerec/data/datasets/sequential/amazon.py
--rw-rw-rw-   0        0        0     2820 2023-04-26 08:41:52.000000 freerec-0.3.7/freerec/data/datasets/sequential/base.py
--rw-rw-rw-   0        0        0     1756 2023-04-26 07:33:17.000000 freerec-0.3.7/freerec/data/datasets/sequential/movielens.py
--rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.3.7/freerec/data/datasets/sequential/steam.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.329848 freerec-0.3.7/freerec/data/datasets/session/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:38.000000 freerec-0.3.7/freerec/data/datasets/session/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/datasets/session/base.py
--rw-rw-rw-   0        0        0    29845 2023-04-25 10:57:51.000000 freerec-0.3.7/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.341851 freerec-0.3.7/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0     2177 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0    10217 2023-04-25 11:14:13.000000 freerec-0.3.7/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    17962 2023-04-25 11:11:28.000000 freerec-0.3.7/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     3228 2023-04-10 09:00:22.000000 freerec-0.3.7/freerec/data/postprocessing/source.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.350849 freerec-0.3.7/freerec/data/preprocessing/
--rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.3.7/freerec/data/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    21887 2023-05-23 13:18:29.000000 freerec-0.3.7/freerec/data/preprocessing/base.py
--rw-rw-rw-   0        0        0     9234 2023-05-23 13:15:06.000000 freerec-0.3.7/freerec/data/preprocessing/datasets.py
--rw-rw-rw-   0        0        0      807 2023-03-23 07:09:59.000000 freerec-0.3.7/freerec/data/tags.py
--rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.3.7/freerec/data/transformation.py
--rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.3.7/freerec/data/utils.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/dict2obj.py
--rw-rw-rw-   0        0        0    31403 2023-05-25 01:48:48.000000 freerec-0.3.7/freerec/launcher.py
--rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.3.7/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.356851 freerec-0.3.7/freerec/models/
--rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.3.7/freerec/models/base.py
--rw-rw-rw-   0        0        0    16699 2023-05-12 03:00:42.000000 freerec-0.3.7/freerec/parser.py
--rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.3.7/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 01:55:28.293849 freerec-0.3.7/freerec.egg-info/
--rw-rw-rw-   0        0        0     3280 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 01:55:28.000000 freerec-0.3.7/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 01:55:28.358850 freerec-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-05-25 01:54:47.000000 freerec-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.232179 freerec-0.4.1/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3280 2023-05-28 12:32:05.231179 freerec-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2815 2023-05-25 01:23:33.000000 freerec-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.159134 freerec-0.4.1/freerec/
+-rw-rw-rw-   0        0        0      505 2023-05-28 12:06:21.000000 freerec-0.4.1/freerec/__init__.py
+-rw-rw-rw-   0        0        0     4528 2023-05-25 13:17:13.000000 freerec-0.4.1/freerec/__main__.py
+-rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.4.1/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.196282 freerec-0.4.1/freerec/data/
+-rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.4.1/freerec/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.198279 freerec-0.4.1/freerec/data/datasets/
+-rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.4.1/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    19752 2023-05-28 05:44:01.000000 freerec-0.4.1/freerec/data/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.200279 freerec-0.4.1/freerec/data/datasets/context/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.4.1/freerec/data/datasets/context/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/context/base.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.207344 freerec-0.4.1/freerec/data/datasets/general/
+-rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/general/__init__.py
+-rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.4.1/freerec/data/datasets/general/amazon.py
+-rw-rw-rw-   0        0        0     3876 2023-04-26 08:41:43.000000 freerec-0.4.1/freerec/data/datasets/general/base.py
+-rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.4.1/freerec/data/datasets/general/gowalla.py
+-rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.4.1/freerec/data/datasets/general/movielens.py
+-rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.4.1/freerec/data/datasets/general/yelp.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.209348 freerec-0.4.1/freerec/data/datasets/knowledge/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.4.1/freerec/data/datasets/knowledge/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/knowledge/base.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.213926 freerec-0.4.1/freerec/data/datasets/sequential/
+-rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.4.1/freerec/data/datasets/sequential/__init__.py
+-rw-rw-rw-   0        0        0    10771 2023-04-26 07:43:46.000000 freerec-0.4.1/freerec/data/datasets/sequential/amazon.py
+-rw-rw-rw-   0        0        0     3037 2023-05-26 07:30:24.000000 freerec-0.4.1/freerec/data/datasets/sequential/base.py
+-rw-rw-rw-   0        0        0     1756 2023-04-26 07:33:17.000000 freerec-0.4.1/freerec/data/datasets/sequential/movielens.py
+-rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.4.1/freerec/data/datasets/sequential/steam.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.216926 freerec-0.4.1/freerec/data/datasets/session/
+-rw-rw-rw-   0        0        0       29 2023-05-26 06:43:44.000000 freerec-0.4.1/freerec/data/datasets/session/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-05-26 07:26:22.000000 freerec-0.4.1/freerec/data/datasets/session/base.py
+-rw-rw-rw-   0        0        0     1427 2023-05-28 06:05:18.000000 freerec-0.4.1/freerec/data/datasets/session/diginetica.py
+-rw-rw-rw-   0        0        0     3293 2023-05-28 06:04:35.000000 freerec-0.4.1/freerec/data/datasets/session/yoochoose.py
+-rw-rw-rw-   0        0        0    29845 2023-04-25 10:57:51.000000 freerec-0.4.1/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.225664 freerec-0.4.1/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0     7097 2023-05-28 11:51:29.000000 freerec-0.4.1/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0    11138 2023-05-28 11:39:12.000000 freerec-0.4.1/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    19079 2023-05-26 07:00:49.000000 freerec-0.4.1/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     3228 2023-04-10 09:00:22.000000 freerec-0.4.1/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.228179 freerec-0.4.1/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.4.1/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    22062 2023-05-28 05:33:20.000000 freerec-0.4.1/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0    12875 2023-05-28 05:48:08.000000 freerec-0.4.1/freerec/data/preprocessing/datasets.py
+-rw-rw-rw-   0        0        0      864 2023-05-25 12:55:38.000000 freerec-0.4.1/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.4.1/freerec/data/transformation.py
+-rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.4.1/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0    31054 2023-05-28 05:17:28.000000 freerec-0.4.1/freerec/launcher.py
+-rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.4.1/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.230179 freerec-0.4.1/freerec/models/
+-rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16699 2023-05-12 03:00:42.000000 freerec-0.4.1/freerec/parser.py
+-rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.4.1/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.190472 freerec-0.4.1/freerec.egg-info/
+-rw-rw-rw-   0        0        0     3280 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:32:05.232686 freerec-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-05-25 05:39:48.000000 freerec-0.4.1/setup.py
```

### Comparing `freerec-0.3.7/LICENSE` & `freerec-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/PKG-INFO` & `freerec-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.3.7
+Version: 0.4.1
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freerec-0.3.7/README.md` & `freerec-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/__main__.py` & `freerec-0.4.1/freerec/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def make(args):
     # Make dataset:
     #
     #    freerec make DATASET --root=../data
     #
     from .data.preprocessing import datasets
-    from .data.tags import USER, ITEM, TIMESTAMP
+    from .data.tags import USER, SESSION, ITEM, TIMESTAMP
 
     converter = getattr(datasets, args.dataset)(
         root=args.root,
         filename=args.filename
     )
 
     star4pos = args.star4pos
@@ -57,14 +57,22 @@
         fields = None if args.all else (USER.name, ITEM.name, TIMESTAMP.name)
         converter.make_sequential_dataset_by_ratio(
             star4pos=star4pos,
             kcore4user=kcore4user,
             kcore4item=kcore4item,
             fields=fields
         )
+    elif args.datatype == 'sess' and args.by == 'ratio':
+        fields = None if args.all else (SESSION.name, ITEM.name, TIMESTAMP.name)
+        converter.make_session_dataset(
+            star4pos=star4pos,
+            kcore4user=kcore4user,
+            kcore4item=kcore4item,
+            fields=fields
+        )
     else:
         raise ValueError(f"`{args.datatype}' type dataset cannot be made by `{args.by}'")
 
 def main():
     parser = argparse.ArgumentParser("FreeRec")
     subparsers = parser.add_subparsers()
 
@@ -89,15 +97,15 @@
     make_parser = subparsers.add_parser("make")
     make_parser.set_defaults(func=make)
 
     make_parser.add_argument("dataset", type=str, help="dataset name")
     make_parser.add_argument("--root", type=str, default=".", help="data")
     make_parser.add_argument("--filename", type=str, default=None, help="filename of Atomic files")
 
-    make_parser.add_argument("--datatype", type=str, choices=('gen', 'seq'), default='gen')
+    make_parser.add_argument("--datatype", type=str, choices=('gen', 'seq', 'sess'), default='gen')
     make_parser.add_argument("--by", type=str, choices=('ratio', 'last-two'), default='ratio')
 
     make_parser.add_argument("--star4pos", type=int, default=0, help="select interactions with `Rating > star4pos'")
     make_parser.add_argument("--kcore4user", type=int, default=10, help="select kcore interactions according to User")
     make_parser.add_argument("--kcore4item", type=int, default=10, help="select kcore interactions according to Item")
     make_parser.add_argument("--ratios", type=str, default="8,1,1", help="the ratios of training|validation|test set")
```

### Comparing `freerec-0.3.7/freerec/criterions.py` & `freerec-0.4.1/freerec/criterions.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/dataloader.py` & `freerec-0.4.1/freerec/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/base.py` & `freerec-0.4.1/freerec/data/datasets/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterator, Optional, TypeVar, Tuple
 
 import torch, os, abc
 import numpy as np
 import torchdata.datapipes as dp
 from freeplot.utils import import_pickle, export_pickle
 
-from ..tags import FieldTags, SPARSE, USER, ITEM, ID
+from ..tags import FieldTags, SPARSE, USER, SESSION, ITEM, ID
 from ..fields import Field, BufferField, FieldList, FieldTuple
 from ..utils import download_from_url, extract_archive
 from ...utils import timemeter, infoLogger, mkdirs, warnLogger
 
 
 __all__ = ['BaseSet', 'RecDataSet']
 
@@ -471,15 +471,16 @@
         A chunk of the pickle data.
         """
         datapipe = dp.iter.FileLister(
             os.path.join(
                 self.path,
                 DEFAULT_PICKLE_FMT.format(self.__class__.__name__),
                 self.mode
-            )
+            ),
+            non_deterministic=False # return sorted chunks
         )
         for file_ in datapipe:
             yield self.read_pickle(file_)
 
     @timemeter("DataSet/compile")
     def compile(self):
         r"""
@@ -541,10 +542,69 @@
         if self.mode == 'train':
             return self.trainsize
         elif self.mode == 'valid':
             return self.validsize
         else:
             return self.testsize
 
+    def to_seqs(self, master: Tuple = (USER, ID), keepid: bool = False):
+        r"""
+        Return dataset in sequence.
+
+        Parameters:
+        -----------
+        master: Tuple
+            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
+        keepid: bool, default to False
+            `True`: return list of (id, items)
+            `False`: return list of items
+        
+        Returns:
+        --------
+        List
+        """
+        Master = self.fields[master]
+        assert Master is not None, f"{Master} is not in fields ..."
+        seqs = [[] for id_ in range(Master.count)]
+
+        for chunk in self:
+            list(map(
+                lambda id_, item: seqs[id_].append(item),
+                chunk[master], chunk[ITEM, ID]
+            ))
+
+        if keepid:
+            seqs = [(id_, tuple(items)) for id_, items in enumerate(seqs)]
+        else:
+            seqs = [tuple(items) for items in seqs]
+
+        return seqs
+
+    def to_roll_seqs(self, master: Tuple = (USER, ID), minlen: int = 2):
+        r"""
+        Rolling dataset in sequence.
+
+        Parameters:
+        -----------
+        master: Tuple
+            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
+        minlen: int
+            Shorest sequence
+       
+        Returns:
+        --------
+        List
+        """
+        seqs = self.to_seqs(master=master, keepid=True)
+
+        roll_seqs = []
+        for id_, items in seqs:
+            for k in range(minlen, len(items) + 1):
+                roll_seqs.append(
+                    (id_, items[:k])
+                )
+
+        return roll_seqs
+
     def __str__(self) -> str:
         cfg = '\n'.join(map(str, self.fields))
         return f"[{self.__class__.__name__}] >>> \n" + cfg
```

### Comparing `freerec-0.3.7/freerec/data/datasets/general/amazon.py` & `freerec-0.4.1/freerec/data/datasets/general/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/general/base.py` & `freerec-0.4.1/freerec/data/datasets/general/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/general/gowalla.py` & `freerec-0.4.1/freerec/data/datasets/general/gowalla.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/general/movielens.py` & `freerec-0.4.1/freerec/data/datasets/general/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/general/yelp.py` & `freerec-0.4.1/freerec/data/datasets/general/yelp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/sequential/amazon.py` & `freerec-0.4.1/freerec/data/datasets/sequential/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/sequential/base.py` & `freerec-0.4.1/freerec/data/datasets/sequential/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 
+import numpy as np
 import torchdata.datapipes as dp
 
 from ..base import RecDataSet
 from ...tags import TIMESTAMP, USER, ITEM, ID
 from ...fields import Field, SparseField, DenseField
 from ....utils import infoLogger
 from ....dict2obj import Config
@@ -61,15 +62,20 @@
         return datapipe
 
     def summary(self):
         super().summary()
         from prettytable import PrettyTable
         User, Item = self.fields[USER, ID], self.fields[ITEM, ID]
 
-        table = PrettyTable(['#Users', '#Items', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
+        table = PrettyTable(['#Users', '#Items', 'Avg.Len', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
+        trainlens =  list(filter(lambda x: x > 0, [len(items) for items in self.train().to_seqs()]))
         table.add_row([
-            User.count, Item.count, self.trainsize + self.validsize + self.testsize,
+            User.count, Item.count, 
+            np.mean(
+                trainlens
+            ).item() + 2,
+            self.trainsize + self.validsize + self.testsize,
             self.trainsize, self.validsize, self.testsize,
             (self.trainsize + self.validsize + self.testsize) / (User.count * Item.count)
         ])
 
         infoLogger(table)
```

### Comparing `freerec-0.3.7/freerec/data/datasets/sequential/movielens.py` & `freerec-0.4.1/freerec/data/datasets/sequential/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/datasets/sequential/steam.py` & `freerec-0.4.1/freerec/data/datasets/sequential/steam.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/fields.py` & `freerec-0.4.1/freerec/data/fields.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/postprocessing/base.py` & `freerec-0.4.1/freerec/data/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/postprocessing/row.py` & `freerec-0.4.1/freerec/data/postprocessing/row.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torchdata.datapipes as dp
 from itertools import repeat, chain
 
 
 __all__ = [
     "DropEmpty", 
     "LeftPruningRow", "RightPruningRow",
+    "DropingDuplicates",
     "LeftShiftingRow", "RightShiftingRow",
     "LeftPaddingRow", "RightPaddingRow",
 ]
 
 
 #==================================Filter==================================
 class RowFilter(dp.iter.IterDataPipe):
@@ -233,14 +234,50 @@
             indices=indices
         )
 
     def _rprune(self, x):
         return x[:self.maxlen]
 
 
+@dp.functional_datapipe("drop_duplicates_")
+class DropingDuplicates(RowMapper):
+    r"""
+    A functional datapipe that drop the duplicates.
+
+    Parameters:
+    -----------
+    source_dp: IterDataPipe 
+        The input datapipe to prune.
+    indices : Iterable[int]
+        The indices of the elements in each row to which `fn` should be applied.
+    ordered: bool
+        `True`: keeping order.
+    """
+
+    def __init__(
+        self, source_dp: dp.iter.IterDataPipe, 
+        indices: Union[None, int, Iterable[int]],
+        ordered: bool = True
+    ) -> None:
+
+        self.ordered = ordered
+
+        super().__init__(
+            source_dp=source_dp, 
+            fn=self._drop_in_order if self.ordered else self._drop,
+            indices=indices
+        )
+
+    def _drop(self, x):
+        return list(set(x))
+
+    def _drop_in_order(self, x):
+        return sorted(set(x), key=x.index)
+
+
 @dp.functional_datapipe("lshift_")
 class LeftShiftingRow(RowMapper):
     r"""
     Mapper that left shifts the input data by a specified offset.
 
     Parameters:
     -----------
@@ -316,15 +353,15 @@
 
     Parameters:
     -----------
     source_dp : dp.iter.IterDataPipe
         The source data pipeline to operate on.
     indices : Iterable[int]
         The indices of the elements in each row to which `fn` should be applied.
-    max_len : int
+    maxlen : int
         The maximum length to pad the sequences to.
     padding_value : int, optional (default=0)
         The value to use for padding.
     """
 
     def __init__(
         self, source_dp: dp.iter.IterDataPipe, 
@@ -352,15 +389,15 @@
 
     Parameters:
     -----------
     source_dp : dp.iter.IterDataPipe
         The source data pipeline to operate on.
     indices : Iterable[int]
         The indices of the elements in each row to which `fn` should be applied.
-    max_len : int
+    maxlen : int
         The maximum length to right pad the sequences to.
     padding_value : int, optional (default=0)
         The value to use for padding.
     """
 
     def __init__(
         self, source_dp: dp.iter.IterDataPipe,
```

### Comparing `freerec-0.3.7/freerec/data/postprocessing/sampler.py` & `freerec-0.4.1/freerec/data/postprocessing/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 
 
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 import random
 import torchdata.datapipes as dp
 
 from .base import Postprocessor
 from ..datasets.base import RecDataSet
 from ..fields import SparseField
-from ..tags import USER, ITEM, ID
+from ..tags import USER, SESSION, ITEM, ID
 from ...utils import timemeter
 
 
 __all__ = [
     'GenTrainUniformSampler', 'GenValidYielder', 'GenTestYielder',
     'SeqTrainYielder', 'SeqValidYielder', 'SeqTestYielder', 
-    'SeqTrainUniformSampler', 'SeqValidSampler', 'SeqTestSampler'
+    'SeqTrainUniformSampler', 'SeqValidSampler', 'SeqTestSampler',
+    'SessTrainYielder', 'SessValidYielder', 'SessTestYielder', 
 ]
 
 
 #===============================For General Recommendation===============================
 
 @dp.functional_datapipe("gen_train_uniform_sampling_")
 class GenTrainUniformSampler(Postprocessor):
@@ -344,24 +345,14 @@
                 posItems = self.posItems[user]
                 # (user, seqs, unseen, seen)
                 yield [user, posItems[:-1], posItems[-1:], posItems[:-1]]
 
 
 @dp.functional_datapipe("seq_test_yielding_")
 class SeqTestYielder(SeqValidYielder):
-    r"""
-    A functional datapipe for yielding (user, positives, targets).
-
-    Parameters:
-    -----------
-    source_dp: dp.iter.IterableWrapper 
-        A datapipe that yields users.
-    dataset: RecDataSet 
-        The dataset object that contains field objects.
-    """
 
     @timemeter("SeqTestYielder/prepare")
     def prepare(self, dataset: RecDataSet):
         r"""
         Prepare the data before yielding.
 
         Parameters:
@@ -547,8 +538,53 @@
         )
 
         for chunk in dataset.test():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
-        self.posItems = [tuple(items) for items in self.posItems]
+        self.posItems = [tuple(items) for items in self.posItems]
+
+
+#===============================For Session Recommendation===============================
+
+
+@dp.functional_datapipe("sess_train_yielding_")
+class SessTrainYielder(Postprocessor):
+    r"""
+    A functional datapipe for yielding (sess, sequences, targets).
+
+    Parameters:
+    -----------
+    source_dp: dp.iter.IterableWrapper 
+        A datapipe that yields users.
+    dataset: RecDataSet 
+        The dataset object that contains field objects.
+    """
+
+    def __init__(
+        self, source_dp: dp.iter.IterableWrapper,
+        dataset: Optional[RecDataSet] = None,
+    ) -> None:
+        super().__init__(source_dp)
+
+    def _check(self, sequence) -> bool:
+        return len(sequence) > 1
+
+    def __iter__(self):
+        for sess, sequence in self.source:
+            if self._check(sequence):
+                yield [sess, sequence[:-1], sequence[-1:]]
+
+
+@dp.functional_datapipe("sess_valid_yielding_")
+class SessValidYielder(SessTrainYielder):
+
+    def __iter__(self):
+        for sess, sequence in self.source:
+            if self._check(sequence):
+                # (user, seqs, unseen, seen)
+                yield [sess, sequence[:-1], sequence[-1:], sequence[:-1]]
+
+
+@dp.functional_datapipe("sess_test_yielding_")
+class SessTestYielder(SessValidYielder): ...
```

### Comparing `freerec-0.3.7/freerec/data/postprocessing/source.py` & `freerec-0.4.1/freerec/data/postprocessing/source.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/preprocessing/base.py` & `freerec-0.4.1/freerec/data/preprocessing/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from typing import Tuple, Iterable, Optional, Union, Mapping
 
 import os, random
 import numpy as np
 import pandas as pd
 from math import floor, ceil
 
-from ..tags import USER, ITEM, RATING, TIMESTAMP
+from ..tags import USER, SESSION, ITEM, RATING, TIMESTAMP
 
 from ...utils import infoLogger, warnLogger, mkdirs
 
 
 __all__ = ['AtomicConverter']
 
 
 NAME_FORMAT_DICT = {
     'user_id': USER.name,
+    'session_id': SESSION.name,
     'item_id': ITEM.name,
     'venue_id': ITEM.name, # FourSquare
     'rating': RATING.name,
     'timestamp': TIMESTAMP.name
 }
 
 
@@ -205,15 +206,16 @@
             )
     
     def filter_by_core(
         self,
         low4user: Union[None, int, float] = None, 
         high4user: Union[None, int, float] = None,
         low4item: Union[None, int, float] = None, 
-        high4item: Union[None, int, float] = None
+        high4item: Union[None, int, float] = None,
+        master: str = USER.name
     ):
         r"""
         Filter (user, item) by k-core settings.
 
         Parameters:
         -----------
         low4user: int, float, optional
@@ -233,22 +235,22 @@
         high4user = high4user if high4user else float('inf')
         low4item = low4item if low4item else float('-inf')
         high4item = high4item if high4item else float('inf')
         df = self.interactions
         dsz = -1
         infoLogger(
             f"[Converter] >>> Filter dataframe: "
-            f"User in [{low4user}, {high4user}]; "
+            f"{master} in [{low4user}, {high4user}]; "
             f"Item in [{low4item}, {high4item}] ..."
         )
         infoLogger(f"[Converter] >>> Current datasize: {len(df)} ...")
         while dsz != len(df):
             dsz = len(df)
             # filter by user
-            users = df[USER.name]
+            users = df[master]
             counts = users.value_counts()
             bool_indices = users.isin(
                 counts[(low4user <= counts) & (counts <= high4user)].index
             )
             df = df[bool_indices]
 
             # filter by item
@@ -259,30 +261,30 @@
             )
             df = df[bool_indices]
 
             infoLogger(f"[Converter] >>> Current datasize: {len(df)}")
 
         self.interactions = df
 
-    def user2token(self):
+    def user2token(self, master: str = USER.name):
         infoLogger(f"[Converter] >>> Map user ID to Token ...")
-        user_ids = sorted(self.interactions[USER.name].unique().tolist())
+        user_ids = sorted(self.interactions[master].unique().tolist())
         self.userCount = len(user_ids)
 
         user_tokens = list(range(len(user_ids)))
         self.userMaps = dict(
             zip(user_ids, user_tokens)
         )
 
         if self.userFeats is not None:
-            self.userFeats = self.userFeats[self.userFeats[USER.name].isin(user_ids)]
-            self.userFeats = self.userFeats.sort_values([USER.name])
+            self.userFeats = self.userFeats[self.userFeats[master].isin(user_ids)]
+            self.userFeats = self.userFeats.sort_values([master])
 
         self.map_col(
-            USER.name, self.userMaps, 
+            master, self.userMaps, 
             pools=(self.interactions, self.userFeats)
         )
 
     def item2token(self):
         infoLogger(f"[Converter] >>> Map item ID to Token ...")
         item_ids = sorted(self.interactions[ITEM.name].unique().tolist())
         self.itemCount = len(item_ids)
@@ -297,22 +299,22 @@
             self.itemFeats = self.itemFeats.sort_values([ITEM.name])
 
         self.map_col(
             ITEM.name, self.itemMaps, 
             pools=(self.interactions, self.itemFeats)
         )
 
-    def sort_by_timestamp(self):
+    def sort_by_timestamp(self, master: str = USER.name):
         df = self.interactions
         try:
-            df = df.sort_values(by=[USER.name, TIMESTAMP.name])
-            infoLogger(f"[Converter] >>> Sort by [{USER.name}] [{TIMESTAMP.name}] ...")
+            df = df.sort_values(by=[master, TIMESTAMP.name])
+            infoLogger(f"[Converter] >>> Sort by [{master}] [{TIMESTAMP.name}] ...")
         except KeyError:
-            df = df.sort_values(by=[USER.name])
-            infoLogger(f"[Converter] >>> Sort by [{USER.name}] ...")
+            df = df.sort_values(by=[master])
+            infoLogger(f"[Converter] >>> Sort by [{master}] ...")
         finally:
             self.interactions = df
 
     def gen_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
         traingroups = []
         validgroups = []
@@ -370,27 +372,27 @@
         self.trainiter = pd.concat(traingroups).reset_index(drop=True)
         self.validiter = pd.concat(validgroups).reset_index(drop=True)
         self.testiter = pd.concat(testgroups).reset_index(drop=True)
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(USER.name)[TIMESTAMP.name].min().sort_values().index)
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
         validgroups = groups[l:r]
         testgroups = groups[r:]
 
-        self.trainiter = self.interactions[self.interactions[USER.name].isin(traingroups)]
-        self.validiter = self.interactions[self.interactions[USER.name].isin(validgroups)]
-        self.testiter = self.interactions[self.interactions[USER.name].isin(testgroups)]
+        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
+        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
+        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
 
     def save(self, path: str):
         mkdirs(path)
 
         infoLogger(f"[Converter] >>> Save `train.txt' to {path} ...")
         df = pd.DataFrame(self.trainiter)
         df.to_csv(os.path.join(path, 'train.txt'), sep='\t', index=False)
@@ -542,22 +544,21 @@
         path = os.path.join(
             self.root, 'Sequential', 
             '_'.join([self.dataset, code, 'Chron'])
         )
 
         self.save(path)
 
-
     def make_session_dataset(
         self,
         star4pos: int = 0,
         kcore4user: int = 2,
         kcore4item: int = 5,
         ratios: Tuple[int, int, int] = (8, 1, 1),
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name),
+        fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
     ):
         r"""
         Make session dataset by ratios.
 
         Flows:
         ------
         1. filter out `inactive' items and short sessions;
@@ -574,18 +575,18 @@
         ratios: Tuple[int, int, int], default to (8, 1, 1)
             The ratios of training|validation|test set.
         fields: Iterable[str], default to (User, Item, Timestamp)
             The fields reserved.
         """
         self.load()
         self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item)
-        self.user2token()
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name)
+        self.user2token(master=SESSION.name)
         self.item2token()
-        self.sort_by_timestamp()
+        self.sort_by_timestamp(master=SESSION.name)
         if fields:
             self.reserve(fields)
         self.sess_split_by_ratio(ratios)
 
         code = f"{kcore4user}{kcore4item}{star4pos}{''.join(map(str, ratios))}"
         path = os.path.join(
             self.root, 'Session',
```

### Comparing `freerec-0.3.7/freerec/data/tags.py` & `freerec-0.4.1/freerec/data/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class FieldTags(Enum):
     Sparse = 'Sparse'
     Dense = 'Dense'
     User = 'User'
     Item = 'Item'
+    Session = 'Session'
     Interaction = 'Interaction'
     Timestamp = 'Timestamp'
     Rating = 'Rating'
     ID = 'ID'
     Feature = 'Feature'
     Target = 'Target'
     Positive = 'Positive'
@@ -20,14 +21,15 @@
     Unseen = 'Unseen'
 
 
 SPARSE = FieldTags('Sparse')
 DENSE = FieldTags('Dense')
 USER = FieldTags('User')
 ITEM = FieldTags('Item')
+SESSION = FieldTags('Session')
 INTERACTION = FieldTags('Interaction')
 TIMESTAMP = FieldTags('Timestamp')
 RATING = FieldTags('Rating')
 ID = FieldTags('ID')
 FEATURE = FieldTags('Feature')
 TARGET = FieldTags('Target')
 POSITIVE = FieldTags('Positive')
```

### Comparing `freerec-0.3.7/freerec/data/transformation.py` & `freerec-0.4.1/freerec/data/transformation.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/data/utils.py` & `freerec-0.4.1/freerec/data/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/dict2obj.py` & `freerec-0.4.1/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/launcher.py` & `freerec-0.4.1/freerec/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,1961 +3,1939 @@
 00000020: 6162 6c65 2c20 4974 6572 6162 6c65 2c20  able, Iterable, 
 00000030: 4c69 7374 2c20 4469 6374 2c20 4f70 7469  List, Dict, Opti
 00000040: 6f6e 616c 2c20 5475 706c 652c 2055 6e69  onal, Tuple, Uni
 00000050: 6f6e 0d0a 0d0a 696d 706f 7274 2074 6f72  on....import tor
 00000060: 6368 2c20 6162 632c 206f 732c 2074 696d  ch, abc, os, tim
 00000070: 652c 2073 7973 2c20 7369 676e 616c 2c20  e, sys, signal, 
 00000080: 7073 7574 696c 2c20 6174 6578 6974 0d0a  psutil, atexit..
-00000090: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-000000a0: 2070 640d 0a66 726f 6d20 746f 7263 6864   pd..from torchd
-000000b0: 6174 612e 6461 7461 7069 7065 732e 6974  ata.datapipes.it
-000000c0: 6572 2069 6d70 6f72 7420 4974 6572 4461  er import IterDa
-000000d0: 7461 5069 7065 0d0a 6672 6f6d 2074 6f72  taPipe..from tor
-000000e0: 6368 2e75 7469 6c73 2e74 656e 736f 7262  ch.utils.tensorb
-000000f0: 6f61 7264 2069 6d70 6f72 7420 5375 6d6d  oard import Summ
-00000100: 6172 7957 7269 7465 720d 0a66 726f 6d20  aryWriter..from 
-00000110: 6675 6e63 746f 6f6c 7320 696d 706f 7274  functools import
-00000120: 2070 6172 7469 616c 0d0a 6672 6f6d 2069   partial..from i
-00000130: 7465 7274 6f6f 6c73 2069 6d70 6f72 7420  tertools import 
-00000140: 7072 6f64 7563 740d 0a66 726f 6d20 636f  product..from co
-00000150: 6c6c 6563 7469 6f6e 7320 696d 706f 7274  llections import
-00000160: 2064 6566 6175 6c74 6469 6374 0d0a 6672   defaultdict..fr
-00000170: 6f6d 2066 7265 6570 6c6f 742e 7574 696c  om freeplot.util
-00000180: 7320 696d 706f 7274 2069 6d70 6f72 745f  s import import_
-00000190: 7069 636b 6c65 2c20 6578 706f 7274 5f70  pickle, export_p
-000001a0: 6963 6b6c 650d 0a0d 0a66 726f 6d20 2e64  ickle....from .d
-000001b0: 6174 612e 6669 656c 6473 2069 6d70 6f72  ata.fields impor
-000001c0: 7420 4669 656c 644d 6f64 756c 652c 2046  t FieldModule, F
-000001d0: 6965 6c64 5475 706c 650d 0a66 726f 6d20  ieldTuple..from 
-000001e0: 2e64 6174 612e 6461 7461 6c6f 6164 6572  .data.dataloader
-000001f0: 2069 6d70 6f72 7420 4461 7461 4c6f 6164   import DataLoad
-00000200: 6572 0d0a 6672 6f6d 202e 6d6f 6465 6c73  er..from .models
-00000210: 2069 6d70 6f72 7420 5265 6353 7973 4172   import RecSysAr
-00000220: 6368 0d0a 6672 6f6d 202e 6372 6974 6572  ch..from .criter
-00000230: 696f 6e73 2069 6d70 6f72 7420 4261 7365  ions import Base
-00000240: 4372 6974 6572 696f 6e0d 0a66 726f 6d20  Criterion..from 
-00000250: 2e64 6963 7432 6f62 6a20 696d 706f 7274  .dict2obj import
-00000260: 2043 6f6e 6669 670d 0a66 726f 6d20 2e75   Config..from .u
-00000270: 7469 6c73 2069 6d70 6f72 7420 4176 6572  tils import Aver
-00000280: 6167 654d 6574 6572 2c20 4d6f 6e69 746f  ageMeter, Monito
-00000290: 722c 2074 696d 656d 6574 6572 2c20 696e  r, timemeter, in
-000002a0: 666f 4c6f 6767 6572 0d0a 6672 6f6d 202e  foLogger..from .
-000002b0: 6d65 7472 6963 7320 696d 706f 7274 202a  metrics import *
-000002c0: 0d0a 6672 6f6d 202e 7061 7273 6572 2069  ..from .parser i
-000002d0: 6d70 6f72 7420 5449 4d45 0d0a 0d0a 0d0a  mport TIME......
-000002e0: 5f5f 616c 6c5f 5f20 3d20 5b27 4368 6965  __all__ = ['Chie
-000002f0: 6643 6f61 6368 272c 2027 436f 6163 6827  fCoach', 'Coach'
-00000300: 2c20 2741 6461 7074 6572 275d 0d0a 0d0a  , 'Adapter']....
-00000310: 0d0a 4445 4641 554c 545f 4d45 5452 4943  ..DEFAULT_METRIC
-00000320: 5320 3d20 7b0d 0a20 2020 2027 4c4f 5353  S = {..    'LOSS
-00000330: 273a 206c 616d 6264 6120 783a 2078 2c0d  ': lambda x: x,.
-00000340: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00000350: 2323 0d0a 2020 2020 274d 5345 273a 206d  ##..    'MSE': m
-00000360: 6561 6e5f 7371 7561 7265 645f 6572 726f  ean_squared_erro
-00000370: 722c 0d0a 2020 2020 274d 4145 273a 206d  r,..    'MAE': m
-00000380: 6561 6e5f 6162 735f 6572 726f 722c 0d0a  ean_abs_error,..
-00000390: 2020 2020 2752 4d53 4527 3a20 726f 6f74      'RMSE': root
-000003a0: 5f6d 7365 2c0d 0a20 2020 2023 2323 2323  _mse,..    #####
-000003b0: 2323 2323 2323 2323 0d0a 2020 2020 2750  ########..    'P
-000003c0: 5245 4349 5349 4f4e 273a 2070 7265 6369  RECISION': preci
-000003d0: 7369 6f6e 2c0d 0a20 2020 2027 5245 4341  sion,..    'RECA
-000003e0: 4c4c 273a 2072 6563 616c 6c2c 0d0a 2020  LL': recall,..  
-000003f0: 2020 2746 3127 3a20 6631 5f73 636f 7265    'F1': f1_score
-00000400: 2c0d 0a20 2020 2027 4155 4327 3a20 6175  ,..    'AUC': au
-00000410: 726f 632c 0d0a 2020 2020 2748 4954 5241  roc,..    'HITRA
-00000420: 5445 273a 2068 6974 5f72 6174 652c 0d0a  TE': hit_rate,..
-00000430: 2020 2020 2323 2323 2323 2323 2323 2323      ############
-00000440: 230d 0a20 2020 2027 4e44 4347 273a 206e  #..    'NDCG': n
-00000450: 6f72 6d61 6c69 7a65 645f 6463 672c 0d0a  ormalized_dcg,..
-00000460: 2020 2020 274d 5252 273a 206d 6561 6e5f      'MRR': mean_
-00000470: 7265 6369 7072 6f63 616c 5f72 616e 6b2c  reciprocal_rank,
-00000480: 0d0a 2020 2020 274d 4150 273a 206d 6561  ..    'MAP': mea
-00000490: 6e5f 6176 6572 6167 655f 7072 6563 6973  n_average_precis
-000004a0: 696f 6e0d 0a7d 0d0a 0d0a 4445 4641 554c  ion..}....DEFAUL
-000004b0: 545f 464d 5453 203d 207b 0d0a 2020 2020  T_FMTS = {..    
-000004c0: 274c 4f53 5327 3a20 222e 3566 222c 0d0a  'LOSS': ".5f",..
-000004d0: 2020 2020 2323 2323 2323 2323 2323 2323      ############
-000004e0: 230d 0a20 2020 2027 4d53 4527 3a20 222e  #..    'MSE': ".
-000004f0: 3466 222c 0d0a 2020 2020 274d 4145 273a  4f",..    'MAE':
-00000500: 2022 2e34 6622 2c0d 0a20 2020 2027 524d   ".4f",..    'RM
-00000510: 5345 273a 2022 2e34 6622 2c0d 0a20 2020  SE': ".4f",..   
-00000520: 2023 2323 2323 2323 2323 2323 2323 0d0a   #############..
-00000530: 2020 2020 2750 5245 4349 5349 4f4e 273a      'PRECISION':
-00000540: 2022 2e34 6622 2c0d 0a20 2020 2027 5245   ".4f",..    'RE
-00000550: 4341 4c4c 273a 2022 2e34 6622 2c0d 0a20  CALL': ".4f",.. 
-00000560: 2020 2027 4631 273a 2022 2e34 6622 2c0d     'F1': ".4f",.
-00000570: 0a20 2020 2027 4155 4327 3a20 222e 3466  .    'AUC': ".4f
-00000580: 222c 0d0a 2020 2020 2748 4954 5241 5445  ",..    'HITRATE
-00000590: 273a 2022 2e34 6622 2c0d 0a20 2020 2023  ': ".4f",..    #
-000005a0: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-000005b0: 2020 274e 4443 4727 3a20 222e 3466 222c    'NDCG': ".4f",
-000005c0: 0d0a 2020 2020 274d 5252 273a 2022 2e34  ..    'MRR': ".4
-000005d0: 6622 2c0d 0a20 2020 2027 4d41 5027 3a20  f",..    'MAP': 
-000005e0: 222e 3466 222c 0d0a 7d0d 0a0d 0a44 4546  ".4f",..}....DEF
-000005f0: 4155 4c54 5f42 4553 545f 4341 5354 4552  AULT_BEST_CASTER
-00000600: 203d 207b 0d0a 2020 2020 274c 4f53 5327   = {..    'LOSS'
-00000610: 3a20 6d69 6e2c 0d0a 2020 2020 2323 2323  : min,..    ####
-00000620: 2323 2323 2323 2323 230d 0a20 2020 2027  #########..    '
-00000630: 4d53 4527 3a20 6d69 6e2c 0d0a 2020 2020  MSE': min,..    
-00000640: 274d 4145 273a 206d 696e 2c0d 0a20 2020  'MAE': min,..   
-00000650: 2027 524d 5345 273a 206d 696e 2c0d 0a20   'RMSE': min,.. 
-00000660: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-00000670: 0d0a 2020 2020 2750 5245 4349 5349 4f4e  ..    'PRECISION
-00000680: 273a 206d 6178 2c0d 0a20 2020 2027 5245  ': max,..    'RE
-00000690: 4341 4c4c 273a 206d 6178 2c0d 0a20 2020  CALL': max,..   
-000006a0: 2027 4631 273a 206d 6178 2c0d 0a20 2020   'F1': max,..   
-000006b0: 2027 4155 4327 3a20 6d61 782c 0d0a 2020   'AUC': max,..  
-000006c0: 2020 2748 4954 5241 5445 273a 206d 6178    'HITRATE': max
-000006d0: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
-000006e0: 2323 2323 0d0a 2020 2020 274e 4443 4727  ####..    'NDCG'
-000006f0: 3a20 6d61 782c 0d0a 2020 2020 274d 5252  : max,..    'MRR
-00000700: 273a 206d 6178 2c0d 0a20 2020 2027 4d41  ': max,..    'MA
-00000710: 5027 3a20 6d61 782c 0d0a 7d0d 0a0d 0a0d  P': max,..}.....
-00000720: 0a63 6c61 7373 205f 4475 6d6d 794d 6f64  .class _DummyMod
-00000730: 756c 6528 746f 7263 682e 6e6e 2e4d 6f64  ule(torch.nn.Mod
-00000740: 756c 6529 3a0d 0a20 2020 2022 2222 5468  ule):..    """Th
-00000750: 6973 2069 7320 6120 6475 6d6d 7920 6d6f  is is a dummy mo
-00000760: 6475 6c65 2074 6861 7420 7365 7276 6573  dule that serves
-00000770: 2061 7320 6120 706c 6163 6568 6f6c 6465   as a placeholde
-00000780: 7220 666f 7220 6120 7265 616c 206d 6f64  r for a real mod
-00000790: 656c 2e22 2222 0d0a 2020 2020 6465 6620  el."""..    def 
-000007a0: 666f 7277 6172 6428 7365 6c66 2c20 2a61  forward(self, *a
-000007b0: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-000007c0: 0a20 2020 2020 2020 2022 2222 4475 6d6d  .        """Dumm
-000007d0: 7920 666f 7277 6172 6420 6d65 7468 6f64  y forward method
-000007e0: 2074 6861 7420 7261 6973 6573 2061 2060   that raises a `
-000007f0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000800: 726f 7260 2e22 2222 0d0a 2020 2020 2020  ror`."""..      
-00000810: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-00000820: 6d65 6e74 6564 4572 726f 7228 224e 6f20  mentedError("No 
-00000830: 6d6f 6465 6c20 6176 6169 6c61 626c 6520  model available 
-00000840: 666f 7220 436f 6163 6820 2e2e 2e22 290d  for Coach ...").
-00000850: 0a0d 0a20 2020 2064 6566 2073 7465 7028  ...    def step(
-00000860: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-00000870: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00000880: 2022 2222 4475 6d6d 7920 7374 6570 206d   """Dummy step m
-00000890: 6574 686f 6420 7468 6174 2072 6169 7365  ethod that raise
-000008a0: 7320 6120 604e 6f74 496d 706c 656d 656e  s a `NotImplemen
-000008b0: 7465 6445 7272 6f72 602e 2222 220d 0a20  tedError`.""".. 
-000008c0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-000008d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000008e0: 2822 4e6f 206f 7074 696d 697a 6572 206f  ("No optimizer o
-000008f0: 7220 6c72 2073 6368 6564 756c 6572 2061  r lr scheduler a
-00000900: 7661 696c 6162 6c65 2066 6f72 2043 6f61  vailable for Coa
-00000910: 6368 202e 2e2e 2229 0d0a 0d0a 2020 2020  ch ...")....    
-00000920: 6465 6620 6261 636b 7761 7264 2873 656c  def backward(sel
-00000930: 662c 202a 6172 6773 2c20 2a2a 6b77 6172  f, *args, **kwar
-00000940: 6773 293a 0d0a 2020 2020 2020 2020 2222  gs):..        ""
-00000950: 2244 756d 6d79 2062 6163 6b77 6172 6420  "Dummy backward 
-00000960: 6d65 7468 6f64 2074 6861 7420 7261 6973  method that rais
-00000970: 6573 2061 2060 4e6f 7449 6d70 6c65 6d65  es a `NotImpleme
-00000980: 6e74 6564 4572 726f 7260 2e22 2222 0d0a  ntedError`."""..
-00000990: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-000009a0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-000009b0: 7228 224e 6f20 6f70 7469 6d69 7a65 7220  r("No optimizer 
-000009c0: 6176 6169 6c61 626c 6520 666f 7220 436f  available for Co
-000009d0: 6163 6820 2e2e 2e22 290d 0a0d 0a0d 0a63  ach ...")......c
-000009e0: 6c61 7373 2043 6869 6566 436f 6163 6828  lass ChiefCoach(
-000009f0: 6d65 7461 636c 6173 733d 6162 632e 4142  metaclass=abc.AB
-00000a00: 434d 6574 6129 3a0d 0a20 2020 2072 2222  CMeta):..    r""
-00000a10: 2220 0d0a 2020 2020 5468 6520 6043 6869  " ..    The `Chi
-00000a20: 6566 436f 6163 6860 2063 6c61 7373 2069  efCoach` class i
-00000a30: 7320 7468 6520 746f 702d 6c65 7665 6c20  s the top-level 
-00000a40: 636c 6173 7320 666f 7220 7275 6e6e 696e  class for runnin
-00000a50: 6720 7468 6520 7472 6169 6e69 6e67 2061  g the training a
-00000a60: 6e64 2065 7661 6c75 6174 696f 6e20 6c6f  nd evaluation lo
-00000a70: 6f70 732e 0d0a 0d0a 2020 2020 5061 7261  ops.....    Para
-00000a80: 6d65 7465 7273 3a0d 0a20 2020 202d 2d2d  meters:..    ---
-00000a90: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 7472  --------..    tr
-00000aa0: 6169 6e70 6970 6520 3a20 4974 6572 4461  ainpipe : IterDa
-00000ab0: 7461 5069 7065 0d0a 2020 2020 2020 2020  taPipe..        
-00000ac0: 4974 6572 6162 6c65 2064 6174 6120 7069  Iterable data pi
-00000ad0: 7065 6c69 6e65 2066 6f72 2074 7261 696e  peline for train
-00000ae0: 696e 6720 6461 7461 2e0d 0a20 2020 2076  ing data...    v
-00000af0: 616c 6964 7069 7065 203a 2049 7465 7244  alidpipe : IterD
-00000b00: 6174 6150 6970 652c 206f 7074 696f 6e61  ataPipe, optiona
-00000b10: 6c0d 0a20 2020 2020 2020 2049 7465 7261  l..        Itera
-00000b20: 626c 6520 6461 7461 2070 6970 656c 696e  ble data pipelin
-00000b30: 6520 666f 7220 7661 6c69 6461 7469 6f6e  e for validation
-00000b40: 2064 6174 612e 0d0a 2020 2020 2020 2020   data...        
-00000b50: 4966 2060 4e6f 6e65 602c 2075 7365 2060  If `None`, use `
-00000b60: 7472 6169 6e70 6970 6560 2069 6e73 7465  trainpipe` inste
-00000b70: 6164 2e0d 0a20 2020 2074 6573 7470 6970  ad...    testpip
-00000b80: 6520 3a20 4974 6572 4461 7461 5069 7065  e : IterDataPipe
-00000b90: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00000ba0: 2020 2020 4974 6572 6162 6c65 2064 6174      Iterable dat
-00000bb0: 6120 7069 7065 6c69 6e65 2066 6f72 2074  a pipeline for t
-00000bc0: 6573 7469 6e67 2064 6174 612e 0d0a 2020  esting data...  
-00000bd0: 2020 2020 2020 4966 2060 4e6f 6e65 602c        If `None`,
-00000be0: 2075 7365 2060 7661 6c69 6470 6970 6560   use `validpipe`
-00000bf0: 2069 6e73 7465 6164 2e0d 0a20 2020 2066   instead...    f
-00000c00: 6965 6c64 7320 3a20 4974 6572 6162 6c65  ields : Iterable
-00000c10: 5b46 6965 6c64 4d6f 6475 6c65 5d0d 0a20  [FieldModule].. 
-00000c20: 2020 2020 2020 2054 7570 6c65 206f 6620         Tuple of 
-00000c30: 6046 6965 6c64 4d6f 6475 6c65 6073 2066  `FieldModule`s f
-00000c40: 6f72 2064 6174 6173 6574 2066 6965 6c64  or dataset field
-00000c50: 732e 0d0a 2020 2020 6d6f 6465 6c20 3a20  s...    model : 
-00000c60: 556e 696f 6e5b 5265 6353 7973 4172 6368  Union[RecSysArch
-00000c70: 2c20 746f 7263 682e 6e6e 2e4d 6f64 756c  , torch.nn.Modul
-00000c80: 652c 204e 6f6e 655d 0d0a 2020 2020 2020  e, None]..      
-00000c90: 2020 4d6f 6465 6c20 666f 7220 7472 6169    Model for trai
-00000ca0: 6e69 6e67 2061 6e64 2065 7661 6c75 6174  ning and evaluat
-00000cb0: 696e 672e 200d 0a20 2020 2020 2020 2049  ing. ..        I
-00000cc0: 6620 604e 6f6e 6560 2c20 7573 6520 5f44  f `None`, use _D
-00000cd0: 756d 6d79 4d6f 6475 6c65 2069 6e73 7465  ummyModule inste
-00000ce0: 6164 2c20 7768 6963 6820 7368 6f75 6c64  ad, which should
-00000cf0: 206e 6f74 2063 616c 6c20 6066 6f72 7761   not call `forwa
-00000d00: 7264 602e 0d0a 2020 2020 6372 6974 6572  rd`...    criter
-00000d10: 696f 6e20 3a20 556e 696f 6e5b 4261 7365  ion : Union[Base
-00000d20: 4372 6974 6572 696f 6e2c 2043 616c 6c61  Criterion, Calla
-00000d30: 626c 655d 0d0a 2020 2020 2020 2020 4361  ble]..        Ca
-00000d40: 6c6c 6162 6c65 2066 6f72 2063 6f6d 7075  llable for compu
-00000d50: 7469 6e67 2074 6865 206c 6f73 7320 6675  ting the loss fu
-00000d60: 6e63 7469 6f6e 2e0d 0a20 2020 206f 7074  nction...    opt
-00000d70: 696d 697a 6572 203a 2074 6f72 6368 2e6f  imizer : torch.o
-00000d80: 7074 696d 2e4f 7074 696d 697a 6572 2c20  ptim.Optimizer, 
-00000d90: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00000da0: 2020 4f70 7469 6d69 7a65 7220 666f 7220    Optimizer for 
-00000db0: 7570 6461 7469 6e67 206d 6f64 656c 2070  updating model p
-00000dc0: 6172 616d 6574 6572 732e 200d 0a20 2020  arameters. ..   
-00000dd0: 2020 2020 2049 6620 604e 6f6e 6560 2c20       If `None`, 
-00000de0: 7573 6520 5f44 756d 6d79 4d6f 6475 6c65  use _DummyModule
-00000df0: 2069 6e73 7465 6164 2c20 7768 6963 6820   instead, which 
-00000e00: 7368 6f75 6c64 206e 6f74 2063 616c 6c20  should not call 
-00000e10: 6073 7465 7060 2061 6e64 2060 6261 636b  `step` and `back
-00000e20: 7761 7264 602e 0d0a 2020 2020 6c72 5f73  ward`...    lr_s
-00000e30: 6368 6564 756c 6572 203a 2074 6f72 6368  cheduler : torch
-00000e40: 2e6f 7074 696d 2e6c 725f 7363 6865 6475  .optim.lr_schedu
-00000e50: 6c65 722e 5f4c 5253 6368 6564 756c 6572  ler._LRScheduler
-00000e60: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00000e70: 2020 2020 4c65 6172 6e69 6e67 2072 6174      Learning rat
-00000e80: 6520 7363 6865 6475 6c65 722e 2049 6620  e scheduler. If 
-00000e90: 604e 6f6e 6560 2c20 7573 6520 5f44 756d  `None`, use _Dum
-00000ea0: 6d79 4d6f 6475 6c65 2069 6e73 7465 6164  myModule instead
-00000eb0: 2c20 0d0a 2020 2020 2020 2020 7768 6963  , ..        whic
-00000ec0: 6820 7368 6f75 6c64 206e 6f74 2063 616c  h should not cal
-00000ed0: 6c20 6073 7465 7060 2e0d 0a20 2020 2064  l `step`...    d
-00000ee0: 6576 6963 6520 3a20 556e 696f 6e5b 746f  evice : Union[to
-00000ef0: 7263 682e 6465 7669 6365 2c20 7374 722c  rch.device, str,
-00000f00: 2069 6e74 5d0d 0a20 2020 2020 2020 2044   int]..        D
-00000f10: 6576 6963 6520 6f6e 2077 6869 6368 2074  evice on which t
-00000f20: 6f20 7275 6e20 7468 6520 636f 6d70 7574  o run the comput
-00000f30: 6174 696f 6e2e 200d 0a20 2020 2020 2020  ation. ..       
-00000f40: 2020 2020 202d 2060 746f 7263 682e 6465       - `torch.de
-00000f50: 7669 6365 600d 0a20 2020 2020 2020 2020  vice`..         
-00000f60: 2020 202d 2060 7374 7260 3a20 4c69 6b65     - `str`: Like
-00000f70: 2060 6370 7560 2c20 6063 7564 613a 3060   `cpu`, `cuda:0`
-00000f80: 2e0d 0a20 2020 2020 2020 2020 2020 202d  ...            -
-00000f90: 2060 696e 7460 3a20 5573 696e 6720 6375   `int`: Using cu
-00000fa0: 6461 3a60 696e 7460 2e0d 0a20 2020 2022  da:`int`...    "
-00000fb0: 2222 0d0a 0d0a 0d0a 2020 2020 6465 6620  ""......    def 
-00000fc0: 5f5f 696e 6974 5f5f 280d 0a20 2020 2020  __init__(..     
-00000fd0: 2020 2073 656c 662c 202a 2c0d 0a20 2020     self, *,..   
-00000fe0: 2020 2020 2074 7261 696e 7069 7065 3a20       trainpipe: 
-00000ff0: 4974 6572 4461 7461 5069 7065 2c20 7661  IterDataPipe, va
-00001000: 6c69 6470 6970 653a 204f 7074 696f 6e61  lidpipe: Optiona
-00001010: 6c5b 4974 6572 4461 7461 5069 7065 5d2c  l[IterDataPipe],
-00001020: 2074 6573 7470 6970 653a 204f 7074 696f   testpipe: Optio
-00001030: 6e61 6c5b 4974 6572 4461 7461 5069 7065  nal[IterDataPipe
-00001040: 5d2c 2066 6965 6c64 733a 2049 7465 7261  ], fields: Itera
-00001050: 626c 655b 4669 656c 644d 6f64 756c 655d  ble[FieldModule]
-00001060: 2c0d 0a20 2020 2020 2020 206d 6f64 656c  ,..        model
-00001070: 3a20 556e 696f 6e5b 5265 6353 7973 4172  : Union[RecSysAr
-00001080: 6368 2c20 746f 7263 682e 6e6e 2e4d 6f64  ch, torch.nn.Mod
-00001090: 756c 652c 204e 6f6e 655d 2c20 6372 6974  ule, None], crit
-000010a0: 6572 696f 6e3a 2055 6e69 6f6e 5b42 6173  erion: Union[Bas
-000010b0: 6543 7269 7465 7269 6f6e 2c20 4361 6c6c  eCriterion, Call
-000010c0: 6162 6c65 5d2c 200d 0a20 2020 2020 2020  able], ..       
-000010d0: 206f 7074 696d 697a 6572 3a20 4f70 7469   optimizer: Opti
-000010e0: 6f6e 616c 5b74 6f72 6368 2e6f 7074 696d  onal[torch.optim
-000010f0: 2e4f 7074 696d 697a 6572 5d2c 206c 725f  .Optimizer], lr_
-00001100: 7363 6865 6475 6c65 723a 204f 7074 696f  scheduler: Optio
-00001110: 6e61 6c5b 746f 7263 682e 6f70 7469 6d2e  nal[torch.optim.
-00001120: 6c72 5f73 6368 6564 756c 6572 2e5f 4c52  lr_scheduler._LR
-00001130: 5363 6865 6475 6c65 725d 2c0d 0a20 2020  Scheduler],..   
-00001140: 2020 2020 2064 6576 6963 653a 2055 6e69       device: Uni
-00001150: 6f6e 5b74 6f72 6368 2e64 6576 6963 652c  on[torch.device,
-00001160: 2073 7472 2c20 696e 745d 0d0a 2020 2020   str, int]..    
-00001170: 293a 0d0a 0d0a 2020 2020 2020 2020 7365  ):....        se
-00001180: 6c66 2e66 6965 6c64 733a 2046 6965 6c64  lf.fields: Field
-00001190: 5475 706c 655b 4669 656c 644d 6f64 756c  Tuple[FieldModul
-000011a0: 655d 203d 2046 6965 6c64 5475 706c 6528  e] = FieldTuple(
-000011b0: 6669 656c 6473 290d 0a20 2020 2020 2020  fields)..       
-000011c0: 2073 656c 662e 6465 7669 6365 203d 2074   self.device = t
-000011d0: 6f72 6368 2e64 6576 6963 6528 6465 7669  orch.device(devi
-000011e0: 6365 290d 0a20 2020 2020 2020 2074 7279  ce)..        try
-000011f0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00001200: 6f72 6368 2e63 7564 612e 7365 745f 6465  orch.cuda.set_de
-00001210: 7669 6365 2873 656c 662e 6465 7669 6365  vice(self.device
-00001220: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-00001230: 7420 5661 6c75 6545 7272 6f72 3a0d 0a20  t ValueError:.. 
-00001240: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00001250: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00001260: 4174 7472 6962 7574 6545 7272 6f72 3a0d  AttributeError:.
-00001270: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-00001280: 730d 0a0d 0a20 2020 2020 2020 2073 656c  s....        sel
-00001290: 662e 5f73 6574 5f64 6174 6170 6970 6528  f._set_datapipe(
-000012a0: 7472 6169 6e70 6970 652c 2076 616c 6964  trainpipe, valid
-000012b0: 7069 7065 2c20 7465 7374 7069 7065 290d  pipe, testpipe).
-000012c0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-000012d0: 6574 5f6f 7468 6572 286d 6f64 656c 2c20  et_other(model, 
-000012e0: 6372 6974 6572 696f 6e2c 206f 7074 696d  criterion, optim
-000012f0: 697a 6572 2c20 6c72 5f73 6368 6564 756c  izer, lr_schedul
-00001300: 6572 290d 0a0d 0a20 2020 2020 2020 2073  er)....        s
-00001310: 656c 662e 5f5f 6d6f 6465 203d 2027 7472  elf.__mode = 'tr
-00001320: 6169 6e27 0d0a 0d0a 2020 2020 2020 2020  ain'....        
-00001330: 6465 6620 636c 6561 6e28 293a 0d0a 2020  def clean():..  
-00001340: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
-00001350: 203d 2070 7375 7469 6c2e 5072 6f63 6573   = psutil.Proces
-00001360: 7328 6f73 2e67 6574 7069 6428 2929 0d0a  s(os.getpid())..
-00001370: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00001380: 6472 656e 203d 2070 6172 656e 742e 6368  dren = parent.ch
-00001390: 696c 6472 656e 2872 6563 7572 7369 7665  ildren(recursive
-000013a0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-000013b0: 2020 2020 666f 7220 7072 6f63 6573 7320      for process 
-000013c0: 696e 2063 6869 6c64 7265 6e3a 0d0a 2020  in children:..  
-000013d0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000013e0: 6f63 6573 732e 7365 6e64 5f73 6967 6e61  ocess.send_signa
-000013f0: 6c28 7369 676e 616c 2e53 4947 5445 524d  l(signal.SIGTERM
-00001400: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00001410: 7375 7469 6c2e 7761 6974 5f70 726f 6373  sutil.wait_procs
-00001420: 2863 6869 6c64 7265 6e2c 2074 696d 656f  (children, timeo
-00001430: 7574 3d35 290d 0a0d 0a20 2020 2020 2020  ut=5)....       
-00001440: 2061 7465 7869 742e 7265 6769 7374 6572   atexit.register
-00001450: 2863 6c65 616e 290d 0a0d 0a20 2020 2064  (clean)....    d
-00001460: 6566 205f 7365 745f 6461 7461 7069 7065  ef _set_datapipe
-00001470: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-00001480: 0d0a 2020 2020 2020 2020 7472 6169 6e70  ..        trainp
-00001490: 6970 652c 0d0a 2020 2020 2020 2020 7661  ipe,..        va
-000014a0: 6c69 6470 6970 653d 4e6f 6e65 2c0d 0a20  lidpipe=None,.. 
-000014b0: 2020 2020 2020 2074 6573 7470 6970 653d         testpipe=
-000014c0: 4e6f 6e65 2c0d 0a20 2020 2029 3a0d 0a20  None,..    ):.. 
-000014d0: 2020 2020 2020 2022 2222 5365 7420 7468         """Set th
-000014e0: 6520 6461 7461 2070 6970 6520 666f 7220  e data pipe for 
-000014f0: 7472 6169 6e69 6e67 2c20 7661 6c69 6461  training, valida
-00001500: 7469 6f6e 2061 6e64 2074 6573 742e 2222  tion and test.""
-00001510: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00001520: 7472 6169 6e70 6970 6520 3d20 7472 6169  trainpipe = trai
-00001530: 6e70 6970 650d 0a20 2020 2020 2020 2073  npipe..        s
-00001540: 656c 662e 7661 6c69 6470 6970 6520 3d20  elf.validpipe = 
-00001550: 7365 6c66 2e74 7261 696e 7069 7065 2069  self.trainpipe i
-00001560: 6620 7661 6c69 6470 6970 6520 6973 204e  f validpipe is N
-00001570: 6f6e 6520 656c 7365 2076 616c 6964 7069  one else validpi
-00001580: 7065 0d0a 2020 2020 2020 2020 7365 6c66  pe..        self
-00001590: 2e74 6573 7470 6970 6520 3d20 7365 6c66  .testpipe = self
-000015a0: 2e76 616c 6964 7069 7065 2069 6620 7465  .validpipe if te
-000015b0: 7374 7069 7065 2069 7320 4e6f 6e65 2065  stpipe is None e
-000015c0: 6c73 6520 7465 7374 7069 7065 0d0a 0d0a  lse testpipe....
-000015d0: 2020 2020 6465 6620 5f73 6574 5f6f 7468      def _set_oth
-000015e0: 6572 280d 0a20 2020 2020 2020 2073 656c  er(..        sel
-000015f0: 662c 0d0a 2020 2020 2020 2020 6d6f 6465  f,..        mode
-00001600: 6c3d 4e6f 6e65 2c20 6372 6974 6572 696f  l=None, criterio
-00001610: 6e3d 4e6f 6e65 2c20 6f70 7469 6d69 7a65  n=None, optimize
-00001620: 723d 4e6f 6e65 2c20 6c72 5f73 6368 6564  r=None, lr_sched
-00001630: 756c 6572 3d4e 6f6e 652c 0d0a 2020 2020  uler=None,..    
-00001640: 293a 0d0a 2020 2020 2020 2020 2222 2253  ):..        """S
-00001650: 6574 2074 6865 206f 7468 6572 206e 6563  et the other nec
-00001660: 6573 7361 7279 2063 6f6d 706f 6e65 6e74  essary component
-00001670: 732e 2222 220d 0a20 2020 2020 2020 2073  s."""..        s
-00001680: 656c 662e 6372 6974 6572 696f 6e20 3d20  elf.criterion = 
-00001690: 6372 6974 6572 696f 6e0d 0a20 2020 2020  criterion..     
-000016a0: 2020 2073 656c 662e 6d6f 6465 6c20 3d20     self.model = 
-000016b0: 6d6f 6465 6c2e 746f 2873 656c 662e 6465  model.to(self.de
-000016c0: 7669 6365 2920 6966 206d 6f64 656c 2065  vice) if model e
-000016d0: 6c73 6520 5f44 756d 6d79 4d6f 6475 6c65  lse _DummyModule
-000016e0: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-000016f0: 2e6f 7074 696d 697a 6572 203d 206f 7074  .optimizer = opt
-00001700: 696d 697a 6572 2069 6620 6f70 7469 6d69  imizer if optimi
-00001710: 7a65 7220 656c 7365 205f 4475 6d6d 794d  zer else _DummyM
-00001720: 6f64 756c 6528 290d 0a20 2020 2020 2020  odule()..       
-00001730: 2073 656c 662e 6c72 5f73 6368 6564 756c   self.lr_schedul
-00001740: 6572 203d 206c 725f 7363 6865 6475 6c65  er = lr_schedule
-00001750: 7220 6966 206c 725f 7363 6865 6475 6c65  r if lr_schedule
-00001760: 7220 656c 7365 205f 4475 6d6d 794d 6f64  r else _DummyMod
-00001770: 756c 6528 290d 0a0d 0a20 2020 2040 7072  ule()....    @pr
-00001780: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-00001790: 6d6f 6465 2873 656c 6629 3a0d 0a20 2020  mode(self):..   
-000017a0: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
-000017b0: 6375 7272 656e 7420 6d6f 6465 206f 6620  current mode of 
-000017c0: 7468 6520 6368 6965 6620 636f 6163 682e  the chief coach.
-000017d0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-000017e0: 7572 6e20 7365 6c66 2e5f 5f6d 6f64 650d  urn self.__mode.
-000017f0: 0a0d 0a20 2020 2040 7469 6d65 6d65 7465  ...    @timemete
-00001800: 7228 2243 6f61 6368 2f74 7261 696e 2229  r("Coach/train")
-00001810: 0d0a 2020 2020 6465 6620 7472 6169 6e28  ..    def train(
-00001820: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
-00001830: 293a 0d0a 2020 2020 2020 2020 2222 2253  ):..        """S
-00001840: 7461 7274 2074 7261 696e 696e 6720 616e  tart training an
-00001850: 6420 7265 7475 726e 2074 6865 2074 7261  d return the tra
-00001860: 696e 696e 6720 6c6f 7373 2e22 2222 0d0a  ining loss."""..
-00001870: 2020 2020 2020 2020 7365 6c66 2e5f 5f6d          self.__m
-00001880: 6f64 6520 3d20 2774 7261 696e 270d 0a20  ode = 'train'.. 
-00001890: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-000018a0: 6c2e 7472 6169 6e28 290d 0a20 2020 2020  l.train()..     
-000018b0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
-000018c0: 7261 696e 5f70 6572 5f65 706f 6368 2865  rain_per_epoch(e
-000018d0: 706f 6368 290d 0a0d 0a20 2020 2040 7469  poch)....    @ti
-000018e0: 6d65 6d65 7465 7228 2243 6f61 6368 2f76  memeter("Coach/v
-000018f0: 616c 6964 2229 0d0a 2020 2020 4074 6f72  alid")..    @tor
-00001900: 6368 2e6e 6f5f 6772 6164 2829 0d0a 2020  ch.no_grad()..  
-00001910: 2020 6465 6620 7661 6c69 6428 7365 6c66    def valid(self
-00001920: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
-00001930: 2020 2020 2020 2020 2222 2253 7461 7274          """Start
-00001940: 2076 616c 6964 6174 696f 6e20 616e 6420   validation and 
-00001950: 7265 7475 726e 2074 6865 2076 616c 6964  return the valid
-00001960: 6174 696f 6e20 6d65 7472 6963 732e 2222  ation metrics.""
-00001970: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00001980: 5f5f 6d6f 6465 203d 2027 7661 6c69 6427  __mode = 'valid'
-00001990: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000019a0: 6f64 656c 2e65 7661 6c28 290d 0a20 2020  odel.eval()..   
-000019b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000019c0: 2e65 7661 6c75 6174 6528 6570 6f63 683d  .evaluate(epoch=
-000019d0: 6570 6f63 682c 2070 7265 6669 783d 2776  epoch, prefix='v
-000019e0: 616c 6964 2729 0d0a 0d0a 2020 2020 4074  alid')....    @t
-000019f0: 696d 656d 6574 6572 2822 436f 6163 682f  imemeter("Coach/
-00001a00: 7465 7374 2229 0d0a 2020 2020 4074 6f72  test")..    @tor
-00001a10: 6368 2e6e 6f5f 6772 6164 2829 0d0a 2020  ch.no_grad()..  
-00001a20: 2020 6465 6620 7465 7374 2873 656c 662c    def test(self,
-00001a30: 2065 706f 6368 3a20 696e 7429 3a0d 0a20   epoch: int):.. 
-00001a40: 2020 2020 2020 2022 2222 5374 6172 7420         """Start 
-00001a50: 7465 7374 696e 6720 616e 6420 7265 7475  testing and retu
-00001a60: 726e 2074 6865 2074 6573 7420 6d65 7472  rn the test metr
-00001a70: 6963 732e 2222 220d 0a20 2020 2020 2020  ics."""..       
-00001a80: 2073 656c 662e 5f5f 6d6f 6465 203d 2027   self.__mode = '
-00001a90: 7465 7374 270d 0a20 2020 2020 2020 2073  test'..        s
-00001aa0: 656c 662e 6d6f 6465 6c2e 6576 616c 2829  elf.model.eval()
-00001ab0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001ac0: 2073 656c 662e 6576 616c 7561 7465 2865   self.evaluate(e
-00001ad0: 706f 6368 3d65 706f 6368 2c20 7072 6566  poch=epoch, pref
-00001ae0: 6978 3d27 7465 7374 2729 0d0a 0d0a 2020  ix='test')....  
-00001af0: 2020 4061 6263 2e61 6273 7472 6163 746d    @abc.abstractm
-00001b00: 6574 686f 640d 0a20 2020 2064 6566 2074  ethod..    def t
-00001b10: 7261 696e 5f70 6572 5f65 706f 6368 2873  rain_per_epoch(s
-00001b20: 656c 662c 2065 706f 6368 3a20 696e 7429  elf, epoch: int)
-00001b30: 3a0d 0a20 2020 2020 2020 2072 6169 7365  :..        raise
-00001b40: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00001b50: 7272 6f72 280d 0a20 2020 2020 2020 2020  rror(..         
-00001b60: 2020 2066 227b 7365 6c66 2e5f 5f63 6c61     f"{self.__cla
-00001b70: 7373 5f5f 2e5f 5f6e 616d 655f 5f7d 2e74  ss__.__name__}.t
-00001b80: 7261 696e 5f70 6572 5f65 706f 6368 2829  rain_per_epoch()
-00001b90: 2073 686f 756c 6420 6265 2069 6d70 6c65   should be imple
-00001ba0: 6d65 6e74 6564 202e 2e2e 220d 0a20 2020  mented ..."..   
-00001bb0: 2020 2020 2029 0d0a 0d0a 2020 2020 4061       )....    @a
-00001bc0: 6263 2e61 6273 7472 6163 746d 6574 686f  bc.abstractmetho
-00001bd0: 640d 0a20 2020 2064 6566 2065 7661 6c75  d..    def evalu
-00001be0: 6174 6528 7365 6c66 2c20 6570 6f63 683a  ate(self, epoch:
-00001bf0: 2069 6e74 2c20 7072 6566 6978 3a20 7374   int, prefix: st
-00001c00: 7220 3d20 2776 616c 6964 2729 3a0d 0a20  r = 'valid'):.. 
-00001c10: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00001c20: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00001c30: 280d 0a20 2020 2020 2020 2020 2020 2066  (..            f
-00001c40: 227b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  "{self.__class__
-00001c50: 2e5f 5f6e 616d 655f 5f7d 2e65 7661 6c75  .__name__}.evalu
-00001c60: 6174 6528 2920 7368 6f75 6c64 2062 6520  ate() should be 
-00001c70: 696d 706c 656d 656e 7465 6420 2e2e 2e22  implemented ..."
-00001c80: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-00001c90: 2020 2064 6566 2072 6567 6973 7465 725f     def register_
-00001ca0: 6d65 7472 6963 280d 0a20 2020 2020 2020  metric(..       
-00001cb0: 2073 656c 662c 206e 616d 653a 2073 7472   self, name: str
-00001cc0: 2c20 6675 6e63 3a20 4361 6c6c 6162 6c65  , func: Callable
-00001cd0: 2c20 0d0a 2020 2020 2020 2020 666d 743a  , ..        fmt:
-00001ce0: 2073 7472 203d 2027 2e34 6627 2c20 6265   str = '.4f', be
-00001cf0: 7374 5f63 6173 7465 723a 2043 616c 6c61  st_caster: Calla
-00001d00: 626c 6520 3d20 6d61 780d 0a20 2020 2029  ble = max..    )
-00001d10: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-00001d20: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
-00001d30: 2052 6567 6973 7465 7220 6120 6d65 7472   Register a metr
-00001d40: 6963 2e0d 0a0d 0a20 2020 2020 2020 2050  ic.....        P
-00001d50: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00001d60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00001d70: 2020 2020 2020 206e 616d 6520 3a20 7374         name : st
-00001d80: 720d 0a20 2020 2020 2020 2020 2020 2054  r..            T
-00001d90: 6865 2063 6f6d 706c 6574 6520 6e61 6d65  he complete name
-00001da0: 206f 6620 7468 6520 6d65 7472 6963 2c20   of the metric, 
-00001db0: 7375 6368 2061 7320 604c 4f53 5332 602e  such as `LOSS2`.
-00001dc0: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00001dd0: 6520 6e6f 7461 7469 6f6e 2060 4060 2073  e notation `@` s
-00001de0: 686f 756c 6420 6e6f 7420 6265 2069 6e63  hould not be inc
-00001df0: 6c75 6465 642c 2069 2e65 2e2c 2027 4c4f  luded, i.e., 'LO
-00001e00: 5353 4032 2720 6973 2069 6e76 616c 6964  SS@2' is invalid
-00001e10: 2e0d 0a20 2020 2020 2020 2066 756e 6320  ...        func 
-00001e20: 3a20 4361 6c6c 6162 6c65 0d0a 2020 2020  : Callable..    
-00001e30: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
-00001e40: 7469 6f6e 2074 6f20 7072 6f63 6573 7320  tion to process 
-00001e50: 7468 6520 6461 7461 2066 6f72 2074 6865  the data for the
-00001e60: 206d 6574 7269 632e 0d0a 2020 2020 2020   metric...      
-00001e70: 2020 666d 7420 3a20 7374 722c 206f 7074    fmt : str, opt
-00001e80: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-00001e90: 2020 2054 6865 2066 6f72 6d61 7420 746f     The format to
-00001ea0: 2075 7365 2077 6865 6e20 7072 696e 7469   use when printi
-00001eb0: 6e67 2074 6865 206d 6574 7269 632c 2064  ng the metric, d
-00001ec0: 6566 6175 6c74 7320 746f 2060 272e 3466  efaults to `'.4f
-00001ed0: 2760 2e0d 0a20 2020 2020 2020 2062 6573  '`...        bes
-00001ee0: 745f 6361 7374 6572 203a 2043 616c 6c61  t_caster : Calla
-00001ef0: 626c 652c 206f 7074 696f 6e61 6c0d 0a20  ble, optional.. 
-00001f00: 2020 2020 2020 2020 2020 2041 2066 756e             A fun
-00001f10: 6374 696f 6e20 7573 6564 2074 6f20 6361  ction used to ca
-00001f20: 7374 2074 6865 2062 6573 7420 7661 6c75  st the best valu
-00001f30: 6520 6f66 2074 6865 206d 6574 7269 632c  e of the metric,
-00001f40: 2064 6566 6175 6c74 7320 746f 2060 6d61   defaults to `ma
-00001f50: 7860 2e0d 0a20 2020 2020 2020 2020 2020  x`...           
-00001f60: 200d 0a20 2020 2020 2020 2052 6574 7572   ..        Retur
-00001f70: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00001f80: 2d2d 2d0d 0a20 2020 2020 2020 204e 6f6e  ---..        Non
-00001f90: 650d 0a20 2020 2020 2020 200d 0a20 2020  e..        ..   
-00001fa0: 2020 2020 2052 6169 7365 730d 0a20 2020       Raises..   
-00001fb0: 2020 2020 202d 2d2d 2d2d 2d0d 0a20 2020       ------..   
-00001fc0: 2020 2020 2041 7373 6572 7469 6f6e 4572       AssertionEr
-00001fd0: 726f 720d 0a20 2020 2020 2020 2020 2020  ror..           
-00001fe0: 2057 6865 6e20 606e 616d 6560 2068 6173   When `name` has
-00001ff0: 2061 6c72 6561 6479 2062 6565 6e20 7265   already been re
-00002000: 6769 7374 6572 6564 206f 7220 636f 6e74  gistered or cont
-00002010: 6169 6e73 2074 6865 206e 6f74 6174 696f  ains the notatio
-00002020: 6e20 6040 602e 0d0a 2020 2020 2020 2020  n `@`...        
-00002030: 2222 220d 0a0d 0a20 2020 2020 2020 206e  """....        n
-00002040: 616d 6520 3d20 6e61 6d65 2e75 7070 6572  ame = name.upper
-00002050: 2829 0d0a 2020 2020 2020 2020 6173 7365  ()..        asse
-00002060: 7274 2044 4546 4155 4c54 5f4d 4554 5249  rt DEFAULT_METRI
-00002070: 4353 2e67 6574 286e 616d 652c 204e 6f6e  CS.get(name, Non
-00002080: 6529 2069 7320 4e6f 6e65 2c20 6622 5468  e) is None, f"Th
-00002090: 6520 6d65 7472 6963 207b 6e61 6d65 7d20  e metric {name} 
-000020a0: 616c 7265 6164 7920 6578 6973 7473 202e  already exists .
-000020b0: 2e2e 220d 0a20 2020 2020 2020 2061 7373  .."..        ass
-000020c0: 6572 7420 2740 2720 6e6f 7420 696e 206e  ert '@' not in n
-000020d0: 616d 652c 2066 2254 6865 206d 6574 7269  ame, f"The metri
-000020e0: 6320 6e61 6d65 2068 6173 2069 6e76 616c  c name has inval
-000020f0: 6964 206e 6f74 6174 696f 6e20 6f66 2060  id notation of `
-00002100: 4027 202e 2e2e 220d 0a20 2020 2020 2020  @' ..."..       
-00002110: 2044 4546 4155 4c54 5f4d 4554 5249 4353   DEFAULT_METRICS
-00002120: 5b6e 616d 655d 203d 2066 756e 630d 0a20  [name] = func.. 
-00002130: 2020 2020 2020 2044 4546 4155 4c54 5f46         DEFAULT_F
-00002140: 4d54 535b 6e61 6d65 5d20 3d20 666d 740d  MTS[name] = fmt.
-00002150: 0a20 2020 2020 2020 2044 4546 4155 4c54  .        DEFAULT
-00002160: 5f42 4553 545f 4341 5354 4552 5b6e 616d  _BEST_CASTER[nam
-00002170: 655d 203d 2062 6573 745f 6361 7374 6572  e] = best_caster
-00002180: 0d0a 0d0a 0d0a 636c 6173 7320 436f 6163  ......class Coac
-00002190: 6828 4368 6965 6643 6f61 6368 293a 0d0a  h(ChiefCoach):..
-000021a0: 2020 2020 2222 2254 6865 2066 7261 6d65      """The frame
-000021b0: 776f 726b 2066 6f72 2074 7261 696e 696e  work for trainin
-000021c0: 672e 2222 220d 0a0d 0a20 2020 2064 6566  g."""....    def
-000021d0: 2070 7265 7061 7265 5f64 6174 616c 6f61   prepare_dataloa
-000021e0: 6465 7228 7365 6c66 2920 2d3e 204e 6f6e  der(self) -> Non
-000021f0: 653a 0d0a 2020 2020 2020 2020 2222 2250  e:..        """P
-00002200: 7265 7061 7265 2064 6174 6120 6c6f 6164  repare data load
-00002210: 6572 7320 666f 7220 7472 6169 6e69 6e67  ers for training
-00002220: 2c20 7661 6c69 6461 7469 6f6e 2c20 616e  , validation, an
-00002230: 6420 7465 7374 696e 6720 6461 7461 2e22  d testing data."
-00002240: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00002250: 2e74 7261 696e 6c6f 6164 6572 203d 2044  .trainloader = D
-00002260: 6174 614c 6f61 6465 7228 0d0a 2020 2020  ataLoader(..    
-00002270: 2020 2020 2020 2020 6461 7461 7069 7065          datapipe
-00002280: 3d73 656c 662e 7472 6169 6e70 6970 652c  =self.trainpipe,
-00002290: 200d 0a20 2020 2020 2020 2020 2020 206e   ..            n
-000022a0: 756d 5f77 6f72 6b65 7273 3d73 656c 662e  um_workers=self.
-000022b0: 6366 672e 6e75 6d5f 776f 726b 6572 732c  cfg.num_workers,
-000022c0: 0d0a 2020 2020 2020 2020 2020 2020 7069  ..            pi
-000022d0: 6e5f 6d65 6d6f 7279 3d73 656c 662e 6366  n_memory=self.cf
-000022e0: 672e 7069 6e5f 6d65 6d6f 7279 0d0a 2020  g.pin_memory..  
-000022f0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00002300: 2073 656c 662e 7661 6c69 646c 6f61 6465   self.validloade
-00002310: 7220 3d20 4461 7461 4c6f 6164 6572 280d  r = DataLoader(.
-00002320: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00002330: 6170 6970 653d 7365 6c66 2e76 616c 6964  apipe=self.valid
-00002340: 7069 7065 2c20 0d0a 2020 2020 2020 2020  pipe, ..        
-00002350: 2020 2020 6e75 6d5f 776f 726b 6572 733d      num_workers=
-00002360: 7365 6c66 2e63 6667 2e6e 756d 5f77 6f72  self.cfg.num_wor
-00002370: 6b65 7273 2c0d 0a20 2020 2020 2020 2020  kers,..         
-00002380: 2020 2070 696e 5f6d 656d 6f72 793d 7365     pin_memory=se
-00002390: 6c66 2e63 6667 2e70 696e 5f6d 656d 6f72  lf.cfg.pin_memor
-000023a0: 790d 0a20 2020 2020 2020 2029 0d0a 2020  y..        )..  
-000023b0: 2020 2020 2020 7365 6c66 2e74 6573 746c        self.testl
-000023c0: 6f61 6465 7220 3d20 4461 7461 4c6f 6164  oader = DataLoad
-000023d0: 6572 280d 0a20 2020 2020 2020 2020 2020  er(..           
-000023e0: 2064 6174 6170 6970 653d 7365 6c66 2e74   datapipe=self.t
-000023f0: 6573 7470 6970 652c 200d 0a20 2020 2020  estpipe, ..     
-00002400: 2020 2020 2020 206e 756d 5f77 6f72 6b65         num_worke
-00002410: 7273 3d73 656c 662e 6366 672e 6e75 6d5f  rs=self.cfg.num_
-00002420: 776f 726b 6572 732c 0d0a 2020 2020 2020  workers,..      
-00002430: 2020 2020 2020 7069 6e5f 6d65 6d6f 7279        pin_memory
-00002440: 3d73 656c 662e 6366 672e 7069 6e5f 6d65  =self.cfg.pin_me
-00002450: 6d6f 7279 0d0a 2020 2020 2020 2020 290d  mory..        ).
-00002460: 0a20 2020 200d 0a20 2020 2040 7072 6f70  .    ..    @prop
-00002470: 6572 7479 0d0a 2020 2020 6465 6620 6461  erty..    def da
-00002480: 7461 6c6f 6164 6572 2873 656c 6629 3a0d  taloader(self):.
-00002490: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000024a0: 726e 2074 6865 2063 6f72 7265 7370 6f6e  rn the correspon
-000024b0: 6469 6e67 2064 6174 6120 6c6f 6164 6572  ding data loader
-000024c0: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
-000024d0: 6520 6375 7272 656e 7420 6d6f 6465 2e22  e current mode."
-000024e0: 2222 0d0a 2020 2020 2020 2020 6966 2073  ""..        if s
-000024f0: 656c 662e 6d6f 6465 203d 3d20 2774 7261  elf.mode == 'tra
-00002500: 696e 273a 0d0a 2020 2020 2020 2020 2020  in':..          
-00002510: 2020 7265 7475 726e 2073 656c 662e 7472    return self.tr
-00002520: 6169 6e6c 6f61 6465 720d 0a20 2020 2020  ainloader..     
-00002530: 2020 2065 6c69 6620 7365 6c66 2e6d 6f64     elif self.mod
-00002540: 6520 3d3d 2027 7661 6c69 6427 3a0d 0a20  e == 'valid':.. 
-00002550: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002560: 6e20 7365 6c66 2e76 616c 6964 6c6f 6164  n self.validload
-00002570: 6572 0d0a 2020 2020 2020 2020 656c 7365  er..        else
-00002580: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00002590: 6574 7572 6e20 7365 6c66 2e74 6573 746c  eturn self.testl
-000025a0: 6f61 6465 720d 0a0d 0a20 2020 2040 7072  oader....    @pr
-000025b0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-000025c0: 6d6f 6e69 746f 7273 2873 656c 6629 202d  monitors(self) -
-000025d0: 3e20 4d6f 6e69 746f 723a 0d0a 2020 2020  > Monitor:..    
-000025e0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-000025f0: 6520 6d6f 6e69 746f 7220 6469 6374 696f  e monitor dictio
-00002600: 6e61 7279 2066 6f72 2074 6865 2064 6966  nary for the dif
-00002610: 6665 7265 6e74 206d 6f64 6573 2028 2774  ferent modes ('t
-00002620: 7261 696e 272c 2027 7661 6c69 6427 2c20  rain', 'valid', 
-00002630: 2774 6573 7427 292e 2222 220d 0a20 2020  'test')."""..   
-00002640: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002650: 2e5f 5f6d 6f6e 6974 6f72 730d 0a0d 0a20  .__monitors.... 
-00002660: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00002670: 2020 6465 6620 6d65 7465 7234 6265 7374    def meter4best
-00002680: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002690: 2072 6574 7572 6e20 7365 6c66 2e5f 5f62   return self.__b
-000026a0: 6573 745f 6d65 7465 720d 0a0d 0a20 2020  est_meter....   
-000026b0: 2040 6d65 7465 7234 6265 7374 2e73 6574   @meter4best.set
-000026c0: 7465 720d 0a20 2020 2064 6566 206d 6574  ter..    def met
-000026d0: 6572 3462 6573 7428 7365 6c66 2c20 6d65  er4best(self, me
-000026e0: 7465 723a 2041 7665 7261 6765 4d65 7465  ter: AverageMete
-000026f0: 7229 3a0d 0a20 2020 2020 2020 2073 656c  r):..        sel
-00002700: 662e 5f5f 6265 7374 5f6d 6574 6572 203d  f.__best_meter =
-00002710: 206d 6574 6572 0d0a 2020 2020 2020 2020   meter..        
-00002720: 696e 666f 4c6f 6767 6572 2866 225b 436f  infoLogger(f"[Co
-00002730: 6163 685d 203e 3e3e 2053 6574 2062 6573  ach] >>> Set bes
-00002740: 7420 6d65 7465 723a 207b 6d65 7465 722e  t meter: {meter.
-00002750: 6e61 6d65 7d20 2229 0d0a 0d0a 2020 2020  name} ")....    
-00002760: 4074 696d 656d 6574 6572 2822 436f 6163  @timemeter("Coac
-00002770: 682f 636f 6d70 696c 6522 290d 0a20 2020  h/compile")..   
-00002780: 2064 6566 2063 6f6d 7069 6c65 280d 0a20   def compile(.. 
-00002790: 2020 2020 2020 2073 656c 662c 2063 6667         self, cfg
-000027a0: 3a20 436f 6e66 6967 2c20 6d6f 6e69 746f  : Config, monito
-000027b0: 7273 3a20 4c69 7374 5b73 7472 5d2c 200d  rs: List[str], .
-000027c0: 0a20 2020 2020 2020 2077 6869 6368 3462  .        which4b
-000027d0: 6573 743a 2073 7472 203d 2027 4c4f 5353  est: str = 'LOSS
-000027e0: 270d 0a20 2020 2029 3a0d 0a20 2020 2020  '..    ):..     
-000027f0: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
-00002800: 204c 6f61 6420 7468 6520 636f 6e66 6967   Load the config
-00002810: 7572 6174 696f 6e20 616e 6420 7365 7420  uration and set 
-00002820: 7570 206d 6f6e 6974 6f72 7320 666f 7220  up monitors for 
-00002830: 7472 6169 6e69 6e67 2e0d 0a0d 0a20 2020  training.....   
-00002840: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-00002850: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00002860: 2d2d 2d0d 0a20 2020 2020 2020 2063 6667  ---..        cfg
-00002870: 203a 2043 6f6e 6669 670d 0a20 2020 2020   : Config..     
-00002880: 2020 2020 2020 2041 2063 6f6e 6669 6775         A configu
-00002890: 7261 7469 6f6e 206f 626a 6563 7420 7769  ration object wi
-000028a0: 7468 2074 6865 2074 7261 696e 696e 6720  th the training 
-000028b0: 6465 7461 696c 732e 0d0a 2020 2020 2020  details...      
-000028c0: 2020 6d6f 6e69 746f 7273 203a 204c 6973    monitors : Lis
-000028d0: 745b 7374 725d 0d0a 2020 2020 2020 2020  t[str]..        
-000028e0: 2020 2020 4120 6c69 7374 206f 6620 6d65      A list of me
-000028f0: 7472 6963 206e 616d 6573 2074 6f20 6265  tric names to be
-00002900: 206d 6f6e 6974 6f72 6564 2064 7572 696e   monitored durin
-00002910: 6720 7472 6169 6e69 6e67 2e0d 0a20 2020  g training...   
-00002920: 2020 2020 2077 6869 6368 3462 6573 7420       which4best 
-00002930: 3a20 7374 722c 2064 6566 6175 6c74 7320  : str, defaults 
-00002940: 604c 4f53 5327 0d0a 2020 2020 2020 2020  `LOSS'..        
-00002950: 2020 2020 5468 6520 6d65 7472 6963 2075      The metric u
-00002960: 7365 6420 666f 7220 7365 6c65 6374 696e  sed for selectin
-00002970: 6720 7468 6520 6265 7374 2063 6865 636b  g the best check
-00002980: 706f 696e 742e 0d0a 0d0a 2020 2020 2020  point.....      
-00002990: 2020 4578 616d 706c 6573 0d0a 2020 2020    Examples..    
-000029a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
-000029b0: 2020 2020 2020 3e3e 3e20 636f 6163 683a        >>> coach:
-000029c0: 2043 6f61 6368 0d0a 2020 2020 2020 2020   Coach..        
-000029d0: 3e3e 3e20 636f 6163 682e 636f 6d70 696c  >>> coach.compil
-000029e0: 6528 6366 672c 206d 6f6e 6974 6f72 733d  e(cfg, monitors=
-000029f0: 5b27 6c6f 7373 272c 2027 7265 6361 6c6c  ['loss', 'recall
-00002a00: 4031 3027 2c20 2772 6563 616c 6c40 3230  @10', 'recall@20
-00002a10: 272c 2027 6e64 6367 4031 3027 2c20 276e  ', 'ndcg@10', 'n
-00002a20: 6463 6740 3230 275d 290d 0a20 2020 2020  dcg@20'])..     
-00002a30: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002a40: 7365 6c66 2e63 6667 203d 2063 6667 0d0a  self.cfg = cfg..
-00002a50: 2020 2020 2020 2020 2320 6d65 7465 7273          # meters
-00002a60: 2066 6f72 2074 7261 696e 7c76 616c 6964   for train|valid
-00002a70: 7c74 6573 740d 0a20 2020 2020 2020 2073  |test..        s
-00002a80: 656c 662e 5f5f 6d6f 6e69 746f 7273 203d  elf.__monitors =
-00002a90: 204d 6f6e 6974 6f72 2829 0d0a 2020 2020   Monitor()..    
-00002aa0: 2020 2020 7365 6c66 2e5f 5f6d 6f6e 6974      self.__monit
-00002ab0: 6f72 735b 2774 7261 696e 275d 203d 2064  ors['train'] = d
-00002ac0: 6566 6175 6c74 6469 6374 286c 6973 7429  efaultdict(list)
-00002ad0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00002ae0: 5f6d 6f6e 6974 6f72 735b 2776 616c 6964  _monitors['valid
-00002af0: 275d 203d 2064 6566 6175 6c74 6469 6374  '] = defaultdict
-00002b00: 286c 6973 7429 0d0a 2020 2020 2020 2020  (list)..        
-00002b10: 7365 6c66 2e5f 5f6d 6f6e 6974 6f72 735b  self.__monitors[
-00002b20: 2774 6573 7427 5d20 3d20 6465 6661 756c  'test'] = defaul
-00002b30: 7464 6963 7428 6c69 7374 290d 0a0d 0a20  tdict(list).... 
-00002b40: 2020 2020 2020 2064 6566 2073 6574 5f6d         def set_m
-00002b50: 6f6e 6974 6f72 280d 0a20 2020 2020 2020  onitor(..       
-00002b60: 2020 2020 206e 616d 653a 2073 7472 2c20       name: str, 
-00002b70: 6c61 7374 6e61 6d65 3a20 7374 722c 2070  lastname: str, p
-00002b80: 7265 6669 783a 2073 7472 203d 2027 7472  refix: str = 'tr
-00002b90: 6169 6e27 2c20 2a2a 6b77 6172 6773 0d0a  ain', **kwargs..
-00002ba0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-00002bb0: 2020 2020 2020 2020 2222 2241 6464 2061          """Add a
-00002bc0: 206d 6f6e 6974 6f72 2066 6f72 2074 6865   monitor for the
-00002bd0: 2073 7065 6369 6669 6564 206d 6574 7269   specified metri
-00002be0: 632e 2222 220d 0a20 2020 2020 2020 2020  c."""..         
-00002bf0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00002c00: 2020 2020 2020 2020 206d 6574 6572 203d           meter =
-00002c10: 2041 7665 7261 6765 4d65 7465 7228 0d0a   AverageMeter(..
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
-00002c40: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002c50: 2020 2020 2020 2020 2020 2020 6d65 7472              metr
-00002c60: 6963 3d70 6172 7469 616c 2844 4546 4155  ic=partial(DEFAU
-00002c70: 4c54 5f4d 4554 5249 4353 5b6c 6173 746e  LT_METRICS[lastn
-00002c80: 616d 655d 2c20 2a2a 6b77 6172 6773 292c  ame], **kwargs),
-00002c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002ca0: 2020 2020 2020 2020 2020 666d 743d 4445            fmt=DE
-00002cb0: 4641 554c 545f 464d 5453 5b6c 6173 746e  FAULT_FMTS[lastn
-00002cc0: 616d 655d 2c0d 0a20 2020 2020 2020 2020  ame],..         
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00002ce0: 6573 745f 6361 7374 6572 3d44 4546 4155  est_caster=DEFAU
-00002cf0: 4c54 5f42 4553 545f 4341 5354 4552 5b6c  LT_BEST_CASTER[l
-00002d00: 6173 746e 616d 655d 0d0a 2020 2020 2020  astname]..      
-00002d10: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d30: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
-00002d40: 5b70 7265 6669 785d 5b6c 6173 746e 616d  [prefix][lastnam
-00002d50: 655d 2e61 7070 656e 6428 6d65 7465 7229  e].append(meter)
-00002d60: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00002d70: 6365 7074 204b 6579 4572 726f 723a 0d0a  cept KeyError:..
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 7261 6973 6520 4b65 7945 7272 6f72 280d  raise KeyError(.
-00002da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002db0: 2020 2020 2066 2254 6865 206d 6574 7269       f"The metri
-00002dc0: 6320 6f66 207b 6c61 7374 6e61 6d65 7d20  c of {lastname} 
-00002dd0: 6973 206e 6f74 2069 6e63 6c75 6465 642e  is not included.
-00002de0: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00002df0: 2020 2020 2020 2020 6622 596f 7520 6361          f"You ca
-00002e00: 6e20 7265 6769 7374 6572 2062 7920 6361  n register by ca
-00002e10: 6c6c 696e 6720 6072 6567 6973 7465 725f  lling `register_
-00002e20: 6d65 7472 6963 282e 2e2e 2927 202e 2e2e  metric(...)' ...
-00002e30: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00002e40: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00002e50: 2020 7265 7475 726e 206d 6574 6572 0d0a    return meter..
-00002e60: 0d0a 2020 2020 2020 2020 2320 5550 5045  ..        # UPPE
-00002e70: 520d 0a20 2020 2020 2020 2077 6869 6368  R..        which
-00002e80: 3462 6573 7420 3d20 7768 6963 6834 6265  4best = which4be
-00002e90: 7374 2e75 7070 6572 2829 0d0a 2020 2020  st.upper()..    
-00002ea0: 2020 2020 6d6f 6e69 746f 7273 203d 205b      monitors = [
-00002eb0: 274c 4f53 5327 5d20 2b20 5b6e 616d 652e  'LOSS'] + [name.
-00002ec0: 7570 7065 7228 2920 666f 7220 6e61 6d65  upper() for name
-00002ed0: 2069 6e20 6d6f 6e69 746f 7273 5d20 2b20   in monitors] + 
-00002ee0: 5b77 6869 6368 3462 6573 745d 0d0a 2020  [which4best]..  
-00002ef0: 2020 2020 2020 6d6f 6e69 746f 7273 203d        monitors =
-00002f00: 2073 6f72 7465 6428 7365 7428 6d6f 6e69   sorted(set(moni
-00002f10: 746f 7273 292c 206b 6579 3d6d 6f6e 6974  tors), key=monit
-00002f20: 6f72 732e 696e 6465 7829 0d0a 0d0a 2020  ors.index)....  
-00002f30: 2020 2020 2020 666f 7220 6e61 6d65 2069        for name i
-00002f40: 6e20 6d6f 6e69 746f 7273 3a0d 0a20 2020  n monitors:..   
-00002f50: 2020 2020 2020 2020 2066 6f72 2070 7265           for pre
-00002f60: 6669 7820 696e 2028 2774 7261 696e 272c  fix in ('train',
-00002f70: 2027 7661 6c69 6427 2c20 2774 6573 7427   'valid', 'test'
-00002f80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002f90: 2020 2020 6966 2027 4027 2069 6e20 6e61      if '@' in na
-00002fa0: 6d65 3a0d 0a20 2020 2020 2020 2020 2020  me:..           
-00002fb0: 2020 2020 2020 2020 206c 6173 746e 616d           lastnam
-00002fc0: 652c 204b 203d 206e 616d 652e 7370 6c69  e, K = name.spli
-00002fd0: 7428 2740 2729 0d0a 2020 2020 2020 2020  t('@')..        
-00002fe0: 2020 2020 2020 2020 2020 2020 6d65 7465              mete
-00002ff0: 7220 3d20 7365 745f 6d6f 6e69 746f 7228  r = set_monitor(
-00003000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003010: 2020 2020 2020 2020 2020 6e61 6d65 3d6e            name=n
-00003020: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
-00003030: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00003040: 7374 6e61 6d65 3d6c 6173 746e 616d 652c  stname=lastname,
-00003050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003060: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00003070: 3d70 7265 6669 782c 0d0a 2020 2020 2020  =prefix,..      
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 6b3d 696e 7428 4b29 0d0a 2020 2020    k=int(K)..    
+00000090: 6672 6f6d 2074 6f72 6368 6461 7461 2e64  from torchdata.d
+000000a0: 6174 6170 6970 6573 2e69 7465 7220 696d  atapipes.iter im
+000000b0: 706f 7274 2049 7465 7244 6174 6150 6970  port IterDataPip
+000000c0: 650d 0a66 726f 6d20 746f 7263 682e 7574  e..from torch.ut
+000000d0: 696c 732e 7465 6e73 6f72 626f 6172 6420  ils.tensorboard 
+000000e0: 696d 706f 7274 2053 756d 6d61 7279 5772  import SummaryWr
+000000f0: 6974 6572 0d0a 6672 6f6d 2066 756e 6374  iter..from funct
+00000100: 6f6f 6c73 2069 6d70 6f72 7420 7061 7274  ools import part
+00000110: 6961 6c0d 0a66 726f 6d20 6974 6572 746f  ial..from iterto
+00000120: 6f6c 7320 696d 706f 7274 2070 726f 6475  ols import produ
+00000130: 6374 0d0a 6672 6f6d 2063 6f6c 6c65 6374  ct..from collect
+00000140: 696f 6e73 2069 6d70 6f72 7420 6465 6661  ions import defa
+00000150: 756c 7464 6963 740d 0a66 726f 6d20 6672  ultdict..from fr
+00000160: 6565 706c 6f74 2e75 7469 6c73 2069 6d70  eeplot.utils imp
+00000170: 6f72 7420 696d 706f 7274 5f70 6963 6b6c  ort import_pickl
+00000180: 652c 2065 7870 6f72 745f 7069 636b 6c65  e, export_pickle
+00000190: 0d0a 0d0a 6672 6f6d 202e 6461 7461 2e66  ....from .data.f
+000001a0: 6965 6c64 7320 696d 706f 7274 2046 6965  ields import Fie
+000001b0: 6c64 4d6f 6475 6c65 2c20 4669 656c 6454  ldModule, FieldT
+000001c0: 7570 6c65 0d0a 6672 6f6d 202e 6461 7461  uple..from .data
+000001d0: 2e64 6174 616c 6f61 6465 7220 696d 706f  .dataloader impo
+000001e0: 7274 2044 6174 614c 6f61 6465 720d 0a66  rt DataLoader..f
+000001f0: 726f 6d20 2e6d 6f64 656c 7320 696d 706f  rom .models impo
+00000200: 7274 2052 6563 5379 7341 7263 680d 0a66  rt RecSysArch..f
+00000210: 726f 6d20 2e63 7269 7465 7269 6f6e 7320  rom .criterions 
+00000220: 696d 706f 7274 2042 6173 6543 7269 7465  import BaseCrite
+00000230: 7269 6f6e 0d0a 6672 6f6d 202e 6469 6374  rion..from .dict
+00000240: 326f 626a 2069 6d70 6f72 7420 436f 6e66  2obj import Conf
+00000250: 6967 0d0a 6672 6f6d 202e 7574 696c 7320  ig..from .utils 
+00000260: 696d 706f 7274 2041 7665 7261 6765 4d65  import AverageMe
+00000270: 7465 722c 204d 6f6e 6974 6f72 2c20 7469  ter, Monitor, ti
+00000280: 6d65 6d65 7465 722c 2069 6e66 6f4c 6f67  memeter, infoLog
+00000290: 6765 720d 0a66 726f 6d20 2e6d 6574 7269  ger..from .metri
+000002a0: 6373 2069 6d70 6f72 7420 2a0d 0a66 726f  cs import *..fro
+000002b0: 6d20 2e70 6172 7365 7220 696d 706f 7274  m .parser import
+000002c0: 2054 494d 450d 0a0d 0a0d 0a5f 5f61 6c6c   TIME......__all
+000002d0: 5f5f 203d 205b 2743 6869 6566 436f 6163  __ = ['ChiefCoac
+000002e0: 6827 2c20 2743 6f61 6368 272c 2027 4164  h', 'Coach', 'Ad
+000002f0: 6170 7465 7227 5d0d 0a0d 0a0d 0a44 4546  apter']......DEF
+00000300: 4155 4c54 5f4d 4554 5249 4353 203d 207b  AULT_METRICS = {
+00000310: 0d0a 2020 2020 274c 4f53 5327 3a20 6c61  ..    'LOSS': la
+00000320: 6d62 6461 2078 3a20 782c 0d0a 2020 2020  mbda x: x,..    
+00000330: 2323 2323 2323 2323 2323 2323 230d 0a20  #############.. 
+00000340: 2020 2027 4d53 4527 3a20 6d65 616e 5f73     'MSE': mean_s
+00000350: 7175 6172 6564 5f65 7272 6f72 2c0d 0a20  quared_error,.. 
+00000360: 2020 2027 4d41 4527 3a20 6d65 616e 5f61     'MAE': mean_a
+00000370: 6273 5f65 7272 6f72 2c0d 0a20 2020 2027  bs_error,..    '
+00000380: 524d 5345 273a 2072 6f6f 745f 6d73 652c  RMSE': root_mse,
+00000390: 0d0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
+000003a0: 2323 230d 0a20 2020 2027 5052 4543 4953  ###..    'PRECIS
+000003b0: 494f 4e27 3a20 7072 6563 6973 696f 6e2c  ION': precision,
+000003c0: 0d0a 2020 2020 2752 4543 414c 4c27 3a20  ..    'RECALL': 
+000003d0: 7265 6361 6c6c 2c0d 0a20 2020 2027 4631  recall,..    'F1
+000003e0: 273a 2066 315f 7363 6f72 652c 0d0a 2020  ': f1_score,..  
+000003f0: 2020 2741 5543 273a 2061 7572 6f63 2c0d    'AUC': auroc,.
+00000400: 0a20 2020 2027 4849 5452 4154 4527 3a20  .    'HITRATE': 
+00000410: 6869 745f 7261 7465 2c0d 0a20 2020 2023  hit_rate,..    #
+00000420: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
+00000430: 2020 274e 4443 4727 3a20 6e6f 726d 616c    'NDCG': normal
+00000440: 697a 6564 5f64 6367 2c0d 0a20 2020 2027  ized_dcg,..    '
+00000450: 4d52 5227 3a20 6d65 616e 5f72 6563 6970  MRR': mean_recip
+00000460: 726f 6361 6c5f 7261 6e6b 2c0d 0a20 2020  rocal_rank,..   
+00000470: 2027 4d41 5027 3a20 6d65 616e 5f61 7665   'MAP': mean_ave
+00000480: 7261 6765 5f70 7265 6369 7369 6f6e 0d0a  rage_precision..
+00000490: 7d0d 0a0d 0a44 4546 4155 4c54 5f46 4d54  }....DEFAULT_FMT
+000004a0: 5320 3d20 7b0d 0a20 2020 2027 4c4f 5353  S = {..    'LOSS
+000004b0: 273a 2022 2e35 6622 2c0d 0a20 2020 2023  ': ".5f",..    #
+000004c0: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
+000004d0: 2020 274d 5345 273a 2022 2e34 6622 2c0d    'MSE': ".4f",.
+000004e0: 0a20 2020 2027 4d41 4527 3a20 222e 3466  .    'MAE': ".4f
+000004f0: 222c 0d0a 2020 2020 2752 4d53 4527 3a20  ",..    'RMSE': 
+00000500: 222e 3466 222c 0d0a 2020 2020 2323 2323  ".4f",..    ####
+00000510: 2323 2323 2323 2323 230d 0a20 2020 2027  #########..    '
+00000520: 5052 4543 4953 494f 4e27 3a20 222e 3466  PRECISION': ".4f
+00000530: 222c 0d0a 2020 2020 2752 4543 414c 4c27  ",..    'RECALL'
+00000540: 3a20 222e 3466 222c 0d0a 2020 2020 2746  : ".4f",..    'F
+00000550: 3127 3a20 222e 3466 222c 0d0a 2020 2020  1': ".4f",..    
+00000560: 2741 5543 273a 2022 2e34 6622 2c0d 0a20  'AUC': ".4f",.. 
+00000570: 2020 2027 4849 5452 4154 4527 3a20 222e     'HITRATE': ".
+00000580: 3466 222c 0d0a 2020 2020 2323 2323 2323  4f",..    ######
+00000590: 2323 2323 2323 230d 0a20 2020 2027 4e44  #######..    'ND
+000005a0: 4347 273a 2022 2e34 6622 2c0d 0a20 2020  CG': ".4f",..   
+000005b0: 2027 4d52 5227 3a20 222e 3466 222c 0d0a   'MRR': ".4f",..
+000005c0: 2020 2020 274d 4150 273a 2022 2e34 6622      'MAP': ".4f"
+000005d0: 2c0d 0a7d 0d0a 0d0a 4445 4641 554c 545f  ,..}....DEFAULT_
+000005e0: 4245 5354 5f43 4153 5445 5220 3d20 7b0d  BEST_CASTER = {.
+000005f0: 0a20 2020 2027 4c4f 5353 273a 206d 696e  .    'LOSS': min
+00000600: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
+00000610: 2323 2323 0d0a 2020 2020 274d 5345 273a  ####..    'MSE':
+00000620: 206d 696e 2c0d 0a20 2020 2027 4d41 4527   min,..    'MAE'
+00000630: 3a20 6d69 6e2c 0d0a 2020 2020 2752 4d53  : min,..    'RMS
+00000640: 4527 3a20 6d69 6e2c 0d0a 2020 2020 2323  E': min,..    ##
+00000650: 2323 2323 2323 2323 2323 230d 0a20 2020  ###########..   
+00000660: 2027 5052 4543 4953 494f 4e27 3a20 6d61   'PRECISION': ma
+00000670: 782c 0d0a 2020 2020 2752 4543 414c 4c27  x,..    'RECALL'
+00000680: 3a20 6d61 782c 0d0a 2020 2020 2746 3127  : max,..    'F1'
+00000690: 3a20 6d61 782c 0d0a 2020 2020 2741 5543  : max,..    'AUC
+000006a0: 273a 206d 6178 2c0d 0a20 2020 2027 4849  ': max,..    'HI
+000006b0: 5452 4154 4527 3a20 6d61 782c 0d0a 2020  TRATE': max,..  
+000006c0: 2020 2323 2323 2323 2323 2323 2323 230d    #############.
+000006d0: 0a20 2020 2027 4e44 4347 273a 206d 6178  .    'NDCG': max
+000006e0: 2c0d 0a20 2020 2027 4d52 5227 3a20 6d61  ,..    'MRR': ma
+000006f0: 782c 0d0a 2020 2020 274d 4150 273a 206d  x,..    'MAP': m
+00000700: 6178 2c0d 0a7d 0d0a 0d0a 0d0a 636c 6173  ax,..}......clas
+00000710: 7320 5f44 756d 6d79 4d6f 6475 6c65 2874  s _DummyModule(t
+00000720: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 293a  orch.nn.Module):
+00000730: 0d0a 2020 2020 2222 2254 6869 7320 6973  ..    """This is
+00000740: 2061 2064 756d 6d79 206d 6f64 756c 6520   a dummy module 
+00000750: 7468 6174 2073 6572 7665 7320 6173 2061  that serves as a
+00000760: 2070 6c61 6365 686f 6c64 6572 2066 6f72   placeholder for
+00000770: 2061 2072 6561 6c20 6d6f 6465 6c2e 2222   a real model.""
+00000780: 220d 0a20 2020 2064 6566 2066 6f72 7761  "..    def forwa
+00000790: 7264 2873 656c 662c 202a 6172 6773 2c20  rd(self, *args, 
+000007a0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+000007b0: 2020 2020 2222 2244 756d 6d79 2066 6f72      """Dummy for
+000007c0: 7761 7264 206d 6574 686f 6420 7468 6174  ward method that
+000007d0: 2072 6169 7365 7320 6120 604e 6f74 496d   raises a `NotIm
+000007e0: 706c 656d 656e 7465 6445 7272 6f72 602e  plementedError`.
+000007f0: 2222 220d 0a20 2020 2020 2020 2072 6169  """..        rai
+00000800: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+00000810: 6445 7272 6f72 2822 4e6f 206d 6f64 656c  dError("No model
+00000820: 2061 7661 696c 6162 6c65 2066 6f72 2043   available for C
+00000830: 6f61 6368 202e 2e2e 2229 0d0a 0d0a 2020  oach ...")....  
+00000840: 2020 6465 6620 7374 6570 2873 656c 662c    def step(self,
+00000850: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00000860: 293a 0d0a 2020 2020 2020 2020 2222 2244  ):..        """D
+00000870: 756d 6d79 2073 7465 7020 6d65 7468 6f64  ummy step method
+00000880: 2074 6861 7420 7261 6973 6573 2061 2060   that raises a `
+00000890: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+000008a0: 726f 7260 2e22 2222 0d0a 2020 2020 2020  ror`."""..      
+000008b0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+000008c0: 6d65 6e74 6564 4572 726f 7228 224e 6f20  mentedError("No 
+000008d0: 6f70 7469 6d69 7a65 7220 6f72 206c 7220  optimizer or lr 
+000008e0: 7363 6865 6475 6c65 7220 6176 6169 6c61  scheduler availa
+000008f0: 626c 6520 666f 7220 436f 6163 6820 2e2e  ble for Coach ..
+00000900: 2e22 290d 0a0d 0a20 2020 2064 6566 2062  .")....    def b
+00000910: 6163 6b77 6172 6428 7365 6c66 2c20 2a61  ackward(self, *a
+00000920: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
+00000930: 0a20 2020 2020 2020 2022 2222 4475 6d6d  .        """Dumm
+00000940: 7920 6261 636b 7761 7264 206d 6574 686f  y backward metho
+00000950: 6420 7468 6174 2072 6169 7365 7320 6120  d that raises a 
+00000960: 604e 6f74 496d 706c 656d 656e 7465 6445  `NotImplementedE
+00000970: 7272 6f72 602e 2222 220d 0a20 2020 2020  rror`."""..     
+00000980: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00000990: 656d 656e 7465 6445 7272 6f72 2822 4e6f  ementedError("No
+000009a0: 206f 7074 696d 697a 6572 2061 7661 696c   optimizer avail
+000009b0: 6162 6c65 2066 6f72 2043 6f61 6368 202e  able for Coach .
+000009c0: 2e2e 2229 0d0a 0d0a 0d0a 636c 6173 7320  ..")......class 
+000009d0: 4368 6965 6643 6f61 6368 286d 6574 6163  ChiefCoach(metac
+000009e0: 6c61 7373 3d61 6263 2e41 4243 4d65 7461  lass=abc.ABCMeta
+000009f0: 293a 0d0a 2020 2020 7222 2222 200d 0a20  ):..    r""" .. 
+00000a00: 2020 2054 6865 2060 4368 6965 6643 6f61     The `ChiefCoa
+00000a10: 6368 6020 636c 6173 7320 6973 2074 6865  ch` class is the
+00000a20: 2074 6f70 2d6c 6576 656c 2063 6c61 7373   top-level class
+00000a30: 2066 6f72 2072 756e 6e69 6e67 2074 6865   for running the
+00000a40: 2074 7261 696e 696e 6720 616e 6420 6576   training and ev
+00000a50: 616c 7561 7469 6f6e 206c 6f6f 7073 2e0d  aluation loops..
+00000a60: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+00000a70: 733a 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  s:..    --------
+00000a80: 2d2d 2d0d 0a20 2020 2074 7261 696e 7069  ---..    trainpi
+00000a90: 7065 203a 2049 7465 7244 6174 6150 6970  pe : IterDataPip
+00000aa0: 650d 0a20 2020 2020 2020 2049 7465 7261  e..        Itera
+00000ab0: 626c 6520 6461 7461 2070 6970 656c 696e  ble data pipelin
+00000ac0: 6520 666f 7220 7472 6169 6e69 6e67 2064  e for training d
+00000ad0: 6174 612e 0d0a 2020 2020 7661 6c69 6470  ata...    validp
+00000ae0: 6970 6520 3a20 4974 6572 4461 7461 5069  ipe : IterDataPi
+00000af0: 7065 2c20 6f70 7469 6f6e 616c 0d0a 2020  pe, optional..  
+00000b00: 2020 2020 2020 4974 6572 6162 6c65 2064        Iterable d
+00000b10: 6174 6120 7069 7065 6c69 6e65 2066 6f72  ata pipeline for
+00000b20: 2076 616c 6964 6174 696f 6e20 6461 7461   validation data
+00000b30: 2e0d 0a20 2020 2020 2020 2049 6620 604e  ...        If `N
+00000b40: 6f6e 6560 2c20 7573 6520 6074 7261 696e  one`, use `train
+00000b50: 7069 7065 6020 696e 7374 6561 642e 0d0a  pipe` instead...
+00000b60: 2020 2020 7465 7374 7069 7065 203a 2049      testpipe : I
+00000b70: 7465 7244 6174 6150 6970 652c 206f 7074  terDataPipe, opt
+00000b80: 696f 6e61 6c0d 0a20 2020 2020 2020 2049  ional..        I
+00000b90: 7465 7261 626c 6520 6461 7461 2070 6970  terable data pip
+00000ba0: 656c 696e 6520 666f 7220 7465 7374 696e  eline for testin
+00000bb0: 6720 6461 7461 2e0d 0a20 2020 2020 2020  g data...       
+00000bc0: 2049 6620 604e 6f6e 6560 2c20 7573 6520   If `None`, use 
+00000bd0: 6076 616c 6964 7069 7065 6020 696e 7374  `validpipe` inst
+00000be0: 6561 642e 0d0a 2020 2020 6669 656c 6473  ead...    fields
+00000bf0: 203a 2049 7465 7261 626c 655b 4669 656c   : Iterable[Fiel
+00000c00: 644d 6f64 756c 655d 0d0a 2020 2020 2020  dModule]..      
+00000c10: 2020 5475 706c 6520 6f66 2060 4669 656c    Tuple of `Fiel
+00000c20: 644d 6f64 756c 6560 7320 666f 7220 6461  dModule`s for da
+00000c30: 7461 7365 7420 6669 656c 6473 2e0d 0a20  taset fields... 
+00000c40: 2020 206d 6f64 656c 203a 2055 6e69 6f6e     model : Union
+00000c50: 5b52 6563 5379 7341 7263 682c 2074 6f72  [RecSysArch, tor
+00000c60: 6368 2e6e 6e2e 4d6f 6475 6c65 2c20 4e6f  ch.nn.Module, No
+00000c70: 6e65 5d0d 0a20 2020 2020 2020 204d 6f64  ne]..        Mod
+00000c80: 656c 2066 6f72 2074 7261 696e 696e 6720  el for training 
+00000c90: 616e 6420 6576 616c 7561 7469 6e67 2e20  and evaluating. 
+00000ca0: 0d0a 2020 2020 2020 2020 4966 2060 4e6f  ..        If `No
+00000cb0: 6e65 602c 2075 7365 205f 4475 6d6d 794d  ne`, use _DummyM
+00000cc0: 6f64 756c 6520 696e 7374 6561 642c 2077  odule instead, w
+00000cd0: 6869 6368 2073 686f 756c 6420 6e6f 7420  hich should not 
+00000ce0: 6361 6c6c 2060 666f 7277 6172 6460 2e0d  call `forward`..
+00000cf0: 0a20 2020 2063 7269 7465 7269 6f6e 203a  .    criterion :
+00000d00: 2055 6e69 6f6e 5b42 6173 6543 7269 7465   Union[BaseCrite
+00000d10: 7269 6f6e 2c20 4361 6c6c 6162 6c65 5d0d  rion, Callable].
+00000d20: 0a20 2020 2020 2020 2043 616c 6c61 626c  .        Callabl
+00000d30: 6520 666f 7220 636f 6d70 7574 696e 6720  e for computing 
+00000d40: 7468 6520 6c6f 7373 2066 756e 6374 696f  the loss functio
+00000d50: 6e2e 0d0a 2020 2020 6f70 7469 6d69 7a65  n...    optimize
+00000d60: 7220 3a20 746f 7263 682e 6f70 7469 6d2e  r : torch.optim.
+00000d70: 4f70 7469 6d69 7a65 722c 206f 7074 696f  Optimizer, optio
+00000d80: 6e61 6c0d 0a20 2020 2020 2020 204f 7074  nal..        Opt
+00000d90: 696d 697a 6572 2066 6f72 2075 7064 6174  imizer for updat
+00000da0: 696e 6720 6d6f 6465 6c20 7061 7261 6d65  ing model parame
+00000db0: 7465 7273 2e20 0d0a 2020 2020 2020 2020  ters. ..        
+00000dc0: 4966 2060 4e6f 6e65 602c 2075 7365 205f  If `None`, use _
+00000dd0: 4475 6d6d 794d 6f64 756c 6520 696e 7374  DummyModule inst
+00000de0: 6561 642c 2077 6869 6368 2073 686f 756c  ead, which shoul
+00000df0: 6420 6e6f 7420 6361 6c6c 2060 7374 6570  d not call `step
+00000e00: 6020 616e 6420 6062 6163 6b77 6172 6460  ` and `backward`
+00000e10: 2e0d 0a20 2020 206c 725f 7363 6865 6475  ...    lr_schedu
+00000e20: 6c65 7220 3a20 746f 7263 682e 6f70 7469  ler : torch.opti
+00000e30: 6d2e 6c72 5f73 6368 6564 756c 6572 2e5f  m.lr_scheduler._
+00000e40: 4c52 5363 6865 6475 6c65 722c 206f 7074  LRScheduler, opt
+00000e50: 696f 6e61 6c0d 0a20 2020 2020 2020 204c  ional..        L
+00000e60: 6561 726e 696e 6720 7261 7465 2073 6368  earning rate sch
+00000e70: 6564 756c 6572 2e20 4966 2060 4e6f 6e65  eduler. If `None
+00000e80: 602c 2075 7365 205f 4475 6d6d 794d 6f64  `, use _DummyMod
+00000e90: 756c 6520 696e 7374 6561 642c 200d 0a20  ule instead, .. 
+00000ea0: 2020 2020 2020 2077 6869 6368 2073 686f         which sho
+00000eb0: 756c 6420 6e6f 7420 6361 6c6c 2060 7374  uld not call `st
+00000ec0: 6570 602e 0d0a 2020 2020 6465 7669 6365  ep`...    device
+00000ed0: 203a 2055 6e69 6f6e 5b74 6f72 6368 2e64   : Union[torch.d
+00000ee0: 6576 6963 652c 2073 7472 2c20 696e 745d  evice, str, int]
+00000ef0: 0d0a 2020 2020 2020 2020 4465 7669 6365  ..        Device
+00000f00: 206f 6e20 7768 6963 6820 746f 2072 756e   on which to run
+00000f10: 2074 6865 2063 6f6d 7075 7461 7469 6f6e   the computation
+00000f20: 2e20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
+00000f30: 2d20 6074 6f72 6368 2e64 6576 6963 6560  - `torch.device`
+00000f40: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+00000f50: 6073 7472 603a 204c 696b 6520 6063 7075  `str`: Like `cpu
+00000f60: 602c 2060 6375 6461 3a30 602e 0d0a 2020  `, `cuda:0`...  
+00000f70: 2020 2020 2020 2020 2020 2d20 6069 6e74            - `int
+00000f80: 603a 2055 7369 6e67 2063 7564 613a 6069  `: Using cuda:`i
+00000f90: 6e74 602e 0d0a 2020 2020 2222 220d 0a0d  nt`...    """...
+00000fa0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+00000fb0: 745f 5f28 0d0a 2020 2020 2020 2020 7365  t__(..        se
+00000fc0: 6c66 2c20 2a2c 0d0a 2020 2020 2020 2020  lf, *,..        
+00000fd0: 7472 6169 6e70 6970 653a 2049 7465 7244  trainpipe: IterD
+00000fe0: 6174 6150 6970 652c 2076 616c 6964 7069  ataPipe, validpi
+00000ff0: 7065 3a20 4f70 7469 6f6e 616c 5b49 7465  pe: Optional[Ite
+00001000: 7244 6174 6150 6970 655d 2c20 7465 7374  rDataPipe], test
+00001010: 7069 7065 3a20 4f70 7469 6f6e 616c 5b49  pipe: Optional[I
+00001020: 7465 7244 6174 6150 6970 655d 2c20 6669  terDataPipe], fi
+00001030: 656c 6473 3a20 4974 6572 6162 6c65 5b46  elds: Iterable[F
+00001040: 6965 6c64 4d6f 6475 6c65 5d2c 0d0a 2020  ieldModule],..  
+00001050: 2020 2020 2020 6d6f 6465 6c3a 2055 6e69        model: Uni
+00001060: 6f6e 5b52 6563 5379 7341 7263 682c 2074  on[RecSysArch, t
+00001070: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 2c20  orch.nn.Module, 
+00001080: 4e6f 6e65 5d2c 2063 7269 7465 7269 6f6e  None], criterion
+00001090: 3a20 556e 696f 6e5b 4261 7365 4372 6974  : Union[BaseCrit
+000010a0: 6572 696f 6e2c 2043 616c 6c61 626c 655d  erion, Callable]
+000010b0: 2c20 0d0a 2020 2020 2020 2020 6f70 7469  , ..        opti
+000010c0: 6d69 7a65 723a 204f 7074 696f 6e61 6c5b  mizer: Optional[
+000010d0: 746f 7263 682e 6f70 7469 6d2e 4f70 7469  torch.optim.Opti
+000010e0: 6d69 7a65 725d 2c20 6c72 5f73 6368 6564  mizer], lr_sched
+000010f0: 756c 6572 3a20 4f70 7469 6f6e 616c 5b74  uler: Optional[t
+00001100: 6f72 6368 2e6f 7074 696d 2e6c 725f 7363  orch.optim.lr_sc
+00001110: 6865 6475 6c65 722e 5f4c 5253 6368 6564  heduler._LRSched
+00001120: 756c 6572 5d2c 0d0a 2020 2020 2020 2020  uler],..        
+00001130: 6465 7669 6365 3a20 556e 696f 6e5b 746f  device: Union[to
+00001140: 7263 682e 6465 7669 6365 2c20 7374 722c  rch.device, str,
+00001150: 2069 6e74 5d0d 0a20 2020 2029 3a0d 0a0d   int]..    ):...
+00001160: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+00001170: 656c 6473 3a20 4669 656c 6454 7570 6c65  elds: FieldTuple
+00001180: 5b46 6965 6c64 4d6f 6475 6c65 5d20 3d20  [FieldModule] = 
+00001190: 4669 656c 6454 7570 6c65 2866 6965 6c64  FieldTuple(field
+000011a0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+000011b0: 2e64 6576 6963 6520 3d20 746f 7263 682e  .device = torch.
+000011c0: 6465 7669 6365 2864 6576 6963 6529 0d0a  device(device)..
+000011d0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+000011e0: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
+000011f0: 6375 6461 2e73 6574 5f64 6576 6963 6528  cuda.set_device(
+00001200: 7365 6c66 2e64 6576 6963 6529 0d0a 2020  self.device)..  
+00001210: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00001220: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
+00001230: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00001240: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
+00001250: 6275 7465 4572 726f 723a 0d0a 2020 2020  buteError:..    
+00001260: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
+00001270: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00001280: 745f 6461 7461 7069 7065 2874 7261 696e  t_datapipe(train
+00001290: 7069 7065 2c20 7661 6c69 6470 6970 652c  pipe, validpipe,
+000012a0: 2074 6573 7470 6970 6529 0d0a 2020 2020   testpipe)..    
+000012b0: 2020 2020 7365 6c66 2e5f 7365 745f 6f74      self._set_ot
+000012c0: 6865 7228 6d6f 6465 6c2c 2063 7269 7465  her(model, crite
+000012d0: 7269 6f6e 2c20 6f70 7469 6d69 7a65 722c  rion, optimizer,
+000012e0: 206c 725f 7363 6865 6475 6c65 7229 0d0a   lr_scheduler)..
+000012f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001300: 5f6d 6f64 6520 3d20 2774 7261 696e 270d  _mode = 'train'.
+00001310: 0a0d 0a20 2020 2020 2020 2064 6566 2063  ...        def c
+00001320: 6c65 616e 2829 3a0d 0a20 2020 2020 2020  lean():..       
+00001330: 2020 2020 2070 6172 656e 7420 3d20 7073       parent = ps
+00001340: 7574 696c 2e50 726f 6365 7373 286f 732e  util.Process(os.
+00001350: 6765 7470 6964 2829 290d 0a20 2020 2020  getpid())..     
+00001360: 2020 2020 2020 2063 6869 6c64 7265 6e20         children 
+00001370: 3d20 7061 7265 6e74 2e63 6869 6c64 7265  = parent.childre
+00001380: 6e28 7265 6375 7273 6976 653d 5472 7565  n(recursive=True
+00001390: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+000013a0: 6f72 2070 726f 6365 7373 2069 6e20 6368  or process in ch
+000013b0: 696c 6472 656e 3a0d 0a20 2020 2020 2020  ildren:..       
+000013c0: 2020 2020 2020 2020 2070 726f 6365 7373           process
+000013d0: 2e73 656e 645f 7369 676e 616c 2873 6967  .send_signal(sig
+000013e0: 6e61 6c2e 5349 4754 4552 4d29 0d0a 2020  nal.SIGTERM)..  
+000013f0: 2020 2020 2020 2020 2020 7073 7574 696c            psutil
+00001400: 2e77 6169 745f 7072 6f63 7328 6368 696c  .wait_procs(chil
+00001410: 6472 656e 2c20 7469 6d65 6f75 743d 3529  dren, timeout=5)
+00001420: 0d0a 0d0a 2020 2020 2020 2020 6174 6578  ....        atex
+00001430: 6974 2e72 6567 6973 7465 7228 636c 6561  it.register(clea
+00001440: 6e29 0d0a 0d0a 0d0a 2020 2020 6465 6620  n)......    def 
+00001450: 5f73 6574 5f64 6174 6170 6970 6528 0d0a  _set_datapipe(..
+00001460: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+00001470: 2020 2020 2020 2074 7261 696e 7069 7065         trainpipe
+00001480: 2c0d 0a20 2020 2020 2020 2076 616c 6964  ,..        valid
+00001490: 7069 7065 3d4e 6f6e 652c 0d0a 2020 2020  pipe=None,..    
+000014a0: 2020 2020 7465 7374 7069 7065 3d4e 6f6e      testpipe=Non
+000014b0: 652c 0d0a 2020 2020 293a 0d0a 2020 2020  e,..    ):..    
+000014c0: 2020 2020 2222 2253 6574 2074 6865 2064      """Set the d
+000014d0: 6174 6120 7069 7065 2066 6f72 2074 7261  ata pipe for tra
+000014e0: 696e 696e 672c 2076 616c 6964 6174 696f  ining, validatio
+000014f0: 6e20 616e 6420 7465 7374 2e22 2222 0d0a  n and test."""..
+00001500: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00001510: 696e 7069 7065 203d 2074 7261 696e 7069  inpipe = trainpi
+00001520: 7065 0d0a 2020 2020 2020 2020 7365 6c66  pe..        self
+00001530: 2e76 616c 6964 7069 7065 203d 2073 656c  .validpipe = sel
+00001540: 662e 7472 6169 6e70 6970 6520 6966 2076  f.trainpipe if v
+00001550: 616c 6964 7069 7065 2069 7320 4e6f 6e65  alidpipe is None
+00001560: 2065 6c73 6520 7661 6c69 6470 6970 650d   else validpipe.
+00001570: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+00001580: 7374 7069 7065 203d 2073 656c 662e 7661  stpipe = self.va
+00001590: 6c69 6470 6970 6520 6966 2074 6573 7470  lidpipe if testp
+000015a0: 6970 6520 6973 204e 6f6e 6520 656c 7365  ipe is None else
+000015b0: 2074 6573 7470 6970 650d 0a0d 0a20 2020   testpipe....   
+000015c0: 2064 6566 205f 7365 745f 6f74 6865 7228   def _set_other(
+000015d0: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
+000015e0: 0a20 2020 2020 2020 206d 6f64 656c 3d4e  .        model=N
+000015f0: 6f6e 652c 2063 7269 7465 7269 6f6e 3d4e  one, criterion=N
+00001600: 6f6e 652c 206f 7074 696d 697a 6572 3d4e  one, optimizer=N
+00001610: 6f6e 652c 206c 725f 7363 6865 6475 6c65  one, lr_schedule
+00001620: 723d 4e6f 6e65 2c0d 0a20 2020 2029 3a0d  r=None,..    ):.
+00001630: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
+00001640: 7468 6520 6f74 6865 7220 6e65 6365 7373  the other necess
+00001650: 6172 7920 636f 6d70 6f6e 656e 7473 2e22  ary components."
+00001660: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001670: 2e63 7269 7465 7269 6f6e 203d 2063 7269  .criterion = cri
+00001680: 7465 7269 6f6e 0d0a 2020 2020 2020 2020  terion..        
+00001690: 7365 6c66 2e6d 6f64 656c 203d 206d 6f64  self.model = mod
+000016a0: 656c 2e74 6f28 7365 6c66 2e64 6576 6963  el.to(self.devic
+000016b0: 6529 2069 6620 6d6f 6465 6c20 656c 7365  e) if model else
+000016c0: 205f 4475 6d6d 794d 6f64 756c 6528 290d   _DummyModule().
+000016d0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+000016e0: 7469 6d69 7a65 7220 3d20 6f70 7469 6d69  timizer = optimi
+000016f0: 7a65 7220 6966 206f 7074 696d 697a 6572  zer if optimizer
+00001700: 2065 6c73 6520 5f44 756d 6d79 4d6f 6475   else _DummyModu
+00001710: 6c65 2829 0d0a 2020 2020 2020 2020 7365  le()..        se
+00001720: 6c66 2e6c 725f 7363 6865 6475 6c65 7220  lf.lr_scheduler 
+00001730: 3d20 6c72 5f73 6368 6564 756c 6572 2069  = lr_scheduler i
+00001740: 6620 6c72 5f73 6368 6564 756c 6572 2065  f lr_scheduler e
+00001750: 6c73 6520 5f44 756d 6d79 4d6f 6475 6c65  lse _DummyModule
+00001760: 2829 0d0a 0d0a 2020 2020 4070 726f 7065  ()....    @prope
+00001770: 7274 790d 0a20 2020 2064 6566 206d 6f64  rty..    def mod
+00001780: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00001790: 2020 2222 2247 6574 2074 6865 2063 7572    """Get the cur
+000017a0: 7265 6e74 206d 6f64 6520 6f66 2074 6865  rent mode of the
+000017b0: 2063 6869 6566 2063 6f61 6368 2e22 2222   chief coach."""
+000017c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000017d0: 2073 656c 662e 5f5f 6d6f 6465 0d0a 0d0a   self.__mode....
+000017e0: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
+000017f0: 436f 6163 682f 7472 6169 6e22 290d 0a20  Coach/train").. 
+00001800: 2020 2064 6566 2074 7261 696e 2873 656c     def train(sel
+00001810: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
+00001820: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
+00001830: 7420 7472 6169 6e69 6e67 2061 6e64 2072  t training and r
+00001840: 6574 7572 6e20 7468 6520 7472 6169 6e69  eturn the traini
+00001850: 6e67 206c 6f73 732e 2222 220d 0a20 2020  ng loss."""..   
+00001860: 2020 2020 2073 656c 662e 5f5f 6d6f 6465       self.__mode
+00001870: 203d 2027 7472 6169 6e27 0d0a 2020 2020   = 'train'..    
+00001880: 2020 2020 7365 6c66 2e6d 6f64 656c 2e74      self.model.t
+00001890: 7261 696e 2829 0d0a 2020 2020 2020 2020  rain()..        
+000018a0: 7265 7475 726e 2073 656c 662e 7472 6169  return self.trai
+000018b0: 6e5f 7065 725f 6570 6f63 6828 6570 6f63  n_per_epoch(epoc
+000018c0: 6829 0d0a 0d0a 2020 2020 4074 696d 656d  h)....    @timem
+000018d0: 6574 6572 2822 436f 6163 682f 7661 6c69  eter("Coach/vali
+000018e0: 6422 290d 0a20 2020 2040 746f 7263 682e  d")..    @torch.
+000018f0: 6e6f 5f67 7261 6428 290d 0a20 2020 2064  no_grad()..    d
+00001900: 6566 2076 616c 6964 2873 656c 662c 2065  ef valid(self, e
+00001910: 706f 6368 3a20 696e 7429 3a0d 0a20 2020  poch: int):..   
+00001920: 2020 2020 2022 2222 5374 6172 7420 7661       """Start va
+00001930: 6c69 6461 7469 6f6e 2061 6e64 2072 6574  lidation and ret
+00001940: 7572 6e20 7468 6520 7661 6c69 6461 7469  urn the validati
+00001950: 6f6e 206d 6574 7269 6373 2e22 2222 0d0a  on metrics."""..
+00001960: 2020 2020 2020 2020 7365 6c66 2e5f 5f6d          self.__m
+00001970: 6f64 6520 3d20 2776 616c 6964 270d 0a20  ode = 'valid'.. 
+00001980: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00001990: 6c2e 6576 616c 2829 0d0a 2020 2020 2020  l.eval()..      
+000019a0: 2020 7265 7475 726e 2073 656c 662e 6576    return self.ev
+000019b0: 616c 7561 7465 2865 706f 6368 3d65 706f  aluate(epoch=epo
+000019c0: 6368 2c20 7072 6566 6978 3d27 7661 6c69  ch, prefix='vali
+000019d0: 6427 290d 0a0d 0a20 2020 2040 7469 6d65  d')....    @time
+000019e0: 6d65 7465 7228 2243 6f61 6368 2f74 6573  meter("Coach/tes
+000019f0: 7422 290d 0a20 2020 2040 746f 7263 682e  t")..    @torch.
+00001a00: 6e6f 5f67 7261 6428 290d 0a20 2020 2064  no_grad()..    d
+00001a10: 6566 2074 6573 7428 7365 6c66 2c20 6570  ef test(self, ep
+00001a20: 6f63 683a 2069 6e74 293a 0d0a 2020 2020  och: int):..    
+00001a30: 2020 2020 2222 2253 7461 7274 2074 6573      """Start tes
+00001a40: 7469 6e67 2061 6e64 2072 6574 7572 6e20  ting and return 
+00001a50: 7468 6520 7465 7374 206d 6574 7269 6373  the test metrics
+00001a60: 2e22 2222 0d0a 2020 2020 2020 2020 7365  ."""..        se
+00001a70: 6c66 2e5f 5f6d 6f64 6520 3d20 2774 6573  lf.__mode = 'tes
+00001a80: 7427 0d0a 2020 2020 2020 2020 7365 6c66  t'..        self
+00001a90: 2e6d 6f64 656c 2e65 7661 6c28 290d 0a20  .model.eval().. 
+00001aa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001ab0: 6c66 2e65 7661 6c75 6174 6528 6570 6f63  lf.evaluate(epoc
+00001ac0: 683d 6570 6f63 682c 2070 7265 6669 783d  h=epoch, prefix=
+00001ad0: 2774 6573 7427 290d 0a0d 0a20 2020 2040  'test')....    @
+00001ae0: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
+00001af0: 6f64 0d0a 2020 2020 6465 6620 7472 6169  od..    def trai
+00001b00: 6e5f 7065 725f 6570 6f63 6828 7365 6c66  n_per_epoch(self
+00001b10: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
+00001b20: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00001b30: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00001b40: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00001b50: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
+00001b60: 5f2e 5f5f 6e61 6d65 5f5f 7d2e 7472 6169  _.__name__}.trai
+00001b70: 6e5f 7065 725f 6570 6f63 6828 2920 7368  n_per_epoch() sh
+00001b80: 6f75 6c64 2062 6520 696d 706c 656d 656e  ould be implemen
+00001b90: 7465 6420 2e2e 2e22 0d0a 2020 2020 2020  ted ..."..      
+00001ba0: 2020 290d 0a0d 0a20 2020 2040 6162 632e    )....    @abc.
+00001bb0: 6162 7374 7261 6374 6d65 7468 6f64 0d0a  abstractmethod..
+00001bc0: 2020 2020 6465 6620 6576 616c 7561 7465      def evaluate
+00001bd0: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
+00001be0: 742c 2070 7265 6669 783a 2073 7472 203d  t, prefix: str =
+00001bf0: 2027 7661 6c69 6427 293a 0d0a 2020 2020   'valid'):..    
+00001c00: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00001c10: 6c65 6d65 6e74 6564 4572 726f 7228 0d0a  lementedError(..
+00001c20: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
+00001c30: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
+00001c40: 6e61 6d65 5f5f 7d2e 6576 616c 7561 7465  name__}.evaluate
+00001c50: 2829 2073 686f 756c 6420 6265 2069 6d70  () should be imp
+00001c60: 6c65 6d65 6e74 6564 202e 2e2e 220d 0a20  lemented ...".. 
+00001c70: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00001c80: 6465 6620 7265 6769 7374 6572 5f6d 6574  def register_met
+00001c90: 7269 6328 0d0a 2020 2020 2020 2020 7365  ric(..        se
+00001ca0: 6c66 2c20 6e61 6d65 3a20 7374 722c 2066  lf, name: str, f
+00001cb0: 756e 633a 2043 616c 6c61 626c 652c 200d  unc: Callable, .
+00001cc0: 0a20 2020 2020 2020 2066 6d74 3a20 7374  .        fmt: st
+00001cd0: 7220 3d20 272e 3466 272c 2062 6573 745f  r = '.4f', best_
+00001ce0: 6361 7374 6572 3a20 4361 6c6c 6162 6c65  caster: Callable
+00001cf0: 203d 206d 6178 0d0a 2020 2020 2920 2d3e   = max..    ) ->
+00001d00: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00001d10: 7222 2222 0d0a 2020 2020 2020 2020 5265  r"""..        Re
+00001d20: 6769 7374 6572 2061 206d 6574 7269 632e  gister a metric.
+00001d30: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+00001d40: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00001d60: 2020 2020 6e61 6d65 203a 2073 7472 0d0a      name : str..
+00001d70: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00001d80: 636f 6d70 6c65 7465 206e 616d 6520 6f66  complete name of
+00001d90: 2074 6865 206d 6574 7269 632c 2073 7563   the metric, suc
+00001da0: 6820 6173 2060 4c4f 5353 3260 2e0d 0a20  h as `LOSS2`... 
+00001db0: 2020 2020 2020 2020 2020 2054 6865 206e             The n
+00001dc0: 6f74 6174 696f 6e20 6040 6020 7368 6f75  otation `@` shou
+00001dd0: 6c64 206e 6f74 2062 6520 696e 636c 7564  ld not be includ
+00001de0: 6564 2c20 692e 652e 2c20 274c 4f53 5340  ed, i.e., 'LOSS@
+00001df0: 3227 2069 7320 696e 7661 6c69 642e 0d0a  2' is invalid...
+00001e00: 2020 2020 2020 2020 6675 6e63 203a 2043          func : C
+00001e10: 616c 6c61 626c 650d 0a20 2020 2020 2020  allable..       
+00001e20: 2020 2020 2054 6865 2066 756e 6374 696f       The functio
+00001e30: 6e20 746f 2070 726f 6365 7373 2074 6865  n to process the
+00001e40: 2064 6174 6120 666f 7220 7468 6520 6d65   data for the me
+00001e50: 7472 6963 2e0d 0a20 2020 2020 2020 2066  tric...        f
+00001e60: 6d74 203a 2073 7472 2c20 6f70 7469 6f6e  mt : str, option
+00001e70: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00001e80: 5468 6520 666f 726d 6174 2074 6f20 7573  The format to us
+00001e90: 6520 7768 656e 2070 7269 6e74 696e 6720  e when printing 
+00001ea0: 7468 6520 6d65 7472 6963 2c20 6465 6661  the metric, defa
+00001eb0: 756c 7473 2074 6f20 6027 2e34 6627 602e  ults to `'.4f'`.
+00001ec0: 0d0a 2020 2020 2020 2020 6265 7374 5f63  ..        best_c
+00001ed0: 6173 7465 7220 3a20 4361 6c6c 6162 6c65  aster : Callable
+00001ee0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00001ef0: 2020 2020 2020 2020 4120 6675 6e63 7469          A functi
+00001f00: 6f6e 2075 7365 6420 746f 2063 6173 7420  on used to cast 
+00001f10: 7468 6520 6265 7374 2076 616c 7565 206f  the best value o
+00001f20: 6620 7468 6520 6d65 7472 6963 2c20 6465  f the metric, de
+00001f30: 6661 756c 7473 2074 6f20 606d 6178 602e  faults to `max`.
+00001f40: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00001f50: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+00001f60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001f70: 0d0a 2020 2020 2020 2020 4e6f 6e65 0d0a  ..        None..
+00001f80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001f90: 2020 5261 6973 6573 0d0a 2020 2020 2020    Raises..      
+00001fa0: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
+00001fb0: 2020 4173 7365 7274 696f 6e45 7272 6f72    AssertionError
+00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00001fd0: 656e 2060 6e61 6d65 6020 6861 7320 616c  en `name` has al
+00001fe0: 7265 6164 7920 6265 656e 2072 6567 6973  ready been regis
+00001ff0: 7465 7265 6420 6f72 2063 6f6e 7461 696e  tered or contain
+00002000: 7320 7468 6520 6e6f 7461 7469 6f6e 2060  s the notation `
+00002010: 4060 2e0d 0a20 2020 2020 2020 2022 2222  @`...        """
+00002020: 0d0a 0d0a 2020 2020 2020 2020 6e61 6d65  ....        name
+00002030: 203d 206e 616d 652e 7570 7065 7228 290d   = name.upper().
+00002040: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002050: 4445 4641 554c 545f 4d45 5452 4943 532e  DEFAULT_METRICS.
+00002060: 6765 7428 6e61 6d65 2c20 4e6f 6e65 2920  get(name, None) 
+00002070: 6973 204e 6f6e 652c 2066 2254 6865 206d  is None, f"The m
+00002080: 6574 7269 6320 7b6e 616d 657d 2061 6c72  etric {name} alr
+00002090: 6561 6479 2065 7869 7374 7320 2e2e 2e22  eady exists ..."
+000020a0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000020b0: 2027 4027 206e 6f74 2069 6e20 6e61 6d65   '@' not in name
+000020c0: 2c20 6622 5468 6520 6d65 7472 6963 206e  , f"The metric n
+000020d0: 616d 6520 6861 7320 696e 7661 6c69 6420  ame has invalid 
+000020e0: 6e6f 7461 7469 6f6e 206f 6620 6040 2720  notation of `@' 
+000020f0: 2e2e 2e22 0d0a 2020 2020 2020 2020 4445  ..."..        DE
+00002100: 4641 554c 545f 4d45 5452 4943 535b 6e61  FAULT_METRICS[na
+00002110: 6d65 5d20 3d20 6675 6e63 0d0a 2020 2020  me] = func..    
+00002120: 2020 2020 4445 4641 554c 545f 464d 5453      DEFAULT_FMTS
+00002130: 5b6e 616d 655d 203d 2066 6d74 0d0a 2020  [name] = fmt..  
+00002140: 2020 2020 2020 4445 4641 554c 545f 4245        DEFAULT_BE
+00002150: 5354 5f43 4153 5445 525b 6e61 6d65 5d20  ST_CASTER[name] 
+00002160: 3d20 6265 7374 5f63 6173 7465 720d 0a0d  = best_caster...
+00002170: 0a0d 0a63 6c61 7373 2043 6f61 6368 2843  ...class Coach(C
+00002180: 6869 6566 436f 6163 6829 3a0d 0a20 2020  hiefCoach):..   
+00002190: 2022 2222 5468 6520 6672 616d 6577 6f72   """The framewor
+000021a0: 6b20 666f 7220 7472 6169 6e69 6e67 2e22  k for training."
+000021b0: 2222 0d0a 0d0a 2020 2020 6465 6620 7072  ""....    def pr
+000021c0: 6570 6172 655f 6461 7461 6c6f 6164 6572  epare_dataloader
+000021d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+000021e0: 0a20 2020 2020 2020 2022 2222 5072 6570  .        """Prep
+000021f0: 6172 6520 6461 7461 206c 6f61 6465 7273  are data loaders
+00002200: 2066 6f72 2074 7261 696e 696e 672c 2076   for training, v
+00002210: 616c 6964 6174 696f 6e2c 2061 6e64 2074  alidation, and t
+00002220: 6573 7469 6e67 2064 6174 612e 2222 220d  esting data.""".
+00002230: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00002240: 6169 6e6c 6f61 6465 7220 3d20 4461 7461  ainloader = Data
+00002250: 4c6f 6164 6572 280d 0a20 2020 2020 2020  Loader(..       
+00002260: 2020 2020 2064 6174 6170 6970 653d 7365       datapipe=se
+00002270: 6c66 2e74 7261 696e 7069 7065 2c20 0d0a  lf.trainpipe, ..
+00002280: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00002290: 776f 726b 6572 733d 7365 6c66 2e63 6667  workers=self.cfg
+000022a0: 2e6e 756d 5f77 6f72 6b65 7273 2c0d 0a20  .num_workers,.. 
+000022b0: 2020 2020 2020 2020 2020 2070 696e 5f6d             pin_m
+000022c0: 656d 6f72 793d 7365 6c66 2e63 6667 2e70  emory=self.cfg.p
+000022d0: 696e 5f6d 656d 6f72 790d 0a20 2020 2020  in_memory..     
+000022e0: 2020 2029 0d0a 2020 2020 2020 2020 7365     )..        se
+000022f0: 6c66 2e76 616c 6964 6c6f 6164 6572 203d  lf.validloader =
+00002300: 2044 6174 614c 6f61 6465 7228 0d0a 2020   DataLoader(..  
+00002310: 2020 2020 2020 2020 2020 6461 7461 7069            datapi
+00002320: 7065 3d73 656c 662e 7661 6c69 6470 6970  pe=self.validpip
+00002330: 652c 200d 0a20 2020 2020 2020 2020 2020  e, ..           
+00002340: 206e 756d 5f77 6f72 6b65 7273 3d73 656c   num_workers=sel
+00002350: 662e 6366 672e 6e75 6d5f 776f 726b 6572  f.cfg.num_worker
+00002360: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00002370: 7069 6e5f 6d65 6d6f 7279 3d73 656c 662e  pin_memory=self.
+00002380: 6366 672e 7069 6e5f 6d65 6d6f 7279 0d0a  cfg.pin_memory..
+00002390: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000023a0: 2020 2073 656c 662e 7465 7374 6c6f 6164     self.testload
+000023b0: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
+000023c0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+000023d0: 7461 7069 7065 3d73 656c 662e 7465 7374  tapipe=self.test
+000023e0: 7069 7065 2c20 0d0a 2020 2020 2020 2020  pipe, ..        
+000023f0: 2020 2020 6e75 6d5f 776f 726b 6572 733d      num_workers=
+00002400: 7365 6c66 2e63 6667 2e6e 756d 5f77 6f72  self.cfg.num_wor
+00002410: 6b65 7273 2c0d 0a20 2020 2020 2020 2020  kers,..         
+00002420: 2020 2070 696e 5f6d 656d 6f72 793d 7365     pin_memory=se
+00002430: 6c66 2e63 6667 2e70 696e 5f6d 656d 6f72  lf.cfg.pin_memor
+00002440: 790d 0a20 2020 2020 2020 2029 0d0a 2020  y..        )..  
+00002450: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
+00002460: 790d 0a20 2020 2064 6566 2064 6174 616c  y..    def datal
+00002470: 6f61 6465 7228 7365 6c66 293a 0d0a 2020  oader(self):..  
+00002480: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00002490: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+000024a0: 6720 6461 7461 206c 6f61 6465 7220 6465  g data loader de
+000024b0: 7065 6e64 696e 6720 6f6e 2074 6865 2063  pending on the c
+000024c0: 7572 7265 6e74 206d 6f64 652e 2222 220d  urrent mode.""".
+000024d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000024e0: 2e6d 6f64 6520 3d3d 2027 7472 6169 6e27  .mode == 'train'
+000024f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00002500: 6574 7572 6e20 7365 6c66 2e74 7261 696e  eturn self.train
+00002510: 6c6f 6164 6572 0d0a 2020 2020 2020 2020  loader..        
+00002520: 656c 6966 2073 656c 662e 6d6f 6465 203d  elif self.mode =
+00002530: 3d20 2776 616c 6964 273a 0d0a 2020 2020  = 'valid':..    
+00002540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002550: 656c 662e 7661 6c69 646c 6f61 6465 720d  elf.validloader.
+00002560: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002570: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002580: 726e 2073 656c 662e 7465 7374 6c6f 6164  rn self.testload
+00002590: 6572 0d0a 0d0a 2020 2020 4070 726f 7065  er....    @prope
+000025a0: 7274 790d 0a20 2020 2064 6566 206d 6f6e  rty..    def mon
+000025b0: 6974 6f72 7328 7365 6c66 2920 2d3e 204d  itors(self) -> M
+000025c0: 6f6e 6974 6f72 3a0d 0a20 2020 2020 2020  onitor:..       
+000025d0: 2022 2222 5265 7475 726e 2074 6865 206d   """Return the m
+000025e0: 6f6e 6974 6f72 2064 6963 7469 6f6e 6172  onitor dictionar
+000025f0: 7920 666f 7220 7468 6520 6469 6666 6572  y for the differ
+00002600: 656e 7420 6d6f 6465 7320 2827 7472 6169  ent modes ('trai
+00002610: 6e27 2c20 2776 616c 6964 272c 2027 7465  n', 'valid', 'te
+00002620: 7374 2729 2e22 2222 0d0a 2020 2020 2020  st')."""..      
+00002630: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00002640: 6d6f 6e69 746f 7273 0d0a 0d0a 2020 2020  monitors....    
+00002650: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00002660: 6566 206d 6574 6572 3462 6573 7428 7365  ef meter4best(se
+00002670: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00002680: 7475 726e 2073 656c 662e 5f5f 6265 7374  turn self.__best
+00002690: 5f6d 6574 6572 0d0a 0d0a 2020 2020 406d  _meter....    @m
+000026a0: 6574 6572 3462 6573 742e 7365 7474 6572  eter4best.setter
+000026b0: 0d0a 2020 2020 6465 6620 6d65 7465 7234  ..    def meter4
+000026c0: 6265 7374 2873 656c 662c 206d 6574 6572  best(self, meter
+000026d0: 3a20 4176 6572 6167 654d 6574 6572 293a  : AverageMeter):
+000026e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000026f0: 5f62 6573 745f 6d65 7465 7220 3d20 6d65  _best_meter = me
+00002700: 7465 720d 0a20 2020 2020 2020 2069 6e66  ter..        inf
+00002710: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
+00002720: 5d20 3e3e 3e20 5365 7420 6265 7374 206d  ] >>> Set best m
+00002730: 6574 6572 3a20 7b6d 6574 6572 2e6e 616d  eter: {meter.nam
+00002740: 657d 2022 290d 0a0d 0a20 2020 2040 7469  e} ")....    @ti
+00002750: 6d65 6d65 7465 7228 2243 6f61 6368 2f63  memeter("Coach/c
+00002760: 6f6d 7069 6c65 2229 0d0a 2020 2020 6465  ompile")..    de
+00002770: 6620 636f 6d70 696c 6528 0d0a 2020 2020  f compile(..    
+00002780: 2020 2020 7365 6c66 2c20 6366 673a 2043      self, cfg: C
+00002790: 6f6e 6669 672c 206d 6f6e 6974 6f72 733a  onfig, monitors:
+000027a0: 204c 6973 745b 7374 725d 2c20 0d0a 2020   List[str], ..  
+000027b0: 2020 2020 2020 7768 6963 6834 6265 7374        which4best
+000027c0: 3a20 7374 7220 3d20 274c 4f53 5327 0d0a  : str = 'LOSS'..
+000027d0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+000027e0: 7222 2222 0d0a 2020 2020 2020 2020 4c6f  r"""..        Lo
+000027f0: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
+00002800: 7469 6f6e 2061 6e64 2073 6574 2075 7020  tion and set up 
+00002810: 6d6f 6e69 746f 7273 2066 6f72 2074 7261  monitors for tra
+00002820: 696e 696e 672e 0d0a 0d0a 2020 2020 2020  ining.....      
+00002830: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00002840: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00002850: 0d0a 2020 2020 2020 2020 6366 6720 3a20  ..        cfg : 
+00002860: 436f 6e66 6967 0d0a 2020 2020 2020 2020  Config..        
+00002870: 2020 2020 4120 636f 6e66 6967 7572 6174      A configurat
+00002880: 696f 6e20 6f62 6a65 6374 2077 6974 6820  ion object with 
+00002890: 7468 6520 7472 6169 6e69 6e67 2064 6574  the training det
+000028a0: 6169 6c73 2e0d 0a20 2020 2020 2020 206d  ails...        m
+000028b0: 6f6e 6974 6f72 7320 3a20 4c69 7374 5b73  onitors : List[s
+000028c0: 7472 5d0d 0a20 2020 2020 2020 2020 2020  tr]..           
+000028d0: 2041 206c 6973 7420 6f66 206d 6574 7269   A list of metri
+000028e0: 6320 6e61 6d65 7320 746f 2062 6520 6d6f  c names to be mo
+000028f0: 6e69 746f 7265 6420 6475 7269 6e67 2074  nitored during t
+00002900: 7261 696e 696e 672e 0d0a 2020 2020 2020  raining...      
+00002910: 2020 7768 6963 6834 6265 7374 203a 2073    which4best : s
+00002920: 7472 2c20 6465 6661 756c 7473 2060 4c4f  tr, defaults `LO
+00002930: 5353 270d 0a20 2020 2020 2020 2020 2020  SS'..           
+00002940: 2054 6865 206d 6574 7269 6320 7573 6564   The metric used
+00002950: 2066 6f72 2073 656c 6563 7469 6e67 2074   for selecting t
+00002960: 6865 2062 6573 7420 6368 6563 6b70 6f69  he best checkpoi
+00002970: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2045  nt.....        E
+00002980: 7861 6d70 6c65 730d 0a20 2020 2020 2020  xamples..       
+00002990: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
+000029a0: 2020 203e 3e3e 2063 6f61 6368 3a20 436f     >>> coach: Co
+000029b0: 6163 680d 0a20 2020 2020 2020 203e 3e3e  ach..        >>>
+000029c0: 2063 6f61 6368 2e63 6f6d 7069 6c65 2863   coach.compile(c
+000029d0: 6667 2c20 6d6f 6e69 746f 7273 3d5b 276c  fg, monitors=['l
+000029e0: 6f73 7327 2c20 2772 6563 616c 6c40 3130  oss', 'recall@10
+000029f0: 272c 2027 7265 6361 6c6c 4032 3027 2c20  ', 'recall@20', 
+00002a00: 276e 6463 6740 3130 272c 2027 6e64 6367  'ndcg@10', 'ndcg
+00002a10: 4032 3027 5d29 0d0a 2020 2020 2020 2020  @20'])..        
+00002a20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00002a30: 662e 6366 6720 3d20 6366 670d 0a20 2020  f.cfg = cfg..   
+00002a40: 2020 2020 2023 206d 6574 6572 7320 666f       # meters fo
+00002a50: 7220 7472 6169 6e7c 7661 6c69 647c 7465  r train|valid|te
+00002a60: 7374 0d0a 2020 2020 2020 2020 7365 6c66  st..        self
+00002a70: 2e5f 5f6d 6f6e 6974 6f72 7320 3d20 4d6f  .__monitors = Mo
+00002a80: 6e69 746f 7228 290d 0a20 2020 2020 2020  nitor()..       
+00002a90: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
+00002aa0: 5b27 7472 6169 6e27 5d20 3d20 6465 6661  ['train'] = defa
+00002ab0: 756c 7464 6963 7428 6c69 7374 290d 0a20  ultdict(list).. 
+00002ac0: 2020 2020 2020 2073 656c 662e 5f5f 6d6f         self.__mo
+00002ad0: 6e69 746f 7273 5b27 7661 6c69 6427 5d20  nitors['valid'] 
+00002ae0: 3d20 6465 6661 756c 7464 6963 7428 6c69  = defaultdict(li
+00002af0: 7374 290d 0a20 2020 2020 2020 2073 656c  st)..        sel
+00002b00: 662e 5f5f 6d6f 6e69 746f 7273 5b27 7465  f.__monitors['te
+00002b10: 7374 275d 203d 2064 6566 6175 6c74 6469  st'] = defaultdi
+00002b20: 6374 286c 6973 7429 0d0a 0d0a 2020 2020  ct(list)....    
+00002b30: 2020 2020 6465 6620 7365 745f 6d6f 6e69      def set_moni
+00002b40: 746f 7228 0d0a 2020 2020 2020 2020 2020  tor(..          
+00002b50: 2020 6e61 6d65 3a20 7374 722c 206c 6173    name: str, las
+00002b60: 746e 616d 653a 2073 7472 2c20 7072 6566  tname: str, pref
+00002b70: 6978 3a20 7374 7220 3d20 2774 7261 696e  ix: str = 'train
+00002b80: 272c 202a 2a6b 7761 7267 730d 0a20 2020  ', **kwargs..   
+00002b90: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00002ba0: 2020 2020 2022 2222 4164 6420 6120 6d6f       """Add a mo
+00002bb0: 6e69 746f 7220 666f 7220 7468 6520 7370  nitor for the sp
+00002bc0: 6563 6966 6965 6420 6d65 7472 6963 2e22  ecified metric."
+00002bd0: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
+00002be0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00002bf0: 2020 2020 2020 6d65 7465 7220 3d20 4176        meter = Av
+00002c00: 6572 6167 654d 6574 6572 280d 0a20 2020  erageMeter(..   
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 2020 206e 616d 653d 6e61 6d65 2c0d       name=name,.
+00002c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c40: 2020 2020 2020 2020 206d 6574 7269 633d           metric=
+00002c50: 7061 7274 6961 6c28 4445 4641 554c 545f  partial(DEFAULT_
+00002c60: 4d45 5452 4943 535b 6c61 7374 6e61 6d65  METRICS[lastname
+00002c70: 5d2c 202a 2a6b 7761 7267 7329 2c0d 0a20  ], **kwargs),.. 
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2020 2020 2066 6d74 3d44 4546 4155         fmt=DEFAU
+00002ca0: 4c54 5f46 4d54 535b 6c61 7374 6e61 6d65  LT_FMTS[lastname
+00002cb0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00002cc0: 2020 2020 2020 2020 2020 2020 6265 7374              best
+00002cd0: 5f63 6173 7465 723d 4445 4641 554c 545f  _caster=DEFAULT_
+00002ce0: 4245 5354 5f43 4153 5445 525b 6c61 7374  BEST_CASTER[last
+00002cf0: 6e61 6d65 5d0d 0a20 2020 2020 2020 2020  name]..         
+00002d00: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00002d10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002d20: 6c66 2e5f 5f6d 6f6e 6974 6f72 735b 7072  lf.__monitors[pr
+00002d30: 6566 6978 5d5b 6c61 7374 6e61 6d65 5d2e  efix][lastname].
+00002d40: 6170 7065 6e64 286d 6574 6572 290d 0a20  append(meter).. 
+00002d50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00002d60: 7420 4b65 7945 7272 6f72 3a0d 0a20 2020  t KeyError:..   
+00002d70: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00002d80: 7365 204b 6579 4572 726f 7228 0d0a 2020  se KeyError(..  
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 6622 5468 6520 6d65 7472 6963 206f    f"The metric o
+00002db0: 6620 7b6c 6173 746e 616d 657d 2069 7320  f {lastname} is 
+00002dc0: 6e6f 7420 696e 636c 7564 6564 2e20 220d  not included. ".
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2020 2020 2066 2259 6f75 2063 616e 2072       f"You can r
+00002df0: 6567 6973 7465 7220 6279 2063 616c 6c69  egister by calli
+00002e00: 6e67 2060 7265 6769 7374 6572 5f6d 6574  ng `register_met
+00002e10: 7269 6328 2e2e 2e29 2720 2e2e 2e22 0d0a  ric(...)' ..."..
+00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e30: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00002e40: 6574 7572 6e20 6d65 7465 720d 0a0d 0a20  eturn meter.... 
+00002e50: 2020 2020 2020 2023 2055 5050 4552 0d0a         # UPPER..
+00002e60: 2020 2020 2020 2020 7768 6963 6834 6265          which4be
+00002e70: 7374 203d 2077 6869 6368 3462 6573 742e  st = which4best.
+00002e80: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
+00002e90: 206d 6f6e 6974 6f72 7320 3d20 5b27 4c4f   monitors = ['LO
+00002ea0: 5353 275d 202b 205b 6e61 6d65 2e75 7070  SS'] + [name.upp
+00002eb0: 6572 2829 2066 6f72 206e 616d 6520 696e  er() for name in
+00002ec0: 206d 6f6e 6974 6f72 735d 202b 205b 7768   monitors] + [wh
+00002ed0: 6963 6834 6265 7374 5d0d 0a20 2020 2020  ich4best]..     
+00002ee0: 2020 206d 6f6e 6974 6f72 7320 3d20 736f     monitors = so
+00002ef0: 7274 6564 2873 6574 286d 6f6e 6974 6f72  rted(set(monitor
+00002f00: 7329 2c20 6b65 793d 6d6f 6e69 746f 7273  s), key=monitors
+00002f10: 2e69 6e64 6578 290d 0a0d 0a20 2020 2020  .index)....     
+00002f20: 2020 2066 6f72 206e 616d 6520 696e 206d     for name in m
+00002f30: 6f6e 6974 6f72 733a 0d0a 2020 2020 2020  onitors:..      
+00002f40: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
+00002f50: 2069 6e20 2827 7472 6169 6e27 2c20 2776   in ('train', 'v
+00002f60: 616c 6964 272c 2027 7465 7374 2729 3a0d  alid', 'test'):.
+00002f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f80: 2069 6620 2740 2720 696e 206e 616d 653a   if '@' in name:
+00002f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002fa0: 2020 2020 2020 6c61 7374 6e61 6d65 2c20        lastname, 
+00002fb0: 4b20 3d20 6e61 6d65 2e73 706c 6974 2827  K = name.split('
+00002fc0: 4027 290d 0a20 2020 2020 2020 2020 2020  @')..           
+00002fd0: 2020 2020 2020 2020 206d 6574 6572 203d           meter =
+00002fe0: 2073 6574 5f6d 6f6e 6974 6f72 280d 0a20   set_monitor(.. 
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003000: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
+00003010: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003020: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
+00003030: 616d 653d 6c61 7374 6e61 6d65 2c0d 0a20  ame=lastname,.. 
+00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003050: 2020 2020 2020 2070 7265 6669 783d 7072         prefix=pr
+00003060: 6566 6978 2c0d 0a20 2020 2020 2020 2020  efix,..         
+00003070: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00003080: 3d69 6e74 284b 290d 0a20 2020 2020 2020  =int(K)..       
+00003090: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
 000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000030c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000030d0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000030e0: 7374 6e61 6d65 203d 206e 616d 650d 0a20  stname = name.. 
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003100: 2020 206d 6574 6572 203d 2073 6574 5f6d     meter = set_m
-00003110: 6f6e 6974 6f72 280d 0a20 2020 2020 2020  onitor(..       
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 206e 616d 653d 6e61 6d65 2c0d 0a20 2020   name=name,..   
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2020 206c 6173 746e 616d 653d 6c61       lastname=la
-00003160: 7374 6e61 6d65 2c0d 0a20 2020 2020 2020  stname,..       
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2070 7265 6669 783d 7072 6566 6978 0d0a   prefix=prefix..
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-000031b0: 2020 2020 2020 2069 6620 7072 6566 6978         if prefix
-000031c0: 203d 3d20 2776 616c 6964 2720 616e 6420   == 'valid' and 
-000031d0: 6e61 6d65 203d 3d20 7768 6963 6834 6265  name == which4be
-000031e0: 7374 3a0d 0a20 2020 2020 2020 2020 2020  st:..           
-000031f0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-00003200: 7465 7234 6265 7374 203d 206d 6574 6572  ter4best = meter
-00003210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003220: 2020 2020 2020 7365 6c66 2e5f 6265 7374        self._best
-00003230: 203d 202d 666c 6f61 7428 2769 6e66 2729   = -float('inf')
-00003240: 2069 6620 6d65 7465 722e 6361 7374 6572   if meter.caster
-00003250: 2069 7320 6d61 7820 656c 7365 2066 6c6f   is max else flo
-00003260: 6174 2827 696e 6627 290d 0a20 2020 2020  at('inf')..     
-00003270: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003280: 656c 662e 5f62 6573 745f 6570 6f63 6820  elf._best_epoch 
-00003290: 3d20 300d 0a0d 0a20 2020 2020 2020 2023  = 0....        #
-000032a0: 2050 7265 7061 7265 2064 6174 6120 6c6f   Prepare data lo
-000032b0: 6164 6572 730d 0a20 2020 2020 2020 2073  aders..        s
-000032c0: 656c 662e 7072 6570 6172 655f 6461 7461  elf.prepare_data
-000032d0: 6c6f 6164 6572 2829 0d0a 0d0a 2020 2020  loader()....    
-000032e0: 6465 6620 7361 7665 2873 656c 6629 202d  def save(self) -
-000032f0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00003300: 2022 2222 5361 7665 2074 6865 206d 6f64   """Save the mod
-00003310: 656c 2222 220d 0a20 2020 2020 2020 2074  el"""..        t
-00003320: 6f72 6368 2e73 6176 6528 7365 6c66 2e6d  orch.save(self.m
-00003330: 6f64 656c 2e73 7461 7465 5f64 6963 7428  odel.state_dict(
-00003340: 292c 206f 732e 7061 7468 2e6a 6f69 6e28  ), os.path.join(
-00003350: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
-00003360: 482c 2073 656c 662e 6366 672e 5341 5645  H, self.cfg.SAVE
-00003370: 445f 4649 4c45 4e41 4d45 2929 0d0a 0d0a  D_FILENAME))....
-00003380: 2020 2020 6465 6620 6c6f 6164 2873 656c      def load(sel
-00003390: 662c 2070 6174 683a 2073 7472 2c20 6669  f, path: str, fi
-000033a0: 6c65 6e61 6d65 3a20 4f70 7469 6f6e 616c  lename: Optional
-000033b0: 5b73 7472 5d20 3d20 4e6f 6e65 2c20 2a2a  [str] = None, **
-000033c0: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
-000033d0: 0d0a 2020 2020 2020 2020 6669 6c65 6e61  ..        filena
-000033e0: 6d65 203d 2073 656c 662e 6366 672e 5341  me = self.cfg.SA
-000033f0: 5645 445f 4649 4c45 4e41 4d45 2069 6620  VED_FILENAME if 
-00003400: 6669 6c65 6e61 6d65 2069 7320 4e6f 6e65  filename is None
-00003410: 2065 6c73 6520 6669 6c65 6e61 6d65 0d0a   else filename..
-00003420: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
-00003430: 656c 2e6c 6f61 645f 7374 6174 655f 6469  el.load_state_di
-00003440: 6374 2874 6f72 6368 2e6c 6f61 6428 6f73  ct(torch.load(os
-00003450: 2e70 6174 682e 6a6f 696e 2870 6174 682c  .path.join(path,
-00003460: 2066 696c 656e 616d 6529 2c20 2a2a 6b77   filename), **kw
-00003470: 6172 6773 2929 0d0a 0d0a 2020 2020 6465  args))....    de
-00003480: 6620 7361 7665 5f63 6865 636b 706f 696e  f save_checkpoin
-00003490: 7428 7365 6c66 2c20 6570 6f63 683a 2069  t(self, epoch: i
-000034a0: 6e74 2920 2d3e 204e 6f6e 653a 0d0a 2020  nt) -> None:..  
-000034b0: 2020 2020 2020 7222 2222 0d0a 2020 2020        r"""..    
-000034c0: 2020 2020 5361 7665 2063 7572 7265 6e74      Save current
-000034d0: 2063 6865 636b 706f 696e 7420 6174 2065   checkpoint at e
-000034e0: 706f 6368 2e0d 0a0d 0a20 2020 2020 2020  poch.....       
-000034f0: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-00003500: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00003510: 2d0d 0a20 2020 2020 2020 2020 2020 2065  -..            e
-00003520: 706f 6368 203a 696e 7420 4375 7272 656e  poch :int Curren
-00003530: 7420 6570 6f63 6820 6e75 6d62 6572 2e0d  t epoch number..
-00003540: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00003550: 6e73 3a0d 0a20 2020 2020 2020 202d 2d2d  ns:..        ---
-00003560: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2020  -----..         
-00003570: 2020 204e 6f6e 650d 0a20 2020 2020 2020     None..       
-00003580: 2022 2222 0d0a 2020 2020 2020 2020 7061   """..        pa
-00003590: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-000035a0: 6e28 7365 6c66 2e63 6667 2e43 4845 434b  n(self.cfg.CHECK
-000035b0: 504f 494e 545f 5041 5448 2c20 7365 6c66  POINT_PATH, self
-000035c0: 2e63 6667 2e43 4845 434b 504f 494e 545f  .cfg.CHECKPOINT_
-000035d0: 4649 4c45 4e41 4d45 290d 0a20 2020 2020  FILENAME)..     
-000035e0: 2020 2063 6865 636b 706f 696e 7420 3d20     checkpoint = 
-000035f0: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
-00003600: 6368 6563 6b70 6f69 6e74 5b27 6570 6f63  checkpoint['epoc
-00003610: 6827 5d20 3d20 6570 6f63 680d 0a20 2020  h'] = epoch..   
-00003620: 2020 2020 2066 6f72 206d 6f64 756c 6520       for module 
-00003630: 696e 2073 656c 662e 6366 672e 4348 4543  in self.cfg.CHEC
-00003640: 4b50 4f49 4e54 5f4d 4f44 554c 4553 3a0d  KPOINT_MODULES:.
-00003650: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-00003660: 636b 706f 696e 745b 6d6f 6475 6c65 5d20  ckpoint[module] 
-00003670: 3d20 6765 7461 7474 7228 7365 6c66 2c20  = getattr(self, 
-00003680: 6d6f 6475 6c65 292e 7374 6174 655f 6469  module).state_di
-00003690: 6374 2829 0d0a 2020 2020 2020 2020 6368  ct()..        ch
-000036a0: 6563 6b70 6f69 6e74 5b27 6d6f 6e69 746f  eckpoint['monito
-000036b0: 7273 275d 203d 2073 656c 662e 6d6f 6e69  rs'] = self.moni
-000036c0: 746f 7273 2e73 7461 7465 5f64 6963 7428  tors.state_dict(
-000036d0: 290d 0a20 2020 2020 2020 2074 6f72 6368  )..        torch
-000036e0: 2e73 6176 6528 6368 6563 6b70 6f69 6e74  .save(checkpoint
-000036f0: 2c20 7061 7468 290d 0a0d 0a20 2020 2064  , path)....    d
-00003700: 6566 206c 6f61 645f 6368 6563 6b70 6f69  ef load_checkpoi
-00003710: 6e74 2873 656c 6629 202d 3e20 696e 743a  nt(self) -> int:
-00003720: 0d0a 2020 2020 2020 2020 7222 2222 0d0a  ..        r"""..
-00003730: 2020 2020 2020 2020 4c6f 6164 206c 6173          Load las
-00003740: 7420 7361 7665 6420 6368 6563 6b70 6f69  t saved checkpoi
-00003750: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2052  nt.....        R
-00003760: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00003770: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
-00003780: 2020 2065 706f 6368 3a20 696e 7420 0d0a     epoch: int ..
-00003790: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000037a0: 6570 6f63 6820 6e75 6d62 6572 206c 6f61  epoch number loa
-000037b0: 6465 6420 6672 6f6d 2074 6865 2063 6865  ded from the che
-000037c0: 636b 706f 696e 742e 0d0a 2020 2020 2020  ckpoint...      
-000037d0: 2020 2222 220d 0a20 2020 2020 2020 2070    """..        p
-000037e0: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-000037f0: 696e 2873 656c 662e 6366 672e 4348 4543  in(self.cfg.CHEC
-00003800: 4b50 4f49 4e54 5f50 4154 482c 2073 656c  KPOINT_PATH, sel
-00003810: 662e 6366 672e 4348 4543 4b50 4f49 4e54  f.cfg.CHECKPOINT
-00003820: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
-00003830: 2020 2020 6368 6563 6b70 6f69 6e74 203d      checkpoint =
-00003840: 2074 6f72 6368 2e6c 6f61 6428 7061 7468   torch.load(path
-00003850: 290d 0a20 2020 2020 2020 2066 6f72 206d  )..        for m
-00003860: 6f64 756c 6520 696e 2073 656c 662e 6366  odule in self.cf
-00003870: 672e 4348 4543 4b50 4f49 4e54 5f4d 4f44  g.CHECKPOINT_MOD
-00003880: 554c 4553 3a0d 0a20 2020 2020 2020 2020  ULES:..         
-00003890: 2020 2067 6574 6174 7472 2873 656c 662c     getattr(self,
-000038a0: 206d 6f64 756c 6529 2e6c 6f61 645f 7374   module).load_st
-000038b0: 6174 655f 6469 6374 2863 6865 636b 706f  ate_dict(checkpo
-000038c0: 696e 745b 6d6f 6475 6c65 5d29 0d0a 2020  int[module])..  
-000038d0: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
-000038e0: 6f72 732e 6c6f 6164 5f73 7461 7465 5f64  ors.load_state_d
-000038f0: 6963 7428 6368 6563 6b70 6f69 6e74 5b27  ict(checkpoint['
-00003900: 6d6f 6e69 746f 7273 275d 290d 0a20 2020  monitors'])..   
-00003910: 2020 2020 2072 6574 7572 6e20 6368 6563       return chec
-00003920: 6b70 6f69 6e74 5b27 6570 6f63 6827 5d0d  kpoint['epoch'].
-00003930: 0a0d 0a20 2020 2064 6566 2073 6176 655f  ...    def save_
-00003940: 6265 7374 2873 656c 6629 202d 3e20 4e6f  best(self) -> No
-00003950: 6e65 3a0d 0a20 2020 2020 2020 2074 6f72  ne:..        tor
-00003960: 6368 2e73 6176 6528 7365 6c66 2e6d 6f64  ch.save(self.mod
-00003970: 656c 2e73 7461 7465 5f64 6963 7428 292c  el.state_dict(),
-00003980: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00003990: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
-000039a0: 2073 656c 662e 6366 672e 4245 5354 5f46   self.cfg.BEST_F
-000039b0: 494c 454e 414d 4529 290d 0a0d 0a20 2020  ILENAME))....   
-000039c0: 2064 6566 206c 6f61 645f 6265 7374 2873   def load_best(s
-000039d0: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
-000039e0: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
-000039f0: 7228 6622 5b43 6f61 6368 5d20 3e3e 3e20  r(f"[Coach] >>> 
-00003a00: 4c6f 6164 2062 6573 7420 6d6f 6465 6c20  Load best model 
-00003a10: 4045 706f 6368 207b 7365 6c66 2e5f 6265  @Epoch {self._be
-00003a20: 7374 5f65 706f 6368 3a3c 3464 7d20 2229  st_epoch:<4d} ")
-00003a30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00003a40: 6f64 656c 2e6c 6f61 645f 7374 6174 655f  odel.load_state_
-00003a50: 6469 6374 2874 6f72 6368 2e6c 6f61 6428  dict(torch.load(
-00003a60: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00003a70: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00003a80: 7365 6c66 2e63 6667 2e42 4553 545f 4649  self.cfg.BEST_FI
-00003a90: 4c45 4e41 4d45 2929 290d 0a0d 0a20 2020  LENAME)))....   
-00003aa0: 2064 6566 2063 6865 636b 5f62 6573 7428   def check_best(
-00003ab0: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
-00003ac0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00003ad0: 2020 2020 2222 2255 7064 6174 6520 6265      """Update be
-00003ae0: 7374 2076 616c 7565 2e22 2222 0d0a 2020  st value."""..  
-00003af0: 2020 2020 2020 6966 2073 656c 662e 6d65        if self.me
-00003b00: 7465 7234 6265 7374 2e61 6374 6976 653a  ter4best.active:
-00003b10: 0d0a 2020 2020 2020 2020 2020 2020 6265  ..            be
-00003b20: 7374 5f20 3d20 7365 6c66 2e6d 6574 6572  st_ = self.meter
-00003b30: 3462 6573 742e 7768 6963 685f 6973 5f62  4best.which_is_b
-00003b40: 6574 7465 7228 7365 6c66 2e5f 6265 7374  etter(self._best
-00003b50: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00003b60: 6620 6265 7374 5f20 213d 2073 656c 662e  f best_ != self.
-00003b70: 5f62 6573 743a 0d0a 2020 2020 2020 2020  _best:..        
-00003b80: 2020 2020 2020 2020 7365 6c66 2e5f 6265          self._be
-00003b90: 7374 203d 2062 6573 745f 0d0a 2020 2020  st = best_..    
-00003ba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003bb0: 2e5f 6265 7374 5f65 706f 6368 203d 2065  ._best_epoch = e
-00003bc0: 706f 6368 0d0a 2020 2020 2020 2020 2020  poch..          
-00003bd0: 2020 2020 2020 696e 666f 4c6f 6767 6572        infoLogger
-00003be0: 2866 225b 436f 6163 685d 203e 3e3e 2042  (f"[Coach] >>> B
-00003bf0: 6574 7465 7220 2a2a 2a7b 7365 6c66 2e6d  etter ***{self.m
-00003c00: 6574 6572 3462 6573 742e 6e61 6d65 7d2a  eter4best.name}*
-00003c10: 2a2a 206f 6620 2a2a 2a7b 7365 6c66 2e5f  ** of ***{self._
-00003c20: 6265 7374 3a2e 3466 7d2a 2a2a 2022 290d  best:.4f}*** ").
-00003c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c40: 2073 656c 662e 7361 7665 5f62 6573 7428   self.save_best(
-00003c50: 290d 0a0d 0a20 2020 2064 6566 2065 7661  )....    def eva
-00003c60: 6c5f 6174 5f62 6573 7428 7365 6c66 293a  l_at_best(self):
-00003c70: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00003c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003c90: 2e6c 6f61 645f 6265 7374 2829 0d0a 2020  .load_best()..  
-00003ca0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00003cb0: 616c 6964 2873 656c 662e 5f62 6573 745f  alid(self._best_
-00003cc0: 6570 6f63 6829 0d0a 2020 2020 2020 2020  epoch)..        
-00003cd0: 2020 2020 7365 6c66 2e74 6573 7428 7365      self.test(se
-00003ce0: 6c66 2e5f 6265 7374 5f65 706f 6368 290d  lf._best_epoch).
-00003cf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003d00: 662e 7374 6570 2873 656c 662e 5f62 6573  f.step(self._bes
-00003d10: 745f 6570 6f63 6829 0d0a 2020 2020 2020  t_epoch)..      
-00003d20: 2020 2020 2020 7365 6c66 2e6c 6f61 6428        self.load(
-00003d30: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
-00003d40: 482c 2073 656c 662e 6366 672e 5341 5645  H, self.cfg.SAVE
-00003d50: 445f 4649 4c45 4e41 4d45 290d 0a20 2020  D_FILENAME)..   
-00003d60: 2020 2020 2065 7863 6570 7420 4669 6c65       except File
-00003d70: 4e6f 7446 6f75 6e64 4572 726f 723a 0d0a  NotFoundError:..
-00003d80: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00003d90: 4c6f 6767 6572 2866 225b 436f 6163 685d  Logger(f"[Coach]
-00003da0: 203e 3e3e 204e 6f20 6265 7374 206d 6f64   >>> No best mod
-00003db0: 656c 2077 6173 2072 6563 6f72 6465 642e  el was recorded.
-00003dc0: 2053 6b69 7020 6974 202e 2e2e 2229 0d0a   Skip it ...")..
-00003dd0: 0d0a 2020 2020 6465 6620 7265 7375 6d65  ..    def resume
-00003de0: 2873 656c 6629 202d 3e20 696e 743a 0d0a  (self) -> int:..
-00003df0: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
-00003e00: 2020 2020 2020 5265 7375 6d65 2074 7261        Resume tra
-00003e10: 696e 696e 6720 6672 6f6d 2074 6865 206c  ining from the l
-00003e20: 6173 7420 6368 6563 6b70 6f69 6e74 2e0d  ast checkpoint..
-00003e30: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00003e40: 6e73 3a0d 0a20 2020 2020 2020 202d 2d2d  ns:..        ---
-00003e50: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-00003e60: 7461 7274 5f65 706f 6368 3a20 696e 740d  tart_epoch: int.
-00003e70: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00003e80: 2065 706f 6368 206e 756d 6265 7220 746f   epoch number to
-00003e90: 2072 6573 756d 6520 7472 6169 6e69 6e67   resume training
-00003ea0: 2066 726f 6d2e 0d0a 2020 2020 2020 2020   from...        
-00003eb0: 2222 220d 0a20 2020 2020 2020 2073 7461  """..        sta
-00003ec0: 7274 5f65 706f 6368 3a20 696e 7420 3d20  rt_epoch: int = 
-00003ed0: 300d 0a20 2020 2020 2020 2069 6620 7365  0..        if se
-00003ee0: 6c66 2e63 6667 2e72 6573 756d 653a 0d0a  lf.cfg.resume:..
-00003ef0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00003f00: 745f 6570 6f63 6820 3d20 7365 6c66 2e6c  t_epoch = self.l
-00003f10: 6f61 645f 6368 6563 6b70 6f69 6e74 2829  oad_checkpoint()
-00003f20: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00003f30: 666f 4c6f 6767 6572 2866 225b 436f 6163  foLogger(f"[Coac
-00003f40: 685d 203e 3e3e 204c 6f61 6420 6c61 7374  h] >>> Load last
-00003f50: 2063 6865 636b 706f 696e 7420 616e 6420   checkpoint and 
-00003f60: 7472 6169 6e20 6672 6f6d 2065 706f 6368  train from epoch
-00003f70: 3a20 7b73 7461 7274 5f65 706f 6368 7d22  : {start_epoch}"
-00003f80: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00003f90: 6e20 7374 6172 745f 6570 6f63 680d 0a0d  n start_epoch...
-00003fa0: 0a20 2020 2040 746f 7263 682e 6e6f 5f67  .    @torch.no_g
-00003fb0: 7261 6428 290d 0a20 2020 2064 6566 206d  rad()..    def m
-00003fc0: 6f6e 6974 6f72 280d 0a20 2020 2020 2020  onitor(..       
-00003fd0: 2073 656c 662c 202a 7661 6c75 6573 2c0d   self, *values,.
-00003fe0: 0a20 2020 2020 2020 206e 3a20 696e 7420  .        n: int 
-00003ff0: 3d20 312c 206d 6f64 653a 2073 7472 203d  = 1, mode: str =
-00004000: 2027 6d65 616e 272c 200d 0a20 2020 2020   'mean', ..     
-00004010: 2020 2070 7265 6669 783a 2073 7472 203d     prefix: str =
-00004020: 2027 7472 6169 6e27 2c20 706f 6f6c 3a20   'train', pool: 
-00004030: 4f70 7469 6f6e 616c 5b49 7465 7261 626c  Optional[Iterabl
-00004040: 655d 203d 204e 6f6e 650d 0a20 2020 2029  e] = None..    )
-00004050: 3a0d 0a0d 0a20 2020 2020 2020 2072 2222  :....        r""
-00004060: 220d 0a20 2020 2020 2020 204c 6f67 2064  "..        Log d
-00004070: 6174 6120 7661 6c75 6573 2074 6f20 7370  ata values to sp
-00004080: 6563 6966 6963 206d 6f6e 6974 6f72 732e  ecific monitors.
-00004090: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-000040a0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
-000040b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020   -----------..  
-000040c0: 2020 2020 2020 2a76 616c 7565 7320 3a20        *values : 
-000040d0: 6461 7461 0d0a 2020 2020 2020 2020 2020  data..          
-000040e0: 2020 5468 6520 6461 7461 2076 616c 7565    The data value
-000040f0: 7320 746f 2062 6520 6c6f 6767 6564 2e0d  s to be logged..
-00004100: 0a20 2020 2020 2020 206e 203a 2069 6e74  .        n : int
-00004110: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00004120: 6520 6261 7463 6820 7369 7a65 2069 6e20  e batch size in 
-00004130: 6765 6e65 7261 6c2e 0d0a 2020 2020 2020  general...      
-00004140: 2020 6d6f 6465 203a 2073 7472 2c20 6f70    mode : str, op
-00004150: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00004160: 2020 2020 5468 6520 6d6f 6465 2074 6f20      The mode to 
-00004170: 636f 6d70 7574 6520 7468 6520 6d65 7472  compute the metr
-00004180: 6963 2e20 4361 6e20 6265 2027 7375 6d27  ic. Can be 'sum'
-00004190: 206f 7220 276d 6561 6e27 2028 6465 6661   or 'mean' (defa
-000041a0: 756c 7429 2e0d 0a20 2020 2020 2020 2070  ult)...        p
-000041b0: 7265 6669 7820 3a20 7374 722c 206f 7074  refix : str, opt
-000041c0: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-000041d0: 2020 2054 6865 2070 7265 6669 7820 7374     The prefix st
-000041e0: 7269 6e67 2069 6e64 6963 6174 696e 6720  ring indicating 
-000041f0: 7768 6963 6820 6d6f 6465 2074 6865 2076  which mode the v
-00004200: 616c 7565 7320 6265 6c6f 6e67 2074 6f2e  alues belong to.
-00004210: 2043 616e 2062 6520 2774 7261 696e 272c   Can be 'train',
-00004220: 2027 7465 7374 2720 6f72 2027 7661 6c69   'test' or 'vali
-00004230: 6427 2e0d 0a20 2020 2020 2020 2070 6f6f  d'...        poo
-00004240: 6c20 3a20 4c69 7374 5b73 7472 5d2c 206f  l : List[str], o
-00004250: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00004260: 2020 2020 2041 206c 6973 7420 6f66 206d       A list of m
-00004270: 6574 7269 6320 6e61 6d65 7320 746f 206c  etric names to l
-00004280: 6f67 2e20 4966 204e 6f6e 652c 2061 6c6c  og. If None, all
-00004290: 206d 6574 7269 6373 2069 6e20 7468 6520   metrics in the 
-000042a0: 706f 6f6c 206f 6620 6070 7265 6669 7860  pool of `prefix`
-000042b0: 2077 696c 6c20 6265 206c 6f67 6765 642e   will be logged.
-000042c0: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-000042d0: 0a20 2020 2020 2020 206d 6574 7269 6373  .        metrics
-000042e0: 3a20 4469 6374 5b4c 6973 745d 203d 2073  : Dict[List] = s
-000042f0: 656c 662e 6d6f 6e69 746f 7273 5b70 7265  elf.monitors[pre
-00004300: 6669 785d 0d0a 2020 2020 2020 2020 706f  fix]..        po
-00004310: 6f6c 203d 206d 6574 7269 6373 2069 6620  ol = metrics if 
-00004320: 706f 6f6c 2069 7320 4e6f 6e65 2065 6c73  pool is None els
-00004330: 6520 706f 6f6c 0d0a 2020 2020 2020 2020  e pool..        
-00004340: 666f 7220 6c61 7374 6e61 6d65 2069 6e20  for lastname in 
-00004350: 706f 6f6c 3a0d 0a20 2020 2020 2020 2020  pool:..         
-00004360: 2020 2066 6f72 206d 6574 6572 2069 6e20     for meter in 
-00004370: 6d65 7472 6963 732e 6765 7428 6c61 7374  metrics.get(last
-00004380: 6e61 6d65 2e75 7070 6572 2829 2c20 5b5d  name.upper(), []
-00004390: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000043a0: 2020 2020 6d65 7465 7228 2a76 616c 7565      meter(*value
-000043b0: 732c 206e 3d6e 2c20 6d6f 6465 3d6d 6f64  s, n=n, mode=mod
-000043c0: 6529 0d0a 0d0a 2020 2020 6465 6620 7374  e)....    def st
-000043d0: 6570 2873 656c 662c 2065 706f 6368 3a20  ep(self, epoch: 
-000043e0: 696e 7429 3a0d 0a20 2020 2020 2020 2072  int):..        r
-000043f0: 2222 220d 0a20 2020 2020 2020 2050 7269  """..        Pri
-00004400: 6e74 7320 7472 6169 6e69 6e67 2073 7461  nts training sta
-00004410: 7475 7320 616e 6420 6576 616c 7561 7469  tus and evaluati
-00004420: 6f6e 2072 6573 756c 7473 2066 6f72 2065  on results for e
-00004430: 6163 6820 6570 6f63 682c 200d 0a20 2020  ach epoch, ..   
-00004440: 2020 2020 2061 6e64 2072 6573 6574 7320       and resets 
-00004450: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-00004460: 6720 6041 7665 7261 6765 4d65 7465 7260  g `AverageMeter`
-00004470: 2069 6e73 7461 6e63 6573 2e0d 0a0d 0a20   instances..... 
-00004480: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00004490: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-000044a0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000044b0: 2065 706f 6368 203a 2069 6e74 0d0a 2020   epoch : int..  
-000044c0: 2020 2020 2020 2020 2020 5468 6520 6570            The ep
-000044d0: 6f63 6820 6e75 6d62 6572 2e0d 0a0d 0a20  och number..... 
-000044e0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-000044f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00004500: 2d0d 0a20 2020 2020 2020 204e 6f6e 650d  -..        None.
-00004510: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00004520: 2020 2020 2020 6d65 7472 6963 733a 2044        metrics: D
-00004530: 6963 745b 7374 722c 204c 6973 745b 4176  ict[str, List[Av
-00004540: 6572 6167 654d 6574 6572 5d5d 0d0a 2020  erageMeter]]..  
-00004550: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
-00004560: 2c20 6d65 7472 6963 7320 696e 2073 656c  , metrics in sel
-00004570: 662e 6d6f 6e69 746f 7273 2e69 7465 6d73  f.monitors.items
-00004580: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00004590: 2069 6e66 6f73 203d 205b 6622 5b43 6f61   infos = [f"[Coa
-000045a0: 6368 5d20 3e3e 3e20 7b70 7265 6669 782e  ch] >>> {prefix.
-000045b0: 7570 7065 7228 293a 357d 2040 4570 6f63  upper():5} @Epoc
-000045c0: 683a 207b 6570 6f63 683a 3c34 647d 203e  h: {epoch:<4d} >
-000045d0: 3e3e 2022 5d0d 0a20 2020 2020 2020 2020  >> "]..         
-000045e0: 2020 2066 6f72 206d 6574 6572 7320 696e     for meters in
-000045f0: 206d 6574 7269 6373 2e76 616c 7565 7328   metrics.values(
-00004600: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004610: 2020 2020 696e 666f 7320 2b3d 205b 6d65      infos += [me
-00004620: 7465 722e 7374 6570 2829 2066 6f72 206d  ter.step() for m
-00004630: 6574 6572 2069 6e20 6d65 7465 7273 2069  eter in meters i
-00004640: 6620 6d65 7465 722e 6163 7469 7665 5d0d  f meter.active].
-00004650: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
-00004660: 6f4c 6f67 6765 7228 2720 7c7c 2027 2e6a  oLogger(' || '.j
-00004670: 6f69 6e28 696e 666f 7329 290d 0a0d 0a20  oin(infos)).... 
-00004680: 2020 2040 7469 6d65 6d65 7465 7228 2243     @timemeter("C
-00004690: 6f61 6368 2f73 756d 6d61 7279 2229 0d0a  oach/summary")..
-000046a0: 2020 2020 6465 6620 7375 6d6d 6172 7928      def summary(
-000046b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000046c0: 7222 2222 0d0a 2020 2020 2020 2020 5375  r"""..        Su
-000046d0: 6d6d 6172 7920 7468 6520 7768 6f6c 6520  mmary the whole 
-000046e0: 7472 6169 6e69 6e67 2070 726f 6365 7373  training process
-000046f0: 2e0d 0a0d 0a20 2020 2020 2020 2047 656e  .....        Gen
-00004700: 6572 6174 6520 6120 7375 6d6d 6172 7920  erate a summary 
-00004710: 6f66 2074 6865 2065 6e74 6972 6520 7472  of the entire tr
-00004720: 6169 6e69 6e67 2070 726f 6365 7373 2c20  aining process, 
-00004730: 696e 636c 7564 696e 6720 7468 6520 6869  including the hi
-00004740: 7374 6f72 6963 616c 2065 7661 6c75 6174  storical evaluat
-00004750: 696f 6e20 7265 7375 6c74 732c 2074 6865  ion results, the
-00004760: 2062 6573 740d 0a20 2020 2020 2020 2068   best..        h
-00004770: 6973 746f 7269 6361 6c20 7265 7375 6c74  istorical result
-00004780: 732c 2061 6e64 2074 6865 2063 7572 7665  s, and the curve
-00004790: 7320 6f66 2068 6973 746f 7269 6361 6c20  s of historical 
-000047a0: 7265 7375 6c74 732e 2054 6865 2072 6573  results. The res
-000047b0: 756c 7469 6e67 2073 756d 6d61 7279 2069  ulting summary i
-000047c0: 7320 7361 7665 6420 746f 2061 204d 6172  s saved to a Mar
-000047d0: 6b64 6f77 6e20 6669 6c65 206e 616d 6564  kdown file named
-000047e0: 0d0a 2020 2020 2020 2020 2253 756d 6d61  ..        "Summa
-000047f0: 7279 2e6d 6422 2069 6e20 7468 6520 6073  ry.md" in the `s
-00004800: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00004810: 6020 6469 7265 6374 6f72 792e 0d0a 0d0a  ` directory.....
-00004820: 2020 2020 2020 2020 4164 6469 7469 6f6e          Addition
-00004830: 616c 6c79 2c20 7468 6520 6265 7374 2068  ally, the best h
-00004840: 6973 746f 7269 6361 6c20 7265 7375 6c74  istorical result
-00004850: 7320 6172 6520 7361 7665 6420 746f 2061  s are saved to a
-00004860: 2062 696e 6172 7920 6669 6c65 206e 616d   binary file nam
-00004870: 6564 2060 7365 6c66 2e63 6667 2e4d 4f4e  ed `self.cfg.MON
-00004880: 4954 4f52 5f42 4553 545f 4649 4c45 4e41  ITOR_BEST_FILENA
-00004890: 4d45 602e 0d0a 2020 2020 2020 2020 2222  ME`...        ""
-000048a0: 220d 0a20 2020 2020 2020 2073 203d 2022  "..        s = "
-000048b0: 7c20 207b 7072 6566 6978 7d20 207c 2020  |  {prefix}  |  
-000048c0: 207b 6e61 6d65 7d20 2020 7c20 2020 7b76   {name}   |   {v
-000048d0: 616c 7d20 2020 7c20 2020 7b65 706f 6368  al}   |   {epoch
-000048e0: 7d20 2020 7c20 2020 7b69 6d67 7d20 2020  }   |   {img}   
-000048f0: 7c5c 6e22 0d0a 2020 2020 2020 2020 696e  |\n"..        in
-00004900: 666f 203d 2022 220d 0a20 2020 2020 2020  fo = ""..       
-00004910: 2069 6e66 6f20 2b3d 2022 7c20 2050 7265   info += "|  Pre
-00004920: 6669 7820 207c 2020 204d 6574 7269 6320  fix  |   Metric 
-00004930: 2020 7c20 2020 4265 7374 2020 207c 2020    |   Best   |  
-00004940: 2040 4570 6f63 6820 2020 7c20 2020 496d   @Epoch   |   Im
-00004950: 6720 2020 7c5c 6e22 0d0a 2020 2020 2020  g   |\n"..      
-00004960: 2020 696e 666f 202b 3d20 227c 203a 2d2d    info += "| :--
-00004970: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+000030b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000030c0: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
+000030d0: 616d 6520 3d20 6e61 6d65 0d0a 2020 2020  ame = name..    
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 6d65 7465 7220 3d20 7365 745f 6d6f 6e69  meter = set_moni
+00003100: 746f 7228 0d0a 2020 2020 2020 2020 2020  tor(..          
+00003110: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00003120: 6d65 3d6e 616d 652c 0d0a 2020 2020 2020  me=name,..      
+00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003140: 2020 6c61 7374 6e61 6d65 3d6c 6173 746e    lastname=lastn
+00003150: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
+00003160: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00003170: 6566 6978 3d70 7265 6669 780d 0a20 2020  efix=prefix..   
+00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003190: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000031a0: 2020 2020 6966 2070 7265 6669 7820 3d3d      if prefix ==
+000031b0: 2027 7661 6c69 6427 2061 6e64 206e 616d   'valid' and nam
+000031c0: 6520 3d3d 2077 6869 6368 3462 6573 743a  e == which4best:
+000031d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000031e0: 2020 2020 2020 7365 6c66 2e6d 6574 6572        self.meter
+000031f0: 3462 6573 7420 3d20 6d65 7465 720d 0a20  4best = meter.. 
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2073 656c 662e 5f62 6573 7420 3d20     self._best = 
+00003220: 2d66 6c6f 6174 2827 696e 6627 2920 6966  -float('inf') if
+00003230: 206d 6574 6572 2e63 6173 7465 7220 6973   meter.caster is
+00003240: 206d 6178 2065 6c73 6520 666c 6f61 7428   max else float(
+00003250: 2769 6e66 2729 0d0a 2020 2020 2020 2020  'inf')..        
+00003260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003270: 2e5f 6265 7374 5f65 706f 6368 203d 2030  ._best_epoch = 0
+00003280: 0d0a 0d0a 2020 2020 2020 2020 2320 5072  ....        # Pr
+00003290: 6570 6172 6520 6461 7461 206c 6f61 6465  epare data loade
+000032a0: 7273 0d0a 2020 2020 2020 2020 7365 6c66  rs..        self
+000032b0: 2e70 7265 7061 7265 5f64 6174 616c 6f61  .prepare_dataloa
+000032c0: 6465 7228 290d 0a0d 0a20 2020 2064 6566  der()....    def
+000032d0: 2073 6176 6528 7365 6c66 2920 2d3e 204e   save(self) -> N
+000032e0: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
+000032f0: 2253 6176 6520 7468 6520 6d6f 6465 6c22  "Save the model"
+00003300: 2222 0d0a 2020 2020 2020 2020 746f 7263  ""..        torc
+00003310: 682e 7361 7665 2873 656c 662e 6d6f 6465  h.save(self.mode
+00003320: 6c2e 7374 6174 655f 6469 6374 2829 2c20  l.state_dict(), 
+00003330: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
+00003340: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
+00003350: 7365 6c66 2e63 6667 2e53 4156 4544 5f46  self.cfg.SAVED_F
+00003360: 494c 454e 414d 4529 290d 0a0d 0a20 2020  ILENAME))....   
+00003370: 2064 6566 206c 6f61 6428 7365 6c66 2c20   def load(self, 
+00003380: 7061 7468 3a20 7374 722c 2066 696c 656e  path: str, filen
+00003390: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+000033a0: 725d 203d 204e 6f6e 652c 202a 2a6b 7761  r] = None, **kwa
+000033b0: 7267 7329 202d 3e20 4e6f 6e65 3a0d 0a20  rgs) -> None:.. 
+000033c0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+000033d0: 3d20 7365 6c66 2e63 6667 2e53 4156 4544  = self.cfg.SAVED
+000033e0: 5f46 494c 454e 414d 4520 6966 2066 696c  _FILENAME if fil
+000033f0: 656e 616d 6520 6973 204e 6f6e 6520 656c  ename is None el
+00003400: 7365 2066 696c 656e 616d 650d 0a20 2020  se filename..   
+00003410: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
+00003420: 6c6f 6164 5f73 7461 7465 5f64 6963 7428  load_state_dict(
+00003430: 746f 7263 682e 6c6f 6164 286f 732e 7061  torch.load(os.pa
+00003440: 7468 2e6a 6f69 6e28 7061 7468 2c20 6669  th.join(path, fi
+00003450: 6c65 6e61 6d65 292c 202a 2a6b 7761 7267  lename), **kwarg
+00003460: 7329 290d 0a0d 0a20 2020 2064 6566 2073  s))....    def s
+00003470: 6176 655f 6368 6563 6b70 6f69 6e74 2873  ave_checkpoint(s
+00003480: 656c 662c 2065 706f 6368 3a20 696e 7429  elf, epoch: int)
+00003490: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+000034a0: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
+000034b0: 2053 6176 6520 6375 7272 656e 7420 6368   Save current ch
+000034c0: 6563 6b70 6f69 6e74 2061 7420 6570 6f63  eckpoint at epoc
+000034d0: 682e 0d0a 0d0a 2020 2020 2020 2020 5061  h.....        Pa
+000034e0: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
+000034f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a     -----------..
+00003500: 2020 2020 2020 2020 2020 2020 6570 6f63              epoc
+00003510: 6820 3a69 6e74 2043 7572 7265 6e74 2065  h :int Current e
+00003520: 706f 6368 206e 756d 6265 722e 0d0a 0d0a  poch number.....
+00003530: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003540: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00003550: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
+00003560: 4e6f 6e65 0d0a 2020 2020 2020 2020 2222  None..        ""
+00003570: 220d 0a20 2020 2020 2020 2070 6174 6820  "..        path 
+00003580: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+00003590: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
+000035a0: 4e54 5f50 4154 482c 2073 656c 662e 6366  NT_PATH, self.cf
+000035b0: 672e 4348 4543 4b50 4f49 4e54 5f46 494c  g.CHECKPOINT_FIL
+000035c0: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
+000035d0: 6368 6563 6b70 6f69 6e74 203d 2064 6963  checkpoint = dic
+000035e0: 7428 290d 0a20 2020 2020 2020 2063 6865  t()..        che
+000035f0: 636b 706f 696e 745b 2765 706f 6368 275d  ckpoint['epoch']
+00003600: 203d 2065 706f 6368 0d0a 2020 2020 2020   = epoch..      
+00003610: 2020 666f 7220 6d6f 6475 6c65 2069 6e20    for module in 
+00003620: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
+00003630: 494e 545f 4d4f 4455 4c45 533a 0d0a 2020  INT_MODULES:..  
+00003640: 2020 2020 2020 2020 2020 6368 6563 6b70            checkp
+00003650: 6f69 6e74 5b6d 6f64 756c 655d 203d 2067  oint[module] = g
+00003660: 6574 6174 7472 2873 656c 662c 206d 6f64  etattr(self, mod
+00003670: 756c 6529 2e73 7461 7465 5f64 6963 7428  ule).state_dict(
+00003680: 290d 0a20 2020 2020 2020 2063 6865 636b  )..        check
+00003690: 706f 696e 745b 276d 6f6e 6974 6f72 7327  point['monitors'
+000036a0: 5d20 3d20 7365 6c66 2e6d 6f6e 6974 6f72  ] = self.monitor
+000036b0: 732e 7374 6174 655f 6469 6374 2829 0d0a  s.state_dict()..
+000036c0: 2020 2020 2020 2020 746f 7263 682e 7361          torch.sa
+000036d0: 7665 2863 6865 636b 706f 696e 742c 2070  ve(checkpoint, p
+000036e0: 6174 6829 0d0a 0d0a 2020 2020 6465 6620  ath)....    def 
+000036f0: 6c6f 6164 5f63 6865 636b 706f 696e 7428  load_checkpoint(
+00003700: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
+00003710: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
+00003720: 2020 2020 204c 6f61 6420 6c61 7374 2073       Load last s
+00003730: 6176 6564 2063 6865 636b 706f 696e 742e  aved checkpoint.
+00003740: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003750: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
+00003760: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00003770: 6570 6f63 683a 2069 6e74 200d 0a20 2020  epoch: int ..   
+00003780: 2020 2020 2020 2020 2054 6865 2065 706f           The epo
+00003790: 6368 206e 756d 6265 7220 6c6f 6164 6564  ch number loaded
+000037a0: 2066 726f 6d20 7468 6520 6368 6563 6b70   from the checkp
+000037b0: 6f69 6e74 2e0d 0a20 2020 2020 2020 2022  oint...        "
+000037c0: 2222 0d0a 2020 2020 2020 2020 7061 7468  ""..        path
+000037d0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000037e0: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
+000037f0: 494e 545f 5041 5448 2c20 7365 6c66 2e63  INT_PATH, self.c
+00003800: 6667 2e43 4845 434b 504f 494e 545f 4649  fg.CHECKPOINT_FI
+00003810: 4c45 4e41 4d45 290d 0a20 2020 2020 2020  LENAME)..       
+00003820: 2063 6865 636b 706f 696e 7420 3d20 746f   checkpoint = to
+00003830: 7263 682e 6c6f 6164 2870 6174 6829 0d0a  rch.load(path)..
+00003840: 2020 2020 2020 2020 666f 7220 6d6f 6475          for modu
+00003850: 6c65 2069 6e20 7365 6c66 2e63 6667 2e43  le in self.cfg.C
+00003860: 4845 434b 504f 494e 545f 4d4f 4455 4c45  HECKPOINT_MODULE
+00003870: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
+00003880: 6765 7461 7474 7228 7365 6c66 2c20 6d6f  getattr(self, mo
+00003890: 6475 6c65 292e 6c6f 6164 5f73 7461 7465  dule).load_state
+000038a0: 5f64 6963 7428 6368 6563 6b70 6f69 6e74  _dict(checkpoint
+000038b0: 5b6d 6f64 756c 655d 290d 0a20 2020 2020  [module])..     
+000038c0: 2020 2073 656c 662e 6d6f 6e69 746f 7273     self.monitors
+000038d0: 2e6c 6f61 645f 7374 6174 655f 6469 6374  .load_state_dict
+000038e0: 2863 6865 636b 706f 696e 745b 276d 6f6e  (checkpoint['mon
+000038f0: 6974 6f72 7327 5d29 0d0a 2020 2020 2020  itors'])..      
+00003900: 2020 7265 7475 726e 2063 6865 636b 706f    return checkpo
+00003910: 696e 745b 2765 706f 6368 275d 0d0a 0d0a  int['epoch']....
+00003920: 2020 2020 6465 6620 7361 7665 5f62 6573      def save_bes
+00003930: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+00003940: 0d0a 2020 2020 2020 2020 746f 7263 682e  ..        torch.
+00003950: 7361 7665 2873 656c 662e 6d6f 6465 6c2e  save(self.model.
+00003960: 7374 6174 655f 6469 6374 2829 2c20 6f73  state_dict(), os
+00003970: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00003980: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
+00003990: 6c66 2e63 6667 2e42 4553 545f 4649 4c45  lf.cfg.BEST_FILE
+000039a0: 4e41 4d45 2929 0d0a 0d0a 2020 2020 6465  NAME))....    de
+000039b0: 6620 6c6f 6164 5f62 6573 7428 7365 6c66  f load_best(self
+000039c0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+000039d0: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
+000039e0: 225b 436f 6163 685d 203e 3e3e 204c 6f61  "[Coach] >>> Loa
+000039f0: 6420 6265 7374 206d 6f64 656c 2040 4570  d best model @Ep
+00003a00: 6f63 6820 7b73 656c 662e 5f62 6573 745f  och {self._best_
+00003a10: 6570 6f63 683a 3c34 647d 2022 290d 0a20  epoch:<4d} ").. 
+00003a20: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00003a30: 6c2e 6c6f 6164 5f73 7461 7465 5f64 6963  l.load_state_dic
+00003a40: 7428 746f 7263 682e 6c6f 6164 286f 732e  t(torch.load(os.
+00003a50: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
+00003a60: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
+00003a70: 662e 6366 672e 4245 5354 5f46 494c 454e  f.cfg.BEST_FILEN
+00003a80: 414d 4529 2929 0d0a 0d0a 2020 2020 6465  AME)))....    de
+00003a90: 6620 6368 6563 6b5f 6265 7374 2873 656c  f check_best(sel
+00003aa0: 662c 2065 706f 6368 3a20 696e 7429 202d  f, epoch: int) -
+00003ab0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+00003ac0: 2022 2222 5570 6461 7465 2062 6573 7420   """Update best 
+00003ad0: 7661 6c75 652e 2222 220d 0a20 2020 2020  value."""..     
+00003ae0: 2020 2069 6620 7365 6c66 2e6d 6574 6572     if self.meter
+00003af0: 3462 6573 742e 6163 7469 7665 3a0d 0a20  4best.active:.. 
+00003b00: 2020 2020 2020 2020 2020 2062 6573 745f             best_
+00003b10: 203d 2073 656c 662e 6d65 7465 7234 6265   = self.meter4be
+00003b20: 7374 2e77 6869 6368 5f69 735f 6265 7474  st.which_is_bett
+00003b30: 6572 2873 656c 662e 5f62 6573 7429 0d0a  er(self._best)..
+00003b40: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+00003b50: 6573 745f 2021 3d20 7365 6c66 2e5f 6265  est_ != self._be
+00003b60: 7374 3a0d 0a20 2020 2020 2020 2020 2020  st:..           
+00003b70: 2020 2020 2073 656c 662e 5f62 6573 7420       self._best 
+00003b80: 3d20 6265 7374 5f0d 0a20 2020 2020 2020  = best_..       
+00003b90: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+00003ba0: 6573 745f 6570 6f63 6820 3d20 6570 6f63  est_epoch = epoc
+00003bb0: 680d 0a20 2020 2020 2020 2020 2020 2020  h..             
+00003bc0: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+00003bd0: 5b43 6f61 6368 5d20 3e3e 3e20 4265 7474  [Coach] >>> Bett
+00003be0: 6572 202a 2a2a 7b73 656c 662e 6d65 7465  er ***{self.mete
+00003bf0: 7234 6265 7374 2e6e 616d 657d 2a2a 2a20  r4best.name}*** 
+00003c00: 6f66 202a 2a2a 7b73 656c 662e 5f62 6573  of ***{self._bes
+00003c10: 743a 2e34 667d 2a2a 2a20 2229 0d0a 2020  t:.4f}*** ")..  
+00003c20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003c30: 6c66 2e73 6176 655f 6265 7374 2829 0d0a  lf.save_best()..
+00003c40: 0d0a 2020 2020 6465 6620 6576 616c 5f61  ..    def eval_a
+00003c50: 745f 6265 7374 2873 656c 6629 3a0d 0a20  t_best(self):.. 
+00003c60: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00003c70: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00003c80: 6164 5f62 6573 7428 290d 0a20 2020 2020  ad_best()..     
+00003c90: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00003ca0: 6428 7365 6c66 2e5f 6265 7374 5f65 706f  d(self._best_epo
+00003cb0: 6368 290d 0a20 2020 2020 2020 2020 2020  ch)..           
+00003cc0: 2073 656c 662e 7465 7374 2873 656c 662e   self.test(self.
+00003cd0: 5f62 6573 745f 6570 6f63 6829 0d0a 2020  _best_epoch)..  
+00003ce0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00003cf0: 7465 7028 7365 6c66 2e5f 6265 7374 5f65  tep(self._best_e
+00003d00: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
+00003d10: 2020 2073 656c 662e 6c6f 6164 2873 656c     self.load(sel
+00003d20: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
+00003d30: 7365 6c66 2e63 6667 2e53 4156 4544 5f46  self.cfg.SAVED_F
+00003d40: 494c 454e 414d 4529 0d0a 2020 2020 2020  ILENAME)..      
+00003d50: 2020 6578 6365 7074 2046 696c 654e 6f74    except FileNot
+00003d60: 466f 756e 6445 7272 6f72 3a0d 0a20 2020  FoundError:..   
+00003d70: 2020 2020 2020 2020 2069 6e66 6f4c 6f67           infoLog
+00003d80: 6765 7228 6622 5b43 6f61 6368 5d20 3e3e  ger(f"[Coach] >>
+00003d90: 3e20 4e6f 2062 6573 7420 6d6f 6465 6c20  > No best model 
+00003da0: 7761 7320 7265 636f 7264 6564 2e20 536b  was recorded. Sk
+00003db0: 6970 2069 7420 2e2e 2e22 290d 0a0d 0a20  ip it ...").... 
+00003dc0: 2020 2064 6566 2072 6573 756d 6528 7365     def resume(se
+00003dd0: 6c66 2920 2d3e 2069 6e74 3a0d 0a20 2020  lf) -> int:..   
+00003de0: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
+00003df0: 2020 2052 6573 756d 6520 7472 6169 6e69     Resume traini
+00003e00: 6e67 2066 726f 6d20 7468 6520 6c61 7374  ng from the last
+00003e10: 2063 6865 636b 706f 696e 742e 0d0a 0d0a   checkpoint.....
+00003e20: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003e30: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00003e40: 2d2d 0d0a 2020 2020 2020 2020 7374 6172  --..        star
+00003e50: 745f 6570 6f63 683a 2069 6e74 0d0a 2020  t_epoch: int..  
+00003e60: 2020 2020 2020 2020 2020 5468 6520 6570            The ep
+00003e70: 6f63 6820 6e75 6d62 6572 2074 6f20 7265  och number to re
+00003e80: 7375 6d65 2074 7261 696e 696e 6720 6672  sume training fr
+00003e90: 6f6d 2e0d 0a20 2020 2020 2020 2022 2222  om...        """
+00003ea0: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
+00003eb0: 6570 6f63 683a 2069 6e74 203d 2030 0d0a  epoch: int = 0..
+00003ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003ed0: 6366 672e 7265 7375 6d65 3a0d 0a20 2020  cfg.resume:..   
+00003ee0: 2020 2020 2020 2020 2073 7461 7274 5f65           start_e
+00003ef0: 706f 6368 203d 2073 656c 662e 6c6f 6164  poch = self.load
+00003f00: 5f63 6865 636b 706f 696e 7428 290d 0a20  _checkpoint().. 
+00003f10: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
+00003f20: 6f67 6765 7228 6622 5b43 6f61 6368 5d20  ogger(f"[Coach] 
+00003f30: 3e3e 3e20 4c6f 6164 206c 6173 7420 6368  >>> Load last ch
+00003f40: 6563 6b70 6f69 6e74 2061 6e64 2074 7261  eckpoint and tra
+00003f50: 696e 2066 726f 6d20 6570 6f63 683a 207b  in from epoch: {
+00003f60: 7374 6172 745f 6570 6f63 687d 2229 0d0a  start_epoch}")..
+00003f70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003f80: 7461 7274 5f65 706f 6368 0d0a 0d0a 2020  tart_epoch....  
+00003f90: 2020 4074 6f72 6368 2e6e 6f5f 6772 6164    @torch.no_grad
+00003fa0: 2829 0d0a 2020 2020 6465 6620 6d6f 6e69  ()..    def moni
+00003fb0: 746f 7228 0d0a 2020 2020 2020 2020 7365  tor(..        se
+00003fc0: 6c66 2c20 2a76 616c 7565 732c 0d0a 2020  lf, *values,..  
+00003fd0: 2020 2020 2020 6e3a 2069 6e74 203d 2031        n: int = 1
+00003fe0: 2c20 6d6f 6465 3a20 7374 7220 3d20 276d  , mode: str = 'm
+00003ff0: 6561 6e27 2c20 0d0a 2020 2020 2020 2020  ean', ..        
+00004000: 7072 6566 6978 3a20 7374 7220 3d20 2774  prefix: str = 't
+00004010: 7261 696e 272c 2070 6f6f 6c3a 204f 7074  rain', pool: Opt
+00004020: 696f 6e61 6c5b 4974 6572 6162 6c65 5d20  ional[Iterable] 
+00004030: 3d20 4e6f 6e65 0d0a 2020 2020 293a 0d0a  = None..    ):..
+00004040: 0d0a 2020 2020 2020 2020 7222 2222 0d0a  ..        r"""..
+00004050: 2020 2020 2020 2020 4c6f 6720 6461 7461          Log data
+00004060: 2076 616c 7565 7320 746f 2073 7065 6369   values to speci
+00004070: 6669 6320 6d6f 6e69 746f 7273 2e0d 0a0d  fic monitors....
+00004080: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00004090: 6572 733a 0d0a 2020 2020 2020 2020 2d2d  ers:..        --
+000040a0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+000040b0: 2020 202a 7661 6c75 6573 203a 2064 6174     *values : dat
+000040c0: 610d 0a20 2020 2020 2020 2020 2020 2054  a..            T
+000040d0: 6865 2064 6174 6120 7661 6c75 6573 2074  he data values t
+000040e0: 6f20 6265 206c 6f67 6765 642e 0d0a 2020  o be logged...  
+000040f0: 2020 2020 2020 6e20 3a20 696e 740d 0a20        n : int.. 
+00004100: 2020 2020 2020 2020 2020 2054 6865 2062             The b
+00004110: 6174 6368 2073 697a 6520 696e 2067 656e  atch size in gen
+00004120: 6572 616c 2e0d 0a20 2020 2020 2020 206d  eral...        m
+00004130: 6f64 6520 3a20 7374 722c 206f 7074 696f  ode : str, optio
+00004140: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+00004150: 2054 6865 206d 6f64 6520 746f 2063 6f6d   The mode to com
+00004160: 7075 7465 2074 6865 206d 6574 7269 632e  pute the metric.
+00004170: 2043 616e 2062 6520 2773 756d 2720 6f72   Can be 'sum' or
+00004180: 2027 6d65 616e 2720 2864 6566 6175 6c74   'mean' (default
+00004190: 292e 0d0a 2020 2020 2020 2020 7072 6566  )...        pref
+000041a0: 6978 203a 2073 7472 2c20 6f70 7469 6f6e  ix : str, option
+000041b0: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+000041c0: 5468 6520 7072 6566 6978 2073 7472 696e  The prefix strin
+000041d0: 6720 696e 6469 6361 7469 6e67 2077 6869  g indicating whi
+000041e0: 6368 206d 6f64 6520 7468 6520 7661 6c75  ch mode the valu
+000041f0: 6573 2062 656c 6f6e 6720 746f 2e20 4361  es belong to. Ca
+00004200: 6e20 6265 2027 7472 6169 6e27 2c20 2774  n be 'train', 't
+00004210: 6573 7427 206f 7220 2776 616c 6964 272e  est' or 'valid'.
+00004220: 0d0a 2020 2020 2020 2020 706f 6f6c 203a  ..        pool :
+00004230: 204c 6973 745b 7374 725d 2c20 6f70 7469   List[str], opti
+00004240: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+00004250: 2020 4120 6c69 7374 206f 6620 6d65 7472    A list of metr
+00004260: 6963 206e 616d 6573 2074 6f20 6c6f 672e  ic names to log.
+00004270: 2049 6620 4e6f 6e65 2c20 616c 6c20 6d65   If None, all me
+00004280: 7472 6963 7320 696e 2074 6865 2070 6f6f  trics in the poo
+00004290: 6c20 6f66 2060 7072 6566 6978 6020 7769  l of `prefix` wi
+000042a0: 6c6c 2062 6520 6c6f 6767 6564 2e0d 0a20  ll be logged... 
+000042b0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+000042c0: 2020 2020 2020 6d65 7472 6963 733a 2044        metrics: D
+000042d0: 6963 745b 4c69 7374 5d20 3d20 7365 6c66  ict[List] = self
+000042e0: 2e6d 6f6e 6974 6f72 735b 7072 6566 6978  .monitors[prefix
+000042f0: 5d0d 0a20 2020 2020 2020 2070 6f6f 6c20  ]..        pool 
+00004300: 3d20 6d65 7472 6963 7320 6966 2070 6f6f  = metrics if poo
+00004310: 6c20 6973 204e 6f6e 6520 656c 7365 2070  l is None else p
+00004320: 6f6f 6c0d 0a20 2020 2020 2020 2066 6f72  ool..        for
+00004330: 206c 6173 746e 616d 6520 696e 2070 6f6f   lastname in poo
+00004340: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
+00004350: 666f 7220 6d65 7465 7220 696e 206d 6574  for meter in met
+00004360: 7269 6373 2e67 6574 286c 6173 746e 616d  rics.get(lastnam
+00004370: 652e 7570 7065 7228 292c 205b 5d29 3a0d  e.upper(), []):.
+00004380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004390: 206d 6574 6572 282a 7661 6c75 6573 2c20   meter(*values, 
+000043a0: 6e3d 6e2c 206d 6f64 653d 6d6f 6465 290d  n=n, mode=mode).
+000043b0: 0a0d 0a20 2020 2064 6566 2073 7465 7028  ...    def step(
+000043c0: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
+000043d0: 293a 0d0a 2020 2020 2020 2020 7222 2222  ):..        r"""
+000043e0: 0d0a 2020 2020 2020 2020 5072 696e 7473  ..        Prints
+000043f0: 2074 7261 696e 696e 6720 7374 6174 7573   training status
+00004400: 2061 6e64 2065 7661 6c75 6174 696f 6e20   and evaluation 
+00004410: 7265 7375 6c74 7320 666f 7220 6561 6368  results for each
+00004420: 2065 706f 6368 2c20 0d0a 2020 2020 2020   epoch, ..      
+00004430: 2020 616e 6420 7265 7365 7473 2074 6865    and resets the
+00004440: 2063 6f72 7265 7370 6f6e 6469 6e67 2060   corresponding `
+00004450: 4176 6572 6167 654d 6574 6572 6020 696e  AverageMeter` in
+00004460: 7374 616e 6365 732e 0d0a 0d0a 2020 2020  stances.....    
+00004470: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+00004480: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00004490: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6570  ----..        ep
+000044a0: 6f63 6820 3a20 696e 740d 0a20 2020 2020  och : int..     
+000044b0: 2020 2020 2020 2054 6865 2065 706f 6368         The epoch
+000044c0: 206e 756d 6265 722e 0d0a 0d0a 2020 2020   number.....    
+000044d0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+000044e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
+000044f0: 2020 2020 2020 2020 4e6f 6e65 0d0a 2020          None..  
+00004500: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004510: 2020 206d 6574 7269 6373 3a20 4469 6374     metrics: Dict
+00004520: 5b73 7472 2c20 4c69 7374 5b41 7665 7261  [str, List[Avera
+00004530: 6765 4d65 7465 725d 5d0d 0a20 2020 2020  geMeter]]..     
+00004540: 2020 2066 6f72 2070 7265 6669 782c 206d     for prefix, m
+00004550: 6574 7269 6373 2069 6e20 7365 6c66 2e6d  etrics in self.m
+00004560: 6f6e 6974 6f72 732e 6974 656d 7328 293a  onitors.items():
+00004570: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00004580: 666f 7320 3d20 5b66 225b 436f 6163 685d  fos = [f"[Coach]
+00004590: 203e 3e3e 207b 7072 6566 6978 2e75 7070   >>> {prefix.upp
+000045a0: 6572 2829 3a35 7d20 4045 706f 6368 3a20  er():5} @Epoch: 
+000045b0: 7b65 706f 6368 3a3c 3464 7d20 3e3e 3e20  {epoch:<4d} >>> 
+000045c0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+000045d0: 666f 7220 6d65 7465 7273 2069 6e20 6d65  for meters in me
+000045e0: 7472 6963 732e 7661 6c75 6573 2829 3a0d  trics.values():.
+000045f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004600: 2069 6e66 6f73 202b 3d20 5b6d 6574 6572   infos += [meter
+00004610: 2e73 7465 7028 2920 666f 7220 6d65 7465  .step() for mete
+00004620: 7220 696e 206d 6574 6572 7320 6966 206d  r in meters if m
+00004630: 6574 6572 2e61 6374 6976 655d 0d0a 2020  eter.active]..  
+00004640: 2020 2020 2020 2020 2020 696e 666f 4c6f            infoLo
+00004650: 6767 6572 2827 207c 7c20 272e 6a6f 696e  gger(' || '.join
+00004660: 2869 6e66 6f73 2929 0d0a 0d0a 2020 2020  (infos))....    
+00004670: 4074 696d 656d 6574 6572 2822 436f 6163  @timemeter("Coac
+00004680: 682f 7375 6d6d 6172 7922 290d 0a20 2020  h/summary")..   
+00004690: 2064 6566 2073 756d 6d61 7279 2873 656c   def summary(sel
+000046a0: 6629 3a0d 0a20 2020 2020 2020 2072 2222  f):..        r""
+000046b0: 220d 0a20 2020 2020 2020 2053 756d 6d61  "..        Summa
+000046c0: 7279 2074 6865 2077 686f 6c65 2074 7261  ry the whole tra
+000046d0: 696e 696e 6720 7072 6f63 6573 732e 0d0a  ining process...
+000046e0: 0d0a 2020 2020 2020 2020 4765 6e65 7261  ..        Genera
+000046f0: 7465 2061 2073 756d 6d61 7279 206f 6620  te a summary of 
+00004700: 7468 6520 656e 7469 7265 2074 7261 696e  the entire train
+00004710: 696e 6720 7072 6f63 6573 732c 2069 6e63  ing process, inc
+00004720: 6c75 6469 6e67 2074 6865 2068 6973 746f  luding the histo
+00004730: 7269 6361 6c20 6576 616c 7561 7469 6f6e  rical evaluation
+00004740: 2072 6573 756c 7473 2c20 7468 6520 6265   results, the be
+00004750: 7374 0d0a 2020 2020 2020 2020 6869 7374  st..        hist
+00004760: 6f72 6963 616c 2072 6573 756c 7473 2c20  orical results, 
+00004770: 616e 6420 7468 6520 6375 7276 6573 206f  and the curves o
+00004780: 6620 6869 7374 6f72 6963 616c 2072 6573  f historical res
+00004790: 756c 7473 2e20 5468 6520 7265 7375 6c74  ults. The result
+000047a0: 696e 6720 7375 6d6d 6172 7920 6973 2073  ing summary is s
+000047b0: 6176 6564 2074 6f20 6120 4d61 726b 646f  aved to a Markdo
+000047c0: 776e 2066 696c 6520 6e61 6d65 640d 0a20  wn file named.. 
+000047d0: 2020 2020 2020 2022 5375 6d6d 6172 792e         "Summary.
+000047e0: 6d64 2220 696e 2074 6865 2060 7365 6c66  md" in the `self
+000047f0: 2e63 6667 2e4c 4f47 5f50 4154 4860 2064  .cfg.LOG_PATH` d
+00004800: 6972 6563 746f 7279 2e0d 0a0d 0a20 2020  irectory.....   
+00004810: 2020 2020 2041 6464 6974 696f 6e61 6c6c       Additionall
+00004820: 792c 2074 6865 2062 6573 7420 6869 7374  y, the best hist
+00004830: 6f72 6963 616c 2072 6573 756c 7473 2061  orical results a
+00004840: 7265 2073 6176 6564 2074 6f20 6120 6269  re saved to a bi
+00004850: 6e61 7279 2066 696c 6520 6e61 6d65 6420  nary file named 
+00004860: 6073 656c 662e 6366 672e 4d4f 4e49 544f  `self.cfg.MONITO
+00004870: 525f 4245 5354 5f46 494c 454e 414d 4560  R_BEST_FILENAME`
+00004880: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00004890: 2020 2020 2020 2020 696d 706f 7274 2070          import p
+000048a0: 616e 6461 7320 6173 2070 640d 0a0d 0a20  andas as pd.... 
+000048b0: 2020 2020 2020 2073 203d 2022 7c20 207b         s = "|  {
+000048c0: 7072 6566 6978 7d20 207c 2020 207b 6e61  prefix}  |   {na
+000048d0: 6d65 7d20 2020 7c20 2020 7b76 616c 7d20  me}   |   {val} 
+000048e0: 2020 7c20 2020 7b65 706f 6368 7d20 2020    |   {epoch}   
+000048f0: 7c20 2020 7b69 6d67 7d20 2020 7c5c 6e22  |   {img}   |\n"
+00004900: 0d0a 2020 2020 2020 2020 696e 666f 203d  ..        info =
+00004910: 2022 220d 0a20 2020 2020 2020 2069 6e66   ""..        inf
+00004920: 6f20 2b3d 2022 7c20 2050 7265 6669 7820  o += "|  Prefix 
+00004930: 207c 2020 204d 6574 7269 6320 2020 7c20   |   Metric   | 
+00004940: 2020 4265 7374 2020 207c 2020 2040 4570    Best   |   @Ep
+00004950: 6f63 6820 2020 7c20 2020 496d 6720 2020  och   |   Img   
+00004960: 7c5c 6e22 0d0a 2020 2020 2020 2020 696e  |\n"..        in
+00004970: 666f 202b 3d20 227c 203a 2d2d 2d2d 2d2d  fo += "| :------
 00004980: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
 00004990: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
-000049a0: 2d2d 2d2d 2d3a 207c 5c6e 220d 0a20 2020  -----: |\n"..   
-000049b0: 2020 2020 2064 6174 6120 3d20 5b5d 0d0a       data = []..
-000049c0: 2020 2020 2020 2020 6265 7374 203d 2064          best = d
-000049d0: 6566 6175 6c74 6469 6374 2864 6963 7429  efaultdict(dict)
-000049e0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
-000049f0: 7072 6566 6978 2c20 6d65 7472 6963 7320  prefix, metrics 
-00004a00: 696e 2073 656c 662e 6d6f 6e69 746f 7273  in self.monitors
-00004a10: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00004a20: 2020 2020 2020 206d 6574 7269 6373 3a20         metrics: 
-00004a30: 6465 6661 756c 7464 6963 745b 7374 722c  defaultdict[str,
-00004a40: 204c 6973 745b 4176 6572 6167 654d 6574   List[AverageMet
-00004a50: 6572 5d5d 0d0a 2020 2020 2020 2020 2020  er]]..          
-00004a60: 2020 6672 6571 203d 2031 2069 6620 7072    freq = 1 if pr
-00004a70: 6566 6978 203d 3d20 2774 7261 696e 2720  efix == 'train' 
-00004a80: 656c 7365 2073 656c 662e 6366 672e 4556  else self.cfg.EV
-00004a90: 414c 5f46 5245 510d 0a20 2020 2020 2020  AL_FREQ..       
-00004aa0: 2020 2020 2066 6f72 206c 6173 746e 616d       for lastnam
-00004ab0: 652c 206d 6574 6572 7320 696e 206d 6574  e, meters in met
-00004ac0: 7269 6373 2e69 7465 6d73 2829 3a0d 0a20  rics.items():.. 
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004ae0: 6f72 206d 6574 6572 2069 6e20 6d65 7465  or meter in mete
-00004af0: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-00004b00: 2020 2020 2020 2020 2023 2053 6b69 7020           # Skip 
-00004b10: 7468 6f73 6520 6d65 7465 7273 206e 6576  those meters nev
-00004b20: 6572 2061 6374 6976 6174 6564 2e0d 0a20  er activated... 
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2069 6620 6c65 6e28 6d65 7465 722e     if len(meter.
-00004b50: 6869 7374 6f72 7929 203d 3d20 303a 0d0a  history) == 0:..
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00004b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004b90: 2020 2020 2020 6d65 7465 722e 706c 6f74        meter.plot
-00004ba0: 2866 7265 713d 6672 6571 290d 0a20 2020  (freq=freq)..   
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2069 6d67 6e61 6d65 203d 206d 6574 6572   imgname = meter
-00004bd0: 2e73 6176 6528 7061 7468 3d6f 732e 7061  .save(path=os.pa
-00004be0: 7468 2e6a 6f69 6e28 7365 6c66 2e63 6667  th.join(self.cfg
-00004bf0: 2e4c 4f47 5f50 4154 482c 2073 656c 662e  .LOG_PATH, self.
-00004c00: 6366 672e 5355 4d4d 4152 595f 4449 5229  cfg.SUMMARY_DIR)
-00004c10: 2c20 7072 6566 6978 3d70 7265 6669 7829  , prefix=prefix)
-00004c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004c30: 2020 2020 2020 6570 6f63 682c 2076 616c        epoch, val
-00004c40: 203d 206d 6574 6572 2e61 7267 6265 7374   = meter.argbest
-00004c50: 2866 7265 7129 0d0a 2020 2020 2020 2020  (freq)..        
-00004c60: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00004c70: 202b 3d20 732e 666f 726d 6174 280d 0a20   += s.format(.. 
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2070 7265 6669 783d 7072         prefix=pr
-00004ca0: 6566 6978 2c20 6e61 6d65 3d6d 6574 6572  efix, name=meter
-00004cb0: 2e6e 616d 652c 0d0a 2020 2020 2020 2020  .name,..        
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 7661 6c3d 7661 6c2c 2065 706f 6368 3d65  val=val, epoch=e
-00004ce0: 706f 6368 2c20 696d 673d 6622 215b 5d28  poch, img=f"![](
-00004cf0: 7b69 6d67 6e61 6d65 7d29 220d 0a20 2020  {imgname})"..   
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00004d20: 2020 2020 2020 2020 6461 7461 2e61 7070          data.app
-00004d30: 656e 6428 5b70 7265 6669 782c 206d 6574  end([prefix, met
-00004d40: 6572 2e6e 616d 652c 2076 616c 2c20 6570  er.name, val, ep
-00004d50: 6f63 685d 290d 0a20 2020 2020 2020 2020  och])..         
-00004d60: 2020 2020 2020 2020 2020 2069 6620 7661             if va
-00004d70: 6c20 213d 202d 313a 2023 204f 6e6c 7920  l != -1: # Only 
-00004d80: 7361 7665 2061 7661 696c 6162 6c65 2064  save available d
-00004d90: 6174 612e 0d0a 2020 2020 2020 2020 2020  ata...          
-00004da0: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00004db0: 7374 5b70 7265 6669 785d 5b6d 6574 6572  st[prefix][meter
-00004dc0: 2e6e 616d 655d 203d 2076 616c 0d0a 0d0a  .name] = val....
-00004dd0: 2020 2020 2020 2020 6669 6c65 5f20 3d20          file_ = 
-00004de0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00004df0: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00004e00: 7365 6c66 2e63 6667 2e53 554d 4d41 5259  self.cfg.SUMMARY
-00004e10: 5f44 4952 2c20 7365 6c66 2e63 6667 2e53  _DIR, self.cfg.S
-00004e20: 554d 4d41 5259 5f46 494c 454e 414d 4529  UMMARY_FILENAME)
-00004e30: 0d0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
-00004e40: 7065 6e28 6669 6c65 5f2c 2022 7722 2c20  pen(file_, "w", 
-00004e50: 656e 636f 6469 6e67 3d22 7574 6638 2229  encoding="utf8")
-00004e60: 2061 7320 6668 3a0d 0a20 2020 2020 2020   as fh:..       
-00004e70: 2020 2020 2066 682e 7772 6974 6528 696e       fh.write(in
-00004e80: 666f 290d 0a0d 0a20 2020 2020 2020 2064  fo)....        d
-00004e90: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
-00004ea0: 2864 6174 612c 2063 6f6c 756d 6e73 3d5b  (data, columns=[
-00004eb0: 2750 7265 6669 7827 2c20 274d 6574 7269  'Prefix', 'Metri
-00004ec0: 6327 2c20 2742 6573 7427 2c20 2740 4570  c', 'Best', '@Ep
-00004ed0: 6f63 6827 5d29 0d0a 2020 2020 2020 2020  och'])..        
-00004ee0: 696e 666f 4c6f 6767 6572 2873 7472 2864  infoLogger(str(d
-00004ef0: 6629 290d 0a20 2020 2020 2020 2069 6e66  f))..        inf
-00004f00: 6f4c 6f67 6765 7228 6622 5b4c 6f47 5f50  oLogger(f"[LoG_P
-00004f10: 6154 485d 203e 3e3e 207b 7365 6c66 2e63  aTH] >>> {self.c
-00004f20: 6667 2e4c 4f47 5f50 4154 487d 2229 0d0a  fg.LOG_PATH}")..
-00004f30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00004f40: 6f6e 6974 6f72 732e 7772 6974 6528 6f73  onitors.write(os
-00004f50: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00004f60: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
-00004f70: 6c66 2e63 6667 2e53 554d 4d41 5259 5f44  lf.cfg.SUMMARY_D
-00004f80: 4952 2929 2023 2074 656e 736f 7262 6f61  IR)) # tensorboa
-00004f90: 7264 0d0a 0d0a 2020 2020 2020 2020 7365  rd....        se
-00004fa0: 6c66 2e6d 6f6e 6974 6f72 732e 7361 7665  lf.monitors.save
-00004fb0: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-00004fc0: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
-00004fd0: 2073 656c 662e 6366 672e 4441 5441 5f44   self.cfg.DATA_D
-00004fe0: 4952 292c 2073 656c 662e 6366 672e 4d4f  IR), self.cfg.MO
-00004ff0: 4e49 544f 525f 4649 4c45 4e41 4d45 290d  NITOR_FILENAME).
-00005000: 0a20 2020 2020 2020 2065 7870 6f72 745f  .        export_
-00005010: 7069 636b 6c65 2862 6573 742c 206f 732e  pickle(best, os.
-00005020: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00005030: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
-00005040: 662e 6366 672e 4441 5441 5f44 4952 2c20  f.cfg.DATA_DIR, 
-00005050: 7365 6c66 2e63 6667 2e4d 4f4e 4954 4f52  self.cfg.MONITOR
-00005060: 5f42 4553 545f 4649 4c45 4e41 4d45 2929  _BEST_FILENAME))
-00005070: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00005080: 0d0a 2020 2020 4074 696d 656d 6574 6572  ..    @timemeter
-00005090: 2822 436f 6163 682f 6669 7422 290d 0a20  ("Coach/fit").. 
-000050a0: 2020 2064 6566 2066 6974 2873 656c 6629     def fit(self)
-000050b0: 3a0d 0a0d 0a20 2020 2020 2020 2064 6566  :....        def
-000050c0: 2073 6967 6e61 6c5f 6861 6e64 6c65 7228   signal_handler(
-000050d0: 7369 672c 2066 7261 6d65 293a 0d0a 2020  sig, frame):..  
-000050e0: 2020 2020 2020 2020 2020 696e 666f 4c6f            infoLo
-000050f0: 6767 6572 2866 225c 3033 335b 303b 3331  gger(f"\033[0;31
-00005100: 3b34 376d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ;47m============
+000049a0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+000049b0: 2d3a 207c 5c6e 220d 0a20 2020 2020 2020  -: |\n"..       
+000049c0: 2064 6174 6120 3d20 5b5d 0d0a 2020 2020   data = []..    
+000049d0: 2020 2020 6265 7374 203d 2064 6566 6175      best = defau
+000049e0: 6c74 6469 6374 2864 6963 7429 0d0a 0d0a  ltdict(dict)....
+000049f0: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
+00004a00: 6978 2c20 6d65 7472 6963 7320 696e 2073  ix, metrics in s
+00004a10: 656c 662e 6d6f 6e69 746f 7273 2e69 7465  elf.monitors.ite
+00004a20: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00004a30: 2020 206d 6574 7269 6373 3a20 6465 6661     metrics: defa
+00004a40: 756c 7464 6963 745b 7374 722c 204c 6973  ultdict[str, Lis
+00004a50: 745b 4176 6572 6167 654d 6574 6572 5d5d  t[AverageMeter]]
+00004a60: 0d0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
+00004a70: 6571 203d 2031 2069 6620 7072 6566 6978  eq = 1 if prefix
+00004a80: 203d 3d20 2774 7261 696e 2720 656c 7365   == 'train' else
+00004a90: 2073 656c 662e 6366 672e 4556 414c 5f46   self.cfg.EVAL_F
+00004aa0: 5245 510d 0a20 2020 2020 2020 2020 2020  REQ..           
+00004ab0: 2066 6f72 206c 6173 746e 616d 652c 206d   for lastname, m
+00004ac0: 6574 6572 7320 696e 206d 6574 7269 6373  eters in metrics
+00004ad0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00004ae0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+00004af0: 6574 6572 2069 6e20 6d65 7465 7273 3a0d  eter in meters:.
+00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b10: 2020 2020 2023 2053 6b69 7020 7468 6f73       # Skip thos
+00004b20: 6520 6d65 7465 7273 206e 6576 6572 2061  e meters never a
+00004b30: 6374 6976 6174 6564 2e0d 0a20 2020 2020  ctivated...     
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004b50: 6620 6c65 6e28 6d65 7465 722e 6869 7374  f len(meter.hist
+00004b60: 6f72 7929 203d 3d20 303a 0d0a 2020 2020  ory) == 0:..    
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b80: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 6d65 7465 722e 706c 6f74 2866 7265    meter.plot(fre
+00004bb0: 713d 6672 6571 290d 0a20 2020 2020 2020  q=freq)..       
+00004bc0: 2020 2020 2020 2020 2020 2020 2069 6d67               img
+00004bd0: 6e61 6d65 203d 206d 6574 6572 2e73 6176  name = meter.sav
+00004be0: 6528 7061 7468 3d6f 732e 7061 7468 2e6a  e(path=os.path.j
+00004bf0: 6f69 6e28 7365 6c66 2e63 6667 2e4c 4f47  oin(self.cfg.LOG
+00004c00: 5f50 4154 482c 2073 656c 662e 6366 672e  _PATH, self.cfg.
+00004c10: 5355 4d4d 4152 595f 4449 5229 2c20 7072  SUMMARY_DIR), pr
+00004c20: 6566 6978 3d70 7265 6669 7829 0d0a 2020  efix=prefix)..  
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 6570 6f63 682c 2076 616c 203d 206d    epoch, val = m
+00004c50: 6574 6572 2e61 7267 6265 7374 2866 7265  eter.argbest(fre
+00004c60: 7129 0d0a 2020 2020 2020 2020 2020 2020  q)..            
+00004c70: 2020 2020 2020 2020 696e 666f 202b 3d20          info += 
+00004c80: 732e 666f 726d 6174 280d 0a20 2020 2020  s.format(..     
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2070 7265 6669 783d 7072 6566 6978     prefix=prefix
+00004cb0: 2c20 6e61 6d65 3d6d 6574 6572 2e6e 616d  , name=meter.nam
+00004cc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004cd0: 2020 2020 2020 2020 2020 2020 7661 6c3d              val=
+00004ce0: 7661 6c2c 2065 706f 6368 3d65 706f 6368  val, epoch=epoch
+00004cf0: 2c20 696d 673d 6622 215b 5d28 7b69 6d67  , img=f"![]({img
+00004d00: 6e61 6d65 7d29 220d 0a20 2020 2020 2020  name})"..       
+00004d10: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 2020 2020 6461 7461 2e61 7070 656e 6428      data.append(
+00004d40: 5b70 7265 6669 782c 206d 6574 6572 2e6e  [prefix, meter.n
+00004d50: 616d 652c 2076 616c 2c20 6570 6f63 685d  ame, val, epoch]
+00004d60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004d70: 2020 2020 2020 2069 6620 7661 6c20 213d         if val !=
+00004d80: 202d 313a 2023 204f 6e6c 7920 7361 7665   -1: # Only save
+00004d90: 2061 7661 696c 6162 6c65 2064 6174 612e   available data.
+00004da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004db0: 2020 2020 2020 2020 2020 6265 7374 5b70            best[p
+00004dc0: 7265 6669 785d 5b6d 6574 6572 2e6e 616d  refix][meter.nam
+00004dd0: 655d 203d 2076 616c 0d0a 0d0a 2020 2020  e] = val....    
+00004de0: 2020 2020 6669 6c65 5f20 3d20 6f73 2e70      file_ = os.p
+00004df0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
+00004e00: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
+00004e10: 2e63 6667 2e53 554d 4d41 5259 5f44 4952  .cfg.SUMMARY_DIR
+00004e20: 2c20 7365 6c66 2e63 6667 2e53 554d 4d41  , self.cfg.SUMMA
+00004e30: 5259 5f46 494c 454e 414d 4529 0d0a 2020  RY_FILENAME)..  
+00004e40: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00004e50: 6669 6c65 5f2c 2022 7722 2c20 656e 636f  file_, "w", enco
+00004e60: 6469 6e67 3d22 7574 6638 2229 2061 7320  ding="utf8") as 
+00004e70: 6668 3a0d 0a20 2020 2020 2020 2020 2020  fh:..           
+00004e80: 2066 682e 7772 6974 6528 696e 666f 290d   fh.write(info).
+00004e90: 0a0d 0a20 2020 2020 2020 2064 6620 3d20  ...        df = 
+00004ea0: 7064 2e44 6174 6146 7261 6d65 2864 6174  pd.DataFrame(dat
+00004eb0: 612c 2063 6f6c 756d 6e73 3d5b 2750 7265  a, columns=['Pre
+00004ec0: 6669 7827 2c20 274d 6574 7269 6327 2c20  fix', 'Metric', 
+00004ed0: 2742 6573 7427 2c20 2740 4570 6f63 6827  'Best', '@Epoch'
+00004ee0: 5d29 0d0a 2020 2020 2020 2020 696e 666f  ])..        info
+00004ef0: 4c6f 6767 6572 2873 7472 2864 6629 290d  Logger(str(df)).
+00004f00: 0a20 2020 2020 2020 2069 6e66 6f4c 6f67  .        infoLog
+00004f10: 6765 7228 6622 5b4c 6f47 5f50 6154 485d  ger(f"[LoG_PaTH]
+00004f20: 203e 3e3e 207b 7365 6c66 2e63 6667 2e4c   >>> {self.cfg.L
+00004f30: 4f47 5f50 4154 487d 2229 0d0a 0d0a 2020  OG_PATH}")....  
+00004f40: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
+00004f50: 6f72 732e 7772 6974 6528 6f73 2e70 6174  ors.write(os.pat
+00004f60: 682e 6a6f 696e 2873 656c 662e 6366 672e  h.join(self.cfg.
+00004f70: 4c4f 475f 5041 5448 2c20 7365 6c66 2e63  LOG_PATH, self.c
+00004f80: 6667 2e53 554d 4d41 5259 5f44 4952 2929  fg.SUMMARY_DIR))
+00004f90: 2023 2074 656e 736f 7262 6f61 7264 0d0a   # tensorboard..
+00004fa0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+00004fb0: 6f6e 6974 6f72 732e 7361 7665 286f 732e  onitors.save(os.
+00004fc0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
+00004fd0: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
+00004fe0: 662e 6366 672e 4441 5441 5f44 4952 292c  f.cfg.DATA_DIR),
+00004ff0: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
+00005000: 525f 4649 4c45 4e41 4d45 290d 0a20 2020  R_FILENAME)..   
+00005010: 2020 2020 2065 7870 6f72 745f 7069 636b       export_pick
+00005020: 6c65 2862 6573 742c 206f 732e 7061 7468  le(best, os.path
+00005030: 2e6a 6f69 6e28 7365 6c66 2e63 6667 2e4c  .join(self.cfg.L
+00005040: 4f47 5f50 4154 482c 2073 656c 662e 6366  OG_PATH, self.cf
+00005050: 672e 4441 5441 5f44 4952 2c20 7365 6c66  g.DATA_DIR, self
+00005060: 2e63 6667 2e4d 4f4e 4954 4f52 5f42 4553  .cfg.MONITOR_BES
+00005070: 545f 4649 4c45 4e41 4d45 2929 0d0a 0d0a  T_FILENAME))....
+00005080: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00005090: 2020 4074 696d 656d 6574 6572 2822 436f    @timemeter("Co
+000050a0: 6163 682f 6669 7422 290d 0a20 2020 2064  ach/fit")..    d
+000050b0: 6566 2066 6974 2873 656c 6629 3a0d 0a0d  ef fit(self):...
+000050c0: 0a20 2020 2020 2020 2064 6566 2073 6967  .        def sig
+000050d0: 6e61 6c5f 6861 6e64 6c65 7228 7369 672c  nal_handler(sig,
+000050e0: 2066 7261 6d65 293a 0d0a 2020 2020 2020   frame):..      
+000050f0: 2020 2020 2020 696e 666f 4c6f 6767 6572        infoLogger
+00005100: 2866 225c 3033 335b 303b 3331 3b34 376d  (f"\033[0;31;47m
 00005110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005120: 3d3d 3d54 4552 4d49 4e41 5445 2043 5552  ===TERMINATE CUR
-00005130: 5245 4e54 2050 524f 4345 5353 3d3d 3d3d  RENT PROCESS====
-00005140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c 3033 335b  ===========\033[
-00005160: 306d 2229 0d0a 2020 2020 2020 2020 2020  0m")..          
-00005170: 2020 7379 732e 6578 6974 2829 0d0a 2020    sys.exit()..  
-00005180: 2020 2020 2020 7369 676e 616c 2e73 6967        signal.sig
-00005190: 6e61 6c28 7369 676e 616c 2e53 4947 494e  nal(signal.SIGIN
-000051a0: 542c 2073 6967 6e61 6c5f 6861 6e64 6c65  T, signal_handle
-000051b0: 7229 0d0a 0d0a 2020 2020 2020 2020 7374  r)....        st
-000051c0: 6172 745f 6570 6f63 6820 3d20 7365 6c66  art_epoch = self
-000051d0: 2e72 6573 756d 6528 290d 0a20 2020 2020  .resume()..     
-000051e0: 2020 2066 6f72 2065 706f 6368 2069 6e20     for epoch in 
-000051f0: 7261 6e67 6528 7374 6172 745f 6570 6f63  range(start_epoc
-00005200: 682c 2073 656c 662e 6366 672e 6570 6f63  h, self.cfg.epoc
-00005210: 6873 293a 0d0a 2020 2020 2020 2020 2020  hs):..          
-00005220: 2020 6966 2065 706f 6368 2025 2073 656c    if epoch % sel
-00005230: 662e 6366 672e 4348 4543 4b50 4f49 4e54  f.cfg.CHECKPOINT
-00005240: 5f46 5245 5120 3d3d 2030 3a0d 0a20 2020  _FREQ == 0:..   
-00005250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005260: 662e 7361 7665 5f63 6865 636b 706f 696e  f.save_checkpoin
-00005270: 7428 6570 6f63 6829 0d0a 2020 2020 2020  t(epoch)..      
-00005280: 2020 2020 2020 6966 2065 706f 6368 2025        if epoch %
-00005290: 2073 656c 662e 6366 672e 4556 414c 5f46   self.cfg.EVAL_F
-000052a0: 5245 5120 3d3d 2030 3a0d 0a20 2020 2020  REQ == 0:..     
-000052b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000052c0: 6c66 2e63 6667 2e45 5641 4c5f 5641 4c49  lf.cfg.EVAL_VALI
-000052d0: 443a 0d0a 2020 2020 2020 2020 2020 2020  D:..            
-000052e0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-000052f0: 6964 2865 706f 6368 290d 0a20 2020 2020  id(epoch)..     
-00005300: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00005310: 6c66 2e63 6667 2e45 5641 4c5f 5445 5354  lf.cfg.EVAL_TEST
-00005320: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005330: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
-00005340: 2865 706f 6368 290d 0a20 2020 2020 2020  (epoch)..       
-00005350: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-00005360: 6265 7374 2865 706f 6368 290d 0a20 2020  best(epoch)..   
-00005370: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00005380: 6570 2865 706f 6368 290d 0a20 2020 2020  ep(epoch)..     
-00005390: 2020 2020 2020 2073 656c 662e 7472 6169         self.trai
-000053a0: 6e28 6570 6f63 6829 0d0a 0d0a 2020 2020  n(epoch)....    
-000053b0: 2020 2020 7365 6c66 2e73 6176 6528 290d      self.save().
-000053c0: 0a0d 0a20 2020 2020 2020 2023 206c 6173  ...        # las
-000053d0: 7420 6570 6f63 680d 0a20 2020 2020 2020  t epoch..       
-000053e0: 2073 656c 662e 7661 6c69 6428 7365 6c66   self.valid(self
-000053f0: 2e63 6667 2e65 706f 6368 7329 0d0a 2020  .cfg.epochs)..  
-00005400: 2020 2020 2020 7365 6c66 2e74 6573 7428        self.test(
-00005410: 7365 6c66 2e63 6667 2e65 706f 6368 7329  self.cfg.epochs)
-00005420: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00005430: 6865 636b 5f62 6573 7428 7365 6c66 2e63  heck_best(self.c
-00005440: 6667 2e65 706f 6368 7329 0d0a 2020 2020  fg.epochs)..    
-00005450: 2020 2020 7365 6c66 2e73 7465 7028 7365      self.step(se
-00005460: 6c66 2e63 6667 2e65 706f 6368 7329 0d0a  lf.cfg.epochs)..
-00005470: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00005480: 756d 6d61 7279 2829 0d0a 0d0a 2020 2020  ummary()....    
-00005490: 2020 2020 7365 6c66 2e65 7661 6c5f 6174      self.eval_at
-000054a0: 5f62 6573 7428 290d 0a0d 0a0d 0a63 6c61  _best()......cla
-000054b0: 7373 2041 6461 7074 6572 3a0d 0a20 2020  ss Adapter:..   
-000054c0: 2072 2222 220d 0a20 2020 2050 6172 616d   r"""..    Param
-000054d0: 7320 7475 6e65 722e 0d0a 0d0a 2020 2020  s tuner.....    
-000054e0: 466c 6f77 733a 0d0a 2020 2020 2d2d 2d2d  Flows:..    ----
-000054f0: 2d2d 0d0a 2020 2020 312e 2063 6f6d 7069  --..    1. compi
-00005500: 6c65 3a20 636f 6e66 6967 7572 6520 7468  le: configure th
-00005510: 6520 636f 6d6d 616e 642c 2065 6e76 6972  e command, envir
-00005520: 6f6e 6d65 6e74 732c 2061 6e64 2070 6172  onments, and par
-00005530: 616d 6574 6572 7320 666f 7220 7472 6169  ameters for trai
-00005540: 6e69 6e67 2e0d 0a20 2020 2032 2e20 616c  ning...    2. al
-00005550: 6c6f 6361 7465 2064 6576 6963 6573 2066  locate devices f
-00005560: 6f72 2076 6172 696f 7573 2070 6172 616d  or various param
-00005570: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
-00005580: 2d20 7265 6769 7374 6572 2074 6865 2049  - register the I
-00005590: 442c 206c 6f67 2070 6174 682c 2061 6e64  D, log path, and
-000055a0: 2064 6576 6963 6520 6669 7273 740d 0a20   device first.. 
-000055b0: 2020 2020 2020 202d 2065 7865 6375 7465         - execute
-000055c0: 2074 6865 2063 6f6d 6d61 6e64 0d0a 2020   the command..  
-000055d0: 2020 2020 2020 2d20 636f 6c6c 6563 7420        - collect 
-000055e0: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
-000055f0: 2074 6865 206c 6f67 2070 6174 6820 616e   the log path an
-00005600: 6420 6f75 7470 7574 2074 6f20 5465 6e73  d output to Tens
-00005610: 6f72 426f 6172 640d 0a20 2020 2020 2020  orBoard..       
-00005620: 202d 2073 6176 6520 7468 6520 6368 6563   - save the chec
-00005630: 6b70 6f69 6e74 0d0a 2020 2020 2020 2020  kpoint..        
-00005640: 2d20 7265 6c65 6173 6520 7468 6520 636f  - release the co
-00005650: 7272 6573 706f 6e64 696e 6720 6465 7669  rresponding devi
-00005660: 6365 0d0a 0d0a 2020 2020 4578 616d 706c  ce....    Exampl
-00005670: 6573 3a0d 0a20 2020 202d 2d2d 2d2d 2d2d  es:..    -------
-00005680: 2d2d 0d0a 2020 2020 3e3e 3e20 6366 6720  --..    >>> cfg 
-00005690: 3d20 7b27 636f 6d6d 616e 6427 3a20 2770  = {'command': 'p
-000056a0: 7974 686f 6e20 7878 782e 7079 272c 2027  ython xxx.py', '
-000056b0: 7061 7261 6d73 273a 207b 276f 7074 696d  params': {'optim
-000056c0: 697a 6572 273a 205b 2773 6764 272c 2027  izer': ['sgd', '
-000056d0: 6164 616d 275d 7d7d 0d0a 2020 2020 3e3e  adam']}}..    >>
-000056e0: 3e20 7475 6e65 7220 3d20 4164 6170 7465  > tuner = Adapte
-000056f0: 7228 290d 0a20 2020 203e 3e3e 2074 756e  r()..    >>> tun
-00005700: 6572 2e63 6f6d 7069 6c65 2863 6667 290d  er.compile(cfg).
-00005710: 0a20 2020 203e 3e3e 2074 756e 6572 2e66  .    >>> tuner.f
-00005720: 6974 2829 0d0a 2020 2020 2222 220d 0a0d  it()..    """...
-00005730: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00005740: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00005750: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00005760: 6172 616d 7320 3d20 5b5d 0d0a 2020 2020  arams = []..    
-00005770: 2020 2020 7365 6c66 2e76 616c 7565 7320      self.values 
-00005780: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
-00005790: 6c66 2e64 6576 6963 6573 203d 2074 7570  lf.devices = tup
-000057a0: 6c65 2829 0d0a 0d0a 2020 2020 2020 2020  le()....        
-000057b0: 6465 6620 636c 6561 6e28 293a 0d0a 2020  def clean():..  
-000057c0: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
-000057d0: 203d 2070 7375 7469 6c2e 5072 6f63 6573   = psutil.Proces
-000057e0: 7328 6f73 2e67 6574 7069 6428 2929 0d0a  s(os.getpid())..
-000057f0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00005800: 6472 656e 203d 2070 6172 656e 742e 6368  dren = parent.ch
-00005810: 696c 6472 656e 2872 6563 7572 7369 7665  ildren(recursive
-00005820: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00005830: 2020 2020 666f 7220 7072 6f63 6573 7320      for process 
-00005840: 696e 2063 6869 6c64 7265 6e3a 0d0a 2020  in children:..  
-00005850: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00005860: 6f63 6573 732e 7365 6e64 5f73 6967 6e61  ocess.send_signa
-00005870: 6c28 7369 676e 616c 2e53 4947 5445 524d  l(signal.SIGTERM
-00005880: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00005890: 7375 7469 6c2e 7761 6974 5f70 726f 6373  sutil.wait_procs
-000058a0: 2863 6869 6c64 7265 6e2c 2074 696d 656f  (children, timeo
-000058b0: 7574 3d35 290d 0a0d 0a20 2020 2020 2020  ut=5)....       
-000058c0: 2061 7465 7869 742e 7265 6769 7374 6572   atexit.register
-000058d0: 2863 6c65 616e 290d 0a0d 0a20 2020 2040  (clean)....    @
-000058e0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-000058f0: 6620 434f 4d4d 414e 4428 7365 6c66 293a  f COMMAND(self):
-00005900: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00005910: 2073 656c 662e 6366 672e 434f 4d4d 414e   self.cfg.COMMAN
-00005920: 440d 0a0d 0a20 2020 2064 6566 2072 6567  D....    def reg
-00005930: 6973 7465 7228 7365 6c66 2c20 6465 7669  ister(self, devi
-00005940: 6365 3a20 7374 7229 202d 3e20 5475 706c  ce: str) -> Tupl
-00005950: 655b 7374 722c 2073 7472 5d3a 0d0a 2020  e[str, str]:..  
-00005960: 2020 2020 2020 7365 6c66 2e63 6667 2e45        self.cfg.E
-00005970: 4e56 535b 2769 6427 5d20 3d20 7469 6d65  NVS['id'] = time
-00005980: 2e73 7472 6674 696d 6528 5449 4d45 290d  .strftime(TIME).
-00005990: 0a20 2020 2020 2020 2073 656c 662e 6366  .        self.cf
-000059a0: 672e 454e 5653 5b27 6465 7669 6365 275d  g.ENVS['device']
-000059b0: 203d 2064 6576 6963 650d 0a20 2020 2020   = device..     
-000059c0: 2020 2063 6f6d 6d61 6e64 203d 2073 656c     command = sel
-000059d0: 662e 434f 4d4d 414e 4420 2b20 7365 6c66  f.COMMAND + self
-000059e0: 2e67 6574 5f6f 7074 696f 6e28 2769 6427  .get_option('id'
-000059f0: 2c20 7365 6c66 2e63 6667 2e45 4e56 532e  , self.cfg.ENVS.
-00005a00: 6964 290d 0a20 2020 2020 2020 2063 6f6d  id)..        com
-00005a10: 6d61 6e64 202b 3d20 7365 6c66 2e67 6574  mand += self.get
-00005a20: 5f6f 7074 696f 6e28 2764 6576 6963 6527  _option('device'
-00005a30: 2c20 7365 6c66 2e63 6667 2e45 4e56 532e  , self.cfg.ENVS.
-00005a40: 6465 7669 6365 290d 0a20 2020 2020 2020  device)..       
-00005a50: 2072 6574 7572 6e20 636f 6d6d 616e 642c   return command,
-00005a60: 2073 656c 662e 6366 672e 454e 5653 2e69   self.cfg.ENVS.i
-00005a70: 642c 2073 656c 662e 6366 672e 4c4f 475f  d, self.cfg.LOG_
-00005a80: 5041 5448 2e66 6f72 6d61 7428 2a2a 7365  PATH.format(**se
-00005a90: 6c66 2e63 6667 2e45 4e56 5329 0d0a 0d0a  lf.cfg.ENVS)....
-00005aa0: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
-00005ab0: 4164 6170 7465 722f 636f 6d70 696c 6522  Adapter/compile"
-00005ac0: 290d 0a20 2020 2064 6566 2063 6f6d 7069  )..    def compi
-00005ad0: 6c65 2873 656c 662c 2063 6667 3a20 436f  le(self, cfg: Co
-00005ae0: 6e66 6967 2920 2d3e 204e 6f6e 653a 0d0a  nfig) -> None:..
-00005af0: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
-00005b00: 2020 2020 2020 436f 6e66 6967 7572 6520        Configure 
-00005b10: 7468 6520 636f 6d6d 616e 642c 2065 6e76  the command, env
-00005b20: 6972 6f6e 6d65 6e74 732c 2061 6e64 2070  ironments, and p
-00005b30: 6172 616d 6574 6572 7320 666f 7220 7472  arameters for tr
-00005b40: 6169 6e69 6e67 2e0d 0a0d 0a20 2020 2020  aining.....     
-00005b50: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-00005b60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00005b70: 2d2d 2d0d 0a20 2020 2020 2020 2063 6667  ---..        cfg
-00005b80: 203a 2043 6f6e 6669 670d 0a20 2020 2020   : Config..     
-00005b90: 2020 2020 2020 2041 6e20 6f62 6a65 6374         An object
-00005ba0: 2074 6861 7420 636f 6e74 6169 6e73 2074   that contains t
-00005bb0: 6865 2063 6f6d 6d61 6e64 2c20 656e 7669  he command, envi
-00005bc0: 726f 6e6d 656e 7473 2c20 7061 7261 6d65  ronments, parame
-00005bd0: 7465 7273 2c20 616e 6420 6465 6661 756c  ters, and defaul
-00005be0: 7473 2e0d 0a0d 0a20 2020 2020 2020 2046  ts.....        F
-00005bf0: 6c6f 7773 3a0d 0a20 2020 2020 2020 202d  lows:..        -
-00005c00: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2031  -----..        1
-00005c10: 2e20 4164 6420 656e 7669 726f 6e6d 656e  . Add environmen
-00005c20: 7461 6c20 7061 7261 6d65 7465 7273 2074  tal parameters t
-00005c30: 6f20 7468 6520 6261 7369 6320 6063 6f6d  o the basic `com
-00005c40: 6d61 6e64 602e 0d0a 2020 2020 2020 2020  mand`...        
-00005c50: 322e 2052 6567 6973 7465 7220 616c 6c20  2. Register all 
-00005c60: 6176 6169 6c61 626c 6520 6465 7669 6365  available device
-00005c70: 732e 0d0a 2020 2020 2020 2020 332e 2043  s...        3. C
-00005c80: 6f6e 7665 7274 2061 6c6c 2070 6172 616d  onvert all param
-00005c90: 6574 6572 7320 6672 6f6d 2060 6366 672e  eters from `cfg.
-00005ca0: 5041 5241 4d53 602e 0d0a 2020 2020 2020  PARAMS`...      
-00005cb0: 2020 342e 2043 6f6e 7665 7274 2061 6c6c    4. Convert all
-00005cc0: 2064 6566 6175 6c74 7320 6672 6f6d 2060   defaults from `
-00005cd0: 6366 672e 4445 4641 554c 5453 602e 0d0a  cfg.DEFAULTS`...
-00005ce0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00005cf0: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00005d00: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4e6f  ----..        No
-00005d10: 6e65 0d0a 2020 2020 2020 2020 2222 220d  ne..        """.
-00005d20: 0a20 2020 2020 2020 2073 656c 662e 6366  .        self.cf
-00005d30: 6720 3d20 6366 670d 0a20 2020 2020 2020  g = cfg..       
-00005d40: 2070 6965 6365 203d 2022 5c74 7b6b 6579   piece = "\t{key
-00005d50: 7d3a 207b 7661 6c73 7d20 5c6e 220d 0a20  }: {vals} \n".. 
-00005d60: 2020 2020 2020 2065 6e76 732c 2070 6172         envs, par
-00005d70: 616d 732c 2064 6566 6175 6c74 7320 3d20  ams, defaults = 
-00005d80: 2222 2c20 2222 2c20 2222 0d0a 2020 2020  "", "", ""..    
-00005d90: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
-00005da0: 2069 6e20 7365 6c66 2e63 6667 2e45 4e56   in self.cfg.ENV
-00005db0: 532e 6974 656d 7328 293a 0d0a 2020 2020  S.items():..    
-00005dc0: 2020 2020 2020 2020 6966 206b 6579 203d          if key =
-00005dd0: 3d20 2764 6576 6963 6527 3a0d 0a20 2020  = 'device':..   
-00005de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005df0: 662e 6465 7669 6365 7320 3d20 7475 706c  f.devices = tupl
-00005e00: 6528 7661 6c2e 7370 6c69 7428 272c 2729  e(val.split(',')
-00005e10: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00005e20: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00005e30: 2020 2020 2020 7365 6c66 2e63 6667 2e43        self.cfg.C
-00005e40: 4f4d 4d41 4e44 202b 3d20 7365 6c66 2e67  OMMAND += self.g
-00005e50: 6574 5f6f 7074 696f 6e28 6b65 792c 2076  et_option(key, v
-00005e60: 616c 290d 0a20 2020 2020 2020 2020 2020  al)..           
-00005e70: 2065 6e76 7320 2b3d 2070 6965 6365 2e66   envs += piece.f
-00005e80: 6f72 6d61 7428 6b65 793d 6b65 792c 2076  ormat(key=key, v
-00005e90: 616c 733d 7661 6c29 0d0a 2020 2020 2020  als=val)..      
-00005ea0: 2020 666f 7220 6b65 792c 2076 616c 7320    for key, vals 
-00005eb0: 696e 2073 656c 662e 6366 672e 5041 5241  in self.cfg.PARA
-00005ec0: 4d53 2e69 7465 6d73 2829 3a0d 0a20 2020  MS.items():..   
-00005ed0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00005ee0: 7374 616e 6365 2876 616c 732c 2028 7374  stance(vals, (st
-00005ef0: 722c 2069 6e74 2c20 666c 6f61 7429 293a  r, int, float)):
-00005f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005f10: 2020 7661 6c73 203d 205b 7661 6c73 5d0d    vals = [vals].
-00005f20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005f30: 662e 6465 706c 6f79 5f70 6172 616d 7328  f.deploy_params(
-00005f40: 6b65 792c 2076 616c 7329 0d0a 2020 2020  key, vals)..    
-00005f50: 2020 2020 2020 2020 7061 7261 6d73 202b          params +
-00005f60: 3d20 7069 6563 652e 666f 726d 6174 286b  = piece.format(k
-00005f70: 6579 3d6b 6579 2c20 7661 6c73 3d76 616c  ey=key, vals=val
-00005f80: 7329 0d0a 2020 2020 2020 2020 666f 7220  s)..        for 
-00005f90: 6b65 792c 2076 616c 2069 6e20 7365 6c66  key, val in self
-00005fa0: 2e63 6667 2e44 4546 4155 4c54 532e 6974  .cfg.DEFAULTS.it
-00005fb0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00005fc0: 2020 2020 7365 6c66 2e63 6667 2e44 4546      self.cfg.DEF
-00005fd0: 4155 4c54 535b 6b65 795d 203d 2076 616c  AULTS[key] = val
-00005fe0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
-00005ff0: 6661 756c 7473 202b 3d20 7069 6563 652e  faults += piece.
-00006000: 666f 726d 6174 286b 6579 3d6b 6579 2c20  format(key=key, 
-00006010: 7661 6c73 3d76 616c 290d 0a0d 0a20 2020  vals=val)....   
-00006020: 2020 2020 2063 6667 5f69 6e66 6f73 203d       cfg_infos =
-00006030: 2066 2263 6f6d 6d61 6e64 3a20 7b73 656c   f"command: {sel
-00006040: 662e 6366 672e 434f 4d4d 414e 447d 205c  f.cfg.COMMAND} \
-00006050: 6e65 6e76 733a 205c 6e7b 656e 7673 7d70  nenvs: \n{envs}p
-00006060: 6172 616d 733a 205c 6e7b 7061 7261 6d73  arams: \n{params
-00006070: 7d64 6566 6175 6c74 733a 205c 6e7b 6465  }defaults: \n{de
-00006080: 6661 756c 7473 7d22 0d0a 2020 2020 2020  faults}"..      
-00006090: 2020 696e 666f 4c6f 6767 6572 2866 225c    infoLogger(f"\
-000060a0: 3033 335b 303b 3331 3b34 376d 7b63 6667  033[0;31;47m{cfg
-000060b0: 5f69 6e66 6f73 7d5c 3033 335b 306d 2229  _infos}\033[0m")
-000060c0: 0d0a 2020 2020 2020 2020 0d0a 0d0a 2020  ..        ....  
-000060d0: 2020 6465 6620 6465 706c 6f79 5f70 6172    def deploy_par
-000060e0: 616d 7328 7365 6c66 2c20 6b65 793a 2073  ams(self, key: s
-000060f0: 7472 2c20 7661 6c73 3a20 4974 6572 6162  tr, vals: Iterab
-00006100: 6c65 293a 0d0a 2020 2020 2020 2020 7365  le):..        se
-00006110: 6c66 2e70 6172 616d 732e 6170 7065 6e64  lf.params.append
-00006120: 286b 6579 290d 0a20 2020 2020 2020 2073  (key)..        s
-00006130: 656c 662e 7661 6c75 6573 2e61 7070 656e  elf.values.appen
-00006140: 6428 7661 6c73 290d 0a0d 0a20 2020 2040  d(vals)....    @
-00006150: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-00006160: 2020 6465 6620 6765 745f 6f70 7469 6f6e    def get_option
-00006170: 286b 6579 3a20 7374 722c 2076 616c 3a20  (key: str, val: 
-00006180: 416e 7929 3a0d 0a20 2020 2020 2020 2072  Any):..        r
-00006190: 2222 220d 0a20 2020 2020 2020 2043 6f6e  """..        Con
-000061a0: 7665 7274 2028 6b65 792c 2076 616c 2920  vert (key, val) 
-000061b0: 746f 2027 2d2d 6b65 793d 7661 6c27 2e0d  to '--key=val'..
-000061c0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000061d0: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
-000061e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
-000061f0: 2020 2020 206b 6579 203a 2073 7472 0d0a       key : str..
-00006200: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00006210: 6b65 7920 6f66 2074 6865 2070 6172 616d  key of the param
-00006220: 6574 6572 2e0d 0a20 2020 2020 2020 2076  eter...        v
-00006230: 616c 203a 2041 6e79 0d0a 2020 2020 2020  al : Any..      
-00006240: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-00006250: 6f66 2074 6865 2070 6172 616d 6574 6572  of the parameter
-00006260: 2e0d 0a0d 0a20 2020 2020 2020 204e 6f74  .....        Not
-00006270: 6573 3a0d 0a20 2020 2020 2020 202d 2d2d  es:..        ---
-00006280: 2d2d 2d0d 0a20 2020 2020 2020 2041 6c6c  ---..        All
-00006290: 2027 5f27 2069 6e20 606b 6579 6020 7769   '_' in `key` wi
-000062a0: 6c6c 2062 6520 7265 706c 6163 6564 2062  ll be replaced b
-000062b0: 7920 272d 272e 0d0a 0d0a 2020 2020 2020  y '-'.....      
-000062c0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-000062d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
-000062e0: 2020 2020 2020 7374 720d 0a20 2020 2020        str..     
-000062f0: 2020 2020 2020 2054 6865 2070 6172 616d         The param
-00006300: 6574 6572 2077 6974 6820 666f 726d 6174  eter with format
-00006310: 2027 2d2d 6b65 793d 7661 6c27 2e0d 0a0d   '--key=val'....
-00006320: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00006330: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00006340: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 203e  -----..        >
-00006350: 3e3e 2041 6461 7074 6572 2e67 6574 5f6f  >> Adapter.get_o
-00006360: 7074 696f 6e28 276c 7227 2c20 2731 652d  ption('lr', '1e-
-00006370: 3327 290d 0a20 2020 2020 2020 2027 2d2d  3')..        '--
-00006380: 6c72 3d31 652d 3327 0d0a 2020 2020 2020  lr=1e-3'..      
-00006390: 2020 3e3e 3e20 4164 6170 7465 722e 6765    >>> Adapter.ge
-000063a0: 745f 6f70 7469 6f6e 2827 6c65 6172 6e69  t_option('learni
-000063b0: 6e67 5f72 6174 6527 2c20 2731 652d 3327  ng_rate', '1e-3'
-000063c0: 290d 0a20 2020 2020 2020 2027 2d2d 6c65  )..        '--le
-000063d0: 6172 6e69 6e67 2d72 6174 653d 3165 2d33  arning-rate=1e-3
-000063e0: 270d 0a20 2020 2020 2020 2022 2222 0d0a  '..        """..
-000063f0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00006400: 2220 2d2d 7b6b 6579 2e72 6570 6c61 6365  " --{key.replace
-00006410: 2827 5f27 2c20 272d 2729 7d3d 7b76 616c  ('_', '-')}={val
-00006420: 7d22 0d0a 0d0a 2020 2020 6465 6620 6c6f  }"....    def lo
-00006430: 6164 5f62 6573 7428 7365 6c66 2c20 6c6f  ad_best(self, lo
-00006440: 6750 6174 683a 2073 7472 293a 0d0a 2020  gPath: str):..  
-00006450: 2020 2020 2020 2222 224c 6f61 6420 6265        """Load be
-00006460: 7374 2e70 6963 6b6c 6520 6672 6f6d 206c  st.pickle from l
-00006470: 6f67 5061 7468 206f 6620 636f 7272 6573  ogPath of corres
-00006480: 706f 6e64 696e 672e 2222 220d 0a20 2020  ponding."""..   
-00006490: 2020 2020 2066 696c 655f 203d 206f 732e       file_ = os.
-000064a0: 7061 7468 2e6a 6f69 6e28 6c6f 6750 6174  path.join(logPat
-000064b0: 682c 2073 656c 662e 6366 672e 4441 5441  h, self.cfg.DATA
-000064c0: 5f44 4952 2c20 7365 6c66 2e63 6667 2e4d  _DIR, self.cfg.M
-000064d0: 4f4e 4954 4f52 5f42 4553 545f 4649 4c45  ONITOR_BEST_FILE
-000064e0: 4e41 4d45 290d 0a20 2020 2020 2020 2072  NAME)..        r
-000064f0: 6574 7572 6e20 696d 706f 7274 5f70 6963  eturn import_pic
-00006500: 6b6c 6528 6669 6c65 5f29 0d0a 0d0a 2020  kle(file_)....  
-00006510: 2020 6465 6620 7772 6974 6528 7365 6c66    def write(self
-00006520: 2c20 6964 5f3a 2073 7472 2c20 6c6f 6750  , id_: str, logP
-00006530: 6174 683a 2073 7472 2c20 7061 7261 6d73  ath: str, params
-00006540: 3a20 4469 6374 293a 0d0a 2020 2020 2020  : Dict):..      
-00006550: 2020 7222 2222 0d0a 2020 2020 2020 2020    r"""..        
-00006560: 5772 6974 6520 6578 7065 7269 6d65 6e74  Write experiment
-00006570: 2072 6573 756c 7473 2074 6f20 7465 6e73   results to tens
-00006580: 6f72 626f 6172 642e 0d0a 0d0a 2020 2020  orboard.....    
-00006590: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-000065a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000065b0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6964  ----..        id
-000065c0: 5f3a 2073 7472 0d0a 2020 2020 2020 2020  _: str..        
-000065d0: 2020 2020 4578 7065 7269 6d65 6e74 2049      Experiment I
-000065e0: 442e 0d0a 2020 2020 2020 2020 6c6f 6750  D...        logP
-000065f0: 6174 683a 2073 7472 0d0a 2020 2020 2020  ath: str..      
-00006600: 2020 2020 2020 5061 7468 2074 6f20 7468        Path to th
-00006610: 6520 6578 7065 7269 6d65 6e74 206c 6f67  e experiment log
-00006620: 732e 0d0a 2020 2020 2020 2020 7061 7261  s...        para
-00006630: 6d73 3a20 4469 6374 0d0a 2020 2020 2020  ms: Dict..      
-00006640: 2020 2020 2020 436f 6e66 6967 7572 6174        Configurat
-00006650: 696f 6e20 7061 7261 6d65 7465 7273 206f  ion parameters o
-00006660: 6620 7468 6520 6578 7065 7269 6d65 6e74  f the experiment
-00006670: 2e0d 0a0d 0a20 2020 2020 2020 2046 6c6f  .....        Flo
-00006680: 7773 3a0d 0a20 2020 2020 2020 202d 2d2d  ws:..        ---
-00006690: 2d2d 2d0d 0a20 2020 2020 2020 2031 2e20  ---..        1. 
-000066a0: 4c6f 6164 2074 6865 2062 6573 7420 6461  Load the best da
-000066b0: 7461 2066 726f 6d20 606c 6f67 5061 7468  ta from `logPath
-000066c0: 602e 0d0a 2020 2020 2020 2020 322e 2057  `...        2. W
-000066d0: 7269 7465 2074 6865 2062 6573 7420 6461  rite the best da
-000066e0: 7461 2074 6f20 7465 6e73 6f72 626f 6172  ta to tensorboar
-000066f0: 6420 7769 7468 2060 7061 7261 6d73 602e  d with `params`.
-00006700: 0d0a 0d0a 2020 2020 2020 2020 4e6f 7465  ....        Note
-00006710: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00006720: 2d2d 0d0a 2020 2020 2020 2020 4966 2079  --..        If y
-00006730: 6f75 2066 696e 6420 602d 3160 2061 7070  ou find `-1` app
-00006740: 6561 7269 6e67 2069 6e20 7468 6520 7465  earing in the te
-00006750: 6e73 6f72 626f 6172 642c 0d0a 2020 2020  nsorboard,..    
-00006760: 2020 2020 6974 2063 6f75 6c64 206d 6561      it could mea
-00006770: 6e20 7468 6174 2074 6865 2064 6174 6120  n that the data 
-00006780: 6973 206f 6620 6073 7472 6020 7479 7065  is of `str` type
-00006790: 2c0d 0a20 2020 2020 2020 2077 6869 6368  ,..        which
-000067a0: 2077 696c 6c20 6361 7573 6520 616e 2065   will cause an e
-000067b0: 7272 6f72 2069 6620 6974 2069 7320 7365  rror if it is se
-000067c0: 6e74 2074 6f20 7465 6e73 6f72 626f 6172  nt to tensorboar
-000067d0: 6420 6469 7265 6374 6c79 210d 0a20 2020  d directly!..   
-000067e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000067f0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00006800: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
-00006810: 6c6f 6164 5f62 6573 7428 6c6f 6750 6174  load_best(logPat
-00006820: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-00006830: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00006840: 6f69 6e28 7365 6c66 2e63 6667 2e43 4f52  oin(self.cfg.COR
-00006850: 455f 4c4f 475f 5041 5448 2c20 6964 5f29  E_LOG_PATH, id_)
-00006860: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00006870: 7468 2053 756d 6d61 7279 5772 6974 6572  th SummaryWriter
-00006880: 286c 6f67 5f64 6972 3d70 6174 6829 2061  (log_dir=path) a
-00006890: 7320 7772 6974 6572 3a0d 0a20 2020 2020  s writer:..     
-000068a0: 2020 2020 2020 2020 2020 206d 6574 7269             metri
-000068b0: 6373 203d 2064 6963 7428 290d 0a20 2020  cs = dict()..   
-000068c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000068d0: 2070 7265 6669 782c 2062 6573 7420 696e   prefix, best in
-000068e0: 2064 6174 612e 6974 656d 7328 293a 0d0a   data.items():..
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 666f 7220 6d65 7472 6963 2c20      for metric, 
-00006910: 7661 6c20 696e 2062 6573 742e 6974 656d  val in best.item
-00006920: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00006930: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00006940: 6c20 3d20 7661 6c20 6966 2069 7369 6e73  l = val if isins
-00006950: 7461 6e63 6528 7661 6c2c 2028 696e 742c  tance(val, (int,
-00006960: 2066 6c6f 6174 2929 2065 6c73 6520 2d31   float)) else -1
-00006970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006980: 2020 2020 2020 2020 2020 6d65 7472 6963            metric
-00006990: 735b 272f 272e 6a6f 696e 285b 7072 6566  s['/'.join([pref
-000069a0: 6978 2c20 6d65 7472 6963 5d29 5d20 3d20  ix, metric])] = 
-000069b0: 7661 6c0d 0a20 2020 2020 2020 2020 2020  val..           
-000069c0: 2020 2020 2077 7269 7465 722e 6164 645f       writer.add_
-000069d0: 6870 6172 616d 7328 0d0a 2020 2020 2020  hparams(..      
-000069e0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000069f0: 7261 6d73 2c20 6d65 7472 6963 732c 0d0a  rams, metrics,..
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-00006a20: 7420 4578 6365 7074 696f 6e3a 0d0a 2020  t Exception:..  
-00006a30: 2020 2020 2020 2020 2020 696e 666f 4c6f            infoLo
-00006a40: 6767 6572 280d 0a20 2020 2020 2020 2020  gger(..         
-00006a50: 2020 2020 2020 2066 225c 3033 335b 303b         f"\033[0;
-00006a60: 3331 3b34 376d 5b41 6461 7074 6572 5d20  31;47m[Adapter] 
-00006a70: 3e3e 3e20 556e 6b6e 6f77 6e20 6572 726f  >>> Unknown erro
-00006a80: 7273 2068 6170 7065 6e2e 2054 6869 7320  rs happen. This 
-00006a90: 6973 206d 6169 6e6c 7920 6475 6520 746f  is mainly due to
-00006aa0: 2061 626e 6f72 6d61 6c20 6578 6974 7320   abnormal exits 
-00006ab0: 6f66 2063 6869 6c64 2070 726f 6365 7373  of child process
-00006ac0: 6573 2e5c 3033 335b 306d 220d 0a20 2020  es.\033[0m"..   
-00006ad0: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
-00006ae0: 2020 6465 6620 6561 6368 5f67 7269 6428    def each_grid(
-00006af0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00006b00: 2222 2247 7269 6420 7365 6172 6368 2066  """Grid search f
-00006b10: 6f72 2065 6163 6820 6b69 6e64 206f 6620  or each kind of 
-00006b20: 7061 7261 6d2e 2222 220d 0a20 2020 2020  param."""..     
-00006b30: 2020 2066 6f72 206b 6579 2c20 7661 6c73     for key, vals
-00006b40: 2069 6e20 7a69 7028 7365 6c66 2e70 6172   in zip(self.par
-00006b50: 616d 732c 2073 656c 662e 7661 6c75 6573  ams, self.values
-00006b60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00006b70: 666f 7220 7661 6c20 696e 2076 616c 733a  for val in vals:
-00006b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006b90: 2020 7969 656c 6420 7365 6c66 2e63 6667    yield self.cfg
-00006ba0: 2e44 4546 4155 4c54 5320 7c20 7b6b 6579  .DEFAULTS | {key
-00006bb0: 3a20 7661 6c7d 0d0a 0d0a 2020 2020 6465  : val}....    de
-00006bc0: 6620 7072 6f64 7563 745f 6772 6964 2873  f product_grid(s
-00006bd0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00006be0: 2222 4772 6964 2073 6561 7263 6820 6163  ""Grid search ac
-00006bf0: 726f 7373 2061 6c6c 2063 6f6d 6269 6e61  ross all combina
-00006c00: 7469 6f6e 206f 6620 7061 7261 6d73 2222  tion of params""
-00006c10: 220d 0a20 2020 2020 2020 2066 6f72 2076  "..        for v
-00006c20: 616c 7320 696e 2070 726f 6475 6374 282a  als in product(*
-00006c30: 7365 6c66 2e76 616c 7565 7329 3a0d 0a20  self.values):.. 
-00006c40: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00006c50: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
-00006c60: 5453 207c 207b 6f70 7469 6f6e 3a76 616c  TS | {option:val
-00006c70: 2066 6f72 206f 7074 696f 6e2c 2076 616c   for option, val
-00006c80: 2069 6e20 7a69 7028 7365 6c66 2e70 6172   in zip(self.par
-00006c90: 616d 732c 2076 616c 7329 7d0d 0a0d 0a20  ams, vals)}.... 
-00006ca0: 2020 2064 6566 2073 6176 655f 6368 6563     def save_chec
-00006cb0: 6b70 6f69 6e74 2873 656c 662c 2073 6f75  kpoint(self, sou
-00006cc0: 7263 653a 204c 6973 7429 202d 3e20 4e6f  rce: List) -> No
-00006cd0: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
-00006ce0: 5361 7665 2074 6865 2072 6573 7420 6f66  Save the rest of
-00006cf0: 2070 6172 616d 732e 2222 220d 0a20 2020   params."""..   
-00006d00: 2020 2020 2070 6174 6820 3d20 6f73 2e70       path = os.p
-00006d10: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
-00006d20: 672e 434f 5245 5f43 4845 434b 504f 494e  g.CORE_CHECKPOIN
-00006d30: 545f 5041 5448 2c20 7365 6c66 2e63 6667  T_PATH, self.cfg
-00006d40: 2e43 4845 434b 504f 494e 545f 4649 4c45  .CHECKPOINT_FILE
-00006d50: 4e41 4d45 290d 0a20 2020 2020 2020 2063  NAME)..        c
-00006d60: 6865 636b 706f 696e 7420 3d20 6469 6374  heckpoint = dict
-00006d70: 2829 0d0a 2020 2020 2020 2020 6368 6563  ()..        chec
-00006d80: 6b70 6f69 6e74 5b27 736f 7572 6365 275d  kpoint['source']
-00006d90: 203d 2073 6f75 7263 650d 0a20 2020 2020   = source..     
-00006da0: 2020 2074 6f72 6368 2e73 6176 6528 6368     torch.save(ch
-00006db0: 6563 6b70 6f69 6e74 2c20 7061 7468 290d  eckpoint, path).
-00006dc0: 0a0d 0a20 2020 2040 7469 6d65 6d65 7465  ...    @timemete
-00006dd0: 7228 2243 6f61 6368 2f72 6573 756d 6522  r("Coach/resume"
-00006de0: 290d 0a20 2020 2064 6566 206c 6f61 645f  )..    def load_
-00006df0: 6368 6563 6b70 6f69 6e74 2873 656c 6629  checkpoint(self)
-00006e00: 202d 3e20 696e 743a 0d0a 2020 2020 2020   -> int:..      
-00006e10: 2020 2222 224c 6f61 6420 7468 6520 7265    """Load the re
-00006e20: 7374 206f 6620 7061 7261 6d73 2e22 2222  st of params."""
-00006e30: 0d0a 2020 2020 2020 2020 696e 666f 4c6f  ..        infoLo
-00006e40: 6767 6572 2866 225b 436f 6163 685d 203e  gger(f"[Coach] >
-00006e50: 3e3e 204c 6f61 6420 7468 6520 7265 6365  >> Load the rece
-00006e60: 6e74 2063 6865 636b 706f 696e 7420 2e2e  nt checkpoint ..
-00006e70: 2e22 290d 0a20 2020 2020 2020 2070 6174  .")..        pat
-00006e80: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-00006e90: 2873 656c 662e 6366 672e 434f 5245 5f43  (self.cfg.CORE_C
-00006ea0: 4845 434b 504f 494e 545f 5041 5448 2c20  HECKPOINT_PATH, 
-00006eb0: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
-00006ec0: 494e 545f 4649 4c45 4e41 4d45 290d 0a20  INT_FILENAME).. 
-00006ed0: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
-00006ee0: 7420 3d20 746f 7263 682e 6c6f 6164 2870  t = torch.load(p
-00006ef0: 6174 6829 0d0a 2020 2020 2020 2020 7265  ath)..        re
-00006f00: 7475 726e 2063 6865 636b 706f 696e 745b  turn checkpoint[
-00006f10: 2773 6f75 7263 6527 5d0d 0a0d 0a20 2020  'source']....   
-00006f20: 2064 6566 2072 6573 756d 6528 7365 6c66   def resume(self
-00006f30: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
-00006f40: 6573 756d 6520 6672 6f6d 2074 6865 2072  esume from the r
-00006f50: 6563 656e 7420 6368 6563 6b70 6f69 6e74  ecent checkpoint
-00006f60: 2e22 2222 0d0a 2020 2020 2020 2020 736f  ."""..        so
-00006f70: 7572 6365 203d 2073 656c 662e 6561 6368  urce = self.each
-00006f80: 5f67 7269 6428 2920 6966 2073 656c 662e  _grid() if self.
-00006f90: 6366 672e 4558 434c 5553 4956 4520 656c  cfg.EXCLUSIVE el
-00006fa0: 7365 2073 656c 662e 7072 6f64 7563 745f  se self.product_
-00006fb0: 6772 6964 2829 0d0a 2020 2020 2020 2020  grid()..        
-00006fc0: 736f 7572 6365 203d 206c 6973 7428 736f  source = list(so
-00006fd0: 7572 6365 295b 3a3a 2d31 5d0d 0a20 2020  urce)[::-1]..   
-00006fe0: 2020 2020 2073 6f75 7263 6520 3d20 7365       source = se
-00006ff0: 6c66 2e6c 6f61 645f 6368 6563 6b70 6f69  lf.load_checkpoi
-00007000: 6e74 2829 2069 6620 7365 6c66 2e63 6667  nt() if self.cfg
-00007010: 2e72 6573 756d 6520 656c 7365 2073 6f75  .resume else sou
-00007020: 7263 650d 0a20 2020 2020 2020 2072 6574  rce..        ret
-00007030: 7572 6e20 736f 7572 6365 0d0a 0d0a 2020  urn source....  
-00007040: 2020 6465 6620 7275 6e28 7365 6c66 2c20    def run(self, 
-00007050: 636f 6d6d 616e 643a 2073 7472 2c20 7061  command: str, pa
-00007060: 7261 6d73 3a20 4469 6374 293a 0d0a 2020  rams: Dict):..  
-00007070: 2020 2020 2020 2222 2253 7461 7274 2061        """Start a
-00007080: 206e 6577 2073 7562 7072 6f63 6573 7322   new subprocess"
-00007090: 2222 0d0a 2020 2020 2020 2020 696d 706f  ""..        impo
-000070a0: 7274 2073 7562 7072 6f63 6573 732c 2073  rt subprocess, s
-000070b0: 686c 6578 0d0a 2020 2020 2020 2020 666f  hlex..        fo
-000070c0: 7220 6f70 7469 6f6e 2c20 7661 6c20 696e  r option, val in
-000070d0: 2070 6172 616d 732e 6974 656d 7328 293a   params.items():
-000070e0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000070f0: 6d6d 616e 6420 2b3d 2073 656c 662e 6765  mmand += self.ge
-00007100: 745f 6f70 7469 6f6e 286f 7074 696f 6e2c  t_option(option,
-00007110: 2076 616c 290d 0a20 2020 2020 2020 2069   val)..        i
-00007120: 6e66 6f4c 6f67 6765 7228 6622 5c30 3333  nfoLogger(f"\033
-00007130: 5b30 3b33 313b 3437 6d7b 636f 6d6d 616e  [0;31;47m{comman
-00007140: 647d 5c30 3333 5b30 6d22 290d 0a20 2020  d}\033[0m")..   
-00007150: 2020 2020 2072 6574 7572 6e20 7375 6270       return subp
-00007160: 726f 6365 7373 2e50 6f70 656e 2873 686c  rocess.Popen(shl
-00007170: 6578 2e73 706c 6974 2863 6f6d 6d61 6e64  ex.split(command
-00007180: 2929 0d0a 0d0a 2020 2020 6465 6620 7761  ))....    def wa
-00007190: 6974 2873 656c 662c 2074 6173 6b73 3a20  it(self, tasks: 
-000071a0: 4c69 7374 293a 0d0a 2020 2020 2020 2020  List):..        
-000071b0: 2222 2257 6169 7420 7574 696c 2061 6c6c  """Wait util all
-000071c0: 2070 726f 6365 7373 6573 2074 6572 6d69   processes termi
-000071d0: 6e61 7465 2e22 2222 0d0a 2020 2020 2020  nate."""..      
-000071e0: 2020 7461 736b 7320 3d20 5b74 6173 6b20    tasks = [task 
-000071f0: 666f 7220 7461 736b 2069 6e20 7461 736b  for task in task
-00007200: 7320 6966 2074 6173 6b20 6973 206e 6f74  s if task is not
-00007210: 204e 6f6e 655d 0d0a 2020 2020 2020 2020   None]..        
-00007220: 666f 7220 7072 6f63 6573 735f 2c20 6964  for process_, id
-00007230: 5f2c 206c 6f67 5061 7468 2c20 7061 7261  _, logPath, para
-00007240: 6d73 2069 6e20 7461 736b 733a 0d0a 2020  ms in tasks:..  
-00007250: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-00007260: 735f 2e77 6169 7428 290d 0a20 2020 2020  s_.wait()..     
-00007270: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
-00007280: 6528 6964 5f2c 206c 6f67 5061 7468 2c20  e(id_, logPath, 
-00007290: 7061 7261 6d73 290d 0a0d 0a20 2020 2064  params)....    d
-000072a0: 6566 2070 6f6c 6c28 7365 6c66 2c20 7461  ef poll(self, ta
-000072b0: 736b 733a 204c 6973 7429 3a0d 0a20 2020  sks: List):..   
-000072c0: 2020 2020 2022 2222 5761 6974 2075 7469       """Wait uti
-000072d0: 6c20 616e 7920 7072 6f63 6573 7320 7465  l any process te
-000072e0: 726d 696e 6174 6573 2e22 2222 0d0a 2020  rminates."""..  
-000072f0: 2020 2020 2020 6465 6620 6973 5f6e 756c        def is_nul
-00007300: 6c28 7461 736b 293a 0d0a 2020 2020 2020  l(task):..      
-00007310: 2020 2020 2020 7265 7475 726e 2074 6173        return tas
-00007320: 6b20 6973 204e 6f6e 650d 0a20 2020 2020  k is None..     
-00007330: 2020 2062 7566 6665 725f 736f 7572 6365     buffer_source
-00007340: 203d 205b 7461 736b 5b2d 315d 2066 6f72   = [task[-1] for
-00007350: 2074 6173 6b20 696e 2074 6173 6b73 2069   task in tasks i
-00007360: 6620 7461 736b 2069 7320 6e6f 7420 4e6f  f task is not No
-00007370: 6e65 5d0d 0a20 2020 2020 2020 2074 696d  ne]..        tim
-00007380: 652e 736c 6565 7028 3129 2023 2066 6f72  e.sleep(1) # for
-00007390: 2075 6e69 7175 6520 6964 0d0a 2020 2020   unique id..    
-000073a0: 2020 2020 7768 696c 6520 6e6f 7420 616e      while not an
-000073b0: 7928 6d61 7028 6973 5f6e 756c 6c2c 2074  y(map(is_null, t
-000073c0: 6173 6b73 2929 3a0d 0a20 2020 2020 2020  asks)):..       
-000073d0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000073e0: 3729 0d0a 2020 2020 2020 2020 2020 2020  7)..            
-000073f0: 6275 6666 6572 5f73 6f75 7263 6520 3d20  buffer_source = 
-00007400: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00007410: 666f 7220 692c 2028 7072 6f63 6573 735f  for i, (process_
-00007420: 2c20 6964 5f2c 206c 6f67 5061 7468 2c20  , id_, logPath, 
-00007430: 7061 7261 6d73 2920 696e 2065 6e75 6d65  params) in enume
-00007440: 7261 7465 2874 6173 6b73 293a 0d0a 2020  rate(tasks):..  
-00007450: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00007460: 2070 726f 6365 7373 5f2e 706f 6c6c 2829   process_.poll()
-00007470: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 2020 2073 656c 662e 7772 6974 6528 6964     self.write(id
-000074a0: 5f2c 206c 6f67 5061 7468 2c20 7061 7261  _, logPath, para
-000074b0: 6d73 290d 0a20 2020 2020 2020 2020 2020  ms)..           
-000074c0: 2020 2020 2020 2020 2074 6173 6b73 5b69           tasks[i
-000074d0: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 2020  ] = None..      
-000074e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-000074f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007500: 2020 2020 2062 7566 6665 725f 736f 7572       buffer_sour
-00007510: 6365 2e61 7070 656e 6428 7061 7261 6d73  ce.append(params
-00007520: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007530: 7361 7665 5f63 6865 636b 706f 696e 7428  save_checkpoint(
-00007540: 7365 6c66 2e73 6f75 7263 6520 2b20 6275  self.source + bu
-00007550: 6666 6572 5f73 6f75 7263 6529 0d0a 2020  ffer_source)..  
-00007560: 2020 2020 2020 7265 7475 726e 2074 6173        return tas
-00007570: 6b73 2e69 6e64 6578 284e 6f6e 6529 0d0a  ks.index(None)..
-00007580: 0d0a 2020 2020 6465 6620 7465 726d 696e  ..    def termin
-00007590: 6174 6528 7365 6c66 2c20 7461 736b 733a  ate(self, tasks:
-000075a0: 204c 6973 7429 3a0d 0a20 2020 2020 2020   List):..       
-000075b0: 2074 6173 6b73 203d 205b 7461 736b 2066   tasks = [task f
-000075c0: 6f72 2074 6173 6b20 696e 2074 6173 6b73  or task in tasks
-000075d0: 2069 6620 7461 736b 2069 7320 6e6f 7420   if task is not 
-000075e0: 4e6f 6e65 5d0d 0a20 2020 2020 2020 2066  None]..        f
-000075f0: 6f72 2070 726f 6365 7373 5f2c 205f 2c20  or process_, _, 
-00007600: 5f2c 205f 2069 6e20 7461 736b 733a 0d0a  _, _ in tasks:..
-00007610: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-00007620: 726f 6365 7373 5f2e 706f 6c6c 2829 2069  rocess_.poll() i
-00007630: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00007640: 2020 2020 2020 2020 2070 726f 6365 7373           process
-00007650: 5f2e 7465 726d 696e 6174 6528 290d 0a20  _.terminate().. 
-00007660: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00007670: 7028 3329 0d0a 2020 2020 2020 2020 666f  p(3)..        fo
-00007680: 7220 7072 6f63 6573 735f 2c20 5f2c 205f  r process_, _, _
-00007690: 2c20 5f20 696e 2074 6173 6b73 3a0d 0a20  , _ in tasks:.. 
-000076a0: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-000076b0: 6f63 6573 735f 2e70 6f6c 6c28 2920 6973  ocess_.poll() is
-000076c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000076d0: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
-000076e0: 2e6b 696c 6c28 290d 0a20 2020 2020 2020  .kill()..       
-000076f0: 2073 7973 2e65 7869 7428 290d 0a0d 0a20   sys.exit().... 
-00007700: 2020 2040 7469 6d65 6d65 7465 7228 2241     @timemeter("A
-00007710: 6461 7074 6572 2f66 6974 2229 0d0a 2020  dapter/fit")..  
-00007720: 2020 6465 6620 6669 7428 7365 6c66 293a    def fit(self):
-00007730: 0d0a 2020 2020 2020 2020 2222 2247 7269  ..        """Gri
-00007740: 6420 7365 6172 6368 2e22 2222 0d0a 2020  d search."""..  
-00007750: 2020 2020 2020 7365 6c66 2e73 6f75 7263        self.sourc
-00007760: 6520 3d20 7365 6c66 2e72 6573 756d 6528  e = self.resume(
-00007770: 290d 0a20 2020 2020 2020 2074 6173 6b73  )..        tasks
-00007780: 203d 205b 4e6f 6e65 2066 6f72 205f 2069   = [None for _ i
-00007790: 6e20 7261 6e67 6528 6c65 6e28 7365 6c66  n range(len(self
-000077a0: 2e64 6576 6963 6573 2929 5d0d 0a0d 0a20  .devices))].... 
-000077b0: 2020 2020 2020 2064 6566 2073 6967 6e61         def signa
-000077c0: 6c5f 6861 6e64 6c65 7228 7369 672c 2066  l_handler(sig, f
-000077d0: 7261 6d65 293a 0d0a 2020 2020 2020 2020  rame):..        
-000077e0: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
-000077f0: 225c 3033 335b 303b 3331 3b34 376d 3d3d  "\033[0;31;47m==
-00007800: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d54 4552  =============TER
-00007820: 4d49 4e41 5445 2041 4c4c 2053 5542 5052  MINATE ALL SUBPR
-00007830: 4f43 4553 5345 533d 3d3d 3d3d 3d3d 3d3d  OCESSES=========
-00007840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007850: 3d3d 3d3d 3d3d 5c30 3333 5b30 6d22 290d  ======\033[0m").
-00007860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007870: 662e 7465 726d 696e 6174 6528 7461 736b  f.terminate(task
-00007880: 7329 0d0a 2020 2020 2020 2020 7369 676e  s)..        sign
-00007890: 616c 2e73 6967 6e61 6c28 7369 676e 616c  al.signal(signal
-000078a0: 2e53 4947 494e 542c 2073 6967 6e61 6c5f  .SIGINT, signal_
-000078b0: 6861 6e64 6c65 7229 0d0a 0d0a 2020 2020  handler)....    
-000078c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000078d0: 2020 2020 2020 7768 696c 6520 7365 6c66        while self
-000078e0: 2e73 6f75 7263 653a 0d0a 2020 2020 2020  .source:..      
-000078f0: 2020 2020 2020 2020 2020 696e 6465 7820            index 
-00007900: 3d20 7365 6c66 2e70 6f6c 6c28 7461 736b  = self.poll(task
-00007910: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00007920: 2020 2020 6465 7669 6365 203d 2073 656c      device = sel
-00007930: 662e 6465 7669 6365 735b 696e 6465 785d  f.devices[index]
-00007940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007950: 2020 7061 7261 6d73 203d 2073 656c 662e    params = self.
-00007960: 736f 7572 6365 2e70 6f70 2829 0d0a 2020  source.pop()..  
-00007970: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00007980: 6d6d 616e 642c 2069 645f 2c20 6c6f 6750  mmand, id_, logP
-00007990: 6174 6820 3d20 7365 6c66 2e72 6567 6973  ath = self.regis
-000079a0: 7465 7228 6465 7669 6365 290d 0a20 2020  ter(device)..   
-000079b0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-000079c0: 6365 7373 5f20 3d20 7365 6c66 2e72 756e  cess_ = self.run
-000079d0: 2863 6f6d 6d61 6e64 2c20 7061 7261 6d73  (command, params
-000079e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000079f0: 2020 2074 6173 6b73 5b69 6e64 6578 5d20     tasks[index] 
-00007a00: 3d20 2870 726f 6365 7373 5f2c 2069 645f  = (process_, id_
-00007a10: 2c20 6c6f 6750 6174 682c 2070 6172 616d  , logPath, param
-00007a20: 7329 0d0a 2020 2020 2020 2020 6578 6365  s)..        exce
-00007a30: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00007a40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00007a50: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
-00007a60: 2020 6669 6e61 6c6c 793a 0d0a 2020 2020    finally:..    
-00007a70: 2020 2020 2020 2020 7365 6c66 2e77 6169          self.wai
-00007a80: 7428 7461 736b 7329 0d0a 2020 2020 2020  t(tasks)..      
-00007a90: 2020 2020 2020 7365 6c66 2e74 6572 6d69        self.termi
-00007aa0: 6e61 7465 2874 6173 6b73 29              nate(tasks)
+00005120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d54  ===============T
+00005130: 4552 4d49 4e41 5445 2043 5552 5245 4e54  ERMINATE CURRENT
+00005140: 2050 524f 4345 5353 3d3d 3d3d 3d3d 3d3d   PROCESS========
+00005150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005160: 3d3d 3d3d 3d3d 3d5c 3033 335b 306d 2229  =======\033[0m")
+00005170: 0d0a 2020 2020 2020 2020 2020 2020 7379  ..            sy
+00005180: 732e 6578 6974 2829 0d0a 2020 2020 2020  s.exit()..      
+00005190: 2020 7369 676e 616c 2e73 6967 6e61 6c28    signal.signal(
+000051a0: 7369 676e 616c 2e53 4947 494e 542c 2073  signal.SIGINT, s
+000051b0: 6967 6e61 6c5f 6861 6e64 6c65 7229 0d0a  ignal_handler)..
+000051c0: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
+000051d0: 6570 6f63 6820 3d20 7365 6c66 2e72 6573  epoch = self.res
+000051e0: 756d 6528 290d 0a20 2020 2020 2020 2066  ume()..        f
+000051f0: 6f72 2065 706f 6368 2069 6e20 7261 6e67  or epoch in rang
+00005200: 6528 7374 6172 745f 6570 6f63 682c 2073  e(start_epoch, s
+00005210: 656c 662e 6366 672e 6570 6f63 6873 293a  elf.cfg.epochs):
+00005220: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005230: 2065 706f 6368 2025 2073 656c 662e 6366   epoch % self.cf
+00005240: 672e 4348 4543 4b50 4f49 4e54 5f46 5245  g.CHECKPOINT_FRE
+00005250: 5120 3d3d 2030 3a0d 0a20 2020 2020 2020  Q == 0:..       
+00005260: 2020 2020 2020 2020 2073 656c 662e 7361           self.sa
+00005270: 7665 5f63 6865 636b 706f 696e 7428 6570  ve_checkpoint(ep
+00005280: 6f63 6829 0d0a 2020 2020 2020 2020 2020  och)..          
+00005290: 2020 6966 2065 706f 6368 2025 2073 656c    if epoch % sel
+000052a0: 662e 6366 672e 4556 414c 5f46 5245 5120  f.cfg.EVAL_FREQ 
+000052b0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+000052c0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000052d0: 6667 2e45 5641 4c5f 5641 4c49 443a 0d0a  fg.EVAL_VALID:..
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 2020 2020 7365 6c66 2e76 616c 6964 2865      self.valid(e
+00005300: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
+00005310: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00005320: 6667 2e45 5641 4c5f 5445 5354 3a0d 0a20  fg.EVAL_TEST:.. 
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2073 656c 662e 7465 7374 2865 706f     self.test(epo
+00005350: 6368 290d 0a20 2020 2020 2020 2020 2020  ch)..           
+00005360: 2073 656c 662e 6368 6563 6b5f 6265 7374   self.check_best
+00005370: 2865 706f 6368 290d 0a20 2020 2020 2020  (epoch)..       
+00005380: 2020 2020 2073 656c 662e 7374 6570 2865       self.step(e
+00005390: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
+000053a0: 2020 2073 656c 662e 7472 6169 6e28 6570     self.train(ep
+000053b0: 6f63 6829 0d0a 0d0a 2020 2020 2020 2020  och)....        
+000053c0: 7365 6c66 2e73 6176 6528 290d 0a0d 0a20  self.save().... 
+000053d0: 2020 2020 2020 2023 206c 6173 7420 6570         # last ep
+000053e0: 6f63 680d 0a20 2020 2020 2020 2073 656c  och..        sel
+000053f0: 662e 7661 6c69 6428 7365 6c66 2e63 6667  f.valid(self.cfg
+00005400: 2e65 706f 6368 7329 0d0a 2020 2020 2020  .epochs)..      
+00005410: 2020 7365 6c66 2e74 6573 7428 7365 6c66    self.test(self
+00005420: 2e63 6667 2e65 706f 6368 7329 0d0a 2020  .cfg.epochs)..  
+00005430: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00005440: 5f62 6573 7428 7365 6c66 2e63 6667 2e65  _best(self.cfg.e
+00005450: 706f 6368 7329 0d0a 2020 2020 2020 2020  pochs)..        
+00005460: 7365 6c66 2e73 7465 7028 7365 6c66 2e63  self.step(self.c
+00005470: 6667 2e65 706f 6368 7329 0d0a 0d0a 2020  fg.epochs)....  
+00005480: 2020 2020 2020 7365 6c66 2e73 756d 6d61        self.summa
+00005490: 7279 2829 0d0a 0d0a 2020 2020 2020 2020  ry()....        
+000054a0: 7365 6c66 2e65 7661 6c5f 6174 5f62 6573  self.eval_at_bes
+000054b0: 7428 290d 0a0d 0a0d 0a63 6c61 7373 2041  t()......class A
+000054c0: 6461 7074 6572 3a0d 0a20 2020 2072 2222  dapter:..    r""
+000054d0: 220d 0a20 2020 2050 6172 616d 7320 7475  "..    Params tu
+000054e0: 6e65 722e 0d0a 0d0a 2020 2020 466c 6f77  ner.....    Flow
+000054f0: 733a 0d0a 2020 2020 2d2d 2d2d 2d2d 0d0a  s:..    ------..
+00005500: 2020 2020 312e 2063 6f6d 7069 6c65 3a20      1. compile: 
+00005510: 636f 6e66 6967 7572 6520 7468 6520 636f  configure the co
+00005520: 6d6d 616e 642c 2065 6e76 6972 6f6e 6d65  mmand, environme
+00005530: 6e74 732c 2061 6e64 2070 6172 616d 6574  nts, and paramet
+00005540: 6572 7320 666f 7220 7472 6169 6e69 6e67  ers for training
+00005550: 2e0d 0a20 2020 2032 2e20 616c 6c6f 6361  ...    2. alloca
+00005560: 7465 2064 6576 6963 6573 2066 6f72 2076  te devices for v
+00005570: 6172 696f 7573 2070 6172 616d 6574 6572  arious parameter
+00005580: 733a 0d0a 2020 2020 2020 2020 2d20 7265  s:..        - re
+00005590: 6769 7374 6572 2074 6865 2049 442c 206c  gister the ID, l
+000055a0: 6f67 2070 6174 682c 2061 6e64 2064 6576  og path, and dev
+000055b0: 6963 6520 6669 7273 740d 0a20 2020 2020  ice first..     
+000055c0: 2020 202d 2065 7865 6375 7465 2074 6865     - execute the
+000055d0: 2063 6f6d 6d61 6e64 0d0a 2020 2020 2020   command..      
+000055e0: 2020 2d20 636f 6c6c 6563 7420 696e 666f    - collect info
+000055f0: 726d 6174 696f 6e20 6672 6f6d 2074 6865  rmation from the
+00005600: 206c 6f67 2070 6174 6820 616e 6420 6f75   log path and ou
+00005610: 7470 7574 2074 6f20 5465 6e73 6f72 426f  tput to TensorBo
+00005620: 6172 640d 0a20 2020 2020 2020 202d 2073  ard..        - s
+00005630: 6176 6520 7468 6520 6368 6563 6b70 6f69  ave the checkpoi
+00005640: 6e74 0d0a 2020 2020 2020 2020 2d20 7265  nt..        - re
+00005650: 6c65 6173 6520 7468 6520 636f 7272 6573  lease the corres
+00005660: 706f 6e64 696e 6720 6465 7669 6365 0d0a  ponding device..
+00005670: 0d0a 2020 2020 4578 616d 706c 6573 3a0d  ..    Examples:.
+00005680: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a  .    ---------..
+00005690: 2020 2020 3e3e 3e20 6366 6720 3d20 7b27      >>> cfg = {'
+000056a0: 636f 6d6d 616e 6427 3a20 2770 7974 686f  command': 'pytho
+000056b0: 6e20 7878 782e 7079 272c 2027 7061 7261  n xxx.py', 'para
+000056c0: 6d73 273a 207b 276f 7074 696d 697a 6572  ms': {'optimizer
+000056d0: 273a 205b 2773 6764 272c 2027 6164 616d  ': ['sgd', 'adam
+000056e0: 275d 7d7d 0d0a 2020 2020 3e3e 3e20 7475  ']}}..    >>> tu
+000056f0: 6e65 7220 3d20 4164 6170 7465 7228 290d  ner = Adapter().
+00005700: 0a20 2020 203e 3e3e 2074 756e 6572 2e63  .    >>> tuner.c
+00005710: 6f6d 7069 6c65 2863 6667 290d 0a20 2020  ompile(cfg)..   
+00005720: 203e 3e3e 2074 756e 6572 2e66 6974 2829   >>> tuner.fit()
+00005730: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
+00005740: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00005750: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
+00005760: 2020 2020 2020 7365 6c66 2e70 6172 616d        self.param
+00005770: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00005780: 7365 6c66 2e76 616c 7565 7320 3d20 5b5d  self.values = []
+00005790: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+000057a0: 6576 6963 6573 203d 2074 7570 6c65 2829  evices = tuple()
+000057b0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+000057c0: 790d 0a20 2020 2064 6566 2043 4f4d 4d41  y..    def COMMA
+000057d0: 4e44 2873 656c 6629 3a0d 0a20 2020 2020  ND(self):..     
+000057e0: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+000057f0: 6667 2e43 4f4d 4d41 4e44 0d0a 0d0a 2020  fg.COMMAND....  
+00005800: 2020 6465 6620 7265 6769 7374 6572 2873    def register(s
+00005810: 656c 662c 2064 6576 6963 653a 2073 7472  elf, device: str
+00005820: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
+00005830: 7374 725d 3a0d 0a20 2020 2020 2020 2073  str]:..        s
+00005840: 656c 662e 6366 672e 454e 5653 5b27 6964  elf.cfg.ENVS['id
+00005850: 275d 203d 2074 696d 652e 7374 7266 7469  '] = time.strfti
+00005860: 6d65 2854 494d 4529 0d0a 2020 2020 2020  me(TIME)..      
+00005870: 2020 7365 6c66 2e63 6667 2e45 4e56 535b    self.cfg.ENVS[
+00005880: 2764 6576 6963 6527 5d20 3d20 6465 7669  'device'] = devi
+00005890: 6365 0d0a 2020 2020 2020 2020 636f 6d6d  ce..        comm
+000058a0: 616e 6420 3d20 7365 6c66 2e43 4f4d 4d41  and = self.COMMA
+000058b0: 4e44 202b 2073 656c 662e 6765 745f 6f70  ND + self.get_op
+000058c0: 7469 6f6e 2827 6964 272c 2073 656c 662e  tion('id', self.
+000058d0: 6366 672e 454e 5653 2e69 6429 0d0a 2020  cfg.ENVS.id)..  
+000058e0: 2020 2020 2020 636f 6d6d 616e 6420 2b3d        command +=
+000058f0: 2073 656c 662e 6765 745f 6f70 7469 6f6e   self.get_option
+00005900: 2827 6465 7669 6365 272c 2073 656c 662e  ('device', self.
+00005910: 6366 672e 454e 5653 2e64 6576 6963 6529  cfg.ENVS.device)
+00005920: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005930: 2063 6f6d 6d61 6e64 2c20 7365 6c66 2e63   command, self.c
+00005940: 6667 2e45 4e56 532e 6964 2c20 7365 6c66  fg.ENVS.id, self
+00005950: 2e63 6667 2e4c 4f47 5f50 4154 482e 666f  .cfg.LOG_PATH.fo
+00005960: 726d 6174 282a 2a73 656c 662e 6366 672e  rmat(**self.cfg.
+00005970: 454e 5653 290d 0a0d 0a20 2020 2040 7469  ENVS)....    @ti
+00005980: 6d65 6d65 7465 7228 2241 6461 7074 6572  memeter("Adapter
+00005990: 2f63 6f6d 7069 6c65 2229 0d0a 2020 2020  /compile")..    
+000059a0: 6465 6620 636f 6d70 696c 6528 7365 6c66  def compile(self
+000059b0: 2c20 6366 673a 2043 6f6e 6669 6729 202d  , cfg: Config) -
+000059c0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+000059d0: 2072 2222 220d 0a20 2020 2020 2020 2043   r"""..        C
+000059e0: 6f6e 6669 6775 7265 2074 6865 2063 6f6d  onfigure the com
+000059f0: 6d61 6e64 2c20 656e 7669 726f 6e6d 656e  mand, environmen
+00005a00: 7473 2c20 616e 6420 7061 7261 6d65 7465  ts, and paramete
+00005a10: 7273 2066 6f72 2074 7261 696e 696e 672e  rs for training.
+00005a20: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+00005a30: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+00005a40: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020   -----------..  
+00005a50: 2020 2020 2020 6366 6720 3a20 436f 6e66        cfg : Conf
+00005a60: 6967 0d0a 2020 2020 2020 2020 2020 2020  ig..            
+00005a70: 416e 206f 626a 6563 7420 7468 6174 2063  An object that c
+00005a80: 6f6e 7461 696e 7320 7468 6520 636f 6d6d  ontains the comm
+00005a90: 616e 642c 2065 6e76 6972 6f6e 6d65 6e74  and, environment
+00005aa0: 732c 2070 6172 616d 6574 6572 732c 2061  s, parameters, a
+00005ab0: 6e64 2064 6566 6175 6c74 732e 0d0a 0d0a  nd defaults.....
+00005ac0: 2020 2020 2020 2020 466c 6f77 733a 0d0a          Flows:..
+00005ad0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
+00005ae0: 2020 2020 2020 2020 312e 2041 6464 2065          1. Add e
+00005af0: 6e76 6972 6f6e 6d65 6e74 616c 2070 6172  nvironmental par
+00005b00: 616d 6574 6572 7320 746f 2074 6865 2062  ameters to the b
+00005b10: 6173 6963 2060 636f 6d6d 616e 6460 2e0d  asic `command`..
+00005b20: 0a20 2020 2020 2020 2032 2e20 5265 6769  .        2. Regi
+00005b30: 7374 6572 2061 6c6c 2061 7661 696c 6162  ster all availab
+00005b40: 6c65 2064 6576 6963 6573 2e0d 0a20 2020  le devices...   
+00005b50: 2020 2020 2033 2e20 436f 6e76 6572 7420       3. Convert 
+00005b60: 616c 6c20 7061 7261 6d65 7465 7273 2066  all parameters f
+00005b70: 726f 6d20 6063 6667 2e50 4152 414d 5360  rom `cfg.PARAMS`
+00005b80: 2e0d 0a20 2020 2020 2020 2034 2e20 436f  ...        4. Co
+00005b90: 6e76 6572 7420 616c 6c20 6465 6661 756c  nvert all defaul
+00005ba0: 7473 2066 726f 6d20 6063 6667 2e44 4546  ts from `cfg.DEF
+00005bb0: 4155 4c54 5360 2e0d 0a0d 0a20 2020 2020  AULTS`.....     
+00005bc0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00005bd0: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
+00005be0: 2020 2020 2020 204e 6f6e 650d 0a20 2020         None..   
+00005bf0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00005c00: 2020 7365 6c66 2e63 6667 203d 2063 6667    self.cfg = cfg
+00005c10: 0d0a 2020 2020 2020 2020 7069 6563 6520  ..        piece 
+00005c20: 3d20 225c 747b 6b65 797d 3a20 7b76 616c  = "\t{key}: {val
+00005c30: 737d 205c 6e22 0d0a 2020 2020 2020 2020  s} \n"..        
+00005c40: 656e 7673 2c20 7061 7261 6d73 2c20 6465  envs, params, de
+00005c50: 6661 756c 7473 203d 2022 222c 2022 222c  faults = "", "",
+00005c60: 2022 220d 0a20 2020 2020 2020 2066 6f72   ""..        for
+00005c70: 206b 6579 2c20 7661 6c20 696e 2073 656c   key, val in sel
+00005c80: 662e 6366 672e 454e 5653 2e69 7465 6d73  f.cfg.ENVS.items
+00005c90: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00005ca0: 2069 6620 6b65 7920 3d3d 2027 6465 7669   if key == 'devi
+00005cb0: 6365 273a 0d0a 2020 2020 2020 2020 2020  ce':..          
+00005cc0: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
+00005cd0: 6573 203d 2074 7570 6c65 2876 616c 2e73  es = tuple(val.s
+00005ce0: 706c 6974 2827 2c27 2929 0d0a 2020 2020  plit(','))..    
+00005cf0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005d10: 656c 662e 6366 672e 434f 4d4d 414e 4420  elf.cfg.COMMAND 
+00005d20: 2b3d 2073 656c 662e 6765 745f 6f70 7469  += self.get_opti
+00005d30: 6f6e 286b 6579 2c20 7661 6c29 0d0a 2020  on(key, val)..  
+00005d40: 2020 2020 2020 2020 2020 656e 7673 202b            envs +
+00005d50: 3d20 7069 6563 652e 666f 726d 6174 286b  = piece.format(k
+00005d60: 6579 3d6b 6579 2c20 7661 6c73 3d76 616c  ey=key, vals=val
+00005d70: 290d 0a20 2020 2020 2020 2066 6f72 206b  )..        for k
+00005d80: 6579 2c20 7661 6c73 2069 6e20 7365 6c66  ey, vals in self
+00005d90: 2e63 6667 2e50 4152 414d 532e 6974 656d  .cfg.PARAMS.item
+00005da0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00005db0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00005dc0: 7661 6c73 2c20 2873 7472 2c20 696e 742c  vals, (str, int,
+00005dd0: 2066 6c6f 6174 2929 3a0d 0a20 2020 2020   float)):..     
+00005de0: 2020 2020 2020 2020 2020 2076 616c 7320             vals 
+00005df0: 3d20 5b76 616c 735d 0d0a 2020 2020 2020  = [vals]..      
+00005e00: 2020 2020 2020 7365 6c66 2e64 6570 6c6f        self.deplo
+00005e10: 795f 7061 7261 6d73 286b 6579 2c20 7661  y_params(key, va
+00005e20: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
+00005e30: 2070 6172 616d 7320 2b3d 2070 6965 6365   params += piece
+00005e40: 2e66 6f72 6d61 7428 6b65 793d 6b65 792c  .format(key=key,
+00005e50: 2076 616c 733d 7661 6c73 290d 0a20 2020   vals=vals)..   
+00005e60: 2020 2020 2066 6f72 206b 6579 2c20 7661       for key, va
+00005e70: 6c20 696e 2073 656c 662e 6366 672e 4445  l in self.cfg.DE
+00005e80: 4641 554c 5453 2e69 7465 6d73 2829 3a0d  FAULTS.items():.
+00005e90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005ea0: 662e 6366 672e 4445 4641 554c 5453 5b6b  f.cfg.DEFAULTS[k
+00005eb0: 6579 5d20 3d20 7661 6c0d 0a20 2020 2020  ey] = val..     
+00005ec0: 2020 2020 2020 2064 6566 6175 6c74 7320         defaults 
+00005ed0: 2b3d 2070 6965 6365 2e66 6f72 6d61 7428  += piece.format(
+00005ee0: 6b65 793d 6b65 792c 2076 616c 733d 7661  key=key, vals=va
+00005ef0: 6c29 0d0a 0d0a 2020 2020 2020 2020 6366  l)....        cf
+00005f00: 675f 696e 666f 7320 3d20 6622 636f 6d6d  g_infos = f"comm
+00005f10: 616e 643a 207b 7365 6c66 2e63 6667 2e43  and: {self.cfg.C
+00005f20: 4f4d 4d41 4e44 7d20 5c6e 656e 7673 3a20  OMMAND} \nenvs: 
+00005f30: 5c6e 7b65 6e76 737d 7061 7261 6d73 3a20  \n{envs}params: 
+00005f40: 5c6e 7b70 6172 616d 737d 6465 6661 756c  \n{params}defaul
+00005f50: 7473 3a20 5c6e 7b64 6566 6175 6c74 737d  ts: \n{defaults}
+00005f60: 220d 0a20 2020 2020 2020 2069 6e66 6f4c  "..        infoL
+00005f70: 6f67 6765 7228 6622 5c30 3333 5b30 3b33  ogger(f"\033[0;3
+00005f80: 313b 3437 6d7b 6366 675f 696e 666f 737d  1;47m{cfg_infos}
+00005f90: 5c30 3333 5b30 6d22 290d 0a20 2020 2020  \033[0m")..     
+00005fa0: 2020 200d 0a0d 0a20 2020 2064 6566 2064     ....    def d
+00005fb0: 6570 6c6f 795f 7061 7261 6d73 2873 656c  eploy_params(sel
+00005fc0: 662c 206b 6579 3a20 7374 722c 2076 616c  f, key: str, val
+00005fd0: 733a 2049 7465 7261 626c 6529 3a0d 0a20  s: Iterable):.. 
+00005fe0: 2020 2020 2020 2073 656c 662e 7061 7261         self.para
+00005ff0: 6d73 2e61 7070 656e 6428 6b65 7929 0d0a  ms.append(key)..
+00006000: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00006010: 7565 732e 6170 7065 6e64 2876 616c 7329  ues.append(vals)
+00006020: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00006030: 6574 686f 640d 0a20 2020 2064 6566 2067  ethod..    def g
+00006040: 6574 5f6f 7074 696f 6e28 6b65 793a 2073  et_option(key: s
+00006050: 7472 2c20 7661 6c3a 2041 6e79 293a 0d0a  tr, val: Any):..
+00006060: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
+00006070: 2020 2020 2020 436f 6e76 6572 7420 286b        Convert (k
+00006080: 6579 2c20 7661 6c29 2074 6f20 272d 2d6b  ey, val) to '--k
+00006090: 6579 3d76 616c 272e 0d0a 0d0a 2020 2020  ey=val'.....    
+000060a0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+000060b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000060c0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6b65  ----..        ke
+000060d0: 7920 3a20 7374 720d 0a20 2020 2020 2020  y : str..       
+000060e0: 2020 2020 2054 6865 206b 6579 206f 6620       The key of 
+000060f0: 7468 6520 7061 7261 6d65 7465 722e 0d0a  the parameter...
+00006100: 2020 2020 2020 2020 7661 6c20 3a20 416e          val : An
+00006110: 790d 0a20 2020 2020 2020 2020 2020 2054  y..            T
+00006120: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00006130: 7061 7261 6d65 7465 722e 0d0a 0d0a 2020  parameter.....  
+00006140: 2020 2020 2020 4e6f 7465 733a 0d0a 2020        Notes:..  
+00006150: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
+00006160: 2020 2020 2020 416c 6c20 275f 2720 696e        All '_' in
+00006170: 2060 6b65 7960 2077 696c 6c20 6265 2072   `key` will be r
+00006180: 6570 6c61 6365 6420 6279 2027 2d27 2e0d  eplaced by '-'..
+00006190: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000061a0: 6e73 3a0d 0a20 2020 2020 2020 202d 2d2d  ns:..        ---
+000061b0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+000061c0: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
+000061d0: 5468 6520 7061 7261 6d65 7465 7220 7769  The parameter wi
+000061e0: 7468 2066 6f72 6d61 7420 272d 2d6b 6579  th format '--key
+000061f0: 3d76 616c 272e 0d0a 0d0a 2020 2020 2020  =val'.....      
+00006200: 2020 4578 616d 706c 6573 3a0d 0a20 2020    Examples:..   
+00006210: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a       ---------..
+00006220: 2020 2020 2020 2020 3e3e 3e20 4164 6170          >>> Adap
+00006230: 7465 722e 6765 745f 6f70 7469 6f6e 2827  ter.get_option('
+00006240: 6c72 272c 2027 3165 2d33 2729 0d0a 2020  lr', '1e-3')..  
+00006250: 2020 2020 2020 272d 2d6c 723d 3165 2d33        '--lr=1e-3
+00006260: 270d 0a20 2020 2020 2020 203e 3e3e 2041  '..        >>> A
+00006270: 6461 7074 6572 2e67 6574 5f6f 7074 696f  dapter.get_optio
+00006280: 6e28 276c 6561 726e 696e 675f 7261 7465  n('learning_rate
+00006290: 272c 2027 3165 2d33 2729 0d0a 2020 2020  ', '1e-3')..    
+000062a0: 2020 2020 272d 2d6c 6561 726e 696e 672d      '--learning-
+000062b0: 7261 7465 3d31 652d 3327 0d0a 2020 2020  rate=1e-3'..    
+000062c0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000062d0: 2072 6574 7572 6e20 6622 202d 2d7b 6b65   return f" --{ke
+000062e0: 792e 7265 706c 6163 6528 275f 272c 2027  y.replace('_', '
+000062f0: 2d27 297d 3d7b 7661 6c7d 220d 0a0d 0a20  -')}={val}".... 
+00006300: 2020 2064 6566 206c 6f61 645f 6265 7374     def load_best
+00006310: 2873 656c 662c 206c 6f67 5061 7468 3a20  (self, logPath: 
+00006320: 7374 7229 3a0d 0a20 2020 2020 2020 2022  str):..        "
+00006330: 2222 4c6f 6164 2062 6573 742e 7069 636b  ""Load best.pick
+00006340: 6c65 2066 726f 6d20 6c6f 6750 6174 6820  le from logPath 
+00006350: 6f66 2063 6f72 7265 7370 6f6e 6469 6e67  of corresponding
+00006360: 2e22 2222 0d0a 2020 2020 2020 2020 6669  ."""..        fi
+00006370: 6c65 5f20 3d20 6f73 2e70 6174 682e 6a6f  le_ = os.path.jo
+00006380: 696e 286c 6f67 5061 7468 2c20 7365 6c66  in(logPath, self
+00006390: 2e63 6667 2e44 4154 415f 4449 522c 2073  .cfg.DATA_DIR, s
+000063a0: 656c 662e 6366 672e 4d4f 4e49 544f 525f  elf.cfg.MONITOR_
+000063b0: 4245 5354 5f46 494c 454e 414d 4529 0d0a  BEST_FILENAME)..
+000063c0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+000063d0: 6d70 6f72 745f 7069 636b 6c65 2866 696c  mport_pickle(fil
+000063e0: 655f 290d 0a0d 0a20 2020 2064 6566 2077  e_)....    def w
+000063f0: 7269 7465 2873 656c 662c 2069 645f 3a20  rite(self, id_: 
+00006400: 7374 722c 206c 6f67 5061 7468 3a20 7374  str, logPath: st
+00006410: 722c 2070 6172 616d 733a 2044 6963 7429  r, params: Dict)
+00006420: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
+00006430: 0a20 2020 2020 2020 2057 7269 7465 2065  .        Write e
+00006440: 7870 6572 696d 656e 7420 7265 7375 6c74  xperiment result
+00006450: 7320 746f 2074 656e 736f 7262 6f61 7264  s to tensorboard
+00006460: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00006470: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00006480: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
+00006490: 2020 2020 2020 2069 645f 3a20 7374 720d         id_: str.
+000064a0: 0a20 2020 2020 2020 2020 2020 2045 7870  .            Exp
+000064b0: 6572 696d 656e 7420 4944 2e0d 0a20 2020  eriment ID...   
+000064c0: 2020 2020 206c 6f67 5061 7468 3a20 7374       logPath: st
+000064d0: 720d 0a20 2020 2020 2020 2020 2020 2050  r..            P
+000064e0: 6174 6820 746f 2074 6865 2065 7870 6572  ath to the exper
+000064f0: 696d 656e 7420 6c6f 6773 2e0d 0a20 2020  iment logs...   
+00006500: 2020 2020 2070 6172 616d 733a 2044 6963       params: Dic
+00006510: 740d 0a20 2020 2020 2020 2020 2020 2043  t..            C
+00006520: 6f6e 6669 6775 7261 7469 6f6e 2070 6172  onfiguration par
+00006530: 616d 6574 6572 7320 6f66 2074 6865 2065  ameters of the e
+00006540: 7870 6572 696d 656e 742e 0d0a 0d0a 2020  xperiment.....  
+00006550: 2020 2020 2020 466c 6f77 733a 0d0a 2020        Flows:..  
+00006560: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
+00006570: 2020 2020 2020 312e 204c 6f61 6420 7468        1. Load th
+00006580: 6520 6265 7374 2064 6174 6120 6672 6f6d  e best data from
+00006590: 2060 6c6f 6750 6174 6860 2e0d 0a20 2020   `logPath`...   
+000065a0: 2020 2020 2032 2e20 5772 6974 6520 7468       2. Write th
+000065b0: 6520 6265 7374 2064 6174 6120 746f 2074  e best data to t
+000065c0: 656e 736f 7262 6f61 7264 2077 6974 6820  ensorboard with 
+000065d0: 6070 6172 616d 7360 2e0d 0a0d 0a20 2020  `params`.....   
+000065e0: 2020 2020 204e 6f74 6573 3a0d 0a20 2020       Notes:..   
+000065f0: 2020 2020 202d 2d2d 2d2d 2d0d 0a20 2020       ------..   
+00006600: 2020 2020 2049 6620 796f 7520 6669 6e64       If you find
+00006610: 2060 2d31 6020 6170 7065 6172 696e 6720   `-1` appearing 
+00006620: 696e 2074 6865 2074 656e 736f 7262 6f61  in the tensorboa
+00006630: 7264 2c0d 0a20 2020 2020 2020 2069 7420  rd,..        it 
+00006640: 636f 756c 6420 6d65 616e 2074 6861 7420  could mean that 
+00006650: 7468 6520 6461 7461 2069 7320 6f66 2060  the data is of `
+00006660: 7374 7260 2074 7970 652c 0d0a 2020 2020  str` type,..    
+00006670: 2020 2020 7768 6963 6820 7769 6c6c 2063      which will c
+00006680: 6175 7365 2061 6e20 6572 726f 7220 6966  ause an error if
+00006690: 2069 7420 6973 2073 656e 7420 746f 2074   it is sent to t
+000066a0: 656e 736f 7262 6f61 7264 2064 6972 6563  ensorboard direc
+000066b0: 746c 7921 0d0a 2020 2020 2020 2020 2222  tly!..        ""
+000066c0: 220d 0a20 2020 2020 2020 2074 7279 3a0d  "..        try:.
+000066d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000066e0: 6120 3d20 7365 6c66 2e6c 6f61 645f 6265  a = self.load_be
+000066f0: 7374 286c 6f67 5061 7468 290d 0a20 2020  st(logPath)..   
+00006700: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+00006710: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
+00006720: 662e 6366 672e 434f 5245 5f4c 4f47 5f50  f.cfg.CORE_LOG_P
+00006730: 4154 482c 2069 645f 290d 0a20 2020 2020  ATH, id_)..     
+00006740: 2020 2020 2020 2077 6974 6820 5375 6d6d         with Summ
+00006750: 6172 7957 7269 7465 7228 6c6f 675f 6469  aryWriter(log_di
+00006760: 723d 7061 7468 2920 6173 2077 7269 7465  r=path) as write
+00006770: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00006780: 2020 2020 6d65 7472 6963 7320 3d20 6469      metrics = di
+00006790: 6374 2829 0d0a 2020 2020 2020 2020 2020  ct()..          
+000067a0: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
+000067b0: 2c20 6265 7374 2069 6e20 6461 7461 2e69  , best in data.i
+000067c0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+000067d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000067e0: 206d 6574 7269 632c 2076 616c 2069 6e20   metric, val in 
+000067f0: 6265 7374 2e69 7465 6d73 2829 3a0d 0a20  best.items():.. 
+00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006810: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
+00006820: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+00006830: 616c 2c20 2869 6e74 2c20 666c 6f61 7429  al, (int, float)
+00006840: 2920 656c 7365 202d 310d 0a20 2020 2020  ) else -1..     
+00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 206d 6574 7269 6373 5b27 2f27 2e6a     metrics['/'.j
+00006870: 6f69 6e28 5b70 7265 6669 782c 206d 6574  oin([prefix, met
+00006880: 7269 635d 295d 203d 2076 616c 0d0a 2020  ric])] = val..  
+00006890: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+000068a0: 6974 6572 2e61 6464 5f68 7061 7261 6d73  iter.add_hparams
+000068b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000068c0: 2020 2020 2020 2070 6172 616d 732c 206d         params, m
+000068d0: 6574 7269 6373 2c0d 0a20 2020 2020 2020  etrics,..       
+000068e0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+000068f0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00006900: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
+00006910: 2020 2069 6e66 6f4c 6f67 6765 7228 0d0a     infoLogger(..
+00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006930: 6622 5c30 3333 5b30 3b33 313b 3437 6d5b  f"\033[0;31;47m[
+00006940: 4164 6170 7465 725d 203e 3e3e 2055 6e6b  Adapter] >>> Unk
+00006950: 6e6f 776e 2065 7272 6f72 7320 6861 7070  nown errors happ
+00006960: 656e 2e20 5468 6973 2069 7320 6d61 696e  en. This is main
+00006970: 6c79 2064 7565 2074 6f20 6162 6e6f 726d  ly due to abnorm
+00006980: 616c 2065 7869 7473 206f 6620 6368 696c  al exits of chil
+00006990: 6420 7072 6f63 6573 7365 732e 5c30 3333  d processes.\033
+000069a0: 5b30 6d22 0d0a 2020 2020 2020 2020 2020  [0m"..          
+000069b0: 2020 290d 0a0d 0a20 2020 2064 6566 2065    )....    def e
+000069c0: 6163 685f 6772 6964 2873 656c 6629 3a0d  ach_grid(self):.
+000069d0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
+000069e0: 2073 6561 7263 6820 666f 7220 6561 6368   search for each
+000069f0: 206b 696e 6420 6f66 2070 6172 616d 2e22   kind of param."
+00006a00: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
+00006a10: 6b65 792c 2076 616c 7320 696e 207a 6970  key, vals in zip
+00006a20: 2873 656c 662e 7061 7261 6d73 2c20 7365  (self.params, se
+00006a30: 6c66 2e76 616c 7565 7329 3a0d 0a20 2020  lf.values):..   
+00006a40: 2020 2020 2020 2020 2066 6f72 2076 616c           for val
+00006a50: 2069 6e20 7661 6c73 3a0d 0a20 2020 2020   in vals:..     
+00006a60: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00006a70: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
+00006a80: 5453 207c 207b 6b65 793a 2076 616c 7d0d  TS | {key: val}.
+00006a90: 0a0d 0a20 2020 2064 6566 2070 726f 6475  ...    def produ
+00006aa0: 6374 5f67 7269 6428 7365 6c66 293a 0d0a  ct_grid(self):..
+00006ab0: 2020 2020 2020 2020 2222 2247 7269 6420          """Grid 
+00006ac0: 7365 6172 6368 2061 6372 6f73 7320 616c  search across al
+00006ad0: 6c20 636f 6d62 696e 6174 696f 6e20 6f66  l combination of
+00006ae0: 2070 6172 616d 7322 2222 0d0a 2020 2020   params"""..    
+00006af0: 2020 2020 666f 7220 7661 6c73 2069 6e20      for vals in 
+00006b00: 7072 6f64 7563 7428 2a73 656c 662e 7661  product(*self.va
+00006b10: 6c75 6573 293a 0d0a 2020 2020 2020 2020  lues):..        
+00006b20: 2020 2020 7969 656c 6420 7365 6c66 2e63      yield self.c
+00006b30: 6667 2e44 4546 4155 4c54 5320 7c20 7b6f  fg.DEFAULTS | {o
+00006b40: 7074 696f 6e3a 7661 6c20 666f 7220 6f70  ption:val for op
+00006b50: 7469 6f6e 2c20 7661 6c20 696e 207a 6970  tion, val in zip
+00006b60: 2873 656c 662e 7061 7261 6d73 2c20 7661  (self.params, va
+00006b70: 6c73 297d 0d0a 0d0a 2020 2020 6465 6620  ls)}....    def 
+00006b80: 7361 7665 5f63 6865 636b 706f 696e 7428  save_checkpoint(
+00006b90: 7365 6c66 2c20 736f 7572 6365 3a20 4c69  self, source: Li
+00006ba0: 7374 2920 2d3e 204e 6f6e 653a 0d0a 2020  st) -> None:..  
+00006bb0: 2020 2020 2020 2222 2253 6176 6520 7468        """Save th
+00006bc0: 6520 7265 7374 206f 6620 7061 7261 6d73  e rest of params
+00006bd0: 2e22 2222 0d0a 2020 2020 2020 2020 7061  ."""..        pa
+00006be0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00006bf0: 6e28 7365 6c66 2e63 6667 2e43 4f52 455f  n(self.cfg.CORE_
+00006c00: 4348 4543 4b50 4f49 4e54 5f50 4154 482c  CHECKPOINT_PATH,
+00006c10: 2073 656c 662e 6366 672e 4348 4543 4b50   self.cfg.CHECKP
+00006c20: 4f49 4e54 5f46 494c 454e 414d 4529 0d0a  OINT_FILENAME)..
+00006c30: 2020 2020 2020 2020 6368 6563 6b70 6f69          checkpoi
+00006c40: 6e74 203d 2064 6963 7428 290d 0a20 2020  nt = dict()..   
+00006c50: 2020 2020 2063 6865 636b 706f 696e 745b       checkpoint[
+00006c60: 2773 6f75 7263 6527 5d20 3d20 736f 7572  'source'] = sour
+00006c70: 6365 0d0a 2020 2020 2020 2020 746f 7263  ce..        torc
+00006c80: 682e 7361 7665 2863 6865 636b 706f 696e  h.save(checkpoin
+00006c90: 742c 2070 6174 6829 0d0a 0d0a 2020 2020  t, path)....    
+00006ca0: 4074 696d 656d 6574 6572 2822 436f 6163  @timemeter("Coac
+00006cb0: 682f 7265 7375 6d65 2229 0d0a 2020 2020  h/resume")..    
+00006cc0: 6465 6620 6c6f 6164 5f63 6865 636b 706f  def load_checkpo
+00006cd0: 696e 7428 7365 6c66 2920 2d3e 2069 6e74  int(self) -> int
+00006ce0: 3a0d 0a20 2020 2020 2020 2022 2222 4c6f  :..        """Lo
+00006cf0: 6164 2074 6865 2072 6573 7420 6f66 2070  ad the rest of p
+00006d00: 6172 616d 732e 2222 220d 0a20 2020 2020  arams."""..     
+00006d10: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+00006d20: 5b43 6f61 6368 5d20 3e3e 3e20 4c6f 6164  [Coach] >>> Load
+00006d30: 2074 6865 2072 6563 656e 7420 6368 6563   the recent chec
+00006d40: 6b70 6f69 6e74 202e 2e2e 2229 0d0a 2020  kpoint ...")..  
+00006d50: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
+00006d60: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
+00006d70: 6667 2e43 4f52 455f 4348 4543 4b50 4f49  fg.CORE_CHECKPOI
+00006d80: 4e54 5f50 4154 482c 2073 656c 662e 6366  NT_PATH, self.cf
+00006d90: 672e 4348 4543 4b50 4f49 4e54 5f46 494c  g.CHECKPOINT_FIL
+00006da0: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
+00006db0: 6368 6563 6b70 6f69 6e74 203d 2074 6f72  checkpoint = tor
+00006dc0: 6368 2e6c 6f61 6428 7061 7468 290d 0a20  ch.load(path).. 
+00006dd0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+00006de0: 6563 6b70 6f69 6e74 5b27 736f 7572 6365  eckpoint['source
+00006df0: 275d 0d0a 0d0a 2020 2020 6465 6620 7265  ']....    def re
+00006e00: 7375 6d65 2873 656c 6629 3a0d 0a20 2020  sume(self):..   
+00006e10: 2020 2020 2022 2222 5265 7375 6d65 2066       """Resume f
+00006e20: 726f 6d20 7468 6520 7265 6365 6e74 2063  rom the recent c
+00006e30: 6865 636b 706f 696e 742e 2222 220d 0a20  heckpoint.""".. 
+00006e40: 2020 2020 2020 2073 6f75 7263 6520 3d20         source = 
+00006e50: 7365 6c66 2e65 6163 685f 6772 6964 2829  self.each_grid()
+00006e60: 2069 6620 7365 6c66 2e63 6667 2e45 5843   if self.cfg.EXC
+00006e70: 4c55 5349 5645 2065 6c73 6520 7365 6c66  LUSIVE else self
+00006e80: 2e70 726f 6475 6374 5f67 7269 6428 290d  .product_grid().
+00006e90: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
+00006ea0: 3d20 6c69 7374 2873 6f75 7263 6529 5b3a  = list(source)[:
+00006eb0: 3a2d 315d 0d0a 2020 2020 2020 2020 736f  :-1]..        so
+00006ec0: 7572 6365 203d 2073 656c 662e 6c6f 6164  urce = self.load
+00006ed0: 5f63 6865 636b 706f 696e 7428 2920 6966  _checkpoint() if
+00006ee0: 2073 656c 662e 6366 672e 7265 7375 6d65   self.cfg.resume
+00006ef0: 2065 6c73 6520 736f 7572 6365 0d0a 2020   else source..  
+00006f00: 2020 2020 2020 7265 7475 726e 2073 6f75        return sou
+00006f10: 7263 650d 0a0d 0a20 2020 2064 6566 2072  rce....    def r
+00006f20: 756e 2873 656c 662c 2063 6f6d 6d61 6e64  un(self, command
+00006f30: 3a20 7374 722c 2070 6172 616d 733a 2044  : str, params: D
+00006f40: 6963 7429 3a0d 0a20 2020 2020 2020 2022  ict):..        "
+00006f50: 2222 5374 6172 7420 6120 6e65 7720 7375  ""Start a new su
+00006f60: 6270 726f 6365 7373 2222 220d 0a20 2020  bprocess"""..   
+00006f70: 2020 2020 2069 6d70 6f72 7420 7375 6270       import subp
+00006f80: 726f 6365 7373 2c20 7368 6c65 780d 0a20  rocess, shlex.. 
+00006f90: 2020 2020 2020 2066 6f72 206f 7074 696f         for optio
+00006fa0: 6e2c 2076 616c 2069 6e20 7061 7261 6d73  n, val in params
+00006fb0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00006fc0: 2020 2020 2020 2063 6f6d 6d61 6e64 202b         command +
+00006fd0: 3d20 7365 6c66 2e67 6574 5f6f 7074 696f  = self.get_optio
+00006fe0: 6e28 6f70 7469 6f6e 2c20 7661 6c29 0d0a  n(option, val)..
+00006ff0: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
+00007000: 6572 2866 225c 3033 335b 303b 3331 3b34  er(f"\033[0;31;4
+00007010: 376d 7b63 6f6d 6d61 6e64 7d5c 3033 335b  7m{command}\033[
+00007020: 306d 2229 0d0a 2020 2020 2020 2020 7265  0m")..        re
+00007030: 7475 726e 2073 7562 7072 6f63 6573 732e  turn subprocess.
+00007040: 506f 7065 6e28 7368 6c65 782e 7370 6c69  Popen(shlex.spli
+00007050: 7428 636f 6d6d 616e 6429 290d 0a0d 0a20  t(command)).... 
+00007060: 2020 2064 6566 2077 6169 7428 7365 6c66     def wait(self
+00007070: 2c20 7461 736b 733a 204c 6973 7429 3a0d  , tasks: List):.
+00007080: 0a20 2020 2020 2020 2022 2222 5761 6974  .        """Wait
+00007090: 2075 7469 6c20 616c 6c20 7072 6f63 6573   util all proces
+000070a0: 7365 7320 7465 726d 696e 6174 652e 2222  ses terminate.""
+000070b0: 220d 0a20 2020 2020 2020 2074 6173 6b73  "..        tasks
+000070c0: 203d 205b 7461 736b 2066 6f72 2074 6173   = [task for tas
+000070d0: 6b20 696e 2074 6173 6b73 2069 6620 7461  k in tasks if ta
+000070e0: 736b 2069 7320 6e6f 7420 4e6f 6e65 5d0d  sk is not None].
+000070f0: 0a20 2020 2020 2020 2066 6f72 2070 726f  .        for pro
+00007100: 6365 7373 5f2c 2069 645f 2c20 6c6f 6750  cess_, id_, logP
+00007110: 6174 682c 2070 6172 616d 7320 696e 2074  ath, params in t
+00007120: 6173 6b73 3a0d 0a20 2020 2020 2020 2020  asks:..         
+00007130: 2020 2070 726f 6365 7373 5f2e 7761 6974     process_.wait
+00007140: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00007150: 7365 6c66 2e77 7269 7465 2869 645f 2c20  self.write(id_, 
+00007160: 6c6f 6750 6174 682c 2070 6172 616d 7329  logPath, params)
+00007170: 0d0a 0d0a 2020 2020 6465 6620 706f 6c6c  ....    def poll
+00007180: 2873 656c 662c 2074 6173 6b73 3a20 4c69  (self, tasks: Li
+00007190: 7374 293a 0d0a 2020 2020 2020 2020 2222  st):..        ""
+000071a0: 2257 6169 7420 7574 696c 2061 6e79 2070  "Wait util any p
+000071b0: 726f 6365 7373 2074 6572 6d69 6e61 7465  rocess terminate
+000071c0: 732e 2222 220d 0a20 2020 2020 2020 2064  s."""..        d
+000071d0: 6566 2069 735f 6e75 6c6c 2874 6173 6b29  ef is_null(task)
+000071e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000071f0: 6574 7572 6e20 7461 736b 2069 7320 4e6f  eturn task is No
+00007200: 6e65 0d0a 2020 2020 2020 2020 6275 6666  ne..        buff
+00007210: 6572 5f73 6f75 7263 6520 3d20 5b74 6173  er_source = [tas
+00007220: 6b5b 2d31 5d20 666f 7220 7461 736b 2069  k[-1] for task i
+00007230: 6e20 7461 736b 7320 6966 2074 6173 6b20  n tasks if task 
+00007240: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
+00007250: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00007260: 2831 2920 2320 666f 7220 756e 6971 7565  (1) # for unique
+00007270: 2069 640d 0a20 2020 2020 2020 2077 6869   id..        whi
+00007280: 6c65 206e 6f74 2061 6e79 286d 6170 2869  le not any(map(i
+00007290: 735f 6e75 6c6c 2c20 7461 736b 7329 293a  s_null, tasks)):
+000072a0: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+000072b0: 6d65 2e73 6c65 6570 2837 290d 0a20 2020  me.sleep(7)..   
+000072c0: 2020 2020 2020 2020 2062 7566 6665 725f           buffer_
+000072d0: 736f 7572 6365 203d 205b 5d0d 0a20 2020  source = []..   
+000072e0: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+000072f0: 2870 726f 6365 7373 5f2c 2069 645f 2c20  (process_, id_, 
+00007300: 6c6f 6750 6174 682c 2070 6172 616d 7329  logPath, params)
+00007310: 2069 6e20 656e 756d 6572 6174 6528 7461   in enumerate(ta
+00007320: 736b 7329 3a0d 0a20 2020 2020 2020 2020  sks):..         
+00007330: 2020 2020 2020 2069 6620 7072 6f63 6573         if proces
+00007340: 735f 2e70 6f6c 6c28 2920 6973 206e 6f74  s_.poll() is not
+00007350: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00007360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007370: 2e77 7269 7465 2869 645f 2c20 6c6f 6750  .write(id_, logP
+00007380: 6174 682c 2070 6172 616d 7329 0d0a 2020  ath, params)..  
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 7461 736b 735b 695d 203d 204e 6f6e    tasks[i] = Non
+000073b0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+000073c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000073d0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
+000073e0: 6666 6572 5f73 6f75 7263 652e 6170 7065  ffer_source.appe
+000073f0: 6e64 2870 6172 616d 7329 0d0a 2020 2020  nd(params)..    
+00007400: 2020 2020 7365 6c66 2e73 6176 655f 6368      self.save_ch
+00007410: 6563 6b70 6f69 6e74 2873 656c 662e 736f  eckpoint(self.so
+00007420: 7572 6365 202b 2062 7566 6665 725f 736f  urce + buffer_so
+00007430: 7572 6365 290d 0a20 2020 2020 2020 2072  urce)..        r
+00007440: 6574 7572 6e20 7461 736b 732e 696e 6465  eturn tasks.inde
+00007450: 7828 4e6f 6e65 290d 0a0d 0a20 2020 2064  x(None)....    d
+00007460: 6566 2074 6572 6d69 6e61 7465 2873 656c  ef terminate(sel
+00007470: 662c 2074 6173 6b73 3a20 4c69 7374 293a  f, tasks: List):
+00007480: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
+00007490: 3d20 5b74 6173 6b20 666f 7220 7461 736b  = [task for task
+000074a0: 2069 6e20 7461 736b 7320 6966 2074 6173   in tasks if tas
+000074b0: 6b20 6973 206e 6f74 204e 6f6e 655d 0d0a  k is not None]..
+000074c0: 2020 2020 2020 2020 666f 7220 7072 6f63          for proc
+000074d0: 6573 735f 2c20 5f2c 205f 2c20 5f20 696e  ess_, _, _, _ in
+000074e0: 2074 6173 6b73 3a0d 0a20 2020 2020 2020   tasks:..       
+000074f0: 2020 2020 2069 6620 7072 6f63 6573 735f       if process_
+00007500: 2e70 6f6c 6c28 2920 6973 204e 6f6e 653a  .poll() is None:
+00007510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007520: 2020 7072 6f63 6573 735f 2e74 6572 6d69    process_.termi
+00007530: 6e61 7465 2829 0d0a 2020 2020 2020 2020  nate()..        
+00007540: 7469 6d65 2e73 6c65 6570 2833 290d 0a20  time.sleep(3).. 
+00007550: 2020 2020 2020 2066 6f72 2070 726f 6365         for proce
+00007560: 7373 5f2c 205f 2c20 5f2c 205f 2069 6e20  ss_, _, _, _ in 
+00007570: 7461 736b 733a 0d0a 2020 2020 2020 2020  tasks:..        
+00007580: 2020 2020 6966 2070 726f 6365 7373 5f2e      if process_.
+00007590: 706f 6c6c 2829 2069 7320 4e6f 6e65 3a0d  poll() is None:.
+000075a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000075b0: 2070 726f 6365 7373 5f2e 6b69 6c6c 2829   process_.kill()
+000075c0: 0d0a 2020 2020 2020 2020 7379 732e 6578  ..        sys.ex
+000075d0: 6974 2829 0d0a 0d0a 2020 2020 4074 696d  it()....    @tim
+000075e0: 656d 6574 6572 2822 4164 6170 7465 722f  emeter("Adapter/
+000075f0: 6669 7422 290d 0a20 2020 2064 6566 2066  fit")..    def f
+00007600: 6974 2873 656c 6629 3a0d 0a20 2020 2020  it(self):..     
+00007610: 2020 2022 2222 4772 6964 2073 6561 7263     """Grid searc
+00007620: 682e 2222 220d 0a20 2020 2020 2020 2073  h."""..        s
+00007630: 656c 662e 736f 7572 6365 203d 2073 656c  elf.source = sel
+00007640: 662e 7265 7375 6d65 2829 0d0a 2020 2020  f.resume()..    
+00007650: 2020 2020 7461 736b 7320 3d20 5b4e 6f6e      tasks = [Non
+00007660: 6520 666f 7220 5f20 696e 2072 616e 6765  e for _ in range
+00007670: 286c 656e 2873 656c 662e 6465 7669 6365  (len(self.device
+00007680: 7329 295d 0d0a 0d0a 2020 2020 2020 2020  s))]....        
+00007690: 6465 6620 7369 676e 616c 5f68 616e 646c  def signal_handl
+000076a0: 6572 2873 6967 2c20 6672 616d 6529 3a0d  er(sig, frame):.
+000076b0: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+000076c0: 6f4c 6f67 6765 7228 6622 5c30 3333 5b30  oLogger(f"\033[0
+000076d0: 3b33 313b 3437 6d3d 3d3d 3d3d 3d3d 3d3d  ;31;47m=========
+000076e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000076f0: 3d3d 3d3d 3d3d 5445 524d 494e 4154 4520  ======TERMINATE 
+00007700: 414c 4c20 5355 4250 524f 4345 5353 4553  ALL SUBPROCESSES
+00007710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c  ===============\
+00007730: 3033 335b 306d 2229 0d0a 2020 2020 2020  033[0m")..      
+00007740: 2020 2020 2020 7365 6c66 2e74 6572 6d69        self.termi
+00007750: 6e61 7465 2874 6173 6b73 290d 0a20 2020  nate(tasks)..   
+00007760: 2020 2020 2073 6967 6e61 6c2e 7369 676e       signal.sign
+00007770: 616c 2873 6967 6e61 6c2e 5349 4749 4e54  al(signal.SIGINT
+00007780: 2c20 7369 676e 616c 5f68 616e 646c 6572  , signal_handler
+00007790: 290d 0a0d 0a20 2020 2020 2020 2074 7279  )....        try
+000077a0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
+000077b0: 6869 6c65 2073 656c 662e 736f 7572 6365  hile self.source
+000077c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000077d0: 2020 2069 6e64 6578 203d 2073 656c 662e     index = self.
+000077e0: 706f 6c6c 2874 6173 6b73 290d 0a20 2020  poll(tasks)..   
+000077f0: 2020 2020 2020 2020 2020 2020 2064 6576               dev
+00007800: 6963 6520 3d20 7365 6c66 2e64 6576 6963  ice = self.devic
+00007810: 6573 5b69 6e64 6578 5d0d 0a20 2020 2020  es[index]..     
+00007820: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00007830: 7320 3d20 7365 6c66 2e73 6f75 7263 652e  s = self.source.
+00007840: 706f 7028 290d 0a20 2020 2020 2020 2020  pop()..         
+00007850: 2020 2020 2020 2063 6f6d 6d61 6e64 2c20         command, 
+00007860: 6964 5f2c 206c 6f67 5061 7468 203d 2073  id_, logPath = s
+00007870: 656c 662e 7265 6769 7374 6572 2864 6576  elf.register(dev
+00007880: 6963 6529 0d0a 2020 2020 2020 2020 2020  ice)..          
+00007890: 2020 2020 2020 7072 6f63 6573 735f 203d        process_ =
+000078a0: 2073 656c 662e 7275 6e28 636f 6d6d 616e   self.run(comman
+000078b0: 642c 2070 6172 616d 7329 0d0a 2020 2020  d, params)..    
+000078c0: 2020 2020 2020 2020 2020 2020 7461 736b              task
+000078d0: 735b 696e 6465 785d 203d 2028 7072 6f63  s[index] = (proc
+000078e0: 6573 735f 2c20 6964 5f2c 206c 6f67 5061  ess_, id_, logPa
+000078f0: 7468 2c20 7061 7261 6d73 290d 0a20 2020  th, params)..   
+00007900: 2020 2020 2066 696e 616c 6c79 3a0d 0a20       finally:.. 
+00007910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007920: 7761 6974 2874 6173 6b73 290d 0a20 2020  wait(tasks)..   
+00007930: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00007940: 726d 696e 6174 6528 7461 736b 7329       rminate(tasks)
```

### Comparing `freerec-0.3.7/freerec/metrics.py` & `freerec-0.4.1/freerec/metrics.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/models/base.py` & `freerec-0.4.1/freerec/models/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/parser.py` & `freerec-0.4.1/freerec/parser.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec/utils.py` & `freerec-0.4.1/freerec/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.7/freerec.egg-info/PKG-INFO` & `freerec-0.4.1/freerec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.3.7
+Version: 0.4.1
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freerec-0.3.7/freerec.egg-info/SOURCES.txt` & `freerec-0.4.1/freerec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 freerec/data/datasets/sequential/__init__.py
 freerec/data/datasets/sequential/amazon.py
 freerec/data/datasets/sequential/base.py
 freerec/data/datasets/sequential/movielens.py
 freerec/data/datasets/sequential/steam.py
 freerec/data/datasets/session/__init__.py
 freerec/data/datasets/session/base.py
+freerec/data/datasets/session/diginetica.py
+freerec/data/datasets/session/yoochoose.py
 freerec/data/postprocessing/__init__.py
 freerec/data/postprocessing/base.py
 freerec/data/postprocessing/column.py
 freerec/data/postprocessing/row.py
 freerec/data/postprocessing/sampler.py
 freerec/data/postprocessing/source.py
 freerec/data/preprocessing/__init__.py
```

### Comparing `freerec-0.3.7/setup.py` & `freerec-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 requires = [
     "torchdata==0.4.1",
     "tqdm>=4.64.0",
     'scipy>=1.9.1',
-    "freeplot>=0.3.2",
+    "freeplot>=0.3.3",
     "PyYAML>=6.0",
     "tensorboard>=2.10.0",
     "psutil>=5.9.0",
     "prettytable>=3.4.1"
 ]
```

