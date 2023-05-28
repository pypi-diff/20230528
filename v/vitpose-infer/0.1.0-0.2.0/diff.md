# Comparing `tmp/vitpose_infer-0.1.0.tar.gz` & `tmp/vitpose_infer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitpose_infer-0.1.0.tar", last modified: Sun May 28 17:35:19 2023, max compression
+gzip compressed data, was "vitpose_infer-0.2.0.tar", last modified: Sun May 28 17:47:23 2023, max compression
```

## Comparing `vitpose_infer-0.1.0.tar` & `vitpose_infer-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    35149 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/LICENSE
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1813 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/PKG-INFO
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1303 2023-05-28 17:34:46.000000 vitpose_infer-0.1.0/README.md
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      584 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/pyproject.toml
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       38 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/setup.cfg
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.071467 vitpose_infer-0.1.0/src/
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.071467 vitpose_infer-0.1.0/src/vitpose_infer/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       30 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/__init__.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.071467 vitpose_infer-0.1.0/src/vitpose_infer/builder/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       40 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/__init__.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.075467 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1272 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/__init__.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1868 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/alexnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6374 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/cpm.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6946 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hourglass.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7048 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hourglass_ae.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    29872 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hrformer.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    35843 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/litehrnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     9995 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mobilenet_v2.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7271 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mobilenet_v3.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    18464 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mspn.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12005 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/regnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12124 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/resnest.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6659 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/resnext.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    21759 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/rsn.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     8057 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/scnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4602 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/seresnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7039 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/seresnext.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11942 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/shufflenet_v1.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    10666 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/shufflenet_v2.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    10003 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/tcn.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1561 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/test_torch.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.075467 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      358 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/__init__.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      889 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/channel_shuffle.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4196 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/inverted_residual.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1056 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/make_divisible.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1983 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/se_layer.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     2845 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/utils.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7165 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vgg.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6586 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vipnas_mbv3.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    21737 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vipnas_resnet.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11235 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vit.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.071467 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5218 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5228 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_simple_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5223 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5231 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_simple_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5221 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5229 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_simple_coco_256x192.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/__init__.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1258 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/__init__.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11162 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/deconv_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5789 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/deeppose_regression_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3318 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/hmr_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    19773 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/interhand_3d_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12400 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/temporal_regression_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4038 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_base_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    20048 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_multi_stage_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    14516 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_simple_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    13385 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/vipnas_heatmap_simple_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6040 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/voxelpose_head.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     2410 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/builder/model_builder.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3946 2023-05-25 07:16:41.000000 vitpose_infer-0.1.0/src/vitpose_infer/main.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4138 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/model_builder.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4395 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/ViTPose_trt.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/__init__.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      332 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/convert_to_trt.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3394 2023-05-25 06:44:09.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/general_utils.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1064 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/inference_test.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      708 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/logger_helper.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7933 2023-05-25 06:44:01.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/pose_utils.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12498 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/pose_viz.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      958 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/timerr.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4851 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/visualizer.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/setup.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.079467 vitpose_infer-0.1.0/src/vitpose_infer/tracker/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/tracker/__init__.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      951 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/tracker/basetrack.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11953 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/tracker/byte_tracker.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     9547 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/tracker/kalman_filter.py
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6188 2023-05-24 06:40:56.000000 vitpose_infer-0.1.0/src/vitpose_infer/tracker/matching.py
-drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:35:19.071467 vitpose_infer-0.1.0/src/vitpose_infer.egg-info/
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1813 2023-05-28 17:35:19.000000 vitpose_infer-0.1.0/src/vitpose_infer.egg-info/PKG-INFO
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3667 2023-05-28 17:35:19.000000 vitpose_infer-0.1.0/src/vitpose_infer.egg-info/SOURCES.txt
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        1 2023-05-28 17:35:19.000000 vitpose_infer-0.1.0/src/vitpose_infer.egg-info/dependency_links.txt
--rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       14 2023-05-28 17:35:19.000000 vitpose_infer-0.1.0/src/vitpose_infer.egg-info/top_level.txt
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    35149 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/LICENSE
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1827 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/PKG-INFO
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1303 2023-05-28 17:34:46.000000 vitpose_infer-0.2.0/README.md
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      598 2023-05-28 17:47:16.000000 vitpose_infer-0.2.0/pyproject.toml
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       38 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/setup.cfg
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.699359 vitpose_infer-0.2.0/src/
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.699359 vitpose_infer-0.2.0/src/vitpose_infer/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       30 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/__init__.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.699359 vitpose_infer-0.2.0/src/vitpose_infer/builder/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       40 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/__init__.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1272 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/__init__.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1868 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/alexnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6374 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/cpm.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6946 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hourglass.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7048 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hourglass_ae.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    29872 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hrformer.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    35843 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/litehrnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     9995 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mobilenet_v2.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7271 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mobilenet_v3.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    18464 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mspn.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12005 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/regnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12124 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/resnest.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6659 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/resnext.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    21759 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/rsn.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     8057 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/scnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4602 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/seresnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7039 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/seresnext.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11942 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/shufflenet_v1.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    10666 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/shufflenet_v2.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    10003 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/tcn.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1561 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/test_torch.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      358 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/__init__.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      889 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/channel_shuffle.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4196 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/inverted_residual.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1056 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/make_divisible.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1983 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/se_layer.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     2845 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/utils.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7165 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vgg.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6586 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vipnas_mbv3.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    21737 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vipnas_resnet.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11235 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vit.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.699359 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5218 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5228 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_simple_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5223 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5231 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_simple_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5221 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5229 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_simple_coco_256x192.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/__init__.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1258 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/__init__.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11162 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/deconv_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     5789 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/deeppose_regression_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3318 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/hmr_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    19773 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/interhand_3d_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12400 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/temporal_regression_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4038 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_base_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    20048 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_multi_stage_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    14516 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_simple_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    13385 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/vipnas_heatmap_simple_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6040 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/voxelpose_head.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     2410 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/builder/model_builder.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3946 2023-05-25 07:16:41.000000 vitpose_infer-0.2.0/src/vitpose_infer/main.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4138 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/model_builder.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4395 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/ViTPose_trt.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/__init__.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      332 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/convert_to_trt.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3394 2023-05-25 06:44:09.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/general_utils.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1064 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/inference_test.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      708 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/logger_helper.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     7933 2023-05-25 06:44:01.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/pose_utils.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    12498 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/pose_viz.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      958 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/timerr.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     4851 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/visualizer.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/setup.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.703359 vitpose_infer-0.2.0/src/vitpose_infer/tracker/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        0 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/tracker/__init__.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)      951 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/tracker/basetrack.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)    11953 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/tracker/byte_tracker.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     9547 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/tracker/kalman_filter.py
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     6188 2023-05-24 06:40:56.000000 vitpose_infer-0.2.0/src/vitpose_infer/tracker/matching.py
+drwxrwxr-x   0 gpastal   (1001) gpastal   (1001)        0 2023-05-28 17:47:23.699359 vitpose_infer-0.2.0/src/vitpose_infer.egg-info/
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     1827 2023-05-28 17:47:23.000000 vitpose_infer-0.2.0/src/vitpose_infer.egg-info/PKG-INFO
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)     3667 2023-05-28 17:47:23.000000 vitpose_infer-0.2.0/src/vitpose_infer.egg-info/SOURCES.txt
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)        1 2023-05-28 17:47:23.000000 vitpose_infer-0.2.0/src/vitpose_infer.egg-info/dependency_links.txt
+-rw-rw-r--   0 gpastal   (1001) gpastal   (1001)       14 2023-05-28 17:47:23.000000 vitpose_infer-0.2.0/src/vitpose_infer.egg-info/top_level.txt
```

### Comparing `vitpose_infer-0.1.0/LICENSE` & `vitpose_infer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/PKG-INFO` & `vitpose_infer-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vitpose_infer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Vitpose with yolov5 and tracking
 Author-email: gpastal24 <some.email@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/gpastal24/ViTPose-Pytorch
+Project-URL: Bug Tracker, https://github.com/gpastal24/ViTPose-Pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vitpose_infer-0.1.0/README.md` & `vitpose_infer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/__init__.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/alexnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/alexnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/cpm.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/cpm.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hourglass.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hourglass.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hourglass_ae.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hourglass_ae.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/hrformer.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/hrformer.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/litehrnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/litehrnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mobilenet_v2.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mobilenet_v3.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/mspn.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/mspn.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/regnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/regnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/resnest.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/resnext.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/rsn.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/rsn.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/scnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/scnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/seresnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/seresnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/seresnext.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/seresnext.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/shufflenet_v1.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/shufflenet_v1.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/shufflenet_v2.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/shufflenet_v2.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/tcn.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/tcn.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/test_torch.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/test_torch.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/channel_shuffle.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/inverted_residual.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/make_divisible.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/se_layer.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/utils/utils.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vgg.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vgg.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vipnas_mbv3.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vipnas_mbv3.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vipnas_resnet.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vipnas_resnet.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/backbones/vit.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_simple_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_base_simple_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_simple_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_huge_simple_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_simple_coco_256x192.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/configs/coco/ViTPose_large_simple_coco_256x192.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/__init__.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/deconv_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/deconv_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/deeppose_regression_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/deeppose_regression_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/hmr_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/hmr_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/interhand_3d_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/interhand_3d_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/temporal_regression_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/temporal_regression_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_base_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_base_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_multi_stage_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_multi_stage_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/topdown_heatmap_simple_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/topdown_heatmap_simple_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/vipnas_heatmap_simple_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/vipnas_heatmap_simple_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/heads/voxelpose_head.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/heads/voxelpose_head.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/builder/model_builder.py` & `vitpose_infer-0.2.0/src/vitpose_infer/builder/model_builder.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/main.py` & `vitpose_infer-0.2.0/src/vitpose_infer/main.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/model_builder.py` & `vitpose_infer-0.2.0/src/vitpose_infer/model_builder.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/ViTPose_trt.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/ViTPose_trt.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/general_utils.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/inference_test.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/inference_test.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/logger_helper.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/logger_helper.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/pose_utils.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/pose_utils.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/pose_viz.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/pose_viz.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/timerr.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/timerr.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/pose_utils/visualizer.py` & `vitpose_infer-0.2.0/src/vitpose_infer/pose_utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/tracker/basetrack.py` & `vitpose_infer-0.2.0/src/vitpose_infer/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/tracker/byte_tracker.py` & `vitpose_infer-0.2.0/src/vitpose_infer/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/tracker/kalman_filter.py` & `vitpose_infer-0.2.0/src/vitpose_infer/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer/tracker/matching.py` & `vitpose_infer-0.2.0/src/vitpose_infer/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer.egg-info/PKG-INFO` & `vitpose_infer-0.2.0/src/vitpose_infer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vitpose-infer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Vitpose with yolov5 and tracking
 Author-email: gpastal24 <some.email@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/gpastal24/ViTPose-Pytorch
+Project-URL: Bug Tracker, https://github.com/gpastal24/ViTPose-Pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vitpose_infer-0.1.0/src/vitpose_infer.egg-info/SOURCES.txt` & `vitpose_infer-0.2.0/src/vitpose_infer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

