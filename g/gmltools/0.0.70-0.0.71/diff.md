# Comparing `tmp/gmltools-0.0.70.tar.gz` & `tmp/gmltools-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.70.tar", last modified: Sun May 28 12:02:06 2023, max compression
+gzip compressed data, was "gmltools-0.0.71.tar", last modified: Sun May 28 12:17:32 2023, max compression
```

## Comparing `gmltools-0.0.70.tar` & `gmltools-0.0.71.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.100188 gmltools-0.0.70/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.70/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.70/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-28 12:02:06.099183 gmltools-0.0.70/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.70/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:05.943919 gmltools-0.0.70/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.70/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.70/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.70/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-28 12:01:38.000000 gmltools-0.0.70/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 12:02:06.101192 gmltools-0.0.70/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-28 12:01:28.000000 gmltools-0.0.70/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:05.915436 gmltools-0.0.70/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:05.952047 gmltools-0.0.70/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.70/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.70/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.047808 gmltools-0.0.70/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.70/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    41440 2023-05-28 12:01:11.000000 gmltools-0.0.70/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.072370 gmltools-0.0.70/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.70/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.70/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.70/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.70/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.70/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.70/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.70/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.082578 gmltools-0.0.70/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.70/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.70/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.70/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.096157 gmltools-0.0.70/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.70/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.70/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.70/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.70/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:02:06.018540 gmltools-0.0.70/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-28 12:02:05.000000 gmltools-0.0.70/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-28 12:02:05.000000 gmltools-0.0.70/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 12:02:05.000000 gmltools-0.0.70/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-28 12:02:05.000000 gmltools-0.0.70/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 12:02:05.000000 gmltools-0.0.70/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.131543 gmltools-0.0.71/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.71/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.71/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-28 12:17:32.130547 gmltools-0.0.71/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.71/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.035800 gmltools-0.0.71/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.71/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.71/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.71/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-28 12:17:11.000000 gmltools-0.0.71/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:17:32.131543 gmltools-0.0.71/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-28 12:17:04.000000 gmltools-0.0.71/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.015890 gmltools-0.0.71/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.039827 gmltools-0.0.71/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.71/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.71/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.092528 gmltools-0.0.71/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.71/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    41821 2023-05-28 12:16:44.000000 gmltools-0.0.71/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.111755 gmltools-0.0.71/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.71/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.71/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.71/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.71/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.71/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.71/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.71/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.118853 gmltools-0.0.71/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.71/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.71/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.71/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.129549 gmltools-0.0.71/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.71/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.71/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.71/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.71/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:17:32.072957 gmltools-0.0.71/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-28 12:17:31.000000 gmltools-0.0.71/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-28 12:17:31.000000 gmltools-0.0.71/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:17:31.000000 gmltools-0.0.71/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-28 12:17:31.000000 gmltools-0.0.71/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 12:17:31.000000 gmltools-0.0.71/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.70/LICENSE` & `gmltools-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/Models.ipynb` & `gmltools-0.0.71/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/PKG-INFO` & `gmltools-0.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.70
+Version: 0.0.71
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.70/README.md` & `gmltools-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.71/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/gmltools.yml` & `gmltools-0.0.71/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/mltools.yml` & `gmltools-0.0.71/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/pyproject.toml` & `gmltools-0.0.71/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.70"
+version = "0.0.71"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.70/setup.py` & `gmltools-0.0.71/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.70',
+    'version': '0.0.71',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.70/src/gmltools/To_Do.txt` & `gmltools-0.0.71/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/eda/eda.py` & `gmltools-0.0.71/src/gmltools/eda/eda.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,15 +444,17 @@
     
 
 #--------------------------------------------------------PLOT DATA--------------------------------------------------------#
 class ExploreManager:
     def __init__(self,df):
         self.df=df
 
-    def plot_correlation(self, method='pearson', figsize=(1000,1000), colorscale='agsunset', title=None, title_size=24, label_size=14, save=False, save_path="./imgs/correlations/"):
+
+
+    def plot_correlation(self, method='pearson', figsize=(1000,1000), colorscale='agsunset', title=None, title_size=24, label_size=14, annotation_font_size=10, save=False, save_path="./imgs/correlations/"):
         """
         Plotly heatmap of the correlation matrix of a dataframe
 
         Parameters
         ----------
         df : pd.DataFrame
 
@@ -468,14 +470,17 @@
         
         title_size : int, optional
             The size of the plot's title. The default is 24.
 
         label_size : int, optional
             The size of the plot's labels. The default is 14.
 
+        annotation_font_size : int, optional
+            The size of the annotation's font inside the heatmap's cells. The default is 10.
+
         save : bool, optional
             Whether to save the plot as a file. The default is False.
 
         save_path : str, optional
             The path where to save the plot. The default is "./imgs/correlations/".
 
         Returns
@@ -483,23 +488,29 @@
         None.
         """
         assert isinstance(self.df, pd.DataFrame), "df must be a pd.DataFrame"
         assert isinstance(figsize, tuple), "figsize must be a tuple"
         assert isinstance(colorscale,str), "colorscale must be a str"
         
         fig = ff.create_annotated_heatmap(z=self.df.corr().values, 
-                                            x=self.df.corr().columns.tolist(), 
-                                            y=self.df.corr().columns.tolist(), 
-                                            annotation_text=self.df.corr().round(2).values, 
-                                            showscale=True)
+                                        x=self.df.corr().columns.tolist(), 
+                                        y=self.df.corr().columns.tolist(), 
+                                        annotation_text=self.df.corr().round(2).values, 
+                                        font_colors=['black'], 
+                                        showscale=True)
         fig.update_layout(title=title, 
-                            title_font=dict(size=title_size),
-                            xaxis=dict(tickfont=dict(size=label_size)),
-                            yaxis=dict(tickfont=dict(size=label_size)))
+                        title_font=dict(size=title_size),
+                        xaxis=dict(tickfont=dict(size=label_size)),
+                        yaxis=dict(tickfont=dict(size=label_size)))
         fig.update_traces(colorscale='agsunset')
+
+        # Increase annotation font size
+        for i in range(len(fig.layout.annotations)):
+            fig.layout.annotations[i].font.size = annotation_font_size
+
         fig.update_layout(width=figsize[0], height=figsize[1])
         fig.show()
 
         # Check if save is set to True
         if save:
             # Check if the directory exists
             if not os.path.exists(save_path):
@@ -508,14 +519,15 @@
 
             # Save the figure
             pio.write_image(fig, save_path + f'{title}_correlation_heatmap.png')
 
 
 
 
+
     def plot_distribution(self, bins:int=50, figsize:tuple=(600, 400), category_column=None, x_range=None, shared_yaxes:bool=False, shared_xaxes:bool=False, histnorm=None):
         """
         Plot the distribution of the numeric columns in the dataset. When category_column is provided, the distribution of each category is plotted 
         with the boxplot. Otherwise, the distribution of the entire dataset is plotted with the histogram. You can select the number of bins for the histogram.
         the range of the x-axis and the type of normalization for the histogram. histnorm="probability density" or None.
 
         Parameters
```

### Comparing `gmltools-0.0.70/src/gmltools/models/bayes.py` & `gmltools-0.0.71/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.71/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models/dummy_model.py` & `gmltools-0.0.71/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models/model.py` & `gmltools-0.0.71/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models/models_info.py` & `gmltools-0.0.71/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.71/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.71/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.71/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.71/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.71/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.71/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.70/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.71/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.70
+Version: 0.0.71
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.70/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.71/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

