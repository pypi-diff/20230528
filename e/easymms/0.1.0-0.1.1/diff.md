# Comparing `tmp/easymms-0.1.0.tar.gz` & `tmp/easymms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.0.tar", last modified: Sun May 28 03:19:51 2023, max compression
+gzip compressed data, was "easymms-0.1.1.tar", last modified: Sun May 28 04:22:42 2023, max compression
```

## Comparing `easymms-0.1.0.tar` & `easymms-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:19:51.943117 easymms-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-28 03:19:38.000000 easymms-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 03:19:51.943117 easymms-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-28 03:19:38.000000 easymms-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:19:51.943117 easymms-0.1.0/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-28 03:19:38.000000 easymms-0.1.0/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-28 03:19:38.000000 easymms-0.1.0/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-28 03:19:38.000000 easymms-0.1.0/easymms/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-28 03:19:38.000000 easymms-0.1.0/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:19:51.943117 easymms-0.1.0/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 03:19:51.000000 easymms-0.1.0/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 03:19:51.947117 easymms-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-28 03:19:38.000000 easymms-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:19:51.943117 easymms-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 03:19:38.000000 easymms-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-28 03:19:38.000000 easymms-0.1.0/tests/test_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-28 04:22:31.000000 easymms-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 04:22:42.409532 easymms-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-28 04:22:31.000000 easymms-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 04:22:42.409532 easymms-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-28 04:22:31.000000 easymms-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:31.000000 easymms-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-28 04:22:31.000000 easymms-0.1.1/tests/test_asr.py
```

### Comparing `easymms-0.1.0/LICENSE` & `easymms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/PKG-INFO` & `easymms-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
```

### Comparing `easymms-0.1.0/README.md` & `easymms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/easymms/__init__.py` & `easymms-0.1.1/easymms/__init__.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/easymms/_logger.py` & `easymms-0.1.1/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/easymms/constants.py` & `easymms-0.1.1/easymms/constants.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/easymms/utils.py` & `easymms-0.1.1/easymms/utils.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.0/easymms.egg-info/PKG-INFO` & `easymms-0.1.1/easymms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
```

### Comparing `easymms-0.1.0/setup.py` & `easymms-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.0",
+    version="0.1.1",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
```

### Comparing `easymms-0.1.0/tests/test_asr.py` & `easymms-0.1.1/tests/test_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from unittest import TestCase
 
 from easymms.models.asr import ASRModel
 
 
 class TestASR(TestCase):
-    asr = ASRModel('../models/mms1b_fl102.pt')
+    asr = ASRModel('../models_dir/mms1b_fl102.pt')
     eng_files = ['../assets/eng_1.mp3', '../assets/eng_2.flac']
     ara_files = ['../assets/ara_1.ogg']
 
     def test_transcribe_eng(self):
         res = self.asr.transcribe(self.eng_files, align=True, lang='eng')
         self.assertIsNotNone(res)
         self.assertIsInstance(res, list)
```

