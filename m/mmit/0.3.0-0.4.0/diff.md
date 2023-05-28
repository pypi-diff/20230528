# Comparing `tmp/mmit-0.3.0.tar.gz` & `tmp/mmit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.3.0.tar", last modified: Sun May 28 14:06:43 2023, max compression
+gzip compressed data, was "mmit-0.4.0.tar", last modified: Sun May 28 15:27:53 2023, max compression
```

## Comparing `mmit-0.3.0.tar` & `mmit-0.4.0.tar`

### file list

```diff
@@ -1,124 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.094220 mmit-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.066220 mmit-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 14:06:28.000000 mmit-0.3.0/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-28 14:06:28.000000 mmit-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.066220 mmit-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-28 14:06:28.000000 mmit-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-28 14:06:28.000000 mmit-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 14:06:28.000000 mmit-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-28 14:06:28.000000 mmit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-28 14:06:43.094220 mmit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-28 14:06:28.000000 mmit-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.066220 mmit-0.3.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 14:06:28.000000 mmit-0.3.0/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-05-28 14:06:28.000000 mmit-0.3.0/docker/build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-28 14:06:28.000000 mmit-0.3.0/docker/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-05-28 14:06:28.000000 mmit-0.3.0/docker/start_container.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.066220 mmit-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.066220 mmit-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.062220 mmit-0.3.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.070220 mmit-0.3.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/_static/css/baseline.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.070220 mmit-0.3.0/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/_static/logo/logo_title.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.070220 mmit-0.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/api/create_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/api/create_encoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/api/create_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.070220 mmit-0.3.0/docs/source/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/guide/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.062220 mmit-0.3.0/docs/source/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.074220 mmit-0.3.0/docs/source/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/decoders/deeplabv3+.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/decoders/deeplabv3.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/decoders/fpn.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/decoders/unet++.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/decoders/unet.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.074220 mmit-0.3.0/docs/source/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-28 14:06:28.000000 mmit-0.3.0/docs/source/modules/encoders/timm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.074220 mmit-0.3.0/mmit/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.078220 mmit-0.3.0/mmit/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/base/upsamplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.078220 mmit-0.3.0/mmit/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/basedecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.078220 mmit-0.3.0/mmit/decoders/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.082220 mmit-0.3.0/mmit/decoders/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3plus/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3plus/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/deeplabv3plus/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.082220 mmit-0.3.0/mmit/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/fpn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/fpn/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.082220 mmit-0.3.0/mmit/decoders/pspnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/pspnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/pspnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/pspnet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.082220 mmit-0.3.0/mmit/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/unet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.086220 mmit-0.3.0/mmit/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.086220 mmit-0.3.0/mmit/decoders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/utils/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/decoders/utils/resizing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.086220 mmit-0.3.0/mmit/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/encoders/basencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.086220 mmit-0.3.0/mmit/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/encoders/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.090220 mmit-0.3.0/mmit/factory/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/factory/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/factory/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.090220 mmit-0.3.0/mmit/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/heads/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/heads/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.090220 mmit-0.3.0/mmit/models/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-28 14:06:28.000000 mmit-0.3.0/mmit/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.074220 mmit-0.3.0/mmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-28 14:06:43.000000 mmit-0.3.0/mmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-28 14:06:43.000000 mmit-0.3.0/mmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:06:43.000000 mmit-0.3.0/mmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 14:06:43.000000 mmit-0.3.0/mmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 14:06:43.000000 mmit-0.3.0/mmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-28 14:06:28.000000 mmit-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:06:43.094220 mmit-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.090220 mmit-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:43.094220 mmit-0.3.0/tests/demo_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/demo_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/demo_blocks/classic_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/demo_blocks/classic_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/demo_blocks/cursed_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/test_base_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 14:06:28.000000 mmit-0.3.0/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 15:27:32.000000 mmit-0.4.0/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-28 15:27:32.000000 mmit-0.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-28 15:27:32.000000 mmit-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-28 15:27:32.000000 mmit-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 15:27:32.000000 mmit-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-28 15:27:32.000000 mmit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-28 15:27:53.467454 mmit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-28 15:27:32.000000 mmit-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 15:27:32.000000 mmit-0.4.0/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-05-28 15:27:32.000000 mmit-0.4.0/docker/build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-28 15:27:32.000000 mmit-0.4.0/docker/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-05-28 15:27:32.000000 mmit-0.4.0/docker/start_container.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.455454 mmit-0.4.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.455454 mmit-0.4.0/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/deeplabv3+.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/deeplabv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/linknet.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/pspnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-28 15:27:32.000000 mmit-0.4.0/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.459454 mmit-0.4.0/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3plus/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3plus/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/deeplabv3plus/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/linknet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/linknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/linknet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/linknet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/pspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/pspnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/pspnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/pspnet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-28 15:27:32.000000 mmit-0.4.0/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.463454 mmit-0.4.0/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-28 15:27:53.000000 mmit-0.4.0/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-28 15:27:53.000000 mmit-0.4.0/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:27:53.000000 mmit-0.4.0/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 15:27:53.000000 mmit-0.4.0/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 15:27:53.000000 mmit-0.4.0/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-28 15:27:32.000000 mmit-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:27:53.467454 mmit-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:53.467454 mmit-0.4.0/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 15:27:32.000000 mmit-0.4.0/tests/test_end2end.py
```

### Comparing `mmit-0.3.0/.github/issue_template.md` & `mmit-0.4.0/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/.github/pull_request_template.md` & `mmit-0.4.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/.github/workflows/python-publish.yml` & `mmit-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/.gitignore` & `mmit-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/LICENSE` & `mmit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/PKG-INFO` & `mmit-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.3.0/README.md` & `mmit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docker/start_container.sh` & `mmit-0.4.0/docker/start_container.sh`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/.readthedocs.yaml` & `mmit-0.4.0/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/Makefile` & `mmit-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/make.bat` & `mmit-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/_static/css/baseline.css` & `mmit-0.4.0/docs/source/_static/css/baseline.css`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/_static/logo/logo.png` & `mmit-0.4.0/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/_static/logo/logo_title.png` & `mmit-0.4.0/docs/source/_static/logo/logo_title.png`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/conf.py` & `mmit-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/guide/examples.md` & `mmit-0.4.0/docs/source/guide/examples.md`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/docs/source/index.md` & `mmit-0.4.0/docs/source/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 :maxdepth: 1
 
 modules/decoders/unet
 modules/decoders/unet++
 modules/decoders/fpn
 modules/decoders/deeplabv3
 modules/decoders/deeplabv3+
+modules/decoders/pspnet
+modules/decoders/linknet
 ```
 
 ```{toctree}
 :caption: 'Encoders'
 :maxdepth: 1
 
 modules/encoders/timm
```

### Comparing `mmit-0.3.0/mmit/base/activations.py` & `mmit-0.4.0/mmit/base/activations.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/base/extra.py` & `mmit-0.4.0/mmit/base/extra.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/base/mismatch.py` & `mmit-0.4.0/mmit/base/mismatch.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/base/norms.py` & `mmit-0.4.0/mmit/base/norms.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/base/upsamplers.py` & `mmit-0.4.0/mmit/base/upsamplers.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/basedecoder.py` & `mmit-0.4.0/mmit/decoders/basedecoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/deeplabv3/aspp.py` & `mmit-0.4.0/mmit/decoders/deeplabv3/aspp.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/deeplabv3/model.py` & `mmit-0.4.0/mmit/decoders/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/deeplabv3/parts.py` & `mmit-0.4.0/mmit/decoders/deeplabv3/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/deeplabv3plus/model.py` & `mmit-0.4.0/mmit/decoders/deeplabv3plus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/deeplabv3plus/parts.py` & `mmit-0.4.0/mmit/decoders/deeplabv3plus/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/fpn/model.py` & `mmit-0.4.0/mmit/decoders/fpn/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/fpn/parts.py` & `mmit-0.4.0/mmit/decoders/fpn/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/pspnet/model.py` & `mmit-0.4.0/mmit/decoders/pspnet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/pspnet/parts.py` & `mmit-0.4.0/mmit/decoders/pspnet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/unet/model.py` & `mmit-0.4.0/mmit/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/unet/parts.py` & `mmit-0.4.0/mmit/decoders/unet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/unetplusplus/model.py` & `mmit-0.4.0/mmit/decoders/unetplusplus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/decoders/utils/resize.py` & `mmit-0.4.0/mmit/decoders/utils/resize.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/encoders/basencoder.py` & `mmit-0.4.0/mmit/encoders/basencoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/encoders/timm/model.py` & `mmit-0.4.0/mmit/encoders/timm/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/factory/components.py` & `mmit-0.4.0/mmit/factory/components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/factory/factory.py` & `mmit-0.4.0/mmit/factory/factory.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/factory/registry.py` & `mmit-0.4.0/mmit/factory/registry.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/heads/classification.py` & `mmit-0.4.0/mmit/heads/classification.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit/heads/segmentation.py` & `mmit-0.4.0/mmit/heads/segmentation.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/mmit.egg-info/PKG-INFO` & `mmit-0.4.0/mmit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.3.0/mmit.egg-info/SOURCES.txt` & `mmit-0.4.0/mmit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 docs/source/api/create_model.md
 docs/source/guide/examples.md
 docs/source/guide/install.md
 docs/source/guide/quickstart.md
 docs/source/modules/decoders/deeplabv3+.md
 docs/source/modules/decoders/deeplabv3.md
 docs/source/modules/decoders/fpn.md
+docs/source/modules/decoders/linknet.md
+docs/source/modules/decoders/pspnet.md
 docs/source/modules/decoders/unet++.md
 docs/source/modules/decoders/unet.md
 docs/source/modules/encoders/timm.md
 mmit/__init__.py
 mmit.egg-info/PKG-INFO
 mmit.egg-info/SOURCES.txt
 mmit.egg-info/dependency_links.txt
@@ -51,14 +53,17 @@
 mmit/decoders/deeplabv3plus/__init__.py
 mmit/decoders/deeplabv3plus/aspp.py
 mmit/decoders/deeplabv3plus/model.py
 mmit/decoders/deeplabv3plus/parts.py
 mmit/decoders/fpn/__init__.py
 mmit/decoders/fpn/model.py
 mmit/decoders/fpn/parts.py
+mmit/decoders/linknet/__init__.py
+mmit/decoders/linknet/model.py
+mmit/decoders/linknet/parts.py
 mmit/decoders/pspnet/__init__.py
 mmit/decoders/pspnet/model.py
 mmit/decoders/pspnet/parts.py
 mmit/decoders/unet/__init__.py
 mmit/decoders/unet/model.py
 mmit/decoders/unet/parts.py
 mmit/decoders/unetplusplus/__init__.py
```

### Comparing `mmit-0.3.0/pyproject.toml` & `mmit-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
     "torch>=1.10"
 ]
 requires-python = ">=3.8"
-version = "0.3.0"
+version = "0.4.0"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
```

### Comparing `mmit-0.3.0/tests/demo_blocks/classic_decoder.py` & `mmit-0.4.0/tests/demo_blocks/classic_decoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/tests/demo_blocks/classic_encoder.py` & `mmit-0.4.0/tests/demo_blocks/classic_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/tests/demo_blocks/cursed_encoder.py` & `mmit-0.4.0/tests/demo_blocks/cursed_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/tests/test_base_components.py` & `mmit-0.4.0/tests/test_base_components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.3.0/tests/test_decoders.py` & `mmit-0.4.0/tests/test_decoders.py`

 * *Files identical despite different names*

