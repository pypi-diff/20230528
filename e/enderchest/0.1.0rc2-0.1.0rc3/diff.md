# Comparing `tmp/enderchest-0.1.0rc2.tar.gz` & `tmp/enderchest-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc2.tar", last modified: Sat May 27 18:51:41 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc3.tar", last modified: Sat May 27 23:52:54 2023, max compression
```

## Comparing `enderchest-0.1.0rc2.tar` & `enderchest-0.1.0rc3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31131 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.476633 enderchest-0.1.0rc3/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/versioneer.py
```

### Comparing `enderchest-0.1.0rc2/LICENSE` & `enderchest-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/PKG-INFO` & `enderchest-0.1.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -35,15 +35,15 @@
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
 ## Installation
 
-EnderChest is written for **Python 3.11 or greater,** but should otherwise
+EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
```

### Comparing `enderchest-0.1.0rc2/README.md` & `enderchest-0.1.0rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
 ## Installation
 
-EnderChest is written for **Python 3.11 or greater,** but should otherwise
+EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
```

### Comparing `enderchest-0.1.0rc2/enderchest/cli.py` & `enderchest-0.1.0rc3/enderchest/cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/craft.py` & `enderchest-0.1.0rc3/enderchest/craft.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,27 +518,27 @@
         _ = load_ender_chest_remotes(minecraft_root)  # to display some log messages
         values = (
             prompt(
                 (
                     "What hosts (EnderChest installations) should use this shulker box?"
                     "\nProvide a comma-separated list (wildcards are allowed)"
                     "\nand remember to include the name of this EnderChest"
-                    f'("{load_ender_chest(minecraft_root).name}")'
+                    f' ("{load_ender_chest(minecraft_root).name}")'
                 ),
                 suggestion="*",
             )
             or "*"
         )
         hosts = tuple(host.strip() for host in values.split(","))
 
         # TODO: DRY this into a dedicated function
 
         # TODO: stop wastefully reloading the cfg
         host = load_ender_chest(minecraft_root).name
-        print(hosts, host)
+
         if not any(
             fnmatch.fnmatchcase(host.lower(), host_spec.lower()) for host_spec in hosts
         ):
             CRAFT_LOGGER.warning(
                 "This shulker box will not link to any instances on this machine"
             )
             if not confirm(default=False):
```

### Comparing `enderchest-0.1.0rc2/enderchest/enderchest.py` & `enderchest-0.1.0rc3/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/filesystem.py` & `enderchest-0.1.0rc3/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/gather.py` & `enderchest-0.1.0rc3/enderchest/gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     else:
         GATHER_LOGGER.log(
             log_level,
             "These are the instances that are currently registered"
             f" to the {minecraft_root} EnderChest:\n"
             + "\n".join(
                 [
-                    f"  {i + 1}. {_render_instance(instance)})"
+                    f"  {i + 1}. {_render_instance(instance)}"
                     for i, instance in enumerate(instances)
                 ]
             ),
         )
     return instances
```

### Comparing `enderchest-0.1.0rc2/enderchest/instance.py` & `enderchest-0.1.0rc3/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/loggers.py` & `enderchest-0.1.0rc3/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/place.py` & `enderchest-0.1.0rc3/enderchest/place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/prompt.py` & `enderchest-0.1.0rc3/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/remote.py` & `enderchest-0.1.0rc3/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/shulker_box.py` & `enderchest-0.1.0rc3/enderchest/shulker_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     This method *does not* match snapshots to their corresponding version
     range--for that you're just going to have to be explicit.
     """
     try:
         return semver.SimpleSpec(version_spec).match(semver.Version(version_string))
     except ValueError:
         # fall back to simple fnmatching
-        return fnmatch.fnmatchcase(version_spec.lower(), version_string.lower())
+        return fnmatch.fnmatchcase(version_string.lower(), version_spec.lower())
 
 
 DEFAULT_SHULKER_FOLDERS = (  # TODO: customize in enderchest.cfg
     "config",
     "mods",
     "resourcepacks",
     "saves",
```

### Comparing `enderchest-0.1.0rc2/enderchest/sync/__init__.py` & `enderchest-0.1.0rc3/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/sync/file.py` & `enderchest-0.1.0rc3/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/sync/rsync.py` & `enderchest-0.1.0rc3/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/conftest.py` & `enderchest-0.1.0rc3/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_cli.py` & `enderchest-0.1.0rc3/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_craft.py` & `enderchest-0.1.0rc3/enderchest/test/test_craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_gather.py` & `enderchest-0.1.0rc3/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_instance.py` & `enderchest-0.1.0rc3/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_place.py` & `enderchest-0.1.0rc3/enderchest/test/test_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import pytest
 
 from enderchest import ShulkerBox
 from enderchest import filesystem as fs
 from enderchest import place
+from enderchest import shulker_box as sb
 
 from . import utils
 
 
 class TestRglob:
     def test_max_depth_of_one_is_equivalent_to_a_plain_glob(self, minecraft_root):
         glob = sorted(minecraft_root.iterdir())
@@ -252,14 +253,42 @@
 
         # also make sure the original file is okay
         assert (
             original_target.read_text() == "I will trade you these\nfor less of these\n"
         )
 
 
+class TestMatchesVersion:
+    @pytest.mark.parametrize(
+        "version", ("1.19.4", "1.20-pre6", "23w13a_or_b", "not even trying")
+    )
+    def test_simple_equality_checks(self, version):
+        assert sb._matches_version(version, version)
+
+    @pytest.mark.parametrize(
+        "version_spec",
+        ("1.19", "1.19.*", ">=1.19.0,<1.20"),
+        ids=("minor-version", "wildcard", "bounding"),
+    )
+    def test_version_bounding(self, version_spec):
+        assert sb._matches_version(version_spec, "1.19.4")
+
+    @pytest.mark.parametrize(
+        "version", ("1.19.4", "1.20-pre6", "23w13a_or_b", "not even trying")
+    )
+    def test_star_matches_anything(self, version):
+        assert sb._matches_version("*", version)
+
+    @pytest.mark.parametrize(
+        "version", ("1.20-pre1", "1.20-rc1", "1.20.3-pre16", "1.20-forge")
+    )
+    def test_prereleases_etc_align_with_their_wildcarded_versions(self, version):
+        assert sb._matches_version("1.20*", version)
+
+
 class TestShulkerInstanceMatching:
     @staticmethod
     def matchall(shulker: ShulkerBox) -> list[str]:
         """Return the names of the testing instances that match the
         provided shulker
 
         Parameters
```

### Comparing `enderchest-0.1.0rc2/enderchest/test/test_sync.py` & `enderchest-0.1.0rc3/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc3/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc3/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest/test/utils.py` & `enderchest-0.1.0rc3/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc3/enderchest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -35,15 +35,15 @@
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
 ## Installation
 
-EnderChest is written for **Python 3.11 or greater,** but should otherwise
+EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
 
 ```bash
 $ python -m pip install --user enderchest
 ```
```

### Comparing `enderchest-0.1.0rc2/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc3/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/setup.py` & `enderchest-0.1.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc2/versioneer.py` & `enderchest-0.1.0rc3/versioneer.py`

 * *Files identical despite different names*

