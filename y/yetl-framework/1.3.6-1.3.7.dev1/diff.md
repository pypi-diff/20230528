# Comparing `tmp/yetl-framework-1.3.6.tar.gz` & `tmp/yetl-framework-1.3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.3.6.tar", last modified: Sun May 14 21:09:07 2023, max compression
+gzip compressed data, was "yetl-framework-1.3.7.dev1.tar", last modified: Sun May 28 10:50:50 2023, max compression
```

## Comparing `yetl-framework-1.3.6.tar` & `yetl-framework-1.3.7.dev1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7948 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4195 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6273 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-14 21:09:07.000000 yetl-framework-1.3.6/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.265317 yetl-framework-1.3.7.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-28 10:50:50.265317 yetl-framework-1.3.7.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-28 10:50:50.265317 yetl-framework-1.3.7.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1117 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.253317 yetl-framework-1.3.7.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.253317 yetl-framework-1.3.7.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.257317 yetl-framework-1.3.7.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8759 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.261317 yetl-framework-1.3.7.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3990 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6228 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3713 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.261317 yetl-framework-1.3.7.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-28 10:49:51.000000 yetl-framework-1.3.7.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 10:50:50.265317 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-28 10:50:50.000000 yetl-framework-1.3.7.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.3.6/PKG-INFO` & `yetl-framework-1.3.7.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.6
+Version: 1.3.7.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -83,15 +83,14 @@
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
         delta.autoOptimize.autoCompact: true
         delta.autoOptimize.optimizeWrite: true
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: default
 
@@ -130,15 +129,14 @@
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
       mergeSchema: true
```

### Comparing `yetl-framework-1.3.6/README.md` & `yetl-framework-1.3.7.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,14 @@
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
         delta.autoOptimize.autoCompact: true
         delta.autoOptimize.optimizeWrite: true
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: default
 
@@ -115,15 +114,14 @@
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
       mergeSchema: true
```

### Comparing `yetl-framework-1.3.6/setup.py` & `yetl-framework-1.3.7.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.3.6",
+    version="1.3.7.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.3.6/yetl/__main__.py` & `yetl-framework-1.3.7.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/cli/_init.py` & `yetl-framework-1.3.7.dev1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/__init__.py` & `yetl-framework-1.3.7.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_config.py` & `yetl-framework-1.3.7.dev1/yetl/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,18 @@
         return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
+        create_table: bool = True
     ):
         table_mapping = self.tables.get_table_mapping(
-            stage=stage, table=table, database=database
+            stage=stage, table=table, database=database, create_table=create_table
         )
 
         return table_mapping
 
     def set_checkpoint(
         self,
         source: Table,
```

### Comparing `yetl-framework-1.3.6/yetl/config/_decorators.py` & `yetl-framework-1.3.7.dev1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_logging_config.py` & `yetl-framework-1.3.7.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_project.py` & `yetl-framework-1.3.7.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_spark_context.py` & `yetl-framework-1.3.7.dev1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_tables.py` & `yetl-framework-1.3.7.dev1/yetl/config/_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,20 +125,38 @@
         object it self. This dictionary index is held on self.tables_index
         """
         for index, table_config in self.tables_index.items():
             self.tables_index[index] = table_factory.make(
                 table_config["table_type"], table_config
             )
 
+    def create_table(
+        self,
+        stage: Union[StageType, str] = _INDEX_WILDCARD,
+        database=_INDEX_WILDCARD,
+        table=_INDEX_WILDCARD,
+        first_match: bool = True,
+        **kwargs
+    ):
+        return self.lookup_table(
+            stage=stage,
+            database=database,
+            table=table,
+            first_match=first_match,
+            create_table=True,
+            **kwargs
+        )
+
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
+        create_table: bool = False,
         **kwargs,
     ):
         index = Tables.get_index(stage, database, table)
         matches = fnmatch.filter(list(self.tables_index.keys()), index)
 
         if not matches:
             raise Exception(f"index {index} not found in tables_index")
@@ -169,38 +187,52 @@
             }
 
         if first_match:
             matches = matches[0]
             table = tables_index[matches]
             msg_tables = f"{table.database}.{table.table}"
             self._logger.info(f"Matched tables: {msg_tables}")
+            if create_table:
+                table.create_table()
             return table
         else:
             tables = [tables_index[i] for i in matches]
             msg_tables = "\n".join([f"{t.database}.{t.table}" for t in tables])
             self._logger.info(f"Matched tables: {msg_tables}")
+            if create_table:
+                for t in tables:
+                    t.create_table()
             return tables
 
     def get_table_mapping(
-        self, stage: StageType, table=_INDEX_WILDCARD, database=_INDEX_WILDCARD
+        self,
+        stage: StageType,
+        table=_INDEX_WILDCARD,
+        database=_INDEX_WILDCARD,
+        create_table: bool = True
     ):
         destination = self.lookup_table(
-            stage=stage, database=database, table=table, first_match=True
+            stage=stage,
+            database=database,
+            table=table,
+            first_match=True,
+            create_table=create_table
         )
         source = {}
 
         tables = []
         try:
             for index in destination.depends_on:
                 do_stage, do_database, do_table = Tables.parse_index(index)
                 tables = tables + self.lookup_table(
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
                     first_match=False,
+                    create_table=create_table
                 )
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
         for tbl in tables:
             source[tbl.table] = tbl
```

### Comparing `yetl-framework-1.3.6/yetl/config/_timeslice.py` & `yetl-framework-1.3.7.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/_utils.py` & `yetl-framework-1.3.7.dev1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/deltalake.py` & `yetl-framework-1.3.7.dev1/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/table/_deltalake.py` & `yetl-framework-1.3.7.dev1/yetl/config/table/_deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,38 +17,33 @@
 
 class DeltaLake(Table):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._spark = DeltaLakeFn(project=self.project)
         self._render()
-        if self.create_table:
-            self.create_delta_table()
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     _spark: DeltaLakeFn = PrivateAttr(default=None)
     depends_on: List[str] = Field(default=[])
     delta_properties: Dict[str, str] = Field(default=None)
     delta_constraints: Dict[str, str] = Field(default=None)
     partition_by: List[str] = Field(default=None)
     z_order_by: List[str] = Field(default=None)
-    create_table: bool = Field(default=True)
-    managed: bool = Field(default=False)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
     stage: StageType = Field(...)
     managed: bool = Field(default=False)
-    create_table: bool = Field(default=True)
     sql: str = Field(default=None)
 
     def _load_sql(self, path: str):
         path = abs_config_path(self.config_path, path)
         sql = load_text(path)
         return sql
 
@@ -90,15 +85,15 @@
             value = self.options.get("checkpointLocation")
             if value:
                 self.options["checkpointLocation"] = render_jinja(
                     value, self._replacements
                 )
 
     # TODO: Create or alter table
-    def create_delta_table(self):
+    def create_table(self):
         self._spark.create_database(self.database)
 
         if self.managed:
             self._spark.create_table(
                 database=self.database,
                 table=self.table,
                 delta_properties=self.delta_properties,
```

### Comparing `yetl-framework-1.3.6/yetl/config/table/_factory.py` & `yetl-framework-1.3.7.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl/config/table/_read.py` & `yetl-framework-1.3.7.dev1/yetl/config/table/_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
         self.path = os.path.join(self.location, self.filename)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
-    create_table: bool = Field(default=True)
     managed: bool = Field(default=False)
     trigger: str = Field(default=None)
     trigger_type: TriggerType = Field(default=None)
     filename: str = Field(...)
     filename_date_format: str = Field(...)
     path_date_format: str = Field(...)
     format: str = Field(...)
@@ -143,15 +142,15 @@
         columns_cnt = len(columns)
         ddls = len(self.ddl)
         if columns_cnt != ddls:
             raise Exception(
                 f"Headless files with schema hints must have a fully hinted schema since it must work positionally. Datasets!=dll({columns_cnt}!={ddls}"
             )
 
-        for i, c in enumerate(columns):
+        for i, _ in enumerate(columns):
             from_name = f"_c{i}"
             to_name = self.ddl[i].split(" ")[0].strip()
             logging.info(f"rename {from_name} to {to_name}")
             df: Union[StreamingQuery, DataFrame] = df.withColumnRenamed(
                 from_name, to_name
             )
```

### Comparing `yetl-framework-1.3.6/yetl/config/table/_table.py` & `yetl-framework-1.3.7.dev1/yetl/config/table/_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,7 +103,10 @@
                 return ValidationThreshold.default_select_sql()
 
         if threshold_type == ValidationThresholdType.warning:
             if self.warning_thresholds:
                 return self.warning_thresholds.select_sql()
             else:
                 return ValidationThreshold.default_select_sql()
+
+    def create_table(self):
+        pass
```

### Comparing `yetl-framework-1.3.6/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.3.7.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.6/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.3.7.dev1/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.6
+Version: 1.3.7.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -83,15 +83,14 @@
   delta_lake:
     # delta table properties can be set at stage level or table level
     delta_properties:
         delta.appendOnly: true
         delta.autoOptimize.autoCompact: true
         delta.autoOptimize.optimizeWrite: true
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: default
 
@@ -130,15 +129,14 @@
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
-    create_table: true
     container: datalake
     location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     checkpoint_location: "/mnt/{{container}}/checkpoint/{{checkpoint}}"
     options:
       mergeSchema: true
```

### Comparing `yetl-framework-1.3.6/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.3.7.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

