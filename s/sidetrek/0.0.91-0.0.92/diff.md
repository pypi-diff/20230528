# Comparing `tmp/sidetrek-0.0.91.tar.gz` & `tmp/sidetrek-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.91.tar", max compression
+gzip compressed data, was "sidetrek-0.0.92.tar", max compression
```

## Comparing `sidetrek-0.0.91.tar` & `sidetrek-0.0.92.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.91/README.md
--rw-r--r--   0        0        0      776 2023-05-27 14:53:06.799077 sidetrek-0.0.91/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.91/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.91/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.91/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    10270 2023-05-26 21:33:27.204243 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2857 2023-05-26 23:29:03.067762 sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.91/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    11999 2023-05-26 21:33:20.619575 sidetrek-0.0.91/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     3937 2023-05-27 14:53:02.645504 sidetrek-0.0.91/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.91/sidetrek/collect_env.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.91/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.91/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-26 15:36:54.943156 sidetrek-0.0.91/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.91/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.91/sidetrek/global_fns.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.91/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.91/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.91/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 sidetrek-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.92/README.md
+-rw-r--r--   0        0        0      619 2023-05-28 01:34:20.320700 sidetrek-0.0.92/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.92/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.92/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.92/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    10270 2023-05-26 21:33:27.204243 sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2857 2023-05-26 23:29:03.067762 sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.92/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    11999 2023-05-26 21:33:20.619575 sidetrek-0.0.92/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     4193 2023-05-27 21:18:22.800776 sidetrek-0.0.92/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.92/sidetrek/collect_env.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.92/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.92/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.92/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.92/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.92/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.92/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.92/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.92/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 sidetrek-0.0.92/PKG-INFO
```

### Comparing `sidetrek-0.0.91/pyproject.toml` & `sidetrek-0.0.92/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.91"
+version = "0.0.92"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 typer = {extras = ["all"], version = "^0.7.0"}
-numba = "^0.56.4" # Required for mlflow: mlflow depends on old version of numba which won't install via poetry, so we had to manually include it here
-mlflow = "^2.0"
-flytekit = "^1.2.10,<=1.4.2"
 requests = "^2.28.2"
 pylint = "^2.17.0"
 torchdata = "^0.6.0"
 fsspec = "^2023.4.0"
 s3fs = "^2023.4.0"
 bentoml = "^1.0.20"
+mlflow = "^2.3.2"
+flytekit = "^1.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sidetrek-0.0.91/sidetrek/__init__.py` & `sidetrek-0.0.92/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/cli.py` & `sidetrek-0.0.92/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.92/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.92/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.92/sidetrek/cli_commands/workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import json
 import time
 import threading
 from pathlib import Path
 import typer
 import subprocess
 from time import sleep
 from rich import print
@@ -35,44 +36,45 @@
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
     ) as progress:
         print("generated_local_sidetrek_dir_path", get_generated_local_sidetrek_dir_path())
 
-        # # Add a timer
-        # print_timer()
-
         # Get current user
         auth_step = progress.add_task(description="Authenticating...", total=None)
         current_user = get_current_user()
         print(f"current_user={current_user}")
+
+        # Get aws credentials and set it as env var for execution (grants temporary local s3 access for datasets)
+        aws_creds = get_aws_creds()
+        if aws_creds is None:
+            raise Exception("Failed to get aws credentials")
+        aws_env = {**os.environ, "AWS_ACCESS_KEY_ID": aws_creds["AccessKeyId"], "AWS_SECRET_ACCESS_KEY": aws_creds["SecretKey"], "AWS_SESSION_TOKEN": aws_creds["SessionToken"]}
+
         progress.remove_task(auth_step)
         time_elapsed = round(time.time() - start_time, 2)
         print(f"[green]✔️ [white]Authenticated [grey89]({time_elapsed}s)")
 
         # Always use the draft version for testing
         wf_generation_step = progress.add_task(description="Generating the workflow...", total=None)
         workflow_version = get_workflow_draft_version(workflow_id=workflow_id)
         # print(f"workflow_version={workflow_version}")
 
+        # Check dataset auth - i.e. make sure this user has access to the dataset they're trying to access
+        wf_ui = json.loads(workflow_version["ui"])
+        wf_dataset_ids = [node.get("data", {}).get("datasetId") for node in wf_ui["nodes"] if node["type"] == "dataset"]
+
         # Generate the workflow file
         wf_file_path = download_generated_flyte_workflow(user_id=current_user["id"], workflow_version=workflow_version)
         generated_wf_name = get_generated_workflow_name(workflow_id)
         progress.remove_task(wf_generation_step)
         time_elapsed = round(time.time() - start_time, 2)
         print(f"[green]✔️ [white]Workflow generated [grey89]({time_elapsed}s) - {wf_file_path.as_posix()}")
 
-        # Get aws credentials and set it as env var for execution (grants temporary local s3 access)
-        aws_creds = get_aws_creds()
-        if aws_creds is None:
-            raise Exception("Failed to get aws credentials")
-
-        aws_env = {**os.environ, "AWS_ACCESS_KEY_ID": aws_creds["AccessKeyId"], "AWS_SECRET_ACCESS_KEY": aws_creds["SecretKey"], "AWS_SESSION_TOKEN": aws_creds["SessionToken"]}
-
         wf_execution_step = progress.add_task(description="Executing the workflow...", total=None)
         # print(" ".join(["pyflyte", "run", wf_file_path.as_posix(), generated_wf_name, "--_wf_args", workflow_args]))
         with subprocess.Popen(
             ["pyflyte", "run", wf_file_path, generated_wf_name, "--_wf_args", workflow_args],
             cwd=get_generated_local_sidetrek_dir_path(),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
```

### Comparing `sidetrek-0.0.91/sidetrek/collect_env.py` & `sidetrek-0.0.92/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/datapipes.py` & `sidetrek-0.0.92/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/dataset.py` & `sidetrek-0.0.92/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/global_fns.py` & `sidetrek-0.0.92/sidetrek/global_fns.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/loggers.py` & `sidetrek-0.0.92/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/sidetrek/types/dataset.py` & `sidetrek-0.0.92/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.91/PKG-INFO` & `sidetrek-0.0.92/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.91
+Version: 0.0.92
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bentoml (>=1.0.20,<2.0.0)
-Requires-Dist: flytekit (>=1.2.10,<=1.4.2)
+Requires-Dist: flytekit (>=1.6.1,<2.0.0)
 Requires-Dist: fsspec (>=2023.4.0,<2024.0.0)
-Requires-Dist: mlflow (>=2.0,<3.0)
-Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: pylint (>=2.17.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: s3fs (>=2023.4.0,<2024.0.0)
 Requires-Dist: torchdata (>=0.6.0,<0.7.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

