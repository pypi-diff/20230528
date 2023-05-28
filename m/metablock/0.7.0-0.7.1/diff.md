# Comparing `tmp/metablock-0.7.0.tar.gz` & `tmp/metablock-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metablock-0.7.0.tar", max compression
+gzip compressed data, was "metablock-0.7.1.tar", max compression
```

## Comparing `metablock-0.7.0.tar` & `metablock-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1482 2023-05-27 10:27:29.751370 metablock-0.7.0/LICENSE
--rw-r--r--   0        0        0      502 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/cli.py
--rw-r--r--   0        0        0     5001 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/client.py
--rw-r--r--   0        0        0     6718 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/components.py
--rw-r--r--   0        0        0      542 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/extensions.py
--rw-r--r--   0        0        0     1912 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/orgs.py
--rw-r--r--   0        0        0        0 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/py.typed
--rw-r--r--   0        0        0     3220 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/spaces.py
--rw-r--r--   0        0        0     1486 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/user.py
--rw-r--r--   0        0        0      338 2023-05-27 10:27:29.751370 metablock-0.7.0/metablock/utils.py
--rw-r--r--   0        0        0      953 2023-05-27 10:27:29.751370 metablock-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1118 2023-05-27 10:27:29.751370 metablock-0.7.0/readme.md
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 metablock-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-05-28 14:27:26.005277 metablock-0.7.1/LICENSE
+-rw-r--r--   0        0        0      502 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/cli.py
+-rw-r--r--   0        0        0     5001 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/client.py
+-rw-r--r--   0        0        0     6704 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/components.py
+-rw-r--r--   0        0        0      542 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/extensions.py
+-rw-r--r--   0        0        0     1912 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/orgs.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/py.typed
+-rw-r--r--   0        0        0     3266 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/spaces.py
+-rw-r--r--   0        0        0     1486 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/user.py
+-rw-r--r--   0        0        0      338 2023-05-28 14:27:26.005277 metablock-0.7.1/metablock/utils.py
+-rw-r--r--   0        0        0      953 2023-05-28 14:27:26.005277 metablock-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1118 2023-05-28 14:27:26.005277 metablock-0.7.1/readme.md
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 metablock-0.7.1/PKG-INFO
```

### Comparing `metablock-0.7.0/LICENSE` & `metablock-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/metablock/cli.py` & `metablock-0.7.1/metablock/cli.py`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/metablock/client.py` & `metablock-0.7.1/metablock/client.py`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/metablock/components.py` & `metablock-0.7.1/metablock/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         url = self.list_create_url()
         kwargs.setdefault("wrap", self.entity_list)
         return cast(
             list[E],
             await self.cli.request(url, **kwargs),
         )
 
-    async def get_full_list(self, **kwargs: Any) -> list[MetablockEntity]:
+    async def get_full_list(self, **kwargs: Any) -> list[E]:
         return [d async for d in self.paginate(**kwargs)]
 
     async def get(self, id_: str, **kwargs: Any) -> E:
         url = f"{self.url}/{id_}"
         kwargs.setdefault("wrap", self.entity)
         return cast(E, await self.cli.get(url, **kwargs))
```

### Comparing `metablock-0.7.0/metablock/extensions.py` & `metablock-0.7.1/metablock/extensions.py`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/metablock/orgs.py` & `metablock-0.7.1/metablock/orgs.py`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/metablock/spaces.py` & `metablock-0.7.1/metablock/spaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     """Object representing a space"""
 
     @property
     def blocks(self) -> SpaceBlocks:
         return SpaceBlocks(self, Block, "services")
 
     @property
-    def services(self) -> SpaceBlocks:
+    def services(self) -> SpaceBlocks:  # pragma: no cover
+        # TODO: Deprecate
         return self.blocks
 
     @property
     def extensions(self) -> SpaceExtensions:
         return SpaceExtensions(self, SpaceExtension, "extensions")
```

### Comparing `metablock-0.7.0/metablock/user.py` & `metablock-0.7.1/metablock/user.py`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/pyproject.toml` & `metablock-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metablock"
-version = "0.7.0"
+version = "0.7.1"
 description = "Metablock cloud python client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `metablock-0.7.0/readme.md` & `metablock-0.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `metablock-0.7.0/PKG-INFO` & `metablock-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metablock
-Version: 0.7.0
+Version: 0.7.1
 Summary: Metablock cloud python client
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

