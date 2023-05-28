# Comparing `tmp/embedin-0.2.1.tar.gz` & `tmp/embedin-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedin-0.2.1.tar", last modified: Wed May 17 03:02:11 2023, max compression
+gzip compressed data, was "embedin-0.2.2a0.tar", last modified: Sun May 28 02:11:56 2023, max compression
```

## Comparing `embedin-0.2.1.tar` & `embedin-0.2.2a0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.636803 embedin-0.2.1/
--rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.2.1/LICENSE
--rw-r--r--   0 xchen375   (502) staff       (20)     3492 2023-05-17 03:02:11.636191 embedin-0.2.1/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     3055 2023-05-17 03:00:39.000000 embedin-0.2.1/README.md
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.609407 embedin-0.2.1/embedin/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.2.1/embedin/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.611707 embedin-0.2.1/embedin/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     7381 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.613420 embedin-0.2.1/embedin/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)     1931 2023-05-15 01:03:38.000000 embedin-0.2.1/embedin/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      134 2023-05-13 23:39:26.000000 embedin-0.2.1/embedin/embedding/embedding_base.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1647 2023-05-13 23:39:26.000000 embedin-0.2.1/embedin/embedding/openai_embedding.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2043 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/embedding/sentence_transformer.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.616036 embedin-0.2.1/embedin/index/
--rw-r--r--   0 xchen375   (502) staff       (20)      693 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2317 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/flat_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2331 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/hnsw_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1373 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/index/index_base.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.617686 embedin-0.2.1/embedin/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/model/embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.619385 embedin-0.2.1/embedin/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2667 2023-05-15 21:05:11.000000 embedin-0.2.1/embedin/repository/collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     4381 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/repository/embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.620959 embedin-0.2.1/embedin/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/embedin/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2322 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/service/collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     4114 2023-05-17 03:00:39.000000 embedin-0.2.1/embedin/service/embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.621618 embedin-0.2.1/embedin/util/
--rw-r--r--   0 xchen375   (502) staff       (20)     1354 2023-05-13 19:19:06.000000 embedin-0.2.1/embedin/util/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.611293 embedin-0.2.1/embedin.egg-info/
--rw-r--r--   0 xchen375   (502) staff       (20)     3492 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     1463 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/SOURCES.txt
--rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/dependency_links.txt
--rw-r--r--   0 xchen375   (502) staff       (20)      170 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/requires.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-05-17 03:02:11.000000 embedin-0.2.1/embedin.egg-info/top_level.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-05-17 03:02:11.636953 embedin-0.2.1/setup.cfg
--rw-r--r--   0 xchen375   (502) staff       (20)      841 2023-05-17 03:00:33.000000 embedin-0.2.1/setup.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.622345 embedin-0.2.1/tests/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.2.1/tests/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.622841 embedin-0.2.1/tests/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     2951 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.625463 embedin-0.2.1/tests/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)     1282 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      296 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_embedding_base.py
--rw-r--r--   0 xchen375   (502) staff       (20)      818 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_openai_embedding.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1398 2023-05-13 23:39:26.000000 embedin-0.2.1/tests/embedding/test_sentence_transformer_embedding.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.627848 embedin-0.2.1/tests/index/
--rw-r--r--   0 xchen375   (502) staff       (20)     2065 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2593 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/test_flat_index.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2939 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/index/test_hnsw_index.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.630258 embedin-0.2.1/tests/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1938 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/model/test_collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2044 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/model/test_embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.632527 embedin-0.2.1/tests/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2479 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/repository/test_collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     7360 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/repository/test_embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.634407 embedin-0.2.1/tests/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.1/tests/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1333 2023-04-22 22:11:55.000000 embedin-0.2.1/tests/service/test_collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3752 2023-05-17 03:00:39.000000 embedin-0.2.1/tests/service/test_embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-17 03:02:11.635237 embedin-0.2.1/tests/util/
--rw-r--r--   0 xchen375   (502) staff       (20)     1588 2023-05-13 19:19:06.000000 embedin-0.2.1/tests/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.494742 embedin-0.2.2a0/
+-rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.2.2a0/LICENSE
+-rw-r--r--   0 xchen375   (502) staff       (20)     3347 2023-05-28 02:11:56.494369 embedin-0.2.2a0/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     2908 2023-05-21 13:33:44.000000 embedin-0.2.2a0/README.md
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.456565 embedin-0.2.2a0/embedin/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1107 2023-05-18 22:17:52.000000 embedin-0.2.2a0/embedin/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.459368 embedin-0.2.2a0/embedin/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     8261 2023-05-28 01:56:56.000000 embedin-0.2.2a0/embedin/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.462650 embedin-0.2.2a0/embedin/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2594 2023-05-18 23:55:57.000000 embedin-0.2.2a0/embedin/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      798 2023-05-18 23:56:42.000000 embedin-0.2.2a0/embedin/embedding/embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2310 2023-05-18 23:55:56.000000 embedin-0.2.2a0/embedin/embedding/openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2706 2023-05-18 23:55:57.000000 embedin-0.2.2a0/embedin/embedding/sentence_transformer.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.465646 embedin-0.2.2a0/embedin/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1356 2023-05-18 23:55:57.000000 embedin-0.2.2a0/embedin/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2990 2023-05-21 14:58:47.000000 embedin-0.2.2a0/embedin/index/flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2994 2023-05-18 23:55:56.000000 embedin-0.2.2a0/embedin/index/hnsw_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2036 2023-05-18 23:55:57.000000 embedin-0.2.2a0/embedin/index/index_base.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.468308 embedin-0.2.2a0/embedin/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)      952 2023-05-21 02:26:20.000000 embedin-0.2.2a0/embedin/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      978 2023-05-21 02:15:30.000000 embedin-0.2.2a0/embedin/model/collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1313 2023-05-21 01:25:37.000000 embedin-0.2.2a0/embedin/model/embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.471363 embedin-0.2.2a0/embedin/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)      662 2023-05-18 23:55:56.000000 embedin-0.2.2a0/embedin/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3798 2023-05-21 13:33:55.000000 embedin-0.2.2a0/embedin/repository/collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     5534 2023-05-21 13:19:25.000000 embedin-0.2.2a0/embedin/repository/embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.474380 embedin-0.2.2a0/embedin/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)      662 2023-05-18 23:55:56.000000 embedin-0.2.2a0/embedin/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2948 2023-05-21 13:04:47.000000 embedin-0.2.2a0/embedin/service/collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     4978 2023-05-21 13:22:21.000000 embedin-0.2.2a0/embedin/service/embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.475492 embedin-0.2.2a0/embedin/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2017 2023-05-18 23:55:57.000000 embedin-0.2.2a0/embedin/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.458962 embedin-0.2.2a0/embedin.egg-info/
+-rw-r--r--   0 xchen375   (502) staff       (20)     3347 2023-05-28 02:11:56.000000 embedin-0.2.2a0/embedin.egg-info/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     1463 2023-05-28 02:11:56.000000 embedin-0.2.2a0/embedin.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-05-28 02:11:56.000000 embedin-0.2.2a0/embedin.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)      170 2023-05-28 02:11:56.000000 embedin-0.2.2a0/embedin.egg-info/requires.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-05-28 02:11:56.000000 embedin-0.2.2a0/embedin.egg-info/top_level.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-05-28 02:11:56.494844 embedin-0.2.2a0/setup.cfg
+-rw-r--r--   0 xchen375   (502) staff       (20)      847 2023-05-28 01:51:41.000000 embedin-0.2.2a0/setup.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.476328 embedin-0.2.2a0/tests/
+-rw-r--r--   0 xchen375   (502) staff       (20)      662 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.477324 embedin-0.2.2a0/tests/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     3614 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.481242 embedin-0.2.2a0/tests/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1909 2023-05-18 23:56:42.000000 embedin-0.2.2a0/tests/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      959 2023-05-18 23:55:57.000000 embedin-0.2.2a0/tests/embedding/test_embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1481 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/embedding/test_openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2061 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/embedding/test_sentence_transformer_embedding.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.484368 embedin-0.2.2a0/tests/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2679 2023-05-28 01:48:18.000000 embedin-0.2.2a0/tests/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3295 2023-05-28 01:52:42.000000 embedin-0.2.2a0/tests/index/test_flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3591 2023-05-28 01:48:03.000000 embedin-0.2.2a0/tests/index/test_hnsw_index.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.486963 embedin-0.2.2a0/tests/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1737 2023-05-21 13:33:55.000000 embedin-0.2.2a0/tests/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2601 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/model/test_collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2707 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/model/test_embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.489736 embedin-0.2.2a0/tests/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)      662 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     4089 2023-05-21 13:09:59.000000 embedin-0.2.2a0/tests/repository/test_collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     8283 2023-05-21 11:57:47.000000 embedin-0.2.2a0/tests/repository/test_embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.492307 embedin-0.2.2a0/tests/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)      662 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1996 2023-05-18 23:55:57.000000 embedin-0.2.2a0/tests/service/test_collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     4459 2023-05-21 12:57:46.000000 embedin-0.2.2a0/tests/service/test_embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-28 02:11:56.493376 embedin-0.2.2a0/tests/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2251 2023-05-18 23:55:56.000000 embedin-0.2.2a0/tests/util/__init__.py
```

### Comparing `embedin-0.2.1/LICENSE` & `embedin-0.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedin-0.2.1/PKG-INFO` & `embedin-0.2.2a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,100 +12,107 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Embedin - Empower AI with persistent memory
 [![PyPI](https://img.shields.io/pypi/v/embedin?label=embedin)](https://pypi.org/project/embedin/)
 [![Coverage Status](https://coveralls.io/repos/github/EmbedInAI/EmbedInDB/badge.svg)](https://coveralls.io/github/EmbedInAI/EmbedInDB)
 
-## What is Embedin
-Embedin is a highly efficient software library designed to seamlessly convert widely-used databases, such as MySQL, PostgreSQL, and MS SQL Server, into a vector database with minimal effort. Its lightweight design enables quick and easy integration into your existing software stack, allowing you to leverage the benefits of a vector database without the need for extensive modifications to your current system. 
+Embedin is an open-source vector database and efficient library that seamlessly converts popular databases like MySQL, PostgreSQL, and MS SQL Server into vector databases with zero effort.
 
-With fast indexing and retrieval, it's ideal for high-performance applications such as natural language processing, image recognition, and recommendation systems. Embedin's simple API and query language make it easy to use and integrate. 
+Embedin is an ideal solution for AI applications like natural language processing, image recognition, and recommendation systems, offering fast indexing and retrieval. Its simple API and query language ensure ease of use and seamless integration.
+
+## Minimum Requirements
+Python 3.7 or higher.
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory
+### Store embeddings in memory
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
-result = client.query("These are tests", top_k=1)
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+result = client.query("These are tests", top_k=1)  # Query the most similar text from the collection
 print(result)
 ```
 
-### Using Sqlite
+### Store embeddings in SQLite
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using PostgreSQL
+### Store embeddings in PostgreSQL
+
+#### Start PostgreSQL Docker container
+```bash
+cd docker
+docker-compose up embedin-postgres
+```
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MySQL
+### Store embeddings in MySQL
+
+#### Start MySQL Docker container
+```bash
+cd docker
+docker-compose up embedin-mysql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MS-SQL
+### Store embeddings in SQL Server
+
+#### Start SQL Server Docker container
+```bash
+cd docker
+docker-compose up embedin-mssql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
-client = Client(collection_name="test_collection", url=url)
+client = Embedin(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
-## For development
-
-Clone the repo
-```bash
-git clone https://github.com/EmbedInAI/embedin.git
-```
-
-Start PostgreSQL DB (Only necessary for using PostgreSQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-postgres
-```
+## More References
+* [API Reference](./API.md)
 
-Start MySQL DB (Only necessary for using MySQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mysql
-```
 
-Start MS-SQL DB (Only necessary for using MS-SQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mssql
-```
+## Contribute
+Please refer [Contributors Guide](./CONTRIBUTING.md)
 
-Run unit test with coverage report
-```bash
-coverage run -m unittest discover -s tests -p '*.py'
-coverage report
-```
+# TODO
+- unit test fail on faiss index (segmentation fault)
```

### Comparing `embedin-0.2.1/README.md` & `embedin-0.2.2a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,104 @@
 # Embedin - Empower AI with persistent memory
 [![PyPI](https://img.shields.io/pypi/v/embedin?label=embedin)](https://pypi.org/project/embedin/)
 [![Coverage Status](https://coveralls.io/repos/github/EmbedInAI/EmbedInDB/badge.svg)](https://coveralls.io/github/EmbedInAI/EmbedInDB)
 
-## What is Embedin
-Embedin is a highly efficient software library designed to seamlessly convert widely-used databases, such as MySQL, PostgreSQL, and MS SQL Server, into a vector database with minimal effort. Its lightweight design enables quick and easy integration into your existing software stack, allowing you to leverage the benefits of a vector database without the need for extensive modifications to your current system. 
+Embedin is an open-source vector database and efficient library that seamlessly converts popular databases like MySQL, PostgreSQL, and MS SQL Server into vector databases with zero effort.
 
-With fast indexing and retrieval, it's ideal for high-performance applications such as natural language processing, image recognition, and recommendation systems. Embedin's simple API and query language make it easy to use and integrate. 
+Embedin is an ideal solution for AI applications like natural language processing, image recognition, and recommendation systems, offering fast indexing and retrieval. Its simple API and query language ensure ease of use and seamless integration.
+
+## Minimum Requirements
+Python 3.7 or higher.
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory
+### Store embeddings in memory
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
-result = client.query("These are tests", top_k=1)
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+result = client.query("These are tests", top_k=1)  # Query the most similar text from the collection
 print(result)
 ```
 
-### Using Sqlite
+### Store embeddings in SQLite
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using PostgreSQL
+### Store embeddings in PostgreSQL
+
+#### Start PostgreSQL Docker container
+```bash
+cd docker
+docker-compose up embedin-postgres
+```
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MySQL
+### Store embeddings in MySQL
+
+#### Start MySQL Docker container
+```bash
+cd docker
+docker-compose up embedin-mysql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MS-SQL
+### Store embeddings in SQL Server
+
+#### Start SQL Server Docker container
+```bash
+cd docker
+docker-compose up embedin-mssql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
-client = Client(collection_name="test_collection", url=url)
+client = Embedin(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
-## For development
+## More References
+* [API Reference](./API.md)
 
-Clone the repo
-```bash
-git clone https://github.com/EmbedInAI/embedin.git
-```
 
-Start PostgreSQL DB (Only necessary for using PostgreSQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-postgres
-```
+## Contribute
+Please refer [Contributors Guide](./CONTRIBUTING.md)
 
-Start MySQL DB (Only necessary for using MySQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mysql
-```
-
-Start MS-SQL DB (Only necessary for using MS-SQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mssql
-```
-
-Run unit test with coverage report
-```bash
-coverage run -m unittest discover -s tests -p '*.py'
-coverage report
-```
+# TODO
+- unit test fail on faiss index (segmentation fault)
```

### Comparing `embedin-0.2.1/embedin/client/__init__.py` & `embedin-0.2.2a0/embedin/client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             self.embedding_fn = Embedding.create_embedding(embedding_fn)
 
         if url is None:
             engine = create_engine("sqlite:///:memory:", echo=debug)
         else:
             engine = create_engine(url)
 
-        session = sessionmaker(bind=engine)
+        session = sessionmaker(bind=engine, expire_on_commit=False)
         self.session = session()
 
         self.collection_service = CollectionService(self.session)
         self.embedding_service = EmbeddingService(self.session)
 
         embeddings = kwargs.get("embeddings")
         embeddings_meta = kwargs.get("meta")
@@ -89,15 +89,15 @@
         elif texts is not None:
             embeddings = self.embedding_fn(texts)
             inserted_rows = self.embedding_service.add_all(
                 self.collection_id, embeddings, texts, embeddings_meta
             )
 
         self.embedding_rows.extend(inserted_rows)
-        total_embeddings = [row.embedding_data for row in self.embedding_rows]
+        total_embeddings = [row.get("embedding_data") for row in self.embedding_rows]
 
         self.index_hint = index_hint
         self.search_index = None
         if total_embeddings:
             self.search_index = Index(total_embeddings, self.index_hint)
 
     def create_or_get_collection(self, name):
@@ -123,31 +123,30 @@
         Args:
             name (str): Name of the collection.
 
         Returns:
             str: ID of the new collection.
         """
         collection = self.collection_service.create(name)
-        self.collection_id = collection.id
+        self.collection_id = collection.get("id")
         return self.collection_id
 
     def get_collection(self, name):
         """
         Retrieve the ID of an existing collection with the given name.
 
         Args:
             name (str): Name of the collection.
 
         Returns:
             str: ID of the collection, or None if no collection with the given name exists.
         """
         collection = self.collection_service.get_by_name(name)
-        if collection:
-            self.collection_id = collection.id
-            return self.collection_id
+        self.collection_id = collection.get("id")
+        return self.collection_id
 
     def add_data(self, texts, meta_data=None):
         """
         Add new data to the collection.
 
         Args:
             texts (list of str): List of text data to add to the collection.
@@ -160,15 +159,15 @@
         logger.info("Adding embedding to the database")
         inserted_data = self.embedding_service.add_all(
             self.collection_id, embeddings, texts, meta_data
         )
 
         self.embedding_rows.extend(inserted_data)
 
-        inserted_embeddings = [row.embedding_data for row in inserted_data]
+        inserted_embeddings = [row.get("embedding_data") for row in inserted_data]
 
         if self.search_index is None:
             self.search_index = Index(embeddings, self.index_hint)
         else:
             self.search_index.update_index(inserted_embeddings)
 
     def query(self, query_texts, top_k=3):
@@ -185,12 +184,33 @@
                           {'text': str, 'meta_data': object or None}
         """
         if isinstance(query_texts, str):
             query_texts = [query_texts]
         query_embeddings = self.embedding_fn(query_texts)
         indices = self.search_index.search(query_embeddings, top_k)
         matched_embeddings = [
-            {"text": r.text, "meta_data": r.meta_data}
+            {"text": r.get("text"), "meta_data": r.get("meta_data")}
             for i, r in enumerate(self.embedding_rows)
             if i in indices
         ]
         return matched_embeddings
+
+
+if __name__ == "__main__":
+    url = "sqlite:///test.db"
+    texts = [
+        "Which fourteen hundred years ago were nail'd",
+        "Over whose acres walk'd those blessed feet",
+        "Which fourteen hundred years ago were nail'd",
+        "For our advantage on the bitter cross.",
+        "But this our purpose now is twelve month old,",
+        "And bootless 'tis to tell you we will go:",
+        "Therefore we meet not now. Then let me hear",
+        "Of you, my gentle cousin Westmoreland,",
+        "What yesternight our council did decree",
+        "In forwarding this dear expedience.",
+        "My liege, this haste was hot in quest",
+    ]
+    client = Client(collection_name="test_collection", texts=texts, url=url)
+    client.add_data(["That is a good day!"])
+    result = client.query(texts[0:10], top_k=2)
+    print(result)
```

### Comparing `embedin-0.2.1/embedin/embedding/sentence_transformer.py` & `embedin-0.2.2a0/embedin/embedding/sentence_transformer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# -*- coding: utf-8 -*-
+# embedin - A vector database that empowers AI with persistent memory,
+# (C) 2023 EmbedInAI
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from sentence_transformers import SentenceTransformer
 
 from embedin.embedding.embedding_base import EmbeddingBase
 
 
 class SentenceTransformerEmbedding(EmbeddingBase):
     """
```

### Comparing `embedin-0.2.1/embedin/repository/collection_repository.py` & `embedin-0.2.2a0/embedin/service/collection_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,86 @@
-import uuid
+# -*- coding: utf-8 -*-
+# embedin - A vector database that empowers AI with persistent memory,
+# (C) 2023 EmbedInAI
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from embedin.model.collection_model import CollectionModel
+from embedin.repository.collection_repository import CollectionRepository
 
 
-class CollectionRepository:
+class CollectionService:
     """
-    A repository for managing collections in a database.
+    A service class for handling operations related to collections.
 
-    Parameters:
-    -----------
-    session: sqlalchemy.orm.Session
-        The database session to use.
+    Attributes:
+        collection_repo (CollectionRepository): The repository instance for handling database interactions.
 
     Methods:
-    --------
-    create_table():
-        Creates the table in the database for collections.
-
-    get_by_name(name: str) -> CollectionModel or None:
-        Retrieves a collection from the database by name.
-
-    create(name: str, get_if_exist: bool = True) -> CollectionModel:
-        Creates a new collection in the database with the given name.
-        If the collection already exists and get_if_exist is True, it returns the existing collection.
-        If get_if_exist is False, it raises a ValueError.
+        get_by_name(name):
+            Fetches a collection from the database by its name.
+
+            Args:
+                name (str): The name of the collection to retrieve.
+
+            Returns:
+                CollectionModel: A CollectionModel representing the row of the collection fetched from the database.
+
+        create(name, get_if_exist=True):
+            Creates a new collection in the database.
+
+            Args:
+                name (str): The name of the new collection.
+                get_if_exist (bool): If True, return the existing collection if it already exists. If False, create a new collection with the given name.
+
+            Returns:
+                CollectionModel: A CollectionModel representing the newly created collection.
     """
 
     def __init__(self, session):
         """
-        Constructs a new CollectionRepository with the given database session.
-        """
-
-        self.session = session
-        self.create_table()
+        Initializes a new instance of the CollectionService class.
 
-    def create_table(self):
-        """
-        Creates the table in the database for collections.
+        Args:
+            session (Session): A database session object for making database queries.
         """
 
-        CollectionModel.metadata.create_all(self.session.bind)
+        self.collection_repo = CollectionRepository(session)
 
     def get_by_name(self, name):
         """
-        Retrieves a collection from the database by name.
+        Fetches a collection from the database by its name.
 
-        Parameters:
-        -----------
-        name: str
-            The name of the collection to retrieve.
+        Args:
+            name (str): The name of the collection to retrieve.
 
         Returns:
-        --------
-        collection: CollectionModel or None
-            The collection with the given name, or None if it does not exist.
+            collection: dict
+            The collection with the given name
         """
 
-        collection = self.session.query(CollectionModel).filter_by(name=name).first()
-        return collection
+        row = self.collection_repo.get_by_name(name)
+        return row
 
     def create(self, name, get_if_exist=True):
         """
-        Creates a new collection in the database with the given name.
+        Creates a new collection in the database.
 
-        Parameters:
-        -----------
-        name: str
-            The name of the collection to create.
-        get_if_exist: bool, optional (default=True)
-            If the collection already exists and get_if_exist is True, it returns the existing collection.
-            If get_if_exist is False, it raises a ValueError.
+        Args:
+            name (str): The name of the new collection.
+            get_if_exist (bool): If True, return the existing collection if it already exists. If False, create a new collection with the given name.
 
         Returns:
-        --------
-        collection: CollectionModel
-            The newly created collection.
+            CollectionModel: A CollectionModel representing the newly created collection.
         """
 
-        collection = self.get_by_name(name)
-        if collection:
-            if get_if_exist:
-                return collection
-            raise ValueError(f"Collection with name {name} already exists")
-
-        collection_id = str(uuid.uuid4())
-        collection = CollectionModel(id=collection_id, name=name)
-        self.session.add(collection)
-        self.session.commit()
-
+        collection = self.collection_repo.create(name, get_if_exist)
         return collection
```

### Comparing `embedin-0.2.1/embedin/repository/embedding_repository.py` & `embedin-0.2.2a0/embedin/repository/embedding_repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,36 @@
+# -*- coding: utf-8 -*-
+# embedin - A vector database that empowers AI with persistent memory,
+# (C) 2023 EmbedInAI
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import logging
+
 from sqlalchemy.exc import IntegrityError
 from tqdm import tqdm
 
 from embedin.model.embedding_model import EmbeddingModel
 
+# Configure the root logger to output to the console
+logging.basicConfig(
+    format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
+)
+
+logger = logging.getLogger(__name__)
+
 
 class EmbeddingRepository:
     """
     This class provides methods to interact with embeddings stored in the database.
 
     Attributes:
         session (sqlalchemy.orm.Session): The database session to use for querying and modifying data.
@@ -40,15 +64,15 @@
         """
         Adds multiple embeddings to the database using loop, returning the successfully inserted rows.
 
         Args:
             rows (List[EmbeddingModel]): A list of EmbeddingModel objects to add to the database.
 
         Returns:
-            List[EmbeddingModel]: A list of successfully inserted EmbeddingModel objects.
+            List[EmbeddingModel]: A list of successfully inserted EmbeddingModel.
         """
         inserted_rows = []
         for row in rows:
             try:
                 self.session.merge(row)
                 self.session.commit()
                 inserted_rows.append(row)
@@ -58,75 +82,83 @@
 
     def add_all(self, rows):
         """
         The method adds multiple embeddings to the database in batches, and in case of exceptions,
         it switches to adding them one by one. It then returns the list of successfully inserted rows.
 
         Args:
-            rows (List[EmbeddingModel]): A list of EmbeddingModel objects to add to the database.
+            rows (List[dct]): A list of dict objects to add to the database.
 
         Returns:
-            List[EmbeddingModel]: A list of successfully inserted EmbeddingModel objects.
+            List[dict]: A list of dictionaries representing EmbeddingModel objects from the collection with the given id.
         """
+        rows = [EmbeddingModel(**row) for row in rows]
+
         inserted_rows = []
 
         batch_size = 200
         extra_batch = len(rows) % batch_size > 0
         num_batches = len(rows) // batch_size + extra_batch
 
         with tqdm(total=len(rows), desc="Inserting rows to database") as pbar:
             for batch_index in range(num_batches):
                 batch_start = batch_index * batch_size
                 batch_end = batch_start + batch_size
                 batch = rows[batch_start:batch_end]
 
                 try:
-                    self.session.bulk_save_objects(batch)
+                    self.session.bulk_save_objects(batch)  # TODO using SQL
                     self.session.commit()
                     inserted_rows.extend(batch)
 
-                except (IntegrityError, Exception):
+                except (IntegrityError, Exception) as e:
                     self.session.rollback()
                     self.session.expunge_all()
                     inserted_rows.extend(self._add_rows_one_by_one(batch))
 
                 pbar.update(len(batch))
 
+        inserted_rows = [r.to_dict() for r in inserted_rows]
+
         return inserted_rows
 
     # This is only needed when bulk add in add_all is implemented
     def get_by_ids(self, ids):
         """
         Returns the embeddings with the given ids.
 
         Args:
             ids (List[str]): A list of embedding ids to retrieve.
 
         Returns:
-            List[EmbeddingModel]: A list of EmbeddingModel objects with the given ids.
+            List[dict]: A list of dictionaries representing EmbeddingModel objects from the collection with the given id.
         """
 
         # Get the successfully inserted data
         rows = (
             self.session.query(EmbeddingModel).filter(EmbeddingModel.id.in_(ids)).all()
         )
 
+        rows = [r.to_dict() for r in rows]
+
         return rows
 
     def get_by_collection_id(self, collection_id):
         """
         Returns all embeddings in the collection with the given id.
 
         Args:
             collection_id (str): The id of the collection to retrieve embeddings from.
 
         Returns:
-            List[EmbeddingModel]: A list of EmbeddingModel objects in the collection with the given id.
+            List[dict]: A list of dictionaries representing EmbeddingModel objects from the collection with the given id.
         """
 
         rows = (
             self.session.query(EmbeddingModel)
             .filter(EmbeddingModel.collection_id == collection_id)
             .all()
         )
 
+        rows = [r.to_dict() for r in rows]
+
         return rows
```

### Comparing `embedin-0.2.1/embedin.egg-info/PKG-INFO` & `embedin-0.2.2a0/embedin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,100 +12,107 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Embedin - Empower AI with persistent memory
 [![PyPI](https://img.shields.io/pypi/v/embedin?label=embedin)](https://pypi.org/project/embedin/)
 [![Coverage Status](https://coveralls.io/repos/github/EmbedInAI/EmbedInDB/badge.svg)](https://coveralls.io/github/EmbedInAI/EmbedInDB)
 
-## What is Embedin
-Embedin is a highly efficient software library designed to seamlessly convert widely-used databases, such as MySQL, PostgreSQL, and MS SQL Server, into a vector database with minimal effort. Its lightweight design enables quick and easy integration into your existing software stack, allowing you to leverage the benefits of a vector database without the need for extensive modifications to your current system. 
+Embedin is an open-source vector database and efficient library that seamlessly converts popular databases like MySQL, PostgreSQL, and MS SQL Server into vector databases with zero effort.
 
-With fast indexing and retrieval, it's ideal for high-performance applications such as natural language processing, image recognition, and recommendation systems. Embedin's simple API and query language make it easy to use and integrate. 
+Embedin is an ideal solution for AI applications like natural language processing, image recognition, and recommendation systems, offering fast indexing and retrieval. Its simple API and query language ensure ease of use and seamless integration.
+
+## Minimum Requirements
+Python 3.7 or higher.
 
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memory
+### Store embeddings in memory
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
-result = client.query("These are tests", top_k=1)
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+result = client.query("These are tests", top_k=1)  # Query the most similar text from the collection
 print(result)
 ```
 
-### Using Sqlite
+### Store embeddings in SQLite
 ```python
-from embedin.client import Client
+from embedin import Embedin
 
 url = 'sqlite:///test.db'
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using PostgreSQL
+### Store embeddings in PostgreSQL
+
+#### Start PostgreSQL Docker container
+```bash
+cd docker
+docker-compose up embedin-postgres
+```
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MySQL
+### Store embeddings in MySQL
+
+#### Start MySQL Docker container
+```bash
+cd docker
+docker-compose up embedin-mysql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
-client = Client(collection_name="test_collection", texts=["This is a test", "Hello world!"])
+client = Embedin(collection_name="test_collection", texts=["This is a test", "Hello world!"], url=url)
 result = client.query("These are tests", top_k=1)
 ```
 
-### Using MS-SQL
+### Store embeddings in SQL Server
+
+#### Start SQL Server Docker container
+```bash
+cd docker
+docker-compose up embedin-mssql
+```
+
+__example__
+
 ```python
 import os
 
-from embedin.client import Client
+from embedin import Embedin
 
 url = os.getenv('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
-client = Client(collection_name="test_collection", url=url)
+client = Embedin(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
-## For development
-
-Clone the repo
-```bash
-git clone https://github.com/EmbedInAI/embedin.git
-```
-
-Start PostgreSQL DB (Only necessary for using PostgreSQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-postgres
-```
+## More References
+* [API Reference](./API.md)
 
-Start MySQL DB (Only necessary for using MySQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mysql
-```
 
-Start MS-SQL DB (Only necessary for using MS-SQL as the storage)
-```bash
-cd docker
-docker-compose up embedin-mssql
-```
+## Contribute
+Please refer [Contributors Guide](./CONTRIBUTING.md)
 
-Run unit test with coverage report
-```bash
-coverage run -m unittest discover -s tests -p '*.py'
-coverage report
-```
+# TODO
+- unit test fail on faiss index (segmentation fault)
```

### Comparing `embedin-0.2.1/embedin.egg-info/SOURCES.txt` & `embedin-0.2.2a0/embedin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedin-0.2.1/setup.py` & `embedin-0.2.2a0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8"
     ) as fh:
         return fh.read()
 
 
 setuptools.setup(
     name="embedin",
-    version="0.2.1",
+    version="0.2.2-alpha",
     author="EmbedInAI",
     author_email="EmbedInAI@gmail.com",
     description="A lightweight vector database",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/EmbedInAI/EmbedInDB",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `embedin-0.2.1/tests/model/test_embedding_model.py` & `embedin-0.2.2a0/tests/model/test_embedding_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# -*- coding: utf-8 -*-
+# embedin - A vector database that empowers AI with persistent memory,
+# (C) 2023 EmbedInAI
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import unittest
 from datetime import datetime
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
 from embedin.model.embedding_model import Base, EmbeddingModel
```

### Comparing `embedin-0.2.1/tests/util/__init__.py` & `embedin-0.2.2a0/tests/util/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# -*- coding: utf-8 -*-
+# embedin - A vector database that empowers AI with persistent memory,
+# (C) 2023 EmbedInAI
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import unittest
 
 import numpy as np
 
 from embedin.util import to_np_array
```

