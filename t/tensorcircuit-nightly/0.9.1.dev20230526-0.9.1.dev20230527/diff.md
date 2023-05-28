# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230526.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230526.tar", last modified: Fri May 26 12:39:19 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230527.tar", last modified: Sat May 27 12:37:15 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230526.tar` & `tensorcircuit-nightly-0.9.1.dev20230527.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/
--rw-r--r--   0 runner    (1001) docker     (122)    25259 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18978 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6448 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.797004 tensorcircuit-nightly-0.9.1.dev20230526/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.801004 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-26 12:39:13.000000 tensorcircuit-nightly-0.9.1.dev20230526/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-26 12:39:13.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10766 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.567785 tensorcircuit-nightly-0.9.1.dev20230527/
+-rw-r--r--   0 runner    (1001) docker     (122)    25330 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-27 12:37:15.563785 tensorcircuit-nightly-0.9.1.dev20230527/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18978 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6448 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.551785 tensorcircuit-nightly-0.9.1.dev20230527/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.555785 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6356 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5892 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-27 12:37:15.567785 tensorcircuit-nightly-0.9.1.dev20230527/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-27 12:37:09.000000 tensorcircuit-nightly-0.9.1.dev20230527/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-27 12:37:09.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14325 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10766 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.559785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.563785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.563785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.563785 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-27 12:37:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-27 12:37:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 12:37:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-27 12:37:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-27 12:37:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 12:37:15.563785 tensorcircuit-nightly-0.9.1.dev20230527/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-27 12:15:15.000000 tensorcircuit-nightly-0.9.1.dev20230527/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230527/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 - `c.expectation_ps()` now also supports `ps` argument directly (pauli structures)
 
 - Add tc version print in `tc.about()` method
 
 - tc now supports fancy batch indexing for gates, e.g. `c.rxx([0, 1, 2], [1, 2, 3], theta=K.ones([3]))`
 
+- Task management via group tag (when `submit_task` and `list_tasks`)
+
 ### Fixed
 
 - `tc.results.counts.plot_histogram` now can dispatch kws to corresponding qiskit method
 
 - New implementation for `c.inverse()` to partially avoid unrecognized gate name issue
 
 - Fixed bug for `batch_expectation_ps` for jax backend
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230527/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230527/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230527/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230526
+Version: 0.9.1.dev20230527
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/README.md` & `tensorcircuit-nightly-0.9.1.dev20230527/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230527/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/cnconf.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.ifconfig",
     "sphinx_copybutton",
     "nbsphinx",
     "toctree_filter",
+    "sphinx.ext.napoleon",
     "myst_parser",
+    "sphinx_design",
 ]
 
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.ifconfig",
     "sphinx_copybutton",
     "nbsphinx",
     "toctree_filter",
     "sphinx.ext.napoleon",
     "myst_parser",
+    "sphinx_design",
 ]
 
 nbsphinx_allow_errors = True
 
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230527/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230527/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230526"
+__version__ = "0.9.1.dev20230527"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/tencent.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     lang: str = "OPENQASM",
     shots: Union[int, Sequence[int]] = 1024,
     version: str = "1",
     prior: int = 1,
     circuit: Optional[Union[AbstractCircuit, Sequence[AbstractCircuit]]] = None,
     source: Optional[Union[str, Sequence[str]]] = None,
     remarks: Optional[str] = None,
+    group: Optional[str] = None,
     compiling: bool = False,
     compiled_options: Optional[Dict[str, Any]] = None,
     enable_qiskit_initial_mapping: bool = False,
     # measure: Optional[Sequence[int]] = None,
     enable_qos_qubit_mapping: bool = True,
     enable_qos_gate_decomposition: bool = True,
     enable_qos_initial_mapping: bool = False,
@@ -257,26 +258,28 @@
                     "device": device_str,
                     "shots": sh,
                     "source": sc,
                     "version": version,
                     "lang": lang,
                     "prior": prior,
                     "remarks": remarks,
+                    "group": group,
                 }
             )
 
     else:
         json = {  # type: ignore
             "device": device_str,
             "shots": shots,
             "source": source,
             "version": version,
             "lang": lang,
             "prior": prior,
             "remarks": remarks,
+            "group": group,
         }
     r = rpost_json(
         tencent_base_url + "task/submit", json=json, headers=tencent_headers(token)
     )
     r = error_handling(r)
     rtn = []
     for t in r["tasks"]:
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230526
+Version: 0.9.1.dev20230527
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230527/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230527/tests/test_van.py`

 * *Files identical despite different names*

