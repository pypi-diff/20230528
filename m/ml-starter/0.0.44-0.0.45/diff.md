# Comparing `tmp/ml-starter-0.0.44.tar.gz` & `tmp/ml-starter-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.44.tar", last modified: Wed May 24 20:47:28 2023, max compression
+gzip compressed data, was "ml-starter-0.0.45.tar", last modified: Sat May 27 22:05:25 2023, max compression
```

## Comparing `ml-starter-0.0.44.tar` & `ml-starter-0.0.45.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.963292 ml-starter-0.0.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 20:47:15.000000 ml-starter-0.0.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 20:47:15.000000 ml-starter-0.0.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 20:47:28.963292 ml-starter-0.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-24 20:47:15.000000 ml-starter-0.0.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.931290 ml-starter-0.0.44/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.931290 ml-starter-0.0.44/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.931290 ml-starter-0.0.44/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.931290 ml-starter-0.0.44/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.935291 ml-starter-0.0.44/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.935291 ml-starter-0.0.44/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.935291 ml-starter-0.0.44/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.939291 ml-starter-0.0.44/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60524 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.939291 ml-starter-0.0.44/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.943291 ml-starter-0.0.44/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.943291 ml-starter-0.0.44/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.943291 ml-starter-0.0.44/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.943291 ml-starter-0.0.44/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.947291 ml-starter-0.0.44/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.947291 ml-starter-0.0.44/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.947291 ml-starter-0.0.44/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.947291 ml-starter-0.0.44/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.951291 ml-starter-0.0.44/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.959292 ml-starter-0.0.44/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.959292 ml-starter-0.0.44/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-24 20:47:15.000000 ml-starter-0.0.44/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:47:28.963292 ml-starter-0.0.44/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 20:47:28.000000 ml-starter-0.0.44/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-24 20:47:28.000000 ml-starter-0.0.44/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:47:28.000000 ml-starter-0.0.44/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 20:47:28.000000 ml-starter-0.0.44/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-24 20:47:28.000000 ml-starter-0.0.44/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 20:47:15.000000 ml-starter-0.0.44/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 20:47:15.000000 ml-starter-0.0.44/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 20:47:15.000000 ml-starter-0.0.44/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 20:47:15.000000 ml-starter-0.0.44/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 20:47:28.963292 ml-starter-0.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 20:47:15.000000 ml-starter-0.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.268329 ml-starter-0.0.45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 22:05:13.000000 ml-starter-0.0.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 22:05:13.000000 ml-starter-0.0.45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-27 22:05:25.268329 ml-starter-0.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 22:05:13.000000 ml-starter-0.0.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.252328 ml-starter-0.0.45/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.252328 ml-starter-0.0.45/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.252328 ml-starter-0.0.45/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.256328 ml-starter-0.0.45/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.256328 ml-starter-0.0.45/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.256328 ml-starter-0.0.45/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.256328 ml-starter-0.0.45/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.256328 ml-starter-0.0.45/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60524 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.260328 ml-starter-0.0.45/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.260328 ml-starter-0.0.45/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.260328 ml-starter-0.0.45/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.260328 ml-starter-0.0.45/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.260328 ml-starter-0.0.45/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.264329 ml-starter-0.0.45/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.264329 ml-starter-0.0.45/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.264329 ml-starter-0.0.45/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.264329 ml-starter-0.0.45/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.264329 ml-starter-0.0.45/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.268329 ml-starter-0.0.45/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.268329 ml-starter-0.0.45/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-27 22:05:13.000000 ml-starter-0.0.45/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:05:25.268329 ml-starter-0.0.45/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-27 22:05:25.000000 ml-starter-0.0.45/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-27 22:05:25.000000 ml-starter-0.0.45/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 22:05:25.000000 ml-starter-0.0.45/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 22:05:25.000000 ml-starter-0.0.45/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-27 22:05:25.000000 ml-starter-0.0.45/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-27 22:05:13.000000 ml-starter-0.0.45/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 22:05:13.000000 ml-starter-0.0.45/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 22:05:13.000000 ml-starter-0.0.45/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-27 22:05:13.000000 ml-starter-0.0.45/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-27 22:05:25.272329 ml-starter-0.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-27 22:05:13.000000 ml-starter-0.0.45/setup.py
```

### Comparing `ml-starter-0.0.44/LICENSE` & `ml-starter-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/PKG-INFO` & `ml-starter-0.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.44
+Version: 0.0.45
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.44/README.md` & `ml-starter-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/api.py` & `ml-starter-0.0.45/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/core/common_types.py` & `ml-starter-0.0.45/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/core/config.py` & `ml-starter-0.0.45/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/core/env.py` & `ml-starter-0.0.45/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/core/registry.py` & `ml-starter-0.0.45/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/core/state.py` & `ml-starter-0.0.45/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/launchers/base.py` & `ml-starter-0.0.45/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/launchers/mp.py` & `ml-starter-0.0.45/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/launchers/slurm.py` & `ml-starter-0.0.45/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/launchers/torchrun.py` & `ml-starter-0.0.45/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/loggers/base.py` & `ml-starter-0.0.45/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/loggers/meter.py` & `ml-starter-0.0.45/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/loggers/multi.py` & `ml-starter-0.0.45/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/loggers/stdout.py` & `ml-starter-0.0.45/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/loggers/tensorboard.py` & `ml-starter-0.0.45/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/base.py` & `ml-starter-0.0.45/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/constant.py` & `ml-starter-0.0.45/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.45/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.45/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/linear.py` & `ml-starter-0.0.45/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.45/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.45/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/activations.py` & `ml-starter-0.0.45/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/base.py` & `ml-starter-0.0.45/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/embeddings.py` & `ml-starter-0.0.45/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/init.py` & `ml-starter-0.0.45/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/kmeans.py` & `ml-starter-0.0.45/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/lora.py` & `ml-starter-0.0.45/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/norms.py` & `ml-starter-0.0.45/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/parallel.py` & `ml-starter-0.0.45/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/blip.py` & `ml-starter-0.0.45/ml/models/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/clip.py` & `ml-starter-0.0.45/ml/models/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/hubert.py` & `ml-starter-0.0.45/ml/models/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/llama.py` & `ml-starter-0.0.45/ml/models/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/rwkv.py` & `ml-starter-0.0.45/ml/models/pretrained/rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/models/pretrained/sam.py` & `ml-starter-0.0.45/ml/models/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/adam.py` & `ml-starter-0.0.45/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/adamw.py` & `ml-starter-0.0.45/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/adan.py` & `ml-starter-0.0.45/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/base.py` & `ml-starter-0.0.45/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/common.py` & `ml-starter-0.0.45/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/sgd.py` & `ml-starter-0.0.45/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/optimizers/shampoo.py` & `ml-starter-0.0.45/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/scripts/cli.py` & `ml-starter-0.0.45/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/scripts/stage.py` & `ml-starter-0.0.45/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/scripts/train.py` & `ml-starter-0.0.45/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/base.py` & `ml-starter-0.0.45/ml/tasks/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 :class:`ml.tasks.sl.SupervisedLearningTask` or
 :class:`ml.tasks.rl.ReinforcementLearningTask` classes instead of this base
 class.
 """
 
 import functools
 import logging
+import os
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, is_dataclass
 from pathlib import Path
 from typing import Any, Generic, Mapping, Sequence, Sized, TypeVar
 
 import numpy as np
 import torch
-from omegaconf import II, MISSING
+from omegaconf import II, MISSING, OmegaConf
 from torch import Tensor, nn
 from torch.optim.optimizer import Optimizer
 from torch.utils.data.dataloader import DataLoader
 from torch.utils.data.dataset import Dataset
 from torch.utils.data.sampler import Sampler
 
 from ml.core.common_types import Batch, Loss, Output
 from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.env import is_debugging
-from ml.core.state import Phase, State, cast_phase
+from ml.core.state import Phase, State
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.models.base import BaseModel
 from ml.tasks.datasets.collate import CollateMode, collate
 from ml.tasks.datasets.error_handling import (
     ErrorHandlingConfig,
     get_error_handling_dataset,
@@ -44,14 +45,24 @@
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.random import set_random_seed
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+def num_workers(default: int) -> int:
+    if (cpu_count := os.cpu_count()) is None:
+        return default
+    # This is a somewhat arbitrary heuristic, but seems to be a fine default.
+    return min(cpu_count * 2, 8)
+
+
+OmegaConf.register_new_resolver("ml.num_workers", num_workers, replace=True)
+
+
 class CumulativeTimer:
     """Defines a simple timer to track an average value."""
 
     def __init__(self) -> None:
         self.steps = 0
         self.elapsed_time = 0.0
 
@@ -148,61 +159,67 @@
     drop_last: bool = conf_field(MISSING, help="Should the last batch be dropped if not full")
     timeout: float = conf_field(0, help="How long to wait for a sample to be ready")
     prefetch_factor: int | None = conf_field(None, help="Number of items to pre-fetch on each worker")
     persistent_workers: bool = conf_field(False, help="Persist worker processes between epochs")
     seed: int = conf_field(1337, help="Dataloader random seed")
 
 
-DEFAULT_DATALOADER_CONFIGS: dict[str, DataLoaderConfig] = {
-    "train": DataLoaderConfig(
-        shuffle=True,
-        num_workers=8,
-        pin_memory=True,
-        drop_last=True,
-        persistent_workers=True,
-    ),
-    "valid": DataLoaderConfig(
-        batch_size=II("task.dataloader.train.batch_size"),
-        shuffle=True,
-        num_workers=0,
-        pin_memory=False,
-        drop_last=False,
-        persistent_workers=False,
-    ),
-    "test": DataLoaderConfig(
-        batch_size=II("task.dataloader.valid.batch_size"),
-        shuffle=False,
-        num_workers=0,
-        pin_memory=False,
-        drop_last=False,
-        persistent_workers=False,
-    ),
-}
+@dataclass
+class DataLoaderConfigs:
+    train_dl: DataLoaderConfig = conf_field(
+        DataLoaderConfig(
+            shuffle=True,
+            num_workers=II("ml.num_workers:8"),
+            pin_memory=True,
+            drop_last=True,
+            persistent_workers=True,
+        ),
+        help="Train dataloader config",
+    )
+    valid_dl: DataLoaderConfig = conf_field(
+        DataLoaderConfig(
+            batch_size=II("task.train_dl.batch_size"),
+            shuffle=True,
+            num_workers=0,
+            pin_memory=False,
+            drop_last=False,
+            persistent_workers=False,
+        ),
+        help="Valid dataloader config",
+    )
+    test_dl: DataLoaderConfig = conf_field(
+        DataLoaderConfig(
+            batch_size=II("task.valid_dl.batch_size"),
+            shuffle=False,
+            num_workers=0,
+            pin_memory=False,
+            drop_last=False,
+            persistent_workers=False,
+        ),
+        help="Test dataloader config",
+    )
 
 
 @dataclass
 class FinishTrainingConfig:
     max_epochs: int | None = conf_field(None, help="Maximum number of epochs to run")
     max_steps: int | None = conf_field(None, help="Maximum number of steps to run")
     max_samples: int | None = conf_field(None, help="Maximum number of samples to run")
 
 
 @dataclass
 class LossConfig:
-    reduce_type: str = conf_field("sum", help="Loss reduction type to use")
+    loss_reduce_type: str = conf_field("sum", help="Loss reduction type to use")
 
 
 @dataclass
-class BaseTaskConfig(BaseConfig):
+class BaseTaskConfig(BaseConfig, DataLoaderConfigs, FinishTrainingConfig, LossConfig):
     """Defines the base config for all tasks."""
 
-    finished: FinishTrainingConfig = conf_field(FinishTrainingConfig(), help="Finish training config")
-    error_handling: ErrorHandlingConfig = conf_field(ErrorHandlingConfig(), help="Error handling config")
-    dataloader: dict[str, DataLoaderConfig] = conf_field(DEFAULT_DATALOADER_CONFIGS, help="Dataloader config")
-    loss: LossConfig = conf_field(LossConfig(), help="Loss config")
+    errors: ErrorHandlingConfig = conf_field(ErrorHandlingConfig(), help="Error handling config")
 
 
 BaseTaskConfigT = TypeVar("BaseTaskConfigT", bound=BaseTaskConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 
 
 class BaseTask(
@@ -214,30 +231,32 @@
     """Defines the base task type."""
 
     def __init__(self, config: BaseTaskConfigT) -> None:
         nn.Module.__init__(self)
         BaseObject.__init__(self, config)
 
         self.dataloader_configs: dict[Phase, DataLoaderConfig] = {
-            cast_phase(k): v for k, v in config.dataloader.items()
+            "train": self.config.train_dl,
+            "valid": self.config.valid_dl,
+            "test": self.config.test_dl,
         }
 
         # This flag can be toggled to end training from anywhere in the task.
         self.__training_over_flag = False
 
         # Timers for iterations.
         self.train_timer = StateTimer()
         self.valid_timer = StateTimer()
         self.test_timer = StateTimer()
 
         # Used to log values.
         self.logger = MultiLogger(default_namespace="task")
 
         # Final loss reduce type.
-        self.__final_loss_reduce_type = cast_reduce_type(self.config.loss.reduce_type)
+        self.__final_loss_reduce_type = cast_reduce_type(self.config.loss_reduce_type)
 
     @functools.cached_property
     @torch.jit.ignore
     def _device(self) -> type[BaseDevice]:
         return AutoDevice.detect_device()
 
     @functools.cached_property
```

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.45/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.45/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/collate.py` & `ml-starter-0.0.45/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.45/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.45/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.45/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.45/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.45/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/utils.py` & `ml-starter-0.0.45/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.45/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/environments/base.py` & `ml-starter-0.0.45/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/environments/utils.py` & `ml-starter-0.0.45/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/environments/worker.py` & `ml-starter-0.0.45/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/losses/reduce.py` & `ml-starter-0.0.45/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/rl/base.py` & `ml-starter-0.0.45/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/rl/replay.py` & `ml-starter-0.0.45/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/tasks/sl/base.py` & `ml-starter-0.0.45/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/base.py` & `ml-starter-0.0.45/ml/trainers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 from ml.utils.device.base import BaseDevice, Prefetcher
 from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def resolve(path: str) -> str:
+def abs_path(path: str) -> str:
     return str(Path(path).resolve())
 
 
 def cpu_count(default: int) -> int:
     if (cpu_count := os.cpu_count()) is not None:
         return cpu_count
     return default
 
 
-OmegaConf.register_new_resolver("resolve", resolve)
-OmegaConf.register_new_resolver("cpu_count", cpu_count)
+OmegaConf.register_new_resolver("ml.abs_path", abs_path, replace=True)
+OmegaConf.register_new_resolver("ml.cpu_count", cpu_count, replace=True)
 
 LockType = Literal["running", "scheduled", "ckpt"]
 
 
 def add_lock_file(exp_dir: Path, lock_type: LockType, *, exists_ok: bool = False) -> None:
     if is_master():
         if (lock_file := exp_dir / f".lock_{lock_type}").exists():
@@ -216,17 +216,17 @@
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
 
-    exp_name: str = conf_field(II("exp_name:null"), help="The name of the training job")
+    exp_name: str = conf_field(II("ml.exp_name:null"), help="The name of the training job")
     log_dir_name: str = conf_field("logs", help="Name of the subdirectory which contains logs")
-    base_run_dir: str = conf_field(II("resolve:${oc.env:RUN_DIR}"), help="The base directory for all runs")
+    base_run_dir: str = conf_field(II("ml.abs_path:${oc.env:RUN_DIR}"), help="The base directory for all runs")
     run_id: int = conf_field(MISSING, help="The run ID to use")
     use_double_weight_precision: bool = conf_field(False, help="If set, use doubles for weights instead of floats")
     checkpoint: CheckpointConfig = conf_field(CheckpointConfig())
 
     @classmethod
     def resolve(cls, config: "BaseTrainerConfig") -> None:
         if OmegaConf.is_missing(config, "run_id"):
```

### Comparing `ml-starter-0.0.44/ml/trainers/learning.py` & `ml-starter-0.0.45/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/compile.py` & `ml-starter-0.0.45/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.45/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.45/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.45/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.45/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.45/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.45/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.45/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.45/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.45/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/rl.py` & `ml-starter-0.0.45/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/trainers/sl.py` & `ml-starter-0.0.45/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/argparse.py` & `ml-starter-0.0.45/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/atomic.py` & `ml-starter-0.0.45/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/augmentation.py` & `ml-starter-0.0.45/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/caching.py` & `ml-starter-0.0.45/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/checkpoint.py` & `ml-starter-0.0.45/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/cli.py` & `ml-starter-0.0.45/ml/utils/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,15 @@
     # Parses all of the additional config overrides.
     if len(args) > 0:
         split_args = [a.split("=") for a in args]
         assert all(len(a) == 2 for a in split_args), f"Got invalid arguments: {[a for a in split_args if len(a) != 2]}"
         argument_parts += [f"{k.split('.')[-1]}_{v}" for k, v in sorted(split_args) if k not in IGNORE_ARGS]
 
     # Registers an OmegaConf resolver with the job name.
-    if not OmegaConf.has_resolver("exp_name"):
-        OmegaConf.register_new_resolver("exp_name", partial(get_exp_name, args=argument_parts))
+    OmegaConf.register_new_resolver("ml.exp_name", partial(get_exp_name, args=argument_parts), replace=True)
     set_exp_name(get_exp_name(args=argument_parts))
 
     # Finally, builds the config.
     try:
         for path in paths:
             config = cast(DictConfig, OmegaConf.merge(config, OmegaConf.load(path)))
         config = cast(DictConfig, OmegaConf.merge(config, OmegaConf.from_dotlist(args)))
```

### Comparing `ml-starter-0.0.44/ml/utils/colors.py` & `ml-starter-0.0.45/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/config.py` & `ml-starter-0.0.45/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/data.py` & `ml-starter-0.0.45/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/datetime.py` & `ml-starter-0.0.45/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/device/auto.py` & `ml-starter-0.0.45/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/device/base.py` & `ml-starter-0.0.45/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/device/cpu.py` & `ml-starter-0.0.45/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/device/gpu.py` & `ml-starter-0.0.45/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/device/metal.py` & `ml-starter-0.0.45/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/distributed.py` & `ml-starter-0.0.45/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/image.py` & `ml-starter-0.0.45/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/large_models.py` & `ml-starter-0.0.45/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/logging.py` & `ml-starter-0.0.45/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/meter.py` & `ml-starter-0.0.45/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/parallel.py` & `ml-starter-0.0.45/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/staging.py` & `ml-starter-0.0.45/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/timer.py` & `ml-starter-0.0.45/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/torch_distributed.py` & `ml-starter-0.0.45/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml/utils/video.py` & `ml-starter-0.0.45/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.45/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.44
+Version: 0.0.45
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.44/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.45/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/pyproject.toml` & `ml-starter-0.0.45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.44/setup.py` & `ml-starter-0.0.45/setup.py`

 * *Files identical despite different names*

