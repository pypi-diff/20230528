# Comparing `tmp/sentry_dynamic_sampling_lib-1.1.4a1.tar.gz` & `tmp/sentry_dynamic_sampling_lib-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_dynamic_sampling_lib-1.1.4a1.tar", max compression
+gzip compressed data, was "sentry_dynamic_sampling_lib-1.2.0a1.tar", max compression
```

## Comparing `sentry_dynamic_sampling_lib-1.1.4a1.tar` & `sentry_dynamic_sampling_lib-1.2.0a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1303 2023-02-27 13:19:59.475966 sentry_dynamic_sampling_lib-1.1.4a1/LICENSE
--rw-r--r--   0        0        0     2047 2023-02-27 13:19:59.475966 sentry_dynamic_sampling_lib-1.1.4a1/README.md
--rw-r--r--   0        0        0     3101 2023-02-27 13:20:10.583878 sentry_dynamic_sampling_lib-1.1.4a1/pyproject.toml
--rw-r--r--   0        0        0     1672 2023-02-27 13:19:59.479966 sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/__init__.py
--rw-r--r--   0        0        0     5424 2023-02-27 13:19:59.479966 sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/sampler.py
--rw-r--r--   0        0        0      568 2023-02-27 13:19:59.479966 sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/settings.py
--rw-r--r--   0        0        0     3158 2023-02-27 13:19:59.479966 sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/shared.py
--rw-r--r--   0        0        0      507 2023-02-27 13:19:59.479966 sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/utils.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.1.4a1/setup.py
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.1.4a1/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-05-28 14:55:25.309643 sentry_dynamic_sampling_lib-1.2.0a1/LICENSE
+-rw-r--r--   0        0        0     2047 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/README.md
+-rw-r--r--   0        0        0     3101 2023-05-28 14:55:35.061684 sentry_dynamic_sampling_lib-1.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1682 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/__init__.py
+-rw-r--r--   0        0        0     5617 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/sampler.py
+-rw-r--r--   0        0        0      603 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/settings.py
+-rw-r--r--   0        0        0     4089 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/shared.py
+-rw-r--r--   0        0        0      507 2023-05-28 14:55:25.313644 sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/utils.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a1/setup.py
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 sentry_dynamic_sampling_lib-1.2.0a1/PKG-INFO
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/LICENSE` & `sentry_dynamic_sampling_lib-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/README.md` & `sentry_dynamic_sampling_lib-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/pyproject.toml` & `sentry_dynamic_sampling_lib-1.2.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentry-dynamic-sampling-lib"
-version = "1.1.4-alpha.1"
+version = "1.2.0-alpha.1"
 description = "This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling."
 authors = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 maintainers = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
 readme = "README.md"
 packages = [{ include = "sentry_dynamic_sampling_lib" }]
 license = "BSD-2-Clause"
 repository = "https://github.com/SpikeeLabs/django-admin-action-tools"
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/__init__.py` & `sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     if client is None:
         return
 
     if CONTROLLER_HOST:
         app_key = build_app_key(client.options)
         controller_endpoint = urljoin(CONTROLLER_HOST, CONTROLLER_PATH)
         metric_endpoint = urljoin(CONTROLLER_HOST, METRIC_PATH)
-        print(f"Sentry Wrapper: Injecting TracesSampler. App Key : {app_key}")
+        LOGGER.warning("Sentry Wrapper: Injecting TracesSampler. App Key : %s", app_key)
         client.options["traces_sampler"] = TraceSampler(
             poll_interval=POLL_INTERVAL,
             metric_interval=METRIC_INTERVAL,
             metric_endpoint=metric_endpoint,
             controller_endpoint=controller_endpoint,
             app_key=app_key,
         )
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/sampler.py` & `sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.metrics.set_mode(MetricType.WSGI, data["wsgi_collect_metrics"])
 
     def update_metrics(self):
         for metric_type, data in self.metrics:
             data = {
                 "app": self.app_key,
                 "type": metric_type.value,
-                "data": dict(data.most_common(10)),
+                "data": dict(data),
             }
             try:
                 self.session.post(
                     self.metric_endpoint.format(self.app_key, metric_type.value),
                     json=data,
                 )
                 LOGGER.debug("Metric %s pushed", metric_type.value)
@@ -150,16 +150,18 @@
         self.kill()
 
     def __call__(self, sampling_context):
         self._ensure_controller()
         if sampling_context:
             if "wsgi_environ" in sampling_context:
                 path = sampling_context["wsgi_environ"].get("PATH_INFO", "")
-                if path in self.app_config.ignored_paths:
+                user_agent = sampling_context["wsgi_environ"].get("HTTP_USER_AGENT", "")
+                if path in self.app_config.ignored_paths or user_agent.startswith(self.app_config.ignored_user_agents):
                     return 0
                 self.metrics.count_path(path)
+                self.metrics.count_user_agent(user_agent)
             if "celery_job" in sampling_context:
                 task = sampling_context["celery_job"].get("task", "")
                 if task in self.app_config.ignored_tasks:
                     return 0
                 self.metrics.count_task(task)
         return self.app_config.sample_rate
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/settings.py` & `sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 # default value overridden by controller
 DEFAULT_IGNORED_PATH = {"/health", "/healthz", "/health/", "/healthz/"}
 DEFAULT_IGNORED_TASK = set()
+DEFAULT_IGNORED_USER_AGENT = set()
 DEFAULT_SAMPLE_RATE = 0.0
 
 # controller variables
 CONTROLLER_HOST = os.getenv("SENTRY_CONTROLLER_HOST")
 CONTROLLER_PATH = os.getenv("SENTRY_CONTROLLER_PATH", "/sentry/apps/{}/")
 METRIC_PATH = os.getenv("SENTRY_CONTROLLER_METRIC_PATH", "/sentry/apps/{}/metrics/{}/")
 POLL_INTERVAL = int(os.getenv("SENTRY_CONTROLLER_POLL_INTERVAL", "60"))
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/sentry_dynamic_sampling_lib/shared.py` & `sentry_dynamic_sampling_lib-1.2.0a1/sentry_dynamic_sampling_lib/shared.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 from collections import Counter
 from enum import Enum
 from threading import RLock
 
 from sentry_dynamic_sampling_lib.settings import (
     DEFAULT_IGNORED_PATH,
     DEFAULT_IGNORED_TASK,
+    DEFAULT_IGNORED_USER_AGENT,
     DEFAULT_SAMPLE_RATE,
 )
 from sentry_dynamic_sampling_lib.utils import synchronized
 
 LOGGER = logging.getLogger("SentryWrapper")
 
 
 class AppConfig:
     def __init__(self) -> None:
         self._lock = RLock()
         self._sample_rate = DEFAULT_SAMPLE_RATE
         self._ignored_paths = DEFAULT_IGNORED_PATH
+        self._ignored_user_agents = tuple(DEFAULT_IGNORED_USER_AGENT)
         self._ignored_tasks = DEFAULT_IGNORED_TASK
 
     @property
     @synchronized
     def sample_rate(self):
         return self._sample_rate
 
@@ -38,75 +40,96 @@
     @ignored_paths.setter
     @synchronized
     def ignored_paths(self, new_ignored_paths):
         self._ignored_paths = set(new_ignored_paths)
 
     @property
     @synchronized
+    def ignored_user_agents(self):
+        return self._ignored_user_agents
+
+    @ignored_user_agents.setter
+    @synchronized
+    def ignored_user_agents(self, new_ignored_user_agents):
+        self._ignored_user_agents = tuple(new_ignored_user_agents)
+
+    @property
+    @synchronized
     def ignored_tasks(self):
         return self._ignored_tasks
 
     @ignored_tasks.setter
     @synchronized
     def ignored_tasks(self, new_ignored_tasks):
         self._ignored_tasks = set(new_ignored_tasks)
 
     @synchronized
     def update(self, data):
         self._sample_rate = data["active_sample_rate"]
         self._ignored_paths = set(data["wsgi_ignore_path"])
         self._ignored_tasks = set(data["celery_ignore_task"])
+        self._ignored_user_agents = tuple(data.get("wsgi_ignore_user_agent", []))
 
 
 class MetricType(Enum):
     WSGI = "WSGI"
     CELERY = "CELERY"
 
 
 class Metric:
     def __init__(self) -> None:
         self._lock = RLock()
         self._metrics = {
-            MetricType.WSGI: {"activated": False, "data": Counter()},
-            MetricType.CELERY: {"activated": False, "data": Counter()},
+            MetricType.WSGI: {"activated": False, "data": {"path": Counter(), "user_agent": Counter()}},
+            MetricType.CELERY: {"activated": False, "data": {"task": Counter()}},
         }
 
     def set_mode(self, _type, mode):
         self._metrics[_type]["activated"] = mode
 
     def get_mode(self, _type):
         return self._metrics[_type]["activated"]
 
     @synchronized
     def count_path(self, path):
         metric = self._metrics[MetricType.WSGI]
         if metric["activated"]:
-            metric["data"][path] += 1
+            metric["data"]["path"][path] += 1
+
+    @synchronized
+    def count_user_agent(self, user_agent):
+        metric = self._metrics[MetricType.WSGI]
+        if metric["activated"]:
+            metric["data"]["user_agent"][user_agent] += 1
 
     @synchronized
     def count_task(self, path):
         metric = self._metrics[MetricType.CELERY]
         if metric["activated"]:
-            metric["data"][path] += 1
+            metric["data"]["task"][path] += 1
 
     def __iter__(self):
         """
         List activated non-empty metrics
 
         Yields:
             Tuple(MetricType, Counter): the activated non-empty metrics
         """
         for metric_type, metric in self._metrics.items():
             # check if metric is activated
             if not metric["activated"]:
                 LOGGER.debug("Metric %s disabled", metric_type.value)
                 continue
             with self._lock:
-                # check im metric is empty
-                if len(metric["data"]) == 0:
-                    LOGGER.debug("Metric %s is empty", metric_type.value)
+                data = {}
+                for name, counter in metric["data"].items():
+                    # check if metric is empty
+                    if len(counter) == 0:
+                        LOGGER.debug("Metric %s:%s is empty", metric_type.value, name)
+                        continue
+                    data[name] = dict(counter.most_common(10))
+                    metric["data"][name] = Counter()
+                if not data:
                     continue
-                data = metric["data"]
-                metric["data"] = Counter()
 
             # yield outside of the lock to not block write while callee execute
             yield metric_type, data
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/setup.py` & `sentry_dynamic_sampling_lib-1.2.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psutil>=5.9.4,<6.0.0',
  'requests-cache>=0.9.7,<0.10.0',
  'schedule>=1.1.0,<2.0.0',
  'wrapt>=1.14.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'sentry-dynamic-sampling-lib',
-    'version': '1.1.4a1',
+    'version': '1.2.0a1',
     'description': 'This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling.',
     'long_description': '# Sentry Dynamic Sampling Controller\n\n[![PyPI](https://img.shields.io/pypi/v/sentry-dynamic-sampling-lib?color=blue)](https://pypi.org/project/sentry-dynamic-sampling-lib/)\n![Tests Status](https://github.com/SpikeeLabs/sentry-dynamic-sampling-lib/actions/workflows/.github/workflows/tests.yml/badge.svg)\n[![codecov](https://codecov.io/gh/SpikeeLabs/sentry-dynamic-sampling-lib/branch/main/graph/badge.svg?token=RON7F8QTZX)](https://codecov.io/gh/SpikeeLabs/sentry-dynamic-sampling-lib)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sentry-dynamic-sampling-lib)\n![PyPI - License](https://img.shields.io/pypi/l/sentry-dynamic-sampling-lib)\n\n---\nThis project aims to provide dynamic sampling without relying on Sentry own\'s Dynamic Sampling.\nThis libs works by adding a `traces_sampler` callback to sentry.\nIn the background a thread fetch the data from the [controller](https://github.com/SpikeeLabs/sentry-dynamic-sampling-controller)\nIt\'s also able to ignore WSGI route an Celery task set in controller.\n\n\n\n\n\n## Usage\n```python\nimport sentry_sdk\nfrom sentry_dynamic_sampling_lib import init_wrapper\n\n# init sentry as usual\n# without traces_sampler and sample_rate param\nsentry_sdk.init(  # pylint: disable=E0110\n    dsn=SENTRY_DSN,\n    integrations=[],\n    environment=ENVIRONMENT,\n    release=SENTRY_RELEASE,\n)\n\n# hook sentry_dynamic_sampling_lib into sentry\ninit_wrapper()\n```\n\n\n## Configuration\nThe following environment variables can be used to configure the lib\n\n```bash\nSENTRY_CONTROLLER_HOST=none # (required, no default)\nSENTRY_CONTROLLER_PATH="/sentry/apps/{}/" # (optional, default to example)\nSENTRY_CONTROLLER_METRIC_PATH="/sentry/apps/{}/metrics/{}/" # (optional, default to example)\nSENTRY_CONTROLLER_POLL_INTERVAL=60 # (optional, default to example)\nSENTRY_CONTROLLER_METRIC_INTERVAL=600 # (optional, default to example)\n```\n\n\n\n\n## Development\n```bash\n# install deps\npoetry install\n\n# pre-commit\npoetry run pre-commit install --install-hook\npoetry run pre-commit install --install-hooks --hook-type commit-msg\n```\n',
     'author': 'jeanloup.monnier',
     'author_email': 'jean-loup.monnier@spikeelabs.fr',
     'maintainer': 'jeanloup.monnier',
     'maintainer_email': 'jean-loup.monnier@spikeelabs.fr',
     'url': 'https://github.com/SpikeeLabs/django-admin-action-tools',
```

### Comparing `sentry_dynamic_sampling_lib-1.1.4a1/PKG-INFO` & `sentry_dynamic_sampling_lib-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-dynamic-sampling-lib
-Version: 1.1.4a1
+Version: 1.2.0a1
 Summary: This project aims to provide dynamic sampling without relying on Sentry Dynamic Sampling.
 Home-page: https://github.com/SpikeeLabs/django-admin-action-tools
 License: BSD-2-Clause
 Author: jeanloup.monnier
 Author-email: jean-loup.monnier@spikeelabs.fr
 Maintainer: jeanloup.monnier
 Maintainer-email: jean-loup.monnier@spikeelabs.fr
```

