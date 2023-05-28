# Comparing `tmp/lpr_pkg-2.0.1.tar.gz` & `tmp/lpr_pkg-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpr_pkg-2.0.1.tar", max compression
+gzip compressed data, was "lpr_pkg-2.0.2.tar", max compression
```

## Comparing `lpr_pkg-2.0.1.tar` & `lpr_pkg-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.1/README.md
--rw-r--r--   0        0        0      780 2023-05-28 08:30:11.289357 lpr_pkg-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.1/src/lpr_pkg/__init__.py
--rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.1/src/lpr_pkg/helpers.py
--rw-r--r--   0        0        0     4811 2023-05-28 08:30:05.113258 lpr_pkg-2.0.1/src/lpr_pkg/model_class.py
--rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.1/src/lpr_pkg/utils.py
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.2/README.md
+-rw-r--r--   0        0        0      780 2023-05-28 08:33:35.671172 lpr_pkg-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.2/src/lpr_pkg/__init__.py
+-rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.2/src/lpr_pkg/helpers.py
+-rw-r--r--   0        0        0     4825 2023-05-28 08:33:24.491190 lpr_pkg-2.0.2/src/lpr_pkg/model_class.py
+-rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.2/src/lpr_pkg/utils.py
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.2/PKG-INFO
```

### Comparing `lpr_pkg-2.0.1/README.md` & `lpr_pkg-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.1/pyproject.toml` & `lpr_pkg-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LPR_pkg"
-version = "2.0.1"
+version = "2.0.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 easydict = "1.9"
```

### Comparing `lpr_pkg-2.0.1/src/lpr_pkg/helpers.py` & `lpr_pkg-2.0.2/src/lpr_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.1/src/lpr_pkg/model_class.py` & `lpr_pkg-2.0.2/src/lpr_pkg/model_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         session = self.__prepare_session()
         if self.mode == "local":
             ort_inputs = {session.get_inputs()[0].name: input}
             return session.run(None, ort_inputs)
         else:
             inputs = []
             outputs = []
-            input = [input]
+            input = input[np.newaxis,...]
             inputs.append(grpcclient.InferInput("image", [1,96, 144, 3], "FP32"))
             inputs[0].set_data_from_numpy(input)
 
             outputs.append(grpcclient.InferRequestedOutput("OCR_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Region_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Color_Output"))
             results = session.infer(
```

### Comparing `lpr_pkg-2.0.1/src/lpr_pkg/utils.py` & `lpr_pkg-2.0.2/src/lpr_pkg/utils.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.1/PKG-INFO` & `lpr_pkg-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpr-pkg
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

