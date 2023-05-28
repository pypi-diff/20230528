# Comparing `tmp/mct-quantizers-1.0.0.28052023.post83647.tar.gz` & `tmp/mct-quantizers-1.0.0.28052023.post92442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-1.0.0.28052023.post83647.tar", last modified: Sun May 28 08:36:48 2023, max compression
+gzip compressed data, was "mct-quantizers-1.0.0.28052023.post92442.tar", last modified: Sun May 28 09:24:43 2023, max compression
```

## Comparing `mct-quantizers-1.0.0.28052023.post83647.tar` & `mct-quantizers-1.0.0.28052023.post92442.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.170359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.170359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.170359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-28 08:36:28.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:36:48.170359 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 08:36:47.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-28 08:36:48.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 08:36:47.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 08:36:47.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 08:36:47.000000 mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 08:36:48.174359 mct-quantizers-1.0.0.28052023.post83647/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-28 08:36:47.000000 mct-quantizers-1.0.0.28052023.post83647/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.786147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-28 09:24:42.000000 mct-quantizers-1.0.0.28052023.post92442/setup.py
```

### Comparing `mct-quantizers-1.0.0.28052023.post83647/LICENSE.md` & `mct-quantizers-1.0.0.28052023.post92442/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, BaseInferableQuantizer
+from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, BaseInferableQuantizer, mark_quantizer
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.keras.activation_quantization_holder import KerasActivationQuantizationHolder
 from mct_quantizers.pytorch.activation_quantization_holder import PytorchActivationQuantizationHolder
 from mct_quantizers.keras.load_model import keras_load_quantized_model
 from mct_quantizers.keras.quantize_wrapper import KerasQuantizationWrapper
 from mct_quantizers.pytorch.load_model import pytorch_load_quantized_model
 from mct_quantizers.pytorch.quantize_wrapper import PytorchQuantizationWrapper
 
+from mct_quantizers.common import constants
+from mct_quantizers.keras import quantizers
+from mct_quantizers.pytorch import quantizers
+
 __version__ = "1.0.0"
```

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/constants.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/quant_info.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/common/quant_utils.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/load_model.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/logger.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/mct_quantizers.egg-info/SOURCES.txt` & `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post83647/setup.py` & `mct-quantizers-1.0.0.28052023.post92442/setup.py`

 * *Files identical despite different names*

