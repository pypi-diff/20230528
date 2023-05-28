# Comparing `tmp/ardilla-0.2.1b0.tar.gz` & `tmp/ardilla-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.2.1b0.tar", last modified: Fri May 26 03:01:09 2023, max compression
+gzip compressed data, was "ardilla-0.3.0b0.tar", last modified: Sun May 28 06:11:37 2023, max compression
```

## Comparing `ardilla-0.2.1b0.tar` & `ardilla-0.3.0b0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.099812 ardilla-0.2.1b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.2.1b0/LICENCE
--rw-rw-rw-   0        0        0     5298 2023-05-26 03:01:09.097814 ardilla-0.2.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     4396 2023-05-25 05:34:17.000000 ardilla-0.2.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.003809 ardilla-0.2.1b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.2.1b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3537 2023-05-26 02:48:12.000000 ardilla-0.2.1b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.084811 ardilla-0.2.1b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.2.1b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.2.1b0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     8929 2023-05-26 02:57:48.000000 ardilla-0.2.1b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     2398 2023-05-25 18:19:51.000000 ardilla-0.2.1b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     8537 2023-05-26 02:56:48.000000 ardilla-0.2.1b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     4983 2023-05-25 18:16:14.000000 ardilla-0.2.1b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.2.1b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.2.1b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.2.1b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2885 2023-05-25 17:39:33.000000 ardilla-0.2.1b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.2.1b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.2.1b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5181 2023-05-25 17:28:48.000000 ardilla-0.2.1b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.052814 ardilla-0.2.1b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     5298 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1216 2023-05-26 03:00:00.000000 ardilla-0.2.1b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 03:01:09.099812 ardilla-0.2.1b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.094814 ardilla-0.2.1b0/tests/
--rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.2.1b0/tests/test_async.py
--rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.2.1b0/tests/test_models.py
--rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.2.1b0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:11:37.555184 ardilla-0.3.0b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.0b0/LICENCE
+-rw-rw-rw-   0        0        0     5203 2023-05-28 06:11:37.553187 ardilla-0.3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4301 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 06:11:37.327168 ardilla-0.3.0b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.0b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     4794 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:11:37.519779 ardilla-0.3.0b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.0b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     8530 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     1997 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     8762 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     2019 2023-05-28 05:59:00.000000 ardilla-0.3.0b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.0b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.0b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2885 2023-05-25 17:39:33.000000 ardilla-0.3.0b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.0b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6454 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     5463 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:11:37.494820 ardilla-0.3.0b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     5203 2023-05-28 06:11:36.000000 ardilla-0.3.0b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-28 06:11:36.000000 ardilla-0.3.0b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:11:36.000000 ardilla-0.3.0b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-05-28 06:11:36.000000 ardilla-0.3.0b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 06:11:36.000000 ardilla-0.3.0b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1216 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 06:11:37.558291 ardilla-0.3.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 06:11:37.545629 ardilla-0.3.0b0/tests/
+-rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.3.0b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.0b0/tests/test_sync.py
```

### Comparing `ardilla-0.2.1b0/LICENCE` & `ardilla-0.3.0b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.1b0/PKG-INFO` & `ardilla-0.3.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.2.1b0
+Version: 0.3.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -73,36 +73,28 @@
 
 ## How to use
 
 ```py
 from ardilla import Engine, Model, Crud
 from pydantic import Field
 
-engine = Engine('db.sqlite3')
-
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-crud = engine.crud(User)
-
 def main():
-    # get or none
-    user = crud.get_or_none(id=1) # user with id of 1
-    # get or create
-    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-    # get many
-    users = crud.get_many(name='chris') # all users named chris
-    # save one
-    user3 = User(id=3, name='moni', age=35)
-    user.age += 1 # it's her birthday
-    crud.save_one(user3)
-    # save many
-    crud.save_many(user, user2, user3)
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
```

### Comparing `ardilla-0.2.1b0/README.md` & `ardilla-0.3.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,36 +50,28 @@
 
 ## How to use
 
 ```py
 from ardilla import Engine, Model, Crud
 from pydantic import Field
 
-engine = Engine('db.sqlite3')
-
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-crud = engine.crud(User)
-
 def main():
-    # get or none
-    user = crud.get_or_none(id=1) # user with id of 1
-    # get or create
-    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-    # get many
-    users = crud.get_many(name='chris') # all users named chris
-    # save one
-    user3 = User(id=3, name='moni', age=35)
-    user.age += 1 # it's her birthday
-    crud.save_one(user3)
-    # save many
-    crud.save_many(user, user2, user3)
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
```

### Comparing `ardilla-0.2.1b0/ardilla/asyncio/crud.py` & `ardilla-0.3.0b0/ardilla/crud.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,259 +1,267 @@
 from __future__ import annotations
-from functools import wraps
-from typing import Literal, Generic, Optional, Union
+import sqlite3
+from sqlite3 import Row
+from contextlib import contextmanager
+from typing import Literal, Generic, Optional, Union, Generator
+
+from . import queries
+from .abc import BaseCrud
+from .models import M
+from .errors import QueryExecutionError, disconnected_engine_error, DisconnectedEngine
+from .schemas import SQLFieldType
+
+
+@contextmanager
+def contextcursor(con: sqlite3.Connection) -> Generator[sqlite3.Cursor, None, None]:
+    """a context manager wrapper for sqlite3.Cursor
 
-import aiosqlite
-from aiosqlite import Row
+    Args:
+        con (sqlite3.Connection): the connection
 
-from ..errors import QueryExecutionError
-from ..models import M
-from ..abc import CrudABC
-from ..logging import log
-from ..schemas import SQLFieldType
-from .. import queries
+    Raises:
+        disconnected_engine_error: if the connection is non functioning
 
-from .abc import AbstractAsyncEngine
-
-
-def async_verify_kws(coro):
+    Yields:
+        Generator[sqlite3.Cursor, None, None]: the cursor
     """
-    Decorator for sync Crud methods to prevent
-    injection in the keys of the CRUD methods
-    """
-    @wraps(coro)
-    async def wrapper(self: AsyncCrud, *ags, **kws):
-        for key in kws:
-            if key not in self.Model.__fields__:
-                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
-        return await coro(self, *ags, **kws)
-    return wrapper
+    cur = None
+    try:
+        cur = con.cursor()
+        yield cur
+    except Exception as e:
+        if (
+            isinstance(e, sqlite3.ProgrammingError)
+            and str(e) == "Cannot operate on a closed database."
+        ):
+            raise DisconnectedEngine(str(e))
+        else:
+            raise e
+    finally:
+        if cur is not None:
+            cur.close()
 
-class AsyncCrud(CrudABC, Generic[M]):
-    """Abstracts CRUD actions for model associated tables"""
-
-    engine: AbstractAsyncEngine
-
-    @async_verify_kws
-    async def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
-        """Returns a row as an instance of the model if one is found or none
 
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as column names and values to
-                a select query
-
-        Example:
-            ```py
-            await crud.get_or_none(id=42)
+class Crud(BaseCrud, Generic[M]):
+    """Abstracts CRUD actions for model associated tables"""
 
-            # returns an object with id of 42 or None if there isn't one in the database
-            ```
-        Returns:
-            The object found with the criteria if any
-        """
-        q, vals = queries.for_get_or_none(self.tablename, kws)
-        async with self.engine as con:
-            async with con.execute(q, vals) as cur:
-                row: Union[Row, None] = await cur.fetchone()
-                if row:
-                    return self._row2obj(row)
-        return None
+    connection: sqlite3.Connection
 
-    async def _do_insert(
+    def _do_insert(
         self,
         ignore: bool = False,
         returning: bool = True,
         /,
         **kws: SQLFieldType,
-    ):
+    ) -> Optional[M]:
         """private helper method for insertion methods
 
         Args:
             ignore (bool, optional): Ignores conflicts silently. Defaults to False.
             returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
-            kws (SQLFieldType): the column names and values for the insertion query
+            kws (SQLFieldType): the column name and values for the insert query
 
         Raises:
             QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
 
         Returns:
             An instance of model if any row is returned
         """
         q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
 
-        async with self.engine as con:
-            con = await self.engine.connect()
-            cur = None
+        with contextcursor(self.connection) as cur:
             try:
-                cur = await con.execute(q, vals)
-            except aiosqlite.IntegrityError as e:
+                cur.execute(q, vals)
+            except sqlite3.IntegrityError as e:
                 raise QueryExecutionError(str(e))
-            else:
-                row = await cur.fetchone()
-                await con.commit()
-                if returning and row:
-                    return self._row2obj(row, cur.lastrowid)
-            finally:
-                if cur is not None:
-                    await cur.close()
-                await con.close()
 
-    @async_verify_kws
-    async def insert(self, **kws: SQLFieldType) -> M:
+            row = cur.fetchone()
+            self.connection.commit()
+            if returning and row:
+                return self._row2obj(row, cur.lastrowid)
+
+        return None
+
+    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
+        """Returns a row as an instance of the model if one is found or none
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as column names and values to
+                a select query
+
+        Example:
+            ```py
+            crud.get_or_none(id=42)
+
+            # returns an object with id of 42 or None if there isn't one in the database
+            ```
+
+        Returns:
+            The object found with the criteria if any
         """
-        Inserts a record into the database.
+        self.verify_kws(kws)
+        q, vals = queries.for_get_or_none(self.tablename, kws)
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            row: Union[Row, None] = cur.fetchone()
+            if row:
+                return self._row2obj(row)
+        return None
+
+    def insert(self, **kws: SQLFieldType) -> M:
+        """Inserts a record into the database.
 
         Args:
-            kws (SQLFieldType): the column names and values for the insertion query
+            kws (SQLFieldType): The keyword arguments are passed as the column names and values
+                to the insert query
 
         Returns:
-            Returns the inserted row as an instance of the model
+            Creates a new entry in the database and returns the object
+
         Rises:
-            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
+            `ardilla.error.QueryExecutionError`: if there's a conflict when inserting the record
         """
-        return await self._do_insert(False, True, **kws)
+        self.verify_kws(kws)
+        return self._do_insert(False, True, **kws)
 
-    @async_verify_kws
-    async def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
+    def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
         """Inserts a record to the database with the keywords passed. It ignores conflicts.
 
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
 
         Returns:
             The newly created row as an instance of the model if there was no conflicts
         """
-        return await self._do_insert(True, True, **kws)
+        self.verify_kws(kws)
+        return self._do_insert(True, True, **kws)
 
-    @async_verify_kws
-    async def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
+    def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
         """Returns an object from the database with the spefied matching data
         Args:
             kws (SQLFieldType): the key value pairs will be used to query for an existing row
                 if no record is found then a new row will be inserted
         Returns:
             A tuple with two values, the object and a boolean indicating if the
                 object was newly created or not
         """
+        self.verify_kws(kws)
         created = False
-        result = await self.get_or_none(**kws)
+        result = self.get_or_none(**kws)
         if not result:
-            result = await self.insert_or_ignore(**kws)
+            result = self.insert_or_ignore(**kws)
             created = True
         return result, created
-    
-    async def get_all(self) -> list[M]:
+
+    def get_all(self) -> list[M]:
         """Gets all objects from the database
-        
         Returns:
             A list with all the rows in table as instances of the model
         """
-        q = f"SELECT rowid, * FROM {self.tablename};"
-        log.debug(f"Querying: {q}")
-
-        async with self.engine as con:
-            async with con.execute(q) as cur:
-                return [self._row2obj(row) for row in await cur.fetchall()]
+        return self.get_many()
 
-    async def get_many(
+    def get_many(
         self,
         order_by: Optional[dict[str, str]] = None,
         limit: Optional[int] = None,
         **kws: SQLFieldType,
     ) -> list[M]:
         """Queries the database and returns objects that meet the criteris
 
         Args:
             order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
                 The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
                 Case in values is insensitive
-            kws (SQLFieldType): the column names and values for the select query
 
             limit (Optional[int], optional): The number of items to return. Defaults to None.
+            kws (SQLFieldType): The column names and values for the select query
 
         Returns:
             a list of rows matching the criteria as intences of the model
         """
-        for key in kws:
-            if key not in self.Model.__fields__:
-                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
-            
+        self.verify_kws(kws)
         q, vals = queries.for_get_many(
             self.Model, order_by=order_by, limit=limit, kws=kws
         )
-        async with self.engine as con:
-            async with con.execute(q, vals) as cur:
-                rows: list[Row] = await cur.fetchall()
-                return [self._row2obj(row) for row in rows]
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            rows: list[Row] = cur.fetchall()
+            return [self._row2obj(row) for row in rows]
 
-    async def save_one(self, obj: M) -> Literal[True]:
+    def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database
 
         Args:
             obj (M): the object to persist
 
         Returns:
             The literal `True` if the method ran successfuly
         """
         q, vals = queries.for_save_one(obj)
-
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
         return True
 
-    async def save_many(self, *objs: M) -> Literal[True]:
+    def save_many(self, *objs: tuple[M]) -> Literal[True]:
         """Saves all the passed objects to the database
 
         Args:
             objs (M): the objects to persist
 
         Returns:
             The literal `True` if the method ran successfuly
         """
         q, vals = queries.for_save_many(objs)
-
-        async with self.engine as con:
-            await con.executemany(q, vals)
-            await con.commit()
+        try:
+            self.connection.executemany(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
 
         return True
 
-    async def delete_one(self, obj: M) -> Literal[True]:
+    def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
         If the object has a PK field or the rowid setup, those will be
         used to locate the obj and delete it.
         If not, this function will delete any row that meets the values of the object
 
 
         Args:
             obj (M): the object to delete
 
         Returns:
             The literal `True` if the method ran successfuly
 
         """
-        q, vals = queries.for_delete_one(obj)
 
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+        q, vals = queries.for_delete_one(obj)
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
         return True
 
-    async def delete_many(self, *objs: M) -> Literal[True]:
+    def delete_many(self, *objs: M) -> Literal[True]:
         """
         Deletes all the objects passed
 
         Args:
             objs (M): the object to delete
 
         Returns:
             The literal `True` if the method ran successfuly
 
         """
         q, vals = queries.for_delete_many(objs)
-
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
+        return True
```

### Comparing `ardilla-0.2.1b0/ardilla/asyncio/engine.py` & `ardilla-0.3.0b0/ardilla/asyncio/engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 from __future__ import annotations
+
 import aiosqlite
 
-from .crud import AsyncCrud
+from ..abc import BaseEngine
 from ..models import M
-from ..engine import Engine
+from ..errors import DisconnectedEngine
 
-from .abc import AbstractAsyncEngine
+from .crud import AsyncCrud
 
-class AsyncEngine(Engine, AbstractAsyncEngine):
+class AsyncEngine(BaseEngine):
     """Async Engine that uses `aiosqlite.Connection` and `aiosqlite.Cursor`
-    Inhetits attributes from `Engine`
     """
-    def __init__(self, path: str, enable_foreing_keys: bool = False, single_connection: bool = False):
-        if single_connection is True:
-            raise NotImplementedError('The async engine does not support single connection for now')
-        super().__init__(path, enable_foreing_keys, single_connection)
+    con: aiosqlite.Connection
     
     async def connect(self) -> aiosqlite.Connection:
         """
         Stablishes a connection to the database
         Returns:
             The connection
         """
+        await self.close()
         con = await aiosqlite.connect(self.path)
         con.row_factory = aiosqlite.Row
+        if self.enable_foreing_keys:
+            await con.execute('PRAGMA foreign_keys = ON;')
+        self.con = con
         return con
 
-    async def __aenter__(self) -> aiosqlite.Connection:
+    async def close(self) -> None:
+        if self.check_connection():
+            await self.con.close()
+
+    async def __aenter__(self) -> AsyncEngine:
         """Stablishes the connection and if specified enables foreign keys pragma
 
         Returns:
             The connection
         """
-        self.acon = await self.connect()
-        if self.enable_foreing_keys:
-            await self.acon.execute('PRAGMA foreign_keys = ON;')
-            
-        return self.acon
+        await self.connect()
+        return self
 
     async def __aexit__(self, *_):
         """Closes the connection"""
-        await self.acon.close()
-
-    async def setup(self):
-        """Creates the tables setup by the engine
-        """
-        async with self as con:
-            for table in self.schemas:
-                await con.execute(table)
-                self.tables_created.add(table)
-            await con.commit()
+        await self.close()
     
-    def crud(self, Model: type[M]) -> AsyncCrud[M]:
+    async def crud(self, Model: type[M]) -> AsyncCrud[M]:
         """
-        This function runs synchronously and works exactly like `Engine.crud` but
+        This function works exactly like `Engine.crud` but
         returns an instance of `ardilla.asyncio.crud.AsyncCrud` instead of `ardilla.crud.Crud`
+        and is asynchronous
         
         Returns:
             The async Crud for the given model
         """
-        crud = self._cruds.setdefault(Model, AsyncCrud(Model, self))
+        if not self.check_connection():
+            raise DisconnectedEngine("Can't create crud objects with a disconnected engine")
+            
         if Model.__schema__ not in self.tables_created:
-            with self as con:
-                con.execute(Model.__schema__)
-                con.commit()
+            await self.con.execute(Model.__schema__)
+            await self.con.commit()
             self.tables_created.add(Model.__schema__)
-        return crud
+            
+        return AsyncCrud(Model, self.con)
```

### Comparing `ardilla-0.2.1b0/ardilla/crud.py` & `ardilla-0.3.0b0/ardilla/asyncio/crud.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,248 @@
 from __future__ import annotations
-from functools import wraps
-import sqlite3
-from sqlite3 import Row
 from typing import Literal, Generic, Optional, Union
 
-from .abc import CrudABC, AbstractEngine
-from .models import M
-from .errors import QueryExecutionError
-from .logging import log
-from .schemas import SQLFieldType
-from . import queries
-
-
-def verify_kws(f):
-    """
-    Decorator for sync Crud methods to prevent
-    injection in the keys of the CRUD methods
-    """
-    @wraps(f)
-    def wrapper(self: Crud, *ags, **kws):
-        for key in kws:
-            if key not in self.Model.__fields__:
-                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
-        return f(self, *ags, **kws)
-    return wrapper
+from typing import Any
+import aiosqlite
+from aiosqlite import Row
+
+from ..errors import QueryExecutionError, disconnected_engine_error
+from ..models import M
+from ..abc import BaseCrud
+from ..schemas import SQLFieldType
+from ..errors import DisconnectedEngine
+from .. import queries
+
+
+class ConnectionProxy:
+    def __init__(self, connection: aiosqlite.Connection):
+        self._connection = connection
+    
+    def __getattr__(self, __name: str) -> Any:
+        if self._connection._running and self._connection._connection:
+            return getattr(self._connection, __name)
+        else:
+            raise DisconnectedEngine('The engine is disconnected')
 
-class Crud(CrudABC, Generic[M]):
+
+class AsyncCrud(BaseCrud, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
+    connection: aiosqlite.Connection
+    
+    def __init__(self, Model: type[M], connection: aiosqlite.Connection) -> None:
+        connection = ConnectionProxy(connection)
+        super().__init__(Model, connection)
 
-    engine: AbstractEngine
 
-    def _do_insert(
+    async def _do_insert(
         self,
         ignore: bool = False,
         returning: bool = True,
         /,
         **kws: SQLFieldType,
-    ) -> Optional[M]:
+    ):
         """private helper method for insertion methods
 
         Args:
             ignore (bool, optional): Ignores conflicts silently. Defaults to False.
             returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
-            kws (SQLFieldType): the column name and values for the insert query
+            kws (SQLFieldType): the column names and values for the insertion query
 
         Raises:
             QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
 
         Returns:
             An instance of model if any row is returned
         """
         q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
 
-        with self.engine as con:
-            with self.engine.cursor(con) as cur:
-                try:
-                    cur.execute(q, vals)
-                except sqlite3.IntegrityError as e:
-                    raise QueryExecutionError(str(e))
-
-                row = cur.fetchone()
-                con.commit()
-                if returning and row:
-                    return self._row2obj(row, cur.lastrowid)
-
-        return None
+        cur = None
+        try:
+            cur = await self.connection.execute(q, vals)
+        except aiosqlite.IntegrityError as e:
+            raise QueryExecutionError(str(e))
+        except aiosqlite.ProgrammingError as e:
+            raise disconnected_engine_error
+        else:
+            row = await cur.fetchone()
+            await self.connection.commit()
+            if returning and row:
+                return self._row2obj(row, cur.lastrowid)
+        finally:
+            if cur is not None:
+                await cur.close()
 
-    @verify_kws
-    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
+    async def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
         """Returns a row as an instance of the model if one is found or none
 
         Args:
-            kws (SQLFieldType): The keyword arguments are passed as column names and values to 
+            kws (SQLFieldType): The keyword arguments are passed as column names and values to
                 a select query
-            
-        Example: 
+
+        Example:
             ```py
-            crud.get_or_none(id=42)
-            
-            # returns an object with id of 42 or None if there isn't one in the database 
+            await crud.get_or_none(id=42)
+
+            # returns an object with id of 42 or None if there isn't one in the database
             ```
-        
         Returns:
             The object found with the criteria if any
         """
+        self.verify_kws(kws)
         q, vals = queries.for_get_or_none(self.tablename, kws)
-        with self.engine as con:
-            ctxcur = self.engine.cursor(con)
-            with ctxcur as cur:
-                cur.execute(q, vals)
-                row: Union[Row, None] = cur.fetchone()
-                if row:
-                    return self._row2obj(row)
+
+        async with self.connection.execute(q, vals) as cur:
+            row: Union[Row, None] = await cur.fetchone()
+            if row:
+                return self._row2obj(row)
         return None
 
-    @verify_kws
-    def insert(self, **kws: SQLFieldType) -> M:
-        """Inserts a record into the database.
-        
+    async def insert(self, **kws: SQLFieldType) -> M:
+        """
+        Inserts a record into the database.
+
         Args:
-            kws (SQLFieldType): The keyword arguments are passed as the column names and values
-                to the insert query
-        
+            kws (SQLFieldType): the column names and values for the insertion query
+
         Returns:
-            Creates a new entry in the database and returns the object
-            
+            Returns the inserted row as an instance of the model
         Rises:
-            `ardilla.error.QueryExecutionError`: if there's a conflict when inserting the record
+            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
-        return self._do_insert(False, True, **kws)
+        self.verify_kws(kws)
+        return await self._do_insert(False, True, **kws)
 
-    @verify_kws
-    def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
+    async def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
         """Inserts a record to the database with the keywords passed. It ignores conflicts.
-        
+
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
 
         Returns:
             The newly created row as an instance of the model if there was no conflicts
         """
-        return self._do_insert(True, True, **kws)
-
+        self.verify_kws(kws)
+        return await self._do_insert(True, True, **kws)
 
-    @verify_kws
-    def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
+    async def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
         """Returns an object from the database with the spefied matching data
         Args:
             kws (SQLFieldType): the key value pairs will be used to query for an existing row
                 if no record is found then a new row will be inserted
         Returns:
-            A tuple with two values, the object and a boolean indicating if the 
+            A tuple with two values, the object and a boolean indicating if the
                 object was newly created or not
         """
         created = False
-        result = self.get_or_none(**kws)
+        result = await self.get_or_none(**kws)
         if not result:
-            result = self.insert_or_ignore(**kws)
+            result = await self.insert_or_ignore(**kws)
             created = True
         return result, created
 
-    def get_all(self) -> list[M]:
+    async def get_all(self) -> list[M]:
         """Gets all objects from the database
+
         Returns:
             A list with all the rows in table as instances of the model
         """
-        return self.get_many()
+        q = f"SELECT rowid, * FROM {self.tablename};"
 
-    def get_many(
+        async with self.connection.execute(q) as cur:
+            return [self._row2obj(row) for row in await cur.fetchall()]
+
+    async def get_many(
         self,
         order_by: Optional[dict[str, str]] = None,
         limit: Optional[int] = None,
         **kws: SQLFieldType,
     ) -> list[M]:
         """Queries the database and returns objects that meet the criteris
 
         Args:
             order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
                 The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
                 Case in values is insensitive
-            
+            kws (SQLFieldType): the column names and values for the select query
+
             limit (Optional[int], optional): The number of items to return. Defaults to None.
-            kws (SQLFieldType): The column names and values for the select query
 
         Returns:
             a list of rows matching the criteria as intences of the model
         """
-        for key in kws:
-            if key not in self.Model.__fields__:
-                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
-        q, vals = queries.for_get_many(self.Model, order_by=order_by, limit=limit, kws=kws)
-        with self.engine as con:
-            ctxcur = self.engine.cursor(con)
-            with ctxcur as cur:
-                cur.execute(q, vals)
-                rows: list[Row] = cur.fetchall()
-                return [self._row2obj(row) for row in rows]
+        self.verify_kws(kws)
+
+        q, vals = queries.for_get_many(
+            self.Model, order_by=order_by, limit=limit, kws=kws
+        )
+        async with self.connection.execute(q, vals) as cur:
+            rows: list[Row] = await cur.fetchall()
+            return [self._row2obj(row) for row in rows]
 
-    def save_one(self, obj: M) -> Literal[True]:
+    async def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database
 
         Args:
             obj (M): the object to persist
 
         Returns:
             The literal `True` if the method ran successfuly
         """
         q, vals = queries.for_save_one(obj)
 
-        with self.engine as con:
-            con.execute(q, vals)
-            con.commit()
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
         return True
 
-    def save_many(self, *objs: tuple[M]) -> Literal[True]:
+    async def save_many(self, *objs: M) -> Literal[True]:
         """Saves all the passed objects to the database
 
         Args:
             objs (M): the objects to persist
 
         Returns:
             The literal `True` if the method ran successfuly
-        """        
+        """
         q, vals = queries.for_save_many(objs)
-        with self.engine as con:
-            con.executemany(q, vals)
-            con.commit()
+
+        await self.connection.executemany(q, vals)
+        await self.connection.commit()
 
         return True
 
-    def delete_one(self, obj: M) -> Literal[True]:
+    async def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
         If the object has a PK field or the rowid setup, those will be
         used to locate the obj and delete it.
         If not, this function will delete any row that meets the values of the object
 
 
         Args:
             obj (M): the object to delete
 
         Returns:
             The literal `True` if the method ran successfuly
-            
+
         """
-        
         q, vals = queries.for_delete_one(obj)
-        with self.engine as con:
-            con.execute(q, vals)
-            con.commit()
 
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
         return True
 
-    def delete_many(self, *objs: M) -> Literal[True]:
+    async def delete_many(self, *objs: M) -> Literal[True]:
         """
         Deletes all the objects passed
 
         Args:
             objs (M): the object to delete
 
         Returns:
             The literal `True` if the method ran successfuly
-            
+
         """
         q, vals = queries.for_delete_many(objs)
-        with self.engine as con:
-            con.execute(q, vals)
-            con.commit()
 
-        return True
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
```

### Comparing `ardilla-0.2.1b0/ardilla/fields.py` & `ardilla-0.3.0b0/ardilla/fields.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.1b0/ardilla/models.py` & `ardilla-0.3.0b0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.1b0/ardilla/ordering.py` & `ardilla-0.3.0b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.1b0/ardilla/queries.py` & `ardilla-0.3.0b0/ardilla/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     Returns:
         tuple[str, tuple[Any, ...]]
     """
     if not objs:
         raise IndexError('param "objs" is empty, pass at least one object')
 
     tablename = objs[0].__tablename__
-    placeholders = ", ".join("?" for _ in objs)
+    placeholders = ", ".join("?" * len(objs))
     if all(obj.__rowid__ for obj in objs):
         vals = tuple(obj.__rowid__ for obj in objs)
         q = f"DELETE FROM {tablename} WHERE rowid IN ({placeholders})"
 
     elif pk := objs[0].__pk__:
         vals = tuple(getattr(obj, pk) for obj in objs)
         q = f"DELETE FROM {tablename} WHERE id IN ({placeholders})"
```

### Comparing `ardilla-0.2.1b0/ardilla/schemas.py` & `ardilla-0.3.0b0/ardilla/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,18 +76,24 @@
             if k in extra and extra[k]:
                 if pk is not None:
                     raise ModelIntegrityError('Only one primary key per model is allowed')
                 elif hasattr(Model, '__pk__') and Model.__pk__ != name:
                     raise ModelIntegrityError(f"field {name} is marked as pk, but __pk__ points to another field.")
                 
                 pk = name
+                
                 schema += ' PRIMARY KEY'
 
                 if auto and T in AUTOFIELDS:
                     schema += AUTOFIELDS[T]
+                    # make the field not required
+                    # this allows users to create
+                    # objects from the model without knowing the final 
+                    # value in the database
+                    field.required = False
                 elif auto:
                     raise autoerror
                 break
         else:
             if auto and T in AUTOFIELDS.keys() - {int}:
                 schema += AUTOFIELDS[T]
             elif auto:
```

### Comparing `ardilla-0.2.1b0/ardilla.egg-info/PKG-INFO` & `ardilla-0.3.0b0/ardilla.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.2.1b0
+Version: 0.3.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -73,36 +73,28 @@
 
 ## How to use
 
 ```py
 from ardilla import Engine, Model, Crud
 from pydantic import Field
 
-engine = Engine('db.sqlite3')
-
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-crud = engine.crud(User)
-
 def main():
-    # get or none
-    user = crud.get_or_none(id=1) # user with id of 1
-    # get or create
-    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-    # get many
-    users = crud.get_many(name='chris') # all users named chris
-    # save one
-    user3 = User(id=3, name='moni', age=35)
-    user.age += 1 # it's her birthday
-    crud.save_one(user3)
-    # save many
-    crud.save_many(user, user2, user3)
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
```

### Comparing `ardilla-0.2.1b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.3.0b0/ardilla.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,13 +14,12 @@
 ardilla/schemas.py
 ardilla.egg-info/PKG-INFO
 ardilla.egg-info/SOURCES.txt
 ardilla.egg-info/dependency_links.txt
 ardilla.egg-info/requires.txt
 ardilla.egg-info/top_level.txt
 ardilla/asyncio/__init__.py
-ardilla/asyncio/abc.py
 ardilla/asyncio/crud.py
 ardilla/asyncio/engine.py
 tests/test_async.py
 tests/test_models.py
 tests/test_sync.py
```

### Comparing `ardilla-0.2.1b0/pyproject.toml` & `ardilla-0.3.0b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.2.1-beta"
+version = "0.3.0-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ardilla-0.2.1b0/tests/test_models.py` & `ardilla-0.3.0b0/tests/test_models.py`

 * *Files identical despite different names*

