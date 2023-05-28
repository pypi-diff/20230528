# Comparing `tmp/gocart-0.4.1.tar.gz` & `tmp/gocart-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.4.1.tar", last modified: Thu May 25 11:32:00 2023, max compression
+gzip compressed data, was "gocart-0.4.2.tar", last modified: Sun May 28 17:00:45 2023, max compression
```

## Comparing `gocart-0.4.1.tar` & `gocart-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.750195 gocart-0.4.1/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2979 2023-05-25 11:27:47.000000 gocart-0.4.1/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-25 11:27:47.000000 gocart-0.4.1/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-25 11:27:47.000000 gocart-0.4.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-25 11:32:00.750195 gocart-0.4.1/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5499 2023-05-25 11:27:47.000000 gocart-0.4.1/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.746194 gocart-0.4.1/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10395 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.750195 gocart-0.4.1/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4198 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.750195 gocart-0.4.1/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.750195 gocart-0.4.1/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    15522 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.738194 gocart-0.4.1/gocart/resources/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.750195 gocart-0.4.1/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-25 11:27:47.000000 gocart-0.4.1/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-25 11:32:00.746194 gocart-0.4.1/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-25 11:31:00.000000 gocart-0.4.1/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-25 11:32:00.000000 gocart-0.4.1/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-25 11:32:00.750195 gocart-0.4.1/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-05-25 11:27:47.000000 gocart-0.4.1/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.241709 gocart-0.4.2/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3709 2023-05-28 16:55:56.000000 gocart-0.4.2/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-28 16:55:56.000000 gocart-0.4.2/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-28 16:55:56.000000 gocart-0.4.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-05-28 17:00:45.241709 gocart-0.4.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-05-28 16:55:56.000000 gocart-0.4.2/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.233709 gocart-0.4.2/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.237709 gocart-0.4.2/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4525 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.237709 gocart-0.4.2/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.241709 gocart-0.4.2/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16256 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.225709 gocart-0.4.2/gocart/resources/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.241709 gocart-0.4.2/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-28 16:55:56.000000 gocart-0.4.2/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-28 17:00:45.233709 gocart-0.4.2/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-28 16:59:33.000000 gocart-0.4.2/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-28 17:00:44.000000 gocart-0.4.2/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-28 17:00:45.241709 gocart-0.4.2/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-05-28 16:55:56.000000 gocart-0.4.2/setup.py
```

### Comparing `gocart-0.4.1/CHANGES.md` & `gocart-0.4.2/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 
 ## Release Notes
 
+**v0.4.2 - May 28, 2023**
+
+- **ENHANCEMENT**: added a `burst` filtering parameter. If set to True, burst event alerts will pass the filter, otherwise they filtered out (default).
+- **REFACTOR**: maps with `CREATOR: ligo-skymap-from-samples` now named on file as `bilby.multiorder.fits`.
+- **REFACTOR**: try, except added to listen parser. If an alert breaks the parser an ugly error message is reported, but the listener stays alive to listen to subsequent alerts.
+- **FIXED**: burst events causing headaches for filtering and map conversion. The first 'real' burst event provided the necessary alert packet and map to create a realistic unit test for the entire codebase. The code is now much more robust to busrt event alerts.
+
 **v0.4.1 - May 25, 2023**
 
 - **FIXED**: a bug in filtering routine that caused alerts to pass the filtering algorithm if an unknown parameter in the filtering settings was found. It now fails by default instead of passing.
 
 **0.4.0 - May 24, 2023**
 
 - **FEATURE**: gocart can now run in daemon mode. Use the commands `gocart listen|quit|restart|status`
```

### Comparing `gocart-0.4.1/LICENSE` & `gocart-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/PKG-INFO` & `gocart-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.1
+Version: 0.4.2
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.1.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.2.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gocart
 
+[![](https://zenodo.org/badge/614846695.svg)](https://zenodo.org/badge/latestdoi/614846695)  
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/pypi/v/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/conda/vn/conda-forge/gocart)](https://anaconda.org/conda-forge/gocart)
 [![](https://pepy.tech/badge/gocart)](https://pepy.tech/project/gocart)
 [![](https://img.shields.io/github/license/thespacedoctor/gocart)](https://github.com/thespacedoctor/gocart)
 
+
 <!-- STATUS BADGES -->  
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
@@ -107,8 +110,20 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## How to cite gocart
 
+If you use `gocart` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_gocart,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7970743},
+license = {GPL-3.0-only},
+title = {{gocart}},
+url = {https://github.com/thespacedoctor/gocart}
+}
+```
```

### Comparing `gocart-0.4.1/README.md` & `gocart-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # gocart
 
+[![](https://zenodo.org/badge/614846695.svg)](https://zenodo.org/badge/latestdoi/614846695)  
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/pypi/v/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/conda/vn/conda-forge/gocart)](https://anaconda.org/conda-forge/gocart)
 [![](https://pepy.tech/badge/gocart)](https://pepy.tech/project/gocart)
 [![](https://img.shields.io/github/license/thespacedoctor/gocart)](https://github.com/thespacedoctor/gocart)
 
+
 <!-- STATUS BADGES -->  
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
@@ -90,8 +93,20 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## How to cite gocart
 
+If you use `gocart` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_gocart,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7970743},
+license = {GPL-3.0-only},
+title = {{gocart}},
+url = {https://github.com/thespacedoctor/gocart}
+}
+```
```

### Comparing `gocart-0.4.1/gocart/advanced_settings.yaml` & `gocart-0.4.2/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/cl_utils.py` & `gocart-0.4.2/gocart/cl_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,14 +168,15 @@
                 self.log.info('starting the ``action`` method')
 
                 from gcn_kafka import Consumer
                 from confluent_kafka import TopicPartition
                 from gocart.parsers import lvk
 
                 firstConnect = kwargs["firstConnect"]
+                pluginsFlag = kwargs["pluginsFlag"]
 
                 from datetime import datetime, date, time
                 now = datetime.now()
                 now = now.strftime("%Y%m%dt%H%M%S")
 
                 print(f"gocart listen started at {now}")
 
@@ -210,26 +211,30 @@
                             print(f"{count} messages read ...")
                             if not len(messages):
                                 more = False
 
                         firstConnect = False
                         print(f"This is your first time using the listen command. gocart will now listen for all new incoming alerts (skipping the {count} previous alerts currently in this topic). If you stop listening and restart sometime later, gocart will immediately collect all alerts missed while off-line.")
                     for message in consumer.consume(timeout=5):
-                        parser = lvk(
-                            log=log,
-                            record=message.value(),
-                            settings=settings,
-                            plugins=a["pluginsFlag"]
-                        ).parse()
-                        consumer.commit(message)
+                        try:
+                            parser = lvk(
+                                log=log,
+                                record=message.value(),
+                                settings=settings,
+                                plugins=pluginsFlag
+                            ).parse()
+                            consumer.commit(message)
+                        except Exception as e:
+                            consumer.commit(message)
+                            log.error(f'could not parse alert! Failed with error: {e}')
 
                 self.log.info('completed the ``action`` method')
                 return None
 
-        d = myDaemon(log=log, name="gocart", firstConnect=firstConnect)
+        d = myDaemon(log=log, name="gocart", firstConnect=firstConnect, pluginsFlag=a["pluginsFlag"])
 
         if a['listen']:
             d.start()
         elif a['quit']:
             d.stop()
         elif a['restart']:
             d.restart()
```

### Comparing `gocart-0.4.1/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.4.2/gocart/commonutils/flatten_healpix_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,39 +86,46 @@
     # CREATE DATA FRAME FROM A DICTIONARY OF LISTS
     myDict = {
         f'IPIX{nside}': ipixNside,
         f'UNIQ': uniqList
     }
     upTable = pd.DataFrame(myDict)
     # MERGE DATAFRAMES
-    upTable = upTable.merge(tableData, on=['UNIQ'], how='inner')[[f'IPIX{nside}', 'PROBDENSITY', 'DISTMU', 'DISTSIGMA', 'DISTNORM']]
+    if "DISTMU" in upTable.columns:
+        upTable = upTable.merge(tableData, on=['UNIQ'], how='inner')[[f'IPIX{nside}', 'PROBDENSITY', 'DISTMU', 'DISTSIGMA', 'DISTNORM']]
+    else:
+        upTable = upTable.merge(tableData, on=['UNIQ'], how='inner')[[f'IPIX{nside}', 'PROBDENSITY']]
     pixArea = ah.nside_to_pixel_area(nside).to_value(u.steradian)
     upTable["PROB"] = upTable["PROBDENSITY"] * pixArea
     # REMOVE COLUMN FROM DATA FRAME
     upTable.drop(columns=['PROBDENSITY'], inplace=True)
 
     # DOWNSAMPLE TABLE
     mask = tableData['NSIDE'] > nside
     downTable = tableData.loc[mask].copy()
     downTable.reset_index(inplace=True)
 
     # FIND THE PIXEL INDEX AT ORDER NSIDE
     downTable[f'IPIX{nside}'] = np.floor_divide(tableData.loc[mask, 'IPIX'], np.power(4, (tableData.loc[mask, 'LEVEL'].values - level)))
     # GROUP RESULTS
-    downTable = downTable.groupby([f'IPIX{nside}']).agg({'PROB': 'sum', 'DISTMU': 'mean', 'DISTSIGMA': 'mean', 'DISTNORM': 'mean'})
+    if "DISTMU" in downTable.columns:
+        downTable = downTable.groupby([f'IPIX{nside}']).agg({'PROB': 'sum', 'DISTMU': 'mean', 'DISTSIGMA': 'mean', 'DISTNORM': 'mean'})
+    else:
+        downTable = downTable.groupby([f'IPIX{nside}']).agg({'PROB': 'sum'})
     downTable.reset_index(inplace=True)
 
     skymap = pd.concat([downTable, upTable], ignore_index=True)
     # SORT BY COLUMN NAME
     skymap.sort_values([f'IPIX{nside}'],
                        ascending=[True], inplace=True)
 
     # SET INDEX AND SORT DATA FRAME
     skymap.reset_index(inplace=True)
     skymap.drop(columns=[f'IPIX{nside}', 'index'], inplace=True)
 
     # REMOVE FILTERED ROWS FROM DATA FRAME
-    mask = (skymap['DISTMU'].isnull())
-    skymap.loc[mask, 'DISTMU'] = np.inf
+    if "DISTMU" in downTable.columns:
+        mask = (skymap['DISTMU'].isnull())
+        skymap.loc[mask, 'DISTMU'] = np.inf
 
     log.debug('completed the ``flatten_healpix_map`` function')
     return skymap
```

### Comparing `gocart-0.4.1/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.2/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/convert/aitoff.py` & `gocart-0.4.2/gocart/convert/aitoff.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/convert/ascii.py` & `gocart-0.4.2/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/convert/healpix2cart.py` & `gocart-0.4.2/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/default_settings.yaml` & `gocart-0.4.2/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/parsers/lvk.py` & `gocart-0.4.2/gocart/parsers/lvk.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,19 +148,19 @@
                 far /= 365.
                 far = f"1 per {far:0.1f} yrs"
             else:
                 far = f"1 per {far:0.1f} days"
             print(f'EVENT: {self.record["superevent_id"]} detected at {self.record["event"]["time"].replace("Z","")} UTC ({self.record["event"]["group"]})')
             print(f'ALERT: {self.record["alert_type"].replace("_"," ")} reported at {self.record["time_created"].replace("Z","")} UTC (+{timeDelta:.2f} mins)')
             print(f'FAR: {far}')
-            if "classification" in self.record['event']:
+            if "classification" in self.record['event'] and len(self.record['event']['classification']):
                 for k, v in self.record['event']['classification'].items():
                     self.record['event']['classification'][k] = float(f'{v:.2f}')
                 print(f"CLASSIFICATION: {self.record['event']['classification']}")
-            if "properties" in self.record['event']:
+            if "properties" in self.record['event'] and len(self.record['event']['properties']):
                 print(f"PROPERTIES: {self.record['event']['properties']})")
         else:
             print(f'EVENT: {self.record["superevent_id"]}')
             print(f'ALERT: {self.record["alert_type"].replace("_"," ")} reported at {self.record["time_created"].replace("Z","")} UTC')
 
         # PARSE SKY MAP
         header, extras, fitsPath = {}, {}, None
@@ -221,14 +221,16 @@
             # DUMP JSON TO FILE
             writeFile = open(jsonPath, "w")
             json.dump(self.record, writeFile, indent=4)
             writeFile.close()
 
         # WRITE SKY MAP
         if localisation:
+            if localisation == "ligo-skymap-from-samples":
+                localisation = "bilby"
             fitsPath = f"{alertDir}/{localisation}.multiorder.fits"
             with open(fitsPath, "wb") as f:
                 f.write(skymap_bytes)
 
         # WRITE META
         with open(alertDir + "/meta.yaml", 'w') as stream:
             yaml.dump(meta, stream, default_flow_style=False)
@@ -309,39 +311,48 @@
                 'alert_types',
                 "ns_lower",
                 "far_upper",
                 "dist_upper",
                 "area90_upper",
                 "hasns_lower",
                 "hasremnant_lower",
-                "event_dir_exits"
+                "event_dir_exists",
+                "burst"
             ]
 
+            # BURST EVENTS
+            if 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'group' in alert['ALERT']['event'] and alert['ALERT']['event']['group']:
+                passing = False
+                if "burst" in f and f["burst"]:
+                    passing = True
+                else:
+                    message.append(f"This is a burst event")
+
             if 'alert_types' in f and not alert['ALERT']['alert_type'].lower() in f['alert_types']:
                 passing = False
                 message.append(f"Alert type is {alert['ALERT']['alert_type'].lower()}")
-            if "ns_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'classification' in alert['ALERT']['event'] and not alert['ALERT']['event']['classification']['BNS'] + alert['ALERT']['event']['classification']['NSBH'] >= f["ns_lower"]:
+            if "ns_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'classification' in alert['ALERT']['event'] and len(alert['ALERT']['event']['classification']) and not alert['ALERT']['event']['classification']['BNS'] + alert['ALERT']['event']['classification']['NSBH'] >= f["ns_lower"]:
                 passing = False
                 message.append(f"BNS+NSBH = {alert['ALERT']['event']['classification']['BNS'] + alert['ALERT']['event']['classification']['NSBH']} (< {f['ns_lower']})")
             if "far_upper" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and not alert['ALERT']['event']['far'] < f["far_upper"]:
                 passing = False
                 message.append(f"FAR = {alert['ALERT']['event']['far']} (> {f['far_upper']})")
             if "dist_upper" in f and 'DISTMEAN' in alert['HEADER'] and alert['HEADER']['DISTMEAN'] and not alert['HEADER']['DISTMEAN'] < f["dist_upper"]:
                 passing = False
                 message.append(f"DISTMEAN = {alert['HEADER']['DISTMEAN']} (> {f['dist_upper']})")
             if "area90_upper" in f and 'EXTRA' in alert and 'area90' in alert['EXTRA'] and not alert['EXTRA']['area90'] < f["area90_upper"]:
                 passing = False
                 message.append(f"area90 = {alert['EXTRA']['area90']} (> {f['area90_upper']})")
-            if "hasns_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and not alert['ALERT']['event']['properties']['HasNS'] >= f["hasns_lower"]:
+            if "hasns_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and len(alert['ALERT']['event']['properties']) and not alert['ALERT']['event']['properties']['HasNS'] >= f["hasns_lower"]:
                 passing = False
                 message.append(f"HasNS = {alert['ALERT']['event']['properties']['HasNS']} (< {f['hasns_lower']})")
-            if "hasremnant_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and not alert['ALERT']['event']['properties']['HasRemnant'] >= f["hasremnant_lower"]:
+            if "hasremnant_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and len(alert['ALERT']['event']['properties']) and not alert['ALERT']['event']['properties']['HasRemnant'] >= f["hasremnant_lower"]:
                 passing = False
                 message.append(f"HasRemnant = {alert['ALERT']['event']['properties']['HasRemnant']} (< {f['hasremnant_lower']})")
-            if "event_dir_exits" in f:
+            if "event_dir_exists" in f:
                 if self.record["superevent_id"][0] == 'M':
                     eventDir = self.mockDir + self.record["superevent_id"]
                 else:
                     eventDir = self.eventDir + self.record["superevent_id"]
                 if not os.path.exists(eventDir):
                     passing = False
                     message.append(f"The event has not previously passed the filtering criteria")
```

### Comparing `gocart-0.4.1/gocart/resources/plugins/gp_template.py` & `gocart-0.4.2/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/setup.cfg` & `gocart-0.4.2/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart/test_settings.yaml` & `gocart-0.4.2/gocart/test_settings.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,32 @@
         nside: 16
     # WRITE ORIGINAL JSON ALERTS TO FILE?
     json: True
 
     # UP FRONT FILTERING OF ALERTS. ONLY IF AN ALERT PASSES 1 OR MORE OF THESE FILTERS WILL THE ALERT (AND ASSOCIATED ASSETS) GET WRITTEN TO FILE
     # AN ALERT MUST PASS ALL INDIVIDUAL CRITERIA WITHIN A FILTER TO PASS
     filters:
+        - name: burst
+          alert_types: [initial, update]
+          burst: True
         - name: general
-          alert_types: [initial, update, retraction]
+          alert_types: [initial, update]
           ns_lower: 0.9
           far_upper: 1.6e-08
           dist_upper: 500
           area90_upper: 2000
         - name: high significance
-          alert_types: [initial, update, retraction]
+          alert_types: [initial, update]
           ns_lower: 0.99
           far_upper: 1.6e-10
           dist_upper: 250
           hasns_lower: 0.9
           hasremnant_lower: 0.5
+        - name: live event
+          event_dir_exists: True
 
 
 gcn-kafka:
     client_id: XXXX
     client_secret: XXXX
 
 logging settings:
```

### Comparing `gocart-0.4.1/gocart/utKit.py` & `gocart-0.4.2/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/gocart.egg-info/PKG-INFO` & `gocart-0.4.2/gocart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.1
+Version: 0.4.2
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.1.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.2.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gocart
 
+[![](https://zenodo.org/badge/614846695.svg)](https://zenodo.org/badge/latestdoi/614846695)  
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/pypi/v/gocart)](https://pypi.org/project/gocart/)
 [![](https://img.shields.io/conda/vn/conda-forge/gocart)](https://anaconda.org/conda-forge/gocart)
 [![](https://pepy.tech/badge/gocart)](https://pepy.tech/project/gocart)
 [![](https://img.shields.io/github/license/thespacedoctor/gocart)](https://github.com/thespacedoctor/gocart)
 
+
 <!-- STATUS BADGES -->  
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
@@ -107,8 +110,20 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## How to cite gocart
 
+If you use `gocart` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_gocart,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7970743},
+license = {GPL-3.0-only},
+title = {{gocart}},
+url = {https://github.com/thespacedoctor/gocart}
+}
+```
```

### Comparing `gocart-0.4.1/gocart.egg-info/SOURCES.txt` & `gocart-0.4.2/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.4.1/setup.py` & `gocart-0.4.2/setup.py`

 * *Files identical despite different names*

