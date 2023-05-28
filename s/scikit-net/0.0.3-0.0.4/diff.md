# Comparing `tmp/scikit-net-0.0.3.tar.gz` & `tmp/scikit-net-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-net-0.0.3.tar", last modified: Sun May 28 19:18:05 2023, max compression
+gzip compressed data, was "scikit-net-0.0.4.tar", last modified: Sun May 28 19:28:26 2023, max compression
```

## Comparing `scikit-net-0.0.3.tar` & `scikit-net-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.769550 scikit-net-0.0.3/
--rw-rw-rw-   0        0        0     1097 2023-05-28 19:15:13.000000 scikit-net-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2982 2023-05-28 19:18:05.769550 scikit-net-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2403 2023-05-28 19:15:13.000000 scikit-net-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.663420 scikit-net-0.0.3/scikit_net.egg-info/
--rw-rw-rw-   0        0        0     2982 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 19:18:05.769550 scikit-net-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1778 2023-05-28 19:16:11.000000 scikit-net-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.664421 scikit-net-0.0.3/sknet/
--rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.689931 scikit-net-0.0.3/sknet/network_construction/
--rw-rw-rw-   0        0        0      482 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/__init__.py
--rw-rw-rw-   0        0        0    31835 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/dataset_constructors.py
--rw-rw-rw-   0        0        0     2471 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/general_constructors.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.696933 scikit-net-0.0.3/sknet/network_construction/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/tests/__init__.py
--rw-rw-rw-   0        0        0    10630 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/tests/test_network_construction.py
--rw-rw-rw-   0        0        0    11583 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/time_series_constructors.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.708451 scikit-net-0.0.3/sknet/semi_supervised/
--rw-rw-rw-   0        0        0       86 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/semi_supervised/__init__.py
--rw-rw-rw-   0        0        0    10575 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/semi_supervised/modularity_label_propagation.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.723652 scikit-net-0.0.3/sknet/supervised/
--rw-rw-rw-   0        0        0      179 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/__init__.py
--rw-rw-rw-   0        0        0    12364 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/ease_of_access.py
--rw-rw-rw-   0        0        0     9637 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/high_level_classification.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.733668 scikit-net-0.0.3/sknet/supervised/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/__init__.py
--rw-rw-rw-   0        0        0     6165 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/test_ease_of_access.py
--rw-rw-rw-   0        0        0     1631 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/test_high_level_classification.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.744373 scikit-net-0.0.3/sknet/unsupervised/
--rw-rw-rw-   0        0        0       90 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/unsupervised/__init__.py
--rw-rw-rw-   0        0        0    12078 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/unsupervised/stochastic_particle_competition.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.768488 scikit-net-0.0.3/sknet/utils/
--rw-rw-rw-   0        0        0      191 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/__init__.py
--rw-rw-rw-   0        0        0      939 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/low_level_models_handler.py
--rw-rw-rw-   0        0        0     1037 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/network_metrics_handler.py
--rw-rw-rw-   0        0        0      472 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/network_types_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.650097 scikit-net-0.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-05-28 19:15:13.000000 scikit-net-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2982 2023-05-28 19:28:26.650097 scikit-net-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2403 2023-05-28 19:15:13.000000 scikit-net-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.631226 scikit-net-0.0.4/scikit_net.egg-info/
+-rw-rw-rw-   0        0        0     2982 2023-05-28 19:28:26.000000 scikit-net-0.0.4/scikit_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-05-28 19:28:26.000000 scikit-net-0.0.4/scikit_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:28:26.000000 scikit-net-0.0.4/scikit_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-28 19:28:26.000000 scikit-net-0.0.4/scikit_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 19:28:26.000000 scikit-net-0.0.4/scikit_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:28:26.651248 scikit-net-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1778 2023-05-28 19:28:09.000000 scikit-net-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.632227 scikit-net-0.0.4/sknet/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.635227 scikit-net-0.0.4/sknet/network_construction/
+-rw-rw-rw-   0        0        0      482 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/__init__.py
+-rw-rw-rw-   0        0        0    31835 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/dataset_constructors.py
+-rw-rw-rw-   0        0        0     2471 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/general_constructors.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.637228 scikit-net-0.0.4/sknet/network_construction/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/tests/__init__.py
+-rw-rw-rw-   0        0        0    10630 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/tests/test_network_construction.py
+-rw-rw-rw-   0        0        0    11583 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/network_construction/time_series_constructors.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.639228 scikit-net-0.0.4/sknet/semi_supervised/
+-rw-rw-rw-   0        0        0       86 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/semi_supervised/__init__.py
+-rw-rw-rw-   0        0        0    10575 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/semi_supervised/modularity_label_propagation.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.641251 scikit-net-0.0.4/sknet/supervised/
+-rw-rw-rw-   0        0        0      179 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/__init__.py
+-rw-rw-rw-   0        0        0    12364 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/ease_of_access.py
+-rw-rw-rw-   0        0        0     9637 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/high_level_classification.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.644250 scikit-net-0.0.4/sknet/supervised/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/tests/__init__.py
+-rw-rw-rw-   0        0        0     6165 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/tests/test_ease_of_access.py
+-rw-rw-rw-   0        0        0     1631 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/supervised/tests/test_high_level_classification.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.645588 scikit-net-0.0.4/sknet/unsupervised/
+-rw-rw-rw-   0        0        0       90 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0    12078 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/unsupervised/stochastic_particle_competition.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:28:26.649093 scikit-net-0.0.4/sknet/utils/
+-rw-rw-rw-   0        0        0      191 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/utils/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/utils/low_level_models_handler.py
+-rw-rw-rw-   0        0        0     1037 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/utils/network_metrics_handler.py
+-rw-rw-rw-   0        0        0      472 2023-05-28 19:15:13.000000 scikit-net-0.0.4/sknet/utils/network_types_handler.py
```

### Comparing `scikit-net-0.0.3/LICENSE` & `scikit-net-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/PKG-INFO` & `scikit-net-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-net
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine Learning in Complex Networks
 Home-page: https://github.com/TNanukem/scikit-net
 Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
 Author: Tiago Toledo Jr
 Author-email: tiago.nanu@gmail.com
 License: MIT
 Keywords: Machine Learning,Complex Networks
```

### Comparing `scikit-net-0.0.3/README.md` & `scikit-net-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/scikit_net.egg-info/PKG-INFO` & `scikit-net-0.0.4/scikit_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-net
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine Learning in Complex Networks
 Home-page: https://github.com/TNanukem/scikit-net
 Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
 Author: Tiago Toledo Jr
 Author-email: tiago.nanu@gmail.com
 License: MIT
 Keywords: Machine Learning,Complex Networks
```

### Comparing `scikit-net-0.0.3/scikit_net.egg-info/SOURCES.txt` & `scikit-net-0.0.4/scikit_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/setup.py` & `scikit-net-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="scikit-net",
-    version="0.0.3",
+    version="0.0.4",
     description="Machine Learning in Complex Networks",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TNanukem/scikit-net",
     download_url='https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz',  # noqa: E501
     keywords=['Machine Learning', 'Complex Networks'],
     author="Tiago Toledo Jr",
```

### Comparing `scikit-net-0.0.3/sknet/network_construction/dataset_constructors.py` & `scikit-net-0.0.4/sknet/network_construction/dataset_constructors.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/network_construction/general_constructors.py` & `scikit-net-0.0.4/sknet/network_construction/general_constructors.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/network_construction/tests/test_network_construction.py` & `scikit-net-0.0.4/sknet/network_construction/tests/test_network_construction.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/network_construction/time_series_constructors.py` & `scikit-net-0.0.4/sknet/network_construction/time_series_constructors.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/semi_supervised/modularity_label_propagation.py` & `scikit-net-0.0.4/sknet/semi_supervised/modularity_label_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/supervised/ease_of_access.py` & `scikit-net-0.0.4/sknet/supervised/ease_of_access.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/supervised/high_level_classification.py` & `scikit-net-0.0.4/sknet/supervised/high_level_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/supervised/tests/test_ease_of_access.py` & `scikit-net-0.0.4/sknet/supervised/tests/test_ease_of_access.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/supervised/tests/test_high_level_classification.py` & `scikit-net-0.0.4/sknet/supervised/tests/test_high_level_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/unsupervised/stochastic_particle_competition.py` & `scikit-net-0.0.4/sknet/unsupervised/stochastic_particle_competition.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/utils/low_level_models_handler.py` & `scikit-net-0.0.4/sknet/utils/low_level_models_handler.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.3/sknet/utils/network_metrics_handler.py` & `scikit-net-0.0.4/sknet/utils/network_metrics_handler.py`

 * *Files identical despite different names*

