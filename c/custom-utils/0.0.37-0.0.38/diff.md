# Comparing `tmp/custom-utils-0.0.37.tar.gz` & `tmp/custom-utils-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-utils-0.0.37.tar", last modified: Sat May 27 15:27:13 2023, max compression
+gzip compressed data, was "custom-utils-0.0.38.tar", last modified: Sun May 28 12:46:00 2023, max compression
```

## Comparing `custom-utils-0.0.37.tar` & `custom-utils-0.0.38.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.837412 custom-utils-0.0.37/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.37/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-27 15:27:13.837412 custom-utils-0.0.37/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15705 2023-05-27 15:26:46.000000 custom-utils-0.0.37/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.821412 custom-utils-0.0.37/custom_utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.829412 custom-utils-0.0.37/custom_utils/alerter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/alerter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.37/custom_utils/alerter/slack.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.829412 custom-utils-0.0.37/custom_utils/configurer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/configurer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/configurer/profiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/configurer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.833413 custom-utils-0.0.37/custom_utils/connector/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/connector/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/connector/bigquery.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/connector/mongodb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.37/custom_utils/connector/mysql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.37/custom_utils/connector/s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.37/custom_utils/exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.37/custom_utils/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.825412 custom-utils-0.0.37/custom_utils.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      484 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-27 15:27:13.837412 custom-utils-0.0.37/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2023-05-27 15:27:02.000000 custom-utils-0.0.37/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.777759 custom-utils-0.0.38/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.38/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-28 12:46:00.773759 custom-utils-0.0.38/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15705 2023-05-27 15:26:46.000000 custom-utils-0.0.38/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.725758 custom-utils-0.0.38/custom_utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.745758 custom-utils-0.0.38/custom_utils/alerter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/alerter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.38/custom_utils/alerter/slack.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.757758 custom-utils-0.0.38/custom_utils/configurer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/configurer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/configurer/profiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/configurer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.769759 custom-utils-0.0.38/custom_utils/connector/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/connector/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/connector/bigquery.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/connector/mongodb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.38/custom_utils/connector/mysql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.38/custom_utils/connector/s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.38/custom_utils/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.38/custom_utils/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.737758 custom-utils-0.0.38/custom_utils.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-28 12:46:00.777759 custom-utils-0.0.38/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1373 2023-05-28 12:45:49.000000 custom-utils-0.0.38/setup.py
```

### Comparing `custom-utils-0.0.37/LICENSE` & `custom-utils-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/PKG-INFO` & `custom-utils-0.0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.37
+Version: 0.0.38
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.37 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.38 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
 mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
```

### Comparing `custom-utils-0.0.37/README.md` & `custom-utils-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/alerter/slack.py` & `custom-utils-0.0.38/custom_utils/alerter/slack.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/configurer/profiler.py` & `custom-utils-0.0.38/custom_utils/configurer/profiler.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/configurer/utils.py` & `custom-utils-0.0.38/custom_utils/configurer/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/connector/bigquery.py` & `custom-utils-0.0.38/custom_utils/connector/bigquery.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/connector/mongodb.py` & `custom-utils-0.0.38/custom_utils/connector/mongodb.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/connector/mysql.py` & `custom-utils-0.0.38/custom_utils/connector/mysql.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/connector/s3.py` & `custom-utils-0.0.38/custom_utils/connector/s3.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/exceptions.py` & `custom-utils-0.0.38/custom_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils/utils.py` & `custom-utils-0.0.38/custom_utils/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/custom_utils.egg-info/PKG-INFO` & `custom-utils-0.0.38/custom_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.37
+Version: 0.0.38
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.37 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.38 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
 mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
```

### Comparing `custom-utils-0.0.37/custom_utils.egg-info/SOURCES.txt` & `custom-utils-0.0.38/custom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.37/setup.py` & `custom-utils-0.0.38/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 EXTRAS_REQUIRE = {
     's3' : [ 'boto', 'boto3', 'joblib'],
-    'mysql':  ['SQLAlchemy', 'SQLAlchemy-JSONField',
-               'SQLAlchemy-Utils', 'mysql-connector', 'mysql-replication',],
+    'mysql':  ['SQLAlchemy', 'SQLAlchemy-JSONField', 'SQLAlchemy-Utils', 'mysql-connector-python',],
     'bigquery': ['tqdm==4.49.0','google-cloud-bigquery==2.1.0', 'pandas_gbq', 'google-cloud' ],
     'mongodb': ['pymongo==3.10.0'],
     'slack': ['slack-sdk==3.21.3'],
 }
 
 # construct special 'full' extra that adds requirements for all built-in
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     author="Rahul Kumar",
     author_email="rahulnkumar7@gmail.com",
     name='custom-utils',
     description='Utilities for database connectors, slack alerter, loggers etc',
-    version="0.0.37",
+    version="0.0.38",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RahulnKumar/custom-utils',
     packages=find_packages(),
     python_requires=">=3.6.9",
     install_requires=['python-dotenv', 'subprocess32',],
     extras_require=EXTRAS_REQUIRE,
```

