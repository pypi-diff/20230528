# Comparing `tmp/META_TOOLBOX-2023.2.tar.gz` & `tmp/META_TOOLBOX-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "META_TOOLBOX-2023.2.tar", last modified: Sun May 28 01:14:31 2023, max compression
+gzip compressed data, was "META_TOOLBOX-2023.3.tar", last modified: Sun May 28 18:20:03 2023, max compression
```

## Comparing `META_TOOLBOX-2023.2.tar` & `META_TOOLBOX-2023.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    11357 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/LICENSE
-drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/META_TOOLBOX/
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    38741 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     7901 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_CO_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      112 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_DE_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    14095 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_FA_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     6332 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_FUNCTIONS.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1410 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_GA_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    19743 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_GRAPHICS_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      929 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_HC_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     3650 2023-05-28 00:47:17.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_KNAPSACK.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1280 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_PSO_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     2544 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_SA_LIBRARY.py
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      333 2023-05-27 23:50:52.000000 META_TOOLBOX-2023.2/META_TOOLBOX/__init__.py
-drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/PKG-INFO
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      575 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)        1 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       24 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/requires.txt
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       13 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/top_level.txt
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/PKG-INFO
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      607 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/README.md
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       38 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/setup.cfg
--rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      730 2023-05-28 01:00:12.000000 META_TOOLBOX-2023.2/setup.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 18:20:03.353035 META_TOOLBOX-2023.3/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    11357 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/LICENSE
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 18:20:03.353035 META_TOOLBOX-2023.3/META_TOOLBOX/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    38741 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     7901 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_CO_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      112 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_DE_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    14095 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_FA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     6332 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_FUNCTIONS.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1410 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_GA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    19743 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_GRAPHICS_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      929 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_HC_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     3650 2023-05-28 00:47:17.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_KNAPSACK.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     2739 2023-05-28 18:19:42.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_PORTIFOLIO.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1280 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_PSO_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     2544 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/META_TOOLBOX/META_SA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      364 2023-05-28 18:19:42.000000 META_TOOLBOX-2023.3/META_TOOLBOX/__init__.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 18:20:03.353035 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 18:20:03.000000 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      607 2023-05-28 18:20:03.000000 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)        1 2023-05-28 18:20:03.000000 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       33 2023-05-28 18:20:03.000000 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/requires.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       13 2023-05-28 18:20:03.000000 META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/top_level.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 18:20:03.353035 META_TOOLBOX-2023.3/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      607 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.3/README.md
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       38 2023-05-28 18:20:03.353035 META_TOOLBOX-2023.3/setup.cfg
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      742 2023-05-28 18:19:42.000000 META_TOOLBOX-2023.3/setup.py
```

### Comparing `META_TOOLBOX-2023.2/LICENSE` & `META_TOOLBOX-2023.3/LICENSE`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_CO_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_CO_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_FA_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_FA_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_FUNCTIONS.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_FUNCTIONS.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_GA_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_GA_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_GRAPHICS_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_GRAPHICS_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_HC_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_HC_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_KNAPSACK.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_KNAPSACK.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_PSO_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_PSO_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX/META_SA_LIBRARY.py` & `META_TOOLBOX-2023.3/META_TOOLBOX/META_SA_LIBRARY.py`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/PKG-INFO` & `META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: META-TOOLBOX
-Version: 2023.2
+Version: 2023.3
 Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
 Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
 Author-email: wanderlei_junior@ufcat.edu.br
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/SOURCES.txt` & `META_TOOLBOX-2023.3/META_TOOLBOX.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 META_TOOLBOX/META_DE_LIBRARY.py
 META_TOOLBOX/META_FA_LIBRARY.py
 META_TOOLBOX/META_FUNCTIONS.py
 META_TOOLBOX/META_GA_LIBRARY.py
 META_TOOLBOX/META_GRAPHICS_LIBRARY.py
 META_TOOLBOX/META_HC_LIBRARY.py
 META_TOOLBOX/META_KNAPSACK.py
+META_TOOLBOX/META_PORTIFOLIO.py
 META_TOOLBOX/META_PSO_LIBRARY.py
 META_TOOLBOX/META_SA_LIBRARY.py
 META_TOOLBOX/__init__.py
 META_TOOLBOX.egg-info/PKG-INFO
 META_TOOLBOX.egg-info/SOURCES.txt
 META_TOOLBOX.egg-info/dependency_links.txt
 META_TOOLBOX.egg-info/requires.txt
```

### Comparing `META_TOOLBOX-2023.2/PKG-INFO` & `META_TOOLBOX-2023.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: META_TOOLBOX
-Version: 2023.2
+Version: 2023.3
 Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
 Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
 Author-email: wanderlei_junior@ufcat.edu.br
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `META_TOOLBOX-2023.2/README.md` & `META_TOOLBOX-2023.3/README.md`

 * *Files identical despite different names*

### Comparing `META_TOOLBOX-2023.2/setup.py` & `META_TOOLBOX-2023.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     	name = 'META_TOOLBOX',
-    	version = '2023.2',
+    	version = '2023.3',
 		url = 'https://wmpjrufg.github.io/META_TOOLBOX/',
     	license = 'Apache License',
     	author_email = 'wanderlei_junior@ufcat.edu.br',
     	packages = ['META_TOOLBOX'],
     	description = "The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.",
     	classifiers = ["Programming Language :: Python","Topic :: Scientific/Engineering :: Mathematics", "Topic :: Scientific/Engineering"],
-    	install_requires = ["Numpy", "Xlsxwriter", "pandas"]
+    	install_requires = ["Numpy", "Xlsxwriter", "pandas", "yfinance"]
     )
```

