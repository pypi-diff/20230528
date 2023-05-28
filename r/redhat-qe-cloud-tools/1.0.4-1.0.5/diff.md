# Comparing `tmp/redhat_qe_cloud_tools-1.0.4.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.4.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.5.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.4.tar` & `redhat_qe_cloud_tools-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/LICENSE
--rw-r--r--   0        0        0      845 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-24 07:19:50.881588 redhat_qe_cloud_tools-1.0.4/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/__init__.py
--rw-r--r--   0        0        0      455 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/README.md
--rw-r--r--   0        0        0        0 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/aws_roles.py
--rw-r--r--   0        0        0     1893 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     6218 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      782 2023-05-24 07:19:50.882588 redhat_qe_cloud_tools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     1893 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     6218 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      782 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.5/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.4/LICENSE` & `redhat_qe_cloud_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/README.md` & `redhat_qe_cloud_tools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.5/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_roles/aws_roles.py` & `redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/roles.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.5/clouds/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.5/clouds/aws/delete_s3_velero_bucket.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.4/pyproject.toml` & `redhat_qe_cloud_tools-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.4"
+version = "1.0.5"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
```

### Comparing `redhat_qe_cloud_tools-1.0.4/PKG-INFO` & `redhat_qe_cloud_tools-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

