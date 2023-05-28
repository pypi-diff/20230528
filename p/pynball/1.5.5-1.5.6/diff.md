# Comparing `tmp/pynball-1.5.5.tar.gz` & `tmp/pynball-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball-1.5.5.tar", last modified: Fri Apr 21 13:35:21 2023, max compression
+gzip compressed data, was "pynball-1.5.6.tar", last modified: Sun May 28 12:44:49 2023, max compression
```

## Comparing `pynball-1.5.5.tar` & `pynball-1.5.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.403856 pynball-1.5.5/
--rw-rw-rw-   0        0        0      140 2023-04-19 21:02:11.000000 pynball-1.5.5/AUTHORS.md
--rw-rw-rw-   0        0        0     7570 2023-04-21 13:35:11.000000 pynball-1.5.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.5/LICENSE
--rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12613 2023-04-21 13:35:21.403856 pynball-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    11282 2023-04-19 21:46:58.000000 pynball-1.5.5/README.md
--rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0     1571 2023-04-21 13:35:21.403856 pynball-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:30:25.000000 pynball-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.225375 pynball-1.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.256684 pynball-1.5.5/src/pynball/
--rw-rw-rw-   0        0        0      293 2023-04-21 13:35:11.000000 pynball-1.5.5/src/pynball/__init__.py
--rw-rw-rw-   0        0        0    31204 2023-04-21 12:24:49.000000 pynball-1.5.5/src/pynball/pynball.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.272291 pynball-1.5.5/src/pynball.egg-info/
--rw-rw-rw-   0        0        0    12613 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.403856 pynball-1.5.5/tests/
--rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.5/tests/test__check_pyenv.py
--rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.5/tests/test__check_virtual_env.py
--rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.5/tests/test__execute.py
--rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.5/tests/test__get_pynball.py
--rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.5/tests/test__message.py
--rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.5/tests/test__set_get_del_env.py
--rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.5/tests/test__set_pynball.py
--rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.5/tests/test_add.py
--rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.5/tests/test_delete.py
--rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.5/tests/test_lsproject.py
--rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.5/tests/test_mkproject.py
--rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.5/tests/test_rmproject.py
--rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.5/tests/test_version.py
--rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.5/tests/test_versions.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.126065 pynball-1.5.6/
+-rw-rw-rw-   0        0        0      140 2023-04-19 21:02:11.000000 pynball-1.5.6/AUTHORS.md
+-rw-rw-rw-   0        0        0     7598 2023-05-28 12:44:37.000000 pynball-1.5.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12613 2023-05-28 12:44:49.126065 pynball-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11282 2023-04-19 21:46:58.000000 pynball-1.5.6/README.md
+-rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1571 2023-05-28 12:44:49.126065 pynball-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:30:25.000000 pynball-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.016680 pynball-1.5.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.047935 pynball-1.5.6/src/pynball/
+-rw-rw-rw-   0        0        0      293 2023-05-28 12:44:38.000000 pynball-1.5.6/src/pynball/__init__.py
+-rw-rw-rw-   0        0        0    31371 2023-05-28 11:13:49.000000 pynball-1.5.6/src/pynball/pynball.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.063553 pynball-1.5.6/src/pynball.egg-info/
+-rw-rw-rw-   0        0        0    12613 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-05-28 12:44:49.000000 pynball-1.5.6/src/pynball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 12:44:48.000000 pynball-1.5.6/src/pynball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 12:44:49.110432 pynball-1.5.6/tests/
+-rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.6/tests/test__check_pyenv.py
+-rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.6/tests/test__check_virtual_env.py
+-rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.6/tests/test__execute.py
+-rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.6/tests/test__get_pynball.py
+-rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.6/tests/test__message.py
+-rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.6/tests/test__set_get_del_env.py
+-rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.6/tests/test__set_pynball.py
+-rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.6/tests/test_add.py
+-rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.6/tests/test_delete.py
+-rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.6/tests/test_lsproject.py
+-rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.6/tests/test_mkproject.py
+-rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.6/tests/test_rmproject.py
+-rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.6/tests/test_version.py
+-rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.6/tests/test_versions.py
```

### Comparing `pynball-1.5.5/CHANGELOG.md` & `pynball-1.5.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.6 (2023-05-28)
+
+
 ## v1.5.5 (2023-04-21)
 ### Fix
 * Shebang for version 3 env ([`57d4c92`](https://github.com/Stephen-RA-King/pynball/commit/57d4c927521b73c715f5f574fe208b2f9966f878))
 
 ### Documentation
 * Update email link ([`39fba7a`](https://github.com/Stephen-RA-King/pynball/commit/39fba7adc7058d786735e65daab3f8c7d979aaee))
 * Update email address ([`736bb43`](https://github.com/Stephen-RA-King/pynball/commit/736bb432ab7501c58c9bab0813b560e6316cae22))
```

### Comparing `pynball-1.5.5/LICENSE` & `pynball-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/PKG-INFO` & `pynball-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.5
+Version: 1.5.6
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynball-1.5.5/README.md` & `pynball-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/pyproject.toml` & `pynball-1.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/setup.cfg` & `pynball-1.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/src/pynball/pynball.py` & `pynball-1.5.6/src/pynball/pynball.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,15 +680,18 @@
         return
     for directory in [_WORKON_HOME, _PROJECT_HOME]:
         del_path = directory / project_name
         if directory == _PROJECT_HOME and delete_all != "y":
             continue
         try:
             shutil.rmtree(del_path, onerror=del_rw)
-            message = f"'{project_name}' has been deleted"
+            if directory == _WORKON_HOME:
+                message = f"'{project_name}' (virtualenv files) have been deleted"
+            else:
+                message = f"'{project_name}' (project files) have been deleted"
             _feedback(message, "nominal")
         except FileNotFoundError:
             message = f"Project: '{project_name}' does not exist"
             _feedback(message, "warning")
         except PermissionError:
             message = f"Insufficient permissions to delete {project_name}"
             _feedback(message, "warning")
```

### Comparing `pynball-1.5.5/src/pynball.egg-info/PKG-INFO` & `pynball-1.5.6/src/pynball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.5
+Version: 1.5.6
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynball-1.5.5/src/pynball.egg-info/SOURCES.txt` & `pynball-1.5.6/src/pynball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test__check_pyenv.py` & `pynball-1.5.6/tests/test__check_pyenv.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test__check_virtual_env.py` & `pynball-1.5.6/tests/test__check_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test__get_pynball.py` & `pynball-1.5.6/tests/test__get_pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test__message.py` & `pynball-1.5.6/tests/test__message.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test__set_get_del_env.py` & `pynball-1.5.6/tests/test__set_get_del_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_add.py` & `pynball-1.5.6/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_delete.py` & `pynball-1.5.6/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_lsproject.py` & `pynball-1.5.6/tests/test_lsproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_mkproject.py` & `pynball-1.5.6/tests/test_mkproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_rmproject.py` & `pynball-1.5.6/tests/test_rmproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.5/tests/test_versions.py` & `pynball-1.5.6/tests/test_versions.py`

 * *Files identical despite different names*

