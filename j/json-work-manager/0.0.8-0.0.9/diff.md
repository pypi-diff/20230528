# Comparing `tmp/json-work-manager-0.0.8.tar.gz` & `tmp/json-work-manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-work-manager-0.0.8.tar", last modified: Wed Mar 29 03:07:25 2023, max compression
+gzip compressed data, was "json-work-manager-0.0.9.tar", last modified: Thu Mar 30 00:15:59 2023, max compression
```

## Comparing `json-work-manager-0.0.8.tar` & `json-work-manager-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 03:07:25.688324 json-work-manager-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      698 2023-03-29 03:07:25.688324 json-work-manager-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 03:07:25.686324 json-work-manager-0.0.8/json_work_manager/
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21280 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager/json_work_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 03:07:25.688324 json-work-manager-0.0.8/json_work_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/json_work_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 03:07:25.688324 json-work-manager-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      603 2023-03-29 03:07:25.000000 json-work-manager-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:15:59.188009 json-work-manager-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-03-30 00:15:59.187009 json-work-manager-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:15:59.186009 json-work-manager-0.0.9/json_work_manager/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21295 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager/json_work_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21280 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager/json_work_manager_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 00:15:59.187009 json-work-manager-0.0.9/json_work_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/json_work_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 00:15:59.188009 json-work-manager-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      603 2023-03-30 00:15:58.000000 json-work-manager-0.0.9/setup.py
```

### Comparing `json-work-manager-0.0.8/PKG-INFO` & `json-work-manager-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-work-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Json work manager
 Home-page: https://github.com/automatethem/json-work-manager
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `json-work-manager-0.0.8/json_work_manager/json_work_manager.py` & `json-work-manager-0.0.9/json_work_manager/json_work_manager_old.py`

 * *Files identical despite different names*

### Comparing `json-work-manager-0.0.8/json_work_manager.egg-info/PKG-INFO` & `json-work-manager-0.0.9/json_work_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-work-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Json work manager
 Home-page: https://github.com/automatethem/json-work-manager
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `json-work-manager-0.0.8/setup.py` & `json-work-manager-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='json-work-manager',
-	version='0.0.8',
+	version='0.0.9',
 	description='Json work manager',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/json-work-manager',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

