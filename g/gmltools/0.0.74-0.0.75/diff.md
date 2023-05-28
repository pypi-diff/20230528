# Comparing `tmp/gmltools-0.0.74.tar.gz` & `tmp/gmltools-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.74.tar", last modified: Sun May 28 19:12:47 2023, max compression
+gzip compressed data, was "gmltools-0.0.75.tar", last modified: Sun May 28 20:00:25 2023, max compression
```

## Comparing `gmltools-0.0.74.tar` & `gmltools-0.0.75.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.873036 gmltools-0.0.74/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.74/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.74/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-28 19:12:47.871836 gmltools-0.0.74/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.74/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.778005 gmltools-0.0.74/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.74/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.74/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.74/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-28 19:12:15.000000 gmltools-0.0.74/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 19:12:47.873036 gmltools-0.0.74/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-28 19:12:05.000000 gmltools-0.0.74/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.744767 gmltools-0.0.74/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.783004 gmltools-0.0.74/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.74/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.74/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.833736 gmltools-0.0.74/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.74/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42863 2023-05-28 19:12:34.000000 gmltools-0.0.74/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.851316 gmltools-0.0.74/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.74/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.74/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.74/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.74/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.74/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.74/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.74/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.859247 gmltools-0.0.74/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.74/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.74/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.74/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.868816 gmltools-0.0.74/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.74/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.74/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.74/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.74/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:47.810893 gmltools-0.0.74/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-28 19:12:47.000000 gmltools-0.0.74/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-28 19:12:47.000000 gmltools-0.0.74/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:12:47.000000 gmltools-0.0.74/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-28 19:12:47.000000 gmltools-0.0.74/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 19:12:47.000000 gmltools-0.0.74/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.467955 gmltools-0.0.75/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.75/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.75/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-28 20:00:25.464958 gmltools-0.0.75/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.75/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.043456 gmltools-0.0.75/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.75/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.75/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.75/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-28 19:59:49.000000 gmltools-0.0.75/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 20:00:25.467955 gmltools-0.0.75/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-28 19:59:42.000000 gmltools-0.0.75/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:24.901303 gmltools-0.0.75/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.088387 gmltools-0.0.75/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.75/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.75/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.187967 gmltools-0.0.75/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.75/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    42993 2023-05-28 19:59:17.000000 gmltools-0.0.75/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.334186 gmltools-0.0.75/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.75/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.75/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.75/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.75/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.75/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.75/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.75/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.386561 gmltools-0.0.75/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.75/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.75/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.75/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.461433 gmltools-0.0.75/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.75/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.75/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.75/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.75/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.159505 gmltools-0.0.75/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.74/LICENSE` & `gmltools-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/Models.ipynb` & `gmltools-0.0.75/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/PKG-INFO` & `gmltools-0.0.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.74
+Version: 0.0.75
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.74/README.md` & `gmltools-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.75/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/gmltools.yml` & `gmltools-0.0.75/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/mltools.yml` & `gmltools-0.0.75/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/pyproject.toml` & `gmltools-0.0.75/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.74"
+version = "0.0.75"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.74/setup.py` & `gmltools-0.0.75/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.74',
+    'version': '0.0.75',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.74/src/gmltools/To_Do.txt` & `gmltools-0.0.75/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/eda/eda.py` & `gmltools-0.0.75/src/gmltools/eda/eda.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,15 @@
         if save:
             # Check if the directory exists
             if not os.path.exists(save_path):
                 # If the directory does not exist, create it
                 os.makedirs(save_path)
 
             # Save the figure
+            
             pio.write_image(fig, save_path + f'{title}_correlation_heatmap.png')
 
 
 
 
 
     def plot_distribution(self, bins:int=50, figsize:tuple=(600, 400), save_name="", category_column=None, x_range=None, shared_yaxes:bool=False, shared_xaxes:bool=False, histnorm=None, label_size:int=14, tick_size:int=12, title_size:int=16
@@ -590,15 +591,18 @@
             if save:
                 # Check if the directory exists
                 if not os.path.exists(save_path):
                     # If the directory does not exist, create it
                     os.makedirs(save_path)
 
                 # Save the figure
-                pio.write_image(hist, save_path + f'{col_}_dist_{save_name}.png')
+                # Save the figure
+                hist.write_image(save_path + f'{col_}_dist_{save_name}.png')
+
+                #pio.write_image(hist, save_path + f'{col_}_dist_{save_name}.png')
 
 
 
     def correlation_sum_combinations(self , target_var:str,remove_vars:list=None):
         """
         Funcion que devuelve la combinacion de variables sumadas que maximiza la correlacion con la variable objetivo
```

### Comparing `gmltools-0.0.74/src/gmltools/models/bayes.py` & `gmltools-0.0.75/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.75/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models/dummy_model.py` & `gmltools-0.0.75/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models/model.py` & `gmltools-0.0.75/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models/models_info.py` & `gmltools-0.0.75/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.75/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.75/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.75/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.75/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.75/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.75/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.74/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.75/src/gmltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.74
+Version: 0.0.75
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.74/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.75/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

