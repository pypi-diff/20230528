# Comparing `tmp/hg-loggingmod-0.2.1.tar.gz` & `tmp/hg-loggingmod-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hg-loggingmod-0.2.1.tar", last modified: Sun May 28 14:17:18 2023, max compression
+gzip compressed data, was "hg-loggingmod-0.3.0.tar", last modified: Mon Oct 25 21:13:03 2021, max compression
```

## Comparing `hg-loggingmod-0.2.1.tar` & `hg-loggingmod-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-05-28 14:17:18.994328 hg-loggingmod-0.2.1/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2019-10-10 08:42:38.000000 hg-loggingmod-0.2.1/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       34 2020-03-25 23:00:30.000000 hg-loggingmod-0.2.1/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4973 2023-05-28 14:17:18.993328 hg-loggingmod-0.2.1/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4613 2020-06-21 19:09:56.000000 hg-loggingmod-0.2.1/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-05-28 14:17:18.993328 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4973 2023-05-28 14:17:18.000000 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      366 2023-05-28 14:17:18.000000 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2023-05-28 14:17:18.000000 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       10 2023-05-28 14:17:18.000000 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        9 2023-05-28 14:17:18.000000 hg-loggingmod-0.2.1/hg_loggingmod.egg-info/top_level.txt
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-05-28 14:17:18.993328 hg-loggingmod-0.2.1/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2020-03-25 23:38:02.000000 hg-loggingmod-0.2.1/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-05-28 14:17:18.993328 hg-loggingmod-0.2.1/hgext3rd/loggingmod/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8160 2023-05-28 13:09:41.000000 hg-loggingmod-0.2.1/hgext3rd/loggingmod/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      840 2020-06-21 18:58:04.000000 hg-loggingmod-0.2.1/hgext3rd/loggingmod/config.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1883 2020-06-21 18:58:04.000000 hg-loggingmod-0.2.1/hgext3rd/loggingmod/sentry.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2023-05-28 14:16:50.000000 hg-loggingmod-0.2.1/hgext3rd/loggingmod/version.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2023-05-28 14:17:18.994328 hg-loggingmod-0.2.1/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      862 2020-06-21 19:09:56.000000 hg-loggingmod-0.2.1/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       34 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6278 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4613 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6278 2021-10-25 21:13:03.000000 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      366 2021-10-25 21:13:03.000000 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2021-10-25 21:13:03.000000 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       10 2021-10-25 21:13:03.000000 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        9 2021-10-25 21:13:03.000000 hg-loggingmod-0.3.0/hg_loggingmod.egg-info/top_level.txt
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/hgext3rd/loggingmod/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8172 2021-10-25 16:31:36.000000 hg-loggingmod-0.3.0/hgext3rd/loggingmod/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      840 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/hgext3rd/loggingmod/config.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1883 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/hgext3rd/loggingmod/sentry.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2021-10-25 21:12:27.000000 hg-loggingmod-0.3.0/hgext3rd/loggingmod/version.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2021-10-25 21:13:03.179855 hg-loggingmod-0.3.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      862 2021-10-25 09:41:43.000000 hg-loggingmod-0.3.0/setup.py
```

### Comparing `hg-loggingmod-0.2.1/LICENSE` & `hg-loggingmod-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hg-loggingmod-0.2.1/PKG-INFO` & `hg-loggingmod-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: hg-loggingmod
-Version: 0.2.1
-Summary: Managing Mercurial logs with the standard Python logging module
-Home-page: https://dev.heptapod.net/heptapod/hgext-loggingmod
-Author: Georges Racinet
-Author-email: georges.racinet@octobus.net
-License: GPLv2+
-Keywords: hg mercurial
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mercurial logs through the `logging` module
 
 This extension redirects most user feedback meant for terminals to the
 Python `logging` module of the standard library.
 
 This is intended intended primarily for server-side use cases, and is unlikely
 to be useful for client-side operation.
```

### Comparing `hg-loggingmod-0.2.1/hgext3rd/loggingmod/__init__.py` & `hg-loggingmod-0.3.0/hgext3rd/loggingmod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
                 datefmt=datefmt)
     )
     hg_handler.addFilter(MissingRepoFilter())
     hg_logger.addHandler(hg_handler)
 
     jsonconf = ui.config(CONFIG_SECTION, b'config.json', default=None)
     logger.info("jsonconf=%r", jsonconf)
-    if jsonconf:
+    if jsonconf is not None:
         with open(jsonconf) as conffile:
             conf_dict = json.load(conffile)
         logging.config.dictConfig(conf_dict)
 
     iniconf = ui.config(CONFIG_SECTION, b'config.ini', default=None)
     if iniconf is not None:
         logging.config.fileConfig(iniconf)
```

### Comparing `hg-loggingmod-0.2.1/hgext3rd/loggingmod/config.py` & `hg-loggingmod-0.3.0/hgext3rd/loggingmod/config.py`

 * *Files identical despite different names*

### Comparing `hg-loggingmod-0.2.1/hgext3rd/loggingmod/sentry.py` & `hg-loggingmod-0.3.0/hgext3rd/loggingmod/sentry.py`

 * *Files identical despite different names*

### Comparing `hg-loggingmod-0.2.1/setup.py` & `hg-loggingmod-0.3.0/setup.py`

 * *Files identical despite different names*

