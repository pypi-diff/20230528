# Comparing `tmp/dbnd-spark-1.0.8.1.tar.gz` & `tmp/dbnd-spark-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-spark-1.0.8.1.tar", last modified: Tue Nov 22 15:16:26 2022, max compression
+gzip compressed data, was "dbnd-spark-1.0.9.1.tar", last modified: Tue Nov 22 16:26:52 2022, max compression
```

## Comparing `dbnd-spark-1.0.8.1.tar` & `dbnd-spark-1.0.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.337854 dbnd-spark-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 15:16:26.337854 dbnd-spark-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:26.337854 dbnd-spark-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      552 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.329853 dbnd-spark-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.332853 dbnd-spark-1.0.8.1/src/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.333853 dbnd-spark-1.0.8.1/src/dbnd_spark/_core/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1604 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_core/spark_error_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.334853 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 15:16:10.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.334853 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/
--rw-rw-rw-   0 root         (0) root         (0)    10850 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 15:16:10.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4843 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    24389 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/spark_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/deequ_metrics_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.335853 dbnd-spark-1.0.8.1/src/dbnd_spark/livy/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/livy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4140 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8108 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_spark.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_spark_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.336854 dbnd-spark-1.0.8.1/src/dbnd_spark/local/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/local/local_spark.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/local/local_spark_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8848 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)     7042 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.336854 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/spark_marshalling.py
--rw-rw-rw-   0 root         (0) root         (0)     7155 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/spark_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.336854 dbnd-spark-1.0.8.1/src/dbnd_spark/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-spark-1.0.8.1/src/dbnd_spark/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:26.333853 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 15:16:26.000000 dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.034262 dbnd-spark-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      222 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 16:26:52.034262 dbnd-spark-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:52.035262 dbnd-spark-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      552 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.020260 dbnd-spark-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.026261 dbnd-spark-1.0.9.1/src/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.029261 dbnd-spark-1.0.9.1/src/dbnd_spark/_core/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_core/spark_error_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.029261 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 16:26:28.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.030261 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/
+-rw-rw-rw-   0 root         (0) root         (0)    10850 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 16:26:28.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    24389 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/spark_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/deequ_metrics_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.032261 dbnd-spark-1.0.9.1/src/dbnd_spark/livy/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/livy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4140 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8108 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_spark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_spark_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.033262 dbnd-spark-1.0.9.1/src/dbnd_spark/local/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/local/local_spark.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/local/local_spark_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8848 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     7042 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.033262 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/spark_marshalling.py
+-rw-rw-rw-   0 root         (0) root         (0)     7155 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/spark_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.034262 dbnd-spark-1.0.9.1/src/dbnd_spark/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-spark-1.0.9.1/src/dbnd_spark/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:52.028261 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1425 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 16:26:51.000000 dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/top_level.txt
```

### Comparing `dbnd-spark-1.0.8.1/LICENSE` & `dbnd-spark-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/PKG-INFO` & `dbnd-spark-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-spark
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

### Comparing `dbnd-spark-1.0.8.1/setup.cfg` & `dbnd-spark-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-spark-1.0.8.1/setup.py` & `dbnd-spark-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/__init__.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/_core/spark_error_parser.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/_core/spark_error_parser.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/_plugin.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/LICENSE` & `dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/connection.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/connection.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/_vendor/airflow/spark_hook.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/_vendor/airflow/spark_hook.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/deequ_metrics_repository.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/deequ_metrics_repository.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_batch.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_batch.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_spark.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/livy/livy_spark_config.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/livy/livy_spark_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/local/local_spark.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/local/local_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/local/local_spark_config.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/local/local_spark_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_bootstrap.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_config.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_ctrl.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_listener.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_listener.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_session.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_session.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/__init__.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/spark_marshalling.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/spark_marshalling.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark/spark_targets/spark_values.py` & `dbnd-spark-1.0.9.1/src/dbnd_spark/spark_targets/spark_values.py`

 * *Files identical despite different names*

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/PKG-INFO` & `dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-spark
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

### Comparing `dbnd-spark-1.0.8.1/src/dbnd_spark.egg-info/SOURCES.txt` & `dbnd-spark-1.0.9.1/src/dbnd_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

