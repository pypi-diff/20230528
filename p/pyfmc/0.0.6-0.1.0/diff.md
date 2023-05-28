# Comparing `tmp/pyfmc-0.0.6.tar.gz` & `tmp/pyfmc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmc-0.0.6.tar", last modified: Sun May  7 12:51:13 2023, max compression
+gzip compressed data, was "pyfmc-0.1.0.tar", last modified: Sun May 28 08:31:57 2023, max compression
```

## Comparing `pyfmc-0.0.6.tar` & `pyfmc-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.352846 pyfmc-0.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 12:51:13.352846 pyfmc-0.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-06 14:11:21.000000 pyfmc-0.0.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/common/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/common/historical_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/simulations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/simulations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-05-07 12:49:37.000000 pyfmc-0.0.6/pyfmc/simulations/gbm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.352846 pyfmc-0.0.6/pyfmc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-07 12:51:13.352846 pyfmc-0.0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-05-07 12:49:37.000000 pyfmc-0.0.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 08:31:57.844532 pyfmc-0.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3018 2023-05-28 08:31:57.844532 pyfmc-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1887 2023-05-28 08:31:42.000000 pyfmc-0.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 08:31:57.836531 pyfmc-0.1.0/pyfmc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 13:51:16.000000 pyfmc-0.1.0/pyfmc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 08:31:57.840532 pyfmc-0.1.0/pyfmc/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 13:51:16.000000 pyfmc-0.1.0/pyfmc/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 13:51:16.000000 pyfmc-0.1.0/pyfmc/common/historical_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 13:51:16.000000 pyfmc-0.1.0/pyfmc/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 08:31:57.840532 pyfmc-0.1.0/pyfmc/simulations/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 13:51:16.000000 pyfmc-0.1.0/pyfmc/simulations/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4728 2023-05-28 08:31:42.000000 pyfmc-0.1.0/pyfmc/simulations/gbm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 08:31:57.844532 pyfmc-0.1.0/pyfmc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3018 2023-05-28 08:31:57.000000 pyfmc-0.1.0/pyfmc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-05-28 08:31:57.000000 pyfmc-0.1.0/pyfmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-28 08:31:57.000000 pyfmc-0.1.0/pyfmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-28 08:31:57.000000 pyfmc-0.1.0/pyfmc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-28 08:31:57.000000 pyfmc-0.1.0/pyfmc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-28 08:31:57.844532 pyfmc-0.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      714 2023-05-28 08:31:42.000000 pyfmc-0.1.0/setup.py
```

### Comparing `pyfmc-0.0.6/pyfmc/common/historical_data.py` & `pyfmc-0.1.0/pyfmc/common/historical_data.py`

 * *Files identical despite different names*

### Comparing `pyfmc-0.0.6/pyfmc/simulations/gbm.py` & `pyfmc-0.1.0/pyfmc/simulations/gbm.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,41 +2,85 @@
 from typing import Optional
 from math import sqrt
 
 import torch
 import numpy as np
 import pandas as pd
 from tqdm import trange
+import seaborn as sns
+import matplotlib.pyplot as plt
 
 from . import Simulations
 from ..exceptions import SimulationException
 from ..common import HistoricalData, get_device
 
 logger = logging.getLogger("pyfmc.simulations.gbm")
 
 
+class Trajectory:
+    def __init__(self, dist: torch.Tensor, label: str = "Trajectory") -> None:
+        self.dist = dist
+        self.label = label
+
+    def value(self):
+        return self.dist
+
+    def plot(self, title=None, xlabel=None, ylabel=None):
+        fig, ax = plt.subplots()
+        sns.lineplot(data=self.dist, legend=False)
+        ax.set_xlabel(xlabel or "time")
+        ax.set_ylabel(ylabel or self.label)
+        ax.set_title(title or self.label)
+        return ax
+
+
+class Distribution:
+    def __init__(self, dist: torch.Tensor, label: str = "Distribution"):
+        self.dist = dist.numpy()
+        self.label = label
+
+    def value(self):
+        return self.dist
+
+    def plot(self, bins=10, kde=False, title=None, xlabel=None, ylabel=None):
+        fig, ax = plt.subplots()
+        if kde:
+            sns.kdeplot(data=self.dist, color="blue", fill=True, ax=ax)
+        else:
+            sns.histplot(self.dist, bins=bins, ax=ax)
+        ax.set_xlabel(xlabel or self.label)
+        ax.set_ylabel(ylabel or ("Density" if kde else "Counts"))
+        ax.set_title(title or self.label)
+        return ax
+
+    def __str__(self) -> str:
+        return str(self.dist)
+
+
 class GBMResult:
     def __init__(
         self, init_dist: torch.Tensor, final_dist: torch.Tensor, trajectories: Optional[torch.Tensor] = None
     ) -> None:
         self.init_dist = init_dist.cpu()
         self.final_dist = final_dist.cpu()
         self._trajectories = trajectories.cpu() if trajectories is not None else trajectories
 
     def price_distribution(self):
-        return self.final_dist.numpy()
+        return Distribution(self.final_dist, label="Price Distribution")
 
     def trajectories(self):
         if self._trajectories is None:
             logger.warning("No trajectories")
             return
-        return self._trajectories.numpy()
+        return Trajectory(self._trajectories)
 
     def return_distribution(self):
-        return torch.div(torch.sub(self.final_dist, self.init_dist), self.init_dist).numpy()
+        return Distribution(
+            torch.div(torch.sub(self.final_dist, self.init_dist), self.init_dist), label="Return Distribution"
+        )
 
     def VaR(self, alpha: float):
         return np.percentile(self.return_distribution(), alpha)
 
 
 class GBM(Simulations):
     def __init__(
@@ -58,35 +102,35 @@
         self.n_trajectories = n_trajectories
         if (open_index and close_index) not in df.columns:
             raise SimulationException("Wrong open_index or close_index")
 
     def simulate(self):
         hist_data = HistoricalData(self.df, self.open_index, self.close_index)
         device = get_device() if self.device_acc else torch.device("cpu")
+        dtype = torch.float32 if device == torch.device("mps") else torch.float64
         logger.info("Using device: %s", device)
 
-        exp_return = torch.tensor(hist_data.return_mean, device=device)
-        std_return = torch.tensor(hist_data.return_std, device=device)
+        exp_return = torch.tensor(hist_data.return_mean, device=device, dtype=dtype)
+        std_return = torch.tensor(hist_data.return_std, device=device, dtype=dtype)
         last_price = hist_data.get_latest_close_price()
 
-        s0 = torch.tensor([last_price for _ in range(self.n_walkers)], device=device)
+        s0 = torch.tensor([last_price] * self.n_walkers, device=device, dtype=dtype)
         init_dist = torch.clone(s0)
         trajectories = init_dist[: self.n_trajectories] if self.n_trajectories > 0 else None
 
-        s1 = torch.zeros(self.n_walkers, device=device)
-        ds = torch.zeros(self.n_walkers, device=device)
+        s1 = torch.zeros(self.n_walkers, device=device, dtype=dtype)
+        ds = torch.zeros(self.n_walkers, device=device, dtype=dtype)
         dt = torch.tensor(self.step_size)
 
         for _ in trange(self.n_steps):
-            epsilon = torch.randn(self.n_walkers, device=device)
-            shock = torch.multiply(std_return * sqrt(dt), epsilon)
-            drift = torch.multiply(dt, exp_return)
-            _sum = torch.add(shock, drift)
-            ds = torch.multiply(_sum, s0)
-            s1 = torch.add(s0, ds)
+            epsilon = torch.randn(self.n_walkers, device=device, dtype=dtype)
+            shock = (std_return * sqrt(dt)) * epsilon
+            drift = dt * exp_return
+            ds = (shock + drift) * s0
+            s1 = s0 + ds
             s0 = torch.clone(s1)
             if self.n_trajectories > 0:
                 trajectories = torch.concat((trajectories, s0[: self.n_trajectories]))
 
         s0 = s0[torch.isfinite(s0)]
         return GBMResult(
             init_dist,
```

### Comparing `pyfmc-0.0.6/setup.py` & `pyfmc-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="pyfmc",
-    version="0.0.6",
+    version="0.1.0",
     author="Ethan Lee",
     author_email="ethan2000.el@gmail.com",
     description="Finance Monte-Carlo Simulation using PyTorch",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages("."),
     package_dir={"": "."},
     url="https://github.com/ethanlee928/pyfmc",
-    install_requires=["torch==2.0.0", "tqdm==4.65.0", "numpy==1.24.3", "pandas==2.0.0"],
+    install_requires=["torch==2.0.0", "tqdm==4.65.0", "numpy==1.24.3", "pandas==2.0.0", "seaborn==0.12.2"],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

