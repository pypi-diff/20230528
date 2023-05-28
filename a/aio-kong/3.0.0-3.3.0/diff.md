# Comparing `tmp/aio_kong-3.0.0.tar.gz` & `tmp/aio_kong-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_kong-3.0.0.tar", max compression
+gzip compressed data, was "aio_kong-3.3.0.tar", max compression
```

## Comparing `aio_kong-3.0.0.tar` & `aio_kong-3.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1461 2022-12-18 11:49:30.226388 aio_kong-3.0.0/LICENSE
--rw-r--r--   0        0        0       54 2022-12-18 11:49:30.226388 aio_kong-3.0.0/kong/__init__.py
--rw-r--r--   0        0        0     2315 2022-12-18 11:49:30.226388 aio_kong-3.0.0/kong/auths.py
--rw-r--r--   0        0        0      278 2022-12-18 11:49:30.226388 aio_kong-3.0.0/kong/certificates.py
--rw-r--r--   0        0        0     1986 2022-12-18 11:49:30.226388 aio_kong-3.0.0/kong/cli.py
--rw-r--r--   0        0        0     3785 2022-12-18 11:49:30.226388 aio_kong-3.0.0/kong/client.py
--rw-r--r--   0        0        0     5342 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/components.py
--rw-r--r--   0        0        0     2720 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/consumers.py
--rw-r--r--   0        0        0     2685 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/plugins.py
--rw-r--r--   0        0        0     1461 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/routes.py
--rw-r--r--   0        0        0     2514 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/services.py
--rw-r--r--   0        0        0      665 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/snis.py
--rw-r--r--   0        0        0      931 2022-12-18 11:49:30.230388 aio_kong-3.0.0/kong/utils.py
--rw-r--r--   0        0        0     1563 2022-12-18 11:49:30.230388 aio_kong-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2177 2022-12-18 11:49:30.230388 aio_kong-3.0.0/readme.md
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 aio_kong-3.0.0/setup.py
--rw-r--r--   0        0        0     3587 1970-01-01 00:00:00.000000 aio_kong-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-05-28 17:47:27.486255 aio_kong-3.3.0/LICENSE
+-rw-r--r--   0        0        0       54 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/__init__.py
+-rw-r--r--   0        0        0     2315 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/auths.py
+-rw-r--r--   0        0        0      278 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/certificates.py
+-rw-r--r--   0        0        0     1986 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/cli.py
+-rw-r--r--   0        0        0     3783 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/client.py
+-rw-r--r--   0        0        0     5342 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/components.py
+-rw-r--r--   0        0        0     2720 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/consumers.py
+-rw-r--r--   0        0        0     2685 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/plugins.py
+-rw-r--r--   0        0        0     1526 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/routes.py
+-rw-r--r--   0        0        0     2514 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/services.py
+-rw-r--r--   0        0        0      665 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/snis.py
+-rw-r--r--   0        0        0      931 2023-05-28 17:47:27.486255 aio_kong-3.3.0/kong/utils.py
+-rw-r--r--   0        0        0     1563 2023-05-28 17:47:27.486255 aio_kong-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2192 2023-05-28 17:47:27.486255 aio_kong-3.3.0/readme.md
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 aio_kong-3.3.0/PKG-INFO
```

### Comparing `aio_kong-3.0.0/LICENSE` & `aio_kong-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/auths.py` & `aio_kong-3.3.0/kong/auths.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/cli.py` & `aio_kong-3.3.0/kong/cli.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/client.py` & `aio_kong-3.3.0/kong/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def __repr__(self) -> str:
         return self.url
 
     __str__ = __repr__
 
     @property
-    def cli(self) -> "Kong":
+    def cli(self) -> Kong:
         return self
 
     async def close(self) -> None:
         if self.session:
             await self.session.close()
 
     async def __aenter__(self) -> Kong:
```

### Comparing `aio_kong-3.0.0/kong/components.py` & `aio_kong-3.3.0/kong/components.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/consumers.py` & `aio_kong-3.3.0/kong/consumers.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/plugins.py` & `aio_kong-3.3.0/kong/plugins.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/routes.py` & `aio_kong-3.3.0/kong/routes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from itertools import zip_longest
 from typing import cast
 
 from .components import UUID, CrudComponent, JsonType
 from .plugins import KongEntityWithPlugins
 from .utils import as_list
 
 
@@ -15,30 +14,32 @@
     Entity = KongEntityWithPlugins
 
     async def delete(self, id_: str | UUID) -> bool:
         route = cast(KongEntityWithPlugins, self.wrap({"id": id_}))
         await route.plugins.delete_all()
         return await super().delete(id_)
 
-    async def apply_json(self, data: JsonType, clear: bool = True) -> list:
+    async def apply_json(self, data: JsonType, clear: bool = True) -> list[dict]:
         if not isinstance(data, list):
             data = [data]
         routes = await self.get_list()
+        route_map = {r.name: r for r in routes}
         result = []
-        for entry, route in zip_longest(data, routes):
-            if not entry:
-                if route and clear:
-                    await self.delete(route.id)
-                continue
+        for entry in data:
+            name = entry.get("name")
+            route = route_map.pop(name, None) if name else None
             entry = entry.copy()
             plugins = entry.pop("plugins", [])
             as_list("hosts", entry)
             as_list("paths", entry)
             as_list("methods", entry)
             if not route:
                 entity = await self.create(**entry)
             else:
                 entity = await self.update(route.id, **entry)
             route = cast(KongEntityWithPlugins, entity)
             route.data["plugins"] = await route.plugins.apply_json(plugins)
             result.append(route.data)
+        if clear:
+            for route in route_map.values():
+                await self.delete(route.id)
         return result
```

### Comparing `aio_kong-3.0.0/kong/services.py` & `aio_kong-3.3.0/kong/services.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/snis.py` & `aio_kong-3.3.0/kong/snis.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/kong/utils.py` & `aio_kong-3.3.0/kong/utils.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.0.0/pyproject.toml` & `aio_kong-3.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-kong"
-version = "3.0.0"
+version = "3.3.0"
 description = "Asynchronous Kong Client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 packages = [
     {include = "kong"}
 ]
```

### Comparing `aio_kong-3.0.0/readme.md` & `aio_kong-3.3.0/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Async Python Client for Kong
 
 [![PyPI version](https://badge.fury.io/py/aio-kong.svg)](https://badge.fury.io/py/aio-kong)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-kong.svg)](https://pypi.org/project/aio-kong)
 [![Build](https://github.com/quantmind/aio-kong/workflows/build/badge.svg)](https://github.com/quantmind/aio-kong/actions?query=workflow%3Abuild)
-[![codecov](https://codecov.io/gh/quantmind/aio-kong/branch/master/graph/badge.svg)](https://codecov.io/gh/quantmind/aio-kong)
+[![codecov](https://codecov.io/gh/quantmind/aio-kong/branch/main/graph/badge.svg?token=JF5L0PEkW6)](https://codecov.io/gh/quantmind/aio-kong)
 [![Downloads](https://img.shields.io/pypi/dd/aio-kong.svg)](https://pypi.org/project/aio-kong/)
 
 
-Tested with [kong][] v3.1
+Tested with [kong][] v3.3
 
 ## Installation & Testing
 
 To install the package
 
 ```
 pip install aio-kong
```

### Comparing `aio_kong-3.0.0/setup.py` & `aio_kong-3.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,114 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aio-kong
+Version: 3.3.0
+Summary: Asynchronous Kong Client
+License: BSD-3-Clause
+Author: Luca
+Author-email: luca@quantmind.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Project-URL: Issues, https://github.com/quantmind/aio-kong/issues
+Project-URL: Repository, https://github.com/quantmind/aio-kong
+Description-Content-Type: text/markdown
+
+# Async Python Client for Kong
+
+[![PyPI version](https://badge.fury.io/py/aio-kong.svg)](https://badge.fury.io/py/aio-kong)
+[![Python versions](https://img.shields.io/pypi/pyversions/aio-kong.svg)](https://pypi.org/project/aio-kong)
+[![Build](https://github.com/quantmind/aio-kong/workflows/build/badge.svg)](https://github.com/quantmind/aio-kong/actions?query=workflow%3Abuild)
+[![codecov](https://codecov.io/gh/quantmind/aio-kong/branch/main/graph/badge.svg?token=JF5L0PEkW6)](https://codecov.io/gh/quantmind/aio-kong)
+[![Downloads](https://img.shields.io/pypi/dd/aio-kong.svg)](https://pypi.org/project/aio-kong/)
+
+
+Tested with [kong][] v3.3
+
+## Installation & Testing
+
+To install the package
+
+```
+pip install aio-kong
+```
+
+To run tests, clone and
+
+```
+make test
+```
+
+:warning: If you don't have Kong or postgres running locally, run the services first
+
+```bash
+make services
+```
+
+test certificates were generated using the command
+
+```
+openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -nodes -subj '/CN=localhost'
+```
+
+## Client
+
+The client can be imported via
+
+```python
+from kong.client import Kong
+```
+
+In a coroutine:
+
+```python
+async with Kong() as cli:
+    services = await cli.services.get_list()
+    print(json.dumps([s.data for s in services], indent=2))
+```
+
+By default the url is obtained from the "KONG_ADMIN_URL" environment variable which defaults to http://127.0.0.1:8001.
+
+The client has handlers for all Kong objects
+
+- [cli.services](./kong/services.py) CRUD operations on services
+- [cli.routes](./kong/routes.py) CRUD operations on routes
+- [cli.plugins](./kong/plugins.py) CRUD operations on plugins
+- [cli.consumers](./kong/consumers.py) CRUD operations on consumers
+- [cli.certificates](./kong/certificates.py) CRUD operations on TLS certificates
+- [cli.snis](./kong/snis.py) CRUD operations on SNIs
+- `cli.acls` To list all ACLs
+
+### Apply a configuration
+
+The client allow to apply a configuration object to kong:
+
+```python
+await cli.apply_json(config)
+```
+
+## Command line tool
+
+The library install the `kongfig` command line tool for uploading kong configuration files.
+
+```
+kongfig --yaml config.yaml
+```
 
-packages = \
-['kong']
+[kong]: https://github.com/Kong/kong
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0', 'aiohttp>=3.8.1,<4.0.0', 'click>=8.1.3,<9.0.0']
-
-setup_kwargs = {
-    'name': 'aio-kong',
-    'version': '3.0.0',
-    'description': 'Asynchronous Kong Client',
-    'long_description': '# Async Python Client for Kong\n\n[![PyPI version](https://badge.fury.io/py/aio-kong.svg)](https://badge.fury.io/py/aio-kong)\n[![Python versions](https://img.shields.io/pypi/pyversions/aio-kong.svg)](https://pypi.org/project/aio-kong)\n[![Build](https://github.com/quantmind/aio-kong/workflows/build/badge.svg)](https://github.com/quantmind/aio-kong/actions?query=workflow%3Abuild)\n[![codecov](https://codecov.io/gh/quantmind/aio-kong/branch/master/graph/badge.svg)](https://codecov.io/gh/quantmind/aio-kong)\n[![Downloads](https://img.shields.io/pypi/dd/aio-kong.svg)](https://pypi.org/project/aio-kong/)\n\n\nTested with [kong][] v3.1\n\n## Installation & Testing\n\nTo install the package\n\n```\npip install aio-kong\n```\n\nTo run tests, clone and\n\n```\nmake test\n```\n\n:warning: If you don\'t have Kong or postgres running locally, run the services first\n\n```bash\nmake services\n```\n\ntest certificates were generated using the command\n\n```\nopenssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -nodes -subj \'/CN=localhost\'\n```\n\n## Client\n\nThe client can be imported via\n\n```python\nfrom kong.client import Kong\n```\n\nIn a coroutine:\n\n```python\nasync with Kong() as cli:\n    services = await cli.services.get_list()\n    print(json.dumps([s.data for s in services], indent=2))\n```\n\nBy default the url is obtained from the "KONG_ADMIN_URL" environment variable which defaults to http://127.0.0.1:8001.\n\nThe client has handlers for all Kong objects\n\n- [cli.services](./kong/services.py) CRUD operations on services\n- [cli.routes](./kong/routes.py) CRUD operations on routes\n- [cli.plugins](./kong/plugins.py) CRUD operations on plugins\n- [cli.consumers](./kong/consumers.py) CRUD operations on consumers\n- [cli.certificates](./kong/certificates.py) CRUD operations on TLS certificates\n- [cli.snis](./kong/snis.py) CRUD operations on SNIs\n- `cli.acls` To list all ACLs\n\n### Apply a configuration\n\nThe client allow to apply a configuration object to kong:\n\n```python\nawait cli.apply_json(config)\n```\n\n## Command line tool\n\nThe library install the `kongfig` command line tool for uploading kong configuration files.\n\n```\nkongfig --yaml config.yaml\n```\n\n[kong]: https://github.com/Kong/kong\n',
-    'author': 'Luca',
-    'author_email': 'luca@quantmind.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

