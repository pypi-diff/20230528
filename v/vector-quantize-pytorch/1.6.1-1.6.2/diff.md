# Comparing `tmp/vector_quantize_pytorch-1.6.1.tar.gz` & `tmp/vector_quantize_pytorch-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.6.1.tar", last modified: Sat May 27 16:30:41 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.2.tar", last modified: Sun May 28 00:35:53 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.6.1.tar` & `vector_quantize_pytorch-1.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:30:41.839069 vector_quantize_pytorch-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-27 16:30:41.839069 vector_quantize_pytorch-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 16:30:41.839069 vector_quantize_pytorch-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:30:41.839069 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    28278 2023-05-27 16:30:32.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:30:41.839069 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-27 16:30:41.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-27 16:30:41.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:30:41.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-27 16:30:41.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 16:30:41.000000 vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:35:53.589716 vector_quantize_pytorch-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 00:35:53.589716 vector_quantize_pytorch-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 00:35:53.589716 vector_quantize_pytorch-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:35:53.585715 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28302 2023-05-28 00:35:40.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 00:35:53.585715 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 00:35:53.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-28 00:35:53.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 00:35:53.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 00:35:53.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 00:35:53.000000 vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.6.1/LICENSE` & `vector_quantize_pytorch-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.1/PKG-INFO` & `vector_quantize_pytorch-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.6.1
+Version: 1.6.2
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.6.1/README.md` & `vector_quantize_pytorch-1.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -385,7 +385,17 @@
     title   = {Straightening Out the Straight-Through Estimator: Overcoming Optimization Challenges in Vector Quantized Networks},
     author  = {Huh, Minyoung and Cheung, Brian and Agrawal, Pulkit and Isola, Phillip},
     booktitle = {International Conference on Machine Learning},
     year    = {2023},
     organization = {PMLR}
 }
 ```
+
+```bibtex
+@inproceedings{rogozhnikov2022einops,
+    title   = {Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
+    author  = {Alex Rogozhnikov},
+    booktitle = {International Conference on Learning Representations},
+    year    = {2022},
+    url     = {https://openreview.net/forum?id=oapKSVM2bcj}
+}
+```
```

#### html2text {}

```diff
@@ -163,7 +163,12 @@
 Through and Beyond}, author = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and
 Bin Yu and Jianfeng Gao}, journal = {ArXiv}, year = {2023}, volume = {abs/
 2304.08612} } ``` ```bibtex @inproceedings{huh2023improvedvqste, title =
 {Straightening Out the Straight-Through Estimator: Overcoming Optimization
 Challenges in Vector Quantized Networks}, author = {Huh, Minyoung and Cheung,
 Brian and Agrawal, Pulkit and Isola, Phillip}, booktitle = {International
 Conference on Machine Learning}, year = {2023}, organization = {PMLR} } ```
+```bibtex @inproceedings{rogozhnikov2022einops, title = {Einops: Clear and
+Reliable Tensor Manipulations with Einstein-like Notation}, author = {Alex
+Rogozhnikov}, booktitle = {International Conference on Learning
+Representations}, year = {2022}, url = {https://openreview.net/
+forum?id=oapKSVM2bcj} } ```
```

### Comparing `vector_quantize_pytorch-1.6.1/setup.py` & `vector_quantize_pytorch-1.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.6.1',
+  version = '1.6.2',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.1/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.2/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,19 +319,19 @@
 
     @torch.jit.ignore
     def update_affine(self, data, embed):
         assert self.affine_param
 
         var_fn = partial(torch.var, unbiased = False)
 
-        self.update_with_decay('batch_mean', reduce(data, '... d -> d', 'mean'), self.affine_param_batch_decay)
-        self.update_with_decay('batch_variance', reduce(data, '... d -> d', var_fn), self.affine_param_batch_decay)
+        self.update_with_decay('batch_mean', reduce(data, 'h ... d -> h 1 d', 'mean'), self.affine_param_batch_decay)
+        self.update_with_decay('batch_variance', reduce(data, 'h ... d -> h 1 d', var_fn), self.affine_param_batch_decay)
 
-        self.update_with_decay('codebook_mean', reduce(embed, '... d -> d', 'mean'), self.affine_param_codebook_decay)
-        self.update_with_decay('codebook_variance', reduce(embed, '... d -> d', var_fn), self.affine_param_codebook_decay)
+        self.update_with_decay('codebook_mean', reduce(embed, 'h ... d -> h 1 d', 'mean'), self.affine_param_codebook_decay)
+        self.update_with_decay('codebook_variance', reduce(embed, 'h ... d -> h 1 d', var_fn), self.affine_param_codebook_decay)
 
     def replace(self, batch_samples, batch_mask):
         for ind, (samples, mask) in enumerate(zip(batch_samples.unbind(dim = 0), batch_mask.unbind(dim = 0))):
             if not torch.any(mask):
                 continue
 
             sampled = self.sample_fn(rearrange(samples, '... -> 1 ...'), mask.sum().item())
```

### Comparing `vector_quantize_pytorch-1.6.1/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.6.2/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.6.1
+Version: 1.6.2
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

