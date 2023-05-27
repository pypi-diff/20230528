# Comparing `tmp/haiku_geometric-0.0.3.tar.gz` & `tmp/haiku_geometric-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/haiku_geometric-0.0.3.tar", last modified: Wed Apr  5 20:42:02 2023, max compression
+gzip compressed data, was "haiku_geometric-0.0.4.tar", last modified: Sat May 27 23:26:54 2023, max compression
```

## Comparing `haiku_geometric-0.0.3.tar` & `haiku_geometric-0.0.4.tar`

### file list

```diff
@@ -1,132 +1,138 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/.github/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/.github/workflows/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1209 2023-04-05 20:20:14.000000 haiku_geometric-0.0.3/.github/workflows/python-app.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)     1799 2022-12-22 10:54:25.000000 haiku_geometric-0.0.3/.gitignore
--rw-r--r--   0 alex      (1000) alex      (1000)      625 2023-03-08 22:37:37.000000 haiku_geometric-0.0.3/.readthedocs.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)    10132 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     8703 2023-03-06 21:52:54.000000 haiku_geometric-0.0.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)      638 2022-12-24 12:48:33.000000 haiku_geometric-0.0.3/docs/Makefile
--rw-rw-r--   0 alex      (1000) alex      (1000)      804 2022-12-24 12:48:33.000000 haiku_geometric-0.0.3/docs/make.bat
--rw-r--r--   0 alex      (1000) alex      (1000)      333 2023-03-11 22:25:18.000000 haiku_geometric-0.0.3/docs/requirements.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/docs/source/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3762 2023-03-11 22:28:54.000000 haiku_geometric-0.0.3/docs/source/conf.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      882 2023-01-05 01:44:50.000000 haiku_geometric-0.0.3/docs/source/examples.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)     1606 2023-04-05 19:39:34.000000 haiku_geometric-0.0.3/docs/source/index.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/docs/source/modules/
--rw-rw-r--   0 alex      (1000) alex      (1000)      292 2023-01-05 00:30:58.000000 haiku_geometric-0.0.3/docs/source/modules/datasets.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-04-05 19:39:20.000000 haiku_geometric-0.0.3/docs/source/modules/models.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)     1697 2023-01-04 20:14:21.000000 haiku_geometric-0.0.3/docs/source/modules/nn.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)      381 2022-12-25 17:07:10.000000 haiku_geometric-0.0.3/docs/source/modules/transforms.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)      362 2023-02-24 23:07:17.000000 haiku_geometric-0.0.3/docs/source/modules/utils.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/docs/source/notebooks/
--rw-rw-r--   0 alex      (1000) alex      (1000)    11150 2023-01-08 14:14:57.000000 haiku_geometric-0.0.3/docs/source/notebooks/1_quickstart.ipynb
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/docs/source/notebooks/_static/
--rw-rw-r--   0 alex      (1000) alex      (1000)    20134 2023-01-04 23:21:17.000000 haiku_geometric-0.0.3/docs/source/notebooks/_static/graph1.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    19712 2023-01-04 23:34:05.000000 haiku_geometric-0.0.3/docs/source/notebooks/_static/graph2.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     7122 2023-01-05 15:30:15.000000 haiku_geometric-0.0.3/docs/source/notebooks/creating_dataset.ipynb
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/examples/
--rw-rw-r--   0 alex      (1000) alex      (1000)    11148 2023-01-08 14:04:48.000000 haiku_geometric-0.0.3/examples/1_quickstart.ipynb
--rw-rw-r--   0 alex      (1000) alex      (1000)    20118 2023-01-05 15:42:06.000000 haiku_geometric-0.0.3/examples/GATConv_CORA.ipynb
--rw-rw-r--   0 alex      (1000) alex      (1000)    15424 2023-01-05 15:41:27.000000 haiku_geometric-0.0.3/examples/GCNConv_karate_club.ipynb
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)      185 2023-02-22 22:48:24.000000 haiku_geometric-0.0.3/haiku_geometric/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/
--rw-rw-r--   0 alex      (1000) alex      (1000)      423 2023-01-05 00:20:36.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1738 2023-01-05 00:30:13.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/base.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6074 2023-01-01 22:55:10.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/gnn_benchmark_dataset.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3289 2023-01-01 22:08:25.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/karate_dataset.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3269 2023-01-01 22:54:48.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/ogb_dataset.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6253 2023-01-04 20:43:22.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/planetoid_dataset.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2761 2023-01-01 22:10:36.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/toy_dataset.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1330 2023-01-01 23:05:48.000000 haiku_geometric-0.0.3/haiku_geometric/datasets/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3552 2023-04-05 20:26:14.000000 haiku_geometric-0.0.3/haiku_geometric/models/MLP.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      104 2023-03-23 17:08:28.000000 haiku_geometric-0.0.3/haiku_geometric/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5111 2023-04-05 20:33:47.000000 haiku_geometric-0.0.3/haiku_geometric/models/node2vec.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/
--rw-rw-r--   0 alex      (1000) alex      (1000)      106 2022-12-31 16:03:36.000000 haiku_geometric-0.0.3/haiku_geometric/nn/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/
--rw-rw-r--   0 alex      (1000) alex      (1000)      380 2022-12-30 14:14:01.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      254 2022-12-22 17:22:33.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/base.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1972 2022-12-22 17:22:47.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/basic.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3841 2023-01-01 22:14:38.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/degree_scaler.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4042 2023-01-01 22:16:40.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/multi.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      677 2023-01-01 22:16:40.000000 haiku_geometric-0.0.3/haiku_geometric/nn/aggr/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/attention/
--rw-rw-r--   0 alex      (1000) alex      (1000)       96 2022-12-31 16:59:20.000000 haiku_geometric-0.0.3/haiku_geometric/nn/attention/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      849 2022-12-31 16:56:51.000000 haiku_geometric-0.0.3/haiku_geometric/nn/attention/self_attention.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/
--rw-rw-r--   0 alex      (1000) alex      (1000)      581 2022-12-31 16:46:59.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2174 2022-12-31 16:55:56.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7941 2023-03-06 00:12:14.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3445 2022-12-25 16:13:28.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gated_graph_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5599 2023-03-25 00:25:26.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9278 2023-03-06 00:15:29.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/general_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2385 2022-12-25 15:57:11.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3063 2023-01-01 22:16:40.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gine_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10081 2023-02-10 19:39:38.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/gps_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2591 2022-12-25 15:57:32.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/graph_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4904 2023-01-01 23:11:07.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/pna_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3981 2022-12-25 15:57:41.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/sage_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      679 2022-12-22 15:52:35.000000 haiku_geometric-0.0.3/haiku_geometric/nn/conv/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/dense/
--rw-rw-r--   0 alex      (1000) alex      (1000)       75 2022-12-24 16:28:03.000000 haiku_geometric-0.0.3/haiku_geometric/nn/dense/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1724 2023-01-01 22:16:40.000000 haiku_geometric-0.0.3/haiku_geometric/nn/dense/linear.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/nn/pool/
--rw-rw-r--   0 alex      (1000) alex      (1000)      179 2022-12-24 16:27:45.000000 haiku_geometric-0.0.3/haiku_geometric/nn/pool/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2022-12-22 15:54:37.000000 haiku_geometric-0.0.3/haiku_geometric/nn/pool/global_pool.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/transforms/
--rw-rw-r--   0 alex      (1000) alex      (1000)      241 2023-03-02 23:18:18.000000 haiku_geometric-0.0.3/haiku_geometric/transforms/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2930 2023-03-06 00:24:35.000000 haiku_geometric-0.0.3/haiku_geometric/transforms/add_self_loops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      335 2023-01-05 00:17:09.000000 haiku_geometric-0.0.3/haiku_geometric/transforms/normalize.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      380 2023-03-02 23:18:18.000000 haiku_geometric-0.0.3/haiku_geometric/transforms/remove_self_loops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)      470 2023-03-25 19:15:33.000000 haiku_geometric-0.0.3/haiku_geometric/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2863 2023-03-24 23:44:33.000000 haiku_geometric-0.0.3/haiku_geometric/utils/coalesce.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9781 2023-03-26 17:16:07.000000 haiku_geometric-0.0.3/haiku_geometric/utils/laplacian.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8853 2023-04-05 19:47:42.000000 haiku_geometric-0.0.3/haiku_geometric/utils/magnetic_laplacian.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4212 2023-04-05 18:43:45.000000 haiku_geometric-0.0.3/haiku_geometric/utils/random_walk.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1331 2023-03-24 23:41:24.000000 haiku_geometric-0.0.3/haiku_geometric/utils/undirected.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      671 2023-03-22 16:38:01.000000 haiku_geometric-0.0.3/haiku_geometric/utils/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    10132 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3327 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-01-01 22:48:42.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/haiku_geometric.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2023-03-25 01:42:52.000000 haiku_geometric-0.0.3/requirements.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      582 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)       37 2021-11-14 17:58:45.000000 haiku_geometric-0.0.3/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/datasets/
--rw-rw-r--   0 alex      (1000) alex      (1000)      295 2023-01-01 18:38:53.000000 haiku_geometric-0.0.3/test/datasets/test_karate.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      301 2023-01-04 20:47:28.000000 haiku_geometric-0.0.3/test/datasets/test_toy.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1482 2023-04-05 19:36:12.000000 haiku_geometric-0.0.3/test/models/test_Node2Vec.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:01.000000 haiku_geometric-0.0.3/test/nn/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/nn/aggr/
--rw-rw-r--   0 alex      (1000) alex      (1000)      922 2023-01-01 18:50:45.000000 haiku_geometric-0.0.3/test/nn/aggr/test_basic.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/nn/conv/
--rw-rw-r--   0 alex      (1000) alex      (1000)      723 2023-01-01 18:49:01.000000 haiku_geometric-0.0.3/test/nn/conv/test_EdgeConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1644 2023-01-01 18:51:28.000000 haiku_geometric-0.0.3/test/nn/conv/test_GCNConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      857 2023-01-01 18:49:44.000000 haiku_geometric-0.0.3/test/nn/conv/test_GINConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      946 2023-01-01 18:49:49.000000 haiku_geometric-0.0.3/test/nn/conv/test_GINEConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2117 2023-02-25 00:01:01.000000 haiku_geometric-0.0.3/test/nn/conv/test_GPSLayer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-01-01 18:49:24.000000 haiku_geometric-0.0.3/test/nn/conv/test_GatedGraphConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1592 2023-01-01 18:51:03.000000 haiku_geometric-0.0.3/test/nn/conv/test_GeneralConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1356 2023-01-01 18:50:20.000000 haiku_geometric-0.0.3/test/nn/conv/test_GraphConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2127 2023-01-01 18:55:57.000000 haiku_geometric-0.0.3/test/nn/conv/test_PNAConv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1115 2023-01-01 18:50:25.000000 haiku_geometric-0.0.3/test/nn/conv/test_SAGEConv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/nn/dense/
--rw-rw-r--   0 alex      (1000) alex      (1000)      690 2023-01-01 18:51:41.000000 haiku_geometric-0.0.3/test/nn/dense/test_linear.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/nn/pool/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2185 2023-01-01 18:51:58.000000 haiku_geometric-0.0.3/test/nn/pool/test_global.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-04-05 20:19:34.000000 haiku_geometric-0.0.3/test/requirements.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-05 20:42:02.000000 haiku_geometric-0.0.3/test/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)      760 2023-03-06 20:26:26.000000 haiku_geometric-0.0.3/test/utils/test_coalesce.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      835 2023-03-26 17:29:38.000000 haiku_geometric-0.0.3/test/utils/test_eigv_laplacian.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2915 2023-03-06 16:02:00.000000 haiku_geometric-0.0.3/test/utils/test_laplacian.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2942 2023-04-05 19:47:50.000000 haiku_geometric-0.0.3/test/utils/test_magnetic_laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.104675 haiku_geometric-0.0.4/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.072675 haiku_geometric-0.0.4/.github/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.076675 haiku_geometric-0.0.4/.github/workflows/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1209 2023-04-05 20:20:14.000000 haiku_geometric-0.0.4/.github/workflows/python-app.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1799 2022-12-22 10:54:25.000000 haiku_geometric-0.0.4/.gitignore
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2023-03-08 22:37:37.000000 haiku_geometric-0.0.4/.readthedocs.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11387 2023-05-27 23:26:54.104675 haiku_geometric-0.0.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9894 2023-05-27 23:18:20.000000 haiku_geometric-0.0.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      638 2022-12-24 12:48:33.000000 haiku_geometric-0.0.4/docs/Makefile
+-rw-rw-r--   0 alex      (1000) alex      (1000)      804 2022-12-24 12:48:33.000000 haiku_geometric-0.0.4/docs/make.bat
+-rw-r--r--   0 alex      (1000) alex      (1000)      343 2023-05-08 08:55:22.000000 haiku_geometric-0.0.4/docs/requirements.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/docs/source/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3762 2023-04-24 23:18:05.000000 haiku_geometric-0.0.4/docs/source/conf.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      882 2023-01-05 01:44:50.000000 haiku_geometric-0.0.4/docs/source/examples.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1652 2023-05-27 22:58:04.000000 haiku_geometric-0.0.4/docs/source/index.rst
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/docs/source/modules/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      292 2023-01-05 00:30:58.000000 haiku_geometric-0.0.4/docs/source/modules/datasets.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-04-05 19:39:20.000000 haiku_geometric-0.0.4/docs/source/modules/models.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1697 2023-01-04 20:14:21.000000 haiku_geometric-0.0.4/docs/source/modules/nn.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)      381 2022-12-25 17:07:10.000000 haiku_geometric-0.0.4/docs/source/modules/transforms.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)      362 2023-02-24 23:07:17.000000 haiku_geometric-0.0.4/docs/source/modules/utils.rst
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/docs/source/notebooks/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11150 2023-01-08 14:14:57.000000 haiku_geometric-0.0.4/docs/source/notebooks/1_quickstart.ipynb
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/docs/source/notebooks/_static/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20134 2023-01-04 23:21:17.000000 haiku_geometric-0.0.4/docs/source/notebooks/_static/graph1.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19712 2023-01-04 23:34:05.000000 haiku_geometric-0.0.4/docs/source/notebooks/_static/graph2.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7134 2023-05-27 19:23:56.000000 haiku_geometric-0.0.4/docs/source/notebooks/creating_dataset.ipynb
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.080675 haiku_geometric-0.0.4/examples/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11148 2023-01-08 14:04:48.000000 haiku_geometric-0.0.4/examples/1_quickstart.ipynb
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20125 2023-05-27 18:20:15.000000 haiku_geometric-0.0.4/examples/GATConv_CORA.ipynb
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15424 2023-01-05 15:41:27.000000 haiku_geometric-0.0.4/examples/GCNConv_karate_club.ipynb
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.084675 haiku_geometric-0.0.4/haiku_geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      222 2023-04-24 19:10:41.000000 haiku_geometric-0.0.4/haiku_geometric/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.084675 haiku_geometric-0.0.4/haiku_geometric/datasets/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      423 2023-01-05 00:20:36.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1754 2023-05-07 16:14:22.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/base.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6126 2023-05-07 18:50:18.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/gnn_benchmark_dataset.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3289 2023-01-01 22:08:25.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/karate_dataset.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3299 2023-05-07 16:16:15.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/ogb_dataset.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6283 2023-05-07 16:17:47.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/planetoid_dataset.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2761 2023-01-01 22:10:36.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/toy_dataset.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1330 2023-01-01 23:05:48.000000 haiku_geometric-0.0.4/haiku_geometric/datasets/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.088675 haiku_geometric-0.0.4/haiku_geometric/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3552 2023-04-05 20:26:14.000000 haiku_geometric-0.0.4/haiku_geometric/models/MLP.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      104 2023-03-23 17:08:28.000000 haiku_geometric-0.0.4/haiku_geometric/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5111 2023-04-05 20:33:47.000000 haiku_geometric-0.0.4/haiku_geometric/models/node2vec.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.088675 haiku_geometric-0.0.4/haiku_geometric/nn/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      106 2022-12-31 16:03:36.000000 haiku_geometric-0.0.4/haiku_geometric/nn/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.088675 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      380 2022-12-30 14:14:01.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      254 2022-12-22 17:22:33.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/base.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1972 2022-12-22 17:22:47.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/basic.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3841 2023-01-01 22:14:38.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/degree_scaler.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4042 2023-01-01 22:16:40.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/multi.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      677 2023-01-01 22:16:40.000000 haiku_geometric-0.0.4/haiku_geometric/nn/aggr/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.088675 haiku_geometric-0.0.4/haiku_geometric/nn/attention/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      152 2023-04-24 15:22:12.000000 haiku_geometric-0.0.4/haiku_geometric/nn/attention/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1027 2023-04-24 14:53:47.000000 haiku_geometric-0.0.4/haiku_geometric/nn/attention/self_attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3673 2023-04-24 22:55:04.000000 haiku_geometric-0.0.4/haiku_geometric/nn/attention/transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.092675 haiku_geometric-0.0.4/haiku_geometric/nn/conv/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      581 2022-12-31 16:46:59.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2174 2022-12-31 16:55:56.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7941 2023-03-06 00:12:14.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3445 2022-12-25 16:13:28.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gated_graph_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5599 2023-03-25 00:25:26.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9278 2023-03-06 00:15:29.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/general_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2385 2022-12-25 15:57:11.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3063 2023-01-01 22:16:40.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gine_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10081 2023-02-10 19:39:38.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/gps_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2591 2022-12-25 15:57:32.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/graph_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4904 2023-01-01 23:11:07.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/pna_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3981 2022-12-25 15:57:41.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/sage_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      679 2022-12-22 15:52:35.000000 haiku_geometric-0.0.4/haiku_geometric/nn/conv/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.092675 haiku_geometric-0.0.4/haiku_geometric/nn/dense/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       75 2022-12-24 16:28:03.000000 haiku_geometric-0.0.4/haiku_geometric/nn/dense/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1724 2023-01-01 22:16:40.000000 haiku_geometric-0.0.4/haiku_geometric/nn/dense/linear.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.092675 haiku_geometric-0.0.4/haiku_geometric/nn/pool/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      179 2022-12-24 16:27:45.000000 haiku_geometric-0.0.4/haiku_geometric/nn/pool/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2022-12-22 15:54:37.000000 haiku_geometric-0.0.4/haiku_geometric/nn/pool/global_pool.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/haiku_geometric/posenc/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-04-24 18:46:41.000000 haiku_geometric-0.0.4/haiku_geometric/posenc/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6836 2023-04-24 23:28:33.000000 haiku_geometric-0.0.4/haiku_geometric/posenc/laplacian_encoder.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17692 2023-04-24 23:37:13.000000 haiku_geometric-0.0.4/haiku_geometric/posenc/mag_laplacian_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/haiku_geometric/transforms/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      241 2023-03-02 23:18:18.000000 haiku_geometric-0.0.4/haiku_geometric/transforms/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2930 2023-03-06 00:24:35.000000 haiku_geometric-0.0.4/haiku_geometric/transforms/add_self_loops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      335 2023-01-05 00:17:09.000000 haiku_geometric-0.0.4/haiku_geometric/transforms/normalize.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      380 2023-03-02 23:18:18.000000 haiku_geometric-0.0.4/haiku_geometric/transforms/remove_self_loops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/haiku_geometric/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      532 2023-05-07 18:49:40.000000 haiku_geometric-0.0.4/haiku_geometric/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3507 2023-05-27 19:38:12.000000 haiku_geometric-0.0.4/haiku_geometric/utils/batch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2863 2023-03-24 23:44:33.000000 haiku_geometric-0.0.4/haiku_geometric/utils/coalesce.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9803 2023-04-24 16:47:20.000000 haiku_geometric-0.0.4/haiku_geometric/utils/laplacian.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8845 2023-04-24 23:31:47.000000 haiku_geometric-0.0.4/haiku_geometric/utils/magnetic_laplacian.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4212 2023-04-05 18:43:45.000000 haiku_geometric-0.0.4/haiku_geometric/utils/random_walk.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1331 2023-03-24 23:41:24.000000 haiku_geometric-0.0.4/haiku_geometric/utils/undirected.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      671 2023-03-22 16:38:01.000000 haiku_geometric-0.0.4/haiku_geometric/utils/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.084675 haiku_geometric-0.0.4/haiku_geometric.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11387 2023-05-27 23:26:54.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3529 2023-05-27 23:26:54.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-27 23:26:54.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-01-01 22:48:42.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-05-27 23:26:54.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-05-27 23:26:54.000000 haiku_geometric-0.0.4/haiku_geometric.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2023-03-25 01:42:52.000000 haiku_geometric-0.0.4/requirements.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      582 2023-05-27 23:26:54.104675 haiku_geometric-0.0.4/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)       37 2021-11-14 17:58:45.000000 haiku_geometric-0.0.4/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/test/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/test/datasets/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      295 2023-01-01 18:38:53.000000 haiku_geometric-0.0.4/test/datasets/test_karate.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      301 2023-01-04 20:47:28.000000 haiku_geometric-0.0.4/test/datasets/test_toy.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.096675 haiku_geometric-0.0.4/test/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1482 2023-04-05 19:36:12.000000 haiku_geometric-0.0.4/test/models/test_Node2Vec.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.076675 haiku_geometric-0.0.4/test/nn/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.100675 haiku_geometric-0.0.4/test/nn/aggr/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      922 2023-01-01 18:50:45.000000 haiku_geometric-0.0.4/test/nn/aggr/test_basic.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.100675 haiku_geometric-0.0.4/test/nn/conv/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      723 2023-01-01 18:49:01.000000 haiku_geometric-0.0.4/test/nn/conv/test_EdgeConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1644 2023-01-01 18:51:28.000000 haiku_geometric-0.0.4/test/nn/conv/test_GCNConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      857 2023-01-01 18:49:44.000000 haiku_geometric-0.0.4/test/nn/conv/test_GINConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      946 2023-01-01 18:49:49.000000 haiku_geometric-0.0.4/test/nn/conv/test_GINEConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2117 2023-02-25 00:01:01.000000 haiku_geometric-0.0.4/test/nn/conv/test_GPSLayer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-01-01 18:49:24.000000 haiku_geometric-0.0.4/test/nn/conv/test_GatedGraphConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1592 2023-01-01 18:51:03.000000 haiku_geometric-0.0.4/test/nn/conv/test_GeneralConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1356 2023-01-01 18:50:20.000000 haiku_geometric-0.0.4/test/nn/conv/test_GraphConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2127 2023-01-01 18:55:57.000000 haiku_geometric-0.0.4/test/nn/conv/test_PNAConv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1115 2023-01-01 18:50:25.000000 haiku_geometric-0.0.4/test/nn/conv/test_SAGEConv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.100675 haiku_geometric-0.0.4/test/nn/dense/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      690 2023-01-01 18:51:41.000000 haiku_geometric-0.0.4/test/nn/dense/test_linear.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.100675 haiku_geometric-0.0.4/test/nn/pool/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2185 2023-01-01 18:51:58.000000 haiku_geometric-0.0.4/test/nn/pool/test_global.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-04-05 20:19:34.000000 haiku_geometric-0.0.4/test/requirements.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-27 23:26:54.104675 haiku_geometric-0.0.4/test/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      760 2023-03-06 20:26:26.000000 haiku_geometric-0.0.4/test/utils/test_coalesce.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      835 2023-03-26 17:29:38.000000 haiku_geometric-0.0.4/test/utils/test_eigv_laplacian.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2915 2023-03-06 16:02:00.000000 haiku_geometric-0.0.4/test/utils/test_laplacian.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2942 2023-04-05 19:47:50.000000 haiku_geometric-0.0.4/test/utils/test_magnetic_laplacian.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `haiku_geometric-0.0.3/.github/workflows/python-app.yml` & `haiku_geometric-0.0.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/.gitignore` & `haiku_geometric-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/.readthedocs.yml` & `haiku_geometric-0.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/PKG-INFO` & `haiku_geometric-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haiku_geometric
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/alexOarga/haiku-geometric
 Author: Alex Oarga
 Author-email: alex718123@gmail.com
 License: Apache-2.0 license
 Description: # Haiku Geometric
         
@@ -117,14 +117,22 @@
         | [GraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GraphConv)           | Graph convolution layer from the [Weisfeiler and Leman Go Neural: Higher-order Graph Neural Networks](https://arxiv.org/abs/1810.02244) paper. |
         | [GeneralConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GeneralConv)       | A general GNN layer adapted from the [Design Space for Graph Neural Networks](https://arxiv.org/abs/2011.08843) paper.                         |
         | [GatedGraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GatedGraphConv) | Graph convolution layer from the [Gated Graph Sequence Neural Networks](https://arxiv.org/abs/1511.05493) paper.                               |
         | [EdgeConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.EdgeConv)             | Edge convolution layer from the [Dynamic Graph CNN for Learning on Point Clouds](https://arxiv.org/abs/1801.07829) paper.                      |
         | [PNAConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.PNAConv)               | Propagation Network layer from the [Principal Neighbourhood Aggregation for Graph Nets](https://arxiv.org/abs/2004.05718) paper.               |
         | [GPSLayer](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GPSLayer)             | Graph Pooling layer from the [Recipe for a General, Powerful, Scalable Graph Transformer](https://arxiv.org/abs/2205.12454) paper.             |
         
+        ## Implemented positional encodings
+        
+        The following positional encodings are currently available:
+        
+        | Model                                                                                                                     | Description                                                                                                                                     |
+        |---------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
+        | [LaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.LaplacianEncoder)    | Laplacian positional encoding from the [Rethinking Graph Transformers with Spectral Attention](https://arxiv.org/pdf/2106.03893) paper.         |
+        | [MagLaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.MagLaplacianEncoder)  | Magnetic Laplacian positional encoding from the [Transformers Meet Directed Graphs](https://arxiv.org/pdf/2302.00049) paper. |
         
         ## Issues
         
         If you encounter any issue, please [open an issue](https://github.com/alexOarga/haiku-geometric/issues/new).
         
         ## Running tests
```

### Comparing `haiku_geometric-0.0.3/README.md` & `haiku_geometric-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,22 @@
 | [GraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GraphConv)           | Graph convolution layer from the [Weisfeiler and Leman Go Neural: Higher-order Graph Neural Networks](https://arxiv.org/abs/1810.02244) paper. |
 | [GeneralConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GeneralConv)       | A general GNN layer adapted from the [Design Space for Graph Neural Networks](https://arxiv.org/abs/2011.08843) paper.                         |
 | [GatedGraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GatedGraphConv) | Graph convolution layer from the [Gated Graph Sequence Neural Networks](https://arxiv.org/abs/1511.05493) paper.                               |
 | [EdgeConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.EdgeConv)             | Edge convolution layer from the [Dynamic Graph CNN for Learning on Point Clouds](https://arxiv.org/abs/1801.07829) paper.                      |
 | [PNAConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.PNAConv)               | Propagation Network layer from the [Principal Neighbourhood Aggregation for Graph Nets](https://arxiv.org/abs/2004.05718) paper.               |
 | [GPSLayer](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GPSLayer)             | Graph Pooling layer from the [Recipe for a General, Powerful, Scalable Graph Transformer](https://arxiv.org/abs/2205.12454) paper.             |
 
+## Implemented positional encodings
+
+The following positional encodings are currently available:
+
+| Model                                                                                                                     | Description                                                                                                                                     |
+|---------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
+| [LaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.LaplacianEncoder)    | Laplacian positional encoding from the [Rethinking Graph Transformers with Spectral Attention](https://arxiv.org/pdf/2106.03893) paper.         |
+| [MagLaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.MagLaplacianEncoder)  | Magnetic Laplacian positional encoding from the [Transformers Meet Directed Graphs](https://arxiv.org/pdf/2302.00049) paper. |
 
 ## Issues
 
 If you encounter any issue, please [open an issue](https://github.com/alexOarga/haiku-geometric/issues/new).
 
 ## Running tests
```

### Comparing `haiku_geometric-0.0.3/docs/Makefile` & `haiku_geometric-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/make.bat` & `haiku_geometric-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/conf.py` & `haiku_geometric-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/examples.rst` & `haiku_geometric-0.0.4/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/index.rst` & `haiku_geometric-0.0.4/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,30 @@
    
 .. toctree::
    :caption: Contents
    :maxdepth: 1
 
    notebooks/1_quickstart
    notebooks/creating_dataset
+   notebooks/batch_support
    examples
 
 .. toctree::
    :glob:
    :maxdepth: 1
    :caption: API Reference
 
    modules/nn
    modules/datasets
    modules/models
+   modules/posenc
    modules/transforms
    modules/utils
 
 
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `haiku_geometric-0.0.3/docs/source/modules/nn.rst` & `haiku_geometric-0.0.4/docs/source/modules/nn.rst`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/notebooks/1_quickstart.ipynb` & `haiku_geometric-0.0.4/docs/source/notebooks/1_quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/notebooks/_static/graph1.png` & `haiku_geometric-0.0.4/docs/source/notebooks/_static/graph1.png`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/notebooks/_static/graph2.png` & `haiku_geometric-0.0.4/docs/source/notebooks/_static/graph2.png`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/docs/source/notebooks/creating_dataset.ipynb` & `haiku_geometric-0.0.4/docs/source/notebooks/creating_dataset.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950396825396826%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'version': '3.9.16'}}"}*

```diff
@@ -217,27 +217,27 @@
         }
     ],
     "metadata": {
         "colab": {
             "provenance": []
         },
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.12"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `haiku_geometric-0.0.3/examples/1_quickstart.ipynb` & `haiku_geometric-0.0.4/examples/1_quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/examples/GATConv_CORA.ipynb` & `haiku_geometric-0.0.4/examples/GATConv_CORA.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996969696969697%*

 * *Differences: {"'cells'": "{21: {'source': ['Not bad but needs more regularization / tuning.']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}}"}*

```diff
@@ -539,26 +539,26 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "lNGveYI-hXmz"
             },
             "source": [
-                "Not bad but needs more regularization / fine tuning!"
+                "Not bad but needs more regularization / tuning."
             ]
         }
     ],
     "metadata": {
         "accelerator": "GPU",
         "colab": {
             "provenance": []
         },
         "gpuClass": "standard",
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
```

### Comparing `haiku_geometric-0.0.3/examples/GCNConv_karate_club.ipynb` & `haiku_geometric-0.0.4/examples/GCNConv_karate_club.ipynb`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/base.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     - train_mask: If available, array of booleans indicating which elements are in the train set.
     
     """
     nodes: Optional[ArrayTree]
     edges: Optional[ArrayTree]
     receivers: Optional[jnp.ndarray]  # with integer dtype
     senders: Optional[jnp.ndarray]  # with integer dtype
-    n_node: int  # with integer dtype
-    n_edge: int   # with integer dtype
+    n_node: jnp.ndarray  # with integer dtype
+    n_edge: jnp.ndarray   # with integer dtype
     globals: Optional[ArrayTree]
     position: Optional[jnp.ndarray]
     y: Optional[jnp.ndarray]
     train_mask: Optional[jnp.ndarray]
 
 
 class GraphDataset():
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/gnn_benchmark_dataset.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,16 @@
             return DataGraphTuple(
                 nodes=jnp.array(graph['x'].numpy()),
                 position=jnp.array(graph['pos'].numpy()),
                 y=jnp.array(graph['y']),
                 edges=jnp.array(graph['edge_attr'].numpy()),
                 senders=jnp.array(graph['edge_index'].numpy()[0]),
                 receivers=jnp.array(graph['edge_index'].numpy()[1]),
-                n_node=graph['x'].shape[0],
-                n_edge=graph['edge_index'].shape[1],
+                n_node=jnp.array([graph['x'].shape[0]]),
+                n_edge=jnp.array([graph['edge_index'].shape[1]]),
                 globals=None,
                 train_mask=None,
             )
 
         bar = tqdm(range(len(data)))
         for i in bar:
             bar.set_description("Processing graph ")
@@ -121,16 +121,16 @@
             res.append(
                 DataGraphTuple(
                     nodes=None,
                     edges=None,
                     y=jnp.array(y),
                     senders=jnp.array(adj.row),
                     receivers=jnp.array(adj.col),
-                    n_node=adj.shape[0],
-                    n_edge=adj.row.shape[0],
+                    n_node=jnp.array([adj.shape[0]]),
+                    n_edge=jnp.array([adj.row.shape[0]]),
                     globals=None,
                     position=None,
                     train_mask=None,
                 )
             )
 
         return res
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/karate_dataset.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/karate_dataset.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/ogb_dataset.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/ogb_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         graph = graph[0]
 
         args = {
             'nodes': jnp.asarray(graph['node_feat']),
             'edges': jnp.asarray(graph['edge_feat']),
             'senders': jnp.asarray(graph['edge_index'][0]),
             'receivers': jnp.asarray(graph['edge_index'][1]),
-            'n_node': graph['num_nodes'],
-            'n_edge': graph['edge_index'].shape[1],
+            'n_node': jnp.asarray([graph['num_nodes']]),
+            'n_edge': jnp.asarray([graph['edge_index'].shape[1]]),
             'globals': None,
             'y': jnp.asarray(y),
             'train_mask': None,
             'position': None
         }
         return DataGraphTuple(**args)
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/planetoid_dataset.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/planetoid_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         senders, receivers = self._senders_receivers_from_dict(graph)
 
         graph = DataGraphTuple(
             nodes=nx,
             senders=senders,
             receivers=receivers,
             edges=None,
-            n_node=ny.shape[0],
-            n_edge=senders.shape[0],
+            n_node=jnp.asarray([ny.shape[0]]),
+            n_edge=jnp.asarray([senders.shape[0]]),
             globals=None,
             y=ny,
             train_mask=None,
             position=None
         )
 
         train_mask = train_mask
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/toy_dataset.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/toy_dataset.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/datasets/utils.py` & `haiku_geometric-0.0.4/haiku_geometric/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/models/MLP.py` & `haiku_geometric-0.0.4/haiku_geometric/models/MLP.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/models/node2vec.py` & `haiku_geometric-0.0.4/haiku_geometric/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/aggr/basic.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/aggr/degree_scaler.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/aggr/degree_scaler.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/aggr/multi.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/aggr/utils.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/attention/self_attention.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/attention/self_attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import haiku as hk
 import jax
+import warnings
 import jax.numpy as jnp
 from typing import Optional
 
 
 class SelfAttention(hk.MultiHeadAttention):
     """Self attention with a causal mask applied."""
 
@@ -11,14 +12,20 @@
             self,
             query: jnp.ndarray,
             key: Optional[jnp.ndarray] = None,
             value: Optional[jnp.ndarray] = None,
             mask: Optional[jnp.ndarray] = None,
     ) -> jnp.ndarray:
         """"""
+        warnings.warn(
+            "SelfAttention will be removed"
+            "Please use haiku.MultiHeadAttention.",
+            DeprecationWarning,
+        )
+
         key = key if key is not None else query
         value = value if value is not None else query
 
         seq_len = query.shape[1]
         causal_mask = jnp.tril(jnp.ones((seq_len, seq_len)))
         mask = mask * causal_mask if mask is not None else causal_mask
         mask_shape = mask.shape
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/__init__.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/edge_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gat_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gated_graph_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gcn_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/general_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gin_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gine_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gine_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/gps_layer.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/gps_layer.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/graph_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/pna_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/sage_conv.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/conv/utils.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/conv/utils.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/dense/linear.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/nn/pool/global_pool.py` & `haiku_geometric-0.0.4/haiku_geometric/nn/pool/global_pool.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/transforms/add_self_loops.py` & `haiku_geometric-0.0.4/haiku_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/coalesce.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/coalesce.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/laplacian.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,16 @@
             (default: :obj:`5`)
         eigv_norm (str, optional): The normalization to apply to the eigenvectors.
             (default: :obj:`"L2"`). Available options are:
             1. :obj:`None` : No normalization.
             2. :obj:`"L2"` : Normalize the eigenvectors to have unit L2 norm.
 
     Returns:
-        :obj:`Tuple(jnp.ndarray, jnp.ndarray)`: The top-k eigenvalues and eigenvectors of the Laplacian.
+        :obj:`(jnp.ndarray)`:  (k,) eigenvalues.
+        :obj:`(jnp.ndarray)`:  (num_nodes, k) of eigenvector values per node.
     """
 
     L = get_laplacian_matrix(
         senders, receivers, edge_weight, normalization,num_nodes)
     evals, evects = jnp.linalg.eigh(L)
 
     N = len(evals)
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/magnetic_laplacian.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/magnetic_laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     return eigenvalues.real, eigenvectors, laplacian
 
 
 def eigv_magnetic_laplacian(
         senders: jnp.ndarray,
         receivers: jnp.ndarray,
-        n_node: jnp.ndarray,
+        n_node: int,
         k: int,
         k_excl: int,
         q: float = 0.25,
         q_absolute: bool = False,
         norm_comps_sep: bool = False,
         l2_norm: bool = True,
         sign_rotate: bool = True,
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/random_walk.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/random_walk.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/undirected.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric/utils/utils.py` & `haiku_geometric-0.0.4/haiku_geometric/utils/utils.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/haiku_geometric.egg-info/PKG-INFO` & `haiku_geometric-0.0.4/haiku_geometric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haiku-geometric
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/alexOarga/haiku-geometric
 Author: Alex Oarga
 Author-email: alex718123@gmail.com
 License: Apache-2.0 license
 Description: # Haiku Geometric
         
@@ -117,14 +117,22 @@
         | [GraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GraphConv)           | Graph convolution layer from the [Weisfeiler and Leman Go Neural: Higher-order Graph Neural Networks](https://arxiv.org/abs/1810.02244) paper. |
         | [GeneralConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GeneralConv)       | A general GNN layer adapted from the [Design Space for Graph Neural Networks](https://arxiv.org/abs/2011.08843) paper.                         |
         | [GatedGraphConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GatedGraphConv) | Graph convolution layer from the [Gated Graph Sequence Neural Networks](https://arxiv.org/abs/1511.05493) paper.                               |
         | [EdgeConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.EdgeConv)             | Edge convolution layer from the [Dynamic Graph CNN for Learning on Point Clouds](https://arxiv.org/abs/1801.07829) paper.                      |
         | [PNAConv](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.PNAConv)               | Propagation Network layer from the [Principal Neighbourhood Aggregation for Graph Nets](https://arxiv.org/abs/2004.05718) paper.               |
         | [GPSLayer](https://haiku-geometric.readthedocs.io/en/latest/modules/nn.html#haiku_geometric.nn.conv.GPSLayer)             | Graph Pooling layer from the [Recipe for a General, Powerful, Scalable Graph Transformer](https://arxiv.org/abs/2205.12454) paper.             |
         
+        ## Implemented positional encodings
+        
+        The following positional encodings are currently available:
+        
+        | Model                                                                                                                     | Description                                                                                                                                     |
+        |---------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
+        | [LaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.LaplacianEncoder)    | Laplacian positional encoding from the [Rethinking Graph Transformers with Spectral Attention](https://arxiv.org/pdf/2106.03893) paper.         |
+        | [MagLaplacianEncoder](https://haiku-geometric.readthedocs.io/en/latest/modules/posenc.html#haiku_geometric.posenc.MagLaplacianEncoder)  | Magnetic Laplacian positional encoding from the [Transformers Meet Directed Graphs](https://arxiv.org/pdf/2302.00049) paper. |
         
         ## Issues
         
         If you encounter any issue, please [open an issue](https://github.com/alexOarga/haiku-geometric/issues/new).
         
         ## Running tests
```

### Comparing `haiku_geometric-0.0.3/haiku_geometric.egg-info/SOURCES.txt` & `haiku_geometric-0.0.4/haiku_geometric.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 haiku_geometric/nn/aggr/base.py
 haiku_geometric/nn/aggr/basic.py
 haiku_geometric/nn/aggr/degree_scaler.py
 haiku_geometric/nn/aggr/multi.py
 haiku_geometric/nn/aggr/utils.py
 haiku_geometric/nn/attention/__init__.py
 haiku_geometric/nn/attention/self_attention.py
+haiku_geometric/nn/attention/transformer.py
 haiku_geometric/nn/conv/__init__.py
 haiku_geometric/nn/conv/edge_conv.py
 haiku_geometric/nn/conv/gat_conv.py
 haiku_geometric/nn/conv/gated_graph_conv.py
 haiku_geometric/nn/conv/gcn_conv.py
 haiku_geometric/nn/conv/general_conv.py
 haiku_geometric/nn/conv/gin_conv.py
@@ -63,19 +64,23 @@
 haiku_geometric/nn/conv/pna_conv.py
 haiku_geometric/nn/conv/sage_conv.py
 haiku_geometric/nn/conv/utils.py
 haiku_geometric/nn/dense/__init__.py
 haiku_geometric/nn/dense/linear.py
 haiku_geometric/nn/pool/__init__.py
 haiku_geometric/nn/pool/global_pool.py
+haiku_geometric/posenc/__init__.py
+haiku_geometric/posenc/laplacian_encoder.py
+haiku_geometric/posenc/mag_laplacian_encoder.py
 haiku_geometric/transforms/__init__.py
 haiku_geometric/transforms/add_self_loops.py
 haiku_geometric/transforms/normalize.py
 haiku_geometric/transforms/remove_self_loops.py
 haiku_geometric/utils/__init__.py
+haiku_geometric/utils/batch.py
 haiku_geometric/utils/coalesce.py
 haiku_geometric/utils/laplacian.py
 haiku_geometric/utils/magnetic_laplacian.py
 haiku_geometric/utils/random_walk.py
 haiku_geometric/utils/undirected.py
 haiku_geometric/utils/utils.py
 test/requirements.txt
```

### Comparing `haiku_geometric-0.0.3/setup.cfg` & `haiku_geometric-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = haiku_geometric
 url = https://github.com/alexOarga/haiku-geometric
-version = 0.0.3
+version = 0.0.4
 author = Alex Oarga
 author_email = alex718123@gmail.com
 long_description = file: README.md, CHANGELOG.rst, LICENSE
 long_description_content_type = text/markdown
 license = Apache-2.0 license
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `haiku_geometric-0.0.3/test/models/test_Node2Vec.py` & `haiku_geometric-0.0.4/test/models/test_Node2Vec.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/aggr/test_basic.py` & `haiku_geometric-0.0.4/test/nn/aggr/test_basic.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_EdgeConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_EdgeConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GCNConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GCNConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GINConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GINConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GINEConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GINEConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GPSLayer.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GPSLayer.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GatedGraphConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GatedGraphConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GeneralConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GeneralConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_GraphConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_GraphConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_PNAConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_PNAConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/conv/test_SAGEConv.py` & `haiku_geometric-0.0.4/test/nn/conv/test_SAGEConv.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/dense/test_linear.py` & `haiku_geometric-0.0.4/test/nn/dense/test_linear.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/nn/pool/test_global.py` & `haiku_geometric-0.0.4/test/nn/pool/test_global.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/utils/test_coalesce.py` & `haiku_geometric-0.0.4/test/utils/test_coalesce.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/utils/test_eigv_laplacian.py` & `haiku_geometric-0.0.4/test/utils/test_eigv_laplacian.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/utils/test_laplacian.py` & `haiku_geometric-0.0.4/test/utils/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `haiku_geometric-0.0.3/test/utils/test_magnetic_laplacian.py` & `haiku_geometric-0.0.4/test/utils/test_magnetic_laplacian.py`

 * *Files identical despite different names*

