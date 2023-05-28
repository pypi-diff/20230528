# Comparing `tmp/pyserini_indexer-0.2.0.tar.gz` & `tmp/pyserini_indexer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserini_indexer-0.2.0.tar", last modified: Sun May 28 14:24:16 2023, max compression
+gzip compressed data, was "pyserini_indexer-0.3.1.tar", last modified: Sun May 28 17:36:13 2023, max compression
```

## Comparing `pyserini_indexer-0.2.0.tar` & `pyserini_indexer-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,12 @@
--rw-r--r--   0        0        0     1018 2023-05-28 14:14:34.812707 pyserini_indexer-0.2.0/README.md
--rw-r--r--   0        0        0       96 2023-05-27 19:25:39.286631 pyserini_indexer-0.2.0/handlers/__init__.py
--rw-r--r--   0        0        0     3315 2023-05-28 13:27:49.042822 pyserini_indexer-0.2.0/handlers/indexes.py
--rw-r--r--   0        0        0     1693 2023-05-28 14:19:45.829361 pyserini_indexer-0.2.0/handlers/searcher.py
--rw-r--r--   0        0        0      461 2023-05-28 14:24:16.662683 pyserini_indexer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3663 2023-05-27 22:51:12.186121 pyserini_indexer-0.2.0/tests/indexes/ance/docid
--rw-r--r--   0        0        0  1250349 2023-05-27 22:51:12.186121 pyserini_indexer-0.2.0/tests/indexes/ance/index
--rw-r--r--   0        0        0      157 2023-05-27 22:48:29.052795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdm
--rw-r--r--   0        0        0    43953 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdt
--rw-r--r--   0        0        0       64 2023-05-27 22:48:29.052795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fdx
--rw-r--r--   0        0        0      343 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.fnm
--rw-r--r--   0        0        0      109 2023-05-27 22:48:29.032795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.nvd
--rw-r--r--   0        0        0      103 2023-05-27 22:48:29.032795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.nvm
--rw-r--r--   0        0        0      488 2023-05-27 22:48:29.092795 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.si
--rw-r--r--   0        0        0    31054 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvd
--rw-r--r--   0        0        0      162 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvm
--rw-r--r--   0        0        0       82 2023-05-27 22:48:29.056128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0.tvx
--rw-r--r--   0        0        0     4291 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.doc
--rw-r--r--   0        0        0      473 2023-05-27 22:48:29.036128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.dvd
--rw-r--r--   0        0        0      133 2023-05-27 22:48:29.036128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.dvm
--rw-r--r--   0        0        0     8835 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.pos
--rw-r--r--   0        0        0    20243 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tim
--rw-r--r--   0        0        0      554 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tip
--rw-r--r--   0        0        0      280 2023-05-27 22:48:29.086128 pyserini_indexer-0.2.0/tests/indexes/bm25/_0_Lucene90_0.tmd
--rw-r--r--   0        0        0      154 2023-05-27 22:48:29.099461 pyserini_indexer-0.2.0/tests/indexes/bm25/segments_1
--rw-r--r--   0        0        0        0 2023-05-27 22:48:28.849461 pyserini_indexer-0.2.0/tests/indexes/bm25/write.lock
--rw-r--r--   0        0        0     3663 2023-05-27 22:51:28.442788 pyserini_indexer-0.2.0/tests/indexes/minilm_v2/docid
--rw-r--r--   0        0        0   625197 2023-05-27 22:51:28.442788 pyserini_indexer-0.2.0/tests/indexes/minilm_v2/index
--rw-r--r--   0        0        0     3663 2023-05-28 13:09:53.979533 pyserini_indexer-0.2.0/tests/indexes/tct_colbert/docid
--rw-r--r--   0        0        0  1250349 2023-05-28 13:09:53.989533 pyserini_indexer-0.2.0/tests/indexes/tct_colbert/index
--rw-r--r--   0        0        0     1632 2023-05-28 14:19:02.639363 pyserini_indexer-0.2.0/tests/test_searcher.py
--rw-r--r--   0        0        0     3265 2023-05-27 19:53:33.706563 pyserini_indexer-0.2.0/tests/test_splitter.py
--rw-r--r--   0        0        0      909 2023-05-28 13:27:49.036155 pyserini_indexer-0.2.0/tests/test_vectors.py
--rw-r--r--   0        0        0        0 2023-05-27 11:43:05.806172 pyserini_indexer-0.2.0/utils/__init__.py
--rw-r--r--   0        0        0      550 2023-05-27 19:51:31.406568 pyserini_indexer-0.2.0/utils/models.py
--rw-r--r--   0        0        0     1754 2023-05-27 09:14:18.293201 pyserini_indexer-0.2.0/utils/splitter.py
--rw-r--r--   0        0        0      733 2023-05-28 13:27:49.046155 pyserini_indexer-0.2.0/utils/vectors.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 pyserini_indexer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-05-28 14:14:34.812707 pyserini_indexer-0.3.1/README.md
+-rw-r--r--   0        0        0      678 2023-05-28 17:36:13.602977 pyserini_indexer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-05-28 17:19:04.696352 pyserini_indexer-0.3.1/pyserini_indexer/__init__.py
+-rw-r--r--   0        0        0     1808 2023-05-28 17:18:56.229685 pyserini_indexer-0.3.1/pyserini_indexer/__main__.py
+-rw-r--r--   0        0        0      116 2023-05-28 16:00:08.529877 pyserini_indexer-0.3.1/pyserini_indexer/handlers/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-28 17:22:38.523010 pyserini_indexer-0.3.1/pyserini_indexer/handlers/indexes.py
+-rw-r--r--   0        0        0     1710 2023-05-28 17:22:38.523010 pyserini_indexer-0.3.1/pyserini_indexer/handlers/searcher.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:43:05.806172 pyserini_indexer-0.3.1/pyserini_indexer/utils/__init__.py
+-rw-r--r--   0        0        0      550 2023-05-27 19:51:31.406568 pyserini_indexer-0.3.1/pyserini_indexer/utils/models.py
+-rw-r--r--   0        0        0     1754 2023-05-27 09:14:18.293201 pyserini_indexer-0.3.1/pyserini_indexer/utils/splitter.py
+-rw-r--r--   0        0        0      733 2023-05-28 17:22:38.526343 pyserini_indexer-0.3.1/pyserini_indexer/utils/vectors.py
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 pyserini_indexer-0.3.1/PKG-INFO
```

### Comparing `pyserini_indexer-0.2.0/README.md` & `pyserini_indexer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyserini_indexer-0.2.0/handlers/indexes.py` & `pyserini_indexer-0.3.1/pyserini_indexer/handlers/indexes.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import (  # we use python 3.9 so typings are bit outdated :/
     Callable, Dict, List, Union)
 
 import faiss
 import numpy as np
 import tqdm
 
-import utils.models as models
-import utils.vectors as vectors
-from utils.splitter import redundant_splitter
+import pyserini_indexer.utils.models as models
+import pyserini_indexer.utils.vectors as vectors
+from pyserini_indexer.utils.splitter import redundant_splitter
 
 NUM_THREADS = os.getenv("NUM_THREADS", "2")
 
 
 def build_bm25_command(inp, out):
     return [
         "python",
```

### Comparing `pyserini_indexer-0.2.0/handlers/searcher.py` & `pyserini_indexer-0.3.1/pyserini_indexer/handlers/searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from typing import Optional
 
 import pyserini.search.faiss as faiss
 import pyserini.search.hybrid as hybrid
 import pyserini.search.lucene as lucene
 
-import utils.models as models
+import pyserini_indexer.utils.models as models
 
 
 @functools.lru_cache
 def get_searcher(
     index_dir: str,
     *,
     dense_model: Optional[str] = None,
```

### Comparing `pyserini_indexer-0.2.0/utils/models.py` & `pyserini_indexer-0.3.1/pyserini_indexer/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyserini_indexer-0.2.0/utils/splitter.py` & `pyserini_indexer-0.3.1/pyserini_indexer/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `pyserini_indexer-0.2.0/utils/vectors.py` & `pyserini_indexer-0.3.1/pyserini_indexer/utils/vectors.py`

 * *Files identical despite different names*

### Comparing `pyserini_indexer-0.2.0/PKG-INFO` & `pyserini_indexer-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyserini-indexer
-Version: 0.2.0
-Summary: Helper application for building index files that uses pyserini
+Version: 0.3.1
+Summary: Helper application for building search indexes with pyserini
 Author-Email: michal <michalwilk139@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: pyserini>=0.21.0
 Requires-Dist: faiss-cpu>=1.7.4
 Requires-Dist: torch>=2.0.1
 Description-Content-Type: text/markdown
```

