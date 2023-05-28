# Comparing `tmp/lpr_pkg-1.1.0.tar.gz` & `tmp/lpr_pkg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpr_pkg-1.1.0.tar", max compression
+gzip compressed data, was "lpr_pkg-2.0.0.tar", max compression
```

## Comparing `lpr_pkg-1.1.0.tar` & `lpr_pkg-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-1.1.0/README.md
--rw-r--r--   0        0        0      780 2023-05-28 05:17:33.948644 lpr_pkg-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-1.1.0/src/lpr_pkg/__init__.py
--rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-1.1.0/src/lpr_pkg/helpers.py
--rw-r--r--   0        0        0     4415 2023-05-28 04:49:56.214318 lpr_pkg-1.1.0/src/lpr_pkg/model_class.py
--rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-1.1.0/src/lpr_pkg/utils.py
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.0/README.md
+-rw-r--r--   0        0        0      780 2023-05-28 08:28:14.175479 lpr_pkg-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.0/src/lpr_pkg/__init__.py
+-rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.0/src/lpr_pkg/helpers.py
+-rw-r--r--   0        0        0     4782 2023-05-28 08:27:59.107236 lpr_pkg-2.0.0/src/lpr_pkg/model_class.py
+-rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.0/src/lpr_pkg/utils.py
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.0/PKG-INFO
```

### Comparing `lpr_pkg-1.1.0/README.md` & `lpr_pkg-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lpr_pkg-1.1.0/pyproject.toml` & `lpr_pkg-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LPR_pkg"
-version = "1.1.0"
+version = "2.0.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 easydict = "1.9"
```

### Comparing `lpr_pkg-1.1.0/src/lpr_pkg/helpers.py` & `lpr_pkg-2.0.0/src/lpr_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-1.1.0/src/lpr_pkg/model_class.py` & `lpr_pkg-2.0.0/src/lpr_pkg/model_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,20 +109,26 @@
         if self.mode == "local":
             ort_inputs = {session.get_inputs()[0].name: input}
             return session.run(None, ort_inputs)
         else:
             inputs = []
             outputs = []
 
-            inputs.append(grpcclient.InferInput("x", [1, 3, 512, 1024], "FP32"))
+            inputs.append(grpcclient.InferInput("image", [96, 144, 3], "FP32"))
             inputs[0].set_data_from_numpy(input)
 
-            outputs.append(grpcclient.InferRequestedOutput("softmax_0.tmp_0"))
+            outputs.append(grpcclient.InferRequestedOutput("OCR_Output"))
+            outputs.append(grpcclient.InferRequestedOutput("Region_Output"))
+            outputs.append(grpcclient.InferRequestedOutput("Color_Output"))
             results = session.infer(
                 model_name=self.triton_model_name,
                 inputs=inputs,
                 outputs=outputs,
                 headers={},
             )
-            output = results.as_numpy("softmax_0.tmp_0")
+            ocr_pred = results.as_numpy("OCR_Output")
+            region_pred = results.as_numpy("Region_Output")
+            color_pred = results.as_numpy("Color_Output")
+            output = (ocr_pred, region_pred, color_pred)
             print(output)
+            # ocr_pred, region_pred, color_pred
             return output
```

### Comparing `lpr_pkg-1.1.0/src/lpr_pkg/utils.py` & `lpr_pkg-2.0.0/src/lpr_pkg/utils.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-1.1.0/PKG-INFO` & `lpr_pkg-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpr-pkg
-Version: 1.1.0
+Version: 2.0.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

