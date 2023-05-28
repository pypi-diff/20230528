# Comparing `tmp/lpr_pkg-2.0.3.tar.gz` & `tmp/lpr_pkg-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpr_pkg-2.0.3.tar", max compression
+gzip compressed data, was "lpr_pkg-2.0.4.tar", max compression
```

## Comparing `lpr_pkg-2.0.3.tar` & `lpr_pkg-2.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.3/README.md
--rw-r--r--   0        0        0      780 2023-05-28 08:35:53.019230 lpr_pkg-2.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.3/src/lpr_pkg/__init__.py
--rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.3/src/lpr_pkg/helpers.py
--rw-r--r--   0        0        0     4887 2023-05-28 08:35:44.487213 lpr_pkg-2.0.3/src/lpr_pkg/model_class.py
--rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.3/src/lpr_pkg/utils.py
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.4/README.md
+-rw-r--r--   0        0        0      780 2023-05-28 08:37:00.047416 lpr_pkg-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.4/src/lpr_pkg/__init__.py
+-rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.4/src/lpr_pkg/helpers.py
+-rw-r--r--   0        0        0     4845 2023-05-28 08:36:43.699362 lpr_pkg-2.0.4/src/lpr_pkg/model_class.py
+-rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.4/src/lpr_pkg/utils.py
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.4/PKG-INFO
```

### Comparing `lpr_pkg-2.0.3/README.md` & `lpr_pkg-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.3/pyproject.toml` & `lpr_pkg-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LPR_pkg"
-version = "2.0.3"
+version = "2.0.4"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 easydict = "1.9"
```

### Comparing `lpr_pkg-2.0.3/src/lpr_pkg/helpers.py` & `lpr_pkg-2.0.4/src/lpr_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.3/src/lpr_pkg/model_class.py` & `lpr_pkg-2.0.4/src/lpr_pkg/model_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,14 @@
         if self.mode == "local":
             ort_inputs = {session.get_inputs()[0].name: input}
             return session.run(None, ort_inputs)
         else:
             inputs = []
             outputs = []
             print(input.shape)
-            input = input[np.newaxis,...]
             inputs.append(grpcclient.InferInput("image", [1,96, 144, 3], "FP32"))
             inputs[0].set_data_from_numpy(input)
             print(input.shape)
 
             outputs.append(grpcclient.InferRequestedOutput("OCR_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Region_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Color_Output"))
```

### Comparing `lpr_pkg-2.0.3/src/lpr_pkg/utils.py` & `lpr_pkg-2.0.4/src/lpr_pkg/utils.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.3/PKG-INFO` & `lpr_pkg-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpr-pkg
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

