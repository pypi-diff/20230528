# Comparing `tmp/RobustifyToolkit-0.1.0.tar.gz` & `tmp/RobustifyToolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobustifyToolkit-0.1.0.tar", last modified: Thu May 25 20:27:30 2023, max compression
+gzip compressed data, was "RobustifyToolkit-0.1.1.tar", last modified: Sat May 27 21:57:47 2023, max compression
```

## Comparing `RobustifyToolkit-0.1.0.tar` & `RobustifyToolkit-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/robustify/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/robustify/noise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise_corruptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/robustify/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_scorers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_gaussianNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_poissonNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_scikt-learn_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_tensorflow_keras_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.747047 RobustifyToolkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-27 21:57:47.747047 RobustifyToolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.743047 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-27 21:57:47.000000 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-27 21:57:47.000000 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 21:57:47.000000 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-27 21:57:47.000000 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 21:57:47.000000 RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.743047 RobustifyToolkit-0.1.1/robustify/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.743047 RobustifyToolkit-0.1.1/robustify/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/noise/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/noise/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/noise_corruptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.747047 RobustifyToolkit-0.1.1/robustify/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/robustify/utils/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 21:57:47.747047 RobustifyToolkit-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:47.747047 RobustifyToolkit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_gaussianNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_poissonNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_scikt-learn_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_tensorflow_keras_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-27 21:57:38.000000 RobustifyToolkit-0.1.1/tests/test_transform.py
```

### Comparing `RobustifyToolkit-0.1.0/LICENSE` & `RobustifyToolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/PKG-INFO` & `RobustifyToolkit-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `RobustifyToolkit-0.1.0/README.md` & `RobustifyToolkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/PKG-INFO` & `RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/SOURCES.txt` & `RobustifyToolkit-0.1.1/RobustifyToolkit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,11 +19,13 @@
 robustify/utils/_progress.py
 robustify/utils/_sampling.py
 robustify/utils/_scorers.py
 robustify/utils/_train.py
 robustify/utils/_transform.py
 tests/__init__.py
 tests/test_gaussianNoise.py
+tests/test_importances.py
 tests/test_poissonNoise.py
 tests/test_sampling.py
 tests/test_scikt-learn_compatibility.py
-tests/test_tensorflow_keras_compatibility.py
+tests/test_tensorflow_keras_compatibility.py
+tests/test_transform.py
```

### Comparing `RobustifyToolkit-0.1.0/robustify/noise/continuous.py` & `RobustifyToolkit-0.1.1/robustify/noise/continuous.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/robustify/noise/discrete.py` & `RobustifyToolkit-0.1.1/robustify/noise/discrete.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/robustify/noise_corruptions.py` & `RobustifyToolkit-0.1.1/robustify/noise_corruptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,29 @@
 from .utils._importances import filter_on_importance_method
 from .utils._scorers import get_scorer
 from .utils._train import reset_model, train_model, train_baseline
 from .utils._filter import filter_on_method, get_levels
 from .utils._progress import initialize_progress_bar
 from .utils._transform import df_from_array, check_corruptions, fill_missing_columns
 
-
 def set_random_seed(random_state):
     """ Set random seed for different packages
     Parameters
     ----------
     random_state: int, RandomState instance or None, deafult=None Controls
     randomness external packages
     """
     np.random.seed(random_state)
     random.seed(random_state)
     tf.random.set_seed(random_state)
 
 def corrupt_data(model, corruption_list, X_train, X_test, scorer, y_train=None,
                  y_test=None, column_names=None, label_name=None, measure=None,
                  n_corruptions=10, random_state=None, custom_train=None, 
-                 custom_predict=None, plot=True):
+                 custom_predict=None, show_plots=True):
     """ Perform noise corruption on tabular data.
 
     Parameters
     ----------
     model: object
         An object which manages the estimation and decoding of a model. Must
         either provide a fit and predict method, or these will have to be
@@ -76,16 +75,17 @@
         not included in X_test as a feature.
 	
     column_names: list, default=None
         List of column names for input samples. Values defaults to index values
         if None. Not required if X_train is a dataframe with column names.
 	
     label_name: str or int, deafult=None
-        Column name or column index corresponding to the target values. Required
-        if y_train or y_test are None.
+        Column name or column index corresponding to the target values. Required 
+        if y_train or y_test are None and X_train is a DataFrame containg the 
+        target values.
 	
     measure: {None, "eli5", "lime", "shap"}, default=None
         If None default is either coef_ or feature_importances_ attributes where
         applicable, or permutation importance. Not available for models that use
         custom fit or predict methods. See further explanation of the other
         methods <link>here.
 	
@@ -106,33 +106,39 @@
           object has fit method with signature fit(X, y).
 	
     custom_predict: callable, default=None
         Callable with signature predict_func(model, X). Must return list,
         ndarray, tensor, or dataframe of same length as X. Not required if model
         object has predict method with signature predict(X).
 	
-    plot: bool, default=True
+    show_plots: bool, default=True
         Determines whether plots of feature importances, variance and score are
         shown. 
           
     Returns
     -------
 	result: Bunch or dict of such instances.
         Dictionary-like object, with the following attributes: corrupted_df:
         DataFrame
             The noisy data as a result of all corruptions specified in
             corruption_list. If levels are specified as a range or list of
             values, corrupted_df will be a result of the final level.
         corruption_result: DataFrame
             The value, variance and score (as defined by the scorer) for each
             feature and each level specified in corruption_list.
+        value_plot: Figure
+            A plot showing the average value of the specified features for each noise corruption. 
+        variance_plot: Figure
+            A plot showing the average variance of the value of the specified features for each noise corruption. 
+        score_plot: Figure
+            A plot showing the average score of the specified features for each noise corruption. 
     """
     set_random_seed(random_state)
-    df_train = df_from_array(X_train, column_names, y_train, label_name)
-    X_test = df_from_array(X_test, column_names)
+    df_train, label_name = df_from_array(X_train, column_names, y_train, label_name)
+    X_test, _ = df_from_array(X_test, column_names)
     corruption_list = check_corruptions(df_train, corruption_list)
     progress_bar = initialize_progress_bar(corruption_list, n_corruptions, df_train)
     corrupted_df = pd.DataFrame(columns=list(df_train))
     baseline_results, label_name = train_baseline(df_train, X_test, y_test, model,
                                                   scorer, measure, label_name, random_state,
                                                   custom_train, custom_predict)
     progress_bar.update(1)
@@ -148,21 +154,26 @@
                                                                 random_state, progress_bar, custom_train,
                                                                 custom_predict)
         corruption_results = pd.concat([corruption_results, corruption_result])
 
         for column_name in list(method_corrupt_df):
             corrupted_df[column_name] = method_corrupt_df[column_name].values
 
-    if plot:
-        plot_data(baseline_results, corruption_results, str(model), n_corruptions,
+    
+    value_plot, variance_plot, score_plot = plot_data(baseline_results, corruption_results, str(model), n_corruptions,
                   measured_property, corruption_list)
+    if show_plots:
+        value_plot.show()
+        variance_plot.show()
+        score_plot.show()
+        
     corrupted_df = fill_missing_columns(corrupted_df, df_train)
     progress_bar.close()
     corruption_results = corruption_results.sort_values(by=['feature_name', 'level'])
-    result = Bunch(corrupted_df=corrupted_df, corruption_result=corruption_result)
+    result = Bunch(corrupted_df=corrupted_df, corruption_result=corruption_result, value_plot=value_plot, variance_plot=variance_plot, score_plot=score_plot)
     return result
 
 def perform_corruption(df_train, X_test, y_test, model, scorer, measure, method,
                        randomlist, label_name, random_state, progress_bar,
                        custom_train, custom_predict):
     """ Perfroms a specific noise corruption on features.
```

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/__init__.py` & `RobustifyToolkit-0.1.1/robustify/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_filter.py` & `RobustifyToolkit-0.1.1/robustify/utils/_filter.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_importances.py` & `RobustifyToolkit-0.1.1/robustify/utils/_importances.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sklearn.inspection import permutation_importance
 from eli5.sklearn import PermutationImportance
 from eli5.permutation_importance import get_score_importances
 from lime import lime_tabular
 import shap
 
 def filter_on_importance_method(model, index, X, y, random_state, scoring, measure, custom_predict):
+    if measure: measure = measure.lower()
     switcher = {
         None: lambda: check_for_deafult_properties(model, index, X, y, random_state, scoring),
         'eli5': lambda: calculate_eli5_importances(model, index, X, y, random_state, scoring),
         'shap': lambda: calculate_shap_importances(model, index, X),
         'lime': lambda: calculate_lime_importances(model, index, X, custom_predict)
     }
     return switcher.get(measure, lambda:
```

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_plot.py` & `RobustifyToolkit-0.1.1/robustify/utils/_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,27 @@
                                           corruption_results['feature_name'].isin(features)]])
         else:
             bar_list.append(corruption)
             df_plot_bar = pd.concat([df_plot_bar,
                                      corruption_results[
                                          corruption_results['feature_name'].isin(features)]])
     if len(line_list) > 0:
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+        fig_1 = plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
                                measured_property, 'value', line_list)
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+        fig_2 = plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
                                measured_property, 'variance', line_list)
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+        fig_3 = plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
                                measured_property,'score', line_list)
     if len(bar_list) > 0:
-        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
+        fig_1 = plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
                                     measured_property, 'value', bar_list)
-        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
+        fig_2 = plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
                                     measured_property, 'variance', bar_list)
-        plot_corruption_scores_hist(baseline_results, df_plot_bar, model_name, corruptions, 'score')
+        fig_3 = plot_corruption_scores_hist(baseline_results, df_plot_bar, model_name, corruptions, 'score')
+    return fig_1, fig_2, fig_3
 
 def get_colors_from_fig(fig):
     colors = []
     f = fig.full_figure_for_development(warn=False)
     f.for_each_trace(lambda t: colors.append(t.marker.color))
     return colors
 
@@ -103,15 +104,15 @@
                                              corruption_results['feature_name'].unique().tolist())
     fig.update_layout(dict(updatemenus=buttons), xaxis_title="Feature",
                       yaxis_title=measured_property, title=title, font=dict(size=18))
     if measured_name == "score":
         fig.add_hline(y=baseline_results[measured_name].iloc[0], line_dash="dash", line_width=4)
     else:
         fig.update_traces(visible=False, selector=lambda t: not t.name in visible_features)
-    fig.show()
+    return fig
 
 def plot_corruption_values_hist(baseline_results, corruption_results, model_name,
                                 corruptions, measured_property, measured_name, corruptions_list):
     title = "Average {} of {} for features for {} over {} noise corruptions".format(
         measured_name.replace("_", " "), measured_property, model_name, corruptions)
     results = pd.DataFrame(columns=['feature_name', measured_name, measured_name +'_noisy'])
     order = corruption_results['feature_name'].unique().tolist()
@@ -150,15 +151,15 @@
               title=title,
               xaxis_title="Feature",
               yaxis_title=measured_property,
               font={"size":18},
               bargroupgap=0,
               barmode='group')
     fig.update_traces(visible=False, selector=lambda t: not t.name in visible_features)
-    fig.show()
+    return fig
 
 def plot_corruption_scores_hist(baseline_results, corruption_results, model_name,
                                 corruptions, measured_name):
     title = "Average {} for {} over {} noise corruptions".format(
         measured_name.replace("_", " "), model_name, corruptions)
     results = pd.DataFrame(columns=['feature_name', measured_name])
     baseline_results = baseline_results.sort_values("feature_name")
@@ -201,8 +202,8 @@
             yanchor="top"),],),
             title=title,
             xaxis_title="Feature",
             yaxis_title=measured_name,
             font={"size": 18},
             yaxis_range=[results[measured_name].min() - score_diff,
                          results[measured_name].max() + score_diff])
-    fig.show()
+    return fig
```

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_predict.py` & `RobustifyToolkit-0.1.1/robustify/utils/_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             y_pred = custom_predict(model, X)
             verify_predictions(X, y_pred, custom_predict)
             return convert_to_numpy(y_pred)
         except Exception:
             raise
     else:
         try:
-            y_pred = model.predict(X)
+            y_pred = model.predict(X.values)
             return convert_to_numpy(y_pred)
         except Exception:
             raise
 
 def verify_predictions(X, y_pred,custom_predict):
     if y_pred is None:
         raise TypeError("No predictions produced by method {}".format(custom_predict.__name__))
```

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_scorers.py` & `RobustifyToolkit-0.1.1/robustify/utils/_scorers.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.1.0/robustify/utils/_train.py` & `RobustifyToolkit-0.1.1/robustify/utils/_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return custom_train(model, X, y)
     except:
         raise Exception("Could not train the model")
 
 def train_model(model, X, y, custom_train):
     if custom_train != None:
         return custom_train_model(model, X, y, custom_train)  
-    model.fit(X, y.values.ravel())
+    model.fit(X.values, y.values.ravel())
     return model
 
 def reset_model(model):
     if isinstance(model, nn.Conv2d):
         torch.nn.init.xavier_uniform(model.weight.data)
     return model
```

### Comparing `RobustifyToolkit-0.1.0/setup.py` & `RobustifyToolkit-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 from setuptools import find_packages, setup
 setup(
     name='RobustifyToolkit',
     packages=find_packages(include=['robustify', 'robustify.noise', 'robustify.utils', 'tests']),
-    version='0.1.0',
+    version='0.1.1',
     readme="README.md",
     description="Robustify:" ,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Isabel Foster',
     license='MIT',
     classifiers=[
@@ -41,8 +41,8 @@
                       'lime',
                       'shap',
                       'torch'],
     setup_requires=['pytest-runner'], 
     tests_require=['pytest==7.3.1'],
     test_suite='tests',
 )
-    
+
```

### Comparing `RobustifyToolkit-0.1.0/tests/test_gaussianNoise.py` & `RobustifyToolkit-0.1.1/tests/test_gaussianNoise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from robustify import gaussian_noise
 import numpy as np
 import pandas as pd
 
-df = pd.read_csv('tests/test_column_gaussian.csv', index_col=0)
+df = pd.read_csv('tests/resources/test_column_gaussian.csv', index_col=0)
 test_data = df['jet_1_pt'].values
 
 def test_gaussian_average_value_0():
     percentage = 0.0
     noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (average_percentagee == 0)
```

### Comparing `RobustifyToolkit-0.1.0/tests/test_poissonNoise.py` & `RobustifyToolkit-0.1.1/tests/test_poissonNoise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from robustify import poisson_noise
 import numpy as np
 import pandas as pd
 
-df = pd.read_csv('tests/test_column_poission.csv', index_col=0)
+df = pd.read_csv('tests/resources/test_column_poission.csv', index_col=0)
 test_data = df['jet_n'].values
 
 def test_poisson_random_state_is_set():
     noisy_data_1 = poisson_noise(test_data, random_state=10)
     noisy_data_2 = poisson_noise(test_data, random_state=10)
     assert (sorted(noisy_data_1) == sorted(noisy_data_2))
```

### Comparing `RobustifyToolkit-0.1.0/tests/test_scikt-learn_compatibility.py` & `RobustifyToolkit-0.1.1/tests/test_scikt-learn_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,27 @@
                        'accuracy',
                        y_train_classification, 
                        y_test_classification,  
                        column_names=['sepal_length', 'sepal_width', 'petal_length', 'petal_width'], 
                        label_name='species', 
                        n_corruptions=10,
                        random_state=10, 
-                       plot=False)
+                       show_plots=False)
 
 def run_corruption_regression(model):
     return corrupt_data(model,
                        corruption_list_regression, 
                        X_train_regression, 
                        X_test_regression, 
                        "r2",
                        y_train_regression,
                        y_test_regression,
                        n_corruptions=10,
                        random_state=10,
-                       plot=False)
+                       show_plots=False)
 
 def test_linear_model_regression():
     model = linear_model.LinearRegression()
     result = run_corruption_regression(model)
     assert (result.corrupted_df is not None)
     assert (result.corruption_result is not None)
     assert (result.corruption_result.isnull().values.any() == False)
```

### Comparing `RobustifyToolkit-0.1.0/tests/test_tensorflow_keras_compatibility.py` & `RobustifyToolkit-0.1.1/tests/test_tensorflow_keras_compatibility.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,30 +31,30 @@
                        'r2', 
                        y_train_classification, 
                        y_test_classification, 
                        column_names=['sepal_length', 'sepal_width', 'petal_length', 'petal_width'],
                        label_name='species', 
                        n_corruptions=10,
                        random_state=10, 
-                       plot=False)
+                       show_plots=False)
 
 def run_corruption_regression(model):
     return corrupt_data(model,
                        corruption_list_regression,  
                        X_train_regression, 
                        X_test_regression,
                        "r2",
                        y_train_regression,
                        y_test_regression,
                        ['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6'],
                        'diabetes',
                        "eli5",
                        10,
                        random_state=10,
-                       plot=False)
+                       show_plots=False)
 
 def test_tensorflow_is_reproducible():
     model_1 = tf.keras.Sequential([
     layers.Dense(units=1)
     ])
     model_1.compile(
     optimizer=tf.keras.optimizers.Adam(learning_rate=0.1),
```

