# Comparing `tmp/custom-utils-0.0.38.tar.gz` & `tmp/custom-utils-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-utils-0.0.38.tar", last modified: Sun May 28 12:46:00 2023, max compression
+gzip compressed data, was "custom-utils-0.0.39.tar", last modified: Sun May 28 13:26:22 2023, max compression
```

## Comparing `custom-utils-0.0.38.tar` & `custom-utils-0.0.39.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.777759 custom-utils-0.0.38/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.38/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-28 12:46:00.773759 custom-utils-0.0.38/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15705 2023-05-27 15:26:46.000000 custom-utils-0.0.38/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.725758 custom-utils-0.0.38/custom_utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.745758 custom-utils-0.0.38/custom_utils/alerter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/alerter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.38/custom_utils/alerter/slack.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.757758 custom-utils-0.0.38/custom_utils/configurer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/configurer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/configurer/profiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/configurer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.769759 custom-utils-0.0.38/custom_utils/connector/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.38/custom_utils/connector/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/connector/bigquery.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.38/custom_utils/connector/mongodb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.38/custom_utils/connector/mysql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.38/custom_utils/connector/s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.38/custom_utils/exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.38/custom_utils/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 12:46:00.737758 custom-utils-0.0.38/custom_utils.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-28 12:46:00.000000 custom-utils-0.0.38/custom_utils.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-28 12:46:00.777759 custom-utils-0.0.38/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1373 2023-05-28 12:45:49.000000 custom-utils-0.0.38/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.774135 custom-utils-0.0.39/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.39/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16420 2023-05-28 13:26:22.774135 custom-utils-0.0.39/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15790 2023-05-28 13:00:24.000000 custom-utils-0.0.39/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.770135 custom-utils-0.0.39/custom_utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.774135 custom-utils-0.0.39/custom_utils/alerter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.39/custom_utils/alerter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.39/custom_utils/alerter/slack.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.774135 custom-utils-0.0.39/custom_utils/configurer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.39/custom_utils/configurer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/configurer/profiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/configurer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.774135 custom-utils-0.0.39/custom_utils/connector/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.39/custom_utils/connector/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/connector/bigquery.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.39/custom_utils/connector/mongodb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.39/custom_utils/connector/mysql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.39/custom_utils/connector/s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.39/custom_utils/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.39/custom_utils/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-28 13:26:22.774135 custom-utils-0.0.39/custom_utils.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16420 2023-05-28 13:26:22.000000 custom-utils-0.0.39/custom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-28 13:26:22.000000 custom-utils-0.0.39/custom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-28 13:26:22.000000 custom-utils-0.0.39/custom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      386 2023-05-28 13:26:22.000000 custom-utils-0.0.39/custom_utils.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-28 13:26:22.000000 custom-utils-0.0.39/custom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-28 13:26:22.774135 custom-utils-0.0.39/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1347 2023-05-28 13:26:16.000000 custom-utils-0.0.39/setup.py
```

### Comparing `custom-utils-0.0.38/LICENSE` & `custom-utils-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/PKG-INFO` & `custom-utils-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.38
+Version: 0.0.39
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
+Provides-Extra: slack
+Provides-Extra: mongodb
 Provides-Extra: s3
 Provides-Extra: mysql
 Provides-Extra: bigquery
-Provides-Extra: mongodb
-Provides-Extra: slack
 Provides-Extra: full
 License-File: LICENSE
 
 # custom-utils
 Pip Package for Database Connectors, Alerter, Log Formatter etc
 
 
@@ -51,15 +51,16 @@
 ***
 
 ## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
-    `pip install custom-utils[full]` --> full installation  
+    `pip install custom-utils[full]` --> full installation (linux/windows)  
+    `pip install "custom-utils[full]"` --> full installation (mac)  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
 	
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.38 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.39 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
-mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
+Description-Content-Type: text/markdown Provides-Extra: slack Provides-Extra:
+mongodb Provides-Extra: s3 Provides-Extra: mysql Provides-Extra: bigquery
 Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
 Database Connectors, Alerter, Log Formatter etc ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
 ## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
 (#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
 connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
 mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
 Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
 Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
 formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
 *** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
 install custom-utils` --> minimal installation `pip install custom-utils[full]`
---> full installation `pip install custom-utils
+--> full installation (linux/windows) `pip install "custom-utils[full]"` --
+> full installation (mac) `pip install custom-utils
 [s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
 from github repository** (Any one) `pip install git+https://github.com/
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
```

### Comparing `custom-utils-0.0.38/README.md` & `custom-utils-0.0.39/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 ***
 
 ## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
-    `pip install custom-utils[full]` --> full installation  
+    `pip install custom-utils[full]` --> full installation (linux/windows)  
+    `pip install "custom-utils[full]"` --> full installation (mac)  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
 	
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
 mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
 Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
 Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
 formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
 *** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
 install custom-utils` --> minimal installation `pip install custom-utils[full]`
---> full installation `pip install custom-utils
+--> full installation (linux/windows) `pip install "custom-utils[full]"` --
+> full installation (mac) `pip install custom-utils
 [s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
 from github repository** (Any one) `pip install git+https://github.com/
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
```

### Comparing `custom-utils-0.0.38/custom_utils/alerter/slack.py` & `custom-utils-0.0.39/custom_utils/alerter/slack.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/configurer/profiler.py` & `custom-utils-0.0.39/custom_utils/configurer/profiler.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/configurer/utils.py` & `custom-utils-0.0.39/custom_utils/configurer/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/connector/bigquery.py` & `custom-utils-0.0.39/custom_utils/connector/bigquery.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/connector/mongodb.py` & `custom-utils-0.0.39/custom_utils/connector/mongodb.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/connector/mysql.py` & `custom-utils-0.0.39/custom_utils/connector/mysql.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/connector/s3.py` & `custom-utils-0.0.39/custom_utils/connector/s3.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/exceptions.py` & `custom-utils-0.0.39/custom_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils/utils.py` & `custom-utils-0.0.39/custom_utils/utils.py`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/custom_utils.egg-info/PKG-INFO` & `custom-utils-0.0.39/custom_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.38
+Version: 0.0.39
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
+Provides-Extra: slack
+Provides-Extra: mongodb
 Provides-Extra: s3
 Provides-Extra: mysql
 Provides-Extra: bigquery
-Provides-Extra: mongodb
-Provides-Extra: slack
 Provides-Extra: full
 License-File: LICENSE
 
 # custom-utils
 Pip Package for Database Connectors, Alerter, Log Formatter etc
 
 
@@ -51,15 +51,16 @@
 ***
 
 ## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
-    `pip install custom-utils[full]` --> full installation  
+    `pip install custom-utils[full]` --> full installation (linux/windows)  
+    `pip install "custom-utils[full]"` --> full installation (mac)  
     `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
 	
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.38 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.39 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
 rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
-Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
-mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
+Description-Content-Type: text/markdown Provides-Extra: slack Provides-Extra:
+mongodb Provides-Extra: s3 Provides-Extra: mysql Provides-Extra: bigquery
 Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
 Database Connectors, Alerter, Log Formatter etc ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
 ## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
 (#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
 connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
 mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
 Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
 Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
 formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
 *** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
 install custom-utils` --> minimal installation `pip install custom-utils[full]`
---> full installation `pip install custom-utils
+--> full installation (linux/windows) `pip install "custom-utils[full]"` --
+> full installation (mac) `pip install custom-utils
 [s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
 from github repository** (Any one) `pip install git+https://github.com/
 rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
 custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
 utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
 Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
 from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
```

### Comparing `custom-utils-0.0.38/custom_utils.egg-info/SOURCES.txt` & `custom-utils-0.0.39/custom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom-utils-0.0.38/setup.py` & `custom-utils-0.0.39/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 from itertools import chain
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 EXTRAS_REQUIRE = {
-    's3' : [ 'boto', 'boto3', 'joblib'],
-    'mysql':  ['SQLAlchemy', 'SQLAlchemy-JSONField', 'SQLAlchemy-Utils', 'mysql-connector-python',],
-    'bigquery': ['tqdm==4.49.0','google-cloud-bigquery==2.1.0', 'pandas_gbq', 'google-cloud' ],
-    'mongodb': ['pymongo==3.10.0'],
-    'slack': ['slack-sdk==3.21.3'],
+    'slack'    : ['slack-sdk==3.21.3'],
+    'mongodb'  : ['pymongo==3.10.0'],
+    's3'       : [ 'boto', 'boto3', 'joblib'],
+    'mysql'    :  ['SQLAlchemy', 'mysql-connector-python',],
+    'bigquery' : ['tqdm==4.49.0','google-cloud-bigquery==2.1.0', 'pandas_gbq', 'google-cloud' ],
+
 }
 
 # construct special 'full' extra that adds requirements for all built-in
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     author="Rahul Kumar",
     author_email="rahulnkumar7@gmail.com",
     name='custom-utils',
     description='Utilities for database connectors, slack alerter, loggers etc',
-    version="0.0.38",
+    version="0.0.39",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RahulnKumar/custom-utils',
     packages=find_packages(),
     python_requires=">=3.6.9",
     install_requires=['python-dotenv', 'subprocess32',],
     extras_require=EXTRAS_REQUIRE,
```

