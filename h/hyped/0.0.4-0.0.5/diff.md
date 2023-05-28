# Comparing `tmp/hyped-0.0.4.tar.gz` & `tmp/hyped-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.0.4.tar", last modified: Thu May 18 15:51:14 2023, max compression
+gzip compressed data, was "hyped-0.0.5.tar", last modified: Sun May 28 16:21:09 2023, max compression
```

## Comparing `hyped-0.0.4.tar` & `hyped-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.105875 hyped-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 15:51:02.000000 hyped-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:51:14.101875 hyped-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-18 15:51:02.000000 hyped-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.085875 hyped-0.0.4/hyped/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.089875 hyped-0.0.4/hyped/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/xcr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.089875 hyped-0.0.4/hyped/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/evaluate/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/mlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/seqeval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/modeling/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/mlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.097875 hyped-0.0.4/hyped/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.097875 hyped-0.0.4/hyped/pipeline/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/msl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/pipeline/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/bio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/typedlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/typedmapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.085875 hyped-0.0.4/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:51:14.105875 hyped-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-18 15:51:02.000000 hyped-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.551022 hyped-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 16:20:58.000000 hyped-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-28 16:21:09.551022 hyped-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-28 16:20:58.000000 hyped-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.539022 hyped-0.0.5/hyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.539022 hyped-0.0.5/hyped/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/datasets/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/datasets/xcr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.539022 hyped-0.0.5/hyped/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.543022 hyped-0.0.5/hyped/stages/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.543022 hyped-0.0.5/hyped/stages/prepare/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/filters/msl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.543022 hyped-0.0.5/hyped/stages/prepare/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/processors/bio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/prepare/processors/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.543022 hyped-0.0.5/hyped/stages/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/test/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.543022 hyped-0.0.5/hyped/stages/train/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.547022 hyped-0.0.5/hyped/stages/train/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.547022 hyped-0.0.5/hyped/stages/train/metrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/metrics/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/metrics/mlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/metrics/seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/metrics/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.551022 hyped-0.0.5/hyped/stages/train/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.551022 hyped-0.0.5/hyped/stages/train/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/mlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/heads/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/stages/train/modeling/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.551022 hyped-0.0.5/hyped/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/utils/typedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-28 16:20:58.000000 hyped-0.0.5/hyped/utils/typedmapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:21:09.539022 hyped-0.0.5/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 16:21:09.000000 hyped-0.0.5/hyped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 16:21:09.551022 hyped-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-28 16:20:58.000000 hyped-0.0.5/setup.py
```

### Comparing `hyped-0.0.4/LICENSE` & `hyped-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/PKG-INFO` & `hyped-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of data pipelines to ease the training of transformer models
 Home-page: https://github.com/ndoll1998/hyped/tree/master
 Author: Niclas Doll
 Author-email: niclas@amazonis.net
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
@@ -49,53 +49,95 @@
 The following demonstates how to train a text classification model on the [`imdb`](https://huggingface.co/datasets/imdb) dataset by going through all three stages of the ML pipeline (from `examples/run.sh`).
 
 ```bash
 # data preparation stage
 # runs the data preparation pipeline specified in the
 # configuration file and saves the prepared dataset
 # to the specified location
-python -m hyped.scripts.prepare \
+python -m hyped.stages.prepare \
     -c examples/text_cls/imdb/distilbert_data.json \
     -o output/distilbert_data
 
 # model training stage
 # trains a model on the prepared data generated by the
 # previous stage
-python -m hyped.scripts.train \
+python -m hyped.stages.train \
     -c examples/text_cls/imdb/distilbert_run.json \
     -d output/distilbert_data \
     -o output/model
 
 # model evaluation stage
 # evaluates the trained model on the test split of the
 # prepared dataset generated earlier
-python -m hyped.scripts.evaluate \
+python -m hyped.stages.evaluate \
     -c examples/text_cls/imdb/distilbert_run.json \
     -d output/distilbert_data \
     -m output/model/best-model
 ```
 
 ## features
 
 `hyped` currently implements all components required to train and evaluate models for the following NLP tasks:
 
  - Text Classification
  - Named Entity Recognition
  - Multi-label Classification
+ - Causal Language Modeling
 
+### adapters
+
+`hyped` is build upon [`adapter-transformers`](https://docs.adapterhub.ml/), which allows the configuration of a variety of model architectures. See the following excerpt for how to configure an adapter model in the run configuration (from [`examples/cls/imdb/distilbert_run.json`](examples/cls/imdb/distilbert_run.json)):
+
+```json
+{
+    "model": {
+        "pretrained_ckpt": "distilbert-base-uncased",
+        
+        "adapter_name": "imdb",
+        "adapter": {
+            "train_adapter": true,
+            "adapter_config": "pfeiffer"
+        },
+
+        "heads": {
+            "cls": {
+                "head_type": "hyped-cls-head",
+                "label_column": "labels"
+            }
+        }
+    }
+}
+```
+
+The `adapter` field in the above configuration mirrors the [`AdapterArguments`](https://docs.adapterhub.ml/classes/adapter_training.html#transformers.adapters.training.AdapterArguments) class and can specify all it's values (e.g. `load_adapter` for loading pretrained adapters). Furthermore, by setting `train_adapter` to True, only the paramters of the adapter and head are trained, while the pretrained encoder parameters are frozen.
+
+Alternatively, the adapter configuration can also be omitted, in which case no adapter is used and the encoder output is directly passed to the prediction heads.
+
+### dvc
+
+`hyped` is designed to be easily integratable into existing data pipelines. Thus, it fits well with [`dvc`](https://dvc.org/) pipelines. See [`examples/dvc`](examples/dvc) for an example setup.
+
+### deepspeed
+
+`hyped` supports distributed training allowing for both pre-training and fine-tuning of very large language models. See [`examples/lm/run.json`](examples/lm/run.json) for an example configuration. To lauch a distributed training you need to use `hyped`'s command line interface:
+
+```bash
+deepspeed --no_python hyped train -c config.json -d data/ -o model/
+```
 
 ## roadmap
 
-`hyped` is still in its very early stages. With time the goal is to make the framework applicable to a wide variety of tasks and setups. Planned features include the following:
+`hyped` is currently in its early stages of development. Over time, the goal is to expand its applicability to a diverse range of tasks and setups. The following features are planned for future development:
 
  - ~~support adapter training~~
+ - ~~support transformers models~~
  - support more tasks
    - Masked Language Modeling
-   - Causal Language Modeling
+   - ~~Causal Language Modeling~~
    - nested Named Entity Recognition
    - Question Answering
  - support multi-modal encoders
    - LayoutLM
    - LiLT
  - support distributed training/inference
-   - deepspeed
+   - ~~deepspeed~~
    - pytorch DDP and FSDP
```

### Comparing `hyped-0.0.4/hyped/datasets/__init__.py` & `hyped-0.0.5/hyped/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/datasets/cas.py` & `hyped-0.0.5/hyped/datasets/cas.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/datasets/xcr.py` & `hyped-0.0.5/hyped/datasets/xcr.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/auto.py` & `hyped-0.0.5/hyped/stages/train/metrics/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from . import metrics
 from .metrics.base import HypedMetric, HypedMetricConfig
 from .collection import HypedMetricCollection
 from transformers.adapters import heads
 from hyped.utils.typedmapping import typedmapping
+from functools import cmp_to_key
 
 class HypedAutoMetric(object):
     METRICS_MAPPING = typedmapping[
         type[heads.PredictionHead],
         typedmapping
     ]()
 
     @classmethod
     def from_head(
         cls,
         head:heads.PredictionHead,
         config:HypedMetricConfig
     ) -> HypedMetric:
         # find metrics for head
-        for head_t, metrics_mapping in cls.METRICS_MAPPING.items():
+        key = cmp_to_key(lambda t, v: 2 * issubclass(v, t) - 1)
+        for head_t in sorted(cls.METRICS_MAPPING, key=key):
             if isinstance(head, head_t):
                 # find specific metric
+                metrics_mapping = cls.METRICS_MAPPING[head_t]
                 metric_t = metrics_mapping.get(type(config), None)
                 # check if metric type found
                 if metric_t is None:
                     raise ValueError("Invalid metric type `%s`." % config.metric_type)
                 # create metric instance
                 metric = metric_t(head, config)
                 return metric
```

### Comparing `hyped-0.0.4/hyped/evaluate/collection.py` & `hyped-0.0.5/hyped/stages/train/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/metrics/base.py` & `hyped-0.0.5/hyped/stages/train/metrics/metrics/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/metrics/cls.py` & `hyped-0.0.5/hyped/stages/train/metrics/metrics/cls.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/metrics/mlc.py` & `hyped-0.0.5/hyped/stages/train/metrics/metrics/mlc.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/metrics/seqeval.py` & `hyped-0.0.5/hyped/stages/train/metrics/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/evaluate/processors.py` & `hyped-0.0.5/hyped/stages/train/metrics/processors.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/modeling/auto.py` & `hyped-0.0.5/hyped/stages/train/modeling/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,7 +59,8 @@
     def register_custom_head(cls, head_name, head_type):
         cls.CUSTOM_HEAD_MAPPING[head_name] = head_type
 
 # register prediction heads
 HypedAutoAdapterModel.register_custom_head(heads.HypedClsHeadConfig.head_type, heads.HypedClsHead)
 HypedAutoAdapterModel.register_custom_head(heads.HypedMlcHeadConfig.head_type, heads.HypedMlcHead)
 HypedAutoAdapterModel.register_custom_head(heads.HypedTaggingHeadConfig.head_type, heads.HypedTaggingHead)
+HypedAutoAdapterModel.register_custom_head(heads.HypedCausalLMHeadConfig.head_type, heads.HypedCausalLMHead)
```

### Comparing `hyped-0.0.4/hyped/modeling/heads/base.py` & `hyped-0.0.5/hyped/stages/train/modeling/heads/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,18 +66,21 @@
     @property
     def loss_coeff(self) -> float:
         return self.config['loss_coeff']
 
     def get_label_names(self) -> list[str]:
         return [self.label_column]
 
+    def get_labels(self, kwargs) -> dict[str, Any]:
+        return {'labels': kwargs.get(self.label_column, None)}
+
     def forward(self, *args, **kwargs):
         # prepare kwargs, rename label column as expected by base
         kwargs = kwargs.copy()
-        kwargs['labels'] = kwargs.pop(self.label_column, None)
+        kwargs.update(self.get_labels(kwargs))
         # run base class
         out = self.wrapped_forward(*args, **kwargs)
 
         # apply loss coefficient
         if kwargs['labels'] is not None:
             if isinstance(out, dict):
                 out['loss'] *= self.loss_coeff
@@ -86,12 +89,7 @@
 
         # return output
         return out
 
     @abstractmethod
     def wrapped_forward(self, *args, **kwargs):
         ...
-
-    def collate_labels(self, labels:list, return_tensors:str ='pt'):
-        if return_tensors != 'pt':
-            raise NotImplementedError()
-        return torch.stack(labels, dim=0)
```

### Comparing `hyped-0.0.4/hyped/modeling/heads/cls.py` & `hyped-0.0.5/hyped/stages/train/modeling/heads/cls.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/modeling/heads/mlc.py` & `hyped-0.0.5/hyped/stages/train/modeling/heads/mlc.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,19 +43,7 @@
             self,
             label_column=label_column,
             loss_coeff=loss_coeff
         )
 
     # set forward function
     wrapped_forward = MultiLabelClassificationHead.forward
-
-    def collate_labels(self, labels:list[list[int]], return_tensors:str ='pt'):
-        if return_tensors != 'pt':
-            raise NotImplementedError()
-
-        num_labels = self.config['num_labels']
-        # binarize labels
-        binarized_labels = torch.zeros((len(labels), num_labels), dtype=int)
-        for i, ids in enumerate(labels):
-            binarized_labels[i, ids] = 1
-        # return
-        return binarized_labels
```

### Comparing `hyped-0.0.4/hyped/modeling/heads/tagging.py` & `hyped-0.0.5/hyped/stages/train/modeling/heads/tagging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import torch
 from transformers import PreTrainedModel
 from transformers.adapters.heads import TaggingHead
 from .base import HypedPredictionHead, HypedPredictionHeadConfig
 
 from datasets.features import Sequence, ClassLabel
 from dataclasses import dataclass
 from typing import Literal
@@ -38,9 +39,17 @@
         )
         HypedPredictionHead.__init__(
             self,
             label_column=label_column,
             loss_coeff=loss_coeff
         )
 
+    def get_labels(self, kwargs):
+        mask = kwargs.get('attention_mask', None)
+        # get labels and mask out invalid targets
+        labels = HypedPredictionHead.get_labels(self, kwargs)['labels']
+        labels = torch.where(mask.bool(), labels, -100) if mask is not None else labels
+        # return labels dict
+        return {'labels': labels}
+
     # set forward function
     wrapped_forward = TaggingHead.forward
```

### Comparing `hyped-0.0.4/hyped/modeling/trainer.py` & `hyped-0.0.5/hyped/stages/train/modeling/trainer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/auto.py` & `hyped-0.0.5/hyped/stages/prepare/auto.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/filters/base.py` & `hyped-0.0.5/hyped/stages/prepare/filters/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/filters/msl.py` & `hyped-0.0.5/hyped/stages/prepare/filters/msl.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/pipeline.py` & `hyped-0.0.5/hyped/stages/prepare/pipeline.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/processors/base.py` & `hyped-0.0.5/hyped/stages/prepare/processors/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/processors/bio.py` & `hyped-0.0.5/hyped/stages/prepare/processors/bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/pipeline/processors/tokenizer.py` & `hyped-0.0.5/hyped/stages/prepare/processors/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/scripts/prepare.py` & `hyped-0.0.5/hyped/stages/prepare/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
-import hyped
 import datasets
 import transformers
 import numpy as np
 import pydantic
 import logging
-# register packaged datasets
-import hyped.datasets
+# hyped
+from .pipeline import Pipeline
+from .processors import AnyProcessorConfig
+from .filters import AnyFilterConfig
 # utils
 from typing_extensions import Annotated
 
+
 logger = logging.getLogger(__name__)
 
 class DataConfig(pydantic.BaseModel):
     """Data Configuration Model"""
     dataset:str
     splits:dict[str, str] = {
         datasets.Split.TRAIN: datasets.Split.TRAIN,
@@ -53,41 +55,41 @@
 class PrepareConfig(pydantic.BaseModel):
     """Data Configuration Model"""
     # dataset config
     data:DataConfig
     # preprocessing pipeline
     pipeline:list[
         Annotated[
-            hyped.pipeline.AnyProcessorConfig,
+            AnyProcessorConfig,
             pydantic.Field(..., discriminator='processor_type')
         ]
     ]
-    filters:list[hyped.pipeline.AnyFilterConfig]
+    filters:list[AnyFilterConfig]
     # columns to keep
     columns:dict[str, str]
 
     # data filters
     #filters:list[
     #    Annotated[
-    #        hyped.AnyFilterConfig,
+    #        AnyFilterConfig,
     #        pydantic.Field(..., discriminator='filter_type')
     #    ]
     #]
 
 def prepare_dataset(
     ds:datasets.DatasetDict,
     config:PrepareConfig,
     max_size:int | None =None,
 ) -> datasets.DatasetDict:
 
     # get dataset info
     info = next(iter(ds.values())).info
 
     # create pipeline
-    pipe = hyped.pipeline.Pipeline(
+    pipe = Pipeline(
         processors=config.pipeline,
         filters=config.filters
     )
 
     # reduce datasets if they are too large
     for s, d in ds.items():
         if (max_size is not None) and (len(d) > max_size):
@@ -117,54 +119,50 @@
     logger.info("Data Preprocessing Complete.")
     for s, d in ds.items():
         logger.info("Generated %s split of %i documents" % (s, len(d)))
 
     return ds
 
 
-def main():
-    from argparse import ArgumentParser
-    # build argument parser
-    parser = ArgumentParser(description="Prepare dataset for training")
-    parser.add_argument("-c", "--config", type=str, required=True, help="Path to run configuration file in .json format")
-    parser.add_argument("-n", "--max-size", type=int, default=None, help="Maximum number of data points per split")
-    parser.add_argument("-s", "--splits", type=str, nargs='*', default=[], help="Subset of data splits to prepare")
-    parser.add_argument("-o", "--out-dir", type=str, required=True, help="Path to store prepared dataset in")
-    # parse arguments
-    args = parser.parse_args()
+def main(
+    config:str,
+    max_size:int,
+    splits:list[str],
+    out_dir:str,
+    local_rank:int =-1 # not used
+) -> None:
+
+    # register hyped datasets
+    import hyped.datasets
 
     # check if config exists
-    if not os.path.isfile(args.config):
-        raise FileNotFoundError(args.config)
+    if not os.path.isfile(config):
+        raise FileNotFoundError(config)
 
     # load config
-    logger.info("Loading data configuration from %s" % args.config)
-    config = PrepareConfig.parse_file(args.config)
+    logger.info("Loading data configuration from %s" % config)
+    config = PrepareConfig.parse_file(config)
 
     # overwrite splits
-    for split in args.splits:
+    for split in splits:
         if split not in config.data.splits:
-            raise ValueError("Splits `%s` not specified in configuration %s." % (split, args.config))
+            raise ValueError("Splits `%s` not specified in configuration %s." % (split, config))
     # only keep splits that are named in arguments
-    if len(args.splits) > 0:
-        config.data.splits = {s: config.data.splits[s] for s in args.splits}
+    if len(splits) > 0:
+        config.data.splits = {s: config.data.splits[s] for s in splits}
 
     # load dataset splits
     logger.info("Downloading/Loading dataset splits")
     ds = datasets.load_dataset(
         config.data.dataset,
         split=config.data.splits,
         **config.data.kwargs
     )
     # prepare dataset
     logger.info("Preparing dataset splits")
-    ds = prepare_dataset(ds, config, max_size=args.max_size)
+    ds = prepare_dataset(ds, config, max_size=max_size)
 
     # convert dataset dict keys to string for save to disk
     ds = datasets.DatasetDict({str(k): d for k, d in ds.items()})
     # save dataset to disk
-    logger.info("Saving dataset to %s" % args.out_dir)
-    ds.save_to_disk(args.out_dir)
-
-if __name__ == '__main__':
-    logging.basicConfig(level=logging.INFO)
-    main()
+    logger.info("Saving dataset to %s" % out_dir)
+    ds.save_to_disk(out_dir)
```

### Comparing `hyped-0.0.4/hyped/scripts/train.py` & `hyped-0.0.5/hyped/stages/train/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,213 @@
+from __future__ import annotations
+
 import os
 import json
-import hyped
 import datasets
 import transformers
 import pydantic
 import dataclasses
 import logging
 # utils
 from copy import copy
 from datetime import datetime
 from functools import partial
 from itertools import chain, product
-from typing import Any, Optional
+from typing import Any, Optional, Literal
 from typing_extensions import Annotated
+# hyped
+from . import modeling
+from .metrics import HypedAutoMetric
+from .metrics.metrics import AnyHypedMetricConfig
 
 import warnings
 # ignore warning of _n_gpu field of TrainingArguments
 # dataclass when converted to pydantic model
 warnings.filterwarnings(
     "ignore",
     category=RuntimeWarning,
     message="fields may not start with an underscore, ignoring \"_n_gpu\""
 )
 
 # TODO: log more stuff
 logger = logging.getLogger(__name__)
 
-class ModelConfig(pydantic.BaseModel):
-    """Model Configuration Model"""
+class TransformerModelConfig(pydantic.BaseModel):
+    """Transformer Model Configuration Model"""
+    library:Literal['transformers'] = 'transformers'
+    # task and head name
+    task:str
+    head_name:str
+    label_column:str = "labels"
+    # base model
+    pretrained_ckpt:str
+    kwargs:dict ={}
+
+    @pydantic.validator('pretrained_ckpt', pre=True)
+    def _check_pretrained_ckpt(cls, value):
+        try:
+            # check if model is valid by loading config
+            transformers.AutoConfig.from_pretrained(value)
+        except OSError as e:
+            # handle model invalid
+            raise ValueError("Unkown pretrained checkpoint: %s" % value) from e
+
+        return value
+
+    @property
+    def problem_type(self) -> str:
+        problem_type_lookup = {
+            "sequence-classification": "single_label_classification",
+            "multi-label-classification": "multi_label_classification",
+            "sequence-tagging": "token_classification",
+            "causal-language-modeling": "causal-language-modeling"
+        }
+        # check if task is valid
+        if self.task not in problem_type_lookup:
+            raise ValueError("Invalid task `%s`, must be one of %s" % (value, list(problem_type_lookup.keys())))
+        # return problem type for task
+        return problem_type_lookup[self.task]
+
+    @property
+    def auto_class(self) -> type:
+        auto_class_lookup = {
+            "sequence-classification": transformers.AutoModelForSequenceClassification,
+            "multi-label-classification": transformers.AutoModelForSequenceClassification,
+            "sequence-tagging": transformers.AutoModelForTokenClassification,
+            "causal-language-modeling": transformers.AutoModelForCausalLM
+        }
+        # check if task is valid
+        if self.task not in auto_class_lookup:
+            raise ValueError("Invalid task `%s`, must be one of %s" % (value, list(auto_class_lookup.keys())))
+        # return problem type for task
+        return auto_class_lookup[self.task]
+
+    @property
+    def head_config_class(self) -> type:
+        head_config_lookup = {
+            "sequence-classification": modeling.heads.HypedClsHeadConfig,
+            "multi-label-classification": modeling.heads.HypedMlcHeadConfig,
+            "sequence-tagging": modeling.heads.HypedTaggingHeadConfig,
+            "causal-language-modeling": modeling.heads.HypedCausalLMHeadConfig
+        }
+        # check if task is valid
+        if self.task not in head_config_lookup:
+            raise ValueError("Invalid task `%s`, must be one of %s" % (value, list(head_config_lookup.keys())))
+        # return problem type for task
+        return head_config_lookup[self.task]
+
+    def build(self, info:datasets.DatasetInfo) -> transformers.PreTrainedModel:
+
+        # load pretrained config
+        config, kwargs = transformers.AutoConfig.from_pretrained(self.pretrained_ckpt, **self.kwargs, return_unused_kwargs=True)
+
+        # create a head config with the correct labels
+        # only used for generating the label space
+        head_config = self.head_config_class(label_column=self.label_column)
+        head_config.check_and_prepare(info.features)
+        # update num labels and label2id mapping
+        if head_config.num_labels is not None:
+            config.num_labels = head_config.num_labels
+        if head_config.id2label is not None:
+            config.id2label = head_config.id2label
+        # set the problem type, especially important for sequence classification
+        # tells the model whether to solve a single- or multi-label sequence classification task
+        config.problem_type = self.problem_type
+
+        # load pretrained model and wrap it
+        model = self.auto_class.from_pretrained(self.pretrained_ckpt, config=config, **kwargs)
+        model = modeling.TransformerModelWrapper(
+            model,
+            head_name=self.head_name,
+            head_config=head_config
+        )
+        # return wrapped model instance
+        return model
+
+    def build_tokenizer(self) -> transformers.PreTrainedTokenizer:
+        return transformers.AutoTokenizer.from_pretrained(self.pretrained_ckpt, use_fast=True)
+
+    @property
+    def trainer_t(self) -> type[transformers.Trainer]:
+        # use the default transformers trainer
+        return transformers.Trainer
+
+class AdapterTransformerModelConfig(pydantic.BaseModel):
+    """Adapter Transformer Model Configuration Model"""
+    library:Literal['adapter-transformers'] = 'adapter-transformers'
     # base model
     pretrained_ckpt:str
     kwargs:dict ={}
     # adapter setup
     adapter_name:None|str = None # defaults to dataset name
     adapter:None|transformers.adapters.AdapterArguments = None
     # prediction heads
     heads:dict[
         str,
         Annotated[
-            hyped.modeling.heads.AnyHypedHeadConfig,
+            modeling.heads.AnyHypedHeadConfig,
             pydantic.Field(..., discriminator='head_type')
         ]
     ]
 
     def check_and_prepare(self, features:datasets.Features) -> None:
         [hconfig.check_and_prepare(features) for hconfig in self.heads.values()]
 
-    @property
-    def pretrained_config(self) -> transformers.PretrainedConfig:
+    def build(self, info:datasets.DatasetInfo) -> transformers.PreTrainedModel:
+        # set default adapter name and prepare model for data
+        self.adapter_name = self.adapter_name or info.builder_name
+        self.check_and_prepare(info.features)
+
         # load pretrained configuration and wrap for adapter model
-        config = transformers.AutoConfig.from_pretrained(self.pretrained_ckpt)
+        config, kwargs = transformers.AutoConfig.from_pretrained(self.pretrained_ckpt, **self.kwargs, return_unused_kwargs=True)
         config = transformers.adapters.wrappers.configuration.wrap_config(config)
         # add prediction head configs
         config.prediction_heads = {hname: dataclasses.asdict(hconfig) for hname, hconfig in self.heads.items()}
-        # add adapter configs if needed
+
+        # build the model
+        model = modeling.HypedAutoAdapterModel.from_pretrained(
+            self.pretrained_ckpt,
+            config=config,
+            **kwargs
+        )
+        # activate all heads
+        model.active_head = list(model.heads.keys())
+        # set up adapter
         if self.adapter is not None:
+            # check if name is set
             if self.adapter_name is None:
                 raise ValueError("`adapter_name` in model configuration not set!")
-            if self.adapter_name not in config.adapters:
-                adapter_config = transformers.adapters.AdapterConfig.load(self.adapter.adapter_config)
-                config.adapters.add(self.adapter_name, config=adapter_config)
-        # return config
-        return config
+            # set up adapter
+            transformers.adapters.training.setup_adapter_training(
+                model=model,
+                adapter_args=dataclasses.replace(
+                    self.adapter,
+                    train_adapter=True
+                ),
+                adapter_name=self.adapter_name
+            )
+
+            # unfreeze model parameters when not only 
+            # training adapter weights 
+            if not self.adapter.train_adapter:
+                model.freeze_model(False)
+
+        # return model instance
+        return model
+
+    def build_tokenizer(self) -> transformers.PreTrainedTokenizer:
+        return transformers.AutoTokenizer.from_pretrained(self.pretrained_ckpt, use_fast=True)
 
     @property
     def trainer_t(self) -> type[transformers.Trainer]:
         use_adapter_trainer = (self.adapter is not None) and self.adapter.train_adapter
-        return hyped.modeling.MultiHeadAdapterTrainer if use_adapter_trainer else hyped.modeling.MultiHeadTrainer
+        return modeling.MultiHeadAdapterTrainer if use_adapter_trainer else \
+            modeling.MultiHeadTrainer
 
-    @pydantic.validator('pretrained_ckpt')
+    @pydantic.validator('pretrained_ckpt', pre=True)
     def _check_pretrained_ckpt(cls, value):
         try:
             # check if model is valid by loading config
             transformers.AutoConfig.from_pretrained(value)
         except OSError as e:
             # handle model invalid
             raise ValueError("Unkown pretrained checkpoint: %s" % value) from e
@@ -108,14 +243,15 @@
     log_level:Optional[str] ='warning'
     # fields with incomplete types in Training Arguments
     # set type to avoid error in pydantic validation
     debug:str|list[transformers.debug_utils.DebugOption]               =""
     sharded_ddp:str|list[transformers.trainer_utils.ShardedDDPOption]  =""
     fsdp:str|list[transformers.trainer_utils.FSDPOption]               =""
     fsdp_config:Optional[str|dict]                                     =None
+    deepspeed:Optional[str|dict]                                       =None
     # don't do that because we use args and kwargs in the
     # model's forward function which confuses the trainer
     remove_unused_columns:bool =False
 
     # use pytorch implementation of AdamW optimizer
     # to avoid deprecation warning
     optim="adamw_torch"
@@ -141,34 +277,61 @@
         }
 
 class RunConfig(pydantic.BaseModel):
     """Run Configuration Model"""
     # run name
     name:str
     # model and trainer configuration
-    model:ModelConfig
+    model:TransformerModelConfig|AdapterTransformerModelConfig = pydantic.Field(..., discriminator='library')
     trainer:TrainerConfig
     metrics:dict[
         str,
         list[
             Annotated[
-                hyped.evaluate.metrics.AnyHypedMetricConfig,
+                AnyHypedMetricConfig,
                 pydantic.Field(..., discriminator='metric_type')
             ]
         ]
     ]
 
+    @pydantic.validator('model', pre=True)
+    def _infer_model_library(cls, value):
+        if 'library' not in value:
+
+            if ('heads' in value) and ('task' in value):
+                raise ValueError("Could not infer library from model config, both `heads` and `task` field specified!")
+
+            if 'heads' in value:
+                # if heads are present then this is an adapter model
+                value['library'] = "adapter-transformers"
+
+            elif 'task' in value:
+                # if task is specified then this is a pure transformer model
+                value['library'] = "transformers"
+
+            else:
+                raise ValueError("Could not infer library from model config, neither `heads` nor `task` field specified!")
+
+        return value
+
     @pydantic.validator('trainer', pre=True)
     def _pass_name_to_trainer_config(cls, v, values):
         assert 'name' in values
         if isinstance(v, pydantic.BaseModel):
             return v.copy(update={'name': values.get('name')})
         elif isinstance(v, dict):
             return v | {'name': values.get('name')}
 
+def get_format_info(data:datasets.Dataset) -> datasets.Features:
+    return dataclasses.replace(
+        data.info,
+        task_templates=[],
+        features=data.info.features.copy() if data.format['columns'] is None else \
+            datasets.Features({n: data.info.features[n] for n in data.format['columns']})
+    )
 
 def load_data_split(path:str, split:str) -> datasets.Dataset:
     # check if specific dataset split exists
     dpath = os.path.join(path, str(split))
     if not os.path.isdir(dpath):
         raise FileNotFoundError(dpath)
     # load split
@@ -214,141 +377,122 @@
         split: datasets.concatenate_datasets(data, info=combine_infos([d.info for d in data]), split=split)
         for split, data in ds.items()
         if len(data) > 0
     })
 
 def build_trainer(
     trainer_t:type[transformers.Trainer],
+    info:datasets.DatasetInfo,
+    tokenizer:transformers.PreTrainedTokenizer,
     model:transformers.PreTrainedModel,
     args:transformers.TrainingArguments,
-    features:datasets.Features,
-    metric_configs:dict[str, hyped.evaluate.metrics.AnyHypedMetricConfig],
-    output_dir:str = None,
-    disable_tqdm:bool =False
+    metric_configs:dict[str, AnyHypedMetricConfig],
+    local_rank:int =-1
 ) -> transformers.Trainer:
     """Create trainer instance ensuring correct interfacing between trainer and metrics"""
 
-    # create fixed order over label names
+    # create fixed order over label names for all model heads
     label_names = chain.from_iterable(h.get_label_names() for h in model.heads.values())
     label_names = list(set(list(label_names)))
-    # specify label columns and overwrite output directory if given
+    # set label names order in arguments
     args.label_names = label_names
-    args.output_dir = output_dir or args.output_dir
-    # disable tqdm
-    args.disable_tqdm = disable_tqdm
+    # update local rank in trainer configuration
+    args.local_rank = local_rank
 
     # create metrics
-    metrics = hyped.evaluate.HypedAutoMetric.from_model(
+    metrics = HypedAutoMetric.from_model(
         model=model,
         metric_configs=metric_configs,
         label_order=args.label_names
     )
 
     # create data collator
-    collator = hyped.modeling.HypedDataCollator(
+    collator = modeling.HypedDataCollator(
+        tokenizer=tokenizer,
         heads=model.heads.values(),
-        features=features
+        features=info.features
     )
 
     # create trainer instance
-    return trainer_t(
+    trainer = trainer_t(
         model=model,
         args=args,
         # datasets need to be set manually
         train_dataset=None,
         eval_dataset=None,
         # data collator
         data_collator=collator,
         # compute metrics
         preprocess_logits_for_metrics=metrics.preprocess,
         compute_metrics=metrics.compute
     )
+    # add early stopping callback
+    trainer.add_callback(
+        transformers.EarlyStoppingCallback(
+            early_stopping_patience=args.early_stopping_patience,
+            early_stopping_threshold=args.early_stopping_threshold
+        )
+    )
+    # return trainer instance
+    return trainer
 
 def train(
     config:RunConfig,
     ds:datasets.DatasetDict,
     output_dir:str = None,
+    local_rank:int = -1,
     disable_tqdm:bool = False
 ) -> transformers.Trainer:
 
     # check for train and validation datasets
     if datasets.Split.TRAIN not in ds:
         raise KeyError("No train dataset found, got %s!" % list(ds.keys()))
     if datasets.Split.VALIDATION not in ds:
         raise KeyError("No validation dataset found, got %s!" % list(ds.keys()))
 
-    # set default adapter name
-    config.model.adapter_name = config.model.adapter_name or \
-        ds[datasets.Split.TRAIN].info.builder_name
-
-    # prepare model for data
-    features = ds[datasets.Split.TRAIN].info.features
-    config.model.check_and_prepare(features)
-    # build the model
-    model = hyped.modeling.HypedAutoAdapterModel.from_pretrained(
-        config.model.pretrained_ckpt,
-        config=config.model.pretrained_config,
-        **config.model.kwargs
-    )
-    # activate all heads
-    model.active_head = list(model.heads.keys())
-    # set up adapter
-    if config.model.adapter is not None:
-        transformers.adapters.training.setup_adapter_training(
-            model=model,
-            adapter_args=config.model.adapter,
-            adapter_name=config.model.adapter_name
-        )
-
+    # update trainer arguments
+    config.trainer.output_dir = output_dir or args.output_dir
+    config.trainer.disable_tqdm = disable_tqdm
+
+    # get dataset info but replace features with restricted features
+    data = next(iter(ds.values()))
+    info = get_format_info(data)
+    # build model and trainer
     trainer = build_trainer(
         trainer_t=config.model.trainer_t,
-        model=model,
+        info=info,
+        tokenizer=config.model.build_tokenizer(),
+        model=config.model.build(info),
         args=config.trainer,
-        features=features,
         metric_configs=config.metrics,
-        output_dir=output_dir,
-        disable_tqdm=disable_tqdm
-    )
-    # set train and validation datasets
-    trainer.train_dataset=ds[datasets.Split.TRAIN]
-    trainer.eval_dataset=ds[datasets.Split.VALIDATION]
-    # add early stopping callback
-    trainer.add_callback(
-        transformers.EarlyStoppingCallback(
-            early_stopping_patience=config.trainer.early_stopping_patience,
-            early_stopping_threshold=config.trainer.early_stopping_threshold
-        )
+        local_rank=local_rank
     )
+    # set datasets
+    trainer.train_dataset = ds[datasets.Split.TRAIN]
+    trainer.eval_dataset = ds[datasets.Split.VALIDATION]
 
     # run trainer
     trainer.train()
 
     return trainer
 
-def main():
-    from argparse import ArgumentParser
-    # build argument parser
-    parser = ArgumentParser(description="Train Transformer model on prepared datasets")
-    parser.add_argument("-c", "--config", type=str, required=True, help="Path to run configuration file in .json format")
-    parser.add_argument("-d", "--data", type=str, nargs='+', required=True, help="Paths to prepared data dumps")
-    parser.add_argument("-o", "--out-dir", type=str, default=None, help="Output directory, by default uses directoy specified in config")
-    # parse arguments
-    args = parser.parse_args()
-
+def main(
+    config:str,
+    data:list[str],
+    out_dir:str,
+    local_rank:int =-1
+) -> None:
     # check if config exists
-    if not os.path.isfile(args.config):
-        raise FileNotFoundError(args.config)
+    if not os.path.isfile(config):
+        raise FileNotFoundError(config)
+
     # load config
-    logger.info("Loading run configuration from %s" % args.config)
-    config = RunConfig.parse_file(args.config)
+    logger.info("Loading run configuration from %s" % config)
+    config = RunConfig.parse_file(config)
 
     # run training
     splits = [datasets.Split.TRAIN, datasets.Split.VALIDATION]
-    trainer = train(config, collect_data(args.data, splits), args.out_dir)
+    trainer = train(config, collect_data(data, splits), out_dir, local_rank)
 
     # save trainer model in output directory if given
-    if args.out_dir is not None:
-        trainer.save_model(os.path.join(args.out_dir, "best-model"))
-
-if __name__ == '__main__':
-    logging.basicConfig(level=logging.INFO)
-    main()
+    if out_dir is not None:
+        trainer.save_model(os.path.join(out_dir, "best-model"))
```

### Comparing `hyped-0.0.4/hyped/utils/typedlist.py` & `hyped-0.0.5/hyped/utils/typedlist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped/utils/typedmapping.py` & `hyped-0.0.5/hyped/utils/typedmapping.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.4/hyped.egg-info/PKG-INFO` & `hyped-0.0.5/hyped.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of data pipelines to ease the training of transformer models
 Home-page: https://github.com/ndoll1998/hyped/tree/master
 Author: Niclas Doll
 Author-email: niclas@amazonis.net
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
@@ -49,53 +49,95 @@
 The following demonstates how to train a text classification model on the [`imdb`](https://huggingface.co/datasets/imdb) dataset by going through all three stages of the ML pipeline (from `examples/run.sh`).
 
 ```bash
 # data preparation stage
 # runs the data preparation pipeline specified in the
 # configuration file and saves the prepared dataset
 # to the specified location
-python -m hyped.scripts.prepare \
+python -m hyped.stages.prepare \
     -c examples/text_cls/imdb/distilbert_data.json \
     -o output/distilbert_data
 
 # model training stage
 # trains a model on the prepared data generated by the
 # previous stage
-python -m hyped.scripts.train \
+python -m hyped.stages.train \
     -c examples/text_cls/imdb/distilbert_run.json \
     -d output/distilbert_data \
     -o output/model
 
 # model evaluation stage
 # evaluates the trained model on the test split of the
 # prepared dataset generated earlier
-python -m hyped.scripts.evaluate \
+python -m hyped.stages.evaluate \
     -c examples/text_cls/imdb/distilbert_run.json \
     -d output/distilbert_data \
     -m output/model/best-model
 ```
 
 ## features
 
 `hyped` currently implements all components required to train and evaluate models for the following NLP tasks:
 
  - Text Classification
  - Named Entity Recognition
  - Multi-label Classification
+ - Causal Language Modeling
 
+### adapters
+
+`hyped` is build upon [`adapter-transformers`](https://docs.adapterhub.ml/), which allows the configuration of a variety of model architectures. See the following excerpt for how to configure an adapter model in the run configuration (from [`examples/cls/imdb/distilbert_run.json`](examples/cls/imdb/distilbert_run.json)):
+
+```json
+{
+    "model": {
+        "pretrained_ckpt": "distilbert-base-uncased",
+        
+        "adapter_name": "imdb",
+        "adapter": {
+            "train_adapter": true,
+            "adapter_config": "pfeiffer"
+        },
+
+        "heads": {
+            "cls": {
+                "head_type": "hyped-cls-head",
+                "label_column": "labels"
+            }
+        }
+    }
+}
+```
+
+The `adapter` field in the above configuration mirrors the [`AdapterArguments`](https://docs.adapterhub.ml/classes/adapter_training.html#transformers.adapters.training.AdapterArguments) class and can specify all it's values (e.g. `load_adapter` for loading pretrained adapters). Furthermore, by setting `train_adapter` to True, only the paramters of the adapter and head are trained, while the pretrained encoder parameters are frozen.
+
+Alternatively, the adapter configuration can also be omitted, in which case no adapter is used and the encoder output is directly passed to the prediction heads.
+
+### dvc
+
+`hyped` is designed to be easily integratable into existing data pipelines. Thus, it fits well with [`dvc`](https://dvc.org/) pipelines. See [`examples/dvc`](examples/dvc) for an example setup.
+
+### deepspeed
+
+`hyped` supports distributed training allowing for both pre-training and fine-tuning of very large language models. See [`examples/lm/run.json`](examples/lm/run.json) for an example configuration. To lauch a distributed training you need to use `hyped`'s command line interface:
+
+```bash
+deepspeed --no_python hyped train -c config.json -d data/ -o model/
+```
 
 ## roadmap
 
-`hyped` is still in its very early stages. With time the goal is to make the framework applicable to a wide variety of tasks and setups. Planned features include the following:
+`hyped` is currently in its early stages of development. Over time, the goal is to expand its applicability to a diverse range of tasks and setups. The following features are planned for future development:
 
  - ~~support adapter training~~
+ - ~~support transformers models~~
  - support more tasks
    - Masked Language Modeling
-   - Causal Language Modeling
+   - ~~Causal Language Modeling~~
    - nested Named Entity Recognition
    - Question Answering
  - support multi-modal encoders
    - LayoutLM
    - LiLT
  - support distributed training/inference
-   - deepspeed
+   - ~~deepspeed~~
    - pytorch DDP and FSDP
```

### Comparing `hyped-0.0.4/setup.py` & `hyped-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hyped",
-    version="0.0.4",
+    version="0.0.5",
     description="A collection of data pipelines to ease the training of transformer models",
     long_description=open("README.md", "r").read(),
     long_description_content_type='text/markdown',
     author="Niclas Doll",
     author_email="niclas@amazonis.net",
     url="https://github.com/ndoll1998/hyped/tree/master",
     packages=find_packages(exclude='tests'),
@@ -18,9 +18,14 @@
     ],
     install_requires=[
         'adapter-transformers>=3.2.1',
         'datasets>=2.12.0',
         'evaluate>=0.4.0',
         'torch>=2.0.0',
         'pydantic>=1.10.7'
-    ]
+    ],
+    entry_points={
+        "console_scripts": [
+            'hyped = hyped.cli:main'
+        ]
+    }
 )
```

