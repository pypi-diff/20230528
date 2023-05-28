# Comparing `tmp/databand-1.0.8.1.tar.gz` & `tmp/databand-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databand-1.0.8.1.tar", last modified: Tue Nov 22 15:16:29 2022, max compression
+gzip compressed data, was "databand-1.0.9.1.tar", last modified: Tue Nov 22 16:26:56 2022, max compression
```

## Comparing `databand-1.0.8.1.tar` & `databand-1.0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:29.276154 databand-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 databand-1.0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4013 2022-11-22 15:16:29.276154 databand-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1826 2022-11-22 15:16:09.000000 databand-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9487 2022-11-22 15:16:09.000000 databand-1.0.8.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:29.277154 databand-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2536 2022-11-22 15:16:09.000000 databand-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:29.274154 databand-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:29.276154 databand-1.0.8.1/src/databand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4013 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1251 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:29.000000 databand-1.0.8.1/src/databand.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:56.051677 databand-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 databand-1.0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4013 2022-11-22 16:26:56.051677 databand-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2022-11-22 16:26:26.000000 databand-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9487 2022-11-22 16:26:26.000000 databand-1.0.9.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:56.052677 databand-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2022-11-22 16:26:26.000000 databand-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:56.048676 databand-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:56.051677 databand-1.0.9.1/src/databand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4013 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1251 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:56.000000 databand-1.0.9.1/src/databand.egg-info/top_level.txt
```

### Comparing `databand-1.0.8.1/LICENSE` & `databand-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databand-1.0.8.1/PKG-INFO` & `databand-1.0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databand
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

### Comparing `databand-1.0.8.1/README.md` & `databand-1.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `databand-1.0.8.1/pyproject.toml` & `databand-1.0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databand-1.0.8.1/setup.cfg` & `databand-1.0.9.1/setup.cfg`

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

### Comparing `databand-1.0.8.1/setup.py` & `databand-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `databand-1.0.8.1/src/databand.egg-info/PKG-INFO` & `databand-1.0.9.1/src/databand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databand
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

### Comparing `databand-1.0.8.1/src/databand.egg-info/requires.txt` & `databand-1.0.9.1/src/databand.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-dbnd==1.0.8.1
+dbnd==1.0.9.1
 
 [airflow]
-dbnd-airflow==1.0.8.1
+dbnd-airflow==1.0.9.1
 
 [airflow-auto-tracking]
-dbnd-airflow-auto-tracking==1.0.8.1
+dbnd-airflow-auto-tracking==1.0.9.1
 
 [airflow-export]
-dbnd-airflow-export==1.0.8.1
+dbnd-airflow-export==1.0.9.1
 
 [airflow-versioned-dag]
-dbnd-airflow-versioned-dag==1.0.8.1
+dbnd-airflow-versioned-dag==1.0.9.1
 
 [airflow_1_10_10]
-dbnd-airflow[airflow_1_10_10]==1.0.8.1
+dbnd-airflow[airflow_1_10_10]==1.0.9.1
 
 [airflow_1_10_11]
-dbnd-airflow[airflow_1_10_11]==1.0.8.1
+dbnd-airflow[airflow_1_10_11]==1.0.9.1
 
 [airflow_1_10_12]
-dbnd-airflow[airflow_1_10_12]==1.0.8.1
+dbnd-airflow[airflow_1_10_12]==1.0.9.1
 
 [airflow_1_10_13]
-dbnd-airflow[airflow_1_10_13]==1.0.8.1
+dbnd-airflow[airflow_1_10_13]==1.0.9.1
 
 [airflow_1_10_14]
-dbnd-airflow[airflow_1_10_14]==1.0.8.1
+dbnd-airflow[airflow_1_10_14]==1.0.9.1
 
 [airflow_1_10_15]
-dbnd-airflow[airflow_1_10_15]==1.0.8.1
+dbnd-airflow[airflow_1_10_15]==1.0.9.1
 
 [airflow_1_10_7]
-dbnd-airflow[airflow_1_10_7]==1.0.8.1
+dbnd-airflow[airflow_1_10_7]==1.0.9.1
 
 [airflow_1_10_8]
-dbnd-airflow[airflow_1_10_8]==1.0.8.1
+dbnd-airflow[airflow_1_10_8]==1.0.9.1
 
 [airflow_1_10_9]
-dbnd-airflow[airflow_1_10_9]==1.0.8.1
+dbnd-airflow[airflow_1_10_9]==1.0.9.1
 
 [airflow_bundle]
-dbnd-airflow[airflow]==1.0.8.1
+dbnd-airflow[airflow]==1.0.9.1
 
 [aws]
-dbnd-aws==1.0.8.1
+dbnd-aws==1.0.9.1
 
 [azure]
-dbnd-azure==1.0.8.1
+dbnd-azure==1.0.9.1
 
 [databricks]
-dbnd-databricks==1.0.8.1
+dbnd-databricks==1.0.9.1
 
 [docker]
-dbnd-docker==1.0.8.1
+dbnd-docker==1.0.9.1
 
 [gcp]
-dbnd-gcp==1.0.8.1
+dbnd-gcp==1.0.9.1
 
 [hdfs]
-dbnd-hdfs==1.0.8.1
+dbnd-hdfs==1.0.9.1
 
 [k8s]
-dbnd-docker==1.0.8.1
+dbnd-docker==1.0.9.1
 
 [luigi]
-dbnd-luigi==1.0.8.1
+dbnd-luigi==1.0.9.1
 
 [mlflow]
-dbnd-mlflow==1.0.8.1
+dbnd-mlflow==1.0.9.1
 
 [postgres]
-dbnd-postgres==1.0.8.1
+dbnd-postgres==1.0.9.1
 
 [qubole]
-dbnd-qubole==1.0.8.1
+dbnd-qubole==1.0.9.1
 
 [redshift]
-dbnd-redshift==1.0.8.1
+dbnd-redshift==1.0.9.1
 
 [snowflake]
-dbnd-snowflake==1.0.8.1
+dbnd-snowflake==1.0.9.1
 
 [spark]
-dbnd-spark==1.0.8.1
+dbnd-spark==1.0.9.1
 
 [tensorflow]
-dbnd-tensorflow==1.0.8.1
+dbnd-tensorflow==1.0.9.1
```

