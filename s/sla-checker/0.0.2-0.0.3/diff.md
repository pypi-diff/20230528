# Comparing `tmp/sla_checker-0.0.2.tar.gz` & `tmp/sla_checker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sla_checker-0.0.2.tar", last modified: Tue Dec 17 08:23:26 2019, max compression
+gzip compressed data, was "sla_checker-0.0.3.tar", last modified: Sun May 28 15:36:51 2023, max compression
```

## Comparing `sla_checker-0.0.2.tar` & `sla_checker-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-17 08:23:26.637821 sla_checker-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (115)     2916 2019-12-17 08:23:26.637821 sla_checker-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1857 2019-12-17 08:23:11.000000 sla_checker-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-12-17 08:23:26.637821 sla_checker-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (115)      766 2019-12-17 08:23:11.000000 sla_checker-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-17 08:23:26.637821 sla_checker-0.0.2/sla_checker/
--rw-r--r--   0 runner    (1001) docker     (115)      109 2019-12-17 08:23:11.000000 sla_checker-0.0.2/sla_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6192 2019-12-17 08:23:11.000000 sla_checker-0.0.2/sla_checker/sla_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-17 08:23:26.637821 sla_checker-0.0.2/sla_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     2916 2019-12-17 08:23:26.000000 sla_checker-0.0.2/sla_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      209 2019-12-17 08:23:26.000000 sla_checker-0.0.2/sla_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-17 08:23:26.000000 sla_checker-0.0.2/sla_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       12 2019-12-17 08:23:26.000000 sla_checker-0.0.2/sla_checker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:36:51.477640 sla_checker-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 15:36:48.000000 sla_checker-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-28 15:36:51.477640 sla_checker-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-28 15:36:48.000000 sla_checker-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 15:36:51.477640 sla_checker-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-05-28 15:36:49.000000 sla_checker-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:36:51.477640 sla_checker-0.0.3/sla_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-28 15:36:49.000000 sla_checker-0.0.3/sla_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-28 15:36:48.000000 sla_checker-0.0.3/sla_checker/sla_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:36:51.477640 sla_checker-0.0.3/sla_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 15:36:51.000000 sla_checker-0.0.3/sla_checker.egg-info/top_level.txt
```

### Comparing `sla_checker-0.0.2/README.md` & `sla_checker-0.0.3/README.md`

 * *Files identical despite different names*

