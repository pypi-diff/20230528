# Comparing `tmp/quantumflow-1.2.1.tar.gz` & `tmp/quantumflow-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumflow-1.2.1.tar", last modified: Tue Dec  7 15:23:00 2021, max compression
+gzip compressed data, was "quantumflow-1.3.0.tar", last modified: Sun May 28 16:48:10 2023, max compression
```

## Comparing `quantumflow-1.2.1.tar` & `quantumflow-1.3.0.tar`

### file list

```diff
@@ -1,150 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.201986 quantumflow-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.177986 quantumflow-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.181986 quantumflow-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2021-12-07 15:22:45.000000 quantumflow-1.2.1/.github/workflows/python-build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      865 2021-12-07 15:22:45.000000 quantumflow-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-12-07 15:22:45.000000 quantumflow-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-12-07 15:22:45.000000 quantumflow-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-07 15:22:45.000000 quantumflow-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2021-12-07 15:22:45.000000 quantumflow-1.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-12-07 15:23:00.201986 quantumflow-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-12-07 15:22:45.000000 quantumflow-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.185986 quantumflow-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.185986 quantumflow-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/_static/qf.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.185986 quantumflow-1.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/bibtex.json
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/channels.rst
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/circuits.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/decomp.rst
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/devnotes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/gates.rst
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/gradients.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/info.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5106 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/ops.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/pauli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/qubits.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/states.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/transform.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/translate.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/xcirq.rst
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/xforest.rst
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/xqiskit.rst
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/xquirk.rst
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-07 15:22:45.000000 quantumflow-1.2.1/docs/zreferences.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.185986 quantumflow-1.2.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)      766 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/circuit_compilation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18925 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/circuit_identities.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1160 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/circuit_visulizations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      627 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/cswap_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/examples_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2295 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/gate_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1975 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/gops.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2215 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/state_prep_w16.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      875 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/state_prep_w4.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1389 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/swaptest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6196 2021-12-07 15:22:45.000000 quantumflow-1.2.1/examples/weyl.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-12-07 15:22:45.000000 quantumflow-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.193986 quantumflow-1.2.1/quantumflow/
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     9366 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (121)    11319 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/channels_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16313 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/circuits.py
--rw-r--r--   0 runner    (1001) docker     (121)    10498 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/circuits_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/config_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9213 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/dagcircuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/dagcircuit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23698 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/decompositions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8751 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/decompositions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/deprecated_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22486 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/gates.py
--rw-r--r--   0 runner    (1001) docker     (121)    19145 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/gates_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/gatesets.py
--rw-r--r--   0 runner    (1001) docker     (121)     9164 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/gradients.py
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/gradients_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12291 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6860 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/info_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23698 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16799 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/paulialgebra.py
--rw-r--r--   0 runner    (1001) docker     (121)     8494 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/paulialgebra_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/qubits.py
--rw-r--r--   0 runner    (1001) docker     (121)    16470 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/states.py
--rw-r--r--   0 runner    (1001) docker     (121)     7003 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/states_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.197986 quantumflow-1.2.1/quantumflow/stdgates/
--rw-r--r--   0 runner    (1001) docker     (121)     9432 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates.py
--rw-r--r--   0 runner    (1001) docker     (121)    26828 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_1q.py
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_1q_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    31071 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_2q.py
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_2q_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11580 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_3q.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_3q_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8014 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_cirq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_cirq_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6348 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_forest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_forest_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12320 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_qasm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_qasm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6366 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdgates/stdgates_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13443 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/stdops_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6082 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/tensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/tensors_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5510 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/transform_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.201986 quantumflow-1.2.1/quantumflow/translate/
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8489 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translate_gates.py
--rw-r--r--   0 runner    (1001) docker     (121)     7701 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translate_stdgates_1q.py
--rw-r--r--   0 runner    (1001) docker     (121)    25774 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translate_stdgates_2q.py
--rw-r--r--   0 runner    (1001) docker     (121)    16353 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translate_stdgates_3q.py
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translate_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/translate/translations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5104 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/transpile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/transpile_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10640 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/var.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/var_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23955 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)    18135 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/visualization_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xbraket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xbraket_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8356 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xcirq.py
--rw-r--r--   0 runner    (1001) docker     (121)     8322 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xcirq_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xforest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xforest_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6311 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqiskit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqiskit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqsim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqsim_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xquirk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xquirk_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6462 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqutip.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2021-12-07 15:22:45.000000 quantumflow-1.2.1/quantumflow/xqutip_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.197986 quantumflow-1.2.1/quantumflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-12-07 15:22:59.000000 quantumflow-1.2.1/quantumflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2021-12-07 15:23:00.000000 quantumflow-1.2.1/quantumflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:22:59.000000 quantumflow-1.2.1/quantumflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-12-07 15:22:59.000000 quantumflow-1.2.1/quantumflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-07 15:22:59.000000 quantumflow-1.2.1/quantumflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:22:59.000000 quantumflow-1.2.1/quantumflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-12-07 15:23:00.201986 quantumflow-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      112 2021-12-07 15:22:45.000000 quantumflow-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:23:00.201986 quantumflow-1.2.1/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2021-12-07 15:22:45.000000 quantumflow-1.2.1/tutorial/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    29410 2021-12-07 15:22:45.000000 quantumflow-1.2.1/tutorial/qf-tutorial-translate.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    17473 2021-12-07 15:22:45.000000 quantumflow-1.2.1/tutorial/qf-tutorial-transpile.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.710193 quantumflow-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.698193 quantumflow-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.698193 quantumflow-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-28 16:47:55.000000 quantumflow-1.3.0/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-28 16:47:55.000000 quantumflow-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-28 16:47:55.000000 quantumflow-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-28 16:47:55.000000 quantumflow-1.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 16:47:55.000000 quantumflow-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-28 16:47:55.000000 quantumflow-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-28 16:48:10.710193 quantumflow-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-28 16:47:55.000000 quantumflow-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.702193 quantumflow-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.702193 quantumflow-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/_static/qf.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.702193 quantumflow-1.3.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/bibtex.json
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/circuits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/decomp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/devnotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/gates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/gradients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/ops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/pauli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/qubits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/states.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/transform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/translate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/xcirq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/xforest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/xqiskit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/xquirk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-28 16:47:55.000000 quantumflow-1.3.0/docs/zreferences.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.702193 quantumflow-1.3.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/circuit_compilation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18925 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/circuit_identities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/circuit_visulizations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/cswap_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/examples_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2294 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/gate_translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/gops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/state_prep_w16.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/state_prep_w4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/swaptest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-05-28 16:47:55.000000 quantumflow-1.3.0/examples/weyl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-28 16:47:55.000000 quantumflow-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 16:47:55.000000 quantumflow-1.3.0/pyrightconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.706193 quantumflow-1.3.0/quantumflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/channels_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/circuits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/dagcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/dagcircuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23683 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/decompositions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/deprecated_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/future_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/gatesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/gradients_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23893 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/paulialgebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/paulialgebra_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/qubits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/states_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.710193 quantumflow-1.3.0/quantumflow/stdgates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_1q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_1q_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_2q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_2q_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_3q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_3q_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_cirq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_forest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_qasm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdgates/stdgates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/stdops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/tensors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/transform_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.710193 quantumflow-1.3.0/quantumflow/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translate_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translate_stdgates_1q.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translate_stdgates_2q.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translate_stdgates_3q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/translate/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/transpile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/transpile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/var_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/visualization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xbraket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xbraket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xcirq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xcirq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xforest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqiskit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqsim_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xquirk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xquirk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqutip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-28 16:47:55.000000 quantumflow-1.3.0/quantumflow/xqutip_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.710193 quantumflow-1.3.0/quantumflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:48:10.000000 quantumflow-1.3.0/quantumflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-28 16:48:10.710193 quantumflow-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-05-28 16:47:55.000000 quantumflow-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:48:10.710193 quantumflow-1.3.0/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-28 16:47:55.000000 quantumflow-1.3.0/tutorial/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29410 2023-05-28 16:47:55.000000 quantumflow-1.3.0/tutorial/qf-tutorial-translate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-05-28 16:47:55.000000 quantumflow-1.3.0/tutorial/qf-tutorial-transpile.ipynb
```

### Comparing `quantumflow-1.2.1/.github/workflows/python-build.yml` & `quantumflow-1.3.0/.github/workflows/python-build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,59 +13,62 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9']
+        python-version: ['3.9', '3.10', '3.11']
         os: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with: 
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install base
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
         python -m pip install pytest
     - name: Test with pytest (Tests should pass without extra dependancies installed)
       run: |
         python -m $(python -Wi setup.py --name).about
         python -m pytest
     - name: Install extra dependencies
+      if: runner.os == 'Linux'
       run: |
         python -m pip install --upgrade pip
         python -m pip install wheel
         python -m pip install .[dev]  # install package + test dependencies
     - name: Install extra Linux dependencies
       if: runner.os == 'Linux'
       run: |
+        sudo apt-get update
         sudo apt-get install texlive texlive-latex-extra latexmk poppler-utils
         mkdir -p ~/texmf/tex/latex
         wget http://mirrors.ctan.org/graphics/pgf/contrib/quantikz/tikzlibraryquantikz.code.tex -P ~/texmf/tex/latex
     - name: About
       if: runner.os == 'Linux'
       run: |
         python -m $(python -Wi setup.py --name).about
         echo
         pdflatex --version
         pdftocairo -v
     - name: Test coverage with pytest
       if: runner.os == 'Linux'
       run: |
-        python -m pytest --cov --cov-fail-under 100
+        python -m pytest --cov --cov-fail-under 95
     - name: Lint with black and isort (run `make delint` to fix issues)
       if: runner.os == 'Linux'
       run: |
+        python -m pip install black --upgrade  # Weirdly one of the optimal dependencies downgrades black 
         black --check .  
         isort --check -m 3 --tc .
     - name: Lint with flake8
       if: runner.os == 'Linux'
       run: |
         flake8 .            
     - name: Typecheck with mypy
@@ -73,17 +76,19 @@
       run: |
         mypy
     - name: Build documentation with sphinx
       if: runner.os == 'Linux'
       run: |
         sphinx-build -M html docs docs/_build
     - name: Test notebooks (against master)
+      if: runner.os == 'Linux'
       run: |
         pytest --nbmake tutorial
     - name: Test with all supported minor versions of cirq
+      if: runner.os == 'Linux'
       run: |
         python -m pip install cirq~=0.8.0
         python -m pytest quantumflow/xcirq_test.py    
         python -m pip install cirq~=0.9.0
         python -m pytest quantumflow/xcirq_test.py
         python -m pip install cirq~=0.10.0
         python -m pytest quantumflow/xcirq_test.py
```

### Comparing `quantumflow-1.2.1/.github/workflows/python-publish.yml` & `quantumflow-1.3.0/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `quantumflow-1.2.1/.gitignore` & `quantumflow-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/LICENSE` & `quantumflow-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/Makefile` & `quantumflow-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/PKG-INFO` & `quantumflow-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: quantumflow
-Version: 1.2.1
+Version: 1.3.0
 Summary: "Cross compiler for gate based models of quantum computing"
 Home-page: https://github.com/gecrooks/quantumflow/
 Author: Gavin Crooks
 Author-email: gavincrooks@gmail.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: ext
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 #  QuantumFlow: A Quantum Algorithms Development Toolkit
@@ -57,9 +56,7 @@
 ```
 $ git clone https://github.com/gecrooks/quantumflow.git
 $ cd quantumflow
 $ pip install -e .[dev]
 ```
 
 
-
-
```

### Comparing `quantumflow-1.2.1/README.md` & `quantumflow-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/Makefile` & `quantumflow-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/_static/qf.css` & `quantumflow-1.3.0/docs/_static/qf.css`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/conf.py` & `quantumflow-1.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 
 def do_edits():
-
     pats = [
         # Hacks to shorten type descriptors
         (r"quantumflow\.qubits", r"qf"),
         (r"quantumflow\.ops", r"qf"),
         (r"quantumflow\.stdops", r"qf"),
         (r"quantumflow\.gates\.gates_one", r"qf"),
         (r"quantumflow\.gates\.gates_two", r"qf"),
```

### Comparing `quantumflow-1.2.1/docs/devnotes.rst` & `quantumflow-1.3.0/docs/devnotes.rst`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/index.rst` & `quantumflow-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/intro.rst` & `quantumflow-1.3.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/docs/references.bib` & `quantumflow-1.3.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/circuit_compilation.py` & `quantumflow-1.3.0/examples/circuit_compilation.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/circuit_identities.py` & `quantumflow-1.3.0/examples/circuit_identities.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/circuit_visulizations.py` & `quantumflow-1.3.0/examples/circuit_visulizations.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/cswap_decomposition.py` & `quantumflow-1.3.0/examples/cswap_decomposition.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/examples_test.py` & `quantumflow-1.3.0/examples/examples_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/gate_translations.py` & `quantumflow-1.3.0/examples/gate_translations.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         circ1f = circ1.resolve(concrete)
         assert qf.gates_close(circ0f.asgate(), circ1f.asgate())
 
 
 def _print_circuit_identity(
     name, circ0, circ1, min_col_width=0, col_sep=5, left_margin=8
 ):
-
     print()
     print("", name)
     print()
 
     circ0 = qf.Circuit(circ0)
     circ1 = qf.Circuit(circ1)
```

### Comparing `quantumflow-1.2.1/examples/gops.py` & `quantumflow-1.3.0/examples/gops.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         qbs = random.sample(qubits, K)
         circ += gate.on(*qbs)
 
     return circ
 
 
 def _cli():
-
     gates = [
         qf.I(0),
         qf.X(0),
         qf.Y(0),
         qf.Z(0),
         qf.S(0),
         qf.T(0),
```

### Comparing `quantumflow-1.2.1/examples/state_prep_w16.py` & `quantumflow-1.3.0/examples/state_prep_w16.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/state_prep_w4.py` & `quantumflow-1.3.0/examples/state_prep_w4.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/swaptest.py` & `quantumflow-1.3.0/examples/swaptest.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/examples/weyl.py` & `quantumflow-1.3.0/examples/weyl.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
     ax.set_zticks([])
 
     pyplot.show()
 
 
 # ---------- Command Line Interface ----------
 def _cli():
-
     parser = argparse.ArgumentParser(
         description=__description__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
     parser.add_argument("--version", action="version", version=__version__)
     parser.add_argument(
```

### Comparing `quantumflow-1.2.1/quantumflow/__init__.py` & `quantumflow-1.3.0/quantumflow/__init__.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/channels.py` & `quantumflow-1.3.0/quantumflow/channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 .. autofunction:: random_channel
 """
 
 # Kudos: Kraus maps originally adapted from Nick Rubin's reference-qvm
 
 from functools import reduce
 from operator import add
-from typing import Sequence
+from typing import Optional, Sequence
 
 import numpy as np
 from scipy import linalg
 
 from . import tensors, utils
 from .ops import Channel, Gate, Operation, UnitaryGate
 from .qubits import Qubit, Qubits, sorted_qubits
@@ -81,15 +81,15 @@
 class Kraus(Operation):
     """A Kraus representation of a quantum channel"""
 
     # DOCME: operator-value-sum representation
     # FIXME: Shouldn't take Gate, since may not be Unitary operators
 
     def __init__(
-        self, operators: Sequence[Gate], weights: Sequence[float] = None
+        self, operators: Sequence[Gate], weights: Optional[Sequence[float]] = None
     ) -> None:
         self.operators = operators
 
         if weights is None:
             weights = [1.0] * len(operators)
 
         self.weights = tuple(weights)
@@ -101,15 +101,15 @@
         """
         raise TypeError("Not possible in general")
 
     def aschannel(self) -> Channel:
         """Returns: Action of Kraus operators as a superoperator Channel"""
         qubits = self.qubits
         N = len(qubits)
-        ident = UnitaryGate(np.eye(2 ** N), qubits).aschannel()
+        ident = UnitaryGate(np.eye(2**N), qubits).aschannel()
 
         tensors = [(op.aschannel() @ ident).tensor for op in self.operators]
         if self.weights is not None:
             tensors = [t * w for t, w in zip(tensors, self.weights)]
         chan_tensor = reduce(add, tensors)
 
         return Channel(chan_tensor, self.qubits)
@@ -160,17 +160,16 @@
     """A Kraus channel which is a convex mixture of unitary dynamics.
 
     This Channel is unital, but not all unital channels are unitary
     mixtures.
     """
 
     def __init__(
-        self, operators: Sequence[Gate], weights: Sequence[float] = None
+        self, operators: Sequence[Gate], weights: Optional[Sequence[float]] = None
     ) -> None:
-
         from .info import almost_unitary
 
         for op in operators:
             if not almost_unitary(op):
                 raise ValueError("Operators not all unitary")  # pragma: no cover
 
         if weights is not None and not np.isclose(np.sum(weights), 1.0):
@@ -254,59 +253,61 @@
     assert np.all(evals.real >= 0.0)  # FIXME exception
 
     values = np.sqrt(evals.real)
 
     ops = []
     for i in range(2 ** (2 * N)):
         if not np.isclose(values[i], 0.0):
-            mat = np.reshape(evecs[i], (2 ** N, 2 ** N)) * values[i]
+            mat = np.reshape(evecs[i], (2**N, 2**N)) * values[i]
             g = UnitaryGate(mat, qubits)
             ops.append(g)
 
     return Kraus(ops)
 
 
 def kraus_iscomplete(kraus: Kraus) -> bool:
     """Returns True if the collection of (weighted) Kraus operators are
     complete. (Which is necessary for a CPTP map to preserve trace)
     """
     qubits = kraus.qubits
     N = kraus.qubit_nb
 
-    ident = UnitaryGate(np.eye(2 ** N), qubits)
+    ident = UnitaryGate(np.eye(2**N), qubits)
 
     tensors = [(op.H @ op @ ident).asoperator() for op in kraus.operators]
     tensors = [t * w for t, w in zip(tensors, kraus.weights)]
 
     tensor = reduce(np.add, tensors)
     res = UnitaryGate(tensor, qubits)
 
     N = res.qubit_nb
-    return np.allclose(res.asoperator(), np.eye(2 ** N))
+    return np.allclose(res.asoperator(), np.eye(2**N))
 
 
 # TODO: as class RandomChannel?
 # Author: GEC (2019)
-def random_channel(qubits: Qubits, rank: int = None, unital: bool = False) -> Channel:
+def random_channel(
+    qubits: Qubits, rank: Optional[int] = None, unital: bool = False
+) -> Channel:
     """
     Returns: A randomly sampled Channel drawn from the BCSZ ensemble with
     the specified Kraus rank.
 
     Args:
         qubits: A list, or number, of qubits.
         rank: Kraus rank of channel. (Defaults to full rank)
 
     Ref:
         "Random quantum operations", Bruzda, Cappellini, Sommers, and
         Zyczkowski, Physics Letters A 373, 320 (2009). arXiv:0804.2361
     """
     qubits = tuple(qubits)
     N = len(qubits)
-    dim = 2 ** N  # Hilbert space dimension
-    size = (dim ** 2, dim ** 2) if rank is None else (dim ** 2, rank)
+    dim = 2**N  # Hilbert space dimension
+    size = (dim**2, dim**2) if rank is None else (dim**2, rank)
 
     # arXiv:0804.2361 page 4, steps 1 to 4
     # arXiv:0709.0824 page 6
     X = utils.complex_ginibre_ensemble(size)
     XX = X @ X.conj().T
 
     if unital:
```

### Comparing `quantumflow-1.2.1/quantumflow/channels_test.py` & `quantumflow-1.3.0/quantumflow/channels_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/circuits.py` & `quantumflow-1.3.0/quantumflow/circuits.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,18 @@
 
 class Circuit(Sequence, Operation):
     """A quantum Circuit contains a sequences of circuit elements.
     These can be any quantum Operation, including other circuits.
     """
 
     def __init__(
-        self, *elements: Union[Iterable[Operation], Operation], qubits: Qubits = None
+        self,
+        *elements: Union[Iterable[Operation], Operation],
+        qubits: Optional[Qubits] = None,
     ) -> None:
-
         elements = tuple(elements)
 
         if len(elements) == 1 and isinstance(elements[0], Iterable):
             # Legacy interface
             elements = tuple(elements[0])  # type: ignore
 
         qbs = [q for elem in elements for q in elem.qubits]  # type: ignore
@@ -165,29 +166,29 @@
         return self.rewire(labels)
 
     def rewire(self, labels: Dict[Qubit, Qubit]) -> "Circuit":
         return Circuit(
             [elem.rewire(labels) for elem in self], qubits=list(labels.values())
         )
 
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         """
         Apply the action of this circuit upon a state.
 
         If no initial state provided an initial zero state will be created.
         """
         if ket is None:
             qubits = self.qubits
             ket = zero_state(qubits=qubits)
 
         for elem in self:
             ket = elem.run(ket)
         return ket
 
-    def evolve(self, rho: Density = None) -> Density:
+    def evolve(self, rho: Optional[Density] = None) -> Density:
         if rho is None:
             qubits = self.qubits
             rho = zero_state(qubits=qubits).asdensity()
 
         for elem in self:
             rho = elem.evolve(rho)
         return rho
@@ -314,19 +315,19 @@
         q0 = controls[0]
         if isinstance(gate, X):
             circ += CNot(q0, gate.qubits[0])
         else:
             cgate = ControlGate(gate, [q0])
             circ += cgate
     else:
-        circ += control_circuit(controls[-1:], gate ** 0.5)
+        circ += control_circuit(controls[-1:], gate**0.5)
         circ += control_circuit(controls[0:-1], X(controls[-1]))
-        circ += control_circuit(controls[-1:], gate ** -0.5)
+        circ += control_circuit(controls[-1:], gate**-0.5)
         circ += control_circuit(controls[0:-1], X(controls[-1]))
-        circ += control_circuit(controls[0:-1], gate ** 0.5)
+        circ += control_circuit(controls[0:-1], gate**0.5)
     return circ
 
 
 def zyz_circuit(t0: Variable, t1: Variable, t2: Variable, q0: Qubit) -> Circuit:
     """A circuit of ZPow, XPow, ZPow gates on the same qubit"""
     return euler_circuit(t0, t1, t2, q0, "ZYZ")
```

### Comparing `quantumflow-1.2.1/quantumflow/circuits_test.py` & `quantumflow-1.3.0/quantumflow/circuits_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,36 +220,36 @@
 
 
 def test_phase_estimation_circuit_1() -> None:
     N = 8
     phase = 1 / 4
     gate = qf.Rz(-4 * np.pi * phase, N)
     circ = qf.phase_estimation_circuit(gate, range(N))
-    res = circ.run().measure()[0:N]
-    est_phase = bitlist_to_int(res) / 2 ** N
+    res = list(circ.run().measure()[0:N])
+    est_phase = bitlist_to_int(res) / 2**N
     assert np.isclose(phase, est_phase)
 
 
 def test_phase_estimation_circuit_2() -> None:
     N = 8
     phase = 12 / 256
     gate = qf.Rz(-4 * np.pi * phase, N)
     circ = qf.phase_estimation_circuit(gate, range(N))
-    res = circ.run().measure()[0:N]
-    est_phase = bitlist_to_int(res) / 2 ** N
+    res = list(circ.run().measure()[0:N])
+    est_phase = bitlist_to_int(res) / 2**N
     assert np.isclose(phase, est_phase)
 
 
 def test_phase_estimation_circuit_3() -> None:
     N = 8
     phase = 12 / 256
     gate = qf.ZZ(-4 * phase, N, N + 1)
     circ = qf.phase_estimation_circuit(gate, range(N))
-    res = circ.run().measure()[0:N]
-    est_phase = bitlist_to_int(res) / 2 ** N
+    res = list(circ.run().measure()[0:N])
+    est_phase = bitlist_to_int(res) / 2**N
     assert np.isclose(phase, est_phase)
 
     with pytest.raises(ValueError):
         # Gate and output qubits overlap
         _ = qf.phase_estimation_circuit(gate, range(N + 1))
 
 
@@ -268,16 +268,16 @@
 
                 state = np.zeros(shape=[2] * 6)
                 state[bits] = 1
                 ket = qf.State(state)
 
                 ket = circ.run(ket)
                 bits2 = ket.measure()
-                res = bits2[[5, 2, 3]]  # type: ignore
-                res = bitlist_to_int(res)
+                res0 = list(bits2[[5, 2, 3]])
+                res = bitlist_to_int(res0)
 
                 assert res == expected
 
     # Three bit addition circuit
     circ = qf.addition_circuit([0, 1, 2], [3, 4, 5], [6, 7])
     for c0 in range(0, 2):
         for a0 in range(0, 8):
@@ -291,15 +291,15 @@
                 state = np.zeros(shape=[2] * 8)
                 state[bits] = 1
                 ket = qf.State(state)
 
                 ket = circ.run(ket)
                 bits2 = ket.measure()
                 res = bits2[[7, 3, 4, 5]]  # type: ignore
-                res = bitlist_to_int(res)
+                res = bitlist_to_int(res)  # type: ignore
 
                 # print(c0, a0, a1, expected, res)
                 assert res == expected
 
     with pytest.raises(ValueError):
         qf.addition_circuit([0, 1, 2], [3, 4, 5, 6], [7, 8])
```

### Comparing `quantumflow-1.2.1/quantumflow/config.py` & `quantumflow-1.3.0/quantumflow/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 Package wide configuration
 """
 
 import platform
 import re
 import sys
 import typing
+from typing import Optional
 
-from .utils import importlib_metadata
+from .future import importlib_metadata
 
 __all__ = ["__version__", "about"]
 
 
 package_name = "quantumflow"
 
 try:
@@ -52,15 +53,15 @@
 NYCTRL = "⊗"  # ⊗ 'circled times'
 CTRL = "●"
 NCTRL = "○"
 CONJ = "⁺"  # Unicode "superscript plus sign"
 SQRT = "√"
 
 
-def about(file: typing.TextIO = None) -> None:
+def about(file: Optional[typing.TextIO] = None) -> None:
     """Print information about the configuration
 
      ``> python -m quantumflow.about``
 
     Args:
         file: Output stream (Defaults to stdout)
     """
```

### Comparing `quantumflow-1.2.1/quantumflow/config_test.py` & `quantumflow-1.3.0/quantumflow/config_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/dagcircuit.py` & `quantumflow-1.3.0/quantumflow/dagcircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 
 """
 QuantumFlow: Directed Acyclic Graph representations of a Circuit.
 """
 
 import itertools
 import textwrap
-from typing import Any, Dict, Generator, Iterable, Iterator, List, Tuple
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+)
 
 import networkx as nx
 import numpy as np
 import opt_einsum
 
 from . import utils
 from .circuits import Circuit
@@ -76,15 +85,14 @@
     DAGCircuit is iterable, yielding all of the operation nodes in
     topological sort order.
 
     Note: Provisional API
     """
 
     def __init__(self, elements: Iterable[Operation]) -> None:
-
         self.graph = nx.MultiDiGraph()
         self._qubits_in: Dict[Qubit, In] = {}
         self._qubits_out: Dict[Qubit, Out] = {}
 
         for elem in elements:
             self.append(elem)  # type: ignore
 
@@ -242,22 +250,22 @@
     def __iter__(self) -> Iterator[Operation]:
         for elem in nx.topological_sort(self.graph):
             # Filter in and out nodes
             if not isinstance(elem, In) and not isinstance(elem, Out):
                 yield elem
 
     # DOCME TESTME
-    def next_element(self, elem: Operation, qubit: Qubit = None) -> Operation:
+    def next_element(self, elem: Operation, qubit: Optional[Qubit] = None) -> Operation:
         for _, node, key in self.graph.edges(elem, keys=True):
             if qubit is None or key == qubit:
                 return node
         assert False  # Insanity check  # FIXME, raise exception
 
     # DOCME TESTME
-    def prev_element(self, elem: Operation, qubit: Qubit = None) -> Operation:
+    def prev_element(self, elem: Operation, qubit: Optional[Qubit] = None) -> Operation:
         for node, _, key in self.graph.in_edges(elem, keys=True):
             if qubit is None or key == qubit:
                 return node
         assert False  # Insanity check  # FIXME, raise exception
 
     def next_edges(self, elem: Operation) -> List[Tuple[Any, Any, Qubit]]:
         qubits = elem.qubits
```

### Comparing `quantumflow-1.2.1/quantumflow/dagcircuit_test.py` & `quantumflow-1.3.0/quantumflow/dagcircuit_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/decompositions.py` & `quantumflow-1.3.0/quantumflow/decompositions.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     U = gate.asoperator()
     U /= np.linalg.det(U) ** (1 / 2)
 
     nx = -U[0, 1].imag
     ny = -U[0, 1].real
     nz = -U[0, 0].imag
-    N = np.sqrt(nx ** 2 + ny ** 2 + nz ** 2)
+    N = np.sqrt(nx**2 + ny**2 + nz**2)
     if N == 0:  # Identity
         nx, ny, nz = 1, 1, 1
     else:
         nx /= N
         ny /= N
         nz /= N
     sin_halftheta = N
@@ -178,15 +178,15 @@
     results if the gate is not the direct product of two 1-qubit gates.
     """
 
     if gate.qubit_nb != 2:
         raise ValueError("Expected 2-qubit gate")
 
     U = gate.asoperator()
-    rank = 2 ** gate.qubit_nb
+    rank = 2**gate.qubit_nb
     U /= np.linalg.det(U) ** (1 / rank)
 
     R = U.reshape(2, 2, 2, 2)
     R = R.transpose(0, 2, 1, 3)
     R = R.reshape(4, 4)
 
     u, s, vh = np.linalg.svd(R)
@@ -257,15 +257,15 @@
         raise ValueError("Expected 2-qubit gate")
 
     q0, q1 = gate.qubits
 
     assert almost_unitary(gate)  # Sanity check
     U = gate.asoperator()
 
-    rank = 2 ** gate.qubit_nb
+    rank = 2**gate.qubit_nb
     U /= np.linalg.det(U) ** (1 / rank)  # U is in SU(4) so det U = 1
 
     U_mb = Q_H @ U @ Q  # Transform gate to Magic Basis [1, (eq. 17, 18)]
     M = U_mb.transpose() @ U_mb  # Construct M matrix [1, (eq. 22)]
 
     # Diagonalize symmetric complex matrix
     eigvals, eigvecs = _orthogonal_diagonalization(M)
@@ -411,15 +411,14 @@
 
     return coords
 
 
 def _constrain_to_weyl(
     lambdas: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-
     for permutation in itertools.permutations(range(4)):
         for signs in ([1, 1, 1, 1], [1, 1, -1, -1], [-1, 1, -1, 1], [1, -1, -1, 1]):
             signed_lambdas = lambdas * np.asarray(signs)
             perm = list(permutation)
             lambdas_perm = signed_lambdas[perm]
 
             coords = _lambdas_to_coords(lambdas_perm)
@@ -732,27 +731,27 @@
         # https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.cossin.html
         # Note that the cosine-sine thetas are half our thetas due to standard
         # quantum  convections.
         (A1, A2), halfthetas, (B1, B2) = scipy.linalg.cossin(U, p=R, q=R, separate=True)
 
         M2 = B1 @ B2.conj().T
         eigvals, V = np.linalg.eig(M2)
-        D = np.diag(eigvals ** 0.5)
+        D = np.diag(eigvals**0.5)
         W = D @ V.conj().T @ B2
         thetas = np.real(np.log(eigvals) * 1j)
 
         yield from qs_deke(Unitary(W, controls), euler)
         yield MultiplexedRzGate(thetas, controls=controls, target=target)
         yield from qs_deke(Unitary(V, controls), euler)
 
         yield MultiplexedRyGate(halfthetas * 2, controls=controls, target=target)
 
         M2 = A1 @ A2.conj().T
         eigvals, V = np.linalg.eig(M2)
-        D = np.diag(eigvals ** 0.5)
+        D = np.diag(eigvals**0.5)
         W = D @ V.conj().T @ A2
         thetas = np.real(np.log(eigvals) * 1j)
 
         yield from qs_deke(Unitary(W, controls), euler)
         yield MultiplexedRzGate(thetas, controls=controls, target=target)
         yield from qs_deke(Unitary(V, controls), euler)
```

### Comparing `quantumflow-1.2.1/quantumflow/decompositions_test.py` & `quantumflow-1.3.0/quantumflow/decompositions_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,14 @@
     gate1 = circ1.asgate()
     assert qf.gates_close(gate0, gate1)
 
 
 def test_orthogonal_diagonalization() -> None:
     samples = 100
     for _ in range(samples):
-
         # Build a random symmetric complex matrix
         orthoganal = scipy.stats.special_ortho_group.rvs(4)
         eigvals = (
             np.random.normal(size=(4,)) + 1j * np.random.normal(size=(4,))
         ) / np.sqrt(2.0)
         M = orthoganal @ np.diag(eigvals) @ orthoganal.T
```

### Comparing `quantumflow-1.2.1/quantumflow/deprecated.py` & `quantumflow-1.3.0/quantumflow/deprecated.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/deprecated_test.py` & `quantumflow-1.3.0/quantumflow/deprecated_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/gates.py` & `quantumflow-1.3.0/quantumflow/gates.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,26 +65,28 @@
 
 from typing import (
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
+    Optional,
     Sequence,
     Tuple,
     Union,
     cast,
 )
 
 import networkx as nx
 import numpy as np
 import scipy
 
 from . import tensors, utils, var
 from .circuits import Circuit
+from .future import cached_property
 from .ops import Channel, Gate, Operation, UnitaryGate
 from .paulialgebra import Pauli, sX, sY, sZ
 from .qubits import Qubit, Qubits
 from .states import Density, State
 from .stdgates import CNot, I, Ry, Rz, Swap, XPow, YPow, ZPow
 from .tensors import QubitTensor, asqutensor
 from .var import Variable
@@ -116,17 +118,17 @@
     cv_hermitian = True
     cv_tensor_structure = "identity"
 
     @property
     def hamiltonian(self) -> Pauli:
         return Pauli.zero()
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
-        return tensors.asqutensor(np.eye(2 ** self.qubit_nb))
+        return tensors.asqutensor(np.eye(2**self.qubit_nb))
 
     def __pow__(self, t: Variable) -> "IdentityGate":
         return self
 
     @property
     def H(self) -> "IdentityGate":
         return self
@@ -139,34 +141,34 @@
 
 
 class CompositeGate(Gate):
     """
     A quantum gate represented by a sequence of quantum gates.
     """
 
-    def __init__(self, *elements: Gate, qubits: Qubits = None) -> None:
+    def __init__(self, *elements: Gate, qubits: Optional[Qubits] = None) -> None:
         circ = Circuit(Circuit(elements).flat(), qubits=qubits)
 
         for elem in circ:
             if not isinstance(elem, Gate):
                 raise ValueError("A CompositeGate must be composed of Gates")
 
         super().__init__(qubits=circ.qubits)
         self.circuit = circ
 
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         return self.circuit.run(ket)
 
-    def evolve(self, rho: Density = None) -> Density:
+    def evolve(self, rho: Optional[Density] = None) -> Density:
         return self.circuit.evolve(rho)
 
     def aschannel(self) -> "Channel":
         return self.circuit.aschannel()
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return self.circuit.asgate().tensor
 
     @property
     def H(self) -> "CompositeGate":
         return CompositeGate(*self.circuit.H, qubits=self.qubits)
 
@@ -215,15 +217,17 @@
     The symbols are used in circuit diagrams. Z-basis control '●' and anti-control '○'
     symbols are standard, the rest are adapted from quirk.
     """
 
     # Note: ControlGate and StdCtrlGate share interface and code.
     # But unification probably not worth the trouble
 
-    def __init__(self, target: Gate, controls: Qubits, axes: str = None) -> None:
+    def __init__(
+        self, target: Gate, controls: Qubits, axes: Optional[str] = None
+    ) -> None:
         controls = tuple(controls)
         qubits = tuple(controls) + tuple(target.qubits)
         if len(set(qubits)) != len(qubits):
             raise ValueError("Control and gate qubits overlap")
 
         if axes is None:
             axes = "Z" * len(controls)
@@ -263,15 +267,15 @@
 
         ham = self.target.hamiltonian
         for q, axis in zip(self.control_qubits, self.axes):
             ham *= ctrlham[axis].on(q)
 
         return ham
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         # FIXME: This approach generates a tensor with unnecessary numerical noise.
         return UnitaryGate.from_hamiltonian(self.hamiltonian, self.qubits).tensor
 
     def resolve(self, subs: Mapping[str, float]) -> "ControlGate":
         target = self.target.resolve(subs)
         return ControlGate(target, self.control_qubits, self.axes)
@@ -367,24 +371,24 @@
             perm[qubits.index(q0)] = qubits.index(q1)
         perm.extend([idx + N for idx in perm])
 
         tensor = tensors.permute(rho.tensor, perm)
 
         return Density(tensor, qubits, rho.memory)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         N = self.qubit_nb
         qubits = self.qubits
 
         perm = list(range(2 * N))
         for q0, q1 in zip(qubits, self.qubits_out):
             perm[qubits.index(q0)] = qubits.index(q1)
 
-        U = np.eye(2 ** N)
+        U = np.eye(2**N)
         U = np.reshape(U, [2] * 2 * N)
         U = np.transpose(U, perm)
         return tensors.asqutensor(U)
 
 
 # end class MultiSwapGate
 
@@ -428,15 +432,15 @@
     def __init__(self, qubits: Qubits) -> None:
         super().__init__(qubits=qubits)
 
     @property
     def H(self) -> "InvQFTGate":
         return InvQFTGate(self.qubits)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return Circuit(self.decompose()).asgate().on(*self.qubits).tensor
 
 
 # end class QFTGate
 
 
@@ -446,15 +450,15 @@
     def __init__(self, qubits: Qubits) -> None:
         super().__init__(qubits=qubits)
 
     @property
     def H(self) -> "QFTGate":
         return QFTGate(self.qubits)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return Circuit(self.decompose()).asgate().on(*self.qubits).tensor
 
 
 # end class InvQFTGate
 
 
@@ -462,26 +466,25 @@
     """
     A Gate corresponding to the exponential of the Pauli algebra element,
     i.e. exp[-1.0j * alpha * element]
     """
 
     # Kudos: GEC (2019).
 
-    def __init__(self, element: Pauli, alpha: float) -> None:
-
+    def __init__(self, element: Pauli, alpha: Variable) -> None:
         super().__init__(qubits=element.qubits)
         self.element = element
         self.alpha = alpha
 
     def __str__(self) -> str:
         return f"PauliGate({self.element}, {self.alpha}) {self.qubits}"
 
     @property
     def H(self) -> "PauliGate":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "PauliGate":
         return PauliGate(self.element, self.alpha * t)
 
     @property
     def hamiltonian(self) -> "Pauli":
         return self.alpha * self.element
@@ -489,34 +492,35 @@
     def resolve(self, subs: Mapping[str, float]) -> "PauliGate":
         if var.is_symbolic(self.alpha):
             alpha = var.asfloat(self.alpha, subs)
             return PauliGate(self.element, alpha)
         return self
 
     def decompose(
-        self, topology: nx.Graph = None
+        self, topology: Optional[nx.Graph] = None
     ) -> Iterator[Union[CNot, XPow, YPow, ZPow]]:
         """
         Returns a Circuit corresponding to the exponential of
         the Pauli algebra element object, i.e. exp[-1.0j * alpha * element]
 
         If a qubit topology is provided then the returned circuit will
         respect the qubit connectivity, adding swaps as necessary.
         """
         from .translate import translate_PauliGate
 
         yield from translate_PauliGate(self, topology)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return Circuit(self.decompose()).asgate().on(*self.qubits).tensor
 
 
 # end class PauliGate
 
+
 # TODO: Move
 def merge_diagonal_gates(
     gate0: "DiagonalGate", gate1: "DiagonalGate"
 ) -> "DiagonalGate":
     qubits = Circuit([gate0, gate1]).qubits
     K = len(qubits)
 
@@ -570,15 +574,15 @@
     cv_tensor_structure = "diagonal"
 
     def __init__(
         self, diag_hamiltonian: Union[np.ndarray, Sequence[Variable]], qubits: Qubits
     ) -> None:
         super().__init__(qubits=qubits, params=tuple(diag_hamiltonian))
 
-        assert len(self.params) == 2 ** self.qubit_nb  # FIXME
+        assert len(self.params) == 2**self.qubit_nb  # FIXME
 
     # DOCME TESTME
     @classmethod
     def from_gate(cls, gate: Gate) -> "DiagonalGate":
         if isinstance(gate, DiagonalGate):
             return gate
 
@@ -604,25 +608,25 @@
         qubits = tuple(qubits)
         if self.qubits == qubits:
             return self
         params = np.resize(np.asarray(self.params), [2] * self.qubit_nb)
         params = tensors.permute(params, self.qubit_indices(qubits))
         return DiagonalGate(tuple(params.flatten()), qubits)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return asqutensor(np.diag(self.tensor_diagonal.flatten()))
 
-    @utils.cached_property
+    @cached_property
     def tensor_diagonal(self) -> QubitTensor:
         return asqutensor(np.exp(-1.0j * np.asarray(self.params)))
 
     @property
     def H(self) -> "DiagonalGate":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "DiagonalGate":
         params = [p * e for p in self.params]
         return DiagonalGate(params, self.qubits)
 
 
 # end class DiagonalGate
@@ -653,25 +657,25 @@
             raise ValueError("Wrong number of target gates.")
 
         super().__init__(qubits)
         self.controls = controls
         self.targets = targets
         self.gates = gates
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         blocks = [gate.asoperator() for gate in self.gates]
         return asqutensor(scipy.linalg.block_diag(*blocks))
 
     @property
     def H(self) -> "MultiplexedGate":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "MultiplexedGate":
-        gates = [gate ** e for gate in self.gates]
+        gates = [gate**e for gate in self.gates]
         return MultiplexedGate(gates, self.controls)
 
     # TODO: deke to 2^N control gates
 
     # Testme
     def resolve(self, subs: Mapping[str, float]) -> "MultiplexedGate":
         gates = cast(Sequence[Gate], [gate.resolve(subs) for gate in self.gates])
@@ -700,36 +704,35 @@
     """Uniformly controlled (multiplexed) Rz gate"""
 
     cv_tensor_structure = "diagonal"
 
     def __init__(
         self, thetas: Sequence[Variable], controls: Qubits, target: Qubit
     ) -> None:
-
         thetas = tuple(thetas)
         gates = [Rz(theta, target) for theta in thetas]
         super().__init__(gates=gates, controls=controls)
         self._params = thetas  # FIXME: This seems broken?
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return asqutensor(np.diag(self.tensor_diagonal.flatten()))
 
-    @utils.cached_property
+    @cached_property
     def tensor_diagonal(self) -> QubitTensor:
-        diagonal = []
+        diagonal: List[float] = []
         for theta in self.params:
             rz = Rz(theta, 0)
             diagonal.extend(np.diag(rz.tensor))
 
         return asqutensor(diagonal)
 
     @property
     def H(self) -> "MultiplexedRzGate":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "MultiplexedRzGate":
         thetas = [e * p for p in self.params]
         return MultiplexedRzGate(thetas, self.controls, self.targets[0])
 
 
 # end class MultiplexedRzGate
@@ -737,23 +740,22 @@
 
 class MultiplexedRyGate(MultiplexedGate):
     """Uniformly controlled (multiplexed) Ry gate"""
 
     def __init__(
         self, thetas: Sequence[Variable], controls: Qubits, target: Qubit
     ) -> None:
-
         thetas = tuple(thetas)
         gates = [Ry(theta, target) for theta in thetas]
         super().__init__(gates=gates, controls=controls)
         self._params = thetas  # FIXME: This seems broken?
 
     @property
     def H(self) -> "MultiplexedRyGate":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "MultiplexedRyGate":
         thetas = [e * p for p in self.params]
         return MultiplexedRyGate(thetas, self.controls, self.targets[0])
 
 
 # end class MultiplexedRyGate
```

### Comparing `quantumflow-1.2.1/quantumflow/gates_test.py` & `quantumflow-1.3.0/quantumflow/gates_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     assert len(circ) == 6
 
     for n in range(1, 6):
         assert qf.IdentityGate(list(range(n))).qubit_nb == n
 
     assert gate.hamiltonian.is_zero()
 
-    assert gate ** 2 is gate
+    assert gate**2 is gate
 
 
 def test_qftgate() -> None:
     circ = qf.Circuit()
     circ += qf.X(2)
     circ += qf.QFTGate([0, 1, 2])
 
@@ -160,15 +160,14 @@
     gate = qf.PauliGate(qf.sI(0), alpha)
     assert gate.element.is_identity()
     circ = qf.Circuit(gate.decompose())
     assert len(circ) == 0
 
 
 def test_PauliGate_more() -> None:
-
     alphas = [0.1, 2.0, -3.14, -0.4]
     paulis = [
         qf.sZ(0) + 1,
         qf.sY(0),
         qf.sX(0),
         0.5 * np.pi * qf.sZ(0) * qf.sZ(1),
         0.5 * np.pi * qf.sX(0) * qf.sZ(1),
@@ -198,50 +197,49 @@
     g = qf.PauliGate(qf.sZ(0), 0.3)
     assert g.resolve(subs={"alpha": 0.3}) is g
 
 
 def test_PauliGate_pow() -> None:
     alpha = 0.4
     gate0 = qf.PauliGate(qf.sZ(0), alpha)
-    gate1 = gate0 ** 0.3
+    gate1 = gate0**0.3
     gate2 = qf.Unitary(gate0.tensor, gate0.qubits) ** 0.3
     assert qf.gates_close(gate1, gate2)
-    assert qf.gates_close(gate1.H, gate2 ** -1)
+    assert qf.gates_close(gate1.H, gate2**-1)
 
     gate3 = qf.UnitaryGate.from_hamiltonian(gate0.hamiltonian, qubits=gate0.qubits)
     assert qf.gates_close(gate0, gate3)
 
     s = str(gate0)
     print(s)
 
 
 def test_DiagonalGate() -> None:
-
     gate0 = qf.DiagonalGate([0.1, -0.1], qubits=[1])
     gate1 = qf.Rz(0.2, 1)
     assert qf.gates_close(gate0, gate0)
     assert qf.gates_close(gate0, gate1)
-    assert qf.gates_close(gate0.H, gate0 ** -1)
+    assert qf.gates_close(gate0.H, gate0**-1)
 
     gate2 = qf.DiagonalGate([0.1, -0.1], qubits=[1])
     gate3 = qf.ZPow(0.2 / np.pi, 1)
     assert qf.gates_close(gate2, gate3)
 
     gate4 = qf.DiagonalGate([0, 0, 0, -np.pi], qubits=[0, 1])
     gate5 = qf.CZ(0, 1)
     assert qf.gates_close(gate4, gate5)
-    assert qf.gates_close(gate4 ** 0.1, gate5 ** 0.1)
+    assert qf.gates_close(gate4**0.1, gate5**0.1)
 
     circ0 = qf.Circuit(gate0.decompose())
     assert qf.gates_close(gate0, circ0.asgate())
 
     circ4 = qf.Circuit(gate4.decompose())
     assert qf.gates_close(gate4, circ4.asgate())
 
-    gate6 = gate4 ** 0.2
+    gate6 = gate4**0.2
     circ6 = qf.Circuit(gate6.decompose())
     assert qf.gates_close(gate6, circ6.asgate())
 
     gate7 = qf.DiagonalGate([0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8], qubits=[0, 1, 2])
     circ7 = qf.Circuit(gate7.decompose())
     assert qf.gates_close(gate7, circ7.asgate())
 
@@ -316,18 +314,17 @@
         [Symbol("b0"), Symbol("b1"), Symbol("b2"), Symbol("b3")], qubits=[1, 2]
     )
 
     _ = merge_diagonal_gates(gate0, gate1)
 
 
 def test_DiagonalGate_decomposition_count() -> None:
-
     for N in range(1, 9):
         qbs = list(range(0, N))
-        params = np.random.rand(2 ** N)
+        params = np.random.rand(2**N)
         gate = qf.DiagonalGate(params, qbs)
         circ = qf.Circuit(gate.decompose())
         ops = qf.count_operations(circ)
         print(N, ops)
         # print(qf.circuit_to_diagram(circ))
 
         # From Shende2006a
@@ -388,15 +385,15 @@
 
     gate7 = qf.MultiplexedRzGate(
         thetas=tuple(np.random.rand(16)), controls=[0, 1, 2, 3], target=4
     )
     circ7 = qf.Circuit(gate7.decompose())
     assert qf.gates_close(circ7.asgate(), gate7)
 
-    assert qf.gates_close(gate1.H, gate1 ** -1)
+    assert qf.gates_close(gate1.H, gate1**-1)
 
     assert str(gate1) == "MultiplexedRzGate(1/10) 2"
 
 
 def test_MultiplexedRzGate_str() -> None:
     gate1 = qf.MultiplexedRzGate(thetas=[0.1324], controls=(), target=2)
     s = str(gate1)
@@ -422,19 +419,19 @@
 
     gate7 = qf.MultiplexedRyGate(
         thetas=tuple(np.random.rand(2)), controls=[0], target=4
     )
     circ7 = qf.Circuit(gate7.decompose())
     assert qf.gates_close(circ7.asgate(), gate7)
 
-    assert qf.gates_close(gate1.H, gate1 ** -1)
+    assert qf.gates_close(gate1.H, gate1**-1)
     gate2 = qf.Unitary(gate1.asoperator(), gate1.qubits)
     assert qf.gates_close(gate1.H, gate2.H)
-    assert qf.gates_close(gate1 ** 2, gate2 ** 2)
-    assert qf.gates_close(gate1 ** -1, gate2 ** -1)
+    assert qf.gates_close(gate1**2, gate2**2)
+    assert qf.gates_close(gate1**-1, gate2**-1)
 
 
 def test_MultiplexedGate() -> None:
     gate1 = qf.MultiplexedGate(
         [qf.Rz(0.1, 2), qf.Rz(0.2, 2), qf.Rz(0.3, 2), qf.Rz(0.4, 2)], [0, 1]
     )
     gate2 = qf.MultiplexedRzGate([0.1, 0.2, 0.3, 0.4], [0, 1], 2)
@@ -523,21 +520,20 @@
     gate13 = qf.ControlGate(qf.Swap(1, 2), [0], axes="z")
     assert str(gate13) == "ControlGate(Swap 1 2, 'z') 0"
 
 
 def test_ControlGate_resolve() -> None:
     theta = Symbol("theta")
     gate0 = qf.ControlGate(qf.Rx(theta, 1), [0])
-    gate1 = gate0.resolve({theta: 2.3})
+    gate1 = gate0.resolve({theta: 2.3})  # type: ignore  # FIXME
     gate2 = qf.ControlGate(qf.Rx(2.3, 1), [0])
     assert qf.gates_close(gate1, gate2)
 
 
 def test_ControlGate_axes() -> None:
-
     gate0 = qf.ControlGate(qf.Z(1), [0], axes="z")
     gate1 = qf.Circuit([qf.X(0), qf.CZ(0, 1), qf.X(0)]).asgate()
     assert qf.gates_close(gate0, gate1)
 
     gate0 = qf.ControlGate(qf.X(2), [0, 1], axes="ZZ")
     gate1 = qf.CCNot(0, 1, 2)
     assert qf.gates_close(gate0, gate1)
```

### Comparing `quantumflow-1.2.1/quantumflow/gatesets.py` & `quantumflow-1.3.0/quantumflow/gatesets.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/gradients.py` & `quantumflow-1.3.0/quantumflow/gradients.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 .. autofunction::   expectation_gradients
 .. autofunction::   state_fidelity_gradients
 .. autofunction::   state_angle_gradients
 .. autofunction::   parameter_shift_circuits
 
 """
 
-from typing import Callable, Sequence, Tuple
+from typing import Callable, Optional, Sequence, Tuple
 
 import numpy as np
 from numpy import pi
 
 from . import tensors
 from .circuits import Circuit
 from .deprecated import join_gates
@@ -81,15 +81,15 @@
 }
 
 
 def expectation_gradients(
     ket0: State,
     circ: Circuit,
     hermitian: Operation,
-    dfunc: Callable[[float], float] = None,
+    dfunc: Optional[Callable[[float], float]] = None,
 ) -> Sequence[float]:
     """
     Calculate the gradients of a function of expectation for a
     parameterized quantum circuit, using the middle-out algorithm.
 
     Args:
         ket0: An initial state.
@@ -125,15 +125,15 @@
 
         f0 = gen.run(forward)
         g = -2 * r * np.imag(tensors.inner(f0.tensor, back.tensor))
 
         if dfunc is not None:
             g = g * dfunc(float(expectation))
 
-        grads.append(g)
+        grads.append(float(g))
 
     return grads
 
 
 def state_fidelity_gradients(
     ket0: State, ket1: State, circ: Circuit
 ) -> Sequence[float]:
```

### Comparing `quantumflow-1.2.1/quantumflow/gradients_test.py` & `quantumflow-1.3.0/quantumflow/gradients_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/info.py` & `quantumflow-1.3.0/quantumflow/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
 .. autofunction:: channel_angle
 .. autofunction:: channels_close
 .. autofunction:: average_gate_fidelity
 .. autofunction:: almost_unital
 """
 
+from typing import Optional
+
 import numpy as np
 import scipy.stats
 from scipy.linalg import sqrtm  # matrix square root
 
 from . import tensors
 from .channels import Kraus
 from .circuits import Circuit
@@ -195,15 +197,15 @@
     competently mixed state.
 
     Two closely related.info are the linear entropy, 1- purity, and the
     participation ratio, 1/purity.
     """
     tensor = rho.tensor
     N = rho.qubit_nb
-    matrix = np.reshape(tensor, [2 ** N, 2 ** N])
+    matrix = np.reshape(tensor, [2**N, 2**N])
     return float(np.trace(matrix @ matrix))
 
 
 def fidelity(rho0: Density, rho1: Density) -> float:
     """Return the fidelity F(rho0, rho1) between two mixed quantum states."""
     rho1 = rho1.permute(rho0.qubits)
     op0 = rho0.asoperator()
@@ -241,15 +243,15 @@
 
     Closeness is measured with the Fubini-Study fidelity.
     """
     rho1 = rho1.permute(rho0.qubits)
     return fubini_study_close(rho0.tensor, rho1.tensor, atol)
 
 
-def entropy(rho: Density, base: float = None) -> float:
+def entropy(rho: Density, base: Optional[float] = None) -> float:
     """
     Returns the von-Neumann entropy of a mixed quantum state.
 
     Args:
         rho:    A density matrix
         base:   Optional logarithm base. Default is base e, and entropy is
                .info in nats. For bits set base to 2.
@@ -261,15 +263,18 @@
     probs = np.linalg.eigvalsh(op)
     probs = np.maximum(probs, 0.0)  # Compensate for floating point errors
     return scipy.stats.entropy(probs, base=base)
 
 
 # TESTME
 def mutual_info(
-    rho: Density, qubits0: Qubits, qubits1: Qubits = None, base: float = None
+    rho: Density,
+    qubits0: Qubits,
+    qubits1: Optional[Qubits] = None,
+    base: Optional[float] = None,
 ) -> float:
     """Compute the bipartite von-Neumann mutual information of a mixed
     quantum state.
 
     Args:
         rho:    A density matrix of the complete system
         qubits0: Qubits of system 0
@@ -296,15 +301,15 @@
 def trace_distance(rho0: Density, rho1: Density) -> float:
     """
     Compute the trace distance between two mixed states
     :math:`T(rho_0,rho_1) = (1/2)||rho_0-rho_1||_1`
     """
     op0 = rho0.asoperator()
     op1 = rho1.asoperator()
-    return 0.5 * np.linalg.norm(op0 - op1, 1)
+    return float(0.5 * np.linalg.norm(op0 - op1, 1))
 
 
 # Measures on gates
 
 
 def gate_angle(gate0: Gate, gate1: Gate) -> float:
     """The Fubini-Study angle between gates"""
@@ -327,15 +332,15 @@
     """Returns: True if gates are almost identical and
     have almost the same phase.
     """
     gate1 = gate1.permute(gate0.qubits)
     if not gates_close(gate0, gate1):
         return False
     N = gate0.qubit_nb
-    phase = np.trace((gate1 @ gate0.H).asoperator()) / 2 ** N
+    phase = np.trace((gate1 @ gate0.H).asoperator()) / 2**N
     return bool(np.isclose(phase, 1.0, atol=atol))
 
 
 # TESTME
 def gates_commute(gate0: Gate, gate1: Gate, atol: float = ATOL) -> bool:
     """Returns: True if gates (almost) commute."""
     gate01 = Circuit([gate0, gate1]).asgate()
@@ -356,14 +361,15 @@
 def almost_hermitian(gate: Gate) -> bool:
     """Return true if gate tensor is (almost) Hermitian"""
     return gates_close(gate, gate.H)
 
 
 # Measures on circuits
 
+
 # DOCME
 def circuits_close(
     circ0: Circuit, circ1: Circuit, atol: float = ATOL, reps: int = 16
 ) -> bool:
     """Returns: True if circuits are (probably) almost identical.
 
     We check closeness by running multiple random initial states
@@ -395,44 +401,44 @@
     Closeness is measured with the channel angle.
     """
     chan1 = chan1.permute(chan0.qubits)
     return fubini_study_close(chan0.tensor, chan1.tensor, atol)
 
 
 # TESTME  multiqubits
-def average_gate_fidelity(kraus: Kraus, target: Gate = None) -> float:
+def average_gate_fidelity(kraus: Kraus, target: Optional[Gate] = None) -> float:
     """Return the average gate fidelity between a noisy gate (specified by a
     Kraus representation of a superoperator), and a purely unitary target gate.
 
     If the target gate is not specified, default to identity gate.
     """
 
     if target is None:
         target = IdentityGate(kraus.qubits)
     else:
         if kraus.qubits != target.qubits:
             raise ValueError("Qubits must be same")  # pragma: no cover  # TESTME
 
     N = kraus.qubit_nb
-    d = 2 ** N
+    d = 2**N
 
     U = target.H.asoperator()
 
     summand = 0
     for w, K in zip(kraus.weights, kraus.operators):
         summand += np.absolute(np.trace(w * U @ K.asoperator())) ** 2
 
-    return (d + summand) / (d + d ** 2)
+    return (d + summand) / (d + d**2)
 
 
 # Author: GEC (2019)
 def almost_unital(chan: Channel) -> bool:
     """Return true if the channel is (almost) unital."""
     # Unital channels leave the identity unchanged.
-    dim = 2 ** chan.qubit_nb
+    dim = 2**chan.qubit_nb
     eye0 = np.eye(dim, dim)
     rho0 = Density(eye0, chan.qubits)
     rho1 = chan.evolve(rho0)
     eye1 = rho1.asoperator()
     return np.allclose(eye0, eye1)
```

### Comparing `quantumflow-1.2.1/quantumflow/info_test.py` & `quantumflow-1.3.0/quantumflow/info_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import quantumflow as qf
 from quantumflow.config import ATOL
 
 from .config_test import REPS
 
 
 def test_fubini_study_angle() -> None:
-
     for _ in range(REPS):
         theta = random.uniform(-np.pi, +np.pi)
 
         ang = qf.fubini_study_angle(qf.I(0).tensor, qf.Rx(theta, 0).su().tensor)
         assert np.isclose(2 * ang / abs(theta), 1.0)
 
         ang = qf.fubini_study_angle(qf.I(0).tensor, qf.Ry(theta, 0).tensor)
```

### Comparing `quantumflow-1.2.1/quantumflow/ops.py` & `quantumflow-1.3.0/quantumflow/ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,67 +43,64 @@
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
+    Union,
 )
 
 import numpy as np
 import scipy
 from scipy.linalg import fractional_matrix_power as matpow
 from scipy.linalg import logm
 
-from . import tensors, utils, var
+from . import tensors, var
+from .future import cached_property
 from .qubits import Qubit, Qubits
 from .states import Density, State
 from .tensors import QubitTensor
 from .var import Variable
 
 # standard workaround to avoid circular imports from type hints
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike  # pragma: no cover
 
     from .paulialgebra import Pauli  # pragma: no cover
     from .stdgates import StdGate  # noqa:F401  # pragma: no cover
 
-
 __all__ = [
     "Operation",
     "Gate",
     "UnitaryGate",
     "Channel",
     "Unitary",
     "OPERATIONS",
     "GATES",
 ]
 
 
-OperationType = TypeVar("OperationType", bound="Operation")
-"""Generic type annotations for subtypes of Operation"""
-
-GateType = TypeVar("GateType", bound="Gate")
-"""Generic type annotations for subtypes of Gate"""
-
-
 _EXCLUDED_OPERATIONS = set(
     ["Operation", "Gate", "StdGate", "StdCtrlGate", "In", "Out", "NoWire"]
 )
 # Names of operations to exclude from registration. Includes (effectively) abstract base
 # classes and internal operations.
 
 
 OPERATIONS: Dict[str, Type["Operation"]] = {}
 """All quantum operations (All non-abstract subclasses of Operation)"""
 
 GATES: Dict[str, Type["Gate"]] = {}
 """All gates (All non-abstract subclasses of Gate)"""
 
 
+OperationTV = TypeVar("OperationTV", bound="Operation")
+
+
 @total_ordering
 class Operation(ABC):
     """An operation on a quantum state. An element of a quantum circuit.
 
     Abstract Base Class for Gate, Circuit, and other quantum operations.
 
     Attributes:
@@ -116,41 +113,41 @@
 
     __slots__ = ["_tensor", "_qubits", "_params"]
 
     cv_interchangeable: ClassVar[bool] = False
     """Is this a multi-qubit operation that is known to be invariant under
     permutations of qubits?"""
 
-    cv_qubit_nb: ClassVar[int] = None
+    cv_qubit_nb: ClassVar[int] = 0
     """The number of qubits, for operations with a fixed number of qubits"""
 
-    cv_args: ClassVar[Optional[Tuple[str, ...]]] = None
-    """The names of the parameters for this operation (For operations with a fixed number
-    of float parameters)"""
+    cv_args: ClassVar[Union[Tuple[str, ...], Tuple]] = ()
+    """The names of the parameters for this operation (For operations with a fixed
+    number of float parameters)"""
 
     def __init_subclass__(cls) -> None:
         # Note: The __init_subclass__ initializes all subclasses of a given class.
         # see https://www.python.org/dev/peps/pep-0487/
 
         name = cls.__name__
         if name not in _EXCLUDED_OPERATIONS:
             OPERATIONS[name] = cls
 
     def __init__(
         self,
         qubits: Qubits,
-        params: Sequence[Variable] = None,
+        params: Optional[Sequence[Variable]] = None,
     ) -> None:
         self._qubits: Qubits = tuple(qubits)
         self._params: Tuple[Variable, ...] = ()
         if params is not None:
             self._params = tuple(params)
-        self._tensor: QubitTensor = None
+        self._tensor: Optional[QubitTensor] = None
 
-        if self.cv_qubit_nb is not None:
+        if self.cv_qubit_nb != 0:
             if self.cv_qubit_nb != len(self._qubits):
                 raise ValueError(
                     "Wrong number of qubits for Operation"
                 )  # pragma: no cover
 
     def __iter__(self) -> Iterator["Operation"]:
         yield self
@@ -166,23 +163,23 @@
         return self._qubits
 
     @property
     def qubit_nb(self) -> int:
         """Return the total number of qubits"""
         return len(self.qubits)
 
-    def on(self: OperationType, *qubits: Qubit) -> OperationType:
+    def on(self: OperationTV, *qubits: Qubit) -> OperationTV:
         """Return a copy of this Operation with new qubits"""
         if len(qubits) != self.qubit_nb:
             raise ValueError("Wrong number of qubits")
         op = copy(self)
         op._qubits = qubits
         return op
 
-    def rewire(self: OperationType, labels: Dict[Qubit, Qubit]) -> OperationType:
+    def rewire(self: OperationTV, labels: Dict[Qubit, Qubit]) -> OperationTV:
         """Relabel qubits and return copy of this Operation"""
         qubits = tuple(labels[q] for q in self.qubits)
         return self.on(*qubits)
 
     def qubit_indices(self, qubits: Qubits) -> Tuple[int, ...]:
         """Convert qubits to index positions.
 
@@ -201,35 +198,39 @@
 
     def param(self, name: str) -> Variable:
         """Return a a named parameters of this Operation.
 
         Raise:
             KeyError: If unrecognized parameter name
         """
+        if self.cv_args is None:
+            raise KeyError("No parameters")
         try:
             idx = self.cv_args.index(name)
         except ValueError:
             raise KeyError("Unknown parameter name", name)
 
         return self._params[idx]
 
     # rename? param_asfloat? Then use where needed.
-    def float_param(self, name: str, subs: Mapping[str, float] = None) -> float:
+    def float_param(
+        self, name: str, subs: Optional[Mapping[str, float]] = None
+    ) -> float:
         """Return a a named parameters of this Operation as a float.
 
         Args:
             name: The name of the parameter (should be in cls.cv_args)
             subs: Symbolic substitutions to resolve symbolic Variables
         Raise:
             KeyError:  If unrecognized parameter name
             ValueError: If Variable cannot be converted to float
         """
         return var.asfloat(self.param(name), subs)
 
-    def resolve(self: OperationType, subs: Mapping[str, float]) -> OperationType:
+    def resolve(self: OperationTV, subs: Mapping[str, float]) -> OperationTV:
         """Resolve symbolic parameters"""
         # params = {k: var.asfloat(v, subs) for k, v in self.params.items()}
         op = copy(self)
         _params = [var.asfloat(v, subs) for v in self.params]
         op._params = tuple(_params)
         op._tensor = None
         return op
@@ -340,14 +341,17 @@
 
         return labels
 
 
 # End class Operation
 
 
+GateTV = TypeVar("GateTV", bound="Gate")
+
+
 class Gate(Operation):
     """
     A quantum logic gate. A unitary operator that acts upon a collection
     of qubits.
     """
 
     cv_hermitian: ClassVar[bool] = False
@@ -403,25 +407,25 @@
         # See test_gate_hamiltonians()
         from .paulialgebra import pauli_decompose_hermitian
 
         H = -logm(self.asoperator()) / 1.0j
         pauli = pauli_decompose_hermitian(H, self.qubits)
         return pauli
 
-    def asgate(self: GateType) -> GateType:
+    def asgate(self: GateTV) -> GateTV:
         return self
 
     def aschannel(self) -> "Channel":
         """Convert a Gate into a Channel"""
         N = self.qubit_nb
         R = 4
 
         # TODO: As Kraus?
         tensor = np.outer(self.tensor, self.H.tensor)
-        tensor = np.reshape(tensor, [2 ** N] * R)
+        tensor = np.reshape(tensor, [2**N] * R)
         tensor = np.transpose(tensor, [0, 3, 1, 2])
 
         return Channel(tensor, self.qubits)
 
     def __pow__(self, t: float) -> "Gate":
         """Return this gate raised to the given power."""
         matrix = matpow(self.asoperator(), t)
@@ -442,25 +446,25 @@
         return tensors.flatten(self.tensor, rank=2)
 
     @property
     @abstractmethod
     def tensor(self) -> QubitTensor:
         pass
 
-    @utils.cached_property
+    @cached_property
     def tensor_diagonal(self) -> QubitTensor:
         """
         Returns the diagonal of the tensor representation of this operation
         (if possible)
         """
         return tensors.asqutensor(np.diag(self.asoperator()))
 
     def su(self) -> "UnitaryGate":
         """Convert gate tensor to the special unitary group."""
-        rank = 2 ** self.qubit_nb
+        rank = 2**self.qubit_nb
         U = self.asoperator()
         U /= np.linalg.det(U) ** (1 / rank)
         return UnitaryGate(U, self.qubits)
 
     @property
     def H(self) -> "Gate":
         return UnitaryGate(self.asoperator().conj().T, self.qubits)
@@ -579,17 +583,19 @@
     @classmethod
     def from_hamiltonian(cls, hamiltonian: "Pauli", qubits: Qubits) -> "UnitaryGate":
         """Create a Unitary gate U from a Pauli operator H, U = exp(-i H)"""
         op = hamiltonian.asoperator(qubits)
         U = scipy.linalg.expm(-1j * op)
         return cls(U, qubits)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         """Returns the tensor representation of gate operator"""
+        if self._tensor is None:
+            raise ValueError("No tensor representation")
         return self._tensor
 
 
 # End class UnitaryGate
 
 # Deprecated. Renamed to UnitaryGate
 Unitary = UnitaryGate
@@ -599,31 +605,32 @@
 class Channel(Operation):
     """A quantum channel"""
 
     def __init__(
         self,
         tensor: "ArrayLike",
         qubits: Qubits,
-        params: Sequence[var.Variable] = None,
-        name: str = None,  # FIXME
+        params: Optional[Sequence[var.Variable]] = None,
+        name: Optional[str] = None,  # FIXME
     ) -> None:
-
         tensor = tensors.asqutensor(tensor)
 
         N = np.ndim(tensor) // 4
         if len(qubits) != N:
             raise ValueError("Wrong number of qubits for tensor")
 
         super().__init__(qubits=qubits, params=params)
         self._tensor = tensor
         self._name = type(self).__name__ if name is None else name
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         """Return the tensor representation of the channel's superoperator"""
+        if self._tensor is None:
+            raise ValueError("No tensor representation")
         return self._tensor
 
     @property
     def name(self) -> str:
         return self._name
 
     def permute(self, qubits: Qubits) -> "Channel":
@@ -655,15 +662,15 @@
         the Choi matrix representation. (See channel.choi())
         """
 
         N = self.qubit_nb
 
         # TODO: Use tensor_transpose, or remove tensor_transpose
         tensor = self.tensor
-        tensor = np.reshape(tensor, [2 ** N] * 4)
+        tensor = np.reshape(tensor, [2**N] * 4)
         tensor = np.transpose(tensor, (0, 2, 1, 3))
         tensor = np.reshape(tensor, [2] * 4 * N)
         return Channel(tensor, self.qubits)
 
     def choi(self) -> QubitTensor:
         """Return the Choi matrix representation of this super
         operator"""
```

### Comparing `quantumflow-1.2.1/quantumflow/ops_test.py` & `quantumflow-1.3.0/quantumflow/ops_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pytest
 from sympy import Symbol
 
 import quantumflow as qf
 
 
 def test_operation_incommensurate_qubits() -> None:
-
     gate1 = qf.CCNot("a", "c", "b")
     indices = gate1.qubit_indices(["a", "b", "c"])
     assert indices == (0, 2, 1)
 
     with pytest.raises(ValueError):
         _ = gate1.qubit_indices(["a", "b", "x"])
 
@@ -97,15 +96,15 @@
 
 def test_gate_symbolic_params() -> None:
     theta = Symbol("θ")
 
     gate0 = qf.Rz(theta, 1)
     assert str(gate0) == "Rz(θ) 1"
 
-    gate1 = gate0 ** 4
+    gate1 = gate0**4
     assert str(gate1) == "Rz(4*θ) 1"
 
     circ = qf.Circuit([gate0, gate1])
     print(circ)
     diag = qf.circuit_to_diagram(circ)
     assert diag == "1: ───Rz(θ)───Rz(4*θ)───\n"
```

### Comparing `quantumflow-1.2.1/quantumflow/paulialgebra.py` & `quantumflow-1.3.0/quantumflow/paulialgebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 
 import heapq
 from cmath import isclose  # type: ignore
 from functools import reduce
 from itertools import groupby, product
 from numbers import Complex
 from operator import itemgetter, mul
-from typing import Any, Dict, Iterator, List, Set, Tuple, cast
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, cast
 
 import numpy as np
+import sympy
 
 from . import var
 from .config import ATOL
 from .ops import Operation
 from .qubits import Qubit, Qubits
 from .states import State
 from .tensors import QubitTensor
-from .var import Variable
+from .var import ComplexVariable
 
 __all__ = [
     "PauliTerm",
     "Pauli",
     "sX",
     "sY",
     "sZ",
@@ -60,15 +61,15 @@
     "paulis_commute",
     "pauli_commuting_sets",
     "paulis_close",
     "pauli_decompose_hermitian",
 ]
 
 
-PauliTerm = Tuple[Qubits, str, Variable]
+PauliTerm = Tuple[Qubits, str, ComplexVariable]
 
 PAULI_OPS = ["X", "Y", "Z", "I"]
 
 PAULI_PROD = {
     "ZZ": ("I", 1.0),
     "YY": ("I", 1.0),
     "XX": ("I", 1.0),
@@ -135,31 +136,35 @@
         qbs = sorted(list(qubits))
         super().__init__(qbs)
 
         self.terms = tuple(the_terms)
 
     # Rename coeff?
     @classmethod
-    def term(cls, qubits: Qubits, ops: str, coefficient: Variable = 1.0) -> "Pauli":
+    def term(
+        cls, qubits: Qubits, ops: str, coefficient: ComplexVariable = 1.0
+    ) -> "Pauli":
         """
         Create an element of the Pauli algebra from a sequence of qubits
         and operators. Qubits must be unique and sortable
         """
         return cls((qubits, ops, coefficient))
 
     @classmethod
-    def sigma(cls, qubit: Qubit, operator: str, coefficient: complex = 1.0) -> "Pauli":
+    def sigma(
+        cls, qubit: Qubit, operator: str, coefficient: ComplexVariable = 1.0
+    ) -> "Pauli":
         """Returns a Pauli operator ('I', 'X', 'Y', or 'Z') acting
         on the given qubit"""
         if operator == "I":
             return cls.scalar(coefficient)
         return cls.term([qubit], operator, coefficient)
 
     @classmethod
-    def scalar(cls, coefficient: complex) -> "Pauli":
+    def scalar(cls, coefficient: ComplexVariable) -> "Pauli":
         """Return a scalar multiple of the Pauli identity element."""
         return cls.term((), "", coefficient)
 
     def is_scalar(self) -> bool:
         """Returns true if this object is a scalar multiple of the Pauli
         identity element"""
         if len(self.terms) > 1:
@@ -296,29 +301,29 @@
         if not isinstance(other, Pauli):
             return NotImplemented
         return self.terms == other.terms
 
     def __hash__(self) -> int:
         return hash(self.terms)
 
-    def asoperator(self, qubits: Qubits = None) -> QubitTensor:
+    def asoperator(self, qubits: Optional[Qubits] = None) -> QubitTensor:
         # DOCME: Use of qubits argument here.
 
         # Late import to prevent circular imports
         from .gates import IdentityGate
         from .stdgates import STDGATES as NAMED_GATES
 
         qubits = self.qubits if qubits is None else qubits
         if self.is_zero():
             N = len(qubits)
-            return np.zeros(shape=(2 ** N, 2 ** N))
+            return np.zeros(shape=(2**N, 2**N))
 
         res = []
         for qbs, ops, coeff in self.terms:
-            if var.is_symbolic(coeff):
+            if isinstance(coeff, sympy.Expr):
                 coeff = complex(coeff)
             gate = IdentityGate(qubits)
             for q, op in zip(qbs, ops):
                 gate = NAMED_GATES[op](q) @ gate  # type: ignore
             res.append(gate.asoperator() * coeff)
         return cast(np.ndarray, sum(res))
 
@@ -351,30 +356,30 @@
 
         return pauli_sum(*paulis)
 
 
 # End class Pauli
 
 
-def sX(qubit: Qubit, coefficient: complex = 1) -> Pauli:
+def sX(qubit: Qubit, coefficient: ComplexVariable = 1) -> Pauli:
     """Return the Pauli sigma_X operator acting on the given qubit"""
     return Pauli.sigma(qubit, "X", coefficient)
 
 
-def sY(qubit: Qubit, coefficient: complex = 1) -> Pauli:
+def sY(qubit: Qubit, coefficient: ComplexVariable = 1) -> Pauli:
     """Return the Pauli sigma_Y operator acting on the given qubit"""
     return Pauli.sigma(qubit, "Y", coefficient)
 
 
-def sZ(qubit: Qubit, coefficient: complex = 1) -> Pauli:
+def sZ(qubit: Qubit, coefficient: ComplexVariable = 1) -> Pauli:
     """Return the Pauli sigma_Z operator acting on the given qubit"""
     return Pauli.sigma(qubit, "Z", coefficient)
 
 
-def sI(qubit: Qubit, coefficient: complex = 1) -> Pauli:
+def sI(qubit: Qubit, coefficient: ComplexVariable = 1) -> Pauli:
     """Return the Pauli sigma_I (identity) operator. The qubit is irrelevant,
     but kept as an argument for consistency"""
     return Pauli.sigma(qubit, "I", coefficient)
 
 
 def pauli_sum(*elements: Pauli) -> Pauli:
     """Return the sum of elements of the Pauli algebra"""
@@ -455,16 +460,17 @@
             x = x * x
             n = (n - 1) // 2
     return x * y
 
 
 def paulis_close(pauli0: Pauli, pauli1: Pauli, atol: float = ATOL) -> bool:
     """Returns: True if Pauli elements are almost identical."""
-    pauli = pauli0 - pauli1
-    d = sum(abs(coeff) ** 2 for _, _, coeff in pauli.terms)
+    pauli: Pauli = pauli0 - pauli1
+
+    d = sum(abs(cast(Complex, coeff)) ** 2 for _, _, coeff in pauli.terms)
     return d <= atol
 
 
 def paulis_commute(element0: Pauli, element1: Pauli) -> bool:
     """
     Return true if the two elements of the Pauli algebra commute.
     i.e. if element0 * element1 == element1 * element0
@@ -476,15 +482,14 @@
     def _coincident_parity(term0: PauliTerm, term1: PauliTerm) -> bool:
         non_similar = 0
         key = itemgetter(0)
 
         op0 = zip(term0[0], term0[1])
         op1 = zip(term1[0], term1[1])
         for _, qops in groupby(heapq.merge(op0, op1, key=key), key=key):
-
             listqops = list(qops)
             if len(listqops) == 2 and listqops[0][1] != listqops[1][1]:
                 non_similar += 1
         return non_similar % 2 == 0
 
     for term0, term1 in product(element0, element1):
         if not _coincident_parity(term0, term1):
@@ -516,15 +521,17 @@
                 break
         if not assigned:
             groups.append(pterm)
 
     return tuple(groups)
 
 
-def pauli_decompose_hermitian(matrix: np.ndarray, qubits: Qubits = None) -> Pauli:
+def pauli_decompose_hermitian(
+    matrix: np.ndarray, qubits: Optional[Qubits] = None
+) -> Pauli:
     """Decompose a Hermitian matrix into an element of the Pauli algebra.
 
     This works because tensor products of Pauli matrices form an orthonormal
     basis in the linear space of all 2^N×2^N matrices under Hilbert-Schmidt
     inner product.
     """
     # TODO: This should work for any matrix, not just Hermitian?
@@ -545,15 +552,15 @@
         qubits = list(range(N))
     else:
         assert len(qubits) == N
 
     terms = []
     for ops in product("IXYZ", repeat=N):
         P = Pauli.term(qubits, "".join(ops)).asoperator(qubits=qubits)
-        coeff = np.real(np.trace(P @ matrix) / (2 ** N))
+        coeff = np.real(np.trace(P @ matrix) / (2**N))
         term = Pauli.term(qubits, "".join(ops), coeff)
         terms.append(term)
 
     return pauli_sum(*terms)
 
 
 # fin
```

### Comparing `quantumflow-1.2.1/quantumflow/paulialgebra_test.py` & `quantumflow-1.3.0/quantumflow/paulialgebra_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,24 +182,24 @@
     assert len(p) == 1
     assert p.terms[0][2] == 5
 
 
 def test_power() -> None:
     p = sX(0) + sY(1) + qf.Pauli.term([2, 3], "XY")
 
-    assert p ** 0 == qf.Pauli.identity()
-    assert p ** 1 == p
-    assert p * p == p ** 2
-    assert p * p * p == p ** 3
-    assert p * p * p * p * p * p * p * p * p * p == p ** 10
+    assert p**0 == qf.Pauli.identity()
+    assert p**1 == p
+    assert p * p == p**2
+    assert p * p * p == p**3
+    assert p * p * p * p * p * p * p * p * p * p == p**10
 
     with pytest.raises(ValueError):
-        p ** -1
+        p**-1
 
-    p ** 400
+    p**400
 
 
 def test_simplify() -> None:
     t1 = sZ(0) * sZ(1)
     t2 = sZ(0) * sZ(1)
     assert (t1 + t2) == 2 * sZ(0) * sZ(1)
```

### Comparing `quantumflow-1.2.1/quantumflow/qubits.py` & `quantumflow-1.3.0/quantumflow/qubits.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 sortable python object (most immutable types), but typically an integer or string.
 e.g. `[0, 1, 2]`, or `['a', 'b', 'c']`.
 
 """
 
 from typing import Any, Sequence
 
-from .utils import Protocol
+from .future import Protocol, TypeAlias
 
 __all__ = ("Qubit", "Qubits", "sorted_qubits")
 
 
 class Qubit(Protocol):
     """Type for qubits. Any sortable and hashable python object.
     e.g. strings, integers, tuples of strings and integers, etc.
     """
 
-    def __lt__(self, other: Any) -> bool:
+    def __lt__(self, other: Any, /) -> bool:
         pass
 
     def __hash__(self) -> int:
         pass
 
 
-Qubits = Sequence[Qubit]
+Qubits: TypeAlias = Sequence[Qubit]
 """Type for sequence of qubits"""
 
 
 def sorted_qubits(qbs: Qubits) -> Qubits:
     """Return a sorted list of unique qubits in canonical order.
 
     Qubits can be of different types, so we sort first by type (as a string),
```

### Comparing `quantumflow-1.2.1/quantumflow/states.py` & `quantumflow-1.3.0/quantumflow/states.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from math import sqrt
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Mapping,
+    Optional,
     TextIO,
     Tuple,
     TypeVar,
     Union,
 )
 
 import numpy as np
@@ -67,22 +68,20 @@
     "zero_state",
     "Density",
     "mixed_density",
     "random_density",
     "join_densities",
 ]
 
-
-QuantumStateType = TypeVar("QuantumStateType", bound="QuantumState")
-"""TypeVar for quantum states"""
+QuantumStateTV = TypeVar("QuantumStateTV", bound="QuantumState")
 
 
 class QuantumState(ABC):
     def __init__(
-        self, tensor: "ArrayLike", qubits: Qubits, memory: Mapping = None
+        self, tensor: "ArrayLike", qubits: Qubits, memory: Optional[Mapping] = None
     ) -> None:
         """
         Abstract base class for representations of a quantum state.
 
         Args:
             tensor: A vector or tensor of state amplitudes
             qubits: A sequence of qubit names.
@@ -116,46 +115,48 @@
 
     @property
     def qubit_nb(self) -> int:
         """Return the total number of qubits"""
         return len(self._qubits)
 
     def replace(
-        self: QuantumStateType,
+        self: QuantumStateTV,
         *,
-        tensor: "ArrayLike" = None,
-        qubits: Qubits = None,
-        memory: Mapping = None,
-    ) -> QuantumStateType:
+        tensor: Optional["ArrayLike"] = None,
+        qubits: Optional[Qubits] = None,
+        memory: Optional[Mapping] = None,
+    ) -> QuantumStateTV:
         """
         Creates a copy of this state, replacing the fields specified.
         """
         # Interface similar to dataclasses.replace
         tensor = self.tensor if tensor is None else tensor
         qubits = self.qubits if qubits is None else qubits
         memory = self.memory if memory is None else memory
         return type(self)(tensor, qubits, memory)
 
-    def store(self: QuantumStateType, *args: Any, **kwargs: Any) -> QuantumStateType:
+    def store(self: QuantumStateTV, *args: Any, **kwargs: Any) -> QuantumStateTV:
         """Update information in classical memory and return a new State."""
         mem = self.memory.update(*args, **kwargs)
         return self.replace(memory=mem)
 
     # TESTME
-    def on(self: QuantumStateType, *qubits: Qubit) -> QuantumStateType:
+    def on(self: QuantumStateTV, *qubits: Qubit) -> QuantumStateTV:
         """Return a copy of this State with new qubits"""
         return self.replace(qubits=qubits)
 
     # TESTME
-    def rewire(self: QuantumStateType, labels: Dict[Qubit, Qubit]) -> QuantumStateType:
+    def rewire(self: QuantumStateTV, labels: Dict[Qubit, Qubit]) -> QuantumStateTV:
         """Relabel qubits and return copy of this Operation"""
         qubits = tuple(labels[q] for q in self.qubits)
         return self.on(*qubits)
 
-    def permute(self: QuantumStateType, qubits: Qubits = None) -> QuantumStateType:
+    def permute(
+        self: QuantumStateTV, qubits: Optional[Qubits] = None
+    ) -> QuantumStateTV:
         """Return a copy of this state with state tensor transposed to
         put qubits in the given order. If an explicit qubit
         ordering isn't supplied, we put qubits in sorted order.
         """
         if qubits is None:
             qubits = sorted_qubits(self.qubits)
         tensor = tensors.permute(self.tensor, self.qubit_indices(qubits))
@@ -179,15 +180,18 @@
 
     Note that memory usage grows exponentially with the number of qubits.
     (16*2^N bytes for N qubits)
 
     """
 
     def __init__(
-        self, tensor: "ArrayLike", qubits: Qubits = None, memory: Mapping = None
+        self,
+        tensor: "ArrayLike",
+        qubits: Optional[Qubits] = None,
+        memory: Optional[Mapping] = None,
     ) -> None:
         """Create a new State from a tensor of qubit amplitudes
 
         Args:
             tensor: A vector or tensor of state amplitudes
             qubits: A sequence of qubit names.
                 (Defaults to integer indices, e.g. [0, 1, 2] for 3 qubits)
@@ -223,15 +227,15 @@
         # TODO: Can we do this within backend?
         probs = np.real(self.probabilities())
         res = np.random.multinomial(trials, probs.ravel())
         res = res.reshape(probs.shape)
         return res
 
     def expectation(
-        self, diag_hermitian: "ArrayLike", trials: int = None
+        self, diag_hermitian: "ArrayLike", trials: Optional[int] = None
     ) -> QubitTensor:
         """Return the expectation of a measurement. Since we can only measure
         our computer in the computational basis, we only require the diagonal
         of the Hermitian in that basis.
 
         If the number of trials is specified, we sample the given number of
         times. Else we return the exact expectation (as if we'd performed an
@@ -250,18 +254,17 @@
 
         Returns:
             A [2]*bits array of qubit states, either 0 or 1
         """
         probs = np.real(self.probabilities())
         indices = np.asarray(list(np.ndindex(*[2] * self.qubit_nb)))
         res = np.random.choice(probs.size, p=probs.ravel())
-        res = indices[res]
-        return res
+        return indices[res]
 
-    def asdensity(self, qubits: Qubits = None) -> "Density":
+    def asdensity(self, qubits: Optional[Qubits] = None) -> "Density":
         """Convert a pure state to a density matrix.
 
         Args:
             qubits: The qubit subspace. If not given return the density
                     matrix for all the qubits (which can take a lot of memory!)
         """
         N = self.qubit_nb
@@ -353,23 +356,25 @@
 
 
 # = Output =
 
 # TODO: clean up. Move to visualization?
 
 
-def print_state(state: State, file: TextIO = None) -> None:
+def print_state(state: State, file: Optional[TextIO] = None) -> None:
     """Print a state vector"""
     for index, amplitude in np.ndenumerate(state.tensor):
         ket = "".join([str(n) for n in index])
         print(ket, ":", amplitude, file=file)
 
 
 # TODO: Should work for density also. Check
-def print_probabilities(state: State, ndigits: int = 4, file: TextIO = None) -> None:
+def print_probabilities(
+    state: State, ndigits: int = 4, file: Optional[TextIO] = None
+) -> None:
     """
     Pretty print state probabilities.
 
     Args:
         state:
         ndigits: Number of digits of accuracy
         file: Output stream (Defaults to stdout)
@@ -386,15 +391,18 @@
 # --  Mixed Quantum States --
 
 
 class Density(QuantumState):
     """A density matrix representation of a mixed quantum state"""
 
     def __init__(
-        self, tensor: "ArrayLike", qubits: Qubits = None, memory: Mapping = None
+        self,
+        tensor: "ArrayLike",
+        qubits: Optional[Qubits] = None,
+        memory: Optional[Mapping] = None,
     ) -> None:
         tensor = tensors.asqutensor(tensor)
 
         N = np.ndim(tensor) // 2
         if qubits is None:
             qubits = range(N)
         elif len(qubits) != N:
@@ -417,30 +425,32 @@
         prob = tensors.diag(self.tensor)
         return prob
 
     def asoperator(self) -> QubitTensor:
         """Return the density matrix as a square array"""
         return tensors.flatten(self.tensor, rank=2)
 
-    def asdensity(self, qubits: Qubits = None) -> "Density":
+    def asdensity(self, qubits: Optional[Qubits] = None) -> "Density":
         if qubits is None:
             return self
         tensor = tensors.partial_trace(self.tensor, self.qubit_indices(qubits))
         return Density(tensor, qubits, self.memory)
 
 
 def mixed_density(qubits: Union[int, Qubits]) -> Density:
     """Returns the completely mixed density matrix"""
     N, qubits = _qubits_count_tuple(qubits)
-    matrix = np.eye(2 ** N) / 2 ** N
+    matrix = np.eye(2**N) / 2**N
     return Density(matrix, qubits)
 
 
 def random_density(
-    qubits: Union[int, Qubits], rank: int = None, ensemble: str = "Hilbert–Schmidt"
+    qubits: Union[int, Qubits],
+    rank: Optional[int] = None,
+    ensemble: str = "Hilbert–Schmidt",
 ) -> Density:
     """
     Returns: A randomly sampled Density
 
     Args:
         qubits: A list or number of qubits.
         rank: Rank of density matrix. (Defaults to full rank)
@@ -460,54 +470,58 @@
         return random_density_bures(qubits, rank)
     raise ValueError(
         "Unknown ensemble. " "Valid Options are 'Hilbert–Schmidt' or 'Bures"
     )
 
 
 # TODO: Check math
-def random_density_hs(qubits: Union[int, Qubits], rank: int = None) -> Density:
+def random_density_hs(
+    qubits: Union[int, Qubits], rank: Optional[int] = None
+) -> Density:
     """
     Returns: A randomly sampled Density from the Hilbert–Schmidt
                 ensemble of quantum states.
 
     Args:
         qubits: A list or number of qubits.
         rank: Rank of density matrix. (Defaults to full rank)
 
     Ref:
         "Induced.info in the space of mixed quantum states" Karol
         Zyczkowski, Hans-Juergen Sommers, J. Phys. A34, 7111-7125 (2001)
         arXiv:quant-ph/0012101
     """
     N, qubits = _qubits_count_tuple(qubits)
-    size = (2 ** N, 2 ** N) if rank is None else (2 ** N, rank)
+    size = (2**N, 2**N) if rank is None else (2**N, rank)
 
     X = utils.complex_ginibre_ensemble(size)
     matrix = X @ X.conj().T
     matrix /= np.trace(matrix)
 
     return Density(matrix, qubits=qubits)
 
 
 # TODO: Check math
-def random_density_bures(qubits: Union[int, Qubits], rank: int = None) -> Density:
+def random_density_bures(
+    qubits: Union[int, Qubits], rank: Optional[int] = None
+) -> Density:
     """
     Returns: A random Density drawn from the Bures measure.
 
     Args:
         qubits: A list or number of qubits.
         rank: Rank of density matrix. (Defaults to full rank)
 
     Ref:
         "Random Bures mixed states and the distribution of their purity",
          Osipov, Sommers, and Zyczkowski, J. Phys. A: Math. Theor. 43,
          055302 (2010). arXiv:0909.5094
     """
     N, qubits = _qubits_count_tuple(qubits)
-    dim = 2 ** N
+    dim = 2**N
     size = (dim, dim) if rank is None else (dim, rank)
     P = np.eye(dim) + utils.unitary_ensemble(dim)
     G = utils.complex_ginibre_ensemble(size=size)
     B = P @ G @ G.conj().T @ P.conj().T
     B /= np.trace(B)
 
     return Density(B, qubits=qubits)
```

### Comparing `quantumflow-1.2.1/quantumflow/states_test.py` & `quantumflow-1.3.0/quantumflow/states_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/__init__.py` & `quantumflow-1.3.0/quantumflow/stdgates/__init__.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # DO Rename
 
 from typing import ClassVar, Dict, List, Mapping, Type, TypeVar
 
 import numpy as np
 import scipy
 
-from .. import utils
 from ..config import CONJ, CTRL, SQRT
+from ..future import cached_property
 from ..ops import _EXCLUDED_OPERATIONS, Gate
 from ..paulialgebra import Pauli, sZ
 from ..qubits import Qubit, Qubits
 from ..tensors import QubitTensor, asqutensor
 from ..var import Variable
 
 __all__ = (
@@ -70,15 +70,14 @@
         args.extend(str(p) for p in self.params)
         args.extend(str(qubit) for qubit in self.qubits)
         fargs = ", ".join(args)
 
         return f"{self.name}({fargs})"
 
     def _diagram_labels_(self) -> List[str]:
-
         label = self.name
 
         label = label.replace("ISwap", "iSwap")
         label = label.replace("Phased", "Ph")
 
         if label.startswith("Sqrt"):
             label = SQRT + label[4:]
@@ -103,29 +102,29 @@
                 labels[i] = labels[i] + "_%s" % i
 
         return labels
 
 
 # End class StdGate
 
-
-StdCtrlGateType = TypeVar("StdCtrlGateType", bound="StdCtrlGate")
-"""Generic type annotations for subtypes of StdCtrlGate"""
+StdCtrlGateTV = TypeVar("StdCtrlGateTV", bound="StdCtrlGate")
 
 
 class StdCtrlGate(StdGate):
     """A standard gate that is a controlled version of another standard gate.
 
     Subclasses should set the `cv_target` class variable to the target gate type.
     """
 
     # nb: ControlGate and StdCtrlGate share interface and code.
     # But unification probably not worth the trouble
 
-    cv_target: ClassVar[Type[StdGate]] = None
+    from .stdgates_1q import I
+
+    cv_target: ClassVar[Type[StdGate]] = I  # null gate
     """StdGate type that is the target of this controlled gate.
     Should be set by subclasses"""
 
     def __init_subclass__(cls) -> None:
         super().__init_subclass__()
 
         assert cls.cv_target is not None
@@ -157,25 +156,25 @@
     @property
     def hamiltonian(self) -> Pauli:
         ham = self.target.hamiltonian
         for q in self.control_qubits:
             ham *= (1 - sZ(q)) / 2
         return ham
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         ctrl_block = np.identity(
-            2 ** self.cv_qubit_nb - 2 ** self.cv_target.cv_qubit_nb
+            2**self.cv_qubit_nb - 2**self.cv_target.cv_qubit_nb
         )
         target_block = self.target.asoperator()
         unitary = scipy.linalg.block_diag(ctrl_block, target_block)
 
         return asqutensor(unitary)
 
-    def resolve(self: StdCtrlGateType, subs: Mapping[str, float]) -> StdCtrlGateType:
+    def resolve(self: StdCtrlGateTV, subs: Mapping[str, float]) -> StdCtrlGateTV:
         target = self.target.resolve(subs)
         return type(self)(*target.params, *self.qubits)  # type: ignore
 
     def _diagram_labels_(self) -> List[str]:
         return ([CTRL] * self.control_qubit_nb) + self.target._diagram_labels_()
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_1q.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_1q.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 from typing import Dict, List, Type
 
 import numpy as np
 
 from .. import tensors, utils, var
+from ..future import cached_property
 from ..paulialgebra import Pauli, sI, sX, sY, sZ
 from ..qubits import Qubit
 from ..states import Density, State
 from ..tensors import QubitTensor
 from ..var import PI, Variable
 from .stdgates import StdGate
 
@@ -55,23 +56,16 @@
     Args:
         gate:       The gate instance to specialize
         periods:    The periods of the gate's parameters. Gate parameters
                     are wrapped to range[0,period]
         opts:       A map from particular gate parameters to a special case
                     of the original gate type
     """
-    # params = list(gate.params)
 
-    params = list(gate.params)
-
-    # for p in params:
-    #     if variable_is_symbolic(p):
-    #         return gate
-
-    params = [var.asfloat(p) % pd for p, pd in zip(params, periods)]
+    params = [var.asfloat(p) % pd for p, pd in zip(gate.params, periods)]
 
     for values, gatetype in opts.items():
         if np.isclose(params, values):
             return gatetype(*gate.qubits)  # type: ignore
 
     return type(gate)(*params, *gate.qubits)  # type: ignore
 
@@ -92,15 +86,15 @@
     def __init__(self, q0: Qubit) -> None:
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         return Pauli.zero()
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return tensors.asqutensor(np.eye(2))
 
     @property
     def H(self) -> "I":
         return self  # Hermitian
 
@@ -141,23 +135,23 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         (phi,) = self.params
         return -phi * sI(q0)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         phi = var.asfloat(self.param("phi"))
         unitary = [[np.exp(1j * phi), 0.0], [0.0, np.exp(1j * phi)]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Ph":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Ph":
         return Ph(t * self.param("phi"), *self.qubits)
 
     def run(self, ket: State) -> State:
         (phi,) = self.params
         tensor = ket.tensor * np.exp(1j * phi)
@@ -186,15 +180,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -(PI / 2) * (1 - sX(q0))
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = [[0, 1], [1, 0]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "X":
         return self  # Hermitian
@@ -228,15 +222,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -(PI / 2) * (1 - sY(q0))
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray([[0, -1.0j], [1.0j, 0]])
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Y":
         return self  # Hermitian
@@ -268,15 +262,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -(PI / 2) * (1 - sZ(q0))
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray([[1, 0], [0, -1.0]])
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Z":
         return self  # Hermitian
@@ -305,15 +299,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return (PI / 2) * ((sX(q0) + sZ(q0)) / np.sqrt(2) - 1)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray([[1, 1], [1, -1]]) / np.sqrt(2)
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "_H":  # See NB implementation note below
         return self  # Hermitian
@@ -355,15 +349,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return (PI / 2) * (sZ(q0) - 1) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray([[1.0, 0.0], [0.0, 1.0j]])
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "S_H":
         return S_H(*self.qubits)
@@ -392,15 +386,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return (PI / 2) * (sZ(q0) - 1) / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = [[1.0, 0.0], [0.0, np.exp(1j * np.pi / 4.0)]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "T_H":
         return T_H(*self.qubits)
@@ -431,23 +425,23 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (theta,) = self.params
         (q0,) = self.qubits
         return theta * (sZ(q0) - 1) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
         unitary = [[1.0, 0.0], [0.0, np.exp(1j * theta)]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "PhaseShift":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "PhaseShift":
         return PhaseShift(self.param("theta") * t, *self.qubits)
 
     def run(self, ket: State) -> State:
         (theta,) = self.params
         return ZPow(theta / np.pi, *self.qubits).run(ket)
@@ -485,26 +479,26 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (theta,) = self.params
         (q0,) = self.qubits
         return theta * sX(q0) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
         unitary = [
             [np.cos(theta / 2), -1.0j * np.sin(theta / 2)],
             [-1.0j * np.sin(theta / 2), np.cos(theta / 2)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Rx":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Rx":
         return Rx(self.param("theta") * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
         (theta,) = self.params
@@ -535,26 +529,26 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (theta,) = self.params
         (q0,) = self.qubits
         return theta * sY(q0) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
         unitary = [
             [np.cos(theta / 2.0), -np.sin(theta / 2.0)],
             [np.sin(theta / 2.0), np.cos(theta / 2.0)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Ry":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Ry":
         return Ry(self.param("theta") * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
         (theta,) = self.params
@@ -585,23 +579,23 @@
         super().__init__(params=[theta], qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return self.param("theta") * sZ(q0) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
         unitary = [[np.exp(-theta * 0.5j), 0], [0, np.exp(theta * 0.5j)]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Rz":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Rz":
         return Rz(self.param("theta") * t, *self.qubits)
 
     def run(self, ket: State) -> State:
         (theta,) = self.params
         return ZPow(theta / np.pi, *self.qubits).run(ket)
@@ -636,15 +630,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -PI * (sZ(q0) - 1) / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray([[1.0, 0.0], [0.0, -1.0j]])
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "S":
         return S(*self.qubits)
@@ -673,15 +667,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -PI * (sZ(q0) - 1) / 8
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = [[1.0, 0.0], [0.0, np.exp(-1j * np.pi / 4.0)]]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "T":
         return T(*self.qubits)
@@ -707,31 +701,30 @@
         theta: Angle of rotation on Block sphere
         (nx, ny, nz): A three-dimensional real unit vector
     """
 
     def __init__(
         self, theta: Variable, nx: Variable, ny: Variable, nz: Variable, q0: Qubit
     ) -> None:
-
-        norm = var.sqrt(nx ** 2 + ny ** 2 + nz ** 2)
+        norm = var.sqrt(nx**2 + ny**2 + nz**2)
 
         nx /= norm
         ny /= norm
         nz /= norm
         theta *= norm
 
         super().__init__(params=[theta, nx, ny, nz], qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         theta, nx, ny, nz = self.params
         (q0,) = self.qubits
         return theta * (nx * sX(q0) + ny * sY(q0) + nz * sZ(q0)) / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
         nx = var.asfloat(self.param("nx"))
         ny = var.asfloat(self.param("ny"))
         nz = var.asfloat(self.param("nz"))
 
         cost = np.cos(theta / 2)
@@ -741,15 +734,15 @@
             [-1j * sint * nx + sint * ny, cost + 1j * sint * nz],
         ]
 
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Rn":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Rn":
         theta, nx, ny, nz = self.params
         return Rn(t * theta, nx, ny, nz, *self.qubits)
 
     # TODO:     def specialize(self) -> Gate:
 
@@ -772,27 +765,27 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (t,) = self.params
         (q0,) = self.qubits
         return t * (sX(q0) - 1) * PI / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = np.pi * var.asfloat(self.param("t"))
         phase = np.exp(0.5j * theta)
         unitary = [
             [phase * np.cos(theta / 2), phase * -1.0j * np.sin(theta / 2)],
             [phase * -1.0j * np.sin(theta / 2), phase * np.cos(theta / 2)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "XPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "XPow":
         return XPow(t * self.param("t"), *self.qubits)
 
     def specialize(self) -> StdGate:
         opts = {0.0: I, 0.5: V, 1.0: X, 1.5: V_H, 2.0: I}
         return _specialize_gate(self, [2], opts)
@@ -819,27 +812,27 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (t,) = self.params
         (q0,) = self.qubits
         return t * (sY(q0) - 1) * PI / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = np.pi * var.asfloat(self.param("t"))
         phase = np.exp(0.5j * theta)
         unitary = [
             [phase * np.cos(theta / 2.0), phase * -np.sin(theta / 2.0)],
             [phase * np.sin(theta / 2.0), phase * np.cos(theta / 2.0)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "YPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "YPow":
         return YPow(t * self.param("t"), *self.qubits)
 
     def specialize(self) -> StdGate:
         opts = {0.0: I, 1.0: Y, 2.0: I}
         return _specialize_gate(self, [2], opts)
@@ -864,15 +857,15 @@
 
     @property
     def hamiltonian(self) -> Pauli:
         (t,) = self.params
         (q0,) = self.qubits
         return t * (sZ(q0) - 1) * PI / 2
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = np.pi * var.asfloat(self.param("t"))
         phase = np.exp(0.5j * theta)
         unitary = [
             [phase * np.exp(-theta * 0.5j), 0],
             [0, phase * np.exp(theta * 0.5j)],
         ]
@@ -918,15 +911,15 @@
     def __init__(self, t: Variable, q0: Qubit) -> None:
         super().__init__(params=[t], qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         return H(*self.qubits).hamiltonian * self.param("t")
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = np.pi * var.asfloat(self.param("t"))
         phase = np.exp(0.5j * theta)
         unitary = [
             [
                 phase * np.cos(theta / 2)
                 - (phase * 1.0j * np.sin(theta / 2)) / np.sqrt(2),
@@ -938,15 +931,15 @@
                 + (phase * 1.0j * np.sin(theta / 2)) / np.sqrt(2),
             ],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "HPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "HPow":
         return HPow(t * self.param("t"), *self.qubits)
 
     def specialize(self) -> StdGate:
         opts = {0.0: I, 1.0: H, 2.0: I}
         return _specialize_gate(self, [2], opts)
@@ -964,15 +957,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return (sX(q0) - 1) * PI / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return XPow(0.5, *self.qubits).tensor
 
     @property
     def H(self) -> "V_H":
         return V_H(*self.qubits)
 
@@ -992,15 +985,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -(sX(q0) - 1) * PI / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return XPow(-0.5, *self.qubits).tensor
 
     @property
     def H(self) -> "V":
         return V(*self.qubits)
 
@@ -1020,15 +1013,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return (sY(q0) - 1) * PI / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return YPow(0.5, *self.qubits).tensor
 
     @property
     def H(self) -> "SqrtY_H":
         return SqrtY_H(*self.qubits)
 
@@ -1048,15 +1041,15 @@
         super().__init__(qubits=[q0])
 
     @property
     def hamiltonian(self) -> Pauli:
         (q0,) = self.qubits
         return -(sY(q0) - 1) * PI / 4
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return YPow(-0.5, *self.qubits).tensor
 
     @property
     def H(self) -> "SqrtY":
         return SqrtY(*self.qubits)
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_1q_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_1q_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_2q.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_2q.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 from typing import List
 
 import numpy as np
 
 from .. import tensors, utils, var
 from ..config import CTRL, SWAP_TARGET, TARGET
+from ..future import cached_property
 from ..ops import UnitaryGate
 from ..paulialgebra import Pauli, sX, sY, sZ
 from ..qubits import Qubit
 from ..states import State
 from ..tensors import QubitTensor
-from ..utils import cached_property
 from ..var import PI, Variable
 from .stdgates import StdCtrlGate, StdGate
 from .stdgates_1q import V_H, H, I, S, T, V, X, XPow, Y, YPow, Z, ZPow
 
 _H = H
 
 # 2 qubit gates, alphabetic order
@@ -120,15 +120,15 @@
             * np.sqrt(2 - np.sqrt(2))
             / 2
         )
         return tensors.asqutensor(U)
 
     @property
     def H(self) -> "Can":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Can":
         return Can(-t / 2, -t / 4, 0, *self.qubits)
 
 
 class Barenco(StdGate):
     """A universal two-qubit gate:
@@ -224,15 +224,15 @@
 
         gate = yy @ xx
         gate = zz @ gate
         return gate.tensor
 
     @property
     def H(self) -> "Can":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Can":
         tx, ty, tz = self.params
         return Can(tx * t, ty * t, tz * t, *self.qubits)
 
     # TODO: XY, ECP, ...
     def specialize(self) -> StdGate:
@@ -355,15 +355,15 @@
     cv_target = XPow
 
     def __init__(self, t: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[t], qubits=[q0, q1])
 
     @property
     def H(self) -> "CNotPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "CNotPow":
         (t,) = self.params
         return CNotPow(e * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
@@ -395,15 +395,15 @@
     @cached_property
     def tensor(self) -> QubitTensor:
         U = UnitaryGate.from_hamiltonian(self.hamiltonian, self.qubits)
         return tensors.asqutensor(U.tensor)
 
     @property
     def H(self) -> "CrossResonance":
-        return self ** -1
+        return self**-1
 
     # TESTME
     def __pow__(self, t: Variable) -> "CrossResonance":
         s, b, c = self.params
         return CrossResonance(t * s, b, c, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
@@ -497,15 +497,15 @@
     cv_target = YPow
 
     def __init__(self, t: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[t], qubits=[q0, q1])
 
     @property
     def H(self) -> "CYPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "CYPow":
         (t,) = self.params
         return CYPow(e * t, *self.qubits)
 
 
 # End class CYPow
@@ -606,15 +606,15 @@
     cv_tensor_structure = "diagonal"
 
     def __init__(self, t: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[t], qubits=[q0, q1])
 
     @property
     def H(self) -> "CZPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "CZPow":
         (t,) = self.params
         return CZPow(e * t, *self.qubits)
 
 
 # End class CZPow
@@ -640,15 +640,15 @@
 
     @cached_property
     def tensor(self) -> QubitTensor:
         return Can(1 / 2, 1 / 4, 1 / 4, *self.qubits).tensor
 
     @property
     def H(self) -> "Can":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Can":
         return Can(t / 2, t / 4, t / 4, *self.qubits)
 
 
 # end class ECP
 
@@ -672,15 +672,15 @@
     @cached_property
     def tensor(self) -> QubitTensor:
         (t,) = self.params
         return Can(t, t, t, *self.qubits).tensor
 
     @property
     def H(self) -> "Exch":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "Exch":
         (t,) = self.params
         return Exch(e * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
@@ -737,15 +737,15 @@
             [0, np.sin(theta), np.cos(theta), 0],
             [0, 0, 0, 1],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "Givens":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "Givens":
         (theta,) = self.params
         return Givens(t * theta, *self.qubits)
 
 
 # end class Givens
@@ -784,15 +784,15 @@
         s01 = utils.multi_slice(axes, [0, 1])
         tensor[s01] = 1.0j * ket.tensor[s10]
         tensor[s10] = 1.0j * ket.tensor[s01]
         return State(tensor, ket.qubits, ket.memory)
 
     @property
     def H(self) -> "XY":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "XY":
         return XY(-t / 2, *self.qubits)
 
 
 # end class ISWAP
 
@@ -1053,15 +1053,15 @@
             [0, -1.0j * np.sin(theta / 2), np.cos(theta / 2), 0],
             [-1.0j * np.sin(theta / 2), 0, 0, np.cos(theta / 2)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "XX":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "XX":
         (t,) = self.params
         return XX(e * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
@@ -1095,15 +1095,15 @@
     @cached_property
     def tensor(self) -> QubitTensor:
         t = var.asfloat(self.param("t"))
         return Can(t, t, 0, *self.qubits).tensor
 
     @property
     def H(self) -> "XY":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "XY":
         (t,) = self.params
         return XY(e * t, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return ["XY^{t}"] * 2
@@ -1138,15 +1138,15 @@
             [0, -1.0j * np.sin(theta / 2), np.cos(theta / 2), 0],
             [1.0j * np.sin(theta / 2), 0, 0, np.cos(theta / 2)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "YY":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "YY":
         (t,) = self.params
         return YY(e * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
@@ -1195,15 +1195,15 @@
                 [[0, 0], [0, np.exp(-1j * theta / 2)]],
             ],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "ZZ":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "ZZ":
         (t,) = self.params
         return ZZ(e * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_2q_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_2q_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_3q.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_3q.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 from typing import List
 
 import numpy as np
 
 from .. import tensors, utils, var
 from ..config import CTRL
+from ..future import cached_property
 from ..paulialgebra import Pauli, sX, sZ
 from ..qubits import Qubit
 from ..states import State
 from ..tensors import QubitTensor
 from ..var import PI, Variable
 from .stdgates import StdCtrlGate, StdGate
 from .stdgates_1q import X, XPow, Z
@@ -57,15 +58,15 @@
         super().__init__(qubits=[q0, q1, q2])
 
     @property
     def hamiltonian(self) -> Pauli:
         q0, q1, q2 = self.qubits
         return -sX(q2) * (1 - sZ(q1)) * (1 - sZ(q0)) * PI / 8
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray(
             [
                 [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
@@ -143,15 +144,15 @@
     cv_target = XPow
 
     def __init__(self, t: Variable, q0: Qubit, q1: Qubit, q2: Qubit) -> None:
         super().__init__(params=[t], qubits=[q0, q1, q2])
 
     @property
     def H(self) -> "CCXPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "CCXPow":
         (t,) = self.params
         return CCXPow(e * t, *self.qubits)
 
 
 # end class CCXPow
@@ -301,15 +302,15 @@
         D. Deutsch, Quantum Computational Networks,
             Proc. R. Soc. Lond. A 425, 73 (1989).
     """
 
     def __init__(self, theta: Variable, q0: Qubit, q1: Qubit, q2: Qubit) -> None:
         super().__init__(params=[theta], qubits=[q0, q1, q2])
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         theta = var.asfloat(self.param("theta"))
 
         unitary = [
             [1, 0, 0, 0, 0, 0, 0, 0],
             [0, 1, 0, 0, 0, 0, 0, 0],
             [0, 0, 1, 0, 0, 0, 0, 0],
@@ -365,15 +366,15 @@
         return (
             (1 - sZ(q0))
             * (-2 - sZ(q1) * sX(q2) + sZ(q1) * sZ(q2) + sX(q2) + sZ(q2))
             * PI
             / 8
         )
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         unitary = np.asarray(
             [
                 [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_3q_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_3q_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_cirq.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_cirq.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from typing import List
 
 import numpy as np
 
 from .. import tensors, var
 from ..config import SWAP_TARGET
+from ..future import cached_property
 from ..paulialgebra import Pauli
 from ..qubits import Qubit
 from ..tensors import QubitTensor
-from ..utils import cached_property
 from ..var import Variable
 from .stdgates import StdGate
 from .stdgates_1q import I, X, XPow, ZPow
 from .stdgates_2q import CZ, Swap
 
 __all__ = ("PhasedX", "PhasedXPow", "FSim", "FSwap", "FSwapPow", "Sycamore")
 
@@ -80,15 +80,15 @@
     def tensor(self) -> QubitTensor:
         p, t = self.params
         gate = ZPow(p, 0) @ XPow(t, 0) @ ZPow(-p, 0)
         return gate.tensor
 
     @property
     def H(self) -> "PhasedXPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "PhasedXPow":
         p, s = self.params
         return PhasedXPow(p, s * t, *self.qubits)
 
     def specialize(self) -> StdGate:
         qbs = self.qubits
@@ -147,15 +147,15 @@
             [0, -1.0j * np.sin(theta), np.cos(theta), 0],
             [0, 0, 0, np.exp(-1j * phi)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "FSim":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "FSim":
         theta, phi = self.params
         return FSim(theta * t, phi * t, *self.qubits)
 
 
 # end class FSim
@@ -237,26 +237,27 @@
             [0, -1.0j * g * s, g * c, 0],
             [0, 0, 0, p],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "FSwapPow":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "FSwapPow":
         (t,) = self.params
         return FSwapPow(e * t, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return [SWAP_TARGET + "ᶠ^{t}"] * 2
 
 
 # End class FSwapPow
 
+
 # FIXME: Syc
 class Sycamore(StdGate):
     r"""The Sycamore gate is a two-qubit gate equivalent to
     ``FSim(π/2, π/6)``, and locally equivalent to ``Can(1/2, 1/2, 1/12)``.
 
     This gate was used to demonstrate quantum on Google's Sycamore chip.
 
@@ -282,15 +283,15 @@
 
     @cached_property
     def tensor(self) -> QubitTensor:
         return FSim(np.pi / 2, np.pi / 6, 0, 1).tensor
 
     @property
     def H(self) -> "FSim":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "FSim":
         return FSim(t * np.pi / 2, t * np.pi / 6, *self.qubits)
 
 
 # end class Sycamore
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_cirq_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_cirq_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     q0 = "4"
     for _ in range(REPS):
         t = random.uniform(0, 1)
         p = random.uniform(-2, +2)
 
         gate0 = qf.PhasedX(p, q0)
         gate1 = qf.PhasedXPow(p, t, q0)
-        assert qf.gates_close(gate0 ** t, gate1)
-        assert (gate0 ** t).qubits == (q0,)
+        assert qf.gates_close(gate0**t, gate1)
+        assert (gate0**t).qubits == (q0,)
 
         gate0.H
         gate1.H
-        gate2 = gate1 ** t
+        gate2 = gate1**t
         p2, t2 = gate2.params
         assert p2 == p
-        assert np.isclose(t2 - t ** 2, 0.0)
+        assert np.isclose(t2 - t**2, 0.0)
 
         assert qf.gates_close(gate0, gate0.specialize())
 
     assert qf.gates_close(qf.PhasedX(-2.0, q0).specialize(), qf.X(q0))
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_forest.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from typing import List
 
 import numpy as np
 
 from .. import tensors, var
 from ..config import CTRL, NCTRL
+from ..future import cached_property
 from ..paulialgebra import Pauli, sZ
 from ..qubits import Qubit
 from ..tensors import QubitTensor
-from ..utils import cached_property
 from ..var import Variable
 from .stdgates import StdGate
 
 __all__ = ("CPhase", "CPhase00", "CPhase01", "CPhase10", "PSwap")
 
 
 class CPhase(StdGate):
@@ -50,15 +50,15 @@
             [0, 0, 1.0, 0],
             [0, 0, 0, np.exp(1j * theta)],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "CPhase":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CPhase":
         theta = self.param("theta") * t
         return CPhase(theta, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return [CTRL, "P({theta})"]
@@ -94,15 +94,15 @@
             [0, 0, 1.0, 0],
             [0, 0, 0, 1.0],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "CPhase00":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CPhase00":
         theta = self.param("theta")
         return CPhase00(theta * t, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return [NCTRL + "({theta})", NCTRL + "({theta})"]
@@ -135,15 +135,15 @@
             [0, 0, 1.0, 0],
             [0, 0, 0, 1.0],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "CPhase01":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CPhase01":
         theta = self.param("theta")
         return CPhase01(theta * t, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return [NCTRL + "({theta})", CTRL + "({theta})"]
@@ -177,15 +177,15 @@
             [0, 0, np.exp(1j * var.asfloat(self.param("theta"))), 0],
             [0, 0, 0, 1.0],
         ]
         return tensors.asqutensor(unitary)
 
     @property
     def H(self) -> "CPhase10":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CPhase10":
         theta = self.param("theta")
         return CPhase10(theta * t, *self.qubits)
 
     def _diagram_labels_(self) -> List[str]:
         return [CTRL + "({theta})", NCTRL + "({theta})"]
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_forest_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_forest_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_qasm.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_qasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 
 from typing import List
 
 import numpy as np
 
 from .. import tensors
 from ..config import CTRL
+from ..future import cached_property
 from ..qubits import Qubit
 from ..tensors import QubitTensor
-from ..utils import cached_property
 from ..var import Variable
 from .stdgates import StdCtrlGate, StdGate
 from .stdgates_1q import PhaseShift, Rx, Ry, Rz
 from .stdgates_2q import XX, YY, ZZ, CNot
 from .stdgates_forest import CPhase
 
 __all__ = ("U3", "U2", "CU3", "CRZ", "RZZ", "CRx", "CRy", "CRz", "Rxx", "Ryy", "Rzz")
@@ -258,15 +258,15 @@
     cv_target = Rx
 
     def __init__(self, theta: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[theta], qubits=[q0, q1])
 
     @property
     def H(self) -> "CRx":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CRx":
         theta = self.param("theta")
         return CRx(theta * t, *self.qubits)
 
 
 # end class CRx
@@ -277,15 +277,15 @@
     cv_target = Ry
 
     def __init__(self, theta: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[theta], qubits=[q0, q1])
 
     @property
     def H(self) -> "CRy":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CRy":
         theta = self.param("theta")
         return CRy(theta * t, *self.qubits)
 
 
 # end class CRy
@@ -297,15 +297,15 @@
     cv_tensor_structure = "diagonal"
 
     def __init__(self, theta: Variable, q0: Qubit, q1: Qubit) -> None:
         super().__init__(params=[theta], qubits=[q0, q1])
 
     @property
     def H(self) -> "CRz":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, t: Variable) -> "CRz":
         theta = self.param("theta")
         return CRz(theta * t, *self.qubits)
 
 
 # end class CRz
@@ -329,15 +329,15 @@
     def tensor(self) -> QubitTensor:
         q0, q1 = self.qubits
         (theta,) = self.params
         return XX(theta / np.pi, q0, q1).tensor
 
     @property
     def H(self) -> "Rxx":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "Rxx":
         (theta,) = self.params
         return Rxx(theta * e, *self.qubits)
 
 
 # end class Ryy
@@ -357,15 +357,15 @@
     def tensor(self) -> QubitTensor:
         q0, q1 = self.qubits
         (theta,) = self.params
         return YY(theta / np.pi, q0, q1).tensor
 
     @property
     def H(self) -> "Ryy":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "Ryy":
         (theta,) = self.params
         return Ryy(theta * e, *self.qubits)
 
 
 # end class Rxx
@@ -387,15 +387,15 @@
     def tensor(self) -> QubitTensor:
         q0, q1 = self.qubits
         (theta,) = self.params
         return ZZ(theta / np.pi, q0, q1).tensor
 
     @property
     def H(self) -> "Rzz":
-        return self ** -1
+        return self**-1
 
     def __pow__(self, e: Variable) -> "Rzz":
         (theta,) = self.params
         return Rzz(theta * e, *self.qubits)
 
 
 # end class Rzz
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_qasm_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_qasm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,24 +63,24 @@
     theta = 0.23
     gate0 = qf.CRZ(theta, 0, 1)
     coords = qf.canonical_coords(gate0)
     assert np.isclose(coords[0], 0.5 * theta / np.pi)
     assert np.isclose(coords[1], 0.0)
     assert np.isclose(coords[2], 0.0)
 
-    coords = qf.canonical_coords(gate0 ** 3.3)
+    coords = qf.canonical_coords(gate0**3.3)
     assert np.isclose(coords[0], 3.3 * 0.5 * theta / np.pi)
 
     gate1 = qf.Circuit([qf.CRZ(theta, 0, 1), qf.CRZ(theta, 0, 1).H]).asgate()
     assert qf.almost_identity(gate1)
 
 
 def test_RZZ() -> None:
     theta = 0.23
     gate0 = qf.RZZ(theta, 0, 1)
     gate1 = qf.ZZ(theta / np.pi, 0, 1)
     assert qf.gates_close(gate0, gate1)
     assert qf.gates_close(gate0.H, gate1.H)
-    assert qf.gates_close(gate0 ** 0.12, gate1 ** 0.12)
+    assert qf.gates_close(gate0**0.12, gate1**0.12)
 
 
 # fin
```

### Comparing `quantumflow-1.2.1/quantumflow/stdgates/stdgates_test.py` & `quantumflow-1.3.0/quantumflow/stdgates/stdgates_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2020-, Gavin E. Crooks and contributors
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 import random
 from itertools import chain
-from typing import Type
+from typing import Optional, Type
 
 import numpy as np
 import pytest
 
 import quantumflow as qf
 from quantumflow.visualization import kwarg_to_symbol
 
@@ -51,25 +51,23 @@
 
     g2 = qf.CNot(0, 1)
     assert repr(g2) == "CNot(0, 1)"
 
 
 @pytest.mark.parametrize("gatet", qf.STDGATES.values())
 def test_stdgates_repr(gatet: Type[qf.StdGate]) -> None:
-
     gate0 = _randomize_gate(gatet)
     rep = repr(gate0)
     gate1 = eval(rep, dict(qf.STDGATES))
     assert type(gate0) == type(gate1)
     assert qf.gates_close(gate0, gate1)
 
 
 @pytest.mark.parametrize("gatet", qf.STDGATES.values())
 def test_stdgates(gatet: Type[qf.StdGate]) -> None:
-
     # Test creation
     gate = _randomize_gate(gatet)
 
     # Test correct number of qubits
     assert gate.qubit_nb == gatet.cv_qubit_nb
 
     # Test hermitian conjugate
@@ -79,30 +77,30 @@
 
     # Test inverse
     eye = gate @ inv_gate
     assert qf.gates_close(qf.IdentityGate(range(gate.qubit_nb)), eye)
     assert qf.gates_phase_close(qf.IdentityGate(range(gate.qubit_nb)), eye)
 
     # Test pow
-    assert qf.gates_close(gate ** -1, inv_gate)
-    assert qf.gates_close((gate ** 0.5) ** 2, gate)
-    assert qf.gates_close((gate ** 0.3) @ (gate ** 0.7), gate)
+    assert qf.gates_close(gate**-1, inv_gate)
+    assert qf.gates_close((gate**0.5) ** 2, gate)
+    assert qf.gates_close((gate**0.3) @ (gate**0.7), gate)
 
-    hgate = qf.Unitary((gate ** 0.5).tensor, gate.qubits)
+    hgate = qf.Unitary((gate**0.5).tensor, gate.qubits)
     assert qf.gates_close(hgate @ hgate, gate)
 
 
-def _tensor_structure(tensor: qf.QubitTensor) -> "str":
+def _tensor_structure(tensor: qf.QubitTensor) -> Optional["str"]:
     # "identity", "diagonal", "permutation", "monomial"
     # TODO: Swap
 
     N = np.ndim(tensor) // 2
-    M = np.reshape(tensor, (2 ** N, 2 ** N))
+    M = np.reshape(tensor, (2**N, 2**N))
 
-    if np.all(M == np.eye(2 ** N)):
+    if np.all(M == np.eye(2**N)):
         return "identity"
 
     if np.all(M == np.diag(np.diagonal(M))):
         return "diagonal"
 
     if (
         (M.sum(axis=0) == 1).all()
@@ -118,15 +116,14 @@
         return "monomial"
 
     return None
 
 
 @pytest.mark.parametrize("gatet", qf.STDGATES.values())
 def test_tensor_properties(gatet: Type[qf.StdGate]) -> None:
-
     gate = _randomize_gate(gatet)
 
     assert qf.almost_unitary(gate)
 
     if gatet.cv_hermitian:
         assert gate is gate.H
         assert qf.almost_hermitian(gate)
@@ -142,15 +139,14 @@
         random.shuffle(qbs)
         perm_gate = gate.on(*qbs)
         assert qf.gates_close(gate, perm_gate)
 
 
 @pytest.mark.parametrize("gatet", qf.STDGATES.values())
 def test_hamiltonians(gatet: Type[qf.StdGate]) -> None:
-
     gate0 = _randomize_gate(gatet)
 
     qbs = gate0.qubits
     ham = gate0.hamiltonian
 
     gate1 = qf.UnitaryGate.from_hamiltonian(ham, qbs)
 
@@ -158,20 +154,21 @@
     assert qf.gates_phase_close(gate0, gate1)
 
 
 @pytest.mark.parametrize("gatet", qf.STDGATES.values())
 def test_symbolic(gatet: Type[qf.StdGate]) -> None:
     if len(gatet.cv_args) == 0:
         return
+
     args = {kwarg_to_symbol[arg]: random.uniform(-4, 4) for arg in gatet.cv_args}
     qbs = range(gatet.cv_qubit_nb)
 
     # Make gate with symbols
-    gate0 = gatet(*chain(args, qbs))
-    gate1 = gate0.resolve(subs=args)
+    gate0 = gatet(*args.values(), *qbs)  # type: ignore
+    gate1 = gate0.resolve(subs=args)  # type: ignore
     gate2 = gatet(*args.values(), *qbs)  # type: ignore
     assert isinstance(gate1, qf.StdGate)
     assert qf.gates_close(gate1, gate2)
 
     # Arguments with symbolic constants should be converted to float before
     # creating tensor
     gate0 = gatet(*chain(([qf.PI] * len(args)), qbs))
```

### Comparing `quantumflow-1.2.1/quantumflow/stdops.py` & `quantumflow-1.3.0/quantumflow/stdops.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,27 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Hashable,
     Iterator,
     List,
+    Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 import numpy as np
 
-from . import tensors, utils
+from . import tensors
 from .circuits import Circuit
 from .config import CIRCUIT_INDENT
+from .future import cached_property
 from .ops import _EXCLUDED_OPERATIONS, Channel, Gate, Operation, Unitary
 from .qubits import Qubit, Qubits, sorted_qubits
 from .states import Density, State
 from .tensors import QubitTensor
 from .var import Variable
 
 __all__ = [
@@ -78,15 +80,15 @@
 
 class Moment(Sequence, Operation):
     """
     Represents a collection of Operations that operate on disjoint qubits,
     so that they may be applied at the same moment of time.
     """
 
-    def __init__(self, *elements: Operation, qubits: Qubits = None) -> None:
+    def __init__(self, *elements: Operation, qubits: Optional[Qubits] = None) -> None:
         circ = Circuit(Circuit(elements).flat(), qubits=qubits)  # type: ignore
 
         qbs = list(q for elem in circ for q in elem.qubits)
         if len(qbs) != len(set(qbs)):
             raise ValueError("Qubits of operations within Moments must be disjoint.")
 
         super().__init__(qubits=circ.qubits)
@@ -97,18 +99,18 @@
 
     def __len__(self) -> int:
         return self._circ.__len__()
 
     def __iter__(self) -> Iterator[Operation]:
         yield from self._circ
 
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         return self._circ.run(ket)
 
-    def evolve(self, rho: Density = None) -> Density:
+    def evolve(self, rho: Optional[Density] = None) -> Density:
         return self._circ.evolve(rho)
 
     def asgate(self) -> "Gate":
         return self._circ.asgate()
 
     def aschannel(self) -> "Channel":
         return self._circ.aschannel()
@@ -138,15 +140,15 @@
 
 # end class Moment
 
 
 class Measure(Operation):
     """Measure a quantum bit and copy result to a classical bit"""
 
-    def __init__(self, qubit: Qubit, cbit: Hashable = None) -> None:
+    def __init__(self, qubit: Qubit, cbit: Optional[Hashable] = None) -> None:
         if cbit is None:
             cbit = qubit
 
         super().__init__(qubits=[qubit])
         self.qubit = qubit
         self.cbit = cbit
 
@@ -237,15 +239,15 @@
     """An operation that initializes the quantum state"""
 
     def __init__(self, ket: State):
         self._ket = ket
         self._qubits = ket.qubits  # FIXME
         super().__init__(ket.qubits)
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return self._ket.tensor
 
     def run(self, ket: State) -> State:
         return self._ket.permute(ket.qubits)
 
     def evolve(self, rho: Density) -> Density:
@@ -307,14 +309,15 @@
     @property
     def H(self) -> "Projection":
         return self  # pragma: no cover  # TESTME
 
 
 # end class Projection
 
+
 # FIXME: no zero qubit ops?
 class Store(Operation):
     """Store a value in the classical memory of the state."""
 
     def __init__(self, key: Hashable, value: Any, qubits: Qubits = ()) -> None:
         super().__init__(qubits=qubits)
         self.key = key
@@ -437,28 +440,28 @@
         return self.circuit.qubits
 
     @property
     def tensor(self) -> QubitTensor:
         raise NotImplementedError()
 
     @abstractmethod
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         raise NotImplementedError()
 
 
 # end class Simulator
 
 
 class QFSimulator(Simulator):
     """Our standard QuantumnFlow quantum circuit simulator as a Simulator subclass."""
 
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         return self.circuit.run(ket)
 
-    def evolve(self, rho: Density = None) -> Density:
+    def evolve(self, rho: Optional[Density] = None) -> Density:
         return self.circuit.evolve(rho)
 
 
 # end class QFSimulator
 
 
 class Project0(Gate):
@@ -467,15 +470,15 @@
     A non-unitary operation that represents the effect of a measurement. The norm
     of the resultant state is multiplied by the probability of observing 0.
     """
 
     def __init__(self, q0: Qubit = 0) -> None:
         super().__init__(qubits=[q0])
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return tensors.asqutensor([[1, 0], [0, 0]])
 
     def _diagram_labels_(self) -> List[str]:
         return ["|0⟩⟨0|"]
 
 
@@ -485,15 +488,15 @@
     A non-unitary operation that represents the effect of a measurement. The norm
     of the resultant state is multiplied by the probability of observing 1.
     """
 
     def __init__(self, q0: Qubit = 0) -> None:
         super().__init__(qubits=[q0])
 
-    @utils.cached_property
+    @cached_property
     def tensor(self) -> QubitTensor:
         return tensors.asqutensor([[0, 0], [0, 1]])
 
     def _diagram_labels_(self) -> List[str]:
         return ["|1⟩⟨1|"]
```

### Comparing `quantumflow-1.2.1/quantumflow/stdops_test.py` & `quantumflow-1.3.0/quantumflow/stdops_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/tensors.py` & `quantumflow-1.3.0/quantumflow/tensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 # DOCME
 
 import string
-from typing import TYPE_CHECKING, List, Sequence, Tuple
+from typing import TYPE_CHECKING, List, Optional, Sequence, Tuple
 
 import numpy as np
 
+from .future import TypeAlias
+
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike  # pragma: no cover
 
 
 __all__ = ("QubitTensor", "asqutensor")
 
 
-qubit_dtype = np.complex128
+qubit_dtype: TypeAlias = np.complex128
 """The complex data type used by the backend"""
 
-QubitTensor = np.ndarray
+QubitTensor: TypeAlias = np.ndarray
 """Type hint for numpy arrays representing quantum data.
 QubitTensor arrays have complex data type, and all axes have length 2."""
 
 
 def asqutensor(array: "ArrayLike") -> QubitTensor:
     """Converts a tensor like object to a numpy array object with complex data
     type, and reshapes to [2]*N (So the number of elements must be a power of 2)
@@ -44,18 +46,18 @@
 """Subscripts that can be used with numpy's einsum"""
 
 
 def flatten(tensor: QubitTensor, rank: int) -> np.ndarray:
     """Return tensor with with qubit indices flattened"""
     R = rank
     N = np.ndim(tensor) // R
-    return np.reshape(tensor, [2 ** N] * R)
+    return np.reshape(tensor, [2**N] * R)
 
 
-def transpose(tensor: QubitTensor, perm: Sequence[int] = None) -> QubitTensor:
+def transpose(tensor: QubitTensor, perm: Optional[Sequence[int]] = None) -> QubitTensor:
     """(Super)-operator transpose. Permutes the meta-indices.
     Default is to invert the meta-index order.
     """
     R = len(perm) if perm is not None else 2
     tensor = flatten(tensor, R)
     tensor = np.transpose(tensor, perm)
     tensor = asqutensor(tensor)
@@ -98,15 +100,15 @@
 
     tensor = np.outer(tensor0, tensor1)
 
     # Interleave meta axes
     # R = 1  perm = (0, 1)
     # R = 2  perm = (0, 2, 1, 3)
     # R = 4  perm = (0, 4, 1, 5, 2, 6, 3, 7)
-    tensor = np.reshape(tensor, ([2 ** N0] * R) + ([2 ** N1] * R))
+    tensor = np.reshape(tensor, ([2**N0] * R) + ([2**N1] * R))
     perm = [idx for ij in zip(range(0, R), range(R, 2 * R)) for idx in ij]
     if R != 1:
         tensor = transpose(tensor, perm)
 
     return tensor
 
 
@@ -177,22 +179,22 @@
 def tensormul(
     tensor0: QubitTensor, tensor1: QubitTensor, indices: Tuple[int, ...]
 ) -> QubitTensor:
     N = np.ndim(tensor1)
     K = np.ndim(tensor0) // 2
     assert K == len(indices)
 
-    gate = np.reshape(tensor0, [2 ** K, 2 ** K])
+    gate = np.reshape(tensor0, [2**K, 2**K])
 
     perm = list(indices) + [n for n in range(N) if n not in indices]
     inv_perm = np.argsort(perm)
 
     tensor = tensor1
     tensor = np.transpose(tensor, perm)
-    tensor = np.reshape(tensor, [2 ** K, 2 ** (N - K)])
+    tensor = np.reshape(tensor, [2**K, 2 ** (N - K)])
 
     tensor = np.matmul(gate, tensor)
 
     tensor = np.reshape(tensor, [2] * N)
     tensor = np.transpose(tensor, inv_perm)
 
     return tensor
@@ -209,15 +211,15 @@
     assert K == len(indices)
 
     perm = list(indices) + [n for n in range(N) if n not in indices]
     inv_perm = np.argsort(perm)
 
     tensor = tensor1
     tensor = np.transpose(tensor, perm)
-    tensor = np.reshape(tensor, [2 ** K, 2 ** (N - K)])
+    tensor = np.reshape(tensor, [2**K, 2 ** (N - K)])
 
     tensor = np.transpose(tensor)
     tensor = tensor * tensor0_diagonal.flatten()
     tensor = np.transpose(tensor)
 
     tensor = np.reshape(tensor, [2] * N)
     tensor = np.transpose(tensor, inv_perm)
```

### Comparing `quantumflow-1.2.1/quantumflow/tensors_test.py` & `quantumflow-1.3.0/quantumflow/tensors_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/transform.py` & `quantumflow-1.3.0/quantumflow/transform.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/transform_test.py` & `quantumflow-1.3.0/quantumflow/transform_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/translate/__init__.py` & `quantumflow-1.3.0/quantumflow/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/translate/translate_gates.py` & `quantumflow-1.3.0/quantumflow/translate/translate_gates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2019-, Gavin E. Crooks and the QuantumFlow contributors
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 
-from typing import Iterator, Union
+from typing import Iterator, Optional, Union
 
 import networkx as nx
 import numpy as np
 from networkx.algorithms.approximation.steinertree import steiner_tree
 from sympy.combinatorics import Permutation
 
 from ..circuits import Circuit
@@ -86,22 +86,21 @@
             q1 = qubits[n1]
             yield CZ(q1, q0) ** (1 / 2 ** (n1 - n0))
     yield from translate_ReversalGate_to_swap_network(ReversalGate(qubits))
 
 
 @register_translation
 def translate_InvQFTGate(gate: InvQFTGate) -> Iterator[Union[H, CZPow, Swap]]:
-
     gates = list(translate_QFTGate(QFTGate(gate.qubits)))
     yield from (gate.H for gate in gates[::-1])
 
 
 @register_translation
 def translate_PauliGate(
-    gate: PauliGate, topology: nx.Graph = None
+    gate: PauliGate, topology: Optional[nx.Graph] = None
 ) -> Iterator[Union[CNot, XPow, YPow, ZPow]]:
     """
     Yields a circuit corresponding to the exponential of
     the Pauli algebra element object, i.e. exp[-1.0j * alpha * element]
 
     If a qubit topology is provided then the returned circuit will
     respect the qubit connectivity, adding swaps as necessary.
```

### Comparing `quantumflow-1.2.1/quantumflow/translate/translate_stdgates_1q.py` & `quantumflow-1.3.0/quantumflow/translate/translate_stdgates_1q.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/translate/translate_stdgates_2q.py` & `quantumflow-1.3.0/quantumflow/translate/translate_stdgates_2q.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     yield H(q1)
     yield CZ(q0, q1)
     yield H(q1)
 
 
 @register_translation
 def translate_cnot_to_sqrtiswap(gate: CNot) -> Iterator[Union[SqrtISwap_H, X, S_H, H]]:
-    """Translate an ECP gate to a square-root-iswap sandwich"""
+    """Translate a CNOT gate to a square-root-iswap sandwich"""
     q0, q1 = gate.qubits
 
     # TODO: simplify 1-qubit gates
     yield H(q1)
     yield S_H(q0)
     yield S_H(q1)
     yield H(q0)
@@ -323,27 +323,27 @@
 ) -> Iterator[Union[XX, XPow, YPow, X]]:
     """Translate a cross resonance gate to an XX based circuit"""
     s, b, c = gate.params
     q0, q1 = gate.qubits
 
     t7 = (
         var.arccos(
-            ((1 + b ** 2 * var.cos(var.PI * var.sqrt(1 + b ** 2) * s))) / (1 + b ** 2)
+            ((1 + b**2 * var.cos(var.PI * var.sqrt(1 + b**2) * s))) / (1 + b**2)
         )
         / var.PI
     )
     t4 = c * s
     t1 = (
         var.arccos(
-            var.cos(0.5 * var.PI * var.sqrt(1 + b ** 2) * s) / var.cos(t7 * var.PI / 2)
+            var.cos(0.5 * var.PI * var.sqrt(1 + b**2) * s) / var.cos(t7 * var.PI / 2)
         )
         / var.PI
     )
 
-    a = var.sin(var.PI * var.sqrt(1 + b ** 2) * s / 2)
+    a = var.sin(var.PI * var.sqrt(1 + b**2) * s / 2)
     t7 *= var.sign(a) * var.sign(b)
     t1 *= var.sign(a)
 
     yield XPow(t1, q0)
     yield YPow(1.5, q0)
     yield X(q0)
     yield XPow(t4, q1)
@@ -623,15 +623,15 @@
     """Translate iswap gate to square-root iswaps"""
     q0, q1 = gate.qubits
     yield SqrtISwap(q0, q1)
     yield SqrtISwap(q0, q1)
 
 
 @register_translation
-def translate_iswap_to_xy(gate: ISwap) -> Iterator[Union[XY]]:
+def translate_iswap_to_xy(gate: ISwap) -> Iterator[XY]:
     """Convert ISwap gate to a XY gate."""
     q0, q1 = gate.qubits
     yield XY(-0.5, q0, q1)
 
 
 @register_translation
 def translate_pswap_to_canonical(gate: PSwap) -> Iterator[Union[Can, Y]]:
@@ -642,31 +642,31 @@
     t = 0.5 - theta / var.PI
     yield Y(q0)
     yield Can(0.5, 0.5, t, q0, q1)
     yield Y(q1)
 
 
 @register_translation
-def translate_rxx_to_xx(gate: Rxx) -> Iterator[Union[XX]]:
+def translate_rxx_to_xx(gate: Rxx) -> Iterator[XX]:
     """Translate QASM's RXX gate to standard gates"""
     q0, q1 = gate.qubits
     (theta,) = gate.params
     yield XX(theta / var.PI, q0, q1)
 
 
 @register_translation
-def translate_ryy_to_yy(gate: Ryy) -> Iterator[Union[YY]]:
+def translate_ryy_to_yy(gate: Ryy) -> Iterator[YY]:
     """Translate QASM's RYY gate to standard gates"""
     q0, q1 = gate.qubits
     (theta,) = gate.params
     yield YY(theta / var.PI, q0, q1)
 
 
 @register_translation
-def translate_rzz_to_zz(gate: Rzz) -> Iterator[Union[ZZ]]:
+def translate_rzz_to_zz(gate: Rzz) -> Iterator[ZZ]:
     """Translate QASM's RZZ gate to standard gates"""
     q0, q1 = gate.qubits
     (theta,) = gate.params
     yield ZZ(theta / var.PI, q0, q1)
 
 
 @register_translation
@@ -834,15 +834,15 @@
     yield CNot(q0, q1)
     yield CH(q0, q1)
     yield CNot(q0, q1)
     yield CNot(q1, q0)
 
 
 @register_translation
-def translate_xx_to_can(gate: XX) -> Iterator[Union[Can]]:
+def translate_xx_to_can(gate: XX) -> Iterator[Can]:
     """Convert an XX gate to a canonical circuit."""
     q0, q1 = gate.qubits
     t = gate.param("t")
     yield Can(t, 0, 0, q0, q1)
 
 
 @register_translation
@@ -882,15 +882,15 @@
     yield ZPow(t, q1)
     yield SqrtISwap_H(q0, q1)
     yield T_H(q0)
     yield T(q1)
 
 
 @register_translation
-def translate_yy_to_can(gate: YY) -> Iterator[Union[Can]]:
+def translate_yy_to_can(gate: YY) -> Iterator[Can]:
     """Convert an YY gate to a canonical circuit."""
     q0, q1 = gate.qubits
     t = gate.param("t")
     yield Can(0, t, 0, q0, q1)
 
 
 @register_translation
@@ -902,15 +902,15 @@
     yield XPow(0.5, q1)
     yield ZZ(t, q0, q1)
     yield XPow(-0.5, q0)
     yield XPow(-0.5, q1)
 
 
 @register_translation
-def translate_zz_to_can(gate: ZZ) -> Iterator[Union[Can]]:
+def translate_zz_to_can(gate: ZZ) -> Iterator[Can]:
     """Convert an ZZ gate to a canonical circuit."""
     q0, q1 = gate.qubits
     t = gate.param("t")
     yield Can(0, 0, t, q0, q1)
 
 
 @register_translation
```

### Comparing `quantumflow-1.2.1/quantumflow/translate/translate_stdgates_3q.py` & `quantumflow-1.3.0/quantumflow/translate/translate_stdgates_3q.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/translate/translate_test.py` & `quantumflow-1.3.0/quantumflow/translate/translate_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,24 @@
 
 @pytest.mark.parametrize("trans", STD_TRANSLATIONS)  # type: ignore
 def test_std_gate_translators_symbolic(trans: Callable) -> None:
     """Check that translations can handle symbolic arguments"""
     gatet = translation_source_gate(trans)
     args = [kwarg_to_symbol[a] for a in gatet.cv_args]
     qbs = range(gatet.cv_qubit_nb)
-    gate = gatet(*chain(args, qbs))
+    gate = gatet(*chain(args, qbs))  # type: ignore
 
     qubits = "abcdefg"[0 : gate.qubit_nb]  # Check that qubits are preserved
     gate = gate.on(*qubits)
 
     circ0 = qf.Circuit([gate])
     circ1 = qf.Circuit(trans(gate))  # type: ignore
 
-    circ0f = circ0.resolve(concrete)
-    circ1f = circ1.resolve(concrete)
+    circ0f = circ0.resolve(concrete)  # type: ignore  # FIXME
+    circ1f = circ1.resolve(concrete)  # type: ignore  # FIXME
     assert qf.gates_close(circ0f.asgate(), circ1f.asgate())
 
 
 def test_translate() -> None:
     circ0 = qf.Circuit([qf.CSwap(0, 1, 2)])
 
     translators = [
```

### Comparing `quantumflow-1.2.1/quantumflow/translate/translations.py` & `quantumflow-1.3.0/quantumflow/translate/translations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2019-, Gavin E. Crooks and the QuantumFlow contributors
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 
-from typing import Callable, Iterable, List, Sequence, Tuple, Type
+from typing import Callable, Iterable, List, Optional, Sequence, Tuple, Type
 
 from ..circuits import Circuit
 from ..ops import Gate
 from ..stdgates import S_H, T_H, CNot, H, I, Ph, S, T, YPow, ZPow
 
 __all__ = [
     "TRANSLATIONS",
@@ -35,30 +35,30 @@
 
 
 def translation_source_gate(trans: Callable) -> Type[Gate]:
     return trans.__annotations__["gate"]
 
 
 def translation_target_gates(trans: Callable) -> Tuple[Type[Gate]]:
-
     try:
         ret = trans.__annotations__["return"].__args__[0]
     except KeyError:  # pragma: no cover   # FIXME
         raise ValueError("Translation missing return type annotation")
 
     if hasattr(ret, "__args__"):  # Union
         gates = ret.__args__
     else:
         gates = (ret,)
 
     return gates
 
 
 def select_translations(
-    target_gates: Iterable[Type[Gate]], translations: Iterable[Callable] = None
+    target_gates: Iterable[Type[Gate]],
+    translations: Optional[Iterable[Callable]] = None,
 ) -> List[Callable]:
     """Return a list of translations that will translate source gates to target
     gates.
 
     If no translations are specified, we use all QuantumFlow translations
     listed in qf.TRANSLATIONS
 
@@ -111,16 +111,16 @@
 
 # Deprecated
 select_translators = select_translations
 
 
 def circuit_translate(
     circ: Circuit,
-    translators: Sequence = None,
-    targets: Iterable[Type[Gate]] = None,
+    translators: Optional[Sequence] = None,
+    targets: Optional[Iterable[Type[Gate]]] = None,
     recurse: bool = True,
 ) -> Circuit:
     """Apply a collection of translations to each gate in a circuit.
     If recurse, then apply translations to output of translations
     until translationally invariant.
     """
     if translators is not None and targets is not None:
```

### Comparing `quantumflow-1.2.1/quantumflow/transpile.py` & `quantumflow-1.3.0/quantumflow/transpile.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     intermediate_form = _transpile_from(circuit)
     final_form = _transpile_to(intermediate_form, output_format)
 
     return final_form
 
 
 def _transpile_from(circuit: Any) -> Circuit:
-
     input_format = _guess_format(circuit)
 
     if input_format == "braket":
         from . import xbraket
 
         return xbraket.braket_to_circuit(circuit)
 
@@ -142,15 +141,14 @@
     if "qutip" in typestr and "QubitCircuit" in typestr:
         return "qutip"
 
     raise ValueError(f"Unknown source format for circuit: {typestr}")
 
 
 def _transpile_to(circuit: Circuit, output_format: str) -> Any:
-
     if output_format == "braket":
         from . import xbraket
 
         return xbraket.circuit_to_braket(circuit, translate=True)
 
     if output_format == "cirq":
         from . import xcirq
```

### Comparing `quantumflow-1.2.1/quantumflow/transpile_test.py` & `quantumflow-1.3.0/quantumflow/transpile_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 pytest.importorskip("qsimcirq")  # noqa: 402
 pytest.importorskip("braket")  # noqa: 402
 pytest.importorskip("cirq")  # noqa: 402
 pytest.importorskip("qiskit")  # noqa: 402
 
 
 def test_guess_format() -> None:
-
     circ = qf.Circuit(qf.X(0), qf.Z(1))
 
     c0 = xcirq.circuit_to_cirq(circ)
     f0 = _guess_format(c0)
     assert f0 == "cirq"
 
     c1 = xbraket.circuit_to_braket(circ)
@@ -55,25 +54,23 @@
     "qsim",
     "qutip",
 ]
 
 
 @pytest.mark.parametrize("circuit_format", circuit_formats)
 def test_transpile(circuit_format: str) -> None:
-
     circ0 = qf.Circuit(qf.X(0), qf.Z(1))
 
     circ1 = transpile(circ0, output_format=circuit_format)
     circ2 = transpile(circ1, output_format="quantumflow")
     assert qf.circuits_close(circ0, circ2)
 
 
 @pytest.mark.parametrize("circuit_format", circuit_formats)
 def test_transpile_translate(circuit_format: str) -> None:
-
     circ0 = qf.Circuit(
         qf.X(0), qf.Z(1), qf.Margolus(0, 1, 2), qf.Can(0.1, 0.2, 0.3, 2, 3)
     )
 
     circ1 = transpile(circ0, output_format=circuit_format)
     circ2 = transpile(circ1, output_format="quantumflow")
     assert qf.circuits_close(circ0, circ2)
@@ -95,14 +92,13 @@
 
     circ2 = transpile(circ1)
     assert qf.circuits_close(circ0, circ2)
     print(circ2)
 
 
 def test_transpile_errors() -> None:
-
     with pytest.raises(ValueError):
         _ = transpile(19939848)
 
     circ0 = qf.Circuit(qf.Margolus(0, 1, 2))
     with pytest.raises(ValueError):
         _ = transpile(circ0, output_format="NOT_A_FORMAT")
```

### Comparing `quantumflow-1.2.1/quantumflow/utils.py` & `quantumflow-1.3.0/quantumflow/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,17 @@
     TypeVar,
     Union,
 )
 
 import networkx as nx
 import numpy as np
 
+from .future import importlib_metadata  # noqa: F401  # Backwards compatibility
+
 __all__ = (
-    # Future
-    "importlib_metadata",
-    "cached_property",
-    "Protocol",
     "deprecated",
     # Collections
     "multi_slice",
     "invert_map",
     "FrozenDict",
     # Math
     "almost_integer",
@@ -50,54 +48,15 @@
     "to_graph6",
     "spanning_tree_count",
     "octagonal_tiling_graph",
     "truncated_grid_2d_graph",
 )
 
 
-# -- Future present --
-
-try:
-    # python >= 3.8
-    from importlib import metadata as importlib_metadata  # type: ignore
-except ImportError:  # pragma: no cover
-    # python == 3.7
-    import importlib_metadata  # type: ignore  # noqa: F401
-
-
-try:  # pragma: no cover
-    # Python >= 3.8
-    from functools import cached_property  # type: ignore
-except ImportError:  # pragma: no cover
-    # python == 3.7
-    def cached_property(func):  # type: ignore
-        """
-        Method decorator for immutable properties.
-        The result is cached on the first call.
-        """
-
-        def wrapper(instance):  # type: ignore
-            attr = "_cached_property_" + func.__name__
-            if hasattr(instance, attr):
-                return getattr(instance, attr)
-            result = func(instance)
-            setattr(instance, attr, result)
-            return result
-
-        return property(wrapper)
-
-
-try:
-    # python >= 3.8
-    from typing import Protocol  # type: ignore
-except ImportError:  # pragma: no cover
-    # python == 3.7
-    from typing_extensions import Protocol  # type: ignore  # noqa: F401
-
-
+# TODO: Replace with deprecated package?
 def deprecated(func: Callable) -> Callable:
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
     @wraps(func)
     def _new_func(*args: Any, **kwargs: Any) -> Any:
@@ -112,15 +71,17 @@
 
     return _new_func
 
 
 # -- Collections --
 
 
-def multi_slice(axes: Sequence, items: Sequence, axes_nb: int = None) -> Tuple:
+def multi_slice(
+    axes: Sequence, items: Sequence, axes_nb: Optional[int] = None
+) -> Tuple:
     """Construct a multidimensional slice to access array data.
     e.g. mydata[multi_slice([3,5], [1,2]))] is equivalent to
     mydata[:,:,:,1,:,2,...]
     """
 
     N = max(axes) + 1 if axes_nb is None else axes_nb
     slices: List[Any] = [slice(None)] * N
@@ -217,15 +178,15 @@
 
     out = 0
     for bit in bitlist:
         out = (out << 1) | bit
     return out
 
 
-def int_to_bitlist(x: int, pad: int = None) -> List[int]:
+def int_to_bitlist(x: int, pad: Optional[int] = None) -> List[int]:
     """Converts an integer to a binary sequence of bits.
 
     Pad prepends with sufficient zeros to ensures that the returned list
     contains at least this number of bits.
 
     >>> from quantumflow.utils import int_to_bitlist
     >>> int_to_bitlist(4, 4))
@@ -265,15 +226,15 @@
         4096,
         8192,
         10000,
     ]
 )
 
 
-def rationalize(flt: float, denominators: Set[int] = None) -> Fraction:
+def rationalize(flt: float, denominators: Optional[Set[int]] = None) -> Fraction:
     """Convert a floating point number to a Fraction with a small
     denominator.
 
     Args:
         flt:            A floating point number
         denominators:   Collection of standard denominators. Default is
             1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 16, 32, 64, 100, 128, 256, 512,
@@ -373,15 +334,15 @@
                 edges = edges + up
 
             for (x0, y0), (x1, y1) in edges:
                 grp.add_edge((m * 4 + x0, n * 4 + y0), (m * 4 + x1, n * 4 + y1))
     return grp
 
 
-def truncated_grid_2d_graph(m: int, n: int, t: int = None) -> nx.Graph:
+def truncated_grid_2d_graph(m: int, n: int, t: Optional[int] = None) -> nx.Graph:
     """Generate a rectangular grid graph (of width `m` and height `n`),
     with corners removed. It the truncation `t` is not given, then it
     is set to half the shortest side (rounded down)
 
     truncated_grid_graph(12, 11) returns the topology of Google's
     bristlecone chip.
     """
```

### Comparing `quantumflow-1.2.1/quantumflow/utils_test.py` & `quantumflow-1.3.0/quantumflow/utils_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,43 +6,14 @@
 import networkx as nx
 import numpy as np
 import pytest
 
 from quantumflow import utils
 
 
-def test_cached_property() -> None:
-    class Thing:
-        def __init__(self, value: int) -> None:
-            self.value = value
-
-        @utils.cached_property
-        def plus1(self) -> int:
-            return self.value + 1
-
-        @utils.cached_property
-        def plus2(self) -> int:
-            return self.value + 2
-
-    two = Thing(2)
-    assert two.plus1 == 2 + 1
-    assert two.plus1 == 2 + 1
-    assert two.plus2 == 2 + 2
-    assert two.plus1 == 2 + 1
-
-    ten = Thing(10)
-    assert ten.plus1 == 10 + 1
-    assert ten.plus1 == 10 + 1
-    assert ten.plus2 == 10 + 2
-    assert ten.plus2 == 10 + 2
-
-    assert two.plus1 == 2 + 1
-    assert two.plus2 == 2 + 2
-
-
 def test_deprecated() -> None:
     class Something:
         @utils.deprecated
         def some_thing(self) -> None:
             pass
 
     obj = Something()
```

### Comparing `quantumflow-1.2.1/quantumflow/var.py` & `quantumflow-1.3.0/quantumflow/var.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 # Copyright 2019-, Gavin E. Crooks and contributors
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 # DOCME
 
-from typing import Mapping, Union
+from typing import Mapping, Optional, Union
 
 import numpy as np
 import sympy
 
 from . import utils
 from .config import ATOL, RTOL
+from .future import TypeAlias
 
-__all__ = ("Variable", "PI")
+__all__ = ("Variable", "ComplexVariable", "PI")
 
 
 Symbol = sympy.Symbol
 """Class for symbols in symbolic expressions"""
 
 
-Variable = Union[float, sympy.Expr]
+Variable: TypeAlias = Union[float, sympy.Expr]
 """Type for parameters. Either a float, sympy.Symbol or sympy.Expr"""
 
+ComplexVariable: TypeAlias = Union[float, complex, sympy.Expr]
+"""Type for complex parameters. Either a float, complex, sympy.Symbol or sympy.Expr"""
+
 
 PI = sympy.pi
 """Symbolic constant pi"""
 
 
+# If confuses mypy, inline `isinstance(x, sympy.Expr)` directly.
 def is_symbolic(x: Variable) -> bool:
     """Returns true if a symbolic expression"""
     return isinstance(x, sympy.Expr)
 
 
-def isclose(x: Variable, y: Variable, atol: float = ATOL, rtol: float = RTOL) -> bool:
+def isclose(
+    x: ComplexVariable, y: ComplexVariable, atol: float = ATOL, rtol: float = RTOL
+) -> bool:
     """Compares two variables.
 
     Returns: True if variables are almost identical concrete numbers,
         of if they are the same symbolic expression, else False.
     """
-    if not is_symbolic(x) and not is_symbolic(y):
+    if not isinstance(x, sympy.Expr) and not isinstance(y, sympy.Expr):
         return bool(np.isclose(x, y, atol=atol, rtol=rtol))
-    if is_symbolic(x) and is_symbolic(y):
+    if isinstance(x, sympy.Expr) and isinstance(y, sympy.Expr):
         return x == y
     return False
 
 
 # DOCME # Testme
-def almost_zero(x: Variable, atol: float = ATOL) -> bool:
+def almost_zero(x: ComplexVariable, atol: float = ATOL) -> bool:
     """Is the variable symbolically zero, or numerically almost zero."""
     if x == sympy.S.Zero:
         return True
     return isclose(x, 0.0, atol=atol)
 
 
-def asfloat(x: Variable, subs: Mapping[str, float] = None) -> float:
+def asfloat(x: Variable, subs: Optional[Mapping[str, float]] = None) -> float:
     """Convert a variable to a float"""
     if is_symbolic(x) and subs:
         x = x.evalf(subs=subs)  # type: ignore
     return float(x)
 
 
 def asexpression(flt: float) -> sympy.Expr:
@@ -85,67 +92,67 @@
 
 
 # The following math functions act on Variables, and return symbolic expression if
 # the variable is symbolic, or numerical values if the variable is a number
 
 
 def arccos(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.acos(x)
     return np.arccos(x)
 
 
 def arcsin(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.asin(x)
     return np.arcsin(x)
 
 
 def arctan(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.atan(x)
     return np.arctan(x)
 
 
 def arctan2(x1: Variable, x2: Variable) -> Variable:
-    if is_symbolic(x1) or is_symbolic(x2):
+    if isinstance(x1, sympy.Expr) or isinstance(x2, sympy.Expr):
         return sympy.atan2(x1, x2)
     return np.arctan2(x1, x2)
 
 
 def cos(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.cos(x)
     return np.cos(x)
 
 
 def exp(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.exp(x)
     return np.exp(x)
 
 
 def sign(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.sign(x)
     return np.sign(x)
 
 
 def sin(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.sin(x)
     return np.sin(x)
 
 
 def sqrt(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.sqrt(x)
     return np.sqrt(x)
 
 
 def tan(x: Variable) -> Variable:
-    if is_symbolic(x):
+    if isinstance(x, sympy.Expr):
         return sympy.tan(x)
     return np.tan(x)
 
 
 # fin
```

### Comparing `quantumflow-1.2.1/quantumflow/var_test.py` & `quantumflow-1.3.0/quantumflow/var_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/visualization.py` & `quantumflow-1.3.0/quantumflow/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 QuantumFlow: Visualizations of quantum circuits,
 """
 
 import os
 import re
 import subprocess
 import tempfile
-from typing import Any, Dict, List, Sequence, TextIO
+from typing import Any, Dict, List, Optional, Sequence, TextIO
 
 import numpy as np
 import sympy
 from PIL import Image
 from sympy import Symbol
 
 from . import utils, var
@@ -132,22 +132,22 @@
 
     def _diagram_labels_(self) -> List[str]:
         return ["  "]
 
 
 def circuit_to_latex(
     circ: Circuit,
-    qubits: Qubits = None,
+    qubits: Optional[Qubits] = None,
     document: bool = True,
     package: str = "quantikz",
-    options: str = None,
+    options: Optional[str] = None,
     scale: float = 0.75,
     qubit_labels: bool = True,
-    left_labels: Sequence[str] = None,  # DOCME TESTME
-    right_labels: Sequence[str] = None,  # DOCME TESTME
+    left_labels: Optional[Sequence[str]] = None,  # DOCME TESTME
+    right_labels: Optional[Sequence[str]] = None,  # DOCME TESTME
 ) -> str:
     """
     Create an image of a quantum circuit in LaTeX.
 
 
     Args:
         circ:       A quantum Circuit
@@ -248,14 +248,15 @@
 
             if name not in LATEX_GATESET:
                 raise NotImplementedError(str(gate))
 
             pretty_params: Dict[str, str] = {}
             # FIXME: Do I need gate isinstance (Also below)
             if isinstance(elem, Gate) and elem.params:
+                assert gate.cv_args is not None  # FIXME
                 pretty_params = {
                     key: _pretty(value, format="latex")
                     for key, value in zip(gate.cv_args, elem.params)
                 }
 
             # Construct text labels
             name = elem.name
@@ -503,15 +504,15 @@
             ["pdftocairo", "-singlefile", "-png", "-q", tmppath + ".pdf", tmppath]
         )
         img = Image.open(tmppath + ".png")
 
     return img
 
 
-def circuit_to_image(circ: Circuit, qubits: Qubits = None) -> Image:
+def circuit_to_image(circ: Circuit, qubits: Optional[Qubits] = None) -> Image:
     """Create an image of a quantum circuit.
 
     A convenience function that calls circuit_to_latex() and latex_to_image().
 
     Args:
         circ:       A quantum Circuit
         qubits:     Optional qubit list to specify qubit order
@@ -526,15 +527,15 @@
     latex = circuit_to_latex(circ, qubits)
     img = latex_to_image(latex)
     return img
 
 
 def circuit_to_diagram(
     circ: Circuit,
-    qubits: Qubits = None,
+    qubits: Optional[Qubits] = None,
     use_unicode: bool = True,
     transpose: bool = False,
     qubit_labels: bool = True,
 ) -> str:
     """
     Draw a text diagram of a quantum circuit.
 
@@ -594,14 +595,15 @@
         for elem in layer:
             idx = [qubit_idx[q] for q in elem.qubits]
 
             # Pretty print parameters
             pretty_params: Dict[str, str] = {}
             params = elem.params
             if params:
+                assert elem.cv_args is not None  # FIXME
                 pretty_params = {
                     key: _pretty(value, format="text")
                     for key, value in zip(elem.cv_args, params)
                 }
 
             text_labels = elem._diagram_labels_()
 
@@ -759,15 +761,15 @@
 unicode_ascii.update(dict(zip(STD_BOX_CHARS, ASCII_BOX_CHARS)))
 
 
 def _unicode_to_ascii(text: str) -> str:
     return "".join(unicode_ascii.get(c, c) for c in text)
 
 
-def print_gate(gate: Gate, ndigits: int = 2, file: TextIO = None) -> None:
+def print_gate(gate: Gate, ndigits: int = 2, file: Optional[TextIO] = None) -> None:
     """Pretty print a gate tensor
 
     Args:
         gate:
         ndigits:
         file: Stream to which to write. Defaults to stdout
     """
```

### Comparing `quantumflow-1.2.1/quantumflow/visualization_test.py` & `quantumflow-1.3.0/quantumflow/visualization_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/xbraket.py` & `quantumflow-1.3.0/quantumflow/xbraket.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Interface between IBM's Qiskit and QuantumFlow
 
 .. autoclass:: QiskitSimulator
 .. autofunction:: qiskit_to_circuit
 .. autofunction:: circuit_to_qiskit
 """
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 import numpy as np
 
 from .circuits import Circuit
 from .gatesets import BRAKET_GATES
 from .states import State
 from .stdgates import STDGATES
@@ -164,15 +164,15 @@
 
 def translate_to_braket(circ: Circuit) -> Circuit:
     """Convert QF gates to gates understood by qiskit"""
     return circuit_translate(circ, targets=BRAKET_GATES)
 
 
 class BraketSimulator(Simulator):
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         try:
             from braket.devices import LocalSimulator
         except ModuleNotFoundError as err:  # pragma: no cover
             raise ModuleNotFoundError(_IMPORT_ERROR_MSG) from err
 
         if ket is not None:
             raise NotImplementedError("Initial ket not supported")
```

### Comparing `quantumflow-1.2.1/quantumflow/xbraket_test.py` & `quantumflow-1.3.0/quantumflow/xbraket_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     bkcirc = bkcirc.xx(0, 1, np.pi * 0.5)
     bkcirc = bkcirc.xy(0, 2, np.pi * 0.5)
     circ = braket_to_circuit(bkcirc)
     print(circ)
 
 
 def test_circuit_to_qiskit() -> None:
-
     circ = qf.Circuit([qf.CNot(0, 1), qf.Rz(0.2, 1)])
     bkcirc = circuit_to_braket(circ)
     print(bkcirc)
 
 
 def test_braketsimulator() -> None:
     circ = qf.Circuit()
```

### Comparing `quantumflow-1.2.1/quantumflow/xcirq.py` & `quantumflow-1.3.0/quantumflow/xcirq.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 .. autofunction:: to_cirq_qubit
 
 """
 
 # Conventions
 # cqc: Abbreviation for Cirq circuit
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 import numpy as np
 
 from . import var
 from .circuits import Circuit
 from .gatesets import CIRQ_GATES
 from .ops import Unitary
@@ -86,15 +86,15 @@
     results will not be as accurate.
     """
 
     def __init__(self, circ: Circuit) -> None:
         super().__init__(circ)
         self._cqc = circuit_to_cirq(self.circuit, translate=True)
 
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         try:
             import cirq
         except ModuleNotFoundError as err:  # pragma: no cover
             raise ModuleNotFoundError(_IMPORT_ERROR_MSG) from err
 
         if ket is None:
             qubits = self.qubits
```

### Comparing `quantumflow-1.2.1/quantumflow/xcirq_test.py` & `quantumflow-1.3.0/quantumflow/xcirq_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,28 +148,28 @@
     # gate = cirq_to_circuit(cq.Circuit(cq.IdentityGate(2).on(q0, q1)))[0]
 
     op = (cq.PhasedISwapPowGate() ** 0.5).on(q0, q1)
     circ = cirq_to_circuit(cq.Circuit(op))
     assert qf.gates_close(circ.asgate(), qf.Givens(0.5 * pi / 2, 0, 1))
 
     op = cq.PhasedXZGate(
-        x_exponent=0.125, z_exponent=0.25, axis_phase_exponent=0.375
+        x_exponent=0.125, z_exponent=0.25, axis_phase_exponent=0.375  # type: ignore
     ).on(q0)
     circ = cirq_to_circuit(cq.Circuit(op))
     assert len(circ) == 3
 
 
 def test_cirq_to_circuit2() -> None:
     import cirq as cq  # noqa: E402
 
     q0 = cq.GridQubit(0, 0)
     q1 = cq.GridQubit(1, 0)
 
     def basic_circuit(meas=False):  # type: ignore
-        sqrt_x = cq.X ** 0.5
+        sqrt_x = cq.X**0.5
         yield cq.X(q0) ** 0.5, sqrt_x(q1)
         yield cq.CZ(q0, q1)
         yield sqrt_x(q0), sqrt_x(q1)
         if meas:
             yield cq.measure(q0, key="q0"), cq.measure(q1, key="q1")
 
     cqc = cq.Circuit()
```

### Comparing `quantumflow-1.2.1/quantumflow/xforest.py` & `quantumflow-1.3.0/quantumflow/xforest.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/xforest_test.py` & `quantumflow-1.3.0/quantumflow/xforest_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/xqiskit.py` & `quantumflow-1.3.0/quantumflow/xqiskit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Note: Installation of qiskit is optional, so we defer import
 
 # Note that QASM specific gates are defined in quantumflow/stdgates/stdgates_qasm.py
 # since you might want to use those gates in QuantumFlow without loading
 # qiskit
 
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from .circuits import Circuit
 from .gatesets import QISKIT_GATES
 from .states import State
 from .stdgates import STDGATES
 from .stdops import If, Initialize, Simulator
 from .translate import circuit_translate
@@ -91,15 +91,15 @@
 """Map from qiskit operation names to QuantumFlow names"""
 
 
 # TODO: 'multiplexer', 'snapshot', 'unitary'
 
 
 class QiskitSimulator(Simulator):
-    def run(self, ket: State = None) -> State:
+    def run(self, ket: Optional[State] = None) -> State:
         try:
             import qiskit
         except ModuleNotFoundError as err:  # pragma: no cover
             raise ModuleNotFoundError(_IMPORT_ERROR_MSG) from err
 
         circ = self.circuit
         if ket is not None:
```

### Comparing `quantumflow-1.2.1/quantumflow/xqiskit_test.py` & `quantumflow-1.3.0/quantumflow/xqiskit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     qasm_to_circuit,
     qiskit_to_circuit,
     translate_to_qiskit,
 )
 
 
 def test_qiskit_to_circuit() -> None:
-
     q = QuantumRegister(5)
     c = ClassicalRegister(5)
     qc = QuantumCircuit(q, c)
 
     qc.ccx(q[0], q[1], q[2])
     qc.ch(q[0], q[1])
     qc.crz(0.1, q[0], q[1])
```

### Comparing `quantumflow-1.2.1/quantumflow/xqsim.py` & `quantumflow-1.3.0/quantumflow/xqsim.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 Interface to qsim
 
 https://github.com/quantumlib/qsim
 
 """
 
+from typing import Optional
+
 from .circuits import Circuit
 from .gatesets import QSIM_GATES
 from .states import State
 from .stdops import Simulator
 from .translate import circuit_translate
 from .xcirq import circuit_to_cirq
 
@@ -31,28 +33,26 @@
     """Interface to the qsim quantum simulator. Adapts a QF Circuit (or
     other sequence of Operations).
 
     Ref:
         https://github.com/quantumlib/qsim
     """
 
-    def __init__(self, circ: Circuit) -> None:
-
+    def __init__(self, circ: Circuit, translate: bool = True) -> None:
         try:
             import qsimcirq
         except ModuleNotFoundError as err:  # pragma: no cover
             raise ModuleNotFoundError(_IMPORT_ERROR_MSG) from err
 
         circ = translate_circuit_to_qsim(circ)
         super().__init__(circ)
         self._cirq = circuit_to_cirq(self.circuit)
         self._qsim_circuit = qsimcirq.QSimCircuit(self._cirq)
 
-    def run(self, ket: State = None) -> State:
-
+    def run(self, ket: Optional[State] = None) -> State:
         try:
             import qsimcirq
         except ModuleNotFoundError as err:  # pragma: no cover
             raise ModuleNotFoundError(_IMPORT_ERROR_MSG) from err
 
         if ket is not None:
             raise NotImplementedError("Not yet supported")
```

### Comparing `quantumflow-1.2.1/quantumflow/xqsim_test.py` & `quantumflow-1.3.0/quantumflow/xqsim_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/xquirk.py` & `quantumflow-1.3.0/quantumflow/xquirk.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow/xquirk_test.py` & `quantumflow-1.3.0/quantumflow/xquirk_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2019-, Gavin E. Crooks and the QuantumFlow contributors
 #
 # This source code is licensed under the Apache License, Version 2.0 found in
 # the LICENSE.txt file in the root directory of this source tree.
 
 import urllib
+import urllib.parse
 
 import pytest
 
 import quantumflow as qf
 from quantumflow.xquirk import circuit_to_quirk, quirk_url, translate_to_quirk
```

### Comparing `quantumflow-1.2.1/quantumflow/xqutip.py` & `quantumflow-1.3.0/quantumflow/xqutip.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 # CZ                Requires bugfix in QuTiP (Use CSIGN instead)
 # B                 Requires bugfix in QuTiP
 # swapalpha         Requires bugfix in QuTiP
 # molmer_sorensen   Gate defined but not supported by QuTiP's QubitCircuit
 # qrot
 # QASMU
 
-from typing import TYPE_CHECKING, Dict, Type, cast
+from typing import TYPE_CHECKING, Dict, Optional, Type, cast
 
 from . import var
 from .circuits import Circuit
 from .gatesets import QUTIP_GATES
 from .ops import Gate
 from .stdgates import (  # B,; Exch,
     CS,
@@ -110,15 +110,15 @@
 __all__ = ("qutip_to_circuit", "circuit_to_qutip", "translate_to_qutip", "QUTIP_GATES")
 
 
 _IMPORT_ERROR_MSG = """External dependency 'qutip' not installed. Install
 with 'pip install qutip'"""
 
 
-_QUTIP_GATE_NAMES: Dict[Type[Gate], str] = {
+_QUTIP_GATE_NAMES: Dict[Type[Gate], Optional[str]] = {
     I: None,
     Ph: "GLOBALPHASE",
     Rx: "RX",
     Ry: "RY",
     Rz: "RZ",
     V: "SQRTNOT",
     H: "SNOT",
```

### Comparing `quantumflow-1.2.1/quantumflow/xqutip_test.py` & `quantumflow-1.3.0/quantumflow/xqutip_test.py`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/quantumflow.egg-info/PKG-INFO` & `quantumflow-1.3.0/quantumflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: quantumflow
-Version: 1.2.1
+Version: 1.3.0
 Summary: "Cross compiler for gate based models of quantum computing"
 Home-page: https://github.com/gecrooks/quantumflow/
 Author: Gavin Crooks
 Author-email: gavincrooks@gmail.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: ext
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 #  QuantumFlow: A Quantum Algorithms Development Toolkit
@@ -57,9 +56,7 @@
 ```
 $ git clone https://github.com/gecrooks/quantumflow.git
 $ cd quantumflow
 $ pip install -e .[dev]
 ```
 
 
-
-
```

### Comparing `quantumflow-1.2.1/quantumflow.egg-info/SOURCES.txt` & `quantumflow-1.3.0/quantumflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .readthedocs.yml
 LICENSE
 Makefile
 README.md
 pyproject.toml
+pyrightconfig.json
 setup.cfg
 setup.py
 .github/workflows/python-build.yml
 .github/workflows/python-publish.yml
 docs/Makefile
 docs/bibtex.json
 docs/channels.rst
@@ -58,14 +59,16 @@
 quantumflow/config_test.py
 quantumflow/dagcircuit.py
 quantumflow/dagcircuit_test.py
 quantumflow/decompositions.py
 quantumflow/decompositions_test.py
 quantumflow/deprecated.py
 quantumflow/deprecated_test.py
+quantumflow/future.py
+quantumflow/future_test.py
 quantumflow/gates.py
 quantumflow/gates_test.py
 quantumflow/gatesets.py
 quantumflow/gradients.py
 quantumflow/gradients_test.py
 quantumflow/info.py
 quantumflow/info_test.py
```

### Comparing `quantumflow-1.2.1/quantumflow.egg-info/requires.txt` & `quantumflow-1.3.0/quantumflow.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,52 @@
+typing_extensions>=4.1.1
 numpy
-scipy
+scipy<1.10.0
 sympy>=1.6
 networkx
 decorator<5.0.0
 opt_einsum
-pillow
+pillow!=9.1.0
 matplotlib
 
 [:python_version < "3.8"]
 importlib_metadata
-typing_extensions
 
 [dev]
 cirq>=0.8.0
 qiskit>=0.24.0
 ruamel.yaml
 pyquil>=2.28.0
-qsimcirq
 qutip
 amazon-braket-sdk
 sphinx
 sphinxcontrib-bibtex
 guzzle-sphinx-theme
 setuptools_scm
 twine
 setupext-janitor
 numpy>=1.20
 pytest>=4.6
 pytest-cov
 flake8
-mypy
+mypy>=0.931
 black
 isort
 nbmake
 
+[dev:python_version < "3.11"]
+qsimcirq>=0.10.2
+
 [docs]
 sphinx
 sphinxcontrib-bibtex
 guzzle-sphinx-theme
 setuptools_scm
 
 [ext]
 cirq>=0.8.0
 qiskit>=0.24.0
 ruamel.yaml
 pyquil>=2.28.0
-qsimcirq
+qsimcirq>=0.10.2
 qutip
 amazon-braket-sdk
```

### Comparing `quantumflow-1.2.1/setup.cfg` & `quantumflow-1.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -14,73 +14,73 @@
 	License :: OSI Approved :: Apache Software License
 	Topic :: Scientific/Engineering
 	Programming Language :: Python
 	Natural Language :: English
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
 [options]
 zip_safe = True
-python_requires = >= 3.7
+python_requires = >= 3.9
 packages = find:
 install_requires = 
-	importlib_metadata      ; python_version < "3.8"   # PEP508 environment marker
-	typing_extensions       ; python_version < "3.8"   # PEP508 environment marker
+	importlib_metadata                  ; python_version < "3.8"   # PEP508 environment marker
+	typing_extensions       >= 4.1.1
 	numpy
-	scipy
+	scipy                   < 1.10.0    # v1.10 breaks tests
 	sympy                   >= 1.6
 	networkx
 	decorator               < 5.0.0     # 5.0 breaks networkx dependancy
 	opt_einsum
-	pillow
+	pillow                  != 9.1.0    # 9.1.0 has problems on some versions of MacOS
 	matplotlib
 setup_requires = 
 	setuptools_scm
 
 [options.extras_require]
 ext = 
 	cirq                    >= 0.8.0
 	qiskit                  >= 0.24.0
 	ruamel.yaml                         # Additional requirement for pyquil
 	pyquil                  >= 2.28.0
-	qsimcirq
+	qsimcirq                >= 0.10.2
 	qutip
 	amazon-braket-sdk
 docs = 
 	sphinx
 	sphinxcontrib-bibtex
 	guzzle-sphinx-theme
 	setuptools_scm
 dev = 
 	cirq                    >= 0.8.0
 	qiskit                  >= 0.24.0
-	ruamel.yaml
+	ruamel.yaml                         # Additional requirement for pyquil
 	pyquil                  >= 2.28.0
-	qsimcirq
+	qsimcirq                >= 0.10.2   ; python_version < "3.11"   # PEP508 environment marker
 	qutip
 	amazon-braket-sdk
 	
 	sphinx
 	sphinxcontrib-bibtex
 	guzzle-sphinx-theme
-	
 	setuptools_scm
 	twine
+	
 	setupext-janitor
 	
 	numpy                   >= 1.20     # Needed for numpy.typehints
 	pytest >= 4.6
 	pytest-cov
 	flake8
-	mypy
+	mypy                    >= 0.931
 	black
 	isort
 	nbmake                              # for testing notebooks
 
 [tool:pytest]
 testpaths = 
 	quantumflow
@@ -101,19 +101,20 @@
 	except ImportError
 	assert False
 	raise NotImplementedError()
 	pass
 
 [flake8]
 max-line-length = 88
-ignore = E203, W503     # Conform to black
+ignore = 
+	E203,
+	W503
 
 [mypy]
 files = quantumflow
 ignore_missing_imports = True
 disallow_untyped_defs = True
-strict_optional = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `quantumflow-1.2.1/tutorial/qf-tutorial-translate.ipynb` & `quantumflow-1.3.0/tutorial/qf-tutorial-translate.ipynb`

 * *Files identical despite different names*

### Comparing `quantumflow-1.2.1/tutorial/qf-tutorial-transpile.ipynb` & `quantumflow-1.3.0/tutorial/qf-tutorial-transpile.ipynb`

 * *Files identical despite different names*

