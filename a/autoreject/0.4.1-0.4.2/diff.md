# Comparing `tmp/autoreject-0.4.1.tar.gz` & `tmp/autoreject-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoreject-0.4.1.tar", last modified: Thu Jan 12 17:10:04 2023, max compression
+gzip compressed data, was "autoreject-0.4.2.tar", last modified: Sun May 28 09:05:33 2023, max compression
```

## Comparing `autoreject-0.4.1.tar` & `autoreject-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:10:04.386441 autoreject-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-01-12 17:09:52.000000 autoreject-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-12 17:09:52.000000 autoreject-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-12 17:10:04.386441 autoreject-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-01-12 17:09:52.000000 autoreject-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:10:04.386441 autoreject-0.4.1/autoreject/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56239 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/autoreject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/bayesopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/ransac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:10:04.386441 autoreject-0.4.1/autoreject/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/tests/test_autoreject.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/tests/test_bayesopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/tests/test_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-01-12 17:09:52.000000 autoreject-0.4.1/autoreject/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:10:04.386441 autoreject-0.4.1/autoreject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-12 17:10:04.000000 autoreject-0.4.1/autoreject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-12 17:10:04.000000 autoreject-0.4.1/autoreject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 17:10:04.000000 autoreject-0.4.1/autoreject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-12 17:10:04.000000 autoreject-0.4.1/autoreject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-12 17:10:04.000000 autoreject-0.4.1/autoreject.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:10:04.386441 autoreject-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_auto_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_autoreject_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_channel_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_estimate_global_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_global_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-01-12 17:09:52.000000 autoreject-0.4.1/examples/plot_visualize_bad_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-12 17:10:04.386441 autoreject-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-01-12 17:09:52.000000 autoreject-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:05:33.182927 autoreject-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 09:05:22.000000 autoreject-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-28 09:05:22.000000 autoreject-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-28 09:05:33.182927 autoreject-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-28 09:05:22.000000 autoreject-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:05:33.178927 autoreject-0.4.2/autoreject/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56534 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/autoreject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/bayesopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/ransac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:05:33.178927 autoreject-0.4.2/autoreject/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/tests/test_autoreject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/tests/test_bayesopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/tests/test_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18166 2023-05-28 09:05:22.000000 autoreject-0.4.2/autoreject/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:05:33.178927 autoreject-0.4.2/autoreject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-28 09:05:33.000000 autoreject-0.4.2/autoreject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-28 09:05:33.000000 autoreject-0.4.2/autoreject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:05:33.000000 autoreject-0.4.2/autoreject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-28 09:05:33.000000 autoreject-0.4.2/autoreject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 09:05:33.000000 autoreject-0.4.2/autoreject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:05:33.182927 autoreject-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_auto_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_autoreject_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_channel_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_estimate_global_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_global_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-28 09:05:22.000000 autoreject-0.4.2/examples/plot_visualize_bad_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-28 09:05:33.182927 autoreject-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-28 09:05:22.000000 autoreject-0.4.2/setup.py
```

### Comparing `autoreject-0.4.1/LICENSE` & `autoreject-0.4.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016-2022, autoreject developers
+Copyright (c) 2016-2023, autoreject developers
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `autoreject-0.4.1/PKG-INFO` & `autoreject-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoreject
-Version: 0.4.1
+Version: 0.4.2
 Summary: Automated rejection and repair of epochs in M/EEG.
 Home-page: http://autoreject.github.io/
 Download-URL: https://github.com/autoreject/autoreject.git
 Maintainer: Mainak Jas
 Maintainer-email: mainakjas@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, http://autoreject.github.io/
@@ -19,15 +19,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 autoreject
 ==========
@@ -62,15 +62,15 @@
 
 .. docs_readme_include_label
 
 Installation
 ------------
 
 We recommend the `Anaconda Python distribution <https://www.anaconda.com/>`_
-and a **Python version >= 3.7**.
+and a **Python version >= 3.8**.
 To obtain the stable release of ``autoreject``, you can use ``pip``::
 
     pip install -U autoreject
 
 Or ``conda``::
 
     conda install -c conda-forge autoreject
@@ -88,19 +88,19 @@
 
 and it should not give any error messages.
 
 Below, we list the dependencies for ``autoreject``.
 All required dependencies are installed automatically when you install ``autoreject``.
 
 * ``mne`` (>=1.0)
-* ``numpy`` (>=1.20)
-* ``scipy`` (>=1.6)
-* ``scikit-learn`` (>=0.24)
+* ``numpy`` (>=1.20.2)
+* ``scipy`` (>=1.6.3)
+* ``scikit-learn`` (>=0.24.2)
 * ``joblib``
-* ``matplotlib`` (>=3.3)
+* ``matplotlib`` (>=3.4.0)
 
 Optional dependencies are:
 
 * ``openneuro-py`` (>= 2021.10.1, for fetching data from `OpenNeuro.org <https://openneuro.org>`_)
 
 Quickstart
 ==========
@@ -118,15 +118,16 @@
 rejection dictionary, simply do:
 
 .. code:: python
 
 	>>> from autoreject import get_rejection_threshold
 	>>> reject = get_rejection_threshold(epochs)  # doctest: +SKIP
 
-We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_.
+We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_
+(see `PyPREP <https://github.com/sappelhoff/pyprep>`_ for a full implementation of the PREP pipeline).
 The API is the same:
 
 .. code:: python
 
 	>>> from autoreject import Ransac
 	>>> rsc = Ransac()
 	>>> epochs_clean = rsc.fit_transform(epochs)  # doctest: +SKIP
```

### Comparing `autoreject-0.4.1/README.rst` & `autoreject-0.4.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 .. docs_readme_include_label
 
 Installation
 ------------
 
 We recommend the `Anaconda Python distribution <https://www.anaconda.com/>`_
-and a **Python version >= 3.7**.
+and a **Python version >= 3.8**.
 To obtain the stable release of ``autoreject``, you can use ``pip``::
 
     pip install -U autoreject
 
 Or ``conda``::
 
     conda install -c conda-forge autoreject
@@ -57,19 +57,19 @@
 
 and it should not give any error messages.
 
 Below, we list the dependencies for ``autoreject``.
 All required dependencies are installed automatically when you install ``autoreject``.
 
 * ``mne`` (>=1.0)
-* ``numpy`` (>=1.20)
-* ``scipy`` (>=1.6)
-* ``scikit-learn`` (>=0.24)
+* ``numpy`` (>=1.20.2)
+* ``scipy`` (>=1.6.3)
+* ``scikit-learn`` (>=0.24.2)
 * ``joblib``
-* ``matplotlib`` (>=3.3)
+* ``matplotlib`` (>=3.4.0)
 
 Optional dependencies are:
 
 * ``openneuro-py`` (>= 2021.10.1, for fetching data from `OpenNeuro.org <https://openneuro.org>`_)
 
 Quickstart
 ==========
@@ -87,15 +87,16 @@
 rejection dictionary, simply do:
 
 .. code:: python
 
 	>>> from autoreject import get_rejection_threshold
 	>>> reject = get_rejection_threshold(epochs)  # doctest: +SKIP
 
-We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_.
+We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_
+(see `PyPREP <https://github.com/sappelhoff/pyprep>`_ for a full implementation of the PREP pipeline).
 The API is the same:
 
 .. code:: python
 
 	>>> from autoreject import Ransac
 	>>> rsc = Ransac()
 	>>> epochs_clean = rsc.fit_transform(epochs)  # doctest: +SKIP
```

### Comparing `autoreject-0.4.1/autoreject/autoreject.py` & `autoreject-0.4.2/autoreject/autoreject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1270,28 +1270,32 @@
         """Initialize the Rejection Log."""
         self.bad_epochs = bad_epochs
         self.labels = labels
         self.ch_names = ch_names
         assert len(bad_epochs) == labels.shape[0]
         assert len(ch_names) == labels.shape[1]
 
-    def plot(self, orientation='vertical', show_names='auto', show=True,
-             ax=None):
+    def plot(self, orientation='vertical', show_names='auto', aspect='equal',
+             show=True, ax=None):
         """Plot an image of good, bad and interpolated channels for each epoch.
 
         Parameters
         ----------
         orientation : 'vertical' | 'horizontal'
             If `'vertical'` (default), will plot sensors on x-axis and epochs
             on y-axis. If `'horizontal'`, will plot epochs on x-axis and
             sensors on y-axis.
         show_names : 'auto' | int
             If 'auto' (default), show all channel names if fewer than 25
             entries. Otherwise it shows every 5 entries. If int, show every
             show_names entries.
+        aspect : 'equal' | 'auto'
+            If 'equal', the pixels are square. If 'auto', the axis is fixed
+            and the aspect ratio is adjusted for data to fit. See documentation
+            of plt.imshow() for more details.
         show : bool
             If True (default), display the figure immediately.
         ax : matplotlib.axes.Axes | None
             The axes to plot to. In ``None`` (default), create a new
             figure and axes.
 
         Returns
@@ -1316,15 +1320,16 @@
         image = self.labels.copy()
         image[image == 2] = 0.5  # move interp to 0.5
         # good, interp, bad
         legend_label = {0: 'good', 0.5: 'interpolated', 1: 'bad'}
         cmap = mpl.colors.ListedColormap(['lightgreen', 'blue', 'red'])
         if orientation == 'horizontal':
             img = ax.imshow(image.T, cmap=cmap,
-                            vmin=0, vmax=1, interpolation='nearest')
+                            vmin=0, vmax=1, interpolation='nearest',
+                            aspect=aspect)
             ax.set_xlabel('Epochs')
             ax.set_ylabel('Channels')
             plt.setp(ax, yticks=range(0, self.labels.shape[1], show_names),
                      yticklabels=ch_names_)
             plt.setp(ax.get_yticklabels(), fontsize=8)
             # add red box around rejected epochs
             for idx in np.where(self.bad_epochs)[0]:
```

### Comparing `autoreject-0.4.1/autoreject/bayesopt.py` & `autoreject-0.4.2/autoreject/bayesopt.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/autoreject/conftest.py` & `autoreject-0.4.2/autoreject/conftest.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/autoreject/ransac.py` & `autoreject-0.4.2/autoreject/ransac.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/autoreject/tests/test_autoreject.py` & `autoreject-0.4.2/autoreject/tests/test_autoreject.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         mne.pick_types(epochs.info, meg=False, eeg=True)[::16],
         mne.pick_types(epochs.info, meg=False, eeg=False, eog=True)]
     pick_ch_names = [epochs.ch_names[pp] for pp in pre_picks]
     bad_ch_names = [epochs.ch_names[ix] for ix in range(len(epochs.ch_names))
                     if ix not in pre_picks]
     epochs_with_bads = epochs.copy()
     epochs_with_bads.info['bads'] = bad_ch_names
-    epochs.pick_channels(pick_ch_names)
+    epochs.pick_channels(pick_ch_names, ordered=False)
 
     epochs_fit = epochs[:12]  # make sure to use different size of epochs
     epochs_new = epochs[12:]
     epochs_with_bads_fit = epochs_with_bads[:12]
 
     X = epochs_fit.get_data()
     n_epochs, n_channels, n_times = X.shape
```

### Comparing `autoreject-0.4.1/autoreject/tests/test_ransac.py` & `autoreject-0.4.2/autoreject/tests/test_ransac.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/autoreject/tests/test_utils.py` & `autoreject-0.4.2/autoreject/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     raw.del_proj()
     evoked = mne.read_evokeds(evoked_fname, condition='Left Auditory',
                               baseline=(None, 0))
     event_id = {'Visual/Left': 3}
     tmin, tmax = -0.2, 0.5
     events = mne.find_events(raw)
     picks = mne.pick_channels(raw.info['ch_names'],
-                              ['MEG 2443', 'MEG 2442', 'MEG 2441'])
+                              ['MEG 2443', 'MEG 2442', 'MEG 2441'],
+                              ordered=False)
     epochs = mne.Epochs(raw, events, event_id, tmin, tmax,
                         picks=picks, baseline=(None, 0),
                         reject=None, preload=True)
 
     this_epoch = epochs.copy()
     assert this_epoch.info['bads'] == ['MEG 2443']
     epochs_clean = clean_by_interp(this_epoch)
```

### Comparing `autoreject-0.4.1/autoreject/tests/test_viz.py` & `autoreject-0.4.2/autoreject/tests/test_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     raw.crop(0, 15)
     raw.del_proj()
 
     set_matplotlib_defaults(plt)
 
     events = mne.find_events(raw)
     picks = mne.pick_channels(raw.info['ch_names'],
-                              ['MEG 2443', 'MEG 2442', 'MEG 2441'])
+                              ['MEG 2443', 'MEG 2442', 'MEG 2441'],
+                              ordered=False)
     epochs = mne.Epochs(raw, events, picks=picks, baseline=(None, 0),
                         reject=None, preload=True,
                         event_id={'1': 1, '2': 2, '3': 3, '4': 4})
     bad_epochs_idx = [0, 1, 3]
     n_epochs, n_channels, _ = epochs.get_data().shape
     bad_epochs = np.zeros(n_epochs, dtype=bool)
     bad_epochs[bad_epochs_idx] = True
```

### Comparing `autoreject-0.4.1/autoreject/utils.py` & `autoreject-0.4.2/autoreject/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import numpy as np
 
 import mne
 from mne import pick_types, pick_info
 from mne.io.pick import _picks_to_idx
 from mne.channels.interpolation import _do_interp_dots
+from mne.forward._field_interpolation import _setup_dots
 
 
 def _check_ch_locs(chs):
     """Check if channel locations exist.
 
     Parameters
     ----------
@@ -398,16 +399,15 @@
     from mne.bem import _check_origin
 
     if templates is None:
         templates = _read_coil_defs(verbose='error')
     coils = _create_meg_coils(info['chs'], 'normal', info['dev_head_t'],
                               templates)
     my_origin = _check_origin((0., 0., 0.04), info)
-    int_rad, noise, lut_fun, n_fact = _patch_setup_dots(mode, info,
-                                                        coils, 'meg')
+    int_rad, noise, lut_fun, n_fact = _setup_dots(mode, info, coils, 'meg')
     self_dots = _do_self_dots(int_rad, False, coils, my_origin, 'meg',
                               lut_fun, n_fact, n_jobs=1)
     cross_dots = _do_cross_dots(int_rad, False, coils, coils,
                                 my_origin, 'meg', lut_fun, n_fact).T
     return self_dots, cross_dots
 
 
@@ -430,16 +430,16 @@
     miss = 1e-4  # Smoothing criterion for MEG
 
     info_from = pick_info(info, pick_from, copy=True)
     templates = _read_coil_defs(verbose='error')
     coils_from = _create_meg_coils(info_from['chs'], 'normal',
                                    info_from['dev_head_t'], templates)
     my_origin = _check_origin((0., 0., 0.04), info_from)
-    int_rad, noise, lut_fun, n_fact = _patch_setup_dots(mode, info_from,
-                                                        coils_from, 'meg')
+    int_rad, noise, lut_fun, n_fact = _setup_dots(mode, info_from,
+                                                  coils_from, 'meg')
 
     # This function needs a clean input. It hates the presence of other
     # channels than MEG channels. Make sure all is picked.
     if dots is None:
         dots = self_dots, cross_dots = _compute_dots(
             info, mode=mode, templates=templates)
     else:
@@ -455,24 +455,14 @@
     # XXX: hack to silence _compute_mapping_matrix
     with mne.utils.use_log_level('error'):
         fmd['data'] = _compute_mapping_matrix(fmd, info_from)
 
     return fmd['data']
 
 
-def _patch_setup_dots(mode, info, coils, ch):
-    """Monkey patch _setup_dots for MNE-Python >= v0.24."""
-    from mne.forward._field_interpolation import _setup_dots
-    from mne.utils import check_version
-    if not check_version('mne', '0.24'):
-        return _setup_dots(mode, coils, ch)
-    else:
-        return _setup_dots(mode, info, coils, ch)
-
-
 def _get_channel_type(epochs, picks):
     """return whether a set of picks are all meg or all eeg channels."""
     picked_info = mne.io.pick.pick_info(epochs.info, picks)
     ch_types_picked = {
         mne.io.meas_info.channel_type(picked_info, idx)
         for idx in range(len(picks))}
     invalid_ch_types_present = [key for key in ch_types_picked
```

### Comparing `autoreject-0.4.1/autoreject.egg-info/PKG-INFO` & `autoreject-0.4.2/autoreject.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoreject
-Version: 0.4.1
+Version: 0.4.2
 Summary: Automated rejection and repair of epochs in M/EEG.
 Home-page: http://autoreject.github.io/
 Download-URL: https://github.com/autoreject/autoreject.git
 Maintainer: Mainak Jas
 Maintainer-email: mainakjas@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, http://autoreject.github.io/
@@ -19,15 +19,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 autoreject
 ==========
@@ -62,15 +62,15 @@
 
 .. docs_readme_include_label
 
 Installation
 ------------
 
 We recommend the `Anaconda Python distribution <https://www.anaconda.com/>`_
-and a **Python version >= 3.7**.
+and a **Python version >= 3.8**.
 To obtain the stable release of ``autoreject``, you can use ``pip``::
 
     pip install -U autoreject
 
 Or ``conda``::
 
     conda install -c conda-forge autoreject
@@ -88,19 +88,19 @@
 
 and it should not give any error messages.
 
 Below, we list the dependencies for ``autoreject``.
 All required dependencies are installed automatically when you install ``autoreject``.
 
 * ``mne`` (>=1.0)
-* ``numpy`` (>=1.20)
-* ``scipy`` (>=1.6)
-* ``scikit-learn`` (>=0.24)
+* ``numpy`` (>=1.20.2)
+* ``scipy`` (>=1.6.3)
+* ``scikit-learn`` (>=0.24.2)
 * ``joblib``
-* ``matplotlib`` (>=3.3)
+* ``matplotlib`` (>=3.4.0)
 
 Optional dependencies are:
 
 * ``openneuro-py`` (>= 2021.10.1, for fetching data from `OpenNeuro.org <https://openneuro.org>`_)
 
 Quickstart
 ==========
@@ -118,15 +118,16 @@
 rejection dictionary, simply do:
 
 .. code:: python
 
 	>>> from autoreject import get_rejection_threshold
 	>>> reject = get_rejection_threshold(epochs)  # doctest: +SKIP
 
-We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_.
+We also implement RANSAC from the `PREP pipeline <https://doi.org/10.3389/fninf.2015.00016>`_
+(see `PyPREP <https://github.com/sappelhoff/pyprep>`_ for a full implementation of the PREP pipeline).
 The API is the same:
 
 .. code:: python
 
 	>>> from autoreject import Ransac
 	>>> rsc = Ransac()
 	>>> epochs_clean = rsc.fit_transform(epochs)  # doctest: +SKIP
```

### Comparing `autoreject-0.4.1/autoreject.egg-info/SOURCES.txt` & `autoreject-0.4.2/autoreject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_auto_repair.py` & `autoreject-0.4.2/examples/plot_auto_repair.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_autoreject_workflow.py` & `autoreject-0.4.2/examples/plot_autoreject_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,38 +27,41 @@
 # .. contents:: Table of Contents
 #    :local:
 #
 # First, we download resting-state EEG data from a Parkinson's patient
 # from OpenNeuro. We will do this using ``openneuro-py`` which can be
 # installed with the command ``pip install openneuro-py``.
 
-import os.path as op
+import os
 import matplotlib.pyplot as plt
 import openneuro
 
 import mne
 import autoreject
 
 dataset = 'ds002778'  # The id code on OpenNeuro for this example dataset
 subject_id = 'pd14'
 
-target_dir = op.join(op.dirname(autoreject.__file__), '..', 'examples')
+target_dir = os.path.join(
+    os.path.dirname(autoreject.__file__), '..', 'examples', dataset)
+os.makedirs(target_dir, exist_ok=True)
+
 openneuro.download(dataset=dataset, target_dir=target_dir,
                    include=[f'sub-{subject_id}/ses-off'])
 
 # %%
 # We will now load in the raw data from the bdf file downloaded from OpenNeuro
 # and, since this is resting-state data without any events, make regularly
 # spaced events with which to epoch the raw data. In the averaged plot,
 # we can see that there may be some eyeblink
 # artifact contamination but, overall, the data is typical of
 # resting-state EEG.
 
-raw_fname = op.join(target_dir, f'sub-{subject_id}',
-                    'ses-off', 'eeg', 'sub-pd14_ses-off_task-rest_eeg.bdf')
+raw_fname = os.path.join(target_dir, f'sub-{subject_id}', 'ses-off', 'eeg',
+                         'sub-pd14_ses-off_task-rest_eeg.bdf')
 raw = mne.io.read_raw_bdf(raw_fname, preload=True)
 dig_montage = mne.channels.make_standard_montage('biosemi32')
 raw.drop_channels([ch for ch in raw.ch_names
                    if ch not in dig_montage.ch_names])
 raw.set_montage(dig_montage)  # use the standard montage
 epochs = mne.make_fixed_length_epochs(raw, duration=3, preload=True)
```

### Comparing `autoreject-0.4.1/examples/plot_channel_thresholds.py` & `autoreject-0.4.2/examples/plot_channel_thresholds.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_estimate_global_reject.py` & `autoreject-0.4.2/examples/plot_estimate_global_reject.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_global_reject.py` & `autoreject-0.4.2/examples/plot_global_reject.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_ransac.py` & `autoreject-0.4.2/examples/plot_ransac.py`

 * *Files identical despite different names*

### Comparing `autoreject-0.4.1/examples/plot_visualize_bad_epochs.py` & `autoreject-0.4.2/examples/plot_visualize_bad_epochs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 import autoreject
 
 dataset = 'ds000117'  # The id code on OpenNeuro for this example dataset
 subject_id = 16  # OpenfMRI format of subject numbering
 
 target_dir = os.path.join(
     os.path.dirname(autoreject.__file__), '..', 'examples', dataset)
-if not os.path.isdir(target_dir):
-    os.makedirs(target_dir)
+os.makedirs(target_dir, exist_ok=True)
 
 openneuro.download(dataset=dataset, target_dir=target_dir,
                    include=[f'sub-{subject_id}/ses-meg/'])
 
 # %%
 # We will create epochs with data starting 200 ms before trigger onset
 # and continuing up to 800 ms after that. The data contains visual stimuli for
```

### Comparing `autoreject-0.4.1/setup.py` & `autoreject-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,35 +46,36 @@
               'Operating System :: Unix',
               'Operating System :: MacOS',
               'Programming Language :: Python :: 3',
           ],
           platforms='any',
           keywords=('electroencephalography eeg magnetoencephalography '
                     'meg preprocessing analysis'),
-          python_requires='~=3.7',
+          python_requires='~=3.8',
           install_requires=[
-              'numpy >= 1.20',
-              'scipy >= 1.6',
+              'numpy >= 1.20.2',
+              'scipy >= 1.6.3',
               'mne[hdf5] >= 1.0',
-              'scikit-learn >= 0.24',
+              'scikit-learn >= 0.24.2',
               'joblib',
-              'matplotlib >= 3.3',
+              'matplotlib >= 3.4.0',
           ],
           extras_require={
               'test': [
                   'pytest',
                   'pytest-cov',
                   'pytest-sugar',
                   'check-manifest',
                   'flake8',
+                  'importlib_resources'  # drop after minimum Py >=3.10
               ],
               'doc': [
                   'sphinx',
                   'sphinx-gallery',
-                  'sphinx_bootstrap_theme',
+                  'pydata-sphinx-theme',
                   'sphinx-copybutton',
                   'sphinx-github-role',
                   'numpydoc',
                   'cython',
                   'pillow',
                   'openneuro-py >= 2021.10.1',
               ]
```

