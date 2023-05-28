# Comparing `tmp/easytorch-3.7.9.tar.gz` & `tmp/easytorch-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.9.tar", last modified: Sun May 28 01:34:24 2023, max compression
+gzip compressed data, was "easytorch-3.8.0.tar", last modified: Sun May 28 12:25:50 2023, max compression
```

## Comparing `easytorch-3.7.9.tar` & `easytorch-3.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 01:34:11.000000 easytorch-3.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 01:34:24.450652 easytorch-3.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-28 01:34:11.000000 easytorch-3.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.446653 easytorch-3.7.9/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.446653 easytorch-3.7.9/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 01:34:24.450652 easytorch-3.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-28 01:34:11.000000 easytorch-3.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 12:25:34.000000 easytorch-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 12:25:50.607754 easytorch-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-28 12:25:34.000000 easytorch-3.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-28 12:25:34.000000 easytorch-3.8.0/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:25:50.607754 easytorch-3.8.0/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 12:25:50.000000 easytorch-3.8.0/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 12:25:50.000000 easytorch-3.8.0/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:25:50.000000 easytorch-3.8.0/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 12:25:50.000000 easytorch-3.8.0/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 12:25:50.000000 easytorch-3.8.0/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:25:50.607754 easytorch-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-28 12:25:34.000000 easytorch-3.8.0/setup.py
```

### Comparing `easytorch-3.7.9/LICENSE` & `easytorch-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/PKG-INFO` & `easytorch-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.9
+Version: 3.8.0
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.9/README.md` & `easytorch-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/config/__init__.py` & `easytorch-3.8.0/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/config/state.py` & `easytorch-3.8.0/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/data/data.py` & `easytorch-3.8.0/easytorch/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             files = sorted(files)
             if self.conf['phase'] == Phase.INFERENCE:
                 split = {Phase.INFERENCE: files}
 
             else:
                 split = _du.create_ratio_split(files, self.conf['split_ratio'])
 
-        _spl = self.conf['save_dir'] + _sep + f"SPLIT_{_Path(self.conf['save_dir']).name}_{self.conf['name']}.json"
+        _spl = self.conf['save_dir'] + _sep + f"SPLIT_{self.conf['name']}.json"
         with open(_spl, 'w') as fw:
             _json.dump(split, fw)
 
         for k in split:
             info(f" - Data count: {len(split[k])}, phase:{k}", self.conf['verbose'])
 
         return split
```

### Comparing `easytorch-3.7.9/easytorch/data/datautils.py` & `easytorch-3.8.0/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/data/multiproc.py` & `easytorch-3.8.0/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/easytorch.py` & `easytorch-3.8.0/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/metrics/loss.py` & `easytorch-3.8.0/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/metrics/metrics.py` & `easytorch-3.8.0/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/runner.py` & `easytorch-3.8.0/easytorch/runner.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/utils/__init__.py` & `easytorch-3.8.0/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/utils/ddp_check.py` & `easytorch-3.8.0/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/utils/tensorutils.py` & `easytorch-3.8.0/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/vision/imageutils.py` & `easytorch-3.8.0/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/vision/plotter.py` & `easytorch-3.8.0/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch/vision/transforms.py` & `easytorch-3.8.0/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/easytorch.egg-info/PKG-INFO` & `easytorch-3.8.0/easytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.9
+Version: 3.8.0
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.9/easytorch.egg-info/SOURCES.txt` & `easytorch-3.8.0/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.9/setup.py` & `easytorch-3.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.9",
+    version="3.8.0",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

