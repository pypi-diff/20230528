# Comparing `tmp/timeblock-0.1.0.tar.gz` & `tmp/timeblock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeblock-0.1.0.tar", last modified: Sun May 28 21:37:39 2023, max compression
+gzip compressed data, was "timeblock-0.1.1.tar", last modified: Sun May 28 21:38:41 2023, max compression
```

## Comparing `timeblock-0.1.0.tar` & `timeblock-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:37:39.816927 timeblock-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-28 21:37:30.000000 timeblock-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-28 21:37:30.000000 timeblock-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:30.000000 timeblock-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:37:39.816927 timeblock-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:37:30.000000 timeblock-0.1.0/timeblock/tests/test_blocktimer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:37:39.816927 timeblock-0.1.0/timeblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 21:37:39.000000 timeblock-0.1.0/timeblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:38:41.364689 timeblock-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:38:41.364689 timeblock-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-28 21:38:32.000000 timeblock-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-28 21:38:32.000000 timeblock-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:38:32.000000 timeblock-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:38:41.364689 timeblock-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:38:41.360689 timeblock-0.1.1/timeblock/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 21:38:32.000000 timeblock-0.1.1/timeblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-28 21:38:32.000000 timeblock-0.1.1/timeblock/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:38:41.364689 timeblock-0.1.1/timeblock/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:38:32.000000 timeblock-0.1.1/timeblock/tests/test_blocktimer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:38:41.364689 timeblock-0.1.1/timeblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-28 21:38:41.000000 timeblock-0.1.1/timeblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-28 21:38:41.000000 timeblock-0.1.1/timeblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:38:41.000000 timeblock-0.1.1/timeblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 21:38:41.000000 timeblock-0.1.1/timeblock.egg-info/top_level.txt
```

### Comparing `timeblock-0.1.0/PKG-INFO` & `timeblock-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: timeblock
-Version: 0.1.0
+Version: 0.1.1
 Summary: Time blocks of code using a context manager
 Author-email: Daniel Hails <timeblock@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/timeblock
 Project-URL: Bug Tracker, https://github.com/DJRHails/timeblock/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🕐 timeblock
 
 Helpful snippet for timing blocks, basically [contexttimer](https://github.com/brouberol/contexttimer) with a few tweaks / forked.
 
 ```bash
-pip install timeblock==0.1.0
+pip install timeblock==0.1.1
 ```
 
 ```python
 from timeblock import Timer
 
 with Timer() as timer:
     sleep(1)
```

### Comparing `timeblock-0.1.0/pyproject.toml` & `timeblock-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timeblock"
-version = "0.1.0"
+version = "0.1.1"
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
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `timeblock-0.1.0/timeblock/block.py` & `timeblock-0.1.1/timeblock/block.py`

 * *Files identical despite different names*

### Comparing `timeblock-0.1.0/timeblock.egg-info/PKG-INFO` & `timeblock-0.1.1/timeblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: timeblock
-Version: 0.1.0
+Version: 0.1.1
 Summary: Time blocks of code using a context manager
 Author-email: Daniel Hails <timeblock@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/timeblock
 Project-URL: Bug Tracker, https://github.com/DJRHails/timeblock/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🕐 timeblock
 
 Helpful snippet for timing blocks, basically [contexttimer](https://github.com/brouberol/contexttimer) with a few tweaks / forked.
 
 ```bash
-pip install timeblock==0.1.0
+pip install timeblock==0.1.1
 ```
 
 ```python
 from timeblock import Timer
 
 with Timer() as timer:
     sleep(1)
```

