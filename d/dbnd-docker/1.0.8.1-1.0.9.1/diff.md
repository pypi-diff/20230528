# Comparing `tmp/dbnd-docker-1.0.8.1.tar.gz` & `tmp/dbnd-docker-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-docker-1.0.8.1.tar", last modified: Tue Nov 22 15:16:21 2022, max compression
+gzip compressed data, was "dbnd-docker-1.0.9.1.tar", last modified: Tue Nov 22 16:26:44 2022, max compression
```

## Comparing `dbnd-docker-1.0.8.1.tar` & `dbnd-docker-1.0.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.207329 dbnd-docker-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1404 2022-11-22 15:16:21.207329 dbnd-docker-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:21.208330 dbnd-docker-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.199329 dbnd-docker-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.202329 dbnd-docker-1.0.8.1/src/dbnd_docker/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/container_engine_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.204329 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_engine_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_task_run_ctrl.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/docker_ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.205329 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.206329 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/pod_launcher.py
--rw-rw-rw-   0 root         (0) root         (0)     7766 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/pod_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/secrets_shim.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/volume_shims.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/dns1123_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)    17497 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kube_dbnd_client.py
--rw-rw-rw-   0 root         (0) root         (0)     5844 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kube_resources_checker.py
--rw-rw-rw-   0 root         (0) root         (0)    29018 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kubernetes_engine_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kubernetes_task_run_ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.206329 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/dbnd_extended_resources.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2022-11-22 15:16:09.000000 dbnd-docker-1.0.8.1/src/dbnd_docker/submit_ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:21.203329 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1404 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1421 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       86 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 15:16:21.000000 dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.463485 dbnd-docker-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-11-22 16:26:44.464486 dbnd-docker-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:44.465485 dbnd-docker-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      630 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.453484 dbnd-docker-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.456485 dbnd-docker-1.0.9.1/src/dbnd_docker/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/container_engine_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.460485 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_engine_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_task_run_ctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/docker_ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.461485 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.463485 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/pod_launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     7766 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/pod_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/secrets_shim.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/volume_shims.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/dns1123_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    17497 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kube_dbnd_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kube_resources_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)    29018 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kubernetes_engine_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kubernetes_task_run_ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.463485 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/dbnd_extended_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2022-11-22 16:26:26.000000 dbnd-docker-1.0.9.1/src/dbnd_docker/submit_ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:44.458485 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       86 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-11-22 16:26:44.000000 dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/top_level.txt
```

### Comparing `dbnd-docker-1.0.8.1/LICENSE` & `dbnd-docker-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/PKG-INFO` & `dbnd-docker-1.0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-docker
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

### Comparing `dbnd-docker-1.0.8.1/setup.cfg` & `dbnd-docker-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-docker-1.0.8.1/setup.py` & `dbnd-docker-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/_plugin.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/container_engine_config.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/container_engine_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_build.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_build.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_engine_config.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_engine_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_task.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/docker/docker_task_run_ctrl.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/docker/docker_task_run_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/pod_reconciler.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/pod_reconciler.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/secrets_shim.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/secrets_shim.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/compat/volume_shims.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/compat/volume_shims.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/dns1123_clean_names.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/dns1123_clean_names.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kube_dbnd_client.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kube_dbnd_client.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kube_resources_checker.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kube_resources_checker.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kubernetes_engine_config.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kubernetes_engine_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/kubernetes_task_run_ctrl.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/kubernetes_task_run_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/dbnd_extended_resources.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/dbnd_extended_resources.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/kubernetes/vendorized_airflow/request_factory.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/kubernetes/vendorized_airflow/request_factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker/submit_ctrl.py` & `dbnd-docker-1.0.9.1/src/dbnd_docker/submit_ctrl.py`

 * *Files identical despite different names*

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/PKG-INFO` & `dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-docker
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

### Comparing `dbnd-docker-1.0.8.1/src/dbnd_docker.egg-info/SOURCES.txt` & `dbnd-docker-1.0.9.1/src/dbnd_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

