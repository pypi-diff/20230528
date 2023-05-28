# Comparing `tmp/graph_read_simulator-0.0.8.tar.gz` & `tmp/graph_read_simulator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_read_simulator-0.0.8.tar", last modified: Sun Jun 19 22:06:01 2022, max compression
+gzip compressed data, was "graph_read_simulator-0.0.9.tar", last modified: Sun Jun 19 22:09:59 2022, max compression
```

## Comparing `graph_read_simulator-0.0.8.tar` & `graph_read_simulator-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:06:01.334915 graph_read_simulator-0.0.8/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      294 2022-06-19 22:06:01.334915 graph_read_simulator-0.0.8/PKG-INFO
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:06:01.330915 graph_read_simulator-0.0.8/graph_read_simulator/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     5886 2021-11-29 20:22:06.000000 graph_read_simulator-0.0.8/graph_read_simulator/chip_seq.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    12593 2022-04-04 11:09:27.000000 graph_read_simulator-0.0.8/graph_read_simulator/command_line_interface.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     6234 2022-06-10 18:26:45.000000 graph_read_simulator-0.0.8/graph_read_simulator/diploid_reference_builder.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)      780 2019-10-02 17:23:19.000000 graph_read_simulator-0.0.8/graph_read_simulator/id_assignment.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     4541 2022-04-04 10:02:48.000000 graph_read_simulator-0.0.8/graph_read_simulator/simulation.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     6628 2022-06-19 22:05:44.000000 graph_read_simulator-0.0.8/graph_read_simulator/util.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     9313 2021-11-29 20:22:06.000000 graph_read_simulator-0.0.8/graph_read_simulator/vcf_simulation.py
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:06:01.334915 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/
--rw-------   0 ivargry   (1000) ivargry   (1000)      294 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/PKG-INFO
--rw-------   0 ivargry   (1000) ivargry   (1000)      588 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/SOURCES.txt
--rw-------   0 ivargry   (1000) ivargry   (1000)        1 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/dependency_links.txt
--rw-------   0 ivargry   (1000) ivargry   (1000)       91 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/entry_points.txt
--rw-------   0 ivargry   (1000) ivargry   (1000)        1 2020-09-25 10:38:36.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/not-zip-safe
--rw-------   0 ivargry   (1000) ivargry   (1000)       52 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/requires.txt
--rw-------   0 ivargry   (1000) ivargry   (1000)       21 2022-06-19 22:06:01.000000 graph_read_simulator-0.0.8/graph_read_simulator.egg-info/top_level.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2022-06-19 22:06:01.334915 graph_read_simulator-0.0.8/setup.cfg
--rwxrwxr-x   0 ivargry   (1000) ivargry   (1000)      822 2022-06-19 22:05:51.000000 graph_read_simulator-0.0.8/setup.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:09:59.680682 graph_read_simulator-0.0.9/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      294 2022-06-19 22:09:59.680682 graph_read_simulator-0.0.9/PKG-INFO
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:09:59.680682 graph_read_simulator-0.0.9/graph_read_simulator/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     5886 2021-11-29 20:22:06.000000 graph_read_simulator-0.0.9/graph_read_simulator/chip_seq.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    12593 2022-04-04 11:09:27.000000 graph_read_simulator-0.0.9/graph_read_simulator/command_line_interface.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     6234 2022-06-10 18:26:45.000000 graph_read_simulator-0.0.9/graph_read_simulator/diploid_reference_builder.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)      780 2019-10-02 17:23:19.000000 graph_read_simulator-0.0.9/graph_read_simulator/id_assignment.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     4491 2022-06-19 22:09:26.000000 graph_read_simulator-0.0.9/graph_read_simulator/simulation.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     6628 2022-06-19 22:05:44.000000 graph_read_simulator-0.0.9/graph_read_simulator/util.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     9313 2021-11-29 20:22:06.000000 graph_read_simulator-0.0.9/graph_read_simulator/vcf_simulation.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-06-19 22:09:59.680682 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/
+-rw-------   0 ivargry   (1000) ivargry   (1000)      294 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/PKG-INFO
+-rw-------   0 ivargry   (1000) ivargry   (1000)      588 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/SOURCES.txt
+-rw-------   0 ivargry   (1000) ivargry   (1000)        1 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/dependency_links.txt
+-rw-------   0 ivargry   (1000) ivargry   (1000)       91 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/entry_points.txt
+-rw-------   0 ivargry   (1000) ivargry   (1000)        1 2020-09-25 10:38:36.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/not-zip-safe
+-rw-------   0 ivargry   (1000) ivargry   (1000)       52 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/requires.txt
+-rw-------   0 ivargry   (1000) ivargry   (1000)       21 2022-06-19 22:09:59.000000 graph_read_simulator-0.0.9/graph_read_simulator.egg-info/top_level.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2022-06-19 22:09:59.680682 graph_read_simulator-0.0.9/setup.cfg
+-rwxrwxr-x   0 ivargry   (1000) ivargry   (1000)      822 2022-06-19 22:09:46.000000 graph_read_simulator-0.0.9/setup.py
```

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/chip_seq.py` & `graph_read_simulator-0.0.9/graph_read_simulator/chip_seq.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/command_line_interface.py` & `graph_read_simulator-0.0.9/graph_read_simulator/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/diploid_reference_builder.py` & `graph_read_simulator-0.0.9/graph_read_simulator/diploid_reference_builder.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/id_assignment.py` & `graph_read_simulator-0.0.9/graph_read_simulator/id_assignment.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/simulation.py` & `graph_read_simulator-0.0.9/graph_read_simulator/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 import logging
 logging.basicConfig(level=logging.INFO, format="%(asctime)s, %(levelname)s: %(message)s")
 from pyfaidx import Fasta
-from offsetbasedgraph import NumpyIndexedInterval
 from numpy.random import randint
 import numpy as np
 from simple_read_mutator import Mutator
 from Bio.Seq import Seq
 
 
 class OneToOneCoordinateMap:
```

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/util.py` & `graph_read_simulator-0.0.9/graph_read_simulator/util.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator/vcf_simulation.py` & `graph_read_simulator-0.0.9/graph_read_simulator/vcf_simulation.py`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/graph_read_simulator.egg-info/SOURCES.txt` & `graph_read_simulator-0.0.9/graph_read_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graph_read_simulator-0.0.8/setup.py` & `graph_read_simulator-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='graph_read_simulator',
-      version='0.0.8',
+      version='0.0.9',
       description='Graph Read Simulator',
       url='http://github.com/ivargr/graph_read_simulator',
       author='Ivar Grytten',
       author_email='',
       license='MIT',
       packages=['graph_read_simulator'],
       zip_safe=False,
```

