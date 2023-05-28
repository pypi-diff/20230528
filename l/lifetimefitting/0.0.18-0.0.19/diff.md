# Comparing `tmp/lifetimefitting-0.0.18.tar.gz` & `tmp/lifetimefitting-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.18.tar", last modified: Sat May 27 03:40:25 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.19.tar", last modified: Sun May 28 14:51:57 2023, max compression
```

## Comparing `lifetimefitting-0.0.18.tar` & `lifetimefitting-0.0.19.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.178601 lifetimefitting-0.0.18/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:57.206711 lifetimefitting-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-28 14:51:57.206711 lifetimefitting-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:57.202711 lifetimefitting-0.0.19/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:57.202711 lifetimefitting-0.0.19/app/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:57.202711 lifetimefitting-0.0.19/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:51:57.206711 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-28 14:51:57.000000 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-28 14:51:57.000000 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:51:57.000000 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-28 14:51:57.000000 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 14:51:57.000000 lifetimefitting-0.0.19/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:51:57.206711 lifetimefitting-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-28 14:51:46.000000 lifetimefitting-0.0.19/setup.py
```

### Comparing `lifetimefitting-0.0.18/LICENSE.md` & `lifetimefitting-0.0.19/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.18/PKG-INFO` & `lifetimefitting-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.18
+Version: 0.0.19
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.18/README.md` & `lifetimefitting-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.18/app/funcs/expFuncs.py` & `lifetimefitting-0.0.19/app/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.18/app/funcs/fittingFuncs.py` & `lifetimefitting-0.0.19/app/funcs/fittingFuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import struct
 import numpy as np
 from phdimporter import TRF
 from scipy.optimize import curve_fit
 from PyQt6.QtWidgets import QFileDialog, QMessageBox, QLineEdit
-from .gui import Ui_Form
-from .expFuncs import linFuncWC, linFuncx2, linFuncx3, linFuncx4
-from .expFuncs import expFunc, expFuncWC, expFuncx2, expFuncx3, expFuncx4
+from gui import Ui_Form
+from expFuncs import linFuncWC, linFuncx2, linFuncx3, linFuncx4
+from expFuncs import expFunc, expFuncWC, expFuncx2, expFuncx3, expFuncx4
 
 
 def chiSQ(y_obs, y_pred, popt) -> float:
     dof = len(y_obs) - (len(popt))
     # ensure no divide by 0
     y_pred_max_1 = [i + 1 if i == 0 else i for i in y_pred]
     return np.sum(np.divide(np.square(np.subtract(y_obs, y_pred)), y_pred_max_1)) / len(y_pred)
@@ -61,14 +61,15 @@
                            )
 
     residual = np.sum(np.subtract(y, FLFuncList[expCount](x, *popt)))
 
     return popt, residual
 
 def fitFL(ui, plot=True, x_in=None, y_in=None, irf_in=None) -> None:
+    
     csv = 'x,y_lin,y_log\n'
     csvTail = '\n'
     outPrint = ''
     maxIter = ui.maxIter_widg.value()
     binSize = ui.binSize_widg.value()
     expCount = ui.expCount_widg.value()
 
@@ -188,19 +189,21 @@
                 ui.axList += ui.ax1.plot(x_func, expFuncWC(x_func, I0, τ, c), 'g--', lw=0.5)
                 ui.axList += ui.ax3.plot(x_func, expFuncWC(x_func, I0, τ, c), 'g--', lw=0.5)
             else:
                 ui.axList += ui.ax1.plot(x_func, expFunc(x_func, I0, τ), 'g--', lw=0.5)
                 ui.axList += ui.ax3.plot(x_func, expFunc(x_func, I0, τ), 'g--', lw=0.5)
         ui.axList += ui.ax1.plot(x_func, FLFuncList[expCount](x_func, *popt), 'k--', lw=1)
         ui.axList += ui.ax3.plot(x_func, FLFuncList[expCount](x_func, *popt), 'k--', lw=1)
-        # ax1.scatter([d], [I0], c='purple')
+
         residualList = np.subtract(FLLinFuncList[expCount](x, *popt), np.log(y))
         ui.axList += [ui.ax2.scatter(x, residualList, s=0.1, c='b')]
         residualList = np.subtract(FLFuncList[expCount](x, *popt), y,)
         ui.axList += [ui.ax4.scatter(x, residualList, s=0.1, c='b')]
+        
+
         ui.canvas.draw()
         ui.text_output.setText(outPrint)
 
         for x, y_lin, y_log in zip(x_in, FLFuncList[expCount](x_raw, *popt), FLLinFuncList[expCount](x_raw, *popt)):
             csv += f'{x},{y_lin},{y_log}\n'
         csv += f'\n{csvTail}'
```

### Comparing `lifetimefitting-0.0.18/app/funcs/gui.py` & `lifetimefitting-0.0.19/app/funcs/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.18/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.19/app/lifetimefitting/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import matplotlib.pyplot as plt
 from PyQt6 import QtWidgets
 from PyQt6.QtWidgets import QFileDialog
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from phdimporter import TRF
 from funcs.gui import Ui_Form
 from funcs.fittingFuncs import loadAndCull, fitFL
+import sys
 
 def plotFL():
     global csv
+    plt.close('all')
     for i in ui.axList:
         i.remove()
     ui.axList = []
+    ui.ax1.relim()
+    ui.ax1.autoscale_view()
+    ui.ax2.relim()
+    ui.ax2.autoscale_view()
+    ui.ax3.relim()
+    ui.ax3.autoscale_view()
+    ui.ax4.relim()
+    ui.ax4.autoscale_view()
     _, irf, loaded1 = loadAndCull(ui.irf_file, ui)
     x, y, loaded2 = loadAndCull(ui.trf_file, ui)
     if loaded1 and loaded2:
         csv = fitFL(ui, x_in=x, y_in=y, irf_in=irf)
 
 def trf_browse():
     ui.trf_file.setText(file_dialog.getOpenFileName(directory="/Users/adrea/gdrive/Monash/PhD/Fluorophore/data/tr/AAQ", filter="PicoHarp binary of text file (*.phd *.txt)")[0])
@@ -37,15 +47,14 @@
     ui.axList = []
 
     # log plot
     ui.ax1.set_yscale('log')
     ui.ax1.set_ylim(1e-1, 1e5, auto=False)
     ui.ax1.axhline(0, c='k', lw=0.5)
     ui.ax1.axvline(0, c='k', lw=0.5)
-    ui.ax1.set_xlabel('Time (ns)')
     ui.ax1.set_ylabel('Counts')
     # linear plot
     ui.ax3.set_ylabel('Counts')
     ui.ax3.axvline(0, c='k', lw=0.5)
     # log residuals
     ui.ax2.set_ylabel('Residuals\n(exp)')
     ui.ax2.axvline(0, c='k', lw=0.5)
@@ -68,15 +77,14 @@
         save_csv_dialog = QFileDialog()
         name = save_csv_dialog.getSaveFileName(filter="CSV Sheet (*.csv)")[0]
         if name != '':
             with open(name, 'w+') as f:
                 f.writelines(csv)
 
 if __name__ == "__main__":
-    import sys
     app = QtWidgets.QApplication(sys.argv)
     Form = QtWidgets.QWidget()
     ui = Ui_Form()
     ui.setupUi(Form)
     setupPlot()
 
     # file loading
```

### Comparing `lifetimefitting-0.0.18/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.19/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.18
+Version: 0.0.19
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.18/setup.py` & `lifetimefitting-0.0.19/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.18",
+    version = "0.0.19",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

