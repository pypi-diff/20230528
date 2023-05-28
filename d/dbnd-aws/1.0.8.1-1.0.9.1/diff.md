# Comparing `tmp/dbnd-aws-1.0.8.1.tar.gz` & `tmp/dbnd-aws-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-aws-1.0.8.1.tar", last modified: Tue Nov 22 15:16:17 2022, max compression
+gzip compressed data, was "dbnd-aws-1.0.9.1.tar", last modified: Tue Nov 22 16:26:39 2022, max compression
```

## Comparing `dbnd-aws-1.0.8.1.tar` & `dbnd-aws-1.0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.546955 dbnd-aws-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 15:16:17.546955 dbnd-aws-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:17.547955 dbnd-aws-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      837 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.539955 dbnd-aws-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.542955 dbnd-aws-1.0.8.1/src/dbnd_aws/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.543955 dbnd-aws-1.0.8.1/src/dbnd_aws/batch/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/batch/aws_batch_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.544955 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7679 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_cluster_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.545955 dbnd-aws-1.0.8.1/src/dbnd_aws/fs/
--rw-rw-rw-   0 root         (0) root         (0)      244 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/fs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22225 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/fs/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.545955 dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4615 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/estimator_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/sagemaker_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/sagemaker_task.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2022-11-22 15:16:09.000000 dbnd-aws-1.0.8.1/src/dbnd_aws/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:17.543955 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      878 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      109 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-22 15:16:17.000000 dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.234949 dbnd-aws-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 16:26:39.234949 dbnd-aws-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:39.236950 dbnd-aws-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      837 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.224948 dbnd-aws-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.228949 dbnd-aws-1.0.9.1/src/dbnd_aws/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.230949 dbnd-aws-1.0.9.1/src/dbnd_aws/batch/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/batch/aws_batch_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.232949 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7679 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_cluster_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.232949 dbnd-aws-1.0.9.1/src/dbnd_aws/fs/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/fs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22225 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/fs/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.234949 dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4615 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/estimator_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/sagemaker_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/sagemaker_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2022-11-22 16:26:26.000000 dbnd-aws-1.0.9.1/src/dbnd_aws/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:39.230949 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1423 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      878 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      109 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-22 16:26:39.000000 dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/top_level.txt
```

### Comparing `dbnd-aws-1.0.8.1/LICENSE` & `dbnd-aws-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/PKG-INFO` & `dbnd-aws-1.0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-aws
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

### Comparing `dbnd-aws-1.0.8.1/setup.cfg` & `dbnd-aws-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-aws-1.0.8.1/setup.py` & `dbnd-aws-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/_plugin.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/batch/aws_batch_ctrl.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/batch/aws_batch_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/credentials.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_cluster.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_cluster.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_cluster_builder.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_cluster_builder.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_config.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_ctrl.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/emr/emr_step.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/emr/emr_step.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/env.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/env.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/fs/s3.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/fs/s3.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/estimator_config.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/estimator_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/sagemaker_ctrl.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/sagemaker_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws/sagemaker/sagemaker_task.py` & `dbnd-aws-1.0.9.1/src/dbnd_aws/sagemaker/sagemaker_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/PKG-INFO` & `dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-aws
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

### Comparing `dbnd-aws-1.0.8.1/src/dbnd_aws.egg-info/SOURCES.txt` & `dbnd-aws-1.0.9.1/src/dbnd_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

