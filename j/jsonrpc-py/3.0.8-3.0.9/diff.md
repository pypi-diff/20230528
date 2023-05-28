# Comparing `tmp/jsonrpc-py-3.0.8.tar.gz` & `tmp/jsonrpc-py-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.8.tar", last modified: Sat May  6 14:57:44 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.9.tar", last modified: Sun May 28 11:12:51 2023, max compression
```

## Comparing `jsonrpc-py-3.0.8.tar` & `jsonrpc-py-3.0.9.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.445853 jsonrpc-py-3.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     2899 2023-05-06 14:57:44.444853 jsonrpc-py-3.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.421851 jsonrpc-py-3.0.8/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.414850 jsonrpc-py-3.0.8/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.424851 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.432852 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.435852 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.439853 jsonrpc-py-3.0.8/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9422 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     4098 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.441853 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2899 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2021 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1834 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 14:57:44.445853 jsonrpc-py-3.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.444853 jsonrpc-py-3.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     5630 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.009646 jsonrpc-py-3.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-05-28 11:12:51.008646 jsonrpc-py-3.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.996646 jsonrpc-py-3.0.9/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.993646 jsonrpc-py-3.0.9/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.997646 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.002646 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.004646 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.006646 jsonrpc-py-3.0.9/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9422 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4098 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.007646 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 11:12:51.009646 jsonrpc-py-3.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.008646 jsonrpc-py-3.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.8/.gitlab-ci.yml` & `jsonrpc-py-3.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/LICENSE` & `jsonrpc-py-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/Makefile` & `jsonrpc-py-3.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/PKG-INFO` & `jsonrpc-py-3.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.8
+Version: 3.0.9
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
@@ -24,14 +24,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: ujson
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
```

### Comparing `jsonrpc-py-3.0.8/README.md` & `jsonrpc-py-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/changelog.rst` & `jsonrpc-py-3.0.9/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/conf.py` & `jsonrpc-py-3.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/deployment.rst` & `jsonrpc-py-3.0.9/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/index.rst` & `jsonrpc-py-3.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/quickstart.rst` & `jsonrpc-py-3.0.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/docs/reference.rst` & `jsonrpc-py-3.0.9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/__init__.py` & `jsonrpc-py-3.0.9/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/asgi.py` & `jsonrpc-py-3.0.9/jsonrpc/asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.9/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/errors.py` & `jsonrpc-py-3.0.9/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/request.py` & `jsonrpc-py-3.0.9/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/response.py` & `jsonrpc-py-3.0.9/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/serializer.py` & `jsonrpc-py-3.0.9/jsonrpc/serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,23 @@
-from json import dumps as json_dumps, loads as json_loads
+from functools import partial
 from typing import Any, Final
 
 from .errors import Error, ErrorEnum
 
+try:
+    from ujson import dumps as _ujson_dumps, loads as _ujson_loads
+
+    dumps = partial(_ujson_dumps, ensure_ascii=False, escape_forward_slashes=False)
+    loads = partial(_ujson_loads)
+except ImportError:  # pragma: no cover
+    from json import dumps as _json_dumps, loads as _json_loads
+
+    dumps = partial(_json_dumps, ensure_ascii=False, separators=(",", ":"))
+    loads = partial(_json_loads)
+
 __all__: Final[tuple[str, ...]] = ("JSONSerializer",)
 
 
 class JSONSerializer:
     """
     Simple class for JSON serialization and deserialization.
     """
@@ -21,23 +32,23 @@
         Returns the JSON representation of a value.
 
         :param obj: An any type of object that must be JSON serializable.
         :raises jsonrpc.Error: If any exception has occurred due the serialization or/and encoding to :py:class:`bytes`.
         :returns: The :py:class:`bytes` object containing the serialized Python data structure.
         """
         try:
-            return json_dumps(obj, ensure_ascii=True, separators=(",", ":")).encode("ascii")
+            return dumps(obj).encode("utf-8")
         except Exception as exc:
             raise Error(code=ErrorEnum.PARSE_ERROR, message="Failed to serialize object to JSON") from exc
 
     def deserialize(self, obj: bytes, /) -> Any:
         """
         Returns the value encoded in JSON in appropriate Python type.
 
         :param obj: The :py:class:`bytes` object containing the serialized JSON document.
         :raises jsonrpc.Error: If any exception has occurred due the deserialization or/and decoding from :py:class:`bytes`.
         :returns: An any type of object containing the deserialized Python data structure.
         """
         try:
-            return json_loads(obj)
+            return loads(obj)
         except Exception as exc:
             raise Error(code=ErrorEnum.PARSE_ERROR, message="Failed to deserialize object from JSON") from exc
```

### Comparing `jsonrpc-py-3.0.8/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.9/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc/utilities.py` & `jsonrpc-py-3.0.9/jsonrpc/utilities.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.9/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.8
+Version: 3.0.9
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
@@ -24,14 +24,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: ujson
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
```

### Comparing `jsonrpc-py-3.0.8/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.9/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,27 +49,29 @@
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
 docs/changelog/v3.x.x/v3.0.5.rst
 docs/changelog/v3.x.x/v3.0.6.rst
 docs/changelog/v3.x.x/v3.0.7.rst
 docs/changelog/v3.x.x/v3.0.8.rst
+docs/changelog/v3.x.x/v3.0.9.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
 jsonrpc/serializer.py
 jsonrpc/typedefs.py
 jsonrpc/utilities.py
 jsonrpc_py.egg-info/PKG-INFO
 jsonrpc_py.egg-info/SOURCES.txt
 jsonrpc_py.egg-info/dependency_links.txt
+jsonrpc_py.egg-info/requires.txt
 jsonrpc_py.egg-info/top_level.txt
 tests/__init__.py
 tests/test_asgi.py
 tests/test_dispatcher.py
 tests/test_errors.py
 tests/test_request.py
 tests/test_response.py
```

### Comparing `jsonrpc-py-3.0.8/pyproject.toml` & `jsonrpc-py-3.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 [project.urls]
 "Homepage" = "https://docs.jsonrpc.ru"
 "Source Code" = "https://gitlab.com/jsonrpc/jsonrpc-py"
 "Documentation" = "https://docs.jsonrpc.ru"
 "Change Log" = "https://docs.jsonrpc.ru/changelog.html"
 
+[project.optional-dependencies]
+ujson = ["ujson"]
+
 [tool.black]
 line_length = 140
 preview = true
 
 [tool.isort]
 profile = "black"
 combine_as_imports = true
```

### Comparing `jsonrpc-py-3.0.8/tests/test_asgi.py` & `jsonrpc-py-3.0.9/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_dispatcher.py` & `jsonrpc-py-3.0.9/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_errors.py` & `jsonrpc-py-3.0.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_request.py` & `jsonrpc-py-3.0.9/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_response.py` & `jsonrpc-py-3.0.9/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_serializer.py` & `jsonrpc-py-3.0.9/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.8/tests/test_utilities.py` & `jsonrpc-py-3.0.9/tests/test_utilities.py`

 * *Files identical despite different names*

