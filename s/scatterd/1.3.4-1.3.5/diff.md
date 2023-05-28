# Comparing `tmp/scatterd-1.3.4.tar.gz` & `tmp/scatterd-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.3.4.tar", last modified: Sat May 27 20:53:37 2023, max compression
+gzip compressed data, was "scatterd-1.3.5.tar", last modified: Sun May 28 21:15:12 2023, max compression
```

## Comparing `scatterd-1.3.4.tar` & `scatterd-1.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 20:53:37.505298 scatterd-1.3.4/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-05-27 20:53:37.505298 scatterd-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 20:53:37.496293 scatterd-1.3.4/scatterd/
--rw-rw-rw-   0        0        0     1790 2023-05-27 20:50:53.000000 scatterd-1.3.4/scatterd/__init__.py
--rw-rw-rw-   0        0        0     7314 2023-05-27 20:14:36.000000 scatterd-1.3.4/scatterd/examples.py
--rw-rw-rw-   0        0        0    22320 2023-05-27 20:25:37.000000 scatterd-1.3.4/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:53:37.504284 scatterd-1.3.4/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-05-27 20:53:37.000000 scatterd-1.3.4/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-27 20:53:37.000000 scatterd-1.3.4/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 20:53:37.000000 scatterd-1.3.4/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-27 20:53:37.000000 scatterd-1.3.4/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 20:53:37.000000 scatterd-1.3.4/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-05-27 20:53:37.510302 scatterd-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-05-27 20:51:23.000000 scatterd-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.035347 scatterd-1.3.5/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-05-28 21:15:12.036345 scatterd-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.010876 scatterd-1.3.5/scatterd/
+-rw-rw-rw-   0        0        0     1831 2023-05-28 18:52:48.000000 scatterd-1.3.5/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     7314 2023-05-27 20:14:36.000000 scatterd-1.3.5/scatterd/examples.py
+-rw-rw-rw-   0        0        0    21289 2023-05-28 20:59:17.000000 scatterd-1.3.5/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.034350 scatterd-1.3.5/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-05-28 21:15:12.051439 scatterd-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-05-27 20:51:23.000000 scatterd-1.3.5/setup.py
```

### Comparing `scatterd-1.3.4/LICENSE` & `scatterd-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.4/PKG-INFO` & `scatterd-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.4
+Version: 1.3.5
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.4.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.4 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.5 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.4.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.4/README.md` & `scatterd-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.4/scatterd/__init__.py` & `scatterd-1.3.5/scatterd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing
+from scatterd.scatterd import scatterd, import_example, set_colors, _preprocessing, jitter_func, normalize_between_0_and_1
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.3.4'
+__version__ = '1.3.5'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Scatterd is an easy and fast way of creating beautiful scatter plots.
```

### Comparing `scatterd-1.3.4/scatterd/examples.py` & `scatterd-1.3.5/scatterd/examples.py`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.4/scatterd/scatterd.py` & `scatterd-1.3.5/scatterd/scatterd.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,80 +314,64 @@
             opaque = np.maximum(c_rgb[:, -1], 0.1)
             c_rgb = c_rgb[:, :3]
 
     # Return
     return c_rgb, opaque
 
 
-# %% Create gradient based on density.
-# def gradient_on_density_color(X, c_rgb, labels, showfig=False):
-#     """Set gradient on density color."""
-#     if labels is None: labels = np.repeat(0, X.shape[0])
-#     from scipy.stats import gaussian_kde
-#     uilabels = np.unique(labels)
-#     # density_colors = np.repeat([1., 1., 1.], len(labels), axis=0).reshape(-1, 3)
-#     density_colors = np.ones_like(c_rgb)
-
-#     if (len(uilabels)!=len(labels)):
-#         for label in uilabels:
-#             idx = np.where(labels==label)[0]
-#             if X.shape[1]==2:
-#                 xy = np.vstack([X[idx, 0], X[idx, 1]])
-#             else:
-#                 xy = np.vstack([X[idx, 0], X[idx, 1], X[idx, 2]])
-
-#             try:
-#                 # Compute density
-#                 z = gaussian_kde(xy)(xy)
-#                 # Sort on density
-#                 didx = idx[np.argsort(z)[::-1]]
-#             except:
-#                 didx=idx
-
-#             # order colors correctly based Density
-#             density_colors[didx] = c_rgb[idx, :]
-
-#             if showfig:
-#                 plt.figure()
-#                 fig, ax = plt.subplots(1,2, figsize=(20,10))
-#                 ax[0].scatter(X[didx,0], X[didx,1], color=c_rgb[idx, 0:3], alpha=c_rgb[idx, 3], edgecolor='#000000')
-#                 ax[1].scatter(idx, idx, color=c_rgb[idx, 0:3], alpha=c_rgb[idx, 3], edgecolor='#000000')
+# %% Jitter
+def jitter_func(x, jitter=0.01):
+    """Add jitter to data.
+
+    Noise is generated from random normal distribution and added to the data.
+
+    Parameters
+    ----------
+    x : numpy array
+        input data.
+    jitter : float, optional
+        Strength of generated noise. The default is 0.01.
+
+    Returns
+    -------
+    x : array-like
+        Data including noise.
 
-#         c_rgb=density_colors
-
-#     # Return
-#     return c_rgb
+    """
+    if jitter is None or jitter is False: jitter=0
+    if jitter is True: jitter=0.01
+    if jitter>0 and x is not None:
+        x = x + np.random.normal(0, jitter, size=len(x))
+    return x
 
 
 # %% Fontcolor
 def _preprocessing(x, y, z, labels, jitter, norm=False):
-    if jitter is None or jitter is False: jitter=0
-    if jitter is True: jitter=0.01
-    if jitter>0:
-        x = x + np.random.normal(0, jitter, size=len(x))
-        if y is not None: y = y + np.random.normal(0, jitter, size=len(y))
-        if z is not None: z = z + np.random.normal(0, jitter, size=len(z))
+    # Add jitter
+    x = jitter_func(x, jitter=jitter)
+    y = jitter_func(y, jitter=jitter)
+    z = jitter_func(z, jitter=jitter)
 
     # Combine into array
     if z is not None:
         X = np.c_[x, y, z]
     else:
         X = np.c_[x, y]
     # Normalize data
     if norm:
-        X = _normalize(X)
+        X = normalize_between_0_and_1(X)
     # Labels
     # if labels is None:
     #     labels=np.zeros_like(y).astype(int)
     # Return
     return X, labels
 
 
-# %% Fontcolor
-def _normalize(X):
+# %% Normalize between [0-1]
+def normalize_between_0_and_1(X):
     x_min, x_max = np.min(X, 0), np.max(X, 0)
     out = (X - x_min) / (x_max - x_min)
     out[np.isnan(out)]=1
     return out
 
 
 # %% Fontcolor
```

### Comparing `scatterd-1.3.4/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.5/scatterd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.4
+Version: 1.3.5
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.4.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.4 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.5 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.4.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.4/setup.py` & `scatterd-1.3.5/setup.py`

 * *Files identical despite different names*

