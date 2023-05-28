# Comparing `tmp/scikit-net-0.0.2.tar.gz` & `tmp/scikit-net-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-net-0.0.2.tar", last modified: Fri Oct 15 12:05:16 2021, max compression
+gzip compressed data, was "scikit-net-0.0.3.tar", last modified: Sun May 28 19:18:05 2023, max compression
```

## Comparing `scikit-net-0.0.2.tar` & `scikit-net-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:16.330746 scikit-net-0.0.2/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     2484 2021-10-15 12:05:16.326747 scikit-net-0.0.2/PKG-INFO
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     1660 2021-10-15 11:51:14.000000 scikit-net-0.0.2/README.md
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.010745 scikit-net-0.0.2/scikit_net.egg-info/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     2484 2021-10-15 12:04:56.000000 scikit-net-0.0.2/scikit_net.egg-info/PKG-INFO
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     1069 2021-10-15 12:04:57.000000 scikit-net-0.0.2/scikit_net.egg-info/SOURCES.txt
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)        1 2021-10-15 12:04:56.000000 scikit-net-0.0.2/scikit_net.egg-info/dependency_links.txt
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      210 2021-10-15 12:04:56.000000 scikit-net-0.0.2/scikit_net.egg-info/requires.txt
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)        6 2021-10-15 12:04:56.000000 scikit-net-0.0.2/scikit_net.egg-info/top_level.txt
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)       38 2021-10-15 12:05:16.333748 scikit-net-0.0.2/setup.cfg
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     1742 2021-10-15 12:04:04.000000 scikit-net-0.0.2/setup.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.045749 scikit-net-0.0.2/sknet/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/__init__.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.410748 scikit-net-0.0.2/sknet/network_construction/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      335 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)    24814 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/dataset_constructors.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     2471 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/general_constructors.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.560747 scikit-net-0.0.2/sknet/network_construction/tests/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/tests/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     4115 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/tests/test_network_construction.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     7546 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/network_construction/time_series_constructors.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.680743 scikit-net-0.0.2/sknet/semi_supervised/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)       86 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/semi_supervised/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     6404 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/semi_supervised/modularity_label_propagation.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.824747 scikit-net-0.0.2/sknet/supervised/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      179 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)    12323 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/ease_of_access.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     9637 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/high_level_classification.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:15.996744 scikit-net-0.0.2/sknet/supervised/tests/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/tests/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     2158 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/tests/test_ease_of_access.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     1285 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/supervised/tests/test_high_level_classification.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:16.076747 scikit-net-0.0.2/sknet/unsupervised/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)       90 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/unsupervised/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)    12078 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/unsupervised/stochastic_particle_competition.py
-drwxrwxrwx   0 tiago     (1000) tiago     (1000)        0 2021-10-15 12:05:16.247746 scikit-net-0.0.2/sknet/utils/
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      191 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/utils/__init__.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      939 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/utils/low_level_models_handler.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)     1037 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/utils/network_metrics_handler.py
--rwxrwxrwx   0 tiago     (1000) tiago     (1000)      472 2021-10-15 11:51:15.000000 scikit-net-0.0.2/sknet/utils/network_types_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.769550 scikit-net-0.0.3/
+-rw-rw-rw-   0        0        0     1097 2023-05-28 19:15:13.000000 scikit-net-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2982 2023-05-28 19:18:05.769550 scikit-net-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2403 2023-05-28 19:15:13.000000 scikit-net-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.663420 scikit-net-0.0.3/scikit_net.egg-info/
+-rw-rw-rw-   0        0        0     2982 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 19:18:05.000000 scikit-net-0.0.3/scikit_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:18:05.769550 scikit-net-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1778 2023-05-28 19:16:11.000000 scikit-net-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.664421 scikit-net-0.0.3/sknet/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.689931 scikit-net-0.0.3/sknet/network_construction/
+-rw-rw-rw-   0        0        0      482 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/__init__.py
+-rw-rw-rw-   0        0        0    31835 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/dataset_constructors.py
+-rw-rw-rw-   0        0        0     2471 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/general_constructors.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.696933 scikit-net-0.0.3/sknet/network_construction/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/tests/__init__.py
+-rw-rw-rw-   0        0        0    10630 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/tests/test_network_construction.py
+-rw-rw-rw-   0        0        0    11583 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/network_construction/time_series_constructors.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.708451 scikit-net-0.0.3/sknet/semi_supervised/
+-rw-rw-rw-   0        0        0       86 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/semi_supervised/__init__.py
+-rw-rw-rw-   0        0        0    10575 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/semi_supervised/modularity_label_propagation.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.723652 scikit-net-0.0.3/sknet/supervised/
+-rw-rw-rw-   0        0        0      179 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/__init__.py
+-rw-rw-rw-   0        0        0    12364 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/ease_of_access.py
+-rw-rw-rw-   0        0        0     9637 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/high_level_classification.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.733668 scikit-net-0.0.3/sknet/supervised/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/__init__.py
+-rw-rw-rw-   0        0        0     6165 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/test_ease_of_access.py
+-rw-rw-rw-   0        0        0     1631 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/supervised/tests/test_high_level_classification.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.744373 scikit-net-0.0.3/sknet/unsupervised/
+-rw-rw-rw-   0        0        0       90 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0    12078 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/unsupervised/stochastic_particle_competition.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:18:05.768488 scikit-net-0.0.3/sknet/utils/
+-rw-rw-rw-   0        0        0      191 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/low_level_models_handler.py
+-rw-rw-rw-   0        0        0     1037 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/network_metrics_handler.py
+-rw-rw-rw-   0        0        0      472 2023-05-28 19:15:13.000000 scikit-net-0.0.3/sknet/utils/network_types_handler.py
```

### Comparing `scikit-net-0.0.2/PKG-INFO` & `scikit-net-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-Metadata-Version: 2.1
-Name: scikit-net
-Version: 0.0.2
-Summary: Machine Learning in Complex Networks
-Home-page: https://github.com/TNanukem/scikit-net
-Author: Tiago Toledo Jr
-Author-email: tiago.nanu@gmail.com
-License: MIT
-Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
-Description: ![sknet Logo](https://github.com/TNanukem/sknet/blob/develop/docs/source/_static/full_logo.png "sknet Logo")
-        
-        ![Codecov branch](https://img.shields.io/codecov/c/github/tnanukem/sknet/develop?token=PIQ338YNK1)
-        
-        The sknet project is a scikit-learn and NetworkX compatible framework for machine learning in complex networks. It provides learning algorithms for complex networks, as well as transforming methods to turn tabular data into complex networks.
-        
-        It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning.
-        
-        ## :computer: Installation
-        
-        The sknet installation is available via PiPy:
-        
-            pip install scikit-net
-        
-        ## :high_brightness: Quickstart
-        
-        The following code snippet shows how one can transform tabular data into a complex network and then use it to create a classifier:
-        
-            from sklearn.datasets import load_iris
-            from sknet.network_construction import KNNConstructor
-            from sknet.supervised import EaseOfAccessClassifier
-        
-            X, y = load_iris(return_X_y = True)
-            X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
-        
-            # The constructor responsible for transforming the tabular data into a complex network
-            knn_c = KNNConstructor(k=5)
-        
-            classifier = EaseOfAccessClassifier()
-            classifier.fit(X_train, y_train, constructor=knn_c)
-            y_pred = classifier.predict(X_test)
-            accuracy_score(y_test, y_pred)
-        
-        ## :pencil: Documentation
-        
-        We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/sknet/
-        
-Keywords: Machine Learning,Complex Networks
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+![sknet Logo](https://github.com/TNanukem/sknet/blob/develop/docs/source/_static/full_logo.png "sknet Logo")
+
+![Codecov branch](https://img.shields.io/codecov/c/github/tnanukem/sknet/develop?token=PIQ338YNK1)
+
+The sknet project is a scikit-learn and NetworkX compatible framework for machine learning in complex networks. It provides learning algorithms for complex networks, as well as transforming methods to turn tabular data into complex networks.
+
+It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning. It main focus
+is to help researchers and students to develop solutions using machine learning on complex networks.
+
+## :computer: Installation
+
+The sknet installation is available via PiPy:
+
+    pip install scikit-net
+
+## :high_brightness: Quickstart
+
+The following code snippet shows how one can transform tabular data into a complex network and then use it to create a classifier:
+
+    from sklearn.model_selection import train_test_split
+    from sklean.metrics import accuracy_score
+    from sklearn.datasets import load_iris
+    from sknet.network_construction import KNNConstructor
+    from sknet.supervised import EaseOfAccessClassifier
+
+    X, y = load_iris(return_X_y = True)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
+
+    # The constructor responsible for transforming the tabular data into a complex network
+    knn_c = KNNConstructor(k=5)
+
+    classifier = EaseOfAccessClassifier()
+    classifier.fit(X_train, y_train, constructor=knn_c)
+    y_pred = classifier.predict(X_test)
+    accuracy_score(y_test, y_pred)
+
+## :pencil: Documentation
+
+We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/scikit-net/
+
+## Citation
+
+If you used the scikit-net on your research project, please cite us using the following publication:
+
+    @article{Toledo2021,
+    doi = {10.21105/joss.03864},
+    url = {https://doi.org/10.21105/joss.03864},
+    year = {2021},
+    publisher = {The Open Journal},
+    volume = {6},
+    number = {68},
+    pages = {3864},
+    author = {Tiago Toledo},
+    title = {sknet: A Python framework for Machine Learning in Complex Networks},
+    journal = {Journal of Open Source Software}
+    }
```

### Comparing `scikit-net-0.0.2/README.md` & `scikit-net-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,44 @@
+Metadata-Version: 2.1
+Name: scikit-net
+Version: 0.0.3
+Summary: Machine Learning in Complex Networks
+Home-page: https://github.com/TNanukem/scikit-net
+Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
+Author: Tiago Toledo Jr
+Author-email: tiago.nanu@gmail.com
+License: MIT
+Keywords: Machine Learning,Complex Networks
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![sknet Logo](https://github.com/TNanukem/sknet/blob/develop/docs/source/_static/full_logo.png "sknet Logo")
 
 ![Codecov branch](https://img.shields.io/codecov/c/github/tnanukem/sknet/develop?token=PIQ338YNK1)
 
 The sknet project is a scikit-learn and NetworkX compatible framework for machine learning in complex networks. It provides learning algorithms for complex networks, as well as transforming methods to turn tabular data into complex networks.
 
-It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning.
+It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning. It main focus
+is to help researchers and students to develop solutions using machine learning on complex networks.
 
 ## :computer: Installation
 
 The sknet installation is available via PiPy:
 
     pip install scikit-net
 
 ## :high_brightness: Quickstart
 
 The following code snippet shows how one can transform tabular data into a complex network and then use it to create a classifier:
 
+    from sklearn.model_selection import train_test_split
+    from sklean.metrics import accuracy_score
     from sklearn.datasets import load_iris
     from sknet.network_construction import KNNConstructor
     from sknet.supervised import EaseOfAccessClassifier
 
     X, y = load_iris(return_X_y = True)
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
 
@@ -29,8 +48,25 @@
     classifier = EaseOfAccessClassifier()
     classifier.fit(X_train, y_train, constructor=knn_c)
     y_pred = classifier.predict(X_test)
     accuracy_score(y_test, y_pred)
 
 ## :pencil: Documentation
 
-We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/sknet/
+We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/scikit-net/
+
+## Citation
+
+If you used the scikit-net on your research project, please cite us using the following publication:
+
+    @article{Toledo2021,
+    doi = {10.21105/joss.03864},
+    url = {https://doi.org/10.21105/joss.03864},
+    year = {2021},
+    publisher = {The Open Journal},
+    volume = {6},
+    number = {68},
+    pages = {3864},
+    author = {Tiago Toledo},
+    title = {sknet: A Python framework for Machine Learning in Complex Networks},
+    journal = {Journal of Open Source Software}
+    }
```

### Comparing `scikit-net-0.0.2/scikit_net.egg-info/PKG-INFO` & `scikit-net-0.0.3/scikit_net.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,72 @@
-Metadata-Version: 2.1
-Name: scikit-net
-Version: 0.0.2
-Summary: Machine Learning in Complex Networks
-Home-page: https://github.com/TNanukem/scikit-net
-Author: Tiago Toledo Jr
-Author-email: tiago.nanu@gmail.com
-License: MIT
-Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
-Description: ![sknet Logo](https://github.com/TNanukem/sknet/blob/develop/docs/source/_static/full_logo.png "sknet Logo")
-        
-        ![Codecov branch](https://img.shields.io/codecov/c/github/tnanukem/sknet/develop?token=PIQ338YNK1)
-        
-        The sknet project is a scikit-learn and NetworkX compatible framework for machine learning in complex networks. It provides learning algorithms for complex networks, as well as transforming methods to turn tabular data into complex networks.
-        
-        It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning.
-        
-        ## :computer: Installation
-        
-        The sknet installation is available via PiPy:
-        
-            pip install scikit-net
-        
-        ## :high_brightness: Quickstart
-        
-        The following code snippet shows how one can transform tabular data into a complex network and then use it to create a classifier:
-        
-            from sklearn.datasets import load_iris
-            from sknet.network_construction import KNNConstructor
-            from sknet.supervised import EaseOfAccessClassifier
-        
-            X, y = load_iris(return_X_y = True)
-            X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
-        
-            # The constructor responsible for transforming the tabular data into a complex network
-            knn_c = KNNConstructor(k=5)
-        
-            classifier = EaseOfAccessClassifier()
-            classifier.fit(X_train, y_train, constructor=knn_c)
-            y_pred = classifier.predict(X_test)
-            accuracy_score(y_test, y_pred)
-        
-        ## :pencil: Documentation
-        
-        We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/sknet/
-        
-Keywords: Machine Learning,Complex Networks
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: scikit-net
+Version: 0.0.3
+Summary: Machine Learning in Complex Networks
+Home-page: https://github.com/TNanukem/scikit-net
+Download-URL: https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz
+Author: Tiago Toledo Jr
+Author-email: tiago.nanu@gmail.com
+License: MIT
+Keywords: Machine Learning,Complex Networks
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![sknet Logo](https://github.com/TNanukem/sknet/blob/develop/docs/source/_static/full_logo.png "sknet Logo")
+
+![Codecov branch](https://img.shields.io/codecov/c/github/tnanukem/sknet/develop?token=PIQ338YNK1)
+
+The sknet project is a scikit-learn and NetworkX compatible framework for machine learning in complex networks. It provides learning algorithms for complex networks, as well as transforming methods to turn tabular data into complex networks.
+
+It started in 2021 as a project from volunteers to help to improve the development of research on the interface between complex networks and machine learning. It main focus
+is to help researchers and students to develop solutions using machine learning on complex networks.
+
+## :computer: Installation
+
+The sknet installation is available via PiPy:
+
+    pip install scikit-net
+
+## :high_brightness: Quickstart
+
+The following code snippet shows how one can transform tabular data into a complex network and then use it to create a classifier:
+
+    from sklearn.model_selection import train_test_split
+    from sklean.metrics import accuracy_score
+    from sklearn.datasets import load_iris
+    from sknet.network_construction import KNNConstructor
+    from sknet.supervised import EaseOfAccessClassifier
+
+    X, y = load_iris(return_X_y = True)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33)
+
+    # The constructor responsible for transforming the tabular data into a complex network
+    knn_c = KNNConstructor(k=5)
+
+    classifier = EaseOfAccessClassifier()
+    classifier.fit(X_train, y_train, constructor=knn_c)
+    y_pred = classifier.predict(X_test)
+    accuracy_score(y_test, y_pred)
+
+## :pencil: Documentation
+
+We provide an extensive API documentation as well with some user guides. The documentation is available on https://tnanukem.github.io/scikit-net/
+
+## Citation
+
+If you used the scikit-net on your research project, please cite us using the following publication:
+
+    @article{Toledo2021,
+    doi = {10.21105/joss.03864},
+    url = {https://doi.org/10.21105/joss.03864},
+    year = {2021},
+    publisher = {The Open Journal},
+    volume = {6},
+    number = {68},
+    pages = {3864},
+    author = {Tiago Toledo},
+    title = {sknet: A Python framework for Machine Learning in Complex Networks},
+    journal = {Journal of Open Source Software}
+    }
```

### Comparing `scikit-net-0.0.2/scikit_net.egg-info/SOURCES.txt` & `scikit-net-0.0.3/scikit_net.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 scikit_net.egg-info/PKG-INFO
 scikit_net.egg-info/SOURCES.txt
 scikit_net.egg-info/dependency_links.txt
 scikit_net.egg-info/requires.txt
 scikit_net.egg-info/top_level.txt
```

### Comparing `scikit-net-0.0.2/setup.py` & `scikit-net-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="scikit-net",
-    version="0.0.2",
+    version="0.0.3",
     description="Machine Learning in Complex Networks",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TNanukem/scikit-net",
     download_url='https://github.com/TNanukem/scikit-net/archive/refs/tags/v0.0.1.tar.gz',  # noqa: E501
     keywords=['Machine Learning', 'Complex Networks'],
     author="Tiago Toledo Jr",
@@ -23,15 +23,16 @@
         "Programming Language :: Python :: 3.8",
     ],
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     install_requires=['attrs',
                       'decorator',
                       'importlib-metadata',
-                      'iniconfig',
+                      'iniconfig'
+                      'giotto-tda',
                       'joblib',
                       'networkx',
                       'numpy',
                       'packaging',
                       'pandas',
                       'pluggy',
                       'py',
```

### Comparing `scikit-net-0.0.2/sknet/network_construction/dataset_constructors.py` & `scikit-net-0.0.3/sknet/network_construction/dataset_constructors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import networkx as nx
 
 from abc import ABCMeta, abstractmethod
+from sklearn.metrics import pairwise_distances
 from sklearn.neighbors import KDTree, BallTree
 
 
 class BaseConstructor(metaclass=ABCMeta):
     """
     This class allows to transform a dataset into a networkx
     complex network by using the several different transformation
@@ -47,15 +48,14 @@
         If by some reason the transformer is not fitted, this will generate
         an error.
 
         After the new nodes are added, one should use the get_network
         function to retrieve the network with the new nodes.
 
         """
-        pass
 
     def fit(self, X, y=None):
         """Fit the constructor creating the NetworkX graph
 
         Parameters
         ----------
         X : {array-like, pandas dataframe} of shape (n_samples, n_features)
@@ -179,15 +179,15 @@
     --------
     >>> from sklearn.datasets import load_iris
     >>> from dataset_constructors import KNNConstructor
     >>> X, y = load_iris(return_X_y = True)
     >>> knn_c = KNNConstructor(k=3)
     >>> knn_c.fit(X, y)
     >>> G = knn_c.transform()
-    >>> print(len(G.nodes))
+    >>> # print(len(G.nodes))
     150
 
     Notes
     -----
 
     References
     ----------
@@ -324,15 +324,15 @@
     --------
     >>> from sklearn.datasets import load_iris
     >>> from dataset_constructors import EpsilonRadiusConstructor
     >>> X, y = load_iris(return_X_y = True)
     >>> eps_c = EpsilonRadiusConstructor(epsilon=3)
     >>> eps_c.fit(X, y)
     >>> G = eps_c.transform()
-    >>> print(len(G.nodes))
+    >>> # print(len(G.nodes))
     150
 
     Notes
     -----
 
     References
     ----------
@@ -479,15 +479,15 @@
     --------
     >>> from sklearn.datasets import load_iris
     >>> from dataset_constructors import KNNEpislonRadiusConstructor
     >>> X, y = load_iris(return_X_y = True)
     >>> ke_c = KNNEpislonRadiusConstructor(k=3, epsilon=0.3)
     >>> ke_c.fit(X, y)
     >>> G = ke_c.transform()
-    >>> print(len(G.nodes))
+    >>> # print(len(G.nodes))
     150
 
     Notes
     -----
     The KNN is used for sparse regions while the Epsilon-Radius is used for
     dense regions. This approach hopes to overcome the limitations of the
     individual components, allowing for a better network construction. The
@@ -647,7 +647,199 @@
     # Low dimensional spaces are fit to KD-Tree
     if X.shape[1] < 30:
         return KDTree(X, leaf_size=leaf_size, metric=metric)
 
     # High dimensional spaces are fit to Ball Tree
     if X.shape[1] >= 30:
         return BallTree(X, leaf_size=leaf_size, metric=metric)
+
+
+class SingleLinkageHeuristicConstructor(BaseConstructor):
+    """
+    Use Single Linkage Heuristics to generate a complex network from
+    tabular data
+
+    Parameters
+    ----------
+    k : int, default=3
+        The number of closests points between two grops to be considered
+        to create an edge.
+    lambda_ : positive float, default=0.1
+        Multiplying factor on the average dissimilarity on the groups to
+        define the critical distance
+    sep_comp : boolean, default=True
+        If True and if y is not None, then each class of the dataset
+        will be a separated component, so nodes from one class will only
+        be connected to those of the same class. If False then this
+        restriction is not applied.
+    metric : str or DistanceMetric object, default='euclidean'
+        The distance metric to use for the neighborhood tree. Refer
+        to the DistanceMetric class documentation from sklearn for a list
+        of available metrics
+    n_jobs : int, default=None
+        The number of parallel jobs to run for neighbors search.
+        None means 1 unless in a joblib.parallel_backend context and -1 means
+        using all processors.
+
+    Examples
+    --------
+    >>> from sklearn.datasets import load_iris
+    >>> from dataset_constructors import SingleLinkageHeuristicConstructor
+    >>> X, y = load_iris(return_X_y = True)
+    >>> ch = SingleLinkageHeuristicConstructor(k=3, epsilon=0.3)
+    >>> ch.fit(X, y)
+    >>> G = ke_c.transform()
+    >>> # print(len(G.nodes))
+    150
+
+    References
+    ----------
+    Cupertino, T.H., Huertas, J., & Zhao, L. (2013). Data clustering using
+    controlled consensus in complex networks. Neurocomputing, 118, 132-140.
+
+    """
+    def __init__(self, k=3, lambda_=0.1, sep_comp=False,
+                 metric='euclidean', n_jobs=None):
+        self.k = k
+        self.lambda_ = lambda_
+        self.sep_comp = sep_comp
+        self.metric = metric
+        self.n_jobs = n_jobs
+
+    def get_params(self, deep=True):
+        return {'k': self.k, 'lambda_': self.lambda_,
+                'sep_comp': self.sep_comp,
+                'metric': self.metric, 'n_jobs': self.n_jobs}
+
+    def add_nodes(self, X, y=None):
+        """Add nodes to an existing network inside a fitted transformer
+        object
+
+        Parameters
+        ----------
+        X : {array-like, pandas dataframe} of shape (n_samples, n_features)
+            The input data.
+        y : {ndarray, pandas series}, shape (n_samples,) or
+        (n_samples, n_classes), default=None
+            The true classes.
+
+        Notes
+        -----
+        If y is set, then the class of each node will be inserted into
+        the node information under the label 'class'. If sep_comp is true
+        then each class will be a separated component of the network.
+
+        If by some reason the transformer is not fitted, this will generate
+        an error.
+
+        After the new nodes are added, one should use the get_network
+        function to retrieve the network with the new nodes.
+
+        """
+        if isinstance(X, pd.DataFrame) or isinstance(X, pd.Series):
+            X = np.array(X)
+
+        if self.lambda_ < 0:
+            raise Exception('lambda_ parameter should be positive')
+
+        if self.fitting:
+            self.G_ = nx.Graph()
+            self.groups_ = np.array([i for i in range(len(X))])
+        else:
+            self.groups_.extend(
+                [i + np.max(np.unique(self.groups)) for i in range(len(X))]
+            )
+            X = np.vstack((self.X_, X))
+
+        if y is None and self.sep_comp is True:
+            raise Exception(
+                """y parameter is required for separated construction,
+                set sep_comp to False"""
+            )
+
+        number_of_groups = len(self.groups_)
+
+        X_dist = pairwise_distances(X, metric=self.metric,
+                                    n_jobs=self.n_jobs)
+
+        while number_of_groups > 1:
+            if number_of_groups == len(X):
+                dist = X_dist
+
+            else:
+                dist = self._generate_new_X_dist(X_dist)
+
+            for i in range(dist.shape[0]):
+                dist[i, i] = np.inf
+
+            # Finds the two closest groups and get their values
+            i, j = np.unravel_index(dist.argmin(), dist.shape)
+
+            # If the two closest groups are the same, then find other pair
+            if self.groups_[i] == self.groups_[j]:
+                while self.groups_[i] == self.groups_[j]:
+                    dist[i][j] = np.inf
+                    i, j = np.unravel_index(dist.argmin(), dist.shape)
+
+            # Finds the nodes that are on the group i and j
+            g1 = np.where(self.groups_ == self.groups_[i])[0]
+            g1_idx = i
+
+            g2 = np.where(self.groups_ == self.groups_[j])[0]
+            g2_idx = j
+
+            # Finds the distance between all members of the group
+            g1_dists = pairwise_distances(X[g1])
+
+            g2_dists = pairwise_distances(X[g2])
+
+            # Finds the average intra-cluster dissimilarity
+            d1 = np.mean(g1_dists)
+            d2 = np.mean(g2_dists)
+
+            # Select the k most similar nodes between G1 and G2
+            group_distance = pairwise_distances(X[g1], X[g2])
+            candidates = []
+
+            if group_distance.shape[0] < self.k:
+                k = group_distance.shape[0]
+            else:
+                k = self.k
+
+            for i in range(k):
+                i, j = np.unravel_index(
+                    group_distance.argmin(), group_distance.shape
+                )
+                candidates.append((g1[i], g2[j]))
+                group_distance[i, j] = np.inf
+
+            # Generate edges
+            dc = self.lambda_ * max(d1, d2)
+
+            for u, v in candidates:
+                if self.sep_comp is True and y[u] != y[v]:
+                    continue
+                if dist[u, v] <= dc:
+                    self.G_.add_edge(u, v, weight=dist[u, v])
+
+            # Merge groups
+            self.groups_[
+                self.groups_ == self.groups_[g2_idx]] = self.groups_[g1_idx]
+
+            # Update number of groups
+            number_of_groups = len(np.unique(self.groups_))
+
+    def _generate_new_X_dist(self, X_dist):
+        number_of_groups = len(self.groups_)
+
+        new_X_dist = np.zeros((number_of_groups, number_of_groups))
+
+        # Find the distance between the two closest nodes for each group pair
+        for i in np.unique(self.groups_):
+            for j in np.unique(self.groups_):
+                if i != j:
+                    g1_nodes = np.where(self.groups_ == i)[0]
+                    g2_nodes = np.where(self.groups_ == j)[0]
+
+                    new_X_dist[i, j] = np.min(X_dist[g1_nodes, :][:, g2_nodes])
+
+        return new_X_dist
```

### Comparing `scikit-net-0.0.2/sknet/network_construction/general_constructors.py` & `scikit-net-0.0.3/sknet/network_construction/general_constructors.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.2/sknet/network_construction/time_series_constructors.py` & `scikit-net-0.0.3/sknet/network_construction/time_series_constructors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import warnings
 import pandas as pd
 import networkx as nx
 import numpy as np
 
 from scipy.stats import pearsonr
 from abc import ABCMeta, abstractmethod
+from sklearn.metrics import pairwise_distances
+from gtda.time_series import SingleTakensEmbedding
 
 
 class TimeSeriesBaseConstructor(metaclass=ABCMeta):
     """
     This class allows to transform a time series into a networkx
     complex network by using the several different transformation
     methods
 
     Do not use this abstract class, use derived classes instead
     """
-    def __init__(self):
-        pass
 
     def fit(self, X, y=None):
         """Fit the constructor creating the NetworkX graph
 
         Parameters
         ----------
         X : {array-like, pandas dataframe} of shape (n_samples, n_features)
@@ -69,15 +69,15 @@
             The network version of the inserted time series data
         """
         self.fit(X, y)
         return self.G_
 
     @abstractmethod
     def add_nodes(self, X, y=None):
-        pass
+        """Adds a node to the graph"""
 
     def set_params(self, **parameters):
         for parameter, value in parameters.items():
             setattr(self, parameter, value)
         return self
 
 
@@ -193,15 +193,15 @@
         The network version of the inserted time series data
 
     Examples
     --------
     >>> from sknet.network_construction import MultivariateCorrelationConstructor  # noqa: E501
     >>> r = 0.5
     >>> L = 10
-    >>> constructor = UnivariateCorrelationConstructor(r, L)
+    >>> constructor = MultivariateCorrelationConstructor(r, L)
     >>> constructor.fit(X)
     >>> G_ = constructor.transform()
 
     References
     ----------
     Silva, Thiago & Zhao, Liang. (2016). Machine Learning in
     Complex Networks. 10.1007/978-3-319-17290-3.
@@ -250,7 +250,116 @@
         # Make the D matrix
         C[C < self.r] = 0
         C[C >= self.r] = 1
 
         self.G_ = nx.from_numpy_array(C)
 
         self.X_ = X
+
+
+class UnivariateRecurrenceNetworkConstructor(TimeSeriesBaseConstructor):
+    """
+    Creates a networkX complex network from a univariate time series
+    by creating edges between recurrent (close) states on the phase space
+    of the series.
+
+    The phase space is constructed using the Takens Embedding Theorem.
+
+    Parameters
+    ----------
+    epsilon : float, optional (default=0.1)
+        The required distance between two states for them to be considered a
+        recurrence and hence be connected
+    d : int, optional (default=None)
+        The dimension of the embedding to be used for the Takens embedding.
+        If None and tau is also None, the best parameter will be
+        automatically chosen.
+    tau : int, optional (default=None)
+        The time delay to be used on the Takens Embedding. If None and
+        tau is also None, the best parameter will be automatically chosen.
+    metric : str, optional (default='euclidean')
+        The distance metric to be used to calculate the distance between
+        two points on the phase space
+    n_jobs : int, optional (default=None)
+        The number of parallel processes to be used when applying the
+        Takens embedding and when calculating the distances between the
+        states. None means 1 core will be used, -1 means use all cores.
+    Attributes
+    ----------
+    G_ : NetworkX graph
+        The network version of the inserted time series data
+
+    Examples
+    --------
+    >>> from sknet.network_construction import UnivariateRecurrenceNetworkConstructor  # noqa: E501
+    >>> constructor = UnivariateRecurrenceNetworkConstructor(10)
+    >>> constructor.fit(X)
+    >>> G_ = constructor.transform()
+
+    References
+    ----------
+    Donner, R.V., Zou, Y., Donges, J.F., Marwan, N., Kurths, J.: Recurrence
+    networks – a novel paradigm for nonlinear time series analysis.
+    New J. Phys. 12, 033025 (2010)
+
+    """
+    def __init__(self, epsilon=0.1, d=None, tau=None, metric='euclidean',
+                 n_jobs=None):
+        self.epsilon = epsilon
+        self.d = d
+        self.tau = tau
+        self.metric = metric
+        self.n_jobs = n_jobs
+
+    def get_params(self, deep=True):
+        return {'epsilon': self.epsilon, 'd': self.d, 'tau': self.tau,
+                'metric': self.metric, 'n_jobs': self.n_jobs}
+
+    def add_nodes(self, X, y=None):
+        """Add nodes to an existing network inside a fitted transformer
+        object
+
+        Parameters
+        ----------
+        X : {array-like, pandas dataframe} of shape (n_samples, n_features)
+            The input data.
+        y : ignored, used just for API convention
+        """
+        if isinstance(X, pd.DataFrame) or isinstance(X, pd.Series):
+            X = np.array(X)
+
+        if X.shape[1] > 1:
+            warnings.warn(
+                """More than one feature identified in the series.
+                   Recurrence should not be used on multivariate series"""
+            )
+
+        if self.X_ is not None:
+            X = np.vstack((self.X_, X))
+
+        # Generate the state space of the time series X
+        if self.d is None and self.tau is None:
+            takens_dict = {'parameters_type': 'search'}
+        else:
+            takens_dict = {'parameters_type': 'fixed', 'dimension': self.d,
+                           'time_delay': self.tau}
+
+        takens_dict['n_jobs'] = self.n_jobs
+
+        takens = SingleTakensEmbedding(**takens_dict)
+
+        space = takens.fit_transform(X)
+
+        # Get distance metric
+        R = pairwise_distances(space, metric=self.metric, n_jobs=self.n_jobs)
+
+        # Generate the recurrence matrix
+        R[R <= self.epsilon] = 1
+        R[R > self.epsilon] = 0
+
+        # Remove self-loops
+        for i in range(R.shape[0]):
+            R[i, i] = 0
+
+        self.G_ = nx.from_numpy_array(R)
+
+        self.X_ = X
```

### Comparing `scikit-net-0.0.2/sknet/supervised/ease_of_access.py` & `scikit-net-0.0.3/sknet/supervised/ease_of_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
             predictions.append(self._aggregation_method(self.tau_))
 
         return predictions
 
     @abstractmethod
     def _aggregation_method(self, tau):
-        pass
+        """Defines which aggregation method to use"""
 
     def _get_distance_metric(self):
         metric = self.constructor_.metric
 
         if type(metric) is str:
             return DistanceMetric.get_metric(metric)
```

### Comparing `scikit-net-0.0.2/sknet/supervised/high_level_classification.py` & `scikit-net-0.0.3/sknet/supervised/high_level_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.2/sknet/supervised/tests/test_ease_of_access.py` & `scikit-net-0.0.3/sknet/supervised/tests/test_high_level_classification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,52 @@
 import pytest
 import numpy as np
-import pandas as pd
 
 from sklearn.datasets import load_iris
 from sklearn.model_selection import train_test_split
 
 from sknet.network_construction import KNNConstructor
-from sknet.supervised import EaseOfAccessClassifier
+from sknet.supervised import HighLevelClassifier
 
 
 @pytest.fixture
 def X_y_generator():
 
     X, y = load_iris(return_X_y=True)
     X_train, X_test, y_train, y_test = train_test_split(X, y,
                                                         test_size=0.33,
                                                         random_state=42)
 
     return X_train, y_train, X_test, y_test
 
 
 @pytest.fixture
-def module_generator_eigen(X_y_generator):
+def module_generator(X_y_generator):
     knn = KNNConstructor(k=3)
-    classifier = EaseOfAccessClassifier(t=5)
+    classifier = HighLevelClassifier(
+        'random_forest', 0.5, [0.5, 0.5],
+        ['clustering_coefficient', 'assortativity']
+    )
     classifier.fit(X_y_generator[0], X_y_generator[1], constructor=knn)
 
     return classifier
 
 
-@pytest.fixture
-def module_generator_power(X_y_generator):
-    knn = KNNConstructor(k=3)
-    classifier = EaseOfAccessClassifier(t=5, method='power')
-    classifier.fit(X_y_generator[0], X_y_generator[1], constructor=knn)
-
-    return classifier
-
-
-@pytest.fixture
-def class_generator(module_generator_eigen,
-                    module_generator_power,
-                    X_y_generator):
-
-    pred_eig = module_generator_eigen.predict(X_y_generator[2])
-    pred_power = module_generator_power.predict(X_y_generator[2])
-
-    return module_generator_eigen, module_generator_power, pred_eig, pred_power
-
-
-def test__stationary_distribution(class_generator):
-    np.testing.assert_almost_equal(class_generator[0].P_inf,
-                                   class_generator[1].P_inf)
-
-    pd.testing.assert_frame_equal(class_generator[0].tau_,
-                                  class_generator[1].tau_)
+def test_predict(module_generator, X_y_generator):
 
+    expected = [1, 0, 2, 1, 1, 0, 1, 2, 1, 1, 2, 0, 0, 0, 0,
+                1, 2, 1, 1, 2, 0, 2, 0, 2, 2, 2, 2, 2, 0, 0,
+                0, 0, 1, 0, 0, 2, 1, 0, 0, 0, 2, 1, 1, 0, 0,
+                1, 1, 2, 1, 2]
+    pred = module_generator.predict(X_y_generator[2])
+    np.testing.assert_equal(expected, pred)
 
-def test_predictions(class_generator):
 
-    expected = [1, 0, 2, 1, 1, 0, 1, 2, 1, 1, 2, 0, 0, 0, 0, 1,
-                2, 1, 1, 2, 0, 1, 0, 2, 2, 2, 2, 2, 0, 0, 0, 0,
-                1, 0, 0, 1, 1, 0, 0, 0, 2, 1, 1, 0, 0, 1, 2, 2,
-                1, 2]
+def test_set_get_param(module_generator):
+    module_generator.set_params(p=0.2)
+    assert module_generator.get_params()['p'] == 0.2
 
-    eigen_pred = class_generator[2]
-    power_pred = class_generator[3]
 
-    assert eigen_pred == power_pred == expected
+def test_alpha_raise_on_fit(module_generator):
+    module_generator.set_params(alpha=[0.7, 0.9])
+    with pytest.raises(Exception):
+        module_generator.fit(X_y_generator[0], X_y_generator[1])
```

### Comparing `scikit-net-0.0.2/sknet/unsupervised/stochastic_particle_competition.py` & `scikit-net-0.0.3/sknet/unsupervised/stochastic_particle_competition.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.2/sknet/utils/low_level_models_handler.py` & `scikit-net-0.0.3/sknet/utils/low_level_models_handler.py`

 * *Files identical despite different names*

### Comparing `scikit-net-0.0.2/sknet/utils/network_metrics_handler.py` & `scikit-net-0.0.3/sknet/utils/network_metrics_handler.py`

 * *Files identical despite different names*

