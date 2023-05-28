# Comparing `tmp/pca-2.0.1.tar.gz` & `tmp/pca-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-2.0.1.tar", last modified: Fri Apr 28 11:38:45 2023, max compression
+gzip compressed data, was "pca-2.0.2.tar", last modified: Sun May 28 21:20:52 2023, max compression
```

## Comparing `pca-2.0.1.tar` & `pca-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.529502 pca-2.0.1/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9981 2023-04-28 11:38:45.527947 pca-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9457 2023-04-23 08:28:30.000000 pca-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.418075 pca-2.0.1/pca/
--rw-rw-rw-   0        0        0     1272 2023-04-28 11:38:30.000000 pca-2.0.1/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.518970 pca-2.0.1/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.1/pca/data/__init__.py
--rw-rw-rw-   0        0        0    33412 2023-04-28 11:37:18.000000 pca-2.0.1/pca/examples.py
--rw-rw-rw-   0        0        0    77776 2023-04-28 11:25:11.000000 pca-2.0.1/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.523957 pca-2.0.1/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.1/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.1/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.507999 pca-2.0.1/pca.egg-info/
--rw-rw-rw-   0        0        0     9981 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-04-28 11:38:45.000000 pca-2.0.1/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 11:38:45.529941 pca-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.944193 pca-2.0.2/
+-rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10335 2023-05-28 21:20:52.942703 pca-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.901265 pca-2.0.2/pca/
+-rw-rw-rw-   0        0        0     1272 2023-05-28 21:20:40.000000 pca-2.0.2/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.940201 pca-2.0.2/pca/data/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.2/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    33480 2023-04-28 11:42:55.000000 pca-2.0.2/pca/examples.py
+-rw-rw-rw-   0        0        0    78132 2023-05-28 14:18:17.000000 pca-2.0.2/pca/pca.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.941706 pca-2.0.2/pca/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.2/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.2/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.937430 pca-2.0.2/pca.egg-info/
+-rw-rw-rw-   0        0        0    10335 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 21:20:52.944193 pca-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.2/setup.py
```

### Comparing `pca-2.0.1/LICENSE` & `pca-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-2.0.1/PKG-INFO` & `pca-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.1
+Version: 2.0.2
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -55,19 +55,22 @@
 
 **⭐️ Star this repo if you like it ⭐️**
 
 ---
 
 ## Read the Medium blog for more details.
 
-<p align="left">
-  <a href="https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
-  </a>
-</p>
+#### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
+
+#### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
+
+#### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
+
+
+#
 
 
 ---
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.1 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.2 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
@@ -36,22 +36,27 @@
 compatibility when combining with other packages. But this package can do a lot
 more. Besides the regular pca, it can also perform **SparsePCA**, and
 **TruncatedSVD**. Depending on your input data, the best approach will be
 choosen. Other functionalities of PCA are: * **Biplot** to plot the loadings *
 Determine the **explained variance** * Extract the best performing **features**
 * Scatter plot with the **loadings** * Outlier detection using **Hotelling T2
 and/or SPE/Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ##
-Read the Medium blog for more details.
-[https://github.com/erdogant/pca/blob/master/docs/figs/
-medium_blog1.png?raw=true]
---- ## [Documentation pages](https://erdogant.github.io/pca/) On the
-[documentation pages](https://erdogant.github.io/pca/) you can find detailed
-information about the working of the ``pca`` with many examples. --- ##
-Installation ```bash pip install pca ``` ##### Import pca package ```python
-from pca import pca ``` #
+Read the Medium blog for more details. #### [1. What are PCA loadings and how
+to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-
+loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal
+Component Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
+towardsdatascience.com/outlier-detection-using-principal-component-analysis-
+and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
+comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
+towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) # --- ## [Documentation pages](https://
+erdogant.github.io/pca/) On the [documentation pages](https://
+erdogant.github.io/pca/) you can find detailed information about the working of
+the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
+##### Import pca package ```python from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
 fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
```

### Comparing `pca-2.0.1/README.md` & `pca-2.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,19 +40,22 @@
 
 **⭐️ Star this repo if you like it ⭐️**
 
 ---
 
 ## Read the Medium blog for more details.
 
-<p align="left">
-  <a href="https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
-  </a>
-</p>
+#### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
+
+#### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
+
+#### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
+
+
+#
 
 
 ---
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples.
```

#### html2text {}

```diff
@@ -29,22 +29,27 @@
 compatibility when combining with other packages. But this package can do a lot
 more. Besides the regular pca, it can also perform **SparsePCA**, and
 **TruncatedSVD**. Depending on your input data, the best approach will be
 choosen. Other functionalities of PCA are: * **Biplot** to plot the loadings *
 Determine the **explained variance** * Extract the best performing **features**
 * Scatter plot with the **loadings** * Outlier detection using **Hotelling T2
 and/or SPE/Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ##
-Read the Medium blog for more details.
-[https://github.com/erdogant/pca/blob/master/docs/figs/
-medium_blog1.png?raw=true]
---- ## [Documentation pages](https://erdogant.github.io/pca/) On the
-[documentation pages](https://erdogant.github.io/pca/) you can find detailed
-information about the working of the ``pca`` with many examples. --- ##
-Installation ```bash pip install pca ``` ##### Import pca package ```python
-from pca import pca ``` #
+Read the Medium blog for more details. #### [1. What are PCA loadings and how
+to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-
+loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal
+Component Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
+towardsdatascience.com/outlier-detection-using-principal-component-analysis-
+and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
+comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
+towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) # --- ## [Documentation pages](https://
+erdogant.github.io/pca/) On the [documentation pages](https://
+erdogant.github.io/pca/) you can find detailed information about the working of
+the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
+##### Import pca package ```python from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
 fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
```

### Comparing `pca-2.0.1/pca/__init__.py` & `pca-2.0.2/pca/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
 Description
```

### Comparing `pca-2.0.1/pca/examples.py` & `pca-2.0.2/pca/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
              cmap='bwr_r',
              fontsize=22,
              legend=2,
              density=True,
              arrowdict={'color_strong': 'r', 'color_weak': 'g'},
              title='Biplot with with the pca library.')
 
+# model.biplot(arrowdict={'color_strong': 'r', 'color_weak': 'g'})
 
 # %%
 # from sklearn.datasets import make_friedman1
 # X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
 # model = pca()
 # model.fit_transform(X)
```

### Comparing `pca-2.0.1/pca/pca.py` & `pca-2.0.2/pca/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,27 @@
     References
     ----------
     * Blog: https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559
     * Github: https://github.com/erdogant/pca
     * Documentation: https://erdogant.github.io/pca/
 
     """
+    def __init__(self,
+                 n_components=0.95,
+                 n_feat=25,
+                 method='pca',
+                 alpha=0.05,
+                 multipletests='fdr_bh',
+                 n_std=3,
+                 onehot=False,
+                 normalize=False,
+                 detect_outliers=['ht2', 'spe'],
+                 random_state=None,
+                 verbose=3):
 
-    def __init__(self, n_components=0.95, n_feat=25, method='pca', alpha=0.05, multipletests='fdr_bh', n_std=3, onehot=False, normalize=False, detect_outliers=['ht2', 'spe'], random_state=None, verbose=3):
         """Initialize pca with user-defined parameters."""
         if isinstance(detect_outliers, str): detect_outliers = [detect_outliers]
         if detect_outliers is not None: detect_outliers=list(map(str.lower, detect_outliers))
 
         if onehot:
             if verbose>=3: print('[pca] >Method is set to: [sparse_pca] because onehot=True.')
             method = 'sparse_pca'
@@ -539,14 +550,15 @@
                 title=None,
                 legend=None,
                 figsize=(25, 15),
                 dpi=100,
                 visible=True,
                 fig=None,
                 ax=None,
+                grid=True,
                 y=None,  # deprecated
                 label=None,  # deprecated
                 verbose=3):
         """Scatter 2d plot.
 
         Parameters
         ----------
@@ -654,21 +666,23 @@
                            c=c,
                            labels=labels,
                            edgecolor=edgecolor,
                            alpha=alpha,
                            marker=marker,
                            jitter=jitter,
                            density=density,
+                           opaque_type='per_class',
                            density_on_top=density_on_top,
                            gradient=gradient,
                            cmap=cmap,
                            legend=legend,
                            fontcolor=fontcolor,
                            fontsize=fontsize,
                            fontweight=fontweight,
+                           grid=grid,
                            dpi=dpi,
                            figsize=figsize,
                            visible=visible,
                            fig=fig,
                            ax=ax)
 
         # Plot the SPE with Elipse
@@ -704,14 +718,15 @@
                title=None,
                legend=None,
                figsize=(25, 15),
                visible=True,
                fig=None,
                ax=None,
                dpi=100,
+               grid=True,
                y=None,  # deprecated
                label=None,  # deprecated
                verbose=None):
         """Create Biplot.
 
         Plots the Principal components with the samples, and the best performing features.
         Per PC, The feature with absolute highest loading is gathered. This can result into features that are seen over multiple PCs, and some features may never be detected.
@@ -835,15 +850,15 @@
             return None, None
 
         # Input checks
         arrowdict, cmap, PC, d3, s = _biplot_input_checks(self.results, PC, cmap, arrowdict, color_arrow, fontsize, fontweight, c, s, verbose)
         # Pre-processing
         labels, topfeat, n_feat = self._fig_preprocessing(labels, n_feat, d3)
         # Scatterplot
-        fig, ax = self.scatter(labels=labels, legend=legend, PC=PC, SPE=SPE, HT2=HT2, cmap=cmap, visible=visible, figsize=figsize, alpha=alpha, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, fontcolor=fontcolor, fontweight=fontweight, fontsize=fontsize, edgecolor=edgecolor, density=density, density_on_top=density_on_top, dpi=dpi, verbose=verbose)
+        fig, ax = self.scatter(labels=labels, legend=legend, PC=PC, SPE=SPE, HT2=HT2, cmap=cmap, visible=visible, figsize=figsize, alpha=alpha, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, fontcolor=fontcolor, fontweight=fontweight, fontsize=fontsize, edgecolor=edgecolor, density=density, density_on_top=density_on_top, dpi=dpi, grid=grid, verbose=verbose)
         # Add the loadings with arrow to the plot
         fig, ax = _plot_loadings(self, topfeat, n_feat, PC, d3, arrowdict, fig, ax, verbose)
         # Plot
         if visible: plt.show()
         # Return
         return fig, ax
```

### Comparing `pca-2.0.1/pca/tests/test_pca.py` & `pca-2.0.2/pca/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.1/pca.egg-info/PKG-INFO` & `pca-2.0.2/pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.1
+Version: 2.0.2
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -55,19 +55,22 @@
 
 **⭐️ Star this repo if you like it ⭐️**
 
 ---
 
 ## Read the Medium blog for more details.
 
-<p align="left">
-  <a href="https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559">
-  <img src="https://github.com/erdogant/pca/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
-  </a>
-</p>
+#### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
+
+#### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
+
+#### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
+
+
+#
 
 
 ---
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.1 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.2 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
@@ -36,22 +36,27 @@
 compatibility when combining with other packages. But this package can do a lot
 more. Besides the regular pca, it can also perform **SparsePCA**, and
 **TruncatedSVD**. Depending on your input data, the best approach will be
 choosen. Other functionalities of PCA are: * **Biplot** to plot the loadings *
 Determine the **explained variance** * Extract the best performing **features**
 * Scatter plot with the **loadings** * Outlier detection using **Hotelling T2
 and/or SPE/Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ##
-Read the Medium blog for more details.
-[https://github.com/erdogant/pca/blob/master/docs/figs/
-medium_blog1.png?raw=true]
---- ## [Documentation pages](https://erdogant.github.io/pca/) On the
-[documentation pages](https://erdogant.github.io/pca/) you can find detailed
-information about the working of the ``pca`` with many examples. --- ##
-Installation ```bash pip install pca ``` ##### Import pca package ```python
-from pca import pca ``` #
+Read the Medium blog for more details. #### [1. What are PCA loadings and how
+to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-
+loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal
+Component Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
+towardsdatascience.com/outlier-detection-using-principal-component-analysis-
+and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
+comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
+towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) # --- ## [Documentation pages](https://
+erdogant.github.io/pca/) On the [documentation pages](https://
+erdogant.github.io/pca/) you can find detailed information about the working of
+the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
+##### Import pca package ```python from pca import pca ``` #
 Quick_start                            Make_biplot
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
 master/docs/figs/                      master/docs/figs/
 fig_scatter.png?raw=true]              custom_example_2.png?raw=true]
 #
 Plot_Explained_variance                3D_plots
 [https://github.com/erdogant/pca/blob/ [https://github.com/erdogant/pca/blob/
```

### Comparing `pca-2.0.1/setup.py` & `pca-2.0.2/setup.py`

 * *Files identical despite different names*

