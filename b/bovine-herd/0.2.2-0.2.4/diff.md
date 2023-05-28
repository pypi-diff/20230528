# Comparing `tmp/bovine_herd-0.2.2.tar.gz` & `tmp/bovine_herd-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_herd-0.2.2.tar", max compression
+gzip compressed data, was "bovine_herd-0.2.4.tar", max compression
```

## Comparing `bovine_herd-0.2.2.tar` & `bovine_herd-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1345 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/README.md
--rw-r--r--   0        0        0     1763 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/__init__.py
--rw-r--r--   0        0        0      488 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/config.py
--rw-r--r--   0        0        0      345 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/__init__.py
--rw-r--r--   0        0        0      698 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/activitypub.py
--rw-r--r--   0        0        0     4986 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/server/endpoints.py
--rw-r--r--   0        0        0      832 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/info.py
--rw-r--r--   0        0        0     1993 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/server/wellknown.py
--rw-r--r--   0        0        0   154974 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/static/cow.jpg
--rw-r--r--   0        0        0   285585 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/static/moocow.png
--rw-r--r--   0        0        0   549258 2023-05-22 14:17:04.650842 bovine_herd-0.2.2/bovine_herd/static/profile.png
--rw-r--r--   0        0        0     1234 2023-05-22 14:17:04.650842 bovine_herd-0.2.2/bovine_herd/static/style.css
--rw-r--r--   0        0        0   362136 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/static/woodpecker.png
--rw-r--r--   0        0        0      961 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/templates/index.html
--rw-r--r--   0        0        0     1128 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/test/__init__.py
--rw-r--r--   0        0        0      274 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/test_utils.py
--rw-r--r--   0        0        0       23 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/version.py
--rw-r--r--   0        0        0      875 2023-05-25 18:44:02.802690 bovine_herd-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 bovine_herd-0.2.2/setup.py
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 bovine_herd-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1345 2023-05-27 18:23:43.579051 bovine_herd-0.2.4/README.md
+-rw-r--r--   0        0        0     1763 2023-05-27 18:23:43.579051 bovine_herd-0.2.4/bovine_herd/__init__.py
+-rw-r--r--   0        0        0      488 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/config.py
+-rw-r--r--   0        0        0      345 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/server/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/server/activitypub.py
+-rw-r--r--   0        0        0     4986 2023-05-27 18:24:49.612369 bovine_herd-0.2.4/bovine_herd/server/endpoints.py
+-rw-r--r--   0        0        0      832 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/server/info.py
+-rw-r--r--   0        0        0     1993 2023-05-27 18:23:43.579051 bovine_herd-0.2.4/bovine_herd/server/wellknown.py
+-rw-r--r--   0        0        0   154974 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/static/cow.jpg
+-rw-r--r--   0        0        0   285585 2023-05-22 14:17:04.646842 bovine_herd-0.2.4/bovine_herd/static/moocow.png
+-rw-r--r--   0        0        0   549258 2023-05-22 14:17:04.650842 bovine_herd-0.2.4/bovine_herd/static/profile.png
+-rw-r--r--   0        0        0     1234 2023-05-22 14:17:04.650842 bovine_herd-0.2.4/bovine_herd/static/style.css
+-rw-r--r--   0        0        0   362136 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/static/woodpecker.png
+-rw-r--r--   0        0        0      961 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/templates/index.html
+-rw-r--r--   0        0        0     1128 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/utils/test/__init__.py
+-rw-r--r--   0        0        0      274 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/utils/test_utils.py
+-rw-r--r--   0        0        0       23 2023-05-22 14:17:04.654842 bovine_herd-0.2.4/bovine_herd/version.py
+-rw-r--r--   0        0        0      875 2023-05-27 18:57:02.807740 bovine_herd-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 bovine_herd-0.2.4/setup.py
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 bovine_herd-0.2.4/PKG-INFO
```

### Comparing `bovine_herd-0.2.2/README.md` & `bovine_herd-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/__init__.py` & `bovine_herd-0.2.4/bovine_herd/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/server/activitypub.py` & `bovine_herd-0.2.4/bovine_herd/server/activitypub.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/server/endpoints.py` & `bovine_herd-0.2.4/bovine_herd/server/endpoints.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/server/info.py` & `bovine_herd-0.2.4/bovine_herd/server/info.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/server/wellknown.py` & `bovine_herd-0.2.4/bovine_herd/server/wellknown.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/static/cow.jpg` & `bovine_herd-0.2.4/bovine_herd/static/cow.jpg`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/static/moocow.png` & `bovine_herd-0.2.4/bovine_herd/static/moocow.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/static/profile.png` & `bovine_herd-0.2.4/bovine_herd/static/profile.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/static/style.css` & `bovine_herd-0.2.4/bovine_herd/static/style.css`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/static/woodpecker.png` & `bovine_herd-0.2.4/bovine_herd/static/woodpecker.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/templates/index.html` & `bovine_herd-0.2.4/bovine_herd/templates/index.html`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/utils/__init__.py` & `bovine_herd-0.2.4/bovine_herd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/bovine_herd/utils/test/__init__.py` & `bovine_herd-0.2.4/bovine_herd/utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.2/pyproject.toml` & `bovine_herd-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "bovine-herd"
-version = "0.2.2"
+version = "0.2.4"
 description = ""
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_herd"}]
 repository = "https://codeberg.org/bovine/bovine"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
 markdown = "^3.4.1"
 python-markdown-math = "^0.8"
 bovine-store = "^0.2.1"
 bovine-process = "^0.2.0"
 asyncstdlib = "^3.10.5"
-bovine-pubsub = "^0.2.0"
+bovine-pubsub = "^0.2.4"
 tortoise-orm = {extras = ["asyncpg"], version = "^0.19.3"}
 aiodns = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bovine_herd-0.2.2/setup.py` & `bovine_herd-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 {'': ['*'], 'bovine_herd': ['static/*', 'templates/*']}
 
 install_requires = \
 ['aiodns>=3.0.0,<4.0.0',
  'aiohttp>=3.8.3,<4.0.0',
  'asyncstdlib>=3.10.5,<4.0.0',
  'bovine-process>=0.2.0,<0.3.0',
- 'bovine-pubsub>=0.2.0,<0.3.0',
+ 'bovine-pubsub>=0.2.4,<0.3.0',
  'bovine-store>=0.2.1,<0.3.0',
  'markdown>=3.4.1,<4.0.0',
  'python-markdown-math>=0.8,<0.9',
  'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'bovine-herd',
-    'version': '0.2.2',
+    'version': '0.2.4',
     'description': '',
     'long_description': '# bovine_herd\n\n`bovine_herd` is a `bovine` powered ActivityPub server, which interoperates with the rest of the FediVerse.\n\nRunning:\n\n```bash\npip install bovine_herd\nhypercorn bovine_herd:app\n```\n\nThis will start `bovine_herd` using an sqlite3 database.\n\n## Interacting with the fediverse\n\nAssume that you alias `$DOMAIN` so that it redirects to the above server, e.g. via....\n\nThen by running\n\n```bash\npip install bovine_tool\npython -mbovine_tool.register --domain $DOMAIN moocow\n```\n\nyou create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:\n\n```bash\npython -mbovine_tool.manage --new_did_key $BOVINE_NAME\n```\n\nyou will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via\n\n```bash\npython -mbovine.msg --secret $SECRET --host $DOMAIN moooo\n```\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.\n- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_herd-0.2.2/PKG-INFO` & `bovine_herd-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bovine-herd
-Version: 0.2.2
+Version: 0.2.4
 Summary: 
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: asyncstdlib (>=3.10.5,<4.0.0)
 Requires-Dist: bovine-process (>=0.2.0,<0.3.0)
-Requires-Dist: bovine-pubsub (>=0.2.0,<0.3.0)
+Requires-Dist: bovine-pubsub (>=0.2.4,<0.3.0)
 Requires-Dist: bovine-store (>=0.2.1,<0.3.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: python-markdown-math (>=0.8,<0.9)
 Requires-Dist: tortoise-orm[asyncpg] (>=0.19.3,<0.20.0)
 Project-URL: Repository, https://codeberg.org/bovine/bovine
 Description-Content-Type: text/markdown
```

