# Comparing `tmp/pybe-0.0.2.tar.gz` & `tmp/pybe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybe-0.0.2.tar", last modified: Fri May 26 18:30:54 2023, max compression
+gzip compressed data, was "pybe-1.0.0.tar", last modified: Sun May 28 13:22:16 2023, max compression
```

## Comparing `pybe-0.0.2.tar` & `pybe-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:30:54.264044 pybe-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 18:30:41.000000 pybe-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-26 18:30:54.264044 pybe-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-26 18:30:41.000000 pybe-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:30:54.260044 pybe-0.0.2/pybe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:30:41.000000 pybe-0.0.2/pybe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-26 18:30:41.000000 pybe-0.0.2/pybe/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 18:30:41.000000 pybe-0.0.2/pybe/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:30:54.264044 pybe-0.0.2/pybe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-26 18:30:54.000000 pybe-0.0.2/pybe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 18:30:54.000000 pybe-0.0.2/pybe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:30:54.000000 pybe-0.0.2/pybe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 18:30:54.000000 pybe-0.0.2/pybe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 18:30:54.000000 pybe-0.0.2/pybe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-26 18:30:41.000000 pybe-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 18:30:54.264044 pybe-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 18:30:41.000000 pybe-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:22:16.380410 pybe-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 13:21:59.000000 pybe-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-28 13:22:16.380410 pybe-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-28 13:21:59.000000 pybe-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:22:16.380410 pybe-1.0.0/pybe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 13:21:59.000000 pybe-1.0.0/pybe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-28 13:21:59.000000 pybe-1.0.0/pybe/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-28 13:21:59.000000 pybe-1.0.0/pybe/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:22:16.380410 pybe-1.0.0/pybe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-28 13:22:16.000000 pybe-1.0.0/pybe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 13:22:16.000000 pybe-1.0.0/pybe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:22:16.000000 pybe-1.0.0/pybe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-28 13:22:16.000000 pybe-1.0.0/pybe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 13:22:16.000000 pybe-1.0.0/pybe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-28 13:21:59.000000 pybe-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-28 13:22:16.380410 pybe-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-28 13:21:59.000000 pybe-1.0.0/setup.py
```

### Comparing `pybe-0.0.2/LICENSE.txt` & `pybe-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybe-0.0.2/pybe/benchmark.py` & `pybe-1.0.0/pybe/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from tqdm import tqdm
 import multiprocessing as mp
 
 
 class Benchmark:
     """Benchmark any Python function
 
-    This class lets you
-    **benchmark** any Python function (with vectors of real numbers as output)
-    **store** the results in a csv (default) or excel file
-    **read** from previous benchmark results.
+    pybe.Benchmark allows you to:
+
+    * **benchmark** any Python function (with vectors of real numbers as output)
+
+    * **store** the results in a csv (default) or excel file and
+
+    * **read** from previous benchmark results.
 
     .. epigraph::
         **How it works:**
         Specify a list of inputs and apply a given function to those inputs a specified number of times
     """
 
     def __init__(self,
@@ -53,15 +56,15 @@
             if true, run the benchmark on parallel (using multiprocessing)
 
 
         Examples
         --------
         Initialize the benchmark class.
 
-        benchmark = Benchmark()
+        >>> benchmark = Benchmark()
 
         Define the function to be benchmarked. This function must take a single argument (float or string) and return
         a dictionary where each key represents one output
 
         >>> def test_function(i: int):
         >>>     return {"value": i}
 
@@ -110,30 +113,30 @@
         self._name_outputs = list(result_x.keys())
         self._result = pd.concat([pd.DataFrame(result, index=[0]) for result in self._result], ignore_index=True)
 
         if store:
             self.to_csv(name)
 
     def to_excel(self, name: str = 'benchmark'):
-        """Save results to excel (xlsx) file
+        """Save results to excel (xlsx) file (file path is file path of script)
 
         Parameters
         ----------
         name : str
-            _name of the benchmark
+            name of the benchmark
         """
         self.result.to_excel(f'{name}.xlsx')
 
     def to_csv(self, name: str = 'benchmark'):
-        """Save results to csv file
+        """Save results to csv file (file path is file path of script)
 
         Parameters
         ----------
         name : str
-            _name of the benchmark
+            name of the benchmark
         """
         self.result.to_csv(f'{name}.csv', index=False)
 
     @property
     def result(self) -> pd.DataFrame:
         """Return the result of the benchmark as a pandas DataFrame
 
@@ -141,29 +144,29 @@
         -------
         pd.DataFrame
             result of the benchmark
 
         """
         return self._result
 
-    def read_from_csv(self, benchmark_yaml_file_path: str):
+    def read_from_csv(self, benchmark_csv_file_path: str):
         """Read previous results of corresponding yaml file and store them in this instance
 
         Parameters
         ----------
-        benchmark_yaml_file_path : str
+        benchmark_csv_file_path : str
             path of benchmark yaml file
 
         Examples
         --------
         >>> benchmark = Benchmark() # initialize benchmark instance
-        >>> benchmark.read_from_csv(benchmark_csv_file_path="./benchmark1.csv") # read results
+        >>> benchmark.read_from_csv(benchmark_csv_file_path="./benchmark.csv") # read results
         >>> print(benchmark.result) # print result
         """
-        self._result = pd.read_csv(benchmark_yaml_file_path)
+        self._result = pd.read_csv(benchmark_csv_file_path)
 
     def return_outputs(self, input: float):
         return self.result.loc[self.result['Input'] == input]
 
     @property
     def inputs(self) -> List[Union[str, float]]:
         """Return the list of inputs of the benchmark
```

### Comparing `pybe-0.0.2/pybe/wrappers.py` & `pybe-1.0.0/pybe/wrappers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Decorator for the function to be benchmarked
 
 Includes
-- timer (track time for each iteration)
+
++ timer (track time for each iteration)
 
 """
 
 import time
 from functools import wraps
 
 
@@ -19,14 +20,18 @@
     func : Callable[..., Dict[Union[str, float], float]]
         function to be benchmarked which takes either a string or float as input and returns a float as output
 
     Returns
     -------
     Callable[..., Dict[Union[str, float], float]]
         function to be benchmarked with additional time needed as output
+
+    Examples
+    --------
+
     """
     @wraps(func)
     def function_with_timer(*args, **kwargs):
         start_time = time.perf_counter()
         result = func(*args, **kwargs)
         end_time = time.perf_counter()
         total_time = end_time - start_time
```

### Comparing `pybe-0.0.2/setup.py` & `pybe-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     with open('README.md') as f:
         return f.read()
 
 
 if __name__ == '__main__':
     setup(
         name='pybe',
-        version='0.0.2',
+        version='1.0.0',
         license='MIT',
-        description='Small package for benchmarking python functions',
+        description='Benchmarking python functions',
         long_description=readme(),
         long_description_content_type='text/markdown',
         author='Nicolai Palm',
         author_email='nicolaipalm@googlemail.com',
         classifiers=[
             'Programming Language :: Python :: 3',
             'License :: OSI Approved :: MIT License',
```

