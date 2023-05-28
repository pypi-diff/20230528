# Comparing `tmp/coba-6.4.2.tar.gz` & `tmp/coba-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\coba-6.4.2.tar", last modified: Thu Apr  6 14:58:16 2023, max compression
+gzip compressed data, was "dist\coba-6.5.0.tar", last modified: Sun May 28 19:12:44 2023, max compression
```

## Comparing `coba-6.4.2.tar` & `coba-6.5.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/
--rw-rw-rw-   0        0        0       40 2021-11-14 20:00:02.000000 coba-6.4.2/AUTHORS
--rw-rw-rw-   0        0        0     1593 2021-11-14 20:00:02.000000 coba-6.4.2/LICENSE
--rw-rw-rw-   0        0        0     7956 2023-04-06 14:58:16.000000 coba-6.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     7336 2023-02-22 16:34:05.000000 coba-6.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/
--rw-rw-rw-   0        0        0     1996 2023-02-22 16:34:05.000000 coba-6.4.2/coba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/backports/
--rw-rw-rw-   0        0        0      222 2022-11-27 17:52:42.000000 coba-6.4.2/coba/backports/__init__.py
--rw-rw-rw-   0        0        0      473 2022-04-27 16:17:38.000000 coba-6.4.2/coba/backports/metadata.py
--rw-rw-rw-   0        0        0      143 2022-11-27 17:52:42.000000 coba-6.4.2/coba/backports/typing.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/contexts/
--rw-rw-rw-   0        0        0     1035 2023-04-05 17:51:59.000000 coba-6.4.2/coba/contexts/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-02-22 16:34:05.000000 coba-6.4.2/coba/contexts/cachers.py
--rw-rw-rw-   0        0        0     9263 2023-03-15 01:44:54.000000 coba-6.4.2/coba/contexts/core.py
--rw-rw-rw-   0        0        0     9715 2023-04-05 18:41:31.000000 coba-6.4.2/coba/contexts/loggers.py
--rw-rw-rw-   0        0        0    15634 2022-12-02 22:43:08.000000 coba-6.4.2/coba/encodings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/environments/
--rw-rw-rw-   0        0        0     2286 2023-02-22 15:59:12.000000 coba-6.4.2/coba/environments/__init__.py
--rw-rw-rw-   0        0        0    21561 2023-04-05 17:27:30.000000 coba-6.4.2/coba/environments/core.py
--rw-rw-rw-   0        0        0    44618 2023-03-15 01:38:26.000000 coba-6.4.2/coba/environments/filters.py
--rw-rw-rw-   0        0        0    14316 2023-02-22 16:34:05.000000 coba-6.4.2/coba/environments/openml.py
--rw-rw-rw-   0        0        0     8220 2023-03-11 23:39:33.000000 coba-6.4.2/coba/environments/primitives.py
--rw-rw-rw-   0        0        0     2598 2023-02-22 16:34:05.000000 coba-6.4.2/coba/environments/serialized.py
--rw-rw-rw-   0        0        0    10122 2023-02-22 16:34:56.000000 coba-6.4.2/coba/environments/supervised.py
--rw-rw-rw-   0        0        0    24193 2023-02-22 15:59:12.000000 coba-6.4.2/coba/environments/synthetics.py
--rw-rw-rw-   0        0        0     6179 2023-04-05 19:12:23.000000 coba-6.4.2/coba/environments/templates.py
--rw-rw-rw-   0        0        0     1126 2022-04-27 16:17:38.000000 coba-6.4.2/coba/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/experiments/
--rw-rw-rw-   0        0        0      859 2023-01-14 22:42:57.000000 coba-6.4.2/coba/experiments/__init__.py
--rw-rw-rw-   0        0        0     9404 2023-04-05 18:43:13.000000 coba-6.4.2/coba/experiments/core.py
--rw-rw-rw-   0        0        0     9302 2023-04-05 19:38:54.000000 coba-6.4.2/coba/experiments/process.py
--rw-rw-rw-   0        0        0    52988 2023-04-05 18:54:33.000000 coba-6.4.2/coba/experiments/results.py
--rw-rw-rw-   0        0        0    25294 2023-03-15 01:58:08.000000 coba-6.4.2/coba/experiments/tasks.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/learners/
--rw-rw-rw-   0        0        0     1120 2023-02-22 16:34:05.000000 coba-6.4.2/coba/learners/__init__.py
--rw-rw-rw-   0        0        0     6453 2023-03-15 01:04:42.000000 coba-6.4.2/coba/learners/bandit.py
--rw-rw-rw-   0        0        0     7801 2023-02-22 16:34:05.000000 coba-6.4.2/coba/learners/corral.py
--rw-rw-rw-   0        0        0     4757 2023-04-05 18:54:39.000000 coba-6.4.2/coba/learners/linucb.py
--rw-rw-rw-   0        0        0    14794 2023-03-01 23:52:04.000000 coba-6.4.2/coba/learners/primitives.py
--rw-rw-rw-   0        0        0    30352 2023-03-15 02:33:32.000000 coba-6.4.2/coba/learners/vowpal.py
--rw-rw-rw-   0        0        0     4277 2023-03-15 01:43:39.000000 coba-6.4.2/coba/multiprocessing.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/pipes/
--rw-rw-rw-   0        0        0     2394 2023-02-22 16:34:05.000000 coba-6.4.2/coba/pipes/__init__.py
--rw-rw-rw-   0        0        0     1902 2023-02-22 16:34:05.000000 coba-6.4.2/coba/pipes/core.py
--rw-rw-rw-   0        0        0    15360 2023-02-25 19:41:52.000000 coba-6.4.2/coba/pipes/filters.py
--rw-rw-rw-   0        0        0    14945 2023-03-01 23:34:22.000000 coba-6.4.2/coba/pipes/multiprocessing.py
--rw-rw-rw-   0        0        0     6622 2023-02-22 16:34:05.000000 coba-6.4.2/coba/pipes/primitives.py
--rw-rw-rw-   0        0        0    13017 2023-02-22 16:00:21.000000 coba-6.4.2/coba/pipes/readers.py
--rw-rw-rw-   0        0        0    18680 2023-02-22 16:34:05.000000 coba-6.4.2/coba/pipes/rows.py
--rw-rw-rw-   0        0        0     3734 2023-03-01 23:34:22.000000 coba-6.4.2/coba/pipes/sinks.py
--rw-rw-rw-   0        0        0     6154 2023-03-01 23:34:22.000000 coba-6.4.2/coba/pipes/sources.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba/primitives/
--rw-rw-rw-   0        0        0      870 2023-03-11 21:43:20.000000 coba-6.4.2/coba/primitives/__init__.py
--rw-rw-rw-   0        0        0      930 2022-12-13 14:59:41.000000 coba-6.4.2/coba/primitives/feedbacks.py
--rw-rw-rw-   0        0        0     6432 2023-03-11 21:54:59.000000 coba-6.4.2/coba/primitives/rewards.py
--rw-rw-rw-   0        0        0     4425 2023-02-22 16:34:05.000000 coba-6.4.2/coba/primitives/rows.py
--rw-rw-rw-   0        0        0      234 2022-12-13 01:57:20.000000 coba-6.4.2/coba/primitives/semantic.py
--rw-rw-rw-   0        0        0      556 2023-02-22 16:34:05.000000 coba-6.4.2/coba/primitives/types.py
--rw-rw-rw-   0        0        0    10887 2023-03-12 00:39:45.000000 coba-6.4.2/coba/random.py
--rw-rw-rw-   0        0        0     1405 2023-02-22 15:59:12.000000 coba-6.4.2/coba/register.py
--rw-rw-rw-   0        0        0    10657 2022-05-30 19:08:09.000000 coba-6.4.2/coba/registry.py
--rw-rw-rw-   0        0        0     7199 2023-03-01 23:34:22.000000 coba-6.4.2/coba/statistics.py
--rw-rw-rw-   0        0        0     4504 2023-01-14 22:42:57.000000 coba-6.4.2/coba/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/
--rw-rw-rw-   0        0        0     7956 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1466 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-06 14:58:16.000000 coba-6.4.2/coba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 14:58:16.000000 coba-6.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1273 2023-04-06 14:28:50.000000 coba-6.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/
+-rw-rw-rw-   0        0        0       40 2023-05-11 00:41:22.000000 coba-6.5.0/AUTHORS
+-rw-rw-rw-   0        0        0     1593 2023-05-11 00:41:22.000000 coba-6.5.0/LICENSE
+-rw-rw-rw-   0        0        0     7933 2023-05-28 19:12:44.000000 coba-6.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7336 2023-05-11 00:41:22.000000 coba-6.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/
+-rw-rw-rw-   0        0        0     2406 2023-05-24 18:06:29.000000 coba-6.5.0/coba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/backports/
+-rw-rw-rw-   0        0        0      222 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/metadata.py
+-rw-rw-rw-   0        0        0      143 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/contexts/
+-rw-rw-rw-   0        0        0     1035 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/cachers.py
+-rw-rw-rw-   0        0        0     9263 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/core.py
+-rw-rw-rw-   0        0        0     9726 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/loggers.py
+-rw-rw-rw-   0        0        0    15634 2023-05-11 00:41:22.000000 coba-6.5.0/coba/encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/environments/
+-rw-rw-rw-   0        0        0     2317 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/__init__.py
+-rw-rw-rw-   0        0        0    22278 2023-05-15 01:59:07.000000 coba-6.5.0/coba/environments/core.py
+-rw-rw-rw-   0        0        0    50314 2023-05-28 18:39:49.000000 coba-6.5.0/coba/environments/filters.py
+-rw-rw-rw-   0        0        0    14343 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/openml.py
+-rw-rw-rw-   0        0        0     7792 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/primitives.py
+-rw-rw-rw-   0        0        0     3014 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/serialized.py
+-rw-rw-rw-   0        0        0     9630 2023-05-18 00:29:59.000000 coba-6.5.0/coba/environments/supervised.py
+-rw-rw-rw-   0        0        0    24199 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/synthetics.py
+-rw-rw-rw-   0        0        0     6179 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/templates.py
+-rw-rw-rw-   0        0        0     1126 2023-05-11 00:41:22.000000 coba-6.5.0/coba/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/experiments/
+-rw-rw-rw-   0        0        0     1050 2023-05-14 20:33:18.000000 coba-6.5.0/coba/experiments/__init__.py
+-rw-rw-rw-   0        0        0     9556 2023-05-12 13:18:19.000000 coba-6.5.0/coba/experiments/core.py
+-rw-rw-rw-   0        0        0     9312 2023-05-11 00:41:22.000000 coba-6.5.0/coba/experiments/process.py
+-rw-rw-rw-   0        0        0    52540 2023-05-19 22:26:08.000000 coba-6.5.0/coba/experiments/results.py
+-rw-rw-rw-   0        0        0    39708 2023-05-28 18:57:52.000000 coba-6.5.0/coba/experiments/tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/learners/
+-rw-rw-rw-   0        0        0     1155 2023-05-24 18:07:17.000000 coba-6.5.0/coba/learners/__init__.py
+-rw-rw-rw-   0        0        0     7907 2023-05-11 00:41:22.000000 coba-6.5.0/coba/learners/bandit.py
+-rw-rw-rw-   0        0        0     8055 2023-05-24 19:10:26.000000 coba-6.5.0/coba/learners/corral.py
+-rw-rw-rw-   0        0        0     5010 2023-05-11 00:41:22.000000 coba-6.5.0/coba/learners/linucb.py
+-rw-rw-rw-   0        0        0     4376 2023-05-27 01:06:49.000000 coba-6.5.0/coba/learners/primitives.py
+-rw-rw-rw-   0        0        0     9021 2023-05-26 14:25:09.000000 coba-6.5.0/coba/learners/safety.py
+-rw-rw-rw-   0        0        0    30752 2023-05-28 18:41:36.000000 coba-6.5.0/coba/learners/vowpal.py
+-rw-rw-rw-   0        0        0     4288 2023-05-11 00:41:22.000000 coba-6.5.0/coba/multiprocessing.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/pipes/
+-rw-rw-rw-   0        0        0     2378 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-05-15 13:57:18.000000 coba-6.5.0/coba/pipes/core.py
+-rw-rw-rw-   0        0        0    15589 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/filters.py
+-rw-rw-rw-   0        0        0    15095 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/multiprocessing.py
+-rw-rw-rw-   0        0        0     6622 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/primitives.py
+-rw-rw-rw-   0        0        0    13003 2023-05-18 00:30:21.000000 coba-6.5.0/coba/pipes/readers.py
+-rw-rw-rw-   0        0        0    18327 2023-05-18 00:32:45.000000 coba-6.5.0/coba/pipes/rows.py
+-rw-rw-rw-   0        0        0     3734 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/sinks.py
+-rw-rw-rw-   0        0        0     6115 2023-05-12 03:29:30.000000 coba-6.5.0/coba/pipes/sources.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/primitives/
+-rw-rw-rw-   0        0        0      928 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/feedbacks.py
+-rw-rw-rw-   0        0        0     6745 2023-05-26 03:19:33.000000 coba-6.5.0/coba/primitives/rewards.py
+-rw-rw-rw-   0        0        0     4425 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/rows.py
+-rw-rw-rw-   0        0        0      234 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/semantic.py
+-rw-rw-rw-   0        0        0      657 2023-05-16 05:30:40.000000 coba-6.5.0/coba/primitives/types.py
+-rw-rw-rw-   0        0        0    11036 2023-05-13 00:19:56.000000 coba-6.5.0/coba/random.py
+-rw-rw-rw-   0        0        0     1405 2023-05-11 00:41:22.000000 coba-6.5.0/coba/register.py
+-rw-rw-rw-   0        0        0    10657 2023-05-11 00:41:22.000000 coba-6.5.0/coba/registry.py
+-rw-rw-rw-   0        0        0     8417 2023-05-11 00:41:22.000000 coba-6.5.0/coba/statistics.py
+-rw-rw-rw-   0        0        0     4594 2023-05-11 00:41:22.000000 coba-6.5.0/coba/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/
+-rw-rw-rw-   0        0        0     7933 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1490 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:12:44.000000 coba-6.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2023-05-28 19:09:21.000000 coba-6.5.0/setup.py
```

### Comparing `coba-6.4.2/LICENSE` & `coba-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/PKG-INFO` & `coba-6.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 6.4.2
+Version: 6.5.0
 Summary: A contextual bandit research package.
 Home-page: https://github.com/VowpalWabbit/coba
 Author: Mark Rucker
 Author-email: rucker.mark@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -97,9 +96,7 @@
  ## Results
 
  The end result of an Experiment is a Result object which has been built for easy analysis. The result class provides a number of plots as well as filtering capabilities out of the box. If the built in functionality isn't advanced enough data from experiments can be accesed directly from a three table structure: a Learner table, Environment table, and Interaction table. These tables can be ported to pandas dataframes where all manner of advanced filtering and plotting can be performed to discover the strengths and weaknesses of Learners on various Environments.
 
  ## Examples
 
  An examples directory is included in the repository with a number of code and experiment demonstrations. These examples show how to create experiments, evaluate learners against them and plot the results.
-
-
```

### Comparing `coba-6.4.2/README.md` & `coba-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/__init__.py` & `coba-6.5.0/coba/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from coba.contexts     import CobaContext, NullLogger
 from coba.environments import Environments, ArffSource, CsvSource, LibSvmSource, ManikSource
 from coba.environments import SimulatedInteraction, LoggedInteraction, GroundedInteraction, LambdaSimulation
 from coba.experiments  import Experiment, Result, SimpleEvaluation, SimpleLearnerInfo, SimpleEnvironmentInfo
+from coba.experiments  import ExplorationEvaluation, OnPolicyEvaluation, OffPolicyEvaluation
 
 from coba.random import CobaRandom
 
+from coba.learners.primitives import Learner
+from coba.learners.safety import SafeLearner
 from coba.learners.bandit import EpsilonBanditLearner, UcbBanditLearner, FixedLearner, RandomLearner
 from coba.learners.corral import CorralLearner
-from coba.learners.vowpal import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner
+from coba.learners.vowpal import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner, VowpalRndLearner
 from coba.learners.vowpal import VowpalCoverLearner, VowpalRegcbLearner, VowpalSquarecbLearner, VowpalOffPolicyLearner
 from coba.learners.linucb import LinUCBLearner
 
+from coba.utilities import peek_first
+
 from coba.exceptions import CobaException
 
 from coba.backports import version, PackageNotFoundError
 
 try:
     #Option (5) on https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
     __version__ = version('coba') 
@@ -37,23 +42,30 @@
     'VowpalEpsilonLearner',
     'VowpalSoftmaxLearner',
     'VowpalBagLearner',
     'VowpalCoverLearner',
     'VowpalRegcbLearner',
     'VowpalSquarecbLearner',
     'VowpalOffPolicyLearner',
+    'VowpalRndLearner',
     'OnlineGroundedEval',
     'OnlineOnPolicyEval',
     'CobaRandom',
     'NullLogger',
     'ArffSource',
     'CsvSource',
     'LibSvmSource',
     'ManikSource',
     'SimulatedInteraction',
     'LoggedInteraction',
     'GroundedInteraction',
     'SimpleEvaluation', 
     'SimpleLearnerInfo', 
     'SimpleEnvironmentInfo',
-    'LambdaSimulation'
+    'LambdaSimulation',
+    'Learner',
+    'SafeLearner',
+    'ExplorationEvaluation',
+    'OnPolicyEvaluation',
+    'OffPolicyEvaluation',
+    'peek_first'
 ]
```

### Comparing `coba-6.4.2/coba/contexts/__init__.py` & `coba-6.5.0/coba/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/contexts/cachers.py` & `coba-6.5.0/coba/contexts/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/contexts/core.py` & `coba-6.5.0/coba/contexts/core.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/contexts/loggers.py` & `coba-6.5.0/coba/contexts/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,12 +291,12 @@
 class ExceptLog(Filter[Union[str,Exception],str]):
     """A Log decorator that turns exceptions into messages."""
 
     def filter(self, log: Union[str,Exception]) -> str:
         if isinstance(log, str):
             return log
         elif isinstance(log, CobaException):
-            return str(log)
+            return f"EXCEPTION: {log}"
         else:
             tb  = ''.join(traceback.format_tb(log.__traceback__))
             msg = ''.join(traceback.TracebackException.from_exception(log).format_exception_only())
             return f"Unexpected exception:\n\n{tb}\n  {msg}"
```

### Comparing `coba-6.4.2/coba/encodings.py` & `coba-6.5.0/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/environments/__init__.py` & `coba-6.5.0/coba/environments/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from coba.environments.core       import Environments
 from coba.environments.primitives import Interaction, Environment, SafeEnvironment, EnvironmentFilter
 from coba.environments.primitives import SimulatedInteraction, LoggedInteraction, GroundedInteraction
 from coba.environments.filters    import Shuffle, Take, Identity, Reservoir, Riffle, Cache
 from coba.environments.filters    import Sort, Scale, Cycle, Impute, Flatten, Params
-from coba.environments.filters    import Binary, Sparse, Where, Noise, Grounded
+from coba.environments.filters    import Binary, Sparse, Where, Noise, Grounded, OpeRewards
 from coba.environments.filters    import Repr, Finalize, Batch, BatchSafe, Chunk, Logged
 
 from coba.environments.synthetics import LambdaSimulation, LinearSyntheticSimulation, NeighborsSyntheticSimulation
 from coba.environments.synthetics import KernelSyntheticSimulation, MLPSyntheticSimulation
 from coba.environments.openml     import OpenmlSimulation, OpenmlSource
 from coba.environments.supervised import SupervisedSimulation, CsvSource, ArffSource, LibSvmSource, ManikSource
 
@@ -57,9 +57,10 @@
     'Cache',
     'Grounded',
     'Finalize',
     'Repr',
     'Batch',
     'BatchSafe',
     'Chunk',
-    'Logged'
+    'Logged',
+    'OpeRewards'
 ]
```

### Comparing `coba-6.4.2/coba/environments/core.py` & `coba-6.5.0/coba/environments/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,50 +6,49 @@
 from coba.backports import Literal
 
 from coba                 import pipes
 from coba.contexts        import CobaContext, DiskCacher, DecoratedLogger, ExceptLog, NameLog, StampLog
 from coba.pipes.sources   import DataFrameSource
 from coba.primitives      import Context, Action
 from coba.random          import CobaRandom
-from coba.pipes           import Pipes, Source, HttpSource, IterableSource, JsonDecode, Foreach
+from coba.pipes           import Pipes, Source, HttpSource, IterableSource, JsonDecode
 from coba.exceptions      import CobaException
 from coba.multiprocessing import CobaMultiprocessor
 from coba.learners        import Learner
 
 from coba.environments.primitives import Environment
 
 from coba.environments.templates  import EnvironmentsTemplateV1, EnvironmentsTemplateV2
 from coba.environments.openml     import OpenmlSimulation
 from coba.environments.synthetics import LinearSyntheticSimulation, NeighborsSyntheticSimulation
 from coba.environments.synthetics import KernelSyntheticSimulation, MLPSyntheticSimulation, LambdaSimulation
 from coba.environments.supervised import SupervisedSimulation
 
-
 from coba.environments.filters   import EnvironmentFilter, Repr, Batch, Chunk, Logged, Finalize, BatchSafe
 from coba.environments.filters   import Binary, Shuffle, Take, Sparse, Reservoir, Cycle, Scale, Unbatch, Slice
 from coba.environments.filters   import Impute, Where, Noise, Riffle, Sort, Flatten, Cache, Params, Grounded
-from coba.environments.filters   import MappingToInteraction
+from coba.environments.filters   import MappingToInteraction, OpeRewards
 
 from coba.environments.serialized import EnvironmentFromObjects, EnvironmentsToObjects, ZipMemberToObjects, ObjectsToZipMember
 
 class Environments(collections.abc.Sequence, Sequence[Environment]):
     """A friendly wrapper around commonly used environment functionality."""
 
     @staticmethod
     def cache_dir(path:Union[str,Path]) -> Type['Environments']:
         CobaContext.cacher = DiskCacher(path)
         return Environments
 
     @overload
     @staticmethod
-    def from_template(filesource:Source[Iterable[str]]) -> 'Environments': ...
+    def from_template(filesource:Source[Iterable[str]], **user_vars) -> 'Environments': ...
 
     @overload
     @staticmethod
-    def from_template(fileurl:str) -> 'Environments': ...
+    def from_template(fileurl:str, **user_vars) -> 'Environments': ...
 
     @staticmethod
     def from_template(arg, **user_vars) -> 'Environments':
         """Instantiate Environments from an environment template file with user defined variables."""
         try:
             return Environments(*EnvironmentsTemplateV2(arg, **user_vars).read())
         except Exception as e: #pragma: no cover
@@ -159,23 +158,25 @@
 
     @overload
     @staticmethod
     def from_openml(data_id: Union[int,Sequence[int]],
         drop_missing: bool = True,
         take: int = None,
         *,
-        target:str = None) -> 'Environments':
+        target:str = None,
+        label_type:Literal['c','r','m'] = None) -> 'Environments':
         ...
 
     @overload
     @staticmethod
     def from_openml(*,task_id: Union[int,Sequence[int]],
         drop_missing: bool = True,
         take: int = None,
-        target:str = None) -> 'Environments':
+        target:str = None,
+        label_type:Literal['m','c','r'] = None) -> 'Environments':
         ...
 
     @staticmethod
     def from_openml(*args,**kwargs) -> 'Environments':
         """Create a SimulatedEnvironment from datasets available on openml."""
 
         kwargs.update(zip(['data_id','drop_missing','take'], args))
@@ -213,16 +214,18 @@
     @staticmethod
     def from_supervised(*args, **kwargs) -> 'Environments':
         """Create a SimulatedEnvironment from a supervised dataset"""
         return Environments(SupervisedSimulation(*args, **kwargs))
 
     @staticmethod
     def from_save(path:str) -> 'Environments':
-        make = lambda m: EnvironmentFromObjects(ZipMemberToObjects(path,m))
-        return Environments(list(map(make,ZipFile(path).namelist())))
+        envs = []
+        for name in ZipFile(path).namelist():
+            envs.append(EnvironmentFromObjects(ZipMemberToObjects(path,name)))
+        return Environments(envs)
 
     @overload
     def from_lambda(self,
         n_interactions: Optional[int],
         context       : Callable[[int               ],Context         ],
         actions       : Callable[[int,Context       ],Sequence[Action]],
         reward        : Callable[[int,Context,Action],float           ]) -> 'Environments':
@@ -321,23 +324,23 @@
         """Take a fixed number of interactions from the Environments."""
         return self.filter(Take(n_interactions))
     
     def slice(self, start: Optional[int], stop: Optional[int]=None, step:int = 1) -> 'Environments':
         """Take a slice of interactions from an Environment."""
         return self.filter(Slice(start,stop,step))
 
-    def reservoir(self, n_interactions: int, seeds: Union[int,Sequence[int]]) -> 'Environments':
+    def reservoir(self, n_interactions: int, seeds: Union[int,Sequence[int]]=1) -> 'Environments':
         """Take a random fixed number of interactions from the Environments."""
         if isinstance(seeds,int): seeds = [seeds]
         return self.filter([Reservoir(n_interactions,seed) for seed in seeds])
 
     def scale(self,
         shift: Union[float,Literal["min","mean","med"]] = "min",
         scale: Union[float,Literal["minmax","std","iqr","maxabs"]] = "minmax",
-        targets: Union[Literal["context","rewards","argmax"], Sequence[Literal["context","rewards","argmax"]]] = "context",
+        targets: Union[Literal["context","ope_rewards","argmax"], Sequence[Literal["context","ope_rewards","argmax"]]] = "context",
         using: Optional[int] = None) -> 'Environments':
         """Apply an affine shift and scaling factor to precondition environments."""
         if isinstance(targets,str): targets = [targets]
         return self.filter(Pipes.join(*[Scale(shift, scale, t, using) for t in targets]))
 
     def impute(self,
         stats: Union[Literal["mean","median","mode"],Sequence[Literal["mean","median","mode"]]] = "mean",
@@ -366,16 +369,24 @@
         """Flatten environment's context and actions."""
         return self.filter(Flatten())
 
     def materialize(self) -> 'Environments':
         """Materialize the environments in memory. Ideal for stateful environments such as Jupyter Notebook."""
         #we use pipes.cache directly because the environment cache will copy 
         #which we don't need when we materialize an environment in memory
-        envs = Environments([Pipes.join(env, pipes.Cache(25)) for env in self])
+        envs = Environments([Pipes.join(env, Finalize(apply_repr=False), pipes.Cache(25,True)) for env in self])
+        
         for env in envs: list(env.read()) #force read to pre-load cache
+            
+        for env in envs:
+            for i in range(len(env)-1):
+                pipe = env[i]
+                if isinstance(pipe, pipes.Cache) and not pipe._protected:
+                    pipe._cache = None
+
         return envs
 
     def grounded(self, n_users: int, n_normal:int, n_words:int, n_good:int, seed:int=1) -> 'Environments':
         """Convert from simulated environments to interaction grounded environments."""
         return self.filter(Grounded(n_users, n_normal, n_words, n_good, seed))
 
     def repr(self, 
@@ -389,23 +400,27 @@
         return self.filter(Batch(batch_size))
 
     def chunk(self, cache:bool = True) -> 'Environments':
         """Create a chunk point in the environments pipeline to compose how multiprocess is conducted."""
         envs = Environments([Pipes.join(env, Chunk()) for env in self])
         return envs.cache() if cache else envs
 
-    def logged(self, learners: Union[Learner,Sequence[Learner]], rewards:Literal["DM","IPS"] = "DM", seed:float = 1.23) -> 'Environments':
+    def logged(self, learners: Union[Learner,Sequence[Learner]], seed:Optional[float] = 1.23) -> 'Environments':
         """Create a logged environment using the given learner for the logging policy."""
         if not isinstance(learners, collections.abc.Sequence): learners = [learners]
-        return self.filter(BatchSafe(Finalize())).filter([Logged(learner, rewards, seed) for learner in learners ])
+        return self.filter(BatchSafe(Finalize())).filter([Logged(learner, seed) for learner in learners ])
 
     def unbatch(self):
         """Unbatch interactions in the environments."""
         return self.filter(Unbatch())
 
+    def ope_rewards(self, rewards_type:Literal['IPS','DM','DR','NO'] = None):
+        """Reward estimates for off-policy evaluation."""
+        return self.filter(OpeRewards(rewards_type))
+
     def save(self, path: str, processes:int=1, overwrite:bool=False) -> 'Environments':
 
         self_envs = list(self)
 
         if Path(path).exists():
             try:
                 path_envs   = Environments.from_save(path)
@@ -425,38 +440,41 @@
 
                 if is_equal and not self_envs:
                     return path_envs
                 if not is_equal and overwrite:
                     Path(path).unlink()
                 if not is_equal and not overwrite:
                     raise CobaException("The Environments save file does not match the actual Environments and overwite is False.")
-            
+
             except BadZipFile:
                 if overwrite:
                     Path(path).unlink()
                 else:
                     raise CobaException("The given save file appears to be corrupted. Please check it and delete if it is unusable.")
 
         CobaContext.logger = DecoratedLogger([ExceptLog()], CobaContext.logger, [StampLog()] if processes ==1 else [NameLog(), StampLog()])
         Pipes.join(IterableSource(self_envs),CobaMultiprocessor(EnvironmentsToObjects(),processes),ObjectsToZipMember(path)).run()
         CobaContext.logger = CobaContext.logger.undecorate()
-        
+
         return Environments.from_save(path)
 
     def cache(self) -> 'Environments':
         """Create a cache point in the environments so that earlier steps in the pipeline can be re-used in several pipes."""
         return Environments([Pipes.join(env, Cache(25)) for env in self])
 
     def filter(self, filter: Union[EnvironmentFilter,Sequence[EnvironmentFilter]]) -> 'Environments':
         """Apply filters to each environment currently in Environments."""
         filters = filter if isinstance(filter, collections.abc.Sequence) else [filter]
         return Environments([Pipes.join(e,f) for e in self._environments for f in filters])
 
-    def __getitem__(self, index:int) -> Environment:
-        return self._environments[index]
+    def __getitem__(self, index:Any) -> Union[Environment,'Environments']:
+        if isinstance(index,slice):
+            return Environments(self._environments[index])
+        else:
+            return self._environments[index]
 
     def __iter__(self) -> Iterator[Environment]:
         return iter(self._environments)
 
     def __len__(self) -> int:
         return len(self._environments)
```

### Comparing `coba-6.4.2/coba/environments/filters.py` & `coba-6.5.0/coba/environments/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from typing import Optional, Sequence, Union, Iterable, Any, Tuple, Callable, Mapping
 from coba.backports import Literal
 
 from coba            import pipes, primitives
 from coba.random     import CobaRandom
 from coba.exceptions import CobaException
 from coba.statistics import iqr
-from coba.contexts   import CobaContext
-from coba.utilities  import peek_first
-from coba.primitives import ScaleReward, BinaryReward, SequenceReward, BatchReward, IPSReward
+from coba.utilities  import peek_first, PackageChecker
+from coba.primitives import ScaleReward, BinaryReward, SequenceReward, BatchReward
+from coba.primitives import IPSReward, SequenceFeedback, MappingReward, MulticlassReward
 from coba.primitives import Feedback, BatchFeedback
 from coba.learners   import Learner, SafeLearner
 from coba.pipes      import Filter
 
 from coba.environments.primitives import EnvironmentFilter, Interaction
 
 class Identity(pipes.Identity, EnvironmentFilter):
@@ -36,32 +36,42 @@
 
 class Slice(pipes.Slice, EnvironmentFilter):
     """Take a slice of interactions from an Environment."""
     pass
 
 class Shuffle(pipes.Shuffle, EnvironmentFilter):
     """Shuffle a sequence of Interactions in an Environment."""
-    
+
     def filter(self, interactions: Iterable[Interaction]) -> Sequence[Any]:
         first, interactions = peek_first(interactions)
 
-        if 'action' in first and 'reward' in first:
-            #this is here because otherwise offpolicy evaluation can give a
+        if not interactions:
+            yield from []
+
+        elif 'action' in first and 'reward' in first:
+            #this is here because if it is not offpolicy evaluation can give a
             #very biased estimate when seeds are the same. To see this run.
                 # import numpy as np
                 # from coba import CobaRandom
 
                 # N    = 1_000_000
                 # seed = 9
 
                 # R1 = CobaRandom(seed).randoms(N)
                 # R2 = CobaRandom(seed).shuffle(R1)
 
                 # np.corrcoef(R1,R2)
-            yield from CobaRandom("AB").shuffle(list(super().filter(interactions)))
+
+            old_seed = self._seed
+            new_seed = self._seed * 3.21 if self._seed is not None else self._seed
+
+            self._seed = new_seed
+            yield from super().filter(interactions)
+            self._seed = old_seed
+
         else:
             yield from super().filter(interactions)
 
 class Reservoir(pipes.Reservoir, EnvironmentFilter):
     """Take a fixed number of random Interactions from an Environment."""
     pass
 
@@ -146,15 +156,15 @@
                 for k in context.keys()-unscalable_cols:
                     unscaled[k].append(context[k])
 
         elif self._target == "context" and is_value_context:
             unscaled = [interaction['context'] for interaction in fitting_interactions]
 
         elif self._target == "rewards" and is_discrete:
-            rwd_vals = lambda i: list(map(i['rewards'].eval,range(len(i['actions']))))
+            rwd_vals = lambda i: list(map(i['rewards'].eval,i['actions']))
             unscaled = sum(list(map(rwd_vals,fitting_interactions)),[])
 
         elif self._target == "rewards" and not is_discrete:
             unscaled = []
 
         elif self._target == "argmax":
             unscaled = [interaction['rewards'].argmax() for interaction in fitting_interactions]
@@ -357,15 +367,15 @@
         if is_dense:
             imputations = {}
             impute_binary = {}
             for i, col in zip(imputable_cols,unimputed):
                 imputation = self._get_imputation(col)
                 if imputation is not None:
                     imputations[i] = imputation
-                    if self._miss and any([c is None for c in col]): 
+                    if self._miss and any([c is None for c in col]):
                         impute_binary[i] = len(impute_binary)
 
         elif is_sparse:
             imputations = {}
             impute_binary = {}
             binary_template = {}
             for k,col in unimputed.items():
@@ -395,23 +405,23 @@
                             is_missing[impute_binary[k]] = 1
                 context += is_missing
 
             elif is_sparse:
 
                 is_missing = binary_template.copy()
                 for k,v in context.items():
-                    if v is None: 
+                    if v is None:
                         context[k] = imputations[k]
                         if k in impute_binary:
                             is_missing[impute_binary[k]] = 1
                 context.update(is_missing)
 
             elif is_value:
                 if impute_binary:
-                    if context is None: 
+                    if context is None:
                         interaction["context"] = [imputations,1]
                     else:
                         interaction["context"] = [context,0]
                 else:
                     if context is None:
                         interaction["context"] = imputations
 
@@ -473,17 +483,17 @@
                 new['action'] = self._make_sparse(new['action'],action_has_headers, 'action')
 
             yield new
 
     def _make_sparse(self, value, has_headers:bool, default_header:str) -> Optional[dict]:
         if value is None:
             return value
-        if isinstance(value,primitives.Dense): 
+        if isinstance(value,primitives.Dense):
             value_list = list(value)
-            return {k:value_list[i] for k,i in value.headers.items() if i < len(value_list)} if has_headers else dict(enumerate(value))
+            return {k:value_list[i] for k,i in value.headers.items() if i < len(value_list) and value_list[i] != 0} if has_headers else {k:v for k,v in enumerate(value) if v != 0 }
         if isinstance(value,primitives.Sparse):
             return value
         return {default_header:value}
 
 class Cycle(EnvironmentFilter):
     """Cycle all rewards associated with actions by one place.
 
@@ -518,24 +528,26 @@
             n_actions  = len(action_set)
 
             onehot_actions  = {tuple([0]*n+[1]+[0]*(n_actions-n-1)) for n in range(n_actions)}
             is_discrete     = 0 < n_actions and n_actions < float('inf')
             is_onehots      = action_set == onehot_actions
             is_categoricals = all([isinstance(a,str) for a in action_set])
 
-            if not is_discrete or (not is_onehots and not is_categoricals):
+            is_cyclable = is_discrete and (is_onehots or is_categoricals)
+
+            if not is_cyclable:
                 warnings.warn("Cycle only works for discrete environments without action features. It will be ignored in this case.")
                 yield from with_cycle_interactions
             else:
                 for interaction in with_cycle_interactions:
-                    rewards = deque(interaction['rewards'])
+                    rewards = deque(map(interaction['rewards'].eval,interaction['actions']))
                     rewards.rotate(1)
 
                     new = interaction.copy()
-                    new['rewards'] = SequenceReward(list(rewards))
+                    new['rewards'] = SequenceReward(interaction['actions'],list(rewards))
 
                     yield new
 
 class Flatten(EnvironmentFilter):
     """Flatten the context and action features for interactions."""
 
     def __init__(self):
@@ -731,40 +743,41 @@
         return params
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         rng = CobaRandom(self._seed)
 
         for interaction in interactions:
+
             new = interaction.copy()
 
-            noisy_context = self._noises(interaction['context'], rng, self._context_noise)
-            noisy_actions = [self._noises(a, rng, self._action_noise) for a in interaction['actions'] ]
-            noisy_rewards = [ self._noises(r, rng, self._reward_noise) for r in interaction['rewards'] ]
-            noisy_rewards = SequenceReward(noisy_rewards)
+            context = new['context']
+            actions = new['actions']
+            rewards = new['rewards']
+
+            noisy_context = self._noises(context, rng, self._context_noise)
+            noisy_actions = [ self._noises(a, rng, self._action_noise) for a in actions ]
+            noisy_rewards = [ self._noises(r, rng, self._reward_noise) for r in map(rewards.eval,actions) ]
+            noisy_rewards = SequenceReward(noisy_actions, noisy_rewards)
 
             new['context'] = noisy_context
             new['actions'] = noisy_actions
             new['rewards'] = noisy_rewards
 
             yield new
 
     def _noises(self, value:Union[None,float,str,Mapping,Sequence], rng: CobaRandom, noiser: Callable[[float,CobaRandom], float]):
-
         if isinstance(value, primitives.Sparse):
             #we sort so that noise generation is deterministic with respect to seed
             return { k:self._noise(v, rng, noiser) for k,v in sorted(value.items()) }
-
         if isinstance(value, primitives.Dense):
             return [ self._noise(v, rng, noiser) for v in value ]
-
         return self._noise(value, rng, noiser)
 
     def _noise(self, value:Union[None,float,str], rng: CobaRandom, noiser: Callable[[float,CobaRandom], float]) -> float:
-
         return value if not isinstance(value,(int,float)) else noiser(value, rng)
 
 class Params(EnvironmentFilter):
     """Add parameters to an environment."""
     def __init__(self, params: Mapping[str, Any]) -> None:
         self._params = params
 
@@ -785,17 +798,17 @@
             self._seed   = seed
             self._argmax = argmax
 
         @lru_cache(maxsize=None)
         def eval(self, arg):
             if not self._rng: self._rng = CobaRandom(self._seed)
             if arg == self._argmax:
-                return self._rng.choice(self._goods) 
+                return self._rng.choice(self._goods)
             else:
-                return self._rng.choice(self._bads) 
+                return self._rng.choice(self._bads)
 
     def __init__(self, n_users: int, n_normal:int, n_words:int, n_good:int, seed:int) -> None:
         self._n_users  = self._cast_int(n_users , "n_users" )
         self._n_normal = self._cast_int(n_normal, "n_normal")
         self._n_words  = self._cast_int(n_words , "n_words" )
         self._n_good   = self._cast_int(n_good  , "n_good"  )
         self._seed     = seed
@@ -822,23 +835,23 @@
             "igl_seed" : self._seed
         }
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
         rng = CobaRandom(self._seed)
 
         #we make it a set for faster contains checks
-        normalids       = set(self.normalids) 
+        normalids       = set(self.normalids)
         normal          = [u in normalids for u in self.userids]
         userid_isnormal = list(zip(self.userids,normal))
 
         first,interactions = peek_first(interactions)
 
         if not interactions: return []
 
-        is_binary_rwd = {0,1} == set(first['rewards'])
+        is_binary_rwd = set(map(first['rewards'].eval, first['actions'])) == {0,1}
         first_context = first['context']
 
         is_sparse = isinstance(first_context,primitives.Sparse)
         is_dense  = isinstance(first_context,primitives.Dense)
 
         goods = [(g,) for g in self.goodwords]
         bads  = [(b,) for b in self.badwords ]
@@ -873,50 +886,72 @@
     def _cast_int(self, value:Union[float,int], value_name:str) -> int:
         if isinstance(value, int): return value
         if isinstance(value, float) and value.is_integer(): return int(value)
         raise CobaException(f"{value_name} must be a whole number and not {value}.")
 
 class Repr(EnvironmentFilter):
     def __init__(self, 
-        cat_context:Literal["onehot","onehot_tuple","string"] = None,
-        cat_actions:Literal["onehot","onehot_tuple","string"] = None) -> None:
-        self._cat_context = cat_context
-        self._cat_actions = cat_actions
+        categorical_context:Literal["onehot","onehot_tuple","string"] = None,
+        categorical_actions:Literal["onehot","onehot_tuple","string"] = None) -> None:
+        self._cat_context = categorical_context
+        self._cat_actions = categorical_actions
 
     @property
     def params(self) -> Mapping[str, Any]:
-        return {"cat_context": self._cat_context, "cat_actions": self._cat_actions}
+        return {"categoricals_in_context": self._cat_context, "categoricals_in_actions": self._cat_actions}
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
 
-        has_actions = 'actions' in first
+        has_actions   = 'actions' in first and bool(first['actions'])
+        has_rewards   = 'rewards' in first
+        has_feedbacks = 'feedbacks' in first
+
+        n_tee = 1 + int(self._cat_context is not None) + int(self._cat_actions is not None and has_actions)
 
-        I = tee(interactions, 3 if has_actions else 2)
+        if n_tee == 1:
+            tees = iter([interactions])
+        else:
+            tees = iter(tee(interactions, n_tee))
 
-        interactions     = I[0]
-        cat_context_iter = pipes.EncodeCatRows(self._cat_context).filter(i['context'] for i in I[1])
+        if self._cat_context is not None:
+            cat_context_iter = pipes.EncodeCatRows(self._cat_context).filter(i['context'] for i in next(tees))
 
-        if has_actions:
-            cat_actions_iter = pipes.EncodeCatRows(self._cat_actions, True).filter(action for i in I[2] for action in i['actions'])
+        if self._cat_actions and has_actions:
+            cat_actions_iter = pipes.EncodeCatRows(self._cat_actions).filter(i['actions'] for i in next(tees))
+
+        for interaction in next(tees):
 
-        for interaction in interactions:
             new = interaction.copy()
-            new['context'] = next(cat_context_iter)
 
-            if has_actions:
-                new['actions'] = list(islice(cat_actions_iter,len(interaction['actions'])))
+            if self._cat_context:
+                new['context'] = next(cat_context_iter)
+
+            if has_actions and self._cat_actions:
+                new_actions = next(cat_actions_iter)
+                old_actions = new['actions']
+
+                if new_actions != old_actions or type(new_actions[0]) != type(old_actions[0]):
+                    new['actions'] = new_actions
+
+                if new_actions != old_actions:
+                    if has_rewards:
+                        if isinstance(new['rewards'],MulticlassReward):
+                            new['rewards'] = MulticlassReward(new_actions[old_actions.index(new['rewards'].argmax())])
+                        else:
+                            new['rewards'] = SequenceReward(new_actions,list(map(new['rewards'].eval,old_actions)))
+                    if has_feedbacks:
+                        new['feedbacks'] = SequenceFeedback(new_actions,list(map(new['feedbacks'].eval,old_actions)))
 
             yield new
 
 class Batch(EnvironmentFilter):
-
     def __init__(self, batch_size: int) -> None:
         self._batch_size = batch_size
 
     @property
     def params(self) -> Mapping[str,Any]:
         return {'batched': self._batch_size}
 
@@ -982,14 +1017,17 @@
             unbatched = Unbatch().filter(interactions)
             filtered  = self._filter.filter(unbatched)
             rebatched = Batch(batch_size).filter(filtered)
             yield from rebatched
 
 class Finalize(EnvironmentFilter):
 
+    def __init__(self, apply_repr: bool = True):
+        self._apply_repr = apply_repr
+
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
 
         first_has_context = 'context' in first
@@ -1006,21 +1044,24 @@
             is_dense_action  = isinstance(first['action'],primitives.Dense)
             is_sparse_action = isinstance(first['action'],primitives.Sparse)
 
         context_materialized = not first_has_context or (not is_dense_context and not is_sparse_context or isinstance(first['context']   ,(list,tuple,dict)))
         actions_materialized = not first_has_actions or (not is_dense_actions and not is_sparse_actions or isinstance(first['actions'][0],(list,tuple,dict)))
         action_materialized  = not first_has_action  or (not is_dense_action  and not is_sparse_action  or isinstance(first['action']    ,(list,tuple,dict)))
 
-        for interaction in Repr("onehot","onehot").filter(interactions):
+        if self._apply_repr:
+            interactions = Repr("onehot","onehot_tuple").filter(interactions)
+
+        for interaction in interactions:
 
             new = interaction.copy()
 
             if not context_materialized and is_dense_context:
                 new['context'] = list(new['context'])
-            elif not context_materialized and is_sparse_context :
+            elif not context_materialized and is_sparse_context:
                 new['context'] = new['context'].copy()
 
             if not actions_materialized and is_dense_actions:
                 new['actions'] = list(map(list,new['actions']))
             elif not actions_materialized and is_sparse_action:
                 new['actions'] = list(map(methodcaller('copy'),new['actions']))
 
@@ -1034,49 +1075,42 @@
 class Chunk(EnvironmentFilter):
     """A placeholder filter that exists only to semantically indicate how an environment pipe should be chunked for processing."""
     def filter(self, items: Iterable[Interaction]) -> Iterable[Interaction]:
         return items
 
 class Logged(EnvironmentFilter):
 
-    def __init__(self, learner: Learner, rewards:Literal["DM","IPS"] = "DM", seed:float = 1.23) -> None:
+    def __init__(self, learner: Learner, seed: Optional[float] = 1.23) -> None:
         self._learner = learner
-        self._rewards = rewards
         self._seed    = seed
 
     @property
     def params(self) -> Mapping[str, Any]:
-        return {"learner": SafeLearner(self._learner).params, "logged":True, "rewards": self._rewards, "log_seed":self._seed}
+        return {"learner": SafeLearner(self._learner).params, "logged":True, "log_seed":self._seed}
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
 
         if 'context' not in first or 'actions' not in first or 'rewards' not in first:
             raise CobaException("We were unable to create a logged representation of the interaction.")
 
         #Avoid circular dependency
-        from coba.experiments.tasks import SimpleEvaluation
+        from coba.experiments.tasks import OnPolicyEvaluation
 
-        CobaContext.store['experiment_seed'] = self._seed
+        seed = self._seed if self._seed is not None else CobaRandom().random()
 
         I1,I2 = tee(interactions,2)
         flat_int = Unbatch().filter(I1)
-        eval_log = SimpleEvaluation(record=['action','reward','probability']).process(copy.deepcopy(self._learner),I2)
+        eval_log = OnPolicyEvaluation(record=['action','reward','probability'],seed=seed).process(copy.deepcopy(self._learner),I2)
         for interaction, log in zip(flat_int,eval_log):
             out = interaction.copy()
             out.update(log)
-
-            if self._rewards == "IPS":
-                actions = interaction.get('actions',[])
-                action  = actions.index(log['action']) if len(actions) > 0 else log['action']
-                out['rewards'] = IPSReward(log['reward'],action,log['probability'])
-
             yield out
 
 class Mutable(EnvironmentFilter):
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first, interactions = peek_first(interactions)
@@ -1109,7 +1143,105 @@
         elif first_is_value:
             for interaction in interactions:
                 yield interaction.copy()
 
 class MappingToInteraction(Filter[Iterable[Mapping], Iterable[Interaction]]):
     def filter(self, items: Iterable[Mapping]) -> Iterable[Interaction]:
         yield from map(Interaction.from_dict,items)
+
+class OpeRewards(EnvironmentFilter):
+
+    def __init__(self, rwds_type:Literal['IPS','DM','DR','NO']=None):
+        if rwds_type in ['DM','DR']:
+            PackageChecker.vowpalwabbit("Rewards.__init__")
+        self._rwds_type = rwds_type
+
+    @property
+    def params(self) -> Mapping[str, Any]:
+        return {'rewards_type': self._rwds_type} if self._rwds_type else {}
+
+    def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
+        if self._rwds_type is None:
+            yield from interactions
+
+        elif self._rwds_type == "NO":
+            for log in interactions:
+                log = log.copy()
+                log.pop('rewards',None)
+                yield log
+
+        elif self._rwds_type == "IPS":
+            for log in interactions:
+                log = log.copy()
+                log['rewards'] = IPSReward(log['reward'], log['action'], log.get('probability'))
+                yield log
+
+        elif self._rwds_type in ["DM","DR"]:
+            from coba.learners.vowpal import VowpalMediator
+
+            rng = CobaRandom(1)
+            vw = VowpalMediator()
+
+            # When using cb_adf to estimate rewards for actions instead of the
+            # regression we would receive rewards far outside of the expected boundaries.
+            #vw.init_learner("--cb_adf --interactions xa --interactions xxa --quiet ", label_type=4)
+            vw.init_learner("--interactions xa --interactions xxa --quiet ", label_type=1)
+
+            #so that we don't run forever
+            #when interactions is re-iterable
+            interactions = iter(interactions)
+
+            while True:
+
+                #Batch Shuffling reduces the correlation between
+                #the reward functions learned by this VW learner
+                #and potential downstream VW learners. If this
+                #correlation is strong, we will over estimate
+                #the downstream VW learner's performance.
+                L = list(islice(interactions,4000))
+                R = [ [] for _ in range(len(L)) ]
+                X = []
+
+                if not L: break
+
+                for log, rewards in rng.shuffle(list(zip(L,R)), inplace=True):
+                    log_context = log['context']
+                    log_action  = log['action']
+                    log_reward  = log['reward']
+                    log_prob    = log['probability']
+
+                    #type-4
+                    #labels            = [None]*len(log_actions)
+                    #labels[log_index] = f"{log_index+1}:{log_reward}:{log_prob}"
+                    #vw.learn(vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions], labels))
+
+                    #type-1
+                    vw.learn(vw.make_example({"x":log_context, "a": log_action}, f"{log_reward} {1/log_prob}"))
+
+                for log, rewards in rng.shuffle(list(zip(L,R)), inplace=True):
+                    log_context = log['context']
+                    log_actions = log['actions']
+                    log_action  = log['action']
+                    log_reward  = log['reward']
+                    log_prob    = log['probability']
+                    log_index   = log_actions.index(log_action)
+
+                    #type-4
+                    #examples = vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions])
+                    #rewards.extend(vw.predict(examples))
+
+                    #type-1
+                    examples = vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions])
+                    rewards.extend(vw.predict(e) for e in examples)
+
+                    if self._rwds_type=="DR":
+                        rewards[log_index] += (log_reward-rewards[log_index])/log_prob
+
+                for log,rewards in zip(L,R):
+                    log = log.copy()
+
+                    try:
+                        log['rewards'] = MappingReward(dict(zip(log['actions'],rewards)))
+                    except:
+                        log['rewards'] = SequenceReward(log['actions'],rewards)
+
+                    yield log
```

### Comparing `coba-6.4.2/coba/environments/openml.py` & `coba-6.5.0/coba/environments/openml.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
 class OpenmlSimulation(SupervisedSimulation):
     """A supervised simulation created from an openml dataset.
     Download a dataset from openml.org and create a SupervisedSimulation.
     """
 
     @overload
-    def __init__(self, data_id: int, drop_missing: bool = True, take: int = None, *, target:str = None):
+    def __init__(self, data_id: int, drop_missing: bool = True, take: int = None, *, target:str = None, ):
         """Instantiate an OpenmlSimulation.
         Args:
             data_id: The data id uniquely identifying the dataset on openml (i.e., openml.org/d/{id})
             drop_missing: Drop data rows with missing values.
             take: The number of interactions we'd like the simulation to have (these will be selected at random).
             target: The column that should be marked as the prediction label in the source.
         """
@@ -284,15 +284,15 @@
             target: The column that should be marked as the prediction label in the source.
         """
         ...
 
     def __init__(self, *args, **kwargs) -> None:
         """Instantiate an OpenmlSimulation."""
         kwargs.update(zip(['data_id','drop_missing','take'], args))
-        super().__init__(OpenmlSource(**kwargs), None, None, kwargs.get('take',None))
+        super().__init__(OpenmlSource(**kwargs), None, kwargs.get('label_type',None), kwargs.get('take',None))
 
     @property
     def params(self) -> Dict[str, Any]:
         return {**super().params, "type": "OpenmlSimulation" }
 
     def __str__(self) -> str:
```

### Comparing `coba-6.4.2/coba/environments/primitives.py` & `coba-6.5.0/coba/environments/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,20 +43,15 @@
             actions : Features describing available actions during the interaction.
             rewards : The reward for each action in the interaction.
             kwargs : Any additional information.
         """
 
         self['context'] = context
         self['actions'] = actions
-        if isinstance(rewards,(list,tuple)):
-            if len(rewards) != len(actions): 
-                raise CobaException("The given actions and rewards did not line up.")
-            self['rewards'] = SequenceReward(rewards)
-        else:
-            self['rewards'] = rewards
+        self['rewards'] = rewards if not isinstance(rewards,(list,tuple)) else SequenceReward(actions,rewards)
 
         if kwargs: self.update(kwargs)
 
 class GroundedInteraction(Interaction):
     """A grounded interaction based on Interaction Grounded Learning which feedbacks instead of rewards."""
     __slots__=()
     keywords = {'type', 'context', 'actions', 'rewards', 'feedbacks'}
@@ -75,16 +70,16 @@
             rewards: The reward for each action in the interaction.
             feedbacks: The feedback for each action in the interaction.
             **kwargs: Additional information that should be recorded in the interactions table of an experiment result.
         """
 
         self['context'] = context
         self['actions'] = actions
-        self['rewards'] = SequenceReward(rewards) if isinstance(rewards,(list,tuple)) else rewards
-        self['feedbacks'] = SequenceFeedback(feedbacks) if isinstance(feedbacks,(list,tuple)) else feedbacks
+        self['rewards'] = SequenceReward(actions,rewards) if isinstance(rewards,(list,tuple)) else rewards
+        self['feedbacks'] = SequenceFeedback(actions,feedbacks) if isinstance(feedbacks,(list,tuple)) else feedbacks
 
         if kwargs: self.update(kwargs)
 
 class LoggedInteraction(Interaction):
     """A logged interaction with an action, reward and optional probability."""
     __slots__ = ()
     keywords = {'type', 'context', 'action', 'reward', 'probability', 'actions', 'rewards'}
@@ -117,18 +112,15 @@
             rewards: The rewards to use for off policy evaluation. These rewards will not be shown to any learners. They will
                 only be recorded in experimental results. If probability and actions is provided and rewards is None then 
                 rewards will be initialized using the IPS estimator.
             **kwargs : Any additional information.
         """
 
         if isinstance(kwargs.get('rewards'),(list,tuple)):
-            self['rewards'] = SequenceReward(kwargs.pop('rewards'))
-        elif kwargs.get('rewards') is None and kwargs.get('actions') is not None:
-            ips_action = kwargs['actions'].index(action) if isinstance(kwargs['actions'],(list,tuple)) else action
-            self['rewards'] = IPSReward(reward,ips_action,kwargs.get('probability'))
+            self['rewards'] = SequenceReward(kwargs['actions'],kwargs.pop('rewards'))
 
         self['context'] = context
         self['action']  = action
         self['reward']  = reward
 
         if kwargs: self.update({k:v for k,v in kwargs.items() if v is not None})
```

### Comparing `coba-6.4.2/coba/environments/serialized.py` & `coba-6.5.0/coba/environments/serialized.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,30 +36,46 @@
 class ZipMemberToObjects(Source[Iterable[object]]):
     def __init__(self, zip:str, member:str):
         self._zip    = zip
         self._member = member
 
     def read(self) -> Iterable[object]:
         try:
-            with ZipFile(self._zip) as zip:
-                with zip.open(self._member) as f:
-                    yield from map(pickle.load, repeat(f))
+            with ZipFile(self._zip) as z:
+                with z.open(self._member) as m:
+                    yield from map(pickle.load, repeat(m))
         except EOFError:
             pass
 
 class EnvironmentsToObjects(Filter[Environment, Iterable]):
     def filter(self, envs: Union[Environment,Sequence[Environment]]) -> Iterable[Iterable[object]]:
         if not isinstance(envs,(abc.Iterable)): envs = [envs]
         for env in envs:
             with CobaContext.logger.time("Materializing environment..."):
-                yield list(chain([{"version":1,"coba_version":version("coba")},env.params], env.read()))
+                yield list(self._env_to_objects(env))
+
+    def _env_to_objects(self,env):
+        yield {"version":2,"coba_version":version("coba")}
+        yield env.params
+        I = iter(env.read())
+        batch = list(islice(I,1000))
+        while batch: 
+            yield batch
+            batch = list(islice(I,1000))
 
 class EnvironmentFromObjects(Environment):
     def __init__(self, source: Source[Iterable[object]]) -> None:
         self._source = source
 
     @property
     def params(self) -> Mapping[str,Any]:
-        return next(islice(self._source.read(),1,None))
+        return list(islice(self._source.read(),1,2))[0]
 
     def read(self) -> Iterable[Interaction]:
-        yield from islice(self._source.read(),2,None)
+
+        I = iter(self._source.read())
+        version_data = list(islice(I,2))[0]
+        
+        if version_data['version'] == 1: #pragma: no cover
+            yield from I
+        else:
+            yield from chain.from_iterable(I)
```

### Comparing `coba-6.4.2/coba/environments/supervised.py` & `coba-6.5.0/coba/environments/supervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from itertools import chain, count
+from itertools import chain
 from typing import Any, Iterable, Union, Sequence, overload, Dict, MutableSequence, MutableMapping
 from coba.backports import Literal
 
 from coba.pipes import Pipes, Source, IterableSource, LabelRows, Reservoir, UrlSource, CsvReader
 from coba.pipes import CsvReader, ArffReader, LibsvmReader, ManikReader
 
 from coba.utilities import peek_first
@@ -48,16 +48,15 @@
     def __init__(self,source: Union[str,Source[Iterable[str]]]) -> None:
         """Instantiate an ArffSource.
 
         Args:
             source: The data source. Accepts either a string representing the source location or another Source.
         """
         source       = UrlSource(source) if isinstance(source,str) else source
-        reader       = ArffReader()
-        self._source = Pipes.join(source, reader)
+        self._source = Pipes.join(source, ArffReader())
 
     def read(self) -> Union[Iterable[MutableSequence], Iterable[MutableMapping]]:
         """Read and parse the arff source."""
         return self._source.read()
 
     @property
     def params(self) -> Dict[str, Any]:
@@ -75,17 +74,16 @@
 
     def __init__(self, source: Union[str,Source[Iterable[str]]]) -> None:
         """Instantiate a LibsvmSource.
 
         Args:
             source: The data source. Accepts either a string representing the source location or another Source.
         """
-        source = UrlSource(source) if isinstance(source,str) else source
-        reader = LibsvmReader()
-        self._source = Pipes.join(source, reader)
+        source       = UrlSource(source) if isinstance(source,str) else source
+        self._source = Pipes.join(source, LibsvmReader())
 
     def read(self) -> Iterable[MutableMapping]:
         """Read and parse the libsvm source."""
         return self._source.read()
 
     @property
     def params(self) -> Dict[str, Any]:
@@ -103,17 +101,16 @@
 
     def __init__(self, source: Union[str,Source[Iterable[str]]]) -> None:
         """Instantiate a ManikSource.
 
         Args:
             source: The data source. Accepts either a string representing the source location or another Source.
         """
-        source = UrlSource(source) if isinstance(source,str) else source
-        reader = ManikReader()
-        self._source = Pipes.join(source, reader)
+        source       = UrlSource(source) if isinstance(source,str) else source
+        self._source = Pipes.join(source, ManikReader())
 
     def read(self) -> Iterable[MutableMapping]:
         """Read and parse the manik source."""
         return self._source.read()
 
     @property
     def params(self) -> Dict[str, Any]:
@@ -190,49 +187,45 @@
 
         first, rows = peek_first(self._source.read())
         first_row_type = 0 if hasattr(first,'label') else 1
 
         if not rows: return []
 
         first_label      = first.label if first_row_type == 0 else first[1]
-        first_label_type = first.tipe if first_row_type == 0 else None
+        first_label_type = first.tipe  if first_row_type == 0 else None
 
         if first_label_type is None:
             label_type = self._label_type or ("r" if isinstance(first_label, (int,float)) else "c")
         else:
             label_type = self._label_type or first_label_type
 
         label_type = label_type.lower()
         self._params['label_type'] = label_type.upper()
 
-        #these are the cases where we need to know all labels in the dataset to determine actions
-        if label_type == "m" or (label_type == "c" and not isinstance(first_label, Categorical)):
-            rows = list(rows)
-            if first_row_type == 0: labels = [r.label for r in rows]
-            if first_row_type == 1: labels = [r[1]    for r in rows]
-
         if label_type == "r":
             actions = []
             reward  = L1Reward
-        elif label_type == "m":
-            actions = sorted(set(list(chain(*labels))))
-            action_indexes = dict(zip(actions,count()))
-            reward = lambda label: HammingReward(list(map(action_indexes.__getitem__,label)))
+        
+        elif label_type == "c" and isinstance(first_label, Categorical):
+            #Handling the categoricals separately allows for a performance optimization
+            #since we can use the Categorical's as_int property rather than action_indexes
+            actions = [ Categorical(l,first_label.levels) for l in first_label.levels ]
+            reward  = MulticlassReward
         else:
-            if isinstance(first_label,Categorical):
-                #Handling the categoricals separately allows for a performance optimization
-                #since we can use the Categorical's as_int property rather than action_indexes
-                actions   = [ Categorical(l,first_label.levels) for l in first_label.levels ]
-                n_actions = len(actions)
-                reward    = lambda label: MulticlassReward(n_actions, label.as_int)
+            #we need to know all labels in the dataset to determine actions
+            rows = list(rows)
+            lbls = [r.label for r in rows] if first_row_type == 0 else [r[1] for r in rows]
+
+            if label_type == "m":
+                actions = sorted(set(list(chain(*lbls))))
+                reward = HammingReward
             else:
-                actions        = sorted(set(labels))
-                n_actions      = len(actions)
-                action_indexes = dict(zip(actions,count()))
-                reward         = lambda label: MulticlassReward(n_actions, action_indexes[label])
+                delist  = lambda l: l[0] if isinstance(l,list) else l
+                actions = sorted(set(map(delist,lbls)))
+                reward  = lambda l: MulticlassReward(delist(l))
 
         if first_row_type == 0:
             for row in rows:
                 yield {'context':row.feats,'actions':actions,'rewards':reward(row.label)}
         else:
             for row in rows:
-                yield {'context':row[0]   ,'actions':actions,'rewards':reward(row[1])}
+                yield {'context':row[0],'actions':actions,'rewards':reward(row[1])}
```

### Comparing `coba-6.4.2/coba/environments/synthetics.py` & `coba-6.5.0/coba/environments/synthetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         _reward  = lambda i,c,a: self._reward (i,c,a,rng) if rng else self._reward (i,c,a)
 
         for i in islice(count(), self._n_interactions):
             context  = _context(i)
             actions  = _actions(i, context)
             rewards  = [ _reward(i, context, action) for action in actions]
 
-            yield {'context':context,'actions':actions,'rewards': SequenceReward(rewards) }
+            yield {'context':context,'actions':actions,'rewards': SequenceReward(actions,rewards) }
 
     def __str__(self) -> str:
         return "LambdaSimulation"
 
     class Spoof:
         def __init__(self, interactions, _params, _str, _name) -> None:
             self._str           = _str
@@ -344,15 +344,14 @@
         def context(index:int, rng: CobaRandom) -> Context:
             return tuple(rng.randoms(n_context_features,-1.5,1.5)) if n_context_features else None
 
         def actions(index:int, context: Context, rng: CobaRandom) -> Sequence[Action]:
             return [ tuple(rng.randoms(n_action_features,-1.5,1.5)) for _ in range(n_actions) ] if n_action_features else one_hot_acts
 
         def reward(index:int, context:Context, action:Action, rng: CobaRandom) -> float:
-
             part_index = action.index(1) if exemplar_parts > 1                           else 0
             context    = context         if n_context_features                           else []
             action     = action          if n_action_features or not n_context_features  else []
 
             f = list(context)+list(action)
             E = self._exemplars[part_index]
             W = self._weights  [part_index]
```

### Comparing `coba-6.4.2/coba/environments/templates.py` & `coba-6.5.0/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/exceptions.py` & `coba-6.5.0/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/experiments/__init__.py` & `coba-6.5.0/coba/experiments/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 This module contains the Experiment evaluator, implementations of specific tasks that are performed
 during an experiment evaluation, and the Result datastructures returned after experiment evalution.
 """
 
 from coba.experiments.core    import Experiment
 from coba.experiments.results import Result, Table
 from coba.experiments.tasks   import LearnerTask, SimpleLearnerInfo
-from coba.experiments.tasks   import EnvironmentTask, SimpleEnvironmentInfo, ClassEnvironmentInfo
-from coba.experiments.tasks   import EvaluationTask, SimpleEvaluation
+from coba.experiments.tasks   import EnvironmentTask, SimpleEnvironmentInfo, ClassEnvironmentInfo, LambdaEvaluation
+from coba.experiments.tasks   import EvaluationTask, SimpleEvaluation, OnPolicyEvaluation, OffPolicyEvaluation, ExplorationEvaluation
 
 __all__ = [
     'Result',
     'Table',
     'Experiment',
     'LearnerTask',
     'EnvironmentTask',
     'EvaluationTask',
     'SimpleLearnerInfo',
     'ClassEnvironmentInfo',
     'SimpleEvaluation',
     'SimpleEnvironmentInfo',
+    'OnPolicyEvaluation',
+    'OffPolicyEvaluation',
+    'ExplorationEvaluation',
+    'LambdaEvaluation'
 ]
```

### Comparing `coba-6.4.2/coba/experiments/core.py` & `coba-6.5.0/coba/experiments/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from coba.environments import Environment
 from coba.multiprocessing import CobaMultiprocessor
 from coba.contexts import CobaContext, ExceptLog, StampLog, NameLog, DecoratedLogger, ExceptionLogger
 from coba.exceptions import CobaException
 
 from coba.experiments.process import CreateWorkItems,  RemoveFinished, ChunkByChunk, MaxChunkSize, ProcessWorkItems
 from coba.experiments.tasks   import EnvironmentTask, EvaluationTask, LearnerTask
-from coba.experiments.tasks   import SimpleLearnerInfo, SimpleEnvironmentInfo, SimpleEvaluation
+from coba.experiments.tasks   import SimpleLearnerInfo, SimpleEnvironmentInfo, SimpleEvaluation, LambdaEvaluation
 from coba.experiments.results import Result, TransactionIO
 
 class Experiment:
     """An Experiment using a collection of environments and learners."""
 
     @overload
     def __init__(self,
@@ -66,14 +66,17 @@
 
         self._pairs            = args[0]
         self._description      = kwargs.get('description',None)
         self._learner_task     = kwargs.get('learner_task', SimpleLearnerInfo())
         self._environment_task = kwargs.get('environment_task', SimpleEnvironmentInfo())
         self._evaluation_task  = kwargs.get('evaluation_task', SimpleEvaluation())
 
+        if callable(self._evaluation_task):
+            self._evaluation_task = LambdaEvaluation(self._evaluation_task)
+
         if any([lrn is None for lrn,_ in self._pairs]):
             raise CobaException("A Learner was given whose value was None, which can't be processed.")
 
         if any([env is None for _,env in self._pairs]):
             raise CobaException("An Environment was given whose value was None, which can't be processed.")
 
         self._processes        : Optional[int] = None
@@ -118,15 +121,15 @@
         return self._maxchunksperchild if self._maxchunksperchild is not None else CobaContext.experiment.maxchunksperchild
 
     @property
     def maxtasksperchunk(self) -> int:
         """The maximum number of tasks allowed in a chunk before breaking a chunk into smaller chunks."""
         return self._maxtasksperchunk if self._maxtasksperchunk is not None else CobaContext.experiment.maxtasksperchunk
 
-    def run(self, result_file:str = None, quiet:bool = False, processes:int = None, seed: int = 1) -> Result:
+    def run(self, result_file:str = None, quiet:bool = False, processes:int = None, seed: Optional[int] = 1) -> Result:
         """Run the experiment and return the results.
 
         Args:
             result_file: The file for writing and restoring results.
             quiet: Indicates that logged output should be turned off.
             processes: The number of processes to create for evaluating the experiment.
             seed: The seed that will determine all randomness within the experiment.
```

### Comparing `coba-6.4.2/coba/experiments/process.py` & `coba-6.5.0/coba/experiments/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
 class RemoveFinished(Filter[Iterable[WorkItem], Iterable[WorkItem]]):
     def __init__(self, restored: Optional[Result]) -> None:
         self._restored = restored
 
     def filter(self, tasks: Iterable[WorkItem]) -> Iterable[WorkItem]:
 
-        finished_learners = set(self._restored.learners.col_values()[0]) if self._restored else set()
-        finished_environments = set(self._restored.environments.col_values()[0]) if self._restored else set()
-        finished_evaluations = set(zip(*self._restored.interactions.col_values()[:2])) if self._restored else set()
+        finished_learners = set(self._restored.learners['learner_id']) if self._restored else set()
+        finished_environments = set(self._restored.environments['environment_id']) if self._restored else set()
+        finished_evaluations = set(self._restored.interactions[['environment_id','learner_id']]) if self._restored else set()
 
         for task in tasks:
 
             is_learner_task = task.env_id is None
             is_environ_task = task.lrn_id is None
             is_eval_task    = not (is_learner_task or is_environ_task)
```

### Comparing `coba-6.4.2/coba/experiments/results.py` & `coba-6.5.0/coba/experiments/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import datetime
 import re
 import collections
 import collections.abc
 
+from bisect import bisect_left, bisect_right
 from pathlib import Path
 from numbers import Number
-from operator import truediv, sub, itemgetter, eq, contains, ge, lt, le, gt, or_
+from operator import truediv, sub, itemgetter, gt
 from abc import abstractmethod
 from itertools import chain, repeat, accumulate, groupby, count, compress
-from typing import Any, Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, NamedTuple, overload
+from typing import Any, Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, NamedTuple
 from coba.backports import Literal
 
+from coba.primitives import Batch
 from coba.environments import Environment
 from coba.statistics import mean, stdev, StandardErrorOfMean, BootstrapConfidenceInterval, BinomialConfidenceInterval, PointAndInterval
 from coba.contexts import CobaContext
 from coba.exceptions import CobaException
-from coba.utilities import PackageChecker
+from coba.utilities import PackageChecker, peek_first
 from coba.pipes import Pipes, Sink, Source, JsonEncode, JsonDecode, DiskSource, DiskSink, IterableSource, ListSink, Foreach
 
 def exponential_moving_average(values:Sequence[float], span:int=None) -> Iterable[float]:
     #exponential moving average identical to Pandas df.ewm(span=span).mean()
     alpha = 2/(1+span)
     cumwindow  = list(accumulate(values          , lambda a,v: v + (1-alpha)*a))
     cumdivisor = list(accumulate([1.]*len(values), lambda a,v: v + (1-alpha)*a))
     return map(truediv, cumwindow, cumdivisor)
 
 def moving_average(values:Sequence[float], span:int=None) -> Iterable[float]:
-
     if span == 1:
         return values
 
     if span is None or span >= len(values):
         return tuple(map(truediv, accumulate(values),count(1)))
 
     window_sums  = accumulate(map(sub, values, chain(repeat(0,span),values)))
@@ -39,490 +39,470 @@
     return map(truediv,window_sums,window_sizes)
 
 def old_to_new(
     env_rows: Mapping[int           ,Mapping[str,Any]] = {},
     lrn_rows: Mapping[int           ,Mapping[str,Any]] = {},
     int_rows: Mapping[Tuple[int,int],Mapping[str,Any]] = {}) -> Tuple[Sequence,Sequence,Sequence]:
 
-    env_hdrs = set().union(*[v.keys()            for v in env_rows.values()]) - {'environment_id'}
-    lrn_hdrs = set().union(*[v.keys()            for v in lrn_rows.values()]) - {'learner_id'}
-    int_hdrs = set().union(*[v['_packed'].keys() for v in int_rows.values()]) - {'environment_id','learner_id','index'}
-
-    rwd_col = ['reward'] if 'reward' in int_hdrs else []
-
-    env_hdrs = ['environment_id'                     ] +           sorted(env_hdrs)
-    lrn_hdrs = [                 'learner_id'        ] +           sorted(lrn_hdrs)
-    int_hdrs = ['environment_id','learner_id','index'] + rwd_col + sorted(int_hdrs-{'reward'})
-
-    env_table = Table(env_hdrs)
-    lrn_table = Table(lrn_hdrs)
-    int_table = Table(int_hdrs)
-
-    env_rows = [ { "environment_id":k, **v } for k,v in env_rows.items() ]
-    env_table.insert(rows=[[row.get(k) for k in env_hdrs] for row in env_rows])
+    rwd_col = ['reward'] if any('reward' in v.keys() for v in int_rows.values()) else []
 
-    lrn_rows = [ { "learner_id" :k,   **v } for k,v in lrn_rows.items() ]
-    lrn_table.insert(rows=[[row.get(k) for k in lrn_hdrs] for row in lrn_rows])
+    env_table = Table(columns=['environment_id'                     ]          )
+    lrn_table = Table(columns=[                 'learner_id'        ]          )
+    int_table = Table(columns=['environment_id','learner_id','index'] + rwd_col)
 
-    #These are the actual data columns
-    int_hdrs = int_hdrs[3:]
+    env_table.insert([{"environment_id":e,                **v} for e,v in env_rows.items()])
+    lrn_table.insert([{                   "learner_id":l, **v} for l,v in lrn_rows.items()])
 
     for (env_id, lrn_id), results in int_rows.items():
         if results.get('_packed'):
-            names,cols = zip(*results['_packed'].items())
-            N          = len(cols[0])
 
-            if len(int_hdrs) != len(names):
-                cols  += (Repeat(None,N),)*(len(int_hdrs) - len(names))
-                names += tuple(set(int_hdrs)-set(names))
+            packed = results['_packed']
+            N = len(packed[next(iter(packed))])
 
-            index_columns     = (Repeat(env_id,N), Repeat(lrn_id,N), Count(1,N+1))
-            ordered_data_cols = tuple(cols[names.index(col)] for col in int_hdrs)
+            packed['environment_id'] = repeat(env_id,N)
+            packed['learner_id'    ] = repeat(lrn_id,N)
+            packed['index'         ] = range(1,N+1)
 
-            int_table.insert(cols=index_columns+ordered_data_cols)
+            int_table.insert(packed)
 
     return env_table, lrn_table, int_table
 
-def env_len_lrn_counts(interactions: 'Table') -> Tuple[Mapping[int,int],Mapping[int,int]]:
-    ###WARNING, this logic has been highly optimized
-    env_lengths  = {}
-    env_lrn_cnts = collections.defaultdict(int)
-    for g, i in groupby(zip(*interactions.col_values()[:2])):
-        env_lrn_cnts[g[0]]+=1
-        if g[0] not in env_lengths:
-            env_lengths[g[0]] = sum(1 for _ in i)
-
-    return env_lengths, env_lrn_cnts
-
-class Repeat:
-    __slots__ =('value','times')
-    def __init__(self, value, times):
-        self.value = value
-        self.times = times
+def env_len_and_cnt(interactions: 'Table') -> Tuple[Mapping[int,int],Mapping[int,int]]:
+    env_len = {}
+    env_cnt = {}
+    for table in interactions.groupby(2):
+        env_id = table['environment_id'][0]
+        env_len[env_id] = len(table)
+        env_cnt[env_id] = env_cnt.get(env_id,0)+1
+
+    return env_len, env_cnt
+
+class View:
+
+    class ListView:
+        def __init__(self, seq:Sequence, sel:Sequence):
+            self._seq = seq
+            self._sel = sel
+
+        def __len__(self):
+            return len(self._sel)
+
+        def __getitem__(self,key):
+            if isinstance(key,slice):
+                return View.ListView(self._seq,self._sel[key])
+            else:
+                return self._seq[self._sel[key]]
 
-    def __iter__(self):
-        return iter(repeat(self.value,self.times))
+        def __iter__(self):
+            return iter(map(self._seq.__getitem__,self._sel))
 
-    def __len__(self) -> int:
-        return self.times
+    def __init__(self, data: Mapping[str,Sequence], selection: Union[Sequence[int],slice]) -> None:
+        self._data = data
+        self._selection = selection
 
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,Repeat) and o.value == self.value and o.times == self.times
+    def keys(self):
+        return self._data.keys()
 
-class Count:
-    __slots__ =('start','end')
-    def __init__(self, start,end):
-        self.start = start
-        self.end   = end
+    def values(self):
+        return [self[k] for k in self]
 
     def __iter__(self):
-        return iter(range(self.start, self.end))
+        return iter(self._data)
 
-    def __len__(self) -> int:
-        return self.end-self.start
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,Count) and o.start == self.start and o.end == self.end
-
-class Compress:
-    __slots__ =('_chunk','_keep')
-    def __init__(self,chunk,keep):
-        self._chunk = chunk
-        self._keep = keep
-
-    def __iter__(self):
-        return iter(compress(self._chunk,self._keep))
+    def __getitem__(self,key):
+        if isinstance(self._selection,slice):
+            return self._data[key][self._selection]
+        else:
+            return View.ListView(self._data[key], self._selection)
 
-    def __len__(self) -> int:
-        return sum(self._keep)
+    def __setitem__(self,key,value):
+        raise CobaException("A view of the data cannot be modified.")
 
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,Compress) and self._chunk == o._chunk and self._keep == o._keep
+    def __contains__(self,key) -> bool:
+        return key in self._data
 
 class Table:
     """A container class for storing tabular data."""
-    #Potentially overkill but by having our own "simple" table implementation we can provide
-    #Several useful pieces of functionality out of the box. Additionally, when working with
-    #Very large experiments pandas can become quite slow while our Table will work acceptably.
-
-    @overload
-    def __init__(self, table: 'Table', keep:Sequence[bool]=None) -> None:
-        """Copy a Table and optionally indicate which entries to keep.
+    #Potentially overkill, however, by having our own "simple" table implementation we can provide
+    #several useful pieces of functionality out of the box. Additionally, when working with
+    #very large experiments pandas can become quite slow while our Table works acceptably.
+    def __init__(self, data:Union[Mapping, Sequence[Mapping], Sequence[Sequence]] = (), columns: Sequence[str] = (), indexes: Sequence[str]= ()):
+
+        self._columns = tuple(columns)
+        self._data    = {c:[] for c in columns}
+        self.insert(data)
+        self._indexes = tuple(indexes)
+        self._lohis   = self._calc_lohis()
 
-        Args:
-            table: The table to copy.
-            keep: Which column rows to keep.
-        """
-
-    @overload
-    def __init__(self, columns: Sequence[str]) -> None:
-        """Instantiate a Table.
-
-        Args:
-            cols: The names assigned to each item in an element of rows.
-        """
-
-    def __init__(self, *args):
-
-        if isinstance(args[0], Table):
-            self._col_names  = args[0].col_names
-            self._col_chunks = [list(col) for col in args[0]._col_chunks]
-
-            if len(args) > 1:
-                keep = args[1]
-                assert len(keep) == len(self)
-
-                n_cols   = len(self._col_names)
-                n_chunks = len(self._col_chunks[0]) if n_cols else 0
-
-                empty = tuple()
-                i = 0
-
-                for j in range(n_chunks):
-                    chunk_size = len(self._col_chunks[0][j])
-                    chunk_keep = keep[i:i+chunk_size]
-
-                    if all(chunk_keep):
-                        pass
-                    elif not any(chunk_keep):
-                        for col in self._col_chunks: col[j] = empty
-                    else:
-                        for col in self._col_chunks: col[j] = Compress(col[j], chunk_keep)
-
-                    i+=chunk_size
-        else:
-            self._col_names = args[0]
-            self._col_chunks = [[] for _ in args[0]]
+    @property
+    def columns(self) -> Sequence[str]:
+        return self._columns
 
     @property
-    def col_names(self) -> Sequence[str]:
-        """The columns in the table."""
-        return self._col_names
+    def indexes(self) -> Sequence[str]:
+        return self._indexes
 
-    def col_values(self) -> Sequence[Iterable[Any]]:
-        return [ chain.from_iterable(c) for c in self._col_chunks]
+    def insert(self, data:Union[Mapping, Sequence[Mapping], Sequence[Sequence]]=()) -> 'Table':
+        data_is_empty              = not data
+        data_is_where_clause_view  = data and isinstance(data,View)
+        data_is_sequence_of_dicts  = data and isinstance(data,collections.abc.Sequence) and isinstance(data[0],collections.abc.Mapping)
+        data_is_mapping_of_columns = data and isinstance(data,collections.abc.Mapping)
+
+        if data_is_empty:
+            return self
+
+        if data_is_where_clause_view:
+            self._data = data
+            return self
+
+        if data_is_sequence_of_dicts:
+            data = {k:[d.get(k) for d in data] for k in set().union(*(d.keys() for d in data))}
+            data_is_mapping_of_columns = True
+
+        if data_is_mapping_of_columns:
+            old,new = set(self._columns), set(data.keys())
+            old_len = len(self)
+            new_len = 0
+
+            for hdr in new-old:
+                self._data[hdr] = list(chain(repeat(None, old_len), data[hdr]))
+                new_len = len(self._data[hdr])
+
+            for hdr in new&old:
+                self._data[hdr].extend(data[hdr])
+                new_len = len(self._data[hdr])
+
+            for hdr in old-new:
+                self._data[hdr].extend(repeat(None,new_len-old_len))
+
+            self._columns += tuple(sorted(new-old))
+
+        else: #data_is_list_of_rows
+            assert len(data[0]) == len(self._columns), "The given data rows don't align with the table's headers."
+            for hdr,col in zip(self._columns,zip(*data)):
+                self._data[hdr].extend(col)  
 
-    def row_values(self) -> Iterable[Sequence[Any]]:
-        return zip(*self.col_values())
+        self._indexes = ()
+        self._lohis = {}
 
-    def insert(self, *, cols:Sequence[Iterable[Any]]=None, rows:Sequence[Sequence[Any]]=None) -> 'Table':
+        return self
 
-        if cols:
-            assert len(cols) == len(self._col_names), "A column entry was not provided for every column"
-            assert len(set(map(len,cols))) == 1, "Different sized column entries were provided."
+    def index(self, *indx) -> 'Table':
 
-            for col,new in zip(self._col_chunks,cols):
-                col.append(new)
+        if not indx: return self
+        if not self._data: return self
+        indx = [col for col in indx if col in self._columns]
+        if self._indexes == tuple(indx): return self
+
+        lohis   = [(0,len(self))]
+        indexes = list(range(len(self)))
+
+        for col in indx:
+            for lo,hi in lohis:
+                indexes[lo:hi] = sorted(indexes[lo:hi],key=self._data[col].__getitem__)
+            self._data[col][:] = map(self._data[col].__getitem__,indexes)
+            if col != indx[-1]: lohis = list(chain.from_iterable(self._sub_lohis(lo, hi, self._data[col]) for lo, hi in lohis))
 
-        if rows:
-            assert len(rows[0]) == len(self._col_names), "A column entry was not provided for every column"
-            assert len(set(map(len,rows))) == 1, "Different sized row entries were provided."
+        for col in self._data.keys()-set(indx):
+            self._data[col][:] = map(self._data[col].__getitem__,indexes)
 
-            for col,new in zip(self._col_chunks,zip(*rows)):
-                col.append(new)
+        self._indexes = tuple(indx)
+        self._lohis = self._calc_lohis()
 
         return self
 
-    def filter(self, row_pred:Callable[[Sequence[Any]],bool] = None, comparison:Literal['default','=','<=','<','>','>=','match','in']="default", **kwargs) -> 'Table':
-        """Filter to specific rows. Applied as an Or. To "And" call filter multiple times.
+    def where(self, row_pred:Callable[[Sequence],bool] = None, comparison:Literal['=','<=','<','>','>=','match','in'] = None, **kwargs) -> 'Table':
+        """Filter to specific rows.
 
         Args:
-            pred: A predicate that returns true for row dictionaries that should be kept.
+            pred: A predicate that accepts rows and returns true for rows that should be kept.
             kwargs: key value pairs where the key is the column and the value indicates what
                 value a row should have in that column to be kept. Keeping logic depends on
                 the row value type and the kwargs value type. If kwarg value == row value keep
                 the row. If kwarg value is callable pass the row value to the predicate. If
                 kwarg value is a collection keep the row if the row value is in the collection.
                 If kwarg value is a string apply a regular expression match to the row value.
         """
 
-        keep = list(map(row_pred,self)) if row_pred else [False]*len(self) if kwargs else [True]*len(self)
+        if not row_pred and not kwargs:
+            return self
 
-        is_default_comparison = comparison == 'default'
+        if row_pred:
+            selection = list(compress(count(),map(row_pred,self[:])))
+            return Table(View(self._data,selection), self._columns, self._indexes) 
+ 
+        if kwargs:
+            selection = []
+            for kw,arg in kwargs.items():
+                if kw in self._indexes and comparison != "match" and not callable(kwargs[kw]):
+                    for lo,hi in self._lohis[kw]:
+                        for l,h in self._compare(lo,hi,self._data[kw],arg,comparison,"bisect"):
+                            selection.extend(range(l,h))
+                else:
+                    selection.extend(self._compare(0,len(self),self._data[kw],arg,comparison,"foreach"))
 
-        for filter_col, filter_val in kwargs.items():
+            selection=sorted(set(selection))
+            return Table(View(self._data,selection), self._columns, self._indexes)
 
-            chunks = self._col_chunks[self._col_names.index(filter_col)]
+    def groupby(self, level:int) -> Iterable['Table']:
+        for l,h in self._lohis[self._indexes[level]]:
+            yield Table(View(self._data, slice(l,h)), self._columns, self._indexes)
 
-            if is_default_comparison:
-                if isinstance(filter_val,collections.abc.Container) and not isinstance(filter_val,str):
-                    comparison = 'in'
-                else:
-                    comparison = "="
+    def copy(self) -> 'Table':
+        return Table(dict(self._data), tuple(self._columns), tuple(self._indexes))
 
-            if callable(filter_val):
-                keep = list(map(or_,keep,map(filter_val,chain.from_iterable(chunks))))
+    def to_pandas(self):
+        """Turn the Table into a Pandas data frame."""
 
-            elif comparison == "in":
-                try:
-                    filter_val = set(filter_val)
-                except:
-                    pass
+        PackageChecker.pandas("Table.to_pandas")
+        import pandas as pd
 
-                compare = contains
+        #data must be dict instance to work as desired
+        data = {k:self._data[k] for k in self._data}
+        return pd.DataFrame(data, columns=self.columns)
 
-                new_keep = []
-                i = 0
+    def to_dicts(self) -> Iterable[Mapping[str,Any]]:
+        """Turn the Table into a sequence of tuples."""
 
-                for chunk in chunks:
-                    if chunk.__class__ is Repeat:
-                        if compare(filter_val,chunk.value):
-                            new_keep.extend(repeat(True,len(chunk)))
-                        else:
-                            new_keep.extend(keep[i:i+len(chunk)])
-                    else:
-                        new_keep.extend(map(or_,keep[i:i+len(chunk)],map(compare,repeat(filter_val),chunk)))
+        for i in range(len(self)):
+            yield {c:self._data[c][i] for c in self._columns}
 
-                    i+=len(chunk)
+    def __getitem__(self,idx1):
 
-                keep = new_keep
+        if isinstance(idx1,str):
+            return self._data[idx1]
 
-            elif comparison == "=":
-                compare = eq
+        if isinstance(idx1,slice) and idx1.start is None and idx1.stop is None and idx1.step is None:
+            idx1 = self.columns
 
-                new_keep = []
-                i = 0
+        if isinstance(idx1,collections.abc.Collection):
+            return list(zip(*(self._data[col] for col in idx1)))
 
-                for chunk in chunks:
-                    if chunk.__class__ is Repeat:
-                        if compare(filter_val,chunk.value):
-                            new_keep.extend(repeat(True,len(chunk)))
-                        else:
-                            new_keep.extend(keep[i:i+len(chunk)])
-                    else:
-                        new_keep.extend(map(or_,keep[i:i+len(chunk)],map(compare,repeat(filter_val),chunk)))
+        raise KeyError(idx1)
 
-                    i+=len(chunk)
+    def __iter__(self) -> Iterator[Sequence[Any]]:
+        return iter(self[:])
 
-                keep = new_keep
+    def __str__(self) -> str:
+        return str({"Columns": self.columns, "Rows": len(self)})
 
-            elif comparison in ["<","<=",">=",">"]:
-                compare = [lt,le,ge,gt][["<","<=",">=",">"].index(comparison)]
+    def __len__(self) -> int:
+        return len(self._data[next(iter(self._data))]) if self._data else 0
 
-                new_keep = []
-                i = 0
-
-                for chunk in chunks:
-                    if chunk.__class__ is Count:
-                        pass
-                        lower = compare(chunk.start,filter_val)
-                        equal = compare(filter_val ,filter_val)
-                        upper = compare(chunk.end  ,filter_val)
-
-                        if lower==upper:
-                            if lower:
-                                new_keep.extend(repeat(True,len(chunk)))
-                            else:
-                                new_keep.extend(keep[i:i+len(chunk)])
-                        else:
-                            n_lower = filter_val-chunk.start
-                            n_equal = int((chunk.end-filter_val)>0)
-                            n_upper = chunk.end-filter_val-1
-
-                            if lower:
-                                new_keep.extend(repeat(True,n_lower))
-                            else:
-                                new_keep.extend(keep[i:i+n_lower])
-
-                            if n_equal:
-                                new_keep.append(keep[i+n_lower] or equal)
-
-                            if upper:
-                                new_keep.extend(repeat(True,n_upper))
-                            else:
-                                new_keep.extend(keep[i+n_lower+1:i+n_lower+1+n_upper])
-                    elif chunk.__class__ is Repeat:
-                        if compare(chunk.value, filter_val):
-                            new_keep.extend(repeat(True,len(chunk)))
-                        else:
-                            new_keep.extend(keep[i:i+len(chunk)])
-                    else:
-                        new_keep.extend(map(or_,keep[i:i+len(chunk)],map(compare,chunk,repeat(filter_val))))
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o,Table) and o._data == self._data
 
-                    i+=len(chunk)
+    def _ipython_display_(self):
+        #pretty print in jupyter notebook (https://ipython.readthedocs.io/en/stable/config/integrating.html)
+        print(str(self))
 
-                keep = new_keep
+    def _calc_lohis(self):
 
-            elif comparison == 'match':
+        if not self._indexes: return {}
 
-                is_sequence = isinstance(filter_val,collections.abc.Sequence) and not isinstance(filter_val,str)
-                filter_vals = filter_val if is_sequence else [filter_val]
-                values      = list(chain.from_iterable(chunks))
+        lohis = [[(0,len(self))]]
 
-                for filter_val in filter_vals:
-                    if isinstance(filter_val,Number) and isinstance(values[0],Number):
-                        keep = [a or v == filter_val for a,v in zip(keep,values)]
-                    elif isinstance(filter_val,Number) and isinstance(values[0],str):
-                        _re = re.compile(f'(\D|^){filter_val}(\D|$)')
-                        keep = [a or bool(_re.search(v)) for a,v in zip(keep,values)]
-                    elif isinstance(filter_val,str) and isinstance(values[0],str):
-                        _re = re.compile(filter_val)
-                        keep = [a or filter_val == v or bool(_re.search(v)) for a,v in zip(keep,values)]
+        for k in self._indexes[:-1]:
+            indexcol = self._data[k]
+            lohis.append([lh for lo,hi in lohis[-1] for lh in self._sub_lohis(lo,hi,indexcol)])
 
-        return Table(self, keep)
+        return dict(zip(self._indexes,lohis))
 
-    def to_pandas(self) -> Any:
-        """Turn the Table into a Pandas data frame."""
+    def _sub_lohis(self,lo,hi,col):
+        while lo != hi:
+            new_hi = bisect_right(col,col[lo],lo,hi)
+            yield (lo,new_hi)
+            lo = new_hi
 
-        PackageChecker.pandas("Table.to_pandas")
-        import pandas as pd
-        return pd.DataFrame(self.row_values(), columns=self.col_names)
+    def _compare(self,lo,hi,col,arg,comparison,method):
 
-    def to_dicts(self) -> Sequence[Mapping[str,Any]]:
-        """Turn the Table into a sequence of tuples."""
-        return [dict(zip(self.col_names,row)) for row in self]
+        if method != "bisect" or callable(arg): 
+            col = col[lo:hi]
 
-    def __iter__(self) -> Iterator[Sequence[Any]]:
-        return iter(zip(*self.col_values()))
+        if callable(arg):
+            return list(compress(count(lo),map(arg,col)))
 
-    def __str__(self) -> str:
-        return str({"Columns": self.col_names, "Rows": len(self)})
+        if comparison == "in" or (comparison is None and isinstance(arg,collections.abc.Iterable) and not isinstance(arg,str)):
+            if method == "bisect":
+                return [ (bisect_left(col,v,lo,hi),bisect_right(col,v,lo,hi)) for v in arg ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c in arg ]
 
-    def __len__(self) -> int:
-        if self._col_chunks:
-            return sum(map(len,self._col_chunks[0]))
-        return 0
+        if comparison == "=" or (comparison is None and (not isinstance(arg,collections.abc.Iterable) or isinstance(arg,str))):
+            if method == "bisect":
+                return [ (bisect_left(col,arg,lo,hi),bisect_right(col,arg,lo,hi)) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c == arg ]
 
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,Table) and o.col_names == self.col_names and all(r1==r2 for r1,r2 in zip(o.row_values(),self.row_values()))
+        if comparison == "<":
+            if method == "bisect":
+                return [ (lo,bisect_left(col,arg,lo,hi)) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c < arg ]
 
-    def _ipython_display_(self):
-        #pretty print in jupyter notebook (https://ipython.readthedocs.io/en/stable/config/integrating.html)
-        print(str(self))
+        if comparison == "<=":
+            if method == "bisect":
+                return [ (lo,bisect_right(col,arg,lo,hi)) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c <= arg ]
 
-class TransactionIO_V4(Source['Result'], Sink[Any]):
+        if comparison == ">=":
+            if method == "bisect":
+                return [ (bisect_left(col,arg,lo,hi), hi) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c >= arg ]
 
-    def __init__(self, log_file: Optional[str] = None, minify:bool=True) -> None:
+        if comparison == ">":
+            if method == "bisect":
+                return [ (bisect_right(col,arg,lo,hi), hi) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c > arg ]
+
+        if comparison == "match":
+            if isinstance(arg,Number) and col and isinstance(col[0],Number):
+                return [ i for i,c in enumerate(col,lo) if c == arg ]
+            elif isinstance(arg,Number) and isinstance(col[0],str):
+                _re = re.compile(f'(\D|^){arg}(\D|$)')
+                return [ i for i,c in enumerate(col,lo) if _re.search(c) ]
+            elif isinstance(arg,str) and isinstance(col[0],str):
+                _re = re.compile(arg)
+                return [ i for i,c in enumerate(col,lo) if _re.search(c) ]
+
+class TransactionIO_V3(Source['Result'], Sink[Any]):
+
+    def __init__(self, log_file: Optional[str] = None, minify:bool = True) -> None:
 
         self._log_file = log_file
         self._minify   = minify
         self._source   = DiskSource(log_file) if log_file else IterableSource()
-        self._sink     = DiskSink(log_file)   if log_file else ListSink(self._source.iterable)
+        self._sink     = DiskSink(log_file) if log_file else ListSink(self._source.iterable)
 
     def write(self, item: Any) -> None:
         if isinstance(self._sink, ListSink):
             self._sink.write(self._encode(item))
         else:
-            if not Path(self._sink._filename).exists():self._sink.write('["version",4]')
+            if not Path(self._sink._filename).exists():self._sink.write('["version",3]')
             self._sink.write(JsonEncode(self._minify).filter(self._encode(item)))
 
     def read(self) -> 'Result':
-
-        exp_dict = {}
+        n_lrns   = None
+        n_envs   = None
         lrn_rows = {}
         env_rows = {}
         int_rows = {}
 
         if isinstance(self._source, IterableSource):
             decoded_source = self._source
         else:
             decoded_source = Pipes.join(self._source, Foreach(JsonDecode()))
 
         for trx in decoded_source.read():
 
             if not trx: continue
 
-            if trx[0] == "experiment":
-                exp_dict = trx[1]
+            if trx[0] == "benchmark":
+                n_lrns = trx[1]["n_learners"]
+                n_envs = trx[1]["n_simulations"]
 
-            if trx[0] == "E":
+            if trx[0] == "S":
                 env_rows[trx[1]] = trx[2]
 
             if trx[0] == "L":
                 lrn_rows[trx[1]] = trx[2]
 
             if trx[0] == "I":
                 int_rows[tuple(trx[1])] = trx[2]
 
-        return Result(*old_to_new(env_rows, lrn_rows, int_rows), exp_dict)
+        return Result(*old_to_new(env_rows, lrn_rows, int_rows), {"n_learners":n_lrns,"n_environments":n_envs})
 
     def _encode(self,item):
         if item[0] == "T0":
-            return ['experiment', {"n_learners":item[1], "n_environments":item[2], "description":None} if len(item)==3 else item[1] ]
+            return ['benchmark', {"n_learners":item[1], "n_simulations":item[2]}]
 
         if item[0] == "T1":
             return ["L", item[1], item[2]]
 
         if item[0] == "T2":
-            return ["E", item[1], item[2]]
+            return ["S", item[1], item[2]]
 
         if item[0] == "T3":
             rows_T = collections.defaultdict(list)
 
             for row in item[2]:
                 for col,val in row.items():
                     rows_T[col].append(val)
 
             return ["I", item[1], { "_packed": rows_T }]
 
         return None
 
-class TransactionIO_V3(Source['Result'], Sink[Any]):
+class TransactionIO_V4(Source['Result'], Sink[Any]):
 
-    def __init__(self, log_file: Optional[str] = None, minify:bool = True) -> None:
+    def __init__(self, log_file: Optional[str] = None, minify:bool=True) -> None:
 
         self._log_file = log_file
         self._minify   = minify
         self._source   = DiskSource(log_file) if log_file else IterableSource()
-        self._sink     = DiskSink(log_file) if log_file else ListSink(self._source.iterable)
+        self._sink     = DiskSink(log_file)   if log_file else ListSink(self._source.iterable)
 
     def write(self, item: Any) -> None:
         if isinstance(self._sink, ListSink):
             self._sink.write(self._encode(item))
         else:
-            if not Path(self._sink._filename).exists():self._sink.write('["version",3]')
+            if not Path(self._sink._filename).exists():self._sink.write('["version",4]')
             self._sink.write(JsonEncode(self._minify).filter(self._encode(item)))
 
     def read(self) -> 'Result':
-        n_lrns   = None
-        n_envs   = None
+
+        exp_dict = {}
         lrn_rows = {}
         env_rows = {}
         int_rows = {}
 
         if isinstance(self._source, IterableSource):
             decoded_source = self._source
         else:
             decoded_source = Pipes.join(self._source, Foreach(JsonDecode()))
 
         for trx in decoded_source.read():
 
             if not trx: continue
 
-            if trx[0] == "benchmark":
-                n_lrns = trx[1]["n_learners"]
-                n_envs = trx[1]["n_simulations"]
+            if trx[0] == "experiment":
+                exp_dict = trx[1]
 
-            if trx[0] == "S":
+            if trx[0] == "E":
                 env_rows[trx[1]] = trx[2]
 
             if trx[0] == "L":
                 lrn_rows[trx[1]] = trx[2]
 
             if trx[0] == "I":
                 int_rows[tuple(trx[1])] = trx[2]
 
-        return Result(*old_to_new(env_rows, lrn_rows, int_rows), {"n_learners":n_lrns,"n_environments":n_envs})
+        return Result(*old_to_new(env_rows, lrn_rows, int_rows), exp_dict)
 
     def _encode(self,item):
         if item[0] == "T0":
-            return ['benchmark', {"n_learners":item[1], "n_simulations":item[2]}]
+            return ['experiment', {"n_learners":item[1], "n_environments":item[2], "description":None} if len(item)==3 else item[1] ]
 
         if item[0] == "T1":
             return ["L", item[1], item[2]]
 
         if item[0] == "T2":
-            return ["S", item[1], item[2]]
+            return ["E", item[1], item[2]]
 
         if item[0] == "T3":
             rows_T = collections.defaultdict(list)
 
+            keys = set().union(*[r.keys() for r in item[2]])
+
             for row in item[2]:
-                for col,val in row.items():
-                    rows_T[col].append(val)
+                for key in keys:
+                    rows_T[key].append(row.get(key,None))
 
             return ["I", item[1], { "_packed": rows_T }]
 
         return None
 
 class TransactionIO(Source['Result'], Sink[Any]):
 
@@ -706,51 +686,42 @@
                 plt.close()
 
 class FilterPlottingData:
 
     def filter(self, unfinished:'Result', x:Sequence[str], y:str) -> Table:
 
         if len(unfinished.interactions) == 0: raise CobaException("This result doesn't contain any evaluation data to plot.")
-        if y not in unfinished.interactions.col_names: raise CobaException(f"{y} is not available in the environment. Plotting has been stopped.")
+        if y not in unfinished.interactions.columns: raise CobaException(f"{y} is not available in the environment. Plotting has been stopped.")
 
         finished = unfinished.filter_fin('min' if x == ['index'] else None)
 
         if len(finished.learners) == 0:
-            raise CobaException("This result does not contain an environment which has been finished for every learner. Plotting has been stopped.")
+            raise CobaException("This result does not contain an environment that has been finished for every learner. Plotting has been stopped.")
 
         if len(finished.environments) != len(unfinished.environments):
             CobaContext.logger.log("Environments not present for all learners have been excluded. To supress this call filter_fin() before plotting.")
 
-        if max(map(len, finished.interactions._col_chunks[2])) != max(map(len, unfinished.interactions._col_chunks[2])) > 1 and x == ['index']:
+        if len(set(map(len,unfinished.interactions.groupby(2)))) > 1 and x == ['index']:
             CobaContext.logger.log("This result contains environments of different lengths. The plot only includes interactions up to the shortest environment. To supress this warning in the future call <result>.filter_fin(n_interactions) before plotting.")
 
         return finished.interactions
 
 class SmoothPlottingData:
 
     def filter(self, interactions:Table, y:str, span:Optional[int]) -> Sequence[Mapping[str,Any]]:
 
-        try:#pragma: no cover
-            #I'm not crazy about this because it depends on some implementation details but it is too fast not to
-            y_index = interactions.col_names.index(y)
-            out     = []
-
-            for eid, lid, Y in zip(*interactions._col_chunks[:2], interactions._col_chunks[y_index]):
-                out.append({"environment_id":eid.value, "learner_id":lid.value, y:moving_average(Y,span)})
-
+        try:
+            out = []
+            for table in interactions.groupby(2):
+                out.append({"environment_id":table['environment_id'][0], "learner_id":table['learner_id'][0], y:moving_average(table[y],span)})
             return out
-        except:
-            Y = interactions.col_values()[interactions.col_names.index(y)]
-            G = iter(zip(*interactions.col_values()[:2]))
-
+        except:#pragma: no cover
             out = []
-
-            for g, _Y in groupby(Y, lambda key, G=G: next(G)):
-                out.append({"environment_id":g[0], "learner_id":g[1], y:moving_average(list(_Y),span)})
-
+            for g, Y in groupby(interactions[["environment_id","learner_id", y]], itemgetter(slice(2))):
+                out.append({"environment_id":g[0], "learner_id":g[1], y:moving_average(list(Y),span)})
             return out
 
 class ContrastPlottingData:
 
     def filter(self, rows:Sequence[Mapping[str,Any]], y:str, mode:Union[Literal["diff","prob",'scat'],Callable[[float,float],float]], learner_id1:int) -> Sequence[Mapping[str,Any]]:
 
         sort_key  = lambda row: (row['environment_id'], 0 if row['learner_id']==learner_id1 else 1)
@@ -828,71 +799,96 @@
 
         if not Path(filename).exists():
             raise CobaException("We were unable to find the given Result file.")
 
         return TransactionIO(filename).read()
 
     @staticmethod
-    def from_logged_envs(environments: Sequence[Environment]):
+    def from_logged_envs(environments: Iterable[Environment],include_probability:bool=False):
 
-        environments = [e for e in environments if e.params.get('logged')]
-
-        envs_params = []
-        lrns_params = []
+        env_param_list = []
+        lrn_param_list = []
+        env_param_dict = {}
+        lrn_param_dict = {}
 
         env_rows = {}
         lrn_rows = {}
         int_rows = {}
 
+        def determine_id(param,param_list,param_dict):
+            try:
+                key = frozenset(param.items())
+                if key not in param_dict:
+                    param_dict[key] = len(param_list)
+                    param_list.append(param)
+                return param_dict[key]
+            except:
+                try:
+                    return param_list.index(param)
+                except:
+                    param_list.append(param)
+                    return len(param_list)-1
+
         my_mean = lambda x: sum(x)/len(x)
 
         for env in environments:
 
-            is_batched = 'batched' in env.params
-            env_params  = dict(env.params)
-            lrn_params  = env_params.pop('learner')
+            first, interactions = peek_first(env.read())
 
-            try:
-                env_id = envs_params.index(env_params)
-            except:
-                env_id = len(envs_params)
-                envs_params.append(env_params)
-                env_rows[env_id] = env_params
+            if not env.params.get('logged'): continue
+            if not interactions: continue
 
-            try:
-                lrn_id = lrns_params.index(lrn_params)
-            except:
-                lrn_id = len(lrns_params)
-                lrns_params.append(lrn_params)
-                lrn_rows[lrn_id] = lrn_params
+            is_batched = isinstance(first['reward'],(Batch,list,tuple))
+            env_param = dict(env.params)
+            lrn_param = env_param.pop('learner')
+
+            env_id = determine_id(env_param,env_param_list,env_param_dict)
+            lrn_id = determine_id(lrn_param,lrn_param_list,lrn_param_dict)
+
+            if env_id not in env_rows: env_rows[env_id] = env_param
+            if lrn_id not in lrn_rows: lrn_rows[lrn_id] = lrn_param
+
+            keys = first.keys() - {'context', 'actions', 'rewards'}
+            if not include_probability: keys -= {'probability'}
+
+            _packed = {k:[] for k in keys}
+            results = {"_packed": _packed}
 
             if is_batched:
-                results = {'_packed':{'reward': list(map(my_mean,map(itemgetter('reward'),env.read())))}}
+                for interaction in interactions:
+                    for k in keys:
+                        _packed[k].append(my_mean(interaction[k]))
             else:
-                results = {'_packed':{'reward': list(map(itemgetter('reward'),env.read())) }}
+                for interaction in interactions:
+                    for k in keys:
+                        _packed[k].append(interaction[k])
 
             int_rows[(env_id,lrn_id)]= results
 
         return Result(*old_to_new(env_rows,lrn_rows,int_rows))
 
     def __init__(self,
-        env_rows: Union[Sequence,Table] = Table([]),
-        lrn_rows: Union[Sequence,Table] = Table([]),
-        int_rows: Union[Sequence,Table] = Table([]),
+        env_rows: Union[Sequence,Table] = Table(),
+        lrn_rows: Union[Sequence,Table] = Table(),
+        int_rows: Union[Sequence,Table] = Table(),
         exp_dict: Mapping  = {}) -> None:
         """Instantiate a Result class.
 
         This constructor should never be called directly. Instead a Result file should be created
         from an Experiment and the result file should be loaded via Result.from_file(filename).
         """
         self.experiment = exp_dict
 
-        self._environments = env_rows if isinstance(env_rows,Table) else Table(env_rows[0]).insert(rows=env_rows[1:])
-        self._learners     = lrn_rows if isinstance(lrn_rows,Table) else Table(lrn_rows[0]).insert(rows=lrn_rows[1:])
-        self._interactions = int_rows if isinstance(int_rows,Table) else Table(int_rows[0]).insert(rows=int_rows[1:])
+        self._environments = env_rows if isinstance(env_rows,Table) else Table(columns=env_rows[0]).insert(env_rows[1:])
+        self._learners     = lrn_rows if isinstance(lrn_rows,Table) else Table(columns=lrn_rows[0]).insert(lrn_rows[1:])
+        self._interactions = int_rows if isinstance(int_rows,Table) else Table(columns=int_rows[0]).insert(int_rows[1:])
+
+        self._environments.index('environment_id'                     )
+        self._learners    .index(                 'learner_id'        )
+        self._interactions.index('environment_id','learner_id','index')
 
         self._plotter = MatplotlibPlotter()
 
     @property
     def learners(self) -> Table:
         """The collection of learners used in the Experiment.
 
@@ -920,67 +916,67 @@
 
     def set_plotter(self, plotter: Plotter) -> None:
         """Manually set the underlying plotting tool. By default matplotlib is used though this can be changed."""
         self._plotter = plotter
 
     def copy(self) -> 'Result':
         """Create a copy of Result."""
-        return Result(Table(self.environments), Table(self.learners), Table(self.interactions), self.experiment)
+        return Result(self.environments.copy(), self.learners.copy(), self.interactions.copy(), dict(self.experiment))
 
     def filter_fin(self, n_interactions: Union[int,Literal['min']] = None) -> 'Result':
         """Filter the result to only contain data about environments with all learners and interactions.
 
         Args:
             n_interactions: The number of interactions at which an environment is considered complete.
         """
         interactions = self.interactions
         learners     = self.learners
         environments = self.environments
 
-        env_lengths, env_lrn_cnts = env_len_lrn_counts(interactions)
-        if n_interactions == 'min': n_interactions = min(env_lengths.values())
+        env_lens, env_cnts = env_len_and_cnt(interactions)
+        n_interactions = min(env_lens.values()) if n_interactions == "min" else n_interactions
 
         def has_all(env_id):
-            return env_lrn_cnts[env_id] == len(learners)
+            return env_cnts.get(env_id,-1) == len(learners)
 
         def has_min(env_id):
-            return n_interactions == None or env_lengths[env_id] >= n_interactions
+            return n_interactions == None or env_lens.get(env_id,-1) >= n_interactions
 
-        complete_ids = set([env_id for env_id in environments.col_values()[0] if has_all(env_id) and has_min(env_id)])
+        complete_ids = set([env_id for env_id in environments["environment_id"] if has_all(env_id) and has_min(env_id)])
 
-        if complete_ids != set(env_lengths.keys()):
-            environments = environments.filter(environment_id=complete_ids)
-            interactions = interactions.filter(environment_id=complete_ids)
+        if complete_ids != set(env_lens.keys()):
+            environments = environments.where(environment_id=complete_ids)
+            interactions = interactions.where(environment_id=complete_ids)
 
-        if n_interactions and {n_interactions} != set(env_lengths.values()):
-            interactions = interactions.filter(index=n_interactions,comparison="<=")
+        if n_interactions and {n_interactions} != set(env_lens.values()):
+            interactions = interactions.where(index=n_interactions,comparison="<=")
 
         if len(environments) == 0:
-            learners = learners.filter(lambda _:False)
+            learners = learners.where(lambda _:False)
             CobaContext.logger.log(f"There was no environment which was finished for every learner.")
 
         return Result(environments, learners, interactions, self.experiment)
 
     def filter_env(self, pred:Callable[[Mapping[str,Any]],bool] = None, **kwargs: Any) -> 'Result':
         """Filter the result to only contain data about specific environments.
 
         Args:
             pred: A predicate that returns true for learner dictionaries that should be kept.
             **kwargs: key-value pairs to filter on. To see filtering options see Table.filter.
         """
 
         if len(self.environments) == 0: return self
 
-        environments = self.environments.filter(pred, **kwargs)
+        environments = self.environments.where(pred, **kwargs)
         learners     = self.learners
         interactions = self.interactions
 
         if len(environments) != len(self.environments):
-            interactions = interactions.filter(environment_id=set(environments.col_values()[0]))
-            learners     = learners    .filter(learner_id    =set(interactions.col_values()[1]))
+            interactions = interactions.where(environment_id=set(environments["environment_id"]))
+            learners     = learners    .where(learner_id    =set(interactions["learner_id"]))
 
         if len(environments) == 0:
             CobaContext.logger.log(f"No environments matched the given filter.")
 
         return Result(environments,learners,interactions,self.experiment)
 
     def filter_lrn(self, pred:Callable[[Mapping[str,Any]],bool] = None, **kwargs: Any) -> 'Result':
@@ -989,20 +985,20 @@
         Args:
             pred: A predicate that returns true for learner dictionaries that should be kept.
             **kwargs: key-value pairs to filter on. To see filtering options see Table.filter.
         """
         if len(self.learners) == 0: return self
 
         environments = self.environments
-        learners     = self.learners.filter(pred, **kwargs)
+        learners     = self.learners.where(pred, **kwargs)
         interactions = self.interactions
 
         if len(learners) != len(self.learners):
-            interactions = self.interactions.filter(learner_id    =set(learners.col_values()[0]))
-            environments = self.environments.filter(environment_id=set(interactions.col_values()[0]))
+            interactions = self.interactions.where(learner_id    =set(learners["learner_id"]))
+            environments = self.environments.where(environment_id=set(interactions["environment_id"]))
 
         if len(learners) == 0:
             CobaContext.logger.log(f"No learners matched the given filter.")
 
         return Result(environments,learners,interactions)
 
     def plot_contrast(self,
@@ -1057,15 +1053,15 @@
                 raise CobaException("plot_contrast does not currently support contrasting by `index`.")
 
             rows = FilterPlottingData().filter(self.filter_lrn(learner_id=[learner_id1, learner_id2]), x, y)
             rows = SmoothPlottingData().filter(rows, y, span)
             rows = ContrastPlottingData().filter(rows, y, mode, learner_id1)
 
             envs = self.environments
-            XYE = TransformToXYE().filter(rows, { row[0]:dict(zip(envs.col_names,row)) for row in envs }, x, y, err)
+            XYE = TransformToXYE().filter(rows, { row[0]:dict(zip(envs.columns,row)) for row in envs }, x, y, err)
 
             if x != ['index']:
                 XYE = sorted(XYE, key=lambda xye: xye[1], reverse=reverse)
 
             bound = .5 if mode == "prob" else 0
 
             win,tie,loss = [],[],[]
@@ -1165,15 +1161,15 @@
 
             self._validate_parameters(x)
 
             rows = FilterPlottingData().filter(self, x, y)
             rows = SmoothPlottingData().filter(rows, y, span)
 
             envs     = self.environments
-            env_rows = { row[0]:dict(zip(envs.col_names,row)) for row in envs }
+            env_rows = { row[0]:dict(zip(envs.columns,row)) for row in envs }
             get_key  = lambda row: row['learner_id']
             lines    = []
 
             style = "-" if x == ['index'] else "."
 
             def get_color(colors:Union[None,Sequence[Union[str,int]]], i:int):
                 try:
@@ -1218,16 +1214,16 @@
             self._plotter.plot(ax, lines, title, xlabel, ylabel, xlim, ylim, xticks, yticks, xrotation, yrotation, out)
         except CobaException as e:
             CobaContext.logger.log(str(e))
 
     def _full_name(self,lrn_id:int) -> str:
         """A user-friendly name created from a learner's params for reporting purposes."""
 
-        cols = self.learners.col_names
-        vals = list(self.learners.row_values())[list(self.learners.col_values()[0]).index(lrn_id)]
+        cols = self.learners.columns
+        vals = self.learners.where(learner_id=lrn_id)[:][0]
 
         values = dict((k,v) for k,v in zip(cols,vals) if v is not None)
         family = values.get('family',values['learner_id'])
         params = f"({','.join(f'{k}={v}' for k,v in values.items() if k not in ['family','learner_id'])})"
 
         return family if params == '()' else family+params
```

### Comparing `coba-6.4.2/coba/learners/__init__.py` & `coba-6.5.0/coba/learners/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """This module contains all public learners and learner interfaces."""
 
-from coba.learners.primitives import Learner, SafeLearner, PMF, ActionScore
+from coba.learners.primitives import Learner, PMF, ActionProb
+from coba.learners.safety     import SafeLearner
 from coba.learners.bandit     import EpsilonBanditLearner, UcbBanditLearner, FixedLearner, RandomLearner
 from coba.learners.corral     import CorralLearner
 from coba.learners.vowpal     import VowpalMediator
 from coba.learners.vowpal     import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner
 from coba.learners.vowpal     import VowpalCoverLearner, VowpalRegcbLearner, VowpalSquarecbLearner, VowpalOffPolicyLearner
 from coba.learners.linucb     import LinUCBLearner
 
 __all__ = [
     'PMF',
-    'ActionScore',
+    'ActionProb',
     'Learner',
     'SafeLearner',
     'RandomLearner',
     'FixedLearner',
     'EpsilonBanditLearner',
     'UcbBanditLearner',
     'CorralLearner',
```

### Comparing `coba-6.4.2/coba/learners/bandit.py` & `coba-6.5.0/coba/learners/bandit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import math
 
 from collections import defaultdict
-from typing import Any, Dict, Optional, cast, Hashable
+from typing import Any, Mapping, Sequence, Optional, Hashable
 
 from coba.primitives import Context, Action, Actions
 from coba.statistics import OnlineVariance
-from coba.learners.primitives import Learner, PMF, PMF, requires_hashables
+from coba.learners.primitives import Learner, PMF, PMF, Prob, requires_hashables
 
 @requires_hashables
 class EpsilonBanditLearner(Learner):
     """A bandit learner using epsilon-greedy for exploration."""
 
     def __init__(self, epsilon: float=.05) -> None:
         """Instantiate an EpsilonBanditLearner.
 
         Args:
             epsilon: We explore with probability epsilon and exploit otherwise.
         """
 
         self._epsilon = epsilon
 
-        self._N: Dict[Hashable, int            ] = defaultdict(int)
-        self._Q: Dict[Hashable, Optional[float]] = defaultdict(int)
+        self._N: Mapping[Hashable, int            ] = defaultdict(int)
+        self._Q: Mapping[Hashable, Optional[float]] = defaultdict(int)
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
         return {"family": "epsilon_bandit", "epsilon": self._epsilon }
 
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        values    = [ self._Q[action] for action in actions ]
+        max_value = None if set(values) == {None} else max(v for v in values if v is not None)
+        max_count = sum(v==max_value for v in values)
+
+        prob_selected_randomly = 1/len(actions) * self._epsilon
+        prob_selected_greedily = 1/max_count * (1-self._epsilon)
+
+        return [ prob_selected_randomly + int(self._Q[action]==max_value)*prob_selected_greedily for action in request ]
+
     def predict(self, context: Context, actions: Actions) -> PMF:
         values      = [ self._Q[action] for action in actions ]
         max_value   = None if set(values) == {None} else max(v for v in values if v is not None)
         max_indexes = [i for i in range(len(values)) if values[i]==max_value]
 
         prob_selected_randomly = [1/len(actions) * self._epsilon] * len(actions)
         prob_selected_greedily = [ int(i in max_indexes)/len(max_indexes) * (1-self._epsilon) for i in range(len(actions))]
 
         return PMF([p1+p2 for p1,p2 in zip(prob_selected_randomly,prob_selected_greedily)])
 
     def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
 
         alpha = 1/(self._N[action]+1)
-        old_Q = cast(float, 0 if self._Q[action] is None else self._Q[action])
+        old_Q = self._Q[action] or 0.0
 
         self._Q[action] = (1-alpha) * old_Q + alpha * reward
         self._N[action] = self._N[action] + 1
 
 @requires_hashables
 class UcbBanditLearner(Learner):
     """A bandit learner using upper confidence bound estimates for exploration.
@@ -57,38 +67,51 @@
         the multiarmed bandit problem." Machine learning 47.2-3 (2002): 235-256.
     """
 
     def __init__(self):
         """Instantiate a UcbBanditLearner."""
         #these variable names were selected for easier comparison with the original paper
         self._t     : int = 0
-        self._m     : Dict[Action, float         ] = {}
-        self._s     : Dict[Action, int           ] = {}
-        self._v     : Dict[Action, OnlineVariance] = {}
+        self._m     : Mapping[Action, float         ] = {}
+        self._s     : Mapping[Action, int           ] = {}
+        self._v     : Mapping[Action, OnlineVariance] = {}
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
 
         return { "family": "UCB_bandit" }
 
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        never_observed_actions = set(actions) - self._m.keys()
+
+        if never_observed_actions:
+            max_actions = never_observed_actions
+        else:
+            values      = [ self._m[a] + self._Avg_R_UCB(a) for a in actions ]
+            max_value   = max(values)
+            max_actions = [ a for a,v in zip(actions,values) if v==max_value ]
+
+        return [int(action in max_actions)/len(max_actions) for action in request]
+
     def predict(self, context: Context, actions: Actions) -> PMF:
 
-        self._t += 1
-        never_observed_actions = [ a for a in actions if a not in self._m ]
+        never_observed_actions = set(actions) - self._m.keys()
 
         if never_observed_actions:
             max_actions = never_observed_actions
         else:
             values      = [ self._m[a] + self._Avg_R_UCB(a) for a in actions ]
             max_value   = max(values)
             max_actions = [ a for a,v in zip(actions,values) if v==max_value ]
 
         return PMF([int(action in max_actions)/len(max_actions) for action in actions])
 
     def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
+        
+        self._t += 1
 
         assert 0 <= reward and reward <= 1, "This algorithm assumes that reward has support in [0,1]."
 
         if action not in self._m:
             self._m[action] = reward
             self._s[action] = 1
             self._v[action] = OnlineVariance()
@@ -141,16 +164,20 @@
         """
 
         assert round(sum(pmf),3) == 1, "The given pmf must sum to one to be a valid pmf."
         assert all([p >= 0 for p in pmf]), "All given probabilities of the pmf must be greater than or equal to 0."
         self._pmf = pmf
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
         return {"family":"fixed"}
+    
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        probs = self._pmf
+        return [ probs[actions.index(a)] for a in request ]
 
     def predict(self, context: Context, actions: Actions) -> PMF:
         return PMF(self._pmf)
 
     def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
         pass
 
@@ -158,15 +185,18 @@
     """A learner that selects actions according to a uniform distribution."""
 
     def __init__(self):
         """Instantiate a RandomLearner."""
         pass
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
         return {"family":"random"}
+    
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        return [1/len(actions)]*len(request)
 
     def predict(self, context: Context, actions: Actions) -> PMF:
         return PMF([1/len(actions)]*len(actions))
 
     def learn(self, context: Context, actions: Actions, action: Action, reward: float, probability: float) -> None:
         pass
```

### Comparing `coba-6.4.2/coba/learners/corral.py` & `coba-6.5.0/coba/learners/corral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import math
 
-from typing import Any, Sequence, Optional, Dict, Tuple
+from typing import Any, Sequence, Optional, Mapping, Tuple
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.primitives import Context, Action
 
-from coba.learners.primitives import Learner, SafeLearner, PMF, kwargs, Actions
+from coba.learners.safety import SafeLearner
+from coba.learners.primitives import Learner, PMF, kwargs, Actions, Prob
 
 class CorralLearner(Learner):
     """A meta-learner that takes a collection of learners and determines
     which is best in an environment.
 
     This is an implementation of the Agarwal et al. (2017) Corral algorithm
     and requires that the reward is always in [0,1].
@@ -60,17 +61,21 @@
 
         self._mode = mode
 
         self._random_pick   = CobaRandom(seed)
         self._random_reject = CobaRandom(CobaRandom(seed).randint(0,1000))
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
         return { "family": "corral", "eta": self._eta_init, "mode":self._mode, "T": self._T, "B": [ str(b) for b in self._base_learners ], "seed":self._random_pick._seed }
 
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        probs = self.predict(context,actions)[0]
+        return [ probs[actions.index(a)] for a in request ]
+
     def predict(self, context: Context, actions: Sequence[Action]) -> Tuple[PMF,kwargs]:
 
         base_predicts = [ base_algorithm.predict(context, actions) for base_algorithm in self._base_learners ]
         base_actions, base_probs, base_infos = zip(*base_predicts)
 
         predict = [ sum([p_b*int(a==b_a) for p_b,b_a in zip(self._p_bars, base_actions)]) for a in actions ]
         info    = (base_actions, base_probs, base_infos)
```

### Comparing `coba-6.4.2/coba/learners/linucb.py` & `coba-6.5.0/coba/learners/linucb.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any, Dict, Sequence
+from typing import Any, Mapping, Sequence
 
 from coba.exceptions import CobaException
 from coba.utilities import PackageChecker
 from coba.primitives import Context, Action
 from coba.encodings import InteractionsEncoder
 
-from coba.learners.primitives import PMF, Actions, Learner
+from coba.learners.primitives import PMF, Learner, Actions, Prob
 
 class LinUCBLearner(Learner):
     """A contextual bandit learner that represents expected reward as a
     linear function of context and action features. Exploration is carried
     out according to upper confidence bound estimates.
 
     This is an implementation of the Chu et al. (2011) LinUCB algorithm using the
@@ -47,59 +47,62 @@
 
         self._X = features
         self._X_encoder = InteractionsEncoder(features)
 
         self._theta = None
         self._A_inv = None
 
+        import numpy as np
+        self._np = np
+
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> Mapping[str, Any]:
         return {'family': 'LinUCB', 'alpha': self._alpha, 'features': self._X}
 
-    def predict(self, context: Context, actions: Actions) -> PMF:
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        probs = self.predict(context,actions)
+        return [ probs[actions.index(a)] for a in request ]
 
-        import numpy as np
+    def predict(self, context: Context, actions: Actions) -> PMF:
 
         if isinstance(actions[0], dict) or isinstance(context, dict):
             raise CobaException("Sparse data cannot be handled by this implementation at this time.")
 
         if not context:
             self._X_encoder = InteractionsEncoder(list(set(filter(None,[ f.replace('x','') if isinstance(f,str) else f for f in self._X ]))))
 
         context = context or []
-        features: np.ndarray = np.array([self._X_encoder.encode(x=context,a=action) for action in actions]).T
+        features = self._np.array([self._X_encoder.encode(x=context,a=action) for action in actions]).T
 
         if(self._A_inv is None):
-            self._theta = np.zeros(features.shape[0])
-            self._A_inv = np.identity(features.shape[0])
+            self._theta = self._np.zeros(features.shape[0])
+            self._A_inv = self._np.identity(features.shape[0])
 
         point_estimate = self._theta @ features
-        point_bounds   = np.diagonal(features.T @ self._A_inv @ features)
+        point_bounds   = self._np.diagonal(features.T @ self._A_inv @ features)
 
-        action_values = point_estimate + self._alpha*np.sqrt(point_bounds)
-        max_indexes   = np.where(action_values == np.amax(action_values))[0]
+        action_values = point_estimate + self._alpha*self._np.sqrt(point_bounds)
+        max_indexes   = self._np.where(action_values == self._np.amax(action_values))[0]
 
         return PMF([int(ind in max_indexes)/len(max_indexes) for ind in range(len(actions))])
 
     def learn(self, context: Context, actions: Actions, action: Action, reward: float, probability: float) -> None:
 
-        import numpy as np
-
         if isinstance(action, dict) or isinstance(context, dict):
             raise CobaException("Sparse data cannot be handled by this algorithm.")
 
         if not context:
             self._X_encoder = InteractionsEncoder(list(set(filter(None,[ f.replace('x','') if isinstance(f,str) else f for f in self._X ]))))
 
         context = context or []
-        features: np.ndarray = np.array(self._X_encoder.encode(x=context,a=action)).T
+        features = self._np.array(self._X_encoder.encode(x=context,a=action)).T
 
         if(self._A_inv is None):
-            self._theta = np.zeros((features.shape[0]))
-            self._A_inv = np.identity(features.shape[0])
+            self._theta = self._np.zeros((features.shape[0]))
+            self._A_inv = self._np.identity(features.shape[0])
 
         r = self._theta @ features
         w = self._A_inv @ features
         v = features    @ w
 
-        self._A_inv = self._A_inv - np.outer(w,w)/(1+v)
+        self._A_inv = self._A_inv - self._np.outer(w,w)/(1+v)
         self._theta = self._theta + (reward-r)/(1+v) * w
```

### Comparing `coba-6.4.2/coba/learners/primitives.py` & `coba-6.5.0/coba/pipes/multiprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,361 +1,363 @@
-from collections import abc
-from math import isclose
-from abc import ABC, abstractmethod
-from itertools import repeat
-from typing import Any, Sequence, Union, Tuple, Callable, Mapping, Optional, Type
+import pickle
+import threading as mt
+import multiprocessing as mp
+
+from queue import Empty
+from traceback import format_tb
+from typing import Iterable, Mapping, Callable, Optional, Union, Sequence, Any
+from coba.backports import Literal
 
+from coba.utilities import peek_first
 from coba.exceptions import CobaException
-from coba.random import CobaRandom
-from coba.primitives import Context, Action, Actions
-from coba.primitives import Batch, Dense, Sparse, HashableDense, HashableSparse
-
-kwargs = Mapping[str,Any]
-Score  = float
-PDF    = Callable[[Action],float]
-
-class PMF(list):
-    pass
-
-class ActionScore(tuple):
-    def __new__(self, action: Action, score: Score):
-        return tuple.__new__(ActionScore, (action, score))
-
-Prediction = Union[
-    PDF,
-    PMF,
-    ActionScore,
-    Tuple[PDF         , kwargs],
-    Tuple[PMF         , kwargs],
-    Tuple[ActionScore , kwargs],
-    Tuple[Action,Score, kwargs],
-]
+from coba.pipes.primitives import Filter, Line, SourceSink
+from coba.pipes.filters import Slice
+from coba.pipes.sources import IterableSource, QueueSource
+from coba.pipes.sinks import QueueSink
+
+# handle not picklable (this is handled by explicitly pickling) (UNITTESTED)
+# handle empty list (this is done  naturally) (UNITTESTED)
+# handle exceptions in process (wrap worker executing code in an exception handler) (UNITTESTED)
+# handle AttributeErrors. This occurs when... (handled by Pickler) (UNITTESTED)
+
+# handle ctrl-c without hanging (manually tested)
+#   > This is super hard... I've been trying to do this for years... here are things I've done
+#   > I make all threads and processes daemons to protect against them not closing
+#   > When I'm done I shutdown in-queue loading and then empty both the in-queue and out-queue
+#   > I use try-finally idioms to close all queues that we create
+#   > I assert that all processes are in fact closed when passed to the callback
+
+# handle Experiment.evaluate not being called inside of __name__=='__main__' (manually tested)
+#   > Handled by checking exitcode on processes and using an event synchronizer on first process start
+
+#There are three potential contexts -- spawn, fork, and forkserver. On windows and mac spawn is the only option.
+#On Linux the default option is fork. Fork creates processes faster and can share memory but also doesn't play
+#well with threads. Therefore, to make behavior consistent across Linux, Windows, and Mac and avoid potential bugs
+#we force our multiprocessors to always use spawn.
+spawn_context = mp.get_context("spawn")
+
+class ProcessLine(spawn_context.Process):
+
+    ### We create a lock so that we can safely receive any possible exceptions. Empirical
+    ### tests showed that creating a Pipe and Lock doesn't seem to slow us down too much.
+
+    def __init__(self, line: Line, callback: Callable = None):
+
+        self._line      = line
+        self._callback  = callback
+        self._exception = None
+        self._traceback = None
+        self._poisoned  = False
+        super().__init__(daemon=True)
+
+    def start(self) -> None:
+        callback               = self._callback
+        self._callback         = None
+        self._recv, self._send = spawn_context.Pipe(False)
+        self._lock             = spawn_context.Lock()
+        super().start()
+
+        if callback:
+            def join_and_call(self=self):
+                self.join()
+                callback(self)
+            mt.Thread(target=join_and_call,daemon=True).start()
 
-class Learner(ABC):
-    """The Learner interface for contextual bandit learning."""
+    def run(self): #pragma: no cover (coverage can't be tracked for code that runs on background prcesses)
+        try:
+            self._line.run()
+        except Exception as e:
+            if str(e).startswith("Can't get attribute"):
+                ex,tb = CobaException(
+                    "We attempted to evaluate your code in multiple processes but we were unable to find all the code "
+                    "definitions needed to pass the tasks to the processes. The two most common causes of this error are: "
+                    "1) a learner or simulation is defined in a Jupyter Notebook cell or 2) a necessary class definition "
+                    "exists inside the `__name__=='__main__'` code block in the main execution script. In either case "
+                    "you can choose one of three simple solutions: 1) evaluate your code on a single process with no limit on "
+                    "child tasks, 2) if in Jupyter notebook define all necessary classes in a separate file and include the "
+                    "classes via import statements, or 3) move your class definitions outside the `__name__=='__main__'` check."
+                ),None
+            else:
+                ex,tb = e,format_tb(e.__traceback__)
+        except KeyboardInterrupt as e:
+            ex,tb = e,None
+        else:
+            ex,tb = None,None
 
-    @property
-    def params(self) -> Mapping[str,Any]: # pragma: no cover
-        """Parameters describing the learner (used for descriptive purposes only).
+        self._send.send((ex, tb, hasattr(self._line[0],'_poisoned') and self._line[0]._poisoned))
 
-        Remarks:
-            These will become columns in the learners table of experiment results.
-        """
-        return {}
+    def join(self) -> None:
+        super().join()
+        self._get_result()
 
-    @abstractmethod
-    def predict(self, context: Context, actions: Sequence[Action]) -> Prediction:
-        """Predict which action to take in the context.
+    @property
+    def pipeline(self) -> Line:
+        return self._line
 
-        Args:
-            context: The current context. It will either be None (multi-armed bandit),
-                a value (a single feature) a hashable tuple (dense context), or a
-                hashable dictionary (sparse context).
-            actions: The current set of actions to choose from in the given context.
-                Each action will either be a value (a single feature), a hashable tuple
-                (dense context), or a hashable dictionary (sparse context)..
+    @property
+    def traceback(self) -> Sequence[str]:
+        return self._traceback
 
-        Returns:
-            A Prediction. Several prediction formats are supported. See the type-hint for these.
-        """
-        ...
+    @property
+    def exception(self) -> Optional[Exception]:
+        return self._exception
 
-    @abstractmethod
-    def learn(self,
-        context: Context,
-        actions: Actions,
-        action: Action,
-        feedback: Union[float,Any],
-        score: float,
-        **kwargs) -> None:
-        """Learn about the action taken in the context.
+    @property
+    def poisoned(self) -> bool:
+        return self._poisoned
 
-        Args:
-            context: The context in which the action was taken.
-            actions: The set of actions chosen from.
-            action: Either the action that was chosen or the index of the action that was chosen.
-            feedback: This will be reward for contextual bandit problems and feedback for IGL problems.
-            score: This will be the probability for the action taken if a PMF/PDF is returned by predict.
-                 It will be the score if an action-score pair is returned by predict. And it will be the
-                 probability if off-policy learning is being performed on LoggedInteractions.
-            **kwargs: Optional information returned with the prediction.
-        """
-        ...
+    def _get_result(self):
+        with self._lock:
+            if not self._recv.closed:
+                if self._recv.poll():
+                    ex,tb,po = self._recv.recv()
+                    self._exception = ex
+                    self._traceback = tb
+                    self._poisoned  = po
+                self._send.close()
+                self._recv.close()
+
+class ThreadLine(mt.Thread):
+
+    def __init__(self, line: Line, callback: Callable = None) -> None:
+        self._line      = line
+        self._callback  = callback
+        self._exception = None
+        self._traceback = None
+        self._poisoned  = False
+        super().__init__(daemon=True)
+
+    def start(self) -> None:
+
+        super().start()
+
+        if self._callback:
+            #we start a thread and join so that the callback
+            #is not called until the thread is no longer alive
+            def join_and_call():
+                self.join()
+                self._callback(self)
+            mt.Thread(target=join_and_call,daemon=True).start()
 
-class SafeLearner(Learner):
-    """A wrapper for learner-likes that guarantees interface consistency."""
+    def run(self) -> None:
+        try:
+            self._line.run()
+        except Exception as e:
+            self._exception = e
+            self._traceback = format_tb(e.__traceback__)
+        self._poisoned  = hasattr(self._line[0],'_poisoned') and self._line[0]._poisoned
 
-    def __init__(self, learner: Learner, seed:int=1) -> None:
-        """Instantiate a SafeLearner.
+    @property
+    def pipeline(self) -> Line:
+        return self._line
 
-        Args:
-            learner: The learner we wish to make sure has the expected interface
-        """
+    @property
+    def traceback(self) -> Sequence[str]:
+        return self._traceback
 
-        self._learner     = learner if not isinstance(learner, SafeLearner) else learner._learner
-        self._rng         = CobaRandom(seed)
-        self._batched     = None
-        self._batched_lrn = None
-        self._batched_mjr = None
-        self._pred_type   = None #1==PDF,2==PMF,3==Action/Score
-        self._with_info   = None
-        self._learn_type  = None #3==current,2==old with info,1==old without info
+    @property
+    def exception(self) -> Optional[Exception]:
+        return self._exception
 
     @property
-    def full_name(self) -> str:
-        """A user-friendly name created from a learner's params for reporting purposes."""
+    def poisoned(self) -> bool:
+        return self._poisoned
 
-        params = dict(self.params)
-        family = params.pop("family")
+class AsyncableLine(SourceSink):
 
-        if len(params) > 0:
-            return f"{family}({','.join(f'{k}={v}' for k,v in params.items())})"
+    def run_async(self, 
+        callback:Callable[['AsyncableLine',Optional[Exception],Optional[str]],None]=None,
+        mode:Literal['process','thread']='process') -> Union[ThreadLine,ProcessLine]:
+        """Run the pipeline asynchronously."""
+
+        mode = mode.lower()
+
+        if mode == "process":
+            worker = ProcessLine(line=self, callback=callback)
+        elif mode == "thread":
+            worker = ThreadLine(line=self, callback=callback)
         else:
-            return family
+            raise CobaException(f"Unrecognized pipe async mode {mode}. Valid values are 'process' and 'thread'.")
 
-    @property
-    def params(self) -> Mapping[str, Any]:
-        try:
-            params = self._learner.params
-            params = params if isinstance(params,dict) else params()
-        except AttributeError:
-            params = {}
+        worker.start()
+        return worker
 
-        if "family" not in params:
-            params["family"] = self._learner.__class__.__name__
+class Unchunker:
+    def __init__(self, chunked: bool) -> None:
+        self._chunked = chunked
+    def filter(self, items: Iterable[Any]) -> Iterable[Any]:
+        if not self._chunked: items = [items]
+        for item in items: yield from item
 
-        return params
+class Pickler:
 
-    def predict(self, context: Context, actions: Actions) -> Tuple[Action,Score,kwargs]:
+    def filter(self, items) -> Iterable[bytes]:
+        try:
+            yield from map(pickle.dumps,items)
+        except Exception as e:
+            if "pickle" in str(e) or "Pickling" in str(e):
+                message = (
+                    f"We attempted to process your code on multiple processes but were unable to do so due to a pickle "
+                    f"error. The exact error received was '{str(e)}'. Errors this kind can often be fixed in one of two "
+                    f"ways: 1) evaluate the experiment in question on a single process with no limit on the tasks per child "
+                    f"or 2) modify the named class to be picklable. The easiest way to make a given class picklable is to "
+                    f"add `def __reduce__(self): return (<the class in question>, (<tuple of constructor arguments>))` to "
+                    f"the class. For more information see https://docs.python.org/3/library/pickle.html#object.__reduce__."
+                )
+                raise CobaException(message)
+            else: #pragma: no cover
+                raise
+
+class Unpickler:
+    def filter(self, items):
+        yield from map(pickle.loads,items)
+
+class EventSetter:
+    def __init__(self, event: mt.Event) -> None:
+        self._event = event
+    def filter(self, items):
+        self._event.set()
+        return items
+
+class Stopper:
+    def __init__(self) -> None:
+        self._stop = False
+
+    def stop(self) -> None:
+        self._stop = True
+
+    def filter(self, items):
+        for item in items:
+            if self._stop: break
+            yield item
+
+class Multiprocessor(Filter[Iterable[Any], Iterable[Any]]):
+    """Create multiple processes to filter given items."""
+
+    def __init__(self,
+            filter: Filter[Iterable[Any], Iterable[Any]],
+            n_processes: int = 1,
+            maxtasksperchild: int = 0,
+            chunked: bool = False,) -> None:
+        """Instantiate a Multiprocessor.
 
-        pred      = self._safe_predict(context,actions)
-        pred_type = self._pred_type
-        batched   = self._batched
+        Args:
+            filter: The inner pipe that will be executed on multiple processes.
+            n_processes: The number of processes that should be created to filter items.
+            maxtasksperchild: The number of items/chunks a process should filter before restarting.
+            chunked: Indicates that the given items have been chunked.
+        """
+        self._filter           = filter
+        self._chunked          = chunked
+        self._max_processes    = n_processes
+        self._maxtasksperchild = maxtasksperchild or None
 
-        if pred_type is None and not batched: # first call only
-            self._determine_pred_format(pred,actions)
-            pred_type = self._pred_type
+    @property
+    def params(self) -> Mapping[str,Any]:
+        return self._filter.params
 
-        elif pred_type is None and batched:
-            if self._batched_mjr:
-                test_pred = pred[0] 
-            else:
-                test_pred = [p[0] if not isinstance(p,dict) else {k:v[0] for k,v in p.items()} for p in pred]
-            self._determine_pred_format(test_pred,actions[0])
-            pred_type = self._pred_type
-
-        if not self._with_info:
-            pred_info = {}
-        elif self._info_dict:
-            pred_info = {k:[p[-1][k] for p in pred] for k in pred[0][-1]} if self._batched_mjr else pred[-1]
-        else:
-            pred_info = {'_': [p[-1] for p in pred]} if batched else {'_': pred[-1]}
+    def filter(self, items: Iterable[Any]) -> Iterable[Any]:
 
-        if self._pred_type == 2:
-            if not batched:
-                pmf = pred[0] if pred_info else pred
-                action,score = self._get_pmf_action_score(self._rng,pmf,actions)
-            else:
-                pmf = [p[0] if pred_info else p for p in pred] if self._batched_mjr else pred[0]
-                action,score = list(zip(*map(self._get_pmf_action_score, repeat(self._rng), pmf, actions)))
-        else:
-            action,score = list(zip(*[p[:2] for p in pred])) if self._batched_mjr else pred[:2]
+        items = peek_first(items)[1]
+        if not items: return []
 
-        if batched:
-            return Batch(action), Batch(score), pred_info
+        if self._max_processes == 1 and self._maxtasksperchild is None:
+            yield from self._filter.filter(Unchunker(self._chunked).filter(items))
         else:
-            return action, score, pred_info
+            event = spawn_context.Event()
 
-    def learn(self, context, actions, action, reward, probability, **kwargs) -> None:
+            #for some reason if this mp queue get too big we can't keyboradinterrupt
+            #therefore, we slightly limit its size and then empty it before closing.
+            in_queue  = spawn_context.Queue(maxsize=self._max_processes*2)
+            out_queue = spawn_context.Queue()
+            in_put    = QueueSink(in_queue,foreach=True)
+            in_get    = QueueSource(in_queue)
+            out_put   = QueueSink(out_queue,foreach=True)
+            out_get   = QueueSource(out_queue)
+            pickler   = Pickler()
+            unpickler = Unpickler() 
+            get_max   = Slice(None,self._maxtasksperchild)
+            unchunk   = Unchunker(self._chunked)
+            setter    = EventSetter(event)
+
+            self._n_procs      = self._max_processes
+            self._exceptions   = []
+            self._poison       = None
+            self._main_err     = False
+            self._load_stopper = Stopper() #this works because the loader is a thread which means we have shared memory
+
+            load_line   = SourceSink(IterableSource(items), self._load_stopper, pickler, in_put)
+            filter_line = SourceSink(in_get, setter, unpickler, get_max, unchunk, self._filter, out_put)
+
+            def loader_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
+                if worker.exception: self._exceptions.append(worker.exception)
+                in_put.write(self._load_stopper.filter([self._poison]*self._n_procs))
+
+            def filter_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
+                if worker.exception: self._exceptions.append(worker.exception)
+
+                assert not worker.is_alive()
+
+                #only known cause of exitcode != 0 is a missing `if __name__ == '__main__'``.
+                if worker.exitcode != 0: #pragma: no cover
+                    #exitcode -15 is keyboard interrupt...
+                    if worker.exitcode != -15:
+                        print(worker.exitcode)
+                    self._main_err = True
+                    event.set()
+
+                #we have to stop on exception because depending on where the exception occurred
+                #we may not have actually read anything from the input queue. If we didn't then
+                #the input queue will never empty and we'll be stuck starting processes forever.
+                if not worker.poisoned and not self._exceptions and worker.exitcode == 0:
+                    ProcessLine(worker.pipeline,callback=filter_finished_or_failed).start()
+                else:
+                    self._n_procs -= 1
+                    if self._n_procs == 0:
+                        try:
+                            out_put.write([self._poison])
+                        except ValueError: #pragma: no cover
+                            pass
 
-        if self._batched is None:
-            self._batched = isinstance(context,Batch)
+            load_thread = ThreadLine(load_line, callback=loader_finished_or_failed)
+            filt_procs  = [ProcessLine(filter_line, callback=filter_finished_or_failed) for _ in range(self._n_procs)]
 
-        if self._batched and self._batched_lrn == False:
-            for i in range(len(context)):
-                self._safe_learn(context[i],actions[i],action[i],reward[i],probability[i], {k:v[i] for k,v in kwargs.items()})
-        else:
             try:
-                self._safe_learn(context,actions,action,reward,probability,kwargs)
-            except:
-                all_failed = False
+                load_thread.start()
+                filt_procs.pop().start()
+
+                #by waiting we can avoid throwing multiple exceptions
+                #when there is a problem with starting a new process
+                event.wait()
+                if not self._main_err:
+                    for p in filt_procs: p.start()
+                    yield from out_get.read()
+
+            finally:
+
+                #stop loading into the input queue
+                self._load_stopper.stop()
+
+                #empty the input queue and then close it
+                #if we don't empty first then we can easily
+                #lock during a keyboard interrupt
                 try:
-                    for i in range(len(context)):
-                        self._safe_learn(context[i],actions[i],action[i],reward[i],probability[i], {k:v[i] for k,v in kwargs.items()})
-                    self._batched_lrn = False
-                except:
-                    all_failed = True
-                if all_failed: raise
-
-    def _determine_pred_type(self,pred,is_discrete) -> Optional[int]:
-        if self._is_type_1(pred): raise CobaException("PDF predictions are currently not supported.")
-        if self._is_type_2(pred,is_discrete): return 2
-        if self._is_type_3(pred,is_discrete): return 3
-        return None
-
-    def _determine_has_info(self,pred,pred_type) -> Mapping[Any,Any]:
-        if pred_type == 2:
-            return not isinstance(pred[0],(int,float))
-        else: #pred_type==3
-            return len(pred) == 3
-
-    def _determine_pred_format(self, pred, actions):
-
-        is_discrete = 0 < len(actions) and len(actions) < float('inf')
-        pred_type = self._determine_pred_type(pred, is_discrete) or self.get_inferred_type(pred, actions)
-        with_info = self._determine_has_info(pred,pred_type)
-
-        self._pred_type = pred_type
-        self._with_info = with_info
-        self._info_dict = with_info and isinstance(pred[-1],dict) 
-
-    def _safe_predict(self, context, actions):
-
-        batched = self._batched
-
-        if batched is None: 
-            batched = isinstance(context,Batch)
-            self._batched = batched
-
-        if not batched:
-            return self._learner.predict(context,actions)
-
-        if batched:
-            batched_lrn = self._batched_lrn
-            if batched_lrn == True:
-                return self._learner.predict(context,actions)
-            elif batched_lrn == False:
-                return list(map(self._learner.predict,context,actions))
-            elif batched_lrn is None:
+                    while True: in_queue.get_nowait()
+                except Empty:
+                    pass
+                    #closing can cause exceptions 
+                    #and doesn't seem to help anything
+                    #in_queue.close()
+
+                #empty the input queue and then close it
+                #if we don't empty first then we can easily
+                #lock during a keyboard interrupt
                 try:
-                    batch_size = len(context)
-                    pred = self._learner.predict(context,actions)
-                    n_rows = len(pred)
-                    n_cols = len(pred[0])
-
-                    self._batched_lrn = True
-
-                    if n_rows != n_cols:
-                        self._batched_mjr = len(pred) == batch_size
-                    else:
-                        #The major order of pred is not determinable. So we
-                        #now do a small "test" to determine the major order.
-                        test_pred = self._learner.predict(Batch([context[0]]),Batch([actions[0]]))
-                        self._batched_mjr = len(test_pred) == 1
-                    return pred
-
-                except Exception as e:
-                    self._batched_lrn = False
-                    self._batched_mjr = True
-                    try:
-                        return list(map(self._learner.predict,context,actions))
-                    except:
-                        pass
-                    raise
-
-    def _safe_learn(self,context,actions,action,reward,probability,kwargs):
-        if self._learn_type==3:
-            self._learner.learn(context, actions, action, reward, probability, **kwargs)
-        elif self._learn_type==2:
-            self._learner.learn(context, action, reward, probability, kwargs.get('_',kwargs))
-        elif self._learn_type==1:
-            self._learner.learn(context, action, reward, probability)
-        else:
-            all_failed = False
-            try:
-                self._learner.learn(context, actions, action, reward, probability, **kwargs)
-                self._learn_type = 3
-            except:
-                try:
-                    self._learner.learn(context, action, reward, probability, kwargs.get('_',kwargs))
-                    self._learn_type = 2
-                except:
-                    try:
-                        self._learner.learn(context, action, reward, probability)
-                        self._learn_type = 1
-                    except:
-                        all_failed = True
-
-                if all_failed: raise
-
-    def _is_type_1(self, pred):
-        #PDF
-        return callable(pred) or callable(pred[0])
-
-    def _is_type_2(self, pred, is_discrete:bool):
-        #PMF
-
-        explicit = isinstance(pred,PMF) or isinstance(pred[0],PMF)
-        pmf_sans_info = is_discrete and isinstance(pred,abc.Sequence) and len(pred) > 3 or len(pred) == 3 and not isinstance(pred[2],dict)
-        pmf_with_info = is_discrete and isinstance(pred,abc.Sequence) and len(pred) == 2 and isinstance(pred[0],abc.Sequence)
-        
-        return (explicit or pmf_sans_info or pmf_with_info) and not (isinstance(pred,ActionScore) or isinstance(pred[0],ActionScore))
-
-    def _is_type_3(self, pred, is_discrete:bool):
-        #Action Score
-        explicit = isinstance(pred,ActionScore) or isinstance(pred[0],ActionScore)
-        with_info = is_discrete and len(pred) == 3 and not isinstance(pred[2],(float,int))
-        return explicit or with_info or not is_discrete
-
-    def get_inferred_type(self,pred,actions) -> int:
-        possible_types = []
-
-        if self._possible_type_2(pred,actions): possible_types.append(2)
-        if self._possible_type_3(pred,actions): possible_types.append(3)
-
-        if len(possible_types) == 1:
-            return possible_types[0]
-        else:
-            raise CobaException("We were unable to parse the given prediction format." 
-                " This is likely because action features were returned for a discrete"
-                " problem. When the action space is discrete, and you wish to directly"
-                " return the selected action rather than a PMF, please provide the"
-                " action index (i.e., actions.index(action)). Alternatively, this can"
-                " also happen for two action problems. In this case we suggest using"
-                " coba.learners.Probs or coba.learners.ActionScore to provide explicit"
-                " type information (e.g., return coba.learners.Probs([1,0])).")
-
-    def _pred_0_possible_pmf(self,pred,actions):
-        possible_pmf = pred[0] if isinstance(pred[0],abc.Sequence) else pred
-        return isclose(sum(possible_pmf), 1, abs_tol=.001) and len(possible_pmf) == len(actions)
-
-    def _pred_0_possible_action(self,pred,actions):
-        is_discrete = 0 < len(actions) and len(actions) < float('inf')
-        return not is_discrete or pred[0] in list(range(len(actions)))
-
-    def _possible_type_2(self,pred,actions):
-        #PMF
-        return self._pred_0_possible_pmf(pred,actions)
-
-    def _possible_type_3(self,pred,actions):
-        #action,score
-        correct_shape = len(pred) in [2,3]        
-        return self._pred_0_possible_action(pred,actions) and correct_shape
-
-    def _get_pmf_action_score(self,rng,pmf,actions):
-        assert len(pmf) == len(actions), "The learner returned an invalid number of probabilities for the actions"
-        assert isclose(sum(pmf), 1, abs_tol=.001), "The learner returned a pmf which does not sum to one."
-        return rng.choice(list(zip(actions,pmf)), pmf)
-
-    def __str__(self) -> str:
-        return self.full_name
-
-def requires_hashables(cls:Type[Learner]):
-
-    def make_hashable(item):
-        if isinstance(item,Dense): return HashableDense(item)
-        if isinstance(item,Sparse): return HashableSparse(item)
-        return item
-
-    old_predict = cls.predict
-    old_learn   = cls.learn
-
-    def new_predict(self,c,A):
-        return old_predict(self,make_hashable(c),list(map(make_hashable,A)))
-
-    def new_learn(self,c,A,a,r,p,**kwargs):
-        old_learn(self,make_hashable(c),list(map(make_hashable,A)), make_hashable(a),r,p,**kwargs)
-
-    cls.predict = new_predict
-    cls.learn   = new_learn
+                    while True: out_queue.get_nowait()
+                except Empty:
+                    pass
+                    #closing can cause exceptions
+                    #and doesn't seem to help anything
+                    #out_queue.close()
 
-    return cls
+            if self._exceptions:
+                raise self._exceptions[0]
```

### Comparing `coba-6.4.2/coba/learners/vowpal.py` & `coba-6.5.0/coba/learners/vowpal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from itertools import repeat, compress
 from sys import platform
 from typing import Any, Dict, Union, Sequence, Mapping, Optional, Tuple
 
 from coba.backports import Literal
 from coba.exceptions import CobaException
-from coba.learners.primitives import Learner, PMF
+from coba.learners.primitives import Learner, PMF, Prob
 from coba.primitives import Sparse, Context, Action, Actions
 from coba.utilities import PackageChecker
 
 Feature       = Union[str,int,float]
 Features      = Union[Feature, Sequence[Feature], Dict[str,Union[int,float]]]
 Namespaces    = Dict[str,Features]
 VW_Features   = Sequence[Union[str,int,Tuple[Union[str,int],Union[int,float]],Dict[str,Union[int,float]]]]
@@ -20,14 +20,15 @@
 class VowpalMediator:
     """A class to handle all communication between Coba and VW."""
 
     def __init__(self) -> None:
         self._vw = None
         self._namespace_keys = []
         self._namespace_keys_index: Dict[str,int] = {}
+        self._args = ""
  
         PackageChecker.vowpalwabbit('VowpalMediator.__init__')
 
     @property
     def is_initialized(self) -> bool:
         """Indicate whether init_learner has been called previously."""
         return self._vw is not None
@@ -60,29 +61,30 @@
         if self._vw is not None:
             raise CobaException("We cannot initilaize a VW learner twice in a single mediator.")
 
         self._version = [ int(v) for v in __version__.split(".") ]
         self._vw = pyvw.Workspace(args) if self._version[0] >= 9 else pyvw.vw(args)
         self._label_type = pyvw.LabelType(label_type) if self._version[0] >= 9 else label_type
         self._example_init = pyvw.Example if self._version[0] >= 9 else pyvw.example
+        self._args = args
 
         return self
 
     def predict(self, example: Any) -> Any:
         """Predict for an example created by the mediator."""
         pred = self._vw.predict(example)
         self._vw.finish_example(example)
         return pred
 
     def learn(self, example: Any) -> None:
         """Learn for an example created by the mediator."""
         self._vw.learn(example)
         self._vw.finish_example(example)
 
-    def make_example(self, namespaces: Namespaces, label:Optional[str]) -> Any:
+    def make_example(self, namespaces: Namespaces, label:Optional[str] = None) -> Any:
         """Create a VW example.
 
         Args:
             ns: The features grouped by namespace in this example.
             label: An optional label (required if this example will be used for learning).
         """
         ns = dict(self._prep_namespaces(namespaces))
@@ -99,15 +101,15 @@
             self._vw.finish()
     
     # override to transform example before they get pushed down to VW
     # i.e. change namespaces from the default 'x' in shared to any other namespace
     def transform_example(self, vw_shared, vw_uniques, labels):
         pass
 
-    def make_examples(self, shared: Namespaces, uniques: Sequence[Namespaces], labels:Optional[Sequence[str]]) -> Sequence[Any]:
+    def make_examples(self, shared: Namespaces, uniques: Sequence[Namespaces], labels:Optional[Sequence[str]] = None) -> Sequence[Any]:
         """Create a list of VW examples.
 
         Args:
             shared: The features grouped by namespace in this example.
             separates: The features, grouped by namespace, unique to each each example. 
             label: An optional label (required if this example will be used for learning).
         """
@@ -190,14 +192,17 @@
             keys  = list(map(str,range(index,index+length)))
 
             self._namespace_keys_index[namespace] = index
             self._namespace_keys += keys
 
         return keys
 
+    def __str__(self) -> str:
+        return self._args
+
 class VowpalLearner(Learner):
     """A friendly wrapper around Vowpal Wabbit's python interface to support CB learning.
 
     Remarks:
         This learner requires that the Vowpal Wabbit package be installed. This package can be
         installed via `pip install vowpalwabbit`. To learn more about solving contextual bandit
         problems with Vowpal Wabbit see `here`__ and `here`__.
@@ -273,14 +278,18 @@
 
         self._vw = vw or VowpalMediator()
 
     @property
     def params(self) -> Mapping[str, Any]:
         return {"family": "vw", 'args': self._args.replace("--quiet","").strip()}
 
+    def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
+        probs = self.predict(context,actions)
+        return probs if actions == request else list(map(probs.__getitem__,map(actions.index,request)))
+
     def predict(self, context: Context, actions: Sequence[Action]) -> PMF:
 
         if not self._vw.is_initialized and self._adf:
             self._vw.init_learner(self._args, 4)
 
         if not self._vw.is_initialized and not self._adf and self._n_actions:
             self._vw.init_learner(self._args, 4)
@@ -345,15 +354,17 @@
 
         if self._adf:
             self._vw.learn(self._vw.make_examples(context, adfs, labels))
         else:
             self._vw.learn(self._vw.make_example(context, label))
 
     def _labels(self,actions,index,reward:float,prob:float) -> Sequence[Optional[str]]:
-        return [ f"{i+1}:{round(-reward,5)}:{round(prob,5)}" if i == index else None for i in range(len(actions))]
+        labels = [None]*len(actions)
+        labels[index] = f"{index+1}:{round(-reward,5)}:{round(prob,5)}"
+        return labels
 
     def _finish(self):
         try:
             self._vw.finish()
         except AttributeError:
             #we do these checks because when mocking up for unittests
             #it is possible that _vw actually isn't ever initialized
```

### Comparing `coba-6.4.2/coba/multiprocessing.py` & `coba-6.5.0/coba/multiprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 read_stdlog   = QueueSource(stdlog)
                 write_stdlog  = QueueSink(stdlog)
 
                 stdlog_writer = Pipes.join(read_stdlog,Foreach(CobaContext.logger.sink)).run_async(mode="thread")
 
                 logger = CobaContext.logger
                 cacher = ConcurrentCacher(CobaContext.cacher,array,lock)
-                store  = { "openml_semaphore": mp.Semaphore(3), **CobaContext.store }
+                store  = { "openml_semaphore": spawn_context.Semaphore(3), **CobaContext.store }
 
                 filter = CobaMultiprocessor.ProcessFilter(self._filter, logger, cacher, store, write_stdlog)
 
             try:
                 yield from Multiprocessor(filter, self._processes, self._maxtasksperchild, self._chunked).filter(items)
 
             except Exception as e:
```

### Comparing `coba-6.4.2/coba/pipes/__init__.py` & `coba-6.5.0/coba/pipes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     "Shuffle",
     "NullSink",
     "ConsoleSink",
     "DiskSink",
     "ListSink",
     "QueueSink",
     "LambdaSink",
-    "QueueIO",
     "SourceFilters",
     "Cache",
     "LazyDense",
     "LazySparse",
     "EncodeDense",
     "LabelDense",
     "KeepDense",
```

### Comparing `coba-6.4.2/coba/pipes/core.py` & `coba-6.5.0/coba/pipes/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 from coba.exceptions import CobaException
 
-from coba.pipes.primitives import Filter, Source, Sink, SourceFilters, FiltersFilter, FiltersSink, SourceSink, Foreach
+from coba.pipes.primitives import Filter, Source, Sink, SourceFilters, FiltersFilter, FiltersSink, Foreach
 from coba.pipes.multiprocessing import AsyncableLine
 
 class Pipes:
 
     @staticmethod
     def join(*pipes: Union[Source, Filter, Sink]) -> Union[Source, Filter, Sink, AsyncableLine]:
         """Join a sequence of pipes into a single pipe.
```

### Comparing `coba-6.4.2/coba/pipes/filters.py` & `coba-6.5.0/coba/pipes/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
         if seed is not None and (not isinstance(seed,int) or seed < 0):
             raise ValueError(f"Invalid parameter for Shuffle: {seed}. An optional integer value >= 0 was expected.")
 
         self._seed = seed
 
     def filter(self, items: Iterable[Any]) -> Sequence[Any]:
-        yield from CobaRandom(self._seed).shuffle(list(items))
+        items = items.copy() if isinstance(items,list) else list(items)
+        yield from CobaRandom(self._seed).shuffle(items,inplace=True)
 
     @property
     def params(self) -> Mapping[str, Any]:
         return { "shuffle": self._seed }
 
 class Take(Filter[Iterable[Any], Sequence[Any]]):
     """Take a fixed number of items from an iterable."""
@@ -131,33 +132,34 @@
         return { "reservoir_count": self._count, "reservoir_seed": self._seed }
 
     def filter(self, items: Iterable[Any]) -> Sequence[Any]:
 
         rng = CobaRandom(self._seed)
 
         if self._count == 0:
-            return []
-
-        if self._count is None:
-            return rng.shuffle(items)
-
-        W         = 1
-        items     = iter(items)
-        reservoir = rng.shuffle(list(islice(items,self._count)))
+            yield from []
 
-        try:
-            while True:
-                [r1,r2,r3] = rng.randoms(3)
-                W = W * math.exp(math.log(r1)/ (self._count or 1) )
-                S = math.floor(math.log(r2)/math.log(1-W))
-                reservoir[int(r3*self._count-.001)] = next(islice(items,S,S+1))
-        except StopIteration:
-            pass
+        elif self._count is None:
+            yield from rng.shuffle(items)
+        
+        else:
+            W         = 1
+            items     = iter(items)
+            reservoir = rng.shuffle(list(islice(items,self._count)))
+
+            try:
+                while True:
+                    [r1,r2,r3] = rng.randoms(3)
+                    W = W * math.exp(math.log(r1)/ (self._count or 1) )
+                    S = math.floor(math.log(r2)/math.log(1-W))
+                    reservoir[int(r3*self._count-.001)] = next(islice(items,S,S+1))
+            except StopIteration:
+                pass
 
-        return reservoir
+            yield from reservoir
 
 class JsonEncode(Filter[Any, str]):
     """A filter which turn a Python object into JSON strings."""
 
     def _min(self, obj):
         #WARNING: This method doesn't handle primitive types such int, float, or str. We handle this shortcoming
         #WARNING: by making sure no primitive type is passed to this method in filter. Accepting the shortcoming
@@ -394,17 +396,18 @@
                 for k,v in self._defaults.items():
                     if k not in row: row[k] = v
 
             yield row
 
 class Cache(Filter[Iterable[Any], Iterable[Any]]):
 
-    def __init__(self,n_slice:int=25) -> None:
-        self._cache = None
-        self._n_slice = n_slice
+    def __init__(self,n_slice:int=25,protected:bool=False) -> None:
+        self._cache     = None
+        self._n_slice   = n_slice
+        self._protected = protected
 
     def filter(self, items: Iterable[Any]) -> Iterable[Any]:
         n_slice = self._n_slice
 
         if self._cache:
             yield from self._cache
```

### Comparing `coba-6.4.2/coba/pipes/primitives.py` & `coba-6.5.0/coba/pipes/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/pipes/readers.py` & `coba-6.5.0/coba/pipes/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import csv
 
 from operator import methodcaller
 from collections import deque
 from itertools import islice, chain, count, takewhile
 from typing import Iterable, Sequence, Union, Any, Pattern, Tuple, Mapping
-from typing import MutableSequence, MutableMapping, Callable, Iterator
+from typing import MutableSequence, MutableMapping, Callable
 
 from coba.exceptions import CobaException
 from coba.encodings import Encoder, CategoricalEncoder
 from coba.utilities import peek_first
 from coba.primitives.rows import Dense, Sparse
 
 from coba.pipes.rows import HeadRows, LazyDense, LazySparse
@@ -149,15 +149,15 @@
 
         for line in lines:
             if line[0] == "%": continue
             missing = " ?," in line or line[-3:] == " ?}"
             yield line,missing
 
 class ArffLineReader(Filter[str, Sequence[str]]):
-    def __init__(self, is_dense:bool, n_columns:int, ):
+    def __init__(self, is_dense:bool, n_columns:int):
         self._is_dense = is_dense
         self._n_columns = n_columns
 
         #only used when parsing dense lines
         self._fallback_delim = None
         self._quotes         = '"'+"'"
         self._dialect        = dict(skipinitialspace=True,escapechar="\\",doublequote=False)
@@ -298,15 +298,15 @@
         line_reader = ArffLineReader(is_dense,len(attrs))
 
         headers,encoders = zip(*attr_reader.filter(attrs))
 
         if is_dense:
             hdr_map = dict(zip(headers, count()))
             for line,missing in data_reader.filter(data):
-                yield LazyDense(lambda line=line:line_reader.filter(line), encoders,hdr_map, missing)
+                yield LazyDense(lambda line=line:line_reader.filter(line),encoders,hdr_map,missing)
 
         else:
             encs = dict(enumerate(encoders))
             fwd  = dict(zip(headers,count()))
             inv  = dict(zip(count(),headers))
             nsp  = set()
             for k,v in encs.items():
```

### Comparing `coba-6.4.2/coba/pipes/rows.py` & `coba-6.5.0/coba/pipes/rows.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     def __getitem__(self, key: int):
         key = key if key.__class__ is int else self.headers[key]
         val = self._load_or_get()[key]
         enc = self._enc
 
         if not enc:
             return val
-
         else:
             try:
                 return enc[key](val)
             except:
                 if val in ['?','']: return None
                 raise
 
@@ -81,22 +80,22 @@
         row = row()
         self._row = row
         return row
 
     def __getitem__(self, key: str):
         key = self._fwd.get(key,key)
         enc = self._enc
-        
+
         try:
             val = self._load_or_get()[key]
         except KeyError:
             if key not in self._nsp: raise
             val = "0"
 
-        if not enc: 
+        if not enc:
             return val
         else:
             try:
                 return enc.get(key,lambda x:x)(val)
             except:
                 if val in ['?','']: return None
                 raise
@@ -489,68 +488,64 @@
         if isinstance(first,Dense):
             ind = first.headers[label] if isinstance(label,str) else label
             return map(LabelDense, rows, repeat(ind), repeat(tipe))
         else:
             return map(LabelSparse, rows, repeat(label), repeat(tipe))
 
 class EncodeCatRows(Filter[Iterable[Union[Any,Dense,Sparse]], Iterable[Union[Any,Dense,Sparse]]]):
-    def __init__(self, tipe=Literal["onehot","onehot_tuple","string"], value_rows:bool = False) -> None:
+    def __init__(self, tipe=Literal["onehot","onehot_unflat","string"], value_rows:bool = False) -> None:
         self._tipe = tipe
-        self._value_rows = value_rows
 
     def filter(self, rows: Iterable[Union[Any,Dense,Sparse]]) -> Iterable[Union[Any,Dense,Sparse]]:
-
         if self._tipe is None: return rows
         first, rows = peek_first(rows)
         if not rows: return []
-    
-        if self._value_rows:
-            rows = self._encode_value_generator(rows)
-        elif isinstance(first,Dense):
-            rows = self._encode_dense_generator(rows, first)
-        elif isinstance(first,Sparse):
-            rows = self._encode_sparse_generator(rows, first)
+
+        if isinstance(first,(Dense,Sparse)):
+            rows = self._encode_collection(rows, first)
         else:
-            rows = rows
+            rows = self._encode_values(rows, first)
 
         if self._tipe =='onehot':
             rows = Flatten().filter(rows)
 
         return rows
 
-    def _encode_value_generator(self, rows):
-        first,rows = peek_first(rows)
+    def _encode_values(self, rows, first):
         if not isinstance(first,Categorical):
             yield from rows
-        elif self._tipe == "string":
+        elif self._tipe == 'string':
             yield from map(str,rows)
-        elif "onehot" in self._tipe:
-            for row in rows: yield row.as_onehot
+        else:
+            yield from (r.as_onehot for r in rows)
 
-    def _encode_dense_generator(self, rows, first):
-        is_mutable = isinstance(first, list)
-        cat_cols =  [i for i,v in enumerate(first) if isinstance(v,Categorical) ]
-       
-        if self._tipe == "string":
-            for row in rows:
-                row = row.copy() if is_mutable else list(row)
-                for i in cat_cols: row[i] = str(row[i])
-                yield row
-        elif "onehot" in self._tipe:
-            for row in rows:
-                row = row.copy() if is_mutable else list(row)
-                for i in cat_cols: row[i] = row[i].as_onehot
-                yield row
+    def _encode_collection(self, rows, first):
+
+        if isinstance(first,Sparse):
+            cat_cols = [k for k,v in first.items() if isinstance(v,Categorical) ]
+        else:
+            cat_cols = [i for i,v in enumerate(first) if isinstance(v,Categorical) ]
+
+        copyable = not isinstance(first,tuple)
+        get_string = 'string' == self._tipe
+
+        prev_row   = None
+        prev_yield = None
+
+        for row in rows:
+            if row == prev_row:
+                #this check doesn't cost us much and will greatly
+                #speed up the encoding of repeated categorical actions
+                yield prev_yield
+            else:
+                prev_row = row
+                row = row.copy() if copyable else list(row)
+
+                if get_string:
+                    for k in cat_cols:
+                        row[k] = str(row[k])
+                else:
+                    for k in cat_cols:
+                        row[k] = row[k].as_onehot
 
-    def _encode_sparse_generator(self, rows, first):
-        cat_cols = [k for k,v in first.items() if isinstance(v,Categorical) ]
-        
-        if self._tipe == "string":
-            for row in rows:
-                row = row.copy()
-                for k in cat_cols: row[k] = str(row[k])
-                yield row
-        elif "onehot" in self._tipe:
-            for row in rows:
-                row = row.copy()
-                for k in cat_cols: row[k] = row[k].as_onehot
                 yield row
+                prev_yield = row
```

### Comparing `coba-6.4.2/coba/pipes/sinks.py` & `coba-6.5.0/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/pipes/sources.py` & `coba-6.5.0/coba/pipes/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,30 +55,30 @@
         self._mode     = mode
 
     def __enter__(self) -> 'DiskSource':
         self._count += 1
 
         if self._file is None:
             if ".gz" in self._filename:
-                self._file = gzip.open(self._filename, f"{self._mode}b", compresslevel=6)
+                self._file = gzip.open(self._filename, f"{self._mode}t")
             else:
-                self._file = open(self._filename, f"{self._mode}b")
+                self._file = open(self._filename, self._mode)
 
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self._count -= 1
         if self._count == 0 and self._file is not None:
             self._file.close()
             self._file = None
 
     def read(self) -> Iterable[str]:
         with self:
             for line in self._file:
-                yield line.decode('utf-8').rstrip('\r\n')
+                yield line.rstrip('\r\n')
 
 class QueueSource(Source[Iterable[Any]]):
     """A source which reads from a queue."""
 
     def __init__(self, queue:Queue, block:bool=True, poison:Any=None) -> None:
         """Instantiate a QueueSource.
```

### Comparing `coba-6.4.2/coba/primitives/__init__.py` & `coba-6.5.0/coba/primitives/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from coba.primitives.semantic import Context, Action, Actions, AIndex, Batch
 from coba.primitives.types import Categorical
 from coba.primitives.rows import Dense, Sparse, HashableDense, HashableSparse
 from coba.primitives.feedbacks import Feedback, SequenceFeedback, BatchFeedback
-from coba.primitives.rewards import Reward, L1Reward, HammingReward, BinaryReward, ScaleReward, SequenceReward, MulticlassReward, BatchReward, IPSReward
+from coba.primitives.rewards import Reward, L1Reward, HammingReward, BinaryReward, ScaleReward, IPSReward
+from coba.primitives.rewards import SequenceReward, MappingReward, MulticlassReward, BatchReward
 
 __all__ = [
     'Reward',
     'L1Reward',
     'HammingReward',
     'BinaryReward',
     'ScaleReward',
     'IPSReward',
     'SequenceReward',
+    'MappingReward',
     'MulticlassReward',
     'Feedback',
     'SequenceFeedback',
     'Dense',
     'Sparse',
     'HashableDense',
     'HashableSparse',
     'Categorical',
     'Context',
     'Action',
     'Actions',
-    'AIndex',
     'Batch',
     'BatchReward',
     'BatchFeedback',
 ]
```

### Comparing `coba-6.4.2/coba/primitives/rewards.py` & `coba-6.5.0/coba/primitives/rewards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,214 @@
-from operator import eq
 from abc import ABC, abstractmethod
-from collections import abc
-from itertools import repeat
-from typing import Union, Sequence, Iterator, Optional, Any
+from typing import Sequence, Optional, Mapping, Any
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
-from coba.primitives.semantic import Action, AIndex, Batch
+from coba.primitives.semantic import Action, Batch
 
 class Reward(ABC):
     __slots__ = ()
-    
+
     @abstractmethod
-    def eval(self, arg: Union[Action,AIndex]) -> float:
+    def eval(self, action: Action) -> float:
         ...
 
     @abstractmethod
-    def argmax(self) -> Union[Action,AIndex]:
+    def argmax(self) -> Action:
         ...
-    
+
+    @abstractmethod
     def max(self) -> float:
-        return self.eval(self.argmax())
+        ...
 
 class IPSReward(Reward):
     __slots__ = ('_reward','_action')
 
-    def __init__(self, reward: float, action: Union[Action,AIndex], probability: Optional[float]) -> None:
+    def __init__(self, reward: float, action: Action, probability: Optional[float]) -> None:
         self._reward = reward/(probability or 1)
         self._action = action
 
-    def eval(self, arg: Union[Action,AIndex]) -> float:
-        return (arg == self._action)*self._reward
+    def eval(self, arg: Action) -> float:
+        return self._reward if arg == self._action else 0
 
-    def argmax(self) -> Union[Action,AIndex]:
+    def argmax(self) -> Action:
         return self._action
     
     def max(self) -> float:
-        return self.eval(self.argmax())
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,IPSReward) and o._reward == self._reward and o._action == self._action
+        return self._reward 
 
     def __reduce__(self):
         #this makes the pickle smaller
         return IPSReward, (self._reward, self._action, 1)
+    
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o,IPSReward) and o._reward == self._reward and o._action == self._action
 
 class L1Reward(Reward):
     __slots__ = ('_label',)
 
-    def __init__(self, label: float) -> None:
-        self._label = label
+    def __init__(self, action: float) -> None:
+        self._label = action
+
+    def eval(self, action: float) -> float: #pragma: no cover
+        return action-self._label if self._label > action else self._label-action 
 
     def argmax(self) -> float:
         return self._label
 
-    def eval(self, arg: float) -> float: #pragma: no cover
-        return arg-self._label if self._label > arg else self._label-arg 
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,L1Reward) and o._label == self._label
+    def max(self) -> float:
+        return 0
 
     def __reduce__(self):
         #this makes the pickle smaller
         return L1Reward, (self._label,)
 
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o,L1Reward) and o._label == self._label
+
 class HammingReward(Reward):
     __slots__ = ('_labels',)
 
-    def __init__(self, labels: Sequence[AIndex]) -> None:
-        self._labels  = set(labels)
+    def __init__(self, labels: Sequence[Action]) -> None:
+        self._labels = set(labels)
 
-    def argmax(self) -> Sequence[AIndex]:
-        return self._labels
+    def eval(self, arg: Sequence[Action]) -> float:
+        return len(self._labels.intersection(arg))/len(self._labels.union(arg))
 
-    def eval(self, arg: Sequence[AIndex]) -> float:
-        return len(self._labels.intersection(arg))/len(self._labels)
+    def argmax(self) -> Sequence[Action]:
+        return self._labels
+    
+    def max(self) -> float:
+        return 1
 
     def __reduce__(self):
         #this makes the pickle smaller
         return HammingReward, (tuple(self._labels),)
 
 class BinaryReward(Reward):
     __slots__ = ('_argmax',)
-    
-    def __init__(self, value: Union[Action,AIndex]):
-        self._argmax = value
 
-    def argmax(self) -> Union[Action,AIndex]:
+    def __init__(self, action: Action):
+        self._argmax = action
+
+    def eval(self, action: Action) -> float:
+        return float(self._argmax==action)
+
+    def argmax(self) -> Action:
         return self._argmax
 
-    def eval(self, arg: Union[Action,AIndex]) -> float:
-        return float(self._argmax==arg)
+    def max(self) -> Action:
+        return 1
 
     def __reduce__(self):
         #this makes the pickle smaller
         return BinaryReward, (self._argmax,)
+    
+    def __eq__(self, o: object) -> bool:
+        return o == self._argmax or (isinstance(o,BinaryReward) and o._argmax == self._argmax)
 
 class ScaleReward(Reward):
+    __slots__ = ('_reward', '_shift', '_scale', '_target')
     def __init__(self, reward: Reward, shift: float, scale: float, target: Literal["argmax","value"]) -> None:
-
-        if target not in ["argmax","value"]:
-            raise CobaException("An unrecognized scaling target was requested for a Reward.")
-
         self._reward = reward
         self._shift  = shift
         self._scale  = scale
-        self._target = target
+        self._target = 'argmax' if target == 0 else 'value' if target ==1 else target
+
+    def eval(self, action: Any) -> float:
+        if self._target == "argmax":
+            return self._reward.eval(action+(1-self._scale)*self._reward.argmax()-self._scale*self._shift)
+        if self._target == "value":
+            return (self._reward.eval(action)+self._shift)*self._scale
 
-        old_argmax = reward.argmax()
-        new_argmax = (old_argmax+shift)*scale if target == "argmax" else old_argmax
+    def argmax(self) -> Action:
+        if self._target == "argmax":
+            return (self._reward.argmax()+self._shift)*self._scale
+        else:
+            return self._reward.argmax()
+    
+    def max(self) -> float:
+        return self.eval(self.argmax())
 
-        self._old_argmax = old_argmax
-        self._new_argmax = new_argmax
+    def __reduce__(self):
+        #this makes the pickle smaller
+        return ScaleReward, (self._reward, self._shift, self._scale, 0 if self._target == "argmax" else 1)
 
-        self._old_eval = reward.eval
+class SequenceReward(Reward):
+    __slots__ = ('_actions','_rewards')
 
-    def argmax(self) -> float:
-        return self._new_argmax
+    def __init__(self, actions: Sequence[Action], rewards: Sequence[float]) -> None:
+        if len(actions) != len(rewards): 
+            raise CobaException("The given actions and rewards did not line up.")
 
-    def eval(self, arg: Any) -> float: #pragma: no cover
-        if self._target == "argmax":
-            return self._old_eval(self._old_argmax + (arg-self._new_argmax))
-        if self._target == "value":
-            return (self._old_eval(arg)+self._shift)*self._scale
+        self._actions = actions
+        self._rewards = rewards
+
+    def eval(self, action: Action) -> float:
+        return self._rewards[self._actions.index(action)]
+
+    def argmax(self) -> Action:
+        return self._actions[self._rewards.index(max(self._rewards))]
+
+    def max(self) -> float:
+        return max(self._rewards)
 
     def __reduce__(self):
         #this makes the pickle smaller
-        return ScaleReward, (self._reward, self._shift, self._scale, self._target)
+        return SequenceReward, (self._actions,self._rewards)
 
-class SequenceReward(Reward):
-    __slots__ = ('_values', )
-    
-    def __init__(self, values: Sequence[float]) -> None:
-        self._values = values
+    def __eq__(self, o: object) -> bool:
+        return o == self._rewards or (isinstance(o,SequenceReward) and o._actions == self._actions and o._rewards == self._rewards)
 
-    def eval(self, arg: AIndex) -> float:
-        return self._values[arg]
+class MappingReward(Reward):
+    __slots__ = ('_mapping','eval')
+
+    def __init__(self, mapping: Mapping[Action,float]) -> None:
+        self._mapping = mapping
+        self.eval     = mapping.__getitem__
 
     def argmax(self) -> Action:
-        max_r = self._values[0]
+        max_r = -float('inf')
         max_a = 0
-        for a,r in enumerate(self._values):
+        for a,r in self._mapping.items():
             if r > max_r:
                 max_a = a
                 max_r = r
         return max_a
 
-    def __getitem__(self, index: int) -> float:
-        return self._values[index]
-
-    def __len__(self) -> int:
-        return len(self._values)
-
-    def __iter__(self) -> Iterator[float]:
-        return iter(self._values)
-
-    def __eq__(self, o: object) -> bool:
-        try:
-            return list(o) == list(self)
-        except:
-            return False
+    def max(self) -> float:
+        return max(self._mapping.values())
 
     def __reduce__(self):
         #this makes the pickle smaller
-        return SequenceReward, (tuple(self._values),)
+        return MappingReward, (self._mapping,)
+
+    def __eq__(self, o: object) -> bool:
+        return o == self._mapping or (isinstance(o,MappingReward) and o._mapping == self._mapping)
 
 class MulticlassReward(Reward):
-    __slots__=('_n_labels','_label')
+    __slots__=('_label',)
     
-    def __init__(self, n_labels: int, label: AIndex) -> None:
-        self._n_labels = n_labels
-        self._label    = label
+    def __init__(self, label: Action) -> None:
+        self._label = label
 
-    def eval(self, action: AIndex) -> float:
+    def eval(self, action: Action) -> float:
         return int(self._label == action)
 
     def argmax(self) -> Action:
         return self._label
-
-    def __getitem__(self, index: int) -> float:
-        #we do this strange index lookup to let
-        #the _indexes list handle a bad index value
-        if index < 0: index = self._n_labels+index
-
-        if index < 0 or self._n_labels <= index:
-            raise IndexError()
-
-        return index == self._label
-
-    def __len__(self) -> int:
-        return self._n_labels
-
-    def __iter__(self) -> Iterator[float]:
-        return iter(map(int,map(eq, range(self._n_labels), repeat(self._label))))
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o,abc.Sequence) and list(o) == list(self)
+    
+    def max(self) -> float:
+        return 1
 
     def __reduce__(self):
-        return MulticlassReward, (self._n_labels, self._label)
+        return MulticlassReward, (self._label,)
+    
+    def __eq__(self, o: object) -> bool:
+        return o == self._label or (isinstance(o,MulticlassReward) and o._label == self._label)
 
 class BatchReward(Batch):
     def eval(self, actions: Sequence[Action]) -> Sequence[float]:
         return list(map(lambda r,a: r.eval(a), self, actions))
 
     def argmax(self) -> Sequence[Action]:
         return [r.argmax() for r in self]
```

### Comparing `coba-6.4.2/coba/primitives/rows.py` & `coba-6.5.0/coba/primitives/rows.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/primitives/types.py` & `coba-6.5.0/coba/primitives/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,7 +11,10 @@
         self.as_int = levels.index(value)
         onehot = [0]*len(levels)
         onehot[self.as_int] = 1
         self.as_onehot = tuple(onehot)
 
     def __repr__(self) -> str:
         return f"Categorical('{self}',{self.levels})"
+    
+    def __reduce__(self):
+        return Categorical, (str(self),list(map(str,self.levels)))
```

### Comparing `coba-6.4.2/coba/random.py` & `coba-6.5.0/coba/random.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,37 +79,40 @@
             max: The maximum value for the random numbers.
 
         Returns:
             The generated random number in [`min`,`max`].
         """
         return min+(max-min)*next(self._randu)        
 
-    def shuffle(self, sequence: Sequence[Any]) -> Sequence[Any]:
+    def shuffle(self, sequence: Sequence[Any], inplace: bool = False) -> Sequence[Any]:
         """Shuffle the order of items in a sequence.
 
         Args:
             sequence: The sequence of items that are to be shuffled.
+            inplace: The sequence of items should be shuffled within the given sequence
 
         Returns:
             A new sequence with the order of items shuffled.
 
         Remarks:
             This is the Richard Durstenfeld's method popularized by Donald Knuth in The Art of Computer
             Programming. This algorithm is unbiased (i.e., all possible permutations are equally likely to occur).
         """
 
         n = len(sequence)
         if n < 2: return sequence
-        l = list(sequence)
+
+        l = sequence if inplace else list(sequence)
 
         #i goes from 0 to n-2
         #j is always i <= j < n
         for i,r in islice(enumerate(self._randu),n-1):
             j = i+int(r*(n-i)) 
             l[i], l[j] = l[j], l[i]
+        
         return l
 
     def randint(self, a:int, b:int) -> int:
         """Generate a uniform random integer in [a, b].
 
         Args:
             a: The inclusive lower bound for the random integer.
```

### Comparing `coba-6.4.2/coba/register.py` & `coba-6.5.0/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/registry.py` & `coba-6.5.0/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-6.4.2/coba/statistics.py` & `coba-6.5.0/coba/statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from math import hypot, isnan, erf, sqrt
 from sys import version_info
 from operator import mul, sub
-from itertools import repeat
+from bisect import bisect_left 
+from itertools import repeat, accumulate
 from abc import abstractmethod, ABC
 from typing import Sequence, Tuple, Union, Callable
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.utilities import PackageChecker
@@ -16,27 +17,59 @@
 
     values = sorted(values)
 
     p25,p75 = percentile(values, [0.25,0.75])
 
     return p75-p25
 
-def percentile(values: Sequence[float], percentiles: Union[float,Sequence[float]]) -> Union[float, Tuple[float,...]]:
+def weighted_percentile(values: Sequence[float], weights: Sequence[float], percentiles: Union[float,Sequence[float]], sort: bool = True) -> Union[float, Tuple[float,...]]:
+
+    def _percentile(values: Sequence[float], weights:Sequence[float], percentile: float) -> float:
+        assert 0 <= percentile and percentile <= 1, "Percentile must be between 0 and 1 inclusive."
+
+        if percentile == 0:
+            return values[0]
+        
+        if percentile == 1:
+            return values[-1]
+
+        R = bisect_left(weights,percentile)
+        L = R-1
+        LP = (weights[R]-percentile)/(weights[R]-weights[L])
+
+        return LP*values[L] + (1-LP)*values[R]
+
+    if sort:
+        values, weights = zip(*sorted(zip(values,weights)))
+    
+    weights = (0,)+weights[1:]
+    weight_sum = sum(weights)
+    weights    = [w/weight_sum for w in accumulate(weights) ] 
+
+    if isinstance(percentiles,(float,int)):
+        return _percentile(values, weights, percentiles)
+    else:
+        return tuple([_percentile(values, weights, p) for p in percentiles ])
+
+def percentile(values: Sequence[float], percentiles: Union[float,Sequence[float]], sort: bool = True) -> Union[float, Tuple[float,...]]:
 
     def _percentile(values: Sequence[float], percentile: float) -> float:
         assert 0 <= percentile and percentile <= 1, "Percentile must be between 0 and 1 inclusive."
 
         i = percentile*(len(values)-1)
-
-        if i == int(i):
-            return values[int(i)]
+        I = int(i)
+        
+        if i == I:
+            return values[I]
         else:
-            return values[int(i)] * (1-(i-int(i))) + values[int(i)+1] * (i-int(i))
+            w = (i-I)
+            return (1-w)*values[I] + w*values[I+1]
 
-    values = sorted(values)
+    if sort:
+        values = sorted(values)
 
     if isinstance(percentiles,(float,int)):
         return _percentile(values, percentiles)
     else:
         return tuple([_percentile(values, p) for p in percentiles ])
 
 def phi(x: float) -> float:
@@ -78,15 +111,16 @@
 class StandardErrorOfMean(PointAndInterval):
 
     def __init__(self, z_score:float=1.96) -> None:
         self._z_score = z_score 
 
     def calculate(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
         mu = mean(sample)
-        se = stdev(sample)/(len(sample)**(.5))
+        se = 0 if len(sample) == 1 else stdev(sample)/(len(sample)**(.5))
+        
         return (mu, (self._z_score*se,self._z_score*se))
 
 class BootstrapConfidenceInterval(PointAndInterval):
 
     def __init__(self, confidence:float, statistic:Callable[[Sequence[float]], float]) -> None:
         self._conf = confidence
         self._stat = statistic
```

### Comparing `coba-6.4.2/coba/utilities.py` & `coba-6.5.0/coba/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import warnings
 import importlib
 
-from itertools import chain
+from itertools import chain, islice
 from collections import defaultdict
-from typing import TypeVar, Iterable, Tuple, Sequence
+from typing import TypeVar, Iterable, Tuple, Union, Sequence
 
 from coba.exceptions import CobaExit
 
 def coba_exit(message:str):
     #we ignore warnings before exiting in order to make jupyter's output a little cleaner
     warnings.filterwarnings("ignore",message="To exit: use 'exit', 'quit', or Ctrl-D.")
     raise CobaExit(message) from None
@@ -110,14 +110,15 @@
             raise KeyError( key )
         else:
             value = self.default_factory(key)
             self[key] = value
             return value
 
 _T = TypeVar("_T")
-def peek_first(items: Iterable[_T]) -> Tuple[_T, Iterable[_T]]:
+def peek_first(items: Iterable[_T], n:int=1) -> Tuple[Union[_T,Sequence[_T]], Iterable[_T]]:
     items = iter(items)
-    try:
-        first = next(items)
-        return first, chain([first],items)
-    except StopIteration:
-        return None, []
+    first = list(islice(items,n))
+
+    items = [] if not first else chain(first,items)
+    first = None if not first else first[0] if n==1 else first
+
+    return first, items
```

### Comparing `coba-6.4.2/coba.egg-info/PKG-INFO` & `coba-6.5.0/coba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 6.4.2
+Version: 6.5.0
 Summary: A contextual bandit research package.
 Home-page: https://github.com/VowpalWabbit/coba
 Author: Mark Rucker
 Author-email: rucker.mark@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -97,9 +96,7 @@
  ## Results
 
  The end result of an Experiment is a Result object which has been built for easy analysis. The result class provides a number of plots as well as filtering capabilities out of the box. If the built in functionality isn't advanced enough data from experiments can be accesed directly from a three table structure: a Learner table, Environment table, and Interaction table. These tables can be ported to pandas dataframes where all manner of advanced filtering and plotting can be performed to discover the strengths and weaknesses of Learners on various Environments.
 
  ## Examples
 
  An examples directory is included in the repository with a number of code and experiment demonstrations. These examples show how to create experiments, evaluate learners against them and plot the results.
-
-
```

### Comparing `coba-6.4.2/coba.egg-info/SOURCES.txt` & `coba-6.5.0/coba.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 coba/experiments/results.py
 coba/experiments/tasks.py
 coba/learners/__init__.py
 coba/learners/bandit.py
 coba/learners/corral.py
 coba/learners/linucb.py
 coba/learners/primitives.py
+coba/learners/safety.py
 coba/learners/vowpal.py
 coba/pipes/__init__.py
 coba/pipes/core.py
 coba/pipes/filters.py
 coba/pipes/multiprocessing.py
 coba/pipes/primitives.py
 coba/pipes/readers.py
```

### Comparing `coba-6.4.2/setup.py` & `coba-6.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 MAJOR               = 6
-MINOR               = 4
-MICRO               = 2
+MINOR               = 5
+MICRO               = 0
 VERSION             = f"{MAJOR}.{MINOR}.{MICRO}"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="coba",
```

