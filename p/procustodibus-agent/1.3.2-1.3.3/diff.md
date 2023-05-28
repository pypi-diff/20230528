# Comparing `tmp/procustodibus_agent-1.3.2.tar.gz` & `tmp/procustodibus_agent-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procustodibus_agent-1.3.2.tar", last modified: Fri Mar 17 01:04:21 2023, max compression
+gzip compressed data, was "procustodibus_agent-1.3.3.tar", last modified: Sun May 28 00:35:05 2023, max compression
```

## Comparing `procustodibus_agent-1.3.2.tar` & `procustodibus_agent-1.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2023-03-17 00:35:06.000000 procustodibus_agent-1.3.2/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.3.2/MANIFEST.in
--rw-rw-r--   0 justin    (1000) justin    (1000)     4657 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     3524 2023-03-17 00:35:08.000000 procustodibus_agent-1.3.2/README.md
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/procustodibus_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      200 2023-03-17 00:36:40.000000 procustodibus_agent-1.3.2/procustodibus_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2893 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.2/procustodibus_agent/agent.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    10924 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.2/procustodibus_agent/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1895 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.2/procustodibus_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    14687 2022-09-26 02:23:07.000000 procustodibus_agent-1.3.2/procustodibus_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     5411 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.2/procustodibus_agent/connectivity.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.2/procustodibus_agent/credentials.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    40359 2022-02-24 02:03:11.000000 procustodibus_agent-1.3.2/procustodibus_agent/executor.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3259 2021-11-12 03:42:31.000000 procustodibus_agent-1.3.2/procustodibus_agent/ip_route.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/procustodibus_agent/mfa/
--rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.3.2/procustodibus_agent/mfa/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.2/procustodibus_agent/mfa/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.3.2/procustodibus_agent/mfa/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.3.2/procustodibus_agent/resolve_hostname.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.3.2/procustodibus_agent/wg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    12981 2022-08-15 19:42:34.000000 procustodibus_agent-1.3.2/procustodibus_agent/wg_cnf.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/
--rw-rw-r--   0 justin    (1000) justin    (1000)     4657 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)      919 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      187 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      671 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       20 2023-03-17 01:04:21.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.3.2/procustodibus_agent.egg-info/zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)       92 2022-09-26 02:20:41.000000 procustodibus_agent-1.3.2/pyproject.toml
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/requirements/
--rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.3.2/requirements/dev.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.2/requirements/lint.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       82 2023-03-16 01:04:31.000000 procustodibus_agent-1.3.2/requirements/prod.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.3.2/requirements/test.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      811 2023-03-17 01:04:21.144556 procustodibus_agent-1.3.2/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)     2144 2023-03-17 00:35:08.000000 procustodibus_agent-1.3.2/setup.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2023-03-17 00:35:06.000000 procustodibus_agent-1.3.3/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.3.3/MANIFEST.in
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4657 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3524 2023-03-17 00:35:08.000000 procustodibus_agent-1.3.3/README.md
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-28 00:35:05.651759 procustodibus_agent-1.3.3/procustodibus_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      200 2023-05-28 00:06:44.000000 procustodibus_agent-1.3.3/procustodibus_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2893 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.3/procustodibus_agent/agent.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    10924 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.3/procustodibus_agent/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1895 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.3/procustodibus_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    14687 2022-09-26 02:23:07.000000 procustodibus_agent-1.3.3/procustodibus_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5411 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.3/procustodibus_agent/connectivity.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.3.3/procustodibus_agent/credentials.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    40359 2022-02-24 02:03:11.000000 procustodibus_agent-1.3.3/procustodibus_agent/executor.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3259 2021-11-12 03:42:31.000000 procustodibus_agent-1.3.3/procustodibus_agent/ip_route.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/procustodibus_agent/mfa/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.3.3/procustodibus_agent/mfa/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.3/procustodibus_agent/mfa/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.3.3/procustodibus_agent/mfa/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.3.3/procustodibus_agent/resolve_hostname.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.3.3/procustodibus_agent/wg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    12981 2022-08-15 19:42:34.000000 procustodibus_agent-1.3.3/procustodibus_agent/wg_cnf.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4657 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)      919 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      187 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      671 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       20 2023-05-28 00:35:05.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.3.3/procustodibus_agent.egg-info/zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)       92 2022-09-26 02:20:41.000000 procustodibus_agent-1.3.3/pyproject.toml
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/requirements/
+-rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.3.3/requirements/dev.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.3.3/requirements/lint.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       82 2023-03-16 01:04:31.000000 procustodibus_agent-1.3.3/requirements/prod.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.3.3/requirements/test.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      811 2023-05-28 00:35:05.655766 procustodibus_agent-1.3.3/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2144 2023-03-17 00:35:08.000000 procustodibus_agent-1.3.3/setup.py
```

### Comparing `procustodibus_agent-1.3.2/LICENSE` & `procustodibus_agent-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/PKG-INFO` & `procustodibus_agent-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.3.2
+Version: 1.3.3
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
```

### Comparing `procustodibus_agent-1.3.2/README.md` & `procustodibus_agent-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/agent.py` & `procustodibus_agent-1.3.3/procustodibus_agent/agent.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/api.py` & `procustodibus_agent-1.3.3/procustodibus_agent/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/cli.py` & `procustodibus_agent-1.3.3/procustodibus_agent/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/cnf.py` & `procustodibus_agent-1.3.3/procustodibus_agent/cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/connectivity.py` & `procustodibus_agent-1.3.3/procustodibus_agent/connectivity.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/credentials.py` & `procustodibus_agent-1.3.3/procustodibus_agent/credentials.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/executor.py` & `procustodibus_agent-1.3.3/procustodibus_agent/executor.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/ip_route.py` & `procustodibus_agent-1.3.3/procustodibus_agent/ip_route.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/mfa/__init__.py` & `procustodibus_agent-1.3.3/procustodibus_agent/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/mfa/api.py` & `procustodibus_agent-1.3.3/procustodibus_agent/mfa/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/mfa/cli.py` & `procustodibus_agent-1.3.3/procustodibus_agent/mfa/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/resolve_hostname.py` & `procustodibus_agent-1.3.3/procustodibus_agent/resolve_hostname.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/wg.py` & `procustodibus_agent-1.3.3/procustodibus_agent/wg.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent/wg_cnf.py` & `procustodibus_agent-1.3.3/procustodibus_agent/wg_cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent.egg-info/PKG-INFO` & `procustodibus_agent-1.3.3/procustodibus_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus-agent
-Version: 1.3.2
+Version: 1.3.3
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
```

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent.egg-info/SOURCES.txt` & `procustodibus_agent-1.3.3/procustodibus_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/procustodibus_agent.egg-info/requires.txt` & `procustodibus_agent-1.3.3/procustodibus_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/requirements/lint.txt` & `procustodibus_agent-1.3.3/requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/setup.cfg` & `procustodibus_agent-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.3.2/setup.py` & `procustodibus_agent-1.3.3/setup.py`

 * *Files identical despite different names*

