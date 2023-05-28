# Comparing `tmp/enderchest-0.1.0rc3.tar.gz` & `tmp/enderchest-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc3.tar", last modified: Sat May 27 23:52:54 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc4.tar", last modified: Sun May 28 01:15:14 2023, max compression
```

## Comparing `enderchest-0.1.0rc3.tar` & `enderchest-0.1.0rc4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:52:54.476633 enderchest-0.1.0rc3/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 23:52:54.000000 enderchest-0.1.0rc3/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 23:52:54.480633 enderchest-0.1.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-27 23:52:46.000000 enderchest-0.1.0rc3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31106 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.589811 enderchest-0.1.0rc4/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:15:14.589811 enderchest-0.1.0rc4/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 01:15:14.000000 enderchest-0.1.0rc4/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-28 01:15:14.593811 enderchest-0.1.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-28 01:15:04.000000 enderchest-0.1.0rc4/versioneer.py
```

### Comparing `enderchest-0.1.0rc3/LICENSE` & `enderchest-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/PKG-INFO` & `enderchest-0.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.0rc3/README.md` & `enderchest-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/cli.py` & `enderchest-0.1.0rc4/enderchest/cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/craft.py` & `enderchest-0.1.0rc4/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/enderchest.py` & `enderchest-0.1.0rc4/enderchest/enderchest.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         """
         parser = ConfigParser(
             allow_no_value=True,
             delimiters=("=",),
             inline_comment_prefixes=(";",),
             interpolation=None,
         )
+        parser.optionxform = str  # type: ignore
         try:
             assert parser.read(config_file)
         except ParsingError as bad_cfg:
             raise ValueError(f"Could not parse {config_file}") from bad_cfg
         except AssertionError:
             raise FileNotFoundError(f"Could not open {config_file}")
 
@@ -294,14 +295,15 @@
             An INI-syntax rendering of this EnderChest's config
 
         Notes
         -----
         The "root" attribute is ignored for this method
         """
         config = ConfigParser(allow_no_value=True, interpolation=None)
+        config.optionxform = str  # type: ignore
         config.add_section("properties")
         config.set("properties", "name", self.name)
         config.set("properties", "address", self._uri.netloc)
         config.set("properties", "sync-protocol", self._uri.scheme)
         config.set(
             "properties",
             "sync-confirmation-time",
```

### Comparing `enderchest-0.1.0rc3/enderchest/filesystem.py` & `enderchest-0.1.0rc4/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/gather.py` & `enderchest-0.1.0rc4/enderchest/gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable, Sequence
 from urllib.parse import ParseResult
 
 from enderchest.sync import render_remote
 
 from . import filesystem as fs
 from .enderchest import EnderChest, create_ender_chest
-from .instance import InstanceSpec
+from .instance import InstanceSpec, _parse_version
 from .loggers import GATHER_LOGGER
 from .shulker_box import ShulkerBox
 
 
 def load_ender_chest(minecraft_root: Path) -> EnderChest:
     """Load the configuration from the enderchest.cfg file in the EnderChest
     folder.
@@ -488,18 +488,18 @@
 
     versions: list[str] = []
     tags: list[str] = ["vanilla"]
     for version in raw_versions:
         if version.startswith("latest-"):
             mapped_version = version_lookup.get(version[len("latest-") :])
             if mapped_version is not None:
-                versions.append(mapped_version)
+                versions.append(_parse_version(mapped_version))
                 tags.append(version)
                 continue
-        versions.append(version)
+        versions.append(_parse_version(version))
 
     return InstanceSpec(name, minecraft_folder, tuple(versions), None, tuple(tags))
 
 
 def gather_metadata_for_mmc_instance(
     minecraft_folder: Path, instgroups_file: Path | None = None
 ) -> InstanceSpec:
@@ -535,15 +535,15 @@
 
         version: str | None = None
         modloader: str | None = None
 
         for component in components:
             match component.get("uid"), component.get("cachedName", ""):
                 case "net.minecraft", _:
-                    version = component["version"]
+                    version = _parse_version(component["version"])
                 case "net.fabricmc.fabric-loader", _:
                     modloader = "Fabric Loader"
                 case "org.quiltmc.quilt-loader", _:
                     modloader = "Quilt Loader"
                 case ("net.minecraftforge", _) | (_, "Forge"):
                     modloader = "Forge"
                 case _, name if name.endswith("oader"):
```

### Comparing `enderchest-0.1.0rc3/enderchest/instance.py` & `enderchest-0.1.0rc4/enderchest/instance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Specification of a Minecraft instance"""
+import re
 from configparser import SectionProxy
 from pathlib import Path
 from typing import NamedTuple
 
 
 class InstanceSpec(NamedTuple):
     """Specification of a Minecraft instance
@@ -50,15 +51,18 @@
             If a required key is absent
         ValueError
             If a required entry cannot be parsed
         """
         return cls(
             section.name,
             Path(section["root"]),
-            tuple(section["minecraft_version"].strip().split()),
+            tuple(
+                _parse_version(version.strip())
+                for version in section["minecraft_version"].strip().split()
+            ),
             section.get("modloader", None),
             tuple(
                 tag.strip()
                 for tag in section.get("tags", "")
                 .replace(",", "\n")
                 .strip()
                 .split("\n")
@@ -85,7 +89,32 @@
     bool
         True if and only if the two instances have the same root, with regards
         to the provided `minecraft_root`
     """
     path = minecraft_root / instance.root.expanduser()
     other_path = minecraft_root / other_instance.root.expanduser()
     return path.expanduser().resolve() == other_path.expanduser().resolve()
+
+
+def _parse_version(version_string: str) -> str:
+    """The first release of each major Minecraft version doesn't follow strict
+    major.minor.patch semver. This method appends the ".0" so that our version
+    matcher doesn't mess up
+
+    Parameters
+    ----------
+    version_string : str
+        The version read in from the Minecraft instance's config
+
+    Returns
+    -------
+    str
+        Either the original version string or the original version string with
+        ".0" tacked onto the end of it
+
+    Notes
+    -----
+    Regex adapted straight from https://semver.org
+    """
+    if re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)$", version_string):
+        return version_string + ".0"
+    return version_string
```

### Comparing `enderchest-0.1.0rc3/enderchest/loggers.py` & `enderchest-0.1.0rc4/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/place.py` & `enderchest-0.1.0rc4/enderchest/place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/prompt.py` & `enderchest-0.1.0rc4/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/remote.py` & `enderchest-0.1.0rc4/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/shulker_box.py` & `enderchest-0.1.0rc4/enderchest/shulker_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         priority = 0
         max_link_depth = 2
         root = config_file.parent
         name = root.name
         parser = ConfigParser(
             allow_no_value=True, inline_comment_prefixes=(";",), interpolation=None
         )
+        parser.optionxform = str  # type: ignore
         try:
             assert parser.read(config_file)
         except ParsingError as bad_cfg:
             raise ValueError(f"Could not parse {config_file}") from bad_cfg
         except AssertionError:
             raise FileNotFoundError(f"Could not open {config_file}")
 
@@ -163,14 +164,15 @@
             An INI-syntax rendering of this shulker box's config
 
         Notes
         -----
         The "root" attribute is ignored for this method
         """
         config = ConfigParser(allow_no_value=True, interpolation=None)
+        config.optionxform = str  # type: ignore
         config.add_section("properties")
         config.set("properties", "priority", str(self.priority))
         if self.max_link_depth != 2:
             config.set("properties", "max-link-depth", str(self.max_link_depth))
         config.set("properties", "last_modified", dt.datetime.now().isoformat(sep=" "))
         config.set(
             "properties", "generated_by_enderchest_version", get_versions()["version"]
```

### Comparing `enderchest-0.1.0rc3/enderchest/sync/__init__.py` & `enderchest-0.1.0rc4/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/sync/file.py` & `enderchest-0.1.0rc4/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/sync/rsync.py` & `enderchest-0.1.0rc4/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/conftest.py` & `enderchest-0.1.0rc4/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_cli.py` & `enderchest-0.1.0rc4/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_craft.py` & `enderchest-0.1.0rc4/enderchest/test/test_craft.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             3,
             "original",
             minecraft_root / "EnderChest" / "original",
             match_criteria=(
                 ("minecraft", (">=1.12,<2.0",)),
                 ("modloader", ("*",)),
                 ("tags", ("aether", "optifine")),
-                ("instances", ("aether legacy", "paradise lost")),
+                ("instances", ("aether legacy", "Paradise Lost")),
             ),
             link_folders=("screenshots", "logs"),
         )
 
         utils.pre_populate_enderchest(minecraft_root / "EnderChest")
 
         create_shulker_box(minecraft_root, original_shulker)
```

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_gather.py` & `enderchest-0.1.0rc4/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_instance.py` & `enderchest-0.1.0rc4/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_place.py` & `enderchest-0.1.0rc4/enderchest/test/test_place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/test_sync.py` & `enderchest-0.1.0rc4/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc4/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc4/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/enderchest/test/utils.py` & `enderchest-0.1.0rc4/enderchest/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         The folder where the pack file should be generated (the parent of
         the .minecraft folder)
     minecraft_version : str
         The minecraft version
     loader : str | None
         The loader (None if it's a vanilla instance)
     """
+    if minecraft_version.endswith(".0"):
+        # learned the hard way that mmc-pack files don't have use ".0"
+        minecraft_version = minecraft_version[:-2]
 
     components: list[dict[str, str]] = [
         {
             "cachedName": "Minecraft",
             "cachedRequires": "dontreadme",
             "cachedVersion": "dontreadme",
             "important": "dontreadme",
```

### Comparing `enderchest-0.1.0rc3/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc4/enderchest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.0rc3/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc4/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/setup.py` & `enderchest-0.1.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc3/versioneer.py` & `enderchest-0.1.0rc4/versioneer.py`

 * *Files identical despite different names*

