# Comparing `tmp/asphalt-4.9.0.tar.gz` & `tmp/asphalt-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphalt-4.9.0.tar", last modified: Sat May 21 22:29:45 2022, max compression
+gzip compressed data, was "asphalt-4.9.1.tar", last modified: Sun May 22 13:42:25 2022, max compression
```

## Comparing `asphalt-4.9.0.tar` & `asphalt-4.9.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-21 22:29:33.000000 asphalt-4.9.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-05-21 22:29:33.000000 asphalt-4.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-21 22:29:33.000000 asphalt-4.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-05-21 22:29:33.000000 asphalt-4.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-21 22:29:33.000000 asphalt-4.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-21 22:29:33.000000 asphalt-4.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-05-21 22:29:45.701951 asphalt-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-21 22:29:33.000000 asphalt-4.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/acknowledgements.rst
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/modules/component.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/modules/context.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/modules/event.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/modules/runner.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/modules/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/tutorials/echo.rst
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19354 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/tutorials/webnotifier.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/components.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/concurrency.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10474 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/events.rst
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/userguide/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13236 2022-05-21 22:29:33.000000 asphalt-4.9.0/docs/versionhistory.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/examples/tutorial1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/examples/tutorial1/echo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial1/echo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial1/echo/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial1/echo/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/examples/tutorial1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial1/tests/test_client_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/examples/tutorial2/
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial2/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/examples/tutorial2/webnotifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial2/webnotifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial2/webnotifier/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-21 22:29:33.000000 asphalt-4.9.0/examples/tutorial2/webnotifier/detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-05-21 22:29:33.000000 asphalt-4.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-21 22:29:45.701951 asphalt-4.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.697951 asphalt-4.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/src/asphalt/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/src/asphalt/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6936 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/component.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    39264 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    11208 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/event.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-05-21 22:29:33.000000 asphalt-4.9.0/src/asphalt/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/src/asphalt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-21 22:29:45.000000 asphalt-4.9.0/src/asphalt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 22:29:45.701951 asphalt-4.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12245 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    34408 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_context_py38.py
--rw-r--r--   0 runner    (1001) docker     (121)     9071 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     9397 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2022-05-21 22:29:33.000000 asphalt-4.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-22 13:42:10.000000 asphalt-4.9.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-05-22 13:42:10.000000 asphalt-4.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-22 13:42:10.000000 asphalt-4.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-05-22 13:42:10.000000 asphalt-4.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-22 13:42:10.000000 asphalt-4.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-22 13:42:10.000000 asphalt-4.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-05-22 13:42:25.795328 asphalt-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-22 13:42:10.000000 asphalt-4.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/acknowledgements.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/modules/component.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/modules/context.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/modules/event.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/modules/runner.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/modules/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/tutorials/echo.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    19354 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/tutorials/webnotifier.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/components.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/concurrency.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10474 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/events.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/userguide/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13347 2022-05-22 13:42:10.000000 asphalt-4.9.1/docs/versionhistory.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/examples/tutorial1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/examples/tutorial1/echo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial1/echo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial1/echo/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial1/echo/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/examples/tutorial1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial1/tests/test_client_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/examples/tutorial2/
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/examples/tutorial2/webnotifier/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial2/webnotifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial2/webnotifier/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-22 13:42:10.000000 asphalt-4.9.1/examples/tutorial2/webnotifier/detector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-05-22 13:42:10.000000 asphalt-4.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-22 13:42:25.795328 asphalt-4.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.791327 asphalt-4.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/src/asphalt/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/src/asphalt/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6936 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39821 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11208 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7243 2022-05-22 13:42:10.000000 asphalt-4.9.1/src/asphalt/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/src/asphalt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-22 13:42:25.000000 asphalt-4.9.1/src/asphalt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 13:42:25.795328 asphalt-4.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12245 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34408 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_context_py38.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9071 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9397 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5317 2022-05-22 13:42:10.000000 asphalt-4.9.1/tests/test_utils.py
```

### Comparing `asphalt-4.9.0/.github/workflows/publish.yml` & `asphalt-4.9.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/.github/workflows/test.yml` & `asphalt-4.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/.pre-commit-config.yaml` & `asphalt-4.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/LICENSE` & `asphalt-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/PKG-INFO` & `asphalt-4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asphalt
-Version: 4.9.0
+Version: 4.9.1
 Summary: A microframework for network oriented applications
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Component projects, https://github.com/asphalt-framework
 Project-URL: Documentation, https://asphalt.readthedocs.org/en/latest/
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt
```

### Comparing `asphalt-4.9.0/README.rst` & `asphalt-4.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/conf.py` & `asphalt-4.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/index.rst` & `asphalt-4.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/tutorials/echo.rst` & `asphalt-4.9.1/docs/tutorials/echo.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/tutorials/webnotifier.rst` & `asphalt-4.9.1/docs/tutorials/webnotifier.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/architecture.rst` & `asphalt-4.9.1/docs/userguide/architecture.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/components.rst` & `asphalt-4.9.1/docs/userguide/components.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/concurrency.rst` & `asphalt-4.9.1/docs/userguide/concurrency.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/contexts.rst` & `asphalt-4.9.1/docs/userguide/contexts.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/deployment.rst` & `asphalt-4.9.1/docs/userguide/deployment.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/events.rst` & `asphalt-4.9.1/docs/userguide/events.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/userguide/testing.rst` & `asphalt-4.9.1/docs/userguide/testing.rst`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/docs/versionhistory.rst` & `asphalt-4.9.1/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
-**UNRELEASED**
+**4.9.1** (2022-05-22)
+
+- Fixed type annotation for ``@context_teardown``
+- Improved type annotations
+
+**4.9.0** (2022-05-22)
 
 - Added ``asphalt.core.get_resources()`` as a top-level shortcut for
   ``current_context().get_resources(...)``
 - Allowed resource retrieval and generation in teardown callbacks until the context has
   been completely closed (this would previously raise
   ``RuntimeError("this context has already been closed")``)
 - Allowed specifying optional dependencies with dependency injection, using either
```

### Comparing `asphalt-4.9.0/examples/tutorial1/echo/client.py` & `asphalt-4.9.1/examples/tutorial1/echo/client.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/examples/tutorial1/echo/server.py` & `asphalt-4.9.1/examples/tutorial1/echo/server.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/examples/tutorial1/tests/test_client_server.py` & `asphalt-4.9.1/examples/tutorial1/tests/test_client_server.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/examples/tutorial2/config.yaml` & `asphalt-4.9.1/examples/tutorial2/config.yaml`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/examples/tutorial2/webnotifier/app.py` & `asphalt-4.9.1/examples/tutorial2/webnotifier/app.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/examples/tutorial2/webnotifier/detector.py` & `asphalt-4.9.1/examples/tutorial2/webnotifier/detector.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/pyproject.toml` & `asphalt-4.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/__init__.py` & `asphalt-4.9.1/src/asphalt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/cli.py` & `asphalt-4.9.1/src/asphalt/core/cli.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/component.py` & `asphalt-4.9.1/src/asphalt/core/component.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/concurrent.py` & `asphalt-4.9.1/src/asphalt/core/concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             try:
                 loop = get_running_loop()
             except RuntimeError:
                 # Event loop not available -- we're in a worker thread
                 return func(ctx, *args, **kwargs)
 
             # Resolve the executor resource name to an Executor instance
+            _executor: Executor | None
             if isinstance(executor, str):
                 _executor = ctx.require_resource(Executor, executor)
             else:
                 _executor = executor
 
             callback = partial(func, ctx, *args, **kwargs)
             return loop.run_in_executor(_executor, callback)
```

### Comparing `asphalt-4.9.0/src/asphalt/core/context.py` & `asphalt-4.9.1/src/asphalt/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 logger = logging.getLogger(__name__)
 factory_callback_type = Callable[["Context"], Any]
 resource_name_re = re.compile(r"\w+")
 T_Resource = TypeVar("T_Resource")
 T_Retval = TypeVar("T_Retval")
 T_Context = TypeVar("T_Context", bound="Context")
+T_Self = TypeVar("T_Self")
 P = ParamSpec("P")
 _current_context: ContextVar[Context | None] = ContextVar(
     "_current_context", default=None
 )
 
 
 class ResourceContainer:
@@ -107,42 +108,42 @@
     :ivar bool is_factory: ``True`` if ``value_or_factory`` if this is a resource factory
     """
 
     __slots__ = "value_or_factory", "types", "name", "context_attr", "is_factory"
 
     def __init__(
         self,
-        value_or_factory,
+        value_or_factory: Any,
         types: Tuple[type, ...],
         name: str,
         context_attr: Optional[str],
         is_factory: bool,
     ) -> None:
         self.value_or_factory = value_or_factory
         self.types = types
         self.name = name
         self.context_attr = context_attr
         self.is_factory = is_factory
 
-    def generate_value(self, ctx: Context):
+    def generate_value(self, ctx: Context) -> Any:
         assert self.is_factory, "generate_value() only works for resource factories"
         value = self.value_or_factory(ctx)
 
         container = ResourceContainer(
             value, self.types, self.name, self.context_attr, False
         )
         for type_ in self.types:
             ctx._resources[(type_, self.name)] = container
 
         if self.context_attr:
             setattr(ctx, self.context_attr, value)
 
         return value
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         typenames = ", ".join(qualified_name(cls) for cls in self.types)
         value_repr = (
             "factory=%s" % callable_name(self.value_or_factory)
             if self.is_factory
             else "value=%r" % self.value_or_factory
         )
         return (
@@ -868,17 +869,34 @@
     if isinstance(arg, str):
         resource_name = arg
         return outer_wrapper
 
     return asyncio_extras.threadpool(arg)
 
 
+@overload
 def context_teardown(
     func: Callable[[T_Context], AsyncGenerator[None, Exception | None]]
-) -> Callable[[T_Context], Coroutine]:
+) -> Callable[[T_Context], Coroutine[Any, Any, None]]:
+    ...
+
+
+@overload
+def context_teardown(
+    func: Callable[[T_Self, T_Context], AsyncGenerator[None, Exception | None]]
+) -> Callable[[T_Self, T_Context], Coroutine[Any, Any, None]]:
+    ...
+
+
+def context_teardown(
+    func: Callable[[T_Context], AsyncGenerator[None, Exception | None]]
+    | Callable[[T_Self, T_Context], AsyncGenerator[None, Exception | None]]
+) -> Callable[[T_Context], Coroutine[Any, Any, None]] | Callable[
+    [T_Self, T_Context], Coroutine[Any, Any, None]
+]:
     """
     Wrap an async generator function to execute the rest of the function at context teardown.
 
     This function returns an async function, which, when called, starts the wrapped async
     generator. The wrapped async function is run until the first ``yield`` statement
     When the context is being torn down, the exception that ended the context, if any, is sent to
     the generator.
```

### Comparing `asphalt-4.9.0/src/asphalt/core/event.py` & `asphalt-4.9.1/src/asphalt/core/event.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/runner.py` & `asphalt-4.9.1/src/asphalt/core/runner.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/src/asphalt/core/utils.py` & `asphalt-4.9.1/src/asphalt/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     "merge_config",
     "PluginContainer",
 )
 
 import sys
 from importlib import import_module
 from inspect import isclass
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, overload
 
 from typeguard import check_argument_types
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import EntryPoint, entry_points
 else:
     from importlib_metadata import EntryPoint, entry_points
 
+T_Object = TypeVar("T_Object")
 
-def resolve_reference(ref: Any) -> Any:
+
+def resolve_reference(ref: object) -> Any:
     """
     Return the object pointed to by ``ref``.
 
     If ``ref`` is not a string or does not contain ``:``, it is returned as is.
 
     References must be in the form  <modulename>:<varname> where <modulename> is the fully
     qualified module name and varname is the path to the variable inside that module.
@@ -52,31 +54,29 @@
             obj = getattr(obj, name)
 
         return obj
     except AttributeError:
         raise LookupError(f"error resolving reference {ref}: error looking up object")
 
 
-def qualified_name(obj) -> str:
+def qualified_name(obj: object) -> str:
     """
     Return the qualified name (e.g. package.module.Type) for the given object.
 
     If ``obj`` is not a class, the returned name will match its type instead.
 
     """
-    if not isclass(obj):
-        obj = type(obj)
-
-    if obj.__module__ == "builtins":
-        return obj.__name__
+    cls = obj if isclass(obj) else type(obj)
+    if cls.__module__ == "builtins":
+        return cls.__name__
     else:
-        return f"{obj.__module__}.{obj.__qualname__}"
+        return f"{cls.__module__}.{cls.__qualname__}"
 
 
-def callable_name(func: Callable) -> str:
+def callable_name(func: Callable[..., Any]) -> str:
     """Return the qualified name (e.g. package.module.func) for the given callable."""
     if func.__module__ == "builtins":
         return func.__name__
     else:
         return f"{func.__module__}.{func.__qualname__}"
 
 
@@ -128,15 +128,23 @@
 
     def __init__(self, namespace: str, base_class: type = None) -> None:
         self.namespace = namespace
         self.base_class = base_class
         group = entry_points().select(group=namespace)  # type: ignore[attr-defined]
         self._entrypoints = {ep.name: ep for ep in group}
 
-    def resolve(self, obj):
+    @overload
+    def resolve(self, obj: str) -> Any:
+        pass
+
+    @overload
+    def resolve(self, obj: T_Object) -> T_Object:
+        pass
+
+    def resolve(self, obj: Any) -> Any:
         """
         Resolve a reference to an entry point or a variable in a module.
 
         If ``obj`` is a ``module:varname`` reference to an object, :func:`resolve_reference` is
         used to resolve it. If it is a string of any other kind, the named entry point is loaded
         from this container's namespace. Otherwise, ``obj`` is returned as is.
 
@@ -171,15 +179,15 @@
         :param constructor_kwargs: keyword arguments passed to the constructor of the plugin class
         :return: the plugin instance
 
         """
         assert check_argument_types()
         assert self.base_class, "base class has not been defined"
         plugin_class = self.resolve(type)
-        if not issubclass(plugin_class, self.base_class):
+        if not isclass(plugin_class) or not issubclass(plugin_class, self.base_class):
             raise TypeError(
                 "{} is not a subclass of {}".format(
                     qualified_name(plugin_class), qualified_name(self.base_class)
                 )
             )
 
         return plugin_class(**constructor_kwargs)
```

### Comparing `asphalt-4.9.0/src/asphalt.egg-info/PKG-INFO` & `asphalt-4.9.1/src/asphalt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asphalt
-Version: 4.9.0
+Version: 4.9.1
 Summary: A microframework for network oriented applications
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Component projects, https://github.com/asphalt-framework
 Project-URL: Documentation, https://asphalt.readthedocs.org/en/latest/
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt
```

### Comparing `asphalt-4.9.0/src/asphalt.egg-info/SOURCES.txt` & `asphalt-4.9.1/src/asphalt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_cli.py` & `asphalt-4.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_component.py` & `asphalt-4.9.1/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_concurrent.py` & `asphalt-4.9.1/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_context.py` & `asphalt-4.9.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_event.py` & `asphalt-4.9.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_runner.py` & `asphalt-4.9.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `asphalt-4.9.0/tests/test_utils.py` & `asphalt-4.9.1/tests/test_utils.py`

 * *Files identical despite different names*

