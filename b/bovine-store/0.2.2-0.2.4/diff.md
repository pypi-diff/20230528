# Comparing `tmp/bovine_store-0.2.2.tar.gz` & `tmp/bovine_store-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_store-0.2.2.tar", max compression
+gzip compressed data, was "bovine_store-0.2.4.tar", max compression
```

## Comparing `bovine_store-0.2.2.tar` & `bovine_store-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2754 2023-05-22 14:17:04.670843 bovine_store-0.2.2/README.md
--rw-r--r--   0        0        0     6489 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/__init__.py
--rw-r--r--   0        0        0     1115 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/actor/__init__.py
--rw-r--r--   0        0        0     7070 2023-05-25 18:44:02.790690 bovine_store-0.2.2/bovine_store/actor/bovine_store_actor.py
--rw-r--r--   0        0        0     1844 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/actor/register.py
--rw-r--r--   0        0        0      731 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/actor/test_bovine_application_actor.py
--rw-r--r--   0        0        0     5217 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/actor/test_bovine_store_actor.py
--rw-r--r--   0        0        0     1684 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/actor/test_register.py
--rw-r--r--   0        0        0     1955 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/blueprint.py
--rw-r--r--   0        0        0      578 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/config.py
--rw-r--r--   0        0        0        0 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/fedi/__init__.py
--rw-r--r--   0        0        0      999 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/fedi/authorize.py
--rw-r--r--   0        0        0     1597 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/fedi/retrieve_public_key.py
--rw-r--r--   0        0        0     2398 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/fedi/test_authorize.py
--rw-r--r--   0        0        0     3986 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/fedi/test_retrieve_public_key.py
--rw-r--r--   0        0        0     2285 2023-05-22 14:17:04.670843 bovine_store-0.2.2/bovine_store/models.py
--rw-r--r--   0        0        0     1274 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/__init__.py
--rw-r--r--   0        0        0     3432 2023-05-25 18:44:02.790690 bovine_store-0.2.2/bovine_store/store/collection.py
--rw-r--r--   0        0        0     1101 2023-05-25 18:44:02.790690 bovine_store-0.2.2/bovine_store/store/remote.py
--rw-r--r--   0        0        0     1343 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/retrieve_object.py
--rw-r--r--   0        0        0     2544 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/store.py
--rw-r--r--   0        0        0      533 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_application_actor_data.py
--rw-r--r--   0        0        0     4100 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_collection.py
--rw-r--r--   0        0        0     1657 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_retrieve_object.py
--rw-r--r--   0        0        0     3591 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_store.py
--rw-r--r--   0        0        0     1904 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_store_remote.py
--rw-r--r--   0        0        0      184 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/test_utils.py
--rw-r--r--   0        0        0      582 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/store/utils.py
--rw-r--r--   0        0        0     3541 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/templates/fallback.html
--rw-r--r--   0        0        0      314 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/test_bovine_admin_store.py
--rw-r--r--   0        0        0      475 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/test_store.py
--rw-r--r--   0        0        0      455 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/types.py
--rw-r--r--   0        0        0      787 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/utils/__init__.py
--rw-r--r--   0        0        0      834 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/utils/collection.py
--rw-r--r--   0        0        0     1288 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/utils/ordered_collection.py
--rw-r--r--   0        0        0      680 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/utils/permissions.py
--rw-r--r--   0        0        0     2403 2023-05-22 14:17:04.674842 bovine_store-0.2.2/bovine_store/utils/test.py
--rw-r--r--   0        0        0      619 2023-05-22 14:17:04.678842 bovine_store-0.2.2/bovine_store/utils/test_path.py
--rw-r--r--   0        0        0      726 2023-05-22 14:17:04.678842 bovine_store-0.2.2/bovine_store/utils/test_permissions.py
--rw-r--r--   0        0        0      294 2023-03-30 06:22:46.668327 bovine_store-0.2.2/bovine_store/utils/test_summary.py
--rw-r--r--   0        0        0      375 2023-05-22 14:17:04.678842 bovine_store-0.2.2/bovine_store/utils/test_test.py
--rw-r--r--   0        0        0      917 2023-05-25 18:44:02.806690 bovine_store-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 bovine_store-0.2.2/setup.py
--rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 bovine_store-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2754 2023-05-22 14:17:04.670843 bovine_store-0.2.4/README.md
+-rw-r--r--   0        0        0     6489 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/__init__.py
+-rw-r--r--   0        0        0     1115 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/actor/__init__.py
+-rw-r--r--   0        0        0     7070 2023-05-27 18:23:43.579051 bovine_store-0.2.4/bovine_store/actor/bovine_store_actor.py
+-rw-r--r--   0        0        0     1844 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/actor/register.py
+-rw-r--r--   0        0        0      731 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/actor/test_bovine_application_actor.py
+-rw-r--r--   0        0        0     5217 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/actor/test_bovine_store_actor.py
+-rw-r--r--   0        0        0     1684 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/actor/test_register.py
+-rw-r--r--   0        0        0     1955 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/blueprint.py
+-rw-r--r--   0        0        0      578 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/fedi/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/fedi/authorize.py
+-rw-r--r--   0        0        0     1597 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/fedi/retrieve_public_key.py
+-rw-r--r--   0        0        0     2398 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/fedi/test_authorize.py
+-rw-r--r--   0        0        0     3986 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/fedi/test_retrieve_public_key.py
+-rw-r--r--   0        0        0     2285 2023-05-22 14:17:04.670843 bovine_store-0.2.4/bovine_store/models.py
+-rw-r--r--   0        0        0     1356 2023-05-27 18:23:43.579051 bovine_store-0.2.4/bovine_store/store/__init__.py
+-rw-r--r--   0        0        0     3432 2023-05-27 18:23:43.579051 bovine_store-0.2.4/bovine_store/store/collection.py
+-rw-r--r--   0        0        0     1101 2023-05-27 18:23:43.579051 bovine_store-0.2.4/bovine_store/store/remote.py
+-rw-r--r--   0        0        0     1343 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/retrieve_object.py
+-rw-r--r--   0        0        0     2544 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/store.py
+-rw-r--r--   0        0        0      533 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_application_actor_data.py
+-rw-r--r--   0        0        0     4100 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_collection.py
+-rw-r--r--   0        0        0     1657 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_retrieve_object.py
+-rw-r--r--   0        0        0     3591 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_store.py
+-rw-r--r--   0        0        0     1904 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_store_remote.py
+-rw-r--r--   0        0        0      184 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/test_utils.py
+-rw-r--r--   0        0        0      582 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/store/utils.py
+-rw-r--r--   0        0        0     3541 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/templates/fallback.html
+-rw-r--r--   0        0        0      314 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/test_bovine_admin_store.py
+-rw-r--r--   0        0        0      475 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/test_store.py
+-rw-r--r--   0        0        0      455 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/types.py
+-rw-r--r--   0        0        0      787 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/utils/__init__.py
+-rw-r--r--   0        0        0      834 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/utils/collection.py
+-rw-r--r--   0        0        0     1288 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/utils/ordered_collection.py
+-rw-r--r--   0        0        0      680 2023-05-22 14:17:04.674842 bovine_store-0.2.4/bovine_store/utils/permissions.py
+-rw-r--r--   0        0        0     2231 2023-05-27 18:23:43.579051 bovine_store-0.2.4/bovine_store/utils/test.py
+-rw-r--r--   0        0        0      619 2023-05-22 14:17:04.678842 bovine_store-0.2.4/bovine_store/utils/test_path.py
+-rw-r--r--   0        0        0      726 2023-05-22 14:17:04.678842 bovine_store-0.2.4/bovine_store/utils/test_permissions.py
+-rw-r--r--   0        0        0      294 2023-03-30 06:22:46.668327 bovine_store-0.2.4/bovine_store/utils/test_summary.py
+-rw-r--r--   0        0        0      375 2023-05-22 14:17:04.678842 bovine_store-0.2.4/bovine_store/utils/test_test.py
+-rw-r--r--   0        0        0      917 2023-05-27 18:46:03.793874 bovine_store-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 bovine_store-0.2.4/setup.py
+-rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 bovine_store-0.2.4/PKG-INFO
```

### Comparing `bovine_store-0.2.2/README.md` & `bovine_store-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/__init__.py` & `bovine_store-0.2.4/bovine_store/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/__init__.py` & `bovine_store-0.2.4/bovine_store/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/bovine_store_actor.py` & `bovine_store-0.2.4/bovine_store/actor/bovine_store_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/register.py` & `bovine_store-0.2.4/bovine_store/actor/register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/test_bovine_application_actor.py` & `bovine_store-0.2.4/bovine_store/actor/test_bovine_application_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/test_bovine_store_actor.py` & `bovine_store-0.2.4/bovine_store/actor/test_bovine_store_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/actor/test_register.py` & `bovine_store-0.2.4/bovine_store/actor/test_register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/blueprint.py` & `bovine_store-0.2.4/bovine_store/blueprint.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/config.py` & `bovine_store-0.2.4/bovine_store/config.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/fedi/authorize.py` & `bovine_store-0.2.4/bovine_store/fedi/authorize.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/fedi/retrieve_public_key.py` & `bovine_store-0.2.4/bovine_store/fedi/retrieve_public_key.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/fedi/test_authorize.py` & `bovine_store-0.2.4/bovine_store/fedi/test_authorize.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/fedi/test_retrieve_public_key.py` & `bovine_store-0.2.4/bovine_store/fedi/test_retrieve_public_key.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/models.py` & `bovine_store-0.2.4/bovine_store/models.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/__init__.py` & `bovine_store-0.2.4/bovine_store/store/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                 public_key, private_key = generate_rsa_public_private_key()
             await BovineActorKeyPair.create(
                 bovine_actor=actor,
                 name="main-key",
                 private_key=private_key,
                 public_key=public_key,
             )
+            return {"public_key": public_key, "private_key": private_key, **data}
         return data
 
     await actor.fetch_related("keypairs")
 
     for kp in actor.keypairs:
         if kp.name == "main-key":
             return {"private_key": kp.private_key, "public_key": kp.public_key}
```

### Comparing `bovine_store-0.2.2/bovine_store/store/collection.py` & `bovine_store-0.2.4/bovine_store/store/collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/remote.py` & `bovine_store-0.2.4/bovine_store/store/remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/retrieve_object.py` & `bovine_store-0.2.4/bovine_store/store/retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/store.py` & `bovine_store-0.2.4/bovine_store/store/store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/test_application_actor_data.py` & `bovine_store-0.2.4/bovine_store/store/test_application_actor_data.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/test_collection.py` & `bovine_store-0.2.4/bovine_store/store/test_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/test_retrieve_object.py` & `bovine_store-0.2.4/bovine_store/store/test_retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/test_store.py` & `bovine_store-0.2.4/bovine_store/store/test_store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/test_store_remote.py` & `bovine_store-0.2.4/bovine_store/store/test_store_remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/store/utils.py` & `bovine_store-0.2.4/bovine_store/store/utils.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/templates/fallback.html` & `bovine_store-0.2.4/bovine_store/templates/fallback.html`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/__init__.py` & `bovine_store-0.2.4/bovine_store/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/collection.py` & `bovine_store-0.2.4/bovine_store/utils/collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/ordered_collection.py` & `bovine_store-0.2.4/bovine_store/utils/ordered_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/permissions.py` & `bovine_store-0.2.4/bovine_store/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/test.py` & `bovine_store-0.2.4/bovine_store/utils/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,19 +31,14 @@
 async def store():
     if not os.environ.get("POSTGRES"):
         db_file = "test_db.db"
         db_url = f"sqlite://{db_file}"
 
         store = BovineStore(
             db_url,
-            application_data={
-                "public_key": "public",
-                "account_url": "localhost",
-                "access_token": "secret",
-            },
             session=AsyncMock(),
         )
 
         await init_connection(db_url)
 
         yield store
         await close_connection()
```

### Comparing `bovine_store-0.2.2/bovine_store/utils/test_path.py` & `bovine_store-0.2.4/bovine_store/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/bovine_store/utils/test_permissions.py` & `bovine_store-0.2.4/bovine_store/utils/test_permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.2/pyproject.toml` & `bovine_store-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-store"
-version = "0.2.2"
+version = "0.2.4"
 description = "Store for ActivityPub activities, actors and objects"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine_store"}]
 repository = "https://codeberg.org/bovine/bovine"
```

### Comparing `bovine_store-0.2.2/setup.py` & `bovine_store-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 install_requires = \
 ['bovine>=0.2.1,<0.3.0',
  'quart>=0.18.3,<0.19.0',
  'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'bovine-store',
-    'version': '0.2.2',
+    'version': '0.2.4',
     'description': 'Store for ActivityPub activities, actors and objects',
     'long_description': '# bovine_store\n\n`bovine_store` is meant to be the module handling storing of\nlocal ActivityPub objects and caching of remote ActivityPub\nobjects.\n\n## Usage\n\nbovine_store assumes that a database connection is initialized using [tortoise-orm](https://tortoise.github.io/). See `examples/basic_app.py` for how to do this in the context of a quart app.\n\n## TODO\n\n- [ ] When properties of actor are updated, send an update Activity\n- [ ] Generally rework the actor properties mechanism. It is currently not possible to emulate say Mastodon featured collection with it.\n- [ ] bovine_store.models.BovineActorKeyPair needs renamings; and work, e.g. a future identity column should have a uniqueness constraint.\n- [ ] Generally the code quality is not as high as it should be.\n\n## Design discussion\n\nSome goals and design decisions:\n\n- Objects with an id are stored separately and can be looked up via this id. This is done by json-ld magic.\n- Collections are not stored. Instead for local items, the information that the item belongs to a collection is stored. `bovine_store.store.collection` contains the coroutines necessary to build the collection from this information. All collections are assumed to ActivityStreams 2 `OrderedCollection` and ordered by the database id.\n- Every object is currently assigned an `owner`. The idea was that an activity is owner by its actor. This can then be propagated to the subobjects, e.g. the object, attachments, and so on. Unfortunately, this is too naive:\n  - Some implementations include remote objects, e.g. the object being liked in a Like Activity.\n  - Mastodon includes its custom emojis. These have an id and should probably belong to the server.\n- There are three kinds of visibility.\n  - An object is always visible to its owner\n  - Public Objects are assigned `VisibilityType.PUBLIC`. These can viewed by all users providing valid authentication.\n  - Furthemore, by adding actors to the `VisibileTo` list of an object. This can be made visible to the corresponding actors.\n- An item is visible to be inside a collection if and only if said item is visible. This should probably be augmented by visible to the owner of the collection.\n- `bovine_store.blueprint` contains a quart blueprint with the basic retrievel mechanism for the stored objects.\n- `bovine_store.collection` contains the helper routine for collection responses.\n\n## Examples\n\nA demonstration webserver can be seen using\n\n```bash\npoetry run python examples/basic_app.py\n```\n\nNote this is a very basic example. Instructions what the example does are\nprinted to the command line after start.\n\nNote: This example creates two files `db.sqlite3`, which contains the\ndatabase and `context_cache.sqlite`, which contains the cache of json-ld\ncontexts.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_store-0.2.2/PKG-INFO` & `bovine_store-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-store
-Version: 0.2.2
+Version: 0.2.4
 Summary: Store for ActivityPub activities, actors and objects
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

