# Comparing `tmp/pyserini_indexer-0.1.0.tar.gz` & `tmp/pyserini_indexer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserini_indexer-0.1.0.tar", last modified: Fri May 26 20:07:37 2023, max compression
+gzip compressed data, was "pyserini_indexer-0.2.0.tar", last modified: Sun May 28 14:24:16 2023, max compression
```

## Comparing `pyserini_indexer-0.1.0.tar` & `pyserini_indexer-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,38 @@
--rw-r--r--   0        0        0      327 2023-05-26 20:01:52.422404 pyserini_indexer-0.1.0/README.md
--rw-r--r--   0        0        0     2428 2023-05-26 19:31:26.125812 pyserini_indexer-0.1.0/__main__.py
--rw-r--r--   0        0        0     1280 2023-05-26 19:40:56.849122 pyserini_indexer-0.1.0/indexes.py
--rw-r--r--   0        0        0      461 2023-05-26 20:07:37.452390 pyserini_indexer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 pyserini_indexer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-05-28 14:14:34.812707 pyserini_indexer-0.2.0/README.md
+-rw-r--r--   0        0        0       96 2023-05-27 19:25:39.286631 pyserini_indexer-0.2.0/handlers/__init__.py
+-rw-r--r--   0        0        0     3315 2023-05-28 13:27:49.042822 pyserini_indexer-0.2.0/handlers/indexes.py
+-rw-r--r--   0        0        0     1693 2023-05-28 14:19:45.829361 pyserini_indexer-0.2.0/handlers/searcher.py
+-rw-r--r--   0        0        0      461 2023-05-28 14:24:16.662683 pyserini_indexer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3663 2023-05-27 22:51:12.186121 pyserini_indexer-0.2.0/tests/indexes/ance/docid
+-rw-r--r--   0        0        0  1250349 2023-05-27 22:51:12.186121 pyserini_indexer-0.2.0/tests/indexes/ance/index
+-rw-r--r--   0        0        0      157 2023-05-27 22:48:29.052795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdm
+-rw-r--r--   0        0        0    43953 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdt
+-rw-r--r--   0        0        0       64 2023-05-27 22:48:29.052795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdx
+-rw-r--r--   0        0        0      343 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fnm
+-rw-r--r--   0        0        0      109 2023-05-27 22:48:29.032795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.nvd
+-rw-r--r--   0        0        0      103 2023-05-27 22:48:29.032795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.nvm
+-rw-r--r--   0        0        0      488 2023-05-27 22:48:29.092795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.si
+-rw-r--r--   0        0        0    31054 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvd
+-rw-r--r--   0        0        0      162 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvm
+-rw-r--r--   0        0        0       82 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvx
+-rw-r--r--   0        0        0     4291 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.doc
+-rw-r--r--   0        0        0      473 2023-05-27 22:48:29.036128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.dvd
+-rw-r--r--   0        0        0      133 2023-05-27 22:48:29.036128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.dvm
+-rw-r--r--   0        0        0     8835 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.pos
+-rw-r--r--   0        0        0    20243 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tim
+-rw-r--r--   0        0        0      554 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tip
+-rw-r--r--   0        0        0      280 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tmd
+-rw-r--r--   0        0        0      154 2023-05-27 22:48:29.099461 pyserini_indexer-0.2.0/tests/indexes/bm25/segments_1
+-rw-r--r--   0        0        0        0 2023-05-27 22:48:28.849461 pyserini_indexer-0.2.0/tests/indexes/bm25/write.lock
+-rw-r--r--   0        0        0     3663 2023-05-27 22:51:28.442788 pyserini_indexer-0.2.0/tests/indexes/minilm_v2/docid
+-rw-r--r--   0        0        0   625197 2023-05-27 22:51:28.442788 pyserini_indexer-0.2.0/tests/indexes/minilm_v2/index
+-rw-r--r--   0        0        0     3663 2023-05-28 13:09:53.979533 pyserini_indexer-0.2.0/tests/indexes/tct_colbert/docid
+-rw-r--r--   0        0        0  1250349 2023-05-28 13:09:53.989533 pyserini_indexer-0.2.0/tests/indexes/tct_colbert/index
+-rw-r--r--   0        0        0     1632 2023-05-28 14:19:02.639363 pyserini_indexer-0.2.0/tests/test_searcher.py
+-rw-r--r--   0        0        0     3265 2023-05-27 19:53:33.706563 pyserini_indexer-0.2.0/tests/test_splitter.py
+-rw-r--r--   0        0        0      909 2023-05-28 13:27:49.036155 pyserini_indexer-0.2.0/tests/test_vectors.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:43:05.806172 pyserini_indexer-0.2.0/utils/__init__.py
+-rw-r--r--   0        0        0      550 2023-05-27 19:51:31.406568 pyserini_indexer-0.2.0/utils/models.py
+-rw-r--r--   0        0        0     1754 2023-05-27 09:14:18.293201 pyserini_indexer-0.2.0/utils/splitter.py
+-rw-r--r--   0        0        0      733 2023-05-28 13:27:49.046155 pyserini_indexer-0.2.0/utils/vectors.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 pyserini_indexer-0.2.0/PKG-INFO
```

