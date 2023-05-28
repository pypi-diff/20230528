# Comparing `tmp/soccminer-0.0.41a1.tar.gz` & `tmp/soccminer-0.0.42a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/projappl/project_2002565/soccminer_eval/soccminer/dist/tmpukcaxxp2/soccminer-0.0.41a1.tar", last modified: Sun May 28 17:02:25 2023, max compression
+gzip compressed data, was "/projappl/project_2002565/soccminer_eval/soccminer/dist/tmpsleio_e9/soccminer-0.0.42a1.tar", last modified: Sun May 28 17:42:10 2023, max compression
```

## Comparing `soccminer-0.0.41a1.tar` & `soccminer-0.0.42a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       38 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/setup.cfg
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     1136 2022-01-20 20:24:37.000000 soccminer-0.0.41a1/LICENSE
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      835 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/SOURCES.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 16:33:34.000000 soccminer-0.0.41a1/soccminer.egg-info/not-zip-safe
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/dependency_links.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/PKG-INFO
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       91 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/requires.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       10 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer.egg-info/top_level.txt
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     5182 2022-01-20 20:24:37.000000 soccminer-0.0.41a1/README.md
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/PKG-INFO
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/bin/
--rwxrwxr-x   0 sridhara (10009479) project_2002565 (2002565)    18355 2023-05-28 16:22:19.000000 soccminer-0.0.41a1/bin/main.py
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)      686 2023-05-28 17:02:16.000000 soccminer-0.0.41a1/setup.py
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:02:25.000000 soccminer-0.0.41a1/soccminer/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)   102093 2023-05-28 16:20:14.000000 soccminer-0.0.41a1/soccminer/java_ast_parsing.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    27195 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/project_meta.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      969 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/java_proj_miner.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    17071 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/java_project_meta_attributes.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     4030 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/proj_comments_main_attr.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2191 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/process_parameters.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      669 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/exception_monitoring.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     3167 2022-12-16 03:41:20.000000 soccminer-0.0.41a1/soccminer/srcml.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    23894 2023-01-12 15:01:49.000000 soccminer-0.0.41a1/soccminer/helper.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1058 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/project_attributes.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    66128 2023-05-28 16:59:08.000000 soccminer-0.0.41a1/soccminer/comments_miner.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    29129 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/source_code_details.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     6298 2023-04-03 11:08:21.000000 soccminer-0.0.41a1/soccminer/parse_source_files.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      601 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/__init__.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     7812 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/comments.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    31360 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/json_serialization.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      400 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/environment.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      647 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/performance_time.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1028 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/proj_comments_comprehensive_attr.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2886 2022-12-16 02:30:58.000000 soccminer-0.0.41a1/soccminer/soccminer_logger.py
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       38 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/setup.cfg
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     1136 2022-01-20 20:24:37.000000 soccminer-0.0.42a1/LICENSE
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      835 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/SOURCES.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 17:42:09.000000 soccminer-0.0.42a1/soccminer.egg-info/not-zip-safe
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/dependency_links.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/PKG-INFO
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       91 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/requires.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       10 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer.egg-info/top_level.txt
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     5182 2022-01-20 20:24:37.000000 soccminer-0.0.42a1/README.md
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/PKG-INFO
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/bin/
+-rwxrwxr-x   0 sridhara (10009479) project_2002565 (2002565)    18355 2023-05-28 16:22:19.000000 soccminer-0.0.42a1/bin/main.py
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)      686 2023-05-28 17:41:54.000000 soccminer-0.0.42a1/setup.py
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 17:42:10.000000 soccminer-0.0.42a1/soccminer/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)   102093 2023-05-28 16:20:14.000000 soccminer-0.0.42a1/soccminer/java_ast_parsing.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    27195 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/project_meta.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      969 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/java_proj_miner.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    17071 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/java_project_meta_attributes.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     4030 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/proj_comments_main_attr.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2191 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/process_parameters.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      669 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/exception_monitoring.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     3167 2022-12-16 03:41:20.000000 soccminer-0.0.42a1/soccminer/srcml.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    23894 2023-01-12 15:01:49.000000 soccminer-0.0.42a1/soccminer/helper.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1058 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/project_attributes.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    66128 2023-05-28 16:59:08.000000 soccminer-0.0.42a1/soccminer/comments_miner.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    29129 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/source_code_details.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     6298 2023-04-03 11:08:21.000000 soccminer-0.0.42a1/soccminer/parse_source_files.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      601 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/__init__.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     7812 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/comments.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    31360 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/json_serialization.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      400 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/environment.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      647 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/performance_time.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1028 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/proj_comments_comprehensive_attr.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2886 2022-12-16 02:30:58.000000 soccminer-0.0.42a1/soccminer/soccminer_logger.py
```

### Comparing `soccminer-0.0.41a1/LICENSE` & `soccminer-0.0.42a1/LICENSE`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer.egg-info/SOURCES.txt` & `soccminer-0.0.42a1/soccminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/README.md` & `soccminer-0.0.42a1/README.md`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/bin/main.py` & `soccminer-0.0.42a1/bin/main.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/setup.py` & `soccminer-0.0.42a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='soccminer',
-    version='0.0.41a1',
+    version='0.0.42a1',
     packages=['soccminer'],
     scripts=['bin/main.py'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Topic :: Text Processing :: Linguistic',
```

### Comparing `soccminer-0.0.41a1/soccminer/java_ast_parsing.py` & `soccminer-0.0.42a1/soccminer/java_ast_parsing.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/project_meta.py` & `soccminer-0.0.42a1/soccminer/project_meta.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/java_proj_miner.py` & `soccminer-0.0.42a1/soccminer/java_proj_miner.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/java_project_meta_attributes.py` & `soccminer-0.0.42a1/soccminer/java_project_meta_attributes.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/proj_comments_main_attr.py` & `soccminer-0.0.42a1/soccminer/proj_comments_main_attr.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/process_parameters.py` & `soccminer-0.0.42a1/soccminer/process_parameters.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/exception_monitoring.py` & `soccminer-0.0.42a1/soccminer/exception_monitoring.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/srcml.py` & `soccminer-0.0.42a1/soccminer/srcml.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/helper.py` & `soccminer-0.0.42a1/soccminer/helper.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/project_attributes.py` & `soccminer-0.0.42a1/soccminer/project_attributes.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/comments_miner.py` & `soccminer-0.0.42a1/soccminer/comments_miner.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/source_code_details.py` & `soccminer-0.0.42a1/soccminer/source_code_details.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/parse_source_files.py` & `soccminer-0.0.42a1/soccminer/parse_source_files.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/__init__.py` & `soccminer-0.0.42a1/soccminer/__init__.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/comments.py` & `soccminer-0.0.42a1/soccminer/comments.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/json_serialization.py` & `soccminer-0.0.42a1/soccminer/json_serialization.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/performance_time.py` & `soccminer-0.0.42a1/soccminer/performance_time.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/proj_comments_comprehensive_attr.py` & `soccminer-0.0.42a1/soccminer/proj_comments_comprehensive_attr.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.41a1/soccminer/soccminer_logger.py` & `soccminer-0.0.42a1/soccminer/soccminer_logger.py`

 * *Files identical despite different names*

