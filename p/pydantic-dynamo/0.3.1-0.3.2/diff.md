# Comparing `tmp/pydantic_dynamo-0.3.1.tar.gz` & `tmp/pydantic_dynamo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_dynamo-0.3.1.tar", max compression
+gzip compressed data, was "pydantic_dynamo-0.3.2.tar", max compression
```

## Comparing `pydantic_dynamo-0.3.1.tar` & `pydantic_dynamo-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.3.1/pydantic_dynamo/__init__.py
--rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.3.1/pydantic_dynamo/constants.py
--rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.3.1/pydantic_dynamo/exceptions.py
--rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.1/pydantic_dynamo/models.py
--rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.3.1/pydantic_dynamo/repository.py
--rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.1/pydantic_dynamo/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.3.1/pydantic_dynamo/v2/__init__.py
--rw-r--r--   0        0        0     4403 2023-04-29 12:58:54.202235 pydantic_dynamo-0.3.1/pydantic_dynamo/v2/models.py
--rw-r--r--   0        0        0    17272 2023-04-29 20:42:00.023856 pydantic_dynamo-0.3.1/pydantic_dynamo/v2/repository.py
--rw-r--r--   0        0        0     3805 2023-04-29 13:00:04.168642 pydantic_dynamo-0.3.1/pydantic_dynamo/v2/sync_repository.py
--rw-r--r--   0        0        0     2693 2023-05-04 00:29:12.717791 pydantic_dynamo-0.3.1/pydantic_dynamo/v2/write_once.py
--rw-r--r--   0        0        0     1260 2023-05-04 00:37:20.834323 pydantic_dynamo-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    18573 2023-04-29 23:01:49.944457 pydantic_dynamo-0.3.1/README.md
--rw-r--r--   0        0        0    18706 1970-01-01 00:00:00.000000 pydantic_dynamo-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.3.2/pydantic_dynamo/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.3.2/pydantic_dynamo/constants.py
+-rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.3.2/pydantic_dynamo/exceptions.py
+-rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.2/pydantic_dynamo/models.py
+-rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.3.2/pydantic_dynamo/repository.py
+-rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.2/pydantic_dynamo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.3.2/pydantic_dynamo/v2/__init__.py
+-rw-r--r--   0        0        0     4403 2023-04-29 12:58:54.202235 pydantic_dynamo-0.3.2/pydantic_dynamo/v2/models.py
+-rw-r--r--   0        0        0    17379 2023-05-28 12:40:45.131509 pydantic_dynamo-0.3.2/pydantic_dynamo/v2/repository.py
+-rw-r--r--   0        0        0     3805 2023-04-29 13:00:04.168642 pydantic_dynamo-0.3.2/pydantic_dynamo/v2/sync_repository.py
+-rw-r--r--   0        0        0     2693 2023-05-04 00:29:12.717791 pydantic_dynamo-0.3.2/pydantic_dynamo/v2/write_once.py
+-rw-r--r--   0        0        0     1260 2023-05-28 12:41:14.416585 pydantic_dynamo-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    18573 2023-04-29 23:01:49.944457 pydantic_dynamo-0.3.2/README.md
+-rw-r--r--   0        0        0    18706 1970-01-01 00:00:00.000000 pydantic_dynamo-0.3.2/PKG-INFO
```

### Comparing `pydantic_dynamo-0.3.1/LICENSE` & `pydantic_dynamo-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/models.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/repository.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/utils.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/v2/models.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/v2/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/v2/repository.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/v2/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,25 +313,28 @@
             ]
             yield BatchResponse(contents=contents)
 
     def _db_item_to_object(self, db_item: Dict[str, Any]) -> PartitionedContent[ObjT]:
         expiry: Optional[datetime] = None
         if db_expiry := db_item.pop(INTERNAL_TTL, None):
             expiry = datetime.fromtimestamp(int(db_expiry), tz=timezone.utc)
-        return PartitionedContent[self._item_class](  # type: ignore[name-defined]
-            partition_ids=db_item.pop(self._partition_key)
+
+        item_kwargs = {
+            "partition_ids": db_item.pop(self._partition_key)
             .replace(self._partition_id(EMPTY_LIST), "", 1)
             .split("#"),
-            content_ids=db_item.pop(self._sort_key)
+            "content_ids": db_item.pop(self._sort_key)
             .replace(self._content_id(EMPTY_LIST), "", 1)
             .split("#"),
-            item=self._item_class(**db_item),
-            current_version=db_item.pop(INTERNAL_OBJECT_VERSION),
-            expiry=expiry,
-        )
+            "item": self._item_class(**db_item),
+            "expiry": expiry,
+        }
+        if version := db_item.pop(INTERNAL_OBJECT_VERSION, None):
+            item_kwargs["current_version"] = version
+        return PartitionedContent[self._item_class](**item_kwargs)  # type: ignore[name-defined]
 
     async def delete(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
     ) -> None:
         if partition_id is None:
```

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/v2/sync_repository.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/v2/sync_repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pydantic_dynamo/v2/write_once.py` & `pydantic_dynamo-0.3.2/pydantic_dynamo/v2/write_once.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/pyproject.toml` & `pydantic_dynamo-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-dynamo"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["David Jetter <davidajetter@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pydantic_dynamo"}]
 homepage = "https://github.com/david-a-jetter/pydantic-dynamo"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_dynamo-0.3.1/README.md` & `pydantic_dynamo-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.3.1/PKG-INFO` & `pydantic_dynamo-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-dynamo
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/david-a-jetter/pydantic-dynamo
 Author: David Jetter
 Author-email: davidajetter@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

