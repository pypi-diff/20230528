# Comparing `tmp/dhint-0.0.5.tar.gz` & `tmp/dhint-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.5.tar", max compression
+gzip compressed data, was "dhint-0.0.6.tar", max compression
```

## Comparing `dhint-0.0.5.tar` & `dhint-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      220 2023-05-26 17:43:41.774221 dhint-0.0.5/dhint/__init__.py
--rw-r--r--   0        0        0     7759 2023-05-26 17:43:41.772127 dhint-0.0.5/dhint/base.py
--rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.5/dhint/collections.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.5/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.5/dhint/hints.py
--rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.5/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.5/dhint/protocols.py
--rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.5/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.5/dhint/type_hint.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.5/dhint/types.py
--rw-r--r--   0        0        0      330 2023-05-26 17:45:55.539685 dhint-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      616 2023-05-26 17:46:02.951814 dhint-0.0.5/setup.py
--rw-r--r--   0        0        0      382 2023-05-26 17:46:02.952010 dhint-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-05-28 18:11:56.153127 dhint-0.0.6/dhint/__init__.py
+-rw-r--r--   0        0        0    12346 2023-05-28 21:49:45.365627 dhint-0.0.6/dhint/base.py
+-rw-r--r--   0        0        0     4068 2023-05-27 02:24:55.001024 dhint-0.0.6/dhint/collections.py
+-rw-r--r--   0        0        0     5276 2023-05-28 21:49:45.368265 dhint-0.0.6/dhint/descriptors.py
+-rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.6/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.6/dhint/hints.py
+-rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.6/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.6/dhint/protocols.py
+-rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.6/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.6/dhint/type_hint.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.6/dhint/types.py
+-rw-r--r--   0        0        0      330 2023-05-28 21:51:27.869541 dhint-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-28 21:51:47.466280 dhint-0.0.6/setup.py
+-rw-r--r--   0        0        0      382 2023-05-28 21:51:47.466514 dhint-0.0.6/PKG-INFO
```

### Comparing `dhint-0.0.5/dhint/collections.py` & `dhint-0.0.6/dhint/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__ = ['DictModel', 'StringModel', 'Regex', 'ListModel', 'StringListModel']
+__all__ = ['DictModel', 'StringModel', 'Regex', 'ListModel', 'StringListModel', 'SetModel']
 
 import re
 from typing import Collection, Any, Iterable, Optional
 from collections import UserDict, UserList, UserString, deque, ChainMap
 from .base import *
 
 
@@ -41,14 +41,20 @@
 
     def __delitem__(self, key):
         try:
             del self.data[key]
         finally:
             pass
 
+
+class SetModel(set):
+    def __init__(self, *args):
+        self.data = ListModel()
+        self.data.include(*args)
+        super().__init__(self.data)
     
 class StringModel(UserString, BaseCollection):
     """Container for strings"""
     
     def init_data(self) -> str:
         if len(self.args) > 0:
             data = str(self.args.pop(0))
```

### Comparing `dhint-0.0.5/dhint/functions.py` & `dhint-0.0.6/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/dhint/hints.py` & `dhint-0.0.6/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/dhint/json_encoder.py` & `dhint-0.0.6/dhint/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/dhint/subdescriptor.py` & `dhint-0.0.6/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/dhint/type_hint.py` & `dhint-0.0.6/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/dhint/types.py` & `dhint-0.0.6/dhint/types.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.5/setup.py` & `dhint-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0', 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

