# Comparing `tmp/dbnd-postgres-1.0.8.1.tar.gz` & `tmp/dbnd-postgres-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-postgres-1.0.8.1.tar", last modified: Tue Nov 22 15:16:24 2022, max compression
+gzip compressed data, was "dbnd-postgres-1.0.9.1.tar", last modified: Tue Nov 22 16:26:48 2022, max compression
```

## Comparing `dbnd-postgres-1.0.8.1.tar` & `dbnd-postgres-1.0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.099625 dbnd-postgres-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 15:16:24.100625 dbnd-postgres-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      300 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:24.101625 dbnd-postgres-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      492 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.096625 dbnd-postgres-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.098625 dbnd-postgres-1.0.8.1/src/dbnd_postgres/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/log_pg_table_operator.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/postgres_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8902 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/postgres_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2022-11-22 15:16:09.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres/postgres_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:24.099625 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      509 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 15:16:24.000000 dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:48.609910 dbnd-postgres-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 16:26:48.609910 dbnd-postgres-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      300 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:48.610911 dbnd-postgres-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      492 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:48.605910 dbnd-postgres-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:48.607910 dbnd-postgres-1.0.9.1/src/dbnd_postgres/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/log_pg_table_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/postgres_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/postgres_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2022-11-22 16:26:26.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres/postgres_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:48.608910 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      509 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 16:26:48.000000 dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/top_level.txt
```

### Comparing `dbnd-postgres-1.0.8.1/LICENSE` & `dbnd-postgres-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-postgres-1.0.8.1/PKG-INFO` & `dbnd-postgres-1.0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-postgres
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-postgres-1.0.8.1/setup.cfg` & `dbnd-postgres-1.0.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.8.1
+version = 1.0.9.1
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-postgres-1.0.8.1/src/dbnd_postgres/log_pg_table_operator.py` & `dbnd-postgres-1.0.9.1/src/dbnd_postgres/log_pg_table_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-postgres-1.0.8.1/src/dbnd_postgres/postgres_controller.py` & `dbnd-postgres-1.0.9.1/src/dbnd_postgres/postgres_controller.py`

 * *Files identical despite different names*

### Comparing `dbnd-postgres-1.0.8.1/src/dbnd_postgres/postgres_values.py` & `dbnd-postgres-1.0.9.1/src/dbnd_postgres/postgres_values.py`

 * *Files identical despite different names*

### Comparing `dbnd-postgres-1.0.8.1/src/dbnd_postgres.egg-info/PKG-INFO` & `dbnd-postgres-1.0.9.1/src/dbnd_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-postgres
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

