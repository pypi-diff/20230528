# Comparing `tmp/aio_fluid-0.5.1.tar.gz` & `tmp/aio_fluid-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_fluid-0.5.1.tar", max compression
+gzip compressed data, was "aio_fluid-0.5.2.tar", max compression
```

## Comparing `aio_fluid-0.5.1.tar` & `aio_fluid-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1517 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/LICENSE
--rw-r--r--   0        0        0       64 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/backdoor.py
--rw-r--r--   0        0        0      593 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/cors.py
--rw-r--r--   0        0        0     2165 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/datajson.py
--rw-r--r--   0        0        0     1493 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/db.py
--rw-r--r--   0        0        0      218 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/dev.py
--rw-r--r--   0        0        0      575 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/executor.py
--rw-r--r--   0        0        0     1225 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/fields.py
--rw-r--r--   0        0        0       75 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/github/__init__.py
--rw-r--r--   0        0        0      866 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/github/client.py
--rw-r--r--   0        0        0     4084 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/github/repo.py
--rw-r--r--   0        0        0    11637 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/http.py
--rw-r--r--   0        0        0      138 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/json.py
--rw-r--r--   0        0        0     2326 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/kernel.py
--rw-r--r--   0        0        0      296 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/kong.py
--rw-r--r--   0        0        0     2920 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/log.py
--rw-r--r--   0        0        0     9481 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/node.py
--rw-r--r--   0        0        0     3784 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/redis.py
--rw-r--r--   0        0        0      620 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/redis_status.py
--rw-r--r--   0        0        0      758 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/scheduler/__init__.py
--rw-r--r--   0        0        0     8413 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/scheduler/broker.py
--rw-r--r--   0        0        0      347 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/scheduler/constants.py
--rw-r--r--   0        0        0     9532 2023-04-01 19:05:06.630872 aio_fluid-0.5.1/fluid/scheduler/consumer.py
--rw-r--r--   0        0        0     2746 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/cpubound.py
--rw-r--r--   0        0        0     4209 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/crontab.py
--rw-r--r--   0        0        0     1280 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/every.py
--rw-r--r--   0        0        0     2306 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/readme.md
--rw-r--r--   0        0        0     1424 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/scheduler.py
--rw-r--r--   0        0        0     4546 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/task.py
--rw-r--r--   0        0        0     1547 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/task_run.py
--rw-r--r--   0        0        0      363 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/scheduler/utils.py
--rw-r--r--   0        0        0     2023 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/service.py
--rw-r--r--   0        0        0      429 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/settings.py
--rw-r--r--   0        0        0     6692 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/stacksampler.py
--rw-r--r--   0        0        0     1003 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/status.py
--rw-r--r--   0        0        0      399 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/sync_run.py
--rw-r--r--   0        0        0      526 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/text.py
--rw-r--r--   0        0        0      599 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/types.py
--rw-r--r--   0        0        0     2584 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/fluid/utils.py
--rw-r--r--   0        0        0     1875 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1215 2023-04-01 19:05:06.634872 aio_fluid-0.5.1/readme.md
--rw-r--r--   0        0        0     3234 1970-01-01 00:00:00.000000 aio_fluid-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/LICENSE
+-rw-r--r--   0        0        0       64 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/__init__.py
+-rw-r--r--   0        0        0     1633 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/backdoor.py
+-rw-r--r--   0        0        0      593 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/cors.py
+-rw-r--r--   0        0        0     2165 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/datajson.py
+-rw-r--r--   0        0        0     1493 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/db.py
+-rw-r--r--   0        0        0      218 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/dev.py
+-rw-r--r--   0        0        0      575 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/executor.py
+-rw-r--r--   0        0        0     1225 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/fields.py
+-rw-r--r--   0        0        0       75 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/client.py
+-rw-r--r--   0        0        0     4084 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/repo.py
+-rw-r--r--   0        0        0    11637 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/http.py
+-rw-r--r--   0        0        0      138 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/json.py
+-rw-r--r--   0        0        0     2326 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/kernel.py
+-rw-r--r--   0        0        0      296 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/kong.py
+-rw-r--r--   0        0        0     2920 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/log.py
+-rw-r--r--   0        0        0     9481 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/node.py
+-rw-r--r--   0        0        0     3784 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/redis.py
+-rw-r--r--   0        0        0      620 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/redis_status.py
+-rw-r--r--   0        0        0      758 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/__init__.py
+-rw-r--r--   0        0        0     8413 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/broker.py
+-rw-r--r--   0        0        0      347 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/constants.py
+-rw-r--r--   0        0        0     9532 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/consumer.py
+-rw-r--r--   0        0        0     2746 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/cpubound.py
+-rw-r--r--   0        0        0     4209 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/crontab.py
+-rw-r--r--   0        0        0     1280 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/every.py
+-rw-r--r--   0        0        0     2306 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/readme.md
+-rw-r--r--   0        0        0     1424 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/scheduler.py
+-rw-r--r--   0        0        0     4546 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/task.py
+-rw-r--r--   0        0        0     1547 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/task_run.py
+-rw-r--r--   0        0        0      363 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/utils.py
+-rw-r--r--   0        0        0     2023 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/service.py
+-rw-r--r--   0        0        0      429 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/settings.py
+-rw-r--r--   0        0        0     6692 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/stacksampler.py
+-rw-r--r--   0        0        0     1003 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/status.py
+-rw-r--r--   0        0        0      399 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/sync_run.py
+-rw-r--r--   0        0        0      526 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/text.py
+-rw-r--r--   0        0        0      599 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/types.py
+-rw-r--r--   0        0        0     2584 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/utils.py
+-rw-r--r--   0        0        0     1875 2023-05-28 18:10:59.720717 aio_fluid-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-05-28 18:10:59.720717 aio_fluid-0.5.2/readme.md
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 aio_fluid-0.5.2/PKG-INFO
```

### Comparing `aio_fluid-0.5.1/LICENSE` & `aio_fluid-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/backdoor.py` & `aio_fluid-0.5.2/fluid/backdoor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/cors.py` & `aio_fluid-0.5.2/fluid/cors.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/datajson.py` & `aio_fluid-0.5.2/fluid/datajson.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/db.py` & `aio_fluid-0.5.2/fluid/db.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/executor.py` & `aio_fluid-0.5.2/fluid/executor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/fields.py` & `aio_fluid-0.5.2/fluid/fields.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/github/client.py` & `aio_fluid-0.5.2/fluid/github/client.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/github/repo.py` & `aio_fluid-0.5.2/fluid/github/repo.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/http.py` & `aio_fluid-0.5.2/fluid/http.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/kernel.py` & `aio_fluid-0.5.2/fluid/kernel.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/log.py` & `aio_fluid-0.5.2/fluid/log.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/node.py` & `aio_fluid-0.5.2/fluid/node.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/redis.py` & `aio_fluid-0.5.2/fluid/redis.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/redis_status.py` & `aio_fluid-0.5.2/fluid/redis_status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/__init__.py` & `aio_fluid-0.5.2/fluid/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/broker.py` & `aio_fluid-0.5.2/fluid/scheduler/broker.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/consumer.py` & `aio_fluid-0.5.2/fluid/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/cpubound.py` & `aio_fluid-0.5.2/fluid/scheduler/cpubound.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/crontab.py` & `aio_fluid-0.5.2/fluid/scheduler/crontab.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/every.py` & `aio_fluid-0.5.2/fluid/scheduler/every.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/readme.md` & `aio_fluid-0.5.2/fluid/scheduler/readme.md`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/scheduler.py` & `aio_fluid-0.5.2/fluid/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/task.py` & `aio_fluid-0.5.2/fluid/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/scheduler/task_run.py` & `aio_fluid-0.5.2/fluid/scheduler/task_run.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/service.py` & `aio_fluid-0.5.2/fluid/service.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/stacksampler.py` & `aio_fluid-0.5.2/fluid/stacksampler.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/status.py` & `aio_fluid-0.5.2/fluid/status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/text.py` & `aio_fluid-0.5.2/fluid/text.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/types.py` & `aio_fluid-0.5.2/fluid/types.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/fluid/utils.py` & `aio_fluid-0.5.2/fluid/utils.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.1/pyproject.toml` & `aio_fluid-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-fluid"
-version = "0.5.1"
+version = "0.5.2"
 description = "Tools for backend python services"
 license = "BSD"
 authors = ["Luca <luca@quantmind.com>"]
 readme = "readme.md"
 packages = [
     {include = "fluid"}
 ]
@@ -40,15 +40,15 @@
 aioconsole = "^0.6.1"
 python-slugify = {version = "^8.0.1", extras = ["unidecode"]}
 python-json-logger = "^2.0.2"
 colorlog = "^6.6.0"
 aiohttp_cors = "^0.7.0"
 aiobotocore = {version = "~2.4.2", extras=["boto3"]}
 s3fs = {version = "^2023.3.0"}
-aio-kong = "^3.0.0"
+aio-kong = "^3.3.0"
 uvloop = "^0.17.0"
 pycountry = "^22.3.5"
 redis = "^4.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 isort = "^5.9.3"
```

### Comparing `aio_fluid-0.5.1/readme.md` & `aio_fluid-0.5.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tools for backend python services
 
 [![PyPI version](https://badge.fury.io/py/aio-fluid.svg)](https://badge.fury.io/py/aio-fluid)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-fluid.svg)](https://pypi.org/project/aio-fluid)
 [![build](https://github.com/quantmind/fluid/workflows/build/badge.svg)](https://github.com/quantmind/aio-fluid/actions?query=workflow%3Abuild)
-[![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/master/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
+[![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/main/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
 
 ## Installation
 
 This is a simple python package you can install via pip:
 
 ```
 pip install aio-fluid
```

### Comparing `aio_fluid-0.5.1/PKG-INFO` & `aio_fluid-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-fluid
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools for backend python services
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -14,23 +14,20 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: aio-kong (>=3.0.0,<4.0.0)
+Requires-Dist: aio-kong (>=3.3.0,<4.0.0)
 Requires-Dist: aio-openapi (>=3.2.0,<4.0.0)
 Requires-Dist: aiobotocore[boto3] (>=2.4.2,<2.5.0)
 Requires-Dist: aioconsole (>=0.6.1,<0.7.0)
 Requires-Dist: aiohttp_cors (>=0.7.0,<0.8.0)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: prometheus-async (>=22.1.0,<23.0.0)
@@ -46,15 +43,15 @@
 Description-Content-Type: text/markdown
 
 # Tools for backend python services
 
 [![PyPI version](https://badge.fury.io/py/aio-fluid.svg)](https://badge.fury.io/py/aio-fluid)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-fluid.svg)](https://pypi.org/project/aio-fluid)
 [![build](https://github.com/quantmind/fluid/workflows/build/badge.svg)](https://github.com/quantmind/aio-fluid/actions?query=workflow%3Abuild)
-[![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/master/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
+[![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/main/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
 
 ## Installation
 
 This is a simple python package you can install via pip:
 
 ```
 pip install aio-fluid
```

