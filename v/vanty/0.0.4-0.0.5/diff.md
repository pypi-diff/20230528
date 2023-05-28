# Comparing `tmp/vanty-0.0.4.tar.gz` & `tmp/vanty-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanty-0.0.4.tar", max compression
+gzip compressed data, was "vanty-0.0.5.tar", max compression
```

## Comparing `vanty-0.0.4.tar` & `vanty-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.4/LICENSE
--rw-r--r--   0        0        0     1246 2023-05-26 17:56:09.814324 vanty-0.0.4/README.md
--rw-r--r--   0        0        0      660 2023-05-26 18:05:14.860558 vanty-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.4/vanty/__init__.py
--rw-r--r--   0        0        0       64 2023-05-26 18:05:07.438529 vanty-0.0.4/vanty/__main__.py
--rw-r--r--   0        0        0     2494 2023-05-26 18:06:12.522287 vanty-0.0.4/vanty/_client.py
--rw-r--r--   0        0        0     1194 2023-05-26 18:06:12.531596 vanty-0.0.4/vanty/auth.py
--rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.4/vanty/cli.py
--rw-r--r--   0        0        0     3652 2023-05-26 16:18:23.487417 vanty-0.0.4/vanty/config.py
--rw-r--r--   0        0        0     3469 2023-05-26 18:05:07.445619 vanty-0.0.4/vanty/dev.py
--rw-r--r--   0        0        0     1842 2023-05-26 16:00:32.579158 vanty-0.0.4/vanty/ops.py
--rw-r--r--   0        0        0      811 2023-05-26 17:53:22.962011 vanty-0.0.4/vanty/project.py
--rw-r--r--   0        0        0      948 2023-05-26 16:00:32.166597 vanty-0.0.4/vanty/schema.py
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 vanty-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1246 2023-05-26 17:56:09.814324 vanty-0.0.5/README.md
+-rw-r--r--   0        0        0      666 2023-05-28 11:36:32.036729 vanty-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.5/vanty/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-28 11:37:40.483417 vanty-0.0.5/vanty/__main__.py
+-rw-r--r--   0        0        0     2494 2023-05-26 18:06:12.522287 vanty-0.0.5/vanty/_client.py
+-rw-r--r--   0        0        0     1194 2023-05-26 18:06:12.531596 vanty-0.0.5/vanty/auth.py
+-rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.5/vanty/cli.py
+-rw-r--r--   0        0        0     3652 2023-05-26 16:18:23.487417 vanty-0.0.5/vanty/config.py
+-rw-r--r--   0        0        0     3469 2023-05-26 18:05:07.445619 vanty-0.0.5/vanty/dev.py
+-rw-r--r--   0        0        0     1842 2023-05-26 16:00:32.579158 vanty-0.0.5/vanty/ops.py
+-rw-r--r--   0        0        0      811 2023-05-26 17:53:22.962011 vanty-0.0.5/vanty/project.py
+-rw-r--r--   0        0        0      948 2023-05-26 16:00:32.166597 vanty-0.0.5/vanty/schema.py
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 vanty-0.0.5/PKG-INFO
```

### Comparing `vanty-0.0.4/LICENSE` & `vanty-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/README.md` & `vanty-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/pyproject.toml` & `vanty-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vanty"
-version = "0.0.4"
+version = "0.0.5"
 description = "CLI for installing and managing projects & applications from advantch.com"
 authors = ["Themba <themba@advantch.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "vanty"}]
 
 [tool.poetry.dependencies]
@@ -14,15 +14,15 @@
 django-environ = "^0.10.0"
 sh = "^2.0.4"
 toml = "^0.10.2"
 httpx = "^0.24.1"
 pydantic = "^1.10.8"
 
 [tool.poetry.scripts]
-vanty = "vanty.cli:app"
+vanty = "vanty.__main__:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 respx = "^0.20.1"
 
 
 [build-system]
```

### Comparing `vanty-0.0.4/vanty/_client.py` & `vanty-0.0.5/vanty/_client.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/auth.py` & `vanty-0.0.5/vanty/auth.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/config.py` & `vanty-0.0.5/vanty/config.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/dev.py` & `vanty-0.0.5/vanty/dev.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/ops.py` & `vanty-0.0.5/vanty/ops.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/project.py` & `vanty-0.0.5/vanty/project.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/vanty/schema.py` & `vanty-0.0.5/vanty/schema.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.4/PKG-INFO` & `vanty-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanty
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI for installing and managing projects & applications from advantch.com
 License: Apache
 Author: Themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

