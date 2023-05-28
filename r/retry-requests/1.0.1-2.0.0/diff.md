# Comparing `tmp/retry-requests-1.0.1.tar.gz` & `tmp/retry-requests-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/retry-requests-1.0.1.tar", last modified: Thu Jun 18 18:00:13 2020, max compression
+gzip compressed data, was "retry-requests-2.0.0.tar", last modified: Sun May 28 18:27:43 2023, max compression
```

## Comparing `retry-requests-1.0.1.tar` & `retry-requests-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2020-06-18 18:00:13.891492 retry-requests-1.0.1/
--rw-r--r--   0 bustawin   (501) staff       (20)     2952 2020-06-18 18:00:13.891685 retry-requests-1.0.1/PKG-INFO
--rw-r--r--   0 bustawin   (501) staff       (20)     1490 2019-12-28 09:55:25.000000 retry-requests-1.0.1/README.rst
-drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2020-06-18 18:00:13.890119 retry-requests-1.0.1/retry_requests/
--rw-r--r--   0 bustawin   (501) staff       (20)     2838 2019-12-28 09:49:00.000000 retry-requests-1.0.1/retry_requests/__init__.py
-drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2020-06-18 18:00:13.891287 retry-requests-1.0.1/retry_requests.egg-info/
--rw-r--r--   0 bustawin   (501) staff       (20)     2952 2020-06-18 18:00:13.000000 retry-requests-1.0.1/retry_requests.egg-info/PKG-INFO
--rw-r--r--   0 bustawin   (501) staff       (20)      245 2020-06-18 18:00:13.000000 retry-requests-1.0.1/retry_requests.egg-info/SOURCES.txt
--rw-r--r--   0 bustawin   (501) staff       (20)        1 2020-06-18 18:00:13.000000 retry-requests-1.0.1/retry_requests.egg-info/dependency_links.txt
--rw-r--r--   0 bustawin   (501) staff       (20)       24 2020-06-18 18:00:13.000000 retry-requests-1.0.1/retry_requests.egg-info/requires.txt
--rw-r--r--   0 bustawin   (501) staff       (20)       15 2020-06-18 18:00:13.000000 retry-requests-1.0.1/retry_requests.egg-info/top_level.txt
--rw-r--r--   0 bustawin   (501) staff       (20)      104 2020-06-18 18:00:13.892229 retry-requests-1.0.1/setup.cfg
--rw-r--r--   0 bustawin   (501) staff       (20)     1414 2020-06-18 17:59:52.000000 retry-requests-1.0.1/setup.py
+drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2023-05-28 18:27:43.597964 retry-requests-2.0.0/
+-rw-r--r--   0 bustawin   (501) staff       (20)    35149 2023-05-28 17:00:45.000000 retry-requests-2.0.0/LICENSE
+-rw-r--r--   0 bustawin   (501) staff       (20)     2535 2023-05-28 18:27:43.598008 retry-requests-2.0.0/PKG-INFO
+-rw-r--r--   0 bustawin   (501) staff       (20)     1490 2023-05-28 17:00:45.000000 retry-requests-2.0.0/README.rst
+drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2023-05-28 18:27:43.597297 retry-requests-2.0.0/retry_requests/
+-rw-r--r--   0 bustawin   (501) staff       (20)     2836 2023-05-28 18:25:53.000000 retry-requests-2.0.0/retry_requests/__init__.py
+drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2023-05-28 18:27:43.597774 retry-requests-2.0.0/retry_requests.egg-info/
+-rw-r--r--   0 bustawin   (501) staff       (20)     2535 2023-05-28 18:27:43.000000 retry-requests-2.0.0/retry_requests.egg-info/PKG-INFO
+-rw-r--r--   0 bustawin   (501) staff       (20)      275 2023-05-28 18:27:43.000000 retry-requests-2.0.0/retry_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 bustawin   (501) staff       (20)        1 2023-05-28 18:27:43.000000 retry-requests-2.0.0/retry_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 bustawin   (501) staff       (20)       38 2023-05-28 18:27:43.000000 retry-requests-2.0.0/retry_requests.egg-info/requires.txt
+-rw-r--r--   0 bustawin   (501) staff       (20)       15 2023-05-28 18:27:43.000000 retry-requests-2.0.0/retry_requests.egg-info/top_level.txt
+-rw-r--r--   0 bustawin   (501) staff       (20)      104 2023-05-28 18:27:43.598153 retry-requests-2.0.0/setup.cfg
+-rw-r--r--   0 bustawin   (501) staff       (20)     1431 2023-05-28 18:25:53.000000 retry-requests-2.0.0/setup.py
+drwxr-xr-x   0 bustawin   (501) staff       (20)        0 2023-05-28 18:27:43.597865 retry-requests-2.0.0/tests/
+-rw-r--r--   0 bustawin   (501) staff       (20)     1531 2023-05-28 18:25:53.000000 retry-requests-2.0.0/tests/test_testing.py
```

### Comparing `retry-requests-1.0.1/PKG-INFO` & `retry-requests-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: retry-requests
-Version: 1.0.1
+Version: 2.0.0
 Summary: Make requests's sessions auto-retry on failure.
 Home-page: https://github.com/bustawin/retry-requests
 Author: Xavier Bustamante Talavera
 Author-email: xavier@bustawin.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/bustawin/retry-requests
 Project-URL: Code, https://github.com/bustawin/retry-requests
 Project-URL: Issue tracker, https://github.com/bustawin/retry-requests/issues
-Description: Retry-requests
-        ##############
-        Configures the passed-in `requests' <http://python-requests.org>`_ ``Session``
-        to retry on failed requests due to connection errors, timeouts,
-        specific HTTP response codes (5XX by default) and 30X redirections
-        —anything that could fail.
-        
-        Python 3.6+.
-        
-        Basic usage:
-        
-        .. code-block:: python
-        
-          from retry_requests import retry
-          my_session = retry()
-          my_session.get("http://foo.bar")
-        
-        This ``get`` will retry three times in case of error waiting some time between retries.
-        Errors could be:
-        
-        - Waiting for the server to start answering for 5 seconds.
-        - No access to the server or a dropped connection.
-        - An HTTP answer of 500, 502, or 504.
-        
-        You can change these defaults:
-        
-        .. code-block:: python
-        
-          from retry_requests import retry
-          from requests import Session
-          my_session = retry(Session(), retries=5, backoff_factor=0.2)
-          my_session.get('https://foo.bar')
-        
-        Check the function ``retry`` to know more about this configuration.
-        
-        Note that you have a ``TSession``, a ``Session`` with a default timeout,
-        and ``RSession``, a ``Session`` with a timeout that always ``raise_for_status()``,
-        for your convenience.
-        
-        
-        Heavily inspired from `Peterbe.com <https://www.peterbe.com/plog/
-        best-practice-with-retries-with-requests>`_. Thank you!
-        
-        Installing
-        **********
-        Just ``pip install retry-requests``.
-        
-        Testing
-        *******
-        Clone this project and then, at its root directory, run ``python setup.py test``.
-        Note that you need an active Internet connection to run the tests.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: test
+License-File: LICENSE
+
+Retry-requests
+##############
+Configures the passed-in `requests' <http://python-requests.org>`_ ``Session``
+to retry on failed requests due to connection errors, timeouts,
+specific HTTP response codes (5XX by default) and 30X redirections
+—anything that could fail.
+
+Python 3.6+.
+
+Basic usage:
+
+.. code-block:: python
+
+  from retry_requests import retry
+  my_session = retry()
+  my_session.get("http://foo.bar")
+
+This ``get`` will retry three times in case of error waiting some time between retries.
+Errors could be:
+
+- Waiting for the server to start answering for 5 seconds.
+- No access to the server or a dropped connection.
+- An HTTP answer of 500, 502, or 504.
+
+You can change these defaults:
+
+.. code-block:: python
+
+  from retry_requests import retry
+  from requests import Session
+  my_session = retry(Session(), retries=5, backoff_factor=0.2)
+  my_session.get('https://foo.bar')
+
+Check the function ``retry`` to know more about this configuration.
+
+Note that you have a ``TSession``, a ``Session`` with a default timeout,
+and ``RSession``, a ``Session`` with a timeout that always ``raise_for_status()``,
+for your convenience.
+
+
+Heavily inspired from `Peterbe.com <https://www.peterbe.com/plog/
+best-practice-with-retries-with-requests>`_. Thank you!
+
+Installing
+**********
+Just ``pip install retry-requests``.
+
+Testing
+*******
+Clone this project and then, at its root directory, run ``python setup.py test``.
+Note that you need an active Internet connection to run the tests.
```

### Comparing `retry-requests-1.0.1/README.rst` & `retry-requests-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `retry-requests-1.0.1/retry_requests/__init__.py` & `retry-requests-2.0.0/retry_requests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     Returns:
         A session object with the retry setup.
     """
     session = session or TSession()
 
     # Retry too in non-idempotent methods like POST
-    kwargs.setdefault("method_whitelist", False)
+    kwargs.setdefault("allowed_methods", None)
 
     r = Retry(
         total=retries,
         read=retries,
         connect=retries,
         backoff_factor=backoff_factor,
         status_forcelist=status_to_retry,
```

### Comparing `retry-requests-1.0.1/retry_requests.egg-info/PKG-INFO` & `retry-requests-2.0.0/retry_requests.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: retry-requests
-Version: 1.0.1
+Version: 2.0.0
 Summary: Make requests's sessions auto-retry on failure.
 Home-page: https://github.com/bustawin/retry-requests
 Author: Xavier Bustamante Talavera
 Author-email: xavier@bustawin.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/bustawin/retry-requests
 Project-URL: Code, https://github.com/bustawin/retry-requests
 Project-URL: Issue tracker, https://github.com/bustawin/retry-requests/issues
-Description: Retry-requests
-        ##############
-        Configures the passed-in `requests' <http://python-requests.org>`_ ``Session``
-        to retry on failed requests due to connection errors, timeouts,
-        specific HTTP response codes (5XX by default) and 30X redirections
-        —anything that could fail.
-        
-        Python 3.6+.
-        
-        Basic usage:
-        
-        .. code-block:: python
-        
-          from retry_requests import retry
-          my_session = retry()
-          my_session.get("http://foo.bar")
-        
-        This ``get`` will retry three times in case of error waiting some time between retries.
-        Errors could be:
-        
-        - Waiting for the server to start answering for 5 seconds.
-        - No access to the server or a dropped connection.
-        - An HTTP answer of 500, 502, or 504.
-        
-        You can change these defaults:
-        
-        .. code-block:: python
-        
-          from retry_requests import retry
-          from requests import Session
-          my_session = retry(Session(), retries=5, backoff_factor=0.2)
-          my_session.get('https://foo.bar')
-        
-        Check the function ``retry`` to know more about this configuration.
-        
-        Note that you have a ``TSession``, a ``Session`` with a default timeout,
-        and ``RSession``, a ``Session`` with a timeout that always ``raise_for_status()``,
-        for your convenience.
-        
-        
-        Heavily inspired from `Peterbe.com <https://www.peterbe.com/plog/
-        best-practice-with-retries-with-requests>`_. Thank you!
-        
-        Installing
-        **********
-        Just ``pip install retry-requests``.
-        
-        Testing
-        *******
-        Clone this project and then, at its root directory, run ``python setup.py test``.
-        Note that you need an active Internet connection to run the tests.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: test
+License-File: LICENSE
+
+Retry-requests
+##############
+Configures the passed-in `requests' <http://python-requests.org>`_ ``Session``
+to retry on failed requests due to connection errors, timeouts,
+specific HTTP response codes (5XX by default) and 30X redirections
+—anything that could fail.
+
+Python 3.6+.
+
+Basic usage:
+
+.. code-block:: python
+
+  from retry_requests import retry
+  my_session = retry()
+  my_session.get("http://foo.bar")
+
+This ``get`` will retry three times in case of error waiting some time between retries.
+Errors could be:
+
+- Waiting for the server to start answering for 5 seconds.
+- No access to the server or a dropped connection.
+- An HTTP answer of 500, 502, or 504.
+
+You can change these defaults:
+
+.. code-block:: python
+
+  from retry_requests import retry
+  from requests import Session
+  my_session = retry(Session(), retries=5, backoff_factor=0.2)
+  my_session.get('https://foo.bar')
+
+Check the function ``retry`` to know more about this configuration.
+
+Note that you have a ``TSession``, a ``Session`` with a default timeout,
+and ``RSession``, a ``Session`` with a timeout that always ``raise_for_status()``,
+for your convenience.
+
+
+Heavily inspired from `Peterbe.com <https://www.peterbe.com/plog/
+best-practice-with-retries-with-requests>`_. Thank you!
+
+Installing
+**********
+Just ``pip install retry-requests``.
+
+Testing
+*******
+Clone this project and then, at its root directory, run ``python setup.py test``.
+Note that you need an active Internet connection to run the tests.
```

### Comparing `retry-requests-1.0.1/setup.py` & `retry-requests-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from setuptools import find_packages, setup
 
 test_requires = ["pytest"]
 
 setup(
     name="retry-requests",
-    version="1.0.1",
+    version="2.0.0",
     url="https://github.com/bustawin/retry-requests",
     project_urls={
         "Documentation": "https://github.com/bustawin/retry-requests",
         "Code": "https://github.com/bustawin/retry-requests",
         "Issue tracker": "https://github.com/bustawin/retry-requests/issues",
     },
     license="GPLv3+",
     author="Xavier Bustamante Talavera",
     author_email="xavier@bustawin.com",
     description="Make requests's sessions auto-retry on failure.",
     packages=find_packages(),
     python_requires=">=3.6",
     long_description=Path("README.rst").read_text("utf8"),
-    install_requires=["requests"],
+    install_requires=["requests", "urllib3>=1.26"],
     extras_require={"test": test_requires},
     tests_require=test_requires,
     setup_requires=["pytest-runner"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

