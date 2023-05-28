# Comparing `tmp/vector_quantize_pytorch-1.6.3.tar.gz` & `tmp/vector_quantize_pytorch-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.6.3.tar", last modified: Sun May 28 16:32:41 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.4.tar", last modified: Sun May 28 17:08:11 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.6.3.tar` & `vector_quantize_pytorch-1.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:41.570721 vector_quantize_pytorch-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 16:32:41.570721 vector_quantize_pytorch-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 16:32:41.570721 vector_quantize_pytorch-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:41.570721 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    29475 2023-05-28 16:32:32.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:32:41.570721 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 16:32:41.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-28 16:32:41.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:32:41.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 16:32:41.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 16:32:41.000000 vector_quantize_pytorch-1.6.3/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:08:11.534656 vector_quantize_pytorch-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 17:08:11.534656 vector_quantize_pytorch-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:08:11.534656 vector_quantize_pytorch-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:08:11.534656 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29952 2023-05-28 17:07:54.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:08:11.534656 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 17:08:11.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-28 17:08:11.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:08:11.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 17:08:11.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 17:08:11.000000 vector_quantize_pytorch-1.6.4/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.6.3/LICENSE` & `vector_quantize_pytorch-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.3/PKG-INFO` & `vector_quantize_pytorch-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.6.3
+Version: 1.6.4
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.6.3/README.md` & `vector_quantize_pytorch-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.3/setup.py` & `vector_quantize_pytorch-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.6.3',
+  version = '1.6.4',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.3/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.4/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,16 @@
         reinmax = False,  # using reinmax for improved straight-through, assuming straight through helps at all
         sync_codebook = False,
         sync_affine_param = False,
         ema_update = True,
         learnable_codebook = False,
         affine_param = False,
         affine_param_batch_decay = 0.99,
-        affine_param_codebook_decay = 0.9
+        affine_param_codebook_decay = 0.9,
+        sync_update_v = 0. # the v that controls optimistic vs pessimistic update for synchronous update rule (21) https://minyoungg.github.io/vqtorch/assets/draft_050523.pdf
     ):
         super().__init__()
         self.dim = dim
         self.heads = heads
         self.separate_codebook_per_head = separate_codebook_per_head
 
         codebook_dim = default(codebook_dim, dim)
@@ -654,14 +655,17 @@
         self.project_in = nn.Linear(dim, codebook_input_dim) if requires_projection else nn.Identity()
         self.project_out = nn.Linear(codebook_input_dim, dim) if requires_projection else nn.Identity()
 
         self.eps = eps
         self.commitment_weight = commitment_weight
         self.commitment_use_cross_entropy_loss = commitment_use_cross_entropy_loss # whether to use cross entropy loss to codebook as commitment loss
 
+        assert 0 <= sync_update_v <= 1.
+        self.sync_update_v = sync_update_v
+
         codebook_class = EuclideanCodebook if not use_cosine_sim else CosineSimCodebook
 
         gumbel_sample_fn = partial(
             gumbel_sample,
             stochastic = stochastic_sample_codes,
             reinmax = reinmax,
             straight_through = straight_through
@@ -770,14 +774,18 @@
         # quantize
 
         quantize, embed_ind, distances = self._codebook(x, sample_codebook_temp = sample_codebook_temp)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
+            if self.sync_update_v > 0.:
+                # (21) in https://minyoungg.github.io/vqtorch/assets/draft_050523.pdf
+                quantize = quantize + self.sync_update_v * (quantize - quantize.detach())
+
         # function for calculating cross entropy loss to distance matrix
         # used for (1) naturalspeech2 training residual vq latents to be close to the correct codes and (2) cross-entropy based commitment loss
 
         def calculate_ce_loss(codes):
             if not is_multiheaded:
                 dist_einops_eq = '1 b n l -> b l n'
             elif self.separate_codebook_per_head:
```

