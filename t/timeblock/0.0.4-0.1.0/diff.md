# Comparing `tmp/timeblock-0.0.4.tar.gz` & `tmp/timeblock-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeblock-0.0.4.tar", last modified: Sun May 28 21:34:15 2023, max compression
+gzip compressed data, was "timeblock-0.1.0.tar", last modified: Sun May 28 21:37:39 2023, max compression
```

## Comparing `timeblock-0.0.4.tar` & `timeblock-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:34:15.730635 timeblock-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:34:15.730635 timeblock-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-28 21:34:06.000000 timeblock-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-28 21:34:06.000000 timeblock-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:34:06.000000 timeblock-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:34:15.730635 timeblock-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:34:15.726635 timeblock-0.0.4/timeblock/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 21:34:06.000000 timeblock-0.0.4/timeblock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:34:15.726635 timeblock-0.0.4/timeblock/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:34:06.000000 timeblock-0.0.4/timeblock/tests/test_blocktimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-28 21:34:06.000000 timeblock-0.0.4/timeblock/timeblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:34:15.726635 timeblock-0.0.4/timeblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:34:15.000000 timeblock-0.0.4/timeblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-28 21:34:15.000000 timeblock-0.0.4/timeblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:34:15.000000 timeblock-0.0.4/timeblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 21:34:15.000000 timeblock-0.0.4/timeblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:37:39.816927 timeblock-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-28 21:37:30.000000 timeblock-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-28 21:37:30.000000 timeblock-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:30.000000 timeblock-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:37:39.816927 timeblock-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/tests/test_blocktimer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/top_level.txt
```

### Comparing `timeblock-0.0.4/PKG-INFO` & `timeblock-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: timeblock
-Version: 0.0.4
+Version: 0.1.0
 Summary: Time blocks of code using a context manager
 Author-email: Daniel Hails <timeblock@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/timeblock
 Project-URL: Bug Tracker, https://github.com/DJRHails/timeblock/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🕐 timeblock
 
 Helpful snippet for timing blocks, basically [contexttimer](https://github.com/brouberol/contexttimer) with a few tweaks / forked.
 
 ```bash
-pip install timeblock==0.0.4
+pip install timeblock==0.1.0
 ```
 
 ```python
 from timeblock import Timer
 
 with Timer() as timer:
     sleep(1)
```

### Comparing `timeblock-0.0.4/pyproject.toml` & `timeblock-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timeblock"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
     { name="Daniel Hails", email="timeblock@hails.info" },
 ]
 description = "Time blocks of code using a context manager"
 requires-python = ">=3.10"
 dynamic = ["dependencies", "readme"]
 
@@ -20,15 +20,15 @@
 dependencies = {file = ["requirements.txt"]}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `timeblock-0.0.4/timeblock/timeblock.py` & `timeblock-0.1.0/timeblock/block.py`

 * *Files identical despite different names*

### Comparing `timeblock-0.0.4/timeblock.egg-info/PKG-INFO` & `timeblock-0.1.0/timeblock.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: timeblock
-Version: 0.0.4
+Version: 0.1.0
 Summary: Time blocks of code using a context manager
 Author-email: Daniel Hails <timeblock@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/timeblock
 Project-URL: Bug Tracker, https://github.com/DJRHails/timeblock/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🕐 timeblock
 
 Helpful snippet for timing blocks, basically [contexttimer](https://github.com/brouberol/contexttimer) with a few tweaks / forked.
 
 ```bash
-pip install timeblock==0.0.4
+pip install timeblock==0.1.0
 ```
 
 ```python
 from timeblock import Timer
 
 with Timer() as timer:
     sleep(1)
```

