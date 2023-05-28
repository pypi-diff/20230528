# Comparing `tmp/xarray-beam-0.6.0.tar.gz` & `tmp/xarray-beam-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-beam-0.6.0.tar", last modified: Tue Mar 28 17:59:50 2023, max compression
+gzip compressed data, was "xarray-beam-0.6.1.tar", last modified: Sun May 28 17:47:31 2023, max compression
```

## Comparing `xarray-beam-0.6.0.tar` & `xarray-beam-0.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-03-28 17:59:50.283745 xarray-beam-0.6.0/
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-05-11 23:10:09.000000 xarray-beam-0.6.0/LICENSE
--rw-r--r--   0 shoyer   (365133) eng       (5000)      307 2023-03-28 17:59:50.283619 xarray-beam-0.6.0/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2042 2022-09-03 04:41:09.000000 xarray-beam-0.6.0/README.md
--rw-r--r--   0 shoyer   (365133) eng       (5000)       99 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/pyproject.toml
--rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-03-28 17:59:50.283787 xarray-beam-0.6.0/setup.cfg
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1477 2023-03-28 17:59:40.000000 xarray-beam-0.6.0/setup.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-03-28 17:59:50.280814 xarray-beam-0.6.0/xarray_beam/
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1259 2023-03-28 17:59:40.000000 xarray-beam-0.6.0/xarray_beam/__init__.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-03-28 17:59:50.283434 xarray-beam-0.6.0/xarray_beam/_src/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      575 2021-05-11 23:10:09.000000 xarray-beam-0.6.0/xarray_beam/_src/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3507 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/combiners.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4147 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/combiners_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    17033 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/core.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    18245 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/core_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5389 2022-09-27 21:22:06.000000 xarray-beam-0.6.0/xarray_beam/_src/integration_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4688 2022-09-27 21:22:06.000000 xarray-beam-0.6.0/xarray_beam/_src/pangeo_forge.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6725 2022-09-27 21:22:06.000000 xarray-beam-0.6.0/xarray_beam/_src/pangeo_forge_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    19755 2023-03-28 17:59:40.000000 xarray-beam-0.6.0/xarray_beam/_src/rechunk.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    26966 2023-03-28 17:59:40.000000 xarray-beam-0.6.0/xarray_beam/_src/rechunk_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3283 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/test_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3805 2022-09-27 21:22:06.000000 xarray-beam-0.6.0/xarray_beam/_src/threadmap.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2756 2022-09-27 21:22:06.000000 xarray-beam-0.6.0/xarray_beam/_src/threadmap_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    15985 2022-11-18 23:13:26.000000 xarray-beam-0.6.0/xarray_beam/_src/zarr.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    12066 2023-02-08 01:59:34.000000 xarray-beam-0.6.0/xarray_beam/_src/zarr_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-03-28 17:59:50.281432 xarray-beam-0.6.0/xarray_beam.egg-info/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      307 2023-03-28 17:59:49.000000 xarray-beam-0.6.0/xarray_beam.egg-info/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)      707 2023-03-28 17:59:50.000000 xarray-beam-0.6.0/xarray_beam.egg-info/SOURCES.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-03-28 17:59:50.000000 xarray-beam-0.6.0/xarray_beam.egg-info/dependency_links.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)      193 2023-03-28 17:59:50.000000 xarray-beam-0.6.0/xarray_beam.egg-info/requires.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       12 2023-03-28 17:59:50.000000 xarray-beam-0.6.0/xarray_beam.egg-info/top_level.txt
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.147050 xarray-beam-0.6.1/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-05-11 23:10:09.000000 xarray-beam-0.6.1/LICENSE
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-28 17:47:31.146874 xarray-beam-0.6.1/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2042 2022-09-03 04:41:09.000000 xarray-beam-0.6.1/README.md
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       99 2023-02-08 01:59:34.000000 xarray-beam-0.6.1/pyproject.toml
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-05-28 17:47:31.147099 xarray-beam-0.6.1/setup.cfg
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1477 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/setup.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.143113 xarray-beam-0.6.1/xarray_beam/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1259 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/__init__.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.146577 xarray-beam-0.6.1/xarray_beam/_src/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      575 2021-05-11 23:10:09.000000 xarray-beam-0.6.1/xarray_beam/_src/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3676 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/combiners.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4708 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/combiners_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    17235 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/core.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    18487 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/core_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5389 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/integration_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4688 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6725 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    19755 2023-03-28 17:59:40.000000 xarray-beam-0.6.1/xarray_beam/_src/rechunk.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    26966 2023-03-28 17:59:40.000000 xarray-beam-0.6.1/xarray_beam/_src/rechunk_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3283 2023-02-08 01:59:34.000000 xarray-beam-0.6.1/xarray_beam/_src/test_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3805 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/threadmap.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2756 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/threadmap_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    16172 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/zarr.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    12614 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/zarr_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.144043 xarray-beam-0.6.1/xarray_beam.egg-info/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      707 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      193 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/requires.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       12 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/top_level.txt
```

### Comparing `xarray-beam-0.6.0/LICENSE` & `xarray-beam-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/README.md` & `xarray-beam-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/setup.py` & `xarray-beam-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     'pangeo-forge-recipes',
     'scipy',
     'h5netcdf'
 ]
 
 setuptools.setup(
     name='xarray-beam',
-    version='0.6.0',
+    version='0.6.1',
     license='Apache 2.0',
     author='Google LLC',
     author_email='noreply@google.com',
     install_requires=base_requires,
     extras_require={
         'tests': tests_requires,
         'docs': docs_requires,
```

### Comparing `xarray-beam-0.6.0/xarray_beam/__init__.py` & `xarray-beam-0.6.1/xarray_beam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 from xarray_beam._src.zarr import (
     open_zarr,
     make_template,
     ChunksToZarr,
     DatasetToZarr,
 )
 
-__version__ = '0.6.0'
+__version__ = '0.6.1'
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/__init__.py` & `xarray-beam-0.6.1/xarray_beam/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/combiners.py` & `xarray-beam-0.6.1/xarray_beam/_src/combiners.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Combiners for xarray-beam."""
 from __future__ import annotations
 import dataclasses
-import functools
 from typing import Optional, Sequence, Union
 
 import apache_beam as beam
 import numpy.typing as npt
 import xarray
 
 from xarray_beam._src import core
@@ -78,45 +77,50 @@
 @dataclasses.dataclass
 class Mean(beam.PTransform):
   """Calculate the mean over one or more distributed dataset dimensions."""
 
   dim: Union[str, Sequence[str]]
   skipna: bool = True
   dtype: Optional[npt.DTypeLike] = None
+  fanout: Optional[int] = None
 
   def _update_key(
       self, key: core.Key, chunk: xarray.Dataset
   ) -> tuple[core.Key, xarray.Dataset]:
     dims = [self.dim] if isinstance(self.dim, str) else self.dim
     new_key = key.with_offsets(**{d: None for d in dims if d in key.offsets})
     return new_key, chunk
 
   def expand(self, pcoll):
     return (
         pcoll
         | beam.MapTuple(self._update_key)
-        | Mean.PerKey(self.dim, self.skipna, self.dtype)
+        | Mean.PerKey(self.dim, self.skipna, self.dtype, self.fanout)
     )
 
   @dataclasses.dataclass
   class Globally(beam.PTransform):
     """Calculate global mean over a pcollection of xarray.Dataset objects."""
 
     dim: DimLike = None
     skipna: bool = True
     dtype: Optional[npt.DTypeLike] = None
+    fanout: Optional[int] = None
 
     def expand(self, pcoll):
       combine_fn = MeanCombineFn(self.dim, self.skipna, self.dtype)
-      return pcoll | beam.CombineGlobally(combine_fn)
+      return pcoll | beam.CombineGlobally(combine_fn).with_fanout(self.fanout)
 
   @dataclasses.dataclass
   class PerKey(beam.PTransform):
     """Calculate per-key mean over a pcollection of (hashable, Dataset)."""
 
     dim: DimLike = None
     skipna: bool = True
     dtype: Optional[npt.DTypeLike] = None
+    fanout: Optional[int] = None
 
     def expand(self, pcoll):
       combine_fn = MeanCombineFn(self.dim, self.skipna, self.dtype)
-      return pcoll | beam.CombinePerKey(combine_fn)
+      return pcoll | beam.CombinePerKey(combine_fn).with_hot_key_fanout(
+          self.fanout
+      )
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/combiners_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/combiners_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,19 @@
       (actual,) = inputs_y | xbeam.Mean.Globally(skipna=False)
       xarray.testing.assert_allclose(expected, actual)
 
       expected = dataset.mean('x', skipna=False)
       (actual,) = inputs_x | xbeam.Mean.Globally(skipna=False)
       xarray.testing.assert_allclose(expected, actual)
 
+    with self.subTest('with-fanout'):
+      expected = dataset.mean('y', skipna=True)
+      (actual,) = inputs_y | xbeam.Mean.Globally(fanout=2)
+      xarray.testing.assert_allclose(expected, actual)
+
   def test_dim_globally(self):
     inputs = [
         xarray.Dataset({'x': ('time', [1, 2])}),
         xarray.Dataset({'x': ('time', [3])}),
     ]
     expected = xarray.Dataset({'x': 2.0})
     (actual,) = inputs | xbeam.Mean.Globally(dim='time')
@@ -90,14 +95,26 @@
         (xbeam.Key({}), xarray.Dataset({'y': 3.5})),
     ]
     actual = inputs | xbeam.Mean('x')
     self.assertAllCloseChunks(actual, expected)
     actual = inputs | xbeam.Mean(['x'])
     self.assertAllCloseChunks(actual, expected)
 
+  def test_mean_many(self):
+    inputs = []
+    for i in range(0, 100, 10):
+      inputs.append(
+          (xbeam.Key({'x': i}), xarray.Dataset({'y': ('x', i + np.arange(10))}))
+      )
+    expected = [
+        (xbeam.Key({}), xarray.Dataset({'y': 49.5})),
+    ]
+    actual = inputs | xbeam.Mean('x', fanout=2)
+    self.assertAllCloseChunks(actual, expected)
+
   def test_mean_2d(self):
     inputs = [
         (xbeam.Key({'y': 0}), xarray.Dataset({'z': (('x', 'y'), [[1, 2, 3]])})),
         (xbeam.Key({'y': 3}), xarray.Dataset({'z': (('x', 'y'), [[4, 5, 6]])})),
     ]
 
     expected = [
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/core.py` & `xarray-beam-0.6.1/xarray_beam/_src/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,16 +272,16 @@
       split_vars: bool = False,
       num_threads: Optional[int] = None,
       shard_keys_threshold: int = 200_000,
   ):
     """Initialize DatasetToChunks.
 
     Args:
-      dataset: dataset or datasets to split into (Key, xarray.Dataset) or
-        (Key, [xarray.Dataset, ...]) pairs.
+      dataset: dataset or datasets to split into (Key, xarray.Dataset) or (Key,
+        [xarray.Dataset, ...]) pairs.
       chunks: optional chunking scheme. Required if the dataset is *not* already
         chunked. If the dataset *is* already chunked with Dask, `chunks` takes
         precedence over the existing chunks.
       split_vars: whether to split the dataset into separate records for each
         data variable or to keep all data variables together. This is
         recommended if you don't need to perform joint operations on different
         dataset variables and individual variable chunks are sufficiently large.
@@ -295,16 +295,21 @@
         rather than only on the host process. This is important for scaling
         pipelines to millions of tasks.
     """
     self.dataset = dataset
     self._validate(dataset, split_vars)
     if chunks is None:
       chunks = self._first.chunks
-    if not chunks:
-      raise ValueError("dataset must be chunked or chunks must be provided")
+      if not chunks:
+        raise ValueError("dataset must be chunked or chunks must be provided")
+    for dim in chunks:
+      if not any(dim in ds.dims for ds in self._datasets):
+        raise ValueError(
+            f"chunks key {dim!r} is not a dimension on the provided dataset(s)"
+        )
     expanded_chunks = normalize_expanded_chunks(chunks, self._first.sizes)
     self.expanded_chunks = expanded_chunks
     self.split_vars = split_vars
     self.num_threads = num_threads
     self.shard_keys_threshold = shard_keys_threshold
     # TODO(shoyer): consider recalculating these potentially large properties on
     # each worker, rather than only once on the host.
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/core_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,23 +375,23 @@
     )
     self.assertIdenticalChunks(actual, expected)
 
   def test_dataset_to_chunks_empty(self):
     dataset = xarray.Dataset()
     expected = [(xbeam.Key({}), dataset)]
     actual = test_util.EagerPipeline() | xbeam.DatasetToChunks(
-        dataset, chunks={'x': -1}
+        dataset, chunks={}
     )
     self.assertIdenticalChunks(actual, expected)
 
   def test_datasets_to_chunks_empty(self):
     datasets = [xarray.Dataset() for _ in range(5)]
     expected = [(xbeam.Key({}), datasets)]
     actual = test_util.EagerPipeline() | xbeam.DatasetToChunks(
-        datasets, chunks={'x': -1}
+        datasets, chunks={}
     )
     self.assertIdenticalChunks(actual, expected)
 
   def test_task_count(self):
     dataset = xarray.Dataset({
         'foo': (('x', 'y'), np.zeros((3, 6))),
         'bar': ('x', np.zeros(3)),
@@ -439,14 +439,22 @@
 
     with self.assertRaisesWithLiteralMatch(
         ValueError, 'dataset must be chunked or chunks must be provided'
     ):
       test_util.EagerPipeline() | xbeam.DatasetToChunks(dataset, chunks=None)
 
     with self.assertRaisesWithLiteralMatch(
+        ValueError,
+        "chunks key 'invalid' is not a dimension on the provided dataset(s)",
+    ):
+      test_util.EagerPipeline() | xbeam.DatasetToChunks(
+          dataset, chunks={'invalid': 1}
+      )
+
+    with self.assertRaisesWithLiteralMatch(
         TypeError,
         "'dataset' must be an 'xarray.Dataset' or 'list[xarray.Dataset]'",
     ):
       test_util.EagerPipeline() | xbeam.DatasetToChunks({'foo': dataset})
 
     with self.assertRaisesWithLiteralMatch(
         ValueError, 'dataset list cannot be empty'
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/integration_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/integration_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/pangeo_forge.py` & `xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/pangeo_forge_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/rechunk.py` & `xarray-beam-0.6.1/xarray_beam/_src/rechunk.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/rechunk_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/rechunk_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/test_util.py` & `xarray-beam-0.6.1/xarray_beam/_src/test_util.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/threadmap.py` & `xarray-beam-0.6.1/xarray_beam/_src/threadmap.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/threadmap_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/threadmap_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/zarr.py` & `xarray-beam-0.6.1/xarray_beam/_src/zarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,17 +126,19 @@
   result = dataset.copy()
 
   # load non-lazy variables into memory
   result.update(dataset.drop_vars(lazy_vars).compute())
 
   # override the lazy variables
   delayed = dask.delayed(_raise_template_error)()
-  name = 'make_template'
   for k, v in dataset.variables.items():
     if k in lazy_vars:
+      # names of dask arrays are used for keeping track of results, so arrays
+      # with the same name cannot have different shape or dtype
+      name = f"make_template_{'x'.join(map(str, v.shape))}_{v.dtype}"
       result[k].data = dask.array.from_delayed(
           delayed, v.shape, v.dtype, name=name
       )
 
   return result
```

### Comparing `xarray-beam-0.6.0/xarray_beam/_src/zarr_test.py` & `xarray-beam-0.6.1/xarray_beam/_src/zarr_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,10 +333,24 @@
         re.escape(
             "Zarr cannot handle inconsistent chunk sizes along dimension 'x': "
             '(3, 2, 1)'
         ),
     ):
       xbeam._src.zarr._infer_zarr_chunks(dataset.chunk({'x': (3, 2, 1)}))
 
+  def test_chunks_to_zarr_docs_demo(self):
+    # verify that the ChunksToChunk demo from our docs works
+    data = np.random.RandomState(0).randn(2920, 25, 53)
+    ds = xarray.Dataset({'temperature': (('time', 'lat', 'lon'), data)})
+    chunks = {'time': 1000, 'lat': 25, 'lon': 53}
+    temp_dir = self.create_tempdir().full_path
+    (
+        test_util.EagerPipeline()
+        | xbeam.DatasetToChunks(ds, chunks)
+        | xbeam.ChunksToZarr(temp_dir)
+    )
+    result = xarray.open_zarr(temp_dir)
+    xarray.testing.assert_identical(result, ds)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `xarray-beam-0.6.0/xarray_beam.egg-info/SOURCES.txt` & `xarray-beam-0.6.1/xarray_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

