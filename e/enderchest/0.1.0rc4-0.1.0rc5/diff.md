# Comparing `tmp/enderchest-0.1.0rc4.tar.gz` & `tmp/enderchest-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc4.tar", last modified: Sun May 28 01:15:14 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc5.tar", last modified: Sun May 28 17:37:25 2023, max compression
```

## Comparing `enderchest-0.1.0rc4.tar` & `enderchest-0.1.0rc5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.589811 enderchest-0.1.0rc4/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.589811 enderchest-0.1.0rc4/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.504461 enderchest-0.1.0rc5/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 17:37:25.504461 enderchest-0.1.0rc5/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/versioneer.py
```

### Comparing `enderchest-0.1.0rc4/LICENSE` & `enderchest-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/PKG-INFO` & `enderchest-0.1.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.0rc4/README.md` & `enderchest-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/cli.py` & `enderchest-0.1.0rc5/enderchest/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,31 +108,35 @@
         "register (or update the registry of) a remote EnderChest",
         _update_ender_chest,
     ),
     (
         # I freely admit this is ridiculous
         sum(
             (
-                (verb, *(f"{verb} {alias}" for alias in _instance_aliases))
+                (
+                    verb,
+                    *(
+                        f"{verb} {alias}"
+                        # pluralization is hard
+                        for alias in ("shulker_boxes", "shulkerboxes", "shulkers")
+                    ),
+                )
                 for verb in _list_aliases
             ),
             (),
         ),
-        "list the minecraft instances registered with your Enderchest",
-        gather.load_ender_chest_instances,
+        "list the shulker boxes inside your Enderchest",
+        gather.load_shulker_boxes,
     ),
     (
         tuple(
-            f"{verb} {alias}"
-            for verb in _list_aliases
-            # pluralization is hard
-            for alias in ("shulker_boxes", "shulkerboxes", "shulkers")
+            f"{verb} {alias}" for verb in _list_aliases for alias in _instance_aliases
         ),
-        "list the shulker boxes inside your Enderchest",
-        gather.load_shulker_boxes,
+        "list the minecraft instances registered with your Enderchest",
+        gather.load_ender_chest_instances,
     ),
     (
         tuple(
             f"{verb} {alias}" for verb in _list_aliases for alias in _shulker_aliases
         ),
         "list the instances that match the specified shulker box",
         _list_shulker_box,
```

### Comparing `enderchest-0.1.0rc4/enderchest/craft.py` & `enderchest-0.1.0rc5/enderchest/craft.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,19 @@
         if copy_from:
             try:
                 for remote, alias in fetch_remotes_from_a_remote_ender_chest(copy_from):
                     if alias == ender_chest.name:
                         continue  # don't register yourself!
                     ender_chest.register_remote(remote, alias)
             except (RuntimeError, ValueError) as fetch_fail:
-                CRAFT_LOGGER.warning(
+                CRAFT_LOGGER.error(
                     f"Could not fetch remotes from {copy_from}:\n  {fetch_fail}"
                 )
+                CRAFT_LOGGER.error("Aborting.")
+                return
 
         for extra_remote in remotes or ():
             if isinstance(extra_remote, (str, ParseResult)):
                 ender_chest.register_remote(extra_remote)
             else:
                 ender_chest.register_remote(*extra_remote)
 
@@ -531,16 +533,16 @@
         hosts = tuple(host.strip() for host in values.split(","))
 
         # TODO: DRY this into a dedicated function
 
         # TODO: stop wastefully reloading the cfg
         host = load_ender_chest(minecraft_root).name
 
-        if not any(
-            fnmatch.fnmatchcase(host.lower(), host_spec.lower()) for host_spec in hosts
+        if not shulker_box._replace(match_criteria=(("hosts", hosts),)).matches_host(
+            host
         ):
             CRAFT_LOGGER.warning(
                 "This shulker box will not link to any instances on this machine"
             )
             if not confirm(default=False):
                 continue
         break
```

### Comparing `enderchest-0.1.0rc4/enderchest/enderchest.py` & `enderchest-0.1.0rc5/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/filesystem.py` & `enderchest-0.1.0rc5/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/gather.py` & `enderchest-0.1.0rc5/enderchest/gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,26 +316,51 @@
         shulker_box = _load_shulker_box(config_file)
     except (FileNotFoundError, ValueError) as bad_box:
         GATHER_LOGGER.error(
             f"Could not load shulker box {shulker_box_name}\n  {bad_box}"
         )
         return ()
 
-    instances = load_ender_chest_instances(minecraft_root, log_level=logging.DEBUG)
-    if not instances:
-        return instances
+    chest = load_ender_chest(minecraft_root)
+
+    if not shulker_box.matches_host(chest.name):
+        GATHER_LOGGER.warning(
+            "This shulker box will not link to any instances on this machine"
+        )
+        return ()
+
+    if not chest.instances:
+        GATHER_LOGGER.warning(
+            "This EnderChest does not have any instances registered."
+            " To register some, run the command:"
+            "\nenderchest gather minecraft",
+        )
+        return ()
+
+    GATHER_LOGGER.debug(
+        "These are the instances that are currently registered"
+        f" to the {minecraft_root} EnderChest:\n"
+        + "\n".join(
+            [
+                f"  {i + 1}. {_render_instance(instance)}"
+                for i, instance in enumerate(chest.instances)
+            ]
+        ),
+    )
 
     if shulker_box is None:
         return ()
-    matches = [instance for instance in instances if shulker_box.matches(instance)]
+    matches = [
+        instance for instance in chest.instances if shulker_box.matches(instance)
+    ]
 
     if len(matches) == 0:
         report = "does not link to by any registered instances"
     else:
-        report = "is linked to by the following instancs:\n" + "\n".join(
+        report = "is linked to by the following instances:\n" + "\n".join(
             f"  - {_render_instance(instance)}" for instance in matches
         )
 
     GATHER_LOGGER.info(f"The shulker box {_render_shulker_box(shulker_box)} {report}")
 
     return matches
```

### Comparing `enderchest-0.1.0rc4/enderchest/instance.py` & `enderchest-0.1.0rc5/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/loggers.py` & `enderchest-0.1.0rc5/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/place.py` & `enderchest-0.1.0rc5/enderchest/place.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Symlinking functionality"""
-import fnmatch
 import itertools
 import logging
 import os
 from pathlib import Path
 from typing import Iterable
 
 from . import filesystem as fs
@@ -59,26 +58,19 @@
         return
 
     instances = load_ender_chest_instances(minecraft_root, log_level=logging.DEBUG)
 
     shulker_boxes: list[ShulkerBox] = []
 
     for shulker_box in load_shulker_boxes(minecraft_root, log_level=logging.DEBUG):
-        for condition, values in shulker_box.match_criteria:
-            if condition == "hosts":
-                # TODO: DRY this into a dedicated function
-                if not any(
-                    fnmatch.fnmatchcase(host.lower(), host_spec.lower())
-                    for host_spec in values
-                ):
-                    PLACE_LOGGER.debug(
-                        f"{shulker_box.name} is not intended"
-                        f" for linking to this host ({host})"
-                    )
-                    break
+        if not shulker_box.matches_host(host):
+            PLACE_LOGGER.debug(
+                f"{shulker_box.name} is not intended for linking to this host ({host})"
+            )
+            break
         else:
             shulker_boxes.append(shulker_box)
 
     skip_instances: list[InstanceSpec] = []
 
     def handle_error(instance: InstanceSpec) -> str:
         """Centralized error-handling
@@ -99,15 +91,15 @@
         """
         if error_handling == "prompt":
             proceed_how = (
                 prompt(
                     "How would you like to proceed?"
                     "\n[Q]uit, [C]ontinue, abort linking the rest of this shulker/instance [M]atch?"
                     "\nskip the rest of this [I]nstance, skip the rest of this [S]hulker box?",
-                    suggestion="I",  # TODO: in my experience it's usally an instance issue
+                    suggestion="I",  # TODO: reevaluate default (it's 50/50 due to link folders)
                 )
                 .lower()
                 .replace(" ", "")
                 .replace("-", "")
                 .replace("_", "")
             )
             match proceed_how:
@@ -213,15 +205,14 @@
                     except (OSError, NotADirectoryError) as oh_no:
                         PLACE_LOGGER.error(
                             f"Error linking shulker box {shulker_box.name}"
                             f" to instance {instance.name}:"
                             f"\n  {(instance.root / resource_path)}"
                             " already exists"
                         )
-                        # TODO: option to record failure but keep going
                         match handle_error(instance):
                             case "return":
                                 return
                             case "break":
                                 match_exit = "break"
                                 break
                             case "continue":
```

### Comparing `enderchest-0.1.0rc4/enderchest/prompt.py` & `enderchest-0.1.0rc5/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/remote.py` & `enderchest-0.1.0rc5/enderchest/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
     Raises
     ------
     RuntimeError
         If the remote list could not be pulled
     """
     remote_chest = load_remote_ender_chest(uri)
-    remotes: list[tuple[ParseResult, str]] = [(remote_chest._uri, remote_chest.name)]
+    remotes: list[tuple[ParseResult, str]] = [
+        (urlparse(uri) if isinstance(uri, str) else uri, remote_chest.name)
+    ]
 
     remotes.extend(remote_chest.remotes)
     SYNC_LOGGER.info(
         "Loaded the following remotes:\n"
         + "\n".join(f"  - {render_remote(alias, uri)}" for uri, alias in remotes)
     )
 
@@ -154,15 +156,15 @@
     for remote_uri, alias in remotes:
         if dry_run:
             runs: tuple[bool, ...] = (True,)
         elif sync_confirm_wait is False or sync_confirm_wait <= 0:
             runs = (False,)
         else:
             runs = (True, False)
-        for run_type in runs:
+        for do_dry_run in runs:
             try:
                 if pull_or_push == "pull":
                     SYNC_LOGGER.info(
                         "Attempting to pull changes from"
                         f" {render_remote(alias, remote_uri)}"
                     )
                     remote_chest = remote_uri._replace(
@@ -181,15 +183,15 @@
                         exclude=[
                             os.path.join(
                                 fs.ENDER_CHEST_FOLDER_NAME, fs.ENDER_CHEST_CONFIG_NAME
                             ),
                             os.path.join(fs.ENDER_CHEST_FOLDER_NAME, ".*"),
                             *(sync_kwargs.pop("exclude", None) or ()),
                         ],
-                        dry_run=run_type,
+                        dry_run=do_dry_run,
                         **sync_kwargs,
                     )
                 else:
                     SYNC_LOGGER.info(
                         f"Attempting to push changes to {render_remote(alias, remote_uri)}"
                     )
                     local_chest = fs.ender_chest_folder(minecraft_root)
@@ -199,29 +201,29 @@
                         exclude=[
                             os.path.join(
                                 fs.ENDER_CHEST_FOLDER_NAME, fs.ENDER_CHEST_CONFIG_NAME
                             ),
                             os.path.join(fs.ENDER_CHEST_FOLDER_NAME, ".*"),
                             *(sync_kwargs.pop("exclude", None) or ()),
                         ],
-                        dry_run=run_type,
+                        dry_run=do_dry_run,
                         **sync_kwargs,
                     )
             except (
                 FileNotFoundError,
                 ValueError,
                 NotImplementedError,
                 TimeoutError,
             ) as sync_fail:
                 SYNC_LOGGER.warning(
                     f"Could not sync changes with {render_remote(alias, remote_uri)}:"
                     f"\n  {sync_fail}"
                 )
                 break
-            if sync_confirm_wait is False:
+            if do_dry_run == runs[-1]:
                 continue
             if sync_confirm_wait is True:
                 if not confirm(default=True):
                     SYNC_LOGGER.error("Aborting")
                     return
             else:
                 SYNC_LOGGER.debug(f"Waiting for {sync_confirm_wait} seconds")
```

### Comparing `enderchest-0.1.0rc4/enderchest/shulker_box.py` & `enderchest-0.1.0rc5/enderchest/shulker_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,15 +256,32 @@
                 case "hosts":
                     # this is handled at a higher level
                     pass
                 case _:
                     raise NotImplementedError(
                         f"Don't know how to apply match condition {condition}."
                     )
+        return True
+
+    def matches_host(self, hostname: str):
+        """Determine whether the shulker box should be linked to from the
+        current host machine
 
+        Returns
+        -------
+        bool
+            True if the shulker box's hosts spec matches the host, False otherwise.
+        """
+        for condition, values in self.match_criteria:
+            if condition == "hosts":
+                if not any(
+                    fnmatch.fnmatchcase(hostname.lower(), host_spec.lower())
+                    for host_spec in values
+                ):
+                    return False
         return True
 
 
 def _normalize_modloader(loader: str | None) -> list[str]:
     """Implement common modloader aliases
 
     Parameters
```

### Comparing `enderchest-0.1.0rc4/enderchest/sync/__init__.py` & `enderchest-0.1.0rc5/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/sync/file.py` & `enderchest-0.1.0rc5/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/sync/rsync.py` & `enderchest-0.1.0rc5/enderchest/sync/rsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,12 +274,12 @@
         The URI to convert
 
     Returns
     -------
     str
         The SSH-format address
     """
-    return "{user}@{host}:{path}".format(
-        user=uri.username,
+    return "{user}{host}:{path}".format(
+        user=f"{uri.username}@" if uri.username else "",
         host=(uri.hostname or "localhost") + (f":{uri.port}" if uri.port else ""),
         path=path_from_uri(uri).as_posix(),
     )
```

### Comparing `enderchest-0.1.0rc4/enderchest/test/conftest.py` & `enderchest-0.1.0rc5/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_cli.py` & `enderchest-0.1.0rc5/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_craft.py` & `enderchest-0.1.0rc5/enderchest/test/test_craft.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,27 +129,52 @@
             raise AssertionError("I was not to be called.")
 
         create_log: list[tuple[Path, Any]] = []
 
         def mock_create(root, chest) -> None:
             create_log.append((root, chest))
 
-        def mock_gather(*args, **kwargs) -> list[Any]:
+        def mock_gather(*args, **kwargs) -> list:
             return []
 
+        def mock_fetch_remotes(*args, **kwargs) -> list:
+            raise AssertionError("I was not to be called.")
+
         monkeypatch.setattr(craft, "specify_ender_chest_from_prompt", mock_prompt)
         monkeypatch.setattr(craft, "create_ender_chest", mock_create)
         monkeypatch.setattr(craft, "gather_minecraft_instances", mock_gather)
         monkeypatch.setattr(
-            craft, "fetch_remotes_from_a_remote_ender_chest", mock_gather
+            craft, "fetch_remotes_from_a_remote_ender_chest", mock_fetch_remotes
         )
 
         craft.craft_ender_chest(minecraft_root, **{argument: value})
         assert len(create_log) == 1
 
+    def test_failed_fetch_aborts_the_create(self, monkeypatch, minecraft_root):
+        def mock_prompt(root) -> Any:
+            raise AssertionError("I was not to be called.")
+
+        def mock_create(root, chest) -> None:
+            raise AssertionError("I was not to be called.")
+
+        def mock_gather(*args, **kwargs) -> list:
+            return []
+
+        def mock_fetch_remotes(*args, **kwargs) -> list:
+            raise RuntimeError("Don't feel like it.")
+
+        monkeypatch.setattr(craft, "specify_ender_chest_from_prompt", mock_prompt)
+        monkeypatch.setattr(craft, "create_ender_chest", mock_create)
+        monkeypatch.setattr(craft, "gather_minecraft_instances", mock_gather)
+        monkeypatch.setattr(
+            craft, "fetch_remotes_from_a_remote_ender_chest", mock_fetch_remotes
+        )
+
+        craft.craft_ender_chest(minecraft_root, copy_from="prayer://unreachable")
+
     def test_default_behavior_is_to_prevent_overwrite(self, minecraft_root, caplog):
         create_ender_chest(
             minecraft_root,
             EnderChest(
                 "openbagtwo@battlestation" + minecraft_root.absolute().as_posix()
             ),
         )
```

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_gather.py` & `enderchest-0.1.0rc5/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_instance.py` & `enderchest-0.1.0rc5/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_place.py` & `enderchest-0.1.0rc5/enderchest/test/test_place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/test_sync.py` & `enderchest-0.1.0rc5/enderchest/test/test_sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,48 @@
 
 class TestPathFromURI:
     def test_roundtrip(self, tmpdir):
         original_path = Path(tmpdir) / "this has a space in it" / "(="
         assert path_from_uri(urlparse(original_path.as_uri())) == original_path
 
 
+@pytest.mark.xfail(
+    not shutil.which("rsync"), reason="rsync is not installed on this system"
+)  # TODO: remove xfail once this method has been moved to a different module
+class TestURIToSSH:
+    @pytest.fixture(scope="class")
+    def rsync_module(self):
+        from enderchest.sync import rsync
+
+        yield rsync
+
+    def test_simple_parse(self, rsync_module):
+        address = rsync_module.uri_to_ssh(
+            urlparse("rsync://openbagtwo@couchgaming:22/home/openbagtwo/minecraft")
+        )
+        assert address == "openbagtwo@couchgaming:22:/home/openbagtwo/minecraft"
+
+    def test_no_username_parse(self, rsync_module):
+        address = rsync_module.uri_to_ssh(
+            urlparse("rsync://steamdeck/home/openbagtwo/minecraft")
+        )
+        assert address == "steamdeck:/home/openbagtwo/minecraft"
+
+    def test_no_netloc_parse(self, rsync_module):
+        address = rsync_module.uri_to_ssh(
+            urlparse("rsync:///mnt/external/minecraft-bkp")
+        )
+        assert address == "localhost:/mnt/external/minecraft-bkp"
+
+    def test_no_hostname_parse(self, rsync_module):
+        """Can't believe this is a valid URI"""
+        address = rsync_module.uri_to_ssh(urlparse("rsync://nugget@/home/nugget/"))
+        assert address == "nugget@localhost:/home/nugget"
+
+
 class TestFileIgnorePatternBuilder:
     def test_simple_match(self):
         assert file.ignore_patterns("hello")(
             "greetings", ("bonjour", "hello", "hellooooo")
         ) == {"hello"}
 
     def test_wildcard(self):
@@ -170,20 +204,22 @@
                 minecraft_root / "worlds" / "olam",
             ),
         ):
             path.unlink(missing_ok=True)
             path.symlink_to(target, target_is_directory=target.is_dir())
 
     def test_create_from_remote_chest(self, remote, minecraft_root):
-        craft.craft_ender_chest(minecraft_root, copy_from=remote, overwrite=True)
+        craft.craft_ender_chest(
+            minecraft_root, copy_from=remote.geturl(), overwrite=True
+        )
 
-        assert [
-            (alias, remote.scheme)
-            for remote, alias in gather.load_ender_chest_remotes(minecraft_root)
-        ] == [("closer than you think", self.protocol), ("birdhouse", "ipoac")]
+        assert gather.load_ender_chest_remotes(minecraft_root) == [
+            (remote, "closer than you think"),
+            (urlparse("ipoac://yoursoul@birdhouse/minecraft"), "birdhouse"),
+        ]
 
     def test_open_grabs_files_from_upstream(self, minecraft_root, remote):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
         r.sync_with_remotes(minecraft_root, "pull")
         assert (
             minecraft_root / "EnderChest" / "optifine" / "mods" / "optifine.jar"
         ).read_text() == "it's okay"
```

### Comparing `enderchest-0.1.0rc4/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc5/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc5/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest/test/utils.py` & `enderchest-0.1.0rc5/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc5/enderchest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.0rc4/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc5/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/setup.py` & `enderchest-0.1.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc4/versioneer.py` & `enderchest-0.1.0rc5/versioneer.py`

 * *Files identical despite different names*

