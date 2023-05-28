# Comparing `tmp/faceid-lib-2.0.1.tar.gz` & `tmp/faceid-lib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid-lib-2.0.1.tar", max compression
+gzip compressed data, was "faceid-lib-2.0.2.tar", max compression
```

## Comparing `faceid-lib-2.0.1.tar` & `faceid-lib-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0     2640 2023-05-02 16:15:31.835306 faceid-lib-2.0.1/README.md
--rw-r--r--   0        0        0      590 2023-05-02 16:07:58.988298 faceid-lib-2.0.1/faceid_lib/CHANGELOG.md
--rw-r--r--   0        0        0      207 2022-06-14 05:34:42.430362 faceid-lib-2.0.1/faceid_lib/Makefile
--rw-r--r--   0        0        0       22 2021-09-08 03:10:42.869012 faceid-lib-2.0.1/faceid_lib/__init__.py
--rw-r--r--   0        0        0       89 2021-09-08 03:10:42.869614 faceid-lib-2.0.1/faceid_lib/__main__.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.869886 faceid-lib-2.0.1/faceid_lib/events/__init__.py
--rw-r--r--   0        0        0     2457 2021-11-24 01:10:13.748662 faceid-lib-2.0.1/faceid_lib/events/event_producer.py
--rw-r--r--   0        0        0     2389 2021-11-24 01:10:07.200887 faceid-lib-2.0.1/faceid_lib/events/event_receiver.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.872032 faceid-lib-2.0.1/faceid_lib/logger/__init__.py
--rw-r--r--   0        0        0      199 2021-09-08 03:10:42.872966 faceid-lib-2.0.1/faceid_lib/logger/logger_helper.py
--rw-r--r--   0        0        0     2220 2022-06-14 06:03:39.559713 faceid-lib-2.0.1/faceid_lib/ratelimiter/__init__.py
--rw-r--r--   0        0        0     2579 2021-10-24 16:39:30.131894 faceid-lib-2.0.1/faceid_lib/ratelimiter/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1735 2021-10-24 16:39:30.133523 faceid-lib-2.0.1/faceid_lib/ratelimiter/__pycache__/depends.cpython-39.pyc
--rw-r--r--   0        0        0     1754 2021-10-24 16:39:30.134988 faceid-lib-2.0.1/faceid_lib/ratelimiter/depends.py
--rw-r--r--   0        0        0        0 2023-05-02 08:06:17.257207 faceid-lib-2.0.1/faceid_lib/vector_similarity/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 08:06:29.895236 faceid-lib-2.0.1/faceid_lib/vector_similarity/v1/__init__.py
--rw-r--r--   0        0        0     1263 2023-05-02 16:03:47.093803 faceid-lib-2.0.1/faceid_lib/vector_similarity/v1/power.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.873272 faceid-lib-2.0.1/faceid_lib/workflow/__init__.py
--rw-r--r--   0        0        0      284 2021-09-08 03:10:42.873899 faceid-lib-2.0.1/faceid_lib/workflow/workflow_helper.py
--rw-r--r--   0        0        0     1253 2023-05-02 16:15:39.931279 faceid-lib-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3833 2023-05-02 16:18:08.579347 faceid-lib-2.0.1/setup.py
--rw-r--r--   0        0        0     3806 2023-05-02 16:18:08.579867 faceid-lib-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2640 2023-05-28 15:35:29.796981 faceid-lib-2.0.2/README.md
+-rw-r--r--   0        0        0     2235 2023-05-26 08:43:24.659565 faceid-lib-2.0.2/build.py
+-rw-r--r--   0        0        0      590 2023-05-26 07:24:21.410634 faceid-lib-2.0.2/faceid_lib/CHANGELOG.md
+-rw-r--r--   0        0        0      240 2023-05-26 08:41:56.166622 faceid-lib-2.0.2/faceid_lib/Makefile
+-rwxr-xr-x   0        0        0    39408 2023-05-28 15:42:19.000000 faceid-lib-2.0.2/faceid_lib/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    47040 2023-05-28 15:42:20.000000 faceid-lib-2.0.2/faceid_lib/__main__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    39024 2023-05-28 15:42:37.000000 faceid-lib-2.0.2/faceid_lib/events/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    96640 2023-05-28 15:42:34.000000 faceid-lib-2.0.2/faceid_lib/events/event_producer.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    96400 2023-05-28 15:42:37.000000 faceid-lib-2.0.2/faceid_lib/events/event_receiver.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    39024 2023-05-28 15:42:20.000000 faceid-lib-2.0.2/faceid_lib/logger/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    65280 2023-05-28 15:42:21.000000 faceid-lib-2.0.2/faceid_lib/logger/logger_helper.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   128696 2023-05-28 15:42:27.000000 faceid-lib-2.0.2/faceid_lib/ratelimiter/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0   122464 2023-05-28 15:42:24.000000 faceid-lib-2.0.2/faceid_lib/ratelimiter/depends.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    39160 2023-05-28 15:42:27.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    39104 2023-05-28 15:42:28.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    68360 2023-05-28 15:42:29.000000 faceid-lib-2.0.2/faceid_lib/vector_similarity/v1/power.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    39048 2023-05-28 15:42:32.000000 faceid-lib-2.0.2/faceid_lib/workflow/__init__.cpython-38-darwin.so
+-rwxr-xr-x   0        0        0    66688 2023-05-28 15:42:31.000000 faceid-lib-2.0.2/faceid_lib/workflow/workflow_helper.cpython-38-darwin.so
+-rw-r--r--   0        0        0     1629 2023-05-28 15:41:41.440546 faceid-lib-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3696 2023-05-28 15:43:09.081791 faceid-lib-2.0.2/PKG-INFO
```

### Comparing `faceid-lib-2.0.1/README.md` & `faceid-lib-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.1/faceid_lib/CHANGELOG.md` & `faceid-lib-2.0.2/faceid_lib/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.1/pyproject.toml` & `faceid-lib-2.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,65 @@
 [tool.poetry]
 name = "faceid-lib"
-version = "2.0.1"
+version = "2.0.2"
 description = "Simple and flexible AI/ML workflow engine by Picaso - FaceID"
 authors = ["Dani Gunawan <danigunawan.elektroug@gmail.com>"]
-# New attributes
+
 license = "Apache License"
 readme = "README.md"
-homepage = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
-repository = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
+homepage = "#"
+repository = "#"
 keywords = ["machine learning", "Deep Learning", "Message Broker", "Distributed System", "pipeline", "rabbitmq", "ratelimiter"]
 classifiers = [
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.7",
 ]
+
+# Only include cythonized files in final build
 include = [
     "LICENSE",
+    "faceid_lib/**/*.so",  # ignored in VCS, so we need to be explicit
 ]
 
+exclude = [
+    "faceid_lib/**/*.py",
+    ]
+
 [tool.poetry.dependencies]
 python = "^3.7"
 pika = "^1.2.0"
-requests = "^2.25.1"
+requests = "*"
+# requests-toolbelt = "^0.10.1"
+# urllib3 = "^1.26.15"
 aioredis = "1.3.1"
 fastapi = "*"
+appengine-python-standard = "^1.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 bandit = "*"
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 pytest-xdist = "*"
 uvicorn = "*"
 requests = "*"
+# requests-toolbelt = "^0.10.1"
+# urllib3 = "^1.26.15"
+Cython = "*"
 
-# New scripts
 [tool.poetry.scripts]
 faceid-lib = 'faceid_lib:main'
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0", "setuptools~=50.3.2"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.build]
+# The allows us to build C extensions (using Cython). Unstable feature
+# https://github.com/python-poetry/poetry/issues/2740#issuecomment-666551481
+script = "build.py"
+generate-setup-file = false
```

### Comparing `faceid-lib-2.0.1/setup.py` & `faceid-lib-2.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,163 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: faceid-lib
+Version: 2.0.2
+Summary: Simple and flexible AI/ML workflow engine by Picaso - FaceID
+Home-page: #
+License: Apache License
+Keywords: machine learning,Deep Learning,Message Broker,Distributed System,pipeline,rabbitmq,ratelimiter
+Author: Dani Gunawan
+Author-email: danigunawan.elektroug@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Requires-Dist: aioredis (==1.3.1)
+Requires-Dist: appengine-python-standard (>=1.1.1,<2.0.0)
+Requires-Dist: fastapi
+Requires-Dist: pika (>=1.2.0,<2.0.0)
+Requires-Dist: requests
+Project-URL: Repository, #
+Description-Content-Type: text/markdown
+
+# picaso-engine ML faceid workflow
+
+## Overview
+
+This is a helper library for picaso-engine ML faceid workflow product. The idea of this library is to wrap all reusable code to simplify and improve workflow implementation.
+
+Supported functionality:
+
+- API to communicate with RabbitMQ for event receiver/producer
+- Workflow call helper
+- Logger call helper
+- Rate-limiting strategies
+- Computing vector similarity helper (ex. Face Similarity Search)
+
+## Author
+picaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan
+
+## Instructions
+Version number should be updated in __init__.py and pyproject.toml
+
+1. Install Poetry
+
+```
+pip install poetry
+```
+
+2. Add pika and requests libraries
+
+```
+poetry add pika
+poetry add requests
+```
+
+3. Build
+
+```
+poetry lock --no-update
+poetry install
+poetry build
+```
+
+4. Publish to TestPyPI
+
+```
+poetry publish -r testpypi
+```
+
+5. Install from TestPyPI
+
+```
+pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple  faceid-lib
+```
+
+6. Publish to PyPI
+
+```
+poetry publish
+```
+
+7. Install from PyPI
+
+```
+pip install faceid-lib
+```
+
+8. Test imported library from CMD
+
+```
+python -m faceid_lib
+```
+
+9. Import EventReceiver
+
+```
+from faceid_lib.events.event_receiver import EventReceiver
+```
+
+10. Import EventProducer
+
+```
+from faceid_lib.events.event_producer import EventProducer
+```
+
+11. Import FastAPILimiter, RateLimiter
+
+```
+from faceid_lib.ratelimiter import FastAPILimiter
+from faceid_lib.ratelimiter.depends import RateLimiter
+```
+
+## Structure
+
+```
+.
+├── LICENSE
+├── poetry.lock
+├── pyproject.toml
+├── faceid_lib
+│   ├── __init__.py
+│   ├── __main__.py
+│   ├── events
+│       ├── __init__.py
+│       ├── event_producer.py
+│       └── event_receiver.py
+│   ├── ratelimiter
+│       ├── __init__.py
+│       └── depends.py
+│   ├── logger
+│       ├── __init__.py
+│       └── logger_helper.py
+│   ├── workflow
+│       ├── __init__.py
+│       └── workflow_helper.py
+│   ├── vector_similarity
+│       ├── __init__.py
+│       ├── v1
+│           ├── __init__.py
+│           └── power.py
+└── README.md
+```
+
+## Changelogs 2.0.0 - 2.0.1 (2023-05-02)
+- compute similarity helper
+
+## Changelogs 1.0.9 (2022-06-14)
+- modify response & handler
 
-packages = \
-['faceid_lib',
- 'faceid_lib.events',
- 'faceid_lib.logger',
- 'faceid_lib.ratelimiter',
- 'faceid_lib.vector_similarity',
- 'faceid_lib.vector_similarity.v1',
- 'faceid_lib.workflow']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aioredis==1.3.1', 'fastapi', 'pika>=1.2.0,<2.0.0', 'requests>=2.25.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['faceid-lib = faceid_lib:main']}
-
-setup_kwargs = {
-    'name': 'faceid-lib',
-    'version': '2.0.1',
-    'description': 'Simple and flexible AI/ML workflow engine by Picaso - FaceID',
-    'long_description': '# picaso-engine ML faceid workflow\n\n## Overview\n\nThis is a helper library for picaso-engine ML faceid workflow product. The idea of this library is to wrap all reusable code to simplify and improve workflow implementation.\n\nSupported functionality:\n\n- API to communicate with RabbitMQ for event receiver/producer\n- Workflow call helper\n- Logger call helper\n- Rate-limiting strategies\n- Computing vector similarity helper (ex. Face Similarity Search)\n\n## Author\npicaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan\n\n## Instructions\nVersion number should be updated in __init__.py and pyproject.toml\n\n1. Install Poetry\n\n```\npip install poetry\n```\n\n2. Add pika and requests libraries\n\n```\npoetry add pika\npoetry add requests\n```\n\n3. Build\n\n```\npoetry lock --no-update\npoetry install\npoetry build\n```\n\n4. Publish to TestPyPI\n\n```\npoetry publish -r testpypi\n```\n\n5. Install from TestPyPI\n\n```\npip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple  faceid-lib\n```\n\n6. Publish to PyPI\n\n```\npoetry publish\n```\n\n7. Install from PyPI\n\n```\npip install faceid-lib\n```\n\n8. Test imported library from CMD\n\n```\npython -m faceid_lib\n```\n\n9. Import EventReceiver\n\n```\nfrom faceid_lib.events.event_receiver import EventReceiver\n```\n\n10. Import EventProducer\n\n```\nfrom faceid_lib.events.event_producer import EventProducer\n```\n\n11. Import FastAPILimiter, RateLimiter\n\n```\nfrom faceid_lib.ratelimiter import FastAPILimiter\nfrom faceid_lib.ratelimiter.depends import RateLimiter\n```\n\n## Structure\n\n```\n.\n├── LICENSE\n├── poetry.lock\n├── pyproject.toml\n├── faceid_lib\n│   ├── __init__.py\n│   ├── __main__.py\n│   ├── events\n│       ├── __init__.py\n│       ├── event_producer.py\n│       └── event_receiver.py\n│   ├── ratelimiter\n│       ├── __init__.py\n│       └── depends.py\n│   ├── logger\n│       ├── __init__.py\n│       └── logger_helper.py\n│   ├── workflow\n│       ├── __init__.py\n│       └── workflow_helper.py\n│   ├── vector_similarity\n│       ├── __init__.py\n│       ├── v1\n│           ├── __init__.py\n│           └── power.py\n└── README.md\n```\n\n## Changelogs 2.0.0 - 2.0.1 (2023-05-02)\n- compute similarity helper\n\n## Changelogs 1.0.9 (2022-06-14)\n- modify response & handler\n\n## Changelogs 1.0.5 (2021-10-24)\n- downgrade pika version to 1.1.0\n\n## Changelogs 1.0.4 (2021-10-24)\n- enhancment rate limiting\n\n## License\nLicensed under the Apache License, Version 2.0. Copyright 2020-2021 picaso-engine ML, Dani Gunawan.\n',
-    'author': 'Dani Gunawan',
-    'author_email': 'danigunawan.elektroug@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Changelogs 1.0.5 (2021-10-24)
+- downgrade pika version to 1.1.0
 
+## Changelogs 1.0.4 (2021-10-24)
+- enhancment rate limiting
+
+## License
+Licensed under the Apache License, Version 2.0. Copyright 2020-2021 picaso-engine ML, Dani Gunawan.
 
-setup(**setup_kwargs)
```

