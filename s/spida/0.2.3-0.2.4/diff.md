# Comparing `tmp/spida-0.2.3.tar.gz` & `tmp/spida-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.2.3.tar", last modified: Fri May 26 21:03:04 2023, max compression
+gzip compressed data, was "spida-0.2.4.tar", last modified: Sun May 28 19:05:17 2023, max compression
```

## Comparing `spida-0.2.3.tar` & `spida-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 21:03:04.827109 spida-0.2.3/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6854 2023-05-26 21:03:04.826102 spida-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6396 2023-05-26 20:57:16.000000 spida-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 21:03:04.827109 spida-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-26 21:02:09.000000 spida-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:03:04.779735 spida-0.2.3/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.3/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:03:04.818056 spida-0.2.3/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-26 19:59:37.000000 spida-0.2.3/spida/data/config.json
--rw-rw-rw-   0        0        0    16254 2023-05-26 19:17:58.000000 spida-0.2.3/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:03:04.824084 spida-0.2.3/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.3/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.2.3/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.2.3/spida/utils/misc.py
--rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.3/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:03:04.816042 spida-0.2.3/spida.egg-info/
--rw-rw-rw-   0        0        0     6854 2023-05-26 21:03:04.000000 spida-0.2.3/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-26 21:03:04.000000 spida-0.2.3/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 21:03:04.000000 spida-0.2.3/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-26 21:03:04.000000 spida-0.2.3/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 21:03:04.000000 spida-0.2.3/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.508336 spida-0.2.4/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-28 19:05:17.507148 spida-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:05:17.508336 spida-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-28 19:02:39.000000 spida-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.464731 spida-0.2.4/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.4/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.496319 spida-0.2.4/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-28 19:01:46.000000 spida-0.2.4/spida/data/config.json
+-rw-rw-rw-   0        0        0    16560 2023-05-28 18:51:43.000000 spida-0.2.4/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.504045 spida-0.2.4/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.4/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.2.4/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.2.4/spida/utils/misc.py
+-rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.4/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.494320 spida-0.2.4/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/top_level.txt
```

### Comparing `spida-0.2.3/LICENSE` & `spida-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.2.3/PKG-INFO` & `spida-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -84,21 +84,15 @@
 
 Spida supports the ControlNet extension, which allows for conditioning the generation process using ControlNet modules. You can use the `annotate()` function to annotate a batch of images using a specified ControlNet module:
 
 ```python
 annotated_images = spida.annotate(images, annotator="controlnet_module")
 ```
 
-The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation. An `annotated_image` from `annotated_images` can be passed into the ControlNet unit settings using the `cnet_settings()` function:
-
-```python
-cnet_sets = spida.cnet_settings(annotated_image, annotator="controlnet_module")
-```
-
-This function returns a dictionary containing the settings for a ControlNet unit. You can customize various parameters such as the model, weight, resolution, thresholds, control mode, resize mode, and more. Now, if you set the `cnet_settings` parameter in `txt2img()` to `cnet_sets`, the image generation process will be conditioned by the ControlNet.
+The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation.
 
 ### Retrieving Info
 
 Spida has multiple functions for retrieving information, they are listed here:
 
 ```python
 # get functions
@@ -181,24 +175,21 @@
 
 # Set the Stable Diffusion model
 spida.model("model_name")
 
 # Create an image to annotate
 imgs = spida.txt2img("chair")
 
-# Annotate the image using ControlNet
-depth = spida.annotate(imgs, annotator="depth")[0]
-
 # Generate the settings for a ControlNet unit
-cset = spida.cnet_settings(depth, annotator="depth")
+cset = spida.cnet_settings(imgs[0])
 
 # Use the settings for conditioning the generation process
 results = spida.txt2img("chair", cnet_settings=cset)
 
 # Create and display a grid showing each step of the process
-grid = spida.grid_img(np.array([imgs[0], spida.gray2rgb(depth), results[0]]), (1, None))
+grid = spida.grid_img(np.array([imgs[0], results[1], results[0]]), (1, None))
 spida.show(grid)
 ```
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

### Comparing `spida-0.2.3/README.md` & `spida-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,21 +70,15 @@
 
 Spida supports the ControlNet extension, which allows for conditioning the generation process using ControlNet modules. You can use the `annotate()` function to annotate a batch of images using a specified ControlNet module:
 
 ```python
 annotated_images = spida.annotate(images, annotator="controlnet_module")
 ```
 
-The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation. An `annotated_image` from `annotated_images` can be passed into the ControlNet unit settings using the `cnet_settings()` function:
-
-```python
-cnet_sets = spida.cnet_settings(annotated_image, annotator="controlnet_module")
-```
-
-This function returns a dictionary containing the settings for a ControlNet unit. You can customize various parameters such as the model, weight, resolution, thresholds, control mode, resize mode, and more. Now, if you set the `cnet_settings` parameter in `txt2img()` to `cnet_sets`, the image generation process will be conditioned by the ControlNet.
+The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation.
 
 ### Retrieving Info
 
 Spida has multiple functions for retrieving information, they are listed here:
 
 ```python
 # get functions
@@ -167,24 +161,21 @@
 
 # Set the Stable Diffusion model
 spida.model("model_name")
 
 # Create an image to annotate
 imgs = spida.txt2img("chair")
 
-# Annotate the image using ControlNet
-depth = spida.annotate(imgs, annotator="depth")[0]
-
 # Generate the settings for a ControlNet unit
-cset = spida.cnet_settings(depth, annotator="depth")
+cset = spida.cnet_settings(imgs[0])
 
 # Use the settings for conditioning the generation process
 results = spida.txt2img("chair", cnet_settings=cset)
 
 # Create and display a grid showing each step of the process
-grid = spida.grid_img(np.array([imgs[0], spida.gray2rgb(depth), results[0]]), (1, None))
+grid = spida.grid_img(np.array([imgs[0], results[1], results[0]]), (1, None))
 spida.show(grid)
 ```
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

### Comparing `spida-0.2.3/setup.py` & `spida-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.2.3/spida/stable_diffusion.py` & `spida-0.2.4/spida/stable_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     dsts[0] = dst
     for i, v in enumerate(dsts_b64strs[1:], start=1):
         dsts[i] = utils.img.b64str2img(v)
     return dsts
 
 
 def cnet_settings(
-    annotated_img: np.ndarray,
+    img: np.ndarray,
     annotator: str = "depth",
     model: str = None,
     weight: float = 1.0,
     resolution: int = None,
     thresholds: tuple = (None, None),
     control_mode: int = 0,
     resize_mode: int = 1,
@@ -294,18 +294,18 @@
     search: bool = True,
 ):
     """
     Generates the settings for a ControlNet unit.
 
     Parameters
     ----------
-    annotated_img : numpy.ndarray
-        Annotated image to be used as input for the ControlNet unit.
+    img : numpy.ndarray
+        Image to be used as input for the ControlNet unit.
     annotator : str, optional
-        Preprocessor to use on the input image. Defaults to "depth".
+        The ControlNet module used for the annotation. Defaults to "depth".
     model : str, optional
         Name of the model to use for conditioning in the unit. If not specified, searches for the appropriate model.
     weight : float, optional
         Weight of the unit. Defaults to 1.0.
     resolution : int, optional
         Resolution of the preprocessor. If not specified, uses the smaller dimension of the input image.
     thresholds : tuple, optional
@@ -326,32 +326,45 @@
         Whether to search for the annotator. Defaults to True.
 
     Returns
     -------
     dict
         A dictionary containing the settings for a ControlNet unit.
     """
-    if search:
-        annotator_res = search_annotators(annotator)[0]
+    if annotator is not None:
+        if search:
+            annotator_res = search_annotators(annotator)[0]
+        else:
+            annotator_res = annotator
     else:
-        annotator_res = annotator
-    if model is None:
-        model = search_cnet_models(annotator_res)[0]
+        annotator_res = None
+
+    if model is not None:
+        if search:
+            model_res = search_cnet_models(model)[0]
+        else:
+            model_res = model
+    else:
+        if annotator_res is not None:
+            model_res = search_cnet_models(annotator_res)[0]
+        else:
+            model_res = search_cnet_models("depth")[0]
+
     if resolution is None:
-        resolution = min(annotated_img.shape[:2])
+        resolution = min(img.shape[:2])
     if mask is None:
         mask_b64str = None
     else:
         mask_b64str = utils.img.img2b64str(mask)
-    input_b64str = utils.img.img2b64str(annotated_img)
+    input_b64str = utils.img.img2b64str(img)
     return {
         "input_image": input_b64str,
         "mask": mask_b64str,
         "module": annotator_res,
-        "model": model,
+        "model": model_res,
         "weight": weight,
         "resize_mode": resize_mode,
         "lowvram": lowvram,
         "processor_res": resolution,
         "threshold_a": thresholds[0],
         "threshold_b": thresholds[1],
         "guidance_start": guidance_start,
```

### Comparing `spida-0.2.3/spida/utils/img.py` & `spida-0.2.4/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.3/spida/utils/misc.py` & `spida-0.2.4/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.3/spida/utils/net.py` & `spida-0.2.4/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.3/spida.egg-info/PKG-INFO` & `spida-0.2.4/spida.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -84,21 +84,15 @@
 
 Spida supports the ControlNet extension, which allows for conditioning the generation process using ControlNet modules. You can use the `annotate()` function to annotate a batch of images using a specified ControlNet module:
 
 ```python
 annotated_images = spida.annotate(images, annotator="controlnet_module")
 ```
 
-The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation. An `annotated_image` from `annotated_images` can be passed into the ControlNet unit settings using the `cnet_settings()` function:
-
-```python
-cnet_sets = spida.cnet_settings(annotated_image, annotator="controlnet_module")
-```
-
-This function returns a dictionary containing the settings for a ControlNet unit. You can customize various parameters such as the model, weight, resolution, thresholds, control mode, resize mode, and more. Now, if you set the `cnet_settings` parameter in `txt2img()` to `cnet_sets`, the image generation process will be conditioned by the ControlNet.
+The `controlnet_module` parameter should be the name of the ControlNet module to be used for annotation.
 
 ### Retrieving Info
 
 Spida has multiple functions for retrieving information, they are listed here:
 
 ```python
 # get functions
@@ -181,24 +175,21 @@
 
 # Set the Stable Diffusion model
 spida.model("model_name")
 
 # Create an image to annotate
 imgs = spida.txt2img("chair")
 
-# Annotate the image using ControlNet
-depth = spida.annotate(imgs, annotator="depth")[0]
-
 # Generate the settings for a ControlNet unit
-cset = spida.cnet_settings(depth, annotator="depth")
+cset = spida.cnet_settings(imgs[0])
 
 # Use the settings for conditioning the generation process
 results = spida.txt2img("chair", cnet_settings=cset)
 
 # Create and display a grid showing each step of the process
-grid = spida.grid_img(np.array([imgs[0], spida.gray2rgb(depth), results[0]]), (1, None))
+grid = spida.grid_img(np.array([imgs[0], results[1], results[0]]), (1, None))
 spida.show(grid)
 ```
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

