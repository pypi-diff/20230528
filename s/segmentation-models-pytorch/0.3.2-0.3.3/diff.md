# Comparing `tmp/segmentation_models_pytorch-0.3.2.tar.gz` & `tmp/segmentation_models_pytorch-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/segmentation_models_pytorch-0.3.2.tar", last modified: Sat Jan  7 10:37:23 2023, max compression
+gzip compressed data, was "dist/segmentation_models_pytorch-0.3.3.tar", last modified: Sun May 28 15:49:37 2023, max compression
```

## Comparing `segmentation_models_pytorch-0.3.2.tar` & `segmentation_models_pytorch-0.3.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    34276 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29540 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/datasets/oxford_pet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/dpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/inceptionresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mix_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mobileone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_gernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_sknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_universal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/lovasz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/mcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/soft_bce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/soft_ce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/tversky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24443 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/metrics/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34276 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 10:37:23.000000 segmentation_models_pytorch-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-01-07 10:37:14.000000 segmentation_models_pytorch-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    34023 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/datasets/oxford_pet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/dpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/inceptionresnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20402 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mix_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mobileone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_gernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_sknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_universal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/lovasz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/mcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/soft_bce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/soft_ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/tversky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24443 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/metrics/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34023 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:49:37.000000 segmentation_models_pytorch-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-28 15:49:25.000000 segmentation_models_pytorch-0.3.3/setup.py
```

### Comparing `segmentation_models_pytorch-0.3.2/LICENSE` & `segmentation_models_pytorch-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/PKG-INFO` & `segmentation_models_pytorch-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_models_pytorch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Image segmentation models with pre-trained backbones. PyTorch.
 Home-page: https://github.com/qubvel/segmentation_models.pytorch
 Author: Pavel Iakubovskii
 Author-email: qubvel@gmail.com
 License: MIT
 Description: 
         <div align="center">
@@ -17,15 +17,15 @@
         [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/qubvel/segmentation_models.pytorch/tests.yml?branch=master&style=for-the-badge)](https://github.com/qubvel/segmentation_models.pytorch/actions/workflows/tests.yml) 
         [![Read the Docs](https://img.shields.io/readthedocs/smp?style=for-the-badge&logo=readthedocs&logoColor=white)](https://smp.readthedocs.io/en/latest/) 
         <br>
         [![PyPI](https://img.shields.io/pypi/v/segmentation-models-pytorch?color=blue&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/segmentation-models-pytorch/) 
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/segmentation-models-pytorch?style=for-the-badge&color=blue)](https://pepy.tech/project/segmentation-models-pytorch) 
         <br>
         [![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.4+-red?style=for-the-badge&logo=pytorch)](https://pepy.tech/project/segmentation-models-pytorch) 
-        [![Python - Version](https://img.shields.io/badge/PYTHON-3.6+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
+        [![Python - Version](https://img.shields.io/badge/PYTHON-3.7+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
         
         </div>
         
         The main features of this library are:
         
          - High level API (just two lines to create a neural network)
          - 9 models architectures for binary and multi class segmentation (including legendary Unet)
@@ -474,33 +474,30 @@
         ### 🏆 Competitions won with the library
         
         `Segmentation Models` package is widely used in the image segmentation competitions.
         [Here](https://github.com/qubvel/segmentation_models.pytorch/blob/master/HALLOFFAME.md) you can find competitions, names of the winners and links to their solutions.
         
         ### 🤝 Contributing
         
-        ##### Install linting and formatting pre-commit hooks
-        ```bash
-        pip install pre-commit black==22.3.0 flake8==4.0.1
-        pre-commit install
-        ```
+        #### Install SMP  
         
-        ##### Run tests
         ```bash
-        pytest -p no:cacheprovider
+        make install_dev  # create .venv, install SMP in dev mode
         ```
         
-        ##### Run tests in docker
+        #### Run tests and code checks  
+        
         ```bash
-        $ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev pytest -p no:cacheprovider
+        make all          # run flake8, black, tests
         ```
         
-        ##### Generate table with encoders (in case you add a new encoder)
+        #### Update table with encoders  
+        
         ```bash
-        $ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev python misc/generate_table.py
+        make table        # generate table with encoders and print to stdout
         ```
         
         ### 📝 Citing
         ```
         @misc{Iakubovskii:2019,
           Author = {Pavel Iakubovskii},
           Title = {Segmentation Models Pytorch},
```

### Comparing `segmentation_models_pytorch-0.3.2/README.md` & `segmentation_models_pytorch-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/qubvel/segmentation_models.pytorch/tests.yml?branch=master&style=for-the-badge)](https://github.com/qubvel/segmentation_models.pytorch/actions/workflows/tests.yml) 
 [![Read the Docs](https://img.shields.io/readthedocs/smp?style=for-the-badge&logo=readthedocs&logoColor=white)](https://smp.readthedocs.io/en/latest/) 
 <br>
 [![PyPI](https://img.shields.io/pypi/v/segmentation-models-pytorch?color=blue&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/segmentation-models-pytorch/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/segmentation-models-pytorch?style=for-the-badge&color=blue)](https://pepy.tech/project/segmentation-models-pytorch) 
 <br>
 [![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.4+-red?style=for-the-badge&logo=pytorch)](https://pepy.tech/project/segmentation-models-pytorch) 
-[![Python - Version](https://img.shields.io/badge/PYTHON-3.6+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
+[![Python - Version](https://img.shields.io/badge/PYTHON-3.7+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
 
 </div>
 
 The main features of this library are:
 
  - High level API (just two lines to create a neural network)
  - 9 models architectures for binary and multi class segmentation (including legendary Unet)
@@ -465,33 +465,30 @@
 ### 🏆 Competitions won with the library
 
 `Segmentation Models` package is widely used in the image segmentation competitions.
 [Here](https://github.com/qubvel/segmentation_models.pytorch/blob/master/HALLOFFAME.md) you can find competitions, names of the winners and links to their solutions.
 
 ### 🤝 Contributing
 
-##### Install linting and formatting pre-commit hooks
-```bash
-pip install pre-commit black==22.3.0 flake8==4.0.1
-pre-commit install
-```
+#### Install SMP  
 
-##### Run tests
 ```bash
-pytest -p no:cacheprovider
+make install_dev  # create .venv, install SMP in dev mode
 ```
 
-##### Run tests in docker
+#### Run tests and code checks  
+
 ```bash
-$ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev pytest -p no:cacheprovider
+make all          # run flake8, black, tests
 ```
 
-##### Generate table with encoders (in case you add a new encoder)
+#### Update table with encoders  
+
 ```bash
-$ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev python misc/generate_table.py
+make table        # generate table with encoders and print to stdout
 ```
 
 ### 📝 Citing
 ```
 @misc{Iakubovskii:2019,
   Author = {Pavel Iakubovskii},
   Title = {Segmentation Models Pytorch},
```

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/__init__.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/heads.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/heads.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/initialization.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/initialization.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/base/modules.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/base/modules.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/datasets/oxford_pet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/datasets/oxford_pet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/deeplabv3/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/fpn/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/fpn/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/linknet/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/linknet/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/manet/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/manet/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pan/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pan/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/pspnet/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/pspnet/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unet/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/decoder.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/decoder.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/decoders/unetplusplus/model.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/decoders/unetplusplus/model.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/__init__.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,26 +97,26 @@
 
 def get_preprocessing_params(encoder_name, pretrained="imagenet"):
 
     if encoder_name.startswith("tu-"):
         encoder_name = encoder_name[3:]
         if not timm.models.is_model_pretrained(encoder_name):
             raise ValueError(f"{encoder_name} does not have pretrained weights and preprocessing parameters")
-        settings = timm.models.get_pretrained_cfg(encoder_name)
+        settings = timm.models.get_pretrained_cfg(encoder_name).__dict__
     else:
         all_settings = encoders[encoder_name]["pretrained_settings"]
         if pretrained not in all_settings.keys():
             raise ValueError("Available pretrained options {}".format(all_settings.keys()))
         settings = all_settings[pretrained]
 
     formatted_settings = {}
     formatted_settings["input_space"] = settings.get("input_space", "RGB")
     formatted_settings["input_range"] = list(settings.get("input_range", [0, 1]))
-    formatted_settings["mean"] = list(settings.get("mean"))
-    formatted_settings["std"] = list(settings.get("std"))
+    formatted_settings["mean"] = list(settings["mean"])
+    formatted_settings["std"] = list(settings["std"])
 
     return formatted_settings
 
 
 def get_preprocessing_fn(encoder_name, pretrained="imagenet"):
     params = get_preprocessing_params(encoder_name, pretrained=pretrained)
     return functools.partial(preprocess_input, **params)
```

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/_base.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/_base.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/_utils.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/densenet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/densenet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/dpn.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/dpn.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/efficientnet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/efficientnet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/inceptionresnetv2.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/inceptionv4.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mix_transformer.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mix_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This work is licensed under the NVIDIA Source Code License
 # ---------------------------------------------------------------
 import math
 import torch
 import torch.nn as nn
 from functools import partial
 
-from timm.models.layers import DropPath, to_2tuple, trunc_normal_
+from timm.layers import DropPath, to_2tuple, trunc_normal_
 
 
 class Mlp(nn.Module):
     def __init__(self, in_features, hidden_features=None, out_features=None, act_layer=nn.GELU, drop=0.0):
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
```

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mobilenet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mobilenet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/mobileone.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/mobileone.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/resnet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/senet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/senet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_efficientnet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_efficientnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 
 import torch
 import torch.nn as nn
 
 from timm.models.efficientnet import EfficientNet
 from timm.models.efficientnet import decode_arch_def, round_channels, default_cfgs
-from timm.models.layers.activations import Swish
+from timm.layers.activations import Swish
 
 from ._base import EncoderMixin
 
 
 def get_efficientnet_kwargs(channel_multiplier=1.0, depth_multiplier=1.0, drop_rate=0.2):
     """Create EfficientNet model.
     Ref impl: https://github.com/tensorflow/tpu/blob/master/models/official/efficientnet/efficientnet_model.py
@@ -154,226 +154,227 @@
     ):
         kwargs = gen_efficientnet_lite_kwargs(channel_multiplier, depth_multiplier, drop_rate)
         super().__init__(stage_idxs, out_channels, depth, **kwargs)
 
 
 def prepare_settings(settings):
     return {
-        "mean": settings["mean"],
-        "std": settings["std"],
-        "url": settings["url"],
+        "mean": settings.mean,
+        "std": settings.std,
+        "url": settings.url,
         "input_range": (0, 1),
         "input_space": "RGB",
     }
 
 
 timm_efficientnet_encoders = {
     "timm-efficientnet-b0": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b0"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b0_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b0_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b0"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b0"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b0"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 40, 112, 320),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.0,
             "depth_multiplier": 1.0,
             "drop_rate": 0.2,
         },
     },
     "timm-efficientnet-b1": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b1"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b1_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b1_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b1"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b1"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b1"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 40, 112, 320),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.0,
             "depth_multiplier": 1.1,
             "drop_rate": 0.2,
         },
     },
     "timm-efficientnet-b2": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b2"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b2_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b2_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b2"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b2"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b2"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 48, 120, 352),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.1,
             "depth_multiplier": 1.2,
             "drop_rate": 0.3,
         },
     },
     "timm-efficientnet-b3": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b3"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b3_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b3_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b3"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b3"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b3"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 40, 32, 48, 136, 384),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.2,
             "depth_multiplier": 1.4,
             "drop_rate": 0.3,
         },
     },
     "timm-efficientnet-b4": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b4"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b4_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b4_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b4"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b4"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b4"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 48, 32, 56, 160, 448),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.4,
             "depth_multiplier": 1.8,
             "drop_rate": 0.4,
         },
     },
     "timm-efficientnet-b5": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b5"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b5_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b5_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b5"].cfgs["in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b5"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b5"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 48, 40, 64, 176, 512),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.6,
             "depth_multiplier": 2.2,
             "drop_rate": 0.4,
         },
     },
     "timm-efficientnet-b6": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b6"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b6_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b6_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b6"].cfgs["aa_in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b6"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b6"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 56, 40, 72, 200, 576),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.8,
             "depth_multiplier": 2.6,
             "drop_rate": 0.5,
         },
     },
     "timm-efficientnet-b7": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b7"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b7_ap"]),
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b7_ns"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b7"].cfgs["aa_in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b7"].cfgs["ap_in1k"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_b7"].cfgs["ns_jft_in1k"]),
         },
         "params": {
             "out_channels": (3, 64, 48, 80, 224, 640),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 2.0,
             "depth_multiplier": 3.1,
             "drop_rate": 0.5,
         },
     },
     "timm-efficientnet-b8": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b8"]),
-            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b8_ap"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_b8"].cfgs["ra_in1k"]),
+            "advprop": prepare_settings(default_cfgs["tf_efficientnet_b8"].cfgs["ap_in1k"]),
         },
         "params": {
             "out_channels": (3, 72, 56, 88, 248, 704),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 2.2,
             "depth_multiplier": 3.6,
             "drop_rate": 0.5,
         },
     },
     "timm-efficientnet-l2": {
         "encoder": EfficientNetEncoder,
         "pretrained_settings": {
-            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_l2_ns"]),
+            "noisy-student": prepare_settings(default_cfgs["tf_efficientnet_l2"].cfgs["ns_jft_in1k"]),
+            "noisy-student-475": prepare_settings(default_cfgs["tf_efficientnet_l2"].cfgs["ns_jft_in1k_475"]),
         },
         "params": {
             "out_channels": (3, 136, 104, 176, 480, 1376),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 4.3,
             "depth_multiplier": 5.3,
             "drop_rate": 0.5,
         },
     },
     "timm-tf_efficientnet_lite0": {
         "encoder": EfficientNetLiteEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite0"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite0"].cfgs["in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 40, 112, 320),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.0,
             "depth_multiplier": 1.0,
             "drop_rate": 0.2,
         },
     },
     "timm-tf_efficientnet_lite1": {
         "encoder": EfficientNetLiteEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite1"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite1"].cfgs["in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 40, 112, 320),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.0,
             "depth_multiplier": 1.1,
             "drop_rate": 0.2,
         },
     },
     "timm-tf_efficientnet_lite2": {
         "encoder": EfficientNetLiteEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite2"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite2"].cfgs["in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 24, 48, 120, 352),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.1,
             "depth_multiplier": 1.2,
             "drop_rate": 0.3,
         },
     },
     "timm-tf_efficientnet_lite3": {
         "encoder": EfficientNetLiteEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite3"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite3"].cfgs["in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 32, 48, 136, 384),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.2,
             "depth_multiplier": 1.4,
             "drop_rate": 0.3,
         },
     },
     "timm-tf_efficientnet_lite4": {
         "encoder": EfficientNetLiteEncoder,
         "pretrained_settings": {
-            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite4"]),
+            "imagenet": prepare_settings(default_cfgs["tf_efficientnet_lite4"].cfgs["in1k"]),
         },
         "params": {
             "out_channels": (3, 32, 32, 56, 160, 448),
             "stage_idxs": (2, 3, 5),
             "channel_multiplier": 1.4,
             "depth_multiplier": 1.8,
             "drop_rate": 0.4,
```

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_gernet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_gernet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_mobilenetv3.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_regnet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_regnet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_res2net.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_res2net.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_resnest.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_resnest.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_sknet.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_sknet.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/timm_universal.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/timm_universal.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/vgg.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/vgg.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/encoders/xception.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/encoders/xception.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/_functional.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/_functional.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/constants.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/constants.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/dice.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/dice.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/focal.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/focal.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/jaccard.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/jaccard.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/lovasz.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/lovasz.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/mcc.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/mcc.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/soft_bce.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/soft_bce.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/soft_ce.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/soft_ce.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/losses/tversky.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/metrics/functional.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/base.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/base.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/functional.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/losses.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/meter.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/meter.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/metrics.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch/utils/train.py` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch/utils/train.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/PKG-INFO` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-models-pytorch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Image segmentation models with pre-trained backbones. PyTorch.
 Home-page: https://github.com/qubvel/segmentation_models.pytorch
 Author: Pavel Iakubovskii
 Author-email: qubvel@gmail.com
 License: MIT
 Description: 
         <div align="center">
@@ -17,15 +17,15 @@
         [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/qubvel/segmentation_models.pytorch/tests.yml?branch=master&style=for-the-badge)](https://github.com/qubvel/segmentation_models.pytorch/actions/workflows/tests.yml) 
         [![Read the Docs](https://img.shields.io/readthedocs/smp?style=for-the-badge&logo=readthedocs&logoColor=white)](https://smp.readthedocs.io/en/latest/) 
         <br>
         [![PyPI](https://img.shields.io/pypi/v/segmentation-models-pytorch?color=blue&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/segmentation-models-pytorch/) 
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/segmentation-models-pytorch?style=for-the-badge&color=blue)](https://pepy.tech/project/segmentation-models-pytorch) 
         <br>
         [![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.4+-red?style=for-the-badge&logo=pytorch)](https://pepy.tech/project/segmentation-models-pytorch) 
-        [![Python - Version](https://img.shields.io/badge/PYTHON-3.6+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
+        [![Python - Version](https://img.shields.io/badge/PYTHON-3.7+-red?style=for-the-badge&logo=python&logoColor=white)](https://pepy.tech/project/segmentation-models-pytorch) 
         
         </div>
         
         The main features of this library are:
         
          - High level API (just two lines to create a neural network)
          - 9 models architectures for binary and multi class segmentation (including legendary Unet)
@@ -474,33 +474,30 @@
         ### 🏆 Competitions won with the library
         
         `Segmentation Models` package is widely used in the image segmentation competitions.
         [Here](https://github.com/qubvel/segmentation_models.pytorch/blob/master/HALLOFFAME.md) you can find competitions, names of the winners and links to their solutions.
         
         ### 🤝 Contributing
         
-        ##### Install linting and formatting pre-commit hooks
-        ```bash
-        pip install pre-commit black==22.3.0 flake8==4.0.1
-        pre-commit install
-        ```
+        #### Install SMP  
         
-        ##### Run tests
         ```bash
-        pytest -p no:cacheprovider
+        make install_dev  # create .venv, install SMP in dev mode
         ```
         
-        ##### Run tests in docker
+        #### Run tests and code checks  
+        
         ```bash
-        $ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev pytest -p no:cacheprovider
+        make all          # run flake8, black, tests
         ```
         
-        ##### Generate table with encoders (in case you add a new encoder)
+        #### Update table with encoders  
+        
         ```bash
-        $ docker build -f docker/Dockerfile.dev -t smp:dev . && docker run --rm smp:dev python misc/generate_table.py
+        make table        # generate table with encoders and print to stdout
         ```
         
         ### 📝 Citing
         ```
         @misc{Iakubovskii:2019,
           Author = {Pavel Iakubovskii},
           Title = {Segmentation Models Pytorch},
```

### Comparing `segmentation_models_pytorch-0.3.2/segmentation_models_pytorch.egg-info/SOURCES.txt` & `segmentation_models_pytorch-0.3.3/segmentation_models_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segmentation_models_pytorch-0.3.2/setup.py` & `segmentation_models_pytorch-0.3.3/setup.py`

 * *Files identical despite different names*

