# Comparing `tmp/python-sonarqube-api-2.0.1.tar.gz` & `tmp/python-sonarqube-api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sonarqube-api-2.0.1.tar", last modified: Fri May 26 14:53:49 2023, max compression
+gzip compressed data, was "python-sonarqube-api-2.0.2.tar", last modified: Sun May 28 13:14:42 2023, max compression
```

## Comparing `python-sonarqube-api-2.0.1.tar` & `python-sonarqube-api-2.0.2.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:49.003585 python-sonarqube-api-2.0.1/
--rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     6065 2023-05-26 14:53:49.003365 python-sonarqube-api-2.0.1/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     4946 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.981671 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6065 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     1200 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-26 14:53:48.000000 python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-26 14:53:49.003692 python-sonarqube-api-2.0.1/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.982179 python-sonarqube-api-2.0.1/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:48.999445 python-sonarqube-api-2.0.1/sonarqube/rest/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6785 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3668 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      890 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/monitoring.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5352 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8700 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1528 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3264 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/rest/views.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-26 14:53:49.003049 python-sonarqube-api-2.0.1/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3356 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.1/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.616214 python-sonarqube-api-2.0.2/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/LICENSE
+-rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/MANIFEST.in
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5856 2023-05-28 13:14:42.615965 python-sonarqube-api-2.0.2/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4737 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/README.rst
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.598734 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5856 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1144 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/requirements.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-28 13:14:42.616272 python-sonarqube-api-2.0.2/setup.cfg
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/setup.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.599020 python-sonarqube-api-2.0.2/sonarqube/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/__init__.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.612925 python-sonarqube-api-2.0.2/sonarqube/rest/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6232 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/audit_logs.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2110 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/duplications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/editions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/favorites.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/languages.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/measures.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/metrics.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_analyses.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_branches.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_dump.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_tags.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2389 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8231 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/server.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2928 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/user_tokens.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/views.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.614893 python-sonarqube-api-2.0.2/sonarqube/utils/
+-rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/common.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2370 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/utils/config.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/exceptions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/rest_client.py
```

### Comparing `python-sonarqube-api-2.0.1/LICENSE` & `python-sonarqube-api-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/PKG-INFO` & `python-sonarqube-api-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPL
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,25 +51,25 @@
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
  * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-   that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
+   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 60                  | more than 280         |
+| Functions           | 40                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -78,20 +78,14 @@
 Community Edition
 -----------------
 
 The easiest way to install the latest version is by using pip to pull it from PyPI::
 
     pip install  --upgrade python-sonarqube-api
 
-You may also use Git to clone the repository from Github and install it manually::
-
-    git clone https://github.com/shijl0925/python-sonarqube-api.git
-    cd python-sonarqube-api
-    python setup.py install
-
 
 Professional Edition
 --------------------
 Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
 
     pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
```

### Comparing `python-sonarqube-api-2.0.1/README.rst` & `python-sonarqube-api-2.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
  * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-   that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
+   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 60                  | more than 280         |
+| Functions           | 40                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -51,20 +51,14 @@
 Community Edition
 -----------------
 
 The easiest way to install the latest version is by using pip to pull it from PyPI::
 
     pip install  --upgrade python-sonarqube-api
 
-You may also use Git to clone the repository from Github and install it manually::
-
-    git clone https://github.com/shijl0925/python-sonarqube-api.git
-    cd python-sonarqube-api
-    python setup.py install
-
 
 Professional Edition
 --------------------
 Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
 
     pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
```

### Comparing `python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/PKG-INFO` & `python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPL
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,25 +51,25 @@
 Editions
 ========
 
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
  * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-   that are more useful for developers with more than 130 interface functions. To use PE and get timely Email support and continuous updates,
+   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 60                  | more than 280         |
+| Functions           | 40                  | more than 280         |
 | (REST APIs)         |                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 Installation
@@ -78,20 +78,14 @@
 Community Edition
 -----------------
 
 The easiest way to install the latest version is by using pip to pull it from PyPI::
 
     pip install  --upgrade python-sonarqube-api
 
-You may also use Git to clone the repository from Github and install it manually::
-
-    git clone https://github.com/shijl0925/python-sonarqube-api.git
-    cd python-sonarqube-api
-    python setup.py install
-
 
 Professional Edition
 --------------------
 Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
 
     pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
```

### Comparing `python-sonarqube-api-2.0.1/python_sonarqube_api.egg-info/SOURCES.txt` & `python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,24 @@
 sonarqube/rest/duplications.py
 sonarqube/rest/editions.py
 sonarqube/rest/favorites.py
 sonarqube/rest/issues.py
 sonarqube/rest/languages.py
 sonarqube/rest/measures.py
 sonarqube/rest/metrics.py
-sonarqube/rest/monitoring.py
 sonarqube/rest/project_analyses.py
 sonarqube/rest/project_badges.py
 sonarqube/rest/project_branches.py
 sonarqube/rest/project_dump.py
 sonarqube/rest/project_tags.py
 sonarqube/rest/projects.py
 sonarqube/rest/qualitygates.py
 sonarqube/rest/qualityprofiles.py
 sonarqube/rest/rules.py
 sonarqube/rest/server.py
-sonarqube/rest/settings.py
 sonarqube/rest/user_groups.py
 sonarqube/rest/user_tokens.py
 sonarqube/rest/users.py
 sonarqube/rest/views.py
 sonarqube/utils/__init__.py
 sonarqube/utils/common.py
 sonarqube/utils/config.py
```

### Comparing `python-sonarqube-api-2.0.1/setup.py` & `python-sonarqube-api-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/__init__.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,23 @@
 from sonarqube.rest.ce import SonarQubeCe
 from sonarqube.rest.project_branches import SonarQubeProjectBranches
 from sonarqube.rest.qualitygates import SonarQubeQualityGates
 from sonarqube.rest.rules import SonarQubeRules
 from sonarqube.rest.qualityprofiles import SonarQubeQualityProfiles
 from sonarqube.rest.duplications import SonarQubeDuplications
 from sonarqube.rest.metrics import SonarQubeMetrics
-from sonarqube.rest.settings import SonarQubeSettings
 from sonarqube.rest.auth import SonarQubeAuth
 from sonarqube.rest.favorites import SonarQubeFavorites
 from sonarqube.rest.languages import SonarQubeLanguages
 from sonarqube.rest.project_badges import SonarQubeProjectBadges
 from sonarqube.rest.project_tags import SonarQubeProjectTags
 from sonarqube.rest.project_analyses import SonarQubeProjectAnalyses
 from sonarqube.rest.server import SonarQubeServer
 from sonarqube.rest.user_tokens import SonarQubeUserTokens
-from sonarqube.rest.monitoring import SonarQubeMonitoring
 from sonarqube.rest.project_dump import SonarQubeProjectDump
-from sonarqube.rest.audit_logs import SonarQubeAuditLogs
 from sonarqube.rest.editions import SonarQubeEditions
 from sonarqube.rest.views import SonarQubeViews
 
 
 class SonarQubeClient:
     """
     A Python Client for SonarQube Server APIs.
@@ -177,23 +174,14 @@
         SonarQube metrics Operations
 
         :return:
         """
         return SonarQubeMetrics(api=self)
 
     @property
-    def settings(self):
-        """
-        SonarQube settings Operations
-
-        :return:
-        """
-        return SonarQubeSettings(api=self)
-
-    @property
     def auth(self):
         """
         SonarQube authentication Operations
 
         :return:
         """
         return SonarQubeAuth(api=self)
@@ -258,35 +246,23 @@
         SonarQube user tokens Operations
 
         :return:
         """
         return SonarQubeUserTokens(api=self)
 
     @property
-    def monitoring(self):
-        return SonarQubeMonitoring(api=self)
-
-    @property
     def project_dump(self):
         """
         Project export/import
 
         :return:
         """
         return SonarQubeProjectDump(api=self)
 
     @property
-    def audit_logs(self):
-        """
-        Manage Audit logs
-
-        """
-        return SonarQubeAuditLogs(api=self)
-
-    @property
     def editions(self):
         """
         Manage SonarSource commercial editions
 
         """
         return SonarQubeEditions(api=self)
```

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/audit_logs.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/audit_logs.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/auth.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/duplications.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/editions.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/editions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/favorites.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/favorites.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/issues.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/issues.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/languages.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/languages.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/measures.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/measures.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/metrics.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/project_analyses.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/project_analyses.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/project_badges.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/project_badges.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/project_branches.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/project_branches.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/project_dump.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/project_dump.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/project_tags.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/project_tags.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/projects.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/projects.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/qualityprofiles.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/qualityprofiles.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/rules.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_RULES_SEARCH_ENDPOINT,
     API_RULES_CREATE_ENDPOINT,
-    API_RULES_SHOW_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeRules(RestClient):
     """
     SonarQube rules Operations
@@ -259,21 +258,8 @@
             * CODE_SMELL
             * BUG
             * VULNERABILITY
             * SECURITY_HOTSPOT
         :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2' (Only for custom rule)
 
         :return: request response
-        """
-
-    @GET(API_RULES_SHOW_ENDPOINT)
-    def get_rule(self, key, organization=None, actives="false"):
-        """
-        SINCE 4.2
-        Get detailed information about a rule.
-
-        :param key: Rule key
-        :param organization: organization key.
-        :param actives: Show rule's activations for all profiles ("active rules").
-          Possible values are for: true or false. default value is false.
-        :return:
         """
```

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/server.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/user_groups.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/user_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from sonarqube.utils.rest_client import RestClient
 from sonarqube.utils.config import (
     API_USER_GROUPS_SEARCH_ENDPOINT,
     API_USER_GROUPS_CREATE_ENDPOINT,
-    API_USER_GROUPS_DELETE_ENDPOINT,
     API_USER_GROUPS_UPDATE_ENDPOINT,
 )
 from sonarqube.utils.common import GET, POST
 
 
 class SonarQubeUserGroups(RestClient):
     """
@@ -59,26 +58,14 @@
 
         :param name: Name for the new group. A group name cannot be larger than 255 characters and must be unique.
           The value 'anyone' (whatever the case) is reserved and cannot be used.
         :param organization: organization key.
         :param description: Description for the new group. A group description cannot be larger than 200 characters.
         :return: request response
         """
-
-    @POST(API_USER_GROUPS_DELETE_ENDPOINT)
-    def delete_group(self, name, organization=None):
-        """
-        SINCE 5.2
-        Delete a group. The default groups cannot be deleted.
-
-        :param name: group name
-        :param organization: organization key.
-        :return:
-        """
-
     @POST(API_USER_GROUPS_UPDATE_ENDPOINT)
     def update_group(self, currentName, name=None, description=None):
         """
         SINCE 5.2
         Update a group.
 
         :param currentName: Name of the group to be updated. (since 8.5)
```

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/user_tokens.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/user_tokens.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/users.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/users.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/rest/views.py` & `python-sonarqube-api-2.0.2/sonarqube/rest/views.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/utils/common.py` & `python-sonarqube-api-2.0.2/sonarqube/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.1/sonarqube/utils/config.py` & `python-sonarqube-api-2.0.2/sonarqube/utils/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,38 @@
 API_COMPONENTS_SHOW_ENDPOINT = "/api/components/show"
 
 API_PROJECTS_SEARCH_ENDPOINT = "/api/projects/search"
-API_AUDIT_LOGS_DOWNLOAD_ENDPOINT = "/api/audit_logs/download"
-
-API_MONITORING_METRICS_ENDPOINT = "/api/monitoring/metrics"
 
 API_USERS_SEARCH_ENDPOINT = "/api/users/search"
 API_USER_GROUPS_SEARCH_ENDPOINT = "/api/user_groups/search"
 API_USER_GROUPS_CREATE_ENDPOINT = "/api/user_groups/create"
 API_USER_GROUPS_DELETE_ENDPOINT = "/api/user_groups/delete"
 API_USER_GROUPS_UPDATE_ENDPOINT = "/api/user_groups/update"
 API_CE_ACTIVITY_ENDPOINT = "/api/ce/activity"
-API_CE_ACTIVITY_STATUS_ENDPOINT = "/api/ce/activity_status"
-API_CE_ANALYSIS_STATUS_ENDPOINT = "/api/ce/analysis_status"
-API_CE_COMPONENT_ENDPOINT = "/api/ce/component"
-API_CE_TASK_ENDPOINT = "/api/ce/task"
 
 API_MEASURES_COMPONENT_ENDPOINT = "/api/measures/component"
 
 API_PROJECT_BRANCHES_LIST_ENDPOINT = "/api/project_branches/list"
 API_ISSUES_SEARCH_ENDPOINT = "/api/issues/search"
 API_ISSUES_ASSIGN_ENDPOINT = "/api/issues/assign"
 API_QUALITYGATES_LIST_ENDPOINT = "/api/qualitygates/list"
 API_QUALITYGATES_SELECT_ENDPOINT = "/api/qualitygates/select"
-API_QUALITYGATES_DESELECT_ENDPOINT = "/api/qualitygates/deselect"
-API_QUALITYGATES_SHOW_ENDPOINT = "/api/qualitygates/show"
-API_QUALITYGATES_CREATE_ENDPOINT = "/api/qualitygates/create"
-API_QUALITYGATES_DESTROY_ENDPOINT = "/api/qualitygates/destroy"
-API_QUALITYGATES_RENAME_ENDPOINT = "/api/qualitygates/rename"
 API_QUALITYGATES_SEARCH_ENDPOINT = "/api/qualitygates/search"
-API_QUALITYGATES_SET_AS_DEFAULT_ENDPOINT = "/api/qualitygates/set_as_default"
-API_QUALITYGATES_ADD_GROUP_ENDPOINT = "/api/qualitygates/add_group"
-
 API_RULES_SEARCH_ENDPOINT = "/api/rules/search"
 API_RULES_CREATE_ENDPOINT = "/api/rules/create"
-API_RULES_SHOW_ENDPOINT = "/api/rules/show"
 
 API_QUALITYPROFILES_ACTIVATE_RULE_ENDPOINT = "/api/qualityprofiles/activate_rule"
 API_QUALITYPROFILES_SEARCH_ENDPOINT = "/api/qualityprofiles/search"
 API_QUALITYPROFILES_DELETE_ENDPOINT = "/api/qualityprofiles/delete"
 API_QUALITYPROFILES_CREATE_ENDPOINT = "/api/qualityprofiles/create"
 API_DUPLICATIONS_SHOW_ENDPOINT = "/api/duplications/show"
 
-API_PDFREPORT_GET_ENDPOINT = "/api/pdfreport/get"
-
 API_METRICS_SEARCH_ENDPOINT = "/api/metrics/search"
 API_METRICS_TYPES_ENDPOINT = "/api/metrics/types"
 
-API_SETTINGS_SET_ENDPOINT = "/api/settings/set"
-API_SETTINGS_VALUES_ENDPOINT = "/api/settings/values"
-
 API_AUTH_VALIDATE_ENDPOINT = "/api/authentication/validate"
 
 API_FAVORITES_SEARCH_ENDPOINT = "/api/favorites/search"
 
 API_LANGUAGES_LIST_ENDPOINT = "/api/languages/list"
 
 API_PROJECT_BADGES_MEASURE_ENDPOINT = "/api/project_badges/measure"
```

### Comparing `python-sonarqube-api-2.0.1/sonarqube/utils/rest_client.py` & `python-sonarqube-api-2.0.2/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

