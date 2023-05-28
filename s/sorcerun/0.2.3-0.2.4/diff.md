# Comparing `tmp/sorcerun-0.2.3.tar.gz` & `tmp/sorcerun-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.3.tar", last modified: Fri May 26 23:48:11 2023, max compression
+gzip compressed data, was "sorcerun-0.2.4.tar", last modified: Sun May 28 08:29:08 2023, max compression
```

## Comparing `sorcerun-0.2.3.tar` & `sorcerun-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 23:47:58.000000 sorcerun-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 23:48:11.979192 sorcerun-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 23:47:58.000000 sorcerun-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:48:11.979192 sorcerun-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 23:47:58.000000 sorcerun-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-28 08:28:55.000000 sorcerun-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 08:29:08.815688 sorcerun-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-28 08:28:55.000000 sorcerun-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 08:29:08.815688 sorcerun-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-28 08:28:55.000000 sorcerun-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.3/LICENSE` & `sorcerun-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.3/PKG-INFO` & `sorcerun-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.3
+Version: 0.2.4
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.3/README.md` & `sorcerun-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.3/setup.py` & `sorcerun-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.3/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.4/sorcerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.3
+Version: 0.2.4
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.3/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.4/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.3/sorcerun_package/cli.py` & `sorcerun-0.2.4/sorcerun_package/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,20 @@
         config = yaml.safe_load(file)
 
     for k, v in config.items():
         if type(v) != list:
             config[k] = [v]
 
     param_grid = ParameterGrid([config])
-    print(f"Parameter grid contains {len(param_grid)} combinations")
+    total_num_params = len(param_grid)
+    print(f"Parameter grid contains {total_num_params} combinations")
 
     # Run the Sacred experiment with the provided adapter function and config
-    for param in param_grid:
-        print(f"Running with config:\n{param}")
+    for i, param in enumerate(param_grid):
+        print(f"Run {i+1}/{total_num_params} with config:\n{param}")
         run_sacred_experiment(adapter_func, param, auth_path)
 
 
 @sorcerun.group()
 def mongo():
     pass
 
@@ -123,14 +124,23 @@
     except subprocess.CalledProcessError as e:
         click.echo(f"Error occurred while running Omniboard: {e}")
 
 
 @sorcerun.command()
 def screen():
     screen_session_name = "sorcerun"
+
+    # result = subprocess.Popen("screen -ls", shell=True, stdout=subprocess.PIPE)
+    # output = "\n".join(str(a) for a in result.stdout.readlines())
+
+    # click.echo(output)
+    # if screen_session_name in output:
+    #     click.echo(f"Screen session '{screen_session_name}' already exists.")
+    #     return
+
     # Check if in conda environment
     conda_env = os.environ.get("CONDA_DEFAULT_ENV", None)
     activate_conda = f"conda activate {conda_env}\n" if conda_env else ""
 
     # Start new detached screen session
     screen_command = ["screen", "-dmS", screen_session_name]
     subprocess.Popen(screen_command)
```

### Comparing `sorcerun-0.2.3/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.4/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.3/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.4/sorcerun_package/sacred_utils.py`

 * *Files identical despite different names*

