# Comparing `tmp/fil-1.1.0.tar.gz` & `tmp/fil-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fil-1.1.0.tar", max compression
+gzip compressed data, was "fil-1.2.0.tar", max compression
```

## Comparing `fil-1.1.0.tar` & `fil-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.1.0/README.md
--rw-r--r--   0        0        0     5579 2023-05-21 10:49:57.389177 fil-1.1.0/fil.py
--rw-r--r--   0        0        0      496 2023-05-21 10:50:21.836044 fil-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 fil-1.1.0/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.2.0/README.md
+-rw-r--r--   0        0        0     5633 2023-05-28 10:47:19.543564 fil-1.2.0/fil.py
+-rw-r--r--   0        0        0      496 2023-05-28 10:48:29.683341 fil-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.2.0/PKG-INFO
```

### Comparing `fil-1.1.0/README.md` & `fil-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fil-1.1.0/fil.py` & `fil-1.2.0/fil.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     dicts = ({'key': i} for i in range(10))
     fil.write(dicts, 'file.jsonl')
 """
 
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Union
-import json
+try:
+    import ujson as json
+except ImportError:
+    import json
 import safer
 
 __all__ = 'read', 'write', 'SUFFIX_TO_CLASS'
 
 # JSON is the type used by JSON, TOML, or Yaml
 JSON = Union[Dict, List, None, bool, float, int, str]
 JSON_Lines = Iterator[JSON]
```

### Comparing `fil-1.1.0/PKG-INFO` & `fil-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fil
-Version: 1.1.0
+Version: 1.2.0
 Summary: 🏺 Read/write JSON/TOML/Yaml/txt 🏺
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

