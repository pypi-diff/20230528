# Comparing `tmp/domjudge_utility-0.0.8.tar.gz` & `tmp/domjudge_utility-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domjudge_utility-0.0.8.tar", max compression
+gzip compressed data, was "domjudge_utility-0.0.9.tar", max compression
```

## Comparing `domjudge_utility-0.0.8.tar` & `domjudge_utility-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/LICENSE
--rw-r--r--   0        0        0      636 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/README.md
--rw-r--r--   0        0        0       47 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/__init__.py
--rw-r--r--   0        0        0    22055 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/dump.py
--rw-r--r--   0        0        0     3329 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/dump_config.py
--rw-r--r--   0        0        0      394 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/utils.py
--rw-r--r--   0        0        0       22 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/version.py
--rw-r--r--   0        0        0     1161 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/README.md
+-rw-r--r--   0        0        0       47 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/domjudge_utility/__init__.py
+-rw-r--r--   0        0        0    22063 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/domjudge_utility/dump.py
+-rw-r--r--   0        0        0     3329 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/domjudge_utility/dump_config.py
+-rw-r--r--   0        0        0      394 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/domjudge_utility/utils.py
+-rw-r--r--   0        0        0       22 2023-05-27 16:19:23.982420 domjudge_utility-0.0.9/domjudge_utility/version.py
+-rw-r--r--   0        0        0     1161 2023-05-27 16:19:23.986420 domjudge_utility-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.9/PKG-INFO
```

### Comparing `domjudge_utility-0.0.8/LICENSE` & `domjudge_utility-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.8/README.md` & `domjudge_utility-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.8/domjudge_utility/dump.py` & `domjudge_utility-0.0.9/domjudge_utility/dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
             contest["duration"]) - self.get_seconds(contest["scoreboard_freeze_duration"])
 
         users = {}
         solutions = {}
 
         for team in teams:
             item = {}
-            item['name'] = team['name']
+            item['name'] = team['display_name']
             item['college'] = team['affiliation']
             item['is_exclude'] = self.is_observers(team)
 
             users[team['id']] = item
 
         submission_index = 1
         for submission in submissions:
```

### Comparing `domjudge_utility-0.0.8/domjudge_utility/dump_config.py` & `domjudge_utility-0.0.9/domjudge_utility/dump_config.py`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.8/pyproject.toml` & `domjudge_utility-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domjudge-utility"
-version = "0.0.8"
+version = "0.0.9"
 description = "DOMjudge Utility"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `domjudge_utility-0.0.8/PKG-INFO` & `domjudge_utility-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domjudge-utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: DOMjudge Utility
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

