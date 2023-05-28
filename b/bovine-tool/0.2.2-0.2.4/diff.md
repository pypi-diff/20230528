# Comparing `tmp/bovine_tool-0.2.2.tar.gz` & `tmp/bovine_tool-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_tool-0.2.2.tar", max compression
+gzip compressed data, was "bovine_tool-0.2.4.tar", max compression
```

## Comparing `bovine_tool-0.2.2.tar` & `bovine_tool-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      952 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/__init__.py
--rw-r--r--   0        0        0      495 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/cleanup.py
--rw-r--r--   0        0        0      277 2023-05-22 14:17:04.678842 bovine_tool-0.2.2/bovine_tool/create.py
--rw-r--r--   0        0        0     2014 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/manage.py
--rw-r--r--   0        0        0      770 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/register.py
--rw-r--r--   0        0        0      557 2023-05-22 14:17:04.682842 bovine_tool-0.2.2/bovine_tool/store.py
--rw-r--r--   0        0        0      520 2023-05-25 18:44:02.806690 bovine_tool-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 bovine_tool-0.2.2/setup.py
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 bovine_tool-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1349 2023-05-27 18:23:43.579051 bovine_tool-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 14:17:04.678842 bovine_tool-0.2.4/bovine_tool/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-22 14:17:04.678842 bovine_tool-0.2.4/bovine_tool/cleanup.py
+-rw-r--r--   0        0        0      277 2023-05-22 14:17:04.678842 bovine_tool-0.2.4/bovine_tool/create.py
+-rw-r--r--   0        0        0     2014 2023-05-22 14:17:04.682842 bovine_tool-0.2.4/bovine_tool/manage.py
+-rw-r--r--   0        0        0      770 2023-05-22 14:17:04.682842 bovine_tool-0.2.4/bovine_tool/register.py
+-rw-r--r--   0        0        0      557 2023-05-22 14:17:04.682842 bovine_tool-0.2.4/bovine_tool/store.py
+-rw-r--r--   0        0        0      520 2023-05-27 18:46:03.793874 bovine_tool-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 bovine_tool-0.2.4/setup.py
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 bovine_tool-0.2.4/PKG-INFO
```

### Comparing `bovine_tool-0.2.2/bovine_tool/manage.py` & `bovine_tool-0.2.4/bovine_tool/manage.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.2/bovine_tool/register.py` & `bovine_tool-0.2.4/bovine_tool/register.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.2/bovine_tool/store.py` & `bovine_tool-0.2.4/bovine_tool/store.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.2/pyproject.toml` & `bovine_tool-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-tool"
-version = "0.2.2"
+version = "0.2.4"
 description = "Basic tools to administrate a bovine herd"
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_tool"}]
 repository = "https://codeberg.org/bovine/bovine"
 
 [tool.poetry.dependencies]
```

