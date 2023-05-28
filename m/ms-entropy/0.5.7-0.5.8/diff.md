# Comparing `tmp/ms_entropy-0.5.7.tar.gz` & `tmp/ms_entropy-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.7.tar", last modified: Tue May 16 23:36:49 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.8.tar", last modified: Sun May 28 06:21:42 2023, max compression
```

## Comparing `ms_entropy-0.5.7.tar` & `ms_entropy-0.5.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.7/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.7/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.7/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.007383 ms_entropy-0.5.7/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-13 02:10:56.000000 ms_entropy-0.5.7/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-15 19:49:33.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    28087 2023-05-16 23:34:52.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/file_io/
--rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.7/ms_entropy/file_io/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/lbm2_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/mgf_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/msp_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     3916 2023-05-16 23:31:01.000000 ms_entropy-0.5.7/ms_entropy/file_io/mzml_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/shared.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-15 19:09:34.000000 ms_entropy-0.5.7/ms_entropy/file_io/spec_file.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/tools.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       85 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.7/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1682 2023-05-16 23:36:30.000000 ms_entropy-0.5.7/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/
+-rw-rw-r--   0 yli       (1000) yli       (1000)    11357 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3396 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    28087 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1728 2023-05-28 06:20:51.000000 ms_entropy-0.5.8/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3916 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       85 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1682 2023-05-28 06:21:13.000000 ms_entropy-0.5.8/setup.py
```

### Comparing `ms_entropy-0.5.7/LICENSE` & `ms_entropy-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/README.md` & `ms_entropy-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 You can find the benchmark results and the original code used in our manuscript under the `manuscript` folder here: [manuscript](https://github.com/YuanyueLi/FlashEntropySearch/tree/main/manuscript).
 
 We are continuously improving the code, and the latest version of the code can be found under the `ms_entropy` folder.
 
 You can find a brief introduction below, or you can find a more detailed documentation here: [https://flashentropysearch.readthedocs.io](https://flashentropysearch.readthedocs.io/).
 
+## GUI
+You can find the Graphical user interface (GUI) here: [Entropy Search](https://github.com/YuanyueLi/EntropySearch/releases)
+
 ## In brief
 
 ### Installation
 
 Python >= 3.8, C compiler and Python development headers are required.
 
 ```bash
```

### Comparing `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.5.8/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.5.8/ms_entropy/file_io/mgf_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,10 +42,11 @@
                     continue
                 key, value = items
                 key = key.strip().lower()
                 value = value.strip()
                 spectrum_info[key] = value
             else:
                 items = line.split()
-                spectrum_info['peaks'].append([items[0], items[1]])
+                if len(items)>=2:
+                    spectrum_info['peaks'].append([items[0], items[1]])
 
     fi.close()
```

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.5.8/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.5.8/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/shared.py` & `ms_entropy-0.5.8/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.5.8/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.pyx` & `ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy/tools/tools.py` & `ms_entropy-0.5.8/ms_entropy/tools/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.5.8/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.7/setup.py` & `ms_entropy-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.7',
+    version='0.5.8',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=find_packages(where='.', exclude=['tests', 'docs', 'examples', 'manuscript', 'dist', 'build']),
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
```

