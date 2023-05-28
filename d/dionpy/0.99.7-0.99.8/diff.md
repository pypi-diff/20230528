# Comparing `tmp/dionpy-0.99.7.tar.gz` & `tmp/dionpy-0.99.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dionpy-0.99.7.tar", max compression
+gzip compressed data, was "dionpy-0.99.8.tar", max compression
```

## Comparing `dionpy-0.99.7.tar` & `dionpy-0.99.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1068 2022-08-09 17:20:39.809565 dionpy-0.99.7/LICENSE
--rwxr-xr-x   0        0        0      305 2022-11-09 17:44:18.328435 dionpy-0.99.7/README.md
--rw-r--r--   0        0        0     1034 2023-05-22 21:14:53.954975 dionpy-0.99.7/pyproject.toml
--rwxr-xr-x   0        0        0     4892 2023-05-05 23:38:28.402144 dionpy-0.99.7/src/dionpy/DLayer.py
--rwxr-xr-x   0        0        0     6246 2023-05-05 23:39:53.469536 dionpy-0.99.7/src/dionpy/FLayer.py
--rwxr-xr-x   0        0        0    23815 2023-05-05 23:38:28.378144 dionpy-0.99.7/src/dionpy/IonFrame.py
--rwxr-xr-x   0        0        0     8643 2023-05-05 23:38:28.410144 dionpy-0.99.7/src/dionpy/IonLayer.py
--rwxr-xr-x   0        0        0    15802 2023-05-05 23:38:28.414144 dionpy-0.99.7/src/dionpy/IonModel.py
--rwxr-xr-x   0        0        0      189 2022-08-05 19:11:20.810361 dionpy-0.99.7/src/dionpy/__init__.py
--rwxr-xr-x   0        0        0        0 2022-07-30 19:21:54.420046 dionpy-0.99.7/src/dionpy/modules/__init__.py
--rwxr-xr-x   0        0        0      155 2022-10-08 16:14:43.272649 dionpy-0.99.7/src/dionpy/modules/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      151 2022-08-05 19:03:44.347964 dionpy-0.99.7/src/dionpy/modules/__pycache__/__init__.cpython-38.pyc
--rwxr-xr-x   0        0        0     1473 2022-10-08 16:14:43.292639 dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc
--rwxr-xr-x   0        0        0     1503 2022-08-22 18:27:05.149833 dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc
--rw-r--r--   0        0        0     6015 2023-05-05 23:40:04.961453 dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc
--rwxr-xr-x   0        0        0     6041 2022-08-24 17:53:23.444818 dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2895 2023-04-17 23:55:21.174568 dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc
--rwxr-xr-x   0        0        0     2404 2022-09-13 17:23:53.972099 dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc
--rw-r--r--   0        0        0     4042 2023-04-17 23:39:36.664536 dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc
--rwxr-xr-x   0        0        0     3325 2022-08-05 19:03:44.351964 dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc
--rw-r--r--   0        0        0     6818 2023-04-19 00:05:43.520857 dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc
--rwxr-xr-x   0        0        0     3943 2022-10-05 20:19:58.421732 dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc
--rwxr-xr-x   0        0        0     1166 2022-07-30 19:21:54.420046 dionpy-0.99.7/src/dionpy/modules/col_freq_agg.csv
--rwxr-xr-x   0        0        0     1214 2022-08-22 18:26:43.278932 dionpy-0.99.7/src/dionpy/modules/collision_models.py
--rwxr-xr-x   0        0        0     5564 2023-05-05 23:40:02.877468 dionpy-0.99.7/src/dionpy/modules/helpers.py
--rwxr-xr-x   0        0        0     2524 2023-04-17 23:53:52.255388 dionpy-0.99.7/src/dionpy/modules/ion_tools.py
--rwxr-xr-x   0        0        0     3802 2023-04-17 22:22:14.774661 dionpy-0.99.7/src/dionpy/modules/parallel.py
--rwxr-xr-x   0        0        0     7308 2023-04-19 00:05:17.461073 dionpy-0.99.7/src/dionpy/modules/plotting.py
--rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 dionpy-0.99.7/setup.py
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 dionpy-0.99.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2022-08-09 17:20:39.809565 dionpy-0.99.8/LICENSE
+-rwxr-xr-x   0        0        0      305 2022-11-09 17:44:18.328435 dionpy-0.99.8/README.md
+-rw-r--r--   0        0        0     1071 2023-05-28 21:13:42.006598 dionpy-0.99.8/pyproject.toml
+-rwxr-xr-x   0        0        0     4893 2023-05-28 21:13:05.666884 dionpy-0.99.8/src/dionpy/DLayer.py
+-rwxr-xr-x   0        0        0     6246 2023-05-05 23:39:53.469536 dionpy-0.99.8/src/dionpy/FLayer.py
+-rwxr-xr-x   0        0        0    23957 2023-05-28 21:12:57.750946 dionpy-0.99.8/src/dionpy/IonFrame.py
+-rwxr-xr-x   0        0        0     8643 2023-05-05 23:38:28.410144 dionpy-0.99.8/src/dionpy/IonLayer.py
+-rwxr-xr-x   0        0        0    15802 2023-05-05 23:38:28.414144 dionpy-0.99.8/src/dionpy/IonModel.py
+-rwxr-xr-x   0        0        0      189 2022-08-05 19:11:20.810361 dionpy-0.99.8/src/dionpy/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-07-30 19:21:54.420046 dionpy-0.99.8/src/dionpy/modules/__init__.py
+-rwxr-xr-x   0        0        0      155 2022-10-08 16:14:43.272649 dionpy-0.99.8/src/dionpy/modules/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      151 2022-08-05 19:03:44.347964 dionpy-0.99.8/src/dionpy/modules/__pycache__/__init__.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1473 2022-10-08 16:14:43.292639 dionpy-0.99.8/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1503 2022-08-22 18:27:05.149833 dionpy-0.99.8/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc
+-rw-r--r--   0        0        0     6015 2023-05-05 23:40:04.961453 dionpy-0.99.8/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc
+-rwxr-xr-x   0        0        0     6041 2022-08-24 17:53:23.444818 dionpy-0.99.8/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2895 2023-04-17 23:55:21.174568 dionpy-0.99.8/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2404 2022-09-13 17:23:53.972099 dionpy-0.99.8/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc
+-rw-r--r--   0        0        0     4042 2023-04-17 23:39:36.664536 dionpy-0.99.8/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3325 2022-08-05 19:03:44.351964 dionpy-0.99.8/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc
+-rw-r--r--   0        0        0     6818 2023-04-19 00:05:43.520857 dionpy-0.99.8/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3943 2022-10-05 20:19:58.421732 dionpy-0.99.8/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1166 2022-07-30 19:21:54.420046 dionpy-0.99.8/src/dionpy/modules/col_freq_agg.csv
+-rwxr-xr-x   0        0        0     1214 2022-08-22 18:26:43.278932 dionpy-0.99.8/src/dionpy/modules/collision_models.py
+-rwxr-xr-x   0        0        0     5564 2023-05-05 23:40:02.877468 dionpy-0.99.8/src/dionpy/modules/helpers.py
+-rwxr-xr-x   0        0        0     2524 2023-04-17 23:53:52.255388 dionpy-0.99.8/src/dionpy/modules/ion_tools.py
+-rwxr-xr-x   0        0        0     3802 2023-04-17 22:22:14.774661 dionpy-0.99.8/src/dionpy/modules/parallel.py
+-rwxr-xr-x   0        0        0     7394 2023-05-22 21:44:59.503264 dionpy-0.99.8/src/dionpy/modules/plotting.py
+-rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 dionpy-0.99.8/setup.py
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 dionpy-0.99.8/PKG-INFO
```

### Comparing `dionpy-0.99.7/LICENSE` & `dionpy-0.99.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/pyproject.toml` & `dionpy-0.99.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dionpy"
-version = "0.99.7"
+version = "0.99.8"
 description = "Dynamic ionosphere model for global 21 cm experiments"
 authors = ["Vadym Bidula <vadym.bidula@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/lap1dem/dionpy"
 include = [
     "LICENSE",
@@ -27,24 +27,26 @@
 it = "^1.0.0"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autodoc-typehints = "^1.19.1"
 ffmpeg-progress-yield = "^0.3.0"
 sphinxcontrib-bibtex = "^2.5.0"
 setuptools = "^67.6.1"
-iricore = "^1.3.1"
+iricore = "^1.4.1"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 PyQt5 = "^5.15.6"
 PyYAML = "^6.0"
 qrcode = {extras = ["pil"], version = "^7.3.1"}
 #deepdish = "^0.3.7"
 #pydarnio = "^1.1.1"
 #pydarn = "^3.0"
 #psutil = "^5.9.4"
 pandas = "^1.5.3"
+unlzw = "^0.1.1"
+cartopy = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dionpy-0.99.7/src/dionpy/DLayer.py` & `dionpy-0.99.8/src/dionpy/DLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             ded = self.ed(el, az, layer=i)
             det = self.et(el, az, layer=i)
             freq_p = plasfreq(ded)
             ds = srange(theta, heights_km[i] * 1e3 + 0.5 * dh) - srange(theta, heights_km[i] * 1e3 - 0.5 * dh)
             atten[..., i] = np.exp(-2 * np.pi * freq_p ** 2 * freq_c * ds / (freq ** 2 + freq_c ** 2) / c)
             emiss[..., i] = (1 - atten[..., i]) * det
 
-        atten = atten.prod(axis=2)
+        atten = atten.prod(axis=-1)
         emiss = emiss.sum(axis=-1)
 
         if atten.size == 1:
             atten = atten[0, 0]
         if emission:
             return atten, emiss
         return atten
```

### Comparing `dionpy-0.99.7/src/dionpy/FLayer.py` & `dionpy-0.99.8/src/dionpy/FLayer.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/IonFrame.py` & `dionpy-0.99.8/src/dionpy/IonFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,35 +131,38 @@
     def atten(
         self,
         el: float | np.ndarray,
         az: float | np.ndarray,
         freq: float | np.ndarray,
         _pbar_desc: str | None = None,
         col_freq: str = "default",
+        emission: bool = True,
         troposphere: bool = True,
     ) -> float | np.ndarray:
         """
         :param el: Elevation of observation(s) in [deg].
         :param az: Azimuth of observation(s) in [deg].
         :param freq: Frequency of observation(s) in [MHz]. If  - the calculation will be performed in parallel on all
                      available cores. Requires `dt` to be a single datetime object.
         :param col_freq: Collision frequency model. Available options: 'default', 'nicolet', 'setty', 'aggrawal',
                          or float in Hz.
+        :param emission: If True - also returns array of emission temperatures.
         :param troposphere: If True - the troposphere refraction correction will be applied before calculation.
         :param _pbar_desc: Description of progress bar. If None - the progress bar will not appear.
         :return: Attenuation factor at given sky coordinates, time and frequency of observation. Output is the
                  attenuation factor between 0 (total attenuation) and 1 (no attenuation).
         """
         return self._parallel_calc(
             self.dlayer.atten,
             el,
             az,
             freq,
             _pbar_desc,
             col_freq=col_freq,
+            emission=emission,
             troposphere=troposphere,
         )
 
     def radec2altaz(self, ra: float | np.ndarray, dec: float | np.ndarray):
         """
         Converts sky coordinates to altitude and azimuth angles in horizontal CS.
```

### Comparing `dionpy-0.99.7/src/dionpy/IonLayer.py` & `dionpy-0.99.8/src/dionpy/IonLayer.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/IonModel.py` & `dionpy-0.99.8/src/dionpy/IonModel.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc` & `dionpy-0.99.8/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/col_freq_agg.csv` & `dionpy-0.99.8/src/dionpy/modules/col_freq_agg.csv`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/collision_models.py` & `dionpy-0.99.8/src/dionpy/modules/collision_models.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/helpers.py` & `dionpy-0.99.8/src/dionpy/modules/helpers.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/ion_tools.py` & `dionpy-0.99.8/src/dionpy/modules/ion_tools.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/parallel.py` & `dionpy-0.99.8/src/dionpy/modules/parallel.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.7/src/dionpy/modules/plotting.py` & `dionpy-0.99.8/src/dionpy/modules/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "cmap": "A colormap to use in the plot.",
     "cbformat": "Formatter of numbers on the colorbar scale.",
     "nancolor": "A color to fill np.nan in the plot.",
     "infcolor": "A color to fill np.inf in the plot.",
     "local_time": "Difference between local time and UTC. If specified - local time is shown instead of UTC.",
     "cinfo": "If true - places model info in the centre of the picture.",
     "lfont": "If true - the font size of labels is increased.",
+    "cbar": "If true - a colorbar is added.",
 }
 
 
 def polar_plot(
     data: Sequence[np.ndarray, np.ndarray, np.ndarray],
     dt: datetime | None = None,
     pos: Sequence[float, float, float] | None = None,
@@ -46,14 +47,15 @@
     cmap: str = "plasma",
     cbformat: str = None,
     nancolor: str = "black",
     infcolor: str = "white",
     local_time: int | None = None,
     cinfo: bool = False,
     lfont: bool = False,
+    cbar: bool = True,
 ):
     """
     A core function for graphic generation on the visible sky field.
     See all available option listed in dionpy.plot_kwargs.
 
     :return: A matplotlib figure.
     """
@@ -92,15 +94,16 @@
     rfmt = lambda x_, _: f"{x_:.0f}°"
     ax.yaxis.set_major_formatter(FuncFormatter(rfmt))
     ax.set_theta_direction(-1)
 
     labelsize = 14 if lfont else 11
     ax.tick_params(axis="both", which="major", labelsize=labelsize)
     ax.tick_params(axis="y", which="major", labelcolor=labelcolor)
-    cbar = plt.colorbar(img, fraction=0.042, pad=0.08, format=cbformat)
+    if cbar:
+        cbar = plt.colorbar(img, fraction=0.042, pad=0.08, format=cbformat)
     cbar.set_label(label=barlabel, size=labelsize)
     cbar.ax.tick_params(labelsize=labelsize)
     cbar.ax.yaxis.get_offset_text().set_fontsize(labelsize)
     plt.title(title, fontsize=14, pad=20)
 
     if plotlabel == "":
         if pos is not None:
```

### Comparing `dionpy-0.99.7/setup.py` & `dionpy-0.99.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 install_requires = \
 ['Sphinx>=5.0.2,<6.0.0',
  'echaim>=1.0.8,<2.0.0',
  'ffmpeg-progress-yield>=0.3.0,<0.4.0',
  'h5py>=3.7.0,<4.0.0',
  'healpy>=1.16.1,<2.0.0',
- 'iricore>=1.3.1,<2.0.0',
+ 'iricore>=1.4.1,<2.0.0',
  'it>=1.0.0,<2.0.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.22,<2.0',
  'pymap3d>=3.0.1,<4.0.0',
  'pytz>=2022.1,<2023.0',
  'scipy>=1.9.3,<2.0.0',
  'setuptools>=67.6.1,<68.0.0',
  'sphinx-autodoc-typehints>=1.19.1,<2.0.0',
  'sphinx-rtd-theme>=1.0.0,<2.0.0',
  'sphinxcontrib-bibtex>=2.5.0,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'dionpy',
-    'version': '0.99.7',
+    'version': '0.99.8',
     'description': 'Dynamic ionosphere model for global 21 cm experiments',
     'long_description': '[//]: # (![]&#40;docs/images/logos/logo_wide.png&#41;)\n\n# DIonPy\nThe `dionpy` package provides model of ionosphere refraction and attenuation based on the \n[IRI2020 Ionosphere Model](https://irimodel.org/).\n\nMore details are available at our [documentation page](https://dionpy.readthedocs.io/en/latest/).',
     'author': 'Vadym Bidula',
     'author_email': 'vadym.bidula@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lap1dem/dionpy',
```

### Comparing `dionpy-0.99.7/PKG-INFO` & `dionpy-0.99.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dionpy
-Version: 0.99.7
+Version: 0.99.8
 Summary: Dynamic ionosphere model for global 21 cm experiments
 Home-page: https://github.com/lap1dem/dionpy
 License: MIT
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sphinx (>=5.0.2,<6.0.0)
 Requires-Dist: echaim (>=1.0.8,<2.0.0)
 Requires-Dist: ffmpeg-progress-yield (>=0.3.0,<0.4.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: healpy (>=1.16.1,<2.0.0)
-Requires-Dist: iricore (>=1.3.1,<2.0.0)
+Requires-Dist: iricore (>=1.4.1,<2.0.0)
 Requires-Dist: it (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pymap3d (>=3.0.1,<4.0.0)
 Requires-Dist: pytz (>=2022.1,<2023.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
```

