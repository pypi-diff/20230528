# Comparing `tmp/ansible-galaxy-local-deps-0.3.0.tar.gz` & `tmp/ansible-galaxy-local-deps-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-galaxy-local-deps-0.3.0.tar", last modified: Sun Mar 26 01:37:27 2023, max compression
+gzip compressed data, was "ansible-galaxy-local-deps-0.3.1.tar", last modified: Sun May 28 05:04:10 2023, max compression
```

## Comparing `ansible-galaxy-local-deps-0.3.0.tar` & `ansible-galaxy-local-deps-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 01:37:27.000000 ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/addos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/changedep.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/dropos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/gendottravis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/gengithubactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/installdeps.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/loggingsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/slurp.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/writedeps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 01:37:27.457271 ansible-galaxy-local-deps-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/tests/test_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-26 01:37:15.000000 ansible-galaxy-local-deps-0.3.0/tests/test_gendottravis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:04:10.242808 ansible-galaxy-local-deps-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-28 05:04:10.242808 ansible-galaxy-local-deps-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 05:04:10.242808 ansible-galaxy-local-deps-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:04:10.234808 ansible-galaxy-local-deps-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:04:10.238808 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 05:04:10.000000 ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:04:10.242808 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/addos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/changedep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/dropos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/gendottravis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/gengithubactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/installdeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/loggingsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/slurp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/writedeps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:04:10.242808 ansible-galaxy-local-deps-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/tests/test_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-28 05:03:52.000000 ansible-galaxy-local-deps-0.3.1/tests/test_gendottravis.py
```

### Comparing `ansible-galaxy-local-deps-0.3.0/LICENSE` & `ansible-galaxy-local-deps-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/PKG-INFO` & `ansible-galaxy-local-deps-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-galaxy-local-deps
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI for interacting with Ansible roles and their CIs
 Home-page: http://github.com/andrewrothstein/ansible-galaxy-local-deps
 Author: Andrew Rothstein
 Author-email: andrew.rothstein@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ansible-galaxy-local-deps-0.3.0/setup.py` & `ansible-galaxy-local-deps-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='ansible-galaxy-local-deps',
-      version='0.3.0',
+      version='0.3.1',
       description='CLI for interacting with Ansible roles and their CIs',
       url='http://github.com/andrewrothstein/ansible-galaxy-local-deps',
       author='Andrew Rothstein',
       author_email='andrew.rothstein@gmail.com',
       license='MIT',
       packages=find_packages('src'),
       package_dir={'': 'src'},
```

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/PKG-INFO` & `ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-galaxy-local-deps
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI for interacting with Ansible roles and their CIs
 Home-page: http://github.com/andrewrothstein/ansible-galaxy-local-deps
 Author: Andrew Rothstein
 Author-email: andrew.rothstein@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansible_galaxy_local_deps.egg-info/SOURCES.txt` & `ansible-galaxy-local-deps-0.3.1/src/ansible_galaxy_local_deps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/addos.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/addos.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/changedep.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/changedep.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/deps.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/deps.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/dropos.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/dropos.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/dump.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/dump.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/finder.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/gendottravis.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/gendottravis.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/gengithubactions.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/gengithubactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     },
                     {
                         'name': 'task ver',
                         'run': 'task --version'
                     },
                     {
                         'name': 'download task mono',
-                        'uses': 'actions/checkout@v2',
+                        'uses': 'actions/checkout@v3',
                         'with': {
                             'repository': 'andrewrothstein/tasks',
                             'ref': 'develop',
                             'path': 'taskmono'
                         }
                     }
                 ] + steps
```

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/installdeps.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/installdeps.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/slurp.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/slurp.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/src/ansiblegalaxylocaldeps/writedeps.py` & `ansible-galaxy-local-deps-0.3.1/src/ansiblegalaxylocaldeps/writedeps.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/tests/test_deps.py` & `ansible-galaxy-local-deps-0.3.1/tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `ansible-galaxy-local-deps-0.3.0/tests/test_gendottravis.py` & `ansible-galaxy-local-deps-0.3.1/tests/test_gendottravis.py`

 * *Files identical despite different names*

