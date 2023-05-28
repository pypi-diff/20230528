# Comparing `tmp/toha_nearest_neighbor-0.3.0.tar.gz` & `tmp/toha_nearest_neighbor-0.4.0.tar.gz`

## Comparing `toha_nearest_neighbor-0.3.0.tar` & `toha_nearest_neighbor-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.3.0/local_dependencies/macros/Cargo.toml
--rw-r--r--   0     1001      123     2509 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/local_dependencies/macros/src/lib.rs
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     1115 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/.github/workflows/gh-pages.yml
--rw-r--r--   0     1001      123     1772 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/.github/workflows/python.yml
--rw-r--r--   0     1001      123       50 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/.gitignore
--rw-r--r--   0     1001      123    35149 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/LICENSE
--rw-r--r--   0     1001      123       80 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/MANIFEST.in
--rw-r--r--   0     1001      123      752 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/README.md
--rw-r--r--   0     1001      123     3061 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/benches/brute_force.rs
--rw-r--r--   0     1001      123     2356 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/benches/tree.rs
--rw-r--r--   0     1001      123      638 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/docs/make.bat
--rw-r--r--   0     1001      123     1006 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/docs/source/conf.py
--rw-r--r--   0     1001      123     1132 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/docs/source/index.rst
--rw-r--r--   0     1001      123      330 2023-03-02 21:29:20.000000 toha_nearest_neighbor-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123     5695 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/scripts/plots.py
--rw-r--r--   0     1001      123     8265 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/src/brute_force.rs
--rw-r--r--   0     1001      123     4328 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123    10718 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/src/pybind.rs
--rw-r--r--   0     1001      123     7837 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/src/tree.rs
--rw-r--r--   0     1001      123      674 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/src/validate_bindings.py
--rw-r--r--   0     1001      123   302368 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/static/benchmarks.png
--rw-r--r--   0     1001      123      557 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/toha_nearest_neighbor.pyi
--rwxr-xr-x   0     1001      123      502 2023-03-02 21:29:17.000000 toha_nearest_neighbor-0.3.0/update_python_version.sh
--rw-r--r--   0     1001      123    25366 2023-03-02 21:30:31.000000 toha_nearest_neighbor-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.4.0/local_dependencies/macros/Cargo.toml
+-rw-r--r--   0     1001      123     2509 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/local_dependencies/macros/src/lib.rs
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123       70 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/.cargo/config
+-rw-r--r--   0     1001      123     1115 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0     1001      123     1772 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/.github/workflows/python.yml
+-rw-r--r--   0     1001      123       72 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/LICENSE
+-rw-r--r--   0     1001      123       80 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/MANIFEST.in
+-rw-r--r--   0     1001      123      752 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/README.md
+-rw-r--r--   0     1001      123     3061 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/benches/brute_force.rs
+-rw-r--r--   0     1001      123     2356 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/benches/tree.rs
+-rw-r--r--   0     1001      123      638 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/docs/make.bat
+-rw-r--r--   0     1001      123     1006 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/docs/source/conf.py
+-rw-r--r--   0     1001      123     1132 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/docs/source/index.rst
+-rw-r--r--   0     1001      123      330 2023-05-28 08:39:31.000000 toha_nearest_neighbor-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123    50438 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/scripts/plots.jl
+-rw-r--r--   0     1001      123     8524 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/scripts/plots.py
+-rw-r--r--   0     1001      123     8265 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/src/brute_force.rs
+-rw-r--r--   0     1001      123     4328 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123    10872 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/src/pybind.rs
+-rw-r--r--   0     1001      123     7837 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/src/tree.rs
+-rw-r--r--   0     1001      123      674 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/src/validate_bindings.py
+-rw-r--r--   0     1001      123     3287 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/static/benchmarks.json
+-rw-r--r--   0     1001      123   302368 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/static/benchmarks.png
+-rw-r--r--   0     1001      123      557 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/toha_nearest_neighbor.pyi
+-rwxr-xr-x   0     1001      123      502 2023-05-28 08:39:29.000000 toha_nearest_neighbor-0.4.0/update_python_version.sh
+-rw-r--r--   0     1001      123    25632 2023-05-28 08:40:58.000000 toha_nearest_neighbor-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 toha_nearest_neighbor-0.4.0/PKG-INFO
```

### Comparing `toha_nearest_neighbor-0.3.0/local_dependencies/macros/src/lib.rs` & `toha_nearest_neighbor-0.4.0/local_dependencies/macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/Cargo.toml` & `toha_nearest_neighbor-0.4.0/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "toha_nearest_neighbor"
-version = "0.3.0"
+version = "0.4.0"
 edition = "2021"
 
 [lib]
 name = "toha_nearest_neighbor"
 crate-type = ["cdylib", "rlib"]
 
 # pybind.rs/brute_force for some reason is interpereted as a doctest
@@ -31,7 +31,9 @@
 
 [[bench]]
 name = "tree"
 harness = false
 
 [profile.release]
 lto = "fat"
+codegen-units = 1
+panic = "abort"
```

### Comparing `toha_nearest_neighbor-0.3.0/.github/workflows/gh-pages.yml` & `toha_nearest_neighbor-0.4.0/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/.github/workflows/python.yml` & `toha_nearest_neighbor-0.4.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/LICENSE` & `toha_nearest_neighbor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/README.md` & `toha_nearest_neighbor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/benches/brute_force.rs` & `toha_nearest_neighbor-0.4.0/benches/brute_force.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/benches/tree.rs` & `toha_nearest_neighbor-0.4.0/benches/tree.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/docs/Makefile` & `toha_nearest_neighbor-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/docs/make.bat` & `toha_nearest_neighbor-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/docs/source/conf.py` & `toha_nearest_neighbor-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/docs/source/index.rst` & `toha_nearest_neighbor-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/scripts/plots.py` & `toha_nearest_neighbor-0.4.0/scripts/plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import toha_nearest_neighbor as toha
 import matplotlib.pyplot as plt
 from sklearn.neighbors import NearestNeighbors
 import numpy as np
-from typing import Tuple
+from typing import Tuple, Callable
 import time
-from statistics import mean
+from statistics import mean, median
 import math
 from scipy.spatial import KDTree
+import json
 
 DIM = 2
 
 def create_data(line_ct: int, point_ct: int) -> Tuple[np.ndarray, np.ndarray]:
     line_pts = np.random.rand(line_ct, DIM)
     cloud_pts = np.random.rand(point_ct, DIM)
 
@@ -78,27 +79,42 @@
 
     for _ in range(times):
         start = time.time()
         fn()
         end = time.time()
         runtimes.append(end - start)
 
-    return mean(runtimes)
+    return median(runtimes)
 
-def bench_helper(fn, output_list: list[float]):
-    out_mean = bench(fn, 10)
+def bench_helper(fn, size, output_list: list[float]):
+    if size < 500:
+        times = 500
+    elif size < 2000:
+        times = 40
+    else:
+        times = 10
+
+    out_mean = bench(fn, times)
 
     print(f"mean runtime was {out_mean}")
 
     # convert the mean time to ms
     output_list.append(out_mean)
 
+def bench_one(line_sizes: list[int], cloud_sizes:list[int], fn: Callable[..., None]):
+    out = []
+    for lines_ct,  clouds_ct in zip(line_sizes, cloud_sizes):
+        lines, clouds = create_data(lines_ct, clouds_ct)
+        l = lambda: fn(lines, clouds)
+        bench_helper(l, out)
+
+    return out
 
 def bench_all():
-    line_sizes = [100, 500, 1000, 5_000, 10_000, 15_000, 20_000, 30_000]
+    line_sizes = [100, 200, 300, 500, 600, 700, 800, 900, 1_000, 2_000, 4_000, 5_000, 10_000, 30_000]
     #line_sizes = [100, 500, 1000]
     cloud_sizes = line_sizes.copy()
 
     python_brute= []
     numpy_brute= []
     scikit_brute = []
     scikit_kd = []
@@ -114,83 +130,164 @@
 
     for (line_size, cloud_size) in zip(line_sizes, cloud_sizes):
         lines, clouds = create_data(line_size, cloud_size)
 
         xs.append(line_size * cloud_size)
 
         # python brute
-        if line_size <= 5_000:
+        if line_size <= 500:
             python_xs.append(line_size * cloud_size)
 
             l = lambda : bench_python_brute(lines, clouds)
-            bench_helper(l, python_brute)
+            bench_helper(l, line_size, python_brute)
 
         # numpy brute
         l = lambda : bench_numpy_brute(lines, clouds)
-        bench_helper(l, numpy_brute)
+        bench_helper(l, line_size, numpy_brute)
 
         # scikit brute
         l = lambda : bench_scikit(lines, clouds, "brute")
-        bench_helper(l, scikit_brute)
+        bench_helper(l, line_size, scikit_brute)
 
         # scikit kd
         l = lambda : bench_scikit(lines, clouds, "kd_tree")
-        bench_helper(l, scikit_kd)
+        bench_helper(l, line_size, scikit_kd)
 
         #scipy kd
         l = lambda : bench_scipy(lines, clouds, False)
-        bench_helper(l, scipy_kd)
+        bench_helper(l, line_size, scipy_kd)
 
         #scipy kd compact
         l = lambda : bench_scipy(lines, clouds, True)
-        bench_helper(l, scipy_kd_compact)
+        bench_helper(l, line_size, scipy_kd_compact)
 
         # rust brute serial
         l = lambda : bench_rust_brute(lines, clouds, False)
-        bench_helper(l, rust_brute)
+        bench_helper(l, line_size, rust_brute)
 
         # rust kd serial
         l = lambda : bench_rust_kd(lines, clouds, False)
-        bench_helper(l, rust_kd)
+        bench_helper(l, line_size, rust_kd)
 
         # rust brute parallel
         l = lambda : bench_rust_brute(lines, clouds, True)
-        bench_helper(l, rust_brute_par)
+        bench_helper(l, line_size, rust_brute_par)
 
         # rust kd parallel
         l = lambda : bench_rust_kd(lines, clouds, True)
-        bench_helper(l, rust_kd_par)
+        bench_helper(l, line_size, rust_kd_par)
 
         print(f"finished size {line_size} | {cloud_size}")
 
-    fig = plt.figure(figsize = (8, 6), dpi=300)
-    ax = fig.add_subplot(1, 1, 1)
-    ax.set_xlabel("total point size (num neighbors * num point cloud)")
-    ax.set_ylabel("runtime [s]")
-
-    ax.set_yscale('log')
-    ax.set_xscale('log')
-
-    style_brute = "solid"
-    style_kd = "dashed"
-
-    ax.plot(python_xs, python_brute, label = "python brute", color = "black", linestyle = style_brute)
-    ax.plot(xs, numpy_brute, label = "numpy brute", color = "blue", linestyle = style_brute)
+    results = {
+        "x" :xs,
+        "python_x": python_xs,
+        "python_brute_numpy_index": python_brute,
+        "numpy_brute": numpy_brute,
+        "scikit_brute": scikit_brute,
+        "scikit_kd": scikit_kd,
+        "scipy_kd": scipy_kd,
+        "scipy_kd_compact": scipy_kd_compact,
+        "rust_brute": rust_brute,
+        "rust_kd": rust_kd,
+        "rust_brute_par": rust_brute_par,
+        "rust_kd_par": rust_kd_par,
+    }
+
+    with open("./static/benchmarks.json", "w") as f:
+        json.dump(results, f)
+
+    #fig = plt.figure(figsize = (8, 6), dpi=300)
+    #ax = fig.add_subplot(1, 1, 1)
+    #ax.set_xlabel("total point size (num neighbors * num point cloud)")
+    #ax.set_ylabel("runtime [s]")
+
+    #ax.set_yscale('log')
+    #ax.set_xscale('log')
+
+    #style_brute = "solid"
+    #style_kd = "dashed"
+
+    #ax.plot(python_xs, python_brute, label = "python brute", color = "black", linestyle = style_brute)
+    #ax.plot(xs, numpy_brute, label = "numpy brute", color = "blue", linestyle = style_brute)
+
+    #ax.plot(xs, scikit_brute, label = "scikit brute", color = "green", linestyle = style_brute)
+    #ax.plot(xs, scikit_kd, label = "scikit kd", color = "green", linestyle = style_kd)
+
+    #ax.plot(xs, scipy_kd, label = "scipy kd", color = "cyan", linestyle = style_kd)
+    #ax.plot(xs, scipy_kd_compact, label = "scipy kd compact", color = "grey", linestyle = style_kd)
+
+    #ax.plot(xs, rust_brute, label = "rust brute", color = "red", linestyle=style_brute)
+    #ax.plot(xs, rust_kd, label = "rust kd", color = "red", linestyle=style_kd)
 
-    ax.plot(xs, scikit_brute, label = "scikit brute", color = "green", linestyle = style_brute)
-    ax.plot(xs, scikit_kd, label = "scikit kd", color = "green", linestyle = style_kd)
+    #ax.plot(xs, rust_brute_par, label = "rust brute parallel", color = "orange", linestyle = style_brute)
+    #ax.plot(xs, rust_kd_par, label = "rust kd parallel", color = "orange", linestyle = style_kd)
 
-    ax.plot(xs, scipy_kd, label = "scipy kd", color = "cyan", linestyle = style_kd)
-    ax.plot(xs, scipy_kd_compact, label = "scipy kd compact", color = "grey", linestyle = style_kd)
-
-    ax.plot(xs, rust_brute, label = "rust brute", color = "red", linestyle=style_brute)
-    ax.plot(xs, rust_kd, label = "rust kd", color = "red", linestyle=style_kd)
-
-    ax.plot(xs, rust_brute_par, label = "rust brute parallel", color = "orange", linestyle = style_brute)
-    ax.plot(xs, rust_kd_par, label = "rust kd parallel", color = "orange", linestyle = style_kd)
-
-    plt.legend()
-
-    plt.savefig("./static/benchmarks.png", bbox_inches="tight")
+    #plt.legend()
 
+    #plt.savefig("./static/benchmarks.png", bbox_inches="tight")
 
 bench_all()
+
+#lines : list[int] = [100, 500, 1000, 5_000, 10_000, 15_000, 20_000, 30_000]
+#clouds = lines.copy()
+#
+#print("python brute (numpy indexing)")
+#l = lambda lines,clouds: bench_python_brute(lines, clouds)
+#py_short_lines = [i for i in lines if i <= 100]
+#out = bench_one(py_short_lines, py_short_lines, l)
+#print(out)
+#
+#
+## numpy brute
+#print("numpy brute")
+#l = lambda lines,clouds: bench_numpy_brute(lines, clouds)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## scikit brute
+#print("scikit brute")
+#l = lambda lines,clouds: bench_scikit(lines, clouds, "brute")
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## scikit kd
+#print("scikit kd")
+#l = lambda lines,clouds: bench_scikit(lines, clouds, "kd_tree")
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+##scipy kd
+#print("scipy kd")
+#l = lambda lines,clouds: bench_scipy(lines, clouds, False)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+##scipy kd compact
+#print("scipy kd compact")
+#l = lambda lines,clouds: bench_scipy(lines, clouds, True)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## rust brute serial
+#print("rust brute serial")
+#l = lambda lines,clouds: bench_rust_brute(lines, clouds, False)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## rust kd serial
+#print("rust kd serial")
+#l = lambda lines,clouds: bench_rust_kd(lines, clouds, False)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## rust brute parallel
+#print("rust brute parallel")
+#l = lambda lines,clouds: bench_rust_brute(lines, clouds, True)
+#out = bench_one(lines, clouds, l)
+#print(out)
+#
+## rust kd parallel
+#print("rust kd parallel")
+#l = lambda lines,clouds: bench_rust_kd(lines, clouds, True)
+#out = bench_one(lines, clouds, l)
+#print(out)
```

### Comparing `toha_nearest_neighbor-0.3.0/src/brute_force.rs` & `toha_nearest_neighbor-0.4.0/src/brute_force.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/src/lib.rs` & `toha_nearest_neighbor-0.4.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/src/pybind.rs` & `toha_nearest_neighbor-0.4.0/src/pybind.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 #[pyfunction]
 #[pyo3(signature = (line_points, point_cloud, parallel = false))]
 /// For every point in ``point_cloud``, find it's nearest neighbor in ``line_points`` using a
 /// brute-force algorithm. Returns a tuple of the closest ``line_points`` locations and
 /// their associated distances.
 ///
-/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, 2)``
-/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, 2)``
+/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, POINT DIMENSION)``
+/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)``
 /// :param bool parallel: enable parallel processing for the dataset. If you have more than 2,000 line points and 2,000 point cloud points this may be useful.
 ///
-/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, 2)`` shaped array of the points where
+/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)`` shaped array of the points where
 /// each ``i`` th row of the returned array is a row of ``line_points`` that is closest to the
 /// ``i`` th row of ``point_cloud``
 ///
 /// Example:
 ///
 /// .. code-block::
 ///     
@@ -79,16 +79,16 @@
 
 #[pyfunction]
 #[pyo3(signature = (line_points, point_cloud, parallel = false))]
 /// For every point in ``point_cloud``, find it's nearest neighbor in ``line_points`` using a
 /// brute-force algorithm. Returns a tuple of indicies of the closest ``line_points`` rows and
 /// their associated distances.
 ///
-/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, 2)``
-/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, 2)``
+/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, POINT DIMENSION)``
+/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)``
 /// :param bool parallel: enable parallel processing for the dataset. If you have more than 2,000 line points and 2,000 point cloud points this may be useful.
 ///
 /// Example:
 ///
 /// .. code-block::
 ///     
 ///     import toha_nearest_neighbor
@@ -141,19 +141,19 @@
 
 #[pyfunction]
 #[pyo3(signature = (line_points, point_cloud, parallel = false))]
 /// For every point in ``point_cloud``, find it's nearest neighbor in ``line_points`` using a
 /// brute-force algorithm. Returns a tuple of the closest ``line_points`` locations and
 /// their associated distances.
 ///
-/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, 2)``
-/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, 2)``
+/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, POINT DIMENSION)``
+/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)``
 /// :param bool parallel: enable parallel processing for the dataset. If you have more than 2,000 line points and 2,000 point cloud points this may be useful.
 ///
-/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, 2)`` shaped array of the points where
+/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)`` shaped array of the points where
 /// each ``i`` th row of the returned array is a row of ``line_points`` that is closest to the
 /// ``i`` th row of ``point_cloud``
 ///
 /// Example:
 ///
 /// .. code-block::
 ///     
@@ -209,19 +209,19 @@
 
 #[pyfunction]
 #[pyo3(signature = (line_points, point_cloud, parallel = false))]
 /// For every point in ``point_cloud``, find it's nearest neighbor in ``line_points`` using a
 /// kd-tree algorithm. Returns a tuple of indicies of the closest ``line_points`` rows and
 /// their associated distances.
 ///
-/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, 2)``
-/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, 2)``
+/// :param np.ndarray line_points: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_LINE_POINTS, POINT DIMENSION)``
+/// :param np.ndarray point_cloud: a 2D numpy array with each point being described by a row, and columns of coordinates of that point. Array should be in the shape ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)``
 /// :param bool parallel: enable parallel processing for the dataset. If you have more than 2,000 line points and 2,000 point cloud points this may be useful.
 ///
-/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, 2)`` shaped array of the points where
+/// this function returns  a ``(NUM_POINT_CLOUD_POINTS, POINT DIMENSION)`` shaped array of the points where
 /// each ``i`` th row of the returned array is a row of ``line_points`` that is closest to the
 /// ``i`` th row of ``point_cloud``
 ///
 /// Example:
 ///
 /// .. code-block::
 ///
```

### Comparing `toha_nearest_neighbor-0.3.0/src/tree.rs` & `toha_nearest_neighbor-0.4.0/src/tree.rs`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/src/validate_bindings.py` & `toha_nearest_neighbor-0.4.0/src/validate_bindings.py`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/static/benchmarks.png` & `toha_nearest_neighbor-0.4.0/static/benchmarks.png`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/toha_nearest_neighbor.pyi` & `toha_nearest_neighbor-0.4.0/toha_nearest_neighbor.pyi`

 * *Files identical despite different names*

### Comparing `toha_nearest_neighbor-0.3.0/Cargo.lock` & `toha_nearest_neighbor-0.4.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -47,44 +47,44 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "bitflags",
  "clap_lex",
  "indexmap",
  "textwrap",
 ]
 
@@ -131,17 +131,17 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -180,17 +180,17 @@
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -221,17 +221,17 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -246,23 +246,23 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kd-tree"
 version = "0.5.1"
@@ -278,58 +278,56 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "macros"
 version = "0.1.0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -427,26 +425,26 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "ordered-float"
-version = "3.4.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d84eb1409416d254e4a9c8fa56cc24701755025b458f0fcd8e59e1f5f40c23bf"
+checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -465,17 +463,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "pdqselect"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7778906d9321dd56cde1d1ffa69a73e59dcf5fda6d366f62727adf2bd4193aee"
 
@@ -511,86 +509,86 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -635,27 +633,27 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -666,38 +664,38 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -708,37 +706,37 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.93"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -755,18 +753,29 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
@@ -778,115 +787,114 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "toha_nearest_neighbor"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "criterion",
  "kd-tree",
  "macros",
  "ndarray",
  "ndarray-rand",
  "num-traits",
  "numpy",
  "pyo3",
  "rayon",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -926,61 +934,61 @@
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `toha_nearest_neighbor-0.3.0/PKG-INFO` & `toha_nearest_neighbor-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toha_nearest_neighbor
-Version: 0.3.0
+Version: 0.4.0
 License-File: LICENSE
 Summary: 
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # toha_nearest_neighbor
 
 Serial and parallel bindings to brute force and kd-tree methods for low dimensional (<16)
```

