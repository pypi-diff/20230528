# Comparing `tmp/dtbase-0.0.2.tar.gz` & `tmp/dtbase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtbase-0.0.2.tar", max compression
+gzip compressed data, was "dtbase-0.0.3.tar", max compression
```

## Comparing `dtbase-0.0.2.tar` & `dtbase-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.2/dtbase/__init__.py
--rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.2/dtbase/config.py
--rw-r--r--   0        0        0     5718 2023-05-26 23:58:37.934512 dtbase-0.0.2/dtbase/engine.py
--rw-r--r--   0        0        0      369 2023-05-26 23:58:37.937495 dtbase-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      632 2023-05-26 23:58:47.685747 dtbase-0.0.2/setup.py
--rw-r--r--   0        0        0      412 2023-05-26 23:58:47.685947 dtbase-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.3/dtbase/__init__.py
+-rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.3/dtbase/config.py
+-rw-r--r--   0        0        0     5718 2023-05-26 23:58:37.934512 dtbase-0.0.3/dtbase/engine.py
+-rw-r--r--   0        0        0      369 2023-05-28 21:57:12.156664 dtbase-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      632 2023-05-28 21:57:24.397059 dtbase-0.0.3/setup.py
+-rw-r--r--   0        0        0      412 2023-05-28 21:57:24.397279 dtbase-0.0.3/PKG-INFO
```

### Comparing `dtbase-0.0.2/dtbase/config.py` & `dtbase-0.0.3/dtbase/config.py`

 * *Files identical despite different names*

### Comparing `dtbase-0.0.2/dtbase/engine.py` & `dtbase-0.0.3/dtbase/engine.py`

 * *Files identical despite different names*

