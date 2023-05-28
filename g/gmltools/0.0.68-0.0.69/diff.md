# Comparing `tmp/gmltools-0.0.68.tar.gz` & `tmp/gmltools-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.68.tar", last modified: Sun May 28 11:48:53 2023, max compression
+gzip compressed data, was "gmltools-0.0.69.tar", last modified: Sun May 28 11:50:14 2023, max compression
```

## Comparing `gmltools-0.0.68.tar` & `gmltools-0.0.69.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.969634 gmltools-0.0.68/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.68/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.68/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-28 11:48:53.968670 gmltools-0.0.68/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.68/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.594081 gmltools-0.0.68/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.68/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.68/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.68/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-28 11:48:16.000000 gmltools-0.0.68/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 11:48:53.969634 gmltools-0.0.68/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-28 11:48:08.000000 gmltools-0.0.68/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.468820 gmltools-0.0.68/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.626632 gmltools-0.0.68/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.68/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.68/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.724085 gmltools-0.0.68/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.68/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    41232 2023-05-28 11:47:05.000000 gmltools-0.0.68/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.855897 gmltools-0.0.68/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.68/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.68/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.68/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.68/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.68/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.68/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.68/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.901753 gmltools-0.0.68/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.68/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.68/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.68/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.965757 gmltools-0.0.68/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.68/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.68/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.68/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.68/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:48:53.692422 gmltools-0.0.68/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-28 11:48:52.000000 gmltools-0.0.68/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-28 11:48:53.000000 gmltools-0.0.68/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:48:52.000000 gmltools-0.0.68/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-28 11:48:52.000000 gmltools-0.0.68/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 11:48:52.000000 gmltools-0.0.68/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.149604 gmltools-0.0.69/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.69/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.69/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-28 11:50:14.149604 gmltools-0.0.69/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.69/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.034251 gmltools-0.0.69/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.69/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.69/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.69/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-28 11:49:47.000000 gmltools-0.0.69/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:50:14.150570 gmltools-0.0.69/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-28 11:49:39.000000 gmltools-0.0.69/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:13.995373 gmltools-0.0.69/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.040267 gmltools-0.0.69/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.69/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.69/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.100677 gmltools-0.0.69/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.69/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    41232 2023-05-28 11:47:05.000000 gmltools-0.0.69/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.123604 gmltools-0.0.69/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.69/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.69/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.69/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.69/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.69/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.69/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.69/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.133569 gmltools-0.0.69/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.69/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.69/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.69/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.146614 gmltools-0.0.69/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.69/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.69/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.69/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.69/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:50:14.095765 gmltools-0.0.69/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-28 11:50:13.000000 gmltools-0.0.69/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-28 11:50:13.000000 gmltools-0.0.69/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:50:13.000000 gmltools-0.0.69/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-28 11:50:13.000000 gmltools-0.0.69/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 11:50:13.000000 gmltools-0.0.69/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.68/LICENSE` & `gmltools-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/Models.ipynb` & `gmltools-0.0.69/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/PKG-INFO` & `gmltools-0.0.69/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.68
+Version: 0.0.69
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.68/README.md` & `gmltools-0.0.69/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.69/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/gmltools.yml` & `gmltools-0.0.69/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/mltools.yml` & `gmltools-0.0.69/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/pyproject.toml` & `gmltools-0.0.69/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.68"
+version = "0.0.69"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.68/setup.py` & `gmltools-0.0.69/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.68',
+    'version': '0.0.69',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.68/src/gmltools/To_Do.txt` & `gmltools-0.0.69/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/eda/eda.py` & `gmltools-0.0.69/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/bayes.py` & `gmltools-0.0.69/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.69/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/dummy_model.py` & `gmltools-0.0.69/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/model.py` & `gmltools-0.0.69/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/models_info.py` & `gmltools-0.0.69/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.69/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.69/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.69/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.69/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.69/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.69/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.68/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.69/src/gmltools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.68
+Version: 0.0.69
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.68/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.69/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

