# Comparing `tmp/flixit-0.4.tar.gz` & `tmp/flixit-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixit-0.4.tar", last modified: Sun May 28 08:50:16 2023, max compression
+gzip compressed data, was "flixit-0.5.tar", last modified: Sun May 28 19:12:58 2023, max compression
```

## Comparing `flixit-0.4.tar` & `flixit-0.5.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 08:50:16.955056 flixit-0.4/
--rw-rw-rw-   0        0        0      256 2023-05-28 08:50:16.955056 flixit-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       27 2023-05-28 08:18:42.000000 flixit-0.4/README.rst
--rw-rw-rw-   0        0        0      115 2023-05-28 08:50:16.962056 flixit-0.4/setup.cfg
--rw-rw-rw-   0        0        0      393 2023-05-28 08:49:51.000000 flixit-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:50:16.764618 flixit-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 08:50:16.896715 flixit-0.4/src/flixit/
--rw-rw-rw-   0        0        0     2276 2023-05-27 18:03:50.000000 flixit-0.4/src/flixit/CUDA_Matrix_Multiplication.py
--rw-rw-rw-   0        0        0     1764 2023-05-27 18:03:50.000000 flixit-0.4/src/flixit/CUDA_Vector_Addition.py
--rw-rw-rw-   0        0        0     2729 2023-05-27 18:03:51.000000 flixit-0.4/src/flixit/HPC_Assignment_1.py
--rw-rw-rw-   0        0        0     3587 2023-05-27 18:03:51.000000 flixit-0.4/src/flixit/HPC_Assignment_2.py
--rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.4/src/flixit/__init__.py
--rw-rw-rw-   0        0        0     4026 2023-05-28 08:45:33.000000 flixit-0.4/src/flixit/bouston_house_linear_regression.py
--rw-rw-rw-   0        0        0     6253 2023-05-28 08:46:38.000000 flixit-0.4/src/flixit/demo_ocr.py
--rw-rw-rw-   0        0        0     4548 2023-05-28 08:47:01.000000 flixit-0.4/src/flixit/dl_mnistfashion.py
--rw-rw-rw-   0        0        0     2809 2023-05-28 08:47:23.000000 flixit-0.4/src/flixit/google_stock_prices_using_rnn.py
--rw-rw-rw-   0        0        0     1457 2023-05-27 18:03:51.000000 flixit-0.4/src/flixit/parallel_reduction.py
--rw-rw-rw-   0        0        0     6379 2023-05-28 08:47:48.000000 flixit-0.4/src/flixit/plant_disease_detection_using_keras.py
--rw-rw-rw-   0        0        0     6730 2023-05-28 08:48:39.000000 flixit-0.4/src/flixit/sentiment_analysis_on_imdb_dataset___nn.py
--rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.4/src/flixit/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:50:16.954055 flixit-0.4/src/flixit.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-28 08:50:16.000000 flixit-0.4/src/flixit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-28 08:50:16.000000 flixit-0.4/src/flixit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 08:50:16.000000 flixit-0.4/src/flixit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 08:50:16.000000 flixit-0.4/src/flixit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:58.515345 flixit-0.5/
+-rw-rw-rw-   0        0        0      256 2023-05-28 19:12:58.515345 flixit-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-05-28 08:18:42.000000 flixit-0.5/README.rst
+-rw-rw-rw-   0        0        0      115 2023-05-28 19:12:58.517349 flixit-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      393 2023-05-28 19:12:23.000000 flixit-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:58.420771 flixit-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:58.479874 flixit-0.5/src/flixit/
+-rw-rw-rw-   0        0        0     2276 2023-05-27 18:03:50.000000 flixit-0.5/src/flixit/CUDA_Matrix_Multiplication.py
+-rw-rw-rw-   0        0        0     1764 2023-05-27 18:03:50.000000 flixit-0.5/src/flixit/CUDA_Vector_Addition.py
+-rw-rw-rw-   0        0        0     2729 2023-05-27 18:03:51.000000 flixit-0.5/src/flixit/HPC_Assignment_1_bfs_dfs.py
+-rw-rw-rw-   0        0        0     3587 2023-05-27 18:03:51.000000 flixit-0.5/src/flixit/HPC_Assignment_2_merge_bubble.py
+-rw-rw-rw-   0        0        0      444 2023-05-28 14:35:35.000000 flixit-0.5/src/flixit/UbuntuStepsnew.py
+-rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.5/src/flixit/__init__.py
+-rw-rw-rw-   0        0        0     4026 2023-05-28 08:45:33.000000 flixit-0.5/src/flixit/bouston_house_linear_regression.py
+-rw-rw-rw-   0        0        0     1276 2023-05-28 19:08:46.000000 flixit-0.5/src/flixit/bouston_sidnew.py
+-rw-rw-rw-   0        0        0     1301 2023-05-28 13:43:25.000000 flixit-0.5/src/flixit/bubble_sort_parallel_hpc2.py
+-rw-rw-rw-   0        0        0     1103 2023-05-28 18:46:27.000000 flixit-0.5/src/flixit/bubblen.py
+-rw-rw-rw-   0        0        0     6253 2023-05-28 08:46:38.000000 flixit-0.5/src/flixit/demo_ocr.py
+-rw-rw-rw-   0        0        0     4548 2023-05-28 08:47:01.000000 flixit-0.5/src/flixit/dl_mnistfashion.py
+-rw-rw-rw-   0        0        0     2809 2023-05-28 08:47:23.000000 flixit-0.5/src/flixit/google_stock_prices_using_rnn.py
+-rw-rw-rw-   0        0        0     2638 2023-05-28 18:48:25.000000 flixit-0.5/src/flixit/google_stock_using_rnn_sid.py
+-rw-rw-rw-   0        0        0     4572 2023-05-28 18:32:37.000000 flixit-0.5/src/flixit/hpc_4_cuda_multiply_and_addition.py
+-rw-rw-rw-   0        0        0     1953 2023-05-28 18:46:27.000000 flixit-0.5/src/flixit/merge.py
+-rw-rw-rw-   0        0        0     2563 2023-05-28 13:43:25.000000 flixit-0.5/src/flixit/merge_sort_parallel_hpc2.py
+-rw-rw-rw-   0        0        0     1643 2023-05-28 18:46:29.000000 flixit-0.5/src/flixit/paralSidreduction.py
+-rw-rw-rw-   0        0        0     6379 2023-05-28 08:47:48.000000 flixit-0.5/src/flixit/plant_disease_detection_using_keras.py
+-rw-rw-rw-   0        0        0     6730 2023-05-28 08:48:39.000000 flixit-0.5/src/flixit/sentiment_analysis_on_imdb_dataset___nn.py
+-rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.5/src/flixit/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:12:58.513347 flixit-0.5/src/flixit.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-28 19:12:58.000000 flixit-0.5/src/flixit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-05-28 19:12:58.000000 flixit-0.5/src/flixit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:12:58.000000 flixit-0.5/src/flixit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 19:12:58.000000 flixit-0.5/src/flixit.egg-info/top_level.txt
```

### Comparing `flixit-0.4/src/flixit/CUDA_Matrix_Multiplication.py` & `flixit-0.5/src/flixit/CUDA_Matrix_Multiplication.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/CUDA_Vector_Addition.py` & `flixit-0.5/src/flixit/CUDA_Vector_Addition.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/HPC_Assignment_1.py` & `flixit-0.5/src/flixit/HPC_Assignment_1_bfs_dfs.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/HPC_Assignment_2.py` & `flixit-0.5/src/flixit/HPC_Assignment_2_merge_bubble.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/bouston_house_linear_regression.py` & `flixit-0.5/src/flixit/bouston_house_linear_regression.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/demo_ocr.py` & `flixit-0.5/src/flixit/demo_ocr.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/dl_mnistfashion.py` & `flixit-0.5/src/flixit/dl_mnistfashion.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/google_stock_prices_using_rnn.py` & `flixit-0.5/src/flixit/google_stock_prices_using_rnn.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/plant_disease_detection_using_keras.py` & `flixit-0.5/src/flixit/plant_disease_detection_using_keras.py`

 * *Files identical despite different names*

### Comparing `flixit-0.4/src/flixit/sentiment_analysis_on_imdb_dataset___nn.py` & `flixit-0.5/src/flixit/sentiment_analysis_on_imdb_dataset___nn.py`

 * *Files identical despite different names*

