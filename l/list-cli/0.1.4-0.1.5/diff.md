# Comparing `tmp/list-cli-0.1.4.tar.gz` & `tmp/list-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-cli-0.1.4.tar", last modified: Mon May 22 17:15:30 2023, max compression
+gzip compressed data, was "list-cli-0.1.5.tar", last modified: Sun May 28 19:18:01 2023, max compression
```

## Comparing `list-cli-0.1.4.tar` & `list-cli-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.313138 list-cli-0.1.4/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.4/LICENSE
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-22 17:15:30.313207 list-cli-0.1.4/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.4/README.md
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.312411 list-cli-0.1.4/list_cli/
--rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.4/list_cli/__init__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.4/list_cli/__main__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-18 21:29:58.000000 list-cli-0.1.4/list_cli/__version__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)    12180 2023-05-18 21:27:25.000000 list-cli-0.1.4/list_cli/processors.py
--rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.4/list_cli/results.py
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.313014 list-cli-0.1.4/list_cli.egg-info/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-22 17:15:30.313407 list-cli-0.1.4/setup.cfg
--rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.4/setup.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.121319 list-cli-0.1.5/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.5/LICENSE
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-28 19:18:01.121388 list-cli-0.1.5/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.5/README.md
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.120357 list-cli-0.1.5/list_cli/
+-rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.5/list_cli/__init__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.5/list_cli/__main__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-28 19:17:06.000000 list-cli-0.1.5/list_cli/__version__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)    12511 2023-05-28 19:13:53.000000 list-cli-0.1.5/list_cli/processors.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.5/list_cli/results.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.121205 list-cli-0.1.5/list_cli.egg-info/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-28 19:18:01.121586 list-cli-0.1.5/setup.cfg
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.5/setup.py
```

### Comparing `list-cli-0.1.4/LICENSE` & `list-cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.4/PKG-INFO` & `list-cli-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.4/README.md` & `list-cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.4/list_cli/__main__.py` & `list-cli-0.1.5/list_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.4/list_cli/processors.py` & `list-cli-0.1.5/list_cli/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,41 +126,45 @@
         self._database.append(datum)
         return SuccessResult() if self._write_database() else ErrorResult()
 
     def _done(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
             return ErrorResult()
+        if index is None or index >= len(bucket):
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.DONE_BUCKET
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+            break
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _edit(
         self,
         index=None,
         message=None
     ) -> Result:
         if not message:
             return ErrorResult()
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
             return ErrorResult()
+        if index is None or index >= len(bucket):
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['message'] = message
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+            break
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _ensure_database_exists(self) -> bool:
         database_file_path = self._database_file_path
         database_dirname = dirname(database_file_path)
         if database_dirname and not isdir(database_dirname):
             makedirs(database_dirname)
         if not isfile(database_file_path):
@@ -228,48 +232,52 @@
     def _get_user(self) -> str:
         return getuser()
 
     def _handoff(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
             return ErrorResult()
+        if index is None or index >= len(bucket):
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.HANDED_OFF_BUCKET
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+            break
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _move(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
-        if not bucket:
+        if not bucket or index >= len(bucket):
             return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.MOVED_BUCKET
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+            break
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _remove(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
             return ErrorResult()
+        if index is None or index >= len(bucket):
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.REMOVED_BUCKET
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+            break
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _render(self, bucket_id) -> Result:
         bucket = self._get_bucket(bucket_id)
         if not bucket:
             return Result(had_error=bucket_id != self.ADDED_BUCKET, had_output=False)
         if self._output_file_path:
             print(f'{self._database_file_path}:{linesep}')
@@ -277,21 +285,22 @@
             print('%3d. %s' % (datum_index + 1, datum['message']))
         return SuccessResult(had_output=True)
 
     def _touch(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
             return ErrorResult()
+        if index is None or index >= len(bucket):
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
-            if datum_index != index:
+            if datum_index == index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
-            return SuccessResult() if self._write_database() else ErrorResult()
-        return ErrorResult()
+        return SuccessResult() if self._write_database() else ErrorResult()
 
     def _write_database(self) -> bool:
         with open(self._database_file_path, 'w') as database_file:
             for datum in self._database:
                 database_file.write(
                     "%s\t%s\t%s\t%s\t%d\t%d\t%s\t%s%s" % (
                         datum['id'],
```

### Comparing `list-cli-0.1.4/list_cli/results.py` & `list-cli-0.1.5/list_cli/results.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.4/list_cli.egg-info/PKG-INFO` & `list-cli-0.1.5/list_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.4/setup.py` & `list-cli-0.1.5/setup.py`

 * *Files identical despite different names*

